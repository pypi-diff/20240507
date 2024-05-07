# Comparing `tmp/test_nvf_builds-0.0.2.tar.gz` & `tmp/test_nvf_builds-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_nvf_builds-0.0.2.tar", last modified: Mon May  6 15:42:05 2024, max compression
+gzip compressed data, was "test_nvf_builds-0.0.3.tar", last modified: Mon May  6 16:00:07 2024, max compression
```

## Comparing `test_nvf_builds-0.0.2.tar` & `test_nvf_builds-0.0.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 15:42:05.659165 test_nvf_builds-0.0.2/
--rw-r--r--   0 mostafa    (501) staff       (20)      402 2024-05-06 15:42:05.659096 test_nvf_builds-0.0.2/PKG-INFO
--rw-r--r--   0 mostafa    (501) staff       (20)       85 2024-05-06 07:53:59.000000 test_nvf_builds-0.0.2/README.md
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 15:42:05.654161 test_nvf_builds-0.0.2/oasysnow/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:25.000000 test_nvf_builds-0.0.2/oasysnow/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 15:42:05.654263 test_nvf_builds-0.0.2/oasysnow/nvflare/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:50:57.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 15:42:05.654359 test_nvf_builds-0.0.2/oasysnow/nvflare/client/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:25:11.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/client/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 15:42:05.654996 test_nvf_builds-0.0.2/oasysnow/nvflare/client/filters/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:35.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/client/filters/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     3468 2024-05-02 11:52:22.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/client/filters/filter_data.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2471 2024-05-02 11:52:22.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/client/filters/filter_results.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 15:42:05.655504 test_nvf_builds-0.0.2/oasysnow/nvflare/client/trainer/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:41.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/client/trainer/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     5232 2024-05-02 13:52:34.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/client/trainer/trainer.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 15:42:05.656214 test_nvf_builds-0.0.2/oasysnow/nvflare/model/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:36:02.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/model/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2460 2024-05-02 13:22:42.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/model/gennet_model.py
--rw-r--r--   0 mostafa    (501) staff       (20)     1928 2024-05-02 13:26:14.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/model/global_model.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 15:42:05.656458 test_nvf_builds-0.0.2/oasysnow/nvflare/server/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:11.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/server/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 15:42:05.656961 test_nvf_builds-0.0.2/oasysnow/nvflare/server/filters/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:45.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/server/filters/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 15:42:05.657457 test_nvf_builds-0.0.2/oasysnow/nvflare/server/filters/attestation_service/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:56:34.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/server/filters/attestation_service/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:46:21.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/server/filters/attestation_service/server.py
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:56:28.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/server/filters/attestation_service/verification.py
--rw-r--r--   0 mostafa    (501) staff       (20)     4442 2024-05-03 13:51:03.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/server/filters/filter_data.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2475 2024-04-19 21:41:54.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/server/filters/filter_results.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 15:42:05.657669 test_nvf_builds-0.0.2/oasysnow/nvflare/server/model_runner/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:45:46.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/server/model_runner/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     5422 2024-05-02 14:00:51.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/server/model_runner/model_runner.py
--rw-r--r--   0 mostafa    (501) staff       (20)       36 2024-05-06 15:40:29.000000 test_nvf_builds-0.0.2/requirements.txt
--rw-r--r--   0 mostafa    (501) staff       (20)      435 2024-05-06 15:42:05.659415 test_nvf_builds-0.0.2/setup.cfg
--rw-r--r--   0 mostafa    (501) staff       (20)      322 2024-05-06 15:10:01.000000 test_nvf_builds-0.0.2/setup.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 15:42:05.658849 test_nvf_builds-0.0.2/test_nvf_builds.egg-info/
--rw-r--r--   0 mostafa    (501) staff       (20)      402 2024-05-06 15:42:05.000000 test_nvf_builds-0.0.2/test_nvf_builds.egg-info/PKG-INFO
--rw-r--r--   0 mostafa    (501) staff       (20)     1139 2024-05-06 15:42:05.000000 test_nvf_builds-0.0.2/test_nvf_builds.egg-info/SOURCES.txt
--rw-r--r--   0 mostafa    (501) staff       (20)        1 2024-05-06 15:42:05.000000 test_nvf_builds-0.0.2/test_nvf_builds.egg-info/dependency_links.txt
--rw-r--r--   0 mostafa    (501) staff       (20)       36 2024-05-06 15:42:05.000000 test_nvf_builds-0.0.2/test_nvf_builds.egg-info/requires.txt
--rw-r--r--   0 mostafa    (501) staff       (20)        9 2024-05-06 15:42:05.000000 test_nvf_builds-0.0.2/test_nvf_builds.egg-info/top_level.txt
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 16:00:07.405554 test_nvf_builds-0.0.3/
+-rw-r--r--   0 mostafa    (501) staff       (20)      402 2024-05-06 16:00:07.405484 test_nvf_builds-0.0.3/PKG-INFO
+-rw-r--r--   0 mostafa    (501) staff       (20)       85 2024-05-06 07:53:59.000000 test_nvf_builds-0.0.3/README.md
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 16:00:07.400495 test_nvf_builds-0.0.3/oasysnow/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:25.000000 test_nvf_builds-0.0.3/oasysnow/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 16:00:07.400629 test_nvf_builds-0.0.3/oasysnow/federated/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:50:57.000000 test_nvf_builds-0.0.3/oasysnow/federated/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 16:00:07.400750 test_nvf_builds-0.0.3/oasysnow/federated/client/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:25:11.000000 test_nvf_builds-0.0.3/oasysnow/federated/client/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 16:00:07.401459 test_nvf_builds-0.0.3/oasysnow/federated/client/filters/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:35.000000 test_nvf_builds-0.0.3/oasysnow/federated/client/filters/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     3468 2024-05-06 15:57:38.000000 test_nvf_builds-0.0.3/oasysnow/federated/client/filters/filter_data.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2471 2024-05-06 15:57:38.000000 test_nvf_builds-0.0.3/oasysnow/federated/client/filters/filter_results.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 16:00:07.401982 test_nvf_builds-0.0.3/oasysnow/federated/client/trainer/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:41.000000 test_nvf_builds-0.0.3/oasysnow/federated/client/trainer/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     5234 2024-05-06 15:59:26.000000 test_nvf_builds-0.0.3/oasysnow/federated/client/trainer/trainer.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 16:00:07.402730 test_nvf_builds-0.0.3/oasysnow/federated/model/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:36:02.000000 test_nvf_builds-0.0.3/oasysnow/federated/model/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2460 2024-05-02 13:22:42.000000 test_nvf_builds-0.0.3/oasysnow/federated/model/gennet_model.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     1930 2024-05-06 15:58:12.000000 test_nvf_builds-0.0.3/oasysnow/federated/model/global_model.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 16:00:07.402996 test_nvf_builds-0.0.3/oasysnow/federated/server/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:11.000000 test_nvf_builds-0.0.3/oasysnow/federated/server/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 16:00:07.403408 test_nvf_builds-0.0.3/oasysnow/federated/server/filters/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:45.000000 test_nvf_builds-0.0.3/oasysnow/federated/server/filters/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 16:00:07.403919 test_nvf_builds-0.0.3/oasysnow/federated/server/filters/attestation_service/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:56:34.000000 test_nvf_builds-0.0.3/oasysnow/federated/server/filters/attestation_service/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:46:21.000000 test_nvf_builds-0.0.3/oasysnow/federated/server/filters/attestation_service/server.py
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:56:28.000000 test_nvf_builds-0.0.3/oasysnow/federated/server/filters/attestation_service/verification.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     4442 2024-05-06 15:57:39.000000 test_nvf_builds-0.0.3/oasysnow/federated/server/filters/filter_data.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2475 2024-04-19 21:41:54.000000 test_nvf_builds-0.0.3/oasysnow/federated/server/filters/filter_results.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 16:00:07.404167 test_nvf_builds-0.0.3/oasysnow/federated/server/model_runner/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:45:46.000000 test_nvf_builds-0.0.3/oasysnow/federated/server/model_runner/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     5424 2024-05-06 15:59:11.000000 test_nvf_builds-0.0.3/oasysnow/federated/server/model_runner/model_runner.py
+-rw-r--r--   0 mostafa    (501) staff       (20)       36 2024-05-06 15:40:29.000000 test_nvf_builds-0.0.3/requirements.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)      435 2024-05-06 16:00:07.405815 test_nvf_builds-0.0.3/setup.cfg
+-rw-r--r--   0 mostafa    (501) staff       (20)      322 2024-05-06 15:10:01.000000 test_nvf_builds-0.0.3/setup.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 16:00:07.405241 test_nvf_builds-0.0.3/test_nvf_builds.egg-info/
+-rw-r--r--   0 mostafa    (501) staff       (20)      402 2024-05-06 16:00:07.000000 test_nvf_builds-0.0.3/test_nvf_builds.egg-info/PKG-INFO
+-rw-r--r--   0 mostafa    (501) staff       (20)     1177 2024-05-06 16:00:07.000000 test_nvf_builds-0.0.3/test_nvf_builds.egg-info/SOURCES.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)        1 2024-05-06 16:00:07.000000 test_nvf_builds-0.0.3/test_nvf_builds.egg-info/dependency_links.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)       36 2024-05-06 16:00:07.000000 test_nvf_builds-0.0.3/test_nvf_builds.egg-info/requires.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)        9 2024-05-06 16:00:07.000000 test_nvf_builds-0.0.3/test_nvf_builds.egg-info/top_level.txt
```

### Comparing `test_nvf_builds-0.0.2/oasysnow/nvflare/client/filters/filter_data.py` & `test_nvf_builds-0.0.3/oasysnow/federated/client/filters/filter_data.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.2/oasysnow/nvflare/client/filters/filter_results.py` & `test_nvf_builds-0.0.3/oasysnow/federated/client/filters/filter_results.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.2/oasysnow/nvflare/client/trainer/trainer.py` & `test_nvf_builds-0.0.3/oasysnow/federated/client/trainer/trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from nvflare.apis.fl_context import FLContext
 from nvflare.apis.fl_constant import FLContextKey, ReturnCode
 from nvflare.app_common.app_constant import AppConstants
 from nvflare.apis.shareable import Shareable, make_reply
 from nvflare.apis.signal import Signal
 from gennet.utils.Dataloader import *
 from gennet.utils.Utility_functions import *
-from oasysnow.nvflare.model.global_model import GlobalModel
+from oasysnow.federated.model.global_model import GlobalModel
 
 import random
 
 
 class Trainer(Executor):
     def __init__(self, epochs_per_round):
         super().__init__()
```

### Comparing `test_nvf_builds-0.0.2/oasysnow/nvflare/model/gennet_model.py` & `test_nvf_builds-0.0.3/oasysnow/federated/model/gennet_model.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.2/oasysnow/nvflare/model/global_model.py` & `test_nvf_builds-0.0.3/oasysnow/federated/model/global_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import tensorflow as tf
 from gennet.utils.LocallyDirected1D import LocallyDirected1D
 from gennet.utils.Utility_functions import sensitivity, specificity
-from oasysnow.nvflare.model.gennet_model import GenNet
+from oasysnow.federated.model.gennet_model import GenNet
 import pathlib
 
 class GlobalModel():
     def __init__(self):
 
         self.weight_positive_class = 2
         self.weight_negative_class = 1
```

### Comparing `test_nvf_builds-0.0.2/oasysnow/nvflare/server/filters/filter_data.py` & `test_nvf_builds-0.0.3/oasysnow/federated/server/filters/filter_data.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.2/oasysnow/nvflare/server/filters/filter_results.py` & `test_nvf_builds-0.0.3/oasysnow/federated/server/filters/filter_results.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.2/oasysnow/nvflare/server/model_runner/model_runner.py` & `test_nvf_builds-0.0.3/oasysnow/federated/server/model_runner/model_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from nvflare.apis.fl_context import FLContext
 from nvflare.app_common.abstract.model import ModelLearnable
 from nvflare.app_common.abstract.model import make_model_learnable
 from nvflare.app_common.abstract.model_persistor import ModelPersistor
 from nvflare.app_common.app_constant import AppConstants
 import nvflare.app_common.shareablegenerators.full_model_shareable_generator as SG
 import numpy as np
-from oasysnow.nvflare.model.global_model import GlobalModel
+from oasysnow.federated.model.global_model import GlobalModel
 
 
 class ModelRunner(ModelPersistor):
     def __init__(self, save_name="tf2_model.pkl"):
         super().__init__()
         self.save_name = save_name
         self.inputsize = 100
```

