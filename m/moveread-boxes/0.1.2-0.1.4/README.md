# Comparing `tmp/moveread_boxes-0.1.2.tar.gz` & `tmp/moveread_boxes-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_boxes-0.1.2.tar", last modified: Thu Apr 25 07:24:02 2024, max compression
+gzip compressed data, was "moveread_boxes-0.1.4.tar", last modified: Tue May  7 13:37:56 2024, max compression
```

## Comparing `moveread_boxes-0.1.2.tar` & `moveread_boxes-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:24:02.144243 moveread_boxes-0.1.2/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1348 2024-04-25 07:24:02.144243 moveread_boxes-0.1.2/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      866 2024-04-25 05:33:54.000000 moveread_boxes-0.1.2/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      555 2024-04-25 07:23:58.000000 moveread_boxes-0.1.2/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 07:24:02.144243 moveread_boxes-0.1.2/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:24:02.144243 moveread_boxes-0.1.2/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:24:02.134243 moveread_boxes-0.1.2/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:24:02.144243 moveread_boxes-0.1.2/src/moveread/boxes/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      155 2024-04-21 17:24:46.000000 moveread_boxes-0.1.2/src/moveread/boxes/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      430 2024-04-25 05:20:32.000000 moveread_boxes-0.1.2/src/moveread/boxes/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1485 2024-04-25 05:20:03.000000 moveread_boxes-0.1.2/src/moveread/boxes/annotations.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      507 2024-04-21 18:40:35.000000 moveread_boxes-0.1.2/src/moveread/boxes/export_.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1936 2024-04-25 07:23:31.000000 moveread_boxes-0.1.2/src/moveread/boxes/model_extract.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:24:02.144243 moveread_boxes-0.1.2/src/moveread_boxes.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1348 2024-04-25 07:24:02.000000 moveread_boxes-0.1.2/src/moveread_boxes.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      396 2024-04-25 07:24:02.000000 moveread_boxes-0.1.2/src/moveread_boxes.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 07:24:02.000000 moveread_boxes-0.1.2/src/moveread_boxes.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       88 2024-04-25 07:24:02.000000 moveread_boxes-0.1.2/src/moveread_boxes.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-04-25 07:24:02.000000 moveread_boxes-0.1.2/src/moveread_boxes.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:37:56.872430 moveread_boxes-0.1.4/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1381 2024-05-07 13:37:56.872430 moveread_boxes-0.1.4/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      866 2024-04-25 05:33:54.000000 moveread_boxes-0.1.4/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      576 2024-05-07 13:37:54.000000 moveread_boxes-0.1.4/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 13:37:56.872430 moveread_boxes-0.1.4/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:37:56.872430 moveread_boxes-0.1.4/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:37:56.872430 moveread_boxes-0.1.4/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:37:56.872430 moveread_boxes-0.1.4/src/moveread/boxes/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      155 2024-04-21 17:24:46.000000 moveread_boxes-0.1.4/src/moveread/boxes/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      430 2024-04-25 05:20:32.000000 moveread_boxes-0.1.4/src/moveread/boxes/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1485 2024-04-25 05:20:03.000000 moveread_boxes-0.1.4/src/moveread/boxes/annotations.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      507 2024-04-21 18:40:35.000000 moveread_boxes-0.1.4/src/moveread/boxes/export_.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1936 2024-04-25 07:23:31.000000 moveread_boxes-0.1.4/src/moveread/boxes/model_extract.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:37:56.872430 moveread_boxes-0.1.4/src/moveread_boxes.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1381 2024-05-07 13:37:56.000000 moveread_boxes-0.1.4/src/moveread_boxes.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      396 2024-05-07 13:37:56.000000 moveread_boxes-0.1.4/src/moveread_boxes.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 13:37:56.000000 moveread_boxes-0.1.4/src/moveread_boxes.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      106 2024-05-07 13:37:56.000000 moveread_boxes-0.1.4/src/moveread_boxes.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-07 13:37:56.000000 moveread_boxes-0.1.4/src/moveread_boxes.egg-info/top_level.txt
```

### Comparing `moveread_boxes-0.1.2/PKG-INFO` & `moveread_boxes-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: moveread-boxes
-Version: 0.1.2
+Version: 0.1.4
 Summary: Annotating and exporting boxes for Moveread
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-core
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: scoresheet-models
 Requires-Dist: numpy
 Requires-Dist: opencv-python
+Requires-Dist: robust-extraction
 Requires-Dist: pydantic
 Requires-Dist: haskellian
 Requires-Dist: lazy-loader
 Requires-Dist: typing-extensions
 
 # Moveread Boxes
```

### Comparing `moveread_boxes-0.1.2/README.md` & `moveread_boxes-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `moveread_boxes-0.1.2/pyproject.toml` & `moveread_boxes-0.1.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-boxes"
-version = "0.1.2"
+version = "0.1.4"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Annotating and exporting boxes for Moveread"
 dependencies = [
-  "scoresheet-models", "numpy", "opencv-python",
+  "scoresheet-models", "numpy", "opencv-python", "robust-extraction",
   "pydantic", "haskellian", "lazy-loader", "typing-extensions"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
 repo = "https://github.com/moveread/python-core"
```

### Comparing `moveread_boxes-0.1.2/src/moveread/boxes/annotations.py` & `moveread_boxes-0.1.4/src/moveread/boxes/annotations.py`

 * *Files identical despite different names*

### Comparing `moveread_boxes-0.1.2/src/moveread/boxes/model_extract.py` & `moveread_boxes-0.1.4/src/moveread/boxes/model_extract.py`

 * *Files identical despite different names*

### Comparing `moveread_boxes-0.1.2/src/moveread_boxes.egg-info/PKG-INFO` & `moveread_boxes-0.1.4/src/moveread_boxes.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: moveread-boxes
-Version: 0.1.2
+Version: 0.1.4
 Summary: Annotating and exporting boxes for Moveread
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-core
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: scoresheet-models
 Requires-Dist: numpy
 Requires-Dist: opencv-python
+Requires-Dist: robust-extraction
 Requires-Dist: pydantic
 Requires-Dist: haskellian
 Requires-Dist: lazy-loader
 Requires-Dist: typing-extensions
 
 # Moveread Boxes
```
