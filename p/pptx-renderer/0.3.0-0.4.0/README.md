# Comparing `tmp/pptx_renderer-0.3.0.tar.gz` & `tmp/pptx_renderer-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pptx_renderer-0.3.0.tar", last modified: Thu Aug 17 07:11:35 2023, max compression
+gzip compressed data, was "pptx_renderer-0.4.0.tar", last modified: Tue May  7 12:04:16 2024, max compression
```

## Comparing `pptx_renderer-0.3.0.tar` & `pptx_renderer-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 07:11:35.737722 pptx_renderer-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-17 07:11:24.000000 pptx_renderer-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-08-17 07:11:35.737722 pptx_renderer-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-08-17 07:11:24.000000 pptx_renderer-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 07:11:35.737722 pptx_renderer-0.3.0/pptx_renderer/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-17 07:11:24.000000 pptx_renderer-0.3.0/pptx_renderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-08-17 07:11:24.000000 pptx_renderer-0.3.0/pptx_renderer/command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-17 07:11:24.000000 pptx_renderer-0.3.0/pptx_renderer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-08-17 07:11:24.000000 pptx_renderer-0.3.0/pptx_renderer/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-08-17 07:11:24.000000 pptx_renderer-0.3.0/pptx_renderer/pptx_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-08-17 07:11:24.000000 pptx_renderer-0.3.0/pptx_renderer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 07:11:35.737722 pptx_renderer-0.3.0/pptx_renderer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-08-17 07:11:35.000000 pptx_renderer-0.3.0/pptx_renderer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-17 07:11:35.000000 pptx_renderer-0.3.0/pptx_renderer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-17 07:11:35.000000 pptx_renderer-0.3.0/pptx_renderer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-17 07:11:35.000000 pptx_renderer-0.3.0/pptx_renderer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-17 07:11:35.000000 pptx_renderer-0.3.0/pptx_renderer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-17 07:11:35.000000 pptx_renderer-0.3.0/pptx_renderer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-08-17 07:11:24.000000 pptx_renderer-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-17 07:11:35.737722 pptx_renderer-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-17 07:11:24.000000 pptx_renderer-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 07:11:35.737722 pptx_renderer-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-17 07:11:24.000000 pptx_renderer-0.3.0/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-17 07:11:24.000000 pptx_renderer-0.3.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:04:16.350458 pptx_renderer-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-07 12:04:12.000000 pptx_renderer-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-07 12:04:16.350458 pptx_renderer-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-07 12:04:12.000000 pptx_renderer-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:04:16.346458 pptx_renderer-0.4.0/pptx_renderer/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-07 12:04:12.000000 pptx_renderer-0.4.0/pptx_renderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-07 12:04:12.000000 pptx_renderer-0.4.0/pptx_renderer/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-07 12:04:12.000000 pptx_renderer-0.4.0/pptx_renderer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6605 2024-05-07 12:04:12.000000 pptx_renderer-0.4.0/pptx_renderer/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-07 12:04:12.000000 pptx_renderer-0.4.0/pptx_renderer/pptx_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-07 12:04:12.000000 pptx_renderer-0.4.0/pptx_renderer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:04:16.350458 pptx_renderer-0.4.0/pptx_renderer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-07 12:04:16.000000 pptx_renderer-0.4.0/pptx_renderer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-07 12:04:16.000000 pptx_renderer-0.4.0/pptx_renderer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 12:04:16.000000 pptx_renderer-0.4.0/pptx_renderer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-07 12:04:16.000000 pptx_renderer-0.4.0/pptx_renderer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-07 12:04:16.000000 pptx_renderer-0.4.0/pptx_renderer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-07 12:04:16.000000 pptx_renderer-0.4.0/pptx_renderer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-07 12:04:12.000000 pptx_renderer-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 12:04:16.350458 pptx_renderer-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 12:04:12.000000 pptx_renderer-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:04:16.350458 pptx_renderer-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-07 12:04:12.000000 pptx_renderer-0.4.0/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-07 12:04:12.000000 pptx_renderer-0.4.0/tests/test_cli.py
```

### Comparing `pptx_renderer-0.3.0/LICENSE` & `pptx_renderer-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pptx_renderer-0.3.0/PKG-INFO` & `pptx_renderer-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pptx_renderer
-Version: 0.3.0
+Version: 0.4.0
 Summary: Render ppt like a jupyter notebook
 Author-email: Najeem Muhammed <najeem@gmail.com>
 License: MIT License
         
         Copyright (c) 2023, Najeem Muhammed
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,16 +28,21 @@
 Project-URL: Bug Tracker, https://github.com/idling-mind/pptx_renderer/issues
 Keywords: powerpoint,ppt,pptx,presentation,slides
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: python-pptx
+Requires-Dist: click
+Requires-Dist: Pillow>=9.3
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: coverage; extra == "test"
 
 # PPTX Renderer
 
 This package let's you run your powerpoint presentations like a jupyter-notebook.
 You can insert placeholders in the ppt and also write python code in the ppt's
 notes and use either a python function or an equivalent commandline tool to
 convert it into an output rendered presentation.
```

### Comparing `pptx_renderer-0.3.0/README.md` & `pptx_renderer-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pptx_renderer-0.3.0/pptx_renderer/command_line.py` & `pptx_renderer-0.4.0/pptx_renderer/command_line.py`

 * *Files identical despite different names*

### Comparing `pptx_renderer-0.3.0/pptx_renderer/pptx_renderer.py` & `pptx_renderer-0.4.0/pptx_renderer/pptx_renderer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Main Module"""
 
 import re
 from os import PathLike
 from pathlib import Path
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, Optional, Union, Callable
 from warnings import warn as warning
 from functools import partial
 from . import plugins
 
 from pptx import Presentation
 from pptx.enum.shapes import MSO_SHAPE_TYPE
 
@@ -28,21 +28,23 @@
 
     def __init__(self, template_path: Union[str, PathLike]):
         self.template_path = template_path
         self.plugins = {}
         self.namespace = {}
         for plugin in PLUGINS:
             self.register_plugin(plugin.__name__, plugin)
-    
-    def register_plugin(self, name: str, func: callable):
+
+    def register_plugin(self, name: str, func: Callable):
         """Register a plugin function.
 
         The plugin function should take 2 or more arguments. The first argument
         is the result of evaluating the python statement. The second argument is
         a dictionary containing the following keys:
+        - result: The result of evaluating the python statement
+        - presentation: The output pptx presentation object
         - shape: The pptx shape object where the placeholder is present
         - slide: The pptx slide object where the placeholder is present
         - slide_no: The slide number where the placeholder is present
         The remaining arguments are the arguments passed to the plugin function
 
         Args:
             name (str): Name of the plugin.
@@ -89,15 +91,15 @@
                     handle_shapes(shape.shapes)
 
         def handle_text_frame(shape):
             matches = re.finditer(r"{{{(.*)}}}", shape.text)
             if not matches:
                 return
             for match_assignment in matches:
-                parts = match_assignment.group(1).split(":")
+                parts = match_assignment.group(1).split(":", 1)
                 try:
                     result = eval(fix_quotes(parts[0]), self.namespace)
                 except Exception as ex:
                     if skip_failed:
                         warning(
                             f"Evaluation of '{parts[0]}' in slide {slide_no+1} failed"
                         )
@@ -137,15 +139,15 @@
         def handle_table(shape):
             for row in shape.table.rows:
                 for cell in row.cells:
                     matches = re.finditer(r"{{{(.*)}}}", cell.text)
                     if not matches:
                         continue
                     for match_assignment in matches:
-                        parts = match_assignment.group(1).split(":")
+                        parts = match_assignment.group(1).split(":", 1)
                         try:
                             result = eval(fix_quotes(parts[0]), self.namespace)
                         except Exception as ex:
                             if skip_failed:
                                 warning(
                                     f"Evaluation of '{parts[0]}' in slide {slide_no+1} failed"
                                 )
```

### Comparing `pptx_renderer-0.3.0/pptx_renderer/utils.py` & `pptx_renderer-0.4.0/pptx_renderer/utils.py`

 * *Files identical despite different names*

### Comparing `pptx_renderer-0.3.0/pptx_renderer.egg-info/PKG-INFO` & `pptx_renderer-0.4.0/pptx_renderer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pptx-renderer
-Version: 0.3.0
+Name: pptx_renderer
+Version: 0.4.0
 Summary: Render ppt like a jupyter notebook
 Author-email: Najeem Muhammed <najeem@gmail.com>
 License: MIT License
         
         Copyright (c) 2023, Najeem Muhammed
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,16 +28,21 @@
 Project-URL: Bug Tracker, https://github.com/idling-mind/pptx_renderer/issues
 Keywords: powerpoint,ppt,pptx,presentation,slides
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: python-pptx
+Requires-Dist: click
+Requires-Dist: Pillow>=9.3
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: coverage; extra == "test"
 
 # PPTX Renderer
 
 This package let's you run your powerpoint presentations like a jupyter-notebook.
 You can insert placeholders in the ppt and also write python code in the ppt's
 notes and use either a python function or an equivalent commandline tool to
 convert it into an output rendered presentation.
```

### Comparing `pptx_renderer-0.3.0/pyproject.toml` & `pptx_renderer-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pptx_renderer-0.3.0/tests/test_basic.py` & `pptx_renderer-0.4.0/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `pptx_renderer-0.3.0/tests/test_cli.py` & `pptx_renderer-0.4.0/tests/test_cli.py`

 * *Files identical despite different names*

