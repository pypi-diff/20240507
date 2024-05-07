# Comparing `tmp/ymlstash-1.0.0.tar.gz` & `tmp/ymlstash-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ymlstash-1.0.0.tar", max compression
+gzip compressed data, was "ymlstash-1.0.1.tar", max compression
```

## Comparing `ymlstash-1.0.0.tar` & `ymlstash-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2024-05-07 18:56:12.873162 ymlstash-1.0.0/LICENSE
--rw-r--r--   0        0        0     1099 2024-05-07 19:06:24.763995 ymlstash-1.0.0/README.md
--rw-r--r--   0        0        0      474 2024-05-07 13:38:51.615865 ymlstash-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       50 2024-05-07 13:34:28.333474 ymlstash-1.0.0/ymlstash/__init__.py
--rw-r--r--   0        0        0     1691 2024-05-07 19:16:15.727816 ymlstash-1.0.0/ymlstash/stash.py
--rw-r--r--   0        0        0     1759 1970-01-01 00:00:00.000000 ymlstash-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-07 18:56:12.873162 ymlstash-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1266 2024-05-07 19:30:45.260589 ymlstash-1.0.1/README.md
+-rw-r--r--   0        0        0      641 2024-05-07 20:11:41.617108 ymlstash-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       50 2024-05-07 13:34:28.333474 ymlstash-1.0.1/ymlstash/__init__.py
+-rw-r--r--   0        0        0     1691 2024-05-07 19:16:15.727816 ymlstash-1.0.1/ymlstash/stash.py
+-rw-r--r--   0        0        0     1926 1970-01-01 00:00:00.000000 ymlstash-1.0.1/PKG-INFO
```

### Comparing `ymlstash-1.0.0/LICENSE` & `ymlstash-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ymlstash-1.0.0/README.md` & `ymlstash-1.0.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 # ymlstash
 
 A simple ORM-like utility for operating on local YAML files via Python dataclasses.
 
+## Install
+
+Package is published on PyPI - https://pypi.org/project/ymlstash/
+
+Install from pip or your favorite package manager:
+
+```bash
+$ pip install ymlstash
+```
+
 ## Usage
 
 Define a dataclass:
 
 ```python
 from dataclasses import dataclass
 from typing import ClassVar
```

### Comparing `ymlstash-1.0.0/ymlstash/stash.py` & `ymlstash-1.0.1/ymlstash/stash.py`

 * *Files identical despite different names*

### Comparing `ymlstash-1.0.0/PKG-INFO` & `ymlstash-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ymlstash
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple ORM-like utility for operating on local YAML files via Python dataclasses
 License: MIT
 Author: Yuval Adam
 Author-email: _@yuv.al
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,24 @@
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Description-Content-Type: text/markdown
 
 # ymlstash
 
 A simple ORM-like utility for operating on local YAML files via Python dataclasses.
 
+## Install
+
+Package is published on PyPI - https://pypi.org/project/ymlstash/
+
+Install from pip or your favorite package manager:
+
+```bash
+$ pip install ymlstash
+```
+
 ## Usage
 
 Define a dataclass:
 
 ```python
 from dataclasses import dataclass
 from typing import ClassVar
```

