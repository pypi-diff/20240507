# Comparing `tmp/google-maps-fleetengine-delivery-0.1.7.tar.gz` & `tmp/google-maps-fleetengine-delivery-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-maps-fleetengine-delivery-0.1.7.tar", last modified: Tue Mar  5 19:01:25 2024, max compression
+gzip compressed data, was "google-maps-fleetengine-delivery-0.1.8.tar", last modified: Tue May  7 20:43:59 2024, max compression
```

## Comparing `google-maps-fleetengine-delivery-0.1.7.tar` & `google-maps-fleetengine-delivery-0.1.8.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:25.855020 google-maps-fleetengine-delivery-0.1.7/
--rw-rw-r--   0 root         (0)     1003    11358 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5839 2024-03-05 19:01:25.855020 google-maps-fleetengine-delivery-0.1.7/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4391 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:25.839019 google-maps-fleetengine-delivery-0.1.7/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:25.839019 google-maps-fleetengine-delivery-0.1.7/google/maps/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:25.843019 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery/
--rw-rw-r--   0 root         (0)     1003     2996 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:25.847020 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/
--rw-rw-r--   0 root         (0)     1003     2634 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     4838 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:25.847020 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:25.847020 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/services/delivery_service/
--rw-rw-r--   0 root         (0)     1003      773 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/services/delivery_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    75315 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/services/delivery_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    93141 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/services/delivery_service/client.py
--rw-rw-r--   0 root         (0)     1003    16072 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/services/delivery_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:25.851020 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/
--rw-rw-r--   0 root         (0)     1003     1414 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    14692 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    23901 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    24445 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    68054 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:25.851020 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/types/
--rw-rw-r--   0 root         (0)     1003     2320 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    16752 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/types/common.py
--rw-rw-r--   0 root         (0)     1003    25006 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/types/delivery_api.py
--rw-rw-r--   0 root         (0)     1003    17286 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/types/delivery_vehicles.py
--rw-rw-r--   0 root         (0)     1003     5374 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/types/header.py
--rw-rw-r--   0 root         (0)     1003     6215 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/types/task_tracking_info.py
--rw-rw-r--   0 root         (0)     1003    19744 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/types/tasks.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:25.851020 google-maps-fleetengine-delivery-0.1.7/google_maps_fleetengine_delivery.egg-info/
--rw-r--r--   0 root         (0)     1003     5839 2024-03-05 19:01:25.000000 google-maps-fleetengine-delivery-0.1.7/google_maps_fleetengine_delivery.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2065 2024-03-05 19:01:25.000000 google-maps-fleetengine-delivery-0.1.7/google_maps_fleetengine_delivery.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-05 19:01:25.000000 google-maps-fleetengine-delivery-0.1.7/google_maps_fleetengine_delivery.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-05 19:01:25.000000 google-maps-fleetengine-delivery-0.1.7/google_maps_fleetengine_delivery.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      338 2024-03-05 19:01:25.000000 google-maps-fleetengine-delivery-0.1.7/google_maps_fleetengine_delivery.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-03-05 19:01:25.000000 google-maps-fleetengine-delivery-0.1.7/google_maps_fleetengine_delivery.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-03-05 19:01:25.855020 google-maps-fleetengine-delivery-0.1.7/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3260 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:25.851020 google-maps-fleetengine-delivery-0.1.7/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:25.851020 google-maps-fleetengine-delivery-0.1.7/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:25.855020 google-maps-fleetengine-delivery-0.1.7/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:25.855020 google-maps-fleetengine-delivery-0.1.7/tests/unit/gapic/fleetengine_delivery_v1/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/tests/unit/gapic/fleetengine_delivery_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   324724 2024-03-05 18:46:03.000000 google-maps-fleetengine-delivery-0.1.7/tests/unit/gapic/fleetengine_delivery_v1/test_delivery_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.583009 google-maps-fleetengine-delivery-0.1.8/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5839 2024-05-07 20:43:59.583009 google-maps-fleetengine-delivery-0.1.8/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4391 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.571007 google-maps-fleetengine-delivery-0.1.8/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.571007 google-maps-fleetengine-delivery-0.1.8/google/maps/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.571007 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery/
+-rw-rw-r--   0 root         (0)     1003     2996 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.575008 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/
+-rw-rw-r--   0 root         (0)     1003     2634 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4838 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.575008 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.575008 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/
+-rw-rw-r--   0 root         (0)     1003      773 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    75315 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    93141 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/client.py
+-rw-rw-r--   0 root         (0)     1003    16072 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.575008 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1414 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14692 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    23901 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    24445 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    68054 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.579008 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2320 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16752 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/common.py
+-rw-rw-r--   0 root         (0)     1003    25036 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/delivery_api.py
+-rw-rw-r--   0 root         (0)     1003    17286 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/delivery_vehicles.py
+-rw-rw-r--   0 root         (0)     1003     5374 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/header.py
+-rw-rw-r--   0 root         (0)     1003     6215 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/task_tracking_info.py
+-rw-rw-r--   0 root         (0)     1003    19744 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/tasks.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.579008 google-maps-fleetengine-delivery-0.1.8/google_maps_fleetengine_delivery.egg-info/
+-rw-r--r--   0 root         (0)     1003     5839 2024-05-07 20:43:59.000000 google-maps-fleetengine-delivery-0.1.8/google_maps_fleetengine_delivery.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2065 2024-05-07 20:43:59.000000 google-maps-fleetengine-delivery-0.1.8/google_maps_fleetengine_delivery.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-07 20:43:59.000000 google-maps-fleetengine-delivery-0.1.8/google_maps_fleetengine_delivery.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-07 20:43:59.000000 google-maps-fleetengine-delivery-0.1.8/google_maps_fleetengine_delivery.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      338 2024-05-07 20:43:59.000000 google-maps-fleetengine-delivery-0.1.8/google_maps_fleetengine_delivery.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-05-07 20:43:59.000000 google-maps-fleetengine-delivery-0.1.8/google_maps_fleetengine_delivery.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-05-07 20:43:59.583009 google-maps-fleetengine-delivery-0.1.8/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3260 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.579008 google-maps-fleetengine-delivery-0.1.8/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.579008 google-maps-fleetengine-delivery-0.1.8/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.583009 google-maps-fleetengine-delivery-0.1.8/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.583009 google-maps-fleetengine-delivery-0.1.8/tests/unit/gapic/fleetengine_delivery_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/tests/unit/gapic/fleetengine_delivery_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   349414 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/tests/unit/gapic/fleetengine_delivery_v1/test_delivery_service.py
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/LICENSE` & `google-maps-fleetengine-delivery-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `google-maps-fleetengine-delivery-0.1.7/MANIFEST.in` & `google-maps-fleetengine-delivery-0.1.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-maps-fleetengine-delivery-0.1.7/PKG-INFO` & `google-maps-fleetengine-delivery-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-maps-fleetengine-delivery
-Version: 0.1.7
+Version: 0.1.8
 Summary: Google Maps Fleetengine Delivery API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-maps-fleetengine-delivery
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/README.rst` & `google-maps-fleetengine-delivery-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery/__init__.py` & `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery/gapic_version.py` & `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.7"  # {x-release-please-version}
+__version__ = "0.1.8"  # {x-release-please-version}
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/__init__.py` & `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/gapic_metadata.json` & `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/gapic_version.py` & `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.7"  # {x-release-please-version}
+__version__ = "0.1.8"  # {x-release-please-version}
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/services/__init__.py` & `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/services/delivery_service/__init__.py` & `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/services/delivery_service/async_client.py` & `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/services/delivery_service/client.py` & `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/services/delivery_service/pagers.py` & `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/pagers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/__init__.py` & `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/base.py` & `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/grpc.py` & `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/grpc_asyncio.py` & `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/rest.py` & `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/types/__init__.py` & `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/types/common.py` & `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/types/delivery_api.py` & `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/delivery_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -599,16 +599,16 @@
             ``ListTasks`` must match the call that provided the page
             token.
         filter (str):
             Optional. A filter query to apply when listing Tasks. See
             http://aip.dev/160 for examples of filter syntax. If you
             don't specify a value, or if you filter on an empty string,
             then all Tasks are returned. For information about the Task
-            properties that you can filter on, see `Task
-            list </maps/documentation/transportation-logistics/last-mile-fleet-solution/fleet-performance/fleet-engine/deliveries_api#list_tasks>`__.
+            properties that you can filter on, see `List
+            tasks <https://developers.google.com/maps/documentation/transportation-logistics/last-mile-fleet-solution/fleet-performance/fleet-engine/deliveries_api#list-tasks>`__.
     """
 
     header: mfd_header.DeliveryRequestHeader = proto.Field(
         proto.MESSAGE,
         number=1,
         message=mfd_header.DeliveryRequestHeader,
     )
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/types/delivery_vehicles.py` & `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/delivery_vehicles.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/types/header.py` & `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/header.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/types/task_tracking_info.py` & `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/task_tracking_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/google/maps/fleetengine_delivery_v1/types/tasks.py` & `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/google_maps_fleetengine_delivery.egg-info/PKG-INFO` & `google-maps-fleetengine-delivery-0.1.8/google_maps_fleetengine_delivery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-maps-fleetengine-delivery
-Version: 0.1.7
+Version: 0.1.8
 Summary: Google Maps Fleetengine Delivery API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-maps-fleetengine-delivery
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/google_maps_fleetengine_delivery.egg-info/SOURCES.txt` & `google-maps-fleetengine-delivery-0.1.8/google_maps_fleetengine_delivery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-maps-fleetengine-delivery-0.1.7/setup.py` & `google-maps-fleetengine-delivery-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/tests/__init__.py` & `google-maps-fleetengine-delivery-0.1.8/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/tests/unit/__init__.py` & `google-maps-fleetengine-delivery-0.1.8/tests/unit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/tests/unit/gapic/__init__.py` & `google-maps-fleetengine-delivery-0.1.8/tests/unit/gapic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/tests/unit/gapic/fleetengine_delivery_v1/__init__.py` & `google-maps-fleetengine-delivery-0.1.8/tests/unit/gapic/fleetengine_delivery_v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-delivery-0.1.7/tests/unit/gapic/fleetengine_delivery_v1/test_delivery_service.py` & `google-maps-fleetengine-delivery-0.1.8/tests/unit/gapic/fleetengine_delivery_v1/test_delivery_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -1182,15 +1182,16 @@
             type_=delivery_vehicles.DeliveryVehicle.DeliveryVehicleType.AUTO,
         )
         response = client.create_delivery_vehicle(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == delivery_api.CreateDeliveryVehicleRequest()
+        request = delivery_api.CreateDeliveryVehicleRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, delivery_vehicles.DeliveryVehicle)
     assert response.name == "name_value"
     assert (
         response.navigation_status == common.DeliveryVehicleNavigationStatus.NO_GUIDANCE
     )
@@ -1212,14 +1213,71 @@
     ) as call:
         client.create_delivery_vehicle()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.CreateDeliveryVehicleRequest()
 
 
+def test_create_delivery_vehicle_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = DeliveryServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = delivery_api.CreateDeliveryVehicleRequest(
+        parent="parent_value",
+        delivery_vehicle_id="delivery_vehicle_id_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.create_delivery_vehicle), "__call__"
+    ) as call:
+        client.create_delivery_vehicle(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == delivery_api.CreateDeliveryVehicleRequest(
+            parent="parent_value",
+            delivery_vehicle_id="delivery_vehicle_id_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_create_delivery_vehicle_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = DeliveryServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.create_delivery_vehicle), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            delivery_vehicles.DeliveryVehicle(
+                name="name_value",
+                navigation_status=common.DeliveryVehicleNavigationStatus.NO_GUIDANCE,
+                current_route_segment=b"current_route_segment_blob",
+                type_=delivery_vehicles.DeliveryVehicle.DeliveryVehicleType.AUTO,
+            )
+        )
+        response = await client.create_delivery_vehicle()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == delivery_api.CreateDeliveryVehicleRequest()
+
+
 @pytest.mark.asyncio
 async def test_create_delivery_vehicle_async(
     transport: str = "grpc_asyncio",
     request_type=delivery_api.CreateDeliveryVehicleRequest,
 ):
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1244,15 +1302,16 @@
             )
         )
         response = await client.create_delivery_vehicle(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == delivery_api.CreateDeliveryVehicleRequest()
+        request = delivery_api.CreateDeliveryVehicleRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, delivery_vehicles.DeliveryVehicle)
     assert response.name == "name_value"
     assert (
         response.navigation_status == common.DeliveryVehicleNavigationStatus.NO_GUIDANCE
     )
@@ -1428,15 +1487,16 @@
             type_=delivery_vehicles.DeliveryVehicle.DeliveryVehicleType.AUTO,
         )
         response = client.get_delivery_vehicle(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == delivery_api.GetDeliveryVehicleRequest()
+        request = delivery_api.GetDeliveryVehicleRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, delivery_vehicles.DeliveryVehicle)
     assert response.name == "name_value"
     assert (
         response.navigation_status == common.DeliveryVehicleNavigationStatus.NO_GUIDANCE
     )
@@ -1458,14 +1518,69 @@
     ) as call:
         client.get_delivery_vehicle()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.GetDeliveryVehicleRequest()
 
 
+def test_get_delivery_vehicle_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = DeliveryServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = delivery_api.GetDeliveryVehicleRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_delivery_vehicle), "__call__"
+    ) as call:
+        client.get_delivery_vehicle(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == delivery_api.GetDeliveryVehicleRequest(
+            name="name_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_get_delivery_vehicle_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = DeliveryServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_delivery_vehicle), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            delivery_vehicles.DeliveryVehicle(
+                name="name_value",
+                navigation_status=common.DeliveryVehicleNavigationStatus.NO_GUIDANCE,
+                current_route_segment=b"current_route_segment_blob",
+                type_=delivery_vehicles.DeliveryVehicle.DeliveryVehicleType.AUTO,
+            )
+        )
+        response = await client.get_delivery_vehicle()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == delivery_api.GetDeliveryVehicleRequest()
+
+
 @pytest.mark.asyncio
 async def test_get_delivery_vehicle_async(
     transport: str = "grpc_asyncio", request_type=delivery_api.GetDeliveryVehicleRequest
 ):
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1489,15 +1604,16 @@
             )
         )
         response = await client.get_delivery_vehicle(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == delivery_api.GetDeliveryVehicleRequest()
+        request = delivery_api.GetDeliveryVehicleRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, delivery_vehicles.DeliveryVehicle)
     assert response.name == "name_value"
     assert (
         response.navigation_status == common.DeliveryVehicleNavigationStatus.NO_GUIDANCE
     )
@@ -1651,15 +1767,16 @@
             type_=delivery_vehicles.DeliveryVehicle.DeliveryVehicleType.AUTO,
         )
         response = client.update_delivery_vehicle(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == delivery_api.UpdateDeliveryVehicleRequest()
+        request = delivery_api.UpdateDeliveryVehicleRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, delivery_vehicles.DeliveryVehicle)
     assert response.name == "name_value"
     assert (
         response.navigation_status == common.DeliveryVehicleNavigationStatus.NO_GUIDANCE
     )
@@ -1681,14 +1798,65 @@
     ) as call:
         client.update_delivery_vehicle()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.UpdateDeliveryVehicleRequest()
 
 
+def test_update_delivery_vehicle_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = DeliveryServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = delivery_api.UpdateDeliveryVehicleRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_delivery_vehicle), "__call__"
+    ) as call:
+        client.update_delivery_vehicle(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == delivery_api.UpdateDeliveryVehicleRequest()
+
+
+@pytest.mark.asyncio
+async def test_update_delivery_vehicle_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = DeliveryServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_delivery_vehicle), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            delivery_vehicles.DeliveryVehicle(
+                name="name_value",
+                navigation_status=common.DeliveryVehicleNavigationStatus.NO_GUIDANCE,
+                current_route_segment=b"current_route_segment_blob",
+                type_=delivery_vehicles.DeliveryVehicle.DeliveryVehicleType.AUTO,
+            )
+        )
+        response = await client.update_delivery_vehicle()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == delivery_api.UpdateDeliveryVehicleRequest()
+
+
 @pytest.mark.asyncio
 async def test_update_delivery_vehicle_async(
     transport: str = "grpc_asyncio",
     request_type=delivery_api.UpdateDeliveryVehicleRequest,
 ):
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1713,15 +1881,16 @@
             )
         )
         response = await client.update_delivery_vehicle(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == delivery_api.UpdateDeliveryVehicleRequest()
+        request = delivery_api.UpdateDeliveryVehicleRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, delivery_vehicles.DeliveryVehicle)
     assert response.name == "name_value"
     assert (
         response.navigation_status == common.DeliveryVehicleNavigationStatus.NO_GUIDANCE
     )
@@ -1882,15 +2051,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = delivery_api.BatchCreateTasksResponse()
         response = client.batch_create_tasks(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == delivery_api.BatchCreateTasksRequest()
+        request = delivery_api.BatchCreateTasksRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, delivery_api.BatchCreateTasksResponse)
 
 
 def test_batch_create_tasks_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
@@ -1906,14 +2076,64 @@
     ) as call:
         client.batch_create_tasks()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.BatchCreateTasksRequest()
 
 
+def test_batch_create_tasks_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = DeliveryServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = delivery_api.BatchCreateTasksRequest(
+        parent="parent_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.batch_create_tasks), "__call__"
+    ) as call:
+        client.batch_create_tasks(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == delivery_api.BatchCreateTasksRequest(
+            parent="parent_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_batch_create_tasks_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = DeliveryServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.batch_create_tasks), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            delivery_api.BatchCreateTasksResponse()
+        )
+        response = await client.batch_create_tasks()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == delivery_api.BatchCreateTasksRequest()
+
+
 @pytest.mark.asyncio
 async def test_batch_create_tasks_async(
     transport: str = "grpc_asyncio", request_type=delivery_api.BatchCreateTasksRequest
 ):
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1932,15 +2152,16 @@
             delivery_api.BatchCreateTasksResponse()
         )
         response = await client.batch_create_tasks(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == delivery_api.BatchCreateTasksRequest()
+        request = delivery_api.BatchCreateTasksRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, delivery_api.BatchCreateTasksResponse)
 
 
 @pytest.mark.asyncio
 async def test_batch_create_tasks_async_from_dict():
@@ -2003,15 +2224,16 @@
             delivery_vehicle_id="delivery_vehicle_id_value",
         )
         response = client.create_task(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == delivery_api.CreateTaskRequest()
+        request = delivery_api.CreateTaskRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, tasks.Task)
     assert response.name == "name_value"
     assert response.type_ == tasks.Task.Type.PICKUP
     assert response.state == tasks.Task.State.OPEN
     assert response.task_outcome == tasks.Task.TaskOutcome.SUCCEEDED
@@ -2035,14 +2257,70 @@
     with mock.patch.object(type(client.transport.create_task), "__call__") as call:
         client.create_task()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.CreateTaskRequest()
 
 
+def test_create_task_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = DeliveryServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = delivery_api.CreateTaskRequest(
+        parent="parent_value",
+        task_id="task_id_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.create_task), "__call__") as call:
+        client.create_task(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == delivery_api.CreateTaskRequest(
+            parent="parent_value",
+            task_id="task_id_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_create_task_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = DeliveryServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.create_task), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            tasks.Task(
+                name="name_value",
+                type_=tasks.Task.Type.PICKUP,
+                state=tasks.Task.State.OPEN,
+                task_outcome=tasks.Task.TaskOutcome.SUCCEEDED,
+                task_outcome_location_source=tasks.Task.TaskOutcomeLocationSource.PROVIDER,
+                tracking_id="tracking_id_value",
+                delivery_vehicle_id="delivery_vehicle_id_value",
+            )
+        )
+        response = await client.create_task()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == delivery_api.CreateTaskRequest()
+
+
 @pytest.mark.asyncio
 async def test_create_task_async(
     transport: str = "grpc_asyncio", request_type=delivery_api.CreateTaskRequest
 ):
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -2067,15 +2345,16 @@
             )
         )
         response = await client.create_task(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == delivery_api.CreateTaskRequest()
+        request = delivery_api.CreateTaskRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, tasks.Task)
     assert response.name == "name_value"
     assert response.type_ == tasks.Task.Type.PICKUP
     assert response.state == tasks.Task.State.OPEN
     assert response.task_outcome == tasks.Task.TaskOutcome.SUCCEEDED
@@ -2246,15 +2525,16 @@
             delivery_vehicle_id="delivery_vehicle_id_value",
         )
         response = client.get_task(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == delivery_api.GetTaskRequest()
+        request = delivery_api.GetTaskRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, tasks.Task)
     assert response.name == "name_value"
     assert response.type_ == tasks.Task.Type.PICKUP
     assert response.state == tasks.Task.State.OPEN
     assert response.task_outcome == tasks.Task.TaskOutcome.SUCCEEDED
@@ -2278,14 +2558,68 @@
     with mock.patch.object(type(client.transport.get_task), "__call__") as call:
         client.get_task()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.GetTaskRequest()
 
 
+def test_get_task_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = DeliveryServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = delivery_api.GetTaskRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_task), "__call__") as call:
+        client.get_task(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == delivery_api.GetTaskRequest(
+            name="name_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_get_task_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = DeliveryServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_task), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            tasks.Task(
+                name="name_value",
+                type_=tasks.Task.Type.PICKUP,
+                state=tasks.Task.State.OPEN,
+                task_outcome=tasks.Task.TaskOutcome.SUCCEEDED,
+                task_outcome_location_source=tasks.Task.TaskOutcomeLocationSource.PROVIDER,
+                tracking_id="tracking_id_value",
+                delivery_vehicle_id="delivery_vehicle_id_value",
+            )
+        )
+        response = await client.get_task()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == delivery_api.GetTaskRequest()
+
+
 @pytest.mark.asyncio
 async def test_get_task_async(
     transport: str = "grpc_asyncio", request_type=delivery_api.GetTaskRequest
 ):
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -2310,15 +2644,16 @@
             )
         )
         response = await client.get_task(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == delivery_api.GetTaskRequest()
+        request = delivery_api.GetTaskRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, tasks.Task)
     assert response.name == "name_value"
     assert response.type_ == tasks.Task.Type.PICKUP
     assert response.state == tasks.Task.State.OPEN
     assert response.task_outcome == tasks.Task.TaskOutcome.SUCCEEDED
@@ -2463,15 +2798,16 @@
             next_page_token="next_page_token_value",
         )
         response = client.search_tasks(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == delivery_api.SearchTasksRequest()
+        request = delivery_api.SearchTasksRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.SearchTasksPager)
     assert response.next_page_token == "next_page_token_value"
 
 
 def test_search_tasks_empty_call():
@@ -2486,14 +2822,66 @@
     with mock.patch.object(type(client.transport.search_tasks), "__call__") as call:
         client.search_tasks()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.SearchTasksRequest()
 
 
+def test_search_tasks_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = DeliveryServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = delivery_api.SearchTasksRequest(
+        parent="parent_value",
+        tracking_id="tracking_id_value",
+        page_token="page_token_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.search_tasks), "__call__") as call:
+        client.search_tasks(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == delivery_api.SearchTasksRequest(
+            parent="parent_value",
+            tracking_id="tracking_id_value",
+            page_token="page_token_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_search_tasks_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = DeliveryServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.search_tasks), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            delivery_api.SearchTasksResponse(
+                next_page_token="next_page_token_value",
+            )
+        )
+        response = await client.search_tasks()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == delivery_api.SearchTasksRequest()
+
+
 @pytest.mark.asyncio
 async def test_search_tasks_async(
     transport: str = "grpc_asyncio", request_type=delivery_api.SearchTasksRequest
 ):
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -2512,15 +2900,16 @@
             )
         )
         response = await client.search_tasks(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == delivery_api.SearchTasksRequest()
+        request = delivery_api.SearchTasksRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.SearchTasksAsyncPager)
     assert response.next_page_token == "next_page_token_value"
 
 
 @pytest.mark.asyncio
@@ -2851,15 +3240,16 @@
             delivery_vehicle_id="delivery_vehicle_id_value",
         )
         response = client.update_task(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == delivery_api.UpdateTaskRequest()
+        request = delivery_api.UpdateTaskRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, tasks.Task)
     assert response.name == "name_value"
     assert response.type_ == tasks.Task.Type.PICKUP
     assert response.state == tasks.Task.State.OPEN
     assert response.task_outcome == tasks.Task.TaskOutcome.SUCCEEDED
@@ -2883,14 +3273,64 @@
     with mock.patch.object(type(client.transport.update_task), "__call__") as call:
         client.update_task()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.UpdateTaskRequest()
 
 
+def test_update_task_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = DeliveryServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = delivery_api.UpdateTaskRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.update_task), "__call__") as call:
+        client.update_task(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == delivery_api.UpdateTaskRequest()
+
+
+@pytest.mark.asyncio
+async def test_update_task_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = DeliveryServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.update_task), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            tasks.Task(
+                name="name_value",
+                type_=tasks.Task.Type.PICKUP,
+                state=tasks.Task.State.OPEN,
+                task_outcome=tasks.Task.TaskOutcome.SUCCEEDED,
+                task_outcome_location_source=tasks.Task.TaskOutcomeLocationSource.PROVIDER,
+                tracking_id="tracking_id_value",
+                delivery_vehicle_id="delivery_vehicle_id_value",
+            )
+        )
+        response = await client.update_task()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == delivery_api.UpdateTaskRequest()
+
+
 @pytest.mark.asyncio
 async def test_update_task_async(
     transport: str = "grpc_asyncio", request_type=delivery_api.UpdateTaskRequest
 ):
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -2915,15 +3355,16 @@
             )
         )
         response = await client.update_task(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == delivery_api.UpdateTaskRequest()
+        request = delivery_api.UpdateTaskRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, tasks.Task)
     assert response.name == "name_value"
     assert response.type_ == tasks.Task.Type.PICKUP
     assert response.state == tasks.Task.State.OPEN
     assert response.task_outcome == tasks.Task.TaskOutcome.SUCCEEDED
@@ -3079,15 +3520,16 @@
             total_size=1086,
         )
         response = client.list_tasks(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == delivery_api.ListTasksRequest()
+        request = delivery_api.ListTasksRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListTasksPager)
     assert response.next_page_token == "next_page_token_value"
     assert response.total_size == 1086
 
 
@@ -3103,14 +3545,67 @@
     with mock.patch.object(type(client.transport.list_tasks), "__call__") as call:
         client.list_tasks()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.ListTasksRequest()
 
 
+def test_list_tasks_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = DeliveryServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = delivery_api.ListTasksRequest(
+        parent="parent_value",
+        page_token="page_token_value",
+        filter="filter_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_tasks), "__call__") as call:
+        client.list_tasks(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == delivery_api.ListTasksRequest(
+            parent="parent_value",
+            page_token="page_token_value",
+            filter="filter_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_list_tasks_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = DeliveryServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_tasks), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            delivery_api.ListTasksResponse(
+                next_page_token="next_page_token_value",
+                total_size=1086,
+            )
+        )
+        response = await client.list_tasks()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == delivery_api.ListTasksRequest()
+
+
 @pytest.mark.asyncio
 async def test_list_tasks_async(
     transport: str = "grpc_asyncio", request_type=delivery_api.ListTasksRequest
 ):
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -3130,15 +3625,16 @@
             )
         )
         response = await client.list_tasks(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == delivery_api.ListTasksRequest()
+        request = delivery_api.ListTasksRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListTasksAsyncPager)
     assert response.next_page_token == "next_page_token_value"
     assert response.total_size == 1086
 
 
@@ -3469,15 +3965,16 @@
             task_outcome=tasks.Task.TaskOutcome.SUCCEEDED,
         )
         response = client.get_task_tracking_info(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == delivery_api.GetTaskTrackingInfoRequest()
+        request = delivery_api.GetTaskTrackingInfoRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, task_tracking_info.TaskTrackingInfo)
     assert response.name == "name_value"
     assert response.tracking_id == "tracking_id_value"
     assert response.state == tasks.Task.State.OPEN
     assert response.task_outcome == tasks.Task.TaskOutcome.SUCCEEDED
@@ -3497,14 +3994,69 @@
     ) as call:
         client.get_task_tracking_info()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.GetTaskTrackingInfoRequest()
 
 
+def test_get_task_tracking_info_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = DeliveryServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = delivery_api.GetTaskTrackingInfoRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_task_tracking_info), "__call__"
+    ) as call:
+        client.get_task_tracking_info(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == delivery_api.GetTaskTrackingInfoRequest(
+            name="name_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_get_task_tracking_info_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = DeliveryServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_task_tracking_info), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            task_tracking_info.TaskTrackingInfo(
+                name="name_value",
+                tracking_id="tracking_id_value",
+                state=tasks.Task.State.OPEN,
+                task_outcome=tasks.Task.TaskOutcome.SUCCEEDED,
+            )
+        )
+        response = await client.get_task_tracking_info()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == delivery_api.GetTaskTrackingInfoRequest()
+
+
 @pytest.mark.asyncio
 async def test_get_task_tracking_info_async(
     transport: str = "grpc_asyncio",
     request_type=delivery_api.GetTaskTrackingInfoRequest,
 ):
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -3529,15 +4081,16 @@
             )
         )
         response = await client.get_task_tracking_info(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == delivery_api.GetTaskTrackingInfoRequest()
+        request = delivery_api.GetTaskTrackingInfoRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, task_tracking_info.TaskTrackingInfo)
     assert response.name == "name_value"
     assert response.tracking_id == "tracking_id_value"
     assert response.state == tasks.Task.State.OPEN
     assert response.task_outcome == tasks.Task.TaskOutcome.SUCCEEDED
@@ -3687,15 +4240,16 @@
             total_size=1086,
         )
         response = client.list_delivery_vehicles(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == delivery_api.ListDeliveryVehiclesRequest()
+        request = delivery_api.ListDeliveryVehiclesRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListDeliveryVehiclesPager)
     assert response.next_page_token == "next_page_token_value"
     assert response.total_size == 1086
 
 
@@ -3713,14 +4267,71 @@
     ) as call:
         client.list_delivery_vehicles()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.ListDeliveryVehiclesRequest()
 
 
+def test_list_delivery_vehicles_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = DeliveryServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = delivery_api.ListDeliveryVehiclesRequest(
+        parent="parent_value",
+        page_token="page_token_value",
+        filter="filter_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_delivery_vehicles), "__call__"
+    ) as call:
+        client.list_delivery_vehicles(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == delivery_api.ListDeliveryVehiclesRequest(
+            parent="parent_value",
+            page_token="page_token_value",
+            filter="filter_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_list_delivery_vehicles_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = DeliveryServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_delivery_vehicles), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            delivery_api.ListDeliveryVehiclesResponse(
+                next_page_token="next_page_token_value",
+                total_size=1086,
+            )
+        )
+        response = await client.list_delivery_vehicles()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == delivery_api.ListDeliveryVehiclesRequest()
+
+
 @pytest.mark.asyncio
 async def test_list_delivery_vehicles_async(
     transport: str = "grpc_asyncio",
     request_type=delivery_api.ListDeliveryVehiclesRequest,
 ):
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -3743,15 +4354,16 @@
             )
         )
         response = await client.list_delivery_vehicles(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == delivery_api.ListDeliveryVehiclesRequest()
+        request = delivery_api.ListDeliveryVehiclesRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListDeliveryVehiclesAsyncPager)
     assert response.next_page_token == "next_page_token_value"
     assert response.total_size == 1086
```

