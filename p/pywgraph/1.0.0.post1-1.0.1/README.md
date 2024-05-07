# Comparing `tmp/pywgraph-1.0.0.post1.tar.gz` & `tmp/pywgraph-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywgraph-1.0.0.post1.tar", last modified: Sun May  5 18:54:41 2024, max compression
+gzip compressed data, was "pywgraph-1.0.1.tar", last modified: Tue May  7 19:46:34 2024, max compression
```

## Comparing `pywgraph-1.0.0.post1.tar` & `pywgraph-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:54:41.050526 pywgraph-1.0.0.post1/
--rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-05-05 18:54:41.046526 pywgraph-1.0.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-05-05 18:54:37.000000 pywgraph-1.0.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:54:41.046526 pywgraph-1.0.0.post1/pywgraph/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-05 18:54:37.000000 pywgraph-1.0.0.post1/pywgraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-05 18:54:37.000000 pywgraph-1.0.0.post1/pywgraph/_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-05 18:54:37.000000 pywgraph-1.0.0.post1/pywgraph/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-05-05 18:54:37.000000 pywgraph-1.0.0.post1/pywgraph/_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-05 18:54:37.000000 pywgraph-1.0.0.post1/pywgraph/_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-05 18:54:37.000000 pywgraph-1.0.0.post1/pywgraph/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:54:41.046526 pywgraph-1.0.0.post1/pywgraph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-05-05 18:54:41.000000 pywgraph-1.0.0.post1/pywgraph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-05 18:54:41.000000 pywgraph-1.0.0.post1/pywgraph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 18:54:41.000000 pywgraph-1.0.0.post1/pywgraph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-05 18:54:41.000000 pywgraph-1.0.0.post1/pywgraph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-05 18:54:41.000000 pywgraph-1.0.0.post1/pywgraph.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 18:54:41.050526 pywgraph-1.0.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-05 18:54:37.000000 pywgraph-1.0.0.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:54:41.046526 pywgraph-1.0.0.post1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:54:37.000000 pywgraph-1.0.0.post1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-05 18:54:37.000000 pywgraph-1.0.0.post1/tests/test_directed_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-05 18:54:37.000000 pywgraph-1.0.0.post1/tests/test_path_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-05 18:54:37.000000 pywgraph-1.0.0.post1/tests/test_weighted_directed_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-05 18:54:37.000000 pywgraph-1.0.0.post1/tests/test_weighted_directed_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-05 18:54:37.000000 pywgraph-1.0.0.post1/tests/test_weighted_directed_graph_arrays.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:46:34.808596 pywgraph-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-05-07 19:46:34.804595 pywgraph-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11272 2024-05-07 19:46:28.000000 pywgraph-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:46:34.804595 pywgraph-1.0.1/pywgraph/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 19:46:28.000000 pywgraph-1.0.1/pywgraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-07 19:46:28.000000 pywgraph-1.0.1/pywgraph/_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-07 19:46:28.000000 pywgraph-1.0.1/pywgraph/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-05-07 19:46:28.000000 pywgraph-1.0.1/pywgraph/_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-07 19:46:28.000000 pywgraph-1.0.1/pywgraph/_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-07 19:46:28.000000 pywgraph-1.0.1/pywgraph/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:46:34.804595 pywgraph-1.0.1/pywgraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-05-07 19:46:34.000000 pywgraph-1.0.1/pywgraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-07 19:46:34.000000 pywgraph-1.0.1/pywgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:46:34.000000 pywgraph-1.0.1/pywgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-07 19:46:34.000000 pywgraph-1.0.1/pywgraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-07 19:46:34.000000 pywgraph-1.0.1/pywgraph.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 19:46:34.808596 pywgraph-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-07 19:46:28.000000 pywgraph-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:46:34.804595 pywgraph-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:46:28.000000 pywgraph-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-07 19:46:28.000000 pywgraph-1.0.1/tests/test_directed_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-07 19:46:28.000000 pywgraph-1.0.1/tests/test_path_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-07 19:46:28.000000 pywgraph-1.0.1/tests/test_weighted_directed_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-05-07 19:46:28.000000 pywgraph-1.0.1/tests/test_weighted_directed_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-07 19:46:28.000000 pywgraph-1.0.1/tests/test_weighted_directed_graph_arrays.py
```

### Comparing `pywgraph-1.0.0.post1/PKG-INFO` & `pywgraph-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: pywgraph
-Version: 1.0.0.post1
+Version: 1.0.1
 Summary: A python implementation of weighted directed graphs where weights can be elements of a mathematical group
+Home-page: https://github.com/josek98/pywgraph
 Author: josek98
 Author-email: josemmsscc98@gmail.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Requires-Dist: pytest>=7.0; extra == "dev"
 Requires-Dist: twine>=4.0.2; extra == "dev"
@@ -255,7 +256,14 @@
 # None
 
 graph.weight_between("A", "Z", np.array([1,1]))
 # np.array([1,1])
 ```
 
 Notice that this graph is not conmutative since the weight of the path `["A", "C"]` is different from the weight of the path `["A", "B", "C]`.
+
+## Release Notes
+
+### Version 1.0.1 (2024-05-07)
+
+- Added a method to `WeightedDirectedGraph` to add a new node. 
+- Added a method to `WeightedDirectedGraph` to add a new edge. This can be doned given the desire weight, given a path between the nodes to connect and use the product of the weights or just let the graph find a path between nodes and use the product of the weights.
```

### Comparing `pywgraph-1.0.0.post1/README.md` & `pywgraph-1.0.1/pywgraph.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: pywgraph
+Version: 1.0.1
+Summary: A python implementation of weighted directed graphs where weights can be elements of a mathematical group
+Home-page: https://github.com/josek98/pywgraph
+Author: josek98
+Author-email: josemmsscc98@gmail.com
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Requires-Dist: pytest>=7.0; extra == "dev"
+Requires-Dist: twine>=4.0.2; extra == "dev"
+
 # pywgraph
 A library to manipulate weighted graphs in python. This library focus on directed graphs whose edges have weights. The weights of the graph can be any elements of a fixed mathematical group. By default, the underlying group is set to be the real numbers with the multiplication. Thus, when trasversing the graph, the weight of the path is the product of the weights of the edges, but in general, it is the product under the binary operation of the group. 
 
 For this reason, this package also includes a basic abstraction of a group. The group definition is base on:
 *  The a function of two variables that return one element (the binary operation of the group).
 *  The inverse function of an element. This is, the function that given an element of the group returns it inverse. 
 *  The identity element of the group.
@@ -243,7 +256,14 @@
 # None
 
 graph.weight_between("A", "Z", np.array([1,1]))
 # np.array([1,1])
 ```
 
 Notice that this graph is not conmutative since the weight of the path `["A", "C"]` is different from the weight of the path `["A", "B", "C]`.
+
+## Release Notes
+
+### Version 1.0.1 (2024-05-07)
+
+- Added a method to `WeightedDirectedGraph` to add a new node. 
+- Added a method to `WeightedDirectedGraph` to add a new edge. This can be doned given the desire weight, given a path between the nodes to connect and use the product of the weights or just let the graph find a path between nodes and use the product of the weights.
```

### Comparing `pywgraph-1.0.0.post1/pywgraph/_edge.py` & `pywgraph-1.0.1/pywgraph/_edge.py`

 * *Files identical despite different names*

### Comparing `pywgraph-1.0.0.post1/pywgraph/_groups.py` & `pywgraph-1.0.1/pywgraph/_groups.py`

 * *Files identical despite different names*

### Comparing `pywgraph-1.0.0.post1/pywgraph/_utils.py` & `pywgraph-1.0.1/pywgraph/_utils.py`

 * *Files identical despite different names*

### Comparing `pywgraph-1.0.0.post1/pywgraph.egg-info/PKG-INFO` & `pywgraph-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: pywgraph
-Version: 1.0.0.post1
-Summary: A python implementation of weighted directed graphs where weights can be elements of a mathematical group
-Author: josek98
-Author-email: josemmsscc98@gmail.com
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Requires-Dist: pytest>=7.0; extra == "dev"
-Requires-Dist: twine>=4.0.2; extra == "dev"
-
 # pywgraph
 A library to manipulate weighted graphs in python. This library focus on directed graphs whose edges have weights. The weights of the graph can be any elements of a fixed mathematical group. By default, the underlying group is set to be the real numbers with the multiplication. Thus, when trasversing the graph, the weight of the path is the product of the weights of the edges, but in general, it is the product under the binary operation of the group. 
 
 For this reason, this package also includes a basic abstraction of a group. The group definition is base on:
 *  The a function of two variables that return one element (the binary operation of the group).
 *  The inverse function of an element. This is, the function that given an element of the group returns it inverse. 
 *  The identity element of the group.
@@ -255,7 +243,14 @@
 # None
 
 graph.weight_between("A", "Z", np.array([1,1]))
 # np.array([1,1])
 ```
 
 Notice that this graph is not conmutative since the weight of the path `["A", "C"]` is different from the weight of the path `["A", "B", "C]`.
+
+## Release Notes
+
+### Version 1.0.1 (2024-05-07)
+
+- Added a method to `WeightedDirectedGraph` to add a new node. 
+- Added a method to `WeightedDirectedGraph` to add a new edge. This can be doned given the desire weight, given a path between the nodes to connect and use the product of the weights or just let the graph find a path between nodes and use the product of the weights.
```

### Comparing `pywgraph-1.0.0.post1/tests/test_directed_edge.py` & `pywgraph-1.0.1/tests/test_directed_edge.py`

 * *Files identical despite different names*

### Comparing `pywgraph-1.0.0.post1/tests/test_path_finding.py` & `pywgraph-1.0.1/tests/test_path_finding.py`

 * *Files identical despite different names*

### Comparing `pywgraph-1.0.0.post1/tests/test_weighted_directed_edge.py` & `pywgraph-1.0.1/tests/test_weighted_directed_edge.py`

 * *Files identical despite different names*

### Comparing `pywgraph-1.0.0.post1/tests/test_weighted_directed_graph_arrays.py` & `pywgraph-1.0.1/tests/test_weighted_directed_graph_arrays.py`

 * *Files identical despite different names*

