# Comparing `tmp/django_money-3.5.1.tar.gz` & `tmp/django_money-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_money-3.5.1.tar", last modified: Sun May  5 16:42:52 2024, max compression
+gzip compressed data, was "django_money-3.5.2.tar", last modified: Tue May  7 21:31:58 2024, max compression
```

## Comparing `django_money-3.5.1.tar` & `django_money-3.5.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:42:52.837454 django_money-3.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-05 16:42:44.000000 django_money-3.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-05 16:42:44.000000 django_money-3.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18278 2024-05-05 16:42:52.837454 django_money-3.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16571 2024-05-05 16:42:44.000000 django_money-3.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:42:52.837454 django_money-3.5.1/django_money.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18278 2024-05-05 16:42:52.000000 django_money-3.5.1/django_money.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-05 16:42:52.000000 django_money-3.5.1/django_money.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 16:42:52.000000 django_money-3.5.1/django_money.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-05 16:42:52.000000 django_money-3.5.1/django_money.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-05 16:42:52.000000 django_money-3.5.1/django_money.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:42:52.829454 django_money-3.5.1/djmoney/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:42:52.829454 django_money-3.5.1/djmoney/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:42:52.829454 django_money-3.5.1/djmoney/contrib/django_rest_framework/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/contrib/django_rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/contrib/django_rest_framework/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:42:52.833454 django_money-3.5.1/djmoney/contrib/exchange/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/contrib/exchange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/contrib/exchange/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:42:52.833454 django_money-3.5.1/djmoney/contrib/exchange/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/contrib/exchange/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/contrib/exchange/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/contrib/exchange/backends/fixer.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/contrib/exchange/backends/openexchangerates.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/contrib/exchange/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:42:52.833454 django_money-3.5.1/djmoney/contrib/exchange/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/contrib/exchange/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/contrib/exchange/management/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:42:52.833454 django_money-3.5.1/djmoney/contrib/exchange/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/contrib/exchange/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/contrib/exchange/management/commands/clear_rates.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/contrib/exchange/management/commands/update_rates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:42:52.833454 django_money-3.5.1/djmoney/contrib/exchange/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/contrib/exchange/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/contrib/exchange/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/contrib/exchange/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:42:52.833454 django_money-3.5.1/djmoney/forms/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/forms/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/forms/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:42:52.833454 django_money-3.5.1/djmoney/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13303 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/models/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/models/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/models/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/money.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/money.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:42:52.837454 django_money-3.5.1/djmoney/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/templatetags/djmoney.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-05 16:42:44.000000 django_money-3.5.1/djmoney/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-05 16:42:44.000000 django_money-3.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-05 16:42:52.841454 django_money-3.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-05-05 16:42:44.000000 django_money-3.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:42:52.837454 django_money-3.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-05 16:42:44.000000 django_money-3.5.1/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-05-05 16:42:44.000000 django_money-3.5.1/tests/test_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-05-05 16:42:44.000000 django_money-3.5.1/tests/test_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)    39497 2024-05-05 16:42:44.000000 django_money-3.5.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-05 16:42:44.000000 django_money-3.5.1/tests/test_money.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-05 16:42:44.000000 django_money-3.5.1/tests/test_reversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-05 16:42:44.000000 django_money-3.5.1/tests/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-05 16:42:44.000000 django_money-3.5.1/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-05 16:42:44.000000 django_money-3.5.1/tests/test_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:31:58.042766 django_money-3.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-07 21:31:47.000000 django_money-3.5.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-07 21:31:47.000000 django_money-3.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18279 2024-05-07 21:31:58.042766 django_money-3.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16572 2024-05-07 21:31:47.000000 django_money-3.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:31:58.038766 django_money-3.5.2/django_money.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18279 2024-05-07 21:31:58.000000 django_money-3.5.2/django_money.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-07 21:31:58.000000 django_money-3.5.2/django_money.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 21:31:58.000000 django_money-3.5.2/django_money.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 21:31:58.000000 django_money-3.5.2/django_money.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 21:31:58.000000 django_money-3.5.2/django_money.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:31:58.030766 django_money-3.5.2/djmoney/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:31:58.030766 django_money-3.5.2/djmoney/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:31:58.034766 django_money-3.5.2/djmoney/contrib/django_rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/contrib/django_rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/contrib/django_rest_framework/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:31:58.034766 django_money-3.5.2/djmoney/contrib/exchange/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/contrib/exchange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/contrib/exchange/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:31:58.034766 django_money-3.5.2/djmoney/contrib/exchange/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/contrib/exchange/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/contrib/exchange/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/contrib/exchange/backends/fixer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/contrib/exchange/backends/openexchangerates.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/contrib/exchange/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:31:58.034766 django_money-3.5.2/djmoney/contrib/exchange/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/contrib/exchange/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/contrib/exchange/management/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:31:58.034766 django_money-3.5.2/djmoney/contrib/exchange/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/contrib/exchange/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/contrib/exchange/management/commands/clear_rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/contrib/exchange/management/commands/update_rates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:31:58.034766 django_money-3.5.2/djmoney/contrib/exchange/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/contrib/exchange/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/contrib/exchange/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/contrib/exchange/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:31:58.034766 django_money-3.5.2/djmoney/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/forms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/forms/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:31:58.038766 django_money-3.5.2/djmoney/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13303 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/models/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/models/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/models/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/money.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/money.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:31:58.038766 django_money-3.5.2/djmoney/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/templatetags/djmoney.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-07 21:31:47.000000 django_money-3.5.2/djmoney/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 21:31:47.000000 django_money-3.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-07 21:31:58.042766 django_money-3.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-05-07 21:31:47.000000 django_money-3.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:31:58.038766 django_money-3.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-07 21:31:47.000000 django_money-3.5.2/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-05-07 21:31:47.000000 django_money-3.5.2/tests/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-05-07 21:31:47.000000 django_money-3.5.2/tests/test_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39497 2024-05-07 21:31:47.000000 django_money-3.5.2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-07 21:31:47.000000 django_money-3.5.2/tests/test_money.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-07 21:31:47.000000 django_money-3.5.2/tests/test_reversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-07 21:31:47.000000 django_money-3.5.2/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-07 21:31:47.000000 django_money-3.5.2/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-07 21:31:47.000000 django_money-3.5.2/tests/test_tags.py
```

### Comparing `django_money-3.5.1/LICENSE.txt` & `django_money-3.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/PKG-INFO` & `django_money-3.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-money
-Version: 3.5.1
+Version: 3.5.2
 Summary: Adds support for using money and currency fields in django models and forms. Uses py-moneyed as the money implementation.
 Home-page: https://github.com/django-money/django-money
 Maintainer: Greg Reinbach
 Maintainer-email: greg@reinbach.com
 License: BSD
 Keywords: django,py-money,money
 Platform: Any
@@ -462,15 +462,15 @@
 Both of them accept ``-b/--backend`` option, that will update/clear data only for this backend.
 And ``clear_rates`` accepts ``-a/--all`` option, that will clear data for all backends.
 
 To set up a periodic rates update you could use Celery task:
 
 .. code:: python
 
-    CELERYBEAT_SCHEDULE = {
+    CELERY_BEAT_SCHEDULE = {
         'update_rates': {
             'task': 'path.to.your.task',
             'schedule': crontab(minute=0, hour=0),
             'kwargs': {}  # For custom arguments
         }
     }
```

### Comparing `django_money-3.5.1/README.rst` & `django_money-3.5.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -419,15 +419,15 @@
 Both of them accept ``-b/--backend`` option, that will update/clear data only for this backend.
 And ``clear_rates`` accepts ``-a/--all`` option, that will clear data for all backends.
 
 To set up a periodic rates update you could use Celery task:
 
 .. code:: python
 
-    CELERYBEAT_SCHEDULE = {
+    CELERY_BEAT_SCHEDULE = {
         'update_rates': {
             'task': 'path.to.your.task',
             'schedule': crontab(minute=0, hour=0),
             'kwargs': {}  # For custom arguments
         }
     }
```

### Comparing `django_money-3.5.1/django_money.egg-info/PKG-INFO` & `django_money-3.5.2/django_money.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-money
-Version: 3.5.1
+Version: 3.5.2
 Summary: Adds support for using money and currency fields in django models and forms. Uses py-moneyed as the money implementation.
 Home-page: https://github.com/django-money/django-money
 Maintainer: Greg Reinbach
 Maintainer-email: greg@reinbach.com
 License: BSD
 Keywords: django,py-money,money
 Platform: Any
@@ -462,15 +462,15 @@
 Both of them accept ``-b/--backend`` option, that will update/clear data only for this backend.
 And ``clear_rates`` accepts ``-a/--all`` option, that will clear data for all backends.
 
 To set up a periodic rates update you could use Celery task:
 
 .. code:: python
 
-    CELERYBEAT_SCHEDULE = {
+    CELERY_BEAT_SCHEDULE = {
         'update_rates': {
             'task': 'path.to.your.task',
             'schedule': crontab(minute=0, hour=0),
             'kwargs': {}  # For custom arguments
         }
     }
```

### Comparing `django_money-3.5.1/django_money.egg-info/SOURCES.txt` & `django_money-3.5.2/django_money.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/djmoney/_compat.py` & `django_money-3.5.2/djmoney/_compat.py`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/djmoney/admin.py` & `django_money-3.5.2/djmoney/admin.py`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/djmoney/contrib/django_rest_framework/fields.py` & `django_money-3.5.2/djmoney/contrib/django_rest_framework/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
     def get_value(self, data):
         default_currency = None
         parent_meta = getattr(self.parent, "Meta", None)
 
         if parent_meta and hasattr(parent_meta, "model"):
             model_meta = self.parent.Meta.model._meta
-            field = model_meta.get_field(self.field_name)
+            field = model_meta.get_field(self.source)
             default_currency = field.default_currency
 
         amount = super().get_value(data)
         currency = data.get(get_currency_field_name(self.field_name), self.default_currency or default_currency)
         if currency and amount is not None and not isinstance(amount, MONEY_CLASSES) and amount is not empty:
             return _PrimitiveMoney(amount=amount, currency=currency)
         return amount
```

### Comparing `django_money-3.5.1/djmoney/contrib/exchange/backends/base.py` & `django_money-3.5.2/djmoney/contrib/exchange/backends/base.py`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/djmoney/contrib/exchange/backends/fixer.py` & `django_money-3.5.2/djmoney/contrib/exchange/backends/fixer.py`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/djmoney/contrib/exchange/backends/openexchangerates.py` & `django_money-3.5.2/djmoney/contrib/exchange/backends/openexchangerates.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,8 +14,8 @@
             raise ImproperlyConfigured(
                 "settings.OPEN_EXCHANGE_RATES_APP_ID should be set to use OpenExchangeRatesBackend"
             )
         self.url = url
         self.access_key = access_key
 
     def get_params(self):
-        return {"app_id": self.access_key}
+        return {"app_id": self.access_key, "base": settings.BASE_CURRENCY}
```

### Comparing `django_money-3.5.1/djmoney/contrib/exchange/management/base.py` & `django_money-3.5.2/djmoney/contrib/exchange/management/base.py`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/djmoney/contrib/exchange/management/commands/clear_rates.py` & `django_money-3.5.2/djmoney/contrib/exchange/management/commands/clear_rates.py`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/djmoney/contrib/exchange/migrations/0001_initial.py` & `django_money-3.5.2/djmoney/contrib/exchange/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/djmoney/contrib/exchange/models.py` & `django_money-3.5.2/djmoney/contrib/exchange/models.py`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/djmoney/forms/fields.py` & `django_money-3.5.2/djmoney/forms/fields.py`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/djmoney/forms/widgets.py` & `django_money-3.5.2/djmoney/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/djmoney/models/fields.py` & `django_money-3.5.2/djmoney/models/fields.py`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/djmoney/models/managers.py` & `django_money-3.5.2/djmoney/models/managers.py`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/djmoney/models/validators.py` & `django_money-3.5.2/djmoney/models/validators.py`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/djmoney/money.py` & `django_money-3.5.2/djmoney/money.py`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/djmoney/money.pyi` & `django_money-3.5.2/djmoney/money.pyi`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/djmoney/serializers.py` & `django_money-3.5.2/djmoney/serializers.py`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/djmoney/settings.py` & `django_money-3.5.2/djmoney/settings.py`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/djmoney/templatetags/djmoney.py` & `django_money-3.5.2/djmoney/templatetags/djmoney.py`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/djmoney/utils.py` & `django_money-3.5.2/djmoney/utils.py`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/setup.cfg` & `django_money-3.5.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/setup.py` & `django_money-3.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/tests/test_admin.py` & `django_money-3.5.2/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/tests/test_form.py` & `django_money-3.5.2/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/tests/test_managers.py` & `django_money-3.5.2/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/tests/test_models.py` & `django_money-3.5.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/tests/test_money.py` & `django_money-3.5.2/tests/test_money.py`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/tests/test_reversion.py` & `django_money-3.5.2/tests/test_reversion.py`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/tests/test_serialization.py` & `django_money-3.5.2/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/tests/test_settings.py` & `django_money-3.5.2/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django_money-3.5.1/tests/test_tags.py` & `django_money-3.5.2/tests/test_tags.py`

 * *Files identical despite different names*

