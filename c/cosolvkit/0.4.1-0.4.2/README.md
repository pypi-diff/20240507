# Comparing `tmp/cosolvkit-0.4.1.tar.gz` & `tmp/cosolvkit-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosolvkit-0.4.1.tar", last modified: Tue Apr 30 23:18:40 2024, max compression
+gzip compressed data, was "cosolvkit-0.4.2.tar", last modified: Tue May  7 01:17:24 2024, max compression
```

## Comparing `cosolvkit-0.4.1.tar` & `cosolvkit-0.4.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:18:40.897496 cosolvkit-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-30 23:18:32.000000 cosolvkit-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-30 23:18:40.897496 cosolvkit-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10798 2024-04-30 23:18:32.000000 cosolvkit-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:18:40.893496 cosolvkit-0.4.1/cosolvkit/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-30 23:18:32.000000 cosolvkit-0.4.1/cosolvkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20997 2024-04-30 23:18:32.000000 cosolvkit-0.4.1/cosolvkit/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-30 23:18:32.000000 cosolvkit-0.4.1/cosolvkit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    62055 2024-04-30 23:18:32.000000 cosolvkit-0.4.1/cosolvkit/cosolvent_system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:18:40.893496 cosolvkit-0.4.1/cosolvkit/data/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-30 23:18:32.000000 cosolvkit-0.4.1/cosolvkit/data/aromatic.json
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-30 23:18:32.000000 cosolvkit-0.4.1/cosolvkit/data/config.json
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-30 23:18:32.000000 cosolvkit-0.4.1/cosolvkit/data/cosolvents.json
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-30 23:18:32.000000 cosolvkit-0.4.1/cosolvkit/data/forcefields.json
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-30 23:18:32.000000 cosolvkit-0.4.1/cosolvkit/data/h_bonding.json
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-30 23:18:32.000000 cosolvkit-0.4.1/cosolvkit/data/lipophilic.json
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-30 23:18:32.000000 cosolvkit-0.4.1/cosolvkit/data/negative.json
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-30 23:18:32.000000 cosolvkit-0.4.1/cosolvkit/data/positive.json
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-04-30 23:18:32.000000 cosolvkit-0.4.1/cosolvkit/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-30 23:18:32.000000 cosolvkit-0.4.1/cosolvkit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:18:40.893496 cosolvkit-0.4.1/cosolvkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-30 23:18:40.000000 cosolvkit-0.4.1/cosolvkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-30 23:18:40.000000 cosolvkit-0.4.1/cosolvkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 23:18:40.000000 cosolvkit-0.4.1/cosolvkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 23:18:40.000000 cosolvkit-0.4.1/cosolvkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 23:18:40.000000 cosolvkit-0.4.1/cosolvkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 23:18:32.000000 cosolvkit-0.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:18:40.893496 cosolvkit-0.4.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-04-30 23:18:32.000000 cosolvkit-0.4.1/scripts/create_cosolvent_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-30 23:18:32.000000 cosolvkit-0.4.1/scripts/post_simulation_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 23:18:40.897496 cosolvkit-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-30 23:18:32.000000 cosolvkit-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:17:24.145645 cosolvkit-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-07 01:17:24.141646 cosolvkit-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12032 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:17:24.141646 cosolvkit-0.4.2/cosolvkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25858 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58843 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/cosolvent_system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:17:24.141646 cosolvkit-0.4.2/cosolvkit/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/data/aromatic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/data/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/data/cosolvents.json
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/data/forcefields.json
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/data/h_bonding.json
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/data/lipophilic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/data/negative.json
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/data/positive.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:17:24.141646 cosolvkit-0.4.2/cosolvkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-07 01:17:24.000000 cosolvkit-0.4.2/cosolvkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-07 01:17:24.000000 cosolvkit-0.4.2/cosolvkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 01:17:24.000000 cosolvkit-0.4.2/cosolvkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 01:17:24.000000 cosolvkit-0.4.2/cosolvkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-07 01:17:24.000000 cosolvkit-0.4.2/cosolvkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:17:24.141646 cosolvkit-0.4.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/scripts/create_cosolvent_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/scripts/post_simulation_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 01:17:24.145645 cosolvkit-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/setup.py
```

### Comparing `cosolvkit-0.4.1/LICENSE` & `cosolvkit-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.1/PKG-INFO` & `cosolvkit-0.4.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: cosolvkit
-Version: 0.4.1
+Version: 0.4.2
 Summary: CosolvKit
 Home-page: https://github.com/forlilab/cosolvkit
 Author: Niccolo Bruciaferri, Jerome Eberhardt
 Author-email: forli@scripps.edu
 License: LGPL-2.1
 Keywords: molecular modeling,drug design,cosolvent,MD simulations
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.9, <3.12
 License-File: LICENSE
```

### Comparing `cosolvkit-0.4.1/README.md` & `cosolvkit-0.4.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,34 @@
-[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) [![License: LGPL v2.1](https://img.shields.io/badge/License-LGPL_v2.1-green.svg)](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html)
+[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) [![License: LGPL v2.1](https://img.shields.io/badge/License-LGPL_v2.1-green.svg)](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html) [![PyPI - Version](https://img.shields.io/pypi/v/cosolvkit)](https://pypi.org/project/cosolvkit/0.4.1/) [![Powered by RDKit](https://img.shields.io/badge/Powered%20by-RDKit-3838ff.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQBAMAAADt3eJSAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAAFVBMVEXc3NwUFP8UPP9kZP+MjP+0tP////9ZXZotAAAAAXRSTlMAQObYZgAAAAFiS0dEBmFmuH0AAAAHdElNRQfmAwsPGi+MyC9RAAAAQElEQVQI12NgQABGQUEBMENISUkRLKBsbGwEEhIyBgJFsICLC0iIUdnExcUZwnANQWfApKCK4doRBsKtQFgKAQC5Ww1JEHSEkAAAACV0RVh0ZGF0ZTpjcmVhdGUAMjAyMi0wMy0xMVQxNToyNjo0NyswMDowMDzr2J4AAAAldEVYdGRhdGU6bW9kaWZ5ADIwMjItMDMtMTFUMTU6MjY6NDcrMDA6MDBNtmAiAAAAAElFTkSuQmCC)](https://www.rdkit.org/)
+[![Documentation Status](https://readthedocs.org/projects/cosolvkit/badge/?version=latest)](https://cosolvkit.readthedocs.io/en/latest/?badge=latest)
+      
+    
 
 # CosolvKit
-The python package for creating cosolvent system
+The python package for creating cosolvent system.  
+
+Pre-print version of the original paper is freely accessible at the link https://doi.org/10.26434/chemrxiv-2024-rmsnj.
+
+## Documentation
+The installation instructions, documentation and tutorials can be found on http://cosolvkit.readthedocs.io/.
 
 ## Installation
 I highly recommend you to install the Anaconda distribution (https://www.continuum.io/downloads) if you want a clean python environnment with nearly all the prerequisites already installed. To install everything properly, you just have to do this:
 ```bash
 $ conda create -n cosolvkit -c conda-forge -f cosolvkit_env.yml
 ```
 For faster installation, use `mamba` or `micromamba` instead of `conda`.
 
-Finally, we can install the `CosolvKit` package
+Finally, we can install the `CosolvKit` package via `pip`:
+```bash
+$ pip instal cosolvkit
+```
+
+or directly download and install the source code from git: 
+
 ```bash
 $ git clone https://github.com/forlilab/cosolvkit
 $ cd cosolvkit
 $ pip install -e .
 ```
 
 ## Quick tutorial
```

### Comparing `cosolvkit-0.4.1/cosolvkit/analysis.py` & `cosolvkit-0.4.2/cosolvkit/analysis.py`

 * *Files 24% similar despite different names*

```diff
@@ -27,21 +27,39 @@
 from cosolvkit.cosolvent_system import CosolventMolecule
 
 
 BOLTZMANN_CONSTANT_KB = 0.0019872041
 
 
 def _normalization(data, a=0, b=0):
+    """_summary_
+
+    :param data: list of data points
+    :type data: list
+    :param a: int a, defaults to 0
+    :type a: int, optional
+    :param b: int b, defaults to 0
+    :type b: int, optional
+    :return: normalized data
+    :rtype: list
+    """
     min_data = np.min(data)
     max_data = np.max(data)
     return a + ((data - min_data) * (b - a)) / (max_data - min_data)
 
 
 def _smooth_grid_free_energy(gfe, sigma=1):
-    """ Empirical grid free energy smoothing
+    """_summary_
+
+    :param gfe: _description_
+    :type gfe: _type_
+    :param sigma: _description_, defaults to 1
+    :type sigma: int, optional
+    :return: _description_
+    :rtype: _type_
     """
     # We keep only the favorable spots with energy < 0 kcal/mol
     gfe_fav = np.copy(gfe)
     gfe_fav[gfe > 0.] = 0.
     # We smooth the energy a bit
     gfe_fav_smooth = gaussian_filter(gfe_fav, sigma=sigma)
     # Normalize data between the original energy minima value and 0
@@ -120,15 +138,19 @@
         assert (box_size > 0).all(), "Error: grid size cannot contain negative numbers."
 
         sub_grid = _subset_grid(grid, center, box_size, gridsize)
         sub_grid.export(fname)
 
 
 class Analysis(AnalysisBase):
+    """Analysis class to generate density grids
 
+    :param AnalysisBase: Base MDAnalysis class
+    :type AnalysisBase: AnalysisBase
+    """
     def __init__(self, atomgroup, gridsize=0.5, **kwargs):
         super(Analysis, self).__init__(atomgroup.universe.trajectory, **kwargs)
 
         if atomgroup.n_atoms == 0:
             print("Error: no atoms were selected.")
             sys.exit(1)
 
@@ -201,16 +223,28 @@
 
     def export_atomic_grid_free_energy(self, fname, gridsize=0.5, center=None, box_size=None):
         """ Export atomic grid free energy
         """
         _export(fname, self._agfe, gridsize, center, box_size)
 
 class Report:
-    # style.use('ggplot')
+    """Report class. This is the main class that takes care of post MD simulation processing and analysis.
+    """
     def __init__(self, log_file, traj_file, top_file, cosolvents_path):
+        """_summary_
+
+        :param log_file: log file generated by MD Simulation. In CosolvKit this is called statistics.csv
+        :type log_file: str
+        :param traj_file: Trajectory file generated by MD Simulation.
+        :type traj_file: str
+        :param top_file: Topology file generated by CosolvKit.
+        :type top_file: str
+        :param cosolvents_path: path to the json file defining the cosolvents present in the system.
+        :type cosolvents_path: str
+        """
         self.statistics = log_file
         self.trajectory = traj_file
         self.topology = top_file
         self.universe = Universe(self.topology, self.trajectory)
         self.cosolvents = list()
 
         with open(cosolvents_path) as fi:
@@ -221,28 +255,40 @@
         self._volume = None
         self._temperature = None
         self._potential_energy = None
         self._potential_energy, self._temperature, self._volume = self._get_temp_vol_pot(self.statistics)
         return
     
     def generate_report(self, out_path):
+        """Creates the main plots for RDFs, autocorrelations and equilibration.
+
+        :param out_path: path to where to save the results. 
+        :type out_path: str
+        """
         print("Generating report...")
         # setup results folders
         report_path = os.path.join(out_path, "report")
         rdf_path = os.path.join(report_path, "rdf")
         os.makedirs(report_path, exist_ok=True)
         os.makedirs(rdf_path, exist_ok=True)
 
         # Generate equilibration plot
         self._plot_temp_vol_pot(report_path)
         print("Plotting RDFs")
         self._rdf_mda(self.universe, self.cosolvents, rdf_path)
         return
     
     def generate_density_maps(self, out_path, analysis_selection_string=""):
+        """Generates the desnity maps for the target cosolvents.
+
+        :param out_path: path to where to save the density files.
+        :type out_path: str
+        :param analysis_selection_string: MD Analysis selection string if want to generate densities only for specific molecules, defaults to ""
+        :type analysis_selection_string: str, optional
+        """
         print("Generating density maps...")
         os.makedirs(out_path, exist_ok=True)
         volume = self._volume[-1]
         temperature = self._temperature[-1]
         if analysis_selection_string == "":
             print("No cosolvent specified for the densities analysis. Generating a density map for each cosolvent.")
             for cosolvent in self.cosolvents:
@@ -258,14 +304,27 @@
                                volume=volume,
                                temperature=temperature,
                                out_path=out_path,
                                cosolvent_name=None)
         return
     
     def generate_pymol_reports(self, topology, trajectory, density_files, selection_string, out_path):
+        """Generate the PyMol reports from the density maps.
+
+        :param topology: Topology generated by CosolvKit.
+        :type topology: str
+        :param trajectory: Trajectory generated by MD Simulation.
+        :type trajectory: str
+        :param density_files: list of density files to include in the same PyMol session. Limited to 5.
+        :type density_files: list
+        :param selection_string: PyMol selection string if willing to specify target residues.
+        :type selection_string: str
+        :param out_path: path to where to save the PyMol session.
+        :type out_path: str
+        """
         colors = ['marine', 
                   'orange', 
                   'magenta',
                   'salmon',
                   'purple']
         
         assert len(density_files) < len(colors), "Error! Too many density files, not enough colors available!"
@@ -327,36 +386,60 @@
         with open(os.path.join(out_path, "pymol_session_cmd.pml"), "w") as fo:
             fo.write(cmd_string)
             
         cmd.save(os.path.join(out_path, "pymol_results_session.pse"))
         return
     
     def _run_analysis(self, selection_string, volume, temperature, out_path, cosolvent_name=None):
+        """Creates Analysis object and generates densities.
+
+        :param selection_string: MD Analysis selection string.
+        :type selection_string: str
+        :param volume: volume of the system.
+        :type volume: float
+        :param temperature: temperature of the system.
+        :type temperature: float
+        :param out_path: path to where to save the results.
+        :type out_path: str
+        :param cosolvent_name: name of the cosolvent if not analysing all the cosolvents in the system, defaults to None
+        :type cosolvent_name: str, optional
+        """
         fig_density_name = os.path.join(out_path, f"map_density.dx")
         fig_energy_name =  os.path.join(out_path, f"map_agfe.dx")
         if cosolvent_name is not None:
             fig_density_name = os.path.join(out_path, f"map_density_{cosolvent_name}.dx")
             fig_energy_name =  os.path.join(out_path, f"map_agfe_{cosolvent_name}.dx")
         analysis = Analysis(self.universe.select_atoms(selection_string), verbose=True)
         analysis.run()
         analysis.atomic_grid_free_energy(volume, temperature)
         analysis.export_density(fig_density_name)
         analysis.export_atomic_grid_free_energy(fig_energy_name)
         self.density_file = fig_density_name
         return
 
     def _get_temp_vol_pot(self, log_file):
+        """Returns temperature, volume and potential energy of the system during the MD simulation.
+
+        :param log_file: log file generated by the MD simulation. In CosolvKit is statistics.csv.
+        :type log_file: str
+        :return: potential energy, temperature and volume of the system for each frame.
+        :rtype: tuple(list, list, list)
+        """
         df = pd.read_csv(log_file)
         pot_e = list(df["Potential Energy (kJ/mole)"])
         temp = list(df["Temperature (K)"])
         vol = list(df["Box Volume (nm^3)"])
         return pot_e, temp, vol
 
     def _plot_temp_vol_pot(self, outpath=None):
+        """Plots equilibration data.
 
+        :param outpath: path to where to save the plot, defaults to None
+        :type outpath: str, optional
+        """
         if outpath is not None:
             fig_name = f"{outpath}/simulation_statistics.png"
 
         fig, axs = plt.subplots(3, 1, figsize=(12, 6))
 
         axs[0].plot(self._potential_energy, color='green', linewidth=2)
         axs[0].set_title('Potential Energy',)
@@ -376,14 +459,23 @@
         plt.tight_layout()
         plt.savefig(fig_name)
         plt.close()
 
         return 
     
     def _rdf_mda(self, universe: Universe, cosolvents: list, outpath=None):
+        """Generates the plots for RDFs and Autocorrelations.
+
+        :param universe: MD Analysis Universe that is created from the topology and trajectories.
+        :type universe: Universe
+        :param cosolvents: list of cosolvents in the system
+        :type cosolvents: list
+        :param outpath: path to where to save the plots, defaults to None
+        :type outpath: str, optional
+        """
         np.seterr(divide='ignore', invalid='ignore')
         wat_resname = "HOH"
         # if top.endswith("cosolv_system.prmtop"):
         #     wat_resname = "WAT"
         oxygen_atoms = universe.select_atoms(f"resname {wat_resname} and name O")
         sim_frames = len(universe.trajectory)
         step_size = int(sim_frames/250)
@@ -463,23 +555,43 @@
             item.set_visible(False)
         if outpath is not None:
             plt.savefig(f"{outpath}/rdf_HOH_O.png")
         plt.close()
         return
 
     def _autocorrelation(self, data):        
-        """Autocorrelation function"""
+        """Gets the autocorrelation values.
+
+        :param data: list of data for which the autocorrelation has to be computed.
+        :type data: list
+        :return: list of autocorrelations.
+        :rtype: list
+        """
         n = len(data)
         mean = np.mean(data)
         autocorr = correlate(data - mean, data - mean, mode='full', method='auto')
         return autocorr[n - 1:]
     
     def _plot_autocorrelation(self, data, ax, cosolvent_name1=None, cosolvent_atom1=None, cosolvent_name2=None, cosolvent_atom2=None):
-        """
+        """Plots autocorrelations.
 
+        :param data: list of data points for which we want to plot autocorrelations.
+        :type data: list
+        :param ax: matplotlib axis to add the autocorrelation to the RDF plot.
+        :type ax: matplotlib.pyplot.axisß
+        :param cosolvent_name1: name of the first cosolvent molecule, defaults to None
+        :type cosolvent_name1: str, optional
+        :param cosolvent_atom1: name of the first atom, defaults to None
+        :type cosolvent_atom1: str, optional
+        :param cosolvent_name2: name of the second cosolvent molecule, defaults to None
+        :type cosolvent_name2: str, optional
+        :param cosolvent_atom2: name of the second atom, defaults to None
+        :type cosolvent_atom2: str, optional
+        :return: the axis with the autocorrelation plot
+        :rtype: matplotlib.pyplot.axis
         """
         title = f"{cosolvent_name1} {cosolvent_atom1}-{cosolvent_name2} {cosolvent_atom2}"
         data = data[0::2]
         autocorr_values = self._autocorrelation(data)
         # Normalize autocorrelation values for better plotting
         normalized_autocorr = autocorr_values / np.max(np.abs(autocorr_values))
         lags = np.arange(0, len(autocorr_values))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cosolvkit-0.4.1/cosolvkit/config.py` & `cosolvkit-0.4.2/cosolvkit/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import os
 import json
 from inspect import signature
 
 class Config(object):
+    """This class handles the config.json options and the whole Cosolvent setup.
+
+    :param object: inherits from the base class
+    :type object: object
+    """
     def __init__(self, 
                  cosolvents=None,
                  forcefields=None,
                  md_format=None,
                  receptor=True,
                  protein_path=None,
                  clean_protein=True,
@@ -50,23 +55,36 @@
         self.radius = radius
         self.output = output
         self.run_cosovlent_system = run_cosolvent_system
         self.run_md = run_md
     
     @classmethod
     def get_defaults_dict(cls):
+        """Returns a dictionary of all the class attributes
+
+        :return: dictionary of class attributes
+        :rtype: dict
+        """
         defaults = {}
         sig = signature(cls)
         for key in sig.parameters:
             defaults[key] = sig.parameters[key].default 
         return defaults
 
         
     @classmethod
     def from_config(cls, config):
+        """Sets up the parameters to run cosolvent from the config.json file supplied.
+
+        :param config: loads the config.json file and populates the class attributes
+        :type config: str
+        :raises ValueError: raises an error if some attributes are not recognized
+        :return: instance of the Config class
+        :rtype: Config
+        """
         expected_keys = cls.get_defaults_dict().keys()
         with open(config) as f:
             config = json.load(f)
         bad_keys = [k for k in config if k not in expected_keys]
         if len(bad_keys) > 0:
             err_msg = "unexpected keys in Config.from_config():" + os.linesep
             for key in bad_keys:
```

### Comparing `cosolvkit-0.4.1/cosolvkit/cosolvent_system.py` & `cosolvkit-0.4.2/cosolvkit/cosolvent_system.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,42 +8,43 @@
 from scipy.stats import qmc
 import math 
 from itertools import product
 import parmed
 from openmm import Vec3, unit, XmlSerializer, System, CustomNonbondedForce, NonbondedForce, OpenMMException
 import openmm.app as app
 import openmm.unit as openmmunit
+import rdkit
 from rdkit import Chem
 from rdkit.Chem import AllChem
 from openff.toolkit import Molecule, Topology
 from openmmforcefields.generators import EspalomaTemplateGenerator, GAFFTemplateGenerator, SMIRNOFFTemplateGenerator
 from openmmforcefields.generators.template_generators import SmallMoleculeTemplateGenerator
 from cosolvkit.utils import fix_pdb, MutuallyExclusiveParametersError
 
 
 proteinResidues = ['ALA', 'ASN', 'CYS', 'GLU', 'HIS', 'LEU', 'MET', 'PRO', 'THR', 'TYR', 'ARG', 'ASP', 'GLN', 'GLY', 'ILE', 'LYS', 'PHE', 'SER', 'TRP', 'VAL']
 rnaResidues = ['A', 'G', 'C', 'U', 'I']
 dnaResidues = ['DA', 'DG', 'DC', 'DT', 'DI']
 
 class CosolventMolecule(object):
-    def __init__(self, name, smiles=None, mol_filename=None, resname=None, copies=None, concentration=None):
-        """Create a Cosolvent object.
-
-        Parameters
-        ----------
-        name : str
-            Name of the molecule.
-        smiles : str, default=None
-            SMILES string of the molecule in the chosen protonation state.
-        mol_filename : str, default=None
-            MOL/SDF filename of the molecule in the chosen protonation state.
-        resname : str, default=None
-            3-letters residue name of the molecule. If None, the first 3 
-            letters of the name will be used as uppercase.
+    def __init__(self, name: str, smiles: str=None, mol_filename: str=None, resname: str=None, copies: int=None, concentration: float=None):
+        """Creates a Cosolvent object.
 
+        :param name: name of the molecule
+        :type name: str
+        :param smiles: SMILES string of the molecule in the chose protonation state, defaults to None
+        :type smiles: str, optional
+        :param mol_filename: MOL/SDF filename of the molecule, defaults to None
+        :type mol_filename: str, optional
+        :param resname: 3-letters residue name of the molecule. If None, the first 3 uppercase letters of the name will be used, defaults to None
+        :type resname: str, optional
+        :param copies: number of copies of cosolvent the user wants to place, defaults to None
+        :type copies: int, optional
+        :param concentration: if the number of copies is unknown the user can specify the concentration in Molar units, defaults to None
+        :type concentration: float, optional
         """
         if resname is None:
             self.resname = name[:3].upper()
         else:
             self.resname = resname
 
         # assert not self.resname in AMBER_SUPPORTED_RESNAMES, f"Error: the residue name {self.resname} is already defined in AMBER."
@@ -100,26 +101,21 @@
         positions = positions - np.mean(positions, axis=0)
         self.positions = positions
         self.mol_filename = mol_filename
         self.pdb_conect = self._get_pdb_conect(mol)
         return
     
     
-    def _generate_atom_names_from_mol(self, rdkit_mol):
-        """Generate atom names from an RDKit molecule.
+    def _generate_atom_names_from_mol(self, rdkit_mol: rdkit.Chem.rdchem.Mol) -> list:
+        """Generates atom names from an RDKit molecule.
 
-        Parameters
-        ----------
-        rdkit_mol : rdkit.Chem.rdchem.Mol
-            RDKit molecule.
-
-        Returns
-        -------
-        list
-            List of atom names.
+        :param rdkit_mol: RDKit molecule
+        :type rdkit_mol: rdkit.Chem.rdchem.Mol
+        :return: list of atom names.
+        :rtype: list
         """
         atom_names = []
         counter = {}
 
         for atom in rdkit_mol.GetAtoms():
             atom_name = atom.GetSymbol()
 
@@ -130,15 +126,22 @@
 
             atom_name += str(counter[atom_name])
             atom_names.append(atom_name)
 
         return atom_names
 
 
-    def _get_pdb_conect(self, rdkit_mol):
+    def _get_pdb_conect(self, rdkit_mol: rdkit.Chem.rdchem.Mol) -> list:
+        """Generates bonds definition (unused)
+
+        :param rdkit_mol: RDKit molecule
+        :type rdkit_mol: rdkit.Chem.rdchem.Mol
+        :return: list of bonds
+        :rtype: list
+        """
         conect = []
 
         pdb_string = Chem.MolToPDBBlock(rdkit_mol)
         pdb_lines = pdb_string.split('\n')
 
         for i, line in enumerate(pdb_lines):
             if 'CONECT' in line:
@@ -150,37 +153,29 @@
     def __init__(self, 
                  cosolvents: dict,
                  forcefields: dict,
                  simulation_format: str, 
                  modeller: app.Modeller,  
                  padding: openmmunit.Quantity = 12*openmmunit.angstrom, 
                  radius: openmmunit.Quantity = None):
+        """Create cosolvent system.
+
+        :param cosolvents: dictionary of cosolvent molecules
+        :type cosolvents: dict
+        :param forcefields: dictionary of forcefields to use
+        :type forcefields: dict
+        :param simulation_format: MD format that want to be used for the simulation. Supported formats: Amber, Gromacs, CHARMM, openMM 
+        :type simulation_format: str
+        :param modeller: openmm modeller created from topology and positions.
+        :type modeller: openmm.app.Modeller
+        :param padding: specifies the padding used to create the simulation box, defaults to 12*openmmunit.angstrom
+        :type padding: openmm.unit.Quantity, optional
+        :param radius: Specifies the radius to create the box without receptor, defaults to None
+        :type radius: openmm.unit.Quantity, optional
         """
-            Create cosolvent system.
-            By default it accepts a pdb string for the receptor, otherwise can call
-            the from_filename method and pass a pdb file path.
-
-            Args:
-                cosolvents : dict
-                    Dictionary of cosolvent molecules
-                forcefields : dict
-                    Dictionary of forcefields to use
-                simulation_format : str
-                    MD format that want to be used for the simulation.
-                    Supported formats: Amber, Gromacs, CHARMM or openMM
-                modeller : app.Modeller
-                    Modeller containing topology and positions information.
-                padding : openmm.unit.Quantity
-                    Specifies the padding used to create the simulation box 
-                    if no receptor is provided. Default to 12 Angstrom
-                radius : openmm.unit.Quantity
-                    Specifies the radius to create the box without receptor.
-                    Default is None
-        """ 
-        
         # Private
         self._available_formats = ["AMBER", "GROMACS", "CHARMM", "OPENMM"]
         self._cosolvent_positions = defaultdict(list)
         self._box = None
         self._periodic_box_vectors = None
         self._box_volume = None
         self._padding = padding
@@ -222,67 +217,31 @@
         self.box_volume = vX * vY * vZ
         print("Parametrizing system with forcefields")
         self.forcefield = self._parametrize_system(forcefields, simulation_format, self.cosolvents)
         print(f"Box Volume: {self.box_volume} nm**3")
         print(f"\t{self.box_volume*1000} A^3")
         return
     
-    # @classmethod
-    # def from_filename(cls, 
-    #                   cosolvents: str,
-    #                   forcefields: str,
-    #                   simulation_format: str, 
-    #                   receptor: str,  
-    #                   padding: openmmunit.Quantity = 12*openmmunit.angstrom,
-    #                   clean_protein: bool=True):
-    #     """
-    #         Create a CosolventSystem with receptor from the pdb file path.
-
-    #         Args:
-    #                 cosolvents : str
-    #                     Path to the cosolvents.json file
-    #                 forcefields : str
-    #                     Path to the forcefields.json file
-    #                 simulation_format : str
-    #                     MD format that want to be used for the simulation.
-    #                     Supported formats: Amber, Gromacs, CHARMM or openMM
-    #                 receptor : None | str
-    #                     PDB string of the protein. 
-    #                     By default is None to allow cosolvent
-    #                     simulations without receptor
-    #                 padding : openmm.unit.Quantity
-    #                     Specifies the padding used to create the simulation box 
-    #                     if no receptor is provided. Default to 12 Angstrom
-    #                 radius : openmm.unit.Quantity
-    #                     Specifies the radius to create the box without receptor.
-    #                     Default is None
-    #                 clean_protein : bool
-    #                     Determines if the protein will be cleaned and prepared
-    #                     with PDBFixer or not.
-    #                     Default is False
-    #     """
-    #     with open(receptor) as fi:
-    #         pdb_string = fi.read()
-    #     return cls(cosolvents, forcefields, simulation_format, io.StringIO(pdb_string), padding, None, clean_protein)
-    
 #region Public
     def build(self,
               solvent_smiles: str="H2O", 
               n_solvent_molecules: int=None,
               neutralize: bool=True):
         """This function adds thd cosolvents specified in the CosolvSystem
         and solvates with the desired solvent. If n_solvent_molecules is not passed
         the function will try to fill the box with the desired solvent to a certain extent.
         Please note that the solvation with solvents different from water may highly impact
         the execution time.
 
-        Args:
-            solvent_smiles (str, optional): smiles string defining the desired solvent to use. Defaults to "H2O".
-            n_solvent_molecules (int, optional): number of mulecules of solvent to add. Defaults to None.
-            neutralize (bool, optional): if True, the system charge will be neutralized by OpenMM. Defaults to True.
+        :param solvent_smiles: smiles string defining the desired solvent to use, defaults to "H2O"
+        :type solvent_smiles: str, optional
+        :param n_solvent_molecules: number of molecules of solvent to add, defaults to None
+        :type n_solvent_molecules: int, optional
+        :param neutralize: if True, the system charge will be neutralized by OpenMM, defaults to True
+        :type neutralize: bool, optional
         """
         volume_not_occupied_by_cosolvent = self.fitting_checks()
         assert volume_not_occupied_by_cosolvent is not None, "The requested volume for the cosolvents exceeds the available volume! Please try increasing the box padding or radius."
         receptor_positions = self.modeller.positions.value_in_unit(openmmunit.nanometer)
         cosolv_xyzs = self.add_cosolvents(self.cosolvents, self.vectors, self.lowerBound, self.upperBound, receptor_positions)
         self.modeller = self._setup_new_topology(cosolv_xyzs, self.modeller.topology, self.modeller.positions)
         if solvent_smiles == "H2O":
@@ -307,21 +266,22 @@
             solv_xyz = self.add_cosolvents(d_mol, self.vectors, self.lowerBound, self.upperBound, self.modeller.positions)
             self.modeller = self._setup_new_topology(solv_xyz, self.modeller.topology, self.modeller.positions)
             
         self.system = self._create_system(self.forcefield, self.modeller.topology)
         return
     
     def add_repulsive_forces(self, residues_names: list, epsilon: float=0.01, sigma: float=10.0):
-        """
-            This function adds a LJ repulsive potential between the specified molecules.
+        """This function adds a LJ repulsive potential between the specified molecules.
 
-            Args:
-                residues_names (list): list of residue names.
-                epsilon (float): depth of the potential well in kcal/mol (default: 0.01 kcal/mol)
-                sigma (float): inter-particle distance in Angstrom (default: 10 A)      
+        :param residues_names: list of residue names
+        :type residues_names: list
+        :param epsilon: depth of the potential well in kcal/mol, defaults to 0.01
+        :type epsilon: float, optional
+        :param sigma: inter-particle distance in Angstrom, defaults to 10.0
+        :type sigma: float, optional
         """
         epsilon = np.sqrt(epsilon * epsilon) * openmmunit.kilocalories_per_mole
         sigma = sigma * openmmunit.angstrom
 
         forces = { force.__class__.__name__ : force for force in self.system.getForces()}
         nb_force = forces['NonbondedForce']
         cutoff_distance = nb_force.getCutoffDistance()
@@ -359,61 +319,68 @@
         self.system.addForce(repulsive_force)
 
         return
 
     def save_pdb(self, topology: app.Topology, positions: list, out_path: str):
         """Saves the specified topology and position to the out_path file.
 
-        Args:
-            topology (app.Topology): topology used
-            positions (list): list of 3D coords
-            out_path (str): path to where to save the file
+        :param topology: topology used
+        :type topology: openmm.app.Topology
+        :param positions: list of 3D coords
+        :type positions: list
+        :param out_path: path to where to save the dile
+        :type out_path: str
         """
         app.PDBFile.writeFile(
             topology,
             positions,
             open(out_path, "w"),
             keepIds=True
         )
         return
 
     def save_system(self, out_path: str, system: System):
         """Saves the openmm system to the desired out path.
 
-        Args:
-            out_path (str): path where to save the System
-            system (System): system to be saved
+        :param out_path: path where to save the System
+        :type out_path: str
+        :param system: system to save
+        :type system: openmm.System
         """
         with open(f"{out_path}/system.xml", "w") as fo:
             fo.write(XmlSerializer.serialize(system))
         return
     
     def load_system(self, system_path: str) -> System:
-        """Loads the desired system.
-
-        Args:
-            system_path (str): path to the system file
+        """Loads the specified openmm system.
 
-        Returns:
-            System: system
+        :param system_path: path to the system file.
+        :type system_path: str
+        :return: a system instance.
+        :rtype: openmm.System
         """
         with open(system_path) as fi:
             system = XmlSerializer.deserialize(fi.read())
         return system
 
     def save_topology(self, topology: app.Topology, positions: list, system: System, simulation_format: str, forcefield: app.ForceField, out_path: str):
         """Save the topology files necessary for MD simulations according to the simulation engine specified.
 
-        Args:
-            topology (app.Topology): openmm topology 
-            positions (list): list of 3D coordinates of the topology
-            system (System): openmm system
-            simulation_format (str): name of the simulation engine
-            forcefield (app.Forcefield): openmm forcefield
-            out_path (str): output path to where to save the topology files
+        :param topology: openmm topology
+        :type topology: openmm.app.Topology
+        :param positions: list of 3D coordinates
+        :type positions: list
+        :param system: openmm system
+        :type system: openmm.System
+        :param simulation_format: name of the simulation engine
+        :type simulation_format: str
+        :param forcefield: openmm forcefield
+        :type forcefield: openmm.app.ForceField
+        :param out_path: output path to where to save the topology files
+        :type out_path: str
         """
         new_system = forcefield.createSystem(topology,
                                              nonbondedMethod=app.PME,
                                              nonbondedCutoff=10*openmmunit.angstrom,
                                              removeCMMotion=False,
                                              rigidWater=False,
                                              hydrogenMass=3.0*openmmunit.amu)
@@ -444,42 +411,43 @@
 #endregion
     
 #region Private
 #region Misc
     def _copies_from_concentration(self, water_volume: float):
         """Computes the number of copies of cosolvent necessary to reach the desired concentration
 
-        Args:
-            water_volume (float): volume available to be filled with cosolvents.
+        :param water_volume: volume available to be filled with cosolvents
+        :type water_volume: float
         """
         for cosolvent in self.cosolvents:
             if cosolvent.concentration is not None:
                 cosolvent.copies = int(math.floor((((cosolvent.concentration*openmmunit.molar)*(water_volume*openmmunit.liters))*openmmunit.AVOGADRO_CONSTANT_NA) + 0.5))
         return
 
     
     def _get_n_waters(self) -> int:
-        """Returns the number of waters in the system
+        """Returns the number of waters in the system.
 
-        Returns:
-            int: number of waters in the system
+        :return: number of waters in the system
+        :rtype: int
         """
         res = [r.name for r in self.modeller.topology.residues()]
         return res.count('HOH')
     
     def _setup_new_topology(self, cosolvents_positions: dict, receptor_topology: app.Topology = None, receptor_positions:list = None) -> app.Modeller:
         """Returns a new modeller with the topolgy with the new molecules specified
 
-        Args:
-            cosolvents_positions (dict): keys are cosolvent molecules and values are lists of position of the new molecules to add
-            receptor_topology (app.Topology, optional): old topology to which add the new molecules. Defaults to None.
-            receptor_positions (list, optional): old positions to which add the new molecules. Defaults to None.
-
-        Returns:
-            app.Modeller: new modeller containing combined topology and positions
+        :param cosolvents_positions: keys are cosolvent molecules and values are lists of position of the new molecules to add
+        :type cosolvents_positions: dict
+        :param receptor_topology: old topology to which add the new molecules, defaults to None
+        :type receptor_topology: openmm.app.Topology, optional
+        :param receptor_positions: old positions to which add the new molecules, defaults to None
+        :type receptor_positions: list, optional
+        :return: new modeller containing combined topology and positions
+        :rtype: openmm.app.Modeller
         """
         new_mod = None
         last_res_id = 0
         
         # Add the receptor first if present
         if receptor_topology is not None and receptor_positions is not None and len(receptor_positions) > 0: 
             new_mod = app.Modeller(receptor_topology, receptor_positions)
@@ -511,19 +479,21 @@
             
         new_mod.topology.setPeriodicBoxVectors(self._periodic_box_vectors)
         return new_mod
     
     def _to_openmm_topology(self, off_topology: Topology, starting_id: int) -> app.Topology:
         """Converts an openff topology to openmm without specifying a different chain for each residue.
 
-        Args:
-            topology (Topology): Openff Topology
-
-        Returns:
-            app.Topology: returns the corresponding openmm Topology.
+        :param off_topology: Openff Topology
+        :type off_topology: openff.Topology
+        :param starting_id: starting index
+        :type starting_id: int
+        :raises RuntimeError: if something goes wrong
+        :return: openmm topology
+        :rtype: openmm.app.Topology
         """
         from openff.toolkit.topology.molecule import Bond
 
         omm_topology = app.Topology()
 
         off_topology._ensure_unique_atom_names("residues")
 
@@ -640,20 +610,20 @@
 
             omm_topology.setPeriodicBoxVectors(to_openmm(off_topology.box_vectors))
         return omm_topology
             
     def _create_system(self, forcefield: app.forcefield, topology: app.Topology) -> System:
         """Returns system created from the Forcefield and the Topology.
 
-        Args:
-            forcefield (app.forcefield): Forcefield(s) used to build the system
-            topology (app.Topology): Topology used to build the system 
-
-        Returns:
-            System: created system
+        :param forcefield: forcefield(s) used to build the system
+        :type forcefield: openmm.app.forcefield
+        :param topology: topology used to build the system
+        :type topology: openmm.app.Topology
+        :return: the new system
+        :rtype: openmm.System
         """
         print("Creating system")
         system = forcefield.createSystem(topology,
                                          nonbondedMethod=app.PME,
                                          nonbondedCutoff=10*openmmunit.angstrom,
                                          switchDistance=9*openmmunit.angstrom,
                                          removeCMMotion=True,
@@ -669,23 +639,26 @@
                        upperBound: openmmunit.Quantity | Vec3,
                        receptor_positions: list) -> dict:
         """This function adds the desired number of cosolvent molecules using the halton sequence
         to generate random uniformly distributed points inside the grid where to place the cosolvent molecules.
         At first, if a receptor/protein is present the halton sequence points that would clash with the protein
         are pruned.
 
-        Args:
-            cosolvents (dict): keys are cosolvent molecules and values are 3D coordinates of the molecule
-            vectors (tuple[Vec3, Vec3, Vec3]): vectors defining the simulation box
-            lowerBound (openmmunit.Quantity | Vec3): lower bound of the simulation box
-            upperBound (openmmunit.Quantity | Vec3): upper bound of the simulation box
-            receptor_positions (list): 3D coordinates of the receptor
-
-        Returns:
-            dict: keys are cosolvent molecules and values are 3D coordinates of the newly added cosolvents molecules
+        :param cosolvents: keys are cosolvent molecules and values are 3D coordinates of the molecule
+        :type cosolvents: dict
+        :param vectors: vectors defining the simulation box
+        :type vectors: tuple[openmm.Vec3, openmm.Vec3, openmm.Vec3]
+        :param lowerBound: lower bound of the simulation box
+        :type lowerBound: openmm.unit.Quantity | Vec3
+        :param upperBound: upper bound of the simulation box
+        :type upperBound: openmm.unit.Quantity | Vec3
+        :param receptor_positions: list of 3D coordinates of the receptor
+        :type receptor_positions: list
+        :return: keys are cosolvent molecules and values are 3D coordinates of the newly added cosolvent molecules
+        :rtype: dict
         """
         edge_cutoff = 2.5*openmmunit.angstrom
         prot_kdtree = None
         # This is used to update the kdtree of the placed cosolvents
         placed_atoms_positions = []
         if receptor_positions is not None and len(receptor_positions) > 0:
             prot_kdtree = spatial.cKDTree(receptor_positions)
@@ -753,23 +726,23 @@
 
 
         return used_halton_ids+list(close_to)
 
     def check_coordinates_to_add(self, new_coords: np.ndarray, cosolvent_kdtree: spatial.cKDTree, protein_kdtree: spatial.cKDTree) -> bool:
         """Checks that the new coordinates don't clash with the receptor (if present) and/or other cosolvent molecules
 
-        Args:
-            new_coords (np.ndarray): coordinates of the new molecule of shape (n, 3)
-            cosolvent_kdtree (spatial.cKDTree): binary tree of the cosolvent molecules present in the box
-            protein_kdtree (spatial.cKDTree): binary tree of the receptor's coordinates
-
-        Returns:
-            bool: True if there are no clashes False otherwise
+        :param new_coords: coordinates of the new molecule of shape (n, 3)
+        :type new_coords: np.ndarray
+        :param cosolvent_kdtree: tree of the cosolvent molecules present in the box
+        :type cosolvent_kdtree: spatial.cKDTree
+        :param protein_kdtree: tree of the receptor's coordinates
+        :type protein_kdtree: spatial.cKDTree
+        :return: True if there are no clashes, False otherwise
+        :rtype: bool
         """
-        
         cosolvent_clashes = False
         protein_clashes = False
         check_clashes = cosolvent_kdtree is not None or protein_kdtree is not None
         if cosolvent_kdtree is not None:
             cosolvent_clashes = any(cosolvent_kdtree.query_ball_point(new_coords, self.cosolvents_radius.value_in_unit(openmmunit.nanometer)))
         if protein_kdtree is not None:
             protein_clashes = any(protein_kdtree.query_ball_point(new_coords, self.protein_radius.value_in_unit(openmmunit.nanometer)))
@@ -790,27 +763,31 @@
                       protein_kdtree: spatial.cKDTree) -> tuple[np.ndarray, list]:
         """Accepts or reject the halton move. A random halton point is selected and checked, if accepted
         the cosolvent is placed there, otherwise a local search is performed in the neighbors of the point 
         (1 tile). If the local search produces no clashes the new position is accepted, otherwise a new 
         random halton point is selected and the old one is marked as not good. The algorithm stops
         when a move is accepted or 1000000 of trials are done and no move is accepted.
 
-        Args:
-            xyz (np.ndarray): 3D coordinates of the cosolvent molecule
-            halton (list): halton sequence
-            kdtree (spatial.cKDTree): binary tree of the cosolvent molecules positions already placed in the box
-            valid_ids (list): valid halton indices
-            lowerBound (openmmunit.Quantity | Vec3): lower bound of the box
-            upperBound (openmmunit.Quantity | Vec3): upper bound of the box
-            protein_kdtree (spatial.cKDTree): binary tree of the protein's positions
-
-        Returns:
-            tuple[np.ndarray, list]: accepted coordinates for the cosolvent and the used halton ids
-        """
-        
+        :param xyz: 3D coordinates of the cosolvent molecule
+        :type xyz: np.ndarray
+        :param halton: halton sequence
+        :type halton: list
+        :param kdtree: tree of the cosolvent molecules positions already placed in the box
+        :type kdtree: spatial.cKDTree
+        :param valid_ids: valid halton indices
+        :type valid_ids: list
+        :param lowerBound: lower bound of the box
+        :type lowerBound: openmm.unit.Quantity | Vec3
+        :param upperBound: upper bound of the box
+        :type upperBound: openmm.unit.Quantity | Vec3
+        :param protein_kdtree: tree of the protein's positions
+        :type protein_kdtree: spatial.cKDTree
+        :return: accepted coordinates for the cosolvent and the used halton ids
+        :rtype: tuple[np.ndarray, list]
+        """        
         trial = 0
         accepted = False
         coords_to_return = 0
         moves = self.local_search()
         while not accepted and trial < 1000000:
             halton_idx = np.random.choice(len(valid_ids))
             rotated_xyz = self.generate_rotation(xyz)
@@ -835,21 +812,22 @@
 
     def is_in_box(self, 
                   xyzs: np.ndarray, 
                   lowerBound: openmmunit.Quantity | Vec3, 
                   upperBound: openmmunit.Quantity | Vec3) -> bool:
         """Checks if the coordinates are in the box or not
 
-        Args:
-            xyzs (np.ndarray): coordinates to check
-            lowerBound (openmmunit.Quantity | Vec3): lower bound of the box
-            upperBound (openmmunit.Quantity | Vec3): upper bound of the box
-
-        Returns:
-            bool: True if all the coordinates are in the box, False otherwise
+        :param xyzs: coordinates to check
+        :type xyzs: np.ndarray
+        :param lowerBound: lower bound of the box
+        :type lowerBound: openmmunit.Quantity | Vec3
+        :param upperBound: upper bound of the box
+        :type upperBound: openmmunit.Quantity | Vec3
+        :return: True if all the coordinates are in the box, Flase otherwise
+        :rtype: bool
         """
         # cutoff = (1.5*openmmunit.angstrom).value_in_unit(openmmunit.nanometer)
         xyzs = np.atleast_2d(xyzs)
         x, y, z = xyzs[:, 0], xyzs[:, 1], xyzs[:, 2]
 
         xmin, xmax = lowerBound[0], upperBound[0][0]
         ymin, ymax = lowerBound[1], upperBound[1][1]
@@ -861,28 +839,29 @@
         all_in = np.all((x_in, y_in, z_in), axis=0)
 
         return np.all(all_in)
 
     def local_search(self) -> list:
         """Return all the possible moves in the 1 tile neighbors
 
-        Returns:
-            list: combinations
+        :return: combinations
+        :rtype: list
         """
         step = 1
         moves = filter(lambda point: not all(axis ==0 for axis in point), list(product([-step, 0, step], repeat=3)))
         return moves
 
     def generate_rotation(self, coords: np.ndarray) -> np.ndarray:
-        """ Rotate a list of 3D [x,y,z] vectors about corresponding random uniformly
+        """Rotate a list of 3D [x,y,z] vectors about corresponding random uniformly
             distributed quaternion [w, x, y, z]
-        Args:
-            coords (np.ndarray) with shape [n,3]: list of [x,y,z] cartesian vector coordinates
-        Returns:
-            np.ndarray: rotated coordinates
+
+        :param coords: list of [x, y, z] cartesian vector coordinates
+        :type coords: np.ndarray
+        :return: rotated coordinates
+        :rtype: np.ndarray
         """
         rand = np.random.rand(3)
         r1 = np.sqrt(1.0 - rand[0])
         r2 = np.sqrt(rand[0])
         pi2 = math.pi * 2.0
         t1 = pi2 * rand[1]
         t2 = pi2 * rand[2]
@@ -894,19 +873,18 @@
         return rotation.apply(coords)
     
 #region SizeChecks
     def calculate_mol_volume(self, mol_positions: np.ndarray) -> float:
         """Calculates the volume occupied by the 3D coordinates provided based
         on voxelization.
 
-        Args:
-            mol_positions (np.ndarray): 3D coordinates
-
-        Returns:
-            float: volume occupied in nm**3
+        :param mol_positions: 3D coordinates of the molecule
+        :type mol_positions: np.ndarray
+        :return: volume occupied in nm**3
+        :rtype: float
         """
         padding = 3.5*openmmunit.angstrom
         offset = 1.5*openmmunit.angstrom
         mesh_step = 0.3*openmmunit.angstrom
         padding = padding.value_in_unit(openmmunit.nanometer)
         offset = offset.value_in_unit(openmmunit.nanometer)
         mesh_step = mesh_step.value_in_unit(openmmunit.nanometer)
@@ -925,16 +903,16 @@
         return round(len(points)*mesh_step**3, 2)
 
     def fitting_checks(self) -> float | None:
         """Checks if the required cosolvents can fit in the box and 
         do not exceed the 50% of the available fillable volume 
         (volume not occupied by the receptor, if present).
 
-        Returns:
-            float | None: available volume if the cosolvents can fit, None otherwise
+        :return: available volume if the cosolvents can fit, None otherwise
+        :rtype: float | None
         """
         prot_volume = 0
         if self.receptor:
             prot_volume = self.calculate_mol_volume(self.modeller.positions)
             prot_volume = prot_volume
             print(f"Volume protein: {prot_volume*1000} A^3")
         empty_volume = self.cubic_nanometers_to_liters(self.box_volume - prot_volume)
@@ -949,67 +927,66 @@
         if volume_occupied_by_cosolvent > empty_available_volume:
             return None
         return empty_available_volume
 
     def liters_to_cubic_nanometers(self, liters: float | openmmunit.Quantity) -> float:
         """Converts liters in cubic nanometers
 
-        Args:
-            liters (float | openmmunit.Quantity): volume to convert
-
-        Returns:
-            float: converted volume 
+        :param liters: volume to convert
+        :type liters: float | openmm.unit.Quantity
+        :return: converted volume
+        :rtype: float
         """
         if isinstance(liters, openmmunit.Quantity):
             liters = liters.value_in_unit(openmmunit.liters)
         value = liters * 1e+24
         return value
 
     def cubic_nanometers_to_liters(self, vol: float) -> float:
         """Converts cubic nanometers in liters
 
-        Args:
-            vol (float): volume to convert
-
-        Returns:
-            float: converted volume
+        :param vol: volume to convert
+        :type vol: float
+        :return: converted volume
+        :rtype: float
         """
         value = vol * 1e-24
         return value
 #endregion
 #endregion                
 
 #region ForceFieldParametrization
     def _parametrize_system(self, forcefields: dict, engine: str, cosolvents: dict) -> app.ForceField:
         """Parametrize the system with the specified forcefields
 
-        Args:
-            forcefields (dict): dictionary the forcefields to use
-            engine (str): name of the simulation engine
-            cosolvents (dict): cosolvent molecules
-
-        Returns:
-            app.ForceField: forcefield obj
+        :param forcefields: dictionary of the forcefields to use (from forcefields.json)
+        :type forcefields: dict
+        :param engine: name of the simulation engine to use
+        :type engine: str
+        :param cosolvents: cosolvent moleucles (from cosolvents.json)
+        :type cosolvents: dict
+        :return: forcefield object
+        :rtype: openmm.app.ForceField
         """
         engine = engine.upper()
         forcefield = app.ForceField(*forcefields[engine])
         sm_ff = forcefields["small_molecules"][0]
         small_molecule_ff = self._parametrize_cosolvents(cosolvents, small_molecule_ff=sm_ff)
         forcefield.registerTemplateGenerator(small_molecule_ff.generator)
         return forcefield
 
     def _parametrize_cosolvents(self, cosolvents: dict, small_molecule_ff="espaloma") -> SmallMoleculeTemplateGenerator:
         """Parametrizes cosolvent molecules according to the forcefiled specified.
 
-        Args:
-            cosolvents (dict): cosolvents specified
-            small_molecule_ff (str, optional): name of the forcefield to use. Defaults to "espaloma".
-
-        Returns:
-            SmallMoleculeTemplateGenerator: forcefiled obj
+        :param cosolvents: cosolvents specified
+        :type cosolvents: dict
+        :param small_molecule_ff: name of the forcefield to use, defaults to "espaloma"
+        :type small_molecule_ff: str, optional
+        :return: forcefield object for the small molecules
+        :rtype: SmallMoleculeTemplateGenerator
         """
         molecules = list()
         for cosolvent in cosolvents:
             try:
                 molecules.append(Molecule.from_smiles(cosolvent.smiles, name=cosolvent.name))
             except Exception as e:
                 print(e)
@@ -1031,24 +1008,24 @@
                                                                 Vec3, 
                                                                 openmmunit.Quantity | Vec3,
                                                                 openmmunit.Quantity | Vec3]:
         """Builds the simulation box. If a receptor is passed it is used alongside with the padding
         parameter to build the box automatically, otherwise a radius has to be passed. If no receptor
         the box is centered on the point [0, 0, 0].
 
-        Args:
-            positions (np.ndarray): coordinates of the receptor if present
-            padding (openmmunit.Quantity): padding to be used
-            radius (openmmunit.Quantity, optional): radius specified if no receptor is passed. Defaults to None.
-
-        Returns:
-            tuple[tuple[Vec3, Vec3, Vec3], Vec3, openmmunit.Quantity | Vec3, openmmunit.Quantity | Vec3]: 
-                The first element returned is a tuple containing the three vectors describing the simulation box.
+        :param positions: coordinates of the receptor if present
+        :type positions: np.ndarray
+        :param padding: padding to be used
+        :type padding: openmm.unit.Quantity
+        :param radius: radius specified if no receptor is passed, defaults to None
+        :type radius: openmm.unit.Quantity, optional
+        :return: The first element returned is a tuple containing the three vectors describing the simulation box.
                 The second element is the box itself.
-                Third and fourth elements are the lower and upper bound of the simulation box. 
+                Third and fourth elements are the lower and upper bound of the simulation box.
+        :rtype: tuple[tuple[Vec3, Vec3, Vec3], Vec3, openmmunit.Quantity | Vec3, openmmunit.Quantity | Vec3]
         """
         padding = padding.value_in_unit(openmmunit.nanometer)
         if positions is not None:
             positions = positions.value_in_unit(openmmunit.nanometer)
             minRange = Vec3(*(min((pos[i] for pos in positions)) for i in range(3)))
             maxRange = Vec3(*(max((pos[i] for pos in positions)) for i in range(3)))
             center = 0.5*(minRange+maxRange)
@@ -1078,39 +1055,35 @@
                  forcefields: str,
                  simulation_format: str, 
                  modeller: app.Modeller,  
                  padding: openmmunit.Quantity = 12*openmmunit.angstrom, 
                  radius: openmmunit.Quantity = None,
                  lipid_type: str=None,
                  lipid_patch_path: str=None):
-        """
-        Creates a CosolventMembraneSystem.
+        """Creates a CosolventMembraneSystem.
 
-        Args:
-            cosolvents (str): Path to the cosolvents.json file
-            forcefields (str): Path to the forcefields.json file
-            simulation_format (str): MD format that want to be used for the simulation.
-                                     Supported formats: Amber, Gromacs, CHARMM or openMM
-            modeller (app.Modeller): Modeller containing topology and positions information.                                                                          
-            padding (openmmunit.Quantity, optional): Specifies the padding used to create the simulation box 
-                                                     if no receptor is provided. Default to 12 Angstrom. 
-                                                     Defaults to 12*openmmunit.angstrom.
-            radius (openmmunit.Quantity, optional): Specifies the radius to create the box without receptor.
-                                                    Defaults to None.
-            clean_protein (bool, optional): Determines if the protein will be cleaned and prepared with PDBFixer or not. 
-                                            Defaults to False.
-            lipid_type (str, optional): Lipid type to use to build the membrane system, 
-                                        supported types: ["POPC", "POPE", "DLPC", "DLPE", "DMPC", "DOPC", "DPPC"]. 
+        :param cosolvents: path to the cosolvents.json file
+        :type cosolvents: str
+        :param forcefields: path to the forcefields.json file
+        :type forcefields: str
+        :param simulation_format: MD format that want to be used for the simulation
+        :type simulation_format: str
+        :param modeller: Modeller containing topology and positions information
+        :type modeller: openmm.app.Modeller
+        :param padding: specify the padding to be used to create the simulation box, defaults to 12*openmmunit.angstrom
+        :type padding: openmm.unit.Quantity, optional
+        :param radius: specifies the radius to create the box without receptor, defaults to None
+        :type radius: openmm.unit.Quantity, optional
+        :param lipid_type: lipid type to use to build the membrane system, defaults to None. Supported types: ["POPC", "POPE", "DLPC", "DLPE", "DMPC", "DOPC", "DPPC"]. 
                                         Mutually exclusive with <lipid_patch_path>.
-                                        Defaults to None.
-            lipid_patch_path (str, optional): If lipid type is None the path to a pre-equilibrated patch of custom
-                                              lipids membrane can be passed. Mutually exclusive with <lipid_type>.
-                                              Defaults to None.
+        :type lipid_type: str, optional
+        :param lipid_patch_path: if lipid type is None the path to a pre-equilibrated patch of custom lipids membrane can be passed, defaults to None. Mutually exclusive with <lipid_type>
+        :type lipid_patch_path: str, optional
+        :raises MutuallyExclusiveParametersError: custom Exception
         """
-        
         super().__init__(cosolvents=cosolvents,
                          forcefields=forcefields,
                          simulation_format=simulation_format,
                          modeller=modeller,
                          padding=padding,
                          radius=radius)
         
@@ -1125,75 +1098,27 @@
         if self.lipid_type is not None and lipid_patch_path is None:
             assert self.lipid_type in self._available_lipids, print(f"Error! The specified lipid is not supported! Please choose between the following lipid types:\n\t{self._available_lipids}")
         elif lipid_patch_path is not None and self.lipid_type is None:
             self.lipid_patch = app.PDBFile(lipid_patch_path)
         else:
             raise MutuallyExclusiveParametersError("Error! <lipid_type> and <lipid_patch_path> are mutually exclusive parameters. Please pass just one of them.")
     
-    # @classmethod
-    # def from_filename(cls, 
-    #                   cosolvents: str,
-    #                   forcefields: str,
-    #                   simulation_format: str, 
-    #                   receptor: str,  
-    #                   padding: openmmunit.Quantity = 12*openmmunit.angstrom,
-    #                   clean_protein: bool=False,
-    #                   lipid_type: str=None,
-    #                   lipid_patch_path: str=None):
-    #     """
-    #     Create a CosolventMembraneSystem with receptor from the pdb file path.
-
-    #     Args:
-    #         cosolvents (str): Path to the cosolvents.json file
-    #         forcefields (str): Path to the forcefields.json file
-    #         simulation_format (str): MD format that want to be used for the simulation.
-    #                                  Supported formats: Amber, Gromacs, CHARMM or openMM
-    #         receptor (str, optional): PDB string of the protein. 
-    #                                   By default is None to allow cosolvent
-    #                                   simulations without receptor. Defaults to None.
-    #         padding (openmmunit.Quantity, optional): Specifies the padding used to create the simulation box 
-    #                                                  if no receptor is provided. Default to 12 Angstrom. 
-    #                                                  Defaults to 12*openmmunit.angstrom.
-    #         clean_protein (bool, optional): Determines if the protein will be cleaned and prepared with PDBFixer or not. 
-    #                                         Defaults to False.
-    #         lipid_type (str, optional): Lipid type to use to build the membrane system, 
-    #                                     supported types: ["POPC", "POPE", "DLPC", "DLPE", "DMPC", "DOPC", "DPPC"]. 
-    #                                     Mutually exclusive with <lipid_patch_path>.
-    #                                     Defaults to None.
-    #         lipid_patch_path (str, optional): If lipid type is None the path to a pre-equilibrated patch of custom
-    #                                           lipids membrane can be passed. Mutually exclusive with <lipid_type>.
-    #                                           Defaults to None.
-    #     """
-    #     with open(receptor) as fi:
-    #         pdb_string = fi.read()
-    #     return cls(cosolvents, 
-    #                forcefields, 
-    #                simulation_format, 
-    #                io.StringIO(pdb_string), 
-    #                padding, 
-    #                None, 
-    #                clean_protein, 
-    #                lipid_type, 
-    #                lipid_patch_path)
-    
     def add_membrane(self, cosolvent_placement: int=0, neutralize: bool=True, waters_to_keep: list=None):
-        """Create the membrane system.
+        """Create a membrane system
 
-        Args:
-            cosolvent_placement (int): Determines on what side of the membrane will the cosolvents be placed.
-                                       * -1: Inside the membrane
-                                       * +1: Outside the membrane
-                                       *  0: Everywhere 
-                                       Defaults to 0.
-            neutralize (bool, optional): If neutralize the system when solvating the membrane. Defaults to True.
-            waters_to_keep (list, optional): A list of the indices of key waters that should not be deleted. 
-                                             Defaults to None.
-
-        Raises:
-            SystemError: If OpenMM is not able to relax the system after adding the membrane a SystemError is raised.
+        :param cosolvent_placement: determines on what side of the membrane will the cosolvents be placed, defaults to 0.
+                                    * -1: inside the membrane
+                                    * +1: outside the membrane
+                                    * 0: everywhere
+        :type cosolvent_placement: int, optional
+        :param neutralize: if neutralize the system when solvating the membrane, defaults to True
+        :type neutralize: bool, optional
+        :param waters_to_keep: a list of the indices of key waters that should not be deleted, defaults to None
+        :type waters_to_keep: list, optional
+        :raises SystemError: if OpenMM is not able to relax the system after adding the membrane a SystemError is raised
         """
         waters_residue_names = ["HOH", "WAT"]
         # OpenMM default
         padding = 1 * openmmunit.nanometer
         self._cosolvent_placement = cosolvent_placement
         if self._cosolvent_placement == 0: print("No preference of what side of the membrane to place the cosolvents")
         elif self._cosolvent_placement == 1: print("Placing cosolvent molecules outside of the membrane")
@@ -1236,20 +1161,18 @@
                                            maxRange[2]-minRange[2]])).astype(int)
         self.lowerBound = center-box/2
         self.upperBound = center+box/2
         self._periodic_box_vectors = self.modeller.topology.getPeriodicBoxVectors().value_in_unit(openmmunit.nanometer)
         return
 
     def build(self, neutralize: bool=True):
-        """
-        Adds the cosolvent molecules to the system.
-
+        """Adds the cosolvent molecules to the system
 
-        Args:
-            neutralize (bool, optional): If neutralize the system during solvation. Defaults to True.
+        :param neutralize: if neutralize the system during solvation, defaults to True
+        :type neutralize: bool, optional
         """
         if self._cosolvent_placement != 0:
             lipid_positions = list()
             atoms = list(self.modeller.topology.atoms())
             positions = self.modeller.positions.value_in_unit(openmmunit.nanometer)
             for i in range(len(atoms)):
                 if atoms[i].residue.name not in proteinResidues and atoms[i].residue.name not in dnaResidues and atoms[i].residue.name not in rnaResidues:
```

### Comparing `cosolvkit-0.4.1/cosolvkit/data/config.json` & `cosolvkit-0.4.2/cosolvkit/data/config.json`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.1/cosolvkit/data/cosolvents.json` & `cosolvkit-0.4.2/cosolvkit/data/cosolvents.json`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.1/cosolvkit/utils.py` & `cosolvkit-0.4.2/cosolvkit/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,88 +18,96 @@
 import mdtraj
 from MDAnalysis import Universe
 from openmm.app import *
 from openmm import *
 import pdbfixer
 
 class MutuallyExclusiveParametersError(Exception):
-        pass   
+    """A custom exception.
 
+    :param Exception: this is a custom exception for mutually exclusive parameters
+    :type Exception: Exception
+    """
+    pass   
 
-def add_harmonic_restraints(prmtop, inpcrd, system, atom_selection, k=1.0):
-    """Add harmonic restraints to the system.
 
-    Args:
-        prmtop (AmberPrmtopFile): Amber topology object
-        inpcrd (AmberInpcrdFile): Amber coordinates object
-        system (System): OpenMM system object created from the Amber topology object
-        atom_selection (str): Atom selection (see MDTraj documentation)
-        k (float): harmonic force restraints in kcal/mol/A**2 (default: 1 kcal/mol/A**2)
+# def add_harmonic_restraints(prmtop, inpcrd, system, atom_selection, k=1.0):
+#     """Add harmonic restraints to the system.
 
-    Returns:
-        (list, int): list of all the atom ids on which am harmonic force is applied, index with the System of the force that was added
+#     Args:
+#         prmtop (AmberPrmtopFile): Amber topology object
+#         inpcrd (AmberInpcrdFile): Amber coordinates object
+#         system (System): OpenMM system object created from the Amber topology object
+#         atom_selection (str): Atom selection (see MDTraj documentation)
+#         k (float): harmonic force restraints in kcal/mol/A**2 (default: 1 kcal/mol/A**2)
 
-    """
-    mdtop = mdtraj.Topology.from_openmm(prmtop.topology)
-    atom_idxs = mdtop.select(atom_selection)
-    positions = inpcrd.positions
+#     Returns:
+#         (list, int): list of all the atom ids on which am harmonic force is applied, index with the System of the force that was added
 
-    # Tranform constant to the right unit
-    k = k * unit.kilocalories_per_mole / unit.angstroms**2
-    k = k.value_in_unit_system(unit.md_unit_system)
+#     """
+#     mdtop = mdtraj.Topology.from_openmm(prmtop.topology)
+#     atom_idxs = mdtop.select(atom_selection)
+#     positions = inpcrd.positions
 
-    if atom_idxs.size == 0:
-        print("Warning: no atoms selected using: %s" % atom_selection)
-        return ([], None)
+#     # Tranform constant to the right unit
+#     k = k * unit.kilocalories_per_mole / unit.angstroms**2
+#     k = k.value_in_unit_system(unit.md_unit_system)
 
-    # Take into accoun the periodic condition
-    # http://docs.openmm.org/latest/api-python/generated/simtk.openmm.openmm.CustomExternalForce.html
-    force = CustomExternalForce("k * periodicdistance(x, y, z, x0, y0, z0)^2")
+#     if atom_idxs.size == 0:
+#         print("Warning: no atoms selected using: %s" % atom_selection)
+#         return ([], None)
+
+#     # Take into accoun the periodic condition
+#     # http://docs.openmm.org/latest/api-python/generated/simtk.openmm.openmm.CustomExternalForce.html
+#     force = CustomExternalForce("k * periodicdistance(x, y, z, x0, y0, z0)^2")
     
-    harmonic_force_idx = system.addForce(force)
+#     harmonic_force_idx = system.addForce(force)
     
-    force.addGlobalParameter("k", k)
-    print(force.getGlobalParameterDefaultValue(0))
-    force.addPerParticleParameter("x0")
-    force.addPerParticleParameter("y0")
-    force.addPerParticleParameter("z0")
+#     force.addGlobalParameter("k", k)
+#     print(force.getGlobalParameterDefaultValue(0))
+#     force.addPerParticleParameter("x0")
+#     force.addPerParticleParameter("y0")
+#     force.addPerParticleParameter("z0")
     
-    for atom_idx in atom_idxs:
-        #print(atom_idx, positions[atom_idx].value_in_unit_system(units.md_unit_system))
-        force.addParticle(int(atom_idx), positions[atom_idx].value_in_unit_system(unit.md_unit_system))
+#     for atom_idx in atom_idxs:
+#         #print(atom_idx, positions[atom_idx].value_in_unit_system(units.md_unit_system))
+#         force.addParticle(int(atom_idx), positions[atom_idx].value_in_unit_system(unit.md_unit_system))
 
-    return atom_idxs
+#     return atom_idxs
 
 
-def update_harmonic_restraints(simulation, k=1.0):
-    """Update harmonic restraints force
+# def update_harmonic_restraints(simulation, k=1.0):
+#     """Update harmonic restraints force
     
-    Args:
-        simulation (Simulation): OpenMM simulation object
-        k (float): new harmonic force constraint in kcal/mol/A**2 (default: 1 kcal/mol/A**2)
+#     Args:
+#         simulation (Simulation): OpenMM simulation object
+#         k (float): new harmonic force constraint in kcal/mol/A**2 (default: 1 kcal/mol/A**2)
 
-    """
-    # Tranform constant to the right unit
-    k = k * unit.kilocalories_per_mole / unit.angstroms**2
-    k = k.value_in_unit_system(unit.md_unit_system)
+#     """
+#     # Tranform constant to the right unit
+#     k = k * unit.kilocalories_per_mole / unit.angstroms**2
+#     k = k.value_in_unit_system(unit.md_unit_system)
     
-    simulation.context.setParameter('k', k)
+#     simulation.context.setParameter('k', k)
 
 def fix_pdb(pdbfile: str, pdbxfile: str, keep_heterogens: bool=False) -> tuple[Topology, list]:
-    """ Fixes common problems in PDB such as:
+    """Fixes common problems in PDB such as:
             - missing atoms
             - missing residues
             - missing hydrogens
             - remove nonstandard residues
-    
-    Args:
-        pdbfile (str): pdb string old format
-        pdbxfile (str): pdb string new format
-        keep_heterogens (bool): if False all the heterogen atoms but waters are deleted.
-                                Defaults to False.
+
+    :param pdbfile: pdb string old format
+    :type pdbfile: str
+    :param pdbxfile: pdb string new format
+    :type pdbxfile: str
+    :param keep_heterogens: if False all heterogen atoms but waters are deleted, defaults to False
+    :type keep_heterogens: bool, optional
+    :return: new topology and positions
+    :rtype: tuple[Topology, list]
     """
     fixer = pdbfixer.PDBFixer(pdbfile=pdbfile, pdbxfile=pdbxfile)
     fixer.findMissingResidues()
     
     chains = list(fixer.topology.chains())
     keys = fixer.missingResidues.keys()
     for key in list(keys):
@@ -114,19 +122,19 @@
     fixer.addMissingAtoms()
     fixer.addMissingHydrogens(7)
     return fixer.topology, fixer.positions
     
 def add_variants(topology: Topology, positions: list, variants: list=list()) -> tuple[Topology, list]:
     """Adds variants for specific protonation states.
 
-    Args:
-        topology (Topology): openmm topology
-        positions (list): openmm positions
-        variants (list): list of variants to apply for the protonation states. 
-                         The ones to leave untouched are passed as None. Defaults to list().
-
-    Returns:
-        tuple[Topology, list]: topology and positions with added protonation states.
+    :param topology: openmm topology
+    :type topology: Topology
+    :param positions: openmm positions
+    :type positions: list
+    :param variants: list of variants to apply for the protonation states, defaults to list()
+    :type variants: list, optional
+    :return: topology and positions with added protonation states
+    :rtype: tuple[Topology, list]
     """
     modeller = Modeller(topology, positions)
     added_variants = modeller.addHydrogens(variants=variants)
     return modeller.topology, modeller.positions
```

### Comparing `cosolvkit-0.4.1/cosolvkit.egg-info/PKG-INFO` & `cosolvkit-0.4.2/cosolvkit.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: cosolvkit
-Version: 0.4.1
+Version: 0.4.2
 Summary: CosolvKit
 Home-page: https://github.com/forlilab/cosolvkit
 Author: Niccolo Bruciaferri, Jerome Eberhardt
 Author-email: forli@scripps.edu
 License: LGPL-2.1
 Keywords: molecular modeling,drug design,cosolvent,MD simulations
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.9, <3.12
 License-File: LICENSE
```

### Comparing `cosolvkit-0.4.1/cosolvkit.egg-info/SOURCES.txt` & `cosolvkit-0.4.2/cosolvkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.1/scripts/create_cosolvent_system.py` & `cosolvkit-0.4.2/scripts/create_cosolvent_system.py`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.1/scripts/post_simulation_processing.py` & `cosolvkit-0.4.2/scripts/post_simulation_processing.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,29 +5,32 @@
     parser = argparse.ArgumentParser(description="Runs cosolvkit and MD simulation afterwards.")
     parser.add_argument('-l', '--log_file', dest='log_file', required=True,
                         action='store', help='path to the log file from MD simulation')
     parser.add_argument('-traj', dest='traj_file', required=True,
                         action='store', help='path to the traj <.dcd> file from MD simulation')
     parser.add_argument('-topo', dest='top_file', required=True,
                         action='store', help='path to the topology file from MD simulation')
+    parser.add_argument('-densitises', nargs='+', help='path to the density files passed as a list',
+                        action='store', dest='densities', required=True)
     parser.add_argument('-o', '--out_path', dest='out_path', required=True,
                         action='store', help='path where to store output plots')
     parser.add_argument('-c', '--cosolvents', dest='cosolvents', required=True,
                         action='store', help='path to the json file containing cosolvents used for the simulation')
     return parser.parse_args()
 
 
 if __name__ == "__main__":
     args = cmd_lineparser()
     log_file = args.log_file
     traj_file = args.traj_file
     top_file = args.top_file
+    densities = args.densities
     out_path = args.out_path
     cosolvents_path = args.cosolvents
 
     report = Report(log_file, traj_file, top_file, cosolvents_path)
     report.generate_report(out_path=out_path)
     report.generate_pymol_reports(report.topology, 
                                   report.trajectory, 
-                                  density_files=["path_to_density_file"], 
+                                  density_files=densities, 
                                   selection_string='', 
                                   out_path=out_path)
```

### Comparing `cosolvkit-0.4.1/setup.py` & `cosolvkit-0.4.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,31 +14,31 @@
         for filename in fnmatch.filter(filenames, '*'):
             matches.append(os.path.join(root, filename))
 
     return matches
 
 
 setup(name="cosolvkit",
-      version='0.4.1',
+      version='0.4.2',
       description="CosolvKit",
       author="Niccolo Bruciaferri, Jerome Eberhardt",
       author_email="forli@scripps.edu",
       url="https://github.com/forlilab/cosolvkit",
       packages=find_packages(),
       scripts=["scripts/create_cosolvent_system.py",
                "scripts/post_simulation_processing.py"],
       package_data={"cosolvkit" : ["data/*"]},
       data_files=[("", ["README.md", "LICENSE"]),
                   ("scripts", find_files("scripts"))],
       include_package_data=True,
       zip_safe=False,
+      python_requires=">=3.9, <3.12",
       license="LGPL-2.1",
       keywords=["molecular modeling", "drug design",
                 "cosolvent", "MD simulations"],
-      classifiers=["Programming Language :: Python :: 3.8",
-                   "Programming Language :: Python :: 3.9",
+      classifiers=["Programming Language :: Python :: 3.9",
                    "Programming Language :: Python :: 3.10",
                    "Programming Language :: Python :: 3.11",
                    "Operating System :: Unix",
                    "Operating System :: MacOS",
                    "Topic :: Scientific/Engineering"]
 )
```

