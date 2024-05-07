# Comparing `tmp/qbitrr2-4.5.7.tar.gz` & `tmp/qbitrr2-4.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbitrr2-4.5.7.tar", last modified: Wed May  1 13:50:23 2024, max compression
+gzip compressed data, was "qbitrr2-4.5.8.tar", last modified: Tue May  7 07:26:20 2024, max compression
```

## Comparing `qbitrr2-4.5.7.tar` & `qbitrr2-4.5.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:50:23.617251 qbitrr2-4.5.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-01 13:50:18.000000 qbitrr2-4.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-01 13:50:23.617251 qbitrr2-4.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-01 13:50:18.000000 qbitrr2-4.5.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-01 13:50:18.000000 qbitrr2-4.5.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:50:23.613251 qbitrr2-4.5.7/qBitrr/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-01 13:50:18.000000 qbitrr2-4.5.7/qBitrr/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   226829 2024-05-01 13:50:18.000000 qbitrr2-4.5.7/qBitrr/arss.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-01 13:50:18.000000 qbitrr2-4.5.7/qBitrr/bundled_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-01 13:50:18.000000 qbitrr2-4.5.7/qBitrr/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-01 13:50:18.000000 qbitrr2-4.5.7/qBitrr/env_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-01 13:50:18.000000 qbitrr2-4.5.7/qBitrr/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-01 13:50:18.000000 qbitrr2-4.5.7/qBitrr/ffprobe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26588 2024-05-01 13:50:18.000000 qbitrr2-4.5.7/qBitrr/gen_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-01 13:50:18.000000 qbitrr2-4.5.7/qBitrr/home_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-01 13:50:18.000000 qbitrr2-4.5.7/qBitrr/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7347 2024-05-01 13:50:18.000000 qbitrr2-4.5.7/qBitrr/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-01 13:50:18.000000 qbitrr2-4.5.7/qBitrr/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-01 13:50:18.000000 qbitrr2-4.5.7/qBitrr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:50:23.617251 qbitrr2-4.5.7/qBitrr2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-01 13:50:23.000000 qbitrr2-4.5.7/qBitrr2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-01 13:50:23.000000 qbitrr2-4.5.7/qBitrr2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:50:23.000000 qbitrr2-4.5.7/qBitrr2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-01 13:50:23.000000 qbitrr2-4.5.7/qBitrr2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-01 13:50:23.000000 qbitrr2-4.5.7/qBitrr2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 13:50:23.000000 qbitrr2-4.5.7/qBitrr2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-01 13:50:23.617251 qbitrr2-4.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 13:50:18.000000 qbitrr2-4.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:26:20.994596 qbitrr2-4.5.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-07 07:26:12.000000 qbitrr2-4.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-07 07:26:20.994596 qbitrr2-4.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-07 07:26:12.000000 qbitrr2-4.5.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-07 07:26:12.000000 qbitrr2-4.5.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:26:20.990596 qbitrr2-4.5.8/qBitrr/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-07 07:26:12.000000 qbitrr2-4.5.8/qBitrr/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   226892 2024-05-07 07:26:12.000000 qbitrr2-4.5.8/qBitrr/arss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-07 07:26:12.000000 qbitrr2-4.5.8/qBitrr/bundled_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-07 07:26:12.000000 qbitrr2-4.5.8/qBitrr/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-07 07:26:12.000000 qbitrr2-4.5.8/qBitrr/env_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-07 07:26:12.000000 qbitrr2-4.5.8/qBitrr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-07 07:26:12.000000 qbitrr2-4.5.8/qBitrr/ffprobe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26588 2024-05-07 07:26:12.000000 qbitrr2-4.5.8/qBitrr/gen_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-07 07:26:12.000000 qbitrr2-4.5.8/qBitrr/home_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-07 07:26:12.000000 qbitrr2-4.5.8/qBitrr/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7347 2024-05-07 07:26:12.000000 qbitrr2-4.5.8/qBitrr/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-07 07:26:12.000000 qbitrr2-4.5.8/qBitrr/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-07 07:26:12.000000 qbitrr2-4.5.8/qBitrr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:26:20.990596 qbitrr2-4.5.8/qBitrr2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-07 07:26:20.000000 qbitrr2-4.5.8/qBitrr2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-07 07:26:20.000000 qbitrr2-4.5.8/qBitrr2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:26:20.000000 qbitrr2-4.5.8/qBitrr2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 07:26:20.000000 qbitrr2-4.5.8/qBitrr2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-07 07:26:20.000000 qbitrr2-4.5.8/qBitrr2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 07:26:20.000000 qbitrr2-4.5.8/qBitrr2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-07 07:26:20.994596 qbitrr2-4.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:26:12.000000 qbitrr2-4.5.8/setup.py
```

### Comparing `qbitrr2-4.5.7/LICENSE` & `qbitrr2-4.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.5.7/PKG-INFO` & `qbitrr2-4.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qBitrr2
-Version: 4.5.7
+Version: 4.5.8
 Summary: "A simple Python script to talk to qBittorrent and Arr's"
 Home-page: https://github.com/Feramance/qBitrr
 Author: Feramance
 Author-email: fera@fera.wtf
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Feramance/qBitrr/issues
 Project-URL: Source Code, https://github.com/Feramance/qBitrr
```

### Comparing `qbitrr2-4.5.7/README.md` & `qbitrr2-4.5.8/README.md`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.5.7/pyproject.toml` & `qbitrr2-4.5.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 [tool.black]
 line-length = 99
 target-version = ['py38']
 
 [tool.poetry]
 name = "pypi-public"
-version = "4.5.7"
+version = "4.5.8"
 description = "A simple script to monitor qBit and communicate with Radarr and Sonarr"
 authors = ["Drapersniper", "Feramance"]
 readme = "README.md"
 repository = "https://github.com/Feramance/qBitrr"
 url = "https://pypi.org/simple/"
 
 [tool.autopep8]
```

### Comparing `qbitrr2-4.5.7/qBitrr/arss.py` & `qbitrr2-4.5.8/qBitrr/arss.py`

 * *Files 0% similar despite different names*

```diff
@@ -3883,14 +3883,15 @@
         elif (
             torrent.state_enum
             in (
                 TorrentStates.METADATA_DOWNLOAD,
                 TorrentStates.STALLED_DOWNLOAD,
             )
             and "qBitrr-ignored" not in torrent.tags
+            and "qBitrr-free_space_paused" not in torrent.tags
         ):
             self._process_single_torrent_stalled_torrent(torrent, "Stalled State")
         elif (
             torrent.state_enum.is_downloading
             and torrent.state_enum != TorrentStates.METADATA_DOWNLOAD
             and torrent.hash not in self.special_casing_file_check
             and torrent.hash not in self.cleaned_torrents
```

### Comparing `qbitrr2-4.5.7/qBitrr/config.py` & `qbitrr2-4.5.8/qBitrr/config.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.5.7/qBitrr/env_config.py` & `qbitrr2-4.5.8/qBitrr/env_config.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.5.7/qBitrr/errors.py` & `qbitrr2-4.5.8/qBitrr/errors.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.5.7/qBitrr/ffprobe.py` & `qbitrr2-4.5.8/qBitrr/ffprobe.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.5.7/qBitrr/gen_config.py` & `qbitrr2-4.5.8/qBitrr/gen_config.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.5.7/qBitrr/home_path.py` & `qbitrr2-4.5.8/qBitrr/home_path.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.5.7/qBitrr/logger.py` & `qbitrr2-4.5.8/qBitrr/logger.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.5.7/qBitrr/main.py` & `qbitrr2-4.5.8/qBitrr/main.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.5.7/qBitrr/tables.py` & `qbitrr2-4.5.8/qBitrr/tables.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.5.7/qBitrr/utils.py` & `qbitrr2-4.5.8/qBitrr/utils.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.5.7/qBitrr2.egg-info/PKG-INFO` & `qbitrr2-4.5.8/qBitrr2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qBitrr2
-Version: 4.5.7
+Version: 4.5.8
 Summary: "A simple Python script to talk to qBittorrent and Arr's"
 Home-page: https://github.com/Feramance/qBitrr
 Author: Feramance
 Author-email: fera@fera.wtf
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Feramance/qBitrr/issues
 Project-URL: Source Code, https://github.com/Feramance/qBitrr
```

### Comparing `qbitrr2-4.5.7/qBitrr2.egg-info/requires.txt` & `qbitrr2-4.5.8/qBitrr2.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.5.7/setup.cfg` & `qbitrr2-4.5.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qBitrr2
-version = 4.5.7
+version = 4.5.8
 description = "A simple Python script to talk to qBittorrent and Arr's"
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Feramance/qBitrr
 author = Feramance
 author_email = fera@fera.wtf
 license = MIT
```

