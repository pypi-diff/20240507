# Comparing `tmp/jinjax-0.35.tar.gz` & `tmp/jinjax-0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinjax-0.35.tar", max compression
+gzip compressed data, was "jinjax-0.36.tar", max compression
```

## Comparing `jinjax-0.35.tar` & `jinjax-0.36.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      497 2024-04-30 22:45:12.583815 jinjax-0.35/README.md
--rw-r--r--   0        0        0     3839 2024-04-30 22:45:12.591815 jinjax-0.35/pyproject.toml
--rw-r--r--   0        0        0      189 2024-04-30 22:45:12.591815 jinjax-0.35/src/jinjax/__init__.py
--rw-r--r--   0        0        0    13762 2024-04-30 22:45:12.591815 jinjax-0.35/src/jinjax/catalog.py
--rw-r--r--   0        0        0     6416 2024-04-30 22:45:12.591815 jinjax-0.35/src/jinjax/component.py
--rw-r--r--   0        0        0      409 2024-04-30 22:45:12.591815 jinjax-0.35/src/jinjax/exceptions.py
--rw-r--r--   0        0        0     5289 2024-04-30 22:45:12.591815 jinjax-0.35/src/jinjax/html_attrs.py
--rw-r--r--   0        0        0     4657 2024-04-30 22:45:12.591815 jinjax-0.35/src/jinjax/jinjax.py
--rw-r--r--   0        0        0     1304 2024-04-30 22:45:12.591815 jinjax-0.35/src/jinjax/middleware.py
--rw-r--r--   0        0        0        0 2024-04-30 22:45:12.591815 jinjax-0.35/src/jinjax/py.typed
--rw-r--r--   0        0        0       54 2024-04-30 22:45:12.591815 jinjax-0.35/src/jinjax/utils.py
--rw-r--r--   0        0        0     1848 1970-01-01 00:00:00.000000 jinjax-0.35/PKG-INFO
+-rw-r--r--   0        0        0      497 2024-05-07 20:49:16.440922 jinjax-0.36/README.md
+-rw-r--r--   0        0        0     3839 2024-05-07 20:49:16.448922 jinjax-0.36/pyproject.toml
+-rw-r--r--   0        0        0      189 2024-05-07 20:49:16.448922 jinjax-0.36/src/jinjax/__init__.py
+-rw-r--r--   0        0        0    13752 2024-05-07 20:49:16.448922 jinjax-0.36/src/jinjax/catalog.py
+-rw-r--r--   0        0        0     6897 2024-05-07 20:49:16.448922 jinjax-0.36/src/jinjax/component.py
+-rw-r--r--   0        0        0      409 2024-05-07 20:49:16.448922 jinjax-0.36/src/jinjax/exceptions.py
+-rw-r--r--   0        0        0     5289 2024-05-07 20:49:16.448922 jinjax-0.36/src/jinjax/html_attrs.py
+-rw-r--r--   0        0        0     4657 2024-05-07 20:49:16.448922 jinjax-0.36/src/jinjax/jinjax.py
+-rw-r--r--   0        0        0     1304 2024-05-07 20:49:16.448922 jinjax-0.36/src/jinjax/middleware.py
+-rw-r--r--   0        0        0        0 2024-05-07 20:49:16.448922 jinjax-0.36/src/jinjax/py.typed
+-rw-r--r--   0        0        0       83 2024-05-07 20:49:16.448922 jinjax-0.36/src/jinjax/utils.py
+-rw-r--r--   0        0        0     1848 1970-01-01 00:00:00.000000 jinjax-0.36/PKG-INFO
```

### Comparing `jinjax-0.35/pyproject.toml` & `jinjax-0.36/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "jinjax"
-version = "0.35"
+version = "0.36"
 description = "Replace your HTML templates with Python server-Side components"
 authors = ["Juan-Pablo Scaletti <juanpablo@jpscaletti.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://jinjax.scaletti.dev/"
 repository = "https://github.com/jpsca/jinjax"
 documentation = "https://jinjax.scaletti.dev/guides/"
```

### Comparing `jinjax-0.35/src/jinjax/catalog.py` & `jinjax-0.36/src/jinjax/catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,25 +7,23 @@
 from markupsafe import Markup
 
 from .component import Component
 from .exceptions import ComponentNotFound, InvalidArgument
 from .html_attrs import HTMLAttrs
 from .jinjax import JinjaX
 from .middleware import ComponentsMiddleware
-from .utils import logger
+from .utils import DELIMITER, SLASH, logger
 
 
 TFileExt = t.Union[tuple[str, ...], str]
 
 DEFAULT_URL_ROOT = "/static/components/"
 ALLOWED_EXTENSIONS = (".css", ".js", ".mjs")
 DEFAULT_PREFIX = ""
 DEFAULT_EXTENSION = ".jinja"
-DELIMITER = "."
-SLASH = "/"
 PROP_ATTRS = "attrs"
 PROP_CONTENT = "content"
 
 
 class Catalog:
     """
     Attributes:
```

### Comparing `jinjax-0.35/src/jinjax/component.py` & `jinjax-0.36/src/jinjax/component.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from keyword import iskeyword
 from pathlib import Path
 
 from jinja2 import Template
 from markupsafe import Markup
 
 from .exceptions import InvalidArgument, MissingRequiredArgument
+from .utils import DELIMITER
 
 
 if t.TYPE_CHECKING:
     from typing_extensions import Self
 
 
 RX_PROPS_START = re.compile(r"{#-?\s*def\s+")
@@ -79,14 +80,26 @@
 
         if path is not None:
             source = source or path.read_text()
             mtime = mtime or path.stat().st_mtime
         if source:
             self.load_metadata(source)
 
+        if path is not None:
+            folder = path.parent
+            default_name = self.name.rsplit(DELIMITER, 1)[-1]
+
+            default_css = f"{default_name}.css"
+            if (folder / default_css).is_file():
+                self.css.extend(self.parse_files_expr(default_css))
+
+            default_js = f"{default_name}.js"
+            if (folder / default_js).is_file():
+                self.js.extend(self.parse_files_expr(default_js))
+
         self.path = path
         self.mtime = mtime
         self.tmpl = tmpl
 
     @classmethod
     def from_cache(
         cls,
```

### Comparing `jinjax-0.35/src/jinjax/html_attrs.py` & `jinjax-0.36/src/jinjax/html_attrs.py`

 * *Files identical despite different names*

### Comparing `jinjax-0.35/src/jinjax/jinjax.py` & `jinjax-0.36/src/jinjax/jinjax.py`

 * *Files identical despite different names*

### Comparing `jinjax-0.35/src/jinjax/middleware.py` & `jinjax-0.36/src/jinjax/middleware.py`

 * *Files identical despite different names*

### Comparing `jinjax-0.35/PKG-INFO` & `jinjax-0.36/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinjax
-Version: 0.35
+Version: 0.36
 Summary: Replace your HTML templates with Python server-Side components
 Home-page: https://jinjax.scaletti.dev/
 License: MIT
 Author: Juan-Pablo Scaletti
 Author-email: juanpablo@jpscaletti.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

