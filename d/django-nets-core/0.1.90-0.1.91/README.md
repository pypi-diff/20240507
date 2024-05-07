# Comparing `tmp/django_nets_core-0.1.90.tar.gz` & `tmp/django_nets_core-0.1.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_nets_core-0.1.90.tar", last modified: Tue May  7 17:48:03 2024, max compression
+gzip compressed data, was "django_nets_core-0.1.91.tar", last modified: Tue May  7 18:00:00 2024, max compression
```

## Comparing `django_nets_core-0.1.90.tar` & `django_nets_core-0.1.91.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:48:03.590879 django_nets_core-0.1.90/
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.90/LICENSE
--rw-rw-r--   0 dev       (1001) dev       (1001)      396 2024-05-07 17:28:08.000000 django_nets_core-0.1.90/MANIFEST.in
--rw-r--r--   0 dev       (1001) dev       (1001)    13678 2024-05-07 17:48:03.590879 django_nets_core-0.1.90/PKG-INFO
--rw-rw-r--   0 dev       (1001) dev       (1001)    12153 2024-05-05 18:59:42.000000 django_nets_core-0.1.90/README.rst
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:48:03.590879 django_nets_core-0.1.90/django_nets_core.egg-info/
--rw-r--r--   0 dev       (1001) dev       (1001)    13678 2024-05-07 17:48:03.000000 django_nets_core-0.1.90/django_nets_core.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1001) dev       (1001)     2299 2024-05-07 17:48:03.000000 django_nets_core-0.1.90/django_nets_core.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)        1 2024-05-07 17:48:03.000000 django_nets_core-0.1.90/django_nets_core.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)      286 2024-05-07 17:48:03.000000 django_nets_core-0.1.90/django_nets_core.egg-info/requires.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)       10 2024-05-07 17:48:03.000000 django_nets_core-0.1.90/django_nets_core.egg-info/top_level.txt
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:48:03.586879 django_nets_core-0.1.90/nets_core/
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.90/nets_core/__init__.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2440 2024-05-05 19:35:20.000000 django_nets_core-0.1.90/nets_core/admin.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      665 2024-05-07 16:47:52.000000 django_nets_core-0.1.90/nets_core/apps.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      807 2024-05-05 05:05:51.000000 django_nets_core-0.1.90/nets_core/asgi.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      537 2024-05-04 23:43:26.000000 django_nets_core-0.1.90/nets_core/auth_urls.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      229 2024-05-05 05:05:51.000000 django_nets_core-0.1.90/nets_core/celery.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     4901 2024-05-05 18:50:21.000000 django_nets_core-0.1.90/nets_core/decorators.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3276 2024-05-04 23:43:26.000000 django_nets_core-0.1.90/nets_core/firebase_messages.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     6465 2024-05-04 23:43:26.000000 django_nets_core-0.1.90/nets_core/handlers.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2502 2024-05-07 16:19:36.000000 django_nets_core-0.1.90/nets_core/listeners.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     4460 2024-05-05 18:01:33.000000 django_nets_core-0.1.90/nets_core/mail.py
--rwxrwxr-x   0 dev       (1001) dev       (1001)      665 2024-05-04 23:43:26.000000 django_nets_core-0.1.90/nets_core/manage.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:48:03.582879 django_nets_core-0.1.90/nets_core/management/
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:48:03.586879 django_nets_core-0.1.90/nets_core/management/commands/
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-05 02:03:24.000000 django_nets_core-0.1.90/nets_core/management/commands/__init__.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:48:03.586879 django_nets_core-0.1.90/nets_core/management/commands/__pycache__/
--rw-rw-r--   0 dev       (1001) dev       (1001)      165 2024-05-05 02:44:07.000000 django_nets_core-0.1.90/nets_core/management/commands/__pycache__/__init__.cpython-312.pyc
--rw-rw-r--   0 dev       (1001) dev       (1001)    28055 2024-05-05 05:05:51.000000 django_nets_core-0.1.90/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc
--rw-rw-r--   0 dev       (1001) dev       (1001)    22259 2024-05-05 19:59:37.000000 django_nets_core-0.1.90/nets_core/management/commands/nets-settings.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:48:03.586879 django_nets_core-0.1.90/nets_core/middleware/
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:48:03.586879 django_nets_core-0.1.90/nets_core/middleware/__pycache__/
--rw-rw-r--   0 dev       (1001) dev       (1001)     3004 2024-05-05 04:39:30.000000 django_nets_core-0.1.90/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc
--rw-rw-r--   0 dev       (1001) dev       (1001)     2113 2024-05-05 19:54:31.000000 django_nets_core-0.1.90/nets_core/middleware/auth_token.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:48:03.590879 django_nets_core-0.1.90/nets_core/migrations/
--rw-rw-r--   0 dev       (1001) dev       (1001)     5274 2024-05-04 23:43:26.000000 django_nets_core-0.1.90/nets_core/migrations/0001_initial.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      422 2024-05-04 23:43:26.000000 django_nets_core-0.1.90/nets_core/migrations/0002_alter_verificationcode_token.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2208 2024-05-04 23:43:26.000000 django_nets_core-0.1.90/nets_core/migrations/0003_userdevice.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      360 2024-05-04 23:43:26.000000 django_nets_core-0.1.90/nets_core/migrations/0004_remove_userdevice_device_id_userdevice_uuid.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      480 2024-05-04 23:43:26.000000 django_nets_core-0.1.90/nets_core/migrations/0005_userdevice_uuid.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      454 2024-05-04 23:43:26.000000 django_nets_core-0.1.90/nets_core/migrations/0006_verificationcode_device.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      533 2024-05-04 23:43:26.000000 django_nets_core-0.1.90/nets_core/migrations/0007_alter_verificationcode_device.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2056 2024-05-04 23:43:26.000000 django_nets_core-0.1.90/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      455 2024-05-04 23:43:26.000000 django_nets_core-0.1.90/nets_core/migrations/0009_userdevice_ip.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     6844 2024-05-05 19:06:27.000000 django_nets_core-0.1.90/nets_core/migrations/0010_permission_role_userrole_and_more.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      427 2024-05-05 19:35:28.000000 django_nets_core-0.1.90/nets_core/migrations/0011_role_enabled.py
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.90/nets_core/migrations/__init__.py
--rw-rw-r--   0 dev       (1001) dev       (1001)    14303 2024-05-07 17:42:53.000000 django_nets_core-0.1.90/nets_core/models.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     6425 2024-05-04 23:43:26.000000 django_nets_core-0.1.90/nets_core/params.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:48:03.590879 django_nets_core-0.1.90/nets_core/procedures/
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:48:03.590879 django_nets_core-0.1.90/nets_core/procedures/__pycache__/
--rw-rw-r--   0 dev       (1001) dev       (1001)     1511 2024-05-07 16:19:56.000000 django_nets_core-0.1.90/nets_core/procedures/__pycache__/create_nets_core_functions.cpython-312.pyc
--rw-rw-r--   0 dev       (1001) dev       (1001)     1607 2024-05-07 17:30:24.000000 django_nets_core-0.1.90/nets_core/procedures/__pycache__/nets_core_functions.cpython-312.pyc
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:48:03.590879 django_nets_core-0.1.90/nets_core/procedures/functions/
--rw-rw-r--   0 dev       (1001) dev       (1001)     2269 2024-05-07 17:47:54.000000 django_nets_core-0.1.90/nets_core/procedures/functions/nets_core_postgresql_model_to_json.sql
--rw-rw-r--   0 dev       (1001) dev       (1001)     1284 2024-05-07 17:33:26.000000 django_nets_core-0.1.90/nets_core/procedures/nets_core_functions.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      902 2024-05-04 23:43:26.000000 django_nets_core-0.1.90/nets_core/responses.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3055 2024-05-04 23:43:26.000000 django_nets_core-0.1.90/nets_core/security.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2490 2024-05-07 17:24:57.000000 django_nets_core-0.1.90/nets_core/serializers.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3387 2024-05-05 18:22:43.000000 django_nets_core-0.1.90/nets_core/settings.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     1820 2024-05-05 05:05:51.000000 django_nets_core-0.1.90/nets_core/settings_nets.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      753 2024-05-05 05:16:02.000000 django_nets_core-0.1.90/nets_core/tasks.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:48:03.582879 django_nets_core-0.1.90/nets_core/templates/
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:48:03.590879 django_nets_core-0.1.90/nets_core/templates/nets_core/
--rw-rw-r--   0 dev       (1001) dev       (1001)     6978 2024-05-04 23:43:26.000000 django_nets_core-0.1.90/nets_core/templates/nets_core/base.html
--rw-rw-r--   0 dev       (1001) dev       (1001)     1954 2024-05-04 23:43:26.000000 django_nets_core-0.1.90/nets_core/templates/nets_core/delete_account.html
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-05 18:03:29.000000 django_nets_core-0.1.90/nets_core/templates/nets_core/delete_account_info.html
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:48:03.590879 django_nets_core-0.1.90/nets_core/templates/nets_core/email/
--rw-rw-r--   0 dev       (1001) dev       (1001)    16103 2024-05-04 23:43:26.000000 django_nets_core-0.1.90/nets_core/templates/nets_core/email/base_email.html
--rw-rw-r--   0 dev       (1001) dev       (1001)     1032 2024-05-04 23:43:26.000000 django_nets_core-0.1.90/nets_core/templates/nets_core/email/new_login.html
--rw-rw-r--   0 dev       (1001) dev       (1001)      316 2024-05-04 23:43:26.000000 django_nets_core-0.1.90/nets_core/templates/nets_core/email/verification_code.html
--rw-rw-r--   0 dev       (1001) dev       (1001)      824 2024-05-04 23:43:26.000000 django_nets_core-0.1.90/nets_core/urls.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3003 2024-05-05 18:49:07.000000 django_nets_core-0.1.90/nets_core/utils.py
--rw-rw-r--   0 dev       (1001) dev       (1001)    11727 2024-05-05 18:04:42.000000 django_nets_core-0.1.90/nets_core/views.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      395 2024-05-04 23:43:26.000000 django_nets_core-0.1.90/nets_core/wsgi.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      100 2024-05-05 00:47:40.000000 django_nets_core-0.1.90/pyproject.toml
--rw-rw-r--   0 dev       (1001) dev       (1001)      181 2024-05-05 01:49:02.000000 django_nets_core-0.1.90/requirements.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)     1334 2024-05-07 17:48:03.590879 django_nets_core-0.1.90/setup.cfg
--rw-rw-r--   0 dev       (1001) dev       (1001)       38 2024-05-04 23:43:26.000000 django_nets_core-0.1.90/setup.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.896583 django_nets_core-0.1.91/
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/LICENSE
+-rw-rw-r--   0 dev       (1001) dev       (1001)      396 2024-05-07 17:28:08.000000 django_nets_core-0.1.91/MANIFEST.in
+-rw-r--r--   0 dev       (1001) dev       (1001)    14299 2024-05-07 18:00:00.896583 django_nets_core-0.1.91/PKG-INFO
+-rw-rw-r--   0 dev       (1001) dev       (1001)    12774 2024-05-07 17:59:28.000000 django_nets_core-0.1.91/README.rst
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.896583 django_nets_core-0.1.91/django_nets_core.egg-info/
+-rw-r--r--   0 dev       (1001) dev       (1001)    14299 2024-05-07 18:00:00.000000 django_nets_core-0.1.91/django_nets_core.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2299 2024-05-07 18:00:00.000000 django_nets_core-0.1.91/django_nets_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)        1 2024-05-07 18:00:00.000000 django_nets_core-0.1.91/django_nets_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)      286 2024-05-07 18:00:00.000000 django_nets_core-0.1.91/django_nets_core.egg-info/requires.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)       10 2024-05-07 18:00:00.000000 django_nets_core-0.1.91/django_nets_core.egg-info/top_level.txt
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.892583 django_nets_core-0.1.91/nets_core/
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/__init__.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2440 2024-05-05 19:35:20.000000 django_nets_core-0.1.91/nets_core/admin.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      665 2024-05-07 16:47:52.000000 django_nets_core-0.1.91/nets_core/apps.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      807 2024-05-05 05:05:51.000000 django_nets_core-0.1.91/nets_core/asgi.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      537 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/auth_urls.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      229 2024-05-05 05:05:51.000000 django_nets_core-0.1.91/nets_core/celery.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     4901 2024-05-05 18:50:21.000000 django_nets_core-0.1.91/nets_core/decorators.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3276 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/firebase_messages.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6465 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/handlers.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2502 2024-05-07 16:19:36.000000 django_nets_core-0.1.91/nets_core/listeners.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     4460 2024-05-05 18:01:33.000000 django_nets_core-0.1.91/nets_core/mail.py
+-rwxrwxr-x   0 dev       (1001) dev       (1001)      665 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/manage.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.888583 django_nets_core-0.1.91/nets_core/management/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.892583 django_nets_core-0.1.91/nets_core/management/commands/
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-05 02:03:24.000000 django_nets_core-0.1.91/nets_core/management/commands/__init__.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.892583 django_nets_core-0.1.91/nets_core/management/commands/__pycache__/
+-rw-rw-r--   0 dev       (1001) dev       (1001)      165 2024-05-05 02:44:07.000000 django_nets_core-0.1.91/nets_core/management/commands/__pycache__/__init__.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)    28055 2024-05-05 05:05:51.000000 django_nets_core-0.1.91/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)    22259 2024-05-05 19:59:37.000000 django_nets_core-0.1.91/nets_core/management/commands/nets-settings.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.892583 django_nets_core-0.1.91/nets_core/middleware/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.892583 django_nets_core-0.1.91/nets_core/middleware/__pycache__/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3004 2024-05-05 04:39:30.000000 django_nets_core-0.1.91/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2113 2024-05-05 19:54:31.000000 django_nets_core-0.1.91/nets_core/middleware/auth_token.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.896583 django_nets_core-0.1.91/nets_core/migrations/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     5274 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/migrations/0001_initial.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      422 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/migrations/0002_alter_verificationcode_token.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2208 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/migrations/0003_userdevice.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      360 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/migrations/0004_remove_userdevice_device_id_userdevice_uuid.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      480 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/migrations/0005_userdevice_uuid.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      454 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/migrations/0006_verificationcode_device.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      533 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/migrations/0007_alter_verificationcode_device.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2056 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      455 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/migrations/0009_userdevice_ip.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6844 2024-05-05 19:06:27.000000 django_nets_core-0.1.91/nets_core/migrations/0010_permission_role_userrole_and_more.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      427 2024-05-05 19:35:28.000000 django_nets_core-0.1.91/nets_core/migrations/0011_role_enabled.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/migrations/__init__.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)    14960 2024-05-07 17:51:02.000000 django_nets_core-0.1.91/nets_core/models.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6425 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/params.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.896583 django_nets_core-0.1.91/nets_core/procedures/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.896583 django_nets_core-0.1.91/nets_core/procedures/__pycache__/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1511 2024-05-07 16:19:56.000000 django_nets_core-0.1.91/nets_core/procedures/__pycache__/create_nets_core_functions.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1607 2024-05-07 17:30:24.000000 django_nets_core-0.1.91/nets_core/procedures/__pycache__/nets_core_functions.cpython-312.pyc
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.896583 django_nets_core-0.1.91/nets_core/procedures/functions/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2269 2024-05-07 17:47:54.000000 django_nets_core-0.1.91/nets_core/procedures/functions/nets_core_postgresql_model_to_json.sql
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1284 2024-05-07 17:33:26.000000 django_nets_core-0.1.91/nets_core/procedures/nets_core_functions.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      902 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/responses.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3055 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/security.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2490 2024-05-07 17:24:57.000000 django_nets_core-0.1.91/nets_core/serializers.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3387 2024-05-05 18:22:43.000000 django_nets_core-0.1.91/nets_core/settings.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1820 2024-05-05 05:05:51.000000 django_nets_core-0.1.91/nets_core/settings_nets.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      753 2024-05-05 05:16:02.000000 django_nets_core-0.1.91/nets_core/tasks.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.888583 django_nets_core-0.1.91/nets_core/templates/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.896583 django_nets_core-0.1.91/nets_core/templates/nets_core/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6978 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/templates/nets_core/base.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1954 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/templates/nets_core/delete_account.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-05 18:03:29.000000 django_nets_core-0.1.91/nets_core/templates/nets_core/delete_account_info.html
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.896583 django_nets_core-0.1.91/nets_core/templates/nets_core/email/
+-rw-rw-r--   0 dev       (1001) dev       (1001)    16103 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/templates/nets_core/email/base_email.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1032 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/templates/nets_core/email/new_login.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)      316 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/templates/nets_core/email/verification_code.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)      824 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/urls.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3003 2024-05-05 18:49:07.000000 django_nets_core-0.1.91/nets_core/utils.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)    11727 2024-05-05 18:04:42.000000 django_nets_core-0.1.91/nets_core/views.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      395 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/wsgi.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      100 2024-05-05 00:47:40.000000 django_nets_core-0.1.91/pyproject.toml
+-rw-rw-r--   0 dev       (1001) dev       (1001)      181 2024-05-05 01:49:02.000000 django_nets_core-0.1.91/requirements.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1334 2024-05-07 18:00:00.896583 django_nets_core-0.1.91/setup.cfg
+-rw-rw-r--   0 dev       (1001) dev       (1001)       38 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/setup.py
```

### Comparing `django_nets_core-0.1.90/PKG-INFO` & `django_nets_core-0.1.91/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-nets-core
-Version: 0.1.90
+Version: 0.1.91
 Summary: A lazy API rest request handler.
 Home-page: https://github.com/esbozos/django-nets-core
 Author: Norman Torres
 Author-email: norman.nets@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -209,36 +209,45 @@
 
 Note that both models should be defined in your settings file. Both require def __str__(self): to be defined.
 If enabled roles and permissions will be check over project and membership enabled	
 example of models:
 
 .. code-block:: python
 
-    class MyProjectModel(models.Model):
+    from nets_core.models import OwnedModel, NetsCoreBaseModel
+    # use of OwnedModel is optional, but recommended to include user, created and updated fields, 
+    # if not used, include user, created and updated fields in your model
+    class MyProjectModel(OwnedModel):
         name = models.CharField(max_length=255)
         enabled = models.BooleanField(default=True)
         description = models.TextField(blank=True, null=True)
         created_at = models.DateTimeField(auto_now_add=True)
         updated_at = models.DateTimeField(auto_now=True)
 
         def __str__(self):
             return self.name
 
-    class MyProjectMemberModel(models.Model):
-        project = models.ForeignKey(MyProjectModel, on_delete=models.CASCADE)
-        user = models.ForeignKey(User, on_delete=models.CASCADE) # User from django.contrib.auth.models or your custom user model
+    class MyProjectMemberModel(OwnedModel):
+        project = models.ForeignKey(MyProjectModel, on_delete=models.CASCADE)        
         is_superuser = models.BooleanField(default=False)
         enabled = models.BooleanField(default=True)
         created_at = models.DateTimeField(auto_now_add=True)
         updated_at = models.DateTimeField(auto_now=True)
 
         def __str__(self):
             return f'{self.user} - {self.project}'
 
-Setting  is_superuser to True will give user superuser permissions over project
+Setting  is_superuser to True will give user superuser permissions over project, OwnedModel is Abstract model that include user, created and updated fields
+
+.. warning::
+
+    NetsCoreBaseModel is an abstract model that include created and updated fields and implements to_json method that allow to serialize model to json
+    passing fields as tuple to include or "__all__" to include. This is a store function in database for fast access to json data.
+    TODO: include examples of use to serialize model to json based on fields required per view or endpoint. Inspired in Facebook GraphQL
+
 
 Set verification code expire time
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. code-block:: python
 
     NETS_CORE_VERIFICATION_CODE_EXPIRE_SECONDS = 15*60 # 900 seconds
```

### Comparing `django_nets_core-0.1.90/README.rst` & `django_nets_core-0.1.91/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -168,36 +168,45 @@
 
 Note that both models should be defined in your settings file. Both require def __str__(self): to be defined.
 If enabled roles and permissions will be check over project and membership enabled	
 example of models:
 
 .. code-block:: python
 
-    class MyProjectModel(models.Model):
+    from nets_core.models import OwnedModel, NetsCoreBaseModel
+    # use of OwnedModel is optional, but recommended to include user, created and updated fields, 
+    # if not used, include user, created and updated fields in your model
+    class MyProjectModel(OwnedModel):
         name = models.CharField(max_length=255)
         enabled = models.BooleanField(default=True)
         description = models.TextField(blank=True, null=True)
         created_at = models.DateTimeField(auto_now_add=True)
         updated_at = models.DateTimeField(auto_now=True)
 
         def __str__(self):
             return self.name
 
-    class MyProjectMemberModel(models.Model):
-        project = models.ForeignKey(MyProjectModel, on_delete=models.CASCADE)
-        user = models.ForeignKey(User, on_delete=models.CASCADE) # User from django.contrib.auth.models or your custom user model
+    class MyProjectMemberModel(OwnedModel):
+        project = models.ForeignKey(MyProjectModel, on_delete=models.CASCADE)        
         is_superuser = models.BooleanField(default=False)
         enabled = models.BooleanField(default=True)
         created_at = models.DateTimeField(auto_now_add=True)
         updated_at = models.DateTimeField(auto_now=True)
 
         def __str__(self):
             return f'{self.user} - {self.project}'
 
-Setting  is_superuser to True will give user superuser permissions over project
+Setting  is_superuser to True will give user superuser permissions over project, OwnedModel is Abstract model that include user, created and updated fields
+
+.. warning::
+
+    NetsCoreBaseModel is an abstract model that include created and updated fields and implements to_json method that allow to serialize model to json
+    passing fields as tuple to include or "__all__" to include. This is a store function in database for fast access to json data.
+    TODO: include examples of use to serialize model to json based on fields required per view or endpoint. Inspired in Facebook GraphQL
+
 
 Set verification code expire time
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. code-block:: python
 
     NETS_CORE_VERIFICATION_CODE_EXPIRE_SECONDS = 15*60 # 900 seconds
```

### Comparing `django_nets_core-0.1.90/django_nets_core.egg-info/PKG-INFO` & `django_nets_core-0.1.91/django_nets_core.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-nets-core
-Version: 0.1.90
+Version: 0.1.91
 Summary: A lazy API rest request handler.
 Home-page: https://github.com/esbozos/django-nets-core
 Author: Norman Torres
 Author-email: norman.nets@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -209,36 +209,45 @@
 
 Note that both models should be defined in your settings file. Both require def __str__(self): to be defined.
 If enabled roles and permissions will be check over project and membership enabled	
 example of models:
 
 .. code-block:: python
 
-    class MyProjectModel(models.Model):
+    from nets_core.models import OwnedModel, NetsCoreBaseModel
+    # use of OwnedModel is optional, but recommended to include user, created and updated fields, 
+    # if not used, include user, created and updated fields in your model
+    class MyProjectModel(OwnedModel):
         name = models.CharField(max_length=255)
         enabled = models.BooleanField(default=True)
         description = models.TextField(blank=True, null=True)
         created_at = models.DateTimeField(auto_now_add=True)
         updated_at = models.DateTimeField(auto_now=True)
 
         def __str__(self):
             return self.name
 
-    class MyProjectMemberModel(models.Model):
-        project = models.ForeignKey(MyProjectModel, on_delete=models.CASCADE)
-        user = models.ForeignKey(User, on_delete=models.CASCADE) # User from django.contrib.auth.models or your custom user model
+    class MyProjectMemberModel(OwnedModel):
+        project = models.ForeignKey(MyProjectModel, on_delete=models.CASCADE)        
         is_superuser = models.BooleanField(default=False)
         enabled = models.BooleanField(default=True)
         created_at = models.DateTimeField(auto_now_add=True)
         updated_at = models.DateTimeField(auto_now=True)
 
         def __str__(self):
             return f'{self.user} - {self.project}'
 
-Setting  is_superuser to True will give user superuser permissions over project
+Setting  is_superuser to True will give user superuser permissions over project, OwnedModel is Abstract model that include user, created and updated fields
+
+.. warning::
+
+    NetsCoreBaseModel is an abstract model that include created and updated fields and implements to_json method that allow to serialize model to json
+    passing fields as tuple to include or "__all__" to include. This is a store function in database for fast access to json data.
+    TODO: include examples of use to serialize model to json based on fields required per view or endpoint. Inspired in Facebook GraphQL
+
 
 Set verification code expire time
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. code-block:: python
 
     NETS_CORE_VERIFICATION_CODE_EXPIRE_SECONDS = 15*60 # 900 seconds
```

### Comparing `django_nets_core-0.1.90/django_nets_core.egg-info/SOURCES.txt` & `django_nets_core-0.1.91/django_nets_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/admin.py` & `django_nets_core-0.1.91/nets_core/admin.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/apps.py` & `django_nets_core-0.1.91/nets_core/apps.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/asgi.py` & `django_nets_core-0.1.91/nets_core/asgi.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/auth_urls.py` & `django_nets_core-0.1.91/nets_core/auth_urls.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/decorators.py` & `django_nets_core-0.1.91/nets_core/decorators.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/firebase_messages.py` & `django_nets_core-0.1.91/nets_core/firebase_messages.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/handlers.py` & `django_nets_core-0.1.91/nets_core/handlers.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/listeners.py` & `django_nets_core-0.1.91/nets_core/listeners.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/mail.py` & `django_nets_core-0.1.91/nets_core/mail.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/manage.py` & `django_nets_core-0.1.91/nets_core/manage.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc` & `django_nets_core-0.1.91/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/management/commands/nets-settings.py` & `django_nets_core-0.1.91/nets_core/management/commands/nets-settings.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc` & `django_nets_core-0.1.91/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/middleware/auth_token.py` & `django_nets_core-0.1.91/nets_core/middleware/auth_token.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/migrations/0001_initial.py` & `django_nets_core-0.1.91/nets_core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/migrations/0003_userdevice.py` & `django_nets_core-0.1.91/nets_core/migrations/0003_userdevice.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/migrations/0007_alter_verificationcode_device.py` & `django_nets_core-0.1.91/nets_core/migrations/0007_alter_verificationcode_device.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py` & `django_nets_core-0.1.91/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/migrations/0010_permission_role_userrole_and_more.py` & `django_nets_core-0.1.91/nets_core/migrations/0010_permission_role_userrole_and_more.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/models.py` & `django_nets_core-0.1.91/nets_core/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,30 @@
     created = models.DateTimeField(_('Created'), auto_now_add=True)
     updated = models.DateTimeField(_('updated'), auto_now=True)
     
     objects = NetsCoreBaseManager()
 
     class Meta:
         abstract = True
+        
+    def to_json(self, fields: tuple = None):
+        if not fields:
+            raise ValueError(_("Fields must be provided"))
+        if fields == '__all__':
+            # get fiels to tupple but names from columns in db table schema, user should be user_id
+            schema = self._meta.get_fields()
+            fields = tuple([field.column for field in schema if hasattr(field, 'column')])
+            
+        
+        if not isinstance(fields, tuple):
+            raise ValueError(_("Fields must be a tuple"))
+        
+        from nets_core.serializers import NetsCoreModelToJson
+        return NetsCoreModelToJson(self, fields).to_json()
+
 
 class OwnedModel(models.Model):
     user = models.ForeignKey(User, on_delete=models.CASCADE)
     created = models.DateTimeField(_('Created'), auto_now_add=True)
     updated = models.DateTimeField(_('updated'), auto_now=True)
     
     objects = NetsCoreBaseManager()
```

### Comparing `django_nets_core-0.1.90/nets_core/params.py` & `django_nets_core-0.1.91/nets_core/params.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/procedures/__pycache__/create_nets_core_functions.cpython-312.pyc` & `django_nets_core-0.1.91/nets_core/procedures/__pycache__/create_nets_core_functions.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/procedures/__pycache__/nets_core_functions.cpython-312.pyc` & `django_nets_core-0.1.91/nets_core/procedures/__pycache__/nets_core_functions.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/procedures/functions/nets_core_postgresql_model_to_json.sql` & `django_nets_core-0.1.91/nets_core/procedures/functions/nets_core_postgresql_model_to_json.sql`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/procedures/nets_core_functions.py` & `django_nets_core-0.1.91/nets_core/procedures/nets_core_functions.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/responses.py` & `django_nets_core-0.1.91/nets_core/responses.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/security.py` & `django_nets_core-0.1.91/nets_core/security.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/serializers.py` & `django_nets_core-0.1.91/nets_core/serializers.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/settings.py` & `django_nets_core-0.1.91/nets_core/settings.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/settings_nets.py` & `django_nets_core-0.1.91/nets_core/settings_nets.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/tasks.py` & `django_nets_core-0.1.91/nets_core/tasks.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/templates/nets_core/base.html` & `django_nets_core-0.1.91/nets_core/templates/nets_core/base.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/templates/nets_core/delete_account.html` & `django_nets_core-0.1.91/nets_core/templates/nets_core/delete_account.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/templates/nets_core/email/base_email.html` & `django_nets_core-0.1.91/nets_core/templates/nets_core/email/base_email.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/templates/nets_core/email/new_login.html` & `django_nets_core-0.1.91/nets_core/templates/nets_core/email/new_login.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/urls.py` & `django_nets_core-0.1.91/nets_core/urls.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/utils.py` & `django_nets_core-0.1.91/nets_core/utils.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/nets_core/views.py` & `django_nets_core-0.1.91/nets_core/views.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.90/setup.cfg` & `django_nets_core-0.1.91/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-nets-core
-version = 0.1.90
+version = 0.1.91
 description = A lazy API rest request handler.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/esbozos/django-nets-core
 author = Norman Torres
 author_email = norman.nets@gmail.com
 license = BSD-3-Clause
```

