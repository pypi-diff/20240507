# Comparing `tmp/prismacloud_cli-0.8.7.tar.gz` & `tmp/prismacloud_cli-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prismacloud_cli-0.8.7.tar", last modified: Mon Apr 29 15:23:04 2024, max compression
+gzip compressed data, was "prismacloud_cli-0.8.8.tar", last modified: Tue May  7 10:06:49 2024, max compression
```

## Comparing `prismacloud_cli-0.8.7.tar` & `prismacloud_cli-0.8.8.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:23:04.526956 prismacloud_cli-0.8.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-04-29 15:23:04.526956 prismacloud_cli-0.8.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:23:04.514956 prismacloud_cli-0.8.7/prismacloud/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:23:04.518956 prismacloud_cli-0.8.7/prismacloud/cli/
--rw-r--r--   0 runner    (1001) docker     (127)    16643 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12625 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:23:04.518956 prismacloud_cli-0.8.7/prismacloud/cli/cspm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_alert.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_current.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_iam.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_pov.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_rql.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_saas_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_usage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:23:04.522956 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_audits.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_defenders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_host_auto_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_hosts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_incidents.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_intelligence.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_license.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_scans.py
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_serverless_auto_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     8836 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_users.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:23:04.522956 prismacloud_cli-0.8.7/prismacloud/cli/pccs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/pccs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31896 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/pccs/cmd_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/pccs/cmd_reviews.py
--rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/pccs/cmd_suppressions.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:23:04.526956 prismacloud_cli-0.8.7/prismacloud_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-04-29 15:23:04.000000 prismacloud_cli-0.8.7/prismacloud_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-29 15:23:04.000000 prismacloud_cli-0.8.7/prismacloud_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:23:04.000000 prismacloud_cli-0.8.7/prismacloud_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-29 15:23:04.000000 prismacloud_cli-0.8.7/prismacloud_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-29 15:23:04.000000 prismacloud_cli-0.8.7/prismacloud_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-29 15:23:04.000000 prismacloud_cli-0.8.7/prismacloud_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-29 15:23:04.526956 prismacloud_cli-0.8.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:23:04.526956 prismacloud_cli-0.8.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:06:49.762928 prismacloud_cli-0.8.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-05-07 10:06:49.762928 prismacloud_cli-0.8.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:06:49.750928 prismacloud_cli-0.8.8/prismacloud/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:06:49.750928 prismacloud_cli-0.8.8/prismacloud/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    16643 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12625 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:06:49.754928 prismacloud_cli-0.8.8/prismacloud/cli/cspm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cspm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cspm/cmd_alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cspm/cmd_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cspm/cmd_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cspm/cmd_compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cspm/cmd_current.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cspm/cmd_iam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cspm/cmd_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cspm/cmd_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cspm/cmd_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cspm/cmd_pov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cspm/cmd_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cspm/cmd_rql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cspm/cmd_saas_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cspm/cmd_usage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:06:49.758928 prismacloud_cli-0.8.8/prismacloud/cli/cwpp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cwpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_audits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_defenders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_host_auto_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_incidents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_intelligence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_license.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_scans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_serverless_auto_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8836 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:06:49.758928 prismacloud_cli-0.8.8/prismacloud/cli/pccs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/pccs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31896 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/pccs/cmd_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/pccs/cmd_reviews.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/pccs/cmd_suppressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/prismacloud/cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:06:49.762928 prismacloud_cli-0.8.8/prismacloud_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-05-07 10:06:49.000000 prismacloud_cli-0.8.8/prismacloud_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-07 10:06:49.000000 prismacloud_cli-0.8.8/prismacloud_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 10:06:49.000000 prismacloud_cli-0.8.8/prismacloud_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 10:06:49.000000 prismacloud_cli-0.8.8/prismacloud_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-07 10:06:49.000000 prismacloud_cli-0.8.8/prismacloud_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 10:06:49.000000 prismacloud_cli-0.8.8/prismacloud_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-07 10:06:49.762928 prismacloud_cli-0.8.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:06:49.758928 prismacloud_cli-0.8.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-07 10:06:00.000000 prismacloud_cli-0.8.8/tests/test_cli.py
```

### Comparing `prismacloud_cli-0.8.7/LICENSE` & `prismacloud_cli-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/PKG-INFO` & `prismacloud_cli-0.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prismacloud-cli
-Version: 0.8.7
+Version: 0.8.8
 Summary: Prisma Cloud CLI
 Home-page: https://github.com/PaloAltoNetworks/prismacloud-cli
 Author: Steven de Boer, Simon Melotte, Tom Kishel
 Author-email: stdeboer@paloaltonetworks.com, smelotte@paloaltonetworks.com, tkishel@paloaltonetworks.com
 License: BSD
 Keywords: prisma cloud cli
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `prismacloud_cli-0.8.7/README.md` & `prismacloud_cli-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/__init__.py` & `prismacloud_cli-0.8.8/prismacloud/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/api.py` & `prismacloud_cli-0.8.8/prismacloud/cli/api.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_alert.py` & `prismacloud_cli-0.8.8/prismacloud/cli/cspm/cmd_alert.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_cloud.py` & `prismacloud_cli-0.8.8/prismacloud/cli/cspm/cmd_cloud.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_compliance.py` & `prismacloud_cli-0.8.8/prismacloud/cli/cspm/cmd_compliance.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_iam.py` & `prismacloud_cli-0.8.8/prismacloud/cli/cspm/cmd_iam.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_inventory.py` & `prismacloud_cli-0.8.8/prismacloud/cli/cspm/cmd_inventory.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_licenses.py` & `prismacloud_cli-0.8.8/prismacloud/cli/cspm/cmd_licenses.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_policy.py` & `prismacloud_cli-0.8.8/prismacloud/cli/cspm/cmd_policy.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_pov.py` & `prismacloud_cli-0.8.8/prismacloud/cli/cspm/cmd_pov.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_resource.py` & `prismacloud_cli-0.8.8/prismacloud/cli/cspm/cmd_resource.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_rql.py` & `prismacloud_cli-0.8.8/prismacloud/cli/cspm/cmd_rql.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,16 @@
         if query.startswith("config from iam"):
             search_params["searchType"] = "iam"
             search_params["timeRange"] = {"type": "to_now", "value": "epoch"}  # Latest results
             result_list = pc_api.search_iam_read(search_params=search_params)
         elif query.startswith("config from"):
             result_list = pc_api.search_config_read(search_params=search_params)
         elif query.startswith("network from"):
+            # For a network query, focus on field data.nodes
+            field = "data.nodes"
             result_list = pc_api.search_network_read(search_params=search_params)
         elif query.startswith("event from"):
             result_list = pc_api.search_event_read(search_params=search_params)
         else:
             logging.error("Unknown RQL query type (limited to: config|network|event).")
 
         if field == "":
```

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_saas_version.py` & `prismacloud_cli-0.8.8/prismacloud/cli/cspm/cmd_saas_version.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_audits.py` & `prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_audits.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_containers.py` & `prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_containers.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_defenders.py` & `prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_defenders.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_discovery.py` & `prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_discovery.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_host_auto_deploy.py` & `prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_host_auto_deploy.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_hosts.py` & `prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_hosts.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_images.py` & `prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_images.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_incidents.py` & `prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_incidents.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_logs.py` & `prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_logs.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_monitor.py` & `prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_monitor.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_policies.py` & `prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_policies.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_registry.py` & `prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_registry.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_scans.py` & `prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_scans.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_serverless_auto_deploy.py` & `prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_serverless_auto_deploy.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_stats.py` & `prismacloud_cli-0.8.8/prismacloud/cli/cwpp/cmd_stats.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/pccs/cmd_repositories.py` & `prismacloud_cli-0.8.8/prismacloud/cli/pccs/cmd_repositories.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud/cli/pccs/cmd_suppressions.py` & `prismacloud_cli-0.8.8/prismacloud/cli/pccs/cmd_suppressions.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/prismacloud_cli.egg-info/PKG-INFO` & `prismacloud_cli-0.8.8/prismacloud_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prismacloud-cli
-Version: 0.8.7
+Version: 0.8.8
 Summary: Prisma Cloud CLI
 Home-page: https://github.com/PaloAltoNetworks/prismacloud-cli
 Author: Steven de Boer, Simon Melotte, Tom Kishel
 Author-email: stdeboer@paloaltonetworks.com, smelotte@paloaltonetworks.com, tkishel@paloaltonetworks.com
 License: BSD
 Keywords: prisma cloud cli
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `prismacloud_cli-0.8.7/prismacloud_cli.egg-info/SOURCES.txt` & `prismacloud_cli-0.8.8/prismacloud_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/setup.py` & `prismacloud_cli-0.8.8/setup.py`

 * *Files identical despite different names*

### Comparing `prismacloud_cli-0.8.7/tests/test_cli.py` & `prismacloud_cli-0.8.8/tests/test_cli.py`

 * *Files identical despite different names*

