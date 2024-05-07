# Comparing `tmp/playsound3-2.1.0.tar.gz` & `tmp/playsound3-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playsound3-2.1.0.tar", last modified: Mon May  6 23:37:50 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `playsound3-2.1.0.tar` & `playsound3-2.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-05-06 23:37:50.700136 playsound3-2.1.0/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1155 2024-05-06 21:20:06.000000 playsound3-2.1.0/LICENSE
--rw-r--r--   0 gaha      (1000) gaha      (1000)     2724 2024-05-06 23:37:50.700136 playsound3-2.1.0/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1723 2024-05-06 23:35:58.000000 playsound3-2.1.0/README.md
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-05-06 23:37:50.700136 playsound3-2.1.0/playsound3/
--rw-r--r--   0 gaha      (1000) gaha      (1000)       44 2024-05-06 14:32:01.000000 playsound3-2.1.0/playsound3/__init__.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     3898 2024-05-06 23:37:03.000000 playsound3-2.1.0/playsound3/playsound3.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-05-06 23:37:50.700136 playsound3-2.1.0/playsound3.egg-info/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     2724 2024-05-06 23:37:50.000000 playsound3-2.1.0/playsound3.egg-info/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1000)      258 2024-05-06 23:37:50.000000 playsound3-2.1.0/playsound3.egg-info/SOURCES.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)        1 2024-05-06 23:37:50.000000 playsound3-2.1.0/playsound3.egg-info/dependency_links.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-05-06 23:37:50.000000 playsound3-2.1.0/playsound3.egg-info/requires.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)       11 2024-05-06 23:37:50.000000 playsound3-2.1.0/playsound3.egg-info/top_level.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)      207 2024-05-06 12:41:28.000000 playsound3-2.1.0/pyproject.toml
--rw-r--r--   0 gaha      (1000) gaha      (1000)       38 2024-05-06 23:37:50.700136 playsound3-2.1.0/setup.cfg
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1365 2024-05-06 23:36:21.000000 playsound3-2.1.0/setup.py
+-rwxr-xr-x   0        0        0      104 2020-02-02 00:00:00.000000 playsound3-2.1.1/script_release.sh
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 playsound3-2.1.1/.idea/.gitignore
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 playsound3-2.1.1/.idea/misc.xml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 playsound3-2.1.1/.idea/modules.xml
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 playsound3-2.1.1/.idea/playsound3.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 playsound3-2.1.1/.idea/vcs.xml
+-rw-r--r--   0        0        0    15985 2020-02-02 00:00:00.000000 playsound3-2.1.1/.idea/workspace.xml
+-rw-r--r--   0        0        0     9348 2020-02-02 00:00:00.000000 playsound3-2.1.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 playsound3-2.1.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 playsound3-2.1.1/playsound3/__init__.py
+-rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 playsound3-2.1.1/playsound3/playsound3.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 playsound3-2.1.1/.gitignore
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 playsound3-2.1.1/LICENSE
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 playsound3-2.1.1/README.md
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 playsound3-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 playsound3-2.1.1/PKG-INFO
```

### Comparing `playsound3-2.1.0/LICENSE` & `playsound3-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `playsound3-2.1.0/PKG-INFO` & `playsound3-2.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,36 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: playsound3
-Version: 2.1.0
+Version: 2.1.1
 Summary: Cross-platform library to play audio files
-Home-page: https://github.com/sjmikler/playsound3
-Author: Szymon Mikler
-Author-email: sjmikler@gmail.com
-License: MIT
-Keywords: sound playsound music wave wav mp3 media song play audio
+Project-URL: Repository, https://github.com/sjmikler/playsound3
+Project-URL: Issues, https://github.com/sjmikler/playsound3/issues
+Project-URL: Documentation, https://github.com/sjmikler/playsound3?tab=readme-ov-file#documentation
+Author-email: Szymon Mikler <sjmikler@gmail.com>, Taylor Marks <taylor@marksfam.com>
+Maintainer-email: Szymon Mikler <sjmikler@gmail.com>
+License: MIT License
+License-File: LICENSE
+Keywords: audio,media,mp3,music,play,playsound,song,sound,wav,wave
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Multimedia :: Sound/Audio :: MIDI
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players :: MP3
 Requires-Python: >=3.7
+Requires-Dist: pygobject; platform_system == 'Linux'
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pygobject; platform_system == "Linux"
 
 > This repository was forked from [TaylorSMarks/playsound](https://github.com/TaylorSMarks/playsound)
 
 # playsound3
 
 [![PyPi version](https://img.shields.io/badge/dynamic/json?label=latest&query=info.version&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fplaysound3%2Fjson)](https://pypi.org/project/playsound3)
 [![PyPI license](https://img.shields.io/badge/dynamic/json?label=license&query=info.license&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fplaysound3%2Fjson)](https://pypi.org/project/playsound3)
@@ -71,9 +76,9 @@
 This should be a local file or a URL.
 There's an optional second argument, block, which is set to True by default.
 Setting it to False makes the function run asynchronously.
 
 ## Supported systems
 
 * Linux, using GStreamer (built-in on Linux distributions)
-* Windows, using windll.winmm (built-in on Windows)
+* Windows, using winmm.dll (built-in on Windows)
 * OS X, using afplay utility (built-in on OS X)
```

### Comparing `playsound3-2.1.0/README.md` & `playsound3-2.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -46,9 +46,9 @@
 This should be a local file or a URL.
 There's an optional second argument, block, which is set to True by default.
 Setting it to False makes the function run asynchronously.
 
 ## Supported systems
 
 * Linux, using GStreamer (built-in on Linux distributions)
-* Windows, using windll.winmm (built-in on Windows)
+* Windows, using winmm.dll (built-in on Windows)
 * OS X, using afplay utility (built-in on OS X)
```

### Comparing `playsound3-2.1.0/playsound3/playsound3.py` & `playsound3-2.1.1/playsound3/playsound3.py`

 * *Files identical despite different names*

### Comparing `playsound3-2.1.0/setup.py` & `playsound3-2.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,54 @@
-from pathlib import Path
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "playsound3"
+version = "2.1.1"
+requires-python = ">=3.7"
+authors = [
+    { name = "Szymon Mikler", email = "sjmikler@gmail.com" },
+    { name = "Taylor Marks", email = "taylor@marksfam.com" },
+]
+maintainers = [
+    { name = "Szymon Mikler", email = "sjmikler@gmail.com" },
+]
+description = "Cross-platform library to play audio files"
+readme = { file = "README.md", content-type = "text/markdown" }
+license = { text = "MIT License" }
+keywords = ["audio", "sound", "song", "play", "media", "playsound", "music", "wave", "wav", "mp3"]
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Topic :: Multimedia :: Sound/Audio :: MIDI",
+    "Topic :: Multimedia :: Sound/Audio :: Players",
+    "Topic :: Multimedia :: Sound/Audio :: Players :: MP3",
+    "Operating System :: OS Independent",
+]
+dependencies = [
+    "pygobject; platform_system=='Linux'",
+]
+
+[project.urls]
+Repository = "https://github.com/sjmikler/playsound3"
+Issues = "https://github.com/sjmikler/playsound3/issues"
+Documentation = "https://github.com/sjmikler/playsound3?tab=readme-ov-file#documentation"
+
+##################################
+## Formatting and testing tools ##
+##################################
+
+[tool.isort]
+profile = "black"
+line_length = 120
 
-from setuptools import find_packages, setup
-
-
-def package_relative_path(path):
-    return Path(__file__).parent / path
-
-
-long_description = package_relative_path("README.md").read_text(encoding="UTF-8")
-
-setup(
-    name="playsound3",
-    version="2.1.0",
-    description="Cross-platform library to play audio files",
-    url="https://github.com/sjmikler/playsound3",
-    author="Szymon Mikler",
-    author_email="sjmikler@gmail.com",
-    license="MIT",
-    classifiers=[
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-        "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12",
-        "Topic :: Multimedia :: Sound/Audio :: MIDI",
-        "Topic :: Multimedia :: Sound/Audio :: Players",
-        "Topic :: Multimedia :: Sound/Audio :: Players :: MP3",
-    ],
-    keywords="sound playsound music wave wav mp3 media song play audio",
-    packages=find_packages(),
-    python_requires=">=3.7",
-    install_requires=[
-        "pygobject; platform_system=='Linux'",
-    ],
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-)
+[tool.black]
+line_length = 120
```

