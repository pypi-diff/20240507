# Comparing `tmp/dltrain-0.0.4.tar.gz` & `tmp/dltrain-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dltrain-0.0.4.tar", last modified: Sat May  4 14:02:03 2024, max compression
+gzip compressed data, was "dltrain-0.1.0.tar", last modified: Tue May  7 03:11:00 2024, max compression
```

## Comparing `dltrain-0.0.4.tar` & `dltrain-0.1.0.tar`

### file list

```diff
@@ -1,36 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 14:02:03.826791 dltrain-0.0.4/
--rw-rw-rw-   0        0        0     1091 2024-04-07 09:17:30.000000 dltrain-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      813 2024-05-04 14:02:03.825799 dltrain-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      174 2024-04-07 12:04:01.000000 dltrain-0.0.4/README.md
--rw-rw-rw-   0        0        0      625 2024-04-08 10:01:12.000000 dltrain-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-04 14:02:03.826791 dltrain-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-04 14:02:03.783791 dltrain-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-04 14:02:03.801791 dltrain-0.0.4/src/dltrain/
--rw-rw-rw-   0        0        0      219 2024-04-07 09:09:29.000000 dltrain-0.0.4/src/dltrain/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 14:02:03.823792 dltrain-0.0.4/src/dltrain/builder/
--rw-rw-rw-   0        0        0       32 2024-05-04 13:43:22.000000 dltrain-0.0.4/src/dltrain/builder/__init__.py
--rw-rw-rw-   0        0        0     1132 2024-05-04 11:16:47.000000 dltrain-0.0.4/src/dltrain/builder/base.py
--rw-rw-rw-   0        0        0     3623 2024-05-04 13:52:21.000000 dltrain-0.0.4/src/dltrain/builder/builder.py
--rw-rw-rw-   0        0        0      212 2024-05-04 13:37:24.000000 dltrain-0.0.4/src/dltrain/builder/core.py
--rw-rw-rw-   0        0        0      613 2024-05-04 13:43:22.000000 dltrain-0.0.4/src/dltrain/builder/criterion.py
--rw-rw-rw-   0        0        0     1377 2024-05-04 13:34:54.000000 dltrain-0.0.4/src/dltrain/builder/evaluation_handler.py
--rw-rw-rw-   0        0        0      631 2024-05-04 13:34:54.000000 dltrain-0.0.4/src/dltrain/builder/model.py
--rw-rw-rw-   0        0        0     1143 2024-05-04 13:53:40.000000 dltrain-0.0.4/src/dltrain/builder/optimizer.py
--rw-rw-rw-   0        0        0      533 2024-05-04 13:52:21.000000 dltrain-0.0.4/src/dltrain/builder/scheduler.py
--rw-rw-rw-   0        0        0      718 2024-05-04 13:34:54.000000 dltrain-0.0.4/src/dltrain/builder/transforms.py
--rw-rw-rw-   0        0        0      747 2024-04-07 09:09:29.000000 dltrain-0.0.4/src/dltrain/checkpoint.py
--rw-rw-rw-   0        0        0     6069 2024-04-08 10:00:24.000000 dltrain-0.0.4/src/dltrain/dataset.py
--rw-rw-rw-   0        0        0     1235 2024-04-07 09:09:29.000000 dltrain-0.0.4/src/dltrain/delineator.py
--rw-rw-rw-   0        0        0      935 2024-05-03 11:30:58.000000 dltrain-0.0.4/src/dltrain/error.py
--rw-rw-rw-   0        0        0     2644 2024-05-04 03:27:06.000000 dltrain-0.0.4/src/dltrain/evaluation.py
--rw-rw-rw-   0        0        0     1738 2024-04-07 09:09:29.000000 dltrain-0.0.4/src/dltrain/forward.py
--rw-rw-rw-   0        0        0     4489 2024-04-07 09:09:29.000000 dltrain-0.0.4/src/dltrain/models.py
--rw-rw-rw-   0        0        0     1290 2024-04-07 09:09:29.000000 dltrain-0.0.4/src/dltrain/options.py
--rw-rw-rw-   0        0        0    11789 2024-05-04 03:27:06.000000 dltrain-0.0.4/src/dltrain/train.py
--rw-rw-rw-   0        0        0     1145 2024-04-07 09:09:29.000000 dltrain-0.0.4/src/dltrain/transform.py
--rw-rw-rw-   0        0        0     5417 2024-04-07 08:49:36.000000 dltrain-0.0.4/src/dltrain/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-04 14:02:03.824792 dltrain-0.0.4/src/dltrain.egg-info/
--rw-rw-rw-   0        0        0      813 2024-05-04 14:02:03.000000 dltrain-0.0.4/src/dltrain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      776 2024-05-04 14:02:03.000000 dltrain-0.0.4/src/dltrain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 14:02:03.000000 dltrain-0.0.4/src/dltrain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-04 14:02:03.000000 dltrain-0.0.4/src/dltrain.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 03:11:00.555852 dltrain-0.1.0/
+-rw-rw-rw-   0        0        0     1091 2024-04-07 09:17:30.000000 dltrain-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      813 2024-05-07 03:11:00.554853 dltrain-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2024-04-07 12:04:01.000000 dltrain-0.1.0/README.md
+-rw-rw-rw-   0        0        0      625 2024-05-07 03:10:37.000000 dltrain-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-07 03:11:00.555852 dltrain-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-07 03:11:00.367330 dltrain-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-07 03:11:00.464333 dltrain-0.1.0/src/dltrain/
+-rw-rw-rw-   0        0        0      229 2024-05-05 13:13:52.000000 dltrain-0.1.0/src/dltrain/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:11:00.551857 dltrain-0.1.0/src/dltrain/builder/
+-rw-rw-rw-   0        0        0       32 2024-05-04 13:43:22.000000 dltrain-0.1.0/src/dltrain/builder/__init__.py
+-rw-rw-rw-   0        0        0     1207 2024-05-07 01:28:09.000000 dltrain-0.1.0/src/dltrain/builder/base.py
+-rw-rw-rw-   0        0        0     3219 2024-05-07 03:07:53.000000 dltrain-0.1.0/src/dltrain/builder/builder.py
+-rw-rw-rw-   0        0        0      212 2024-05-04 13:37:24.000000 dltrain-0.1.0/src/dltrain/builder/core.py
+-rw-rw-rw-   0        0        0      714 2024-05-05 13:08:13.000000 dltrain-0.1.0/src/dltrain/builder/criterion.py
+-rw-rw-rw-   0        0        0     1177 2024-05-05 13:08:13.000000 dltrain-0.1.0/src/dltrain/builder/dataset.py
+-rw-rw-rw-   0        0        0      721 2024-05-05 13:08:13.000000 dltrain-0.1.0/src/dltrain/builder/delineator.py
+-rw-rw-rw-   0        0        0     1556 2024-05-05 13:08:13.000000 dltrain-0.1.0/src/dltrain/builder/evaluation.py
+-rw-rw-rw-   0        0        0      488 2024-05-07 01:12:49.000000 dltrain-0.1.0/src/dltrain/builder/forward.py
+-rw-rw-rw-   0        0        0      281 2024-05-07 03:07:32.000000 dltrain-0.1.0/src/dltrain/builder/inject.py
+-rw-rw-rw-   0        0        0      840 2024-05-05 13:08:13.000000 dltrain-0.1.0/src/dltrain/builder/model.py
+-rw-rw-rw-   0        0        0     1169 2024-05-07 01:28:56.000000 dltrain-0.1.0/src/dltrain/builder/optimizer.py
+-rw-rw-rw-   0        0        0      533 2024-05-04 13:52:21.000000 dltrain-0.1.0/src/dltrain/builder/scheduler.py
+-rw-rw-rw-   0        0        0      718 2024-05-05 13:08:13.000000 dltrain-0.1.0/src/dltrain/builder/transforms.py
+-rw-rw-rw-   0        0        0      747 2024-04-07 09:09:29.000000 dltrain-0.1.0/src/dltrain/checkpoint.py
+-rw-rw-rw-   0        0        0     5177 2024-05-05 13:08:13.000000 dltrain-0.1.0/src/dltrain/dataset.py
+-rw-rw-rw-   0        0        0     1300 2024-05-05 13:08:13.000000 dltrain-0.1.0/src/dltrain/delineator.py
+-rw-rw-rw-   0        0        0      935 2024-05-03 11:30:58.000000 dltrain-0.1.0/src/dltrain/error.py
+-rw-rw-rw-   0        0        0     3949 2024-05-05 13:08:13.000000 dltrain-0.1.0/src/dltrain/evaluation.py
+-rw-rw-rw-   0        0        0     6478 2024-05-07 02:10:02.000000 dltrain-0.1.0/src/dltrain/forward.py
+-rw-rw-rw-   0        0        0     1203 2024-05-07 03:07:32.000000 dltrain-0.1.0/src/dltrain/inject.py
+-rw-rw-rw-   0        0        0     4523 2024-05-07 02:14:49.000000 dltrain-0.1.0/src/dltrain/models.py
+-rw-rw-rw-   0        0        0     1290 2024-04-07 09:09:29.000000 dltrain-0.1.0/src/dltrain/options.py
+-rw-rw-rw-   0        0        0    11930 2024-05-07 02:10:30.000000 dltrain-0.1.0/src/dltrain/train.py
+-rw-rw-rw-   0        0        0     1145 2024-04-07 09:09:29.000000 dltrain-0.1.0/src/dltrain/transform.py
+-rw-rw-rw-   0        0        0     5417 2024-04-07 08:49:36.000000 dltrain-0.1.0/src/dltrain/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:11:00.553864 dltrain-0.1.0/src/dltrain.egg-info/
+-rw-rw-rw-   0        0        0      813 2024-05-07 03:11:00.000000 dltrain-0.1.0/src/dltrain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      916 2024-05-07 03:11:00.000000 dltrain-0.1.0/src/dltrain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 03:11:00.000000 dltrain-0.1.0/src/dltrain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-07 03:11:00.000000 dltrain-0.1.0/src/dltrain.egg-info/top_level.txt
```

### Comparing `dltrain-0.0.4/LICENSE` & `dltrain-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.4/PKG-INFO` & `dltrain-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dltrain
-Version: 0.0.4
+Version: 0.1.0
 Summary: This is a package for PyTorch training, and this project provides a large number of high-level training APIs and low-level interfaces to meet all training needs
 Author-email: XiaosYu <lijingyu_ai@163.com>
 Project-URL: Homepage, https://github.com/XiaosYu/dltrain
 Project-URL: Bug Tracker, https://github.com/XiaosYu/dltrain/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dltrain-0.0.4/pyproject.toml` & `dltrain-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dltrain"
-version = "0.0.4"
+version = "0.1.0"
 authors = [
   { name="XiaosYu", email="lijingyu_ai@163.com" },
 ]
 description = "This is a package for PyTorch training, and this project provides a large number of high-level training APIs and low-level interfaces to meet all training needs"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dltrain-0.0.4/src/dltrain/builder/base.py` & `dltrain-0.1.0/src/dltrain/builder/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from typing import Union
+
 from .core import Wizard
+from ..checkpoint import CheckPoint
+
 import torch
 
 
 class BaseWizard(Wizard):
     def __init__(self):
         self._batch_size = 16
         self._seed = 3407
@@ -20,17 +23,17 @@
         self._seed = seed
         return self
 
     def set_checkpoint(self, checkpoint: bool = False):
         self._save_checkpoint = checkpoint
         return self
 
-    def use_checkpoint(self, checkpoint_path: str):
-        self._start_checkpoint = checkpoint_path
-        return self
+    def use_checkpoint(self, checkpoint: str) -> CheckPoint:
+        self._start_checkpoint = torch.load(checkpoint)
+        return self._start_checkpoint
 
     def use_epoch(self, epochs: int = 10):
         self._epochs = epochs
         return self
 
     def use_device(self, device: Union[torch.device, str]):
         if isinstance(device, str):
```

### Comparing `dltrain-0.0.4/src/dltrain/builder/builder.py` & `dltrain-0.1.0/src/dltrain/builder/builder.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,63 +1,46 @@
 import string
 import random
-from typing import Dict
 
-import torch
-
-from dltrain.forward import Forward, SimpleForward
-from dltrain.delineator import Delineator, TrainEvalSetDelineator, RandomSplitDelineator
-from dltrain.transform import Container
-from dltrain.dataset import DLDataset
-
-from torch.nn import Module, CrossEntropyLoss, MSELoss
-from torch.optim import Optimizer, Adam
-from torch import device
-from torch.optim.lr_scheduler import LRScheduler
 
+from ..transform import Container
+from .inject import InjectWizard
 from ..options import TrainOptions
 from .optimizer import OptimizerWizard
 from .scheduler import SchedulerWizard
 from .base import BaseWizard
 from .criterion import CriterionWizard
-from .evaluation_handler import EvaluationWizard
+from .evaluation import EvaluationWizard
 from .model import ModelWizard
 from .transforms import TransformWizard
-from ..dataset import DatasetWizard
+from .dataset import DatasetWizard
+from .delineator import DelineatorWizard
+from .forward import ForwardWizard
 
 __all__ = [
     'TaskBuilder'
 ]
 
 
 class TaskBuilder:
     def __init__(self, task_name=None):
         self.task_name: str = task_name if task_name is not None else ''.join(
             random.choices(string.digits + string.ascii_letters, k=5))
 
-        self._forward: Forward = SimpleForward()
-        self._delineator: Delineator = None
-
+        self.forward = ForwardWizard()
         self.evaluation_handler = EvaluationWizard()
         self.optimizer = OptimizerWizard()
         self.base = BaseWizard()
         self.criterion = CriterionWizard()
         self.scheduler = SchedulerWizard()
         self.model = ModelWizard()
         self.transform = TransformWizard()
         self.dataset = DatasetWizard()
-
-    def use_forward(self, forward: Forward):
-        self._forward = forward
-
-    def use_train_eval_set(self, train_set: DLDataset, eval_set: DLDataset):
-        self._delineator = TrainEvalSetDelineator(train_set, eval_set)
-
-    def use_random_split_dataset(self, dataset: DLDataset, train=0.8, eval=0.2):
-        self._delineator = RandomSplitDelineator(dataset, train, eval)
+        self.delineator = DelineatorWizard()
+        self.inject = InjectWizard()
 
     def build(self):
         options = TrainOptions()
         options.task_name = self.task_name
 
         # 载入优化器
         optimizer = self.optimizer.get_kwargs()
@@ -90,13 +73,19 @@
 
         # 载入数据变换
         transform = self.transform.get_kwargs()
         options.features_transform = Container(transform['features_transform'])
         options.targets_transform = Container(transform['targets_transform'])
 
         # 数据集设置
-        options.delineator = self._delineator
+        options.delineator = self.delineator.get_kwargs()['delineator']
 
         # 设置前馈
-        options.forward = self._forward
+        options.forward = self.forward.get_kwargs()['forward']
+
+        # 载入注入
+        injects = self.inject.get_kwargs()['injects']
+        if hasattr(options.forward, 'bind'):
+            for inject in injects:
+                options.forward.bind(inject)
 
         return options
```

### Comparing `dltrain-0.0.4/src/dltrain/builder/criterion.py` & `dltrain-0.1.0/src/dltrain/builder/criterion.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 from torch import nn
 
 class CriterionWizard(Wizard):
     def __init__(self):
         self._criterion = None
 
+    def use_criterion(self, criterion):
+        self._criterion = criterion
+        return self
+
     def use_mse(self):
         self._criterion = nn.MSELoss()
         return self
 
     def use_l1(self):
         self._criterion = nn.L1Loss()
         return self
```

### Comparing `dltrain-0.0.4/src/dltrain/builder/model.py` & `dltrain-0.1.0/src/dltrain/builder/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 from .core import Wizard
-from ..models import MultilayerPerceptron, PyTorchNativeCNN, create_native_model
+from ..models import MultilayerPerceptron, PyTorchNativeCNN, create_native_model, Module
 
 
 class ModelWizard(Wizard):
     def __init__(self):
         self._model = None
 
+    def use_model(self, model: Module):
+        self._model = model
+        return self
+
     def use_mlp(self, features, targets, layers=None, activation='sigmoid'):
         model = MultilayerPerceptron(features, targets, layers, activation)
         self._model = model
 
     def use_pytorch_model(self, model_name: str, num_classes: int, pretrained: bool = False):
         model = create_native_model(model_name, num_classes, pretrained=pretrained)
         model = PyTorchNativeCNN(model)
         self._model = model
+
+    def use_resnet18(self, num_classes):
+        return self.use_pytorch_model('resnet18', num_classes)
```

### Comparing `dltrain-0.0.4/src/dltrain/builder/optimizer.py` & `dltrain-0.1.0/src/dltrain/builder/optimizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 
 class OptimizerWizard(Wizard):
     def __init__(self):
         self._type = None
         self._parameters = {}
 
+        self.use_sgd()
+
     def use_optimizer(self, optimizer: type[Optimizer], **kwargs):
         self._type = optimizer
         self._parameters = kwargs
         return self
 
     def use_sgd(self, lr=1e-2, momentum=0, dampening=0, weight_decay=0):
         return self.use_optimizer(SGD, lr=lr, momentum=momentum, dampening=dampening, weight_decay=weight_decay)
```

### Comparing `dltrain-0.0.4/src/dltrain/builder/scheduler.py` & `dltrain-0.1.0/src/dltrain/builder/scheduler.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.4/src/dltrain/builder/transforms.py` & `dltrain-0.1.0/src/dltrain/builder/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from ..transform import Transform, Standardize, Resize
 from .core import Wizard
 
+
 class TransformWizard(Wizard):
     def __init__(self):
         self._features_transform = []
         self._targets_transform = []
 
-    def add_transform(self, transform: Transform, is_feature = True):
+    def add_transform(self, transform: Transform, is_feature=True):
         if is_feature:
             self._features_transform.append(transform)
         else:
             self._targets_transform.append(transform)
 
         return self
```

### Comparing `dltrain-0.0.4/src/dltrain/checkpoint.py` & `dltrain-0.1.0/src/dltrain/checkpoint.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.4/src/dltrain/dataset.py` & `dltrain-0.1.0/src/dltrain/dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,69 +3,34 @@
 from torch import Tensor, cat
 from abc import ABCMeta, abstractmethod
 from .error import check_length, try_convert, raise_error
 
 import os
 
 __all__ = [
-    'DatasetWizard',
     'DLDataset',
     'VectorCategoricalDataset',
     'VectorRegressionDataset',
     'PyTorchNativeDataset',
-    'ImageCategoricalDataset'
+    'ImageCategoricalDataset',
+    'EmptyDataset'
 ]
 
 
 def load_images(folder_name):
     from PIL import Image
     from torchvision.transforms.functional import to_tensor
 
     images = []
     for filename in os.listdir(folder_name):
         image = Image.open(filename)
         images.append(to_tensor(image))
 
     return torch.Tensor(images)
 
-class DatasetWizard:
-    @classmethod
-    def use_mnist(cls, root, train, download=False):
-        from torchvision.datasets import MNIST
-        from torchvision.transforms import ToTensor
-
-        dataset = MNIST(root, train=train, transform=ToTensor(), download=download)
-        return PyTorchNativeDataset(dataset)
-
-    @classmethod
-    def use_iris(cls):
-        from sklearn.datasets import load_iris
-
-        iris = load_iris()
-        data = iris.data
-        target = iris.target
-        return VectorCategoricalDataset(data, target)
-
-    @classmethod
-    def use_image_folder(cls, root):
-        from torchvision.datasets import ImageFolder
-        from torchvision.transforms import ToTensor
-
-        dataset = ImageFolder(root, transform=ToTensor())
-        return PyTorchNativeDataset(dataset)
-
-    @classmethod
-    def use_lfw(cls):
-        from sklearn.datasets import fetch_lfw_people
-
-        lfw = fetch_lfw_people()
-        features, labels = lfw.images, lfw.target
-
-        return ImageCategoricalDataset(features, labels)
-
 
 class DLDataset(Dataset, metaclass=ABCMeta):
 
     def get_data(self):
         features, targets = None, None
         loader = DataLoader(self, batch_size=128)
         for idx, (feature, target) in enumerate(loader):
@@ -89,14 +54,25 @@
     def __len__(self):
         return self.get_length()
 
     def __getitem__(self, idx):
         return self.index_of(idx)
 
 
+class EmptyDataset(DLDataset):
+    def __init__(self):
+        super().__init__()
+
+    def index_of(self, idx):
+        return None
+
+    def get_length(self):
+        return 0
+
+
 class PyTorchNativeDataset(DLDataset):
     def __init__(self, dataset):
         self.dataset = dataset
 
     def index_of(self, idx):
         return self.dataset[idx]
```

### Comparing `dltrain-0.0.4/src/dltrain/delineator.py` & `dltrain-0.1.0/src/dltrain/delineator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from abc import ABCMeta, abstractmethod
 
-from .dataset import DLDataset, PyTorchNativeDataset
+from .dataset import DLDataset, PyTorchNativeDataset, EmptyDataset
 from torch.utils.data import random_split
 
-
 __all__ = [
     'Delineator',
     'TrainEvalSetDelineator',
     'RandomSplitDelineator'
 ]
 
+
 class Delineator(metaclass=ABCMeta):
     @abstractmethod
     def get_train_set(self) -> DLDataset:
         pass
 
     @abstractmethod
     def get_eval_set(self) -> DLDataset:
         pass
 
 
 class TrainEvalSetDelineator(Delineator):
-    def __init__(self, train_set: DLDataset, eval_set: DLDataset):
+    def __init__(self, train_set: DLDataset, eval_set: DLDataset = None):
         self.train_set = train_set
-        self.eval_set = eval_set
+        self.eval_set = eval_set if eval_set is not None else EmptyDataset()
 
     def get_eval_set(self) -> DLDataset:
         return self.eval_set
 
     def get_train_set(self) -> DLDataset:
         return self.train_set
```

### Comparing `dltrain-0.0.4/src/dltrain/error.py` & `dltrain-0.1.0/src/dltrain/error.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.4/src/dltrain/models.py` & `dltrain-0.1.0/src/dltrain/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,15 @@
             modules.append(constructor())
             modules.append(Linear(hidden, targets))
         else:
             last_num = features
             for layer in layers:
                 modules.append(Linear(last_num, layer))
                 modules.append(constructor())
+                last_num = layer
             modules.append(Linear(last_num, targets))
 
         self.layers = Sequential(
             *modules
         )
 
     def forward(self, data):
```

### Comparing `dltrain-0.0.4/src/dltrain/options.py` & `dltrain-0.1.0/src/dltrain/options.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.4/src/dltrain/train.py` & `dltrain-0.1.0/src/dltrain/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,16 @@
         logger = LoggerContext()
         logger.info('Starting training')
 
         set_plt()
 
         checkpoint: CheckPoint = None
         if options.start_checkpoint is not None:
-            checkpoint = torch.load(options.start_checkpoint)
+            checkpoint = torch.load(options.start_checkpoint) if (
+                isinstance(options.start_checkpoint, str)) else options.start_checkpoint
             options = checkpoint.options
 
             logger.info(f'Loading checkpoint at {options.start_checkpoint}')
 
         if checkpoint is None:
             makedirs(options.task_name, exist_ok=True)
             makedirs(os.path.join(options.task_name, 'weights'), exist_ok=True)
@@ -121,15 +122,15 @@
                     if targets_transform is not None:
                         y = targets_transform(y)
 
                     loss = forward(model=model,
                                    criterion=criterion,
                                    x=x, y=y, eval=False,
                                    evaluation=train_evaluation,
-                                   optimizer=optimizer)
+                                   optimizer=optimizer, epoch=epoch, idx=idx)
 
                     pbar.set_postfix(loss=float(loss))
                     pbar.update(1)
 
                 pbar.set_postfix(loss=float(loss))
 
             if scheduler is not None:
@@ -145,15 +146,15 @@
                         x = features_transform(x)
 
                     if targets_transform is not None:
                         y = targets_transform(y)
 
                     loss = forward(model=model,
                                    criterion=criterion,
-                                   x=x, y=y, eval=True,
+                                   x=x, y=y, eval=True, epoch=epoch, idx=idx,
                                    evaluation=eval_evaluation)
 
                 # 计算训练集与测试集Loss
                 train_loss = criterion(train_evaluation.predictions, train_evaluation.exacts)
                 eval_loss = criterion(eval_evaluation.predictions, eval_evaluation.exacts)
                 total_train_loss.append(float(train_loss))
                 total_eval_loss.append(float(eval_loss))
@@ -281,7 +282,8 @@
                     **total_eval_evaluation
                 }
             )
             eval_evaluation_frame.index.name = 'Epoch'
             eval_evaluation_frame.to_csv(f'{options.task_name}/eval_evaluation_result.csv', encoding='utf-8')
 
         logger.save(f'{options.task_name}/log.txt')
+
```

### Comparing `dltrain-0.0.4/src/dltrain/transform.py` & `dltrain-0.1.0/src/dltrain/transform.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.4/src/dltrain/utils.py` & `dltrain-0.1.0/src/dltrain/utils.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.4/src/dltrain.egg-info/PKG-INFO` & `dltrain-0.1.0/src/dltrain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dltrain
-Version: 0.0.4
+Version: 0.1.0
 Summary: This is a package for PyTorch training, and this project provides a large number of high-level training APIs and low-level interfaces to meet all training needs
 Author-email: XiaosYu <lijingyu_ai@163.com>
 Project-URL: Homepage, https://github.com/XiaosYu/dltrain
 Project-URL: Bug Tracker, https://github.com/XiaosYu/dltrain/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dltrain-0.0.4/src/dltrain.egg-info/SOURCES.txt` & `dltrain-0.1.0/src/dltrain.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,26 +4,31 @@
 src/dltrain/__init__.py
 src/dltrain/checkpoint.py
 src/dltrain/dataset.py
 src/dltrain/delineator.py
 src/dltrain/error.py
 src/dltrain/evaluation.py
 src/dltrain/forward.py
+src/dltrain/inject.py
 src/dltrain/models.py
 src/dltrain/options.py
 src/dltrain/train.py
 src/dltrain/transform.py
 src/dltrain/utils.py
 src/dltrain.egg-info/PKG-INFO
 src/dltrain.egg-info/SOURCES.txt
 src/dltrain.egg-info/dependency_links.txt
 src/dltrain.egg-info/top_level.txt
 src/dltrain/builder/__init__.py
 src/dltrain/builder/base.py
 src/dltrain/builder/builder.py
 src/dltrain/builder/core.py
 src/dltrain/builder/criterion.py
-src/dltrain/builder/evaluation_handler.py
+src/dltrain/builder/dataset.py
+src/dltrain/builder/delineator.py
+src/dltrain/builder/evaluation.py
+src/dltrain/builder/forward.py
+src/dltrain/builder/inject.py
 src/dltrain/builder/model.py
 src/dltrain/builder/optimizer.py
 src/dltrain/builder/scheduler.py
 src/dltrain/builder/transforms.py
```

