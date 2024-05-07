# Comparing `tmp/fabrics-0.9.1.tar.gz` & `tmp/fabrics-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrics-0.9.1.tar", max compression
+gzip compressed data, was "fabrics-0.9.4.tar", max compression
```

## Comparing `fabrics-0.9.1.tar` & `fabrics-0.9.4.tar`

### file list

```diff
@@ -1,34 +1,38 @@
--rw-r--r--   0        0        0    35306 2024-04-01 00:42:59.157119 fabrics-0.9.1/LICENSE
--rw-r--r--   0        0        0     4831 2024-04-01 00:42:59.157119 fabrics-0.9.1/README.md
--rw-r--r--   0        0        0       40 2024-04-01 00:42:59.301118 fabrics-0.9.1/fabrics/.gitignore
--rw-r--r--   0        0        0       71 2024-04-01 00:42:59.301118 fabrics-0.9.1/fabrics/__init__.py
--rw-r--r--   0        0        0      249 2024-04-01 00:42:59.301118 fabrics-0.9.1/fabrics/components/energies/execution_energies.py
--rw-r--r--   0        0        0     3048 2024-04-01 00:42:59.301118 fabrics-0.9.1/fabrics/components/leaves/attractor.py
--rw-r--r--   0        0        0     2453 2024-04-01 00:42:59.301118 fabrics-0.9.1/fabrics/components/leaves/dynamic_attractor.py
--rw-r--r--   0        0        0     4354 2024-04-01 00:42:59.301118 fabrics-0.9.1/fabrics/components/leaves/dynamic_geometry.py
--rw-r--r--   0        0        0     2915 2024-04-01 00:42:59.301118 fabrics-0.9.1/fabrics/components/leaves/dynamic_leaf.py
--rw-r--r--   0        0        0    16364 2024-04-01 00:42:59.301118 fabrics-0.9.1/fabrics/components/leaves/geometry.py
--rw-r--r--   0        0        0     2733 2024-04-01 00:42:59.301118 fabrics-0.9.1/fabrics/components/leaves/leaf.py
--rw-r--r--   0        0        0     2807 2024-04-01 00:42:59.301118 fabrics-0.9.1/fabrics/components/maps/parameterized_maps.py
--rw-r--r--   0        0        0     1319 2024-04-01 00:42:59.305118 fabrics-0.9.1/fabrics/defaults/default_energies.py
--rw-r--r--   0        0        0     1609 2024-04-01 00:42:59.305118 fabrics-0.9.1/fabrics/defaults/default_geometries.py
--rw-r--r--   0        0        0      918 2024-04-01 00:42:59.305118 fabrics-0.9.1/fabrics/defaults/default_leaves.py
--rw-r--r--   0        0        0     1852 2024-04-01 00:42:59.305118 fabrics-0.9.1/fabrics/defaults/default_maps.py
--rw-r--r--   0        0        0      260 2024-04-01 00:42:59.305118 fabrics-0.9.1/fabrics/diffGeometry/casadi_helpers.py
--rw-r--r--   0        0        0     3605 2024-04-01 00:42:59.305118 fabrics-0.9.1/fabrics/diffGeometry/diffMap.py
--rw-r--r--   0        0        0     4016 2024-04-01 00:42:59.305118 fabrics-0.9.1/fabrics/diffGeometry/energized_geometry.py
--rw-r--r--   0        0        0     7189 2024-04-01 00:42:59.305118 fabrics-0.9.1/fabrics/diffGeometry/energy.py
--rw-r--r--   0        0        0     3364 2024-04-01 00:42:59.305118 fabrics-0.9.1/fabrics/diffGeometry/geometry.py
--rw-r--r--   0        0        0     6934 2024-04-01 00:42:59.305118 fabrics-0.9.1/fabrics/diffGeometry/spec.py
--rw-r--r--   0        0        0     2818 2024-04-01 00:42:59.305118 fabrics-0.9.1/fabrics/diffGeometry/speedControl.py
--rw-r--r--   0        0        0     6969 2024-04-01 00:42:59.305118 fabrics-0.9.1/fabrics/helpers/casadiFunctionWrapper.py
--rw-r--r--   0        0        0       75 2024-04-01 00:42:59.305118 fabrics-0.9.1/fabrics/helpers/constants.py
--rw-r--r--   0        0        0     8725 2024-04-01 00:42:59.305118 fabrics-0.9.1/fabrics/helpers/distances.py
--rw-r--r--   0        0        0      273 2024-04-01 00:42:59.305118 fabrics-0.9.1/fabrics/helpers/exceptions.py
--rw-r--r--   0        0        0     2688 2024-04-01 00:42:59.305118 fabrics-0.9.1/fabrics/helpers/functions.py
--rw-r--r--   0        0        0     3940 2024-04-01 00:42:59.305118 fabrics-0.9.1/fabrics/helpers/variables.py
--rw-r--r--   0        0        0     6252 2024-04-01 00:42:59.305118 fabrics-0.9.1/fabrics/planner/non_holonomic_parameterized_planner.py
--rw-r--r--   0        0        0    29924 2024-04-01 00:42:59.305118 fabrics-0.9.1/fabrics/planner/parameterized_planner.py
--rw-r--r--   0        0        0     1548 2024-04-01 00:42:59.305118 fabrics-0.9.1/fabrics/planner/serialized_planner.py
--rw-r--r--   0        0        0     1171 2024-04-01 00:43:24.920940 fabrics-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     5919 1970-01-01 00:00:00.000000 fabrics-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    35306 2024-05-07 15:03:43.357805 fabrics-0.9.4/LICENSE
+-rw-r--r--   0        0        0     4831 2024-05-07 15:03:43.357805 fabrics-0.9.4/README.md
+-rw-r--r--   0        0        0       40 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/.gitignore
+-rw-r--r--   0        0        0       71 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/__init__.py
+-rw-r--r--   0        0        0      249 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/components/energies/execution_energies.py
+-rw-r--r--   0        0        0     2720 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/components/environment/__init__.py
+-rw-r--r--   0        0        0     3048 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/components/leaves/attractor.py
+-rw-r--r--   0        0        0     2453 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/components/leaves/dynamic_attractor.py
+-rw-r--r--   0        0        0     4354 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/components/leaves/dynamic_geometry.py
+-rw-r--r--   0        0        0     2915 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/components/leaves/dynamic_leaf.py
+-rw-r--r--   0        0        0    16601 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/components/leaves/geometry.py
+-rw-r--r--   0        0        0     2733 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/components/leaves/leaf.py
+-rw-r--r--   0        0        0     2807 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/components/maps/parameterized_maps.py
+-rw-r--r--   0        0        0     2372 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/components/robot_representation/__init__.py
+-rw-r--r--   0        0        0     1319 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/defaults/default_energies.py
+-rw-r--r--   0        0        0     1609 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/defaults/default_geometries.py
+-rw-r--r--   0        0        0      918 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/defaults/default_leaves.py
+-rw-r--r--   0        0        0     1852 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/defaults/default_maps.py
+-rw-r--r--   0        0        0      260 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/diffGeometry/casadi_helpers.py
+-rw-r--r--   0        0        0     3587 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/diffGeometry/diffMap.py
+-rw-r--r--   0        0        0     4007 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/diffGeometry/energized_geometry.py
+-rw-r--r--   0        0        0     7171 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/diffGeometry/energy.py
+-rw-r--r--   0        0        0     3355 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/diffGeometry/geometry.py
+-rw-r--r--   0        0        0     6925 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/diffGeometry/spec.py
+-rw-r--r--   0        0        0     2818 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/diffGeometry/speedControl.py
+-rw-r--r--   0        0        0     7267 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/helpers/casadiFunctionWrapper.py
+-rw-r--r--   0        0        0       75 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/helpers/constants.py
+-rw-r--r--   0        0        0     9331 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/helpers/distances.py
+-rw-r--r--   0        0        0      273 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/helpers/exceptions.py
+-rw-r--r--   0        0        0     2688 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/helpers/functions.py
+-rw-r--r--   0        0        0     7697 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/helpers/geometric_primitives.py
+-rw-r--r--   0        0        0     4857 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/helpers/variables.py
+-rw-r--r--   0        0        0     4099 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/planner/configuration_classes.py
+-rw-r--r--   0        0        0     6225 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/planner/non_holonomic_parameterized_planner.py
+-rw-r--r--   0        0        0    34405 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/planner/parameterized_planner.py
+-rw-r--r--   0        0        0     1548 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/planner/serialized_planner.py
+-rw-r--r--   0        0        0     1183 2024-05-07 15:03:43.505804 fabrics-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     5921 1970-01-01 00:00:00.000000 fabrics-0.9.4/PKG-INFO
```

### Comparing `fabrics-0.9.1/LICENSE` & `fabrics-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.1/README.md` & `fabrics-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.1/fabrics/components/leaves/attractor.py` & `fabrics-0.9.4/fabrics/components/leaves/attractor.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.1/fabrics/components/leaves/dynamic_attractor.py` & `fabrics-0.9.4/fabrics/components/leaves/dynamic_attractor.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.1/fabrics/components/leaves/dynamic_geometry.py` & `fabrics-0.9.4/fabrics/components/leaves/dynamic_geometry.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.1/fabrics/components/leaves/dynamic_leaf.py` & `fabrics-0.9.4/fabrics/components/leaves/dynamic_leaf.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.1/fabrics/components/leaves/geometry.py` & `fabrics-0.9.4/fabrics/components/leaves/geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,24 @@
         """
         x = self._x
         xdot = self._xdot
         new_parameters, lagrangian_geometry = parse_symbolic_input(finsler_structure, x, xdot, name=self._leaf_name)
         self._parent_variables.add_parameters(new_parameters)
         self._lag = Lagrangian(lagrangian_geometry, var=self._leaf_variables)
 
+class AvoidanceLeaf(GenericGeometryLeaf):
+    def _init__(
+            self, 
+            parent_variables: Variables,
+            name: str,
+            phi: ca.SX,
+            ):
+        super().__init__(parent_variables, name, phi)
+
+
 class LimitLeaf(GenericGeometryLeaf):
     """
     The LimitLeaf is geometry leaf for joint limits.
 
     This leaf is not parameterized as the joint limits remain static for one robot.
     """
     def __init__(
```

### Comparing `fabrics-0.9.1/fabrics/components/leaves/leaf.py` & `fabrics-0.9.4/fabrics/components/leaves/leaf.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.1/fabrics/components/maps/parameterized_maps.py` & `fabrics-0.9.4/fabrics/components/maps/parameterized_maps.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.1/fabrics/defaults/default_energies.py` & `fabrics-0.9.4/fabrics/defaults/default_energies.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.1/fabrics/defaults/default_geometries.py` & `fabrics-0.9.4/fabrics/defaults/default_geometries.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.1/fabrics/defaults/default_leaves.py` & `fabrics-0.9.4/fabrics/defaults/default_leaves.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.1/fabrics/defaults/default_maps.py` & `fabrics-0.9.4/fabrics/defaults/default_maps.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.1/fabrics/diffGeometry/diffMap.py` & `fabrics-0.9.4/fabrics/diffGeometry/diffMap.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         return ca.mtimes(self._Jdot, self.qdot())
 
     def phidot(self) -> ca.SX:
         return ca.mtimes(self._J, self.qdot())
 
     def concretize(self) -> None:
         self._funs = CasadiFunctionWrapper(
-            "funs", self._vars.asDict(), {"phi": self._phi, "J": self._J, "Jdot": self._Jdot}
+            "funs", self._vars, {"phi": self._phi, "J": self._J, "Jdot": self._Jdot}
         )
 
     def params(self) -> dict:
         return self._vars.parameters()
 
     def state_variables(self) -> dict:
         return self._vars.state_variables()
@@ -80,15 +80,15 @@
         return [self._x_ref_name, self._xdot_ref_name, self._xddot_ref_name]
 
     def phidot(self) -> ca.SX:
         return self._phi_dot
 
     def concretize(self) -> None:
         self._funs = CasadiFunctionWrapper(
-            "funs", self._vars.asDict(), {"x_rel": self._phi, "xdot_rel": self._phi_dot}
+            "funs", self._vars, {"x_rel": self._phi, "xdot_rel": self._phi_dot}
         )
 
     def forward(self, **kwargs):
         evaluations = self._funs.evaluate(**kwargs)
         x = evaluations['x_rel']
         xdot = evaluations['xdot_rel']
         return x, xdot
```

### Comparing `fabrics-0.9.1/fabrics/diffGeometry/energized_geometry.py` & `fabrics-0.9.4/fabrics/diffGeometry/energized_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
             var += refTraj._vars
         """
         self._funs = ca.Function(
             "M", var, [self.M(), self.f(), self._xddot, self._alpha]
         )
         """
         self._funs = CasadiFunctionWrapper(
-                "funs", var.asDict(), {"M": self.M(), 'f': self.f(), 'xddot': self._xddot, 'alpha': self._alpha}
+                "funs", var, {"M": self.M(), 'f': self.f(), 'xddot': self._xddot, 'alpha': self._alpha}
         )
 
     def evaluate(self, **kwargs):
         evaluations = self._funs.evaluate(**kwargs)
         M = evaluations['M']
         f = evaluations['f']
         xddot = evaluations['xddot']
```

### Comparing `fabrics-0.9.1/fabrics/diffGeometry/energy.py` & `fabrics-0.9.4/fabrics/diffGeometry/energy.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
     def concretize(self):
         self._S.concretize()
         var = deepcopy(self._vars)
         for refTraj in self._refTrajs:
             var += refTraj._vars
         self._funs = CasadiFunctionWrapper(
-            "funs", var.asDict(), {"H": self._H}
+            "funs", var, {"H": self._H}
         )
 
     def ref_names(self) -> list:
         return [self._x_ref_name, self._xdot_ref_name, self._xddot_ref_name]
 
 
     def evaluate(self, **kwargs):
@@ -179,14 +179,14 @@
         self._lg = lg
         l = 0.5 * lg ** 2
         super().__init__(l, **kwargs)
 
     def concretize(self):
         super().concretize()
         self._funs_lg = CasadiFunctionWrapper(
-            "funs", self._vars.asDict(), {"Lg": self._lg}
+            "funs", self._vars, {"Lg": self._lg}
         )
 
     def evaluate(self, **kwargs):
         M, f, l = super().evaluate(**kwargs)
         lg = self._funs_lg.evaluate(**kwargs)['Lg']
         return M, f, l, lg
```

### Comparing `fabrics-0.9.1/fabrics/diffGeometry/geometry.py` & `fabrics-0.9.4/fabrics/diffGeometry/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
     def concretize(self):
         self._xddot = -self._h
         var = deepcopy(self._vars)
         for refTraj in self._refTrajs:
             var += refTraj._vars
         self._funs = CasadiFunctionWrapper(
-            "funs", var.asDict(), {"h": self._h, "xddot": self._xddot}
+            "funs", var, {"h": self._h, "xddot": self._xddot}
         )
 
     def evaluate(self, **kwargs):
         evaluations = self._funs.evaluate(**kwargs)
         h_eval = evaluations['h']
         xddot_eval = evaluations['xddot']
         return [h_eval, xddot_eval]
```

### Comparing `fabrics-0.9.1/fabrics/diffGeometry/spec.py` & `fabrics-0.9.4/fabrics/diffGeometry/spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
     def concretize(self):
         self._xddot = -self.h()
         var = deepcopy(self._vars)
         for refTraj in self._refTrajs:
             var += refTraj._vars
         self._funs = CasadiFunctionWrapper(
-            "funs", var.asDict(), {"M": self.M(), "f": self.f(), "xddot": self._xddot}
+            "funs", var, {"M": self.M(), "f": self.f(), "xddot": self._xddot}
         )
 
     def evaluate(self, **kwargs):
         evaluations = self._funs.evaluate(**kwargs)
         M_eval = evaluations["M"]
         if len(M_eval.shape) == 1:
             M_eval = np.array([M_eval])
```

### Comparing `fabrics-0.9.1/fabrics/diffGeometry/speedControl.py` & `fabrics-0.9.4/fabrics/diffGeometry/speedControl.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.1/fabrics/helpers/casadiFunctionWrapper.py` & `fabrics-0.9.4/fabrics/helpers/casadiFunctionWrapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import pdb
 import casadi as ca
+from fabrics.helpers.variables import Variables
 import numpy as np
 import os
 import pickle
 import _pickle as cPickle
 import bz2
 import logging
 
 
 class InputMissmatchError(Exception):
     pass
 
 
 class CasadiFunctionWrapper(object):
 
-    def __init__(self, name: str, inputs: dict, expressions: dict):
+    def __init__(self, name: str, variables: Variables, expressions: dict):
         self._name = name
-        self._inputs = inputs
+        self._inputs = variables.asDict()
         self._expressions = expressions
+        self._argument_dictionary = variables.parameters_values()
         self.create_function()
 
     def create_function(self):
         self._input_keys = sorted(tuple(self._inputs.keys()))
         self._input_sizes = {i: self._inputs[i].size() for i in self._inputs}
         self._list_expressions = [self._expressions[i] for i in sorted(self._expressions.keys())]
         input_expressions = [self._inputs[i] for i in self._input_keys]
@@ -31,80 +33,80 @@
         return self._function
 
     def serialize(self, file_name):
         with bz2.BZ2File(file_name, 'w') as f:
             pickle.dump(self._function.serialize(), f)
             pickle.dump(list(self._expressions.keys()), f)
             pickle.dump(self._input_keys, f)
+            pickle.dump(self._argument_dictionary, f)
 
     def evaluate(self, **kwargs):
-        argument_dictionary = {}
         for key in kwargs: # pragma no cover
             if key == 'x_obst' or key == 'x_obsts':
                 obstacle_dictionary = {}
                 for j, x_obst_j in enumerate(kwargs[key]):
                     obstacle_dictionary[f'x_obst_{j}'] = x_obst_j
-                argument_dictionary.update(obstacle_dictionary)
+                self._argument_dictionary.update(obstacle_dictionary)
             if key == 'radius_obst' or key == 'radius_obsts':
                 radius_dictionary = {}
                 for j, radius_obst_j in enumerate(kwargs[key]):
                     radius_dictionary[f'radius_obst_{j}'] = radius_obst_j
-                argument_dictionary.update(radius_dictionary)
+                self._argument_dictionary.update(radius_dictionary)
             if key == 'x_obst_dynamic' or key == 'x_obsts_dynamic':
                 obstacle_dyn_dictionary = {}
                 for j, x_obst_dyn_j in enumerate(kwargs[key]):
                     obstacle_dyn_dictionary[f'x_obst_dynamic_{j}'] = x_obst_dyn_j
-                argument_dictionary.update(obstacle_dyn_dictionary)
+                self._argument_dictionary.update(obstacle_dyn_dictionary)
             if key == 'xdot_obst_dynamic' or key == 'xdot_obsts_dynamic':
                 xdot_dyn_dictionary = {}
                 for j, xdot_obst_dyn_j in enumerate(kwargs[key]):
                     xdot_dyn_dictionary[f'xdot_obst_dynamic_{j}'] = xdot_obst_dyn_j
-                argument_dictionary.update(xdot_dyn_dictionary)
+                self._argument_dictionary.update(xdot_dyn_dictionary)
             if key == 'xddot_obst_dynamic' or key == 'xddot_obsts_dynamic':
                 xddot_dyn_dictionary = {}
                 for j, xddot_obst_dyn_j in enumerate(kwargs[key]):
                     xddot_dyn_dictionary[f'xddot_obst_dynamic_{j}'] = xddot_obst_dyn_j
-                argument_dictionary.update(xddot_dyn_dictionary)
+                self._argument_dictionary.update(xddot_dyn_dictionary)
             if key == 'radius_obst_dynamic' or key == 'radius_obsts_dynamic':
                 radius_dyn_dictionary = {}
                 for j, radius_obst_dyn_j in enumerate(kwargs[key]):
                     radius_dyn_dictionary[f'radius_obst_dynamic_{j}'] = radius_obst_dyn_j
-                argument_dictionary.update(radius_dyn_dictionary)
+                self._argument_dictionary.update(radius_dyn_dictionary)
             if key == 'x_obst_cuboid' or key == 'x_obsts_cuboid':
                 x_obst_cuboid_dictionary = {}
                 for j, x_obst_cuboid_j in enumerate(kwargs[key]):
                     x_obst_cuboid_dictionary[f'x_obst_cuboid_{j}'] = x_obst_cuboid_j
-                argument_dictionary.update(x_obst_cuboid_dictionary)
+                self._argument_dictionary.update(x_obst_cuboid_dictionary)
             if key == 'size_obst_cuboid' or key == 'size_obsts_cuboid':
                 size_obst_cuboid_dictionary = {}
                 for j, size_obst_cuboid_j in enumerate(kwargs[key]):
                     size_obst_cuboid_dictionary[f'size_obst_cuboid_{j}'] = size_obst_cuboid_j
-                argument_dictionary.update(size_obst_cuboid_dictionary)
+                self._argument_dictionary.update(size_obst_cuboid_dictionary)
             if key.startswith('radius_body') and key.endswith('links'):
                 # Radius bodies can be passed using a dictionary where the keys are simple integers.
                 radius_body_dictionary = {}
                 body_size_inputs = [input_exp for input_exp in self._input_keys if input_exp.startswith('radius_body')]
                 for link_nr, radius_body_j in kwargs[key].items():
                     try:
                         key = [body_size_input for body_size_input in body_size_inputs if str(link_nr) in body_size_input][0]
                     except IndexError as e:
                         logging.warning(f"No body link with index {link_nr} in the inputs. Body link {link_nr} is ignored.")
                     radius_body_dictionary[key] = radius_body_j
-                argument_dictionary.update(radius_body_dictionary)
+                self._argument_dictionary.update(radius_body_dictionary)
             else:
-                argument_dictionary[key] = kwargs[key]
+                self._argument_dictionary[key] = kwargs[key]
         input_arrays = []
         try:
             for i in self._input_keys:
                 """
-                if not argument_dictionary[i].size == self._input_sizes[i][0] * self._input_sizes[i][1]:
-                    raise InputMissmatchError(f"Size of input argument {i} with size {argument_dictionary[i].size} does not match size required {self._input_sizes[i][0]}")
+                if not self._argument_dictionary[i].size == self._input_sizes[i][0] * self._input_sizes[i][1]:
+                    raise InputMissmatchError(f"Size of input argument {i} with size {self._argument_dictionary[i].size} does not match size required {self._input_sizes[i][0]}")
                 """
-                input_arrays.append(argument_dictionary[i])
-            input_arrays = [argument_dictionary[i] for i in self._input_keys]
+                input_arrays.append(self._argument_dictionary[i])
+            input_arrays = [self._argument_dictionary[i] for i in self._input_keys]
         except KeyError as e:
             msg = f"Key {e} is not contained in the inputs\n"
             msg += f"Possible keys are {self._input_keys}\n"
             msg += f"You provided {list(kwargs.keys())}\n"
             raise InputMissmatchError(msg)
         try:
             list_array_outputs = self._function(*input_arrays)
@@ -129,13 +131,14 @@
     def __init__(self, file_name: str):
         if os.path.isfile(file_name):
             logging.info(f"Initializing casadiFunctionWrapper from {file_name}")
             data = bz2.BZ2File(file_name, 'rb')
             self._function = ca.Function().deserialize(cPickle.load(data))
             expression_keys = cPickle.load(data)
             self._input_keys = cPickle.load(data)
+            self._argument_dictionary = cPickle.load(data)
             self._expressions = {}
             for key in expression_keys:
                 self._expressions[key] = []
             self._isload = True
```

### Comparing `fabrics-0.9.1/fabrics/helpers/distances.py` & `fabrics-0.9.4/fabrics/helpers/distances.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,29 @@
     t = ca.dot(point_vector, line_vector) / ca.dot(line_vector, line_vector)
     t = ca.fmax(0, ca.fmin(1, t))
     return line_start + t * line_vector
 
 def clamp(a: ca.SX, a_min: float, a_max: float):
     return ca.fmin(a_max, ca.fmax(a, a_min))
 
+def point_to_point(point_1: ca.SX, point_2: ca.SX) -> ca.SX:
+    return ca.norm_2(point_1 - point_2)
+
+def sphere_to_point(sphere_center: ca.SX,
+                    point: ca.SX,
+                    sphere_radius: ca.SX) -> ca.SX:
+    return point_to_point(sphere_center, point) - sphere_radius
+
+def sphere_to_sphere(sphere_1_center: ca.SX,
+                     sphere_2_center: ca.SX,
+                     sphere_1_radius: ca.SX,
+                     sphere_2_radius: ca.SX) -> ca.SX:
+    distance = point_to_point(sphere_1_center, sphere_2_center)
+    return distance - sphere_1_radius - sphere_2_radius
+
 def point_to_line(point: ca.SX, line_start: ca.SX, line_end: ca.SX) -> ca.SX:
     line_vec = line_end - line_start
     point_vec = point - line_start
     proj_length = ca.dot(point_vec, line_vec) / ca.norm_2(line_vec)
     distance_0 = ca.norm_2(point - line_start)
     distance_1 = ca.norm_2(point - line_end)
     proj_point = line_start + proj_length * line_vec / ca.norm_2(line_vec)
```

### Comparing `fabrics-0.9.1/fabrics/helpers/functions.py` & `fabrics-0.9.4/fabrics/helpers/functions.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.1/fabrics/helpers/variables.py` & `fabrics-0.9.4/fabrics/helpers/variables.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,59 @@
+from typing import Union
 import casadi as ca
+import numpy as np
 from copy import deepcopy
 
 class ParameterNotFoundError(Exception):
     pass
 
 
 class Variables(object):
-    def __init__(self, state_variables=None, parameters=None):
+    def __init__(self, state_variables=None, parameters=None, parameters_values=None):
         if state_variables is None:
             state_variables = {}
         if parameters is None:
             parameters = {}
+        if parameters_values is None:
+            parameters_values = {}
         self._state_variables = state_variables
         self._parameters = parameters
+        self._parameters_values = parameters_values
         if len(state_variables) > 0:
             self._state_variable_names = list(state_variables.keys())
         if len(parameters) > 0:
             self._parameter_names = list(parameters.keys())
 
     def state_variables(self):
         return self._state_variables
 
     def add_state_variable(self, name, value):
         self._state_variables[name] = value
 
     def parameters(self) -> dict:
         return self._parameters
 
+    def parameters_values(self) -> dict:
+        return self._parameters_values
+
     def add_parameter(self, name: str, value: ca.SX) -> None:
         self._parameters[name] = value
 
+    def add_parameter_value(self, name: str, value: Union[float, np.ndarray]) -> None:
+        if name not in self._parameters:
+            raise ParameterNotFoundError(f"Parameter {name} not in parameters")
+        self._parameters_values[name] = value
+
     def add_parameters(self, parameter_dict: dict) -> None:
         self._parameters.update(parameter_dict)
 
+    def add_parameters_values(self, parameter_dict: dict) -> None:
+        for parameter_name, parameter_value in parameter_dict.items():
+            self.add_parameter_value(parameter_name, parameter_value)
+
     def set_parameters(self, parameters):
         self._parameters = parameters
 
     def variable_by_name(self, name: str) -> ca.SX:
         return self._state_variables[name]
 
     def parameter_by_name(self, name: str) -> ca.SX:
@@ -90,16 +107,20 @@
                     counter = 1
                     while new_key in joined_parameters.keys():
                         new_key = key + "_" + str(counter)
                         counter += 1
                     joined_parameters[new_key] = value
             else:
                 joined_parameters[key] = value
-
-        return Variables(state_variables=joined_state_variables, parameters=joined_parameters)
+        joined_parameters_values = {**self.parameters_values(), **b.parameters_values()}
+        return Variables(
+            state_variables=joined_state_variables,
+            parameters=joined_parameters,
+            parameters_values=joined_parameters_values,
+        )
 
     def len(self):
         return len(self._parameters.values()) + len(
             self._state_variables.values()
         )
 
     def __repr__(self):
```

### Comparing `fabrics-0.9.1/fabrics/planner/non_holonomic_parameterized_planner.py` & `fabrics-0.9.4/fabrics/planner/non_holonomic_parameterized_planner.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         M_base[3:q.size()[0],3:q.size()[0]] = M_arm_energy
         base_energy = 0.5 * ca.dot(qdot, ca.mtimes(M_base, qdot))
         base_geometry = Geometry(h=ca.SX(np.zeros(self._dof)), var=self.variables)
         base_lagrangian = Lagrangian(base_energy, var=self._variables)
         self._geometry = WeightedGeometry(g=base_geometry, le=base_lagrangian)
 
     def extra_terms_function(self):
-        extra_terms_functions = CasadiFunctionWrapper("extra_terms", self._variables.asDict(), {"J_nh": self._J_nh, "f_extra": self._f_extra})
+        extra_terms_functions = CasadiFunctionWrapper("extra_terms", self._variables, {"J_nh": self._J_nh, "f_extra": self._f_extra})
         return extra_terms_functions
 
     def concretize(self, mode='acc', time_step=None):
         if mode == 'vel':
             if not time_step:
                 raise Exception("No time step passed in velocity mode.")
         eps = 1e-6
@@ -125,14 +125,14 @@
             logging.info("No forcing term, using pure geoemtry")
             raise AttributeError(e)
             logging.error(e)
             self._geometry.concretize()
             xddot = self._geometry._xddot - self._geometry._alpha * self._geometry._vars.velocity_variable()
         if mode == 'acc':
             self._funs = CasadiFunctionWrapper(
-                "funs", self.variables.asDict(), {"action": xddot}
+                "funs", self.variables, {"action": xddot}
             )
         elif mode == 'vel':
             action = self._qudot + time_step * xddot
             self._funs = CasadiFunctionWrapper(
-                "funs", self.variables.asDict(), {"action": action}
+                "funs", self.variables, {"action": action}
             )
```

### Comparing `fabrics-0.9.1/fabrics/planner/parameterized_planner.py` & `fabrics-0.9.4/fabrics/planner/parameterized_planner.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,52 @@
-from dataclasses import dataclass, field
-import deprecation
-from typing import Dict, Optional, List
 import logging
-import casadi as ca
-from forwardkinematics.fksCommon.fk import ForwardKinematics
-from forwardkinematics.urdfFks.urdfFk import LinkNotInURDFError
-import numpy as np
 from copy import deepcopy
-from fabrics.helpers.exceptions import ExpressionSparseError
-from fabrics import __version__
-
-from fabrics.helpers.variables import Variables
-from fabrics.helpers.constants import eps
-from fabrics.helpers.functions import is_sparse, parse_symbolic_input
+from typing import Dict, List, Optional
 
-from fabrics.diffGeometry.diffMap import DifferentialMap, DynamicDifferentialMap
-from fabrics.diffGeometry.energy import Lagrangian
-from fabrics.diffGeometry.geometry import Geometry
-from fabrics.diffGeometry.energized_geometry import WeightedGeometry
-from fabrics.diffGeometry.speedControl import Damper
+import casadi as ca
+import deprecation
+import numpy as np
 
-from fabrics.helpers.casadiFunctionWrapper import CasadiFunctionWrapper
+from forwardkinematics.fksCommon.fk import ForwardKinematics
+from forwardkinematics.urdfFks.urdfFk import LinkNotInURDFError
+from mpscenes.goals.goal_composition import GoalComposition
+from mpscenes.goals.sub_goal import SubGoal
+from pyquaternion import Quaternion
 
+from fabrics import __version__
 from fabrics.components.energies.execution_energies import ExecutionLagrangian
-from fabrics.components.leaves.leaf import Leaf
 from fabrics.components.leaves.attractor import GenericAttractor
 from fabrics.components.leaves.dynamic_attractor import GenericDynamicAttractor
-from fabrics.components.leaves.dynamic_geometry import DynamicObstacleLeaf, GenericDynamicGeometryLeaf
-from fabrics.components.leaves.geometry import (CapsuleSphereLeaf,
-                                                ObstacleLeaf, LimitLeaf,
+from fabrics.components.leaves.dynamic_geometry import (
+    DynamicObstacleLeaf, GenericDynamicGeometryLeaf)
+from fabrics.components.leaves.geometry import (AvoidanceLeaf,
+                                                CapsuleCuboidLeaf,
+                                                CapsuleSphereLeaf,
+                                                ESDFGeometryLeaf,
+                                                GenericGeometryLeaf, LimitLeaf,
+                                                ObstacleLeaf,
                                                 PlaneConstraintGeometryLeaf,
                                                 SelfCollisionLeaf,
-                                                GenericGeometryLeaf,
-                                                ESDFGeometryLeaf,
-                                                SphereCuboidLeaf,
-                                                CapsuleCuboidLeaf)
-from mpscenes.goals.goal_composition import GoalComposition
-from mpscenes.goals.sub_goal import SubGoal
-
-from forwardkinematics.fksCommon.fk_creator import FkCreator
-from forwardkinematics.urdfFks.generic_urdf_fk import GenericURDFFk
+                                                SphereCuboidLeaf)
+from fabrics.components.leaves.leaf import Leaf
+from fabrics.diffGeometry.diffMap import (DifferentialMap,
+                                          DynamicDifferentialMap)
+from fabrics.diffGeometry.energized_geometry import WeightedGeometry
+from fabrics.diffGeometry.energy import Lagrangian
+from fabrics.diffGeometry.geometry import Geometry
+from fabrics.diffGeometry.speedControl import Damper
+from fabrics.helpers.casadiFunctionWrapper import CasadiFunctionWrapper
+from fabrics.helpers.constants import eps
+from fabrics.helpers.exceptions import ExpressionSparseError
+from fabrics.helpers.functions import is_sparse, parse_symbolic_input
+from fabrics.helpers.geometric_primitives import Sphere
+from fabrics.helpers.variables import Variables
+from fabrics.planner.configuration_classes import (FabricPlannerConfig,
+                                                   ProblemConfiguration)
 
-from pyquaternion import Quaternion
 
 class InvalidRotationAnglesError(Exception):
     pass
 
 class LeafNotFoundError(Exception):
     pass
 
@@ -62,79 +63,38 @@
         return quaternion.rotation_matrix
     elif isinstance(angles, ca.SX):
         return angles
     else:
         raise(InvalidRotationAnglesError)
 
 
-
-@dataclass
-class FabricPlannerConfig:
-    base_energy: str = (
-        "0.5 * 0.2 * ca.dot(xdot, xdot)"
-    )
-    collision_geometry: str = (
-        "-0.5 / (x ** 5) * (-0.5 * (ca.sign(xdot) - 1)) * xdot ** 2"
-    )
-    collision_finsler: str = (
-        "0.1/(x**1) * xdot**2"
-    )
-    limit_geometry: str = (
-        "-0.1 / (x ** 1) * xdot ** 2"
-    )
-    limit_finsler: str = (
-        "0.1/(x**1) * (-0.5 * (ca.sign(xdot) - 1)) * xdot**2"
-    )
-    self_collision_geometry: str = (
-        "-0.5 / (x ** 1) * (-0.5 * (ca.sign(xdot) - 1)) * xdot ** 2"
-    )
-    self_collision_finsler: str = (
-        "0.1/(x**1) * xdot**2"
-    )
-    geometry_plane_constraint: str = (
-        "-0.5 / (x ** 5) * (-0.5 * (ca.sign(xdot) - 1)) * xdot ** 2"
-    )
-    finsler_plane_constraint: str = (
-        "0.1/(x**1) * xdot**2"
-    )
-    attractor_potential: str = (
-        "5.0 * (ca.norm_2(x) + 1 / 10 * ca.log(1 + ca.exp(-2 * 10 * ca.norm_2(x))))"
-    )
-    attractor_metric: str = (
-        "((2.0 - 0.3) * ca.exp(-1 * (0.75 * ca.norm_2(x))**2) + 0.3) * ca.SX(np.identity(x.size()[0]))"
-    )
-    damper_beta: str = (
-        "0.5 * (ca.tanh(-0.5 * (ca.norm_2(x) - 0.02)) + 1) * 6.5 + 0.01 + ca.fmax(0, sym('a_ex') - sym('a_le'))"
-    )
-    damper_eta: str = (
-        "0.5 * (ca.tanh(-0.9 * (1 - 1/2) * ca.dot(xdot, xdot) - 0.5) + 1)"
-    )
-    """
-    damper_beta: str = (
-        "0.5 * (ca.tanh(-sym('alpha_b') * (ca.norm_2(x) - sym('radius_shift'))) + 1) * sym('beta_close') + sym('beta_distant') + ca.fmax(0, sym('a_ex') - sym('a_le'))"
-    )
-    damper_eta: str = (
-        "0.5 * (ca.tanh(-sym('alpha_eta') * sym('ex_lag') * (1 - sym('ex_factor')) - 0.5) + 1)"
-    )
-    """
+class ParameterizedFabricPlanner(object):
+    
+    _dof: int
+    _config: FabricPlannerConfig
+    _problem_configuration : ProblemConfiguration
+    leaves: Dict[str, Leaf]
+    _ref_sign: int
 
 
-class ParameterizedFabricPlanner(object):
     def __init__(self, dof: int, forward_kinematics: ForwardKinematics, **kwargs):
         self._dof = dof
         self._config = FabricPlannerConfig(**kwargs)
         self._forward_kinematics = forward_kinematics
         self.initialize_joint_variables()
         self.set_base_geometry()
         self._target_velocity = np.zeros(self._geometry.x().size()[0])
         self._ref_sign = 1
         self.leaves = {}
 
     """ INITIALIZING """
 
+    def load_fabrics_configuration(self, fabrics_configuration: dict):
+        self._config = FabricPlannerConfig(**fabrics_configuration)
+
     def initialize_joint_variables(self):
         q = ca.SX.sym("q", self._dof)
         qdot = ca.SX.sym("qdot", self._dof)
         self._variables = Variables(state_variables={"q": q, "qdot": qdot})
 
     def set_base_geometry(self):
         q = self._variables.position_variable()
@@ -229,14 +189,16 @@
         self._forced_geometry += WeightedGeometry(
             g=geometry, le=lagrangian
         ).pull(forward_map)
         if prime_forcing_leaf:
             self._forced_variables = geometry._vars
             self._forced_forward_map = forward_map
         self._variables = self._variables + self._forced_geometry._vars
+        self._geometry.concretize()
+        self._forced_geometry.concretize(ref_sign=self._ref_sign)
 
     def add_dynamic_forcing_geometry(
         self,
         forward_map: DifferentialMap,
         dynamic_map: DifferentialMap,
         lagrangian: Lagrangian,
         geometry: Geometry,
@@ -256,14 +218,16 @@
         self._forced_geometry += ppwg
         if prime_forcing_leaf:
             self._forced_variables = geometry._vars
             self._forced_forward_map = forward_map
         self._variables = self._variables + self._forced_geometry._vars
         self._target_velocity += ca.mtimes(ca.transpose(forward_map._J), target_velocity)
         self._ref_sign = -1
+        self._geometry.concretize()
+        self._forced_geometry.concretize(ref_sign=self._ref_sign)
 
     def set_execution_energy(self, execution_lagrangian: Lagrangian):
         assert isinstance(execution_lagrangian, Lagrangian)
         composed_geometry = Geometry(s=self._geometry)
         self._execution_lagrangian = execution_lagrangian
         self._execution_geometry = WeightedGeometry(
             g=composed_geometry, le=execution_lagrangian
@@ -275,41 +239,31 @@
                 g=forced_geometry, le=execution_lagrangian
             )
             self._forced_speed_controlled_geometry.concretize()
         except AttributeError:
             logging.warning("No damping")
 
     def set_speed_control(self):
-        self._geometry.concretize()
-        self._forced_geometry.concretize(ref_sign=self._ref_sign)
         x_psi = self._forced_variables.position_variable()
         dm_psi = self._forced_forward_map
         exLag = self._execution_lagrangian
         a_ex = ca.SX.sym("a_ex", 1)
         a_le = ca.SX.sym("a_le", 1)
         beta_expression = self.config.damper_beta
         eta_expression = self.config.damper_eta
         self._damper = Damper(beta_expression, eta_expression, x_psi, dm_psi, exLag._l)
         self._variables.add_parameters(self._damper.symbolic_parameters())
 
-    def get_forward_kinematics(self, link_name) -> ca.SX:
+    def get_forward_kinematics(self, link_name, position_only: bool = True) -> ca.SX:
         if isinstance(link_name, ca.SX):
             return link_name
-        if isinstance(self._forward_kinematics, GenericURDFFk):
-            fk = self._forward_kinematics.fk(
-                self._variables.position_variable(),
-                self._forward_kinematics._rootLink,
-                link_name,
-                positionOnly=True
-            )
-        else:
-            fk = self._forward_kinematics.fk(
+        fk = self._forward_kinematics.casadi(
                 self._variables.position_variable(),
                 link_name,
-                positionOnly=True
+                position_only=position_only
             )
         return fk
 
     def add_capsule_sphere_geometry(
             self,
             obstacle_name: str,
             capsule_name: str,
@@ -501,14 +455,110 @@
         lower_limit_geometry.set_finsler_structure(self.config.limit_finsler)
         upper_limit_geometry = LimitLeaf(self._variables, joint_index, limits[1], 1)
         upper_limit_geometry.set_geometry(self.config.limit_geometry)
         upper_limit_geometry.set_finsler_structure(self.config.limit_finsler)
         self.add_leaf(lower_limit_geometry)
         self.add_leaf(upper_limit_geometry)
 
+    def load_problem_configuration(self, problem_configuration: ProblemConfiguration):
+        self._problem_configuration = ProblemConfiguration(**problem_configuration)
+        for obstacle in self._problem_configuration.environment.obstacles:
+            self._variables.add_parameters(obstacle.sym_parameters)
+
+        self.set_collision_avoidance()
+        #self.set_self_collision_avoidance()
+        self.set_joint_limits()
+        if self._config.forcing_type in ['forced', 'speed-controlled', 'forced-energized']:
+            self.set_goal_component(self._problem_configuration.goal_composition)
+        if self._config.forcing_type in ['speed-controlled', 'execution-energy', 'forced-energized']:
+            execution_energy = ExecutionLagrangian(self._variables)
+            self.set_execution_energy(execution_energy)
+        if self._config.forcing_type in ['speed-controlled']:
+            self.set_speed_control()
+
+    def set_joint_limits(self):
+        limits = np.zeros((self._dof, 2))
+        limits[:, 0] = self._problem_configuration.joint_limits.lower_limits
+        limits[:, 1] = self._problem_configuration.joint_limits.upper_limits
+        limits = limits.tolist()
+        for joint_index in range(len(limits)):
+            self.add_limit_geometry(joint_index, limits[joint_index])
+
+    def set_self_collision_avoidance(self) -> None:
+        if not self._problem_configuration.robot_representation.self_collision_pairs:
+            return
+        for link_name,  paired_links_names in self._problem_configuration.robot_representation.self_collision_pairs.items():
+            link = self._problem_configuration.robot_representation.collision_links[link_name]
+            for paired_link_name in paired_links_names:
+                paired_link = self._problem_configuration.robot_representation.collision_links[paired_link_name]
+                if isinstance(link, Sphere) and isinstance(paired_link, Sphere):
+                    self.add_spherical_self_collision_geometry(
+                            paired_link_name,
+                            link_name,
+                    )
+
+
+    def set_collision_avoidance(self) -> None:
+        if not self._problem_configuration.robot_representation.collision_links:
+            return
+        for link_name, collision_link in self._problem_configuration.robot_representation.collision_links.items():
+            fk = self.get_forward_kinematics(link_name, position_only=False)
+            if fk.shape == (3, 3):
+                fk_augmented = ca.SX.eye(4)
+                fk_augmented[0:2, 0:2] = fk[0:2, 0:2]
+                fk_augmented[0:2, 3] = fk[0:2, 2]
+                fk = fk_augmented
+            if fk.shape == (4, 4) and is_sparse(fk[0:3, 3]):
+                message = (
+                        f"Expression {fk[0:3, 3]} for link {link_name} "
+                        "is sparse and thus skipped."
+                )
+                logging.warning(message.format_map(locals()))
+                continue
+            elif fk.shape != (4, 4) and is_sparse(fk):
+                message = (
+                        f"Expression {fk} for link {link_name} "
+                        "is sparse and thus skipped."
+                )
+                logging.warning(message.format_map(locals()))
+                continue
+            collision_link.set_origin(fk)
+            self._variables.add_parameters(collision_link.sym_parameters)
+            self._variables.add_parameters_values(collision_link.parameters)
+            for obstacle in self._problem_configuration.environment.obstacles:
+                distance = collision_link.distance(obstacle)
+                leaf_name = f"{link_name}_{obstacle.name}_leaf"
+                leaf = AvoidanceLeaf(self._variables, leaf_name, distance)
+                leaf.set_geometry(self.config.collision_geometry)
+                leaf.set_finsler_structure(self.config.collision_finsler)
+                self.add_leaf(leaf)
+            """
+            for i in range(self._problem_configuration.environment.number_spheres['dynamic']):
+                obstacle_name = f"obst_dynamic_{i}"
+                if isinstance(collision_link, Sphere):
+                    self.add_dynamic_spherical_obstacle_geometry(
+                            obstacle_name,
+                            link_name,
+                            fk,
+                            reference_parameter_list[i],
+                            dynamic_obstacle_dimension=dynamic_obstacle_dimension,
+                    )
+            for i in range(self._problem_configuration.environment.number_planes):
+                constraint_name = f"constraint_{i}"
+                if isinstance(collision_link, Sphere):
+                    self.add_plane_constraint(constraint_name, link_name, fk)
+
+            for i in range(self._problem_configuration.environment.number_cuboids['static']):
+                obstacle_name = f"obst_cuboid_{i}"
+                if isinstance(collision_link, Sphere):
+                    self.add_cuboid_obstacle_geometry(obstacle_name, link_name, fk)
+            """
+
+
+
 
     def set_components(
         self,
         collision_links: Optional[list] = None,
         self_collision_pairs: Optional[dict] = None,
         collision_links_esdf: Optional[list] = None,
         goal: Optional[GoalComposition] = None,
@@ -640,40 +690,50 @@
 
 
     def concretize(self, mode='acc', time_step=None):
         self._mode = mode
         if mode == 'vel':
             if not time_step:
                 raise Exception("No time step passed in velocity mode.")
-        try:
+        self._geometry.concretize()
+        if self._config.forcing_type in ['speed-controlled']:
             eta = self._damper.substitute_eta()
             a_ex = (
                 eta * self._execution_geometry._alpha
                 + (1 - eta) * self._forced_speed_controlled_geometry._alpha
             )
             beta_subst = self._damper.substitute_beta(-a_ex, -self._geometry._alpha)
             xddot = self._forced_geometry._xddot - (a_ex + beta_subst) * (
                 self._geometry.xdot()
                 - ca.mtimes(self._forced_geometry.Minv(), self._target_velocity)
             )
             #xddot = self._forced_geometry._xddot
-        except AttributeError:
+        elif self._config.forcing_type == 'execution-energy':
             logging.warn("No forcing term, using pure geoemtry with energization.")
-            self._geometry.concretize()
             #xddot = self._geometry._xddot - self._geometry._alpha * self._geometry._vars.velocity_variable()
             xddot = self._execution_geometry._xddot - self._execution_geometry._alpha * self._geometry._vars.velocity_variable()
+        elif self._config.forcing_type == 'forced-energized':
+            logging.warn("Using forced geoemtry with constant execution energy.")
+            xddot = self._forced_speed_controlled_geometry._xddot - self._forced_speed_controlled_geometry._alpha * self._geometry._vars.velocity_variable()
+        elif self._config.forcing_type == 'forced':
+            logging.warn("No execution energy, using forced geomtry without speed regulation.")
+            xddot = self._forced_geometry._xddot - self._geometry._alpha * self._geometry._vars.velocity_variable()
+        elif self._config.forcing_type == 'pure-geometry':
+            xddot = self._geometry._xddot
+        else:
+            raise Exception(f"Unknown forcing type {self._config.forcing_type}.")
 
         if mode == 'acc':
             self._funs = CasadiFunctionWrapper(
-                "funs", self.variables.asDict(), {"action": xddot}
+                "funs", self.variables, {"action": xddot}
             )
         elif mode == 'vel':
             action = self._geometry.xdot() + time_step * xddot
             self._funs = CasadiFunctionWrapper(
-                "funs", self.variables.asDict(), {"action": action}
+                "funs", self.variables, {"action": action}
             )
             
 
     def serialize(self, file_name: str):
         """
         Serializes the fabric planner.
```

### Comparing `fabrics-0.9.1/fabrics/planner/serialized_planner.py` & `fabrics-0.9.4/fabrics/planner/serialized_planner.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.1/pyproject.toml` & `fabrics-0.9.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fabrics"
-version = "0.9.1"
+version = "0.9.4"
 description = "Optimization fabrics in python."
 authors = ["Max Spahn <m.spahn@tudelft.nl>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 repository = "https://tud-amr/fabrics"
 keywords = ["robotics", "motion-planning", "geometry"]
 
@@ -17,24 +17,25 @@
 pickle-mixin = "^1.0.2"
 quaternionic = "^1.0.0"
 mpscenes = "^0.4"
 pynput = "^1.7.6"
 vector = "^1.1.1"
 pytest = "6.2.5"
 deprecation = "^2.1.0"
-forwardkinematics = ">=1.1.4,<1.2"
+forwardkinematics = "^1.2.2"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.13.4"
 pytest = "^6.2.5"
 pytest-cov = "^4.0.0"
 black = "^23.9.1"
+isort = "^5.13.2"
 
 [tool.poetry.group.tutorials]
 optional = true
 
 [tool.poetry.group.tutorials.dependencies]
 planarenvs = "^1.4"
 matplotlib = "^3.7.0"
```

### Comparing `fabrics-0.9.1/PKG-INFO` & `fabrics-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: fabrics
-Version: 0.9.1
+Version: 0.9.4
 Summary: Optimization fabrics in python.
 Home-page: https://tud-amr/fabrics
 License: GPL-3.0-or-later
 Keywords: robotics,motion-planning,geometry
 Author: Max Spahn
 Author-email: m.spahn@tudelft.nl
 Requires-Python: >=3.8,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: casadi (>=3.5.5)
 Requires-Dist: deprecation (>=2.1.0,<3.0.0)
-Requires-Dist: forwardkinematics (>=1.1.4,<1.2)
+Requires-Dist: forwardkinematics (>=1.2.2,<2.0.0)
 Requires-Dist: geomdl (>=5.3.1,<6.0.0)
 Requires-Dist: mpscenes (>=0.4,<0.5)
 Requires-Dist: numpy (>=1.15.3,<2.0.0)
 Requires-Dist: pickle-mixin (>=1.0.2,<2.0.0)
 Requires-Dist: pynput (>=1.7.6,<2.0.0)
 Requires-Dist: pyquaternion (>=0.9.9,<0.10.0)
 Requires-Dist: pytest (==6.2.5)
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: fabrics Version: 0.9.1 Summary: Optimization
+Metadata-Version: 2.1 Name: fabrics Version: 0.9.4 Summary: Optimization
 fabrics in python. Home-page: https://tud-amr/fabrics License: GPL-3.0-or-later
 Keywords: robotics,motion-planning,geometry Author: Max Spahn Author-email:
 m.spahn@tudelft.nl Requires-Python: >=3.8,<3.10 Classifier: License :: OSI
 Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Requires-Dist: casadi
 (>=3.5.5) Requires-Dist: deprecation (>=2.1.0,<3.0.0) Requires-Dist:
-forwardkinematics (>=1.1.4,<1.2) Requires-Dist: geomdl (>=5.3.1,<6.0.0)
+forwardkinematics (>=1.2.2,<2.0.0) Requires-Dist: geomdl (>=5.3.1,<6.0.0)
 Requires-Dist: mpscenes (>=0.4,<0.5) Requires-Dist: numpy (>=1.15.3,<2.0.0)
 Requires-Dist: pickle-mixin (>=1.0.2,<2.0.0) Requires-Dist: pynput
 (>=1.7.6,<2.0.0) Requires-Dist: pyquaternion (>=0.9.9,<0.10.0) Requires-Dist:
 pytest (==6.2.5) Requires-Dist: quaternionic (>=1.0.0,<2.0.0) Requires-Dist:
 vector (>=1.1.1,<2.0.0) Project-URL: Repository, https://tud-amr/fabrics
 Description-Content-Type: text/markdown # (Geometric) Fabrics [![Build and
 Agents](https://github.com/maxspahn/fabrics/actions/workflows/
```

