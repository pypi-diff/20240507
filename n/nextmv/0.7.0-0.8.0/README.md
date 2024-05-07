# Comparing `tmp/nextmv-0.7.0.tar.gz` & `tmp/nextmv-0.8.0.tar.gz`

## Comparing `nextmv-0.7.0.tar` & `nextmv-0.8.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 nextmv-0.7.0/nextmv-py.code-workspace
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nextmv-0.7.0/requirements.txt
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 nextmv-0.7.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 nextmv-0.7.0/.github/workflows/python-lint.yml
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 nextmv-0.7.0/.github/workflows/python-test.yml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nextmv-0.7.0/nextmv/__about__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 nextmv-0.7.0/nextmv/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 nextmv-0.7.0/nextmv/base_model.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 nextmv-0.7.0/nextmv/cloud/__init__.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 nextmv-0.7.0/nextmv/cloud/acceptance_test.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 nextmv-0.7.0/nextmv/cloud/account.py
--rw-r--r--   0        0        0    26676 2020-02-02 00:00:00.000000 nextmv-0.7.0/nextmv/cloud/application.py
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 nextmv-0.7.0/nextmv/cloud/batch_experiment.py
--rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 nextmv-0.7.0/nextmv/cloud/client.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 nextmv-0.7.0/nextmv/cloud/input_set.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 nextmv-0.7.0/nextmv/cloud/status.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 nextmv-0.7.0/nextmv/nextroute/__init__.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 nextmv-0.7.0/nextmv/nextroute/check/__init__.py
--rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 nextmv-0.7.0/nextmv/nextroute/check/schema.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 nextmv-0.7.0/nextmv/nextroute/schema/__init__.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 nextmv-0.7.0/nextmv/nextroute/schema/input.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nextmv-0.7.0/nextmv/nextroute/schema/location.py
--rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 nextmv-0.7.0/nextmv/nextroute/schema/output.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 nextmv-0.7.0/nextmv/nextroute/schema/stop.py
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 nextmv-0.7.0/nextmv/nextroute/schema/vehicle.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 nextmv-0.7.0/tests/test_base_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.7.0/tests/cloud/__init__.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 nextmv-0.7.0/tests/cloud/test_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.7.0/tests/nextroute/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.7.0/tests/nextroute/schema/__init__.py
--rw-r--r--   0        0        0     5134 2020-02-02 00:00:00.000000 nextmv-0.7.0/tests/nextroute/schema/input.json
--rw-r--r--   0        0        0    25755 2020-02-02 00:00:00.000000 nextmv-0.7.0/tests/nextroute/schema/output.json
--rw-r--r--   0        0        0    28915 2020-02-02 00:00:00.000000 nextmv-0.7.0/tests/nextroute/schema/output_with_check.json
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 nextmv-0.7.0/tests/nextroute/schema/test_input.py
--rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 nextmv-0.7.0/tests/nextroute/schema/test_output.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 nextmv-0.7.0/.gitignore
--rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 nextmv-0.7.0/LICENSE
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 nextmv-0.7.0/README.md
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 nextmv-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    15424 2020-02-02 00:00:00.000000 nextmv-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 nextmv-0.8.0/nextmv-py.code-workspace
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nextmv-0.8.0/requirements.txt
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 nextmv-0.8.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 nextmv-0.8.0/.github/workflows/python-lint.yml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 nextmv-0.8.0/.github/workflows/python-test.yml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nextmv-0.8.0/nextmv/__about__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 nextmv-0.8.0/nextmv/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 nextmv-0.8.0/nextmv/base_model.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 nextmv-0.8.0/nextmv/cloud/__init__.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 nextmv-0.8.0/nextmv/cloud/acceptance_test.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 nextmv-0.8.0/nextmv/cloud/account.py
+-rw-r--r--   0        0        0    27129 2020-02-02 00:00:00.000000 nextmv-0.8.0/nextmv/cloud/application.py
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 nextmv-0.8.0/nextmv/cloud/batch_experiment.py
+-rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 nextmv-0.8.0/nextmv/cloud/client.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 nextmv-0.8.0/nextmv/cloud/input_set.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 nextmv-0.8.0/nextmv/cloud/status.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 nextmv-0.8.0/nextmv/nextroute/__init__.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 nextmv-0.8.0/nextmv/nextroute/check/__init__.py
+-rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 nextmv-0.8.0/nextmv/nextroute/check/schema.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 nextmv-0.8.0/nextmv/nextroute/schema/__init__.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 nextmv-0.8.0/nextmv/nextroute/schema/input.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nextmv-0.8.0/nextmv/nextroute/schema/location.py
+-rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 nextmv-0.8.0/nextmv/nextroute/schema/output.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 nextmv-0.8.0/nextmv/nextroute/schema/stop.py
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 nextmv-0.8.0/nextmv/nextroute/schema/vehicle.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 nextmv-0.8.0/tests/test_base_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.8.0/tests/cloud/__init__.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 nextmv-0.8.0/tests/cloud/test_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.8.0/tests/nextroute/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.8.0/tests/nextroute/schema/__init__.py
+-rw-r--r--   0        0        0     5134 2020-02-02 00:00:00.000000 nextmv-0.8.0/tests/nextroute/schema/input.json
+-rw-r--r--   0        0        0    25755 2020-02-02 00:00:00.000000 nextmv-0.8.0/tests/nextroute/schema/output.json
+-rw-r--r--   0        0        0    28915 2020-02-02 00:00:00.000000 nextmv-0.8.0/tests/nextroute/schema/output_with_check.json
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 nextmv-0.8.0/tests/nextroute/schema/test_input.py
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 nextmv-0.8.0/tests/nextroute/schema/test_output.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 nextmv-0.8.0/.gitignore
+-rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 nextmv-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 nextmv-0.8.0/README.md
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 nextmv-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    15424 2020-02-02 00:00:00.000000 nextmv-0.8.0/PKG-INFO
```

### Comparing `nextmv-0.7.0/.github/workflows/publish.yml` & `nextmv-0.8.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/.github/workflows/python-lint.yml` & `nextmv-0.8.0/.github/workflows/python-lint.yml`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/.github/workflows/python-test.yml` & `nextmv-0.8.0/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/nextmv/cloud/__init__.py` & `nextmv-0.8.0/nextmv/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/nextmv/cloud/acceptance_test.py` & `nextmv-0.8.0/nextmv/cloud/acceptance_test.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/nextmv/cloud/account.py` & `nextmv-0.8.0/nextmv/cloud/account.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/nextmv/cloud/application.py` & `nextmv-0.8.0/nextmv/cloud/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,14 +210,33 @@
         """
 
         _ = self.client.request(
             method="PATCH",
             endpoint=f"{self.endpoint}/runs/{run_id}/cancel",
         )
 
+    def delete_batch_experiment(
+        self,
+        id: str,
+    ) -> None:
+        """
+        Deletes a batch experiment, along with all of its runs.
+
+        Args:
+            id: ID of the batch experiment.
+
+        Raises:
+            requests.HTTPError: If the response status code is not 2xx.
+        """
+
+        _ = self.client.request(
+            method="DELETE",
+            endpoint=f"{self.experiments_endpoint}/batch/{id}",
+        )
+
     def input_set(self, input_set_id: str) -> InputSet:
         """
         Get an input set.
 
         Args:
             input_set_id: ID of the input set.
```

### Comparing `nextmv-0.7.0/nextmv/cloud/batch_experiment.py` & `nextmv-0.8.0/nextmv/cloud/batch_experiment.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/nextmv/cloud/client.py` & `nextmv-0.8.0/nextmv/cloud/client.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/nextmv/cloud/input_set.py` & `nextmv-0.8.0/nextmv/cloud/input_set.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/nextmv/cloud/status.py` & `nextmv-0.8.0/nextmv/cloud/status.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/nextmv/nextroute/check/__init__.py` & `nextmv-0.8.0/nextmv/nextroute/check/__init__.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/nextmv/nextroute/check/schema.py` & `nextmv-0.8.0/nextmv/nextroute/check/schema.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/nextmv/nextroute/schema/__init__.py` & `nextmv-0.8.0/nextmv/nextroute/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/nextmv/nextroute/schema/input.py` & `nextmv-0.8.0/nextmv/nextroute/schema/input.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/nextmv/nextroute/schema/output.py` & `nextmv-0.8.0/nextmv/nextroute/schema/output.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/nextmv/nextroute/schema/stop.py` & `nextmv-0.8.0/nextmv/nextroute/schema/stop.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/nextmv/nextroute/schema/vehicle.py` & `nextmv-0.8.0/nextmv/nextroute/schema/vehicle.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/tests/test_base_model.py` & `nextmv-0.8.0/tests/test_base_model.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/tests/cloud/test_client.py` & `nextmv-0.8.0/tests/cloud/test_client.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/tests/nextroute/schema/input.json` & `nextmv-0.8.0/tests/nextroute/schema/input.json`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/tests/nextroute/schema/output.json` & `nextmv-0.8.0/tests/nextroute/schema/output.json`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/tests/nextroute/schema/output_with_check.json` & `nextmv-0.8.0/tests/nextroute/schema/output_with_check.json`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/tests/nextroute/schema/test_input.py` & `nextmv-0.8.0/tests/nextroute/schema/test_input.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/tests/nextroute/schema/test_output.py` & `nextmv-0.8.0/tests/nextroute/schema/test_output.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/.gitignore` & `nextmv-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/LICENSE` & `nextmv-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/README.md` & `nextmv-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/pyproject.toml` & `nextmv-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nextmv-0.7.0/PKG-INFO` & `nextmv-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nextmv
-Version: 0.7.0
+Version: 0.8.0
 Summary: The Python SDK for Nextmv
 Project-URL: Homepage, https://www.nextmv.io
 Project-URL: Documentation, https://www.nextmv.io/docs
 Project-URL: Repository, https://github.com/nextmv-io/nextmv-py
 Author-email: Nextmv <tech@nextmv.io>
 Maintainer-email: Nextmv <tech@nextmv.io>
 License:                                  Apache License
```

