# Comparing `tmp/nbrisk-35.1.3.tar.gz` & `tmp/nbrisk-40.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbrisk-35.1.3.tar", last modified: Tue Apr 23 00:14:45 2024, max compression
+gzip compressed data, was "nbrisk-40.0.1.tar", last modified: Mon May  6 23:32:09 2024, max compression
```

## Comparing `nbrisk-35.1.3.tar` & `nbrisk-40.0.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-23 00:14:45.415381 nbrisk-35.1.3/
--rw-rw-r--   0 renato    (1000) renato    (1000)    10174 2022-08-15 01:26:39.000000 nbrisk-35.1.3/LICENSE
--rw-rw-r--   0 renato    (1000) renato    (1000)       43 2022-08-15 01:38:51.000000 nbrisk-35.1.3/MANIFEST.in
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-23 00:14:45.415381 nbrisk-35.1.3/NbRisk.egg-info/
--rw-r--r--   0 renato    (1000) renato    (1000)     3209 2024-04-23 00:14:45.000000 nbrisk-35.1.3/NbRisk.egg-info/PKG-INFO
--rw-rw-r--   0 renato    (1000) renato    (1000)     2191 2024-04-23 00:14:45.000000 nbrisk-35.1.3/NbRisk.egg-info/SOURCES.txt
--rw-rw-r--   0 renato    (1000) renato    (1000)        1 2024-04-23 00:14:45.000000 nbrisk-35.1.3/NbRisk.egg-info/dependency_links.txt
--rw-rw-r--   0 renato    (1000) renato    (1000)        8 2024-04-23 00:14:45.000000 nbrisk-35.1.3/NbRisk.egg-info/top_level.txt
--rw-r--r--   0 renato    (1000) renato    (1000)     3209 2024-04-23 00:14:45.415381 nbrisk-35.1.3/PKG-INFO
--rw-rw-r--   0 renato    (1000) renato    (1000)     2780 2024-04-05 18:53:39.000000 nbrisk-35.1.3/README.md
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-23 00:14:45.403381 nbrisk-35.1.3/nb_risk/
--rw-rw-r--   0 renato    (1000) renato    (1000)      738 2024-04-22 23:55:34.000000 nbrisk-35.1.3/nb_risk/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      222 2023-01-19 18:35:20.000000 nbrisk-35.1.3/nb_risk/admin.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-23 00:14:45.403381 nbrisk-35.1.3/nb_risk/api/
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 nbrisk-35.1.3/nb_risk/api/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     1467 2024-04-22 02:10:22.000000 nbrisk-35.1.3/nb_risk/api/nested_serializers.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     5376 2024-04-22 02:09:48.000000 nbrisk-35.1.3/nb_risk/api/serializers.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      489 2023-04-21 01:34:23.000000 nbrisk-35.1.3/nb_risk/api/urls.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     1179 2023-04-21 01:34:15.000000 nbrisk-35.1.3/nb_risk/api/views.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     3213 2023-04-21 01:04:22.000000 nbrisk-35.1.3/nb_risk/choices.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     2108 2024-04-22 01:37:47.000000 nbrisk-35.1.3/nb_risk/columns.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     4220 2024-04-22 23:56:18.000000 nbrisk-35.1.3/nb_risk/cve.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     1975 2024-04-22 01:37:47.000000 nbrisk-35.1.3/nb_risk/filters.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     8322 2024-04-23 00:02:09.000000 nbrisk-35.1.3/nb_risk/forms.py
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 nbrisk-35.1.3/nb_risk/middleware.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-23 00:14:45.407381 nbrisk-35.1.3/nb_risk/migrations/
--rw-r--r--   0 renato    (1000) renato    (1000)     6544 2023-01-25 19:11:25.000000 nbrisk-35.1.3/nb_risk/migrations/0001_initial.py
--rw-r--r--   0 renato    (1000) renato    (1000)     1558 2023-04-21 00:03:25.000000 nbrisk-35.1.3/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py
--rw-r--r--   0 renato    (1000) renato    (1000)     1391 2023-04-21 01:36:32.000000 nbrisk-35.1.3/nb_risk/migrations/0003_control.py
--rw-r--r--   0 renato    (1000) renato    (1000)      394 2023-05-10 13:39:08.000000 nbrisk-35.1.3/nb_risk/migrations/0004_alter_vulnerability_options.py
--rw-r--r--   0 renato    (1000) renato    (1000)      434 2023-05-13 16:13:09.000000 nbrisk-35.1.3/nb_risk/migrations/0005_alter_vulnerability_cvssbasescore.py
--rw-r--r--   0 renato    (1000) renato    (1000)      424 2023-05-13 17:11:12.000000 nbrisk-35.1.3/nb_risk/migrations/0006_vulnerability_unique_vuln_name.py
--rw-r--r--   0 renato    (1000) renato    (1000)      615 2023-08-20 02:18:04.000000 nbrisk-35.1.3/nb_risk/migrations/0007_remove_vulnerability_unique_vuln_name_and_more.py
--rw-r--r--   0 renato    (1000) renato    (1000)        0 2023-01-25 19:11:25.000000 nbrisk-35.1.3/nb_risk/migrations/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     8712 2023-08-20 02:17:50.000000 nbrisk-35.1.3/nb_risk/models.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     4078 2024-04-22 01:37:47.000000 nbrisk-35.1.3/nb_risk/navigation.py
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2024-04-08 01:05:57.000000 nbrisk-35.1.3/nb_risk/signals.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     4050 2024-04-22 01:37:47.000000 nbrisk-35.1.3/nb_risk/tables.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      803 2024-04-22 01:37:47.000000 nbrisk-35.1.3/nb_risk/template_content.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-23 00:14:45.395382 nbrisk-35.1.3/nb_risk/templates/
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-23 00:14:45.415381 nbrisk-35.1.3/nb_risk/templates/nb_risk/
--rw-rw-r--   0 renato    (1000) renato    (1000)     1199 2023-05-12 19:59:37.000000 nbrisk-35.1.3/nb_risk/templates/nb_risk/control.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      235 2023-05-12 19:59:37.000000 nbrisk-35.1.3/nb_risk/templates/nb_risk/control_assets.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      235 2023-05-12 19:59:37.000000 nbrisk-35.1.3/nb_risk/templates/nb_risk/control_risks.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      667 2023-01-19 19:51:37.000000 nbrisk-35.1.3/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      269 2023-01-19 18:13:59.000000 nbrisk-35.1.3/nb_risk/templates/nb_risk/generic_vulnerability_list.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     2087 2023-01-25 21:22:56.000000 nbrisk-35.1.3/nb_risk/templates/nb_risk/risk.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     1939 2023-05-12 19:59:37.000000 nbrisk-35.1.3/nb_risk/templates/nb_risk/threatevent.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      233 2023-05-12 19:59:37.000000 nbrisk-35.1.3/nb_risk/templates/nb_risk/threatevent_vulnerabilities.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     1694 2023-04-02 19:40:16.000000 nbrisk-35.1.3/nb_risk/templates/nb_risk/threatsource.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     2455 2023-05-12 19:59:37.000000 nbrisk-35.1.3/nb_risk/templates/nb_risk/vulnerability.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      233 2023-05-12 19:59:37.000000 nbrisk-35.1.3/nb_risk/templates/nb_risk/vulnerability_affected_assets.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      296 2023-01-25 01:39:38.000000 nbrisk-35.1.3/nb_risk/templates/nb_risk/vulnerability_assignment_button.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      236 2023-02-16 01:36:47.000000 nbrisk-35.1.3/nb_risk/templates/nb_risk/vulnerability_list.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     1473 2024-04-22 01:37:47.000000 nbrisk-35.1.3/nb_risk/templates/nb_risk/vulnerability_search.html
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-23 00:14:45.415381 nbrisk-35.1.3/nb_risk/tests/
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2024-03-23 00:49:42.000000 nbrisk-35.1.3/nb_risk/tests/__init__.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-23 00:14:45.415381 nbrisk-35.1.3/nb_risk/tests/control/
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2024-03-23 01:01:28.000000 nbrisk-35.1.3/nb_risk/tests/control/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     1133 2024-03-23 00:50:09.000000 nbrisk-35.1.3/nb_risk/tests/custom.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-23 00:14:45.415381 nbrisk-35.1.3/nb_risk/tests/threatsource/
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2024-03-23 01:01:12.000000 nbrisk-35.1.3/nb_risk/tests/threatsource/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     1900 2024-04-22 01:37:47.000000 nbrisk-35.1.3/nb_risk/tests/threatsource/test_api.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     2158 2024-04-22 01:37:47.000000 nbrisk-35.1.3/nb_risk/tests/threatsource/test_filters.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     2359 2024-04-22 01:37:47.000000 nbrisk-35.1.3/nb_risk/tests/threatsource/test_views.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-23 00:14:45.415381 nbrisk-35.1.3/nb_risk/tests/vulnerability/
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2024-04-05 18:16:40.000000 nbrisk-35.1.3/nb_risk/tests/vulnerability/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     1809 2024-04-22 01:37:47.000000 nbrisk-35.1.3/nb_risk/tests/vulnerability/test_filters.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     1982 2024-04-22 01:37:47.000000 nbrisk-35.1.3/nb_risk/tests/vulnerability/test_views.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-23 00:14:45.415381 nbrisk-35.1.3/nb_risk/tests/vulnerabilityassignment/
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2024-04-22 01:58:26.000000 nbrisk-35.1.3/nb_risk/tests/vulnerabilityassignment/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     3510 2024-04-22 01:53:41.000000 nbrisk-35.1.3/nb_risk/tests/vulnerabilityassignment/test_api.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     4945 2024-04-23 00:03:14.000000 nbrisk-35.1.3/nb_risk/urls.py
--rw-rw-r--   0 renato    (1000) renato    (1000)       23 2024-04-23 00:10:49.000000 nbrisk-35.1.3/nb_risk/version.py
--rw-rw-r--   0 renato    (1000) renato    (1000)    11769 2024-04-22 23:59:41.000000 nbrisk-35.1.3/nb_risk/views.py
--rw-rw-r--   0 renato    (1000) renato    (1000)       38 2024-04-23 00:14:45.415381 nbrisk-35.1.3/setup.cfg
--rw-rw-r--   0 renato    (1000) renato    (1000)     1195 2023-01-19 04:15:27.000000 nbrisk-35.1.3/setup.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-05-06 23:32:09.678556 nbrisk-40.0.1/
+-rw-rw-r--   0 renato    (1000) renato    (1000)    10174 2022-08-15 01:26:39.000000 nbrisk-40.0.1/LICENSE
+-rw-rw-r--   0 renato    (1000) renato    (1000)       43 2022-08-15 01:38:51.000000 nbrisk-40.0.1/MANIFEST.in
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-05-06 23:32:09.678556 nbrisk-40.0.1/NbRisk.egg-info/
+-rw-r--r--   0 renato    (1000) renato    (1000)     3209 2024-05-06 23:32:09.000000 nbrisk-40.0.1/NbRisk.egg-info/PKG-INFO
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2194 2024-05-06 23:32:09.000000 nbrisk-40.0.1/NbRisk.egg-info/SOURCES.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)        1 2024-05-06 23:32:09.000000 nbrisk-40.0.1/NbRisk.egg-info/dependency_links.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)        8 2024-05-06 23:32:09.000000 nbrisk-40.0.1/NbRisk.egg-info/top_level.txt
+-rw-r--r--   0 renato    (1000) renato    (1000)     3209 2024-05-06 23:32:09.678556 nbrisk-40.0.1/PKG-INFO
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2780 2024-04-05 18:53:39.000000 nbrisk-40.0.1/README.md
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-05-06 23:32:09.666556 nbrisk-40.0.1/nb_risk/
+-rw-rw-r--   0 renato    (1000) renato    (1000)      738 2024-05-06 23:03:16.000000 nbrisk-40.0.1/nb_risk/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      222 2023-01-19 18:35:20.000000 nbrisk-40.0.1/nb_risk/admin.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-05-06 23:32:09.670556 nbrisk-40.0.1/nb_risk/api/
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 nbrisk-40.0.1/nb_risk/api/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1008 2024-05-06 23:02:32.000000 nbrisk-40.0.1/nb_risk/api/nested_serializers.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     5560 2024-05-06 23:02:32.000000 nbrisk-40.0.1/nb_risk/api/serializers.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      489 2023-04-21 01:34:23.000000 nbrisk-40.0.1/nb_risk/api/urls.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1179 2023-04-21 01:34:15.000000 nbrisk-40.0.1/nb_risk/api/views.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3213 2023-04-21 01:04:22.000000 nbrisk-40.0.1/nb_risk/choices.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2313 2024-05-06 23:02:32.000000 nbrisk-40.0.1/nb_risk/columns.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     4212 2024-05-06 23:02:32.000000 nbrisk-40.0.1/nb_risk/cve.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2020 2024-05-06 23:02:32.000000 nbrisk-40.0.1/nb_risk/filtersets.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     8369 2024-05-06 23:02:32.000000 nbrisk-40.0.1/nb_risk/forms.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 nbrisk-40.0.1/nb_risk/middleware.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-05-06 23:32:09.670556 nbrisk-40.0.1/nb_risk/migrations/
+-rw-r--r--   0 renato    (1000) renato    (1000)     6544 2023-01-25 19:11:25.000000 nbrisk-40.0.1/nb_risk/migrations/0001_initial.py
+-rw-r--r--   0 renato    (1000) renato    (1000)     1558 2023-04-21 00:03:25.000000 nbrisk-40.0.1/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py
+-rw-r--r--   0 renato    (1000) renato    (1000)     1391 2023-04-21 01:36:32.000000 nbrisk-40.0.1/nb_risk/migrations/0003_control.py
+-rw-r--r--   0 renato    (1000) renato    (1000)      394 2023-05-10 13:39:08.000000 nbrisk-40.0.1/nb_risk/migrations/0004_alter_vulnerability_options.py
+-rw-r--r--   0 renato    (1000) renato    (1000)      434 2023-05-13 16:13:09.000000 nbrisk-40.0.1/nb_risk/migrations/0005_alter_vulnerability_cvssbasescore.py
+-rw-r--r--   0 renato    (1000) renato    (1000)      424 2023-05-13 17:11:12.000000 nbrisk-40.0.1/nb_risk/migrations/0006_vulnerability_unique_vuln_name.py
+-rw-r--r--   0 renato    (1000) renato    (1000)      615 2023-08-20 02:18:04.000000 nbrisk-40.0.1/nb_risk/migrations/0007_remove_vulnerability_unique_vuln_name_and_more.py
+-rw-r--r--   0 renato    (1000) renato    (1000)        0 2023-01-25 19:11:25.000000 nbrisk-40.0.1/nb_risk/migrations/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     8712 2023-08-20 02:17:50.000000 nbrisk-40.0.1/nb_risk/models.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     4071 2024-05-06 23:02:32.000000 nbrisk-40.0.1/nb_risk/navigation.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2024-04-08 01:05:57.000000 nbrisk-40.0.1/nb_risk/signals.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3686 2024-05-06 23:02:32.000000 nbrisk-40.0.1/nb_risk/tables.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      803 2024-05-06 23:02:32.000000 nbrisk-40.0.1/nb_risk/template_content.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-05-06 23:32:09.658556 nbrisk-40.0.1/nb_risk/templates/
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-05-06 23:32:09.674556 nbrisk-40.0.1/nb_risk/templates/nb_risk/
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1199 2023-05-12 19:59:37.000000 nbrisk-40.0.1/nb_risk/templates/nb_risk/control.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      235 2023-05-12 19:59:37.000000 nbrisk-40.0.1/nb_risk/templates/nb_risk/control_assets.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      235 2023-05-12 19:59:37.000000 nbrisk-40.0.1/nb_risk/templates/nb_risk/control_risks.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      667 2023-01-19 19:51:37.000000 nbrisk-40.0.1/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      269 2023-01-19 18:13:59.000000 nbrisk-40.0.1/nb_risk/templates/nb_risk/generic_vulnerability_list.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2087 2023-01-25 21:22:56.000000 nbrisk-40.0.1/nb_risk/templates/nb_risk/risk.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1939 2023-05-12 19:59:37.000000 nbrisk-40.0.1/nb_risk/templates/nb_risk/threatevent.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      233 2023-05-12 19:59:37.000000 nbrisk-40.0.1/nb_risk/templates/nb_risk/threatevent_vulnerabilities.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1694 2023-04-02 19:40:16.000000 nbrisk-40.0.1/nb_risk/templates/nb_risk/threatsource.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2455 2023-05-12 19:59:37.000000 nbrisk-40.0.1/nb_risk/templates/nb_risk/vulnerability.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      233 2023-05-12 19:59:37.000000 nbrisk-40.0.1/nb_risk/templates/nb_risk/vulnerability_affected_assets.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      296 2023-01-25 01:39:38.000000 nbrisk-40.0.1/nb_risk/templates/nb_risk/vulnerability_assignment_button.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      236 2023-02-16 01:36:47.000000 nbrisk-40.0.1/nb_risk/templates/nb_risk/vulnerability_list.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1513 2024-05-06 23:02:32.000000 nbrisk-40.0.1/nb_risk/templates/nb_risk/vulnerability_search.html
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-05-06 23:32:09.674556 nbrisk-40.0.1/nb_risk/tests/
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2024-03-23 00:49:42.000000 nbrisk-40.0.1/nb_risk/tests/__init__.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-05-06 23:32:09.674556 nbrisk-40.0.1/nb_risk/tests/control/
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2024-03-23 01:01:28.000000 nbrisk-40.0.1/nb_risk/tests/control/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1133 2024-03-23 00:50:09.000000 nbrisk-40.0.1/nb_risk/tests/custom.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-05-06 23:32:09.674556 nbrisk-40.0.1/nb_risk/tests/threatsource/
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2024-03-23 01:01:12.000000 nbrisk-40.0.1/nb_risk/tests/threatsource/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1917 2024-05-06 23:02:32.000000 nbrisk-40.0.1/nb_risk/tests/threatsource/test_api.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2161 2024-05-06 23:02:32.000000 nbrisk-40.0.1/nb_risk/tests/threatsource/test_filters.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2364 2024-05-06 23:02:32.000000 nbrisk-40.0.1/nb_risk/tests/threatsource/test_views.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-05-06 23:32:09.678556 nbrisk-40.0.1/nb_risk/tests/vulnerability/
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2024-04-05 18:16:40.000000 nbrisk-40.0.1/nb_risk/tests/vulnerability/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1812 2024-05-06 23:02:32.000000 nbrisk-40.0.1/nb_risk/tests/vulnerability/test_filters.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1988 2024-05-06 23:02:32.000000 nbrisk-40.0.1/nb_risk/tests/vulnerability/test_views.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-05-06 23:32:09.678556 nbrisk-40.0.1/nb_risk/tests/vulnerabilityassignment/
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2024-04-22 01:58:26.000000 nbrisk-40.0.1/nb_risk/tests/vulnerabilityassignment/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3510 2024-04-22 01:53:41.000000 nbrisk-40.0.1/nb_risk/tests/vulnerabilityassignment/test_api.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     4950 2024-05-06 23:02:32.000000 nbrisk-40.0.1/nb_risk/urls.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)       23 2024-05-06 23:23:18.000000 nbrisk-40.0.1/nb_risk/version.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)    12059 2024-05-06 23:02:32.000000 nbrisk-40.0.1/nb_risk/views.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)       38 2024-05-06 23:32:09.678556 nbrisk-40.0.1/setup.cfg
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1195 2023-01-19 04:15:27.000000 nbrisk-40.0.1/setup.py
```

### Comparing `nbrisk-35.1.3/LICENSE` & `nbrisk-40.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nbrisk-35.1.3/NbRisk.egg-info/PKG-INFO` & `nbrisk-40.0.1/NbRisk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NbRisk
-Version: 35.1.3
+Version: 40.0.1
 Summary: NIST 800-30 Risk Management for Netbox
 Home-page: https://github.com/renatoalmeidaoliveira/nbrisk
 Author: Renato Almdida Oliveira
 Author-email: renato.almeida.oliveira@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nbrisk-35.1.3/NbRisk.egg-info/SOURCES.txt` & `nbrisk-40.0.1/NbRisk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 NbRisk.egg-info/dependency_links.txt
 NbRisk.egg-info/top_level.txt
 nb_risk/__init__.py
 nb_risk/admin.py
 nb_risk/choices.py
 nb_risk/columns.py
 nb_risk/cve.py
-nb_risk/filters.py
+nb_risk/filtersets.py
 nb_risk/forms.py
 nb_risk/middleware.py
 nb_risk/models.py
 nb_risk/navigation.py
 nb_risk/signals.py
 nb_risk/tables.py
 nb_risk/template_content.py
```

### Comparing `nbrisk-35.1.3/PKG-INFO` & `nbrisk-40.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NbRisk
-Version: 35.1.3
+Version: 40.0.1
 Summary: NIST 800-30 Risk Management for Netbox
 Home-page: https://github.com/renatoalmeidaoliveira/nbrisk
 Author: Renato Almdida Oliveira
 Author-email: renato.almeida.oliveira@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nbrisk-35.1.3/README.md` & `nbrisk-40.0.1/README.md`

 * *Files identical despite different names*

### Comparing `nbrisk-35.1.3/nb_risk/__init__.py` & `nbrisk-40.0.1/nb_risk/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from extras.plugins import PluginConfig
+from netbox.plugins import PluginConfig
 from .version import __version__
 
 
+
 class NbriskConfig(PluginConfig):
     name = "nb_risk"
     base_url = "nb_risk"
     verbose_name = "Risk Management"
     description = "NIST 800-30 Risk Management for Netbox"
     version = __version__
     author = "Renato Almdida Oliveira"
     author_email = "renato.almeida.oliveira@gmail.com"
-    min_version = "3.5.0"
-    max_version = "3.7.99"
+    min_version = "4.0.0"
+    max_version = "4.0.99"
     required_settings = []
     default_settings = {
         "supported_assets": [
             "dcim.device",
             "virtualization.virtualmachine",
             "tenancy.tenant",
             "dcim.site",
         ],
         "additional_assets": [],
         "proxies": {},
     }
 
-
 config = NbriskConfig  # noqa
```

### Comparing `nbrisk-35.1.3/nb_risk/api/nested_serializers.py` & `nbrisk-40.0.1/nb_risk/api/nested_serializers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,34 @@
 from rest_framework import serializers
 
 from netbox.api.serializers import WritableNestedSerializer
 from .. import models, choices
 
 # ThreatSource Nested Serializers
 
-class NestedThreatSourceSerializer(WritableNestedSerializer):
-    url = serializers.HyperlinkedIdentityField(
-        view_name="plugins-api:nb_risk-api:threatsource-detail"
-    )
-    display = serializers.SerializerMethodField('get_display')
+# class NestedThreatSourceSerializer(WritableNestedSerializer):
+#     url = serializers.HyperlinkedIdentityField(
+#         view_name="plugins-api:nb_risk-api:threatsource-detail"
+#     )
+#     display = serializers.SerializerMethodField('get_display')
     
-    def get_display(self, obj):
-        return obj.name
+#     def get_display(self, obj):
+#         return obj.name
 
-    class Meta:
-        model = models.ThreatSource
-        fields = ["id", "url", "display", "name"]
+#     class Meta:
+#         model = models.ThreatSource
+#         fields = ["id", "url", "display", "name"]
     
 # Risk Nested Serializers
 
 class NestedRiskSerializer(WritableNestedSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name="plugins-api:nb_risk-api:risk-detail"
     )
     display = serializers.SerializerMethodField('get_display')
     
     def get_display(self, obj):
         return obj.name
 
     class Meta:
         model = models.Risk
-        fields = ["id", "url", "display", "name"]
-
-# VulnerabilityAssignment Nested Serializers
-
-class NestedVulnerabilityAssignmentSerializer(WritableNestedSerializer):
-    url = serializers.HyperlinkedIdentityField(
-        view_name="plugins-api:nb_risk-api:vulnerabilityassignment-detail"
-    )
-    display = serializers.SerializerMethodField('get_display')
-    
-    def get_display(self, obj):
-        return obj.name
-
-    class Meta:
-        model = models.VulnerabilityAssignment
-        fields = ["id", "url", "display"]
+        fields = ["id", "url", "display", "name"]
```

### Comparing `nbrisk-35.1.3/nb_risk/api/serializers.py` & `nbrisk-40.0.1/nb_risk/api/serializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 from netbox.api.fields import ChoiceField, ContentTypeField, SerializedPKRelatedField
 from netbox.api.serializers import WritableNestedSerializer
 from utilities.api import get_serializer_for_model
 
 
 from netbox.api.serializers import NetBoxModelSerializer
 from nb_risk.api.nested_serializers import (
-    NestedThreatSourceSerializer,
     NestedRiskSerializer,
-    NestedVulnerabilityAssignmentSerializer,
 )
 from .. import models, choices
 
 # ThreatSource Serializers
 
 class ThreatSourceSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:nb_risk-api:threatsource-detail")
@@ -33,14 +31,15 @@
             "name",
             "threat_type",
             "capability",
             "intent",
             "targeting",
             "description",
         ]
+        brief_fields = ['id', 'url', 'display', 'name', 'description']
 
 # ThreatEvent Serializers
 
 class ThreatEventSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:nb_risk-api:threatevent-detail")
     display = serializers.SerializerMethodField('get_display')
     threat_source = serializers.SlugRelatedField(slug_field="name", queryset=models.ThreatSource.objects.all())
@@ -61,14 +60,16 @@
             "threat_source",
             "relevance",
             "likelihood",
             "impact",
             "vulnerability",
         ]
 
+        brief_fields = ['id', 'url', 'display', 'name', 'description']
+
 # Vulnerability Serializers
 
 class VulnerabilitySerializer(NetBoxModelSerializer):
     
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:nb_risk-api:vulnerability-detail")
     display = serializers.SerializerMethodField('get_display')
 
@@ -82,14 +83,16 @@
             "url",
             "display",
             "name",
             "cve",
             "description",
         ]
 
+        brief_fields = ['id', 'url', 'display', 'name', 'description']
+
 
 # VulnerabilityAssignment Serializers
 
 class VulnerabilityAssignmentSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:nb_risk-api:vulnerabilityassignment-detail")
     display = serializers.SerializerMethodField('get_display')
     asset_object_type = ContentTypeField(
@@ -126,14 +129,15 @@
             "url",
             "display",
             "asset_object_type",
             "asset_id",
             "asset",
             "vulnerability",
         ]
+        brief_fields = ['id', 'url', 'display']
 
 # Risk Serializers
 
 class RiskSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:nb_risk-api:risk-detail")
     display = serializers.SerializerMethodField('get_display')
```

### Comparing `nbrisk-35.1.3/nb_risk/api/views.py` & `nbrisk-40.0.1/nb_risk/api/views.py`

 * *Files identical despite different names*

### Comparing `nbrisk-35.1.3/nb_risk/choices.py` & `nbrisk-40.0.1/nb_risk/choices.py`

 * *Files identical despite different names*

### Comparing `nbrisk-35.1.3/nb_risk/columns.py` & `nbrisk-40.0.1/nb_risk/columns.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,27 +34,33 @@
             availabilityImpact = record["availabilityImpact"]
         else:
             availabilityImpact = ""
         if "baseScore" in record:
             baseScore = record["baseScore"]
         else:
             baseScore = ""
-
+        if "return_url" in record:
+            return_url = record["return_url"]
+        else:
+            return_url = None
 
         url = reverse("plugins:nb_risk:vulnerability_add")
         query = {
             "cve": cve,
             "notes": description,
             "name": cve,
             "cvssaccessVector": accessVector,
             "cvssaccessComplexity": accessComplexity,
             "cvssauthentication": authentication,
             "cvssconfidentialityImpact": confidentialityImpact,
             "cvssintegrityImpact": integrityImpact,
             "cvssavailabilityImpact": availabilityImpact,
             "cvssbaseScore": baseScore,
         }
+        if return_url:
+            query["return_url"] = return_url
+            
         encoded_query = urlencode(query)
         url = f"{url}?{encoded_query}"
 
         html = f'<a href={url} class="btn btn-primary btn-sm"><i class="mdi mdi-plus" aria-hidden="true"></i></a>'
         return mark_safe(html)
```

### Comparing `nbrisk-35.1.3/nb_risk/cve.py` & `nbrisk-40.0.1/nb_risk/cve.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from netbox.plugins.utils import get_plugin_config
 from dcim.models import Device, Site, DeviceType
 from tenancy.models import Tenant
 from virtualization.models import VirtualMachine
-from extras.plugins.utils import get_plugin_config
+
 from utilities.views import ViewTab, register_model_view
 from django.contrib.contenttypes.models import ContentType
 from django.shortcuts import get_object_or_404
 
 from django.views.generic import View
 from django.shortcuts import redirect, render
 
@@ -13,15 +14,15 @@
 from utilities.permissions import get_permission_for_model
 
 import logging
 import requests
 
 logger = logging.getLogger(__name__)
 
-from . import forms, models, tables, filters
+from . import forms, models, tables
 
 # Vulnerability Search Views
 
 
 class VulnerabilitySearchView(ObjectPermissionRequiredMixin, View):
     queryset = models.Vulnerability.objects.all()
     template_name = "nb_risk/vulnerability_search.html"
@@ -43,15 +44,14 @@
                 "tab": self.tab,
                 "cves": cves,
                 "filter_form": self.filterset_form,
                 "table": table,
             },
         )
 
-
 def get_query(request):
     if request.GET.get("cpe") is not None:
         return {
             "URI" : "https://services.nvd.nist.gov/rest/json/cpes/2.0",
             "payload":  {"cpeName": request.GET.get("cpe") } 
         }
     elif request.GET.get("cve") is not None:
@@ -111,8 +111,8 @@
                             cve[attribute] = ""
             return_url = f"{request.path}?{request.META['QUERY_STRING']}"
             cve["return_url"] = return_url
             output.append(cve)
         return output
     except Exception as e:
         print(e)
-        return []
+        return []
```

### Comparing `nbrisk-35.1.3/nb_risk/filters.py` & `nbrisk-40.0.1/nb_risk/filtersets.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # ThreatSource Filters
 
 
 class ThreatSourceFilterSet(NetBoxModelFilterSet):
     class Meta:
         model = models.ThreatSource
-        fields = ["id", "name", "threat_type", "capability", "intent", "targeting"]
+        fields = ["id", "name", "threat_type", "capability", "intent", "targeting", "description", "notes"]
 
 
 # ThreatEvent Filters
 
 
 class ThreatEventFilterSet(NetBoxModelFilterSet):
     class Meta:
@@ -29,14 +29,15 @@
     class Meta:
         model = models.Vulnerability
         fields = [
             "id",
             "name",
             "cve",
             "description",
+            "notes",
             "cvssaccessVector",
             "cvssaccessComplexity",
             "cvssauthentication",
             "cvssconfidentialityImpact",
             "cvssintegrityImpact",
             "cvssavailabilityImpact",
             "cvssbaseScore",
```

### Comparing `nbrisk-35.1.3/nb_risk/forms.py` & `nbrisk-40.0.1/nb_risk/forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,23 @@
     NetBoxModelForm,
     NetBoxModelFilterSetForm,
     NetBoxModelBulkEditForm,
     NetBoxModelImportForm,
 )
 from ipam.models import IPAddress
 from dcim.models import Device, DeviceType
-from utilities.forms import BootstrapMixin
 from utilities.forms.fields import (
     DynamicModelMultipleChoiceField,
     SlugField,
     DynamicModelChoiceField,
     CSVModelMultipleChoiceField,
     CSVModelChoiceField,
     CSVContentTypeField,
 )
+from utilities.forms.rendering import FieldSet
 
 from . import models, choices
 
 # ThreatSource Forms
 
 
 class ThreatSourceForm(NetBoxModelForm):
@@ -107,17 +107,18 @@
 
 # Vulnerability Forms
 
 
 class VulnerabilityForm(NetBoxModelForm):
 
     fieldsets = (
-        ("Vulnerability", ("name", "cve", "description", "notes"),),
-        ("CVSSv2 Score", ("cvssaccessVector", "cvssaccessComplexity", "cvssauthentication", "cvssconfidentialityImpact", "cvssintegrityImpact", "cvssavailabilityImpact", "cvssbaseScore")),
-    )
+        FieldSet("name", "cve", "description", "notes", name="Vulnerability"),
+        FieldSet("cvssaccessVector", "cvssaccessComplexity", "cvssauthentication", "cvssconfidentialityImpact", "cvssintegrityImpact", "cvssavailabilityImpact", "cvssbaseScore", name="CVSSv2 Score"),
+      )
+      
     class Meta:
         model = models.Vulnerability
         fields = [
             "name",
             "cve",
             "description",
             "notes",
@@ -139,16 +140,16 @@
 
 
 class VulnerabilitySearchFilterForm(NetBoxModelFilterSetForm):
     
     model = models.Vulnerability
 
     fieldsets = (
-        ("CVE", ("cve", "keyword") ),
-        ("CPE", ("cpe", "device_type", "version", "part")),
+        FieldSet("cve", "keyword", name="CVE"),
+        FieldSet("cpe", "device_type", "version", "part", name="CPE"),
     )    
 
     cpe = forms.CharField(label="CPE Name", required=False)
 
     cve = forms.CharField(label="CVE", required=False)
 
     keyword = forms.CharField(label="Keyword", required=False)
@@ -180,20 +181,21 @@
             "cvssavailabilityImpact",
             "cvssbaseScore",
         ]
 
 # VulnerabilityAssignment Forms
 
 
-class VulnerabilityAssignmentForm(BootstrapMixin, forms.ModelForm):
+class VulnerabilityAssignmentForm(forms.ModelForm):
 
     vulnerability = DynamicModelChoiceField(
         queryset=models.Vulnerability.objects.all(),
         required=True,
     )
+    
 
     class Meta:
         model = models.VulnerabilityAssignment
         fields = ["asset_object_type", "asset_id", "vulnerability"]
         widgets = {
             "asset_object_type": forms.HiddenInput(),
             "asset_id": forms.HiddenInput(),
@@ -253,14 +255,17 @@
                 if parent is not None:
                     asset_type = ContentType.objects.get_for_model(parent)
                     asset_id = parent.id
                     if models.VulnerabilityAssignment.objects.filter(asset_object_type=asset_type, asset_id=asset_id, vulnerability=vuln).exists():
                         raise forms.ValidationError(
                             f"Vulnerability {vuln} is already assigned to {ip_address} asset object {parent}"
                         )
+
+
+
         return cleaned_data
     
 
     class Meta:
         model = models.VulnerabilityAssignment
         fields = [
             "asset_object_type",
```

### Comparing `nbrisk-35.1.3/nb_risk/migrations/0001_initial.py` & `nbrisk-40.0.1/nb_risk/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `nbrisk-35.1.3/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py` & `nbrisk-40.0.1/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py`

 * *Files identical despite different names*

### Comparing `nbrisk-35.1.3/nb_risk/migrations/0003_control.py` & `nbrisk-40.0.1/nb_risk/migrations/0003_control.py`

 * *Files identical despite different names*

### Comparing `nbrisk-35.1.3/nb_risk/migrations/0007_remove_vulnerability_unique_vuln_name_and_more.py` & `nbrisk-40.0.1/nb_risk/migrations/0007_remove_vulnerability_unique_vuln_name_and_more.py`

 * *Files identical despite different names*

### Comparing `nbrisk-35.1.3/nb_risk/models.py` & `nbrisk-40.0.1/nb_risk/models.py`

 * *Files identical despite different names*

### Comparing `nbrisk-35.1.3/nb_risk/navigation.py` & `nbrisk-40.0.1/nb_risk/navigation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from extras.plugins import PluginMenu, PluginMenuItem, PluginMenuButton
-from utilities.choices import ButtonColorChoices
+from netbox.plugins import PluginMenu, PluginMenuItem, PluginMenuButton
 
 menu = PluginMenu(
     label="Risk Assessment",
     icon_class="mdi mdi-spider",
     groups=(
         (
             "Threat",
@@ -13,29 +12,27 @@
                     link="plugins:nb_risk:threatsource_list",
                     link_text="Threat Sources",
                     buttons=(
                         PluginMenuButton(
                             "plugins:nb_risk:threatsource_add",
                             "Add",
                             "mdi mdi-plus-thick",
-                            ButtonColorChoices.GREEN,
                             permissions=["nb_risk.add_threatsource"],
                         ),
                     ),
                 ),
                 PluginMenuItem(
                     permissions=["nb_risk.view_threatevent"],
                     link="plugins:nb_risk:threatevent_list",
                     link_text="Threat Events",
                     buttons=(
                         PluginMenuButton(
                             "plugins:nb_risk:threatevent_add",
                             "Add",
                             "mdi mdi-plus-thick",
-                            ButtonColorChoices.GREEN,
                             permissions=["nb_risk.add_threatevent"],
                         ),
                     ),
                 ),
             ),
         ),
         (
@@ -46,30 +43,36 @@
                     link="plugins:nb_risk:vulnerability_list",
                     link_text="Vulnerabilities",
                     buttons=(
                         PluginMenuButton(
                             "plugins:nb_risk:vulnerability_add",
                             "Add",
                             "mdi mdi-plus-thick",
-                            ButtonColorChoices.GREEN,
                             permissions=["nb_risk.add_vulnerability"],
                         ),
                         PluginMenuButton(
                             "plugins:nb_risk:vulnerability_search",
                             "Search",
                             "mdi mdi-magnify",
-                            ButtonColorChoices.BLUE,
                             permissions=["nb_risk.view_vulnerability"],
                         ),
                     ),
                 ),
                 PluginMenuItem(
                     permissions=["nb_risk.view_vulnerabilityassignment"],
                     link="plugins:nb_risk:vulnerabilityassignment_list",
                     link_text="Vulnerability Assignments",
+                    buttons=(
+                        PluginMenuButton(
+                            "plugins:nb_risk:vulnerabilityassignment_import",
+                            "Import",
+                            "mdi mdi-upload",
+                            permissions=["nb_risk.add_vulnerabilityassignment"],
+                        ),
+                    ),
                 ),
             ),
         ),
         (
             "Risk",
             (
                 PluginMenuItem(
@@ -77,29 +80,27 @@
                     link="plugins:nb_risk:risk_list",
                     link_text="Risks",
                     buttons=(
                         PluginMenuButton(
                             "plugins:nb_risk:risk_add",
                             "Add",
                             "mdi mdi-plus-thick",
-                            ButtonColorChoices.GREEN,
                             permissions=["nb_risk.add_risk"],
                         ),
                     ),
                 ),
                 PluginMenuItem(
                     permissions=["nb_risk.view_control"],
                     link="plugins:nb_risk:control_list",
                     link_text="Controls",
                     buttons=(
                         PluginMenuButton(
                             "plugins:nb_risk:control_add",
                             "Add",
                             "mdi mdi-plus-thick",
-                            ButtonColorChoices.GREEN,
                             permissions=["nb_risk.add_control"],
                         ),
                     ),
                 ),
             ),
         ),
     ),
```

### Comparing `nbrisk-35.1.3/nb_risk/tables.py` & `nbrisk-40.0.1/nb_risk/tables.py`

 * *Files 18% similar despite different names*

```diff
@@ -82,15 +82,14 @@
     class Meta(NetBoxTable.Meta):
         model = models.VulnerabilityAssignment
         fields = ["asset", "asset_object_type"]
 
 
 class VulnerabilityExploitListTable(NetBoxTable):
 
-    actions = columns.ActionsColumn(actions=("delete",))
 
     asset = tables.Column(linkify=True)
 
     vulnerability = tables.Column(linkify=True)
 
     asset_object_type = tables.Column(verbose_name="Asset Type")
 
@@ -114,32 +113,30 @@
         model = models.Risk
         fields = ["name", "threat_event", "likelihood", "impact", "risk_level"]
 
 
 # CVE Tables
 
 
-class CveTable(tables.Table):
+class CveTable(NetBoxTable):
 
     id = tables.Column(attrs={"td": {"class": "text-end text-nowrap"}})
     description = tables.Column()
     accessVector = tables.Column(verbose_name="Access Vector")
-    accessComplexity = tables.Column(verbose_name="Access Complexity")
-    authentication = tables.Column(verbose_name="Authentication")
-    confidentialityImpact = tables.Column(verbose_name="Confidentiality Impact")
-    integrityImpact = tables.Column(verbose_name="Integrity Impact")
-    availabilityImpact = tables.Column(verbose_name="Availability Impact")
-    baseScore = tables.Column(verbose_name="Base Score")
 
     create = riskColumns.CreateColumn(empty_values=())
 
-    class Meta:
-        attrs = {
-            "class": "table table-hover object-list",
-        }
+    class Meta(NetBoxTable.Meta):
+        model = models.Vulnerability
+        fields = ["id",
+                  "description",
+                  "accessVector", 
+                  "create"
+                  ]
+
 
 # Control Tables
 
 class ControlTable(NetBoxTable):
     name = tables.Column(linkify=True)
     class Meta(NetBoxTable.Meta):
         model = models.Control
```

### Comparing `nbrisk-35.1.3/nb_risk/template_content.py` & `nbrisk-40.0.1/nb_risk/template_content.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from extras.plugins import PluginTemplateExtension
-from extras.plugins.utils import get_plugin_config
+from netbox.plugins import PluginTemplateExtension
+from netbox.plugins.utils import get_plugin_config
 from django.conf import settings
 from packaging import version
 
 NETBOX_CURRENT_VERSION = version.parse(settings.VERSION)
 
 
 def create_button(model_name):
```

### Comparing `nbrisk-35.1.3/nb_risk/templates/nb_risk/control.html` & `nbrisk-40.0.1/nb_risk/templates/nb_risk/control.html`

 * *Files identical despite different names*

### Comparing `nbrisk-35.1.3/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html` & `nbrisk-40.0.1/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html`

 * *Files identical despite different names*

### Comparing `nbrisk-35.1.3/nb_risk/templates/nb_risk/risk.html` & `nbrisk-40.0.1/nb_risk/templates/nb_risk/risk.html`

 * *Files identical despite different names*

### Comparing `nbrisk-35.1.3/nb_risk/templates/nb_risk/threatevent.html` & `nbrisk-40.0.1/nb_risk/templates/nb_risk/threatevent.html`

 * *Files identical despite different names*

### Comparing `nbrisk-35.1.3/nb_risk/templates/nb_risk/threatsource.html` & `nbrisk-40.0.1/nb_risk/templates/nb_risk/threatsource.html`

 * *Files identical despite different names*

### Comparing `nbrisk-35.1.3/nb_risk/templates/nb_risk/vulnerability.html` & `nbrisk-40.0.1/nb_risk/templates/nb_risk/vulnerability.html`

 * *Files identical despite different names*

### Comparing `nbrisk-35.1.3/nb_risk/templates/nb_risk/vulnerability_search.html` & `nbrisk-40.0.1/nb_risk/templates/nb_risk/vulnerability_search.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-{% extends 'base/layout.html' %}
+{% extends 'generic/_base.html' %}
 {% load render_table from django_tables2 %}
 
+{% block title %}Vulnerability Search{% endblock %}
+
+
 {% block tabs %}
   <ul class="nav nav-tabs px-3">
     <li class="nav-item" role="presentation">
-      <button class="nav-link active" id="object-list-tab" data-bs-toggle="tab" data-bs-target="#object-list" type="button" role="tab" aria-controls="edit-form" aria-selected="true">
+      <button class="nav-link active" id="object-list-tab" data-bs-toggle="tab" data-bs-target="#object-list" type="button" role="tab" aria-controls="edit-form" aria-selected="false">
         Results {% badge table.page.paginator.count %}
       </button>
     </li>
     {% if filter_form %}
       <li class="nav-item" role="presentation">
-        <button class="nav-link" id="filters-form-tab" data-bs-toggle="tab" data-bs-target="#filters-form" type="button" role="tab" aria-controls="object-list" aria-selected="false">
+        <button class="nav-link" id="filters-form-tab" data-bs-toggle="tab" data-bs-target="#filters-form" type="button" role="tab" aria-controls="object-list" aria-selected="true">
           Filters
           {% if filter_form %}{% badge filter_form.changed_data|length bg_color="primary" %}{% endif %}
         </button>
       </li>
     {% endif %}
   </ul>
 {% endblock tabs %}
 
-{% block content-wrapper %}
+{% block content %}
   <div class="tab-content">
     <div class="tab-pane show active" id="object-list" role="tabpanel" aria-labelledby="object-list-tab">
       <div class="card">
         <div class="card-body" id="object_list">
           {% include 'htmx/table.html' %}
         </div>
       </div>
@@ -33,8 +36,8 @@
     {# Filter form #}
     {% if filter_form %}
       <div class="tab-pane show" id="filters-form" role="tabpanel" aria-labelledby="filters-form-tab">
         {% include 'inc/filter_list.html' %}
       </div>
     {% endif %}
   </div>
-{% endblock content-wrapper %}
+{% endblock content %}
```

### Comparing `nbrisk-35.1.3/nb_risk/tests/custom.py` & `nbrisk-40.0.1/nb_risk/tests/custom.py`

 * *Files identical despite different names*

### Comparing `nbrisk-35.1.3/nb_risk/tests/threatsource/test_api.py` & `nbrisk-40.0.1/nb_risk/tests/threatsource/test_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,8 +39,8 @@
         ThreatSource.objects.bulk_create(t_sources)
 
         cls.create_data = [ 
             {"name": "ThreatSource X","threat_type": choices.ThreatTypeChoices.THREAT_TYPE_1,"capability": choices.CapabilityChoices.CAPABILITY_1, "description": "A new threat source", },
             {"name": "ThreatSource Y","threat_type": choices.ThreatTypeChoices.THREAT_TYPE_1,"capability": choices.CapabilityChoices.CAPABILITY_1, "description": "Another new threat source", },
         ]
 
-        cls.brief_fields = ['display', 'id', 'name', 'url']
+        cls.brief_fields = ['description', 'display', 'id','name', 'url'   ]
```

### Comparing `nbrisk-35.1.3/nb_risk/tests/threatsource/test_filters.py` & `nbrisk-40.0.1/nb_risk/tests/threatsource/test_filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.test import TestCase
 
 from utilities.testing import ChangeLoggedFilterSetTests
 
 from nb_risk.models import ThreatSource
-from nb_risk.filters import ThreatSourceFilterSet
+from nb_risk.filtersets import ThreatSourceFilterSet
 from nb_risk import choices
 
 
 class ThreatSourceFilterTestCase(TestCase, ChangeLoggedFilterSetTests):
     queryset = ThreatSource.objects.all()
     filterset = ThreatSourceFilterSet
```

### Comparing `nbrisk-35.1.3/nb_risk/tests/threatsource/test_views.py` & `nbrisk-40.0.1/nb_risk/tests/threatsource/test_views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from utilities.testing import ViewTestCases, create_tags
 
 from nb_risk.tests.custom import ModelViewTestCase
 from nb_risk.models import ThreatSource
 from nb_risk import choices
 
 
-class ControlViewTestCase(
+class ThreatSourceViewTestCase(
     ModelViewTestCase,
     ViewTestCases.GetObjectViewTestCase,
     ViewTestCases.CreateObjectViewTestCase,
     ViewTestCases.EditObjectViewTestCase,
     ViewTestCases.DeleteObjectViewTestCase,
     ViewTestCases.ListObjectsViewTestCase,
     ViewTestCases.GetObjectChangelogViewTestCase,
```

### Comparing `nbrisk-35.1.3/nb_risk/tests/vulnerability/test_filters.py` & `nbrisk-40.0.1/nb_risk/tests/vulnerability/test_filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.test import TestCase
 
 from utilities.testing import ChangeLoggedFilterSetTests
 
 from nb_risk.models import Vulnerability
-from nb_risk.filters import VulnerabilityFilterSet
+from nb_risk.filtersets import VulnerabilityFilterSet
 from nb_risk import choices
 
 
 class VulnerabilityFilterTestCase(TestCase, ChangeLoggedFilterSetTests):
     queryset = Vulnerability.objects.all()
     filterset = VulnerabilityFilterSet
```

### Comparing `nbrisk-35.1.3/nb_risk/tests/vulnerability/test_views.py` & `nbrisk-40.0.1/nb_risk/tests/vulnerability/test_views.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from utilities.testing import ViewTestCases, create_tags
 
 from nb_risk.tests.custom import ModelViewTestCase
 from nb_risk.models import Vulnerability
 from nb_risk import choices
 
 
-class ControlViewTestCase(
+class VulnerabilityViewTestCase(
     ModelViewTestCase,
     ViewTestCases.GetObjectViewTestCase,
     ViewTestCases.CreateObjectViewTestCase,
     ViewTestCases.EditObjectViewTestCase,
     ViewTestCases.DeleteObjectViewTestCase,
     ViewTestCases.ListObjectsViewTestCase,
     ViewTestCases.GetObjectChangelogViewTestCase,
```

### Comparing `nbrisk-35.1.3/nb_risk/tests/vulnerabilityassignment/test_api.py` & `nbrisk-40.0.1/nb_risk/tests/vulnerabilityassignment/test_api.py`

 * *Files identical despite different names*

### Comparing `nbrisk-35.1.3/nb_risk/urls.py` & `nbrisk-40.0.1/nb_risk/urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     path("vulnerability-assignments/add/", views.VulnerabilityAssignmentEditView.as_view(), name="vulnerabilityassignment_add",),
     path("vulnerability-assignments/", views.VulnerabilityAssignmentListView.as_view(), name="vulnerabilityassignment_list",),
     path("vulnerability-assignment/delete/", views.VulnerabilityAssignmentBulkDeleteView.as_view(), name="vulnerabilityassignment_bulk_delete",),
     path("vulnerability-assignments/<int:pk>/delete/", views.VulnerabilityAssignmentDeleteView.as_view(), name="vulnerabilityassignment_delete",),
     path("vulnerability-assignments/<int:pk>/edit/", views.VulnerabilityAssignmentEditView.as_view(), name="vulnerabilityassignment_edit",),
     path('vulnerability-assignments/<int:pk>/', include(get_model_urls(app_name, 'vulnerabilityassignment'))),
     path('vulnerability-assignments/import/', views.VulnerabilityAssignmentImportView.as_view(), name='vulnerabilityassignment_import'),
+    
     # Risk URLs
     path("risk/", views.RiskListView.as_view(), name="risk_list"),
     path("risk/add/", views.RiskEditView.as_view(), name="risk_add"),
     path("risk/<int:pk>/", views.RiskView.as_view(), name="risk"),
     path('risk/<int:pk>/', include(get_model_urls(app_name, 'risk'))),
     path("risk/<int:pk>/edit/", views.RiskEditView.as_view(), name="risk_edit"),
     path("risk/<int:pk>/delete/", views.RiskDeleteView.as_view(), name="risk_delete"),
```

### Comparing `nbrisk-35.1.3/nb_risk/views.py` & `nbrisk-40.0.1/nb_risk/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,39 @@
+from django.core.exceptions import MultipleObjectsReturned, ValidationError, ObjectDoesNotExist
+from django.contrib.contenttypes.models import ContentType
+
 from netbox.views import generic
 from dcim.models import Device, Site
 from tenancy.models import Tenant
 from virtualization.models import VirtualMachine
-from core.models import ContentType
+from core.models import ObjectType as ContentType
+from ipam.models import IPAddress
 
-from extras.plugins.utils import get_plugin_config
+from netbox.plugins.utils import get_plugin_config
 from utilities.views import ViewTab, register_model_view
 from django.shortcuts import get_object_or_404
+from django.urls import reverse
 
 import logging
 
 logger = logging.getLogger(__name__)
 
-from . import forms, models, tables, filters
+from . import forms, models, tables, filtersets
 
 # ThreatSource Views
 
 
 class ThreatSourceView(generic.ObjectView):
     queryset = models.ThreatSource.objects.all()
 
 
 class ThreatSourceListView(generic.ObjectListView):
     queryset = models.ThreatSource.objects.all()
     table = tables.ThreatSourceTable
-    filterset = filters.ThreatSourceFilterSet
+    filterset = filtersets.ThreatSourceFilterSet
     filterset_form = forms.ThreatSourceFilterForm
 
 
 class ThreatSourceEditView(generic.ObjectEditView):
     queryset = models.ThreatSource.objects.all()
     form = forms.ThreatSourceForm
 
@@ -36,15 +41,15 @@
 class ThreatSourceImportView(generic.BulkImportView):
     queryset = models.ThreatSource.objects.all()
     model_form = forms.ThreatSourceImportForm
     table = tables.ThreatSourceTable
 
 class ThreatSourceBulkEditView(generic.BulkEditView):
     queryset = models.ThreatSource.objects.all()
-    filterset = filters.ThreatSourceFilterSet
+    filterset = filtersets.ThreatSourceFilterSet
     table = tables.ThreatSourceTable
     form = forms.ThreatSourceBulkEditForm
 
 class ThreatSourceBulkDeleteView(generic.BulkDeleteView):
     queryset = models.ThreatSource.objects.all()
     table = tables.ThreatSourceTable
 
@@ -71,15 +76,15 @@
             childrens = parent.vulnerability.all()
             return childrens
 
 
 class ThreatEventListView(generic.ObjectListView):
     queryset = models.ThreatEvent.objects.all()
     table = tables.ThreatEventTable
-    filterset = filters.ThreatEventFilterSet
+    filterset = filtersets.ThreatEventFilterSet
     filterset_form = forms.ThreatEventFilterForm
 
 
 class ThreatEventEditView(generic.ObjectEditView):
     queryset = models.ThreatEvent.objects.all()
     form = forms.ThreatEventForm
 
@@ -112,15 +117,15 @@
             childrens = models.VulnerabilityAssignment.objects.filter(vulnerability=parent)
             return childrens
 
     
 class VulnerabilityListView(generic.ObjectListView):
     queryset = models.Vulnerability.objects.all()
     table = tables.VulnerabilityTable
-    filterset = filters.VulnerabilityFilterSet
+    filterset = filtersets.VulnerabilityFilterSet
     filterset_form = forms.VulnerabilityFilterForm
     template_name = "nb_risk/vulnerability_list.html"
 
 
 class VulnerabilityEditView(generic.ObjectEditView):
     queryset = models.Vulnerability.objects.all()
     form = forms.VulnerabilityForm
@@ -194,24 +199,27 @@
 
 class VulnerabilityAssignmentEditView(generic.ObjectEditView):
     queryset = models.VulnerabilityAssignment.objects.all()
     form = forms.VulnerabilityAssignmentForm
     template_name = "nb_risk/generic_vulnerability_assignment_edit.html"
 
     def alter_object(self, instance, request, args, kwargs):
+
         if not instance.pk:
             # Assign the object based on URL kwargs
             content_type = get_object_or_404(
                 ContentType, pk=request.GET.get("asset_object_type")
             )
             instance.object = get_object_or_404(
                 content_type.model_class(), pk=request.GET.get("asset_id")
             )
+        else:
+            instance.object = instance.asset
         return instance
-
+    
     def get_extra_addanother_params(self, request):
         return {
             "asset_object_type": request.GET.get("asset_object_type"),
             "asset_id": request.GET.get("asset_id"),
         }
 
 
@@ -221,17 +229,16 @@
 class VulnerabilityAssignmentBulkDeleteView(generic.BulkDeleteView):
     queryset = models.VulnerabilityAssignment.objects.all()
     table = tables.VulnerabilityExploitListTable
 
 class VulnerabilityAssignmentListView(generic.ObjectListView):
     queryset = models.VulnerabilityAssignment.objects.all()
     table = tables.VulnerabilityExploitListTable
-    filterset = filters.VulnerabilityAssignmentFilterSet
+    filterset = filtersets.VulnerabilityAssignmentFilterSet
     filterset_form = forms.VulnerabilityAssignmentFilterForm
-    actions = ('import', 'export', )
 
 class VulnerabilityAssignmentImportView(generic.BulkImportView):
     queryset = models.VulnerabilityAssignment.objects.all()
     model_form = forms.VulnerabilityAssignmentImportForm
     table = tables.VulnerabilityExploitListTable
 
     def save_object(self, object_form, request):
@@ -244,21 +251,24 @@
             )
             vulnAssingment.full_clean()
             vulnAssingment.save()
             return vulnAssingment                        
 
 
         return object_form.save()
+
+
+
 # Risk Views
 
 
 class RiskListView(generic.ObjectListView):
     queryset = models.Risk.objects.all()
     table = tables.RiskTable
-    filterset = filters.RiskFilterSet
+    filterset = filtersets.RiskFilterSet
     filterset_form = forms.RiskFilterForm
 
 
 class RiskView(generic.ObjectView):
     queryset = models.Risk.objects.all()
 
 
@@ -276,15 +286,15 @@
     table = tables.RiskTable
 
 # Control Views
 
 class ControlListView(generic.ObjectListView):
     queryset = models.Control.objects.all()
     table = tables.ControlTable
-    filterset = filters.ControlFilterSet
+    filterset = filtersets.ControlFilterSet
     filterset_form = forms.ControlFilterForm
 
 class ControlView(generic.ObjectView):
     queryset = models.Control.objects.all()
 
     def get_extra_context(self, request, instance):
         risks = instance.risk.all()
```

### Comparing `nbrisk-35.1.3/setup.py` & `nbrisk-40.0.1/setup.py`

 * *Files identical despite different names*

