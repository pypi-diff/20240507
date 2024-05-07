# Comparing `tmp/iterfzf-1.3.0.51.0.tar.gz` & `tmp/iterfzf-1.4.0.51.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iterfzf-1.3.0.51.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "iterfzf-1.4.0.51.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `iterfzf-1.3.0.51.0.tar` & `iterfzf-1.4.0.51.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35147 2024-05-06 03:06:36.592626 iterfzf-1.3.0.51.0/LICENSE
--rw-r--r--   0        0        0    10007 2024-05-06 03:06:36.592626 iterfzf-1.3.0.51.0/README.rst
--rw-r--r--   0        0        0    11869 2024-05-06 03:06:36.592626 iterfzf-1.3.0.51.0/build_dist.py
--rw-r--r--   0        0        0     4022 2024-05-06 03:06:36.592626 iterfzf-1.3.0.51.0/iterfzf/__init__.py
--rw-r--r--   0        0        0    27912 2024-05-06 03:07:10.424747 iterfzf-1.3.0.51.0/iterfzf/fzf-0.51.0-release.json
--rwxr-xr-x   0        0        0  4325888 2024-05-06 03:07:08.896742 iterfzf-1.3.0.51.0/iterfzf/fzf.exe
--rw-r--r--   0        0        0      714 2024-05-06 03:06:36.592626 iterfzf-1.3.0.51.0/iterfzf/test_iterfzf.py
--rw-r--r--   0        0        0     1694 2024-05-06 03:06:36.592626 iterfzf-1.3.0.51.0/pyproject.toml
--rw-r--r--   0        0        0    11335 1970-01-01 00:00:00.000000 iterfzf-1.3.0.51.0/PKG-INFO
+-rw-r--r--   0        0        0    35147 2024-05-07 03:17:53.362538 iterfzf-1.4.0.51.0/LICENSE
+-rw-r--r--   0        0        0    10472 2024-05-07 03:17:53.362538 iterfzf-1.4.0.51.0/README.rst
+-rw-r--r--   0        0        0    11869 2024-05-07 03:17:53.362538 iterfzf-1.4.0.51.0/build_dist.py
+-rw-r--r--   0        0        0     4261 2024-05-07 03:17:53.362538 iterfzf-1.4.0.51.0/iterfzf/__init__.py
+-rw-r--r--   0        0        0    27916 2024-05-07 03:18:40.947113 iterfzf-1.4.0.51.0/iterfzf/fzf-0.51.0-release.json
+-rwxr-xr-x   0        0        0  4325888 2024-05-07 03:18:39.447095 iterfzf-1.4.0.51.0/iterfzf/fzf.exe
+-rw-r--r--   0        0        0      714 2024-05-07 03:17:53.362538 iterfzf-1.4.0.51.0/iterfzf/test_iterfzf.py
+-rw-r--r--   0        0        0     1694 2024-05-07 03:17:53.362538 iterfzf-1.4.0.51.0/pyproject.toml
+-rw-r--r--   0        0        0    11800 1970-01-01 00:00:00.000000 iterfzf-1.4.0.51.0/PKG-INFO
```

### Comparing `iterfzf-1.3.0.51.0/LICENSE` & `iterfzf-1.4.0.51.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iterfzf-1.3.0.51.0/README.rst` & `iterfzf-1.4.0.51.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,21 @@
    For both modes, the function returns ``None`` if nothing is matched or
    a user cancelled.
 
    ``False`` by default.
 
    Corresponds to ``-m``/``--multi`` option.
 
+``bind``
+   The key/event bindings to pass to ``fzf``.
+
+   Dictionary of the form {KEY: ACTION} or {EVENT: ACTION}.
+
+   Corresponds to ``--bind=KEYBINDS`` option.
+
 ``print_query``
    If ``True`` the return type is a tuple where the first element is the query
    the user actually typed, and the second element is the selected output as
    described above and depending on the state of ``multi``.
 
    ``False`` by default.
 
@@ -196,14 +203,26 @@
      |   |
      |   \---- 4. bundled fzf's minor version
      \-------- 2. iterfzf's minor version
 
 .. _Semantic Versioning: http://semver.org/
 
 
+Version 1.4.0.51.0
+~~~~~~~~~~~~~~~~~~
+
+Released on May 7, 2024.  Bundles ``fzf`` `0.51.0`__.
+
+- Added ``bind`` option. [`#21`__, `#36`__ by Gregory.K]
+
+__ https://github.com/junegunn/fzf/releases/tag/0.51.0
+__ https://github.com/dahlia/iterfzf/issues/21
+__ https://github.com/dahlia/iterfzf/pull/36
+
+
 Version 1.3.0.51.0
 ~~~~~~~~~~~~~~~~~~
 
 Released on May 6, 2024.  Bundles ``fzf`` `0.51.0`__.
 
 - Added ``sort`` option.  [`#18`__, `#35`__ by Gregory.K]
 - Officially support Python 3.12.
```

### Comparing `iterfzf-1.3.0.51.0/build_dist.py` & `iterfzf-1.4.0.51.0/build_dist.py`

 * *Files identical despite different names*

### Comparing `iterfzf-1.3.0.51.0/iterfzf/__init__.py` & `iterfzf-1.4.0.51.0/iterfzf/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import print_function
 
 import errno
 from os import fspath, PathLike
 from pathlib import Path
 import subprocess
 import sys
-from typing import AnyStr, Iterable, Literal, Optional
+from typing import AnyStr, Iterable, Literal, Mapping, Optional
 
 __all__ = '__fzf_version__', '__version__', 'BUNDLED_EXECUTABLE', 'iterfzf'
 
 __fzf_version__ = '0.51.0'
-__version__ = '1.3.' + __fzf_version__
+__version__ = '1.4.' + __fzf_version__
 
 POSIX_EXECUTABLE_NAME: Literal['fzf'] = 'fzf'
 WINDOWS_EXECUTABLE_NAME: Literal['fzf.exe'] = 'fzf.exe'
 EXECUTABLE_NAME: Literal['fzf', 'fzf.exe'] = \
     WINDOWS_EXECUTABLE_NAME \
     if sys.platform == 'win32' \
     else POSIX_EXECUTABLE_NAME
@@ -26,18 +26,19 @@
     iterable: Iterable[AnyStr],
     *,
     # Sorting:
     sort: bool = False,
     # Search mode:
     extended: bool = True,
     exact: bool = False,
-    case_sensitive: bool = None,
+    case_sensitive: Optional[bool] = None,
     # Interface:
     multi: bool = False,
     mouse: bool = True,
+    bind: Optional[Mapping[str, str]] = None,
     print_query: bool = False,
     # Layout:
     prompt: str = '> ',
     ansi: bool = False,
     preview: Optional[str] = None,
     # Misc:
     query: str = '',
@@ -55,14 +56,19 @@
         cmd.append('+i' if case_sensitive else '-i')
     if exact:
         cmd.append('--exact')
     if multi:
         cmd.append('--multi')
     if not mouse:
         cmd.append('--no-mouse')
+    if bind:
+        bind_options = ','.join(
+            r"{}:{}".format(key, action) for key, action in bind.items()
+        )
+        cmd.append('--bind=' + bind_options)
     if print_query:
         cmd.append('--print-query')
     if query:
         cmd.append('--query=' + query)
     if preview:
         cmd.append('--preview=' + preview)
     if ansi:
```

### Comparing `iterfzf-1.3.0.51.0/iterfzf/fzf-0.51.0-release.json` & `iterfzf-1.4.0.51.0/iterfzf/fzf-0.51.0-release.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9963562753036437%*

 * *Differences: {"'assets'": "{0: {'download_count': 503}, 1: {'download_count': 1334}, 2: {'download_count': 30}, "*

 * *             "3: {'download_count': 15998}, 4: {'download_count': 1266}, 5: {'download_count': "*

 * *             "14}, 6: {'download_count': 21}, 7: {'download_count': 57}, 8: {'download_count': 7}, "*

 * *             "9: {'download_count': 12}, 10: {'download_count': 10}, 11: {'download_count': 13}, "*

 * *             "12: {'download_count': 4805}, 13: {'download_count': 76}, 14: {'download_count': 7}, "*

 * *              […]*

```diff
@@ -1,14 +1,14 @@
 {
     "assets": [
         {
             "browser_download_url": "https://github.com/junegunn/fzf/releases/download/0.51.0/fzf-0.51.0-darwin_amd64.zip",
             "content_type": "application/zip",
             "created_at": "2024-05-01T05:37:00Z",
-            "download_count": 419,
+            "download_count": 503,
             "id": 165283849,
             "label": "",
             "name": "fzf-0.51.0-darwin_amd64.zip",
             "node_id": "RA_kwDOANKv9s4J2ggJ",
             "size": 1566862,
             "state": "uploaded",
             "updated_at": "2024-05-01T05:37:01Z",
@@ -34,15 +34,15 @@
             },
             "url": "https://api.github.com/repos/junegunn/fzf/releases/assets/165283849"
         },
         {
             "browser_download_url": "https://github.com/junegunn/fzf/releases/download/0.51.0/fzf-0.51.0-darwin_arm64.zip",
             "content_type": "application/zip",
             "created_at": "2024-05-01T05:37:00Z",
-            "download_count": 1062,
+            "download_count": 1334,
             "id": 165283850,
             "label": "",
             "name": "fzf-0.51.0-darwin_arm64.zip",
             "node_id": "RA_kwDOANKv9s4J2ggK",
             "size": 1482202,
             "state": "uploaded",
             "updated_at": "2024-05-01T05:37:01Z",
@@ -68,15 +68,15 @@
             },
             "url": "https://api.github.com/repos/junegunn/fzf/releases/assets/165283850"
         },
         {
             "browser_download_url": "https://github.com/junegunn/fzf/releases/download/0.51.0/fzf-0.51.0-freebsd_amd64.tar.gz",
             "content_type": "application/octet-stream",
             "created_at": "2024-05-01T05:36:59Z",
-            "download_count": 23,
+            "download_count": 30,
             "id": 165283845,
             "label": "",
             "name": "fzf-0.51.0-freebsd_amd64.tar.gz",
             "node_id": "RA_kwDOANKv9s4J2ggF",
             "size": 1489995,
             "state": "uploaded",
             "updated_at": "2024-05-01T05:37:00Z",
@@ -102,15 +102,15 @@
             },
             "url": "https://api.github.com/repos/junegunn/fzf/releases/assets/165283845"
         },
         {
             "browser_download_url": "https://github.com/junegunn/fzf/releases/download/0.51.0/fzf-0.51.0-linux_amd64.tar.gz",
             "content_type": "application/octet-stream",
             "created_at": "2024-05-01T05:36:59Z",
-            "download_count": 12783,
+            "download_count": 15998,
             "id": 165283843,
             "label": "",
             "name": "fzf-0.51.0-linux_amd64.tar.gz",
             "node_id": "RA_kwDOANKv9s4J2ggD",
             "size": 1497424,
             "state": "uploaded",
             "updated_at": "2024-05-01T05:36:59Z",
@@ -136,15 +136,15 @@
             },
             "url": "https://api.github.com/repos/junegunn/fzf/releases/assets/165283843"
         },
         {
             "browser_download_url": "https://github.com/junegunn/fzf/releases/download/0.51.0/fzf-0.51.0-linux_arm64.tar.gz",
             "content_type": "application/octet-stream",
             "created_at": "2024-05-01T05:36:56Z",
-            "download_count": 993,
+            "download_count": 1266,
             "id": 165283837,
             "label": "",
             "name": "fzf-0.51.0-linux_arm64.tar.gz",
             "node_id": "RA_kwDOANKv9s4J2gf9",
             "size": 1388953,
             "state": "uploaded",
             "updated_at": "2024-05-01T05:36:58Z",
@@ -170,15 +170,15 @@
             },
             "url": "https://api.github.com/repos/junegunn/fzf/releases/assets/165283837"
         },
         {
             "browser_download_url": "https://github.com/junegunn/fzf/releases/download/0.51.0/fzf-0.51.0-linux_armv5.tar.gz",
             "content_type": "application/octet-stream",
             "created_at": "2024-05-01T05:36:56Z",
-            "download_count": 8,
+            "download_count": 14,
             "id": 165283832,
             "label": "",
             "name": "fzf-0.51.0-linux_armv5.tar.gz",
             "node_id": "RA_kwDOANKv9s4J2gf4",
             "size": 1461190,
             "state": "uploaded",
             "updated_at": "2024-05-01T05:36:58Z",
@@ -204,15 +204,15 @@
             },
             "url": "https://api.github.com/repos/junegunn/fzf/releases/assets/165283832"
         },
         {
             "browser_download_url": "https://github.com/junegunn/fzf/releases/download/0.51.0/fzf-0.51.0-linux_armv6.tar.gz",
             "content_type": "application/octet-stream",
             "created_at": "2024-05-01T05:36:56Z",
-            "download_count": 10,
+            "download_count": 21,
             "id": 165283834,
             "label": "",
             "name": "fzf-0.51.0-linux_armv6.tar.gz",
             "node_id": "RA_kwDOANKv9s4J2gf6",
             "size": 1451107,
             "state": "uploaded",
             "updated_at": "2024-05-01T05:36:58Z",
@@ -238,15 +238,15 @@
             },
             "url": "https://api.github.com/repos/junegunn/fzf/releases/assets/165283834"
         },
         {
             "browser_download_url": "https://github.com/junegunn/fzf/releases/download/0.51.0/fzf-0.51.0-linux_armv7.tar.gz",
             "content_type": "application/octet-stream",
             "created_at": "2024-05-01T05:36:56Z",
-            "download_count": 38,
+            "download_count": 57,
             "id": 165283831,
             "label": "",
             "name": "fzf-0.51.0-linux_armv7.tar.gz",
             "node_id": "RA_kwDOANKv9s4J2gf3",
             "size": 1449119,
             "state": "uploaded",
             "updated_at": "2024-05-01T05:36:58Z",
@@ -272,15 +272,15 @@
             },
             "url": "https://api.github.com/repos/junegunn/fzf/releases/assets/165283831"
         },
         {
             "browser_download_url": "https://github.com/junegunn/fzf/releases/download/0.51.0/fzf-0.51.0-linux_loong64.tar.gz",
             "content_type": "application/octet-stream",
             "created_at": "2024-05-01T05:36:58Z",
-            "download_count": 6,
+            "download_count": 7,
             "id": 165283840,
             "label": "",
             "name": "fzf-0.51.0-linux_loong64.tar.gz",
             "node_id": "RA_kwDOANKv9s4J2ggA",
             "size": 1452037,
             "state": "uploaded",
             "updated_at": "2024-05-01T05:36:59Z",
@@ -306,15 +306,15 @@
             },
             "url": "https://api.github.com/repos/junegunn/fzf/releases/assets/165283840"
         },
         {
             "browser_download_url": "https://github.com/junegunn/fzf/releases/download/0.51.0/fzf-0.51.0-linux_ppc64le.tar.gz",
             "content_type": "application/octet-stream",
             "created_at": "2024-05-01T05:36:56Z",
-            "download_count": 7,
+            "download_count": 12,
             "id": 165283835,
             "label": "",
             "name": "fzf-0.51.0-linux_ppc64le.tar.gz",
             "node_id": "RA_kwDOANKv9s4J2gf7",
             "size": 1381489,
             "state": "uploaded",
             "updated_at": "2024-05-01T05:36:58Z",
@@ -340,15 +340,15 @@
             },
             "url": "https://api.github.com/repos/junegunn/fzf/releases/assets/165283835"
         },
         {
             "browser_download_url": "https://github.com/junegunn/fzf/releases/download/0.51.0/fzf-0.51.0-linux_s390x.tar.gz",
             "content_type": "application/octet-stream",
             "created_at": "2024-05-01T05:36:59Z",
-            "download_count": 5,
+            "download_count": 10,
             "id": 165283847,
             "label": "",
             "name": "fzf-0.51.0-linux_s390x.tar.gz",
             "node_id": "RA_kwDOANKv9s4J2ggH",
             "size": 1464544,
             "state": "uploaded",
             "updated_at": "2024-05-01T05:37:00Z",
@@ -374,15 +374,15 @@
             },
             "url": "https://api.github.com/repos/junegunn/fzf/releases/assets/165283847"
         },
         {
             "browser_download_url": "https://github.com/junegunn/fzf/releases/download/0.51.0/fzf-0.51.0-openbsd_amd64.tar.gz",
             "content_type": "application/octet-stream",
             "created_at": "2024-05-01T05:36:56Z",
-            "download_count": 11,
+            "download_count": 13,
             "id": 165283838,
             "label": "",
             "name": "fzf-0.51.0-openbsd_amd64.tar.gz",
             "node_id": "RA_kwDOANKv9s4J2gf-",
             "size": 1493285,
             "state": "uploaded",
             "updated_at": "2024-05-01T05:36:58Z",
@@ -408,15 +408,15 @@
             },
             "url": "https://api.github.com/repos/junegunn/fzf/releases/assets/165283838"
         },
         {
             "browser_download_url": "https://github.com/junegunn/fzf/releases/download/0.51.0/fzf-0.51.0-windows_amd64.zip",
             "content_type": "application/zip",
             "created_at": "2024-05-01T05:36:59Z",
-            "download_count": 4073,
+            "download_count": 4805,
             "id": 165283844,
             "label": "",
             "name": "fzf-0.51.0-windows_amd64.zip",
             "node_id": "RA_kwDOANKv9s4J2ggE",
             "size": 1726777,
             "state": "uploaded",
             "updated_at": "2024-05-01T05:37:00Z",
@@ -442,15 +442,15 @@
             },
             "url": "https://api.github.com/repos/junegunn/fzf/releases/assets/165283844"
         },
         {
             "browser_download_url": "https://github.com/junegunn/fzf/releases/download/0.51.0/fzf-0.51.0-windows_arm64.zip",
             "content_type": "application/zip",
             "created_at": "2024-05-01T05:36:56Z",
-            "download_count": 67,
+            "download_count": 76,
             "id": 165283836,
             "label": "",
             "name": "fzf-0.51.0-windows_arm64.zip",
             "node_id": "RA_kwDOANKv9s4J2gf8",
             "size": 1607770,
             "state": "uploaded",
             "updated_at": "2024-05-01T05:36:58Z",
@@ -476,15 +476,15 @@
             },
             "url": "https://api.github.com/repos/junegunn/fzf/releases/assets/165283836"
         },
         {
             "browser_download_url": "https://github.com/junegunn/fzf/releases/download/0.51.0/fzf-0.51.0-windows_armv5.zip",
             "content_type": "application/zip",
             "created_at": "2024-05-01T05:36:58Z",
-            "download_count": 5,
+            "download_count": 7,
             "id": 165283841,
             "label": "",
             "name": "fzf-0.51.0-windows_armv5.zip",
             "node_id": "RA_kwDOANKv9s4J2ggB",
             "size": 1700621,
             "state": "uploaded",
             "updated_at": "2024-05-01T05:36:59Z",
@@ -510,15 +510,15 @@
             },
             "url": "https://api.github.com/repos/junegunn/fzf/releases/assets/165283841"
         },
         {
             "browser_download_url": "https://github.com/junegunn/fzf/releases/download/0.51.0/fzf-0.51.0-windows_armv6.zip",
             "content_type": "application/zip",
             "created_at": "2024-05-01T05:36:56Z",
-            "download_count": 5,
+            "download_count": 7,
             "id": 165283833,
             "label": "",
             "name": "fzf-0.51.0-windows_armv6.zip",
             "node_id": "RA_kwDOANKv9s4J2gf5",
             "size": 1691851,
             "state": "uploaded",
             "updated_at": "2024-05-01T05:36:58Z",
@@ -544,15 +544,15 @@
             },
             "url": "https://api.github.com/repos/junegunn/fzf/releases/assets/165283833"
         },
         {
             "browser_download_url": "https://github.com/junegunn/fzf/releases/download/0.51.0/fzf-0.51.0-windows_armv7.zip",
             "content_type": "application/zip",
             "created_at": "2024-05-01T05:36:59Z",
-            "download_count": 17,
+            "download_count": 20,
             "id": 165283842,
             "label": "",
             "name": "fzf-0.51.0-windows_armv7.zip",
             "node_id": "RA_kwDOANKv9s4J2ggC",
             "size": 1684860,
             "state": "uploaded",
             "updated_at": "2024-05-01T05:36:59Z",
@@ -578,15 +578,15 @@
             },
             "url": "https://api.github.com/repos/junegunn/fzf/releases/assets/165283842"
         },
         {
             "browser_download_url": "https://github.com/junegunn/fzf/releases/download/0.51.0/fzf_0.51.0_checksums.txt",
             "content_type": "text/plain; charset=utf-8",
             "created_at": "2024-05-01T05:36:59Z",
-            "download_count": 59,
+            "download_count": 64,
             "id": 165283846,
             "label": "",
             "name": "fzf_0.51.0_checksums.txt",
             "node_id": "RA_kwDOANKv9s4J2ggG",
             "size": 1631,
             "state": "uploaded",
             "updated_at": "2024-05-01T05:36:59Z",
@@ -644,19 +644,19 @@
     "prerelease": false,
     "published_at": "2024-05-01T05:37:01Z",
     "reactions": {
         "+1": 32,
         "-1": 0,
         "confused": 0,
         "eyes": 0,
-        "heart": 11,
+        "heart": 12,
         "hooray": 10,
         "laugh": 2,
         "rocket": 10,
-        "total_count": 65,
+        "total_count": 66,
         "url": "https://api.github.com/repos/junegunn/fzf/releases/153625875/reactions"
     },
     "tag_name": "0.51.0",
     "tarball_url": "https://api.github.com/repos/junegunn/fzf/tarball/0.51.0",
     "target_commitish": "master",
     "upload_url": "https://uploads.github.com/repos/junegunn/fzf/releases/153625875/assets{?name,label}",
     "url": "https://api.github.com/repos/junegunn/fzf/releases/153625875",
```

### Comparing `iterfzf-1.3.0.51.0/iterfzf/fzf.exe` & `iterfzf-1.4.0.51.0/iterfzf/fzf.exe`

 * *Files identical despite different names*

### Comparing `iterfzf-1.3.0.51.0/iterfzf/test_iterfzf.py` & `iterfzf-1.4.0.51.0/iterfzf/test_iterfzf.py`

 * *Files identical despite different names*

### Comparing `iterfzf-1.3.0.51.0/pyproject.toml` & `iterfzf-1.4.0.51.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iterfzf-1.3.0.51.0/PKG-INFO` & `iterfzf-1.4.0.51.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterfzf
-Version: 1.3.0.51.0
+Version: 1.4.0.51.0
 Summary: Pythonic interface to fzf
 Keywords: fzf
 Author-email: "Hong Minhee (洪 民憙)" <hong@minhee.org>
 Requires-Python: >= 3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console :: Curses
@@ -102,14 +102,21 @@
    For both modes, the function returns ``None`` if nothing is matched or
    a user cancelled.
 
    ``False`` by default.
 
    Corresponds to ``-m``/``--multi`` option.
 
+``bind``
+   The key/event bindings to pass to ``fzf``.
+
+   Dictionary of the form {KEY: ACTION} or {EVENT: ACTION}.
+
+   Corresponds to ``--bind=KEYBINDS`` option.
+
 ``print_query``
    If ``True`` the return type is a tuple where the first element is the query
    the user actually typed, and the second element is the selected output as
    described above and depending on the state of ``multi``.
 
    ``False`` by default.
 
@@ -225,14 +232,26 @@
      |   |
      |   \---- 4. bundled fzf's minor version
      \-------- 2. iterfzf's minor version
 
 .. _Semantic Versioning: http://semver.org/
 
 
+Version 1.4.0.51.0
+~~~~~~~~~~~~~~~~~~
+
+Released on May 7, 2024.  Bundles ``fzf`` `0.51.0`__.
+
+- Added ``bind`` option. [`#21`__, `#36`__ by Gregory.K]
+
+__ https://github.com/junegunn/fzf/releases/tag/0.51.0
+__ https://github.com/dahlia/iterfzf/issues/21
+__ https://github.com/dahlia/iterfzf/pull/36
+
+
 Version 1.3.0.51.0
 ~~~~~~~~~~~~~~~~~~
 
 Released on May 6, 2024.  Bundles ``fzf`` `0.51.0`__.
 
 - Added ``sort`` option.  [`#18`__, `#35`__ by Gregory.K]
 - Officially support Python 3.12.
```

