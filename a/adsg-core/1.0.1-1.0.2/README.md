# Comparing `tmp/adsg-core-1.0.1.tar.gz` & `tmp/adsg_core-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adsg-core-1.0.1.tar", last modified: Tue Mar 26 07:41:10 2024, max compression
+gzip compressed data, was "adsg_core-1.0.2.tar", last modified: Tue May  7 18:18:56 2024, max compression
```

## Comparing `adsg-core-1.0.1.tar` & `adsg_core-1.0.2.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:41:10.623854 adsg-core-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-26 07:41:04.000000 adsg-core-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-03-26 07:41:10.623854 adsg-core-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-03-26 07:41:04.000000 adsg-core-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:41:10.607854 adsg-core-1.0.1/adsg_core/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:41:10.611854 adsg-core-1.0.1/adsg_core/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13405 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/examples/apollo.py
--rw-r--r--   0 runner    (1001) docker     (127)    11146 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/examples/gnc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/func_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:41:10.611854 adsg-core-1.0.1/adsg_core/graph/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31067 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/graph/adsg.py
--rw-r--r--   0 runner    (1001) docker     (127)    10115 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/graph/adsg_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    28185 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/graph/adsg_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    10848 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/graph/choice_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/graph/choices.py
--rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/graph/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/graph/graph_edges.py
--rw-r--r--   0 runner    (1001) docker     (127)     8205 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/graph/incompatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)    27782 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/graph/influence_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:41:10.611854 adsg-core-1.0.1/adsg_core/graph/sup/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/graph/sup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13215 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/graph/sup/dsg.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/graph/sup/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    23921 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/graph/traversal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:41:10.615854 adsg-core-1.0.1/adsg_core/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:41:10.615854 adsg-core-1.0.1/adsg_core/optimization/assign_enc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/assignment_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:41:10.615854 adsg-core-1.0.1/adsg_core/optimization/assign_enc/eager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/eager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:41:10.615854 adsg-core-1.0.1/adsg_core/optimization/assign_enc/eager/encodings/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/eager/encodings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/eager/encodings/direct_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/eager/encodings/group_amount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/eager/encodings/group_element.py
--rw-r--r--   0 runner    (1001) docker     (127)    10027 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/eager/encodings/grouped_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:41:10.615854 adsg-core-1.0.1/adsg_core/optimization/assign_enc/eager/imputation/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/eager/imputation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/eager/imputation/auto_mod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/eager/imputation/closest.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/eager/imputation/constraint_violation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/eager/imputation/delta.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/eager/imputation/first.py
--rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/encoder_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    26589 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:41:10.619854 adsg-core-1.0.1/adsg_core/optimization/assign_enc/enumerating/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/enumerating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/enumerating/ordinal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/enumerating/recursive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:41:10.619854 adsg-core-1.0.1/adsg_core/optimization/assign_enc/lazy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/lazy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:41:10.619854 adsg-core-1.0.1/adsg_core/optimization/assign_enc/lazy/encodings/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/lazy/encodings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10120 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/lazy/encodings/conn_idx.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/lazy/encodings/direct_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    11709 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/lazy/encodings/group_amount.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:41:10.619854 adsg-core-1.0.1/adsg_core/optimization/assign_enc/lazy/imputation/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/lazy/imputation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/lazy/imputation/closest.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/lazy/imputation/constraint_violation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/lazy/imputation/delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/lazy/imputation/first.py
--rw-r--r--   0 runner    (1001) docker     (127)    21837 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/lazy_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)    52697 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:41:10.619854 adsg-core-1.0.1/adsg_core/optimization/assign_enc/patterns/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/patterns/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    35386 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/patterns/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)    17799 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/assign_enc/time_limiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/dv_output_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    46950 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/graph_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:41:10.619854 adsg-core-1.0.1/adsg_core/optimization/hierarchy/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/hierarchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15782 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/hierarchy/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    79099 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/hierarchy/complete.py
--rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/hierarchy/fast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/hierarchy/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/hierarchy/sel_choice.py
--rw-r--r--   0 runner    (1001) docker     (127)    11789 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/problem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:41:10.623854 adsg-core-1.0.1/adsg_core/optimization/sel_choice_enc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/sel_choice_enc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15235 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/sel_choice_enc/brute_force.py
--rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/sel_choice_enc/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/optimization/sel_choice_enc/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-03-26 07:41:04.000000 adsg-core-1.0.1/adsg_core/render.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:41:10.623854 adsg-core-1.0.1/adsg_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-03-26 07:41:10.000000 adsg-core-1.0.1/adsg_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-03-26 07:41:10.000000 adsg-core-1.0.1/adsg_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 07:41:10.000000 adsg-core-1.0.1/adsg_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-26 07:41:10.000000 adsg-core-1.0.1/adsg_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-26 07:41:10.000000 adsg-core-1.0.1/adsg_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-26 07:41:04.000000 adsg-core-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-26 07:41:10.623854 adsg-core-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:56.697445 adsg_core-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-07 18:18:51.000000 adsg_core-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-05-07 18:18:56.697445 adsg_core-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-07 18:18:51.000000 adsg_core-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:56.685444 adsg_core-1.0.2/adsg_core/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:56.685444 adsg_core-1.0.2/adsg_core/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13405 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/examples/apollo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11146 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/examples/gnc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/func_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:56.689444 adsg_core-1.0.2/adsg_core/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31483 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/graph/adsg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/graph/adsg_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28185 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/graph/adsg_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10848 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/graph/choice_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/graph/choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/graph/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/graph/graph_edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8205 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/graph/incompatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27782 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/graph/influence_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:56.689444 adsg_core-1.0.2/adsg_core/graph/sup/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/graph/sup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13215 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/graph/sup/dsg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/graph/sup/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23921 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/graph/traversal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:56.689444 adsg_core-1.0.2/adsg_core/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:56.693445 adsg_core-1.0.2/adsg_core/optimization/assign_enc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/assignment_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:56.693445 adsg_core-1.0.2/adsg_core/optimization/assign_enc/eager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/eager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:56.693445 adsg_core-1.0.2/adsg_core/optimization/assign_enc/eager/encodings/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/eager/encodings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/eager/encodings/direct_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/eager/encodings/group_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/eager/encodings/group_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10027 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/eager/encodings/grouped_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:56.693445 adsg_core-1.0.2/adsg_core/optimization/assign_enc/eager/imputation/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/eager/imputation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/eager/imputation/auto_mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/eager/imputation/closest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/eager/imputation/constraint_violation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/eager/imputation/delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/eager/imputation/first.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/encoder_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26589 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:56.693445 adsg_core-1.0.2/adsg_core/optimization/assign_enc/enumerating/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/enumerating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/enumerating/ordinal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/enumerating/recursive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:56.693445 adsg_core-1.0.2/adsg_core/optimization/assign_enc/lazy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/lazy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:56.693445 adsg_core-1.0.2/adsg_core/optimization/assign_enc/lazy/encodings/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/lazy/encodings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10120 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/lazy/encodings/conn_idx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/lazy/encodings/direct_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11709 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/lazy/encodings/group_amount.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:56.697445 adsg_core-1.0.2/adsg_core/optimization/assign_enc/lazy/imputation/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/lazy/imputation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/lazy/imputation/closest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/lazy/imputation/constraint_violation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/lazy/imputation/delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/lazy/imputation/first.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21837 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/lazy_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52697 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:56.697445 adsg_core-1.0.2/adsg_core/optimization/assign_enc/patterns/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/patterns/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35386 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/patterns/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17799 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/assign_enc/time_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/dv_output_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46950 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/graph_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:56.697445 adsg_core-1.0.2/adsg_core/optimization/hierarchy/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/hierarchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15782 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/hierarchy/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79099 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/hierarchy/complete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/hierarchy/fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/hierarchy/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/hierarchy/sel_choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11789 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/problem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:56.697445 adsg_core-1.0.2/adsg_core/optimization/sel_choice_enc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/sel_choice_enc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15235 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/sel_choice_enc/brute_force.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/sel_choice_enc/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/optimization/sel_choice_enc/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-07 18:18:51.000000 adsg_core-1.0.2/adsg_core/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:56.697445 adsg_core-1.0.2/adsg_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-05-07 18:18:56.000000 adsg_core-1.0.2/adsg_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-07 18:18:56.000000 adsg_core-1.0.2/adsg_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 18:18:56.000000 adsg_core-1.0.2/adsg_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-07 18:18:56.000000 adsg_core-1.0.2/adsg_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-07 18:18:56.000000 adsg_core-1.0.2/adsg_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-07 18:18:51.000000 adsg_core-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-07 18:18:56.701444 adsg_core-1.0.2/setup.cfg
```

### Comparing `adsg-core-1.0.1/LICENSE` & `adsg_core-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/PKG-INFO` & `adsg_core-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adsg-core
-Version: 1.0.1
+Version: 1.0.2
 Summary: Architecture Design Space Graph Core
 Author: Jasper Bussemaker
 Author-email: jasper.bussemaker@dlr.de
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3
```

### Comparing `adsg-core-1.0.1/README.md` & `adsg_core-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/examples/apollo.py` & `adsg_core-1.0.2/adsg_core/examples/apollo.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/examples/gnc.py` & `adsg_core-1.0.2/adsg_core/examples/gnc.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/func_cache.py` & `adsg_core-1.0.2/adsg_core/func_cache.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/graph/adsg.py` & `adsg_core-1.0.2/adsg_core/graph/adsg.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,21 +154,25 @@
         """Export to DOT (use Graphviz / https://viz-js.com/ to view)"""
         export_dot(self._get_graph_for_export(), path, start_nodes=self.derivation_start_nodes)
 
     def export_drawio(self, path):
         """Export to draw.io"""
         export_drawio(self._get_graph_for_export(), path, start_nodes=self.derivation_start_nodes)
 
-    def render(self):
-        from adsg_core.render import render
-        render(self)
+    def render(self, title=None):
+        """Render the ADSG as a graph.
+        Open a webbrowser, or renders it as cell output if used in an IPython/Jupyter notebook."""
+        from adsg_core.render import ADSGRenderer
+        ADSGRenderer(self, title=title).render()
 
-    def render_all(self, idx=None):
-        from adsg_core.render import render_all_instances
-        render_all_instances(self, idx=idx)
+    def render_all(self, idx=None, title=None):
+        """Renders all ADSG instances as a graph (optionally provide only specific indices to render).
+        Open a webbrowser, or renders it as cell output if used in an IPython/Jupyter notebook."""
+        from adsg_core.render import ADSGRenderer
+        ADSGRenderer(self, title=title).render_all_instances(idx=idx)
 
     def _get_graph_for_export(self):
         graph = nx.MultiDiGraph()
         graph.add_edges_from(self._graph.edges(data=True))
         graph.add_nodes_from(self._graph.nodes(data=True))
         self._export_prepare(graph)
         return graph
```

### Comparing `adsg-core-1.0.1/adsg_core/graph/adsg_basic.py` & `adsg_core-1.0.2/adsg_core/graph/adsg_basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,14 +134,18 @@
         for i, option_node in enumerate(option_nodes):
             if option_node.option_id is None:
                 option_node.option_id = i
 
             edges.append((choice_node, option_node))
 
         self.add_edges(edges)
+
+        # Reset influence matrix
+        self._influence_matrix = None
+
         return choice_node
 
     def add_connection_choice(self, choice_id: str, src_nodes: ConnNodes, tgt_nodes: ConnNodes,
                               exclude: List[Tuple[ConnectorNode, ConnectorNode]] = None) -> ConnectionChoiceNode:
         """
         A connection choice is a choice on how to connect one or more source nodes to one or more target nodes.
         Each connector node can place constraints on the accepted connection degree: one or more specific numbers,
```

### Comparing `adsg-core-1.0.1/adsg_core/graph/adsg_nodes.py` & `adsg_core-1.0.2/adsg_core/graph/adsg_nodes.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/graph/choice_constraints.py` & `adsg_core-1.0.2/adsg_core/graph/choice_constraints.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/graph/choices.py` & `adsg_core-1.0.2/adsg_core/graph/choices.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/graph/export.py` & `adsg_core-1.0.2/adsg_core/graph/export.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,21 @@
         if v not in node_id_map:
             node_id_map[v] = i
             i += 1
 
         u_node = get_node(u, node_id_map[u])
         v_node = get_node(v, node_id_map[v])
 
-        attr = d.copy()
+        attr = {}
+        for key, value in d.items():
+            value = str(value)
+            if ':' in value:
+                value = f'\"{value}\"'
+            attr[key] = value
+
         edge_type = get_edge_type((u, v, k, d))
         if edge_type == EdgeType.INCOMPATIBILITY:
             attr['color'] = 'red'
             attr['arrowhead'] = 'none'
             attr['constraint'] = 'false'
 
             if (u, v) in shown_incompatibilities:
```

### Comparing `adsg-core-1.0.1/adsg_core/graph/graph_edges.py` & `adsg_core-1.0.2/adsg_core/graph/graph_edges.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/graph/incompatibility.py` & `adsg_core-1.0.2/adsg_core/graph/incompatibility.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/graph/influence_matrix.py` & `adsg_core-1.0.2/adsg_core/graph/influence_matrix.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/graph/sup/dsg.py` & `adsg_core-1.0.2/adsg_core/graph/sup/dsg.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/graph/sup/nodes.py` & `adsg_core-1.0.2/adsg_core/graph/sup/nodes.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/graph/traversal.py` & `adsg_core-1.0.2/adsg_core/graph/traversal.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/assign_enc/assignment_manager.py` & `adsg_core-1.0.2/adsg_core/optimization/assign_enc/assignment_manager.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/assign_enc/eager/encodings/direct_matrix.py` & `adsg_core-1.0.2/adsg_core/optimization/assign_enc/eager/encodings/direct_matrix.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/assign_enc/eager/encodings/group_amount.py` & `adsg_core-1.0.2/adsg_core/optimization/assign_enc/eager/encodings/group_amount.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/assign_enc/eager/encodings/group_element.py` & `adsg_core-1.0.2/adsg_core/optimization/assign_enc/eager/encodings/group_element.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/assign_enc/eager/encodings/grouped_base.py` & `adsg_core-1.0.2/adsg_core/optimization/assign_enc/eager/encodings/grouped_base.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/assign_enc/eager/imputation/auto_mod.py` & `adsg_core-1.0.2/adsg_core/optimization/assign_enc/eager/imputation/auto_mod.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/assign_enc/eager/imputation/closest.py` & `adsg_core-1.0.2/adsg_core/optimization/assign_enc/eager/imputation/closest.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/assign_enc/eager/imputation/constraint_violation.py` & `adsg_core-1.0.2/adsg_core/optimization/assign_enc/eager/imputation/constraint_violation.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/assign_enc/eager/imputation/delta.py` & `adsg_core-1.0.2/adsg_core/optimization/assign_enc/eager/imputation/delta.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/assign_enc/eager/imputation/first.py` & `adsg_core-1.0.2/adsg_core/optimization/assign_enc/eager/imputation/first.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/assign_enc/encoder_registry.py` & `adsg_core-1.0.2/adsg_core/optimization/assign_enc/encoder_registry.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/assign_enc/encoding.py` & `adsg_core-1.0.2/adsg_core/optimization/assign_enc/encoding.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/assign_enc/enumerating/ordinal.py` & `adsg_core-1.0.2/adsg_core/optimization/assign_enc/enumerating/ordinal.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/assign_enc/enumerating/recursive.py` & `adsg_core-1.0.2/adsg_core/optimization/assign_enc/enumerating/recursive.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/assign_enc/lazy/encodings/conn_idx.py` & `adsg_core-1.0.2/adsg_core/optimization/assign_enc/lazy/encodings/conn_idx.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/assign_enc/lazy/encodings/direct_matrix.py` & `adsg_core-1.0.2/adsg_core/optimization/assign_enc/lazy/encodings/direct_matrix.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/assign_enc/lazy/encodings/group_amount.py` & `adsg_core-1.0.2/adsg_core/optimization/assign_enc/lazy/encodings/group_amount.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/assign_enc/lazy/imputation/closest.py` & `adsg_core-1.0.2/adsg_core/optimization/assign_enc/lazy/imputation/closest.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/assign_enc/lazy/imputation/constraint_violation.py` & `adsg_core-1.0.2/adsg_core/optimization/assign_enc/lazy/imputation/constraint_violation.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/assign_enc/lazy/imputation/delta.py` & `adsg_core-1.0.2/adsg_core/optimization/assign_enc/lazy/imputation/delta.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/assign_enc/lazy/imputation/first.py` & `adsg_core-1.0.2/adsg_core/optimization/assign_enc/lazy/imputation/first.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/assign_enc/lazy_encoding.py` & `adsg_core-1.0.2/adsg_core/optimization/assign_enc/lazy_encoding.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/assign_enc/matrix.py` & `adsg_core-1.0.2/adsg_core/optimization/assign_enc/matrix.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/assign_enc/patterns/encoder.py` & `adsg_core-1.0.2/adsg_core/optimization/assign_enc/patterns/encoder.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/assign_enc/patterns/patterns.py` & `adsg_core-1.0.2/adsg_core/optimization/assign_enc/patterns/patterns.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/assign_enc/selector.py` & `adsg_core-1.0.2/adsg_core/optimization/assign_enc/selector.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/assign_enc/time_limiter.py` & `adsg_core-1.0.2/adsg_core/optimization/assign_enc/time_limiter.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/dv_output_defs.py` & `adsg_core-1.0.2/adsg_core/optimization/dv_output_defs.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/evaluator.py` & `adsg_core-1.0.2/adsg_core/optimization/evaluator.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/graph_processor.py` & `adsg_core-1.0.2/adsg_core/optimization/graph_processor.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/hierarchy/base.py` & `adsg_core-1.0.2/adsg_core/optimization/hierarchy/base.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/hierarchy/complete.py` & `adsg_core-1.0.2/adsg_core/optimization/hierarchy/complete.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/hierarchy/fast.py` & `adsg_core-1.0.2/adsg_core/optimization/hierarchy/fast.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/hierarchy/registry.py` & `adsg_core-1.0.2/adsg_core/optimization/hierarchy/registry.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/hierarchy/sel_choice.py` & `adsg_core-1.0.2/adsg_core/optimization/hierarchy/sel_choice.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/problem.py` & `adsg_core-1.0.2/adsg_core/optimization/problem.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/sel_choice_enc/brute_force.py` & `adsg_core-1.0.2/adsg_core/optimization/sel_choice_enc/brute_force.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/sel_choice_enc/encoder.py` & `adsg_core-1.0.2/adsg_core/optimization/sel_choice_enc/encoder.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core/optimization/sel_choice_enc/util.py` & `adsg_core-1.0.2/adsg_core/optimization/sel_choice_enc/util.py`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/adsg_core.egg-info/PKG-INFO` & `adsg_core-1.0.2/adsg_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adsg-core
-Version: 1.0.1
+Version: 1.0.2
 Summary: Architecture Design Space Graph Core
 Author: Jasper Bussemaker
 Author-email: jasper.bussemaker@dlr.de
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3
```

### Comparing `adsg-core-1.0.1/adsg_core.egg-info/SOURCES.txt` & `adsg_core-1.0.2/adsg_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adsg-core-1.0.1/setup.cfg` & `adsg_core-1.0.2/setup.cfg`

 * *Files identical despite different names*

