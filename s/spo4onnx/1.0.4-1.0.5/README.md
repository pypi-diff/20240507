# Comparing `tmp/spo4onnx-1.0.4.tar.gz` & `tmp/spo4onnx-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spo4onnx-1.0.4.tar", last modified: Mon Apr 22 10:40:16 2024, max compression
+gzip compressed data, was "spo4onnx-1.0.5.tar", last modified: Tue May  7 06:26:21 2024, max compression
```

## Comparing `spo4onnx-1.0.4.tar` & `spo4onnx-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:40:16.325687 spo4onnx-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-22 10:40:10.000000 spo4onnx-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-04-22 10:40:16.321687 spo4onnx-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-04-22 10:40:10.000000 spo4onnx-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 10:40:16.325687 spo4onnx-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-22 10:40:10.000000 spo4onnx-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:40:16.321687 spo4onnx-1.0.4/spo4onnx/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-22 10:40:10.000000 spo4onnx-1.0.4/spo4onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-22 10:40:10.000000 spo4onnx-1.0.4/spo4onnx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23814 2024-04-22 10:40:10.000000 spo4onnx-1.0.4/spo4onnx/onnx_partial_optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:40:16.321687 spo4onnx-1.0.4/spo4onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-04-22 10:40:16.000000 spo4onnx-1.0.4/spo4onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-22 10:40:16.000000 spo4onnx-1.0.4/spo4onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 10:40:16.000000 spo4onnx-1.0.4/spo4onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-22 10:40:16.000000 spo4onnx-1.0.4/spo4onnx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-22 10:40:16.000000 spo4onnx-1.0.4/spo4onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:26:21.718257 spo4onnx-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-07 06:26:14.000000 spo4onnx-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-05-07 06:26:21.718257 spo4onnx-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-05-07 06:26:14.000000 spo4onnx-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 06:26:21.718257 spo4onnx-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-07 06:26:14.000000 spo4onnx-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:26:21.718257 spo4onnx-1.0.5/spo4onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-07 06:26:14.000000 spo4onnx-1.0.5/spo4onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-07 06:26:14.000000 spo4onnx-1.0.5/spo4onnx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24430 2024-05-07 06:26:14.000000 spo4onnx-1.0.5/spo4onnx/onnx_partial_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:26:21.718257 spo4onnx-1.0.5/spo4onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-05-07 06:26:21.000000 spo4onnx-1.0.5/spo4onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-07 06:26:21.000000 spo4onnx-1.0.5/spo4onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 06:26:21.000000 spo4onnx-1.0.5/spo4onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 06:26:21.000000 spo4onnx-1.0.5/spo4onnx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 06:26:21.000000 spo4onnx-1.0.5/spo4onnx.egg-info/top_level.txt
```

### Comparing `spo4onnx-1.0.4/LICENSE` & `spo4onnx-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spo4onnx-1.0.4/PKG-INFO` & `spo4onnx-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spo4onnx
-Version: 1.0.4
+Version: 1.0.5
 Summary: Simple tool for partial optimization of ONNX. Further optimize some models that cannot be optimized with onnx-optimizer and onnxsim by several tens of percent. In particular, models containing Einsum and OneHot.
 Home-page: https://github.com/PINTO0309/spo4onnx
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
```

### Comparing `spo4onnx-1.0.4/README.md` & `spo4onnx-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `spo4onnx-1.0.4/setup.py` & `spo4onnx-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `spo4onnx-1.0.4/spo4onnx/onnx_partial_optimization.py` & `spo4onnx-1.0.5/spo4onnx/onnx_partial_optimization.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,14 +123,17 @@
 
     Returns
     ----------
     outputs: List[np.ndarray]
         Results of inference using dummy tensor
     """
     # Separate onnx at specified output_names position
+    metadata_props = None
+    if hasattr(onnx_graph, 'metadata_props'):
+        metadata_props = onnx_graph.metadata_props
     gs_graph = gs.import_onnx(onnx_graph)
 
     # reduce all axes except batch axis
     for i, node in enumerate(gs_graph.nodes):
         if gs_graph.opset <= 17 \
             and gs_graph.nodes[i].op in ['ReduceMax', 'ReduceMean', 'ReduceMin', 'ReduceProd'] \
             and 'axes' not in node.attrs:
@@ -176,14 +179,16 @@
     for graph_node in gs_graph.nodes:
         for node_output in graph_node.outputs:
             if node_output.name in output_names:
                 if node_output.dtype is not None:
                     gs_graph.outputs.append(node_output)
 
     new_onnx_graph = gs.export_onnx(graph=gs_graph, do_type_check=False, **kwargs)
+    if metadata_props is not None:
+        new_onnx_graph.metadata_props.extend(metadata_props)
     tmp_onnx_path = ''
     tmp_onnx_external_weights_path =''
     try:
         serializer: ProtoSerializer = onnx._get_serializer(fmt='protobuf')
         serialized_graph = serializer.serialize_proto(proto=new_onnx_graph)
     except ValueError as ve:
         tmp_onnx_path = 'tmp.onnx'
@@ -368,14 +373,18 @@
     # onnx_graph If specified, onnx_graph is processed first
     if not onnx_graph:
         onnx_graph = onnx.load(input_onnx_file_path)
 
     # domain, ir_version
     domain: str = onnx_graph.domain
     ir_version: int = onnx_graph.ir_version
+    meta_data = {'domain': domain, 'ir_version': ir_version}
+    metadata_props = None
+    if hasattr(onnx_graph, 'metadata_props'):
+        metadata_props = onnx_graph.metadata_props
 
     # import
     gs_graph = gs.import_onnx(onnx_graph)
 
     # optimization_times
     if optimization_times == 0:
         optimization_times = math.ceil(len(gs_graph.nodes) / 1000)
@@ -400,15 +409,18 @@
     try:
         output_clear = False
         for graph_output in gs_graph.outputs:
             if graph_output.shape is not None \
                 and sum([1 if isinstance(s, int) and s < 1 else 0 for s in graph_output.shape]) > 0:
                 graph_output.shape = None
                 output_clear = True
-        onnx_graph_opt = onnx.shape_inference.infer_shapes(gs.export_onnx(gs_graph, do_type_check=False, **{'domain': domain, 'ir_version': ir_version}))
+        exported_onnx_graph = gs.export_onnx(gs_graph, do_type_check=False, **meta_data)
+        if metadata_props is not None:
+            exported_onnx_graph.metadata_props.extend(metadata_props)
+        onnx_graph_opt = onnx.shape_inference.infer_shapes(exported_onnx_graph)
         gs_graph = gs.import_onnx(onnx_graph_opt)
         if input_onnx_file_path and output_clear:
             onnx.save(onnx_graph_opt, f=input_onnx_file_path)
     except Exception as ex:
         onnx_graph_opt = onnx_graph
 
     # Force installation of onnxsim==0.4.30
@@ -509,15 +521,17 @@
                 ]
                 for target_op in target_ops:
                     correction_op_output: gs.Variable = target_op.outputs[0]
                     if correction_op_output.name in onnx_tensor_infos_for_validation:
                         onnx_output_shape = list(onnx_tensor_infos_for_validation[correction_op_output.name].shape)
                         correction_op_output.shape = onnx_output_shape
                 try:
-                    model_simp = gs.export_onnx(gs_graph, do_type_check=False, **{'domain': domain, 'ir_version': ir_version})
+                    model_simp = gs.export_onnx(gs_graph, do_type_check=False, **meta_data)
+                    if metadata_props is not None:
+                        model_simp.metadata_props.extend(metadata_props)
                     model_simp, check = simplify(
                         model=model_simp,
                         overwrite_input_shapes=overwrite_input_shape,
                     )
                 except:
                     pass
                 onnx_graph_opt = model_simp
```

### Comparing `spo4onnx-1.0.4/spo4onnx.egg-info/PKG-INFO` & `spo4onnx-1.0.5/spo4onnx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spo4onnx
-Version: 1.0.4
+Version: 1.0.5
 Summary: Simple tool for partial optimization of ONNX. Further optimize some models that cannot be optimized with onnx-optimizer and onnxsim by several tens of percent. In particular, models containing Einsum and OneHot.
 Home-page: https://github.com/PINTO0309/spo4onnx
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
```

