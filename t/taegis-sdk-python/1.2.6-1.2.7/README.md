# Comparing `tmp/taegis_sdk_python-1.2.6.tar.gz` & `tmp/taegis_sdk_python-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taegis_sdk_python-1.2.6.tar", last modified: Thu Apr 25 22:08:51 2024, max compression
+gzip compressed data, was "taegis_sdk_python-1.2.7.tar", last modified: Tue May  7 12:47:36 2024, max compression
```

## Comparing `taegis_sdk_python-1.2.6.tar` & `taegis_sdk_python-1.2.7.tar`

### file list

```diff
@@ -1,274 +1,274 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.603420 taegis_sdk_python-1.2.6/
--rw-rw-rw-   0 root         (0) root         (0)    10173 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       84 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2871 2024-04-25 22:08:51.603420 taegis_sdk_python-1.2.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2119 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)      151 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 22:08:51.603420 taegis_sdk_python-1.2.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1571 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.575420 taegis_sdk_python-1.2.6/taegis_sdk_python/
--rw-rw-rw-   0 root         (0) root         (0)      895 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1135 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/_consts.py
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-04-25 22:08:51.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     9120 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     1740 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2636 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/errors.py
--rw-rw-rw-   0 root         (0) root         (0)    15383 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/service_core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.575420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/
--rw-rw-rw-   0 root         (0) root         (0)    18716 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.575420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/access_points/
--rw-rw-rw-   0 root         (0) root         (0)      976 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/access_points/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2419 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/access_points/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2313 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/access_points/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      893 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/access_points/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1377 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/access_points/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.575420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/agent/
--rw-rw-rw-   0 root         (0) root         (0)     1154 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/agent/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3167 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/agent/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/agent/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     5316 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/agent/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.575420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/alerts/
--rw-rw-rw-   0 root         (0) root         (0)      892 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/alerts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4785 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/alerts/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6011 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/alerts/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     1724 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/alerts/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    80085 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/alerts/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.579420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets/
--rw-rw-rw-   0 root         (0) root         (0)      893 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7235 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    16354 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    23548 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.579420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets2/
--rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9308 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets2/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    16070 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets2/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets2/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    44413 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets2/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.579420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/audits/
--rw-rw-rw-   0 root         (0) root         (0)      893 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/audits/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1361 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/audits/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3909 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/audits/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/audits/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    12825 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/audits/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.579420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/authz/
--rw-rw-rw-   0 root         (0) root         (0)      881 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/authz/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3484 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/authz/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    14226 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/authz/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/authz/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    13254 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/authz/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.579420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/byoti/
--rw-rw-rw-   0 root         (0) root         (0)      881 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/byoti/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2761 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/byoti/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3010 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/byoti/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/byoti/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    10026 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/byoti/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.583420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/clients/
--rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/clients/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4001 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/clients/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2562 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/clients/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/clients/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7361 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/clients/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.583420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/collector/
--rw-rw-rw-   0 root         (0) root         (0)      929 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/collector/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17250 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/collector/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    27472 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/collector/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/collector/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    43430 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/collector/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.583420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/comments/
--rw-rw-rw-   0 root         (0) root         (0)      917 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/comments/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4946 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/comments/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7300 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/comments/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/comments/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     5118 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/comments/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.583420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/contracted_endpoint/
--rw-rw-rw-   0 root         (0) root         (0)     1059 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/contracted_endpoint/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      923 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/contracted_endpoint/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2717 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/contracted_endpoint/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      935 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/contracted_endpoint/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1866 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/contracted_endpoint/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.583420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/datasources/
--rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/datasources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1794 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/datasources/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1807 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/datasources/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/datasources/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2862 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/datasources/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.583420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/detector_registry/
--rw-rw-rw-   0 root         (0) root         (0)     1034 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/detector_registry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      909 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/detector_registry/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3194 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/detector_registry/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/detector_registry/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3164 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/detector_registry/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.583420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_command_manager/
--rw-rw-rw-   0 root         (0) root         (0)     1381 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_command_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7325 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_command_manager/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3523 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_command_manager/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      983 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8618 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_command_manager/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.587420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_management_service/
--rw-rw-rw-   0 root         (0) root         (0)     1417 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_management_service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6935 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_management_service/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7179 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_management_service/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_management_service/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    21447 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_management_service/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.587420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/event_search/
--rw-rw-rw-   0 root         (0) root         (0)      965 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/event_search/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      874 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/event_search/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2805 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/event_search/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/event_search/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3609 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/event_search/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.587420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/events/
--rw-rw-rw-   0 root         (0) root         (0)     1215 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1346 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/events/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2775 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/events/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     2508 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/events/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    11022 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/events/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.587420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/exports/
--rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/exports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14201 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/exports/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    10873 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/exports/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/exports/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    25813 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/exports/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.587420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/fast_ioc/
--rw-rw-rw-   0 root         (0) root         (0)     1201 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/fast_ioc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      846 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/fast_ioc/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3177 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/fast_ioc/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      858 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/fast_ioc/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3467 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/fast_ioc/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.587420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/file_info/
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/file_info/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4508 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/file_info/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3510 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/file_info/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      865 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/file_info/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    39710 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/file_info/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.591420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/ingest_stats/
--rw-rw-rw-   0 root         (0) root         (0)      966 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/ingest_stats/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      874 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/ingest_stats/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     4123 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/ingest_stats/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/ingest_stats/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3947 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/ingest_stats/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.591420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations/
--rw-rw-rw-   0 root         (0) root         (0)     1007 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26132 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    32299 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      904 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    37546 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.591420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations2/
--rw-rw-rw-   0 root         (0) root         (0)     1019 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15493 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations2/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     8585 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations2/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      911 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations2/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    59951 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations2/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.591420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/mitre_attack_info/
--rw-rw-rw-   0 root         (0) root         (0)     1025 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/mitre_attack_info/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/mitre_attack_info/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     9291 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/mitre_attack_info/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/mitre_attack_info/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3202 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/mitre_attack_info/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.591420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_context/
--rw-rw-rw-   0 root         (0) root         (0)     1061 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_context/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4584 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_context/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     4704 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_context/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      955 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_context/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     6279 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_context/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.595420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_ioc/
--rw-rw-rw-   0 root         (0) root         (0)     1313 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_ioc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      898 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_ioc/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3229 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_ioc/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      910 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_ioc/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3901 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_ioc/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.595420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/notebooks/
--rw-rw-rw-   0 root         (0) root         (0)      928 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/notebooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2253 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/notebooks/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1286 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/notebooks/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/notebooks/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/notebooks/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.595420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/notifications/
--rw-rw-rw-   0 root         (0) root         (0)      986 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/notifications/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6906 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/notifications/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2462 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/notifications/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      897 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/notifications/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8811 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/notifications/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.595420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/preferences/
--rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/preferences/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7272 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/preferences/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7360 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/preferences/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/preferences/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    17016 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/preferences/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.595420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/queries/
--rw-rw-rw-   0 root         (0) root         (0)      915 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/queries/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3852 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/queries/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     4382 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/queries/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/queries/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    10778 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/queries/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.595420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/roadrunner/
--rw-rw-rw-   0 root         (0) root         (0)      941 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/roadrunner/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6287 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/roadrunner/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6420 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/roadrunner/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/roadrunner/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    14157 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/roadrunner/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.599420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/rules/
--rw-rw-rw-   0 root         (0) root         (0)      881 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/rules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14238 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/rules/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    17159 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/rules/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/rules/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    25560 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/rules/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.599420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/sharelinks/
--rw-rw-rw-   0 root         (0) root         (0)      941 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/sharelinks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1426 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/sharelinks/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1381 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/sharelinks/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/sharelinks/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2578 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/sharelinks/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.599420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/subjects/
--rw-rw-rw-   0 root         (0) root         (0)      917 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/subjects/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      850 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/subjects/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1451 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/subjects/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/subjects/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3651 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/subjects/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.599420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenant_profiles/
--rw-rw-rw-   0 root         (0) root         (0)     1010 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenant_profiles/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19209 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenant_profiles/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    11166 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenant_profiles/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      907 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenant_profiles/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    23270 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenant_profiles/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.599420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenants/
--rw-rw-rw-   0 root         (0) root         (0)     1349 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenants/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17846 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenants/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7989 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenants/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenants/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    46328 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenants/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.599420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat/
--rw-rw-rw-   0 root         (0) root         (0)      894 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1906 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    12121 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    46398 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.603420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat_score/
--rw-rw-rw-   0 root         (0) root         (0)      966 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat_score/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      874 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat_score/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2208 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat_score/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat_score/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4092 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat_score/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.603420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/trip/
--rw-rw-rw-   0 root         (0) root         (0)      869 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/trip/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4135 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/trip/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3447 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/trip/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      834 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/trip/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     6813 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/trip/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.603420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/users/
--rw-rw-rw-   0 root         (0) root         (0)      881 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/users/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12152 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/users/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7321 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/users/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/users/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    26696 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/users/types.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/tokens.py
--rw-rw-rw-   0 root         (0) root         (0)     7548 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.603420 taegis_sdk_python-1.2.6/taegis_sdk_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2871 2024-04-25 22:08:51.000000 taegis_sdk_python-1.2.6/taegis_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11058 2024-04-25 22:08:51.000000 taegis_sdk_python-1.2.6/taegis_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 22:08:51.000000 taegis_sdk_python-1.2.6/taegis_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      152 2024-04-25 22:08:51.000000 taegis_sdk_python-1.2.6/taegis_sdk_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-25 22:08:51.000000 taegis_sdk_python-1.2.6/taegis_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.115649 taegis_sdk_python-1.2.7/
+-rw-rw-rw-   0 root         (0) root         (0)    10173 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       84 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2871 2024-05-07 12:47:36.115649 taegis_sdk_python-1.2.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2119 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      151 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 12:47:36.115649 taegis_sdk_python-1.2.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.083649 taegis_sdk_python-1.2.7/taegis_sdk_python/
+-rw-rw-rw-   0 root         (0) root         (0)      895 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/_consts.py
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-05-07 12:47:35.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     9120 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     1740 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2636 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    15383 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/service_core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.083649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/
+-rw-rw-rw-   0 root         (0) root         (0)    18790 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.083649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/access_points/
+-rw-rw-rw-   0 root         (0) root         (0)      976 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/access_points/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2419 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/access_points/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/access_points/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      893 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/access_points/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1377 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/access_points/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.087648 taegis_sdk_python-1.2.7/taegis_sdk_python/services/agent/
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/agent/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/agent/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3167 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/agent/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/agent/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5316 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/agent/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.087648 taegis_sdk_python-1.2.7/taegis_sdk_python/services/alerts/
+-rw-rw-rw-   0 root         (0) root         (0)      892 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/alerts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4785 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/alerts/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6011 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/alerts/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1724 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/alerts/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    80085 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/alerts/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.087648 taegis_sdk_python-1.2.7/taegis_sdk_python/services/assets/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/assets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7235 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/assets/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    16354 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/assets/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/assets/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    23548 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/assets/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.087648 taegis_sdk_python-1.2.7/taegis_sdk_python/services/assets2/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/assets2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9308 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/assets2/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    16070 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/assets2/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/assets2/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    44413 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/assets2/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.087648 taegis_sdk_python-1.2.7/taegis_sdk_python/services/audits/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/audits/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1361 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/audits/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3909 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/audits/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/audits/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    12825 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/audits/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.091649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/authz/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/authz/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3484 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/authz/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    14226 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/authz/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/authz/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    13254 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/authz/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.091649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/byoti/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/byoti/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2761 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/byoti/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3010 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/byoti/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/byoti/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10026 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/byoti/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.091649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/clients/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/clients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4001 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/clients/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2562 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/clients/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/clients/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7361 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/clients/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.091649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/collector/
+-rw-rw-rw-   0 root         (0) root         (0)      929 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/collector/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17250 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/collector/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    27472 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/collector/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/collector/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    43430 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/collector/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.091649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/comments/
+-rw-rw-rw-   0 root         (0) root         (0)      917 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/comments/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4946 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/comments/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7300 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/comments/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/comments/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5118 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/comments/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.095649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/contracted_endpoint/
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/contracted_endpoint/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      923 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/contracted_endpoint/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2717 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/contracted_endpoint/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      935 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/contracted_endpoint/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1866 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/contracted_endpoint/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.095649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/datasources/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/datasources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1794 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/datasources/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1807 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/datasources/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/datasources/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2862 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/datasources/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.095649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/detector_registry/
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/detector_registry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      909 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/detector_registry/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3194 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/detector_registry/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/detector_registry/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3164 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/detector_registry/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.095649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/endpoint_command_manager/
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/endpoint_command_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7325 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/endpoint_command_manager/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3523 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/endpoint_command_manager/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      983 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8618 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/endpoint_command_manager/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.095649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/endpoint_management_service/
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/endpoint_management_service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6935 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/endpoint_management_service/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7179 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/endpoint_management_service/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/endpoint_management_service/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    21447 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/endpoint_management_service/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.095649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/event_search/
+-rw-rw-rw-   0 root         (0) root         (0)      965 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/event_search/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      874 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/event_search/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2805 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/event_search/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/event_search/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3609 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/event_search/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.099649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/events/
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1346 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/events/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2775 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/events/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/events/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    11022 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/events/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.099649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/exports/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/exports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14201 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/exports/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    10873 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/exports/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/exports/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    25813 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/exports/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.099649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/fast_ioc/
+-rw-rw-rw-   0 root         (0) root         (0)     1201 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/fast_ioc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      846 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/fast_ioc/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3177 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/fast_ioc/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      858 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/fast_ioc/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3467 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/fast_ioc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.099649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/file_info/
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/file_info/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4508 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/file_info/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3510 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/file_info/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      865 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/file_info/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    39710 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/file_info/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.099649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/ingest_stats/
+-rw-rw-rw-   0 root         (0) root         (0)      966 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/ingest_stats/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      874 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/ingest_stats/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     4123 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/ingest_stats/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/ingest_stats/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3947 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/ingest_stats/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.103649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/investigations/
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/investigations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26132 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/investigations/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    32299 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/investigations/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      904 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/investigations/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    37546 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/investigations/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.103649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/investigations2/
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/investigations2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20039 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/investigations2/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     9469 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/investigations2/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      911 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/investigations2/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    63078 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/investigations2/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.103649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/mitre_attack_info/
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/mitre_attack_info/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/mitre_attack_info/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     9291 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/mitre_attack_info/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/mitre_attack_info/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3202 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/mitre_attack_info/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.103649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/multi_tenant_context/
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/multi_tenant_context/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4584 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/multi_tenant_context/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     4704 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/multi_tenant_context/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      955 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/multi_tenant_context/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6279 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/multi_tenant_context/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.103649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/multi_tenant_ioc/
+-rw-rw-rw-   0 root         (0) root         (0)     1313 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/multi_tenant_ioc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      898 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/multi_tenant_ioc/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3229 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/multi_tenant_ioc/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      910 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/multi_tenant_ioc/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3901 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/multi_tenant_ioc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.103649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/notebooks/
+-rw-rw-rw-   0 root         (0) root         (0)      928 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/notebooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2253 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/notebooks/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/notebooks/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/notebooks/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/notebooks/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.107649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/notifications/
+-rw-rw-rw-   0 root         (0) root         (0)      986 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/notifications/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6906 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/notifications/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2462 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/notifications/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      897 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/notifications/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8811 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/notifications/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.107649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/preferences/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/preferences/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7272 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/preferences/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7360 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/preferences/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/preferences/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    17016 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/preferences/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.107649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/queries/
+-rw-rw-rw-   0 root         (0) root         (0)      915 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/queries/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3852 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/queries/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     4382 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/queries/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/queries/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10778 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/queries/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.107649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/roadrunner/
+-rw-rw-rw-   0 root         (0) root         (0)      941 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/roadrunner/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6287 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/roadrunner/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6420 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/roadrunner/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/roadrunner/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    14157 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/roadrunner/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.107649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/rules/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/rules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14238 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/rules/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    17159 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/rules/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/rules/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    25560 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/rules/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.111649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/sharelinks/
+-rw-rw-rw-   0 root         (0) root         (0)      941 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/sharelinks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1426 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/sharelinks/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/sharelinks/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/sharelinks/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2578 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/sharelinks/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.111649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/subjects/
+-rw-rw-rw-   0 root         (0) root         (0)      917 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/subjects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      850 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/subjects/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1451 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/subjects/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/subjects/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3651 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/subjects/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.111649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/tenant_profiles/
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/tenant_profiles/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19209 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/tenant_profiles/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    11166 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/tenant_profiles/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      907 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/tenant_profiles/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    23270 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/tenant_profiles/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.111649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/tenants/
+-rw-rw-rw-   0 root         (0) root         (0)     1349 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/tenants/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17846 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/tenants/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7989 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/tenants/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/tenants/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    46524 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/tenants/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.111649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/threat/
+-rw-rw-rw-   0 root         (0) root         (0)      894 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/threat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1906 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/threat/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    12121 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/threat/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/threat/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    46398 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/threat/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.115649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/threat_score/
+-rw-rw-rw-   0 root         (0) root         (0)      966 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/threat_score/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      874 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/threat_score/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2208 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/threat_score/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/threat_score/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4092 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/threat_score/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.115649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/trip/
+-rw-rw-rw-   0 root         (0) root         (0)      869 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/trip/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4135 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/trip/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3447 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/trip/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      834 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/trip/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6813 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/trip/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.115649 taegis_sdk_python-1.2.7/taegis_sdk_python/services/users/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/users/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12152 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/users/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7321 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/users/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/users/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    26696 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/services/users/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/tokens.py
+-rw-rw-rw-   0 root         (0) root         (0)     7548 2024-05-07 12:47:24.000000 taegis_sdk_python-1.2.7/taegis_sdk_python/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:47:36.115649 taegis_sdk_python-1.2.7/taegis_sdk_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2871 2024-05-07 12:47:35.000000 taegis_sdk_python-1.2.7/taegis_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11058 2024-05-07 12:47:35.000000 taegis_sdk_python-1.2.7/taegis_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 12:47:35.000000 taegis_sdk_python-1.2.7/taegis_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      152 2024-05-07 12:47:35.000000 taegis_sdk_python-1.2.7/taegis_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-07 12:47:35.000000 taegis_sdk_python-1.2.7/taegis_sdk_python.egg-info/top_level.txt
```

### Comparing `taegis_sdk_python-1.2.6/LICENSE` & `taegis_sdk_python-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/PKG-INFO` & `taegis_sdk_python-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taegis-sdk-python
-Version: 1.2.6
+Version: 1.2.7
 Summary: Taegis Python SDK
 Home-page: https://github.com/secureworks/taegis-sdk-python
 Author: Secureworks
 Author-email: sdks@secureworks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `taegis_sdk_python-1.2.6/README.md` & `taegis_sdk_python-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/setup.py` & `taegis_sdk_python-1.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/_consts.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/_consts.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/authentication.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/authentication.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/config.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/config.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/errors.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/errors.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/service_core.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/service_core.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,19 +162,20 @@
         self._context_kwargs[threading.get_ident()].append(kwargs)
         return self
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        if self._context_kwargs[threading.get_ident()]:
-            self._context_kwargs[threading.get_ident()].pop()
+        if threading.get_ident() in self._context_kwargs:
+            if self._context_kwargs[threading.get_ident()]:
+                self._context_kwargs[threading.get_ident()].pop()
 
-        else:
-            del self._context_kwargs[threading.get_ident()]
+            else:
+                del self._context_kwargs[threading.get_ident()]
 
     @property
     def _context_manager(self):
         """Internal Context Manager property."""
         temp_context = {}
 
         for kwarg in self._context_kwargs.get(self._thread_id, []):
```

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/access_points/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/access_points/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/access_points/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/access_points/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/access_points/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/access_points/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/access_points/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/access_points/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/access_points/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/access_points/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/agent/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/agent/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/agent/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/agent/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/agent/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/agent/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/agent/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/agent/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/agent/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/alerts/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/alerts/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/alerts/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/alerts/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/alerts/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/alerts/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/alerts/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/alerts/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/alerts/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/alerts/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/assets/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/assets/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/assets/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/assets/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets2/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/assets2/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets2/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/assets2/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets2/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/assets2/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets2/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/assets2/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets2/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/assets2/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/audits/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/audits/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/audits/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/audits/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/audits/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/audits/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/audits/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/audits/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/audits/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/audits/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/authz/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/authz/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/authz/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/authz/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/authz/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/authz/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/authz/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/authz/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/authz/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/authz/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/byoti/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/byoti/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/byoti/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/byoti/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/byoti/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/byoti/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/byoti/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/byoti/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/byoti/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/byoti/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/clients/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/clients/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/clients/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/clients/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/clients/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/clients/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/clients/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/clients/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/clients/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/collector/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/collector/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/collector/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/collector/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/collector/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/collector/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/collector/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/collector/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/collector/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/collector/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/comments/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/comments/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/comments/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/comments/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/comments/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/comments/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/comments/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/comments/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/comments/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/comments/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/contracted_endpoint/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/contracted_endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/contracted_endpoint/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/contracted_endpoint/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/contracted_endpoint/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/contracted_endpoint/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/contracted_endpoint/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/contracted_endpoint/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/contracted_endpoint/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/contracted_endpoint/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/datasources/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/datasources/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/datasources/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/datasources/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/datasources/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/datasources/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/datasources/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/datasources/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/datasources/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/datasources/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/detector_registry/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/detector_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/detector_registry/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/detector_registry/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/detector_registry/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/detector_registry/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/detector_registry/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/detector_registry/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/detector_registry/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/detector_registry/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_command_manager/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/endpoint_command_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_command_manager/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/endpoint_command_manager/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_command_manager/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/endpoint_command_manager/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_command_manager/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/endpoint_command_manager/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_management_service/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/endpoint_management_service/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_management_service/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/endpoint_management_service/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_management_service/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/endpoint_management_service/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_management_service/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/endpoint_management_service/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_management_service/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/endpoint_management_service/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/event_search/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/event_search/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/event_search/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/event_search/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/event_search/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/event_search/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/event_search/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/event_search/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/event_search/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/event_search/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/events/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/events/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/events/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/events/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/events/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/events/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/events/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/events/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/events/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/events/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/exports/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/exports/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/exports/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/exports/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/exports/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/exports/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/exports/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/exports/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/exports/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/exports/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/fast_ioc/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/fast_ioc/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/fast_ioc/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/fast_ioc/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/fast_ioc/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/fast_ioc/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/fast_ioc/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/fast_ioc/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/fast_ioc/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/fast_ioc/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/file_info/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/file_info/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/file_info/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/file_info/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/file_info/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/file_info/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/file_info/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/file_info/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/file_info/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/file_info/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/ingest_stats/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/ingest_stats/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/ingest_stats/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/ingest_stats/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/ingest_stats/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/ingest_stats/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/ingest_stats/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/ingest_stats/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/ingest_stats/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/ingest_stats/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/investigations/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/investigations/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/investigations/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/investigations/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/investigations/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations2/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/investigations2/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations2/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/investigations2/queries.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 class TaegisSDKInvestigations2Query:
     """Taegis Investigations2 Query operations."""
 
     def __init__(self, service: Investigations2Service):
         self.service = service
 
     def investigation_v2(self, arguments: InvestigationV2Arguments) -> InvestigationV2:
-        """Get an Investigation."""
+        """investigationV2 gets a single Investigation.."""
         endpoint = "investigationV2"
 
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "arguments": prepare_input(arguments),
             },
@@ -44,15 +44,15 @@
         if result.get(endpoint) is not None:
             return InvestigationV2.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query investigationV2")
 
     def investigations_v2(
         self, arguments: InvestigationsV2Arguments
     ) -> InvestigationsV2:
-        """Search investigations."""
+        """investigationsV2 returns a list of investigations matching the provided arguments.."""
         endpoint = "investigationsV2"
 
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "arguments": prepare_input(arguments),
             },
@@ -61,15 +61,15 @@
         if result.get(endpoint) is not None:
             return InvestigationsV2.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query investigationsV2")
 
     def investigation_rule(
         self, arguments: InvestigationRuleArguments
     ) -> InvestigationRule:
-        """Get an auto-investigation rule."""
+        """investigationRule gets an auto-investigation rule."""
         endpoint = "investigationRule"
 
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "arguments": prepare_input(arguments),
             },
@@ -78,15 +78,15 @@
         if result.get(endpoint) is not None:
             return InvestigationRule.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query investigationRule")
 
     def investigation_rules(
         self, arguments: InvestigationRulesArguments
     ) -> InvestigationRules:
-        """Get auto-investigation rules."""
+        """investigationRules returns a list of investigation rules matching the provided arguments.."""
         endpoint = "investigationRules"
 
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "arguments": prepare_input(arguments),
             },
@@ -95,15 +95,15 @@
         if result.get(endpoint) is not None:
             return InvestigationRules.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query investigationRules")
 
     def investigation_template(
         self, arguments: InvestigationTemplateArguments
     ) -> InvestigationTemplate:
-        """Get an auto-investigation template."""
+        """investigationTemplate gets an auto-investigation template."""
         endpoint = "investigationTemplate"
 
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "arguments": prepare_input(arguments),
             },
@@ -112,15 +112,15 @@
         if result.get(endpoint) is not None:
             return InvestigationTemplate.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query investigationTemplate")
 
     def investigation_templates(
         self, arguments: InvestigationTemplatesArguments
     ) -> InvestigationTemplates:
-        """Get auto-investigation templates."""
+        """investigationTemplates returns a list of investigation templates matching the provided arguments.."""
         endpoint = "investigationTemplates"
 
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "arguments": prepare_input(arguments),
             },
@@ -129,15 +129,17 @@
         if result.get(endpoint) is not None:
             return InvestigationTemplates.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query investigationTemplates")
 
     def export_investigation_resources(
         self, arguments: ExportInvestigationResourcesArguments
     ) -> InvestigationResourceExport:
-        """Get the yaml string for auto-investigation resources (rules & templates)."""
+        """exportInvestigationResources returns a YAML string representation for auto-investigation resources (rules & templates).
+        The returned string can be saved into a file and imported back into the system using importInvestigationResources..
+        """
         endpoint = "exportInvestigationResources"
 
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "arguments": prepare_input(arguments),
             },
@@ -146,45 +148,45 @@
         if result.get(endpoint) is not None:
             return InvestigationResourceExport.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query exportInvestigationResources")
 
     def investigation_v2_timeline(
         self, arguments: InvestigationV2TimelineArguments
     ) -> InvestigationV2Timeline:
-        """Get the investigation timeline."""
+        """investigationV2Timeline returns an investigation timeline detailing the order of alerts, events and other actions taken in relation to an investigation.."""
         endpoint = "investigationV2Timeline"
 
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "arguments": prepare_input(arguments),
             },
             output=build_output_string(InvestigationV2Timeline),
         )
         if result.get(endpoint) is not None:
             return InvestigationV2Timeline.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query investigationV2Timeline")
 
     def comments_v2(self, arguments: CommentsV2Arguments) -> CommentsV2:
-        """Get all investigation comments."""
+        """commentsV2 returns all the comments for an investigation."""
         endpoint = "commentsV2"
 
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "arguments": prepare_input(arguments),
             },
             output=build_output_string(CommentsV2),
         )
         if result.get(endpoint) is not None:
             return CommentsV2.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query commentsV2")
 
     def investigation_v2_types(self) -> List[InvestigationV2Type]:
-        """Get investigation types list based on user."""
+        """investigationV2Types returns the available investigation types for a given user and the current tenant's service level."""
         endpoint = "investigationV2Types"
 
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={},
             output=build_output_string(InvestigationV2Type),
         )
@@ -193,15 +195,16 @@
                 [r or {} for r in result.get(endpoint)], many=True
             )
         raise GraphQLNoRowsInResultSetError("for query investigationV2Types")
 
     def investigation_file_v2(
         self, arguments: InvestigationFileV2Arguments
     ) -> InvestigationFileV2:
-        """Get investigation file meta details - includes presigned download url."""
+        """investigationFileV2 returns file details for a single file attached to an investigation based on the arguments provided.
+        The result will also include a pre-signed download url.."""
         endpoint = "investigationFileV2"
 
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "arguments": prepare_input(arguments),
             },
@@ -210,15 +213,17 @@
         if result.get(endpoint) is not None:
             return InvestigationFileV2.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query investigationFileV2")
 
     def investigation_files_v2(
         self, arguments: InvestigationFilesV2Arguments
     ) -> InvestigationFilesV2:
-        """Get investigation files meta details - does not include presigned download urls."""
+        """investigationFilesV2 returns file details for all files matching the arguments provided.
+        The results will not include pre-signed download urls for each file metadata returned..
+        """
         endpoint = "investigationFilesV2"
 
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "arguments": prepare_input(arguments),
             },
```

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations2/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/investigations2/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations2/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/investigations2/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -439,17 +439,17 @@
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class InvestigationTemplatesArguments:
     """InvestigationTemplatesArguments."""
 
+    cql: Optional[str] = field(default=None, metadata=config(field_name="cql"))
     page: Optional[int] = field(default=None, metadata=config(field_name="page"))
     per_page: Optional[int] = field(default=None, metadata=config(field_name="perPage"))
-    cql: Optional[str] = field(default=None, metadata=config(field_name="cql"))
     name: Optional[str] = field(
         default=None,
         metadata=config(
             metadata={"deprecated": True, "deprecation_reason": "no-op; use cql"},
             field_name="name",
         ),
     )
@@ -472,17 +472,17 @@
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class InvestigationRulesArguments:
     """InvestigationRulesArguments."""
 
+    cql: Optional[str] = field(default=None, metadata=config(field_name="cql"))
     page: Optional[int] = field(default=None, metadata=config(field_name="page"))
     per_page: Optional[int] = field(default=None, metadata=config(field_name="perPage"))
-    cql: Optional[str] = field(default=None, metadata=config(field_name="cql"))
     name: Optional[str] = field(
         default=None,
         metadata=config(
             metadata={"deprecated": True, "deprecation_reason": "no-op; use cql"},
             field_name="name",
         ),
     )
@@ -520,18 +520,18 @@
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class AddCommentToInvestigationInput:
     """AddCommentToInvestigationInput."""
 
-    comment: Optional[str] = field(default=None, metadata=config(field_name="comment"))
     investigation_id: Optional[str] = field(
         default=None, metadata=config(field_name="investigationId")
     )
+    comment: Optional[str] = field(default=None, metadata=config(field_name="comment"))
     is_internal: Optional[bool] = field(
         default=None, metadata=config(field_name="isInternal")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
@@ -682,38 +682,14 @@
     is_genesis: Optional[bool] = field(
         default=None, metadata=config(field_name="isGenesis")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
-class TDRUser:
-    """TDRUser."""
-
-    id: Optional[str] = field(default=None, metadata=config(field_name="id"))
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
-class TenantV4:
-    """TenantV4."""
-
-    id: Optional[str] = field(default=None, metadata=config(field_name="id"))
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
-class Subject:
-    """Subject."""
-
-    id: Optional[str] = field(default=None, metadata=config(field_name="id"))
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
 class InvestigationFileMeta:
     """InvestigationFileMeta."""
 
     content_type: Optional[str] = field(
         default=None, metadata=config(field_name="contentType")
     )
     content_md5: Optional[str] = field(
@@ -745,17 +721,17 @@
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class InvestigationFilesV2Arguments:
     """InvestigationFilesV2Arguments."""
 
+    cql: Optional[str] = field(default=None, metadata=config(field_name="cql"))
     page: Optional[int] = field(default=None, metadata=config(field_name="page"))
     per_page: Optional[int] = field(default=None, metadata=config(field_name="perPage"))
-    cql: Optional[str] = field(default=None, metadata=config(field_name="cql"))
     investigation_id: Optional[str] = field(
         default=None,
         metadata=config(
             metadata={
                 "deprecated": True,
                 "deprecation_reason": "use cql query field to filter by investigationId. Setting this field will ignore the provided cql query.",
             },
@@ -770,14 +746,137 @@
     """DeleteInvestigationFileInput."""
 
     file_id: Optional[str] = field(default=None, metadata=config(field_name="fileId"))
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class TenantV4:
+    """TenantV4."""
+
+    id: Optional[str] = field(default=None, metadata=config(field_name="id"))
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
+class Subject:
+    """Subject."""
+
+    id: Optional[str] = field(default=None, metadata=config(field_name="id"))
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
+class TDRUser:
+    """TDRUser."""
+
+    id: Optional[str] = field(default=None, metadata=config(field_name="id"))
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
+class InvestigationStatusCount:
+    """InvestigationStatusCount."""
+
+    count: Optional[int] = field(default=None, metadata=config(field_name="count"))
+    status: Optional[InvestigationStatus] = field(
+        default=None, metadata=config(field_name="status")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
+class InvestigationTypeCount:
+    """InvestigationTypeCount."""
+
+    count: Optional[int] = field(default=None, metadata=config(field_name="count"))
+    type: Optional[InvestigationType] = field(
+        default=None, metadata=config(field_name="type")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
+class InvestigationTenantCount:
+    """InvestigationTenantCount."""
+
+    tenant_id: Optional[str] = field(
+        default=None, metadata=config(field_name="tenantId")
+    )
+    count: Optional[int] = field(default=None, metadata=config(field_name="count"))
+    tenant: Optional[TenantV4] = field(
+        default=None, metadata=config(field_name="tenant")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
+class InvestigationCreatorCount:
+    """InvestigationCreatorCount."""
+
+    creator_id: Optional[str] = field(
+        default=None, metadata=config(field_name="creatorId")
+    )
+    count: Optional[int] = field(default=None, metadata=config(field_name="count"))
+    subject: Optional[Subject] = field(
+        default=None, metadata=config(field_name="subject")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
+class InvestigationAssigneeCount:
+    """InvestigationAssigneeCount."""
+
+    assignee_id: Optional[str] = field(
+        default=None, metadata=config(field_name="assigneeId")
+    )
+    count: Optional[int] = field(default=None, metadata=config(field_name="count"))
+    subject: Optional[Subject] = field(
+        default=None, metadata=config(field_name="subject")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
+class InvestigationsV2Arguments:
+    """InvestigationsV2Arguments."""
+
+    cql: Optional[str] = field(default=None, metadata=config(field_name="cql"))
+    page: Optional[int] = field(default=None, metadata=config(field_name="page"))
+    per_page: Optional[int] = field(default=None, metadata=config(field_name="perPage"))
+    search_children_tenants: Optional[bool] = field(
+        default=None, metadata=config(field_name="searchChildrenTenants")
+    )
+    order_by: Optional[PaginationOrder] = field(
+        default=None,
+        metadata=config(
+            metadata={
+                "deprecated": True,
+                "deprecation_reason": "does not do anything - sorting is done through cql",
+            },
+            field_name="orderBy",
+        ),
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
+class ExportInvestigationResourcesArgument:
+    """ExportInvestigationResourcesArgument."""
+
+    id: Optional[str] = field(default=None, metadata=config(field_name="id"))
+    name: Optional[str] = field(default=None, metadata=config(field_name="name"))
+    type: Optional[InvestigationResourceType] = field(
+        default=None, metadata=config(field_name="type")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class CreateInvestigationRuleInput:
     """CreateInvestigationRuleInput."""
 
     name: Optional[str] = field(default=None, metadata=config(field_name="name"))
     title: Optional[str] = field(default=None, metadata=config(field_name="title"))
     description: Optional[str] = field(
         default=None, metadata=config(field_name="description")
@@ -878,85 +977,14 @@
     state: Optional[InvestigationRuleState] = field(
         default=None, metadata=config(field_name="state")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
-class InvestigationStatusCount:
-    """InvestigationStatusCount."""
-
-    count: Optional[int] = field(default=None, metadata=config(field_name="count"))
-    status: Optional[InvestigationStatus] = field(
-        default=None, metadata=config(field_name="status")
-    )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
-class InvestigationTypeCount:
-    """InvestigationTypeCount."""
-
-    count: Optional[int] = field(default=None, metadata=config(field_name="count"))
-    type: Optional[InvestigationType] = field(
-        default=None, metadata=config(field_name="type")
-    )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
-class InvestigationTenantCount:
-    """InvestigationTenantCount."""
-
-    tenant_id: Optional[str] = field(
-        default=None, metadata=config(field_name="tenantId")
-    )
-    count: Optional[int] = field(default=None, metadata=config(field_name="count"))
-    tenant: Optional[TenantV4] = field(
-        default=None, metadata=config(field_name="tenant")
-    )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
-class InvestigationsV2Arguments:
-    """InvestigationsV2Arguments."""
-
-    page: Optional[int] = field(default=None, metadata=config(field_name="page"))
-    per_page: Optional[int] = field(default=None, metadata=config(field_name="perPage"))
-    cql: Optional[str] = field(default=None, metadata=config(field_name="cql"))
-    search_children_tenants: Optional[bool] = field(
-        default=None, metadata=config(field_name="searchChildrenTenants")
-    )
-    order_by: Optional[PaginationOrder] = field(
-        default=None,
-        metadata=config(
-            metadata={
-                "deprecated": True,
-                "deprecation_reason": "does not do anything - sorting is done through cql",
-            },
-            field_name="orderBy",
-        ),
-    )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
-class ExportInvestigationResourcesArgument:
-    """ExportInvestigationResourcesArgument."""
-
-    id: Optional[str] = field(default=None, metadata=config(field_name="id"))
-    name: Optional[str] = field(default=None, metadata=config(field_name="name"))
-    type: Optional[InvestigationResourceType] = field(
-        default=None, metadata=config(field_name="type")
-    )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
 class InvestigationV2Type:
     """InvestigationV2Type."""
 
     description: Optional[str] = field(
         default=None, metadata=config(field_name="description")
     )
     type: Optional[InvestigationType] = field(
@@ -1060,40 +1088,40 @@
 @dataclass(order=True, eq=True, frozen=True)
 class InvestigationV2TimelineArguments:
     """InvestigationV2TimelineArguments."""
 
     investigation_id: Optional[str] = field(
         default=None, metadata=config(field_name="investigationId")
     )
-    page: Optional[int] = field(default=None, metadata=config(field_name="page"))
-    per_page: Optional[int] = field(default=None, metadata=config(field_name="perPage"))
     created_after: Optional[str] = field(
         default=None, metadata=config(field_name="createdAfter")
     )
     created_before: Optional[str] = field(
         default=None, metadata=config(field_name="createdBefore")
     )
+    page: Optional[int] = field(default=None, metadata=config(field_name="page"))
+    per_page: Optional[int] = field(default=None, metadata=config(field_name="perPage"))
     order_by: Optional[PaginationOrder] = field(
         default=None, metadata=config(field_name="orderBy")
     )
     entity_types: Optional[List[InvestigationV2TimelineEntityType]] = field(
         default=None, metadata=config(field_name="entityTypes")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class InvestigationV2TimelineEntity:
     """InvestigationV2TimelineEntity."""
 
-    type: Optional[str] = field(default=None, metadata=config(field_name="type"))
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
     investigation_id: Optional[str] = field(
         default=None, metadata=config(field_name="investigationId")
     )
+    type: Optional[str] = field(default=None, metadata=config(field_name="type"))
     tenant_id: Optional[str] = field(
         default=None, metadata=config(field_name="tenantId")
     )
     created_at: Optional[str] = field(
         default=None, metadata=config(field_name="createdAt")
     )
     timestamp: Optional[str] = field(
@@ -1105,18 +1133,24 @@
     description: Optional[str] = field(
         default=None, metadata=config(field_name="description")
     )
     descriptor: Optional[str] = field(
         default=None, metadata=config(field_name="descriptor")
     )
     user_id: Optional[str] = field(default=None, metadata=config(field_name="userId"))
-    user: Optional[TDRUser] = field(default=None, metadata=config(field_name="user"))
     user_subject: Optional[Subject] = field(
         default=None, metadata=config(field_name="userSubject")
     )
+    user: Optional[TDRUser] = field(
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use userSubject"},
+            field_name="user",
+        ),
+    )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class CommentsV2Arguments:
     """CommentsV2Arguments."""
 
@@ -1147,14 +1181,76 @@
     alerts: Optional[InvestigationProcessingState] = field(
         default=None, metadata=config(field_name="alerts")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class InvestigationFileV2:
+    """InvestigationFileV2."""
+
+    id: Optional[str] = field(default=None, metadata=config(field_name="id"))
+    investigation_id: Optional[str] = field(
+        default=None, metadata=config(field_name="investigationId")
+    )
+    tenant_id: Optional[str] = field(
+        default=None, metadata=config(field_name="tenantId")
+    )
+    created_at: Optional[str] = field(
+        default=None, metadata=config(field_name="createdAt")
+    )
+    updated_at: Optional[str] = field(
+        default=None, metadata=config(field_name="updatedAt")
+    )
+    deleted_at: Optional[str] = field(
+        default=None, metadata=config(field_name="deletedAt")
+    )
+    uploaded_by_id: Optional[str] = field(
+        default=None, metadata=config(field_name="uploadedById")
+    )
+    deleted_by_id: Optional[str] = field(
+        default=None, metadata=config(field_name="deletedById")
+    )
+    name: Optional[str] = field(default=None, metadata=config(field_name="name"))
+    path: Optional[str] = field(default=None, metadata=config(field_name="path"))
+    size: Optional[int] = field(default=None, metadata=config(field_name="size"))
+    status: Optional[str] = field(default=None, metadata=config(field_name="status"))
+    download_url: Optional[str] = field(
+        default=None, metadata=config(field_name="downloadURL")
+    )
+    uploaded_by_subject: Optional[Subject] = field(
+        default=None, metadata=config(field_name="uploadedBySubject")
+    )
+    deleted_by_subject: Optional[Subject] = field(
+        default=None, metadata=config(field_name="deletedBySubject")
+    )
+    metadata: Optional[InvestigationFileMeta] = field(
+        default=None, metadata=config(field_name="metadata")
+    )
+    uploaded_by: Optional[TDRUser] = field(
+        default=None,
+        metadata=config(
+            metadata={
+                "deprecated": True,
+                "deprecation_reason": "use uploadedBySubject",
+            },
+            field_name="uploadedBy",
+        ),
+    )
+    deleted_by: Optional[TDRUser] = field(
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use deletedBySubject"},
+            field_name="deletedBy",
+        ),
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class AggregatedCounts:
     """AggregatedCounts."""
 
     archived_count: Optional[int] = field(
         default=None, metadata=config(field_name="archivedCount")
     )
     status: Optional[List[InvestigationStatusCount]] = field(
@@ -1165,34 +1261,40 @@
     )
     priority: Optional[List[InvestigationPriorityCount]] = field(
         default=None, metadata=config(field_name="priority")
     )
     tenant: Optional[List[InvestigationTenantCount]] = field(
         default=None, metadata=config(field_name="tenant")
     )
+    assignee: Optional[List[InvestigationAssigneeCount]] = field(
+        default=None, metadata=config(field_name="assignee")
+    )
+    creator: Optional[List[InvestigationCreatorCount]] = field(
+        default=None, metadata=config(field_name="creator")
+    )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class InvestigationTemplate:
     """InvestigationTemplate."""
 
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
-    created_at: Optional[str] = field(
-        default=None, metadata=config(field_name="createdAt")
-    )
     created_by_id: Optional[str] = field(
         default=None, metadata=config(field_name="createdById")
     )
-    updated_at: Optional[str] = field(
-        default=None, metadata=config(field_name="updatedAt")
+    created_at: Optional[str] = field(
+        default=None, metadata=config(field_name="createdAt")
     )
     updated_by_id: Optional[str] = field(
         default=None, metadata=config(field_name="updatedById")
     )
+    updated_at: Optional[str] = field(
+        default=None, metadata=config(field_name="updatedAt")
+    )
     tenant_id: Optional[str] = field(
         default=None, metadata=config(field_name="tenantId")
     )
     name: Optional[str] = field(default=None, metadata=config(field_name="name"))
     title: Optional[str] = field(default=None, metadata=config(field_name="title"))
     description: Optional[str] = field(
         default=None, metadata=config(field_name="description")
@@ -1218,100 +1320,67 @@
     )
     investigation_assignee: Optional[str] = field(
         default=None, metadata=config(field_name="investigationAssignee")
     )
     investigation_status: Optional[str] = field(
         default=None, metadata=config(field_name="investigationStatus")
     )
-    created_by: Optional[TDRUser] = field(
-        default=None, metadata=config(field_name="createdBy")
-    )
     created_by_subject: Optional[Subject] = field(
         default=None, metadata=config(field_name="createdBySubject")
     )
-    updated_by: Optional[TDRUser] = field(
-        default=None, metadata=config(field_name="updatedBy")
-    )
     updated_by_subject: Optional[Subject] = field(
         default=None, metadata=config(field_name="updatedBySubject")
     )
-    investigation_assignee_user: Optional[TDRUser] = field(
-        default=None, metadata=config(field_name="investigationAssigneeUser")
-    )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
-class InvestigationFileV2:
-    """InvestigationFileV2."""
-
-    id: Optional[str] = field(default=None, metadata=config(field_name="id"))
-    investigation_id: Optional[str] = field(
-        default=None, metadata=config(field_name="investigationId")
-    )
-    tenant_id: Optional[str] = field(
-        default=None, metadata=config(field_name="tenantId")
+    investigation_assignee_subject: Optional[Subject] = field(
+        default=None, metadata=config(field_name="investigationAssigneeSubject")
     )
-    created_at: Optional[str] = field(
-        default=None, metadata=config(field_name="createdAt")
-    )
-    updated_at: Optional[str] = field(
-        default=None, metadata=config(field_name="updatedAt")
-    )
-    deleted_at: Optional[str] = field(
-        default=None, metadata=config(field_name="deletedAt")
-    )
-    uploaded_by_id: Optional[str] = field(
-        default=None, metadata=config(field_name="uploadedById")
-    )
-    deleted_by_id: Optional[str] = field(
-        default=None, metadata=config(field_name="deletedById")
-    )
-    name: Optional[str] = field(default=None, metadata=config(field_name="name"))
-    path: Optional[str] = field(default=None, metadata=config(field_name="path"))
-    size: Optional[int] = field(default=None, metadata=config(field_name="size"))
-    status: Optional[str] = field(default=None, metadata=config(field_name="status"))
-    download_url: Optional[str] = field(
-        default=None, metadata=config(field_name="downloadURL")
-    )
-    uploaded_by: Optional[TDRUser] = field(
-        default=None, metadata=config(field_name="uploadedBy")
-    )
-    uploaded_by_subject: Optional[Subject] = field(
-        default=None, metadata=config(field_name="uploadedBySubject")
-    )
-    deleted_by: Optional[TDRUser] = field(
-        default=None, metadata=config(field_name="deletedBy")
+    created_by: Optional[TDRUser] = field(
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use createdBySubject"},
+            field_name="createdBy",
+        ),
     )
-    deleted_by_subject: Optional[Subject] = field(
-        default=None, metadata=config(field_name="deletedBySubject")
+    updated_by: Optional[TDRUser] = field(
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use updatedBySubject"},
+            field_name="updatedBy",
+        ),
     )
-    metadata: Optional[InvestigationFileMeta] = field(
-        default=None, metadata=config(field_name="metadata")
+    investigation_assignee_user: Optional[TDRUser] = field(
+        default=None,
+        metadata=config(
+            metadata={
+                "deprecated": True,
+                "deprecation_reason": "use investigationAssignee",
+            },
+            field_name="investigationAssigneeUser",
+        ),
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class InvestigationRule:
     """InvestigationRule."""
 
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
-    created_at: Optional[str] = field(
-        default=None, metadata=config(field_name="createdAt")
-    )
     created_by_id: Optional[str] = field(
         default=None, metadata=config(field_name="createdById")
     )
-    updated_at: Optional[str] = field(
-        default=None, metadata=config(field_name="updatedAt")
+    created_at: Optional[str] = field(
+        default=None, metadata=config(field_name="createdAt")
     )
     updated_by_id: Optional[str] = field(
         default=None, metadata=config(field_name="updatedById")
     )
+    updated_at: Optional[str] = field(
+        default=None, metadata=config(field_name="updatedAt")
+    )
     tenant_id: Optional[str] = field(
         default=None, metadata=config(field_name="tenantId")
     )
     name: Optional[str] = field(default=None, metadata=config(field_name="name"))
     title: Optional[str] = field(default=None, metadata=config(field_name="title"))
     description: Optional[str] = field(
         default=None, metadata=config(field_name="description")
@@ -1359,49 +1428,57 @@
     exclude_child_tenants: Optional[bool] = field(
         default=None,
         metadata=config(
             metadata={"deprecated": True, "deprecation_reason": "use tenantFilter"},
             field_name="excludeChildTenants",
         ),
     )
-    created_by: Optional[TDRUser] = field(
-        default=None, metadata=config(field_name="createdBy")
-    )
     created_by_subject: Optional[Subject] = field(
         default=None, metadata=config(field_name="createdBySubject")
     )
-    updated_by: Optional[TDRUser] = field(
-        default=None, metadata=config(field_name="updatedBy")
-    )
     updated_by_subject: Optional[Subject] = field(
         default=None, metadata=config(field_name="updatedBySubject")
     )
     state: Optional[InvestigationRuleState] = field(
         default=None, metadata=config(field_name="state")
     )
     template: Optional[InvestigationTemplate] = field(
         default=None, metadata=config(field_name="template")
     )
+    created_by: Optional[TDRUser] = field(
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use createdBySubject"},
+            field_name="createdBy",
+        ),
+    )
+    updated_by: Optional[TDRUser] = field(
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use updatedBySubject"},
+            field_name="updatedBy",
+        ),
+    )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class CommentV2:
     """CommentV2."""
 
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
+    author_id: Optional[str] = field(
+        default=None, metadata=config(field_name="authorId")
+    )
     created_at: Optional[str] = field(
         default=None, metadata=config(field_name="createdAt")
     )
     updated_at: Optional[str] = field(
         default=None, metadata=config(field_name="updatedAt")
     )
-    author_id: Optional[str] = field(
-        default=None, metadata=config(field_name="authorId")
-    )
     comment: Optional[str] = field(default=None, metadata=config(field_name="comment"))
     investigation_id: Optional[str] = field(
         default=None, metadata=config(field_name="investigationId")
     )
     tenant_id: Optional[str] = field(
         default=None, metadata=config(field_name="tenantId")
     )
@@ -1410,31 +1487,43 @@
     )
     read_by_ids: Optional[List[str]] = field(
         default=None, metadata=config(field_name="readByIds")
     )
     is_internal: Optional[bool] = field(
         default=None, metadata=config(field_name="isInternal")
     )
-    author: Optional[TDRUser] = field(
-        default=None, metadata=config(field_name="author")
-    )
     author_subject: Optional[Subject] = field(
         default=None, metadata=config(field_name="authorSubject")
     )
     mentions_subjects: Optional[List[Subject]] = field(
         default=None, metadata=config(field_name="mentionsSubjects")
     )
-    mentions_users: Optional[List[TDRUser]] = field(
-        default=None, metadata=config(field_name="mentionsUsers")
-    )
     read_by_subjects: Optional[List[Subject]] = field(
         default=None, metadata=config(field_name="readBySubjects")
     )
+    author: Optional[TDRUser] = field(
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use authorSubject"},
+            field_name="author",
+        ),
+    )
+    mentions_users: Optional[List[TDRUser]] = field(
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use mentionsSubjects"},
+            field_name="mentionsUsers",
+        ),
+    )
     read_by: Optional[List[TDRUser]] = field(
-        default=None, metadata=config(field_name="readBy")
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use readBySubjects"},
+            field_name="readBy",
+        ),
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class InvestigationV2:
     """InvestigationV2."""
@@ -1453,42 +1542,42 @@
     )
     events_evidence_count: Optional[int] = field(
         default=None, metadata=config(field_name="eventsEvidenceCount")
     )
     search_queries_evidence_count: Optional[int] = field(
         default=None, metadata=config(field_name="searchQueriesEvidenceCount")
     )
+    priority: Optional[int] = field(
+        default=None, metadata=config(field_name="priority")
+    )
     tags: Optional[List[str]] = field(default=None, metadata=config(field_name="tags"))
     contributor_ids: Optional[List[str]] = field(
         default=None, metadata=config(field_name="contributorIds")
     )
     assignee_id: Optional[str] = field(
         default=None, metadata=config(field_name="assigneeId")
     )
     tenant_id: Optional[str] = field(
         default=None, metadata=config(field_name="tenantId")
     )
-    created_at: Optional[str] = field(
-        default=None, metadata=config(field_name="createdAt")
-    )
     created_by_id: Optional[str] = field(
         default=None, metadata=config(field_name="createdById")
     )
-    updated_at: Optional[str] = field(
-        default=None, metadata=config(field_name="updatedAt")
+    created_at: Optional[str] = field(
+        default=None, metadata=config(field_name="createdAt")
     )
     updated_by_id: Optional[str] = field(
         default=None, metadata=config(field_name="updatedById")
     )
+    updated_at: Optional[str] = field(
+        default=None, metadata=config(field_name="updatedAt")
+    )
     archived_at: Optional[str] = field(
         default=None, metadata=config(field_name="archivedAt")
     )
-    priority: Optional[int] = field(
-        default=None, metadata=config(field_name="priority")
-    )
     close_reason: Optional[str] = field(
         default=None, metadata=config(field_name="closeReason")
     )
     rule_id: Optional[str] = field(default=None, metadata=config(field_name="ruleId"))
     service_desk_id: Optional[str] = field(
         default=None, metadata=config(field_name="serviceDeskId")
     )
@@ -1548,44 +1637,35 @@
     )
     events_evidence: Optional[List[EventEvidence]] = field(
         default=None, metadata=config(field_name="eventsEvidence")
     )
     search_queries_evidence: Optional[List[SearchQueryEvidence]] = field(
         default=None, metadata=config(field_name="searchQueriesEvidence")
     )
+    type: Optional[InvestigationType] = field(
+        default=None, metadata=config(field_name="type")
+    )
     status: Optional[InvestigationStatus] = field(
         default=None, metadata=config(field_name="status")
     )
-    contributors: Optional[List[TDRUser]] = field(
-        default=None, metadata=config(field_name="contributors")
-    )
     contributor_subjects: Optional[List[Subject]] = field(
         default=None, metadata=config(field_name="contributorSubjects")
     )
     assignee_subject: Optional[Subject] = field(
         default=None, metadata=config(field_name="assigneeSubject")
     )
     tenant: Optional[TenantV4] = field(
         default=None, metadata=config(field_name="tenant")
     )
-    created_by: Optional[TDRUser] = field(
-        default=None, metadata=config(field_name="createdBy")
-    )
     created_by_subject: Optional[Subject] = field(
         default=None, metadata=config(field_name="createdBySubject")
     )
-    updated_by: Optional[TDRUser] = field(
-        default=None, metadata=config(field_name="updatedBy")
-    )
     updated_by_subject: Optional[Subject] = field(
         default=None, metadata=config(field_name="updatedBySubject")
     )
-    type: Optional[InvestigationType] = field(
-        default=None, metadata=config(field_name="type")
-    )
     processing_status: Optional[InvestigationProcessingStatus] = field(
         default=None, metadata=config(field_name="processingStatus")
     )
     comments_count: Optional[InvestigationCommentsCount] = field(
         default=None, metadata=config(field_name="commentsCount")
     )
     metrics: Optional[Metric] = field(
@@ -1604,14 +1684,38 @@
     assignee: Optional[TDRUser] = field(
         default=None,
         metadata=config(
             metadata={"deprecated": True, "deprecation_reason": "use assigneeSubject"},
             field_name="assignee",
         ),
     )
+    contributors: Optional[List[TDRUser]] = field(
+        default=None,
+        metadata=config(
+            metadata={
+                "deprecated": True,
+                "deprecation_reason": "use contributorSubjects",
+            },
+            field_name="contributors",
+        ),
+    )
+    created_by: Optional[TDRUser] = field(
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use createdBySubject"},
+            field_name="createdBy",
+        ),
+    )
+    updated_by: Optional[TDRUser] = field(
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use updatedBySubject"},
+            field_name="updatedBy",
+        ),
+    )
     metric: Optional[Metric] = field(
         default=None,
         metadata=config(
             metadata={"deprecated": True, "deprecation_reason": "use metrics"},
             field_name="metric",
         ),
     )
```

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/mitre_attack_info/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/mitre_attack_info/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/mitre_attack_info/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/mitre_attack_info/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/mitre_attack_info/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/mitre_attack_info/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/mitre_attack_info/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/mitre_attack_info/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/mitre_attack_info/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/mitre_attack_info/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_context/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/multi_tenant_context/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_context/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/multi_tenant_context/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_context/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/multi_tenant_context/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_context/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/multi_tenant_context/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_context/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/multi_tenant_context/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_ioc/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/multi_tenant_ioc/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_ioc/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/multi_tenant_ioc/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_ioc/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/multi_tenant_ioc/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_ioc/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/multi_tenant_ioc/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_ioc/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/multi_tenant_ioc/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/notebooks/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/notebooks/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/notebooks/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/notebooks/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/notebooks/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/notebooks/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/notebooks/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/notebooks/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/notebooks/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/notifications/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/notifications/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/notifications/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/notifications/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/notifications/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/notifications/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/notifications/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/notifications/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/notifications/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/preferences/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/preferences/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/preferences/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/preferences/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/preferences/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/preferences/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/preferences/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/preferences/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/preferences/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/preferences/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/queries/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/queries/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/queries/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/queries/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/queries/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/queries/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/queries/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/queries/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/queries/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/queries/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/roadrunner/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/roadrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/roadrunner/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/roadrunner/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/roadrunner/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/roadrunner/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/roadrunner/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/roadrunner/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/roadrunner/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/roadrunner/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/rules/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/rules/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/rules/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/rules/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/rules/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/rules/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/rules/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/rules/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/rules/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/sharelinks/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/sharelinks/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/sharelinks/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/sharelinks/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/sharelinks/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/sharelinks/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/sharelinks/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/sharelinks/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/sharelinks/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/sharelinks/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/subjects/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/subjects/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/subjects/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/subjects/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/subjects/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/subjects/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/subjects/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/subjects/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/subjects/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/subjects/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenant_profiles/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/tenant_profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenant_profiles/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/tenant_profiles/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenant_profiles/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/tenant_profiles/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenant_profiles/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/tenant_profiles/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenant_profiles/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/tenant_profiles/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenants/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/tenants/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenants/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/tenants/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenants/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/tenants/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenants/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/tenants/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenants/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/tenants/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,18 @@
     DESC = "desc"
 
 
 class TenantEnvironment(str, Enum):
     """TenantEnvironment."""
 
     PILOT = "pilot"
+    PILOT_CHARLIE = "pilot_charlie"
+    PILOT_DELTA = "pilot_delta"
+    PILOT_ECHO = "pilot_echo"
+    PILOT_FOXTROT = "pilot_foxtrot"
     CHARLIE = "charlie"
     ECHO = "echo"
     DELTA = "delta"
     FOXTROT = "foxtrot"
 
 
 class SSOEnvironment(str, Enum):
@@ -120,14 +124,15 @@
     CREATE_TENANT = "create_tenant"
     DELETE_LABEL_FROM_TENANT = "delete_label_from_tenant"
     DELETE_SSO_CONNECTION = "delete_sso_connection"
     DISABLED_SUPPORT_STATUS = "disabled_support_status"
     ENABLE_TENANT = "enable_tenant"
     ENABLED_SUPPORT_STATUS = "enabled_support_status"
     REMOVE_SERVICE_TO_TENANT = "remove_service_to_tenant"
+    DELETE_SERVICE_FROM_TENANT = "delete_service_from_tenant"
     TENANT_ADDED = "tenant_added"
     TENANT_DISABLED = "tenant_disabled"
     TENANT_REMOVED = "tenant_removed"
     TENANT_UPDATED = "tenant_updated"
     UPDATE_LABEL_FOR_TENANT = "update_label_for_tenant"
     UPDATE_SSO_CONNECTION = "update_sso_connection"
     CREATE_SERVICE = "create_service"
```

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/threat/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/threat/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/threat/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/threat/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/threat/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat_score/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/threat_score/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat_score/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/threat_score/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat_score/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/threat_score/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat_score/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/threat_score/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat_score/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/threat_score/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/trip/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/trip/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/trip/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/trip/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/trip/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/trip/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/trip/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/trip/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/trip/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/trip/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/users/__init__.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/users/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/users/mutations.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/users/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/users/queries.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/users/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/users/subscriptions.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/users/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/services/users/types.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/services/users/types.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/tokens.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/tokens.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python/utils.py` & `taegis_sdk_python-1.2.7/taegis_sdk_python/utils.py`

 * *Files identical despite different names*

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python.egg-info/PKG-INFO` & `taegis_sdk_python-1.2.7/taegis_sdk_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taegis-sdk-python
-Version: 1.2.6
+Version: 1.2.7
 Summary: Taegis Python SDK
 Home-page: https://github.com/secureworks/taegis-sdk-python
 Author: Secureworks
 Author-email: sdks@secureworks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `taegis_sdk_python-1.2.6/taegis_sdk_python.egg-info/SOURCES.txt` & `taegis_sdk_python-1.2.7/taegis_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

