# Comparing `tmp/ado_wrapper-1.7.0.tar.gz` & `tmp/ado_wrapper-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ado_wrapper-1.7.0.tar", max compression
+gzip compressed data, was "ado_wrapper-1.7.1.tar", max compression
```

## Comparing `ado_wrapper-1.7.0.tar` & `ado_wrapper-1.7.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-1.7.0/LICENSE
--rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-1.7.0/README.md
--rw-r--r--   0        0        0      118 2024-04-20 14:42:40.460346 ado_wrapper-1.7.0/ado_wrapper/__init__.py
--rw-r--r--   0        0        0     6516 2024-04-21 14:56:46.791401 ado_wrapper-1.7.0/ado_wrapper/__main__.py
--rw-r--r--   0        0        0     2325 2024-05-03 16:43:39.046186 ado_wrapper-1.7.0/ado_wrapper/client.py
--rw-r--r--   0        0        0    25691 2024-04-21 11:28:27.535399 ado_wrapper-1.7.0/ado_wrapper/dumps.py
--rw-r--r--   0        0        0     3427 2024-05-04 17:24:03.055237 ado_wrapper-1.7.0/ado_wrapper/generate_docs.py
--rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-1.7.0/ado_wrapper/plan_resources/__init__.py
--rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-1.7.0/ado_wrapper/plan_resources/colours.py
--rw-r--r--   0        0        0      296 2024-04-21 14:56:46.792465 ado_wrapper-1.7.0/ado_wrapper/plan_resources/mapping.py
--rw-r--r--   0        0        0     1067 2024-04-21 14:56:46.792911 ado_wrapper-1.7.0/ado_wrapper/plan_resources/plan_repo.py
--rw-r--r--   0        0        0     1820 2024-04-21 14:56:46.793288 ado_wrapper-1.7.0/ado_wrapper/plan_resources/plan_resource.py
--rw-r--r--   0        0        0      809 2024-04-23 08:39:40.317360 ado_wrapper-1.7.0/ado_wrapper/plan_resources/plan_state_manager.py
--rw-r--r--   0        0        0     1173 2024-05-05 12:45:05.895693 ado_wrapper-1.7.0/ado_wrapper/resources/__init__.py
--rw-r--r--   0        0        0     3759 2024-05-06 09:45:35.252086 ado_wrapper-1.7.0/ado_wrapper/resources/agent_pools.py
--rw-r--r--   0        0        0     4763 2024-04-24 08:14:16.703798 ado_wrapper-1.7.0/ado_wrapper/resources/annotated_tags.py
--rw-r--r--   0        0        0     3387 2024-04-22 11:52:18.509396 ado_wrapper-1.7.0/ado_wrapper/resources/branches.py
--rw-r--r--   0        0        0    14870 2024-05-03 16:42:18.453223 ado_wrapper-1.7.0/ado_wrapper/resources/builds.py
--rw-r--r--   0        0        0     6621 2024-05-03 16:39:20.096468 ado_wrapper-1.7.0/ado_wrapper/resources/commits.py
--rw-r--r--   0        0        0     7397 2024-04-23 08:38:52.950096 ado_wrapper-1.7.0/ado_wrapper/resources/environment.py
--rw-r--r--   0        0        0     3308 2024-04-21 14:56:46.796388 ado_wrapper-1.7.0/ado_wrapper/resources/groups.py
--rw-r--r--   0        0        0    15327 2024-05-03 16:42:42.079759 ado_wrapper-1.7.0/ado_wrapper/resources/merge_policies.py
--rw-r--r--   0        0        0     2135 2024-05-02 08:38:58.564678 ado_wrapper-1.7.0/ado_wrapper/resources/projects.py
--rw-r--r--   0        0        0    14012 2024-05-03 16:42:47.416430 ado_wrapper-1.7.0/ado_wrapper/resources/pull_requests.py
--rw-r--r--   0        0        0    12487 2024-04-21 14:56:46.797975 ado_wrapper-1.7.0/ado_wrapper/resources/releases.py
--rw-r--r--   0        0        0    10450 2024-05-05 11:05:13.008884 ado_wrapper-1.7.0/ado_wrapper/resources/repo.py
--rw-r--r--   0        0        0    10546 2024-05-05 18:52:57.391256 ado_wrapper-1.7.0/ado_wrapper/resources/repo_user_permission.py
--rw-r--r--   0        0        0     2853 2024-04-29 16:33:17.512344 ado_wrapper-1.7.0/ado_wrapper/resources/searches.py
--rw-r--r--   0        0        0     5973 2024-04-23 09:01:01.373067 ado_wrapper-1.7.0/ado_wrapper/resources/service_endpoint.py
--rw-r--r--   0        0        0     4557 2024-04-21 14:56:46.799334 ado_wrapper-1.7.0/ado_wrapper/resources/teams.py
--rw-r--r--   0        0        0     8314 2024-05-04 20:57:42.347047 ado_wrapper-1.7.0/ado_wrapper/resources/users.py
--rw-r--r--   0        0        0     4828 2024-04-21 14:56:46.800092 ado_wrapper-1.7.0/ado_wrapper/resources/variable_groups.py
--rw-r--r--   0        0        0     9459 2024-05-06 09:44:07.348306 ado_wrapper-1.7.0/ado_wrapper/state_managed_abc.py
--rw-r--r--   0        0        0     8129 2024-05-03 16:44:33.762863 ado_wrapper-1.7.0/ado_wrapper/state_manager.py
--rw-r--r--   0        0        0     4929 2024-05-05 09:30:08.198011 ado_wrapper-1.7.0/ado_wrapper/utils.py
--rw-r--r--   0        0        0     2760 2024-05-06 09:50:05.884014 ado_wrapper-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-1.7.1/LICENSE
+-rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-1.7.1/README.md
+-rw-r--r--   0        0        0      118 2024-04-20 14:42:40.460346 ado_wrapper-1.7.1/ado_wrapper/__init__.py
+-rw-r--r--   0        0        0     6516 2024-04-21 14:56:46.791401 ado_wrapper-1.7.1/ado_wrapper/__main__.py
+-rw-r--r--   0        0        0     2325 2024-05-03 16:43:39.046186 ado_wrapper-1.7.1/ado_wrapper/client.py
+-rw-r--r--   0        0        0    21892 2024-05-07 18:26:17.266989 ado_wrapper-1.7.1/ado_wrapper/dumps.py
+-rw-r--r--   0        0        0     3537 2024-05-06 10:01:09.344505 ado_wrapper-1.7.1/ado_wrapper/generate_docs.py
+-rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-1.7.1/ado_wrapper/plan_resources/__init__.py
+-rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-1.7.1/ado_wrapper/plan_resources/colours.py
+-rw-r--r--   0        0        0      296 2024-04-21 14:56:46.792465 ado_wrapper-1.7.1/ado_wrapper/plan_resources/mapping.py
+-rw-r--r--   0        0        0     1067 2024-04-21 14:56:46.792911 ado_wrapper-1.7.1/ado_wrapper/plan_resources/plan_repo.py
+-rw-r--r--   0        0        0     1820 2024-04-21 14:56:46.793288 ado_wrapper-1.7.1/ado_wrapper/plan_resources/plan_resource.py
+-rw-r--r--   0        0        0      809 2024-04-23 08:39:40.317360 ado_wrapper-1.7.1/ado_wrapper/plan_resources/plan_state_manager.py
+-rw-r--r--   0        0        0     1173 2024-05-05 12:45:05.895693 ado_wrapper-1.7.1/ado_wrapper/resources/__init__.py
+-rw-r--r--   0        0        0     3791 2024-05-06 09:59:23.335964 ado_wrapper-1.7.1/ado_wrapper/resources/agent_pools.py
+-rw-r--r--   0        0        0     4763 2024-04-24 08:14:16.703798 ado_wrapper-1.7.1/ado_wrapper/resources/annotated_tags.py
+-rw-r--r--   0        0        0     3387 2024-04-22 11:52:18.509396 ado_wrapper-1.7.1/ado_wrapper/resources/branches.py
+-rw-r--r--   0        0        0    15269 2024-05-06 13:26:32.155840 ado_wrapper-1.7.1/ado_wrapper/resources/builds.py
+-rw-r--r--   0        0        0     6621 2024-05-03 16:39:20.096468 ado_wrapper-1.7.1/ado_wrapper/resources/commits.py
+-rw-r--r--   0        0        0     7397 2024-04-23 08:38:52.950096 ado_wrapper-1.7.1/ado_wrapper/resources/environment.py
+-rw-r--r--   0        0        0     3268 2024-05-07 17:20:44.533690 ado_wrapper-1.7.1/ado_wrapper/resources/groups.py
+-rw-r--r--   0        0        0    15678 2024-05-07 19:06:41.212391 ado_wrapper-1.7.1/ado_wrapper/resources/merge_policies.py
+-rw-r--r--   0        0        0     2135 2024-05-02 08:38:58.564678 ado_wrapper-1.7.1/ado_wrapper/resources/projects.py
+-rw-r--r--   0        0        0    14012 2024-05-06 16:33:39.036236 ado_wrapper-1.7.1/ado_wrapper/resources/pull_requests.py
+-rw-r--r--   0        0        0    12487 2024-04-21 14:56:46.797975 ado_wrapper-1.7.1/ado_wrapper/resources/releases.py
+-rw-r--r--   0        0        0    10768 2024-05-07 11:42:12.821826 ado_wrapper-1.7.1/ado_wrapper/resources/repo.py
+-rw-r--r--   0        0        0    10723 2024-05-06 10:05:11.748381 ado_wrapper-1.7.1/ado_wrapper/resources/repo_user_permission.py
+-rw-r--r--   0        0        0     2853 2024-04-29 16:33:17.512344 ado_wrapper-1.7.1/ado_wrapper/resources/searches.py
+-rw-r--r--   0        0        0     5973 2024-04-23 09:01:01.373067 ado_wrapper-1.7.1/ado_wrapper/resources/service_endpoint.py
+-rw-r--r--   0        0        0     4557 2024-04-21 14:56:46.799334 ado_wrapper-1.7.1/ado_wrapper/resources/teams.py
+-rw-r--r--   0        0        0     8326 2024-05-07 18:19:31.197732 ado_wrapper-1.7.1/ado_wrapper/resources/users.py
+-rw-r--r--   0        0        0     4828 2024-04-21 14:56:46.800092 ado_wrapper-1.7.1/ado_wrapper/resources/variable_groups.py
+-rw-r--r--   0        0        0     9459 2024-05-06 09:44:07.348306 ado_wrapper-1.7.1/ado_wrapper/state_managed_abc.py
+-rw-r--r--   0        0        0     8129 2024-05-03 16:44:33.762863 ado_wrapper-1.7.1/ado_wrapper/state_manager.py
+-rw-r--r--   0        0        0     4929 2024-05-05 09:30:08.198011 ado_wrapper-1.7.1/ado_wrapper/utils.py
+-rw-r--r--   0        0        0     2760 2024-05-07 19:07:19.557317 ado_wrapper-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-1.7.1/PKG-INFO
```

### Comparing `ado_wrapper-1.7.0/LICENSE` & `ado_wrapper-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.0/README.md` & `ado_wrapper-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.0/ado_wrapper/__main__.py` & `ado_wrapper-1.7.1/ado_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.0/ado_wrapper/client.py` & `ado_wrapper-1.7.1/ado_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.0/ado_wrapper/dumps.py` & `ado_wrapper-1.7.1/ado_wrapper/dumps.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,17 +159,17 @@
     'dataProviders': {
         'ms.vss-web.component-data': {}, 'ms.vss-web.shared-data': None, 'ms.vss-code-web.branch-policies-data-provider': {
             'identities': "<Member>", 'supportServicePrincipals': True, 'isEditable': True, 'buildDefinitions': None, 'recentStatuses': None,
             'policyGroups': {'{policy_id_uuid}': {
                              'currentScopePolicies': [{'createdBy': "<Member>", 'createdDate': '/Date(1712832031819)/',
                                                        'isEnabled': True, 'isBlocking': True, 'isDeleted': False, 'settings': {'minimumApproverCount': 1, 'creatorVoteCounts': False, 'allowDownvotes': False, 'resetOnSourcePush': False, 'requireVoteOnLastIteration': False, 'resetRejectionsOnSourcePush': False, 'blockLastPusherVote': True, 'requireVoteOnEachIteration': False, 'scope': [{'refName': 'refs/heads/main', 'matchKind': 'Exact', 'repositoryId': '{repo_id}'}]}, 'isEnterpriseManaged': False, '_links': "<links>", 'revision': 13, 'id': 8178, 'url': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/configurations/8178', 'type': {'id': '{policy_id_uuid}', 'url': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/types/{policy_id_uuid}', 'displayName': 'Minimum number of reviewers'}}], 'enterpriseManagedPolicies': None, 
                                                        'inheritedPolicies': [{'createdBy': "<Member>", 'createdDate': '/Date(1710074353140)/', 'isEnabled': True, 'isBlocking': True, 'isDeleted': False, 'settings': {'minimumApproverCount': 1, 'creatorVoteCounts': False, 'allowDownvotes': False, 'resetOnSourcePush': False, 'requireVoteOnLastIteration': False, 'resetRejectionsOnSourcePush': False, 'blockLastPusherVote': False, 'requireVoteOnEachIteration': False, 'scope': [{'refName': None, 'matchKind': 'DefaultBranch', 'repositoryId': None}]}, 'isEnterpriseManaged': False, '_links': {'self': {'href': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/configurations/{config_id}'}, 'policyType': {'href': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/types/{policy_id_uuid}'}}, 'revision': 2, 'id': "{config_id}", 'url': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/configurations/{config_id}', 'type': {'id': '{policy_id_uuid}', 'url': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/types/{policy_id_uuid}', 'displayName': 'Minimum number of reviewers'}}]}, 'c6a1889d-b943-4856-b76f-9e46bb6b0df2': {'currentScopePolicies': None, 'enterpriseManagedPolicies': None,
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          'inheritedPolicies': [{'createdBy': "<Member>", 'createdDate': '/Date(1670239096642)/', 'isEnabled': True, 'isBlocking': True, 'isDeleted': False, 'settings': {'scope': [{'refName': None, 'matchKind': 'DefaultBranch', 'repositoryId': None}]}, 'isEnterpriseManaged': False, '_links': {'self': {'href': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/configurations/40'}, 'policyType': {'href': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/types/c6a1889d-b943-4856-b76f-9e46bb6b0df2'}}, 'revision': 1, 'id': 40, 'url': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/configurations/40', 'type': {'id': 'c6a1889d-b943-4856-b76f-9e46bb6b0df2', 'url': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/types/c6a1889d-b943-4856-b76f-9e46bb6b0df2', 'displayName': 'Comment requirements'}}]},
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          'fd2167ab-b0be-447a-8ec8-39368250530e': {'currentScopePolicies': [{'createdBy': "<Member>", 'createdDate': '/Date(1712766957032)/', 'isEnabled': True, 'isBlocking': True, 'isDeleted': False, 'settings': {'requiredReviewerIds': ['ab35e0e5-b36d-46c4-8d91-714d413e4fae'], 'minimumApproverCount': 1, 'creatorVoteCounts': True, 'scope': [{'refName': 'refs/heads/main', 'matchKind': 'Exact', 'repositoryId': '1aa43e9c-ffca-4388-98b5-59b272a497b8'}]}, 'isEnterpriseManaged': False, '_links': {'self': {'href': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/configurations/8179'}, 'policyType': {'href': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/types/fd2167ab-b0be-447a-8ec8-39368250530e'}}, 'revision': 1, 'id': 8179, 'url': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/configurations/8179', 'type': {'id': 'fd2167ab-b0be-447a-8ec8-39368250530e', 'url': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/types/fd2167ab-b0be-447a-8ec8-39368250530e', 'displayName': 'Required reviewers'}}],
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   'enterpriseManagedPolicies': None, 'inheritedPolicies': None}},
+                                                        'inheritedPolicies': [{'createdBy': "<Member>", 'createdDate': '/Date(1670239096642)/', 'isEnabled': True, 'isBlocking': True, 'isDeleted': False, 'settings': {'scope': [{'refName': None, 'matchKind': 'DefaultBranch', 'repositoryId': None}]}, 'isEnterpriseManaged': False, '_links': {'self': {'href': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/configurations/40'}, 'policyType': {'href': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/types/c6a1889d-b943-4856-b76f-9e46bb6b0df2'}}, 'revision': 1, 'id': 40, 'url': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/configurations/40', 'type': {'id': 'c6a1889d-b943-4856-b76f-9e46bb6b0df2', 'url': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/types/c6a1889d-b943-4856-b76f-9e46bb6b0df2', 'displayName': 'Comment requirements'}}]},
+                                                        'fd2167ab-b0be-447a-8ec8-39368250530e': {'currentScopePolicies': [{'createdBy': "<Member>", 'createdDate': '/Date(1712766957032)/', 'isEnabled': True, 'isBlocking': True, 'isDeleted': False, 'settings': {'requiredReviewerIds': ['ab35e0e5-b36d-46c4-8d91-714d413e4fae'], 'minimumApproverCount': 1, 'creatorVoteCounts': True, 'scope': [{'refName': 'refs/heads/main', 'matchKind': 'Exact', 'repositoryId': '1aa43e9c-ffca-4388-98b5-59b272a497b8'}]}, 'isEnterpriseManaged': False, '_links': {'self': {'href': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/configurations/8179'}, 'policyType': {'href': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/types/fd2167ab-b0be-447a-8ec8-39368250530e'}}, 'revision': 1, 'id': 8179, 'url': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/configurations/8179', 'type': {'id': 'fd2167ab-b0be-447a-8ec8-39368250530e', 'url': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/types/fd2167ab-b0be-447a-8ec8-39368250530e', 'displayName': 'Required reviewers'}}],
+                                                                                                'enterpriseManagedPolicies': None, 'inheritedPolicies': None}},
         }},
 }
 
 SERVICE_ENDPOINT_DUMP = {
     "data": {},
     "id": "{service_endpoint_id}",
     "name": "{service_connection_name}",
```

### Comparing `ado_wrapper-1.7.0/ado_wrapper/generate_docs.py` & `ado_wrapper-1.7.1/ado_wrapper/generate_docs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import inspect
 import re
 
-from ado_wrapper.resources import *
+from ado_wrapper.resources import *  # pylint: disable=W0401,W0614
 
-pattern = re.compile(r'(?<!^)(?=[A-Z])')
+pattern = re.compile(r"(?<!^)(?=[A-Z])")
 ignored_functions = ["get_by_url", "to_json", "from_json", "get_by_abstract_filter", "from_request_payload", "set_lifecycle_policy"]
 string = """
 
 # Examples
 
 All these examples assume an already created AdoClient, perhaps similar to this:
 
@@ -18,16 +18,18 @@
     email, ado_access_token, ado_org, ado_project = file.read().split("\\n")
 
 ado_client = AdoClient(email, ado_access_token, ado_org, ado_project)
 ```
 
 """
 
+
 def pascal_to_snake(string: str) -> str:
-    return pattern.sub('_', string.replace("'", "").strip()).lower().removeprefix("_").replace(" _", " ")
+    return pattern.sub("_", string.replace("'", "").strip()).lower().removeprefix("_").replace(" _", " ")
+
 
 def format_return_type(return_type: str) -> str | None:
     """Returns the value, formatted, and = if it's not None, makes list[`object`] also be called `objects`"""
     return_type = pascal_to_snake(return_type.split(" | ")[0])
     if "." in return_type:
         return_type = return_type.split(".")[-1].removesuffix(">").removeprefix("_")
     if return_type == "str":
@@ -35,47 +37,51 @@
     if return_type.startswith("dict"):
         return "dictionary = "
     if return_type.startswith("none"):
         return ""
     if "state_managed_resource" in return_type:
         return None
     if return_type.startswith("list[_"):
-        return_type = return_type.removeprefix("list[_").removesuffix("]")+"s"
+        return_type = return_type.removeprefix("list[_").removesuffix("]") + "s"
     return f"{return_type} = "
 
+
 def dataclass_attributes(cls) -> list[str]:  # type: ignore[no-untyped-def]
     return [x for x in dir(cls) if x in cls.__dataclass_fields__.keys()]
 
+
 sorted_pairs = dict(sorted({string: value for string, value in globals().items() if string[0].isupper()}.items()))
 
 for class_name, value in sorted_pairs.items():
     # if class_name != "Build":
     #     continue
-    function_data = {key: value for key, value in dict(inspect.getmembers(value)).items()
-                     if not key.startswith("_") and key not in ignored_functions
-                     and key not in dataclass_attributes(globals()[class_name])}
+    function_data = {
+        key: value for key, value in dict(inspect.getmembers(value)).items()
+        if not key.startswith("_") and key not in ignored_functions and 
+        key not in dataclass_attributes(globals()[class_name])  # fmt: skip
+    }
     if not function_data:
         continue
     string += f"-----\n# {class_name}\n<details>\n\n```py\n"
-    for function_name, function_args, in function_data.items():
+    for function_name, function_args in function_data.items():  # fmt: skip
         try:
             signature = inspect.signature(function_args)
-        except TypeError:
+        except TypeError:  # Some random attributes can't be inspected, no worries
             pass
         # =======
         comment = function_name.replace("_", " ").title()
         #
         return_type = format_return_type(str(signature.return_annotation))
         if return_type is None:
             continue
         #
         function_args = [x for x in signature.parameters.keys() if x != "self"]
-        if function_args == ['ado_client', 'update_action', 'url', 'attribute_name', 'attribute_value', 'params']:
+        if function_args == ["ado_client", "update_action", "url", "attribute_name", "attribute_value", "params"]:
             continue  # For things inheritting from update, for the time being before we remap to _update
-        single_args_formatted = [x if i==0 else f"<{x}>" for i, x in enumerate(function_args)]
+        single_args_formatted = [x if i == 0 else f"<{x}>" for i, x in enumerate(function_args)]
         function_args_formatted = ", ".join(single_args_formatted)
         string += f"# {comment}\n{return_type}{class_name if ' = ' in return_type else pascal_to_snake(class_name)}.{function_name}({function_args_formatted})\n\n"
 
     string += "\n```\n</details>\n\n"
 
 with open("examples.md", "w", encoding="utf-8") as file:
     file.write(string.replace("\n\n\n", "\n"))
```

### Comparing `ado_wrapper-1.7.0/ado_wrapper/plan_resources/plan_repo.py` & `ado_wrapper-1.7.1/ado_wrapper/plan_resources/plan_repo.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.0/ado_wrapper/plan_resources/plan_resource.py` & `ado_wrapper-1.7.1/ado_wrapper/plan_resources/plan_resource.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.0/ado_wrapper/plan_resources/plan_state_manager.py` & `ado_wrapper-1.7.1/ado_wrapper/plan_resources/plan_state_manager.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.0/ado_wrapper/resources/__init__.py` & `ado_wrapper-1.7.1/ado_wrapper/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.0/ado_wrapper/resources/agent_pools.py` & `ado_wrapper-1.7.1/ado_wrapper/resources/agent_pools.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,16 +41,18 @@
     def get_by_id(cls, ado_client: AdoClient, agent_pool_id: str) -> AgentPool:
         return super().get_by_url(
             ado_client,
             f"/_apis/distributedtask/pools/{agent_pool_id}?api-version=7.1-preview.1",
         )  # type: ignore[return-value]
 
     @classmethod
-    def create(cls, ado_client: AdoClient, name: str, agent_cloud_id: str | None, auto_provision: bool, auto_size: bool,  # type: ignore[override]
-               auto_update: bool, is_hosted: bool, size: int, target_size: int | None) -> AgentPool:
+    def create(
+        cls, ado_client: AdoClient, name: str, agent_cloud_id: str | None, auto_provision: bool, auto_size: bool,  # type: ignore[override]
+        auto_update: bool, is_hosted: bool, size: int, target_size: int | None  # fmt: skip
+    ) -> AgentPool:
         raise NotImplementedError
         # PAYLOAD = {
         #     "name": name, "agentCloudId": agent_cloud_id, "autoProvision": auto_provision, "autoSize": auto_size,
         #     "autoUpdate": auto_update, "isHosted": is_hosted, "size": size, "targetSize": target_size,
         # }
         # return super().create(
         #     ado_client,
@@ -61,27 +63,27 @@
     # def update(self) -> None:
     #     raise NotImplementedError
     #     # PATCH https://dev.azure.com/{organization}/_apis/distributedtask/pools/{poolId}?api-version=7.1-preview.1
 
     @classmethod
     def delete_by_id(cls, ado_client: AdoClient, agent_pool_id: str) -> None:  # type: ignore[override]
         raise NotImplementedError
-        return super().delete_by_id(
-            ado_client,
-            f"/_apis/distributedtask/pools/{agent_pool_id}?api-version=7.1-preview.1",
-            agent_pool_id
-        )
+        # return super().delete_by_id(
+        #     ado_client,
+        #     f"/_apis/distributedtask/pools/{agent_pool_id}?api-version=7.1-preview.1",
+        #     agent_pool_id
+        # )
 
     @classmethod
     def get_all(cls, ado_client: AdoClient) -> list[AgentPool]:  # type: ignore[override]
         return super().get_all(
             ado_client,
             "/_apis/distributedtask/pools?api-version=7.1-preview.1",
         )  # type: ignore[return-value]
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
     def get_by_name(cls, ado_client: AdoClient, agent_pool_id: str) -> AgentPool | None:
-        return cls.get_by_abstract_filter(ado_client, lambda agent_pool: agent_pool.agent_pool_id==agent_pool_id)  # type: ignore[return-value, attr-defined]
+        return cls.get_by_abstract_filter(ado_client, lambda agent_pool: agent_pool.agent_pool_id == agent_pool_id)  # type: ignore[return-value, attr-defined]
```

### Comparing `ado_wrapper-1.7.0/ado_wrapper/resources/annotated_tags.py` & `ado_wrapper-1.7.1/ado_wrapper/resources/annotated_tags.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.0/ado_wrapper/resources/branches.py` & `ado_wrapper-1.7.1/ado_wrapper/resources/branches.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.0/ado_wrapper/resources/builds.py` & `ado_wrapper-1.7.1/ado_wrapper/resources/builds.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,55 +177,58 @@
 
 @dataclass
 class BuildDefinition(StateManagedResource):
     """https://learn.microsoft.com/en-us/rest/api/azure/devops/build/definitions?view=azure-devops-rest-7.1"""
 
     build_definition_id: str = field(metadata={"is_id_field": True})
     name: str = field(metadata={"editable": True})
-    description: str = field(metadata={"editable": True})
-    path: str
-    created_by: Member | None
-    created_date: datetime | None
+    description: str = field(metadata={"editable": True}, repr=False)
+    path: str = field(repr=False)
+    created_by: Member | None = field(repr=False)
+    created_date: datetime | None  = field(repr=False)
     build_repo: BuildRepository | None = field(repr=False)
-    revision: str = "1"
+    revision: str = field(default="1", repr=False)
     process: dict[str, str | int] | None = field(repr=False, default=None)  # Used internally, mostly ignore
     variables: dict[str, str] = field(default_factory=dict, repr=False)
-    variable_groups: list[int] = field(default_factory=list, repr=False)
+    # variable_groups: list[int] = field(default_factory=list, repr=False)
 
     def __str__(self) -> str:
         return f"{self.name}, {self.build_definition_id}, created by {self.created_by}, created on {self.created_date!s}"
 
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> "BuildDefinition":
         """Repo is not always present, Member is sometimes present, sometimes None"""
         created_by = Member.from_request_payload(data["authoredBy"]) if "authoredBy" in data else None  # fmt: skip
         build_repository = BuildRepository.from_request_payload(data["repository"]) if "repository" in data else None
-        return cls(str(data["id"]), data["name"], data.get("description", ""), data.get("process", {"yamlFilename": "UNKNOWN"})["yamlFilename"], created_by,
-                from_ado_date_string(data.get("createdDate")), build_repository, str(data["revision"]), data.get("process"), data.get("variables", {}), data.get("variableGroups", []))  # fmt: skip
+        return cls(
+            str(data["id"]), data["name"], data.get("description", ""), data.get("process", {"yamlFilename": "UNKNOWN"})["yamlFilename"],
+            created_by, from_ado_date_string(data.get("createdDate")), build_repository, str(data["revision"]), data.get("process"),
+            data.get("variables", {})  # fmt: skip
+        )
 
     @classmethod
     def get_by_id(cls, ado_client: "AdoClient", build_definition_id: str) -> "BuildDefinition":
         return super().get_by_url(
             ado_client,
             f"/{ado_client.ado_project}/_apis/build/definitions/{build_definition_id}?api-version=7.1",
         )  # type: ignore[return-value]
 
     @classmethod
     def create(  # type: ignore[override]
         cls, ado_client: "AdoClient", name: str, repo_id: str, repo_name: str, path_to_pipeline: str,
-        description: str, agent_pool_id: str, variable_groups: list[str], branch_name: str = "main",  # fmt: skip
+        description: str, agent_pool_id: str, branch_name: str = "main",  # fmt: skip
     ) -> "BuildDefinition":
         payload = get_build_definition(name, repo_id, repo_name, path_to_pipeline, description,
                                        ado_client.ado_project, agent_pool_id, branch_name)  # fmt: skip
         return super().create(
             ado_client,
             f"/{ado_client.ado_project}/_apis/build/definitions?api-version=7.0",
             payload=payload,
         )  # type: ignore[return-value]
-        #  | {"variableGroups": [{"id": x for x in variable_groups}]},
+
 
     def update(self, ado_client: "AdoClient", attribute_name: BuildDefinitionEditableAttribute, attribute_value: Any) -> None:  # type: ignore[override]
         if self.build_repo is None or self.process is None:
             raise ValueError("This build definition does not have a (repository or process) in its data, it cannot be updated")
         payload = (
             {"name": self.name, "id": self.build_definition_id, "revision": int(self.revision),
              "repository": {"id": self.build_repo.build_repository_id, "type": self.build_repo.type},
@@ -247,14 +250,15 @@
             ado_client,
             f"/{ado_client.ado_project}/_apis/build/definitions/{resource_id}?forceDelete=true&api-version=7.1",
             resource_id,
         )
 
     @classmethod
     def get_all(cls, ado_client: "AdoClient") -> "list[BuildDefinition]":  # type: ignore[override]
+        """WARNING: This returns a list of references, which don't have variable groups and more data included."""
         return super().get_all(
             ado_client,
             f"/{ado_client.ado_project}/_apis/build/definitions?api-version=7.1",
         )  # type: ignore[return-value]
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
@@ -263,14 +267,18 @@
     @classmethod
     def get_all_by_name(cls, ado_client: "AdoClient", name: str) -> "list[BuildDefinition]":
         return cls.get_by_abstract_filter(ado_client, lambda x: x.name == name)  # type: ignore[return-value, attr-defined]
 
     def get_all_builds_by_definition(self, ado_client: "AdoClient") -> "list[Build]":
         return Build.get_all_by_definition(ado_client, self.build_definition_id)
 
+    def get_latest_build_by_definition(self, ado_client: "AdoClient") -> "Build | None":
+        builds = self.get_all_builds_by_definition(ado_client)
+        return max(builds, key=lambda build: build.start_time if build.start_time else datetime(2000, 0, 0)) if builds else None
+
     @classmethod
     def get_all_by_repo_id(cls, ado_client: "AdoClient", repo_id: str) -> "list[BuildDefinition]":
         return super().get_all(
             ado_client,
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/build/definitions?repositoryId={repo_id}&repositoryType={'TfsGit'}&api-version=7.1",
         )  # type: ignore[return-value]
```

### Comparing `ado_wrapper-1.7.0/ado_wrapper/resources/commits.py` & `ado_wrapper-1.7.1/ado_wrapper/resources/commits.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.0/ado_wrapper/resources/environment.py` & `ado_wrapper-1.7.1/ado_wrapper/resources/environment.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.0/ado_wrapper/resources/groups.py` & `ado_wrapper-1.7.1/ado_wrapper/resources/groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 @dataclass
 class Group(StateManagedResource):
     """https://learn.microsoft.com/en-us/rest/api/azure/devops/graph/groups?view=azure-devops-rest-7.1"""
 
     group_descriptor: str = field(metadata={"is_id_field": True})  # None are editable
     name: str = field(metadata={"internal_name": "displayName"})  # Not editable
     description: str
-    group_id: str  # Not editable, don't use
-    origin_id: str = field(metadata={"internal_name": "originId"})  # Not editable, don't use
+    domain: str
+    origin_id: str = field(metadata={"internal_name": "originId"})  # Not editable
     # group_members: list[GroupMember] = field(default_factory=list)
 
     @classmethod
     def from_request_payload(cls, data: dict[str, str]) -> Group:
         return cls(data["url"].split("/_apis/Graph/Groups/", maxsplit=1)[1], data["displayName"], data.get("description", ""),
                    data["domain"].removeprefix("vstfs:///Classification/TeamProject/"), data["originId"])  # fmt: skip
```

### Comparing `ado_wrapper-1.7.0/ado_wrapper/resources/merge_policies.py` & `ado_wrapper-1.7.1/ado_wrapper/resources/merge_policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,17 @@
     )
     # rint([(x["displayName"], x["id"]) for x in request.json()["value"]])
     return [x for x in request.json()["value"] if x["displayName"] == action_type][0]["id"]  # type: ignore[no-any-return]
 
 
 @dataclass
 class MergePolicyDefaultReviewer(StateManagedResource):
+    """Represents 1 required reviewer and if they're required."""
     policy_id: str = field(metadata={"is_id_field": True})
-    required_reviewer_id: list[str]
+    required_reviewer_id: str
     is_required: bool
 
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> StateManagedResource:
         return cls(data["id"], data["settings"]["requiredReviewerIds"][0], data["isBlocking"])
 
     @staticmethod
@@ -58,28 +59,30 @@
         ).json()
         if request is None:
             return []
         if "ms.vss-code-web.branch-policies-data-provider" not in request["dataProviders"]:
             if not ado_client.suppress_warnings:
                 print(f"No default reviewers found for repo {repo_id}! Most likely it's disabled.")
             return []
-        # ===
-        all_reviewers = [Reviewer(x["displayName"], x["uniqueName"], x["id"], 0, False) for x in request["dataProviders"]["ms.vss-code-web.branch-policies-data-provider"]["identities"]]  # fmt: skip
+        identities = request["dataProviders"]["ms.vss-code-web.branch-policies-data-provider"]["identities"]
+        # === # Maybe switch ["id"] to ["descriptor"]?
+        all_reviewers = [Reviewer(x["displayName"], x["uniqueName"], x["id"]) for x in identities]  # fmt: skip
         for policy_group in request["dataProviders"]["ms.vss-code-web.branch-policies-data-provider"]["policyGroups"].values():
             if policy_group["currentScopePolicies"] is None:
                 continue
             is_required = policy_group["currentScopePolicies"][0]["isBlocking"]
             if is_required and "requiredReviewerIds" in policy_group["currentScopePolicies"][0]["settings"]:
                 reviewers = policy_group["currentScopePolicies"][0]["settings"]["requiredReviewerIds"]
                 for reviewer_id in reviewers:
                     [x for x in all_reviewers if x.member_id == reviewer_id][0].is_required = True
         return all_reviewers
 
     @classmethod
     def add_default_reviewer(cls, ado_client: AdoClient, repo_id: str, reviewer_id: str, is_required: bool, branch_name: str = "main") -> None:  # fmt: skip
+        """If the reviewer is a group, use the Group.origin_id attribute, for users, use their regular user id"""
         if reviewer_id in [x.member_id for x in cls.get_default_reviewers(ado_client, repo_id, branch_name)]:
             raise ValueError("Reviewer already exists! To update, please remove the reviewer first.")
         payload = {
             "type": {"id": _get_type_id(ado_client, "Required reviewers")},
             "isBlocking": is_required,
             "isEnabled": True,
             "settings": {
@@ -234,14 +237,15 @@
             if policies is not None
             else None
         )
 
     # ================== Default Reviewers ================== #
     @staticmethod
     def add_default_reviewer(ado_client: AdoClient, repo_id: str, reviewer_id: str, is_required: bool, branch_name: str = "main") -> None:
+        """If the reviewer is a group, use the Group.origin_id attribute, for users, use their regular user id"""
         return MergePolicyDefaultReviewer.add_default_reviewer(ado_client, repo_id, reviewer_id, is_required, branch_name)
 
     @staticmethod
     def get_default_reviewers(ado_client: AdoClient, repo_id: str, branch_name: str = "main") -> list[Reviewer]:
         return MergePolicyDefaultReviewer.get_default_reviewers(ado_client, repo_id, branch_name)
 
     @staticmethod
```

### Comparing `ado_wrapper-1.7.0/ado_wrapper/resources/projects.py` & `ado_wrapper-1.7.1/ado_wrapper/resources/projects.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.0/ado_wrapper/resources/pull_requests.py` & `ado_wrapper-1.7.1/ado_wrapper/resources/pull_requests.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.0/ado_wrapper/resources/releases.py` & `ado_wrapper-1.7.1/ado_wrapper/resources/releases.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.0/ado_wrapper/resources/repo.py` & `ado_wrapper-1.7.1/ado_wrapper/resources/repo.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import zipfile
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Any, Literal
 
 import requests
 
 from ado_wrapper.resources.commits import Commit
-from ado_wrapper.resources.merge_policies import MergePolicies
+from ado_wrapper.resources.merge_policies import MergePolicies, MergePolicyDefaultReviewer
 from ado_wrapper.resources.pull_requests import PullRequest, PullRequestStatus
 from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.utils import ResourceNotFound, UnknownError
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
     from ado_wrapper.resources.merge_policies import (
@@ -86,18 +86,15 @@
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
     def get_by_name(cls, ado_client: AdoClient, repo_name: str) -> Repo | None:  # type: ignore[return]
-        """Warning, this function must fetch `all` repos to work, be cautious when calling it in a loop."""
-        for repo in cls.get_all(ado_client):
-            if repo.name == repo_name:
-                return repo
+        return cls.get_by_abstract_filter(ado_client, lambda repo: repo.name == repo_name)  # type: ignore[return-type]
 
     def get_file(self, ado_client: AdoClient, file_path: str, branch_name: str = "main") -> str:
         request = ado_client.session.get(
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{self.repo_id}/items?path={file_path}&versionType={'Branch'}&version={branch_name}&api-version=7.1",
         )
         if request.status_code == 404:
             raise ResourceNotFound(f"File {file_path} not found in repo {self.repo_id}")
@@ -159,14 +156,15 @@
             self.update(ado_client, "is_disabled", False)
         self.delete_by_id(ado_client, self.repo_id)
 
     @staticmethod
     def get_content_static(
         ado_client: AdoClient, repo_id: str, file_types: list[str] | None = None, branch_name: str = "main"
     ) -> dict[str, str]:
+        """Fetches the repo for you."""
         repo = Repo.get_by_id(ado_client, repo_id)
         return repo.get_contents(ado_client, file_types, branch_name)
 
     @staticmethod
     def get_branch_merge_policy(ado_client: AdoClient, repo_id: str, branch_name: str = "main") -> MergeBranchPolicy | None:
         return MergePolicies.get_branch_policy(ado_client, repo_id, branch_name)
 
@@ -174,29 +172,36 @@
     def set_branch_merge_policy(ado_client: AdoClient, repo_id: str, minimum_approver_count: int,
                           creator_vote_counts: bool, prohibit_last_pushers_vote: bool, allow_completion_with_rejects: bool,
                           when_new_changes_are_pushed: WhenChangesArePushed, branch_name: str = "main") -> MergePolicies | None:  # fmt: skip
         return MergePolicies.set_branch_policy(ado_client, repo_id, minimum_approver_count, creator_vote_counts,
                                                prohibit_last_pushers_vote, allow_completion_with_rejects, when_new_changes_are_pushed,
                                                branch_name)  # fmt: skip
 
+    @classmethod
+    def get_all_repos_with_required_reviewer(cls, ado_client: AdoClient, reviewer_email: str) -> list[Repo]:
+        return [
+            repo for repo in Repo.get_all(ado_client)
+            if any(x.email.lower()==reviewer_email.lower() for x in MergePolicyDefaultReviewer.get_default_reviewers(ado_client, repo.repo_id))
+        ]
 
 # ====================================================================
 
 
 @dataclass
 class BuildRepository:
     build_repository_id: str = field(metadata={"is_id_field": True})
     name: str | None = None
     type: str = "TfsGit"
     clean: bool | None = None
     checkout_submodules: bool = field(default=False, metadata={"internal_name": "checkoutSubmodules"})
 
     @classmethod
-    def from_request_payload(cls, data: dict[str, str | bool]) -> BuildRepository:
-        return cls(data["id"], data.get("name"), data.get("type", "TfsGit"), data.get("clean"), data.get("checkoutSubmodules", False))  # type: ignore[arg-type]
+    def from_request_payload(cls, data: dict[str, Any]) -> BuildRepository:
+        return cls(data["id"], data.get("name"), data.get("type", "TfsGit"),
+                   data.get("clean"), data.get("checkoutSubmodules", False))  # fmt: skip
 
     @classmethod
     def from_json(cls, data: dict[str, str | bool]) -> BuildRepository:
         return cls(data["id"], data.get("name"), data.get("type", "TfsGit"), data.get("clean"), data.get("checkoutSubmodules", False))  # type: ignore[arg-type]
 
     def to_json(self) -> dict[str, str | bool | None]:
         return {
```

### Comparing `ado_wrapper-1.7.0/ado_wrapper/resources/repo_user_permission.py` & `ado_wrapper-1.7.1/ado_wrapper/resources/repo_user_permission.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 PERMISSION_SET_ID = "2e9eb7ed-3c0a-47d4-87c1-0ffdd275fd87"  # This is global and hardcoded
 ActionType = Literal["Allow", "Deny", "Not set"]
 PermissionType = Literal[
     "bypass_policies_when_completing_pull_requests", "bypass_policies_when_pushing", "contribute",
     "contribute_to_pull_requests", "create_branch", "create_tag", "delete_or_disable_repository",
     "edit_policies", "force_push", "manage_notes", "manage_permissions", "read", "remove_others_locks",
-    "rename_repository",
+    "rename_repository",  # fmt: skip
 ]
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 external_to_internal_mapping = {
     "Bypass policies when completing pull requests": "bypass_policies_when_completing_pull_requests",
@@ -28,16 +28,16 @@
     "Create tag": "create_tag",
     "Delete or disable repository": "delete_or_disable_repository",
     "Edit policies": "edit_policies",
     "Force push (rewrite history, delete branches and tags)": "force_push",
     "Manage notes": "manage_notes",
     "Manage permissions": "manage_permissions",
     "Read": "read",
-    "Remove others\' locks": "remove_others_locks",
-    "Rename repository": "rename_repository"
+    "Remove others' locks": "remove_others_locks",
+    "Rename repository": "rename_repository",
 }
 
 flag_mapping = {  # Where is 1 & 256?
     "bypass_policies_when_completing_pull_requests": 32768,
     "bypass_policies_when_pushing": 128,
     "contribute": 4,
     "contribute_to_pull_requests": 16384,
@@ -49,14 +49,15 @@
     "manage_notes": 64,
     "manage_permissions": 8192,
     "read": 2,
     "remove_others_locks": 4096,
     "rename_repository": 1024,
 }
 
+
 @dataclass
 class UserPermission:
     namespace_id: str = field(repr=False)
     display_name: str
     programmatic_name: str
     token: str = field(repr=False)
     bit: int = field(repr=False)
@@ -69,37 +70,39 @@
             data["namespaceId"], data["displayName"], external_to_internal_mapping.get(data["displayName"], data["displayName"]),
             data["token"], data["bit"], data.get("canEdit", False), data["permissionDisplayString"]  # fmt: skip
         )
 
     @classmethod
     def get_by_subject_descriptor(cls, ado_client: AdoClient, subject_descriptor: str, repo_id: str) -> list[UserPermission]:
         requires_initialisation(ado_client)
-        PAYLOAD = {"contributionIds": ["ms.vss-admin-web.security-view-permissions-data-provider"], "dataProviderContext": {"properties": {
-            "subjectDescriptor": subject_descriptor,
-            "permissionSetId": PERMISSION_SET_ID,
-            "permissionSetToken": f"repoV2/{ado_client.ado_project_id}/{repo_id}",
-        }}}
+        PAYLOAD = {
+            "contributionIds": ["ms.vss-admin-web.security-view-permissions-data-provider"], "dataProviderContext": { "properties": {
+                "subjectDescriptor": subject_descriptor,
+                "permissionSetId": PERMISSION_SET_ID,
+                "permissionSetToken": f"repoV2/{ado_client.ado_project_id}/{repo_id}",
+            }},
+        }  # fmt: skip
         request = ado_client.session.post(
             f"https://dev.azure.com/{ado_client.ado_org}/_apis/Contribution/HierarchyQuery?api-version=5.0-preview.1",
             json=PAYLOAD,
         ).json()["dataProviders"]["ms.vss-admin-web.security-view-permissions-data-provider"]
         if request is None:
             raise ResourceNotFound("Couldn't find perms for that repo, descriptor combo.")
         return [UserPermission.from_request_payload(x) for x in request["subjectPermissions"]]
 
     @classmethod
     def set_by_subject_email(cls, ado_client: AdoClient, repo_id: str, subject_email: str, action: ActionType,
-                             permission: PermissionType, domain_container_id: str = "") -> None:
+                             permission: PermissionType, domain_container_id: str = "") -> None:  # fmt: skip
         requires_initialisation(ado_client)
         if not domain_container_id:
             domain_container_id = AdoUser.get_by_email(ado_client, subject_email).domain_container_id
         PAYLOAD = {"token": f"repoV2/{ado_client.ado_project_id}/{repo_id}", "merge": True, "accessControlEntries":[
             {"descriptor": f"Microsoft.IdentityModel.Claims.ClaimsIdentity;{domain_container_id}\\{subject_email}",
              "allow": flag_mapping[permission] if action == "Allow" else 0, "deny": flag_mapping[permission] if action == "Deny" else 0,
-        }]}
+        }]}  # fmt: skip
         request = ado_client.session.post(
             f"https://dev.azure.com/{ado_client.ado_org}/_apis/AccessControlEntries/{PERMISSION_SET_ID}",
             json=PAYLOAD,
         )
         assert request.status_code == 200
 
     @classmethod
@@ -121,36 +124,36 @@
     def get_all_by_repo_id(cls, ado_client: AdoClient, repo_id: str, users_only: bool=True,
                            ignore_inherits: bool=True, remove_not_set: bool=False) -> dict[str, list[UserPermission]]:  # fmt: skip
         """Gets all user permissions for a repo, user_only removes groups"""
         requires_initialisation(ado_client)
         PAYLOAD =  {"contributionIds":["ms.vss-admin-web.security-view-members-data-provider"], "dataProviderContext": {"properties": {
             "permissionSetId": PERMISSION_SET_ID,
             "permissionSetToken":f"repoV2/{ado_client.ado_project_id}/{repo_id}"
-        }}}
+        }}}  # fmt: skip
         request = ado_client.session.post(
             f"https://dev.azure.com/{ado_client.ado_org}/_apis/Contribution/HierarchyQuery?api-version=7.0-preview.1",
             json=PAYLOAD,
         ).json()["dataProviders"]["ms.vss-admin-web.security-view-members-data-provider"]
         if request is None:
             raise ResourceNotFound("Could not find any permissions for this repo! Does it exist?")
         # We now make descriptor -> display_name mapping
         groups_and_users = {
             identity["descriptor"]: identity["principalName"] if identity["subjectKind"] == "group" else identity["displayName"]
             for identity in request["identities"]
             if not users_only or (identity["subjectKind"] != "group")  # If we're doing users only, don't include if it's a group
-        }
+        }  # fmt: skip
         # We then make user_name -> list[UserPermissions]
         perms_mapping = {
             name: UserPermission.get_by_subject_descriptor(ado_client, descriptor, repo_id)
             for descriptor, name in groups_and_users.items()  # fmt: skip
         }
         # Then, if they want to remove inherited perms, we do that.
         filtered_perms = {
             user: perms for user, perms in perms_mapping.items() if not ignore_inherits or
-            any(x.permission_display_string in ["Allow", "Deny"] for x in perms)
+            any(x.permission_display_string in ["Allow", "Deny"] for x in perms)  # fmt: skip
         }
         # Finally, if they want to remove perms which are left as "Not set", we do that now
         return {  # Filters Not set
             user: [x for x in perms if not remove_not_set or x.permission_display_string != ("Not set")]
             for user, perms in filtered_perms.items()
         }
 
@@ -161,37 +164,37 @@
     @classmethod
     def get_by_subject_email(cls, ado_client: AdoClient, repo_id: str, subject_email: str) -> list[UserPermission]:
         descriptor = AdoUser.get_by_email(ado_client, subject_email).descriptor_id
         return cls.get_by_subject_descriptor(ado_client, repo_id, descriptor)
 
     @staticmethod
     def set_by_subject_email(ado_client: AdoClient, repo_id: str, subject_email: str, action: ActionType,
-                             permission: PermissionType, domain_container_id: str = "") -> None:
+                             permission: PermissionType, domain_container_id: str = "") -> None:  # fmt: skip
         return UserPermission.set_by_subject_email(ado_client, repo_id, subject_email, action, permission, domain_container_id)
 
     @classmethod
     def set_by_subject_email_batch(cls, ado_client: AdoClient, repo_id: str, subject_email: str,
-                                   mapping: dict[PermissionType, ActionType], domain_container_id: str = "") -> None:
+                                   mapping: dict[PermissionType, ActionType], domain_container_id: str = "") -> None:  # fmt: skip
         """Does a batch job of updating permissions, updating all permissions for one subject (user or group)"""
         if not domain_container_id:
             domain_container_id = AdoUser.get_by_email(ado_client, subject_email).domain_container_id
         for permission, action in mapping.items():
             cls.set_by_subject_email(ado_client, repo_id, subject_email, action, permission, domain_container_id)
 
     @classmethod
-    def set_all_permissions_for_repo(cls, ado_client: AdoClient, repo_id: str, mapping: dict[str, dict[PermissionType, ActionType]]) -> None:
+    def set_all_permissions_for_repo(cls, ado_client: AdoClient, repo_id: str, mapping: dict[str, dict[PermissionType, ActionType]]) -> None:  # fmt: skip
         """Takes a mapping of <user_email>: {permission_name: Allow | Deny | Not set}}"""
         domain_container_id = AdoUser.get_by_email(ado_client, list(mapping.keys())[0]).domain_container_id
         for email, permission_pairs in mapping.items():
             cls.set_by_subject_email_batch(ado_client, repo_id, email, permission_pairs, domain_container_id)
 
     @classmethod
     def remove_perm(cls, ado_client: AdoClient, repo_id: str, subject_email: str, domain_container_id: str = "") -> None:
         return UserPermission.remove_perm(ado_client, repo_id, subject_email, domain_container_id)
 
     @staticmethod
     def display_output(permissions: list[UserPermission]) -> str:
-        return "    "+"\n    ".join([str(x) for x in permissions])
+        return "    " + "\n    ".join([str(x) for x in permissions])
 
     @staticmethod
     def display_output_for_repo(mapping: dict[str, list[UserPermission]]) -> str:
-        return "\n".join([user_name+"\n"+RepoUserPermissions.display_output(values) for user_name, values in mapping.items()])
+        return "\n".join([user_name + "\n" + RepoUserPermissions.display_output(values) for user_name, values in mapping.items()])
```

### Comparing `ado_wrapper-1.7.0/ado_wrapper/resources/searches.py` & `ado_wrapper-1.7.1/ado_wrapper/resources/searches.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.0/ado_wrapper/resources/service_endpoint.py` & `ado_wrapper-1.7.1/ado_wrapper/resources/service_endpoint.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.0/ado_wrapper/resources/teams.py` & `ado_wrapper-1.7.1/ado_wrapper/resources/teams.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.0/ado_wrapper/resources/users.py` & `ado_wrapper-1.7.1/ado_wrapper/resources/users.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 # ------------------------------------------------------------------------------------------------------- #
 # ======================================================================================================= #
 
 
 class Reviewer(Member):
     """Identical to Member, but with additional attributes `vote` and `is_required` for PR reviews."""
 
-    def __init__(self, name: str, email: str, reviewer_id: str, vote: VoteOptions, is_required: bool) -> None:
+    def __init__(self, name: str, email: str, reviewer_id: str, vote: VoteOptions = 0, is_required: bool = False) -> None:
         super().__init__(name, email, reviewer_id)
         self.vote = vote
         self.is_required = is_required
 
     def __str__(self) -> str:
         return f'{self.name} ({self.email}) voted {VOTE_ID_TO_TYPE[self.vote]}, and was {"required" if self.is_required else "optional"}'
```

### Comparing `ado_wrapper-1.7.0/ado_wrapper/resources/variable_groups.py` & `ado_wrapper-1.7.1/ado_wrapper/resources/variable_groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.0/ado_wrapper/state_managed_abc.py` & `ado_wrapper-1.7.1/ado_wrapper/state_managed_abc.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.0/ado_wrapper/state_manager.py` & `ado_wrapper-1.7.1/ado_wrapper/state_manager.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.0/ado_wrapper/utils.py` & `ado_wrapper-1.7.1/ado_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.0/pyproject.toml` & `ado_wrapper-1.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "ado_wrapper"
 description = "A high level wrapper around the AzureDevops API including OOP principals and state management"
 authors = ["Ben Skerritt"]
-version = "1.7.0"
+version = "1.7.1"
 license = "Proprietary"
 readme = "README.md"
 packages = [{include = "ado_wrapper"}]
 
 [tool.poetry.scripts]
 ado_wrapper = "ado_wrapper.__main__:main"
```

### Comparing `ado_wrapper-1.7.0/PKG-INFO` & `ado_wrapper-1.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ado_wrapper
-Version: 1.7.0
+Version: 1.7.1
 Summary: A high level wrapper around the AzureDevops API including OOP principals and state management
 License: Proprietary
 Author: Ben Skerritt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

