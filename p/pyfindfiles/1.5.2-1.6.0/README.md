# Comparing `tmp/pyfindfiles-1.5.2.tar.gz` & `tmp/pyfindfiles-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfindfiles-1.5.2.tar", last modified: Mon Jan  2 20:26:33 2023, max compression
+gzip compressed data, was "pyfindfiles-1.6.0.tar", last modified: Mon May  6 23:20:16 2024, max compression
```

## Comparing `pyfindfiles-1.5.2.tar` & `pyfindfiles-1.6.0.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-01-02 20:26:33.701869 pyfindfiles-1.5.2/
--rw-rw-rw-   0        0        0     1081 2023-01-02 19:10:43.000000 pyfindfiles-1.5.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1822 2023-01-02 20:26:33.700672 pyfindfiles-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     1085 2023-01-02 20:06:16.000000 pyfindfiles-1.5.2/README.md
--rw-rw-rw-   0        0        0     1288 2023-01-02 20:23:55.000000 pyfindfiles-1.5.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-02 20:26:33.702375 pyfindfiles-1.5.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-01-02 20:26:33.638889 pyfindfiles-1.5.2/src/
-drwxrwxrwx   0        0        0        0 2023-01-02 20:26:33.661738 pyfindfiles-1.5.2/src/pyfindfiles/
--rw-rw-rw-   0        0        0      124 2023-01-02 20:06:36.000000 pyfindfiles-1.5.2/src/pyfindfiles/__init__.py
--rw-rw-rw-   0        0        0     3961 2023-01-02 20:06:52.000000 pyfindfiles-1.5.2/src/pyfindfiles/__main__.py
--rw-rw-rw-   0        0        0     1486 2023-01-02 20:07:30.000000 pyfindfiles-1.5.2/src/pyfindfiles/async_vid.py
--rw-rw-rw-   0        0        0     1080 2023-01-02 20:22:15.000000 pyfindfiles-1.5.2/src/pyfindfiles/project.py
-drwxrwxrwx   0        0        0        0 2023-01-02 20:26:33.692767 pyfindfiles-1.5.2/src/pyfindfiles/tests/
--rw-rw-rw-   0        0        0        0 2023-01-02 20:05:32.000000 pyfindfiles-1.5.2/src/pyfindfiles/tests/__init__.py
--rw-rw-rw-   0        0        0      201 2023-01-02 20:05:32.000000 pyfindfiles-1.5.2/src/pyfindfiles/tests/test_project.py
--rw-rw-rw-   0        0        0      967 2023-01-02 20:05:32.000000 pyfindfiles-1.5.2/src/pyfindfiles/tests/test_text.py
--rw-rw-rw-   0        0        0      853 2023-01-02 20:05:32.000000 pyfindfiles-1.5.2/src/pyfindfiles/tests/test_video.py
--rw-rw-rw-   0        0        0     1731 2023-01-02 20:22:15.000000 pyfindfiles-1.5.2/src/pyfindfiles/text.py
--rw-rw-rw-   0        0        0     1112 2023-01-02 20:08:36.000000 pyfindfiles-1.5.2/src/pyfindfiles/vid.py
-drwxrwxrwx   0        0        0        0 2023-01-02 20:26:33.692767 pyfindfiles-1.5.2/src/pyfindfiles.egg-info/
--rw-rw-rw-   0        0        0     1822 2023-01-02 20:26:33.000000 pyfindfiles-1.5.2/src/pyfindfiles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      574 2023-01-02 20:26:33.000000 pyfindfiles-1.5.2/src/pyfindfiles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-02 20:26:33.000000 pyfindfiles-1.5.2/src/pyfindfiles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      147 2023-01-02 20:26:33.000000 pyfindfiles-1.5.2/src/pyfindfiles.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      125 2023-01-02 20:26:33.000000 pyfindfiles-1.5.2/src/pyfindfiles.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-01-02 20:26:33.000000 pyfindfiles-1.5.2/src/pyfindfiles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:20:16.847190 pyfindfiles-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-06 23:20:13.000000 pyfindfiles-1.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-06 23:20:16.847190 pyfindfiles-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-06 23:20:13.000000 pyfindfiles-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-06 23:20:13.000000 pyfindfiles-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 23:20:16.847190 pyfindfiles-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:20:16.843189 pyfindfiles-1.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:20:16.843189 pyfindfiles-1.6.0/src/pyfindfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-06 23:20:13.000000 pyfindfiles-1.6.0/src/pyfindfiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-06 23:20:13.000000 pyfindfiles-1.6.0/src/pyfindfiles/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-06 23:20:13.000000 pyfindfiles-1.6.0/src/pyfindfiles/async_vid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-06 23:20:13.000000 pyfindfiles-1.6.0/src/pyfindfiles/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:20:16.847190 pyfindfiles-1.6.0/src/pyfindfiles/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:20:13.000000 pyfindfiles-1.6.0/src/pyfindfiles/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-06 23:20:13.000000 pyfindfiles-1.6.0/src/pyfindfiles/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-06 23:20:13.000000 pyfindfiles-1.6.0/src/pyfindfiles/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-06 23:20:13.000000 pyfindfiles-1.6.0/src/pyfindfiles/tests/test_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-05-06 23:20:13.000000 pyfindfiles-1.6.0/src/pyfindfiles/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-06 23:20:13.000000 pyfindfiles-1.6.0/src/pyfindfiles/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:20:16.847190 pyfindfiles-1.6.0/src/pyfindfiles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-06 23:20:16.000000 pyfindfiles-1.6.0/src/pyfindfiles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-06 23:20:16.000000 pyfindfiles-1.6.0/src/pyfindfiles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 23:20:16.000000 pyfindfiles-1.6.0/src/pyfindfiles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-06 23:20:16.000000 pyfindfiles-1.6.0/src/pyfindfiles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 23:20:16.000000 pyfindfiles-1.6.0/src/pyfindfiles.egg-info/top_level.txt
```

### Comparing `pyfindfiles-1.5.2/LICENSE.txt` & `pyfindfiles-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfindfiles-1.5.2/PKG-INFO` & `pyfindfiles-1.6.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,80 @@
-Metadata-Version: 2.1
-Name: pyfindfiles
-Version: 1.5.2
-Summary: Concurrent, pipelined text and binary file searching via pure Python, cross-platform.
-Keywords: find,grep
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Framework :: AsyncIO
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: lint
-License-File: LICENSE.txt
-
-# PyFindFiles
-
-![ci](https://github.com/scivision/pyfindfiles/workflows/ci/badge.svg)
-[![PyPi Download stats](http://pepy.tech/badge/pyfindfiles)](http://pepy.tech/project/pyfindfiles)
-
-Find files (text or binary) containing text or patterns efficiently with Python, cross-platform.
-Default is to only search files smaller than 10 MBytes.
-Uses pipelining and asyncio to speed up operations.
-
-## Install
-
-Normally install by
-
-```sh
-pip install pyfindfiles
-```
-
-for latest development code
-
-```sh
-git clone https://github.com/scivision/pyfindfiles
-
-pip install -e pyfindfiles
-```
-
-## Usage
-
-`findtext` looks for strings inside text or binary files, and reports filename text is found in.
-
-* `-v`: filename, line number, and text found
-* `-t`: search for files newer than date, or between dates if two dates given.
-
-```sh
-findtext Pattern "*.ext" root
-```
-
-Pattern
-: text to search for
-
-"*.ext"
-: file extension(s) to search for
-
-root
-: top-level directory to search under
-
----
-
-`findvid`
-
-`findvid root` looks under top-level directory `root` for video files (by common file extensions)
+Metadata-Version: 2.1
+Name: pyfindfiles
+Version: 1.6.0
+Summary: Concurrent, pipelined text and binary file searching via pure Python, cross-platform.
+Keywords: find,grep
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Framework :: AsyncIO
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: python-dateutil
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Provides-Extra: lint
+Requires-Dist: flake8; extra == "lint"
+Requires-Dist: flake8-bugbear; extra == "lint"
+Requires-Dist: flake8-builtins; extra == "lint"
+Requires-Dist: flake8-blind-except; extra == "lint"
+Requires-Dist: mypy; extra == "lint"
+Requires-Dist: types-python-dateutil; extra == "lint"
+
+# PyFindFiles
+
+![ci](https://github.com/scivision/pyfindfiles/workflows/ci/badge.svg)
+[![PyPi Download stats](http://pepy.tech/badge/pyfindfiles)](http://pepy.tech/project/pyfindfiles)
+
+Find files (text or binary) containing text or patterns efficiently with Python, cross-platform.
+Default is to only search files smaller than 10 MBytes.
+Uses pipelining and asyncio to speed up operations.
+
+## Install
+
+Normally install by
+
+```sh
+pip install pyfindfiles
+```
+
+for latest development code
+
+```sh
+git clone https://github.com/scivision/pyfindfiles
+
+pip install -e pyfindfiles
+```
+
+## Usage
+
+`findtext` looks for strings inside text or binary files, and reports filename text is found in.
+
+* `-v`: filename, line number, and text found
+* `-t`: search for files newer than date, or between dates if two dates given.
+
+```sh
+python -m pyfindfiles.text Pattern "*.ext" root
+```
+
+Pattern
+: text to search for
+
+"*.ext"
+: file extension(s) to search for
+
+root
+: top-level directory to search under
+
+---
+
+
+```sh
+python -m pyfindfiles.video top
+```
+
+looks under top-level directory "top" for video files (by common file extensions)
```

### Comparing `pyfindfiles-1.5.2/README.md` & `pyfindfiles-1.6.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -27,24 +27,27 @@
 
 `findtext` looks for strings inside text or binary files, and reports filename text is found in.
 
 * `-v`: filename, line number, and text found
 * `-t`: search for files newer than date, or between dates if two dates given.
 
 ```sh
-findtext Pattern "*.ext" root
+python -m pyfindfiles.text Pattern "*.ext" root
 ```
 
 Pattern
 : text to search for
 
 "*.ext"
 : file extension(s) to search for
 
 root
 : top-level directory to search under
 
 ---
 
-`findvid`
 
-`findvid root` looks under top-level directory `root` for video files (by common file extensions)
+```sh
+python -m pyfindfiles.video top
+```
+
+looks under top-level directory "top" for video files (by common file extensions)
```

### Comparing `pyfindfiles-1.5.2/pyproject.toml` & `pyfindfiles-1.6.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,36 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyfindfiles"
-version = "1.5.2"
 description = "Concurrent, pipelined text and binary file searching via pure Python, cross-platform."
 keywords = ["find", "grep"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Console",
   "Framework :: AsyncIO",
   "Intended Audience :: Developers",
   "Intended Audience :: End Users/Desktop",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3"
 ]
-dynamic = ["readme"]
-requires-python = ">=3.8"
+dynamic = ["readme", "version"]
+requires-python = ">=3.9"
 dependencies = ["python-dateutil"]
 
 [project.optional-dependencies]
 tests = ["pytest"]
 lint = ["flake8", "flake8-bugbear", "flake8-builtins", "flake8-blind-except",
 "mypy", "types-python-dateutil"]
 
-[project.scripts]
-findtext = "pyfindfiles.__main__:find_text"
-findvid = "pyfindfiles.__main__:find_video"
-findproj = "pyfindfiles.__main__:find_project"
-
 [tool.setuptools.dynamic]
 readme = {file = ["README.md"], content-type = "text/markdown"}
+version = {attr = "pyfindfiles.__version__"}
 
 [tool.black]
 line-length = 100
 
 [tool.mypy]
 files = ["src"]
-ignore_missing_imports = true
-strict_optional = true
-allow_redefinition = true
-show_error_context = false
-show_column_numbers = true
```

### Comparing `pyfindfiles-1.5.2/src/pyfindfiles/async_vid.py` & `pyfindfiles-1.6.0/src/pyfindfiles/async_vid.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     path = Path(path).expanduser()
     cmd = ["dir", "/s", "*" + ext]
     logging.debug(" ".join(cmd))
     # this has to be _shell due to that "dir" is part of Windows shell itself; _exec won't work.
     proc = await asyncio.create_subprocess_shell(
         " ".join(cmd),
-        cwd=str(path),
+        cwd=path,
         stdout=asyncio.subprocess.PIPE,
         stderr=asyncio.subprocess.DEVNULL,
     )
     stdout, _ = await proc.communicate()
 
     flist = []
     for r in stdout.decode("utf8").split("\n"):
```

### Comparing `pyfindfiles-1.5.2/src/pyfindfiles/project.py` & `pyfindfiles-1.6.0/src/pyfindfiles/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 from pathlib import Path
 import json
 
 
 def detect_lang(path: Path) -> list[str]:
-    """ return lowercase language name, or empty if undetermined.
+    """return lowercase language name, or empty if undetermined.
 
     Reference:
     https://help.github.com/en/github/visualizing-repository-data-with-graphs/
         listing-the-packages-that-a-repository-depends-on#supported-package-ecosystems
     """
 
     cmfn = path / "codemeta.json"
```

### Comparing `pyfindfiles-1.5.2/src/pyfindfiles/tests/test_text.py` & `pyfindfiles-1.6.0/src/pyfindfiles/tests/test_text.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 #!/usr/bin/env python
 import subprocess
 import pytest
-import pyfindfiles as pf
+import pyfindfiles.text as pf
 import os
 from datetime import datetime
+import sys
 
 """
 TEST_STRING_TO_MATCH
 """
 
 
 @pytest.mark.skipif(bool(os.environ.get("CI")), reason="CI does not like recursive search")
 def test_script(tmp_path):
     (tmp_path / "foo.py").write_text("import datetime")
-    ret = subprocess.check_output(["findtext", "import", "*.py", str(tmp_path)], universal_newlines=True)
+    ret = subprocess.check_output(
+        [sys.executable, "-m", "pyfindfiles.text", "import", "*.py", str(tmp_path)],
+        text=True,
+    )
 
     assert isinstance(ret, str)
 
     assert len(ret) > 0
 
 
 def test_glob(tmp_path):
-
     fn = tmp_path / "foo.py"
     fn.write_text("MATCH_ME_NOW_PLEASE")
 
     files = pf.findtext(tmp_path, "MATCH_ME_NOW", globext="*.py")
 
     for file, _ in files:
         assert file.samefile(fn)
 
 
 def test_age(tmp_path):
-
     fn = tmp_path / "foo.py"
     fn.write_text("MATCH_ME_NOW_PLEASE")
 
-    files = pf.findtext(tmp_path, "MATCH_ME_NOW", globext="*.py", age=[datetime(2019, 1, 1)])
+    files = pf.findtext(tmp_path, "MATCH_ME_NOW", globext="*.py", age=[datetime(2024, 1, 1)])
 
     for file, _ in files:
         assert file.samefile(fn)
```

### Comparing `pyfindfiles-1.5.2/src/pyfindfiles/tests/test_video.py` & `pyfindfiles-1.6.0/src/pyfindfiles/tests/test_video.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 #!/usr/bin/env python
 import pytest
 from pathlib import Path
 import subprocess
 import sys
 
-import pyfindfiles.vid as fv
+import pyfindfiles.video as fv
 
 if __file__ is None:
     R = None
 else:
     R = Path(__file__).parent
 
 
 @pytest.mark.skipif(R is None, reason="__file__ missing")
 def test_findvid_serial():
-
     files = fv.findvid(R, ".avi")
 
     flist = list(files)
     print(flist)
     assert len(flist) == 2
 
 
 @pytest.mark.skipif(R is None, reason="__file__ missing")
 @pytest.mark.skipif(sys.platform != "linux", reason="Linux only test")
 def test_findvid_gnu():
-
     files = list(fv.findvid_gnu(R, ".avi"))
 
     assert len(files) == 2
 
 
 @pytest.mark.skipif(R is None, reason="__file__ missing")
 def test_script():
-    files = subprocess.check_output(["findvid", str(R)], universal_newlines=True).strip()
+    files = subprocess.check_output(
+        [sys.executable, "-m", "pyfindfiles.video", str(R)], text=True
+    ).strip()
     flist = files.split("\n")
     print(flist)
     assert len(flist) == 2
```

### Comparing `pyfindfiles-1.5.2/src/pyfindfiles/vid.py` & `pyfindfiles-1.6.0/src/pyfindfiles/video.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
 import typing as T
 from pathlib import Path
 import logging
 import sys
 import subprocess
 import shutil
+from argparse import ArgumentParser
+
+VIDEXT = [".avi", ".mov", ".mp4", ".mpg", ".mpeg", ".webm", ".ogv", ".mkv", ".wmv"]
 
 
 def findvid(path: Path, ext: list[str]) -> T.Iterator[Path]:
     """
     recursive file search in Pure Python.
     about 10 times slower than Linux find, but platform-independent.
     """
@@ -37,11 +40,34 @@
     if sys.platform != "darwin":
         cmd += ["-regextype", "posix-egrep"]
 
     cmd += ["-iregex", r".*(" + r"|".join(exts) + r")$"]
 
     logging.debug(" ".join(cmd))
 
-    stdout = subprocess.check_output(cmd, universal_newlines=True).strip()
+    stdout = subprocess.check_output(cmd, text=True).strip()
 
     for file in stdout.split("\n"):
         yield file
+
+
+if __name__ == "__main__":
+    p = ArgumentParser()
+    p.add_argument("path", help="root path to start recursive search")
+    p.add_argument("-v", "--verbose", action="store_true")
+    p.add_argument("-ext", help="video extension to search for", nargs="+", default=VIDEXT)
+    P = p.parse_args()
+
+    root = Path(P.path).expanduser().resolve()
+    if not root.is_dir():
+        raise NotADirectoryError(root)
+
+    if P.verbose:
+        logging.basicConfig(level=logging.DEBUG)
+
+    if sys.platform == "linux":
+        videos = findvid_gnu(root, P.ext)
+    else:
+        videos = findvid(root, P.ext)
+
+    for video in videos:
+        print(video)
```

### Comparing `pyfindfiles-1.5.2/src/pyfindfiles.egg-info/PKG-INFO` & `pyfindfiles-1.6.0/src/pyfindfiles.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,80 @@
-Metadata-Version: 2.1
-Name: pyfindfiles
-Version: 1.5.2
-Summary: Concurrent, pipelined text and binary file searching via pure Python, cross-platform.
-Keywords: find,grep
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Framework :: AsyncIO
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: lint
-License-File: LICENSE.txt
-
-# PyFindFiles
-
-![ci](https://github.com/scivision/pyfindfiles/workflows/ci/badge.svg)
-[![PyPi Download stats](http://pepy.tech/badge/pyfindfiles)](http://pepy.tech/project/pyfindfiles)
-
-Find files (text or binary) containing text or patterns efficiently with Python, cross-platform.
-Default is to only search files smaller than 10 MBytes.
-Uses pipelining and asyncio to speed up operations.
-
-## Install
-
-Normally install by
-
-```sh
-pip install pyfindfiles
-```
-
-for latest development code
-
-```sh
-git clone https://github.com/scivision/pyfindfiles
-
-pip install -e pyfindfiles
-```
-
-## Usage
-
-`findtext` looks for strings inside text or binary files, and reports filename text is found in.
-
-* `-v`: filename, line number, and text found
-* `-t`: search for files newer than date, or between dates if two dates given.
-
-```sh
-findtext Pattern "*.ext" root
-```
-
-Pattern
-: text to search for
-
-"*.ext"
-: file extension(s) to search for
-
-root
-: top-level directory to search under
-
----
-
-`findvid`
-
-`findvid root` looks under top-level directory `root` for video files (by common file extensions)
+Metadata-Version: 2.1
+Name: pyfindfiles
+Version: 1.6.0
+Summary: Concurrent, pipelined text and binary file searching via pure Python, cross-platform.
+Keywords: find,grep
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Framework :: AsyncIO
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: python-dateutil
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Provides-Extra: lint
+Requires-Dist: flake8; extra == "lint"
+Requires-Dist: flake8-bugbear; extra == "lint"
+Requires-Dist: flake8-builtins; extra == "lint"
+Requires-Dist: flake8-blind-except; extra == "lint"
+Requires-Dist: mypy; extra == "lint"
+Requires-Dist: types-python-dateutil; extra == "lint"
+
+# PyFindFiles
+
+![ci](https://github.com/scivision/pyfindfiles/workflows/ci/badge.svg)
+[![PyPi Download stats](http://pepy.tech/badge/pyfindfiles)](http://pepy.tech/project/pyfindfiles)
+
+Find files (text or binary) containing text or patterns efficiently with Python, cross-platform.
+Default is to only search files smaller than 10 MBytes.
+Uses pipelining and asyncio to speed up operations.
+
+## Install
+
+Normally install by
+
+```sh
+pip install pyfindfiles
+```
+
+for latest development code
+
+```sh
+git clone https://github.com/scivision/pyfindfiles
+
+pip install -e pyfindfiles
+```
+
+## Usage
+
+`findtext` looks for strings inside text or binary files, and reports filename text is found in.
+
+* `-v`: filename, line number, and text found
+* `-t`: search for files newer than date, or between dates if two dates given.
+
+```sh
+python -m pyfindfiles.text Pattern "*.ext" root
+```
+
+Pattern
+: text to search for
+
+"*.ext"
+: file extension(s) to search for
+
+root
+: top-level directory to search under
+
+---
+
+
+```sh
+python -m pyfindfiles.video top
+```
+
+looks under top-level directory "top" for video files (by common file extensions)
```

### Comparing `pyfindfiles-1.5.2/src/pyfindfiles.egg-info/SOURCES.txt` & `pyfindfiles-1.6.0/src/pyfindfiles.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 README.md
 pyproject.toml
 src/pyfindfiles/__init__.py
 src/pyfindfiles/__main__.py
 src/pyfindfiles/async_vid.py
 src/pyfindfiles/project.py
 src/pyfindfiles/text.py
-src/pyfindfiles/vid.py
+src/pyfindfiles/video.py
 src/pyfindfiles.egg-info/PKG-INFO
 src/pyfindfiles.egg-info/SOURCES.txt
 src/pyfindfiles.egg-info/dependency_links.txt
-src/pyfindfiles.egg-info/entry_points.txt
 src/pyfindfiles.egg-info/requires.txt
 src/pyfindfiles.egg-info/top_level.txt
 src/pyfindfiles/tests/__init__.py
 src/pyfindfiles/tests/test_project.py
 src/pyfindfiles/tests/test_text.py
 src/pyfindfiles/tests/test_video.py
```

