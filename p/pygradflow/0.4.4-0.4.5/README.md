# Comparing `tmp/pygradflow-0.4.4.tar.gz` & `tmp/pygradflow-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygradflow-0.4.4.tar", max compression
+gzip compressed data, was "pygradflow-0.4.5.tar", max compression
```

## Comparing `pygradflow-0.4.4.tar` & `pygradflow-0.4.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    10847 2024-05-07 19:36:13.809971 pygradflow-0.4.4/LICENSE
--rw-r--r--   0        0        0      984 2024-05-07 19:36:13.809971 pygradflow-0.4.4/README.md
--rw-r--r--   0        0        0        0 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/__init__.py
--rw-r--r--   0        0        0      872 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/active_set.py
--rw-r--r--   0        0        0     4458 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/cons_problem.py
--rw-r--r--   0        0        0     1749 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/controller.py
--rw-r--r--   0        0        0     2487 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/deriv_check.py
--rw-r--r--   0        0        0     4645 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/display.py
--rw-r--r--   0        0        0     4839 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/eval.py
--rw-r--r--   0        0        0     6380 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/implicit_func.py
--rw-r--r--   0        0        0     5146 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/iterate.py
--rw-r--r--   0        0        0       55 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/log.py
--rw-r--r--   0        0        0     6570 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/newton.py
--rw-r--r--   0        0        0     5173 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/params.py
--rw-r--r--   0        0        0     5111 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/penalty.py
--rw-r--r--   0        0        0     5845 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/problem.py
--rw-r--r--   0        0        0        0 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/py.typed
--rw-r--r--   0        0        0     3378 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/runners/cutest_runner.py
--rw-r--r--   0        0        0      366 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/runners/instance.py
--rw-r--r--   0        0        0     2045 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/runners/qplib_runner.py
--rw-r--r--   0        0        0     7843 2024-05-07 19:36:13.809971 pygradflow-0.4.4/pygradflow/runners/runner.py
--rw-r--r--   0        0        0     4181 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/scale.py
--rw-r--r--   0        0        0    16537 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/solver.py
--rw-r--r--   0        0        0     1284 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/__init__.py
--rw-r--r--   0        0        0     4439 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/asymmetric_step_solver.py
--rw-r--r--   0        0        0     5790 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/box_control.py
--rw-r--r--   0        0        0     2710 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/cond_estimate.py
--rw-r--r--   0        0        0     2431 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/distance_ratio_control.py
--rw-r--r--   0        0        0     2058 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/exact_control.py
--rw-r--r--   0        0        0     3173 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/extended_step_solver.py
--rw-r--r--   0        0        0      543 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/fixed_control.py
--rw-r--r--   0        0        0     2669 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/linear_solver.py
--rw-r--r--   0        0        0     7241 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/opti_control.py
--rw-r--r--   0        0        0     2014 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/residuum_ratio_control.py
--rw-r--r--   0        0        0     2401 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/scaled_step_solver.py
--rw-r--r--   0        0        0     2467 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/standard_step_solver.py
--rw-r--r--   0        0        0     4697 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/step_control.py
--rw-r--r--   0        0        0     2048 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/step_solver.py
--rw-r--r--   0        0        0     4120 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/step/symmetric_step_solver.py
--rw-r--r--   0        0        0      380 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/timer.py
--rw-r--r--   0        0        0     1711 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/transform.py
--rw-r--r--   0        0        0      232 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pygradflow/util.py
--rw-r--r--   0        0        0     1138 2024-05-07 19:36:13.813971 pygradflow-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     1983 1970-01-01 00:00:00.000000 pygradflow-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0    10847 2024-05-07 21:15:39.157537 pygradflow-0.4.5/LICENSE
+-rw-r--r--   0        0        0      984 2024-05-07 21:15:39.157537 pygradflow-0.4.5/README.md
+-rw-r--r--   0        0        0        0 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/__init__.py
+-rw-r--r--   0        0        0      872 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/active_set.py
+-rw-r--r--   0        0        0     4458 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/cons_problem.py
+-rw-r--r--   0        0        0     1749 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/controller.py
+-rw-r--r--   0        0        0     2487 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/deriv_check.py
+-rw-r--r--   0        0        0     4645 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/display.py
+-rw-r--r--   0        0        0     4839 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/eval.py
+-rw-r--r--   0        0        0     6380 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/implicit_func.py
+-rw-r--r--   0        0        0     5146 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/iterate.py
+-rw-r--r--   0        0        0       55 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/log.py
+-rw-r--r--   0        0        0     6570 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/newton.py
+-rw-r--r--   0        0        0     5173 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/params.py
+-rw-r--r--   0        0        0     5111 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/penalty.py
+-rw-r--r--   0        0        0     5845 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/problem.py
+-rw-r--r--   0        0        0        0 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/py.typed
+-rw-r--r--   0        0        0     3378 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/runners/cutest_runner.py
+-rw-r--r--   0        0        0      366 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/runners/instance.py
+-rw-r--r--   0        0        0     2045 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/runners/qplib_runner.py
+-rw-r--r--   0        0        0     8326 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/runners/runner.py
+-rw-r--r--   0        0        0     4181 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/scale.py
+-rw-r--r--   0        0        0    16537 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/solver.py
+-rw-r--r--   0        0        0     1284 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/step/__init__.py
+-rw-r--r--   0        0        0     4439 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/step/asymmetric_step_solver.py
+-rw-r--r--   0        0        0     5790 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/step/box_control.py
+-rw-r--r--   0        0        0     2710 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/step/cond_estimate.py
+-rw-r--r--   0        0        0     2431 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/step/distance_ratio_control.py
+-rw-r--r--   0        0        0     2058 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/step/exact_control.py
+-rw-r--r--   0        0        0     3173 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/step/extended_step_solver.py
+-rw-r--r--   0        0        0      543 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/step/fixed_control.py
+-rw-r--r--   0        0        0     2669 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/step/linear_solver.py
+-rw-r--r--   0        0        0     7241 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/step/opti_control.py
+-rw-r--r--   0        0        0     2014 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/step/residuum_ratio_control.py
+-rw-r--r--   0        0        0     2401 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/step/scaled_step_solver.py
+-rw-r--r--   0        0        0     2467 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/step/standard_step_solver.py
+-rw-r--r--   0        0        0     4697 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/step/step_control.py
+-rw-r--r--   0        0        0     2048 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/step/step_solver.py
+-rw-r--r--   0        0        0     4120 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/step/symmetric_step_solver.py
+-rw-r--r--   0        0        0      380 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/timer.py
+-rw-r--r--   0        0        0     1711 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/transform.py
+-rw-r--r--   0        0        0      232 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pygradflow/util.py
+-rw-r--r--   0        0        0     1138 2024-05-07 21:15:39.161537 pygradflow-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     1983 1970-01-01 00:00:00.000000 pygradflow-0.4.5/PKG-INFO
```

### Comparing `pygradflow-0.4.4/LICENSE` & `pygradflow-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/README.md` & `pygradflow-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/active_set.py` & `pygradflow-0.4.5/pygradflow/active_set.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/cons_problem.py` & `pygradflow-0.4.5/pygradflow/cons_problem.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/controller.py` & `pygradflow-0.4.5/pygradflow/controller.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/deriv_check.py` & `pygradflow-0.4.5/pygradflow/deriv_check.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/display.py` & `pygradflow-0.4.5/pygradflow/display.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/eval.py` & `pygradflow-0.4.5/pygradflow/eval.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/implicit_func.py` & `pygradflow-0.4.5/pygradflow/implicit_func.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/iterate.py` & `pygradflow-0.4.5/pygradflow/iterate.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/newton.py` & `pygradflow-0.4.5/pygradflow/newton.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/params.py` & `pygradflow-0.4.5/pygradflow/params.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/penalty.py` & `pygradflow-0.4.5/pygradflow/penalty.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/problem.py` & `pygradflow-0.4.5/pygradflow/problem.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/runners/cutest_runner.py` & `pygradflow-0.4.5/pygradflow/runners/cutest_runner.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/runners/qplib_runner.py` & `pygradflow-0.4.5/pygradflow/runners/qplib_runner.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/runners/runner.py` & `pygradflow-0.4.5/pygradflow/runners/runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
 import enum
 import itertools
 import logging
 import os
 from abc import ABC, abstractmethod
-from multiprocessing import Pool, TimeoutError, cpu_count
+from concurrent.futures import FIRST_COMPLETED, ProcessPoolExecutor, wait
+from multiprocessing import TimeoutError, cpu_count
 from multiprocessing.pool import ThreadPool
 
 import numpy as np
 
 from pygradflow.log import logger
 from pygradflow.params import Params
 from pygradflow.solver import SolverStatus
@@ -39,30 +40,31 @@
         warn_logger.setLevel(logging.WARN)
 
         def solve():
             return instance.solve(params)
 
         # No time limit
         if params.time_limit == np.inf:
-            return solve()
+            return (instance, solve())
 
         # Solve in thread pool so we can
         # await the result
         thread_pool = ThreadPool(1)
 
         try:
             res = thread_pool.apply_async(solve)
-            return res.get(params.time_limit)
+            result = res.get(params.time_limit)
+            return (instance, result)
         except TimeoutError:
             logger.error("Reached timeout, aborting")
-            return "timeout"
+            return (instance, "timeout")
     except Exception as exc:
         logger.error("Error solving %s", instance.name)
         logger.exception(exc, exc_info=(type(exc), exc, exc.__traceback__))
-        return "error"
+        return (instance, "error")
 
 
 class Runner(ABC):
     def __init__(self, name):
         self.name = name
 
     @abstractmethod
@@ -76,52 +78,66 @@
             value = getattr(args, key)
             if isinstance(attr, enum.EnumMeta):
                 value = attr[value]
             setattr(params, key, value)
 
         return params
 
-    def solve(self, instances, args):
-        results = []
+    def log_filename(self, args, instance):
+        return self.output_filename(args, f"{instance.name}.log")
 
-        run_logger.info("Solving %d instances", len(instances))
+    def solve_instances_sequential(self, instances, args, params):
+        verbose = args.verbose
+        for instance in instances:
+            log_filename = self.log_filename(args, instance)
+            yield try_solve_instance(instance, params, log_filename, verbose)
 
-        params = self.create_params(args)
+    def solve_instances_parallel(self, instances, args, params):
+        verbose = args.verbose
 
-        def log_filename(instance):
-            return self.output_filename(args, f"{instance.name}.log")
+        if args.parallel is True:
+            num_procs = cpu_count()
+        else:
+            num_procs = args.parallel
 
-        verbose = args.verbose
+        run_logger.info("Solving in parallel with up to %d processes", num_procs)
 
-        if args.parallel is not None:
-            if args.parallel is True:
-                num_procs = cpu_count()
-            else:
-                num_procs = args.parallel
+        all_params = itertools.repeat(params)
+        all_log_filenames = [
+            self.log_filename(args, instance) for instance in instances
+        ]
+        all_verbose = itertools.repeat(verbose)
 
-            run_logger.info("Solving in parallel with up to %d processes", num_procs)
+        solve_args = zip(instances, all_params, all_log_filenames, all_verbose)
 
-            all_params = itertools.repeat(params)
-            all_log_filenames = [log_filename(instance) for instance in instances]
-            all_verbose = itertools.repeat(verbose)
+        with ProcessPoolExecutor(num_procs, max_tasks_per_child=1) as pool:
+            futures = [
+                pool.submit(try_solve_instance, *solve_arg) for solve_arg in solve_args
+            ]
 
-            solve_args = zip(instances, all_params, all_log_filenames, all_verbose)
+            while len(futures) != 0:
+                done, futures = wait(futures, return_when=FIRST_COMPLETED)
 
-            with Pool(num_procs, maxtasksperchild=1) as pool:
-                results = pool.starmap(try_solve_instance, solve_args)
+                for item in done:
+                    yield item.result()
 
-        else:
-            for instance in instances:
-                results.append(
-                    try_solve_instance(
-                        instance, params, log_filename(instance), verbose
-                    )
-                )
+    def solve_instances(self, instances, args):
+        # yields sequence of tuples of (instance, result) for each instance
+        results = []
 
-        self.write_results(args, params, instances, results)
+        run_logger.info("Solving %d instances", len(instances))
+
+        params = self.create_params(args)
+
+        verbose = args.verbose
+
+        if args.parallel is not None:
+            yield from self.solve_instances_parallel(instances, args, params)
+        else:
+            yield from self.solve_instances_sequential(instances, args, params)
 
     def filter_instances(self, args):
         instances = []
 
         max_size = args.max_size
         name = args.name
 
@@ -187,17 +203,53 @@
 
         os.makedirs(args.output, exist_ok=True)
 
         instances = self.filter_instances(args)
 
         self.solve(instances, args)
 
-    def write_results(self, args, params, instances, results):
+    def create_csv_row(self, args, instance, result):
+        info = {
+            "instance": instance.name,
+            "num_vars": instance.num_vars,
+            "num_cons": instance.num_cons,
+            "size": instance.size,
+        }
+
+        if result == "timeout":
+            return {
+                **info,
+                "status": "timeout",
+                "total_time": args.time_limit,
+                "iterations": 0,
+                "num_accepted_steps": 0,
+            }
+
+        elif result == "error":
+            return {
+                **info,
+                "status": "error",
+                "total_time": 0.0,
+                "iterations": 0,
+                "num_accepted_steps": 0,
+            }
+        else:
+            return {
+                **info,
+                "status": SolverStatus.short_name(result.status),
+                "total_time": result.total_time,
+                "iterations": result.iterations,
+                "num_accepted_steps": result.num_accepted_steps,
+            }
+
+    def solve(self, instances, args):
         import csv
 
+        params = self.create_params(args)
+
         params.write(self.output_filename(args, "params.yml"))
 
         filename = self.output_filename(args, "output.csv")
 
         run_logger.info("Writing results to '%s'", filename)
 
         fieldnames = [
@@ -211,48 +263,11 @@
             "num_accepted_steps",
         ]
 
         with open(filename, "w") as output_file:
             writer = csv.DictWriter(output_file, fieldnames=fieldnames)
             writer.writeheader()
 
-            for instance, result in zip(instances, results):
-                info = {
-                    "instance": instance.name,
-                    "num_vars": instance.num_vars,
-                    "num_cons": instance.num_cons,
-                    "size": instance.size,
-                }
-
-                if result == "timeout":
-                    writer.writerow(
-                        {
-                            **info,
-                            "status": "timeout",
-                            "total_time": args.time_limit,
-                            "iterations": 0,
-                            "num_accepted_steps": 0,
-                        }
-                    )
-
-                elif result == "error":
-                    writer.writerow(
-                        {
-                            **info,
-                            "status": "error",
-                            "total_time": 0.0,
-                            "iterations": 0,
-                            "num_accepted_steps": 0,
-                        }
-                    )
-                else:
-                    writer.writerow(
-                        {
-                            **info,
-                            "status": SolverStatus.short_name(result.status),
-                            "total_time": result.total_time,
-                            "iterations": result.iterations,
-                            "num_accepted_steps": result.num_accepted_steps,
-                        }
-                    )
-
+            for instance, result in self.solve_instances(instances, args):
+                run_logger.info("Finished instance %s", instance.name)
+                writer.writerow(self.create_csv_row(args, instance, result))
                 output_file.flush()
```

### Comparing `pygradflow-0.4.4/pygradflow/scale.py` & `pygradflow-0.4.5/pygradflow/scale.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/solver.py` & `pygradflow-0.4.5/pygradflow/solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/step/__init__.py` & `pygradflow-0.4.5/pygradflow/step/__init__.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/step/asymmetric_step_solver.py` & `pygradflow-0.4.5/pygradflow/step/asymmetric_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/step/box_control.py` & `pygradflow-0.4.5/pygradflow/step/box_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/step/cond_estimate.py` & `pygradflow-0.4.5/pygradflow/step/cond_estimate.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/step/distance_ratio_control.py` & `pygradflow-0.4.5/pygradflow/step/distance_ratio_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/step/exact_control.py` & `pygradflow-0.4.5/pygradflow/step/exact_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/step/extended_step_solver.py` & `pygradflow-0.4.5/pygradflow/step/extended_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/step/fixed_control.py` & `pygradflow-0.4.5/pygradflow/step/fixed_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/step/linear_solver.py` & `pygradflow-0.4.5/pygradflow/step/linear_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/step/opti_control.py` & `pygradflow-0.4.5/pygradflow/step/opti_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/step/residuum_ratio_control.py` & `pygradflow-0.4.5/pygradflow/step/residuum_ratio_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/step/scaled_step_solver.py` & `pygradflow-0.4.5/pygradflow/step/scaled_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/step/standard_step_solver.py` & `pygradflow-0.4.5/pygradflow/step/standard_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/step/step_control.py` & `pygradflow-0.4.5/pygradflow/step/step_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/step/step_solver.py` & `pygradflow-0.4.5/pygradflow/step/step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/step/symmetric_step_solver.py` & `pygradflow-0.4.5/pygradflow/step/symmetric_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pygradflow/transform.py` & `pygradflow-0.4.5/pygradflow/transform.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.4/pyproject.toml` & `pygradflow-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygradflow"
-version = "0.4.4"
+version = "0.4.5"
 description = "PyGradFlow is a simple implementation of the sequential homotopy method to be used to solve general nonlinear programs."
 authors = ["Christoph Hansknecht <christoph.hansknecht@tu-clausthal.de>"]
 readme = "README.md"
 repository = "https://github.com/chrhansk/pygradflow"
 documentation = "https://pygradflow.readthedocs.io"
```

### Comparing `pygradflow-0.4.4/PKG-INFO` & `pygradflow-0.4.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygradflow
-Version: 0.4.4
+Version: 0.4.5
 Summary: PyGradFlow is a simple implementation of the sequential homotopy method to be used to solve general nonlinear programs.
 Home-page: https://github.com/chrhansk/pygradflow
 Author: Christoph Hansknecht
 Author-email: christoph.hansknecht@tu-clausthal.de
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

