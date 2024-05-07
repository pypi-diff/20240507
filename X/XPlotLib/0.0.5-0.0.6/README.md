# Comparing `tmp/xplotlib-0.0.5.tar.gz` & `tmp/xplotlib-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xplotlib-0.0.5.tar", last modified: Thu May  2 21:41:56 2024, max compression
+gzip compressed data, was "xplotlib-0.0.6.tar", last modified: Tue May  7 20:37:04 2024, max compression
```

## Comparing `xplotlib-0.0.5.tar` & `xplotlib-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:41:56.400501 xplotlib-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-02 21:41:51.000000 xplotlib-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-02 21:41:56.400501 xplotlib-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-02 21:41:51.000000 xplotlib-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-02 21:41:51.000000 xplotlib-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-02 21:41:56.400501 xplotlib-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:41:56.396501 xplotlib-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:41:56.396501 xplotlib-0.0.5/src/XPlotLib/
--rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-05-02 21:41:51.000000 xplotlib-0.0.5/src/XPlotLib/BandgapAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)    18473 2024-05-02 21:41:51.000000 xplotlib-0.0.5/src/XPlotLib/DOSAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-02 21:41:51.000000 xplotlib-0.0.5/src/XPlotLib/XPlotLibUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:41:51.000000 xplotlib-0.0.5/src/XPlotLib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:41:56.400501 xplotlib-0.0.5/src/XPlotLib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-02 21:41:56.000000 xplotlib-0.0.5/src/XPlotLib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-02 21:41:56.000000 xplotlib-0.0.5/src/XPlotLib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 21:41:56.000000 xplotlib-0.0.5/src/XPlotLib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-02 21:41:56.000000 xplotlib-0.0.5/src/XPlotLib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 21:41:56.000000 xplotlib-0.0.5/src/XPlotLib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:37:04.726007 xplotlib-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-07 20:37:00.000000 xplotlib-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13651 2024-05-07 20:37:04.726007 xplotlib-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12981 2024-05-07 20:37:00.000000 xplotlib-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-07 20:37:00.000000 xplotlib-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-07 20:37:04.726007 xplotlib-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:37:04.718007 xplotlib-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:37:04.722007 xplotlib-0.0.6/src/XPlotLib/
+-rw-r--r--   0 runner    (1001) docker     (127)    14137 2024-05-07 20:37:00.000000 xplotlib-0.0.6/src/XPlotLib/BandgapAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18605 2024-05-07 20:37:00.000000 xplotlib-0.0.6/src/XPlotLib/DOSAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-07 20:37:00.000000 xplotlib-0.0.6/src/XPlotLib/XPlotLibUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:37:00.000000 xplotlib-0.0.6/src/XPlotLib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:37:04.722007 xplotlib-0.0.6/src/XPlotLib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13651 2024-05-07 20:37:04.000000 xplotlib-0.0.6/src/XPlotLib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-07 20:37:04.000000 xplotlib-0.0.6/src/XPlotLib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:37:04.000000 xplotlib-0.0.6/src/XPlotLib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-07 20:37:04.000000 xplotlib-0.0.6/src/XPlotLib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 20:37:04.000000 xplotlib-0.0.6/src/XPlotLib.egg-info/top_level.txt
```

### Comparing `xplotlib-0.0.5/LICENSE` & `xplotlib-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xplotlib-0.0.5/setup.cfg` & `xplotlib-0.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = XPlotLib
-version = 0.0.5
+version = 0.0.6
 author = Carl Magnus Meier
 author_email = magnus.meier@outook.de
 description = Libary to plot experimental and theoretical XRay data.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CMM02/XPlotLib
 classifiers =
```

### Comparing `xplotlib-0.0.5/src/XPlotLib/BandgapAnalyzer.py` & `xplotlib-0.0.6/src/XPlotLib/BandgapAnalyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,29 +24,35 @@
         headers = [[f'{header}_energy', f'{header}_intensity'] for header in names]
         headers = [item for sublist in headers for item in sublist]
         return pd.read_csv(path, sep=sep, skiprows=skiprows, header=None, names=headers)
     
     def __normalize(self, list):
         abs_max = max(max(list), -min(list))
         return [x/abs_max for x in list]
+    
+    
+    def __find_onset(self, path, binding, fermi):
+        df = pd.read_csv(path, sep='\\s+', header=None, names=['energy', 'intensity1', 'intensity2', 'intensity3'])
+        onset = min(df.loc[df['intensity1']>0]['energy']) + (binding + fermi) * ryd_to_ev
+        return onset
 
     """
     Load experimental spectra
 
     Parameters
     ----------
     path : str
         Path to the file containing the spectra
     type : str
         Type of the spectra. Must be either 'xes' or 'xas'
     names : list of str
         Names of the spectra
-    skiprows : int
+    skiprows : int, optional
         Number of rows to skip in the beginning of the file
-    sep : str
+    sep : str, optional
         Separator used in the file
     """
     def load_exp_spectra(self, path, type, names, skiprows=2, sep=','):        
         if type == 'xes':
             exp_spectra = self.xes_exp_spectra
         elif type == 'xas':
             exp_spectra = self.xas_exp_spectra
@@ -116,14 +122,22 @@
         x = exp_spectra[name][f'{name}_energy'].values
         y = exp_spectra[name][f'{name}_intensity'].values
         y_smoothed = non_uniform_savgol(x, y, window, poly)
         exp_spectra[name][f'{name}_smoothed_intensity'] = y_smoothed
         # take second derivative
         exp_spectra[name][f'{name}_smoothed_2nd'] = np.gradient(np.gradient(y_smoothed, x), x)
 
+
+        # make sure onset region includes at least one data point
+        if onset_region:
+            if onset_region[0] > onset_region[1]:
+                raise ValueError('The start of the onset region must be smaller than the end.')
+            if onset_region[1] < min(x) or onset_region[0] > max(x):
+                raise ValueError('The onset region is outside of the energy range.')
+
         if show:
             # plot the smoothed data
             if onset_region:
                 fig, (ax, ax_onset) = plt.subplots(1,2, figsize=(10,6))
                 ax_onset.set_xlim(onset_region)
                 ax_onset.set_xlim(onset_region)
                 y_onset = exp_spectra[name].loc[(exp_spectra[name][f'{name}_energy'] >= onset_region[0]) & (exp_spectra[name][f'{name}_energy'] <= onset_region[1]), f'{name}_intensity']
@@ -272,20 +286,42 @@
                 axes[1,0].annotate(text, xy=xy, xytext=xytext, arrowprops=dict(facecolor='black', shrink=0.05), ha='center', va='center', rotation=text_rot)
 
             # annotate first XAS peak
             if self.xas_arrow:
                 xy, xytext, text, text_rot = self.xas_arrow
                 axes[1,1].annotate(text, xy=xy, xytext=xytext, arrowprops=dict(facecolor='black', shrink=0.05), ha='center', va='center', rotation=text_rot)
 
-    
-    def __find_onset(self, path, binding, fermi):
-        df = pd.read_csv(path, sep='\\s+', header=None, names=['energy', 'intensity1', 'intensity2', 'intensity3'])
-        onset = min(df.loc[df['intensity1']>0]['energy']) + (binding + fermi) * ryd_to_ev
-        return onset
-    
+    """
+    Export 2nd derivative of XES and XAS spectra to csv files
+
+    Parameters
+    ----------
+    path : str
+        Path to the directory where the files will be saved
+    name : str
+        Name of the files (without extension)
+    """
+    def export_2nd_derivative(self, path, name):
+        xes_2nd = pd.DataFrame()
+        for xes_exp_name in self.xes_exp_spectra.keys():
+            if f'{xes_exp_name}_smoothed_2nd' not in self.xes_exp_spectra[xes_exp_name].columns:
+                print(f'No 2nd derivative found for {xes_exp_name}. Run smoothen method first, if you want to export the 2nd derivative.')
+                continue
+            xes_2nd[f'{xes_exp_name}_energy'] = self.xes_exp_spectra[xes_exp_name][f'{xes_exp_name}_energy']
+            xes_2nd[f'{xes_exp_name}_2nd'] = self.xes_exp_spectra[xes_exp_name][f'{xes_exp_name}_smoothed_2nd']
+        xes_2nd.to_csv(f'{path}/{name}_XES_2nd.csv', index=False)
+
+        xas_2nd = pd.DataFrame()
+        for xas_exp_name in self.xas_exp_spectra.keys():
+            if f'{xas_exp_name}_smoothed_2nd' not in self.xas_exp_spectra[xas_exp_name].columns:
+                print(f'No 2nd derivative found for {xas_exp_name}. Run smoothen method first, if you want to export the 2nd derivative.')
+                continue
+            xas_2nd[f'{xas_exp_name}_energy'] = self.xas_exp_spectra[xas_exp_name][f'{xas_exp_name}_energy']
+            xas_2nd[f'{xas_exp_name}_2nd'] = self.xas_exp_spectra[xas_exp_name][f'{xas_exp_name}_smoothed_2nd']
+        xas_2nd.to_csv(f'{path}/{name}_XAS_2nd.csv', index=False)
 
     """
     Load unbrodened spectra to determine core hole shift
 
     Parameters
     ----------
     dir : str
@@ -302,49 +338,19 @@
         Fermi energy of the excited state
     """
     def load_unbroadend(self, dir, GS_file, ES_file, GS_binding, GS_fermi, ES_fermi):
         self.gs_onsets.append(self.__find_onset(f'{dir}/{GS_file}', GS_binding, GS_fermi))
         self.es_onsets.append(self.__find_onset(f'{dir}/{ES_file}', GS_binding, ES_fermi))
 
     """
-    Calculate the core hole shift using all previously loaded unbrodened spectra
+    Calculate the core hole shift using all previously loaded unbrodened spectra.
+    !Warning this might not be accurate!
 
     Returns
     -------
     float
         Core hole shift
     """
     def calc_core_hole_shift(self):
         return min(self.es_onsets) - min(self.gs_onsets)
 
-
-    """
-    Export 2nd derivative of XES and XAS spectra to csv files
-
-    Parameters
-    ----------
-    path : str
-        Path to the directory where the files will be saved
-    name : str
-        Name of the files (without extension)
-    """
-
-    def export_2nd_derivative(self, path, name):
-        xes_2nd = pd.DataFrame()
-        for xes_exp_name in self.xes_exp_spectra.keys():
-            if f'{xes_exp_name}_smoothed_2nd' not in self.xes_exp_spectra[xes_exp_name].columns:
-                print(f'No 2nd derivative found for {xes_exp_name}. Run smoothen method first, if you want to export the 2nd derivative.')
-                continue
-            xes_2nd[f'{xes_exp_name}_energy'] = self.xes_exp_spectra[xes_exp_name][f'{xes_exp_name}_energy']
-            xes_2nd[f'{xes_exp_name}_2nd'] = self.xes_exp_spectra[xes_exp_name][f'{xes_exp_name}_smoothed_2nd']
-        xes_2nd.to_csv(f'{path}/{name}_XES_2nd.csv', index=False)
-
-        xas_2nd = pd.DataFrame()
-        for xas_exp_name in self.xas_exp_spectra.keys():
-            if f'{xas_exp_name}_smoothed_2nd' not in self.xas_exp_spectra[xas_exp_name].columns:
-                print(f'No 2nd derivative found for {xas_exp_name}. Run smoothen method first, if you want to export the 2nd derivative.')
-                continue
-            xas_2nd[f'{xas_exp_name}_energy'] = self.xas_exp_spectra[xas_exp_name][f'{xas_exp_name}_energy']
-            xas_2nd[f'{xas_exp_name}_2nd'] = self.xas_exp_spectra[xas_exp_name][f'{xas_exp_name}_smoothed_2nd']
-        xas_2nd.to_csv(f'{path}/{name}_XAS_2nd.csv', index=False)
-
```

### Comparing `xplotlib-0.0.5/src/XPlotLib/DOSAnalyzer.py` & `xplotlib-0.0.6/src/XPlotLib/DOSAnalyzer.py`

 * *Files 5% similar despite different names*

```diff
@@ -240,19 +240,19 @@
     ----------
     path : str
         Path to the spectrum file
     name : str
         Name of the spectrum
     spec_type : str
         Type of the spectrum ("XES" or "XAS")
-    skiprows : int
+    skiprows : int, optional
         Number of rows to skip in the file
-    delim : str
+    delim : str, optional
         Delimiter of the file
-    shift : float
+    shift : float, optional
         Energy shift of the spectrum
     """
     def load_spectrum(self, path, name, spec_type, skiprows=1, delim=',', shift=0):
         spectrum = pd.read_csv(path, header=None, names=['ENERGY', 'intensity'], skiprows=skiprows, delimiter=delim)
         spectrum['ENERGY'] = spectrum['ENERGY'] + shift
         if spec_type == 'XES':
             self.xes_spectra[name] = spectrum
@@ -327,17 +327,17 @@
         #     print(dos)
 
     """
     Set active DOS for plotting
 
     Parameters
     ----------
-    xes_names : list of str
+    xes_names : list of str, optional
         List of XES DOS names to plot
-    xas_names : list of str
+    xas_names : list of str, optional
         List of XAS DOS names to plot
     """
     def set_active_dos(self, xes_names=[], xas_names=[]):
         # reset all active dos
         for dos in self.active_xes_dos.keys():
             self.active_xes_dos[dos] = False
         for dos in self.active_xas_dos.keys():
@@ -368,33 +368,33 @@
 
 
     """
     Set x limits for XES and XAS DOS
 
     Parameters
     ----------
-    xes_x_limits : tuple of float
+    xes_x_limits : tuple of float, optional
         X limits for XES DOS
-    xas_x_limits : tuple of float
+    xas_x_limits : tuple of float, optional
         X limits for XAS DOS
     """
     def set_x_limits(self, xes_x_limits=None, xas_x_limits=None):
         self.xes_x_lims = xes_x_limits
         self.xas_x_lims = xas_x_limits
 
 
     """
     Plot DOS with XES and XAS spectra
 
     Parameters
     ----------
     staggered : bool
         Staggered DOS
-    show_spectra : list of str
-        List of spectra to show ("XES" or "XAS")
+    show_spectra : list of str, optional
+        List of spectra to show ("XES" or "XAS"), default shows both
     """
     def plot_dos(self, staggered=False, show_spectra=['XES', 'XAS']):
         if len(show_spectra) == 0:
             print('No spectra selected for plotting, select from "XES" and "XAS"')
             return
         
         # remove duplicates from show_spectra
@@ -459,16 +459,16 @@
 
     Parameters
     ----------
     path : str
         Path to the directory where to save the DOS
     name : str
         Name of the DOS file
-    export_spectra : list of str
-        List of spectra to export ("XES" or "XAS")
+    export_spectra : list of str, optional
+        List of spectra to export ("XES" or "XAS"), default exports both
     """
     def export_dos(self, path, name, export_spectra=['XES', 'XAS']):
         if len(export_spectra) == 0:
             print('No spectra selected for export, select from "XES" and "XAS"')
             return
         
         # remove duplicates from show_spectra
```

### Comparing `xplotlib-0.0.5/src/XPlotLib/XPlotLibUtils.py` & `xplotlib-0.0.6/src/XPlotLib/XPlotLibUtils.py`

 * *Files identical despite different names*

