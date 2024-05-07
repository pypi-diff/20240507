# Comparing `tmp/pyVIA-0.1.992.tar.gz` & `tmp/pyVIA-0.1.993.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyVIA-0.1.992.tar", last modified: Thu Mar  7 02:47:15 2024, max compression
+gzip compressed data, was "pyVIA-0.1.993.tar", last modified: Tue May  7 07:53:14 2024, max compression
```

## Comparing `pyVIA-0.1.992.tar` & `pyVIA-0.1.993.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-07 02:47:15.636295 pyVIA-0.1.992/
--rwxr-xr-x   0 user      (1000) user      (1000)     1091 2020-09-15 01:01:11.000000 pyVIA-0.1.992/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)    19679 2024-03-07 02:47:15.636295 pyVIA-0.1.992/PKG-INFO
--rwxr-xr-x   0 user      (1000) user      (1000)    19436 2021-04-06 00:42:30.000000 pyVIA-0.1.992/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-07 02:47:15.636295 pyVIA-0.1.992/pyVIA/
--rwxr-xr-x   0 user      (1000) user      (1000)      142 2022-08-25 22:07:17.000000 pyVIA-0.1.992/pyVIA/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)   198051 2024-02-21 07:22:27.000000 pyVIA-0.1.992/pyVIA/core.py
--rwxr-xr-x   0 user      (1000) user      (1000)    14901 2024-02-20 06:46:27.000000 pyVIA-0.1.992/pyVIA/datasets_via.py
--rw-rw-r--   0 user      (1000) user      (1000)   160718 2024-02-20 03:31:08.000000 pyVIA-0.1.992/pyVIA/examples.py
--rw-rw-r--   0 user      (1000) user      (1000)   235007 2024-03-07 02:43:44.000000 pyVIA-0.1.992/pyVIA/plotting_via.py
--rwxr-xr-x   0 user      (1000) user      (1000)    96970 2024-02-21 07:16:06.000000 pyVIA-0.1.992/pyVIA/utils_via.py
--rw-rw-r--   0 user      (1000) user      (1000)     7987 2024-02-20 03:31:08.000000 pyVIA-0.1.992/pyVIA/windmap.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-07 02:47:15.636295 pyVIA-0.1.992/pyVIA.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    19679 2024-03-07 02:47:15.000000 pyVIA-0.1.992/pyVIA.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      304 2024-03-07 02:47:15.000000 pyVIA-0.1.992/pyVIA.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-03-07 02:47:15.000000 pyVIA-0.1.992/pyVIA.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      211 2024-03-07 02:47:15.000000 pyVIA-0.1.992/pyVIA.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        6 2024-03-07 02:47:15.000000 pyVIA-0.1.992/pyVIA.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-03-07 02:47:15.636295 pyVIA-0.1.992/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      959 2024-03-07 02:45:16.000000 pyVIA-0.1.992/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-07 07:53:14.779527 pyVIA-0.1.993/
+-rwxr-xr-x   0 user      (1000) user      (1000)     1091 2020-09-15 01:01:11.000000 pyVIA-0.1.993/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)    19679 2024-05-07 07:53:14.779527 pyVIA-0.1.993/PKG-INFO
+-rwxr-xr-x   0 user      (1000) user      (1000)    19436 2021-04-06 00:42:30.000000 pyVIA-0.1.993/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-07 07:53:14.779527 pyVIA-0.1.993/pyVIA/
+-rwxr-xr-x   0 user      (1000) user      (1000)      142 2022-08-25 22:07:17.000000 pyVIA-0.1.993/pyVIA/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)   198816 2024-05-07 07:51:17.000000 pyVIA-0.1.993/pyVIA/core.py
+-rwxr-xr-x   0 user      (1000) user      (1000)    14901 2024-02-20 06:46:27.000000 pyVIA-0.1.993/pyVIA/datasets_via.py
+-rw-rw-r--   0 user      (1000) user      (1000)   160718 2024-02-20 03:31:08.000000 pyVIA-0.1.993/pyVIA/examples.py
+-rw-rw-rw-   0 user      (1000) user      (1000)   236438 2024-05-07 07:35:16.000000 pyVIA-0.1.993/pyVIA/plotting_via.py
+-rwxr-xr-x   0 user      (1000) user      (1000)    97075 2024-04-12 02:40:43.000000 pyVIA-0.1.993/pyVIA/utils_via.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7987 2024-02-20 03:31:08.000000 pyVIA-0.1.993/pyVIA/windmap.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-07 07:53:14.779527 pyVIA-0.1.993/pyVIA.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    19679 2024-05-07 07:53:14.000000 pyVIA-0.1.993/pyVIA.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      304 2024-05-07 07:53:14.000000 pyVIA-0.1.993/pyVIA.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-07 07:53:14.000000 pyVIA-0.1.993/pyVIA.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      211 2024-05-07 07:53:14.000000 pyVIA-0.1.993/pyVIA.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        6 2024-05-07 07:53:14.000000 pyVIA-0.1.993/pyVIA.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-07 07:53:14.779527 pyVIA-0.1.993/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      957 2024-05-07 07:52:30.000000 pyVIA-0.1.993/setup.py
```

### Comparing `pyVIA-0.1.992/LICENSE.txt` & `pyVIA-0.1.993/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyVIA-0.1.992/PKG-INFO` & `pyVIA-0.1.993/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyVIA
-Version: 0.1.992
+Version: 0.1.993
 Home-page: https://github.com/ShobiStassen/VIA
 Author-email: shobana.venkat88@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `pyVIA-0.1.992/README.md` & `pyVIA-0.1.993/README.md`

 * *Files identical despite different names*

### Comparing `pyVIA-0.1.992/pyVIA/core.py` & `pyVIA-0.1.993/pyVIA/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -459,14 +459,16 @@
     edgepruning_clustering_resolution: float
         (optional, default = 0.15, can also set as 'median') graph pruning for PARC clustering stage. Higher value keeps more edges, results in fewer clusters. Smaller value removes more edges and results in more clusters. Number of standard deviations below the network’s mean-jaccard-weighted edges. 0.1-1 provide reasonable pruning.
         higher value means less pruning (more edges retained). e.g. a value of 0.15 means all edges that are above mean(edgeweight)-0.15*std(edge-weights) are retained.
         We find both 0.15 and ‘median’ to yield good results/starting point and resulting in pruning away ~ 50-60% edges
     keep_all_local_dist: bool, str
         default value of 'auto' means that for smaller datasets local-pruning is done prior to clustering, but for large datasets local pruning is set to False for speed.
         can also set to be bool of True or False
+    do_clustergraph_edgecontrol:bool=True
+        limits the max number of edges per cluster in the clustergraph to 30 edges. Applied after any pruning of edges and serves as a final sense-check that the number of edges per cluster doesnt become intractable
     too_big_factor: float
         (optional, default=0.4). Forces clusters > 0.4*n_cells to be re-clustered
     resolution_parameter: float
         (default =1) larger value means more and smaller clusters
     partition_type:str
         (default "ModularityVP") Options
     small_pop: int
@@ -607,25 +609,25 @@
         [n_samples x n_samples]
     terminal_clusters:list
         (default None) list of terminal clusters
     csr_full_graph: csr matrix of single-cell graph (augmented with sequential data when providing time_series information)
     csr_array_locally_pruned: csr matrix
     ig_full_graph:
     full_neighbor_array:
-    user_defined_terminal_cell:list=[]
-    user_defined_terminal_group:list=[]
+    user_defined_terminal_cell:list=[] list of cell indices corresponding to terminal fate cells
+    user_defined_terminal_group:list=[] list of group level labels corresponding to labels found in true_label, that represent cell fates
     n_milestones: int = None Number of milestones in the via-mds computation (anything more than 10,000 can be computationally heavy and time consuming) Typically auto-determined within the via-mds function
     embedding: ndarray
         [n_cells x 2] provided by user or autocomputed with via-mds or via-umap
 
     '''
 
     def __init__(self, data: ndarray, true_label=None, edgepruning_clustering_resolution_local: float = 1, edgepruning_clustering_resolution=0.15,
                  labels: ndarray = None,
-                 keep_all_local_dist='auto', too_big_factor: float = 0.4, resolution_parameter: float = 1.0,
+                 keep_all_local_dist='auto', do_clustergraph_edgecontrol:bool=True,too_big_factor: float = 0.4, resolution_parameter: float = 1.0,
                  partition_type: str = "ModularityVP", small_pop: int = 10,
                  jac_weighted_edges: bool = True, knn: int = 30, n_iter_leiden: int = 5, random_seed: int = 42,
                  num_threads=-1, distance='l2', time_smallpop=15,
                  super_cluster_labels: bool = False, super_node_degree_list: bool = False,
                  super_terminal_cells: bool = False, x_lazy: float = 0.99, alpha_teleport: float = 0.99,
                  root_user=None, preserve_disconnected: bool = True, dataset: str = '',
                  super_terminal_clusters: list = [],
@@ -658,14 +660,17 @@
         self.velo_weight = velo_weight  # float between 0,1. the weight assigned to directionality and connectivity derived from scRNA-velocity
         if edgebundle_pruning is None: edgebundle_pruning = cluster_graph_pruning
         self.edgebundle_pruning = edgebundle_pruning
         if (root_user is None) & (velocity_matrix is None):
             root_user = []
             dataset = ''
         self.root_user = root_user
+        if root_user is None:  dataset = ''
+        elif (type(root_user[0] == str)): dataset = 'group'
+        else: dataset = ''
         self.dataset = dataset
         self.knn_struct = None
         if isinstance(labels, list):
             labels = np.asarray(labels).flatten()
         self.labels = labels  # np.asarray(pre_labels).flatten() where pre_labels is a list
         self.connected_comp_labels = None
         self.edgelist = None
@@ -679,14 +684,15 @@
 
         if resolution_parameter != 1:
             partition_type = "RBVP"  # Reichardt and Bornholdt’s Potts model. Note that this is the same as ModularityVertexPartition when setting 𝛾 = 1 and normalising by 2m
 
         self.edgepruning_clustering_resolution_local = edgepruning_clustering_resolution_local
         self.edgepruning_clustering_resolution = edgepruning_clustering_resolution  ##0.15 is also a recommended value performing empirically similar to 'median'
         self.keep_all_local_dist = keep_all_local_dist
+        self.do_clustergraph_edgecontrol = do_clustergraph_edgecontrol
         self.too_big_factor = too_big_factor  ##if a cluster exceeds this share of the entire cell population, then the PARC will be run on the large cluster. at 0.4 it does not come into play
         self.resolution_parameter = resolution_parameter
         self.partition_type = partition_type
         self.small_pop = small_pop  # smallest cluster population to be considered a community
         self.jac_weighted_edges = jac_weighted_edges
         self.knn = knn
         self.knn_sequential = knn_sequential  # number of knn in the adjacent time-point for time-series data
@@ -793,18 +799,19 @@
         dict_user_defined_terminal_clusters = {}
         terminal_cluster_list = []
         if len(user_defined_terminal_cell) > 0:
             for i in user_defined_terminal_cell:
                 clus_ = self.labels[i]
                 if clus_ not in terminal_cluster_list:
                     terminal_cluster_list.append(clus_)
+                    dict_user_defined_terminal_clusters[user_defined_terminal_cell] = clus_
                 else:
                     print(f'{i} is a repeated terminal cluster')
-                    terminal_cluster_list.append(clus_)
-                    dict_user_defined_terminal_clusters[user_defined_terminal_cell] = clus_
+                    #terminal_cluster_list.append(clus_)
+
         else:
 
             for user_terminal_group in user_defined_terminal_group:
 
                 # location in indices of which cells belong to this user_terminal_group
                 index_terminal_group = np.where(np.asarray(self.true_label) == user_terminal_group)[0]
                 potential_clusters = self.labels[index_terminal_group]
@@ -2084,15 +2091,15 @@
 
         graph = recompute_weights(graph, Counter(self.labels))  # returns csr matrix
 
         self.cluster_graph_csr_not_pruned = graph  # type csr NOT PRUNED
         edgeweights_pruned_clustergraph, edges_pruned_clustergraph, comp_labels = pruning_clustergraph(graph,
                                                                                                        global_pruning_std=self.cluster_graph_pruning,
                                                                                                        preserve_disconnected=self.preserve_disconnected,
-                                                                                                       preserve_disconnected_after_pruning=self.preserve_disconnected_after_pruning)
+                                                                                                       preserve_disconnected_after_pruning=self.preserve_disconnected_after_pruning, do_max_outgoing=self.do_clustergraph_edgecontrol)
 
         self.connected_comp_labels = comp_labels
         # ig.graph() creates an undirected graph,in which case get_spare_from_igraph will be symmetric for each edge (u,v) and edge (v,u) is created
         locallytrimmed_g = ig.Graph(edges_pruned_clustergraph, edge_attrs={
             'weight': edgeweights_pruned_clustergraph})  # .simplify(combine_edges='sum') #forward biasing happens later
 
         locallytrimmed_sparse_vc = get_sparse_from_igraph(locallytrimmed_g, weight_attr='weight')
@@ -2112,15 +2119,15 @@
 
         # if using a different pruning for visualized edge bundles than the one specified in self.cluster_graph_pruning
         else:
 
             edgeweights_layout, edges_layout, comp_labels_layout = pruning_clustergraph(graph,
                                                                                         global_pruning_std=self.edgebundle_pruning,
                                                                                         preserve_disconnected=self.preserve_disconnected,
-                                                                                        preserve_disconnected_after_pruning=self.preserve_disconnected_after_pruning)
+                                                                                        preserve_disconnected_after_pruning=self.preserve_disconnected_after_pruning,do_max_outgoing=self.do_clustergraph_edgecontrol)
 
             # layout = locallytrimmed_g.layout_fruchterman_reingold(weights='weight') #uses non-clipped weights but this can skew layout due to one or two outlier edges
             layout_g = ig.Graph(edges_layout, edge_attrs={
                 'weight': edgeweights_layout})  # .simplify(combine_edges='sum') remving the 'combined_edges='sum' as it does not handle diagonal self loops which we require to be retained for singleton clusters that are not connected to other clusters
 
             layout_g_csr = get_sparse_from_igraph(layout_g, weight_attr='weight')
             weights_for_layout = np.asarray(layout_g_csr.data)
@@ -2235,15 +2242,15 @@
                         f"{datetime.now()}\tUsing the RNA velocity graph, A top3 candidate for initial state is {velo_root_candidate_i} comprising predominantly of {majority_truth} cells",
                     )
                 print(
                     f"{datetime.now()}\tUsing the RNA velocity graph, the suggested initial root state is {root_i} comprising predominantly of {majority_truth_veloroot0} cells")
 
 
             elif (self.dataset in ['toy', 'faced', 'mESC', 'iPSC', 'group']) and (
-                    self.root_user is not None):  # ((self.dataset == 'toy') | (self.dataset == 'faced')):
+                    self.root_user is not None):
                 root_user_ = None
                 for ri in self.root_user:
                     print(f"{datetime.now()}\tgroup root method")
                     if ri in sc_truelabels_subi:
                         root_user_ = ri
                         print(f"{datetime.now()}\tfor component {comp_i}, the root is {root_user_} and ri {ri}")
                 if root_user_ is None:
@@ -2798,15 +2805,15 @@
                     f'{datetime.now()}\tNo embedding will be computed: if you wish to compute a via-embedding specify one of via-force, via-mds or via-umap')
 
         if self.edgebundle_pruning_twice == False:
             # print('creating bundle with single round of global pruning at a level of', self.edgebundle_pruning)
             print(f"{datetime.now()}\tStarting make edgebundle viagraph...")
             self.hammerbundle_cluster, layout = make_edgebundle_viagraph(layout, g_layout, decay=self.viagraph_decay)
 
-        # simplifying structure of edges used on the visual layout
+        # simplifying structure of edges used on the visual layout (Used when doing edgebundling_pruning_twice AND differention flows)
         edgeweights_maxout_2, edgelist_maxout_2, comp_labels_2 = pruning_clustergraph(
             final_transition_matrix_all_components,
             global_pruning_std=self.visual_cluster_graph_pruning,
             max_outgoing=self.max_visual_outgoing_edges,
             preserve_disconnected=self.preserve_disconnected)
 
         if self.edgebundle_pruning_twice == True:
```

### Comparing `pyVIA-0.1.992/pyVIA/datasets_via.py` & `pyVIA-0.1.993/pyVIA/datasets_via.py`

 * *Files identical despite different names*

### Comparing `pyVIA-0.1.992/pyVIA/examples.py` & `pyVIA-0.1.993/pyVIA/examples.py`

 * *Files identical despite different names*

### Comparing `pyVIA-0.1.992/pyVIA/plotting_via.py` & `pyVIA-0.1.993/pyVIA/plotting_via.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,14 +153,15 @@
     :param via_object: via_object (best way to run this function by simply providing via_object)
     :param sc_graph: igraph graph set as the via attribute self.ig_full_graph (affinity graph)
     :param initial_bandwidth: increasing bw increases merging of minor edges
     :param decay: increasing decay increases merging of minor edges #https://datashader.org/user_guide/Networks.html
     :param milestone_labels: default list=[]. Usually autocomputed. but can provide as single-cell level labels (clusters, groups, which function as milestone groupings of the single cells)
     :param sc_labels_numeric: default is None which automatically chooses via_object's pseudotime or time_series_labels (when available). otherwise set to a list of numerical values representing some sequential/chronological information
     :param terminal_cluster_list: default list [] and automatically uses all terminal clusters. otherwise set to any of the terminal cluster numbers within a list
+    :param global_visual_pruning: prune the edges of the visualized StaVia clustergraph before edgebundling. default =0.5. Can take values (float) 0-3 (standard deviations), smaller number means fewer edges retained
     :return: dictionary containing keys: hb_dict['hammerbundle'] = hb hammerbundle class with hb.x and hb.y containing the coords
                 hb_dict['milestone_embedding'] dataframe with 'x' and 'y' columns for each milestone and hb_dict['edges'] dataframe with columns ['source','target'] milestone for each each and ['cluster_pop'], hb_dict['sc_milestone_labels'] is a list of milestone label for each single cell
 
     '''
     if embedding is None:
         if via_object is not None: embedding = via_object.embedding
 
@@ -208,15 +209,15 @@
     '''
     vertex_milestone_graph = ig.VertexClustering(sc_graph, membership=milestone_labels).cluster_graph(
         combine_edges='sum')
 
     print(f'{datetime.now()}\tRecompute weights')
     vertex_milestone_graph = recompute_weights(vertex_milestone_graph, Counter(milestone_labels))
     print(f'{datetime.now()}\tpruning milestone graph based on recomputed weights')
-    # was at 0.1 global_pruning for 2000+ milestones
+
     edgeweights_pruned_milestoneclustergraph, edges_pruned_milestoneclustergraph, comp_labels = pruning_clustergraph(
         vertex_milestone_graph,
         global_pruning_std=global_visual_pruning,
         preserve_disconnected=True,
         preserve_disconnected_after_pruning=False, do_max_outgoing=False)
 
     print(f'{datetime.now()}\tregenerate igraph on pruned edges')
@@ -442,15 +443,16 @@
         ax.set_yticks([])
         ax.axis('off')
     # Hide grid lines
     ax.grid(False)
     fig.patch.set_visible(True)
     if show_legend:
         ax.legend(fontsize=12, frameon=False)
-        legend = ax.legend(bbox_to_anchor=(1.02, 0.1), loc='upper left', borderaxespad=0)
+        #legend = ax.legend(bbox_to_anchor=(1.02, 0.1), loc='upper left', borderaxespad=0)
+        legend = ax.legend(bbox_to_anchor=(0, 0, 1.2, 1), loc='lower right', borderaxespad=0)
         for i, handle in enumerate(legend.legendHandles):
             # handle.set_edgecolor("#6c2167")  # set_edgecolors
             # handle.set_facecolor(colors[i])
             # handle.set_hatch(hatches[i])
             handle.set_alpha(1)
             handle.set_sizes([40])
     return fig, ax
@@ -1240,15 +1242,15 @@
         #VERY SLOW maybe try with dataframe mode  df.groupby(['team'])['points'].agg(pd.Series.mode)
         for labels_i in via_object.labels:
             loc_labels = np.where(np.asarray(via_object.labels) == labels_i)[0]
             majority_composition = func_mode(list(np.asarray(via_object.true_label)[loc_labels]))
             majority_cluster_population_dict[labels_i] = majority_composition
         print('f End getting majority comp')
         '''
-        for fst_i in via_object.terminal_clusters:
+        for fst_i in marker_lineages:#via_object.terminal_clusters:
             path_orange = G_orange.get_shortest_paths(via_object.root[ii], to=fst_i)[0]
             if len(path_orange) > 0:
                 print(
                     f'{datetime.now()}\tCluster path on clustergraph starting from Root Cluster {via_object.root[ii]} to Terminal Cluster {fst_i}: {path_orange}')
 
                 '''
                 cluster_population_dict = {}
@@ -1326,17 +1328,23 @@
                 revised_sc_path = []
                 for enum_i, clus in enumerate(cluster_path):
                     num_instances_clus = cluster_path.count(clus)
                     if (clus == cluster_path[0]) | (clus == cluster_path[-1]):
                         revised_cluster_path.append(clus)
                         revised_sc_path.append(path[enum_i])
                     else:
+                        '''
                         if num_instances_clus > 1:  # typically intermediate stages spend a few transitions at the sc level within a cluster
                             if clus not in revised_cluster_path: revised_cluster_path.append(clus)  # cluster
                             revised_sc_path.append(path[enum_i])  # index of single cell
+                        '''
+                        if  num_instances_clus >= 1:  # typically intermediate stages spend a few transitions at the sc level within a cluster
+                            if clus not in revised_cluster_path: revised_cluster_path.append(clus)  # cluster
+                            revised_sc_path.append(path[enum_i])  # index of single cell
+
                 print(
                     f"{datetime.now()}\tRevised Cluster level path on sc-knnGraph from Root Cluster {via_object.root[p1_cc[ti - 1]]} to Terminal Cluster {ts_current} along path: {revised_cluster_path}")
                 ti += 1
             fig.patch.set_visible(False)
             if fig_nrows == 1:
                 if fig_ncols == 1:
                     axs.axis('off')
@@ -1455,15 +1463,15 @@
                     headwidth_bundle: float = 0.1, headwidth_alpha: float = 0.8, arrow_frequency: float = 0.05,
                     show_arrow: bool = True, sc_labels_sequential: list = None, sc_labels_expression: list = None,
                     initial_bandwidth=0.03, decay=0.7, n_milestones: int = None, scale_scatter_size_pop: bool = False,
                     show_milestones: bool = True, sc_labels: list = None, text_labels: bool = False,
                     lineage_pathway: list = [], dpi: int = 300, fontsize_title: int = 6, fontsize_labels: int = 6,
                     global_visual_pruning=0.5, use_sc_labels_sequential_for_direction: bool = False, sc_scatter_size=3,
                     sc_scatter_alpha: float = 0.4, add_sc_embedding: bool = True, size_milestones: int = 5,
-                    colorbar_legend='pseudotime'):
+                    colorbar_legend='pseudotime',scale_arrow_headwidth:bool = False):
     '''
 
     Edges can be colored by time-series numeric labels, pseudotime, lineage pathway probabilities,  or gene expression. If not specificed then time-series is chosen if available, otherwise falls back to pseudotime. to use gene expression the sc_labels_expression is provided as a list.
     To specify other numeric sequential data provide a list of sc_labels_sequential = [] n_samples in length. via_object.embedding must be an ndarray of shape (nsamples,2)
 
     :param hammer_bundle_dict: dictionary with keys: hammerbundle object with coordinates of all the edges to draw. If hammer_bundle and layout are None, then this will be computed internally
     :param via_object: type via object, if hammerbundle_dict is None, then you must provide a via_object. Ensure that via_object has embedding attribute
@@ -1810,34 +1818,38 @@
                             for v1 in arrow_coords:
                                 dist_ = dist_points(v1, v2=[seg_p[mid_point, 0], seg_p[mid_point, 1]])
 
                                 if dist_ < arrow_frequency * delta_x: do_arrow = False
                                 if dist_ < arrow_frequency * delta_y: do_arrow = False
 
                         if (do_arrow == True) & (seg_p.shape[0] > 3):
+                            if scale_arrow_headwidth:
+                                headwidth_bundle_ = headwidth_bundle*min(seg_weight,1)
+                                print('doing scale arrow headwidth:', headwidth_bundle_)
+                            else: headwidth_bundle_ = headwidth_bundle
                             if fig_nrows == 1:
                                 if fig_ncols == 1:
                                     ax.arrow(seg_p[mid_point, 0], seg_p[mid_point, 1],
                                              seg_p[mid_point + (direction * step), 0] - seg_p[mid_point, 0],
                                              seg_p[mid_point + (direction * step), 1] - seg_p[mid_point, 1],
-                                             lw=0, length_includes_head=False, head_width=headwidth_bundle, color=rgba,
+                                             lw=0, length_includes_head=False, head_width=headwidth_bundle_, color=rgba,
                                              shape='full', alpha=headwidth_alpha, zorder=5)
 
                                 else:
                                     ax[c].arrow(seg_p[mid_point, 0], seg_p[mid_point, 1],
                                                 seg_p[mid_point + (direction * step), 0] - seg_p[mid_point, 0],
                                                 seg_p[mid_point + (direction * step), 1] - seg_p[mid_point, 1],
-                                                lw=0, length_includes_head=False, head_width=headwidth_bundle,
+                                                lw=0, length_includes_head=False, head_width=headwidth_bundle_,
                                                 color=rgba, shape='full', alpha=headwidth_alpha, zorder=5)
 
                             else:
                                 ax[r, c].arrow(seg_p[mid_point, 0], seg_p[mid_point, 1],
                                                seg_p[mid_point + (direction * step), 0] - seg_p[mid_point, 0],
                                                seg_p[mid_point + (direction * step), 1] - seg_p[mid_point, 1],
-                                               lw=0, length_includes_head=False, head_width=headwidth_bundle,
+                                               lw=0, length_includes_head=False, head_width=headwidth_bundle_,
                                                color=rgba, shape='full', alpha=headwidth_alpha, zorder=5)
                             arrow_coords.append([seg_p[mid_point, 0], seg_p[mid_point, 1]])
 
                     seg_count += 1
                 if show_milestones == False:
                     size_milestones = 0.01
                     show_milestones = True
@@ -2890,14 +2902,16 @@
                         weights = np.asarray(sc_bp[:, i_terminal])[loc_].reshape(-1, 1)
 
                         if len(loc_) > 1:
                             geneGAM = pg.LinearGAM(n_splines=n_splines, spline_order=spline_order, lam=10).fit(x, y,
                                                                                                                weights=weights)
                             xval = np.linspace(min(sc_pt), max_val_pt, 100 * 2)
                             yg = geneGAM.predict(X=xval)
+                            A_under_curve = np.trapz(yg, x=xval)
+                            print(f'Area under curve {gene_i} for branch {majority_true} is {A_under_curve}')
 
                         else:
                             print(
                                 f'{datetime.now()}\tLineage {i_terminal} cannot be reached. Exclude this lineage in trend plotting')
                         if cmap_dict is None:
                             color_ = cmap_[enum_i_lineage]
                         else:
@@ -3409,17 +3423,17 @@
     # X_mds = squareform(pdist(adata_counts.obsm['X_pca'][:, 0:ncomps+20])) #no diffusion makes is less streamlined and compact. more fuzzy
     return X_mds
 
 def plot_piechart_only_viagraph(via_object, type_data='pt', gene_exp: list = [], cmap_piechart: str = 'rainbow', title='',
                            cmap: str = None, ax_text=True, dpi=150, headwidth_arrow=0.1, alpha_edge=0.4,
                            linewidth_edge=2, edge_color='darkblue', reference_labels=None, show_legend: bool = True,
                            pie_size_scale: float = 0.8, fontsize: float = 8, pt_visual_threshold: int = 99,
-                           highlight_terminal_clusters: bool = True, size_node_notpiechart: float = 1,tune_edges:bool = False,initial_bandwidth=0.05, decay=0.9, edgebundle_pruning=0.5):
+                           highlight_terminal_clusters: bool = True, tune_edges:bool = False,initial_bandwidth=0.05, decay=0.9, edgebundle_pruning=0.5):
     '''
-    plot two subplots with a clustergraph level representation of the viagraph showing true-label composition (lhs) and pseudotime/gene expression (rhs)
+    plot clustergraph level representation of the viagraph showing true-label composition (lhs) and pseudotime/gene expression (rhs)
     Returns matplotlib figure with two axes that plot the clustergraph using edge bundling
     left axis shows the clustergraph with each node colored by annotated ground truth membership.
     right axis shows the same clustergraph with each node colored by the pseudotime or gene expression
 
     :param via_object: is class VIA (the same function also exists as a method of the class and an external plotting function
     :param type_data: string  default 'pt' for pseudotime colored nodes. or 'gene'
     :param gene_exp: list of values (or column of dataframe) corresponding to feature or gene expression to be used to color nodes at CLUSTER level
@@ -3716,15 +3730,20 @@
 
     patches, texts = pie_axs[node_i].pie(frac, wedgeprops={'linewidth': 0.0}, colors=color_true_list)
     labels = list(set(reference_labels))
     labels.sort()
     if show_legend == True: plt.legend(patches, labels, loc=(-5, -5), fontsize=6, frameon=False)
 
     if via_object.time_series == True:
-        ti = 'Cluster Composition. K=' + str(via_object.knn) + '. ncomp = ' + str(via_object.ncomp) + 'knnseq_' + str(
+        ti = 'Cluster Composition. K=' + str(via_object.knn) + '. ncomp = ' + str(via_object.ncomp) + 'Temporalknn_' + str(
+            via_object.knn_sequential)
+        if via_object.do_spatial_knn == True:
+            ti = 'Cluster Composition. K=' + str(via_object.knn) + '. ncomp = ' + str(
+                via_object.ncomp) + 'SpatKnn_' + str(
+                via_object.spatial_knn) + 'Temporalknn_' + str(
             via_object.knn_sequential)
     elif via_object.do_spatial_knn == True:
         ti = 'Cluster Composition. K=' + str(via_object.knn) + '. ncomp = ' + str(via_object.ncomp) + 'SpatKnn_' + str(
             via_object.spatial_knn)
     else:
         ti = 'Cluster Composition. K=' + str(via_object.knn) + '. ncomp = ' + str(via_object.ncomp)
     ax.set_title(ti)
```

### Comparing `pyVIA-0.1.992/pyVIA/utils_via.py` & `pyVIA-0.1.993/pyVIA/utils_via.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,14 +259,15 @@
 
     if do_max_outgoing == True: trimmed_n = (initial_links_n - final_links_n) * 100. / initial_links_n
     trimmed_n_glob = (initial_links_n - len(weights)) * 100. / initial_links_n
     if do_max_outgoing == True: print(
         f"{datetime.now()}\t{round(trimmed_n, 1)}% links trimmed from local pruning relative to start")
     if global_pruning_std < 0.5:
         print(f"{datetime.now()}\t{round(trimmed_n_glob, 1)}% links trimmed from global pruning relative to start")
+        if do_max_outgoing: print(f'initial links {initial_links_n} and final_links_n {final_links_n}')
 
     return weights, edges, comp_labels
 
 
 def get_sparse_from_igraph(graph: ig.Graph, weight_attr=None):
     '''
 
@@ -1334,15 +1335,15 @@
 
     pi /= np.sum(pi)
 
     print(f"{datetime.now()}\tStationary distribution normed {np.round(pi, 3)}")
     sorted_pi = np.argsort(pi)
     velo_root_top10 = sorted_pi[0:10]
     print(
-        f"{datetime.now()}\tTop 5 candidates for root: {np.round(sorted_pi[0:10], 2)} with stationary prob (%) {np.round(pi[sorted_pi[0:10]] * 100, 3)}")
+        f"{datetime.now()}\tTop 10 candidates for root: {np.round(sorted_pi[0:10], 2)} with stationary prob (%) {np.round(pi[sorted_pi[0:10]] * 100, 3)}")
     print(f"{datetime.now()}\tTop 5 candidates for terminal: {np.flip(sorted_pi)[0:5]}")
 
     return pi, velo_root_top10
 
 
 def velocity_transition(A, V, G, slope=4):
     '''
```

### Comparing `pyVIA-0.1.992/pyVIA/windmap.py` & `pyVIA-0.1.993/pyVIA/windmap.py`

 * *Files identical despite different names*

### Comparing `pyVIA-0.1.992/pyVIA.egg-info/PKG-INFO` & `pyVIA-0.1.993/pyVIA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyVIA
-Version: 0.1.992
+Version: 0.1.993
 Home-page: https://github.com/ShobiStassen/VIA
 Author-email: shobana.venkat88@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `pyVIA-0.1.992/setup.py` & `pyVIA-0.1.993/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='pyVIA',
-    version='0.1.992', ##March 7, 2024
+    version='0.1.993', ##May 7, 2024
     packages=['pyVIA',],
     license='MIT',
     author_email = 'shobana.venkat88@gmail.com',
     url = 'https://github.com/ShobiStassen/VIA',
     setup_requires = ['numpy>=1.17','pybind11'],
     python_requires = ">=3.8",
     install_requires=['pybind11','numpy>=1.17','scipy','pandas>=0.25','hnswlib','igraph','leidenalg>=0.7.0', 'scikit-learn', 'termcolor','pygam', 'matplotlib','scanpy','umap-learn>=0.5.0','phate','datashader', 'scikit-image', 'pillow','wget','gdown','seaborn','pecanpy','holoviews'],
```

