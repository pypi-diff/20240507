# Comparing `tmp/DesalSim-0.2.tar.gz` & `tmp/desalsim-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DesalSim-0.2.tar", last modified: Tue May  7 11:05:40 2024, max compression
+gzip compressed data, was "desalsim-0.3.tar", last modified: Tue May  7 13:17:14 2024, max compression
```

## Comparing `DesalSim-0.2.tar` & `desalsim-0.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 11:05:40.224807 DesalSim-0.2/
-drwxrwxrwx   0        0        0        0 2024-05-07 11:05:40.167943 DesalSim-0.2/DesalSim.egg-info/
--rw-rw-rw-   0        0        0     8306 2024-05-07 11:05:40.000000 DesalSim-0.2/DesalSim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1588 2024-05-07 11:05:40.000000 DesalSim-0.2/DesalSim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 11:05:40.000000 DesalSim-0.2/DesalSim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-05-07 11:05:40.000000 DesalSim-0.2/DesalSim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       47 2024-05-07 11:05:40.000000 DesalSim-0.2/DesalSim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2024-02-13 14:36:58.000000 DesalSim-0.2/LICENSE
--rw-rw-rw-   0        0        0     8306 2024-05-07 11:05:40.224807 DesalSim-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     8036 2024-05-07 09:19:02.000000 DesalSim-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 11:05:40.183905 DesalSim-0.2/desalination_and_brine_treatment/
--rw-rw-rw-   0        0        0     1128 2024-04-29 21:23:31.000000 DesalSim-0.2/desalination_and_brine_treatment/__init__.py
--rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 DesalSim-0.2/desalination_and_brine_treatment/constants.py
--rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 DesalSim-0.2/desalination_and_brine_treatment/density_calc.py
--rw-rw-rw-   0        0        0     8821 2024-05-06 16:12:13.000000 DesalSim-0.2/desalination_and_brine_treatment/economic_f.py
--rw-rw-rw-   0        0        0     2950 2024-04-29 20:32:39.000000 DesalSim-0.2/desalination_and_brine_treatment/ed_unit_f.py
--rw-rw-rw-   0        0        0    11744 2024-04-29 21:17:33.000000 DesalSim-0.2/desalination_and_brine_treatment/edbm_unit_f.py
--rw-rw-rw-   0        0        0    49286 2024-02-14 10:34:47.000000 DesalSim-0.2/desalination_and_brine_treatment/efc_unit_f.py
--rw-rw-rw-   0        0        0     4494 2024-04-29 20:24:16.000000 DesalSim-0.2/desalination_and_brine_treatment/med_unit_f.py
--rw-rw-rw-   0        0        0    10049 2024-04-29 21:14:03.000000 DesalSim-0.2/desalination_and_brine_treatment/mfpfr_unit_f.py
--rw-rw-rw-   0        0        0     6987 2024-05-06 08:40:06.000000 DesalSim-0.2/desalination_and_brine_treatment/nanofiltration_unit_f.py
--rw-rw-rw-   0        0        0     4366 2024-04-29 21:19:41.000000 DesalSim-0.2/desalination_and_brine_treatment/ro_unit_f.py
--rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 DesalSim-0.2/desalination_and_brine_treatment/scaleup.py
--rw-rw-rw-   0        0        0     8692 2024-04-29 19:44:35.000000 DesalSim-0.2/desalination_and_brine_treatment/thermal_cryst_f.py
-drwxrwxrwx   0        0        0        0 2024-05-07 11:05:40.202851 DesalSim-0.2/example/
--rw-rw-rw-   0        0        0     1128 2024-04-25 10:11:01.000000 DesalSim-0.2/example/__init__.py
--rw-rw-rw-   0        0        0     4531 2024-04-11 13:19:36.000000 DesalSim-0.2/example/comparison.py
--rw-rw-rw-   0        0        0     1888 2024-05-06 15:42:19.000000 DesalSim-0.2/example/constants.py
--rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 DesalSim-0.2/example/density_calc.py
--rw-rw-rw-   0        0        0    11978 2024-05-06 16:09:51.000000 DesalSim-0.2/example/economic_f.py
--rw-rw-rw-   0        0        0     8663 2024-04-29 21:33:04.000000 DesalSim-0.2/example/ed_unit_f.py
--rw-rw-rw-   0        0        0    17118 2024-04-29 21:35:34.000000 DesalSim-0.2/example/edbm_unit_f.py
--rw-rw-rw-   0        0        0    49286 2024-02-14 10:34:47.000000 DesalSim-0.2/example/efc_unit_f.py
--rw-rw-rw-   0        0        0    33181 2024-05-06 17:04:03.000000 DesalSim-0.2/example/example_1.py
--rw-rw-rw-   0        0        0    21599 2024-05-06 16:29:23.000000 DesalSim-0.2/example/example_2.py
--rw-rw-rw-   0        0        0     8532 2024-04-29 21:36:53.000000 DesalSim-0.2/example/med_unit_f.py
--rw-rw-rw-   0        0        0    14921 2024-05-03 08:06:32.000000 DesalSim-0.2/example/mfpfr_unit_f.py
--rw-rw-rw-   0        0        0     9421 2024-05-06 08:39:39.000000 DesalSim-0.2/example/nanofiltration_unit_f.py
--rw-rw-rw-   0        0        0     4366 2024-04-29 21:19:41.000000 DesalSim-0.2/example/ro_unit_f.py
--rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 DesalSim-0.2/example/scaleup.py
--rw-rw-rw-   0        0        0    12262 2024-04-29 21:44:17.000000 DesalSim-0.2/example/thermal_cryst_f.py
--rw-rw-rw-   0        0        0       42 2024-05-07 11:05:40.224807 DesalSim-0.2/setup.cfg
--rw-rw-rw-   0        0        0      609 2024-05-07 09:54:29.000000 DesalSim-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 11:05:40.222813 DesalSim-0.2/tests/
--rw-rw-rw-   0        0        0     1128 2024-04-25 10:11:01.000000 DesalSim-0.2/tests/__init__.py
--rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 DesalSim-0.2/tests/constants.py
--rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 DesalSim-0.2/tests/density_calc.py
--rw-rw-rw-   0        0        0     9094 2024-05-06 16:12:45.000000 DesalSim-0.2/tests/economic_f.py
--rw-rw-rw-   0        0        0     2527 2024-05-06 16:15:02.000000 DesalSim-0.2/tests/economic_unittest.py
--rw-rw-rw-   0        0        0     3255 2024-05-03 14:14:54.000000 DesalSim-0.2/tests/ed_unit_f.py
--rw-rw-rw-   0        0        0     3316 2024-05-03 14:16:37.000000 DesalSim-0.2/tests/ed_unittest.py
--rw-rw-rw-   0        0        0    12680 2024-05-03 13:51:25.000000 DesalSim-0.2/tests/edbm_unit_f.py
--rw-rw-rw-   0        0        0     8386 2024-05-03 13:50:48.000000 DesalSim-0.2/tests/edbm_unittest.py
--rw-rw-rw-   0        0        0     4496 2024-05-02 14:39:30.000000 DesalSim-0.2/tests/med_unit_f.py
--rw-rw-rw-   0        0        0     1555 2024-05-03 14:28:38.000000 DesalSim-0.2/tests/med_unittest.py
--rw-rw-rw-   0        0        0    10407 2024-05-03 12:57:15.000000 DesalSim-0.2/tests/mfpfr_unit_f.py
--rw-rw-rw-   0        0        0     2743 2024-05-03 12:56:18.000000 DesalSim-0.2/tests/mfpfr_unittest.py
--rw-rw-rw-   0        0        0     6961 2024-05-06 08:40:27.000000 DesalSim-0.2/tests/nanofiltration_unit_f.py
--rw-rw-rw-   0        0        0     1777 2024-05-06 08:40:55.000000 DesalSim-0.2/tests/nanofiltration_unittest.py
--rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 DesalSim-0.2/tests/scaleup.py
--rw-rw-rw-   0        0        0     8687 2024-05-05 10:31:06.000000 DesalSim-0.2/tests/thermal_cryst_f.py
--rw-rw-rw-   0        0        0     4560 2024-05-05 10:30:42.000000 DesalSim-0.2/tests/thermal_cryst_unittest.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:17:14.402748 desalsim-0.3/
+drwxrwxrwx   0        0        0        0 2024-05-07 13:17:14.398759 desalsim-0.3/DesalSim.egg-info/
+-rw-rw-rw-   0        0        0     8550 2024-05-07 13:17:14.000000 desalsim-0.3/DesalSim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1276 2024-05-07 13:17:14.000000 desalsim-0.3/DesalSim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 13:17:14.000000 desalsim-0.3/DesalSim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-07 13:17:14.000000 desalsim-0.3/DesalSim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-07 13:17:14.000000 desalsim-0.3/DesalSim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 13:17:14.352913 desalsim-0.3/Desalsim/
+-rw-rw-rw-   0        0        0      797 2024-05-07 12:54:09.000000 desalsim-0.3/Desalsim/__init__.py
+-rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-0.3/Desalsim/constants.py
+-rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.3/Desalsim/density_calc.py
+-rw-rw-rw-   0        0        0     8821 2024-05-06 16:12:13.000000 desalsim-0.3/Desalsim/economic_f.py
+-rw-rw-rw-   0        0        0     2950 2024-04-29 20:32:39.000000 desalsim-0.3/Desalsim/ed_unit_f.py
+-rw-rw-rw-   0        0        0    11744 2024-04-29 21:17:33.000000 desalsim-0.3/Desalsim/edbm_unit_f.py
+-rw-rw-rw-   0        0        0    49286 2024-02-14 10:34:47.000000 desalsim-0.3/Desalsim/efc_unit_f.py
+-rw-rw-rw-   0        0        0     4494 2024-04-29 20:24:16.000000 desalsim-0.3/Desalsim/med_unit_f.py
+-rw-rw-rw-   0        0        0    10049 2024-04-29 21:14:03.000000 desalsim-0.3/Desalsim/mfpfr_unit_f.py
+-rw-rw-rw-   0        0        0     6987 2024-05-06 08:40:06.000000 desalsim-0.3/Desalsim/nanofiltration_unit_f.py
+-rw-rw-rw-   0        0        0     4366 2024-04-29 21:19:41.000000 desalsim-0.3/Desalsim/ro_unit_f.py
+-rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.3/Desalsim/scaleup.py
+-rw-rw-rw-   0        0        0     8692 2024-04-29 19:44:35.000000 desalsim-0.3/Desalsim/thermal_cryst_f.py
+-rw-rw-rw-   0        0        0     1086 2024-02-13 14:36:58.000000 desalsim-0.3/LICENSE
+-rw-rw-rw-   0        0        0     8550 2024-05-07 13:17:14.400754 desalsim-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8225 2024-05-07 12:19:38.000000 desalsim-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 13:17:14.375290 desalsim-0.3/example/
+-rw-rw-rw-   0        0        0      797 2024-05-07 13:01:36.000000 desalsim-0.3/example/__init__.py
+-rw-rw-rw-   0        0        0     4531 2024-04-11 13:19:36.000000 desalsim-0.3/example/comparison.py
+-rw-rw-rw-   0        0        0     1888 2024-05-06 15:42:19.000000 desalsim-0.3/example/constants.py
+-rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.3/example/density_calc.py
+-rw-rw-rw-   0        0        0    11978 2024-05-06 16:09:51.000000 desalsim-0.3/example/economic_f.py
+-rw-rw-rw-   0        0        0     8663 2024-04-29 21:33:04.000000 desalsim-0.3/example/ed_unit_f.py
+-rw-rw-rw-   0        0        0    17118 2024-04-29 21:35:34.000000 desalsim-0.3/example/edbm_unit_f.py
+-rw-rw-rw-   0        0        0    49286 2024-02-14 10:34:47.000000 desalsim-0.3/example/efc_unit_f.py
+-rw-rw-rw-   0        0        0    33181 2024-05-06 17:04:03.000000 desalsim-0.3/example/example_1.py
+-rw-rw-rw-   0        0        0    21599 2024-05-06 16:29:23.000000 desalsim-0.3/example/example_2.py
+-rw-rw-rw-   0        0        0     8532 2024-04-29 21:36:53.000000 desalsim-0.3/example/med_unit_f.py
+-rw-rw-rw-   0        0        0    14921 2024-05-03 08:06:32.000000 desalsim-0.3/example/mfpfr_unit_f.py
+-rw-rw-rw-   0        0        0     9421 2024-05-06 08:39:39.000000 desalsim-0.3/example/nanofiltration_unit_f.py
+-rw-rw-rw-   0        0        0     4366 2024-04-29 21:19:41.000000 desalsim-0.3/example/ro_unit_f.py
+-rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.3/example/scaleup.py
+-rw-rw-rw-   0        0        0    12262 2024-04-29 21:44:17.000000 desalsim-0.3/example/thermal_cryst_f.py
+-rw-rw-rw-   0        0        0       42 2024-05-07 13:17:14.402748 desalsim-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      609 2024-05-07 13:00:15.000000 desalsim-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:17:14.397761 desalsim-0.3/tests/
+-rw-rw-rw-   0        0        0      799 2024-05-07 12:54:02.000000 desalsim-0.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-0.3/tests/constants.py
+-rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.3/tests/density_calc.py
+-rw-rw-rw-   0        0        0     9094 2024-05-06 16:12:45.000000 desalsim-0.3/tests/economic_f.py
+-rw-rw-rw-   0        0        0     2527 2024-05-06 16:15:02.000000 desalsim-0.3/tests/economic_unittest.py
+-rw-rw-rw-   0        0        0     3255 2024-05-03 14:14:54.000000 desalsim-0.3/tests/ed_unit_f.py
+-rw-rw-rw-   0        0        0     3316 2024-05-03 14:16:37.000000 desalsim-0.3/tests/ed_unittest.py
+-rw-rw-rw-   0        0        0    12680 2024-05-03 13:51:25.000000 desalsim-0.3/tests/edbm_unit_f.py
+-rw-rw-rw-   0        0        0     8386 2024-05-03 13:50:48.000000 desalsim-0.3/tests/edbm_unittest.py
+-rw-rw-rw-   0        0        0     4496 2024-05-02 14:39:30.000000 desalsim-0.3/tests/med_unit_f.py
+-rw-rw-rw-   0        0        0     1555 2024-05-03 14:28:38.000000 desalsim-0.3/tests/med_unittest.py
+-rw-rw-rw-   0        0        0    10407 2024-05-03 12:57:15.000000 desalsim-0.3/tests/mfpfr_unit_f.py
+-rw-rw-rw-   0        0        0     2743 2024-05-03 12:56:18.000000 desalsim-0.3/tests/mfpfr_unittest.py
+-rw-rw-rw-   0        0        0     6961 2024-05-06 08:40:27.000000 desalsim-0.3/tests/nanofiltration_unit_f.py
+-rw-rw-rw-   0        0        0     1777 2024-05-06 08:40:55.000000 desalsim-0.3/tests/nanofiltration_unittest.py
+-rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.3/tests/scaleup.py
+-rw-rw-rw-   0        0        0     8687 2024-05-05 10:31:06.000000 desalsim-0.3/tests/thermal_cryst_f.py
+-rw-rw-rw-   0        0        0     4560 2024-05-05 10:30:42.000000 desalsim-0.3/tests/thermal_cryst_unittest.py
```

### Comparing `DesalSim-0.2/DesalSim.egg-info/PKG-INFO` & `desalsim-0.3/DesalSim.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: DesalSim
-Version: 0.2
+Version: 0.3
 Home-page: https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
 Author: rodoulak
 Author-email: r.ktori@tudelft.nl
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.0
+Requires-Dist: pandas>=1.0
 
-# Desalination and Brine Treatment simulation model
+# DesalSim: Desalination and Brine Treatment simulation model
 
  
 ## Overview 
 This project comprises a package of simulation models for desalination and brine treatment technologies, including reverse osmosis, nanofiltration, multi-effect distillation, chemical precipitation, eutectic freeze crystallization, electrodialysis, and thermal crystallization. These technologies are utilized for desalination, ion separation, and salt recovery processes in various industrial and environmental applications.
 
 The simulation models implemented here calculate various parameters such as salt concentration profiles, ion fluxes, energy consumption, chemical consumption, and operational costs. They provide insights into the performance and economics of the technologies under different operating conditions and input parameters. Additionally, the models allow for the integration of different technologies in various configurations to optimize process efficiency and resource utilization.
 
+![system description](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/assets/150446818/bb10e07d-b878-45c8-878a-0c56222546cf)
+
 ## Table of contents
 * [Purpose](#purpose)
 * [Key features](#key-features)
 * [Installation](#installation)
 * [Usage](#usage)
 * [Contributing](#contributing)
 * [Authors and Acknowledgements](#authors-and-acknowledgements)
@@ -57,15 +61,15 @@
 - `density_calc.py`: This file contains the main script for calculating density of a solution based on the tempretaure and the concentration of the solution.
 - `scaleup.py`: This file contains the main script for scaling-up a technology with known capacity using the six-tenths factor rule (m=0.6).
 - `LICENSE`: License file containing the MIT License terms.
 
 ## Installation  
 The easiest way is through pip, in command-line interface:   
 ```
-pip install desalination-and-brine-treatment==0.2
+pip install DesalSim==0.2
 ```
 
 If you want to install the latest GitHub verstion:
 1. Clone the repository to your local machine:
 ```
 git clone https://github.com/your-username/desalination-brine-treatment-simulation.git
 ```
@@ -91,14 +95,15 @@
 You can find Tutorials and documents at: 
 1. [Tutorial File](example/Tutorial.md)
 2. [Tutorial for Example 1](example/Example_1_Tutorial.md)
 3. [Economic Tutorial](example/Economic_Tutorial.md)
 4. The mathematical description of each technology is given in [Mathematical description](paper/Mathematical_description.pdf)
 5. [Example 1](example/example_1.py)
 6. [Example 2](example/example_2.py)
+7. [Scenarios comparison](example/comparison.py)
 
 
 ## Contributing
 Contributions to the project are welcome! If you'd like to contribute, please follow the standard GitHub workflow:
 1. Fork the repository.
 2. Create a new branch (git checkout -b feature/improvement).
 3. Make your changes and commit them (git commit -am 'Add new feature').
```

### Comparing `DesalSim-0.2/LICENSE` & `desalsim-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/PKG-INFO` & `desalsim-0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: DesalSim
-Version: 0.2
+Version: 0.3
 Home-page: https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
 Author: rodoulak
 Author-email: r.ktori@tudelft.nl
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.0
+Requires-Dist: pandas>=1.0
 
-# Desalination and Brine Treatment simulation model
+# DesalSim: Desalination and Brine Treatment simulation model
 
  
 ## Overview 
 This project comprises a package of simulation models for desalination and brine treatment technologies, including reverse osmosis, nanofiltration, multi-effect distillation, chemical precipitation, eutectic freeze crystallization, electrodialysis, and thermal crystallization. These technologies are utilized for desalination, ion separation, and salt recovery processes in various industrial and environmental applications.
 
 The simulation models implemented here calculate various parameters such as salt concentration profiles, ion fluxes, energy consumption, chemical consumption, and operational costs. They provide insights into the performance and economics of the technologies under different operating conditions and input parameters. Additionally, the models allow for the integration of different technologies in various configurations to optimize process efficiency and resource utilization.
 
+![system description](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/assets/150446818/bb10e07d-b878-45c8-878a-0c56222546cf)
+
 ## Table of contents
 * [Purpose](#purpose)
 * [Key features](#key-features)
 * [Installation](#installation)
 * [Usage](#usage)
 * [Contributing](#contributing)
 * [Authors and Acknowledgements](#authors-and-acknowledgements)
@@ -57,15 +61,15 @@
 - `density_calc.py`: This file contains the main script for calculating density of a solution based on the tempretaure and the concentration of the solution.
 - `scaleup.py`: This file contains the main script for scaling-up a technology with known capacity using the six-tenths factor rule (m=0.6).
 - `LICENSE`: License file containing the MIT License terms.
 
 ## Installation  
 The easiest way is through pip, in command-line interface:   
 ```
-pip install desalination-and-brine-treatment==0.2
+pip install DesalSim==0.2
 ```
 
 If you want to install the latest GitHub verstion:
 1. Clone the repository to your local machine:
 ```
 git clone https://github.com/your-username/desalination-brine-treatment-simulation.git
 ```
@@ -91,14 +95,15 @@
 You can find Tutorials and documents at: 
 1. [Tutorial File](example/Tutorial.md)
 2. [Tutorial for Example 1](example/Example_1_Tutorial.md)
 3. [Economic Tutorial](example/Economic_Tutorial.md)
 4. The mathematical description of each technology is given in [Mathematical description](paper/Mathematical_description.pdf)
 5. [Example 1](example/example_1.py)
 6. [Example 2](example/example_2.py)
+7. [Scenarios comparison](example/comparison.py)
 
 
 ## Contributing
 Contributions to the project are welcome! If you'd like to contribute, please follow the standard GitHub workflow:
 1. Fork the repository.
 2. Create a new branch (git checkout -b feature/improvement).
 3. Make your changes and commit them (git commit -am 'Add new feature').
```

### Comparing `DesalSim-0.2/README.md` & `desalsim-0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-# Desalination and Brine Treatment simulation model
+# DesalSim: Desalination and Brine Treatment simulation model
 
  
 ## Overview 
 This project comprises a package of simulation models for desalination and brine treatment technologies, including reverse osmosis, nanofiltration, multi-effect distillation, chemical precipitation, eutectic freeze crystallization, electrodialysis, and thermal crystallization. These technologies are utilized for desalination, ion separation, and salt recovery processes in various industrial and environmental applications.
 
 The simulation models implemented here calculate various parameters such as salt concentration profiles, ion fluxes, energy consumption, chemical consumption, and operational costs. They provide insights into the performance and economics of the technologies under different operating conditions and input parameters. Additionally, the models allow for the integration of different technologies in various configurations to optimize process efficiency and resource utilization.
 
+![system description](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/assets/150446818/bb10e07d-b878-45c8-878a-0c56222546cf)
+
 ## Table of contents
 * [Purpose](#purpose)
 * [Key features](#key-features)
 * [Installation](#installation)
 * [Usage](#usage)
 * [Contributing](#contributing)
 * [Authors and Acknowledgements](#authors-and-acknowledgements)
@@ -47,15 +49,15 @@
 - `density_calc.py`: This file contains the main script for calculating density of a solution based on the tempretaure and the concentration of the solution.
 - `scaleup.py`: This file contains the main script for scaling-up a technology with known capacity using the six-tenths factor rule (m=0.6).
 - `LICENSE`: License file containing the MIT License terms.
 
 ## Installation  
 The easiest way is through pip, in command-line interface:   
 ```
-pip install desalination-and-brine-treatment==0.2
+pip install DesalSim==0.2
 ```
 
 If you want to install the latest GitHub verstion:
 1. Clone the repository to your local machine:
 ```
 git clone https://github.com/your-username/desalination-brine-treatment-simulation.git
 ```
@@ -81,14 +83,15 @@
 You can find Tutorials and documents at: 
 1. [Tutorial File](example/Tutorial.md)
 2. [Tutorial for Example 1](example/Example_1_Tutorial.md)
 3. [Economic Tutorial](example/Economic_Tutorial.md)
 4. The mathematical description of each technology is given in [Mathematical description](paper/Mathematical_description.pdf)
 5. [Example 1](example/example_1.py)
 6. [Example 2](example/example_2.py)
+7. [Scenarios comparison](example/comparison.py)
 
 
 ## Contributing
 Contributions to the project are welcome! If you'd like to contribute, please follow the standard GitHub workflow:
 1. Fork the repository.
 2. Create a new branch (git checkout -b feature/improvement).
 3. Make your changes and commit them (git commit -am 'Add new feature').
```

### Comparing `DesalSim-0.2/desalination_and_brine_treatment/constants.py` & `desalsim-0.3/Desalsim/constants.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/desalination_and_brine_treatment/economic_f.py` & `desalsim-0.3/Desalsim/economic_f.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/desalination_and_brine_treatment/ed_unit_f.py` & `desalsim-0.3/Desalsim/ed_unit_f.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/desalination_and_brine_treatment/edbm_unit_f.py` & `desalsim-0.3/Desalsim/edbm_unit_f.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/desalination_and_brine_treatment/efc_unit_f.py` & `desalsim-0.3/Desalsim/efc_unit_f.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/desalination_and_brine_treatment/med_unit_f.py` & `desalsim-0.3/Desalsim/med_unit_f.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/desalination_and_brine_treatment/mfpfr_unit_f.py` & `desalsim-0.3/Desalsim/mfpfr_unit_f.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/desalination_and_brine_treatment/nanofiltration_unit_f.py` & `desalsim-0.3/Desalsim/nanofiltration_unit_f.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/desalination_and_brine_treatment/ro_unit_f.py` & `desalsim-0.3/Desalsim/ro_unit_f.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/desalination_and_brine_treatment/thermal_cryst_f.py` & `desalsim-0.3/Desalsim/thermal_cryst_f.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/example/comparison.py` & `desalsim-0.3/example/comparison.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/example/constants.py` & `desalsim-0.3/example/constants.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/example/economic_f.py` & `desalsim-0.3/example/economic_f.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/example/ed_unit_f.py` & `desalsim-0.3/example/ed_unit_f.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/example/edbm_unit_f.py` & `desalsim-0.3/example/edbm_unit_f.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/example/efc_unit_f.py` & `desalsim-0.3/example/efc_unit_f.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/example/example_1.py` & `desalsim-0.3/example/example_1.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/example/example_2.py` & `desalsim-0.3/example/example_2.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/example/med_unit_f.py` & `desalsim-0.3/example/med_unit_f.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/example/mfpfr_unit_f.py` & `desalsim-0.3/example/mfpfr_unit_f.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/example/nanofiltration_unit_f.py` & `desalsim-0.3/example/nanofiltration_unit_f.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/example/ro_unit_f.py` & `desalsim-0.3/example/ro_unit_f.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/example/thermal_cryst_f.py` & `desalsim-0.3/example/thermal_cryst_f.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/setup.py` & `desalsim-0.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f: 
     description =f.read()
 
 setup(
       name='DesalSim',
-      version='0.2',
+      version='0.3',
       packages=find_packages(),
       url="https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-",
       author="rodoulak",
       author_email="r.ktori@tudelft.nl",
       license="MIT",
       install_requires=[
           "numpy>=1.0",
```

### Comparing `DesalSim-0.2/tests/constants.py` & `desalsim-0.3/tests/constants.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/tests/economic_f.py` & `desalsim-0.3/tests/economic_f.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/tests/economic_unittest.py` & `desalsim-0.3/tests/economic_unittest.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/tests/ed_unit_f.py` & `desalsim-0.3/tests/ed_unit_f.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/tests/ed_unittest.py` & `desalsim-0.3/tests/ed_unittest.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/tests/edbm_unit_f.py` & `desalsim-0.3/tests/edbm_unit_f.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/tests/edbm_unittest.py` & `desalsim-0.3/tests/edbm_unittest.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/tests/med_unit_f.py` & `desalsim-0.3/tests/med_unit_f.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/tests/med_unittest.py` & `desalsim-0.3/tests/med_unittest.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/tests/mfpfr_unit_f.py` & `desalsim-0.3/tests/mfpfr_unit_f.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/tests/mfpfr_unittest.py` & `desalsim-0.3/tests/mfpfr_unittest.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/tests/nanofiltration_unit_f.py` & `desalsim-0.3/tests/nanofiltration_unit_f.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/tests/nanofiltration_unittest.py` & `desalsim-0.3/tests/nanofiltration_unittest.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/tests/thermal_cryst_f.py` & `desalsim-0.3/tests/thermal_cryst_f.py`

 * *Files identical despite different names*

### Comparing `DesalSim-0.2/tests/thermal_cryst_unittest.py` & `desalsim-0.3/tests/thermal_cryst_unittest.py`

 * *Files identical despite different names*

