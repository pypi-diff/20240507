# Comparing `tmp/segments-ai-1.7.6.tar.gz` & `tmp/segments-ai-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segments-ai-1.7.6.tar", last modified: Mon Apr 22 10:26:25 2024, max compression
+gzip compressed data, was "segments-ai-1.8.0.tar", last modified: Tue May  7 08:56:51 2024, max compression
```

## Comparing `segments-ai-1.7.6.tar` & `segments-ai-1.8.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-04-22 10:26:25.321447 segments-ai-1.7.6/
--rw-r--r--   0 bert      (1000) bert      (1000)     1062 2020-01-04 18:38:00.000000 segments-ai-1.7.6/LICENSE.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)       83 2023-09-06 09:45:12.000000 segments-ai-1.7.6/MANIFEST.in
--rw-rw-r--   0 bert      (1000) bert      (1000)     1179 2024-04-22 10:26:25.321447 segments-ai-1.7.6/PKG-INFO
--rw-rw-r--   0 bert      (1000) bert      (1000)     2955 2023-11-23 15:51:52.000000 segments-ai-1.7.6/README.md
--rw-rw-r--   0 bert      (1000) bert      (1000)      714 2023-11-23 10:20:03.000000 segments-ai-1.7.6/pyproject.toml
--rw-rw-r--   0 bert      (1000) bert      (1000)      194 2024-02-01 10:25:04.000000 segments-ai-1.7.6/requirements.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)      197 2023-11-23 10:20:03.000000 segments-ai-1.7.6/requirements_dev.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)      171 2023-09-21 17:58:29.000000 segments-ai-1.7.6/requirements_docs.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)      233 2024-04-22 10:26:25.321447 segments-ai-1.7.6/setup.cfg
--rw-rw-r--   0 bert      (1000) bert      (1000)     3287 2024-04-22 10:25:16.000000 segments-ai-1.7.6/setup.py
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-04-22 10:26:25.317447 segments-ai-1.7.6/src/
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-04-22 10:26:25.317447 segments-ai-1.7.6/src/segments/
--rw-rw-r--   0 bert      (1000) bert      (1000)      138 2023-11-23 10:20:03.000000 segments-ai-1.7.6/src/segments/__init__.py
--rw-rw-r--   0 bert      (1000) bert      (1000)    87565 2024-03-15 11:08:21.000000 segments-ai-1.7.6/src/segments/client.py
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-04-22 10:26:25.317447 segments-ai-1.7.6/src/segments/data/
--rw-rw-r--   0 bert      (1000) bert      (1000)      501 2022-08-02 10:22:42.000000 segments-ai-1.7.6/src/segments/data/dataset_card_template.md
--rw-rw-r--   0 bert      (1000) bert      (1000)    14548 2024-03-05 14:46:29.000000 segments-ai-1.7.6/src/segments/dataset.py
--rw-rw-r--   0 bert      (1000) bert      (1000)     2191 2023-10-10 09:44:13.000000 segments-ai-1.7.6/src/segments/exceptions.py
--rw-rw-r--   0 bert      (1000) bert      (1000)    30413 2023-11-23 10:20:03.000000 segments-ai-1.7.6/src/segments/export.py
--rw-rw-r--   0 bert      (1000) bert      (1000)    11870 2023-11-23 10:20:03.000000 segments-ai-1.7.6/src/segments/huggingface.py
--rw-rw-r--   0 bert      (1000) bert      (1000)        0 2022-08-02 10:22:42.000000 segments-ai-1.7.6/src/segments/py.typed
--rw-rw-r--   0 bert      (1000) bert      (1000)    23017 2024-04-22 10:25:00.000000 segments-ai-1.7.6/src/segments/typing.py
--rw-rw-r--   0 bert      (1000) bert      (1000)    35687 2024-04-07 13:40:19.000000 segments-ai-1.7.6/src/segments/utils.py
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-04-22 10:26:25.321447 segments-ai-1.7.6/src/segments_ai.egg-info/
--rw-r--r--   0 bert      (1000) bert      (1000)     1179 2024-04-22 10:26:24.000000 segments-ai-1.7.6/src/segments_ai.egg-info/PKG-INFO
--rw-rw-r--   0 bert      (1000) bert      (1000)      691 2024-04-22 10:26:25.000000 segments-ai-1.7.6/src/segments_ai.egg-info/SOURCES.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)        1 2024-04-22 10:26:24.000000 segments-ai-1.7.6/src/segments_ai.egg-info/dependency_links.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)      446 2024-04-22 10:26:25.000000 segments-ai-1.7.6/src/segments_ai.egg-info/requires.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)        9 2024-04-22 10:26:25.000000 segments-ai-1.7.6/src/segments_ai.egg-info/top_level.txt
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-04-22 10:26:25.321447 segments-ai-1.7.6/tests/
--rw-rw-r--   0 bert      (1000) bert      (1000)    38723 2023-11-23 15:51:56.000000 segments-ai-1.7.6/tests/test_client.py
--rw-rw-r--   0 bert      (1000) bert      (1000)     1270 2023-11-23 10:20:03.000000 segments-ai-1.7.6/tests/test_dataset.py
--rw-rw-r--   0 bert      (1000) bert      (1000)        0 2022-08-02 10:22:42.000000 segments-ai-1.7.6/tests/test_huggingface.py
--rw-rw-r--   0 bert      (1000) bert      (1000)      226 2022-08-02 10:22:42.000000 segments-ai-1.7.6/tests/test_random.py
--rw-rw-r--   0 bert      (1000) bert      (1000)     1052 2023-07-21 08:16:50.000000 segments-ai-1.7.6/tests/test_utils.py
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-05-07 08:56:51.379060 segments-ai-1.8.0/
+-rw-r--r--   0 bert      (1000) bert      (1000)     1062 2020-01-04 18:38:00.000000 segments-ai-1.8.0/LICENSE.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)       83 2023-09-06 09:45:12.000000 segments-ai-1.8.0/MANIFEST.in
+-rw-rw-r--   0 bert      (1000) bert      (1000)     1179 2024-05-07 08:56:51.379060 segments-ai-1.8.0/PKG-INFO
+-rw-rw-r--   0 bert      (1000) bert      (1000)     2955 2023-11-23 15:51:52.000000 segments-ai-1.8.0/README.md
+-rw-rw-r--   0 bert      (1000) bert      (1000)      714 2023-11-23 10:20:03.000000 segments-ai-1.8.0/pyproject.toml
+-rw-rw-r--   0 bert      (1000) bert      (1000)      194 2024-02-01 10:25:04.000000 segments-ai-1.8.0/requirements.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)      197 2023-11-23 10:20:03.000000 segments-ai-1.8.0/requirements_dev.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)      171 2023-09-21 17:58:29.000000 segments-ai-1.8.0/requirements_docs.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)      233 2024-05-07 08:56:51.379060 segments-ai-1.8.0/setup.cfg
+-rw-rw-r--   0 bert      (1000) bert      (1000)     3287 2024-05-07 08:55:36.000000 segments-ai-1.8.0/setup.py
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-05-07 08:56:51.371060 segments-ai-1.8.0/src/
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-05-07 08:56:51.375060 segments-ai-1.8.0/src/segments/
+-rw-rw-r--   0 bert      (1000) bert      (1000)      138 2023-11-23 10:20:03.000000 segments-ai-1.8.0/src/segments/__init__.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)    87827 2024-05-07 08:55:20.000000 segments-ai-1.8.0/src/segments/client.py
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-05-07 08:56:51.375060 segments-ai-1.8.0/src/segments/data/
+-rw-rw-r--   0 bert      (1000) bert      (1000)      501 2022-08-02 10:22:42.000000 segments-ai-1.8.0/src/segments/data/dataset_card_template.md
+-rw-rw-r--   0 bert      (1000) bert      (1000)    14575 2024-05-07 08:55:20.000000 segments-ai-1.8.0/src/segments/dataset.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)     2191 2023-10-10 09:44:13.000000 segments-ai-1.8.0/src/segments/exceptions.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)    30466 2024-05-07 08:55:20.000000 segments-ai-1.8.0/src/segments/export.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)    11870 2023-11-23 10:20:03.000000 segments-ai-1.8.0/src/segments/huggingface.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)        0 2022-08-02 10:22:42.000000 segments-ai-1.8.0/src/segments/py.typed
+-rw-rw-r--   0 bert      (1000) bert      (1000)    23071 2024-05-07 08:55:20.000000 segments-ai-1.8.0/src/segments/typing.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)    38454 2024-05-07 08:55:20.000000 segments-ai-1.8.0/src/segments/utils.py
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-05-07 08:56:51.375060 segments-ai-1.8.0/src/segments_ai.egg-info/
+-rw-r--r--   0 bert      (1000) bert      (1000)     1179 2024-05-07 08:56:51.000000 segments-ai-1.8.0/src/segments_ai.egg-info/PKG-INFO
+-rw-rw-r--   0 bert      (1000) bert      (1000)      691 2024-05-07 08:56:51.000000 segments-ai-1.8.0/src/segments_ai.egg-info/SOURCES.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)        1 2024-05-07 08:56:51.000000 segments-ai-1.8.0/src/segments_ai.egg-info/dependency_links.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)      446 2024-05-07 08:56:51.000000 segments-ai-1.8.0/src/segments_ai.egg-info/requires.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)        9 2024-05-07 08:56:51.000000 segments-ai-1.8.0/src/segments_ai.egg-info/top_level.txt
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-05-07 08:56:51.379060 segments-ai-1.8.0/tests/
+-rw-rw-r--   0 bert      (1000) bert      (1000)    38723 2023-11-23 15:51:56.000000 segments-ai-1.8.0/tests/test_client.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)     1270 2023-11-23 10:20:03.000000 segments-ai-1.8.0/tests/test_dataset.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)        0 2022-08-02 10:22:42.000000 segments-ai-1.8.0/tests/test_huggingface.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)      226 2022-08-02 10:22:42.000000 segments-ai-1.8.0/tests/test_random.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)     1052 2023-07-21 08:16:50.000000 segments-ai-1.8.0/tests/test_utils.py
```

### Comparing `segments-ai-1.7.6/LICENSE.txt` & `segments-ai-1.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.6/PKG-INFO` & `segments-ai-1.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: segments-ai
-Version: 1.7.6
+Version: 1.8.0
 Summary: UNKNOWN
 Home-page: https://github.com/segments-ai/segments-ai
-Download-URL: https://github.com/segments-ai/segments-ai/archive/v1.7.6.tar.gz
+Download-URL: https://github.com/segments-ai/segments-ai/archive/v1.8.0.tar.gz
 Author: Segments.ai
 Author-email: bert@segments.ai
 License: MIT
 Keywords: image,segmentation,labeling,vision
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `segments-ai-1.7.6/README.md` & `segments-ai-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.6/pyproject.toml` & `segments-ai-1.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.6/setup.py` & `segments-ai-1.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from typing import List
 
 
 #############
 # Constants #
 #############
-MAJOR, MINOR, PATCH = 1, 7, 6
+MAJOR, MINOR, PATCH = 1, 8, 0
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 
 ####################
 # Helper functions #
 ####################
 # https://github.com/allenai/python-package-template
```

### Comparing `segments-ai-1.7.6/src/segments/client.py` & `segments-ai-1.8.0/src/segments/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,14 +116,19 @@
         except requests.exceptions.Timeout as e:
             # Maybe set up for a retry, or continue in a retry loop
             raise TimeoutError(message=str(e), cause=e)
         except requests.exceptions.HTTPError as e:
             # Make string comparison case insensitive.
             text = e.response.text.lower()
             if "not found" in text or "does not exist" in text:
+                text += """\n
+Possible fixes:
+- Check for typos in the dataset name, sample name, labelset name, etc.
+- Are you using the argument `dataset_name` -> Did you add the organization to the dataset name? E.g., `jane/flowers` instead of `flowers`.
+"""
                 raise NotFoundError(message=text, cause=e)
             if "already exists" in text or "already have" in text:
                 raise AlreadyExistsError(message=text, cause=e)
             if "cannot be added as collaborator" in text or "is already a collaborator" in text:
                 raise CollaboratorError(message=text, cause=e)
             if "authentication credentials were not provided" in text:
                 raise AuthenticationError(message=text, cause=e)
```

### Comparing `segments-ai-1.7.6/src/segments/dataset.py` & `segments-ai-1.8.0/src/segments/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import numpy as np
 import numpy.typing as npt
 import requests
 from PIL import Image, UnidentifiedImageError
 from pydantic import TypeAdapter
 from segments.typing import LabelStatus, Release, SegmentsDatasetCategory
 from segments.utils import (
+    SEGMENTS_ORANGE,
     handle_exif_rotation,
     load_image_from_url,
     load_label_bitmap_from_url,
 )
 from tqdm import tqdm
 
 
@@ -204,15 +205,15 @@
             print("Preloading all samples. This may take a while...")
             with ThreadPool(16) as pool:
                 # list(tqdm(pool.imap_unordered(self.__getitem__, range(num_samples)), total=num_samples))
                 list(
                     tqdm(
                         pool.imap_unordered(_load_image, range(num_samples)),
                         total=num_samples,
-                        colour="#FF9900",
+                        colour=SEGMENTS_ORANGE,
                     )
                 )
 
         print(f"Initialized dataset with {num_samples} images.")
 
     def _load_image_from_cache(self, sample: Dict[str, Any]) -> Tuple[Optional[Image.Image], str]:
         sample_name = os.path.splitext(sample["name"])[0]
```

### Comparing `segments-ai-1.7.6/src/segments/exceptions.py` & `segments-ai-1.8.0/src/segments/exceptions.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.6/src/segments/export.py` & `segments-ai-1.8.0/src/segments/export.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Set, Tuple, Union, cast
 
 import numpy as np
 import numpy.typing as npt
 from PIL import Image
 from segments.typing import SegmentsDatasetCategory
-from segments.utils import get_semantic_bitmap
+from segments.utils import SEGMENTS_ORANGE, get_semantic_bitmap
 from skimage import img_as_ubyte
 from skimage.measure import regionprops
 from tqdm import tqdm
 
 
 # https://adamj.eu/tech/2021/05/13/python-type-hints-how-to-fix-circular-imports/
 if TYPE_CHECKING:
@@ -243,15 +243,15 @@
     #         'name': category
     #     })
 
     images = []
     annotations = []
 
     annotation_id = 1
-    for i in tqdm(range(len(dataset)), total=len(dataset), colour="#FF9900"):
+    for i in tqdm(range(len(dataset)), total=len(dataset), colour=SEGMENTS_ORANGE):
         sample = dataset[i]
 
         if sample["annotations"] is None:
             continue
 
         image_id = i + 1
         images.append(
@@ -415,15 +415,15 @@
 
     categories_dict: Dict[int, SegmentsDatasetCategory] = {category.id: category for category in categories}
     id_generator = IdGenerator(categories_dict)
 
     # IMAGES AND ANNOTATIONS
     images = []
     annotations = []
-    for i in tqdm(range(len(dataset)), total=len(dataset), colour="#FF9900"):
+    for i in tqdm(range(len(dataset)), total=len(dataset), colour=SEGMENTS_ORANGE):
         sample = dataset[i]
 
         if sample["annotations"] is None:
             continue
 
         # Images
         image_id = i + 1
@@ -583,15 +583,15 @@
                     "name": category.name,
                     "color": color,
                     "isthing": isthing,
                 }
             )
         )
 
-    for i in tqdm(range(len(dataset)), total=len(dataset), colour="#FF9900"):
+    for i in tqdm(range(len(dataset)), total=len(dataset), colour=SEGMENTS_ORANGE):
         sample = dataset[i]
 
         if sample["annotations"] is None:
             continue
 
         file_name = os.path.splitext(os.path.basename(sample["name"]))[0]
 
@@ -698,15 +698,15 @@
             "Only bounding box annotations will be processed. Polygon, polyline and keypoint annotations will be ignored."
         )
 
     if dataset.task_type == "image-vector-sequence":
         logger.warning(
             "Note that the sequences will be exported as individual frames, disregarding the tracking information."
         )
-        for i in tqdm(range(len(dataset)), total=len(dataset), colour="#FF9900"):
+        for i in tqdm(range(len(dataset)), total=len(dataset), colour=SEGMENTS_ORANGE):
             sample = dataset[i]
             image_name = os.path.splitext(os.path.basename(sample["name"]))[0]
 
             if image_width is None or image_height is None:
                 raise ValueError("Please provide image_width and image_height parameters (i.e., not None).")
 
             for j, frame in enumerate(sample["labels"]["ground-truth"]["attributes"]["frames"]):
@@ -719,15 +719,15 @@
 
                 # Testing on x is the same as testing len(x)>0 (this also checks that x is not None - see truthy and falsy values in Python)
                 # https://stackoverflow.com/questions/39983695/what-is-truthy-and-falsy-how-is-it-different-from-true-and-false
                 if "annotations" in frame and frame["annotations"]:
                     annotations = frame["annotations"]
                     write_yolo_file(file_name, annotations, image_width, image_height)
     else:
-        for i in tqdm(range(len(dataset)), total=len(dataset), colour="#FF9900"):
+        for i in tqdm(range(len(dataset)), total=len(dataset), colour=SEGMENTS_ORANGE):
             sample = dataset[i]
             image_name = os.path.splitext(os.path.basename(sample["name"]))[0]
             file_name = os.path.join(export_folder, dataset.image_dir, f"{image_name}.txt")
 
             if "annotations" in sample and sample["annotations"]:
                 annotations = sample["annotations"]
                 write_yolo_file(
@@ -772,15 +772,15 @@
     categories = dataset.categories
     # task_type = dataset.task_type
 
     images = []
     annotations = []
 
     annotation_id = 1
-    for i in tqdm(range(len(dataset)), total=len(dataset), colour="#FF9900"):
+    for i in tqdm(range(len(dataset)), total=len(dataset), colour=SEGMENTS_ORANGE):
         sample = dataset[i]
 
         if sample["annotations"] is None:
             continue
 
         image_id = i + 1
         images.append(
```

### Comparing `segments-ai-1.7.6/src/segments/huggingface.py` & `segments-ai-1.8.0/src/segments/huggingface.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.6/src/segments/typing.py` & `segments-ai-1.8.0/src/segments/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,15 @@
     PCD = "pcd"
     BINARY_XYZI = "binary-xyzi"
     KITTI = "kitti"
     BINARY_XYZIR = "binary-xyzir"
     NUSCENES = "nuscenes"
     PLY = "ply"
     LAS = "las"
+    SPLAT = "splat"
 
 
 class ReleaseStatus(str, Enum):
     PENDING = "PENDING"
     SUCCEEDED = "SUCCEEDED"
     FAILED = "FAILED"
 
@@ -336,15 +337,15 @@
     frames: List[ImageVectorFrame]
     format_version: Optional[FormatVersion] = None
 
 
 # Point cloud segmentation
 class PointcloudSegmentationLabelAttributes(BaseModel):
     annotations: List[Annotation]
-    point_annotations: List[int]
+    point_annotations: Optional[List[int]] = None
     format_version: Optional[FormatVersion] = None
 
 
 class XYZ(BaseModel):
     x: float
     y: float
     z: float
@@ -414,15 +415,15 @@
     track_id: int
     is_keyframe: bool = False
     attributes: Optional[ObjectAttributes] = None
 
 
 class PointcloudSegmentationFrame(PointcloudSegmentationLabelAttributes):
     annotations: List[PointcloudSequenceSegmentationAnnotation]
-    point_annotations: List[int]
+    point_annotations: Optional[List[int]] = None
     timestamp: Optional[Timestamp] = None
     format_version: Optional[FormatVersion] = None
 
 
 class PointcloudSequenceSegmentationLabelAttributes(BaseModel):
     frames: List[PointcloudSegmentationFrame]
     format_version: Optional[FormatVersion] = None
```

### Comparing `segments-ai-1.7.6/src/segments/utils.py` & `segments-ai-1.8.0/src/segments/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     XYZW,
     EgoPose,
     ExportFormat,
     PointcloudCuboidLabelAttributes,
     PointcloudSequenceSampleAttributes,
     TaskType,
 )
+from tqdm import tqdm
 
 
 # https://adamj.eu/tech/2021/05/13/python-type-hints-how-to-fix-circular-imports/
 # https://stackoverflow.com/questions/61384752/how-to-type-hint-with-an-optional-import
 if TYPE_CHECKING:
     import open3d as o3d
     from pyquaternion import Quaternion
@@ -41,14 +42,15 @@
 # Variables #
 #############
 session = requests.Session()
 adapter = requests.adapters.HTTPAdapter(max_retries=3)
 session.mount("http://", adapter)
 session.mount("https://", adapter)
 logger = logging.getLogger(__name__)
+SEGMENTS_ORANGE = "#FF9900"
 COMPATIBLE_TASK_TYPES = {
     ExportFormat.COCO_PANOPTIC: {
         TaskType.SEGMENTATION_BITMAP,
         TaskType.SEGMENTATION_BITMAP_HIGHRES,
     },
     ExportFormat.COCO_INSTANCE: {
         TaskType.VECTOR,
@@ -796,15 +798,93 @@
             rgb = np.stack(
                 (ply["vertex"]["red"], ply["vertex"]["green"], ply["vertex"]["blue"]),
                 axis=-1,
             )
         except KeyError:
             rgb = None
 
-    pcd_path = ply_file.replace(".ply", ".pcd")
+    pcd_extension = "_compressed.pcd" if compressed else ".pcd"
+    pcd_path = ply_file.replace(".ply", pcd_extension)
+    # prefer RGB over intensity (tiled point cloud does not support both)
+    intensity = intensity if rgb is None else None
+    array_to_pcd(
+        positions,
+        pcd_path,
+        intensity=intensity,
+        rgb=rgb,
+        compressed=compressed,
+        write_ascii=write_ascii,
+    )
+
+
+def las_to_pcd(las_file: str, compressed: bool = False, write_ascii: bool = True) -> None:
+    """Convert a .las/.laz file to a .pcd file.
+
+    Args:
+        las_file: The path to the .las/.laz file.
+        compressed: If the pcd should be compressed. Defaults to :obj:`False`.
+        write_ascii: If the pcd should be written in ascii format. Defaults to :obj:`True`.
+
+    Returns:
+        None
+
+    Raises:
+        :exc:`ImportError`: If pdal is not installed (to install run ``pip install pdal``).
+    """
+    try:
+        from pdal import Pipeline
+    except ImportError:
+        logger.error("Please install `pdal` first: `pip install pdal`")
+
+    pipeline = json.dumps({"pipeline": [{"type": "readers.las", "filename": las_file}]})
+
+    pipeline = Pipeline(pipeline)
+    pipeline.execute()
+    raw_array = pipeline.arrays[0]
+    column_names = raw_array.dtype.names
+
+    array = []
+    for row in tqdm(raw_array, total=len(raw_array), color=SEGMENTS_ORANGE):
+        array.append(np.array(list(row)))
+    array = np.reshape(array, (-1, len(column_names)))
+
+    def find_las_column_index(column_name: Union[str, List[str]]) -> Union[int, Tuple[int]]:
+        def find_single_las_column_index(column_name: str) -> int:
+            index = column_names.index(column_name)
+
+            if index == -1:
+                return ValueError(f"Can't find column index of column with name {column_name}")
+
+            return index
+
+        if isinstance(column_name, list):
+            return tuple(find_single_las_column_index(column) for column in column_name)
+
+        return find_single_las_column_index(column_name)
+
+    def get_data(column_index: Union[int, List[int]]) -> np.ndarray:
+        if isinstance(column_index, list):
+            return np.stack((array[:, index] for index in column_index), axis=-1)
+
+        return array[:, column_index]
+
+    x, y, z = find_las_column_index(["X", "Y", "Z"])
+    intensity = find_las_column_index("Intensity")
+    r, g, b = find_las_column_index(["Red", "Green", "Blue"])
+
+    positions = get_data([x, y, z])
+    intensity = get_data(intensity)
+    rgb = get_data([r, g, b])
+
+    pcd_extension = "_compressed.pcd" if compressed else ".pcd"
+    pcd_path = (
+        las_file.replace(".las", pcd_extension)
+        if las_file.endswith(".las")
+        else las_file.replace(".laz", pcd_extension)
+    )
     # prefer RGB over intensity (tiled point cloud does not support both)
     intensity = intensity if rgb is None else None
     array_to_pcd(
         positions,
         pcd_path,
         intensity=intensity,
         rgb=rgb,
```

### Comparing `segments-ai-1.7.6/src/segments_ai.egg-info/PKG-INFO` & `segments-ai-1.8.0/src/segments_ai.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: segments-ai
-Version: 1.7.6
+Version: 1.8.0
 Summary: UNKNOWN
 Home-page: https://github.com/segments-ai/segments-ai
-Download-URL: https://github.com/segments-ai/segments-ai/archive/v1.7.6.tar.gz
+Download-URL: https://github.com/segments-ai/segments-ai/archive/v1.8.0.tar.gz
 Author: Segments.ai
 Author-email: bert@segments.ai
 License: MIT
 Keywords: image,segmentation,labeling,vision
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `segments-ai-1.7.6/src/segments_ai.egg-info/SOURCES.txt` & `segments-ai-1.8.0/src/segments_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.6/tests/test_client.py` & `segments-ai-1.8.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.6/tests/test_dataset.py` & `segments-ai-1.8.0/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.6/tests/test_utils.py` & `segments-ai-1.8.0/tests/test_utils.py`

 * *Files identical despite different names*

