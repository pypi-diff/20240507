# Comparing `tmp/django_nets_core-0.1.84.tar.gz` & `tmp/django_nets_core-0.1.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_nets_core-0.1.84.tar", last modified: Tue May  7 17:23:14 2024, max compression
+gzip compressed data, was "django_nets_core-0.1.85.tar", last modified: Tue May  7 17:30:32 2024, max compression
```

## Comparing `django_nets_core-0.1.84.tar` & `django_nets_core-0.1.85.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:23:14.131206 django_nets_core-0.1.84/
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.84/LICENSE
--rw-rw-r--   0 dev       (1001) dev       (1001)      396 2024-05-07 15:50:26.000000 django_nets_core-0.1.84/MANIFEST.in
--rw-r--r--   0 dev       (1001) dev       (1001)    13678 2024-05-07 17:23:14.131206 django_nets_core-0.1.84/PKG-INFO
--rw-rw-r--   0 dev       (1001) dev       (1001)    12153 2024-05-05 18:59:42.000000 django_nets_core-0.1.84/README.rst
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:23:14.131206 django_nets_core-0.1.84/django_nets_core.egg-info/
--rw-r--r--   0 dev       (1001) dev       (1001)    13678 2024-05-07 17:23:14.000000 django_nets_core-0.1.84/django_nets_core.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1001) dev       (1001)     2296 2024-05-07 17:23:14.000000 django_nets_core-0.1.84/django_nets_core.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)        1 2024-05-07 17:23:14.000000 django_nets_core-0.1.84/django_nets_core.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)      286 2024-05-07 17:23:14.000000 django_nets_core-0.1.84/django_nets_core.egg-info/requires.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)       10 2024-05-07 17:23:14.000000 django_nets_core-0.1.84/django_nets_core.egg-info/top_level.txt
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:23:14.127206 django_nets_core-0.1.84/nets_core/
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.84/nets_core/__init__.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2440 2024-05-05 19:35:20.000000 django_nets_core-0.1.84/nets_core/admin.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      665 2024-05-07 16:47:52.000000 django_nets_core-0.1.84/nets_core/apps.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      807 2024-05-05 05:05:51.000000 django_nets_core-0.1.84/nets_core/asgi.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      537 2024-05-04 23:43:26.000000 django_nets_core-0.1.84/nets_core/auth_urls.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      229 2024-05-05 05:05:51.000000 django_nets_core-0.1.84/nets_core/celery.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     4901 2024-05-05 18:50:21.000000 django_nets_core-0.1.84/nets_core/decorators.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3276 2024-05-04 23:43:26.000000 django_nets_core-0.1.84/nets_core/firebase_messages.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     6465 2024-05-04 23:43:26.000000 django_nets_core-0.1.84/nets_core/handlers.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2502 2024-05-07 16:19:36.000000 django_nets_core-0.1.84/nets_core/listeners.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     4460 2024-05-05 18:01:33.000000 django_nets_core-0.1.84/nets_core/mail.py
--rwxrwxr-x   0 dev       (1001) dev       (1001)      665 2024-05-04 23:43:26.000000 django_nets_core-0.1.84/nets_core/manage.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:23:14.123206 django_nets_core-0.1.84/nets_core/management/
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:23:14.131206 django_nets_core-0.1.84/nets_core/management/commands/
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-05 02:03:24.000000 django_nets_core-0.1.84/nets_core/management/commands/__init__.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:23:14.131206 django_nets_core-0.1.84/nets_core/management/commands/__pycache__/
--rw-rw-r--   0 dev       (1001) dev       (1001)      165 2024-05-05 02:44:07.000000 django_nets_core-0.1.84/nets_core/management/commands/__pycache__/__init__.cpython-312.pyc
--rw-rw-r--   0 dev       (1001) dev       (1001)    28055 2024-05-05 05:05:51.000000 django_nets_core-0.1.84/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc
--rw-rw-r--   0 dev       (1001) dev       (1001)    22259 2024-05-05 19:59:37.000000 django_nets_core-0.1.84/nets_core/management/commands/nets-settings.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:23:14.131206 django_nets_core-0.1.84/nets_core/middleware/
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:23:14.131206 django_nets_core-0.1.84/nets_core/middleware/__pycache__/
--rw-rw-r--   0 dev       (1001) dev       (1001)     3004 2024-05-05 04:39:30.000000 django_nets_core-0.1.84/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc
--rw-rw-r--   0 dev       (1001) dev       (1001)     2113 2024-05-05 19:54:31.000000 django_nets_core-0.1.84/nets_core/middleware/auth_token.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:23:14.131206 django_nets_core-0.1.84/nets_core/migrations/
--rw-rw-r--   0 dev       (1001) dev       (1001)     5274 2024-05-04 23:43:26.000000 django_nets_core-0.1.84/nets_core/migrations/0001_initial.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      422 2024-05-04 23:43:26.000000 django_nets_core-0.1.84/nets_core/migrations/0002_alter_verificationcode_token.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2208 2024-05-04 23:43:26.000000 django_nets_core-0.1.84/nets_core/migrations/0003_userdevice.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      360 2024-05-04 23:43:26.000000 django_nets_core-0.1.84/nets_core/migrations/0004_remove_userdevice_device_id_userdevice_uuid.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      480 2024-05-04 23:43:26.000000 django_nets_core-0.1.84/nets_core/migrations/0005_userdevice_uuid.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      454 2024-05-04 23:43:26.000000 django_nets_core-0.1.84/nets_core/migrations/0006_verificationcode_device.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      533 2024-05-04 23:43:26.000000 django_nets_core-0.1.84/nets_core/migrations/0007_alter_verificationcode_device.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2056 2024-05-04 23:43:26.000000 django_nets_core-0.1.84/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      455 2024-05-04 23:43:26.000000 django_nets_core-0.1.84/nets_core/migrations/0009_userdevice_ip.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     6844 2024-05-05 19:06:27.000000 django_nets_core-0.1.84/nets_core/migrations/0010_permission_role_userrole_and_more.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      427 2024-05-05 19:35:28.000000 django_nets_core-0.1.84/nets_core/migrations/0011_role_enabled.py
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.84/nets_core/migrations/__init__.py
--rw-rw-r--   0 dev       (1001) dev       (1001)    14160 2024-05-07 17:09:07.000000 django_nets_core-0.1.84/nets_core/models.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     6425 2024-05-04 23:43:26.000000 django_nets_core-0.1.84/nets_core/params.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:23:14.131206 django_nets_core-0.1.84/nets_core/procedures/
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:23:14.131206 django_nets_core-0.1.84/nets_core/procedures/__pycache__/
--rw-rw-r--   0 dev       (1001) dev       (1001)     1511 2024-05-07 16:19:56.000000 django_nets_core-0.1.84/nets_core/procedures/__pycache__/create_nets_core_functions.cpython-312.pyc
--rw-rw-r--   0 dev       (1001) dev       (1001)     1504 2024-05-07 16:20:53.000000 django_nets_core-0.1.84/nets_core/procedures/__pycache__/nets_core_functions.cpython-312.pyc
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:23:14.131206 django_nets_core-0.1.84/nets_core/procedures/functions/
--rw-rw-r--   0 dev       (1001) dev       (1001)     2266 2024-05-07 17:07:29.000000 django_nets_core-0.1.84/nets_core/procedures/functions/nets_core_postgre_model_to_json.sql
--rw-rw-r--   0 dev       (1001) dev       (1001)     1142 2024-05-07 16:16:05.000000 django_nets_core-0.1.84/nets_core/procedures/nets_core_functions.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      902 2024-05-04 23:43:26.000000 django_nets_core-0.1.84/nets_core/responses.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3055 2024-05-04 23:43:26.000000 django_nets_core-0.1.84/nets_core/security.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2490 2024-05-07 17:23:05.000000 django_nets_core-0.1.84/nets_core/serializers.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3387 2024-05-05 18:22:43.000000 django_nets_core-0.1.84/nets_core/settings.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     1820 2024-05-05 05:05:51.000000 django_nets_core-0.1.84/nets_core/settings_nets.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      753 2024-05-05 05:16:02.000000 django_nets_core-0.1.84/nets_core/tasks.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:23:14.127206 django_nets_core-0.1.84/nets_core/templates/
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:23:14.131206 django_nets_core-0.1.84/nets_core/templates/nets_core/
--rw-rw-r--   0 dev       (1001) dev       (1001)     6978 2024-05-04 23:43:26.000000 django_nets_core-0.1.84/nets_core/templates/nets_core/base.html
--rw-rw-r--   0 dev       (1001) dev       (1001)     1954 2024-05-04 23:43:26.000000 django_nets_core-0.1.84/nets_core/templates/nets_core/delete_account.html
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-05 18:03:29.000000 django_nets_core-0.1.84/nets_core/templates/nets_core/delete_account_info.html
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:23:14.131206 django_nets_core-0.1.84/nets_core/templates/nets_core/email/
--rw-rw-r--   0 dev       (1001) dev       (1001)    16103 2024-05-04 23:43:26.000000 django_nets_core-0.1.84/nets_core/templates/nets_core/email/base_email.html
--rw-rw-r--   0 dev       (1001) dev       (1001)     1032 2024-05-04 23:43:26.000000 django_nets_core-0.1.84/nets_core/templates/nets_core/email/new_login.html
--rw-rw-r--   0 dev       (1001) dev       (1001)      316 2024-05-04 23:43:26.000000 django_nets_core-0.1.84/nets_core/templates/nets_core/email/verification_code.html
--rw-rw-r--   0 dev       (1001) dev       (1001)      824 2024-05-04 23:43:26.000000 django_nets_core-0.1.84/nets_core/urls.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3003 2024-05-05 18:49:07.000000 django_nets_core-0.1.84/nets_core/utils.py
--rw-rw-r--   0 dev       (1001) dev       (1001)    11727 2024-05-05 18:04:42.000000 django_nets_core-0.1.84/nets_core/views.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      395 2024-05-04 23:43:26.000000 django_nets_core-0.1.84/nets_core/wsgi.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      100 2024-05-05 00:47:40.000000 django_nets_core-0.1.84/pyproject.toml
--rw-rw-r--   0 dev       (1001) dev       (1001)      181 2024-05-05 01:49:02.000000 django_nets_core-0.1.84/requirements.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)     1334 2024-05-07 17:23:14.131206 django_nets_core-0.1.84/setup.cfg
--rw-rw-r--   0 dev       (1001) dev       (1001)       38 2024-05-04 23:43:26.000000 django_nets_core-0.1.84/setup.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:30:32.056189 django_nets_core-0.1.85/
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.85/LICENSE
+-rw-rw-r--   0 dev       (1001) dev       (1001)      396 2024-05-07 17:28:08.000000 django_nets_core-0.1.85/MANIFEST.in
+-rw-r--r--   0 dev       (1001) dev       (1001)    13678 2024-05-07 17:30:32.056189 django_nets_core-0.1.85/PKG-INFO
+-rw-rw-r--   0 dev       (1001) dev       (1001)    12153 2024-05-05 18:59:42.000000 django_nets_core-0.1.85/README.rst
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:30:32.056189 django_nets_core-0.1.85/django_nets_core.egg-info/
+-rw-r--r--   0 dev       (1001) dev       (1001)    13678 2024-05-07 17:30:32.000000 django_nets_core-0.1.85/django_nets_core.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2296 2024-05-07 17:30:32.000000 django_nets_core-0.1.85/django_nets_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)        1 2024-05-07 17:30:32.000000 django_nets_core-0.1.85/django_nets_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)      286 2024-05-07 17:30:32.000000 django_nets_core-0.1.85/django_nets_core.egg-info/requires.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)       10 2024-05-07 17:30:32.000000 django_nets_core-0.1.85/django_nets_core.egg-info/top_level.txt
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:30:32.056189 django_nets_core-0.1.85/nets_core/
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.85/nets_core/__init__.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2440 2024-05-05 19:35:20.000000 django_nets_core-0.1.85/nets_core/admin.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      665 2024-05-07 16:47:52.000000 django_nets_core-0.1.85/nets_core/apps.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      807 2024-05-05 05:05:51.000000 django_nets_core-0.1.85/nets_core/asgi.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      537 2024-05-04 23:43:26.000000 django_nets_core-0.1.85/nets_core/auth_urls.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      229 2024-05-05 05:05:51.000000 django_nets_core-0.1.85/nets_core/celery.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     4901 2024-05-05 18:50:21.000000 django_nets_core-0.1.85/nets_core/decorators.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3276 2024-05-04 23:43:26.000000 django_nets_core-0.1.85/nets_core/firebase_messages.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6465 2024-05-04 23:43:26.000000 django_nets_core-0.1.85/nets_core/handlers.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2502 2024-05-07 16:19:36.000000 django_nets_core-0.1.85/nets_core/listeners.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     4460 2024-05-05 18:01:33.000000 django_nets_core-0.1.85/nets_core/mail.py
+-rwxrwxr-x   0 dev       (1001) dev       (1001)      665 2024-05-04 23:43:26.000000 django_nets_core-0.1.85/nets_core/manage.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:30:32.052189 django_nets_core-0.1.85/nets_core/management/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:30:32.056189 django_nets_core-0.1.85/nets_core/management/commands/
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-05 02:03:24.000000 django_nets_core-0.1.85/nets_core/management/commands/__init__.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:30:32.056189 django_nets_core-0.1.85/nets_core/management/commands/__pycache__/
+-rw-rw-r--   0 dev       (1001) dev       (1001)      165 2024-05-05 02:44:07.000000 django_nets_core-0.1.85/nets_core/management/commands/__pycache__/__init__.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)    28055 2024-05-05 05:05:51.000000 django_nets_core-0.1.85/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)    22259 2024-05-05 19:59:37.000000 django_nets_core-0.1.85/nets_core/management/commands/nets-settings.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:30:32.056189 django_nets_core-0.1.85/nets_core/middleware/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:30:32.056189 django_nets_core-0.1.85/nets_core/middleware/__pycache__/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3004 2024-05-05 04:39:30.000000 django_nets_core-0.1.85/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2113 2024-05-05 19:54:31.000000 django_nets_core-0.1.85/nets_core/middleware/auth_token.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:30:32.056189 django_nets_core-0.1.85/nets_core/migrations/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     5274 2024-05-04 23:43:26.000000 django_nets_core-0.1.85/nets_core/migrations/0001_initial.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      422 2024-05-04 23:43:26.000000 django_nets_core-0.1.85/nets_core/migrations/0002_alter_verificationcode_token.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2208 2024-05-04 23:43:26.000000 django_nets_core-0.1.85/nets_core/migrations/0003_userdevice.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      360 2024-05-04 23:43:26.000000 django_nets_core-0.1.85/nets_core/migrations/0004_remove_userdevice_device_id_userdevice_uuid.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      480 2024-05-04 23:43:26.000000 django_nets_core-0.1.85/nets_core/migrations/0005_userdevice_uuid.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      454 2024-05-04 23:43:26.000000 django_nets_core-0.1.85/nets_core/migrations/0006_verificationcode_device.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      533 2024-05-04 23:43:26.000000 django_nets_core-0.1.85/nets_core/migrations/0007_alter_verificationcode_device.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2056 2024-05-04 23:43:26.000000 django_nets_core-0.1.85/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      455 2024-05-04 23:43:26.000000 django_nets_core-0.1.85/nets_core/migrations/0009_userdevice_ip.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6844 2024-05-05 19:06:27.000000 django_nets_core-0.1.85/nets_core/migrations/0010_permission_role_userrole_and_more.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      427 2024-05-05 19:35:28.000000 django_nets_core-0.1.85/nets_core/migrations/0011_role_enabled.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.85/nets_core/migrations/__init__.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)    14160 2024-05-07 17:09:07.000000 django_nets_core-0.1.85/nets_core/models.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6425 2024-05-04 23:43:26.000000 django_nets_core-0.1.85/nets_core/params.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:30:32.056189 django_nets_core-0.1.85/nets_core/procedures/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:30:32.056189 django_nets_core-0.1.85/nets_core/procedures/__pycache__/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1511 2024-05-07 16:19:56.000000 django_nets_core-0.1.85/nets_core/procedures/__pycache__/create_nets_core_functions.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1607 2024-05-07 17:30:24.000000 django_nets_core-0.1.85/nets_core/procedures/__pycache__/nets_core_functions.cpython-312.pyc
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:30:32.056189 django_nets_core-0.1.85/nets_core/procedures/functions/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2266 2024-05-07 17:24:45.000000 django_nets_core-0.1.85/nets_core/procedures/functions/nets_core_postgre_model_to_json.sql
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1214 2024-05-07 17:30:22.000000 django_nets_core-0.1.85/nets_core/procedures/nets_core_functions.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      902 2024-05-04 23:43:26.000000 django_nets_core-0.1.85/nets_core/responses.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3055 2024-05-04 23:43:26.000000 django_nets_core-0.1.85/nets_core/security.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2490 2024-05-07 17:24:57.000000 django_nets_core-0.1.85/nets_core/serializers.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3387 2024-05-05 18:22:43.000000 django_nets_core-0.1.85/nets_core/settings.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1820 2024-05-05 05:05:51.000000 django_nets_core-0.1.85/nets_core/settings_nets.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      753 2024-05-05 05:16:02.000000 django_nets_core-0.1.85/nets_core/tasks.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:30:32.052189 django_nets_core-0.1.85/nets_core/templates/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:30:32.056189 django_nets_core-0.1.85/nets_core/templates/nets_core/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6978 2024-05-04 23:43:26.000000 django_nets_core-0.1.85/nets_core/templates/nets_core/base.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1954 2024-05-04 23:43:26.000000 django_nets_core-0.1.85/nets_core/templates/nets_core/delete_account.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-05 18:03:29.000000 django_nets_core-0.1.85/nets_core/templates/nets_core/delete_account_info.html
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 17:30:32.056189 django_nets_core-0.1.85/nets_core/templates/nets_core/email/
+-rw-rw-r--   0 dev       (1001) dev       (1001)    16103 2024-05-04 23:43:26.000000 django_nets_core-0.1.85/nets_core/templates/nets_core/email/base_email.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1032 2024-05-04 23:43:26.000000 django_nets_core-0.1.85/nets_core/templates/nets_core/email/new_login.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)      316 2024-05-04 23:43:26.000000 django_nets_core-0.1.85/nets_core/templates/nets_core/email/verification_code.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)      824 2024-05-04 23:43:26.000000 django_nets_core-0.1.85/nets_core/urls.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3003 2024-05-05 18:49:07.000000 django_nets_core-0.1.85/nets_core/utils.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)    11727 2024-05-05 18:04:42.000000 django_nets_core-0.1.85/nets_core/views.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      395 2024-05-04 23:43:26.000000 django_nets_core-0.1.85/nets_core/wsgi.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      100 2024-05-05 00:47:40.000000 django_nets_core-0.1.85/pyproject.toml
+-rw-rw-r--   0 dev       (1001) dev       (1001)      181 2024-05-05 01:49:02.000000 django_nets_core-0.1.85/requirements.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1334 2024-05-07 17:30:32.060189 django_nets_core-0.1.85/setup.cfg
+-rw-rw-r--   0 dev       (1001) dev       (1001)       38 2024-05-04 23:43:26.000000 django_nets_core-0.1.85/setup.py
```

### Comparing `django_nets_core-0.1.84/PKG-INFO` & `django_nets_core-0.1.85/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-nets-core
-Version: 0.1.84
+Version: 0.1.85
 Summary: A lazy API rest request handler.
 Home-page: https://github.com/esbozos/django-nets-core
 Author: Norman Torres
 Author-email: norman.nets@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_nets_core-0.1.84/README.rst` & `django_nets_core-0.1.85/README.rst`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/django_nets_core.egg-info/PKG-INFO` & `django_nets_core-0.1.85/django_nets_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-nets-core
-Version: 0.1.84
+Version: 0.1.85
 Summary: A lazy API rest request handler.
 Home-page: https://github.com/esbozos/django-nets-core
 Author: Norman Torres
 Author-email: norman.nets@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_nets_core-0.1.84/django_nets_core.egg-info/SOURCES.txt` & `django_nets_core-0.1.85/django_nets_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/admin.py` & `django_nets_core-0.1.85/nets_core/admin.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/apps.py` & `django_nets_core-0.1.85/nets_core/apps.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/asgi.py` & `django_nets_core-0.1.85/nets_core/asgi.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/auth_urls.py` & `django_nets_core-0.1.85/nets_core/auth_urls.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/decorators.py` & `django_nets_core-0.1.85/nets_core/decorators.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/firebase_messages.py` & `django_nets_core-0.1.85/nets_core/firebase_messages.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/handlers.py` & `django_nets_core-0.1.85/nets_core/handlers.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/listeners.py` & `django_nets_core-0.1.85/nets_core/listeners.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/mail.py` & `django_nets_core-0.1.85/nets_core/mail.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/manage.py` & `django_nets_core-0.1.85/nets_core/manage.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc` & `django_nets_core-0.1.85/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/management/commands/nets-settings.py` & `django_nets_core-0.1.85/nets_core/management/commands/nets-settings.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc` & `django_nets_core-0.1.85/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/middleware/auth_token.py` & `django_nets_core-0.1.85/nets_core/middleware/auth_token.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/migrations/0001_initial.py` & `django_nets_core-0.1.85/nets_core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/migrations/0003_userdevice.py` & `django_nets_core-0.1.85/nets_core/migrations/0003_userdevice.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/migrations/0007_alter_verificationcode_device.py` & `django_nets_core-0.1.85/nets_core/migrations/0007_alter_verificationcode_device.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py` & `django_nets_core-0.1.85/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/migrations/0010_permission_role_userrole_and_more.py` & `django_nets_core-0.1.85/nets_core/migrations/0010_permission_role_userrole_and_more.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/models.py` & `django_nets_core-0.1.85/nets_core/models.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/params.py` & `django_nets_core-0.1.85/nets_core/params.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/procedures/__pycache__/create_nets_core_functions.cpython-312.pyc` & `django_nets_core-0.1.85/nets_core/procedures/__pycache__/create_nets_core_functions.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/procedures/__pycache__/nets_core_functions.cpython-312.pyc` & `django_nets_core-0.1.85/nets_core/procedures/__pycache__/nets_core_functions.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Tue May  7 16:16:05 2024 UTC, .py size: 1142 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 18% similar despite different names*

```diff
@@ -1,94 +1,101 @@
-00000000: cb0d 0d0a 0000 0000 c553 3a66 7604 0000  .........S:fv...
+00000000: cb0d 0d0a 0000 0000 2e65 3a66 be04 0000  .........e:f....
 00000010: e300 0000 0000 0000 0000 0000 0003 0000  ................
 00000020: 0000 0000 00f3 3200 0000 9700 6400 6401  ......2.....d.d.
 00000030: 6c00 5a00 6400 6402 6c01 6d02 5a02 0100  l.Z.d.d.l.m.Z...
 00000040: 6400 6403 6c03 6d04 5a04 0100 6406 6404  d.d.l.m.Z...d.d.
 00000050: 6505 6602 6405 8405 5a06 7901 2907 e900  e.f.d...Z.y.)...
 00000060: 0000 004e 2901 da04 5061 7468 2901 da0b  ...N)...Path)...
 00000070: 636f 6e6e 6563 7469 6f6e 73da 0575 7369  connections..usi
 00000080: 6e67 6301 0000 0000 0000 0000 0000 0007  ngc.............
-00000090: 0000 0003 0000 00f3 1602 0000 9700 6401  ..............d.
+00000090: 0000 0003 0000 00f3 5802 0000 9700 6401  ........X.....d.
 000000a0: 6400 6c00 7d01 7c01 6a03 0000 0000 0000  d.l.}.|.j.......
 000000b0: 0000 0000 0000 0000 0000 0000 7404 0000  ............t...
 000000c0: 0000 0000 0000 ab01 0000 0000 0000 7d02  ..............}.
-000000d0: 7c02 6a07 0000 0000 0000 0000 0000 0000  |.j.............
-000000e0: 0000 0000 0000 6402 7c00 9b00 6403 9d03  ......d.|...d...
-000000f0: ab01 0000 0000 0000 0100 7408 0000 0000  ..........t.....
-00000100: 0000 0000 7c00 1900 0000 7d03 7c03 6a0a  ....|.....}.|.j.
-00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000120: 0000 7d04 740d 0000 0000 0000 0000 740e  ..}.t.........t.
-00000130: 0000 0000 0000 0000 ab01 0000 0000 0000  ................
-00000140: 6a10 0000 0000 0000 0000 0000 0000 0000  j...............
-00000150: 0000 0000 6404 7a0b 0000 7d05 7c05 6a13  ....d.z...}.|.j.
-00000160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000170: 0000 ab00 0000 0000 0000 4400 5d7b 0000  ..........D.]{..
-00000180: 7d06 7c06 6a15 0000 0000 0000 0000 0000  }.|.j...........
-00000190: 0000 0000 0000 0000 ab00 0000 0000 0000  ................
-000001a0: 7301 8c14 6405 7c04 9b00 9d02 7c06 6a16  s...d.|.....|.j.
-000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001c0: 0000 7600 7301 8c26 7c02 6a07 0000 0000  ..v.s..&|.j.....
-000001d0: 0000 0000 0000 0000 0000 0000 0000 6406  ..............d.
-000001e0: 7c06 9b00 9d02 ab01 0000 0000 0000 0100  |...............
-000001f0: 7419 0000 0000 0000 0000 7c06 6407 ab02  t.........|.d...
-00000200: 0000 0000 0000 3500 7d07 7c03 6a1b 0000  ......5.}.|.j...
-00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000220: ab00 0000 0000 0000 6a1d 0000 0000 0000  ........j.......
-00000230: 0000 0000 0000 0000 0000 0000 7c07 6a1f  ............|.j.
-00000240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000250: 0000 ab00 0000 0000 0000 ab01 0000 0000  ................
-00000260: 0000 0100 6400 6400 6400 ab02 0000 0000  ....d.d.d.......
-00000270: 0000 0100 8c7d 0400 7c03 6a21 0000 0000  .....}..|.j!....
-00000280: 0000 0000 0000 0000 0000 0000 0000 ab00  ................
-00000290: 0000 0000 0000 0100 7908 2300 3100 7301  ........y.#.1.s.
-000002a0: 7702 0100 5900 0100 0100 8c98 7803 5900  w...Y.......x.Y.
-000002b0: 7701 2909 4e72 0200 0000 7a21 4372 6561  w.).Nr....z!Crea
-000002c0: 7469 6e67 206e 6574 735f 636f 7265 2066  ting nets_core f
-000002d0: 756e 6374 696f 6e73 2066 6f72 207a 0920  unctions for z. 
-000002e0: 6461 7461 6261 7365 da09 6675 6e63 7469  database..functi
-000002f0: 6f6e 73da 0a6e 6574 735f 636f 7265 5f7a  ons..nets_core_z
-00000300: 1743 7265 6174 696e 6720 6675 6e63 7469  .Creating functi
-00000310: 6f6e 2066 726f 6d20 da01 7254 2911 da07  on from ..rT)...
-00000320: 6c6f 6767 696e 67da 0967 6574 4c6f 6767  logging..getLogg
-00000330: 6572 da08 5f5f 6e61 6d65 5f5f da04 696e  er..__name__..in
-00000340: 666f 7204 0000 00da 0676 656e 646f 7272  for......vendorr
-00000350: 0300 0000 da08 5f5f 6669 6c65 5f5f da06  ......__file__..
-00000360: 7061 7265 6e74 da07 6974 6572 6469 72da  parent..iterdir.
-00000370: 0769 735f 6669 6c65 da04 6e61 6d65 da04  .is_file..name..
-00000380: 6f70 656e da06 6375 7273 6f72 da07 6578  open..cursor..ex
-00000390: 6563 7574 65da 0472 6561 64da 0563 6c6f  ecute..read..clo
-000003a0: 7365 2908 7205 0000 0072 0a00 0000 da06  se).r....r......
-000003b0: 6c6f 6767 6572 da0a 636f 6e6e 6563 7469  logger..connecti
-000003c0: 6f6e da06 656e 6769 6e65 da0e 6675 6e63  on..engine..func
-000003d0: 7469 6f6e 5f66 696c 6573 da04 6669 6c65  tion_files..file
-000003e0: da01 6673 0800 0000 2020 2020 2020 2020  ..fs....        
-000003f0: fa46 2f68 6f6d 652f 6465 762f 646a 616e  .F/home/dev/djan
-00000400: 676f 2d6e 6574 732d 636f 7265 2f6e 6574  go-nets-core/net
-00000410: 735f 636f 7265 2f70 726f 6365 6475 7265  s_core/procedure
-00000420: 732f 6e65 7473 5f63 6f72 655f 6675 6e63  s/nets_core_func
-00000430: 7469 6f6e 732e 7079 da1a 6372 6561 7465  tions.py..create
-00000440: 5f6e 6574 735f 636f 7265 5f66 756e 6374  _nets_core_funct
-00000450: 696f 6e73 7220 0000 0005 0000 0073 f100  ionsr .......s..
-00000460: 0000 8000 f312 0005 13d8 0d14 d70d 1ed1  ................
-00000470: 0d1e 9c78 d30d 2880 46d8 040a 874b 814b  ...x..(.F....K.K
-00000480: d012 33b0 45b0 37b8 29d0 1044 d404 45e4  ..3.E.7.)..D..E.
-00000490: 111c 9855 d111 2380 4ad8 0d17 d70d 1ed1  ...U..#.J.......
-000004a0: 0d1e 8046 dc15 199c 2893 5ed7 152a d115  ...F....(.^..*..
-000004b0: 2aa8 5bd1 1538 804e d810 1ed7 1026 d110  *.[..8.N.....&..
-000004c0: 26d3 1028 f200 0505 3a88 04d8 0b0f 8f3c  &..(....:......<
-000004d0: 893c 8d3e d811 1b98 4698 38d0 0f24 a804  .<.>....F.8..$..
-000004e0: af09 a909 d20f 31d8 1016 970b 910b d01e  ......1.........
-000004f0: 35b0 64b0 56d0 1c3c d410 3ddc 1519 9824  5.d.V..<..=....$
-00000500: a003 935f f000 0111 3aa8 01d8 141e d714  ..._....:.......
-00000510: 25d1 1425 d314 27d7 142f d114 2fb0 01b7  %..%..'../../...
-00000520: 06b1 06b3 08d4 1439 f703 0111 3af0 0001  .......9....:...
-00000530: 113a f009 0505 3af0 0c00 050f d704 14d1  .:....:.........
-00000540: 0414 d404 16d8 0b0f f707 0111 3af0 0001  ............:...
-00000550: 113a fa73 0c00 0000 c236 2e43 3f05 c33f  .:.s.....6.C?..?
-00000560: 0544 0809 2901 da07 6465 6661 756c 7429  .D..)...default)
-00000570: 07da 026f 73da 0770 6174 686c 6962 7203  ...os..pathlibr.
-00000580: 0000 00da 0964 6a61 6e67 6f2e 6462 7204  .....django.dbr.
-00000590: 0000 00da 0373 7472 7220 0000 00a9 00f3  .....strr ......
-000005a0: 0000 0000 721f 0000 00fa 083c 6d6f 6475  ....r......<modu
-000005b0: 6c65 3e72 2800 0000 0100 0000 731a 0000  le>r(.......s...
-000005c0: 00f0 0301 0101 db00 09dd 0018 dd00 21f1  ..............!.
-000005d0: 0417 0110 a063 f400 1701 1072 2700 0000  .....c.....r'...
+000000d0: 7406 0000 0000 0000 0000 7c00 1900 0000  t.........|.....
+000000e0: 7d03 7c03 6a08 0000 0000 0000 0000 0000  }.|.j...........
+000000f0: 0000 0000 0000 0000 7d04 7c02 6a0b 0000  ........}.|.j...
+00000100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000110: 6402 7c00 9b00 6403 7c04 9b00 9d04 ab01  d.|...d.|.......
+00000120: 0000 0000 0000 0100 740d 0000 0000 0000  ........t.......
+00000130: 0000 740e 0000 0000 0000 0000 ab01 0000  ..t.............
+00000140: 0000 0000 6a10 0000 0000 0000 0000 0000  ....j...........
+00000150: 0000 0000 0000 0000 6404 7a0b 0000 7d05  ........d.z...}.
+00000160: 7c05 6a13 0000 0000 0000 0000 0000 0000  |.j.............
+00000170: 0000 0000 0000 ab00 0000 0000 0000 4400  ..............D.
+00000180: 5d9a 0000 7d06 7c06 6a15 0000 0000 0000  ]...}.|.j.......
+00000190: 0000 0000 0000 0000 0000 0000 ab00 0000  ................
+000001a0: 0000 0000 7301 8c14 6405 7c04 9b00 9d02  ....s...d.|.....
+000001b0: 7c06 6a16 0000 0000 0000 0000 0000 0000  |.j.............
+000001c0: 0000 0000 0000 7600 7301 8c26 7c02 6a0b  ......v.s..&|.j.
+000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000001e0: 0000 6406 7c06 9b00 9d02 ab01 0000 0000  ..d.|...........
+000001f0: 0000 0100 7419 0000 0000 0000 0000 7c06  ....t.........|.
+00000200: 6407 ab02 0000 0000 0000 3500 7d07 7c02  d.........5.}.|.
+00000210: 6a0b 0000 0000 0000 0000 0000 0000 0000  j...............
+00000220: 0000 0000 7c07 6a1b 0000 0000 0000 0000  ....|.j.........
+00000230: 0000 0000 0000 0000 0000 ab00 0000 0000  ................
+00000240: 0000 ab01 0000 0000 0000 0100 7c03 6a1d  ............|.j.
+00000250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000260: 0000 ab00 0000 0000 0000 6a1f 0000 0000  ..........j.....
+00000270: 0000 0000 0000 0000 0000 0000 0000 7c07  ..............|.
+00000280: 6a1b 0000 0000 0000 0000 0000 0000 0000  j...............
+00000290: 0000 0000 ab00 0000 0000 0000 ab01 0000  ................
+000002a0: 0000 0000 0100 6400 6400 6400 ab02 0000  ......d.d.d.....
+000002b0: 0000 0000 0100 8c9c 0400 7c03 6a21 0000  ..........|.j!..
+000002c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002d0: ab00 0000 0000 0000 0100 7908 2300 3100  ..........y.#.1.
+000002e0: 7301 7702 0100 5900 0100 0100 8cb7 7803  s.w...Y.......x.
+000002f0: 5900 7701 2909 4e72 0200 0000 7a21 4372  Y.w.).Nr....z!Cr
+00000300: 6561 7469 6e67 206e 6574 735f 636f 7265  eating nets_core
+00000310: 2066 756e 6374 696f 6e73 2066 6f72 207a   functions for z
+00000320: 1120 6461 7461 6261 7365 2065 6e67 696e  . database engin
+00000330: 6520 da09 6675 6e63 7469 6f6e 73da 0a6e  e ..functions..n
+00000340: 6574 735f 636f 7265 5f7a 1743 7265 6174  ets_core_z.Creat
+00000350: 696e 6720 6675 6e63 7469 6f6e 2066 726f  ing function fro
+00000360: 6d20 da01 7254 2911 da07 6c6f 6767 696e  m ..rT)...loggin
+00000370: 67da 0967 6574 4c6f 6767 6572 da08 5f5f  g..getLogger..__
+00000380: 6e61 6d65 5f5f 7204 0000 00da 0676 656e  name__r......ven
+00000390: 646f 72da 0777 6172 6e69 6e67 7203 0000  dor..warningr...
+000003a0: 00da 085f 5f66 696c 655f 5fda 0670 6172  ...__file__..par
+000003b0: 656e 74da 0769 7465 7264 6972 da07 6973  ent..iterdir..is
+000003c0: 5f66 696c 65da 046e 616d 65da 046f 7065  _file..name..ope
+000003d0: 6eda 0472 6561 64da 0663 7572 736f 72da  n..read..cursor.
+000003e0: 0765 7865 6375 7465 da05 636c 6f73 6529  .execute..close)
+000003f0: 0872 0500 0000 720a 0000 00da 066c 6f67  .r....r......log
+00000400: 6765 72da 0a63 6f6e 6e65 6374 696f 6eda  ger..connection.
+00000410: 0665 6e67 696e 65da 0e66 756e 6374 696f  .engine..functio
+00000420: 6e5f 6669 6c65 73da 0466 696c 65da 0166  n_files..file..f
+00000430: 7308 0000 0020 2020 2020 2020 20fa 462f  s....        .F/
+00000440: 686f 6d65 2f64 6576 2f64 6a61 6e67 6f2d  home/dev/django-
+00000450: 6e65 7473 2d63 6f72 652f 6e65 7473 5f63  nets-core/nets_c
+00000460: 6f72 652f 7072 6f63 6564 7572 6573 2f6e  ore/procedures/n
+00000470: 6574 735f 636f 7265 5f66 756e 6374 696f  ets_core_functio
+00000480: 6e73 2e70 79da 1a63 7265 6174 655f 6e65  ns.py..create_ne
+00000490: 7473 5f63 6f72 655f 6675 6e63 7469 6f6e  ts_core_function
+000004a0: 7372 2000 0000 0500 0000 730a 0100 0080  sr .......s.....
+000004b0: 00f3 1200 0513 d80d 14d7 0d1e d10d 1e9c  ................
+000004c0: 78d3 0d28 8046 f406 0012 1d98 55d1 1123  x..(.F......U..#
+000004d0: 804a d80d 17d7 0d1e d10d 1e80 46d8 040a  .J..........F...
+000004e0: 874e 814e d015 36b0 75b0 67d0 3d4e c876  .N.N..6.u.g.=N.v
+000004f0: c868 d013 57d4 0458 dc15 199c 2893 5ed7  .h..W..X....(.^.
+00000500: 152a d115 2aa8 5bd1 1538 804e d810 1ed7  .*..*.[..8.N....
+00000510: 1026 d110 26d3 1028 f200 0605 3a88 04d8  .&..&..(....:...
+00000520: 0b0f 8f3c 893c 8d3e d811 1b98 4698 38d0  ...<.<.>....F.8.
+00000530: 0f24 a804 af09 a909 d20f 31d8 1016 970e  .$........1.....
+00000540: 910e d021 38b8 14b8 06d0 1f3f d410 40dc  ...!8......?..@.
+00000550: 1519 9824 a003 935f f000 0211 3aa8 01d8  ...$..._....:...
+00000560: 141a 974e 914e a031 a736 a136 a338 d414  ...N.N.1.6.6.8..
+00000570: 2cd8 141e d714 25d1 1425 d314 27d7 142f  ,.....%..%..'../
+00000580: d114 2fb0 01b7 06b1 06b3 08d4 1439 f705  ../..........9..
+00000590: 0211 3af0 0002 113a f009 0605 3af0 0e00  ..:....:....:...
+000005a0: 050f d704 14d1 0414 d404 16d8 0b0f f709  ................
+000005b0: 0211 3af0 0002 113a fa73 0d00 0000 c238  ..:....:.s.....8
+000005c0: 410d 4420 05c4 2005 4429 0929 01da 0764  A.D .. .D).)...d
+000005d0: 6566 6175 6c74 2907 da02 6f73 da07 7061  efault)...os..pa
+000005e0: 7468 6c69 6272 0300 0000 da09 646a 616e  thlibr......djan
+000005f0: 676f 2e64 6272 0400 0000 da03 7374 7272  go.dbr......strr
+00000600: 2000 0000 a900 f300 0000 0072 1f00 0000   ..........r....
+00000610: fa08 3c6d 6f64 756c 653e 7228 0000 0001  ..<module>r(....
+00000620: 0000 0073 1a00 0000 f003 0101 01db 0009  ...s............
+00000630: dd00 18dd 0021 f104 1901 10a0 63f4 0019  .....!......c...
+00000640: 0110 7227 0000 00                        ..r'...
```

### Comparing `django_nets_core-0.1.84/nets_core/procedures/functions/nets_core_postgre_model_to_json.sql` & `django_nets_core-0.1.85/nets_core/procedures/functions/nets_core_postgre_model_to_json.sql`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/procedures/nets_core_functions.py` & `django_nets_core-0.1.85/nets_core/procedures/nets_core_functions.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,22 +9,24 @@
     # Example: nets_core_postgresql_model_to_json.sql will create a function to convert a model to json in postgresql
     # we need to check db engine and create the function accordingly
     
     # use stdout to print the sql query
     
     import logging
     logger = logging.getLogger(__name__)
-    logger.info(f"Creating nets_core functions for {using} database")
+    
     
     connection = connections[using]
     engine = connection.vendor
+    logger.warning(f"Creating nets_core functions for {using} database engine {engine}")
     function_files = Path(__file__).parent / "functions"
     for file in function_files.iterdir():
         if file.is_file():
             if f"nets_core_{engine}" in file.name:
-                logger.info(f"Creating function from {file}")
+                logger.warning(f"Creating function from {file}")
                 with open(file, "r") as f:
+                    logger.warning(f.read())
                     connection.cursor().execute(f.read())
     connection.close()
     return True
```

### Comparing `django_nets_core-0.1.84/nets_core/responses.py` & `django_nets_core-0.1.85/nets_core/responses.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/security.py` & `django_nets_core-0.1.85/nets_core/security.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/serializers.py` & `django_nets_core-0.1.85/nets_core/serializers.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/settings.py` & `django_nets_core-0.1.85/nets_core/settings.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/settings_nets.py` & `django_nets_core-0.1.85/nets_core/settings_nets.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/tasks.py` & `django_nets_core-0.1.85/nets_core/tasks.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/templates/nets_core/base.html` & `django_nets_core-0.1.85/nets_core/templates/nets_core/base.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/templates/nets_core/delete_account.html` & `django_nets_core-0.1.85/nets_core/templates/nets_core/delete_account.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/templates/nets_core/email/base_email.html` & `django_nets_core-0.1.85/nets_core/templates/nets_core/email/base_email.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/templates/nets_core/email/new_login.html` & `django_nets_core-0.1.85/nets_core/templates/nets_core/email/new_login.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/urls.py` & `django_nets_core-0.1.85/nets_core/urls.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/utils.py` & `django_nets_core-0.1.85/nets_core/utils.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/nets_core/views.py` & `django_nets_core-0.1.85/nets_core/views.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.84/setup.cfg` & `django_nets_core-0.1.85/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-nets-core
-version = 0.1.84
+version = 0.1.85
 description = A lazy API rest request handler.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/esbozos/django-nets-core
 author = Norman Torres
 author_email = norman.nets@gmail.com
 license = BSD-3-Clause
```

