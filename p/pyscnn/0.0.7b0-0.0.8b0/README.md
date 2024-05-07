# Comparing `tmp/pyscnn-0.0.7b0.tar.gz` & `tmp/pyscnn-0.0.8b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscnn-0.0.7b0.tar", last modified: Fri Nov 17 00:59:50 2023, max compression
+gzip compressed data, was "pyscnn-0.0.8b0.tar", last modified: Tue May  7 18:01:26 2024, max compression
```

## Comparing `pyscnn-0.0.7b0.tar` & `pyscnn-0.0.8b0.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.803694 pyscnn-0.0.7b0/
--rw-r--r--   0 amishkin   (501) staff       (20)     1079 2022-06-14 23:06:36.000000 pyscnn-0.0.7b0/LICENSE
--rw-r--r--   0 amishkin   (501) staff       (20)     3215 2023-11-17 00:59:50.802773 pyscnn-0.0.7b0/PKG-INFO
--rw-r--r--   0 amishkin   (501) staff       (20)     1124 2022-07-04 17:00:59.000000 pyscnn-0.0.7b0/README.md
--rw-r--r--   0 amishkin   (501) staff       (20)      938 2023-11-17 00:59:36.000000 pyscnn-0.0.7b0/pyproject.toml
--rw-r--r--   0 amishkin   (501) staff       (20)       38 2023-11-17 00:59:50.803964 pyscnn-0.0.7b0/setup.cfg
--rw-r--r--   0 amishkin   (501) staff       (20)       54 2022-07-04 16:58:02.000000 pyscnn-0.0.7b0/setup.py
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.714440 pyscnn-0.0.7b0/src/
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.727906 pyscnn-0.0.7b0/src/pyscnn.egg-info/
--rw-r--r--   0 amishkin   (501) staff       (20)     3215 2023-11-17 00:59:50.000000 pyscnn-0.0.7b0/src/pyscnn.egg-info/PKG-INFO
--rw-r--r--   0 amishkin   (501) staff       (20)     4765 2023-11-17 00:59:50.000000 pyscnn-0.0.7b0/src/pyscnn.egg-info/SOURCES.txt
--rw-r--r--   0 amishkin   (501) staff       (20)        1 2023-11-17 00:59:50.000000 pyscnn-0.0.7b0/src/pyscnn.egg-info/dependency_links.txt
--rw-r--r--   0 amishkin   (501) staff       (20)      124 2023-11-17 00:59:50.000000 pyscnn-0.0.7b0/src/pyscnn.egg-info/requires.txt
--rw-r--r--   0 amishkin   (501) staff       (20)        5 2023-11-17 00:59:50.000000 pyscnn-0.0.7b0/src/pyscnn.egg-info/top_level.txt
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.736265 pyscnn-0.0.7b0/src/scnn/
--rw-r--r--   0 amishkin   (501) staff       (20)       76 2022-06-14 22:53:56.000000 pyscnn-0.0.7b0/src/scnn/__init__.py
--rw-r--r--   0 amishkin   (501) staff       (20)    10383 2022-07-05 19:39:06.000000 pyscnn-0.0.7b0/src/scnn/activations.py
--rw-r--r--   0 amishkin   (501) staff       (20)      423 2022-03-17 21:39:08.000000 pyscnn-0.0.7b0/src/scnn/loss_functions.py
--rw-r--r--   0 amishkin   (501) staff       (20)     6440 2022-08-17 23:41:22.000000 pyscnn-0.0.7b0/src/scnn/metrics.py
--rw-r--r--   0 amishkin   (501) staff       (20)    18337 2023-11-17 00:52:40.000000 pyscnn-0.0.7b0/src/scnn/models.py
--rw-r--r--   0 amishkin   (501) staff       (20)    13470 2023-01-19 20:27:26.000000 pyscnn-0.0.7b0/src/scnn/optimize.py
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.738994 pyscnn-0.0.7b0/src/scnn/private/
--rw-r--r--   0 amishkin   (501) staff       (20)        0 2022-02-16 21:35:05.000000 pyscnn-0.0.7b0/src/scnn/private/__init__.py
--rw-r--r--   0 amishkin   (501) staff       (20)     5242 2022-06-14 22:54:38.000000 pyscnn-0.0.7b0/src/scnn/private/initializers.py
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.743427 pyscnn-0.0.7b0/src/scnn/private/interface/
--rw-r--r--   0 amishkin   (501) staff       (20)      982 2023-01-19 20:27:26.000000 pyscnn-0.0.7b0/src/scnn/private/interface/__init__.py
--rw-r--r--   0 amishkin   (501) staff       (20)     3882 2022-08-16 04:17:13.000000 pyscnn-0.0.7b0/src/scnn/private/interface/data.py
--rw-r--r--   0 amishkin   (501) staff       (20)     4501 2022-06-14 22:53:58.000000 pyscnn-0.0.7b0/src/scnn/private/interface/metrics.py
--rw-r--r--   0 amishkin   (501) staff       (20)     6253 2023-10-04 22:38:46.000000 pyscnn-0.0.7b0/src/scnn/private/interface/models.py
--rw-r--r--   0 amishkin   (501) staff       (20)     6110 2023-01-19 20:27:26.000000 pyscnn-0.0.7b0/src/scnn/private/interface/solvers.py
--rw-r--r--   0 amishkin   (501) staff       (20)     1478 2022-06-14 22:53:59.000000 pyscnn-0.0.7b0/src/scnn/private/interface/utils.py
--rw-r--r--   0 amishkin   (501) staff       (20)     3483 2022-07-28 21:16:33.000000 pyscnn-0.0.7b0/src/scnn/private/loss_functions.py
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.747424 pyscnn-0.0.7b0/src/scnn/private/methods/
--rw-r--r--   0 amishkin   (501) staff       (20)     2483 2023-01-19 20:27:26.000000 pyscnn-0.0.7b0/src/scnn/private/methods/__init__.py
--rw-r--r--   0 amishkin   (501) staff       (20)     6105 2022-06-14 22:54:09.000000 pyscnn-0.0.7b0/src/scnn/private/methods/callbacks.py
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.751231 pyscnn-0.0.7b0/src/scnn/private/methods/core/
--rw-r--r--   0 amishkin   (501) staff       (20)      518 2022-03-16 19:06:07.000000 pyscnn-0.0.7b0/src/scnn/private/methods/core/__init__.py
--rw-r--r--   0 amishkin   (501) staff       (20)     1926 2022-03-16 21:27:56.000000 pyscnn-0.0.7b0/src/scnn/private/methods/core/augmented_lagrangian.py
--rw-r--r--   0 amishkin   (501) staff       (20)     2131 2022-06-14 22:54:03.000000 pyscnn-0.0.7b0/src/scnn/private/methods/core/gradient_descent.py
--rw-r--r--   0 amishkin   (501) staff       (20)     2163 2022-06-14 22:54:02.000000 pyscnn-0.0.7b0/src/scnn/private/methods/core/line_search.py
--rw-r--r--   0 amishkin   (501) staff       (20)     5547 2022-06-14 22:54:03.000000 pyscnn-0.0.7b0/src/scnn/private/methods/core/proximal_gradient.py
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.753630 pyscnn-0.0.7b0/src/scnn/private/methods/cvxpy/
--rw-r--r--   0 amishkin   (501) staff       (20)      625 2022-08-02 17:18:25.000000 pyscnn-0.0.7b0/src/scnn/private/methods/cvxpy/__init__.py
--rw-r--r--   0 amishkin   (501) staff       (20)     6244 2022-06-14 22:54:01.000000 pyscnn-0.0.7b0/src/scnn/private/methods/cvxpy/cone_decomposition.py
--rw-r--r--   0 amishkin   (501) staff       (20)     1655 2022-06-14 22:54:02.000000 pyscnn-0.0.7b0/src/scnn/private/methods/cvxpy/cvxpy_solver.py
--rw-r--r--   0 amishkin   (501) staff       (20)     8167 2023-01-19 20:27:26.000000 pyscnn-0.0.7b0/src/scnn/private/methods/cvxpy/training_programs.py
--rw-r--r--   0 amishkin   (501) staff       (20)     2340 2022-06-14 22:54:00.000000 pyscnn-0.0.7b0/src/scnn/private/methods/external_solver.py
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.755598 pyscnn-0.0.7b0/src/scnn/private/methods/line_search/
--rw-r--r--   0 amishkin   (501) staff       (20)      564 2022-03-18 23:29:07.000000 pyscnn-0.0.7b0/src/scnn/private/methods/line_search/__init__.py
--rw-r--r--   0 amishkin   (501) staff       (20)     1191 2022-03-16 19:06:07.000000 pyscnn-0.0.7b0/src/scnn/private/methods/line_search/backtrack.py
--rw-r--r--   0 amishkin   (501) staff       (20)     4251 2022-03-18 23:36:32.000000 pyscnn-0.0.7b0/src/scnn/private/methods/line_search/conditions.py
--rw-r--r--   0 amishkin   (501) staff       (20)     5118 2022-03-16 19:06:07.000000 pyscnn-0.0.7b0/src/scnn/private/methods/line_search/step_size_updates.py
--rw-r--r--   0 amishkin   (501) staff       (20)     2217 2022-06-14 22:54:09.000000 pyscnn-0.0.7b0/src/scnn/private/methods/method_utils.py
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.758385 pyscnn-0.0.7b0/src/scnn/private/methods/optimization_procedures/
--rw-r--r--   0 amishkin   (501) staff       (20)      498 2022-03-16 19:06:07.000000 pyscnn-0.0.7b0/src/scnn/private/methods/optimization_procedures/__init__.py
--rw-r--r--   0 amishkin   (501) staff       (20)    11512 2022-06-14 22:54:08.000000 pyscnn-0.0.7b0/src/scnn/private/methods/optimization_procedures/double_loop_procedure.py
--rw-r--r--   0 amishkin   (501) staff       (20)    11055 2022-06-14 22:54:10.000000 pyscnn-0.0.7b0/src/scnn/private/methods/optimization_procedures/iterative.py
--rw-r--r--   0 amishkin   (501) staff       (20)     4539 2022-06-14 22:54:07.000000 pyscnn-0.0.7b0/src/scnn/private/methods/optimization_procedures/optimization_procedure.py
--rw-r--r--   0 amishkin   (501) staff       (20)     9069 2022-06-14 22:54:08.000000 pyscnn-0.0.7b0/src/scnn/private/methods/optimization_procedures/torch_loop.py
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.762461 pyscnn-0.0.7b0/src/scnn/private/methods/optimizers/
--rw-r--r--   0 amishkin   (501) staff       (20)      609 2022-03-16 19:06:07.000000 pyscnn-0.0.7b0/src/scnn/private/methods/optimizers/__init__.py
--rw-r--r--   0 amishkin   (501) staff       (20)     5933 2023-01-19 20:27:26.000000 pyscnn-0.0.7b0/src/scnn/private/methods/optimizers/augmented_lagrangian.py
--rw-r--r--   0 amishkin   (501) staff       (20)     5473 2022-06-14 22:54:05.000000 pyscnn-0.0.7b0/src/scnn/private/methods/optimizers/fista.py
--rw-r--r--   0 amishkin   (501) staff       (20)     1358 2022-06-14 22:54:07.000000 pyscnn-0.0.7b0/src/scnn/private/methods/optimizers/gd.py
--rw-r--r--   0 amishkin   (501) staff       (20)     1860 2022-06-14 22:54:05.000000 pyscnn-0.0.7b0/src/scnn/private/methods/optimizers/meta_optimizer.py
--rw-r--r--   0 amishkin   (501) staff       (20)     6238 2022-07-26 21:41:48.000000 pyscnn-0.0.7b0/src/scnn/private/methods/optimizers/optimizer.py
--rw-r--r--   0 amishkin   (501) staff       (20)     1842 2022-06-14 22:54:06.000000 pyscnn-0.0.7b0/src/scnn/private/methods/optimizers/pgd.py
--rw-r--r--   0 amishkin   (501) staff       (20)     6190 2022-06-14 22:54:04.000000 pyscnn-0.0.7b0/src/scnn/private/methods/optimizers/proximal_optimizer.py
--rw-r--r--   0 amishkin   (501) staff       (20)      813 2022-06-14 22:54:09.000000 pyscnn-0.0.7b0/src/scnn/private/methods/processing.py
--rw-r--r--   0 amishkin   (501) staff       (20)    10805 2022-06-14 22:54:02.000000 pyscnn-0.0.7b0/src/scnn/private/methods/termination_criteria.py
--rw-r--r--   0 amishkin   (501) staff       (20)    12181 2023-01-19 20:27:26.000000 pyscnn-0.0.7b0/src/scnn/private/metrics.py
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.763992 pyscnn-0.0.7b0/src/scnn/private/models/
--rw-r--r--   0 amishkin   (501) staff       (20)     1188 2023-01-19 20:27:26.000000 pyscnn-0.0.7b0/src/scnn/private/models/__init__.py
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.765698 pyscnn-0.0.7b0/src/scnn/private/models/convex/
--rw-r--r--   0 amishkin   (501) staff       (20)      159 2023-01-19 20:27:26.000000 pyscnn-0.0.7b0/src/scnn/private/models/convex/__init__.py
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.766617 pyscnn-0.0.7b0/src/scnn/private/models/convex/al/
--rw-r--r--   0 amishkin   (501) staff       (20)      113 2023-01-19 20:27:26.000000 pyscnn-0.0.7b0/src/scnn/private/models/convex/al/__init__.py
--rw-r--r--   0 amishkin   (501) staff       (20)    14592 2022-06-14 22:54:17.000000 pyscnn-0.0.7b0/src/scnn/private/models/convex/al/al_mlp.py
--rw-r--r--   0 amishkin   (501) staff       (20)     9867 2022-06-14 22:54:18.000000 pyscnn-0.0.7b0/src/scnn/private/models/convex/convex_mlp.py
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.769134 pyscnn-0.0.7b0/src/scnn/private/models/convex/kernels/
--rw-r--r--   0 amishkin   (501) staff       (20)       70 2022-03-16 19:06:07.000000 pyscnn-0.0.7b0/src/scnn/private/models/convex/kernels/__init__.py
--rw-r--r--   0 amishkin   (501) staff       (20)     5064 2022-03-16 19:06:07.000000 pyscnn-0.0.7b0/src/scnn/private/models/convex/kernels/direct_kernel.py
--rw-r--r--   0 amishkin   (501) staff       (20)     1500 2022-03-16 19:06:07.000000 pyscnn-0.0.7b0/src/scnn/private/models/convex/kernels/einsum_kernel.py
--rw-r--r--   0 amishkin   (501) staff       (20)     5498 2022-03-16 19:06:07.000000 pyscnn-0.0.7b0/src/scnn/private/models/convex/operators.py
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.770632 pyscnn-0.0.7b0/src/scnn/private/models/decompositions/
--rw-r--r--   0 amishkin   (501) staff       (20)       99 2022-04-05 02:13:19.000000 pyscnn-0.0.7b0/src/scnn/private/models/decompositions/__init__.py
--rw-r--r--   0 amishkin   (501) staff       (20)     5610 2022-06-14 22:54:22.000000 pyscnn-0.0.7b0/src/scnn/private/models/decompositions/quadratic_decomposition.py
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.773043 pyscnn-0.0.7b0/src/scnn/private/models/linear/
--rw-r--r--   0 amishkin   (501) staff       (20)      217 2022-03-21 18:45:15.000000 pyscnn-0.0.7b0/src/scnn/private/models/linear/__init__.py
--rw-r--r--   0 amishkin   (501) staff       (20)     2694 2022-06-14 22:54:15.000000 pyscnn-0.0.7b0/src/scnn/private/models/linear/l2_regression.py
--rw-r--r--   0 amishkin   (501) staff       (20)     2596 2022-06-14 22:54:16.000000 pyscnn-0.0.7b0/src/scnn/private/models/linear/logistic_regression.py
--rw-r--r--   0 amishkin   (501) staff       (20)    11006 2023-01-19 20:27:26.000000 pyscnn-0.0.7b0/src/scnn/private/models/model.py
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.773798 pyscnn-0.0.7b0/src/scnn/private/models/non_convex/
--rw-r--r--   0 amishkin   (501) staff       (20)      271 2022-06-14 22:45:38.000000 pyscnn-0.0.7b0/src/scnn/private/models/non_convex/__init__.py
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.776214 pyscnn-0.0.7b0/src/scnn/private/models/non_convex/manual/
--rw-r--r--   0 amishkin   (501) staff       (20)      213 2022-06-14 22:15:52.000000 pyscnn-0.0.7b0/src/scnn/private/models/non_convex/manual/__init__.py
--rw-r--r--   0 amishkin   (501) staff       (20)     3246 2022-06-14 22:54:14.000000 pyscnn-0.0.7b0/src/scnn/private/models/non_convex/manual/gated_relu_mlp.py
--rw-r--r--   0 amishkin   (501) staff       (20)     5277 2022-06-14 22:54:13.000000 pyscnn-0.0.7b0/src/scnn/private/models/non_convex/manual/relu_mlp.py
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.779361 pyscnn-0.0.7b0/src/scnn/private/models/non_convex/torch/
--rw-r--r--   0 amishkin   (501) staff       (20)      266 2022-03-16 19:06:07.000000 pyscnn-0.0.7b0/src/scnn/private/models/non_convex/torch/__init__.py
--rw-r--r--   0 amishkin   (501) staff       (20)      990 2022-03-16 19:06:07.000000 pyscnn-0.0.7b0/src/scnn/private/models/non_convex/torch/gated_relu_layer.py
--rw-r--r--   0 amishkin   (501) staff       (20)      828 2022-06-14 22:54:12.000000 pyscnn-0.0.7b0/src/scnn/private/models/non_convex/torch/layer_wrapper.py
--rw-r--r--   0 amishkin   (501) staff       (20)     4908 2022-06-14 22:54:12.000000 pyscnn-0.0.7b0/src/scnn/private/models/non_convex/torch/sequential_wrapper.py
--rw-r--r--   0 amishkin   (501) staff       (20)     3355 2022-06-14 22:54:21.000000 pyscnn-0.0.7b0/src/scnn/private/models/one_vs_all.py
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.787178 pyscnn-0.0.7b0/src/scnn/private/models/regularizers/
--rw-r--r--   0 amishkin   (501) staff       (20)      607 2023-01-19 20:27:26.000000 pyscnn-0.0.7b0/src/scnn/private/models/regularizers/__init__.py
--rw-r--r--   0 amishkin   (501) staff       (20)     1870 2022-06-14 22:54:18.000000 pyscnn-0.0.7b0/src/scnn/private/models/regularizers/constraint.py
--rw-r--r--   0 amishkin   (501) staff       (20)     3075 2022-06-14 22:54:19.000000 pyscnn-0.0.7b0/src/scnn/private/models/regularizers/feature_group_l1.py
--rw-r--r--   0 amishkin   (501) staff       (20)     2514 2023-01-19 20:27:26.000000 pyscnn-0.0.7b0/src/scnn/private/models/regularizers/group_l1.py
--rw-r--r--   0 amishkin   (501) staff       (20)     3124 2022-06-14 22:54:21.000000 pyscnn-0.0.7b0/src/scnn/private/models/regularizers/group_l1_orthant.py
--rw-r--r--   0 amishkin   (501) staff       (20)     1465 2022-06-14 22:54:20.000000 pyscnn-0.0.7b0/src/scnn/private/models/regularizers/l1.py
--rw-r--r--   0 amishkin   (501) staff       (20)      545 2022-06-14 22:54:20.000000 pyscnn-0.0.7b0/src/scnn/private/models/regularizers/l1_squared.py
--rw-r--r--   0 amishkin   (501) staff       (20)      965 2022-06-14 22:54:19.000000 pyscnn-0.0.7b0/src/scnn/private/models/regularizers/l2.py
--rw-r--r--   0 amishkin   (501) staff       (20)      789 2022-06-14 22:54:19.000000 pyscnn-0.0.7b0/src/scnn/private/models/regularizers/orthant.py
--rw-r--r--   0 amishkin   (501) staff       (20)     1329 2022-03-16 19:06:07.000000 pyscnn-0.0.7b0/src/scnn/private/models/regularizers/regularizer.py
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.788994 pyscnn-0.0.7b0/src/scnn/private/models/solution_mappings/
--rw-r--r--   0 amishkin   (501) staff       (20)     1522 2023-01-19 20:27:26.000000 pyscnn-0.0.7b0/src/scnn/private/models/solution_mappings/__init__.py
--rw-r--r--   0 amishkin   (501) staff       (20)     8109 2023-01-19 20:27:26.000000 pyscnn-0.0.7b0/src/scnn/private/models/solution_mappings/mlps.py
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.790547 pyscnn-0.0.7b0/src/scnn/private/prox/
--rw-r--r--   0 amishkin   (501) staff       (20)      325 2022-06-14 22:41:46.000000 pyscnn-0.0.7b0/src/scnn/private/prox/__init__.py
--rw-r--r--   0 amishkin   (501) staff       (20)     8434 2022-07-04 16:53:40.000000 pyscnn-0.0.7b0/src/scnn/private/prox/proximal_ops.py
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.792467 pyscnn-0.0.7b0/src/scnn/private/utils/
--rw-r--r--   0 amishkin   (501) staff       (20)      297 2022-03-16 19:06:07.000000 pyscnn-0.0.7b0/src/scnn/private/utils/__init__.py
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.795488 pyscnn-0.0.7b0/src/scnn/private/utils/data/
--rw-r--r--   0 amishkin   (501) staff       (20)      423 2023-01-19 20:27:26.000000 pyscnn-0.0.7b0/src/scnn/private/utils/data/__init__.py
--rw-r--r--   0 amishkin   (501) staff       (20)     7979 2023-01-19 20:27:26.000000 pyscnn-0.0.7b0/src/scnn/private/utils/data/synthetic.py
--rw-r--r--   0 amishkin   (501) staff       (20)     2323 2023-10-10 19:13:00.000000 pyscnn-0.0.7b0/src/scnn/private/utils/data/transforms.py
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.798237 pyscnn-0.0.7b0/src/scnn/private/utils/linear/
--rw-r--r--   0 amishkin   (501) staff       (20)      321 2022-03-16 19:06:07.000000 pyscnn-0.0.7b0/src/scnn/private/utils/linear/__init__.py
--rw-r--r--   0 amishkin   (501) staff       (20)      733 2022-03-16 19:06:07.000000 pyscnn-0.0.7b0/src/scnn/private/utils/linear/direct_solvers.py
--rw-r--r--   0 amishkin   (501) staff       (20)     4905 2022-06-14 22:54:11.000000 pyscnn-0.0.7b0/src/scnn/private/utils/linear/iterative_solvers.py
--rw-r--r--   0 amishkin   (501) staff       (20)     2545 2022-06-14 22:54:11.000000 pyscnn-0.0.7b0/src/scnn/private/utils/linear/preconditioners.py
--rw-r--r--   0 amishkin   (501) staff       (20)     2278 2022-03-16 19:06:07.000000 pyscnn-0.0.7b0/src/scnn/private/utils/linear_operators.py
--rw-r--r--   0 amishkin   (501) staff       (20)        0 2021-12-15 05:48:59.000000 pyscnn-0.0.7b0/src/scnn/py.typed
--rw-r--r--   0 amishkin   (501) staff       (20)     2050 2023-01-19 20:27:26.000000 pyscnn-0.0.7b0/src/scnn/regularizers.py
--rw-r--r--   0 amishkin   (501) staff       (20)    13982 2023-01-19 20:27:26.000000 pyscnn-0.0.7b0/src/scnn/solvers.py
--rw-r--r--   0 amishkin   (501) staff       (20)     6258 2022-06-14 22:53:56.000000 pyscnn-0.0.7b0/src/scnn/support.py
-drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2023-11-17 00:59:50.801679 pyscnn-0.0.7b0/test/
--rw-r--r--   0 amishkin   (501) staff       (20)     3918 2022-06-14 22:53:40.000000 pyscnn-0.0.7b0/test/test_activations.py
--rw-r--r--   0 amishkin   (501) staff       (20)     9499 2022-06-14 22:53:41.000000 pyscnn-0.0.7b0/test/test_optimize.py
--rw-r--r--   0 amishkin   (501) staff       (20)     2354 2022-06-14 22:53:51.000000 pyscnn-0.0.7b0/test/test_regularizers.py
--rw-r--r--   0 amishkin   (501) staff       (20)     3517 2022-06-14 22:53:41.000000 pyscnn-0.0.7b0/test/test_solvers.py
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.867510 pyscnn-0.0.8b0/
+-rw-r--r--   0 amishkin   (501) staff       (20)     1079 2022-06-14 23:06:36.000000 pyscnn-0.0.8b0/LICENSE
+-rw-r--r--   0 amishkin   (501) staff       (20)     3217 2024-05-07 18:01:26.867131 pyscnn-0.0.8b0/PKG-INFO
+-rw-r--r--   0 amishkin   (501) staff       (20)     1126 2024-05-07 17:58:09.000000 pyscnn-0.0.8b0/README.md
+-rw-r--r--   0 amishkin   (501) staff       (20)      938 2024-05-07 17:57:24.000000 pyscnn-0.0.8b0/pyproject.toml
+-rw-r--r--   0 amishkin   (501) staff       (20)       38 2024-05-07 18:01:26.867608 pyscnn-0.0.8b0/setup.cfg
+-rw-r--r--   0 amishkin   (501) staff       (20)       54 2022-07-04 16:58:02.000000 pyscnn-0.0.8b0/setup.py
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.782236 pyscnn-0.0.8b0/src/
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.866594 pyscnn-0.0.8b0/src/pyscnn.egg-info/
+-rw-r--r--   0 amishkin   (501) staff       (20)     3217 2024-05-07 18:01:26.000000 pyscnn-0.0.8b0/src/pyscnn.egg-info/PKG-INFO
+-rw-r--r--   0 amishkin   (501) staff       (20)     4765 2024-05-07 18:01:26.000000 pyscnn-0.0.8b0/src/pyscnn.egg-info/SOURCES.txt
+-rw-r--r--   0 amishkin   (501) staff       (20)        1 2024-05-07 18:01:26.000000 pyscnn-0.0.8b0/src/pyscnn.egg-info/dependency_links.txt
+-rw-r--r--   0 amishkin   (501) staff       (20)      124 2024-05-07 18:01:26.000000 pyscnn-0.0.8b0/src/pyscnn.egg-info/requires.txt
+-rw-r--r--   0 amishkin   (501) staff       (20)        5 2024-05-07 18:01:26.000000 pyscnn-0.0.8b0/src/pyscnn.egg-info/top_level.txt
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.797465 pyscnn-0.0.8b0/src/scnn/
+-rw-r--r--   0 amishkin   (501) staff       (20)       76 2022-06-14 22:53:56.000000 pyscnn-0.0.8b0/src/scnn/__init__.py
+-rw-r--r--   0 amishkin   (501) staff       (20)    10383 2023-11-29 23:16:13.000000 pyscnn-0.0.8b0/src/scnn/activations.py
+-rw-r--r--   0 amishkin   (501) staff       (20)      423 2022-03-17 21:39:08.000000 pyscnn-0.0.8b0/src/scnn/loss_functions.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     6440 2023-11-29 22:56:13.000000 pyscnn-0.0.8b0/src/scnn/metrics.py
+-rw-r--r--   0 amishkin   (501) staff       (20)    18337 2024-05-07 17:52:53.000000 pyscnn-0.0.8b0/src/scnn/models.py
+-rw-r--r--   0 amishkin   (501) staff       (20)    13470 2024-05-06 22:40:43.000000 pyscnn-0.0.8b0/src/scnn/optimize.py
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.800376 pyscnn-0.0.8b0/src/scnn/private/
+-rw-r--r--   0 amishkin   (501) staff       (20)        0 2022-02-16 21:35:05.000000 pyscnn-0.0.8b0/src/scnn/private/__init__.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     5242 2022-06-14 22:54:38.000000 pyscnn-0.0.8b0/src/scnn/private/initializers.py
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.804725 pyscnn-0.0.8b0/src/scnn/private/interface/
+-rw-r--r--   0 amishkin   (501) staff       (20)      982 2023-11-29 22:56:13.000000 pyscnn-0.0.8b0/src/scnn/private/interface/__init__.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     3959 2024-05-07 17:54:59.000000 pyscnn-0.0.8b0/src/scnn/private/interface/data.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     4501 2023-11-29 22:56:13.000000 pyscnn-0.0.8b0/src/scnn/private/interface/metrics.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     6376 2024-05-07 17:57:52.000000 pyscnn-0.0.8b0/src/scnn/private/interface/models.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     6110 2023-11-29 22:56:13.000000 pyscnn-0.0.8b0/src/scnn/private/interface/solvers.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     1478 2022-06-14 22:53:59.000000 pyscnn-0.0.8b0/src/scnn/private/interface/utils.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     3483 2022-07-28 21:16:33.000000 pyscnn-0.0.8b0/src/scnn/private/loss_functions.py
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.809302 pyscnn-0.0.8b0/src/scnn/private/methods/
+-rw-r--r--   0 amishkin   (501) staff       (20)     2483 2023-11-29 22:56:13.000000 pyscnn-0.0.8b0/src/scnn/private/methods/__init__.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     6105 2022-06-14 22:54:09.000000 pyscnn-0.0.8b0/src/scnn/private/methods/callbacks.py
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.814132 pyscnn-0.0.8b0/src/scnn/private/methods/core/
+-rw-r--r--   0 amishkin   (501) staff       (20)      518 2022-03-16 19:06:07.000000 pyscnn-0.0.8b0/src/scnn/private/methods/core/__init__.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     1926 2022-03-16 21:27:56.000000 pyscnn-0.0.8b0/src/scnn/private/methods/core/augmented_lagrangian.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     2131 2022-06-14 22:54:03.000000 pyscnn-0.0.8b0/src/scnn/private/methods/core/gradient_descent.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     2163 2022-06-14 22:54:02.000000 pyscnn-0.0.8b0/src/scnn/private/methods/core/line_search.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     5547 2022-06-14 22:54:03.000000 pyscnn-0.0.8b0/src/scnn/private/methods/core/proximal_gradient.py
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.817153 pyscnn-0.0.8b0/src/scnn/private/methods/cvxpy/
+-rw-r--r--   0 amishkin   (501) staff       (20)      625 2022-08-02 17:18:25.000000 pyscnn-0.0.8b0/src/scnn/private/methods/cvxpy/__init__.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     6244 2022-06-14 22:54:01.000000 pyscnn-0.0.8b0/src/scnn/private/methods/cvxpy/cone_decomposition.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     1655 2022-06-14 22:54:02.000000 pyscnn-0.0.8b0/src/scnn/private/methods/cvxpy/cvxpy_solver.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     8167 2023-11-29 22:56:13.000000 pyscnn-0.0.8b0/src/scnn/private/methods/cvxpy/training_programs.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     2340 2022-06-14 22:54:00.000000 pyscnn-0.0.8b0/src/scnn/private/methods/external_solver.py
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.821271 pyscnn-0.0.8b0/src/scnn/private/methods/line_search/
+-rw-r--r--   0 amishkin   (501) staff       (20)      564 2022-03-18 23:29:07.000000 pyscnn-0.0.8b0/src/scnn/private/methods/line_search/__init__.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     1191 2022-03-16 19:06:07.000000 pyscnn-0.0.8b0/src/scnn/private/methods/line_search/backtrack.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     4251 2022-03-18 23:36:32.000000 pyscnn-0.0.8b0/src/scnn/private/methods/line_search/conditions.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     5118 2022-03-16 19:06:07.000000 pyscnn-0.0.8b0/src/scnn/private/methods/line_search/step_size_updates.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     2217 2022-06-14 22:54:09.000000 pyscnn-0.0.8b0/src/scnn/private/methods/method_utils.py
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.825372 pyscnn-0.0.8b0/src/scnn/private/methods/optimization_procedures/
+-rw-r--r--   0 amishkin   (501) staff       (20)      498 2022-03-16 19:06:07.000000 pyscnn-0.0.8b0/src/scnn/private/methods/optimization_procedures/__init__.py
+-rw-r--r--   0 amishkin   (501) staff       (20)    11512 2022-06-14 22:54:08.000000 pyscnn-0.0.8b0/src/scnn/private/methods/optimization_procedures/double_loop_procedure.py
+-rw-r--r--   0 amishkin   (501) staff       (20)    11055 2022-06-14 22:54:10.000000 pyscnn-0.0.8b0/src/scnn/private/methods/optimization_procedures/iterative.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     4539 2022-06-14 22:54:07.000000 pyscnn-0.0.8b0/src/scnn/private/methods/optimization_procedures/optimization_procedure.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     9069 2022-06-14 22:54:08.000000 pyscnn-0.0.8b0/src/scnn/private/methods/optimization_procedures/torch_loop.py
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.831525 pyscnn-0.0.8b0/src/scnn/private/methods/optimizers/
+-rw-r--r--   0 amishkin   (501) staff       (20)      609 2022-03-16 19:06:07.000000 pyscnn-0.0.8b0/src/scnn/private/methods/optimizers/__init__.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     5933 2023-11-29 22:56:13.000000 pyscnn-0.0.8b0/src/scnn/private/methods/optimizers/augmented_lagrangian.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     5473 2022-06-14 22:54:05.000000 pyscnn-0.0.8b0/src/scnn/private/methods/optimizers/fista.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     1358 2022-06-14 22:54:07.000000 pyscnn-0.0.8b0/src/scnn/private/methods/optimizers/gd.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     1860 2022-06-14 22:54:05.000000 pyscnn-0.0.8b0/src/scnn/private/methods/optimizers/meta_optimizer.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     6238 2022-07-26 21:41:48.000000 pyscnn-0.0.8b0/src/scnn/private/methods/optimizers/optimizer.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     1842 2022-06-14 22:54:06.000000 pyscnn-0.0.8b0/src/scnn/private/methods/optimizers/pgd.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     6190 2022-06-14 22:54:04.000000 pyscnn-0.0.8b0/src/scnn/private/methods/optimizers/proximal_optimizer.py
+-rw-r--r--   0 amishkin   (501) staff       (20)      813 2022-06-14 22:54:09.000000 pyscnn-0.0.8b0/src/scnn/private/methods/processing.py
+-rw-r--r--   0 amishkin   (501) staff       (20)    10805 2022-06-14 22:54:02.000000 pyscnn-0.0.8b0/src/scnn/private/methods/termination_criteria.py
+-rw-r--r--   0 amishkin   (501) staff       (20)    12181 2024-05-06 22:40:43.000000 pyscnn-0.0.8b0/src/scnn/private/metrics.py
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.834169 pyscnn-0.0.8b0/src/scnn/private/models/
+-rw-r--r--   0 amishkin   (501) staff       (20)     1188 2024-05-06 22:40:43.000000 pyscnn-0.0.8b0/src/scnn/private/models/__init__.py
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.836386 pyscnn-0.0.8b0/src/scnn/private/models/convex/
+-rw-r--r--   0 amishkin   (501) staff       (20)      159 2024-05-06 22:40:43.000000 pyscnn-0.0.8b0/src/scnn/private/models/convex/__init__.py
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.837976 pyscnn-0.0.8b0/src/scnn/private/models/convex/al/
+-rw-r--r--   0 amishkin   (501) staff       (20)      113 2023-11-29 22:56:13.000000 pyscnn-0.0.8b0/src/scnn/private/models/convex/al/__init__.py
+-rw-r--r--   0 amishkin   (501) staff       (20)    14592 2023-11-29 22:47:39.000000 pyscnn-0.0.8b0/src/scnn/private/models/convex/al/al_mlp.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     9867 2022-06-14 22:54:18.000000 pyscnn-0.0.8b0/src/scnn/private/models/convex/convex_mlp.py
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.840301 pyscnn-0.0.8b0/src/scnn/private/models/convex/kernels/
+-rw-r--r--   0 amishkin   (501) staff       (20)       70 2022-03-16 19:06:07.000000 pyscnn-0.0.8b0/src/scnn/private/models/convex/kernels/__init__.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     5064 2022-03-16 19:06:07.000000 pyscnn-0.0.8b0/src/scnn/private/models/convex/kernels/direct_kernel.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     1500 2022-03-16 19:06:07.000000 pyscnn-0.0.8b0/src/scnn/private/models/convex/kernels/einsum_kernel.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     5498 2022-03-16 19:06:07.000000 pyscnn-0.0.8b0/src/scnn/private/models/convex/operators.py
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.842050 pyscnn-0.0.8b0/src/scnn/private/models/decompositions/
+-rw-r--r--   0 amishkin   (501) staff       (20)       99 2022-04-05 02:13:19.000000 pyscnn-0.0.8b0/src/scnn/private/models/decompositions/__init__.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     5610 2022-06-14 22:54:22.000000 pyscnn-0.0.8b0/src/scnn/private/models/decompositions/quadratic_decomposition.py
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.844446 pyscnn-0.0.8b0/src/scnn/private/models/linear/
+-rw-r--r--   0 amishkin   (501) staff       (20)      217 2022-03-21 18:45:15.000000 pyscnn-0.0.8b0/src/scnn/private/models/linear/__init__.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     2694 2022-06-14 22:54:15.000000 pyscnn-0.0.8b0/src/scnn/private/models/linear/l2_regression.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     2596 2022-06-14 22:54:16.000000 pyscnn-0.0.8b0/src/scnn/private/models/linear/logistic_regression.py
+-rw-r--r--   0 amishkin   (501) staff       (20)    11006 2023-11-29 22:56:13.000000 pyscnn-0.0.8b0/src/scnn/private/models/model.py
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.845148 pyscnn-0.0.8b0/src/scnn/private/models/non_convex/
+-rw-r--r--   0 amishkin   (501) staff       (20)      271 2022-06-14 22:45:38.000000 pyscnn-0.0.8b0/src/scnn/private/models/non_convex/__init__.py
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.847344 pyscnn-0.0.8b0/src/scnn/private/models/non_convex/manual/
+-rw-r--r--   0 amishkin   (501) staff       (20)      213 2022-06-14 22:15:52.000000 pyscnn-0.0.8b0/src/scnn/private/models/non_convex/manual/__init__.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     3246 2024-05-07 17:52:53.000000 pyscnn-0.0.8b0/src/scnn/private/models/non_convex/manual/gated_relu_mlp.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     5277 2022-06-14 22:54:13.000000 pyscnn-0.0.8b0/src/scnn/private/models/non_convex/manual/relu_mlp.py
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.850356 pyscnn-0.0.8b0/src/scnn/private/models/non_convex/torch/
+-rw-r--r--   0 amishkin   (501) staff       (20)      266 2022-03-16 19:06:07.000000 pyscnn-0.0.8b0/src/scnn/private/models/non_convex/torch/__init__.py
+-rw-r--r--   0 amishkin   (501) staff       (20)      990 2022-03-16 19:06:07.000000 pyscnn-0.0.8b0/src/scnn/private/models/non_convex/torch/gated_relu_layer.py
+-rw-r--r--   0 amishkin   (501) staff       (20)      828 2022-06-14 22:54:12.000000 pyscnn-0.0.8b0/src/scnn/private/models/non_convex/torch/layer_wrapper.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     4908 2022-06-14 22:54:12.000000 pyscnn-0.0.8b0/src/scnn/private/models/non_convex/torch/sequential_wrapper.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     3355 2022-06-14 22:54:21.000000 pyscnn-0.0.8b0/src/scnn/private/models/one_vs_all.py
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.855833 pyscnn-0.0.8b0/src/scnn/private/models/regularizers/
+-rw-r--r--   0 amishkin   (501) staff       (20)      607 2023-11-29 22:56:13.000000 pyscnn-0.0.8b0/src/scnn/private/models/regularizers/__init__.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     1870 2022-06-14 22:54:18.000000 pyscnn-0.0.8b0/src/scnn/private/models/regularizers/constraint.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     3075 2022-06-14 22:54:19.000000 pyscnn-0.0.8b0/src/scnn/private/models/regularizers/feature_group_l1.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     2514 2023-11-29 22:56:13.000000 pyscnn-0.0.8b0/src/scnn/private/models/regularizers/group_l1.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     3124 2022-06-14 22:54:21.000000 pyscnn-0.0.8b0/src/scnn/private/models/regularizers/group_l1_orthant.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     1465 2022-06-14 22:54:20.000000 pyscnn-0.0.8b0/src/scnn/private/models/regularizers/l1.py
+-rw-r--r--   0 amishkin   (501) staff       (20)      545 2022-06-14 22:54:20.000000 pyscnn-0.0.8b0/src/scnn/private/models/regularizers/l1_squared.py
+-rw-r--r--   0 amishkin   (501) staff       (20)      965 2022-06-14 22:54:19.000000 pyscnn-0.0.8b0/src/scnn/private/models/regularizers/l2.py
+-rw-r--r--   0 amishkin   (501) staff       (20)      789 2022-06-14 22:54:19.000000 pyscnn-0.0.8b0/src/scnn/private/models/regularizers/orthant.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     1329 2022-03-16 19:06:07.000000 pyscnn-0.0.8b0/src/scnn/private/models/regularizers/regularizer.py
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.856956 pyscnn-0.0.8b0/src/scnn/private/models/solution_mappings/
+-rw-r--r--   0 amishkin   (501) staff       (20)     1522 2023-11-29 22:56:13.000000 pyscnn-0.0.8b0/src/scnn/private/models/solution_mappings/__init__.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     8109 2024-05-07 17:52:53.000000 pyscnn-0.0.8b0/src/scnn/private/models/solution_mappings/mlps.py
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.858080 pyscnn-0.0.8b0/src/scnn/private/prox/
+-rw-r--r--   0 amishkin   (501) staff       (20)      325 2023-11-29 22:56:13.000000 pyscnn-0.0.8b0/src/scnn/private/prox/__init__.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     8434 2023-11-29 22:56:13.000000 pyscnn-0.0.8b0/src/scnn/private/prox/proximal_ops.py
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.859483 pyscnn-0.0.8b0/src/scnn/private/utils/
+-rw-r--r--   0 amishkin   (501) staff       (20)      297 2022-03-16 19:06:07.000000 pyscnn-0.0.8b0/src/scnn/private/utils/__init__.py
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.861092 pyscnn-0.0.8b0/src/scnn/private/utils/data/
+-rw-r--r--   0 amishkin   (501) staff       (20)      423 2023-11-29 22:56:13.000000 pyscnn-0.0.8b0/src/scnn/private/utils/data/__init__.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     7979 2023-11-29 22:56:13.000000 pyscnn-0.0.8b0/src/scnn/private/utils/data/synthetic.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     2446 2024-05-07 17:55:00.000000 pyscnn-0.0.8b0/src/scnn/private/utils/data/transforms.py
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.863466 pyscnn-0.0.8b0/src/scnn/private/utils/linear/
+-rw-r--r--   0 amishkin   (501) staff       (20)      321 2022-03-16 19:06:07.000000 pyscnn-0.0.8b0/src/scnn/private/utils/linear/__init__.py
+-rw-r--r--   0 amishkin   (501) staff       (20)      733 2022-03-16 19:06:07.000000 pyscnn-0.0.8b0/src/scnn/private/utils/linear/direct_solvers.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     4905 2022-06-14 22:54:11.000000 pyscnn-0.0.8b0/src/scnn/private/utils/linear/iterative_solvers.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     2545 2022-06-14 22:54:11.000000 pyscnn-0.0.8b0/src/scnn/private/utils/linear/preconditioners.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     2278 2022-03-16 19:06:07.000000 pyscnn-0.0.8b0/src/scnn/private/utils/linear_operators.py
+-rw-r--r--   0 amishkin   (501) staff       (20)        0 2021-12-15 05:48:59.000000 pyscnn-0.0.8b0/src/scnn/py.typed
+-rw-r--r--   0 amishkin   (501) staff       (20)     2050 2023-11-29 22:56:13.000000 pyscnn-0.0.8b0/src/scnn/regularizers.py
+-rw-r--r--   0 amishkin   (501) staff       (20)    13982 2024-05-06 22:40:43.000000 pyscnn-0.0.8b0/src/scnn/solvers.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     6258 2023-11-29 22:56:13.000000 pyscnn-0.0.8b0/src/scnn/support.py
+drwxr-xr-x   0 amishkin   (501) staff       (20)        0 2024-05-07 18:01:26.865965 pyscnn-0.0.8b0/test/
+-rw-r--r--   0 amishkin   (501) staff       (20)     3918 2022-06-14 22:53:40.000000 pyscnn-0.0.8b0/test/test_activations.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     9499 2022-06-14 22:53:41.000000 pyscnn-0.0.8b0/test/test_optimize.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     2354 2022-06-14 22:53:51.000000 pyscnn-0.0.8b0/test/test_regularizers.py
+-rw-r--r--   0 amishkin   (501) staff       (20)     3517 2022-06-14 22:53:41.000000 pyscnn-0.0.8b0/test/test_solvers.py
```

### Comparing `pyscnn-0.0.7b0/LICENSE` & `pyscnn-0.0.8b0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/PKG-INFO` & `pyscnn-0.0.8b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscnn
-Version: 0.0.7b0
+Version: 0.0.8b0
 Summary: Scalable Convex Neural Networks: a package for fasts convex optimization of shallow neural networks.
 Author-email: Aaron Mishkin <amishkin@cs.stanford.edu>
 License: MIT License
         
         Copyright (c) 2022 Pilanci Research Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -60,15 +60,15 @@
 python -m pip install pyscnn
 ```
 
 Or, clone the repository and manually install: 
 
 ```
 git clone https://github.com/pilancilab/scnn.git
-python -m pip install scnn
+python -m pip install ./scnn
 ```
 
 ### Contributions
 
 Coming soon!
 
 ### Citation
```

### Comparing `pyscnn-0.0.7b0/README.md` & `pyscnn-0.0.8b0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 python -m pip install pyscnn
 ```
 
 Or, clone the repository and manually install: 
 
 ```
 git clone https://github.com/pilancilab/scnn.git
-python -m pip install scnn
+python -m pip install ./scnn
 ```
 
 ### Contributions
 
 Coming soon!
 
 ### Citation
```

### Comparing `pyscnn-0.0.7b0/pyproject.toml` & `pyscnn-0.0.8b0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyscnn"
-version = "0.0.7-beta"
+version = "0.0.8-beta"
 authors = [
   { name="Aaron Mishkin", email="amishkin@cs.stanford.edu" },
 ]
 description = "Scalable Convex Neural Networks: a package for fasts convex optimization of shallow neural networks."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `pyscnn-0.0.7b0/src/pyscnn.egg-info/PKG-INFO` & `pyscnn-0.0.8b0/src/pyscnn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscnn
-Version: 0.0.7b0
+Version: 0.0.8b0
 Summary: Scalable Convex Neural Networks: a package for fasts convex optimization of shallow neural networks.
 Author-email: Aaron Mishkin <amishkin@cs.stanford.edu>
 License: MIT License
         
         Copyright (c) 2022 Pilanci Research Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -60,15 +60,15 @@
 python -m pip install pyscnn
 ```
 
 Or, clone the repository and manually install: 
 
 ```
 git clone https://github.com/pilancilab/scnn.git
-python -m pip install scnn
+python -m pip install ./scnn
 ```
 
 ### Contributions
 
 Coming soon!
 
 ### Citation
```

### Comparing `pyscnn-0.0.7b0/src/pyscnn.egg-info/SOURCES.txt` & `pyscnn-0.0.8b0/src/pyscnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/activations.py` & `pyscnn-0.0.8b0/src/scnn/activations.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/metrics.py` & `pyscnn-0.0.8b0/src/scnn/metrics.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/models.py` & `pyscnn-0.0.8b0/src/scnn/models.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/optimize.py` & `pyscnn-0.0.8b0/src/scnn/optimize.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/initializers.py` & `pyscnn-0.0.8b0/src/scnn/private/initializers.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/interface/__init__.py` & `pyscnn-0.0.8b0/src/scnn/private/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/interface/data.py` & `pyscnn-0.0.8b0/src/scnn/private/interface/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,17 @@
         weights: a :math:`(\\ldots \\times d)` tensor of weights to map back into the input space.
         column_norms: a :math:`(d,)` vector of the column-norms of the original training data.
 
     Returns:
         A :math:`(\\ldots \\times d)` tensor of weights in the original
         input space.
     """
-    return weights / column_norms
+    return np.divide(
+        weights, column_norms, out=np.zeros_like(weights), where=column_norms != 0
+    )
 
 
 def input_into_normalized_space(model_weights, column_norms):
     """Map the weights of a model in the original data space into the column-
     normalized data space.
 
     Args:
```

### Comparing `pyscnn-0.0.7b0/src/scnn/private/interface/metrics.py` & `pyscnn-0.0.8b0/src/scnn/private/interface/metrics.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/interface/models.py` & `pyscnn-0.0.8b0/src/scnn/private/interface/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,18 +88,23 @@
     internal_model: InternalModel
     d, c = model.d + model.bias, model.c
     internal_reg = build_internal_regularizer(regularizer)
 
     if isinstance(model, LinearModel):
         return LinearRegression(d, c, regularizer=internal_reg)
 
+    G_input = model.G
+
+    if model.bias:
+        G_input = np.concatenate([G_input,model.G_bias.reshape([1,-1])],axis=0)
+
     D, G = lab.all_to_tensor(
         compute_activation_patterns(
             lab.to_np(X_train),
-            model.G,
+            G_input,
             bias=model.bias,
         ),
         dtype=lab.get_dtype(),
     )
 
     if isinstance(model, ConvexReLU):
         internal_model = AL_MLP(
```

### Comparing `pyscnn-0.0.7b0/src/scnn/private/interface/solvers.py` & `pyscnn-0.0.8b0/src/scnn/private/interface/solvers.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/interface/utils.py` & `pyscnn-0.0.8b0/src/scnn/private/interface/utils.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/loss_functions.py` & `pyscnn-0.0.8b0/src/scnn/private/loss_functions.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/__init__.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/callbacks.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/callbacks.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/core/__init__.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/core/augmented_lagrangian.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/core/augmented_lagrangian.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/core/gradient_descent.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/core/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/core/line_search.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/core/line_search.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/core/proximal_gradient.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/core/proximal_gradient.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/cvxpy/__init__.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/cvxpy/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/cvxpy/cone_decomposition.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/cvxpy/cone_decomposition.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/cvxpy/cvxpy_solver.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/cvxpy/cvxpy_solver.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/cvxpy/training_programs.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/cvxpy/training_programs.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/external_solver.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/external_solver.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/line_search/__init__.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/line_search/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/line_search/backtrack.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/line_search/backtrack.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/line_search/conditions.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/line_search/conditions.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/line_search/step_size_updates.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/line_search/step_size_updates.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/method_utils.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/method_utils.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/optimization_procedures/double_loop_procedure.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/optimization_procedures/double_loop_procedure.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/optimization_procedures/iterative.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/optimization_procedures/iterative.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/optimization_procedures/optimization_procedure.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/optimization_procedures/optimization_procedure.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/optimization_procedures/torch_loop.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/optimization_procedures/torch_loop.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/optimizers/__init__.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/optimizers/augmented_lagrangian.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/optimizers/augmented_lagrangian.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/optimizers/fista.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/optimizers/fista.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/optimizers/gd.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/optimizers/gd.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/optimizers/meta_optimizer.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/optimizers/meta_optimizer.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/optimizers/optimizer.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/optimizers/pgd.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/optimizers/pgd.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/optimizers/proximal_optimizer.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/optimizers/proximal_optimizer.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/processing.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/processing.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/methods/termination_criteria.py` & `pyscnn-0.0.8b0/src/scnn/private/methods/termination_criteria.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/metrics.py` & `pyscnn-0.0.8b0/src/scnn/private/metrics.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/__init__.py` & `pyscnn-0.0.8b0/src/scnn/private/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/convex/al/al_mlp.py` & `pyscnn-0.0.8b0/src/scnn/private/models/convex/al/al_mlp.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/convex/convex_mlp.py` & `pyscnn-0.0.8b0/src/scnn/private/models/convex/convex_mlp.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/convex/kernels/direct_kernel.py` & `pyscnn-0.0.8b0/src/scnn/private/models/convex/kernels/direct_kernel.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/convex/kernels/einsum_kernel.py` & `pyscnn-0.0.8b0/src/scnn/private/models/convex/kernels/einsum_kernel.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/convex/operators.py` & `pyscnn-0.0.8b0/src/scnn/private/models/convex/operators.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/decompositions/quadratic_decomposition.py` & `pyscnn-0.0.8b0/src/scnn/private/models/decompositions/quadratic_decomposition.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/linear/l2_regression.py` & `pyscnn-0.0.8b0/src/scnn/private/models/linear/l2_regression.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/linear/logistic_regression.py` & `pyscnn-0.0.8b0/src/scnn/private/models/linear/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/model.py` & `pyscnn-0.0.8b0/src/scnn/private/models/model.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/non_convex/manual/gated_relu_mlp.py` & `pyscnn-0.0.8b0/src/scnn/private/models/non_convex/manual/gated_relu_mlp.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/non_convex/manual/relu_mlp.py` & `pyscnn-0.0.8b0/src/scnn/private/models/non_convex/manual/relu_mlp.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/non_convex/torch/gated_relu_layer.py` & `pyscnn-0.0.8b0/src/scnn/private/models/non_convex/torch/gated_relu_layer.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/non_convex/torch/layer_wrapper.py` & `pyscnn-0.0.8b0/src/scnn/private/models/non_convex/torch/layer_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/non_convex/torch/sequential_wrapper.py` & `pyscnn-0.0.8b0/src/scnn/private/models/non_convex/torch/sequential_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/one_vs_all.py` & `pyscnn-0.0.8b0/src/scnn/private/models/one_vs_all.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/regularizers/__init__.py` & `pyscnn-0.0.8b0/src/scnn/private/models/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/regularizers/constraint.py` & `pyscnn-0.0.8b0/src/scnn/private/models/regularizers/constraint.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/regularizers/feature_group_l1.py` & `pyscnn-0.0.8b0/src/scnn/private/models/regularizers/feature_group_l1.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/regularizers/group_l1.py` & `pyscnn-0.0.8b0/src/scnn/private/models/regularizers/group_l1.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/regularizers/group_l1_orthant.py` & `pyscnn-0.0.8b0/src/scnn/private/models/regularizers/group_l1_orthant.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/regularizers/l1.py` & `pyscnn-0.0.8b0/src/scnn/private/models/regularizers/l1.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/regularizers/l1_squared.py` & `pyscnn-0.0.8b0/src/scnn/private/models/regularizers/l1_squared.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/regularizers/l2.py` & `pyscnn-0.0.8b0/src/scnn/private/models/regularizers/l2.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/regularizers/orthant.py` & `pyscnn-0.0.8b0/src/scnn/private/models/regularizers/orthant.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/regularizers/regularizer.py` & `pyscnn-0.0.8b0/src/scnn/private/models/regularizers/regularizer.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/solution_mappings/__init__.py` & `pyscnn-0.0.8b0/src/scnn/private/models/solution_mappings/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/models/solution_mappings/mlps.py` & `pyscnn-0.0.8b0/src/scnn/private/models/solution_mappings/mlps.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/prox/proximal_ops.py` & `pyscnn-0.0.8b0/src/scnn/private/prox/proximal_ops.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/utils/data/synthetic.py` & `pyscnn-0.0.8b0/src/scnn/private/utils/data/synthetic.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/utils/data/transforms.py` & `pyscnn-0.0.8b0/src/scnn/private/utils/data/transforms.py`

 * *Files 25% similar despite different names*

```diff
@@ -59,15 +59,19 @@
     # safe division by columns
     X_train = np.divide(
         X_train, column_norms, out=np.zeros_like(X_train), where=column_norms != 0
     )
     train_set = (X_train, train_set[1])
 
     if test_set is not None:
-        test_set = (test_set[0] / column_norms, test_set[1])
+        X_test, y_test = test_set
+        np.divide(
+            X_test, column_norms, out=np.zeros_like(X_test), where=column_norms != 0
+        )
+        test_set = (X_test, y_test)
 
     return train_set, test_set, column_norms
 
 
 def train_test_split(X, y, valid_prop=0.2, split_seed=1995):
     """ """
     n = y.shape[0]
```

### Comparing `pyscnn-0.0.7b0/src/scnn/private/utils/linear/direct_solvers.py` & `pyscnn-0.0.8b0/src/scnn/private/utils/linear/direct_solvers.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/utils/linear/iterative_solvers.py` & `pyscnn-0.0.8b0/src/scnn/private/utils/linear/iterative_solvers.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/utils/linear/preconditioners.py` & `pyscnn-0.0.8b0/src/scnn/private/utils/linear/preconditioners.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/private/utils/linear_operators.py` & `pyscnn-0.0.8b0/src/scnn/private/utils/linear_operators.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/regularizers.py` & `pyscnn-0.0.8b0/src/scnn/regularizers.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/solvers.py` & `pyscnn-0.0.8b0/src/scnn/solvers.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/src/scnn/support.py` & `pyscnn-0.0.8b0/src/scnn/support.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/test/test_activations.py` & `pyscnn-0.0.8b0/test/test_activations.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/test/test_optimize.py` & `pyscnn-0.0.8b0/test/test_optimize.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/test/test_regularizers.py` & `pyscnn-0.0.8b0/test/test_regularizers.py`

 * *Files identical despite different names*

### Comparing `pyscnn-0.0.7b0/test/test_solvers.py` & `pyscnn-0.0.8b0/test/test_solvers.py`

 * *Files identical despite different names*

