# Comparing `tmp/harmonic-1.2.1.tar.gz` & `tmp/harmonic-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/cosmomatt/Documents/Software/harmonic/dist/.tmp-y0szrhm2/harmonic-1.2.1.tar", last modified: Mon Feb 19 11:22:35 2024, max compression
+gzip compressed data, was "/Users/cosmomatt/Documents/Software/harmonic/dist/.tmp-enuh_di_/harmonic-1.2.2.tar", last modified: Tue May  7 13:52:10 2024, max compression
```

## Comparing `harmonic-1.2.1.tar` & `harmonic-1.2.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-02-19 11:22:35.584873 harmonic-1.2.1/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4804 2023-11-20 09:28:42.000000 harmonic-1.2.1/.pip_readme.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)    35149 2022-06-30 08:33:43.000000 harmonic-1.2.1/LICENSE.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)      716 2022-06-30 08:33:43.000000 harmonic-1.2.1/LICENSE_EXT.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)       89 2022-06-30 08:33:43.000000 harmonic-1.2.1/MANIFEST.in
--rw-r--r--   0 cosmomatt   (503) staff       (20)     6023 2024-02-19 11:22:35.584522 harmonic-1.2.1/PKG-INFO
--rw-r--r--   0 cosmomatt   (503) staff       (20)     7021 2024-02-19 11:19:09.000000 harmonic-1.2.1/README.rst
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-02-19 11:22:35.575560 harmonic-1.2.1/harmonic/
--rw-r--r--   0 cosmomatt   (503) staff       (20)      178 2023-11-21 14:40:12.000000 harmonic-1.2.1/harmonic/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    15008 2023-11-20 09:28:42.000000 harmonic-1.2.1/harmonic/chains.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    20399 2023-11-20 09:28:42.000000 harmonic-1.2.1/harmonic/evidence.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    13918 2023-11-20 09:28:42.000000 harmonic-1.2.1/harmonic/flows.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     3175 2022-06-30 08:33:43.000000 harmonic-1.2.1/harmonic/logs.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    13014 2023-11-21 14:40:12.000000 harmonic-1.2.1/harmonic/model.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     2210 2023-11-20 09:28:42.000000 harmonic-1.2.1/harmonic/model_abstract.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)  1267641 2024-02-19 11:22:35.000000 harmonic-1.2.1/harmonic/model_legacy.c
--rw-r--r--   0 cosmomatt   (503) staff       (20)    56590 2023-11-20 09:28:42.000000 harmonic-1.2.1/harmonic/model_legacy.pyx
--rw-r--r--   0 cosmomatt   (503) staff       (20)    11283 2023-11-21 14:54:42.000000 harmonic-1.2.1/harmonic/utils.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-02-19 11:22:35.583320 harmonic-1.2.1/harmonic.egg-info/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     6023 2024-02-19 11:22:35.000000 harmonic-1.2.1/harmonic.egg-info/PKG-INFO
--rw-r--r--   0 cosmomatt   (503) staff       (20)      621 2024-02-19 11:22:35.000000 harmonic-1.2.1/harmonic.egg-info/SOURCES.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)        1 2024-02-19 11:22:35.000000 harmonic-1.2.1/harmonic.egg-info/dependency_links.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)      195 2024-02-19 11:22:35.000000 harmonic-1.2.1/harmonic.egg-info/requires.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)        9 2024-02-19 11:22:35.000000 harmonic-1.2.1/harmonic.egg-info/top_level.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)      125 2023-11-21 15:15:38.000000 harmonic-1.2.1/pyproject.toml
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-02-19 11:22:35.579504 harmonic-1.2.1/requirements/
--rw-r--r--   0 cosmomatt   (503) staff       (20)      207 2024-02-19 11:19:09.000000 harmonic-1.2.1/requirements/requirements-core.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)       38 2024-02-19 11:22:35.584936 harmonic-1.2.1/setup.cfg
--rw-r--r--   0 cosmomatt   (503) staff       (20)     2164 2024-02-19 11:19:34.000000 harmonic-1.2.1/setup.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-02-19 11:22:35.582703 harmonic-1.2.1/tests/
--rw-r--r--   0 cosmomatt   (503) staff       (20)    21450 2022-06-30 08:33:43.000000 harmonic-1.2.1/tests/test_chains.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    15927 2023-11-20 09:28:42.000000 harmonic-1.2.1/tests/test_evidence.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     7148 2023-11-21 14:40:12.000000 harmonic-1.2.1/tests/test_flow_model.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)      485 2022-06-30 08:33:43.000000 harmonic-1.2.1/tests/test_logs.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    27481 2023-11-20 09:28:42.000000 harmonic-1.2.1/tests/test_model.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     7953 2023-11-21 14:40:12.000000 harmonic-1.2.1/tests/test_utils.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-05-07 13:52:10.590793 harmonic-1.2.2/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4804 2024-05-01 09:34:59.000000 harmonic-1.2.2/.pip_readme.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    35149 2022-06-30 08:33:43.000000 harmonic-1.2.2/LICENSE.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      716 2022-06-30 08:33:43.000000 harmonic-1.2.2/LICENSE_EXT.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       89 2022-06-30 08:33:43.000000 harmonic-1.2.2/MANIFEST.in
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     6023 2024-05-07 13:52:10.590496 harmonic-1.2.2/PKG-INFO
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     7172 2024-05-01 16:00:14.000000 harmonic-1.2.2/README.rst
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-05-07 13:52:10.587037 harmonic-1.2.2/harmonic/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      178 2024-05-01 09:34:59.000000 harmonic-1.2.2/harmonic/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    15008 2024-05-01 09:34:59.000000 harmonic-1.2.2/harmonic/chains.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    20308 2024-05-07 12:49:53.000000 harmonic-1.2.2/harmonic/evidence.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    13918 2024-05-01 09:34:59.000000 harmonic-1.2.2/harmonic/flows.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     3175 2022-06-30 08:33:43.000000 harmonic-1.2.2/harmonic/logs.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    13014 2024-05-01 09:34:59.000000 harmonic-1.2.2/harmonic/model.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     2210 2024-05-01 09:34:59.000000 harmonic-1.2.2/harmonic/model_abstract.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)  1267641 2024-05-07 13:52:10.000000 harmonic-1.2.2/harmonic/model_legacy.c
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    56590 2024-05-01 09:34:59.000000 harmonic-1.2.2/harmonic/model_legacy.pyx
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    11249 2024-05-01 09:34:59.000000 harmonic-1.2.2/harmonic/utils.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-05-07 13:52:10.589985 harmonic-1.2.2/harmonic.egg-info/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     6023 2024-05-07 13:52:10.000000 harmonic-1.2.2/harmonic.egg-info/PKG-INFO
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      621 2024-05-07 13:52:10.000000 harmonic-1.2.2/harmonic.egg-info/SOURCES.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)        1 2024-05-07 13:52:10.000000 harmonic-1.2.2/harmonic.egg-info/dependency_links.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      195 2024-05-07 13:52:10.000000 harmonic-1.2.2/harmonic.egg-info/requires.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)        9 2024-05-07 13:52:10.000000 harmonic-1.2.2/harmonic.egg-info/top_level.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      125 2023-11-21 15:15:38.000000 harmonic-1.2.2/pyproject.toml
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-05-07 13:52:10.588185 harmonic-1.2.2/requirements/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      207 2024-05-01 09:34:59.000000 harmonic-1.2.2/requirements/requirements-core.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       38 2024-05-07 13:52:10.590840 harmonic-1.2.2/setup.cfg
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     2164 2024-05-07 13:49:00.000000 harmonic-1.2.2/setup.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-05-07 13:52:10.589760 harmonic-1.2.2/tests/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    21450 2022-06-30 08:33:43.000000 harmonic-1.2.2/tests/test_chains.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    15766 2024-05-07 12:49:53.000000 harmonic-1.2.2/tests/test_evidence.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     9060 2024-05-01 09:34:59.000000 harmonic-1.2.2/tests/test_flow_model.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      485 2022-06-30 08:33:43.000000 harmonic-1.2.2/tests/test_logs.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    27481 2024-05-01 09:34:59.000000 harmonic-1.2.2/tests/test_model.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     7953 2024-05-01 09:34:59.000000 harmonic-1.2.2/tests/test_utils.py
```

### Comparing `harmonic-1.2.1/.pip_readme.rst` & `harmonic-1.2.2/.pip_readme.rst`

 * *Files identical despite different names*

### Comparing `harmonic-1.2.1/LICENSE.txt` & `harmonic-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `harmonic-1.2.1/LICENSE_EXT.txt` & `harmonic-1.2.2/LICENSE_EXT.txt`

 * *Files identical despite different names*

### Comparing `harmonic-1.2.1/PKG-INFO` & `harmonic-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: harmonic
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python package for efficient Bayesian evidence computation
 Home-page: https://github.com/astro-informatics/harmonic
-Author: Jason D. McEwen, Christopher G. R. Wallis, Matthew A. Price, Matthew M. Docherty, Alicja Polanska & Contributors
+Author: Jason D. McEwen, Alicja Polanska, Christopher G. R. Wallis, Matthew A. Price, Matthew M. Docherty & Contributors
 Author-email: jason.mcewen@ucl.ac.uk
 License: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `harmonic-1.2.1/README.rst` & `harmonic-1.2.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,38 @@
-.. image:: https://img.shields.io/badge/GitHub-harmonic-brightgreen.svg?style=flat
+.. |github| image:: https://img.shields.io/badge/GitHub-harmonic-brightgreen.svg?style=flat
     :target: https://github.com/astro-informatics/harmonic
-.. image:: https://github.com/astro-informatics/harmonic/actions/workflows/python.yml/badge.svg
+.. |tests| image:: https://github.com/astro-informatics/harmonic/actions/workflows/python.yml/badge.svg
     :target: https://github.com/astro-informatics/harmonic/actions/workflows/python.yml
-.. image:: https://readthedocs.org/projects/ansicolortags/badge/?version=latest
+.. |docs| image:: https://readthedocs.org/projects/ansicolortags/badge/?version=latest
     :target: https://astro-informatics.github.io/harmonic/
-.. image:: https://codecov.io/gh/astro-informatics/harmonic/branch/main/graph/badge.svg?token=1s4SATphHV
+.. |codecov| image:: https://codecov.io/gh/astro-informatics/harmonic/branch/main/graph/badge.svg?token=1s4SATphHV
     :target: https://codecov.io/gh/astro-informatics/harmonic
-.. image:: https://badge.fury.io/py/harmonic.svg
+.. |pypi| image:: https://badge.fury.io/py/harmonic.svg
     :target: https://badge.fury.io/py/harmonic
-.. image:: https://img.shields.io/badge/License-GPL-blue.svg
+.. |licence| image:: https://img.shields.io/badge/License-GPL-blue.svg
     :target: http://perso.crans.org/besson/LICENSE.html
-.. image:: http://img.shields.io/badge/arXiv-2111.12720-orange.svg?style=flat
+.. |arxiv1| image:: http://img.shields.io/badge/arXiv-2111.12720-orange.svg?style=flat
     :target: https://arxiv.org/abs/2111.12720
-.. image:: http://img.shields.io/badge/arXiv-2207.04037-orange.svg?style=flat
+.. |arxiv2| image:: http://img.shields.io/badge/arXiv-2207.04037-orange.svg?style=flat
     :target: https://arxiv.org/abs/2207.04037
-.. image:: http://img.shields.io/badge/arXiv-2307.00048-orange.svg?style=flat
+.. |arxiv3| image:: http://img.shields.io/badge/arXiv-2307.00048-orange.svg?style=flat
     :target: https://arxiv.org/abs/2307.00048
 .. .. image:: https://img.shields.io/pypi/pyversions/harmonic.svg
 ..     :target: https://pypi.python.org/pypi/harmonic/
 
-|logo| Harmonic
-=================================================================================================================
+|github| |tests| |docs| |codecov| |pypi| |licence| |arxiv1| |arxiv2| |arxiv3|
+
 
-.. |logo| raw:: html
+.. |logo| image:: ./docs/assets/harm_badge_simple.svg
+    :width: 32
+    :height: 32
+    :align: center
 
-   <img src="./docs/assets/harm_badge_simple.svg" align="center" height="52" width="52">
+|logo| Harmonic
+=================================================================================================================
 
 ``harmonic`` is an open source, well tested and documented Python implementation of the *learnt harmonic mean estimator* (`McEwen et al. 2021 <https://arxiv.org/abs/2111.12720>`_) to compute the marginal likelihood (Bayesian evidence), required for Bayesian model selection.
 
 For an accessible overview of the *learnt harmonic mean estimator* please see this `Towards Data Science article <https://towardsdatascience.com/learnt-harmonic-mean-estimator-for-bayesian-model-selection-47258bb0fc2e>`_.
 
 While ``harmonic`` requires only posterior samples, and so is agnostic to the technique used to perform Markov chain Monte Carlo (MCMC) sampling, ``harmonic`` works exceptionally well with MCMC sampling techniques that naturally provide samples from multiple chains by their ensemble nature, such as affine invariant ensemble samplers.  We therefore advocate use of `harmonic` with the popular `emcee <https://github.com/dfm/emcee>`_ code implementing the affine invariant sampler of `Goodman & Weare (2010) <https://cims.nyu.edu/~weare/papers/d13.pdf>`_.
```

### Comparing `harmonic-1.2.1/harmonic/chains.py` & `harmonic-1.2.2/harmonic/chains.py`

 * *Files identical despite different names*

### Comparing `harmonic-1.2.1/harmonic/evidence.py` & `harmonic-1.2.2/harmonic/evidence.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,22 +65,20 @@
         self.running_sum = np.zeros(nchains)
         self.nsamples_per_chain = np.zeros(nchains)
         self.nsamples_eff_per_chain = np.zeros(nchains)
 
         # Chain parameters and realspace statistics
         self.nchains = nchains
         self.ndim = model.ndim
-        self.evidence_inv = 0.0
-        self.evidence_inv_var = 0.0
-        self.evidence_inv_var_var = 0.0
         self.kurtosis = 0.0
         self.n_eff = 0
 
         # For statistics computed purely in log-space.
         self.ln_evidence_inv = 0.0
+        self.ln_evidence_inv_per_chain = None
         self.ln_evidence_inv_var = 0.0
         self.ln_evidence_inv_var_var = 0.0
         self.ln_kurtosis = 0.0
 
         # Shift selection
         self.shift = shift
         self.shift_set = False
@@ -136,14 +134,18 @@
         nsamples_per_chain = self.nsamples_per_chain
 
         evidence_inv = jnp.sum(self.running_sum)
         nsamples = jnp.sum(self.nsamples_per_chain)
 
         evidence_inv /= nsamples
 
+        self.ln_evidence_inv_per_chain = (
+            jnp.log(self.running_sum) - self.shift_value - jnp.log(nsamples_per_chain)
+        )
+
         """
         The following code computes the exponents of the variance and variance 
         of the variance where possible in log space to avoid overflow errors.
 
         This is a log-space representation of the real-space statistics. One may
         alternatively compute the log-space statistics, but should note that 
         simply taking the exponential of log-space statistics is NOT the same as 
@@ -180,21 +182,14 @@
         self.ln_evidence_inv_var_var = (
             2.0 * evidence_inv_var_ln_temp
             - 3.0 * np.log(n_eff)
             - 4.0 * self.shift_value
             + np.log((kur - 1) + 2.0 / (n_eff - 1))
         )
 
-        # Compute inverse evidence statistics in real-space. In certain settings
-        # these values may return nan due to float overflow: in these cases one
-        # should use the log-space values.
-        self.evidence_inv = np.exp(self.ln_evidence_inv)
-        self.evidence_inv_var = np.exp(self.ln_evidence_inv_var)
-        self.evidence_inv_var_var = np.exp(self.ln_evidence_inv_var_var)
-
         return
 
     def get_masks(self, chain_start_ixs: jnp.ndarray) -> jnp.ndarray:
         """Create mask array for a 2D array of concatenated chains of different lengths.
         Args:
 
             chain_start_ixs (jnp.ndarray[nchains+1]): Start indices of chains
@@ -246,39 +241,41 @@
             raise ValueError("nchains do not match")
 
         if chains.ndim != self.ndim:
             raise ValueError("Chains ndim inconsistent")
 
         X = chains.samples
         Y = chains.ln_posterior
-        running_sum = self.running_sum
-        nsamples_per_chain = self.nsamples_per_chain
-        nsamples_eff_per_chain = self.nsamples_eff_per_chain
         nchains = self.nchains
 
         if self.batch_calculation:
             lnpred = self.model.predict(x=X)
             lnargs = lnpred - Y
             lnargs = lnargs.at[jnp.isinf(lnargs)].set(jnp.nan)
 
         else:
+            lnpred = np.zeros_like(Y)
             lnargs = np.zeros_like(Y)
             for i_chains in range(nchains):
                 i_samples_start = chains.start_indices[i_chains]
                 i_samples_end = chains.start_indices[i_chains + 1]
 
                 for i, i_samples in enumerate(range(i_samples_start, i_samples_end)):
                     lnpredict = self.model.predict(X[i_samples, :])
+                    lnpred[i_samples] = lnpredict
 
                     lnprob = Y[i_samples]
                     lnargs[i_samples] = lnpredict - lnprob
 
                     if np.isinf(lnargs[i_samples]):
                         lnargs[i_samples] = np.nan
 
+                    if np.isinf(lnpred[i_samples]):
+                        lnpred[i_samples] = np.nan
+
         # The following performs a shift in log-space to avoid overflow or float
         # rounding errors in realspace.
         if not self.shift_set:
             if self.shift == Shifting.MAX_SHIFT:
                 # Shifts by max of the log-posterior
                 self.set_shift(-np.nanmax(lnargs))
             if self.shift == Shifting.MEAN_SHIFT:
@@ -295,79 +292,38 @@
             running_sum = jnp.nansum(jnp.where(mask, jnp.exp(lnargs), 0.0))
             return running_sum
 
         def get_nans_per_chain(lnargs, mask):
             nans_num = jnp.sum(jnp.where(mask, jnp.isnan(lnargs), 0.0))
             return nans_num
 
-        if self.batch_calculation:
-            lnargs += self.shift_value
+        lnargs += self.shift_value
 
-            masks = self.get_masks(jnp.array(chains.start_indices))
+        masks = self.get_masks(jnp.array(chains.start_indices))
 
-            running_sum_val = jax.vmap(get_running_sum, in_axes=(None, 0))(
-                lnargs, masks
-            )
-            self.running_sum += running_sum_val
+        running_sum_val = jax.vmap(get_running_sum, in_axes=(None, 0))(lnargs, masks)
+        self.running_sum += running_sum_val
 
-            # Count added number of samples per chain
-            added_nsamples_per_chain = np.diff(jnp.array(chains.start_indices))
-            self.nsamples_per_chain += added_nsamples_per_chain
-
-            # Count number of NaN values per chain and subtract to get effective
-            # number of added samples per chain
-            nan_count_per_chain = jax.vmap(get_nans_per_chain, in_axes=(None, 0))(
-                lnargs, masks
-            )
-            self.nsamples_eff_per_chain += (
-                added_nsamples_per_chain - nan_count_per_chain
-            )
+        # Count added number of samples per chain
+        added_nsamples_per_chain = np.diff(jnp.array(chains.start_indices))
+        self.nsamples_per_chain += added_nsamples_per_chain
 
-        else:
-            for i_chains in range(nchains):
-                i_samples_start = chains.start_indices[i_chains]
-                i_samples_end = chains.start_indices[i_chains + 1]
+        # Count number of NaN values per chain and subtract to get effective
+        # number of added samples per chain
+        nan_count_per_chain = jax.vmap(get_nans_per_chain, in_axes=(None, 0))(
+            lnargs, masks
+        )
+        self.nsamples_eff_per_chain += added_nsamples_per_chain - nan_count_per_chain
 
-                for i, i_samples in enumerate(range(i_samples_start, i_samples_end)):
-                    # Apply shifting term to avoid overflow.
-                    lnarg = lnargs[i_samples] + self.shift_value
-                    # Store realspace or logspace sum depending on choice.
-                    term = np.exp(lnarg)
-                    nsamples_per_chain[i_chains] += 1
-
-                    if not np.isnan(lnargs[i_samples]):
-                        # Count number of samples used.
-                        nsamples_eff_per_chain[i_chains] += 1
-
-                        # Add contribution to running sum.
-                        running_sum[i_chains] += term
-
-                        # Log diagnostic terms.
-                        self.lnargmax = (
-                            lnarg if lnarg > self.lnargmax else self.lnargmax
-                        )
-                        self.lnargmin = (
-                            lnarg if lnarg < self.lnargmin else self.lnargmin
-                        )
-                        self.lnprobmax = (
-                            lnprob if lnprob > self.lnprobmax else self.lnprobmax
-                        )
-                        self.lnprobmin = (
-                            lnprob if lnprob < self.lnprobmin else self.lnprobmin
-                        )
-                        self.lnpredictmax = (
-                            lnpredict
-                            if lnpredict > self.lnpredictmax
-                            else self.lnpredictmax
-                        )
-                        self.lnpredictmin = (
-                            lnpredict
-                            if lnpredict < self.lnpredictmin
-                            else self.lnpredictmin
-                        )
+        self.lnargmax = jnp.nanmax(lnargs)
+        self.lnargmin = jnp.nanmin(lnargs)
+        self.lnprobmax = jnp.nanmax(Y)
+        self.lnprobmin = jnp.nanmin(Y)
+        self.lnpredictmax = jnp.nanmax(lnpred)
+        self.lnpredictmin = jnp.nanmin(lnpred)
 
         self.process_run()
         self.chains_added = True
         self.check_basic_diagnostic()
 
         return
 
@@ -384,15 +340,15 @@
         Raises:
 
             Warnings: Raised if the diagnostic tests fail.
 
         """
 
         NSAMPLES_EFF_WARNING_LEVEL = 30
-        LNARG_WARNING_LEVEL = 400.0
+        LNARG_WARNING_LEVEL = 1000.0
 
         tests_pass = True
 
         if np.mean(self.nsamples_eff_per_chain) <= NSAMPLES_EFF_WARNING_LEVEL:
             lg.warning_log(
                 "Evidence may not be accurate due to low "
                 + "number of effective samples (mean number of effective "
@@ -420,23 +376,36 @@
             (double, double): Tuple containing the following.
 
                 - evidence (double): Estimate of evidence.
 
                 - evidence_std (double): Estimate of standard deviation of
                   evidence.
 
+        Raises:
+
+            ValueError: if inverse evidence or its variance overflows.
         """
 
         self.check_basic_diagnostic()
 
-        common_factor = 1.0 + self.evidence_inv_var / (self.evidence_inv**2)
+        evidence_inv = np.exp(self.ln_evidence_inv)
+        evidence_inv_var = np.exp(self.ln_evidence_inv_var)
+
+        if np.isinf(np.nan_to_num(evidence_inv, nan=np.inf)) or np.isinf(
+            np.nan_to_num(evidence_inv_var, nan=np.inf)
+        ):
+            raise ValueError(
+                "Evidence is too large to represent in non-log space. Use log-space values instead."
+            )
+
+        common_factor = 1.0 + evidence_inv_var / (evidence_inv**2)
 
-        evidence = common_factor / self.evidence_inv
+        evidence = common_factor / evidence_inv
 
-        evidence_std = np.sqrt(self.evidence_inv_var) / (self.evidence_inv**2)
+        evidence_std = np.sqrt(evidence_inv_var) / (evidence_inv**2)
 
         return (evidence, evidence_std)
 
     def compute_ln_evidence(self):
         """Compute log_e of evidence from the inverse evidence.
 
         Returns:
@@ -552,32 +521,54 @@
 
     Raises:
 
         ValueError: Raised if model 1 does not have chains added.
 
         ValueError: Raised if model 2 does not have chains added.
 
+        ValueError: If inverse evidence or its variance for model 1 or model 2 too large
+            to store in non-log space.
+
     """
 
     if not ev1.chains_added:
         raise ValueError("Evidence for model 1 does not have chains added")
     if not ev2.chains_added:
         raise ValueError("Evidence for model 2 does not have chains added")
 
     ev1.check_basic_diagnostic()
     ev2.check_basic_diagnostic()
 
-    common_factor = 1.0 + ev1.evidence_inv_var / (ev1.evidence_inv**2)
+    evidence_inv_ev1 = np.exp(ev1.ln_evidence_inv)
+    evidence_inv_var_ev1 = np.exp(ev1.ln_evidence_inv_var)
+
+    evidence_inv_ev2 = np.exp(ev2.ln_evidence_inv)
+    evidence_inv_var_ev2 = np.exp(ev2.ln_evidence_inv_var)
 
-    bf12 = ev2.evidence_inv / ev1.evidence_inv * common_factor
+    if np.isinf(np.nan_to_num(evidence_inv_ev1, nan=np.inf)) or np.isinf(
+        np.nan_to_num(evidence_inv_var_ev1, nan=np.inf)
+    ):
+        raise ValueError(
+            "Evidence for model 1 is too large to represent in non-log space. Use log-space values instead."
+        )
+    if np.isinf(np.nan_to_num(evidence_inv_ev2, nan=np.inf)) or np.isinf(
+        np.nan_to_num(evidence_inv_var_ev2, nan=np.inf)
+    ):
+        raise ValueError(
+            "Evidence for model 2 is too large to represent in non-log space. Use log-space values instead."
+        )
+
+    common_factor = 1.0 + evidence_inv_var_ev1 / (evidence_inv_ev1**2)
+
+    bf12 = evidence_inv_ev2 / evidence_inv_ev1 * common_factor
 
     bf12_std = np.sqrt(
-        ev1.evidence_inv**2 * ev2.evidence_inv_var
-        + ev2.evidence_inv**2 * ev1.evidence_inv_var
-    ) / (ev1.evidence_inv**2)
+        evidence_inv_ev1**2 * evidence_inv_var_ev2
+        + evidence_inv_ev2**2 * evidence_inv_var_ev1
+    ) / (evidence_inv_ev1**2)
 
     return (bf12, bf12_std)
 
 
 def compute_ln_bayes_factor(ev1, ev2):
     """Computes log_e of Bayes factor of two models.
 
@@ -608,21 +599,36 @@
         raise ValueError("Evidence for model 1 does not have chains added")
     if not ev2.chains_added:
         raise ValueError("Evidence for model 2 does not have chains added")
 
     ev1.check_basic_diagnostic()
     ev2.check_basic_diagnostic()
 
-    common_factor = 1.0 + ev1.evidence_inv_var / (ev1.evidence_inv**2)
+    evidence_inv_ev1 = np.exp(ev1.ln_evidence_inv)
+    evidence_inv_var_ev1 = np.exp(ev1.ln_evidence_inv_var)
+
+    evidence_inv_ev2 = np.exp(ev2.ln_evidence_inv)
+    evidence_inv_var_ev2 = np.exp(ev2.ln_evidence_inv_var)
+
+    if np.isnan(evidence_inv_ev1) or np.isnan(evidence_inv_var_ev1):
+        raise ValueError(
+            "Evidence for model 1 is too large to represent in non-log space. Use log-space values instead."
+        )
+    if np.isnan(evidence_inv_ev2) or np.isnan(evidence_inv_var_ev2):
+        raise ValueError(
+            "Evidence for model 2 is too large to represent in non-log space. Use log-space values instead."
+        )
+
+    common_factor = 1.0 + evidence_inv_var_ev1 / (evidence_inv_ev1**2)
 
     ln_bf12 = (
-        np.log(ev2.evidence_inv) - np.log(ev1.evidence_inv) + np.log(common_factor)
+        np.log(evidence_inv_ev2) - np.log(evidence_inv_ev1) + np.log(common_factor)
     )
 
     factor = (
-        ev1.evidence_inv**2 * ev2.evidence_inv_var
-        + ev2.evidence_inv**2 * ev1.evidence_inv_var
+        evidence_inv_ev1**2 * evidence_inv_var_ev2
+        + evidence_inv_ev2**2 * evidence_inv_var_ev1
     )
 
-    ln_bf12_std = 0.5 * np.log(factor) - 2.0 * np.log(ev1.evidence_inv)
+    ln_bf12_std = 0.5 * np.log(factor) - 2.0 * np.log(evidence_inv_ev1)
 
     return (ln_bf12, ln_bf12_std)
```

### Comparing `harmonic-1.2.1/harmonic/flows.py` & `harmonic-1.2.2/harmonic/flows.py`

 * *Files identical despite different names*

### Comparing `harmonic-1.2.1/harmonic/logs.py` & `harmonic-1.2.2/harmonic/logs.py`

 * *Files identical despite different names*

### Comparing `harmonic-1.2.1/harmonic/model.py` & `harmonic-1.2.2/harmonic/model.py`

 * *Files identical despite different names*

### Comparing `harmonic-1.2.1/harmonic/model_abstract.py` & `harmonic-1.2.2/harmonic/model_abstract.py`

 * *Files identical despite different names*

### Comparing `harmonic-1.2.1/harmonic/model_legacy.c` & `harmonic-1.2.2/harmonic/model_legacy.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 /* Generated by Cython 0.29.30 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/core/include"
+            "/private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/core/include"
         ],
         "name": "harmonic.model_legacy",
         "sources": [
             "harmonic/model_legacy.pyx"
         ]
     },
     "module_name": "harmonic.model_legacy"
@@ -995,195 +995,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":689
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":690
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":691
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":692
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":696
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":697
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":698
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":699
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":703
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":704
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":713
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":714
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":715
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":717
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":718
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":719
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":721
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":722
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":724
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":725
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":726
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1211,42 +1211,42 @@
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_double____double____object____object____object____object____object___to_py;
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":728
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":729
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":730
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":732
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -18897,15 +18897,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_weights);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":734
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18916,30 +18916,30 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew1", __pyx_f[1], 734, 0, __PYX_ERR(1, 734, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_TraceLine(735,0,__PYX_ERR(1, 735, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18951,15 +18951,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":737
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18970,30 +18970,30 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew2", __pyx_f[1], 737, 0, __PYX_ERR(1, 737, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_TraceLine(738,0,__PYX_ERR(1, 738, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -19005,15 +19005,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":740
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -19024,30 +19024,30 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew3", __pyx_f[1], 740, 0, __PYX_ERR(1, 740, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_TraceLine(741,0,__PYX_ERR(1, 741, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -19059,15 +19059,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":743
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -19078,30 +19078,30 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew4", __pyx_f[1], 743, 0, __PYX_ERR(1, 743, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_TraceLine(744,0,__PYX_ERR(1, 744, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -19113,15 +19113,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":746
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19132,30 +19132,30 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew5", __pyx_f[1], 746, 0, __PYX_ERR(1, 746, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_TraceLine(747,0,__PYX_ERR(1, 747, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19167,15 +19167,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":749
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
@@ -19186,63 +19186,63 @@
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
   __Pyx_TraceCall("PyDataType_SHAPE", __pyx_f[1], 749, 0, __PYX_ERR(1, 749, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __Pyx_TraceLine(750,0,__PYX_ERR(1, 750, __pyx_L1_error))
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_TraceLine(751,0,__PYX_ERR(1, 751, __pyx_L1_error))
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_TraceLine(753,0,__PYX_ERR(1, 753, __pyx_L1_error))
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
@@ -19253,15 +19253,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":928
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -19270,35 +19270,35 @@
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
   __Pyx_TraceCall("set_array_base", __pyx_f[1], 928, 0, __PYX_ERR(1, 928, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   __Pyx_TraceLine(929,0,__PYX_ERR(1, 929, __pyx_L1_error))
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __Pyx_TraceLine(930,0,__PYX_ERR(1, 930, __pyx_L1_error))
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -19307,15 +19307,15 @@
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":932
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
@@ -19327,70 +19327,70 @@
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_array_base", 0);
   __Pyx_TraceCall("get_array_base", __pyx_f[1], 932, 0, __PYX_ERR(1, 932, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __Pyx_TraceLine(933,0,__PYX_ERR(1, 933, __pyx_L1_error))
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __Pyx_TraceLine(934,0,__PYX_ERR(1, 934, __pyx_L1_error))
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_TraceLine(935,0,__PYX_ERR(1, 935, __pyx_L1_error))
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_TraceLine(936,0,__PYX_ERR(1, 936, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
@@ -19401,15 +19401,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":940
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19427,15 +19427,15 @@
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
   __Pyx_TraceCall("import_array", __pyx_f[1], 940, 0, __PYX_ERR(1, 940, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   __Pyx_TraceLine(941,0,__PYX_ERR(1, 941, __pyx_L1_error))
@@ -19444,39 +19444,39 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __Pyx_TraceLine(942,0,__PYX_ERR(1, 942, __pyx_L3_error))
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __Pyx_TraceLine(943,0,__PYX_ERR(1, 943, __pyx_L5_except_error))
@@ -19484,15 +19484,15 @@
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __Pyx_TraceLine(944,0,__PYX_ERR(1, 944, __pyx_L5_except_error))
@@ -19501,30 +19501,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19540,15 +19540,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":946
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19566,15 +19566,15 @@
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
   __Pyx_TraceCall("import_umath", __pyx_f[1], 946, 0, __PYX_ERR(1, 946, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   __Pyx_TraceLine(947,0,__PYX_ERR(1, 947, __pyx_L1_error))
@@ -19583,39 +19583,39 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __Pyx_TraceLine(948,0,__PYX_ERR(1, 948, __pyx_L3_error))
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __Pyx_TraceLine(949,0,__PYX_ERR(1, 949, __pyx_L5_except_error))
@@ -19623,15 +19623,15 @@
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __Pyx_TraceLine(950,0,__PYX_ERR(1, 950, __pyx_L5_except_error))
@@ -19640,30 +19640,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19679,15 +19679,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":952
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19705,15 +19705,15 @@
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
   __Pyx_TraceCall("import_ufunc", __pyx_f[1], 952, 0, __PYX_ERR(1, 952, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   __Pyx_TraceLine(953,0,__PYX_ERR(1, 953, __pyx_L1_error))
@@ -19722,39 +19722,39 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __Pyx_TraceLine(954,0,__PYX_ERR(1, 954, __pyx_L3_error))
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __Pyx_TraceLine(955,0,__PYX_ERR(1, 955, __pyx_L5_except_error))
@@ -19762,15 +19762,15 @@
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __Pyx_TraceLine(956,0,__PYX_ERR(1, 956, __pyx_L5_except_error))
@@ -19779,30 +19779,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19818,15 +19818,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":966
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
@@ -19836,26 +19836,26 @@
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
   __Pyx_TraceCall("is_timedelta64_object", __pyx_f[1], 966, 0, __PYX_ERR(1, 966, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_TraceLine(978,0,__PYX_ERR(1, 978, __pyx_L1_error))
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
@@ -19865,15 +19865,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":981
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
@@ -19883,26 +19883,26 @@
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
   __Pyx_TraceCall("is_datetime64_object", __pyx_f[1], 981, 0, __PYX_ERR(1, 981, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_TraceLine(993,0,__PYX_ERR(1, 993, __pyx_L1_error))
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
@@ -19912,15 +19912,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":996
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
@@ -19928,26 +19928,26 @@
   npy_datetime __pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceCall("get_datetime64_value", __pyx_f[1], 996, 1, __PYX_ERR(1, 996, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_TraceLine(1003,1,__PYX_ERR(1, 1003, __pyx_L1_error))
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
@@ -19956,15 +19956,15 @@
   __Pyx_WriteUnraisable("numpy.get_datetime64_value", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
@@ -19972,26 +19972,26 @@
   npy_timedelta __pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceCall("get_timedelta64_value", __pyx_f[1], 1006, 1, __PYX_ERR(1, 1006, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_TraceLine(1010,1,__PYX_ERR(1, 1010, __pyx_L1_error))
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
@@ -20000,15 +20000,15 @@
   __Pyx_WriteUnraisable("numpy.get_timedelta64_value", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -20016,24 +20016,24 @@
   NPY_DATETIMEUNIT __pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceCall("get_datetime64_unit", __pyx_f[1], 1013, 1, __PYX_ERR(1, 1013, __pyx_L1_error));
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __Pyx_TraceLine(1017,1,__PYX_ERR(1, 1017, __pyx_L1_error))
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -21031,26 +21031,26 @@
  *                         "inv_covariance contains a number that is not positive")
  * 
  */
   __pyx_tuple__52 = PyTuple_Pack(1, __pyx_kp_s_inv_covariance_contains_a_number_2); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(0, 1462, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__52);
   __Pyx_GIVEREF(__pyx_tuple__52);
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__55 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__55)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__55);
   __Pyx_GIVEREF(__pyx_tuple__55);
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__56 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__56)) __PYX_ERR(1, 950, __pyx_L1_error)
@@ -22471,165 +22471,165 @@
  */
   __Pyx_TraceLine(1,0,__PYX_ERR(0, 1, __pyx_L1_error))
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
   __Pyx_TraceLine(734,0,__PYX_ERR(1, 734, __pyx_L1_error))
 
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
   __Pyx_TraceLine(737,0,__PYX_ERR(1, 737, __pyx_L1_error))
 
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
   __Pyx_TraceLine(740,0,__PYX_ERR(1, 740, __pyx_L1_error))
 
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
   __Pyx_TraceLine(743,0,__PYX_ERR(1, 743, __pyx_L1_error))
 
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
   __Pyx_TraceLine(746,0,__PYX_ERR(1, 746, __pyx_L1_error))
 
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
   __Pyx_TraceLine(749,0,__PYX_ERR(1, 749, __pyx_L1_error))
 
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
   __Pyx_TraceLine(928,0,__PYX_ERR(1, 928, __pyx_L1_error))
 
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
   __Pyx_TraceLine(932,0,__PYX_ERR(1, 932, __pyx_L1_error))
 
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
   __Pyx_TraceLine(940,0,__PYX_ERR(1, 940, __pyx_L1_error))
 
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
   __Pyx_TraceLine(946,0,__PYX_ERR(1, 946, __pyx_L1_error))
 
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
   __Pyx_TraceLine(952,0,__PYX_ERR(1, 952, __pyx_L1_error))
 
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
   __Pyx_TraceLine(966,0,__PYX_ERR(1, 966, __pyx_L1_error))
 
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
   __Pyx_TraceLine(981,0,__PYX_ERR(1, 981, __pyx_L1_error))
 
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
   __Pyx_TraceLine(996,0,__PYX_ERR(1, 996, __pyx_L1_error))
 
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
   __Pyx_TraceLine(1006,0,__PYX_ERR(1, 1006, __pyx_L1_error))
 
 
-  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-20_0wu_7/lib/python3.9/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../private/var/folders/qc/147mc2mx0ns_fm7mww1l4t_40000gq/T/build-env-ei9yjv89/lib/python3.9/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
   __Pyx_TraceLine(1013,0,__PYX_ERR(1, 1013, __pyx_L1_error))
```

### Comparing `harmonic-1.2.1/harmonic/model_legacy.pyx` & `harmonic-1.2.2/harmonic/model_legacy.pyx`

 * *Files identical despite different names*

### Comparing `harmonic-1.2.1/harmonic/utils.py` & `harmonic-1.2.2/harmonic/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Tuple, List
 import numpy as np
 import harmonic as hm
 import getdist
+from harmonic import model_legacy
 from getdist import plots
 import matplotlib as plt
 
 
 def eval_func_on_grid(func, xmin, xmax, ymin, ymax, nx, ny):
     """
     Evalute 2D function on a grid.
@@ -258,15 +259,15 @@
 
 
 def cross_validation(
     chains,
     domains: List,
     hyper_parameters: List,
     nfold=2,
-    modelClass=None,
+    modelClass=model_legacy.KernelDensityEstimate,
     seed: int = -1,
 ) -> List:
     """Perform n-fold validation for given model using chains to be split into
     validation and training data.
 
     First, splits data into nfold chunks. Second, fits the model using each of
     the hyper-parameters given using all but one of the chunks (the validation
@@ -280,35 +281,32 @@
             training and validation data herein).
 
         domains (List): Domains of the model's parameters.
 
         hyper_parameters (List): List of hyper_parameters where each entry is a
             hyper_parameter list to be considered.
 
-        modelClass (Model): Model that is being cross validated (default = None).
+        modelClass (Model): Model that is being cross validated (default =
+            KernelDensityEstimate).
 
         seed (int): Seed for random number generator when drawing the chains
             (if this is negative the seed is not set).
 
     Returns:
 
         (List): Mean log validation variance (averaged over nfolds) for each hyper-parameter.
 
     Raises:
 
         ValueError: Raised if model is not one of the posible models.
-        ValueError: Raised if no model is provided.
 
     """
 
     ln_validation_variances = np.zeros((nfold, len(hyper_parameters)))
 
-    if modelClass == None:
-        raise ValueError("No model provided!")
-
     if seed > 0:
         np.random.seed(seed)
 
     indexes = list(np.random.permutation(chains.nchains))
 
     nchains_in_val_set = int(chains.nchains / nfold)
```

### Comparing `harmonic-1.2.1/harmonic.egg-info/PKG-INFO` & `harmonic-1.2.2/harmonic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: harmonic
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python package for efficient Bayesian evidence computation
 Home-page: https://github.com/astro-informatics/harmonic
-Author: Jason D. McEwen, Christopher G. R. Wallis, Matthew A. Price, Matthew M. Docherty, Alicja Polanska & Contributors
+Author: Jason D. McEwen, Alicja Polanska, Christopher G. R. Wallis, Matthew A. Price, Matthew M. Docherty & Contributors
 Author-email: jason.mcewen@ucl.ac.uk
 License: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `harmonic-1.2.1/harmonic.egg-info/SOURCES.txt` & `harmonic-1.2.2/harmonic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `harmonic-1.2.1/setup.py` & `harmonic-1.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,18 +44,18 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
     ],
     name="harmonic",
-    version="1.2.1",
+    version="1.2.2",
     prefix=".",
     url="https://github.com/astro-informatics/harmonic",
-    author="Jason D. McEwen, Christopher G. R. Wallis, Matthew A. Price, Matthew M. Docherty, Alicja Polanska & Contributors",
+    author="Jason D. McEwen, Alicja Polanska, Christopher G. R. Wallis, Matthew A. Price, Matthew M. Docherty & Contributors",
     author_email="jason.mcewen@ucl.ac.uk",
     license="GNU General Public License v3 (GPLv3)",
     install_requires=required,
     description="Python package for efficient Bayesian evidence computation",
     long_description_content_type="text/x-rst",
     long_description=long_description,
     packages=["harmonic"],
```

### Comparing `harmonic-1.2.1/tests/test_chains.py` & `harmonic-1.2.2/tests/test_chains.py`

 * *Files identical despite different names*

### Comparing `harmonic-1.2.1/tests/test_evidence.py` & `harmonic-1.2.2/tests/test_evidence.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,17 +28,17 @@
     model.fitted = True
     with pytest.raises(ValueError):
         rho = cbe.Evidence(nchains=0, model=model)
 
     rho = cbe.Evidence(nchains, model)
 
     assert rho.nchains == nchains
-    assert rho.evidence_inv == pytest.approx(0.0)
-    assert rho.evidence_inv_var == pytest.approx(0.0)
-    assert rho.evidence_inv_var_var == pytest.approx(0.0)
+    assert rho.ln_evidence_inv == pytest.approx(0.0)
+    assert rho.ln_evidence_inv_var == pytest.approx(0.0)
+    assert rho.ln_evidence_inv_var_var == pytest.approx(0.0)
     assert rho.running_sum.size == nchains
     assert rho.nsamples_per_chain.size == nchains
     assert rho.shift_value == pytest.approx(0.0)
     assert rho.shift_set == False
     for i_chain in range(nchains):
         assert rho.running_sum[i_chain] == pytest.approx(0.0)
         assert rho.nsamples_per_chain[i_chain] == 0
@@ -78,17 +78,17 @@
     evidence_inv_var_var = (
         evidence_inv_var**2
         * (kurtosis(np.sum(samples, axis=1) / n_samples) + 2 + 2.0 / (nchains - 1))
         * (nchains - 1) ** 2
         / nchains**3
     )
 
-    assert rho.evidence_inv == pytest.approx(evidence_inv, abs=1e-7)
-    assert rho.evidence_inv_var == pytest.approx(evidence_inv_var)
-    assert rho.evidence_inv_var_var == pytest.approx(evidence_inv_var_var)
+    assert np.exp(rho.ln_evidence_inv) == pytest.approx(evidence_inv, abs=1e-7)
+    assert np.exp(rho.ln_evidence_inv_var) == pytest.approx(evidence_inv_var)
+    assert np.exp(rho.ln_evidence_inv_var_var) == pytest.approx(evidence_inv_var_var)
 
     rho = cbe.Evidence(nchains, model, cbe.Shifting.MEAN_SHIFT)
     np.random.seed(1)
     post = np.random.uniform(high=1e3, size=(nchains, n_samples))
     samples = 1.0 / post
     mean_shift = np.mean(np.log(post))
     samples_scaled = samples * np.exp(mean_shift)
@@ -102,17 +102,17 @@
     evidence_inv_var_var = (
         evidence_inv_var**2
         * (kurtosis(np.sum(samples, axis=1) / n_samples) + 2 + 2.0 / (nchains - 1))
         * (nchains - 1) ** 2
         / nchains**3
     )
 
-    assert rho.evidence_inv == pytest.approx(evidence_inv, abs=1e-7)
-    assert rho.evidence_inv_var == pytest.approx(evidence_inv_var)
-    assert rho.evidence_inv_var_var == pytest.approx(evidence_inv_var_var)
+    assert np.exp(rho.ln_evidence_inv) == pytest.approx(evidence_inv, abs=1e-7)
+    assert np.exp(rho.ln_evidence_inv_var) == pytest.approx(evidence_inv_var)
+    assert np.exp(rho.ln_evidence_inv_var_var) == pytest.approx(evidence_inv_var_var)
 
 
 def test_add_chains():
     nchains = 200
     nsamples = 500
     ndim = 2
 
@@ -130,36 +130,36 @@
     sphere = mdl.HyperSphere(ndim, domain)
     sphere.fit(chain.samples, chain.ln_posterior)
 
     # Calculate evidence
     cal_ev = cbe.Evidence(nchains, sphere, cbe.Shifting.MEAN_SHIFT)
     cal_ev.add_chains(chain)
 
-    print("cal_ev.evidence_inv = {}".format(cal_ev.evidence_inv))
+    print("cal_ev.evidence_inv = {}".format(np.exp(cal_ev.ln_evidence_inv)))
 
-    assert cal_ev.evidence_inv == pytest.approx(0.159438606)
-    assert cal_ev.evidence_inv_var == pytest.approx(1.164628268e-07)
-    assert cal_ev.evidence_inv_var_var**0.5 == pytest.approx(1.142786462e-08)
+    assert np.exp(cal_ev.ln_evidence_inv) == pytest.approx(0.159438606)
+    assert np.exp(cal_ev.ln_evidence_inv_var) == pytest.approx(1.164628268e-07)
+    assert np.exp(cal_ev.ln_evidence_inv_var_var)**0.5 == pytest.approx(1.142786462e-08)
 
     nsamples1 = 300
     chains1 = ch.Chains(ndim)
     for i_chain in range(nchains):
         chains1.add_chain(X[i_chain, :nsamples1, :], Y[i_chain, :nsamples1])
     chains2 = ch.Chains(ndim)
     for i_chain in range(nchains):
         chains2.add_chain(X[i_chain, nsamples1:, :], Y[i_chain, nsamples1:])
 
     ev = cbe.Evidence(nchains, sphere, cbe.Shifting.MEAN_SHIFT)
     # Might have small numerical differences if don't use same mean_shift.
     ev.add_chains(chains1)
     ev.add_chains(chains2)
 
-    assert ev.evidence_inv == pytest.approx(0.159438606)
-    assert ev.evidence_inv_var == pytest.approx(1.164628268e-07)
-    assert ev.evidence_inv_var_var**0.5 == pytest.approx(1.142786462e-08)
+    assert np.exp(ev.ln_evidence_inv) == pytest.approx(0.159438606)
+    assert np.exp(ev.ln_evidence_inv_var) == pytest.approx(1.164628268e-07)
+    assert np.exp(ev.ln_evidence_inv_var_var)**0.5 == pytest.approx(1.142786462e-08)
 
     return
 
 
 def test_shifting_settings():
     nchains = 200
     nsamples = 500
@@ -219,16 +219,14 @@
     nchains = 100
 
     model.fitted = True
 
     ev_inv = 1e10
     ev_inv_var = 2e10
     ev = cbe.Evidence(nchains, model)
-    ev.evidence_inv = ev_inv
-    ev.evidence_inv_var = ev_inv_var
     ev.ln_evidence_inv = np.log(ev_inv)
     ev.ln_evidence_inv_var = np.log(ev_inv_var)
 
     (evidence, evidence_std) = ev.compute_evidence()
     assert evidence == pytest.approx((1 + ev_inv_var / ev_inv**2) / ev_inv)
     assert evidence_std**2 == pytest.approx(ev_inv_var / ev_inv**4)
 
@@ -244,29 +242,25 @@
     model.fitted = True
 
     # Check boundary case where ratio 1.0
     # (ln_ev_inv_var = 2 * ln_ev_inv)
     ln_ev_inv = 10
     ln_ev_inv_var = 2 * ln_ev_inv
     ev = cbe.Evidence(nchains, model)
-    ev.evidence_inv = np.exp(ln_ev_inv)
-    ev.evidence_inv_var = np.exp(ln_ev_inv_var)
     ev.ln_evidence_inv = ln_ev_inv
     ev.ln_evidence_inv_var = ln_ev_inv_var
 
     zeta_neg, zeta_pos = ev.compute_ln_inv_evidence_errors()
     assert zeta_neg == np.NINF
     assert zeta_pos == pytest.approx(np.log(2.0))
 
     # Check case where ln_ev_inv_var = ln_ev_inv
     ln_ev_inv = 10
     ln_ev_inv_var = ln_ev_inv
     ev = cbe.Evidence(nchains, model)
-    ev.evidence_inv = np.exp(ln_ev_inv)
-    ev.evidence_inv_var = np.exp(ln_ev_inv_var)
     ev.ln_evidence_inv = ln_ev_inv
     ev.ln_evidence_inv_var = ln_ev_inv_var
 
     zeta_neg, zeta_pos = ev.compute_ln_inv_evidence_errors()
     assert zeta_neg == pytest.approx(
         np.log(1.0 - np.exp(0.5 * ln_ev_inv_var - ln_ev_inv))
     )
@@ -274,16 +268,14 @@
         np.log(1.0 + np.exp(0.5 * ln_ev_inv_var - ln_ev_inv))
     )
 
     # Check case where ln_ev_inv_var = 0.5 * ln_ev_inv
     ln_ev_inv = 10
     ln_ev_inv_var = 0.5 * ln_ev_inv
     ev = cbe.Evidence(nchains, model)
-    ev.evidence_inv = np.exp(ln_ev_inv)
-    ev.evidence_inv_var = np.exp(ln_ev_inv_var)
     ev.ln_evidence_inv = ln_ev_inv
     ev.ln_evidence_inv_var = ln_ev_inv_var
 
     zeta_neg, zeta_pos = ev.compute_ln_inv_evidence_errors()
     assert zeta_neg == pytest.approx(
         np.log(1.0 - np.exp(0.5 * ln_ev_inv_var - ln_ev_inv))
     )
@@ -299,26 +291,26 @@
     domain = [np.array([1e-1, 1e1])]
     sphere = mdl.HyperSphere(ndim, domain)
     sphere.fitted = True
 
     ev1_inv = 1e10
     ev1_inv_var = 2e10
     ev1 = cbe.Evidence(nchains, sphere)
-    ev1.evidence_inv = ev1_inv
-    ev1.evidence_inv_var = ev1_inv_var
+    ev1.ln_evidence_inv = np.log(ev1_inv)
+    ev1.ln_evidence_inv_var = np.log(ev1_inv_var)
     ev1.chains_added = True
 
     ndim = 4
     nchains = 600
 
     ev2_inv = 3e10
     ev2_inv_var = 4e10
     ev2 = cbe.Evidence(nchains, sphere)
-    ev2.evidence_inv = ev2_inv
-    ev2.evidence_inv_var = ev2_inv_var
+    ev2.ln_evidence_inv = np.log(ev2_inv)
+    ev2.ln_evidence_inv_var = np.log(ev2_inv_var)
     ev2.chains_added = True
 
     bf12_check = ev2_inv / ev1_inv * (1.0 + ev2_inv_var / ev2_inv**2)
     bf12_var_check = (
         ev1_inv**2 * ev2_inv_var + ev2_inv**2 * ev1_inv_var
     ) / ev1_inv**4
 
@@ -329,27 +321,24 @@
 
     (ln_bf12, ln_bf12_std) = cbe.compute_ln_bayes_factor(ev1, ev2)
 
     assert bf12 == pytest.approx(np.exp(ln_bf12))
     assert bf12_std == pytest.approx(np.exp(ln_bf12_std))
 
     # Test bayes factor reduces to single evidence calculation.
-    ev2_inv = 1.0
-    ev2_inv_var = 0.0
     ev2 = cbe.Evidence(nchains, sphere)
-    ev2.evidence_inv = ev2_inv
-    ev2.evidence_inv_var = ev2_inv_var
+    ev2.ln_evidence_inv = 0
+    ev2.ln_evidence_inv_var = -np.inf
     ev2.chains_added = True
     (bf12, bf12_std) = cbe.compute_bayes_factor(ev1, ev2)
 
     (evidence, evidence_std) = ev1.compute_evidence()
     assert bf12 == pytest.approx(evidence)
     assert bf12_std == pytest.approx(evidence_std)
 
-
 @pytest.mark.parametrize("model", models_to_test_2)
 def test_serialization(model):
     nchains = 200
     nsamples = 500
     ndim = model.ndim
 
     # Create samples of unnormalised Gaussian
@@ -375,17 +364,17 @@
     ev1.serialize(".test.dat")
 
     # Deserialize evidence
     ev2 = cbe.Evidence.deserialize(".test.dat")
 
     # Test evidence objects the same
     assert ev1.nchains == ev2.nchains
-    assert ev1.evidence_inv == ev2.evidence_inv
-    assert ev1.evidence_inv_var == ev2.evidence_inv_var
-    assert ev1.evidence_inv_var_var == ev2.evidence_inv_var_var
+    assert ev1.ln_evidence_inv == ev2.ln_evidence_inv
+    assert ev1.ln_evidence_inv_var == ev2.ln_evidence_inv_var
+    assert ev1.ln_evidence_inv_var_var == ev2.ln_evidence_inv_var_var
     assert ev1.running_sum.size == ev2.running_sum.size
     assert ev1.nsamples_per_chain.size == ev2.nsamples_per_chain.size
     assert ev1.shift_value == ev2.shift_value
     assert ev1.shift_set == ev2.shift_set
     for i_chain in range(nchains):
         assert ev1.running_sum[i_chain] == ev2.running_sum[i_chain]
         assert ev1.nsamples_per_chain[i_chain] == ev2.nsamples_per_chain[i_chain]
```

### Comparing `harmonic-1.2.1/tests/test_flow_model.py` & `harmonic-1.2.2/tests/test_flow_model.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import pytest
 import harmonic.model as md
 import jax.numpy as jnp
 import jax
 import harmonic as hm
 
 real_nvp_2D = md.RealNVPModel(2, standardize=True)
-spline_4D = md.RQSplineModel(4, standardize=True)
+spline_4D = md.RQSplineModel(4, n_layers=2, n_bins=64, standardize=True)
+spline_3D = md.RQSplineModel(3, n_layers=2, n_bins=64, standardize=False)
 
 model_classes = [md.RealNVPModel, md.RQSplineModel]
 
 models_to_test = [real_nvp_2D, spline_4D]
+models_to_test1 = [real_nvp_2D, spline_4D, spline_3D]
+gaussian_var = [0.1, 0.5, 1.0, 10.0, 20.0]
 
 # Make models for serialization tests
 # NVP params
 ndim = 2
 n_scaled = 13
 n_unscaled = 6
 
@@ -50,32 +53,33 @@
     momentum=momentum,
     temperature=temperature,
 )
 
 models_serialization = [real_NVP_serialization, spline_serialization]
 
 
-def standard_nd_gaussian_pdf(x):
+def standard_nd_gaussian_pdf(x, var=1.0):
     """
     Calculate the probability density function (PDF) of an n-dimensional Gaussian
-    distribution with zero mean and unit covariance.
+    distribution with zero mean and diagonal covariance with entries var.
 
     Parameters:
     - x: Input vector of length n.
+    - var: Gaussian variance
 
     Returns:
     - pdf: log PDF value at input vector x.
     """
     n = len(x)
 
     # The normalizing constant (coefficient)
-    C = -jnp.log(2 * jnp.pi) * n / 2
+    C = -jnp.log(2 * jnp.pi * var) * n / 2
 
     # Calculate the Mahalanobis distance
-    mahalanobis_dist = jnp.dot(x, x)
+    mahalanobis_dist = jnp.dot(x, x) / var
 
     # Calculate the PDF value
     pdf = C - 0.5 * mahalanobis_dist
 
     return pdf
 
 
@@ -144,14 +148,68 @@
     ndim = model.ndim
     assert model.is_fitted() == False
     training_samples = jnp.zeros((12, ndim))
     model.fit(training_samples, verbose=True, epochs=5)
     assert model.is_fitted() == True
 
 
+@pytest.mark.parametrize("model", models_to_test1)
+@pytest.mark.parametrize("var", gaussian_var)
+def test_flows_normalization(model, var):
+    # Define the number of dimensions and the mean of the Gaussian
+    ndim = model.ndim
+    num_samples = 10000
+
+    if isinstance(model, md.RealNVPModel):
+        epochs = 100
+    elif isinstance(model, md.RQSplineModel):
+        epochs = 30
+
+    # Initialize a PRNG key (you can use any valid key)
+    key = jax.random.PRNGKey(0)
+    mean = jnp.zeros(ndim)
+    cov = jnp.eye(ndim) * var
+
+    # Generate random samples from the Gaussian distribution
+    samples = jax.random.multivariate_normal(key, mean, cov, shape=(num_samples,))
+
+    model.fit(samples, epochs=epochs, verbose=True)
+    model.temperature = 1.0
+
+    # MC integral of the flow
+    num_samples_int = 50000
+    shape = (num_samples_int, ndim)
+    # Draw samples from uniform distribution -3 to 3 standard deviations away from mean
+    minval = -3 * var**0.5
+    maxval = 3 * var**0.5
+    uniform_samples = jax.random.uniform(
+        jax.random.PRNGKey(0), shape=shape, minval=minval, maxval=maxval
+    )
+    V = (maxval - minval) ** ndim
+    vals = jnp.exp(model.predict(uniform_samples))
+    integral = jnp.mean(vals) * V
+    assert integral == pytest.approx(1.0, rel=0.1), (
+        "Flow normalization constant is " + str(integral) + "not 1"
+    )
+
+    model.temperature = 0.5
+    vals = jnp.exp(model.predict(uniform_samples))
+    integral = jnp.mean(vals) * V
+    assert integral == pytest.approx(1.0, rel=0.1), (
+        "Flow with T=0.5 normalization constant is " + str(integral) + " not 1"
+    )
+
+    model.temperature = 0.1
+    vals = jnp.exp(model.predict(uniform_samples))
+    integral = jnp.mean(vals) * V
+    assert integral == pytest.approx(1.0, rel=0.1), (
+        "Flow with T=0.1 normalization constant is " + str(integral) + "not 1"
+    )
+
+
 @pytest.mark.parametrize("model", models_to_test)
 def test_flows_gaussian(model):
     # Define the number of dimensions and the mean of the Gaussian
     ndim = model.ndim
     num_samples = 10000
 
     if isinstance(model, md.RealNVPModel):
@@ -171,19 +229,14 @@
 
     nsamples = 5000
     model.temperature = 1.0
     flow_samples = model.sample(nsamples)
     sample_var = jnp.var(flow_samples, axis=0)
     sample_mean = jnp.mean(flow_samples, axis=0)
 
-    test = jnp.ones(ndim) * 0.2
-    assert jnp.exp(model.predict(test)) == pytest.approx(
-        jnp.exp(standard_nd_gaussian_pdf(test)), rel=0.1
-    ), "Flow probability density not in agreement with analytical value"
-
     for i in range(ndim):
         assert sample_mean[i] == pytest.approx(0.0, abs=0.15), (
             "Sample mean in dimension " + str(i) + " is " + str(sample_mean[i])
         )
         assert sample_var[i] == pytest.approx(1.0, abs=0.15), (
             "Sample variance in dimension " + str(i) + " is " + str(sample_var[i])
         )
```

### Comparing `harmonic-1.2.1/tests/test_model.py` & `harmonic-1.2.2/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `harmonic-1.2.1/tests/test_utils.py` & `harmonic-1.2.2/tests/test_utils.py`

 * *Files identical despite different names*

