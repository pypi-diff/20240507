# Comparing `tmp/ComSeg-0.0.5.tar.gz` & `tmp/comseg-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ComSeg-0.0.5.tar", last modified: Sun Mar 10 20:50:49 2024, max compression
+gzip compressed data, was "comseg-0.0.7.tar", last modified: Tue May  7 17:02:50 2024, max compression
```

## Comparing `ComSeg-0.0.5.tar` & `comseg-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-03-10 20:50:49.583917 ComSeg-0.0.5/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1056 2023-10-04 17:16:12.000000 ComSeg-0.0.5/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)     1874 2024-03-10 20:50:49.583917 ComSeg-0.0.5/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)      756 2024-01-04 19:49:48.000000 ComSeg-0.0.5/README.md
--rw-rw-r--   0 tom       (1000) tom       (1000)      610 2024-03-10 20:50:43.000000 ComSeg-0.0.5/pyproject.toml
--rw-rw-r--   0 tom       (1000) tom       (1000)      356 2024-01-04 17:54:13.000000 ComSeg-0.0.5/requirements.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2024-03-10 20:50:49.583917 ComSeg-0.0.5/setup.cfg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-03-10 20:50:49.579917 ComSeg-0.0.5/src/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-03-10 20:50:49.583917 ComSeg-0.0.5/src/ComSeg.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     1874 2024-03-10 20:50:49.000000 ComSeg-0.0.5/src/ComSeg.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)      504 2024-03-10 20:50:49.000000 ComSeg-0.0.5/src/ComSeg.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2024-03-10 20:50:49.000000 ComSeg-0.0.5/src/ComSeg.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)      353 2024-03-10 20:50:49.000000 ComSeg-0.0.5/src/ComSeg.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       16 2024-03-10 20:50:49.000000 ComSeg-0.0.5/src/ComSeg.egg-info/top_level.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        9 2024-02-13 12:19:38.000000 ComSeg-0.0.5/src/__init__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-03-10 20:50:49.583917 ComSeg-0.0.5/src/comseg/
--rw-rw-r--   0 tom       (1000) tom       (1000)      405 2024-03-10 20:50:43.000000 ComSeg-0.0.5/src/comseg/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    18308 2024-02-13 13:33:03.000000 ComSeg-0.0.5/src/comseg/clustering.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    17248 2024-03-10 20:29:48.000000 ComSeg-0.0.5/src/comseg/dataset.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    18527 2024-02-18 12:58:29.000000 ComSeg-0.0.5/src/comseg/dictionary.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    35923 2023-12-12 10:56:00.000000 ComSeg-0.0.5/src/comseg/model.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-03-10 20:50:49.583917 ComSeg-0.0.5/src/comseg/utils/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2023-08-02 11:20:30.000000 ComSeg-0.0.5/src/comseg/utils/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    18730 2023-12-13 09:11:34.000000 ComSeg-0.0.5/src/comseg/utils/custom_louvain.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1887 2023-10-03 13:00:25.000000 ComSeg-0.0.5/src/comseg/utils/plot.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     8640 2023-11-21 18:48:35.000000 ComSeg-0.0.5/src/comseg/utils/preprocessing.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3292 2023-10-25 14:42:29.000000 ComSeg-0.0.5/src/comseg/utils/utils_graph.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-07 17:02:50.462541 comseg-0.0.7/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1056 2023-10-04 17:16:12.000000 comseg-0.0.7/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)     1191 2024-05-07 17:02:50.462541 comseg-0.0.7/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)      756 2024-01-04 19:49:48.000000 comseg-0.0.7/README.md
+-rw-rw-r--   0 tom       (1000) tom       (1000)      513 2024-05-07 17:02:43.000000 comseg-0.0.7/pyproject.toml
+-rw-rw-r--   0 tom       (1000) tom       (1000)      356 2024-01-04 17:54:13.000000 comseg-0.0.7/requirements.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2024-05-07 17:02:50.462541 comseg-0.0.7/setup.cfg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-07 17:02:50.458541 comseg-0.0.7/src/
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-07 17:02:50.462541 comseg-0.0.7/src/ComSeg.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1191 2024-05-07 17:02:50.000000 comseg-0.0.7/src/ComSeg.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)      471 2024-05-07 17:02:50.000000 comseg-0.0.7/src/ComSeg.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2024-05-07 17:02:50.000000 comseg-0.0.7/src/ComSeg.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       16 2024-05-07 17:02:50.000000 comseg-0.0.7/src/ComSeg.egg-info/top_level.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        9 2024-02-13 12:19:38.000000 comseg-0.0.7/src/__init__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-07 17:02:50.462541 comseg-0.0.7/src/comseg/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      405 2024-05-07 15:28:06.000000 comseg-0.0.7/src/comseg/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    18309 2024-03-19 13:32:23.000000 comseg-0.0.7/src/comseg/clustering.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    18590 2024-05-07 15:22:51.000000 comseg-0.0.7/src/comseg/dataset.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    18478 2024-05-07 16:26:44.000000 comseg-0.0.7/src/comseg/dictionary.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    35878 2024-05-07 15:33:03.000000 comseg-0.0.7/src/comseg/model.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-07 17:02:50.462541 comseg-0.0.7/src/comseg/utils/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2023-08-02 11:20:30.000000 comseg-0.0.7/src/comseg/utils/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    18790 2024-05-07 15:31:41.000000 comseg-0.0.7/src/comseg/utils/custom_louvain.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1887 2023-10-03 13:00:25.000000 comseg-0.0.7/src/comseg/utils/plot.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     8640 2023-11-21 18:48:35.000000 comseg-0.0.7/src/comseg/utils/preprocessing.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3292 2023-10-25 14:42:29.000000 comseg-0.0.7/src/comseg/utils/utils_graph.py
```

### Comparing `ComSeg-0.0.5/LICENSE` & `comseg-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ComSeg-0.0.5/README.md` & `comseg-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ComSeg-0.0.5/pyproject.toml` & `comseg-0.0.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 
 
 
+
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "ComSeg"
-version = "0.0.5"
+version = "0.0.7"
 authors = [
   { name="Thomas Defard", email="thomas.defard@mines-paristech.fr" },
 ]
 description = "single cell RNA profiling analysis of imaging-based spatial transcriptomics data"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
-]
-dynamic = ["dependencies"]
-[tool.setuptools.dynamic]
-dependencies = {file = ["requirements.txt"]}
+]
```

### Comparing `ComSeg-0.0.5/src/comseg/clustering.py` & `comseg-0.0.7/src/comseg/clustering.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,14 +94,15 @@
                               n_comps =15,
                               clustering_method ="leiden",
                               n_neighbors = 20,
                               resolution = 1,
                               n_clusters_kmeans = 4,
                               palette = None,
                               plot_umap = False):
+
         """
         Cluster the RNA partition/community expression vector to identify the single cell transcriptomic cluster present in the dataset
 
         :param size_commu_min: minimum number of RNA in a community to be considered for the clustering
         :type size_commu_min: int
         :param norm_vector: if True, the expression vector will be normalized using the scTRANSFORM normalization parameters
         :type norm_vector: bool
```

### Comparing `ComSeg-0.0.5/src/comseg/dataset.py` & `comseg-0.0.7/src/comseg/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,15 +151,18 @@
 
     ### compute the co-expression matrix
 
     def count_matrix_in_situ_from_knn(self,
                                       df_spots_label,
                                       n_neighbors=5,
                                       radius=None,
-                                      remove_self_node = False):
+                                      remove_self_node = False,
+                                      sampling=True,
+                                      sampling_size=10000
+                                      ):
 
 
         """
         Compute the co-expression score matrix for the RNA spatial distribution
 
         :param df_spots_label:  dataframe with the columns x,y,z,gene. the coordinates are rescaled in µm by dict_scale attribute of the dataset object
         :type df_spots_label: pd.DataFrame
@@ -175,14 +178,17 @@
         for gene_id in range(len(self.selected_genes)):
             gene_index_dico[self.selected_genes[gene_id]] = gene_id #todo gene_index_dico to add in self
         ## this part should be factorize with create_directed_nn_graph
         try:
             df_spots_label = df_spots_label.reset_index()
         except Exception as e:
             print(e)
+
+
+
         if "z" in df_spots_label.columns:
             list_coordo_order_no_scaling = np.array([df_spots_label.z, df_spots_label.y, df_spots_label.x]).T
             list_coordo_order = list_coordo_order_no_scaling * np.array(
                 [self.dict_scale['z'], self.dict_scale['y'], self.dict_scale["x"]])
         else:
             list_coordo_order_no_scaling = np.array([df_spots_label.y, df_spots_label.x]).T
             list_coordo_order = list_coordo_order_no_scaling * np.array([self.dict_scale['y'], self.dict_scale['x']])
@@ -199,16 +205,38 @@
 
         nbrs = NearestNeighbors(n_neighbors=n_neighbors, algorithm='ball_tree').fit(list_coordo_order)
         ad = nbrs.kneighbors_graph(list_coordo_order)  ## can be optimize here
         distance = nbrs.kneighbors_graph(list_coordo_order, mode='distance')
         ad[distance > radius] = 0
         ad.eliminate_zeros()
 
+
         rows, cols, BOL = sp.find(ad == 1)
-        edges = list(zip(rows.tolist(), cols.tolist()))
+
+        ## dratf optimisation
+        unique_rows = np.unique(rows)
+        if sampling:
+            if len(unique_rows) > sampling_size:
+                unique_rows = np.random.choice(unique_rows, sampling_size, replace=False)
+
+        list_expression_vec = []
+        for row in unique_rows:
+            col_index = np.nonzero(ad[row])[1]
+            if remove_self_node:
+                col_index = col_index[col_index != row]
+            vectors_gene = list(array_gene_indexed[col_index])
+            vector_distance = np.array([distance[row, col] for col in col_index])
+            expression_vector = np.zeros(len(self.selected_genes))
+            for str_gene_index in range(len(vectors_gene)):
+                str_gene = vectors_gene[str_gene_index]
+                expression_vector[gene_index_dico[str_gene]] += (radius  - 1 *  vector_distance[str_gene_index]) / radius
+            list_expression_vec.append(expression_vector)
+        count_matrix = np.array(list_expression_vec)
+
+        """edges = list(zip(rows.tolist(), cols.tolist()))
 
         G = nx.DiGraph()  # oriented graph
         G.add_nodes_from(list_features_order)
         weighted_edges = [(e[0], e[1], distance[e[0], e[1]]) for e in edges]
         G.add_weighted_edges_from(weighted_edges)
 
         list_expression_vec = []
@@ -220,30 +248,32 @@
             vector_distance = np.array([G[node][suc]['weight'] for suc in G.successors(node)])
             # vector_distance
             expression_vector = np.zeros(len(self.selected_genes))
             for str_gene_index in range(len(vectors_gene)):
                 str_gene = vectors_gene[str_gene_index]
                 expression_vector[gene_index_dico[str_gene]] += (radius  - 1 *  vector_distance[str_gene_index]) / radius
             list_expression_vec.append(expression_vector)
-        count_matrix = np.array(list_expression_vec)
+        count_matrix = np.array(list_expression_vec)"""
         return count_matrix
 
-    def get_dict_proba_edge_in_situ(self, count_matrix,
+    def get_dict_proba_edge_in_situ(self,
+                                    count_matrix,
                                     distance="pearson",
                                     ):
         """
         compute the co-expression correlation matrix from the count_matrix
 
         :param count_matrix: cell by gene matrix
         :type count_matrix: np.array
         :param distance:  choose in ["pearson", "spearman"] default is pearson
         :type distance: str
         :return: a dictionary of dictionary corelation between genes dict[gene_source][gene_target] = correlation
         :rtype: dict
         """
+
         import math
         assert distance in ["spearman", "pearson"]
         from tqdm import tqdm
         dico_proba_edge = {}
         for gene_source in range(len(self.selected_genes)):  # I compute the same thing twice ...
             dico_proba_edge[self.selected_genes[gene_source]] = {}
 
@@ -267,17 +297,16 @@
 
     def compute_edge_weight(
             self,
             images_subset = None,
             n_neighbors=40,
             radius= None ,  # in micormeter
             distance="pearson",
-            sampling=False,
-            sampling_size=100000,
-            sampling_images = False,
+            sampling=True,
+            sampling_size=10000,
     remove_self_node = False):
 
         #print("adapt to when I prune")
 
         """
         compute the gene co-expression correlation at the dataset scale
 
@@ -318,15 +347,17 @@
             #print(df_spots_label)
 
 
             print("image name : ", image_name)
             count_matrix = self.count_matrix_in_situ_from_knn(df_spots_label=df_spots_label,  # df_spots_label,
                                                          n_neighbors=n_neighbors,
                                                          radius=radius,
-                                                        remove_self_node=remove_self_node)
+                                                        remove_self_node=remove_self_node,
+                                                              sampling=True,
+                                                              sampling_size=int(sampling_size/len(list_img) +1))
             list_of_count_matrix.append(count_matrix)
             count_matrix = np.concatenate(list_of_count_matrix, axis=0)
         if sampling:
             if len(count_matrix) > sampling_size:
                 print("count_matrix.shape", count_matrix.shape)
                 print(f"sampling {sampling} vectors")
                 count_matrix = count_matrix[np.random.choice(count_matrix.shape[0], sampling_size, replace=False), :]
```

### Comparing `ComSeg-0.0.5/src/comseg/dictionary.py` & `comseg-0.0.7/src/comseg/dictionary.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,15 +354,14 @@
     def classify_centroid(self,
                       path_dict_cell_centroid = None,
                       n_neighbors=15,
                       dict_in_pixel=True,
                       max_dist_centroid=None,
                       key_pred="leiden_merged",
                       distance="ngb_distance_weights",
-                      convex_hull_centroid=True,
                         file_extension = "tiff.npy"
                       ):
 
         """
         Classify cell centroids based on their  centroid neighbors RNA
         label from ``add_cluster_id_to_graph()``
```

### Comparing `ComSeg-0.0.5/src/comseg/model.py` & `comseg-0.0.7/src/comseg/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,14 @@
                 partition += [set(list_nodes[array_super_node_prior == super_node])]
         else:
             partition = None
 
         assert nx.is_directed(self.G)
         G = self.G.copy()
         G.remove_edges_from([(d[0], d[1]) for d in list(G.edges(data=True)) if d[2]["weight"] < 0])
-        print("only positive w selected")
         if clustering_method == "louvain":
             comm = nx_comm.louvain_communities(G.to_undirected(reciprocal=False),
                                                weight="weight",
                                                resolution=self.resolution,
                                                seed=seed)
 
 
@@ -751,19 +750,16 @@
         csv_list_cell = []
         csv_index_list = []
         for cell_index in range(len(list_cell_id)):
             if len(list_genes_name[cell_index]) > 0:
                 csv_list_z += list(np.array(list_cell_genes_coordinate[cell_index])[:, 0])
                 csv_list_y += list(np.array(list_cell_genes_coordinate[cell_index])[:, 1])
                 csv_list_x += list(np.array(list_cell_genes_coordinate[cell_index])[:, 2])
-
-
                 csv_list_cell += [list_cell_id[cell_index]] * len(list_genes_name[cell_index])
                 csv_list_gene += list_genes_name[cell_index]
-
                 csv_index_list += list(dict_cell_genes_mol_index[list_cell_id[cell_index]])
 
         df_spots = pd.DataFrame({"z": csv_list_z,
                                  "y": csv_list_y,
                                  "x": csv_list_x,
                                  "gene": csv_list_gene,
                                  "cell": csv_list_cell,
```

### Comparing `ComSeg-0.0.5/src/comseg/utils/custom_louvain.py` & `comseg-0.0.7/src/comseg/utils/custom_louvain.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,14 +238,15 @@
         new_mod = modularity(
             graph, inner_partition, resolution=resolution, weight="weight"
         )
         graph = _gen_graph(graph, partition = inner_partition)
         if new_mod - mod <= threshold:
             print(f'stop because of threshold {new_mod - mod} inf to {threshold}')
             return
+        print(f'improvement of modularity {new_mod - mod}')
         mod = new_mod
         yield [s.copy() for s in partition], graph
 
         partition, inner_partition, improvement = _one_level(
             graph=graph,
             m=m,
             partition=partition,
```

### Comparing `ComSeg-0.0.5/src/comseg/utils/plot.py` & `comseg-0.0.7/src/comseg/utils/plot.py`

 * *Files identical despite different names*

### Comparing `ComSeg-0.0.5/src/comseg/utils/preprocessing.py` & `comseg-0.0.7/src/comseg/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `ComSeg-0.0.5/src/comseg/utils/utils_graph.py` & `comseg-0.0.7/src/comseg/utils/utils_graph.py`

 * *Files identical despite different names*

