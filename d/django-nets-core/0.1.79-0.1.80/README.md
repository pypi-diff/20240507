# Comparing `tmp/django_nets_core-0.1.79.tar.gz` & `tmp/django_nets_core-0.1.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_nets_core-0.1.79.tar", last modified: Sun May  5 20:00:59 2024, max compression
+gzip compressed data, was "django_nets_core-0.1.80.tar", last modified: Tue May  7 16:48:41 2024, max compression
```

## Comparing `django_nets_core-0.1.79.tar` & `django_nets_core-0.1.80.tar`

### file list

```diff
@@ -1,72 +1,80 @@
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 20:00:59.571034 django_nets_core-0.1.79/
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/LICENSE
--rw-rw-r--   0 dev       (1001) dev       (1001)      304 2024-05-05 15:47:07.000000 django_nets_core-0.1.79/MANIFEST.in
--rw-r--r--   0 dev       (1001) dev       (1001)    13678 2024-05-05 20:00:59.571034 django_nets_core-0.1.79/PKG-INFO
--rw-rw-r--   0 dev       (1001) dev       (1001)    12153 2024-05-05 18:59:42.000000 django_nets_core-0.1.79/README.rst
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 20:00:59.571034 django_nets_core-0.1.79/django_nets_core.egg-info/
--rw-r--r--   0 dev       (1001) dev       (1001)    13678 2024-05-05 20:00:59.000000 django_nets_core-0.1.79/django_nets_core.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1001) dev       (1001)     2015 2024-05-05 20:00:59.000000 django_nets_core-0.1.79/django_nets_core.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)        1 2024-05-05 20:00:59.000000 django_nets_core-0.1.79/django_nets_core.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)      286 2024-05-05 20:00:59.000000 django_nets_core-0.1.79/django_nets_core.egg-info/requires.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)       10 2024-05-05 20:00:59.000000 django_nets_core-0.1.79/django_nets_core.egg-info/top_level.txt
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 20:00:59.571034 django_nets_core-0.1.79/nets_core/
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/nets_core/__init__.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2440 2024-05-05 19:35:20.000000 django_nets_core-0.1.79/nets_core/admin.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      206 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/nets_core/apps.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      807 2024-05-05 05:05:51.000000 django_nets_core-0.1.79/nets_core/asgi.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      537 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/nets_core/auth_urls.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      229 2024-05-05 05:05:51.000000 django_nets_core-0.1.79/nets_core/celery.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     4901 2024-05-05 18:50:21.000000 django_nets_core-0.1.79/nets_core/decorators.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3276 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/nets_core/firebase_messages.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     6465 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/nets_core/handlers.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2477 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/nets_core/listeners.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     4460 2024-05-05 18:01:33.000000 django_nets_core-0.1.79/nets_core/mail.py
--rwxrwxr-x   0 dev       (1001) dev       (1001)      665 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/nets_core/manage.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 20:00:59.563033 django_nets_core-0.1.79/nets_core/management/
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 20:00:59.571034 django_nets_core-0.1.79/nets_core/management/commands/
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-05 02:03:24.000000 django_nets_core-0.1.79/nets_core/management/commands/__init__.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 20:00:59.571034 django_nets_core-0.1.79/nets_core/management/commands/__pycache__/
--rw-rw-r--   0 dev       (1001) dev       (1001)      165 2024-05-05 02:44:07.000000 django_nets_core-0.1.79/nets_core/management/commands/__pycache__/__init__.cpython-312.pyc
--rw-rw-r--   0 dev       (1001) dev       (1001)    28055 2024-05-05 05:05:51.000000 django_nets_core-0.1.79/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc
--rw-rw-r--   0 dev       (1001) dev       (1001)    22259 2024-05-05 19:59:37.000000 django_nets_core-0.1.79/nets_core/management/commands/nets-settings.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 20:00:59.571034 django_nets_core-0.1.79/nets_core/middleware/
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 20:00:59.571034 django_nets_core-0.1.79/nets_core/middleware/__pycache__/
--rw-rw-r--   0 dev       (1001) dev       (1001)     3004 2024-05-05 04:39:30.000000 django_nets_core-0.1.79/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc
--rw-rw-r--   0 dev       (1001) dev       (1001)     2113 2024-05-05 19:54:31.000000 django_nets_core-0.1.79/nets_core/middleware/auth_token.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 20:00:59.571034 django_nets_core-0.1.79/nets_core/migrations/
--rw-rw-r--   0 dev       (1001) dev       (1001)     5274 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/nets_core/migrations/0001_initial.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      422 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/nets_core/migrations/0002_alter_verificationcode_token.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2208 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/nets_core/migrations/0003_userdevice.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      360 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/nets_core/migrations/0004_remove_userdevice_device_id_userdevice_uuid.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      480 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/nets_core/migrations/0005_userdevice_uuid.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      454 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/nets_core/migrations/0006_verificationcode_device.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      533 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/nets_core/migrations/0007_alter_verificationcode_device.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2056 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      455 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/nets_core/migrations/0009_userdevice_ip.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     6844 2024-05-05 19:06:27.000000 django_nets_core-0.1.79/nets_core/migrations/0010_permission_role_userrole_and_more.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      427 2024-05-05 19:35:28.000000 django_nets_core-0.1.79/nets_core/migrations/0011_role_enabled.py
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/nets_core/migrations/__init__.py
--rw-rw-r--   0 dev       (1001) dev       (1001)    12997 2024-05-05 19:21:33.000000 django_nets_core-0.1.79/nets_core/models.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     6425 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/nets_core/params.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      902 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/nets_core/responses.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3055 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/nets_core/security.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3387 2024-05-05 18:22:43.000000 django_nets_core-0.1.79/nets_core/settings.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     1820 2024-05-05 05:05:51.000000 django_nets_core-0.1.79/nets_core/settings_nets.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      753 2024-05-05 05:16:02.000000 django_nets_core-0.1.79/nets_core/tasks.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 20:00:59.567033 django_nets_core-0.1.79/nets_core/templates/
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 20:00:59.571034 django_nets_core-0.1.79/nets_core/templates/nets_core/
--rw-rw-r--   0 dev       (1001) dev       (1001)     6978 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/nets_core/templates/nets_core/base.html
--rw-rw-r--   0 dev       (1001) dev       (1001)     1954 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/nets_core/templates/nets_core/delete_account.html
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-05 18:03:29.000000 django_nets_core-0.1.79/nets_core/templates/nets_core/delete_account_info.html
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 20:00:59.571034 django_nets_core-0.1.79/nets_core/templates/nets_core/email/
--rw-rw-r--   0 dev       (1001) dev       (1001)    16103 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/nets_core/templates/nets_core/email/base_email.html
--rw-rw-r--   0 dev       (1001) dev       (1001)     1032 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/nets_core/templates/nets_core/email/new_login.html
--rw-rw-r--   0 dev       (1001) dev       (1001)      316 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/nets_core/templates/nets_core/email/verification_code.html
--rw-rw-r--   0 dev       (1001) dev       (1001)      824 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/nets_core/urls.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3003 2024-05-05 18:49:07.000000 django_nets_core-0.1.79/nets_core/utils.py
--rw-rw-r--   0 dev       (1001) dev       (1001)    11727 2024-05-05 18:04:42.000000 django_nets_core-0.1.79/nets_core/views.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      395 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/nets_core/wsgi.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      100 2024-05-05 00:47:40.000000 django_nets_core-0.1.79/pyproject.toml
--rw-rw-r--   0 dev       (1001) dev       (1001)      181 2024-05-05 01:49:02.000000 django_nets_core-0.1.79/requirements.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)     1334 2024-05-05 20:00:59.575034 django_nets_core-0.1.79/setup.cfg
--rw-rw-r--   0 dev       (1001) dev       (1001)       38 2024-05-04 23:43:26.000000 django_nets_core-0.1.79/setup.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 16:48:41.350713 django_nets_core-0.1.80/
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.80/LICENSE
+-rw-rw-r--   0 dev       (1001) dev       (1001)      396 2024-05-07 15:50:26.000000 django_nets_core-0.1.80/MANIFEST.in
+-rw-r--r--   0 dev       (1001) dev       (1001)    13678 2024-05-07 16:48:41.350713 django_nets_core-0.1.80/PKG-INFO
+-rw-rw-r--   0 dev       (1001) dev       (1001)    12153 2024-05-05 18:59:42.000000 django_nets_core-0.1.80/README.rst
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 16:48:41.346713 django_nets_core-0.1.80/django_nets_core.egg-info/
+-rw-r--r--   0 dev       (1001) dev       (1001)    13678 2024-05-07 16:48:41.000000 django_nets_core-0.1.80/django_nets_core.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2296 2024-05-07 16:48:41.000000 django_nets_core-0.1.80/django_nets_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)        1 2024-05-07 16:48:41.000000 django_nets_core-0.1.80/django_nets_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)      286 2024-05-07 16:48:41.000000 django_nets_core-0.1.80/django_nets_core.egg-info/requires.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)       10 2024-05-07 16:48:41.000000 django_nets_core-0.1.80/django_nets_core.egg-info/top_level.txt
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 16:48:41.346713 django_nets_core-0.1.80/nets_core/
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.80/nets_core/__init__.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2440 2024-05-05 19:35:20.000000 django_nets_core-0.1.80/nets_core/admin.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      665 2024-05-07 16:47:52.000000 django_nets_core-0.1.80/nets_core/apps.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      807 2024-05-05 05:05:51.000000 django_nets_core-0.1.80/nets_core/asgi.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      537 2024-05-04 23:43:26.000000 django_nets_core-0.1.80/nets_core/auth_urls.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      229 2024-05-05 05:05:51.000000 django_nets_core-0.1.80/nets_core/celery.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     4901 2024-05-05 18:50:21.000000 django_nets_core-0.1.80/nets_core/decorators.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3276 2024-05-04 23:43:26.000000 django_nets_core-0.1.80/nets_core/firebase_messages.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6465 2024-05-04 23:43:26.000000 django_nets_core-0.1.80/nets_core/handlers.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2502 2024-05-07 16:19:36.000000 django_nets_core-0.1.80/nets_core/listeners.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     4460 2024-05-05 18:01:33.000000 django_nets_core-0.1.80/nets_core/mail.py
+-rwxrwxr-x   0 dev       (1001) dev       (1001)      665 2024-05-04 23:43:26.000000 django_nets_core-0.1.80/nets_core/manage.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 16:48:41.342713 django_nets_core-0.1.80/nets_core/management/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 16:48:41.346713 django_nets_core-0.1.80/nets_core/management/commands/
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-05 02:03:24.000000 django_nets_core-0.1.80/nets_core/management/commands/__init__.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 16:48:41.346713 django_nets_core-0.1.80/nets_core/management/commands/__pycache__/
+-rw-rw-r--   0 dev       (1001) dev       (1001)      165 2024-05-05 02:44:07.000000 django_nets_core-0.1.80/nets_core/management/commands/__pycache__/__init__.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)    28055 2024-05-05 05:05:51.000000 django_nets_core-0.1.80/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)    22259 2024-05-05 19:59:37.000000 django_nets_core-0.1.80/nets_core/management/commands/nets-settings.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 16:48:41.346713 django_nets_core-0.1.80/nets_core/middleware/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 16:48:41.346713 django_nets_core-0.1.80/nets_core/middleware/__pycache__/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3004 2024-05-05 04:39:30.000000 django_nets_core-0.1.80/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2113 2024-05-05 19:54:31.000000 django_nets_core-0.1.80/nets_core/middleware/auth_token.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 16:48:41.346713 django_nets_core-0.1.80/nets_core/migrations/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     5274 2024-05-04 23:43:26.000000 django_nets_core-0.1.80/nets_core/migrations/0001_initial.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      422 2024-05-04 23:43:26.000000 django_nets_core-0.1.80/nets_core/migrations/0002_alter_verificationcode_token.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2208 2024-05-04 23:43:26.000000 django_nets_core-0.1.80/nets_core/migrations/0003_userdevice.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      360 2024-05-04 23:43:26.000000 django_nets_core-0.1.80/nets_core/migrations/0004_remove_userdevice_device_id_userdevice_uuid.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      480 2024-05-04 23:43:26.000000 django_nets_core-0.1.80/nets_core/migrations/0005_userdevice_uuid.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      454 2024-05-04 23:43:26.000000 django_nets_core-0.1.80/nets_core/migrations/0006_verificationcode_device.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      533 2024-05-04 23:43:26.000000 django_nets_core-0.1.80/nets_core/migrations/0007_alter_verificationcode_device.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2056 2024-05-04 23:43:26.000000 django_nets_core-0.1.80/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      455 2024-05-04 23:43:26.000000 django_nets_core-0.1.80/nets_core/migrations/0009_userdevice_ip.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6844 2024-05-05 19:06:27.000000 django_nets_core-0.1.80/nets_core/migrations/0010_permission_role_userrole_and_more.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      427 2024-05-05 19:35:28.000000 django_nets_core-0.1.80/nets_core/migrations/0011_role_enabled.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.80/nets_core/migrations/__init__.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)    14019 2024-05-07 16:46:15.000000 django_nets_core-0.1.80/nets_core/models.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6425 2024-05-04 23:43:26.000000 django_nets_core-0.1.80/nets_core/params.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 16:48:41.346713 django_nets_core-0.1.80/nets_core/procedures/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 16:48:41.346713 django_nets_core-0.1.80/nets_core/procedures/__pycache__/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1511 2024-05-07 16:19:56.000000 django_nets_core-0.1.80/nets_core/procedures/__pycache__/create_nets_core_functions.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1504 2024-05-07 16:20:53.000000 django_nets_core-0.1.80/nets_core/procedures/__pycache__/nets_core_functions.cpython-312.pyc
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 16:48:41.346713 django_nets_core-0.1.80/nets_core/procedures/functions/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1494 2024-05-07 15:45:43.000000 django_nets_core-0.1.80/nets_core/procedures/functions/nets_core_postgre_model_to_json.sql
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1142 2024-05-07 16:16:05.000000 django_nets_core-0.1.80/nets_core/procedures/nets_core_functions.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      902 2024-05-04 23:43:26.000000 django_nets_core-0.1.80/nets_core/responses.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3055 2024-05-04 23:43:26.000000 django_nets_core-0.1.80/nets_core/security.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1233 2024-05-07 16:00:57.000000 django_nets_core-0.1.80/nets_core/serializers.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3387 2024-05-05 18:22:43.000000 django_nets_core-0.1.80/nets_core/settings.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1820 2024-05-05 05:05:51.000000 django_nets_core-0.1.80/nets_core/settings_nets.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      753 2024-05-05 05:16:02.000000 django_nets_core-0.1.80/nets_core/tasks.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 16:48:41.342713 django_nets_core-0.1.80/nets_core/templates/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 16:48:41.346713 django_nets_core-0.1.80/nets_core/templates/nets_core/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6978 2024-05-04 23:43:26.000000 django_nets_core-0.1.80/nets_core/templates/nets_core/base.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1954 2024-05-04 23:43:26.000000 django_nets_core-0.1.80/nets_core/templates/nets_core/delete_account.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-05 18:03:29.000000 django_nets_core-0.1.80/nets_core/templates/nets_core/delete_account_info.html
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 16:48:41.346713 django_nets_core-0.1.80/nets_core/templates/nets_core/email/
+-rw-rw-r--   0 dev       (1001) dev       (1001)    16103 2024-05-04 23:43:26.000000 django_nets_core-0.1.80/nets_core/templates/nets_core/email/base_email.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1032 2024-05-04 23:43:26.000000 django_nets_core-0.1.80/nets_core/templates/nets_core/email/new_login.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)      316 2024-05-04 23:43:26.000000 django_nets_core-0.1.80/nets_core/templates/nets_core/email/verification_code.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)      824 2024-05-04 23:43:26.000000 django_nets_core-0.1.80/nets_core/urls.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3003 2024-05-05 18:49:07.000000 django_nets_core-0.1.80/nets_core/utils.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)    11727 2024-05-05 18:04:42.000000 django_nets_core-0.1.80/nets_core/views.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      395 2024-05-04 23:43:26.000000 django_nets_core-0.1.80/nets_core/wsgi.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      100 2024-05-05 00:47:40.000000 django_nets_core-0.1.80/pyproject.toml
+-rw-rw-r--   0 dev       (1001) dev       (1001)      181 2024-05-05 01:49:02.000000 django_nets_core-0.1.80/requirements.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1334 2024-05-07 16:48:41.350713 django_nets_core-0.1.80/setup.cfg
+-rw-rw-r--   0 dev       (1001) dev       (1001)       38 2024-05-04 23:43:26.000000 django_nets_core-0.1.80/setup.py
```

### Comparing `django_nets_core-0.1.79/PKG-INFO` & `django_nets_core-0.1.80/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-nets-core
-Version: 0.1.79
+Version: 0.1.80
 Summary: A lazy API rest request handler.
 Home-page: https://github.com/esbozos/django-nets-core
 Author: Norman Torres
 Author-email: norman.nets@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_nets_core-0.1.79/README.rst` & `django_nets_core-0.1.80/README.rst`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/django_nets_core.egg-info/PKG-INFO` & `django_nets_core-0.1.80/django_nets_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-nets-core
-Version: 0.1.79
+Version: 0.1.80
 Summary: A lazy API rest request handler.
 Home-page: https://github.com/esbozos/django-nets-core
 Author: Norman Torres
 Author-email: norman.nets@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_nets_core-0.1.79/django_nets_core.egg-info/SOURCES.txt` & `django_nets_core-0.1.80/django_nets_core.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 nets_core/listeners.py
 nets_core/mail.py
 nets_core/manage.py
 nets_core/models.py
 nets_core/params.py
 nets_core/responses.py
 nets_core/security.py
+nets_core/serializers.py
 nets_core/settings.py
 nets_core/settings_nets.py
 nets_core/tasks.py
 nets_core/urls.py
 nets_core/utils.py
 nets_core/views.py
 nets_core/wsgi.py
@@ -47,13 +48,17 @@
 nets_core/migrations/0006_verificationcode_device.py
 nets_core/migrations/0007_alter_verificationcode_device.py
 nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py
 nets_core/migrations/0009_userdevice_ip.py
 nets_core/migrations/0010_permission_role_userrole_and_more.py
 nets_core/migrations/0011_role_enabled.py
 nets_core/migrations/__init__.py
+nets_core/procedures/nets_core_functions.py
+nets_core/procedures/__pycache__/create_nets_core_functions.cpython-312.pyc
+nets_core/procedures/__pycache__/nets_core_functions.cpython-312.pyc
+nets_core/procedures/functions/nets_core_postgre_model_to_json.sql
 nets_core/templates/nets_core/base.html
 nets_core/templates/nets_core/delete_account.html
 nets_core/templates/nets_core/delete_account_info.html
 nets_core/templates/nets_core/email/base_email.html
 nets_core/templates/nets_core/email/new_login.html
 nets_core/templates/nets_core/email/verification_code.html
```

### Comparing `django_nets_core-0.1.79/nets_core/admin.py` & `django_nets_core-0.1.80/nets_core/admin.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/asgi.py` & `django_nets_core-0.1.80/nets_core/asgi.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/auth_urls.py` & `django_nets_core-0.1.80/nets_core/auth_urls.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/decorators.py` & `django_nets_core-0.1.80/nets_core/decorators.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/firebase_messages.py` & `django_nets_core-0.1.80/nets_core/firebase_messages.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/handlers.py` & `django_nets_core-0.1.80/nets_core/handlers.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/listeners.py` & `django_nets_core-0.1.80/nets_core/listeners.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from nets_core.firebase_messages import send_user_device_notification
 from nets_core.models import VerificationCode
-from django.db.models.signals import post_delete, post_save, pre_delete
+from django.db.models.signals import post_delete, post_save, pre_delete, post_migrate, post_init
 from django.dispatch import receiver
 from nets_core.mail import send_email
 from nets_core.models import EmailTemplate
 from django.core.cache import cache
 from django.utils.translation import gettext_lazy as _
 import logging
```

### Comparing `django_nets_core-0.1.79/nets_core/mail.py` & `django_nets_core-0.1.80/nets_core/mail.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/manage.py` & `django_nets_core-0.1.80/nets_core/manage.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc` & `django_nets_core-0.1.80/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/management/commands/nets-settings.py` & `django_nets_core-0.1.80/nets_core/management/commands/nets-settings.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc` & `django_nets_core-0.1.80/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/middleware/auth_token.py` & `django_nets_core-0.1.80/nets_core/middleware/auth_token.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/migrations/0001_initial.py` & `django_nets_core-0.1.80/nets_core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/migrations/0003_userdevice.py` & `django_nets_core-0.1.80/nets_core/migrations/0003_userdevice.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/migrations/0007_alter_verificationcode_device.py` & `django_nets_core-0.1.80/nets_core/migrations/0007_alter_verificationcode_device.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py` & `django_nets_core-0.1.80/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/migrations/0010_permission_role_userrole_and_more.py` & `django_nets_core-0.1.80/nets_core/migrations/0010_permission_role_userrole_and_more.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/models.py` & `django_nets_core-0.1.80/nets_core/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,29 +24,60 @@
 token_timeout_seconds = 15*60 # 15 minutes default
 try:
     token_timeout_seconds = settings.NETS_CORE_VERIFICATION_CODE_EXPIRE_SECONDS
 except Exception as e:
     # Settings not present use default
     pass
 
+class NetsCoreBaseManager(models.Manager):
+    
+    def to_json(self, fields: tuple = None):
+        if not fields:
+            raise ValueError(_("Fields must be provided"))
+        if fields == '__all__':
+            # get fiels to tupple
+            fields = tuple([field.name for field in self.model._meta.fields])
+        
+        if not isinstance(fields, tuple):
+            raise ValueError(_("Fields must be a tuple"))
+        
+        from nets_core.serializers import NetsCoreModelToJson
+        return NetsCoreModelToJson(self, fields).to_json()
+    
+    class Meta:
+        abstract = True
+
+class NetsCoreBaseModel(models.Model):
+    created = models.DateTimeField(_('Created'), auto_now_add=True)
+    updated = models.DateTimeField(_('updated'), auto_now=True)
+    
+    objects = NetsCoreBaseManager()
+
+    class Meta:
+        abstract = True
+
 class OwnedModel(models.Model):
     user = models.ForeignKey(User, on_delete=models.CASCADE)
     created = models.DateTimeField(_('Created'), auto_now_add=True)
     updated = models.DateTimeField(_('updated'), auto_now=True)
+    
+    objects = NetsCoreBaseManager()
 
     class Meta:
         abstract = True
 
 class Permission(models.Model):
     name = models.CharField(_("Name"), max_length=150)
     codename = models.CharField(_("Codename"), max_length=150)
     description = models.CharField(_("Description"), max_length=250, null=True, blank=True)
     project_content_type = models.ForeignKey(ContentType, on_delete=models.CASCADE, null=True, blank=True, related_name='nets_core_permissions')
     project_id = models.PositiveIntegerField(null=True, blank=True)
     project = GenericForeignKey('project_content_type', 'project_id')
+    
+    objects = NetsCoreBaseManager()
 
     class Meta:
         verbose_name = _("Permission")
         verbose_name_plural = _("Permissions")
         db_table = 'nets_core_permission'
         indexes = [
             models.Index(fields=['project_content_type', 'project_id'], name='permission_index')
@@ -70,14 +101,16 @@
     description = models.CharField(_("Description"), max_length=250)
     permissions = models.ManyToManyField(Permission, related_name='roles')
     project_content_type = models.ForeignKey(ContentType, on_delete=models.CASCADE, null=True, blank=True)
     project_id = models.PositiveIntegerField(null=True, blank=True)
     project = GenericForeignKey('project_content_type', 'project_id')
     enabled = models.BooleanField(_("Enabled?"), default=True)
 
+    objects = NetsCoreBaseManager()
+    
     class Meta:
         verbose_name = _("Role")
         verbose_name_plural = _("Roles")
         db_table = 'nets_core_role'
         indexes = [
             models.Index(fields=['project_content_type', 'project_id'], name='role_index')
         ]
@@ -94,14 +127,16 @@
 class UserRole(models.Model):
     user = models.ForeignKey(User, on_delete=models.CASCADE)
     role = models.ForeignKey(Role, on_delete=models.CASCADE)
     project_content_type = models.ForeignKey(ContentType, on_delete=models.CASCADE, null=True, blank=True)
     project_id = models.PositiveIntegerField(null=True, blank=True)
     project = GenericForeignKey('project_content_type', 'project_id')
 
+    objects = NetsCoreBaseManager()
+    
     class Meta:
         verbose_name = _("User Role")
         verbose_name_plural = _("User Roles")
         db_table = 'nets_core_user_role'
 
     def __str__(self):
         if self.project:
```

### Comparing `django_nets_core-0.1.79/nets_core/params.py` & `django_nets_core-0.1.80/nets_core/params.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/responses.py` & `django_nets_core-0.1.80/nets_core/responses.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/security.py` & `django_nets_core-0.1.80/nets_core/security.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/settings.py` & `django_nets_core-0.1.80/nets_core/settings.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/settings_nets.py` & `django_nets_core-0.1.80/nets_core/settings_nets.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/tasks.py` & `django_nets_core-0.1.80/nets_core/tasks.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/templates/nets_core/base.html` & `django_nets_core-0.1.80/nets_core/templates/nets_core/base.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/templates/nets_core/delete_account.html` & `django_nets_core-0.1.80/nets_core/templates/nets_core/delete_account.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/templates/nets_core/email/base_email.html` & `django_nets_core-0.1.80/nets_core/templates/nets_core/email/base_email.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/templates/nets_core/email/new_login.html` & `django_nets_core-0.1.80/nets_core/templates/nets_core/email/new_login.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/urls.py` & `django_nets_core-0.1.80/nets_core/urls.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/utils.py` & `django_nets_core-0.1.80/nets_core/utils.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/nets_core/views.py` & `django_nets_core-0.1.80/nets_core/views.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.79/setup.cfg` & `django_nets_core-0.1.80/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-nets-core
-version = 0.1.79
+version = 0.1.80
 description = A lazy API rest request handler.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/esbozos/django-nets-core
 author = Norman Torres
 author_email = norman.nets@gmail.com
 license = BSD-3-Clause
```

