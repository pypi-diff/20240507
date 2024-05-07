# Comparing `tmp/moveread_pipelines_preprocess-0.1.1.tar.gz` & `tmp/moveread_pipelines_preprocess-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_pipelines_preprocess-0.1.1.tar", last modified: Tue May  7 14:33:06 2024, max compression
+gzip compressed data, was "moveread_pipelines_preprocess-0.1.2.tar", last modified: Tue May  7 14:37:45 2024, max compression
```

## Comparing `moveread_pipelines_preprocess-0.1.1.tar` & `moveread_pipelines_preprocess-0.1.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:06.702426 moveread_pipelines_preprocess-0.1.1/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      765 2024-05-07 14:33:06.702426 moveread_pipelines_preprocess-0.1.1/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       47 2024-05-04 13:39:56.000000 moveread_pipelines_preprocess-0.1.1/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      985 2024-05-07 14:33:04.000000 moveread_pipelines_preprocess-0.1.1/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 14:33:06.702426 moveread_pipelines_preprocess-0.1.1/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:06.692426 moveread_pipelines_preprocess-0.1.1/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:06.692426 moveread_pipelines_preprocess-0.1.1/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:06.692426 moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:06.692426 moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      152 2024-05-04 15:17:40.000000 moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      440 2024-05-05 16:53:46.000000 moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/__init__.pyi
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:06.692426 moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/adapters/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 14:29:38.000000 moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/adapters/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      392 2024-05-04 15:57:10.000000 moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/adapters/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1734 2024-05-07 13:52:27.000000 moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/adapters/correct.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2735 2024-05-04 15:02:16.000000 moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/adapters/extract.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     5476 2024-05-07 14:02:08.000000 moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/adapters/manual_api.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2934 2024-05-04 16:06:41.000000 moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/adapters/preoutput.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      625 2024-05-04 14:54:11.000000 moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/adapters/select.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1367 2024-05-04 14:53:56.000000 moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/adapters/validate.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:06.692426 moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/generated/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      766 2024-05-04 14:49:42.000000 moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/generated/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2223 2024-05-04 14:49:42.000000 moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/generated/local.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     5771 2024-05-04 14:49:42.000000 moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/generated/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:06.692426 moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/integrations/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 15:15:36.000000 moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/integrations/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-05-04 15:15:29.000000 moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/integrations/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1371 2024-05-04 19:40:33.000000 moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/integrations/core.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3302 2024-05-07 14:05:05.000000 moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/main.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:06.692426 moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/scripts/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1690 2024-05-04 17:49:52.000000 moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/scripts/cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      508 2024-05-04 15:25:58.000000 moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/scripts/clientgen_cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      643 2024-05-04 15:13:45.000000 moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/spec.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2794 2024-05-04 15:17:30.000000 moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:06.702426 moveread_pipelines_preprocess-0.1.1/src/moveread_pipelines_preprocess.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      765 2024-05-07 14:33:06.000000 moveread_pipelines_preprocess-0.1.1/src/moveread_pipelines_preprocess.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1472 2024-05-07 14:33:06.000000 moveread_pipelines_preprocess-0.1.1/src/moveread_pipelines_preprocess.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 14:33:06.000000 moveread_pipelines_preprocess-0.1.1/src/moveread_pipelines_preprocess.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      222 2024-05-07 14:33:06.000000 moveread_pipelines_preprocess-0.1.1/src/moveread_pipelines_preprocess.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      220 2024-05-07 14:33:06.000000 moveread_pipelines_preprocess-0.1.1/src/moveread_pipelines_preprocess.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-07 14:33:06.000000 moveread_pipelines_preprocess-0.1.1/src/moveread_pipelines_preprocess.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:37:45.986509 moveread_pipelines_preprocess-0.1.2/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      765 2024-05-07 14:37:45.986509 moveread_pipelines_preprocess-0.1.2/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       47 2024-05-04 13:39:56.000000 moveread_pipelines_preprocess-0.1.2/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      985 2024-05-07 14:37:42.000000 moveread_pipelines_preprocess-0.1.2/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 14:37:45.986509 moveread_pipelines_preprocess-0.1.2/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:37:45.966509 moveread_pipelines_preprocess-0.1.2/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:37:45.966509 moveread_pipelines_preprocess-0.1.2/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:37:45.966509 moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:37:45.976509 moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      152 2024-05-04 15:17:40.000000 moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      440 2024-05-05 16:53:46.000000 moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:37:45.976509 moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/adapters/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 14:29:38.000000 moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/adapters/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      392 2024-05-04 15:57:10.000000 moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/adapters/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1734 2024-05-07 13:52:27.000000 moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/adapters/correct.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2735 2024-05-04 15:02:16.000000 moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/adapters/extract.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     5476 2024-05-07 14:02:08.000000 moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/adapters/manual_api.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2934 2024-05-04 16:06:41.000000 moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/adapters/preoutput.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      625 2024-05-04 14:54:11.000000 moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/adapters/select.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1367 2024-05-04 14:53:56.000000 moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/adapters/validate.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:37:45.976509 moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/generated/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      766 2024-05-04 14:49:42.000000 moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/generated/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2223 2024-05-04 14:49:42.000000 moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/generated/local.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     5771 2024-05-04 14:49:42.000000 moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/generated/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:37:45.976509 moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/integrations/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 15:15:36.000000 moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/integrations/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-05-04 15:15:29.000000 moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/integrations/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1371 2024-05-04 19:40:33.000000 moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/integrations/core.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3302 2024-05-07 14:05:05.000000 moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/main.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:37:45.976509 moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/scripts/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1690 2024-05-04 17:49:52.000000 moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/scripts/cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      508 2024-05-04 15:25:58.000000 moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/scripts/clientgen_cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      643 2024-05-04 15:13:45.000000 moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/spec.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2794 2024-05-04 15:17:30.000000 moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:37:45.986509 moveread_pipelines_preprocess-0.1.2/src/moveread_pipelines_preprocess.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      765 2024-05-07 14:37:45.000000 moveread_pipelines_preprocess-0.1.2/src/moveread_pipelines_preprocess.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1472 2024-05-07 14:37:45.000000 moveread_pipelines_preprocess-0.1.2/src/moveread_pipelines_preprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 14:37:45.000000 moveread_pipelines_preprocess-0.1.2/src/moveread_pipelines_preprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      222 2024-05-07 14:37:45.000000 moveread_pipelines_preprocess-0.1.2/src/moveread_pipelines_preprocess.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      220 2024-05-07 14:37:45.000000 moveread_pipelines_preprocess-0.1.2/src/moveread_pipelines_preprocess.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-07 14:37:45.000000 moveread_pipelines_preprocess-0.1.2/src/moveread_pipelines_preprocess.egg-info/top_level.txt
```

### Comparing `moveread_pipelines_preprocess-0.1.1/PKG-INFO` & `moveread_pipelines_preprocess-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-preprocess
-Version: 0.1.1
+Version: 0.1.2
 Summary: Moveread preprocessing pipeline
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: queue-pipelines[all]
 Requires-Dist: haskellian
```

### Comparing `moveread_pipelines_preprocess-0.1.1/pyproject.toml` & `moveread_pipelines_preprocess-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-pipelines-preprocess"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Moveread preprocessing pipeline"
 dependencies = [
   "queue-pipelines[all]", "haskellian", "kv-api", "dslog",
   "moveread-pipelines-auto-extract",
```

### Comparing `moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/adapters/correct.py` & `moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/adapters/correct.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/adapters/extract.py` & `moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/adapters/extract.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/adapters/manual_api.py` & `moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/adapters/manual_api.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/adapters/preoutput.py` & `moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/adapters/preoutput.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/adapters/select.py` & `moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/adapters/select.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/adapters/validate.py` & `moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/adapters/validate.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/generated/__init__.py` & `moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/generated/local.py` & `moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/generated/local.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/generated/types.py` & `moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/generated/types.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/integrations/core.py` & `moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/integrations/core.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/main.py` & `moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/main.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/scripts/cli.py` & `moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/spec.py` & `moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/spec.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.1/src/moveread/pipelines/preprocess/types.py` & `moveread_pipelines_preprocess-0.1.2/src/moveread/pipelines/preprocess/types.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_preprocess-0.1.1/src/moveread_pipelines_preprocess.egg-info/PKG-INFO` & `moveread_pipelines_preprocess-0.1.2/src/moveread_pipelines_preprocess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-preprocess
-Version: 0.1.1
+Version: 0.1.2
 Summary: Moveread preprocessing pipeline
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: queue-pipelines[all]
 Requires-Dist: haskellian
```

### Comparing `moveread_pipelines_preprocess-0.1.1/src/moveread_pipelines_preprocess.egg-info/SOURCES.txt` & `moveread_pipelines_preprocess-0.1.2/src/moveread_pipelines_preprocess.egg-info/SOURCES.txt`

 * *Files identical despite different names*

