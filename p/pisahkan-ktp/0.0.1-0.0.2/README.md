# Comparing `tmp/pisahkan_ktp-0.0.1.tar.gz` & `tmp/pisahkan_ktp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pisahkan_ktp-0.0.1.tar", max compression
+gzip compressed data, was "pisahkan_ktp-0.0.2.tar", max compression
```

## Comparing `pisahkan_ktp-0.0.1.tar` & `pisahkan_ktp-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rwxr-xr-x   0        0        0     1097 2024-05-07 03:55:25.046040 pisahkan_ktp-0.0.1/LICENSE
--rwxr-xr-x   0        0        0     2993 2024-04-17 10:22:18.366558 pisahkan_ktp-0.0.1/README.md
--rwxr-xr-x   0        0        0      708 2024-05-07 04:31:47.803438 pisahkan_ktp-0.0.1/pyproject.toml
--rwxr-xr-x   0        0        0        0 2024-05-07 03:58:19.125178 pisahkan_ktp-0.0.1/src/pisahkan_ktp/__init__.py
--rwxr-xr-x   0        0        0     8922 2024-05-07 04:13:36.311779 pisahkan_ktp-0.0.1/src/pisahkan_ktp/ktp_helper.py
--rwxr-xr-x   0        0        0     2033 2024-05-07 04:50:22.158284 pisahkan_ktp-0.0.1/src/pisahkan_ktp/ktp_segmenter.py
--rw-r--r--   0        0        0     3763 1970-01-01 00:00:00.000000 pisahkan_ktp-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1097 2024-05-07 03:55:25.046040 pisahkan_ktp-0.0.2/LICENSE
+-rwxr-xr-x   0        0        0     1996 2024-05-07 06:53:15.180845 pisahkan_ktp-0.0.2/README.md
+-rwxr-xr-x   0        0        0      690 2024-05-07 06:59:22.709325 pisahkan_ktp-0.0.2/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2024-05-07 03:58:19.125178 pisahkan_ktp-0.0.2/src/pisahkan_ktp/__init__.py
+-rwxr-xr-x   0        0        0    10785 2024-05-07 06:57:16.481480 pisahkan_ktp-0.0.2/src/pisahkan_ktp/ktp_segmenter.py
+-rw-r--r--   0        0        0     2741 1970-01-01 00:00:00.000000 pisahkan_ktp-0.0.2/PKG-INFO
```

### Comparing `pisahkan_ktp-0.0.1/LICENSE` & `pisahkan_ktp-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pisahkan_ktp-0.0.1/pyproject.toml` & `pisahkan_ktp-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pisahkan-ktp"
-version = "0.0.1"
+version = "0.0.2"
 authors = ["Hanif Yuli Abdillah P <hanifabd23@gmail.com>"]
 description = "Python package for detecting entities in text based on a dictionary and fuzzy similarity"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7"
-numpy = "1.21.6"
 opencv-python = "4.8.0.76"
 opencv-contrib-python = "4.9.0.80"
 pythonRLSA = "1.0.0"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `pisahkan_ktp-0.0.1/src/pisahkan_ktp/ktp_helper.py` & `pisahkan_ktp-0.0.2/src/pisahkan_ktp/ktp_segmenter.py`

 * *Files 18% similar despite different names*

```diff
@@ -226,8 +226,55 @@
     for contour in contours:
         x, y, w, h = cv2.boundingRect(contour)
         if w * h >= min_area_threshold:
             bounding_boxes.append((0, max(y-12, 0), min(x+image.shape[1], int(image.shape[1])), y+h+12))
 
     bounding_boxes.sort(key=lambda bbox: (bbox[1], bbox[0]))
 
-    return bounding_boxes
+    return bounding_boxes
+
+def segmenter(image_path):
+    '''
+     This function identifies and isolates sections of Indonesian identity cards from images. 
+     By detecting text and photo areas, it creates boundaries for province, nik, and personal information.
+    '''
+    assert isinstance(image_path, str), "Tokens can be str() type only"
+
+    # Original Image
+    originalImage, provinsiArea, nikArea, detailArea = prepareRecognitionArea(image_path)
+
+    # Preprocessed Image
+    provinsiAreaPreprocessed = preprocessRecognitionArea(provinsiArea)
+    nikAreaPreprocessed = preprocessRecognitionArea(nikArea)
+    detailAreaPreprocessed = preprocessRecognitionArea(detailArea)
+
+    # Pattern Image
+    provinsiAreaPattern = findTextPattern(provinsiAreaPreprocessed, "provinsi")
+    nikAreaPattern = findTextPattern(nikAreaPreprocessed, "nik")
+    detailAreaPattern = findTextPattern(detailAreaPreprocessed, "detail")
+
+    # Draw bounding boxes on the original image
+    segmented_provinsi = []
+    boundingBoxesRowsProvinsi = provinsiCreateBoudingBox(provinsiAreaPattern, 450)
+    for bbox in boundingBoxesRowsProvinsi:
+        x1, y1, x2, y2 = bbox
+        segmented_provinsi.append(provinsiArea[y1:y2, x1:x2])
+
+    segmented_nik = []
+    boundingBoxesRowsNIK = nikCreateBoudingBox(nikAreaPattern, 450)
+    for bbox in boundingBoxesRowsNIK:
+        x1, y1, x2, y2 = bbox
+        segmented_nik.append(nikArea[y1:y2, x1:x2])
+
+    segmented_detail = []
+    boundingBoxesRowsDetail = detailCreateBoudingBox(detailAreaPattern, 450)
+    for bbox in boundingBoxesRowsDetail:
+        x1, y1, x2, y2 = bbox
+        segmented_detail.append(detailArea[y1:y2, x1:x2])
+
+    return {
+        "image": [originalImage],
+        "provinsiArea": segmented_provinsi,
+        "nikArea": segmented_nik,
+        "detailArea": segmented_detail,
+    }
+
```

