# Comparing `tmp/strangeworks_qiskit-0.4.6.tar.gz` & `tmp/strangeworks_qiskit-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_qiskit-0.4.6.tar", max compression
+gzip compressed data, was "strangeworks_qiskit-0.4.7.tar", max compression
```

## Comparing `strangeworks_qiskit-0.4.6.tar` & `strangeworks_qiskit-0.4.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      457 2024-02-12 15:02:01.742150 strangeworks_qiskit-0.4.6/DESCRIPTION.md
--rw-r--r--   0        0        0    11357 2024-02-12 15:02:01.742150 strangeworks_qiskit-0.4.6/LICENSE
--rw-r--r--   0        0        0     1120 2024-02-12 15:02:17.733905 strangeworks_qiskit-0.4.6/pyproject.toml
--rw-r--r--   0        0        0      392 2024-02-12 15:02:01.742150 strangeworks_qiskit-0.4.6/strangeworks_qiskit/__init__.py
--rw-r--r--   0        0        0     6009 2024-02-12 15:02:01.742150 strangeworks_qiskit-0.4.6/strangeworks_qiskit/_runtime_client.py
--rw-r--r--   0        0        0      910 2024-02-12 15:02:01.742150 strangeworks_qiskit-0.4.6/strangeworks_qiskit/backends/__init__.py
--rw-r--r--   0        0        0     1427 2024-02-12 15:02:01.742150 strangeworks_qiskit-0.4.6/strangeworks_qiskit/backends/_utils.py
--rw-r--r--   0        0        0     1563 2024-02-12 15:02:01.742150 strangeworks_qiskit-0.4.6/strangeworks_qiskit/backends/aws.py
--rw-r--r--   0        0        0      604 2024-02-12 15:02:01.742150 strangeworks_qiskit-0.4.6/strangeworks_qiskit/backends/honeywell.py
--rw-r--r--   0        0        0     8413 2024-02-12 15:02:01.742150 strangeworks_qiskit-0.4.6/strangeworks_qiskit/backends/ibm.py
--rw-r--r--   0        0        0      599 2024-02-12 15:02:01.742150 strangeworks_qiskit-0.4.6/strangeworks_qiskit/backends/ionq.py
--rw-r--r--   0        0        0      932 2024-02-12 15:02:01.742150 strangeworks_qiskit-0.4.6/strangeworks_qiskit/backends/rigetti.py
--rw-r--r--   0        0        0     3497 2024-02-12 15:02:01.742150 strangeworks_qiskit-0.4.6/strangeworks_qiskit/backends/strangeworks.py
--rw-r--r--   0        0        0        0 2024-02-12 15:02:01.746150 strangeworks_qiskit-0.4.6/strangeworks_qiskit/jobs/__init__.py
--rw-r--r--   0        0        0     2852 2024-02-12 15:02:01.746150 strangeworks_qiskit-0.4.6/strangeworks_qiskit/jobs/ibm.py
--rw-r--r--   0        0        0     4729 2024-02-12 15:02:01.746150 strangeworks_qiskit-0.4.6/strangeworks_qiskit/jobs/job.py
--rw-r--r--   0        0        0      884 2024-02-12 15:02:01.746150 strangeworks_qiskit-0.4.6/strangeworks_qiskit/jobs/status.py
--rw-r--r--   0        0        0       74 2024-02-12 15:02:01.746150 strangeworks_qiskit-0.4.6/strangeworks_qiskit/platform/__init__.py
--rw-r--r--   0        0        0     3436 2024-02-12 15:02:01.746150 strangeworks_qiskit-0.4.6/strangeworks_qiskit/platform/backends.py
--rw-r--r--   0        0        0     4354 2024-02-12 15:02:01.746150 strangeworks_qiskit-0.4.6/strangeworks_qiskit/provider.py
--rw-r--r--   0        0        0     9111 2024-02-12 15:02:01.746150 strangeworks_qiskit-0.4.6/strangeworks_qiskit/runtimes.py
--rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 strangeworks_qiskit-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0      457 2024-05-07 13:23:47.340333 strangeworks_qiskit-0.4.7/DESCRIPTION.md
+-rw-r--r--   0        0        0    11357 2024-05-07 13:23:47.340333 strangeworks_qiskit-0.4.7/LICENSE
+-rw-r--r--   0        0        0     1118 2024-05-07 13:23:59.412246 strangeworks_qiskit-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0      392 2024-05-07 13:23:47.344333 strangeworks_qiskit-0.4.7/strangeworks_qiskit/__init__.py
+-rw-r--r--   0        0        0     6009 2024-05-07 13:23:47.344333 strangeworks_qiskit-0.4.7/strangeworks_qiskit/_runtime_client.py
+-rw-r--r--   0        0        0      910 2024-05-07 13:23:47.344333 strangeworks_qiskit-0.4.7/strangeworks_qiskit/backends/__init__.py
+-rw-r--r--   0        0        0     1427 2024-05-07 13:23:47.344333 strangeworks_qiskit-0.4.7/strangeworks_qiskit/backends/_utils.py
+-rw-r--r--   0        0        0     1563 2024-05-07 13:23:47.344333 strangeworks_qiskit-0.4.7/strangeworks_qiskit/backends/aws.py
+-rw-r--r--   0        0        0      604 2024-05-07 13:23:47.344333 strangeworks_qiskit-0.4.7/strangeworks_qiskit/backends/honeywell.py
+-rw-r--r--   0        0        0     8413 2024-05-07 13:23:47.344333 strangeworks_qiskit-0.4.7/strangeworks_qiskit/backends/ibm.py
+-rw-r--r--   0        0        0      599 2024-05-07 13:23:47.344333 strangeworks_qiskit-0.4.7/strangeworks_qiskit/backends/ionq.py
+-rw-r--r--   0        0        0      932 2024-05-07 13:23:47.344333 strangeworks_qiskit-0.4.7/strangeworks_qiskit/backends/rigetti.py
+-rw-r--r--   0        0        0     3497 2024-05-07 13:23:47.344333 strangeworks_qiskit-0.4.7/strangeworks_qiskit/backends/strangeworks.py
+-rw-r--r--   0        0        0        0 2024-05-07 13:23:47.344333 strangeworks_qiskit-0.4.7/strangeworks_qiskit/jobs/__init__.py
+-rw-r--r--   0        0        0     2852 2024-05-07 13:23:47.344333 strangeworks_qiskit-0.4.7/strangeworks_qiskit/jobs/ibm.py
+-rw-r--r--   0        0        0     4729 2024-05-07 13:23:47.344333 strangeworks_qiskit-0.4.7/strangeworks_qiskit/jobs/job.py
+-rw-r--r--   0        0        0      884 2024-05-07 13:23:47.344333 strangeworks_qiskit-0.4.7/strangeworks_qiskit/jobs/status.py
+-rw-r--r--   0        0        0       74 2024-05-07 13:23:47.344333 strangeworks_qiskit-0.4.7/strangeworks_qiskit/platform/__init__.py
+-rw-r--r--   0        0        0     3481 2024-05-07 13:23:47.344333 strangeworks_qiskit-0.4.7/strangeworks_qiskit/platform/backends.py
+-rw-r--r--   0        0        0     4354 2024-05-07 13:23:47.344333 strangeworks_qiskit-0.4.7/strangeworks_qiskit/provider.py
+-rw-r--r--   0        0        0     9111 2024-05-07 13:23:47.344333 strangeworks_qiskit-0.4.7/strangeworks_qiskit/runtimes.py
+-rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 strangeworks_qiskit-0.4.7/PKG-INFO
```

### Comparing `strangeworks_qiskit-0.4.6/LICENSE` & `strangeworks_qiskit-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.6/pyproject.toml` & `strangeworks_qiskit-0.4.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 max-line-length = 88
 per-file-ignores = [
     "__init__.py:F401"
 ]
 
 [tool.poetry]
 name = "strangeworks-qiskit"
-version = "0.4.6"
+version = "0.4.7"
 description = "Strangeworks Qiskit SDK Extension"
 readme = "DESCRIPTION.md"
 authors = ["Strange Devs <hello@strangeworks.com>"]
 license = "Apache-2.0"
 packages = [
     {include = "strangeworks_qiskit"},
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 strangeworks = "^0.5.1"
-qiskit = "<=0.40.0"
+qiskit = "0.40.0"
 strangeworks-core = "^0.3.6"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.1.0"
 Flake8-pyproject = "^1.1.0"
 Flask = "^2.0.2"
 mdformat = "^0.7.14"
```

### Comparing `strangeworks_qiskit-0.4.6/strangeworks_qiskit/_runtime_client.py` & `strangeworks_qiskit-0.4.7/strangeworks_qiskit/_runtime_client.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.6/strangeworks_qiskit/backends/__init__.py` & `strangeworks_qiskit-0.4.7/strangeworks_qiskit/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.6/strangeworks_qiskit/backends/_utils.py` & `strangeworks_qiskit-0.4.7/strangeworks_qiskit/backends/_utils.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.6/strangeworks_qiskit/backends/aws.py` & `strangeworks_qiskit-0.4.7/strangeworks_qiskit/backends/aws.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.6/strangeworks_qiskit/backends/honeywell.py` & `strangeworks_qiskit-0.4.7/strangeworks_qiskit/backends/honeywell.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.6/strangeworks_qiskit/backends/ibm.py` & `strangeworks_qiskit-0.4.7/strangeworks_qiskit/backends/ibm.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.6/strangeworks_qiskit/backends/ionq.py` & `strangeworks_qiskit-0.4.7/strangeworks_qiskit/backends/ionq.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.6/strangeworks_qiskit/backends/rigetti.py` & `strangeworks_qiskit-0.4.7/strangeworks_qiskit/backends/rigetti.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.6/strangeworks_qiskit/backends/strangeworks.py` & `strangeworks_qiskit-0.4.7/strangeworks_qiskit/backends/strangeworks.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.6/strangeworks_qiskit/jobs/ibm.py` & `strangeworks_qiskit-0.4.7/strangeworks_qiskit/jobs/ibm.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.6/strangeworks_qiskit/jobs/job.py` & `strangeworks_qiskit-0.4.7/strangeworks_qiskit/jobs/job.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.6/strangeworks_qiskit/jobs/status.py` & `strangeworks_qiskit-0.4.7/strangeworks_qiskit/jobs/status.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.6/strangeworks_qiskit/platform/backends.py` & `strangeworks_qiskit-0.4.7/strangeworks_qiskit/platform/backends.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """backends.py"""
+
 import json
 from typing import Any, Dict, List, Optional
 
 from pydantic import BaseModel, Field
-from strangeworks.core.client.platform import API, Operation
+from strangeworks.platform.gql import SDKAPI as API
+from strangeworks_core.platform.gql import Operation
 from strangeworks_core.types.backend import Backend
 
 
 get_backends_query = Operation(
     query="""
     query backends(
         $product_slugs: [String!]
```

### Comparing `strangeworks_qiskit-0.4.6/strangeworks_qiskit/provider.py` & `strangeworks_qiskit-0.4.7/strangeworks_qiskit/provider.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.6/strangeworks_qiskit/runtimes.py` & `strangeworks_qiskit-0.4.7/strangeworks_qiskit/runtimes.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.6/PKG-INFO` & `strangeworks_qiskit-0.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: strangeworks-qiskit
-Version: 0.4.6
+Version: 0.4.7
 Summary: Strangeworks Qiskit SDK Extension
 License: Apache-2.0
 Author: Strange Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: qiskit (<=0.40.0)
+Requires-Dist: qiskit (==0.40.0)
 Requires-Dist: strangeworks (>=0.5.1,<0.6.0)
 Requires-Dist: strangeworks-core (>=0.3.6,<0.4.0)
 Description-Content-Type: text/markdown
 
 | ⚠️ | This SDK is currently in pre-release alpha state and subject to change. To get
 more info or access to test features check out the
 [Strangeworks Backstage Pass Program](https://strangeworks.com/backstage). |
```

