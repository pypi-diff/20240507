# Comparing `tmp/pisahkan_ktp-0.0.3.tar.gz` & `tmp/pisahkan_ktp-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pisahkan_ktp-0.0.3.tar", max compression
+gzip compressed data, was "pisahkan_ktp-0.0.4.tar", max compression
```

## Comparing `pisahkan_ktp-0.0.3.tar` & `pisahkan_ktp-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1097 2024-05-07 03:55:25.046040 pisahkan_ktp-0.0.3/LICENSE
--rwxr-xr-x   0        0        0     1996 2024-05-07 06:53:15.180845 pisahkan_ktp-0.0.3/README.md
--rwxr-xr-x   0        0        0      690 2024-05-07 07:03:40.580569 pisahkan_ktp-0.0.3/pyproject.toml
--rwxr-xr-x   0        0        0        0 2024-05-07 03:58:19.125178 pisahkan_ktp-0.0.3/src/pisahkan_ktp/__init__.py
--rwxr-xr-x   0        0        0    10785 2024-05-07 06:57:16.481480 pisahkan_ktp-0.0.3/src/pisahkan_ktp/ktp_segmenter.py
--rw-r--r--   0        0        0     2741 1970-01-01 00:00:00.000000 pisahkan_ktp-0.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1097 2024-05-07 03:55:25.046040 pisahkan_ktp-0.0.4/LICENSE
+-rwxr-xr-x   0        0        0     2055 2024-05-07 07:12:10.276685 pisahkan_ktp-0.0.4/README.md
+-rwxr-xr-x   0        0        0      690 2024-05-07 07:15:25.866253 pisahkan_ktp-0.0.4/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2024-05-07 03:58:19.125178 pisahkan_ktp-0.0.4/src/pisahkan_ktp/__init__.py
+-rwxr-xr-x   0        0        0    10887 2024-05-07 07:15:08.105205 pisahkan_ktp-0.0.4/src/pisahkan_ktp/ktp_segmenter.py
+-rw-r--r--   0        0        0     2799 1970-01-01 00:00:00.000000 pisahkan_ktp-0.0.4/PKG-INFO
```

### Comparing `pisahkan_ktp-0.0.3/LICENSE` & `pisahkan_ktp-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pisahkan_ktp-0.0.3/README.md` & `pisahkan_ktp-0.0.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # **PISAHKAN KTP: Indonesian ID Card (KTP) Information Segmentation**
 
-![Image](./assets/OIG1.jpg)
+<center><img src="./assets/OIG1.jpg" alt="Beautiful Landscape" width="250"></center>
+
 
 ## **About**
 `pisahkan_ktp` is a Python function that extracts province, NIK, and personal information from an image of an Indonesian National Identity Card (KTP). It utilizes image processing techniques to locate and isolate relevant sections of the KTP image, then extracts text data accurately. The extracted information is returned in a structured format, facilitating further processing or integration into other applications.
 
 ## **Requirements**
 - Python 3.7 or Higher
 - numpy
```

### Comparing `pisahkan_ktp-0.0.3/pyproject.toml` & `pisahkan_ktp-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pisahkan-ktp"
-version = "0.0.3"
+version = "0.0.4"
 authors = ["Hanif Yuli Abdillah P <hanifabd23@gmail.com>"]
 description = "Python package for detecting entities in text based on a dictionary and fuzzy similarity"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `pisahkan_ktp-0.0.3/src/pisahkan_ktp/ktp_segmenter.py` & `pisahkan_ktp-0.0.4/src/pisahkan_ktp/ktp_segmenter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import cv2
 import numpy as np
 import math
 from pythonRLSA.rlsa_fast import rlsa_fast
 
 def add_white_block_signature(image, block_width, block_height):
     # Get the dimensions of the original image
@@ -235,14 +236,17 @@
 def segmenter(image_path):
     '''
      This function identifies and isolates sections of Indonesian identity cards from images. 
      By detecting text and photo areas, it creates boundaries for province, nik, and personal information.
     '''
     assert isinstance(image_path, str), "Tokens can be str() type only"
 
+    if not os.path.exists(image_path):
+        return "Image File not Exists!"
+        
     # Original Image
     originalImage, provinsiArea, nikArea, detailArea = prepareRecognitionArea(image_path)
 
     # Preprocessed Image
     provinsiAreaPreprocessed = preprocessRecognitionArea(provinsiArea)
     nikAreaPreprocessed = preprocessRecognitionArea(nikArea)
     detailAreaPreprocessed = preprocessRecognitionArea(detailArea)
```

### Comparing `pisahkan_ktp-0.0.3/PKG-INFO` & `pisahkan_ktp-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pisahkan-ktp
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package for detecting entities in text based on a dictionary and fuzzy similarity
 Author: Hanif Yuli Abdillah P
 Author-email: hanifabd23@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,16 @@
 Requires-Dist: opencv-contrib-python (==4.9.0.80)
 Requires-Dist: opencv-python (==4.8.0.76)
 Requires-Dist: pythonRLSA (==1.0.0)
 Description-Content-Type: text/markdown
 
 # **PISAHKAN KTP: Indonesian ID Card (KTP) Information Segmentation**
 
-![Image](./assets/OIG1.jpg)
+<center><img src="./assets/OIG1.jpg" alt="Beautiful Landscape" width="250"></center>
+
 
 ## **About**
 `pisahkan_ktp` is a Python function that extracts province, NIK, and personal information from an image of an Indonesian National Identity Card (KTP). It utilizes image processing techniques to locate and isolate relevant sections of the KTP image, then extracts text data accurately. The extracted information is returned in a structured format, facilitating further processing or integration into other applications.
 
 ## **Requirements**
 - Python 3.7 or Higher
 - numpy
```

