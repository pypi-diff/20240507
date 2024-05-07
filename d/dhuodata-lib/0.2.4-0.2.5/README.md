# Comparing `tmp/dhuodata_lib-0.2.4.tar.gz` & `tmp/dhuodata_lib-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhuodata_lib-0.2.4.tar", last modified: Wed May  1 23:06:52 2024, max compression
+gzip compressed data, was "dhuodata_lib-0.2.5.tar", last modified: Tue May  7 17:02:09 2024, max compression
```

## Comparing `dhuodata_lib-0.2.4.tar` & `dhuodata_lib-0.2.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-01 23:06:52.751688 dhuodata_lib-0.2.4/
--rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-01 23:06:52.751688 dhuodata_lib-0.2.4/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata_lib-0.2.4/README.md
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-05-01 23:06:52.751688 dhuodata_lib-0.2.4/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-05-01 23:06:06.000000 dhuodata_lib-0.2.4/setup.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-01 23:06:52.747688 dhuodata_lib-0.2.4/src/
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-01 23:06:52.747688 dhuodata_lib-0.2.4/src/dhuodata_lib.egg-info/
--rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-01 23:06:52.000000 dhuodata_lib-0.2.4/src/dhuodata_lib.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      424 2024-05-01 23:06:52.000000 dhuodata_lib-0.2.4/src/dhuodata_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-05-01 23:06:52.000000 dhuodata_lib-0.2.4/src/dhuodata_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)      152 2024-05-01 23:06:52.000000 dhuodata_lib-0.2.4/src/dhuodata_lib.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-05-01 23:06:52.000000 dhuodata_lib-0.2.4/src/dhuodata_lib.egg-info/top_level.txt
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-01 23:06:52.747688 dhuodata_lib-0.2.4/src/dhuolib/
--rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata_lib-0.2.4/src/dhuolib/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata_lib-0.2.4/src/dhuolib/auth.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     4249 2024-04-30 19:18:11.000000 dhuodata_lib-0.2.4/src/dhuolib/clients.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      348 2024-04-25 14:26:18.000000 dhuodata_lib-0.2.4/src/dhuolib/config.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-04-24 18:22:52.000000 dhuodata_lib-0.2.4/src/dhuolib/predict.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1341 2024-04-30 19:13:45.000000 dhuodata_lib-0.2.4/src/dhuolib/services.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      750 2024-04-29 11:53:52.000000 dhuodata_lib-0.2.4/src/dhuolib/validations.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata_lib-0.2.4/src/dhuolib/worker.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-01 23:06:52.747688 dhuodata_lib-0.2.4/tests/
--rw-rw-r--   0 diego     (1000) diego     (1000)     2901 2024-05-01 23:06:51.000000 dhuodata_lib-0.2.4/tests/test_dhuolib.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-07 17:02:09.131811 dhuodata_lib-0.2.5/
+-rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-07 17:02:09.131811 dhuodata_lib-0.2.5/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata_lib-0.2.5/README.md
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-05-07 17:02:09.131811 dhuodata_lib-0.2.5/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-05-07 17:01:55.000000 dhuodata_lib-0.2.5/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-07 17:02:09.127812 dhuodata_lib-0.2.5/src/
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-07 17:02:09.127812 dhuodata_lib-0.2.5/src/dhuodata_lib.egg-info/
+-rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-07 17:02:09.000000 dhuodata_lib-0.2.5/src/dhuodata_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      424 2024-05-07 17:02:09.000000 dhuodata_lib-0.2.5/src/dhuodata_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-05-07 17:02:09.000000 dhuodata_lib-0.2.5/src/dhuodata_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)      152 2024-05-07 17:02:09.000000 dhuodata_lib-0.2.5/src/dhuodata_lib.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-05-07 17:02:09.000000 dhuodata_lib-0.2.5/src/dhuodata_lib.egg-info/top_level.txt
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-07 17:02:09.127812 dhuodata_lib-0.2.5/src/dhuolib/
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata_lib-0.2.5/src/dhuolib/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata_lib-0.2.5/src/dhuolib/auth.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     6880 2024-05-07 16:59:59.000000 dhuodata_lib-0.2.5/src/dhuolib/clients.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      348 2024-04-25 14:26:18.000000 dhuodata_lib-0.2.5/src/dhuolib/config.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-04-24 18:22:52.000000 dhuodata_lib-0.2.5/src/dhuolib/predict.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2017 2024-05-07 17:00:57.000000 dhuodata_lib-0.2.5/src/dhuolib/services.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      789 2024-05-07 16:57:09.000000 dhuodata_lib-0.2.5/src/dhuolib/validations.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata_lib-0.2.5/src/dhuolib/worker.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-07 17:02:09.127812 dhuodata_lib-0.2.5/tests/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     3550 2024-05-07 16:59:04.000000 dhuodata_lib-0.2.5/tests/test_dhuolib.py
```

### Comparing `dhuodata_lib-0.2.4/PKG-INFO` & `dhuodata_lib-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.2.4
+Version: 0.2.5
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Requires-Dist: oci==2.125.3
 Requires-Dist: pydantic==1.8.2
```

### Comparing `dhuodata_lib-0.2.4/README.md` & `dhuodata_lib-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.2.4/setup.py` & `dhuodata_lib-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 README = ""
 if os.path.exists("README.md"):
     README = open("README.md").read()
 
 setup(
     name="dhuodata-lib",
-    version="0.2.4",
+    version="0.2.5",
     long_description=README,
     long_description_content_type="text/markdown",
     author="DHuO Data Team",
     author_email="diego.salles@engdb.com.br",
     url="https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib",
     install_requires=REQUIRED_PACKAGES,
     extras_require={"interactive": DEV_PACKAGES},
```

### Comparing `dhuodata_lib-0.2.4/src/dhuodata_lib.egg-info/PKG-INFO` & `dhuodata_lib-0.2.5/src/dhuodata_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.2.4
+Version: 0.2.5
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Requires-Dist: oci==2.125.3
 Requires-Dist: pydantic==1.8.2
```

### Comparing `dhuodata_lib-0.2.4/src/dhuolib/predict.py` & `dhuodata_lib-0.2.5/src/dhuolib/predict.py`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.2.4/src/dhuolib/validations.py` & `dhuodata_lib-0.2.5/src/dhuolib/validations.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from pydantic import BaseModel, Field
 
 
 class RunExperimentBody(BaseModel):
-    modelname: str = Field(..., description="DEPENDENCY|PREDICT")
-    modeltag: str = Field(..., description="Tag")
     experiment_id: str = Field(..., description="Id")
-    stage: str = Field(..., description="STAGING|PRODUCTION")
-    requirements_file: str = Field(None, description="STAGING|PRODUCTION")
-    model_pkl_file: str = Field(None, description="STAGING|PRODUCTION")
+    requirements_file: str = Field(..., description="STAGING|PRODUCTION")
+    model_pkl_file: str = Field(..., description="STAGING|PRODUCTION")
 
 
 class ExperimentBody(BaseModel):
     experiment_name: str = Field(..., description="Id")
     experiment_tags: dict = Field(..., description="Tags")
-    requirements_file: str = Field(..., description="STAGING|PRODUCTION")
-    model_pkl_file: str = Field(..., description="STAGING|PRODUCTION")
+    requirements_file: str = Field(None, description="STAGING|PRODUCTION")
+    model_pkl_file: str = Field(None, description="STAGING|PRODUCTION")
+
+
+class PredictModelBody(BaseModel):
+    run_id: str = Field(None, description="Run ID")
+    modelname: str = Field(..., description="DEPENDENCY|PREDICT")
+    stage: str = Field(..., description="STAGING|PRODUCTION")
```

### Comparing `dhuodata_lib-0.2.4/tests/test_dhuolib.py` & `dhuodata_lib-0.2.5/tests/test_dhuolib.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,100 @@
-import json
+from dhuolib.clients import DhuolibClient
 import sys
 import unittest
-from unittest.mock import MagicMock, patch
+from unittest.mock import patch
 
 sys.path.append("src")
-from dhuolib.clients import DhuolibClient
 
 
 class TestDhuolibUtils(unittest.TestCase):
     def setUp(self):
         self.end_point = "http://localhost:8000"
         self.dhuolib = DhuolibClient(service_endpoint=self.end_point)
         self.file_path = "tests/files/LogisticRegression_best.pickle"
-        
-    # def test_integracao(self):
-    #     experiment_params = {
-    #         "experiment_name": "test_experiment_nlp",
-    #         "experiment_tags": {"version": "v1", "priority": "P1"},
-    #         "model_pkl_file": "tests/files/LogisticRegression_best.pickle",
-    #         "requirements_file": "tests/files/requirements.txt"
-    #     }
-
-    #     response = self.dhuolib.create_experiment(experiment_params)
 
-        
     def test_deve_lancar_excecao_com_valores_run_params_incorretos(self):
         experiment_params = {
-            "experiment_name": "test_experiment",
-            "experiment_tags": {"version": "v1", "priority": "P1"}
+            "experiment_tags": {"version": "v1", "priority": "P1"},
         }
         response = self.dhuolib.create_experiment(experiment_params)
         self.assertEqual(list(response.keys()), ["error"])
 
     @patch("requests.post")
-    def test_deve_criar_o_experimento_com_run_params_corretos(
-        self, mock_post
-    ):
+    def test_deve_criar_o_experimento_com_run_params_corretos(self, mock_post):
         client = DhuolibClient(service_endpoint=self.end_point)
 
         mock_response = mock_post.return_value
         mock_response.status_code = 201
         mock_response.json.return_value = {"experiment_id": "1"}
 
         experiment_params = {
             "experiment_name": "test_experiment",
-            "experiment_tags": {"version": "v1", "priority": "P1"},
-            "model_pkl_file": "tests/files/LogisticRegression_best.pickle",
-            "requirements_file": "tests/files/requirements.txt"
+            "experiment_tags": {"version": "v1", "priority": "P1"}
         }
-        
+
         response = client.create_experiment(experiment_params)
         self.assertEqual(response, mock_response.json.return_value)
-        
+
     @patch("requests.post")
     def test_deve_executar_o_experimento_com_run_params_corretos(self, mock_post):
         mock_response = mock_post.return_value
         mock_response.status_code = 201
         mock_response.json.return_value = {
+            "experiment_id": "experiment_id",
+            "run_id": "run_id",
+            "model_uri": "model_uri",
+        }
+
+        run_params = {
+            "experiment_id": "2",
+            "model_pkl_file": "tests/files/LogisticRegression_best.pickle",
+            "requirements_file": "tests/files/requirements.txt",
+        }
+        response = self.dhuolib.run_experiment(run_params)
+
+        self.assertEqual(response, mock_response.json.return_value)
+
+    @patch("requests.post")
+    def test_deve_criar_modelo_com_run_params_corretos(self, mock_post):
+        mock_response = mock_post.return_value
+        mock_response.status_code = 201
+        mock_response.json.return_value = {
             "current_stage": "Production",
             "last_updated_timestamp": 1713582060414,
             "model_version": "1",
             "run_id": "9434e517ed104958b6f5f47d33c79184",
             "status": "READY",
         }
 
         run_params = {
-            "experiment_id": '2',
             "stage": "Production",
             "modelname": "nlp_framework",
             "modeltag": "v1",
-            "model_pkl_file": "tests/files/LogisticRegression_best.pickle",
-            "requirements_file": "tests/files/requirements.txt"
+            "run_id": "9434e517ed104958b6f5f47d33c79184",
+            "requirements_file": "tests/files/requirements.txt",
+            "model_uri": "model_uri"
+        }
+
+        response = self.dhuolib.create_model(run_params)
+
+        self.assertEqual(response, mock_response.json.return_value)
+
+    @patch("requests.post")
+    def test_deve_fazer_o_predict_online_a_partir_de_um_dataset(self, mock_post):
+        mock_response = mock_post.return_value
+        mock_response.status_code = 201
+        mock_response.json.return_value = {
+            "model_name": "nlp_framework",
+            "predictions": [0, 1, 0, 1, 0, 1, 0, 1, 0, 1],
         }
-        response = self.dhuolib.run_experiment(run_params)
 
-        self.assertEqual(response, mock_response.json.return_value)
+        run_params = {
+            "stage": "Production",
+            "data": "tests/files/data_predict.csv",
+            "modelname": "nlp_framework",
+
+        }
+
+        response = self.dhuolib.predict_online(run_params)
+
+        self.assertEqual(response, mock_response.json.return_value)
```

