# Comparing `tmp/pyrt_lib_rasmusklitgaard-0.3.9.tar.gz` & `tmp/pyrt_lib_rasmusklitgaard-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrt_lib_rasmusklitgaard-0.3.9.tar", last modified: Wed May  1 13:14:04 2024, max compression
+gzip compressed data, was "pyrt_lib_rasmusklitgaard-0.4.1.tar", last modified: Tue May  7 11:48:10 2024, max compression
```

## Comparing `pyrt_lib_rasmusklitgaard-0.3.9.tar` & `pyrt_lib_rasmusklitgaard-0.4.1.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-01 13:14:04.266215 pyrt_lib_rasmusklitgaard-0.3.9/
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    35076 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.3.9/LICENSE
--rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1776 2024-05-01 13:14:04.266215 pyrt_lib_rasmusklitgaard-0.3.9/PKG-INFO
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      967 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.3.9/README.md
--rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      999 2024-05-01 13:13:58.000000 pyrt_lib_rasmusklitgaard-0.3.9/pyproject.toml
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-01 13:14:04.266215 pyrt_lib_rasmusklitgaard-0.3.9/pyrt_lib_rasmusklitgaard/
--rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      157 2024-05-01 12:58:31.000000 pyrt_lib_rasmusklitgaard-0.3.9/pyrt_lib_rasmusklitgaard/__init__.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4113 2024-05-01 13:14:02.000000 pyrt_lib_rasmusklitgaard-0.3.9/pyrt_lib_rasmusklitgaard/cohort.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    10392 2024-05-01 13:14:02.000000 pyrt_lib_rasmusklitgaard-0.3.9/pyrt_lib_rasmusklitgaard/helpers.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      793 2024-04-09 08:44:14.000000 pyrt_lib_rasmusklitgaard-0.3.9/pyrt_lib_rasmusklitgaard/image_looper.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    14910 2024-05-01 13:14:02.000000 pyrt_lib_rasmusklitgaard-0.3.9/pyrt_lib_rasmusklitgaard/lkb_ntcp.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    32581 2024-05-01 13:14:02.000000 pyrt_lib_rasmusklitgaard-0.3.9/pyrt_lib_rasmusklitgaard/patient.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4724 2024-05-01 13:14:02.000000 pyrt_lib_rasmusklitgaard-0.3.9/pyrt_lib_rasmusklitgaard/resample.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     1242 2024-05-01 13:14:02.000000 pyrt_lib_rasmusklitgaard-0.3.9/pyrt_lib_rasmusklitgaard/select_structures.py
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-01 13:14:04.266215 pyrt_lib_rasmusklitgaard-0.3.9/pyrt_lib_rasmusklitgaard.egg-info/
--rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1776 2024-05-01 13:14:04.000000 pyrt_lib_rasmusklitgaard-0.3.9/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      627 2024-05-01 13:14:04.000000 pyrt_lib_rasmusklitgaard-0.3.9/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)        1 2024-05-01 13:14:04.000000 pyrt_lib_rasmusklitgaard-0.3.9/pyrt_lib_rasmusklitgaard.egg-info/dependency_links.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       74 2024-05-01 13:14:04.000000 pyrt_lib_rasmusklitgaard-0.3.9/pyrt_lib_rasmusklitgaard.egg-info/entry_points.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      140 2024-05-01 13:14:04.000000 pyrt_lib_rasmusklitgaard-0.3.9/pyrt_lib_rasmusklitgaard.egg-info/requires.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       25 2024-05-01 13:14:04.000000 pyrt_lib_rasmusklitgaard-0.3.9/pyrt_lib_rasmusklitgaard.egg-info/top_level.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       38 2024-05-01 13:14:04.266215 pyrt_lib_rasmusklitgaard-0.3.9/setup.cfg
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-07 11:48:10.720611 pyrt_lib_rasmusklitgaard-0.4.1/
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    35076 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.4.1/LICENSE
+-rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1776 2024-05-07 11:48:10.720611 pyrt_lib_rasmusklitgaard-0.4.1/PKG-INFO
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      967 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.4.1/README.md
+-rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)     1060 2024-05-07 11:47:48.000000 pyrt_lib_rasmusklitgaard-0.4.1/pyproject.toml
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-07 11:48:10.720611 pyrt_lib_rasmusklitgaard-0.4.1/pyrt_lib_rasmusklitgaard/
+-rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      150 2024-05-01 13:21:00.000000 pyrt_lib_rasmusklitgaard-0.4.1/pyrt_lib_rasmusklitgaard/__init__.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4113 2024-05-07 11:48:08.000000 pyrt_lib_rasmusklitgaard-0.4.1/pyrt_lib_rasmusklitgaard/cohort.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    11066 2024-05-07 11:48:08.000000 pyrt_lib_rasmusklitgaard-0.4.1/pyrt_lib_rasmusklitgaard/helpers.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      793 2024-04-09 08:44:14.000000 pyrt_lib_rasmusklitgaard-0.4.1/pyrt_lib_rasmusklitgaard/image_looper.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    14910 2024-05-07 11:48:08.000000 pyrt_lib_rasmusklitgaard-0.4.1/pyrt_lib_rasmusklitgaard/lkb_ntcp.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     8758 2024-05-07 11:48:08.000000 pyrt_lib_rasmusklitgaard-0.4.1/pyrt_lib_rasmusklitgaard/parameter_parser.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    32603 2024-05-07 11:48:08.000000 pyrt_lib_rasmusklitgaard-0.4.1/pyrt_lib_rasmusklitgaard/patient.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    12315 2024-05-07 11:48:08.000000 pyrt_lib_rasmusklitgaard-0.4.1/pyrt_lib_rasmusklitgaard/pyrt_database.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4724 2024-05-07 11:48:08.000000 pyrt_lib_rasmusklitgaard-0.4.1/pyrt_lib_rasmusklitgaard/resample.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     1242 2024-05-07 11:48:08.000000 pyrt_lib_rasmusklitgaard-0.4.1/pyrt_lib_rasmusklitgaard/select_structures.py
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-07 11:48:10.720611 pyrt_lib_rasmusklitgaard-0.4.1/pyrt_lib_rasmusklitgaard.egg-info/
+-rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1776 2024-05-07 11:48:10.000000 pyrt_lib_rasmusklitgaard-0.4.1/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      714 2024-05-07 11:48:10.000000 pyrt_lib_rasmusklitgaard-0.4.1/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)        1 2024-05-07 11:48:10.000000 pyrt_lib_rasmusklitgaard-0.4.1/pyrt_lib_rasmusklitgaard.egg-info/dependency_links.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      134 2024-05-07 11:48:10.000000 pyrt_lib_rasmusklitgaard-0.4.1/pyrt_lib_rasmusklitgaard.egg-info/entry_points.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      140 2024-05-07 11:48:10.000000 pyrt_lib_rasmusklitgaard-0.4.1/pyrt_lib_rasmusklitgaard.egg-info/requires.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       25 2024-05-07 11:48:10.000000 pyrt_lib_rasmusklitgaard-0.4.1/pyrt_lib_rasmusklitgaard.egg-info/top_level.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       38 2024-05-07 11:48:10.720611 pyrt_lib_rasmusklitgaard-0.4.1/setup.cfg
```

### Comparing `pyrt_lib_rasmusklitgaard-0.3.9/LICENSE` & `pyrt_lib_rasmusklitgaard-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.3.9/PKG-INFO` & `pyrt_lib_rasmusklitgaard-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrt_lib_rasmusklitgaard
-Version: 0.3.9
+Version: 0.4.1
 Summary: PYthon RadioTherapy library
 Author-email: Rasmus Klitgaard <rasmusklitgaard97@gmail.com>
 Project-URL: Homepage, https://gitlab.com/dcpt-research/pyrt-lib
 Project-URL: Issues, https://gitlab.com/dcpt-research/pyrt-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrt_lib_rasmusklitgaard-0.3.9/README.md` & `pyrt_lib_rasmusklitgaard-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.3.9/pyproject.toml` & `pyrt_lib_rasmusklitgaard-0.4.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "pyrt_lib_rasmusklitgaard"
-version = "0.3.9"
+version = "0.4.1"
 authors = [
   { name="Rasmus Klitgaard", email="rasmusklitgaard97@gmail.com" },
 ]
 description = "PYthon RadioTherapy library"
 readme = "README.md"
 dependencies = [
 "numpy>=1.26.3",
@@ -24,16 +24,16 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.scripts]
-resample_dicom = "pyrt_lib_rasmusklitgaard:resample.main"
-
+resample_dicom = "pyrt_lib_rasmusklitgaard.resample:main"
+pyrt_database = "pyrt_lib_rasmusklitgaard.pyrt_database:main"
 
 [project.urls]
 Homepage = "https://gitlab.com/dcpt-research/pyrt-lib"
 Issues = "https://gitlab.com/dcpt-research/pyrt-lib/issues"
 [tool.hatch.build.targets.wheel]
 only-include = ["pyrt_lib_rasmusklitgaard"]
```

### Comparing `pyrt_lib_rasmusklitgaard-0.3.9/pyrt_lib_rasmusklitgaard/cohort.py` & `pyrt_lib_rasmusklitgaard-0.4.1/pyrt_lib_rasmusklitgaard/cohort.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.3.9/pyrt_lib_rasmusklitgaard/helpers.py` & `pyrt_lib_rasmusklitgaard-0.4.1/pyrt_lib_rasmusklitgaard/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,32 @@
 from shutil import which
 import subprocess
 import os
 import tempfile
 import string
 
 
+def calculate_vh(data_array, stepsize=0.1, nsteps = None):
+    data_array = np.array(data_array)
+    full_volume = np.prod(np.shape(data_array))
+
+    value_array = np.array([0,0])
+    if stepsize != 0:
+        value_array = np.arange(0, np.max(data_array), stepsize)
+
+    if nsteps:
+        value_array = np.linspace(0, np.max(data_array), nsteps)
+    if len(value_array) == 1:
+        value_array = np.append(value_array, stepsize)
+    volume_array = np.zeros_like(value_array)
+    for i,v in enumerate(value_array):
+        sub_volume = np.prod(np.shape(data_array[data_array>v]))
+        volume_array[i] = sub_volume
+    return (value_array, volume_array / full_volume)
+
 def get_patient_metadata(patient_data_sheet, patient_id):
 	this_patient_row = -1
 	# now we need to find the row with this patient id
 	for row_i in range(1,1500):
 		if str(patient_data_sheet["A{}".format(row_i)].value) == patient_id:
 			this_patient_row = row_i
 			break
```

### Comparing `pyrt_lib_rasmusklitgaard-0.3.9/pyrt_lib_rasmusklitgaard/image_looper.py` & `pyrt_lib_rasmusklitgaard-0.4.1/pyrt_lib_rasmusklitgaard/image_looper.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.3.9/pyrt_lib_rasmusklitgaard/lkb_ntcp.py` & `pyrt_lib_rasmusklitgaard-0.4.1/pyrt_lib_rasmusklitgaard/lkb_ntcp.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.3.9/pyrt_lib_rasmusklitgaard/patient.py` & `pyrt_lib_rasmusklitgaard-0.4.1/pyrt_lib_rasmusklitgaard/patient.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,16 +48,17 @@
 		self.set_default_rtdoses()
 		t6=time.time()
 
 		try:
 			if self.wanted_structures == "default":
 				self.wanted_structures = ["ctv", "bladder", "bladder wall", "rectum", "rectal wall", "Bladder Wall", "Rectal Wall", "Rectum", "Bladder", "CTV", "Rectal_Wall", "Bladder_Wall"]
 			self.actual_structure_names = self.get_actual_structure_names(self.wanted_structures)
-		except AttributeError:
+		except AttributeError as e:
 			print("THERE HAS BEEN AN ATTRIBUTE ERROR")
+			print(str(e))
 			code_interact(globals(),locals())
 		t7=time.time()
 
 		self.set_structure_indices()
 		t8=time.time()
```

### Comparing `pyrt_lib_rasmusklitgaard-0.3.9/pyrt_lib_rasmusklitgaard/resample.py` & `pyrt_lib_rasmusklitgaard-0.4.1/pyrt_lib_rasmusklitgaard/resample.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.3.9/pyrt_lib_rasmusklitgaard/select_structures.py` & `pyrt_lib_rasmusklitgaard-0.4.1/pyrt_lib_rasmusklitgaard/select_structures.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.3.9/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO` & `pyrt_lib_rasmusklitgaard-0.4.1/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrt_lib_rasmusklitgaard
-Version: 0.3.9
+Version: 0.4.1
 Summary: PYthon RadioTherapy library
 Author-email: Rasmus Klitgaard <rasmusklitgaard97@gmail.com>
 Project-URL: Homepage, https://gitlab.com/dcpt-research/pyrt-lib
 Project-URL: Issues, https://gitlab.com/dcpt-research/pyrt-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrt_lib_rasmusklitgaard-0.3.9/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt` & `pyrt_lib_rasmusklitgaard-0.4.1/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 README.md
 pyproject.toml
 pyrt_lib_rasmusklitgaard/__init__.py
 pyrt_lib_rasmusklitgaard/cohort.py
 pyrt_lib_rasmusklitgaard/helpers.py
 pyrt_lib_rasmusklitgaard/image_looper.py
 pyrt_lib_rasmusklitgaard/lkb_ntcp.py
+pyrt_lib_rasmusklitgaard/parameter_parser.py
 pyrt_lib_rasmusklitgaard/patient.py
+pyrt_lib_rasmusklitgaard/pyrt_database.py
 pyrt_lib_rasmusklitgaard/resample.py
 pyrt_lib_rasmusklitgaard/select_structures.py
 pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO
 pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt
 pyrt_lib_rasmusklitgaard.egg-info/dependency_links.txt
 pyrt_lib_rasmusklitgaard.egg-info/entry_points.txt
 pyrt_lib_rasmusklitgaard.egg-info/requires.txt
```

