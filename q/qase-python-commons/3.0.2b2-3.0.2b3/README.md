# Comparing `tmp/qase_python_commons-3.0.2b2.tar.gz` & `tmp/qase_python_commons-3.0.2b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qase_python_commons-3.0.2b2.tar", last modified: Mon May  6 13:33:38 2024, max compression
+gzip compressed data, was "qase_python_commons-3.0.2b3.tar", last modified: Tue May  7 11:55:48 2024, max compression
```

## Comparing `qase_python_commons-3.0.2b2.tar` & `qase_python_commons-3.0.2b3.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:33:38.510496 qase_python_commons-3.0.2b2/
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-06 13:33:38.510496 qase_python_commons-3.0.2b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 13:33:38.510496 qase_python_commons-3.0.2b2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:33:38.502496 qase_python_commons-3.0.2b2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:33:38.502496 qase_python_commons-3.0.2b2/src/qase/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:33:38.502496 qase_python_commons-3.0.2b2/src/qase/commons/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:33:38.502496 qase_python_commons-3.0.2b2/src/qase/commons/client/
--rw-r--r--   0 runner    (1001) docker     (127)    10934 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/client/api_v1_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/client/base_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:33:38.502496 qase_python_commons-3.0.2b2/src/qase/commons/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/exceptions/reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:33:38.506496 qase_python_commons-3.0.2b2/src/qase/commons/models/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/models/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/models/basemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/models/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/models/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/models/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/models/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/models/step.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/models/suite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:33:38.506496 qase_python_commons-3.0.2b2/src/qase/commons/profilers/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/profilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/profilers/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/profilers/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/profilers/sleep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:33:38.506496 qase_python_commons-3.0.2b2/src/qase/commons/reporters/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/reporters/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/reporters/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/reporters/testops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:33:38.506496 qase_python_commons-3.0.2b2/src/qase/commons/validators/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/validators/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:33:38.506496 qase_python_commons-3.0.2b2/src/qase_python_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-06 13:33:38.000000 qase_python_commons-3.0.2b2/src/qase_python_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-06 13:33:38.000000 qase_python_commons-3.0.2b2/src/qase_python_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 13:33:38.000000 qase_python_commons-3.0.2b2/src/qase_python_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-06 13:33:38.000000 qase_python_commons-3.0.2b2/src/qase_python_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 13:33:38.000000 qase_python_commons-3.0.2b2/src/qase_python_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:55:48.073988 qase_python_commons-3.0.2b3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-07 11:55:48.073988 qase_python_commons-3.0.2b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 11:55:48.073988 qase_python_commons-3.0.2b3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:55:48.065988 qase_python_commons-3.0.2b3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:55:48.065988 qase_python_commons-3.0.2b3/src/qase/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:55:48.065988 qase_python_commons-3.0.2b3/src/qase/commons/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/src/qase/commons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:55:48.069988 qase_python_commons-3.0.2b3/src/qase/commons/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    10934 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/src/qase/commons/client/api_v1_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/src/qase/commons/client/api_v2_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/src/qase/commons/client/base_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/src/qase/commons/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:55:48.069988 qase_python_commons-3.0.2b3/src/qase/commons/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/src/qase/commons/exceptions/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/src/qase/commons/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/src/qase/commons/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:55:48.069988 qase_python_commons-3.0.2b3/src/qase/commons/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/src/qase/commons/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/src/qase/commons/models/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/src/qase/commons/models/basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/src/qase/commons/models/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/src/qase/commons/models/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/src/qase/commons/models/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/src/qase/commons/models/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/src/qase/commons/models/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/src/qase/commons/models/suite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:55:48.069988 qase_python_commons-3.0.2b3/src/qase/commons/profilers/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/src/qase/commons/profilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/src/qase/commons/profilers/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/src/qase/commons/profilers/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/src/qase/commons/profilers/sleep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:55:48.069988 qase_python_commons-3.0.2b3/src/qase/commons/reporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/src/qase/commons/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/src/qase/commons/reporters/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/src/qase/commons/reporters/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/src/qase/commons/reporters/testops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/src/qase/commons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:55:48.069988 qase_python_commons-3.0.2b3/src/qase/commons/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-07 11:55:41.000000 qase_python_commons-3.0.2b3/src/qase/commons/validators/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:55:48.073988 qase_python_commons-3.0.2b3/src/qase_python_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-07 11:55:48.000000 qase_python_commons-3.0.2b3/src/qase_python_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-07 11:55:48.000000 qase_python_commons-3.0.2b3/src/qase_python_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 11:55:48.000000 qase_python_commons-3.0.2b3/src/qase_python_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-07 11:55:48.000000 qase_python_commons-3.0.2b3/src/qase_python_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 11:55:48.000000 qase_python_commons-3.0.2b3/src/qase_python_commons.egg-info/top_level.txt
```

### Comparing `qase_python_commons-3.0.2b2/PKG-INFO` & `qase_python_commons-3.0.2b3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-python-commons
-Version: 3.0.2b2
+Version: 3.0.2b3
 Summary: A library for Qase TestOps and Qase Report
 Author-email: Qase Team <support@qase.io>
 Project-URL: Homepage, https://github.com/qase-tms/qase-python/tree/master/qase-python-commons
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: certifi>=2024.2.2
 Requires-Dist: attrs>=23.2.0
 Requires-Dist: qase-api-client~=1.0.0b2
+Requires-Dist: qase-api-v2-client~=1.0.0b2
 Requires-Dist: more_itertools
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: mock; extra == "testing"
 Requires-Dist: more_itertools; extra == "testing"
 Requires-Dist: requests; extra == "testing"
```

### Comparing `qase_python_commons-3.0.2b2/pyproject.toml` & `qase_python_commons-3.0.2b3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qase-python-commons"
-version = "3.0.2b2"
+version = "3.0.2b3"
 description = "A library for Qase TestOps and Qase Report"
 readme = "README.md"
 authors = [{name = "Qase Team", email = "support@qase.io"}]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
@@ -27,14 +27,15 @@
 ]
 urls = {"Homepage" = "https://github.com/qase-tms/qase-python/tree/master/qase-python-commons"}
 requires-python = ">=3.7"
 dependencies = [
     "certifi>=2024.2.2",
     "attrs>=23.2.0",
     "qase-api-client~=1.0.0b2",
+    "qase-api-v2-client~=1.0.0b2",
     "more_itertools"
 ]
 
 [project.optional-dependencies]
 testing = [
     "pytest",
     "pytest-cov",
```

### Comparing `qase_python_commons-3.0.2b2/src/qase/commons/client/api_v1_client.py` & `qase_python_commons-3.0.2b3/src/qase/commons/client/api_v1_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     def check_test_run(self, project_code: str, run_id: int) -> bool:
         api_runs = RunsApi(self.client)
         run = api_runs.get_run(code=project_code, id=run_id)
         if run.result.id:
             return True
         return False
 
-    def send_results(self, project_code: str, run_id: int, results: []) -> None:
+    def send_results(self, project_code: str, run_id: str, results: []) -> None:
         api_results = ResultsApi(self.client)
         results_to_send = [self._prepare_result(project_code, result) for result in results]
         self.logger.log_debug(f"Sending results for run {run_id}: {results_to_send}")
         api_results.create_result_bulk(
             code=project_code,
             id=run_id,
             resultcreate_bulk=ResultcreateBulk(
```

### Comparing `qase_python_commons-3.0.2b2/src/qase/commons/client/base_api_client.py` & `qase_python_commons-3.0.2b3/src/qase/commons/client/base_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,39 +49,39 @@
         :param attachment: attachment model
         :return: attachment data or None if attachment not uploaded
         """
         pass
 
     @abc.abstractmethod
     def create_test_run(self, project_code: str, title: str, description: str, plan_id=None,
-                        environment_id=None) -> int:
+                        environment_id=None) -> str:
         """
         Create a test run in Qase TestOps
 
         :param project_code: project code
         :param title: test run title
         :param description: test run description
         :param plan_id: plan id
         :param environment_id: environment id
         :return: test run id
         """
         pass
 
     @abc.abstractmethod
-    def check_test_run(self, project_code: str, run_id: int) -> bool:
+    def check_test_run(self, project_code: str, run_id: str) -> bool:
         """
         Check if test run exists in Qase TestOps
         :param project_code: project code
         :param run_id: test run id
         :return: True if test run exists, False otherwise
         """
         pass
 
     @abc.abstractmethod
-    def send_results(self, project_code: str, run_id: int, results: []) -> None:
+    def send_results(self, project_code: str, run_id: str, results: []) -> None:
         """
         Send test results to Qase TestOps
         :param project_code: project code
         :param run_id: test run id
         :param results: results data
         :return: None
         """
```

### Comparing `qase_python_commons-3.0.2b2/src/qase/commons/config.py` & `qase_python_commons-3.0.2b3/src/qase/commons/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,17 @@
         self.logger = Logger()
         self.config = {}
         self.parseBool = lambda d: d in ("y", "yes", "true", "1", 1, True)
 
         try:
             if os.path.exists(config_file):
                 with open(config_file, "r") as file:
-                    self.config = json.load(file)
+                    def transform_keys(obj):
+                        return {k.lower(): v for k, v in obj.items()}
+                    self.config = json.load(file, object_hook=transform_keys)
         except Exception as e:
             self.logger.log("Failed to load config from file", "error")
 
         # Load from env vars
         try:
             for key, value in os.environ.items():
                 if key.startswith(env_vars_prefix):
```

### Comparing `qase_python_commons-3.0.2b2/src/qase/commons/loader.py` & `qase_python_commons-3.0.2b3/src/qase/commons/loader.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b2/src/qase/commons/logger.py` & `qase_python_commons-3.0.2b3/src/qase/commons/logger.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b2/src/qase/commons/models/attachment.py` & `qase_python_commons-3.0.2b3/src/qase/commons/models/attachment.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b2/src/qase/commons/models/result.py` & `qase_python_commons-3.0.2b3/src/qase/commons/models/result.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b2/src/qase/commons/models/run.py` & `qase_python_commons-3.0.2b3/src/qase/commons/models/run.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b2/src/qase/commons/models/runtime.py` & `qase_python_commons-3.0.2b3/src/qase/commons/models/runtime.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b2/src/qase/commons/models/step.py` & `qase_python_commons-3.0.2b3/src/qase/commons/models/step.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b2/src/qase/commons/profilers/network.py` & `qase_python_commons-3.0.2b3/src/qase/commons/profilers/network.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b2/src/qase/commons/profilers/sleep.py` & `qase_python_commons-3.0.2b3/src/qase/commons/profilers/sleep.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b2/src/qase/commons/reporters/core.py` & `qase_python_commons-3.0.2b3/src/qase/commons/reporters/core.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b2/src/qase/commons/reporters/report.py` & `qase_python_commons-3.0.2b3/src/qase/commons/reporters/report.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b2/src/qase/commons/reporters/testops.py` & `qase_python_commons-3.0.2b3/src/qase/commons/reporters/testops.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,17 @@
         self.processed = []
         self.attachments = {}
 
         """Verify that project exists in TestOps"""
         self.client.get_project(self.project_code)
 
     def _prepare_client(self) -> BaseApiClient:
+        if self.config.get('testops.usev2', False, bool):
+            from ..client.api_v2_client import ApiV2Client
+            return ApiV2Client(self.config, self.logger)
         return ApiV1Client(self.config, self.logger)
 
     def _send_results_threaded(self, results):
         try:
             self.client.send_results(self.project_code, self.run_id, results)
             with self.lock:
                 self.processed.extend(results)
```

### Comparing `qase_python_commons-3.0.2b2/src/qase/commons/utils.py` & `qase_python_commons-3.0.2b3/src/qase/commons/utils.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b2/src/qase_python_commons.egg-info/PKG-INFO` & `qase_python_commons-3.0.2b3/src/qase_python_commons.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-python-commons
-Version: 3.0.2b2
+Version: 3.0.2b3
 Summary: A library for Qase TestOps and Qase Report
 Author-email: Qase Team <support@qase.io>
 Project-URL: Homepage, https://github.com/qase-tms/qase-python/tree/master/qase-python-commons
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: certifi>=2024.2.2
 Requires-Dist: attrs>=23.2.0
 Requires-Dist: qase-api-client~=1.0.0b2
+Requires-Dist: qase-api-v2-client~=1.0.0b2
 Requires-Dist: more_itertools
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: mock; extra == "testing"
 Requires-Dist: more_itertools; extra == "testing"
 Requires-Dist: requests; extra == "testing"
```

### Comparing `qase_python_commons-3.0.2b2/src/qase_python_commons.egg-info/SOURCES.txt` & `qase_python_commons-3.0.2b3/src/qase_python_commons.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 pyproject.toml
 src/qase/commons/__init__.py
 src/qase/commons/config.py
 src/qase/commons/loader.py
 src/qase/commons/logger.py
 src/qase/commons/utils.py
 src/qase/commons/client/api_v1_client.py
+src/qase/commons/client/api_v2_client.py
 src/qase/commons/client/base_api_client.py
 src/qase/commons/exceptions/reporter.py
 src/qase/commons/models/__init__.py
 src/qase/commons/models/attachment.py
 src/qase/commons/models/basemodel.py
 src/qase/commons/models/relation.py
 src/qase/commons/models/result.py
```

