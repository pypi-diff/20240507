# Comparing `tmp/sng4onnx-1.0.2.tar.gz` & `tmp/sng4onnx-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sng4onnx-1.0.2.tar", last modified: Mon Apr 22 12:53:16 2024, max compression
+gzip compressed data, was "sng4onnx-1.0.3.tar", last modified: Tue May  7 04:57:16 2024, max compression
```

## Comparing `sng4onnx-1.0.2.tar` & `sng4onnx-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:53:16.064669 sng4onnx-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-22 12:53:09.000000 sng4onnx-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-22 12:53:16.064669 sng4onnx-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-22 12:53:09.000000 sng4onnx-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 12:53:16.064669 sng4onnx-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-22 12:53:09.000000 sng4onnx-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:53:16.060669 sng4onnx-1.0.2/sng4onnx/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-22 12:53:09.000000 sng4onnx-1.0.2/sng4onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-22 12:53:09.000000 sng4onnx-1.0.2/sng4onnx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-04-22 12:53:09.000000 sng4onnx-1.0.2/sng4onnx/onnx_opname_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:53:16.064669 sng4onnx-1.0.2/sng4onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-22 12:53:16.000000 sng4onnx-1.0.2/sng4onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-22 12:53:16.000000 sng4onnx-1.0.2/sng4onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 12:53:16.000000 sng4onnx-1.0.2/sng4onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-22 12:53:16.000000 sng4onnx-1.0.2/sng4onnx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-22 12:53:16.000000 sng4onnx-1.0.2/sng4onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:57:16.994610 sng4onnx-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-07 04:57:11.000000 sng4onnx-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-05-07 04:57:16.994610 sng4onnx-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-07 04:57:11.000000 sng4onnx-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 04:57:16.994610 sng4onnx-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-07 04:57:11.000000 sng4onnx-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:57:16.990610 sng4onnx-1.0.3/sng4onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 04:57:11.000000 sng4onnx-1.0.3/sng4onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-07 04:57:11.000000 sng4onnx-1.0.3/sng4onnx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-05-07 04:57:11.000000 sng4onnx-1.0.3/sng4onnx/onnx_opname_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:57:16.994610 sng4onnx-1.0.3/sng4onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-05-07 04:57:16.000000 sng4onnx-1.0.3/sng4onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-07 04:57:16.000000 sng4onnx-1.0.3/sng4onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 04:57:16.000000 sng4onnx-1.0.3/sng4onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 04:57:16.000000 sng4onnx-1.0.3/sng4onnx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 04:57:16.000000 sng4onnx-1.0.3/sng4onnx.egg-info/top_level.txt
```

### Comparing `sng4onnx-1.0.2/LICENSE` & `sng4onnx-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sng4onnx-1.0.2/PKG-INFO` & `sng4onnx-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sng4onnx
-Version: 1.0.2
+Version: 1.0.3
 Summary: A simple tool that automatically generates and assigns an OP name to each OP in an old format ONNX file.
 Home-page: https://github.com/PINTO0309/sng4onnx
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
```

### Comparing `sng4onnx-1.0.2/README.md` & `sng4onnx-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `sng4onnx-1.0.2/setup.py` & `sng4onnx-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `sng4onnx-1.0.2/sng4onnx/onnx_opname_generator.py` & `sng4onnx-1.0.3/sng4onnx/onnx_opname_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,14 +75,20 @@
 
     # Loading Graphs
     # onnx_graph If specified, onnx_graph is processed first
     if not onnx_graph:
         onnx_graph = onnx.load(input_onnx_file_path)
     domain: str = onnx_graph.domain
     ir_version: int = onnx_graph.ir_version
+    meta_data = {'domain': domain, 'ir_version': ir_version}
+    if hasattr(onnx_graph, 'metadata_props'):
+        metadata_props = [metadata_prop for metadata_prop in onnx_graph.metadata_props]
+        if len(metadata_props) > 0:
+            metadata_props_dict = {metadata_prop.key: metadata_prop.value for metadata_prop in metadata_props}
+            meta_data = {**meta_data, **metadata_props_dict}
     graph = gs.import_onnx(onnx_graph)
     graph.cleanup().toposort()
 
     # opname auto supplementation
     # OPs in old ONNX files may be missing opname,
     # so opname is automatically completed when opname is empty.
     supplementation_idx = 0
@@ -92,15 +98,15 @@
             supplementation_idx += 1
 
     graph.cleanup().toposort()
 
     # Shape Estimation
     renamed_graph = None
     try:
-        renamed_graph = onnx.shape_inference.infer_shapes(gs.export_onnx(graph, do_type_check=False, **{'domain': domain, 'ir_version': ir_version}))
+        renamed_graph = onnx.shape_inference.infer_shapes(gs.export_onnx(graph, do_type_check=False, **meta_data))
     except:
         renamed_graph = gs.export_onnx(graph)
         if not non_verbose:
             print(
                 f'{Color.YELLOW}WARNING:{Color.RESET} '+
                 'The input shape of the next OP does not match the output shape. '+
                 'Be sure to open the .onnx file to verify the certainty of the geometry.'
```

### Comparing `sng4onnx-1.0.2/sng4onnx.egg-info/PKG-INFO` & `sng4onnx-1.0.3/sng4onnx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sng4onnx
-Version: 1.0.2
+Version: 1.0.3
 Summary: A simple tool that automatically generates and assigns an OP name to each OP in an old format ONNX file.
 Home-page: https://github.com/PINTO0309/sng4onnx
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
```

