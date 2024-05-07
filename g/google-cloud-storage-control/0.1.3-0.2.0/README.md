# Comparing `tmp/google-cloud-storage-control-0.1.3.tar.gz` & `tmp/google-cloud-storage-control-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-storage-control-0.1.3.tar", last modified: Fri Apr 19 00:24:45 2024, max compression
+gzip compressed data, was "google-cloud-storage-control-0.2.0.tar", last modified: Tue May  7 20:43:55 2024, max compression
```

## Comparing `google-cloud-storage-control-0.1.3.tar` & `google-cloud-storage-control-0.2.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.149651 google-cloud-storage-control-0.1.3/
--rw-rw-r--   0 root         (0)     1003    11358 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5526 2024-04-19 00:24:45.149651 google-cloud-storage-control-0.1.3/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4138 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.141650 google-cloud-storage-control-0.1.3/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.141650 google-cloud-storage-control-0.1.3/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.141650 google-cloud-storage-control-0.1.3/google/cloud/storage_control/
--rw-rw-r--   0 root         (0)     1003     2064 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.145651 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/
--rw-rw-r--   0 root         (0)     1003     1899 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003     3061 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.145651 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.145651 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/
--rw-rw-r--   0 root         (0)     1003      769 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/__init__.py
--rw-rw-r--   0 root         (0)     1003    61018 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/async_client.py
--rw-rw-r--   0 root         (0)     1003    81394 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/client.py
--rw-rw-r--   0 root         (0)     1003    11060 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.145651 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/transports/
--rw-rw-r--   0 root         (0)     1003     1193 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    14186 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/transports/base.py
--rw-rw-r--   0 root         (0)     1003    23737 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    24277 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.145651 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/types/
--rw-rw-r--   0 root         (0)     1003     1624 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    28587 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/types/storage_control.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.149651 google-cloud-storage-control-0.1.3/google_cloud_storage_control.egg-info/
--rw-r--r--   0 root         (0)     1003     5526 2024-04-19 00:24:45.000000 google-cloud-storage-control-0.1.3/google_cloud_storage_control.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1590 2024-04-19 00:24:45.000000 google-cloud-storage-control-0.1.3/google_cloud_storage_control.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-19 00:24:45.000000 google-cloud-storage-control-0.1.3/google_cloud_storage_control.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-19 00:24:45.000000 google-cloud-storage-control-0.1.3/google_cloud_storage_control.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      305 2024-04-19 00:24:45.000000 google-cloud-storage-control-0.1.3/google_cloud_storage_control.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-04-19 00:24:45.000000 google-cloud-storage-control-0.1.3/google_cloud_storage_control.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-04-19 00:24:45.149651 google-cloud-storage-control-0.1.3/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3201 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.149651 google-cloud-storage-control-0.1.3/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.149651 google-cloud-storage-control-0.1.3/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.149651 google-cloud-storage-control-0.1.3/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.149651 google-cloud-storage-control-0.1.3/tests/unit/gapic/storage_control_v2/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/tests/unit/gapic/storage_control_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003   194411 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/tests/unit/gapic/storage_control_v2/test_storage_control.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:55.574279 google-cloud-storage-control-0.2.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-05-07 20:40:13.000000 google-cloud-storage-control-0.2.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-05-07 20:40:13.000000 google-cloud-storage-control-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5526 2024-05-07 20:43:55.574279 google-cloud-storage-control-0.2.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4138 2024-05-07 20:40:13.000000 google-cloud-storage-control-0.2.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:55.562277 google-cloud-storage-control-0.2.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:55.562277 google-cloud-storage-control-0.2.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:55.566278 google-cloud-storage-control-0.2.0/google/cloud/storage_control/
+-rw-rw-r--   0 root         (0)     1003     2064 2024-05-07 20:40:13.000000 google-cloud-storage-control-0.2.0/google/cloud/storage_control/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-07 20:40:13.000000 google-cloud-storage-control-0.2.0/google/cloud/storage_control/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2024-05-07 20:40:13.000000 google-cloud-storage-control-0.2.0/google/cloud/storage_control/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:55.566278 google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/
+-rw-rw-r--   0 root         (0)     1003     1899 2024-05-07 20:40:13.000000 google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3061 2024-05-07 20:40:13.000000 google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-07 20:40:13.000000 google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2024-05-07 20:40:13.000000 google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:55.570278 google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:13.000000 google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:55.570278 google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/services/storage_control/
+-rw-rw-r--   0 root         (0)     1003      769 2024-05-07 20:40:13.000000 google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/services/storage_control/__init__.py
+-rw-rw-r--   0 root         (0)     1003    59862 2024-05-07 20:40:13.000000 google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/services/storage_control/async_client.py
+-rw-rw-r--   0 root         (0)     1003    81188 2024-05-07 20:40:13.000000 google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/services/storage_control/client.py
+-rw-rw-r--   0 root         (0)     1003    11060 2024-05-07 20:40:13.000000 google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/services/storage_control/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:55.570278 google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/services/storage_control/transports/
+-rw-rw-r--   0 root         (0)     1003     1193 2024-05-07 20:40:13.000000 google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/services/storage_control/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14186 2024-05-07 20:40:13.000000 google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/services/storage_control/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    24284 2024-05-07 20:40:13.000000 google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/services/storage_control/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    30508 2024-05-07 20:40:13.000000 google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/services/storage_control/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:55.570278 google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/types/
+-rw-rw-r--   0 root         (0)     1003     1624 2024-05-07 20:40:13.000000 google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    28587 2024-05-07 20:40:13.000000 google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/types/storage_control.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:55.574279 google-cloud-storage-control-0.2.0/google_cloud_storage_control.egg-info/
+-rw-r--r--   0 root         (0)     1003     5526 2024-05-07 20:43:55.000000 google-cloud-storage-control-0.2.0/google_cloud_storage_control.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1590 2024-05-07 20:43:55.000000 google-cloud-storage-control-0.2.0/google_cloud_storage_control.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-07 20:43:55.000000 google-cloud-storage-control-0.2.0/google_cloud_storage_control.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-07 20:43:55.000000 google-cloud-storage-control-0.2.0/google_cloud_storage_control.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      305 2024-05-07 20:43:55.000000 google-cloud-storage-control-0.2.0/google_cloud_storage_control.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-05-07 20:43:55.000000 google-cloud-storage-control-0.2.0/google_cloud_storage_control.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-05-07 20:43:55.574279 google-cloud-storage-control-0.2.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3201 2024-05-07 20:40:13.000000 google-cloud-storage-control-0.2.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:55.574279 google-cloud-storage-control-0.2.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:13.000000 google-cloud-storage-control-0.2.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:55.574279 google-cloud-storage-control-0.2.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:13.000000 google-cloud-storage-control-0.2.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:55.574279 google-cloud-storage-control-0.2.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:13.000000 google-cloud-storage-control-0.2.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:55.574279 google-cloud-storage-control-0.2.0/tests/unit/gapic/storage_control_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:13.000000 google-cloud-storage-control-0.2.0/tests/unit/gapic/storage_control_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   226482 2024-05-07 20:40:13.000000 google-cloud-storage-control-0.2.0/tests/unit/gapic/storage_control_v2/test_storage_control.py
```

### Comparing `google-cloud-storage-control-0.1.3/LICENSE` & `google-cloud-storage-control-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.3/MANIFEST.in` & `google-cloud-storage-control-0.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.3/PKG-INFO` & `google-cloud-storage-control-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-storage-control
-Version: 0.1.3
+Version: 0.2.0
 Summary: Google Cloud Storage Control API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-storage-control
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-storage-control-0.1.3/README.rst` & `google-cloud-storage-control-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.3/google/cloud/storage_control/__init__.py` & `google-cloud-storage-control-0.2.0/google/cloud/storage_control/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.3/google/cloud/storage_control/gapic_version.py` & `google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/services/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.3"  # {x-release-please-version}
```

### Comparing `google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/__init__.py` & `google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/gapic_metadata.json` & `google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/gapic_version.py` & `google-cloud-storage-control-0.2.0/tests/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.3"  # {x-release-please-version}
```

### Comparing `google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/__init__.py` & `google-cloud-storage-control-0.2.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/__init__.py` & `google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/services/storage_control/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/async_client.py` & `google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/services/storage_control/async_client.py`

 * *Files 7% similar despite different names*

```diff
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
@@ -206,29 +207,33 @@
         type(StorageControlClient).get_transport_class, type(StorageControlClient)
     )
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, StorageControlTransport] = "grpc_asyncio",
+        transport: Optional[
+            Union[str, StorageControlTransport, Callable[..., StorageControlTransport]]
+        ] = "grpc_asyncio",
         client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the storage control async client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, ~.StorageControlTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,StorageControlTransport,Callable[..., StorageControlTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport to use.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the StorageControlTransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -357,41 +362,42 @@
                 A folder resource. This resource can
                 only exist in a hierarchical namespace
                 enabled bucket. Hierarchical namespace
                 buckets are in allowlist preview.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, folder, folder_id])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = storage_control.CreateFolderRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, storage_control.CreateFolderRequest):
+            request = storage_control.CreateFolderRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
         if folder is not None:
             request.folder = folder
         if folder_id is not None:
             request.folder_id = folder_id
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.create_folder,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.create_folder
+        ]
 
         if not request.request_id:
             request.request_id = str(uuid.uuid4())
 
         # Validate the universe domain.
         self._client._validate_universe_domain()
 
@@ -460,37 +466,38 @@
             retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
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
 
-        request = storage_control.DeleteFolderRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, storage_control.DeleteFolderRequest):
+            request = storage_control.DeleteFolderRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.delete_folder,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.delete_folder
+        ]
 
         if not request.request_id:
             request.request_id = str(uuid.uuid4())
 
         # Validate the universe domain.
         self._client._validate_universe_domain()
 
@@ -567,50 +574,38 @@
                 A folder resource. This resource can
                 only exist in a hierarchical namespace
                 enabled bucket. Hierarchical namespace
                 buckets are in allowlist preview.
 
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
 
-        request = storage_control.GetFolderRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, storage_control.GetFolderRequest):
+            request = storage_control.GetFolderRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.get_folder,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=60.0,
-                multiplier=2,
-                predicate=retries.if_exception_type(
-                    core_exceptions.DeadlineExceeded,
-                    core_exceptions.InternalServerError,
-                    core_exceptions.ResourceExhausted,
-                    core_exceptions.ServiceUnavailable,
-                    core_exceptions.Unknown,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.get_folder
+        ]
 
         if not request.request_id:
             request.request_id = str(uuid.uuid4())
 
         # Validate the universe domain.
         self._client._validate_universe_domain()
 
@@ -692,50 +687,38 @@
 
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
 
-        request = storage_control.ListFoldersRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, storage_control.ListFoldersRequest):
+            request = storage_control.ListFoldersRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.list_folders,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=60.0,
-                multiplier=2,
-                predicate=retries.if_exception_type(
-                    core_exceptions.DeadlineExceeded,
-                    core_exceptions.InternalServerError,
-                    core_exceptions.ResourceExhausted,
-                    core_exceptions.ServiceUnavailable,
-                    core_exceptions.Unknown,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.list_folders
+        ]
 
         # Validate the universe domain.
         self._client._validate_universe_domain()
 
         # Send the request.
         response = await rpc(
             request,
@@ -836,52 +819,40 @@
 
                 The result type for the operation will be :class:`google.cloud.storage_control_v2.types.Folder` A folder resource. This resource can only exist in a hierarchical namespace
                    enabled bucket. Hierarchical namespace buckets are in
                    allowlist preview.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name, destination_folder_id])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = storage_control.RenameFolderRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, storage_control.RenameFolderRequest):
+            request = storage_control.RenameFolderRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
         if destination_folder_id is not None:
             request.destination_folder_id = destination_folder_id
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.rename_folder,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=60.0,
-                multiplier=2,
-                predicate=retries.if_exception_type(
-                    core_exceptions.DeadlineExceeded,
-                    core_exceptions.InternalServerError,
-                    core_exceptions.ResourceExhausted,
-                    core_exceptions.ServiceUnavailable,
-                    core_exceptions.Unknown,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.rename_folder
+        ]
 
         if not request.request_id:
             request.request_id = str(uuid.uuid4())
 
         # Validate the universe domain.
         self._client._validate_universe_domain()
 
@@ -962,50 +933,38 @@
         Returns:
             google.cloud.storage_control_v2.types.StorageLayout:
                 The storage layout configuration of a
                 bucket.
 
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
 
-        request = storage_control.GetStorageLayoutRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, storage_control.GetStorageLayoutRequest):
+            request = storage_control.GetStorageLayoutRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.get_storage_layout,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=60.0,
-                multiplier=2,
-                predicate=retries.if_exception_type(
-                    core_exceptions.DeadlineExceeded,
-                    core_exceptions.InternalServerError,
-                    core_exceptions.ResourceExhausted,
-                    core_exceptions.ServiceUnavailable,
-                    core_exceptions.Unknown,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.get_storage_layout
+        ]
 
         if not request.request_id:
             request.request_id = str(uuid.uuid4())
 
         # Validate the universe domain.
         self._client._validate_universe_domain()
 
@@ -1098,41 +1057,42 @@
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.storage_control_v2.types.ManagedFolder:
                 A managed folder.
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, managed_folder, managed_folder_id])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = storage_control.CreateManagedFolderRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, storage_control.CreateManagedFolderRequest):
+            request = storage_control.CreateManagedFolderRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
         if managed_folder is not None:
             request.managed_folder = managed_folder
         if managed_folder_id is not None:
             request.managed_folder_id = managed_folder_id
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.create_managed_folder,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.create_managed_folder
+        ]
 
         if not request.request_id:
             request.request_id = str(uuid.uuid4())
 
         # Validate the universe domain.
         self._client._validate_universe_domain()
 
@@ -1197,37 +1157,38 @@
             retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
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
 
-        request = storage_control.DeleteManagedFolderRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, storage_control.DeleteManagedFolderRequest):
+            request = storage_control.DeleteManagedFolderRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.delete_managed_folder,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.delete_managed_folder
+        ]
 
         if not request.request_id:
             request.request_id = str(uuid.uuid4())
 
         # Validate the universe domain.
         self._client._validate_universe_domain()
 
@@ -1293,50 +1254,38 @@
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.storage_control_v2.types.ManagedFolder:
                 A managed folder.
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
 
-        request = storage_control.GetManagedFolderRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, storage_control.GetManagedFolderRequest):
+            request = storage_control.GetManagedFolderRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.get_managed_folder,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=60.0,
-                multiplier=2,
-                predicate=retries.if_exception_type(
-                    core_exceptions.DeadlineExceeded,
-                    core_exceptions.InternalServerError,
-                    core_exceptions.ResourceExhausted,
-                    core_exceptions.ServiceUnavailable,
-                    core_exceptions.Unknown,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.get_managed_folder
+        ]
 
         if not request.request_id:
             request.request_id = str(uuid.uuid4())
 
         # Validate the universe domain.
         self._client._validate_universe_domain()
 
@@ -1415,50 +1364,38 @@
                 ListManagedFolders.
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
 
-        request = storage_control.ListManagedFoldersRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, storage_control.ListManagedFoldersRequest):
+            request = storage_control.ListManagedFoldersRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.list_managed_folders,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=60.0,
-                multiplier=2,
-                predicate=retries.if_exception_type(
-                    core_exceptions.DeadlineExceeded,
-                    core_exceptions.InternalServerError,
-                    core_exceptions.ResourceExhausted,
-                    core_exceptions.ServiceUnavailable,
-                    core_exceptions.Unknown,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.list_managed_folders
+        ]
 
         if not request.request_id:
             request.request_id = str(uuid.uuid4())
 
         # Validate the universe domain.
         self._client._validate_universe_domain()
```

### Comparing `google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/client.py` & `google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/services/storage_control/client.py`

 * *Files 2% similar despite different names*

```diff
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
@@ -210,30 +211,28 @@
         )
         return m.groupdict() if m else {}
 
     @staticmethod
     def managed_folder_path(
         project: str,
         bucket: str,
-        managedFolder: str,
+        managed_folder: str,
     ) -> str:
         """Returns a fully-qualified managed_folder string."""
-        return (
-            "projects/{project}/buckets/{bucket}/managedFolders/{managedFolder}".format(
-                project=project,
-                bucket=bucket,
-                managedFolder=managedFolder,
-            )
+        return "projects/{project}/buckets/{bucket}/managedFolders/{managed_folder}".format(
+            project=project,
+            bucket=bucket,
+            managed_folder=managed_folder,
         )
 
     @staticmethod
     def parse_managed_folder_path(path: str) -> Dict[str, str]:
         """Parses a managed_folder path into its component segments."""
         m = re.match(
-            r"^projects/(?P<project>.+?)/buckets/(?P<bucket>.+?)/managedFolders/(?P<managedFolder>.+?)$",
+            r"^projects/(?P<project>.+?)/buckets/(?P<bucket>.+?)/managedFolders/(?P<managed_folder>.+?)$",
             path,
         )
         return m.groupdict() if m else {}
 
     @staticmethod
     def storage_layout_path(
         project: str,
@@ -574,29 +573,33 @@
         """
         return self._universe_domain
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Optional[Union[str, StorageControlTransport]] = None,
+        transport: Optional[
+            Union[str, StorageControlTransport, Callable[..., StorageControlTransport]]
+        ] = None,
         client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the storage control client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, StorageControlTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,StorageControlTransport,Callable[..., StorageControlTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the StorageControlTransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -697,16 +700,23 @@
             if api_key_value and hasattr(
                 google.auth._default, "get_api_key_credentials"
             ):
                 credentials = google.auth._default.get_api_key_credentials(
                     api_key_value
                 )
 
-            Transport = type(self).get_transport_class(cast(str, transport))
-            self._transport = Transport(
+            transport_init: Union[
+                Type[StorageControlTransport], Callable[..., StorageControlTransport]
+            ] = (
+                type(self).get_transport_class(transport)
+                if isinstance(transport, str) or transport is None
+                else cast(Callable[..., StorageControlTransport], transport)
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
@@ -803,27 +813,25 @@
                 A folder resource. This resource can
                 only exist in a hierarchical namespace
                 enabled bucket. Hierarchical namespace
                 buckets are in allowlist preview.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, folder, folder_id])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a storage_control.CreateFolderRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, storage_control.CreateFolderRequest):
             request = storage_control.CreateFolderRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if parent is not None:
                 request.parent = parent
             if folder is not None:
@@ -918,27 +926,25 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
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
-        # in a storage_control.DeleteFolderRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, storage_control.DeleteFolderRequest):
             request = storage_control.DeleteFolderRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
 
@@ -1039,27 +1045,25 @@
                 A folder resource. This resource can
                 only exist in a hierarchical namespace
                 enabled bucket. Hierarchical namespace
                 buckets are in allowlist preview.
 
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
-        # in a storage_control.GetFolderRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, storage_control.GetFolderRequest):
             request = storage_control.GetFolderRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
 
@@ -1165,27 +1169,25 @@
 
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
-        # in a storage_control.ListFoldersRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, storage_control.ListFoldersRequest):
             request = storage_control.ListFoldersRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if parent is not None:
                 request.parent = parent
 
@@ -1308,27 +1310,25 @@
 
                 The result type for the operation will be :class:`google.cloud.storage_control_v2.types.Folder` A folder resource. This resource can only exist in a hierarchical namespace
                    enabled bucket. Hierarchical namespace buckets are in
                    allowlist preview.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name, destination_folder_id])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a storage_control.RenameFolderRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, storage_control.RenameFolderRequest):
             request = storage_control.RenameFolderRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
             if destination_folder_id is not None:
@@ -1435,27 +1435,25 @@
         Returns:
             google.cloud.storage_control_v2.types.StorageLayout:
                 The storage layout configuration of a
                 bucket.
 
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
-        # in a storage_control.GetStorageLayoutRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, storage_control.GetStorageLayoutRequest):
             request = storage_control.GetStorageLayoutRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
 
@@ -1572,27 +1570,25 @@
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.storage_control_v2.types.ManagedFolder:
                 A managed folder.
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, managed_folder, managed_folder_id])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a storage_control.CreateManagedFolderRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, storage_control.CreateManagedFolderRequest):
             request = storage_control.CreateManagedFolderRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if parent is not None:
                 request.parent = parent
             if managed_folder is not None:
@@ -1683,27 +1679,25 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
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
-        # in a storage_control.DeleteManagedFolderRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, storage_control.DeleteManagedFolderRequest):
             request = storage_control.DeleteManagedFolderRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
 
@@ -1793,27 +1787,25 @@
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.storage_control_v2.types.ManagedFolder:
                 A managed folder.
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
-        # in a storage_control.GetManagedFolderRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, storage_control.GetManagedFolderRequest):
             request = storage_control.GetManagedFolderRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
 
@@ -1916,27 +1908,25 @@
                 ListManagedFolders.
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
-        # in a storage_control.ListManagedFoldersRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, storage_control.ListManagedFoldersRequest):
             request = storage_control.ListManagedFoldersRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if parent is not None:
                 request.parent = parent
```

### Comparing `google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/pagers.py` & `google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/services/storage_control/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/transports/__init__.py` & `google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/services/storage_control/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/transports/base.py` & `google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/services/storage_control/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/transports/grpc.py` & `google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/services/storage_control/transports/grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     def __init__(
         self,
         *,
         host: str = "storage.googleapis.com",
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
@@ -68,36 +68,39 @@
             host (Optional[str]):
                  The hostname to connect to (default: 'storage.googleapis.com').
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
@@ -116,15 +119,15 @@
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
@@ -157,15 +160,17 @@
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
```

### Comparing `google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/types/__init__.py` & `google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/types/storage_control.py` & `google-cloud-storage-control-0.2.0/google/cloud/storage_control_v2/types/storage_control.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.3/google_cloud_storage_control.egg-info/PKG-INFO` & `google-cloud-storage-control-0.2.0/google_cloud_storage_control.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-storage-control
-Version: 0.1.3
+Version: 0.2.0
 Summary: Google Cloud Storage Control API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-storage-control
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-storage-control-0.1.3/google_cloud_storage_control.egg-info/SOURCES.txt` & `google-cloud-storage-control-0.2.0/google_cloud_storage_control.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.3/setup.py` & `google-cloud-storage-control-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.3/tests/__init__.py` & `google-cloud-storage-control-0.2.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.3/tests/unit/__init__.py` & `google-cloud-storage-control-0.2.0/tests/unit/gapic/storage_control_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.3/tests/unit/gapic/storage_control_v2/test_storage_control.py` & `google-cloud-storage-control-0.2.0/tests/unit/gapic/storage_control_v2/test_storage_control.py`

 * *Files 6% similar despite different names*

```diff
@@ -1160,14 +1160,17 @@
     client = StorageControlClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_folder), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.create_folder()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         # Ensure that the uuid4 field is set according to AIP 4235
         assert re.match(
             r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
             args[0].request_id,
@@ -1191,14 +1194,17 @@
     request = storage_control.CreateFolderRequest(
         parent="parent_value",
         folder_id="folder_id_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_folder), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.create_folder(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         # Ensure that the uuid4 field is set according to AIP 4235
         assert re.match(
             r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
             args[0].request_id,
@@ -1207,14 +1213,49 @@
         args[0].request_id = None
         assert args[0] == storage_control.CreateFolderRequest(
             parent="parent_value",
             folder_id="folder_id_value",
         )
 
 
+def test_create_folder_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = StorageControlClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.create_folder in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.create_folder] = mock_rpc
+        request = {}
+        client.create_folder(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.create_folder(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_create_folder_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = StorageControlAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -1239,14 +1280,60 @@
         )
         # clear UUID field so that the check below succeeds
         args[0].request_id = None
         assert args[0] == storage_control.CreateFolderRequest()
 
 
 @pytest.mark.asyncio
+async def test_create_folder_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = StorageControlAsyncClient(
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
+            client._client._transport.create_folder
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
+            client._client._transport.create_folder
+        ] = mock_object
+
+        request = {}
+        await client.create_folder(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.create_folder(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_create_folder_async(
     transport: str = "grpc_asyncio", request_type=storage_control.CreateFolderRequest
 ):
     client = StorageControlAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -1458,14 +1545,17 @@
     client = StorageControlClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.delete_folder), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.delete_folder()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         # Ensure that the uuid4 field is set according to AIP 4235
         assert re.match(
             r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
             args[0].request_id,
@@ -1488,14 +1578,17 @@
     # if they meet the requirements of AIP 4235.
     request = storage_control.DeleteFolderRequest(
         name="name_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.delete_folder), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.delete_folder(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         # Ensure that the uuid4 field is set according to AIP 4235
         assert re.match(
             r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
             args[0].request_id,
@@ -1503,14 +1596,49 @@
         # clear UUID field so that the check below succeeds
         args[0].request_id = None
         assert args[0] == storage_control.DeleteFolderRequest(
             name="name_value",
         )
 
 
+def test_delete_folder_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = StorageControlClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.delete_folder in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.delete_folder] = mock_rpc
+        request = {}
+        client.delete_folder(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.delete_folder(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_delete_folder_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = StorageControlAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -1530,14 +1658,60 @@
         )
         # clear UUID field so that the check below succeeds
         args[0].request_id = None
         assert args[0] == storage_control.DeleteFolderRequest()
 
 
 @pytest.mark.asyncio
+async def test_delete_folder_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = StorageControlAsyncClient(
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
+            client._client._transport.delete_folder
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
+            client._client._transport.delete_folder
+        ] = mock_object
+
+        request = {}
+        await client.delete_folder(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.delete_folder(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_delete_folder_async(
     transport: str = "grpc_asyncio", request_type=storage_control.DeleteFolderRequest
 ):
     client = StorageControlAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -1727,14 +1901,17 @@
     client = StorageControlClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_folder), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_folder()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         # Ensure that the uuid4 field is set according to AIP 4235
         assert re.match(
             r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
             args[0].request_id,
@@ -1757,14 +1934,17 @@
     # if they meet the requirements of AIP 4235.
     request = storage_control.GetFolderRequest(
         name="name_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_folder), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_folder(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         # Ensure that the uuid4 field is set according to AIP 4235
         assert re.match(
             r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
             args[0].request_id,
@@ -1772,14 +1952,49 @@
         # clear UUID field so that the check below succeeds
         args[0].request_id = None
         assert args[0] == storage_control.GetFolderRequest(
             name="name_value",
         )
 
 
+def test_get_folder_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = StorageControlClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.get_folder in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.get_folder] = mock_rpc
+        request = {}
+        client.get_folder(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_folder(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_get_folder_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = StorageControlAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -1804,14 +2019,58 @@
         )
         # clear UUID field so that the check below succeeds
         args[0].request_id = None
         assert args[0] == storage_control.GetFolderRequest()
 
 
 @pytest.mark.asyncio
+async def test_get_folder_async_use_cached_wrapped_rpc(transport: str = "grpc_asyncio"):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = StorageControlAsyncClient(
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
+            client._client._transport.get_folder
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
+            client._client._transport.get_folder
+        ] = mock_object
+
+        request = {}
+        await client.get_folder(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.get_folder(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_get_folder_async(
     transport: str = "grpc_asyncio", request_type=storage_control.GetFolderRequest
 ):
     client = StorageControlAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -2003,14 +2262,17 @@
     client = StorageControlClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_folders), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_folders()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == storage_control.ListFoldersRequest()
 
 
 def test_list_folders_non_empty_request_with_auto_populated_field():
@@ -2031,27 +2293,65 @@
         delimiter="delimiter_value",
         lexicographic_start="lexicographic_start_value",
         lexicographic_end="lexicographic_end_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_folders), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_folders(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == storage_control.ListFoldersRequest(
             parent="parent_value",
             page_token="page_token_value",
             prefix="prefix_value",
             delimiter="delimiter_value",
             lexicographic_start="lexicographic_start_value",
             lexicographic_end="lexicographic_end_value",
         )
 
 
+def test_list_folders_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = StorageControlClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.list_folders in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.list_folders] = mock_rpc
+        request = {}
+        client.list_folders(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_folders(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_list_folders_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = StorageControlAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -2068,14 +2368,60 @@
         response = await client.list_folders()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == storage_control.ListFoldersRequest()
 
 
 @pytest.mark.asyncio
+async def test_list_folders_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = StorageControlAsyncClient(
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
+            client._client._transport.list_folders
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
+            client._client._transport.list_folders
+        ] = mock_object
+
+        request = {}
+        await client.list_folders(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.list_folders(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_list_folders_async(
     transport: str = "grpc_asyncio", request_type=storage_control.ListFoldersRequest
 ):
     client = StorageControlAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -2447,14 +2793,17 @@
     client = StorageControlClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.rename_folder), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.rename_folder()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         # Ensure that the uuid4 field is set according to AIP 4235
         assert re.match(
             r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
             args[0].request_id,
@@ -2478,14 +2827,17 @@
     request = storage_control.RenameFolderRequest(
         name="name_value",
         destination_folder_id="destination_folder_id_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.rename_folder), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.rename_folder(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         # Ensure that the uuid4 field is set according to AIP 4235
         assert re.match(
             r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
             args[0].request_id,
@@ -2494,14 +2846,53 @@
         args[0].request_id = None
         assert args[0] == storage_control.RenameFolderRequest(
             name="name_value",
             destination_folder_id="destination_folder_id_value",
         )
 
 
+def test_rename_folder_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = StorageControlClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.rename_folder in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.rename_folder] = mock_rpc
+        request = {}
+        client.rename_folder(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.rename_folder(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_rename_folder_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = StorageControlAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -2523,14 +2914,64 @@
         )
         # clear UUID field so that the check below succeeds
         args[0].request_id = None
         assert args[0] == storage_control.RenameFolderRequest()
 
 
 @pytest.mark.asyncio
+async def test_rename_folder_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = StorageControlAsyncClient(
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
+            client._client._transport.rename_folder
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
+            client._client._transport.rename_folder
+        ] = mock_object
+
+        request = {}
+        await client.rename_folder(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        await client.rename_folder(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_rename_folder_async(
     transport: str = "grpc_asyncio", request_type=storage_control.RenameFolderRequest
 ):
     client = StorageControlAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -2740,14 +3181,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_storage_layout), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_storage_layout()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         # Ensure that the uuid4 field is set according to AIP 4235
         assert re.match(
             r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
             args[0].request_id,
@@ -2773,14 +3217,17 @@
         prefix="prefix_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_storage_layout), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_storage_layout(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         # Ensure that the uuid4 field is set according to AIP 4235
         assert re.match(
             r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
             args[0].request_id,
@@ -2789,14 +3236,53 @@
         args[0].request_id = None
         assert args[0] == storage_control.GetStorageLayoutRequest(
             name="name_value",
             prefix="prefix_value",
         )
 
 
+def test_get_storage_layout_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = StorageControlClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.get_storage_layout in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.get_storage_layout
+        ] = mock_rpc
+        request = {}
+        client.get_storage_layout(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_storage_layout(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_get_storage_layout_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = StorageControlAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -2824,14 +3310,60 @@
         )
         # clear UUID field so that the check below succeeds
         args[0].request_id = None
         assert args[0] == storage_control.GetStorageLayoutRequest()
 
 
 @pytest.mark.asyncio
+async def test_get_storage_layout_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = StorageControlAsyncClient(
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
+            client._client._transport.get_storage_layout
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
+            client._client._transport.get_storage_layout
+        ] = mock_object
+
+        request = {}
+        await client.get_storage_layout(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.get_storage_layout(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_get_storage_layout_async(
     transport: str = "grpc_asyncio",
     request_type=storage_control.GetStorageLayoutRequest,
 ):
     client = StorageControlAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -3045,14 +3577,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_managed_folder), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.create_managed_folder()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         # Ensure that the uuid4 field is set according to AIP 4235
         assert re.match(
             r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
             args[0].request_id,
@@ -3078,14 +3613,17 @@
         managed_folder_id="managed_folder_id_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_managed_folder), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.create_managed_folder(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         # Ensure that the uuid4 field is set according to AIP 4235
         assert re.match(
             r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
             args[0].request_id,
@@ -3094,14 +3632,54 @@
         args[0].request_id = None
         assert args[0] == storage_control.CreateManagedFolderRequest(
             parent="parent_value",
             managed_folder_id="managed_folder_id_value",
         )
 
 
+def test_create_managed_folder_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = StorageControlClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.create_managed_folder
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.create_managed_folder
+        ] = mock_rpc
+        request = {}
+        client.create_managed_folder(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.create_managed_folder(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_create_managed_folder_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = StorageControlAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -3128,14 +3706,60 @@
         )
         # clear UUID field so that the check below succeeds
         args[0].request_id = None
         assert args[0] == storage_control.CreateManagedFolderRequest()
 
 
 @pytest.mark.asyncio
+async def test_create_managed_folder_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = StorageControlAsyncClient(
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
+            client._client._transport.create_managed_folder
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
+            client._client._transport.create_managed_folder
+        ] = mock_object
+
+        request = {}
+        await client.create_managed_folder(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.create_managed_folder(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_create_managed_folder_async(
     transport: str = "grpc_asyncio",
     request_type=storage_control.CreateManagedFolderRequest,
 ):
     client = StorageControlAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -3360,14 +3984,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_managed_folder), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.delete_managed_folder()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         # Ensure that the uuid4 field is set according to AIP 4235
         assert re.match(
             r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
             args[0].request_id,
@@ -3392,14 +4019,17 @@
         name="name_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_managed_folder), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.delete_managed_folder(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         # Ensure that the uuid4 field is set according to AIP 4235
         assert re.match(
             r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
             args[0].request_id,
@@ -3407,14 +4037,54 @@
         # clear UUID field so that the check below succeeds
         args[0].request_id = None
         assert args[0] == storage_control.DeleteManagedFolderRequest(
             name="name_value",
         )
 
 
+def test_delete_managed_folder_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = StorageControlClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.delete_managed_folder
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.delete_managed_folder
+        ] = mock_rpc
+        request = {}
+        client.delete_managed_folder(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.delete_managed_folder(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_delete_managed_folder_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = StorageControlAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -3436,14 +4106,60 @@
         )
         # clear UUID field so that the check below succeeds
         args[0].request_id = None
         assert args[0] == storage_control.DeleteManagedFolderRequest()
 
 
 @pytest.mark.asyncio
+async def test_delete_managed_folder_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = StorageControlAsyncClient(
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
+            client._client._transport.delete_managed_folder
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
+            client._client._transport.delete_managed_folder
+        ] = mock_object
+
+        request = {}
+        await client.delete_managed_folder(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.delete_managed_folder(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_delete_managed_folder_async(
     transport: str = "grpc_asyncio",
     request_type=storage_control.DeleteManagedFolderRequest,
 ):
     client = StorageControlAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -3646,14 +4362,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_managed_folder), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_managed_folder()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         # Ensure that the uuid4 field is set according to AIP 4235
         assert re.match(
             r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
             args[0].request_id,
@@ -3678,14 +4397,17 @@
         name="name_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_managed_folder), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_managed_folder(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         # Ensure that the uuid4 field is set according to AIP 4235
         assert re.match(
             r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
             args[0].request_id,
@@ -3693,14 +4415,53 @@
         # clear UUID field so that the check below succeeds
         args[0].request_id = None
         assert args[0] == storage_control.GetManagedFolderRequest(
             name="name_value",
         )
 
 
+def test_get_managed_folder_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = StorageControlClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.get_managed_folder in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.get_managed_folder
+        ] = mock_rpc
+        request = {}
+        client.get_managed_folder(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_managed_folder(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_get_managed_folder_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = StorageControlAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -3727,14 +4488,60 @@
         )
         # clear UUID field so that the check below succeeds
         args[0].request_id = None
         assert args[0] == storage_control.GetManagedFolderRequest()
 
 
 @pytest.mark.asyncio
+async def test_get_managed_folder_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = StorageControlAsyncClient(
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
+            client._client._transport.get_managed_folder
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
+            client._client._transport.get_managed_folder
+        ] = mock_object
+
+        request = {}
+        await client.get_managed_folder(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.get_managed_folder(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_get_managed_folder_async(
     transport: str = "grpc_asyncio",
     request_type=storage_control.GetManagedFolderRequest,
 ):
     client = StorageControlAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -3944,14 +4751,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_managed_folders), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_managed_folders()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         # Ensure that the uuid4 field is set according to AIP 4235
         assert re.match(
             r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
             args[0].request_id,
@@ -3978,14 +4788,17 @@
         prefix="prefix_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_managed_folders), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_managed_folders(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         # Ensure that the uuid4 field is set according to AIP 4235
         assert re.match(
             r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
             args[0].request_id,
@@ -3995,14 +4808,53 @@
         assert args[0] == storage_control.ListManagedFoldersRequest(
             parent="parent_value",
             page_token="page_token_value",
             prefix="prefix_value",
         )
 
 
+def test_list_managed_folders_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = StorageControlClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.list_managed_folders in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_managed_folders
+        ] = mock_rpc
+        request = {}
+        client.list_managed_folders(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_managed_folders(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_list_managed_folders_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = StorageControlAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -4028,14 +4880,60 @@
         )
         # clear UUID field so that the check below succeeds
         args[0].request_id = None
         assert args[0] == storage_control.ListManagedFoldersRequest()
 
 
 @pytest.mark.asyncio
+async def test_list_managed_folders_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = StorageControlAsyncClient(
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
+            client._client._transport.list_managed_folders
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
+            client._client._transport.list_managed_folders
+        ] = mock_object
+
+        request = {}
+        await client.list_managed_folders(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.list_managed_folders(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_list_managed_folders_async(
     transport: str = "grpc_asyncio",
     request_type=storage_control.ListManagedFoldersRequest,
 ):
     client = StorageControlAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -4965,31 +5863,31 @@
     actual = StorageControlClient.parse_folder_path(path)
     assert expected == actual
 
 
 def test_managed_folder_path():
     project = "cuttlefish"
     bucket = "mussel"
-    managedFolder = "winkle"
+    managed_folder = "winkle"
     expected = (
-        "projects/{project}/buckets/{bucket}/managedFolders/{managedFolder}".format(
+        "projects/{project}/buckets/{bucket}/managedFolders/{managed_folder}".format(
             project=project,
             bucket=bucket,
-            managedFolder=managedFolder,
+            managed_folder=managed_folder,
         )
     )
-    actual = StorageControlClient.managed_folder_path(project, bucket, managedFolder)
+    actual = StorageControlClient.managed_folder_path(project, bucket, managed_folder)
     assert expected == actual
 
 
 def test_parse_managed_folder_path():
     expected = {
         "project": "nautilus",
         "bucket": "scallop",
-        "managedFolder": "abalone",
+        "managed_folder": "abalone",
     }
     path = StorageControlClient.managed_folder_path(**expected)
 
     # Check that the path construction is reversible.
     actual = StorageControlClient.parse_managed_folder_path(path)
     assert expected == actual
```

