# Comparing `tmp/orthographic_projector-0.1.0.tar.gz` & `tmp/orthographic_projector-0.1.1.tar.gz`

## Comparing `orthographic_projector-0.1.0.tar` & `orthographic_projector-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 orthographic_projector-0.1.0/Cargo.toml
--rw-r--r--   0     1000     1000       37 2024-05-06 23:10:43.000000 orthographic_projector-0.1.0/.gitignore
--rw-r--r--   0     1000     1000    18092 2024-04-28 13:42:19.000000 orthographic_projector-0.1.0/LICENSE
--rw-r--r--   0     1000     1000     1117 2024-05-06 23:10:43.000000 orthographic_projector-0.1.0/README.md
--rw-r--r--   0     1000     1000      755 2024-05-06 23:10:43.000000 orthographic_projector-0.1.0/examples/example_generate_projections.py
--rw-r--r--   0     1000     1000     1618 2024-05-06 23:10:43.000000 orthographic_projector-0.1.0/orthographic_projector/__init__.py
--rw-r--r--   0     1000     1000       43 2024-05-06 23:11:31.000000 orthographic_projector-0.1.0/requirements.txt
--rw-r--r--   0     1000     1000     4247 2024-05-06 23:10:43.000000 orthographic_projector-0.1.0/src/lib.rs
--rw-r--r--   0     1000     1000     8811 2024-05-06 12:19:43.000000 orthographic_projector-0.1.0/Cargo.lock
--rw-r--r--   0     1000     1000      526 2024-05-06 23:10:52.000000 orthographic_projector-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1534 1970-01-01 00:00:00.000000 orthographic_projector-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 orthographic_projector-0.1.1/Cargo.toml
+-rw-r--r--   0     1000     1000       47 2024-05-06 23:23:15.000000 orthographic_projector-0.1.1/.gitignore
+-rw-r--r--   0     1000     1000    18092 2024-04-28 13:42:19.000000 orthographic_projector-0.1.1/LICENSE
+-rw-r--r--   0     1000     1000     1117 2024-05-06 23:10:43.000000 orthographic_projector-0.1.1/README.md
+-rw-r--r--   0     1000     1000      879 2024-05-07 16:28:28.000000 orthographic_projector-0.1.1/examples/example_generate_projections.py
+-rw-r--r--   0     1000     1000     1828 2024-05-07 16:30:17.000000 orthographic_projector-0.1.1/orthographic_projector/__init__.py
+-rw-r--r--   0     1000     1000       43 2024-05-06 23:11:31.000000 orthographic_projector-0.1.1/requirements.txt
+-rw-r--r--   0     1000     1000     4247 2024-05-06 23:10:43.000000 orthographic_projector-0.1.1/src/lib.rs
+-rw-r--r--   0     1000     1000     8811 2024-05-07 16:15:04.000000 orthographic_projector-0.1.1/Cargo.lock
+-rw-r--r--   0     1000     1000      526 2024-05-06 23:38:04.000000 orthographic_projector-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1534 1970-01-01 00:00:00.000000 orthographic_projector-0.1.1/PKG-INFO
```

### Comparing `orthographic_projector-0.1.0/LICENSE` & `orthographic_projector-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `orthographic_projector-0.1.0/README.md` & `orthographic_projector-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `orthographic_projector-0.1.0/orthographic_projector/__init__.py` & `orthographic_projector-0.1.1/orthographic_projector/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 import cv2
 import numpy as np
 from .orthographic_projector import generate_projections as _internal_generate_projections
 
 
-def __preprocess_cloud(points, colors, precision):
+def __preprocess_point_cloud(points, colors, precision):
+    if type(points) != np.ndarray:
+        points = np.array(points)
+    if type(colors) != np.ndarray:
+        colors = np.array(colors)
+    if points.shape != colors.shape:
+        raise Exception('Points and colors must have the same shape.')
     min_bound = points.min(axis=0)
     max_bound = points.max(axis=0)
     if np.any(min_bound < 0):
         points -= min_bound
     if np.any(max_bound < 1) or (points.max() <= 1):
         points = (1 << precision) * (points - points.min()) / (points.max() - points.min())
     if colors.max() <= 1 and colors.min() >= 0:
         colors = (colors * 255).astype(np.uint8)
     return points, colors
 
 
-def __crop_img(image, ocp_map):
-    if image.dtype != np.uint8 or ocp_map.dtype != np.uint8:
-        image = image.astype(np.uint8)
-        ocp_map = ocp_map.astype(np.uint8)
-    x, y, w, h = cv2.boundingRect(ocp_map)
-    cropped_image = image[y:y+h, x:x+w]
-    cropped_ocp_map = ocp_map[y:y+h, x:x+w]
-    return cropped_image, cropped_ocp_map
-
-
-def generate_projections(points, colors, precision, filtering, crop):
-    if type(points) != np.ndarray:
-        points = np.array(points)
-    if type(colors) != np.ndarray:
-        colors = np.array(colors)
-    points, colors = __preprocess_cloud(points, colors, precision)
-    img, ocp_map = _internal_generate_projections(points, colors, precision, filtering)
-    img, ocp_map = np.asarray(img), np.asarray(ocp_map)
+def apply_cropping(images, ocp_maps):
+    if images.dtype != np.uint8 or ocp_maps.dtype != np.uint8:
+        images = images.astype(np.uint8)
+        ocp_maps = ocp_maps.astype(np.uint8)
+    images_result = []
+    ocp_maps_result = []
+    for i in range(len(images)):
+        image, ocp_map = images[i], ocp_maps[i]
+        x, y, w, h = cv2.boundingRect(ocp_map)
+        cropped_image = image[y:y+h, x:x+w]
+        cropped_ocp_map = ocp_map[y:y+h, x:x+w]
+        images_result.append(cropped_image)
+        ocp_maps_result.append(cropped_ocp_map)
+    return images_result, ocp_maps_result
+
+
+def generate_projections(points, colors, precision, filtering, crop=False):
+    points, colors = __preprocess_point_cloud(points, colors, precision)
+    images, ocp_maps = _internal_generate_projections(points, colors, precision, filtering)
+    images, ocp_maps = np.asarray(images), np.asarray(ocp_maps)
     if crop is True:
-        img_tmp = []
-        ocp_map_tmp = []
-        for i in range(6):
-            im, ocp = __crop_img(img[i], ocp_map[i])
-            img_tmp.append(im)
-            ocp_map_tmp.append(ocp)
-        img, ocp_map = img_tmp, ocp_map_tmp
-    return img, ocp_map
+        images, ocp_maps = apply_cropping(images, ocp_maps)
+    return images, ocp_maps
```

### Comparing `orthographic_projector-0.1.0/src/lib.rs` & `orthographic_projector-0.1.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orthographic_projector-0.1.0/Cargo.lock` & `orthographic_projector-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "orthographic_projector"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "ndarray",
  "numpy",
  "pyo3",
 ]
 
 [[package]]
```

### Comparing `orthographic_projector-0.1.0/pyproject.toml` & `orthographic_projector-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 classifier = [
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python",
     "Programming Language :: Rust",
 ]
 
 [project.urls]
-repository = "https://github.com/akaTsunemori/orthographic-projector"
+repository = "https://github.com/akaTsunemori/orthographic_projector"
```

### Comparing `orthographic_projector-0.1.0/PKG-INFO` & `orthographic_projector-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.3
 Name: orthographic_projector
-Version: 0.1.0
+Version: 0.1.1
 Requires-Dist: numpy >=1.26
 Requires-Dist: opencv-python >=4.9
 Requires-Dist: toml ==0.10.0
 License-File: LICENSE
 Summary: Generate orthographic projections from a Point Cloud.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: repository, https://github.com/akaTsunemori/orthographic-projector
+Project-URL: repository, https://github.com/akaTsunemori/orthographic_projector
 
 # Orthographic Projector
 #### A Rust-based Python library for generating orthographic projections from point clouds.
 
 ## Prerequisites
 - Python 3.10 or later
 - rustc 1.77.2 or later
```

