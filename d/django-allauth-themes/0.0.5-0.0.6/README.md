# Comparing `tmp/django_allauth_themes-0.0.5.tar.gz` & `tmp/django_allauth_themes-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_allauth_themes-0.0.5.tar", last modified: Mon May  6 07:42:40 2024, max compression
+gzip compressed data, was "django_allauth_themes-0.0.6.tar", last modified: Tue May  7 17:38:20 2024, max compression
```

## Comparing `django_allauth_themes-0.0.5.tar` & `django_allauth_themes-0.0.6.tar`

### file list

```diff
@@ -1,80 +1,108 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 07:42:40.409390 django_allauth_themes-0.0.5/
--rw-rw-rw-   0        0        0     1064 2024-05-03 03:15:33.000000 django_allauth_themes-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       40 2024-05-05 13:23:31.000000 django_allauth_themes-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2432 2024-05-06 07:42:40.408391 django_allauth_themes-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      873 2024-05-06 07:39:42.000000 django_allauth_themes-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 07:42:40.322390 django_allauth_themes-0.0.5/allauth_themes/
-drwxrwxrwx   0        0        0        0 2024-05-06 07:42:40.332391 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/
--rw-rw-rw-   0        0        0        0 2024-05-05 17:31:19.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/__init__.py
--rw-rw-rw-   0        0        0      180 2024-05-05 17:47:55.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/apps.py
-drwxrwxrwx   0        0        0        0 2024-05-06 07:42:40.336389 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/
--rw-rw-rw-   0        0        0      293 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/429.html
-drwxrwxrwx   0        0        0        0 2024-05-06 07:42:40.338390 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/account/
--rw-rw-rw-   0        0        0      110 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/account/base_manage_email.html
--rw-rw-rw-   0        0        0      113 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/account/base_manage_password.html
-drwxrwxrwx   0        0        0        0 2024-05-06 07:42:40.320391 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/
-drwxrwxrwx   0        0        0        0 2024-05-06 07:42:40.360391 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/elements/
--rw-rw-rw-   0        0        0      123 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/elements/alert.html
--rw-rw-rw-   0        0        0      348 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/elements/badge.html
--rw-rw-rw-   0        0        0     1615 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/elements/button.html
--rw-rw-rw-   0        0        0      129 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/elements/button__entrance.html
--rw-rw-rw-   0        0        0     3001 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/elements/field.html
--rw-rw-rw-   0        0        0      603 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/elements/fields.html
--rw-rw-rw-   0        0        0      673 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/elements/form.html
--rw-rw-rw-   0        0        0       80 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/elements/form__entrance.html
--rw-rw-rw-   0        0        0       84 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/elements/h1.html
--rw-rw-rw-   0        0        0       92 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/elements/h1__entrance.html
--rw-rw-rw-   0        0        0       92 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/elements/h2__entrance.html
--rw-rw-rw-   0        0        0      152 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/elements/img.html
--rw-rw-rw-   0        0        0      385 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/elements/panel.html
--rw-rw-rw-   0        0        0      122 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/elements/provider.html
--rw-rw-rw-   0        0        0       92 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/elements/provider_list.html
--rw-rw-rw-   0        0        0       97 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/elements/table.html
-drwxrwxrwx   0        0        0        0 2024-05-06 07:42:40.364392 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/layouts/
--rw-rw-rw-   0        0        0     4814 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/layouts/base.html
--rw-rw-rw-   0        0        0      812 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/layouts/entrance.html
--rw-rw-rw-   0        0        0     2444 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/layouts/manage.html
--rw-rw-rw-   0        0        0      232 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/index.html
-drwxrwxrwx   0        0        0        0 2024-05-06 07:42:40.365390 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/mfa/
--rw-rw-rw-   0        0        0      108 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/mfa/base_manage.html
--rw-rw-rw-   0        0        0      188 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/profile.html
-drwxrwxrwx   0        0        0        0 2024-05-06 07:42:40.367390 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/socialaccount/
--rw-rw-rw-   0        0        0      118 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/socialaccount/base_manage.html
-drwxrwxrwx   0        0        0        0 2024-05-06 07:42:40.368392 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/usersessions/
--rw-rw-rw-   0        0        0      117 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/usersessions/base_manage.html
-drwxrwxrwx   0        0        0        0 2024-05-06 07:42:40.371390 django_allauth_themes-0.0.5/allauth_themes/bootstrap/
--rw-rw-rw-   0        0        0        0 2024-05-06 00:10:25.000000 django_allauth_themes-0.0.5/allauth_themes/bootstrap/__init__.py
--rw-rw-rw-   0        0        0      171 2024-05-06 00:11:10.000000 django_allauth_themes-0.0.5/allauth_themes/bootstrap/apps.py
-drwxrwxrwx   0        0        0        0 2024-05-06 07:42:40.324389 django_allauth_themes-0.0.5/allauth_themes/bootstrap/templates/
-drwxrwxrwx   0        0        0        0 2024-05-06 07:42:40.374392 django_allauth_themes-0.0.5/allauth_themes/bootstrap/templates/account/
--rw-rw-rw-   0        0        0     3854 2024-05-06 07:25:58.000000 django_allauth_themes-0.0.5/allauth_themes/bootstrap/templates/account/email.html
--rw-rw-rw-   0        0        0      735 2024-05-06 06:47:15.000000 django_allauth_themes-0.0.5/allauth_themes/bootstrap/templates/account/logout.html
-drwxrwxrwx   0        0        0        0 2024-05-06 07:42:40.324389 django_allauth_themes-0.0.5/allauth_themes/bootstrap/templates/allauth/
-drwxrwxrwx   0        0        0        0 2024-05-06 07:42:40.395390 django_allauth_themes-0.0.5/allauth_themes/bootstrap/templates/allauth/elements/
--rw-rw-rw-   0        0        0       85 2024-05-06 07:02:28.000000 django_allauth_themes-0.0.5/allauth_themes/bootstrap/templates/allauth/elements/alert.html
--rw-rw-rw-   0        0        0      176 2024-05-06 07:31:02.000000 django_allauth_themes-0.0.5/allauth_themes/bootstrap/templates/allauth/elements/badge.html
--rw-rw-rw-   0        0        0      509 2024-05-06 07:20:37.000000 django_allauth_themes-0.0.5/allauth_themes/bootstrap/templates/allauth/elements/button.html
--rw-rw-rw-   0        0        0      510 2024-05-06 07:24:12.000000 django_allauth_themes-0.0.5/allauth_themes/bootstrap/templates/allauth/elements/button_sm.html
--rw-rw-rw-   0        0        0     2445 2024-05-06 00:40:51.000000 django_allauth_themes-0.0.5/allauth_themes/bootstrap/templates/allauth/elements/field.html
--rw-rw-rw-   0        0        0      602 2024-05-06 00:18:33.000000 django_allauth_themes-0.0.5/allauth_themes/bootstrap/templates/allauth/elements/fields.html
--rw-rw-rw-   0        0        0      169 2024-05-06 05:47:09.000000 django_allauth_themes-0.0.5/allauth_themes/bootstrap/templates/allauth/elements/form.html
--rw-rw-rw-   0        0        0       91 2024-05-06 06:43:56.000000 django_allauth_themes-0.0.5/allauth_themes/bootstrap/templates/allauth/elements/h1.html
--rw-rw-rw-   0        0        0       91 2024-05-06 07:11:22.000000 django_allauth_themes-0.0.5/allauth_themes/bootstrap/templates/allauth/elements/h2.html
--rw-rw-rw-   0        0        0       57 2024-05-06 07:04:59.000000 django_allauth_themes-0.0.5/allauth_themes/bootstrap/templates/allauth/elements/hr.html
--rw-rw-rw-   0        0        0       84 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.5/allauth_themes/bootstrap/templates/allauth/elements/img.html
--rw-rw-rw-   0        0        0      293 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.5/allauth_themes/bootstrap/templates/allauth/elements/panel.html
--rw-rw-rw-   0        0        0      124 2024-05-06 07:11:06.000000 django_allauth_themes-0.0.5/allauth_themes/bootstrap/templates/allauth/elements/provider.html
--rw-rw-rw-   0        0        0       73 2024-05-06 07:06:58.000000 django_allauth_themes-0.0.5/allauth_themes/bootstrap/templates/allauth/elements/provider_list.html
--rw-rw-rw-   0        0        0       69 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.5/allauth_themes/bootstrap/templates/allauth/elements/table.html
-drwxrwxrwx   0        0        0        0 2024-05-06 07:42:40.398391 django_allauth_themes-0.0.5/allauth_themes/bootstrap/templates/allauth/layouts/
--rw-rw-rw-   0        0        0      922 2024-05-06 05:36:26.000000 django_allauth_themes-0.0.5/allauth_themes/bootstrap/templates/allauth/layouts/base.html
--rw-rw-rw-   0        0        0      250 2024-05-06 06:47:32.000000 django_allauth_themes-0.0.5/allauth_themes/bootstrap/templates/allauth/layouts/entrance.html
--rw-rw-rw-   0        0        0      250 2024-05-06 07:16:24.000000 django_allauth_themes-0.0.5/allauth_themes/bootstrap/templates/allauth/layouts/manage.html
-drwxrwxrwx   0        0        0        0 2024-05-06 07:42:40.407392 django_allauth_themes-0.0.5/django_allauth_themes.egg-info/
--rw-rw-rw-   0        0        0     2432 2024-05-06 07:42:40.000000 django_allauth_themes-0.0.5/django_allauth_themes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3586 2024-05-06 07:42:40.000000 django_allauth_themes-0.0.5/django_allauth_themes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 07:42:40.000000 django_allauth_themes-0.0.5/django_allauth_themes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-06 07:42:40.000000 django_allauth_themes-0.0.5/django_allauth_themes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-06 07:42:40.000000 django_allauth_themes-0.0.5/django_allauth_themes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      529 2024-05-06 07:42:29.000000 django_allauth_themes-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-06 07:42:40.410390 django_allauth_themes-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-07 17:38:20.463909 django_allauth_themes-0.0.6/
+-rw-rw-rw-   0        0        0     1064 2024-05-03 03:15:33.000000 django_allauth_themes-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       40 2024-05-05 13:23:31.000000 django_allauth_themes-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2596 2024-05-07 17:38:20.461908 django_allauth_themes-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1037 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 17:38:20.338553 django_allauth_themes-0.0.6/allauth_themes/
+drwxrwxrwx   0        0        0        0 2024-05-07 17:38:20.348797 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/
+-rw-rw-rw-   0        0        0        0 2024-05-05 17:31:19.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/__init__.py
+-rw-rw-rw-   0        0        0      180 2024-05-05 17:47:55.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-07 17:38:20.353798 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/
+-rw-rw-rw-   0        0        0      293 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/429.html
+drwxrwxrwx   0        0        0        0 2024-05-07 17:38:20.355798 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/account/
+-rw-rw-rw-   0        0        0      110 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/account/base_manage_email.html
+-rw-rw-rw-   0        0        0      113 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/account/base_manage_password.html
+drwxrwxrwx   0        0        0        0 2024-05-07 17:38:20.332878 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/
+drwxrwxrwx   0        0        0        0 2024-05-07 17:38:20.379111 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/elements/
+-rw-rw-rw-   0        0        0      123 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/elements/alert.html
+-rw-rw-rw-   0        0        0      348 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/elements/badge.html
+-rw-rw-rw-   0        0        0     1615 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/elements/button.html
+-rw-rw-rw-   0        0        0      129 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/elements/button__entrance.html
+-rw-rw-rw-   0        0        0     3001 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/elements/field.html
+-rw-rw-rw-   0        0        0      603 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/elements/fields.html
+-rw-rw-rw-   0        0        0      673 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/elements/form.html
+-rw-rw-rw-   0        0        0       80 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/elements/form__entrance.html
+-rw-rw-rw-   0        0        0       84 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/elements/h1.html
+-rw-rw-rw-   0        0        0       92 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/elements/h1__entrance.html
+-rw-rw-rw-   0        0        0       92 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/elements/h2__entrance.html
+-rw-rw-rw-   0        0        0      152 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/elements/img.html
+-rw-rw-rw-   0        0        0      385 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/elements/panel.html
+-rw-rw-rw-   0        0        0      122 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/elements/provider.html
+-rw-rw-rw-   0        0        0       92 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/elements/provider_list.html
+-rw-rw-rw-   0        0        0       97 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/elements/table.html
+drwxrwxrwx   0        0        0        0 2024-05-07 17:38:20.383109 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/layouts/
+-rw-rw-rw-   0        0        0     4814 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/layouts/base.html
+-rw-rw-rw-   0        0        0      812 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/layouts/entrance.html
+-rw-rw-rw-   0        0        0     2444 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/layouts/manage.html
+-rw-rw-rw-   0        0        0      232 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/index.html
+drwxrwxrwx   0        0        0        0 2024-05-07 17:38:20.384917 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/mfa/
+-rw-rw-rw-   0        0        0      108 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/mfa/base_manage.html
+-rw-rw-rw-   0        0        0      188 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/profile.html
+drwxrwxrwx   0        0        0        0 2024-05-07 17:38:20.385938 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/socialaccount/
+-rw-rw-rw-   0        0        0      118 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/socialaccount/base_manage.html
+drwxrwxrwx   0        0        0        0 2024-05-07 17:38:20.387935 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/usersessions/
+-rw-rw-rw-   0        0        0      117 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/usersessions/base_manage.html
+drwxrwxrwx   0        0        0        0 2024-05-07 17:38:20.389935 django_allauth_themes-0.0.6/allauth_themes/bootstrap/
+-rw-rw-rw-   0        0        0        0 2024-05-06 00:10:25.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap/__init__.py
+-rw-rw-rw-   0        0        0      171 2024-05-06 00:11:10.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-07 17:38:20.391936 django_allauth_themes-0.0.6/allauth_themes/bootstrap/templates/
+-rw-rw-rw-   0        0        0      306 2024-05-06 08:13:31.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap/templates/429.html
+drwxrwxrwx   0        0        0        0 2024-05-07 17:38:20.336878 django_allauth_themes-0.0.6/allauth_themes/bootstrap/templates/allauth/
+drwxrwxrwx   0        0        0        0 2024-05-07 17:38:20.415251 django_allauth_themes-0.0.6/allauth_themes/bootstrap/templates/allauth/elements/
+-rw-rw-rw-   0        0        0      129 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap/templates/allauth/elements/alert.html
+-rw-rw-rw-   0        0        0      364 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap/templates/allauth/elements/badge.html
+-rw-rw-rw-   0        0        0     1649 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap/templates/allauth/elements/button.html
+-rw-rw-rw-   0        0        0      135 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap/templates/allauth/elements/button__entrance.html
+-rw-rw-rw-   0        0        0      181 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap/templates/allauth/elements/button__manage.html
+-rw-rw-rw-   0        0        0     3072 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap/templates/allauth/elements/field.html
+-rw-rw-rw-   0        0        0      614 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap/templates/allauth/elements/fields.html
+-rw-rw-rw-   0        0        0      687 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap/templates/allauth/elements/form.html
+-rw-rw-rw-   0        0        0       82 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap/templates/allauth/elements/form__entrance.html
+-rw-rw-rw-   0        0        0       89 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap/templates/allauth/elements/h1.html
+-rw-rw-rw-   0        0        0       97 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap/templates/allauth/elements/h1__entrance.html
+-rw-rw-rw-   0        0        0       97 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap/templates/allauth/elements/h2__entrance.html
+-rw-rw-rw-   0        0        0      157 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap/templates/allauth/elements/img.html
+-rw-rw-rw-   0        0        0      402 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap/templates/allauth/elements/panel.html
+-rw-rw-rw-   0        0        0      747 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap/templates/allauth/elements/provider.html
+-rw-rw-rw-   0        0        0       97 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap/templates/allauth/elements/provider_list.html
+-rw-rw-rw-   0        0        0      102 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap/templates/allauth/elements/table.html
+drwxrwxrwx   0        0        0        0 2024-05-07 17:38:20.419748 django_allauth_themes-0.0.6/allauth_themes/bootstrap/templates/allauth/layouts/
+-rw-rw-rw-   0        0        0     1059 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap/templates/allauth/layouts/base.html
+-rw-rw-rw-   0        0        0      287 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap/templates/allauth/layouts/entrance.html
+-rw-rw-rw-   0        0        0      262 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap/templates/allauth/layouts/manage.html
+drwxrwxrwx   0        0        0        0 2024-05-07 17:38:20.421766 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/
+-rw-rw-rw-   0        0        0        0 2024-05-07 10:36:08.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/__init__.py
+-rw-rw-rw-   0        0        0      190 2024-05-07 10:36:08.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-07 17:38:20.423875 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/templates/
+-rw-rw-rw-   0        0        0      306 2024-05-06 08:13:31.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/templates/429.html
+drwxrwxrwx   0        0        0        0 2024-05-07 17:38:20.340780 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/templates/allauth/
+drwxrwxrwx   0        0        0        0 2024-05-07 17:38:20.446923 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/templates/allauth/elements/
+-rw-rw-rw-   0        0        0      129 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/templates/allauth/elements/alert.html
+-rw-rw-rw-   0        0        0      364 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/templates/allauth/elements/badge.html
+-rw-rw-rw-   0        0        0     1656 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/templates/allauth/elements/button.html
+-rw-rw-rw-   0        0        0      135 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/templates/allauth/elements/button__entrance.html
+-rw-rw-rw-   0        0        0      181 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/templates/allauth/elements/button__manage.html
+-rw-rw-rw-   0        0        0     3316 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/templates/allauth/elements/field.html
+-rw-rw-rw-   0        0        0      614 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/templates/allauth/elements/fields.html
+-rw-rw-rw-   0        0        0      697 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/templates/allauth/elements/form.html
+-rw-rw-rw-   0        0        0       82 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/templates/allauth/elements/form__entrance.html
+-rw-rw-rw-   0        0        0       89 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/templates/allauth/elements/h1.html
+-rw-rw-rw-   0        0        0       97 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/templates/allauth/elements/h1__entrance.html
+-rw-rw-rw-   0        0        0       97 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/templates/allauth/elements/h2__entrance.html
+-rw-rw-rw-   0        0        0      157 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/templates/allauth/elements/img.html
+-rw-rw-rw-   0        0        0      402 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/templates/allauth/elements/panel.html
+-rw-rw-rw-   0        0        0      747 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/templates/allauth/elements/provider.html
+-rw-rw-rw-   0        0        0       97 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/templates/allauth/elements/provider_list.html
+-rw-rw-rw-   0        0        0      102 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/templates/allauth/elements/table.html
+drwxrwxrwx   0        0        0        0 2024-05-07 17:38:20.451308 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/templates/allauth/layouts/
+-rw-rw-rw-   0        0        0     1059 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/templates/allauth/layouts/base.html
+-rw-rw-rw-   0        0        0      306 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/templates/allauth/layouts/entrance.html
+-rw-rw-rw-   0        0        0      281 2024-05-07 17:35:02.000000 django_allauth_themes-0.0.6/allauth_themes/bootstrap_grayscale/templates/allauth/layouts/manage.html
+drwxrwxrwx   0        0        0        0 2024-05-07 17:38:20.460910 django_allauth_themes-0.0.6/django_allauth_themes.egg-info/
+-rw-rw-rw-   0        0        0     2596 2024-05-07 17:38:20.000000 django_allauth_themes-0.0.6/django_allauth_themes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5346 2024-05-07 17:38:20.000000 django_allauth_themes-0.0.6/django_allauth_themes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 17:38:20.000000 django_allauth_themes-0.0.6/django_allauth_themes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-07 17:38:20.000000 django_allauth_themes-0.0.6/django_allauth_themes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-07 17:38:20.000000 django_allauth_themes-0.0.6/django_allauth_themes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      529 2024-05-07 17:38:07.000000 django_allauth_themes-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-07 17:38:20.463909 django_allauth_themes-0.0.6/setup.cfg
```

### Comparing `django_allauth_themes-0.0.5/LICENSE` & `django_allauth_themes-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django_allauth_themes-0.0.5/PKG-INFO` & `django_allauth_themes-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-allauth-themes
-Version: 0.0.5
+Version: 0.0.6
 Summary: Themes for Django-Allauth
 Author-email: stackmuse <stackmuse@github.com>
 License: Copyright 2024 StackMuse
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -55,8 +55,13 @@
     - Example theme provided by Django-Allauth
     - Must add `path("i18n/", include("django.conf.urls.i18n")),` to `urls.py`
     ![](https://i.imgur.com/eCtNzPb.png)
 
 1. `allauth_themes.bootstrap`
     - Basic Bootstrap 5 style
     - Blue buttons, rounded corners
-    ![](https://i.imgur.com/QVSZGUf.png)
+    ![](https://i.imgur.com/YVKfiIe.png)
+
+1. `allauth_themes.bootstrap_grayscale`
+    - Bootstrap 5 style
+    - Black buttons, shades of gray, squared corners
+    ![](https://i.imgur.com/nO03Mq0.png)
```

### Comparing `django_allauth_themes-0.0.5/README.md` & `django_allauth_themes-0.0.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -35,8 +35,13 @@
     - Example theme provided by Django-Allauth
     - Must add `path("i18n/", include("django.conf.urls.i18n")),` to `urls.py`
     ![](https://i.imgur.com/eCtNzPb.png)
 
 1. `allauth_themes.bootstrap`
     - Basic Bootstrap 5 style
     - Blue buttons, rounded corners
-    ![](https://i.imgur.com/QVSZGUf.png)
+    ![](https://i.imgur.com/YVKfiIe.png)
+
+1. `allauth_themes.bootstrap_grayscale`
+    - Bootstrap 5 style
+    - Black buttons, shades of gray, squared corners
+    ![](https://i.imgur.com/nO03Mq0.png)
```

### Comparing `django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/elements/button.html` & `django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/elements/button.html`

 * *Files identical despite different names*

### Comparing `django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/elements/field.html` & `django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/elements/field.html`

 * *Files identical despite different names*

### Comparing `django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/elements/fields.html` & `django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/elements/fields.html`

 * *Files identical despite different names*

### Comparing `django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/elements/form.html` & `django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/elements/form.html`

 * *Files identical despite different names*

### Comparing `django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/layouts/base.html` & `django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/layouts/base.html`

 * *Files identical despite different names*

### Comparing `django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/layouts/entrance.html` & `django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/layouts/entrance.html`

 * *Files identical despite different names*

### Comparing `django_allauth_themes-0.0.5/allauth_themes/allauth_bootstrap/templates/allauth/layouts/manage.html` & `django_allauth_themes-0.0.6/allauth_themes/allauth_bootstrap/templates/allauth/layouts/manage.html`

 * *Files identical despite different names*

### Comparing `django_allauth_themes-0.0.5/allauth_themes/bootstrap/templates/allauth/layouts/base.html` & `django_allauth_themes-0.0.6/allauth_themes/bootstrap/templates/allauth/layouts/base.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-{% load static %}
-<!DOCTYPE html>
-<html lang="en">
-<head>
-  <meta charset="utf-8">
-  <meta name="viewport" content="width=device-width, initial-scale=1">
-  <link integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH"
-        href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css"
-        crossorigin="anonymous" rel="stylesheet">
-  <title>{% block head_title %}{% endblock %}</title>
-  <link rel="stylesheet" href="{% static 'bootstrap/css/style.css' %}">
-  {% block extra_head %}{% endblock %}
-</head>
-<body>
-  {% block body %}
-    {% block content %}{% endblock %}
-  {% endblock %}
-  <script integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz"
-          src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"
-          crossorigin="anonymous"></script>
-  {% block extra_body %}{% endblock %}
-</body>
-</html>
+{% load static %}
+<!DOCTYPE html>
+<html lang="en">
+<head>
+  <meta charset="utf-8">
+  <meta name="viewport" content="width=device-width, initial-scale=1">
+  <link integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH"
+        href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css"
+        crossorigin="anonymous" rel="stylesheet">
+  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">
+  <title>{% block head_title %}{% endblock %}</title>
+  <link rel="stylesheet" href="{% static 'allauth/css/style.css' %}">
+  {% block extra_head %}{% endblock %}
+</head>
+<body>
+  {% block body %}
+    {% block content %}{% endblock %}
+  {% endblock %}
+  <script integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz"
+          src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"
+          crossorigin="anonymous"></script>
+  {% block extra_body %}{% endblock %}
+</body>
+</html>
```

### Comparing `django_allauth_themes-0.0.5/django_allauth_themes.egg-info/PKG-INFO` & `django_allauth_themes-0.0.6/django_allauth_themes.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-allauth-themes
-Version: 0.0.5
+Version: 0.0.6
 Summary: Themes for Django-Allauth
 Author-email: stackmuse <stackmuse@github.com>
 License: Copyright 2024 StackMuse
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -55,8 +55,13 @@
     - Example theme provided by Django-Allauth
     - Must add `path("i18n/", include("django.conf.urls.i18n")),` to `urls.py`
     ![](https://i.imgur.com/eCtNzPb.png)
 
 1. `allauth_themes.bootstrap`
     - Basic Bootstrap 5 style
     - Blue buttons, rounded corners
-    ![](https://i.imgur.com/QVSZGUf.png)
+    ![](https://i.imgur.com/YVKfiIe.png)
+
+1. `allauth_themes.bootstrap_grayscale`
+    - Bootstrap 5 style
+    - Black buttons, shades of gray, squared corners
+    ![](https://i.imgur.com/nO03Mq0.png)
```

### Comparing `django_allauth_themes-0.0.5/django_allauth_themes.egg-info/SOURCES.txt` & `django_allauth_themes-0.0.6/django_allauth_themes.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -29,32 +29,56 @@
 allauth_themes/allauth_bootstrap/templates/allauth/layouts/entrance.html
 allauth_themes/allauth_bootstrap/templates/allauth/layouts/manage.html
 allauth_themes/allauth_bootstrap/templates/mfa/base_manage.html
 allauth_themes/allauth_bootstrap/templates/socialaccount/base_manage.html
 allauth_themes/allauth_bootstrap/templates/usersessions/base_manage.html
 allauth_themes/bootstrap/__init__.py
 allauth_themes/bootstrap/apps.py
-allauth_themes/bootstrap/templates/account/email.html
-allauth_themes/bootstrap/templates/account/logout.html
+allauth_themes/bootstrap/templates/429.html
 allauth_themes/bootstrap/templates/allauth/elements/alert.html
 allauth_themes/bootstrap/templates/allauth/elements/badge.html
 allauth_themes/bootstrap/templates/allauth/elements/button.html
-allauth_themes/bootstrap/templates/allauth/elements/button_sm.html
+allauth_themes/bootstrap/templates/allauth/elements/button__entrance.html
+allauth_themes/bootstrap/templates/allauth/elements/button__manage.html
 allauth_themes/bootstrap/templates/allauth/elements/field.html
 allauth_themes/bootstrap/templates/allauth/elements/fields.html
 allauth_themes/bootstrap/templates/allauth/elements/form.html
+allauth_themes/bootstrap/templates/allauth/elements/form__entrance.html
 allauth_themes/bootstrap/templates/allauth/elements/h1.html
-allauth_themes/bootstrap/templates/allauth/elements/h2.html
-allauth_themes/bootstrap/templates/allauth/elements/hr.html
+allauth_themes/bootstrap/templates/allauth/elements/h1__entrance.html
+allauth_themes/bootstrap/templates/allauth/elements/h2__entrance.html
 allauth_themes/bootstrap/templates/allauth/elements/img.html
 allauth_themes/bootstrap/templates/allauth/elements/panel.html
 allauth_themes/bootstrap/templates/allauth/elements/provider.html
 allauth_themes/bootstrap/templates/allauth/elements/provider_list.html
 allauth_themes/bootstrap/templates/allauth/elements/table.html
 allauth_themes/bootstrap/templates/allauth/layouts/base.html
 allauth_themes/bootstrap/templates/allauth/layouts/entrance.html
 allauth_themes/bootstrap/templates/allauth/layouts/manage.html
+allauth_themes/bootstrap_grayscale/__init__.py
+allauth_themes/bootstrap_grayscale/apps.py
+allauth_themes/bootstrap_grayscale/templates/429.html
+allauth_themes/bootstrap_grayscale/templates/allauth/elements/alert.html
+allauth_themes/bootstrap_grayscale/templates/allauth/elements/badge.html
+allauth_themes/bootstrap_grayscale/templates/allauth/elements/button.html
+allauth_themes/bootstrap_grayscale/templates/allauth/elements/button__entrance.html
+allauth_themes/bootstrap_grayscale/templates/allauth/elements/button__manage.html
+allauth_themes/bootstrap_grayscale/templates/allauth/elements/field.html
+allauth_themes/bootstrap_grayscale/templates/allauth/elements/fields.html
+allauth_themes/bootstrap_grayscale/templates/allauth/elements/form.html
+allauth_themes/bootstrap_grayscale/templates/allauth/elements/form__entrance.html
+allauth_themes/bootstrap_grayscale/templates/allauth/elements/h1.html
+allauth_themes/bootstrap_grayscale/templates/allauth/elements/h1__entrance.html
+allauth_themes/bootstrap_grayscale/templates/allauth/elements/h2__entrance.html
+allauth_themes/bootstrap_grayscale/templates/allauth/elements/img.html
+allauth_themes/bootstrap_grayscale/templates/allauth/elements/panel.html
+allauth_themes/bootstrap_grayscale/templates/allauth/elements/provider.html
+allauth_themes/bootstrap_grayscale/templates/allauth/elements/provider_list.html
+allauth_themes/bootstrap_grayscale/templates/allauth/elements/table.html
+allauth_themes/bootstrap_grayscale/templates/allauth/layouts/base.html
+allauth_themes/bootstrap_grayscale/templates/allauth/layouts/entrance.html
+allauth_themes/bootstrap_grayscale/templates/allauth/layouts/manage.html
 django_allauth_themes.egg-info/PKG-INFO
 django_allauth_themes.egg-info/SOURCES.txt
 django_allauth_themes.egg-info/dependency_links.txt
 django_allauth_themes.egg-info/requires.txt
 django_allauth_themes.egg-info/top_level.txt
```

### Comparing `django_allauth_themes-0.0.5/pyproject.toml` & `django_allauth_themes-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 69.5"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-allauth-themes"
-version = "0.0.5"
+version = "0.0.6"
 description = "Themes for Django-Allauth"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
   {name = "stackmuse", email = "stackmuse@github.com" }
 ]
```

