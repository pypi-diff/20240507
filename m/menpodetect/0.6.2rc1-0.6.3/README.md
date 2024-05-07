# Comparing `tmp/menpodetect-0.6.2rc1.tar.gz` & `tmp/menpodetect-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "menpodetect-0.6.2rc1.tar", last modified: Sat Jan  9 18:49:21 2021, max compression
+gzip compressed data, was "menpodetect-0.6.3.tar", last modified: Tue May  7 08:14:54 2024, max compression
```

## Comparing `menpodetect-0.6.2rc1.tar` & `menpodetect-0.6.3.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-09 18:49:21.391583 menpodetect-0.6.2rc1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1643 2021-01-09 18:45:56.000000 menpodetect-0.6.2rc1/LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       74 2021-01-09 18:45:56.000000 menpodetect-0.6.2rc1/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)      247 2021-01-09 18:49:21.391583 menpodetect-0.6.2rc1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3027 2021-01-09 18:45:56.000000 menpodetect-0.6.2rc1/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-09 18:49:21.391583 menpodetect-0.6.2rc1/menpodetect/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      158 2021-01-09 18:45:56.000000 menpodetect-0.6.2rc1/menpodetect/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      474 2021-01-09 18:49:21.391583 menpodetect-0.6.2rc1/menpodetect/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4732 2021-01-09 18:45:56.000000 menpodetect-0.6.2rc1/menpodetect/detect.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-09 18:49:21.383583 menpodetect-0.6.2rc1/menpodetect/dlib/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      269 2021-01-09 18:45:56.000000 menpodetect-0.6.2rc1/menpodetect/dlib/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1073 2021-01-09 18:45:56.000000 menpodetect-0.6.2rc1/menpodetect/dlib/conversion.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4741 2021-01-09 18:45:56.000000 menpodetect-0.6.2rc1/menpodetect/dlib/detect.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3341 2021-01-09 18:45:56.000000 menpodetect-0.6.2rc1/menpodetect/dlib/train.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-09 18:49:21.375583 menpodetect-0.6.2rc1/menpodetect/models/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-09 18:49:21.387583 menpodetect-0.6.2rc1/menpodetect/models/opencv/
--rw-r--r--   0 circleci  (3434) circleci  (3434)   341406 2021-01-09 18:45:56.000000 menpodetect-0.6.2rc1/menpodetect/models/opencv/haarcascade_eye.xml
--rw-r--r--   0 circleci  (3434) circleci  (3434)   676709 2021-01-09 18:45:56.000000 menpodetect-0.6.2rc1/menpodetect/models/opencv/haarcascade_frontalface_alt.xml
--rw-r--r--   0 circleci  (3434) circleci  (3434)   828514 2021-01-09 18:45:56.000000 menpodetect-0.6.2rc1/menpodetect/models/opencv/haarcascade_profileface.xml
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-09 18:49:21.391583 menpodetect-0.6.2rc1/menpodetect/opencv/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      332 2021-01-09 18:45:56.000000 menpodetect-0.6.2rc1/menpodetect/opencv/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      949 2021-01-09 18:45:56.000000 menpodetect-0.6.2rc1/menpodetect/opencv/conversion.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6267 2021-01-09 18:45:56.000000 menpodetect-0.6.2rc1/menpodetect/opencv/detect.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      594 2021-01-09 18:45:56.000000 menpodetect-0.6.2rc1/menpodetect/paths.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-09 18:49:21.391583 menpodetect-0.6.2rc1/menpodetect/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2021-01-09 18:45:56.000000 menpodetect-0.6.2rc1/menpodetect/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3127 2021-01-09 18:45:56.000000 menpodetect-0.6.2rc1/menpodetect/tests/test_detector.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1037 2021-01-09 18:45:56.000000 menpodetect-0.6.2rc1/menpodetect/tests/test_dlib.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1172 2021-01-09 18:45:56.000000 menpodetect-0.6.2rc1/menpodetect/tests/test_opencv.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-09 18:49:21.383583 menpodetect-0.6.2rc1/menpodetect.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      247 2021-01-09 18:49:21.000000 menpodetect-0.6.2rc1/menpodetect.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      824 2021-01-09 18:49:21.000000 menpodetect-0.6.2rc1/menpodetect.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-01-09 18:49:21.000000 menpodetect-0.6.2rc1/menpodetect.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2021-01-09 18:49:21.000000 menpodetect-0.6.2rc1/menpodetect.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2021-01-09 18:49:21.000000 menpodetect-0.6.2rc1/menpodetect.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      213 2021-01-09 18:49:21.391583 menpodetect-0.6.2rc1/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      506 2021-01-09 18:45:56.000000 menpodetect-0.6.2rc1/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    62474 2021-01-09 18:45:56.000000 menpodetect-0.6.2rc1/versioneer.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 08:14:54.030961 menpodetect-0.6.3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      483 2024-05-07 08:12:41.000000 menpodetect-0.6.3/AUTHORS.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1643 2024-05-07 08:12:41.000000 menpodetect-0.6.3/LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       39 2024-05-07 08:12:41.000000 menpodetect-0.6.3/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      251 2024-05-07 08:14:54.030961 menpodetect-0.6.3/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3027 2024-05-07 08:12:41.000000 menpodetect-0.6.3/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 08:14:54.030961 menpodetect-0.6.3/menpodetect/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       99 2024-05-07 08:12:41.000000 menpodetect-0.6.3/menpodetect/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2024-05-07 08:14:54.030961 menpodetect-0.6.3/menpodetect/_static_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6088 2024-05-07 08:12:41.000000 menpodetect-0.6.3/menpodetect/_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4732 2024-05-07 08:12:41.000000 menpodetect-0.6.3/menpodetect/detect.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 08:14:54.026961 menpodetect-0.6.3/menpodetect/dlib/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      269 2024-05-07 08:12:41.000000 menpodetect-0.6.3/menpodetect/dlib/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1073 2024-05-07 08:12:41.000000 menpodetect-0.6.3/menpodetect/dlib/conversion.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4741 2024-05-07 08:12:41.000000 menpodetect-0.6.3/menpodetect/dlib/detect.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3341 2024-05-07 08:12:41.000000 menpodetect-0.6.3/menpodetect/dlib/train.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 08:14:54.022961 menpodetect-0.6.3/menpodetect/models/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 08:14:54.026961 menpodetect-0.6.3/menpodetect/models/opencv/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   341406 2024-05-07 08:12:41.000000 menpodetect-0.6.3/menpodetect/models/opencv/haarcascade_eye.xml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   676709 2024-05-07 08:12:41.000000 menpodetect-0.6.3/menpodetect/models/opencv/haarcascade_frontalface_alt.xml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   828514 2024-05-07 08:12:41.000000 menpodetect-0.6.3/menpodetect/models/opencv/haarcascade_profileface.xml
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 08:14:54.030961 menpodetect-0.6.3/menpodetect/opencv/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      332 2024-05-07 08:12:41.000000 menpodetect-0.6.3/menpodetect/opencv/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      949 2024-05-07 08:12:41.000000 menpodetect-0.6.3/menpodetect/opencv/conversion.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6267 2024-05-07 08:12:41.000000 menpodetect-0.6.3/menpodetect/opencv/detect.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      594 2024-05-07 08:12:41.000000 menpodetect-0.6.3/menpodetect/paths.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 08:14:54.030961 menpodetect-0.6.3/menpodetect/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2024-05-07 08:12:41.000000 menpodetect-0.6.3/menpodetect/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      549 2024-05-07 08:12:41.000000 menpodetect-0.6.3/menpodetect/tests/test_black.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3127 2024-05-07 08:12:41.000000 menpodetect-0.6.3/menpodetect/tests/test_detector.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1037 2024-05-07 08:12:41.000000 menpodetect-0.6.3/menpodetect/tests/test_dlib.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1172 2024-05-07 08:12:41.000000 menpodetect-0.6.3/menpodetect/tests/test_opencv.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 08:14:54.030961 menpodetect-0.6.3/menpodetect.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      251 2024-05-07 08:14:54.000000 menpodetect-0.6.3/menpodetect.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      875 2024-05-07 08:14:54.000000 menpodetect-0.6.3/menpodetect.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-05-07 08:14:54.000000 menpodetect-0.6.3/menpodetect.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2024-05-07 08:14:54.000000 menpodetect-0.6.3/menpodetect.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2024-05-07 08:14:54.000000 menpodetect-0.6.3/menpodetect.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2024-05-07 08:14:54.030961 menpodetect-0.6.3/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      950 2024-05-07 08:12:41.000000 menpodetect-0.6.3/setup.py
```

### Comparing `menpodetect-0.6.2rc1/LICENSE.txt` & `menpodetect-0.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `menpodetect-0.6.2rc1/README.md` & `menpodetect-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `menpodetect-0.6.2rc1/menpodetect/detect.py` & `menpodetect-0.6.3/menpodetect/detect.py`

 * *Files identical despite different names*

### Comparing `menpodetect-0.6.2rc1/menpodetect/dlib/conversion.py` & `menpodetect-0.6.3/menpodetect/dlib/conversion.py`

 * *Files identical despite different names*

### Comparing `menpodetect-0.6.2rc1/menpodetect/dlib/detect.py` & `menpodetect-0.6.3/menpodetect/dlib/detect.py`

 * *Files identical despite different names*

### Comparing `menpodetect-0.6.2rc1/menpodetect/dlib/train.py` & `menpodetect-0.6.3/menpodetect/dlib/train.py`

 * *Files identical despite different names*

### Comparing `menpodetect-0.6.2rc1/menpodetect/models/opencv/haarcascade_eye.xml` & `menpodetect-0.6.3/menpodetect/models/opencv/haarcascade_eye.xml`

 * *Files identical despite different names*

### Comparing `menpodetect-0.6.2rc1/menpodetect/models/opencv/haarcascade_frontalface_alt.xml` & `menpodetect-0.6.3/menpodetect/models/opencv/haarcascade_frontalface_alt.xml`

 * *Files identical despite different names*

### Comparing `menpodetect-0.6.2rc1/menpodetect/models/opencv/haarcascade_profileface.xml` & `menpodetect-0.6.3/menpodetect/models/opencv/haarcascade_profileface.xml`

 * *Files identical despite different names*

### Comparing `menpodetect-0.6.2rc1/menpodetect/opencv/conversion.py` & `menpodetect-0.6.3/menpodetect/opencv/conversion.py`

 * *Files identical despite different names*

### Comparing `menpodetect-0.6.2rc1/menpodetect/opencv/detect.py` & `menpodetect-0.6.3/menpodetect/opencv/detect.py`

 * *Files identical despite different names*

### Comparing `menpodetect-0.6.2rc1/menpodetect/paths.py` & `menpodetect-0.6.3/menpodetect/paths.py`

 * *Files identical despite different names*

### Comparing `menpodetect-0.6.2rc1/menpodetect/tests/test_detector.py` & `menpodetect-0.6.3/menpodetect/tests/test_detector.py`

 * *Files identical despite different names*

### Comparing `menpodetect-0.6.2rc1/menpodetect/tests/test_dlib.py` & `menpodetect-0.6.3/menpodetect/tests/test_dlib.py`

 * *Files identical despite different names*

### Comparing `menpodetect-0.6.2rc1/menpodetect/tests/test_opencv.py` & `menpodetect-0.6.3/menpodetect/tests/test_opencv.py`

 * *Files identical despite different names*

### Comparing `menpodetect-0.6.2rc1/menpodetect.egg-info/SOURCES.txt` & `menpodetect-0.6.3/menpodetect.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+AUTHORS.txt
 LICENSE.txt
 MANIFEST.in
 README.md
-setup.cfg
 setup.py
-versioneer.py
 menpodetect/__init__.py
+menpodetect/_static_version.py
 menpodetect/_version.py
 menpodetect/detect.py
 menpodetect/paths.py
 menpodetect.egg-info/PKG-INFO
 menpodetect.egg-info/SOURCES.txt
 menpodetect.egg-info/dependency_links.txt
 menpodetect.egg-info/requires.txt
@@ -20,10 +20,11 @@
 menpodetect/models/opencv/haarcascade_eye.xml
 menpodetect/models/opencv/haarcascade_frontalface_alt.xml
 menpodetect/models/opencv/haarcascade_profileface.xml
 menpodetect/opencv/__init__.py
 menpodetect/opencv/conversion.py
 menpodetect/opencv/detect.py
 menpodetect/tests/__init__.py
+menpodetect/tests/test_black.py
 menpodetect/tests/test_detector.py
 menpodetect/tests/test_dlib.py
 menpodetect/tests/test_opencv.py
```

