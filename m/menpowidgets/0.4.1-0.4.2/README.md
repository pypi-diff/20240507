# Comparing `tmp/menpowidgets-0.4.1.tar.gz` & `tmp/menpowidgets-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "menpowidgets-0.4.1.tar", last modified: Sun Apr 18 20:46:52 2021, max compression
+gzip compressed data, was "menpowidgets-0.4.2.tar", last modified: Tue May  7 11:48:24 2024, max compression
```

## Comparing `menpowidgets-0.4.1.tar` & `menpowidgets-0.4.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-04-18 20:46:52.328145 menpowidgets-0.4.1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      485 2021-04-18 20:43:47.000000 menpowidgets-0.4.1/AUTHORS.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1643 2021-04-18 20:43:47.000000 menpowidgets-0.4.1/LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       40 2021-04-18 20:43:47.000000 menpowidgets-0.4.1/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)      253 2021-04-18 20:46:52.328145 menpowidgets-0.4.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2084 2021-04-18 20:43:47.000000 menpowidgets-0.4.1/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-04-18 20:46:52.328145 menpowidgets-0.4.1/menpowidgets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      543 2021-04-18 20:43:47.000000 menpowidgets-0.4.1/menpowidgets/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2021-04-18 20:46:52.328145 menpowidgets-0.4.1/menpowidgets/_static_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6088 2021-04-18 20:43:47.000000 menpowidgets-0.4.1/menpowidgets/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5780 2021-04-18 20:43:47.000000 menpowidgets-0.4.1/menpowidgets/abstract.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)   117279 2021-04-18 20:43:47.000000 menpowidgets-0.4.1/menpowidgets/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1077 2021-04-18 20:43:47.000000 menpowidgets-0.4.1/menpowidgets/checks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3520 2021-04-18 20:43:47.000000 menpowidgets-0.4.1/menpowidgets/items.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-04-18 20:46:52.328145 menpowidgets-0.4.1/menpowidgets/js/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5151 2021-04-18 20:43:47.000000 menpowidgets-0.4.1/menpowidgets/js/webcam.js
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-04-18 20:46:52.328145 menpowidgets-0.4.1/menpowidgets/logos/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9466 2021-04-18 20:43:47.000000 menpowidgets-0.4.1/menpowidgets/logos/menpoproject_danger.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9772 2021-04-18 20:43:47.000000 menpowidgets-0.4.1/menpowidgets/logos/menpoproject_info.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7957 2021-04-18 20:43:47.000000 menpowidgets-0.4.1/menpowidgets/logos/menpoproject_minimal.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9717 2021-04-18 20:43:47.000000 menpowidgets-0.4.1/menpowidgets/logos/menpoproject_success.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9658 2021-04-18 20:43:47.000000 menpowidgets-0.4.1/menpowidgets/logos/menpoproject_warning.png
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-04-18 20:46:52.328145 menpowidgets-0.4.1/menpowidgets/menpofitwidgets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      437 2021-04-18 20:43:47.000000 menpowidgets-0.4.1/menpowidgets/menpofitwidgets/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    92849 2021-04-18 20:43:47.000000 menpowidgets-0.4.1/menpowidgets/menpofitwidgets/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)   268757 2021-04-18 20:43:47.000000 menpowidgets-0.4.1/menpowidgets/options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2408 2021-04-18 20:43:47.000000 menpowidgets-0.4.1/menpowidgets/style.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)   212154 2021-04-18 20:43:47.000000 menpowidgets-0.4.1/menpowidgets/tools.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    28321 2021-04-18 20:43:47.000000 menpowidgets-0.4.1/menpowidgets/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-04-18 20:46:52.328145 menpowidgets-0.4.1/menpowidgets.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      253 2021-04-18 20:46:52.000000 menpowidgets-0.4.1/menpowidgets.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      816 2021-04-18 20:46:52.000000 menpowidgets-0.4.1/menpowidgets.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-04-18 20:46:52.000000 menpowidgets-0.4.1/menpowidgets.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       23 2021-04-18 20:46:52.000000 menpowidgets-0.4.1/menpowidgets.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       13 2021-04-18 20:46:52.000000 menpowidgets-0.4.1/menpowidgets.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2021-04-18 20:46:52.328145 menpowidgets-0.4.1/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      918 2021-04-18 20:43:47.000000 menpowidgets-0.4.1/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:48:24.639841 menpowidgets-0.4.2/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      485 2024-05-07 11:45:18.000000 menpowidgets-0.4.2/AUTHORS.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1643 2024-05-07 11:45:18.000000 menpowidgets-0.4.2/LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       40 2024-05-07 11:45:18.000000 menpowidgets-0.4.2/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      283 2024-05-07 11:48:24.635841 menpowidgets-0.4.2/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2084 2024-05-07 11:45:18.000000 menpowidgets-0.4.2/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:48:24.639841 menpowidgets-0.4.2/menpowidgets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      543 2024-05-07 11:45:18.000000 menpowidgets-0.4.2/menpowidgets/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2024-05-07 11:48:24.639841 menpowidgets-0.4.2/menpowidgets/_static_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6088 2024-05-07 11:45:18.000000 menpowidgets-0.4.2/menpowidgets/_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5780 2024-05-07 11:45:18.000000 menpowidgets-0.4.2/menpowidgets/abstract.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   117283 2024-05-07 11:45:18.000000 menpowidgets-0.4.2/menpowidgets/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1077 2024-05-07 11:45:18.000000 menpowidgets-0.4.2/menpowidgets/checks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3522 2024-05-07 11:45:18.000000 menpowidgets-0.4.2/menpowidgets/items.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:48:24.635841 menpowidgets-0.4.2/menpowidgets/js/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5151 2024-05-07 11:45:18.000000 menpowidgets-0.4.2/menpowidgets/js/webcam.js
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:48:24.635841 menpowidgets-0.4.2/menpowidgets/logos/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9466 2024-05-07 11:45:18.000000 menpowidgets-0.4.2/menpowidgets/logos/menpoproject_danger.png
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9772 2024-05-07 11:45:18.000000 menpowidgets-0.4.2/menpowidgets/logos/menpoproject_info.png
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7957 2024-05-07 11:45:18.000000 menpowidgets-0.4.2/menpowidgets/logos/menpoproject_minimal.png
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9717 2024-05-07 11:45:18.000000 menpowidgets-0.4.2/menpowidgets/logos/menpoproject_success.png
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9658 2024-05-07 11:45:18.000000 menpowidgets-0.4.2/menpowidgets/logos/menpoproject_warning.png
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:48:24.635841 menpowidgets-0.4.2/menpowidgets/menpofitwidgets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      437 2024-05-07 11:45:18.000000 menpowidgets-0.4.2/menpowidgets/menpofitwidgets/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    93228 2024-05-07 11:45:18.000000 menpowidgets-0.4.2/menpowidgets/menpofitwidgets/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   268404 2024-05-07 11:45:18.000000 menpowidgets-0.4.2/menpowidgets/options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2408 2024-05-07 11:45:18.000000 menpowidgets-0.4.2/menpowidgets/style.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   212121 2024-05-07 11:45:18.000000 menpowidgets-0.4.2/menpowidgets/tools.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    28731 2024-05-07 11:45:18.000000 menpowidgets-0.4.2/menpowidgets/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 11:48:24.635841 menpowidgets-0.4.2/menpowidgets.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      283 2024-05-07 11:48:24.000000 menpowidgets-0.4.2/menpowidgets.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      816 2024-05-07 11:48:24.000000 menpowidgets-0.4.2/menpowidgets.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-05-07 11:48:24.000000 menpowidgets-0.4.2/menpowidgets.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       23 2024-05-07 11:48:24.000000 menpowidgets-0.4.2/menpowidgets.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       13 2024-05-07 11:48:24.000000 menpowidgets-0.4.2/menpowidgets.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2024-05-07 11:48:24.639841 menpowidgets-0.4.2/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      918 2024-05-07 11:45:18.000000 menpowidgets-0.4.2/setup.py
```

### Comparing `menpowidgets-0.4.1/LICENSE.txt` & `menpowidgets-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `menpowidgets-0.4.1/README.md` & `menpowidgets-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `menpowidgets-0.4.1/menpowidgets/__init__.py` & `menpowidgets-0.4.2/menpowidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `menpowidgets-0.4.1/menpowidgets/_version.py` & `menpowidgets-0.4.2/menpowidgets/_version.py`

 * *Files identical despite different names*

### Comparing `menpowidgets-0.4.1/menpowidgets/abstract.py` & `menpowidgets-0.4.2/menpowidgets/abstract.py`

 * *Files identical despite different names*

### Comparing `menpowidgets-0.4.1/menpowidgets/base.py` & `menpowidgets-0.4.2/menpowidgets/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from collections import Sized, OrderedDict
+from collections import OrderedDict
+from collections.abc import Sized
+
 import matplotlib.pyplot as plt
 from matplotlib import collections as mc
 import numpy as np
 
 import ipywidgets
 import IPython.display as ipydisplay
 
@@ -248,15 +250,15 @@
     header_wid.layout.align_items = "center"
     header_wid.layout.margin = "0px 0px 10px 0px"
 
     options_box = ipywidgets.Tab(
         [info_wid, shape_options_wid, renderer_options_wid, save_figure_wid]
     )
     tab_titles = ["Info", "Shape", "Renderer", "Export"]
-    for (k, tl) in enumerate(tab_titles):
+    for k, tl in enumerate(tab_titles):
         options_box.set_title(k, tl)
 
     output.layout.align_self = "center"
     wid = ipywidgets.VBox([header_wid, options_box, output])
 
     # Set widget's style
     wid.box_style = main_style
@@ -475,15 +477,15 @@
         # Header widget
         header_wid = LogoWidget(style=main_style)
         header_wid.layout.margin = "0px 10px 0px 0px"
     options_box = ipywidgets.Tab(
         [info_wid, shape_options_wid, renderer_options_wid, save_figure_wid]
     )
     tab_titles = ["Info", "Shape", "Renderer", "Export"]
-    for (k, tl) in enumerate(tab_titles):
+    for k, tl in enumerate(tab_titles):
         options_box.set_title(k, tl)
 
     output.layout.align_self = "center"
     wid = ipywidgets.VBox([header_wid, options_box, output])
 
     # Set widget's style
     wid.box_style = main_style
@@ -682,15 +684,15 @@
         # Header widget
         header_wid = LogoWidget(style=main_style)
         header_wid.layout.margin = "0px 10px 0px 0px"
     options_box = ipywidgets.Tab(
         children=[info_wid, landmark_options_wid, renderer_options_wid, save_figure_wid]
     )
     tab_titles = ["Info", "Landmarks", "Renderer", "Export"]
-    for (k, tl) in enumerate(tab_titles):
+    for k, tl in enumerate(tab_titles):
         options_box.set_title(k, tl)
 
     output.layout.align_self = "center"
     wid = ipywidgets.VBox([header_wid, options_box, output])
 
     # Set widget's style
     wid.box_style = main_style
@@ -904,15 +906,15 @@
         # Header widget
         header_wid = LogoWidget(style=main_style)
         header_wid.layout.margin = "0px 10px 0px 0px"
     options_box = ipywidgets.Tab(
         children=[info_wid, landmark_options_wid, renderer_options_wid, save_figure_wid]
     )
     tab_titles = ["Info", "Landmarks", "Renderer", "Export"]
-    for (k, tl) in enumerate(tab_titles):
+    for k, tl in enumerate(tab_titles):
         options_box.set_title(k, tl)
 
     output.layout.align_self = "center"
     wid = ipywidgets.VBox([header_wid, options_box, output])
 
     # Set widget's style
     wid.box_style = main_style
@@ -1071,15 +1073,15 @@
         header_wid.layout.margin = "0px 0px 10px 0px"
     else:
         # Header widget
         header_wid = LogoWidget(style=main_style)
         header_wid.layout.margin = "0px 10px 0px 0px"
     options_box = ipywidgets.Tab([info_wid, mesh_options_wid, save_figure_wid])
     tab_titles = ["Info", "Mesh", "Export"]
-    for (k, tl) in enumerate(tab_titles):
+    for k, tl in enumerate(tab_titles):
         options_box.set_title(k, tl)
 
     output.layout.align_self = "center"
     wid = ipywidgets.VBox([header_wid, options_box, output])
 
     # Set widget's style
     wid.box_style = main_style
@@ -1291,15 +1293,15 @@
             image_options_wid,
             landmark_options_wid,
             renderer_options_wid,
             save_figure_wid,
         ]
     )
     tab_titles = ["Info", "Image", "Landmarks", "Renderer", "Export"]
-    for (k, tl) in enumerate(tab_titles):
+    for k, tl in enumerate(tab_titles):
         options_box.set_title(k, tl)
 
     # Set widget's style
     output.layout.align_self = "center"
     wid = ipywidgets.VBox([header_wid, options_box, output])
     wid.box_style = main_style
     wid.layout.border = "2px solid " + map_styles_to_hex_colours(main_style)
@@ -1518,15 +1520,15 @@
             image_options_wid,
             shape_options_wid,
             renderer_options_wid,
             save_figure_wid,
         ]
     )
     tab_titles = ["Info", "Patches", "Image", "Shape", "Renderer", "Export"]
-    for (k, tl) in enumerate(tab_titles):
+    for k, tl in enumerate(tab_titles):
         options_box.set_title(k, tl)
 
     output.layout.align_self = "center"
     wid = ipywidgets.VBox([header_wid, options_box, output])
 
     # Set widget's style
     wid.box_style = main_style
@@ -2027,15 +2029,15 @@
             shape_options_wid,
             renderer_options_wid,
             info_wid,
             save_figure_wid,
         ]
     )
     tab_titles = ["Model", "Shape", "Renderer", "Info", "Export"]
-    for (k, tl) in enumerate(tab_titles):
+    for k, tl in enumerate(tab_titles):
         options_box.set_title(k, tl)
     logo_wid = LogoWidget(style=main_style)
     logo_wid.layout.margin = "0px 10px 0px 0px"
 
     output.layout.align_self = "center"
     wid = ipywidgets.VBox([logo_wid, options_box, output])
 
@@ -2258,15 +2260,15 @@
                 shape_options_wid,
                 renderer_options_wid,
                 info_wid,
                 save_figure_wid,
             ]
         )
         tab_titles = ["Model", "Shape", "Renderer", "Info", "Export"]
-    for (k, tl) in enumerate(tab_titles):
+    for k, tl in enumerate(tab_titles):
         options_box.set_title(k, tl)
     logo_wid = LogoWidget(style=main_style)
     logo_wid.layout.margin = "0px 10px 0px 0px"
 
     output.layout.align_self = "center"
     wid = ipywidgets.VBox([logo_wid, options_box, output])
 
@@ -2533,15 +2535,15 @@
             landmark_options_wid,
             renderer_options_wid,
             info_wid,
             save_figure_wid,
         ]
     )
     tab_titles = ["Model", "Image", "Landmarks", "Renderer", "Info", "Export"]
-    for (k, tl) in enumerate(tab_titles):
+    for k, tl in enumerate(tab_titles):
         options_box.set_title(k, tl)
     logo_wid = LogoWidget(style=main_style)
     logo_wid.layout.margin = "0px 10px 0px 0px"
 
     output.layout.align_self = "center"
     wid = ipywidgets.VBox([logo_wid, options_box, output])
 
@@ -2804,15 +2806,15 @@
             shape_options_wid,
             renderer_options_wid,
             info_wid,
             save_figure_wid,
         ]
     )
     tab_titles = ["Model", "Patches", "Channels", "Shape", "Renderer", "Info", "Export"]
-    for (k, tl) in enumerate(tab_titles):
+    for k, tl in enumerate(tab_titles):
         options_box.set_title(k, tl)
     logo_wid = LogoWidget(style=main_style)
     logo_wid.layout.margin = "0px 10px 0px 0px"
 
     output.layout.align_self = "center"
     wid = ipywidgets.VBox([logo_wid, options_box, output])
 
@@ -2983,15 +2985,15 @@
     )
     model_parameters_wid.children[0].set_title(0, "Shape")
     model_parameters_wid.children[0].set_title(1, "Texture")
     options_box = ipywidgets.Tab(
         [model_parameters_wid, mesh_options_wid, info_wid, save_figure_wid]
     )
     tab_titles = ["Model", "Mesh", "Info", "Export"]
-    for (k, tl) in enumerate(tab_titles):
+    for k, tl in enumerate(tab_titles):
         options_box.set_title(k, tl)
     logo_wid = LogoWidget(style=main_style)
     logo_wid.layout.margin = "0px 10px 0px 0px"
 
     output.layout.align_self = "center"
     wid = ipywidgets.VBox([logo_wid, options_box, output])
```

### Comparing `menpowidgets-0.4.1/menpowidgets/checks.py` & `menpowidgets-0.4.2/menpowidgets/checks.py`

 * *Files identical despite different names*

### Comparing `menpowidgets-0.4.1/menpowidgets/items.py` & `menpowidgets-0.4.2/menpowidgets/items.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from collections import Sized
+from collections.abc import Sized
 
 from menpo.image import Image
 from menpo.landmark import LandmarkManager
 from menpo.shape import PointCloud, TriMesh
 from menpo.model import PCAModel
 
 
@@ -82,15 +82,15 @@
             PCAModel,
             visualize_shape_model_3d,
             lambda m: isinstance(m.template_instance, PointCloud)
             and m.template_instance.n_dims == 3,
         ),
     ]
 
-    for (cls, widget, test) in cls_to_items_widget:
+    for cls, widget, test in cls_to_items_widget:
         if isinstance(template, cls) and (test is None or test(template)):
             return widget(items, **kwargs)
 
     raise ValueError(
         "No suitable list visualization found for type {} - valid types are "
         "{} or subclasses thereof".format(
             type(template), ", ".format([x[0] for x in cls_to_items_widget])
```

### Comparing `menpowidgets-0.4.1/menpowidgets/js/webcam.js` & `menpowidgets-0.4.2/menpowidgets/js/webcam.js`

 * *Files identical despite different names*

### Comparing `menpowidgets-0.4.1/menpowidgets/logos/menpoproject_danger.png` & `menpowidgets-0.4.2/menpowidgets/logos/menpoproject_danger.png`

 * *Files identical despite different names*

### Comparing `menpowidgets-0.4.1/menpowidgets/logos/menpoproject_info.png` & `menpowidgets-0.4.2/menpowidgets/logos/menpoproject_info.png`

 * *Files identical despite different names*

### Comparing `menpowidgets-0.4.1/menpowidgets/logos/menpoproject_minimal.png` & `menpowidgets-0.4.2/menpowidgets/logos/menpoproject_minimal.png`

 * *Files identical despite different names*

### Comparing `menpowidgets-0.4.1/menpowidgets/logos/menpoproject_success.png` & `menpowidgets-0.4.2/menpowidgets/logos/menpoproject_success.png`

 * *Files identical despite different names*

### Comparing `menpowidgets-0.4.1/menpowidgets/logos/menpoproject_warning.png` & `menpowidgets-0.4.2/menpowidgets/logos/menpoproject_warning.png`

 * *Files identical despite different names*

### Comparing `menpowidgets-0.4.1/menpowidgets/menpofitwidgets/base.py` & `menpowidgets-0.4.2/menpowidgets/menpofitwidgets/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,19 +372,20 @@
             landmark_options_wid,
             renderer_options_wid,
             info_wid,
             save_figure_wid,
         ]
     )
     tab_titles = ["Model", "Image", "Landmarks", "Renderer", "Info", "Export"]
-    for (k, tl) in enumerate(tab_titles):
+    for k, tl in enumerate(tab_titles):
         options_box.set_title(k, tl)
     logo_wid = LogoWidget(style=main_style)
     logo_wid.layout.margin = "0px 10px 0px 0px"
-    wid = ipywidgets.HBox([logo_wid, options_box])
+    output.layout.align_self = "center"
+    wid = ipywidgets.HBox([logo_wid, options_box, output])
 
     # Set widget's style
     wid.box_style = main_style
     wid.layout.border = "2px solid " + map_styles_to_hex_colours(main_style)
 
     # Display final widget
     final_box = ipywidgets.Box([wid])
@@ -708,19 +709,20 @@
             shape_options_wid,
             renderer_options_wid,
             info_wid,
             save_figure_wid,
         ]
     )
     tab_titles = ["Model", "Patches", "Channels", "Shape", "Renderer", "Info", "Export"]
-    for (k, tl) in enumerate(tab_titles):
+    for k, tl in enumerate(tab_titles):
         options_box.set_title(k, tl)
     logo_wid = LogoWidget(style=main_style)
     logo_wid.layout.margin = "0px 10px 0px 0px"
-    wid = ipywidgets.HBox([logo_wid, options_box])
+    output.layout.align_self = "center"
+    wid = ipywidgets.HBox([logo_wid, options_box, output])
 
     # Set widget's style
     wid.box_style = main_style
     wid.layout.border = "2px solid " + map_styles_to_hex_colours(main_style)
 
     # Display final widget
     final_box = ipywidgets.Box([wid])
@@ -984,19 +986,20 @@
             landmark_options_wid,
             renderer_options_wid,
             info_wid,
             save_figure_wid,
         ]
     )
     tab_titles = ["Model", "Image", "Landmarks", "Renderer", "Info", "Export"]
-    for (k, tl) in enumerate(tab_titles):
+    for k, tl in enumerate(tab_titles):
         options_box.set_title(k, tl)
     logo_wid = LogoWidget(style=main_style)
     logo_wid.layout.margin = "0px 10px 0px 0px"
-    wid = ipywidgets.HBox([logo_wid, options_box])
+    output.layout.align_self = "center"
+    wid = ipywidgets.HBox([logo_wid, options_box, output])
 
     # Set widget's style
     wid.box_style = main_style
     wid.layout.border = "2px solid " + map_styles_to_hex_colours(main_style)
 
     # Display final widget
     final_box = ipywidgets.Box([wid])
@@ -1252,19 +1255,20 @@
             shape_options_wid,
             renderer_options_wid,
             info_wid,
             save_figure_wid,
         ]
     )
     tab_titles = ["Model", "Patches", "Image", "Shape", "Renderer", "Info", "Export"]
-    for (k, tl) in enumerate(tab_titles):
+    for k, tl in enumerate(tab_titles):
         options_box.set_title(k, tl)
     logo_wid = LogoWidget(style=main_style)
     logo_wid.layout.margin = "0px 10px 0px 0px"
-    wid = ipywidgets.HBox([logo_wid, options_box])
+    output.layout.align_self = "center"
+    wid = ipywidgets.HBox([logo_wid, options_box, output])
 
     # Set widget's style
     wid.box_style = main_style
     wid.layout.border = "2px solid " + map_styles_to_hex_colours(main_style)
 
     # Display final widget
     final_box = ipywidgets.Box([wid])
@@ -1532,19 +1536,20 @@
             shape_options_wid,
             renderer_options_wid,
             info_wid,
             save_figure_wid,
         ]
     )
     tab_titles = ["Model", "Experts", "Image", "Shape", "Renderer", "Info", "Export"]
-    for (k, tl) in enumerate(tab_titles):
+    for k, tl in enumerate(tab_titles):
         options_box.set_title(k, tl)
     logo_wid = LogoWidget(style=main_style)
     logo_wid.layout.margin = "0px 10px 0px 0px"
-    wid = ipywidgets.HBox([logo_wid, options_box])
+    output.layout.align_self = "center"
+    wid = ipywidgets.HBox([logo_wid, options_box, output])
 
     # Set widget's style
     wid.box_style = main_style
     wid.layout.border = "2px solid " + map_styles_to_hex_colours(main_style)
 
     # Display final widget
     final_box = ipywidgets.Box([wid])
@@ -1736,19 +1741,20 @@
             shape_options_wid,
             renderer_options_wid,
             info_wid,
             save_figure_wid,
         ]
     )
     tab_titles = ["Experts", "Image", "Shape", "Renderer", "Info", "Export"]
-    for (k, tl) in enumerate(tab_titles):
+    for k, tl in enumerate(tab_titles):
         options_box.set_title(k, tl)
     logo_wid = LogoWidget(style=main_style)
     logo_wid.layout.margin = "0px 10px 0px 0px"
-    wid = ipywidgets.HBox([logo_wid, options_box])
+    output.layout.align_self = "center"
+    wid = ipywidgets.HBox([logo_wid, options_box, output])
 
     # Set widget's style
     wid.box_style = main_style
     wid.layout.border = "2px solid " + map_styles_to_hex_colours(main_style)
 
     # Display final widget
     final_box = ipywidgets.Box([wid])
@@ -1903,15 +1909,16 @@
     plot_wid.tab_box.set_title(2, "Legend")
     plot_wid.tab_box.set_title(3, "Axes")
     plot_wid.tab_box.set_title(4, "Zoom")
     plot_wid.tab_box.set_title(5, "Grid")
     plot_wid.tab_box.set_title(6, "Export")
 
     # Display final widget
-    wid = ipywidgets.HBox([logo, plot_wid])
+    output.layout.align_self = "center"
+    wid = ipywidgets.HBox([logo, plot_wid, output])
     wid.box_style = main_style
     wid.layout.border = "2px solid " + map_styles_to_hex_colours(main_style)
     plot_wid.container.border = "0px"
     final_box = ipywidgets.Box([wid])
     final_box.layout.display = "flex"
     ipydisplay.display(final_box)
 
@@ -2346,20 +2353,22 @@
         header_wid = LogoWidget(style=main_style)
         header_wid.layout.margin = "0px 10px 0px 0px"
     # Widget titles
     tab_titles = ["Result", "Info", "Renderer", "Export"]
     options_box = ipywidgets.Tab(
         [fitting_result_wid, info_error_box, renderer_options_wid, save_figure_wid]
     )
-    for (k, tl) in enumerate(tab_titles):
+    for k, tl in enumerate(tab_titles):
         options_box.set_title(k, tl)
+
+    output.layout.align_self = "center"
     if n_fitting_results > 1:
-        wid = ipywidgets.VBox([header_wid, options_box])
+        wid = ipywidgets.VBox([header_wid, options_box, output])
     else:
-        wid = ipywidgets.HBox([header_wid, options_box])
+        wid = ipywidgets.HBox([header_wid, options_box, output])
     if n_fitting_results > 1:
         # If animation is activated and the user selects the save figure tab,
         # then the animation stops.
         def save_fig_tab_fun(change):
             if change["new"] == 3:
                 image_number_wid.pause_animation()
```

### Comparing `menpowidgets-0.4.1/menpowidgets/options.py` & `menpowidgets-0.4.2/menpowidgets/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,20 @@
     ColourSelectionWidget,
     TriMeshOptionsWidget,
     TexturedTriMeshOptionsWidget,
     SwitchWidget,
     MultipleSelectionTogglesWidget,
 )
 from .style import map_styles_to_hex_colours
-from .utils import sample_colours_from_colourmap, lists_are_the_same
+from .utils import (
+    do_one_iteration,
+    sample_colours_from_colourmap,
+    lists_are_the_same,
+    sync_asyncio_sleep,
+)
 
 
 class AnimationOptionsWidget(MenpoWidget):
     r"""
     Creates a widget for animating through a list of objects.
 
     Note that:
@@ -245,58 +250,48 @@
         )
 
         def loop_pressed(change):
             if change["new"]:
                 self.loop_toggle.icon = "repeat"
             else:
                 self.loop_toggle.icon = "long-arrow-right"
-            self.kernel.do_one_iteration()
+            do_one_iteration(self.kernel)
 
         self.loop_toggle.observe(loop_pressed, names="value", type="change")
 
         def fast_forward_pressed(name):
             tmp = self.interval
             tmp -= self.interval_step
             if tmp < 0:
                 tmp = 0
             self.interval = tmp
-            self.kernel.do_one_iteration()
+            do_one_iteration(self.kernel)
 
         self.fast_forward_button.on_click(fast_forward_pressed)
 
         def fast_backward_pressed(name):
             self.interval += self.interval_step
-            self.kernel.do_one_iteration()
+            do_one_iteration(self.kernel)
 
         self.fast_backward_button.on_click(fast_backward_pressed)
 
         def animate(change):
             # Get current index value
             i = self.selected_values
             # Disable the index widget
             self.index_wid_disability(True)
             # Reset stop/pause flags
             self.please_pause = False
             self.please_stop = False
             # Main loop
             while i <= self.max:
-                # Run IPython iteration.
-                # This is the code that makes this operation non-blocking.
-                # This allows widget messages and callbacks to be processed.
-                self.kernel.do_one_iteration()
-
                 # Check pause/stop flags
                 if self.please_pause or self.please_stop:
                     break
 
-                # Run IPython iteration.
-                # This is the code that makes this operation non-blocking.
-                # This allows widget messages and callbacks to be processed.
-                self.kernel.do_one_iteration()
-
                 # Update index value
                 if index_style == "slider":
                     self.index_wid.slider.value = i
                 else:
                     self.index_wid.set_widget_state(
                         {
                             "min": self.min,
@@ -305,27 +300,26 @@
                             "index": i,
                         },
                         loop_enabled=self.loop_enabled,
                         text_editable=False,
                         allow_callback=True,
                     )
 
-                # Run IPython iteration.
-                # This is the code that makes this operation non-blocking.
-                # This allows widget messages and callbacks to be processed.
-                self.kernel.do_one_iteration()
-
                 # Update counter
                 if self.loop_toggle.value and i >= self.max:
                     i = self.min
                 else:
                     i += self.step
 
                 # Wait
-                sleep(self.interval)
+                sync_asyncio_sleep(self.interval)
+                # Run IPython iteration.
+                # This is the code that makes this operation non-blocking.
+                # This allows widget messages and callbacks to be processed.
+                do_one_iteration(self.kernel)
 
             # If stop was pressed, then reset
             if self.please_stop:
                 if index_style == "slider":
                     self.index_wid.slider.value = 0
                 else:
                     self.index_wid.set_widget_state(
@@ -1869,15 +1863,15 @@
                     )
                 )
                 self.tab_titles.append("Grid")
         self.suboptions_tab = ipywidgets.Tab(children=self.options_widgets)
         self.suboptions_tab.layout.flex = "1"  # flex-grow
 
         # set titles
-        for (k, tl) in enumerate(self.tab_titles):
+        for k, tl in enumerate(self.tab_titles):
             self.suboptions_tab.set_title(k, tl)
 
         # Create final widget
         initial_options = renderer_options.copy()
         initial_options.update(self.global_options)
         self.container = ipywidgets.HBox([self.suboptions_tab])
         self.container.layout.flex = "1"  # flex-grow
@@ -1900,25 +1894,25 @@
         self.selected_values = {
             o: self.options_widgets[i].selected_values
             for i, o in enumerate(self.options_tabs)
         }
         # update default values
         current_key = self.get_key(self.labels)
         if "lines_matplotlib" in self.options_tabs:
-            self.default_options[current_key][
-                "lines_matplotlib"
-            ] = self.selected_values["lines_matplotlib"].copy()
+            self.default_options[current_key]["lines_matplotlib"] = (
+                self.selected_values["lines_matplotlib"].copy()
+            )
         if "lines_mayavi" in self.options_tabs:
             self.default_options[current_key]["lines_mayavi"] = self.selected_values[
                 "lines_mayavi"
             ].copy()
         if "markers_matplotlib" in self.options_tabs:
-            self.default_options[current_key][
-                "markers_matplotlib"
-            ] = self.selected_values["markers_matplotlib"].copy()
+            self.default_options[current_key]["markers_matplotlib"] = (
+                self.selected_values["markers_matplotlib"].copy()
+            )
         if "markers_mayavi" in self.options_tabs:
             self.default_options[current_key]["markers_mayavi"] = self.selected_values[
                 "markers_mayavi"
             ].copy()
         # update global values
         if "image_matplotlib" in self.options_tabs:
             self.global_options["image_matplotlib"] = self.selected_values[
@@ -3518,15 +3512,15 @@
         self.box_9 = ipywidgets.VBox([self.facecolour_widget, self.edgecolour_widget])
         self.box_9.layout.align_items = "flex-end"
         self.box_9.layout.margin = "0px 10px 0px 0px"
         self.box_99 = ipywidgets.HBox([self.box_9, self.transparent_checkbox])
         self.box_99.layout.align_items = "center"
         self.box_10 = ipywidgets.Tab([self.box_7, self.box_88, self.box_99])
         tab_titles = ["Path", "Page setup", "Colour"]
-        for (k, tl) in enumerate(tab_titles):
+        for k, tl in enumerate(tab_titles):
             self.box_10.set_title(k, tl)
         self.box_11 = ipywidgets.VBox([self.box_10])
         self.box_12 = ipywidgets.HBox([self.save_button])
         self.box_12.layout.align_items = "center"
         self.container = ipywidgets.VBox([self.box_10, self.box_12])
         self.container.layout.align_items = "center"
 
@@ -3986,15 +3980,15 @@
         self.render_bbox_checkbox = SwitchWidget(
             selected_value=True,
             description="Render bounding boxes",
             switch_type="checkbox",
         )
         self.bboxes_line_width_title = ipywidgets.HTML(value="Line width")
         self.bboxes_line_width_text = ipywidgets.BoundedFloatText(
-            value=1, min=0.0, max=10 ** 6, layout=ipywidgets.Layout(width="2.2cm")
+            value=1, min=0.0, max=10**6, layout=ipywidgets.Layout(width="2.2cm")
         )
         self.bboxes_line_style_title = ipywidgets.HTML(value="Line style")
         line_style_dict = OrderedDict()
         line_style_dict["solid"] = "-"
         line_style_dict["dashed"] = "--"
         line_style_dict["dash-dot"] = "-."
         line_style_dict["dotted"] = ":"
@@ -5186,31 +5180,31 @@
 
         # Set functionality
         def loop_pressed(change):
             if change["new"]:
                 self.loop_toggle.icon = "repeat"
             else:
                 self.loop_toggle.icon = "long-arrow-right"
-            self.kernel.do_one_iteration()
+            do_one_iteration(self.kernel)
 
         self.loop_toggle.observe(loop_pressed, names="value", type="change")
 
         def fast_forward_pressed(name):
             tmp = self.interval
             tmp -= self.interval_step
             if tmp < 0:
                 tmp = 0
             self.interval = tmp
-            self.kernel.do_one_iteration()
+            do_one_iteration(self.kernel)
 
         self.fast_forward_button.on_click(fast_forward_pressed)
 
         def fast_backward_pressed(name):
             self.interval += self.interval_step
-            self.kernel.do_one_iteration()
+            do_one_iteration(self.kernel)
 
         self.fast_backward_button.on_click(fast_backward_pressed)
 
         def animate(change):
             reset_parameters("")
             self.please_stop = False
             self.reset_button.disabled = True
@@ -5219,75 +5213,75 @@
                 n_sliders = self.n_parameters
                 slider_id = 0
                 while slider_id < n_sliders:
                     # animate from 0 to min
                     slider_val = 0.0
                     while slider_val > self.params_bounds[0]:
                         # Run IPython iteration.
-                        self.kernel.do_one_iteration()
+                        do_one_iteration(self.kernel)
 
                         # Check stop flag
                         if self.please_stop:
                             break
 
                         # update slider value
                         slider_val -= self.animation_step
 
                         # set value
                         self.sliders[slider_id].value = slider_val
 
                         # wait
-                        sleep(self.interval)
+                        sync_asyncio_sleep(self.interval)
 
                         # Run IPython iteration.
-                        self.kernel.do_one_iteration()
+                        do_one_iteration(self.kernel)
 
                     # animate from min to max
                     slider_val = self.params_bounds[0]
                     while slider_val < self.params_bounds[1]:
                         # Run IPython iteration.
-                        self.kernel.do_one_iteration()
+                        do_one_iteration(self.kernel)
 
                         # Check stop flag
                         if self.please_stop:
                             break
 
                         # update slider value
                         slider_val += self.animation_step
 
                         # set value
                         self.sliders[slider_id].value = slider_val
 
                         # wait
-                        sleep(self.interval)
+                        sync_asyncio_sleep(self.interval)
 
                         # Run IPython iteration.
-                        self.kernel.do_one_iteration()
+                        do_one_iteration(self.kernel)
 
                     # animate from max to 0
                     slider_val = self.params_bounds[1]
                     while slider_val > 0.0:
                         # Run IPython iteration.
-                        self.kernel.do_one_iteration()
+                        do_one_iteration(self.kernel)
 
                         # Check stop flag
                         if self.please_stop:
                             break
 
                         # update slider value
                         slider_val -= self.animation_step
 
                         # set value
                         self.sliders[slider_id].value = slider_val
 
                         # wait
-                        sleep(self.interval)
+                        sync_asyncio_sleep(self.interval)
 
                         # Run IPython iteration.
-                        self.kernel.do_one_iteration()
+                        do_one_iteration(self.kernel)
 
                     # reset value
                     self.sliders[slider_id].value = 0.0
 
                     # Check stop flag
                     if self.please_stop:
                         break
@@ -5308,75 +5302,75 @@
                     # set dropdown value
                     self.parameters_wid.children[0].value = slider_id
 
                     # animate from 0 to min
                     slider_val = 0.0
                     while slider_val > self.params_bounds[0]:
                         # Run IPython iteration.
-                        self.kernel.do_one_iteration()
+                        do_one_iteration(self.kernel)
 
                         # Check stop flag
                         if self.please_stop:
                             break
 
                         # update slider value
                         slider_val -= self.animation_step
 
                         # set value
                         self.parameters_wid.children[1].value = slider_val
 
                         # wait
-                        sleep(self.interval)
+                        sync_asyncio_sleep(self.interval)
 
                         # Run IPython iteration.
-                        self.kernel.do_one_iteration()
+                        do_one_iteration(self.kernel)
 
                     # animate from min to max
                     slider_val = self.params_bounds[0]
                     while slider_val < self.params_bounds[1]:
                         # Run IPython iteration.
-                        self.kernel.do_one_iteration()
+                        do_one_iteration(self.kernel)
 
                         # Check stop flag
                         if self.please_stop:
                             break
 
                         # update slider value
                         slider_val += self.animation_step
 
                         # set value
                         self.parameters_wid.children[1].value = slider_val
 
                         # wait
-                        sleep(self.interval)
+                        sync_asyncio_sleep(self.interval)
 
                         # Run IPython iteration.
-                        self.kernel.do_one_iteration()
+                        do_one_iteration(self.kernel)
 
                     # animate from max to 0
                     slider_val = self.params_bounds[1]
                     while slider_val > 0.0:
                         # Run IPython iteration.
-                        self.kernel.do_one_iteration()
+                        do_one_iteration(self.kernel)
 
                         # Check stop flag
                         if self.please_stop:
                             break
 
                         # update slider value
                         slider_val -= self.animation_step
 
                         # set value
                         self.parameters_wid.children[1].value = slider_val
 
                         # wait
-                        sleep(self.interval)
+                        sync_asyncio_sleep(self.interval)
 
                         # Run IPython iteration.
-                        self.kernel.do_one_iteration()
+                        do_one_iteration(self.kernel)
 
                     # reset value
                     self.parameters_wid.children[1].value = 0.0
 
                     # Check stop flag
                     if self.please_stop:
                         break
@@ -5693,14 +5687,15 @@
         >>>                            preview_windows_margin=1, style='info')
         >>> wid
 
     By pressing the "Take snapshot" button, the snapshots appear in the
     thumbnails below the stream. The video stream can be interrupted by pressing
     the "Close" button.
     """
+
     javascript_exported = False
 
     def __init__(
         self,
         canvas_width=640,
         hd=True,
         n_preview_windows=5,
```

### Comparing `menpowidgets-0.4.1/menpowidgets/style.py` & `menpowidgets-0.4.2/menpowidgets/style.py`

 * *Files identical despite different names*

### Comparing `menpowidgets-0.4.1/menpowidgets/tools.py` & `menpowidgets-0.4.2/menpowidgets/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -2127,15 +2127,15 @@
             switch_type=render_checkbox_type,
         )
         self.render_lines_switch.layout.margin = "7px"
         self.line_width_title = ipywidgets.HTML(value="Width")
         self.line_width_text = ipywidgets.BoundedFloatText(
             value=line_options["line_width"],
             min=0.0,
-            max=10 ** 6,
+            max=10**6,
             layout=ipywidgets.Layout(width="3cm"),
         )
         self.line_style_title = ipywidgets.HTML(value="Style")
         line_style_dict = OrderedDict()
         line_style_dict["solid"] = "-"
         line_style_dict["dashed"] = "--"
         line_style_dict["dash-dot"] = "-."
@@ -2292,15 +2292,15 @@
             switch_type=render_checkbox_type,
         )
         self.render_lines_switch.layout.margin = "7px"
         self.line_width_title = ipywidgets.HTML(value="Width")
         self.line_width_text = ipywidgets.BoundedFloatText(
             value=line_options["line_width"],
             min=0.0,
-            max=10 ** 6,
+            max=10**6,
             layout=ipywidgets.Layout(width="3cm"),
         )
         self.line_colour_widget = ColourSelectionWidget(
             line_options["line_colour"],
             description="Colour",
             labels=labels,
             render_function=None,
@@ -2445,22 +2445,22 @@
             switch_type=render_checkbox_type,
         )
         self.render_markers_switch.layout.margin = "7px"
         self.marker_size_title = ipywidgets.HTML(value="Size")
         self.marker_size_text = ipywidgets.BoundedIntText(
             value=marker_options["marker_size"],
             min=0,
-            max=10 ** 6,
+            max=10**6,
             layout=ipywidgets.Layout(width="3cm"),
         )
         self.marker_edge_width_title = ipywidgets.HTML(value="Edge width")
         self.marker_edge_width_text = ipywidgets.BoundedFloatText(
             value=marker_options["marker_edge_width"],
             min=0.0,
-            max=10 ** 6,
+            max=10**6,
             layout=ipywidgets.Layout(width="3cm"),
         )
         self.marker_style_title = ipywidgets.HTML(value="Style")
         marker_style_dict = OrderedDict()
         marker_style_dict["point"] = "."
         marker_style_dict["pixel"] = ","
         marker_style_dict["circle"] = "o"
@@ -2680,27 +2680,27 @@
             m1 = 0.1
             m2 = True
             m_icon = "fa-times"
         self.marker_size_text = ipywidgets.BoundedFloatText(
             value=m1,
             disabled=m2,
             min=0,
-            max=10 ** 6,
+            max=10**6,
             layout=ipywidgets.Layout(width="1.9cm"),
         )
         self.marker_size_none = ipywidgets.Button(
             description="",
             icon=m_icon,
             layout=ipywidgets.Layout(width="1.0cm", height="0.8cm"),
         )
         self.marker_resolution_title = ipywidgets.HTML(value="Resolution")
         self.marker_resolution_text = ipywidgets.BoundedIntText(
             value=marker_options["marker_resolution"],
             min=0.0,
-            max=10 ** 6,
+            max=10**6,
             layout=ipywidgets.Layout(width="3cm"),
         )
         self.marker_style_title = ipywidgets.HTML(value="Style")
         marker_style_dict = OrderedDict()
         marker_style_dict["Sphere"] = "sphere"
         marker_style_dict["Cube"] = "cube"
         marker_style_dict["Cone"] = "cone"
@@ -2724,15 +2724,15 @@
             value=marker_options["marker_style"],
             layout=ipywidgets.Layout(width="3cm"),
         )
         self.step_title = ipywidgets.HTML(value="Sampling")
         self.step_text = ipywidgets.BoundedIntText(
             value=marker_options["step"],
             min=0.0,
-            max=10 ** 6,
+            max=10**6,
             layout=ipywidgets.Layout(width="2.6cm"),
         )
         self.marker_colour_widget = ColourSelectionWidget(
             marker_options["marker_colour"],
             description="Colour",
             labels=labels,
             render_function=None,
@@ -2929,15 +2929,15 @@
             options=numbers_font_name_dict,
             value=numbers_options["numbers_font_name"],
             layout=ipywidgets.Layout(width="3cm"),
         )
         self.numbers_font_size_title = ipywidgets.HTML(value="Size")
         self.numbers_font_size_text = ipywidgets.BoundedIntText(
             min=0,
-            max=10 ** 6,
+            max=10**6,
             value=numbers_options["numbers_font_size"],
             layout=ipywidgets.Layout(width="3cm"),
         )
         self.numbers_font_style_title = ipywidgets.HTML(value="Style")
         numbers_font_style_dict = OrderedDict()
         numbers_font_style_dict["normal"] = "normal"
         numbers_font_style_dict["italic"] = "italic"
@@ -3198,15 +3198,15 @@
             n1 = 0.1
             n2 = True
             n_icon = "fa-times"
         self.numbers_size_text = ipywidgets.BoundedFloatText(
             value=n1,
             disabled=n2,
             min=0.0,
-            max=10 ** 6,
+            max=10**6,
             layout=ipywidgets.Layout(width="1.9cm"),
         )
         self.numbers_size_none = ipywidgets.Button(
             description="",
             icon=n_icon,
             layout=ipywidgets.Layout(width="1.0cm", height="0.8cm"),
         )
@@ -3798,15 +3798,15 @@
             value=axes_options["axes_font_name"],
             layout=ipywidgets.Layout(width="3cm"),
         )
         self.axes_font_size_title = ipywidgets.HTML(value="Font Size")
         self.axes_font_size_text = ipywidgets.BoundedIntText(
             value=axes_options["axes_font_size"],
             min=0,
-            max=10 ** 6,
+            max=10**6,
             layout=ipywidgets.Layout(width="3cm"),
         )
         self.axes_font_style_title = ipywidgets.HTML(value="Font Style")
         axes_font_style_dict = OrderedDict()
         axes_font_style_dict["normal"] = "normal"
         axes_font_style_dict["italic"] = "italic"
         axes_font_style_dict["oblique"] = "oblique"
@@ -4060,15 +4060,15 @@
             options=legend_font_name_dict,
             layout=ipywidgets.Layout(width="3cm"),
             value=legend_options["legend_font_name"],
         )
         self.legend_font_size_title = ipywidgets.HTML(value="Size")
         self.legend_font_size_text = ipywidgets.BoundedIntText(
             min=0,
-            max=10 ** 6,
+            max=10**6,
             value=legend_options["legend_font_size"],
             layout=ipywidgets.Layout(width="3cm"),
         )
         self.legend_font_style_title = ipywidgets.HTML(value="Style")
         legend_font_style_dict = OrderedDict()
         legend_font_style_dict["normal"] = "normal"
         legend_font_style_dict["italic"] = "italic"
@@ -4570,15 +4570,15 @@
             switch_type=render_checkbox_type,
         )
         self.render_grid_switch.layout.margin = "7px"
         self.grid_line_width_title = ipywidgets.HTML(value="Width")
         self.grid_line_width_text = ipywidgets.BoundedFloatText(
             value=grid_options["grid_line_width"],
             min=0.0,
-            max=10 ** 6,
+            max=10**6,
             layout=ipywidgets.Layout(width="3cm"),
         )
         self.grid_line_style_title = ipywidgets.HTML(value="Style")
         grid_line_style_dict = OrderedDict()
         grid_line_style_dict["solid"] = "-"
         grid_line_style_dict["dashed"] = "--"
         grid_line_style_dict["dash-dot"] = "-."
@@ -4682,14 +4682,15 @@
         The initial width of the rendered canvas. Note that this doesn't
         actually change the webcam resolution. It simply rescales the
         rendered image, as well as the size of the returned screenshots.
     hd : `bool`, optional
         If ``True``, then the webcam will be set to high definition (HD), i.e.
         720 x 1280. Otherwise the default resolution will be used.
     """
+
     _view_name = Unicode("CameraView").tag(sync=True)
     _view_module = Unicode("camera").tag(sync=True)
     imageurl = Unicode("").tag(sync=True)
     take_snapshot = Bool(False).tag(sync=True)
     canvas_width = Int(640).tag(sync=True)
     canvas_height = Int().tag(sync=True)
     hd = Bool(True).tag(sync=True)
@@ -4755,15 +4756,15 @@
             value=mesh_options["mesh_type"],
             layout=ipywidgets.Layout(width="3cm"),
         )
         self.line_width_title = ipywidgets.HTML(value="Line width")
         self.line_width_text = ipywidgets.BoundedFloatText(
             value=float(mesh_options["line_width"]),
             min=0.0,
-            max=10 ** 6,
+            max=10**6,
             layout=ipywidgets.Layout(width="1.1cm"),
         )
         self.colour_widget = ColourSelectionWidget(
             mesh_options["colour"], description="Colour", render_function=None
         )
         self.alpha_title = ipywidgets.HTML(value="Alpha")
         self.alpha_slider = ipywidgets.FloatSlider(
@@ -4811,34 +4812,34 @@
             m1 = 0.1
             m2 = True
             m_icon = "fa-times"
         self.marker_size_text = ipywidgets.BoundedFloatText(
             value=m1,
             disabled=m2,
             min=0.0,
-            max=10 ** 6,
+            max=10**6,
             layout=ipywidgets.Layout(width="1.9cm"),
         )
         self.marker_size_none = ipywidgets.Button(
             description="",
             icon=m_icon,
             layout=ipywidgets.Layout(width="1.0cm", height="0.8cm"),
         )
         self.marker_resolution_title = ipywidgets.HTML(value="Resolution")
         self.marker_resolution_text = ipywidgets.BoundedIntText(
             value=mesh_options["marker_resolution"],
             min=0,
-            max=10 ** 6,
+            max=10**6,
             layout=ipywidgets.Layout(width="3cm"),
         )
         self.step_title = ipywidgets.HTML(value="Step")
         self.step_text = ipywidgets.BoundedIntText(
             value=mesh_options["step"],
             min=1,
-            max=10 ** 6,
+            max=10**6,
             layout=ipywidgets.Layout(width="3cm"),
         )
 
         # Group widgets
         self.box_1 = ipywidgets.HBox([self.mesh_type_title, self.mesh_type_toggles])
         self.box_1.layout.align_items = "center"
         self.box_1.layout.margin = "9px"
@@ -5058,15 +5059,15 @@
             layout=ipywidgets.Layout(width="3cm"),
         )
         self.mesh_type_toggles.layout.margin = "0px 15px 0px 0px"
         self.line_width_title = ipywidgets.HTML(value="Line width")
         self.line_width_text = ipywidgets.BoundedFloatText(
             value=float(mesh_options["line_width"]),
             min=0.0,
-            max=10 ** 6,
+            max=10**6,
             layout=ipywidgets.Layout(width="1.2cm"),
         )
         self.ambient_title = ipywidgets.HTML(value="Ambient")
         self.ambient_slider = ipywidgets.FloatSlider(
             value=mesh_options["ambient_light"],
             min=0.0,
             max=1.0,
```

### Comparing `menpowidgets-0.4.1/menpowidgets/utils.py` & `menpowidgets-0.4.2/menpowidgets/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,33 @@
+import asyncio
 from struct import pack as struct_pack
 import binascii
+
+import nest_asyncio
 import numpy as np
 
 
+def do_one_iteration(kernel):
+    nest_asyncio.apply()
+
+    loop = asyncio.get_running_loop()
+
+    task = loop.create_task(kernel.do_one_iteration())
+    loop.run_until_complete(task)
+
+
+def sync_asyncio_sleep(interval):
+    nest_asyncio.apply()
+
+    loop = asyncio.get_running_loop()
+
+    task = loop.create_task(asyncio.sleep(interval))
+    loop.run_until_complete(task)
+
+
 def lists_are_the_same(a, b):
     r"""
     Function that checks if two `lists` have the same elements in the same
     order.
 
     Returns
     -------
```

### Comparing `menpowidgets-0.4.1/menpowidgets.egg-info/SOURCES.txt` & `menpowidgets-0.4.2/menpowidgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `menpowidgets-0.4.1/setup.py` & `menpowidgets-0.4.2/setup.py`

 * *Files identical despite different names*

