# Comparing `tmp/moveread_pipelines_input_validation-0.1.1.tar.gz` & `tmp/moveread_pipelines_input_validation-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_pipelines_input_validation-0.1.1.tar", last modified: Tue May  7 14:29:29 2024, max compression
+gzip compressed data, was "moveread_pipelines_input_validation-0.1.2.tar", last modified: Tue May  7 14:32:38 2024, max compression
```

## Comparing `moveread_pipelines_input_validation-0.1.1.tar` & `moveread_pipelines_input_validation-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:29:29.522426 moveread_pipelines_input_validation-0.1.1/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      532 2024-05-07 14:29:29.522426 moveread_pipelines_input_validation-0.1.1/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       60 2024-05-02 17:57:44.000000 moveread_pipelines_input_validation-0.1.1/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      731 2024-05-07 14:29:24.000000 moveread_pipelines_input_validation-0.1.1/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 14:29:29.522426 moveread_pipelines_input_validation-0.1.1/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:29:29.512426 moveread_pipelines_input_validation-0.1.1/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:29:29.512426 moveread_pipelines_input_validation-0.1.1/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:29:29.512426 moveread_pipelines_input_validation-0.1.1/src/moveread/pipelines/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:29:29.522426 moveread_pipelines_input_validation-0.1.1/src/moveread/pipelines/input_validation/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      165 2024-05-02 18:38:03.000000 moveread_pipelines_input_validation-0.1.1/src/moveread/pipelines/input_validation/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      299 2024-05-06 10:40:17.000000 moveread_pipelines_input_validation-0.1.1/src/moveread/pipelines/input_validation/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1984 2024-05-07 14:09:14.000000 moveread_pipelines_input_validation-0.1.1/src/moveread/pipelines/input_validation/api.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1342 2024-05-06 11:30:25.000000 moveread_pipelines_input_validation-0.1.1/src/moveread/pipelines/input_validation/cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      463 2024-05-02 18:38:31.000000 moveread_pipelines_input_validation-0.1.1/src/moveread/pipelines/input_validation/clientgen_cli.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:29:29.522426 moveread_pipelines_input_validation-0.1.1/src/moveread/pipelines/input_validation/integrations/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-06 10:34:33.000000 moveread_pipelines_input_validation-0.1.1/src/moveread/pipelines/input_validation/integrations/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-05-06 10:34:33.000000 moveread_pipelines_input_validation-0.1.1/src/moveread/pipelines/input_validation/integrations/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1681 2024-05-06 10:37:33.000000 moveread_pipelines_input_validation-0.1.1/src/moveread/pipelines/input_validation/integrations/core.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      482 2024-05-07 14:09:28.000000 moveread_pipelines_input_validation-0.1.1/src/moveread/pipelines/input_validation/main.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1002 2024-05-05 16:23:49.000000 moveread_pipelines_input_validation-0.1.1/src/moveread/pipelines/input_validation/sdk.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      590 2024-05-06 13:19:11.000000 moveread_pipelines_input_validation-0.1.1/src/moveread/pipelines/input_validation/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:29:29.522426 moveread_pipelines_input_validation-0.1.1/src/moveread_pipelines_input_validation.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      532 2024-05-07 14:29:29.000000 moveread_pipelines_input_validation-0.1.1/src/moveread_pipelines_input_validation.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      996 2024-05-07 14:29:29.000000 moveread_pipelines_input_validation-0.1.1/src/moveread_pipelines_input_validation.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 14:29:29.000000 moveread_pipelines_input_validation-0.1.1/src/moveread_pipelines_input_validation.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      150 2024-05-07 14:29:29.000000 moveread_pipelines_input_validation-0.1.1/src/moveread_pipelines_input_validation.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       61 2024-05-07 14:29:29.000000 moveread_pipelines_input_validation-0.1.1/src/moveread_pipelines_input_validation.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-07 14:29:29.000000 moveread_pipelines_input_validation-0.1.1/src/moveread_pipelines_input_validation.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:32:38.312415 moveread_pipelines_input_validation-0.1.2/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      532 2024-05-07 14:32:38.312415 moveread_pipelines_input_validation-0.1.2/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       60 2024-05-02 17:57:44.000000 moveread_pipelines_input_validation-0.1.2/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      731 2024-05-07 14:32:36.000000 moveread_pipelines_input_validation-0.1.2/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 14:32:38.312415 moveread_pipelines_input_validation-0.1.2/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:32:38.302415 moveread_pipelines_input_validation-0.1.2/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:32:38.302415 moveread_pipelines_input_validation-0.1.2/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:32:38.302415 moveread_pipelines_input_validation-0.1.2/src/moveread/pipelines/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:32:38.312415 moveread_pipelines_input_validation-0.1.2/src/moveread/pipelines/input_validation/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      165 2024-05-02 18:38:03.000000 moveread_pipelines_input_validation-0.1.2/src/moveread/pipelines/input_validation/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      299 2024-05-06 10:40:17.000000 moveread_pipelines_input_validation-0.1.2/src/moveread/pipelines/input_validation/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1984 2024-05-07 14:09:14.000000 moveread_pipelines_input_validation-0.1.2/src/moveread/pipelines/input_validation/api.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1342 2024-05-06 11:30:25.000000 moveread_pipelines_input_validation-0.1.2/src/moveread/pipelines/input_validation/cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      463 2024-05-02 18:38:31.000000 moveread_pipelines_input_validation-0.1.2/src/moveread/pipelines/input_validation/clientgen_cli.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:32:38.312415 moveread_pipelines_input_validation-0.1.2/src/moveread/pipelines/input_validation/integrations/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-06 10:34:33.000000 moveread_pipelines_input_validation-0.1.2/src/moveread/pipelines/input_validation/integrations/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-05-06 10:34:33.000000 moveread_pipelines_input_validation-0.1.2/src/moveread/pipelines/input_validation/integrations/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1681 2024-05-06 10:37:33.000000 moveread_pipelines_input_validation-0.1.2/src/moveread/pipelines/input_validation/integrations/core.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      482 2024-05-07 14:09:28.000000 moveread_pipelines_input_validation-0.1.2/src/moveread/pipelines/input_validation/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1002 2024-05-05 16:23:49.000000 moveread_pipelines_input_validation-0.1.2/src/moveread/pipelines/input_validation/sdk.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      590 2024-05-06 13:19:11.000000 moveread_pipelines_input_validation-0.1.2/src/moveread/pipelines/input_validation/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:32:38.312415 moveread_pipelines_input_validation-0.1.2/src/moveread_pipelines_input_validation.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      532 2024-05-07 14:32:38.000000 moveread_pipelines_input_validation-0.1.2/src/moveread_pipelines_input_validation.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      996 2024-05-07 14:32:38.000000 moveread_pipelines_input_validation-0.1.2/src/moveread_pipelines_input_validation.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 14:32:38.000000 moveread_pipelines_input_validation-0.1.2/src/moveread_pipelines_input_validation.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      150 2024-05-07 14:32:38.000000 moveread_pipelines_input_validation-0.1.2/src/moveread_pipelines_input_validation.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       61 2024-05-07 14:32:38.000000 moveread_pipelines_input_validation-0.1.2/src/moveread_pipelines_input_validation.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-07 14:32:38.000000 moveread_pipelines_input_validation-0.1.2/src/moveread_pipelines_input_validation.egg-info/top_level.txt
```

### Comparing `moveread_pipelines_input_validation-0.1.1/PKG-INFO` & `moveread_pipelines_input_validation-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-input-validation
-Version: 0.1.1
+Version: 0.1.2
 Summary: Input Validation pipeline for Moveread
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: chess-pairings
 Requires-Dist: pydantic==2.*
```

### Comparing `moveread_pipelines_input_validation-0.1.1/pyproject.toml` & `moveread_pipelines_input_validation-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-pipelines-input-validation"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Input Validation pipeline for Moveread"
 dependencies = [
   "chess-pairings", "pydantic==2.*", "fastapi"
 ]
```

### Comparing `moveread_pipelines_input_validation-0.1.1/src/moveread/pipelines/input_validation/api.py` & `moveread_pipelines_input_validation-0.1.2/src/moveread/pipelines/input_validation/api.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_input_validation-0.1.1/src/moveread/pipelines/input_validation/cli.py` & `moveread_pipelines_input_validation-0.1.2/src/moveread/pipelines/input_validation/cli.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_input_validation-0.1.1/src/moveread/pipelines/input_validation/integrations/core.py` & `moveread_pipelines_input_validation-0.1.2/src/moveread/pipelines/input_validation/integrations/core.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_input_validation-0.1.1/src/moveread/pipelines/input_validation/sdk.py` & `moveread_pipelines_input_validation-0.1.2/src/moveread/pipelines/input_validation/sdk.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_input_validation-0.1.1/src/moveread/pipelines/input_validation/types.py` & `moveread_pipelines_input_validation-0.1.2/src/moveread/pipelines/input_validation/types.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_input_validation-0.1.1/src/moveread_pipelines_input_validation.egg-info/PKG-INFO` & `moveread_pipelines_input_validation-0.1.2/src/moveread_pipelines_input_validation.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-input-validation
-Version: 0.1.1
+Version: 0.1.2
 Summary: Input Validation pipeline for Moveread
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: chess-pairings
 Requires-Dist: pydantic==2.*
```

### Comparing `moveread_pipelines_input_validation-0.1.1/src/moveread_pipelines_input_validation.egg-info/SOURCES.txt` & `moveread_pipelines_input_validation-0.1.2/src/moveread_pipelines_input_validation.egg-info/SOURCES.txt`

 * *Files identical despite different names*
