# Comparing `tmp/jax_sysid-0.4.1.tar.gz` & `tmp/jax_sysid-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax_sysid-0.4.1.tar", last modified: Sun May  5 08:18:06 2024, max compression
+gzip compressed data, was "jax_sysid-0.4.2.tar", last modified: Tue May  7 20:28:20 2024, max compression
```

## Comparing `jax_sysid-0.4.1.tar` & `jax_sysid-0.4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-05-05 08:18:06.960465 jax_sysid-0.4.1/
--rw-r--r--   0 bemporad   (501) staff       (20)    11345 2024-03-01 16:55:21.000000 jax_sysid-0.4.1/LICENSE.txt
--rw-r--r--   0 bemporad   (501) staff       (20)    14758 2024-05-05 08:18:06.960272 jax_sysid-0.4.1/PKG-INFO
--rw-r--r--   0 bemporad   (501) staff       (20)    13958 2024-05-04 08:02:06.000000 jax_sysid-0.4.1/README.md
--rw-r--r--   0 bemporad   (501) staff       (20)      801 2024-05-05 08:15:45.000000 jax_sysid-0.4.1/pyproject.toml
--rw-r--r--   0 bemporad   (501) staff       (20)       38 2024-05-05 08:18:06.960501 jax_sysid-0.4.1/setup.cfg
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-05-05 08:18:06.958312 jax_sysid-0.4.1/src/
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-05-05 08:18:06.959144 jax_sysid-0.4.1/src/jax_sysid/
--rw-r--r--   0 bemporad   (501) staff       (20)        0 2023-01-10 11:29:35.000000 jax_sysid-0.4.1/src/jax_sysid/__init__.py
--rw-r--r--   0 bemporad   (501) staff       (20)    73696 2024-05-05 08:14:08.000000 jax_sysid-0.4.1/src/jax_sysid/models.py
--rw-r--r--   0 bemporad   (501) staff       (20)    11403 2024-05-03 09:46:56.000000 jax_sysid-0.4.1/src/jax_sysid/utils.py
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-05-05 08:18:06.960052 jax_sysid-0.4.1/src/jax_sysid.egg-info/
--rw-r--r--   0 bemporad   (501) staff       (20)    14758 2024-05-05 08:18:06.000000 jax_sysid-0.4.1/src/jax_sysid.egg-info/PKG-INFO
--rw-r--r--   0 bemporad   (501) staff       (20)      314 2024-05-05 08:18:06.000000 jax_sysid-0.4.1/src/jax_sysid.egg-info/SOURCES.txt
--rw-r--r--   0 bemporad   (501) staff       (20)        1 2024-05-05 08:18:06.000000 jax_sysid-0.4.1/src/jax_sysid.egg-info/dependency_links.txt
--rw-r--r--   0 bemporad   (501) staff       (20)       49 2024-05-05 08:18:06.000000 jax_sysid-0.4.1/src/jax_sysid.egg-info/requires.txt
--rw-r--r--   0 bemporad   (501) staff       (20)       10 2024-05-05 08:18:06.000000 jax_sysid-0.4.1/src/jax_sysid.egg-info/top_level.txt
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-05-05 08:18:06.959861 jax_sysid-0.4.1/tests/
--rw-r--r--   0 bemporad   (501) staff       (20)     5280 2024-03-06 15:24:05.000000 jax_sysid-0.4.1/tests/test_models.py
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-05-07 20:28:20.023343 jax_sysid-0.4.2/
+-rw-r--r--   0 bemporad   (501) staff       (20)    11345 2024-03-01 16:55:21.000000 jax_sysid-0.4.2/LICENSE.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)    15596 2024-05-07 20:28:20.023151 jax_sysid-0.4.2/PKG-INFO
+-rw-r--r--   0 bemporad   (501) staff       (20)    14796 2024-05-07 20:16:38.000000 jax_sysid-0.4.2/README.md
+-rw-r--r--   0 bemporad   (501) staff       (20)      801 2024-05-07 15:43:52.000000 jax_sysid-0.4.2/pyproject.toml
+-rw-r--r--   0 bemporad   (501) staff       (20)       38 2024-05-07 20:28:20.023378 jax_sysid-0.4.2/setup.cfg
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-05-07 20:28:20.020724 jax_sysid-0.4.2/src/
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-05-07 20:28:20.021818 jax_sysid-0.4.2/src/jax_sysid/
+-rw-r--r--   0 bemporad   (501) staff       (20)        0 2023-01-10 11:29:35.000000 jax_sysid-0.4.2/src/jax_sysid/__init__.py
+-rw-r--r--   0 bemporad   (501) staff       (20)    73717 2024-05-07 20:13:31.000000 jax_sysid-0.4.2/src/jax_sysid/models.py
+-rw-r--r--   0 bemporad   (501) staff       (20)    11418 2024-05-07 20:13:35.000000 jax_sysid-0.4.2/src/jax_sysid/utils.py
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-05-07 20:28:20.022942 jax_sysid-0.4.2/src/jax_sysid.egg-info/
+-rw-r--r--   0 bemporad   (501) staff       (20)    15596 2024-05-07 20:28:20.000000 jax_sysid-0.4.2/src/jax_sysid.egg-info/PKG-INFO
+-rw-r--r--   0 bemporad   (501) staff       (20)      314 2024-05-07 20:28:20.000000 jax_sysid-0.4.2/src/jax_sysid.egg-info/SOURCES.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)        1 2024-05-07 20:28:20.000000 jax_sysid-0.4.2/src/jax_sysid.egg-info/dependency_links.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)       49 2024-05-07 20:28:20.000000 jax_sysid-0.4.2/src/jax_sysid.egg-info/requires.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)       10 2024-05-07 20:28:20.000000 jax_sysid-0.4.2/src/jax_sysid.egg-info/top_level.txt
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-05-07 20:28:20.022577 jax_sysid-0.4.2/tests/
+-rw-r--r--   0 bemporad   (501) staff       (20)     5280 2024-03-06 15:24:05.000000 jax_sysid-0.4.2/tests/test_models.py
```

### Comparing `jax_sysid-0.4.1/LICENSE.txt` & `jax_sysid-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jax_sysid-0.4.1/PKG-INFO` & `jax_sysid-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-sysid
-Version: 0.4.1
+Version: 0.4.2
 Summary: jax-sysid - A Python package for linear and nonlinear system identification and nonlinear regression using Jax.
 Author-email: Alberto Bemporad <alberto.bemporad@imtlucca.it>
 Project-URL: Homepage, http://cse.lab.imtlucca.it/~bemporad/jax-sysid
 Keywords: system identification,subspace identification,nonlinear regression
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -18,38 +18,38 @@
 Requires-Dist: flax
 Requires-Dist: tqdm
 Requires-Dist: matplotlib
 Requires-Dist: pmlb
 
 <img src="http://cse.lab.imtlucca.it/~bemporad/jax-sysid/images/jax-sysid-logo.png" alt="jax-sysid" width=40%/>
 
-A Python package based on <a href="https://jax.readthedocs.io"> JAX </a> for linear and nonlinear system identification of state-space models, recurrent neural network (RNN) training, and nonlinear regression.
+A Python package based on <a href="https://jax.readthedocs.io"> JAX </a> for linear and nonlinear system identification of state-space models, recurrent neural network (RNN) training, and nonlinear regression/classification.
  
 # Contents
 
 * [Package description](#description)
 
 * [Installation](#install)
 
 * [Basic usage](#basic-usage)
     * [Linear state-space models](#linear)
     * [Nonlinear system identification and RNNs](#nonlinear)
-    * [Static models and nonlinear regression] (#static)
+    * [Static models and nonlinear regression/classification] (#static)
 
 * [Contributors](#contributors)
 
 * [Citing jax-sysid](#bibliography)
 
 * [License](#license)
 
 
 <a name="description"></a>
 ## Package description 
 
-**jax-sysid** is a Python package based on <a href="https://jax.readthedocs.io"> JAX </a> for linear and nonlinear system identification of state-space models, recurrent neural network (RNN) training, and nonlinear regression. The algorithm can handle L1-regularization and group-Lasso regularization and relies on L-BFGS optimization for accurate modeling, fast convergence, and good sparsification of model coefficients.
+**jax-sysid** is a Python package based on <a href="https://jax.readthedocs.io"> JAX </a> for linear and nonlinear system identification of state-space models, recurrent neural network (RNN) training, and nonlinear regression/classification. The algorithm can handle L1-regularization and group-Lasso regularization and relies on L-BFGS optimization for accurate modeling, fast convergence, and good sparsification of model coefficients.
 
 The package implements the approach described in the following paper:
 
 <a name="cite-Bem24"><a>
 > [1] A. Bemporad, "[Linear and nonlinear system identification under $\ell_1$- and group-Lasso regularization via L-BFGS-B](
 http://arxiv.org/abs/2403.03827)," submitted for publication. Available on arXiv at <a href="http://arxiv.org/abs/2403.03827">
 http://arxiv.org/abs/2403.03827</a>, 2024. [[bib entry](#ref1)]
@@ -324,15 +324,15 @@
 ~~~python
 model.optimization(params_min=lb, params_max=ub, x0_min=xmin, x0_max=xmax, ...)
 ~~~
 
 where `lb` and `ub` are lists of arrays with the same structure as `model.params`, while `xmin` and `xmax` are arrays of the same dimension `model.nx` of the state vector. By default, each value is set equal to `None`, i.e., the corresponding constraint is not enforced. See `example_linear_positive.py` for examples of how to use nonnegative constraints to fit a positive linear system.
 
 <a name="static"></a>
-### Static models and nonlinear regression
+### Static models and nonlinear regression / classification
 The same optimization algorithms used to train dynamical models can be used to train static models, i.e., to solve the nonlinear regression problem:
 
 $$  \min_{z}r(z)+\frac{1}{N}\sum_{k=0}^{N-1} \|y_{k}-f(u_k,\theta)\|_2^2$$
 
 where $z=\theta$ is the vector of model parameters to train and $r(z)$ admits the same
 regularization terms as in the case of dynamical models.
 
@@ -383,14 +383,23 @@
 
 ~~~python
 model.optimization(lbfgs_epochs=500, params_min=lb, params_max=ub)
 ~~~
 
 where `lb` and `ub` are lists of arrays with the same structure as `model.params`. See `example_static_convex.py` for examples of how to use nonnegative constraints to fit input-convex neural networks.
 
+To solve classification problems, you need to define a custom loss function to change the default Mean-Squared-Error loss. For example, to train a classifier for a multi-category classification problem with $K$ classes, you can specify a neural network with a linear output layer generating output predictions $\hat y\in R^K$ and define the associated cross-entropy $\ell(\hat y,y) = -\sum_{k=1}^Ky_k\log\left(\frac{e^{\hat y_k}}{\sum_{j=1}^Ke^{\hat y_j}}\right)$ function as follows: 
+
+~~~python
+def cross_entropy(Yhat,Y):
+    return -jax.numpy.sum(jax.nn.log_softmax(Yhat, axis=1)*Y)/Y.shape[0] 
+model.loss(rho_th=1.e-4, output_loss=cross_entropy)
+~~~
+
+See `example_static_fashion_mist.py` for an example using **Keras** with JAX backend to define the neural network model.
                 
 <a name="contributors"><a>
 ## Contributors
 
 This package was coded by Alberto Bemporad.
```

### Comparing `jax_sysid-0.4.1/README.md` & `jax_sysid-0.4.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 <img src="http://cse.lab.imtlucca.it/~bemporad/jax-sysid/images/jax-sysid-logo.png" alt="jax-sysid" width=40%/>
 
-A Python package based on <a href="https://jax.readthedocs.io"> JAX </a> for linear and nonlinear system identification of state-space models, recurrent neural network (RNN) training, and nonlinear regression.
+A Python package based on <a href="https://jax.readthedocs.io"> JAX </a> for linear and nonlinear system identification of state-space models, recurrent neural network (RNN) training, and nonlinear regression/classification.
  
 # Contents
 
 * [Package description](#description)
 
 * [Installation](#install)
 
 * [Basic usage](#basic-usage)
     * [Linear state-space models](#linear)
     * [Nonlinear system identification and RNNs](#nonlinear)
-    * [Static models and nonlinear regression] (#static)
+    * [Static models and nonlinear regression/classification] (#static)
 
 * [Contributors](#contributors)
 
 * [Citing jax-sysid](#bibliography)
 
 * [License](#license)
 
 
 <a name="description"></a>
 ## Package description 
 
-**jax-sysid** is a Python package based on <a href="https://jax.readthedocs.io"> JAX </a> for linear and nonlinear system identification of state-space models, recurrent neural network (RNN) training, and nonlinear regression. The algorithm can handle L1-regularization and group-Lasso regularization and relies on L-BFGS optimization for accurate modeling, fast convergence, and good sparsification of model coefficients.
+**jax-sysid** is a Python package based on <a href="https://jax.readthedocs.io"> JAX </a> for linear and nonlinear system identification of state-space models, recurrent neural network (RNN) training, and nonlinear regression/classification. The algorithm can handle L1-regularization and group-Lasso regularization and relies on L-BFGS optimization for accurate modeling, fast convergence, and good sparsification of model coefficients.
 
 The package implements the approach described in the following paper:
 
 <a name="cite-Bem24"><a>
 > [1] A. Bemporad, "[Linear and nonlinear system identification under $\ell_1$- and group-Lasso regularization via L-BFGS-B](
 http://arxiv.org/abs/2403.03827)," submitted for publication. Available on arXiv at <a href="http://arxiv.org/abs/2403.03827">
 http://arxiv.org/abs/2403.03827</a>, 2024. [[bib entry](#ref1)]
@@ -302,15 +302,15 @@
 ~~~python
 model.optimization(params_min=lb, params_max=ub, x0_min=xmin, x0_max=xmax, ...)
 ~~~
 
 where `lb` and `ub` are lists of arrays with the same structure as `model.params`, while `xmin` and `xmax` are arrays of the same dimension `model.nx` of the state vector. By default, each value is set equal to `None`, i.e., the corresponding constraint is not enforced. See `example_linear_positive.py` for examples of how to use nonnegative constraints to fit a positive linear system.
 
 <a name="static"></a>
-### Static models and nonlinear regression
+### Static models and nonlinear regression / classification
 The same optimization algorithms used to train dynamical models can be used to train static models, i.e., to solve the nonlinear regression problem:
 
 $$  \min_{z}r(z)+\frac{1}{N}\sum_{k=0}^{N-1} \|y_{k}-f(u_k,\theta)\|_2^2$$
 
 where $z=\theta$ is the vector of model parameters to train and $r(z)$ admits the same
 regularization terms as in the case of dynamical models.
 
@@ -361,14 +361,23 @@
 
 ~~~python
 model.optimization(lbfgs_epochs=500, params_min=lb, params_max=ub)
 ~~~
 
 where `lb` and `ub` are lists of arrays with the same structure as `model.params`. See `example_static_convex.py` for examples of how to use nonnegative constraints to fit input-convex neural networks.
 
+To solve classification problems, you need to define a custom loss function to change the default Mean-Squared-Error loss. For example, to train a classifier for a multi-category classification problem with $K$ classes, you can specify a neural network with a linear output layer generating output predictions $\hat y\in R^K$ and define the associated cross-entropy $\ell(\hat y,y) = -\sum_{k=1}^Ky_k\log\left(\frac{e^{\hat y_k}}{\sum_{j=1}^Ke^{\hat y_j}}\right)$ function as follows: 
+
+~~~python
+def cross_entropy(Yhat,Y):
+    return -jax.numpy.sum(jax.nn.log_softmax(Yhat, axis=1)*Y)/Y.shape[0] 
+model.loss(rho_th=1.e-4, output_loss=cross_entropy)
+~~~
+
+See `example_static_fashion_mist.py` for an example using **Keras** with JAX backend to define the neural network model.
                 
 <a name="contributors"><a>
 ## Contributors
 
 This package was coded by Alberto Bemporad.
```

### Comparing `jax_sysid-0.4.1/pyproject.toml` & `jax_sysid-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jax-sysid"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
   { name="Alberto Bemporad", email="alberto.bemporad@imtlucca.it" },
 ]
 description = "jax-sysid - A Python package for linear and nonlinear system identification and nonlinear regression using Jax."
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = ["numpy","scipy","jax","jaxopt","flax","tqdm","matplotlib","pmlb"]
```

### Comparing `jax_sysid-0.4.1/src/jax_sysid/models.py` & `jax_sysid-0.4.2/src/jax_sysid/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-jax-sysid: A Python package for linear and nonlinear system identification and nonlinear regression using Jax.
+jax-sysid: A Python package for linear and nonlinear system identification and nonlinear regression/classification using JAX.
 
 (C) 2024 A. Bemporad, March 6, 2024
 """
 
 import numpy as np
 import time
 import jax
@@ -1694,15 +1694,15 @@
                     The system parameters.
 
                 Returns
                 -------
                 float
                     The loss value.
                 """
-                Yhat = self.output_fcn(U, th).reshape(-1, 1)
+                Yhat = self.output_fcn(U, th).reshape(-1, self.ny)
                 cost = self.output_loss(Yhat, Y)
                 return cost
 
             t_solve = time.time()
 
             if solver == "Adam":
                 @jax.jit
```

### Comparing `jax_sysid-0.4.1/src/jax_sysid/utils.py` & `jax_sysid-0.4.2/src/jax_sysid/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-jax-sysid: A Python package for linear and nonlinear system identification and nonlinear regression using Jax.
+jax-sysid: A Python package for linear and nonlinear system identification and nonlinear regression/classification using JAX.
 
 Utility functions.
 
 (C) 2024 A. Bemporad, March 6, 2024
 """
 
 import numpy as np
```

### Comparing `jax_sysid-0.4.1/src/jax_sysid.egg-info/PKG-INFO` & `jax_sysid-0.4.2/src/jax_sysid.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-sysid
-Version: 0.4.1
+Version: 0.4.2
 Summary: jax-sysid - A Python package for linear and nonlinear system identification and nonlinear regression using Jax.
 Author-email: Alberto Bemporad <alberto.bemporad@imtlucca.it>
 Project-URL: Homepage, http://cse.lab.imtlucca.it/~bemporad/jax-sysid
 Keywords: system identification,subspace identification,nonlinear regression
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -18,38 +18,38 @@
 Requires-Dist: flax
 Requires-Dist: tqdm
 Requires-Dist: matplotlib
 Requires-Dist: pmlb
 
 <img src="http://cse.lab.imtlucca.it/~bemporad/jax-sysid/images/jax-sysid-logo.png" alt="jax-sysid" width=40%/>
 
-A Python package based on <a href="https://jax.readthedocs.io"> JAX </a> for linear and nonlinear system identification of state-space models, recurrent neural network (RNN) training, and nonlinear regression.
+A Python package based on <a href="https://jax.readthedocs.io"> JAX </a> for linear and nonlinear system identification of state-space models, recurrent neural network (RNN) training, and nonlinear regression/classification.
  
 # Contents
 
 * [Package description](#description)
 
 * [Installation](#install)
 
 * [Basic usage](#basic-usage)
     * [Linear state-space models](#linear)
     * [Nonlinear system identification and RNNs](#nonlinear)
-    * [Static models and nonlinear regression] (#static)
+    * [Static models and nonlinear regression/classification] (#static)
 
 * [Contributors](#contributors)
 
 * [Citing jax-sysid](#bibliography)
 
 * [License](#license)
 
 
 <a name="description"></a>
 ## Package description 
 
-**jax-sysid** is a Python package based on <a href="https://jax.readthedocs.io"> JAX </a> for linear and nonlinear system identification of state-space models, recurrent neural network (RNN) training, and nonlinear regression. The algorithm can handle L1-regularization and group-Lasso regularization and relies on L-BFGS optimization for accurate modeling, fast convergence, and good sparsification of model coefficients.
+**jax-sysid** is a Python package based on <a href="https://jax.readthedocs.io"> JAX </a> for linear and nonlinear system identification of state-space models, recurrent neural network (RNN) training, and nonlinear regression/classification. The algorithm can handle L1-regularization and group-Lasso regularization and relies on L-BFGS optimization for accurate modeling, fast convergence, and good sparsification of model coefficients.
 
 The package implements the approach described in the following paper:
 
 <a name="cite-Bem24"><a>
 > [1] A. Bemporad, "[Linear and nonlinear system identification under $\ell_1$- and group-Lasso regularization via L-BFGS-B](
 http://arxiv.org/abs/2403.03827)," submitted for publication. Available on arXiv at <a href="http://arxiv.org/abs/2403.03827">
 http://arxiv.org/abs/2403.03827</a>, 2024. [[bib entry](#ref1)]
@@ -324,15 +324,15 @@
 ~~~python
 model.optimization(params_min=lb, params_max=ub, x0_min=xmin, x0_max=xmax, ...)
 ~~~
 
 where `lb` and `ub` are lists of arrays with the same structure as `model.params`, while `xmin` and `xmax` are arrays of the same dimension `model.nx` of the state vector. By default, each value is set equal to `None`, i.e., the corresponding constraint is not enforced. See `example_linear_positive.py` for examples of how to use nonnegative constraints to fit a positive linear system.
 
 <a name="static"></a>
-### Static models and nonlinear regression
+### Static models and nonlinear regression / classification
 The same optimization algorithms used to train dynamical models can be used to train static models, i.e., to solve the nonlinear regression problem:
 
 $$  \min_{z}r(z)+\frac{1}{N}\sum_{k=0}^{N-1} \|y_{k}-f(u_k,\theta)\|_2^2$$
 
 where $z=\theta$ is the vector of model parameters to train and $r(z)$ admits the same
 regularization terms as in the case of dynamical models.
 
@@ -383,14 +383,23 @@
 
 ~~~python
 model.optimization(lbfgs_epochs=500, params_min=lb, params_max=ub)
 ~~~
 
 where `lb` and `ub` are lists of arrays with the same structure as `model.params`. See `example_static_convex.py` for examples of how to use nonnegative constraints to fit input-convex neural networks.
 
+To solve classification problems, you need to define a custom loss function to change the default Mean-Squared-Error loss. For example, to train a classifier for a multi-category classification problem with $K$ classes, you can specify a neural network with a linear output layer generating output predictions $\hat y\in R^K$ and define the associated cross-entropy $\ell(\hat y,y) = -\sum_{k=1}^Ky_k\log\left(\frac{e^{\hat y_k}}{\sum_{j=1}^Ke^{\hat y_j}}\right)$ function as follows: 
+
+~~~python
+def cross_entropy(Yhat,Y):
+    return -jax.numpy.sum(jax.nn.log_softmax(Yhat, axis=1)*Y)/Y.shape[0] 
+model.loss(rho_th=1.e-4, output_loss=cross_entropy)
+~~~
+
+See `example_static_fashion_mist.py` for an example using **Keras** with JAX backend to define the neural network model.
                 
 <a name="contributors"><a>
 ## Contributors
 
 This package was coded by Alberto Bemporad.
```

### Comparing `jax_sysid-0.4.1/tests/test_models.py` & `jax_sysid-0.4.2/tests/test_models.py`

 * *Files identical despite different names*

