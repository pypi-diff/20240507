# Comparing `tmp/p1afempy-0.2.4.tar.gz` & `tmp/p1afempy-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p1afempy-0.2.4.tar", last modified: Wed Mar 20 15:43:06 2024, max compression
+gzip compressed data, was "p1afempy-0.2.6.tar", last modified: Tue May  7 07:23:20 2024, max compression
```

## Comparing `p1afempy-0.2.4.tar` & `p1afempy-0.2.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 rleu       (501) staff       (20)        0 2024-03-20 15:43:06.088174 p1afempy-0.2.4/
--rw-r--r--   0 rleu       (501) staff       (20)     1050 2024-02-07 10:49:44.000000 p1afempy-0.2.4/LICENSE
--rw-r--r--   0 rleu       (501) staff       (20)    13112 2024-03-20 15:43:06.087503 p1afempy-0.2.4/PKG-INFO
--rw-r--r--   0 rleu       (501) staff       (20)    12523 2024-02-08 07:40:01.000000 p1afempy-0.2.4/README.md
-drwxr-xr-x   0 rleu       (501) staff       (20)        0 2024-03-20 15:43:06.084401 p1afempy-0.2.4/p1afempy/
--rw-r--r--   0 rleu       (501) staff       (20)      218 2024-01-25 07:07:34.000000 p1afempy-0.2.4/p1afempy/__init__.py
--rw-r--r--   0 rleu       (501) staff       (20)     1669 2024-01-25 08:04:57.000000 p1afempy-0.2.4/p1afempy/data_structures.py
--rw-r--r--   0 rleu       (501) staff       (20)     3228 2024-01-25 09:15:00.000000 p1afempy-0.2.4/p1afempy/indicators.py
--rw-r--r--   0 rleu       (501) staff       (20)     4087 2024-02-07 10:49:44.000000 p1afempy-0.2.4/p1afempy/io_helpers.py
--rw-r--r--   0 rleu       (501) staff       (20)    12374 2024-03-20 15:42:54.000000 p1afempy-0.2.4/p1afempy/mesh.py
--rw-r--r--   0 rleu       (501) staff       (20)    18651 2024-02-07 16:49:02.000000 p1afempy-0.2.4/p1afempy/refinement.py
--rw-r--r--   0 rleu       (501) staff       (20)     7063 2024-01-25 09:16:30.000000 p1afempy-0.2.4/p1afempy/solvers.py
-drwxr-xr-x   0 rleu       (501) staff       (20)        0 2024-03-20 15:43:06.086926 p1afempy-0.2.4/p1afempy.egg-info/
--rw-r--r--   0 rleu       (501) staff       (20)    13112 2024-03-20 15:43:06.000000 p1afempy-0.2.4/p1afempy.egg-info/PKG-INFO
--rw-r--r--   0 rleu       (501) staff       (20)      346 2024-03-20 15:43:06.000000 p1afempy-0.2.4/p1afempy.egg-info/SOURCES.txt
--rw-r--r--   0 rleu       (501) staff       (20)        1 2024-03-20 15:43:06.000000 p1afempy-0.2.4/p1afempy.egg-info/dependency_links.txt
--rw-r--r--   0 rleu       (501) staff       (20)       31 2024-03-20 15:43:06.000000 p1afempy-0.2.4/p1afempy.egg-info/requires.txt
--rw-r--r--   0 rleu       (501) staff       (20)       63 2024-03-20 15:43:06.000000 p1afempy-0.2.4/p1afempy.egg-info/top_level.txt
--rw-r--r--   0 rleu       (501) staff       (20)      766 2024-03-20 15:42:54.000000 p1afempy-0.2.4/pyproject.toml
--rw-r--r--   0 rleu       (501) staff       (20)       38 2024-03-20 15:43:06.088330 p1afempy-0.2.4/setup.cfg
+drwxr-xr-x   0 rleu       (501) staff       (20)        0 2024-05-07 07:23:20.872155 p1afempy-0.2.6/
+-rw-r--r--   0 rleu       (501) staff       (20)     1050 2024-02-07 10:49:44.000000 p1afempy-0.2.6/LICENSE
+-rw-r--r--   0 rleu       (501) staff       (20)    13143 2024-05-07 07:23:20.871662 p1afempy-0.2.6/PKG-INFO
+-rw-r--r--   0 rleu       (501) staff       (20)    12523 2024-02-08 07:40:01.000000 p1afempy-0.2.6/README.md
+drwxr-xr-x   0 rleu       (501) staff       (20)        0 2024-05-07 07:23:20.868534 p1afempy-0.2.6/p1afempy/
+-rw-r--r--   0 rleu       (501) staff       (20)      218 2024-04-24 14:13:30.000000 p1afempy-0.2.6/p1afempy/__init__.py
+-rw-r--r--   0 rleu       (501) staff       (20)     1669 2024-01-25 08:04:57.000000 p1afempy-0.2.6/p1afempy/data_structures.py
+-rw-r--r--   0 rleu       (501) staff       (20)     3228 2024-01-25 09:15:00.000000 p1afempy-0.2.6/p1afempy/indicators.py
+-rw-r--r--   0 rleu       (501) staff       (20)     4311 2024-04-26 08:30:58.000000 p1afempy-0.2.6/p1afempy/io_helpers.py
+-rw-r--r--   0 rleu       (501) staff       (20)    16993 2024-04-26 08:30:58.000000 p1afempy-0.2.6/p1afempy/mesh.py
+-rw-r--r--   0 rleu       (501) staff       (20)    28731 2024-04-26 08:30:58.000000 p1afempy-0.2.6/p1afempy/refinement.py
+-rw-r--r--   0 rleu       (501) staff       (20)     7063 2024-01-25 09:16:30.000000 p1afempy-0.2.6/p1afempy/solvers.py
+drwxr-xr-x   0 rleu       (501) staff       (20)        0 2024-05-07 07:23:20.871168 p1afempy-0.2.6/p1afempy.egg-info/
+-rw-r--r--   0 rleu       (501) staff       (20)    13143 2024-05-07 07:23:20.000000 p1afempy-0.2.6/p1afempy.egg-info/PKG-INFO
+-rw-r--r--   0 rleu       (501) staff       (20)      346 2024-05-07 07:23:20.000000 p1afempy-0.2.6/p1afempy.egg-info/SOURCES.txt
+-rw-r--r--   0 rleu       (501) staff       (20)        1 2024-05-07 07:23:20.000000 p1afempy-0.2.6/p1afempy.egg-info/dependency_links.txt
+-rw-r--r--   0 rleu       (501) staff       (20)       47 2024-05-07 07:23:20.000000 p1afempy-0.2.6/p1afempy.egg-info/requires.txt
+-rw-r--r--   0 rleu       (501) staff       (20)       57 2024-05-07 07:23:20.000000 p1afempy-0.2.6/p1afempy.egg-info/top_level.txt
+-rw-r--r--   0 rleu       (501) staff       (20)      787 2024-05-07 07:14:34.000000 p1afempy-0.2.6/pyproject.toml
+-rw-r--r--   0 rleu       (501) staff       (20)       38 2024-05-07 07:23:20.872240 p1afempy-0.2.6/setup.cfg
```

### Comparing `p1afempy-0.2.4/LICENSE` & `p1afempy-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `p1afempy-0.2.4/PKG-INFO` & `p1afempy-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: p1afempy
-Version: 0.2.4
+Version: 0.2.6
 Summary: Adaptive P1 FEM algorithms
 Author-email: Raphael Leu <raphaelleu95@gmail.com>
 Project-URL: Homepage, https://github.com/leuraph/p1afempy
 Project-URL: Issues, https://github.com/leuraph/p1afempy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.18
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pathlib
 Requires-Dist: matplotlib
+Requires-Dist: ismember>=1.0.4
 
 # P1AFEM-PY
 
 This package is the pythonic adaption of the p1afem Matlab package,
 whose code can be found
 [here (ZIP)](https://www.tuwien.at/index.php?eID=dumpFile&t=f&f=180536&token=1b5f89369acab20d59455e42569bf1e0b2db8b41)
 and whose details are described in the paper (open access) [[1]](#1).
```

### Comparing `p1afempy-0.2.4/README.md` & `p1afempy-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `p1afempy-0.2.4/p1afempy/data_structures.py` & `p1afempy-0.2.6/p1afempy/data_structures.py`

 * *Files identical despite different names*

### Comparing `p1afempy-0.2.4/p1afempy/indicators.py` & `p1afempy-0.2.6/p1afempy/indicators.py`

 * *Files identical despite different names*

### Comparing `p1afempy-0.2.4/p1afempy/io_helpers.py` & `p1afempy-0.2.6/p1afempy/io_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,18 @@
     -------
     >>> file_path = Path("path/to/boundary_data.dat")
     >>> boundary_condition = read_boundary_condition(file_path)
     """
     boundary_indices = np.loadtxt(path_to_boundary).astype(np.uint32)
     if shift_indices:
         boundary_indices = boundary_indices - 1
+    # make sure we match the expected shape even if (in an edge case)
+    # the specified boundary condition is only valid on one single edge
+    if len(boundary_indices.shape) == 1:
+        return boundary_indices[None, :]
     return boundary_indices
 
 
 def read_coordinates(path_to_coordinates: Path) -> np.ndarray:
     """
     reads and returns vertices from file
```

### Comparing `p1afempy-0.2.4/p1afempy/mesh.py` & `p1afempy-0.2.6/p1afempy/mesh.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 from p1afempy import data_structures
+from ismember import ismember, is_row_in
 from scipy.sparse import coo_matrix, find
 from matplotlib import pyplot as plt
 
 
 def get_area(coordinates: data_structures.CoordinatesType,
              elements: data_structures.ElementsType) -> np.ndarray:
     """
@@ -137,24 +138,26 @@
     return element_to_edges, edge_to_nodes, boundaries_to_edges
 
 
 def get_global_to_local_index_mapping(unique_idxs: np.ndarray):
     """
     given a set of n unique, non-negative integers I,
     this function returns a vectorized and order preserving mapping
-    `perform_transform` : I -> [0, 1, 2, ..., n-1] =: I'
+    `perform_transform` : I -> [-1, 0, 1, 2, ..., n-1] =: I'
 
     notes
     -----
     - the returned mapping may be used, e.g. to transform global indexation
       to local indexation after extraction of a local patch
     - if global[i, j, ...] <= global[i', j', ...], then we also have
       local[i, j, ...]  <= local[i', j', ...]
     - if N is the number of distinct indices in global_indices,
       then local_indices contains the integers 0, 1, ..., N-1
+    - values of -1 get mapped to -1 as they indicate a boundary in
+      element to neighbour mapping arrays
 
     example
     -------
     >>> global_indices = np.array([[12, 3, 6],
     >>>                            [12, 2, 6],
     >>>                            [12, 3, 15],
     >>>                            [66, 77, 88]])
@@ -164,15 +167,17 @@
     >>> local_indices
         array([[3, 1, 2],
                [3, 0, 2],
                [3, 1, 4],
                [5, 6, 7]])
     """
     local_idx = np.arange(unique_idxs.size)
-    transform = dict(zip(unique_idxs, local_idx))
+    transform = dict(zip(
+        np.hstack((unique_idxs, -1)),
+        np.hstack((local_idx, -1))))
     perform_transform = np.vectorize(lambda old: transform[old])
     return perform_transform
 
 
 def complete_boundaries(elements: data_structures.ElementsType,
                         boundaries: list[data_structures.BoundaryType]
                         ) -> list[data_structures.BoundaryType]:
@@ -201,49 +206,99 @@
     >>> completed_boundaries = complete_boundaries(
     >>>     elements, [boundary])
     >>> completed_boundaries
         [array([[0, 1], [1, 2]]), array([[2, 3], [3, 0]])]
     """
     element_indices_i = elements.flatten()
     element_indices_j = elements[:, [1, 2, 0]].flatten()
-    all_edges = np.column_stack([element_indices_i, element_indices_j])
+    all_edges_ij = np.column_stack([element_indices_i, element_indices_j])
 
-    exterior_edges = []
-    for edge in all_edges:
-        # mark all rows where edge appears
-        edge_is_here = np.sum(np.isin(all_edges, edge), axis=1) == 2
-        # if edge appears twice, it is shared by two elements and therefore
-        # must be interior
-        is_interior = np.sum(edge_is_here) == 2
-        if not is_interior:
-            exterior_edges.append(edge)
-
-    artificial_boundary = []
-    for exterior_edge in exterior_edges:
-        covered = False
-        for boundary in boundaries:
-            if np.any(np.sum(np.isin(boundary, exterior_edge), axis=1) == 2):
-                covered = True
-                break
-        if not covered:
-            artificial_boundary.append(exterior_edge)
+    is_interior = is_row_in(all_edges_ij, all_edges_ij[:, [1, 0]])
 
-    if artificial_boundary:
-        boundaries.append(np.array(artificial_boundary))
+    exterior_edges = all_edges_ij[np.logical_not(is_interior)]
+
+    for boundary in boundaries:
+        covered = is_row_in(exterior_edges, boundary)
+        exterior_edges = exterior_edges[np.logical_not(covered)]
+
+    if exterior_edges.size > 0:
+        boundaries.append(exterior_edges)
     return boundaries
 
 
+def get_local_boundaries(boundaries: list[data_structures.BoundaryType],
+                         local_elements: data_structures.ElementsType,
+                         perform_transform: np.vectorize
+                         ) -> list[data_structures.BoundaryType]:
+    nodes_idx_i = local_elements[:, [0, 1, 2]].flatten()
+    nodes_idx_j = local_elements[:, [1, 2, 0]].flatten()
+    local_edges = np.column_stack((nodes_idx_i, nodes_idx_j))
+
+    local_boundaries = []
+    for boundary in boundaries:
+        shared_edges = is_row_in(boundary, local_edges)
+        if np.any(shared_edges):
+            local_boundaries.append(
+                perform_transform(boundary[shared_edges]))
+    return local_boundaries
+
+
+def get_neighbouring_elements(elements: data_structures.ElementsType,
+                              which_for: int,
+                              element_to_neighbours: np.ndarray
+                              ) -> tuple[
+                                data_structures.ElementsType,
+                                np.ndarray]:
+    """
+    identifies and returns neighbouring elements for a marked element
+
+    Parameters
+    ----------
+    elements: data_structures.ElementsType
+        a 2D array-like structure containing all elements.
+    which_for: int
+        index of the marked element for which neighbouring
+        elements are to be found.
+    element_to_neighbours: np.ndarray
+        array mapping each element to its neighbours
+
+    Returns
+    -------
+    local_elements: data_structures.ElementsType
+        a 2D array-like structure containing neighbouring
+        elements along with the marked element
+    local_element_to_neighbours: np.ndarray
+        all rows of `element_to_neighbours` that correspond
+        to an element included in `local_elements`
+    """
+    local_neighbours = element_to_neighbours[which_for]
+    has_neighbour = local_neighbours >= 0
+
+    local_elements = np.vstack([
+        elements[local_neighbours[has_neighbour], :],
+        elements[which_for]])
+
+    local_element_to_neighbours = np.vstack([
+        element_to_neighbours[local_neighbours[has_neighbour], :],
+        element_to_neighbours[which_for]
+    ])
+
+    return local_elements, local_element_to_neighbours
+
+
 def get_local_patch(coordinates: data_structures.CoordinatesType,
                     elements: data_structures.ElementsType,
                     boundaries: list[data_structures.BoundaryType],
                     which_for: int,
-                    global_values: np.ndarray = np.array([])
+                    element_to_neighbours: np.ndarray,
+                    global_values: np.ndarray = np.array([]),
                     ) -> tuple[data_structures.CoordinatesType,
                                data_structures.ElementsType,
-                               list[data_structures.BoundaryType]]:
+                               list[data_structures.BoundaryType],
+                               np.ndarray, np.ndarray, int]:
     """
     returns the local mesh corresponding to the k-th element
     and its immediate neightbours, i.e. elements that share an edge
     with the selected k-th element
 
     parameters
     ----------
@@ -251,14 +306,16 @@
         coordinates of the mesh at hand
     elements: data_structures.ElementsType
         elements of the mesh at hand
     boundaries: list[data_structures.BoundaryType]
         boundaries of the mesh at hand
     which_for: int
         index of the element for which to extract the local patch
+    element_to_neighbours: np.ndarray
+        array mapping elements to their neighbours
     global_values: np.ndarray = np.array([])
         an array of values defined on the global coordinates
 
     returns
     -------
     local_coordinates: data_structures.CoordinatesType
         coordinates of the selected element and its neighbours,
@@ -271,54 +328,113 @@
     local_boundaries: list[data_structures.BoundaryType]
         boundaries of the local patch inherited from
         the given boundaries, i.e. if none of the elements
         in the local patch touch the boundary at hand,
         an empty list is returned
     local_values: np.ndarray
         the global values given on the local coordinates
+    local_element_to_neighbours: np.ndarray
+        array mapping local elements to local neighbours
+    local_which: int
+        the local index of the marked element `which_for`
 
     notes
     -----
     the returned local patch is indexed in a local fashion, i.e.
     - the indices in local_elements refer to the entries in local_coordinates
     - the indices in all elements in local_boundaries refer to entries in
       local_coordinates
     """
-    # global indices of the marked element's nodes
-    nodes = elements[which_for]
-
-    # identifying the marked element's nieghbours
-    neighbours = np.sum(np.isin(elements, nodes), axis=1) == 2
-
-    # global indices of the local patch's elements
-    local_elements = np.vstack([elements[neighbours], nodes])
+    # indices of all elements neighbouring the selected element
+    # (including the index of the selected element)
+    global_elements_idx = np.hstack((
+        element_to_neighbours[which_for],
+        which_for))
+    # remove -1 as index
+    global_elements_idx = global_elements_idx[global_elements_idx != -1]
+    local_elements_idx = np.arange(global_elements_idx.size)
+    transform = dict(zip(
+        np.hstack((global_elements_idx, -1)),
+        np.hstack((local_elements_idx, -1))))
+    global_to_local_element_index_mapping = np.vectorize(
+        lambda old: transform[old])
+
+    local_element_to_neighbours = element_to_neighbours[global_elements_idx, :]
+    exceeding_elements = np.logical_not(np.isin(
+        local_element_to_neighbours, global_elements_idx))
+    local_element_to_neighbours[exceeding_elements] = -1
 
+    local_elements = elements[global_elements_idx, :]
     # unique sorted global indices of all nodes in global patch
     unique_idxs = np.unique(local_elements)
 
     # retreiving the transformation (global -> local indices)
     perform_transform = get_global_to_local_index_mapping(unique_idxs)
 
-    local_boundaries = []
-    for boundary in boundaries:
-        local_boundary = []
-        for edge in boundary:
-            edge_in_local_patch = np.sum(
-                np.isin(local_elements, edge), axis=1) == 2
-            if np.any(edge_in_local_patch):
-                local_boundary.append(edge)
-        if len(local_boundary) > 0:
-            local_boundary = np.array(local_boundary)
-            local_boundaries.append(perform_transform(local_boundary))
+    # retreive the local boundaries
+    local_boundaries = get_local_boundaries(
+        boundaries=boundaries,
+        local_elements=local_elements,
+        perform_transform=perform_transform)
 
     # local patch's elements in local indices
     local_elements = perform_transform(local_elements)
+    # local patch's neighbour map in local indices
+    # note that we map neighbours of the patch as -1,
+    # indicating a local boundary
+    local_element_to_neighbours = global_to_local_element_index_mapping(
+        local_element_to_neighbours)
 
     # local patch's coordinates
     local_coordinates = coordinates[unique_idxs]
 
     # local value extraction, if given
     local_values = np.array([])
     if global_values.size > 0:
         local_values = global_values[unique_idxs]
 
-    return local_coordinates, local_elements, local_boundaries, local_values
+    local_which = global_to_local_element_index_mapping(which_for)
+
+    # TODO return a local which as well
+    # makes code more maintainable in the future,
+    # because then, outside of the function, we do not
+    # need to assume a specific order of anything
+    # (only in the unit tests, of course)
+    return local_coordinates, local_elements, \
+        local_boundaries, local_values, local_element_to_neighbours, \
+        local_which
+
+
+def get_element_to_neighbours(
+        elements: data_structures.ElementsType) -> np.ndarray:
+    """
+    calculates and returns a map element to neighbours
+
+    parameters
+    ----------
+    elements: data_structures.ElementsType
+        all elements at hand
+
+    returns
+    -------
+    element2neighbours: np.ndarray
+        element2neighbours[k] holds the indices of thk-th
+        element's neighbours, where element2neighbours[k, i]
+        corresponds to the index of the element sharing the i-th
+        edge of the k-th element.
+        a value of `-1` resembles a boundary, i.e. an edge without a neighbour
+    """
+    n_elements = elements.shape[0]
+    I = elements.flatten(order='F')
+    J = elements[:, [1, 2, 0]].flatten(order='F')
+    nodes2edge = coo_matrix((np.arange(1, 3*n_elements+1), (I, J)))
+    mask = nodes2edge > 0
+    _, _, idxIJ = find(nodes2edge)
+    aranged_element_indices = np.arange(1, n_elements + 1)
+    tmp = np.hstack((
+        aranged_element_indices,
+        aranged_element_indices,
+        aranged_element_indices))
+    _, _, neighbourIJ = find(mask + mask.multiply(coo_matrix((tmp, (J, I)))))
+    element2neighbours = np.zeros(3 * n_elements, dtype=int)
+    element2neighbours[idxIJ-1] = neighbourIJ - 1
+    return element2neighbours.reshape((n_elements, 3), order='F') - 1
```

### Comparing `p1afempy-0.2.4/p1afempy/refinement.py` & `p1afempy-0.2.6/p1afempy/refinement.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+import ismember
 from p1afempy.mesh import provide_geometric_data
 from p1afempy.data_structures import \
     CoordinatesType, ElementsType, BoundaryType
 
 
 def generate_new_nodes(edge2newNode: np.ndarray,
                        edge2nodes: np.ndarray,
@@ -26,21 +27,268 @@
             to_embed[edge2nodes[edges_with_new_nodes_indices, 0]] +
             to_embed[edge2nodes[edges_with_new_nodes_indices, 1]]) / 2.
         to_embed = np.hstack([to_embed, new_embedded_values])
 
     return np.vstack([coordinates, new_node_coordinates]), to_embed
 
 
-def refineRG(coordinates: CoordinatesType,
-             elements: ElementsType,
-             marked_element: int,
-             boundaries: list[BoundaryType],
-             to_embed: np.ndarray = np.array([])) -> tuple[CoordinatesType,
-                                                           ElementsType,
-                                                           list[BoundaryType]]:
+def refine_boundaries(elements, which,
+                      boundaries, n_nodes,
+                      element_to_neighbours) -> list[BoundaryType]:
+    edges_to_split_bool = element_to_neighbours[which] == -1
+
+    if not np.any(edges_to_split_bool):
+        return boundaries
+
+    # splitting the boundary, where necessary
+    # ---------------------------------------
+    # 3x2 array of all edges of k-th element
+    possible_edges = np.column_stack((
+        elements[which, [0, 1, 2]].flatten(),
+        elements[which, [1, 2, 0]].flatten()))
+    # isolate edges to be split, i.e. edges
+    # of the k-th element lying on the
+    # domain's boundary
+
+    new_boundaries = []
+    for boundary in boundaries:
+        if boundary.size > 0:
+            boundary_to_split_bool, idx = \
+                ismember.ismember(boundary, possible_edges, method='rows')
+            # indices of new nodes to be inserted in the bundary at hand
+            idx_new_nodes = idx + n_nodes
+            boundary = np.vstack([
+                boundary[np.logical_not(boundary_to_split_bool)],
+                np.column_stack([
+                    boundary[boundary_to_split_bool, 0], idx_new_nodes
+                ]),
+                np.column_stack([
+                    idx_new_nodes, boundary[boundary_to_split_bool, 1]
+                ])
+            ])
+        new_boundaries.append(boundary)
+    return new_boundaries
+
+
+def refine_elements(elements,
+                    element_to_neighbours,
+                    which,
+                    n_nodes) -> ElementsType:
+    index_new_node_1 = n_nodes  # indexing starts at zero
+    index_new_node_2 = n_nodes + 1
+    index_new_node_3 = n_nodes + 2
+
+    # building new elements
+    # ---------------------
+    n_elements = elements.shape[0]
+    # element whose first neighbour is `which`
+    green_1 = np.isin(element_to_neighbours[:, 0], which)
+    # element whose second neighbour is `which`
+    green_2 = np.isin(element_to_neighbours[:, 1], which)
+    # element whose third neighbour is `which`
+    green_3 = np.isin(element_to_neighbours[:, 2], which)
+    # marking `which` as being red-refined
+    red = np.zeros(n_elements, dtype=bool)
+    red[which] = True
+    # the rest of the elements is not marked for refinement
+    # TODO check if this can be improved without reduce
+    none = np.logical_not(
+        np.logical_or.reduce((green_1, green_2,
+                              green_3, red)))
+    # retreiving new elements' indices
+    idx = np.ones(n_elements, dtype=int)
+    idx[green_1] = 2
+    idx[green_2] = 2
+    idx[green_3] = 2
+    idx[red] = 4
+    idx = np.hstack([0, np.cumsum(idx)])
+    new_elements = np.zeros((idx[-1], 3), dtype=int)
+    idx = idx[:-1]
+    # generate new elements
+
+    # no refinement
+    new_elements[idx[none]] = elements[none]
+
+    # TODO check if/how we can remove these `np.any`
+    # green refinement (1)
+    if np.any(green_1):
+        # get the indices of the elements to be green (1) refined
+        idx_element_green_1 = np.nonzero(green_1)[0]
+        # get the indices of the corresponding new nodes
+        _, iloc = ismember.ismember(
+            idx_element_green_1, element_to_neighbours[which, :])
+        idx_new_node_green_1 = n_nodes + iloc
+        # creating and adding the green (1) refined element
+        new_elements[
+            np.hstack((idx[green_1], idx[green_1]+1)), :] = np.vstack((
+                np.column_stack([elements[green_1, 0],
+                                idx_new_node_green_1,
+                                elements[green_1, 2]]),
+                np.column_stack([idx_new_node_green_1,
+                                elements[green_1, 1],
+                                elements[green_1, 2]])
+            ))
+
+    # green refinement (2)
+    if np.any(green_2):
+        # get the index of the element to be green (2) refined
+        idx_element_green_2 = np.nonzero(green_2)[0]
+        # get the indices of the corresponding new nodes
+        _, iloc = ismember.ismember(
+            idx_element_green_2, element_to_neighbours[which, :])
+        idx_new_node_green_2 = n_nodes + iloc
+        # creating and adding the green (2) refined element
+        new_elements[
+            np.hstack((idx[green_2], idx[green_2]+1)), :] = np.vstack((
+                np.column_stack([elements[green_2, 1],
+                                idx_new_node_green_2,
+                                elements[green_2, 0]]),
+                np.column_stack([idx_new_node_green_2,
+                                elements[green_2, 2],
+                                elements[green_2, 0]])
+            ))
+
+    # green refinement (3)
+    if np.any(green_3):
+        # get the index of the element to be green (3) refined
+        idx_element_green_3 = np.nonzero(green_3)[0]
+        # get the indices of the corresponding new nodes
+        _, iloc = ismember.ismember(
+            idx_element_green_3, element_to_neighbours[which, :])
+        idx_new_node_green_3 = n_nodes + iloc
+        # creating and adding the green (3) refined element
+        new_elements[
+            np.hstack((idx[green_3], idx[green_3]+1)), :] = np.vstack((
+                np.column_stack([elements[green_3, 2],
+                                idx_new_node_green_3,
+                                elements[green_3, 1]]),
+                np.column_stack([idx_new_node_green_3,
+                                elements[green_3, 0],
+                                elements[green_3, 1]])
+                    ))
+
+    # red refinement
+    new_elements[
+        np.hstack((
+            idx[red], idx[red]+1,
+            idx[red]+2, idx[red]+3)), :] = np.vstack((
+                np.column_stack([elements[red, 0],
+                                 index_new_node_1,
+                                 index_new_node_3]),
+                np.column_stack([index_new_node_1,
+                                 elements[red, 1],
+                                 index_new_node_2]),
+                np.column_stack([index_new_node_3,
+                                 index_new_node_2,
+                                 elements[red, 2]]),
+                np.column_stack([index_new_node_1,
+                                 index_new_node_2,
+                                 index_new_node_3])
+            ))
+
+    return new_elements
+
+
+def refineRG_with_element_to_neighbours(coordinates: CoordinatesType,
+                                        elements: ElementsType,
+                                        which: int,
+                                        boundaries: list[BoundaryType],
+                                        element_to_neighbours,
+                                        to_embed: np.ndarray = np.array([])
+                                        ) -> tuple[CoordinatesType,
+                                                   ElementsType,
+                                                   list[BoundaryType],
+                                                   np.ndarray]:
+    """
+    red refines a single specified element and removes
+    hanging nodes by green refining neighbouring elements
+
+    Parameters
+    ----------
+    coordinates: CoordinatesType
+        coordinates of the mesh at hand
+    elements: ElementsType
+        elements of the mesh at hand
+    which: int
+        index of the element to be red refined
+    boundaries: list[BoundaryType]
+        list of boundaries at hand
+    element_to_neighbours: np.ndarray
+        array whose j-th entry in the i-th row represents the
+        index of the element sharing the i-th edge of the j-th element
+    to_embed: np.ndarray, optional
+        array containing data on the nodes to be linearly interpolated,
+        defaults to an empty array
+
+    Returns
+    -------
+    new_coordinates: CoordinatesType
+        coordinates of the refined mesh
+    new_elements: ElementsType
+        elements of the refined mesh
+    new_boundaries: list[BoundaryType]
+        boundaries of the refined mesh
+    to_embed: np.ndarray
+        linearly interpolated data on the refined mesh
+
+    Notes
+    -----
+    - this routine does not assume the list of boundary
+      conditions to be complete.
+    - during refinement, three new coordinates are generated,
+      these get simply appended to the existing coordinates
+    """
+    # building (three) new coordinates
+    # --------------------------------
+    x_y_1 = coordinates[elements[which, [0, 1, 2]], :]
+    x_y_2 = coordinates[elements[which, [1, 2, 0]], :]
+    new_coordinates = np.vstack([coordinates,
+                                 (x_y_1 + x_y_2)/2.])
+    # retrieving new nodes' indices
+    n_nodes = coordinates.shape[0]
+
+    # interpolating `to_embed`
+    # ------------------------
+    if to_embed.size > 0:
+        interpolated = (to_embed[elements[which, [0, 1, 2]].flatten()] +
+                        to_embed[elements[which, [1, 2, 0]].flatten()])/2.
+        to_embed = np.hstack([to_embed, interpolated])
+
+    new_elements = refine_elements(elements=elements,
+                                   element_to_neighbours=element_to_neighbours,
+                                   which=which,
+                                   n_nodes=n_nodes)
+
+    new_boundaries = refine_boundaries(
+        elements=elements,
+        boundaries=boundaries,
+        n_nodes=n_nodes,
+        which=which,
+        element_to_neighbours=element_to_neighbours)
+
+    return new_coordinates, new_elements, new_boundaries, to_embed
+
+
+# NOTE This function is based on the refinement technology found in [1]
+# and hence, in theory, should be capable of red-green refining more than one
+# element at once, where each marked element is red-refined and hanging
+# nodes removed by green-refinement. However, checking/testing/realizing
+# this implementation remains an open TODO.
+#
+# [1] S. Funken, D. Praetorius, and P. Wissgott.
+#     Efficient Implementation of Adaptive P1-FEM in Matlab
+#     http://dx.doi.org/10.2478/cmam-2011-0026
+def refineRG_without_element_to_neighbours(
+    coordinates: CoordinatesType,
+    elements: ElementsType,
+    marked_element: int,
+    boundaries: list[BoundaryType],
+    to_embed: np.ndarray = np.array([])) -> tuple[CoordinatesType,
+                                                  ElementsType,
+                                                  list[BoundaryType]]:
     """
     refines the mesh according to
     red-green refinement of one single element
 
     parameters
     ----------
     coordinates: CoordinatesType
@@ -61,24 +309,29 @@
     new_boundaries: list[BoundaryType]
         boundaries of the refines mesh
     embedded_values: np.ndarray
         to_embed interpolated onto the refined mesh
 
     notes
     -----
-    this method does the following
-    - given an element k=marked_element marked for
-      refinement
-    - red refine element k
-    - green refine all neighbouring elements (at most three),
-      meaning that the new vertex on the edge shared by k
-      and its neighbour k' gets connected to the vertex
-      in k' opposite to the shared edge
-    - if any new vertex lies on a boundary,
-      refine the boundary accordingly
+    - this function requires to be passed a complete list of
+      boundaries, i.e. each edge of the mesh at hand must be
+      part of a boundary in `boundaries` (due to implementation
+      details in `provide_geometric_data`)
+
+    - this method does the following:
+        1. given an element k=marked_element marked for
+           refinement
+        2. red refine element k
+        3. green refine all neighbouring elements (at most three),
+           meaning that the new vertex on the edge shared by k
+           and its neighbour k' gets connected to the vertex
+           in k' opposite to the shared edge
+        4. if any new vertex lies on a boundary,
+           refine the boundary accordingly
     """
     nE = elements.shape[0]
 
     # Obtain geometric information on edges
     element2edges, edge2nodes, boundary2edges = \
         provide_geometric_data(elements=elements, boundaries=boundaries)
 
@@ -195,15 +448,14 @@
             np.column_stack([newNodes[red, 0],
                              newNodes[red, 1],
                              newNodes[red, 2]])])
 
     return new_coordinates, new_elements, new_boundaries, embedded_values
 
 
-# TODO refactor s.t. boundary_conditions is optional
 def refineRGB(coordinates: CoordinatesType,
               elements: ElementsType,
               marked_elements: np.ndarray,
               boundary_conditions: list[BoundaryType],
               to_embed: np.ndarray = np.array([])
               ) -> tuple[CoordinatesType,
                          ElementsType,
@@ -251,15 +503,14 @@
         boundary_conditions=boundary_conditions,
         sort_for_longest_egde=True,
         to_embed=to_embed)
     return new_coordinates, new_elements, new_boundaries, embedded_values
 
 
 # TODO refactor s.t. sort_for_longest_egde vanishes, this is an ugly solution
-# TODO refactor s.t. boundary_conditions is optional
 def refineNVB(coordinates: CoordinatesType,
               elements: ElementsType,
               marked_elements: np.ndarray,
               boundary_conditions: list[BoundaryType],
               to_embed: np.ndarray = np.array([]),
               sort_for_longest_egde: bool = False
               ) -> tuple[CoordinatesType,
```

### Comparing `p1afempy-0.2.4/p1afempy/solvers.py` & `p1afempy-0.2.6/p1afempy/solvers.py`

 * *Files identical despite different names*

### Comparing `p1afempy-0.2.4/p1afempy.egg-info/PKG-INFO` & `p1afempy-0.2.6/p1afempy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: p1afempy
-Version: 0.2.4
+Version: 0.2.6
 Summary: Adaptive P1 FEM algorithms
 Author-email: Raphael Leu <raphaelleu95@gmail.com>
 Project-URL: Homepage, https://github.com/leuraph/p1afempy
 Project-URL: Issues, https://github.com/leuraph/p1afempy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.18
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pathlib
 Requires-Dist: matplotlib
+Requires-Dist: ismember>=1.0.4
 
 # P1AFEM-PY
 
 This package is the pythonic adaption of the p1afem Matlab package,
 whose code can be found
 [here (ZIP)](https://www.tuwien.at/index.php?eID=dumpFile&t=f&f=180536&token=1b5f89369acab20d59455e42569bf1e0b2db8b41)
 and whose details are described in the paper (open access) [[1]](#1).
```

### Comparing `p1afempy-0.2.4/pyproject.toml` & `p1afempy-0.2.6/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "p1afempy"
-version = "0.2.4"
+version = "0.2.6"
 authors = [
   { name="Raphael Leu", email="raphaelleu95@gmail.com" },
 ]
 description = "Adaptive P1 FEM algorithms"
 readme = "README.md"
 requires-python = ">=3.9.18"
 dependencies = [
   "numpy",
   "scipy",
   "pathlib",
-  "matplotlib"
+  "matplotlib",
+  "ismember>=1.0.4"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

