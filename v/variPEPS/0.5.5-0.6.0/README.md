# Comparing `tmp/varipeps-0.5.5.tar.gz` & `tmp/varipeps-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varipeps-0.5.5.tar", max compression
+gzip compressed data, was "varipeps-0.6.0.tar", max compression
```

## Comparing `varipeps-0.5.5.tar` & `varipeps-0.6.0.tar`

### file list

```diff
@@ -1,45 +1,48 @@
--rw-r--r--   0        0        0    35103 2024-04-23 10:51:24.456170 varipeps-0.5.5/LICENSE
--rw-r--r--   0        0        0     3116 2024-04-23 10:51:24.456170 varipeps-0.5.5/README.md
--rw-r--r--   0        0        0     1157 2024-04-23 10:51:24.468170 varipeps-0.5.5/pyproject.toml
--rw-r--r--   0        0        0      680 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/__init__.py
--rw-r--r--   0        0        0      741 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/__version__.py
--rw-r--r--   0        0        0    11223 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/config.py
--rw-r--r--   0        0        0      100 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/contractions/__init__.py
--rw-r--r--   0        0        0     5553 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/contractions/apply.py
--rw-r--r--   0        0        0    33811 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/contractions/definitions.py
--rw-r--r--   0        0        0      214 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/ctmrg/__init__.py
--rw-r--r--   0        0        0    24093 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/ctmrg/absorption.py
--rw-r--r--   0        0        0    24758 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/ctmrg/projectors.py
--rw-r--r--   0        0        0    22359 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/ctmrg/routine.py
--rw-r--r--   0        0        0      260 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/expectation/__init__.py
--rw-r--r--   0        0        0     1956 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/expectation/model.py
--rw-r--r--   0        0        0     5609 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/expectation/one_site.py
--rw-r--r--   0        0        0     3352 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/expectation/spiral_helpers.py
--rw-r--r--   0        0        0    17657 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/expectation/three_sites.py
--rw-r--r--   0        0        0    19770 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/expectation/two_sites.py
--rw-r--r--   0        0        0     1184 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/global_state.py
--rw-r--r--   0        0        0      191 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/mapping/__init__.py
--rw-r--r--   0        0        0    44983 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/mapping/florett_pentagon.py
--rw-r--r--   0        0        0    22817 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/mapping/honeycomb.py
--rw-r--r--   0        0        0    39648 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/mapping/kagome.py
--rw-r--r--   0        0        0    46761 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/mapping/maple_leaf.py
--rw-r--r--   0        0        0     1288 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/mapping/model.py
--rw-r--r--   0        0        0    59271 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/mapping/square_kagome.py
--rw-r--r--   0        0        0    19197 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/mapping/triangular.py
--rw-r--r--   0        0        0      152 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/optimization/__init__.py
--rw-r--r--   0        0        0     6434 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/optimization/basinhopping.py
--rw-r--r--   0        0        0    10290 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/optimization/inner_function.py
--rw-r--r--   0        0        0    23104 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/optimization/line_search.py
--rw-r--r--   0        0        0    24682 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/optimization/optimizer.py
--rw-r--r--   0        0        0      113 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/peps/__init__.py
--rw-r--r--   0        0        0    35787 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/peps/tensor.py
--rw-r--r--   0        0        0    41065 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/peps/unitcell.py
--rw-r--r--   0        0        0     1086 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/typing.py
--rw-r--r--   0        0        0      119 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/utils/__init__.py
--rw-r--r--   0        0        0     1285 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/utils/debug_print.py
--rw-r--r--   0        0        0      739 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/utils/func_cache.py
--rw-r--r--   0        0        0     2438 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/utils/periodic_indices.py
--rw-r--r--   0        0        0     1657 2024-04-23 10:51:24.472170 varipeps-0.5.5/varipeps/utils/projector_dict.py
--rw-r--r--   0        0        0     5398 2024-04-23 10:51:24.472170 varipeps-0.5.5/varipeps/utils/random.py
--rw-r--r--   0        0        0     3396 2024-04-23 10:51:24.472170 varipeps-0.5.5/varipeps/utils/svd.py
--rw-r--r--   0        0        0     4254 1970-01-01 00:00:00.000000 varipeps-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0    35103 2024-05-07 15:02:43.637911 varipeps-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3116 2024-05-07 15:02:43.637911 varipeps-0.6.0/README.md
+-rw-r--r--   0        0        0     1157 2024-05-07 15:02:43.649911 varipeps-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      680 2024-05-07 15:02:43.649911 varipeps-0.6.0/varipeps/__init__.py
+-rw-r--r--   0        0        0      741 2024-05-07 15:02:43.649911 varipeps-0.6.0/varipeps/__version__.py
+-rw-r--r--   0        0        0    11223 2024-05-07 15:02:43.649911 varipeps-0.6.0/varipeps/config.py
+-rw-r--r--   0        0        0      100 2024-05-07 15:02:43.649911 varipeps-0.6.0/varipeps/contractions/__init__.py
+-rw-r--r--   0        0        0     5553 2024-05-07 15:02:43.649911 varipeps-0.6.0/varipeps/contractions/apply.py
+-rw-r--r--   0        0        0    55583 2024-05-07 15:02:43.649911 varipeps-0.6.0/varipeps/contractions/definitions.py
+-rw-r--r--   0        0        0      366 2024-05-07 15:02:43.649911 varipeps-0.6.0/varipeps/ctmrg/__init__.py
+-rw-r--r--   0        0        0    24093 2024-05-07 15:02:43.649911 varipeps-0.6.0/varipeps/ctmrg/absorption.py
+-rw-r--r--   0        0        0    24758 2024-05-07 15:02:43.649911 varipeps-0.6.0/varipeps/ctmrg/projectors.py
+-rw-r--r--   0        0        0    22359 2024-05-07 15:02:43.649911 varipeps-0.6.0/varipeps/ctmrg/routine.py
+-rw-r--r--   0        0        0    37048 2024-05-07 15:02:43.649911 varipeps-0.6.0/varipeps/ctmrg/structure_factor_absorption.py
+-rw-r--r--   0        0        0    14143 2024-05-07 15:02:43.649911 varipeps-0.6.0/varipeps/ctmrg/structure_factor_routine.py
+-rw-r--r--   0        0        0      291 2024-05-07 15:02:43.649911 varipeps-0.6.0/varipeps/expectation/__init__.py
+-rw-r--r--   0        0        0     1956 2024-05-07 15:02:43.649911 varipeps-0.6.0/varipeps/expectation/model.py
+-rw-r--r--   0        0        0     5609 2024-05-07 15:02:43.649911 varipeps-0.6.0/varipeps/expectation/one_site.py
+-rw-r--r--   0        0        0     3352 2024-05-07 15:02:43.649911 varipeps-0.6.0/varipeps/expectation/spiral_helpers.py
+-rw-r--r--   0        0        0     5751 2024-05-07 15:02:43.649911 varipeps-0.6.0/varipeps/expectation/structure_factor.py
+-rw-r--r--   0        0        0    17657 2024-05-07 15:02:43.649911 varipeps-0.6.0/varipeps/expectation/three_sites.py
+-rw-r--r--   0        0        0    19770 2024-05-07 15:02:43.649911 varipeps-0.6.0/varipeps/expectation/two_sites.py
+-rw-r--r--   0        0        0     1184 2024-05-07 15:02:43.649911 varipeps-0.6.0/varipeps/global_state.py
+-rw-r--r--   0        0        0      191 2024-05-07 15:02:43.649911 varipeps-0.6.0/varipeps/mapping/__init__.py
+-rw-r--r--   0        0        0    44983 2024-05-07 15:02:43.649911 varipeps-0.6.0/varipeps/mapping/florett_pentagon.py
+-rw-r--r--   0        0        0    22817 2024-05-07 15:02:43.649911 varipeps-0.6.0/varipeps/mapping/honeycomb.py
+-rw-r--r--   0        0        0    39648 2024-05-07 15:02:43.653911 varipeps-0.6.0/varipeps/mapping/kagome.py
+-rw-r--r--   0        0        0    46761 2024-05-07 15:02:43.653911 varipeps-0.6.0/varipeps/mapping/maple_leaf.py
+-rw-r--r--   0        0        0     1288 2024-05-07 15:02:43.653911 varipeps-0.6.0/varipeps/mapping/model.py
+-rw-r--r--   0        0        0    59271 2024-05-07 15:02:43.653911 varipeps-0.6.0/varipeps/mapping/square_kagome.py
+-rw-r--r--   0        0        0    19197 2024-05-07 15:02:43.653911 varipeps-0.6.0/varipeps/mapping/triangular.py
+-rw-r--r--   0        0        0      152 2024-05-07 15:02:43.653911 varipeps-0.6.0/varipeps/optimization/__init__.py
+-rw-r--r--   0        0        0     6434 2024-05-07 15:02:43.653911 varipeps-0.6.0/varipeps/optimization/basinhopping.py
+-rw-r--r--   0        0        0    10290 2024-05-07 15:02:43.653911 varipeps-0.6.0/varipeps/optimization/inner_function.py
+-rw-r--r--   0        0        0    23104 2024-05-07 15:02:43.653911 varipeps-0.6.0/varipeps/optimization/line_search.py
+-rw-r--r--   0        0        0    26426 2024-05-07 15:02:43.653911 varipeps-0.6.0/varipeps/optimization/optimizer.py
+-rw-r--r--   0        0        0      143 2024-05-07 15:02:43.653911 varipeps-0.6.0/varipeps/peps/__init__.py
+-rw-r--r--   0        0        0    61833 2024-05-07 15:02:43.653911 varipeps-0.6.0/varipeps/peps/tensor.py
+-rw-r--r--   0        0        0    41065 2024-05-07 15:02:43.653911 varipeps-0.6.0/varipeps/peps/unitcell.py
+-rw-r--r--   0        0        0     1086 2024-05-07 15:02:43.653911 varipeps-0.6.0/varipeps/typing.py
+-rw-r--r--   0        0        0      119 2024-05-07 15:02:43.653911 varipeps-0.6.0/varipeps/utils/__init__.py
+-rw-r--r--   0        0        0     1285 2024-05-07 15:02:43.653911 varipeps-0.6.0/varipeps/utils/debug_print.py
+-rw-r--r--   0        0        0      739 2024-05-07 15:02:43.653911 varipeps-0.6.0/varipeps/utils/func_cache.py
+-rw-r--r--   0        0        0     2438 2024-05-07 15:02:43.653911 varipeps-0.6.0/varipeps/utils/periodic_indices.py
+-rw-r--r--   0        0        0     1657 2024-05-07 15:02:43.653911 varipeps-0.6.0/varipeps/utils/projector_dict.py
+-rw-r--r--   0        0        0     5398 2024-05-07 15:02:43.653911 varipeps-0.6.0/varipeps/utils/random.py
+-rw-r--r--   0        0        0     3396 2024-05-07 15:02:43.653911 varipeps-0.6.0/varipeps/utils/svd.py
+-rw-r--r--   0        0        0     4254 1970-01-01 00:00:00.000000 varipeps-0.6.0/PKG-INFO
```

### Comparing `varipeps-0.5.5/LICENSE` & `varipeps-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/README.md` & `varipeps-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/pyproject.toml` & `varipeps-0.6.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "variPEPS"
-version = "0.5.5"
+version = "0.6.0"
 description = "Versatile tensor network library for variational ground state simulations in two spatial dimensions"
 authors = ["Jan Naumann <j.naumann@fu-berlin.de>", "Philipp Schmoll <philipp.schmoll@fu-berlin.de>", "Frederik Wilde", "Finn Krein"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/variPEPS/variPEPS_Python"
 documentation = "https://varipeps.readthedocs.io/en/stable/"
 packages = [{include = "varipeps"}]
```

### Comparing `varipeps-0.5.5/varipeps/__init__.py` & `varipeps-0.6.0/varipeps/__init__.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/__version__.py` & `varipeps-0.6.0/varipeps/__version__.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/config.py` & `varipeps-0.6.0/varipeps/config.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/contractions/apply.py` & `varipeps-0.6.0/varipeps/contractions/apply.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/ctmrg/absorption.py` & `varipeps-0.6.0/varipeps/ctmrg/absorption.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/ctmrg/projectors.py` & `varipeps-0.6.0/varipeps/ctmrg/projectors.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/ctmrg/routine.py` & `varipeps-0.6.0/varipeps/ctmrg/routine.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/expectation/model.py` & `varipeps-0.6.0/varipeps/expectation/model.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/expectation/one_site.py` & `varipeps-0.6.0/varipeps/expectation/one_site.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/expectation/spiral_helpers.py` & `varipeps-0.6.0/varipeps/expectation/spiral_helpers.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/expectation/three_sites.py` & `varipeps-0.6.0/varipeps/expectation/three_sites.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/expectation/two_sites.py` & `varipeps-0.6.0/varipeps/expectation/two_sites.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/global_state.py` & `varipeps-0.6.0/varipeps/global_state.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/mapping/florett_pentagon.py` & `varipeps-0.6.0/varipeps/mapping/florett_pentagon.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/mapping/honeycomb.py` & `varipeps-0.6.0/varipeps/mapping/honeycomb.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/mapping/kagome.py` & `varipeps-0.6.0/varipeps/mapping/kagome.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/mapping/maple_leaf.py` & `varipeps-0.6.0/varipeps/mapping/maple_leaf.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/mapping/model.py` & `varipeps-0.6.0/varipeps/mapping/model.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/mapping/square_kagome.py` & `varipeps-0.6.0/varipeps/mapping/square_kagome.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/mapping/triangular.py` & `varipeps-0.6.0/varipeps/mapping/triangular.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/optimization/basinhopping.py` & `varipeps-0.6.0/varipeps/optimization/basinhopping.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/optimization/inner_function.py` & `varipeps-0.6.0/varipeps/optimization/inner_function.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/optimization/line_search.py` & `varipeps-0.6.0/varipeps/optimization/line_search.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/optimization/optimizer.py` & `varipeps-0.6.0/varipeps/optimization/optimizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -182,25 +182,71 @@
     return gradient_unravel(z_result)
 
 
 def autosave_function(
     filename: PathLike,
     tensors: jnp.ndarray,
     unitcell: PEPS_Unit_Cell,
-    counter: Optional[int] = None,
+    counter: Optional[Union[int, str]] = None,
     auxiliary_data: Optional[Dict[str, Any]] = None,
 ) -> None:
     if counter is not None:
         unitcell.save_to_file(
             f"{str(filename)}.{counter}", auxiliary_data=auxiliary_data
         )
     else:
         unitcell.save_to_file(filename, auxiliary_data=auxiliary_data)
 
 
+def _autosave_wrapper(
+    autosave_func,
+    autosave_filename,
+    working_tensors,
+    working_unitcell,
+    working_value,
+    counter,
+    best_run,
+    max_trunc_error_list,
+    step_energies,
+    step_chi,
+    step_conv,
+    spiral_indices,
+    additional_input,
+):
+    auxiliary_data = {
+        "best_run": best_run if best_run is not None else 0,
+        "current_energy": working_value,
+    }
+
+    for k in sorted(max_trunc_error_list.keys()):
+        auxiliary_data[f"max_trunc_error_list_{k:d}"] = max_trunc_error_list[k]
+        auxiliary_data[f"step_energies_{k:d}"] = step_energies[k]
+        auxiliary_data[f"step_chi_{k:d}"] = step_chi[k]
+        auxiliary_data[f"step_conv_{k:d}"] = step_conv[k]
+
+    if spiral_indices is not None:
+        for spiral_i in spiral_indices:
+            auxiliary_data[f"spiral_vector_{spiral_i:d}"] = working_tensors[spiral_i]
+    elif additional_input.get("spiral_vectors") is not None:
+        add_input_spiral = additional_input.get("spiral_vectors")
+        if isinstance(add_input_spiral, jnp.ndarray):
+            add_input_spiral = (add_input_spiral,)
+        for spiral_i, elem in enumerate(add_input_spiral):
+            spiral_i += 1
+            auxiliary_data[f"spiral_vector_{spiral_i:d}"] = elem
+
+    autosave_func(
+        autosave_filename,
+        working_tensors,
+        working_unitcell,
+        counter=counter,
+        auxiliary_data=auxiliary_data,
+    )
+
+
 def optimize_peps_network(
     input_tensors: Union[PEPS_Unit_Cell, Sequence[jnp.ndarray]],
     expectation_func: Expectation_Model,
     convert_to_unitcell_func: Optional[Map_To_PEPS_Model] = None,
     autosave_filename: PathLike = "data/autosave.hdf5",
     autosave_func: Callable[
         [PathLike, Sequence[jnp.ndarray], PEPS_Unit_Cell], None
@@ -252,14 +298,18 @@
         )
         working_unitcell = input_tensors
         generate_unitcell = True
     else:
         if isinstance(input_tensors, collections.abc.Sequence) and isinstance(
             input_tensors[0], PEPS_Unit_Cell
         ):
+            if len(input_tensors[0].get_unique_tensors()) != 1:
+                raise ValueError(
+                    "You want to use spiral PEPS but you use a unit cell with more than one site. Seems wrong to me!"
+                )
             working_tensors = cast(
                 List[jnp.ndarray],
                 [i.tensor for i in input_tensors[0].get_unique_tensors()],
             ) + list(input_tensors[1:])
             working_unitcell = input_tensors[0]
             generate_unitcell = True
         else:
@@ -463,14 +513,30 @@
 
                         if working_value < best_value:
                             best_value = working_value
                             best_tensors = working_tensors
                             best_unitcell = working_unitcell
                             best_run = random_noise_retries
 
+                            _autosave_wrapper(
+                                autosave_func,
+                                autosave_filename,
+                                working_tensors,
+                                working_unitcell,
+                                working_value,
+                                "best",
+                                best_run,
+                                max_trunc_error_list,
+                                step_energies,
+                                step_chi,
+                                step_conv,
+                                spiral_indices,
+                                additional_input,
+                            )
+
                         if isinstance(input_tensors, PEPS_Unit_Cell) or (
                             isinstance(input_tensors, collections.abc.Sequence)
                             and isinstance(input_tensors[0], PEPS_Unit_Cell)
                         ):
                             working_tensors = (
                                 cast(
                                     List[jnp.ndarray],
@@ -573,53 +639,52 @@
                     "Line search step": f"{linesearch_step:0.8f}",
                     "Max. trunc. err.": f"{max_trunc_error:0.8g}",
                 }
             )
             pbar.refresh()
 
             if count % varipeps_config.optimizer_autosave_step_count == 0:
-                auxiliary_data = {
-                    "best_run": best_run if best_run is not None else 0,
-                }
-
-                for k in sorted(max_trunc_error_list.keys()):
-                    auxiliary_data[f"max_trunc_error_list_{k:d}"] = (
-                        max_trunc_error_list[k]
-                    )
-                    auxiliary_data[f"step_energies_{k:d}"] = step_energies[k]
-                    auxiliary_data[f"step_chi_{k:d}"] = step_chi[k]
-                    auxiliary_data[f"step_conv_{k:d}"] = step_conv[k]
-
-                if spiral_indices is not None:
-                    for spiral_i in spiral_indices:
-                        auxiliary_data[f"spiral_vector_{spiral_i:d}"] = working_tensors[
-                            spiral_i
-                        ]
-                elif additional_input.get("spiral_vectors") is not None:
-                    add_input_spiral = additional_input.get("spiral_vectors")
-                    if isinstance(add_input_spiral, jnp.ndarray):
-                        add_input_spiral = (add_input_spiral,)
-                    for spiral_i, elem in enumerate(add_input_spiral):
-                        spiral_i += 1
-                        auxiliary_data[f"spiral_vector_{spiral_i:d}"] = elem
-
-                autosave_func(
+                _autosave_wrapper(
+                    autosave_func,
                     autosave_filename,
                     working_tensors,
                     working_unitcell,
-                    counter=random_noise_retries,
-                    auxiliary_data=auxiliary_data,
+                    working_value,
+                    random_noise_retries,
+                    best_run,
+                    max_trunc_error_list,
+                    step_energies,
+                    step_chi,
+                    step_conv,
+                    spiral_indices,
+                    additional_input,
                 )
 
     if working_value < best_value:
         best_value = working_value
         best_tensors = working_tensors
         best_unitcell = working_unitcell
         best_run = random_noise_retries
 
+        _autosave_wrapper(
+            autosave_func,
+            autosave_filename,
+            working_tensors,
+            working_unitcell,
+            working_value,
+            "best",
+            best_run,
+            max_trunc_error_list,
+            step_energies,
+            step_chi,
+            step_conv,
+            spiral_indices,
+            additional_input,
+        )
+
     print(f"Best energy result found: {best_value}")
 
     return OptimizeResult(
         success=True,
         x=best_tensors,
         fun=best_value,
         unitcell=best_unitcell,
```

### Comparing `varipeps-0.5.5/varipeps/peps/unitcell.py` & `varipeps-0.6.0/varipeps/peps/unitcell.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/typing.py` & `varipeps-0.6.0/varipeps/typing.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/utils/debug_print.py` & `varipeps-0.6.0/varipeps/utils/debug_print.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/utils/func_cache.py` & `varipeps-0.6.0/varipeps/utils/func_cache.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/utils/periodic_indices.py` & `varipeps-0.6.0/varipeps/utils/periodic_indices.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/utils/projector_dict.py` & `varipeps-0.6.0/varipeps/utils/projector_dict.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/utils/random.py` & `varipeps-0.6.0/varipeps/utils/random.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/varipeps/utils/svd.py` & `varipeps-0.6.0/varipeps/utils/svd.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.5/PKG-INFO` & `varipeps-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: variPEPS
-Version: 0.5.5
+Version: 0.6.0
 Summary: Versatile tensor network library for variational ground state simulations in two spatial dimensions
 Home-page: https://github.com/variPEPS/variPEPS_Python
 License: GPL-3.0-or-later
 Author: Jan Naumann
 Author-email: j.naumann@fu-berlin.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

