# Comparing `tmp/desalsim-0.3.tar.gz` & `tmp/desalsim-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desalsim-0.3.tar", last modified: Tue May  7 13:17:14 2024, max compression
+gzip compressed data, was "desalsim-0.4.tar", last modified: Tue May  7 13:34:24 2024, max compression
```

## Comparing `desalsim-0.3.tar` & `desalsim-0.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 13:17:14.402748 desalsim-0.3/
-drwxrwxrwx   0        0        0        0 2024-05-07 13:17:14.398759 desalsim-0.3/DesalSim.egg-info/
--rw-rw-rw-   0        0        0     8550 2024-05-07 13:17:14.000000 desalsim-0.3/DesalSim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1276 2024-05-07 13:17:14.000000 desalsim-0.3/DesalSim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 13:17:14.000000 desalsim-0.3/DesalSim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-05-07 13:17:14.000000 desalsim-0.3/DesalSim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-07 13:17:14.000000 desalsim-0.3/DesalSim.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-07 13:17:14.352913 desalsim-0.3/Desalsim/
--rw-rw-rw-   0        0        0      797 2024-05-07 12:54:09.000000 desalsim-0.3/Desalsim/__init__.py
--rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-0.3/Desalsim/constants.py
--rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.3/Desalsim/density_calc.py
--rw-rw-rw-   0        0        0     8821 2024-05-06 16:12:13.000000 desalsim-0.3/Desalsim/economic_f.py
--rw-rw-rw-   0        0        0     2950 2024-04-29 20:32:39.000000 desalsim-0.3/Desalsim/ed_unit_f.py
--rw-rw-rw-   0        0        0    11744 2024-04-29 21:17:33.000000 desalsim-0.3/Desalsim/edbm_unit_f.py
--rw-rw-rw-   0        0        0    49286 2024-02-14 10:34:47.000000 desalsim-0.3/Desalsim/efc_unit_f.py
--rw-rw-rw-   0        0        0     4494 2024-04-29 20:24:16.000000 desalsim-0.3/Desalsim/med_unit_f.py
--rw-rw-rw-   0        0        0    10049 2024-04-29 21:14:03.000000 desalsim-0.3/Desalsim/mfpfr_unit_f.py
--rw-rw-rw-   0        0        0     6987 2024-05-06 08:40:06.000000 desalsim-0.3/Desalsim/nanofiltration_unit_f.py
--rw-rw-rw-   0        0        0     4366 2024-04-29 21:19:41.000000 desalsim-0.3/Desalsim/ro_unit_f.py
--rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.3/Desalsim/scaleup.py
--rw-rw-rw-   0        0        0     8692 2024-04-29 19:44:35.000000 desalsim-0.3/Desalsim/thermal_cryst_f.py
--rw-rw-rw-   0        0        0     1086 2024-02-13 14:36:58.000000 desalsim-0.3/LICENSE
--rw-rw-rw-   0        0        0     8550 2024-05-07 13:17:14.400754 desalsim-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     8225 2024-05-07 12:19:38.000000 desalsim-0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 13:17:14.375290 desalsim-0.3/example/
--rw-rw-rw-   0        0        0      797 2024-05-07 13:01:36.000000 desalsim-0.3/example/__init__.py
--rw-rw-rw-   0        0        0     4531 2024-04-11 13:19:36.000000 desalsim-0.3/example/comparison.py
--rw-rw-rw-   0        0        0     1888 2024-05-06 15:42:19.000000 desalsim-0.3/example/constants.py
--rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.3/example/density_calc.py
--rw-rw-rw-   0        0        0    11978 2024-05-06 16:09:51.000000 desalsim-0.3/example/economic_f.py
--rw-rw-rw-   0        0        0     8663 2024-04-29 21:33:04.000000 desalsim-0.3/example/ed_unit_f.py
--rw-rw-rw-   0        0        0    17118 2024-04-29 21:35:34.000000 desalsim-0.3/example/edbm_unit_f.py
--rw-rw-rw-   0        0        0    49286 2024-02-14 10:34:47.000000 desalsim-0.3/example/efc_unit_f.py
--rw-rw-rw-   0        0        0    33181 2024-05-06 17:04:03.000000 desalsim-0.3/example/example_1.py
--rw-rw-rw-   0        0        0    21599 2024-05-06 16:29:23.000000 desalsim-0.3/example/example_2.py
--rw-rw-rw-   0        0        0     8532 2024-04-29 21:36:53.000000 desalsim-0.3/example/med_unit_f.py
--rw-rw-rw-   0        0        0    14921 2024-05-03 08:06:32.000000 desalsim-0.3/example/mfpfr_unit_f.py
--rw-rw-rw-   0        0        0     9421 2024-05-06 08:39:39.000000 desalsim-0.3/example/nanofiltration_unit_f.py
--rw-rw-rw-   0        0        0     4366 2024-04-29 21:19:41.000000 desalsim-0.3/example/ro_unit_f.py
--rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.3/example/scaleup.py
--rw-rw-rw-   0        0        0    12262 2024-04-29 21:44:17.000000 desalsim-0.3/example/thermal_cryst_f.py
--rw-rw-rw-   0        0        0       42 2024-05-07 13:17:14.402748 desalsim-0.3/setup.cfg
--rw-rw-rw-   0        0        0      609 2024-05-07 13:00:15.000000 desalsim-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 13:17:14.397761 desalsim-0.3/tests/
--rw-rw-rw-   0        0        0      799 2024-05-07 12:54:02.000000 desalsim-0.3/tests/__init__.py
--rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-0.3/tests/constants.py
--rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.3/tests/density_calc.py
--rw-rw-rw-   0        0        0     9094 2024-05-06 16:12:45.000000 desalsim-0.3/tests/economic_f.py
--rw-rw-rw-   0        0        0     2527 2024-05-06 16:15:02.000000 desalsim-0.3/tests/economic_unittest.py
--rw-rw-rw-   0        0        0     3255 2024-05-03 14:14:54.000000 desalsim-0.3/tests/ed_unit_f.py
--rw-rw-rw-   0        0        0     3316 2024-05-03 14:16:37.000000 desalsim-0.3/tests/ed_unittest.py
--rw-rw-rw-   0        0        0    12680 2024-05-03 13:51:25.000000 desalsim-0.3/tests/edbm_unit_f.py
--rw-rw-rw-   0        0        0     8386 2024-05-03 13:50:48.000000 desalsim-0.3/tests/edbm_unittest.py
--rw-rw-rw-   0        0        0     4496 2024-05-02 14:39:30.000000 desalsim-0.3/tests/med_unit_f.py
--rw-rw-rw-   0        0        0     1555 2024-05-03 14:28:38.000000 desalsim-0.3/tests/med_unittest.py
--rw-rw-rw-   0        0        0    10407 2024-05-03 12:57:15.000000 desalsim-0.3/tests/mfpfr_unit_f.py
--rw-rw-rw-   0        0        0     2743 2024-05-03 12:56:18.000000 desalsim-0.3/tests/mfpfr_unittest.py
--rw-rw-rw-   0        0        0     6961 2024-05-06 08:40:27.000000 desalsim-0.3/tests/nanofiltration_unit_f.py
--rw-rw-rw-   0        0        0     1777 2024-05-06 08:40:55.000000 desalsim-0.3/tests/nanofiltration_unittest.py
--rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.3/tests/scaleup.py
--rw-rw-rw-   0        0        0     8687 2024-05-05 10:31:06.000000 desalsim-0.3/tests/thermal_cryst_f.py
--rw-rw-rw-   0        0        0     4560 2024-05-05 10:30:42.000000 desalsim-0.3/tests/thermal_cryst_unittest.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:34:24.415902 desalsim-0.4/
+drwxrwxrwx   0        0        0        0 2024-05-07 13:34:24.412907 desalsim-0.4/DesalSim.egg-info/
+-rw-rw-rw-   0        0        0     8716 2024-05-07 13:34:24.000000 desalsim-0.4/DesalSim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1276 2024-05-07 13:34:24.000000 desalsim-0.4/DesalSim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 13:34:24.000000 desalsim-0.4/DesalSim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-07 13:34:24.000000 desalsim-0.4/DesalSim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-07 13:34:24.000000 desalsim-0.4/DesalSim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 13:34:24.371677 desalsim-0.4/Desalsim/
+-rw-rw-rw-   0        0        0      797 2024-05-07 12:54:09.000000 desalsim-0.4/Desalsim/__init__.py
+-rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-0.4/Desalsim/constants.py
+-rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.4/Desalsim/density_calc.py
+-rw-rw-rw-   0        0        0     8821 2024-05-06 16:12:13.000000 desalsim-0.4/Desalsim/economic_f.py
+-rw-rw-rw-   0        0        0     2950 2024-04-29 20:32:39.000000 desalsim-0.4/Desalsim/ed_unit_f.py
+-rw-rw-rw-   0        0        0    11744 2024-04-29 21:17:33.000000 desalsim-0.4/Desalsim/edbm_unit_f.py
+-rw-rw-rw-   0        0        0    49286 2024-02-14 10:34:47.000000 desalsim-0.4/Desalsim/efc_unit_f.py
+-rw-rw-rw-   0        0        0     4494 2024-04-29 20:24:16.000000 desalsim-0.4/Desalsim/med_unit_f.py
+-rw-rw-rw-   0        0        0    10049 2024-04-29 21:14:03.000000 desalsim-0.4/Desalsim/mfpfr_unit_f.py
+-rw-rw-rw-   0        0        0     6987 2024-05-06 08:40:06.000000 desalsim-0.4/Desalsim/nanofiltration_unit_f.py
+-rw-rw-rw-   0        0        0     4366 2024-04-29 21:19:41.000000 desalsim-0.4/Desalsim/ro_unit_f.py
+-rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.4/Desalsim/scaleup.py
+-rw-rw-rw-   0        0        0     8692 2024-04-29 19:44:35.000000 desalsim-0.4/Desalsim/thermal_cryst_f.py
+-rw-rw-rw-   0        0        0     1086 2024-02-13 14:36:58.000000 desalsim-0.4/LICENSE
+-rw-rw-rw-   0        0        0     8716 2024-05-07 13:34:24.414902 desalsim-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8391 2024-05-07 13:30:19.000000 desalsim-0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 13:34:24.391633 desalsim-0.4/example/
+-rw-rw-rw-   0        0        0      797 2024-05-07 13:01:36.000000 desalsim-0.4/example/__init__.py
+-rw-rw-rw-   0        0        0     4531 2024-04-11 13:19:36.000000 desalsim-0.4/example/comparison.py
+-rw-rw-rw-   0        0        0     1888 2024-05-06 15:42:19.000000 desalsim-0.4/example/constants.py
+-rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.4/example/density_calc.py
+-rw-rw-rw-   0        0        0    11978 2024-05-06 16:09:51.000000 desalsim-0.4/example/economic_f.py
+-rw-rw-rw-   0        0        0     8663 2024-04-29 21:33:04.000000 desalsim-0.4/example/ed_unit_f.py
+-rw-rw-rw-   0        0        0    17118 2024-04-29 21:35:34.000000 desalsim-0.4/example/edbm_unit_f.py
+-rw-rw-rw-   0        0        0    49286 2024-02-14 10:34:47.000000 desalsim-0.4/example/efc_unit_f.py
+-rw-rw-rw-   0        0        0    33181 2024-05-06 17:04:03.000000 desalsim-0.4/example/example_1.py
+-rw-rw-rw-   0        0        0    21599 2024-05-06 16:29:23.000000 desalsim-0.4/example/example_2.py
+-rw-rw-rw-   0        0        0     8532 2024-04-29 21:36:53.000000 desalsim-0.4/example/med_unit_f.py
+-rw-rw-rw-   0        0        0    14921 2024-05-03 08:06:32.000000 desalsim-0.4/example/mfpfr_unit_f.py
+-rw-rw-rw-   0        0        0     9421 2024-05-06 08:39:39.000000 desalsim-0.4/example/nanofiltration_unit_f.py
+-rw-rw-rw-   0        0        0     4366 2024-04-29 21:19:41.000000 desalsim-0.4/example/ro_unit_f.py
+-rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.4/example/scaleup.py
+-rw-rw-rw-   0        0        0    12262 2024-04-29 21:44:17.000000 desalsim-0.4/example/thermal_cryst_f.py
+-rw-rw-rw-   0        0        0       42 2024-05-07 13:34:24.415902 desalsim-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      609 2024-05-07 13:33:35.000000 desalsim-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:34:24.411911 desalsim-0.4/tests/
+-rw-rw-rw-   0        0        0      799 2024-05-07 12:54:02.000000 desalsim-0.4/tests/__init__.py
+-rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-0.4/tests/constants.py
+-rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.4/tests/density_calc.py
+-rw-rw-rw-   0        0        0     9094 2024-05-06 16:12:45.000000 desalsim-0.4/tests/economic_f.py
+-rw-rw-rw-   0        0        0     2527 2024-05-06 16:15:02.000000 desalsim-0.4/tests/economic_unittest.py
+-rw-rw-rw-   0        0        0     3255 2024-05-03 14:14:54.000000 desalsim-0.4/tests/ed_unit_f.py
+-rw-rw-rw-   0        0        0     3316 2024-05-03 14:16:37.000000 desalsim-0.4/tests/ed_unittest.py
+-rw-rw-rw-   0        0        0    12680 2024-05-03 13:51:25.000000 desalsim-0.4/tests/edbm_unit_f.py
+-rw-rw-rw-   0        0        0     8386 2024-05-03 13:50:48.000000 desalsim-0.4/tests/edbm_unittest.py
+-rw-rw-rw-   0        0        0     4496 2024-05-02 14:39:30.000000 desalsim-0.4/tests/med_unit_f.py
+-rw-rw-rw-   0        0        0     1555 2024-05-03 14:28:38.000000 desalsim-0.4/tests/med_unittest.py
+-rw-rw-rw-   0        0        0    10407 2024-05-03 12:57:15.000000 desalsim-0.4/tests/mfpfr_unit_f.py
+-rw-rw-rw-   0        0        0     2743 2024-05-03 12:56:18.000000 desalsim-0.4/tests/mfpfr_unittest.py
+-rw-rw-rw-   0        0        0     6961 2024-05-06 08:40:27.000000 desalsim-0.4/tests/nanofiltration_unit_f.py
+-rw-rw-rw-   0        0        0     1777 2024-05-06 08:40:55.000000 desalsim-0.4/tests/nanofiltration_unittest.py
+-rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.4/tests/scaleup.py
+-rw-rw-rw-   0        0        0     8687 2024-05-05 10:31:06.000000 desalsim-0.4/tests/thermal_cryst_f.py
+-rw-rw-rw-   0        0        0     4560 2024-05-05 10:30:42.000000 desalsim-0.4/tests/thermal_cryst_unittest.py
```

### Comparing `desalsim-0.3/DesalSim.egg-info/PKG-INFO` & `desalsim-0.4/DesalSim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DesalSim
-Version: 0.3
+Version: 0.4
 Home-page: https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
 Author: rodoulak
 Author-email: r.ktori@tudelft.nl
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.0
@@ -89,16 +89,16 @@
 
 Furthermore, a [comparison file](example/comparison.py) is included, where the results of the two examples are compared in terms of various parameters. Users can extend this comparison by adding more indicators as needed.
 
 For more details on input/output parameters and assumption see [Link to Tutorial File](example/Tutorial.md).
 
 ### Documentation 
 You can find Tutorials and documents at: 
-1. [Tutorial File](example/Tutorial.md)
-2. [Tutorial for Example 1](example/Example_1_Tutorial.md)
+1. [Tutorial File](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/Tutorial.md)
+2. [Tutorial for Example 1](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/Example_1_Tutorial.md)
 3. [Economic Tutorial](example/Economic_Tutorial.md)
 4. The mathematical description of each technology is given in [Mathematical description](paper/Mathematical_description.pdf)
 5. [Example 1](example/example_1.py)
 6. [Example 2](example/example_2.py)
 7. [Scenarios comparison](example/comparison.py)
```

### Comparing `desalsim-0.3/DesalSim.egg-info/SOURCES.txt` & `desalsim-0.4/DesalSim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/Desalsim/__init__.py` & `desalsim-0.4/Desalsim/__init__.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/Desalsim/constants.py` & `desalsim-0.4/Desalsim/constants.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/Desalsim/economic_f.py` & `desalsim-0.4/Desalsim/economic_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/Desalsim/ed_unit_f.py` & `desalsim-0.4/Desalsim/ed_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/Desalsim/edbm_unit_f.py` & `desalsim-0.4/Desalsim/edbm_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/Desalsim/efc_unit_f.py` & `desalsim-0.4/Desalsim/efc_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/Desalsim/med_unit_f.py` & `desalsim-0.4/Desalsim/med_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/Desalsim/mfpfr_unit_f.py` & `desalsim-0.4/Desalsim/mfpfr_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/Desalsim/nanofiltration_unit_f.py` & `desalsim-0.4/Desalsim/nanofiltration_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/Desalsim/ro_unit_f.py` & `desalsim-0.4/Desalsim/ro_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/Desalsim/thermal_cryst_f.py` & `desalsim-0.4/Desalsim/thermal_cryst_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/LICENSE` & `desalsim-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/PKG-INFO` & `desalsim-0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DesalSim
-Version: 0.3
+Version: 0.4
 Home-page: https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
 Author: rodoulak
 Author-email: r.ktori@tudelft.nl
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.0
@@ -89,16 +89,16 @@
 
 Furthermore, a [comparison file](example/comparison.py) is included, where the results of the two examples are compared in terms of various parameters. Users can extend this comparison by adding more indicators as needed.
 
 For more details on input/output parameters and assumption see [Link to Tutorial File](example/Tutorial.md).
 
 ### Documentation 
 You can find Tutorials and documents at: 
-1. [Tutorial File](example/Tutorial.md)
-2. [Tutorial for Example 1](example/Example_1_Tutorial.md)
+1. [Tutorial File](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/Tutorial.md)
+2. [Tutorial for Example 1](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/Example_1_Tutorial.md)
 3. [Economic Tutorial](example/Economic_Tutorial.md)
 4. The mathematical description of each technology is given in [Mathematical description](paper/Mathematical_description.pdf)
 5. [Example 1](example/example_1.py)
 6. [Example 2](example/example_2.py)
 7. [Scenarios comparison](example/comparison.py)
```

### Comparing `desalsim-0.3/README.md` & `desalsim-0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -77,16 +77,16 @@
 
 Furthermore, a [comparison file](example/comparison.py) is included, where the results of the two examples are compared in terms of various parameters. Users can extend this comparison by adding more indicators as needed.
 
 For more details on input/output parameters and assumption see [Link to Tutorial File](example/Tutorial.md).
 
 ### Documentation 
 You can find Tutorials and documents at: 
-1. [Tutorial File](example/Tutorial.md)
-2. [Tutorial for Example 1](example/Example_1_Tutorial.md)
+1. [Tutorial File](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/Tutorial.md)
+2. [Tutorial for Example 1](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/Example_1_Tutorial.md)
 3. [Economic Tutorial](example/Economic_Tutorial.md)
 4. The mathematical description of each technology is given in [Mathematical description](paper/Mathematical_description.pdf)
 5. [Example 1](example/example_1.py)
 6. [Example 2](example/example_2.py)
 7. [Scenarios comparison](example/comparison.py)
```

### Comparing `desalsim-0.3/example/__init__.py` & `desalsim-0.4/example/__init__.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/example/comparison.py` & `desalsim-0.4/example/comparison.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/example/constants.py` & `desalsim-0.4/example/constants.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/example/economic_f.py` & `desalsim-0.4/example/economic_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/example/ed_unit_f.py` & `desalsim-0.4/example/ed_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/example/edbm_unit_f.py` & `desalsim-0.4/example/edbm_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/example/efc_unit_f.py` & `desalsim-0.4/example/efc_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/example/example_1.py` & `desalsim-0.4/example/example_1.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/example/example_2.py` & `desalsim-0.4/example/example_2.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/example/med_unit_f.py` & `desalsim-0.4/example/med_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/example/mfpfr_unit_f.py` & `desalsim-0.4/example/mfpfr_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/example/nanofiltration_unit_f.py` & `desalsim-0.4/example/nanofiltration_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/example/ro_unit_f.py` & `desalsim-0.4/example/ro_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/example/thermal_cryst_f.py` & `desalsim-0.4/example/thermal_cryst_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/setup.py` & `desalsim-0.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f: 
     description =f.read()
 
 setup(
       name='DesalSim',
-      version='0.3',
+      version='0.4',
       packages=find_packages(),
       url="https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-",
       author="rodoulak",
       author_email="r.ktori@tudelft.nl",
       license="MIT",
       install_requires=[
           "numpy>=1.0",
```

### Comparing `desalsim-0.3/tests/__init__.py` & `desalsim-0.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/tests/constants.py` & `desalsim-0.4/tests/constants.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/tests/economic_f.py` & `desalsim-0.4/tests/economic_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/tests/economic_unittest.py` & `desalsim-0.4/tests/economic_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/tests/ed_unit_f.py` & `desalsim-0.4/tests/ed_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/tests/ed_unittest.py` & `desalsim-0.4/tests/ed_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/tests/edbm_unit_f.py` & `desalsim-0.4/tests/edbm_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/tests/edbm_unittest.py` & `desalsim-0.4/tests/edbm_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/tests/med_unit_f.py` & `desalsim-0.4/tests/med_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/tests/med_unittest.py` & `desalsim-0.4/tests/med_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/tests/mfpfr_unit_f.py` & `desalsim-0.4/tests/mfpfr_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/tests/mfpfr_unittest.py` & `desalsim-0.4/tests/mfpfr_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/tests/nanofiltration_unit_f.py` & `desalsim-0.4/tests/nanofiltration_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/tests/nanofiltration_unittest.py` & `desalsim-0.4/tests/nanofiltration_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/tests/thermal_cryst_f.py` & `desalsim-0.4/tests/thermal_cryst_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.3/tests/thermal_cryst_unittest.py` & `desalsim-0.4/tests/thermal_cryst_unittest.py`

 * *Files identical despite different names*

