# Comparing `tmp/keystone_api-0.3.7.tar.gz` & `tmp/keystone_api-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keystone_api-0.3.7.tar", max compression
+gzip compressed data, was "keystone_api-0.3.8.tar", max compression
```

## Comparing `keystone_api-0.3.7.tar` & `keystone_api-0.3.8.tar`

### file list

```diff
@@ -1,134 +1,140 @@
--rw-r--r--   0        0        0    13578 2024-04-30 20:23:18.059406 keystone_api-0.3.7/README.md
--rw-r--r--   0        0        0      428 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/admin_utils/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/admin_utils/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/admin_utils/management/commands/__init__.py
--rw-r--r--   0        0        0     2619 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/admin_utils/management/commands/clean.py
--rw-r--r--   0        0        0     2820 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/admin_utils/management/commands/enable_autocomplete.py
--rw-r--r--   0        0        0      471 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/admin_utils/management/commands/keystone_autocomplete
--rw-r--r--   0        0        0     3618 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/admin_utils/management/commands/quickstart.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/allocations/__init__.py
--rw-r--r--   0        0        0     4543 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/allocations/admin.py
--rw-r--r--   0        0        0     2173 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/allocations/managers.py
--rw-r--r--   0        0        0     3420 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/allocations/migrations/0001_initial.py
--rw-r--r--   0        0        0     1298 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/allocations/migrations/0002_initial.py
--rw-r--r--   0        0        0     1063 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/allocations/migrations/__init__.py
--rw-r--r--   0        0        0     5191 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/allocations/models.py
--rw-r--r--   0        0        0     3347 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/allocations/permissions.py
--rw-r--r--   0        0        0     1917 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/allocations/serializers.py
--rw-r--r--   0        0        0     4324 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/allocations/tasks.py
--rw-r--r--   0        0        0      516 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/allocations/urls.py
--rw-r--r--   0        0        0     3246 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/allocations/views.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/authentication/__init__.py
--rw-r--r--   0        0        0      572 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/authentication/tasks.py
--rw-r--r--   0        0        0      444 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/authentication/urls.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/health/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/health/tests/__init__.py
--rw-r--r--   0        0        0     3199 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/health/tests/test_views.py
--rw-r--r--   0        0        0      244 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/health/urls.py
--rw-r--r--   0        0        0     2066 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/health/views.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/__init__.py
--rw-r--r--   0        0        0     2496 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/admin.py
--rw-r--r--   0        0        0     1101 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/handlers.py
--rw-r--r--   0        0        0     1828 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/middleware.py
--rw-r--r--   0        0        0     1959 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/migrations/0001_initial.py
--rw-r--r--   0        0        0      644 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/migrations/0002_remove_requestlog_date_alter_requestlog_endpoint_and_more.py
--rw-r--r--   0        0        0      638 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/migrations/0003_taskresult.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/migrations/__init__.py
--rw-r--r--   0        0        0     1645 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/models.py
--rw-r--r--   0        0        0     1112 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/serializers.py
--rw-r--r--   0        0        0      709 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/tasks.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/tests/handlers/__init__.py
--rw-r--r--   0        0        0     2560 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/tests/handlers/test_DBHandler.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/tests/middleware/__init__.py
--rw-r--r--   0        0        0     2390 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/tests/middleware/test_LogRequestMiddleware.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/tests/tasks/__init__.py
--rw-r--r--   0        0        0     1791 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/tests/tasks/test_rotate_log_files.py
--rw-r--r--   0        0        0      322 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/urls.py
--rw-r--r--   0        0        0     1284 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/views.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/openapi/__init__.py
--rw-r--r--   0        0        0      326 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/openapi/urls.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/research_products/__init__.py
--rw-r--r--   0        0        0     1705 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/research_products/admin.py
--rw-r--r--   0        0        0     1261 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/research_products/managers.py
--rw-r--r--   0        0        0     1677 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/research_products/migrations/0001_initial.py
--rw-r--r--   0        0        0      437 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/research_products/migrations/0002_grant_grant_number.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/research_products/migrations/__init__.py
--rw-r--r--   0        0        0     1776 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/research_products/models.py
--rw-r--r--   0        0        0     2862 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/research_products/permissions.py
--rw-r--r--   0        0        0      928 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/research_products/serializers.py
--rw-r--r--   0        0        0      338 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/research_products/urls.py
--rw-r--r--   0        0        0     1554 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/research_products/views.py
--rw-r--r--   0        0        0      141 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/scheduler/__init__.py
--rw-r--r--   0        0        0      834 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/scheduler/admin.py
--rw-r--r--   0        0        0      654 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/scheduler/apps.py
--rw-r--r--   0        0        0     1344 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/scheduler/celery.py
--rw-r--r--   0        0        0      875 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/scheduler/checks.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/__init__.py
--rw-r--r--   0        0        0     1307 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/admin.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/management/commands/__init__.py
--rw-r--r--   0        0        0     1056 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/management/commands/ldap_update.py
--rw-r--r--   0        0        0     3134 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/managers.py
--rw-r--r--   0        0        0     3018 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/migrations/0001_initial.py
--rw-r--r--   0        0        0      405 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/migrations/0002_user_is_ldap_user.py
--rw-r--r--   0        0        0      402 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/migrations/0003_alter_researchgroup_name.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/migrations/__init__.py
--rw-r--r--   0        0        0     2383 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/models.py
--rw-r--r--   0        0        0      913 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/permissions.py
--rw-r--r--   0        0        0      887 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/serializers.py
--rw-r--r--   0        0        0     2095 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/tasks.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/apps/users/tests/test_managers/__init__.py
--rw-r--r--   0        0        0     1374 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py
--rw-r--r--   0        0        0     2399 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/apps/users/tests/test_managers/test_UserManager.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/apps/users/tests/test_models/__init__.py
--rw-r--r--   0        0        0     3210 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py
--rw-r--r--   0        0        0      471 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/apps/users/tests/test_models/test_User.py
--rw-r--r--   0        0        0      748 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/apps/users/tests/utils.py
--rw-r--r--   0        0        0      329 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/apps/users/urls.py
--rw-r--r--   0        0        0     1329 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/apps/users/views.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/main/__init__.py
--rw-r--r--   0        0        0      169 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/main/asgi.py
--rw-r--r--   0        0        0     8125 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/main/settings.py
--rw-r--r--   0        0        0     1058 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/main/urls.py
--rw-r--r--   0        0        0      168 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/main/wsgi.py
--rwxr-xr-x   0        0        0      556 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/manage.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/plugins/__init__.py
--rw-r--r--   0        0        0     4728 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/plugins/slurm.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/allocations/__init__.py
--rw-r--r--   0        0        0     2923 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/allocations/test_allocations.py
--rw-r--r--   0        0        0     4229 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/allocations/test_allocations_pk.py
--rw-r--r--   0        0        0     2929 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/allocations/test_clusters.py
--rw-r--r--   0        0        0     3104 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/allocations/test_clusters_pk.py
--rw-r--r--   0        0        0     5631 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/allocations/test_requests.py
--rw-r--r--   0        0        0     5351 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/allocations/test_requests_pk.py
--rw-r--r--   0        0        0     2898 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/allocations/test_reviews.py
--rw-r--r--   0        0        0     4202 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/allocations/test_reviews_pk.py
--rw-r--r--   0        0        0     3921 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/fixtures/multi_research_group.yaml
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/health/__init__.py
--rw-r--r--   0        0        0     3073 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/health/test.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/logging/__init__.py
--rw-r--r--   0        0        0     2871 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/logging/test_apps.py
--rw-r--r--   0        0        0     2879 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/logging/test_requests.py
--rw-r--r--   0        0        0     2873 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/logging/test_tasks.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/openapi/__init__.py
--rw-r--r--   0        0        0     2867 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/openapi/test_json.py
--rw-r--r--   0        0        0     2867 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/openapi/test_yaml.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/research/__init__.py
--rw-r--r--   0        0        0     5611 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/research/test_grants.py
--rw-r--r--   0        0        0     4524 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/research/test_grants_pk.py
--rw-r--r--   0        0        0     5782 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/research/test_publications.py
--rw-r--r--   0        0        0     4438 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/research/test_publications_pk.py
--rw-r--r--   0        0        0        0 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/users/__init__.py
--rw-r--r--   0        0        0     2981 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/users/test_researchgroups.py
--rw-r--r--   0        0        0     4244 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/users/test_researchgroups_pk.py
--rw-r--r--   0        0        0     2964 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/users/test_users.py
--rw-r--r--   0        0        0     4471 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/users/test_users_pk.py
--rw-r--r--   0        0        0     2022 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/utils.py
--rw-r--r--   0        0        0      957 2024-04-30 20:23:38.111181 keystone_api-0.3.7/pyproject.toml
--rw-r--r--   0        0        0    14773 1970-01-01 00:00:00.000000 keystone_api-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0    13578 2024-05-07 15:51:21.888062 keystone_api-0.3.8/README.md
+-rw-r--r--   0        0        0      428 2024-05-07 15:51:21.888062 keystone_api-0.3.8/keystone_api/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.888062 keystone_api-0.3.8/keystone_api/apps/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.888062 keystone_api-0.3.8/keystone_api/apps/admin_utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/admin_utils/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/admin_utils/management/commands/__init__.py
+-rw-r--r--   0        0        0     2619 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/admin_utils/management/commands/clean.py
+-rw-r--r--   0        0        0     2820 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/admin_utils/management/commands/enable_autocomplete.py
+-rw-r--r--   0        0        0      471 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/admin_utils/management/commands/keystone_autocomplete
+-rw-r--r--   0        0        0     3618 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/admin_utils/management/commands/quickstart.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/allocations/__init__.py
+-rw-r--r--   0        0        0     4543 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/allocations/admin.py
+-rw-r--r--   0        0        0     2173 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/allocations/managers.py
+-rw-r--r--   0        0        0     3420 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/allocations/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1298 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/allocations/migrations/0002_initial.py
+-rw-r--r--   0        0        0     1063 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/allocations/migrations/__init__.py
+-rw-r--r--   0        0        0     5191 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/allocations/models.py
+-rw-r--r--   0        0        0     3347 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/allocations/permissions.py
+-rw-r--r--   0        0        0     1917 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/allocations/serializers.py
+-rw-r--r--   0        0        0     5590 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/allocations/tasks.py
+-rw-r--r--   0        0        0      516 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/allocations/urls.py
+-rw-r--r--   0        0        0     3246 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/allocations/views.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/authentication/__init__.py
+-rw-r--r--   0        0        0      572 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/authentication/tasks.py
+-rw-r--r--   0        0        0      444 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/authentication/urls.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/health/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/health/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/health/tests/views/__init__.py
+-rw-r--r--   0        0        0     1213 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/health/tests/views/test_HealthCheckJsonView.py
+-rw-r--r--   0        0        0      978 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/health/tests/views/test_HealthCheckPrometheusView.py
+-rw-r--r--   0        0        0     1094 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/health/tests/views/test_HealthCheckView.py
+-rw-r--r--   0        0        0      667 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/health/tests/views/utils.py
+-rw-r--r--   0        0        0      345 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/health/urls.py
+-rw-r--r--   0        0        0     3569 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/health/views.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/__init__.py
+-rw-r--r--   0        0        0     2496 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/admin.py
+-rw-r--r--   0        0        0     1101 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/handlers.py
+-rw-r--r--   0        0        0     1828 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/middleware.py
+-rw-r--r--   0        0        0     1959 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/migrations/0001_initial.py
+-rw-r--r--   0        0        0      644 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/migrations/0002_remove_requestlog_date_alter_requestlog_endpoint_and_more.py
+-rw-r--r--   0        0        0      638 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/migrations/0003_taskresult.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/migrations/__init__.py
+-rw-r--r--   0        0        0     1645 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/models.py
+-rw-r--r--   0        0        0     1112 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/serializers.py
+-rw-r--r--   0        0        0      733 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/tasks.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/tests/handlers/__init__.py
+-rw-r--r--   0        0        0     2560 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/tests/handlers/test_DBHandler.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/tests/middleware/__init__.py
+-rw-r--r--   0        0        0     2390 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/tests/middleware/test_LogRequestMiddleware.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/tests/tasks/__init__.py
+-rw-r--r--   0        0        0     1791 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/tests/tasks/test_rotate_log_files.py
+-rw-r--r--   0        0        0      322 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/urls.py
+-rw-r--r--   0        0        0     1284 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/views.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/openapi/__init__.py
+-rw-r--r--   0        0        0      326 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/openapi/urls.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/research_products/__init__.py
+-rw-r--r--   0        0        0     1705 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/research_products/admin.py
+-rw-r--r--   0        0        0     1261 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/research_products/managers.py
+-rw-r--r--   0        0        0     1677 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/research_products/migrations/0001_initial.py
+-rw-r--r--   0        0        0      437 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/research_products/migrations/0002_grant_grant_number.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/research_products/migrations/__init__.py
+-rw-r--r--   0        0        0     1776 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/research_products/models.py
+-rw-r--r--   0        0        0     2862 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/research_products/permissions.py
+-rw-r--r--   0        0        0      928 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/research_products/serializers.py
+-rw-r--r--   0        0        0      338 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/research_products/urls.py
+-rw-r--r--   0        0        0     1554 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/research_products/views.py
+-rw-r--r--   0        0        0      141 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/scheduler/__init__.py
+-rw-r--r--   0        0        0      834 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/scheduler/admin.py
+-rw-r--r--   0        0        0      654 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/scheduler/apps.py
+-rw-r--r--   0        0        0     1649 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/scheduler/celery.py
+-rw-r--r--   0        0        0      875 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/scheduler/checks.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/__init__.py
+-rw-r--r--   0        0        0     1307 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/admin.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/management/commands/__init__.py
+-rw-r--r--   0        0        0     1056 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/management/commands/ldap_update.py
+-rw-r--r--   0        0        0     3134 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/managers.py
+-rw-r--r--   0        0        0     3018 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/migrations/0001_initial.py
+-rw-r--r--   0        0        0      405 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/migrations/0002_user_is_ldap_user.py
+-rw-r--r--   0        0        0      402 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/migrations/0003_alter_researchgroup_name.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/migrations/__init__.py
+-rw-r--r--   0        0        0     2383 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/models.py
+-rw-r--r--   0        0        0      913 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/permissions.py
+-rw-r--r--   0        0        0      887 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/serializers.py
+-rw-r--r--   0        0        0     2095 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/tasks.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/tests/test_managers/__init__.py
+-rw-r--r--   0        0        0     1374 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py
+-rw-r--r--   0        0        0     2399 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/tests/test_managers/test_UserManager.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/tests/test_models/__init__.py
+-rw-r--r--   0        0        0     3210 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py
+-rw-r--r--   0        0        0      471 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/tests/test_models/test_User.py
+-rw-r--r--   0        0        0      748 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/tests/utils.py
+-rw-r--r--   0        0        0      329 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/urls.py
+-rw-r--r--   0        0        0     1329 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/views.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/main/__init__.py
+-rw-r--r--   0        0        0      169 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/main/asgi.py
+-rw-r--r--   0        0        0     8125 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/main/settings.py
+-rw-r--r--   0        0        0     1058 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/main/urls.py
+-rw-r--r--   0        0        0      168 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/main/wsgi.py
+-rwxr-xr-x   0        0        0      556 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/manage.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/plugins/__init__.py
+-rw-r--r--   0        0        0     4728 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/plugins/slurm.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/allocations/__init__.py
+-rw-r--r--   0        0        0     2923 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/allocations/test_allocations.py
+-rw-r--r--   0        0        0     4229 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/allocations/test_allocations_pk.py
+-rw-r--r--   0        0        0     2929 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/allocations/test_clusters.py
+-rw-r--r--   0        0        0     3104 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/allocations/test_clusters_pk.py
+-rw-r--r--   0        0        0     5631 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/allocations/test_requests.py
+-rw-r--r--   0        0        0     5351 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/allocations/test_requests_pk.py
+-rw-r--r--   0        0        0     2898 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/allocations/test_reviews.py
+-rw-r--r--   0        0        0     4202 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/allocations/test_reviews_pk.py
+-rw-r--r--   0        0        0     3921 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/fixtures/multi_research_group.yaml
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/health/__init__.py
+-rw-r--r--   0        0        0     2626 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/health/test.py
+-rw-r--r--   0        0        0     2908 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/health/test_json.py
+-rw-r--r--   0        0        0     2908 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/health/test_prom.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/logging/__init__.py
+-rw-r--r--   0        0        0     2871 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/logging/test_apps.py
+-rw-r--r--   0        0        0     2879 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/logging/test_requests.py
+-rw-r--r--   0        0        0     2873 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/logging/test_tasks.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/openapi/__init__.py
+-rw-r--r--   0        0        0     2867 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/openapi/test_json.py
+-rw-r--r--   0        0        0     2867 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/openapi/test_yaml.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/research/__init__.py
+-rw-r--r--   0        0        0     5611 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/research/test_grants.py
+-rw-r--r--   0        0        0     4524 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/research/test_grants_pk.py
+-rw-r--r--   0        0        0     5782 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/research/test_publications.py
+-rw-r--r--   0        0        0     4438 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/research/test_publications_pk.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/users/__init__.py
+-rw-r--r--   0        0        0     2981 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/users/test_researchgroups.py
+-rw-r--r--   0        0        0     4244 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/users/test_researchgroups_pk.py
+-rw-r--r--   0        0        0     2964 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/users/test_users.py
+-rw-r--r--   0        0        0     4471 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/users/test_users_pk.py
+-rw-r--r--   0        0        0     2022 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/utils.py
+-rw-r--r--   0        0        0      957 2024-05-07 15:51:34.851966 keystone_api-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0    14773 1970-01-01 00:00:00.000000 keystone_api-0.3.8/PKG-INFO
```

### Comparing `keystone_api-0.3.7/README.md` & `keystone_api-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/admin_utils/management/commands/clean.py` & `keystone_api-0.3.8/keystone_api/apps/admin_utils/management/commands/clean.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/admin_utils/management/commands/enable_autocomplete.py` & `keystone_api-0.3.8/keystone_api/apps/admin_utils/management/commands/enable_autocomplete.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/admin_utils/management/commands/quickstart.py` & `keystone_api-0.3.8/keystone_api/apps/admin_utils/management/commands/quickstart.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/allocations/admin.py` & `keystone_api-0.3.8/keystone_api/apps/allocations/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/allocations/managers.py` & `keystone_api-0.3.8/keystone_api/apps/allocations/managers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/allocations/migrations/0001_initial.py` & `keystone_api-0.3.8/keystone_api/apps/allocations/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/allocations/migrations/0002_initial.py` & `keystone_api-0.3.8/keystone_api/apps/allocations/migrations/0002_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py` & `keystone_api-0.3.8/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/allocations/models.py` & `keystone_api-0.3.8/keystone_api/apps/allocations/models.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/allocations/permissions.py` & `keystone_api-0.3.8/keystone_api/apps/allocations/permissions.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/allocations/serializers.py` & `keystone_api-0.3.8/keystone_api/apps/allocations/serializers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/allocations/urls.py` & `keystone_api-0.3.8/keystone_api/apps/allocations/urls.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/allocations/views.py` & `keystone_api-0.3.8/keystone_api/apps/allocations/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/authentication/tasks.py` & `keystone_api-0.3.8/keystone_api/apps/authentication/tasks.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/logging/admin.py` & `keystone_api-0.3.8/keystone_api/apps/logging/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/logging/handlers.py` & `keystone_api-0.3.8/keystone_api/apps/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/logging/middleware.py` & `keystone_api-0.3.8/keystone_api/apps/logging/middleware.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/logging/migrations/0001_initial.py` & `keystone_api-0.3.8/keystone_api/apps/logging/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/logging/migrations/0002_remove_requestlog_date_alter_requestlog_endpoint_and_more.py` & `keystone_api-0.3.8/keystone_api/apps/logging/migrations/0002_remove_requestlog_date_alter_requestlog_endpoint_and_more.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/logging/migrations/0003_taskresult.py` & `keystone_api-0.3.8/keystone_api/apps/logging/migrations/0003_taskresult.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/logging/models.py` & `keystone_api-0.3.8/keystone_api/apps/logging/models.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/logging/serializers.py` & `keystone_api-0.3.8/keystone_api/apps/logging/serializers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/logging/tasks.py` & `keystone_api-0.3.8/keystone_api/apps/logging/tasks.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """Scheduled tasks executed in parallel by Celery.
 
 Tasks are scheduled and executed in the background by Celery. They operate
 asynchronously from the rest of the application and log their results in the
 application database.
 """
 
-from datetime import datetime, timedelta
+from datetime import timedelta
 
 from celery import shared_task
 from django.conf import settings
+from django.utils import timezone
 
 from .models import *
 
 
 @shared_task()
 def rotate_log_files() -> None:
     """Delete old log files"""
 
     if settings.LOG_RECORD_ROTATION == 0:
         return
 
-    max_record_age = datetime.now() - timedelta(seconds=settings.LOG_RECORD_ROTATION)
+    max_record_age = timezone.now() - timedelta(seconds=settings.LOG_RECORD_ROTATION)
     AppLog.objects.filter(time__lt=max_record_age).delete()
     RequestLog.objects.filter(time__lt=max_record_age).delete()
```

### Comparing `keystone_api-0.3.7/keystone_api/apps/logging/tests/handlers/test_DBHandler.py` & `keystone_api-0.3.8/keystone_api/apps/logging/tests/handlers/test_DBHandler.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/logging/tests/middleware/test_LogRequestMiddleware.py` & `keystone_api-0.3.8/keystone_api/apps/logging/tests/middleware/test_LogRequestMiddleware.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/logging/tests/tasks/test_rotate_log_files.py` & `keystone_api-0.3.8/keystone_api/apps/logging/tests/tasks/test_rotate_log_files.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/logging/views.py` & `keystone_api-0.3.8/keystone_api/apps/logging/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/research_products/admin.py` & `keystone_api-0.3.8/keystone_api/apps/research_products/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/research_products/managers.py` & `keystone_api-0.3.8/keystone_api/apps/research_products/managers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/research_products/migrations/0001_initial.py` & `keystone_api-0.3.8/keystone_api/apps/research_products/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/research_products/models.py` & `keystone_api-0.3.8/keystone_api/apps/research_products/models.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/research_products/permissions.py` & `keystone_api-0.3.8/keystone_api/apps/research_products/permissions.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/research_products/serializers.py` & `keystone_api-0.3.8/keystone_api/apps/research_products/serializers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/research_products/views.py` & `keystone_api-0.3.8/keystone_api/apps/research_products/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/scheduler/admin.py` & `keystone_api-0.3.8/keystone_api/apps/scheduler/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/scheduler/apps.py` & `keystone_api-0.3.8/keystone_api/apps/scheduler/apps.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/scheduler/celery.py` & `keystone_api-0.3.8/keystone_api/apps/scheduler/celery.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,8 +25,13 @@
         'description': 'This task deletes old log entries according to application settings.'
     },
     'apps.authentication.tasks.flush_expired_tokens': {
         'task': 'apps.authentication.tasks.flush_expired_tokens',
         'schedule': crontab(hour='0', minute='0'),
         'description': 'This task clears the JWT token blacklist.'
     },
+    'apps.allocations.tasks.update_limits': {
+        'task': 'apps.allocations.tasks.update_limits',
+        'schedule': crontab(hour='0', minute='0'),
+        'description': 'This task updates the per cluser usage limits in Slurm for each Research Group based on the state of their allocations.'
+    },
 }
```

### Comparing `keystone_api-0.3.7/keystone_api/apps/scheduler/checks.py` & `keystone_api-0.3.8/keystone_api/apps/scheduler/checks.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/users/admin.py` & `keystone_api-0.3.8/keystone_api/apps/users/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/users/management/commands/ldap_update.py` & `keystone_api-0.3.8/keystone_api/apps/users/management/commands/ldap_update.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/users/managers.py` & `keystone_api-0.3.8/keystone_api/apps/users/managers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/users/migrations/0001_initial.py` & `keystone_api-0.3.8/keystone_api/apps/users/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/users/models.py` & `keystone_api-0.3.8/keystone_api/apps/users/models.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/users/permissions.py` & `keystone_api-0.3.8/keystone_api/apps/users/permissions.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/users/serializers.py` & `keystone_api-0.3.8/keystone_api/apps/users/serializers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/users/tasks.py` & `keystone_api-0.3.8/keystone_api/apps/users/tasks.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py` & `keystone_api-0.3.8/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/users/tests/test_managers/test_UserManager.py` & `keystone_api-0.3.8/keystone_api/apps/users/tests/test_managers/test_UserManager.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py` & `keystone_api-0.3.8/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/users/tests/utils.py` & `keystone_api-0.3.8/keystone_api/apps/users/tests/utils.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/apps/users/views.py` & `keystone_api-0.3.8/keystone_api/apps/users/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/main/settings.py` & `keystone_api-0.3.8/keystone_api/main/settings.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/main/urls.py` & `keystone_api-0.3.8/keystone_api/main/urls.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/manage.py` & `keystone_api-0.3.8/keystone_api/manage.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/plugins/slurm.py` & `keystone_api-0.3.8/keystone_api/plugins/slurm.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/tests/allocations/test_allocations.py` & `keystone_api-0.3.8/keystone_api/tests/allocations/test_allocations.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/tests/allocations/test_allocations_pk.py` & `keystone_api-0.3.8/keystone_api/tests/allocations/test_allocations_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/tests/allocations/test_clusters.py` & `keystone_api-0.3.8/keystone_api/tests/allocations/test_clusters.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/tests/allocations/test_clusters_pk.py` & `keystone_api-0.3.8/keystone_api/tests/allocations/test_clusters_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/tests/allocations/test_requests.py` & `keystone_api-0.3.8/keystone_api/tests/allocations/test_requests.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/tests/allocations/test_requests_pk.py` & `keystone_api-0.3.8/keystone_api/tests/allocations/test_requests_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/tests/allocations/test_reviews.py` & `keystone_api-0.3.8/keystone_api/tests/allocations/test_reviews.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/tests/allocations/test_reviews_pk.py` & `keystone_api-0.3.8/keystone_api/tests/allocations/test_reviews_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/tests/fixtures/multi_research_group.yaml` & `keystone_api-0.3.8/keystone_api/tests/fixtures/multi_research_group.yaml`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/tests/health/test.py` & `keystone_api-0.3.8/keystone_api/tests/health/test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Tests for the `/health/` endpoint"""
 
-import logging
-
-from django.test import TransactionTestCase
 from rest_framework import status
+from rest_framework.test import APITransactionTestCase
 
-from apps.users.tests.utils import create_test_user
+from apps.users.models import User
 
 
-class EndpointPermissions(TransactionTestCase):
+class EndpointPermissions(APITransactionTestCase):
     """Test endpoint user permissions
 
     Endpoint permissions are tested against the following matrix of HTTP responses.
 
     | Authentication      | GET     | HEAD     | OPTIONS | POST | PUT | PATCH | DELETE | TRACE |
     |---------------------|---------|----------|---------|------|-----|-------|--------|-------|
     | Anonymous User      | 200/500 | 200/500  | 200/500 | 405  | 405 | 405   | 405    | 405   |
@@ -23,44 +21,35 @@
     endpoint = '/health/'
     fixtures = ['multi_research_group.yaml']
     valid_responses = (status.HTTP_200_OK, status.HTTP_500_INTERNAL_SERVER_ERROR)
 
     def assert_read_only_responses(self) -> None:
         """Assert the currently authenticated user has read only permissions"""
 
-        # Temporarily disable health check logging
-        # Avoids spamming the console with health check messages
-        health_check_log = logging.getLogger('health-check')
-        log_level = health_check_log.level
-        health_check_log.setLevel(1000)
-
         self.assertIn(self.client.get(self.endpoint).status_code, self.valid_responses)
         self.assertIn(self.client.head(self.endpoint).status_code, self.valid_responses)
         self.assertIn(self.client.options(self.endpoint).status_code, self.valid_responses)
 
         self.assertEqual(self.client.post(self.endpoint).status_code, status.HTTP_405_METHOD_NOT_ALLOWED)
         self.assertEqual(self.client.put(self.endpoint).status_code, status.HTTP_405_METHOD_NOT_ALLOWED)
         self.assertEqual(self.client.patch(self.endpoint).status_code, status.HTTP_405_METHOD_NOT_ALLOWED)
         self.assertEqual(self.client.delete(self.endpoint).status_code, status.HTTP_405_METHOD_NOT_ALLOWED)
         self.assertEqual(self.client.trace(self.endpoint).status_code, status.HTTP_405_METHOD_NOT_ALLOWED)
 
-        # Restore the health chck logger
-        health_check_log.setLevel(log_level)
-
     def test_anonymous_user_permissions(self) -> None:
         """Test unauthenticated users have read-only permissions"""
 
         self.assert_read_only_responses()
 
     def test_authenticated_user_permissions(self) -> None:
         """Test authenticated users have read-only permissions"""
 
-        create_test_user(username='foo', password='foobar123!')
-        self.assertTrue(self.client.login(username='foo', password='foobar123!'))
+        user = User.objects.get(username='generic_user')
+        self.client.force_authenticate(user=user)
         self.assert_read_only_responses()
 
     def test_staff_user_permissions(self) -> None:
         """Test staff users have read-only permissions"""
 
-        create_test_user(username='foo', password='foobar123!')
-        self.assertTrue(self.client.login(username='foo', password='foobar123!'))
+        user = User.objects.get(username='staff_user')
+        self.client.force_authenticate(user=user)
         self.assert_read_only_responses()
```

### Comparing `keystone_api-0.3.7/keystone_api/tests/logging/test_apps.py` & `keystone_api-0.3.8/keystone_api/tests/logging/test_apps.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/tests/logging/test_requests.py` & `keystone_api-0.3.8/keystone_api/tests/logging/test_requests.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/tests/logging/test_tasks.py` & `keystone_api-0.3.8/keystone_api/tests/logging/test_tasks.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/tests/openapi/test_json.py` & `keystone_api-0.3.8/keystone_api/tests/openapi/test_json.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/tests/openapi/test_yaml.py` & `keystone_api-0.3.8/keystone_api/tests/openapi/test_yaml.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/tests/research/test_grants.py` & `keystone_api-0.3.8/keystone_api/tests/research/test_grants.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/tests/research/test_grants_pk.py` & `keystone_api-0.3.8/keystone_api/tests/research/test_grants_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/tests/research/test_publications.py` & `keystone_api-0.3.8/keystone_api/tests/research/test_publications.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/tests/research/test_publications_pk.py` & `keystone_api-0.3.8/keystone_api/tests/research/test_publications_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/tests/users/test_researchgroups.py` & `keystone_api-0.3.8/keystone_api/tests/users/test_researchgroups.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/tests/users/test_researchgroups_pk.py` & `keystone_api-0.3.8/keystone_api/tests/users/test_researchgroups_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/tests/users/test_users.py` & `keystone_api-0.3.8/keystone_api/tests/users/test_users.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/tests/users/test_users_pk.py` & `keystone_api-0.3.8/keystone_api/tests/users/test_users_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/keystone_api/tests/utils.py` & `keystone_api-0.3.8/keystone_api/tests/utils.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.7/pyproject.toml` & `keystone_api-0.3.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "keystone-api"
-version = "0.3.7"
+version = "0.3.8"
 readme = "README.md"
 description = "A REST API for managing user resource allocations on HPC systems."
 authors = ["Pitt Center for Research Computing"]
 keywords = ["Pitt", "CRC", "HPC", "django"]
 
 [tool.poetry.scripts]
 keystone-api = "keystone_api.manage:main"
@@ -26,11 +26,11 @@
 django-jazzmin = "3.0.0"
 djangorestframework = "3.15.1"
 djangorestframework-simplejwt = "5.3.1"
 drf_spectacular = { version = "0.27.2", extras = ["sidecar"] }
 gunicorn = "22.0.0"
 psycopg2-binary = "2.9.9"
 pyyaml = "6.0.1"
-redis = "5.0.3"
-tqdm = "4.66.2"
+redis = "5.0.4"
+tqdm = "4.66.3"
 uritemplate = "4.1.1"
 whitenoise = "6.6.0"
```

### Comparing `keystone_api-0.3.7/PKG-INFO` & `keystone_api-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keystone-api
-Version: 0.3.7
+Version: 0.3.8
 Summary: A REST API for managing user resource allocations on HPC systems.
 Keywords: Pitt,CRC,HPC,django
 Author: Pitt Center for Research Computing
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -19,16 +19,16 @@
 Requires-Dist: django-jazzmin (==3.0.0)
 Requires-Dist: djangorestframework (==3.15.1)
 Requires-Dist: djangorestframework-simplejwt (==5.3.1)
 Requires-Dist: drf_spectacular[sidecar] (==0.27.2)
 Requires-Dist: gunicorn (==22.0.0)
 Requires-Dist: psycopg2-binary (==2.9.9)
 Requires-Dist: pyyaml (==6.0.1)
-Requires-Dist: redis (==5.0.3)
-Requires-Dist: tqdm (==4.66.2)
+Requires-Dist: redis (==5.0.4)
+Requires-Dist: tqdm (==4.66.3)
 Requires-Dist: uritemplate (==4.1.1)
 Requires-Dist: whitenoise (==6.6.0)
 Description-Content-Type: text/markdown
 
 # Keystone API
 
 [![](https://app.codacy.com/project/badge/Grade/9ee06ecdddef4f75a8deeb42fa4a9651)](https://app.codacy.com?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
```

