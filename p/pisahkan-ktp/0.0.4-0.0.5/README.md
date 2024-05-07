# Comparing `tmp/pisahkan_ktp-0.0.4.tar.gz` & `tmp/pisahkan_ktp-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pisahkan_ktp-0.0.4.tar", max compression
+gzip compressed data, was "pisahkan_ktp-0.0.5.tar", max compression
```

## Comparing `pisahkan_ktp-0.0.4.tar` & `pisahkan_ktp-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1097 2024-05-07 03:55:25.046040 pisahkan_ktp-0.0.4/LICENSE
--rwxr-xr-x   0        0        0     2055 2024-05-07 07:12:10.276685 pisahkan_ktp-0.0.4/README.md
--rwxr-xr-x   0        0        0      690 2024-05-07 07:15:25.866253 pisahkan_ktp-0.0.4/pyproject.toml
--rwxr-xr-x   0        0        0        0 2024-05-07 03:58:19.125178 pisahkan_ktp-0.0.4/src/pisahkan_ktp/__init__.py
--rwxr-xr-x   0        0        0    10887 2024-05-07 07:15:08.105205 pisahkan_ktp-0.0.4/src/pisahkan_ktp/ktp_segmenter.py
--rw-r--r--   0        0        0     2799 1970-01-01 00:00:00.000000 pisahkan_ktp-0.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1097 2024-05-07 03:55:25.046040 pisahkan_ktp-0.0.5/LICENSE
+-rwxr-xr-x   0        0        0     2055 2024-05-07 07:12:10.276685 pisahkan_ktp-0.0.5/README.md
+-rwxr-xr-x   0        0        0      690 2024-05-07 07:22:38.653729 pisahkan_ktp-0.0.5/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2024-05-07 03:58:19.125178 pisahkan_ktp-0.0.5/src/pisahkan_ktp/__init__.py
+-rwxr-xr-x   0        0        0    11293 2024-05-07 07:21:41.805011 pisahkan_ktp-0.0.5/src/pisahkan_ktp/ktp_segmenter.py
+-rw-r--r--   0        0        0     2799 1970-01-01 00:00:00.000000 pisahkan_ktp-0.0.5/PKG-INFO
```

### Comparing `pisahkan_ktp-0.0.4/LICENSE` & `pisahkan_ktp-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pisahkan_ktp-0.0.4/README.md` & `pisahkan_ktp-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pisahkan_ktp-0.0.4/pyproject.toml` & `pisahkan_ktp-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pisahkan-ktp"
-version = "0.0.4"
+version = "0.0.5"
 authors = ["Hanif Yuli Abdillah P <hanifabd23@gmail.com>"]
 description = "Python package for detecting entities in text based on a dictionary and fuzzy similarity"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `pisahkan_ktp-0.0.4/src/pisahkan_ktp/ktp_segmenter.py` & `pisahkan_ktp-0.0.5/src/pisahkan_ktp/ktp_segmenter.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,49 +236,51 @@
 def segmenter(image_path):
     '''
      This function identifies and isolates sections of Indonesian identity cards from images. 
      By detecting text and photo areas, it creates boundaries for province, nik, and personal information.
     '''
     assert isinstance(image_path, str), "Tokens can be str() type only"
 
-    if not os.path.exists(image_path):
-        return "Image File not Exists!"
-        
-    # Original Image
-    originalImage, provinsiArea, nikArea, detailArea = prepareRecognitionArea(image_path)
-
-    # Preprocessed Image
-    provinsiAreaPreprocessed = preprocessRecognitionArea(provinsiArea)
-    nikAreaPreprocessed = preprocessRecognitionArea(nikArea)
-    detailAreaPreprocessed = preprocessRecognitionArea(detailArea)
-
-    # Pattern Image
-    provinsiAreaPattern = findTextPattern(provinsiAreaPreprocessed, "provinsi")
-    nikAreaPattern = findTextPattern(nikAreaPreprocessed, "nik")
-    detailAreaPattern = findTextPattern(detailAreaPreprocessed, "detail")
-
-    # Draw bounding boxes on the original image
-    segmented_provinsi = []
-    boundingBoxesRowsProvinsi = provinsiCreateBoudingBox(provinsiAreaPattern, 450)
-    for bbox in boundingBoxesRowsProvinsi:
-        x1, y1, x2, y2 = bbox
-        segmented_provinsi.append(provinsiArea[y1:y2, x1:x2])
-
-    segmented_nik = []
-    boundingBoxesRowsNIK = nikCreateBoudingBox(nikAreaPattern, 450)
-    for bbox in boundingBoxesRowsNIK:
-        x1, y1, x2, y2 = bbox
-        segmented_nik.append(nikArea[y1:y2, x1:x2])
-
-    segmented_detail = []
-    boundingBoxesRowsDetail = detailCreateBoudingBox(detailAreaPattern, 450)
-    for bbox in boundingBoxesRowsDetail:
-        x1, y1, x2, y2 = bbox
-        segmented_detail.append(detailArea[y1:y2, x1:x2])
-
-    return {
-        "image": [originalImage],
-        "provinsiArea": segmented_provinsi,
-        "nikArea": segmented_nik,
-        "detailArea": segmented_detail,
-    }
-        
+    try:
+        # Attempt to open the file in read mode
+        with open(image_path, "r"):
+            # Original Image
+            originalImage, provinsiArea, nikArea, detailArea = prepareRecognitionArea(image_path)
+
+            # Preprocessed Image
+            provinsiAreaPreprocessed = preprocessRecognitionArea(provinsiArea)
+            nikAreaPreprocessed = preprocessRecognitionArea(nikArea)
+            detailAreaPreprocessed = preprocessRecognitionArea(detailArea)
+
+            # Pattern Image
+            provinsiAreaPattern = findTextPattern(provinsiAreaPreprocessed, "provinsi")
+            nikAreaPattern = findTextPattern(nikAreaPreprocessed, "nik")
+            detailAreaPattern = findTextPattern(detailAreaPreprocessed, "detail")
+
+            # Draw bounding boxes on the original image
+            segmented_provinsi = []
+            boundingBoxesRowsProvinsi = provinsiCreateBoudingBox(provinsiAreaPattern, 450)
+            for bbox in boundingBoxesRowsProvinsi:
+                x1, y1, x2, y2 = bbox
+                segmented_provinsi.append(provinsiArea[y1:y2, x1:x2])
+
+            segmented_nik = []
+            boundingBoxesRowsNIK = nikCreateBoudingBox(nikAreaPattern, 450)
+            for bbox in boundingBoxesRowsNIK:
+                x1, y1, x2, y2 = bbox
+                segmented_nik.append(nikArea[y1:y2, x1:x2])
+
+            segmented_detail = []
+            boundingBoxesRowsDetail = detailCreateBoudingBox(detailAreaPattern, 450)
+            for bbox in boundingBoxesRowsDetail:
+                x1, y1, x2, y2 = bbox
+                segmented_detail.append(detailArea[y1:y2, x1:x2])
+
+            return {
+                "image": [originalImage],
+                "provinsiArea": segmented_provinsi,
+                "nikArea": segmented_nik,
+                "detailArea": segmented_detail,
+            }
+    except FileNotFoundError:
+        # If the file does not exist, FileNotFoundError is raised
+        raise FileNotFoundError("File does not exist.")
```

### Comparing `pisahkan_ktp-0.0.4/PKG-INFO` & `pisahkan_ktp-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pisahkan-ktp
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python package for detecting entities in text based on a dictionary and fuzzy similarity
 Author: Hanif Yuli Abdillah P
 Author-email: hanifabd23@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

