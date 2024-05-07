# Comparing `tmp/abm_initialization_collection-0.6.0.tar.gz` & `tmp/abm_initialization_collection-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abm_initialization_collection-0.6.0.tar", max compression
+gzip compressed data, was "abm_initialization_collection-0.6.1.tar", max compression
```

## Comparing `abm_initialization_collection-0.6.0.tar` & `abm_initialization_collection-0.6.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1540 2023-10-18 18:07:00.001908 abm_initialization_collection-0.6.0/LICENSE
--rw-r--r--   0        0        0     3082 2023-10-18 18:07:00.001908 abm_initialization_collection-0.6.0/README.md
--rw-r--r--   0        0        0     1980 2023-10-18 18:07:00.005908 abm_initialization_collection-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-10-18 18:07:00.005908 abm_initialization_collection-0.6.0/src/abm_initialization_collection/__init__.py
--rw-r--r--   0        0        0       52 2023-10-18 18:07:00.005908 abm_initialization_collection-0.6.0/src/abm_initialization_collection/__main__.py
--rw-r--r--   0        0        0      307 2023-10-18 18:07:00.005908 abm_initialization_collection-0.6.0/src/abm_initialization_collection/coordinate/__init__.py
--rw-r--r--   0        0        0      904 2023-10-18 18:07:00.005908 abm_initialization_collection-0.6.0/src/abm_initialization_collection/coordinate/filter_coordinate_bounds.py
--rw-r--r--   0        0        0     3064 2023-10-18 18:07:00.005908 abm_initialization_collection-0.6.0/src/abm_initialization_collection/coordinate/make_grid_coordinates.py
--rw-r--r--   0        0        0      456 2023-10-18 18:07:00.005908 abm_initialization_collection-0.6.0/src/abm_initialization_collection/image/__init__.py
--rw-r--r--   0        0        0     4102 2023-10-18 18:07:00.005908 abm_initialization_collection-0.6.0/src/abm_initialization_collection/image/create_voronoi_image.py
--rw-r--r--   0        0        0      407 2023-10-18 18:07:00.005908 abm_initialization_collection-0.6.0/src/abm_initialization_collection/image/get_image_bounds.py
--rw-r--r--   0        0        0     3181 2023-10-18 18:07:00.005908 abm_initialization_collection-0.6.0/src/abm_initialization_collection/image/plot_contact_sheet.py
--rw-r--r--   0        0        0     1127 2023-10-18 18:07:00.005908 abm_initialization_collection-0.6.0/src/abm_initialization_collection/image/select_fov_images.py
--rw-r--r--   0        0        0        0 2023-10-18 18:07:00.005908 abm_initialization_collection-0.6.0/src/abm_initialization_collection/py.typed
--rw-r--r--   0        0        0      824 2023-10-18 18:07:00.005908 abm_initialization_collection-0.6.0/src/abm_initialization_collection/sample/__init__.py
--rw-r--r--   0        0        0      454 2023-10-18 18:07:00.005908 abm_initialization_collection-0.6.0/src/abm_initialization_collection/sample/exclude_selected_ids.py
--rw-r--r--   0        0        0      716 2023-10-18 18:07:00.005908 abm_initialization_collection-0.6.0/src/abm_initialization_collection/sample/get_image_samples.py
--rw-r--r--   0        0        0     2724 2023-10-18 18:07:00.005908 abm_initialization_collection-0.6.0/src/abm_initialization_collection/sample/get_sample_indices.py
--rw-r--r--   0        0        0      450 2023-10-18 18:07:00.005908 abm_initialization_collection-0.6.0/src/abm_initialization_collection/sample/include_selected_ids.py
--rw-r--r--   0        0        0     1812 2023-10-18 18:07:00.005908 abm_initialization_collection-0.6.0/src/abm_initialization_collection/sample/remove_edge_regions.py
--rw-r--r--   0        0        0     6177 2023-10-18 18:07:00.005908 abm_initialization_collection-0.6.0/src/abm_initialization_collection/sample/remove_unconnected_regions.py
--rw-r--r--   0        0        0     1453 2023-10-18 18:07:00.005908 abm_initialization_collection-0.6.0/src/abm_initialization_collection/sample/scale_sample_coordinates.py
--rw-r--r--   0        0        0     3944 1970-01-01 00:00:00.000000 abm_initialization_collection-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1540 2024-05-07 15:36:54.161644 abm_initialization_collection-0.6.1/LICENSE
+-rw-r--r--   0        0        0     3082 2024-05-07 15:36:54.161644 abm_initialization_collection-0.6.1/README.md
+-rw-r--r--   0        0        0     1974 2024-05-07 15:36:54.165644 abm_initialization_collection-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-07 15:36:54.165644 abm_initialization_collection-0.6.1/src/abm_initialization_collection/__init__.py
+-rw-r--r--   0        0        0       52 2024-05-07 15:36:54.165644 abm_initialization_collection-0.6.1/src/abm_initialization_collection/__main__.py
+-rw-r--r--   0        0        0      307 2024-05-07 15:36:54.165644 abm_initialization_collection-0.6.1/src/abm_initialization_collection/coordinate/__init__.py
+-rw-r--r--   0        0        0      904 2024-05-07 15:36:54.165644 abm_initialization_collection-0.6.1/src/abm_initialization_collection/coordinate/filter_coordinate_bounds.py
+-rw-r--r--   0        0        0     3064 2024-05-07 15:36:54.165644 abm_initialization_collection-0.6.1/src/abm_initialization_collection/coordinate/make_grid_coordinates.py
+-rw-r--r--   0        0        0      456 2024-05-07 15:36:54.165644 abm_initialization_collection-0.6.1/src/abm_initialization_collection/image/__init__.py
+-rw-r--r--   0        0        0     4088 2024-05-07 15:36:54.165644 abm_initialization_collection-0.6.1/src/abm_initialization_collection/image/create_voronoi_image.py
+-rw-r--r--   0        0        0      399 2024-05-07 15:36:54.165644 abm_initialization_collection-0.6.1/src/abm_initialization_collection/image/get_image_bounds.py
+-rw-r--r--   0        0        0     3181 2024-05-07 15:36:54.165644 abm_initialization_collection-0.6.1/src/abm_initialization_collection/image/plot_contact_sheet.py
+-rw-r--r--   0        0        0     1127 2024-05-07 15:36:54.165644 abm_initialization_collection-0.6.1/src/abm_initialization_collection/image/select_fov_images.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:36:54.165644 abm_initialization_collection-0.6.1/src/abm_initialization_collection/py.typed
+-rw-r--r--   0        0        0      824 2024-05-07 15:36:54.165644 abm_initialization_collection-0.6.1/src/abm_initialization_collection/sample/__init__.py
+-rw-r--r--   0        0        0      454 2024-05-07 15:36:54.165644 abm_initialization_collection-0.6.1/src/abm_initialization_collection/sample/exclude_selected_ids.py
+-rw-r--r--   0        0        0      708 2024-05-07 15:36:54.165644 abm_initialization_collection-0.6.1/src/abm_initialization_collection/sample/get_image_samples.py
+-rw-r--r--   0        0        0     2724 2024-05-07 15:36:54.165644 abm_initialization_collection-0.6.1/src/abm_initialization_collection/sample/get_sample_indices.py
+-rw-r--r--   0        0        0      450 2024-05-07 15:36:54.165644 abm_initialization_collection-0.6.1/src/abm_initialization_collection/sample/include_selected_ids.py
+-rw-r--r--   0        0        0     1812 2024-05-07 15:36:54.165644 abm_initialization_collection-0.6.1/src/abm_initialization_collection/sample/remove_edge_regions.py
+-rw-r--r--   0        0        0     6177 2024-05-07 15:36:54.165644 abm_initialization_collection-0.6.1/src/abm_initialization_collection/sample/remove_unconnected_regions.py
+-rw-r--r--   0        0        0     1453 2024-05-07 15:36:54.165644 abm_initialization_collection-0.6.1/src/abm_initialization_collection/sample/scale_sample_coordinates.py
+-rw-r--r--   0        0        0     3989 1970-01-01 00:00:00.000000 abm_initialization_collection-0.6.1/PKG-INFO
```

### Comparing `abm_initialization_collection-0.6.0/LICENSE` & `abm_initialization_collection-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.6.0/README.md` & `abm_initialization_collection-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.6.0/pyproject.toml` & `abm_initialization_collection-0.6.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "abm-initialization-collection"
-version = "0.6.0"
+version = "0.6.1"
 description = "Collection of tasks for initializing ABM simulations."
 authors = [
     "Jessica S. Yu <jesyu@uw.edu>"
 ]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 prefect = "^2.8.2"
 numpy = "^1.24.2"
 pandas = "^1.5.3"
 matplotlib = "^3.7.0"
 hexalattice = "^1.2.1"
-aicsimageio = "^4.9.4"
+bioio = "^1.0.0"
 scikit-image = "^0.19.3"
 scipy = "^1.9.3"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "^5.12.0"
 mypy = "^1.3.0"
```

### Comparing `abm_initialization_collection-0.6.0/src/abm_initialization_collection/coordinate/filter_coordinate_bounds.py` & `abm_initialization_collection-0.6.1/src/abm_initialization_collection/coordinate/filter_coordinate_bounds.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.6.0/src/abm_initialization_collection/coordinate/make_grid_coordinates.py` & `abm_initialization_collection-0.6.1/src/abm_initialization_collection/coordinate/make_grid_coordinates.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.6.0/src/abm_initialization_collection/image/create_voronoi_image.py` & `abm_initialization_collection-0.6.1/src/abm_initialization_collection/image/create_voronoi_image.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from math import floor
 
 import numpy as np
-from aicsimageio import AICSImage
+from bioio import BioImage
 from scipy.ndimage import binary_dilation, binary_fill_holes, distance_transform_edt
 
 
-def create_voronoi_image(
-    image: AICSImage, channel: int, iterations: int, height: int
-) -> np.ndarray:
+def create_voronoi_image(image: BioImage, channel: int, iterations: int, height: int) -> np.ndarray:
     array = image.get_image_data("ZYX", T=0, C=channel)
 
     # Create artificial boundary for voronoi.
     mask = create_boundary_mask(array, iterations)
     lower_bound, upper_bound = get_mask_bounds(array, height)
     mask_id = np.iinfo(array.dtype).max
     array[mask == 0] = mask_id
```

### Comparing `abm_initialization_collection-0.6.0/src/abm_initialization_collection/image/plot_contact_sheet.py` & `abm_initialization_collection-0.6.1/src/abm_initialization_collection/image/plot_contact_sheet.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.6.0/src/abm_initialization_collection/image/select_fov_images.py` & `abm_initialization_collection-0.6.1/src/abm_initialization_collection/image/select_fov_images.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.6.0/src/abm_initialization_collection/sample/__init__.py` & `abm_initialization_collection-0.6.1/src/abm_initialization_collection/sample/__init__.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.6.0/src/abm_initialization_collection/sample/get_image_samples.py` & `abm_initialization_collection-0.6.1/src/abm_initialization_collection/sample/get_image_samples.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
-from aicsimageio import AICSImage
+from bioio import BioImage
 
 
-def get_image_samples(image: AICSImage, sample_indices: list, channel: int) -> pd.DataFrame:
+def get_image_samples(image: BioImage, sample_indices: list, channel: int) -> pd.DataFrame:
     """
     Sample image at given indices into list of (id, x, y, z) samples.
 
     Parameters
     ----------
     image
         Image object to sample.
```

### Comparing `abm_initialization_collection-0.6.0/src/abm_initialization_collection/sample/get_sample_indices.py` & `abm_initialization_collection-0.6.1/src/abm_initialization_collection/sample/get_sample_indices.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.6.0/src/abm_initialization_collection/sample/remove_edge_regions.py` & `abm_initialization_collection-0.6.1/src/abm_initialization_collection/sample/remove_edge_regions.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.6.0/src/abm_initialization_collection/sample/remove_unconnected_regions.py` & `abm_initialization_collection-0.6.1/src/abm_initialization_collection/sample/remove_unconnected_regions.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.6.0/src/abm_initialization_collection/sample/scale_sample_coordinates.py` & `abm_initialization_collection-0.6.1/src/abm_initialization_collection/sample/scale_sample_coordinates.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.6.0/PKG-INFO` & `abm_initialization_collection-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: abm-initialization-collection
-Version: 0.6.0
+Version: 0.6.1
 Summary: Collection of tasks for initializing ABM simulations.
 License: BSD-3-Clause
 Author: Jessica S. Yu
 Author-email: jesyu@uw.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aicsimageio (>=4.9.4,<5.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: bioio (>=1.0.0,<2.0.0)
 Requires-Dist: hexalattice (>=1.2.1,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.0,<4.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: prefect (>=2.8.2,<3.0.0)
 Requires-Dist: scikit-image (>=0.19.3,<0.20.0)
 Requires-Dist: scipy (>=1.9.3,<2.0.0)
```

