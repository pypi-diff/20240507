# Comparing `tmp/pylivestream-2.0.0.tar.gz` & `tmp/pylivestream-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylivestream-2.0.0.tar", last modified: Thu Dec  1 05:55:36 2022, max compression
+gzip compressed data, was "pylivestream-2.1.0.tar", last modified: Tue May  7 03:12:56 2024, max compression
```

## Comparing `pylivestream-2.0.0.tar` & `pylivestream-2.1.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2022-12-01 05:55:36.536646 pylivestream-2.0.0/
--rw-rw-rw-   0        0        0     9558 2021-06-04 20:42:30.000000 pylivestream-2.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0       28 2022-12-01 05:28:41.000000 pylivestream-2.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0    22404 2022-12-01 05:55:36.533641 pylivestream-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    10146 2022-12-01 05:47:49.000000 pylivestream-2.0.0/README.md
--rw-rw-rw-   0        0        0     1234 2022-12-01 05:55:00.000000 pylivestream-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-12-01 05:55:36.537691 pylivestream-2.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-12-01 05:55:36.327275 pylivestream-2.0.0/src/
-drwxrwxrwx   0        0        0        0 2022-12-01 05:55:36.408700 pylivestream-2.0.0/src/pylivestream/
--rw-rw-rw-   0        0        0      112 2022-12-01 04:57:39.000000 pylivestream-2.0.0/src/pylivestream/__init__.py
--rw-rw-rw-   0        0        0     2334 2022-12-01 04:57:39.000000 pylivestream-2.0.0/src/pylivestream/api.py
--rw-rw-rw-   0        0        0     9303 2022-12-01 04:57:39.000000 pylivestream-2.0.0/src/pylivestream/base.py
--rw-rw-rw-   0        0        0      720 2022-12-01 04:57:39.000000 pylivestream-2.0.0/src/pylivestream/camera.py
-drwxrwxrwx   0        0        0        0 2022-12-01 05:55:36.498853 pylivestream-2.0.0/src/pylivestream/data/
--rw-rw-rw-   0        0        0        0 2020-06-10 03:36:45.000000 pylivestream-2.0.0/src/pylivestream/data/__init__.py
--rw-rw-rw-   0        0        0   562810 2020-07-20 12:46:08.000000 pylivestream-2.0.0/src/pylivestream/data/bunny.avi
--rw-rw-rw-   0        0        0     8735 2020-07-20 12:46:08.000000 pylivestream-2.0.0/src/pylivestream/data/check4k.png
--rw-rw-rw-   0        0        0   147223 2020-06-10 03:16:46.000000 pylivestream-2.0.0/src/pylivestream/data/logo.png
--rw-rw-rw-   0        0        0    60959 2020-07-20 12:46:08.000000 pylivestream-2.0.0/src/pylivestream/data/orch.ogg
--rw-rw-rw-   0        0        0     5870 2020-07-20 12:46:08.000000 pylivestream-2.0.0/src/pylivestream/data/orch_short.ogg
--rw-rw-rw-   0        0        0     1250 2022-12-01 04:57:39.000000 pylivestream-2.0.0/src/pylivestream/data/pylivestream.json
--rw-rw-rw-   0        0        0     3717 2021-02-11 02:36:31.000000 pylivestream-2.0.0/src/pylivestream/ffmpeg.py
--rw-rw-rw-   0        0        0     3468 2022-12-01 04:57:39.000000 pylivestream-2.0.0/src/pylivestream/glob.py
--rw-rw-rw-   0        0        0     1186 2022-11-30 20:01:19.000000 pylivestream-2.0.0/src/pylivestream/loopfile.py
--rw-rw-rw-   0        0        0      869 2022-11-30 20:01:22.000000 pylivestream-2.0.0/src/pylivestream/microphone.py
--rw-rw-rw-   0        0        0     1218 2022-11-30 20:01:24.000000 pylivestream-2.0.0/src/pylivestream/screen.py
--rw-rw-rw-   0        0        0      627 2022-11-30 19:59:53.000000 pylivestream-2.0.0/src/pylivestream/screen2disk.py
--rw-rw-rw-   0        0        0    11798 2022-12-01 04:57:39.000000 pylivestream-2.0.0/src/pylivestream/stream.py
-drwxrwxrwx   0        0        0        0 2022-12-01 05:55:36.526857 pylivestream-2.0.0/src/pylivestream/tests/
--rw-rw-rw-   0        0        0     1022 2022-12-01 05:28:41.000000 pylivestream-2.0.0/src/pylivestream/tests/test_class.py
--rw-rw-rw-   0        0        0      229 2022-12-01 04:57:39.000000 pylivestream-2.0.0/src/pylivestream/tests/test_disk.py
--rw-rw-rw-   0        0        0     2756 2022-12-01 05:28:41.000000 pylivestream-2.0.0/src/pylivestream/tests/test_filein.py
--rw-rw-rw-   0        0        0     2082 2022-12-01 05:31:32.000000 pylivestream-2.0.0/src/pylivestream/tests/test_microphone.py
--rw-rw-rw-   0        0        0     1111 2022-12-01 05:28:41.000000 pylivestream-2.0.0/src/pylivestream/tests/test_screen.py
--rw-rw-rw-   0        0        0     1279 2022-12-01 05:28:41.000000 pylivestream-2.0.0/src/pylivestream/tests/test_webcam.py
--rw-rw-rw-   0        0        0     4001 2022-12-01 05:28:41.000000 pylivestream-2.0.0/src/pylivestream/utils.py
-drwxrwxrwx   0        0        0        0 2022-12-01 05:55:36.460691 pylivestream-2.0.0/src/pylivestream.egg-info/
--rw-rw-rw-   0        0        0    22404 2022-12-01 05:55:36.000000 pylivestream-2.0.0/src/pylivestream.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1044 2022-12-01 05:55:36.000000 pylivestream-2.0.0/src/pylivestream.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-01 05:55:36.000000 pylivestream-2.0.0/src/pylivestream.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2022-12-01 05:55:36.000000 pylivestream-2.0.0/src/pylivestream.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-12-01 05:55:36.000000 pylivestream-2.0.0/src/pylivestream.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:12:56.033656 pylivestream-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     9558 2024-05-07 03:12:48.000000 pylivestream-2.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 03:12:48.000000 pylivestream-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11423 2024-05-07 03:12:56.033656 pylivestream-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10199 2024-05-07 03:12:48.000000 pylivestream-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-07 03:12:48.000000 pylivestream-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 03:12:56.033656 pylivestream-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:12:56.025656 pylivestream-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:12:56.025656 pylivestream-2.1.0/src/pylivestream/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-07 03:12:48.000000 pylivestream-2.1.0/src/pylivestream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-07 03:12:48.000000 pylivestream-2.1.0/src/pylivestream/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-07 03:12:48.000000 pylivestream-2.1.0/src/pylivestream/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-07 03:12:48.000000 pylivestream-2.1.0/src/pylivestream/camera.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:12:56.029656 pylivestream-2.1.0/src/pylivestream/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:12:48.000000 pylivestream-2.1.0/src/pylivestream/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   562810 2024-05-07 03:12:48.000000 pylivestream-2.1.0/src/pylivestream/data/bunny.avi
+-rw-r--r--   0 runner    (1001) docker     (127)     8735 2024-05-07 03:12:48.000000 pylivestream-2.1.0/src/pylivestream/data/check4k.png
+-rw-r--r--   0 runner    (1001) docker     (127)   147223 2024-05-07 03:12:48.000000 pylivestream-2.1.0/src/pylivestream/data/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    60959 2024-05-07 03:12:48.000000 pylivestream-2.1.0/src/pylivestream/data/orch.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-07 03:12:48.000000 pylivestream-2.1.0/src/pylivestream/data/orch_short.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-07 03:12:48.000000 pylivestream-2.1.0/src/pylivestream/data/pylivestream.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-05-07 03:12:48.000000 pylivestream-2.1.0/src/pylivestream/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-07 03:12:48.000000 pylivestream-2.1.0/src/pylivestream/fglob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-07 03:12:48.000000 pylivestream-2.1.0/src/pylivestream/loopfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-07 03:12:48.000000 pylivestream-2.1.0/src/pylivestream/microphone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-07 03:12:48.000000 pylivestream-2.1.0/src/pylivestream/screen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-07 03:12:48.000000 pylivestream-2.1.0/src/pylivestream/screen2disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11918 2024-05-07 03:12:48.000000 pylivestream-2.1.0/src/pylivestream/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:12:56.029656 pylivestream-2.1.0/src/pylivestream/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-05-07 03:12:48.000000 pylivestream-2.1.0/src/pylivestream/tests/test_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-07 03:12:48.000000 pylivestream-2.1.0/src/pylivestream/tests/test_disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-07 03:12:48.000000 pylivestream-2.1.0/src/pylivestream/tests/test_filein.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-07 03:12:48.000000 pylivestream-2.1.0/src/pylivestream/tests/test_microphone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-07 03:12:48.000000 pylivestream-2.1.0/src/pylivestream/tests/test_screen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-07 03:12:48.000000 pylivestream-2.1.0/src/pylivestream/tests/test_webcam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-07 03:12:48.000000 pylivestream-2.1.0/src/pylivestream/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:12:56.029656 pylivestream-2.1.0/src/pylivestream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11423 2024-05-07 03:12:56.000000 pylivestream-2.1.0/src/pylivestream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-07 03:12:56.000000 pylivestream-2.1.0/src/pylivestream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 03:12:56.000000 pylivestream-2.1.0/src/pylivestream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-07 03:12:56.000000 pylivestream-2.1.0/src/pylivestream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 03:12:56.000000 pylivestream-2.1.0/src/pylivestream.egg-info/top_level.txt
```

### Comparing `pylivestream-2.0.0/LICENSE.txt` & `pylivestream-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pylivestream-2.0.0/README.md` & `pylivestream-2.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # Python scripted livestreaming using FFmpeg
 
 [![DOI](https://zenodo.org/badge/91214767.svg)](https://zenodo.org/badge/latestdoi/91214767)
 ![Actions Status](https://github.com/scivision/pylivestream/workflows/ci/badge.svg)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/scivision/PyLivestream.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/scivision/PyLivestream/context:python)
 [![pypi versions](https://img.shields.io/pypi/pyversions/PyLivestream.svg)](https://pypi.python.org/pypi/PyLivestream)
 [![PyPi Download stats](https://static.pepy.tech/badge/pylivestream)](https://pepy.tech/project/pylivestream)
 
 Streams to one or **multiple** streaming sites simultaneously, using pure object-oriented Python (no extra packages) and FFmpeg.
 Tested with `flake8`, `mypy` type checking and `pytest`.
-Python >= 3.9 is recommended for full capabilities.
 `visual_tests.py` is a quick check of several command line scripting scenarios on your laptop.
 FFmpeg is used from Python `subprocess` to stream to sites including:
 
 * Facebook Live  (requires FFmpeg >= 4.2 due to mandatory RTMPS)
 * YouTube Live
 * Twitch
 * also Ustream, Vimeo, Restream.io and more for streaming broadcasts.
@@ -64,14 +62,22 @@
 git clone https://github.com/scivision/PyLivestream
 
 cd PyLivestream
 
 python3 -m pip install -e .
 ```
 
+FFmpeg can be obtained like:
+
+* Windows: `winget install ffmpeg`
+* Linux: `sudo apt install ffmpeg`
+* MacOS: `brew install ffmpeg`
+
+If errors result from FFmpeg not in PATH environment variable, optionally set environment variable "FFMPEG_ROOT" to the directory containing FFmpeg executable.
+
 ## Configuration: pylivestream.json
 
 You can skip past this section to "stream start" if it's confusing.
 The defaults might work to get you started.
 
 The pylivestream.json file you create has parameters relevant to the live stream.
 We suggest copying the example
@@ -122,15 +128,15 @@
 
 ## API
 
 There are two ways to start a stream (assuming you've configured as per following sections).
 Both do the same thing.
 
 * command line
-  * python -m pylivestream.glob
+  * python -m pylivestream.fglob
   * python -m pylivestream.screen
   * python -m pylivestream.loopfile
   * python -m pylivestream.screen2disk
   * python -m pylivestream.camera
   * python -m pylivestream.microphone
 * `import pylivestream.api as pls` from within your Python script. For more information type `help(pls)` or `help(pls.stream_microphone)`
   * pls.stream_file()
```

### Comparing `pylivestream-2.0.0/pyproject.toml` & `pylivestream-2.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
+build-backend = "setuptools.build_meta"
 
 [project]
 name = "pylivestream"
-version = "2.0.0"
 description = "Livestream using FFmpeg to YouTube Live, Twitter, Facebook Live, Twitch, and more"
 keywords = ["youtube", "ffmpeg", "twitch", "twitter live", "facebook live", "restream.io"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Console",
   "Intended Audience :: End Users/Desktop",
+  "License :: OSI Approved :: Apache Software License",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3",
   "Topic :: Multimedia :: Graphics :: Capture :: Screen Capture",
   "Topic :: Multimedia :: Sound/Audio :: Capture/Recording",
   "Topic :: Multimedia :: Video :: Capture"
 ]
-license = {file = "LICENSE.txt"}
-dynamic = ["readme"]
-requires-python = ">=3.7"
+dynamic = ["readme", "version"]
+requires-python = ">=3.9"
+
+[tool.setuptools.dynamic]
+readme = {file = ["README.md"], content-type = "text/markdown"}
+version = {attr = "pylivestream.__version__"}
 
 [project.optional-dependencies]
 tests = ["pytest", "pytest-timeout"]
 lint = ["flake8", "flake8-bugbear", "flake8-builtins", "flake8-blind-except", "mypy"]
 captions = ["tinytag"]
 
-[tool.setuptools.dynamic]
-readme = {file = ["README.md"], content-type = "text/markdown"}
-
 [tool.black]
 line-length = 100
 
 [tool.mypy]
 files = ["src"]
 ignore_missing_imports = true
-strict_optional = false
-allow_redefinition = true
-show_error_context = false
-show_column_numbers = true
```

### Comparing `pylivestream-2.0.0/src/pylivestream/api.py` & `pylivestream-2.1.0/src/pylivestream/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 pls.microphone('twitch')
 """
 
 from __future__ import annotations
 from pathlib import Path
 
 from .base import FileIn, Microphone, SaveDisk, Camera
-from .glob import stream_files
+from .fglob import stream_files
 from .screen import stream_screen
 
 __all__ = [
     "stream_file",
     "stream_files",
     "stream_microphone",
     "stream_camera",
@@ -26,17 +26,17 @@
 ]
 
 
 def stream_file(
     ini_file: Path,
     websites: str | list[str],
     video_file: Path,
-    loop: bool = None,
+    loop: bool | None = None,
     assume_yes: bool = False,
-    timeout: float = None,
+    timeout: float | None = None,
 ):
     S = FileIn(ini_file, websites, infn=video_file, loop=loop, yes=assume_yes, timeout=timeout)
     sites: list[str] = list(S.streams.keys())
     # %% Go live
     if assume_yes:
         print(f"going live on {sites} with file {video_file}")
     else:
@@ -46,17 +46,17 @@
     S.golive()
 
 
 def stream_microphone(
     ini_file: Path,
     websites: list[str],
     *,
-    still_image: Path = None,
-    assume_yes: bool = False,
-    timeout: float = None,
+    still_image: Path | None = None,
+    assume_yes: bool | None = False,
+    timeout: float | None = None,
 ):
     """
     livestream audio, with still image background
     """
 
     s = Microphone(ini_file, websites, image=still_image, yes=assume_yes, timeout=timeout)
     sites = list(s.streams.keys())
@@ -66,15 +66,15 @@
     else:
         input(f"Press Enter to go live on {sites}.    Or Ctrl C to abort.")
 
     s.golive()
 
 
 def capture_screen(
-    ini_file: Path, *, out_file: Path, assume_yes: bool = False, timeout: float = None
+    ini_file: Path, *, out_file: Path, assume_yes: bool = False, timeout: float | None = None
 ):
 
     s = SaveDisk(ini_file, out_file, yes=assume_yes, timeout=timeout)
     # %%
     if assume_yes:
         print("saving screen capture to", s.outfn)
     else:
```

### Comparing `pylivestream-2.0.0/src/pylivestream/base.py` & `pylivestream-2.1.0/src/pylivestream/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             + ["-t", CHECKTIMEOUT]
             + self.videoIn(quick=True)
             + self.audioIn(quick=True)
             + ["-t", CHECKTIMEOUT]
             + ["-f", "null", "-"]  # camera needs at output
         )
 
-    def startlive(self, sinks: list[str] = None):
+    def startlive(self, sinks: list[str] | None = None):
         """
         start the stream(s)
         """
 
         if self.docheck:
             self.check_device()
 
@@ -137,15 +137,15 @@
             run(cmd)
 
         # %% stop the listener before starting the next process, or upon final process closing.
         if proc is not None and proc.poll() is None:
             proc.terminate()
         yield
 
-    def check_device(self, site: str = None) -> bool:
+    def check_device(self, site: str | None = None) -> bool:
         """
         requires stream to have been configured first.
         does a quick test stream to "null" to verify device is actually accessible
         """
         if not site:
             try:
                 site = self.site
@@ -247,15 +247,15 @@
         try:
             next(self.streams[unify_streams(self.streams)].startlive(sinks))
         except StopIteration:
             pass
 
 
 class SaveDisk(Stream):
-    def __init__(self, inifn: Path, outfn: Path = None, **kwargs):
+    def __init__(self, inifn: Path, outfn: Path | None = None, **kwargs):
         """
         records to disk screen capture with audio
 
         if not outfn, just cite command that would have run
         """
         super().__init__(inifn, site="file", vidsource="screen", **kwargs)
```

### Comparing `pylivestream-2.0.0/src/pylivestream/camera.py` & `pylivestream-2.1.0/src/pylivestream/camera.py`

 * *Files identical despite different names*

### Comparing `pylivestream-2.0.0/src/pylivestream/data/bunny.avi` & `pylivestream-2.1.0/src/pylivestream/data/bunny.avi`

 * *Files identical despite different names*

### Comparing `pylivestream-2.0.0/src/pylivestream/data/check4k.png` & `pylivestream-2.1.0/src/pylivestream/data/check4k.png`

 * *Files identical despite different names*

### Comparing `pylivestream-2.0.0/src/pylivestream/data/logo.png` & `pylivestream-2.1.0/src/pylivestream/data/logo.png`

 * *Files identical despite different names*

### Comparing `pylivestream-2.0.0/src/pylivestream/data/orch.ogg` & `pylivestream-2.1.0/src/pylivestream/data/orch.ogg`

 * *Files identical despite different names*

### Comparing `pylivestream-2.0.0/src/pylivestream/data/orch_short.ogg` & `pylivestream-2.1.0/src/pylivestream/data/orch_short.ogg`

 * *Files identical despite different names*

### Comparing `pylivestream-2.0.0/src/pylivestream/data/pylivestream.json` & `pylivestream-2.1.0/src/pylivestream/data/pylivestream.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8598214285714286%*

 * *Differences: {"'audio_codec'": "'aac'",*

 * * "'darwin'": "{'video_format': 'uyvy422'}",*

 * * "'linux'": "{'video_format': 'yuv420p'}",*

 * * "'video_codec'": "'libx264'",*

 * * "'win32'": "{'video_format': 'yuv420p'}"}*

```diff
@@ -1,30 +1,33 @@
 {
     "audio_bps": 128000,
+    "audio_codec": "aac",
     "audio_rate": 44100,
     "camera_fps": 30,
     "camera_size": [
         640,
         480
     ],
     "darwin": {
         "audio_chan": "default",
         "hcam": "avfoundation",
         "screen_chan": "1:0",
-        "vcap": "avfoundation"
+        "vcap": "avfoundation",
+        "video_format": "uyvy422"
     },
     "exe": "ffmpeg",
     "ffprobe_exe": "ffprobe",
     "linux": {
         "acap": "pulse",
         "audio_chan": "default",
         "camera_chan": "/dev/video0",
         "hcam": "v4l2",
         "screen_chan": ":0.0",
-        "vcap": "x11grab"
+        "vcap": "x11grab",
+        "video_format": "yuv420p"
     },
     "preset": "veryfast",
     "screencap_fps": 30,
     "screencap_origin": [
         50,
         30
     ],
@@ -52,16 +55,18 @@
         },
         "youtube": {
             "keyframe_sec": 2,
             "streamid": "xxxx-xxxx-xxxx-xxxx",
             "url": "rtmp://a.rtmp.youtube.com/live2"
         }
     },
+    "video_codec": "libx264",
     "win32": {
         "acap": "dshow",
         "audio_chan": "audio=Internal Microphone",
         "camera_chan": "video=Integrated Camera",
         "hcam": "dshow",
         "screen_chan": "desktop",
-        "vcap": "gdigrab"
+        "vcap": "gdigrab",
+        "video_format": "yuv420p"
     }
 }
```

### Comparing `pylivestream-2.0.0/src/pylivestream/ffmpeg.py` & `pylivestream-2.1.0/src/pylivestream/ffmpeg.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import typing as T
 import subprocess
 from time import sleep
 import os
 from pathlib import Path
 import shutil
 import json
+import functools
 
 
 class Ffmpeg:
     def __init__(self):
 
         self.ERROR = ["-loglevel", "error"]
         self.WARNING = ["-loglevel", "warning"]
@@ -18,28 +19,28 @@
         self.YES = ["-y"]
 
         # default 8, increasing can help avoid warnings
         self.QUEUE = ["-thread_queue_size", "8"]
 
         self.THROTTLE = "-re"
 
-    def timelimit(self, t: str | int | float) -> list[str]:
+    def timelimit(self, t: str | int | float | None) -> list[str]:
         if t is None:
             return []
 
         assert isinstance(t, (str, int, float))
 
         t = str(t)
 
         if len(t) > 0:
             return ["-t", str(t)]
         else:
             return []
 
-    def drawtext(self, text: str = None) -> list[str]:
+    def drawtext(self, text: str) -> list[str]:
         # fontfile=/path/to/font.ttf:
         if not text:  # None or '' or [] etc.
             return []
 
         fontcolor = "fontcolor=white"
         fontsize = "fontsize=24"
         box = "box=1"
@@ -62,19 +63,15 @@
         -timeout is the delay to wait for stream input before erroring.
 
         sleep: 0.2 not long enough. 0.3 worked, so set 0.5 for some margin.
         """
 
         TIMEOUT = 0.5
 
-        exe = shutil.which("ffplay")
-        if not exe:
-            raise FileNotFoundError("FFplay not found, cannot start listener")
-
-        cmd = [exe, "-loglevel", "error", "-timeout", "5", "-autoexit", "rtmp://localhost"]
+        cmd = [get_ffplay(), "-loglevel", "error", "-timeout", "5", "-autoexit", "rtmp://localhost"]
 
         print(
             "starting Localhost RTMP listener. \n\n",
             " ".join(cmd),
             "\n\n Press   q   in this terminal to end stream.",
         )
 
@@ -84,47 +81,57 @@
         #                                 '-i', 'rtmp://localhost', '-f', 'null', '-'],
         #                                stdout=subprocess.DEVNULL)
 
         sleep(TIMEOUT)
 
         return proc
 
-    def movingBG(self, bgfn: Path = None) -> list[str]:
+    def movingBG(self, bgfn: Path | None = None) -> list[str]:
         if not bgfn:
             return []
 
         bg = str(bgfn)
         if os.name == "nt":
             bg = bg.replace("\\", "/")  # for PureWindowsPath
 
         return ["-filter_complex", f"movie={bg}:loop=0,setpts=N/FRAME_RATE/TB"]
 
 
-def get_exe(exein: str) -> str:
-    """checks that host streaming program is installed"""
+@functools.cache
+def get_exe(name: str) -> str:
 
-    exe = str(Path(exein).expanduser())
-    # %% verify
-    if not shutil.which(exe):
-        raise FileNotFoundError(
-            f"""
+    for p in (os.environ.get("FFMPEG_ROOT"), None):
+        if exe := shutil.which(name, path=p):
+            return exe
 
+    raise FileNotFoundError(
+        f"""
 *** Must have FFmpeg + FFprobe installed to use PyLivestream.
 https://www.ffmpeg.org/download.html
 
-could not find {exein}
+could not find {name}
 """
-        )
+    )
+
+
+def get_ffmpeg() -> str:
+    return get_exe("ffmpeg")
+
+
+def get_ffplay() -> str:
+    return get_exe("ffplay")
+
 
-    return exe
+def get_ffprobe() -> str:
+    return get_exe("ffprobe")
 
 
-def get_meta(fn: Path, exein: str = None) -> dict[str, T.Any]:
+def get_meta(fn: Path, exein: str | None = None) -> dict[str, T.Any]:
     if not fn:  # audio-only
-        return None
+        return {}
 
     fn = Path(fn).expanduser()
 
     if not fn.is_file():
         raise FileNotFoundError(fn)
 
     exe = get_exe("ffprobe") if exein is None else exein
@@ -136,10 +143,10 @@
         "-print_format",
         "json",
         "-show_streams",
         "-show_format",
         str(fn),
     ]
 
-    ret = subprocess.check_output(cmd, universal_newlines=True)
+    ret = subprocess.check_output(cmd, text=True)
     # %% decode JSON from FFprobe
     return json.loads(ret)
```

### Comparing `pylivestream-2.0.0/src/pylivestream/glob.py` & `pylivestream-2.1.0/src/pylivestream/fglob.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 
 
 def stream_files(
     ini_file: Path,
     websites: list[str],
     *,
     video_path: Path,
-    glob: str = None,
+    glob: str | None = None,
     assume_yes: bool = False,
-    loop: bool = None,
-    shuffle: bool = None,
-    still_image: Path = None,
-    no_meta: bool = None,
-    timeout: float = None,
+    loop: bool = False,
+    shuffle: bool = False,
+    still_image: Path | None = None,
+    no_meta: bool = False,
+    timeout: float | None = None,
 ):
     # %% file / glob wranging
     flist = fileglob(video_path, glob)
 
     print("streaming these files. Be sure list is correct! \n")
     print("\n".join(map(str, flist)))
     print()
@@ -45,27 +45,27 @@
             playonce(flist, still_image, websites, ini_file, shuffle, usemeta, assume_yes, timeout)
     else:
         playonce(flist, still_image, websites, ini_file, shuffle, usemeta, assume_yes, timeout)
 
 
 def playonce(
     flist: list[Path],
-    image: Path,
+    image: Path | None,
     sites: list[str],
     inifn: Path,
     shuffle: bool,
     usemeta: bool,
     yes: bool,
-    timeout: float = None,
+    timeout: float | None = None,
 ):
 
     if shuffle:
         random.shuffle(flist)
 
-    caption: str
+    caption: str | None
 
     for f in flist:
         if usemeta and TinyTag:
             try:
                 caption = meta_caption(TinyTag.get(str(f)))
                 print(caption)
             except LookupError:
@@ -76,15 +76,15 @@
         s = FileIn(
             inifn, sites, infn=f, loop=False, image=image, caption=caption, yes=yes, timeout=timeout
         )
 
         s.golive()
 
 
-def fileglob(path: Path, glob: str) -> list[Path]:
+def fileglob(path: Path, glob: str | None) -> list[Path]:
 
     path = Path(path).expanduser()
 
     if not glob:
         glob = "*.avi"
 
     if path.is_dir():
```

### Comparing `pylivestream-2.0.0/src/pylivestream/loopfile.py` & `pylivestream-2.1.0/src/pylivestream/loopfile.py`

 * *Files identical despite different names*

### Comparing `pylivestream-2.0.0/src/pylivestream/microphone.py` & `pylivestream-2.1.0/src/pylivestream/microphone.py`

 * *Files identical despite different names*

### Comparing `pylivestream-2.0.0/src/pylivestream/screen.py` & `pylivestream-2.1.0/src/pylivestream/screen.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import signal
 import argparse
 
 from .base import Screenshare
 
 
 def stream_screen(
-    ini_file: Path, websites: list[str], *, assume_yes: bool = False, timeout: float = None
+    ini_file: Path, websites: list[str], *, assume_yes: bool = False, timeout: float | None = None
 ):
 
     S = Screenshare(ini_file, websites, yes=assume_yes, timeout=timeout)
     sites: list[str] = list(S.streams.keys())
     # %% Go live
     if assume_yes:
         print("going live on", sites)
```

### Comparing `pylivestream-2.0.0/src/pylivestream/screen2disk.py` & `pylivestream-2.1.0/src/pylivestream/screen2disk.py`

 * *Files identical despite different names*

### Comparing `pylivestream-2.0.0/src/pylivestream/stream.py` & `pylivestream-2.1.0/src/pylivestream/stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,27 +32,24 @@
         self.loglevel: list[str] = self.F.INFO if kwargs.get("verbose") else self.F.ERROR
 
         self.inifn: Path = Path(inifn).expanduser().resolve(strict=True)
 
         self.site: str = site
         self.vidsource = kwargs.get("vidsource")
 
-        if kwargs.get("image"):
-            self.image = Path(kwargs["image"]).expanduser()
-        else:
-            self.image = None
+        self.image = Path(kwargs["image"]).expanduser() if kwargs.get("image") else None
 
-        self.loop: bool = kwargs.get("loop")
+        self.loop: bool = kwargs.get("loop", False)
 
         self.infn = Path(kwargs["infn"]).expanduser() if kwargs.get("infn") else None
         self.yes: list[str] = self.F.YES if kwargs.get("yes") else []
 
         self.queue: list[str] = []  # self.F.QUEUE
 
-        self.caption: str = kwargs.get("caption")
+        self.caption: str = kwargs.get("caption", "")
 
         self.timelimit: list[str] = self.F.timelimit(kwargs.get("timeout"))
 
     def osparam(self, fn: Path) -> None:
         """load OS specific config"""
 
         fn = Path(fn).expanduser().resolve(strict=True)
@@ -76,32 +73,32 @@
         try:
             sitecfg = C["sites"][self.site]
         except KeyError:
             raise KeyError(f"No config sites: {self.site} in {fn}")
 
         if self.vidsource == "camera":
             self.res: list[str] = C.get("camera_size")
-            self.fps: float = C.get("camera_fps")
+            self.fps: float | None = C.get("camera_fps")
             self.movingimage = self.staticimage = False
         elif self.vidsource == "screen":
             self.res = C.get("screencap_size")
             self.fps = C.get("screencap_fps")
             self.origin: list[str] = C.get("screencap_origin", [1, 1])
             self.movingimage = self.staticimage = False
+        elif self.image:  # audio-only stream + background image
+            self.res = utils.get_resolution(self.image, self.probeexe)
+            self.fps = utils.get_framerate(self.infn, self.probeexe)
         elif self.vidsource == "file":  # streaming video from a file
             self.res = utils.get_resolution(self.infn, self.probeexe)
             self.fps = utils.get_framerate(self.infn, self.probeexe)
-        elif self.vidsource is None and self.image:  # audio-only stream + background image
-            self.res = utils.get_resolution(self.image, self.probeexe)
-            self.fps = utils.get_framerate(self.infn, self.probeexe)
         else:  # audio-only
-            self.res = None
+            self.res = []
             self.fps = None
 
-        if self.res is not None and len(self.res) != 2:
+        if self.res and len(self.res) != 2:
             raise ValueError(f"need height, width of video resolution, I have: {self.res}")
 
         self.audio_rate: str = C.get("audio_rate")
         self.preset: str = C.get("preset")
 
         if not self.timelimit:
             self.timelimit = self.F.timelimit(sitecfg.get("timelimit"))
@@ -112,14 +109,18 @@
         self.audio_chan: str = syscfg.get("audio_chan")
 
         self.vcap: str = syscfg.get("vcap")
         self.acap: str = syscfg.get("acap")
 
         self.hcam: str = syscfg.get("hcam")
 
+        self.video_codec = C.get("video_codec")
+        self.audio_codec = C.get("audio_codec")
+        self.video_format = syscfg.get("video_format")
+
         self.video_kbps: int = sitecfg.get("video_kbps")
         self.audio_bps: str = sitecfg.get("audio_bps")
 
         self.keyframe_sec: int = sitecfg.get("keyframe_sec")
 
         self.url: str = sitecfg.get("url")
         self.streamid: str = sitecfg.get("streamid", "")
@@ -129,34 +130,33 @@
         config video input
         """
 
         if self.vidsource == "screen":
             v = self.screengrab(quick)
             if sys.platform == "darwin":
                 # not for files "option pixel_format not found"
-                v = ["-pix_fmt", "uyvy422"] + v
+                v = ["-pix_fmt", self.video_format] + v
         elif self.vidsource == "camera":
             v = self.camera(quick)
             if sys.platform == "darwin":
                 # not for files "option pixel_format not found"
-                v = ["-pix_fmt", "uyvy422"] + v
+                v = ["-pix_fmt", self.video_format] + v
         elif self.vidsource is None or self.vidsource == "file":
             v = self.filein(quick)
         else:
             raise ValueError(f"unknown vidsource {self.vidsource}")
 
         return v
 
     def videoOut(self) -> list[str]:
         """
         configure video output
         """
 
-        vid_format = "uyvy422" if sys.platform == "darwin" else "yuv420p"
-        v: list[str] = ["-codec:v", "libx264", "-pix_fmt", vid_format]
+        v: list[str] = ["-codec:v", self.video_codec, "-pix_fmt", self.video_format]
         # %% set frames/sec, bitrate and keyframe interval
         """
          DON'T DO THIS.
          It makes keyframes/bitrate far off from what streaming sites want
          v += ['-tune', 'stillimage']
 
          The settings below still save video/data bandwidth for the still image
@@ -211,26 +211,33 @@
         https://support.google.com/youtube/answer/2853702?hl=en
         https://www.facebook.com/facebookmedia/get-started/live
         """
 
         if not (self.audio_bps and self.acap and self.audio_chan and self.audio_rate):
             return []
 
-        return ["-codec:a", "aac", "-b:a", str(self.audio_bps), "-ar", str(self.audio_rate)]
+        return [
+            "-codec:a",
+            self.audio_codec,
+            "-b:a",
+            str(self.audio_bps),
+            "-ar",
+            str(self.audio_rate),
+        ]
 
     def video_bitrate(self) -> None:
         """
         get "best" video bitrate.
         Based on YouTube Live minimum specified stream rate.
         """
 
         if self.video_kbps:  # per-site override
             return
 
-        if self.res is not None:
+        if self.res:
             x: int = int(self.res[1])
         elif self.vidsource is None or self.vidsource == "file":
             logging.info("assuming 480p input.")
             x = 480
         else:
             raise ValueError(
                 """
```

### Comparing `pylivestream-2.0.0/src/pylivestream/tests/test_filein.py` & `pylivestream-2.1.0/src/pylivestream/tests/test_filein.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 sites = ["youtube", "facebook"]
 TIMEOUT = 30
 CI = os.environ.get("CI", None) in ("true", "True")
 ini = Path(__file__).parents[1] / "data/pylivestream.json"
 
 
-@pytest.mark.skipif(sys.version_info < (3, 9), reason="python >= 3.9 required")
 def test_props():
 
     with importlib.resources.as_file(
         importlib.resources.files("pylivestream.data").joinpath("bunny.avi")
     ) as fn:
         S = pls.FileIn(ini, websites=sites, infn=fn)
         for s in S.streams:
@@ -27,56 +26,59 @@
 
             if int(S.streams[s].res[1]) == 480:
                 assert S.streams[s].video_kbps == 500
             elif int(S.streams[s].res[1]) == 720:
                 assert S.streams[s].video_kbps == 1800
 
 
-@pytest.mark.skipif(sys.version_info < (3, 9), reason="python >= 3.9 required")
 def test_audio():
 
-    with importlib.resources.as_file(
-        importlib.resources.files("pylivestream.data").joinpath("logo.png")
-    ) as logo, importlib.resources.as_file(
-        importlib.resources.files("pylivestream.data").joinpath("orch_short.ogg")
-    ) as fn:
+    with (
+        importlib.resources.as_file(
+            importlib.resources.files("pylivestream.data").joinpath("logo.png")
+        ) as logo,
+        importlib.resources.as_file(
+            importlib.resources.files("pylivestream.data").joinpath("orch_short.ogg")
+        ) as fn,
+    ):
         S = pls.FileIn(ini, websites=sites, infn=fn, image=logo)
         for s in S.streams:
             assert "-re" in S.streams[s].cmd
             assert S.streams[s].fps is None
 
-            assert S.streams[s].video_kbps == 400
+            assert S.streams[s].video_kbps == 800
 
 
 @pytest.mark.timeout(TIMEOUT)
 @pytest.mark.skipif(CI, reason="CI has no audio hardware typically")
-@pytest.mark.skipif(sys.version_info < (3, 9), reason="python >= 3.9 required")
 def test_simple():
     """stream to localhost"""
-    with importlib.resources.as_file(
-        importlib.resources.files("pylivestream.data").joinpath("logo.png")
-    ) as logo, importlib.resources.as_file(
-        importlib.resources.files("pylivestream.data").joinpath("orch_short.ogg")
-    ) as fn:
+    with (
+        importlib.resources.as_file(
+            importlib.resources.files("pylivestream.data").joinpath("logo.png")
+        ) as logo,
+        importlib.resources.as_file(
+            importlib.resources.files("pylivestream.data").joinpath("orch_short.ogg")
+        ) as fn,
+    ):
         S = pls.FileIn(ini, websites="localhost", infn=fn, image=logo, yes=True, timeout=5)
 
         S.golive()
 
 
 @pytest.mark.skipif(CI, reason="CI has no audio hardware typically")
-@pytest.mark.skipif(sys.version_info < (3, 9), reason="python >= 3.9 required")
 def test_script():
     with importlib.resources.as_file(
         importlib.resources.files("pylivestream.data").joinpath("bunny.avi")
     ) as fn:
         subprocess.check_call(
             [
                 sys.executable,
                 "-m",
-                "pylivestream.glob",
+                "pylivestream.fglob",
                 str(fn),
                 "localhost",
                 str(ini),
                 "--yes",
                 "--timeout",
                 "5",
             ],
```

### Comparing `pylivestream-2.0.0/src/pylivestream/tests/test_microphone.py` & `pylivestream-2.1.0/src/pylivestream/tests/test_microphone.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 TIMEOUT = 30
 CI = os.environ.get("CI", None) in ("true", "True")
 WSL = "Microsoft" in platform.uname().release
 ini = Path(__file__).parents[1] / "data/pylivestream.json"
 
 
-@pytest.mark.skipif(sys.version_info < (3, 9), reason="python >= 3.9 required")
 def test_microphone_props():
 
     with importlib.resources.as_file(
         importlib.resources.files("pylivestream.data").joinpath("logo.png")
     ) as logo:
         S = pls.Microphone(ini, websites=sites, image=logo)
 
@@ -31,15 +30,14 @@
             assert "-re" not in S.streams[s].cmd
             assert S.streams[s].fps is None
             assert S.streams[s].res == [720, 540]
 
             assert S.streams[s].video_kbps == 800
 
 
-@pytest.mark.skipif(sys.version_info < (3, 9), reason="python >= 3.9 required")
 def test_microphone_image():
 
     with importlib.resources.as_file(
         importlib.resources.files("pylivestream.data").joinpath("check4k.png")
     ) as img:
         S = pls.Microphone(ini, websites=sites, image=img)
```

### Comparing `pylivestream-2.0.0/src/pylivestream/tests/test_screen.py` & `pylivestream-2.1.0/src/pylivestream/tests/test_screen.py`

 * *Files identical despite different names*

### Comparing `pylivestream-2.0.0/src/pylivestream/tests/test_webcam.py` & `pylivestream-2.1.0/src/pylivestream/tests/test_webcam.py`

 * *Files identical despite different names*

### Comparing `pylivestream-2.0.0/src/pylivestream/utils.py` & `pylivestream-2.1.0/src/pylivestream/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import annotations
 import logging
 import contextlib
 import subprocess
 from pathlib import Path
 import sys
 import importlib.resources
-import shutil
 
-from .ffmpeg import get_meta
+from .ffmpeg import get_meta, get_ffplay
 
 
 def run(cmd: list[str]):
     """
     shell=True for Windows seems necessary to specify devices enclosed by "" quotes
     """
 
@@ -24,15 +23,15 @@
 
 
 """
 This is an error-tolerant way; we haven't found it necessary.
 I don't like putting enormous amounts in a PIPE, this can be unstable.
 Better to let users know there's a problem.
 
-    ret = subprocess.run(cmd, stderr=subprocess.PIPE, universal_newlines=True)
+    ret = subprocess.run(cmd, stderr=subprocess.PIPE, text=True)
 
     if ret.returncode != 0:
         if "Connection reset by peer" in ret.stderr:
             logging.info('input stream (from your computer) ended.')
         else:
             logging.error(ret.stderr)
 """
@@ -45,35 +44,28 @@
     except subprocess.CalledProcessError:
         logging.critical(f'device not available, test command failed: \n {" ".join(cmd)}')
         ok = False
 
     return ok
 
 
-def check_display(fn: Path = None) -> bool:
+def check_display(fn: Path | None = None) -> bool:
     """see if it's possible to display something with a test file"""
 
-    exe = shutil.which("ffplay")
-
-    if not exe:
-        raise FileNotFoundError("FFplay not found")
-
     def _check_disp(fn: Path | contextlib.AbstractContextManager[Path]) -> int:
-        cmd = [exe, "-loglevel", "error", "-t", "1.0", "-autoexit", str(fn)]
+        cmd = [get_ffplay(), "-loglevel", "error", "-t", "1.0", "-autoexit", str(fn)]
         return subprocess.run(cmd, timeout=10).returncode
 
     if fn:
         ret = _check_disp(fn)
-    elif sys.version_info >= (3, 9):
+    else:
         with importlib.resources.as_file(
             importlib.resources.files(f"{__package__}.data").joinpath("logo.png")
         ) as f:
             ret = _check_disp(f)
-    else:
-        return None
 
     return ret == 0
 
 
 def meta_caption(meta) -> str:
     """makes text from metadata for captioning video"""
     caption = ""
@@ -87,15 +79,15 @@
         caption += meta.artist
     except (TypeError, LookupError, AttributeError):
         pass
 
     return caption
 
 
-def get_resolution(fn: Path, exe: str = None) -> list[str]:
+def get_resolution(fn: Path | None, exe: str | None = None) -> list[str]:
     """
     get resolution (widthxheight) of video file
     http://trac.ffmpeg.org/wiki/FFprobeTips#WidthxHeight
 
     FFprobe gets resolution from the first video stream in the file it finds.
 
     inputs:
@@ -105,30 +97,33 @@
     outputs:
     -------
     res:  (width,height) in pixels of the video
 
     if not a video file, None is returned.
     """
 
+    if fn is None:
+        return []
+
     meta = get_meta(fn, exe)
-    if meta is None:
-        return None
+    if not meta:
+        return []
 
-    res = None
+    res = []
 
     for s in meta["streams"]:
         if s["codec_type"] != "video":
             continue
         res = [s["width"], s["height"]]
         break
 
     return res
 
 
-def get_framerate(fn: Path, exe: str = None) -> float:
+def get_framerate(fn: Path | None, exe: str | None = None) -> float | None:
     """
     get framerate of video file
     http://trac.ffmpeg.org/wiki/FFprobeTips#FrameRate
 
     FFprobe gets framerate from the first video stream in the file it finds.
 
     Parameters
@@ -140,16 +135,19 @@
 
     Returns
     -------
     fps: float
         video framerate (frames/second). If not a video file, None is returned.
     """
 
+    if fn is None:
+        return None
+
     meta = get_meta(fn, exe)
-    if meta is None:
+    if not meta:
         return None
 
     fps = None
 
     for s in meta["streams"]:
         if s["codec_type"] != "video":
             continue
```

### Comparing `pylivestream-2.0.0/src/pylivestream.egg-info/SOURCES.txt` & `pylivestream-2.1.0/src/pylivestream.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 README.md
 pyproject.toml
 src/pylivestream/__init__.py
 src/pylivestream/api.py
 src/pylivestream/base.py
 src/pylivestream/camera.py
 src/pylivestream/ffmpeg.py
-src/pylivestream/glob.py
+src/pylivestream/fglob.py
 src/pylivestream/loopfile.py
 src/pylivestream/microphone.py
 src/pylivestream/screen.py
 src/pylivestream/screen2disk.py
 src/pylivestream/stream.py
 src/pylivestream/utils.py
 src/pylivestream.egg-info/PKG-INFO
```

