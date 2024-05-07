# Comparing `tmp/likefit-0.2.0.tar.gz` & `tmp/likefit-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "likefit-0.2.0.tar", last modified: Wed Jan 31 21:53:45 2024, max compression
+gzip compressed data, was "likefit-0.2.1.tar", last modified: Tue May  7 20:39:24 2024, max compression
```

## Comparing `likefit-0.2.0.tar` & `likefit-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 dravignani  (1000) dravignani  (1000)        0 2024-01-31 21:53:45.515863 likefit-0.2.0/
--rw-rw-r--   0 dravignani  (1000) dravignani  (1000)     1081 2024-01-04 20:52:55.000000 likefit-0.2.0/LICENSE
--rw-r--r--   0 dravignani  (1000) dravignani  (1000)     2908 2024-01-31 21:53:45.515863 likefit-0.2.0/PKG-INFO
--rw-rw-r--   0 dravignani  (1000) dravignani  (1000)      957 2024-01-31 21:49:45.000000 likefit-0.2.0/README.md
-drwxrwxr-x   0 dravignani  (1000) dravignani  (1000)        0 2024-01-31 21:53:45.515863 likefit-0.2.0/likefit.egg-info/
--rw-r--r--   0 dravignani  (1000) dravignani  (1000)     2908 2024-01-31 21:53:45.000000 likefit-0.2.0/likefit.egg-info/PKG-INFO
--rw-rw-r--   0 dravignani  (1000) dravignani  (1000)      301 2024-01-31 21:53:45.000000 likefit-0.2.0/likefit.egg-info/SOURCES.txt
--rw-rw-r--   0 dravignani  (1000) dravignani  (1000)        1 2024-01-31 21:53:45.000000 likefit-0.2.0/likefit.egg-info/dependency_links.txt
--rw-rw-r--   0 dravignani  (1000) dravignani  (1000)       62 2024-01-31 21:53:45.000000 likefit-0.2.0/likefit.egg-info/requires.txt
--rw-rw-r--   0 dravignani  (1000) dravignani  (1000)        8 2024-01-31 21:53:45.000000 likefit-0.2.0/likefit.egg-info/top_level.txt
--rw-rw-r--   0 dravignani  (1000) dravignani  (1000)    33349 2024-01-31 13:00:27.000000 likefit-0.2.0/likefit.py
--rw-rw-r--   0 dravignani  (1000) dravignani  (1000)      788 2024-01-30 15:19:17.000000 likefit-0.2.0/pyproject.toml
--rw-rw-r--   0 dravignani  (1000) dravignani  (1000)       38 2024-01-31 21:53:45.515863 likefit-0.2.0/setup.cfg
-drwxrwxr-x   0 dravignani  (1000) dravignani  (1000)        0 2024-01-31 21:53:45.515863 likefit-0.2.0/test/
--rw-rw-r--   0 dravignani  (1000) dravignani  (1000)     1220 2024-01-30 15:47:44.000000 likefit-0.2.0/test/test_binomial.py
--rw-rw-r--   0 dravignani  (1000) dravignani  (1000)      917 2024-01-30 16:45:09.000000 likefit-0.2.0/test/test_least_squares.py
--rw-rw-r--   0 dravignani  (1000) dravignani  (1000)     1499 2024-01-30 15:47:44.000000 likefit-0.2.0/test/test_linear_least_squares.py
--rw-rw-r--   0 dravignani  (1000) dravignani  (1000)      822 2024-01-30 15:19:17.000000 likefit-0.2.0/test/test_poisson.py
+drwxrwxr-x   0 dravignani  (1000) dravignani  (1000)        0 2024-05-07 20:39:24.281521 likefit-0.2.1/
+-rw-rw-r--   0 dravignani  (1000) dravignani  (1000)     1081 2024-01-04 20:52:55.000000 likefit-0.2.1/LICENSE
+-rw-r--r--   0 dravignani  (1000) dravignani  (1000)     2908 2024-05-07 20:39:24.281521 likefit-0.2.1/PKG-INFO
+-rw-rw-r--   0 dravignani  (1000) dravignani  (1000)      957 2024-01-31 21:49:45.000000 likefit-0.2.1/README.md
+drwxrwxr-x   0 dravignani  (1000) dravignani  (1000)        0 2024-05-07 20:39:24.281521 likefit-0.2.1/likefit.egg-info/
+-rw-r--r--   0 dravignani  (1000) dravignani  (1000)     2908 2024-05-07 20:39:24.000000 likefit-0.2.1/likefit.egg-info/PKG-INFO
+-rw-rw-r--   0 dravignani  (1000) dravignani  (1000)      301 2024-05-07 20:39:24.000000 likefit-0.2.1/likefit.egg-info/SOURCES.txt
+-rw-rw-r--   0 dravignani  (1000) dravignani  (1000)        1 2024-05-07 20:39:24.000000 likefit-0.2.1/likefit.egg-info/dependency_links.txt
+-rw-rw-r--   0 dravignani  (1000) dravignani  (1000)       62 2024-05-07 20:39:24.000000 likefit-0.2.1/likefit.egg-info/requires.txt
+-rw-rw-r--   0 dravignani  (1000) dravignani  (1000)        8 2024-05-07 20:39:24.000000 likefit-0.2.1/likefit.egg-info/top_level.txt
+-rw-rw-r--   0 dravignani  (1000) dravignani  (1000)    35226 2024-02-21 19:43:03.000000 likefit-0.2.1/likefit.py
+-rw-rw-r--   0 dravignani  (1000) dravignani  (1000)      788 2024-05-07 20:37:42.000000 likefit-0.2.1/pyproject.toml
+-rw-rw-r--   0 dravignani  (1000) dravignani  (1000)       38 2024-05-07 20:39:24.281521 likefit-0.2.1/setup.cfg
+drwxrwxr-x   0 dravignani  (1000) dravignani  (1000)        0 2024-05-07 20:39:24.281521 likefit-0.2.1/test/
+-rw-rw-r--   0 dravignani  (1000) dravignani  (1000)     1447 2024-02-20 16:08:57.000000 likefit-0.2.1/test/test_binomial.py
+-rw-rw-r--   0 dravignani  (1000) dravignani  (1000)     1284 2024-02-14 14:26:02.000000 likefit-0.2.1/test/test_least_squares.py
+-rw-rw-r--   0 dravignani  (1000) dravignani  (1000)     1799 2024-02-14 14:26:02.000000 likefit-0.2.1/test/test_linear_least_squares.py
+-rw-rw-r--   0 dravignani  (1000) dravignani  (1000)      822 2024-01-30 15:19:17.000000 likefit-0.2.1/test/test_poisson.py
```

### Comparing `likefit-0.2.0/LICENSE` & `likefit-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `likefit-0.2.0/PKG-INFO` & `likefit-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: likefit
-Version: 0.2.0
+Version: 0.2.1
 Summary: Fit data with least squares and other likelihood methods
 Author-email: Diego Ravignani <diego.ravignani@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Diego Ravignani Guerrero
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `likefit-0.2.0/README.md` & `likefit-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `likefit-0.2.0/likefit.egg-info/PKG-INFO` & `likefit-0.2.1/likefit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: likefit
-Version: 0.2.0
+Version: 0.2.1
 Summary: Fit data with least squares and other likelihood methods
 Author-email: Diego Ravignani <diego.ravignani@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Diego Ravignani Guerrero
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `likefit-0.2.0/likefit.py` & `likefit-0.2.1/likefit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Library to fit data with several likelihood functions
 
+import math
 from abc import ABC, abstractmethod
-
+import collections.abc
 import numpy as np
 from scipy.optimize import minimize
 from scipy.stats import chi2
 import matplotlib.pyplot as plt
-from matplotlib import cm, colors
+from matplotlib import colors
 
 
 # Cost functions of the dependent variable y
 def normal_cost(mu: np.ndarray, ydata: np.ndarray, ydata_error: np.ndarray) -> np.ndarray:
     """
     Calculate the squared z-scores for a normal distribution.
 
@@ -73,25 +74,26 @@
     likelihood_ratio2 = nevents2 * np.log(mu2 / nevents2) - (mu2 - nevents2)
     cost2 = -2 * likelihood_ratio2
     cost[~zero_mask] += cost2
 
     return cost
 
 
-def binomial_cost(proba: np.ndarray, nsuccess: np.ndarray, ntrials: np.ndarray) -> np.ndarray:
+def binomial_cost(proba: float or np.ndarray, nsuccess: float or np.ndarray, ntrials: float or np.ndarray) \
+        -> np.ndarray:
     """
     Calculate the binomial costs for each data point.
 
     Parameters
     ----------
-    proba : np.ndarray
+    proba : float or np.ndarray
         Array of success probabilities for each data point.
-    nsuccess : np.ndarray
+    nsuccess : float or np.ndarray
         Array of the number of successes for each data point.
-    ntrials : np.ndarray
+    ntrials : float or np.ndarray
         Array of the number of trials for each data point.
 
     Returns
     -------
     np.ndarray
         Binomial costs for each data point.
     """
@@ -99,43 +101,53 @@
     """
     The function is defined piecewise for the following cases:
         1) nsuccess=0
         2) 0 < nsuccess < ntrials
         3) nsuccess=ntrials
     """
 
+    proba = np.asarray(proba)
+
+    # If nsuccess is scalar expand to the length of the proba array
+    if not isinstance(nsuccess, collections.abc.Sequence):
+        nsuccess = np.ones_like(proba) * nsuccess
+
+    # If ntrials is scalar expand to the length of the proba array
+    if not isinstance(ntrials, collections.abc.Sequence):
+        ntrials = np.ones_like(proba) * ntrials
+
     cost = np.zeros_like(proba)
 
     # Maximum likelihood estimator of the Bernoulli probability
     proba_mle = nsuccess / ntrials
 
     # Case nsuccess = 0
     zero_mask = nsuccess == 0
     proba1 = proba[zero_mask]
     ntrials1 = ntrials[zero_mask]
     likelihood_ratio1 = ntrials1 * np.log(1 - proba1)
-    cost1 = -2 * likelihood_ratio1.sum()
+    cost1 = -2 * likelihood_ratio1
     cost[zero_mask] += cost1
 
     # Case 0 < nsuccess < ntrials
     intermediate_mask = np.logical_and(0 < nsuccess, nsuccess < ntrials)
     proba2 = proba[intermediate_mask]
     ntrials2 = ntrials[intermediate_mask]
     proba_mle2 = proba_mle[intermediate_mask]
     likelihood_ratio2 = ntrials2 * (proba_mle2 * np.log(proba2 / proba_mle2)
                                     + (1 - proba_mle2) * np.log((1 - proba2) / (1 - proba_mle2)))
-    cost2 = -2 * likelihood_ratio2.sum()
+    cost2 = -2 * likelihood_ratio2
     cost[intermediate_mask] += cost2
 
     # Case nsuccess = ntrials
     ntrials_mask = nsuccess == ntrials
     proba3 = proba[ntrials_mask]
     ntrials3 = ntrials[ntrials_mask]
     likelihood_ratio3 = ntrials3 * np.log(proba3)
-    cost3 = -2 * likelihood_ratio3.sum()
+    cost3 = -2 * likelihood_ratio3
     cost[ntrials_mask] += cost3
 
     return cost
 
 
 # Base class of all fitters
 class LikelihoodFitter(ABC):
@@ -511,31 +523,35 @@
         """
         
         print("Fit summary")
         print(f"Estimators: {self.get_estimators()}")
         print(f"Errors: {self.get_errors()}")
         print(f"Covariance matrix: {self.get_covariance_matrix()}")
         print(f"Correlation matrix: {self.get_correlation_matrix()}")
-        print(f"Deviance: {self.get_chi_square()}")
+        print(f"Chi square: {self.get_chi_square()}")
         print(f"Degrees of freedom: {self.get_ndof()}")
         print(f"Pvalue: {self.get_pvalue()}")
 
-    def plot_fit(self, xlabel="x", ylabel="y"):
+    def plot_fit(self, xlabel="x", ylabel="y", ax=None):
         """
         Plot the data, the fit, and the error band.
 
         Parameters
         ----------
         xlabel : str, optional
             Label for the x-axis.
         ylabel : str, optional
             Label for the y-axis.
+        ax : matplotlib.axis.Axis, optional
+            Axis to make the plot.
         """
-        
-        fig, ax = plt.subplots()
+
+        if ax is None:
+            fig, ax = plt.subplots()
+
         ax.set_xlabel(xlabel)
         ax.set_ylabel(ylabel)
 
         # Plot data
         ax.errorbar(self.xdata, self.get_ydata(), self.get_ydata_errors(), ls='none', marker='o', label="Data")
 
         # Plot fitter
@@ -549,64 +565,78 @@
         yfit_error = self.get_yfit_error(xfit)
         ax.fill_between(xfit, yfit - yfit_error, yfit + yfit_error, color='tab:orange', alpha=0.2)
 
         plt.legend()
         plt.tight_layout()
         plt.show()
 
-    def plot_confidence_ellipses(self, parx_index, pary_index, xlabel=None, ylabel=None):
+    def plot_confidence_ellipses(self, parx_index=0, pary_index=1, nsigma=2, ax=None):
         """
-        Plot the 1σ and 2σ confidence ellipses for a pair of parameters.
+        Plot the confidence ellipses for a pair of parameters.
 
         Parameters
         ----------
-        parx_index : int
-            Index of the x-axis parameter.
-        pary_index : int
-            Index of the y-axis parameter.
-        xlabel : str, optional
-            Label for the x-axis.
-        ylabel : str, optional
-            Label for the y-axis.
+        parx_index : int, optional
+            Index of the x-axis parameter. The first parameter is plotted by default.
+        pary_index : int, optional
+            Index of the y-axis parameter. The second parameter is plotted by default.
+        nsigma : int, optional
+            Number of confidence ellipses to plot.
+        ax : matplotlib.axis.Axis, optional
+            Axis to make the plot.
         """
 
-        fig, ax = plt.subplots()
-        ax.set_xlabel(xlabel)
-        ax.set_ylabel(ylabel)
+        if ax is None:
+            fig, ax = plt.subplots()
+            ax.set_xlabel(f"Parameter {parx_index}")
+            ax.set_ylabel(f"Parameter {pary_index}")
 
         estimators = self.get_estimators()
-        plt.plot(estimators[parx_index], estimators[pary_index], 'o', label="Estimator")
+        ax.plot(estimators[parx_index], estimators[pary_index], 'o', label="Estimator")
 
-        ellipse1 = self.get_confidence_ellipse(parx_index, pary_index, nsigma=1)
-        plt.plot(*ellipse1, label=r"1σ")
-        ellipse2 = self.get_confidence_ellipse(parx_index, pary_index, nsigma=2)
-        plt.plot(*ellipse2, label=r"2σ")
+        # Set plot limits
+        errors = self.get_errors()
 
-        plt.legend()
-        plt.tight_layout()
-        plt.show()
+        parx_min = estimators[parx_index] - (nsigma+1) * errors[parx_index]
+        parx_max = estimators[parx_index] + (nsigma+1) * errors[parx_index]
+        ax.set_xlim(parx_min, parx_max)
+
+        pary_min = estimators[pary_index] - (nsigma+1) * errors[pary_index]
+        pary_max = estimators[pary_index] + (nsigma+1) * errors[pary_index]
+        ax.set_ylim(pary_min, pary_max)
 
-    def plot_cost_function(self, parx_index, pary_index, xlabel=None, ylabel=None, nsigma=2):
+        for k in np.arange(start=1, stop=nsigma+1):
+            ellipse = self.get_confidence_ellipse(parx_index, pary_index, nsigma=k)
+            ax.plot(*ellipse, ls='--', label=f"{k}σ")
+
+        ax.legend()
+
+    def plot_cost_function(self, parx_index=0, pary_index=1, nsigma=2, ax=None):
         """
         Plot the surface of the fit cost function for a pair of parameters.
 
         Parameters
         ----------
         parx_index : int
-            Index of the x-axis parameter.
+            Index of the x-axis parameter. The first parameter is plotted by default.
         pary_index : int
-            Index of the y-axis parameter.
-        xlabel : str, optional
-            Label for the x-axis.
-        ylabel : str, optional
-            Label for the y-axis.
+            Index of the y-axis parameter. The second parameter is plotted by default.
         nsigma : int, optional
             Number of sigma confidence levels to include in the plot.
+        ax : matplotlib.axis.Axis, optional
+            Axis to make the plot.
         """
 
+        # TODO: fix the clipping of the z-axis title
+        if ax is None:
+            fig = plt.figure(figsize=(5, 4))
+            ax = fig.subplots(subplot_kw={'projection': '3d'})
+            ax.set_xlabel(f"Parameter {parx_index}")
+            ax.set_ylabel(f"Parameter {pary_index}")
+
         # Calculate coordinates of the points to plot
         estimators = self.get_estimators()
         errors = self.get_errors()
 
         parx_min = estimators[parx_index] - nsigma * errors[parx_index]
         parx_max = estimators[parx_index] + nsigma * errors[parx_index]
         parx = np.linspace(parx_min, parx_max, num=50)
@@ -616,94 +646,76 @@
         pary = np.linspace(pary_min, pary_max, num=50)
 
         x, y = np.meshgrid(parx, pary)
         cost = self.vcost_function(parx_index, pary_index, parx, pary)
         z = cost - cost.min()
 
         # Plot
-        fig = plt.figure(figsize=(5, 4))
-        ax = fig.subplots(subplot_kw={"projection": "3d"})
-        ax.set_xlabel(xlabel)
-        ax.set_ylabel(ylabel)
         ax.set_zlabel(r"$-2\log(L/L_{max})$")
 
-        # Levels of the contour lines
-        sigma_levels = np.arange(0, 7)
-        bounds = sigma_levels ** 2
-        norm = colors.BoundaryNorm(boundaries=bounds, ncolors=128)
-        surf = ax.plot_surface(x, y, z, cmap=cm.coolwarm, norm=norm)
-
-        # Plot colorbar
-        clb = plt.colorbar(surf, shrink=0.5, location='left')
-        clb.ax.set_title(r"$\sigma^2$")
+        # Scale the colors quadratically with z to include all the colormap evenly
+        sigma_max = math.sqrt(z.max())
+        sigma_levels = np.arange(0, sigma_max, step=0.1)
+        bounds = sigma_levels**2
+        norm = colors.BoundaryNorm(boundaries=bounds, ncolors=256)
 
-        plt.show()
+        ax.plot_surface(x, y, z, cmap=plt.cm.viridis_r, norm=norm)
 
-    def plot_confidence_regions(self, parx_index, pary_index, xlabel=None, ylabel=None, nsigma=2):
+    def plot_confidence_regions(self, parx_index=0, pary_index=1, nsigma=2, ax=None):
         """
         Plot the confidence regions for a pair of parameters.
 
         Parameters
         ----------
         parx_index : int
-            Index of the x-axis parameter.
+            Index of the x-axis parameter. The first parameter is plotted by default.
         pary_index : int
-            Index of the y-axis parameter.
-        xlabel : str, optional
-            Label for the x-axis.
-        ylabel : str, optional
-            Label for the y-axis.
+            Index of the y-axis parameter. The second parameter is plotted by default.
         nsigma : int, optional
             Number of sigma confidence levels to plot.
+        ax : matplotlib.axis.Axis, optional
+            Axis to make the plot.
 
         Returns
         -------
         None
         """
-        
+
+        if ax is None:
+            fig, ax = plt.subplots()
+            ax.set_xlabel(f"Parameter {parx_index}")
+            ax.set_ylabel(f"Parameter {pary_index}")
+
         # Calculate coordinates of the points to plot
         estimators = self.get_estimators()
         errors = self.get_errors()
 
         parx_min = estimators[parx_index] - (nsigma+1) * errors[parx_index]
         parx_max = estimators[parx_index] + (nsigma+1) * errors[parx_index]
         parx = np.linspace(parx_min, parx_max, num=50)
 
         pary_min = estimators[pary_index] - (nsigma+1) * errors[pary_index]
         pary_max = estimators[pary_index] + (nsigma+1) * errors[pary_index]
         pary = np.linspace(pary_min, pary_max, num=50)
 
         x, y = np.meshgrid(parx, pary)
         cost = self.vcost_function(parx_index, pary_index, parx, pary)
-        z = np.sqrt(cost - cost.min())
-
-        # Plot
-        fig, ax = plt.subplots()
-        ax.set_xlabel(xlabel)
-        ax.set_ylabel(ylabel)
+        z = cost - cost.min()
 
         # Levels of the contour lines
-        sigma_levels = np.arange(0, nsigma+1)
-        contours = ax.contour(x, y, z, levels=sigma_levels, colors='black', linestyles='dashed')
+        cost_levels = np.arange(0, nsigma+1)**2
+        contours = ax.contour(x, y, z, levels=cost_levels, colors='black', linestyles='dashed')
 
-        def fmt(nsigma_label):
-            return f"{nsigma_label:.0f}σ"
+        def fmt(level):
+            sigma_label = math.sqrt(level)
+            return f"{sigma_label:.0f}σ"
 
         ax.clabel(contours, contours.levels, fmt=fmt, inline=True)
 
         plt.pcolormesh(x, y, z, shading='auto', cmap=plt.cm.viridis_r)
-        clb = plt.colorbar()
-        clb.ax.set_title(r"$n\sigma$")
-
-        # contours = ax.contourf(xdata, ydata, np.sqrt(z), levels=sigma_levels, cmap='Blues_r')
-        # clb = fig.colorbar(contours)
-        # clb.ax.set_title(r"$n\sigma$")
-
-        plt.tight_layout()
-        plt.show()
 
 
 class LinearLeastSquares(LikelihoodFitter):
     """
     Linear least squares fitter based on the LikelihoodFitter base class.
 
     Parameters
@@ -731,33 +743,41 @@
         Matrix generated by the linear model.
     estimators : np.ndarray
         Maximum likelihood estimators of the fit parameters.
     cova_par : np.ndarray
         Covariance matrix of the fit parameters.
     """
 
-    def __init__(self, xdata, ydata, ydata_error, model):
+    def __init__(self, xdata, ydata, model, ydata_error=1):
         """
         Initialize the LinearLeastSquares instance.
 
         Parameters
         ----------
         xdata : array_like
             The independent variable data.
         ydata : array_like
             The dependent variable data.
-        ydata_error : array_like
-            Errors associated with the dependent variable data.
         model : callable
             The linear model function to fit the data.
+        ydata_error : array_like or float, optional
+            Errors associated with the dependent variable data. It must be the an array of same size as ydata
+            if the errors depend on the data point or a float if the all errors are equal. By default, the
+            errors are set to 1.
         """
         
         LikelihoodFitter.__init__(self, xdata, model)
         self.ydata = ydata
-        self.ydata_error = ydata_error
+
+        # If ydata_error is scalar expand to the length of the ydata array
+        if isinstance(ydata_error, collections.abc.Sequence):
+            self.ydata_error = ydata_error
+        else:
+            self.ydata_error = np.ones_like(ydata) * ydata_error
+
         npar = self.__count_parameters()
         self.__set_model_matrix(npar)
 
     def __count_parameters(self):
         """
         Count the number of the fit parameters 
 
@@ -924,33 +944,40 @@
         The dependent variable data.
     ydata_error : array_like
         Errors associated with the dependent variable data.
     model : callable
         The non-linear model function to fit the data.
     """
     
-    def __init__(self, xdata, ydata, ydata_error, model):
+    def __init__(self, xdata, ydata, model, ydata_error=1):
         """
         Initialize the LeastSquares instance.
 
         Parameters
         ----------
         xdata : array_like
             The independent variable data.
         ydata : array_like
             The dependent variable data.
-        ydata_error : array_like
-            Errors associated with the dependent variable data.
         model : callable
-            The non-linear model function to fit the data.
+            The linear model function to fit the data.
+        ydata_error : array_like or float, optional
+            Errors associated with the dependent variable data. It must be the an array of same size as ydata
+            if the errors depend on the data point or a float if the all errors are equal. By default, the
+            errors are set to 1.
         """
         
         LikelihoodFitter.__init__(self, xdata, model)
         self.ydata = ydata
-        self.ydata_error = ydata_error
+
+        # If ydata_error is scalar expand to the length of the ydata array
+        if isinstance(ydata_error, collections.abc.Sequence):
+            self.ydata_error = ydata_error
+        else:
+            self.ydata_error = np.ones_like(ydata) * ydata_error
 
     def cost_function(self, par):
         """
         Calculate the cost function for the non-linear least squares fit.
 
         Parameters
         ----------
```

### Comparing `likefit-0.2.0/pyproject.toml` & `likefit-0.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "likefit"
-version = "0.2.0"
+version = "0.2.1"
 description = "Fit data with least squares and other likelihood methods"
 readme = "README.md"
 authors = [{ name = "Diego Ravignani", email = "diego.ravignani@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `likefit-0.2.0/test/test_binomial.py` & `likefit-0.2.1/test/test_binomial.py`

 * *Files 20% similar despite different names*

```diff
@@ -31,13 +31,23 @@
     assert binomial_fitter.fit(seed, tol=1e-4) == 0
 
 
 def test_cost_function(binomial_fitter):
     # Test the cost function with some dummy parameters
     par = np.array([0.5, 1])
     cost = binomial_fitter.cost_function(par)
-    assert cost == 2619.431668583625
+    assert cost == 298.832751257985
 
 
 def test_get_ydata(binomial_fitter):
     ydata = binomial_fitter.get_ydata()
     assert np.array_equal(ydata, nsuccess/ntrials)
+
+
+def test_cost_single_trial():
+    ntrials = 30
+    nsuccess = 15
+    proba = np.linspace(0.3, 0.7)
+    cost = likefit.binomial_cost(proba, nsuccess, ntrials)
+    cost_sum = cost.sum()
+    assert cost_sum == 87.78818608512154
+
```

### Comparing `likefit-0.2.0/test/test_least_squares.py` & `likefit-0.2.1/test/test_least_squares.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,20 +10,34 @@
 # fit_model vectorized in xdata
 def fit_model(x, par):
     return par[0] * np.exp(par[1] * x)
 
 
 @pytest.fixture
 def least_squares_fitter():
-    return likefit.LeastSquares(xdata, ydata, ysigma, fit_model)
+    return likefit.LeastSquares(xdata, ydata, fit_model, ysigma)
 
 
 def test_initialization(least_squares_fitter):
     assert np.array_equal(least_squares_fitter.xdata, xdata)
     assert np.array_equal(least_squares_fitter.ydata, ydata)
     assert np.array_equal(least_squares_fitter.ydata_error, ysigma)
     assert least_squares_fitter.model is fit_model
 
 
 def test_fit(least_squares_fitter):
     seed = np.array([0, 0])
     assert least_squares_fitter.fit(seed) == 0
+
+
+def test_constant_errors():
+    ysigma_constant = 1
+    fitter = likefit.LeastSquares(xdata, ydata, fit_model, ysigma_constant)
+    seed = np.array([0, 0])
+    res = fitter.fit(seed)
+    assert res == 0
+
+def test_default_errors():
+    fitter = likefit.LeastSquares(xdata, ydata, fit_model)
+    seed = np.array([0, 0])
+    res = fitter.fit(seed)
+    assert res == 0
```

### Comparing `likefit-0.2.0/test/test_linear_least_squares.py` & `likefit-0.2.1/test/test_linear_least_squares.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Model linear in the parameters
 def fit_model(x, par):
     return par[0] + par[1] * x
 
 
 @pytest.fixture
 def linear_least_squares_fitter():
-    return LinearLeastSquares(xdata, ydata, ysigma, fit_model)
+    return LinearLeastSquares(xdata, ydata, fit_model, ysigma)
 
 
 def test_initialization(linear_least_squares_fitter):
     assert np.array_equal(linear_least_squares_fitter.xdata, xdata)
     assert np.array_equal(linear_least_squares_fitter.ydata, ydata)
     assert np.array_equal(linear_least_squares_fitter.ydata_error, ysigma)
     assert linear_least_squares_fitter.model is fit_model
@@ -33,7 +33,20 @@
     assert npar == 2  # Assuming a simple linear model with two parameters (slope and intercept)
 
 
 def test_fit(linear_least_squares_fitter):
     linear_least_squares_fitter.fit()
     estimators = np.array([2.1192891, -0.7269067])
     assert np.array_equal(linear_least_squares_fitter.estimators.round(7), estimators)
+
+
+def test_constant_errors():
+    ysigma_constant = 1
+    fitter = LinearLeastSquares(xdata, ydata, fit_model, ysigma_constant)
+    res = fitter.fit()
+    assert res == 0
+
+
+def test_default_errors():
+    fitter = LinearLeastSquares(xdata, ydata, fit_model)
+    res = fitter.fit()
+    assert res == 0
```

### Comparing `likefit-0.2.0/test/test_poisson.py` & `likefit-0.2.1/test/test_poisson.py`

 * *Files identical despite different names*

