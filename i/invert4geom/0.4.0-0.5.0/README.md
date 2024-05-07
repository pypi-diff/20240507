# Comparing `tmp/invert4geom-0.4.0.tar.gz` & `tmp/invert4geom-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invert4geom-0.4.0.tar", last modified: Thu Feb 22 02:30:44 2024, max compression
+gzip compressed data, was "invert4geom-0.5.0.tar", last modified: Tue May  7 16:35:17 2024, max compression
```

## Comparing `invert4geom-0.4.0.tar` & `invert4geom-0.5.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 02:30:44.473054 invert4geom-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-02-22 02:30:27.000000 invert4geom-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8430 2024-02-22 02:30:44.473054 invert4geom-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-02-22 02:30:27.000000 invert4geom-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-02-22 02:30:27.000000 invert4geom-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 02:30:44.477054 invert4geom-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 02:30:44.469054 invert4geom-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 02:30:44.469054 invert4geom-0.4.0/src/invert4geom/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-02-22 02:30:27.000000 invert4geom-0.4.0/src/invert4geom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-02-22 02:30:27.000000 invert4geom-0.4.0/src/invert4geom/cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    33902 2024-02-22 02:30:27.000000 invert4geom-0.4.0/src/invert4geom/inversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    16372 2024-02-22 02:30:27.000000 invert4geom-0.4.0/src/invert4geom/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    28552 2024-02-22 02:30:27.000000 invert4geom-0.4.0/src/invert4geom/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-02-22 02:30:27.000000 invert4geom-0.4.0/src/invert4geom/regional.py
--rw-r--r--   0 runner    (1001) docker     (127)    10611 2024-02-22 02:30:27.000000 invert4geom-0.4.0/src/invert4geom/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)    27868 2024-02-22 02:30:27.000000 invert4geom-0.4.0/src/invert4geom/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 02:30:44.473054 invert4geom-0.4.0/src/invert4geom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8430 2024-02-22 02:30:44.000000 invert4geom-0.4.0/src/invert4geom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-02-22 02:30:44.000000 invert4geom-0.4.0/src/invert4geom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 02:30:44.000000 invert4geom-0.4.0/src/invert4geom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-02-22 02:30:44.000000 invert4geom-0.4.0/src/invert4geom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-22 02:30:44.000000 invert4geom-0.4.0/src/invert4geom.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 02:30:44.473054 invert4geom-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 02:30:27.000000 invert4geom-0.4.0/tests/test_cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    25647 2024-02-22 02:30:27.000000 invert4geom-0.4.0/tests/test_inversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-02-22 02:30:27.000000 invert4geom-0.4.0/tests/test_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-02-22 02:30:27.000000 invert4geom-0.4.0/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 02:30:27.000000 invert4geom-0.4.0/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-02-22 02:30:27.000000 invert4geom-0.4.0/tests/test_regional.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 02:30:27.000000 invert4geom-0.4.0/tests/test_synthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)    25474 2024-02-22 02:30:27.000000 invert4geom-0.4.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:35:17.067020 invert4geom-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-07 16:35:10.000000 invert4geom-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-05-07 16:35:17.067020 invert4geom-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-07 16:35:10.000000 invert4geom-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-05-07 16:35:10.000000 invert4geom-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 16:35:17.067020 invert4geom-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:35:17.059020 invert4geom-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:35:17.059020 invert4geom-0.5.0/src/invert4geom/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-07 16:35:10.000000 invert4geom-0.5.0/src/invert4geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11122 2024-05-07 16:35:10.000000 invert4geom-0.5.0/src/invert4geom/cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36264 2024-05-07 16:35:10.000000 invert4geom-0.5.0/src/invert4geom/inversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16430 2024-05-07 16:35:10.000000 invert4geom-0.5.0/src/invert4geom/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31522 2024-05-07 16:35:10.000000 invert4geom-0.5.0/src/invert4geom/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9879 2024-05-07 16:35:10.000000 invert4geom-0.5.0/src/invert4geom/regional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-05-07 16:35:10.000000 invert4geom-0.5.0/src/invert4geom/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27879 2024-05-07 16:35:10.000000 invert4geom-0.5.0/src/invert4geom/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:35:17.063020 invert4geom-0.5.0/src/invert4geom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-05-07 16:35:17.000000 invert4geom-0.5.0/src/invert4geom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-07 16:35:17.000000 invert4geom-0.5.0/src/invert4geom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 16:35:17.000000 invert4geom-0.5.0/src/invert4geom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-07 16:35:17.000000 invert4geom-0.5.0/src/invert4geom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 16:35:17.000000 invert4geom-0.5.0/src/invert4geom.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:35:17.063020 invert4geom-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:35:10.000000 invert4geom-0.5.0/tests/test_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25647 2024-05-07 16:35:10.000000 invert4geom-0.5.0/tests/test_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-07 16:35:10.000000 invert4geom-0.5.0/tests/test_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-07 16:35:10.000000 invert4geom-0.5.0/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:35:10.000000 invert4geom-0.5.0/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-05-07 16:35:10.000000 invert4geom-0.5.0/tests/test_regional.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:35:10.000000 invert4geom-0.5.0/tests/test_synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25696 2024-05-07 16:35:10.000000 invert4geom-0.5.0/tests/test_utils.py
```

### Comparing `invert4geom-0.4.0/LICENSE` & `invert4geom-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invert4geom-0.4.0/PKG-INFO` & `invert4geom-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invert4geom
-Version: 0.4.0
+Version: 0.5.0
 Summary: Constrained gravity inversion to recover the geometry of a density contrast.
 Author-email: Matt Tankersley <matt.d.tankersley@gmail.com>
 License: Copyright 2023 Matt Tankersley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
@@ -60,24 +60,26 @@
 Requires-Dist: nptyping
 Requires-Dist: numba_progress
 Requires-Dist: tqdm
 Requires-Dist: pygmt
 Requires-Dist: dask
 Provides-Extra: opti
 Requires-Dist: optuna>=3.1.0; extra == "opti"
+Requires-Dist: optuna-integration; extra == "opti"
 Requires-Dist: botorch>=0.4.0; extra == "opti"
 Requires-Dist: joblib; extra == "opti"
 Requires-Dist: psutil; extra == "opti"
 Requires-Dist: tqdm_joblib; extra == "opti"
 Provides-Extra: viz
 Requires-Dist: pyvista; extra == "viz"
 Requires-Dist: trame; extra == "viz"
 Requires-Dist: ipywidgets; extra == "viz"
 Requires-Dist: matplotlib; extra == "viz"
 Requires-Dist: seaborn; extra == "viz"
+Requires-Dist: ipython; extra == "viz"
 Provides-Extra: test
 Requires-Dist: pytest>=6; extra == "test"
 Requires-Dist: pytest-cov>=3; extra == "test"
 Requires-Dist: invert4geom[opti]; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx>=4.0; extra == "docs"
 Requires-Dist: myst_parser; extra == "docs"
```

### Comparing `invert4geom-0.4.0/README.md` & `invert4geom-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `invert4geom-0.4.0/pyproject.toml` & `invert4geom-0.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Scientific/Engineering",
   "Typing :: Typed",
 ]
 readme = "README.md"
-version = "0.4.0"
+version = "0.5.0"
 license = {file = "LICENSE"}
 
 keywords = ["inversion", "gravity", "geometry", "density", "Moho", "sediment", "geophysics", "geology", "geoscience"]
 
 dependencies = [
   "numpy",
   "pandas",
@@ -49,25 +49,27 @@
   "pygmt",
   "dask",
 ]
 
 [project.optional-dependencies]
 opti = [
   "optuna>=3.1.0", # need JournalStorage
+  "optuna-integration",
   "botorch>=0.4.0",
   "joblib",
   "psutil",
   "tqdm_joblib",
 ]
 viz = [
   "pyvista",
   "trame",
   "ipywidgets",
   "matplotlib",
   "seaborn",
+  "ipython",
 ]
 test = [
   "pytest >=6",
   "pytest-cov >=3",
   "invert4geom[opti]",
 ]
 docs = [
```

### Comparing `invert4geom-0.4.0/src/invert4geom/cross_validation.py` & `invert4geom-0.5.0/src/invert4geom/cross_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
             test.northing,
             test.upward,
         ),
         field="g_z",
         progressbar=progressbar,
     )
 
-    # compare new layer1 forward with observed
+    # compare forward of inverted layer with observed
     observed = test[kwargs.get("input_grav_column")] - test.reg
     predicted = test.test_point_grav
 
     dif = predicted - observed
 
     score = utils.rmse(dif)
```

### Comparing `invert4geom-0.4.0/src/invert4geom/inversion.py` & `invert4geom-0.5.0/src/invert4geom/inversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 import typing
 
 import harmonica as hm
 import numba
 import numpy as np
 import pandas as pd
 import scipy as sp
+import verde as vd
 import xarray as xr
 from nptyping import NDArray
+from tqdm.autonotebook import tqdm
 
 from invert4geom import plotting, utils
 
 
 @numba.jit(cache=True, nopython=True)  # type: ignore[misc]
 def grav_column_der(
     grav_easting: NDArray,
@@ -322,14 +324,24 @@
         #   k:prisms_layer[k].to_numpy().ravel() for k in list(prisms_layer.variables)}
         df = prisms_layer.to_dataframe().reset_index().dropna().astype(float)  # type: ignore[union-attr]
         prism_easting = df.easting.to_numpy()
         prism_northing = df.northing.to_numpy()
         prism_top = df.top.to_numpy()
         prism_density = df.density.to_numpy()
 
+        if np.all((prism_top - grav_upward.mean()) == 0):
+            msg = (
+                "All prism tops coincides exactly with the elevation of the gravity "
+                "observation points, leading to issues with calculating the vertical "
+                "derivative of gravity with the annulus technique. Either slightly "
+                "change the prism tops or gravity elevations, or use the small-prisms "
+                "vertical derivative technique."
+            )
+            logging.warning(msg)
+
         jac = jacobian_annular(
             grav_easting,
             grav_northing,
             grav_upward,
             prism_easting,
             prism_northing,
             prism_top,
@@ -491,15 +503,15 @@
     # elif solver_type == "numpy least squares":
     #     step = np.linalg.lstsq(
     #         jac,
     #         residuals,
     #     )[0]
 
     # elif solver_type == "steepest descent":
-    #     """Jacobian transppose algorithm"""
+    #     """Jacobian transpose algorithm"""
     #     residuals = residuals
     #     step = jac.T @ residuals
 
     # elif solver_type == "gauss newton":
     #     """
     #     Gauss Newton w/ 1st order Tikhonov regularization
     #     from https://nbviewer.org/github/compgeolab/2020-aachen-inverse-problems/blob/main/gravity-inversion.ipynb # noqa: E501
@@ -718,15 +730,15 @@
 
     # update the forward gravity
     gravity[f"iter_{iteration_number}_forward_grav"] = prisms_ds.prism_layer.gravity(
         coordinates=(gravity.easting, gravity.northing, gravity.upward),
         field="g_z",
     )
 
-    # each iteration updates the topography of the layer to minizime the residual
+    # each iteration updates the topography of the layer to minimize the residual
     # portion of the misfit. We then want to recalculate the forward gravity of the
     # new layer, use the same original regional misfit, and re-calculate the residual
     # Gmisfit  = Gobs_corr - Gforward
     # Gres = Gmisfit - Greg
     # Gres = Gobs_corr_shift - Gforward - Greg
     # update the residual misfit with the new forward gravity and the same regional
     gravity[f"iter_{iteration_number}_final_misfit"] = (
@@ -751,15 +763,17 @@
     deriv_type: str = "annulus",
     jacobian_prism_size: float = 1,
     solver_type: str = "scipy least squares",
     solver_damping: float | None = None,
     upper_confining_layer: xr.DataArray | None = None,
     lower_confining_layer: xr.DataArray | None = None,
     weights_after_solving: bool = False,
+    inversion_region: tuple[float, float, float, float] | None = None,
     plot_convergence: bool = False,
+    plot_dynamic_convergence: bool = False,
 ) -> tuple[pd.DataFrame, pd.DataFrame, dict[str, typing.Any], float]:
     """
     perform a geometric inversion, where the topography is updated to minimize the
     residual misfit between the forward gravity of the layer, and the observed gravity.
     To aid in regularizing an ill-posed problem choose any of the following options:
     * add damping to the solver, with `solver_damping`
     * weight the surface correction values with a weighting grid with
@@ -767,15 +781,16 @@
     * bound the topography of the layer, with `upper_confining_layer` and
     `lower_confining_layer`
 
     Parameters
     ----------
     input_grav : pd.DataFrame
         dataframe with gravity data and coordinates, must have columns "res" and "reg"
-        for residual and regional gravity.
+        for residual and regional gravity, and coordinate columns "easting", "northing",
+        and "upward".
     input_grav_column : str
         column name containing the gravity data *before* regional separation
     prism_layer : xr.Dataset
         starting prism layer
     density_contrast : float
         density contrast of the prisms layer, should be same value used to create the
         starting model
@@ -803,16 +818,21 @@
     upper_confining_layer : xr.DataArray | None, optional
         topographic layer to use as upper limit for inverted topography, by default None
     lower_confining_layer : xr.DataArray | None, optional
         topographic layer to use as lower limit for inverted topography, by default None
     weights_after_solving : bool, optional
         use "weights" variable of prisms dataset to scale surface corrections grid, by
         default False, by default False
+    inversion_region : tuple[float, float, float, float]
+        inside region to calculated residual RMSE within, in the form (min_easting,
+        max_easting, min_northing, max_northing)
     plot_convergence : bool, optional
         plot the misfit convergence, by default False
+    plot_dynamic_convergence : bool, optional
+        plot the misfit convergence dynamically, by default False
 
     Returns
     -------
     tuple[pd.DataFrame, pd.DataFrame, dict[str, typing.Any], float]
         prisms_df: pd.DataFrame, prism properties for each iteration,
         gravity: pd.DataFrame, gravity anomalies for each iteration,
         params: dict, Properties of the inversion such as kwarg values,
@@ -821,14 +841,21 @@
 
     logging.info("starting inversion")
 
     time_start = time.perf_counter()
 
     gravity = copy.deepcopy(input_grav)
 
+    # if inversion region provided, create column of booleans defining inside/outside
+    if inversion_region is not None:
+        gravity["inside"] = vd.inside(
+            (gravity.easting, gravity.northing),
+            region=inversion_region,
+        )
+
     # extract variables from starting prism layer
     (
         prisms_df,
         prisms_ds,
         prism_spacing,
         _,
     ) = utils.extract_prism_data(prism_layer)
@@ -851,15 +878,16 @@
 
     # set starting delta L2 norm to positive infinity
     delta_l2_norm = np.inf
 
     # iteration times
     iter_times = []
 
-    for iteration, _ in enumerate(range(max_iterations), start=1):
+    pbar = tqdm(range(max_iterations), desc="Iteration")
+    for iteration, _ in enumerate(pbar, start=1):
         logging.info(
             "\n #################################### \n iteration %s", iteration
         )
         # start iteration timer
         iter_time_start = time.perf_counter()
 
         # after first iteration reset residual with previous iteration's results
@@ -869,18 +897,25 @@
             gravity["res"] = gravity[f"iter_{iteration-1}_final_misfit"]
             prisms_df["density"] = prisms_df[f"iter_{iteration-1}_density"]
 
         # add starting residual to df
         gravity[f"iter_{iteration}_initial_misfit"] = gravity.res
 
         # set iteration stats
-        initial_rmse = utils.rmse(gravity[f"iter_{iteration}_initial_misfit"])
+        if inversion_region is not None:
+            # if inversion region is supplied, calculate RMSE only within that region
+            initial_rmse = utils.rmse(
+                gravity[gravity.inside][f"iter_{iteration}_initial_misfit"]
+            )
+        else:
+            initial_rmse = utils.rmse(gravity[f"iter_{iteration}_initial_misfit"])
         l2_norm = np.sqrt(initial_rmse)
 
         if iteration == 1:
+            starting_misfit = initial_rmse
             starting_l2_norm = l2_norm
 
         # calculate jacobian sensitivity matrix
         jac = jacobian(
             deriv_type,
             gravity.select_dtypes(include=["number"]),
             empty_jac,
@@ -941,15 +976,21 @@
             gravity,
             prisms_ds,
             input_grav_column,
             iteration,
         )
 
         # update the misfit RMSE
-        updated_rmse = utils.rmse(gravity[f"iter_{iteration}_final_misfit"])
+        if inversion_region is not None:
+            # if inversion region is supplied, calculate RMSE only within that region
+            updated_rmse = utils.rmse(
+                gravity[gravity.inside][f"iter_{iteration}_final_misfit"]
+            )
+        else:
+            updated_rmse = utils.rmse(gravity[f"iter_{iteration}_final_misfit"])
         logging.info("updated misfit RMSE: %s", round(updated_rmse, 4))
         final_rmse = updated_rmse
 
         # update the l2 and delta l2 norms
         previous_delta_l2_norm = copy.copy(delta_l2_norm)
         l2_norm, delta_l2_norm = update_l2_norms(updated_rmse, l2_norm)
         final_l2_norm = l2_norm
@@ -974,15 +1015,25 @@
             starting_l2_norm,
             l2_norm_tolerance,
             delta_l2_norm,
             previous_delta_l2_norm,
             delta_l2_norm_tolerance,
             perc_increase_limit=perc_increase_limit,
         )
+
+        if plot_dynamic_convergence is True:
+            plotting.plot_dynamic_convergence(
+                gravity,
+                l2_norm_tolerance,
+                starting_misfit,
+                inversion_region=inversion_region,
+            )
+
         if end is True:
+            pbar.set_description(f"Inversion ended due to {termination_reason}")
             break
         # end of inversion loop
 
     time_end = time.perf_counter()
 
     elapsed_time = time_end - time_start
 
@@ -1011,10 +1062,14 @@
             f"{round(final_rmse,4)} /{round(final_l2_norm,4)} mGal"
         ),
         "Termination reason": termination_reason,
         "iter_times": iter_times,
     }
 
     if plot_convergence is True:
-        plotting.plot_convergence(gravity, iter_times=iter_times)
+        plotting.plot_convergence(
+            gravity,
+            iter_times=iter_times,
+            inversion_region=inversion_region,
+        )
 
     return prisms_df, gravity, params, elapsed_time
```

### Comparing `invert4geom-0.4.0/src/invert4geom/optimization.py` & `invert4geom-0.5.0/src/invert4geom/optimization.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,14 +196,16 @@
     Run optuna optimization in parallel. Pre-define the study, storage, and objective
     function and input them here.
     """
     if optuna is None:
         msg = "Missing optional dependency 'optuna' required for optimization."
         raise ImportError(msg)
 
+    optuna.logging.set_verbosity(optuna.logging.WARNING)
+
     # load study metadata from storage
     study = optuna.load_study(storage=study_storage, study_name=study_name)
 
     # set up parallel processing and run optimization
     if parallel is True:
         # @utils.supress_stdout
         def optimize_study(
```

### Comparing `invert4geom-0.4.0/src/invert4geom/plotting.py` & `invert4geom-0.5.0/src/invert4geom/plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,22 @@
-from __future__ import annotations
+from __future__ import annotations  # pylint: disable=too-many-lines
 
 import typing
 
 import numpy as np
 import pandas as pd
-import pygmt
+
+try:
+    from IPython.display import clear_output
+except ImportError:
+    clear_output = None
 
 try:
     import matplotlib.pyplot as plt
+    from matplotlib.ticker import MaxNLocator
 except ImportError:
     plt = None
 
 
 try:
     import seaborn as sns
 except ImportError:
@@ -126,14 +131,15 @@
 def plot_cv_scores(
     scores: list[float],
     parameters: list[float],
     logx: bool = False,
     logy: bool = False,
     param_name: str = "Hyperparameter",
     figsize: tuple[float, float] = (5, 3.5),
+    plot_title: str | None = None,
 ) -> None:
     """
     plot a graph of cross-validation scores vs hyperparameter values
 
     Parameters
     ----------
     scores : list[float]
@@ -142,14 +148,16 @@
         parameter values
     logx, logy : bool, optional
         make the x or y axes log scale, by default False
     param_name : str, optional
         name to give for the parameters, by default "Hyperparameter"
     figsize : tuple[float, float], optional
         size of the figure, by default (5, 3.5)
+    plot_title : str | None, optional
+        title of figure, by default None
     """
     # Check if seaborn is installed
     if sns is None:
         msg = "Missing optional dependency 'seaborn' required for plotting."
         raise ImportError(msg)
     sns.set_theme()
     # Check if matplotlib is installed
@@ -159,15 +167,18 @@
 
     df0 = pd.DataFrame({"scores": scores, "parameters": parameters})
     df = df0.sort_values(by="parameters")
 
     best = df.scores.argmin()
 
     plt.figure(figsize=figsize)
-    plt.title(f"{param_name} Cross-validation")
+    if plot_title is not None:
+        plt.title(plot_title)
+    else:
+        plt.title(f"{param_name} Cross-validation")
     plt.plot(df.parameters, df.scores, marker="o")
     plt.plot(
         df.parameters.iloc[best],
         df.scores.iloc[best],
         "s",
         markersize=10,
         color=sns.color_palette()[3],
@@ -184,27 +195,30 @@
     plt.tight_layout()
 
 
 def plot_convergence(
     results: pd.DataFrame,
     iter_times: list[float] | None = None,
     logy: bool = False,
+    inversion_region: tuple[float, float, float, float] | None = None,
     figsize: tuple[float, float] = (5, 3.5),
 ) -> None:
     """
     plot a graph of misfit and time vs iteration number.
 
     Parameters
     ----------
     results : pd.DataFrame
         gravity result dataframe
     iter_times : list[float] | None, optional
         list of iteration execution times, by default None
     logy : bool, optional
         choose whether to plot y axis in log scale, by default False
+    inversion_region : tuple[float, float, float, float] | None, optional
+        inside region of inversion, by default None
     figsize : tuple[float, float], optional
         width and height of figure, by default (5, 3.5)
     """
     # Check if seaborn is installed
     if sns is None:
         msg = "Missing optional dependency 'seaborn' required for plotting."
         raise ImportError(msg)
@@ -214,43 +228,134 @@
     if plt is None:
         msg = "Missing optional dependency 'matplotlib' required for plotting."
         raise ImportError(msg)
 
     # get misfit data at end of each iteration
     cols = [s for s in results.columns.to_list() if "_final_misfit" in s]
     iters = len(cols)
-    final_misfits = [utils.rmse(results[i]) for i in cols]
+    if inversion_region is not None:
+        misfits = [utils.rmse(results[results.inside][i]) for i in cols]
+        starting_misfit = utils.rmse(results[results.inside]["iter_1_initial_misfit"])
+    else:
+        misfits = [utils.rmse(results[i]) for i in cols]
+        starting_misfit = utils.rmse(results["iter_1_initial_misfit"])
+    # add starting misfit to the beginning of the list
+    misfits.insert(0, starting_misfit)
 
     _fig, ax1 = plt.subplots(figsize=figsize)
     plt.title("Inversion convergence")
-    ax1.plot(range(iters), final_misfits, "b-")
+    ax1.plot(range(iters + 1), misfits, "b-")
     ax1.set_xlabel("Iteration")
     if logy:
         ax1.set_yscale("log")
     ax1.set_ylabel("RMS (mGal)", color="b")
     ax1.tick_params(axis="y", colors="b", which="both")
 
     if iter_times is not None:
+        iter_times.insert(0, 0)
         ax2 = ax1.twinx()
-        ax2.plot(range(iters), np.cumsum(iter_times), "g-")
+        ax2.plot(range(iters + 1), np.cumsum(iter_times), "g-")
         ax2.set_ylabel("Cumulative time (s)", color="g")
         ax2.tick_params(axis="y", colors="g")
         ax2.grid(False)
+
+    plt.tight_layout()
+
+
+def plot_dynamic_convergence(
+    results: pd.DataFrame,
+    l2_norm_tolerance: float,
+    starting_misfit: float,
+    inversion_region: tuple[float, float, float, float] | None = None,
+    figsize: tuple[float, float] = (5, 3.5),
+) -> None:
+    """
+    plot a graph of misfit and time vs iteration number.
+
+    Parameters
+    ----------
+    results : pd.DataFrame
+        gravity result dataframe
+    l2_norm_tolerance : float
+        l2 norm tolerance
+    starting_misfit : float
+        starting misfit rmse
+    inversion_region : tuple[float, float, float, float] | None, optional
+        inside region of inversion, by default None
+    figsize : tuple[float, float], optional
+        width and height of figure, by default (5, 3.5)
+    """
+    # Check if seaborn is installed
+    if sns is None:
+        msg = "Missing optional dependency 'seaborn' required for plotting."
+        raise ImportError(msg)
+    sns.set_theme()
+
+    # Check if matplotlib is installed
+    if plt is None:
+        msg = "Missing optional dependency 'matplotlib' required for plotting."
+        raise ImportError(msg)
+
+    # Check if Ipython is installed
+    if clear_output is None:
+        msg = "Missing optional dependency 'IPython' required for plotting."
+        raise ImportError(msg)
+    clear_output(wait=True)
+
+    # get misfit data at end of each iteration
+    cols = [s for s in results.columns.to_list() if "_final_misfit" in s]
+    iters = len(cols)
+    if inversion_region is not None:
+        misfits = [np.sqrt(utils.rmse(results[results.inside][i])) for i in cols]
+    else:
+        misfits = [np.sqrt(utils.rmse(results[i])) for i in cols]
+    # add starting misfit to the beginning of the list
+    misfits.insert(0, np.sqrt(starting_misfit))
+
+    _fig, ax1 = plt.subplots(figsize=figsize)
+    plt.title("Inversion convergence")
+    ax1.plot(range(iters + 1), misfits, "b-")
+    ax1.set_xlabel("Iteration")
+    ax1.set_ylabel("L2-norm", color="b")
+    ax1.tick_params(axis="y", colors="b", which="both")
+
+    # plot horizontal line of misfit tolerance
+    plt.axhline(
+        y=l2_norm_tolerance,
+        linewidth=1,
+        color="r",
+        linestyle="--",
+        label="L2-norm tolerance",
+    )
+    ax1.set_ylim(0.9 * (l2_norm_tolerance), np.sqrt(starting_misfit))
+
+    ax1.xaxis.set_major_locator(MaxNLocator(integer=True))
+
+    plt.plot(
+        iters,
+        misfits[-1],
+        "s",
+        markersize=10,
+        color=sns.color_palette()[3],
+        label="current L2-norm",
+    )
+    plt.legend(
+        loc="upper right",
+    )
     plt.tight_layout()
+    plt.show()
 
 
 def grid_inversion_results(
     misfits: list[str],
     topos: list[str],
     corrections: list[str],
     prisms_ds: xr.Dataset,
     grav_results: pd.DataFrame,
     region: tuple[float, float, float, float],
-    spacing: float,
-    registration: str,
 ) -> tuple[list[xr.DataArray], list[xr.DataArray], list[xr.DataArray]]:
     """
     create grids from the various data variables of the supplied gravity dataframe and
     prism dataset
 
     Parameters
     ----------
@@ -262,33 +367,23 @@
         list of correction variable names in the prism dataset
     prisms_ds : xr.Dataset
         resulting dataset of prism layer from the inversion
     grav_results : pd.DataFrame
         resulting dataframe of gravity data from the inversion
     region : tuple[float, float, float, float]
         region to use for gridding in format (xmin, xmax, ymin, ymax)
-    spacing : float
-        grid spacing in meters
-    registration : str
-       grid registration type, either "g" for gridline or "p" for pixel
 
     Returns
     -------
     tuple[list[xr.DataArray], list[xr.DataArray], list[xr.DataArray]]
         lists of misfit, topography, and correction grids
     """
     misfit_grids = []
     for m in misfits:
-        grid = pygmt.xyz2grd(
-            data=grav_results[["easting", "northing", m]],
-            region=region,
-            spacing=spacing,
-            registration=registration,
-            verbose="q",
-        )
+        grid = grav_results.set_index(["northing", "easting"]).to_xarray()[m]
         misfit_grids.append(grid)
 
     topo_grids = []
     for t in topos:
         topo_grids.append(
             prisms_ds[t].sel(
                 easting=slice(region[0], region[1]),
@@ -307,24 +402,27 @@
 
     return (misfit_grids, topo_grids, corrections_grids)
 
 
 def plot_inversion_topo_results(
     prisms_ds: xr.Dataset,
     topo_cmap_perc: float = 1,
+    region: tuple[float, float, float, float] | None = None,
 ) -> None:
     """
     plot the initial and final topography grids from the inversion and their difference
 
     Parameters
     ----------
     prisms_ds : xr.Dataset
         dataset resulting from inversion
     topo_cmap_perc : float, optional
         value to multiple min and max values by for colorscale, by default 1
+    region : tuple[float, float, float, float], optional
+        clip grids to this region before plotting
     """
     # Check if matplotlib is installed
     if plt is None:
         msg = "Missing optional dependency 'matplotlib' required for plotting."
         raise ImportError(msg)
 
     initial_topo = prisms_ds.starting_topo
@@ -332,14 +430,24 @@
     # list of variables ending in "_layer"
     topos = [s for s in list(prisms_ds.keys()) if "_layer" in s]
     # list of iterations, e.g. [1,2,3,4]
     its = [int(s[5:][:-6]) for s in topos]
 
     final_topo = prisms_ds[f"iter_{max(its)}_layer"]
 
+    if region is not None:
+        initial_topo = initial_topo.sel(
+            easting=slice(region[0], region[1]),
+            northing=slice(region[2], region[3]),
+        )
+        final_topo = final_topo.sel(
+            easting=slice(region[0], region[1]),
+            northing=slice(region[2], region[3]),
+        )
+
     dif = initial_topo - final_topo
 
     robust = True
 
     topo_lims = []
     for g in [initial_topo, final_topo]:
         topo_lims.append(polar_utils.get_min_max(g))
@@ -410,68 +518,52 @@
 
     fig.tight_layout()
 
 
 def plot_inversion_grav_results(
     grav_results: pd.DataFrame,
     region: tuple[float, float, float, float],
-    spacing: float,
-    registration: str,
     iterations: list[int],
 ) -> None:
     """
     plot the initial and final misfit grids from the inversion and their difference
 
     Parameters
     ----------
     grav_results : pd.DataFrame
         resulting dataframe of gravity data from the inversion
     region : tuple[float, float, float, float]
         region to use for gridding in format (xmin, xmax, ymin, ymax)
-    spacing : float
-        grid spacing in meters
-    registration : str
-        grid registration type, either "g" for gridline or "p" for pixel
     iterations : list[int]
         list of all the iteration numbers
     """
-    initial_misfit = pygmt.xyz2grd(
-        data=grav_results[["easting", "northing", "iter_1_initial_misfit"]],
-        region=region,
-        spacing=spacing,
-        registration=registration,
-        verbose="q",
-    )
 
-    final_misfit = pygmt.xyz2grd(
-        data=grav_results[
-            ["easting", "northing", f"iter_{max(iterations)}_final_misfit"]
-        ],
-        region=region,
-        spacing=spacing,
-        registration=registration,
-        verbose="q",
-    )
+    grid = grav_results.set_index(["northing", "easting"]).to_xarray()
+
+    initial_misfit = grid["iter_1_initial_misfit"]
+    final_misfit = grid[f"iter_{max(iterations)}_final_misfit"]
 
     initial_rmse = utils.rmse(grav_results["iter_1_initial_misfit"])
     final_rmse = utils.rmse(grav_results[f"iter_{max(iterations)}_final_misfit"])
 
     _ = polar_utils.grd_compare(
         initial_misfit,
         final_misfit,
+        region=region,
         plot=True,
         grid1_name=f"Initial misfit: RMSE={round(initial_rmse, 2)} mGal",
         grid2_name=f"Final misfit: RMSE={round(final_rmse, 2)} mGal",
         plot_type="xarray",
         cmap="RdBu_r",
-        robust=False,
+        robust=True,
         hist=True,
         inset=False,
         verbose="q",
         title="difference",
+        diff_maxabs=True,
     )
 
 
 def plot_inversion_iteration_results(
     grids: tuple[list[xr.DataArray], list[xr.DataArray], list[xr.DataArray]],
     grav_results: pd.DataFrame,
     topo_results: pd.DataFrame,
@@ -677,16 +769,14 @@
 
 
 def plot_inversion_results(
     grav_results: pd.DataFrame | str,
     topo_results: pd.DataFrame | str,
     parameters: dict[str, typing.Any] | str,
     grav_region: tuple[float, float, float, float] | None,
-    grav_spacing: float,
-    registration: str = "g",
     iters_to_plot: int | None = None,
     plot_iter_results: bool = True,
     plot_topo_results: bool = True,
     plot_grav_results: bool = True,
     **kwargs: typing.Any,
 ) -> None:
     """
@@ -698,18 +788,14 @@
         gravity results dataframe or filename
     topo_results : pd.DataFrame | str
         topography results dataframe or filename
     parameters : dict[str, typing.Any] | str
         inversion parameters dictionary or filename
     grav_region : tuple[float, float, float, float] | None
         region to use for gridding in format (xmin, xmax, ymin, ymax), by default None
-    grav_spacing : float
-        grid spacing in meters
-    registration : str, optional
-        grid registration type, either "g" for gridline or "p" for pixel, by default "g"
     iters_to_plot : int | None, optional
         number of iterations to plot, including the first and last, by default None
     plot_iter_results : bool, optional
         plot the iteration results, by default True
     plot_topo_results : bool, optional
         plot the topography results, by default True
     plot_grav_results : bool, optional
@@ -769,16 +855,14 @@
     grids = grid_inversion_results(
         misfits,
         topos,
         corrections,
         prisms_ds,
         grav_results,
         grav_region,
-        grav_spacing,
-        registration,
     )
 
     if plot_iter_results is True:
         plot_inversion_iteration_results(
             grids,
             grav_results,
             topo_results,
@@ -789,22 +873,21 @@
             corrections_cmap_perc=kwargs.get("corrections_cmap_perc", 1),
         )
 
     if plot_topo_results is True:
         plot_inversion_topo_results(
             prisms_ds,
             topo_cmap_perc=kwargs.get("topo_cmap_perc", 1),
+            region=grav_region,
         )
 
     if plot_grav_results is True:
         plot_inversion_grav_results(
             grav_results,
             grav_region,
-            grav_spacing,
-            registration,
             iterations,
         )
 
 
 def add_light(
     plotter: pyvista.Plotter,
     prisms: xr.Dataset,
```

### Comparing `invert4geom-0.4.0/src/invert4geom/regional.py` & `invert4geom-0.5.0/src/invert4geom/regional.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,69 @@
 import verde as vd
 import xarray as xr
 from nptyping import NDArray
 
 from invert4geom import optimization, utils
 
 
+def regional_dc_shift(
+    grav_df: pd.DataFrame,
+    dc_shift: float | None = None,
+    grav_grid: xr.DataArray | None = None,
+    constraint_points: pd.DataFrame | None = None,
+    coord_names: tuple[str, str] = ("easting", "northing"),
+    regional_col_name: str = "reg",
+) -> pd.DataFrame:
+    """
+    separate the regional field by applying a constant shift (DC-shift) to the gravity
+    data. If constraint points of the layer of interested are supplied, the DC shift
+    will minimize the residual misfit at these constraint points.
+
+    Parameters
+    ----------
+    grav_df : pd.DataFrame
+        gravity data with columns defined by coord_names and input_grav_name.
+    dc_shift : float
+        shift to apply to the data
+    grav_grid : xr.DataArray
+        gridded gravity misfit data
+    constraint_points : pd.DataFrame
+        a dataframe of constraint points with columns X and Y columns defined by the
+        coord_names parameter.
+    coord_names : tuple
+        names of the X and Y column names in constraint points dataframe
+    regional_col_name : str
+        name for the new column in grav_df for the regional field.
+
+    Returns
+    -------
+    pd.DataFrame
+        grav_df with new regional column
+    """
+    if constraint_points is not None:
+        # get the gravity values at the constraint points
+        constraints_df = constraint_points.copy()
+
+        # sample gravity at constraint points
+        constraints_df = utils.sample_grids(
+            df=constraints_df,
+            grid=grav_grid,
+            sampled_name="sampled_grav",
+            coord_names=coord_names,
+        )
+
+        # use RMS of sampled value for DC shift
+        dc_shift = utils.rmse(constraints_df.sampled_grav)
+
+    grav_df[regional_col_name] = dc_shift
+
+    # return the new dataframe
+    return grav_df
+
+
 def regional_filter(
     filter_width: float,
     grav_grid: xr.DataArray,
     grav_df: pd.DataFrame,
     regional_col_name: str = "reg",
 ) -> pd.DataFrame:
     """
```

### Comparing `invert4geom-0.4.0/src/invert4geom/synthetic.py` & `invert4geom-0.5.0/src/invert4geom/synthetic.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,26 +56,32 @@
     return np.exp(-(a * xhat**2 + 2.0 * b * xhat * yhat + c * yhat**2))
 
 
 def synthetic_topography_simple(
     spacing: float,
     region: tuple[float, float, float, float],
     registration: str = "g",
+    scale: float = 1,
+    yoffset: float = 0,
 ) -> xr.Dataset:
     """
     Create a synthetic topography dataset with a few features.
 
     Parameters
     ----------
     spacing : float
         grid spacing in meters
     region : tuple[float, float, float, float]
         bounding edges of the grid in meters in format (xmin, xmax, ymin, ymax)
     registration : str, optional
         grid registration type, either "g" for gridline or "p" for pixel, by default "g"
+    scale : float, optional
+        value to scale the topography by, by default 1
+    yoffset : float, optional
+        value to offset the topography by, by default 0
 
     Returns
     -------
     xr.Dataset
         synthetic topography dataset
     """
     if registration == "g":
@@ -165,15 +171,19 @@
         f3,
         f4,
         f5,
     ]
 
     topo = sum(features)
 
-    topo = topo + 1200
+    topo += 1200
+
+    topo = topo * scale
+
+    topo += yoffset
 
     return vd.make_xarray_grid(
         (x, y),
         topo,
         data_names="upward",
         dims=("northing", "easting"),
     ).upward
```

### Comparing `invert4geom-0.4.0/src/invert4geom/utils.py` & `invert4geom-0.5.0/src/invert4geom/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -580,26 +580,27 @@
         number_enforced = 0
         for i, j in enumerate(df[f"iter_{iteration_number}_correction"]):
             if j < df.max_change_below[i]:
                 number_enforced += 1
                 df.loc[i, f"iter_{iteration_number}_correction"] = df.max_change_below[
                     i
                 ]
+
         logging.info("enforced lower confining surface at %s prisms", number_enforced)
 
     # check that when constrained correction is added to topo it doesn't intersect
     # either bounding layer
     updated_topo: pd.Series[float] = df[f"iter_{iteration_number}_correction"] + df.topo
-    if "upper_bounds" in df and np.any((df.upper_bounds - updated_topo) < 0):
+    if "upper_bounds" in df and np.any((df.upper_bounds - updated_topo) < -0.001):
         msg = (
             "Constraining didn't work and updated topography intersects upper "
             "constraining surface"
         )
         raise ValueError(msg)
-    if "lower_bounds" in df and np.any((updated_topo - df.lower_bounds) < 0):
+    if "lower_bounds" in df and np.any((updated_topo - df.lower_bounds) < -0.001):
         msg = (
             "Constraining didn't work and updated topography intersects lower "
             "constraining surface"
         )
         raise ValueError(msg)
     return df
```

### Comparing `invert4geom-0.4.0/src/invert4geom.egg-info/PKG-INFO` & `invert4geom-0.5.0/src/invert4geom.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invert4geom
-Version: 0.4.0
+Version: 0.5.0
 Summary: Constrained gravity inversion to recover the geometry of a density contrast.
 Author-email: Matt Tankersley <matt.d.tankersley@gmail.com>
 License: Copyright 2023 Matt Tankersley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
@@ -60,24 +60,26 @@
 Requires-Dist: nptyping
 Requires-Dist: numba_progress
 Requires-Dist: tqdm
 Requires-Dist: pygmt
 Requires-Dist: dask
 Provides-Extra: opti
 Requires-Dist: optuna>=3.1.0; extra == "opti"
+Requires-Dist: optuna-integration; extra == "opti"
 Requires-Dist: botorch>=0.4.0; extra == "opti"
 Requires-Dist: joblib; extra == "opti"
 Requires-Dist: psutil; extra == "opti"
 Requires-Dist: tqdm_joblib; extra == "opti"
 Provides-Extra: viz
 Requires-Dist: pyvista; extra == "viz"
 Requires-Dist: trame; extra == "viz"
 Requires-Dist: ipywidgets; extra == "viz"
 Requires-Dist: matplotlib; extra == "viz"
 Requires-Dist: seaborn; extra == "viz"
+Requires-Dist: ipython; extra == "viz"
 Provides-Extra: test
 Requires-Dist: pytest>=6; extra == "test"
 Requires-Dist: pytest-cov>=3; extra == "test"
 Requires-Dist: invert4geom[opti]; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx>=4.0; extra == "docs"
 Requires-Dist: myst_parser; extra == "docs"
```

### Comparing `invert4geom-0.4.0/src/invert4geom.egg-info/SOURCES.txt` & `invert4geom-0.5.0/src/invert4geom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invert4geom-0.4.0/src/invert4geom.egg-info/requires.txt` & `invert4geom-0.5.0/src/invert4geom.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 sphinx_design
 nbsphinx
 nbconvert
 sphinxcontrib-bibtex
 
 [opti]
 optuna>=3.1.0
+optuna-integration
 botorch>=0.4.0
 joblib
 psutil
 tqdm_joblib
 
 [test]
 pytest>=6
@@ -55,7 +56,8 @@
 
 [viz]
 pyvista
 trame
 ipywidgets
 matplotlib
 seaborn
+ipython
```

### Comparing `invert4geom-0.4.0/tests/test_inversion.py` & `invert4geom-0.5.0/tests/test_inversion.py`

 * *Files identical despite different names*

### Comparing `invert4geom-0.4.0/tests/test_optimization.py` & `invert4geom-0.5.0/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `invert4geom-0.4.0/tests/test_regional.py` & `invert4geom-0.5.0/tests/test_regional.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import numpy as np
 import pandas as pd
 import pytest
 import verde as vd
 import xarray as xr
 
-from invert4geom import regional
+from invert4geom import regional, synthetic
 
 # %%
 
 
 def dummy_grid() -> xr.DataArray:
     (x, y, z) = vd.grid_coordinates(
         region=[0, 200, 200, 400],
@@ -35,14 +35,60 @@
 def dummy_df() -> pd.DataFrame:
     df = dummy_grid().to_dataframe().reset_index()
     df["grav"] = 20000
     return df
 
 
 # %%
+def test_regional_dc_shift_constraints():
+    """
+    test the regional_dc_shift function with a supplied constraints
+    """
+    grav_df = dummy_df()
+    region = (0, 200, 200, 400)
+
+    # create 10 random point within the region
+    num_constraints = 10
+    coords = vd.scatter_points(region=region, size=num_constraints, random_state=0)
+    points = pd.DataFrame(data={"easting": coords[0], "northing": coords[1]})
+
+    # print(grav_df.describe())
+
+    df = regional.regional_dc_shift(
+        grav_df=grav_df,
+        grav_grid=dummy_grid().misfit,
+        constraint_points=points,
+        regional_col_name="reg",
+    )
+
+    # print(df.describe())
+
+    # test whether regional field has been removed correctly
+    # by whether the means of the reg and misfit are similar
+    # print(np.mean(df.reg), np.mean(df.misfit))
+    print(np.mean(df.reg), np.mean(df.misfit))
+    assert np.mean(df.reg) == pytest.approx(np.mean(df.misfit), rel=1000)
+
+
+def test_regional_dc_shift():
+    """
+    test the regional_dc_shift function with a supplied DC shift
+    """
+
+    grav_df = dummy_grid().to_dataframe().reset_index()
+
+    df = regional.regional_dc_shift(
+        grav_df=grav_df,
+        dc_shift=-200,
+        regional_col_name="reg",
+    )
+
+    assert df.reg.mean() == -200
+
+
 @pytest.mark.parametrize("fill_method", ["rioxarray", "verde"])
 @pytest.mark.parametrize("trend", [0, 2])
 def test_regional_trend(fill_method, trend):
     """
     test the regional_trend function
     """
     anomalies = dummy_df()
@@ -118,14 +164,22 @@
     test the regional_eq_sources function
     """
     # grav_df = dummy_df()
     # grav_df["Gobs"] = np.random.normal(100, 100, len(grav_df))
 
     grav_df = dummy_grid().to_dataframe().reset_index()
 
+    # add noise
+    grav_df["misfit"], _ = synthetic.contaminate(
+        grav_df["misfit"],
+        stddev=0.2,
+        percent=True,
+        seed=0,
+    )
+
     df = regional.regional_eq_sources(
         source_depth=100e3,
         grav_df=grav_df,
         input_grav_name="misfit",
     )
     # print(df)
     reg_range = np.max(df.reg) - np.min(df.reg)
```

### Comparing `invert4geom-0.4.0/tests/test_utils.py` & `invert4geom-0.5.0/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,31 +410,43 @@
     Test if the sampled column contains valid values at grid nodes.
     """
     grid = dummy_grid().scalars
     name = "sampled_data"
     df = pd.DataFrame({"x": [0, 100, 200], "y": [200, 300, 400]})
     result_df = utils.sample_grids(df, grid, sampled_name=name)
     expected = pd.DataFrame(
-        {"x": [0, 100, 200], "y": [200, 300, 400], name: [40000, 100000, 200000]}
+        {
+            "x": [0, 100, 200],
+            "y": [200, 300, 400],
+            name: [40000, 100000, 200000],
+        },
+    )
+    pdt.assert_frame_equal(
+        result_df,
+        expected,
+        check_dtype=False,
     )
-    pdt.assert_frame_equal(result_df, expected)
 
 
 def test_sample_grids_off_nodes():
     """
     Test if the sampled column contains valid values not on grid nodes.
     """
     grid = dummy_grid().scalars
     name = "sampled_data"
     df = pd.DataFrame({"x": [50, 101], "y": [280, 355]})
     result_df = utils.sample_grids(df, grid, sampled_name=name)
     expected = pd.DataFrame(
         {"x": [50, 101], "y": [280, 355], name: [83790.0, 138949.640109]}
     )
-    pdt.assert_frame_equal(result_df, expected)
+    pdt.assert_frame_equal(
+        result_df,
+        expected,
+        check_dtype=False,
+    )
 
 
 def test_sample_grids_custom_coordinate_names():
     """
     Test if the function handles custom coordinate names correctly.
     """
     grid = dummy_grid().scalars
@@ -444,17 +456,22 @@
     with pytest.raises(KeyError):
         utils.sample_grids(df, grid, sampled_name=name)
     # check function works if coordinate names are provided
     result_df = utils.sample_grids(
         df, grid, sampled_name=name, coord_names=("lon", "lat")
     )
     expected = pd.DataFrame(
-        {"lon": [0, 100, 200], "lat": [200, 300, 400], name: [40000, 100000, 200000]}
+        {"lon": [0, 100, 200], "lat": [200, 300, 400], name: [40000, 100000, 200000]},
+        dtype="int64",
+    )
+    pdt.assert_frame_equal(
+        result_df,
+        expected,
+        check_dtype=False,
     )
-    pdt.assert_frame_equal(result_df, expected)
 
 
 def test_sample_grids_one_out_of_grid_coordinates():
     """
     Test if the function handles out-of-grid coordinates gracefully by setting NaN
     values.
     """
```

