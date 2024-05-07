# Comparing `tmp/playsound3-2.0.4.tar.gz` & `tmp/playsound3-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playsound3-2.0.4.tar", last modified: Mon May  6 20:59:16 2024, max compression
+gzip compressed data, was "playsound3-2.1.0.tar", last modified: Mon May  6 23:37:50 2024, max compression
```

## Comparing `playsound3-2.0.4.tar` & `playsound3-2.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-05-06 20:59:16.832440 playsound3-2.0.4/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1962 2024-05-06 14:15:46.000000 playsound3-2.0.4/LICENSE
--rw-r--r--   0 gaha      (1000) gaha      (1000)     2600 2024-05-06 20:59:16.832440 playsound3-2.0.4/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1599 2024-05-06 20:58:41.000000 playsound3-2.0.4/README.md
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-05-06 20:59:16.832440 playsound3-2.0.4/playsound3/
--rw-r--r--   0 gaha      (1000) gaha      (1000)       44 2024-05-06 14:32:01.000000 playsound3-2.0.4/playsound3/__init__.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     3371 2024-05-06 20:57:13.000000 playsound3-2.0.4/playsound3/playsound3.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-05-06 20:59:16.832440 playsound3-2.0.4/playsound3.egg-info/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     2600 2024-05-06 20:59:16.000000 playsound3-2.0.4/playsound3.egg-info/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1000)      258 2024-05-06 20:59:16.000000 playsound3-2.0.4/playsound3.egg-info/SOURCES.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)        1 2024-05-06 20:59:16.000000 playsound3-2.0.4/playsound3.egg-info/dependency_links.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-05-06 20:59:16.000000 playsound3-2.0.4/playsound3.egg-info/requires.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)       11 2024-05-06 20:59:16.000000 playsound3-2.0.4/playsound3.egg-info/top_level.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)      207 2024-05-06 12:41:28.000000 playsound3-2.0.4/pyproject.toml
--rw-r--r--   0 gaha      (1000) gaha      (1000)       38 2024-05-06 20:59:16.832440 playsound3-2.0.4/setup.cfg
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1365 2024-05-06 20:57:45.000000 playsound3-2.0.4/setup.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-05-06 23:37:50.700136 playsound3-2.1.0/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1155 2024-05-06 21:20:06.000000 playsound3-2.1.0/LICENSE
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     2724 2024-05-06 23:37:50.700136 playsound3-2.1.0/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1723 2024-05-06 23:35:58.000000 playsound3-2.1.0/README.md
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-05-06 23:37:50.700136 playsound3-2.1.0/playsound3/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       44 2024-05-06 14:32:01.000000 playsound3-2.1.0/playsound3/__init__.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     3898 2024-05-06 23:37:03.000000 playsound3-2.1.0/playsound3/playsound3.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-05-06 23:37:50.700136 playsound3-2.1.0/playsound3.egg-info/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     2724 2024-05-06 23:37:50.000000 playsound3-2.1.0/playsound3.egg-info/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      258 2024-05-06 23:37:50.000000 playsound3-2.1.0/playsound3.egg-info/SOURCES.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)        1 2024-05-06 23:37:50.000000 playsound3-2.1.0/playsound3.egg-info/dependency_links.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-05-06 23:37:50.000000 playsound3-2.1.0/playsound3.egg-info/requires.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       11 2024-05-06 23:37:50.000000 playsound3-2.1.0/playsound3.egg-info/top_level.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      207 2024-05-06 12:41:28.000000 playsound3-2.1.0/pyproject.toml
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       38 2024-05-06 23:37:50.700136 playsound3-2.1.0/setup.cfg
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1365 2024-05-06 23:36:21.000000 playsound3-2.1.0/setup.py
```

### Comparing `playsound3-2.0.4/PKG-INFO` & `playsound3-2.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playsound3
-Version: 2.0.4
+Version: 2.1.0
 Summary: Cross-platform library to play audio files
 Home-page: https://github.com/sjmikler/playsound3
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Keywords: sound playsound music wave wav mp3 media song play audio
 Classifier: License :: OSI Approved :: MIT License
@@ -19,21 +19,23 @@
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players :: MP3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pygobject; platform_system == "Linux"
 
-> This repository was initially forked from [TaylorSMarks/playsound](https://github.com/TaylorSMarks/playsound)
+> This repository was forked from [TaylorSMarks/playsound](https://github.com/TaylorSMarks/playsound)
 
-# Playsound3
+# playsound3
 
 [![PyPi version](https://img.shields.io/badge/dynamic/json?label=latest&query=info.version&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fplaysound3%2Fjson)](https://pypi.org/project/playsound3)
 [![PyPI license](https://img.shields.io/badge/dynamic/json?label=license&query=info.license&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fplaysound3%2Fjson)](https://pypi.org/project/playsound3)
 
+Cross platform library to play sound files in Python.
+
 ## Installation
 
 Install via pip:
 
 ```
 pip install playsound3
 ```
@@ -42,32 +44,35 @@
 
 Once installed, you can use the playsound function to play sound files:
 
 ```python
 from playsound3 import playsound
 
 playsound("/path/to/sound/file.mp3")
+
+# or use directly on URLs
+playsound("http://url/to/sound/file.mp3")
 ```
 
 ## Documentation
 
 The playsound module contains only one thing - the function (also named) playsound:
 
 ```python
 def playsound(sound, block: bool = True) -> None:
-    """Play a sound file using an audio player availabile on your system.
+    """Play a sound file using an audio backend availabile in your system.
 
     Args:
         sound: Path to the sound file. Can be either an str or pathlib.Path.
         block: If True, the function will block execution until the sound finishes playing.
     """
 ```
 
 It requires one argument - the path to the file with the sound you'd like to play.
-This should be a local file.
+This should be a local file or a URL.
 There's an optional second argument, block, which is set to True by default.
 Setting it to False makes the function run asynchronously.
 
 ## Supported systems
 
 * Linux, using GStreamer (built-in on Linux distributions)
 * Windows, using windll.winmm (built-in on Windows)
```

### Comparing `playsound3-2.0.4/README.md` & `playsound3-2.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-> This repository was initially forked from [TaylorSMarks/playsound](https://github.com/TaylorSMarks/playsound)
+> This repository was forked from [TaylorSMarks/playsound](https://github.com/TaylorSMarks/playsound)
 
-# Playsound3
+# playsound3
 
 [![PyPi version](https://img.shields.io/badge/dynamic/json?label=latest&query=info.version&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fplaysound3%2Fjson)](https://pypi.org/project/playsound3)
 [![PyPI license](https://img.shields.io/badge/dynamic/json?label=license&query=info.license&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fplaysound3%2Fjson)](https://pypi.org/project/playsound3)
 
+Cross platform library to play sound files in Python.
+
 ## Installation
 
 Install via pip:
 
 ```
 pip install playsound3
 ```
@@ -17,32 +19,35 @@
 
 Once installed, you can use the playsound function to play sound files:
 
 ```python
 from playsound3 import playsound
 
 playsound("/path/to/sound/file.mp3")
+
+# or use directly on URLs
+playsound("http://url/to/sound/file.mp3")
 ```
 
 ## Documentation
 
 The playsound module contains only one thing - the function (also named) playsound:
 
 ```python
 def playsound(sound, block: bool = True) -> None:
-    """Play a sound file using an audio player availabile on your system.
+    """Play a sound file using an audio backend availabile in your system.
 
     Args:
         sound: Path to the sound file. Can be either an str or pathlib.Path.
         block: If True, the function will block execution until the sound finishes playing.
     """
 ```
 
 It requires one argument - the path to the file with the sound you'd like to play.
-This should be a local file.
+This should be a local file or a URL.
 There's an optional second argument, block, which is set to True by default.
 Setting it to False makes the function run asynchronously.
 
 ## Supported systems
 
 * Linux, using GStreamer (built-in on Linux distributions)
 * Windows, using windll.winmm (built-in on Windows)
```

### Comparing `playsound3-2.0.4/playsound3/playsound3.py` & `playsound3-2.1.0/playsound3/playsound3.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,30 @@
+import atexit
 import ctypes
 import logging
-import os
 import platform
 import subprocess
+import tempfile
+import urllib.request
 import uuid
 from pathlib import Path
 from threading import Thread
-from urllib.request import pathname2url
 
 logger = logging.getLogger(__name__)
 
 SYSTEM = platform.system()
+DOWNLOAD_CACHE = dict()
 
 
 class PlaysoundException(Exception):
     pass
 
 
 def playsound(sound, block: bool = True) -> None:
-    """Play a sound file using an audio player availabile on your system.
+    """Play a sound file using an audio backend availabile in your system.
 
     Args:
         sound: Path to the sound file. Can be either an str or pathlib.Path.
         block: If True, the function will block execution until the sound finishes playing.
     """
     sound = _prepare_path(sound)
 
@@ -34,34 +36,38 @@
         func = _playsound_afplay
     else:
         raise PlaysoundException(f"Platform '{SYSTEM}' is not supported")
 
     if block:
         func(sound)
     else:
-        t = Thread(target=func, args=(sound,)).start()
+        t = Thread(target=func, args=(sound,), daemon=True).start()
 
 
 def _prepare_path(sound):
+    if sound.startswith(("http://", "https://")):
+        # To play file from URL, we download the file first to a temporary location
+        if sound not in DOWNLOAD_CACHE:
+            with tempfile.NamedTemporaryFile(delete=False, prefix="playsound3-") as f:
+                urllib.request.urlretrieve(sound, f.name)
+                DOWNLOAD_CACHE[sound] = f.name
+        sound = DOWNLOAD_CACHE[sound]
+
     path = Path(sound)
 
     if not path.exists():
         raise PlaysoundException(f"File not found: {sound}")
-
     return path.absolute().as_posix()
 
 
 def _playsound_gstreamer(sound):
     """Play a sound using gstreamer (built-in Linux)."""
 
-    if not sound.startswith(("http://", "https://", "file://")):
-        path = os.path.abspath(sound)
-        if not os.path.exists(path):
-            raise PlaysoundException(f"File not found: {path}")
-        sound = "file://" + pathname2url(path)
+    if not sound.startswith("file://"):
+        sound = "file://" + urllib.request.pathname2url(sound)
 
     import gi
 
     # Silences gi warning
     gi.require_version("Gst", "1.0")
 
     # GStreamer is included in all Linux distributions
@@ -109,7 +115,18 @@
     """Uses afplay utility (built-in macOS)."""
     logger.debug("afplay: starting playing %s", sound)
     try:
         subprocess.run(["afplay", sound], check=True)
     except subprocess.CalledProcessError as e:
         raise PlaysoundException(f"afplay failed to play sound: {e}")
     logger.debug("afplay: finishing play %s", sound)
+
+
+def _remove_cached_files(cache):
+    """Remove all files saved in the cache when the program ends."""
+    import os
+
+    for path in cache.values():
+        os.remove(path)
+
+
+atexit.register(_remove_cached_files, DOWNLOAD_CACHE)
```

### Comparing `playsound3-2.0.4/playsound3.egg-info/PKG-INFO` & `playsound3-2.1.0/playsound3.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playsound3
-Version: 2.0.4
+Version: 2.1.0
 Summary: Cross-platform library to play audio files
 Home-page: https://github.com/sjmikler/playsound3
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Keywords: sound playsound music wave wav mp3 media song play audio
 Classifier: License :: OSI Approved :: MIT License
@@ -19,21 +19,23 @@
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players :: MP3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pygobject; platform_system == "Linux"
 
-> This repository was initially forked from [TaylorSMarks/playsound](https://github.com/TaylorSMarks/playsound)
+> This repository was forked from [TaylorSMarks/playsound](https://github.com/TaylorSMarks/playsound)
 
-# Playsound3
+# playsound3
 
 [![PyPi version](https://img.shields.io/badge/dynamic/json?label=latest&query=info.version&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fplaysound3%2Fjson)](https://pypi.org/project/playsound3)
 [![PyPI license](https://img.shields.io/badge/dynamic/json?label=license&query=info.license&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fplaysound3%2Fjson)](https://pypi.org/project/playsound3)
 
+Cross platform library to play sound files in Python.
+
 ## Installation
 
 Install via pip:
 
 ```
 pip install playsound3
 ```
@@ -42,32 +44,35 @@
 
 Once installed, you can use the playsound function to play sound files:
 
 ```python
 from playsound3 import playsound
 
 playsound("/path/to/sound/file.mp3")
+
+# or use directly on URLs
+playsound("http://url/to/sound/file.mp3")
 ```
 
 ## Documentation
 
 The playsound module contains only one thing - the function (also named) playsound:
 
 ```python
 def playsound(sound, block: bool = True) -> None:
-    """Play a sound file using an audio player availabile on your system.
+    """Play a sound file using an audio backend availabile in your system.
 
     Args:
         sound: Path to the sound file. Can be either an str or pathlib.Path.
         block: If True, the function will block execution until the sound finishes playing.
     """
 ```
 
 It requires one argument - the path to the file with the sound you'd like to play.
-This should be a local file.
+This should be a local file or a URL.
 There's an optional second argument, block, which is set to True by default.
 Setting it to False makes the function run asynchronously.
 
 ## Supported systems
 
 * Linux, using GStreamer (built-in on Linux distributions)
 * Windows, using windll.winmm (built-in on Windows)
```

### Comparing `playsound3-2.0.4/setup.py` & `playsound3-2.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     return Path(__file__).parent / path
 
 
 long_description = package_relative_path("README.md").read_text(encoding="UTF-8")
 
 setup(
     name="playsound3",
-    version="2.0.4",
+    version="2.1.0",
     description="Cross-platform library to play audio files",
     url="https://github.com/sjmikler/playsound3",
     author="Szymon Mikler",
     author_email="sjmikler@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
```

