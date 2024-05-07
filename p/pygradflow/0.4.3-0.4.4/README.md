# Comparing `tmp/pygradflow-0.4.3.tar.gz` & `tmp/pygradflow-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygradflow-0.4.3.tar", max compression
+gzip compressed data, was "pygradflow-0.4.4.tar", max compression
```

## Comparing `pygradflow-0.4.3.tar` & `pygradflow-0.4.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    10847 2024-05-07 15:14:03.094458 pygradflow-0.4.3/LICENSE
--rw-r--r--   0        0        0      984 2024-05-07 15:14:03.094458 pygradflow-0.4.3/README.md
--rw-r--r--   0        0        0        0 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/__init__.py
--rw-r--r--   0        0        0      872 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/active_set.py
--rw-r--r--   0        0        0     4458 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/cons_problem.py
--rw-r--r--   0        0        0     1749 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/controller.py
--rw-r--r--   0        0        0     2487 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/deriv_check.py
--rw-r--r--   0        0        0     4645 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/display.py
--rw-r--r--   0        0        0     4839 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/eval.py
--rw-r--r--   0        0        0     6380 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/implicit_func.py
--rw-r--r--   0        0        0     5146 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/iterate.py
--rw-r--r--   0        0        0       55 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/log.py
--rw-r--r--   0        0        0     6570 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/newton.py
--rw-r--r--   0        0        0     5173 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/params.py
--rw-r--r--   0        0        0     5111 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/penalty.py
--rw-r--r--   0        0        0     5845 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/problem.py
--rw-r--r--   0        0        0        0 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/py.typed
--rw-r--r--   0        0        0     3378 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/runners/cutest_runner.py
--rw-r--r--   0        0        0      366 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/runners/instance.py
--rw-r--r--   0        0        0     2045 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/runners/qplib_runner.py
--rw-r--r--   0        0        0     7792 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/runners/runner.py
--rw-r--r--   0        0        0     4181 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/scale.py
--rw-r--r--   0        0        0    16537 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/solver.py
--rw-r--r--   0        0        0     1284 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/__init__.py
--rw-r--r--   0        0        0     4439 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/asymmetric_step_solver.py
--rw-r--r--   0        0        0     5790 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/box_control.py
--rw-r--r--   0        0        0     2710 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/cond_estimate.py
--rw-r--r--   0        0        0     2431 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/distance_ratio_control.py
--rw-r--r--   0        0        0     2058 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/exact_control.py
--rw-r--r--   0        0        0     3173 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/extended_step_solver.py
--rw-r--r--   0        0        0      543 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/fixed_control.py
--rw-r--r--   0        0        0     2669 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/linear_solver.py
--rw-r--r--   0        0        0     7241 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/opti_control.py
--rw-r--r--   0        0        0     2014 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/residuum_ratio_control.py
--rw-r--r--   0        0        0     2401 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/scaled_step_solver.py
--rw-r--r--   0        0        0     2467 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/standard_step_solver.py
--rw-r--r--   0        0        0     4697 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/step_control.py
--rw-r--r--   0        0        0     2048 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/step_solver.py
--rw-r--r--   0        0        0     4120 2024-05-07 15:14:03.098458 pygradflow-0.4.3/pygradflow/step/symmetric_step_solver.py
--rw-r--r--   0        0        0      380 2024-05-07 15:14:03.098458 pygradflow-0.4.3/pygradflow/timer.py
--rw-r--r--   0        0        0     1711 2024-05-07 15:14:03.098458 pygradflow-0.4.3/pygradflow/transform.py
--rw-r--r--   0        0        0      232 2024-05-07 15:14:03.098458 pygradflow-0.4.3/pygradflow/util.py
--rw-r--r--   0        0        0     1138 2024-05-07 15:14:03.098458 pygradflow-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     1983 1970-01-01 00:00:00.000000 pygradflow-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    10847 2024-05-07 19:36:13.809971 pygradflow-0.4.4/LICENSE
+-rw-r--r--   0        0        0      984 2024-05-07 19:36:13.809971 pygradflow-0.4.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/__init__.py
+-rw-r--r--   0        0        0      872 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/active_set.py
+-rw-r--r--   0        0        0     4458 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/cons_problem.py
+-rw-r--r--   0        0        0     1749 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/controller.py
+-rw-r--r--   0        0        0     2487 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/deriv_check.py
+-rw-r--r--   0        0        0     4645 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/display.py
+-rw-r--r--   0        0        0     4839 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/eval.py
+-rw-r--r--   0        0        0     6380 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/implicit_func.py
+-rw-r--r--   0        0        0     5146 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/iterate.py
+-rw-r--r--   0        0        0       55 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/log.py
+-rw-r--r--   0        0        0     6570 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/newton.py
+-rw-r--r--   0        0        0     5173 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/params.py
+-rw-r--r--   0        0        0     5111 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/penalty.py
+-rw-r--r--   0        0        0     5845 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/problem.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/py.typed
+-rw-r--r--   0        0        0     3378 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/runners/cutest_runner.py
+-rw-r--r--   0        0        0      366 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/runners/instance.py
+-rw-r--r--   0        0        0     2045 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/runners/qplib_runner.py
+-rw-r--r--   0        0        0     7843 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/runners/runner.py
+-rw-r--r--   0        0        0     4181 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/scale.py
+-rw-r--r--   0        0        0    16537 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/solver.py
+-rw-r--r--   0        0        0     1284 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/__init__.py
+-rw-r--r--   0        0        0     4439 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/asymmetric_step_solver.py
+-rw-r--r--   0        0        0     5790 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/box_control.py
+-rw-r--r--   0        0        0     2710 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/cond_estimate.py
+-rw-r--r--   0        0        0     2431 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/distance_ratio_control.py
+-rw-r--r--   0        0        0     2058 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/exact_control.py
+-rw-r--r--   0        0        0     3173 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/extended_step_solver.py
+-rw-r--r--   0        0        0      543 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/fixed_control.py
+-rw-r--r--   0        0        0     2669 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/linear_solver.py
+-rw-r--r--   0        0        0     7241 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/opti_control.py
+-rw-r--r--   0        0        0     2014 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/residuum_ratio_control.py
+-rw-r--r--   0        0        0     2401 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/scaled_step_solver.py
+-rw-r--r--   0        0        0     2467 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/standard_step_solver.py
+-rw-r--r--   0        0        0     4697 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/step_control.py
+-rw-r--r--   0        0        0     2048 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/step_solver.py
+-rw-r--r--   0        0        0     4120 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/symmetric_step_solver.py
+-rw-r--r--   0        0        0      380 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/timer.py
+-rw-r--r--   0        0        0     1711 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/transform.py
+-rw-r--r--   0        0        0      232 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/util.py
+-rw-r--r--   0        0        0     1138 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     1983 1970-01-01 00:00:00.000000 pygradflow-0.4.4/PKG-INFO
```

### Comparing `pygradflow-0.4.3/LICENSE` & `pygradflow-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/README.md` & `pygradflow-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/active_set.py` & `pygradflow-0.4.4/pygradflow/active_set.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/cons_problem.py` & `pygradflow-0.4.4/pygradflow/cons_problem.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/controller.py` & `pygradflow-0.4.4/pygradflow/controller.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/deriv_check.py` & `pygradflow-0.4.4/pygradflow/deriv_check.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/display.py` & `pygradflow-0.4.4/pygradflow/display.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/eval.py` & `pygradflow-0.4.4/pygradflow/eval.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/implicit_func.py` & `pygradflow-0.4.4/pygradflow/implicit_func.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/iterate.py` & `pygradflow-0.4.4/pygradflow/iterate.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/newton.py` & `pygradflow-0.4.4/pygradflow/newton.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/params.py` & `pygradflow-0.4.4/pygradflow/params.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/penalty.py` & `pygradflow-0.4.4/pygradflow/penalty.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/problem.py` & `pygradflow-0.4.4/pygradflow/problem.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/runners/cutest_runner.py` & `pygradflow-0.4.4/pygradflow/runners/cutest_runner.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/runners/qplib_runner.py` & `pygradflow-0.4.4/pygradflow/runners/qplib_runner.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/runners/runner.py` & `pygradflow-0.4.4/pygradflow/runners/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,16 +207,16 @@
             "size",
             "status",
             "total_time",
             "iterations",
             "num_accepted_steps",
         ]
 
-        with open(filename, "w") as file:
-            writer = csv.DictWriter(file, fieldnames=fieldnames)
+        with open(filename, "w") as output_file:
+            writer = csv.DictWriter(output_file, fieldnames=fieldnames)
             writer.writeheader()
 
             for instance, result in zip(instances, results):
                 info = {
                     "instance": instance.name,
                     "num_vars": instance.num_vars,
                     "num_cons": instance.num_cons,
@@ -250,7 +250,9 @@
                             **info,
                             "status": SolverStatus.short_name(result.status),
                             "total_time": result.total_time,
                             "iterations": result.iterations,
                             "num_accepted_steps": result.num_accepted_steps,
                         }
                     )
+
+                output_file.flush()
```

### Comparing `pygradflow-0.4.3/pygradflow/scale.py` & `pygradflow-0.4.4/pygradflow/scale.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/solver.py` & `pygradflow-0.4.4/pygradflow/solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/step/__init__.py` & `pygradflow-0.4.4/pygradflow/step/__init__.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/step/asymmetric_step_solver.py` & `pygradflow-0.4.4/pygradflow/step/asymmetric_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/step/box_control.py` & `pygradflow-0.4.4/pygradflow/step/box_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/step/cond_estimate.py` & `pygradflow-0.4.4/pygradflow/step/cond_estimate.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/step/distance_ratio_control.py` & `pygradflow-0.4.4/pygradflow/step/distance_ratio_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/step/exact_control.py` & `pygradflow-0.4.4/pygradflow/step/exact_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/step/extended_step_solver.py` & `pygradflow-0.4.4/pygradflow/step/extended_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/step/fixed_control.py` & `pygradflow-0.4.4/pygradflow/step/fixed_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/step/linear_solver.py` & `pygradflow-0.4.4/pygradflow/step/linear_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/step/opti_control.py` & `pygradflow-0.4.4/pygradflow/step/opti_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/step/residuum_ratio_control.py` & `pygradflow-0.4.4/pygradflow/step/residuum_ratio_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/step/scaled_step_solver.py` & `pygradflow-0.4.4/pygradflow/step/scaled_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/step/standard_step_solver.py` & `pygradflow-0.4.4/pygradflow/step/standard_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/step/step_control.py` & `pygradflow-0.4.4/pygradflow/step/step_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/step/step_solver.py` & `pygradflow-0.4.4/pygradflow/step/step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/step/symmetric_step_solver.py` & `pygradflow-0.4.4/pygradflow/step/symmetric_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pygradflow/transform.py` & `pygradflow-0.4.4/pygradflow/transform.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.3/pyproject.toml` & `pygradflow-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygradflow"
-version = "0.4.3"
+version = "0.4.4"
 description = "PyGradFlow is a simple implementation of the sequential homotopy method to be used to solve general nonlinear programs."
 authors = ["Christoph Hansknecht <christoph.hansknecht@tu-clausthal.de>"]
 readme = "README.md"
 repository = "https://github.com/chrhansk/pygradflow"
 documentation = "https://pygradflow.readthedocs.io"
```

### Comparing `pygradflow-0.4.3/PKG-INFO` & `pygradflow-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygradflow
-Version: 0.4.3
+Version: 0.4.4
 Summary: PyGradFlow is a simple implementation of the sequential homotopy method to be used to solve general nonlinear programs.
 Home-page: https://github.com/chrhansk/pygradflow
 Author: Christoph Hansknecht
 Author-email: christoph.hansknecht@tu-clausthal.de
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

