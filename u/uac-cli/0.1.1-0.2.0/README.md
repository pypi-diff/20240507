# Comparing `tmp/uac-cli-0.1.1.tar.gz` & `tmp/uac-cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uac-cli-0.1.1.tar", last modified: Mon May  6 20:23:01 2024, max compression
+gzip compressed data, was "uac-cli-0.2.0.tar", last modified: Tue May  7 21:04:31 2024, max compression
```

## Comparing `uac-cli-0.1.1.tar` & `uac-cli-0.2.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-06 20:23:01.950808 uac-cli-0.1.1/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9033 2024-05-06 20:23:01.950553 uac-cli-0.1.1/PKG-INFO
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     8622 2024-05-06 20:21:34.000000 uac-cli-0.1.1/README.md
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-26 03:38:30.000000 uac-cli-0.1.1/pyproject.toml
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2024-05-06 20:23:01.950855 uac-cli-0.1.1/setup.cfg
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1256 2024-05-05 22:48:41.000000 uac-cli-0.1.1/setup.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-06 20:23:01.926665 uac-cli-0.1.1/uac_cli/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       21 2024-05-06 19:27:35.000000 uac-cli-0.1.1/uac_cli/__init__.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-06 20:23:01.948225 uac-cli-0.1.1/uac_cli/commands/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-05 17:55:51.000000 uac-cli-0.1.1/uac_cli/commands/__init__.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5200 2024-05-05 18:06:52.000000 uac-cli-0.1.1/uac_cli/commands/agent.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5924 2024-05-05 18:08:29.000000 uac-cli-0.1.1/uac_cli/commands/agent_cluster.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      857 2024-05-05 18:19:43.000000 uac-cli-0.1.1/uac_cli/commands/audit.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     8955 2024-05-05 18:23:19.000000 uac-cli-0.1.1/uac_cli/commands/bundle.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2849 2024-05-05 18:20:29.000000 uac-cli-0.1.1/uac_cli/commands/business_service.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5107 2024-05-05 18:20:47.000000 uac-cli-0.1.1/uac_cli/commands/calendar.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1106 2024-05-05 18:21:02.000000 uac-cli-0.1.1/uac_cli/commands/cluster_node.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2143 2024-05-05 22:45:19.000000 uac-cli-0.1.1/uac_cli/commands/config.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    11376 2024-05-05 18:32:10.000000 uac-cli-0.1.1/uac_cli/commands/connection.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3688 2024-05-05 18:21:16.000000 uac-cli-0.1.1/uac_cli/commands/credential.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3268 2024-05-05 18:21:37.000000 uac-cli-0.1.1/uac_cli/commands/custom_day.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2784 2024-05-05 18:22:02.000000 uac-cli-0.1.1/uac_cli/commands/email_template.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1409 2024-05-05 18:22:13.000000 uac-cli-0.1.1/uac_cli/commands/ldap.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      695 2024-05-05 18:41:31.000000 uac-cli-0.1.1/uac_cli/commands/metric.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2809 2024-05-05 18:22:39.000000 uac-cli-0.1.1/uac_cli/commands/oauth_client.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2878 2024-05-05 18:22:58.000000 uac-cli-0.1.1/uac_cli/commands/oms_server.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1484 2024-05-05 18:23:54.000000 uac-cli-0.1.1/uac_cli/commands/property.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      897 2024-05-05 18:24:18.000000 uac-cli-0.1.1/uac_cli/commands/report.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2382 2024-05-05 18:24:34.000000 uac-cli-0.1.1/uac_cli/commands/script.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1075 2024-05-05 18:24:50.000000 uac-cli-0.1.1/uac_cli/commands/server_operation.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2848 2024-05-05 18:25:03.000000 uac-cli-0.1.1/uac_cli/commands/simulation.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      665 2024-05-05 22:30:41.000000 uac-cli-0.1.1/uac_cli/commands/system.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9351 2024-05-06 20:08:49.000000 uac-cli-0.1.1/uac_cli/commands/task.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    17677 2024-05-05 18:25:56.000000 uac-cli-0.1.1/uac_cli/commands/task_instance.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6121 2024-05-05 22:53:03.000000 uac-cli-0.1.1/uac_cli/commands/trigger.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1396 2024-05-05 18:28:59.000000 uac-cli-0.1.1/uac_cli/commands/universal_event.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2939 2024-05-05 18:28:56.000000 uac-cli-0.1.1/uac_cli/commands/universal_event_template.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6110 2024-05-05 18:29:19.000000 uac-cli-0.1.1/uac_cli/commands/universal_template.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4487 2024-05-05 18:29:46.000000 uac-cli-0.1.1/uac_cli/commands/user.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2533 2024-05-05 18:29:32.000000 uac-cli-0.1.1/uac_cli/commands/user_group.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3308 2024-05-05 18:30:07.000000 uac-cli-0.1.1/uac_cli/commands/variable.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3504 2024-05-05 18:30:22.000000 uac-cli-0.1.1/uac_cli/commands/virtual_resource.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4000 2024-05-05 18:30:39.000000 uac-cli-0.1.1/uac_cli/commands/webhook.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4934 2024-05-05 18:30:54.000000 uac-cli-0.1.1/uac_cli/commands/workflow.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4809 2024-05-06 20:12:59.000000 uac-cli-0.1.1/uac_cli/main.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-06 20:23:01.950180 uac-cli-0.1.1/uac_cli/utils/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-05 17:56:14.000000 uac-cli-0.1.1/uac_cli/utils/__init__.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2922 2024-05-05 22:04:40.000000 uac-cli-0.1.1/uac_cli/utils/config.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      460 2024-05-05 18:06:43.000000 uac-cli-0.1.1/uac_cli/utils/options.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2079 2024-05-06 20:06:47.000000 uac-cli-0.1.1/uac_cli/utils/process.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-06 20:23:01.929679 uac-cli-0.1.1/uac_cli.egg-info/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9033 2024-05-06 20:23:01.000000 uac-cli-0.1.1/uac_cli.egg-info/PKG-INFO
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1433 2024-05-06 20:23:01.000000 uac-cli-0.1.1/uac_cli.egg-info/SOURCES.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2024-05-06 20:23:01.000000 uac-cli-0.1.1/uac_cli.egg-info/dependency_links.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       41 2024-05-06 20:23:01.000000 uac-cli-0.1.1/uac_cli.egg-info/entry_points.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      103 2024-05-06 20:23:01.000000 uac-cli-0.1.1/uac_cli.egg-info/requires.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        8 2024-05-06 20:23:01.000000 uac-cli-0.1.1/uac_cli.egg-info/top_level.txt
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-07 21:04:31.324804 uac-cli-0.2.0/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9364 2024-05-07 21:04:31.324468 uac-cli-0.2.0/PKG-INFO
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     8938 2024-05-06 20:25:28.000000 uac-cli-0.2.0/README.md
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      213 2024-05-07 13:48:31.000000 uac-cli-0.2.0/pyproject.toml
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2024-05-07 21:04:31.324861 uac-cli-0.2.0/setup.cfg
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1256 2024-05-05 22:48:41.000000 uac-cli-0.2.0/setup.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-07 21:04:31.308925 uac-cli-0.2.0/uac_cli/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       21 2024-05-07 21:01:33.000000 uac-cli-0.2.0/uac_cli/__init__.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-07 21:04:31.322895 uac-cli-0.2.0/uac_cli/commands/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-05 17:55:51.000000 uac-cli-0.2.0/uac_cli/commands/__init__.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5545 2024-05-07 20:59:24.000000 uac-cli-0.2.0/uac_cli/commands/agent.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6346 2024-05-07 21:00:04.000000 uac-cli-0.2.0/uac_cli/commands/agent_cluster.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      918 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/audit.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9331 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/bundle.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2994 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/business_service.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5357 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/calendar.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1188 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/cluster_node.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2183 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/config.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    11836 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/connection.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3875 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/credential.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3434 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/custom_day.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2929 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/email_template.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1491 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/ldap.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      756 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/metric.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2954 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/oauth_client.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3023 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/oms_server.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1587 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/property.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      958 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/report.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2527 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/script.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1157 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/server_operation.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2993 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/simulation.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      726 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/system.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9664 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/task.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    18242 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/task_instance.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6392 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/trigger.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1499 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/universal_event.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3084 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/universal_event_template.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6360 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/universal_template.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4716 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/user.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2678 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/user_group.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3495 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/variable.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3691 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/virtual_resource.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4208 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/webhook.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5184 2024-05-07 15:20:53.000000 uac-cli-0.2.0/uac_cli/commands/workflow.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4504 2024-05-07 19:37:27.000000 uac-cli-0.2.0/uac_cli/main.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-07 21:04:31.324093 uac-cli-0.2.0/uac_cli/utils/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-05 17:56:14.000000 uac-cli-0.2.0/uac_cli/utils/__init__.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2922 2024-05-05 22:04:40.000000 uac-cli-0.2.0/uac_cli/utils/config.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      460 2024-05-05 18:06:43.000000 uac-cli-0.2.0/uac_cli/utils/options.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2079 2024-05-06 20:06:47.000000 uac-cli-0.2.0/uac_cli/utils/process.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-07 21:04:31.310617 uac-cli-0.2.0/uac_cli.egg-info/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9364 2024-05-07 21:04:31.000000 uac-cli-0.2.0/uac_cli.egg-info/PKG-INFO
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1433 2024-05-07 21:04:31.000000 uac-cli-0.2.0/uac_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2024-05-07 21:04:31.000000 uac-cli-0.2.0/uac_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       41 2024-05-07 21:04:31.000000 uac-cli-0.2.0/uac_cli.egg-info/entry_points.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      103 2024-05-07 21:04:31.000000 uac-cli-0.2.0/uac_cli.egg-info/requires.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        8 2024-05-07 21:04:31.000000 uac-cli-0.2.0/uac_cli.egg-info/top_level.txt
```

### Comparing `uac-cli-0.1.1/PKG-INFO` & `uac-cli-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: uac-cli
-Version: 0.1.1
-Summary: A CLI tool for executing commands against the Stonebranch UAC API
-Author: Stonebranch
-Author-email: huseyim@gmail.com
-License: CC BY-NC 4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # UAC-CLI: CLI for managing Stonebranch - UAC
 
 ## Overview
 
 UAC CLI is a command-line interface tool designed to interact with the Universal Controller API. It provides a comprehensive set of commands for managing resources such as audits, agent clusters, agents, bundles, business services, calendars, cluster nodes, credentials, custom days, database connections, email connections, LDAP configurations, metrics, OAuth clients, OMS servers, PeopleSoft connections, promotion targets, properties, reports, SAP connections, scripts, server operations, simulations, system status, task instances, tasks, triggers, universal events, universal templates, user groups, users, variables, virtual resources, webhooks, and workflows.
 
 ## Features
@@ -201,15 +188,21 @@
 ```bash
 uac agent_cluster create --input agent_cluster_config.json --ignore-ids
 ```
 
 #### Running a Report
 
 ```bash
+# download PDF file
 uac report run_report report_title="Active Tasks" --format pdf --output report_output.pdf
+# download the report in different formats
+uac report run_report report_title="Active Tasks" --format json
+uac report run_report report_title="Active Tasks" --format tab
+uac report run_report report_title="Active Tasks" --format csv
+uac report run_report report_title="Active Tasks" --format xml
 ```
 
 ## Development
 
 To contribute to the UAC CLI tool, clone the repository, make your changes, and submit a pull request. Ensure you follow the project's coding standards and update tests as necessary.
 
 ## Support
@@ -242,8 +235,8 @@
 - **ShareAlike:** If you remix, transform, or build upon the material, you must distribute your contributions under the same license as the original.
 
 - **No additional restrictions:** You may not apply legal terms or technological measures that legally restrict others from doing anything the license permits.
 
 For more information about what you can and can't do under this license, please review the license code and summary at the provided link.
 
 # Disclaimer
-This package is not officially affiliated with Stonebranch, Inc. It is a community-driven project aimed at simplifying the use of Stonebranch UAC APIs.
+This package is not officially affiliated with Stonebranch, Inc. It is a community-driven project aimed at simplifying the use of Stonebranch UAC APIs.
```

### Comparing `uac-cli-0.1.1/README.md` & `uac-cli-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: uac-cli
+Version: 0.2.0
+Summary: A CLI tool for executing commands against the Stonebranch UAC API
+Author: Stonebranch
+Author-email: "Huseyin G." <huseyim@gmail.com>
+License: CC BY-NC 4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 # UAC-CLI: CLI for managing Stonebranch - UAC
 
 ## Overview
 
 UAC CLI is a command-line interface tool designed to interact with the Universal Controller API. It provides a comprehensive set of commands for managing resources such as audits, agent clusters, agents, bundles, business services, calendars, cluster nodes, credentials, custom days, database connections, email connections, LDAP configurations, metrics, OAuth clients, OMS servers, PeopleSoft connections, promotion targets, properties, reports, SAP connections, scripts, server operations, simulations, system status, task instances, tasks, triggers, universal events, universal templates, user groups, users, variables, virtual resources, webhooks, and workflows.
 
 ## Features
@@ -188,15 +201,21 @@
 ```bash
 uac agent_cluster create --input agent_cluster_config.json --ignore-ids
 ```
 
 #### Running a Report
 
 ```bash
+# download PDF file
 uac report run_report report_title="Active Tasks" --format pdf --output report_output.pdf
+# download the report in different formats
+uac report run_report report_title="Active Tasks" --format json
+uac report run_report report_title="Active Tasks" --format tab
+uac report run_report report_title="Active Tasks" --format csv
+uac report run_report report_title="Active Tasks" --format xml
 ```
 
 ## Development
 
 To contribute to the UAC CLI tool, clone the repository, make your changes, and submit a pull request. Ensure you follow the project's coding standards and update tests as necessary.
 
 ## Support
@@ -229,8 +248,8 @@
 - **ShareAlike:** If you remix, transform, or build upon the material, you must distribute your contributions under the same license as the original.
 
 - **No additional restrictions:** You may not apply legal terms or technological measures that legally restrict others from doing anything the license permits.
 
 For more information about what you can and can't do under this license, please review the license code and summary at the provided link.
 
 # Disclaimer
-This package is not officially affiliated with Stonebranch, Inc. It is a community-driven project aimed at simplifying the use of Stonebranch UAC APIs.
+This package is not officially affiliated with Stonebranch, Inc. It is a community-driven project aimed at simplifying the use of Stonebranch UAC APIs.
```

### Comparing `uac-cli-0.1.1/setup.py` & `uac-cli-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.1.1/uac_cli/commands/agent.py` & `uac-cli-0.2.0/uac_cli/commands/agent.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,117 +1,124 @@
+"""
+This file is for the agent command group
+"""
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 @click.group(help='Commands for managing agents, such as retrieving, updating, and deleting agents.')
 def agent():
     pass
 
 @agent.command('get', short_help='Retrieves information on a specific Agent.')
 @click.argument('args', nargs=-1, metavar='agentid=value agentname=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_agent(uac, args, output=None, select=None):
+def get_agent(uac: UniversalController, args, output=None, select=None):
+    """
+    Gets details of an agent.
+    """
     vars_dict = process_input(args)
     response = uac.agents.get_agent(**vars_dict)
     process_output(output, select, response)
 
 
 @agent.command('update', short_help='Modifies the Agent specified by the sysId.')
 @click.argument('args', nargs=-1, metavar='name=value description=value host_name=value queue_name=value ip_address=value log_level=value version=value build=value build_date=value ext_api_level_min=value ext_api_level_max=value extensions=value ext_accept=value ext_accept_list=value hb_intvl=value hb_grace_period=value cpu_load=value os=value os_release=value cpu=value hb_date=value start_date=value status=value jobs=value credentials=value pid=value limit_type=value limit_amount=value current_count=value suspended=value decommissioned=value decommissioned_date=value output_prohibited=value oms_server=value sys_id=value auth_version=value opswise_groups=value exclude_related=value credentials_required=value notifications=value transient=value type=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_agent(uac, args, output=None, input=None, select=None):
+def update_agent(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.agents.update_agent(**vars_dict)
     process_output(output, select, response)
 
 
 @agent.command('delete', short_help='Deletes an Agent.')
 @click.argument('args', nargs=-1, metavar='agentid=value agentname=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_agent(uac, args, output=None, select=None):
+def delete_agent(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.agents.delete_agent(**vars_dict)
     process_output(output, select, response)
 
 
 @agent.command('list', short_help='Retrieves information on all agents.')
 @click.argument('args', nargs=-1, metavar='')
 @click.pass_obj
 @output_option
 @select_option
-def list_agents(uac, args, output=None, select=None):
+def list_agents(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.agents.list_agents(**vars_dict)
     process_output(output, select, response)
 
 
 @agent.command('list_advanced', short_help='Retrieves Agent details using specific query parameters.')
 @click.argument('args', nargs=-1, metavar='agentname=value type=value business_services=value')
 @click.pass_obj
 @output_option
 @select_option
-def list_agents_advanced(uac, args, output=None, select=None):
+def list_agents_advanced(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.agents.list_agents_advanced(**vars_dict)
     process_output(output, select, response)
 
 
 @agent.command('resume', short_help='Resumes the specified agent.')
 @click.argument('args', nargs=-1, metavar='agent_name=value agent_i_d=value')
 @click.pass_obj
 @output_option
 @select_option
-def resume_agent(uac, args, output=None, select=None):
+def resume_agent(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.agents.resume_agent(**vars_dict)
     process_output(output, select, response)
 
 
 @agent.command('resume_membership', short_help='Resumes the specified agent cluster membership.')
 @click.argument('args', nargs=-1, metavar='agent_name=value agent_cluster_name=value agent_i_d=value')
 @click.pass_obj
 @output_option
 @select_option
-def resume_agent_cluster_membership(uac, args, output=None, select=None):
+def resume_agent_cluster_membership(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.agents.resume_agent_cluster_membership(**vars_dict)
     process_output(output, select, response)
 
 
 @agent.command('set_task_execution_limit', short_help='Sets the task execution limit for the specified agent.')
 @click.argument('args', nargs=-1, metavar='agent_name=value agent_i_d=value limit_type=value limit_amount=value')
 @click.pass_obj
 @output_option
 @select_option
-def set_agent_task_execution_limit(uac, args, output=None, select=None):
+def set_agent_task_execution_limit(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.agents.set_agent_task_execution_limit(**vars_dict)
     process_output(output, select, response)
 
 
 @agent.command('suspend', short_help='Suspends the specified agent.')
 @click.argument('args', nargs=-1, metavar='agent_name=value agent_i_d=value')
 @click.pass_obj
 @output_option
 @select_option
-def suspend_agent(uac, args, output=None, select=None):
+def suspend_agent(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.agents.suspend_agent(**vars_dict)
     process_output(output, select, response)
 
 
 @agent.command('suspend_membership', short_help='Suspends the specified agent cluster membership.')
 @click.argument('args', nargs=-1, metavar='agent_name=value agent_cluster_name=value agent_i_d=value')
 @click.pass_obj
 @output_option
 @select_option
-def suspend_agent_cluster_membership(uac, args, output=None, select=None):
+def suspend_agent_cluster_membership(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.agents.suspend_agent_cluster_membership(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/agent_cluster.py` & `uac-cli-0.2.0/uac_cli/commands/agent_cluster.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,130 +1,138 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 @click.group(help='Commands related to managing agent clusters, including creation, deletion, and listing.')
 def agent_cluster():
     pass
 
 @agent_cluster.command('get', short_help='Retrieves information on a specific Agent Cluster.')
 @click.argument('args', nargs=-1, metavar='agentclusterid=value agentclustername=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_agent_cluster(uac, args, output=None, select=None):
+def get_agent_cluster(uac: UniversalController, args, output=None, select=None):
+    """
+    Gets details of an agent cluster.
+
+    Args:
+        agent_cluster_id: agentclusterid
+        agent_cluster_name: agentclustername
+    """
     vars_dict = process_input(args)
     response = uac.agent_clusters.get_agent_cluster(**vars_dict)
     process_output(output, select, response)
 
 
 @agent_cluster.command('update', short_help='Modifies the Agent Cluster specified by the sysId.')
 @click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value name=value description=value opswise_groups=value strict_bsrvc_membership=value distribution=value network_alias=value network_alias_port=value resolution_status=value resolution_description=value last_resolution=value limit_type=value limit_amount=value current_count=value suspended=value suspended_on=value resumed_on=value agent_limit_type=value agent_limit_amount=value last_agent_used=value ignore_inactive_agents=value ignore_suspended_agents=value retain_sys_ids=value agents=value notifications=value type=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_agent_cluster(uac, args, output=None, input=None, select=None):
+def update_agent_cluster(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.agent_clusters.update_agent_cluster(**vars_dict)
     process_output(output, select, response)
 
 
 @agent_cluster.command('create', short_help='Creates a new Agent Cluster.')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_agent_cluster(uac, args, output=None, input=None, select=None, ignore_ids=False):
+def create_agent_cluster(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
     response = uac.agent_clusters.create_agent_cluster(**vars_dict)
     process_output(output, select, response)
 
 
 @agent_cluster.command('delete', short_help='Deletes a specific Agent Cluster.')
 @click.argument('args', nargs=-1, metavar='agentclusterid=value agentclustername=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_agent_cluster(uac, args, output=None, select=None):
+def delete_agent_cluster(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.agent_clusters.delete_agent_cluster(**vars_dict)
     process_output(output, select, response)
 
 
 @agent_cluster.command('list', short_help='Retrieves information on all Agent Clusters.')
 @click.argument('args', nargs=-1, metavar='')
 @click.pass_obj
 @output_option
 @select_option
-def list_agent_clusters(uac, args, output=None, select=None):
+def list_agent_clusters(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.agent_clusters.list_agent_clusters(**vars_dict)
     process_output(output, select, response)
 
 
 @agent_cluster.command('list_advanced', short_help='Retrieves Agent Cluster details using specific query parameters.')
 @click.argument('args', nargs=-1, metavar='agentclustername=value type=value business_services=value')
 @click.pass_obj
 @output_option
 @select_option
-def list_agent_clusters_advanced(uac, args, output=None, select=None):
+def list_agent_clusters_advanced(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.agent_clusters.list_agent_clusters_advanced(**vars_dict)
     process_output(output, select, response)
 
 
 @agent_cluster.command('get_selected_agent', short_help='Retrieves information on a specific Agent from an Agent Cluster for which a Distribution method of Any or Lowest CPU Utilization is specified.')
 @click.argument('args', nargs=-1, metavar='agentclustername=value ignoreexecutionlimit=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_selected_agent(uac, args, output=None, select=None):
+def get_selected_agent(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.agent_clusters.get_selected_agent(**vars_dict)
     process_output(output, select, response)
 
 
 @agent_cluster.command('resolve_cluster', short_help='Resolves the Network Alias for the specified Agent Cluster.')
 @click.argument('args', nargs=-1, metavar='agent_cluster_name=value')
 @click.pass_obj
 @output_option
 @select_option
-def resolve_cluster(uac, args, output=None, select=None):
+def resolve_cluster(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.agent_clusters.resolve_cluster(**vars_dict)
     process_output(output, select, response)
 
 
 @agent_cluster.command('resume', short_help='Resumes the specified Agent Cluster.')
 @click.argument('args', nargs=-1, metavar='agent_cluster_name=value')
 @click.pass_obj
 @output_option
 @select_option
-def resume_cluster(uac, args, output=None, select=None):
+def resume_cluster(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.agent_clusters.resume_cluster(**vars_dict)
     process_output(output, select, response)
 
 
 @agent_cluster.command('set_task_execution_limit', short_help='Sets the task execution limit for the specified Agent Cluster.')
 @click.argument('args', nargs=-1, metavar='agent_cluster_name=value limit_type=value limit_amount=value')
 @click.pass_obj
 @output_option
 @select_option
-def set_cluster_task_execution_limit(uac, args, output=None, select=None):
+def set_cluster_task_execution_limit(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.agent_clusters.set_cluster_task_execution_limit(**vars_dict)
     process_output(output, select, response)
 
 
 @agent_cluster.command('suspend', short_help='Suspends the specified Agent Cluster.')
 @click.argument('args', nargs=-1, metavar='agent_cluster_name=value')
 @click.pass_obj
 @output_option
 @select_option
-def suspend_cluster(uac, args, output=None, select=None):
+def suspend_cluster(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.agent_clusters.suspend_cluster(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/audit.py` & `uac-cli-0.2.0/uac_cli/commands/audit.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 @click.group(name='audit', help='Audit commands for retrieving audit logs and information.')
 def audit():
     pass
 
 @audit.command('list', short_help='Get a list of audits')
 @click.argument('args', nargs=-1, metavar="auditType=auditType source=source status=status createdBy=createdBy tableName=tableName tableRecordName=tableRecordName updatedTimeType=updatedTimeType updatedTime=updatedTime tableKey=tableKey includeChildAudits=includeChildAudits")
 @click.pass_obj
 @output_option
 @select_option
-def list(uac, args, output=None, select=None):
+def list(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.audits.list_audit(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/bundle.py` & `uac-cli-0.2.0/uac_cli/commands/bundle.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 @click.group(help='Bundle management commands, including operations to list, create, and delete bundles.')
 def bundle():
     pass
 
@@ -16,185 +17,185 @@
 
 
 @bundle.command('promote', short_help='Promote a Bundle or schedule the promotion of a Bundle.')
 @click.argument('args', nargs=-1, metavar='id=value name=value promotion_target_id=value promotion_target_name=value notification_option=value override_user=value override_password=value date=value time=value schedule=value create_snapshot=value allow_unv_tmplt_changes=value override_token=value')
 @click.pass_obj
 @output_option
 @select_option
-def promote(uac, args, output=None, select=None):
+def promote(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.bundles.promote(**vars_dict)
     process_output(output, select, response)
 
 
 @bundle.command('get', short_help='Retrieve Bundle details using specific query parameters.')
 @click.argument('args', nargs=-1, metavar='bundleid=value bundlename=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_bundle(uac, args, output=None, select=None):
+def get_bundle(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.bundles.get_bundle(**vars_dict)
     process_output(output, select, response)
 
 
 @bundle.command('update', short_help='Modifies the Bundle specified by the sysId.')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value name=value sys_id=value description=value opswise_groups=value default_promotion_target=value exclude_on_existence=value follow_references=value promote_bundle_definition=value promote_by_business_services=value visible_to=value bundle_agent_clusters=value bundle_applications=value bundle_business_services=value bundle_calendars=value bundle_credentials=value bundle_custom_days=value bundle_database_connections=value bundle_email_connections=value bundle_email_templates=value bundle_o_auth_clients=value bundle_peoplesoft_connections=value bundle_reports=value bundle_sap_connections=value bundle_scripts=value bundle_snmp_managers=value bundle_tasks=value bundle_triggers=value bundle_universal_event_templates=value bundle_universal_templates=value bundle_variables=value bundle_virtual_resources=value version=value exclude_related=value export_release_level=value export_table=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_bundle(uac, args, output=None, input=None, select=None):
+def update_bundle(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.bundles.update_bundle(**vars_dict)
     process_output(output, select, response)
 
 
 @bundle.command('create', short_help='Creates a Bundle.')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_bundle(uac, args, output=None, input=None, select=None, ignore_ids=False):
+def create_bundle(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
     response = uac.bundles.create_bundle(**vars_dict)
     process_output(output, select, response)
 
 
 @bundle.command('delete', short_help='Deletes the specified Bundle.')
 @click.argument('args', nargs=-1, metavar='bundleid=value bundlename=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_bundle(uac, args, output=None, select=None):
+def delete_bundle(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.bundles.delete_bundle(**vars_dict)
     process_output(output, select, response)
 
 
 @bundle.command('create_by_date', short_help='Creates a Bundle by Date.')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_bundle_by_date(uac, args, output=None, input=None, select=None, ignore_ids=False):
+def create_bundle_by_date(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
     response = uac.bundles.create_bundle_by_date(**vars_dict)
     process_output(output, select, response)
 
 
 @bundle.command('get_report', short_help='Retrieve Bundle Report details using specific query parameters.')
 @click.argument('args', nargs=-1, metavar='bundleid=value bundlename=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_bundle_report(uac, args, output=None, select=None):
+def get_bundle_report(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.bundles.get_bundle_report(**vars_dict)
     process_output(output, select, response)
 
 
 @bundle.command('list', short_help='Retrieves information on all Bundles.')
 @click.argument('args', nargs=-1, metavar='bundlename=value business_services=value default_promotion_target=value')
 @click.pass_obj
 @output_option
 @select_option
-def list_bundles(uac, args, output=None, select=None):
+def list_bundles(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.bundles.list_bundles(**vars_dict)
     process_output(output, select, response)
 
 
 
 @promotion.command('cancel_promotion_schedule', short_help='Cancels the scheduled promotion of a Bundle.')
 @click.argument('args', nargs=-1, metavar='scheduleid=value bundleid=value bundlename=value date=value time=value')
 @click.pass_obj
 @output_option
 @select_option
-def cancel_promotion_schedule(uac, args, output=None, select=None):
+def cancel_promotion_schedule(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.bundles.cancel_promotion_schedule(**vars_dict)
     process_output(output, select, response)
 
 
 @promotion.command('delete', short_help='Deletes the scheduled promotion of a Bundle.')
 @click.argument('args', nargs=-1, metavar='scheduleid=value bundleid=value bundlename=value date=value time=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_promotion_schedule(uac, args, output=None, select=None):
+def delete_promotion_schedule(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.bundles.delete_promotion_schedule(**vars_dict)
     process_output(output, select, response)
 
 
 @promotion_target.command('get', short_help='Retrieve a specified Promotion Target details.')
 @click.argument('args', nargs=-1, metavar='targetname=value targetid=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_promotion_target(uac, args, output=None, select=None):
+def get_promotion_target(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.bundles.get_promotion_target(**vars_dict)
     process_output(output, select, response)
 
 
 @promotion_target.command('update', short_help='Modifies the specified Promotion Target.')
 @click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value retain_sys_ids=value name=value description=value uri=value user=value password=value authentication_method=value opswise_groups=value token=value agent_mappings=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_promotion_target(uac, args, output=None, input=None, select=None):
+def update_promotion_target(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.bundles.update_promotion_target(**vars_dict)
     process_output(output, select, response)
 
 
 @promotion_target.command('create', short_help='Creates a Promotion Target.')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_promotion_target(uac, args, output=None, input=None, select=None, ignore_ids=False):
+def create_promotion_target(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
     response = uac.bundles.create_promotion_target(**vars_dict)
     process_output(output, select, response)
 
 
 @promotion_target.command('delete', short_help='Deletes the specified Promotion Target.')
 @click.argument('args', nargs=-1, metavar='targetname=value targetid=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_promotion_target(uac, args, output=None, select=None):
+def delete_promotion_target(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.bundles.delete_promotion_target(**vars_dict)
     process_output(output, select, response)
 
 
 @promotion_target.command('list', short_help='Retrieves information on all Promotion Targets.')
 @click.argument('args', nargs=-1, metavar='targetname=value business_services=value')
 @click.pass_obj
 @output_option
 @select_option
-def list_promotion_targets(uac, args, output=None, select=None):
+def list_promotion_targets(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.bundles.list_promotion_targets(**vars_dict)
     process_output(output, select, response)
 
 
 @promotion_target.command('refresh_target_agents', short_help='None')
 @click.argument('args', nargs=-1, metavar='targetname=value targetid=value username=value password=value token=value')
 @click.pass_obj
 @output_option
 @select_option
-def refresh_target_agents(uac, args, output=None, select=None):
+def refresh_target_agents(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.bundles.refresh_target_agents(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/business_service.py` & `uac-cli-0.2.0/uac_cli/commands/business_service.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 @click.group(help='Commands to manage business services, enabling operations like listing, creating, and updating business services.')
 def business_service():
     pass
 
 
 @business_service.command('get', short_help='Retrieves information on a specific Business Service.')
 @click.argument('args', nargs=-1, metavar='busserviceid=value busservicename=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_business_service(uac, args, output=None, select=None):
+def get_business_service(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.business_services.get_business_service(**vars_dict)
     process_output(output, select, response)
 
 
 @business_service.command('update', short_help='Modifies the Business Service specified by the sysId.')
 @click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value name=value description=value retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_business_service(uac, args, output=None, input=None, select=None):
+def update_business_service(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.business_services.update_business_service(**vars_dict)
     process_output(output, select, response)
 
 
 @business_service.command('create', short_help='Creates a Business Service.')
 @click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value name=value description=value retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_business_service(uac, args, output=None, input=None, select=None, ignore_ids=False):
+def create_business_service(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
     response = uac.business_services.create_business_service(**vars_dict)
     process_output(output, select, response)
 
 
 @business_service.command('delete', short_help='Deletes a Business Service.')
 @click.argument('args', nargs=-1, metavar='busserviceid=value busservicename=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_business_service(uac, args, output=None, select=None):
+def delete_business_service(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.business_services.delete_business_service(**vars_dict)
     process_output(output, select, response)
 
 
 @business_service.command('list', short_help='Retrieves information on all Business Services.')
 @click.argument('args', nargs=-1, metavar='')
 @click.pass_obj
 @output_option
 @select_option
-def list_business_services(uac, args, output=None, select=None):
+def list_business_services(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.business_services.list_business_services(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/calendar.py` & `uac-cli-0.2.0/uac_cli/commands/calendar.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,120 +1,121 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 @click.group(help='Calendar-related commands for managing calendars and custom days within them.')
 def calendar():
     pass
 
 
 @calendar.command('get', short_help='Retrieves information on all Custom Days of a specific Calendar.')
 @click.argument('args', nargs=-1, metavar='calendarid=value calendarname=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_custom_days(uac, args, output=None, select=None):
+def get_custom_days(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.calendars.get_custom_days(**vars_dict)
     process_output(output, select, response)
 
 
 @calendar.command('add', short_help='Adds the specified Custom Day to the specified Calendar.')
 @click.argument('args', nargs=-1, metavar='calendarid=value calendarname=value customdayid=value customdayname=value')
 @click.pass_obj
 @output_option
 @select_option
-def add_custom_day(uac, args, output=None, select=None):
+def add_custom_day(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.calendars.add_custom_day(**vars_dict)
     process_output(output, select, response)
 
 
 @calendar.command('remove', short_help='Removes the specified Custom Day from a specific Calendar.')
 @click.argument('args', nargs=-1, metavar='calendarid=value calendarname=value customdayid=value customdayname=value')
 @click.pass_obj
 @output_option
 @select_option
-def remove_custom_day(uac, args, output=None, select=None):
+def remove_custom_day(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.calendars.remove_custom_day(**vars_dict)
     process_output(output, select, response)
 
 
 @calendar.command('get', short_help='Retrieves information on a specific Calendar.')
 @click.argument('args', nargs=-1, metavar='calendarid=value calendarname=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_calendar(uac, args, output=None, select=None):
+def get_calendar(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.calendars.get_calendar(**vars_dict)
     process_output(output, select, response)
 
 
 @calendar.command('update', short_help='Modifies the Calendar specified by the sysId.')
 @click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value name=value comments=value opswise_groups=value business_days=value first_quarter_start=value second_quarter_start=value third_quarter_start=value fourth_quarter_start=value retain_sys_ids=value first_day_of_week=value custom_days=value local_custom_days=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_calendar(uac, args, output=None, input=None, select=None):
+def update_calendar(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.calendars.update_calendar(**vars_dict)
     process_output(output, select, response)
 
 
 @calendar.command('create', short_help='Creates a new Calendar.')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_calendar(uac, args, output=None, input=None, select=None, ignore_ids=False):
+def create_calendar(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
     response = uac.calendars.create_calendar(**vars_dict)
     process_output(output, select, response)
 
 
 @calendar.command('delete', short_help='Deletes the specified Calendar.')
 @click.argument('args', nargs=-1, metavar='calendarid=value calendarname=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_calendar(uac, args, output=None, select=None):
+def delete_calendar(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.calendars.delete_calendar(**vars_dict)
     process_output(output, select, response)
 
 
 @calendar.command('list', short_help='Retrieves information on all Calendars.')
 @click.argument('args', nargs=-1, metavar='')
 @click.pass_obj
 @output_option
 @select_option
-def list_calendars(uac, args, output=None, select=None):
+def list_calendars(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.calendars.list_calendars(**vars_dict)
     process_output(output, select, response)
 
 
 @calendar.command('list_qualifying_dates_for_local_custom_day', short_help='Retrieves information on Qualifying Dates for a specific Local Custom Day.')
 @click.argument('args', nargs=-1, metavar='customdayname=value calendarid=value calendarname=value')
 @click.pass_obj
 @output_option
 @select_option
-def list_qualifying_dates_for_local_custom_day(uac, args, output=None, select=None):
+def list_qualifying_dates_for_local_custom_day(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.calendars.list_qualifying_dates_for_local_custom_day(**vars_dict)
     process_output(output, select, response)
 
 
 @calendar.command('list_qualifying_periods', short_help='Retrieves information on Qualifying Periods for a specific Local Custom Day.')
 @click.argument('args', nargs=-1, metavar='customdayname=value calendarid=value calendarname=value')
 @click.pass_obj
 @output_option
 @select_option
-def list_qualifying_periods(uac, args, output=None, select=None):
+def list_qualifying_periods(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.calendars.list_qualifying_periods(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/cluster_node.py` & `uac-cli-0.2.0/uac_cli/commands/cluster_node.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 @click.group(help='Commands for managing cluster nodes, including retrieving information about the current node.')
 def cluster_node():
     pass
 
 
 @cluster_node.command('get', short_help='Retrieves information on the current Cluster Node.')
 @click.argument('args', nargs=-1, metavar='')
 @click.pass_obj
 @output_option
 @select_option
-def get_cluster_node(uac, args, output=None, select=None):
+def get_cluster_node(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.cluster_nodes.get_cluster_node(**vars_dict)
     process_output(output, select, response)
 
 
 @cluster_node.command('list', short_help='Retrieves information on all Cluster Nodes.')
 @click.argument('args', nargs=-1, metavar='')
 @click.pass_obj
 @output_option
 @select_option
-def list_cluster_nodes(uac, args, output=None, select=None):
+def list_cluster_nodes(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.cluster_nodes.list_cluster_nodes(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/config.py` & `uac-cli-0.2.0/uac_cli/commands/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pathlib import Path
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 from uac_cli.utils.config import write_config, read_config, ask_profile, read_profile, write_profile
 import json
 
 @click.group()
 def config():
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/connection.py` & `uac-cli-0.2.0/uac_cli/commands/connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 @click.group(help='Parent group for connection-related commands, serving as a namespace for database, email, and other connection types.')
 def connection():
     pass
 
@@ -24,233 +25,233 @@
 
 
 @database.command('get', short_help='Retrieves information on a specific Database Connection.')
 @click.argument('args', nargs=-1, metavar='connectionid=value connectionname=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_database_connection(uac, args, output=None, select=None):
+def get_database_connection(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.databaseconnections.get_database_connection(**vars_dict)
     process_output(output, select, response)
 
 
 @database.command('update', short_help='Modifies the Database Connection specified by the sysId.')
 @click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value name=value db_type=value db_url=value db_driver=value db_max_rows=value db_description=value credentials=value retain_sys_ids=value opswise_groups=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_database_connection(uac, args, output=None, input=None, select=None):
+def update_database_connection(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.databaseconnections.update_database_connection(**vars_dict)
     process_output(output, select, response)
 
 
 @database.command('create', short_help='Creates a Database Connection.')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_database_connection(uac, args, output=None, input=None, select=None, ignore_ids=False):
+def create_database_connection(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
     response = uac.databaseconnections.create_database_connection(**vars_dict)
     process_output(output, select, response)
 
 
 @database.command('delete', short_help='Deletes the specified Database Connection.')
 @click.argument('args', nargs=-1, metavar='connectionid=value connectionname=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_database_connection(uac, args, output=None, select=None):
+def delete_database_connection(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.databaseconnections.delete_database_connection(**vars_dict)
     process_output(output, select, response)
 
 
 @database.command('list', short_help='Retrieves information on all Database Connections.')
 @click.argument('args', nargs=-1, metavar='')
 @click.pass_obj
 @output_option
 @select_option
-def list_database_connections(uac, args, output=None, select=None):
+def list_database_connections(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.databaseconnections.list_database_connections(**vars_dict)
     process_output(output, select, response)
 
 
 @email.command('get', short_help='Retrieves information on a specific Email Connection.')
 @click.argument('args', nargs=-1, metavar='connectionid=value connectionname=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_email_connection(uac, args, output=None, select=None):
+def get_email_connection(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.emailconnections.get_email_connection(**vars_dict)
     process_output(output, select, response)
 
 
 @email.command('update', short_help='Modifies the Email Connection specified by the sysId.')
 @click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value name=value smtp=value smtp_port=value smtp_ssl=value smtp_starttls=value email_addr=value default_user=value default_pwd=value authentication=value authentication_type=value oauth_client=value system_connection=value type=value imap=value imap_port=value imap_ssl=value imap_starttls=value trash_folder=value opswise_groups=value description=value authorized=value retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_email_connection(uac, args, output=None, input=None, select=None):
+def update_email_connection(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.emailconnections.update_email_connection(**vars_dict)
     process_output(output, select, response)
 
 
 @email.command('create', short_help='Creates an Email Connection.')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_email_connection(uac, args, output=None, input=None, select=None, ignore_ids=False):
+def create_email_connection(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
     response = uac.emailconnections.create_email_connection(**vars_dict)
     process_output(output, select, response)
 
 
 @email.command('delete', short_help='Deletes the specified Email Connection.')
 @click.argument('args', nargs=-1, metavar='connectionid=value connectionname=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_email_connection(uac, args, output=None, select=None):
+def delete_email_connection(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.emailconnections.delete_email_connection(**vars_dict)
     process_output(output, select, response)
 
 
 @email.command('list', short_help='Retrieves information on all Email Connections.')
 @click.argument('args', nargs=-1, metavar='')
 @click.pass_obj
 @output_option
 @select_option
-def list_email_connections(uac, args, output=None, select=None):
+def list_email_connections(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.emailconnections.list_email_connections(**vars_dict)
     process_output(output, select, response)
 
 
 @peoplesoft.command('get', short_help='Retrieves information on a specific PeopleSoft Connection.')
 @click.argument('args', nargs=-1, metavar='connectionid=value connectionname=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_peoplesoft_connection(uac, args, output=None, select=None):
+def get_peoplesoft_connection(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.peoplesoftconnections.get_peoplesoft_connection(**vars_dict)
     process_output(output, select, response)
 
 
 @peoplesoft.command('update', short_help='Modifies the PeopleSoft Connection specified by the sysId.')
 @click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value name=value description=value server=value port=value endpoint=value credentials=value retain_sys_ids=value opswise_groups=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_peoplesoft_connection(uac, args, output=None, input=None, select=None):
+def update_peoplesoft_connection(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.peoplesoftconnections.update_peoplesoft_connection(**vars_dict)
     process_output(output, select, response)
 
 
 @peoplesoft.command('create', short_help='Creates a PeopleSoft Connection.')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_peoplesoft_connection(uac, args, output=None, input=None, select=None, ignore_ids=False):
+def create_peoplesoft_connection(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
     response = uac.peoplesoftconnections.create_peoplesoft_connection(**vars_dict)
     process_output(output, select, response)
 
 
 @peoplesoft.command('delete', short_help='Deletes the specified PeopleSoft Connection.')
 @click.argument('args', nargs=-1, metavar='connectionid=value connectionname=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_peoplesoft_connection(uac, args, output=None, select=None):
+def delete_peoplesoft_connection(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.peoplesoftconnections.delete_peoplesoft_connection(**vars_dict)
     process_output(output, select, response)
 
 
 @peoplesoft.command('list', short_help='Retrieves information on all PeopleSoft Connections.')
 @click.argument('args', nargs=-1, metavar='')
 @click.pass_obj
 @output_option
 @select_option
-def list_peoplesoft_connections(uac, args, output=None, select=None):
+def list_peoplesoft_connections(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.peoplesoftconnections.list_peoplesoft_connections(**vars_dict)
     process_output(output, select, response)
 
 
 
 @sap.command('get', short_help='Retrieves information on a specific SAP Connection.')
 @click.argument('args', nargs=-1, metavar='connectionid=value connectionname=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_sap_connection(uac, args, output=None, select=None):
+def get_sap_connection(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.sapconnections.get_sap_connection(**vars_dict)
     process_output(output, select, response)
 
 
 @sap.command('update', short_help='Modifies the SAP Connection specified by the sysId.')
 @click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value name=value sap_connection_type=value sap_ashost=value sap_client=value sap_sysnr=value sap_gwhost=value sap_gwserv=value sap_r3name=value sap_mshost=value sap_group=value opswise_groups=value description=value sap_saprouter=value sap_snc_mode=value sap_snc_lib=value sap_snc_myname=value sap_snc_partnername=value sap_snc_qop=value sap_snc_sso=value sap_mysapsso2=value sap_x509cert=value sap_use_symbolic_names=value retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_sap_connection(uac, args, output=None, input=None, select=None):
+def update_sap_connection(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.sapconnections.update_sap_connection(**vars_dict)
     process_output(output, select, response)
 
 
 @sap.command('create', short_help='Creates an SAP Connection.')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_sap_connection(uac, args, output=None, input=None, select=None, ignore_ids=False):
+def create_sap_connection(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
     response = uac.sapconnections.create_sap_connection(**vars_dict)
     process_output(output, select, response)
 
 
 @sap.command('delete', short_help='Deletes the specified SAP Connection.')
 @click.argument('args', nargs=-1, metavar='connectionid=value connectionname=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_sap_connection(uac, args, output=None, select=None):
+def delete_sap_connection(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.sapconnections.delete_sap_connection(**vars_dict)
     process_output(output, select, response)
 
 
 @sap.command('list', short_help='Retrieves information on all SAP Connections.')
 @click.argument('args', nargs=-1, metavar='')
 @click.pass_obj
 @output_option
 @select_option
-def list_sap_connections(uac, args, output=None, select=None):
+def list_sap_connections(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.sapconnections.list_sap_connections(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/credential.py` & `uac-cli-0.2.0/uac_cli/commands/credential.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,90 +1,91 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 @click.group(help='Credential management commands, including creating, updating, deleting, and changing passwords for credentials.')
 def credential():
     pass
 
 
 
 @credential.command('change_password', short_help='Changes the runtime password of the Credential based on name.')
 @click.argument('args', nargs=-1, metavar='name=value new_runtime_password=value')
 @click.pass_obj
 @output_option
 @select_option
-def change_password(uac, args, output=None, select=None):
+def change_password(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.credentials.change_password(**vars_dict)
     process_output(output, select, response)
 
 
 @credential.command('get', short_help='Retrieves information on a specific Credential.')
 @click.argument('args', nargs=-1, metavar='credentialid=value credentialname=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_credential(uac, args, output=None, select=None):
+def get_credential(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     uac.log.debug('vars_dict: %s', vars_dict)
     response = uac.credentials.get_credential(**vars_dict)
     process_output(output, select, response)
 
 
 @credential.command('update', short_help='Modifies the Credential specified by the sysId.')
 @click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value name=value description=value retain_sys_ids=value runtime_user=value runtime_password=value runtime_pass_phrase=value runtime_token=value provider=value provider_parameters=value runtime_key_location=value type=value opswise_groups=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_credential(uac, args, output=None, input=None, select=None):
+def update_credential(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.credentials.update_credential(**vars_dict)
     process_output(output, select, response)
 
 
 @credential.command('create', short_help='Creates a Credential.')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_credential(uac, args, output=None, input=None, select=None, ignore_ids=False):
+def create_credential(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
     response = uac.credentials.create_credential(**vars_dict)
     process_output(output, select, response)
 
 
 @credential.command('delete', short_help='Deletes the specified Credential.')
 @click.argument('args', nargs=-1, metavar='credentialid=value credentialname=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_credential(uac, args, output=None, select=None):
+def delete_credential(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.credentials.delete_credential(**vars_dict)
     process_output(output, select, response)
 
 
 @credential.command('list', short_help='Retrieves information on all Credentials.')
 @click.argument('args', nargs=-1, metavar='')
 @click.pass_obj
 @output_option
 @select_option
-def list_credentials(uac, args, output=None, select=None):
+def list_credentials(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.credentials.list_credentials(**vars_dict)
     process_output(output, select, response)
 
 
 @credential.command('test_provider', short_help='None')
 @click.argument('args', nargs=-1, metavar='credentialid=value credentialname=value')
 @click.pass_obj
 @output_option
 @select_option
-def test_provider(uac, args, output=None, select=None):
+def test_provider(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     uac.log.debug('vars_dict: %s', vars_dict)
     response = uac.credentials.test_provider(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/custom_day.py` & `uac-cli-0.2.0/uac_cli/commands/custom_day.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,77 +1,78 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 @click.group(help='Commands for managing custom days within calendars.')
 def custom_day():
     pass
 
 
 
 @custom_day.command('get', short_help='Retrieves information on a specific Custom Day.')
 @click.argument('args', nargs=-1, metavar='customdayid=value customdayname=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_custom_day(uac, args, output=None, select=None):
+def get_custom_day(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.custom_days.get_custom_day(**vars_dict)
     process_output(output, select, response)
 
 
 @custom_day.command('update', short_help='Modifies the Custom Day specified by the sysId.')
 @click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value name=value comments=value category=value ctype=value month=value dayofweek=value relfreq=value day=value date=value date_list=value adjustment=value adjustment_amount=value adjustment_type=value nth_amount=value nth_type=value retain_sys_ids=value observed_rules=value period=value holiday=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_custom_day(uac, args, output=None, input=None, select=None):
+def update_custom_day(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.custom_days.update_custom_day(**vars_dict)
     process_output(output, select, response)
 
 
 @custom_day.command('create', short_help='Creates a new Custom Day.')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_custom_day(uac, args, output=None, input=None, select=None, ignore_ids=False):
+def create_custom_day(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
     response = uac.custom_days.create_custom_day(**vars_dict)
     process_output(output, select, response)
 
 
 @custom_day.command('delete', short_help='Deletes a specific Custom Day.')
 @click.argument('args', nargs=-1, metavar='customdayid=value customdayname=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_custom_day(uac, args, output=None, select=None):
+def delete_custom_day(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.custom_days.delete_custom_day(**vars_dict)
     process_output(output, select, response)
 
 
 @custom_day.command('list', short_help='Retrieves information on all Custom Days.')
 @click.argument('args', nargs=-1, metavar='')
 @click.pass_obj
 @output_option
 @select_option
-def list_custom_days(uac, args, output=None, select=None):
+def list_custom_days(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.custom_days.list_custom_days(**vars_dict)
     process_output(output, select, response)
 
 
 @custom_day.command('list_qualifying_dates', short_help='Retrieves information on Qualifying Dates for a specific Custom Day.')
 @click.argument('args', nargs=-1, metavar='customdayid=value customdayname=value calendarid=value calendarname=value')
 @click.pass_obj
 @output_option
 @select_option
-def list_qualifying_dates(uac, args, output=None, select=None):
+def list_qualifying_dates(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.custom_days.list_qualifying_dates(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/email_template.py` & `uac-cli-0.2.0/uac_cli/commands/email_template.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,66 +1,67 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 @click.group(help='Commands to manage email templates, including operations for creation, deletion, and updating templates.')
 def email_template():
     pass
 
 
 
 @email_template.command('get', short_help='Retrieves information on a specific Email Template.')
 @click.argument('args', nargs=-1, metavar='templateid=value templatename=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_email_template(uac, args, output=None, select=None):
+def get_email_template(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.email_templates.get_email_template(**vars_dict)
     process_output(output, select, response)
 
 
 @email_template.command('update', short_help='Modifies the Email Template specified by the sysId.')
 @click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value template_name=value description=value opswise_groups=value connection=value reply_to=value to=value cc=value bcc=value subject=value body=value retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_email_template(uac, args, output=None, input=None, select=None):
+def update_email_template(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.email_templates.update_email_template(**vars_dict)
     process_output(output, select, response)
 
 
 @email_template.command('create', short_help='Creates an Email Template.')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_email_template(uac, args, output=None, input=None, select=None, ignore_ids=False):
+def create_email_template(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
     response = uac.email_templates.create_email_template(**vars_dict)
     process_output(output, select, response)
 
 
 @email_template.command('delete', short_help='Deletes the specified Email Template.')
 @click.argument('args', nargs=-1, metavar='templateid=value templatename=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_email_template(uac, args, output=None, select=None):
+def delete_email_template(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.email_templates.delete_email_template(**vars_dict)
     process_output(output, select, response)
 
 
 @email_template.command('list', short_help='Retrieves information on all Email Templates..')
 @click.argument('args', nargs=-1, metavar='')
 @click.pass_obj
 @output_option
 @select_option
-def list_email_template(uac, args, output=None, select=None):
+def list_email_template(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.email_templates.list_email_template(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/ldap.py` & `uac-cli-0.2.0/uac_cli/commands/ldap.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 @click.group(help='LDAP configuration commands, including updating LDAP settings.')
 def ldap():
     pass
 
 
 @ldap.command('get', short_help='None')
 @click.argument('args', nargs=-1, metavar='')
 @click.pass_obj
 @output_option
 @select_option
-def get_ldap(uac, args, output=None, select=None):
+def get_ldap(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.ldap.get_ldap(**vars_dict)
     process_output(output, select, response)
 
 
 @ldap.command('update', short_help='None')
 @click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value url=value bind_dn=value bind_password=value use_for_authentication=value allow_local_login=value base_dn=value user_id_attribute=value user_filter=value group_filter=value connect_timeout=value read_timeout=value user_membership_attribute=value group_member_attribute=value login_method=value user_target_ou_list=value group_target_ou_list=value mappings=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_ldap(uac, args, output=None, input=None, select=None):
+def update_ldap(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.ldap.update_ldap(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/metric.py` & `uac-cli-0.2.0/uac_cli/commands/metric.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 
 @click.group(help='Commands to scrape and retrieve metrics from the Universal Controller as Prometheus text.')
 def metrics():
     pass
 
 
 @metrics.command('get', short_help='Scrapes the Universal Controller metrics as Prometheus text.')
 @click.argument('args', nargs=-1, metavar='')
 @click.pass_obj
 @output_option
-def get_metrics(uac, args, output=None, select=None):
+def get_metrics(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.metrics.get_metrics(**vars_dict)
     process_output(output, select, response, text=True)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/oauth_client.py` & `uac-cli-0.2.0/uac_cli/commands/oauth_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,67 +1,68 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 @click.group(help='Commands for managing OAuth clients, including creating, updating, and listing OAuth clients.')
 def oauth_client():
     pass
 
 
 
 @oauth_client.command('get', short_help='Retrieves information on a specific OAuth Client')
 @click.argument('args', nargs=-1, metavar='oauthclientid=value oauthclientname=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_o_auth_client(uac, args, output=None, select=None):
+def get_o_auth_client(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.oauth_clients.get_o_auth_client(**vars_dict)
     process_output(output, select, response)
 
 
 @oauth_client.command('update', short_help='Modifies the OAuth Client specified by the sysId..')
 @click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value name=value description=value opswise_groups=value provider=value cluster_redirect_urls=value authorization_endpoint=value token_endpoint=value tenant_id=value client_id=value client_secret=value scopes=value retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_o_auth_client(uac, args, output=None, input=None, select=None):
+def update_o_auth_client(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.oauth_clients.update_o_auth_client(**vars_dict)
     process_output(output, select, response)
 
 
 @oauth_client.command('create', short_help='Creates an OAuth Client.')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_o_auth_client(uac, args, output=None, input=None, select=None, ignore_ids=False):
+def create_o_auth_client(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
     response = uac.oauth_clients.create_o_auth_client(**vars_dict)
     process_output(output, select, response)
 
 
 @oauth_client.command('delete', short_help='Deletes the specified OAuth Client.')
 @click.argument('args', nargs=-1, metavar='oauthclientid=value oauthclientname=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_o_auth_client(uac, args, output=None, select=None):
+def delete_o_auth_client(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.oauth_clients.delete_o_auth_client(**vars_dict)
     process_output(output, select, response)
 
 
 @oauth_client.command('list', short_help='Retrieves information on all OAuth Clients.')
 @click.argument('args', nargs=-1, metavar='')
 @click.pass_obj
 @output_option
 @select_option
-def list_o_auth_clients(uac, args, output=None, select=None):
+def list_o_auth_clients(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.oauth_clients.list_o_auth_clients(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/oms_server.py` & `uac-cli-0.2.0/uac_cli/commands/oms_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 
 @click.group(help='Commands related to OMS servers, including listing, creating, updating, and deleting OMS server configurations.')
 def oms_server():
     pass
 
 @oms_server.command('get', short_help='Retrieves information on a specific OMS Server.')
 @click.argument('args', nargs=-1, metavar='serveraddress=value serverid=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_oms_server(uac, args, output=None, select=None):
+def get_oms_server(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.oms_servers.get_oms_server(**vars_dict)
     process_output(output, select, response)
 
 
 @oms_server.command('update', short_help='Modifies the OMS Server specified by the sysId. To modify OMS Server properties without modifying related records, set excludeRelated = true.')
 @click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value server_address=value description=value opswise_groups=value status=value timeout=value session_status=value suspended=value last_connected=value last_connected_time=value authenticate=value retain_sys_ids=value notifications=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_oms_server(uac, args, output=None, input=None, select=None):
+def update_oms_server(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.oms_servers.update_oms_server(**vars_dict)
     process_output(output, select, response)
 
 
 @oms_server.command('create', short_help='Creates an OMS Server.')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_oms_server(uac, args, output=None, input=None, select=None, ignore_ids=False):
+def create_oms_server(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
     response = uac.oms_servers.create_oms_server(**vars_dict)
     process_output(output, select, response)
 
 
 @oms_server.command('delete', short_help='Deletes the specified OMS Server.')
 @click.argument('args', nargs=-1, metavar='serveraddress=value serverid=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_oms_server(uac, args, output=None, select=None):
+def delete_oms_server(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.oms_servers.delete_oms_server(**vars_dict)
     process_output(output, select, response)
 
 
 @oms_server.command('list', short_help='Retrieves the Server address or partial server address of all OMS servers.')
 @click.argument('args', nargs=-1, metavar='')
 @click.pass_obj
 @output_option
 @select_option
-def list_oms_servers(uac, args, output=None, select=None):
+def list_oms_servers(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.oms_servers.list_oms_servers(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/property.py` & `uac-cli-0.2.0/uac_cli/commands/property.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 @click.group(help='Property management commands, allowing users to list, create, update, and delete properties.')
 def property():
     pass
 
 
 @property.command('get', short_help='Retrieves information on a specific property.')
 @click.argument('args', nargs=-1, metavar='propertyname=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_property(uac, args, output=None, select=None):
+def get_property(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.properties.get_property(**vars_dict)
     process_output(output, select, response)
 
 
 @property.command('update', short_help='Modifies the specified property.')
 @click.argument('args', nargs=-1, metavar='')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_property(uac, args, output=None, input=None, select=None):
+def update_property(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.properties.update_property(**vars_dict)
     process_output(output, select, response)
 
 
 @property.command('list', short_help='Retrieves information on all properties.')
 @click.argument('args', nargs=-1, metavar='')
 @click.pass_obj
 @output_option
 @select_option
-def list_properties(uac, args, output=None, select=None):
+def list_properties(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.properties.list_properties(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/report.py` & `uac-cli-0.2.0/uac_cli/commands/report.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids, output_option_binary
 
 @click.group(help='Commands to run and manage reports, including running reports in various formats.')
 def report():
     pass
 
 
 @report.command('run_report', short_help='None')
 @click.argument('args', nargs=-1, metavar='reporttitle=value visibility=value groupname=value format=')
 @click.pass_obj
 @output_option_binary
 @select_option
 @click.option("--format", type=click.Choice(["csv", "tab", "pdf", "png", "xml", "json"]))
-def run_report(uac, args, output=None, select=None, format="csv"):
+def run_report(uac: UniversalController, args, output=None, select=None, format="csv"):
     vars_dict = process_input(args)
     response = uac.reports.run_report(report_format=format, **vars_dict)
     process_output(output, select, response, text=True, binary=(format in ["pdf", "png"]))
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/script.py` & `uac-cli-0.2.0/uac_cli/commands/script.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,65 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 @click.group(help='Script management commands, including creating, updating, deleting, and listing scripts.')
 def script():
     pass
 
 @script.command('get', short_help='None')
 @click.argument('args', nargs=-1, metavar='scriptid=value scriptname=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_script(uac, args, output=None, select=None):
+def get_script(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.scripts.get_script(**vars_dict)
     process_output(output, select, response)
 
 
 @script.command('update', short_help='None')
 @click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value script_name=value script_type=value description=value content=value resolve_variables=value retain_sys_ids=value opswise_groups=value notes=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_script(uac, args, output=None, input=None, select=None):
+def update_script(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.scripts.update_script(**vars_dict)
     process_output(output, select, response)
 
 
 @script.command('create', short_help='None')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_script(uac, args, output=None, input=None, select=None, ignore_ids=False):
+def create_script(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
     response = uac.scripts.create_script(**vars_dict)
     process_output(output, select, response)
 
 
 @script.command('delete', short_help='None')
 @click.argument('args', nargs=-1, metavar='scriptid=value scriptname=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_script(uac, args, output=None, select=None):
+def delete_script(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.scripts.delete_script(**vars_dict)
     process_output(output, select, response)
 
 
 @script.command('list', short_help='None')
 @click.argument('args', nargs=-1, metavar='')
 @click.pass_obj
 @output_option
 @select_option
-def list_scripts(uac, args, output=None, select=None):
+def list_scripts(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.scripts.list_scripts(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/server_operation.py` & `uac-cli-0.2.0/uac_cli/commands/server_operation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 @click.group(help='Commands for server operations, such as log rolling and temporary property changes.')
 def server_operation():
     pass
 
 @server_operation.command('roll_log', short_help='None')
 @click.argument('args', nargs=-1, metavar='')
 @click.pass_obj
 @output_option
 @select_option
-def roll_log(uac, args, output=None, select=None):
+def roll_log(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.serveroperations.roll_log(**vars_dict)
     process_output(output, select, response)
 
 
 @server_operation.command('temporary_property_change', short_help='None')
 @click.argument('args', nargs=-1, metavar='name=value value=value')
 @click.pass_obj
 @output_option
 @select_option
-def temporary_property_change(uac, args, output=None, select=None):
+def temporary_property_change(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.serveroperations.temporary_property_change(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/simulation.py` & `uac-cli-0.2.0/uac_cli/commands/simulation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 @click.group(help='Commands for managing simulations, including creating, updating, and deleting simulations.')
 def simulation():
     pass
 
 
 @simulation.command('get', short_help='None')
 @click.argument('args', nargs=-1, metavar='simulationid=value taskname=value workflowname=value vertexid=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_simulation(uac, args, output=None, select=None):
+def get_simulation(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.simulations.get_simulation(**vars_dict)
     process_output(output, select, response)
 
 
 @simulation.command('update', short_help='None')
 @click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value retain_sys_ids=value task=value workflow=value vertex_id=value status=value exit_code=value publish_status=value publish_late_start=value publish_late_finish=value publish_early_finish=value abort_actions=value email_notification_actions=value variable_actions=value snmp_notification_actions=value system_operation_actions=value other_options=value outputs=value variables_from_string=value variables=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_simulation(uac, args, output=None, input=None, select=None):
+def update_simulation(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.simulations.update_simulation(**vars_dict)
     process_output(output, select, response)
 
 
 @simulation.command('create', short_help='None')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_simulation(uac, args, output=None, input=None, select=None, ignore_ids=False):
+def create_simulation(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
     response = uac.simulations.create_simulation(**vars_dict)
     process_output(output, select, response)
 
 
 @simulation.command('delete', short_help='None')
 @click.argument('args', nargs=-1, metavar='simulationid=value taskname=value workflowname=value vertexid=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_simulation(uac, args, output=None, select=None):
+def delete_simulation(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.simulations.delete_simulation(**vars_dict)
     process_output(output, select, response)
 
 
 @simulation.command('list_simulations', short_help='None')
 @click.argument('args', nargs=-1, metavar='taskname=value workflowname=value')
 @click.pass_obj
 @output_option
 @select_option
-def list_simulations(uac, args, output=None, select=None):
+def list_simulations(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.simulations.list_simulations(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/system.py` & `uac-cli-0.2.0/uac_cli/commands/system.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 @click.group(help='System-related commands, including retrieving system status and information.')
 @click.pass_obj
 def system(uac):
     if uac is None:
         click.echo(click.style("No profiles found. run `uac config init`", fg="bright_red"))
         exit(255)
 
 @system.command('get', short_help='None')
 @click.pass_obj
 @output_option
 @select_option
-def get_status(uac, output=None, select=None):
+def get_status(uac: UniversalController, output=None, select=None):
     response = uac.system.get_status()
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/task.py` & `uac-cli-0.2.0/uac_cli/commands/task.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 @click.group(help='Task management commands, including creating, updating, deleting, and launching tasks.')
 def task():
     pass
 
 
 @task.command('get', short_help='None')
 @click.argument('args', nargs=-1, metavar='taskid=value taskname=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_task(uac, args, output=None, select=None):
+def get_task(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.tasks.get_task(**vars_dict)
     process_output(output, select, response)
 
 
 @task.command('update', short_help='None')
 @click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value variables=value notes=value actions=value retain_sys_ids=value name=value resolve_name_immediately=value summary=value opswise_groups=value start_held=value start_held_reason=value res_priority=value hold_resources=value credentials=value credentials_var=value credentials_var_check=value retry_maximum=value retry_indefinitely=value retry_interval=value retry_suppress_failure=value ls_enabled=value ls_type=value ls_time=value ls_day_constraint=value ls_nth_amount=value ls_duration=value lf_enabled=value lf_type=value lf_time=value lf_day_constraint=value lf_nth_amount=value lf_duration=value lf_offset_type=value lf_offset_percentage=value lf_offset_duration=value lf_offset_duration_unit=value ef_enabled=value ef_type=value ef_time=value ef_day_constraint=value ef_nth_amount=value ef_duration=value ef_offset_type=value ef_offset_percentage=value ef_offset_duration=value ef_offset_duration_unit=value user_estimated_duration=value cp_duration=value cp_duration_unit=value tw_wait_type=value tw_wait_amount=value tw_wait_time=value tw_wait_duration=value tw_wait_day_constraint=value tw_delay_type=value tw_delay_amount=value tw_delay_duration=value tw_workflow_only=value custom_field1=value custom_field2=value execution_restriction=value restriction_period=value restriction_period_before_date=value restriction_period_after_date=value restriction_period_before_time=value restriction_period_after_time=value restriction_period_date_list=value log_level=value exclusive_with_self=value min_run_time=value max_run_time=value avg_run_time=value last_run_time=value min_run_time_display=value max_run_time_display=value avg_run_time_display=value last_run_time_display=value run_count=value run_time=value first_run=value last_run=value simulation=value enforce_variables=value lock_variables=value override_instance_wait=value time_zone_pref=value virtual_resources=value exclusive_tasks=value type=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_task(uac, args, output=None, input=None, select=None):
+def update_task(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.tasks.update_task(**vars_dict)
     process_output(output, select, response)
 
 
 @task.command('create', short_help='None')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_task(uac, args, output=None, input=None, select=None, ignore_ids=False):
+def create_task(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
     response = uac.tasks.create_task(**vars_dict)
     process_output(output, select, response)
 
 
 @task.group(name='new', short_help='Create new tasks from template.')
 def new_task():
@@ -49,114 +50,114 @@
 
 
 @new_task.command('linux', short_help='Create new Linux tasks from template.')
 @click.argument('args', nargs=-1, metavar='name=taskname agent=agent_name command=[command to execute] script=[name of the script to execute]' )
 @click.pass_obj
 @output_option
 @select_option
-def linux_task(uac, args, output=None, select=None):
+def linux_task(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.tasks.create_linux_task(**vars_dict)
     process_output(output, select, response)
 
 @new_task.command('windows', short_help='Create new Windows tasks from template.')
 @click.argument('args', nargs=-1, metavar='name=taskname agent=agent_name command=[command to execute] script=[name of the script to execute]' )
 @click.pass_obj
 @output_option
 @select_option
-def linux_task(uac, args, output=None, select=None):
+def linux_task(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.tasks.create_windows_task(**vars_dict)
     process_output(output, select, response)
 
 @new_task.command('workflow', short_help='Create new Workflow tasks from template.')
 @click.argument('args', nargs=-1, metavar='name=[workflow name]' )
 @click.pass_obj
 @output_option
 @select_option
-def workflow_task(uac, args, output=None, select=None):
+def workflow_task(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.tasks.create_workflow(**vars_dict)
     process_output(output, select, response)
 
 @new_task.command('ftp', short_help='Create new file transfer tasks from template.')
 @click.argument('args', nargs=-1, metavar='name=taskname agent=agent_name server=remote_server credential_name=remote_server_credential command=[GET, PUT, MGET, MPUT] server_type=[SFTP, FTP, FTPS, FTPES] local_file=file_name remote_file=file_name' )
 @click.pass_obj
 @output_option
 @select_option
-def linux_task(uac, args, output=None, select=None):
+def linux_task(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.tasks.create_ftp_task(**vars_dict)
     process_output(output, select, response)
 
 @task.command('delete', short_help='None')
 @click.argument('args', nargs=-1, metavar='taskid=value taskname=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_task(uac, args, output=None, select=None):
+def delete_task(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.tasks.delete_task(**vars_dict)
     process_output(output, select, response)
 
 
 @task.command('list', short_help='None')
 @click.argument('args', nargs=-1, metavar='name=value enabled=value type=value business_services=value updated_time_type=value updated_time=value workflow_id=value workflow_name=value agent_name=value description=value tasks=value template_id=value template_name=value')
 @click.pass_obj
 @output_option
 @select_option
-def list_tasks(uac, args, output=None, select=None):
+def list_tasks(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.tasks.list_tasks(**vars_dict)
     process_output(output, select, response)
 
 
 @task.command('list_advanced', short_help='None')
 @click.argument('args', nargs=-1, metavar='taskname=value agentname=value type=value business_services=value workflowname=value workflowid=value updated_time=value updated_time_type=value templateid=value templatename=value')
 @click.pass_obj
 @output_option
 @select_option
-def list_tasks_advanced(uac, args, output=None, select=None):
+def list_tasks_advanced(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.tasks.list_tasks_advanced(**vars_dict)
     process_output(output, select, response)
 
 
 @task.command('list_workflow_list', short_help='None')
 @click.argument('args', nargs=-1, metavar='taskname=value taskid=value')
 @click.pass_obj
 @output_option
 @select_option
-def list_workflow_list(uac, args, output=None, select=None):
+def list_workflow_list(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.tasks.list_workflow_list(**vars_dict)
     process_output(output, select, response)
 
 
 @task.command('list_dependency_list_1', short_help='None')
 @click.argument('args', nargs=-1, metavar='taskinstancename=value taskinstanceid=value workflowinstancename=value criteria=value dependencytype=value')
 @click.pass_obj
 @output_option
 @select_option
-def list_dependency_list_1(uac, args, output=None, select=None):
+def list_dependency_list_1(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.tasks.list_dependency_list_1(**vars_dict)
     process_output(output, select, response)
 
 
 @task.command('launch', short_help='None')
 @click.argument('args', nargs=-1, metavar='name=value hold=value hold_reason=value time_zone=value virtual_resource_priority=value virtual_resources=value launch_reason=value simulate=value variables=[comma separated values] variables_map=value')
 @click.pass_obj
 @output_option
 @select_option
 @click.option('--wait', '-w', is_flag=True)
 @click.option('--timeout', '-t', type=int, default=300)
 @click.option('--interval', '-i', type=int, default=10)
 @click.option('--return_rc', '-r', is_flag=True)
-def task_launch(uac, args, output=None, select=None, wait=False, timeout=300, interval=10, return_rc=False):
+def task_launch(uac: UniversalController, args, output=None, select=None, wait=False, timeout=300, interval=10, return_rc=False):
     vars_dict = process_input(args)
     if "variables" in vars_dict:
         try:
             vars = vars_dict.get("variables").split(",")
             vars_dict['variables'] = []
             for var in vars:
                 k = var.split("=")
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/task_instance.py` & `uac-cli-0.2.0/uac_cli/commands/task_instance.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,286 +1,287 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 @click.group(help='Commands for managing task instances, including listing, updating, and controlling the execution of task instances.')
 def task_instance():
     pass
 
 @task_instance.command('delete', short_help='None')
 @click.argument('args', nargs=-1, metavar='name=value id=value criteria=value workflow_instance_name=value resource_name=value recursive=value predecessor_name=value wait_type=value wait_time=value wait_duration=value wait_seconds=value wait_day_constraint=value delay_type=value delay_duration=value delay_seconds=value halt=value priority_type=value task_status=value operational_memo=value hold_reason=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_task_instance(uac, args, output=None, select=None):
+def delete_task_instance(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.task_instances.delete_task_instance(**vars_dict)
     process_output(output, select, response)
 
 
 @task_instance.command('show_variables', short_help='None')
 @click.argument('args', nargs=-1, metavar='taskinstancename=value taskinstanceid=value workflowinstancename=value criteria=value fetchglobal=value')
 @click.pass_obj
 @output_option
 @select_option
-def show_variables(uac, args, output=None, select=None):
+def show_variables(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.task_instances.show_variables(**vars_dict)
     process_output(output, select, response)
 
 
 @task_instance.command('update_operational_memo', short_help='None')
 @click.argument('args', nargs=-1, metavar='memo=message taskinstancename=value taskinstanceid=value workflowinstancename=value criteria=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_operational_memo(uac, args, output=None, input=None, select=None):
+def update_operational_memo(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.task_instances.update_operational_memo(**vars_dict)
     process_output(output, select, response)
 
 
 @task_instance.command('set_priority', short_help='None')
 @click.argument('args', nargs=-1, metavar='name=value id=value criteria=value workflow_instance_name=value resource_name=value recursive=value predecessor_name=value wait_type=value wait_time=value wait_duration=value wait_seconds=value wait_day_constraint=value delay_type=value delay_duration=value delay_seconds=value halt=value priority_type=value task_status=value operational_memo=value hold_reason=value')
 @click.pass_obj
 @output_option
 @select_option
-def task_instance_set_priority(uac, args, output=None, select=None):
+def task_instance_set_priority(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.task_instances.set_priority(**vars_dict)
     process_output(output, select, response)
 
 @task_instance.command('set_complete', short_help='None')
 @click.argument('args', nargs=-1, metavar='name=value id=value criteria=value workflow_instance_name=value operationalMemo=value')
 @click.pass_obj
 @output_option
 @select_option
-def task_instance_set_priority(uac, args, output=None, select=None):
+def task_instance_set_priority(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.task_instances.set_complete(**vars_dict)
     process_output(output, select, response)
 
 
 @task_instance.command('set_timewait', short_help='None')
 @click.argument('args', nargs=-1, metavar='name=value id=value criteria=value workflow_instance_name=value resource_name=value recursive=value predecessor_name=value wait_type=value wait_time=value wait_duration=value wait_seconds=value wait_day_constraint=value delay_type=value delay_duration=value delay_seconds=value halt=value priority_type=value task_status=value operational_memo=value hold_reason=value')
 @click.pass_obj
 @output_option
 @select_option
-def set_timewait(uac, args, output=None, select=None):
+def set_timewait(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.task_instances.set_timewait(**vars_dict)
     process_output(output, select, response)
 
 
 @task_instance.command('list_dependency_list', short_help='None')
 @click.argument('args', nargs=-1, metavar='taskinstancename=value taskinstanceid=value workflowinstancename=value criteria=value dependencytype=value')
 @click.pass_obj
 @output_option
 @select_option
-def list_dependency_list(uac, args, output=None, select=None):
+def list_dependency_list(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.task_instances.list_dependency_list(**vars_dict)
     process_output(output, select, response)
 
 
 @task_instance.command('task_insert', short_help='None')
 @click.argument('args', nargs=-1, metavar='id=value name=value alias=value workflow_instance_id=value workflow_instance_name=value workflow_instance_criteria=value predecessors=value successors=value vertex_x=value vertex_y=value inherit_trigger_time=value')
 @click.pass_obj
 @output_option
 @select_option
-def task_insert(uac, args, output=None, select=None):
+def task_insert(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     if "predecessors" in vars_dict:
         vars_dict["predecessors"] = vars_dict["predecessors"].split(",")
     if "successors" in vars_dict:
         vars_dict["successors"] = vars_dict["successors"].split(",")
     response = uac.task_instances.task_insert(**vars_dict)
     process_output(output, select, response)
 
 
 @task_instance.command('cancel', short_help='None')
 @click.argument('args', nargs=-1, metavar='name=value id=value criteria=value workflow_instance_name=value resource_name=value recursive=value predecessor_name=value wait_type=value wait_time=value wait_duration=value wait_seconds=value wait_day_constraint=value delay_type=value delay_duration=value delay_seconds=value halt=value priority_type=value task_status=value operational_memo=value hold_reason=value')
 @click.pass_obj
 @output_option
 @select_option
-def task_instance_cancel(uac, args, output=None, select=None):
+def task_instance_cancel(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.task_instances.cancel(**vars_dict)
     process_output(output, select, response)
 
 
 @task_instance.command('clear_dependencies', short_help='None')
 @click.argument('args', nargs=-1, metavar='name=value id=value criteria=value workflow_instance_name=value resource_name=value recursive=value predecessor_name=value wait_type=value wait_time=value wait_duration=value wait_seconds=value wait_day_constraint=value delay_type=value delay_duration=value delay_seconds=value halt=value priority_type=value task_status=value operational_memo=value hold_reason=value')
 @click.pass_obj
 @output_option
 @select_option
-def task_instance_clear_dependencies(uac, args, output=None, select=None):
+def task_instance_clear_dependencies(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.task_instances.clear_dependencies(**vars_dict)
     process_output(output, select, response)
 
 
 @task_instance.command('clear_exclusive', short_help='None')
 @click.argument('args', nargs=-1, metavar='name=value id=value criteria=value workflow_instance_name=value resource_name=value recursive=value predecessor_name=value wait_type=value wait_time=value wait_duration=value wait_seconds=value wait_day_constraint=value delay_type=value delay_duration=value delay_seconds=value halt=value priority_type=value task_status=value operational_memo=value hold_reason=value')
 @click.pass_obj
 @output_option
 @select_option
-def task_instance_clear_exclusive(uac, args, output=None, select=None):
+def task_instance_clear_exclusive(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.task_instances.clear_exclusive(**vars_dict)
     process_output(output, select, response)
 
 
 @task_instance.command('clear_instance_wait', short_help='None')
 @click.argument('args', nargs=-1, metavar='name=value id=value criteria=value workflow_instance_name=value resource_name=value recursive=value predecessor_name=value wait_type=value wait_time=value wait_duration=value wait_seconds=value wait_day_constraint=value delay_type=value delay_duration=value delay_seconds=value halt=value priority_type=value task_status=value operational_memo=value hold_reason=value')
 @click.pass_obj
 @output_option
 @select_option
-def task_instance_clear_instance_wait(uac, args, output=None, select=None):
+def task_instance_clear_instance_wait(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.task_instances.clear_instance_wait(**vars_dict)
     process_output(output, select, response)
 
 
 @task_instance.command('clear_predecessors', short_help='None')
 @click.argument('args', nargs=-1, metavar='name=value id=value criteria=value workflow_instance_name=value resource_name=value recursive=value predecessor_name=value wait_type=value wait_time=value wait_duration=value wait_seconds=value wait_day_constraint=value delay_type=value delay_duration=value delay_seconds=value halt=value priority_type=value task_status=value operational_memo=value hold_reason=value')
 @click.pass_obj
 @output_option
 @select_option
-def task_instance_clear_predecessors(uac, args, output=None, select=None):
+def task_instance_clear_predecessors(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.task_instances.clear_predecessors(**vars_dict)
     process_output(output, select, response)
 
 
 @task_instance.command('clear_resources', short_help='None')
 @click.argument('args', nargs=-1, metavar='name=value id=value criteria=value workflow_instance_name=value resource_name=value recursive=value predecessor_name=value wait_type=value wait_time=value wait_duration=value wait_seconds=value wait_day_constraint=value delay_type=value delay_duration=value delay_seconds=value halt=value priority_type=value task_status=value operational_memo=value hold_reason=value')
 @click.pass_obj
 @output_option
 @select_option
-def task_instance_clear_resources(uac, args, output=None, select=None):
+def task_instance_clear_resources(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.task_instances.clear_resources(**vars_dict)
     process_output(output, select, response)
 
 
 @task_instance.command('clear_timewait', short_help='None')
 @click.argument('args', nargs=-1, metavar='name=value id=value criteria=value workflow_instance_name=value resource_name=value recursive=value predecessor_name=value wait_type=value wait_time=value wait_duration=value wait_seconds=value wait_day_constraint=value delay_type=value delay_duration=value delay_seconds=value halt=value priority_type=value task_status=value operational_memo=value hold_reason=value')
 @click.pass_obj
 @output_option
 @select_option
-def task_instance_clear_timewait(uac, args, output=None, select=None):
+def task_instance_clear_timewait(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.task_instances.clear_timewait(**vars_dict)
     process_output(output, select, response)
 
 
 @task_instance.command('force_finish', short_help='None')
 @click.argument('args', nargs=-1, metavar='name=value id=value criteria=value workflow_instance_name=value resource_name=value recursive=value predecessor_name=value wait_type=value wait_time=value wait_duration=value wait_seconds=value wait_day_constraint=value delay_type=value delay_duration=value delay_seconds=value halt=value priority_type=value task_status=value operational_memo=value hold_reason=value')
 @click.pass_obj
 @output_option
 @select_option
-def task_instance_force_finish(uac, args, output=None, select=None):
+def task_instance_force_finish(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.task_instances.force_finish(**vars_dict)
     process_output(output, select, response)
 
 
 @task_instance.command('force_finish_cancel', short_help='None')
 @click.argument('args', nargs=-1, metavar='name=value id=value criteria=value workflow_instance_name=value resource_name=value recursive=value predecessor_name=value wait_type=value wait_time=value wait_duration=value wait_seconds=value wait_day_constraint=value delay_type=value delay_duration=value delay_seconds=value halt=value priority_type=value task_status=value operational_memo=value hold_reason=value')
 @click.pass_obj
 @output_option
 @select_option
-def task_instance_force_finish_cancel(uac, args, output=None, select=None):
+def task_instance_force_finish_cancel(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.task_instances.force_finish_cancel(**vars_dict)
     process_output(output, select, response)
 
 
 @task_instance.command('hold', short_help='None')
 @click.argument('args', nargs=-1, metavar='name=value id=value criteria=value workflow_instance_name=value resource_name=value recursive=value predecessor_name=value wait_type=value wait_time=value wait_duration=value wait_seconds=value wait_day_constraint=value delay_type=value delay_duration=value delay_seconds=value halt=value priority_type=value task_status=value operational_memo=value hold_reason=value')
 @click.pass_obj
 @output_option
 @select_option
-def task_instance_hold(uac, args, output=None, select=None):
+def task_instance_hold(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.task_instances.hold(**vars_dict)
     process_output(output, select, response)
 
 
 @task_instance.command('release', short_help='None')
 @click.argument('args', nargs=-1, metavar='name=value id=value criteria=value workflow_instance_name=value resource_name=value recursive=value predecessor_name=value wait_type=value wait_time=value wait_duration=value wait_seconds=value wait_day_constraint=value delay_type=value delay_duration=value delay_seconds=value halt=value priority_type=value task_status=value operational_memo=value hold_reason=value')
 @click.pass_obj
 @output_option
 @select_option
-def task_instance_release(uac, args, output=None, select=None):
+def task_instance_release(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.task_instances.release(**vars_dict)
     process_output(output, select, response)
 
 
 @task_instance.command('rerun', short_help='None')
 @click.argument('args', nargs=-1, metavar='name=value id=value criteria=value workflow_instance_name=value resource_name=value recursive=value predecessor_name=value wait_type=value wait_time=value wait_duration=value wait_seconds=value wait_day_constraint=value delay_type=value delay_duration=value delay_seconds=value halt=value priority_type=value task_status=value operational_memo=value hold_reason=value')
 @click.pass_obj
 @output_option
 @select_option
-def task_instance_rerun(uac, args, output=None, select=None):
+def task_instance_rerun(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.task_instances.rerun(**vars_dict)
     process_output(output, select, response)
 
 
 @task_instance.command('retrieve_output', short_help='None')
 @click.argument('args', nargs=-1, metavar='taskinstancename=value taskinstanceid=value workflowinstancename=value criteria=value outputtype=value startline=value numlines=value scantext=value operational_memo=value')
 @click.pass_obj
 @output_option
 @select_option
-def task_instance_retrieve_output(uac, args, output=None, select=None):
+def task_instance_retrieve_output(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.task_instances.retrieve_output(**vars_dict)
     process_output(output, select, response)
 
 
 @task_instance.command('skip', short_help='None')
 @click.argument('args', nargs=-1, metavar='name=value id=value criteria=value workflow_instance_name=value resource_name=value recursive=value predecessor_name=value wait_type=value wait_time=value wait_duration=value wait_seconds=value wait_day_constraint=value delay_type=value delay_duration=value delay_seconds=value halt=value priority_type=value task_status=value operational_memo=value hold_reason=value')
 @click.pass_obj
 @output_option
 @select_option
-def task_instance_skip(uac, args, output=None, select=None):
+def task_instance_skip(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.task_instances.skip(**vars_dict)
     process_output(output, select, response)
 
 
 @task_instance.command('skip_path', short_help='None')
 @click.argument('args', nargs=-1, metavar='name=value id=value criteria=value workflow_instance_name=value resource_name=value recursive=value predecessor_name=value wait_type=value wait_time=value wait_duration=value wait_seconds=value wait_day_constraint=value delay_type=value delay_duration=value delay_seconds=value halt=value priority_type=value task_status=value operational_memo=value hold_reason=value')
 @click.pass_obj
 @output_option
 @select_option
-def task_instance_skip_path(uac, args, output=None, select=None):
+def task_instance_skip_path(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.task_instances.skip_path(**vars_dict)
     process_output(output, select, response)
 
 
 @task_instance.command('unskip', short_help='None')
 @click.argument('args', nargs=-1, metavar='name=value id=value criteria=value workflow_instance_name=value')
 @click.pass_obj
 @output_option
 @select_option
-def task_instance_unskip(uac, args, output=None, select=None):
+def task_instance_unskip(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.task_instances.unskip(**vars_dict)
     process_output(output, select, response)
 
 
 @task_instance.command('list', short_help='None')
 @click.argument('args', nargs=-1, metavar='name=value id=value criteria=value workflow_instance_name=value resource_name=value recursive=value predecessor_name=value wait_type=value wait_time=value wait_duration=value wait_seconds=value wait_day_constraint=value delay_type=value delay_duration=value delay_seconds=value halt=value priority_type=value task_status=value operational_memo=value hold_reason=value agent_name=value workflow_instance_criteria=value workflow_instance_id=value status=value type=value execution_user=value late_start=value late_finish=value early_finish=value started_late=value finished_late=value finished_early=value late=value late_early=value business_services=value updated_time_type=value updated_time=value sys_id=value instance_number=value task_id=value task_name=value custom_field1=value custom_field2=value trigger_id=value trigger_name=value workflow_definition_id=value workflow_definition_name=value status_description=value template_id=value template_name=value response_fields=value instance_output_type=value')
 @click.pass_obj
 @output_option
 @select_option
-def list_status(uac, args, output=None, select=None):
+def list_status(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.task_instances.list_status(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/trigger.py` & `uac-cli-0.2.0/uac_cli/commands/trigger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,133 +1,134 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 @click.group(help='Commands for managing triggers, including creating, updating, and listing triggers.')
 def trigger():
     pass
 
 
 @trigger.command('list_qualifying_times', short_help='None')
 @click.argument('args', nargs=-1, metavar='triggerid=value triggername=value count=value startdate=value')
 @click.pass_obj
 @output_option
 @select_option
-def list_qualifying_times(uac, args, output=None, select=None):
+def list_qualifying_times(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.triggers.list_qualifying_times(**vars_dict)
     process_output(output, select, response)
 
 
 @trigger.command('unassign_execution_user', short_help='None')
 @click.argument('args', nargs=-1, metavar='triggerid=value triggername=value')
 @click.pass_obj
 @output_option
 @select_option
-def unassign_execution_user(uac, args, output=None, select=None):
+def unassign_execution_user(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.triggers.unassign_execution_user(**vars_dict)
     process_output(output, select, response)
 
 @trigger.command('assign_execution_user', short_help='None')
 @click.argument('args', nargs=-1, metavar='triggerid=value triggername=value username=username password=password')
 @click.pass_obj
 @output_option
 @select_option
-def unassign_execution_user(uac, args, output=None, select=None):
+def unassign_execution_user(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.triggers.assign_execution_user_to_trigger(**vars_dict)
     process_output(output, select, response)
 
 
 @trigger.command('create', short_help='None')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_temp_trigger(uac, args, output=None, input=None, select=None, ignore_ids=False):
+def create_temp_trigger(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
     response = uac.triggers.create_temp_trigger(**vars_dict)
     process_output(output, select, response)
 
 
 @trigger.command('get', short_help='None')
 @click.argument('args', nargs=-1, metavar='triggerid=value triggername=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_trigger(uac, args, output=None, select=None):
+def get_trigger(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.triggers.get_trigger(**vars_dict)
     process_output(output, select, response)
 
 
 @trigger.command('update', short_help='None')
 @click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value retain_sys_ids=value name=value description=value calendar=value enabled=value forecast=value restriction=value restriction_simple=value restriction_complex=value situation=value action=value restriction_mode=value restriction_adjective=value restriction_nth_amount=value restriction_noun=value restriction_nouns=value restriction_qualifier=value restriction_qualifiers=value skip_count=value skip_active=value simulation_option=value time_zone=value execution_user=value opswise_groups=value tasks=value retention_duration_purge=value retention_duration=value retention_duration_unit=value rd_exclude_backup=value skip_condition=value skip_restriction=value skip_after_date=value skip_after_time=value skip_before_date=value skip_before_time=value skip_date_list=value enabled_by=value enabled_time=value disabled_by=value disabled_time=value next_scheduled_time=value enforce_variables=value lock_variables=value custom_field1=value custom_field2=value variables=value notes=value restriction_qualifiers_from_string=value restriction_nouns_from_string=value type=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_trigger(uac, args, output=None, input=None, select=None):
+def update_trigger(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.triggers.update_trigger(**vars_dict)
     process_output(output, select, response)
 
 @trigger.command('enable_disable', short_help='None')
 @click.argument('args', nargs=-1, metavar='enable=boolean name=triggername')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def enable_disable(uac, args, output=None, input=None, select=None):
+def enable_disable(uac: UniversalController, args, output=None, input=None, select=None):
     _payload = [create_payload(args)]
     response = uac.triggers.enable_disable(payload=_payload)
     process_output(output, select, response)
 
 
 @trigger.command('create', short_help='None')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_trigger(uac, args, output=None, input=None, select=None, ignore_ids=False):
+def create_trigger(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
     response = uac.triggers.create_trigger(**vars_dict)
     process_output(output, select, response)
 
 
 @trigger.command('delete', short_help='None')
 @click.argument('args', nargs=-1, metavar='triggerid=value triggername=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_trigger(uac, args, output=None, select=None):
+def delete_trigger(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.triggers.delete_trigger(**vars_dict)
     process_output(output, select, response)
 
 
 @trigger.command('list', short_help='None')
 @click.argument('args', nargs=-1, metavar='name=value enabled=value type=value business_services=value updated_time_type=value updated_time=value workflow_id=value workflow_name=value agent_name=value description=value tasks=value template_id=value template_name=value')
 @click.pass_obj
 @output_option
 @select_option
-def list_triggers(uac, args, output=None, select=None):
+def list_triggers(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.triggers.list_triggers(**vars_dict)
     process_output(output, select, response)
 
 
 @trigger.command('list_advanced', short_help='None')
 @click.argument('args', nargs=-1, metavar='triggername=value type=value business_services=value enabled=value tasks=value description=value')
 @click.pass_obj
 @output_option
 @select_option
-def list_triggers_advanced(uac, args, output=None, select=None):
+def list_triggers_advanced(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.triggers.list_triggers_advanced(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/universal_event.py` & `uac-cli-0.2.0/uac_cli/commands/universal_event.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 @click.group(help='Commands related to universal events, including publishing and managing universal events.')
 def universal_event():
     pass
 
 @universal_event.command('publish', short_help='None')
 @click.argument('args', nargs=-1, metavar='name=value business_services=value ttl=value attributes=value')
 @click.pass_obj
 @output_option
 @select_option
-def publish(uac, args, output=None, select=None):
+def publish(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.universal_events.publish(**vars_dict)
     process_output(output, select, response)
 
 
 @universal_event.command('pushg', short_help='None')
 @click.argument('args', nargs=-1, metavar='payload=value')
 @click.pass_obj
 @output_option
 @select_option
-def pushg(uac, args, output=None, select=None):
+def pushg(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.universal_events.pushg(**vars_dict)
     process_output(output, select, response)
 
 
 @universal_event.command('push', short_help='None')
 @click.argument('args', nargs=-1, metavar='')
 @click.pass_obj
 @output_option
 @select_option
-def push(uac, args, output=None, select=None):
+def push(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.universal_events.push(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/universal_event_template.py` & `uac-cli-0.2.0/uac_cli/commands/universal_event_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 
 @click.group(help='Commands for managing universal event templates, including creating, updating, and deleting templates.')
 def universal_event_template():
     pass
 
 @universal_event_template.command('get', short_help='None')
 @click.argument('args', nargs=-1, metavar='templateid=value templatename=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_universal_event_template(uac, args, output=None, select=None):
+def get_universal_event_template(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.universal_event_templates.get_universal_event_template(**vars_dict)
     process_output(output, select, response)
 
 
 @universal_event_template.command('update', short_help='None')
 @click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value name=value label=value description=value ttl=value attributes_policy=value attributes=value metric_type=value metric_name=value metric_value_attribute=value metric_unit=value metric_label_attributes=value metric_optional_labels=value retain_sys_ids=value attributes_from_string=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_universal_event_template(uac, args, output=None, input=None, select=None):
+def update_universal_event_template(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.universal_event_templates.update_universal_event_template(**vars_dict)
     process_output(output, select, response)
 
 
 @universal_event_template.command('create', short_help='None')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_universal_event_template(uac, args, output=None, input=None, select=None, ignore_ids=False):
+def create_universal_event_template(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
     response = uac.universal_event_templates.create_universal_event_template(**vars_dict)
     process_output(output, select, response)
 
 
 @universal_event_template.command('delete', short_help='None')
 @click.argument('args', nargs=-1, metavar='templateid=value templatename=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_universal_event_template(uac, args, output=None, select=None):
+def delete_universal_event_template(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.universal_event_templates.delete_universal_event_template(**vars_dict)
     process_output(output, select, response)
 
 
 @universal_event_template.command('list', short_help='None')
 @click.argument('args', nargs=-1, metavar='templatename=value')
 @click.pass_obj
 @output_option
 @select_option
-def list_universal_event_templates(uac, args, output=None, select=None):
+def list_universal_event_templates(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.universal_event_templates.list_universal_event_templates(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/universal_template.py` & `uac-cli-0.2.0/uac_cli/commands/universal_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,122 +1,123 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 @click.group(help='Commands for managing universal templates, including template creation, deletion, and updating.')
 def universal_template():
     pass
 
 
 @universal_template.command('get', short_help='None')
 @click.argument('args', nargs=-1, metavar='templateid=value templatename=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_universal_template(uac, args, output=None, select=None):
+def get_universal_template(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.universal_templates.get_universal_template(**vars_dict)
     process_output(output, select, response)
 
 
 @universal_template.command('update', short_help='None')
 @click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value name=value description=value extension=value variable_prefix=value log_level=value icon_filename=value icon_filesize=value icon_date_created=value template_type=value agent_type=value use_common_script=value script=value script_unix=value script_windows=value script_type_windows=value always_cancel_on_finish=value send_variables=value credentials=value credentials_var=value credentials_var_check=value agent=value agent_var=value agent_var_check=value agent_cluster=value agent_cluster_var=value agent_cluster_var_check=value broadcast_cluster=value broadcast_cluster_var=value broadcast_cluster_var_check=value runtime_dir=value environment=value send_environment=value exit_codes=value exit_code_processing=value exit_code_text=value exit_code_output=value output_type=value output_content_type=value output_path_expression=value output_condition_operator=value output_condition_value=value output_condition_strategy=value auto_cleanup=value output_return_type=value output_return_file=value output_return_sline=value output_return_nline=value output_return_text=value wait_for_output=value output_failure_only=value elevate_user=value desktop_interact=value create_console=value agent_fields_restriction=value credential_fields_restriction=value environment_variables_fields_restriction=value exit_code_processing_fields_restriction=value automatic_output_retrieval_fields_restriction=value retain_sys_ids=value min_release_level=value environment_from_string=value fields=value commands=value events=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_universal_template(uac, args, output=None, input=None, select=None):
+def update_universal_template(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.universal_templates.update_universal_template(**vars_dict)
     process_output(output, select, response)
 
 
 @universal_template.command('create', short_help='None')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_universal_template(uac, args, output=None, input=None, select=None, ignore_ids=False):
+def create_universal_template(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
     response = uac.universal_templates.create_universal_template(**vars_dict)
     process_output(output, select, response)
 
 
 @universal_template.command('delete', short_help='None')
 @click.argument('args', nargs=-1, metavar='templateid=value templatename=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_universal_template(uac, args, output=None, select=None):
+def delete_universal_template(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.universal_templates.delete_universal_template(**vars_dict)
     process_output(output, select, response)
 
 
 @universal_template.command('get', short_help='None')
 @click.argument('args', nargs=-1, metavar='templateid=value templatename=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_extension_archive(uac, args, output=None, select=None):
+def get_extension_archive(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.universal_templates.get_extension_archive(**vars_dict)
     process_output(output, select, response)
 
 
 @universal_template.command('update_extension_archive', short_help='None')
 @click.argument('args', nargs=-1, metavar='')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_extension_archive(uac, args, output=None, input=None, select=None):
+def update_extension_archive(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.universal_templates.update_extension_archive(**vars_dict)
     process_output(output, select, response)
 
 
 @universal_template.command('delete_extension_archive', short_help='None')
 @click.argument('args', nargs=-1, metavar='templateid=value templatename=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_extension_archive(uac, args, output=None, select=None):
+def delete_extension_archive(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.universal_templates.delete_extension_archive(**vars_dict)
     process_output(output, select, response)
 
 
 @universal_template.command('export', short_help='None')
 @click.argument('args', nargs=-1, metavar='templateid=value templatename=value exclude_extension=value')
 @click.pass_obj
 @output_option
 @select_option
-def export_template(uac, args, output=None, select=None):
+def export_template(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.universal_templates.export_template(**vars_dict)
     process_output(output, select, response)
 
 
 @universal_template.command('set_icon', short_help='None')
 @click.argument('args', nargs=-1, metavar='templateid=value templatename=value')
 @click.pass_obj
 @output_option
 @select_option
-def set_template_icon(uac, args, output=None, select=None):
+def set_template_icon(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.universal_templates.set_template_icon(**vars_dict)
     process_output(output, select, response)
 
 
 @universal_template.command('list', short_help='None')
 @click.argument('args', nargs=-1, metavar='templatename=value')
 @click.pass_obj
 @output_option
 @select_option
-def list_universal_templates(uac, args, output=None, select=None):
+def list_universal_templates(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.universal_templates.list_universal_templates(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/user.py` & `uac-cli-0.2.0/uac_cli/commands/variable.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,115 +1,91 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
-@click.group(help='User management commands, including operations for creating, updating, and deleting users, as well as managing authentication tokens.')
-def user():
-    pass
-
-
 
-@user.command('change_password', short_help='None')
-@click.argument('args', nargs=-1, metavar='name=value new_password=value')
-@click.pass_obj
-@output_option
-@select_option
-def change_user_password(uac, args, output=None, select=None):
-    vars_dict = process_input(args)
-    response = uac.users.change_user_password(**vars_dict)
-    process_output(output, select, response)
+@click.group(help='Commands for managing variables, including setting, updating, and listing variables.')
+def variable():
+    pass
 
 
-@user.command('get', short_help='None')
-@click.argument('args', nargs=-1, metavar='userid=value username=value show_tokens=value')
+@variable.command('get', short_help='None')
+@click.argument('args', nargs=-1, metavar='variableid=value variablename=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_user(uac, args, output=None, select=None):
+def get_variable(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
-    response = uac.users.get_user(**vars_dict)
+    response = uac.variables.get_variable(**vars_dict)
     process_output(output, select, response)
 
 
-@user.command('update', short_help='None')
-@click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value retain_sys_ids=value user_name=value user_password=value first_name=value middle_name=value last_name=value email=value title=value active=value locked_out=value password_needs_reset=value business_phone=value mobile_phone=value time_zone=value department=value manager=value browser_access=value command_line_access=value web_service_access=value login_method=value impersonate=value permissions=value user_roles=value tokens=value')
+@variable.command('update', short_help='None')
+@click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value name=value value=value description=value opswise_groups=value retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_user(uac, args, output=None, input=None, select=None):
+def update_variable(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
-    response = uac.users.update_user(**vars_dict)
+    response = uac.variables.update_variable(**vars_dict)
     process_output(output, select, response)
 
 
-@user.command('create', short_help='None')
-@click.argument('args', nargs=-1, metavar='user_name="newuser" user_password="abc123"')
+@variable.command('create', short_help='None')
+@click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_user(uac, args, output=None, input=None, select=None, ignore_ids=False):
-    vars_dict = process_input(args, input, ignore_ids, ignore_ids)
-    uac.log.debug(vars_dict)
-    uac.log.debug(args)
-    vars_dict['payload']["userPassword"] = vars_dict.get('userPassword', vars_dict.get('user_password'))
-    response = uac.users.create_user(**vars_dict)
+def create_variable(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
+    vars_dict = process_input(args, input, ignore_ids)
+    response = uac.variables.create_variable(**vars_dict)
     process_output(output, select, response)
 
 
-@user.command('delete', short_help='None')
-@click.argument('args', nargs=-1, metavar='userid=value username=value')
+@variable.command('delete', short_help='None')
+@click.argument('args', nargs=-1, metavar='variableid=value variablename=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_user(uac, args, output=None, select=None):
+def delete_variable(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
-    response = uac.users.delete_user(**vars_dict)
-    process_output(output, select, response)
-
-
-@user.command('create_token', short_help='None')
-@click.argument('args', nargs=-1, metavar='retain_sys_ids=value user_id=uuid user_name=userName name=token_name expiration=yyyy-mm-dd')
-@click.pass_obj
-@output_option
-@input_option
-@select_option
-def create_user_token(uac, args, output=None, input=None, select=None):
-    vars_dict = process_input(args, input)
-    response = uac.users.create_user_token(**vars_dict)
+    response = uac.variables.delete_variable(**vars_dict)
     process_output(output, select, response)
 
 
-@user.command('revoke_token', short_help='None')
-@click.argument('args', nargs=-1, metavar='userid=value username=value tokenname=value')
+@variable.command('list', short_help='None')
+@click.argument('args', nargs=-1, metavar='variable_name=value scope=value task_name=value trigger_name=value')
 @click.pass_obj
 @output_option
 @select_option
-def revoke_user_token(uac, args, output=None, select=None):
+def list_variables(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
-    response = uac.users.revoke_user_token(**vars_dict)
+    response = uac.variables.list_variables(**vars_dict)
     process_output(output, select, response)
 
 
-@user.command('list_auth_tokens', short_help='None')
-@click.argument('args', nargs=-1, metavar='userid=value username=value')
+@variable.command('list_advanced', short_help='None')
+@click.argument('args', nargs=-1, metavar='scope=value variablename=value taskname=value triggername=value business_services=value')
 @click.pass_obj
 @output_option
 @select_option
-def list_auth_tokens(uac, args, output=None, select=None):
+def list_variables_advanced(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
-    response = uac.users.list_auth_tokens(**vars_dict)
+    response = uac.variables.list_variables_advanced(**vars_dict)
     process_output(output, select, response)
 
 
-@user.command('list', short_help='None')
-@click.argument('args', nargs=-1, metavar='show_tokens=value')
+@variable.command('set', short_help='None')
+@click.argument('args', nargs=-1, metavar='scope=value create=value trigger=value task=value variable=value')
 @click.pass_obj
 @output_option
+@input_option
 @select_option
-def list_users(uac, args, output=None, select=None):
-    vars_dict = process_input(args)
-    response = uac.users.list_users(**vars_dict)
+def variable_set(uac: UniversalController, args, output=None, input=None, select=None):
+    vars_dict = process_input(args, input)
+    response = uac.variables.variable_set(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/user_group.py` & `uac-cli-0.2.0/uac_cli/commands/user_group.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 
 @click.group(help='User group management commands, including listing, creating, updating, and deleting user groups.')
 def user_group():
     pass
@@ -10,58 +11,58 @@
 
 
 @user_group.command('get', short_help='None')
 @click.argument('args', nargs=-1, metavar='groupid=value groupname=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_user_group(uac, args, output=None, select=None):
+def get_user_group(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.user_groups.get_user_group(**vars_dict)
     process_output(output, select, response)
 
 
 @user_group.command('update', short_help='None')
 @click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value retain_sys_ids=value name=value email=value manager=value description=value parent=value ctrl_navigation_visibility=value navigation_visibility=value permissions=value group_roles=value group_members=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_user_group(uac, args, output=None, input=None, select=None):
+def update_user_group(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.user_groups.update_user_group(**vars_dict)
     process_output(output, select, response)
 
 
 @user_group.command('create', short_help='None')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_user_group(uac, args, output=None, input=None, select=None, ignore_ids=False):
+def create_user_group(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
     response = uac.user_groups.create_user_group(**vars_dict)
     process_output(output, select, response)
 
 
 @user_group.command('delete', short_help='None')
 @click.argument('args', nargs=-1, metavar='groupid=value groupname=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_user_group(uac, args, output=None, select=None):
+def delete_user_group(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.user_groups.delete_user_group(**vars_dict)
     process_output(output, select, response)
 
 
 @user_group.command('list', short_help='None')
 @click.argument('args', nargs=-1, metavar='')
 @click.pass_obj
 @output_option
 @select_option
-def list_user_groups(uac, args, output=None, select=None):
+def list_user_groups(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.user_groups.list_user_groups(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/variable.py` & `uac-cli-0.2.0/uac_cli/commands/webhook.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,99 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
-
-@click.group(help='Commands for managing variables, including setting, updating, and listing variables.')
-def variable():
+@click.group(help='Webhook management commands, including creating, updating, enabling, and disabling webhooks.')
+def webhook():
     pass
 
 
-@variable.command('get', short_help='None')
-@click.argument('args', nargs=-1, metavar='variableid=value variablename=value')
+@webhook.command('unassign_execution_user_1', short_help='None')
+@click.argument('args', nargs=-1, metavar='webhookid=value webhookname=value')
+@click.pass_obj
+@output_option
+@select_option
+def unassign_execution_user_1(uac: UniversalController, args, output=None, select=None):
+    vars_dict = process_input(args)
+    response = uac.webhooks.unassign_execution_user_1(**vars_dict)
+    process_output(output, select, response)
+
+
+@webhook.command('get', short_help='None')
+@click.argument('args', nargs=-1, metavar='webhookid=value webhookname=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_variable(uac, args, output=None, select=None):
+def get_webhook(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
-    response = uac.variables.get_variable(**vars_dict)
+    response = uac.webhooks.get_webhook(**vars_dict)
     process_output(output, select, response)
 
 
-@variable.command('update', short_help='None')
-@click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value name=value value=value description=value opswise_groups=value retain_sys_ids=value')
+@webhook.command('update', short_help='None')
+@click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value name=value description=value retain_sys_ids=value opswise_groups=value event=value action=value task=value url=value filter=value enabled_by=value enabled_time=value disabled_by=value disabled_time=value execution_user=value status=value status_description=value url_parameters=value http_headers=value http_auth=value credentials=value url_parameters_from_string=value http_headers_from_string=value event_business_service_criteria=value event_business_services=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_variable(uac, args, output=None, input=None, select=None):
+def update_webhook(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
-    response = uac.variables.update_variable(**vars_dict)
+    response = uac.webhooks.update_webhook(**vars_dict)
     process_output(output, select, response)
 
 
-@variable.command('create', short_help='None')
+@webhook.command('create', short_help='None')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_variable(uac, args, output=None, input=None, select=None, ignore_ids=False):
+def create_webhook(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
-    response = uac.variables.create_variable(**vars_dict)
+    response = uac.webhooks.create_webhook(**vars_dict)
     process_output(output, select, response)
 
 
-@variable.command('delete', short_help='None')
-@click.argument('args', nargs=-1, metavar='variableid=value variablename=value')
+@webhook.command('delete', short_help='None')
+@click.argument('args', nargs=-1, metavar='webhookid=value webhookname=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_variable(uac, args, output=None, select=None):
+def delete_webhook(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
-    response = uac.variables.delete_variable(**vars_dict)
+    response = uac.webhooks.delete_webhook(**vars_dict)
     process_output(output, select, response)
 
 
-@variable.command('list', short_help='None')
-@click.argument('args', nargs=-1, metavar='variable_name=value scope=value task_name=value trigger_name=value')
+@webhook.command('disable', short_help='None')
+@click.argument('args', nargs=-1, metavar='webhookid=value webhookname=value')
 @click.pass_obj
 @output_option
 @select_option
-def list_variables(uac, args, output=None, select=None):
+def disable_webhook(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
-    response = uac.variables.list_variables(**vars_dict)
+    response = uac.webhooks.disable_webhook(**vars_dict)
     process_output(output, select, response)
 
 
-@variable.command('list_advanced', short_help='None')
-@click.argument('args', nargs=-1, metavar='scope=value variablename=value taskname=value triggername=value business_services=value')
+@webhook.command('enable', short_help='None')
+@click.argument('args', nargs=-1, metavar='webhookid=value webhookname=value')
 @click.pass_obj
 @output_option
 @select_option
-def list_variables_advanced(uac, args, output=None, select=None):
+def enable_webhook(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
-    response = uac.variables.list_variables_advanced(**vars_dict)
+    response = uac.webhooks.enable_webhook(**vars_dict)
     process_output(output, select, response)
 
 
-@variable.command('set', short_help='None')
-@click.argument('args', nargs=-1, metavar='scope=value create=value trigger=value task=value variable=value')
+@webhook.command('list', short_help='None')
+@click.argument('args', nargs=-1, metavar='webhookname=value action=value business_services=value description=value event=value task=value taskname=value url=value')
 @click.pass_obj
 @output_option
-@input_option
 @select_option
-def variable_set(uac, args, output=None, input=None, select=None):
-    vars_dict = process_input(args, input)
-    response = uac.variables.variable_set(**vars_dict)
+def list_webhooks(uac: UniversalController, args, output=None, select=None):
+    vars_dict = process_input(args)
+    response = uac.webhooks.list_webhooks(**vars_dict)
     process_output(output, select, response)
-
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/virtual_resource.py` & `uac-cli-0.2.0/uac_cli/commands/virtual_resource.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,89 +1,90 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 @click.group(help='Commands related to virtual resources, including listing, creating, updating, and deleting virtual resources.')
 def virtual_resource():
     pass
 
 
 @virtual_resource.command('get', short_help='None')
 @click.argument('args', nargs=-1, metavar='resourceid=value resourcename=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_virtual_resource(uac, args, output=None, select=None):
+def get_virtual_resource(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.virtual_resources.get_virtual_resource(**vars_dict)
     process_output(output, select, response)
 
 
 @virtual_resource.command('update', short_help='None')
 @click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value name=value limit=value summary=value type=value opswise_groups=value retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_virtual_resource(uac, args, output=None, input=None, select=None):
+def update_virtual_resource(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.virtual_resources.update_virtual_resource(**vars_dict)
     process_output(output, select, response)
 
 
 @virtual_resource.command('create', short_help='None')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_virtual_resource(uac, args, output=None, input=None, select=None, ignore_ids=False):
+def create_virtual_resource(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
     response = uac.virtual_resources.create_virtual_resource(**vars_dict)
     process_output(output, select, response)
 
 
 @virtual_resource.command('delete', short_help='None')
 @click.argument('args', nargs=-1, metavar='resourceid=value resourcename=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_virtual_resource(uac, args, output=None, select=None):
+def delete_virtual_resource(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.virtual_resources.delete_virtual_resource(**vars_dict)
     process_output(output, select, response)
 
 
 @virtual_resource.command('list', short_help='None')
 @click.argument('args', nargs=-1, metavar='name=value resourcename=value type=value')
 @click.pass_obj
 @output_option
 @select_option
-def list_virtual_resources(uac, args, output=None, select=None):
+def list_virtual_resources(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.virtual_resources.list_virtual_resources(**vars_dict)
     process_output(output, select, response)
 
 
 @virtual_resource.command('list_advanced', short_help='None')
 @click.argument('args', nargs=-1, metavar='resourcename=value type=value business_services=value')
 @click.pass_obj
 @output_option
 @select_option
-def list_virtual_resources_advanced(uac, args, output=None, select=None):
+def list_virtual_resources_advanced(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.virtual_resources.list_virtual_resources_advanced(**vars_dict)
     process_output(output, select, response)
 
 
 @virtual_resource.command('update_limit', short_help='None')
 @click.argument('args', nargs=-1, metavar='sys_id=value name=value limit=value description=value type=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_limit(uac, args, output=None, input=None, select=None):
+def update_limit(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.virtual_resources.update_limit(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/commands/workflow.py` & `uac-cli-0.2.0/uac_cli/commands/workflow.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import click
+from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 
 @click.group(help='Workflow management commands, including operations for managing workflow vertices and edges, as well as running workflow forecasts.')
 def workflow():
     pass
@@ -10,111 +11,111 @@
 
 
 @workflow.command('get_edges', short_help='None')
 @click.argument('args', nargs=-1, metavar='workflowid=value workflowname=value sourceid=value targetid=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_edges(uac, args, output=None, select=None):
+def get_edges(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.workflows.get_edges(**vars_dict)
     process_output(output, select, response)
 
 
 @workflow.command('update_edge', short_help='None')
 @click.argument('args', nargs=-1, metavar='sys_id=value workflow_id=value condition=value straight_edge=value points=value source_id=value target_id=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_edge(uac, args, output=None, input=None, select=None):
+def update_edge(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.workflows.update_edge(**vars_dict)
     process_output(output, select, response)
 
 
 @workflow.command('add_edge', short_help='None')
 @click.argument('args', nargs=-1, metavar='workflowid=value workflowname=value condition=value straight_edge=value points=value source_id=value target_id=value')
 @click.pass_obj
 @output_option
 @select_option
-def add_edge(uac, args, output=None, select=None):
+def add_edge(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.workflows.add_edge(**vars_dict)
     process_output(output, select, response)
 
 
 @workflow.command('delete_edge', short_help='None')
 @click.argument('args', nargs=-1, metavar='workflowid=value workflowname=value sourceid=value targetid=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_edge(uac, args, output=None, select=None):
+def delete_edge(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.workflows.delete_edge(**vars_dict)
     process_output(output, select, response)
 
 
 @workflow.command('get_vertices', short_help='None')
 @click.argument('args', nargs=-1, metavar='workflowid=value workflowname=value taskid=value taskname=value taskalias=value vertexid=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_vertices(uac, args, output=None, select=None):
+def get_vertices(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.workflows.get_vertices(**vars_dict)
     process_output(output, select, response)
 
 
 @workflow.command('update_vertex', short_help='None')
 @click.argument('args', nargs=-1, metavar='sys_id=value workflow_id=value task=value alias=value vertex_id=value vertex_x=value vertex_y=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_vertex(uac, args, output=None, input=None, select=None):
+def update_vertex(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.workflows.update_vertex(**vars_dict)
     process_output(output, select, response)
 
 
 @workflow.command('add_vertex', short_help='None')
 @click.argument('args', nargs=-1, metavar='workflowid=value workflowname=value task=value alias=value vertex_id=value vertex_x=value vertex_y=value')
 @click.pass_obj
 @output_option
 @select_option
-def add_vertex(uac, args, output=None, select=None):
+def add_vertex(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.workflows.add_vertex(**vars_dict)
     process_output(output, select, response)
 
 @workflow.command('add_child_vertex', short_help='Adds a vertex and edge')
 @click.argument('args', nargs=-1, metavar='workflow_name=value parent_task_name=name parent_vertex_id=[optional] task_name=new_task vertex_id=[optional] vertexX=None vertexY=None vertex_x_offset=100 vertex_y_offset=100')
 @click.pass_obj
 @output_option
 @select_option
-def add_child_vertex(uac, args, output=None, select=None):
+def add_child_vertex(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.workflows.add_child_vertex(**vars_dict)
     process_output(output, select, response)
 
 
 @workflow.command('delete_vertices', short_help='None')
 @click.argument('args', nargs=-1, metavar='workflowid=value workflowname=value taskid=value taskname=value taskalias=value vertexid=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_vertices(uac, args, output=None, select=None):
+def delete_vertices(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.workflows.delete_vertices(**vars_dict)
     process_output(output, select, response)
 
 
 @workflow.command('get_forecast', short_help='None')
 @click.argument('args', nargs=-1, metavar='workflowid=value workflowname=value calendarid=value calendarname=value triggerid=value triggername=value date=value time=value timezone=value forecast_timezone=value exclude=value variable=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_forecast(uac, args, output=None, select=None):
+def get_forecast(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.workflows.get_forecast(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.1.1/uac_cli/main.py` & `uac-cli-0.2.0/uac_cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,14 @@
-from dotenv import load_dotenv
-import os
-from pathlib import Path
 import sys
 import logging
 import uac_api
 import click
-import yaml
-import uac_api.payload
 from . import __version__
 
-
-from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
-from uac_cli.utils.config import write_config, read_config, ask_profile, read_profile, write_profile
+from uac_cli.utils.config import read_profile
 from uac_cli.commands.agent import agent
 from uac_cli.commands.agent_cluster import agent_cluster
 from uac_cli.commands.audit import audit
 from uac_cli.commands.bundle import bundle, promotion, promotion_target
 from uac_cli.commands.business_service import business_service
 from uac_cli.commands.calendar import calendar
 from uac_cli.commands.cluster_node import cluster_node
@@ -45,17 +38,14 @@
 from uac_cli.commands.virtual_resource import virtual_resource
 from uac_cli.commands.webhook import webhook
 from uac_cli.commands.workflow import workflow
 from uac_cli.commands.config import config
 
 
 
-# Load environment variables from .env file
-load_dotenv()
-
 __output = None
 __select = None
 
 
 class UacCli:
     def __init__(self, profile_name='default', log_level='ERROR'):
         self.log_level = log_level
```

### Comparing `uac-cli-0.1.1/uac_cli/utils/config.py` & `uac-cli-0.2.0/uac_cli/utils/config.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.1.1/uac_cli/utils/process.py` & `uac-cli-0.2.0/uac_cli/utils/process.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.1.1/uac_cli.egg-info/PKG-INFO` & `uac-cli-0.2.0/uac_cli.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: uac-cli
-Version: 0.1.1
+Version: 0.2.0
 Summary: A CLI tool for executing commands against the Stonebranch UAC API
 Author: Stonebranch
-Author-email: huseyim@gmail.com
+Author-email: "Huseyin G." <huseyim@gmail.com>
 License: CC BY-NC 4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
@@ -201,15 +201,21 @@
 ```bash
 uac agent_cluster create --input agent_cluster_config.json --ignore-ids
 ```
 
 #### Running a Report
 
 ```bash
+# download PDF file
 uac report run_report report_title="Active Tasks" --format pdf --output report_output.pdf
+# download the report in different formats
+uac report run_report report_title="Active Tasks" --format json
+uac report run_report report_title="Active Tasks" --format tab
+uac report run_report report_title="Active Tasks" --format csv
+uac report run_report report_title="Active Tasks" --format xml
 ```
 
 ## Development
 
 To contribute to the UAC CLI tool, clone the repository, make your changes, and submit a pull request. Ensure you follow the project's coding standards and update tests as necessary.
 
 ## Support
```

### Comparing `uac-cli-0.1.1/uac_cli.egg-info/SOURCES.txt` & `uac-cli-0.2.0/uac_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

