# Comparing `tmp/volvisualizer-1.1.8-py3-none-any.whl.zip` & `tmp/volvisualizer-1.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 28795 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat       23 b- defN 24-Feb-02 15:36 volvisualizer/__init__.py
--rw-rw-rw-  2.0 fat    33445 b- defN 24-Feb-05 18:11 volvisualizer/graph.py
+Zip file size: 28809 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat       23 b- defN 24-Feb-12 09:01 volvisualizer/__init__.py
+-rw-rw-rw-  2.0 fat    33753 b- defN 24-Feb-12 10:05 volvisualizer/graph.py
 -rw-rw-rw-  2.0 fat    12153 b- defN 24-Jan-09 08:56 volvisualizer/market_data.py
 -rw-rw-rw-  2.0 fat    27280 b- defN 24-Jan-19 09:08 volvisualizer/market_data_prep.py
 -rw-rw-rw-  2.0 fat     2948 b- defN 23-Jun-29 14:24 volvisualizer/utils.py
 -rw-rw-rw-  2.0 fat    30755 b- defN 23-Jun-29 15:10 volvisualizer/vol_methods.py
 -rw-rw-rw-  2.0 fat    14500 b- defN 24-Feb-05 17:50 volvisualizer/volatility.py
 -rw-rw-rw-  2.0 fat     3964 b- defN 24-Feb-05 09:22 volvisualizer/volatility_params.py
--rw-rw-rw-  2.0 fat     1089 b- defN 24-Feb-05 18:15 volvisualizer-1.1.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      751 b- defN 24-Feb-05 18:15 volvisualizer-1.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Feb-05 18:15 volvisualizer-1.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 24-Feb-05 18:15 volvisualizer-1.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1093 b- defN 24-Feb-05 18:15 volvisualizer-1.1.8.dist-info/RECORD
-13 files, 128107 bytes uncompressed, 26969 bytes compressed:  78.9%
+-rw-rw-rw-  2.0 fat     1089 b- defN 24-Feb-12 10:25 volvisualizer-1.1.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      751 b- defN 24-Feb-12 10:25 volvisualizer-1.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Feb-12 10:25 volvisualizer-1.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 24-Feb-12 10:25 volvisualizer-1.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1093 b- defN 24-Feb-12 10:25 volvisualizer-1.1.9.dist-info/RECORD
+13 files, 128415 bytes uncompressed, 26983 bytes compressed:  79.0%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: volvisualizer/volatility.py
 Comment: 
 
 Filename: volvisualizer/volatility_params.py
 Comment: 
 
-Filename: volvisualizer-1.1.8.dist-info/LICENSE
+Filename: volvisualizer-1.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: volvisualizer-1.1.8.dist-info/METADATA
+Filename: volvisualizer-1.1.9.dist-info/METADATA
 Comment: 
 
-Filename: volvisualizer-1.1.8.dist-info/WHEEL
+Filename: volvisualizer-1.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: volvisualizer-1.1.8.dist-info/top_level.txt
+Filename: volvisualizer-1.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: volvisualizer-1.1.8.dist-info/RECORD
+Filename: volvisualizer-1.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## volvisualizer/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.1.8"
+__version__ = "1.1.9"
```

## volvisualizer/graph.py

```diff
@@ -397,14 +397,18 @@
         # Create figure and axis objects and format
         opt_dict = cls._create_opt_labels(
             params=params, 
             opt_dict=opt_dict, 
             output='mpl'
             )
         
+        opt_dict['strikes'] = np.array(params['x'])
+        opt_dict['ttms'] = np.array(params['y'])
+        opt_dict['vols'] = np.array(params['z'])
+
         if params['show_graph']:
             fig, ax = cls._graph_format(params=params, opt_dict=opt_dict)
 
             # Display triangular surface plot, using colormap 'viridis'
             ax.plot_trisurf(params['x'],
                             params['y'],
                             params['z'],
@@ -500,14 +504,17 @@
         # Create figure and axis objects and format
         opt_dict = cls._create_opt_labels(
             params=params, 
             opt_dict=opt_dict, 
             output='mpl'
             )    
 
+        opt_dict['strikes'] = np.array(params['x'])
+        opt_dict['ttms'] = np.array(params['y'])
+        opt_dict['vols'] = np.array(params['z'])
         opt_dict['strikes_linspace'] = x1
         opt_dict['ttms_linspace'] = y1
         opt_dict['strikes_linspace_array'] = x2
         opt_dict['ttms_linspace_array'] = y2
         opt_dict['vol_surface'] = z2
 
         # Plot the surface
```

## Comparing `volvisualizer-1.1.8.dist-info/LICENSE` & `volvisualizer-1.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `volvisualizer-1.1.8.dist-info/METADATA` & `volvisualizer-1.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volvisualizer
-Version: 1.1.8
+Version: 1.1.9
 Summary: Extract and visualize implied volatility from option data.
 Home-page: https://github.com/GBERESEARCH/volvisualizer
 Author: GBERESEARCH
 Author-email: gberesearch@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

## Comparing `volvisualizer-1.1.8.dist-info/RECORD` & `volvisualizer-1.1.9.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-volvisualizer/__init__.py,sha256=jro_fYFaWTpMLcXlRQe53nd8yxygCDFL1sK3eYFcmKI,23
-volvisualizer/graph.py,sha256=VEz7hD4c57tuo18xgdjTKNHxfCtHG2RcteIavcxiCiA,33445
+volvisualizer/__init__.py,sha256=hd2wYPvGunibyWXQ6TDOUOWCOzF6eAI2bFVEYi8US3E,23
+volvisualizer/graph.py,sha256=KU59TuC1FaC_IyU3HsmPmebzoa3Z3jjCC4yLM7ODaj0,33753
 volvisualizer/market_data.py,sha256=0XQrYQwgTT6vO9SeGcT9Mvh8STZ4pyFhS0-EtRuYOns,12153
 volvisualizer/market_data_prep.py,sha256=prcbLLZKLUAc05t19vVRD3qDoVoOP08K2ujxGvcOmwQ,27280
 volvisualizer/utils.py,sha256=beKuHS2pXOV9_sgqsVPrQUMVTDAjjmJc8DNbCmOU5sw,2948
 volvisualizer/vol_methods.py,sha256=2P1yTBHXAzumPcyoYuCLZxXJHOhMtO4_Z90RjduYRMA,30755
 volvisualizer/volatility.py,sha256=YYuxTayacw2L3B_QpLBTcJrtBnTqKUn0BTjr-8fOEi0,14500
 volvisualizer/volatility_params.py,sha256=e9-HFcPB5zOoOLZjK61fMYzGq3_FxmCqbeomPNtLJx4,3964
-volvisualizer-1.1.8.dist-info/LICENSE,sha256=AE-WWqzPtajuHJajyfzO6uPCKh1DW3MqA1NXcnBImL0,1089
-volvisualizer-1.1.8.dist-info/METADATA,sha256=sxIhLmtMWF0Q8A75cEtQGqunV9LI28S2lIe71yF8EI4,751
-volvisualizer-1.1.8.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-volvisualizer-1.1.8.dist-info/top_level.txt,sha256=Tfyh9PL2rX9P1DsThRUSnziSAZJU3o43o73eAOUHCMc,14
-volvisualizer-1.1.8.dist-info/RECORD,,
+volvisualizer-1.1.9.dist-info/LICENSE,sha256=AE-WWqzPtajuHJajyfzO6uPCKh1DW3MqA1NXcnBImL0,1089
+volvisualizer-1.1.9.dist-info/METADATA,sha256=00lPC03xq_Ksy7DS30cqGCK11ZILSvxL0nqy0Mizgdc,751
+volvisualizer-1.1.9.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+volvisualizer-1.1.9.dist-info/top_level.txt,sha256=Tfyh9PL2rX9P1DsThRUSnziSAZJU3o43o73eAOUHCMc,14
+volvisualizer-1.1.9.dist-info/RECORD,,
```

