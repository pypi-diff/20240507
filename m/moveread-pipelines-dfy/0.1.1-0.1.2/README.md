# Comparing `tmp/moveread_pipelines_dfy-0.1.1.tar.gz` & `tmp/moveread_pipelines_dfy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_pipelines_dfy-0.1.1.tar", last modified: Tue May  7 14:33:24 2024, max compression
+gzip compressed data, was "moveread_pipelines_dfy-0.1.2.tar", last modified: Tue May  7 14:38:09 2024, max compression
```

## Comparing `moveread_pipelines_dfy-0.1.1.tar` & `moveread_pipelines_dfy-0.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:24.292427 moveread_pipelines_dfy-0.1.1/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      521 2024-05-07 14:33:24.292427 moveread_pipelines_dfy-0.1.1/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       34 2024-05-05 15:36:13.000000 moveread_pipelines_dfy-0.1.1/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      822 2024-05-07 14:33:22.000000 moveread_pipelines_dfy-0.1.1/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 14:33:24.292427 moveread_pipelines_dfy-0.1.1/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:24.272427 moveread_pipelines_dfy-0.1.1/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:24.272427 moveread_pipelines_dfy-0.1.1/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:24.272427 moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:24.282427 moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      157 2024-05-05 18:21:26.000000 moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      300 2024-05-07 10:37:19.000000 moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1533 2024-05-06 13:11:15.000000 moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/cli.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:24.282427 moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/generated/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      539 2024-05-05 18:09:39.000000 moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/generated/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2644 2024-05-05 18:09:39.000000 moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/generated/local.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3018 2024-05-05 18:09:39.000000 moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/generated/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:24.282427 moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/integrations/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-06 10:09:40.000000 moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/integrations/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-05-06 10:09:40.000000 moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/integrations/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1684 2024-05-06 10:14:43.000000 moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/integrations/core.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1381 2024-05-06 10:29:14.000000 moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/main.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:24.292427 moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/pipelines/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      276 2024-05-05 18:16:26.000000 moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/pipelines/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      655 2024-05-05 18:04:52.000000 moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/pipelines/_gamecorr.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      868 2024-05-05 18:10:26.000000 moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/pipelines/_inputval.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      575 2024-05-05 18:16:10.000000 moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/pipelines/_ocr.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      670 2024-05-06 13:38:47.000000 moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/pipelines/_preprocess.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1888 2024-05-07 10:48:38.000000 moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/spec.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:24.292427 moveread_pipelines_dfy-0.1.1/src/moveread_pipelines_dfy.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      521 2024-05-07 14:33:24.000000 moveread_pipelines_dfy-0.1.1/src/moveread_pipelines_dfy.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1145 2024-05-07 14:33:24.000000 moveread_pipelines_dfy-0.1.1/src/moveread_pipelines_dfy.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 14:33:24.000000 moveread_pipelines_dfy-0.1.1/src/moveread_pipelines_dfy.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      124 2024-05-07 14:33:24.000000 moveread_pipelines_dfy-0.1.1/src/moveread_pipelines_dfy.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      137 2024-05-07 14:33:24.000000 moveread_pipelines_dfy-0.1.1/src/moveread_pipelines_dfy.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-07 14:33:24.000000 moveread_pipelines_dfy-0.1.1/src/moveread_pipelines_dfy.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:38:09.286864 moveread_pipelines_dfy-0.1.2/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      521 2024-05-07 14:38:09.286864 moveread_pipelines_dfy-0.1.2/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       34 2024-05-05 15:36:13.000000 moveread_pipelines_dfy-0.1.2/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      822 2024-05-07 14:38:06.000000 moveread_pipelines_dfy-0.1.2/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 14:38:09.286864 moveread_pipelines_dfy-0.1.2/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:38:09.276863 moveread_pipelines_dfy-0.1.2/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:38:09.276863 moveread_pipelines_dfy-0.1.2/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:38:09.276863 moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:38:09.286864 moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      157 2024-05-05 18:21:26.000000 moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      300 2024-05-07 10:37:19.000000 moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1533 2024-05-06 13:11:15.000000 moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/cli.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:38:09.286864 moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/generated/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      539 2024-05-05 18:09:39.000000 moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/generated/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2644 2024-05-05 18:09:39.000000 moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/generated/local.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3018 2024-05-05 18:09:39.000000 moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/generated/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:38:09.286864 moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/integrations/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-06 10:09:40.000000 moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/integrations/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-05-06 10:09:40.000000 moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/integrations/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1684 2024-05-06 10:14:43.000000 moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/integrations/core.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1381 2024-05-06 10:29:14.000000 moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/main.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:38:09.286864 moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/pipelines/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      276 2024-05-05 18:16:26.000000 moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/pipelines/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      655 2024-05-05 18:04:52.000000 moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/pipelines/_gamecorr.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      868 2024-05-05 18:10:26.000000 moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/pipelines/_inputval.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      575 2024-05-05 18:16:10.000000 moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/pipelines/_ocr.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      670 2024-05-06 13:38:47.000000 moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/pipelines/_preprocess.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1888 2024-05-07 10:48:38.000000 moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/spec.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:38:09.286864 moveread_pipelines_dfy-0.1.2/src/moveread_pipelines_dfy.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      521 2024-05-07 14:38:09.000000 moveread_pipelines_dfy-0.1.2/src/moveread_pipelines_dfy.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1145 2024-05-07 14:38:09.000000 moveread_pipelines_dfy-0.1.2/src/moveread_pipelines_dfy.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 14:38:09.000000 moveread_pipelines_dfy-0.1.2/src/moveread_pipelines_dfy.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      124 2024-05-07 14:38:09.000000 moveread_pipelines_dfy-0.1.2/src/moveread_pipelines_dfy.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      137 2024-05-07 14:38:09.000000 moveread_pipelines_dfy-0.1.2/src/moveread_pipelines_dfy.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-07 14:38:09.000000 moveread_pipelines_dfy-0.1.2/src/moveread_pipelines_dfy.egg-info/top_level.txt
```

### Comparing `moveread_pipelines_dfy-0.1.1/PKG-INFO` & `moveread_pipelines_dfy-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-dfy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pipeline for Moveread DFY
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: moveread-pipelines-input-validation
 Requires-Dist: moveread-pipelines-game-preprocess
```

### Comparing `moveread_pipelines_dfy-0.1.1/pyproject.toml` & `moveread_pipelines_dfy-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-pipelines-dfy"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Pipeline for Moveread DFY"
 dependencies = [
   "moveread-pipelines-input-validation",
   "moveread-pipelines-game-preprocess",
```

### Comparing `moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/cli.py` & `moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/cli.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/generated/__init__.py` & `moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/generated/local.py` & `moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/generated/local.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/generated/types.py` & `moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/generated/types.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/integrations/core.py` & `moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/integrations/core.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/main.py` & `moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/main.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/pipelines/_gamecorr.py` & `moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/pipelines/_gamecorr.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/pipelines/_inputval.py` & `moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/pipelines/_inputval.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/pipelines/_ocr.py` & `moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/pipelines/_ocr.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/pipelines/_preprocess.py` & `moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/pipelines/_preprocess.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_dfy-0.1.1/src/moveread/pipelines/local_dfy/spec.py` & `moveread_pipelines_dfy-0.1.2/src/moveread/pipelines/local_dfy/spec.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_dfy-0.1.1/src/moveread_pipelines_dfy.egg-info/PKG-INFO` & `moveread_pipelines_dfy-0.1.2/src/moveread_pipelines_dfy.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-dfy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pipeline for Moveread DFY
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: moveread-pipelines-input-validation
 Requires-Dist: moveread-pipelines-game-preprocess
```

### Comparing `moveread_pipelines_dfy-0.1.1/src/moveread_pipelines_dfy.egg-info/SOURCES.txt` & `moveread_pipelines_dfy-0.1.2/src/moveread_pipelines_dfy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

