# Comparing `tmp/pygradflow-0.4.2.tar.gz` & `tmp/pygradflow-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygradflow-0.4.2.tar", max compression
+gzip compressed data, was "pygradflow-0.4.3.tar", max compression
```

## Comparing `pygradflow-0.4.2.tar` & `pygradflow-0.4.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    10847 2024-05-06 12:39:25.958263 pygradflow-0.4.2/LICENSE
--rw-r--r--   0        0        0      984 2024-05-06 12:39:25.958263 pygradflow-0.4.2/README.md
--rw-r--r--   0        0        0        0 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/__init__.py
--rw-r--r--   0        0        0      872 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/active_set.py
--rw-r--r--   0        0        0     4458 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/cons_problem.py
--rw-r--r--   0        0        0     1749 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/controller.py
--rw-r--r--   0        0        0     2487 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/deriv_check.py
--rw-r--r--   0        0        0     4645 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/display.py
--rw-r--r--   0        0        0     4839 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/eval.py
--rw-r--r--   0        0        0     6380 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/implicit_func.py
--rw-r--r--   0        0        0     5146 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/iterate.py
--rw-r--r--   0        0        0       55 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/log.py
--rw-r--r--   0        0        0     6570 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/newton.py
--rw-r--r--   0        0        0     5173 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/params.py
--rw-r--r--   0        0        0     5111 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/penalty.py
--rw-r--r--   0        0        0     5845 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/problem.py
--rw-r--r--   0        0        0        0 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/py.typed
--rw-r--r--   0        0        0     3378 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/runners/cutest_runner.py
--rw-r--r--   0        0        0      366 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/runners/instance.py
--rw-r--r--   0        0        0     2045 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/runners/qplib_runner.py
--rw-r--r--   0        0        0     7417 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/runners/runner.py
--rw-r--r--   0        0        0     4181 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/scale.py
--rw-r--r--   0        0        0    16537 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/solver.py
--rw-r--r--   0        0        0     1284 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/step/__init__.py
--rw-r--r--   0        0        0     4439 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/step/asymmetric_step_solver.py
--rw-r--r--   0        0        0     5790 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/step/box_control.py
--rw-r--r--   0        0        0     2710 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/step/cond_estimate.py
--rw-r--r--   0        0        0     2431 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/step/distance_ratio_control.py
--rw-r--r--   0        0        0     2058 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/step/exact_control.py
--rw-r--r--   0        0        0     3173 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/step/extended_step_solver.py
--rw-r--r--   0        0        0      543 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/step/fixed_control.py
--rw-r--r--   0        0        0     2669 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/step/linear_solver.py
--rw-r--r--   0        0        0     7555 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/step/opti_control.py
--rw-r--r--   0        0        0     2014 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/step/residuum_ratio_control.py
--rw-r--r--   0        0        0     2401 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/step/scaled_step_solver.py
--rw-r--r--   0        0        0     2467 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/step/standard_step_solver.py
--rw-r--r--   0        0        0     4697 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/step/step_control.py
--rw-r--r--   0        0        0     2048 2024-05-06 12:39:25.958263 pygradflow-0.4.2/pygradflow/step/step_solver.py
--rw-r--r--   0        0        0     4120 2024-05-06 12:39:25.962263 pygradflow-0.4.2/pygradflow/step/symmetric_step_solver.py
--rw-r--r--   0        0        0      380 2024-05-06 12:39:25.962263 pygradflow-0.4.2/pygradflow/timer.py
--rw-r--r--   0        0        0     1711 2024-05-06 12:39:25.962263 pygradflow-0.4.2/pygradflow/transform.py
--rw-r--r--   0        0        0      232 2024-05-06 12:39:25.962263 pygradflow-0.4.2/pygradflow/util.py
--rw-r--r--   0        0        0     1138 2024-05-06 12:39:25.962263 pygradflow-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1983 1970-01-01 00:00:00.000000 pygradflow-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    10847 2024-05-07 15:14:03.094458 pygradflow-0.4.3/LICENSE
+-rw-r--r--   0        0        0      984 2024-05-07 15:14:03.094458 pygradflow-0.4.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/__init__.py
+-rw-r--r--   0        0        0      872 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/active_set.py
+-rw-r--r--   0        0        0     4458 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/cons_problem.py
+-rw-r--r--   0        0        0     1749 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/controller.py
+-rw-r--r--   0        0        0     2487 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/deriv_check.py
+-rw-r--r--   0        0        0     4645 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/display.py
+-rw-r--r--   0        0        0     4839 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/eval.py
+-rw-r--r--   0        0        0     6380 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/implicit_func.py
+-rw-r--r--   0        0        0     5146 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/iterate.py
+-rw-r--r--   0        0        0       55 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/log.py
+-rw-r--r--   0        0        0     6570 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/newton.py
+-rw-r--r--   0        0        0     5173 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/params.py
+-rw-r--r--   0        0        0     5111 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/penalty.py
+-rw-r--r--   0        0        0     5845 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/problem.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/py.typed
+-rw-r--r--   0        0        0     3378 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/runners/cutest_runner.py
+-rw-r--r--   0        0        0      366 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/runners/instance.py
+-rw-r--r--   0        0        0     2045 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/runners/qplib_runner.py
+-rw-r--r--   0        0        0     7792 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/runners/runner.py
+-rw-r--r--   0        0        0     4181 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/scale.py
+-rw-r--r--   0        0        0    16537 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/solver.py
+-rw-r--r--   0        0        0     1284 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/__init__.py
+-rw-r--r--   0        0        0     4439 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/asymmetric_step_solver.py
+-rw-r--r--   0        0        0     5790 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/box_control.py
+-rw-r--r--   0        0        0     2710 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/cond_estimate.py
+-rw-r--r--   0        0        0     2431 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/distance_ratio_control.py
+-rw-r--r--   0        0        0     2058 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/exact_control.py
+-rw-r--r--   0        0        0     3173 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/extended_step_solver.py
+-rw-r--r--   0        0        0      543 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/fixed_control.py
+-rw-r--r--   0        0        0     2669 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/linear_solver.py
+-rw-r--r--   0        0        0     7241 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/opti_control.py
+-rw-r--r--   0        0        0     2014 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/residuum_ratio_control.py
+-rw-r--r--   0        0        0     2401 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/scaled_step_solver.py
+-rw-r--r--   0        0        0     2467 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/standard_step_solver.py
+-rw-r--r--   0        0        0     4697 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/step_control.py
+-rw-r--r--   0        0        0     2048 2024-05-07 15:14:03.094458 pygradflow-0.4.3/pygradflow/step/step_solver.py
+-rw-r--r--   0        0        0     4120 2024-05-07 15:14:03.098458 pygradflow-0.4.3/pygradflow/step/symmetric_step_solver.py
+-rw-r--r--   0        0        0      380 2024-05-07 15:14:03.098458 pygradflow-0.4.3/pygradflow/timer.py
+-rw-r--r--   0        0        0     1711 2024-05-07 15:14:03.098458 pygradflow-0.4.3/pygradflow/transform.py
+-rw-r--r--   0        0        0      232 2024-05-07 15:14:03.098458 pygradflow-0.4.3/pygradflow/util.py
+-rw-r--r--   0        0        0     1138 2024-05-07 15:14:03.098458 pygradflow-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1983 1970-01-01 00:00:00.000000 pygradflow-0.4.3/PKG-INFO
```

### Comparing `pygradflow-0.4.2/LICENSE` & `pygradflow-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/README.md` & `pygradflow-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/active_set.py` & `pygradflow-0.4.3/pygradflow/active_set.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/cons_problem.py` & `pygradflow-0.4.3/pygradflow/cons_problem.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/controller.py` & `pygradflow-0.4.3/pygradflow/controller.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/deriv_check.py` & `pygradflow-0.4.3/pygradflow/deriv_check.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/display.py` & `pygradflow-0.4.3/pygradflow/display.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/eval.py` & `pygradflow-0.4.3/pygradflow/eval.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/implicit_func.py` & `pygradflow-0.4.3/pygradflow/implicit_func.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/iterate.py` & `pygradflow-0.4.3/pygradflow/iterate.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/newton.py` & `pygradflow-0.4.3/pygradflow/newton.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/params.py` & `pygradflow-0.4.3/pygradflow/params.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/penalty.py` & `pygradflow-0.4.3/pygradflow/penalty.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/problem.py` & `pygradflow-0.4.3/pygradflow/problem.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/runners/cutest_runner.py` & `pygradflow-0.4.3/pygradflow/runners/cutest_runner.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/runners/qplib_runner.py` & `pygradflow-0.4.3/pygradflow/runners/qplib_runner.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/runners/runner.py` & `pygradflow-0.4.3/pygradflow/runners/runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,20 +14,27 @@
 from pygradflow.solver import SolverStatus
 
 run_logger = logging.getLogger(__name__)
 
 formatter = logging.Formatter("%(asctime)s:%(name)s:%(levelname)s:%(message)s")
 
 
-def try_solve_instance(instance, params, log_filename):
+def try_solve_instance(instance, params, log_filename, verbose):
     try:
+        logger.handlers.clear()
+
         handler = logging.FileHandler(log_filename)
         handler.setFormatter(formatter)
-        logger.handlers.clear()
         logger.addHandler(handler)
+
+        if verbose:
+            handler = logging.StreamHandler()
+            handler.setFormatter(formatter)
+            logger.addHandler(handler)
+
         logger.setLevel(logging.INFO)
 
         logging.captureWarnings(True)
         warn_logger = logging.getLogger("py.warnings")
         warn_logger.addHandler(handler)
         warn_logger.setLevel(logging.WARN)
 
@@ -79,34 +86,39 @@
         run_logger.info("Solving %d instances", len(instances))
 
         params = self.create_params(args)
 
         def log_filename(instance):
             return self.output_filename(args, f"{instance.name}.log")
 
+        verbose = args.verbose
+
         if args.parallel is not None:
             if args.parallel is True:
                 num_procs = cpu_count()
             else:
                 num_procs = args.parallel
 
             run_logger.info("Solving in parallel with up to %d processes", num_procs)
 
             all_params = itertools.repeat(params)
             all_log_filenames = [log_filename(instance) for instance in instances]
+            all_verbose = itertools.repeat(verbose)
 
-            solve_args = zip(instances, all_params, all_log_filenames)
+            solve_args = zip(instances, all_params, all_log_filenames, all_verbose)
 
             with Pool(num_procs, maxtasksperchild=1) as pool:
                 results = pool.starmap(try_solve_instance, solve_args)
 
         else:
             for instance in instances:
                 results.append(
-                    try_solve_instance(instance, params, log_filename(instance))
+                    try_solve_instance(
+                        instance, params, log_filename(instance), verbose
+                    )
                 )
 
         self.write_results(args, params, instances, results)
 
     def filter_instances(self, args):
         instances = []
 
@@ -128,14 +140,15 @@
         import argparse
 
         parser = argparse.ArgumentParser()
 
         parser.add_argument("--output", type=str)
         parser.add_argument("--max_size", type=int)
         parser.add_argument("--name", type=str)
+        parser.add_argument("--verbose", action="store_true")
         parser.add_argument("--parallel", nargs="?", type=int, const=True)
 
         group = parser.add_argument_group(title="parameters")
 
         default_params = Params()
 
         for key, attr in default_params.annotations():
```

### Comparing `pygradflow-0.4.2/pygradflow/scale.py` & `pygradflow-0.4.3/pygradflow/scale.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/solver.py` & `pygradflow-0.4.3/pygradflow/solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/step/__init__.py` & `pygradflow-0.4.3/pygradflow/step/__init__.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/step/asymmetric_step_solver.py` & `pygradflow-0.4.3/pygradflow/step/asymmetric_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/step/box_control.py` & `pygradflow-0.4.3/pygradflow/step/box_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/step/cond_estimate.py` & `pygradflow-0.4.3/pygradflow/step/cond_estimate.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/step/distance_ratio_control.py` & `pygradflow-0.4.3/pygradflow/step/distance_ratio_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/step/exact_control.py` & `pygradflow-0.4.3/pygradflow/step/exact_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/step/extended_step_solver.py` & `pygradflow-0.4.3/pygradflow/step/extended_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/step/fixed_control.py` & `pygradflow-0.4.3/pygradflow/step/fixed_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/step/linear_solver.py` & `pygradflow-0.4.3/pygradflow/step/linear_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/step/opti_control.py` & `pygradflow-0.4.3/pygradflow/step/opti_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,24 +224,19 @@
         z0 = np.concatenate([x0, y0])
 
         # Solve using Ipopt
         z, info = super().solve(z0)
 
         assert np.isfinite(z).all()
 
-        if info["status"] != 0:
+        if info["status"] not in [0, 1]:
             raise StepSolverError("Ipopt failed to solve the problem")
 
         x = z[: self.prob_num_vars]
-        if rescaled:
-            v = z[self.prob_num_vars :]
-            w = v / math.sqrt(self.lamb)
-        else:
-            w = z[self.prob_num_vars :]
-        y = iterate.y - w
+        y = info["mult_g"]
 
         return (x, y)
 
 
 class OptimizingController(StepController):
     def step(self, iterate, rho, dt, next_steps, display, timer) -> StepControlResult:
 
@@ -256,15 +251,10 @@
 
         implicit_func = ImplicitFunc(problem, iterate, dt)
 
         value = implicit_func.value_at(next_iterate, rho)
 
         residuum = np.linalg.norm(value)
 
-        if residuum <= 1e-6:
-            return StepControlResult(
-                next_iterate, 0.5 * lamb, active_set=None, rcond=None, accepted=True
-            )
-
         return StepControlResult(
-            next_iterate, 2.0 * lamb, active_set=None, rcond=None, accepted=False
+            next_iterate, 0.5 * lamb, active_set=None, rcond=None, accepted=True
         )
```

### Comparing `pygradflow-0.4.2/pygradflow/step/residuum_ratio_control.py` & `pygradflow-0.4.3/pygradflow/step/residuum_ratio_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/step/scaled_step_solver.py` & `pygradflow-0.4.3/pygradflow/step/scaled_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/step/standard_step_solver.py` & `pygradflow-0.4.3/pygradflow/step/standard_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/step/step_control.py` & `pygradflow-0.4.3/pygradflow/step/step_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/step/step_solver.py` & `pygradflow-0.4.3/pygradflow/step/step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/step/symmetric_step_solver.py` & `pygradflow-0.4.3/pygradflow/step/symmetric_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pygradflow/transform.py` & `pygradflow-0.4.3/pygradflow/transform.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.2/pyproject.toml` & `pygradflow-0.4.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygradflow"
-version = "0.4.2"
+version = "0.4.3"
 description = "PyGradFlow is a simple implementation of the sequential homotopy method to be used to solve general nonlinear programs."
 authors = ["Christoph Hansknecht <christoph.hansknecht@tu-clausthal.de>"]
 readme = "README.md"
 repository = "https://github.com/chrhansk/pygradflow"
 documentation = "https://pygradflow.readthedocs.io"
```

### Comparing `pygradflow-0.4.2/PKG-INFO` & `pygradflow-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygradflow
-Version: 0.4.2
+Version: 0.4.3
 Summary: PyGradFlow is a simple implementation of the sequential homotopy method to be used to solve general nonlinear programs.
 Home-page: https://github.com/chrhansk/pygradflow
 Author: Christoph Hansknecht
 Author-email: christoph.hansknecht@tu-clausthal.de
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

