# Comparing `tmp/danila-lib-1.3.9.tar.gz` & `tmp/danila-lib-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danila-lib-1.3.9.tar", last modified: Tue Apr 23 11:47:14 2024, max compression
+gzip compressed data, was "danila-lib-1.4.0.tar", last modified: Tue May  7 07:32:33 2024, max compression
```

## Comparing `danila-lib-1.3.9.tar` & `danila-lib-1.4.0.tar`

### file list

```diff
@@ -1,32 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 11:47:14.901836 danila-lib-1.3.9/
--rw-rw-rw-   0        0        0     9615 2024-04-23 11:47:14.901836 danila-lib-1.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.3.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 11:47:14.868983 danila-lib-1.3.9/danila/
--rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.3.9/danila/__init__.py
--rw-rw-rw-   0        0        0     9738 2024-04-22 21:01:41.000000 danila-lib-1.3.9/danila/danila.py
-drwxrwxrwx   0        0        0        0 2024-04-23 11:47:14.890885 danila-lib-1.3.9/danila_lib.egg-info/
--rw-rw-rw-   0        0        0     9615 2024-04-23 11:47:14.000000 danila-lib-1.3.9/danila_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      632 2024-04-23 11:47:14.000000 danila-lib-1.3.9/danila_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 11:47:14.000000 danila-lib-1.3.9/danila_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1879 2024-04-23 11:47:14.000000 danila-lib-1.3.9/danila_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-23 11:47:14.000000 danila-lib-1.3.9/danila_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-23 11:47:14.891881 danila-lib-1.3.9/data/
--rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.3.9/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 11:47:14.895863 danila-lib-1.3.9/data/neuro/
--rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.3.9/data/neuro/Letters_recognize.py
--rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.3.9/data/neuro/Rama_classify_class.py
--rw-rw-rw-   0        0        0     2121 2024-04-22 11:59:10.000000 danila-lib-1.3.9/data/neuro/Rama_detect_class.py
--rw-rw-rw-   0        0        0     3159 2024-04-22 19:35:07.000000 danila-lib-1.3.9/data/neuro/Text_detect_class.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.3.9/data/neuro/__init__.py
--rw-rw-rw-   0        0        0      675 2024-04-23 11:46:59.000000 danila-lib-1.3.9/data/neuro/models.py
-drwxrwxrwx   0        0        0        0 2024-04-23 11:47:14.900841 danila-lib-1.3.9/data/result/
--rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.3.9/data/result/Class_im.py
--rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.3.9/data/result/Class_text.py
--rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.3.9/data/result/Image_text_areas.py
--rw-rw-rw-   0        0        0      311 2024-04-22 18:52:56.000000 danila-lib-1.3.9/data/result/Label_area.py
--rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.3.9/data/result/Rect.py
--rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.3.9/data/result/Text_area.py
--rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.3.9/data/result/Yolo_label_rect.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.3.9/data/result/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-23 11:47:14.905818 danila-lib-1.3.9/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-04-23 11:47:13.000000 danila-lib-1.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:32:33.575207 danila-lib-1.4.0/
+-rw-rw-rw-   0        0        0     9615 2024-05-07 07:32:33.575207 danila-lib-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 07:32:33.497104 danila-lib-1.4.0/danila/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.4.0/danila/__init__.py
+-rw-rw-rw-   0        0        0     1777 2024-05-06 15:05:03.000000 danila-lib-1.4.0/danila/danila.py
+-rw-rw-rw-   0        0        0     9741 2024-05-06 15:01:57.000000 danila-lib-1.4.0/danila/danila_v1.py
+-rw-rw-rw-   0        0        0    10159 2024-05-07 07:31:38.000000 danila-lib-1.4.0/danila/danila_v2.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:32:33.512727 danila-lib-1.4.0/danila_lib.egg-info/
+-rw-rw-rw-   0        0        0     9615 2024-05-07 07:32:33.000000 danila-lib-1.4.0/danila_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      772 2024-05-07 07:32:33.000000 danila-lib-1.4.0/danila_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 07:32:33.000000 danila-lib-1.4.0/danila_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1879 2024-05-07 07:32:33.000000 danila-lib-1.4.0/danila_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-07 07:32:33.000000 danila-lib-1.4.0/danila_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 07:32:33.512727 danila-lib-1.4.0/data/
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.4.0/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:32:33.543973 danila-lib-1.4.0/data/neuro/
+-rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.4.0/data/neuro/Letters_recognize.py
+-rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.4.0/data/neuro/Rama_classify_class.py
+-rw-rw-rw-   0        0        0     2121 2024-04-22 11:59:10.000000 danila-lib-1.4.0/data/neuro/Rama_detect_class.py
+-rw-rw-rw-   0        0        0     3159 2024-04-22 19:35:07.000000 danila-lib-1.4.0/data/neuro/Text_detect_class.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.4.0/data/neuro/__init__.py
+-rw-rw-rw-   0        0        0     6373 2024-05-06 15:05:03.000000 danila-lib-1.4.0/data/neuro/letters_in_image.py
+-rw-rw-rw-   0        0        0      752 2024-05-07 03:18:59.000000 danila-lib-1.4.0/data/neuro/models.py
+-rw-rw-rw-   0        0        0     4340 2024-05-07 07:23:47.000000 danila-lib-1.4.0/data/neuro/text_recognize_yolo.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:32:33.575207 danila-lib-1.4.0/data/result/
+-rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.4.0/data/result/Class_im.py
+-rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.4.0/data/result/Class_text.py
+-rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.4.0/data/result/Image_text_areas.py
+-rw-rw-rw-   0        0        0      311 2024-04-22 18:52:56.000000 danila-lib-1.4.0/data/result/Label_area.py
+-rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.4.0/data/result/Rect.py
+-rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.4.0/data/result/Text_area.py
+-rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.4.0/data/result/Yolo_label_rect.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.4.0/data/result/__init__.py
+-rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.4.0/data/result/word_compare_result.py
+-rw-rw-rw-   0        0        0       42 2024-05-07 07:32:33.590827 danila-lib-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-05-07 07:31:38.000000 danila-lib-1.4.0/setup.py
```

### Comparing `danila-lib-1.3.9/PKG-INFO` & `danila-lib-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.3.9
+Version: 1.4.0
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.3.9/README.md` & `danila-lib-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `danila-lib-1.3.9/danila/danila.py` & `danila-lib-1.4.0/danila/danila_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from data.result.Class_text import Class_text
 from data.result.Rect import Rect
 
 """main module for user"""
 from data.neuro.Rama_classify_class import Rama_classify_class
 
 
-class Danila:
+class Danila_v1:
     """main class for user"""
     def __init__(self, yolov5_dir):
 
         self.rama_classify_model = Rama_classify_class()
         yolo_path = yolov5_dir
         rama_no_spring_detect_model_path = RAMA_NO_SPRING_DETECT_MODEL_ADDRESS
         self.rama_no_spring_detect_model = Rama_detect_class(rama_no_spring_detect_model_path,
```

### Comparing `danila-lib-1.3.9/danila_lib.egg-info/PKG-INFO` & `danila-lib-1.4.0/danila_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.3.9
+Version: 1.4.0
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.3.9/danila_lib.egg-info/SOURCES.txt` & `danila-lib-1.4.0/danila_lib.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 README.md
 setup.cfg
 setup.py
 danila/__init__.py
 danila/danila.py
+danila/danila_v1.py
+danila/danila_v2.py
 danila_lib.egg-info/PKG-INFO
 danila_lib.egg-info/SOURCES.txt
 danila_lib.egg-info/dependency_links.txt
 danila_lib.egg-info/requires.txt
 danila_lib.egg-info/top_level.txt
 data/__init__.py
 data/neuro/Letters_recognize.py
 data/neuro/Rama_classify_class.py
 data/neuro/Rama_detect_class.py
 data/neuro/Text_detect_class.py
 data/neuro/__init__.py
+data/neuro/letters_in_image.py
 data/neuro/models.py
+data/neuro/text_recognize_yolo.py
 data/result/Class_im.py
 data/result/Class_text.py
 data/result/Image_text_areas.py
 data/result/Label_area.py
 data/result/Rect.py
 data/result/Text_area.py
 data/result/Yolo_label_rect.py
-data/result/__init__.py
+data/result/__init__.py
+data/result/word_compare_result.py
```

### Comparing `danila-lib-1.3.9/danila_lib.egg-info/requires.txt` & `danila-lib-1.4.0/danila_lib.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.3.9/data/neuro/Letters_recognize.py` & `danila-lib-1.4.0/data/neuro/Letters_recognize.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.3.9/data/neuro/Rama_classify_class.py` & `danila-lib-1.4.0/data/neuro/Rama_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.3.9/data/neuro/Rama_detect_class.py` & `danila-lib-1.4.0/data/neuro/Rama_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.3.9/data/neuro/Text_detect_class.py` & `danila-lib-1.4.0/data/neuro/Text_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.3.9/data/neuro/models.py` & `danila-lib-1.4.0/data/neuro/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,7 +2,8 @@
 RAMA_NO_SPRING_DETECT_MODEL_ADDRESS = 'https://disk.yandex.ru/d/sE5iSXYWL3xEkQ'
 RAMA_SPRING_DETECT_MODEL_ADDRESS = 'https://disk.yandex.ru/d/zAEw0_ALgtBg9Q'
 RAMA_SPRING_RUZHIMMASH_TEXT_DETECT_MODEL_ADDRESS = 'https://disk.yandex.ru/d/b4vCbEzg3t3mTg'
 RAMA_NO_SPRING_BEJICKAYA_TEXT_DETECT_MODEL_ADDRESS = 'https://disk.yandex.ru/d/ZbbcscTS2Han1A'
 LETTERS_RECOGNIZE = 'https://disk.yandex.ru/d/ooaMrpqxl_egoA'
 RAMA_NO_SPRING_RUZHIMMASH_TEXT_DETECT_MODEL_ADDRESS = 'https://disk.yandex.ru/d/b4vCbEzg3t3mTg'
 RAMA_SPRING_BEJICKAYA_TEXT_DETECT_MODEL_ADDRESS = 'https://disk.yandex.ru/d/ZbbcscTS2Han1A'
+TEXT_RECOGNIZE_YOLO_MODEL_ADDRESS = 'https://disk.yandex.ru/d/HN5Cs2zffXipIg'
```

### Comparing `danila-lib-1.3.9/data/result/Image_text_areas.py` & `danila-lib-1.4.0/data/result/Image_text_areas.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.3.9/data/result/Rect.py` & `danila-lib-1.4.0/data/result/Rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.3.9/data/result/Text_area.py` & `danila-lib-1.4.0/data/result/Text_area.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.3.9/data/result/Yolo_label_rect.py` & `danila-lib-1.4.0/data/result/Yolo_label_rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.3.9/setup.py` & `danila-lib-1.4.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   with open('requirements.txt', 'r') as f:
     a = f.read()
   b = a.split()
   return b
 
 setup(
   name='danila-lib',
-  version='1.3.9',
+  version='1.4.0',
   author='arseniy_zhuck',
   author_email='arseniyzhuck@mail.ru',
   description='This is the module for detecting and classifying text on rama pictures',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Arseniy-Zhuck/danila_lib',
   packages=find_packages(),
```

