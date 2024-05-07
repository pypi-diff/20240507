# Comparing `tmp/baseapp_comments-0.1.3.tar.gz` & `tmp/baseapp_comments-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseapp_comments-0.1.3.tar", last modified: Tue Apr 16 18:38:21 2024, max compression
+gzip compressed data, was "baseapp_comments-0.1.4.tar", last modified: Tue May  7 15:39:51 2024, max compression
```

## Comparing `baseapp_comments-0.1.3.tar` & `baseapp_comments-0.1.4.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:38:21.791751 baseapp_comments-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     7343 2024-04-16 18:38:21.791751 baseapp_comments-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:38:21.783751 baseapp_comments-0.1.3/baseapp_comments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:38:21.787751 baseapp_comments-0.1.3/baseapp_comments/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/graphql/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6952 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/graphql/mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/graphql/object_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/graphql/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/graphql/subscriptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:38:21.787751 baseapp_comments-0.1.3/baseapp_comments/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    17671 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/migrations/0002_alter_comment_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/migrations/0003_alter_comment_comments_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/migrations/0004_remove_comment_snapshot_insert_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:38:21.787751 baseapp_comments-0.1.3/baseapp_comments/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/tests/test_comments_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/tests/test_graphql_mutations_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/tests/test_graphql_mutations_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/tests/test_graphql_mutations_pin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/tests/test_graphql_mutations_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/tests/test_graphql_queries_all_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/tests/test_graphql_queries_object_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/tests/test_graphql_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/tests/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/tests/test_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/tests/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:38:21.783751 baseapp_comments-0.1.3/baseapp_comments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7343 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/baseapp_comments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-16 18:38:21.791751 baseapp_comments-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:38:21.791751 baseapp_comments-0.1.3/testproject/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/testproject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/testproject/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/testproject/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/testproject/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:38:21.791751 baseapp_comments-0.1.3/testproject/testapp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/testproject/testapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/testproject/testapp/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/testproject/testapp/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:38:21.791751 baseapp_comments-0.1.3/testproject/testapp/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/testproject/testapp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/testproject/testapp/migrations/0002_auto_20160321_1909.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/testproject/testapp/migrations/0003_auto_20160725_2001.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/testproject/testapp/migrations/0004_auto_20160811_1614.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/testproject/testapp/migrations/0005_user_password_changed_date.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/testproject/testapp/migrations/0006_alter_user_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/testproject/testapp/migrations/0007_user_groups_user_is_staff_user_user_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/testproject/testapp/migrations/0008_user_phone_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/testproject/testapp/migrations/0009_alter_user_options.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/testproject/testapp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/testproject/testapp/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/testproject/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-16 18:38:21.000000 baseapp_comments-0.1.3/testproject/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:39:51.149346 baseapp_comments-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     7343 2024-05-07 15:39:51.153346 baseapp_comments-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:39:51.141346 baseapp_comments-0.1.4/baseapp_comments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:39:51.145346 baseapp_comments-0.1.4/baseapp_comments/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/graphql/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6952 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/graphql/mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/graphql/object_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/graphql/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/graphql/subscriptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:39:51.145346 baseapp_comments-0.1.4/baseapp_comments/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    17671 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/migrations/0002_alter_comment_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/migrations/0003_alter_comment_comments_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/migrations/0004_remove_comment_snapshot_insert_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6279 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/migrations/0005_remove_comment_snapshot_insert_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:39:51.149346 baseapp_comments-0.1.4/baseapp_comments/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/tests/test_comments_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/tests/test_graphql_mutations_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/tests/test_graphql_mutations_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/tests/test_graphql_mutations_pin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/tests/test_graphql_mutations_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/tests/test_graphql_queries_all_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/tests/test_graphql_queries_object_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/tests/test_graphql_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/tests/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/tests/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/tests/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/baseapp_comments/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:39:51.145346 baseapp_comments-0.1.4/baseapp_comments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7343 2024-05-07 15:39:50.000000 baseapp_comments-0.1.4/baseapp_comments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-07 15:39:51.000000 baseapp_comments-0.1.4/baseapp_comments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 15:39:50.000000 baseapp_comments-0.1.4/baseapp_comments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-07 15:39:50.000000 baseapp_comments-0.1.4/baseapp_comments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 15:39:50.000000 baseapp_comments-0.1.4/baseapp_comments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-07 15:39:51.153346 baseapp_comments-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:39:51.149346 baseapp_comments-0.1.4/testproject/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/testproject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/testproject/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/testproject/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/testproject/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:39:51.149346 baseapp_comments-0.1.4/testproject/testapp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/testproject/testapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/testproject/testapp/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/testproject/testapp/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:39:51.149346 baseapp_comments-0.1.4/testproject/testapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/testproject/testapp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/testproject/testapp/migrations/0002_auto_20160321_1909.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/testproject/testapp/migrations/0003_auto_20160725_2001.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/testproject/testapp/migrations/0004_auto_20160811_1614.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/testproject/testapp/migrations/0005_user_password_changed_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/testproject/testapp/migrations/0006_alter_user_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/testproject/testapp/migrations/0007_user_groups_user_is_staff_user_user_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/testproject/testapp/migrations/0008_user_phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/testproject/testapp/migrations/0009_alter_user_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/testproject/testapp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/testproject/testapp/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/testproject/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 15:39:48.000000 baseapp_comments-0.1.4/testproject/wsgi.py
```

### Comparing `baseapp_comments-0.1.3/PKG-INFO` & `baseapp_comments-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseapp_comments
-Version: 0.1.3
+Version: 0.1.4
 Summary: BaseApp Comments
 Home-page: https://github.com/silverlogic/baseapp-backend
 Author: The SilverLogic
 Author-email: dev@tsl.io
 License: BSD-3-Clause  # Example license
 Description: # BaseApp Comments
```

### Comparing `baseapp_comments-0.1.3/README.md` & `baseapp_comments-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/baseapp_comments/admin.py` & `baseapp_comments-0.1.4/baseapp_comments/admin.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/baseapp_comments/graphql/filters.py` & `baseapp_comments-0.1.4/baseapp_comments/graphql/filters.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/baseapp_comments/graphql/mutations.py` & `baseapp_comments-0.1.4/baseapp_comments/graphql/mutations.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/baseapp_comments/graphql/object_types.py` & `baseapp_comments-0.1.4/baseapp_comments/graphql/object_types.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/baseapp_comments/graphql/queries.py` & `baseapp_comments-0.1.4/baseapp_comments/graphql/queries.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/baseapp_comments/graphql/subscriptions.py` & `baseapp_comments-0.1.4/baseapp_comments/graphql/subscriptions.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/baseapp_comments/migrations/0001_initial.py` & `baseapp_comments-0.1.4/baseapp_comments/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/baseapp_comments/migrations/0002_alter_comment_user.py` & `baseapp_comments-0.1.4/baseapp_comments/migrations/0002_alter_comment_user.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/baseapp_comments/migrations/0003_alter_comment_comments_count.py` & `baseapp_comments-0.1.4/baseapp_comments/migrations/0003_alter_comment_comments_count.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/baseapp_comments/migrations/0004_remove_comment_snapshot_insert_and_more.py` & `baseapp_comments-0.1.4/baseapp_comments/migrations/0004_remove_comment_snapshot_insert_and_more.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/baseapp_comments/models.py` & `baseapp_comments-0.1.4/baseapp_comments/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pghistory
 import pgtrigger
 import swapper
 from baseapp_core.graphql import RelayModel
 from baseapp_reactions.models import ReactableModel
+from baseapp_reports.models import ReportableModel
 from django.conf import settings
 from django.contrib.contenttypes.fields import GenericForeignKey, GenericRelation
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 from model_utils.models import TimeStampedModel
 
@@ -45,15 +46,17 @@
 class NonDeletedComments(models.Manager):
     """Automatically filters out soft deleted objects from QuerySets"""
 
     def get_queryset(self):
         return super(NonDeletedComments, self).get_queryset().exclude(status=CommentStatus.DELETED)
 
 
-class AbstractComment(TimeStampedModel, AbstractCommentableModel, ReactableModel, RelayModel):
+class AbstractComment(
+    TimeStampedModel, AbstractCommentableModel, ReactableModel, ReportableModel, RelayModel
+):
     user = models.ForeignKey(
         settings.AUTH_USER_MODEL,
         verbose_name=_("user"),
         related_name="comments",
         on_delete=models.SET_NULL,
         null=True,
         blank=True,
```

### Comparing `baseapp_comments-0.1.3/baseapp_comments/notifications.py` & `baseapp_comments-0.1.4/baseapp_comments/notifications.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/baseapp_comments/permissions.py` & `baseapp_comments-0.1.4/baseapp_comments/permissions.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/baseapp_comments/signals.py` & `baseapp_comments-0.1.4/baseapp_comments/signals.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/baseapp_comments/tests/factories.py` & `baseapp_comments-0.1.4/baseapp_comments/tests/factories.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/baseapp_comments/tests/test_comments_count.py` & `baseapp_comments-0.1.4/baseapp_comments/tests/test_comments_count.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/baseapp_comments/tests/test_graphql_mutations_create.py` & `baseapp_comments-0.1.4/baseapp_comments/tests/test_graphql_mutations_create.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/baseapp_comments/tests/test_graphql_mutations_delete.py` & `baseapp_comments-0.1.4/baseapp_comments/tests/test_graphql_mutations_delete.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/baseapp_comments/tests/test_graphql_mutations_pin.py` & `baseapp_comments-0.1.4/baseapp_comments/tests/test_graphql_mutations_pin.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/baseapp_comments/tests/test_graphql_mutations_update.py` & `baseapp_comments-0.1.4/baseapp_comments/tests/test_graphql_mutations_update.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/baseapp_comments/tests/test_graphql_queries_all_comments.py` & `baseapp_comments-0.1.4/baseapp_comments/tests/test_graphql_queries_all_comments.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/baseapp_comments/tests/test_graphql_queries_object_comments.py` & `baseapp_comments-0.1.4/baseapp_comments/tests/test_graphql_queries_object_comments.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/baseapp_comments/tests/test_graphql_subscriptions.py` & `baseapp_comments-0.1.4/baseapp_comments/tests/test_graphql_subscriptions.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/baseapp_comments/tests/test_notifications.py` & `baseapp_comments-0.1.4/baseapp_comments/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/baseapp_comments/tests/test_users.py` & `baseapp_comments-0.1.4/baseapp_comments/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/baseapp_comments/tests/test_validators.py` & `baseapp_comments-0.1.4/baseapp_comments/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/baseapp_comments/validators.py` & `baseapp_comments-0.1.4/baseapp_comments/validators.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/baseapp_comments.egg-info/PKG-INFO` & `baseapp_comments-0.1.4/baseapp_comments.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseapp-comments
-Version: 0.1.3
+Version: 0.1.4
 Summary: BaseApp Comments
 Home-page: https://github.com/silverlogic/baseapp-backend
 Author: The SilverLogic
 Author-email: dev@tsl.io
 License: BSD-3-Clause  # Example license
 Description: # BaseApp Comments
```

### Comparing `baseapp_comments-0.1.3/baseapp_comments.egg-info/SOURCES.txt` & `baseapp_comments-0.1.4/baseapp_comments.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 baseapp_comments/graphql/object_types.py
 baseapp_comments/graphql/queries.py
 baseapp_comments/graphql/subscriptions.py
 baseapp_comments/migrations/0001_initial.py
 baseapp_comments/migrations/0002_alter_comment_user.py
 baseapp_comments/migrations/0003_alter_comment_comments_count.py
 baseapp_comments/migrations/0004_remove_comment_snapshot_insert_and_more.py
+baseapp_comments/migrations/0005_remove_comment_snapshot_insert_and_more.py
 baseapp_comments/migrations/__init__.py
 baseapp_comments/tests/__init__.py
 baseapp_comments/tests/conftest.py
 baseapp_comments/tests/factories.py
 baseapp_comments/tests/test_comments_count.py
 baseapp_comments/tests/test_graphql_mutations_create.py
 baseapp_comments/tests/test_graphql_mutations_delete.py
```

### Comparing `baseapp_comments-0.1.3/setup.cfg` & `baseapp_comments-0.1.4/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = baseapp_comments
-version = 0.1.3
+version = 0.1.4
 description = BaseApp Comments
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/silverlogic/baseapp-backend
 author = The SilverLogic
 author_email = dev@tsl.io
 license = BSD-3-Clause  # Example license
@@ -14,14 +14,15 @@
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	baseapp-core[graphql] >= 0.2.9
 	baseapp-auth >= 0.2
 	baseapp-notifications >= 0.1
 	baseapp-reactions >= 0.1.8
+	baseapp-reports >= 0.0.1
 
 [options.package_data]
 baseapp_comments = 
 	*.j2
 	*.html
 	*.png
```

### Comparing `baseapp_comments-0.1.3/testproject/graphql.py` & `baseapp_comments-0.1.4/testproject/graphql.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/testproject/settings.py` & `baseapp_comments-0.1.4/testproject/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 # Application definition
 INSTALLED_APPS += [
     "graphene_django",
     "baseapp_notifications",
     "baseapp_reactions",
     "baseapp_comments",
+    "baseapp_reports",
     "baseapp_auth",
     "testproject.testapp",
 ]
 
 ROOT_URLCONF = "testproject.urls"
 
 # Auth
```

### Comparing `baseapp_comments-0.1.3/testproject/testapp/migrations/0001_initial.py` & `baseapp_comments-0.1.4/testproject/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/testproject/testapp/migrations/0002_auto_20160321_1909.py` & `baseapp_comments-0.1.4/testproject/testapp/migrations/0002_auto_20160321_1909.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/testproject/testapp/migrations/0003_auto_20160725_2001.py` & `baseapp_comments-0.1.4/testproject/testapp/migrations/0003_auto_20160725_2001.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/testproject/testapp/migrations/0004_auto_20160811_1614.py` & `baseapp_comments-0.1.4/testproject/testapp/migrations/0004_auto_20160811_1614.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/testproject/testapp/migrations/0005_user_password_changed_date.py` & `baseapp_comments-0.1.4/testproject/testapp/migrations/0005_user_password_changed_date.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/testproject/testapp/migrations/0006_alter_user_id.py` & `baseapp_comments-0.1.4/testproject/testapp/migrations/0006_alter_user_id.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/testproject/testapp/migrations/0007_user_groups_user_is_staff_user_user_permissions.py` & `baseapp_comments-0.1.4/testproject/testapp/migrations/0007_user_groups_user_is_staff_user_user_permissions.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/testproject/testapp/migrations/0009_alter_user_options.py` & `baseapp_comments-0.1.4/testproject/testapp/migrations/0009_alter_user_options.py`

 * *Files identical despite different names*

### Comparing `baseapp_comments-0.1.3/testproject/testapp/models.py` & `baseapp_comments-0.1.4/testproject/testapp/models.py`

 * *Files identical despite different names*

