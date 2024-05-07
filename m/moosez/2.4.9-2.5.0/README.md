# Comparing `tmp/moosez-2.4.9.tar.gz` & `tmp/moosez-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moosez-2.4.9.tar", last modified: Tue May  7 14:26:48 2024, max compression
+gzip compressed data, was "moosez-2.5.0.tar", last modified: Tue May  7 16:28:12 2024, max compression
```

## Comparing `moosez-2.4.9.tar` & `moosez-2.5.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:26:48.285507 moosez-2.4.9/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-07 14:26:44.000000 moosez-2.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-07 14:26:48.285507 moosez-2.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21366 2024-05-07 14:26:44.000000 moosez-2.4.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:26:48.285507 moosez-2.4.9/moosez/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14675 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    25528 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/moosez.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:26:48.285507 moosez-2.4.9/moosez/nnUNet_custom_trainer/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/nnUNet_custom_trainer/MOOSE_custom_trainers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/nnUNet_custom_trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/nnUNet_custom_trainer/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)    15482 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:26:48.285507 moosez-2.4.9/moosez.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-07 14:26:48.000000 moosez-2.4.9/moosez.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-07 14:26:48.000000 moosez-2.4.9/moosez.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:26:48.000000 moosez-2.4.9/moosez.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-07 14:26:48.000000 moosez-2.4.9/moosez.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-07 14:26:48.000000 moosez-2.4.9/moosez.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 14:26:48.000000 moosez-2.4.9/moosez.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 14:26:48.285507 moosez-2.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-07 14:26:44.000000 moosez-2.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:12.438176 moosez-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-07 16:28:07.000000 moosez-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-07 16:28:12.438176 moosez-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21366 2024-05-07 16:28:07.000000 moosez-2.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:12.438176 moosez-2.5.0/moosez/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-07 16:28:07.000000 moosez-2.5.0/moosez/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14564 2024-05-07 16:28:07.000000 moosez-2.5.0/moosez/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-07 16:28:07.000000 moosez-2.5.0/moosez/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-07 16:28:07.000000 moosez-2.5.0/moosez/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-07 16:28:07.000000 moosez-2.5.0/moosez/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-05-07 16:28:07.000000 moosez-2.5.0/moosez/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25759 2024-05-07 16:28:07.000000 moosez-2.5.0/moosez/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-07 16:28:07.000000 moosez-2.5.0/moosez/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13247 2024-05-07 16:28:07.000000 moosez-2.5.0/moosez/moosez.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:12.438176 moosez-2.5.0/moosez/nnUNet_custom_trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-07 16:28:07.000000 moosez-2.5.0/moosez/nnUNet_custom_trainer/MOOSE_custom_trainers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:07.000000 moosez-2.5.0/moosez/nnUNet_custom_trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-07 16:28:07.000000 moosez-2.5.0/moosez/nnUNet_custom_trainer/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-05-07 16:28:07.000000 moosez-2.5.0/moosez/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16110 2024-05-07 16:28:07.000000 moosez-2.5.0/moosez/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:12.438176 moosez-2.5.0/moosez.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-07 16:28:12.000000 moosez-2.5.0/moosez.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-07 16:28:12.000000 moosez-2.5.0/moosez.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 16:28:12.000000 moosez-2.5.0/moosez.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-07 16:28:12.000000 moosez-2.5.0/moosez.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-07 16:28:12.000000 moosez-2.5.0/moosez.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 16:28:12.000000 moosez-2.5.0/moosez.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 16:28:12.438176 moosez-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-07 16:28:07.000000 moosez-2.5.0/setup.py
```

### Comparing `moosez-2.4.9/LICENSE` & `moosez-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moosez-2.4.9/PKG-INFO` & `moosez-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.4.9
+Version: 2.5.0
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/ENHANCE-PET/MOOSE
-Author: Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer
+Author: Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer | Manuel Pires
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: GPLv3
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `moosez-2.4.9/README.md` & `moosez-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `moosez-2.4.9/moosez/constants.py` & `moosez-2.5.0/moosez/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,16 +47,14 @@
 
 TUMOR_LABEL = 12
 
 # FILE NAMES
 
 RESAMPLED_IMAGE_FILE_NAME = 'resampled_image_0000.nii.gz'
 RESAMPLED_MASK_FILE_NAME = 'resampled_mask.nii.gz'
-CHUNK_FILENAMES = ["chunk01_0000.nii.gz", "chunk02_0000.nii.gz", "chunk03_0000.nii.gz"]
-CHUNK_PREFIX = 'chunk'
 
 # DISPLAY PARAMETERS
 
 MIP_ROTATION_STEP = 40
 DISPLAY_VOXEL_SPACING = (3, 3, 3)
 FRAME_DURATION = 0.4
```

### Comparing `moosez-2.4.9/moosez/display.py` & `moosez-2.5.0/moosez/display.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.9/moosez/download.py` & `moosez-2.5.0/moosez/download.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.9/moosez/file_utilities.py` & `moosez-2.5.0/moosez/file_utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,63 +45,57 @@
     :rtype: str
     """
     python_exe = sys.executable
     virtual_env_root = os.path.dirname(os.path.dirname(python_exe))
     return virtual_env_root
 
 
-def get_files(directory: str, wildcard: str) -> list:
+def get_files(directory: str, prefix: str, wildcard: tuple) -> list:
     """
     Returns the list of files in the directory with the specified wildcard.
     
     :param directory: The directory path.
     :type directory: str
     
-    :param wildcard: The wildcard to be used.
-    :type wildcard: str
+    :param wildcard: The wildcards to be used.
+    :type wildcard: tuple
     
     :return: The list of files.
     :rtype: list
     """
     files = []
     for file in os.listdir(directory):
-        if file.endswith(wildcard):
-            files.append(os.path.join(directory, file))
+        if file.startswith(prefix):
+            if file.endswith(wildcard):
+                files.append(os.path.join(directory, file))
     return files
 
 
-def moose_folder_structure(parent_directory: str, model_name: str, modalities: list) -> tuple:
+def moose_folder_structure(parent_directory: str, model_name: str) -> tuple:
     """
     Creates the moose folder structure.
     
     :param parent_directory: The path to the parent directory.
     :type parent_directory: str
     
     :param model_name: The name of the model.
     :type model_name: str
     
-    :param modalities: The list of modalities.
-    :type modalities: list
-    
     :return: A tuple containing the paths to the moose directory, input directories, output directory, and stats directory.
     :rtype: tuple
     """
     moose_dir = os.path.join(parent_directory,
                              'moosez-' + model_name + '-' + datetime.now().strftime('%Y-%m-%d-%H-%M-%S'))
     create_directory(moose_dir)
-    input_dirs = []
-    for modality in modalities:
-        input_dirs.append(os.path.join(moose_dir, modality))
-        create_directory(input_dirs[-1])
 
     output_dir = os.path.join(moose_dir, constants.SEGMENTATIONS_FOLDER)
     stats_dir = os.path.join(moose_dir, constants.STATS_FOLDER)
     create_directory(output_dir)
     create_directory(stats_dir)
-    return moose_dir, input_dirs, output_dir, stats_dir
+    return moose_dir, parent_directory, output_dir, stats_dir
 
 
 def copy_file(file: str, destination: str) -> None:
     """
     Copies a file to the specified destination.
     
     :param file: The path to the file to be copied.
@@ -145,32 +139,14 @@
         files = os.listdir(subject)
         for file in files:
             if file.startswith(modality_tag) and (file.endswith('.nii') or file.endswith('.nii.gz')):
                 selected_files.append(os.path.join(subject, file))
     return selected_files
 
 
-def organise_files_by_modality(moose_compliant_subjects: list, modalities: list, moose_dir: str) -> None:
-    """
-    Organises the files by modality.
-    
-    :param moose_compliant_subjects: The list of moose-compliant subjects paths.
-    :type moose_compliant_subjects: list
-    
-    :param modalities: The list of modalities.
-    :type modalities: list
-    
-    :param moose_dir: The path to the moose directory.
-    :type moose_dir: str
-    """
-    for modality in modalities:
-        files_to_copy = select_files_by_modality(moose_compliant_subjects, modality)
-        copy_files_to_destination(files_to_copy, os.path.join(moose_dir, modality))
-
-
 def find_pet_file(folder: str) -> str:
     """
     Finds the PET file in the specified folder.
     
     :param folder: The path to the folder.
     :type folder: str
```

### Comparing `moosez-2.4.9/moosez/image_conversion.py` & `moosez-2.5.0/moosez/image_conversion.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.9/moosez/image_processing.py` & `moosez-2.5.0/moosez/image_processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 # ----------------------------------------------------------------------------------------------------------------------
 # Author: Lalith Kumar Shiyam Sundar
 #         Sebastian Gutschmayer
+#         Manuel Pires
 # Institution: Medical University of Vienna
 # Research Group: Quantitative Imaging and Medical Physics (QIMP) Team
 # Date: 05.06.2023
 # Version: 2.0.0
 #
 # Description:
 # This module handles image processing for the moosez.
@@ -21,16 +22,15 @@
 
 import SimpleITK as sitk
 import dask
 import dask.array as da
 import nibabel
 import numpy as np
 import pandas as pd
-from moosez.constants import MATRIX_THRESHOLD, Z_AXIS_THRESHOLD, CHUNK_THRESHOLD, MARGIN_PADDING, ORGAN_INDICES, \
-    CHUNK_FILENAMES
+from moosez.constants import MATRIX_THRESHOLD, Z_AXIS_THRESHOLD, CHUNK_THRESHOLD, MARGIN_PADDING, ORGAN_INDICES
 
 
 def get_intensity_statistics(image: sitk.Image, mask_image: sitk.Image, model_name: str, out_csv: str) -> None:
     """
     Get the intensity statistics of a NIFTI image file.
 
     :param image: The source image from which the intensity statistics are calculated.
@@ -91,92 +91,107 @@
             regions_present.append(organ_indices_dict[label])
         else:
             continue
     stats_df.insert(0, 'Regions-Present', np.array(regions_present))
     stats_df.to_csv(out_csv)
 
 
-def split_and_save(image_chunk: da.Array, image_affine: np.ndarray, image_chunk_path: str) -> None:
+def split(image_chunk: da.Array, image_affine: np.ndarray) -> None:
     """
     Get a chunk of the image and save it.
 
     :param image_chunk: The Dask array chunk.
     :type image_chunk: da.Array
     :param image_affine: The image affine transformation.
     :type image_affine: np.ndarray
-    :param image_chunk_path: The path to save the image chunk.
-    :type image_chunk_path: str
     :return: None
     """
     chunk_part = nibabel.Nifti1Image(image_chunk, image_affine)
-    nibabel.save(chunk_part, image_chunk_path)
+    image_data = chunk_part.get_fdata().transpose((2, 1, 0))[None]
+    nnunet_dict = {
+        "nibabel_stuff": {
+            "original_affine": chunk_part.affine
+        },
+        "spacing": [float(i) for i in chunk_part.header.get_zooms()[::-1]]
+    }
+    return image_data, nnunet_dict
 
 
 @dask.delayed
-def delayed_split_and_save(image_chunk: da.Array, image_affine: np.ndarray, image_chunk_path: str) -> None:
+def delayed_split(image_chunk: da.Array, image_affine: np.ndarray) -> None:
     """
     Delayed function to get a chunk of the image and save it.
 
     :param image_chunk: The Dask array chunk.
     :type image_chunk: da.Array
     :param image_affine: The image affine transformation.
     :type image_affine: np.ndarray
-    :param image_chunk_path: The path to save the image chunk.
-    :type image_chunk_path: str
     :return: None
     """
-    split_and_save(image_chunk, image_affine, image_chunk_path)
+    image_data, nnunet_dict = split(image_chunk, image_affine)
+    return image_data, nnunet_dict
 
 
-def write_image(image: nibabel.Nifti1Image, out_image_path: str, large_image: bool = False,
-                is_label: bool = False) -> None:
+def write_segmentation(image: nibabel.Nifti1Image, out_image_path: str) -> None:
     """
     Writes an image either as a single file or multiple files depending on the image size.
 
     :param image: The image to save.
     :type image: nibabel.Nifti1Image
     :param out_image_path: The path to save the image.
     :type out_image_path: str
+    :return: None
+    """
+    resampled_image_path = out_image_path
+    image_as_uint8 = nibabel.Nifti1Image(image.get_fdata().astype(np.uint8), image.affine ,header=image.header)
+    image_as_uint8.set_data_dtype(np.uint8)
+    nibabel.save(image_as_uint8, resampled_image_path)
+
+
+def chunk_image(image: nibabel.Nifti1Image, large_image: bool = False) -> tuple:
+    """
+    Writes an image either as a single file or multiple files depending on the image size.
+
+    :param image: The image to save.
+    :type image: nibabel.Nifti1Image
     :param large_image: Indicates whether the image classifies as large or not.
     :type large_image: bool
-    :param is_label: Indicates whether the image is a label or not.
-    :type is_label: bool
-    :return: None
+    :return: tuple
     """
     image_shape = image.shape
     image_data = da.from_array(image.get_fdata(), chunks=(image_shape[0], image_shape[1], image_shape[2] // 3))
     image_affine = image.affine
 
     if large_image:
         # Calculate indices for image chunks
         num_chunks = 3
         chunk_size = image_shape[2] // num_chunks
         chunk_indices = [(0, chunk_size + MARGIN_PADDING),
                          (chunk_size + 1 - MARGIN_PADDING, chunk_size * 2 + MARGIN_PADDING),
                          (chunk_size * 2 + 1 - MARGIN_PADDING, None)]
-        filenames = CHUNK_FILENAMES
-        save_dir = os.path.dirname(out_image_path)
-        chunk_paths = [os.path.join(save_dir, filename) for filename in filenames]
 
         tasks = []
-        for i, chunk_path in enumerate(chunk_paths):
-            tasks.append(delayed_split_and_save(image_data[:, :, chunk_indices[i][0]:chunk_indices[i][1]].compute(),
-                                                image_affine, chunk_path))
+        for i in range (num_chunks):
+            tasks.append(delayed_split(image_data[:, :, chunk_indices[i][0]:chunk_indices[i][1]].compute(),
+                                                image_affine))
 
-        dask.compute(*tasks)
+        chunk_list = dask.compute(*tasks)
 
-    else:
-        if is_label:
-            resampled_image_path = out_image_path
-            image_as_uint8 = nibabel.Nifti1Image(image.get_fdata().astype(np.uint8), image.affine ,header=image.header)
-            nibabel.save(image_as_uint8, resampled_image_path)
-        else:
-            resampled_image_path = out_image_path
-            nibabel.save(image, resampled_image_path)
+        resampled_image_data = [chunk[0] for chunk in chunk_list]
+        nnunet_dict = [chunk[1] for chunk in chunk_list]
 
+    else:
+        resampled_image_data = image.get_fdata().transpose((2, 1, 0))[None]
+        nnunet_dict = {
+            "nibabel_stuff": {
+                "original_affine": image.affine
+            },
+            "spacing": [float(i) for i in image.header.get_zooms()[::-1]] # Also retrieved like this to make it consistent with sitk
+        }
+    return resampled_image_data, nnunet_dict
 
 class NiftiPreprocessor:
     """
     A class for processing NIfTI images using nibabel and SimpleITK.
 
     Attributes:
     -----------
@@ -532,40 +547,38 @@
         resampled_image = nibabel.Nifti1Image(sitk.GetArrayFromImage(resampled_sitk_image).swapaxes(0, 2),
                                               affine=new_affine,
                                               header=image_header)
 
         return resampled_image
 
     @staticmethod
-    def resample_segmentations(input_image_path: str, desired_spacing: tuple,
+    def resample_segmentations(input_image: nibabel.Nifti1Image, desired_spacing: tuple,
                                desired_size: tuple) -> nibabel.Nifti1Image:
         """
         Resamples an image to a new spacing.
 
-        :param input_image_path: Path to the input image.
-        :type input_image_path: str
+        :param input_image: Image to resample.
+        :type input_image: nibabel.Nifti1Image
         :param desired_spacing: The new spacing to use.
         :type desired_spacing: tuple
         :param desired_size: The new size to use.
         :type desired_size: tuple
         :return: The resampled image as nibabel.Nifti1Image.
         :rtype: nibabel.Nifti1Image
         """
         # Load the image and get necessary information
-        input_image = nibabel.load(input_image_path)
         image_data = input_image.get_fdata()
         image_header = input_image.header
         image_affine = input_image.affine
         original_spacing = image_header.get_zooms()
         translation_vector = image_affine[:3, 3]
         rotation_matrix = image_affine[:3, :3]
 
         # Convert to SimpleITK image format
-        image_data_swapped_axes = image_data.swapaxes(0, 2)
-        sitk_input_image = sitk.GetImageFromArray(image_data_swapped_axes)
+        sitk_input_image = sitk.GetImageFromArray(image_data)
         sitk_input_image.SetSpacing([spacing.item() for spacing in original_spacing])
         axis_flip_matrix = np.diag([-1, -1, 1])
         sitk_input_image.SetOrigin(np.dot(axis_flip_matrix, translation_vector))
         sitk_input_image.SetDirection(
             (np.dot(axis_flip_matrix, rotation_matrix) / np.absolute(original_spacing)).ravel())
 
         desired_spacing = np.array(desired_spacing).astype(np.float64)
```

### Comparing `moosez-2.4.9/moosez/input_validation.py` & `moosez-2.5.0/moosez/input_validation.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,26 +22,14 @@
 import os
 from typing import List
 
 import nibabel as nib
 from moosez import constants
 
 
-def check_directory_exists(directory_path: str) -> None:
-    """
-    Checks if the specified directory exists.
-
-    :param directory_path: The path to the directory.
-    :type directory_path: str
-    :raises: Exception if the directory does not exist.
-    """
-    if not os.path.isdir(directory_path):
-        raise Exception(f"Error: The directory '{directory_path}' does not exist.")
-
-
 def select_moose_compliant_subjects(subject_paths: List[str], modality_tags: List[str]) -> List[str]:
     """
     Selects the subjects that have the files that have names that are compliant with the moosez.
 
     :param subject_paths: The path to the list of subjects that are present in the parent directory.
     :type subject_paths: List[str]
     :param modality_tags: The list of appropriate modality prefixes that should be attached to the files for them to be moose compliant.
```

### Comparing `moosez-2.4.9/moosez/moosez.py` & `moosez-2.5.0/moosez/moosez.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 # ----------------------------------------------------------------------------------------------------------------------
 # Author: Lalith Kumar Shiyam Sundar
+#         Manuel Pires
 # Institution: Medical University of Vienna
 # Research Group: Quantitative Imaging and Medical Physics (QIMP) Team
 # Date: 09.02.2023
 # Version: 2.0.0
 #
 # Description:
 # The main module of the mooseZ. It contains the main function that is executed when the mooseZ is run.
@@ -18,14 +19,19 @@
 
 import argparse
 import glob
 import logging
 import os
 import time
 from datetime import datetime
+import sys
+
+os.environ["nnUNet_raw"] = ""
+os.environ["nnUNet_preprocessed"] = ""
+os.environ["nnUNet_results"] = ""
 
 import SimpleITK
 import colorama
 import emoji
 from halo import Halo
 from moosez import constants
 from moosez import display
@@ -38,16 +44,17 @@
 from moosez import resources
 from moosez.image_processing import ImageResampler
 from moosez.nnUNet_custom_trainer.utility import add_custom_trainers_to_local_nnunetv2
 from moosez.resources import MODELS, AVAILABLE_MODELS
 
 
 def main():
+    log_filename = datetime.now().strftime('moosez-v.2.0.0.%H-%M-%d-%m-%Y.log')
     logging.basicConfig(format='%(asctime)s %(levelname)-8s [%(filename)s:%(lineno)d] %(message)s', level=logging.INFO,
-                        filename=datetime.now().strftime('moosez-v.2.0.0.%H-%M-%d-%m-%Y.log'), filemode='w')
+                        filename=log_filename, filemode='w')
     colorama.init()
 
     # Argument parser
     parser = argparse.ArgumentParser(
         description=display.get_usage_message(),
         formatter_class=argparse.RawTextHelpFormatter,  # To retain the custom formatting
         add_help=False  # We'll add our own help option later
@@ -149,57 +156,69 @@
         print(
             f'{constants.ANSI_RED} {emoji.emojize(":cross_mark:")} No moose compliant subject found to continue!{constants.ANSI_RESET} {emoji.emojize(":light_bulb:")} See: https://github.com/ENHANCE-PET/MOOSE#directory-structure-and-naming-conventions-for-moose-%EF%B8%8F')
         return
 
     # -------------------------------------------------
     # RUN PREDICTION ONLY FOR MOOSE COMPLIANT SUBJECTS
     # -------------------------------------------------
+    original_stdout = sys.stdout
+    original_stderr = sys.stderr
 
     print('')
     print(f'{constants.ANSI_VIOLET} {emoji.emojize(":crystal_ball:")} PREDICT:{constants.ANSI_RESET}')
     print('')
     logging.info(' ')
     logging.info(' PERFORMING PREDICTION:')
     logging.info(' ')
+    # Catch nnunet output to a text file to make debugging nnunet problems easier
+    with open(f"nnunet_output_{log_filename}", "w") as f:
+        sys.stdout = f
+        sys.stderr = f
+        model = predict.initialize_model(model_name)
+    sys.stdout = original_stdout
+    sys.stderr = original_stderr
 
     spinner = Halo(text=' Initiating', spinner='dots')
     spinner.start()
     start_total_time = time.time()
 
     for i, subject in enumerate(moose_compliant_subjects):
         # SETTING UP DIRECTORY STRUCTURE
         spinner.text = f'[{i + 1}/{num_subjects}] Setting up directory structure for {os.path.basename(subject)}...'
         logging.info(' ')
         logging.info(f'{constants.ANSI_VIOLET} SETTING UP MOOSE-Z DIRECTORY:'
                      f'{constants.ANSI_RESET}')
         logging.info(' ')
-        moose_dir, input_dirs, output_dir, stats_dir = file_utilities.moose_folder_structure(subject, model_name,
-                                                                                             modalities)
+        moose_dir, input_dir, output_dir, stats_dir = file_utilities.moose_folder_structure(subject, model_name)
         logging.info(f" MOOSE directory for subject {os.path.basename(subject)} at: {moose_dir}")
 
         # ORGANISE DATA ACCORDING TO MODALITY
         spinner.text = f'[{i + 1}/{num_subjects}] Organising data according to modality for {os.path.basename(subject)}...'
-        file_utilities.organise_files_by_modality([subject], modalities, moose_dir)
 
         # PREPARE THE DATA FOR PREDICTION
         spinner.text = f'[{i + 1}/{num_subjects}] Preparing data for prediction for {os.path.basename(subject)}...'
-        for input_dir in input_dirs:
-            input_validation.make_nnunet_compatible(input_dir)
+
         logging.info(f" {constants.ANSI_GREEN}Data preparation complete using {model_name} for subject "
                      f"{os.path.basename(subject)}{constants.ANSI_RESET}")
 
         # RUN PREDICTION
         start_time = time.time()
         logging.info(' ')
         logging.info(' RUNNING PREDICTION:')
         logging.info(' ')
         spinner.text = f'[{i + 1}/{num_subjects}] Running prediction for {os.path.basename(subject)} using {model_name}...'
 
-        for input_dir in input_dirs:
-            predict.predict(model_name, input_dir, output_dir, accelerator)
+        # Catch nnunet output to a text file to make debugging nnunet problems easier
+        with open(f"nnunet_output_{log_filename}", "a") as f:
+            sys.stdout = f
+            sys.stderr = f
+            predict.predict_from_array(model, input_dir, output_dir, model_name)
+        sys.stdout = original_stdout
+        sys.stderr = original_stderr
+
         logging.info(f"Prediction complete using {model_name}.")
 
         end_time = time.time()
         elapsed_time = end_time - start_time
         spinner.text = f' {constants.ANSI_GREEN}[{i + 1}/{num_subjects}] Prediction done for {os.path.basename(subject)} using {model_name}!' \
                        f' | Elapsed time: {round(elapsed_time / 60, 1)} min{constants.ANSI_RESET}'
         time.sleep(3)
```

### Comparing `moosez-2.4.9/moosez/nnUNet_custom_trainer/MOOSE_custom_trainers.py` & `moosez-2.5.0/moosez/nnUNet_custom_trainer/MOOSE_custom_trainers.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.9/moosez/nnUNet_custom_trainer/utility.py` & `moosez-2.5.0/moosez/nnUNet_custom_trainer/utility.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.9/moosez/resources.py` & `moosez-2.5.0/moosez/resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,160 +62,177 @@
 MODELS = {
     "clin_ct_lungs": {
         "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_lungs_24062023.zip",
         "filename": "Dataset333_HMS3dlungs.zip",
         "directory": "Dataset333_HMS3dlungs",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
-        "multilabel_prefix": "CT_Lungs_",
-        "configuration": "3d_fullres"
+        "multilabel_prefix": "Clin_CT_Lungs_",
+        "configuration": "3d_fullres",
+        "planner": "nnUNetPlans"
     },
     "clin_ct_organs": {
         "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_organs_23062023.zip",
         "filename": "Dataset123_Organs.zip",
         "directory": "Dataset123_Organs",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
-        "multilabel_prefix": "CT_Organs_",
-        "configuration": "3d_fullres"
+        "multilabel_prefix": "Clin_CT_Organs_",
+        "configuration": "3d_fullres",
+        "planner": "nnUNetPlans"
     },
     "preclin_mr_all": {
         "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/preclin_mr_all_05122023.zip",
         "filename": "Dataset234_minimoose.zip",
         "directory": "Dataset234_minimoose",
         "trainer": "nnUNetTrainer",
         "voxel_spacing": [0.4000000059604645, 0.4000000059604645, 0.4000000059604645],
         "multilabel_prefix": "Preclin_MR_all_",
-        "configuration": "3d_fullres"
+        "configuration": "3d_fullres",
+        "planner": "nnUNetPlans"
     },
     "clin_ct_body": {
         "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_body_27112023.zip",
         "filename": "Dataset001_body.zip",
         "directory": "Dataset001_body",
         "trainer": "nnUNetTrainer",
         "voxel_spacing": [5, 5, 5],
-        "multilabel_prefix": "CT_Body_",
-        "configuration": "3d_fullres"
+        "multilabel_prefix": "Clin_CT_Body_",
+        "configuration": "3d_fullres",
+        "planner": "nnUNetPlans"
     },
     "clin_ct_ribs": {
         "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_ribs_19032024.zip",
         "filename": "Dataset444_Ribs.zip",
         "directory": "Dataset444_Ribs",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
-        "multilabel_prefix": "CT_Ribs_",
-        "configuration": "3d_fullres_big_patch"
+        "multilabel_prefix": "Clin_CT_Ribs_",
+        "configuration": "3d_fullres_big_patch",
+        "planner": "nnUNetPlans"
     },
     "clin_ct_muscles": {
         "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_muscles_06022024.zip",
         "filename": "Dataset555_Muscles.zip",
         "directory": "Dataset555_Muscles",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
-        "multilabel_prefix": "CT_Muscles_",
-        "configuration": "3d_fullres"
+        "multilabel_prefix": "Clin_CT_Muscles_",
+        "configuration": "3d_fullres",
+        "planner": "nnUNetPlans"
     },
     "clin_ct_peripheral_bones": {
         "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_peripheral_bones_28082023.zip",
         "filename": "Dataset666_Peripheral-Bones.zip",
         "directory": "Dataset666_Peripheral-Bones",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
-        "multilabel_prefix": "CT_Peripheral-Bones_",
-        "configuration": "3d_fullres"
+        "multilabel_prefix": "Clin_CT_Peripheral-Bones_",
+        "configuration": "3d_fullres",
+        "planner": "nnUNetPlans"
     },
     "clin_ct_fat": {
         "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_fat_31082023.zip",
         "filename": "Dataset777_Fat.zip",
         "directory": "Dataset777_Fat",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
-        "multilabel_prefix": "CT_Fat_",
-        "configuration": "3d_fullres"
+        "multilabel_prefix": "Clin_CT_Fat_",
+        "configuration": "3d_fullres",
+        "planner": "nnUNetPlans"
     },
     "clin_ct_vertebrae": {
         "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_vertebrae_da5_03102023.zip",
         "filename": "Dataset111_Vertebrae.zip",
         "directory": "Dataset111_Vertebrae",
         "trainer": "nnUNetTrainer_2000_epochs_DA5NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
-        "multilabel_prefix": "CT_Vertebrae_",
-        "configuration": "3d_fullres"
+        "multilabel_prefix": "Clin_CT_Vertebrae_",
+        "configuration": "3d_fullres",
+        "planner": "nnUNetPlans"
     },
     "clin_ct_cardiac": {
         "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_cardiac_26012024.zip",
         "filename": "Dataset888_Cardiac.zip",
         "directory": "Dataset888_Cardiac",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
-        "multilabel_prefix": "CT_Cardiac_",
-        "configuration": "3d_fullres"
+        "multilabel_prefix": "Clin_CT_Cardiac_",
+        "configuration": "3d_fullres",
+        "planner": "nnUNetPlans"
     },
     "clin_ct_digestive": {
         "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_digestive_10092023.zip",
         "filename": "Dataset999_Digestive.zip",
         "directory": "Dataset999_Digestive",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
-        "multilabel_prefix": "CT_Digestive_",
-        "configuration": "3d_fullres"
+        "multilabel_prefix": "Clin_CT_Digestive_",
+        "configuration": "3d_fullres",
+        "planner": "nnUNetPlans"
     },
     "preclin_ct_legs": {
         "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/preclin_ct_legs_05122023.zip",
         "filename": "Dataset256_Preclin_leg_muscles.zip",
         "directory": "Dataset256_Preclin_leg_muscles",
         "trainer": "nnUNetTrainerNoMirroring",
         "voxel_spacing": [0.18000000715255737, 0.18000000715255737, 0.18000000715255737],
         "multilabel_prefix": "Preclin_CT_legs_",
-        "configuration": "3d_fullres"
+        "configuration": "3d_fullres",
+        "planner": "nnUNetPlans"
     },
     "clin_ct_all_bones_v1": {
         "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_all_bones_25102023.zip",
         "filename": "Dataset600_Original_bones.zip",
         "directory": "Dataset600_Original_bones",
         "trainer": "nnUNetTrainer_2000epochs",
         "voxel_spacing": [1.5, 1.5, 1.5],
         "multilabel_prefix": "Clin_CT_all_bones_",
-        "configuration": "3d_fullres"
+        "configuration": "3d_fullres",
+        "planner": "nnUNetPlans"
     },
     "clin_ct_PUMA": {
         "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_puma_04042024.zip",
         "filename": "Dataset002_PUMA.zip",
         "directory": "Dataset002_PUMA",
         "trainer": "nnUNetTrainer_2000epochs",
         "voxel_spacing": [1.5, 1.5, 1.5],
         "multilabel_prefix": "Clin_CT_PUMA_",
-        "configuration": "3d_fullres"
+        "configuration": "3d_fullres",
+        "planner": "nnUNetPlans"
     },
     "clin_pt_fdg_brain_v1": {
         "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_fdg_pt_brain_v1_17112023.zip",
         "filename": "Dataset100_Brain_v1.zip",
         "directory": "Dataset100_Brain_v1",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [2.03125, 2.0862598419189453, 2.0862600803375244],
         "multilabel_prefix": "Clin_PT_FDG_brain_",
-        "configuration": "3d_fullres"
+        "configuration": "3d_fullres",
+        "planner": "nnUNetPlans"
     },
     "clin_ct_ALPACA": {
         "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_ALPACA.zip",
-        "filename": "Dataset080_ALPACA.zip",
-        "directory": "Dataset080_ALPACA",
+        "filename": "Dataset080_Alpaca.zip",
+        "directory": "Dataset080_Alpaca",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
         "multilabel_prefix": "Clin_CT_ALPACA_",
-        "configuration": "3d_fullres"
+        "configuration": "3d_fullres",
+        "planner": "nnUNetPlans"
     },
     "clin_ct_PUMA4": {
         "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_PUMA4_06032024.zip",
         "filename": "Dataset003_PUMA4.zip",
         "directory": "Dataset003_PUMA4",
         "trainer": "nnUNetTrainer_2000epochs",
         "voxel_spacing": [4, 4, 4],
         "multilabel_prefix": "Clin_CT_PUMA4_",
-        "configuration": "3d_fullres"
+        "configuration": "3d_fullres",
+        "planner": "nnUNetPlans"
     }
 }
 
 
 # This function returns a dictionary indicating the expected modality for a given model_name, the imaging technique,
 # the type of tissue to be segmented. The model_name should be the same as the unique identifier mentioned in the
 # MODELS dictionary above and the AVAILABLE_MODELS list.
```

### Comparing `moosez-2.4.9/moosez.egg-info/PKG-INFO` & `moosez-2.5.0/moosez.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.4.9
+Version: 2.5.0
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/ENHANCE-PET/MOOSE
-Author: Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer
+Author: Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer | Manuel Pires
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: GPLv3
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `moosez-2.4.9/moosez.egg-info/SOURCES.txt` & `moosez-2.5.0/moosez.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moosez-2.4.9/setup.py` & `moosez-2.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='moosez',
-    version='2.4.9',
-    author='Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer',
+    version='2.5.0',
+    author='Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer | Manuel Pires',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at',
     description='An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks',
     python_requires='>=3.10',
     long_description='mooseZ is an AI-inference engine based on nnUNet, designed for 3D clinical and preclinical'
                      ' whole-body segmentation tasks. It serves models tailored towards different modalities such'
                      ' as PET, CT, and MR. mooseZ provides fast and accurate segmentation results, making it a '
                      'reliable tool for medical imaging applications.',
```

