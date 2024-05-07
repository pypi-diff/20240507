# Comparing `tmp/tnreason-0.2.5.tar.gz` & `tmp/tnreason-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tnreason-0.2.5.tar", last modified: Mon Feb 12 13:19:50 2024, max compression
+gzip compressed data, was "dist/tnreason-1.0.0.tar", last modified: Tue May  7 12:32:51 2024, max compression
```

## Comparing `tnreason-0.2.5.tar` & `tnreason-1.0.0.tar`

### file list

```diff
@@ -1,87 +1,49 @@
-drwxr-xr-x   0 alexgoessmann   (501) staff       (20)        0 2024-02-12 13:19:50.461475 tnreason-0.2.5/
--rw-r--r--   0 alexgoessmann   (501) staff       (20)    34522 2023-11-24 08:23:17.000000 tnreason-0.2.5/LICENSE
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     1068 2024-02-12 13:19:50.460739 tnreason-0.2.5/PKG-INFO
--rw-r--r--   0 alexgoessmann   (501) staff       (20)      236 2024-01-16 14:34:38.000000 tnreason-0.2.5/README.md
--rw-r--r--   0 alexgoessmann   (501) staff       (20)       38 2024-02-12 13:19:50.461670 tnreason-0.2.5/setup.cfg
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     1081 2024-02-12 13:19:35.000000 tnreason-0.2.5/setup.py
-drwxr-xr-x   0 alexgoessmann   (501) staff       (20)        0 2024-02-12 13:19:50.386490 tnreason-0.2.5/tnreason/
--rw-r--r--   0 alexgoessmann   (501) staff       (20)       22 2024-02-07 09:01:09.000000 tnreason-0.2.5/tnreason/__init__.py
-drwxr-xr-x   0 alexgoessmann   (501) staff       (20)        0 2024-02-12 13:19:50.424628 tnreason-0.2.5/tnreason/contraction/
--rw-r--r--   0 alexgoessmann   (501) staff       (20)      485 2024-02-12 13:15:07.000000 tnreason-0.2.5/tnreason/contraction/__init__.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     6364 2024-01-15 16:43:36.000000 tnreason-0.2.5/tnreason/contraction/bc_contraction_generation.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     8358 2023-12-10 16:28:02.000000 tnreason-0.2.5/tnreason/contraction/contraction_optimization.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     2561 2024-01-19 09:51:54.000000 tnreason-0.2.5/tnreason/contraction/contraction_visualization.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)    14574 2024-02-06 16:18:58.000000 tnreason-0.2.5/tnreason/contraction/core_contractor.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     2889 2023-12-13 17:48:58.000000 tnreason-0.2.5/tnreason/contraction/expression_evaluation.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     2399 2024-02-12 08:05:15.000000 tnreason-0.2.5/tnreason/contraction/generic_cores.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     2333 2024-01-03 13:26:29.000000 tnreason-0.2.5/tnreason/contraction/layered_contraction_generation.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     2208 2024-01-03 13:23:55.000000 tnreason-0.2.5/tnreason/contraction/layered_core_contractor.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     1515 2024-01-03 09:39:52.000000 tnreason-0.2.5/tnreason/contraction/layers.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     1084 2024-02-12 13:01:02.000000 tnreason-0.2.5/tnreason/contraction/pgmpy_contractor.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     3755 2024-01-22 13:40:04.000000 tnreason-0.2.5/tnreason/contraction/stub_tree_contraction.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     3565 2024-02-05 08:35:58.000000 tnreason-0.2.5/tnreason/contraction/stub_variable_elimination.py
-drwxr-xr-x   0 alexgoessmann   (501) staff       (20)        0 2024-02-12 13:19:50.429709 tnreason-0.2.5/tnreason/knowledge/
--rw-r--r--   0 alexgoessmann   (501) staff       (20)      251 2024-01-30 07:24:00.000000 tnreason-0.2.5/tnreason/knowledge/__init__.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     2332 2024-01-19 18:28:08.000000 tnreason-0.2.5/tnreason/knowledge/hard_kb.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     8345 2024-02-07 08:53:15.000000 tnreason-0.2.5/tnreason/knowledge/hybrid_kb.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     1908 2024-01-19 19:08:58.000000 tnreason-0.2.5/tnreason/knowledge/soft_kb.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)      243 2024-01-30 07:09:57.000000 tnreason-0.2.5/tnreason/knowledge/storage.py
-drwxr-xr-x   0 alexgoessmann   (501) staff       (20)        0 2024-02-12 13:19:50.433531 tnreason-0.2.5/tnreason/learning/
--rw-r--r--   0 alexgoessmann   (501) staff       (20)        0 2023-11-24 08:59:00.000000 tnreason-0.2.5/tnreason/learning/__init__.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)    11169 2023-12-14 15:03:59.000000 tnreason-0.2.5/tnreason/learning/expression_learning.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     4552 2024-02-07 10:51:35.000000 tnreason-0.2.5/tnreason/learning/formula_sampling.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     4209 2024-02-06 10:31:42.000000 tnreason-0.2.5/tnreason/learning/mle_integrated_learning.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     9031 2024-01-12 09:06:24.000000 tnreason-0.2.5/tnreason/learning/mln_learning.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     2985 2024-01-22 14:51:40.000000 tnreason-0.2.5/tnreason/learning/stub_clause_learner.py
-drwxr-xr-x   0 alexgoessmann   (501) staff       (20)        0 2024-02-12 13:19:50.436200 tnreason-0.2.5/tnreason/logic/
--rw-r--r--   0 alexgoessmann   (501) staff       (20)        0 2023-11-24 08:56:13.000000 tnreason-0.2.5/tnreason/logic/__init__.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     4868 2023-12-12 13:29:10.000000 tnreason-0.2.5/tnreason/logic/basis_calculus.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     9475 2024-02-12 08:13:02.000000 tnreason-0.2.5/tnreason/logic/coordinate_calculus.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     5310 2023-12-13 18:15:16.000000 tnreason-0.2.5/tnreason/logic/expression_calculus.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     3979 2024-02-09 10:42:04.000000 tnreason-0.2.5/tnreason/logic/expression_generation.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     4102 2024-02-05 11:10:59.000000 tnreason-0.2.5/tnreason/logic/expression_simplification.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     4857 2024-02-09 12:55:01.000000 tnreason-0.2.5/tnreason/logic/expression_utils.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     2799 2023-11-21 15:34:28.000000 tnreason-0.2.5/tnreason/logic/expression_visualization.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     2876 2023-11-22 11:50:29.000000 tnreason-0.2.5/tnreason/logic/optimization_calculus.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)      442 2023-11-21 15:34:28.000000 tnreason-0.2.5/tnreason/logic/sparse_cc.py
-drwxr-xr-x   0 alexgoessmann   (501) staff       (20)        0 2024-02-12 13:19:50.447308 tnreason-0.2.5/tnreason/model/
--rw-r--r--   0 alexgoessmann   (501) staff       (20)        0 2023-11-24 08:59:00.000000 tnreason-0.2.5/tnreason/model/__init__.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)    11774 2024-02-09 10:55:40.000000 tnreason-0.2.5/tnreason/model/create_cores.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     1610 2024-01-12 16:49:14.000000 tnreason-0.2.5/tnreason/model/entropies.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     7088 2024-02-12 13:12:18.000000 tnreason-0.2.5/tnreason/model/formula_tensors.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)      669 2024-01-09 19:38:07.000000 tnreason-0.2.5/tnreason/model/generate_test_data.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)    10662 2024-02-05 17:14:48.000000 tnreason-0.2.5/tnreason/model/logic_model.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     6021 2024-01-30 12:33:31.000000 tnreason-0.2.5/tnreason/model/model_visualization.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     3693 2024-02-01 12:40:02.000000 tnreason-0.2.5/tnreason/model/polynomial_model.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)    14602 2024-02-12 13:05:09.000000 tnreason-0.2.5/tnreason/model/sampling.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     6875 2024-02-12 08:17:39.000000 tnreason-0.2.5/tnreason/model/superposed_formula_tensors.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     6652 2024-02-06 17:33:45.000000 tnreason-0.2.5/tnreason/model/tensor_model.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     5856 2024-01-10 10:58:30.000000 tnreason-0.2.5/tnreason/model/tensor_network_mln.py
-drwxr-xr-x   0 alexgoessmann   (501) staff       (20)        0 2024-02-12 13:19:50.452227 tnreason-0.2.5/tnreason/optimization/
--rw-r--r--   0 alexgoessmann   (501) staff       (20)        0 2023-11-24 08:59:00.000000 tnreason-0.2.5/tnreason/optimization/__init__.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)    13817 2024-01-22 14:41:13.000000 tnreason-0.2.5/tnreason/optimization/alternating_mle.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     5901 2024-02-12 13:15:56.000000 tnreason-0.2.5/tnreason/optimization/entropy_maximization.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     1199 2023-12-13 16:26:44.000000 tnreason-0.2.5/tnreason/optimization/expression_refinement.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     6018 2023-12-14 13:46:07.000000 tnreason-0.2.5/tnreason/optimization/generalized_als.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     2499 2023-12-13 16:27:19.000000 tnreason-0.2.5/tnreason/optimization/satisfaction_counter.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     9131 2024-01-30 08:08:18.000000 tnreason-0.2.5/tnreason/optimization/weight_estimation.py
-drwxr-xr-x   0 alexgoessmann   (501) staff       (20)        0 2024-02-12 13:19:50.457651 tnreason-0.2.5/tnreason/probability/
--rw-r--r--   0 alexgoessmann   (501) staff       (20)        0 2024-02-12 09:29:14.000000 tnreason-0.2.5/tnreason/probability/__init__.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)      248 2024-02-12 09:46:06.000000 tnreason-0.2.5/tnreason/probability/distributions.py
-drwxr-xr-x   0 alexgoessmann   (501) staff       (20)        0 2024-02-12 13:19:50.458525 tnreason-0.2.5/tnreason/representation/
--rw-r--r--   0 alexgoessmann   (501) staff       (20)        0 2023-11-24 08:59:00.000000 tnreason-0.2.5/tnreason/representation/__init__.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)      467 2023-11-21 15:34:28.000000 tnreason-0.2.5/tnreason/representation/csv_to_ttl.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     2631 2023-11-21 15:34:28.000000 tnreason-0.2.5/tnreason/representation/factdf_to_cores.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)      828 2023-11-21 15:34:28.000000 tnreason-0.2.5/tnreason/representation/pairdf_to_cores.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     3950 2024-02-08 19:16:02.000000 tnreason-0.2.5/tnreason/representation/pgmpy_inference.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     1668 2023-12-21 16:24:50.000000 tnreason-0.2.5/tnreason/representation/sampledf_to_cores.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     1563 2023-11-21 15:34:28.000000 tnreason-0.2.5/tnreason/representation/sampledf_to_factdf.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)      830 2023-11-21 15:34:28.000000 tnreason-0.2.5/tnreason/representation/sampledf_to_pairdf.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     2515 2023-12-12 13:11:19.000000 tnreason-0.2.5/tnreason/representation/sparse_generator.py
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     1364 2023-11-21 15:34:28.000000 tnreason-0.2.5/tnreason/representation/ttl_to_csv.py
-drwxr-xr-x   0 alexgoessmann   (501) staff       (20)        0 2024-02-12 13:19:50.411481 tnreason-0.2.5/tnreason.egg-info/
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     1068 2024-02-12 13:19:49.000000 tnreason-0.2.5/tnreason.egg-info/PKG-INFO
--rw-r--r--   0 alexgoessmann   (501) staff       (20)     3748 2024-02-12 13:19:50.000000 tnreason-0.2.5/tnreason.egg-info/SOURCES.txt
--rw-r--r--   0 alexgoessmann   (501) staff       (20)        1 2024-02-12 13:19:49.000000 tnreason-0.2.5/tnreason.egg-info/dependency_links.txt
--rw-r--r--   0 alexgoessmann   (501) staff       (20)       60 2024-02-12 13:19:49.000000 tnreason-0.2.5/tnreason.egg-info/requires.txt
--rw-r--r--   0 alexgoessmann   (501) staff       (20)        9 2024-02-12 13:19:49.000000 tnreason-0.2.5/tnreason.egg-info/top_level.txt
+drwxr-xr-x   0 alexgoessmann   (501) staff       (20)        0 2024-05-07 12:32:51.315369 tnreason-1.0.0/
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)    34522 2024-02-21 05:34:38.000000 tnreason-1.0.0/LICENSE
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     1161 2024-05-07 12:32:51.314604 tnreason-1.0.0/PKG-INFO
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)      236 2024-02-21 05:34:38.000000 tnreason-1.0.0/README.md
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)       38 2024-05-07 12:32:51.315536 tnreason-1.0.0/setup.cfg
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     1169 2024-05-07 12:31:45.000000 tnreason-1.0.0/setup.py
+drwxr-xr-x   0 alexgoessmann   (501) staff       (20)        0 2024-05-07 12:32:51.284774 tnreason-1.0.0/tnreason/
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)      385 2024-05-06 15:34:18.000000 tnreason-1.0.0/tnreason/__init__.py
+drwxr-xr-x   0 alexgoessmann   (501) staff       (20)        0 2024-05-07 12:32:51.291510 tnreason-1.0.0/tnreason/algorithms/
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)      263 2024-05-07 12:06:31.000000 tnreason-1.0.0/tnreason/algorithms/__init__.py
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     6486 2024-05-07 11:50:55.000000 tnreason-1.0.0/tnreason/algorithms/alternating_least_squares.py
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     4368 2024-05-07 12:23:03.000000 tnreason-1.0.0/tnreason/algorithms/binary_propagation.py
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     5334 2024-05-07 12:14:22.000000 tnreason-1.0.0/tnreason/algorithms/constraint_propagation.py
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     4584 2024-05-07 12:06:31.000000 tnreason-1.0.0/tnreason/algorithms/gibbs_sampling.py
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     3060 2024-05-07 12:23:03.000000 tnreason-1.0.0/tnreason/algorithms/moment_matching.py
+drwxr-xr-x   0 alexgoessmann   (501) staff       (20)        0 2024-05-07 12:32:51.298062 tnreason-1.0.0/tnreason/encoding/
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)      799 2024-05-07 11:46:34.000000 tnreason-1.0.0/tnreason/encoding/__init__.py
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     1301 2024-05-07 11:46:34.000000 tnreason-1.0.0/tnreason/encoding/auxiliary_cores.py
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)      983 2024-05-07 08:42:12.000000 tnreason-1.0.0/tnreason/encoding/categoricals_to_cores.py
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     1003 2024-05-07 08:42:12.000000 tnreason-1.0.0/tnreason/encoding/data_to_cores.py
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     6451 2024-05-07 08:42:12.000000 tnreason-1.0.0/tnreason/encoding/formulas_to_cores.py
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     6510 2024-05-07 08:42:12.000000 tnreason-1.0.0/tnreason/encoding/neurons_to_cores.py
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)      240 2024-05-07 07:38:38.000000 tnreason-1.0.0/tnreason/encoding/storage.py
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     1887 2024-04-06 11:01:47.000000 tnreason-1.0.0/tnreason/encoding/truth_tables.py
+drwxr-xr-x   0 alexgoessmann   (501) staff       (20)        0 2024-05-07 12:32:51.305835 tnreason-1.0.0/tnreason/engine/
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     2139 2024-05-07 12:28:05.000000 tnreason-1.0.0/tnreason/engine/__init__.py
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     1408 2024-04-16 09:12:04.000000 tnreason-1.0.0/tnreason/engine/engine_visualization.py
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     2502 2024-04-19 06:53:26.000000 tnreason-1.0.0/tnreason/engine/slice_contractor.py
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     1352 2024-05-07 06:36:45.000000 tnreason-1.0.0/tnreason/engine/subscript_creation.py
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     2184 2024-05-07 06:52:47.000000 tnreason-1.0.0/tnreason/engine/workload_to_numpy.py
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     1207 2024-05-07 06:52:47.000000 tnreason-1.0.0/tnreason/engine/workload_to_pgmpy.py
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     1147 2024-05-07 06:56:54.000000 tnreason-1.0.0/tnreason/engine/workload_to_tensorflow.py
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     2845 2024-05-07 07:04:08.000000 tnreason-1.0.0/tnreason/engine/workload_to_tentris.py
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     1252 2024-05-07 06:56:54.000000 tnreason-1.0.0/tnreason/engine/workload_to_torch.py
+drwxr-xr-x   0 alexgoessmann   (501) staff       (20)        0 2024-05-07 12:32:51.313143 tnreason-1.0.0/tnreason/knowledge/
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)      599 2024-05-03 13:09:46.000000 tnreason-1.0.0/tnreason/knowledge/__init__.py
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     1743 2024-05-06 17:00:59.000000 tnreason-1.0.0/tnreason/knowledge/batch_evaluation.py
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     3157 2024-05-07 07:44:04.000000 tnreason-1.0.0/tnreason/knowledge/deductive.py
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     5528 2024-05-07 07:38:38.000000 tnreason-1.0.0/tnreason/knowledge/distributions.py
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     4516 2024-05-07 10:56:15.000000 tnreason-1.0.0/tnreason/knowledge/formula_boosting.py
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     3271 2024-05-06 16:12:44.000000 tnreason-1.0.0/tnreason/knowledge/inductive.py
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     7106 2024-05-07 08:07:17.000000 tnreason-1.0.0/tnreason/knowledge/knowledge_visualization.py
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     3343 2024-05-07 08:10:47.000000 tnreason-1.0.0/tnreason/knowledge/weight_estimation.py
+drwxr-xr-x   0 alexgoessmann   (501) staff       (20)        0 2024-05-07 12:32:51.287076 tnreason-1.0.0/tnreason.egg-info/
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     1161 2024-05-07 12:32:50.000000 tnreason-1.0.0/tnreason.egg-info/PKG-INFO
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)     1366 2024-05-07 12:32:51.000000 tnreason-1.0.0/tnreason.egg-info/SOURCES.txt
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)        1 2024-05-07 12:32:50.000000 tnreason-1.0.0/tnreason.egg-info/dependency_links.txt
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)       86 2024-05-07 12:32:50.000000 tnreason-1.0.0/tnreason.egg-info/requires.txt
+-rw-r--r--   0 alexgoessmann   (501) staff       (20)        9 2024-05-07 12:32:50.000000 tnreason-1.0.0/tnreason.egg-info/top_level.txt
```

### Comparing `tnreason-0.2.5/LICENSE` & `tnreason-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tnreason-0.2.5/setup.py` & `tnreason-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name="tnreason",
-    version="0.2.5",
+    version="1.0.0",
     author="Alex Goessmann",
     author_email="alex.goessmann@web.de",
-    description="A package for reasoning with tensors",
+    description="A package for reasoning based on encoding networks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering :: Artificial Intelligence"
     ],
     install_requires=[
-        "numpy>=1.17", # was 1.23.4",
+        "numpy>=1.17",  # was 1.23.4",
         "pandas>=1.0.0",
         "networkx",
         "pyyaml",
         "rdflib",
-        "matplotlib"
+        "matplotlib",
+        "pgmpy",
+        "importlib-resources"
     ],
     python_requires=">=3",
     license="AGPL-3.0",
     url="https://github.com/EnexaProject/enexa-tensor-reasoning",
-    keywords="inductive reasoning, tensor networks, alternating least squares, markov logic networks"
-)
+    keywords="markov logic networks, tensor networks, alternating least squares, gibbs sampling, inductive logic programming"
+)
```

### Comparing `tnreason-0.2.5/tnreason/contraction/layered_core_contractor.py` & `tnreason-1.0.0/tnreason/engine/slice_contractor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,86 @@
-from tnreason.contraction import layers as lay
-from tnreason.contraction import layered_contraction_generation as lcg
+class SliceCore:
+    def __init__(self, values, colors, name=None):
+        self.values = values
+        self.colors = colors
+        self.name = name
+
+    def __str__(self):
+        return "## Sliced Core " + str(self.name) + " ##\nValues: " + str(self.values) + "\nColors: " + str(self.colors)
 
-class LayeredCoreContractor:
 
-    def __init__(self, layerDict={}, layerList=None, instructionList=None, openColors=[]):
-        self.layerDict = layerDict
-        self.layerList = layerList
-
-        self.instructionList = instructionList
+class SliceContractor:
+    def __init__(self, coreDict={}, openColors=[]):
+        self.coreDict = coreDict
         self.openColors = openColors
 
     def contract(self):
-        contracted = self.layerDict[self.instructionList[0][1]]
-        for instruction in self.instructionList[1:]:
-            if instruction[0] == "add":
-                contracted = lay.contract(contracted, self.layerDict[instruction[1]])
-            elif instruction[0] == "reduce":
-                contracted = contracted.reduce_color(instruction[1])
-        return contracted
-
-    ## From analogous method in standard CoreContractor
-    def create_instructionList_from_layerList(self):
-
-        # Find all colors
-        colorList = []
-        for key in self.layerDict:
-            for color in self.layerDict[key].colors:
-                if color not in colorList and color not in self.openColors:
-                    colorList.append(color)
-
-        # Find cores after which color can be reduced
-        self.layerList = list(self.layerList)
-        self.layerList.reverse()
-        reduceDict = {key: [] for key in self.layerDict}
-        for color in colorList:
-            if color not in self.openColors:
-                for key in self.layerList:
-                    if color in self.layerDict[key].colors:
-                        reduceDict[key].append(color)
-                        break
-        self.layerList.reverse()
-
-        # Create the instructionList
-        self.instructionList = []
-        for key in reduceDict:
-            self.instructionList.append(["add", key])
-            for color in reduceDict[key]:
-                self.instructionList.append(["reduce", color])
+        allColors = set()
+        for key in self.coreDict:
+            allColors = allColors | set(self.coreDict[key].colors)
+
+        values = [(1, set(), set())]
+        for key in self.coreDict:
+            values = slice_contraction(values, self.coreDict[key].values)
+        values = reduce_colors(values, allColors - set(self.openColors))
+        return SliceCore(values, self.openColors)
+
+
+def reduce_colors(values, reduceColors):
+    reducedValues = []
+    for val, pos, neg in values:
+        for reduceColor in reduceColors:
+            if reduceColor not in pos and reduceColor not in neg:
+                val = 2 * val  # Color dimension always 2
+            elif reduceColor in pos:
+                pos.remove(reduceColor)
+            elif reduceColor in neg:
+                neg.remove(reduceColor)
+            else:
+                print(reduceColor, pos, neg, reduceColor in pos, reduceColor in neg)
+        reducedValues.append((val, pos, neg))
+    return reducedValues
+
+
+def slice_contraction(values1, values2):
+    slices = []
+    for slice1 in values1:
+        for slice2 in values2:
+            combined = combine_slices(slice1, slice2)
+            if combined[0] != 0:
+                slices.append(combined)
+    return slices
+
+
+def combine_slices(slice1, slice2):
+    val1, pos1, neg1 = slice1
+    val2, pos2, neg2 = slice2
+
+    pos = pos1 | pos2
+    neg = neg1 | neg2
+    if len(pos & neg) > 0:  ## Check whether the slice zero
+        return (0, [], [])
+    else:
+        return (val1 * val2, pos, neg)
+
 
 if __name__ == "__main__":
-    layDict = lcg.generate_skeletonLayerDict(["a","and",["not","b"]], {"a": 2, "b": 10}, 4)
-    contractor = LayeredCoreContractor(layDict, list(layDict.keys()))
-    contractor.create_instructionList_from_layerList()
-    print(contractor.contract().coresDict)
+    values1 = [
+        (1.1, {"a", "b"}, {"c"}),
+        (0.9, set(), {"d"})
+    ]
+    core1 = SliceCore(values1, ["a", "b", "c"])
+
+    values2 = [
+        (1.1, {"b"}, {"a", "c"}),
+        (2, {"a"}, set())
+    ]
+    core2 = SliceCore(values2, ["a", "b", "c"])
+
+    contracted = SliceContractor(coreDict={
+        "c1": core1,
+        "c2": core2
+    }, openColors=["a", "b"]).contract()
+
+    print(contracted)
+
+    # print([e for e in slice_contraction(values1, values2)])
```

### Comparing `tnreason-0.2.5/tnreason/contraction/pgmpy_contractor.py` & `tnreason-1.0.0/tnreason/engine/workload_to_pgmpy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from pgmpy.models import MarkovNetwork
 from pgmpy.factors.discrete import DiscreteFactor
 from pgmpy.inference import VariableElimination
 
-from tnreason.logic import coordinate_calculus as cc
-
+from tnreason.engine import workload_to_numpy as cor
 
 class PgmpyVariableEliminator:
+    """
+    Executed Contractions using the Variable Elimination Algorithm in Pgmpy.
+    Outputs by default a Numpy Core
+    """
     def __init__(self, coreDict={}, openColors=[]):
         self.model = MarkovNetwork()
         self.add_factors_from_coresDict(coreDict)
 
         self.openColors = openColors
 
     def add_factors_from_coresDict(self, coresDict):
@@ -21,8 +24,8 @@
                         self.model.add_edge(col1, col2)
             self.model.add_factors(
                 DiscreteFactor(coresDict[coreKey].colors, coresDict[coreKey].values.shape, coresDict[coreKey].values)
             )
 
     def contract(self):
         result = VariableElimination(self.model).query(evidence={}, variables=self.openColors)
-        return cc.CoordinateCore(result.values, result.variables)
+        return cor.NumpyCore(result.values, result.variables)
```

