# Comparing `tmp/xopt-2.2.2.tar.gz` & `tmp/xopt-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/Xopt/Xopt/dist/.tmp-6mpyfq9i/xopt-2.2.2.tar", last modified: Mon Apr 15 19:26:55 2024, max compression
+gzip compressed data, was "/home/runner/work/Xopt/Xopt/dist/.tmp-id1f8s_j/xopt-2.2.3.tar", last modified: Tue May  7 19:37:30 2024, max compression
```

## Comparing `xopt-2.2.2.tar` & `xopt-2.2.3.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 19:26:51.000000 xopt-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-15 19:26:51.000000 xopt-2.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-04-15 19:26:55.000000 xopt-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8594 2024-04-15 19:26:51.000000 xopt-2.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:54.000000 xopt-2.2.2/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:51.000000 xopt-2.2.2/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-15 19:26:51.000000 xopt-2.2.2/benchmarks/test_mo.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-15 19:26:51.000000 xopt-2.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-15 19:26:55.000000 xopt-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-15 19:26:51.000000 xopt-2.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/tests/generators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/tests/generators/bayesian/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_bax.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_bayesian_exploration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8970 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_bayesian_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_custom_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_expected_improvement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_hessian_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_high_level.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_mggpo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_mobo.py
--rw-r--r--   0 runner    (1001) docker     (127)    19856 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_model_constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_time_dependent_bo.py
--rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_turbo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_upper_confidence_bound.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/test_extremum_seeking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/test_latin_hypercube.py
--rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/test_neldermead.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/test_rcds.py
--rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/test_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/test_mpi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/test_numerical_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/test_perf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/test_vocs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/test_xopt.py
--rw-r--r--   0 runner    (1001) docker     (127)    78325 2024-04-15 19:26:51.000000 xopt-2.2.2/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/asynchronous.py
--rw-r--r--   0 runner    (1001) docker     (127)    18279 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/generators/
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/generators/bayesian/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/base_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/generators/bayesian/bax/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/bax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/bax/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/bax/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/bax_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/bayesian_exploration.py
--rw-r--r--   0 runner    (1001) docker     (127)    27951 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/bayesian_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/generators/bayesian/custom_botorch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/custom_botorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/custom_botorch/constrained_acquisition.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/custom_botorch/hessian_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/custom_botorch/heteroskedastic.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/custom_botorch/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/custom_botorch/log_acquisition_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/custom_botorch/multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/custom_botorch/proximal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/expected_improvement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/mggpo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/mobo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/generators/bayesian/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/models/prior_mean.py
--rw-r--r--   0 runner    (1001) docker     (127)    10944 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/models/standard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/models/time_dependent.py
--rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/objectives.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/time_dependent.py
--rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/turbo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/upper_confidence_bound.py
--rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17222 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/generators/es/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/es/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/es/extremumseeking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/generators/ga/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/ga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/ga/cnsga.py
--rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/ga/deap_creator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3137 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/ga/deap_fitness_with_constraints.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3138 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/ga/fitness_with_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/generators/rcds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/rcds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14100 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/rcds/rcds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/generators/scipy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/scipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/scipy/latin_hypercube.py
--rw-r--r--   0 runner    (1001) docker     (127)    17535 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/scipy/neldermead.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/mpi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/mpi/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/numerical_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    26153 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/pydantic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/benchmarking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/resources/test_functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/test_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/test_functions/ackley_20.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/test_functions/modified_tnk.py
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/test_functions/multi_objective.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/test_functions/problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/test_functions/rosenbrock.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/test_functions/sinusoid_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/test_functions/sphere_100.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/test_functions/sphere_20.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/test_functions/sphere_50.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/test_functions/tnk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9610 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25108 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/vocs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-04-15 19:26:54.000000 xopt-2.2.2/xopt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-04-15 19:26:54.000000 xopt-2.2.2/xopt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 19:26:54.000000 xopt-2.2.2/xopt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-15 19:26:54.000000 xopt-2.2.2/xopt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 19:26:54.000000 xopt-2.2.2/xopt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:30.000000 xopt-2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 19:37:26.000000 xopt-2.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-07 19:37:26.000000 xopt-2.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-05-07 19:37:30.000000 xopt-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8594 2024-05-07 19:37:26.000000 xopt-2.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:30.000000 xopt-2.2.3/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:26.000000 xopt-2.2.3/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-07 19:37:26.000000 xopt-2.2.3/benchmarks/test_mo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-07 19:37:26.000000 xopt-2.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-07 19:37:30.000000 xopt-2.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-07 19:37:26.000000 xopt-2.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:30.000000 xopt-2.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:30.000000 xopt-2.2.3/tests/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:30.000000 xopt-2.2.3/tests/generators/bayesian/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/generators/bayesian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/generators/bayesian/test_bax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/generators/bayesian/test_bayesian_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9245 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/generators/bayesian/test_bayesian_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/generators/bayesian/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/generators/bayesian/test_custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/generators/bayesian/test_expected_improvement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/generators/bayesian/test_hessian_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/generators/bayesian/test_high_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/generators/bayesian/test_mggpo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/generators/bayesian/test_mobo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19856 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/generators/bayesian/test_model_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/generators/bayesian/test_multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/generators/bayesian/test_time_dependent_bo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/generators/bayesian/test_turbo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/generators/bayesian/test_upper_confidence_bound.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/generators/bayesian/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/generators/test_extremum_seeking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/generators/test_latin_hypercube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/generators/test_neldermead.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/generators/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/generators/test_rcds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/test_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/test_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/test_numerical_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/test_perf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/test_vocs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-05-07 19:37:26.000000 xopt-2.2.3/tests/test_xopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78325 2024-05-07 19:37:26.000000 xopt-2.2.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:30.000000 xopt-2.2.3/xopt/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-07 19:37:30.000000 xopt-2.2.3/xopt/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/asynchronous.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18279 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:30.000000 xopt-2.2.3/xopt/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:30.000000 xopt-2.2.3/xopt/generators/bayesian/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:30.000000 xopt-2.2.3/xopt/generators/bayesian/bax/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/bax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/bax/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/bax/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/bax_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/bayesian_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28488 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/bayesian_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:30.000000 xopt-2.2.3/xopt/generators/bayesian/custom_botorch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/custom_botorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/custom_botorch/constrained_acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/custom_botorch/hessian_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/custom_botorch/heteroskedastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/custom_botorch/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/custom_botorch/log_acquisition_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/custom_botorch/multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/custom_botorch/proximal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/expected_improvement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/mggpo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/mobo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:30.000000 xopt-2.2.3/xopt/generators/bayesian/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/models/prior_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10944 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/models/standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/models/time_dependent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/objectives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/time_dependent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/turbo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/upper_confidence_bound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36387 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/bayesian/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:30.000000 xopt-2.2.3/xopt/generators/es/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/es/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/es/extremumseeking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:30.000000 xopt-2.2.3/xopt/generators/ga/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/ga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/ga/cnsga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/ga/deap_creator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3137 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/ga/deap_fitness_with_constraints.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3138 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/ga/fitness_with_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:30.000000 xopt-2.2.3/xopt/generators/rcds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/rcds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14100 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/rcds/rcds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:30.000000 xopt-2.2.3/xopt/generators/scipy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/scipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/scipy/latin_hypercube.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17535 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/scipy/neldermead.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/generators/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:30.000000 xopt-2.2.3/xopt/mpi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/mpi/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/numerical_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26153 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/pydantic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:30.000000 xopt-2.2.3/xopt/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/resources/benchmarking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:30.000000 xopt-2.2.3/xopt/resources/test_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/resources/test_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/resources/test_functions/ackley_20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/resources/test_functions/modified_tnk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/resources/test_functions/multi_objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/resources/test_functions/problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/resources/test_functions/rosenbrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/resources/test_functions/sinusoid_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/resources/test_functions/sphere_100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/resources/test_functions/sphere_20.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/resources/test_functions/sphere_50.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/resources/test_functions/tnk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/resources/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9762 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25378 2024-05-07 19:37:26.000000 xopt-2.2.3/xopt/vocs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:37:30.000000 xopt-2.2.3/xopt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-05-07 19:37:30.000000 xopt-2.2.3/xopt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-05-07 19:37:30.000000 xopt-2.2.3/xopt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:37:30.000000 xopt-2.2.3/xopt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-07 19:37:30.000000 xopt-2.2.3/xopt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 19:37:30.000000 xopt-2.2.3/xopt.egg-info/top_level.txt
```

### Comparing `xopt-2.2.2/LICENSE` & `xopt-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/PKG-INFO` & `xopt-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xopt
-Version: 2.2.2
+Version: 2.2.3
 Home-page: https://github.com/ChristopherMayes/xopt
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <img src="docs/assets/Xopt-logo.png", width="200">
```

### Comparing `xopt-2.2.2/README.md` & `xopt-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/benchmarks/test_mo.py` & `xopt-2.2.3/benchmarks/test_mo.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/setup.py` & `xopt-2.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/tests/generators/bayesian/test_bax.py` & `xopt-2.2.3/tests/generators/bayesian/test_bax.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/tests/generators/bayesian/test_bayesian_exploration.py` & `xopt-2.2.3/tests/generators/bayesian/test_bayesian_exploration.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/tests/generators/bayesian/test_bayesian_generator.py` & `xopt-2.2.3/tests/generators/bayesian/test_bayesian_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,7 +235,16 @@
         data = deepcopy(TEST_VOCS_DATA)
         gen.add_data(data)
         model = gen.train_model()
         assert torch.allclose(
             model.models[0].input_transform.bounds,
             torch.tensor(((0, 0), (1, 10))).double(),
         )
+
+        # test bad fixed feature name
+        gen = BayesianGenerator(vocs=TEST_VOCS_BASE)
+        gen.fixed_features = {"bad_name": 3.0}
+        data = deepcopy(TEST_VOCS_DATA)
+        gen.add_data(data)
+
+        with pytest.raises(KeyError):
+            gen.train_model()
```

### Comparing `xopt-2.2.2/tests/generators/bayesian/test_constraints.py` & `xopt-2.2.3/tests/generators/bayesian/test_constraints.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/tests/generators/bayesian/test_custom_model.py` & `xopt-2.2.3/tests/generators/bayesian/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/tests/generators/bayesian/test_expected_improvement.py` & `xopt-2.2.3/tests/generators/bayesian/test_expected_improvement.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/tests/generators/bayesian/test_hessian_kernel.py` & `xopt-2.2.3/tests/generators/bayesian/test_hessian_kernel.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/tests/generators/bayesian/test_high_level.py` & `xopt-2.2.3/tests/generators/bayesian/test_high_level.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/tests/generators/bayesian/test_mggpo.py` & `xopt-2.2.3/tests/generators/bayesian/test_mggpo.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/tests/generators/bayesian/test_mobo.py` & `xopt-2.2.3/tests/generators/bayesian/test_mobo.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/tests/generators/bayesian/test_model_constructor.py` & `xopt-2.2.3/tests/generators/bayesian/test_model_constructor.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/tests/generators/bayesian/test_multi_fidelity.py` & `xopt-2.2.3/tests/generators/bayesian/test_multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/tests/generators/bayesian/test_time_dependent_bo.py` & `xopt-2.2.3/tests/generators/bayesian/test_time_dependent_bo.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/tests/generators/bayesian/test_turbo.py` & `xopt-2.2.3/tests/generators/bayesian/test_turbo.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/tests/generators/bayesian/test_upper_confidence_bound.py` & `xopt-2.2.3/tests/generators/bayesian/test_upper_confidence_bound.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/tests/generators/bayesian/test_utils.py` & `xopt-2.2.3/tests/generators/bayesian/test_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from xopt.resources.testing import TEST_VOCS_BASE
 
 
 class TestUtils:
     def test_mobo_objective(self):
         test_vocs_copy = deepcopy(TEST_VOCS_BASE)
         test_vocs_copy.objectives["y2"] = "MAXIMIZE"
-        obj = create_mobo_objective(test_vocs_copy, tkwargs={})
+        obj = create_mobo_objective(test_vocs_copy)
 
         # test large sample shape
         test_samples = torch.randn(3, 4, 5, 3).double()
         output = obj(test_samples)
         assert output.shape == torch.Size([3, 4, 5, 2])
 
         # test to make sure values are correct - minimize axis should be negated
```

### Comparing `xopt-2.2.2/tests/generators/test_extremum_seeking.py` & `xopt-2.2.3/tests/generators/test_extremum_seeking.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/tests/generators/test_latin_hypercube.py` & `xopt-2.2.3/tests/generators/test_latin_hypercube.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/tests/generators/test_neldermead.py` & `xopt-2.2.3/tests/generators/test_neldermead.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/tests/generators/test_random.py` & `xopt-2.2.3/tests/generators/test_random.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/tests/generators/test_rcds.py` & `xopt-2.2.3/tests/generators/test_rcds.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/tests/test_evaluator.py` & `xopt-2.2.3/tests/test_evaluator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 
 import numpy as np
 import pandas as pd
 
-from xopt import Evaluator
+from xopt import Evaluator, Xopt
+from xopt.generators import RandomGenerator
 from xopt.vocs import VOCS
 
 
 class TestEvaluator:
     @staticmethod
     def f(x, a=True):
         if a:
@@ -131,7 +132,33 @@
         vocs = VOCS(variables={"x": [0, 1], "y": [0, 1]}, objectives={"f1": "MINIMIZE"})
         in10 = vocs.random_inputs(10)
 
         # Create Executor insance
         executor = ProcessPoolExecutor(max_workers=MAX_WORKERS)
         ev = Evaluator(function=self.f, executor=executor, max_workers=MAX_WORKERS)
         ev.evaluate_data(in10)
+
+    def test_evaluate_return_types(self):
+        def a(input):
+            return {"f": 1.0}
+
+        def b(input):
+            return {"f": [1.0]}
+
+        def c(input):
+            return {"f": np.array(1.0)}
+
+        def d(input):
+            return {"f": [1.0, 1.0]}
+
+        def e(input):
+            return {"f": np.ones(3)}
+
+        vocs = VOCS(variables={"x": [0, 1]}, objectives={"f": "MINIMIZE"})
+
+        for func in [a, b, c, d, e]:
+            evaluator = Evaluator(function=func)
+            generator = RandomGenerator(vocs=vocs)
+
+            X = Xopt(evaluator=evaluator, generator=generator, vocs=vocs)
+
+            X.random_evaluate(5)
```

### Comparing `xopt-2.2.2/tests/test_generator.py` & `xopt-2.2.3/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/tests/test_io.py` & `xopt-2.2.3/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/tests/test_mpi.py` & `xopt-2.2.3/tests/test_mpi.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/tests/test_numerical_optimizer.py` & `xopt-2.2.3/tests/test_numerical_optimizer.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/tests/test_perf.py` & `xopt-2.2.3/tests/test_perf.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/tests/test_pydantic.py` & `xopt-2.2.3/tests/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/tests/test_utils.py` & `xopt-2.2.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/tests/test_vocs.py` & `xopt-2.2.3/tests/test_vocs.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,22 @@
         assert vocs.n_constraints == 0
 
     def test_empty_objectives(self):
         VOCS(
             variables={"x": [0, 1]},
         )
 
+    def test_output_names(self):
+        test_vocs = VOCS(
+            variables={"x": [0, 1]},
+            objectives={"y1": "MINIMIZE"},
+            constraints={"c1": ["GREATER_THAN", 0], "c2": ["LESS_THAN", 0]},
+        )
+        assert test_vocs.output_names == ["y1", "c1", "c2"]
+
     def test_constraint_specification(self):
         good_constraint_list = [
             ["LESS_THAN", 0],
             ["GREATER_THAN", 0],
             ["less_than", 0],
             ["greater_than", 0],
         ]
@@ -230,14 +238,22 @@
         assert val == [0.5]
 
         vocs.constraints = {}
         idx, val, _ = vocs.select_best(test_data)
         assert idx == 1
         assert val == 0.1
 
+        # test error handling
+        with pytest.raises(RuntimeError):
+            vocs.select_best(pd.DataFrame())
+
+        vocs.constraints = {"c1": ["GREATER_THAN", 10.5]}
+        with pytest.raises(RuntimeError):
+            vocs.select_best(pd.DataFrame())
+
     @pytest.mark.filterwarnings("ignore: All-NaN axis encountered")
     def test_cumulative_optimum(self):
         vocs = deepcopy(TEST_VOCS_BASE)
         obj_name = vocs.objective_names[0]
         test_data = pd.DataFrame(
             {
                 obj_name: [np.nan, 0.0, -0.4, 0.6, np.nan, -0.7],
```

### Comparing `xopt-2.2.2/tests/test_xopt.py` & `xopt-2.2.3/tests/test_xopt.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/versioneer.py` & `xopt-2.2.3/versioneer.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/__init__.py` & `xopt-2.2.3/xopt/__init__.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/asynchronous.py` & `xopt-2.2.3/xopt/asynchronous.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/base.py` & `xopt-2.2.3/xopt/base.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/evaluator.py` & `xopt-2.2.3/xopt/evaluator.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generator.py` & `xopt-2.2.3/xopt/generator.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/__init__.py` & `xopt-2.2.3/xopt/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/bayesian/__init__.py` & `xopt-2.2.3/xopt/generators/bayesian/__init__.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/bayesian/base_model.py` & `xopt-2.2.3/xopt/generators/bayesian/base_model.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/bayesian/bax/acquisition.py` & `xopt-2.2.3/xopt/generators/bayesian/bax/acquisition.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/bayesian/bax/algorithms.py` & `xopt-2.2.3/xopt/generators/bayesian/bax/algorithms.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/bayesian/bax_generator.py` & `xopt-2.2.3/xopt/generators/bayesian/bax_generator.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/bayesian/bayesian_exploration.py` & `xopt-2.2.3/xopt/generators/bayesian/bayesian_exploration.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from pydantic_core.core_schema import ValidationInfo
 from torch import Tensor
 
 from xopt.generators.bayesian.bayesian_generator import (
     BayesianGenerator,
     formatted_base_docstring,
 )
-from xopt.generators.bayesian.objectives import create_exploration_objective
 
 
 class BayesianExplorationGenerator(BayesianGenerator):
     name = "bayesian_exploration"
     supports_batch_generation: bool = True
 
     __doc__ = "Bayesian exploration generator\n" + formatted_base_docstring()
@@ -34,20 +33,14 @@
             model,
             sampler=sampler,
             objective=self._get_objective(),
         )
 
         return qPV
 
-    def _get_objective(self):
-        """return exploration objective, which only captures the output of the first
-        model output"""
-
-        return create_exploration_objective(self.vocs, self._tkwargs)
-
 
 class qPosteriorVariance(MCAcquisitionFunction):
     def __init__(
         self,
         model: Model,
         sampler: Optional[MCSampler] = None,
         objective: Optional[MCAcquisitionObjective] = None,
```

### Comparing `xopt-2.2.2/xopt/generators/bayesian/bayesian_generator.py` & `xopt-2.2.3/xopt/generators/bayesian/bayesian_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -371,14 +371,19 @@
         variable_bounds = deepcopy(self.vocs.variables)
 
         # add fixed feature bounds if requested
         if self.fixed_features is not None:
             # get bounds for each fixed_feature (vocs bounds take precedent)
             for key in self.fixed_features:
                 if key not in variable_bounds:
+                    if key not in data:
+                        raise KeyError(
+                            "generator data needs to contain fixed feature "
+                            f"column name `{key}`"
+                        )
                     f_data = data[key]
                     bounds = [f_data.min(), f_data.max()]
                     if bounds[1] - bounds[0] < 1e-8:
                         bounds[1] = bounds[0] + 1e-8
                     variable_bounds[key] = bounds
 
         _model = self.gp_constructor.build_model(
@@ -541,19 +546,28 @@
         return sampler
 
     @abstractmethod
     def _get_acquisition(self, model):
         pass
 
     def _get_objective(self):
-        """return default objective (scalar objective) determined by vocs"""
+        """
+        return default objective (scalar objective) determined by vocs
+
+        If objectives are specified the returned function will weight model
+        by +/- 1.0 according to MAXIMIZE/MINIMIZE keys in vocs.
+
+        If no objectives are specified, the returned function will weight observable
+        models by +1.0. This is used in Bayesian exploration.
+
+        """
         return create_mc_objective(self.vocs, self._tkwargs)
 
     def _get_constraint_callables(self):
-        """return default objective (scalar objective) determined by vocs"""
+        """return constratint callable determined by vocs"""
         constraint_callables = create_constraint_callables(self.vocs)
         if len(constraint_callables) == 0:
             constraint_callables = None
         return constraint_callables
 
     @property
     def _tkwargs(self):
@@ -751,15 +765,15 @@
         if self.vocs.n_constraints > 0:
             objective_data = objective_data[
                 self.vocs.feasibility_data(self.data)["feasible"].to_list()
             ]
 
         n_objectives = self.vocs.n_objectives
         weights = torch.zeros(n_objectives)
-        weights = set_botorch_weights(weights, self.vocs)
+        weights = set_botorch_weights(self.vocs).to(**self._tkwargs)
         objective_data = objective_data * weights
 
         # compute hypervolume
         bd = DominatedPartitioning(
             ref_point=self.torch_reference_point, Y=objective_data
         )
         volume = bd.compute_hypervolume().item()
```

### Comparing `xopt-2.2.2/xopt/generators/bayesian/custom_botorch/constrained_acquisition.py` & `xopt-2.2.3/xopt/generators/bayesian/custom_botorch/constrained_acquisition.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/bayesian/custom_botorch/hessian_kernel.py` & `xopt-2.2.3/xopt/generators/bayesian/custom_botorch/hessian_kernel.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/bayesian/custom_botorch/heteroskedastic.py` & `xopt-2.2.3/xopt/generators/bayesian/custom_botorch/heteroskedastic.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/bayesian/custom_botorch/identity.py` & `xopt-2.2.3/xopt/generators/bayesian/custom_botorch/identity.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/bayesian/custom_botorch/log_acquisition_function.py` & `xopt-2.2.3/xopt/generators/bayesian/custom_botorch/log_acquisition_function.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/bayesian/custom_botorch/multi_fidelity.py` & `xopt-2.2.3/xopt/generators/bayesian/custom_botorch/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/bayesian/custom_botorch/proximal.py` & `xopt-2.2.3/xopt/generators/bayesian/custom_botorch/proximal.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/bayesian/expected_improvement.py` & `xopt-2.2.3/xopt/generators/bayesian/expected_improvement.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,14 @@
                 model,
                 best_f=best_f,
                 sampler=sampler,
                 objective=self._get_objective(),
             )
         else:
             # analytic acquisition function for single candidate generation
-            weights = torch.zeros(self.vocs.n_outputs).to(**self._tkwargs)
-            weights = set_botorch_weights(weights, self.vocs)
+            weights = set_botorch_weights(self.vocs).to(**self._tkwargs)
             posterior_transform = ScalarizedPosteriorTransform(weights)
             acq = ExpectedImprovement(
                 model, best_f=best_f, posterior_transform=posterior_transform
             )
 
         return acq
```

### Comparing `xopt-2.2.2/xopt/generators/bayesian/mggpo.py` & `xopt-2.2.3/xopt/generators/bayesian/mggpo.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             raise ValueError("model cannot be None")
 
         # get base acquisition function
         acq = self._get_acquisition(model)
         return acq
 
     def _get_objective(self):
-        return create_mobo_objective(self.vocs, self._tkwargs)
+        return create_mobo_objective(self.vocs)
 
     def _get_acquisition(self, model):
         # get reference point from data
         inputs = self.get_input_data(self.data)
         sampler = self._get_sampler(model)
 
         acq = qNoisyExpectedHypervolumeImprovement(
```

### Comparing `xopt-2.2.2/xopt/generators/bayesian/mobo.py` & `xopt-2.2.3/xopt/generators/bayesian/mobo.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class MOBOGenerator(MultiObjectiveBayesianGenerator):
     name = "mobo"
     __doc__ = """Implements Multi-Objective Bayesian Optimization using the Expected
             Hypervolume Improvement acquisition function"""
 
     def _get_objective(self):
-        return create_mobo_objective(self.vocs, self._tkwargs)
+        return create_mobo_objective(self.vocs)
 
     def get_acquisition(self, model):
         """
         Returns a function that can be used to evaluate the acquisition function
         """
         if model is None:
             raise ValueError("model cannot be None")
```

### Comparing `xopt-2.2.2/xopt/generators/bayesian/models/prior_mean.py` & `xopt-2.2.3/xopt/generators/bayesian/models/prior_mean.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/bayesian/models/standard.py` & `xopt-2.2.3/xopt/generators/bayesian/models/standard.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/bayesian/models/time_dependent.py` & `xopt-2.2.3/xopt/generators/bayesian/models/time_dependent.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/bayesian/multi_fidelity.py` & `xopt-2.2.3/xopt/generators/bayesian/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/bayesian/objectives.py` & `xopt-2.2.3/xopt/generators/bayesian/objectives.py`

 * *Files 22% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         return Z[..., output_names.index(name)] - constraint[1]
     elif constraint[0] == "GREATER_THAN":
         return -(Z[..., output_names.index(name)] - constraint[1])
 
 
 def create_constraint_callables(vocs):
     if vocs.constraints is not None:
-        constraint_names = list(vocs.constraints.keys())
+        constraint_names = vocs.constraint_names
         constraint_callables = []
         for name in constraint_names:
             constraint_callables += [
                 partial(
                     constraint_function,
                     vocs=vocs,
                     name=name,
@@ -58,41 +58,27 @@
 
 
 def create_mc_objective(vocs, tkwargs):
     """
     create the objective object
 
     """
-    n_outputs = vocs.n_outputs
-    weights = torch.zeros(n_outputs).to(**tkwargs)
-
-    weights = set_botorch_weights(weights, vocs)
-
-    def obj_callable(Z, X=None):
-        return torch.matmul(Z, weights.reshape(-1, 1)).squeeze(-1)
-
-    return GenericMCObjective(obj_callable)
-
-
-def create_exploration_objective(vocs, tkwargs):
-    n_outputs = vocs.n_outputs
-    weights = torch.zeros(n_outputs).to(**tkwargs)
-    weights[0] = 1.0
+    weights = set_botorch_weights(vocs)
 
     def obj_callable(Z, X=None):
         return torch.matmul(Z, weights.reshape(-1, 1)).squeeze(-1)
 
     return GenericMCObjective(obj_callable)
 
 
-def create_mobo_objective(vocs, tkwargs):
+def create_mobo_objective(vocs):
     """
     botorch assumes maximization so we need to negate any objectives that have
     minimize keyword and zero out anything that is a constraint
     """
-    n_objectives = vocs.n_objectives
-    weights = torch.zeros(n_objectives).to(**tkwargs)
-    weights = set_botorch_weights(weights, vocs)
+    output_names = vocs.output_names
+    objective_indicies = [output_names.index(name) for name in vocs.objectives]
+    weights = set_botorch_weights(vocs)[objective_indicies]
 
     return WeightedMCMultiOutputObjective(
-        weights, outcomes=list(range(vocs.n_objectives)), num_outcomes=vocs.n_objectives
+        weights, outcomes=objective_indicies, num_outcomes=vocs.n_objectives
     )
```

### Comparing `xopt-2.2.2/xopt/generators/bayesian/time_dependent.py` & `xopt-2.2.3/xopt/generators/bayesian/time_dependent.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/bayesian/turbo.py` & `xopt-2.2.3/xopt/generators/bayesian/turbo.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/bayesian/upper_confidence_bound.py` & `xopt-2.2.3/xopt/generators/bayesian/upper_confidence_bound.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import warnings
 
-import torch
 from botorch.acquisition import (
     qUpperConfidenceBound,
     ScalarizedPosteriorTransform,
     UpperConfidenceBound,
 )
 from pydantic import Field, field_validator
 
@@ -58,16 +57,15 @@
                 model,
                 sampler=sampler,
                 objective=self._get_objective(),
                 beta=self.beta,
             )
         else:
             # analytic acquisition function for single candidate generation
-            weights = torch.zeros(self.vocs.n_outputs).to(**self._tkwargs)
-            weights = set_botorch_weights(weights, self.vocs)
+            weights = set_botorch_weights(self.vocs)
             posterior_transform = ScalarizedPosteriorTransform(weights)
             acq = UpperConfidenceBound(
                 model, beta=self.beta, posterior_transform=posterior_transform
             )
 
         return acq
```

### Comparing `xopt-2.2.2/xopt/generators/es/extremumseeking.py` & `xopt-2.2.3/xopt/generators/es/extremumseeking.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/ga/cnsga.py` & `xopt-2.2.3/xopt/generators/ga/cnsga.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/ga/deap_creator.py` & `xopt-2.2.3/xopt/generators/ga/deap_creator.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/ga/deap_fitness_with_constraints.py` & `xopt-2.2.3/xopt/generators/ga/deap_fitness_with_constraints.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/ga/fitness_with_constraints.py` & `xopt-2.2.3/xopt/generators/ga/fitness_with_constraints.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/rcds/rcds.py` & `xopt-2.2.3/xopt/generators/rcds/rcds.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/scipy/latin_hypercube.py` & `xopt-2.2.3/xopt/generators/scipy/latin_hypercube.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/scipy/neldermead.py` & `xopt-2.2.3/xopt/generators/scipy/neldermead.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/generators/utils.py` & `xopt-2.2.3/xopt/generators/utils.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/log.py` & `xopt-2.2.3/xopt/log.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/mpi/run.py` & `xopt-2.2.3/xopt/mpi/run.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/numerical_optimizer.py` & `xopt-2.2.3/xopt/numerical_optimizer.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/pydantic.py` & `xopt-2.2.3/xopt/pydantic.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/resources/benchmarking.py` & `xopt-2.2.3/xopt/resources/benchmarking.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/resources/test_functions/ackley_20.py` & `xopt-2.2.3/xopt/resources/test_functions/ackley_20.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/resources/test_functions/modified_tnk.py` & `xopt-2.2.3/xopt/resources/test_functions/modified_tnk.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/resources/test_functions/multi_objective.py` & `xopt-2.2.3/xopt/resources/test_functions/multi_objective.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/resources/test_functions/problem.py` & `xopt-2.2.3/xopt/resources/test_functions/problem.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/resources/test_functions/rosenbrock.py` & `xopt-2.2.3/xopt/resources/test_functions/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/resources/test_functions/tnk.py` & `xopt-2.2.3/xopt/resources/test_functions/tnk.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/resources/testing.py` & `xopt-2.2.3/xopt/resources/testing.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.2/xopt/utils.py` & `xopt-2.2.3/xopt/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -285,15 +285,19 @@
     """explode all data columns in dataframes that are lists or np.arrays"""
     # TODO: rework the whole list return type handling - this is really slow
     list_types = []
     lengths = []
     for name, val in data.iloc[0].items():
         if isinstance(val, (list, np.ndarray)):
             list_types.append(name)
-            lengths.append(len(val))
+            try:
+                lengths.append(len(val))
+            except TypeError:
+                # handle case when a zero length ndarray is passed
+                lengths.append(1)
     if len(list_types) > 0:
         if len(set(lengths)) > 1:
             raise ValueError("evaluator outputs that are lists must match in size")
 
         if data.shape[0] == 1:
             # Fast path for most common experimental case of 1 candidate per step
             df = _explode_pandas_modified(data, list_types, lengths[0])
```

### Comparing `xopt-2.2.2/xopt/vocs.py` & `xopt-2.2.3/xopt/vocs.py`

 * *Files 1% similar despite different names*

```diff
@@ -541,15 +541,23 @@
             params: input parameters that give the best point
         """
         if self.n_objectives != 1:
             raise NotImplementedError(
                 "cannot select best point when n_objectives is not 1"
             )
 
+        if data.empty:
+            raise RuntimeError("cannot select best point if dataframe is empty")
+
         feasible_data = self.feasibility_data(data)
+        if feasible_data.empty:
+            raise RuntimeError(
+                "cannot select best point if no points satisfy the given constraints"
+            )
+
         ascending_flag = {"MINIMIZE": True, "MAXIMIZE": False}
         obj = self.objectives[self.objective_names[0]]
         obj_name = self.objective_names[0]
         res = data[feasible_data["feasible"]].sort_values(
             obj_name, ascending=ascending_flag[obj]
         )[obj_name][:n]
```

### Comparing `xopt-2.2.2/xopt.egg-info/PKG-INFO` & `xopt-2.2.3/xopt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xopt
-Version: 2.2.2
+Version: 2.2.3
 Home-page: https://github.com/ChristopherMayes/xopt
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <img src="docs/assets/Xopt-logo.png", width="200">
```

### Comparing `xopt-2.2.2/xopt.egg-info/SOURCES.txt` & `xopt-2.2.3/xopt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

