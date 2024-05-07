# Comparing `tmp/mkdocs_d2_plugin-1.3.1.tar.gz` & `tmp/mkdocs_d2_plugin-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_d2_plugin-1.3.1.tar", last modified: Tue May  7 15:46:30 2024, max compression
+gzip compressed data, was "mkdocs_d2_plugin-1.3.2.tar", last modified: Tue May  7 18:47:38 2024, max compression
```

## Comparing `mkdocs_d2_plugin-1.3.1.tar` & `mkdocs_d2_plugin-1.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 landmaj    (501) staff       (20)        0 2024-05-07 15:46:30.104122 mkdocs_d2_plugin-1.3.1/
--rw-r--r--   0 landmaj    (501) staff       (20)     1061 2024-04-17 23:00:44.000000 mkdocs_d2_plugin-1.3.1/LICENSE
--rw-r--r--   0 landmaj    (501) staff       (20)     2170 2024-05-07 15:46:30.103923 mkdocs_d2_plugin-1.3.1/PKG-INFO
--rw-r--r--   0 landmaj    (501) staff       (20)     1153 2024-04-17 23:00:44.000000 mkdocs_d2_plugin-1.3.1/README.md
-drwxr-xr-x   0 landmaj    (501) staff       (20)        0 2024-05-07 15:46:30.102620 mkdocs_d2_plugin-1.3.1/d2/
--rw-r--r--   0 landmaj    (501) staff       (20)      318 2024-04-17 23:00:44.000000 mkdocs_d2_plugin-1.3.1/d2/__init__.py
--rw-r--r--   0 landmaj    (501) staff       (20)     1729 2024-04-17 23:00:44.000000 mkdocs_d2_plugin-1.3.1/d2/config.py
--rw-r--r--   0 landmaj    (501) staff       (20)     1713 2024-04-17 23:00:44.000000 mkdocs_d2_plugin-1.3.1/d2/fence.py
--rw-r--r--   0 landmaj    (501) staff       (20)     2556 2024-05-07 15:26:23.000000 mkdocs_d2_plugin-1.3.1/d2/img.py
--rw-r--r--   0 landmaj    (501) staff       (20)     3674 2024-05-03 14:53:55.000000 mkdocs_d2_plugin-1.3.1/d2/plugin.py
-drwxr-xr-x   0 landmaj    (501) staff       (20)        0 2024-05-07 15:46:30.103720 mkdocs_d2_plugin-1.3.1/mkdocs_d2_plugin.egg-info/
--rw-r--r--   0 landmaj    (501) staff       (20)     2170 2024-05-07 15:46:30.000000 mkdocs_d2_plugin-1.3.1/mkdocs_d2_plugin.egg-info/PKG-INFO
--rw-r--r--   0 landmaj    (501) staff       (20)      331 2024-05-07 15:46:30.000000 mkdocs_d2_plugin-1.3.1/mkdocs_d2_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 landmaj    (501) staff       (20)        1 2024-05-07 15:46:30.000000 mkdocs_d2_plugin-1.3.1/mkdocs_d2_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 landmaj    (501) staff       (20)       93 2024-05-07 15:46:30.000000 mkdocs_d2_plugin-1.3.1/mkdocs_d2_plugin.egg-info/entry_points.txt
--rw-r--r--   0 landmaj    (501) staff       (20)       62 2024-05-07 15:46:30.000000 mkdocs_d2_plugin-1.3.1/mkdocs_d2_plugin.egg-info/requires.txt
--rw-r--r--   0 landmaj    (501) staff       (20)        3 2024-05-07 15:46:30.000000 mkdocs_d2_plugin-1.3.1/mkdocs_d2_plugin.egg-info/top_level.txt
--rw-r--r--   0 landmaj    (501) staff       (20)       38 2024-05-07 15:46:30.104167 mkdocs_d2_plugin-1.3.1/setup.cfg
--rw-r--r--   0 landmaj    (501) staff       (20)     1492 2024-05-07 15:27:11.000000 mkdocs_d2_plugin-1.3.1/setup.py
+drwxr-xr-x   0 landmaj    (501) staff       (20)        0 2024-05-07 18:47:38.449966 mkdocs_d2_plugin-1.3.2/
+-rw-r--r--   0 landmaj    (501) staff       (20)     1061 2024-04-17 23:00:44.000000 mkdocs_d2_plugin-1.3.2/LICENSE
+-rw-r--r--   0 landmaj    (501) staff       (20)     2170 2024-05-07 18:47:38.449730 mkdocs_d2_plugin-1.3.2/PKG-INFO
+-rw-r--r--   0 landmaj    (501) staff       (20)     1153 2024-04-17 23:00:44.000000 mkdocs_d2_plugin-1.3.2/README.md
+drwxr-xr-x   0 landmaj    (501) staff       (20)        0 2024-05-07 18:47:38.448285 mkdocs_d2_plugin-1.3.2/d2/
+-rw-r--r--   0 landmaj    (501) staff       (20)      318 2024-05-07 18:40:40.000000 mkdocs_d2_plugin-1.3.2/d2/__init__.py
+-rw-r--r--   0 landmaj    (501) staff       (20)     1729 2024-05-07 18:40:40.000000 mkdocs_d2_plugin-1.3.2/d2/config.py
+-rw-r--r--   0 landmaj    (501) staff       (20)     1713 2024-05-07 18:43:40.000000 mkdocs_d2_plugin-1.3.2/d2/fence.py
+-rw-r--r--   0 landmaj    (501) staff       (20)     2569 2024-05-07 18:46:27.000000 mkdocs_d2_plugin-1.3.2/d2/img.py
+-rw-r--r--   0 landmaj    (501) staff       (20)     3690 2024-05-07 18:46:04.000000 mkdocs_d2_plugin-1.3.2/d2/plugin.py
+drwxr-xr-x   0 landmaj    (501) staff       (20)        0 2024-05-07 18:47:38.449475 mkdocs_d2_plugin-1.3.2/mkdocs_d2_plugin.egg-info/
+-rw-r--r--   0 landmaj    (501) staff       (20)     2170 2024-05-07 18:47:38.000000 mkdocs_d2_plugin-1.3.2/mkdocs_d2_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 landmaj    (501) staff       (20)      331 2024-05-07 18:47:38.000000 mkdocs_d2_plugin-1.3.2/mkdocs_d2_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 landmaj    (501) staff       (20)        1 2024-05-07 18:47:38.000000 mkdocs_d2_plugin-1.3.2/mkdocs_d2_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 landmaj    (501) staff       (20)       93 2024-05-07 18:47:38.000000 mkdocs_d2_plugin-1.3.2/mkdocs_d2_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 landmaj    (501) staff       (20)       62 2024-05-07 18:47:38.000000 mkdocs_d2_plugin-1.3.2/mkdocs_d2_plugin.egg-info/requires.txt
+-rw-r--r--   0 landmaj    (501) staff       (20)        3 2024-05-07 18:47:38.000000 mkdocs_d2_plugin-1.3.2/mkdocs_d2_plugin.egg-info/top_level.txt
+-rw-r--r--   0 landmaj    (501) staff       (20)       38 2024-05-07 18:47:38.450026 mkdocs_d2_plugin-1.3.2/setup.cfg
+-rw-r--r--   0 landmaj    (501) staff       (20)     1492 2024-05-07 18:47:09.000000 mkdocs_d2_plugin-1.3.2/setup.py
```

### Comparing `mkdocs_d2_plugin-1.3.1/LICENSE` & `mkdocs_d2_plugin-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_d2_plugin-1.3.1/PKG-INFO` & `mkdocs_d2_plugin-1.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-d2-plugin
-Version: 1.3.1
+Version: 1.3.2
 Summary: MkDocs plugin for D2
 Home-page: https://github.com/landmaj/mkdocs-d2-plugin
 Author: Michał Wieluński
 Author-email: michal@wielunski.net
 License: MIT
 Keywords: mkdocs python markdown d2 diagram
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs_d2_plugin-1.3.1/README.md` & `mkdocs_d2_plugin-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_d2_plugin-1.3.1/d2/config.py` & `mkdocs_d2_plugin-1.3.2/d2/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_d2_plugin-1.3.1/d2/fence.py` & `mkdocs_d2_plugin-1.3.2/d2/fence.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,17 +16,17 @@
     ) -> None:
         self.config = config
         self.renderer = renderer
 
     def validator(
         self,
         language: str,
-        inputs: dict[str, str],
-        options: dict[str, Any],
-        attrs: dict[str, Any],
+        inputs: Dict[str, str],
+        options: Dict[str, Any],
+        attrs: Dict[str, Any],
         md: Markdown,
     ) -> bool:
         options["render"] = falsy(inputs.pop("render", "True"))
 
         cfg = self.config.copy()
         cfg.update(**inputs)
         try:
```

### Comparing `mkdocs_d2_plugin-1.3.1/d2/img.py` & `mkdocs_d2_plugin-1.3.2/d2/img.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import xml.etree.ElementTree as etree
 from io import StringIO
 from pathlib import Path
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 
 from markdown import Extension, Markdown
 from markdown.treeprocessors import Treeprocessor
 from pydantic import ValidationError
 
 from d2 import Renderer, error, warning
 from d2.config import D2Config
@@ -20,15 +20,15 @@
         renderer: Renderer,
     ):
         self.base_dir = base_dir
         self.config = config
         self.renderer = renderer
         super().__init__(md)
 
-    def run(self, root: etree.Element) -> etree.Element | None:
+    def run(self, root: etree.Element) -> Optional[etree.Element]:
         for elem in root.iter("img"):
             src = Path(elem.get("src", ""))
             if src.suffix == ".d2":
                 diagram = Path(self.base_dir, src).resolve()
                 if not diagram.exists():
                     warning(f"File not found: {diagram}")
                     continue
```

### Comparing `mkdocs_d2_plugin-1.3.1/d2/plugin.py` & `mkdocs_d2_plugin-1.3.2/d2/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import dbm
 import os
 import subprocess
 from functools import partial
 from hashlib import sha1
 from pathlib import Path
-from typing import List, MutableMapping, Tuple
+from typing import List, MutableMapping, Optional, Tuple
 
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.exceptions import ConfigurationError
 from mkdocs.plugins import BasePlugin
 from mkdocs.utils.yaml import RelativeDirPlaceholder
 from packaging import version
 
@@ -16,15 +16,15 @@
 from d2.config import PluginConfig
 from d2.fence import D2CustomFence
 
 REQUIRED_VERSION = version.parse("0.6.3")
 
 
 class Plugin(BasePlugin[PluginConfig]):
-    def on_config(self, config: MkDocsConfig) -> MkDocsConfig | None:
+    def on_config(self, config: MkDocsConfig) -> Optional[MkDocsConfig]:
         self.cache = None
         if self.config.cache:
             if not os.path.isdir(self.config.cache_dir):
                 os.makedirs(self.config.cache_dir)
             path = Path(self.config.cache_dir, "db").as_posix()
             backend = dbm.whichdb(path)
             info(f"Using cache at {path} ({backend})")
@@ -79,15 +79,15 @@
     def on_post_build(self, config: MkDocsConfig) -> None:
         if self.cache:
             self.cache.close()
 
 
 def render(
     executable: str,
-    cache: MutableMapping[bytes, bytes] | None,
+    cache: Optional[MutableMapping[bytes, bytes]],
     source: bytes,
     opts: List[str],
 ) -> Tuple[str, bool]:
     key = ""
     if cache is not None:
         key = source.hex()
         for opt in opts:
```

### Comparing `mkdocs_d2_plugin-1.3.1/mkdocs_d2_plugin.egg-info/PKG-INFO` & `mkdocs_d2_plugin-1.3.2/mkdocs_d2_plugin.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-d2-plugin
-Version: 1.3.1
+Version: 1.3.2
 Summary: MkDocs plugin for D2
 Home-page: https://github.com/landmaj/mkdocs-d2-plugin
 Author: Michał Wieluński
 Author-email: michal@wielunski.net
 License: MIT
 Keywords: mkdocs python markdown d2 diagram
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs_d2_plugin-1.3.1/setup.py` & `mkdocs_d2_plugin-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 PROJ_DIR = Path(__file__).resolve().parent
 with open(PROJ_DIR / "README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="mkdocs-d2-plugin",
-    version="1.3.1",
+    version="1.3.2",
     description="MkDocs plugin for D2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="mkdocs python markdown d2 diagram",
     url="https://github.com/landmaj/mkdocs-d2-plugin",
     author="Michał Wieluński",
     author_email="michal@wielunski.net",
```

