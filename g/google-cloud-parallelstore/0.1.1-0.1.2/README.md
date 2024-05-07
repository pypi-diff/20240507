# Comparing `tmp/google-cloud-parallelstore-0.1.1.tar.gz` & `tmp/google-cloud-parallelstore-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-parallelstore-0.1.1.tar", last modified: Tue Mar  5 18:57:21 2024, max compression
+gzip compressed data, was "google-cloud-parallelstore-0.1.2.tar", last modified: Tue May  7 20:43:51 2024, max compression
```

## Comparing `google-cloud-parallelstore-0.1.1.tar` & `google-cloud-parallelstore-0.1.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:57:21.245053 google-cloud-parallelstore-0.1.1/
--rw-rw-r--   0 root         (0)     1003    11358 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5258 2024-03-05 18:57:21.245053 google-cloud-parallelstore-0.1.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3876 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:57:21.233059 google-cloud-parallelstore-0.1.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:57:21.233059 google-cloud-parallelstore-0.1.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:57:21.237057 google-cloud-parallelstore-0.1.1/google/cloud/parallelstore/
--rw-rw-r--   0 root         (0)     1003     1488 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/google/cloud/parallelstore/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/google/cloud/parallelstore/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       87 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/google/cloud/parallelstore/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:57:21.241055 google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/
--rw-rw-r--   0 root         (0)     1003     1323 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003     2508 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       87 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:57:21.241055 google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:57:21.241055 google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/services/parallelstore/
--rw-rw-r--   0 root         (0)     1003      765 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/services/parallelstore/__init__.py
--rw-rw-r--   0 root         (0)     1003    51420 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/services/parallelstore/async_client.py
--rw-rw-r--   0 root         (0)     1003    69204 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/services/parallelstore/client.py
--rw-rw-r--   0 root         (0)     1003     5870 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/services/parallelstore/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:57:21.241055 google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/services/parallelstore/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/services/parallelstore/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9603 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/services/parallelstore/transports/base.py
--rw-rw-r--   0 root         (0)     1003    22868 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/services/parallelstore/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    23270 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/services/parallelstore/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    55877 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/services/parallelstore/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:57:21.241055 google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/types/
--rw-rw-r--   0 root         (0)     1003     1052 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    16402 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/types/parallelstore.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:57:21.245053 google-cloud-parallelstore-0.1.1/google_cloud_parallelstore.egg-info/
--rw-r--r--   0 root         (0)     1003     5258 2024-03-05 18:57:21.000000 google-cloud-parallelstore-0.1.1/google_cloud_parallelstore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1662 2024-03-05 18:57:21.000000 google-cloud-parallelstore-0.1.1/google_cloud_parallelstore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-05 18:57:21.000000 google-cloud-parallelstore-0.1.1/google_cloud_parallelstore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-05 18:57:21.000000 google-cloud-parallelstore-0.1.1/google_cloud_parallelstore.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      305 2024-03-05 18:57:21.000000 google-cloud-parallelstore-0.1.1/google_cloud_parallelstore.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-03-05 18:57:21.000000 google-cloud-parallelstore-0.1.1/google_cloud_parallelstore.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-03-05 18:57:21.245053 google-cloud-parallelstore-0.1.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3193 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:57:21.245053 google-cloud-parallelstore-0.1.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:57:21.245053 google-cloud-parallelstore-0.1.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:57:21.245053 google-cloud-parallelstore-0.1.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:57:21.245053 google-cloud-parallelstore-0.1.1/tests/unit/gapic/parallelstore_v1beta/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/tests/unit/gapic/parallelstore_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003   228431 2024-03-05 18:46:02.000000 google-cloud-parallelstore-0.1.1/tests/unit/gapic/parallelstore_v1beta/test_parallelstore.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.681561 google-cloud-parallelstore-0.1.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5258 2024-05-07 20:43:51.681561 google-cloud-parallelstore-0.1.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3876 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.669559 google-cloud-parallelstore-0.1.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.669559 google-cloud-parallelstore-0.1.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.673560 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore/
+-rw-rw-r--   0 root         (0)     1003     1932 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       87 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.673560 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/
+-rw-rw-r--   0 root         (0)     1003     1767 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3204 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       87 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.677561 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.677561 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/
+-rw-rw-r--   0 root         (0)     1003      765 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/__init__.py
+-rw-rw-r--   0 root         (0)     1003    60808 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/async_client.py
+-rw-rw-r--   0 root         (0)     1003    77457 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/client.py
+-rw-rw-r--   0 root         (0)     1003     5870 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.677561 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10443 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    25632 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    27713 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    66171 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.677561 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     1496 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    26281 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/types/parallelstore.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.681561 google-cloud-parallelstore-0.1.2/google_cloud_parallelstore.egg-info/
+-rw-r--r--   0 root         (0)     1003     5258 2024-05-07 20:43:51.000000 google-cloud-parallelstore-0.1.2/google_cloud_parallelstore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1662 2024-05-07 20:43:51.000000 google-cloud-parallelstore-0.1.2/google_cloud_parallelstore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-07 20:43:51.000000 google-cloud-parallelstore-0.1.2/google_cloud_parallelstore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-07 20:43:51.000000 google-cloud-parallelstore-0.1.2/google_cloud_parallelstore.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      305 2024-05-07 20:43:51.000000 google-cloud-parallelstore-0.1.2/google_cloud_parallelstore.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-05-07 20:43:51.000000 google-cloud-parallelstore-0.1.2/google_cloud_parallelstore.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-05-07 20:43:51.681561 google-cloud-parallelstore-0.1.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3193 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.681561 google-cloud-parallelstore-0.1.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.681561 google-cloud-parallelstore-0.1.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.681561 google-cloud-parallelstore-0.1.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.681561 google-cloud-parallelstore-0.1.2/tests/unit/gapic/parallelstore_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/tests/unit/gapic/parallelstore_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003   302813 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/tests/unit/gapic/parallelstore_v1beta/test_parallelstore.py
```

### Comparing `google-cloud-parallelstore-0.1.1/LICENSE` & `google-cloud-parallelstore-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-parallelstore-0.1.1/MANIFEST.in` & `google-cloud-parallelstore-0.1.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-parallelstore-0.1.1/PKG-INFO` & `google-cloud-parallelstore-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-parallelstore
-Version: 0.1.1
+Version: 0.1.2
 Summary: Google Cloud Parallelstore API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-parallelstore
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-parallelstore-0.1.1/README.rst` & `google-cloud-parallelstore-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-parallelstore-0.1.1/google/cloud/parallelstore/__init__.py` & `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore/__init__.py`

 * *Files 21% similar despite different names*

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
@@ -23,27 +23,45 @@
 )
 from google.cloud.parallelstore_v1beta.services.parallelstore.client import (
     ParallelstoreClient,
 )
 from google.cloud.parallelstore_v1beta.types.parallelstore import (
     CreateInstanceRequest,
     DeleteInstanceRequest,
+    ExportDataMetadata,
+    ExportDataRequest,
+    ExportDataResponse,
     GetInstanceRequest,
+    ImportDataMetadata,
+    ImportDataRequest,
+    ImportDataResponse,
     Instance,
     ListInstancesRequest,
     ListInstancesResponse,
     OperationMetadata,
+    TransferCounters,
+    TransferOperationMetadata,
+    TransferType,
     UpdateInstanceRequest,
 )
 
 __all__ = (
     "ParallelstoreClient",
     "ParallelstoreAsyncClient",
     "CreateInstanceRequest",
     "DeleteInstanceRequest",
+    "ExportDataMetadata",
+    "ExportDataRequest",
+    "ExportDataResponse",
     "GetInstanceRequest",
+    "ImportDataMetadata",
+    "ImportDataRequest",
+    "ImportDataResponse",
     "Instance",
     "ListInstancesRequest",
     "ListInstancesResponse",
     "OperationMetadata",
+    "TransferCounters",
+    "TransferOperationMetadata",
     "UpdateInstanceRequest",
+    "TransferType",
 )
```

### Comparing `google-cloud-parallelstore-0.1.1/google/cloud/parallelstore/gapic_version.py` & `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore/gapic_version.py`

 * *Files 1% similar despite different names*

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
-__version__ = "0.1.1"  # {x-release-please-version}
+__version__ = "0.1.2"  # {x-release-please-version}
```

### Comparing `google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/__init__.py` & `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/__init__.py`

 * *Files 24% similar despite different names*

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
@@ -18,27 +18,45 @@
 __version__ = package_version.__version__
 
 
 from .services.parallelstore import ParallelstoreAsyncClient, ParallelstoreClient
 from .types.parallelstore import (
     CreateInstanceRequest,
     DeleteInstanceRequest,
+    ExportDataMetadata,
+    ExportDataRequest,
+    ExportDataResponse,
     GetInstanceRequest,
+    ImportDataMetadata,
+    ImportDataRequest,
+    ImportDataResponse,
     Instance,
     ListInstancesRequest,
     ListInstancesResponse,
     OperationMetadata,
+    TransferCounters,
+    TransferOperationMetadata,
+    TransferType,
     UpdateInstanceRequest,
 )
 
 __all__ = (
     "ParallelstoreAsyncClient",
     "CreateInstanceRequest",
     "DeleteInstanceRequest",
+    "ExportDataMetadata",
+    "ExportDataRequest",
+    "ExportDataResponse",
     "GetInstanceRequest",
+    "ImportDataMetadata",
+    "ImportDataRequest",
+    "ImportDataResponse",
     "Instance",
     "ListInstancesRequest",
     "ListInstancesResponse",
     "OperationMetadata",
     "ParallelstoreClient",
+    "TransferCounters",
+    "TransferOperationMetadata",
+    "TransferType",
     "UpdateInstanceRequest",
 )
```

### Comparing `google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/gapic_metadata.json` & `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/gapic_metadata.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992559523809524%*

 * *Differences: {"'services'": "{'Parallelstore': {'clients': {'grpc': {'rpcs': {'ExportData': "*

 * *               "OrderedDict([('methods', ['export_data'])]), 'ImportData': "*

 * *               "OrderedDict([('methods', ['import_data'])])}}, 'grpc-async': {'rpcs': "*

 * *               "{'ExportData': OrderedDict([('methods', ['export_data'])]), 'ImportData': "*

 * *               "OrderedDict([('methods', ['import_data'])])}}, 'rest': {'rpcs': {'ExportData': "*

 * *               "OrderedDict([('methods', ['export_data'])]), 'ImportData': "*

 * * […]*

```diff
@@ -16,19 +16,29 @@
                             ]
                         },
                         "DeleteInstance": {
                             "methods": [
                                 "delete_instance"
                             ]
                         },
+                        "ExportData": {
+                            "methods": [
+                                "export_data"
+                            ]
+                        },
                         "GetInstance": {
                             "methods": [
                                 "get_instance"
                             ]
                         },
+                        "ImportData": {
+                            "methods": [
+                                "import_data"
+                            ]
+                        },
                         "ListInstances": {
                             "methods": [
                                 "list_instances"
                             ]
                         },
                         "UpdateInstance": {
                             "methods": [
@@ -46,19 +56,29 @@
                             ]
                         },
                         "DeleteInstance": {
                             "methods": [
                                 "delete_instance"
                             ]
                         },
+                        "ExportData": {
+                            "methods": [
+                                "export_data"
+                            ]
+                        },
                         "GetInstance": {
                             "methods": [
                                 "get_instance"
                             ]
                         },
+                        "ImportData": {
+                            "methods": [
+                                "import_data"
+                            ]
+                        },
                         "ListInstances": {
                             "methods": [
                                 "list_instances"
                             ]
                         },
                         "UpdateInstance": {
                             "methods": [
@@ -76,19 +96,29 @@
                             ]
                         },
                         "DeleteInstance": {
                             "methods": [
                                 "delete_instance"
                             ]
                         },
+                        "ExportData": {
+                            "methods": [
+                                "export_data"
+                            ]
+                        },
                         "GetInstance": {
                             "methods": [
                                 "get_instance"
                             ]
                         },
+                        "ImportData": {
+                            "methods": [
+                                "import_data"
+                            ]
+                        },
                         "ListInstances": {
                             "methods": [
                                 "list_instances"
                             ]
                         },
                         "UpdateInstance": {
                             "methods": [
```

### Comparing `google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/gapic_version.py` & `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/gapic_version.py`

 * *Files 1% similar despite different names*

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
-__version__ = "0.1.1"  # {x-release-please-version}
+__version__ = "0.1.2"  # {x-release-please-version}
```

### Comparing `google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/services/__init__.py` & `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/__init__.py`

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

### Comparing `google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/services/parallelstore/__init__.py` & `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/__init__.py`

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

### Comparing `google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/services/parallelstore/async_client.py` & `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/async_client.py`

 * *Files 12% similar despite different names*

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
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
 from typing import (
+    Callable,
     Dict,
     Mapping,
     MutableMapping,
     MutableSequence,
     Optional,
     Sequence,
     Tuple,
@@ -223,29 +224,33 @@
         type(ParallelstoreClient).get_transport_class, type(ParallelstoreClient)
     )
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, ParallelstoreTransport] = "grpc_asyncio",
+        transport: Optional[
+            Union[str, ParallelstoreTransport, Callable[..., ParallelstoreTransport]]
+        ] = "grpc_asyncio",
         client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the parallelstore async client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, ~.ParallelstoreTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,ParallelstoreTransport,Callable[..., ParallelstoreTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport to use.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the ParallelstoreTransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -351,37 +356,38 @@
                 Instances
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = parallelstore.ListInstancesRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, parallelstore.ListInstancesRequest):
+            request = parallelstore.ListInstancesRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.list_instances,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.list_instances
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -462,37 +468,38 @@
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.parallelstore_v1beta.types.Instance:
                 A Parallelstore instance.
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = parallelstore.GetInstanceRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, parallelstore.GetInstanceRequest):
+            request = parallelstore.GetInstanceRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.get_instance,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.get_instance
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -603,41 +610,42 @@
 
                 The result type for the operation will be
                 :class:`google.cloud.parallelstore_v1beta.types.Instance`
                 A Parallelstore instance.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, instance, instance_id])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = parallelstore.CreateInstanceRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, parallelstore.CreateInstanceRequest):
+            request = parallelstore.CreateInstanceRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
         if instance is not None:
             request.instance = instance
         if instance_id is not None:
             request.instance_id = instance_id
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.create_instance,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.create_instance
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -739,39 +747,40 @@
 
                 The result type for the operation will be
                 :class:`google.cloud.parallelstore_v1beta.types.Instance`
                 A Parallelstore instance.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([instance, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = parallelstore.UpdateInstanceRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, parallelstore.UpdateInstanceRequest):
+            request = parallelstore.UpdateInstanceRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if instance is not None:
             request.instance = instance
         if update_mask is not None:
             request.update_mask = update_mask
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.update_instance,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.update_instance
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata(
                 (("instance.name", request.instance.name),)
             ),
@@ -867,37 +876,38 @@
                          rpc Bar(google.protobuf.Empty) returns
                          (google.protobuf.Empty);
 
                       }
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = parallelstore.DeleteInstanceRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, parallelstore.DeleteInstanceRequest):
+            request = parallelstore.DeleteInstanceRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.delete_instance,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.delete_instance
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -919,14 +929,222 @@
             empty_pb2.Empty,
             metadata_type=parallelstore.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
+    async def import_data(
+        self,
+        request: Optional[Union[parallelstore.ImportDataRequest, dict]] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operation_async.AsyncOperation:
+        r"""ImportData copies data from Cloud Storage to
+        Parallelstore.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import parallelstore_v1beta
+
+            async def sample_import_data():
+                # Create a client
+                client = parallelstore_v1beta.ParallelstoreAsyncClient()
+
+                # Initialize request argument(s)
+                request = parallelstore_v1beta.ImportDataRequest(
+                    source_gcs_uri="source_gcs_uri_value",
+                    destination_path="destination_path_value",
+                    name="name_value",
+                )
+
+                # Make the request
+                operation = client.import_data(request=request)
+
+                print("Waiting for operation to complete...")
+
+                response = (await operation).result()
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.parallelstore_v1beta.types.ImportDataRequest, dict]]):
+                The request object. Message representing the request
+                importing data from parallelstore to
+                Cloud Storage.
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.api_core.operation_async.AsyncOperation:
+                An object representing a long-running operation.
+
+                The result type for the operation will be
+                :class:`google.cloud.parallelstore_v1beta.types.ImportDataResponse`
+                ImportDataResponse is the response returned from
+                ImportData rpc.
+
+        """
+        # Create or coerce a protobuf request object.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, parallelstore.ImportDataRequest):
+            request = parallelstore.ImportDataRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.import_data
+        ]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Validate the universe domain.
+        self._client._validate_universe_domain()
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Wrap the response in an operation future.
+        response = operation_async.from_gapic(
+            response,
+            self._client._transport.operations_client,
+            parallelstore.ImportDataResponse,
+            metadata_type=parallelstore.ImportDataMetadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def export_data(
+        self,
+        request: Optional[Union[parallelstore.ExportDataRequest, dict]] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operation_async.AsyncOperation:
+        r"""ExportData copies data from Parallelstore to Cloud
+        Storage
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import parallelstore_v1beta
+
+            async def sample_export_data():
+                # Create a client
+                client = parallelstore_v1beta.ParallelstoreAsyncClient()
+
+                # Initialize request argument(s)
+                request = parallelstore_v1beta.ExportDataRequest(
+                    source_path="source_path_value",
+                    destination_gcs_uri="destination_gcs_uri_value",
+                    name="name_value",
+                )
+
+                # Make the request
+                operation = client.export_data(request=request)
+
+                print("Waiting for operation to complete...")
+
+                response = (await operation).result()
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.parallelstore_v1beta.types.ExportDataRequest, dict]]):
+                The request object. Message representing the request
+                exporting data from Cloud Storage to
+                parallelstore.
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.api_core.operation_async.AsyncOperation:
+                An object representing a long-running operation.
+
+                The result type for the operation will be
+                :class:`google.cloud.parallelstore_v1beta.types.ExportDataResponse`
+                ExportDataResponse is the response returned from
+                ExportData rpc
+
+        """
+        # Create or coerce a protobuf request object.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, parallelstore.ExportDataRequest):
+            request = parallelstore.ExportDataRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.export_data
+        ]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Validate the universe domain.
+        self._client._validate_universe_domain()
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Wrap the response in an operation future.
+        response = operation_async.from_gapic(
+            response,
+            self._client._transport.operations_client,
+            parallelstore.ExportDataResponse,
+            metadata_type=parallelstore.ExportDataMetadata,
+        )
+
+        # Done; return the response.
+        return response
+
     async def list_operations(
         self,
         request: Optional[operations_pb2.ListOperationsRequest] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
```

### Comparing `google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/services/parallelstore/client.py` & `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/client.py`

 * *Files 6% similar despite different names*

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
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
 from typing import (
+    Callable,
     Dict,
     Mapping,
     MutableMapping,
     MutableSequence,
     Optional,
     Sequence,
     Tuple,
@@ -593,29 +594,33 @@
         """
         return self._universe_domain
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Optional[Union[str, ParallelstoreTransport]] = None,
+        transport: Optional[
+            Union[str, ParallelstoreTransport, Callable[..., ParallelstoreTransport]]
+        ] = None,
         client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the parallelstore client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, ParallelstoreTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,ParallelstoreTransport,Callable[..., ParallelstoreTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the ParallelstoreTransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -716,16 +721,23 @@
             if api_key_value and hasattr(
                 google.auth._default, "get_api_key_credentials"
             ):
                 credentials = google.auth._default.get_api_key_credentials(
                     api_key_value
                 )
 
-            Transport = type(self).get_transport_class(cast(str, transport))
-            self._transport = Transport(
+            transport_init: Union[
+                Type[ParallelstoreTransport], Callable[..., ParallelstoreTransport]
+            ] = (
+                type(self).get_transport_class(transport)
+                if isinstance(transport, str) or transport is None
+                else cast(Callable[..., ParallelstoreTransport], transport)
+            )
+            # initialize with the provided callable or the passed in class
+            self._transport = transport_init(
                 credentials=credentials,
                 credentials_file=self._client_options.credentials_file,
                 host=self._api_endpoint,
                 scopes=self._client_options.scopes,
                 client_cert_source_for_mtls=self._client_cert_source,
                 quota_project_id=self._client_options.quota_project_id,
                 client_info=client_info,
@@ -799,27 +811,25 @@
                 Instances
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a parallelstore.ListInstancesRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, parallelstore.ListInstancesRequest):
             request = parallelstore.ListInstancesRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if parent is not None:
                 request.parent = parent
 
@@ -910,27 +920,25 @@
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.parallelstore_v1beta.types.Instance:
                 A Parallelstore instance.
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a parallelstore.GetInstanceRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, parallelstore.GetInstanceRequest):
             request = parallelstore.GetInstanceRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
 
@@ -1051,27 +1059,25 @@
 
                 The result type for the operation will be
                 :class:`google.cloud.parallelstore_v1beta.types.Instance`
                 A Parallelstore instance.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, instance, instance_id])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a parallelstore.CreateInstanceRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, parallelstore.CreateInstanceRequest):
             request = parallelstore.CreateInstanceRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if parent is not None:
                 request.parent = parent
             if instance is not None:
@@ -1187,27 +1193,25 @@
 
                 The result type for the operation will be
                 :class:`google.cloud.parallelstore_v1beta.types.Instance`
                 A Parallelstore instance.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([instance, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a parallelstore.UpdateInstanceRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, parallelstore.UpdateInstanceRequest):
             request = parallelstore.UpdateInstanceRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if instance is not None:
                 request.instance = instance
             if update_mask is not None:
@@ -1315,27 +1319,25 @@
                          rpc Bar(google.protobuf.Empty) returns
                          (google.protobuf.Empty);
 
                       }
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a parallelstore.DeleteInstanceRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, parallelstore.DeleteInstanceRequest):
             request = parallelstore.DeleteInstanceRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
 
@@ -1367,14 +1369,218 @@
             empty_pb2.Empty,
             metadata_type=parallelstore.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
+    def import_data(
+        self,
+        request: Optional[Union[parallelstore.ImportDataRequest, dict]] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operation.Operation:
+        r"""ImportData copies data from Cloud Storage to
+        Parallelstore.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import parallelstore_v1beta
+
+            def sample_import_data():
+                # Create a client
+                client = parallelstore_v1beta.ParallelstoreClient()
+
+                # Initialize request argument(s)
+                request = parallelstore_v1beta.ImportDataRequest(
+                    source_gcs_uri="source_gcs_uri_value",
+                    destination_path="destination_path_value",
+                    name="name_value",
+                )
+
+                # Make the request
+                operation = client.import_data(request=request)
+
+                print("Waiting for operation to complete...")
+
+                response = operation.result()
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.parallelstore_v1beta.types.ImportDataRequest, dict]):
+                The request object. Message representing the request
+                importing data from parallelstore to
+                Cloud Storage.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.api_core.operation.Operation:
+                An object representing a long-running operation.
+
+                The result type for the operation will be
+                :class:`google.cloud.parallelstore_v1beta.types.ImportDataResponse`
+                ImportDataResponse is the response returned from
+                ImportData rpc.
+
+        """
+        # Create or coerce a protobuf request object.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, parallelstore.ImportDataRequest):
+            request = parallelstore.ImportDataRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.import_data]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Validate the universe domain.
+        self._validate_universe_domain()
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Wrap the response in an operation future.
+        response = operation.from_gapic(
+            response,
+            self._transport.operations_client,
+            parallelstore.ImportDataResponse,
+            metadata_type=parallelstore.ImportDataMetadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def export_data(
+        self,
+        request: Optional[Union[parallelstore.ExportDataRequest, dict]] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operation.Operation:
+        r"""ExportData copies data from Parallelstore to Cloud
+        Storage
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import parallelstore_v1beta
+
+            def sample_export_data():
+                # Create a client
+                client = parallelstore_v1beta.ParallelstoreClient()
+
+                # Initialize request argument(s)
+                request = parallelstore_v1beta.ExportDataRequest(
+                    source_path="source_path_value",
+                    destination_gcs_uri="destination_gcs_uri_value",
+                    name="name_value",
+                )
+
+                # Make the request
+                operation = client.export_data(request=request)
+
+                print("Waiting for operation to complete...")
+
+                response = operation.result()
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.parallelstore_v1beta.types.ExportDataRequest, dict]):
+                The request object. Message representing the request
+                exporting data from Cloud Storage to
+                parallelstore.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.api_core.operation.Operation:
+                An object representing a long-running operation.
+
+                The result type for the operation will be
+                :class:`google.cloud.parallelstore_v1beta.types.ExportDataResponse`
+                ExportDataResponse is the response returned from
+                ExportData rpc
+
+        """
+        # Create or coerce a protobuf request object.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, parallelstore.ExportDataRequest):
+            request = parallelstore.ExportDataRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.export_data]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Validate the universe domain.
+        self._validate_universe_domain()
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Wrap the response in an operation future.
+        response = operation.from_gapic(
+            response,
+            self._transport.operations_client,
+            parallelstore.ExportDataResponse,
+            metadata_type=parallelstore.ExportDataMetadata,
+        )
+
+        # Done; return the response.
+        return response
+
     def __enter__(self) -> "ParallelstoreClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
```

### Comparing `google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/services/parallelstore/pagers.py` & `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/pagers.py`

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

### Comparing `google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/services/parallelstore/transports/__init__.py` & `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/transports/__init__.py`

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

### Comparing `google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/services/parallelstore/transports/base.py` & `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/transports/base.py`

 * *Files 3% similar despite different names*

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
@@ -149,14 +149,24 @@
                 client_info=client_info,
             ),
             self.delete_instance: gapic_v1.method.wrap_method(
                 self.delete_instance,
                 default_timeout=None,
                 client_info=client_info,
             ),
+            self.import_data: gapic_v1.method.wrap_method(
+                self.import_data,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.export_data: gapic_v1.method.wrap_method(
+                self.export_data,
+                default_timeout=None,
+                client_info=client_info,
+            ),
         }
 
     def close(self):
         """Closes resources associated with the transport.
 
         .. warning::
              Only call this method if the transport is NOT shared
@@ -214,14 +224,32 @@
     ) -> Callable[
         [parallelstore.DeleteInstanceRequest],
         Union[operations_pb2.Operation, Awaitable[operations_pb2.Operation]],
     ]:
         raise NotImplementedError()
 
     @property
+    def import_data(
+        self,
+    ) -> Callable[
+        [parallelstore.ImportDataRequest],
+        Union[operations_pb2.Operation, Awaitable[operations_pb2.Operation]],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def export_data(
+        self,
+    ) -> Callable[
+        [parallelstore.ExportDataRequest],
+        Union[operations_pb2.Operation, Awaitable[operations_pb2.Operation]],
+    ]:
+        raise NotImplementedError()
+
+    @property
     def list_operations(
         self,
     ) -> Callable[
         [operations_pb2.ListOperationsRequest],
         Union[
             operations_pb2.ListOperationsResponse,
             Awaitable[operations_pb2.ListOperationsResponse],
```

### Comparing `google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/services/parallelstore/transports/grpc.py` & `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/transports/grpc.py`

 * *Files 7% similar despite different names*

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
@@ -67,15 +67,15 @@
     def __init__(
         self,
         *,
         host: str = "parallelstore.googleapis.com",
         credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: Optional[grpc.Channel] = None,
+        channel: Optional[Union[grpc.Channel, Callable[..., grpc.Channel]]] = None,
         api_mtls_endpoint: Optional[str] = None,
         client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
         client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
@@ -87,36 +87,39 @@
             host (Optional[str]):
                  The hostname to connect to (default: 'parallelstore.googleapis.com').
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             scopes (Optional(Sequence[str])): A list of scopes. This argument is
-                ignored if ``channel`` is provided.
-            channel (Optional[grpc.Channel]): A ``Channel`` instance through
-                which to make calls.
+                ignored if a ``channel`` instance is provided.
+            channel (Optional[Union[grpc.Channel, Callable[..., grpc.Channel]]]):
+                A ``Channel`` instance through which to make calls, or a Callable
+                that constructs and returns one. If set to None, ``self.create_channel``
+                is used to create the channel. If a Callable is given, it will be called
+                with the same arguments as used in ``self.create_channel``.
             api_mtls_endpoint (Optional[str]): Deprecated. The mutual TLS endpoint.
                 If provided, it overrides the ``host`` argument and tries to create
                 a mutual TLS channel with client SSL credentials from
                 ``client_cert_source`` or application default SSL credentials.
             client_cert_source (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 Deprecated. A callback to provide client SSL certificate bytes and
                 private key bytes, both in PEM format. It is ignored if
                 ``api_mtls_endpoint`` is None.
             ssl_channel_credentials (grpc.ChannelCredentials): SSL credentials
-                for the grpc channel. It is ignored if ``channel`` is provided.
+                for the grpc channel. It is ignored if a ``channel`` instance is provided.
             client_cert_source_for_mtls (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 A callback to provide client certificate bytes and private key bytes,
                 both in PEM format. It is used to configure a mutual TLS channel. It is
-                ignored if ``channel`` or ``ssl_channel_credentials`` is provided.
+                ignored if a ``channel`` instance or ``ssl_channel_credentials`` is provided.
             quota_project_id (Optional[str]): An optional project to use for billing
                 and quota.
             client_info (google.api_core.gapic_v1.client_info.ClientInfo):
                 The client info used to send a user-agent string along with
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
@@ -135,15 +138,15 @@
         self._operations_client: Optional[operations_v1.OperationsClient] = None
 
         if api_mtls_endpoint:
             warnings.warn("api_mtls_endpoint is deprecated", DeprecationWarning)
         if client_cert_source:
             warnings.warn("client_cert_source is deprecated", DeprecationWarning)
 
-        if channel:
+        if isinstance(channel, grpc.Channel):
             # Ignore credentials if a channel was passed.
             credentials = False
             # If a channel was explicitly provided, set it.
             self._grpc_channel = channel
             self._ssl_channel_credentials = None
 
         else:
@@ -176,15 +179,17 @@
             quota_project_id=quota_project_id,
             client_info=client_info,
             always_use_jwt_access=always_use_jwt_access,
             api_audience=api_audience,
         )
 
         if not self._grpc_channel:
-            self._grpc_channel = type(self).create_channel(
+            # initialize with the provided callable or the default channel
+            channel_init = channel or type(self).create_channel
+            self._grpc_channel = channel_init(
                 self._host,
                 # use the credentials which are saved
                 credentials=self._credentials,
                 # Set ``credentials_file`` to ``None`` here as
                 # the credentials that we saved earlier should be used.
                 credentials_file=None,
                 scopes=self._scopes,
@@ -394,14 +399,68 @@
             self._stubs["delete_instance"] = self.grpc_channel.unary_unary(
                 "/google.cloud.parallelstore.v1beta.Parallelstore/DeleteInstance",
                 request_serializer=parallelstore.DeleteInstanceRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["delete_instance"]
 
+    @property
+    def import_data(
+        self,
+    ) -> Callable[[parallelstore.ImportDataRequest], operations_pb2.Operation]:
+        r"""Return a callable for the import data method over gRPC.
+
+        ImportData copies data from Cloud Storage to
+        Parallelstore.
+
+        Returns:
+            Callable[[~.ImportDataRequest],
+                    ~.Operation]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "import_data" not in self._stubs:
+            self._stubs["import_data"] = self.grpc_channel.unary_unary(
+                "/google.cloud.parallelstore.v1beta.Parallelstore/ImportData",
+                request_serializer=parallelstore.ImportDataRequest.serialize,
+                response_deserializer=operations_pb2.Operation.FromString,
+            )
+        return self._stubs["import_data"]
+
+    @property
+    def export_data(
+        self,
+    ) -> Callable[[parallelstore.ExportDataRequest], operations_pb2.Operation]:
+        r"""Return a callable for the export data method over gRPC.
+
+        ExportData copies data from Parallelstore to Cloud
+        Storage
+
+        Returns:
+            Callable[[~.ExportDataRequest],
+                    ~.Operation]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "export_data" not in self._stubs:
+            self._stubs["export_data"] = self.grpc_channel.unary_unary(
+                "/google.cloud.parallelstore.v1beta.Parallelstore/ExportData",
+                request_serializer=parallelstore.ExportDataRequest.serialize,
+                response_deserializer=operations_pb2.Operation.FromString,
+            )
+        return self._stubs["export_data"]
+
     def close(self):
         self.grpc_channel.close()
 
     @property
     def delete_operation(
         self,
     ) -> Callable[[operations_pb2.DeleteOperationRequest], None]:
```

### Comparing `google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/services/parallelstore/transports/grpc_asyncio.py` & `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/transports/grpc_asyncio.py`

 * *Files 16% similar despite different names*

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
@@ -12,15 +12,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
 import warnings
 
+from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1, grpc_helpers_async, operations_v1
+from google.api_core import retry_async as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.cloud.location import locations_pb2  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
@@ -82,15 +84,14 @@
             credentials (Optional[~.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify this application to the service. If
                 none are specified, the client will attempt to ascertain
                 the credentials from the environment.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
             scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
                 service. These are only used when credentials are not specified and
                 are passed to :func:`google.auth.default`.
             quota_project_id (Optional[str]): An optional project to use for billing
                 and quota.
             kwargs (Optional[dict]): Keyword arguments, which are passed to the
                 channel creation.
@@ -112,15 +113,15 @@
     def __init__(
         self,
         *,
         host: str = "parallelstore.googleapis.com",
         credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: Optional[aio.Channel] = None,
+        channel: Optional[Union[aio.Channel, Callable[..., aio.Channel]]] = None,
         api_mtls_endpoint: Optional[str] = None,
         client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
         client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
@@ -132,37 +133,40 @@
             host (Optional[str]):
                  The hostname to connect to (default: 'parallelstore.googleapis.com').
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
                 service. These are only used when credentials are not specified and
                 are passed to :func:`google.auth.default`.
-            channel (Optional[aio.Channel]): A ``Channel`` instance through
-                which to make calls.
+            channel (Optional[Union[aio.Channel, Callable[..., aio.Channel]]]):
+                A ``Channel`` instance through which to make calls, or a Callable
+                that constructs and returns one. If set to None, ``self.create_channel``
+                is used to create the channel. If a Callable is given, it will be called
+                with the same arguments as used in ``self.create_channel``.
             api_mtls_endpoint (Optional[str]): Deprecated. The mutual TLS endpoint.
                 If provided, it overrides the ``host`` argument and tries to create
                 a mutual TLS channel with client SSL credentials from
                 ``client_cert_source`` or application default SSL credentials.
             client_cert_source (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 Deprecated. A callback to provide client SSL certificate bytes and
                 private key bytes, both in PEM format. It is ignored if
                 ``api_mtls_endpoint`` is None.
             ssl_channel_credentials (grpc.ChannelCredentials): SSL credentials
-                for the grpc channel. It is ignored if ``channel`` is provided.
+                for the grpc channel. It is ignored if a ``channel`` instance is provided.
             client_cert_source_for_mtls (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 A callback to provide client certificate bytes and private key bytes,
                 both in PEM format. It is used to configure a mutual TLS channel. It is
-                ignored if ``channel`` or ``ssl_channel_credentials`` is provided.
+                ignored if a ``channel`` instance or ``ssl_channel_credentials`` is provided.
             quota_project_id (Optional[str]): An optional project to use for billing
                 and quota.
             client_info (google.api_core.gapic_v1.client_info.ClientInfo):
                 The client info used to send a user-agent string along with
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
@@ -181,15 +185,15 @@
         self._operations_client: Optional[operations_v1.OperationsAsyncClient] = None
 
         if api_mtls_endpoint:
             warnings.warn("api_mtls_endpoint is deprecated", DeprecationWarning)
         if client_cert_source:
             warnings.warn("client_cert_source is deprecated", DeprecationWarning)
 
-        if channel:
+        if isinstance(channel, aio.Channel):
             # Ignore credentials if a channel was passed.
             credentials = False
             # If a channel was explicitly provided, set it.
             self._grpc_channel = channel
             self._ssl_channel_credentials = None
         else:
             if api_mtls_endpoint:
@@ -221,15 +225,17 @@
             quota_project_id=quota_project_id,
             client_info=client_info,
             always_use_jwt_access=always_use_jwt_access,
             api_audience=api_audience,
         )
 
         if not self._grpc_channel:
-            self._grpc_channel = type(self).create_channel(
+            # initialize with the provided callable or the default channel
+            channel_init = channel or type(self).create_channel
+            self._grpc_channel = channel_init(
                 self._host,
                 # use the credentials which are saved
                 credentials=self._credentials,
                 # Set ``credentials_file`` to ``None`` here as
                 # the credentials that we saved earlier should be used.
                 credentials_file=None,
                 scopes=self._scopes,
@@ -408,14 +414,112 @@
             self._stubs["delete_instance"] = self.grpc_channel.unary_unary(
                 "/google.cloud.parallelstore.v1beta.Parallelstore/DeleteInstance",
                 request_serializer=parallelstore.DeleteInstanceRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["delete_instance"]
 
+    @property
+    def import_data(
+        self,
+    ) -> Callable[
+        [parallelstore.ImportDataRequest], Awaitable[operations_pb2.Operation]
+    ]:
+        r"""Return a callable for the import data method over gRPC.
+
+        ImportData copies data from Cloud Storage to
+        Parallelstore.
+
+        Returns:
+            Callable[[~.ImportDataRequest],
+                    Awaitable[~.Operation]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "import_data" not in self._stubs:
+            self._stubs["import_data"] = self.grpc_channel.unary_unary(
+                "/google.cloud.parallelstore.v1beta.Parallelstore/ImportData",
+                request_serializer=parallelstore.ImportDataRequest.serialize,
+                response_deserializer=operations_pb2.Operation.FromString,
+            )
+        return self._stubs["import_data"]
+
+    @property
+    def export_data(
+        self,
+    ) -> Callable[
+        [parallelstore.ExportDataRequest], Awaitable[operations_pb2.Operation]
+    ]:
+        r"""Return a callable for the export data method over gRPC.
+
+        ExportData copies data from Parallelstore to Cloud
+        Storage
+
+        Returns:
+            Callable[[~.ExportDataRequest],
+                    Awaitable[~.Operation]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "export_data" not in self._stubs:
+            self._stubs["export_data"] = self.grpc_channel.unary_unary(
+                "/google.cloud.parallelstore.v1beta.Parallelstore/ExportData",
+                request_serializer=parallelstore.ExportDataRequest.serialize,
+                response_deserializer=operations_pb2.Operation.FromString,
+            )
+        return self._stubs["export_data"]
+
+    def _prep_wrapped_messages(self, client_info):
+        """Precompute the wrapped methods, overriding the base class method to use async wrappers."""
+        self._wrapped_methods = {
+            self.list_instances: gapic_v1.method_async.wrap_method(
+                self.list_instances,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.get_instance: gapic_v1.method_async.wrap_method(
+                self.get_instance,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.create_instance: gapic_v1.method_async.wrap_method(
+                self.create_instance,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.update_instance: gapic_v1.method_async.wrap_method(
+                self.update_instance,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.delete_instance: gapic_v1.method_async.wrap_method(
+                self.delete_instance,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.import_data: gapic_v1.method_async.wrap_method(
+                self.import_data,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.export_data: gapic_v1.method_async.wrap_method(
+                self.export_data,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+        }
+
     def close(self):
         return self.grpc_channel.close()
 
     @property
     def delete_operation(
         self,
     ) -> Callable[[operations_pb2.DeleteOperationRequest], None]:
```

### Comparing `google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/services/parallelstore/transports/rest.py` & `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/transports/rest.py`

 * *Files 3% similar despite different names*

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
@@ -84,22 +84,38 @@
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_delete_instance(self, response):
                 logging.log(f"Received response: {response}")
                 return response
 
+            def pre_export_data(self, request, metadata):
+                logging.log(f"Received request: {request}")
+                return request, metadata
+
+            def post_export_data(self, response):
+                logging.log(f"Received response: {response}")
+                return response
+
             def pre_get_instance(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_get_instance(self, response):
                 logging.log(f"Received response: {response}")
                 return response
 
+            def pre_import_data(self, request, metadata):
+                logging.log(f"Received request: {request}")
+                return request, metadata
+
+            def post_import_data(self, response):
+                logging.log(f"Received response: {response}")
+                return response
+
             def pre_list_instances(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_list_instances(self, response):
                 logging.log(f"Received response: {response}")
                 return response
@@ -160,14 +176,37 @@
 
         Override in a subclass to manipulate the response
         after it is returned by the Parallelstore server but before
         it is returned to user code.
         """
         return response
 
+    def pre_export_data(
+        self,
+        request: parallelstore.ExportDataRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[parallelstore.ExportDataRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for export_data
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the Parallelstore server.
+        """
+        return request, metadata
+
+    def post_export_data(
+        self, response: operations_pb2.Operation
+    ) -> operations_pb2.Operation:
+        """Post-rpc interceptor for export_data
+
+        Override in a subclass to manipulate the response
+        after it is returned by the Parallelstore server but before
+        it is returned to user code.
+        """
+        return response
+
     def pre_get_instance(
         self,
         request: parallelstore.GetInstanceRequest,
         metadata: Sequence[Tuple[str, str]],
     ) -> Tuple[parallelstore.GetInstanceRequest, Sequence[Tuple[str, str]]]:
         """Pre-rpc interceptor for get_instance
 
@@ -183,14 +222,37 @@
 
         Override in a subclass to manipulate the response
         after it is returned by the Parallelstore server but before
         it is returned to user code.
         """
         return response
 
+    def pre_import_data(
+        self,
+        request: parallelstore.ImportDataRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[parallelstore.ImportDataRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for import_data
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the Parallelstore server.
+        """
+        return request, metadata
+
+    def post_import_data(
+        self, response: operations_pb2.Operation
+    ) -> operations_pb2.Operation:
+        """Post-rpc interceptor for import_data
+
+        Override in a subclass to manipulate the response
+        after it is returned by the Parallelstore server but before
+        it is returned to user code.
+        """
+        return response
+
     def pre_list_instances(
         self,
         request: parallelstore.ListInstancesRequest,
         metadata: Sequence[Tuple[str, str]],
     ) -> Tuple[parallelstore.ListInstancesRequest, Sequence[Tuple[str, str]]]:
         """Pre-rpc interceptor for list_instances
 
@@ -716,14 +778,109 @@
 
             # Return the response
             resp = operations_pb2.Operation()
             json_format.Parse(response.content, resp, ignore_unknown_fields=True)
             resp = self._interceptor.post_delete_instance(resp)
             return resp
 
+    class _ExportData(ParallelstoreRestStub):
+        def __hash__(self):
+            return hash("ExportData")
+
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
+
+        @classmethod
+        def _get_unset_required_fields(cls, message_dict):
+            return {
+                k: v
+                for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
+                if k not in message_dict
+            }
+
+        def __call__(
+            self,
+            request: parallelstore.ExportDataRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> operations_pb2.Operation:
+            r"""Call the export data method over HTTP.
+
+            Args:
+                request (~.parallelstore.ExportDataRequest):
+                    The request object. Message representing the request
+                exporting data from Cloud Storage to
+                parallelstore.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                ~.operations_pb2.Operation:
+                    This resource represents a
+                long-running operation that is the
+                result of a network API call.
+
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "post",
+                    "uri": "/v1beta/{name=projects/*/locations/*/instances/*}:exportData",
+                    "body": "*",
+                },
+            ]
+            request, metadata = self._interceptor.pre_export_data(request, metadata)
+            pb_request = parallelstore.ExportDataRequest.pb(request)
+            transcoded_request = path_template.transcode(http_options, pb_request)
+
+            # Jsonify the request body
+
+            body = json_format.MessageToJson(
+                transcoded_request["body"], use_integers_for_enums=True
+            )
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(
+                json_format.MessageToJson(
+                    transcoded_request["query_params"],
+                    use_integers_for_enums=True,
+                )
+            )
+            query_params.update(self._get_unset_required_fields(query_params))
+
+            query_params["$alt"] = "json;enum-encoding=int"
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params, strict=True),
+                data=body,
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            # Return the response
+            resp = operations_pb2.Operation()
+            json_format.Parse(response.content, resp, ignore_unknown_fields=True)
+            resp = self._interceptor.post_export_data(resp)
+            return resp
+
     class _GetInstance(ParallelstoreRestStub):
         def __hash__(self):
             return hash("GetInstance")
 
         __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
@@ -801,14 +958,109 @@
             resp = parallelstore.Instance()
             pb_resp = parallelstore.Instance.pb(resp)
 
             json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
             resp = self._interceptor.post_get_instance(resp)
             return resp
 
+    class _ImportData(ParallelstoreRestStub):
+        def __hash__(self):
+            return hash("ImportData")
+
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
+
+        @classmethod
+        def _get_unset_required_fields(cls, message_dict):
+            return {
+                k: v
+                for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
+                if k not in message_dict
+            }
+
+        def __call__(
+            self,
+            request: parallelstore.ImportDataRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> operations_pb2.Operation:
+            r"""Call the import data method over HTTP.
+
+            Args:
+                request (~.parallelstore.ImportDataRequest):
+                    The request object. Message representing the request
+                importing data from parallelstore to
+                Cloud Storage.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                ~.operations_pb2.Operation:
+                    This resource represents a
+                long-running operation that is the
+                result of a network API call.
+
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "post",
+                    "uri": "/v1beta/{name=projects/*/locations/*/instances/*}:importData",
+                    "body": "*",
+                },
+            ]
+            request, metadata = self._interceptor.pre_import_data(request, metadata)
+            pb_request = parallelstore.ImportDataRequest.pb(request)
+            transcoded_request = path_template.transcode(http_options, pb_request)
+
+            # Jsonify the request body
+
+            body = json_format.MessageToJson(
+                transcoded_request["body"], use_integers_for_enums=True
+            )
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(
+                json_format.MessageToJson(
+                    transcoded_request["query_params"],
+                    use_integers_for_enums=True,
+                )
+            )
+            query_params.update(self._get_unset_required_fields(query_params))
+
+            query_params["$alt"] = "json;enum-encoding=int"
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params, strict=True),
+                data=body,
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            # Return the response
+            resp = operations_pb2.Operation()
+            json_format.Parse(response.content, resp, ignore_unknown_fields=True)
+            resp = self._interceptor.post_import_data(resp)
+            return resp
+
     class _ListInstances(ParallelstoreRestStub):
         def __hash__(self):
             return hash("ListInstances")
 
         __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
@@ -1001,22 +1253,38 @@
         self,
     ) -> Callable[[parallelstore.DeleteInstanceRequest], operations_pb2.Operation]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._DeleteInstance(self._session, self._host, self._interceptor)  # type: ignore
 
     @property
+    def export_data(
+        self,
+    ) -> Callable[[parallelstore.ExportDataRequest], operations_pb2.Operation]:
+        # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
+        # In C++ this would require a dynamic_cast
+        return self._ExportData(self._session, self._host, self._interceptor)  # type: ignore
+
+    @property
     def get_instance(
         self,
     ) -> Callable[[parallelstore.GetInstanceRequest], parallelstore.Instance]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._GetInstance(self._session, self._host, self._interceptor)  # type: ignore
 
     @property
+    def import_data(
+        self,
+    ) -> Callable[[parallelstore.ImportDataRequest], operations_pb2.Operation]:
+        # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
+        # In C++ this would require a dynamic_cast
+        return self._ImportData(self._session, self._host, self._interceptor)  # type: ignore
+
+    @property
     def list_instances(
         self,
     ) -> Callable[
         [parallelstore.ListInstancesRequest], parallelstore.ListInstancesResponse
     ]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
```

### Comparing `google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/types/__init__.py` & `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/types/__init__.py`

 * *Files 25% similar despite different names*

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
@@ -12,25 +12,43 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from .parallelstore import (
     CreateInstanceRequest,
     DeleteInstanceRequest,
+    ExportDataMetadata,
+    ExportDataRequest,
+    ExportDataResponse,
     GetInstanceRequest,
+    ImportDataMetadata,
+    ImportDataRequest,
+    ImportDataResponse,
     Instance,
     ListInstancesRequest,
     ListInstancesResponse,
     OperationMetadata,
+    TransferCounters,
+    TransferOperationMetadata,
+    TransferType,
     UpdateInstanceRequest,
 )
 
 __all__ = (
     "CreateInstanceRequest",
     "DeleteInstanceRequest",
+    "ExportDataMetadata",
+    "ExportDataRequest",
+    "ExportDataResponse",
     "GetInstanceRequest",
+    "ImportDataMetadata",
+    "ImportDataRequest",
+    "ImportDataResponse",
     "Instance",
     "ListInstancesRequest",
     "ListInstancesResponse",
     "OperationMetadata",
+    "TransferCounters",
+    "TransferOperationMetadata",
     "UpdateInstanceRequest",
+    "TransferType",
 )
```

### Comparing `google-cloud-parallelstore-0.1.1/google/cloud/parallelstore_v1beta/types/parallelstore.py` & `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/types/parallelstore.py`

 * *Files 21% similar despite different names*

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
@@ -20,26 +20,51 @@
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.parallelstore.v1beta",
     manifest={
+        "TransferType",
         "Instance",
         "ListInstancesRequest",
         "ListInstancesResponse",
         "GetInstanceRequest",
         "CreateInstanceRequest",
         "UpdateInstanceRequest",
         "DeleteInstanceRequest",
         "OperationMetadata",
+        "ImportDataRequest",
+        "ExportDataRequest",
+        "ImportDataResponse",
+        "ImportDataMetadata",
+        "ExportDataResponse",
+        "ExportDataMetadata",
+        "TransferOperationMetadata",
+        "TransferCounters",
     },
 )
 
 
+class TransferType(proto.Enum):
+    r"""Type of transfer that occurred.
+
+    Values:
+        TRANSFER_TYPE_UNSPECIFIED (0):
+            Zero is an illegal value.
+        IMPORT (1):
+            Imports to Parallelstore.
+        EXPORT (2):
+            Exports from Parallelstore.
+    """
+    TRANSFER_TYPE_UNSPECIFIED = 0
+    IMPORT = 1
+    EXPORT = 2
+
+
 class Instance(proto.Message):
     r"""A Parallelstore instance.
 
     Attributes:
         name (str):
             Identifier. The resource name of the instance, in the format
             ``projects/{project}/locations/{location}/instances/{instance_id}``
@@ -94,20 +119,28 @@
             Output only. List of access_points. Contains a list of IPv4
             addresses used for client side configuration.
         network (str):
             Optional. Immutable. The name of the Google Compute Engine
             `VPC network <https://cloud.google.com/vpc/docs/vpc>`__ to
             which the instance is connected.
         reserved_ip_range (str):
-            Optional. Immutable. Contains the id of
+            Optional. Immutable. Contains the id of the
             allocated IP address range associated with the
             private service access connection for example,
             "test-default" associated with IP range
             10.0.0.0/29. If no range id is provided all
             ranges will be considered.
+        effective_reserved_ip_range (str):
+            Output only. Immutable. Contains the id of
+            the allocated IP address range associated with
+            the private service access connection for
+            example, "test-default" associated with IP range
+            10.0.0.0/29. This field is populated by the
+            service and and contains the value currently
+            used by the service.
     """
 
     class State(proto.Enum):
         r"""Represents the different states of a Parallelstore instance.
 
         Values:
             STATE_UNSPECIFIED (0):
@@ -171,14 +204,18 @@
         proto.STRING,
         number=11,
     )
     reserved_ip_range: str = proto.Field(
         proto.STRING,
         number=12,
     )
+    effective_reserved_ip_range: str = proto.Field(
+        proto.STRING,
+        number=14,
+    )
 
 
 class ListInstancesRequest(proto.Message):
     r"""Message for requesting list of Instances
 
     Attributes:
         parent (str):
@@ -479,8 +516,289 @@
     )
     api_version: str = proto.Field(
         proto.STRING,
         number=7,
     )
 
 
+class ImportDataRequest(proto.Message):
+    r"""Message representing the request importing data from
+    parallelstore to Cloud Storage.
+
+
+    .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
+
+    Attributes:
+        source_gcs_uri (str):
+            URI to a Cloud Storage object in format:
+            'gs://<bucket_name>/<path_inside_bucket>'.
+
+            This field is a member of `oneof`_ ``source``.
+        destination_path (str):
+            Optional. Root directory path to the
+            Paralellstore filesystem, starting with '/'.
+            Sets to '/' if no value is set.
+
+            This field is a member of `oneof`_ ``destination``.
+        name (str):
+            Required. Name of the resource.
+        request_id (str):
+            Optional. An optional request ID to identify
+            requests. Specify a unique request ID so that if
+            you must retry your request, the server will
+            know to ignore the request if it has already
+            been completed. The server will guarantee that
+            for at least 60 minutes since the first request.
+
+            For example, consider a situation where you make
+            an initial request and t he request times out.
+            If you make the request again with the same
+            request ID, the server can check if original
+            operation with the same request ID was received,
+            and if so, will ignore the second request. This
+            prevents clients from accidentally creating
+            duplicate commitments.
+
+            The request ID must be a valid UUID with the
+            exception that zero UUID is not supported
+            (00000000-0000-0000-0000-000000000000).
+    """
+
+    source_gcs_uri: str = proto.Field(
+        proto.STRING,
+        number=2,
+        oneof="source",
+    )
+    destination_path: str = proto.Field(
+        proto.STRING,
+        number=3,
+        oneof="destination",
+    )
+    name: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    request_id: str = proto.Field(
+        proto.STRING,
+        number=4,
+    )
+
+
+class ExportDataRequest(proto.Message):
+    r"""Message representing the request exporting data from Cloud
+    Storage to parallelstore.
+
+
+    .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
+
+    Attributes:
+        source_path (str):
+            Optional. Root directory path to the
+            Paralellstore filesystem, starting with '/'.
+            Sets to '/' if no value is set.
+
+            This field is a member of `oneof`_ ``source``.
+        destination_gcs_uri (str):
+            URI to a Cloud Storage object in format:
+            'gs://<bucket_name>/<path_inside_bucket>'.
+
+            This field is a member of `oneof`_ ``destination``.
+        name (str):
+            Required. Name of the resource.
+        request_id (str):
+            Optional. An optional request ID to identify
+            requests. Specify a unique request ID so that if
+            you must retry your request, the server will
+            know to ignore the request if it has already
+            been completed. The server will guarantee that
+            for at least 60 minutes since the first request.
+
+            For example, consider a situation where you make
+            an initial request and t he request times out.
+            If you make the request again with the same
+            request ID, the server can check if original
+            operation with the same request ID was received,
+            and if so, will ignore the second request. This
+            prevents clients from accidentally creating
+            duplicate commitments.
+
+            The request ID must be a valid UUID with the
+            exception that zero UUID is not supported
+            (00000000-0000-0000-0000-000000000000).
+    """
+
+    source_path: str = proto.Field(
+        proto.STRING,
+        number=2,
+        oneof="source",
+    )
+    destination_gcs_uri: str = proto.Field(
+        proto.STRING,
+        number=3,
+        oneof="destination",
+    )
+    name: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    request_id: str = proto.Field(
+        proto.STRING,
+        number=4,
+    )
+
+
+class ImportDataResponse(proto.Message):
+    r"""ImportDataResponse is the response returned from ImportData
+    rpc.
+
+    """
+
+
+class ImportDataMetadata(proto.Message):
+    r"""ImportDataMetadata contains import data operation metadata
+
+    Attributes:
+        operation_metadata (google.cloud.parallelstore_v1beta.types.TransferOperationMetadata):
+            Contains the data transfer operation
+            metadata.
+    """
+
+    operation_metadata: "TransferOperationMetadata" = proto.Field(
+        proto.MESSAGE,
+        number=1,
+        message="TransferOperationMetadata",
+    )
+
+
+class ExportDataResponse(proto.Message):
+    r"""ExportDataResponse is the response returned from ExportData
+    rpc
+
+    """
+
+
+class ExportDataMetadata(proto.Message):
+    r"""ExportDataMetadata contains export data operation metadata
+
+    Attributes:
+        operation_metadata (google.cloud.parallelstore_v1beta.types.TransferOperationMetadata):
+            Contains the data transfer operation
+            metadata.
+    """
+
+    operation_metadata: "TransferOperationMetadata" = proto.Field(
+        proto.MESSAGE,
+        number=1,
+        message="TransferOperationMetadata",
+    )
+
+
+class TransferOperationMetadata(proto.Message):
+    r"""Represents the metadata of the long-running operation.
+
+    Attributes:
+        create_time (google.protobuf.timestamp_pb2.Timestamp):
+            Output only. CCFE supplied fields BEGIN
+            The time the operation was created.
+        end_time (google.protobuf.timestamp_pb2.Timestamp):
+            Output only. The time the operation finished
+            running.
+        counters (google.cloud.parallelstore_v1beta.types.TransferCounters):
+            Information about the progress of the
+            transfer operation.
+        source (str):
+            Required. The origin of the data transfer.
+        destination (str):
+            Required. The destination of the data
+            transfer.
+        transfer_type (google.cloud.parallelstore_v1beta.types.TransferType):
+            The type of transfer occurring.
+    """
+
+    create_time: timestamp_pb2.Timestamp = proto.Field(
+        proto.MESSAGE,
+        number=1,
+        message=timestamp_pb2.Timestamp,
+    )
+    end_time: timestamp_pb2.Timestamp = proto.Field(
+        proto.MESSAGE,
+        number=2,
+        message=timestamp_pb2.Timestamp,
+    )
+    counters: "TransferCounters" = proto.Field(
+        proto.MESSAGE,
+        number=3,
+        message="TransferCounters",
+    )
+    source: str = proto.Field(
+        proto.STRING,
+        number=4,
+    )
+    destination: str = proto.Field(
+        proto.STRING,
+        number=5,
+    )
+    transfer_type: "TransferType" = proto.Field(
+        proto.ENUM,
+        number=6,
+        enum="TransferType",
+    )
+
+
+class TransferCounters(proto.Message):
+    r"""A collection of counters that report the progress of a
+    transfer operation.
+
+    Attributes:
+        objects_found (int):
+            Objects found in the data source that are
+            scheduled to be transferred, excluding any that
+            are filtered based on object conditions or
+            skipped due to sync.
+        bytes_found (int):
+            Bytes found in the data source that are
+            scheduled to be transferred, excluding any that
+            are filtered based on object conditions or
+            skipped due to sync.
+        objects_skipped (int):
+            Objects in the data source that are not
+            transferred because they already exist in the
+            data destination.
+        bytes_skipped (int):
+            Bytes in the data source that are not
+            transferred because they already exist in the
+            data destination.
+        objects_copied (int):
+            Objects that are copied to the data
+            destination.
+        bytes_copied (int):
+            Bytes that are copied to the data
+            destination.
+    """
+
+    objects_found: int = proto.Field(
+        proto.INT64,
+        number=1,
+    )
+    bytes_found: int = proto.Field(
+        proto.INT64,
+        number=2,
+    )
+    objects_skipped: int = proto.Field(
+        proto.INT64,
+        number=3,
+    )
+    bytes_skipped: int = proto.Field(
+        proto.INT64,
+        number=4,
+    )
+    objects_copied: int = proto.Field(
+        proto.INT64,
+        number=5,
+    )
+    bytes_copied: int = proto.Field(
+        proto.INT64,
+        number=6,
+    )
+
+
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-parallelstore-0.1.1/google_cloud_parallelstore.egg-info/PKG-INFO` & `google-cloud-parallelstore-0.1.2/google_cloud_parallelstore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-parallelstore
-Version: 0.1.1
+Version: 0.1.2
 Summary: Google Cloud Parallelstore API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-parallelstore
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-parallelstore-0.1.1/google_cloud_parallelstore.egg-info/SOURCES.txt` & `google-cloud-parallelstore-0.1.2/google_cloud_parallelstore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-parallelstore-0.1.1/setup.py` & `google-cloud-parallelstore-0.1.2/setup.py`

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

### Comparing `google-cloud-parallelstore-0.1.1/tests/__init__.py` & `google-cloud-parallelstore-0.1.2/tests/__init__.py`

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

### Comparing `google-cloud-parallelstore-0.1.1/tests/unit/__init__.py` & `google-cloud-parallelstore-0.1.2/tests/unit/__init__.py`

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

### Comparing `google-cloud-parallelstore-0.1.1/tests/unit/gapic/__init__.py` & `google-cloud-parallelstore-0.1.2/tests/unit/gapic/__init__.py`

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

### Comparing `google-cloud-parallelstore-0.1.1/tests/unit/gapic/parallelstore_v1beta/__init__.py` & `google-cloud-parallelstore-0.1.2/tests/unit/gapic/parallelstore_v1beta/__init__.py`

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

### Comparing `google-cloud-parallelstore-0.1.1/tests/unit/gapic/parallelstore_v1beta/test_parallelstore.py` & `google-cloud-parallelstore-0.1.2/tests/unit/gapic/parallelstore_v1beta/test_parallelstore.py`

 * *Files 13% similar despite different names*

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
@@ -1151,15 +1151,16 @@
             unreachable=["unreachable_value"],
         )
         response = client.list_instances(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == parallelstore.ListInstancesRequest()
+        request = parallelstore.ListInstancesRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListInstancesPager)
     assert response.next_page_token == "next_page_token_value"
     assert response.unreachable == ["unreachable_value"]
 
 
@@ -1169,20 +1170,162 @@
     client = ParallelstoreClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_instances), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_instances()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == parallelstore.ListInstancesRequest()
 
 
+def test_list_instances_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ParallelstoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = parallelstore.ListInstancesRequest(
+        parent="parent_value",
+        page_token="page_token_value",
+        filter="filter_value",
+        order_by="order_by_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_instances), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.list_instances(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == parallelstore.ListInstancesRequest(
+            parent="parent_value",
+            page_token="page_token_value",
+            filter="filter_value",
+            order_by="order_by_value",
+        )
+
+
+def test_list_instances_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ParallelstoreClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.list_instances in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.list_instances] = mock_rpc
+        request = {}
+        client.list_instances(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_instances(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_list_instances_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ParallelstoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_instances), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            parallelstore.ListInstancesResponse(
+                next_page_token="next_page_token_value",
+                unreachable=["unreachable_value"],
+            )
+        )
+        response = await client.list_instances()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == parallelstore.ListInstancesRequest()
+
+
+@pytest.mark.asyncio
+async def test_list_instances_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = ParallelstoreAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.list_instances
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.list_instances
+        ] = mock_object
+
+        request = {}
+        await client.list_instances(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.list_instances(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_list_instances_async(
     transport: str = "grpc_asyncio", request_type=parallelstore.ListInstancesRequest
 ):
     client = ParallelstoreAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1202,15 +1345,16 @@
             )
         )
         response = await client.list_instances(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == parallelstore.ListInstancesRequest()
+        request = parallelstore.ListInstancesRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListInstancesAsyncPager)
     assert response.next_page_token == "next_page_token_value"
     assert response.unreachable == ["unreachable_value"]
 
 
@@ -1577,50 +1721,196 @@
             description="description_value",
             state=parallelstore.Instance.State.CREATING,
             capacity_gib=1247,
             daos_version="daos_version_value",
             access_points=["access_points_value"],
             network="network_value",
             reserved_ip_range="reserved_ip_range_value",
+            effective_reserved_ip_range="effective_reserved_ip_range_value",
         )
         response = client.get_instance(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == parallelstore.GetInstanceRequest()
+        request = parallelstore.GetInstanceRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, parallelstore.Instance)
     assert response.name == "name_value"
     assert response.description == "description_value"
     assert response.state == parallelstore.Instance.State.CREATING
     assert response.capacity_gib == 1247
     assert response.daos_version == "daos_version_value"
     assert response.access_points == ["access_points_value"]
     assert response.network == "network_value"
     assert response.reserved_ip_range == "reserved_ip_range_value"
+    assert response.effective_reserved_ip_range == "effective_reserved_ip_range_value"
 
 
 def test_get_instance_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = ParallelstoreClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_instance), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_instance()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == parallelstore.GetInstanceRequest()
 
 
+def test_get_instance_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ParallelstoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = parallelstore.GetInstanceRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_instance), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.get_instance(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == parallelstore.GetInstanceRequest(
+            name="name_value",
+        )
+
+
+def test_get_instance_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ParallelstoreClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.get_instance in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.get_instance] = mock_rpc
+        request = {}
+        client.get_instance(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_instance(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_get_instance_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ParallelstoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_instance), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            parallelstore.Instance(
+                name="name_value",
+                description="description_value",
+                state=parallelstore.Instance.State.CREATING,
+                capacity_gib=1247,
+                daos_version="daos_version_value",
+                access_points=["access_points_value"],
+                network="network_value",
+                reserved_ip_range="reserved_ip_range_value",
+                effective_reserved_ip_range="effective_reserved_ip_range_value",
+            )
+        )
+        response = await client.get_instance()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == parallelstore.GetInstanceRequest()
+
+
+@pytest.mark.asyncio
+async def test_get_instance_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = ParallelstoreAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.get_instance
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.get_instance
+        ] = mock_object
+
+        request = {}
+        await client.get_instance(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.get_instance(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_get_instance_async(
     transport: str = "grpc_asyncio", request_type=parallelstore.GetInstanceRequest
 ):
     client = ParallelstoreAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1639,33 +1929,36 @@
                 description="description_value",
                 state=parallelstore.Instance.State.CREATING,
                 capacity_gib=1247,
                 daos_version="daos_version_value",
                 access_points=["access_points_value"],
                 network="network_value",
                 reserved_ip_range="reserved_ip_range_value",
+                effective_reserved_ip_range="effective_reserved_ip_range_value",
             )
         )
         response = await client.get_instance(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == parallelstore.GetInstanceRequest()
+        request = parallelstore.GetInstanceRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, parallelstore.Instance)
     assert response.name == "name_value"
     assert response.description == "description_value"
     assert response.state == parallelstore.Instance.State.CREATING
     assert response.capacity_gib == 1247
     assert response.daos_version == "daos_version_value"
     assert response.access_points == ["access_points_value"]
     assert response.network == "network_value"
     assert response.reserved_ip_range == "reserved_ip_range_value"
+    assert response.effective_reserved_ip_range == "effective_reserved_ip_range_value"
 
 
 @pytest.mark.asyncio
 async def test_get_instance_async_from_dict():
     await test_get_instance_async(request_type=dict)
 
 
@@ -1834,15 +2127,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = operations_pb2.Operation(name="operations/spam")
         response = client.create_instance(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == parallelstore.CreateInstanceRequest()
+        request = parallelstore.CreateInstanceRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, future.Future)
 
 
 def test_create_instance_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
@@ -1850,20 +2144,165 @@
     client = ParallelstoreClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_instance), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.create_instance()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == parallelstore.CreateInstanceRequest()
 
 
+def test_create_instance_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ParallelstoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = parallelstore.CreateInstanceRequest(
+        parent="parent_value",
+        instance_id="instance_id_value",
+        request_id="request_id_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.create_instance), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.create_instance(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == parallelstore.CreateInstanceRequest(
+            parent="parent_value",
+            instance_id="instance_id_value",
+            request_id="request_id_value",
+        )
+
+
+def test_create_instance_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ParallelstoreClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.create_instance in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.create_instance] = mock_rpc
+        request = {}
+        client.create_instance(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.create_instance(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_create_instance_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ParallelstoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.create_instance), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/spam")
+        )
+        response = await client.create_instance()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == parallelstore.CreateInstanceRequest()
+
+
+@pytest.mark.asyncio
+async def test_create_instance_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = ParallelstoreAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.create_instance
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.create_instance
+        ] = mock_object
+
+        request = {}
+        await client.create_instance(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        await client.create_instance(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_create_instance_async(
     transport: str = "grpc_asyncio", request_type=parallelstore.CreateInstanceRequest
 ):
     client = ParallelstoreAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1880,15 +2319,16 @@
             operations_pb2.Operation(name="operations/spam")
         )
         response = await client.create_instance(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == parallelstore.CreateInstanceRequest()
+        request = parallelstore.CreateInstanceRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, future.Future)
 
 
 @pytest.mark.asyncio
 async def test_create_instance_async_from_dict():
@@ -2080,15 +2520,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = operations_pb2.Operation(name="operations/spam")
         response = client.update_instance(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == parallelstore.UpdateInstanceRequest()
+        request = parallelstore.UpdateInstanceRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, future.Future)
 
 
 def test_update_instance_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
@@ -2096,20 +2537,161 @@
     client = ParallelstoreClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_instance), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.update_instance()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == parallelstore.UpdateInstanceRequest()
 
 
+def test_update_instance_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ParallelstoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = parallelstore.UpdateInstanceRequest(
+        request_id="request_id_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.update_instance), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.update_instance(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == parallelstore.UpdateInstanceRequest(
+            request_id="request_id_value",
+        )
+
+
+def test_update_instance_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ParallelstoreClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.update_instance in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.update_instance] = mock_rpc
+        request = {}
+        client.update_instance(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.update_instance(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_update_instance_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ParallelstoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.update_instance), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/spam")
+        )
+        response = await client.update_instance()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == parallelstore.UpdateInstanceRequest()
+
+
+@pytest.mark.asyncio
+async def test_update_instance_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = ParallelstoreAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.update_instance
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.update_instance
+        ] = mock_object
+
+        request = {}
+        await client.update_instance(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        await client.update_instance(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_update_instance_async(
     transport: str = "grpc_asyncio", request_type=parallelstore.UpdateInstanceRequest
 ):
     client = ParallelstoreAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -2126,15 +2708,16 @@
             operations_pb2.Operation(name="operations/spam")
         )
         response = await client.update_instance(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == parallelstore.UpdateInstanceRequest()
+        request = parallelstore.UpdateInstanceRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, future.Future)
 
 
 @pytest.mark.asyncio
 async def test_update_instance_async_from_dict():
@@ -2316,15 +2899,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = operations_pb2.Operation(name="operations/spam")
         response = client.delete_instance(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == parallelstore.DeleteInstanceRequest()
+        request = parallelstore.DeleteInstanceRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, future.Future)
 
 
 def test_delete_instance_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
@@ -2332,20 +2916,163 @@
     client = ParallelstoreClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.delete_instance), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.delete_instance()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == parallelstore.DeleteInstanceRequest()
 
 
+def test_delete_instance_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ParallelstoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = parallelstore.DeleteInstanceRequest(
+        name="name_value",
+        request_id="request_id_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.delete_instance), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.delete_instance(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == parallelstore.DeleteInstanceRequest(
+            name="name_value",
+            request_id="request_id_value",
+        )
+
+
+def test_delete_instance_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ParallelstoreClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.delete_instance in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.delete_instance] = mock_rpc
+        request = {}
+        client.delete_instance(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.delete_instance(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_delete_instance_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ParallelstoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.delete_instance), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/spam")
+        )
+        response = await client.delete_instance()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == parallelstore.DeleteInstanceRequest()
+
+
+@pytest.mark.asyncio
+async def test_delete_instance_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = ParallelstoreAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.delete_instance
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.delete_instance
+        ] = mock_object
+
+        request = {}
+        await client.delete_instance(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        await client.delete_instance(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_delete_instance_async(
     transport: str = "grpc_asyncio", request_type=parallelstore.DeleteInstanceRequest
 ):
     client = ParallelstoreAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -2362,15 +3089,16 @@
             operations_pb2.Operation(name="operations/spam")
         )
         response = await client.delete_instance(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == parallelstore.DeleteInstanceRequest()
+        request = parallelstore.DeleteInstanceRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, future.Future)
 
 
 @pytest.mark.asyncio
 async def test_delete_instance_async_from_dict():
@@ -2519,14 +3247,596 @@
             name="name_value",
         )
 
 
 @pytest.mark.parametrize(
     "request_type",
     [
+        parallelstore.ImportDataRequest,
+        dict,
+    ],
+)
+def test_import_data(request_type, transport: str = "grpc"):
+    client = ParallelstoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.import_data), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = operations_pb2.Operation(name="operations/spam")
+        response = client.import_data(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        request = parallelstore.ImportDataRequest()
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, future.Future)
+
+
+def test_import_data_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ParallelstoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.import_data), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.import_data()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == parallelstore.ImportDataRequest()
+
+
+def test_import_data_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ParallelstoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = parallelstore.ImportDataRequest(
+        source_gcs_uri="source_gcs_uri_value",
+        destination_path="destination_path_value",
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.import_data), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.import_data(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == parallelstore.ImportDataRequest(
+            source_gcs_uri="source_gcs_uri_value",
+            destination_path="destination_path_value",
+            name="name_value",
+        )
+
+
+def test_import_data_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ParallelstoreClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.import_data in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.import_data] = mock_rpc
+        request = {}
+        client.import_data(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.import_data(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_import_data_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ParallelstoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.import_data), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/spam")
+        )
+        response = await client.import_data()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == parallelstore.ImportDataRequest()
+
+
+@pytest.mark.asyncio
+async def test_import_data_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = ParallelstoreAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.import_data
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.import_data
+        ] = mock_object
+
+        request = {}
+        await client.import_data(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        await client.import_data(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_import_data_async(
+    transport: str = "grpc_asyncio", request_type=parallelstore.ImportDataRequest
+):
+    client = ParallelstoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.import_data), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/spam")
+        )
+        response = await client.import_data(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        request = parallelstore.ImportDataRequest()
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, future.Future)
+
+
+@pytest.mark.asyncio
+async def test_import_data_async_from_dict():
+    await test_import_data_async(request_type=dict)
+
+
+def test_import_data_field_headers():
+    client = ParallelstoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = parallelstore.ImportDataRequest()
+
+    request.name = "name_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.import_data), "__call__") as call:
+        call.return_value = operations_pb2.Operation(name="operations/op")
+        client.import_data(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_import_data_field_headers_async():
+    client = ParallelstoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = parallelstore.ImportDataRequest()
+
+    request.name = "name_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.import_data), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/op")
+        )
+        await client.import_data(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        parallelstore.ExportDataRequest,
+        dict,
+    ],
+)
+def test_export_data(request_type, transport: str = "grpc"):
+    client = ParallelstoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.export_data), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = operations_pb2.Operation(name="operations/spam")
+        response = client.export_data(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        request = parallelstore.ExportDataRequest()
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, future.Future)
+
+
+def test_export_data_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ParallelstoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.export_data), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.export_data()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == parallelstore.ExportDataRequest()
+
+
+def test_export_data_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ParallelstoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = parallelstore.ExportDataRequest(
+        source_path="source_path_value",
+        destination_gcs_uri="destination_gcs_uri_value",
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.export_data), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.export_data(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == parallelstore.ExportDataRequest(
+            source_path="source_path_value",
+            destination_gcs_uri="destination_gcs_uri_value",
+            name="name_value",
+        )
+
+
+def test_export_data_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ParallelstoreClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.export_data in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.export_data] = mock_rpc
+        request = {}
+        client.export_data(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.export_data(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_export_data_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ParallelstoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.export_data), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/spam")
+        )
+        response = await client.export_data()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == parallelstore.ExportDataRequest()
+
+
+@pytest.mark.asyncio
+async def test_export_data_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = ParallelstoreAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.export_data
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.export_data
+        ] = mock_object
+
+        request = {}
+        await client.export_data(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        await client.export_data(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_export_data_async(
+    transport: str = "grpc_asyncio", request_type=parallelstore.ExportDataRequest
+):
+    client = ParallelstoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.export_data), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/spam")
+        )
+        response = await client.export_data(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        request = parallelstore.ExportDataRequest()
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, future.Future)
+
+
+@pytest.mark.asyncio
+async def test_export_data_async_from_dict():
+    await test_export_data_async(request_type=dict)
+
+
+def test_export_data_field_headers():
+    client = ParallelstoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = parallelstore.ExportDataRequest()
+
+    request.name = "name_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.export_data), "__call__") as call:
+        call.return_value = operations_pb2.Operation(name="operations/op")
+        client.export_data(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_export_data_field_headers_async():
+    client = ParallelstoreAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = parallelstore.ExportDataRequest()
+
+    request.name = "name_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.export_data), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/op")
+        )
+        await client.export_data(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
         parallelstore.ListInstancesRequest,
         dict,
     ],
 )
 def test_list_instances_rest(request_type):
     client = ParallelstoreClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -2558,14 +3868,50 @@
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListInstancesPager)
     assert response.next_page_token == "next_page_token_value"
     assert response.unreachable == ["unreachable_value"]
 
 
+def test_list_instances_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ParallelstoreClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.list_instances in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.list_instances] = mock_rpc
+
+        request = {}
+        client.list_instances(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_instances(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_list_instances_rest_required_fields(
     request_type=parallelstore.ListInstancesRequest,
 ):
     transport_class = transports.ParallelstoreRestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -2890,14 +4236,15 @@
             description="description_value",
             state=parallelstore.Instance.State.CREATING,
             capacity_gib=1247,
             daos_version="daos_version_value",
             access_points=["access_points_value"],
             network="network_value",
             reserved_ip_range="reserved_ip_range_value",
+            effective_reserved_ip_range="effective_reserved_ip_range_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         # Convert return value to protobuf type
         return_value = parallelstore.Instance.pb(return_value)
@@ -2913,14 +4260,51 @@
     assert response.description == "description_value"
     assert response.state == parallelstore.Instance.State.CREATING
     assert response.capacity_gib == 1247
     assert response.daos_version == "daos_version_value"
     assert response.access_points == ["access_points_value"]
     assert response.network == "network_value"
     assert response.reserved_ip_range == "reserved_ip_range_value"
+    assert response.effective_reserved_ip_range == "effective_reserved_ip_range_value"
+
+
+def test_get_instance_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ParallelstoreClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.get_instance in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.get_instance] = mock_rpc
+
+        request = {}
+        client.get_instance(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_instance(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
 
 
 def test_get_instance_rest_required_fields(
     request_type=parallelstore.GetInstanceRequest,
 ):
     transport_class = transports.ParallelstoreRestTransport
 
@@ -3171,14 +4555,15 @@
         "update_time": {},
         "labels": {},
         "capacity_gib": 1247,
         "daos_version": "daos_version_value",
         "access_points": ["access_points_value1", "access_points_value2"],
         "network": "network_value",
         "reserved_ip_range": "reserved_ip_range_value",
+        "effective_reserved_ip_range": "effective_reserved_ip_range_value",
     }
     # The version of a generated dependency at test runtime may differ from the version used during generation.
     # Delete any fields which are not present in the current runtime dependency
     # See https://github.com/googleapis/gapic-generator-python/issues/1748
 
     # Determine if the message type is proto-plus or protobuf
     test_field = parallelstore.CreateInstanceRequest.meta.fields["instance"]
@@ -3259,14 +4644,54 @@
         req.return_value = response_value
         response = client.create_instance(request)
 
     # Establish that the response is the type that we expect.
     assert response.operation.name == "operations/spam"
 
 
+def test_create_instance_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ParallelstoreClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.create_instance in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.create_instance] = mock_rpc
+
+        request = {}
+        client.create_instance(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.create_instance(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_create_instance_rest_required_fields(
     request_type=parallelstore.CreateInstanceRequest,
 ):
     transport_class = transports.ParallelstoreRestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -3551,14 +4976,15 @@
         "update_time": {},
         "labels": {},
         "capacity_gib": 1247,
         "daos_version": "daos_version_value",
         "access_points": ["access_points_value1", "access_points_value2"],
         "network": "network_value",
         "reserved_ip_range": "reserved_ip_range_value",
+        "effective_reserved_ip_range": "effective_reserved_ip_range_value",
     }
     # The version of a generated dependency at test runtime may differ from the version used during generation.
     # Delete any fields which are not present in the current runtime dependency
     # See https://github.com/googleapis/gapic-generator-python/issues/1748
 
     # Determine if the message type is proto-plus or protobuf
     test_field = parallelstore.UpdateInstanceRequest.meta.fields["instance"]
@@ -3639,14 +5065,54 @@
         req.return_value = response_value
         response = client.update_instance(request)
 
     # Establish that the response is the type that we expect.
     assert response.operation.name == "operations/spam"
 
 
+def test_update_instance_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ParallelstoreClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.update_instance in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.update_instance] = mock_rpc
+
+        request = {}
+        client.update_instance(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.update_instance(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_update_instance_rest_required_fields(
     request_type=parallelstore.UpdateInstanceRequest,
 ):
     transport_class = transports.ParallelstoreRestTransport
 
     request_init = {}
     request = request_type(**request_init)
@@ -3920,14 +5386,54 @@
         req.return_value = response_value
         response = client.delete_instance(request)
 
     # Establish that the response is the type that we expect.
     assert response.operation.name == "operations/spam"
 
 
+def test_delete_instance_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ParallelstoreClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.delete_instance in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.delete_instance] = mock_rpc
+
+        request = {}
+        client.delete_instance(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.delete_instance(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_delete_instance_rest_required_fields(
     request_type=parallelstore.DeleteInstanceRequest,
 ):
     transport_class = transports.ParallelstoreRestTransport
 
     request_init = {}
     request_init["name"] = ""
@@ -4148,14 +5654,500 @@
 
 def test_delete_instance_rest_error():
     client = ParallelstoreClient(
         credentials=ga_credentials.AnonymousCredentials(), transport="rest"
     )
 
 
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        parallelstore.ImportDataRequest,
+        dict,
+    ],
+)
+def test_import_data_rest(request_type):
+    client = ParallelstoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {"name": "projects/sample1/locations/sample2/instances/sample3"}
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = operations_pb2.Operation(name="operations/spam")
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.import_data(request)
+
+    # Establish that the response is the type that we expect.
+    assert response.operation.name == "operations/spam"
+
+
+def test_import_data_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ParallelstoreClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.import_data in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.import_data] = mock_rpc
+
+        request = {}
+        client.import_data(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.import_data(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+def test_import_data_rest_required_fields(request_type=parallelstore.ImportDataRequest):
+    transport_class = transports.ParallelstoreRestTransport
+
+    request_init = {}
+    request_init["name"] = ""
+    request = request_type(**request_init)
+    pb_request = request_type.pb(request)
+    jsonified_request = json.loads(
+        json_format.MessageToJson(pb_request, use_integers_for_enums=False)
+    )
+
+    # verify fields with default values are dropped
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).import_data._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with default values are now present
+
+    jsonified_request["name"] = "name_value"
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).import_data._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with non-default values are left alone
+    assert "name" in jsonified_request
+    assert jsonified_request["name"] == "name_value"
+
+    client = ParallelstoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request = request_type(**request_init)
+
+    # Designate an appropriate value for the returned response.
+    return_value = operations_pb2.Operation(name="operations/spam")
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(Session, "request") as req:
+        # We need to mock transcode() because providing default values
+        # for required fields will fail the real version if the http_options
+        # expect actual values for those fields.
+        with mock.patch.object(path_template, "transcode") as transcode:
+            # A uri without fields and an empty body will force all the
+            # request fields to show up in the query_params.
+            pb_request = request_type.pb(request)
+            transcode_result = {
+                "uri": "v1/sample_method",
+                "method": "post",
+                "query_params": pb_request,
+            }
+            transcode_result["body"] = pb_request
+            transcode.return_value = transcode_result
+
+            response_value = Response()
+            response_value.status_code = 200
+            json_return_value = json_format.MessageToJson(return_value)
+
+            response_value._content = json_return_value.encode("UTF-8")
+            req.return_value = response_value
+
+            response = client.import_data(request)
+
+            expected_params = [("$alt", "json;enum-encoding=int")]
+            actual_params = req.call_args.kwargs["params"]
+            assert expected_params == actual_params
+
+
+def test_import_data_rest_unset_required_fields():
+    transport = transports.ParallelstoreRestTransport(
+        credentials=ga_credentials.AnonymousCredentials
+    )
+
+    unset_fields = transport.import_data._get_unset_required_fields({})
+    assert set(unset_fields) == (set(()) & set(("name",)))
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_import_data_rest_interceptors(null_interceptor):
+    transport = transports.ParallelstoreRestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.ParallelstoreRestInterceptor(),
+    )
+    client = ParallelstoreClient(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        operation.Operation, "_set_result_from_operation"
+    ), mock.patch.object(
+        transports.ParallelstoreRestInterceptor, "post_import_data"
+    ) as post, mock.patch.object(
+        transports.ParallelstoreRestInterceptor, "pre_import_data"
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = parallelstore.ImportDataRequest.pb(
+            parallelstore.ImportDataRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = json_format.MessageToJson(
+            operations_pb2.Operation()
+        )
+
+        request = parallelstore.ImportDataRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = operations_pb2.Operation()
+
+        client.import_data(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_import_data_rest_bad_request(
+    transport: str = "rest", request_type=parallelstore.ImportDataRequest
+):
+    client = ParallelstoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {"name": "projects/sample1/locations/sample2/instances/sample3"}
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.import_data(request)
+
+
+def test_import_data_rest_error():
+    client = ParallelstoreClient(
+        credentials=ga_credentials.AnonymousCredentials(), transport="rest"
+    )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        parallelstore.ExportDataRequest,
+        dict,
+    ],
+)
+def test_export_data_rest(request_type):
+    client = ParallelstoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {"name": "projects/sample1/locations/sample2/instances/sample3"}
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = operations_pb2.Operation(name="operations/spam")
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.export_data(request)
+
+    # Establish that the response is the type that we expect.
+    assert response.operation.name == "operations/spam"
+
+
+def test_export_data_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ParallelstoreClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.export_data in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.export_data] = mock_rpc
+
+        request = {}
+        client.export_data(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.export_data(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+def test_export_data_rest_required_fields(request_type=parallelstore.ExportDataRequest):
+    transport_class = transports.ParallelstoreRestTransport
+
+    request_init = {}
+    request_init["name"] = ""
+    request = request_type(**request_init)
+    pb_request = request_type.pb(request)
+    jsonified_request = json.loads(
+        json_format.MessageToJson(pb_request, use_integers_for_enums=False)
+    )
+
+    # verify fields with default values are dropped
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).export_data._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with default values are now present
+
+    jsonified_request["name"] = "name_value"
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).export_data._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with non-default values are left alone
+    assert "name" in jsonified_request
+    assert jsonified_request["name"] == "name_value"
+
+    client = ParallelstoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request = request_type(**request_init)
+
+    # Designate an appropriate value for the returned response.
+    return_value = operations_pb2.Operation(name="operations/spam")
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(Session, "request") as req:
+        # We need to mock transcode() because providing default values
+        # for required fields will fail the real version if the http_options
+        # expect actual values for those fields.
+        with mock.patch.object(path_template, "transcode") as transcode:
+            # A uri without fields and an empty body will force all the
+            # request fields to show up in the query_params.
+            pb_request = request_type.pb(request)
+            transcode_result = {
+                "uri": "v1/sample_method",
+                "method": "post",
+                "query_params": pb_request,
+            }
+            transcode_result["body"] = pb_request
+            transcode.return_value = transcode_result
+
+            response_value = Response()
+            response_value.status_code = 200
+            json_return_value = json_format.MessageToJson(return_value)
+
+            response_value._content = json_return_value.encode("UTF-8")
+            req.return_value = response_value
+
+            response = client.export_data(request)
+
+            expected_params = [("$alt", "json;enum-encoding=int")]
+            actual_params = req.call_args.kwargs["params"]
+            assert expected_params == actual_params
+
+
+def test_export_data_rest_unset_required_fields():
+    transport = transports.ParallelstoreRestTransport(
+        credentials=ga_credentials.AnonymousCredentials
+    )
+
+    unset_fields = transport.export_data._get_unset_required_fields({})
+    assert set(unset_fields) == (set(()) & set(("name",)))
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_export_data_rest_interceptors(null_interceptor):
+    transport = transports.ParallelstoreRestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.ParallelstoreRestInterceptor(),
+    )
+    client = ParallelstoreClient(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        operation.Operation, "_set_result_from_operation"
+    ), mock.patch.object(
+        transports.ParallelstoreRestInterceptor, "post_export_data"
+    ) as post, mock.patch.object(
+        transports.ParallelstoreRestInterceptor, "pre_export_data"
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = parallelstore.ExportDataRequest.pb(
+            parallelstore.ExportDataRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = json_format.MessageToJson(
+            operations_pb2.Operation()
+        )
+
+        request = parallelstore.ExportDataRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = operations_pb2.Operation()
+
+        client.export_data(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_export_data_rest_bad_request(
+    transport: str = "rest", request_type=parallelstore.ExportDataRequest
+):
+    client = ParallelstoreClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {"name": "projects/sample1/locations/sample2/instances/sample3"}
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.export_data(request)
+
+
+def test_export_data_rest_error():
+    client = ParallelstoreClient(
+        credentials=ga_credentials.AnonymousCredentials(), transport="rest"
+    )
+
+
 def test_credentials_transport_error():
     # It is an error to provide credentials and a transport instance.
     transport = transports.ParallelstoreGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
         client = ParallelstoreClient(
@@ -4292,14 +6284,16 @@
     # raise NotImplementedError.
     methods = (
         "list_instances",
         "get_instance",
         "create_instance",
         "update_instance",
         "delete_instance",
+        "import_data",
+        "export_data",
         "get_location",
         "list_locations",
         "get_operation",
         "cancel_operation",
         "delete_operation",
         "list_operations",
     )
@@ -4593,14 +6587,20 @@
     assert session1 != session2
     session1 = client1.transport.update_instance._session
     session2 = client2.transport.update_instance._session
     assert session1 != session2
     session1 = client1.transport.delete_instance._session
     session2 = client2.transport.delete_instance._session
     assert session1 != session2
+    session1 = client1.transport.import_data._session
+    session2 = client2.transport.import_data._session
+    assert session1 != session2
+    session1 = client1.transport.export_data._session
+    session2 = client2.transport.export_data._session
+    assert session1 != session2
 
 
 def test_parallelstore_grpc_transport_channel():
     channel = grpc.secure_channel("http://localhost/", grpc.local_channel_credentials())
 
     # Check that channel is used if provided.
     transport = transports.ParallelstoreGrpcTransport(
```

