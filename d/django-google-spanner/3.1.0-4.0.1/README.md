# Comparing `tmp/django-google-spanner-3.1.0.tar.gz` & `tmp/django-google-spanner-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-google-spanner-3.1.0.tar", last modified: Tue Apr 23 13:03:04 2024, max compression
+gzip compressed data, was "django-google-spanner-4.0.1.tar", last modified: Tue May  7 08:03:15 2024, max compression
```

## Comparing `django-google-spanner-3.1.0.tar` & `django-google-spanner-4.0.1.tar`

### file list

```diff
@@ -1,62 +1,61 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-23 13:03:04.488239 django-google-spanner-3.1.0/
--rw-rw-r--   0 root         (0)     1003     1448 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/LICENSE
--rw-r--r--   0 root         (0)     1003     9380 2024-04-23 13:03:04.488239 django-google-spanner-3.1.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     8103 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-23 13:03:04.488239 django-google-spanner-3.1.0/django_google_spanner.egg-info/
--rw-r--r--   0 root         (0)     1003     9380 2024-04-23 13:03:04.000000 django-google-spanner-3.1.0/django_google_spanner.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1788 2024-04-23 13:03:04.000000 django-google-spanner-3.1.0/django_google_spanner.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-23 13:03:04.000000 django-google-spanner-3.1.0/django_google_spanner.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003      144 2024-04-23 13:03:04.000000 django-google-spanner-3.1.0/django_google_spanner.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003       21 2024-04-23 13:03:04.000000 django-google-spanner-3.1.0/django_google_spanner.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-23 13:03:04.480239 django-google-spanner-3.1.0/django_spanner/
--rw-rw-r--   0 root         (0)     1003     3559 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/__init__.py
--rw-rw-r--   0 root         (0)     1003     1635 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/_opentelemetry_tracing.py
--rw-rw-r--   0 root         (0)     1003     7964 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/base.py
--rw-rw-r--   0 root         (0)     1003      509 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/client.py
--rw-rw-r--   0 root         (0)     1003     5023 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/compiler.py
--rw-rw-r--   0 root         (0)     1003     4197 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/creation.py
--rw-rw-r--   0 root         (0)     1003     1098 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/expressions.py
--rw-rw-r--   0 root         (0)     1003   185105 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/features.py
--rw-rw-r--   0 root         (0)     1003    15053 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/functions.py
--rw-rw-r--   0 root         (0)     1003    13750 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/introspection.py
--rw-rw-r--   0 root         (0)     1003    11510 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/lookups.py
--rw-rw-r--   0 root         (0)     1003    23263 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/operations.py
--rw-rw-r--   0 root         (0)     1003    21797 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/schema.py
--rw-rw-r--   0 root         (0)     1003     1350 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/utils.py
--rw-rw-r--   0 root         (0)     1003       30 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/pyproject.toml
--rw-rw-r--   0 root         (0)     1003      561 2024-04-23 13:03:04.488239 django-google-spanner-3.1.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2321 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-23 13:03:04.476238 django-google-spanner-3.1.0/tests/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-23 13:03:04.480239 django-google-spanner-3.1.0/tests/performance/
--rw-rw-r--   0 root         (0)     1003      194 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/performance/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-23 13:03:04.480239 django-google-spanner-3.1.0/tests/performance/django_spanner/
--rw-rw-r--   0 root         (0)     1003      194 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/performance/django_spanner/__init__.py
--rw-rw-r--   0 root         (0)     1003      443 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/performance/django_spanner/models.py
--rw-rw-r--   0 root         (0)     1003     9090 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/performance/django_spanner/test_benchmark.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-23 13:03:04.480239 django-google-spanner-3.1.0/tests/system/
--rw-rw-r--   0 root         (0)     1003      194 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/system/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-23 13:03:04.484239 django-google-spanner-3.1.0/tests/system/django_spanner/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/system/django_spanner/__init__.py
--rw-rw-r--   0 root         (0)     1003     1021 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/system/django_spanner/models.py
--rw-rw-r--   0 root         (0)     1003     2024 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/system/django_spanner/test_check_constraint.py
--rw-rw-r--   0 root         (0)     1003     3402 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/system/django_spanner/test_decimal.py
--rw-rw-r--   0 root         (0)     1003     1576 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/system/django_spanner/test_json_field.py
--rw-rw-r--   0 root         (0)     1003     1521 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/system/django_spanner/test_queries.py
--rw-rw-r--   0 root         (0)     1003     4193 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/system/django_spanner/utils.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-23 13:03:04.484239 django-google-spanner-3.1.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-23 13:03:04.488239 django-google-spanner-3.1.0/tests/unit/django_spanner/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/__init__.py
--rw-rw-r--   0 root         (0)     1003     1557 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/models.py
--rw-rw-r--   0 root         (0)     1003     1247 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/simple_test.py
--rw-rw-r--   0 root         (0)     1003     4528 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/test__opentelemetry_tracing.py
--rw-rw-r--   0 root         (0)     1003     3372 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/test_base.py
--rw-rw-r--   0 root         (0)     1003      528 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/test_client.py
--rw-rw-r--   0 root         (0)     1003     6961 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/test_compiler.py
--rw-rw-r--   0 root         (0)     1003     1777 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/test_expressions.py
--rw-rw-r--   0 root         (0)     1003     8591 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/test_functions.py
--rw-rw-r--   0 root         (0)     1003     8637 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/test_introspection.py
--rw-rw-r--   0 root         (0)     1003    15614 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/test_lookups.py
--rw-rw-r--   0 root         (0)     1003     8459 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/test_operations.py
--rw-rw-r--   0 root         (0)     1003    16626 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/test_schema.py
--rw-rw-r--   0 root         (0)     1003     1987 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/test_utils.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 08:03:15.858243 django-google-spanner-4.0.1/
+-rw-rw-r--   0 root         (0)     1003     1448 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/LICENSE
+-rw-r--r--   0 root         (0)     1003    10110 2024-05-07 08:03:15.858243 django-google-spanner-4.0.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     8933 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 08:03:15.858243 django-google-spanner-4.0.1/django_google_spanner.egg-info/
+-rw-r--r--   0 root         (0)     1003    10110 2024-05-07 08:03:15.000000 django-google-spanner-4.0.1/django_google_spanner.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1758 2024-05-07 08:03:15.000000 django-google-spanner-4.0.1/django_google_spanner.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-07 08:03:15.000000 django-google-spanner-4.0.1/django_google_spanner.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003      144 2024-05-07 08:03:15.000000 django-google-spanner-4.0.1/django_google_spanner.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003       21 2024-05-07 08:03:15.000000 django-google-spanner-4.0.1/django_google_spanner.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 08:03:15.850242 django-google-spanner-4.0.1/django_spanner/
+-rw-rw-r--   0 root         (0)     1003     3455 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/django_spanner/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1635 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/django_spanner/_opentelemetry_tracing.py
+-rw-rw-r--   0 root         (0)     1003     8276 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/django_spanner/base.py
+-rw-rw-r--   0 root         (0)     1003      509 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/django_spanner/client.py
+-rw-rw-r--   0 root         (0)     1003    10400 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/django_spanner/compiler.py
+-rw-rw-r--   0 root         (0)     1003     4197 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/django_spanner/creation.py
+-rw-rw-r--   0 root         (0)     1003   188727 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/django_spanner/features.py
+-rw-rw-r--   0 root         (0)     1003    15053 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/django_spanner/functions.py
+-rw-rw-r--   0 root         (0)     1003    13178 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/django_spanner/introspection.py
+-rw-rw-r--   0 root         (0)     1003    11510 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/django_spanner/lookups.py
+-rw-rw-r--   0 root         (0)     1003    31149 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/django_spanner/operations.py
+-rw-rw-r--   0 root         (0)     1003    22636 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/django_spanner/schema.py
+-rw-rw-r--   0 root         (0)     1003     1350 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/django_spanner/utils.py
+-rw-rw-r--   0 root         (0)     1003       30 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/pyproject.toml
+-rw-rw-r--   0 root         (0)     1003      561 2024-05-07 08:03:15.858243 django-google-spanner-4.0.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2223 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 08:03:15.842242 django-google-spanner-4.0.1/tests/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 08:03:15.850242 django-google-spanner-4.0.1/tests/performance/
+-rw-rw-r--   0 root         (0)     1003      194 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/tests/performance/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 08:03:15.850242 django-google-spanner-4.0.1/tests/performance/django_spanner/
+-rw-rw-r--   0 root         (0)     1003      194 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/tests/performance/django_spanner/__init__.py
+-rw-rw-r--   0 root         (0)     1003      443 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/tests/performance/django_spanner/models.py
+-rw-rw-r--   0 root         (0)     1003     9090 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/tests/performance/django_spanner/test_benchmark.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 08:03:15.850242 django-google-spanner-4.0.1/tests/system/
+-rw-rw-r--   0 root         (0)     1003      194 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/tests/system/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 08:03:15.850242 django-google-spanner-4.0.1/tests/system/django_spanner/
+-rw-rw-r--   0 root         (0)     1003        0 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/tests/system/django_spanner/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1021 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/tests/system/django_spanner/models.py
+-rw-rw-r--   0 root         (0)     1003     2024 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/tests/system/django_spanner/test_check_constraint.py
+-rw-rw-r--   0 root         (0)     1003     3402 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/tests/system/django_spanner/test_decimal.py
+-rw-rw-r--   0 root         (0)     1003     1576 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/tests/system/django_spanner/test_json_field.py
+-rw-rw-r--   0 root         (0)     1003     1521 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/tests/system/django_spanner/test_queries.py
+-rw-rw-r--   0 root         (0)     1003     4193 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/tests/system/django_spanner/utils.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 08:03:15.854243 django-google-spanner-4.0.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003        0 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 08:03:15.854243 django-google-spanner-4.0.1/tests/unit/django_spanner/
+-rw-rw-r--   0 root         (0)     1003        0 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/tests/unit/django_spanner/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1557 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/tests/unit/django_spanner/models.py
+-rw-rw-r--   0 root         (0)     1003     1247 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/tests/unit/django_spanner/simple_test.py
+-rw-rw-r--   0 root         (0)     1003     4528 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/tests/unit/django_spanner/test__opentelemetry_tracing.py
+-rw-rw-r--   0 root         (0)     1003     3372 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/tests/unit/django_spanner/test_base.py
+-rw-rw-r--   0 root         (0)     1003      528 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/tests/unit/django_spanner/test_client.py
+-rw-rw-r--   0 root         (0)     1003    10021 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/tests/unit/django_spanner/test_compiler.py
+-rw-rw-r--   0 root         (0)     1003     1777 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/tests/unit/django_spanner/test_expressions.py
+-rw-rw-r--   0 root         (0)     1003     8591 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/tests/unit/django_spanner/test_functions.py
+-rw-rw-r--   0 root         (0)     1003     7613 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/tests/unit/django_spanner/test_introspection.py
+-rw-rw-r--   0 root         (0)     1003    15614 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/tests/unit/django_spanner/test_lookups.py
+-rw-rw-r--   0 root         (0)     1003    11688 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/tests/unit/django_spanner/test_operations.py
+-rw-rw-r--   0 root         (0)     1003    16626 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/tests/unit/django_spanner/test_schema.py
+-rw-rw-r--   0 root         (0)     1003     1987 2024-05-07 08:00:39.000000 django-google-spanner-4.0.1/tests/unit/django_spanner/test_utils.py
```

### Comparing `django-google-spanner-3.1.0/LICENSE` & `django-google-spanner-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.1.0/PKG-INFO` & `django-google-spanner-4.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: django-google-spanner
-Version: 3.1.0
+Version: 4.0.1
 Summary: Bridge to enable using Django with Spanner.
 Home-page: https://github.com/googleapis/python-spanner-django
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
-Requires-Python: >=3.6
+Classifier: Framework :: Django :: 4.2
+Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: sqlparse>=0.3.0
 Requires-Dist: google-cloud-spanner>=3.13.0
 Provides-Extra: tracing
 Requires-Dist: opentelemetry-api>=1.1.0; extra == "tracing"
 Requires-Dist: opentelemetry-sdk>=1.1.0; extra == "tracing"
 Requires-Dist: opentelemetry-instrumentation>=0.20b0; extra == "tracing"
@@ -168,14 +166,28 @@
                'ENGINE': 'django_spanner',
                'PROJECT': '$PROJECT',
                'INSTANCE': '$INSTANCE',
                'NAME': '$DATABASE',
            }
        }
 
+Transaction support in autocommit mode
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Django version 4.2 and higher by default supports transactions in autocommit mode.
+A transaction is automatically started if you define an
+[atomic block](https://docs.djangoproject.com/en/4.2/topics/db/transactions/#controlling-transactions-explicitly).
+
+Django version 3.2 and earlier did not support transactions in autocommit mode with Spanner.
+You can enable transactions in autocommit mode with Spanner with the
+`ALLOW_TRANSACTIONS_IN_AUTO_COMMIT` configuration option.
+
+- To enable transactions in autocommit mode in V3.2, set the flag `ALLOW_TRANSACTIONS_IN_AUTO_COMMIT` to True in your settings.py file.
+- To disable transactions in autocommit mode in V4.2, set the flag `ALLOW_TRANSACTIONS_IN_AUTO_COMMIT` to False in your settings.py file.
+
 
 Set credentials and project environment variables
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 You'll need to download a service account JSON key file and point to it using an environment variable:
 
 .. code:: shell
```

### Comparing `django-google-spanner-3.1.0/README.rst` & `django-google-spanner-4.0.1/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -136,14 +136,28 @@
                'ENGINE': 'django_spanner',
                'PROJECT': '$PROJECT',
                'INSTANCE': '$INSTANCE',
                'NAME': '$DATABASE',
            }
        }
 
+Transaction support in autocommit mode
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Django version 4.2 and higher by default supports transactions in autocommit mode.
+A transaction is automatically started if you define an
+[atomic block](https://docs.djangoproject.com/en/4.2/topics/db/transactions/#controlling-transactions-explicitly).
+
+Django version 3.2 and earlier did not support transactions in autocommit mode with Spanner.
+You can enable transactions in autocommit mode with Spanner with the
+`ALLOW_TRANSACTIONS_IN_AUTO_COMMIT` configuration option.
+
+- To enable transactions in autocommit mode in V3.2, set the flag `ALLOW_TRANSACTIONS_IN_AUTO_COMMIT` to True in your settings.py file.
+- To disable transactions in autocommit mode in V4.2, set the flag `ALLOW_TRANSACTIONS_IN_AUTO_COMMIT` to False in your settings.py file.
+
 
 Set credentials and project environment variables
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 You'll need to download a service account JSON key file and point to it using an environment variable:
 
 .. code:: shell
```

### Comparing `django-google-spanner-3.1.0/django_google_spanner.egg-info/PKG-INFO` & `django-google-spanner-4.0.1/django_google_spanner.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: django-google-spanner
-Version: 3.1.0
+Version: 4.0.1
 Summary: Bridge to enable using Django with Spanner.
 Home-page: https://github.com/googleapis/python-spanner-django
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
-Requires-Python: >=3.6
+Classifier: Framework :: Django :: 4.2
+Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: sqlparse>=0.3.0
 Requires-Dist: google-cloud-spanner>=3.13.0
 Provides-Extra: tracing
 Requires-Dist: opentelemetry-api>=1.1.0; extra == "tracing"
 Requires-Dist: opentelemetry-sdk>=1.1.0; extra == "tracing"
 Requires-Dist: opentelemetry-instrumentation>=0.20b0; extra == "tracing"
@@ -168,14 +166,28 @@
                'ENGINE': 'django_spanner',
                'PROJECT': '$PROJECT',
                'INSTANCE': '$INSTANCE',
                'NAME': '$DATABASE',
            }
        }
 
+Transaction support in autocommit mode
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Django version 4.2 and higher by default supports transactions in autocommit mode.
+A transaction is automatically started if you define an
+[atomic block](https://docs.djangoproject.com/en/4.2/topics/db/transactions/#controlling-transactions-explicitly).
+
+Django version 3.2 and earlier did not support transactions in autocommit mode with Spanner.
+You can enable transactions in autocommit mode with Spanner with the
+`ALLOW_TRANSACTIONS_IN_AUTO_COMMIT` configuration option.
+
+- To enable transactions in autocommit mode in V3.2, set the flag `ALLOW_TRANSACTIONS_IN_AUTO_COMMIT` to True in your settings.py file.
+- To disable transactions in autocommit mode in V4.2, set the flag `ALLOW_TRANSACTIONS_IN_AUTO_COMMIT` to False in your settings.py file.
+
 
 Set credentials and project environment variables
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 You'll need to download a service account JSON key file and point to it using an environment variable:
 
 .. code:: shell
```

### Comparing `django-google-spanner-3.1.0/django_google_spanner.egg-info/SOURCES.txt` & `django-google-spanner-4.0.1/django_google_spanner.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 django_google_spanner.egg-info/top_level.txt
 django_spanner/__init__.py
 django_spanner/_opentelemetry_tracing.py
 django_spanner/base.py
 django_spanner/client.py
 django_spanner/compiler.py
 django_spanner/creation.py
-django_spanner/expressions.py
 django_spanner/features.py
 django_spanner/functions.py
 django_spanner/introspection.py
 django_spanner/lookups.py
 django_spanner/operations.py
 django_spanner/schema.py
 django_spanner/utils.py
```

### Comparing `django-google-spanner-3.1.0/django_spanner/__init__.py` & `django-google-spanner-4.0.1/django_spanner/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,44 +16,45 @@
 from google.cloud.spanner_v1 import JsonObject
 from django.db.models.fields import (
     NOT_PROVIDED,
     AutoField,
     Field,
 )
 
-from .expressions import register_expressions
 from .functions import register_functions
 from .lookups import register_lookups
 from .utils import check_django_compatability
 
 # Monkey-patch google.DatetimeWithNanoseconds's __eq__ compare against
 # datetime.datetime.
 from google.api_core.datetime_helpers import DatetimeWithNanoseconds
 
 
 USING_DJANGO_3 = False
 if django.VERSION[:2] == (3, 2):
     USING_DJANGO_3 = True
 
-if USING_DJANGO_3:
-    from django.db.models.fields import (
-        SmallAutoField,
-        BigAutoField,
-    )
-    from django.db.models import JSONField
+USING_DJANGO_4 = False
+if django.VERSION[:2] == (4, 2):
+    USING_DJANGO_4 = True
+
+from django.db.models.fields import (
+    SmallAutoField,
+    BigAutoField,
+)
+from django.db.models import JSONField
 
 __version__ = pkg_resources.get_distribution("django-google-spanner").version
 
 USE_EMULATOR = os.getenv("SPANNER_EMULATOR_HOST") is not None
 
-# Only active LTS django versions (2.2.*, 3.2.*) are supported by this library right now.
-SUPPORTED_DJANGO_VERSIONS = [(2, 2), (3, 2)]
+# Only active LTS django versions (3.2.*, 4.2.*) are supported by this library right now.
+SUPPORTED_DJANGO_VERSIONS = [(3, 2), (4, 2)]
 
 check_django_compatability(SUPPORTED_DJANGO_VERSIONS)
-register_expressions(USING_DJANGO_3)
 register_functions()
 register_lookups()
 
 
 def gen_rand_int64():
     # Credit to https://stackoverflow.com/a/3530326.
     return uuid4().int & 0x7FFFFFFFFFFFFFFF
@@ -69,31 +70,32 @@
     ):
         self.default = gen_rand_int64
 
 
 AutoField.__init__ = autofield_init
 AutoField.db_returning = False
 AutoField.validators = []
-if USING_DJANGO_3:
-    SmallAutoField.__init__ = autofield_init
-    BigAutoField.__init__ = autofield_init
-    SmallAutoField.db_returning = False
-    BigAutoField.db_returning = False
-    SmallAutoField.validators = []
-    BigAutoField.validators = []
-
-    def get_prep_value(self, value):
-        # Json encoding and decoding for spanner is done in python-spanner.
-        if not isinstance(value, JsonObject) and isinstance(value, dict):
-            return JsonObject(value)
 
-        return value
+SmallAutoField.__init__ = autofield_init
+BigAutoField.__init__ = autofield_init
+SmallAutoField.db_returning = False
+BigAutoField.db_returning = False
+SmallAutoField.validators = []
+BigAutoField.validators = []
+
+
+def get_prep_value(self, value):
+    # Json encoding and decoding for spanner is done in python-spanner.
+    if not isinstance(value, JsonObject) and isinstance(value, dict):
+        return JsonObject(value)
+
+    return value
 
-    JSONField.get_prep_value = get_prep_value
 
+JSONField.get_prep_value = get_prep_value
 
 old_datetimewithnanoseconds_eq = getattr(
     DatetimeWithNanoseconds, "__eq__", None
 )
 
 
 def datetimewithnanoseconds_eq(self, other):
```

### Comparing `django-google-spanner-3.1.0/django_spanner/_opentelemetry_tracing.py` & `django-google-spanner-4.0.1/django_spanner/_opentelemetry_tracing.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.1.0/django_spanner/base.py` & `django-google-spanner-4.0.1/django_spanner/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from .client import DatabaseClient
 from .creation import DatabaseCreation
 from .features import DatabaseFeatures
 from .introspection import DatabaseIntrospection
 from .operations import DatabaseOperations
 from .schema import DatabaseSchemaEditor
+from django_spanner import USING_DJANGO_3
 
 
 class DatabaseWrapper(BaseDatabaseWrapper):
     vendor = "spanner"
     display_name = "Cloud Spanner"
 
     # Mapping of Field objects to their column types.
@@ -120,14 +121,23 @@
         :returns: A new instance owned by the existing Spanner Client.
         """
         return spanner.Client(
             project=os.environ["GOOGLE_CLOUD_PROJECT"]
         ).instance(self.settings_dict["INSTANCE"])
 
     @property
+    def allow_transactions_in_auto_commit(self):
+        if "ALLOW_TRANSACTIONS_IN_AUTO_COMMIT" in self.settings_dict:
+            return self.settings_dict["ALLOW_TRANSACTIONS_IN_AUTO_COMMIT"]
+        if USING_DJANGO_3:
+            return False
+        else:
+            return True
+
+    @property
     def _nodb_connection(self):
         raise NotImplementedError(
             'Spanner does not have a "no db" connection.'
         )
 
     def get_connection_params(self):
         """Retrieve the connection parameters.
@@ -201,19 +211,18 @@
             # Use a cursor directly, bypassing Django's utilities.
             self.connection.cursor().execute("SELECT 1")
         except self.Database.Error:
             return False
 
         return True
 
-    # The usual way to start a transaction is to turn autocommit off.
-    # Spanner DB API does not properly start a transaction when disabling
-    # autocommit. To avoid this buggy behavior and to actually enter a new
-    # transaction, an explicit SELECT 1 is required.
     def _start_transaction_under_autocommit(self):
         """
         Start a transaction explicitly in autocommit mode.
-
-        Staying in autocommit mode works around a bug that breaks
-        save points when autocommit is disabled by django.
         """
-        self.connection.cursor().execute("SELECT 1")
+        if self.allow_transactions_in_auto_commit:
+            self.connection.cursor().execute("BEGIN")
+        else:
+            # This won't start a transaction and was a bug in Spanner Django 3.2 version.
+            # Set ALLOW_TRANSACTIONS_IN_AUTO_COMMIT = True in your settings.py file to enable
+            # transactions in autocommit mode for Django 3.2.
+            self.connection.cursor().execute("SELECT 1")
```

### Comparing `django-google-spanner-3.1.0/django_spanner/creation.py` & `django-google-spanner-4.0.1/django_spanner/creation.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.1.0/django_spanner/features.py` & `django-google-spanner-4.0.1/django_spanner/features.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # license that can be found in the LICENSE file or at
 # https://developers.google.com/open-source/licenses/bsd
 
 import os
 
 from django.db.backends.base.features import BaseDatabaseFeatures
 from django.db.utils import InterfaceError
-from django_spanner import USE_EMULATOR, USING_DJANGO_3
+from django_spanner import USE_EMULATOR, USING_DJANGO_3, USING_DJANGO_4
 
 
 class DatabaseFeatures(BaseDatabaseFeatures):
     can_introspect_big_integer_field = False
     can_introspect_duration_field = False
     can_introspect_foreign_keys = False
     # TimeField is introspected as DateTimeField because they both use
@@ -40,24 +40,18 @@
         supports_json_field = False
         # Emulator does not support check constrints.
         supports_column_check_constraints = False
         supports_table_check_constraints = False
     else:
         supports_column_check_constraints = True
         supports_table_check_constraints = True
-        if USING_DJANGO_3:
-            supports_json_field = True
-        else:
-            # Since JsonField was introduced in django3.1 we don't support it for django 2.2
-            supports_json_field = False
+        supports_json_field = True
     supports_primitives_in_json_field = False
     # Spanner does not support order by null modifiers.
-    # For Django 2.2 this feature is handled in code.
-    if USING_DJANGO_3:
-        supports_order_by_nulls_modifier = False
+    supports_order_by_nulls_modifier = False
     # Spanner does not support SELECTing an arbitrary expression that also
     # appears in the GROUP BY clause.
     supports_subqueries_in_group_by = False
     uses_savepoints = False
     # Spanner does not support expression indexes
     # example: CREATE INDEX index_name ON table (LOWER(column_name))
     supports_expression_indexes = False
@@ -76,16 +70,14 @@
         "basic.tests.ModelTest.test_hash",
         "custom_managers.tests.CustomManagerTests.test_slow_removal_through_specified_fk_related_manager",
         "custom_managers.tests.CustomManagerTests.test_slow_removal_through_default_fk_related_manager",
         "generic_relations.test_forms.GenericInlineFormsetTests.test_options",
         "generic_relations.tests.GenericRelationsTests.test_add_bulk_false",
         "generic_relations.tests.GenericRelationsTests.test_generic_update_or_create_when_updated",
         "generic_relations.tests.GenericRelationsTests.test_update_or_create_defaults",
-        "generic_relations.tests.GenericRelationsTests.test_unsaved_instance_on_generic_foreign_key",
-        "generic_relations_regress.tests.GenericRelationTests.test_target_model_is_unsaved",
         "m2m_through_regress.tests.ToFieldThroughTests.test_m2m_relations_unusable_on_null_pk_obj",
         "many_to_many.tests.ManyToManyTests.test_add",
         "many_to_one.tests.ManyToOneTests.test_fk_assignment_and_related_object_cache",
         "many_to_one.tests.ManyToOneTests.test_relation_unsaved",
         "model_fields.test_durationfield.TestSerialization.test_dumping",
         "model_fields.test_uuid.TestSerialization.test_dumping",
         "model_fields.test_booleanfield.ValidationTest.test_nullbooleanfield_blank",
@@ -156,15 +148,14 @@
         "admin_views.tests.AdminViewPermissionsTest.test_history_view",
         "aggregation.test_filter_argument.FilteredAggregateTests.test_plain_annotate",
         "aggregation.tests.AggregateTestCase.test_annotate_basic",
         "aggregation.tests.AggregateTestCase.test_annotation",
         "aggregation.tests.AggregateTestCase.test_filtering",
         "aggregation_regress.tests.AggregationTests.test_more_more",
         "aggregation_regress.tests.AggregationTests.test_more_more_more",
-        "aggregation_regress.tests.AggregationTests.test_ticket_11293",
         "defer_regress.tests.DeferRegressionTest.test_ticket_12163",
         "defer_regress.tests.DeferRegressionTest.test_ticket_23270",
         "distinct_on_fields.tests.DistinctOnTests.test_basic_distinct_on",
         "extra_regress.tests.ExtraRegressTests.test_regression_7314_7372",
         "generic_relations_regress.tests.GenericRelationTests.test_annotate",
         "get_earliest_or_latest.tests.TestFirstLast",
         "known_related_objects.tests.ExistingRelatedInstancesTests.test_reverse_one_to_one_multi_prefetch_related",
@@ -374,129 +365,203 @@
         "model_forms.tests.ModelFormBaseTest.test_exclude_and_validation",
         "model_forms.tests.UniqueTest.test_unique_together",
         "model_forms.tests.UniqueTest.test_override_unique_together_message",
         # os.chmod() doesn't work on Kokoro?
         "file_uploads.tests.DirectoryCreationTests.test_readonly_root",
         # Failing on kokoro but passes locally. Issue: Multiple queries executed expected 1.
         "contenttypes_tests.test_models.ContentTypesTests.test_cache_not_shared_between_managers",
+        # Spanner does not support UUID field natively
+        "model_fields.test_uuid.TestQuerying.test_iexact",
+        # Spanner does not support very long FK name: 400 Foreign Key name not valid
+        "backends.tests.FkConstraintsTests.test_check_constraints_sql_keywords",
+        # Spanner does not support setting a default value on columns.
+        "schema.tests.SchemaTests.test_alter_text_field_to_not_null_with_default_value",
+        # Direct SQL query test that do not follow spanner syntax.
+        "schema.tests.SchemaTests.test_alter_auto_field_quoted_db_column",
+        "schema.tests.SchemaTests.test_alter_primary_key_quoted_db_table",
+        # Insert sql with param variables using %(name)s parameter style is failing
+        # https://github.com/googleapis/python-spanner/issues/542
+        "backends.tests.LastExecutedQueryTest.test_last_executed_query_dict",
+        # Spanner autofield is replaced with uuid4 so validation is disabled
+        "model_fields.test_autofield.AutoFieldTests.test_backend_range_validation",
+        "model_fields.test_autofield.AutoFieldTests.test_redundant_backend_range_validators",
+        "model_fields.test_autofield.AutoFieldTests.test_redundant_backend_range_validators",
+        "model_fields.test_autofield.BigAutoFieldTests.test_backend_range_validation",
+        "model_fields.test_autofield.BigAutoFieldTests.test_redundant_backend_range_validators",
+        "model_fields.test_autofield.BigAutoFieldTests.test_redundant_backend_range_validators",
+        "model_fields.test_autofield.SmallAutoFieldTests.test_backend_range_validation",
+        "model_fields.test_autofield.SmallAutoFieldTests.test_redundant_backend_range_validators",
+        "model_fields.test_autofield.SmallAutoFieldTests.test_redundant_backend_range_validators",
+        # Spanner does not support deferred unique constraints
+        "migrations.test_operations.OperationTests.test_create_model_with_deferred_unique_constraint",
+        # Spanner does not support JSON object query on fields.
+        "db_functions.comparison.test_json_object.JSONObjectTests.test_empty",
+        "db_functions.comparison.test_json_object.JSONObjectTests.test_basic",
+        "db_functions.comparison.test_json_object.JSONObjectTests.test_expressions",
+        "db_functions.comparison.test_json_object.JSONObjectTests.test_nested_empty_json_object",
+        "db_functions.comparison.test_json_object.JSONObjectTests.test_nested_json_object",
+        "db_functions.comparison.test_json_object.JSONObjectTests.test_textfield",
+        # Spanner does not support iso_week_day but week_day is supported.
+        "timezones.tests.LegacyDatabaseTests.test_query_datetime_lookups",
+        "timezones.tests.NewDatabaseTests.test_query_datetime_lookups",
+        "timezones.tests.NewDatabaseTests.test_query_datetime_lookups_in_other_timezone",
+        "db_functions.datetime.test_extract_trunc.DateFunctionTests.test_extract_func",
+        "db_functions.datetime.test_extract_trunc.DateFunctionTests.test_extract_iso_weekday_func",
+        "db_functions.datetime.test_extract_trunc.DateFunctionWithTimeZoneTests.test_extract_func",
+        "db_functions.datetime.test_extract_trunc.DateFunctionWithTimeZoneTests.test_extract_func_with_timezone",
+        "db_functions.datetime.test_extract_trunc.DateFunctionWithTimeZoneTests.test_extract_func_with_timezone",
+        "db_functions.datetime.test_extract_trunc.DateFunctionWithTimeZoneTests.test_extract_iso_weekday_func",
+        # Spanner gived SHA encryption output in bytes, django expects it in hex string format.
+        "db_functions.text.test_sha512.SHA512Tests.test_basic",
+        "db_functions.text.test_sha512.SHA512Tests.test_transform",
+        "db_functions.text.test_md5.MD5Tests.test_basic",
+        "db_functions.text.test_md5.MD5Tests.test_transform",
+        "db_functions.text.test_sha1.SHA1Tests.test_basic",
+        "db_functions.text.test_sha1.SHA1Tests.test_transform",
+        "db_functions.text.test_sha224.SHA224Tests.test_basic",
+        "db_functions.text.test_sha224.SHA224Tests.test_transform",
+        "db_functions.text.test_sha256.SHA256Tests.test_basic",
+        "db_functions.text.test_sha256.SHA256Tests.test_transform",
+        "db_functions.text.test_sha384.SHA384Tests.test_basic",
+        "db_functions.text.test_sha384.SHA384Tests.test_transform",
+        # Spanner does not support RANDOM number generation function
+        "db_functions.math.test_random.RandomTests.test",
+        # Spanner supports order by id, but it's does not work the same way as
+        # an auto increment field.
+        "model_forms.test_modelchoicefield.ModelChoiceFieldTests.test_choice_iterator_passes_model_to_widget",
+        "queries.test_qs_combinators.QuerySetSetOperationTests.test_union_with_values_list_and_order",
+        "ordering.tests.OrderingTests.test_order_by_self_referential_fk",
+        "fixtures.tests.ForwardReferenceTests.test_forward_reference_m2m_natural_key",
+        "fixtures.tests.ForwardReferenceTests.test_forward_reference_fk_natural_key",
+        # Spanner does not support empty list of DML statement.
+        "backends.tests.BackendTestCase.test_cursor_executemany_with_empty_params_list",
+        # Spanner does not support SELECTing an arbitrary expression that also
+        # appears in the GROUP BY clause.
+        "annotations.tests.NonAggregateAnnotationTestCase.test_grouping_by_q_expression_annotation",
+        # Tests that expect it to be empty untill saved in db.
+        "test_utils.test_testcase.TestDataTests.test_class_attribute_identity",
+        "model_fields.test_jsonfield.TestSerialization.test_dumping",
+        "model_fields.test_jsonfield.TestSerialization.test_dumping",
+        "model_fields.test_jsonfield.TestSerialization.test_dumping",
+        "model_fields.test_jsonfield.TestSerialization.test_xml_serialization",
+        "model_fields.test_jsonfield.TestSerialization.test_xml_serialization",
+        "model_fields.test_jsonfield.TestSerialization.test_xml_serialization",
+        "bulk_create.tests.BulkCreateTests.test_unsaved_parent",
+        # Tests that assume a serial pk.
+        "lookup.tests.LookupTests.test_exact_query_rhs_with_selected_columns",
+        "prefetch_related.tests.DirectPrefetchedObjectCacheReuseTests.test_detect_is_fetched",
+        "prefetch_related.tests.DirectPrefetchedObjectCacheReuseTests.test_detect_is_fetched_with_to_attr",
+        # datetimes retrieved from the database with the wrong hour when
+        # USE_TZ = True: https://github.com/googleapis/python-spanner-django/issues/193
+        "timezones.tests.NewDatabaseTests.test_query_convert_timezones",
+        # Spanner doesn't support random ordering.
+        "aggregation.tests.AggregateTestCase.test_aggregation_random_ordering",
+        # Tests that require transactions.
+        "test_utils.tests.CaptureOnCommitCallbacksTests.test_execute",
+        "test_utils.tests.CaptureOnCommitCallbacksTests.test_no_arguments",
+        "test_utils.tests.CaptureOnCommitCallbacksTests.test_pre_callback",
+        "test_utils.tests.CaptureOnCommitCallbacksTests.test_using",
+        # Field: GenericIPAddressField is mapped to String in Spanner
+        "inspectdb.tests.InspectDBTestCase.test_field_types",
+        # BigIntegerField is mapped to IntegerField in Spanner
+        "inspectdb.tests.InspectDBTestCase.test_number_field_types",
+        # Spanner limitation: Cannot change type of column.
+        "schema.tests.SchemaTests.test_char_field_pk_to_auto_field",
+        "schema.tests.SchemaTests.test_ci_cs_db_collation",
+        # Spanner limitation: Cannot rename tables and columns.
+        "migrations.test_operations.OperationTests.test_rename_field_case",
     )
     if USING_DJANGO_3:
         skip_tests += (
-            # Spanner does not support UUID field natively
-            "model_fields.test_uuid.TestQuerying.test_iexact",
-            # Spanner does not support very long FK name: 400 Foreign Key name not valid
-            "backends.tests.FkConstraintsTests.test_check_constraints_sql_keywords",
-            # Spanner does not support setting a default value on columns.
-            "schema.tests.SchemaTests.test_alter_text_field_to_not_null_with_default_value",
-            # Direct SQL query test that do not follow spanner syntax.
-            "schema.tests.SchemaTests.test_alter_auto_field_quoted_db_column",
-            "schema.tests.SchemaTests.test_alter_primary_key_quoted_db_table",
-            # Insert sql with param variables using %(name)s parameter style is failing
-            # https://github.com/googleapis/python-spanner/issues/542
-            "backends.tests.LastExecutedQueryTest.test_last_executed_query_dict",
-            # Spanner autofield is replaced with uuid4 so validation is disabled
-            "model_fields.test_autofield.AutoFieldTests.test_backend_range_validation",
-            "model_fields.test_autofield.AutoFieldTests.test_redundant_backend_range_validators",
-            "model_fields.test_autofield.AutoFieldTests.test_redundant_backend_range_validators",
-            "model_fields.test_autofield.BigAutoFieldTests.test_backend_range_validation",
-            "model_fields.test_autofield.BigAutoFieldTests.test_redundant_backend_range_validators",
-            "model_fields.test_autofield.BigAutoFieldTests.test_redundant_backend_range_validators",
-            "model_fields.test_autofield.SmallAutoFieldTests.test_backend_range_validation",
-            "model_fields.test_autofield.SmallAutoFieldTests.test_redundant_backend_range_validators",
-            "model_fields.test_autofield.SmallAutoFieldTests.test_redundant_backend_range_validators",
-            # Spanner does not support deferred unique constraints
-            "migrations.test_operations.OperationTests.test_create_model_with_deferred_unique_constraint",
-            # Spanner does not support JSON object query on fields.
-            "db_functions.comparison.test_json_object.JSONObjectTests.test_empty",
-            "db_functions.comparison.test_json_object.JSONObjectTests.test_basic",
-            "db_functions.comparison.test_json_object.JSONObjectTests.test_expressions",
-            "db_functions.comparison.test_json_object.JSONObjectTests.test_nested_empty_json_object",
-            "db_functions.comparison.test_json_object.JSONObjectTests.test_nested_json_object",
-            "db_functions.comparison.test_json_object.JSONObjectTests.test_textfield",
-            # Spanner does not support iso_week_day but week_day is supported.
-            "timezones.tests.LegacyDatabaseTests.test_query_datetime_lookups",
-            "timezones.tests.NewDatabaseTests.test_query_datetime_lookups",
-            "timezones.tests.NewDatabaseTests.test_query_datetime_lookups_in_other_timezone",
-            "db_functions.datetime.test_extract_trunc.DateFunctionTests.test_extract_func",
-            "db_functions.datetime.test_extract_trunc.DateFunctionTests.test_extract_iso_weekday_func",
-            "db_functions.datetime.test_extract_trunc.DateFunctionWithTimeZoneTests.test_extract_func",
-            "db_functions.datetime.test_extract_trunc.DateFunctionWithTimeZoneTests.test_extract_func_with_timezone",
-            "db_functions.datetime.test_extract_trunc.DateFunctionWithTimeZoneTests.test_extract_func_with_timezone",
-            "db_functions.datetime.test_extract_trunc.DateFunctionWithTimeZoneTests.test_extract_iso_weekday_func",
-            # Spanner gived SHA encryption output in bytes, django expects it in hex string format.
-            "db_functions.text.test_sha512.SHA512Tests.test_basic",
-            "db_functions.text.test_sha512.SHA512Tests.test_transform",
-            "db_functions.text.test_md5.MD5Tests.test_basic",
-            "db_functions.text.test_md5.MD5Tests.test_transform",
-            "db_functions.text.test_sha1.SHA1Tests.test_basic",
-            "db_functions.text.test_sha1.SHA1Tests.test_transform",
-            "db_functions.text.test_sha224.SHA224Tests.test_basic",
-            "db_functions.text.test_sha224.SHA224Tests.test_transform",
-            "db_functions.text.test_sha256.SHA256Tests.test_basic",
-            "db_functions.text.test_sha256.SHA256Tests.test_transform",
-            "db_functions.text.test_sha384.SHA384Tests.test_basic",
-            "db_functions.text.test_sha384.SHA384Tests.test_transform",
-            # Spanner does not support RANDOM number generation function
-            "db_functions.math.test_random.RandomTests.test",
-            # Spanner supports order by id, but it's does not work the same way as
-            # an auto increment field.
-            "model_forms.test_modelchoicefield.ModelChoiceFieldTests.test_choice_iterator_passes_model_to_widget",
-            "queries.test_qs_combinators.QuerySetSetOperationTests.test_union_with_values_list_and_order",
-            "ordering.tests.OrderingTests.test_order_by_self_referential_fk",
-            "fixtures.tests.ForwardReferenceTests.test_forward_reference_m2m_natural_key",
-            "fixtures.tests.ForwardReferenceTests.test_forward_reference_fk_natural_key",
-            # Spanner does not support empty list of DML statement.
-            "backends.tests.BackendTestCase.test_cursor_executemany_with_empty_params_list",
-            # Spanner does not support SELECTing an arbitrary expression that also
-            # appears in the GROUP BY clause.
-            "annotations.tests.NonAggregateAnnotationTestCase.test_grouping_by_q_expression_annotation",
             # No Django transaction management in Spanner.
             "transactions.tests.DisableDurabiltityCheckTests.test_nested_both_durable",
             "transactions.tests.DisableDurabiltityCheckTests.test_nested_inner_durable",
-            # Tests that expect it to be empty untill saved in db.
-            "test_utils.test_testcase.TestDataTests.test_class_attribute_identity",
-            "model_fields.test_jsonfield.TestSerialization.test_dumping",
-            "model_fields.test_jsonfield.TestSerialization.test_dumping",
-            "model_fields.test_jsonfield.TestSerialization.test_dumping",
-            "model_fields.test_jsonfield.TestSerialization.test_xml_serialization",
-            "model_fields.test_jsonfield.TestSerialization.test_xml_serialization",
-            "model_fields.test_jsonfield.TestSerialization.test_xml_serialization",
-            "bulk_create.tests.BulkCreateTests.test_unsaved_parent",
-            # Tests that assume a serial pk.
-            "lookup.tests.LookupTests.test_exact_query_rhs_with_selected_columns",
-            "prefetch_related.tests.DirectPrefetchedObjectCacheReuseTests.test_detect_is_fetched",
-            "prefetch_related.tests.DirectPrefetchedObjectCacheReuseTests.test_detect_is_fetched_with_to_attr",
-            # datetimes retrieved from the database with the wrong hour when
-            # USE_TZ = True: https://github.com/googleapis/python-spanner-django/issues/193
-            "timezones.tests.NewDatabaseTests.test_query_convert_timezones",
-            # Spanner doesn't support random ordering.
-            "aggregation.tests.AggregateTestCase.test_aggregation_random_ordering",
-            # Tests that require transactions.
-            "test_utils.tests.CaptureOnCommitCallbacksTests.test_execute",
-            "test_utils.tests.CaptureOnCommitCallbacksTests.test_no_arguments",
-            "test_utils.tests.CaptureOnCommitCallbacksTests.test_pre_callback",
-            "test_utils.tests.CaptureOnCommitCallbacksTests.test_using",
-            # Field: GenericIPAddressField is mapped to String in Spanner
-            "inspectdb.tests.InspectDBTestCase.test_field_types",
-            # BigIntegerField is mapped to IntegerField in Spanner
-            "inspectdb.tests.InspectDBTestCase.test_number_field_types",
-            # Spanner limitation: Cannot change type of column.
-            "schema.tests.SchemaTests.test_char_field_pk_to_auto_field",
-            "schema.tests.SchemaTests.test_ci_cs_db_collation",
-            # Spanner limitation: Cannot rename tables and columns.
-            "migrations.test_operations.OperationTests.test_rename_field_case",
+            "generic_relations.tests.GenericRelationsTests.test_unsaved_instance_on_generic_foreign_key",
+            "generic_relations_regress.tests.GenericRelationTests.test_target_model_is_unsaved",
+            "aggregation_regress.tests.AggregationTests.test_ticket_11293",
             # Warning is not raised, not related to spanner.
             "test_utils.test_testcase.TestDataTests.test_undeepcopyable_warning",
         )
-    else:
-        # Tests specific to django 2.2
+    if USING_DJANGO_4:
         skip_tests += (
-            # Tests that assume a serial pk.
-            "prefetch_related.tests.DirectPrefechedObjectCacheReuseTests.test_detect_is_fetched",
-            "prefetch_related.tests.DirectPrefechedObjectCacheReuseTests.test_detect_is_fetched_with_to_attr",
+            "aggregation.tests.AggregateTestCase.test_aggregation_default_expression",
+            "aggregation.tests.AggregateTestCase.test_aggregation_default_integer",
+            "aggregation.tests.AggregateTestCase.test_aggregation_default_unset",
+            "aggregation.tests.AggregateTestCase.test_aggregation_default_using_duration_from_database",
+            "aggregation.tests.AggregateTestCase.test_aggregation_default_zero",
+            "aggregation.tests.AggregateTestCase.test_group_by_nested_expression_with_params",
+            "many_to_one_null.tests.ManyToOneNullTests.test_unsaved",
+            "model_formsets.tests.ModelFormsetTest.test_edit_only_object_outside_of_queryset",
+            "ordering.tests.OrderingTests.test_order_by_expression_ref",
+            "sitemaps_tests.test_http.HTTPSitemapTests.test_alternate_language_for_item_i18n_sitemap",
+            "sitemaps_tests.test_http.HTTPSitemapTests.test_language_for_item_i18n_sitemap",
+            "null_queries.tests.NullQueriesTests.test_unsaved",
+            "prefetch_related.tests.GenericRelationTests.test_deleted_GFK",
+            "aggregation_regress.tests.AggregationTests.test_aggregate_and_annotate_duplicate_columns_proxy",
+            "aggregation_regress.tests.AggregationTests.test_annotation_disjunction",
+            "aggregation_regress.tests.AggregationTests.test_filter_aggregates_negated_and_connector",
+            "aggregation_regress.tests.AggregationTests.test_filter_aggregates_negated_xor_connector",
+            "aggregation_regress.tests.AggregationTests.test_filter_aggregates_or_connector",
+            "aggregation_regress.tests.AggregationTests.test_filter_aggregates_xor_connector",
+            "aggregation_regress.tests.AggregationTests.test_aggregate_and_annotate_duplicate_columns_unmanaged",
+            "queries.test_bulk_update.BulkUpdateTests.test_unsaved_parent",
+            "queries.test_q.QCheckTests.test_basic",
+            "queries.test_q.QCheckTests.test_boolean_expression",
+            "queries.test_q.QCheckTests.test_expression",
+            "queries.tests.ExcludeTests.test_exclude_unsaved_o2o_object",
+            "queries.tests.ExcludeTests.test_exclude_unsaved_object",
+            "queries.tests.Queries5Tests.test_filter_unsaved_object",
+            "queries.tests.QuerySetBitwiseOperationTests.test_xor_with_both_slice",
+            "queries.tests.QuerySetBitwiseOperationTests.test_xor_with_lhs_slice",
+            "queries.tests.QuerySetBitwiseOperationTests.test_xor_with_rhs_slice",
+            "queries.tests.QuerySetBitwiseOperationTests.test_xor_with_both_slice_and_ordering",
+            "queries.tests.Queries1Tests.test_filter_by_related_field_transform",
+            "known_related_objects.tests.ExistingRelatedInstancesTests.test_reverse_fk_select_related_multiple",
+            "known_related_objects.tests.ExistingRelatedInstancesTests.test_multilevel_reverse_fk_select_related",
+            "timezones.tests.NewDatabaseTests.test_aware_time_unsupported",
+            "contenttypes_tests.test_models.ContentTypesTests.test_app_labeled_name",
+            "db_functions.datetime.test_extract_trunc.DateFunctionTests.test_extract_lookup_name_sql_injection",
+            "db_functions.datetime.test_extract_trunc.DateFunctionTests.test_trunc_lookup_name_sql_injection",
+            "db_functions.datetime.test_extract_trunc.DateFunctionWithTimeZoneTests.test_extract_lookup_name_sql_injection",
+            "db_functions.datetime.test_extract_trunc.DateFunctionWithTimeZoneTests.test_trunc_lookup_name_sql_injection",
+            "db_functions.datetime.test_extract_trunc.DateFunctionWithTimeZoneTests.test_trunc_ambiguous_and_invalid_times",
+            "custom_pk.tests.CustomPKTests.test_auto_field_subclass_create",
+            "constraints.tests.UniqueConstraintTests.test_validate_expression_condition",
+            "constraints.tests.CheckConstraintTests.test_validate",
+            "constraints.tests.CheckConstraintTests.test_validate_boolean_expressions",
+            "schema.tests.SchemaTests.test_add_auto_field",
+            "schema.tests.SchemaTests.test_alter_null_with_default_value_deferred_constraints",
+            "schema.tests.SchemaTests.test_autofield_to_o2o",
+            "backends.tests.BackendTestCase.test_queries_bare_where",
+            "expressions.tests.ExpressionOperatorTests.test_lefthand_bitwise_xor_right_null",
+            "expressions.tests.FTimeDeltaTests.test_durationfield_multiply_divide",
+            "inspectdb.tests.InspectDBTestCase.test_same_relations",
+            "migrations.test_operations.OperationTests.test_alter_field_pk_fk_char_to_int",
+            "migrations.test_operations.OperationTests.test_alter_field_with_func_unique_constraint",
+            "migrations.test_operations.OperationTests.test_alter_model_table_m2m_field",
+            "migrations.test_operations.OperationTests.test_remove_unique_together_on_unique_field",
+            "migrations.test_operations.OperationTests.test_rename_field_index_together",
+            "migrations.test_operations.OperationTests.test_rename_field_unique_together",
+            "migrations.test_operations.OperationTests.test_rename_model_with_db_table_rename_m2m",
+            "migrations.test_operations.OperationTests.test_rename_model_with_m2m_models_in_different_apps_with_same_name",
+            "delete.tests.DeletionTests.test_pk_none",
+            "db_functions.datetime.test_extract_trunc.DateFunctionTests.test_trunc_time_comparison",
+            "db_functions.datetime.test_extract_trunc.DateFunctionWithTimeZoneTests.test_trunc_time_comparison",
+            "backends.tests.LastExecutedQueryTest.test_last_executed_query_dict_overlap_keys",
+            "backends.tests.LastExecutedQueryTest.test_last_executed_query_with_duplicate_params",
+            "backends.tests.BackendTestCase.test_queries_logger",
+            "generic_relations.tests.GenericRelationsTests.test_unsaved_generic_foreign_key_parent_bulk_create",
+            "generic_relations.tests.GenericRelationsTests.test_unsaved_generic_foreign_key_parent_save",
+            "schema.tests.SchemaTests.test_add_field_durationfield_with_default",
+            "delete.tests.DeletionTests.test_only_referenced_fields_selected",
+            "bulk_create.tests.BulkCreateTests.test_explicit_batch_size_efficiency",
+            "get_or_create.tests.UpdateOrCreateTests.test_update_only_defaults_and_pre_save_fields_when_local_fields",
+            "backends.base.test_base.DatabaseWrapperLoggingTests.test_commit_debug_log",
+            "backends.base.test_base.DatabaseWrapperLoggingTests.test_rollback_debug_log",
+            "backends.base.test_base.MultiDatabaseTests.test_multi_database_init_connection_state_called_once",
         )
 
     if os.environ.get("SPANNER_EMULATOR_HOST", None):
         # Some code isn't yet supported by the Spanner emulator.
         skip_tests += (
             # Emulator doesn't support views.
             "inspectdb.tests.InspectDBTransactionalTests.test_include_views",
@@ -825,29 +890,14 @@
             "auth_tests.test_forms.UserChangeFormTest.test_bug_17944_unmanageable_password",  # noqa
             "auth_tests.test_forms.UserChangeFormTest.test_bug_19133",  # noqa
             "auth_tests.test_forms.UserChangeFormTest.test_bug_19349_bound_password_field",  # noqa
             "auth_tests.test_forms.UserChangeFormTest.test_custom_form",  # noqa
             "auth_tests.test_forms.UserChangeFormTest.test_password_excluded",  # noqa
             "auth_tests.test_forms.UserChangeFormTest.test_unusable_password",  # noqa
             "auth_tests.test_forms.UserChangeFormTest.test_username_validity",  # noqa
-            "auth_tests.test_forms.UserCreationFormTest.test_both_passwords",  # noqa
-            "auth_tests.test_forms.UserCreationFormTest.test_custom_form",  # noqa
-            "auth_tests.test_forms.UserCreationFormTest.test_custom_form_hidden_username_field",  # noqa
-            "auth_tests.test_forms.UserCreationFormTest.test_custom_form_with_different_username_field",  # noqa
-            "auth_tests.test_forms.UserCreationFormTest.test_duplicate_normalized_unicode",  # noqa
-            "auth_tests.test_forms.UserCreationFormTest.test_invalid_data",  # noqa
-            "auth_tests.test_forms.UserCreationFormTest.test_normalize_username",  # noqa
-            "auth_tests.test_forms.UserCreationFormTest.test_password_help_text",  # noqa
-            "auth_tests.test_forms.UserCreationFormTest.test_password_verification",  # noqa
-            "auth_tests.test_forms.UserCreationFormTest.test_password_whitespace_not_stripped",  # noqa
-            "auth_tests.test_forms.UserCreationFormTest.test_success",  # noqa
-            "auth_tests.test_forms.UserCreationFormTest.test_unicode_username",  # noqa
-            "auth_tests.test_forms.UserCreationFormTest.test_user_already_exists",  # noqa
-            "auth_tests.test_forms.UserCreationFormTest.test_user_create_form_validates_password_with_all_data",  # noqa
-            "auth_tests.test_forms.UserCreationFormTest.test_validates_password",  # noqa
             "auth_tests.test_handlers.ModWsgiHandlerTestCase.test_check_password",  # noqa
             "auth_tests.test_handlers.ModWsgiHandlerTestCase.test_check_password_custom_user",  # noqa
             "auth_tests.test_handlers.ModWsgiHandlerTestCase.test_groups_for_user",  # noqa
             "auth_tests.test_management.ChangepasswordManagementCommandTestCase.test_get_pass",  # noqa
             "auth_tests.test_management.ChangepasswordManagementCommandTestCase.test_get_pass_no_input",  # noqa
             "auth_tests.test_management.ChangepasswordManagementCommandTestCase.test_nonexistent_username",  # noqa
             "auth_tests.test_management.ChangepasswordManagementCommandTestCase.test_password_validation",  # noqa
@@ -1200,15 +1250,14 @@
             "db_functions.text.test_substr.SubstrTests.test_basic",  # noqa
             "db_functions.text.test_substr.SubstrTests.test_expressions",  # noqa
             "db_functions.text.test_substr.SubstrTests.test_start",  # noqa
             "db_functions.text.test_trim.TrimTests.test_trim",  # noqa
             "db_functions.text.test_trim.TrimTests.test_trim_transform",  # noqa
             "db_functions.text.test_upper.UpperTests.test_basic",  # noqa
             "db_functions.text.test_upper.UpperTests.test_transform",  # noqa
-            "defer_regress.tests.DeferAnnotateSelectRelatedTest.test_defer_annotate_select_related",  # noqa
             "delete_regress.tests.DeleteCascadeTransactionTests.test_inheritance",  # noqa
             "delete_regress.tests.DeleteLockingTest.test_concurrent_delete",  # noqa
             "expressions.test_queryset_values.ValuesExpressionsTests.test_chained_values_with_expression",  # noqa
             "expressions.test_queryset_values.ValuesExpressionsTests.test_values_expression",  # noqa
             "expressions.test_queryset_values.ValuesExpressionsTests.test_values_expression_group_by",  # noqa
             "expressions.test_queryset_values.ValuesExpressionsTests.test_values_list_expression",  # noqa
             "expressions.test_queryset_values.ValuesExpressionsTests.test_values_list_expression_flat",  # noqa
@@ -1577,15 +1626,14 @@
             "queries.tests.Queries1Tests.test_ticket4464",  # noqa
             "queries.tests.Queries1Tests.test_ticket4510",  # noqa
             "queries.tests.Queries1Tests.test_ticket6074",  # noqa
             "queries.tests.Queries1Tests.test_ticket6154",  # noqa
             "queries.tests.Queries1Tests.test_ticket6981",  # noqa
             "queries.tests.Queries1Tests.test_ticket7076",  # noqa
             "queries.tests.Queries1Tests.test_ticket7096",  # noqa
-            "queries.tests.Queries1Tests.test_ticket7098",  # noqa
             "queries.tests.Queries1Tests.test_ticket7155",  # noqa
             "queries.tests.Queries1Tests.test_ticket7181",  # noqa
             "queries.tests.Queries1Tests.test_ticket7235",  # noqa
             "queries.tests.Queries1Tests.test_ticket7277",  # noqa
             "queries.tests.Queries1Tests.test_ticket7323",  # noqa
             "queries.tests.Queries1Tests.test_ticket7378",  # noqa
             "queries.tests.Queries1Tests.test_ticket7791",  # noqa
@@ -1790,15 +1838,14 @@
             "sitemaps_tests.test_http.HTTPSitemapTests.test_localized_priority",  # noqa
             "sitemaps_tests.test_http.HTTPSitemapTests.test_no_section",  # noqa
             "sitemaps_tests.test_http.HTTPSitemapTests.test_page_not_int",  # noqa
             "sitemaps_tests.test_http.HTTPSitemapTests.test_paged_sitemap",  # noqa
             "sitemaps_tests.test_http.HTTPSitemapTests.test_requestsite_sitemap",  # noqa
             "sitemaps_tests.test_http.HTTPSitemapTests.test_simple_custom_sitemap",  # noqa
             "sitemaps_tests.test_http.HTTPSitemapTests.test_simple_sitemap",  # noqa
-            "sitemaps_tests.test_http.HTTPSitemapTests.test_simple_sitemap_custom_index",  # noqa
             "sitemaps_tests.test_http.HTTPSitemapTests.test_simple_sitemap_index",  # noqa
             "sitemaps_tests.test_http.HTTPSitemapTests.test_simple_sitemap_section",  # noqa
             "sitemaps_tests.test_http.HTTPSitemapTests.test_sitemap_get_urls_no_site_1",  # noqa
             "sitemaps_tests.test_http.HTTPSitemapTests.test_sitemap_get_urls_no_site_2",  # noqa
             "sitemaps_tests.test_http.HTTPSitemapTests.test_sitemap_item",  # noqa
             "sitemaps_tests.test_http.HTTPSitemapTests.test_sitemap_last_modified",  # noqa
             "sitemaps_tests.test_http.HTTPSitemapTests.test_sitemap_last_modified_date",  # noqa
@@ -1969,169 +2016,167 @@
             "update_only_fields.tests.UpdateOnlyFieldsTests.test_update_fields_only_repeated",  # noqa
             "update_only_fields.tests.UpdateOnlyFieldsTests.test_update_fields_signals",  # noqa
             "validation.tests.BaseModelValidationTests.test_correct_FK_value_validates",  # noqa
             "validation.tests.BaseModelValidationTests.test_limited_FK_raises_error",  # noqa
             "validation.tests.GenericIPAddressFieldTests.test_empty_generic_ip_passes",  # noqa
             "validation.tests.GenericIPAddressFieldTests.test_v4_unpack_uniqueness_detection",  # noqa
             "validation.tests.GenericIPAddressFieldTests.test_v6_uniqueness_detection",  # noqa
+            # Check constraints are not supported by Spanner emulator.
+            "constraints.tests.CheckConstraintTests.test_abstract_name",  # noqa
+            "constraints.tests.CheckConstraintTests.test_database_constraint_unicode",  # noqa
+            # Untyped parameters are not supported:
+            # https://github.com/GoogleCloudPlatform/cloud-spanner-emulator#features-and-limitations
+            "admin_changelist.test_date_hierarchy.DateHierarchyTests.test_bounded_params_with_dst_time_zone",  # noqa
+            "admin_changelist.tests.ChangeListTests.test_changelist_search_form_validation",  # noqa
+            "admin_changelist.tests.ChangeListTests.test_clear_all_filters_link",  # noqa
+            "admin_changelist.tests.ChangeListTests.test_clear_all_filters_link_callable_filter",  # noqa
+            "admin_changelist.tests.ChangeListTests.test_no_clear_all_filters_link",  # noqa
+            "admin_changelist.tests.ChangeListTests.test_no_duplicates_for_inherited_m2m_in_list_filter",  # noqa
+            "admin_changelist.tests.ChangeListTests.test_no_duplicates_for_m2m_in_list_filter",  # noqa
+            "admin_changelist.tests.ChangeListTests.test_no_duplicates_for_m2m_to_inherited_in_list_filter",  # noqa
+            "admin_changelist.tests.ChangeListTests.test_no_duplicates_for_many_to_many_at_second_level_in_search_fields",  # noqa
+            "admin_changelist.tests.ChangeListTests.test_no_duplicates_for_non_unique_related_object_in_list_filter",  # noqa
+            "admin_changelist.tests.ChangeListTests.test_no_duplicates_for_non_unique_related_object_in_search_fields",  # noqa
+            "admin_changelist.tests.ChangeListTests.test_no_duplicates_for_through_m2m_at_second_level_in_list_filter",  # noqa
+            "admin_changelist.tests.ChangeListTests.test_no_duplicates_for_through_m2m_in_list_filter",  # noqa
+            "admin_changelist.tests.ChangeListTests.test_no_exists_for_m2m_in_list_filter_without_params",  # noqa
+            "admin_changelist.tests.ChangeListTests.test_total_ordering_optimization_meta_constraints",  # noqa
+            "admin_docs.test_middleware.XViewMiddlewareTest.test_no_auth_middleware",  # noqa
+            "admin_docs.test_views.AdminDocViewDefaultEngineOnly.test_template_detail_path_traversal",  # noqa
+            "admin_inlines.tests.TestInline.test_custom_form_tabular_inline_extra_field_label",  # noqa
+            "admin_inlines.tests.TestInline.test_inlines_singular_heading_one_to_one",  # noqa
+            "admin_inlines.tests.TestInline.test_non_editable_custom_form_tabular_inline_extra_field_label",  # noqa
+            "admin_views.test_multidb.MultiDatabaseTests.test_delete_view",  # noqa
+            "auth_tests.test_auth_backends.AuthenticateTests.test_authenticate_sensitive_variables",  # noqa
+            "auth_tests.test_auth_backends.AuthenticateTests.test_clean_credentials_sensitive_variables",  # noqa
+            "auth_tests.test_auth_backends.AuthenticateTests.test_skips_backends_with_decorated_method",  # noqa
+            "auth_tests.test_auth_backends.BaseBackendTest.test_get_all_permissions",  # noqa
+            "auth_tests.test_auth_backends.BaseBackendTest.test_get_group_permissions",  # noqa
+            "auth_tests.test_auth_backends.BaseBackendTest.test_get_user_permissions",  # noqa
+            "auth_tests.test_auth_backends.BaseBackendTest.test_has_perm",  # noqa
+            "auth_tests.test_auth_backends.CustomPermissionsUserModelBackendTest.test_authentication_without_credentials",  # noqa
+            "auth_tests.test_auth_backends.ExtensionUserModelBackendTest.test_authentication_without_credentials",  # noqa
+            "auth_tests.test_auth_backends.ModelBackendTest.test_authentication_without_credentials",  # noqa
+            "auth_tests.test_basic.BasicTestCase.test_superuser_no_email_or_password",  # noqa
+            "auth_tests.test_basic.BasicTestCase.test_superuser_no_email_or_password",  # noqa
+            "auth_tests.test_basic.BasicTestCase.test_superuser_no_email_or_password",  # noqa
+            "auth_tests.test_basic.BasicTestCase.test_superuser_no_email_or_password",  # noqa
+            "auth_tests.test_decorators.LoginRequiredTestCase.test_callable",  # noqa
+            "auth_tests.test_decorators.LoginRequiredTestCase.test_login_required",  # noqa
+            "auth_tests.test_decorators.LoginRequiredTestCase.test_login_required_next_url",  # noqa
+            "auth_tests.test_decorators.LoginRequiredTestCase.test_view",  # noqa
+            "auth_tests.test_forms.AdminPasswordChangeFormTest.test_html_autocomplete_attributes",  # noqa
+            "auth_tests.test_forms.AuthenticationFormTest.test_html_autocomplete_attributes",  # noqa
+            "auth_tests.test_forms.AuthenticationFormTest.test_username_field_autocapitalize_none",  # noqa
+            "auth_tests.test_forms.PasswordChangeFormTest.test_html_autocomplete_attributes",  # noqa
+            "auth_tests.test_forms.PasswordResetFormTest.test_html_autocomplete_attributes",  # noqa
+            "auth_tests.test_forms.SetPasswordFormTest.test_html_autocomplete_attributes",  # noqa
+            "auth_tests.test_forms.UserChangeFormTest.test_username_field_autocapitalize_none",  # noqa
+            "auth_tests.test_management.CreatesuperuserManagementCommandTestCase.test_environment_variable_non_interactive",  # noqa
+            "auth_tests.test_management.CreatesuperuserManagementCommandTestCase.test_fields_with_m2m",  # noqa
+            "auth_tests.test_management.CreatesuperuserManagementCommandTestCase.test_fields_with_m2m_interactive",  # noqa
+            "auth_tests.test_management.CreatesuperuserManagementCommandTestCase.test_fields_with_m2m_interactive_blank",  # noqa
+            "auth_tests.test_management.CreatesuperuserManagementCommandTestCase.test_ignore_environment_variable_interactive",  # noqa
+            "auth_tests.test_management.CreatesuperuserManagementCommandTestCase.test_ignore_environment_variable_non_interactive",  # noqa
+            "auth_tests.test_management.GetDefaultUsernameTestCase.test_with_database",  # noqa
+            "auth_tests.test_management.MultiDBCreatesuperuserTestCase.test_createsuperuser_command_suggested_username_with_database_option",  # noqa
+            "auth_tests.test_middleware.TestAuthenticationMiddleware.test_no_session",  # noqa
+            "auth_tests.test_models.UserManagerTestCase.test_runpython_manager_methods",  # noqa
+            "auth_tests.test_models.UserWithPermTestCase.test_backend_without_with_perm",  # noqa
+            "auth_tests.test_models.UserWithPermTestCase.test_basic",  # noqa
+            "auth_tests.test_models.UserWithPermTestCase.test_custom_backend",  # noqa
+            "auth_tests.test_models.UserWithPermTestCase.test_custom_backend_pass_obj",  # noqa
+            "auth_tests.test_models.UserWithPermTestCase.test_invalid_backend_type",  # noqa
+            "auth_tests.test_models.UserWithPermTestCase.test_invalid_permission_name",  # noqa
+            "auth_tests.test_models.UserWithPermTestCase.test_invalid_permission_type",  # noqa
+            "auth_tests.test_models.UserWithPermTestCase.test_multiple_backends",  # noqa
+            "auth_tests.test_models.UserWithPermTestCase.test_nonexistent_backend",  # noqa
+            "auth_tests.test_models.UserWithPermTestCase.test_nonexistent_permission",  # noqa
+            "auth_tests.test_remote_user.AllowAllUsersRemoteUserBackendTest.test_csrf_validation_passes_after_process_request_login",  # noqa
+            "auth_tests.test_remote_user.CustomHeaderRemoteUserTest.test_csrf_validation_passes_after_process_request_login",  # noqa
+            "auth_tests.test_remote_user.PersistentRemoteUserTest.test_csrf_validation_passes_after_process_request_login",  # noqa
+            "auth_tests.test_remote_user.RemoteUserCustomTest.test_csrf_validation_passes_after_process_request_login",  # noqa
+            "auth_tests.test_remote_user.RemoteUserTest.test_csrf_validation_passes_after_process_request_login",  # noqa
+            "auth_tests.test_templates.AuthTemplateTests.test_password_change_done_view",  # noqa
+            "auth_tests.test_templates.AuthTemplateTests.test_password_reset_change_view",  # noqa
+            "auth_tests.test_templates.AuthTemplateTests.test_password_reset_complete_view",  # noqa
+            "auth_tests.test_templates.AuthTemplateTests.test_password_reset_confirm_view_custom_username_hint",  # noqa
+            "auth_tests.test_templates.AuthTemplateTests.test_password_reset_confirm_view_invalid_token",  # noqa
+            "auth_tests.test_templates.AuthTemplateTests.test_password_reset_confirm_view_valid_token",  # noqa
+            "auth_tests.test_templates.AuthTemplateTests.test_password_reset_done_view",  # noqa
+            "auth_tests.test_templates.AuthTemplateTests.test_password_reset_view",  # noqa
+            "auth_tests.test_tokens.TokenGeneratorTest.test_token_with_different_email",  # noqa
+            "auth_tests.test_views.PasswordResetTest.test_confirm_custom_reset_url_token",  # noqa
+            "auth_tests.test_views.PasswordResetTest.test_confirm_custom_reset_url_token_link_redirects_to_set_password_page",  # noqa
+            "datetimes.tests.DateTimesTests.test_datetimes_ambiguous_and_invalid_times",  # noqa
+            "db_functions.comparison.test_cast.CastTests.test_cast_to_duration",  # noqa
+            "fixtures.tests.TestCaseFixtureLoadingTests.test_class_fixtures",  # noqa
+            "generic_inline_admin.tests.GenericInlineAdminParametersTest.test_max_num_param",  # noqa
+            "queries.tests.Queries1Tests.test_excluded_intermediary_m2m_table_joined",  # noqa
+            "queries.tests.Queries1Tests.test_field_with_filterable",  # noqa
+            "queries.tests.Queries1Tests.test_negate_field",  # noqa
+            "queries.tests.Queries1Tests.test_order_by_rawsql",  # noqa
+            "queries.tests.Queries4Tests.test_combine_or_filter_reuse",  # noqa
+            "queries.tests.Queries4Tests.test_filter_reverse_non_integer_pk",  # noqa
+            "schema.tests.SchemaTests.test_alter_field_default_doesnt_perform_queries",  # noqa
+            "sitemaps_tests.test_http.HTTPSitemapTests.test_alternate_i18n_sitemap_index",  # noqa
+            "sitemaps_tests.test_http.HTTPSitemapTests.test_alternate_i18n_sitemap_limited",  # noqa
+            "sitemaps_tests.test_http.HTTPSitemapTests.test_alternate_i18n_sitemap_xdefault",  # noqa
+            "sitemaps_tests.test_http.HTTPSitemapTests.test_simple_i18n_sitemap_index",  # noqa
+            "test_client.tests.ClientTest.test_exc_info",  # noqa
+            "test_client.tests.ClientTest.test_exc_info_none",  # noqa
+            "test_client.tests.ClientTest.test_follow_307_and_308_get_head_query_string",  # noqa
+            "test_client.tests.ClientTest.test_follow_307_and_308_preserves_query_string",  # noqa
         )
-
         if USING_DJANGO_3:
-            # Some tests are different between django 3.2 and 2.2.
             skip_tests += (
-                # Check constraints are not supported by Spanner emulator.
-                "constraints.tests.CheckConstraintTests.test_abstract_name",  # noqa
-                "constraints.tests.CheckConstraintTests.test_database_constraint_expression",  # noqa
                 "constraints.tests.CheckConstraintTests.test_database_constraint_expressionwrapper",  # noqa
-                "constraints.tests.CheckConstraintTests.test_database_constraint_unicode",  # noqa
-                # Untyped parameters are not supported:
-                # https://github.com/GoogleCloudPlatform/cloud-spanner-emulator#features-and-limitations
-                "admin_changelist.test_date_hierarchy.DateHierarchyTests.test_bounded_params_with_dst_time_zone",  # noqa
-                "admin_changelist.tests.ChangeListTests.test_changelist_search_form_validation",  # noqa
-                "admin_changelist.tests.ChangeListTests.test_clear_all_filters_link",  # noqa
-                "admin_changelist.tests.ChangeListTests.test_clear_all_filters_link_callable_filter",  # noqa
-                "admin_changelist.tests.ChangeListTests.test_no_clear_all_filters_link",  # noqa
-                "admin_changelist.tests.ChangeListTests.test_no_duplicates_for_inherited_m2m_in_list_filter",  # noqa
-                "admin_changelist.tests.ChangeListTests.test_no_duplicates_for_m2m_in_list_filter",  # noqa
-                "admin_changelist.tests.ChangeListTests.test_no_duplicates_for_m2m_to_inherited_in_list_filter",  # noqa
-                "admin_changelist.tests.ChangeListTests.test_no_duplicates_for_many_to_many_at_second_level_in_search_fields",  # noqa
-                "admin_changelist.tests.ChangeListTests.test_no_duplicates_for_non_unique_related_object_in_list_filter",  # noqa
-                "admin_changelist.tests.ChangeListTests.test_no_duplicates_for_non_unique_related_object_in_search_fields",  # noqa
-                "admin_changelist.tests.ChangeListTests.test_no_duplicates_for_through_m2m_at_second_level_in_list_filter",  # noqa
-                "admin_changelist.tests.ChangeListTests.test_no_duplicates_for_through_m2m_in_list_filter",  # noqa
-                "admin_changelist.tests.ChangeListTests.test_no_exists_for_m2m_in_list_filter_without_params",  # noqa
-                "admin_changelist.tests.ChangeListTests.test_total_ordering_optimization_meta_constraints",  # noqa
-                "admin_docs.test_middleware.XViewMiddlewareTest.test_no_auth_middleware",  # noqa
-                "admin_docs.test_views.AdminDocViewDefaultEngineOnly.test_template_detail_path_traversal",  # noqa
-                "admin_inlines.tests.TestInline.test_custom_form_tabular_inline_extra_field_label",  # noqa
-                "admin_inlines.tests.TestInline.test_inlines_singular_heading_one_to_one",  # noqa
-                "admin_inlines.tests.TestInline.test_non_editable_custom_form_tabular_inline_extra_field_label",  # noqa
-                "admin_views.test_multidb.MultiDatabaseTests.test_delete_view",  # noqa
-                "auth_tests.test_auth_backends.AuthenticateTests.test_authenticate_sensitive_variables",  # noqa
-                "auth_tests.test_auth_backends.AuthenticateTests.test_clean_credentials_sensitive_variables",  # noqa
-                "auth_tests.test_auth_backends.AuthenticateTests.test_skips_backends_with_decorated_method",  # noqa
-                "auth_tests.test_auth_backends.BaseBackendTest.test_get_all_permissions",  # noqa
-                "auth_tests.test_auth_backends.BaseBackendTest.test_get_group_permissions",  # noqa
-                "auth_tests.test_auth_backends.BaseBackendTest.test_get_user_permissions",  # noqa
-                "auth_tests.test_auth_backends.BaseBackendTest.test_has_perm",  # noqa
-                "auth_tests.test_auth_backends.CustomPermissionsUserModelBackendTest.test_authentication_without_credentials",  # noqa
-                "auth_tests.test_auth_backends.ExtensionUserModelBackendTest.test_authentication_without_credentials",  # noqa
-                "auth_tests.test_auth_backends.ModelBackendTest.test_authentication_without_credentials",  # noqa
-                "auth_tests.test_basic.BasicTestCase.test_superuser_no_email_or_password",  # noqa
-                "auth_tests.test_basic.BasicTestCase.test_superuser_no_email_or_password",  # noqa
-                "auth_tests.test_basic.BasicTestCase.test_superuser_no_email_or_password",  # noqa
-                "auth_tests.test_basic.BasicTestCase.test_superuser_no_email_or_password",  # noqa
-                "auth_tests.test_decorators.LoginRequiredTestCase.test_callable",  # noqa
-                "auth_tests.test_decorators.LoginRequiredTestCase.test_login_required",  # noqa
-                "auth_tests.test_decorators.LoginRequiredTestCase.test_login_required_next_url",  # noqa
-                "auth_tests.test_decorators.LoginRequiredTestCase.test_view",  # noqa
-                "auth_tests.test_forms.AdminPasswordChangeFormTest.test_html_autocomplete_attributes",  # noqa
-                "auth_tests.test_forms.AuthenticationFormTest.test_html_autocomplete_attributes",  # noqa
-                "auth_tests.test_forms.AuthenticationFormTest.test_username_field_autocapitalize_none",  # noqa
-                "auth_tests.test_forms.PasswordChangeFormTest.test_html_autocomplete_attributes",  # noqa
-                "auth_tests.test_forms.PasswordResetFormTest.test_html_autocomplete_attributes",  # noqa
-                "auth_tests.test_forms.SetPasswordFormTest.test_html_autocomplete_attributes",  # noqa
-                "auth_tests.test_forms.UserChangeFormTest.test_username_field_autocapitalize_none",  # noqa
+                "defer_regress.tests.DeferAnnotateSelectRelatedTest.test_defer_annotate_select_related",  # noqa
+                "queries.tests.Queries1Tests.test_ticket7098",  # noqa
+                "auth_tests.test_password_reset_timeout_days.DeprecationTests.test_timeout",  # noqa
+                "constraints.tests.CheckConstraintTests.test_database_constraint_expression",  # noqa
+                "queries.tests.Queries1Tests.test_order_by_raw_column_alias_warning",  # noqa
+                "sitemaps_tests.test_http.HTTPSitemapTests.test_simple_sitemap_custom_index",  # noqa
+                "auth_tests.test_forms.UserCreationFormTest.test_both_passwords",  # noqa
+                "auth_tests.test_forms.UserCreationFormTest.test_custom_form",  # noqa
+                "auth_tests.test_forms.UserCreationFormTest.test_custom_form_hidden_username_field",  # noqa
+                "auth_tests.test_forms.UserCreationFormTest.test_custom_form_with_different_username_field",  # noqa
+                "auth_tests.test_forms.UserCreationFormTest.test_duplicate_normalized_unicode",  # noqa
+                "auth_tests.test_forms.UserCreationFormTest.test_invalid_data",  # noqa
+                "auth_tests.test_forms.UserCreationFormTest.test_normalize_username",  # noqa
+                "auth_tests.test_forms.UserCreationFormTest.test_password_help_text",  # noqa
+                "auth_tests.test_middleware.TestAuthenticationMiddleware.test_session_default_hashing_algorithm",  # noqa
+                "auth_tests.test_forms.UserCreationFormTest.test_password_verification",  # noqa
+                "auth_tests.test_forms.UserCreationFormTest.test_password_whitespace_not_stripped",  # noqa
+                "auth_tests.test_forms.UserCreationFormTest.test_success",  # noqa
+                "auth_tests.test_forms.UserCreationFormTest.test_unicode_username",  # noqa
+                "auth_tests.test_forms.UserCreationFormTest.test_user_already_exists",  # noqa
+                "auth_tests.test_forms.UserCreationFormTest.test_user_create_form_validates_password_with_all_data",  # noqa
+                "auth_tests.test_forms.UserCreationFormTest.test_validates_password",  # noqa
                 "auth_tests.test_forms.UserCreationFormTest.test_html_autocomplete_attributes",  # noqa
                 "auth_tests.test_forms.UserCreationFormTest.test_username_field_autocapitalize_none",  # noqa
-                "auth_tests.test_management.CreatesuperuserManagementCommandTestCase.test_environment_variable_non_interactive",  # noqa
-                "auth_tests.test_management.CreatesuperuserManagementCommandTestCase.test_fields_with_m2m",  # noqa
-                "auth_tests.test_management.CreatesuperuserManagementCommandTestCase.test_fields_with_m2m_interactive",  # noqa
-                "auth_tests.test_management.CreatesuperuserManagementCommandTestCase.test_fields_with_m2m_interactive_blank",  # noqa
-                "auth_tests.test_management.CreatesuperuserManagementCommandTestCase.test_ignore_environment_variable_interactive",  # noqa
-                "auth_tests.test_management.CreatesuperuserManagementCommandTestCase.test_ignore_environment_variable_non_interactive",  # noqa
-                "auth_tests.test_management.GetDefaultUsernameTestCase.test_with_database",  # noqa
-                "auth_tests.test_management.MultiDBCreatesuperuserTestCase.test_createsuperuser_command_suggested_username_with_database_option",  # noqa
                 "auth_tests.test_middleware.TestAuthenticationMiddleware.test_no_password_change_does_not_invalidate_legacy_session",  # noqa
-                "auth_tests.test_middleware.TestAuthenticationMiddleware.test_no_session",  # noqa
-                "auth_tests.test_middleware.TestAuthenticationMiddleware.test_session_default_hashing_algorithm",  # noqa
-                "auth_tests.test_models.UserManagerTestCase.test_runpython_manager_methods",  # noqa
-                "auth_tests.test_models.UserWithPermTestCase.test_backend_without_with_perm",  # noqa
-                "auth_tests.test_models.UserWithPermTestCase.test_basic",  # noqa
-                "auth_tests.test_models.UserWithPermTestCase.test_custom_backend",  # noqa
-                "auth_tests.test_models.UserWithPermTestCase.test_custom_backend_pass_obj",  # noqa
-                "auth_tests.test_models.UserWithPermTestCase.test_invalid_backend_type",  # noqa
-                "auth_tests.test_models.UserWithPermTestCase.test_invalid_permission_name",  # noqa
-                "auth_tests.test_models.UserWithPermTestCase.test_invalid_permission_type",  # noqa
-                "auth_tests.test_models.UserWithPermTestCase.test_multiple_backends",  # noqa
-                "auth_tests.test_models.UserWithPermTestCase.test_nonexistent_backend",  # noqa
-                "auth_tests.test_models.UserWithPermTestCase.test_nonexistent_permission",  # noqa
-                "auth_tests.test_password_reset_timeout_days.DeprecationTests.test_timeout",  # noqa
-                "auth_tests.test_remote_user.AllowAllUsersRemoteUserBackendTest.test_csrf_validation_passes_after_process_request_login",  # noqa
-                "auth_tests.test_remote_user.CustomHeaderRemoteUserTest.test_csrf_validation_passes_after_process_request_login",  # noqa
-                "auth_tests.test_remote_user.PersistentRemoteUserTest.test_csrf_validation_passes_after_process_request_login",  # noqa
-                "auth_tests.test_remote_user.RemoteUserCustomTest.test_csrf_validation_passes_after_process_request_login",  # noqa
-                "auth_tests.test_remote_user.RemoteUserTest.test_csrf_validation_passes_after_process_request_login",  # noqa
-                "auth_tests.test_templates.AuthTemplateTests.test_password_change_done_view",  # noqa
-                "auth_tests.test_templates.AuthTemplateTests.test_password_reset_change_view",  # noqa
-                "auth_tests.test_templates.AuthTemplateTests.test_password_reset_complete_view",  # noqa
-                "auth_tests.test_templates.AuthTemplateTests.test_password_reset_confirm_view_custom_username_hint",  # noqa
-                "auth_tests.test_templates.AuthTemplateTests.test_password_reset_confirm_view_invalid_token",  # noqa
-                "auth_tests.test_templates.AuthTemplateTests.test_password_reset_confirm_view_valid_token",  # noqa
-                "auth_tests.test_templates.AuthTemplateTests.test_password_reset_done_view",  # noqa
-                "auth_tests.test_templates.AuthTemplateTests.test_password_reset_view",  # noqa
                 "auth_tests.test_tokens.TokenGeneratorTest.test_legacy_days_timeout",  # noqa
                 "auth_tests.test_tokens.TokenGeneratorTest.test_legacy_token_validation",  # noqa
                 "auth_tests.test_tokens.TokenGeneratorTest.test_token_default_hashing_algorithm",  # noqa
-                "auth_tests.test_tokens.TokenGeneratorTest.test_token_with_different_email",  # noqa
-                "auth_tests.test_tokens.TokenGeneratorTest.test_token_with_different_email",  # noqa
-                "auth_tests.test_tokens.TokenGeneratorTest.test_token_with_different_email",  # noqa
                 "auth_tests.test_views.LoginTest.test_legacy_session_key_flushed_on_login",  # noqa
-                "auth_tests.test_views.PasswordResetTest.test_confirm_custom_reset_url_token",  # noqa
-                "auth_tests.test_views.PasswordResetTest.test_confirm_custom_reset_url_token_link_redirects_to_set_password_page",  # noqa
-                "datetimes.tests.DateTimesTests.test_datetimes_ambiguous_and_invalid_times",  # noqa
-                "db_functions.comparison.test_cast.CastTests.test_cast_to_duration",  # noqa
-                "fixtures.tests.TestCaseFixtureLoadingTests.test_class_fixtures",  # noqa
-                "generic_inline_admin.tests.GenericInlineAdminParametersTest.test_max_num_param",  # noqa
-                "queries.tests.Queries1Tests.test_excluded_intermediary_m2m_table_joined",  # noqa
-                "queries.tests.Queries1Tests.test_field_with_filterable",  # noqa
-                "queries.tests.Queries1Tests.test_negate_field",  # noqa
-                "queries.tests.Queries1Tests.test_order_by_raw_column_alias_warning",  # noqa
-                "queries.tests.Queries1Tests.test_order_by_rawsql",  # noqa
-                "queries.tests.Queries4Tests.test_combine_or_filter_reuse",  # noqa
-                "queries.tests.Queries4Tests.test_filter_reverse_non_integer_pk",  # noqa
-                "schema.tests.SchemaTests.test_alter_field_default_doesnt_perform_queries",  # noqa
-                "sitemaps_tests.test_http.HTTPSitemapTests.test_alternate_i18n_sitemap_index",  # noqa
-                "sitemaps_tests.test_http.HTTPSitemapTests.test_alternate_i18n_sitemap_limited",  # noqa
-                "sitemaps_tests.test_http.HTTPSitemapTests.test_alternate_i18n_sitemap_xdefault",  # noqa
-                "sitemaps_tests.test_http.HTTPSitemapTests.test_simple_i18n_sitemap_index",  # noqa
-                "test_client.tests.ClientTest.test_exc_info",  # noqa
-                "test_client.tests.ClientTest.test_exc_info_none",  # noqa
-                "test_client.tests.ClientTest.test_follow_307_and_308_get_head_query_string",  # noqa
-                "test_client.tests.ClientTest.test_follow_307_and_308_preserves_query_string",  # noqa
             )
-        else:
+        if USING_DJANGO_4:
             skip_tests += (
-                # Untyped parameters are not supported:
-                # https://github.com/GoogleCloudPlatform/cloud-spanner-emulator#features-and-limitations
-                "queries.tests.Queries1Tests.test_ticket9411",  # noqa
-                "admin_changelist.tests.ChangeListTests.test_distinct_for_inherited_m2m_in_list_filter",  # noqa
-                "admin_changelist.tests.ChangeListTests.test_distinct_for_m2m_in_list_filter",  # noqa
-                "admin_changelist.tests.ChangeListTests.test_distinct_for_m2m_to_inherited_in_list_filter",  # noqa
-                "admin_changelist.tests.ChangeListTests.test_distinct_for_many_to_many_at_second_level_in_search_fields",  # noqa
-                "admin_changelist.tests.ChangeListTests.test_distinct_for_non_unique_related_object_in_list_filter",  # noqa
-                "admin_changelist.tests.ChangeListTests.test_distinct_for_non_unique_related_object_in_search_fields",  # noqa
-                "admin_changelist.tests.ChangeListTests.test_distinct_for_through_m2m_at_second_level_in_list_filter",  # noqa
-                "admin_changelist.tests.ChangeListTests.test_distinct_for_through_m2m_in_list_filter",  # noqa
-                "admin_changelist.tests.ChangeListTests.test_no_distinct_for_m2m_in_list_filter_without_params",  # noqa
-                "aggregation.tests.AggregateTestCase.test_missing_output_field_raises_error",  # noqa
-                "auth_tests.test_decorators.LoginRequiredTestCase.testCallable",  # noqa
-                "auth_tests.test_decorators.LoginRequiredTestCase.testLoginRequired",  # noqa
-                "auth_tests.test_decorators.LoginRequiredTestCase.testLoginRequiredNextUrl",  # noqa
-                "auth_tests.test_decorators.LoginRequiredTestCase.testView",  # noqa
-                "auth_tests.test_remote_user_deprecation.RemoteUserCustomTest.test_configure_user_deprecation_warning",  # noqa
-                "auth_tests.test_templates.AuthTemplateTests.test_PasswordChangeDoneView",  # noqa
-                "auth_tests.test_templates.AuthTemplateTests.test_PasswordResetChangeView",  # noqa
-                "auth_tests.test_templates.AuthTemplateTests.test_PasswordResetCompleteView",  # noqa
-                "auth_tests.test_templates.AuthTemplateTests.test_PasswordResetConfirmView_invalid_token",  # noqa
-                "auth_tests.test_templates.AuthTemplateTests.test_PasswordResetConfirmView_valid_token",  # noqa
-                "auth_tests.test_templates.AuthTemplateTests.test_PasswordResetDoneView",  # noqa
-                "auth_tests.test_templates.AuthTemplateTests.test_PasswordResetView",  # noqa
-                "fixtures.tests.TestCaseFixtureLoadingTests.testClassFixtures",  # noqa
-                "fixtures_model_package.tests.SampleTestCase.testClassFixtures",  # noqa
-                "generic_inline_admin.tests.GenericInlineAdminParametersTest.testMaxNumParam",  # noqa
-                "migrations.test_operations.OperationTests.test_autofield_foreignfield_growth",  # noqa
-                "ordering.tests.OrderingTests.test_deprecated_values_annotate",  # noqa
-                "queries.tests.Queries1Tests.test_ticket2902",  # noqa
-                "schema.tests.SchemaTests.test_alter_field_default_doesnt_perfom_queries",  # noqa
-                "sitemaps_tests.test_http.HTTPSitemapTests.test_simple_i18nsitemap_index",  # noqa
+                "auth_tests.test_forms.BaseUserCreationFormTest.test_both_passwords",  # noqa
+                "auth_tests.test_forms.BaseUserCreationFormTest.test_custom_form",  # noqa
+                "auth_tests.test_forms.BaseUserCreationFormTest.test_custom_form_hidden_username_field",  # noqa
+                "auth_tests.test_forms.BaseUserCreationFormTest.test_custom_form_with_different_username_field",  # noqa
+                "auth_tests.test_forms.BaseUserCreationFormTest.test_duplicate_normalized_unicode",  # noqa
+                "auth_tests.test_forms.BaseUserCreationFormTest.test_invalid_data",  # noqa
+                "auth_tests.test_forms.BaseUserCreationFormTest.test_normalize_username",  # noqa
+                "auth_tests.test_forms.BaseUserCreationFormTest.test_password_help_text",  # noqa
+                "auth_tests.test_forms.BaseUserCreationFormTest.test_password_verification",  # noqa
+                "auth_tests.test_forms.BaseUserCreationFormTest.test_password_whitespace_not_stripped",  # noqa
+                "auth_tests.test_forms.BaseUserCreationFormTest.test_success",  # noqa
+                "auth_tests.test_forms.BaseUserCreationFormTest.test_unicode_username",  # noqa
+                "auth_tests.test_forms.BaseUserCreationFormTest.test_user_already_exists",  # noqa
+                "auth_tests.test_forms.BaseUserCreationFormTest.test_user_create_form_validates_password_with_all_data",  # noqa
+                "auth_tests.test_forms.BaseUserCreationFormTest.test_validates_password",  # noqa
+                "auth_tests.test_forms.BaseUserCreationFormTest.test_html_autocomplete_attributes",  # noqa
+                "auth_tests.test_forms.BaseUserCreationFormTest.test_username_field_autocapitalize_none",  # noqa
             )
```

### Comparing `django-google-spanner-3.1.0/django_spanner/functions.py` & `django-google-spanner-4.0.1/django_spanner/functions.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.1.0/django_spanner/introspection.py` & `django-google-spanner-4.0.1/django_spanner/introspection.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     BaseDatabaseIntrospection,
     FieldInfo,
     TableInfo,
 )
 from django.db.models import Index
 from google.cloud.spanner_v1 import TypeCode
 from django_spanner import USE_EMULATOR
-from django_spanner import USING_DJANGO_3
 
 
 class DatabaseIntrospection(BaseDatabaseIntrospection):
     """A Spanner-specific version of Django introspection utilities."""
 
     data_types_reverse = {
         TypeCode.BOOL: "BooleanField",
@@ -103,41 +102,27 @@
             if details.spanner_type.startswith("STRING"):
                 # Extract the size of the string from, e.g. STRING(#).
                 internal_size = details.spanner_type[7:-1]
                 if internal_size != "MAX":
                     internal_size = int(internal_size)
             else:
                 internal_size = None
-            if USING_DJANGO_3:
-                descriptions.append(
-                    FieldInfo(
-                        column_name,
-                        type_code,
-                        None,  # display_size
-                        internal_size,
-                        None,  # precision
-                        None,  # scale
-                        details.null_ok,
-                        None,  # default
-                        None,  # collation
-                    )
-                )
-            else:
-                descriptions.append(
-                    FieldInfo(
-                        column_name,
-                        type_code,
-                        None,  # display_size
-                        internal_size,
-                        None,  # precision
-                        None,  # scale
-                        details.null_ok,
-                        None,  # default
-                    )
+            descriptions.append(
+                FieldInfo(
+                    column_name,
+                    type_code,
+                    None,  # display_size
+                    internal_size,
+                    None,  # precision
+                    None,  # scale
+                    details.null_ok,
+                    None,  # default
+                    None,  # collation
                 )
+            )
 
         return descriptions
 
     def get_relations(self, cursor, table_name):
         """Return a dictionary of {field_name: (field_name_other_table, other_table)}
         representing all the relationships in the table.
```

### Comparing `django-google-spanner-3.1.0/django_spanner/lookups.py` & `django-google-spanner-4.0.1/django_spanner/lookups.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.1.0/django_spanner/operations.py` & `django-google-spanner-4.0.1/django_spanner/operations.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from datetime import datetime, time
 from uuid import UUID
 
 from django.conf import settings
 from django.db.backends.base.operations import BaseDatabaseOperations
 from django.db.utils import DatabaseError
 from django.utils import timezone
+from django_spanner import USING_DJANGO_3
 from django.utils.duration import duration_microseconds
 from google.cloud.spanner_dbapi.parse_utils import (
     DateStr,
     TimestampStr,
     escape_name,
 )
 
@@ -342,193 +343,421 @@
         :rtype: :class:`uuid.UUID`
         :returns: A converted UUID.
         """
         if value is not None:
             value = UUID(value)
         return value
 
-    def date_extract_sql(self, lookup_type, field_name):
+    def date_extract_sql(self, lookup_type, field_name, params=None):
         """Extract date from the lookup.
 
         :type lookup_type: str
         :param lookup_type: A type of the lookup.
 
         :type field_name: str
         :param field_name: The name of the field.
 
+        :type params: list(str)
+        :param params: list of query params.
+
         :rtype: str
         :returns: A SQL statement for extracting.
         """
         lookup_type = self.extract_names.get(lookup_type, lookup_type)
-        return "EXTRACT(%s FROM %s)" % (lookup_type, field_name)
-
-    def datetime_extract_sql(self, lookup_type, field_name, tzname):
-        """Extract datetime from the lookup.
-
-        :type lookup_type: str
-        :param lookup_type: A type of the lookup.
-
-        :type field_name: str
-        :param field_name: The name of the field.
+        sql = "EXTRACT(%s FROM %s)" % (lookup_type, field_name)
+        if USING_DJANGO_3:
+            return sql
+        return sql, params
+
+    if USING_DJANGO_3:
+
+        def datetime_extract_sql(self, lookup_type, field_name, tzname):
+            """Extract datetime from the lookup.
+
+            :type lookup_type: str
+            :param lookup_type: A type of the lookup.
+
+            :type field_name: str
+            :param field_name: The name of the field.
+
+            :type tzname: str
+            :param tzname: The time zone name. If using of time zone is not
+                           allowed in settings default will be UTC.
+
+            :rtype: str
+            :returns: A SQL statement for extracting.
+            """
+            tzname = tzname if settings.USE_TZ and tzname else "UTC"
+            lookup_type = self.extract_names.get(lookup_type, lookup_type)
+            return 'EXTRACT(%s FROM %s AT TIME ZONE "%s")' % (
+                lookup_type,
+                field_name,
+                tzname,
+            )
 
-        :type tzname: str
-        :param tzname: The time zone name. If using of time zone is not
-                       allowed in settings default will be UTC.
+    else:
 
-        :rtype: str
-        :returns: A SQL statement for extracting.
-        """
-        tzname = tzname if settings.USE_TZ and tzname else "UTC"
-        lookup_type = self.extract_names.get(lookup_type, lookup_type)
-        return 'EXTRACT(%s FROM %s AT TIME ZONE "%s")' % (
-            lookup_type,
-            field_name,
-            tzname,
-        )
+        def datetime_extract_sql(
+            self, lookup_type, field_name, params, tzname
+        ):
+            """Extract datetime from the lookup.
+
+            :type lookup_type: str
+            :param lookup_type: A type of the lookup.
+
+            :type field_name: str
+            :param field_name: The name of the field.
+
+            :type tzname: str
+            :param tzname: The time zone name. If using of time zone is not
+                           allowed in settings default will be UTC.
+
+            :rtype: str
+            :returns: A SQL statement for extracting.
+            """
+            tzname = tzname if settings.USE_TZ and tzname else "UTC"
+            lookup_type = self.extract_names.get(lookup_type, lookup_type)
+            return (
+                'EXTRACT(%s FROM %s AT TIME ZONE "%s")'
+                % (
+                    lookup_type,
+                    field_name,
+                    tzname,
+                ),
+                params,
+            )
 
-    def time_extract_sql(self, lookup_type, field_name):
+    def time_extract_sql(self, lookup_type, field_name, params=None):
         """Extract time from the lookup.
 
         :type lookup_type: str
         :param lookup_type: A type of the lookup.
 
         :type field_name: str
         :param field_name: The name of the field.
 
+        :type params: list(str)
+        :param params: list of query params.
+
         :rtype: str
         :returns: A SQL statement for extracting.
         """
         # Time is stored as TIMESTAMP with UTC time zone.
-        return 'EXTRACT(%s FROM %s AT TIME ZONE "UTC")' % (
+        sql = 'EXTRACT(%s FROM %s AT TIME ZONE "UTC")' % (
             lookup_type,
             field_name,
         )
-
-    def date_trunc_sql(self, lookup_type, field_name, tzname=None):
-        """Truncate date in the lookup.
-
-        :type lookup_type: str
-        :param lookup_type: A type of the lookup.
-
-        :type field_name: str
-        :param field_name: The name of the field.
-
-        :type tzname: str
-        :param tzname: The name of the timezone. This is ignored because
-        Spanner does not support Timezone conversion in DATE_TRUNC function.
-
-        :rtype: str
-        :returns: A SQL statement for truncating.
-        """
-        # https://cloud.google.com/spanner/docs/functions-and-operators#date_trunc
-        if lookup_type == "week":
-            # Spanner truncates to Sunday but Django expects Monday. First,
-            # subtract a day so that a Sunday will be truncated to the previous
-            # week...
-            field_name = (
-                "DATE_SUB(CAST(" + field_name + " AS DATE), INTERVAL 1 DAY)"
+        if USING_DJANGO_3:
+            return sql
+        return sql, params
+
+    if USING_DJANGO_3:
+
+        def date_trunc_sql(self, lookup_type, field_name, tzname=None):
+            """Truncate date in the lookup.
+
+            :type lookup_type: str
+            :param lookup_type: A type of the lookup.
+
+            :type field_name: str
+            :param field_name: The name of the field.
+
+            :type tzname: str
+            :param tzname: The name of the timezone. This is ignored because
+            Spanner does not support Timezone conversion in DATE_TRUNC function.
+
+            :rtype: str
+            :returns: A SQL statement for truncating.
+            """
+            # https://cloud.google.com/spanner/docs/functions-and-operators#date_trunc
+            if lookup_type == "week":
+                # Spanner truncates to Sunday but Django expects Monday. First,
+                # subtract a day so that a Sunday will be truncated to the previous
+                # week...
+                field_name = (
+                    "DATE_SUB(CAST("
+                    + field_name
+                    + " AS DATE), INTERVAL 1 DAY)"
+                )
+            sql = "DATE_TRUNC(CAST(%s AS DATE), %s)" % (
+                field_name,
+                lookup_type,
+            )
+            if lookup_type == "week":
+                # ...then add a day to get from Sunday to Monday.
+                sql = "DATE_ADD(CAST(" + sql + " AS DATE), INTERVAL 1 DAY)"
+            return sql
+
+    else:
+
+        def date_trunc_sql(self, lookup_type, field_name, params, tzname=None):
+            """Truncate date in the lookup.
+
+            :type lookup_type: str
+            :param lookup_type: A type of the lookup.
+
+            :type field_name: str
+            :param field_name: The name of the field.
+
+            :type params: list(str)
+            :param params: list of query params.
+
+            :type tzname: str
+            :param tzname: The name of the timezone. This is ignored because
+            Spanner does not support Timezone conversion in DATE_TRUNC function.
+
+            :rtype: str
+            :returns: A SQL statement for truncating.
+            """
+            # https://cloud.google.com/spanner/docs/functions-and-operators#date_trunc
+            if lookup_type == "week":
+                # Spanner truncates to Sunday but Django expects Monday. First,
+                # subtract a day so that a Sunday will be truncated to the previous
+                # week...
+                field_name = (
+                    "DATE_SUB(CAST("
+                    + field_name
+                    + " AS DATE), INTERVAL 1 DAY)"
+                )
+            sql = "DATE_TRUNC(CAST(%s AS DATE), %s)" % (
+                field_name,
+                lookup_type,
+            )
+            if lookup_type == "week":
+                # ...then add a day to get from Sunday to Monday.
+                sql = "DATE_ADD(CAST(" + sql + " AS DATE), INTERVAL 1 DAY)"
+            return sql, params
+
+    if USING_DJANGO_3:
+
+        def datetime_trunc_sql(self, lookup_type, field_name, tzname="UTC"):
+            """Truncate datetime in the lookup.
+
+            :type lookup_type: str
+            :param lookup_type: A type of the lookup.
+
+            :type field_name: str
+            :param field_name: The name of the field.
+
+            :type tzname: str
+            :param tzname: The name of the timezone.
+
+            :rtype: str
+            :returns: A SQL statement for truncating.
+            """
+            # https://cloud.google.com/spanner/docs/functions-and-operators#timestamp_trunc
+            tzname = tzname if settings.USE_TZ and tzname else "UTC"
+            if lookup_type == "week":
+                # Spanner truncates to Sunday but Django expects Monday. First,
+                # subtract a day so that a Sunday will be truncated to the previous
+                # week...
+                field_name = (
+                    "TIMESTAMP_SUB(" + field_name + ", INTERVAL 1 DAY)"
+                )
+            sql = 'TIMESTAMP_TRUNC(%s, %s, "%s")' % (
+                field_name,
+                lookup_type,
+                tzname,
+            )
+            if lookup_type == "week":
+                # ...then add a day to get from Sunday to Monday.
+                sql = "TIMESTAMP_ADD(" + sql + ", INTERVAL 1 DAY)"
+            return sql
+
+    else:
+
+        def datetime_trunc_sql(
+            self, lookup_type, field_name, params, tzname="UTC"
+        ):
+            """Truncate datetime in the lookup.
+
+            :type lookup_type: str
+            :param lookup_type: A type of the lookup.
+
+            :type field_name: str
+            :param field_name: The name of the field.
+
+            :type params: list(str)
+            :param params: list of query params.
+
+            :type tzname: str
+            :param tzname: The name of the timezone.
+
+            :rtype: str
+            :returns: A SQL statement for truncating.
+            """
+            # https://cloud.google.com/spanner/docs/functions-and-operators#timestamp_trunc
+            tzname = tzname if settings.USE_TZ and tzname else "UTC"
+            if lookup_type == "week":
+                # Spanner truncates to Sunday but Django expects Monday. First,
+                # subtract a day so that a Sunday will be truncated to the previous
+                # week...
+                field_name = (
+                    "TIMESTAMP_SUB(" + field_name + ", INTERVAL 1 DAY)"
+                )
+            sql = 'TIMESTAMP_TRUNC(%s, %s, "%s")' % (
+                field_name,
+                lookup_type,
+                tzname,
+            )
+            if lookup_type == "week":
+                # ...then add a day to get from Sunday to Monday.
+                sql = "TIMESTAMP_ADD(" + sql + ", INTERVAL 1 DAY)"
+            return sql, params
+
+    if USING_DJANGO_3:
+
+        def time_trunc_sql(self, lookup_type, field_name, tzname="UTC"):
+            """Truncate time in the lookup.
+
+            :type lookup_type: str
+            :param lookup_type: A type of the lookup.
+
+            :type field_name: str
+            :param field_name: The name of the field.
+
+            :type tzname: str
+            :param tzname: The name of the timezone. Defaults to 'UTC' For backward compatability.
+
+            :rtype: str
+            :returns: A SQL statement for truncating.
+            """
+            # https://cloud.google.com/spanner/docs/functions-and-operators#timestamp_trunc
+            tzname = tzname if settings.USE_TZ and tzname else "UTC"
+            return 'TIMESTAMP_TRUNC(%s, %s, "%s")' % (
+                field_name,
+                lookup_type,
+                tzname,
             )
-        sql = "DATE_TRUNC(CAST(%s AS DATE), %s)" % (field_name, lookup_type)
-        if lookup_type == "week":
-            # ...then add a day to get from Sunday to Monday.
-            sql = "DATE_ADD(CAST(" + sql + " AS DATE), INTERVAL 1 DAY)"
-        return sql
-
-    def datetime_trunc_sql(self, lookup_type, field_name, tzname="UTC"):
-        """Truncate datetime in the lookup.
-
-        :type lookup_type: str
-        :param lookup_type: A type of the lookup.
-
-        :type field_name: str
-        :param field_name: The name of the field.
-
-        :type tzname: str
-        :param tzname: The name of the timezone.
-
-        :rtype: str
-        :returns: A SQL statement for truncating.
-        """
-        # https://cloud.google.com/spanner/docs/functions-and-operators#timestamp_trunc
-        tzname = tzname if settings.USE_TZ and tzname else "UTC"
-        if lookup_type == "week":
-            # Spanner truncates to Sunday but Django expects Monday. First,
-            # subtract a day so that a Sunday will be truncated to the previous
-            # week...
-            field_name = "TIMESTAMP_SUB(" + field_name + ", INTERVAL 1 DAY)"
-        sql = 'TIMESTAMP_TRUNC(%s, %s, "%s")' % (
-            field_name,
-            lookup_type,
-            tzname,
-        )
-        if lookup_type == "week":
-            # ...then add a day to get from Sunday to Monday.
-            sql = "TIMESTAMP_ADD(" + sql + ", INTERVAL 1 DAY)"
-        return sql
-
-    def time_trunc_sql(self, lookup_type, field_name, tzname="UTC"):
-        """Truncate time in the lookup.
-
-        :type lookup_type: str
-        :param lookup_type: A type of the lookup.
-
-        :type field_name: str
-        :param field_name: The name of the field.
 
-        :type tzname: str
-        :param tzname: The name of the timezone. Defaults to 'UTC' For backward compatability.
+    else:
 
-        :rtype: str
-        :returns: A SQL statement for truncating.
-        """
-        # https://cloud.google.com/spanner/docs/functions-and-operators#timestamp_trunc
-        tzname = tzname if settings.USE_TZ and tzname else "UTC"
-        return 'TIMESTAMP_TRUNC(%s, %s, "%s")' % (
-            field_name,
-            lookup_type,
-            tzname,
-        )
+        def time_trunc_sql(
+            self, lookup_type, field_name, params, tzname="UTC"
+        ):
+            """Truncate time in the lookup.
+
+            :type lookup_type: str
+            :param lookup_type: A type of the lookup.
+
+            :type field_name: str
+            :param field_name: The name of the field.
+
+            :type params: list(str)
+            :param params: list of query params.
+
+            :type tzname: str
+            :param tzname: The name of the timezone. Defaults to 'UTC' For backward compatability.
+
+            :rtype: str
+            :returns: A SQL statement for truncating.
+            """
+            # https://cloud.google.com/spanner/docs/functions-and-operators#timestamp_trunc
+            tzname = tzname if settings.USE_TZ and tzname else "UTC"
+            return (
+                'TIMESTAMP_TRUNC(%s, %s, "%s")'
+                % (
+                    field_name,
+                    lookup_type,
+                    tzname,
+                ),
+                params,
+            )
 
-    def datetime_cast_date_sql(self, field_name, tzname):
-        """Cast date in the lookup.
+    if USING_DJANGO_3:
 
-        :type field_name: str
-        :param field_name: The name of the field.
+        def datetime_cast_date_sql(self, field_name, tzname):
+            """Cast date in the lookup.
 
-        :type tzname: str
-        :param tzname: The time zone name. If using of time zone is not
-                       allowed in settings default will be UTC.
+            :type field_name: str
+            :param field_name: The name of the field.
 
-        :rtype: str
-        :returns: A SQL statement for casting.
-        """
-        # https://cloud.google.com/spanner/docs/functions-and-operators#date
-        tzname = tzname if settings.USE_TZ and tzname else "UTC"
-        return 'DATE(%s, "%s")' % (field_name, tzname)
+            :type tzname: str
+            :param tzname: The time zone name. If using of time zone is not
+                           allowed in settings default will be UTC.
+
+            :rtype: str
+            :returns: A SQL statement for casting.
+            """
+            # https://cloud.google.com/spanner/docs/functions-and-operators#date
+            tzname = tzname if settings.USE_TZ and tzname else "UTC"
+            return 'DATE(%s, "%s")' % (field_name, tzname)
+
+    else:
+
+        def datetime_cast_date_sql(self, field_name, params, tzname):
+            """Cast date in the lookup.
+
+            :type field_name: str
+            :param field_name: The name of the field.
+
+            :type params: list(str)
+            :param params: list of query params.
+
+            :type tzname: str
+            :param tzname: The time zone name. If using of time zone is not
+                           allowed in settings default will be UTC.
+
+            :rtype: str
+            :returns: A SQL statement for casting.
+            """
+            # https://cloud.google.com/spanner/docs/functions-and-operators#date
+            tzname = tzname if settings.USE_TZ and tzname else "UTC"
+            return 'DATE(%s, "%s")' % (field_name, tzname), params
+
+    if USING_DJANGO_3:
+
+        def datetime_cast_time_sql(self, field_name, tzname):
+            """Cast time in the lookup.
+
+            :type field_name: str
+            :param field_name: The name of the field.
+
+            :type tzname: str
+            :param tzname: The time zone name. If using of time zone is not
+                           allowed in settings default will be UTC.
+
+            :rtype: str
+            :returns: A SQL statement for casting.
+            """
+            tzname = tzname if settings.USE_TZ and tzname else "UTC"
+            # Cloud Spanner doesn't have a function for converting
+            # TIMESTAMP to another time zone.
+            return (
+                "TIMESTAMP(FORMAT_TIMESTAMP("
+                "'%%Y-%%m-%%d %%R:%%E9S %%Z', %s, '%s'))"
+                % (field_name, tzname)
+            )
 
-    def datetime_cast_time_sql(self, field_name, tzname):
-        """Cast time in the lookup.
+    else:
 
-        :type field_name: str
-        :param field_name: The name of the field.
+        def datetime_cast_time_sql(self, field_name, params, tzname):
+            """Cast time in the lookup.
 
-        :type tzname: str
-        :param tzname: The time zone name. If using of time zone is not
-                       allowed in settings default will be UTC.
+            :type field_name: str
+            :param field_name: The name of the field.
 
-        :rtype: str
-        :returns: A SQL statement for casting.
-        """
-        tzname = tzname if settings.USE_TZ and tzname else "UTC"
-        # Cloud Spanner doesn't have a function for converting
-        # TIMESTAMP to another time zone.
-        return (
-            "TIMESTAMP(FORMAT_TIMESTAMP("
-            "'%%Y-%%m-%%d %%R:%%E9S %%Z', %s, '%s'))" % (field_name, tzname)
-        )
+            :type params: list(str)
+            :param params: list of query params.
+
+            :type tzname: str
+            :param tzname: The time zone name. If using of time zone is not
+                           allowed in settings default will be UTC.
+
+            :rtype: str
+            :returns: A SQL statement for casting.
+            """
+            tzname = tzname if settings.USE_TZ and tzname else "UTC"
+            # Cloud Spanner doesn't have a function for converting
+            # TIMESTAMP to another time zone.
+            return (
+                "TIMESTAMP(FORMAT_TIMESTAMP("
+                "'%%Y-%%m-%%d %%R:%%E9S %%Z', %s, '%s'))"
+                % (field_name, tzname)
+            ), params
 
     def date_interval_sql(self, timedelta):
         """Get a date interval in microseconds.
 
         :type timedelta: datetime
         :param timedelta: A time delta for the interval.
```

### Comparing `django-google-spanner-3.1.0/django_spanner/schema.py` & `django-google-spanner-4.0.1/django_spanner/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,22 +113,32 @@
             # Add the SQL to our big list
             column_sqls.append(
                 "%s %s" % (self.quote_name(field.column), definition)
             )
             # Create a unique constraint separately because Spanner doesn't
             # allow them inline on a column.
             if field.unique and not field.primary_key:
-                self.deferred_sql.append(
-                    self._create_unique_sql(model, [field.column])
-                )
+                if USING_DJANGO_3:
+                    self.deferred_sql.append(
+                        self._create_unique_sql(model, [field.column])
+                    )
+                else:
+                    self.deferred_sql.append(
+                        self._create_unique_sql(model, [field])
+                    )
 
         # Add any unique_togethers (always deferred, as some fields might be
         # created afterwards, like geometry fields with some backends)
         for fields in model._meta.unique_together:
-            columns = [model._meta.get_field(field).column for field in fields]
+            if USING_DJANGO_3:
+                columns = [
+                    model._meta.get_field(field).column for field in fields
+                ]
+            else:
+                columns = [model._meta.get_field(field) for field in fields]
             self.deferred_sql.append(self._create_unique_sql(model, columns))
         constraints = [
             constraint.constraint_sql(model, self)
             for constraint in model._meta.constraints
         ]
         # Make the table
         sql = self.sql_create_table % {
@@ -276,17 +286,22 @@
                 }
             )
         # Add an index, if required
         self.deferred_sql.extend(self._field_indexes_sql(model, field))
         # Create a unique constraint separately because Spanner doesn't allow
         # them inline on a column.
         if field.unique and not field.primary_key:
-            self.deferred_sql.append(
-                self._create_unique_sql(model, [field.column])
-            )
+            if USING_DJANGO_3:
+                self.deferred_sql.append(
+                    self._create_unique_sql(model, [field.column])
+                )
+            else:
+                self.deferred_sql.append(
+                    self._create_unique_sql(model, [field])
+                )
         # Add any FK constraints later
         if (
             field.remote_field
             and self.connection.features.supports_foreign_keys
             and field.db_constraint
         ):
             self.deferred_sql.append(
@@ -488,15 +503,23 @@
             with trace_call(
                 "CloudSpannerDjango.alter_field.recreate_index",
                 self.connection,
                 trace_attributes,
             ):
                 self.execute(self._create_index_sql(model, fields=[new_field]))
 
-    def _alter_column_type_sql(self, model, old_field, new_field, new_type):
+    def _alter_column_type_sql(
+        self,
+        model,
+        old_field,
+        new_field,
+        new_type,
+        old_collation=None,
+        new_collation=None,
+    ):
         # Spanner needs to use sql_alter_column_not_null if the field is
         # NOT NULL, otherwise the constraint is dropped.
         sql = (
             self.sql_alter_column_type
             if new_field.null
             else self.sql_alter_column_not_null
         )
@@ -526,28 +549,35 @@
         model,
         fields,
         name,
         condition=None,
         deferrable=None,  # Spanner does not require this parameter
         include=None,
         opclasses=None,
+        expressions=None,
     ):
         # Inline constraints aren't supported, so create the index separately.
         if USING_DJANGO_3:
             sql = self._create_unique_sql(
                 model,
                 fields,
                 name=name,
                 condition=condition,
                 include=include,
                 opclasses=opclasses,
             )
         else:
             sql = self._create_unique_sql(
-                model, fields, name=name, condition=condition
+                model,
+                fields,
+                name=name,
+                condition=condition,
+                include=include,
+                opclasses=opclasses,
+                expressions=expressions,
             )
         if sql:
             self.deferred_sql.append(sql)
         return None
 
     def skip_default(self, field):
         """Cloud Spanner doesn't support column defaults."""
```

### Comparing `django-google-spanner-3.1.0/django_spanner/utils.py` & `django-google-spanner-4.0.1/django_spanner/utils.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.1.0/setup.cfg` & `django-google-spanner-4.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.1.0/setup.py` & `django-google-spanner-4.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,20 +55,18 @@
     classifiers=[
         release_status,
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Topic :: Utilities",
         "Framework :: Django",
-        "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.2",
+        "Framework :: Django :: 4.2",
     ],
     extras_require=extras,
-    python_requires=">=3.6",
+    python_requires=">=3.8",
 )
```

### Comparing `django-google-spanner-3.1.0/tests/performance/django_spanner/test_benchmark.py` & `django-google-spanner-4.0.1/tests/performance/django_spanner/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.1.0/tests/system/django_spanner/models.py` & `django-google-spanner-4.0.1/tests/system/django_spanner/models.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.1.0/tests/system/django_spanner/test_check_constraint.py` & `django-google-spanner-4.0.1/tests/system/django_spanner/test_check_constraint.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.1.0/tests/system/django_spanner/test_decimal.py` & `django-google-spanner-4.0.1/tests/system/django_spanner/test_decimal.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.1.0/tests/system/django_spanner/test_json_field.py` & `django-google-spanner-4.0.1/tests/system/django_spanner/test_json_field.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.1.0/tests/system/django_spanner/test_queries.py` & `django-google-spanner-4.0.1/tests/system/django_spanner/test_queries.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.1.0/tests/system/django_spanner/utils.py` & `django-google-spanner-4.0.1/tests/system/django_spanner/utils.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.1.0/tests/unit/django_spanner/models.py` & `django-google-spanner-4.0.1/tests/unit/django_spanner/models.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.1.0/tests/unit/django_spanner/simple_test.py` & `django-google-spanner-4.0.1/tests/unit/django_spanner/simple_test.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.1.0/tests/unit/django_spanner/test__opentelemetry_tracing.py` & `django-google-spanner-4.0.1/tests/unit/django_spanner/test__opentelemetry_tracing.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.1.0/tests/unit/django_spanner/test_base.py` & `django-google-spanner-4.0.1/tests/unit/django_spanner/test_base.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.1.0/tests/unit/django_spanner/test_client.py` & `django-google-spanner-4.0.1/tests/unit/django_spanner/test_client.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.1.0/tests/unit/django_spanner/test_expressions.py` & `django-google-spanner-4.0.1/tests/unit/django_spanner/test_expressions.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.1.0/tests/unit/django_spanner/test_functions.py` & `django-google-spanner-4.0.1/tests/unit/django_spanner/test_functions.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.1.0/tests/unit/django_spanner/test_introspection.py` & `django-google-spanner-4.0.1/tests/unit/django_spanner/test_introspection.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,68 +83,41 @@
             return column_details
 
         cursor.get_table_column_schema = get_table_column_schema
         cursor.description = description()
         table_description = db_introspection.get_table_description(
             cursor=cursor, table_name="Table_1"
         )
-        if USING_DJANGO_3:
-            self.assertEqual(
-                table_description,
-                [
-                    FieldInfo(
-                        name="name",
-                        type_code=TypeCode.STRING,
-                        display_size=None,
-                        internal_size=10,
-                        precision=None,
-                        scale=None,
-                        null_ok=False,
-                        default=None,
-                        collation=None,
-                    ),
-                    FieldInfo(
-                        name="age",
-                        type_code=TypeCode.INT64,
-                        display_size=None,
-                        internal_size=None,
-                        precision=None,
-                        scale=None,
-                        null_ok=True,
-                        default=None,
-                        collation=None,
-                    ),
-                ],
-            )
-        else:
-            self.assertEqual(
-                table_description,
-                [
-                    FieldInfo(
-                        name="name",
-                        type_code=TypeCode.STRING,
-                        display_size=None,
-                        internal_size=10,
-                        precision=None,
-                        scale=None,
-                        null_ok=False,
-                        default=None,
-                    ),
-                    FieldInfo(
-                        name="age",
-                        type_code=TypeCode.INT64,
-                        display_size=None,
-                        internal_size=None,
-                        precision=None,
-                        scale=None,
-                        null_ok=True,
-                        default=None,
-                    ),
-                ],
-            )
+        self.assertEqual(
+            table_description,
+            [
+                FieldInfo(
+                    name="name",
+                    type_code=TypeCode.STRING,
+                    display_size=None,
+                    internal_size=10,
+                    precision=None,
+                    scale=None,
+                    null_ok=False,
+                    default=None,
+                    collation=None,
+                ),
+                FieldInfo(
+                    name="age",
+                    type_code=TypeCode.INT64,
+                    display_size=None,
+                    internal_size=None,
+                    precision=None,
+                    scale=None,
+                    null_ok=True,
+                    default=None,
+                    collation=None,
+                ),
+            ],
+        )
 
     def test_get_primary_key_column(self):
         """
         Tests get primary column of table.
         """
         db_introspection = DatabaseIntrospection(self.connection)
         cursor = mock.MagicMock()
```

### Comparing `django-google-spanner-3.1.0/tests/unit/django_spanner/test_lookups.py` & `django-google-spanner-4.0.1/tests/unit/django_spanner/test_lookups.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.1.0/tests/unit/django_spanner/test_operations.py` & `django-google-spanner-4.0.1/tests/unit/django_spanner/test_operations.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from base64 import b64encode
 from datetime import timedelta
 from decimal import Decimal
 from django.conf import settings
 from django.core.management.color import no_style
 from django.db.utils import DatabaseError
 from google.cloud.spanner_dbapi.types import DateStr
+
+from django_spanner import USING_DJANGO_3
 from tests.unit.django_spanner.simple_test import SpannerSimpleTestClass
 import uuid
 
 
 class TestOperations(SpannerSimpleTestClass):
     def test_max_name_length(self):
         self.assertEqual(self.db_operations.max_name_length(), 128)
@@ -107,75 +109,170 @@
         self.assertIsNone(
             self.db_operations.convert_uuidfield_value(
                 value=None, expression=None, connection=None
             ),
         )
 
     def test_date_extract_sql(self):
-        self.assertEqual(
-            self.db_operations.date_extract_sql("week", "dummy_field"),
-            "EXTRACT(isoweek FROM dummy_field)",
-        )
+        if USING_DJANGO_3:
+            self.assertEqual(
+                self.db_operations.date_extract_sql("week", "dummy_field"),
+                "EXTRACT(isoweek FROM dummy_field)",
+            )
+        else:
+            self.assertEqual(
+                self.db_operations.date_extract_sql("week", "dummy_field"),
+                ("EXTRACT(isoweek FROM dummy_field)", None),
+            )
 
     def test_date_extract_sql_lookup_type_dayofweek(self):
-        self.assertEqual(
-            self.db_operations.date_extract_sql("dayofweek", "dummy_field"),
-            "EXTRACT(dayofweek FROM dummy_field)",
-        )
+        if USING_DJANGO_3:
+            self.assertEqual(
+                self.db_operations.date_extract_sql(
+                    "dayofweek", "dummy_field"
+                ),
+                "EXTRACT(dayofweek FROM dummy_field)",
+            )
+        else:
+            self.assertEqual(
+                self.db_operations.date_extract_sql(
+                    "dayofweek", "dummy_field"
+                ),
+                ("EXTRACT(dayofweek FROM dummy_field)", None),
+            )
 
     def test_datetime_extract_sql(self):
         settings.USE_TZ = True
-        self.assertEqual(
-            self.db_operations.datetime_extract_sql(
-                "dayofweek", "dummy_field", "IST"
-            ),
-            'EXTRACT(dayofweek FROM dummy_field AT TIME ZONE "IST")',
-        )
+        if USING_DJANGO_3:
+            self.assertEqual(
+                self.db_operations.datetime_extract_sql(
+                    "dayofweek", "dummy_field", "IST"
+                ),
+                'EXTRACT(dayofweek FROM dummy_field AT TIME ZONE "IST")',
+            )
+        else:
+            self.assertEqual(
+                self.db_operations.datetime_extract_sql(
+                    "dayofweek", "dummy_field", None, "IST"
+                ),
+                (
+                    'EXTRACT(dayofweek FROM dummy_field AT TIME ZONE "IST")',
+                    None,
+                ),
+            )
 
     def test_datetime_extract_sql_use_tz_false(self):
         settings.USE_TZ = False
-        self.assertEqual(
-            self.db_operations.datetime_extract_sql(
-                "dayofweek", "dummy_field", "IST"
-            ),
-            'EXTRACT(dayofweek FROM dummy_field AT TIME ZONE "UTC")',
-        )
+        if USING_DJANGO_3:
+            self.assertEqual(
+                self.db_operations.datetime_extract_sql(
+                    "dayofweek", "dummy_field", "IST"
+                ),
+                'EXTRACT(dayofweek FROM dummy_field AT TIME ZONE "UTC")',
+            )
+        else:
+            self.assertEqual(
+                self.db_operations.datetime_extract_sql(
+                    "dayofweek", "dummy_field", None, "IST"
+                ),
+                (
+                    'EXTRACT(dayofweek FROM dummy_field AT TIME ZONE "UTC")',
+                    None,
+                ),
+            )
         settings.USE_TZ = True  # reset changes.
 
     def test_time_extract_sql(self):
-        self.assertEqual(
-            self.db_operations.time_extract_sql("dayofweek", "dummy_field"),
-            'EXTRACT(dayofweek FROM dummy_field AT TIME ZONE "UTC")',
-        )
+        if USING_DJANGO_3:
+            self.assertEqual(
+                self.db_operations.time_extract_sql(
+                    "dayofweek", "dummy_field"
+                ),
+                'EXTRACT(dayofweek FROM dummy_field AT TIME ZONE "UTC")',
+            )
+        else:
+            self.assertEqual(
+                self.db_operations.time_extract_sql(
+                    "dayofweek", "dummy_field"
+                ),
+                (
+                    'EXTRACT(dayofweek FROM dummy_field AT TIME ZONE "UTC")',
+                    None,
+                ),
+            )
 
     def test_time_trunc_sql(self):
-        self.assertEqual(
-            self.db_operations.time_trunc_sql("dayofweek", "dummy_field"),
-            'TIMESTAMP_TRUNC(dummy_field, dayofweek, "UTC")',
-        )
+        if USING_DJANGO_3:
+            self.assertEqual(
+                self.db_operations.time_trunc_sql("dayofweek", "dummy_field"),
+                'TIMESTAMP_TRUNC(dummy_field, dayofweek, "UTC")',
+            )
+        else:
+            self.assertEqual(
+                self.db_operations.time_trunc_sql(
+                    "dayofweek", "dummy_field", None
+                ),
+                ('TIMESTAMP_TRUNC(dummy_field, dayofweek, "UTC")', None),
+            )
 
     def test_datetime_cast_date_sql(self):
-        self.assertEqual(
-            self.db_operations.datetime_cast_date_sql("dummy_field", "IST"),
-            'DATE(dummy_field, "IST")',
-        )
+        if USING_DJANGO_3:
+            self.assertEqual(
+                self.db_operations.datetime_cast_date_sql(
+                    "dummy_field", "IST"
+                ),
+                'DATE(dummy_field, "IST")',
+            )
+        else:
+            self.assertEqual(
+                self.db_operations.datetime_cast_date_sql(
+                    "dummy_field", None, "IST"
+                ),
+                ('DATE(dummy_field, "IST")', None),
+            )
 
     def test_datetime_cast_time_sql(self):
         settings.USE_TZ = True
-        self.assertEqual(
-            self.db_operations.datetime_cast_time_sql("dummy_field", "IST"),
-            "TIMESTAMP(FORMAT_TIMESTAMP('%Y-%m-%d %R:%E9S %Z', dummy_field, 'IST'))",
-        )
+        if USING_DJANGO_3:
+            self.assertEqual(
+                self.db_operations.datetime_cast_time_sql(
+                    "dummy_field", "IST"
+                ),
+                "TIMESTAMP(FORMAT_TIMESTAMP('%Y-%m-%d %R:%E9S %Z', dummy_field, 'IST'))",
+            )
+        else:
+            self.assertEqual(
+                self.db_operations.datetime_cast_time_sql(
+                    "dummy_field", None, "IST"
+                ),
+                (
+                    "TIMESTAMP(FORMAT_TIMESTAMP('%Y-%m-%d %R:%E9S %Z', dummy_field, 'IST'))",
+                    None,
+                ),
+            )
 
     def test_datetime_cast_time_sql_use_tz_false(self):
         settings.USE_TZ = False
-        self.assertEqual(
-            self.db_operations.datetime_cast_time_sql("dummy_field", "IST"),
-            "TIMESTAMP(FORMAT_TIMESTAMP('%Y-%m-%d %R:%E9S %Z', dummy_field, 'UTC'))",
-        )
+        if USING_DJANGO_3:
+            self.assertEqual(
+                self.db_operations.datetime_cast_time_sql(
+                    "dummy_field", "IST"
+                ),
+                "TIMESTAMP(FORMAT_TIMESTAMP('%Y-%m-%d %R:%E9S %Z', dummy_field, 'UTC'))",
+            )
+        else:
+            self.assertEqual(
+                self.db_operations.datetime_cast_time_sql(
+                    "dummy_field", None, "IST"
+                ),
+                (
+                    "TIMESTAMP(FORMAT_TIMESTAMP('%Y-%m-%d %R:%E9S %Z', dummy_field, 'UTC'))",
+                    None,
+                ),
+            )
         settings.USE_TZ = True  # reset changes.
 
     def test_date_interval_sql(self):
         self.assertEqual(
             self.db_operations.date_interval_sql(timedelta(days=1)),
             "INTERVAL 86400000000 MICROSECOND",
         )
```

### Comparing `django-google-spanner-3.1.0/tests/unit/django_spanner/test_schema.py` & `django-google-spanner-4.0.1/tests/unit/django_spanner/test_schema.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.1.0/tests/unit/django_spanner/test_utils.py` & `django-google-spanner-4.0.1/tests/unit/django_spanner/test_utils.py`

 * *Files identical despite different names*

