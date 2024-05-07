# Comparing `tmp/omniplate-1.0a0.tar.gz` & `tmp/omniplate-1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniplate-1.0a0.tar", max compression
+gzip compressed data, was "omniplate-1.0b0.tar", max compression
```

## Comparing `omniplate-1.0a0.tar` & `omniplate-1.0b0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      244 2024-03-04 11:11:29.000000 omniplate-1.0a0/README.md
--rw-r--r--   0        0        0      201 2024-03-08 17:39:22.000000 omniplate-1.0a0/omniplate/__init__.py
--rw-r--r--   0        0        0     4163 2024-04-12 15:46:43.988619 omniplate-1.0a0/omniplate/admin.py
--rw-r--r--   0        0        0     1289 2024-03-08 11:28:12.000000 omniplate-1.0a0/omniplate/clogger.py
--rw-r--r--   0        0        0    12877 2024-04-18 12:59:13.108428 omniplate-1.0a0/omniplate/correctauto_bayesian.py
--rw-r--r--   0        0        0    41253 2024-04-18 11:20:14.135894 omniplate-1.0a0/omniplate/corrections.py
--rw-r--r--   0        0        0     1380 2024-03-08 11:28:21.000000 omniplate-1.0a0/omniplate/dilution_data_lucia.tsv
--rw-r--r--   0        0        0     1893 2024-03-08 11:28:21.000000 omniplate-1.0a0/omniplate/dilution_data_xiao.tsv
--rw-r--r--   0        0        0     9484 2024-03-14 12:17:12.097073 omniplate-1.0a0/omniplate/getstats.py
--rw-r--r--   0        0        0    12333 2024-03-31 12:04:44.000000 omniplate-1.0a0/omniplate/loaddata.py
--rw-r--r--   0        0        0    19121 2024-03-21 16:51:56.721344 omniplate-1.0a0/omniplate/manipulatedfs.py
--rw-r--r--   0        0        0     8791 2024-04-12 15:48:50.293118 omniplate-1.0a0/omniplate/midlog.py
--rw-r--r--   0        0        0    10217 2024-03-14 12:18:53.929142 omniplate-1.0a0/omniplate/misc.py
--rw-r--r--   0        0        0     2577 2024-03-08 11:28:12.000000 omniplate-1.0a0/omniplate/old_analyseOldTecan.py
--rw-r--r--   0        0        0     2609 2024-03-08 11:28:12.000000 omniplate-1.0a0/omniplate/old_analyseTecan.py
--rw-r--r--   0        0        0      435 2024-03-08 11:28:12.000000 omniplate-1.0a0/omniplate/omerrors.py
--rw-r--r--   0        0        0    12992 2024-04-15 18:29:26.000000 omniplate-1.0a0/omniplate/omfitderiv.py
--rw-r--r--   0        0        0     3925 2024-03-08 11:28:12.000000 omniplate-1.0a0/omniplate/omgenutils.py
--rw-r--r--   0        0        0     3274 2024-03-08 12:42:05.000000 omniplate-1.0a0/omniplate/ominfo.py
--rw-r--r--   0        0        0     6320 2024-03-27 15:57:57.000000 omniplate-1.0a0/omniplate/omio.py
--rw-r--r--   0        0        0    21013 2024-03-14 12:18:28.204783 omniplate-1.0a0/omniplate/omplot.py
--rw-r--r--   0        0        0     6794 2024-03-08 11:28:12.000000 omniplate-1.0a0/omniplate/omstats.py
--rw-r--r--   0        0        0     6907 2024-03-08 12:21:15.000000 omniplate-1.0a0/omniplate/omwells.py
--rw-r--r--   0        0        0      797 2024-03-08 11:28:12.000000 omniplate-1.0a0/omniplate/parseSunrise.py
--rw-r--r--   0        0        0     1598 2024-03-08 11:28:12.000000 omniplate-1.0a0/omniplate/parseTecan.py
--rw-r--r--   0        0        0     2898 2024-03-08 15:11:40.000000 omniplate-1.0a0/omniplate/parseplate.py
--rw-r--r--   0        0        0     6199 2024-03-31 12:15:36.000000 omniplate-1.0a0/omniplate/platereader.py
--rw-r--r--   0        0        0     6620 2024-03-31 16:27:06.000000 omniplate-1.0a0/omniplate/promoteractivity.py
--rw-r--r--   0        0        0     6232 2024-04-15 18:27:00.000000 omniplate-1.0a0/omniplate/runfitderiv.py
--rw-r--r--   0        0        0     5285 2024-03-25 14:18:47.000000 omniplate-1.0a0/omniplate/sunder.py
--rw-r--r--   0        0        0     1108 2024-04-25 14:26:31.547279 omniplate-1.0a0/pyproject.toml
--rw-r--r--   0        0        0     1534 1970-01-01 00:00:00.000000 omniplate-1.0a0/PKG-INFO
+-rw-r--r--   0        0        0      244 2024-03-04 11:11:29.000000 omniplate-1.0b0/README.md
+-rw-r--r--   0        0        0      201 2024-03-08 17:39:22.000000 omniplate-1.0b0/omniplate/__init__.py
+-rw-r--r--   0        0        0     4163 2024-04-12 15:46:43.988619 omniplate-1.0b0/omniplate/admin.py
+-rw-r--r--   0        0        0     1289 2024-03-08 11:28:12.000000 omniplate-1.0b0/omniplate/clogger.py
+-rw-r--r--   0        0        0    12877 2024-04-18 12:59:13.108428 omniplate-1.0b0/omniplate/correctauto_bayesian.py
+-rw-r--r--   0        0        0    41253 2024-04-18 11:20:14.135894 omniplate-1.0b0/omniplate/corrections.py
+-rw-r--r--   0        0        0     1380 2024-03-08 11:28:21.000000 omniplate-1.0b0/omniplate/dilution_data_lucia.tsv
+-rw-r--r--   0        0        0     1893 2024-03-08 11:28:21.000000 omniplate-1.0b0/omniplate/dilution_data_xiao.tsv
+-rw-r--r--   0        0        0     9484 2024-03-14 12:17:12.097073 omniplate-1.0b0/omniplate/getstats.py
+-rw-r--r--   0        0        0    12637 2024-05-07 15:58:40.479331 omniplate-1.0b0/omniplate/loaddata.py
+-rw-r--r--   0        0        0    19121 2024-03-21 16:51:56.721344 omniplate-1.0b0/omniplate/manipulatedfs.py
+-rw-r--r--   0        0        0     8791 2024-04-12 15:48:50.293118 omniplate-1.0b0/omniplate/midlog.py
+-rw-r--r--   0        0        0    10217 2024-03-14 12:18:53.929142 omniplate-1.0b0/omniplate/misc.py
+-rw-r--r--   0        0        0     2577 2024-03-08 11:28:12.000000 omniplate-1.0b0/omniplate/old_analyseOldTecan.py
+-rw-r--r--   0        0        0     2609 2024-03-08 11:28:12.000000 omniplate-1.0b0/omniplate/old_analyseTecan.py
+-rw-r--r--   0        0        0      435 2024-03-08 11:28:12.000000 omniplate-1.0b0/omniplate/omerrors.py
+-rw-r--r--   0        0        0    12992 2024-04-15 18:29:26.000000 omniplate-1.0b0/omniplate/omfitderiv.py
+-rw-r--r--   0        0        0     3925 2024-03-08 11:28:12.000000 omniplate-1.0b0/omniplate/omgenutils.py
+-rw-r--r--   0        0        0     3274 2024-03-08 12:42:05.000000 omniplate-1.0b0/omniplate/ominfo.py
+-rw-r--r--   0        0        0     6320 2024-03-27 15:57:57.000000 omniplate-1.0b0/omniplate/omio.py
+-rw-r--r--   0        0        0    21013 2024-03-14 12:18:28.204783 omniplate-1.0b0/omniplate/omplot.py
+-rw-r--r--   0        0        0     6794 2024-03-08 11:28:12.000000 omniplate-1.0b0/omniplate/omstats.py
+-rw-r--r--   0        0        0     6907 2024-03-08 12:21:15.000000 omniplate-1.0b0/omniplate/omwells.py
+-rw-r--r--   0        0        0      797 2024-03-08 11:28:12.000000 omniplate-1.0b0/omniplate/parseSunrise.py
+-rw-r--r--   0        0        0     1598 2024-03-08 11:28:12.000000 omniplate-1.0b0/omniplate/parseTecan.py
+-rw-r--r--   0        0        0     2898 2024-03-08 15:11:40.000000 omniplate-1.0b0/omniplate/parseplate.py
+-rw-r--r--   0        0        0     6199 2024-03-31 12:15:36.000000 omniplate-1.0b0/omniplate/platereader.py
+-rw-r--r--   0        0        0     6620 2024-03-31 16:27:06.000000 omniplate-1.0b0/omniplate/promoteractivity.py
+-rw-r--r--   0        0        0     6232 2024-04-15 18:27:00.000000 omniplate-1.0b0/omniplate/runfitderiv.py
+-rw-r--r--   0        0        0     5285 2024-03-25 14:18:47.000000 omniplate-1.0b0/omniplate/sunder.py
+-rw-r--r--   0        0        0     1108 2024-05-07 15:59:18.978773 omniplate-1.0b0/pyproject.toml
+-rw-r--r--   0        0        0     1534 1970-01-01 00:00:00.000000 omniplate-1.0b0/PKG-INFO
```

### Comparing `omniplate-1.0a0/omniplate/admin.py` & `omniplate-1.0b0/omniplate/admin.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0a0/omniplate/clogger.py` & `omniplate-1.0b0/omniplate/clogger.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0a0/omniplate/correctauto_bayesian.py` & `omniplate-1.0b0/omniplate/correctauto_bayesian.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0a0/omniplate/corrections.py` & `omniplate-1.0b0/omniplate/corrections.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0a0/omniplate/dilution_data_lucia.tsv` & `omniplate-1.0b0/omniplate/dilution_data_lucia.tsv`

 * *Files identical despite different names*

### Comparing `omniplate-1.0a0/omniplate/dilution_data_xiao.tsv` & `omniplate-1.0b0/omniplate/dilution_data_xiao.tsv`

 * *Files identical despite different names*

### Comparing `omniplate-1.0a0/omniplate/getstats.py` & `omniplate-1.0b0/omniplate/getstats.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0a0/omniplate/loaddata.py` & `omniplate-1.0b0/omniplate/loaddata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # functions to load the data generated by the plate reader
 # and to parse the annotation file
 import re
 
 import numpy as np
 import pandas as pd
-from scipy import stats
 
 import omniplate.admin as admin
 import omniplate.clogger as clogger
 import omniplate.omerrors as errors
 import omniplate.omgenutils as gu
 from omniplate.parseplate import parseplate
 
@@ -19,14 +18,15 @@
     dnames,
     anames=False,
     platereadertype="Tecan",
     dsheetnumbers=False,
     asheetnumbers=False,
     info=True,
     combine=False,
+    min_dt=0.05,
 ):
     """
     Load raw data files.
 
     Two files are required: one generated by the plate reader and the other
     the corresponding annotation files - both assumed to be xlsx.
 
@@ -48,14 +48,17 @@
         annotation.
     info: boolean
         If True (default), display summary information on the data once
         loaded.
     combine: boolean
         If True (default is False), combine all the data loaded into one
         single experiment.
+    min_dt: float, optional
+        The minimum time interval taken by the plate reader between
+        measurements. Used only when combine=True.
 
     Examples
     -------
     >>> p.load('Data.xlsx', 'DataContents.xlsx')
     >>> p.load('Data.xlsx', 'DataContents.xlsx', info= False)
     """
     dnames = gu.makelist(dnames)
@@ -136,15 +139,15 @@
         self.info
     print(
         '\nWarning: wells with no strains have been changed to "Null"'
         "\nto avoid confusion with pandas.\n"
     )
     # combine into one experiment
     if combine:
-        self.combine_experiments()
+        self.combine_experiments(min_dt=min_dt)
 
 
 def loaddatafiles(
     platereadertype, wdirpath, dname, dsheetnumber, aname, asheetnumber
 ):
     """Call functions to parse data and metadate from the input files."""
     experiment = dname.split(".")[0]
@@ -230,15 +233,15 @@
             )
         )
         return allconditions, allstrains, alldata, wellcontents
     except FileNotFoundError as exc:
         raise errors.FileNotFound(str(wdirpath / aname)) from exc
 
 
-def combine_experiments(self, combined="combined"):
+def combine_experiments(self, min_dt, combined="combined"):
     """
     Combine raw data from all loaded experiments into one experiment.
 
     Only to be run immediately after first loading the data.
 
     Wells are relabelled with a prefix denoting their original
     experiment.
@@ -257,15 +260,20 @@
     datatypes = [
         col
         for col in list(self.r.columns)
         if col not in ["experiment", "condition", "strain", "well", "time"]
     ]
     # define a new universal time
     unique_t = np.sort(self.r.time.unique())
-    dt = np.round(stats.mode(np.diff(unique_t))[0], 2)
+    ut_values, ut_counts = np.unique(
+        np.round(np.diff(unique_t), 2), return_counts=True
+    )
+    dt = ut_values[ut_values > min_dt][
+        np.argmax(ut_counts[ut_values > min_dt])
+    ]
     print(f" Using dt = {dt:.2f}.")
     nt = np.arange(0, unique_t.max(), dt)
     # find index for all wells
     wells_index = list(
         self.r.groupby(["experiment", "condition", "strain", "well"])
         .mean()
         .index
```

### Comparing `omniplate-1.0a0/omniplate/manipulatedfs.py` & `omniplate-1.0b0/omniplate/manipulatedfs.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0a0/omniplate/midlog.py` & `omniplate-1.0b0/omniplate/midlog.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0a0/omniplate/misc.py` & `omniplate-1.0b0/omniplate/misc.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0a0/omniplate/old_analyseOldTecan.py` & `omniplate-1.0b0/omniplate/old_analyseOldTecan.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0a0/omniplate/old_analyseTecan.py` & `omniplate-1.0b0/omniplate/old_analyseTecan.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0a0/omniplate/omfitderiv.py` & `omniplate-1.0b0/omniplate/omfitderiv.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0a0/omniplate/omgenutils.py` & `omniplate-1.0b0/omniplate/omgenutils.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0a0/omniplate/ominfo.py` & `omniplate-1.0b0/omniplate/ominfo.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0a0/omniplate/omio.py` & `omniplate-1.0b0/omniplate/omio.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0a0/omniplate/omplot.py` & `omniplate-1.0b0/omniplate/omplot.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0a0/omniplate/omstats.py` & `omniplate-1.0b0/omniplate/omstats.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0a0/omniplate/omwells.py` & `omniplate-1.0b0/omniplate/omwells.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0a0/omniplate/parseSunrise.py` & `omniplate-1.0b0/omniplate/parseSunrise.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0a0/omniplate/parseTecan.py` & `omniplate-1.0b0/omniplate/parseTecan.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0a0/omniplate/parseplate.py` & `omniplate-1.0b0/omniplate/parseplate.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0a0/omniplate/platereader.py` & `omniplate-1.0b0/omniplate/platereader.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0a0/omniplate/promoteractivity.py` & `omniplate-1.0b0/omniplate/promoteractivity.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0a0/omniplate/runfitderiv.py` & `omniplate-1.0b0/omniplate/runfitderiv.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0a0/omniplate/sunder.py` & `omniplate-1.0b0/omniplate/sunder.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0a0/pyproject.toml` & `omniplate-1.0b0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omniplate"
-version = "1.0a"
+version = "1.0b"
 description = "For analysing and meta-analysing plate-reader data"
 authors = ["Peter Swain <peter.swain@ed.ac.uk>"]
 
 license = "MIT"
 readme = "README.md"
 homepage = "https://swainlab.bio.ed.ac.uk/software/omniplate"
 repository = "https://git.ecdf.ed.ac.uk/pswain/omniplate"
```

### Comparing `omniplate-1.0a0/PKG-INFO` & `omniplate-1.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniplate
-Version: 1.0a0
+Version: 1.0b0
 Summary: For analysing and meta-analysing plate-reader data
 Home-page: https://swainlab.bio.ed.ac.uk/software/omniplate
 License: MIT
 Keywords: omniplate,systems biology,bioinformatics,plate readers
 Author: Peter Swain
 Author-email: peter.swain@ed.ac.uk
 Requires-Python: >=3.8,<3.11
```

