# Comparing `tmp/asteca-0.5.1.tar.gz` & `tmp/asteca-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asteca-0.5.1.tar", max compression
+gzip compressed data, was "asteca-0.5.2.tar", max compression
```

## Comparing `asteca-0.5.1.tar` & `asteca-0.5.2.tar`

### file list

```diff
@@ -1,23 +1,15 @@
--rw-r--r--   0        0        0     1071 2024-04-18 20:24:11.112496 asteca-0.5.1/LICENSE.txt
--rw-r--r--   0        0        0     1140 2024-04-18 20:24:11.112496 asteca-0.5.1/README.md
--rw-r--r--   0        0        0     1041 2024-04-18 20:24:11.112496 asteca-0.5.1/asteca/__init__.py
--rw-r--r--   0        0        0     5166 2024-04-18 20:24:11.116496 asteca-0.5.1/asteca/cluster.py
--rw-r--r--   0        0        0     4508 2024-04-18 20:24:11.116496 asteca-0.5.1/asteca/isochrones.py
--rw-r--r--   0        0        0     3087 2024-04-18 20:24:11.116496 asteca-0.5.1/asteca/likelihood.py
--rw-r--r--   0        0        0        0 2024-04-18 20:24:11.116496 asteca-0.5.1/asteca/modules/__init__.py
--rw-r--r--   0        0        0      161 2024-04-16 20:21:22.225585 asteca-0.5.1/asteca/modules/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      177 2024-04-19 12:46:23.026098 asteca-0.5.1/asteca/modules/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4667 2024-04-19 12:46:23.038098 asteca-0.5.1/asteca/modules/__pycache__/imfs.cpython-311.pyc
--rw-r--r--   0        0        0    10871 2024-04-16 20:21:22.229585 asteca-0.5.1/asteca/modules/__pycache__/isochrones_priv.cpython-310.pyc
--rw-r--r--   0        0        0    23066 2024-04-19 13:28:25.993751 asteca-0.5.1/asteca/modules/__pycache__/isochrones_priv.cpython-311.pyc
--rw-r--r--   0        0        0    10791 2024-04-19 12:46:23.726118 asteca-0.5.1/asteca/modules/__pycache__/likelihood_priv.cpython-311.pyc
--rw-r--r--   0        0        0     9732 2024-04-19 12:46:23.042098 asteca-0.5.1/asteca/modules/__pycache__/mass_binary.cpython-311.pyc
--rw-r--r--   0        0        0    31637 2024-04-19 12:46:23.038098 asteca-0.5.1/asteca/modules/__pycache__/synth_cluster_priv.cpython-311.pyc
--rw-r--r--   0        0        0     3725 2024-04-18 20:24:11.116496 asteca-0.5.1/asteca/modules/imfs.py
--rw-r--r--   0        0        0    18065 2024-04-19 14:21:03.385995 asteca-0.5.1/asteca/modules/isochrones_priv.py
--rw-r--r--   0        0        0     9947 2024-04-18 20:24:11.116496 asteca-0.5.1/asteca/modules/likelihood_priv.py
--rw-r--r--   0        0        0     7845 2024-04-18 20:24:11.116496 asteca-0.5.1/asteca/modules/mass_binary.py
--rw-r--r--   0        0        0    32525 2024-04-18 20:24:11.116496 asteca-0.5.1/asteca/modules/synth_cluster_priv.py
--rw-r--r--   0        0        0    17910 2024-04-18 20:24:11.116496 asteca-0.5.1/asteca/synthetic.py
--rw-r--r--   0        0        0      617 2024-04-19 14:23:44.925857 asteca-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1959 1970-01-01 00:00:00.000000 asteca-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-18 20:24:11.112496 asteca-0.5.2/LICENSE.txt
+-rw-r--r--   0        0        0     1140 2024-04-18 20:24:11.112496 asteca-0.5.2/README.md
+-rw-r--r--   0        0        0     1093 2024-05-05 14:37:26.025497 asteca-0.5.2/asteca/__init__.py
+-rw-r--r--   0        0        0     5978 2024-05-06 15:23:31.088325 asteca-0.5.2/asteca/cluster.py
+-rw-r--r--   0        0        0     6814 2024-05-06 20:00:05.721149 asteca-0.5.2/asteca/isochrones.py
+-rw-r--r--   0        0        0     3088 2024-05-05 14:39:38.802627 asteca-0.5.2/asteca/likelihood.py
+-rw-r--r--   0        0        0        0 2024-04-18 20:24:11.116496 asteca-0.5.2/asteca/modules/__init__.py
+-rw-r--r--   0        0        0     3727 2024-05-05 14:39:38.878630 asteca-0.5.2/asteca/modules/imfs.py
+-rw-r--r--   0        0        0    12359 2024-05-06 12:12:01.145323 asteca-0.5.2/asteca/modules/isochrones_priv.py
+-rw-r--r--   0        0        0    10054 2024-05-05 14:39:39.214643 asteca-0.5.2/asteca/modules/likelihood_priv.py
+-rw-r--r--   0        0        0     7833 2024-05-05 14:39:39.054636 asteca-0.5.2/asteca/modules/mass_binary.py
+-rw-r--r--   0        0        0    35104 2024-05-06 20:09:09.279994 asteca-0.5.2/asteca/modules/synth_cluster_priv.py
+-rw-r--r--   0        0        0    19706 2024-05-06 20:21:49.518241 asteca-0.5.2/asteca/synthetic.py
+-rw-r--r--   0        0        0      617 2024-05-07 19:21:12.421026 asteca-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2010 1970-01-01 00:00:00.000000 asteca-0.5.2/PKG-INFO
```

### Comparing `asteca-0.5.1/LICENSE.txt` & `asteca-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `asteca-0.5.1/README.md` & `asteca-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `asteca-0.5.1/asteca/__init__.py` & `asteca-0.5.2/asteca/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from .isochrones import isochrones
-from .synthetic import synthetic
-from .cluster import cluster
-from .likelihood import likelihood
+from .isochrones import isochrones as isochrones
+from .synthetic import synthetic as synthetic
+from .cluster import cluster as cluster
+from .likelihood import likelihood as likelihood
 
 from contextlib import suppress
 import importlib.metadata
 from pathlib import Path
 
 
 def extract_version() -> str:
```

### Comparing `asteca-0.5.1/asteca/cluster.py` & `asteca-0.5.2/asteca/cluster.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 @dataclass
 class cluster:
     r"""Define a ``cluster`` object.
 
     Parameters
     ----------
     cluster_df : pd.DataFrame
-        pandas DataFrame with the cluster's loaded data
+        `pandas DataFrame <https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html>`_
+        with the cluster's loaded data
     magnitude : str
         Name of the DataFrame column that contains the magnitude
     e_mag : str
         Name of the DataFrame column that contains the magnitude's uncertainty
     color : str
         Name of the DataFrame column that contains the color
     e_color : str
@@ -33,14 +34,15 @@
         Name of the DataFrame column that contains the DEC proper motion
     color2: str, optional, default=None
         Name of the DataFrame column that contains the second color
     e_color2: str, optional, default=None
         Name of the DataFrame column that contains the second color's uncertainty
 
     """
+
     cluster_df: pd.DataFrame
     magnitude: str
     e_mag: str
     color: str
     e_color: str
     ra: Optional[str] = None
     dec: Optional[str] = None
@@ -55,15 +57,15 @@
         self._load()
 
     def _load(self):
         """
         The photometry is store with a '_p' to differentiate from the self.magnitude,
         self.color, etc that are defined with the class is called.
         """
-        print("Reading and processing cluster data")
+        print("Instantiating cluster...")
 
         self.mag_p = np.array(self.cluster_df[self.magnitude])
         self.e_mag_p = np.array(self.cluster_df[self.e_mag])
 
         self.colors_p = [np.array(self.cluster_df[self.color])]
         if self.color2 is not None:
             self.colors_p.append(np.array(self.cluster_df[self.color2]))
@@ -71,14 +73,19 @@
         if self.e_color2 is not None:
             self.e_colors_p.append(np.array(self.cluster_df[self.e_color2]))
 
         if self.ra is not None:
             self.ra_v = self.cluster_df[self.ra]
             self.dec_v = self.cluster_df[self.dec]
 
+        print(f"N_stars        : {len(self.mag_p)}")
+        print(f"Magnitude      : {self.magnitude}")
+        print(f"Color          : {self.color}")
+        if self.color2 is not None:
+            print(f"Color2         : {self.color2}")
         print("Cluster object generated\n")
 
     def radecplot(self):
         r"""Generate a (RA, DEC) plot.
 
         Returns
         -------
@@ -106,63 +113,73 @@
         plt.scatter(ra, dec, s=sizes, c="k", alpha=0.7)
         plt.xlabel("RA")
         plt.ylabel("DEC")
         plt.gca().invert_xaxis()
 
         return ax
 
-    def clustplot(self, ax=None, binar_prob=None):
+    def clustplot(self, ax, color_idx=0, binar_probs=None):
         r"""Generate a color-magnitude plot.
 
         Parameters
         ----------
         ax : matplotlib.axis, optional, default=None
             Matplotlib axis where to draw the plot
-        binar_prob : numpy.array, optional, default=None
+        color_idx : int, default=0
+            Index of the color to plot. If ``0`` (default), plot the first color. If
+            ``1`` plot the second color.
+        binar_probs : numpy.array, optional, default=None
             Array with probabilities of being a binary system for each observed star
 
         Returns
         -------
         matplotlib.axis
             Matplotlib axis object
 
-
         """
-        if ax is None:
-            f, ax = plt.subplots()
+        if color_idx > 1:
+            raise ValueError(
+                f"Wrong 'color_idx' value ({color_idx}), should be one of: [0, 1]"
+            )
 
-        if binar_prob is not None:
-            msk_binar = binar_prob > 0.5
+        if binar_probs is not None:
+            msk_binar = binar_probs > 0.5
 
         mag_col = self.magnitude
         col_col = self.color
+        if color_idx == 1:
+            col_col = self.color2
 
-        if binar_prob is None:
+        if binar_probs is None:
             ax.scatter(
-                self.colors_p[0],
+                self.colors_p[color_idx],
                 self.mag_p,
                 c="green",
                 alpha=0.5,
                 label=f"Observed, N={len(self.mag_p)}",
             )
         else:
             ax.scatter(
-                self.colors_p[0][~msk_binar],
+                self.colors_p[color_idx][~msk_binar],
                 self.mag_p[~msk_binar],
-                c="green",
+                # c="green",
+                c=binar_probs[~msk_binar],
+                marker="o",
                 alpha=0.5,
                 label=f"Observed (single), N={len(self.mag_p[~msk_binar])}",
             )
             ax.scatter(
-                self.colors_p[0][msk_binar],
+                self.colors_p[color_idx][msk_binar],
                 self.mag_p[msk_binar],
-                c="red",
+                # c="red",
+                c=binar_probs[msk_binar],
+                marker="s",
                 alpha=0.5,
                 label=f"Observed (binary), N={len(self.mag_p[msk_binar])}",
             )
 
-        ax.set_ylim(max(self.mag_p) + .5, min(self.mag_p) - .5)
+        ax.set_ylim(max(self.mag_p) + 0.5, min(self.mag_p) - 0.5)
         ax.set_xlabel(col_col)
         ax.set_ylabel(mag_col)
         ax.legend()
 
         return ax
```

### Comparing `asteca-0.5.1/asteca/likelihood.py` & `asteca-0.5.2/asteca/likelihood.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         Bin method used to split the color-magnitude diagram into cells
         (`Hess diagram <https://en.wikipedia.org/wiki/Hess_diagram>`_). If ``manual``
         is selected, a list containing an array of edge values for the magnitude,
         followed by one or two arrays (depending on the number of colors defined) for
         the color(s), also with edge values.
 
     """
+
     my_cluster: cluster
     lkl_name: str = "plr"
     bin_method: str = "knuth"
 
     def __post_init__(self):
         likelihoods = ("plr", "bins_distance")
         if self.lkl_name not in likelihoods:
```

### Comparing `asteca-0.5.1/asteca/modules/imfs.py` & `asteca-0.5.2/asteca/modules/imfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     Sample the inverse CDF up to `Max_mass`
     """
 
     def sampled_inv_cdf(ijkseed, N):
         # mr = np.random.rand(N)
         # The internal seed can not be 'self.seed' because otherwise all the
         # floats returned are equal
-        mr = np.random.default_rng(ijkseed).uniform(0., 1., N)
+        mr = np.random.default_rng(ijkseed).uniform(0.0, 1.0, N)
         return inv_cdf(mr)
 
     # Sample in chunks until the maximum defined mass is reached.
     N_chunk = max(100, int(2.5 * Max_mass / 100.0))
     k, Mass_tot, mass_samples = 0, 0, []
     int_seed = np.random.default_rng(ijseed).integers(1)
     while Mass_tot < Max_mass:
```

### Comparing `asteca-0.5.1/asteca/modules/likelihood_priv.py` & `asteca-0.5.2/asteca/modules/likelihood_priv.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,19 +11,24 @@
         self.bin_method, self.my_cluster.mag_p, self.my_cluster.colors_p
     )
 
     # Obtain histogram for observed cluster.
     hess_diag = []
     for i, col in enumerate(self.my_cluster.colors_p):
         # Fast 2D histogram
-        hess_diag = histogram2d(
-            self.my_cluster.mag_p,
-            col,
-            range=[[ranges[0][0], ranges[0][1]], [ranges[i + 1][0], ranges[i + 1][1]]],
-            bins=[Nbins[0], Nbins[i + 1]],
+        hess_diag.append(
+            histogram2d(
+                self.my_cluster.mag_p,
+                col,
+                range=[
+                    [ranges[0][0], ranges[0][1]],
+                    [ranges[i + 1][0], ranges[i + 1][1]],
+                ],
+                bins=[Nbins[0], Nbins[i + 1]],
+            )
         )
 
     # Flatten array
     cl_histo_f = []
     for i, diag in enumerate(hess_diag):
         cl_histo_f += list(np.array(diag).ravel())
     cl_histo_f = np.array(cl_histo_f)
```

### Comparing `asteca-0.5.1/asteca/modules/mass_binary.py` & `asteca-0.5.2/asteca/modules/mass_binary.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,17 @@
     Generate the 'N_models' models via sampling a Gaussian centered on 'fit_params',
     with standard deviation given by 'model_std'.
     """
     models_ran, int_seed = {}, np.random.default_rng(seed).integers(1)
     for k, f_val in fit_params.items():
         std = model_std[k]
         # models_ran[k] = np.random.normal(f_val, std, N_models)
-        models_ran[k] = np.random.default_rng(seed + int_seed).normal(f_val, std, N_models)
+        models_ran[k] = np.random.default_rng(seed + int_seed).normal(
+            f_val, std, N_models
+        )
         int_seed += 1
     # Transpose dict of arrays into list of dicts
     ran_models = [dict(zip(models_ran, t)) for t in zip(*models_ran.values())]
 
     return ran_models
 
 
@@ -196,18 +198,15 @@
     # Miyamoto & Nagai potential (disk)
     # https://galaxiesbook.org/chapters/II-01.-Flattened-Mass-Distributions.html#Thickened-disk:-the-Miyamoto-Nagai-model
     # https://articles.adsabs.harvard.edu/pdf/1975PASJ...27..533M
     # https://www.astro.utu.fi/~cflynn/galdyn/lecture4.html
     numerator = (
         M_D
         * b**2
-        * (
-            a * r**2
-            + (a + 3 * np.sqrt(z**2 + b**2)) * (a + np.sqrt(z**2 + b**2)) ** 2
-        )
+        * (a * r**2 + (a + 3 * np.sqrt(z**2 + b**2)) * (a + np.sqrt(z**2 + b**2)) ** 2)
     )
     denominator = (b**2 + z**2) ** (3 / 2) * (
         r**2 + (a + np.sqrt(b**2 + z**2)) ** 2
     ) ** (5 / 2)
     Phi_D_laplacian = numerator / denominator
 
     # Sanderson potential (dark matter halo)
```

### Comparing `asteca-0.5.1/asteca/modules/synth_cluster_priv.py` & `asteca-0.5.2/asteca/modules/synth_cluster_priv.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,18 +141,20 @@
     If binarity is processed:
         N_cols: magnitude + color(s) + initial masses + unresolved mag +
             unresolved color(s) + secondary masses
     else:
         N_cols: magnitude + colors + initial mass
 
     """
-    print("Generating binary data")
+    all_colors = [self.isochs.color]
+    if self.isochs.color2 is not None:
+        all_colors.append(self.isochs.color2)
+    N_colors = len(all_colors)
 
     mag_idx = 0
-    N_colors = len(self.isochs.color_filter_name)
     m_ini_idx = mag_idx + N_colors + 1
 
     # Extend to accommodate binary data
     Nz, Na, Nd, Ni = self.isochs.theor_tracks.shape
     theor_tracks = np.concatenate(
         (self.isochs.theor_tracks, np.zeros([Nz, Na, Nd, Ni])), axis=2
     )
@@ -171,57 +173,117 @@
 
             # Calculate unresolved binary magnitude
             mag = isoch[mag_idx]
             mag_m2 = np.interp(m2, mass_ini, mag)
             theor_tracks[mx][ax][m_ini_idx + 1] = mag_combine(mag, mag_m2)
 
             # Calculate unresolved color for each color defined.
-            for ic, color in enumerate(self.isochs.color_filter_name):
+            for ic, color in enumerate(all_colors):
                 mc1 = self.isochs.color_filters[mx][ax][color[0]]
                 mc2 = self.isochs.color_filters[mx][ax][color[1]]
                 f_m1 = np.interp(m2, mass_ini, mc1)
                 f1 = mag_combine(mc1, f_m1)
                 f_m2 = np.interp(m2, mass_ini, mc2)
                 f2 = mag_combine(mc2, f_m2)
                 theor_tracks[mx][ax][m_ini_idx + 1 + 1 + ic] = f1 - f2
 
             # Secondary masses
             theor_tracks[mx][ax][-1] = m2
 
     return theor_tracks
 
 
-def extinction_coeffs(self) -> list:
+def ccmo_ext_coeffs(self) -> list:
     """Obtain extinction coefficients for all the observed filters and colors,
     in the order in which they are stored in theor_tracks.
 
     ext_coefs = [ec_mag, ec_col1, ...]
 
     """
-    print("Obtaining extinction coefficients")
-
-    # For the magnitude.
-    # Effective wavelength in Armstrong.
-    eff_wave = self.isochs.mag_color_lambdas[self.isochs.mag_filter_name]
-    # CCM coefficient. Effective wavelength in inverse microns.
-    ext_coefs = [ccm_model(10000.0 / eff_wave)]
-
-    # For colors.
-    for color in self.isochs.color_filter_name:
-        c_filt1, c_filt2 = color
+    ext_coefs = [[], []]
+    if self.ext_law != "GAIADR3":
+        # For the magnitude.
         # Effective wavelength in Armstrong.
-        eff_wave1 = self.isochs.mag_color_lambdas[c_filt1]
-        eff_wave2 = self.isochs.mag_color_lambdas[c_filt2]
-        ext_coefs.append(
-            [ccm_model(10000.0 / eff_wave1), ccm_model(10000.0 / eff_wave2)]
-        )
+        eff_wave = self.isochs.magnitude_effl
+        # Effective wavelength in inverse microns.
+        ext_coefs[0] = ccmo_model(10000.0 / eff_wave)
+
+        # For colors.
+        eff_wave1, eff_wave2 = self.isochs.color_effl
+        ext_coefs[1] = [ccmo_model(10000.0 / eff_wave1), ccmo_model(10000.0 / eff_wave2)]
+
+    if self.isochs.color2_effl is not None:
+        eff_wave1, eff_wave2 = self.isochs.color2_effl
+        ext_coefs += [[ccmo_model(10000.0 / eff_wave1), ccmo_model(10000.0 / eff_wave2)]]
 
     return ext_coefs
 
 
+def ccmo_model(mw: float) -> list:
+    """Cardelli, Clayton, and Mathis (1989 ApJ. 345, 245) model for extinction
+    coefficients with updated coefficients for near-UV from O'Donnell
+    (1994, ApJ, 422, 158).
+
+    ccm_coef = a + b / Rv
+
+    Implementation taken from:
+
+    http://idlastro.gsfc.nasa.gov/ftp/pro/astro/ccm_unred.pro
+
+    There appears to be an error in the Far-UV range in the original IDL
+    routine where the maximum inverse wavelength is 11 and it should be 10
+    according to Cardelli et al. 1989 (pag 251, Eq (5,a,b)).
+
+    """
+
+    if 0.3 <= mw < 1.1:
+        # Infrared.
+        a, b = 0.574 * (mw**1.61), -0.527 * (mw**1.61)
+
+    elif 1.1 <= mw < 3.3:
+        # Optical/NIR.
+        # Original coefficients from CCM89
+        # c1 = [1., 0.17699, -0.50447, -0.02427, 0.72085, 0.01979, -0.77530,
+        #       0.32999]
+        # c2 = [0., 1.41338, 2.28305, 1.07233, -5.38434, -0.62251, 5.30260,
+        #       -2.09002]
+        # New coefficients from O'Donnell (1994)
+        c1 = [1.0, 0.104, -0.609, 0.701, 1.137, -1.718, -0.827, 1.647, -0.505]
+        c2 = [0.0, 1.952, 2.908, -3.989, -7.985, 11.102, 5.491, -10.805, 3.347]
+        y = mw - 1.82
+        # Reverse because polyval starts from the highest degree.
+        c1.reverse(), c2.reverse()
+        a, b = np.polyval(c1, y), np.polyval(c2, y)
+
+    elif 3.3 <= mw < 8.0:
+        # Mid-UV
+        F_a, F_b = 0.0, 0.0
+        if mw >= 5.9:
+            y = mw - 5.9
+            F_a = -0.04473 * y**2 - 0.009779 * y**3
+            F_b = 0.2130 * y**2 + 0.1207 * y**3
+        a = 1.752 - 0.316 * mw - (0.104 / ((mw - 4.67) ** 2 + 0.341)) + F_a
+        b = -3.090 + 1.825 * mw + (1.206 / ((mw - 4.62) ** 2 + 0.263)) + F_b
+
+    elif 8.0 <= mw <= 10.0:
+        # Far-UV
+        c1 = [-1.073, -0.628, 0.137, -0.070]
+        c2 = [13.670, 4.257, -0.420, 0.374]
+        y = mw - 8.0
+        c1.reverse(), c2.reverse()
+        a, b = np.polyval(c1, y), np.polyval(c2, y)
+    else:
+        raise ValueError(
+            "The effective wavelength is {} [1/micron], beyond "
+            "the CCM model limit (10 [1/micron]).".format(mw)
+        )
+
+    return a, b
+
+
 def sample_imf(self, Nmets: int, Nages: int) -> list:
     """Returns the number of stars per interval of mass for the selected IMF.
 
     Parameters
     ----------
     IMF_name : str
       Name of the IMF to be used.
@@ -234,22 +296,21 @@
       Tuple that contains: a given number of stars sampled from the selected
       IMF, that (approximately) sum to the associated total mass; the
       cumulative sum of those masses.
       One list per metallicity and age values defined is returned. This is to add some
       variety to the sampled IMF.
 
     """
-    print(f"Sampling selected IMF ({self.IMF_name})")
     inv_cdf = invTrnsfSmpl(self.IMF_name)
 
     st_dist_mass = []
     for i in range(Nmets):
         met_lst = []
         for j in range(Nages):
-            sampled_IMF = sampleInv(i+j + self.seed, self.max_mass, inv_cdf)
+            sampled_IMF = sampleInv(i + j + self.seed, self.max_mass, inv_cdf)
             met_lst.append(sampled_IMF)
         st_dist_mass.append(met_lst)
 
     return st_dist_mass
 
 
 def randVals(self) -> dict:
@@ -385,76 +446,14 @@
 
     """
     c = 10**-0.4
     mbin = -2.5 * (-0.4 * m1 + np.log10(1.0 + c ** (m2 - m1)))
     return mbin
 
 
-def ccm_model(mw: float) -> list:
-    """Cardelli, Clayton, and Mathis (1989 ApJ. 345, 245) model for extinction
-    coefficients with updated coefficients for near-UV from O'Donnell
-    (1994, ApJ, 422, 158).
-
-    ccm_coef = a + b / Rv
-
-    Implementation taken from:
-
-    http://idlastro.gsfc.nasa.gov/ftp/pro/astro/ccm_unred.pro
-
-    There appears to be an error in the Far-UV range in the original IDL
-    routine where the maximum inverse wavelength is 11 and it should be 10
-    according to Cardelli et al. 1989 (pag 251, Eq (5,a,b)).
-
-    """
-
-    if 0.3 <= mw < 1.1:
-        # Infrared.
-        a, b = 0.574 * (mw**1.61), -0.527 * (mw**1.61)
-
-    elif 1.1 <= mw < 3.3:
-        # Optical/NIR.
-        # Original coefficients from CCM89
-        # c1 = [1., 0.17699, -0.50447, -0.02427, 0.72085, 0.01979, -0.77530,
-        #       0.32999]
-        # c2 = [0., 1.41338, 2.28305, 1.07233, -5.38434, -0.62251, 5.30260,
-        #       -2.09002]
-        # New coefficients from O'Donnell (1994)
-        c1 = [1.0, 0.104, -0.609, 0.701, 1.137, -1.718, -0.827, 1.647, -0.505]
-        c2 = [0.0, 1.952, 2.908, -3.989, -7.985, 11.102, 5.491, -10.805, 3.347]
-        y = mw - 1.82
-        # Reverse because polyval starts from the highest degree.
-        c1.reverse(), c2.reverse()
-        a, b = np.polyval(c1, y), np.polyval(c2, y)
-
-    elif 3.3 <= mw < 8.0:
-        # Mid-UV
-        F_a, F_b = 0.0, 0.0
-        if mw >= 5.9:
-            y = mw - 5.9
-            F_a = -0.04473 * y**2 - 0.009779 * y**3
-            F_b = 0.2130 * y**2 + 0.1207 * y**3
-        a = 1.752 - 0.316 * mw - (0.104 / ((mw - 4.67) ** 2 + 0.341)) + F_a
-        b = -3.090 + 1.825 * mw + (1.206 / ((mw - 4.62) ** 2 + 0.263)) + F_b
-
-    elif 8.0 <= mw <= 10.0:
-        # Far-UV
-        c1 = [-1.073, -0.628, 0.137, -0.070]
-        c2 = [13.670, 4.257, -0.420, 0.374]
-        y = mw - 8.0
-        c1.reverse(), c2.reverse()
-        a, b = np.polyval(c1, y), np.polyval(c2, y)
-    else:
-        raise ValueError(
-            "The effective wavelength is {} [1/micron], beyond "
-            "the CCM model limit (10 [1/micron]).".format(mw)
-        )
-
-    return a, b
-
-
 def properModel(
     met_age_dict: dict, fix_params: dict, fit_params: dict
 ) -> tuple[float, float, float, float, float, float, float, int, int, int, int]:
     """Define the 'proper' model with values for (z, a) taken from its grid,
     and filled values for those parameters that are fixed.
 
     Parameters
@@ -486,18 +485,18 @@
     if len(met_age_dict["met"]) == 1:
         ml = mh = 0
     else:
         par = met_age_dict["met"]
         mh = min(len(par) - 1, np.searchsorted(par, model_full[0]))
         ml = mh - 1
 
-    if len(met_age_dict["a"]) == 1:
+    if len(met_age_dict["loga"]) == 1:
         al = ah = 0
     else:
-        par = met_age_dict["a"]
+        par = met_age_dict["loga"]
         ah = min(len(par) - 1, np.searchsorted(par, model_full[1]))
         al = ah - 1
 
     return *model_full, ml, mh, al, ah
 
 
 def zaWAverage(theor_tracks, met_age_dict, m_ini_idx, z_model, a_model, ml, mh, al, ah):
@@ -525,15 +524,15 @@
     if ml == al == mh == ah == 0:
         # The np.array() is important to avoid overwriting 'theor_tracks'
         return np.array(theor_tracks[ml][al])
 
     # The four points in the (z, age) grid that define the box that contains
     # the model value (z_model, a_model)
     z1, z2 = met_age_dict["met"][ml], met_age_dict["met"][mh]
-    a1, a2 = met_age_dict["a"][al], met_age_dict["a"][ah]
+    a1, a2 = met_age_dict["loga"][al], met_age_dict["loga"][ah]
     pts = np.array([(z1, a1), (z1, a2), (z2, a1), (z2, a2)])
 
     # Order: (z1, a1), (z1, a2), (z2, a1), (z2, a2)
     isochs = np.array(
         [
             theor_tracks[ml][al],
             theor_tracks[ml][ah],
@@ -635,24 +634,37 @@
     if isochrone.shape[0] > m_ini_idx + 1:
         isochrone[m_ini_idx + 1] += dm
 
     return isochrone
 
 
 def extinction(
-    ext_coefs, rand_norm, rand_unif, DR_distribution, m_ini_idx, Av, dr, Rv, isochrone
+    ext_law,
+    ext_coefs,
+    rand_norm,
+    rand_unif,
+    DR_distribution,
+    m_ini_idx,
+    binar_flag,
+    Av,
+    dr,
+    Rv,
+    isochrone,
 ):
     """
     Modifies magnitude and color(s) according to given values for the
     total absorption Av. Using this parameter instead of the E(B-V) extinction
     reduces the correlation with Rv.
 
     The distance modulus was applied before this function.
 
     isochrone = [mag, c1, (c2), .., Mini, mag_b, c1b, .., Mini_b]
+
+    For the CCMO model:
+
     ext_coefs = [mag_ec, c1_ec, ...]
 
     where:
     mag_ec = [a, b]  ; cX_ec = [[a1, b1], [a2, b2]]
 
     and:
     ccm_coef = a + b / Rv = ext_coefs[i][0] + ext_coefs[i][1] / Rv
@@ -666,14 +678,15 @@
                = (ef_m1 - ef_m2) * Av
                = [(a1 + b1/Rv) - (a2 + b2/Rv)] * Av
                = [(a1 - a2) + (b1 - b2)/Rv] * Av
                = (a12 + b12/Rv) * Av
                = (a12 + b12/Rv) * R_V * E(B-V)
     (m1 - m2)_obs = (m1 - m2)_int + E(m1 - m2)
     (m1 - m2)_obs = (m1 - m2)_int + (a12 + b12/Rv) * R_V * E(B-V)
+
     """
 
     if dr > 0.0:
         Ns = isochrone.shape[-1]
 
         if DR_distribution == "uniform":
             # Av_dr = rand_unif[:Ns] * dr
@@ -685,37 +698,128 @@
         # In place in case I ever want to implement the percentage of stars affected.
         # Without this, all stars are affected by the DR.
         # Av_dr[rand_unif[:Ns] > DR_percentage] = 0.0
 
         # Clip at 0
         Av = np.clip(Av + Av_dr, a_min=0, a_max=np.inf)
 
-    def colmove(ci):
-        Ex = (
-            (ext_coefs[ci][0][0] + ext_coefs[ci][0][1] / Rv)
-            - (ext_coefs[ci][1][0] + ext_coefs[ci][1][1] / Rv)
-        ) * Av
-        return Ex
+    if ext_law == "CCMO":
+        # Magnitude
+        ec_mag = ext_coefs[0][0] + ext_coefs[0][1] / Rv
+        # First color
+        ec_col1 = (ext_coefs[1][0][0] + ext_coefs[1][0][1] / Rv) - (
+            ext_coefs[1][1][0] + ext_coefs[1][1][1] / Rv
+        )
+    elif ext_law == "GAIADR3":
+        # If this model is used the first color is always expected to be BP-RP
+        # BP_RP = isochrone[1]
+        ec_mag, ec_col1 = dustapprox(isochrone[1], Av)
+
+    Ax = ec_mag * Av
+    isochrone[0] += Ax
+    Ex1 = ec_col1 * Av
+    isochrone[1] += Ex1
+
+    # Move binary data.
+    if binar_flag:
+        isochrone[m_ini_idx + 1] += Ax  # Magnitude
+        isochrone[m_ini_idx + 2] += Ex1  # First color
+
+    # Second color
+    if len(ext_coefs) > 2:
+        ec_col2 = (ext_coefs[2][0][0] + ext_coefs[2][0][1] / Rv) - (
+            ext_coefs[2][1][0] + ext_coefs[2][1][1] / Rv
+        )
+        Ex2 = ec_col2 * Av
+        isochrone[2] += Ex2
+        # Move color with binary data.
+        if binar_flag:
+            isochrone[m_ini_idx + 3] += Ex2
 
-    # Move magnitude
-    Ax_d = (ext_coefs[0][0] + ext_coefs[0][1] / Rv) * Av
-    isochrone[0] += Ax_d
-    # Move filters with binary data.
-    if isochrone.shape[0] > m_ini_idx + 1:
-        isochrone[m_ini_idx + 1] += Ax_d
+    return isochrone
 
-    # Move colors.
-    for ci in range(1, m_ini_idx):
-        Ex = colmove(ci)
-        isochrone[ci] += Ex
-        # Move colors with binary data.
-        if isochrone.shape[0] > m_ini_idx + 1:
-            isochrone[m_ini_idx + 1 + ci] += Ex
 
-    return isochrone
+def dustapprox(X_, Av):
+    """
+    The 'coeffs' values are the main sequence values taken from:
+
+    https://www.cosmos.esa.int/web/gaia/edr3-extinction-law
+
+    The order of the coefficients is:
+
+    Intercept   X   X2  X3  A   A2  A3  XA  AX2 XA2
+
+    X_ == BP-RP
+    """
+    coeffs = {
+        "G": (
+            0.995969721536602,
+            -0.159726460302015,
+            0.0122380738156057,
+            0.00090726555099859,
+            -0.0377160263914123,
+            0.00151347495244888,
+            -2.52364537395142e-05,
+            0.0114522658102451,
+            -0.000936914989014318,
+            -0.000260296774134201,
+        ),
+        "BP": (
+            1.15363197483424,
+            -0.0814012991657388,
+            -0.036013023976704,
+            0.0192143585568966,
+            -0.022397548243016,
+            0.000840562680547171,
+            -1.31018008013549e-05,
+            0.00660124080271006,
+            -0.000882247501989453,
+            -0.000111215755291684,
+        ),
+        "RP": (
+            0.66320787941067,
+            -0.0179847164933981,
+            0.000493769449961458,
+            -0.00267994405695751,
+            -0.00651422146709376,
+            3.30179903473159e-05,
+            1.57894227641527e-06,
+            -7.9800898337247e-05,
+            0.000255679812110045,
+            1.10476584967393e-05,
+        ),
+    }
+
+    X_2 = X_**2
+    X_3 = X_**3
+    Av_2 = Av**2
+    Av_3 = Av**3
+
+    def ext_coeff(k):
+        """
+        https://www.cosmos.esa.int/web/gaia/edr3-extinction-law
+        """
+        # X   X2  X3  A   A2  A3  XA  AX2 XA2
+        ay = coeffs[k][0]
+        for i, Xk in enumerate([X_, X_2, X_3]):
+            ay += coeffs[k][1 + i] * Xk
+        for i, Ak in enumerate([Av, Av_2, Av_3]):
+            ay += coeffs[k][4 + i] * Ak
+
+        ay += (
+            coeffs[k][7] * X_ * Av
+            + coeffs[k][9] * X_ * Av_2  # This index not a mistake
+            + coeffs[k][8] * X_2 * Av
+        )
+        return ay
+
+    ec_G = ext_coeff("G")
+    ec_BPRP = ext_coeff("BP") - ext_coeff("RP")
+
+    return ec_G, ec_BPRP
 
 
 def cut_max_mag(isoch_moved, max_mag_syn):
     """
     Remove stars from isochrone with magnitude values larger that the maximum
     observed value.
     """
@@ -898,19 +1002,21 @@
     )
 
     # Move theoretical isochrone using the distance modulus
     isoch_moved = move_isochrone(isochrone, self.m_ini_idx, dm)
 
     # Apply extinction correction
     isoch_extin = extinction(
+        self.ext_law,
         self.ext_coefs,
         self.rand_floats["norm"][0],
         self.rand_floats["unif"][0],
         self.DR_distribution,
         self.m_ini_idx,
+        self.binar_flag,
         av,
         dr,
         rv,
         isoch_moved,
     )
 
     # Remove isochrone stars beyond the maximum magnitude
```

### Comparing `asteca-0.5.1/asteca/synthetic.py` & `asteca-0.5.2/asteca/synthetic.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,191 +20,194 @@
 
     See the :ref:`synth_clusters` section for more details.
 
     Parameters
     ----------
     isochs : :class:`isochrones`
          :py:mod:`asteca.isochrones` object with the loaded files for the theoretical isochrones.
+    ext_law : str, {"CCMO", "GAIADR3"}, default="CCMO"
+        Extinction law. If "*GAIADR3*" is selected, the magnitude and first color defined
+        in :class:`isochrones` and :class:`cluster` are assumed to be Gaia's
+        (E)DR3 **G** and **(BP-RP)** respectively. The second color (if defined) will
+        always be affected by the "*CCMO*" model.
+    DR_distribution : str, {"uniform", "normal"}, default="uniform"
+        Distribution function for the differential reddening.
     IMF_name : str, {"salpeter_1955", "kroupa_2001", "chabrier_2014"}, default="chabrier_2014"
         Name of the initial mass function used to populate the isochrones.
     max_mass : int, default=100_000
         Maximum total initial mass. Should be large enough to allow generating as many
         synthetic stars as observed stars.
     gamma : str, float, {"D&K", "fisher_stepped", "fisher_peaked", "raghavan"}, default="D&K"
         Distribution function for the mass ratio of the binary systems.
-    DR_distribution : str, {"uniform", "normal"}, default="uniform"
-        Distribution function for the differential reddening.
     seed: int, optional, default=None
         Random seed. If ``None`` a random integer will be generated and used.
 
     """
+
     isochs: isochrones
+    ext_law: str = "CCMO"
+    DR_distribution: str = "uniform"
     IMF_name: str = "chabrier_2014"
     max_mass: int = 100_000
     gamma: float | str = "D&K"
-    DR_distribution: str = "uniform"
     seed: Optional[int] = None
 
     def __post_init__(self):
-
         if self.seed is None:
             self.seed = np.random.randint(100000)
-        print(f"Setting random seed to {self.seed}")
 
         # Check gamma distribution
-        gammas = (
-            "D&K",
-            "fisher_stepped",
-            "fisher_peaked",
-            "raghavan",
-        )
+        gammas = ("D&K", "fisher_stepped", "fisher_peaked", "raghavan")
         if isinstance(self.gamma, str):
             if self.gamma not in gammas:
                 raise ValueError(
                     f"gamma '{self.gamma}' not recognized. Should be one of {gammas}"
                 )
 
         # Check differential reddening function
-        DR_funcs = (
-            "uniform",
-            "normal",
-        )
+        DR_funcs = ("uniform", "normal")
         if self.DR_distribution not in DR_funcs:
             raise ValueError(
-                f"Differential reddening function '{self.DR_distribution}' not recognized. "
-                + f"Should be one of {DR_funcs}"
+                f"Differential reddening function '{self.DR_distribution}' not "
+                + f"recognized. Should be one of {DR_funcs}"
             )
 
         # Check IMF function
-        imfs = (
-            "salpeter_1955",
-            "kroupa_2001",
-            "chabrier_2014",
-        )
+        imfs = ("salpeter_1955", "kroupa_2001", "chabrier_2014")
         if self.IMF_name not in imfs:
             raise ValueError(
                 f"IMF '{self.IMF_name}' not recognized. Should be one of {imfs}"
             )
 
+        # Check extinction law
+        ext_laws = ("CCMO", "GAIADR3")
+        if self.ext_law not in ext_laws:
+            raise ValueError(
+                f"Extinction law '{self.ext_law}' not recognized. Should be "
+                + f"one of {ext_laws}"
+            )
+        # if self.ext_law == "CCMO":
+        #     if self.isochs.magnitude_effl is None or self.isochs.color_effl is None:
+        #         raise ValueError(
+        #             f"Extinction law '{self.ext_law}' requires effective lambda\n"
+        #             + "values for the magnitude and first color."
+        #         )
+        # if self.ext_law == "GAIADR3":
+        #     if self.isochs.magnitude_effl is not None or self.isochs.color_effl is not None:
+        #         warnings.warn(
+        #             f"\nExtinction law '{self.ext_law}' does not require effective lambda"
+        #             + " values for the\nmagnitude and first color (assumed to be 'G' "
+        #             + "and 'BP-RP', respectively)."
+        #         )
+
+        print("Instantiating synthetic...")
+
         # Sample the selected IMF
-        # Nmets, Nages = self.theor_tracks.shape[:2]
         Nmets, Nages = self.isochs.theor_tracks.shape[:2]
         self.st_dist_mass = scp.sample_imf(self, Nmets, Nages)
 
         # Add binary systems
         self.theor_tracks = scp.add_binarity(self)
 
         # Get extinction coefficients for these filters
-        self.ext_coefs = scp.extinction_coeffs(self)
+        self.ext_coefs = scp.ccmo_ext_coeffs(self)
 
         # Generate random floats used by `synth_clusters.synthcl_generate()`
         self.rand_floats = scp.randVals(self)
 
+        # Store for internal usage
+        self.met_age_dict = self.isochs.met_age_dict
+
+        print(f"Initial Mass Function  : {self.IMF_name}")
+        print(f"Maximum initial mass   : {self.max_mass}")
+        print(f"Gamma distribution     : {self.gamma}")
+        print(f"Extinction law         : {self.ext_law}")
+        print(f"Differential reddening : {self.DR_distribution}")
+        print(f"Random seed            : {self.seed}")
         print("Synthetic clusters object generated\n")
 
-    def calibrate(self, cluster, fix_params: dict = {}, z_to_FeH: float | None = None):
+    def calibrate(self, cluster, fix_params: dict = {}):
         r"""Calibrate a :py:mod:`asteca.synthetic` object based on a
         :py:mod:`asteca.cluster` object and a dictionary of fixed fundamental parameters
         (``fix_params``).
 
         Use the data obtained from your observed cluster stored in the
         :py:mod:`asteca.cluster` object, to calibrate a :py:mod:`asteca.synthetic`
-        object. Additionally, a dictionary of fixed fundamental parameters 
+        object. Additionally, a dictionary of fixed fundamental parameters
         (metallicity, age, distance, extinction, etc.) can be passed.
 
         See the :ref:`synth_clusters` section for more details.
 
         Parameters
         ----------
         cluster : :class:`cluster`
              :py:mod:`asteca.cluster` object with the processed data from your observed
              cluster.
         fix_params : dict, optional, default={}
             Dictionary with the values for the fixed parameters (if any).
-        z_to_FeH : float, optional, default=None
-            If ``None``, the default ``z`` values (defined when loading the isochrones
-            via the :py:mod:`asteca.isochrones` object) will be used to generate the
-            synthetic clusters. If ``float``, it must represent the solar metallicity
-            for these isochrones. The metallicity values will then be converted to
-            ``[FeH]`` values, to be used by the :meth:`synthetic.generate()` method.
 
         """
+        # Check that the number of colors match
+        if self.isochs.color2_effl is not None and cluster.color2 is None:
+            raise ValueError(
+                "Two colors were defined in 'synthetic' but a single color\n"
+                + "was defined in 'cluster'."
+            )
+        if self.isochs.color2_effl is None and cluster.color2 is not None:
+            raise ValueError(
+                "Two colors were defined in 'cluster' but a single color\n"
+                + "was defined in 'synthetic'."
+            )
+
         # Used by the mass and binary probability estimation
         self.mag_p = cluster.mag_p
         self.colors_p = cluster.colors_p
 
         # Data used by the `generate()` method
         self.max_mag_syn = max(cluster.mag_p)
         self.N_obs_stars = len(cluster.mag_p)
         self.m_ini_idx = len(cluster.colors_p) + 1
         self.err_dist = scp.error_distribution(
             self, cluster.mag_p, cluster.e_mag_p, cluster.e_colors_p
         )
 
         self.fix_params = fix_params
 
-        # Convert z to FeH if requested
-        self.met_age_dict = self.isochs.met_age_dict
-        if z_to_FeH is not None:
-            self._func_z_to_FeH(z_to_FeH)
-
-        # Check if binary systems are to be produced
         self.binar_flag = True
         if "alpha" in list(fix_params.keys()) and "beta" in list(fix_params.keys()):
             if fix_params["alpha"] == 0.0 and fix_params["beta"] == 0.0:
                 self.binar_flag = False
 
+        # Check that the ranges are respected
+        for par in ("met", "loga"):
+            if par not in self.fix_params.keys():
+                N_par = len(self.met_age_dict[par])
+                if N_par == 1:
+                    raise ValueError(
+                        f"Parameter '{par}' is not fixed and its range is limited to "
+                        + f"a single value: {self.met_age_dict[par]}"
+                    )
+
         # # Remove low masses if required
         # if dm_min is not None:
         #     self._rm_low_masses(dm_min)
 
-    def _func_z_to_FeH(self, z_to_FeH):
-        """ """
-        feh = np.log10(self.met_age_dict["met"] / z_to_FeH)
-        N_old = len(feh)
-        round_n = 4
-        while True:
-            feh_r = np.round(feh, round_n)
-            N_new = len(set(feh_r))
-            # If no duplicated values exist after rounding
-            if N_old == N_new:
-                break
-            round_n += 1
-        # Replace old values
-        self.met_age_dict["met"] = feh_r
-
-    def min_max(self) -> tuple[float]:
-        r"""Return the minimum and maximum values for the metallicity and age defined
-        in the theoretical isochrones.
-
-        Returns
-        -------
-        tuple[float]
-            Tuple of (minimum_metallicity, maximum_metallicity, minimum_age, maximum_age)
-
-        """
-        zmin = self.met_age_dict["met"].min()
-        zmax = self.met_age_dict["met"].max()
-        amin = self.met_age_dict["a"].min()
-        amax = self.met_age_dict["a"].max()
-        return zmin, zmax, amin, amax
-
     def generate(self, fit_params: dict) -> np.ndarray:
         r"""Generate a synthetic cluster.
 
         The synthetic cluster is generated according to the parameters given in
         the ``fit_params`` dictionary and the already calibrated
         :py:mod:`asteca.synthetic` object.
 
         Parameters
         ----------
         fit_params : dict
             Dictionary with the values for the fundamental parameters that were **not**
             included in the ``fix_params`` dictionary when the
-            :py:mod:`asteca.synthetic` object was calibrated 
+            :py:mod:`asteca.synthetic` object was calibrated
             (:meth:`synthetic.calibrate()` method).
 
         Returns
         -------
         array[mag, c1, (c2)]
             Return a ``np.array`` containing a synthetic cluster with the shape
             ``[mag, c1, (c2)]``, where ``mag`` is the magnitude dimension, and
@@ -233,19 +236,21 @@
         )
 
         # Move theoretical isochrone using the distance modulus
         isoch_moved = scp.move_isochrone(isochrone, self.m_ini_idx, dm)
 
         # Apply extinction correction
         isoch_extin = scp.extinction(
+            self.ext_law,
             self.ext_coefs,
             self.rand_floats["norm"][0],
             self.rand_floats["unif"][0],
             self.DR_distribution,
             self.m_ini_idx,
+            self.binar_flag,
             av,
             dr,
             rv,
             isoch_moved,
         )
 
         # Remove isochrone stars beyond the maximum magnitude
@@ -273,49 +278,57 @@
         # Assign errors according to errors distribution.
         synth_clust = scp.add_errors(
             isoch_binar, self.err_dist, self.rand_floats["norm"][1]
         )
 
         return synth_clust[: self.m_ini_idx]
 
-    def synthplot(self, fit_params, ax=None, isochplot=False):
+    def synthplot(self, ax, fit_params, color_idx=0, isochplot=False):
         r"""Generate a color-magnitude plot for a synthetic cluster.
 
         The synthetic cluster is generated using the fundamental parameter values
         given in the ``fit_params`` dictionary.
 
         Parameters
         ----------
+        ax : matplotlib.axis, optional, default=None
+            Matplotlib axis where to draw the plot.
         fit_params : dict
             Dictionary with the values for the fundamental parameters that were **not**
             included in the ``fix_params`` dictionary when the
             :py:mod:`asteca.synthetic` object was calibrated
             (:meth:`synthetic.calibrate()` method).
-        ax : matplotlib.axis, optional, default=None
-            Matplotlib axis where to draw the plot.
+        color_idx : int, default=0
+            Index of the color to plot. If ``0`` (default), plot the first color. If
+            ``1`` plot the second color.
         isochplot : bool, default=False
             If ``True``, the accompanying isochrone will be plotted.
 
         Returns
         -------
         matplotlib.axis
             Matplotlib axis object
 
         """
-        if ax is None:
-            f, ax = plt.subplots()
+        if color_idx > 1:
+            raise ValueError(
+                f"Wrong 'color_idx' value ({color_idx}), should be one of: [0, 1]"
+            )
 
         # Generate synthetic cluster.
         synth_clust = scp.generate(self, fit_params)
         if self.binar_flag is True:
             binar_idx = ~np.isnan(synth_clust[-1])
         else:
             binar_idx = np.full(synth_clust.shape[1], False)
 
-        x_synth, y_synth = synth_clust[1], synth_clust[0]
+        y_synth = synth_clust[0]
+        x_synth = synth_clust[1]
+        if color_idx == 1:
+            x_synth = synth_clust[2]
         # Single synthetic systems
         ax.scatter(
             x_synth[~binar_idx],
             y_synth[~binar_idx],
             marker="^",
             c="#519ddb",
             alpha=0.5,
@@ -327,45 +340,50 @@
             y_synth[binar_idx],
             marker="v",
             c="#F34C4C",
             alpha=0.5,
             label=f"Synthetic (binary), N={len(x_synth[binar_idx])}",
         )
 
-        plt.ylabel(list(self.isochs.magnitude.keys())[0])
-        c1, c2 = list(self.isochs.color.keys())
+        plt.ylabel(self.isochs.magnitude)
+        c1, c2 = self.isochs.color
+        if color_idx == 1:
+            c1, c2 = self.isochs.color2
         plt.xlabel(f"{c1}-{c2}")
-        ax.set_ylim(max(self.mag_p) + .5, min(self.mag_p) - .5)
+        ax.set_ylim(max(self.mag_p) + 0.5, min(self.mag_p) - 0.5)
         ax.legend()
 
         if isochplot is False:
             return ax
 
         # Generate displaced isochrone
         fit_params_copy = dict(fit_params)
         fit_params_copy["DR"] = 0.0
         isochrone = scp.generate(self, fit_params_copy, True)
         # Remove stars beyond the color limits
         xmin, xmax = x_synth[~binar_idx].min(), x_synth[~binar_idx].max()
-        msk = (isochrone[1] >= xmin) & (isochrone[1] <= xmax)
+        c_idx = 1
+        if color_idx == 1:
+            c_idx = 2
+        msk = (isochrone[c_idx] >= xmin) & (isochrone[c_idx] <= xmax)
         isochrone = isochrone[:, msk]
-        ax.plot(isochrone[1], isochrone[0], c="k")
+        ax.plot(isochrone[c_idx], isochrone[0], c="k")
 
         return ax
 
     def masses_binary_probs(self, model, model_std):
         r"""Estimate individual masses for the observed stars, along with their binary
         probabilities (if binarity was estimated).
 
         Parameters
         ----------
         model : dict
             Dictionary with the values for the fundamental parameters that were **not**
             included in the ``fix_params`` dictionary when the
-            :py:mod:`asteca.synthetic` object was calibrated 
+            :py:mod:`asteca.synthetic` object was calibrated
             (:meth:`synthetic.calibrate()` method).
         model_std : dict
             Dictionary with the standard deviations for the fundamental parameters in
             the ``model`` argument.
 
         Returns
         -------
@@ -377,38 +395,43 @@
 
         """
         # Generate random models from the selected solution
         models = mb.ranModels(model, model_std, self.seed)
 
         # Observed photometry
         obs_phot = np.array([self.mag_p] + [_ for _ in self.colors_p])
-        # Identify nans in mag and colors and re-write them as -10. This ensures
-        # that the photometric distances to these stars is large enough to not be
-        # matched.
+        # Replace nans in mag and colors to avoid crashing KDTree()
         nan_msk = np.full(obs_phot.shape[1], False)
-        for col in obs_phot:
-            nan_msk = nan_msk | np.isnan(col)
+        for ophot in obs_phot:
+            nan_msk = nan_msk | np.isnan(ophot)
         obs_phot[:, nan_msk] = -10.0
         obs_phot = obs_phot.T
 
-        m12_masses, b_fr_all,  = [], []
+        (
+            m12_masses,
+            b_fr_all,
+        ) = (
+            [],
+            [],
+        )
         for model in models:
             isoch = scp.generate(self, model)
             if not isoch.any():
                 continue
             m1_obs, m2_obs, b_fr = mb.get_m1m2_bpr(self, isoch, obs_phot)
             m12_masses.append([m1_obs, m2_obs])
             b_fr_all.append(b_fr)
         m12_masses = np.array(m12_masses)
 
         # Primary masses (median + stddev)
         m1_med = np.median(m12_masses[:, 0, :], 0)
         m1_std = np.std(m12_masses[:, 0, :], 0)
         # Secondary masses  (median + stddev). Hide 'All-nan slice' warnings
-        with warnings.catch_warnings(action="ignore"):
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")  # TODO: this was changed in Python>3.10
             m2_med = np.nanmedian(m12_masses[:, 1, :], 0)
             # m2 can not be larger than m1
             m2_med = np.min([m1_med, m2_med], 0)
             m2_std = np.nanstd(m12_masses[:, 1, :], 0)
 
         # Binary probability per star
         binar_prob = (~np.isnan(m12_masses[:, 1, :])).sum(0) / m12_masses.shape[0]
@@ -419,14 +442,22 @@
                 "m1": m1_med,
                 "m1_std": m1_std,
                 "m2": m2_med,
                 "m2_std": m2_std,
                 "binar_prob": binar_prob,
             }
         )
+        # Assign all nans to stars with a photometric nan in any dimension
+        df[nan_msk] = np.nan
+        if nan_msk.sum() > 0:
+            warnings.warn(
+                f"\nN={nan_msk.sum()} stars found with no valid photometric data. "
+                + "These will be assigned 'nan' values\nfor masses and "
+                + "binarity probability"
+            )
 
         return df, np.array(b_fr_all)
 
     def _get_masses(self, fit_params, model_std, ra_c, dec_c):
         """
         Estimate the different total masses for the observed cluster
         """
```

### Comparing `asteca-0.5.1/pyproject.toml` & `asteca-0.5.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "asteca"
-version = "0.5.1"
+version = "0.5.2"
 description = "Stellar cluster analysis package"
 authors = ["Gabriel I Perren <gabrielperren@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 keywords = ["cluster", "astrophysics"]
 homepage = "https://asteca.github.io/"
 repository = "https://github.com/asteca/ASteCA"
 documentation = "https://asteca.readthedocs.io/"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 numpy = "^1.26.4"
 matplotlib = "^3.8.4"
 scipy = "^1.13.0"
-astropy = "^6.0.1"
+astropy = "^6.1.0"
 pandas = "^2.2.2"
 fast-histogram = "^0.14"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `asteca-0.5.1/PKG-INFO` & `asteca-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: asteca
-Version: 0.5.1
+Version: 0.5.2
 Summary: Stellar cluster analysis package
 Home-page: https://asteca.github.io/
 License: MIT
 Keywords: cluster,astrophysics
 Author: Gabriel I Perren
 Author-email: gabrielperren@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: astropy (>=6.0.1,<7.0.0)
+Requires-Dist: astropy (>=6.1.0,<7.0.0)
 Requires-Dist: fast-histogram (>=0.14,<0.15)
 Requires-Dist: matplotlib (>=3.8.4,<4.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: scipy (>=1.13.0,<2.0.0)
 Project-URL: Documentation, https://asteca.readthedocs.io/
 Project-URL: Repository, https://github.com/asteca/ASteCA
```

