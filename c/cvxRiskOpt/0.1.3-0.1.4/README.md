# Comparing `tmp/cvxriskopt-0.1.3.tar.gz` & `tmp/cvxriskopt-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxriskopt-0.1.3.tar", last modified: Wed May  1 00:59:23 2024, max compression
+gzip compressed data, was "cvxriskopt-0.1.4.tar", last modified: Tue May  7 19:23:41 2024, max compression
```

## Comparing `cvxriskopt-0.1.3.tar` & `cvxriskopt-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 sleiman    (501) staff       (20)        0 2024-05-01 00:59:23.962991 cvxriskopt-0.1.3/
--rw-r--r--   0 sleiman    (501) staff       (20)    35149 2024-04-24 22:44:20.000000 cvxriskopt-0.1.3/LICENSE
--rw-r--r--   0 sleiman    (501) staff       (20)     1771 2024-05-01 00:59:23.962829 cvxriskopt-0.1.3/PKG-INFO
--rw-r--r--   0 sleiman    (501) staff       (20)      964 2024-04-28 17:00:05.000000 cvxriskopt-0.1.3/README.md
-drwxr-xr-x   0 sleiman    (501) staff       (20)        0 2024-05-01 00:59:23.960245 cvxriskopt-0.1.3/cvxRiskOpt/
--rw-r--r--   0 sleiman    (501) staff       (20)        0 2024-04-09 19:49:24.000000 cvxriskopt-0.1.3/cvxRiskOpt/__init__.py
--rw-r--r--   0 sleiman    (501) staff       (20)    20512 2024-04-30 20:57:20.000000 cvxriskopt-0.1.3/cvxRiskOpt/cclp_risk_opt.py
--rw-r--r--   0 sleiman    (501) staff       (20)     9410 2024-04-30 21:57:24.000000 cvxriskopt-0.1.3/cvxRiskOpt/mpc_helpers.py
--rw-r--r--   0 sleiman    (501) staff       (20)    21710 2024-05-01 00:19:34.000000 cvxriskopt-0.1.3/cvxRiskOpt/wass_risk_opt_pb.py
-drwxr-xr-x   0 sleiman    (501) staff       (20)        0 2024-05-01 00:59:23.962467 cvxriskopt-0.1.3/cvxRiskOpt.egg-info/
--rw-r--r--   0 sleiman    (501) staff       (20)     1771 2024-05-01 00:59:23.000000 cvxriskopt-0.1.3/cvxRiskOpt.egg-info/PKG-INFO
--rw-r--r--   0 sleiman    (501) staff       (20)      398 2024-05-01 00:59:23.000000 cvxriskopt-0.1.3/cvxRiskOpt.egg-info/SOURCES.txt
--rw-r--r--   0 sleiman    (501) staff       (20)        1 2024-05-01 00:59:23.000000 cvxriskopt-0.1.3/cvxRiskOpt.egg-info/dependency_links.txt
--rw-r--r--   0 sleiman    (501) staff       (20)      126 2024-05-01 00:59:23.000000 cvxriskopt-0.1.3/cvxRiskOpt.egg-info/requires.txt
--rw-r--r--   0 sleiman    (501) staff       (20)       11 2024-05-01 00:59:23.000000 cvxriskopt-0.1.3/cvxRiskOpt.egg-info/top_level.txt
--rw-r--r--   0 sleiman    (501) staff       (20)       38 2024-05-01 00:59:23.963030 cvxriskopt-0.1.3/setup.cfg
--rw-r--r--   0 sleiman    (501) staff       (20)     1018 2024-05-01 00:52:26.000000 cvxriskopt-0.1.3/setup.py
-drwxr-xr-x   0 sleiman    (501) staff       (20)        0 2024-05-01 00:59:23.962059 cvxriskopt-0.1.3/tests/
--rw-r--r--   0 sleiman    (501) staff       (20)    12028 2024-04-24 23:38:45.000000 cvxriskopt-0.1.3/tests/test_cclp_risk_opt.py
--rw-r--r--   0 sleiman    (501) staff       (20)     2746 2024-04-24 22:52:27.000000 cvxriskopt-0.1.3/tests/test_mpc_helpers_functions.py
--rw-r--r--   0 sleiman    (501) staff       (20)    26992 2024-05-01 00:47:28.000000 cvxriskopt-0.1.3/tests/test_wass_risk_opt_pb.py
+drwxr-xr-x   0 sleiman    (501) staff       (20)        0 2024-05-07 19:23:41.859899 cvxriskopt-0.1.4/
+-rw-r--r--   0 sleiman    (501) staff       (20)    35149 2024-05-01 16:56:06.000000 cvxriskopt-0.1.4/LICENSE
+-rw-r--r--   0 sleiman    (501) staff       (20)     1771 2024-05-07 19:23:41.859711 cvxriskopt-0.1.4/PKG-INFO
+-rw-r--r--   0 sleiman    (501) staff       (20)      964 2024-05-01 16:56:06.000000 cvxriskopt-0.1.4/README.md
+drwxr-xr-x   0 sleiman    (501) staff       (20)        0 2024-05-07 19:23:41.857733 cvxriskopt-0.1.4/cvxRiskOpt/
+-rw-r--r--   0 sleiman    (501) staff       (20)        0 2024-05-01 16:56:06.000000 cvxriskopt-0.1.4/cvxRiskOpt/__init__.py
+-rw-r--r--   0 sleiman    (501) staff       (20)    20660 2024-05-06 03:26:48.000000 cvxriskopt-0.1.4/cvxRiskOpt/cclp_risk_opt.py
+-rw-r--r--   0 sleiman    (501) staff       (20)     9410 2024-05-01 16:56:06.000000 cvxriskopt-0.1.4/cvxRiskOpt/mpc_helpers.py
+-rw-r--r--   0 sleiman    (501) staff       (20)    21710 2024-05-01 16:56:06.000000 cvxriskopt-0.1.4/cvxRiskOpt/wass_risk_opt_pb.py
+drwxr-xr-x   0 sleiman    (501) staff       (20)        0 2024-05-07 19:23:41.859365 cvxriskopt-0.1.4/cvxRiskOpt.egg-info/
+-rw-r--r--   0 sleiman    (501) staff       (20)     1771 2024-05-07 19:23:41.000000 cvxriskopt-0.1.4/cvxRiskOpt.egg-info/PKG-INFO
+-rw-r--r--   0 sleiman    (501) staff       (20)      398 2024-05-07 19:23:41.000000 cvxriskopt-0.1.4/cvxRiskOpt.egg-info/SOURCES.txt
+-rw-r--r--   0 sleiman    (501) staff       (20)        1 2024-05-07 19:23:41.000000 cvxriskopt-0.1.4/cvxRiskOpt.egg-info/dependency_links.txt
+-rw-r--r--   0 sleiman    (501) staff       (20)      126 2024-05-07 19:23:41.000000 cvxriskopt-0.1.4/cvxRiskOpt.egg-info/requires.txt
+-rw-r--r--   0 sleiman    (501) staff       (20)       11 2024-05-07 19:23:41.000000 cvxriskopt-0.1.4/cvxRiskOpt.egg-info/top_level.txt
+-rw-r--r--   0 sleiman    (501) staff       (20)       38 2024-05-07 19:23:41.859938 cvxriskopt-0.1.4/setup.cfg
+-rw-r--r--   0 sleiman    (501) staff       (20)     1018 2024-05-07 19:19:32.000000 cvxriskopt-0.1.4/setup.py
+drwxr-xr-x   0 sleiman    (501) staff       (20)        0 2024-05-07 19:23:41.858905 cvxriskopt-0.1.4/tests/
+-rw-r--r--   0 sleiman    (501) staff       (20)    14514 2024-05-06 20:06:31.000000 cvxriskopt-0.1.4/tests/test_cclp_risk_opt.py
+-rw-r--r--   0 sleiman    (501) staff       (20)     2746 2024-05-01 16:56:06.000000 cvxriskopt-0.1.4/tests/test_mpc_helpers_functions.py
+-rw-r--r--   0 sleiman    (501) staff       (20)    26992 2024-05-01 16:56:06.000000 cvxriskopt-0.1.4/tests/test_wass_risk_opt_pb.py
```

### Comparing `cvxriskopt-0.1.3/LICENSE` & `cvxriskopt-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxriskopt-0.1.3/PKG-INFO` & `cvxriskopt-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxRiskOpt
-Version: 0.1.3
+Version: 0.1.4
 Summary: Risk-Based Optimization tool using CVXPY and CVXPYgen
 Home-page: https://github.com/TSummersLab/cvxRiskOpt
 Author: Sleiman Safaoui, Tyler Summers
 Author-email: snsafaoui@gmail.com, tyler.summers@utdallas.edu
 Maintainer: Sleiman Safaoui
 Maintainer-email: snsafaoui@gmail.com
 License: GPL-3.0
```

### Comparing `cvxriskopt-0.1.3/README.md` & `cvxriskopt-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `cvxriskopt-0.1.3/cvxRiskOpt/cclp_risk_opt.py` & `cvxriskopt-0.1.4/cvxRiskOpt/cclp_risk_opt.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,14 +84,16 @@
     if not assume_sym:
         scipy.linalg.issymmetric(mat)
     if not assume_psd:
         psd = np.all(np.linalg.eigvals(mat) >= 0)
         if not psd:
             raise ValueError("Input matrix mat is not PSD")
     matsqrt = scipy.linalg.sqrtm(mat)
+    if isinstance(v, np.ndarray):
+        return np.linalg.norm(matsqrt @ v)
     return cp.norm(matsqrt @ v)
 
 
 def _check_b_term(b: int | float | cp.Variable | cp.Expression | None,
                   b_present: bool):
     """
     Checks the b term in the CCLP.
@@ -140,14 +142,16 @@
     if a is not None and xi1_hat is not None and gam11 is not None:
         a_xi1_present = True
         # check a
         if isinstance(a, (int, float)):
             a_len = 1
             a = np.array([a])
         elif isinstance(a, (cp.Variable, cp.Expression)):
+            if a.shape == ():
+                a = cp.reshape(a, (1, ))
             a_len = a.shape[0]
         elif isinstance(a, list):
             a = np.array(a)
             if a.ndim > 1:
                 raise ValueError("a can only be (m,)-dimensional")
             a_len = a.shape[0]
         elif isinstance(a, np.ndarray):
```

### Comparing `cvxriskopt-0.1.3/cvxRiskOpt/mpc_helpers.py` & `cvxriskopt-0.1.4/cvxRiskOpt/mpc_helpers.py`

 * *Files identical despite different names*

### Comparing `cvxriskopt-0.1.3/cvxRiskOpt/wass_risk_opt_pb.py` & `cvxriskopt-0.1.4/cvxRiskOpt/wass_risk_opt_pb.py`

 * *Files identical despite different names*

### Comparing `cvxriskopt-0.1.3/cvxRiskOpt.egg-info/PKG-INFO` & `cvxriskopt-0.1.4/cvxRiskOpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxRiskOpt
-Version: 0.1.3
+Version: 0.1.4
 Summary: Risk-Based Optimization tool using CVXPY and CVXPYgen
 Home-page: https://github.com/TSummersLab/cvxRiskOpt
 Author: Sleiman Safaoui, Tyler Summers
 Author-email: snsafaoui@gmail.com, tyler.summers@utdallas.edu
 Maintainer: Sleiman Safaoui
 Maintainer-email: snsafaoui@gmail.com
 License: GPL-3.0
```

### Comparing `cvxriskopt-0.1.3/setup.py` & `cvxriskopt-0.1.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup
 
 setup(
     name="cvxRiskOpt",
-    version="0.1.3",
+    version="0.1.4",
     description="Risk-Based Optimization tool using CVXPY and CVXPYgen",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Sleiman Safaoui, Tyler Summers",
     author_email="snsafaoui@gmail.com, tyler.summers@utdallas.edu",
     maintainer="Sleiman Safaoui",
     maintainer_email="snsafaoui@gmail.com",
```

### Comparing `cvxriskopt-0.1.3/tests/test_cclp_risk_opt.py` & `cvxriskopt-0.1.4/tests/test_cclp_risk_opt.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 import numpy as np
 import cvxpy as cp
 
-VERBOSE = True  # set to True to print additional data
+VERBOSE = False  # set to True to print additional data
 
 
 class TestCCLPRiskOptHelperFunctions(unittest.TestCase):
     def test_check_b_term(self):
         from cvxRiskOpt.cclp_risk_opt import _check_b_term
 
         # Test case: b is not None and is an integer
@@ -293,14 +293,62 @@
             _det_cclp(kappa_e, a, b, xi1_hat, xi2_hat, gam11, gam12, gam22, a_xi1_present, xi2_present, b_present,
                       assume_sym, assume_psd)
 
         # TODO: ADD TEST CASES FOR THE SPECIAL CASES
 
 
 class TestCCLPRiskOptFunctions(unittest.TestCase):
+    def test_cclp_gauss(self):
+        import cvxpy as cp
+        from cvxRiskOpt.cclp_risk_opt import cclp_gauss
+        from scipy.stats import norm as gauss
+        from scipy.linalg import sqrtm
+        # simple test for Prob(x * xi + b <= 0) >= 1-eps
+        # where
+        # x is a decision variable
+        # xi is a random variable
+        # b is a constant
+        eps = 0.1
+
+        if VERBOSE:
+            print("~~~~~~~~~")
+        xi_mean = 0
+        xi_var = 0.01
+        x = cp.Variable(name='x')
+        b = 1
+        constr = cclp_gauss(eps, a=x, b=b, xi1_hat=xi_mean, gam11=xi_var)
+        known_reform = gauss.ppf(1-eps) * cp.norm(np.sqrt(xi_var) * x) + x * xi_mean + b <= 0
+        if VERBOSE:
+            print(constr.expr)
+            print(known_reform)
+
+            print("~~~~~~~~~")
+        xi_mean = np.array([0, 0])
+        xi_var = np.diag([0.01, 0.1])
+        x = cp.Variable(2, name='x')
+        b = 1
+        constr = cclp_gauss(eps, a=x, b=b, xi1_hat=xi_mean, gam11=xi_var)
+        known_reform = gauss.ppf(1 - eps) * cp.norm(sqrtm(xi_var) @ x) + (x @ xi_mean + b) <= 0
+        if VERBOSE:
+            print(constr.expr)
+            print(known_reform.expr)
+            # print(str(constr.expr) == str(known_reform.expr))
+
+            print("~~~~~~~~~")
+        a = np.array([1, 0])
+        x = cp.Variable(2, name='x')
+        xi_mean = np.array([0, 0]) + x
+        xi_var = np.diag([0.01, 0.1])
+        b = 0
+        constr = cclp_gauss(eps, a=a, b=b, xi1_hat=xi_mean, gam11=xi_var)
+        known_reform = gauss.ppf(1 - eps) * cp.norm(sqrtm(xi_var) @ a) + (a @ xi_mean + b) <= 0
+        if VERBOSE:
+            print(constr.expr)
+            print(known_reform.expr)
+
     def test_simple_1D_mpc(self):
         from examples.cclp_mpc import simple_1d_mpc
         x1, u1 = simple_1d_mpc(use_cpg=False, gen_cpg=False, with_cclp=False, seed=1)
         x2, u2 = simple_1d_mpc(use_cpg=False, gen_cpg=False, with_cclp=True, seed=1)
         if len(x1) == len(x2):
             self.assertFalse(np.allclose(x1, x2, rtol=1e-4, atol=1e-4))
         if len(u1) == len(u2):
@@ -310,10 +358,25 @@
         from examples.cclp_mpc import simple_2d_mpc
         simple_2d_mpc(use_cpg=False, gen_cpg=False, plot_res=False)
 
     def test_hvac_mpc(self):
         from examples.cclp_mpc import hvac_mpc_time_varying_constraints
         hvac_mpc_time_varying_constraints(plot_res=False)
 
+    def test_hvac_mpc_reg(self):
+        from examples.cclp_mpc import temp_mpc_regulator_time_varying_constraints
+        temp_mpc_regulator_time_varying_constraints(plot_res=False)
+
+    def test_portfolio_opt(self):
+        from examples.cclp_portfolio_optimization import portfolio_optimization, moment_portfolio_optimization
+        solver = cp.CLARABEL
+        portfolio_optimization(solver=solver, verbose=VERBOSE)
+        moment_portfolio_optimization(num_sim=1, use_cpg=False, gen_code=False, solver=solver)
+
+    def test_production_opt(self):
+        from examples.cclp_safe_production_optimization import production_optimization
+        cvxpy_x, cro_x = production_optimization(verbose=VERBOSE)
+        self.assertTrue(np.allclose(cvxpy_x, cro_x, rtol=1e-4, atol=1e-4))
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cvxriskopt-0.1.3/tests/test_mpc_helpers_functions.py` & `cvxriskopt-0.1.4/tests/test_mpc_helpers_functions.py`

 * *Files identical despite different names*

### Comparing `cvxriskopt-0.1.3/tests/test_wass_risk_opt_pb.py` & `cvxriskopt-0.1.4/tests/test_wass_risk_opt_pb.py`

 * *Files identical despite different names*

