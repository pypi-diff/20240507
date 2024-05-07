# Comparing `tmp/qase_python_commons-3.0.2b1.tar.gz` & `tmp/qase_python_commons-3.0.2b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qase_python_commons-3.0.2b1.tar", last modified: Mon May  6 08:33:04 2024, max compression
+gzip compressed data, was "qase_python_commons-3.0.2b2.tar", last modified: Mon May  6 13:33:38 2024, max compression
```

## Comparing `qase_python_commons-3.0.2b1.tar` & `qase_python_commons-3.0.2b2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:33:04.394394 qase_python_commons-3.0.2b1/
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-06 08:33:04.394394 qase_python_commons-3.0.2b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 08:33:04.394394 qase_python_commons-3.0.2b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:33:04.386394 qase_python_commons-3.0.2b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:33:04.386394 qase_python_commons-3.0.2b1/src/qase/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:33:04.390395 qase_python_commons-3.0.2b1/src/qase/commons/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:33:04.390395 qase_python_commons-3.0.2b1/src/qase/commons/client/
--rw-r--r--   0 runner    (1001) docker     (127)    10910 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/client/api_v1_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/client/base_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:33:04.390395 qase_python_commons-3.0.2b1/src/qase/commons/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/exceptions/reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:33:04.390395 qase_python_commons-3.0.2b1/src/qase/commons/models/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/models/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/models/basemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/models/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/models/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/models/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/models/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/models/step.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/models/suite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:33:04.390395 qase_python_commons-3.0.2b1/src/qase/commons/profilers/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/profilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/profilers/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/profilers/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/profilers/sleep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:33:04.394394 qase_python_commons-3.0.2b1/src/qase/commons/reporters/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/reporters/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/reporters/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/reporters/testops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:33:04.394394 qase_python_commons-3.0.2b1/src/qase/commons/validators/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/validators/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:33:04.394394 qase_python_commons-3.0.2b1/src/qase_python_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-06 08:33:04.000000 qase_python_commons-3.0.2b1/src/qase_python_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-06 08:33:04.000000 qase_python_commons-3.0.2b1/src/qase_python_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 08:33:04.000000 qase_python_commons-3.0.2b1/src/qase_python_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-06 08:33:04.000000 qase_python_commons-3.0.2b1/src/qase_python_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 08:33:04.000000 qase_python_commons-3.0.2b1/src/qase_python_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:33:38.510496 qase_python_commons-3.0.2b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-06 13:33:38.510496 qase_python_commons-3.0.2b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 13:33:38.510496 qase_python_commons-3.0.2b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:33:38.502496 qase_python_commons-3.0.2b2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:33:38.502496 qase_python_commons-3.0.2b2/src/qase/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:33:38.502496 qase_python_commons-3.0.2b2/src/qase/commons/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:33:38.502496 qase_python_commons-3.0.2b2/src/qase/commons/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    10934 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/client/api_v1_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/client/base_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:33:38.502496 qase_python_commons-3.0.2b2/src/qase/commons/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/exceptions/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:33:38.506496 qase_python_commons-3.0.2b2/src/qase/commons/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/models/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/models/basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/models/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/models/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/models/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/models/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/models/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/models/suite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:33:38.506496 qase_python_commons-3.0.2b2/src/qase/commons/profilers/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/profilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/profilers/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/profilers/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/profilers/sleep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:33:38.506496 qase_python_commons-3.0.2b2/src/qase/commons/reporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/reporters/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/reporters/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/reporters/testops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:33:38.506496 qase_python_commons-3.0.2b2/src/qase/commons/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-06 13:33:31.000000 qase_python_commons-3.0.2b2/src/qase/commons/validators/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:33:38.506496 qase_python_commons-3.0.2b2/src/qase_python_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-06 13:33:38.000000 qase_python_commons-3.0.2b2/src/qase_python_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-06 13:33:38.000000 qase_python_commons-3.0.2b2/src/qase_python_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 13:33:38.000000 qase_python_commons-3.0.2b2/src/qase_python_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-06 13:33:38.000000 qase_python_commons-3.0.2b2/src/qase_python_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 13:33:38.000000 qase_python_commons-3.0.2b2/src/qase_python_commons.egg-info/top_level.txt
```

### Comparing `qase_python_commons-3.0.2b1/PKG-INFO` & `qase_python_commons-3.0.2b2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-python-commons
-Version: 3.0.2b1
+Version: 3.0.2b2
 Summary: A library for Qase TestOps and Qase Report
 Author-email: Qase Team <support@qase.io>
 Project-URL: Homepage, https://github.com/qase-tms/qase-python/tree/master/qase-python-commons
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: certifi>=2024.2.2
 Requires-Dist: attrs>=23.2.0
-Requires-Dist: qaseio==4.0.2
+Requires-Dist: qase-api-client~=1.0.0b2
 Requires-Dist: more_itertools
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: mock; extra == "testing"
 Requires-Dist: more_itertools; extra == "testing"
 Requires-Dist: requests; extra == "testing"
```

### Comparing `qase_python_commons-3.0.2b1/pyproject.toml` & `qase_python_commons-3.0.2b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qase-python-commons"
-version = "3.0.2b1"
+version = "3.0.2b2"
 description = "A library for Qase TestOps and Qase Report"
 readme = "README.md"
 authors = [{name = "Qase Team", email = "support@qase.io"}]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
@@ -26,15 +26,15 @@
     'Programming Language :: Python :: 3.12',
 ]
 urls = {"Homepage" = "https://github.com/qase-tms/qase-python/tree/master/qase-python-commons"}
 requires-python = ">=3.7"
 dependencies = [
     "certifi>=2024.2.2",
     "attrs>=23.2.0",
-    "qaseio==4.0.2",
+    "qase-api-client~=1.0.0b2",
     "more_itertools"
 ]
 
 [project.optional-dependencies]
 testing = [
     "pytest",
     "pytest-cov",
```

### Comparing `qase_python_commons-3.0.2b1/src/qase/commons/client/api_v1_client.py` & `qase_python_commons-3.0.2b2/src/qase/commons/client/api_v1_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Dict, Union
 
 import certifi
-from qaseio import ApiClient, ProjectsApi, Project, EnvironmentsApi, RunsApi, AttachmentsApi, \
+from qase.api_client_v1 import ApiClient, ProjectsApi, Project, EnvironmentsApi, RunsApi, AttachmentsApi, \
     AttachmentGet, RunCreate, ResultsApi, ResultcreateBulk
-from qaseio.configuration import Configuration
+from qase.api_client_v1.configuration import Configuration
 from .. import ConfigManager, Logger
 from .base_api_client import BaseApiClient
 from ..exceptions.reporter import ReporterException
 from ..models import Attachment, Result, Step
 from ..models.step import StepType
```

### Comparing `qase_python_commons-3.0.2b1/src/qase/commons/client/base_api_client.py` & `qase_python_commons-3.0.2b2/src/qase/commons/client/base_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import abc
-from typing import Dict, Union
+from typing import Union
 
-from qaseio import Project, AttachmentGet
+from qase.api_client_v1 import Project, AttachmentGet
 
 from ..models import Attachment
 
 
 class BaseApiClient(abc.ABC):
     @abc.abstractmethod
     def get_project(self, project_code: str) -> Union[Project, None]:
```

### Comparing `qase_python_commons-3.0.2b1/src/qase/commons/config.py` & `qase_python_commons-3.0.2b2/src/qase/commons/config.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b1/src/qase/commons/loader.py` & `qase_python_commons-3.0.2b2/src/qase/commons/loader.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from qaseio.api_client import ApiClient
-from qaseio.configuration import Configuration
-from qaseio.api.plans_api import PlansApi
-from qaseio.rest import ApiException
+from qase.api_client_v1.api_client import ApiClient
+from qase.api_client_v1.configuration import Configuration
+from qase.api_client_v1.api.plans_api import PlansApi
+from qase.api_client_v1.exceptions import ApiException
 
 import certifi
 
 
 class TestOpsPlanLoader:
     def __init__(self, api_token, host='qase.io'):
         configuration = Configuration()
```

### Comparing `qase_python_commons-3.0.2b1/src/qase/commons/logger.py` & `qase_python_commons-3.0.2b2/src/qase/commons/logger.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b1/src/qase/commons/models/attachment.py` & `qase_python_commons-3.0.2b2/src/qase/commons/models/attachment.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b1/src/qase/commons/models/result.py` & `qase_python_commons-3.0.2b2/src/qase/commons/models/result.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b1/src/qase/commons/models/run.py` & `qase_python_commons-3.0.2b2/src/qase/commons/models/run.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b1/src/qase/commons/models/runtime.py` & `qase_python_commons-3.0.2b2/src/qase/commons/models/runtime.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b1/src/qase/commons/models/step.py` & `qase_python_commons-3.0.2b2/src/qase/commons/models/step.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b1/src/qase/commons/profilers/network.py` & `qase_python_commons-3.0.2b2/src/qase/commons/profilers/network.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b1/src/qase/commons/profilers/sleep.py` & `qase_python_commons-3.0.2b2/src/qase/commons/profilers/sleep.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b1/src/qase/commons/reporters/core.py` & `qase_python_commons-3.0.2b2/src/qase/commons/reporters/core.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b1/src/qase/commons/reporters/report.py` & `qase_python_commons-3.0.2b2/src/qase/commons/reporters/report.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b1/src/qase/commons/reporters/testops.py` & `qase_python_commons-3.0.2b2/src/qase/commons/reporters/testops.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b1/src/qase/commons/utils.py` & `qase_python_commons-3.0.2b2/src/qase/commons/utils.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b1/src/qase_python_commons.egg-info/PKG-INFO` & `qase_python_commons-3.0.2b2/src/qase_python_commons.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-python-commons
-Version: 3.0.2b1
+Version: 3.0.2b2
 Summary: A library for Qase TestOps and Qase Report
 Author-email: Qase Team <support@qase.io>
 Project-URL: Homepage, https://github.com/qase-tms/qase-python/tree/master/qase-python-commons
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: certifi>=2024.2.2
 Requires-Dist: attrs>=23.2.0
-Requires-Dist: qaseio==4.0.2
+Requires-Dist: qase-api-client~=1.0.0b2
 Requires-Dist: more_itertools
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: mock; extra == "testing"
 Requires-Dist: more_itertools; extra == "testing"
 Requires-Dist: requests; extra == "testing"
```

### Comparing `qase_python_commons-3.0.2b1/src/qase_python_commons.egg-info/SOURCES.txt` & `qase_python_commons-3.0.2b2/src/qase_python_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

