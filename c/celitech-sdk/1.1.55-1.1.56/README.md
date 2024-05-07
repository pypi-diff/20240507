# Comparing `tmp/celitech_sdk-1.1.55.tar.gz` & `tmp/celitech_sdk-1.1.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celitech_sdk-1.1.55.tar", last modified: Thu May  2 11:27:29 2024, max compression
+gzip compressed data, was "celitech_sdk-1.1.56.tar", last modified: Tue May  7 17:37:31 2024, max compression
```

## Comparing `celitech_sdk-1.1.55.tar` & `celitech_sdk-1.1.56.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.961631 celitech_sdk-1.1.55/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13798 2024-05-02 11:27:29.961631 celitech_sdk-1.1.55/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13417 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 11:27:29.961631 celitech_sdk-1.1.55/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.945631 celitech_sdk-1.1.55/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.949631 celitech_sdk-1.1.55/src/celitech/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.949631 celitech_sdk-1.1.55/src/celitech/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/hooks/hook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.953631 celitech_sdk-1.1.55/src/celitech/models/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/create_purchase_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/create_purchase_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/edit_purchase_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/edit_purchase_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/get_esim_device_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/get_esim_history_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/get_esim_mac_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/get_esim_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/get_purchase_consumption_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/list_destinations_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/list_packages_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/list_purchases_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/top_up_esim_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/top_up_esim_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.953631 celitech_sdk-1.1.55/src/celitech/models/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/utils/cast_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/utils/json_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.953631 celitech_sdk-1.1.55/src/celitech/net/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.953631 celitech_sdk-1.1.55/src/celitech/net/environment/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/environment/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.953631 celitech_sdk-1.1.55/src/celitech/net/headers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/headers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/headers/base_header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.953631 celitech_sdk-1.1.55/src/celitech/net/request_chain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/request_chain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.957631 celitech_sdk-1.1.55/src/celitech/net/request_chain/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/request_chain/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/request_chain/handlers/base_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/request_chain/handlers/hook_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/request_chain/handlers/http_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/request_chain/handlers/retry_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/request_chain/request_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.957631 celitech_sdk-1.1.55/src/celitech/net/transport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/transport/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/transport/request_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/transport/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/transport/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/transport/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.957631 celitech_sdk-1.1.55/src/celitech/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/services/destinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/services/e_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/services/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/services/purchases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.957631 celitech_sdk-1.1.55/src/celitech/services/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/services/utils/base_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/services/utils/default_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/services/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.957631 celitech_sdk-1.1.55/src/celitech_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13798 2024-05-02 11:27:29.000000 celitech_sdk-1.1.55/src/celitech_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-02 11:27:29.000000 celitech_sdk-1.1.55/src/celitech_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 11:27:29.000000 celitech_sdk-1.1.55/src/celitech_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-02 11:27:29.000000 celitech_sdk-1.1.55/src/celitech_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 11:27:29.000000 celitech_sdk-1.1.55/src/celitech_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.207803 celitech_sdk-1.1.56/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14758 2024-05-07 17:37:31.207803 celitech_sdk-1.1.56/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14377 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 17:37:31.207803 celitech_sdk-1.1.56/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.191803 celitech_sdk-1.1.56/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.191803 celitech_sdk-1.1.56/src/celitech/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.191803 celitech_sdk-1.1.56/src/celitech/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/hooks/hook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.195803 celitech_sdk-1.1.56/src/celitech/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/create_purchase_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/create_purchase_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/edit_purchase_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/edit_purchase_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/get_esim_device_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/get_esim_history_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/get_esim_mac_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/get_esim_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/get_purchase_consumption_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/list_destinations_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/list_packages_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/list_purchases_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/top_up_esim_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/top_up_esim_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.195803 celitech_sdk-1.1.56/src/celitech/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/utils/cast_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/utils/json_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.195803 celitech_sdk-1.1.56/src/celitech/net/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.195803 celitech_sdk-1.1.56/src/celitech/net/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/environment/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.199803 celitech_sdk-1.1.56/src/celitech/net/headers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/headers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/headers/base_header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.199803 celitech_sdk-1.1.56/src/celitech/net/request_chain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/request_chain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.199803 celitech_sdk-1.1.56/src/celitech/net/request_chain/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/request_chain/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/request_chain/handlers/base_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/request_chain/handlers/hook_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/request_chain/handlers/http_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/request_chain/handlers/retry_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/request_chain/request_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.203803 celitech_sdk-1.1.56/src/celitech/net/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/transport/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/transport/request_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/transport/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/transport/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/transport/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.203803 celitech_sdk-1.1.56/src/celitech/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/services/destinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/services/e_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/services/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/services/purchases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.203803 celitech_sdk-1.1.56/src/celitech/services/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/services/utils/base_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/services/utils/default_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/services/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.203803 celitech_sdk-1.1.56/src/celitech_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14758 2024-05-07 17:37:31.000000 celitech_sdk-1.1.56/src/celitech_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-07 17:37:31.000000 celitech_sdk-1.1.56/src/celitech_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 17:37:31.000000 celitech_sdk-1.1.56/src/celitech_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 17:37:31.000000 celitech_sdk-1.1.56/src/celitech_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 17:37:31.000000 celitech_sdk-1.1.56/src/celitech_sdk.egg-info/top_level.txt
```

### Comparing `celitech_sdk-1.1.55/LICENSE` & `celitech_sdk-1.1.56/LICENSE`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/PKG-INFO` & `celitech_sdk-1.1.56/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: celitech-sdk
-Version: 1.1.55
+Version: 1.1.56
 Summary: Welcome to the CELITECH API documentation!  Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/) 
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 
-# Celitech Python SDK 1.1.55
+# Celitech Python SDK 1.1.56
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.1.55
+- SDK version: 1.1.56
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
@@ -63,16 +63,17 @@
 
 Name of the destinations
 
 - HTTP Method: `GET`
 - Endpoint: `/destinations`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
+
+| Name | Type | Required | Description |
+| :--- | :--- | :------: | :---------- |
 
 **Return Type**
 
 `ListDestinationsOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -100,24 +101,25 @@
 
 List of available packages
 
 - HTTP Method: `GET`
 - Endpoint: `/packages`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| destination | str | ❌ | List of available packages |
-| start_date | str | ❌ | List of available packages |
-| end_date | str | ❌ | List of available packages |
-| after_cursor | str | ❌ | List of available packages |
-| limit | float | ❌ | List of available packages |
-| start_time | int | ❌ | List of available packages |
-| end_time | int | ❌ | List of available packages |
-| duration | float | ❌ | List of available packages |
+
+| Name         | Type  | Required | Description                |
+| :----------- | :---- | :------: | :------------------------- |
+| destination  | str   |    ❌    | List of available packages |
+| start_date   | str   |    ❌    | List of available packages |
+| end_date     | str   |    ❌    | List of available packages |
+| after_cursor | str   |    ❌    | List of available packages |
+| limit        | float |    ❌    | List of available packages |
+| start_time   | int   |    ❌    | List of available packages |
+| end_time     | int   |    ❌    | List of available packages |
+| duration     | float |    ❌    | List of available packages |
 
 **Return Type**
 
 `ListPackagesOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -149,23 +151,24 @@
 
 This endpoint can be used to list all the successful purchases made between a given interval.
 
 - HTTP Method: `GET`
 - Endpoint: `/purchases`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| iccid | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
-| after_date | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
-| before_date | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
-| after_cursor | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
-| limit | float | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
-| after | float | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
-| before | float | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
+
+| Name         | Type  | Required | Description                                                                                   |
+| :----------- | :---- | :------: | :-------------------------------------------------------------------------------------------- |
+| iccid        | str   |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
+| after_date   | str   |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
+| before_date  | str   |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
+| after_cursor | str   |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
+| limit        | float |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
+| after        | float |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
+| before       | float |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
 
 **Return Type**
 
 `ListPurchasesOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -185,17 +188,18 @@
 
 This endpoint is used to purchase a new eSIM by providing the package details.
 
 - HTTP Method: `POST`
 - Endpoint: `/purchases`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| request_body | CreatePurchaseRequest | ❌ | The request body. |
+
+| Name         | Type                  | Required | Description       |
+| :----------- | :-------------------- | :------: | :---------------- |
+| request_body | CreatePurchaseRequest |    ❌    | The request body. |
 
 **Return Type**
 
 `CreatePurchaseOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -215,17 +219,18 @@
 
 This endpoint is used to top-up an eSIM with the previously associated destination by providing an existing ICCID and the package details. The top-up is not feasible for eSIMs in "DELETED" or "ERROR" state.
 
 - HTTP Method: `POST`
 - Endpoint: `/purchases/topup`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| request_body | TopUpEsimRequest | ❌ | The request body. |
+
+| Name         | Type             | Required | Description       |
+| :----------- | :--------------- | :------: | :---------------- |
+| request_body | TopUpEsimRequest |    ❌    | The request body. |
 
 **Return Type**
 
 `TopUpEsimOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -245,17 +250,18 @@
 
 This endpoint allows you to modify the dates of an existing package with a future activation start time. Editing can only be performed for packages that have not been activated, and it cannot change the package size. The modification must not change the package duration category to ensure pricing consistency.
 
 - HTTP Method: `POST`
 - Endpoint: `/purchases/edit`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| request_body | EditPurchaseRequest | ❌ | The request body. |
+
+| Name         | Type                | Required | Description       |
+| :----------- | :------------------ | :------: | :---------------- |
+| request_body | EditPurchaseRequest |    ❌    | The request body. |
 
 **Return Type**
 
 `EditPurchaseOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -275,17 +281,18 @@
 
 This endpoint can be called for consumption notifications (e.g. every 1 hour or when the user clicks a button). It returns the data balance (consumption) of purchased packages.
 
 - HTTP Method: `GET`
 - Endpoint: `/purchases/{purchaseId}/consumption`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| purchase_id | str | ✅ | This endpoint can be called for consumption notifications (e.g. every 1 hour or when the user clicks a button). It returns the data balance (consumption) of purchased packages. |
+
+| Name        | Type | Required | Description                                                                                                                                                                      |
+| :---------- | :--- | :------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| purchase_id | str  |    ✅    | This endpoint can be called for consumption notifications (e.g. every 1 hour or when the user clicks a button). It returns the data balance (consumption) of purchased packages. |
 
 **Return Type**
 
 `GetPurchaseConsumptionOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -316,17 +323,18 @@
 
 Get status from eSIM
 
 - HTTP Method: `GET`
 - Endpoint: `/esim`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| iccid | str | ✅ | Get status from eSIM |
+
+| Name  | Type | Required | Description          |
+| :---- | :--- | :------: | :------------------- |
+| iccid | str  |    ✅    | Get status from eSIM |
 
 **Return Type**
 
 `GetEsimOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -346,17 +354,18 @@
 
 Get device info from an installed eSIM
 
 - HTTP Method: `GET`
 - Endpoint: `/esim/{iccid}/device`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| iccid | str | ✅ | Get device info from an installed eSIM |
+
+| Name  | Type | Required | Description                            |
+| :---- | :--- | :------: | :------------------------------------- |
+| iccid | str  |    ✅    | Get device info from an installed eSIM |
 
 **Return Type**
 
 `GetEsimDeviceOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -376,17 +385,18 @@
 
 Get history from an eSIM
 
 - HTTP Method: `GET`
 - Endpoint: `/esim/{iccid}/history`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| iccid | str | ✅ | Get history from an eSIM |
+
+| Name  | Type | Required | Description              |
+| :---- | :--- | :------: | :----------------------- |
+| iccid | str  |    ✅    | Get history from an eSIM |
 
 **Return Type**
 
 `GetEsimHistoryOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -406,17 +416,18 @@
 
 Get MAC from eSIM
 
 - HTTP Method: `GET`
 - Endpoint: `/esim/{iccid}/mac`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| iccid | str | ✅ | Get MAC from eSIM |
+
+| Name  | Type | Required | Description       |
+| :---- | :--- | :------: | :---------------- |
+| iccid | str  |    ✅    | Get MAC from eSIM |
 
 **Return Type**
 
 `GetEsimMacOkResponse`
 
 **Example Usage Code Snippet**
```

### Comparing `celitech_sdk-1.1.55/README.md` & `celitech_sdk-1.1.56/src/celitech_sdk.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,23 @@
-# Celitech Python SDK 1.1.55
+Metadata-Version: 2.1
+Name: celitech-sdk
+Version: 1.1.56
+Summary: Welcome to the CELITECH API documentation!  Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/) 
+License: MIT
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.31.0
+
+# Celitech Python SDK 1.1.56
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.1.55
+- SDK version: 1.1.56
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
@@ -53,16 +63,17 @@
 
 Name of the destinations
 
 - HTTP Method: `GET`
 - Endpoint: `/destinations`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
+
+| Name | Type | Required | Description |
+| :--- | :--- | :------: | :---------- |
 
 **Return Type**
 
 `ListDestinationsOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -90,24 +101,25 @@
 
 List of available packages
 
 - HTTP Method: `GET`
 - Endpoint: `/packages`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| destination | str | ❌ | List of available packages |
-| start_date | str | ❌ | List of available packages |
-| end_date | str | ❌ | List of available packages |
-| after_cursor | str | ❌ | List of available packages |
-| limit | float | ❌ | List of available packages |
-| start_time | int | ❌ | List of available packages |
-| end_time | int | ❌ | List of available packages |
-| duration | float | ❌ | List of available packages |
+
+| Name         | Type  | Required | Description                |
+| :----------- | :---- | :------: | :------------------------- |
+| destination  | str   |    ❌    | List of available packages |
+| start_date   | str   |    ❌    | List of available packages |
+| end_date     | str   |    ❌    | List of available packages |
+| after_cursor | str   |    ❌    | List of available packages |
+| limit        | float |    ❌    | List of available packages |
+| start_time   | int   |    ❌    | List of available packages |
+| end_time     | int   |    ❌    | List of available packages |
+| duration     | float |    ❌    | List of available packages |
 
 **Return Type**
 
 `ListPackagesOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -139,23 +151,24 @@
 
 This endpoint can be used to list all the successful purchases made between a given interval.
 
 - HTTP Method: `GET`
 - Endpoint: `/purchases`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| iccid | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
-| after_date | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
-| before_date | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
-| after_cursor | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
-| limit | float | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
-| after | float | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
-| before | float | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
+
+| Name         | Type  | Required | Description                                                                                   |
+| :----------- | :---- | :------: | :-------------------------------------------------------------------------------------------- |
+| iccid        | str   |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
+| after_date   | str   |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
+| before_date  | str   |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
+| after_cursor | str   |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
+| limit        | float |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
+| after        | float |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
+| before       | float |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
 
 **Return Type**
 
 `ListPurchasesOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -175,17 +188,18 @@
 
 This endpoint is used to purchase a new eSIM by providing the package details.
 
 - HTTP Method: `POST`
 - Endpoint: `/purchases`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| request_body | CreatePurchaseRequest | ❌ | The request body. |
+
+| Name         | Type                  | Required | Description       |
+| :----------- | :-------------------- | :------: | :---------------- |
+| request_body | CreatePurchaseRequest |    ❌    | The request body. |
 
 **Return Type**
 
 `CreatePurchaseOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -205,17 +219,18 @@
 
 This endpoint is used to top-up an eSIM with the previously associated destination by providing an existing ICCID and the package details. The top-up is not feasible for eSIMs in "DELETED" or "ERROR" state.
 
 - HTTP Method: `POST`
 - Endpoint: `/purchases/topup`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| request_body | TopUpEsimRequest | ❌ | The request body. |
+
+| Name         | Type             | Required | Description       |
+| :----------- | :--------------- | :------: | :---------------- |
+| request_body | TopUpEsimRequest |    ❌    | The request body. |
 
 **Return Type**
 
 `TopUpEsimOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -235,17 +250,18 @@
 
 This endpoint allows you to modify the dates of an existing package with a future activation start time. Editing can only be performed for packages that have not been activated, and it cannot change the package size. The modification must not change the package duration category to ensure pricing consistency.
 
 - HTTP Method: `POST`
 - Endpoint: `/purchases/edit`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| request_body | EditPurchaseRequest | ❌ | The request body. |
+
+| Name         | Type                | Required | Description       |
+| :----------- | :------------------ | :------: | :---------------- |
+| request_body | EditPurchaseRequest |    ❌    | The request body. |
 
 **Return Type**
 
 `EditPurchaseOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -265,17 +281,18 @@
 
 This endpoint can be called for consumption notifications (e.g. every 1 hour or when the user clicks a button). It returns the data balance (consumption) of purchased packages.
 
 - HTTP Method: `GET`
 - Endpoint: `/purchases/{purchaseId}/consumption`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| purchase_id | str | ✅ | This endpoint can be called for consumption notifications (e.g. every 1 hour or when the user clicks a button). It returns the data balance (consumption) of purchased packages. |
+
+| Name        | Type | Required | Description                                                                                                                                                                      |
+| :---------- | :--- | :------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| purchase_id | str  |    ✅    | This endpoint can be called for consumption notifications (e.g. every 1 hour or when the user clicks a button). It returns the data balance (consumption) of purchased packages. |
 
 **Return Type**
 
 `GetPurchaseConsumptionOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -306,17 +323,18 @@
 
 Get status from eSIM
 
 - HTTP Method: `GET`
 - Endpoint: `/esim`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| iccid | str | ✅ | Get status from eSIM |
+
+| Name  | Type | Required | Description          |
+| :---- | :--- | :------: | :------------------- |
+| iccid | str  |    ✅    | Get status from eSIM |
 
 **Return Type**
 
 `GetEsimOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -336,17 +354,18 @@
 
 Get device info from an installed eSIM
 
 - HTTP Method: `GET`
 - Endpoint: `/esim/{iccid}/device`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| iccid | str | ✅ | Get device info from an installed eSIM |
+
+| Name  | Type | Required | Description                            |
+| :---- | :--- | :------: | :------------------------------------- |
+| iccid | str  |    ✅    | Get device info from an installed eSIM |
 
 **Return Type**
 
 `GetEsimDeviceOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -366,17 +385,18 @@
 
 Get history from an eSIM
 
 - HTTP Method: `GET`
 - Endpoint: `/esim/{iccid}/history`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| iccid | str | ✅ | Get history from an eSIM |
+
+| Name  | Type | Required | Description              |
+| :---- | :--- | :------: | :----------------------- |
+| iccid | str  |    ✅    | Get history from an eSIM |
 
 **Return Type**
 
 `GetEsimHistoryOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -396,17 +416,18 @@
 
 Get MAC from eSIM
 
 - HTTP Method: `GET`
 - Endpoint: `/esim/{iccid}/mac`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| iccid | str | ✅ | Get MAC from eSIM |
+
+| Name  | Type | Required | Description       |
+| :---- | :--- | :------: | :---------------- |
+| iccid | str  |    ✅    | Get MAC from eSIM |
 
 **Return Type**
 
 `GetEsimMacOkResponse`
 
 **Example Usage Code Snippet**
```

### Comparing `celitech_sdk-1.1.55/src/celitech/hooks/hook.py` & `celitech_sdk-1.1.56/src/celitech/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/models/__init__.py` & `celitech_sdk-1.1.56/src/celitech/models/__init__.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/models/base.py` & `celitech_sdk-1.1.56/src/celitech/models/base.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/models/create_purchase_ok_response.py` & `celitech_sdk-1.1.56/src/celitech/models/create_purchase_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/models/create_purchase_request.py` & `celitech_sdk-1.1.56/src/celitech/models/create_purchase_request.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/models/edit_purchase_ok_response.py` & `celitech_sdk-1.1.56/src/celitech/models/edit_purchase_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/models/edit_purchase_request.py` & `celitech_sdk-1.1.56/src/celitech/models/edit_purchase_request.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/models/get_esim_device_ok_response.py` & `celitech_sdk-1.1.56/src/celitech/models/get_esim_device_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/models/get_esim_history_ok_response.py` & `celitech_sdk-1.1.56/src/celitech/models/get_esim_history_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/models/get_esim_mac_ok_response.py` & `celitech_sdk-1.1.56/src/celitech/models/get_esim_mac_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/models/get_esim_ok_response.py` & `celitech_sdk-1.1.56/src/celitech/models/get_esim_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/models/get_purchase_consumption_ok_response.py` & `celitech_sdk-1.1.56/src/celitech/models/get_purchase_consumption_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/models/list_destinations_ok_response.py` & `celitech_sdk-1.1.56/src/celitech/models/list_destinations_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/models/list_packages_ok_response.py` & `celitech_sdk-1.1.56/src/celitech/models/list_packages_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/models/list_purchases_ok_response.py` & `celitech_sdk-1.1.56/src/celitech/models/list_purchases_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/models/top_up_esim_ok_response.py` & `celitech_sdk-1.1.56/src/celitech/models/top_up_esim_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/models/top_up_esim_request.py` & `celitech_sdk-1.1.56/src/celitech/models/top_up_esim_request.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/models/utils/cast_models.py` & `celitech_sdk-1.1.56/src/celitech/models/utils/cast_models.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/models/utils/json_map.py` & `celitech_sdk-1.1.56/src/celitech/models/utils/json_map.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/net/request_chain/handlers/base_handler.py` & `celitech_sdk-1.1.56/src/celitech/net/request_chain/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/net/request_chain/handlers/hook_handler.py` & `celitech_sdk-1.1.56/src/celitech/net/request_chain/handlers/hook_handler.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/net/request_chain/handlers/http_handler.py` & `celitech_sdk-1.1.56/src/celitech/net/request_chain/handlers/http_handler.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/net/request_chain/handlers/retry_handler.py` & `celitech_sdk-1.1.56/src/celitech/net/request_chain/handlers/retry_handler.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/net/request_chain/request_chain.py` & `celitech_sdk-1.1.56/src/celitech/net/request_chain/request_chain.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/net/transport/request.py` & `celitech_sdk-1.1.56/src/celitech/net/transport/request.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/net/transport/request_error.py` & `celitech_sdk-1.1.56/src/celitech/net/transport/request_error.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/net/transport/response.py` & `celitech_sdk-1.1.56/src/celitech/net/transport/response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/net/transport/serializer.py` & `celitech_sdk-1.1.56/src/celitech/net/transport/serializer.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/net/transport/utils.py` & `celitech_sdk-1.1.56/src/celitech/net/transport/utils.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/sdk.py` & `celitech_sdk-1.1.56/src/celitech/sdk.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/services/destinations.py` & `celitech_sdk-1.1.56/src/celitech/services/destinations.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/services/e_sim.py` & `celitech_sdk-1.1.56/src/celitech/services/e_sim.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/services/packages.py` & `celitech_sdk-1.1.56/src/celitech/services/packages.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/services/purchases.py` & `celitech_sdk-1.1.56/src/celitech/services/purchases.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/services/utils/base_service.py` & `celitech_sdk-1.1.56/src/celitech/services/utils/base_service.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/services/utils/default_headers.py` & `celitech_sdk-1.1.56/src/celitech/services/utils/default_headers.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech/services/utils/validator.py` & `celitech_sdk-1.1.56/src/celitech/services/utils/validator.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.55/src/celitech_sdk.egg-info/PKG-INFO` & `celitech_sdk-1.1.56/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,13 @@
-Metadata-Version: 2.1
-Name: celitech-sdk
-Version: 1.1.55
-Summary: Welcome to the CELITECH API documentation!  Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/) 
-License: MIT
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.31.0
-
-# Celitech Python SDK 1.1.55
+# Celitech Python SDK 1.1.56
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.1.55
+- SDK version: 1.1.56
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
@@ -63,16 +53,17 @@
 
 Name of the destinations
 
 - HTTP Method: `GET`
 - Endpoint: `/destinations`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
+
+| Name | Type | Required | Description |
+| :--- | :--- | :------: | :---------- |
 
 **Return Type**
 
 `ListDestinationsOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -100,24 +91,25 @@
 
 List of available packages
 
 - HTTP Method: `GET`
 - Endpoint: `/packages`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| destination | str | ❌ | List of available packages |
-| start_date | str | ❌ | List of available packages |
-| end_date | str | ❌ | List of available packages |
-| after_cursor | str | ❌ | List of available packages |
-| limit | float | ❌ | List of available packages |
-| start_time | int | ❌ | List of available packages |
-| end_time | int | ❌ | List of available packages |
-| duration | float | ❌ | List of available packages |
+
+| Name         | Type  | Required | Description                |
+| :----------- | :---- | :------: | :------------------------- |
+| destination  | str   |    ❌    | List of available packages |
+| start_date   | str   |    ❌    | List of available packages |
+| end_date     | str   |    ❌    | List of available packages |
+| after_cursor | str   |    ❌    | List of available packages |
+| limit        | float |    ❌    | List of available packages |
+| start_time   | int   |    ❌    | List of available packages |
+| end_time     | int   |    ❌    | List of available packages |
+| duration     | float |    ❌    | List of available packages |
 
 **Return Type**
 
 `ListPackagesOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -149,23 +141,24 @@
 
 This endpoint can be used to list all the successful purchases made between a given interval.
 
 - HTTP Method: `GET`
 - Endpoint: `/purchases`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| iccid | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
-| after_date | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
-| before_date | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
-| after_cursor | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
-| limit | float | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
-| after | float | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
-| before | float | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
+
+| Name         | Type  | Required | Description                                                                                   |
+| :----------- | :---- | :------: | :-------------------------------------------------------------------------------------------- |
+| iccid        | str   |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
+| after_date   | str   |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
+| before_date  | str   |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
+| after_cursor | str   |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
+| limit        | float |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
+| after        | float |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
+| before       | float |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
 
 **Return Type**
 
 `ListPurchasesOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -185,17 +178,18 @@
 
 This endpoint is used to purchase a new eSIM by providing the package details.
 
 - HTTP Method: `POST`
 - Endpoint: `/purchases`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| request_body | CreatePurchaseRequest | ❌ | The request body. |
+
+| Name         | Type                  | Required | Description       |
+| :----------- | :-------------------- | :------: | :---------------- |
+| request_body | CreatePurchaseRequest |    ❌    | The request body. |
 
 **Return Type**
 
 `CreatePurchaseOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -215,17 +209,18 @@
 
 This endpoint is used to top-up an eSIM with the previously associated destination by providing an existing ICCID and the package details. The top-up is not feasible for eSIMs in "DELETED" or "ERROR" state.
 
 - HTTP Method: `POST`
 - Endpoint: `/purchases/topup`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| request_body | TopUpEsimRequest | ❌ | The request body. |
+
+| Name         | Type             | Required | Description       |
+| :----------- | :--------------- | :------: | :---------------- |
+| request_body | TopUpEsimRequest |    ❌    | The request body. |
 
 **Return Type**
 
 `TopUpEsimOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -245,17 +240,18 @@
 
 This endpoint allows you to modify the dates of an existing package with a future activation start time. Editing can only be performed for packages that have not been activated, and it cannot change the package size. The modification must not change the package duration category to ensure pricing consistency.
 
 - HTTP Method: `POST`
 - Endpoint: `/purchases/edit`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| request_body | EditPurchaseRequest | ❌ | The request body. |
+
+| Name         | Type                | Required | Description       |
+| :----------- | :------------------ | :------: | :---------------- |
+| request_body | EditPurchaseRequest |    ❌    | The request body. |
 
 **Return Type**
 
 `EditPurchaseOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -275,17 +271,18 @@
 
 This endpoint can be called for consumption notifications (e.g. every 1 hour or when the user clicks a button). It returns the data balance (consumption) of purchased packages.
 
 - HTTP Method: `GET`
 - Endpoint: `/purchases/{purchaseId}/consumption`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| purchase_id | str | ✅ | This endpoint can be called for consumption notifications (e.g. every 1 hour or when the user clicks a button). It returns the data balance (consumption) of purchased packages. |
+
+| Name        | Type | Required | Description                                                                                                                                                                      |
+| :---------- | :--- | :------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| purchase_id | str  |    ✅    | This endpoint can be called for consumption notifications (e.g. every 1 hour or when the user clicks a button). It returns the data balance (consumption) of purchased packages. |
 
 **Return Type**
 
 `GetPurchaseConsumptionOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -316,17 +313,18 @@
 
 Get status from eSIM
 
 - HTTP Method: `GET`
 - Endpoint: `/esim`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| iccid | str | ✅ | Get status from eSIM |
+
+| Name  | Type | Required | Description          |
+| :---- | :--- | :------: | :------------------- |
+| iccid | str  |    ✅    | Get status from eSIM |
 
 **Return Type**
 
 `GetEsimOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -346,17 +344,18 @@
 
 Get device info from an installed eSIM
 
 - HTTP Method: `GET`
 - Endpoint: `/esim/{iccid}/device`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| iccid | str | ✅ | Get device info from an installed eSIM |
+
+| Name  | Type | Required | Description                            |
+| :---- | :--- | :------: | :------------------------------------- |
+| iccid | str  |    ✅    | Get device info from an installed eSIM |
 
 **Return Type**
 
 `GetEsimDeviceOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -376,17 +375,18 @@
 
 Get history from an eSIM
 
 - HTTP Method: `GET`
 - Endpoint: `/esim/{iccid}/history`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| iccid | str | ✅ | Get history from an eSIM |
+
+| Name  | Type | Required | Description              |
+| :---- | :--- | :------: | :----------------------- |
+| iccid | str  |    ✅    | Get history from an eSIM |
 
 **Return Type**
 
 `GetEsimHistoryOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -406,17 +406,18 @@
 
 Get MAC from eSIM
 
 - HTTP Method: `GET`
 - Endpoint: `/esim/{iccid}/mac`
 
 **Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| iccid | str | ✅ | Get MAC from eSIM |
+
+| Name  | Type | Required | Description       |
+| :---- | :--- | :------: | :---------------- |
+| iccid | str  |    ✅    | Get MAC from eSIM |
 
 **Return Type**
 
 `GetEsimMacOkResponse`
 
 **Example Usage Code Snippet**
```

### Comparing `celitech_sdk-1.1.55/src/celitech_sdk.egg-info/SOURCES.txt` & `celitech_sdk-1.1.56/src/celitech_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

