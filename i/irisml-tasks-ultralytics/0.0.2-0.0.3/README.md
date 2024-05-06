# Comparing `tmp/irisml_tasks_ultralytics-0.0.2.tar.gz` & `tmp/irisml_tasks_ultralytics-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irisml_tasks_ultralytics-0.0.2.tar", last modified: Mon Apr 22 21:06:17 2024, max compression
+gzip compressed data, was "irisml_tasks_ultralytics-0.0.3.tar", last modified: Mon May  6 23:41:05 2024, max compression
```

## Comparing `irisml_tasks_ultralytics-0.0.2.tar` & `irisml_tasks_ultralytics-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:06:17.991545 irisml_tasks_ultralytics-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-22 21:03:50.000000 irisml_tasks_ultralytics-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-22 21:06:17.987545 irisml_tasks_ultralytics-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-22 21:03:50.000000 irisml_tasks_ultralytics-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:06:17.983545 irisml_tasks_ultralytics-0.0.2/irisml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:06:17.987545 irisml_tasks_ultralytics-0.0.2/irisml/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-22 21:03:50.000000 irisml_tasks_ultralytics-0.0.2/irisml/tasks/create_ultralytics_train_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-22 21:03:50.000000 irisml_tasks_ultralytics-0.0.2/irisml/tasks/create_ultralytics_yolov9_detection_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:06:17.987545 irisml_tasks_ultralytics-0.0.2/irisml_tasks_ultralytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-22 21:06:17.000000 irisml_tasks_ultralytics-0.0.2/irisml_tasks_ultralytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-22 21:06:17.000000 irisml_tasks_ultralytics-0.0.2/irisml_tasks_ultralytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 21:06:17.000000 irisml_tasks_ultralytics-0.0.2/irisml_tasks_ultralytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-22 21:06:17.000000 irisml_tasks_ultralytics-0.0.2/irisml_tasks_ultralytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-22 21:06:17.000000 irisml_tasks_ultralytics-0.0.2/irisml_tasks_ultralytics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-22 21:03:50.000000 irisml_tasks_ultralytics-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 21:06:17.991545 irisml_tasks_ultralytics-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:06:17.987545 irisml_tasks_ultralytics-0.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-22 21:03:50.000000 irisml_tasks_ultralytics-0.0.2/test/test_create_ultralytics_train_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-22 21:03:50.000000 irisml_tasks_ultralytics-0.0.2/test/test_create_ultralytics_yolov9_detection_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:41:05.613108 irisml_tasks_ultralytics-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-06 23:38:36.000000 irisml_tasks_ultralytics-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-06 23:41:05.613108 irisml_tasks_ultralytics-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-06 23:38:36.000000 irisml_tasks_ultralytics-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:41:05.609107 irisml_tasks_ultralytics-0.0.3/irisml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:41:05.609107 irisml_tasks_ultralytics-0.0.3/irisml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-06 23:38:36.000000 irisml_tasks_ultralytics-0.0.3/irisml/tasks/create_ultralytics_train_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-06 23:38:36.000000 irisml_tasks_ultralytics-0.0.3/irisml/tasks/create_ultralytics_val_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-05-06 23:38:36.000000 irisml_tasks_ultralytics-0.0.3/irisml/tasks/create_ultralytics_yolov9_detection_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:41:05.613108 irisml_tasks_ultralytics-0.0.3/irisml_tasks_ultralytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-06 23:41:05.000000 irisml_tasks_ultralytics-0.0.3/irisml_tasks_ultralytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-06 23:41:05.000000 irisml_tasks_ultralytics-0.0.3/irisml_tasks_ultralytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 23:41:05.000000 irisml_tasks_ultralytics-0.0.3/irisml_tasks_ultralytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-06 23:41:05.000000 irisml_tasks_ultralytics-0.0.3/irisml_tasks_ultralytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 23:41:05.000000 irisml_tasks_ultralytics-0.0.3/irisml_tasks_ultralytics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-06 23:38:36.000000 irisml_tasks_ultralytics-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 23:41:05.613108 irisml_tasks_ultralytics-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:41:05.613108 irisml_tasks_ultralytics-0.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-06 23:38:36.000000 irisml_tasks_ultralytics-0.0.3/test/test_create_ultralytics_train_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-06 23:38:36.000000 irisml_tasks_ultralytics-0.0.3/test/test_create_ultralytics_val_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-06 23:38:36.000000 irisml_tasks_ultralytics-0.0.3/test/test_create_ultralytics_yolov9_detection_model.py
```

### Comparing `irisml_tasks_ultralytics-0.0.2/LICENSE` & `irisml_tasks_ultralytics-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `irisml_tasks_ultralytics-0.0.2/PKG-INFO` & `irisml_tasks_ultralytics-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-ultralytics
-Version: 0.0.2
+Version: 0.0.3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: irisml
 Requires-Dist: ultralytics-nogui<9
 
 # irisml-tasks-ultralytics
```

### Comparing `irisml_tasks_ultralytics-0.0.2/README.md` & `irisml_tasks_ultralytics-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `irisml_tasks_ultralytics-0.0.2/irisml/tasks/create_ultralytics_train_transform.py` & `irisml_tasks_ultralytics-0.0.3/irisml/tasks/create_ultralytics_train_transform.py`

 * *Files identical despite different names*

### Comparing `irisml_tasks_ultralytics-0.0.2/irisml/tasks/create_ultralytics_yolov9_detection_model.py` & `irisml_tasks_ultralytics-0.0.3/irisml/tasks/create_ultralytics_yolov9_detection_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,40 +10,44 @@
 
 logger = logging.getLogger(__name__)
 
 
 class Task(irisml.core.TaskBase):
     """Create a Yolo Detection model using Ultralytics library.
     """
-    VERSION = '0.1.0'
+    VERSION = '0.2.0'
 
     @dataclasses.dataclass
     class Config:
         model_name: typing.Literal['yolov9c', 'yolov9e']
         num_classes: int
+        nms_conf_threshold: float = 0.001
+        nms_iou_threshold: float = 0.7
 
     @dataclasses.dataclass
     class Outputs:
         model: torch.nn.Module
 
     def execute(self, inputs):
         logger.info(f"Creating YOLOv9 detection model. name={self.config.model_name}, num_classes={self.config.num_classes}")
         yolo_model = DetectionModel(self.config.model_name + '.yaml', nc=self.config.num_classes)
         yolo_model.nc = self.config.num_classes
         yolo_model.names = {i: f'class_{i}' for i in range(self.config.num_classes)}
         yolo_cfg = IterableSimpleNamespace(**DEFAULT_CFG_DICT)
         yolo_cfg.nc = self.config.num_classes
         yolo_model.args = yolo_cfg
-        return self.Outputs(model=YoloV9DetectionModel(yolo_model))
+        return self.Outputs(model=YoloV9DetectionModel(yolo_model, nms_conf_threshold=self.config.nms_conf_threshold, nms_iou_threshold=self.config.nms_iou_threshold))
 
 
 class YoloV9DetectionModel(torch.nn.Module):
-    def __init__(self, yolo_model):
+    def __init__(self, yolo_model, nms_conf_threshold, nms_iou_threshold):
         super().__init__()
         self._model = yolo_model
+        self._nms_conf_threshold = nms_conf_threshold
+        self._nms_iou_threshold = nms_iou_threshold
 
     def predict(self, image):
         return self.model(image)
 
     def training_step(self, inputs, targets):
         batch_index = torch.cat([torch.full((len(t), 1), i, device=inputs.device) for i, t in enumerate(targets)], dim=0,)
         cls = torch.cat([t[:, 0] for t in targets], dim=0)
@@ -69,15 +73,15 @@
     def prediction_step(self, inputs):
         assert isinstance(inputs, torch.Tensor) and inputs.dim() == 4  # (N, C, H, W)
 
         if self.training:
             raise RuntimeError("Model is in training mode. Call eval() before prediction_step.")
 
         results = self._model.predict(inputs)
-        yolo_predictions = ultralytics.utils.ops.non_max_suppression(results, conf_thres=0.25, iou_thres=0.7, agnostic=False, max_det=300)
+        yolo_predictions = ultralytics.utils.ops.non_max_suppression(results, conf_thres=self._nms_conf_threshold, iou_thres=self._nms_iou_threshold, agnostic=False, max_det=300)
         predictions = []
         for pred in yolo_predictions:
             assert isinstance(pred, torch.Tensor) and pred.shape[1] == 6  # (x1, y1, x2, y2, conf, cls)
             new_pred = torch.cat([pred[:, 5:6], pred[:, 4:5], pred[:, :4]], dim=1)
             new_pred[:,2] /= inputs.shape[3]
             new_pred[:,3] /= inputs.shape[2]
             new_pred[:,4] /= inputs.shape[3]
```

### Comparing `irisml_tasks_ultralytics-0.0.2/irisml_tasks_ultralytics.egg-info/PKG-INFO` & `irisml_tasks_ultralytics-0.0.3/irisml_tasks_ultralytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-ultralytics
-Version: 0.0.2
+Version: 0.0.3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: irisml
 Requires-Dist: ultralytics-nogui<9
 
 # irisml-tasks-ultralytics
```

### Comparing `irisml_tasks_ultralytics-0.0.2/test/test_create_ultralytics_train_transform.py` & `irisml_tasks_ultralytics-0.0.3/test/test_create_ultralytics_train_transform.py`

 * *Files identical despite different names*

### Comparing `irisml_tasks_ultralytics-0.0.2/test/test_create_ultralytics_yolov9_detection_model.py` & `irisml_tasks_ultralytics-0.0.3/test/test_create_ultralytics_yolov9_detection_model.py`

 * *Files identical despite different names*

