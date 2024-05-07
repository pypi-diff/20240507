# Comparing `tmp/STAIR-tools-1.2.5.tar.gz` & `tmp/STAIR-tools-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "STAIR-tools-1.2.5.tar", last modified: Mon May  6 15:44:10 2024, max compression
+gzip compressed data, was "STAIR-tools-1.2.6.tar", last modified: Mon May  6 16:55:20 2024, max compression
```

## Comparing `STAIR-tools-1.2.5.tar` & `STAIR-tools-1.2.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-06 15:44:10.667342 STAIR-tools-1.2.5/
--rw-r--r--   0 yuanyuan   (501) staff       (20)      253 2024-05-06 15:44:10.667026 STAIR-tools-1.2.5/PKG-INFO
--rwxr-xr-x   0 yuanyuan   (501) staff       (20)     1320 2023-12-25 02:00:08.000000 STAIR-tools-1.2.5/README.md
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-06 15:44:10.662051 STAIR-tools-1.2.5/STAIR/
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8661 2023-12-23 11:23:09.000000 STAIR-tools-1.2.5/STAIR/ABA_annotation.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-06 15:44:10.662386 STAIR-tools-1.2.5/STAIR/ABAanno/
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.5/STAIR/ABAanno/__init__.py
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.5/STAIR/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    18514 2024-05-06 15:17:54.000000 STAIR-tools-1.2.5/STAIR/emb_alignment.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-06 15:44:10.664597 STAIR-tools-1.2.5/STAIR/embedding/
--rw-------   0 yuanyuan   (501) staff       (20)      120 2024-04-25 02:41:10.000000 STAIR-tools-1.2.5/STAIR/embedding/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3804 2024-05-04 11:27:47.000000 STAIR-tools-1.2.5/STAIR/embedding/dataset_ae.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     6022 2024-05-06 15:43:27.000000 STAIR-tools-1.2.5/STAIR/embedding/dataset_hgat.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)      988 2023-12-23 11:23:12.000000 STAIR-tools-1.2.5/STAIR/embedding/loss.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     5493 2023-12-23 11:23:12.000000 STAIR-tools-1.2.5/STAIR/embedding/module_ae.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8658 2023-12-23 11:23:12.000000 STAIR-tools-1.2.5/STAIR/embedding/module_hgat.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     6954 2023-12-23 11:23:12.000000 STAIR-tools-1.2.5/STAIR/embedding/module_hgat1.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    12320 2024-04-29 06:21:03.000000 STAIR-tools-1.2.5/STAIR/loc_alignment.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    14364 2024-04-28 11:59:13.000000 STAIR-tools-1.2.5/STAIR/loc_prediction.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-06 15:44:10.666191 STAIR-tools-1.2.5/STAIR/location/
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.5/STAIR/location/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     7819 2023-12-23 11:23:12.000000 STAIR-tools-1.2.5/STAIR/location/align_fine.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    11236 2023-12-23 11:23:13.000000 STAIR-tools-1.2.5/STAIR/location/align_init.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8534 2023-12-23 11:23:13.000000 STAIR-tools-1.2.5/STAIR/location/edge_detection.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     9354 2023-12-23 11:23:13.000000 STAIR-tools-1.2.5/STAIR/location/edge_detection1.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2298 2023-12-23 11:23:13.000000 STAIR-tools-1.2.5/STAIR/location/transformation.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2821 2023-12-23 11:23:13.000000 STAIR-tools-1.2.5/STAIR/utils.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-06 15:44:10.666804 STAIR-tools-1.2.5/STAIR_tools.egg-info/
--rw-r--r--   0 yuanyuan   (501) staff       (20)      253 2024-05-06 15:44:10.000000 STAIR-tools-1.2.5/STAIR_tools.egg-info/PKG-INFO
--rw-r--r--   0 yuanyuan   (501) staff       (20)      702 2024-05-06 15:44:10.000000 STAIR-tools-1.2.5/STAIR_tools.egg-info/SOURCES.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)        1 2024-05-06 15:44:10.000000 STAIR-tools-1.2.5/STAIR_tools.egg-info/dependency_links.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)        6 2024-05-06 15:44:10.000000 STAIR-tools-1.2.5/STAIR_tools.egg-info/top_level.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)       38 2024-05-06 15:44:10.667412 STAIR-tools-1.2.5/setup.cfg
--rw-------   0 yuanyuan   (501) staff       (20)      489 2024-05-06 15:43:42.000000 STAIR-tools-1.2.5/setup.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-06 16:55:20.361011 STAIR-tools-1.2.6/
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      253 2024-05-06 16:55:20.360719 STAIR-tools-1.2.6/PKG-INFO
+-rwxr-xr-x   0 yuanyuan   (501) staff       (20)     1320 2023-12-25 02:00:08.000000 STAIR-tools-1.2.6/README.md
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-06 16:55:20.355898 STAIR-tools-1.2.6/STAIR/
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8661 2023-12-23 11:23:09.000000 STAIR-tools-1.2.6/STAIR/ABA_annotation.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-06 16:55:20.356248 STAIR-tools-1.2.6/STAIR/ABAanno/
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.6/STAIR/ABAanno/__init__.py
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.6/STAIR/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    18514 2024-05-06 15:17:54.000000 STAIR-tools-1.2.6/STAIR/emb_alignment.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-06 16:55:20.358498 STAIR-tools-1.2.6/STAIR/embedding/
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2024-04-25 02:41:10.000000 STAIR-tools-1.2.6/STAIR/embedding/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3804 2024-05-04 11:27:47.000000 STAIR-tools-1.2.6/STAIR/embedding/dataset_ae.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     6011 2024-05-06 16:54:58.000000 STAIR-tools-1.2.6/STAIR/embedding/dataset_hgat.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)      988 2023-12-23 11:23:12.000000 STAIR-tools-1.2.6/STAIR/embedding/loss.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     5493 2023-12-23 11:23:12.000000 STAIR-tools-1.2.6/STAIR/embedding/module_ae.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8658 2023-12-23 11:23:12.000000 STAIR-tools-1.2.6/STAIR/embedding/module_hgat.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     6954 2023-12-23 11:23:12.000000 STAIR-tools-1.2.6/STAIR/embedding/module_hgat1.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    12320 2024-04-29 06:21:03.000000 STAIR-tools-1.2.6/STAIR/loc_alignment.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    14364 2024-04-28 11:59:13.000000 STAIR-tools-1.2.6/STAIR/loc_prediction.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-06 16:55:20.359936 STAIR-tools-1.2.6/STAIR/location/
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.6/STAIR/location/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     7819 2023-12-23 11:23:12.000000 STAIR-tools-1.2.6/STAIR/location/align_fine.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    11236 2023-12-23 11:23:13.000000 STAIR-tools-1.2.6/STAIR/location/align_init.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8534 2023-12-23 11:23:13.000000 STAIR-tools-1.2.6/STAIR/location/edge_detection.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     9354 2023-12-23 11:23:13.000000 STAIR-tools-1.2.6/STAIR/location/edge_detection1.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2298 2023-12-23 11:23:13.000000 STAIR-tools-1.2.6/STAIR/location/transformation.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2821 2023-12-23 11:23:13.000000 STAIR-tools-1.2.6/STAIR/utils.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-06 16:55:20.360518 STAIR-tools-1.2.6/STAIR_tools.egg-info/
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      253 2024-05-06 16:55:20.000000 STAIR-tools-1.2.6/STAIR_tools.egg-info/PKG-INFO
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      702 2024-05-06 16:55:20.000000 STAIR-tools-1.2.6/STAIR_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)        1 2024-05-06 16:55:20.000000 STAIR-tools-1.2.6/STAIR_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)        6 2024-05-06 16:55:20.000000 STAIR-tools-1.2.6/STAIR_tools.egg-info/top_level.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)       38 2024-05-06 16:55:20.363002 STAIR-tools-1.2.6/setup.cfg
+-rw-------   0 yuanyuan   (501) staff       (20)      489 2024-05-06 16:55:05.000000 STAIR-tools-1.2.6/setup.py
```

### Comparing `STAIR-tools-1.2.5/README.md` & `STAIR-tools-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.5/STAIR/ABA_annotation.py` & `STAIR-tools-1.2.6/STAIR/ABA_annotation.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.5/STAIR/emb_alignment.py` & `STAIR-tools-1.2.6/STAIR/emb_alignment.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.5/STAIR/embedding/dataset_ae.py` & `STAIR-tools-1.2.6/STAIR/embedding/dataset_ae.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.5/STAIR/embedding/dataset_hgat.py` & `STAIR-tools-1.2.6/STAIR/embedding/dataset_hgat.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         print('hom: ', batch_tmp)
         adata_tmp = adata[adata.obs[batch_key]==batch_tmp].copy()
         feat_tmp = adata_tmp.obsm['latent']
         coord_tmp = adata_tmp.obsm[spatial_key]
         adj_tmp = calcu_adj(coord_tmp, 
                             neigh_cal = 'knn', 
                             n_neigh = n_neigh_hom, 
-                            metric ='minkowski')._indices()
+                            metric ='minkowski')
         feat_dict[batch_tmp] = feat_tmp
         coord_dict[batch_tmp] = coord_tmp
         adj_dict[batch_tmp, '0', batch_tmp] = adj_tmp
         index_dict[batch_tmp] = list(adata_tmp.obs_names)
 
     # adjacency matrix between slices
     cross_adj_dict = {}
```

### Comparing `STAIR-tools-1.2.5/STAIR/embedding/loss.py` & `STAIR-tools-1.2.6/STAIR/embedding/loss.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.5/STAIR/embedding/module_ae.py` & `STAIR-tools-1.2.6/STAIR/embedding/module_ae.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.5/STAIR/embedding/module_hgat.py` & `STAIR-tools-1.2.6/STAIR/embedding/module_hgat.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.5/STAIR/embedding/module_hgat1.py` & `STAIR-tools-1.2.6/STAIR/embedding/module_hgat1.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.5/STAIR/loc_alignment.py` & `STAIR-tools-1.2.6/STAIR/loc_alignment.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.5/STAIR/loc_prediction.py` & `STAIR-tools-1.2.6/STAIR/loc_prediction.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.5/STAIR/location/align_fine.py` & `STAIR-tools-1.2.6/STAIR/location/align_fine.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.5/STAIR/location/align_init.py` & `STAIR-tools-1.2.6/STAIR/location/align_init.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.5/STAIR/location/edge_detection.py` & `STAIR-tools-1.2.6/STAIR/location/edge_detection.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.5/STAIR/location/edge_detection1.py` & `STAIR-tools-1.2.6/STAIR/location/edge_detection1.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.5/STAIR/location/transformation.py` & `STAIR-tools-1.2.6/STAIR/location/transformation.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.5/STAIR/utils.py` & `STAIR-tools-1.2.6/STAIR/utils.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.5/STAIR_tools.egg-info/SOURCES.txt` & `STAIR-tools-1.2.6/STAIR_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

