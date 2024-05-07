# Comparing `tmp/fm2prof-2.3.1.tar.gz` & `tmp/fm2prof-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fm2prof-2.3.1.tar", max compression
+gzip compressed data, was "fm2prof-2.3.2.tar", max compression
```

## Comparing `fm2prof-2.3.1.tar` & `fm2prof-2.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       65 2024-04-24 18:51:55.859891 fm2prof-2.3.1/fm2prof/__init__.py
--rw-r--r--   0        0        0       66 2024-04-24 18:51:55.861890 fm2prof-2.3.1/fm2prof/__main__.py
--rw-r--r--   0        0        0     2457 2024-04-24 18:51:55.862889 fm2prof-2.3.1/fm2prof/cli.py
--rw-r--r--   0        0        0    10183 2024-04-24 18:51:55.864889 fm2prof-2.3.1/fm2prof/common.py
--rw-r--r--   0        0        0     4411 2024-04-24 18:51:55.867890 fm2prof-2.3.1/fm2prof/configurationfile_template.json
--rw-r--r--   0        0        0    58333 2024-04-24 18:51:55.841887 fm2prof-2.3.1/fm2prof/CrossSection.py
--rw-r--r--   0        0        0    17564 2024-04-24 18:51:55.844889 fm2prof-2.3.1/fm2prof/Export.py
--rw-r--r--   0        0        0    42566 2024-04-24 18:51:55.847890 fm2prof-2.3.1/fm2prof/Fm2ProfRunner.py
--rw-r--r--   0        0        0     8684 2024-04-24 18:51:55.849890 fm2prof-2.3.1/fm2prof/Functions.py
--rw-r--r--   0        0        0    12579 2024-04-24 18:51:55.852894 fm2prof-2.3.1/fm2prof/Import.py
--rw-r--r--   0        0        0    17768 2024-04-24 18:51:55.854890 fm2prof-2.3.1/fm2prof/IniFile.py
--rw-r--r--   0        0        0    16955 2024-04-24 18:51:55.869892 fm2prof-2.3.1/fm2prof/lib/polysimplify.py
--rw-r--r--   0        0        0     1484 2024-04-24 18:51:55.868896 fm2prof-2.3.1/fm2prof/lib/polysimplify.README.md
--rw-r--r--   0        0        0     1897 2024-04-24 18:51:55.871890 fm2prof-2.3.1/fm2prof/main.py
--rw-r--r--   0        0        0     3158 2024-04-24 18:51:55.856890 fm2prof-2.3.1/fm2prof/MaskOutputFile.py
--rw-r--r--   0        0        0    10321 2024-04-24 18:51:55.857891 fm2prof-2.3.1/fm2prof/RegionPolygonFile.py
--rw-r--r--   0        0        0   107724 2024-04-24 18:51:55.875890 fm2prof-2.3.1/fm2prof/utils.py
--rw-r--r--   0        0        0    35823 2024-04-24 18:51:55.652889 fm2prof-2.3.1/LICENSE.txt
--rw-r--r--   0        0        0      932 2024-04-24 18:51:55.653889 fm2prof-2.3.1/LICENSE_HEADER.txt
--rw-r--r--   0        0        0     1295 2024-04-24 18:51:55.889892 fm2prof-2.3.1/pyproject.toml
--rw-r--r--   0        0        0      794 2024-04-24 18:51:55.654907 fm2prof-2.3.1/README.md
--rw-r--r--   0        0        0     1719 1970-01-01 00:00:00.000000 fm2prof-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0       65 2024-05-07 19:17:57.607455 fm2prof-2.3.2/fm2prof/__init__.py
+-rw-r--r--   0        0        0       66 2024-05-07 19:17:57.608454 fm2prof-2.3.2/fm2prof/__main__.py
+-rw-r--r--   0        0        0     2457 2024-05-07 19:17:57.609456 fm2prof-2.3.2/fm2prof/cli.py
+-rw-r--r--   0        0        0    10183 2024-05-07 19:17:57.610457 fm2prof-2.3.2/fm2prof/common.py
+-rw-r--r--   0        0        0     4411 2024-05-07 19:17:57.614467 fm2prof-2.3.2/fm2prof/configurationfile_template.json
+-rw-r--r--   0        0        0    58333 2024-05-07 19:17:57.592454 fm2prof-2.3.2/fm2prof/CrossSection.py
+-rw-r--r--   0        0        0    17564 2024-05-07 19:17:57.594453 fm2prof-2.3.2/fm2prof/Export.py
+-rw-r--r--   0        0        0    42592 2024-05-07 19:17:57.599496 fm2prof-2.3.2/fm2prof/Fm2ProfRunner.py
+-rw-r--r--   0        0        0     8684 2024-05-07 19:17:57.601459 fm2prof-2.3.2/fm2prof/Functions.py
+-rw-r--r--   0        0        0    12579 2024-05-07 19:17:57.602456 fm2prof-2.3.2/fm2prof/Import.py
+-rw-r--r--   0        0        0    17768 2024-05-07 19:17:57.604457 fm2prof-2.3.2/fm2prof/IniFile.py
+-rw-r--r--   0        0        0    16955 2024-05-07 19:17:57.618454 fm2prof-2.3.2/fm2prof/lib/polysimplify.py
+-rw-r--r--   0        0        0     1484 2024-05-07 19:17:57.617454 fm2prof-2.3.2/fm2prof/lib/polysimplify.README.md
+-rw-r--r--   0        0        0     1897 2024-05-07 19:17:57.620455 fm2prof-2.3.2/fm2prof/main.py
+-rw-r--r--   0        0        0     3158 2024-05-07 19:17:57.605454 fm2prof-2.3.2/fm2prof/MaskOutputFile.py
+-rw-r--r--   0        0        0    10321 2024-05-07 19:17:57.606455 fm2prof-2.3.2/fm2prof/RegionPolygonFile.py
+-rw-r--r--   0        0        0   113935 2024-05-07 19:17:57.622461 fm2prof-2.3.2/fm2prof/utils.py
+-rw-r--r--   0        0        0    35823 2024-05-07 19:17:57.336345 fm2prof-2.3.2/LICENSE.txt
+-rw-r--r--   0        0        0      932 2024-05-07 19:17:57.336345 fm2prof-2.3.2/LICENSE_HEADER.txt
+-rw-r--r--   0        0        0     1295 2024-05-07 19:17:57.633465 fm2prof-2.3.2/pyproject.toml
+-rw-r--r--   0        0        0      794 2024-05-07 19:17:57.338345 fm2prof-2.3.2/README.md
+-rw-r--r--   0        0        0     1719 1970-01-01 00:00:00.000000 fm2prof-2.3.2/PKG-INFO
```

### Comparing `fm2prof-2.3.1/fm2prof/cli.py` & `fm2prof-2.3.2/fm2prof/cli.py`

 * *Files identical despite different names*

### Comparing `fm2prof-2.3.1/fm2prof/common.py` & `fm2prof-2.3.2/fm2prof/common.py`

 * *Files identical despite different names*

### Comparing `fm2prof-2.3.1/fm2prof/configurationfile_template.json` & `fm2prof-2.3.2/fm2prof/configurationfile_template.json`

 * *Files identical despite different names*

### Comparing `fm2prof-2.3.1/fm2prof/CrossSection.py` & `fm2prof-2.3.2/fm2prof/CrossSection.py`

 * *Files identical despite different names*

### Comparing `fm2prof-2.3.1/fm2prof/Export.py` & `fm2prof-2.3.2/fm2prof/Export.py`

 * *Files identical despite different names*

### Comparing `fm2prof-2.3.1/fm2prof/Fm2ProfRunner.py` & `fm2prof-2.3.2/fm2prof/Fm2ProfRunner.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,20 +36,21 @@
     """
     Main class that executes all functionality.
 
     Arguments:
         iniFilePath (str): path to configuration file
     """
 
-    def __init__(self, iniFilePath: str = ""):
+    def __init__(self, iniFilePath: Path | str = ""):
         """
         Initializes the project
 
-        iniFilePath (str): path to a configuration file. If not given,
-                               default values will be used.
+        Parameters:
+            iniFilePath: path to a configuration file. If not given,
+                                default values will be used.
         """
         self.fm_model_data: FmModelData = None
         self._output_files: OutputFiles = OutputFiles()
 
         self._create_logger()
 
         iniFilePath = Path(iniFilePath)
@@ -1103,15 +1104,15 @@
             if it does not already exists!
 
         Arguments:
             path: path to the output path
         """
         self.get_inifile().set_output_directory(path)
 
-    def get_output_directory(self) -> None:
+    def get_output_directory(self) -> str:
         """
         Returns the current output directory
         """
         return self.get_inifile().get_output_directory()
 
     def print_configuration(self) -> str:
         """
```

### Comparing `fm2prof-2.3.1/fm2prof/Functions.py` & `fm2prof-2.3.2/fm2prof/Functions.py`

 * *Files identical despite different names*

### Comparing `fm2prof-2.3.1/fm2prof/Import.py` & `fm2prof-2.3.2/fm2prof/Import.py`

 * *Files identical despite different names*

### Comparing `fm2prof-2.3.1/fm2prof/IniFile.py` & `fm2prof-2.3.2/fm2prof/IniFile.py`

 * *Files identical despite different names*

### Comparing `fm2prof-2.3.1/fm2prof/lib/polysimplify.py` & `fm2prof-2.3.2/fm2prof/lib/polysimplify.py`

 * *Files identical despite different names*

### Comparing `fm2prof-2.3.1/fm2prof/lib/polysimplify.README.md` & `fm2prof-2.3.2/fm2prof/lib/polysimplify.README.md`

 * *Files identical despite different names*

### Comparing `fm2prof-2.3.1/fm2prof/main.py` & `fm2prof-2.3.2/fm2prof/main.py`

 * *Files identical despite different names*

### Comparing `fm2prof-2.3.1/fm2prof/MaskOutputFile.py` & `fm2prof-2.3.2/fm2prof/MaskOutputFile.py`

 * *Files identical despite different names*

### Comparing `fm2prof-2.3.1/fm2prof/RegionPolygonFile.py` & `fm2prof-2.3.2/fm2prof/RegionPolygonFile.py`

 * *Files identical despite different names*

### Comparing `fm2prof-2.3.1/fm2prof/utils.py` & `fm2prof-2.3.2/fm2prof/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import ast
 import locale
 import os
 import re
-import shutil
+import warnings
 from dataclasses import dataclass
 from datetime import datetime, timedelta
-from enum import unique
 from logging import Logger
 from pathlib import Path
+from collections import namedtuple
 from typing import (
     Any,
     Callable,
     Dict,
     Generator,
     Iterable,
     List,
@@ -25,26 +25,33 @@
 import matplotlib.gridspec as gridspec
 import matplotlib.patches as mpatches
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import tqdm
 from matplotlib.figure import Figure
+from matplotlib.legend import Legend
 from matplotlib.ticker import AutoMinorLocator, FormatStrFormatter, MultipleLocator
 from netCDF4 import Dataset
 from pandas.plotting import register_matplotlib_converters
 from scipy.interpolate import interp1d
 
+
 from fm2prof import Project
 from fm2prof.common import FM2ProfBase
 
 register_matplotlib_converters()
 
-COLORSCHEME = ["k", "#00cc96", "#0d38e0"]
+FigureOutput = namedtuple('FigureOutput', ['fig', 'axes', 'legend'])
+StyleGuide = namedtuple('StyleGuide', ['font', 'major_grid', 'minor_grid', 'spine_width'])
 
+COLORSCHEMES = {"Deltares": ["#000000", "#00cc96", "#0d38e0"],
+                "Koeln": ["#000000", "#E69F00", "#56B4E9", "#009E73", "#F0E444", "#0072B2", "#D55E00", "#CC79A7"],  # https://jfly.uni-koeln.de/color/
+                "PaulTolVibrant": ["#0077BB", "#33BBEE", "#009988", "#EE7733", "#CC3311", "#EE3377","#BBBBBB"]
+                }
 
 class GenerateCrossSectionLocationFile(FM2ProfBase):
     """
     Builds a cross-section input file for FM2PROF from a SOBEK 3 DIMR network definition file.
 
     The distance between cross-section is computed from the differences between the offsets/chainages.
     The beginning and end point of each branch are treated as half-distance control volumes.
@@ -400,16 +407,15 @@
         self._ref_geom_y = []
         self._ref_geom_tw = []
         self._ref_geom_fw = []
 
         self.set_logger_message(f"Using {self.fig_dir} as output directory for figures")
 
         # initiate plotstyle
-        # TODO: make configurable which style to use?
-        PlotStyles.van_veen()
+        PlotStyles.apply()
 
     @property
     def branches(self) -> Generator[List[str], None, None]:
         def split_css(name) -> Tuple[str, float, str]:
             chainage = float(name.split("_")[-1])
             branch = "_".join(name.split("_")[:-1])
             return (name, chainage, branch)
@@ -442,14 +448,17 @@
             yield css
 
     def figure_roughness_longitudinal(self, branch: str):
         """
         Assumes the following naming convention:
         [branch]_[optional:branch_order]_[chainage]
         """
+        output_dir = self.fig_dir.joinpath('roughness')
+        if not output_dir.is_dir():
+            os.mkdir(output_dir)
 
         fig, ax = plt.subplots(1, figsize=(12, 5))
 
         css = self.get_cross_sections_for_branch(branch)
 
         chainage = []
         minmax = []
@@ -463,20 +472,22 @@
         ax.plot(chainage, minmax[:, 0], label="minimum")
         ax.plot(chainage, minmax[:, 1], label="maximum")
         ax.set_ylabel("Ruwheid (Chezy)")
         ax.set_xlabel("Afstand [km]")
         ax.set_title(branch)
         fig, lgd = self._SetPlotStyle(fig, use_legend=True)
         plt.savefig(
-            self.fig_dir.joinpath(f"roughness_longitudinal_{branch}.png"),
+            output_dir.joinpath(f"roughness_longitudinal_{branch}.png"),
             bbox_extra_artists=[lgd],
             bbox_inches="tight",
         )
 
-    def get_cross_sections_for_branch(self, branch: str):
+    def get_cross_sections_for_branch(self, branch: str) -> Tuple[str, float, str]:
+        if branch not in self.branches:
+            raise KeyError(f"Branch {branch} not in known branches: {self.branches}")
         def split_css(name) -> Tuple[str, float, str]:
             chainage = float(name.split("_")[-1])
             branch = "_".join(name.split("_")[:-1])
             return (name, chainage, branch)
 
         def get_css_for_branch(css_list, branchname: str):
             return [c for c in css_list if c[2].startswith(branchname)]
@@ -576,15 +587,19 @@
 
             reference_roughness (tuple): tuple(list(z), list(n))
 
             save_to_file (bool): if true, save figure to VisualiseOutput.fig_dir
                                  if false, returns pyplot figure object
 
         """
-        output_file = self.fig_dir.joinpath(f"{css['id']}.png")
+        output_dir = self.fig_dir.joinpath('cross_sections')
+        if not output_dir.is_dir():
+            os.mkdir(output_dir)
+        
+        output_file = output_dir.joinpath(f"{css['id']}.png")
         if output_file.is_file() & ~overwrite:
             self.set_logger_message("file already exists", "debug")
             return
         try:
             fig = plt.figure(figsize=(8, 12))
             gs = fig.add_gridspec(2, 2)
             axs = [
@@ -635,15 +650,15 @@
         Arguments:
             output_map - path to fm2prof output directory
 
         Returns:
             png images saved to file
         """
 
-        figdir = self.output_dir.joinpath("figures/cross_sections")
+        figdir = self.output_dir.joinpath("figures")
         if not figdir.is_dir():
             figdir.mkdir(parents=True)
         return figdir
 
     def _set_files(self):
         self.files = {
             "css_def": os.path.join(self.output_dir, self.__cssdeffile),
@@ -689,15 +704,15 @@
 
         return csslist
 
     def _SetPlotStyle(self, *args, **kwargs):
         """todo: add preference to switch styles or
         inject own style
         """
-        return PlotStyles.van_veen(*args, **kwargs)
+        return PlotStyles.apply(*args, **kwargs)
 
     def _plot_geometry(self, css, ax, reference_geometry=None):
 
         # Get data
         tw = np.append([0], np.array(css["total_width"]))
         fw = np.append([0], np.array(css["flow_width"]))
         l = np.append(css["levels"][0], np.array(css["levels"]))
@@ -904,14 +919,15 @@
         return branch, chainage
 
 
 class PlotStyles:
     myFmt = mdates.DateFormatter("%d-%b")
     monthlocator = mdates.MonthLocator(bymonthday=(1, 10, 20))
     daylocator = mdates.DayLocator(interval=5)
+    colorscheme = COLORSCHEMES["Koeln"]
 
     @staticmethod
     def set_locale(localeString: str):
         try:
             locale.setlocale(locale.LC_TIME, localeString)
         except locale.Error:
             # known error on linux fix:
@@ -928,102 +944,100 @@
                 float(label_string)
 
         except ValueError:
             return True
         except IndexError:
             return False
         return False
-
+    
     @classmethod
-    def pilot_2021(cls, fig, legendbelow=False):
-        for ax in fig.axes:
-            ax.grid(False)
-            ax.spines["top"].set_visible(False)
-            ax.spines["right"].set_visible(False)
-
-            ax.xaxis.set_tick_params(width=2)
-            ax.yaxis.set_tick_params(width=2)
-            for spine in ["left", "bottom"]:
-                ax.spines[spine].set_edgecolor("#272727")
-                ax.spines[spine].set_linewidth(2)
-            if legendbelow:
-                legend = ax.legend(
-                    fancybox=True,
-                    framealpha=0.5,
-                    edgecolor="None",
-                    loc=3,
-                    ncol=3,
-                    bbox_to_anchor=(-0.02, -0.5),
-                )
-            else:
-                legend = ax.legend(fancybox=True, framealpha=0.5, edgecolor="None")
-            legend.get_frame().set_facecolor("#e5eef2")  # #e5eef2 #92b6c7
-            legend.get_frame().set_boxstyle("square", pad=0)
+    def van_veen(cls,
+            fig: Figure | None = None,
+            use_legend: bool = True,
+            extra_labels: List | None = None,
+            ax_align_legend: plt.Axes | None = None,):
+        
+        warnings.warn("This function is deprecated and will be removed on future versions. Use PlotStyle.apply(fig, style='van_veen') instead",
+                      category=DeprecationWarning)
+        cls.apply(fig=fig, style='van_veen', use_legend=use_legend, extra_labels=extra_labels, ax_align_legend=ax_align_legend)
+
 
     @classmethod
-    def van_veen(
+    def apply(
         cls,
-        fig: Figure = None,
+        fig: Figure | None = None,
+        style: str = "sito",
         use_legend: bool = True,
-        extra_labels: Union[List, type(None)] = None,
-        ax_align_legend: plt.Axes = None,
-    ):
-        """Stijl van Van Veen"""
+        extra_labels: List | None = None,
+        ax_align_legend: plt.Axes | None = None,
+    ) -> Tuple[Figure, Legend]:
+        
+        styles: Dict[str, StyleGuide] = dict(sito= StyleGuide(font={"family": "Franca, Arial", "weight": "normal", "size": 16},
+                                 major_grid = dict(visible=True, which="major", linestyle="--", linewidth=1.0, color="#BBBBBB"),
+                                 minor_grid = dict(visible=True, which="minor", linestyle="--", linewidth=1.0, color="#BBBBBB"),
+                                 spine_width=1),
+                      van_veen = StyleGuide(font={"family": "Bahnschrift", "weight": "normal", "size": 18},
+                                 major_grid = dict(visible=True, which="major", linestyle="-", linewidth=1, color="k"),
+                                 minor_grid = dict(visible=True, which="minor", linestyle="-", linewidth=0.5, color="k"),
+                                 spine_width=2)
+                        )
+        
+        if style not in styles:
+            raise KeyError(f"unknown style {style}. Options are {list(styles.keys())}")
+        
+        style_guide: StyleGuide = styles.get(style)
 
-        def initiate():
+        def initiate() -> None:
             # Set default locale to NL
-            # TODO: add localization options
+            # TODO: add localization options (#85)
             PlotStyles.set_locale("nl_NL.UTF-8")
 
             # Color style
             mpl.rcParams["axes.prop_cycle"] = mpl.cycler(
-                color=COLORSCHEME * 3,
-                linestyle=["-"] * 3 + ["--"] * 3 + ["-."] * 3,
-                linewidth=np.linspace(0.5, 3, 9),
+                color=cls.colorscheme * 3,
+                linestyle=["-"] * len(cls.colorscheme) + ["--"] * len(cls.colorscheme) + ["-."] * len(cls.colorscheme),
             )
 
             # Font style
-            font = {"family": "Bahnschrift", "weight": "normal", "size": 18}
+            font = style_guide.font
+
+            # not all fonts support the unicode minus, so disable this option
             mpl.rc("font", **font)
             mpl.rcParams[
                 "axes.unicode_minus"
-            ] = False  # not all fonts support the unicode minus
+            ] = False  
 
-        def styleFigure(fig, use_legend, extra_labels, ax_align_legend):
+        def style_figure(fig, use_legend, extra_labels, ax_align_legend) -> Tuple[Figure, Legend] | Tuple[Figure, List] | None:
             if ax_align_legend is None:
                 ax_align_legend = fig.axes[0]
 
             # this forces labels to be generated. Necessary to detect datetimes
             fig.canvas.draw()
 
             # Set styles for each axis
-            legend_title = r"toelichting"
+            legend_title = r"Toelichting"
             handles = list()
             labels = list()
 
             for ax in fig.axes:
 
-                ax.grid(visible=True, which="major", linestyle="-", linewidth=1, color="k")
-                ax.grid(visible=True, which="minor", linestyle="-", linewidth=0.5, color="k")
+                # Enable grid grid
+                ax.grid(**style_guide.major_grid)
+                ax.grid(**style_guide.minor_grid)
 
                 for _, spine in ax.spines.items():
-                    spine.set_linewidth(2)
+                    spine.set_linewidth(style_guide.spine_width)
 
                 if cls._is_timeaxis(ax.xaxis):
                     ax.xaxis.set_major_formatter(cls.myFmt)
                     ax.xaxis.set_major_locator(cls.monthlocator)
-                    # ax.xaxis.set_minor_locator(cls.daylocator)
                 if cls._is_timeaxis(ax.yaxis):
                     ax.yaxis.set_major_formatter(cls.myFmt)
                     ax.yaxis.set_major_locator(cls.monthlocator)
-                    # ax.yaxis.set_minor_locator(cls.daylocator)
 
-                ax.set_title(ax.get_title().upper())
-                ax.set_xlabel(ax.get_xlabel().upper())
-                ax.set_ylabel(ax.get_ylabel().upper())
                 ax.patch.set_visible(False)
                 h, l = ax.get_legend_handles_labels()
                 handles.extend(h)
                 labels.extend(l)
 
             if extra_labels:
                 handles.extend(extra_labels[0])
@@ -1047,16 +1061,15 @@
             else:
                 return fig, handles, labels
 
         if not fig:
             return initiate()
         else:
             initiate()
-            return styleFigure(fig, use_legend, extra_labels, ax_align_legend)
-
+            return style_figure(fig=fig, use_legend=use_legend, extra_labels=extra_labels, ax_align_legend=ax_align_legend)
 
 @dataclass
 class DeltaresSectionItem:
     value: Any
     comment: str = ""
 
 
@@ -1569,58 +1582,56 @@
                     except StopIteration:
                         hn = ""
                     fw.write(f"{n},{hn},{qn}\n")
 
 
 class Compare1D2D(ModelOutputReader):
     """
-    Class to compare the results of a 1D and 2D model.
+    Utility to compare the results of a 1D and 2D model through 
+    visualisation and statistical post-processing. 
 
-    .. note::
+    Note:
         If 2D and 1D netCDF input files are provided, they will first be 
         converted to csv files. Once csv files are present, the original
         netCDF files are no longer used. In that case, the arguments 
         to `path_1d` and `path_2d` should be `None`. 
 
 
     Example usage:
-
-        >>> plotter = Compare1D2D()
-        >>> # Set path to data
-        >>> plotter.path_flow1d = path_to_dimr_dir
-        >>> plotter.path_flow2d = path_to_nc_file
-        >>> # Example, plot along route
-        >>> route = ['BR', "PK", "NR", "LE"]
-        >>> plotter.figure_longitudinal_time(route=route)
-
-    Parameters
-        project: Project
-
-        path_1d: Union[Path, str],
-        
-        path_2d: Union[Path, str],
-        
-        routes: List[List[str]],
-        
-        start_time: Union[None, datetime] = None,
-        
-        stop_time: Union[None, datetime] = None,
-
+        ``` py
+        from fm2prof import Project, utils
+        project = Project(fr'tests/test_data/compare1d2d/cases/case1/fm2prof.ini')
+        plotter = utils.Compare1D2D(project=project,
+                                    start_time=datetime(year=2000, month=1, day=5))
+
+        plotter.figure_at_station("NR_919.00")
+
+        ```
+
+    Parameters:
+        project: `fm2prof.Project` object.
+        path_1d: path to SOBEK dimr directory
+        path_2d: path to his nc file
+        routes: list of branch abbreviations, e.g. ['NR', 'LK']
+        start_time: start time for plotting and analytics. Use this to crop the time to prevent initalisation from affecting statistics. 
+        stop_time: stop time for plotting and analytics. 
+        style: `PlotStyles` style
     """
 
     _routes: List[List[str]] = None
 
     def __init__(
         self,
         project: Project,
-        path_1d: Union[Path, str] | None,
-        path_2d: Union[Path, str] | None,
-        routes: List[List[str]],
+        path_1d: Union[Path, str] | None = None,
+        path_2d: Union[Path, str] | None = None,
+        routes: List[List[str]] | None = None,
         start_time: Union[None, datetime] = None,
         stop_time: Union[None, datetime] = None,
+        style: str = 'sito',
     ):
         if project:
             super().__init__(logger=project.get_logger(), start_time=start_time, stop_time=stop_time)
             self.output_path = project.get_output_directory()
         else:
             super().__init__()
 
@@ -1638,17 +1649,19 @@
         self._data_1D_H: pd.DataFrame = None
         self._data_2D_H: pd.DataFrame = None
         self._data_1D_H_digitized: pd.DataFrame = None
         self._data_2D_H_digitized: pd.DataFrame = None
         self._qsteps = np.arange(0, 100 * np.ceil(18000 / 100), 200)
 
         # initiate plotstyle
-        PlotStyles.van_veen()
-        self._error_colors = ["#7e3e00", "#b25800", "#d86a00"]
+        self._error_colors = ["#7e3e00", "#FF4433", "#d86a00"]
         self._color_error = self._error_colors[1]
+        self._color_scheme = COLORSCHEMES["Koeln"]
+        self._plotstyle: str = style
+        PlotStyles.apply(style=self._plotstyle)
 
         # set start time
         self.start_time = start_time
         self.stop_time = stop_time
 
         self.read_all_data()
         self.digitize_data()
@@ -1663,15 +1676,17 @@
         for od in output_dirs:
             try:
                 os.makedirs(self.output_path.joinpath(od))
             except FileExistsError:
                 pass
 
     def eval(self):
-
+        """
+        does a bunch
+        """
         for route in tqdm.tqdm(self.routes):
             self.set_logger_message(f"Making figures for route {route}")
             self.figure_longitudinal_rating_curve(route)
             self.figure_longitudinal_time(route)
             self.heatmap_rating_curve(route)
             self.heatmap_time(route)
 
@@ -1694,14 +1709,18 @@
     def file_1D_H_digitized(self):
         return self.file_1D_H.parent.joinpath(f"{self.file_1D_H.stem}_digitized.csv")
 
     @property
     def file_2D_H_digitized(self):
         return self.file_2D_H.parent.joinpath(f"{self.file_2D_H.stem}_digitized.csv")
 
+    @property
+    def colorscheme(self):
+        return self._colorscheme
+    
     def digitize_data(self):
         if self.file_1D_H_digitized.is_file():
             self.set_logger_message("Using existing digitized file for 1d")
             self._data_1D_H_digitized = pd.read_csv(
                 self.file_1D_H_digitized, index_col=0
             )
         else:
@@ -1829,96 +1848,113 @@
                 bstd = s["std"][s.branch == branch].mean()
                 lmw_bias = s.bias[(s.branch == branch) & s.is_lmw].mean()
                 lmw_std = s["std"][(s.branch == branch) & s.is_lmw].mean()
                 f.write(
                     f"{branch},{bbias:.2f}±({bstd:.2f}), {lmw_bias:.2f}±({lmw_std:.2f})\n"
                 )
 
-    def figure_at_station(self, station: str) -> None:
+    def figure_at_station(self, station: str, func:str="time", savefig:bool=True) -> FigureOutput:
         """
-        Create a figure with the results at an observation station.
-
-        Figures are saved to `[Compare1D2D.output_path]/figures/stations`
-
-        Example output:
+        Creates a figure with the timeseries at a single observation station.
 
-        .. figure:: figures_utils/stations/example.png
+        ``` py
+        
+        ```
 
-            example output figure
+        Parameters:
+            station: name of station. use `stations` method to list all station names
+            func: use `time` for a timeseries and `qh` for rating curve
+            savefig: if True, saves to png. If False, returned FigureOutput
+        
+        
 
         """
 
-        fig, axs = plt.subplots(1, 2, figsize=(12, 5))
-        error_axes = [axs[0].twinx(), axs[1].twinx()]
+        fig, ax = plt.subplots(1, figsize=(12, 5))
+        error_ax = ax.twinx()
 
         # q/h view
-        axs[0].plot(
-            self._qsteps,
-            self._data_2D_H_digitized[station],
-            "--",
-            linewidth=2,
-            label="2D",
-        )
-        axs[0].plot(
-            self._qsteps,
-            self._data_1D_H_digitized[station],
-            "-",
-            linewidth=2,
-            label="1D",
-        )
-
-        axs[0].set_title("QH-relatie")
-        axs[0].set_xlabel("afvoer [m$^3$/s]")
-        axs[0].set_ylabel("Waterstand [m+NAP]")
-        error_axes[0].plot(
-            self._qsteps,
-            self._data_1D_H_digitized[station] - self._data_2D_H_digitized[station],
-            ".",
-            color=self._color_error,
-        )
-        # time view
-        axs[1].plot(self.data_2D_H[station], "--", linewidth=2)
-        axs[1].plot(self.data_1D_H[station], "-", linewidth=2)
-        axs[1].set_title("tijdserie")
-
-        error_axes[1].plot(
-            self.data_1D_H[station] - self.data_2D_H[station],
-            ".",
-            label="1D-2D",
-            color=self._color_error,
-        )
+        match func.lower():
+            case "qh":
+                ax.plot(
+                    self._qsteps,
+                    self._data_2D_H_digitized[station],
+                    "--",
+                    linewidth=2,
+                    label="2D",
+                )
+                ax.plot(
+                    self._qsteps,
+                    self._data_1D_H_digitized[station],
+                    "-",
+                    linewidth=2,
+                    label="1D",
+                )
+                ax.set_title(f"{station}\nQH-relatie")
+                ax.set_title("QH-relatie")
+                ax.set_xlabel("Afvoer [m$^3$/s]")
+                ax.set_ylabel("Waterstand [m+NAP]")
+                error_ax.plot(
+                    self._qsteps,
+                    self._data_1D_H_digitized[station] - self._data_2D_H_digitized[station],
+                    ".",
+                    color=self._color_error,
+                )
+            case "time":
+                ax.plot(self.data_2D_H[station], "--", 
+                        linewidth=2,
+                        label="2D")
+                ax.plot(self.data_1D_H[station], "-", 
+                        linewidth=2,
+                        label="1D")
+                
+                ax.set_ylabel("Waterstand [m+NAP]")
+                ax.set_title(f"{station}\nTijdreeks")
+
+                error_ax.plot(
+                    self.data_1D_H[station] - self.data_2D_H[station],
+                    ".",
+                    label="1D-2D",
+                    color=self._color_error,
+                )
 
         # statistics
         stats = self._get_statistics(station)
 
         stats_labels = [
-            f"bias={stats['bias']:.2f}",
-            f"std={stats['std']:.2f}",
-            f"MAE={stats['mae']:.2f}",
+            f"bias={stats['bias']:.2f} m",
+            f"std={stats['std']:.2f} m",
+            f"MAE={stats['mae']:.2f} m",
         ]
         stats_handles = [mpatches.Patch(color="white")] * len(stats_labels)
+        
         # Style
-        suptitle = plt.suptitle(station)
-        fig, lgd = PlotStyles.van_veen(
-            fig, use_legend=True, extra_labels=[stats_handles, stats_labels]
-        )
+        fig, lgd = PlotStyles.apply(fig=fig, 
+                                    style=self._plotstyle,
+                                    use_legend=True, 
+                                    extra_labels=[stats_handles, stats_labels]
+                                )
 
-        for ax in error_axes:
-            self._style_error_axes(ax, ylim=[-0.5, 0.5])
+        self._style_error_axes(error_ax, ylim=[-1, 1])
 
         fig.tight_layout()
-        fig.savefig(
-            self.output_path.joinpath("figures/stations").joinpath(f"{station}.png"),
-            bbox_extra_artists=[lgd, suptitle],
-            bbox_inches="tight",
-        )
-        plt.close()
 
-    def _style_error_axes(self, ax, ylim: List[float] = [-0.5, 0.5]):
+        if savefig:
+            fig.savefig(
+                self.output_path.joinpath("figures/stations").joinpath(f"{station}.png"),
+                bbox_extra_artists=[lgd],
+                bbox_inches="tight",
+            )
+            plt.close()
+        else:
+            return FigureOutput(fig=fig, axes=ax, legend=lgd)
+
+    def _style_error_axes(self, ax, ylim: List[float] = [-0.5, 0.5], ylabel:str="1D-2D [m]"):
         ax.set_ylim(ylim)
+        ax.set_ylabel(ylabel)
         ax.spines["right"].set_edgecolor(self._color_error)
         ax.tick_params(axis="y", colors=self._color_error)
         ax.grid(False)
 
     def _compute_statistics(self) -> pd.DataFrame:
         """
         Computes statistics for the difference between 1D and 2D water levels
@@ -1950,124 +1986,124 @@
 
     def _get_statistics(self, station):
         if self.statistics is None:
             self.statistics = self._compute_statistics()
         return self.statistics.loc[station]
 
     def figure_compare_discharge_at_stations(
-        self, title: str = "notitle", stations: Tuple[str, str] = None
-    ) -> None:
+        self, stations: List[str], title: str = "no_title", savefig:bool=True
+    ) -> FigureOutput | None:
         """
-        Like :meth:`Compare1D2D.figure_at_station`, but compares discharge
+        Like `Compare1D2D.figure_at_station`, but compares discharge
         distribution over two stations.
 
         Example usage:
-
-            >>> Compare1D2().figure_compare_discharge_at_stations(stations=["WL_869.00", "PK_869.00"])
-
+        ``` py
+        Compare1D2().figure_compare_discharge_at_stations(stations=["WL_869.00", "PK_869.00"])
+        ```
         Figures are saved to `[Compare1D2D.output_path]/figures/discharge`
 
         Example output:
 
         .. figure:: figures_utils/discharge/example.png
 
             Example output figure
 
         """
-        fig, axs = plt.subplots(1, 2, figsize=(12, 5))
+        fig, axs = plt.subplots(2, 1, figsize=(12, 10))
 
         ax_error = axs[0].twinx()
         ax_error.set_zorder(
             axs[0].get_zorder() - 1
         )  # default zorder is 0 for ax1 and ax2
 
         if len(stations) != 2:
             print("error: must define 2 stations")
+        
         linestyles_2d = ["-", "--"]
         for j, station in enumerate(stations):
 
             if station not in self.stations():
-                print(f"warning', {station} not known")
+                self.set_logger_message(f"{station} not known", 'warning')
 
             # tijdserie
             axs[0].plot(
                 self.data_2D_Q[station],
                 label=f"2D, {station.split('_')[0]}",
                 linewidth=2,
                 linestyle=linestyles_2d[j],
-                color="k",
             )
             axs[0].plot(
                 self.data_1D_Q[station],
                 label=f"1D, {station.split('_')[0]}",
                 linewidth=2,
                 linestyle="-",
-                color=COLORSCHEME[j + 1],
             )
 
-            ax_error.plot(
-                self._data_1D_Q[station] - self._data_2D_Q[station],
-                ".",
-                color=self._error_colors[j + 1],
-                markersize=5,
-                label=f"1D-2D ({station.split('_')[0]})",
-            )
+        ax_error.plot(
+            self._data_1D_Q[station] - self._data_2D_Q[station],
+            ".",
+            color="r",
+            markersize=5,
+            label=f"1D-2D",
+        )
 
         # discharge distribution
+        
         Q2D = self.data_2D_Q[stations]
         Q1D = self.data_1D_Q[stations]
         axs[1].plot(
             Q2D.sum(axis=1),
             (Q2D.iloc[:, 0] / Q2D.sum(axis=1)) * 100,
             linewidth=2,
-            linestyle=linestyles_2d[0],
-            color="k",
+            linestyle='--',
         )
         axs[1].plot(
             Q1D.sum(axis=1),
             (Q1D.iloc[:, 0] / Q1D.sum(axis=1)) * 100,
             linewidth=2,
             linestyle="-",
-            color=COLORSCHEME[1],
         )
         axs[1].plot(
             Q2D.sum(axis=1),
             (Q2D.iloc[:, 1] / Q2D.sum(axis=1)) * 100,
             linewidth=2,
-            linestyle=linestyles_2d[1],
-            color="k",
+            linestyle='--',
         )
         axs[1].plot(
             Q1D.sum(axis=1),
             (Q1D.iloc[:, 1] / Q1D.sum(axis=1)) * 100,
             linewidth=2,
             linestyle="-",
-            color=COLORSCHEME[2],
         )
 
         # style
         axs[1].set_ylim(0, 100)
         axs[1].set_title("afvoerverdeling")
         axs[1].set_ylabel("percentage t.o.v. totaal")
         axs[1].set_xlabel("afvoer bovenstrooms [m$^3$/s]")
         axs[0].set_ylabel("afvoer [m$^3$/s]")
         axs[0].set_title("tijdserie")
 
         suptitle = plt.suptitle(title.upper())
 
         # Style figure
-        fig, lgd = PlotStyles.van_veen(fig, use_legend=[True, False])
-        self._style_error_axes(ax_error, ylim=[-500, 500])
+        fig, lgd = PlotStyles.apply(fig=fig, style=self._plotstyle, use_legend=True)
+        self._style_error_axes(ax_error, ylim=[-500, 500], ylabel="1D-2D [m$^3$/s]")
         fig.tight_layout()
-        fig.savefig(
-            self.output_path.joinpath("figures/discharge").joinpath(f"{title}.png"),
-            bbox_extra_artists=[lgd, suptitle],
-            bbox_inches="tight",
-        )
-        plt.close()
+
+        if savefig:
+            fig.savefig(
+                self.output_path.joinpath("figures/discharge").joinpath(f"{title}.png"),
+                bbox_extra_artists=[lgd, suptitle],
+                bbox_inches="tight",
+            )
+            plt.close()
+        else:
+            return FigureOutput(fig=fig, axes=axs, legend=lgd)
 
     def get_data_along_route_for_time(
         self, data: pd.DataFrame, route: List[str], time_index: int
     ) -> pd.Series:
         stations, rkms, _ = self.get_route(route)
 
         tmp_data = list()
@@ -2081,121 +2117,216 @@
     ) -> pd.DataFrame:
         stations, rkms, _ = self.get_route(route)
 
         tmp_data = list()
         for station in stations:
             tmp_data.append(data[station])
 
-        return pd.DataFrame(index=rkms, data=tmp_data)
+        df = pd.DataFrame(index=rkms, data=tmp_data)
+
+        # drop duplicates
+        df = df.drop_duplicates()
+        return df
 
     @staticmethod
     def _sec_to_days(seconds):
         return seconds / (3600 * 24)
 
     @staticmethod
     def _get_nearest_time(data: pd.DataFrame, date: datetime = None) -> int:
         try:
             return list(data.index < date).index(False)
         except ValueError:
             # False is not list, return last index
             return len(data.index) - 1
 
-    def figure_longitudinal_time(self, route: List[str]) -> None:
-        """
-        Create a figure along a route with lines at various points in time.
-        Figures are saved to `[Compare1D2D.output_path]/figures/longitudinal`
-
-        Example output:
-
-        .. figure:: figures_utils/longitudinal/example_time_series.png
-
-            example output figure
-
-        """
-        routename = "-".join(route)
-        _, _, lmw_stations = self.get_route(route)
-
-        fig, axs = plt.subplots(2, 1, figsize=(12, 12))
-
-        # plot line every delta_days days
+    def _time_func(self, route) -> Dict[str, pd.Series | str]:
         first_day = self.data_1D_H.index[0]  # + timedelta(days=delta_days) * 2
         last_day = self.data_1D_H.index[-1]
         number_of_days = (last_day - first_day).days
         delta_days = int(number_of_days / 6)
 
         moments = [
             first_day + timedelta(days=i) for i in range(0, number_of_days, delta_days)
         ]
-
-        # Plot LMW station locations
-        h1d = self.get_data_along_route(data=self.data_1D_H, route=route)
-        prevloc = -9999
-        for lmw in lmw_stations:
-            if lmw is None:
-                continue
-            newloc = max(lmw[1], prevloc + 3)
-            prevloc = lmw[1]
-            for ax in axs:
-                ax.axvline(x=lmw[1], linestyle="--")
-            axs[0].text(
-                newloc,
-                h1d.min().min(),
-                lmw[0],
-                fontsize=12,
-                rotation=90,
-                horizontalalignment="right",
-                verticalalignment="bottom",
-            )
+        lines = []
 
         for day in moments:
-
             h1d = self.get_data_along_route_for_time(
-                data=self.data_1D_H,
-                route=route,
-                time_index=self._get_nearest_time(data=self.data_1D_H, date=day),
-            )
+                    data=self.data_1D_H,
+                    route=route,
+                    time_index=self._get_nearest_time(data=self.data_1D_H, date=day),
+                )
 
             h2d = self.get_data_along_route_for_time(
                 data=self.data_2D_H,
                 route=route,
                 time_index=self._get_nearest_time(data=self.data_2D_H, date=day),
             )
 
-            axs[0].plot(h1d, label=f"{day:%b-%d}")
+            lines.append({"1D": h1d, 
+                          "2D": h2d,
+                          "label": f"{day:%b-%d}"})
 
-            axs[0].set_ylabel("waterstand [m+nap]")
+        return lines
+
+    def _last25(self, route: List[str]) -> List[Dict[str, pd.Series | str]]:
+        return self._stat_func(route, stat="last25")
+    
+    def _max13(self, route: List[str]) -> List[Dict[str, pd.Series | str]]:
+        return self._stat_func(route, stat="max13")
+    
+    def _stat_func(self, route: List[str], stat:str="max13") -> List[Dict[str, pd.Series | str]]:
+        """
+        Applies column-wise "last25" or "max13" on 1D and 2D data
+        """
+        def apply_stat(df, stat:str="max13"):
+            columns = df.columns
+            values = []
+            for column in columns:
+                try:
+                    af = df[column].iloc[:,0]
+                except pd.errors.IndexingError:
+                    af = df[column]
+                match stat:
+                    case "max13":
+                        values.append(af.nlargest(13).mean())
+                    case "last25":
+                        values.append(af[-25:].mean())
+            return pd.Series(index=columns, data=values)
+        
+        
+        max13_1d = apply_stat(self.get_data_along_route(self.data_1D_H, route=route).T, stat=stat)
+        max13_2d = apply_stat(self.get_data_along_route(self.data_2D_H, route=route).T, stat=stat)
+
+        return [{"1D": max13_1d, 
+                 "2D": max13_2d,
+                 "label": stat}]
+
+    def _lmw_func(self, station_names, station_locs):
+        st_names = []
+        st_locs = []
+        prev_loc = -9999
+        for name, loc in zip(station_names, station_locs):
+            if "lmw" not in name.lower(): continue
+            if abs(prev_loc - loc) < 5: 
+                self.set_logger_message(f"skipped labelling {name} because too close to previous station", "warning")
+                continue
+            st_names.append(name.split("_")[-1])
+            st_locs.append(loc)
+            prev_loc = loc
+
+        return st_names, st_locs
+    
+    def figure_longitudinal_time(self, route: List[str]) -> None:
+        warnings.warn("Method figure_longitudinal_time will be removed in the future. Use figure_longitudinal(route, stat=\"time\") instead ",
+                      category=DeprecationWarning)
+        
+        self.figure_longitudinal(route, stat="time")
+    
+    def figure_longitudinal(self, 
+                            route: List[str], 
+                            stat: str = 'time',
+                            savefig: bool=True,
+                            label: str = '',
+                            add_to_fig: FigureOutput | None = None) -> FigureOutput | None:
+        """
+        Creates a figure along a `route`. Content of figure depends 
+        on `stat`. Figures are saved to `[Compare1D2D.output_path]/figures/longitudinal`
+
+        Example output:
+
+        ![title](../figures/test_results/compare1d2d/BR-PK-IJ.png)
+
+        Parameters:
+            route: List of branches (e.g. ['NK', 'LK'])
+            stat: what type of longitudinal plot to make. Options are: 
+                - time
+                - last25
+                - max13
+            savefig: if true, figure is saved to png file. If false, `FigureOutput` 
+                     returned, which is input for `add_to_fig`
+            add_to_fig: if `FigureOutput` is provided, adds content to figure.  
+        """
+        # Get route and stations along route
+        routename = "-".join(route)
+        
+        match stat:
+            case 'time':
+                datafunc = self._time_func
+            case "last25":
+                datafunc = self._last25
+            case "max13":
+                datafunc = self._max13
+
+        # Make configurable in the future
+        labelfunc = self._lmw_func
+        
+        # TIME FUNCTION plot line every delta_days days
+        lines = datafunc(route=route)
+        
+        # Get figure object
+        if add_to_fig is None:
+            fig, axs = plt.subplots(2, 1, figsize=(12, 12))
+        else:
+            fig = add_to_fig.fig
+            axs = add_to_fig.axes
+    
+        # Filtering which stations to plot
+        if add_to_fig is None:
+            station_names, station_locs, _ = self.get_route(route)
+            st_names, st_locs = labelfunc(station_names, station_locs)
+            h1d = self.get_data_along_route(data=self.data_1D_H, route=route)
+            for st_name, st_loc in zip(st_names, st_locs):
+                for ax in axs:
+                    ax.axvline(x=st_loc, linestyle="--")
+
+                axs[0].text(
+                    st_loc,
+                    h1d.min().min(),
+                    st_name,
+                    fontsize=12,
+                    rotation=90,
+                    horizontalalignment="left",
+                    verticalalignment="bottom",
+                )
+
+        for line in lines:
+
+            axs[0].plot(line.get("1D"), 
+                        label=f"{label} {line.get('label')}")
+            
+            axs[0].set_ylabel("Waterstand [m+NAP]")
             routestr = "-".join(route)
 
             axs[0].set_title(f"route: {routestr}")
 
-            axs[1].plot(h1d - h2d)
+            axs[1].plot(line.get("1D") - line.get("2D"))
             axs[1].set_ylabel("Verschil 1D-2D [m]")
-
+            
             for ax in axs:
-                ax.set_xlabel("rivierkilometers")
+                ax.set_xlabel("Rivierkilometers")
                 ax.xaxis.set_major_locator(MultipleLocator(20))
                 ax.xaxis.set_minor_locator(MultipleLocator(10))
 
-        # bias
-        diff = self.get_data_along_route(
-            data=self.data_1D_H, route=route
-        ) - self.get_data_along_route(data=self.data_2D_H, route=route)
-
-        axs[1].plot(
-            diff.mean(axis=1), "-", linewidth=4, color="#c65387", label="Gemiddeld"
-        )
+        
         axs[1].set_ylim(-1, 1)
-        fig, lgd = PlotStyles.van_veen(fig, use_legend=[False, False])
-        plt.tight_layout()
-        fig.savefig(
-            self.output_path.joinpath(f"figures/longitudinal/{routename}.png"),
-            bbox_extra_artists=[lgd],
-            bbox_inches="tight",
-        )
-        plt.close()
+        fig, lgd = PlotStyles.apply(fig=fig, style=self._plotstyle, use_legend=True)
+
+        if savefig:
+            plt.tight_layout()
+            fig.savefig(
+                self.output_path.joinpath(f"figures/longitudinal/{routename}.png"),
+                bbox_extra_artists=[lgd],
+                bbox_inches="tight",
+            )
+            plt.close()
+
+        else:
+            return FigureOutput(fig=fig, axes = axs, legend=lgd)
 
     def figure_longitudinal_rating_curve(self, route: List[str]) -> None:
         """
         Create a figure along a route with lines at various dicharges.
         To to this, rating curves are generated at each point by digitizing
         the model output.
 
@@ -2239,29 +2370,14 @@
                 verticalalignment="bottom",
             )
 
         # Plot betrekkingslijnen
         texty_previous = -999
         for discharge in discharge_steps:
             axs[0].plot(h1d[discharge], label=f"{discharge:.0f} m$^3$/s")
-            """
-            texty = h1d[discharge].values[-1]
-            texty += max(0, 1 - (texty - texty_previous))
-            texty_previous = texty
-            
-
-            axs[0].text(
-                h1d[discharge].index[-1] + 2,
-                texty,
-                f"{discharge:.0f} m$^3$/s",
-                verticalalignment="center",
-                fontsize=12,
-                bbox={"facecolor": "white", "edgecolor": "none"},
-            )
-            """
             axs[0].set_ylabel("waterstand [m+nap]")
             routestr = "-".join(route)
 
             axs[0].set_title(f"Betrekkingslijnen\n{routestr}")
 
             axs[1].plot(h1d[discharge] - h2d[discharge])
             axs[1].set_ylabel("Verschil 1D-2D [m]")
@@ -2269,15 +2385,15 @@
             for ax in axs:
                 ax.set_xlabel("rivierkilometers")
                 ax.xaxis.set_major_locator(MultipleLocator(20))
                 ax.xaxis.set_minor_locator(MultipleLocator(10))
 
         # style figure
         axs[1].set_ylim(-1, 1)
-        fig, lgd = PlotStyles.van_veen(fig, use_legend=[True, False])
+        fig, lgd = PlotStyles.apply(fig,style=self._plotstyle, use_legend=True)
         plt.tight_layout()
         fig.savefig(
             self.output_path.joinpath(
                 f"figures/longitudinal/{routename}_rating_curve.png",
             ),
             bbox_extra_artists=[lgd],
             bbox_inches="tight",
@@ -2340,15 +2456,15 @@
             ax.text(routedata.columns[0], lmw[1], lmw[0], fontsize=12)
 
         ax.set_ylabel("rivierkilometer")
         ax.set_title(f"{routename}\nheatmap Verschillen in waterstand 1D-2D")
 
         cb = fig.colorbar(im, ax=ax)
         cb.set_label("waterstandsverschil [m+nap]".upper(), rotation=270, labelpad=15)
-        PlotStyles.van_veen(fig, use_legend=[False])
+        PlotStyles.apply(fig, style=self._plotstyle, use_legend=False)
         fig.tight_layout()
         fig.savefig(
             self.output_path.joinpath(f"figures/heatmaps/{routename}_timeseries.png")
         )
         plt.close()
 
     def heatmap_rating_curve(self, route: List[str]) -> None:
@@ -2390,15 +2506,15 @@
             ax.text(routedata.columns[0], lmw[1], lmw[0], fontsize=12)
 
         ax.set_ylabel("rivierkilometer")
         ax.set_title(f"{routename}\nheatmap Verschillen in waterstand 1D-2D")
 
         cb = fig.colorbar(im, ax=ax)
         cb.set_label("waterstandsverschil [m+nap]".upper(), rotation=270, labelpad=15)
-        PlotStyles.van_veen(fig, use_legend=[False])
+        PlotStyles.apply(fig, style=self._plotstyle, use_legend=False)
         fig.tight_layout()
         fig.savefig(
             self.output_path.joinpath(f"figures/heatmaps/{routename}_rating_curve.png")
         )
         plt.close()
 
     @staticmethod
@@ -2716,16 +2832,16 @@
         ax.set_ylim(-8, 30)
         ax2.spines["right"].set_color(_color_width)
         ax2.yaxis.label.set_color(_color_width)
         ax2.tick_params(axis="y", colors=_color_width)
         ax2.set_ylim(0, 1000)
         ax2.grid(False)
 
-        PlotStyles.van_veen()
-        fig, lgd = PlotStyles.van_veen(fig)
+        PlotStyles.apply()
+        fig, lgd = PlotStyles.apply(fig)
 
         plt.savefig(
             output_file,
             bbox_extra_artists=[lgd],
             bbox_inches="tight",
         )
 
@@ -2795,17 +2911,17 @@
                 label=network2.name,
             )
 
             (hdiff,) = axs[1, i].plot(
                 data_2[i][:, 0], data_1[i][:, 1] - data_2[i][:, 1], "--o", linewidth=2
             )
 
-        PlotStyles.van_veen()
+        PlotStyles.apply()
 
-        fig, lgd = PlotStyles.van_veen(fig)
+        fig, lgd = PlotStyles.apply(fig)
         for ax in axs[0]:
             ax.set_xticklabels([])
         for ax in axs[1]:
             ax.set_ylabel("Verschil [m]")
             ax.set_xlabel("Rivierkilometer")
 
         suptitle_label = route[0] if len(route) == 1 else "-".join(route)
```

### Comparing `fm2prof-2.3.1/LICENSE.txt` & `fm2prof-2.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fm2prof-2.3.1/LICENSE_HEADER.txt` & `fm2prof-2.3.2/LICENSE_HEADER.txt`

 * *Files identical despite different names*

### Comparing `fm2prof-2.3.1/pyproject.toml` & `fm2prof-2.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fm2prof"
-version = "2.3.1"
+version = "2.3.2"
 description = ""
 authors = ["Koen Berends <koen.berends@deltares.nl>"]
 license = "GNU LGPL v3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.13"
```

### Comparing `fm2prof-2.3.1/README.md` & `fm2prof-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `fm2prof-2.3.1/PKG-INFO` & `fm2prof-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fm2prof
-Version: 2.3.1
+Version: 2.3.2
 Summary: 
 License: GNU LGPL v3
 Author: Koen Berends
 Author-email: koen.berends@deltares.nl
 Requires-Python: >=3.10,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

