# Comparing `tmp/moveread_pipelines_game_preprocess-0.1.1.tar.gz` & `tmp/moveread_pipelines_game_preprocess-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_pipelines_game_preprocess-0.1.1.tar", last modified: Tue May  7 14:33:14 2024, max compression
+gzip compressed data, was "moveread_pipelines_game_preprocess-0.1.2.tar", last modified: Tue May  7 14:37:57 2024, max compression
```

## Comparing `moveread_pipelines_game_preprocess-0.1.1.tar` & `moveread_pipelines_game_preprocess-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:14.862427 moveread_pipelines_game_preprocess-0.1.1/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-05-07 14:33:14.862427 moveread_pipelines_game_preprocess-0.1.1/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       85 2024-05-04 18:06:49.000000 moveread_pipelines_game_preprocess-0.1.1/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      771 2024-05-07 14:33:12.000000 moveread_pipelines_game_preprocess-0.1.1/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 14:33:14.862427 moveread_pipelines_game_preprocess-0.1.1/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:14.852427 moveread_pipelines_game_preprocess-0.1.1/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:14.852427 moveread_pipelines_game_preprocess-0.1.1/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:14.852427 moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:14.862427 moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      190 2024-05-04 18:57:40.000000 moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      312 2024-05-05 16:57:44.000000 moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1673 2024-05-06 10:17:13.000000 moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/cli.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:14.862427 moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/generated/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      538 2024-05-06 13:36:44.000000 moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/generated/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2643 2024-05-06 13:36:44.000000 moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/generated/local.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2363 2024-05-06 13:36:44.000000 moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/generated/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:14.862427 moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/integrations/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 19:31:31.000000 moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/integrations/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-05-04 19:31:31.000000 moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/integrations/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1481 2024-05-07 13:45:54.000000 moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/integrations/core.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1797 2024-05-06 10:23:12.000000 moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/main.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:14.862427 moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/pipelines/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      146 2024-05-04 19:01:42.000000 moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/pipelines/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1713 2024-05-05 17:01:06.000000 moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/pipelines/_join.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1043 2024-05-05 17:00:46.000000 moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/pipelines/_preinput.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      590 2024-05-05 18:19:37.000000 moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/pipelines/_preprocess.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      856 2024-05-06 13:36:26.000000 moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/spec.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:33:14.862427 moveread_pipelines_game_preprocess-0.1.1/src/moveread_pipelines_game_preprocess.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-05-07 14:33:14.000000 moveread_pipelines_game_preprocess-0.1.1/src/moveread_pipelines_game_preprocess.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1252 2024-05-07 14:33:14.000000 moveread_pipelines_game_preprocess-0.1.1/src/moveread_pipelines_game_preprocess.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 14:33:14.000000 moveread_pipelines_game_preprocess-0.1.1/src/moveread_pipelines_game_preprocess.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      138 2024-05-07 14:33:14.000000 moveread_pipelines_game_preprocess-0.1.1/src/moveread_pipelines_game_preprocess.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       87 2024-05-07 14:33:14.000000 moveread_pipelines_game_preprocess-0.1.1/src/moveread_pipelines_game_preprocess.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-07 14:33:14.000000 moveread_pipelines_game_preprocess-0.1.1/src/moveread_pipelines_game_preprocess.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:37:57.826689 moveread_pipelines_game_preprocess-0.1.2/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-05-07 14:37:57.826689 moveread_pipelines_game_preprocess-0.1.2/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       85 2024-05-04 18:06:49.000000 moveread_pipelines_game_preprocess-0.1.2/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      771 2024-05-07 14:37:54.000000 moveread_pipelines_game_preprocess-0.1.2/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 14:37:57.826689 moveread_pipelines_game_preprocess-0.1.2/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:37:57.816689 moveread_pipelines_game_preprocess-0.1.2/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:37:57.816689 moveread_pipelines_game_preprocess-0.1.2/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:37:57.816689 moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:37:57.816689 moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      190 2024-05-04 18:57:40.000000 moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      312 2024-05-05 16:57:44.000000 moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1673 2024-05-06 10:17:13.000000 moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/cli.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:37:57.816689 moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/generated/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      538 2024-05-06 13:36:44.000000 moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/generated/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2643 2024-05-06 13:36:44.000000 moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/generated/local.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2363 2024-05-06 13:36:44.000000 moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/generated/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:37:57.816689 moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/integrations/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 19:31:31.000000 moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/integrations/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-05-04 19:31:31.000000 moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/integrations/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1481 2024-05-07 13:45:54.000000 moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/integrations/core.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1797 2024-05-06 10:23:12.000000 moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/main.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:37:57.816689 moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/pipelines/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      146 2024-05-04 19:01:42.000000 moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/pipelines/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1713 2024-05-05 17:01:06.000000 moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/pipelines/_join.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1043 2024-05-05 17:00:46.000000 moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/pipelines/_preinput.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      590 2024-05-05 18:19:37.000000 moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/pipelines/_preprocess.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      856 2024-05-06 13:36:26.000000 moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/spec.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 14:37:57.826689 moveread_pipelines_game_preprocess-0.1.2/src/moveread_pipelines_game_preprocess.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-05-07 14:37:57.000000 moveread_pipelines_game_preprocess-0.1.2/src/moveread_pipelines_game_preprocess.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1252 2024-05-07 14:37:57.000000 moveread_pipelines_game_preprocess-0.1.2/src/moveread_pipelines_game_preprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 14:37:57.000000 moveread_pipelines_game_preprocess-0.1.2/src/moveread_pipelines_game_preprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      138 2024-05-07 14:37:57.000000 moveread_pipelines_game_preprocess-0.1.2/src/moveread_pipelines_game_preprocess.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       87 2024-05-07 14:37:57.000000 moveread_pipelines_game_preprocess-0.1.2/src/moveread_pipelines_game_preprocess.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-07 14:37:57.000000 moveread_pipelines_game_preprocess-0.1.2/src/moveread_pipelines_game_preprocess.egg-info/top_level.txt
```

### Comparing `moveread_pipelines_game_preprocess-0.1.1/PKG-INFO` & `moveread_pipelines_game_preprocess-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-game-preprocess
-Version: 0.1.1
+Version: 0.1.2
 Summary: Like Moveread Preprocess, but joining scoresheets of a same game
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: moveread-pipelines-preprocess
 Requires-Dist: kv-fs
```

### Comparing `moveread_pipelines_game_preprocess-0.1.1/pyproject.toml` & `moveread_pipelines_game_preprocess-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-pipelines-game-preprocess"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Like Moveread Preprocess, but joining scoresheets of a same game"
 dependencies = [
   "moveread-pipelines-preprocess", "kv-fs", "kv-sqlite-sync"
 ]
```

### Comparing `moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/cli.py` & `moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/cli.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/generated/__init__.py` & `moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/generated/local.py` & `moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/generated/local.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/generated/types.py` & `moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/generated/types.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/integrations/core.py` & `moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/integrations/core.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/main.py` & `moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/main.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/pipelines/_join.py` & `moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/pipelines/_join.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/pipelines/_preinput.py` & `moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/pipelines/_preinput.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/pipelines/_preprocess.py` & `moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/pipelines/_preprocess.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_preprocess-0.1.1/src/moveread/pipelines/game_preprocess/spec.py` & `moveread_pipelines_game_preprocess-0.1.2/src/moveread/pipelines/game_preprocess/spec.py`

 * *Files identical despite different names*

### Comparing `moveread_pipelines_game_preprocess-0.1.1/src/moveread_pipelines_game_preprocess.egg-info/PKG-INFO` & `moveread_pipelines_game_preprocess-0.1.2/src/moveread_pipelines_game_preprocess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-pipelines-game-preprocess
-Version: 0.1.1
+Version: 0.1.2
 Summary: Like Moveread Preprocess, but joining scoresheets of a same game
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: moveread-pipelines-preprocess
 Requires-Dist: kv-fs
```

### Comparing `moveread_pipelines_game_preprocess-0.1.1/src/moveread_pipelines_game_preprocess.egg-info/SOURCES.txt` & `moveread_pipelines_game_preprocess-0.1.2/src/moveread_pipelines_game_preprocess.egg-info/SOURCES.txt`

 * *Files identical despite different names*

