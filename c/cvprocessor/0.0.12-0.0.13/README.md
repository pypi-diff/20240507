# Comparing `tmp/cvprocessor-0.0.12.tar.gz` & `tmp/cvprocessor-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvprocessor-0.0.12.tar", last modified: Mon May  6 08:10:50 2024, max compression
+gzip compressed data, was "cvprocessor-0.0.13.tar", last modified: Mon May  6 10:05:12 2024, max compression
```

## Comparing `cvprocessor-0.0.12.tar` & `cvprocessor-0.0.13.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-06 08:10:50.687923 cvprocessor-0.0.12/
--rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.0.12/LICENSE
--rw-r--r--   0 fernando   (501) staff       (20)     1690 2024-05-06 08:10:50.687194 cvprocessor-0.0.12/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)     1042 2024-05-05 07:13:28.000000 cvprocessor-0.0.12/README.md
--rw-r--r--   0 fernando   (501) staff       (20)      770 2024-05-06 08:10:34.000000 cvprocessor-0.0.12/pyproject.toml
--rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-06 08:10:50.688049 cvprocessor-0.0.12/setup.cfg
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-06 08:10:50.677498 cvprocessor-0.0.12/src/
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-06 08:10:50.684035 cvprocessor-0.0.12/src/cvprocessor/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.0.12/src/cvprocessor/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)     5851 2024-05-04 22:18:45.000000 cvprocessor-0.0.12/src/cvprocessor/authors.py
--rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.0.12/src/cvprocessor/common.py
--rw-r--r--   0 fernando   (501) staff       (20)     2106 2024-05-06 08:04:06.000000 cvprocessor-0.0.12/src/cvprocessor/cv.py
--rw-r--r--   0 fernando   (501) staff       (20)     3514 2024-05-04 09:03:16.000000 cvprocessor-0.0.12/src/cvprocessor/education.py
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-04 07:19:43.000000 cvprocessor-0.0.12/src/cvprocessor/experience.py
--rw-r--r--   0 fernando   (501) staff       (20)     2245 2024-05-06 01:06:42.000000 cvprocessor-0.0.12/src/cvprocessor/institutes.py
--rw-r--r--   0 fernando   (501) staff       (20)     1396 2024-05-04 09:02:35.000000 cvprocessor-0.0.12/src/cvprocessor/intro.py
--rw-r--r--   0 fernando   (501) staff       (20)     2088 2024-05-05 08:39:17.000000 cvprocessor-0.0.12/src/cvprocessor/news.py
--rw-r--r--   0 fernando   (501) staff       (20)     9424 2024-05-06 08:04:12.000000 cvprocessor-0.0.12/src/cvprocessor/publications.py
--rw-r--r--   0 fernando   (501) staff       (20)     1050 2024-05-05 10:18:42.000000 cvprocessor-0.0.12/src/cvprocessor/research_interests.py
--rw-r--r--   0 fernando   (501) staff       (20)     2967 2024-05-06 05:39:04.000000 cvprocessor-0.0.12/src/cvprocessor/software.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-06 08:10:50.686540 cvprocessor-0.0.12/src/cvprocessor.egg-info/
--rw-r--r--   0 fernando   (501) staff       (20)     1690 2024-05-06 08:10:50.000000 cvprocessor-0.0.12/src/cvprocessor.egg-info/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      565 2024-05-06 08:10:50.000000 cvprocessor-0.0.12/src/cvprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-06 08:10:50.000000 cvprocessor-0.0.12/src/cvprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-06 08:10:50.000000 cvprocessor-0.0.12/src/cvprocessor.egg-info/requires.txt
--rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-06 08:10:50.000000 cvprocessor-0.0.12/src/cvprocessor.egg-info/top_level.txt
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-06 10:05:12.846043 cvprocessor-0.0.13/
+-rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.0.13/LICENSE
+-rw-r--r--   0 fernando   (501) staff       (20)     1690 2024-05-06 10:05:12.845450 cvprocessor-0.0.13/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)     1042 2024-05-05 07:13:28.000000 cvprocessor-0.0.13/README.md
+-rw-r--r--   0 fernando   (501) staff       (20)      770 2024-05-06 10:04:41.000000 cvprocessor-0.0.13/pyproject.toml
+-rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-06 10:05:12.846314 cvprocessor-0.0.13/setup.cfg
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-06 10:05:12.830892 cvprocessor-0.0.13/src/
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-06 10:05:12.841378 cvprocessor-0.0.13/src/cvprocessor/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.0.13/src/cvprocessor/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5851 2024-05-04 22:18:45.000000 cvprocessor-0.0.13/src/cvprocessor/authors.py
+-rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.0.13/src/cvprocessor/common.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2106 2024-05-06 08:04:06.000000 cvprocessor-0.0.13/src/cvprocessor/cv.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3514 2024-05-04 09:03:16.000000 cvprocessor-0.0.13/src/cvprocessor/education.py
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-04 07:19:43.000000 cvprocessor-0.0.13/src/cvprocessor/experience.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3340 2024-05-06 10:02:34.000000 cvprocessor-0.0.13/src/cvprocessor/institutes.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1396 2024-05-04 09:02:35.000000 cvprocessor-0.0.13/src/cvprocessor/intro.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2088 2024-05-05 08:39:17.000000 cvprocessor-0.0.13/src/cvprocessor/news.py
+-rw-r--r--   0 fernando   (501) staff       (20)     9424 2024-05-06 08:04:12.000000 cvprocessor-0.0.13/src/cvprocessor/publications.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1050 2024-05-05 10:18:42.000000 cvprocessor-0.0.13/src/cvprocessor/research_interests.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2967 2024-05-06 05:39:04.000000 cvprocessor-0.0.13/src/cvprocessor/software.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-06 10:05:12.844869 cvprocessor-0.0.13/src/cvprocessor.egg-info/
+-rw-r--r--   0 fernando   (501) staff       (20)     1690 2024-05-06 10:05:12.000000 cvprocessor-0.0.13/src/cvprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      565 2024-05-06 10:05:12.000000 cvprocessor-0.0.13/src/cvprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-06 10:05:12.000000 cvprocessor-0.0.13/src/cvprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-06 10:05:12.000000 cvprocessor-0.0.13/src/cvprocessor.egg-info/requires.txt
+-rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-06 10:05:12.000000 cvprocessor-0.0.13/src/cvprocessor.egg-info/top_level.txt
```

### Comparing `cvprocessor-0.0.12/LICENSE` & `cvprocessor-0.0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.12/PKG-INFO` & `cvprocessor-0.0.13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.0.12
+Version: 0.0.13
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.0.12/README.md` & `cvprocessor-0.0.13/README.md`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.12/pyproject.toml` & `cvprocessor-0.0.13/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cvprocessor"
-version = "0.0.12"
+version = "0.0.13"
 authors = [
     { name = "F. Fernando Jurado-Lasso", email = "fdo.jurado@gmail.com" },
 ]
 description = "CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cvprocessor-0.0.12/src/cvprocessor/authors.py` & `cvprocessor-0.0.13/src/cvprocessor/authors.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.12/src/cvprocessor/cv.py` & `cvprocessor-0.0.13/src/cvprocessor/cv.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.12/src/cvprocessor/education.py` & `cvprocessor-0.0.13/src/cvprocessor/education.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.12/src/cvprocessor/institutes.py` & `cvprocessor-0.0.13/src/cvprocessor/institutes.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     def __init__(self, pd_dataframe):
         self._pd_dataframe = pd_dataframe
         self._id = None
         self._name = None
         self._address = None
         self._city = None
         self._country = None
+        self._coordinates = None
         self._url = None
         self._load_institute()
 
     @property
     def name(self):
         return self._name
 
@@ -33,32 +34,58 @@
         return self._city
 
     @property
     def country(self):
         return self._country
 
     @property
+    def coordinates(self):
+        return self._coordinates
+
+    @property
     def url(self):
         return self._url
 
+    def convert_coordinates(self, lalng):
+        lalng = lalng.replace("°", "").strip()
+        if "S" in lalng or "W" in lalng:
+            lalng = lalng.replace("S", "").replace("W", "")
+            lalng = "-" + lalng
+        else:
+            lalng = lalng.replace("N", "").replace("E", "")
+        return float(lalng)
+
+    def process_coordinates(self):
+        # Coordinates can be of the form 37.7983° S, 144.9610° E or 3.342119819025848, -76.5306449189542
+        # We will convert them to the form 37.7983, 144.9610
+        if self._coordinates is not None:
+            # split into latitude and longitude
+            coordinates = self._coordinates.split(", ")
+            coordinates = [self.convert_coordinates(
+                coord) for coord in coordinates]
+            self._coordinates = tuple(coordinates)
+
     def _load_institute(self):
         self._id = self._pd_dataframe["id"]
         self._name = self._pd_dataframe["Name"]
         self._address = self._pd_dataframe["Address"]
         self._city = self._pd_dataframe["City"]
         self._country = self._pd_dataframe["Country"]
         self._url = self._pd_dataframe["URL"]
+        self._coordinates = self._pd_dataframe["Coordinates"]
+        self.process_coordinates()
 
     def print(self):
         print(f"Institute ID: {self._id}")
         print(f"Institute Name: {self._name}")
         print(f"Institute Address: {self._address}")
         print(f"Institute City: {self._city}")
         print(f"Institute Country: {self._country}")
         print(f"Institute URL: {self._url}")
+        print(f"Institute Coordinates: {self._coordinates}")
         print("\n")
 
 
 class Institutes:
     def __init__(self, filename):
         self._filename = filename
         self._institute = self._load_institutes()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cvprocessor-0.0.12/src/cvprocessor/intro.py` & `cvprocessor-0.0.13/src/cvprocessor/intro.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.12/src/cvprocessor/news.py` & `cvprocessor-0.0.13/src/cvprocessor/news.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.12/src/cvprocessor/publications.py` & `cvprocessor-0.0.13/src/cvprocessor/publications.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.12/src/cvprocessor/research_interests.py` & `cvprocessor-0.0.13/src/cvprocessor/research_interests.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.12/src/cvprocessor/software.py` & `cvprocessor-0.0.13/src/cvprocessor/software.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.12/src/cvprocessor.egg-info/PKG-INFO` & `cvprocessor-0.0.13/src/cvprocessor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.0.12
+Version: 0.0.13
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.0.12/src/cvprocessor.egg-info/SOURCES.txt` & `cvprocessor-0.0.13/src/cvprocessor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

