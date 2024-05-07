# Comparing `tmp/genv-1.4.1.tar.gz` & `tmp/genv-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genv-1.4.1.tar", last modified: Mon Apr 15 12:00:51 2024, max compression
+gzip compressed data, was "genv-1.4.2.tar", last modified: Tue May  7 08:28:21 2024, max compression
```

## Comparing `genv-1.4.1.tar` & `genv-1.4.2.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.506082 genv-1.4.1/
--rw-r--r--   0 raz       (1001) raz       (1001)    34523 2024-04-15 08:51:52.000000 genv-1.4.1/LICENSE
--rw-r--r--   0 raz       (1001) raz       (1001)     7822 2024-04-15 12:00:51.506082 genv-1.4.1/PKG-INFO
--rw-r--r--   0 raz       (1001) raz       (1001)     7094 2024-04-15 12:00:19.000000 genv-1.4.1/README.md
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.499082 genv-1.4.1/genv/
--rw-r--r--   0 raz       (1001) raz       (1001)      318 2024-04-15 12:00:19.000000 genv-1.4.1/genv/__init__.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.500082 genv-1.4.1/genv/_ray/
--rw-r--r--   0 raz       (1001) raz       (1001)       27 2024-04-15 12:00:19.000000 genv-1.4.1/genv/_ray/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1737 2024-04-15 12:00:19.000000 genv-1.4.1/genv/_ray/remote.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.501082 genv-1.4.1/genv/cli/
--rw-r--r--   0 raz       (1001) raz       (1001)        0 2024-04-15 08:53:25.000000 genv-1.4.1/genv/cli/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     5444 2024-04-15 08:53:25.000000 genv-1.4.1/genv/cli/__main__.py
--rwxrw-rw-   0 raz       (1001) raz       (1001)     2755 2024-02-14 12:55:54.000000 genv-1.4.1/genv/cli/activate.py
--rwxrw-rw-   0 raz       (1001) raz       (1001)     1358 2023-06-12 07:39:27.000000 genv-1.4.1/genv/cli/attach.py
--rwxrw-rw-   0 raz       (1001) raz       (1001)     2295 2023-06-12 07:39:27.000000 genv-1.4.1/genv/cli/config.py
--rwxrw-rw-   0 raz       (1001) raz       (1001)      738 2023-06-12 07:39:27.000000 genv-1.4.1/genv/cli/deactivate.py
--rwxrw-rw-   0 raz       (1001) raz       (1001)      465 2023-06-12 07:39:27.000000 genv-1.4.1/genv/cli/detach.py
--rw-r--r--   0 raz       (1001) raz       (1001)    10817 2024-04-15 08:53:25.000000 genv-1.4.1/genv/cli/devices.py
--rw-r--r--   0 raz       (1001) raz       (1001)     3227 2024-04-15 08:53:25.000000 genv-1.4.1/genv/cli/enforce.py
--rwxrw-rw-   0 raz       (1001) raz       (1001)     9382 2023-06-12 07:39:27.000000 genv-1.4.1/genv/cli/envs.py
--rwxrw-rw-   0 raz       (1001) raz       (1001)      656 2023-06-12 07:39:27.000000 genv-1.4.1/genv/cli/home.py
--rwxr-xr-x   0 raz       (1001) raz       (1001)     6072 2024-04-15 11:53:54.000000 genv-1.4.1/genv/cli/llm.py
--rwxrw-rw-   0 raz       (1001) raz       (1001)      610 2023-06-12 07:39:27.000000 genv-1.4.1/genv/cli/lock.py
--rwxrw-rw-   0 raz       (1001) raz       (1001)     2004 2024-02-11 16:13:17.000000 genv-1.4.1/genv/cli/monitor.py
--rwxr-xr-x   0 raz       (1001) raz       (1001)    22328 2024-04-15 12:00:19.000000 genv-1.4.1/genv/cli/remote.py
--rw-r--r--   0 raz       (1001) raz       (1001)     5133 2024-04-15 12:00:19.000000 genv-1.4.1/genv/cli/shell.py
--rw-r--r--   0 raz       (1001) raz       (1001)      892 2024-04-15 08:53:35.000000 genv-1.4.1/genv/cli/status.py
--rwxr-xr-x   0 raz       (1001) raz       (1001)     1986 2024-04-15 12:00:19.000000 genv-1.4.1/genv/cli/usage.py
--rwxrw-rw-   0 raz       (1001) raz       (1001)      307 2024-02-18 12:59:25.000000 genv-1.4.1/genv/cli/version.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.502082 genv-1.4.1/genv/core/
--rw-r--r--   0 raz       (1001) raz       (1001)      143 2024-04-15 08:53:40.000000 genv-1.4.1/genv/core/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     5677 2024-04-15 12:00:19.000000 genv-1.4.1/genv/core/devices.py
--rw-r--r--   0 raz       (1001) raz       (1001)     3703 2024-04-15 08:53:45.000000 genv-1.4.1/genv/core/envs.py
--rw-r--r--   0 raz       (1001) raz       (1001)      894 2024-04-15 12:00:19.000000 genv-1.4.1/genv/core/processes.py
--rw-r--r--   0 raz       (1001) raz       (1001)      379 2024-04-15 08:54:06.000000 genv-1.4.1/genv/core/snapshot.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1425 2024-04-15 08:54:06.000000 genv-1.4.1/genv/core/system.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1424 2024-04-15 08:54:06.000000 genv-1.4.1/genv/core/utils.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.502082 genv-1.4.1/genv/enforce/
--rw-r--r--   0 raz       (1001) raz       (1001)       49 2024-04-15 08:54:06.000000 genv-1.4.1/genv/enforce/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1288 2024-04-15 08:54:06.000000 genv-1.4.1/genv/enforce/execute.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.502082 genv-1.4.1/genv/enforce/rules/
--rw-r--r--   0 raz       (1001) raz       (1001)      176 2024-04-15 08:54:06.000000 genv-1.4.1/genv/enforce/rules/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)      864 2024-04-15 08:54:06.000000 genv-1.4.1/genv/enforce/rules/env_devices.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1394 2024-04-15 08:54:06.000000 genv-1.4.1/genv/enforce/rules/env_memory.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1449 2024-04-15 08:54:06.000000 genv-1.4.1/genv/enforce/rules/max_devices_per_user.py
--rw-r--r--   0 raz       (1001) raz       (1001)      642 2024-04-15 08:54:06.000000 genv-1.4.1/genv/enforce/rules/non_env_processes.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.502082 genv-1.4.1/genv/entities/
--rw-r--r--   0 raz       (1001) raz       (1001)      119 2024-04-15 08:54:06.000000 genv-1.4.1/genv/entities/__init__.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.503082 genv-1.4.1/genv/entities/core/
--rw-r--r--   0 raz       (1001) raz       (1001)      165 2024-04-15 08:54:06.000000 genv-1.4.1/genv/entities/core/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     7231 2024-04-15 08:54:06.000000 genv-1.4.1/genv/entities/core/devices.py
--rw-r--r--   0 raz       (1001) raz       (1001)     6009 2024-04-15 12:00:19.000000 genv-1.4.1/genv/entities/core/envs.py
--rw-r--r--   0 raz       (1001) raz       (1001)     3484 2024-04-15 08:54:16.000000 genv-1.4.1/genv/entities/core/processes.py
--rw-r--r--   0 raz       (1001) raz       (1001)      982 2024-04-15 08:54:16.000000 genv-1.4.1/genv/entities/core/snapshot.py
--rw-r--r--   0 raz       (1001) raz       (1001)      428 2024-04-15 08:54:16.000000 genv-1.4.1/genv/entities/core/system.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.503082 genv-1.4.1/genv/entities/enforce/
--rw-r--r--   0 raz       (1001) raz       (1001)       54 2024-04-15 08:54:16.000000 genv-1.4.1/genv/entities/enforce/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)      270 2024-04-15 08:54:16.000000 genv-1.4.1/genv/entities/enforce/report.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1126 2024-04-15 08:54:16.000000 genv-1.4.1/genv/entities/enforce/survey.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.503082 genv-1.4.1/genv/metrics/
--rw-r--r--   0 raz       (1001) raz       (1001)      184 2024-04-15 08:54:23.000000 genv-1.4.1/genv/metrics/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     4773 2024-04-15 08:54:23.000000 genv-1.4.1/genv/metrics/collection.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.498082 genv-1.4.1/genv/metrics/export/
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.503082 genv-1.4.1/genv/metrics/export/grafana/
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.503082 genv-1.4.1/genv/metrics/export/grafana/dashboards/
--rw-r--r--   0 raz       (1001) raz       (1001)    22349 2024-04-15 08:54:38.000000 genv-1.4.1/genv/metrics/export/grafana/dashboards/overview.json
--rw-r--r--   0 raz       (1001) raz       (1001)      182 2024-04-15 08:59:58.000000 genv-1.4.1/genv/metrics/export/grafana/grafana.ini
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.498082 genv-1.4.1/genv/metrics/export/grafana/provisioning/
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.503082 genv-1.4.1/genv/metrics/export/grafana/provisioning/dashboards/
--rw-r--r--   0 raz       (1001) raz       (1001)      114 2024-04-15 08:54:38.000000 genv-1.4.1/genv/metrics/export/grafana/provisioning/dashboards/default.yml
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.504082 genv-1.4.1/genv/metrics/export/grafana/provisioning/datasources/
--rw-r--r--   0 raz       (1001) raz       (1001)      134 2024-04-15 08:54:38.000000 genv-1.4.1/genv/metrics/export/grafana/provisioning/datasources/default.yml
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.504082 genv-1.4.1/genv/metrics/export/prometheus/
--rw-r--r--   0 raz       (1001) raz       (1001)      155 2024-04-15 08:54:38.000000 genv-1.4.1/genv/metrics/export/prometheus/prometheus.yml
--rw-r--r--   0 raz       (1001) raz       (1001)      966 2024-04-15 08:54:23.000000 genv-1.4.1/genv/metrics/metric.py
--rw-r--r--   0 raz       (1001) raz       (1001)     2663 2024-04-15 12:00:19.000000 genv-1.4.1/genv/metrics/publisher.py
--rw-r--r--   0 raz       (1001) raz       (1001)      846 2024-04-15 08:54:29.000000 genv-1.4.1/genv/metrics/spec.py
--rw-r--r--   0 raz       (1001) raz       (1001)     4277 2024-04-15 08:54:29.000000 genv-1.4.1/genv/metrics/specs.py
--rw-r--r--   0 raz       (1001) raz       (1001)      174 2024-04-15 08:54:29.000000 genv-1.4.1/genv/metrics/type.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.504082 genv-1.4.1/genv/ray/
--rw-r--r--   0 raz       (1001) raz       (1001)       21 2024-04-15 08:54:48.000000 genv-1.4.1/genv/ray/__init__.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.504082 genv-1.4.1/genv/remote/
--rw-r--r--   0 raz       (1001) raz       (1001)       87 2024-04-15 08:54:48.000000 genv-1.4.1/genv/remote/__init__.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.504082 genv-1.4.1/genv/remote/core/
--rw-r--r--   0 raz       (1001) raz       (1001)      123 2024-04-15 08:54:48.000000 genv-1.4.1/genv/remote/core/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)      381 2024-04-15 08:54:48.000000 genv-1.4.1/genv/remote/core/devices.py
--rw-r--r--   0 raz       (1001) raz       (1001)      377 2024-04-15 08:54:48.000000 genv-1.4.1/genv/remote/core/envs.py
--rw-r--r--   0 raz       (1001) raz       (1001)      387 2024-04-15 08:54:48.000000 genv-1.4.1/genv/remote/core/processes.py
--rw-r--r--   0 raz       (1001) raz       (1001)      834 2024-04-15 09:00:02.000000 genv-1.4.1/genv/remote/core/snapshot.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1530 2024-04-15 09:00:05.000000 genv-1.4.1/genv/remote/core/system.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.504082 genv-1.4.1/genv/remote/enforce/
--rw-r--r--   0 raz       (1001) raz       (1001)       29 2024-04-15 08:54:55.000000 genv-1.4.1/genv/remote/enforce/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)      637 2024-04-15 09:00:08.000000 genv-1.4.1/genv/remote/enforce/execute.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.505082 genv-1.4.1/genv/remote/metrics/
--rw-r--r--   0 raz       (1001) raz       (1001)       35 2024-04-15 08:55:02.000000 genv-1.4.1/genv/remote/metrics/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1523 2024-04-15 08:55:02.000000 genv-1.4.1/genv/remote/metrics/collection.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.505082 genv-1.4.1/genv/remote/utils/
--rw-r--r--   0 raz       (1001) raz       (1001)       40 2024-04-15 08:55:02.000000 genv-1.4.1/genv/remote/utils/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     3206 2024-04-15 12:00:19.000000 genv-1.4.1/genv/remote/utils/ssh.py
--rw-r--r--   0 raz       (1001) raz       (1001)      515 2024-04-15 08:55:09.000000 genv-1.4.1/genv/remote/utils/utils.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.505082 genv-1.4.1/genv/sdk/
--rw-r--r--   0 raz       (1001) raz       (1001)      272 2024-04-15 08:55:09.000000 genv-1.4.1/genv/sdk/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     4132 2024-04-15 09:00:29.000000 genv-1.4.1/genv/sdk/devices.py
--rw-r--r--   0 raz       (1001) raz       (1001)     4280 2024-04-15 12:00:19.000000 genv-1.4.1/genv/sdk/env.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1300 2024-04-15 12:00:19.000000 genv-1.4.1/genv/sdk/utils.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.505082 genv-1.4.1/genv/serialization/
--rw-r--r--   0 raz       (1001) raz       (1001)       44 2024-04-15 08:55:20.000000 genv-1.4.1/genv/serialization/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1803 2024-04-15 08:55:20.000000 genv-1.4.1/genv/serialization/json_.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.505082 genv-1.4.1/genv/shims/
--rwxrw-rw-   0 raz       (1001) raz       (1001)     2750 2023-06-10 15:50:03.000000 genv-1.4.1/genv/shims/docker
--rwxrw-rw-   0 raz       (1001) raz       (1001)     7030 2023-05-07 09:36:08.000000 genv-1.4.1/genv/shims/nvidia-smi
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.506082 genv-1.4.1/genv/utils/
--rw-r--r--   0 raz       (1001) raz       (1001)      107 2024-04-15 08:55:20.000000 genv-1.4.1/genv/utils/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1393 2024-04-15 08:55:20.000000 genv-1.4.1/genv/utils/nvidia_smi.py
--rw-r--r--   0 raz       (1001) raz       (1001)     3526 2024-04-15 12:00:19.000000 genv-1.4.1/genv/utils/os_.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1253 2024-04-15 08:55:33.000000 genv-1.4.1/genv/utils/poll.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.506082 genv-1.4.1/genv/utils/runners/
--rw-r--r--   0 raz       (1001) raz       (1001)       93 2024-04-15 08:55:33.000000 genv-1.4.1/genv/utils/runners/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)      483 2024-04-15 08:55:33.000000 genv-1.4.1/genv/utils/runners/local.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1606 2024-04-15 08:55:33.000000 genv-1.4.1/genv/utils/runners/runner.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1543 2024-04-15 08:55:33.000000 genv-1.4.1/genv/utils/runners/ssh.py
--rw-r--r--   0 raz       (1001) raz       (1001)     3446 2024-04-15 08:55:33.000000 genv-1.4.1/genv/utils/utils.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.500082 genv-1.4.1/genv.egg-info/
--rwxrw-rw-   0 raz       (1001) raz       (1001)     7822 2024-04-15 12:00:51.000000 genv-1.4.1/genv.egg-info/PKG-INFO
--rwxrw-rw-   0 raz       (1001) raz       (1001)     2548 2024-04-15 12:00:51.000000 genv-1.4.1/genv.egg-info/SOURCES.txt
--rwxrw-rw-   0 raz       (1001) raz       (1001)        1 2024-04-15 12:00:51.000000 genv-1.4.1/genv.egg-info/dependency_links.txt
--rwxrw-rw-   0 raz       (1001) raz       (1001)       48 2024-04-15 12:00:51.000000 genv-1.4.1/genv.egg-info/entry_points.txt
--rwxrw-rw-   0 raz       (1001) raz       (1001)       94 2024-04-15 12:00:51.000000 genv-1.4.1/genv.egg-info/requires.txt
--rwxrw-rw-   0 raz       (1001) raz       (1001)        5 2024-04-15 12:00:51.000000 genv-1.4.1/genv.egg-info/top_level.txt
--rw-r--r--   0 raz       (1001) raz       (1001)       38 2024-04-15 12:00:51.506082 genv-1.4.1/setup.cfg
--rw-r--r--   0 raz       (1001) raz       (1001)     1225 2024-04-15 11:57:43.000000 genv-1.4.1/setup.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.676278 genv-1.4.2/
+-rw-r--r--   0 raz       (1001) raz       (1001)    34523 2024-04-15 08:51:52.000000 genv-1.4.2/LICENSE
+-rw-r--r--   0 raz       (1001) raz       (1001)     7822 2024-05-07 08:28:21.676278 genv-1.4.2/PKG-INFO
+-rw-r--r--   0 raz       (1001) raz       (1001)     7094 2024-05-07 08:12:32.000000 genv-1.4.2/README.md
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.668278 genv-1.4.2/genv/
+-rw-r--r--   0 raz       (1001) raz       (1001)      318 2024-05-07 08:12:32.000000 genv-1.4.2/genv/__init__.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.669278 genv-1.4.2/genv/_ray/
+-rw-r--r--   0 raz       (1001) raz       (1001)       27 2024-05-07 08:12:32.000000 genv-1.4.2/genv/_ray/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1737 2024-05-07 08:12:32.000000 genv-1.4.2/genv/_ray/remote.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.670278 genv-1.4.2/genv/cli/
+-rw-r--r--   0 raz       (1001) raz       (1001)        0 2024-04-15 08:53:25.000000 genv-1.4.2/genv/cli/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     5444 2024-04-15 08:53:25.000000 genv-1.4.2/genv/cli/__main__.py
+-rwxrw-rw-   0 raz       (1001) raz       (1001)     2755 2024-02-14 12:55:54.000000 genv-1.4.2/genv/cli/activate.py
+-rwxrw-rw-   0 raz       (1001) raz       (1001)     1358 2023-06-12 07:39:27.000000 genv-1.4.2/genv/cli/attach.py
+-rwxrw-rw-   0 raz       (1001) raz       (1001)     2295 2023-06-12 07:39:27.000000 genv-1.4.2/genv/cli/config.py
+-rwxrw-rw-   0 raz       (1001) raz       (1001)      738 2023-06-12 07:39:27.000000 genv-1.4.2/genv/cli/deactivate.py
+-rwxrw-rw-   0 raz       (1001) raz       (1001)      465 2023-06-12 07:39:27.000000 genv-1.4.2/genv/cli/detach.py
+-rw-r--r--   0 raz       (1001) raz       (1001)    10817 2024-04-15 08:53:25.000000 genv-1.4.2/genv/cli/devices.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3227 2024-04-15 08:53:25.000000 genv-1.4.2/genv/cli/enforce.py
+-rwxrw-rw-   0 raz       (1001) raz       (1001)     9382 2023-06-12 07:39:27.000000 genv-1.4.2/genv/cli/envs.py
+-rwxrw-rw-   0 raz       (1001) raz       (1001)      656 2023-06-12 07:39:27.000000 genv-1.4.2/genv/cli/home.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)     6072 2024-04-15 11:53:54.000000 genv-1.4.2/genv/cli/llm.py
+-rwxrw-rw-   0 raz       (1001) raz       (1001)      610 2023-06-12 07:39:27.000000 genv-1.4.2/genv/cli/lock.py
+-rwxrw-rw-   0 raz       (1001) raz       (1001)     2004 2024-02-11 16:13:17.000000 genv-1.4.2/genv/cli/monitor.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)    22780 2024-05-07 08:23:25.000000 genv-1.4.2/genv/cli/remote.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     5133 2024-05-07 08:12:32.000000 genv-1.4.2/genv/cli/shell.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      892 2024-04-15 08:53:35.000000 genv-1.4.2/genv/cli/status.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)     1986 2024-05-07 08:12:32.000000 genv-1.4.2/genv/cli/usage.py
+-rwxrw-rw-   0 raz       (1001) raz       (1001)      307 2024-02-18 12:59:25.000000 genv-1.4.2/genv/cli/version.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.670278 genv-1.4.2/genv/core/
+-rw-r--r--   0 raz       (1001) raz       (1001)      143 2024-04-15 08:53:40.000000 genv-1.4.2/genv/core/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     5677 2024-05-07 08:12:32.000000 genv-1.4.2/genv/core/devices.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3703 2024-04-15 08:53:45.000000 genv-1.4.2/genv/core/envs.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      894 2024-05-07 08:12:32.000000 genv-1.4.2/genv/core/processes.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      379 2024-04-15 08:54:06.000000 genv-1.4.2/genv/core/snapshot.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1425 2024-04-15 08:54:06.000000 genv-1.4.2/genv/core/system.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1424 2024-04-15 08:54:06.000000 genv-1.4.2/genv/core/utils.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.671278 genv-1.4.2/genv/enforce/
+-rw-r--r--   0 raz       (1001) raz       (1001)       49 2024-04-15 08:54:06.000000 genv-1.4.2/genv/enforce/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1288 2024-04-15 08:54:06.000000 genv-1.4.2/genv/enforce/execute.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.671278 genv-1.4.2/genv/enforce/rules/
+-rw-r--r--   0 raz       (1001) raz       (1001)      176 2024-04-15 08:54:06.000000 genv-1.4.2/genv/enforce/rules/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      864 2024-04-15 08:54:06.000000 genv-1.4.2/genv/enforce/rules/env_devices.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1394 2024-04-15 08:54:06.000000 genv-1.4.2/genv/enforce/rules/env_memory.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1449 2024-04-15 08:54:06.000000 genv-1.4.2/genv/enforce/rules/max_devices_per_user.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      642 2024-04-15 08:54:06.000000 genv-1.4.2/genv/enforce/rules/non_env_processes.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.671278 genv-1.4.2/genv/entities/
+-rw-r--r--   0 raz       (1001) raz       (1001)      119 2024-04-15 08:54:06.000000 genv-1.4.2/genv/entities/__init__.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.672278 genv-1.4.2/genv/entities/core/
+-rw-r--r--   0 raz       (1001) raz       (1001)      165 2024-04-15 08:54:06.000000 genv-1.4.2/genv/entities/core/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     7231 2024-04-15 08:54:06.000000 genv-1.4.2/genv/entities/core/devices.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     6009 2024-05-07 08:12:32.000000 genv-1.4.2/genv/entities/core/envs.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3484 2024-04-15 08:54:16.000000 genv-1.4.2/genv/entities/core/processes.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      982 2024-04-15 08:54:16.000000 genv-1.4.2/genv/entities/core/snapshot.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      428 2024-04-15 08:54:16.000000 genv-1.4.2/genv/entities/core/system.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.672278 genv-1.4.2/genv/entities/enforce/
+-rw-r--r--   0 raz       (1001) raz       (1001)       54 2024-04-15 08:54:16.000000 genv-1.4.2/genv/entities/enforce/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      270 2024-04-15 08:54:16.000000 genv-1.4.2/genv/entities/enforce/report.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1126 2024-04-15 08:54:16.000000 genv-1.4.2/genv/entities/enforce/survey.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.673278 genv-1.4.2/genv/metrics/
+-rw-r--r--   0 raz       (1001) raz       (1001)      184 2024-04-15 08:54:23.000000 genv-1.4.2/genv/metrics/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     4773 2024-04-15 08:54:23.000000 genv-1.4.2/genv/metrics/collection.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.667278 genv-1.4.2/genv/metrics/export/
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.673278 genv-1.4.2/genv/metrics/export/grafana/
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.673278 genv-1.4.2/genv/metrics/export/grafana/dashboards/
+-rw-r--r--   0 raz       (1001) raz       (1001)    22349 2024-04-15 08:54:38.000000 genv-1.4.2/genv/metrics/export/grafana/dashboards/overview.json
+-rw-r--r--   0 raz       (1001) raz       (1001)      182 2024-04-15 08:59:58.000000 genv-1.4.2/genv/metrics/export/grafana/grafana.ini
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.667278 genv-1.4.2/genv/metrics/export/grafana/provisioning/
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.673278 genv-1.4.2/genv/metrics/export/grafana/provisioning/dashboards/
+-rw-r--r--   0 raz       (1001) raz       (1001)      114 2024-04-15 08:54:38.000000 genv-1.4.2/genv/metrics/export/grafana/provisioning/dashboards/default.yml
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.673278 genv-1.4.2/genv/metrics/export/grafana/provisioning/datasources/
+-rw-r--r--   0 raz       (1001) raz       (1001)      134 2024-04-15 08:54:38.000000 genv-1.4.2/genv/metrics/export/grafana/provisioning/datasources/default.yml
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.673278 genv-1.4.2/genv/metrics/export/prometheus/
+-rw-r--r--   0 raz       (1001) raz       (1001)      155 2024-04-15 08:54:38.000000 genv-1.4.2/genv/metrics/export/prometheus/prometheus.yml
+-rw-r--r--   0 raz       (1001) raz       (1001)      966 2024-04-15 08:54:23.000000 genv-1.4.2/genv/metrics/metric.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     2663 2024-05-07 08:12:32.000000 genv-1.4.2/genv/metrics/publisher.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      846 2024-04-15 08:54:29.000000 genv-1.4.2/genv/metrics/spec.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     4277 2024-04-15 08:54:29.000000 genv-1.4.2/genv/metrics/specs.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      174 2024-04-15 08:54:29.000000 genv-1.4.2/genv/metrics/type.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.673278 genv-1.4.2/genv/ray/
+-rw-r--r--   0 raz       (1001) raz       (1001)       21 2024-04-15 08:54:48.000000 genv-1.4.2/genv/ray/__init__.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.673278 genv-1.4.2/genv/remote/
+-rw-r--r--   0 raz       (1001) raz       (1001)       87 2024-04-15 08:54:48.000000 genv-1.4.2/genv/remote/__init__.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.674278 genv-1.4.2/genv/remote/core/
+-rw-r--r--   0 raz       (1001) raz       (1001)      123 2024-04-15 08:54:48.000000 genv-1.4.2/genv/remote/core/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      381 2024-04-15 08:54:48.000000 genv-1.4.2/genv/remote/core/devices.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      377 2024-04-15 08:54:48.000000 genv-1.4.2/genv/remote/core/envs.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      387 2024-04-15 08:54:48.000000 genv-1.4.2/genv/remote/core/processes.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      834 2024-04-15 09:00:02.000000 genv-1.4.2/genv/remote/core/snapshot.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1530 2024-04-15 09:00:05.000000 genv-1.4.2/genv/remote/core/system.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.674278 genv-1.4.2/genv/remote/enforce/
+-rw-r--r--   0 raz       (1001) raz       (1001)       29 2024-04-15 08:54:55.000000 genv-1.4.2/genv/remote/enforce/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      637 2024-04-15 09:00:08.000000 genv-1.4.2/genv/remote/enforce/execute.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.675278 genv-1.4.2/genv/remote/metrics/
+-rw-r--r--   0 raz       (1001) raz       (1001)       35 2024-04-15 08:55:02.000000 genv-1.4.2/genv/remote/metrics/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1523 2024-04-15 08:55:02.000000 genv-1.4.2/genv/remote/metrics/collection.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.675278 genv-1.4.2/genv/remote/utils/
+-rw-r--r--   0 raz       (1001) raz       (1001)       40 2024-04-15 08:55:02.000000 genv-1.4.2/genv/remote/utils/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3206 2024-05-07 08:12:32.000000 genv-1.4.2/genv/remote/utils/ssh.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      515 2024-04-15 08:55:09.000000 genv-1.4.2/genv/remote/utils/utils.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.675278 genv-1.4.2/genv/sdk/
+-rw-r--r--   0 raz       (1001) raz       (1001)      272 2024-04-15 08:55:09.000000 genv-1.4.2/genv/sdk/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     4132 2024-04-15 09:00:29.000000 genv-1.4.2/genv/sdk/devices.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     4280 2024-05-07 08:12:32.000000 genv-1.4.2/genv/sdk/env.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1300 2024-05-07 08:12:32.000000 genv-1.4.2/genv/sdk/utils.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.675278 genv-1.4.2/genv/serialization/
+-rw-r--r--   0 raz       (1001) raz       (1001)       44 2024-04-15 08:55:20.000000 genv-1.4.2/genv/serialization/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1803 2024-04-15 08:55:20.000000 genv-1.4.2/genv/serialization/json_.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.675278 genv-1.4.2/genv/shims/
+-rwxrw-rw-   0 raz       (1001) raz       (1001)     2750 2023-06-10 15:50:03.000000 genv-1.4.2/genv/shims/docker
+-rwxrw-rw-   0 raz       (1001) raz       (1001)     7030 2023-05-07 09:36:08.000000 genv-1.4.2/genv/shims/nvidia-smi
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.676278 genv-1.4.2/genv/utils/
+-rw-r--r--   0 raz       (1001) raz       (1001)      107 2024-04-15 08:55:20.000000 genv-1.4.2/genv/utils/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1393 2024-04-15 08:55:20.000000 genv-1.4.2/genv/utils/nvidia_smi.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3526 2024-05-07 08:12:32.000000 genv-1.4.2/genv/utils/os_.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1253 2024-04-15 08:55:33.000000 genv-1.4.2/genv/utils/poll.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.676278 genv-1.4.2/genv/utils/runners/
+-rw-r--r--   0 raz       (1001) raz       (1001)       93 2024-04-15 08:55:33.000000 genv-1.4.2/genv/utils/runners/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      483 2024-04-15 08:55:33.000000 genv-1.4.2/genv/utils/runners/local.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1606 2024-04-15 08:55:33.000000 genv-1.4.2/genv/utils/runners/runner.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1543 2024-04-15 08:55:33.000000 genv-1.4.2/genv/utils/runners/ssh.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3446 2024-04-15 08:55:33.000000 genv-1.4.2/genv/utils/utils.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-05-07 08:28:21.669278 genv-1.4.2/genv.egg-info/
+-rwxrw-rw-   0 raz       (1001) raz       (1001)     7822 2024-05-07 08:28:21.000000 genv-1.4.2/genv.egg-info/PKG-INFO
+-rwxrw-rw-   0 raz       (1001) raz       (1001)     2548 2024-05-07 08:28:21.000000 genv-1.4.2/genv.egg-info/SOURCES.txt
+-rwxrw-rw-   0 raz       (1001) raz       (1001)        1 2024-05-07 08:28:21.000000 genv-1.4.2/genv.egg-info/dependency_links.txt
+-rwxrw-rw-   0 raz       (1001) raz       (1001)       48 2024-05-07 08:28:21.000000 genv-1.4.2/genv.egg-info/entry_points.txt
+-rwxrw-rw-   0 raz       (1001) raz       (1001)       94 2024-05-07 08:28:21.000000 genv-1.4.2/genv.egg-info/requires.txt
+-rwxrw-rw-   0 raz       (1001) raz       (1001)        5 2024-05-07 08:28:21.000000 genv-1.4.2/genv.egg-info/top_level.txt
+-rw-r--r--   0 raz       (1001) raz       (1001)       38 2024-05-07 08:28:21.676278 genv-1.4.2/setup.cfg
+-rw-r--r--   0 raz       (1001) raz       (1001)     1225 2024-05-07 08:25:47.000000 genv-1.4.2/setup.py
```

### Comparing `genv-1.4.1/LICENSE` & `genv-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/PKG-INFO` & `genv-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genv
-Version: 1.4.1
+Version: 1.4.2
 Summary: GPU environment and cluster management
 Home-page: https://github.com/run-ai/genv
 Author: Run.ai
 Author-email: pypi@run.ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: GPU
```

### Comparing `genv-1.4.1/README.md` & `genv-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/_ray/remote.py` & `genv-1.4.2/genv/_ray/remote.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/cli/__main__.py` & `genv-1.4.2/genv/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/cli/activate.py` & `genv-1.4.2/genv/cli/activate.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/cli/attach.py` & `genv-1.4.2/genv/cli/attach.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/cli/config.py` & `genv-1.4.2/genv/cli/config.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/cli/deactivate.py` & `genv-1.4.2/genv/cli/deactivate.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/cli/devices.py` & `genv-1.4.2/genv/cli/devices.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/cli/enforce.py` & `genv-1.4.2/genv/cli/enforce.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/cli/envs.py` & `genv-1.4.2/genv/cli/envs.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/cli/home.py` & `genv-1.4.2/genv/cli/home.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/cli/llm.py` & `genv-1.4.2/genv/cli/llm.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/cli/lock.py` & `genv-1.4.2/genv/cli/lock.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/cli/monitor.py` & `genv-1.4.2/genv/cli/monitor.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/cli/remote.py` & `genv-1.4.2/genv/cli/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 import asyncio
 import dataclasses
 import itertools
 import os
+import re
 import shutil
 import sys
 from typing import Iterable, NoReturn, Optional, Tuple
 
 import genv
 
 QUERIES = {
@@ -237,14 +238,22 @@
 
     if summary:
         print(
             f"\nTotal {sum([len(snapshot) for snapshot in snapshots])} environments on {len(hosts)} hosts"
         )
 
 
+def _find_llm_port(env: genv.Env) -> Optional[int]:
+    """Finds any port an LLM server environment listens on."""
+
+    match = re.match(r"^llm/[^/]+/(\d+)$", env.config.name)
+    if match:
+        return int(match.group(1))
+
+
 async def do_llm(config: genv.remote.Config, args: argparse.Namespace):
     """Runs the "genv llm" logic."""
 
     if args.llm_command == "attach":
         await do_llm_attach(config, args.model)
     elif args.llm_command == "ps":
         await do_llm_ps(config, args.format, args.header, args.summary, args.timestamp)
@@ -261,17 +270,24 @@
 
     :param model: Model name.
     """
 
     hosts, snapshots = await genv.remote.core.envs.snapshot(config)
 
     for host, snapshot in zip(hosts, snapshots):
-        replicas = len(snapshot.filter(name=f"llm/{model}"))
+        for env in snapshot:
+            if not env.config.name:
+                continue
+
+            if not (
+                env.config.name.startswith(f"llm/{model}/")
+                or env.config.name == f"llm/{model}"  # before 1.4.1
+            ):
+                continue
 
-        if replicas > 0:
             # TODO(raz): we currently attach to the first node; we should pick a node in a smarter way.
             _exec_ssh(host, f"genv llm attach {model}")
 
     raise RuntimeError(f"Could not find LLM model '{model}'")
 
 
 async def do_llm_ps(
@@ -305,16 +321,16 @@
     for host, snapshot in zip(hosts, snapshots):
         for env in snapshot:
             if not (env.config.name and env.config.name.startswith("llm/")):
                 continue
 
             total += 1
 
-            model = env.config.name.split("llm/")[1]
-            port = "N/A"
+            model = env.config.name.split("/")[1]
+            port = _find_llm_port(env) or "N/A"
             created = env.creation if timestamp else env.time_since
             eid = env.eid
             user = env.username or ""
 
             if format == "csv":
                 print(f"{host.hostname},{model},{port},{created},{eid}{user}")
             elif format == "tui":
```

### Comparing `genv-1.4.1/genv/cli/shell.py` & `genv-1.4.2/genv/cli/shell.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/cli/status.py` & `genv-1.4.2/genv/cli/status.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/cli/usage.py` & `genv-1.4.2/genv/cli/usage.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/core/devices.py` & `genv-1.4.2/genv/core/devices.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/core/envs.py` & `genv-1.4.2/genv/core/envs.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/core/processes.py` & `genv-1.4.2/genv/core/processes.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/core/system.py` & `genv-1.4.2/genv/core/system.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/core/utils.py` & `genv-1.4.2/genv/core/utils.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/enforce/execute.py` & `genv-1.4.2/genv/enforce/execute.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/enforce/rules/env_devices.py` & `genv-1.4.2/genv/enforce/rules/env_devices.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/enforce/rules/env_memory.py` & `genv-1.4.2/genv/enforce/rules/env_memory.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/enforce/rules/max_devices_per_user.py` & `genv-1.4.2/genv/enforce/rules/max_devices_per_user.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/enforce/rules/non_env_processes.py` & `genv-1.4.2/genv/enforce/rules/non_env_processes.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/entities/core/devices.py` & `genv-1.4.2/genv/entities/core/devices.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/entities/core/envs.py` & `genv-1.4.2/genv/entities/core/envs.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/entities/core/processes.py` & `genv-1.4.2/genv/entities/core/processes.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/entities/core/snapshot.py` & `genv-1.4.2/genv/entities/core/snapshot.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/entities/enforce/survey.py` & `genv-1.4.2/genv/entities/enforce/survey.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/metrics/collection.py` & `genv-1.4.2/genv/metrics/collection.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/metrics/export/grafana/dashboards/overview.json` & `genv-1.4.2/genv/metrics/export/grafana/dashboards/overview.json`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/metrics/metric.py` & `genv-1.4.2/genv/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/metrics/publisher.py` & `genv-1.4.2/genv/metrics/publisher.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/metrics/spec.py` & `genv-1.4.2/genv/metrics/spec.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/metrics/specs.py` & `genv-1.4.2/genv/metrics/specs.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/remote/core/snapshot.py` & `genv-1.4.2/genv/remote/core/snapshot.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/remote/core/system.py` & `genv-1.4.2/genv/remote/core/system.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/remote/enforce/execute.py` & `genv-1.4.2/genv/remote/enforce/execute.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/remote/metrics/collection.py` & `genv-1.4.2/genv/remote/metrics/collection.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/remote/utils/ssh.py` & `genv-1.4.2/genv/remote/utils/ssh.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/remote/utils/utils.py` & `genv-1.4.2/genv/remote/utils/utils.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/sdk/devices.py` & `genv-1.4.2/genv/sdk/devices.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/sdk/env.py` & `genv-1.4.2/genv/sdk/env.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/sdk/utils.py` & `genv-1.4.2/genv/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/serialization/json_.py` & `genv-1.4.2/genv/serialization/json_.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/shims/docker` & `genv-1.4.2/genv/shims/docker`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/shims/nvidia-smi` & `genv-1.4.2/genv/shims/nvidia-smi`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/utils/nvidia_smi.py` & `genv-1.4.2/genv/utils/nvidia_smi.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/utils/os_.py` & `genv-1.4.2/genv/utils/os_.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/utils/poll.py` & `genv-1.4.2/genv/utils/poll.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/utils/runners/runner.py` & `genv-1.4.2/genv/utils/runners/runner.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/utils/runners/ssh.py` & `genv-1.4.2/genv/utils/runners/ssh.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv/utils/utils.py` & `genv-1.4.2/genv/utils/utils.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/genv.egg-info/PKG-INFO` & `genv-1.4.2/genv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genv
-Version: 1.4.1
+Version: 1.4.2
 Summary: GPU environment and cluster management
 Home-page: https://github.com/run-ai/genv
 Author: Run.ai
 Author-email: pypi@run.ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: GPU
```

### Comparing `genv-1.4.1/genv.egg-info/SOURCES.txt` & `genv-1.4.2/genv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `genv-1.4.1/setup.py` & `genv-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="genv",
-    version="1.4.1",
+    version="1.4.2",
     author="Run.ai",
     author_email="pypi@run.ai",
     description="GPU environment and cluster management",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/run-ai/genv",
     packages=setuptools.find_packages(),
```

