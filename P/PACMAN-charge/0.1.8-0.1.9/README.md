# Comparing `tmp/PACMAN-charge-0.1.8.tar.gz` & `tmp/PACMAN-charge-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PACMAN-charge-0.1.8.tar", last modified: Mon May  6 03:23:30 2024, max compression
+gzip compressed data, was "PACMAN-charge-0.1.9.tar", last modified: Tue May  7 08:19:18 2024, max compression
```

## Comparing `PACMAN-charge-0.1.8.tar` & `PACMAN-charge-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-06 03:23:30.079009 PACMAN-charge-0.1.8/
--rwxrwxrwx   0 root         (0) root         (0)     1068 2024-03-25 02:54:44.000000 PACMAN-charge-0.1.8/LICENSE
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-06 03:23:29.958009 PACMAN-charge-0.1.8/PACMANCharge/
--rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-29 12:12:36.000000 PACMAN-charge-0.1.8/PACMANCharge/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    28392 2024-01-10 01:22:23.000000 PACMAN-charge-0.1.8/PACMANCharge/atom_init.json
--rwxrwxrwx   0 root         (0) root         (0)    25764 2024-05-06 03:22:55.000000 PACMAN-charge-0.1.8/PACMANCharge/pmcharge.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-06 03:23:30.022009 PACMAN-charge-0.1.8/PACMAN_charge.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     3244 2024-05-06 03:23:29.000000 PACMAN-charge-0.1.8/PACMAN_charge.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      334 2024-05-06 03:23:29.000000 PACMAN-charge-0.1.8/PACMAN_charge.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-06 03:23:29.000000 PACMAN-charge-0.1.8/PACMAN_charge.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      121 2024-05-06 03:23:29.000000 PACMAN-charge-0.1.8/PACMAN_charge.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2024-05-06 03:23:29.000000 PACMAN-charge-0.1.8/PACMAN_charge.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)     3244 2024-05-06 03:23:30.078009 PACMAN-charge-0.1.8/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2855 2024-05-06 03:23:01.000000 PACMAN-charge-0.1.8/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-06 03:23:30.080009 PACMAN-charge-0.1.8/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1038 2024-05-06 03:22:58.000000 PACMAN-charge-0.1.8/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-06 03:23:30.063009 PACMAN-charge-0.1.8/test/
--rwxrwxrwx   0 root         (0) root         (0)    34098 2024-05-04 13:50:41.000000 PACMAN-charge-0.1.8/test/Cu-BTC.cif
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-25 03:31:56.000000 PACMAN-charge-0.1.8/test/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      151 2024-05-04 13:49:04.000000 PACMAN-charge-0.1.8/test/test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-07 08:19:19.130684 PACMAN-charge-0.1.9/
+-rwxrwxrwx   0 root         (0) root         (0)     1068 2024-03-25 02:54:44.000000 PACMAN-charge-0.1.9/LICENSE
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-07 08:19:18.989631 PACMAN-charge-0.1.9/PACMANCharge/
+-rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-29 12:12:36.000000 PACMAN-charge-0.1.9/PACMANCharge/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    28392 2024-01-10 01:22:23.000000 PACMAN-charge-0.1.9/PACMANCharge/atom_init.json
+-rwxrwxrwx   0 root         (0) root         (0)    25766 2024-05-07 08:18:34.000000 PACMAN-charge-0.1.9/PACMANCharge/pmcharge.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-07 08:19:19.058670 PACMAN-charge-0.1.9/PACMAN_charge.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     3247 2024-05-07 08:19:18.000000 PACMAN-charge-0.1.9/PACMAN_charge.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      334 2024-05-07 08:19:18.000000 PACMAN-charge-0.1.9/PACMAN_charge.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-07 08:19:18.000000 PACMAN-charge-0.1.9/PACMAN_charge.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      121 2024-05-07 08:19:18.000000 PACMAN-charge-0.1.9/PACMAN_charge.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2024-05-07 08:19:18.000000 PACMAN-charge-0.1.9/PACMAN_charge.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     3247 2024-05-07 08:19:19.128684 PACMAN-charge-0.1.9/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2858 2024-05-07 08:18:14.000000 PACMAN-charge-0.1.9/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-07 08:19:19.131683 PACMAN-charge-0.1.9/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1038 2024-05-07 08:16:59.000000 PACMAN-charge-0.1.9/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-07 08:19:19.113677 PACMAN-charge-0.1.9/test/
+-rwxrwxrwx   0 root         (0) root         (0)    34098 2024-05-06 03:24:36.000000 PACMAN-charge-0.1.9/test/Cu-BTC.cif
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-25 03:31:56.000000 PACMAN-charge-0.1.9/test/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      134 2024-05-06 03:24:19.000000 PACMAN-charge-0.1.9/test/test.py
```

### Comparing `PACMAN-charge-0.1.8/LICENSE` & `PACMAN-charge-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PACMAN-charge-0.1.8/PACMANCharge/atom_init.json` & `PACMAN-charge-0.1.9/PACMANCharge/atom_init.json`

 * *Files identical despite different names*

### Comparing `PACMAN-charge-0.1.8/PACMANCharge/pmcharge.py` & `PACMAN-charge-0.1.9/PACMANCharge/pmcharge.py`

 * *Files 1% similar despite different names*

```diff
@@ -486,15 +486,15 @@
         N,_ = atom_fea.shape
         for conv_func in self.convs:
             nbr_fea,atom_fea,global_fea = conv_func(atom_fea,nbr_fea,nbr_fea_idx1,nbr_fea_idx2,num_nbrs,crystal_atom_idx)          
         global_fea = global_fea / atom_nums
         z = self.phi_u(global_fea)
         return z
 
-def predict(cif_file,charge_type="DDEC6",digits=6,atom_type=True,neutral=True):
+def predict(cif_file,charge_type="DDEC6",digits=6,atom_type=False,neutral=False):
    
     if charge_type == "DDEC6":
         charge_model_name = package_directory + 'ddec.pth'
         nor_name = package_directory + 'ddec.pkl'
     elif charge_type == "Bader":
         charge_model_name = package_directory + 'bader.pth'
         nor_name = package_directory + 'bader.pkl'
```

### Comparing `PACMAN-charge-0.1.8/PACMAN_charge.egg-info/PKG-INFO` & `PACMAN-charge-0.1.9/PACMAN_charge.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PACMAN-charge
-Version: 0.1.8
+Version: 0.1.9
 Summary: Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)
 Home-page: https://github.com/sxm13/PACMAN
 Author: Guobin Zhao
 Author-email: sxmzhaogb@gmai.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,22 +22,22 @@
 [![Requires Python 3.9](https://img.shields.io/badge/Python-3.9-blue.svg?logo=python&logoColor=white)](https://python.org/downloads) [![Zenodo](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.10822403-blue)](https://doi.org/10.5281/zenodo.10822403)  [![MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/sxm13/PACMAN/LICENSE.txt) [![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sxmzhaogb@gmail.com) [![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)]() [![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)]()          
 
 
 # Usage
 
 ```sh      
 from PACMANCharge import pmcharge
-PACMaN.predict(cif_file="./test/Cu-BTC.cif",charge_type="DDEC6",digits=10,atom_type=True,neutral=True)
+PACMaN.predict(cif_file="./test/Cu-BTC.cif",charge_type="DDEC6",digits=6,atom_type=False,neutral=False)
 ```
 
 * cif_file: cif file (without partial atomic charges) **[cif path]**                                                            
 * charge-type (default: DDE6): DDEC6, Bader or CM5                                        
 * digits (default: 6): number of decimal places to print for partial atomic charges. ML models were trained on a 6-digit dataset.                                                                     
-* atom-type (default: True): keep the same partial atomic charge for the same atom types (based on the similarity of partial atomic charges up to 2 decimal places).                                                         
-* neutral (default: True): keep the net charge is zero. We use "mean" method to neuralize the system where the excess charges are equally distributed across all atoms.                                                                            
+* atom-type (default: False): keep the same partial atomic charge for the same atom types (based on the similarity of partial atomic charges up to 2 decimal places).                                                         
+* neutral (default: False): keep the net charge is zero. We use "mean" method to neuralize the system where the excess charges are equally distributed across all atoms.                                                                            
 
 # Website & Zenodo
 PACMAN-APP[link](https://gcn-charge-predicter-mtap.streamlit.app/)       
 DOWNLOAD full code and dataset[link](https://zenodo.org/records/10822403) But we will not update new vesion in Zenodo.            
 
 # Reference
 If you use PACMAN Charge, please cite this paper:
```

### Comparing `PACMAN-charge-0.1.8/PKG-INFO` & `PACMAN-charge-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PACMAN-charge
-Version: 0.1.8
+Version: 0.1.9
 Summary: Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)
 Home-page: https://github.com/sxm13/PACMAN
 Author: Guobin Zhao
 Author-email: sxmzhaogb@gmai.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,22 +22,22 @@
 [![Requires Python 3.9](https://img.shields.io/badge/Python-3.9-blue.svg?logo=python&logoColor=white)](https://python.org/downloads) [![Zenodo](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.10822403-blue)](https://doi.org/10.5281/zenodo.10822403)  [![MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/sxm13/PACMAN/LICENSE.txt) [![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sxmzhaogb@gmail.com) [![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)]() [![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)]()          
 
 
 # Usage
 
 ```sh      
 from PACMANCharge import pmcharge
-PACMaN.predict(cif_file="./test/Cu-BTC.cif",charge_type="DDEC6",digits=10,atom_type=True,neutral=True)
+PACMaN.predict(cif_file="./test/Cu-BTC.cif",charge_type="DDEC6",digits=6,atom_type=False,neutral=False)
 ```
 
 * cif_file: cif file (without partial atomic charges) **[cif path]**                                                            
 * charge-type (default: DDE6): DDEC6, Bader or CM5                                        
 * digits (default: 6): number of decimal places to print for partial atomic charges. ML models were trained on a 6-digit dataset.                                                                     
-* atom-type (default: True): keep the same partial atomic charge for the same atom types (based on the similarity of partial atomic charges up to 2 decimal places).                                                         
-* neutral (default: True): keep the net charge is zero. We use "mean" method to neuralize the system where the excess charges are equally distributed across all atoms.                                                                            
+* atom-type (default: False): keep the same partial atomic charge for the same atom types (based on the similarity of partial atomic charges up to 2 decimal places).                                                         
+* neutral (default: False): keep the net charge is zero. We use "mean" method to neuralize the system where the excess charges are equally distributed across all atoms.                                                                            
 
 # Website & Zenodo
 PACMAN-APP[link](https://gcn-charge-predicter-mtap.streamlit.app/)       
 DOWNLOAD full code and dataset[link](https://zenodo.org/records/10822403) But we will not update new vesion in Zenodo.            
 
 # Reference
 If you use PACMAN Charge, please cite this paper:
```

### Comparing `PACMAN-charge-0.1.8/README.md` & `PACMAN-charge-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 [![Requires Python 3.9](https://img.shields.io/badge/Python-3.9-blue.svg?logo=python&logoColor=white)](https://python.org/downloads) [![Zenodo](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.10822403-blue)](https://doi.org/10.5281/zenodo.10822403)  [![MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/sxm13/PACMAN/LICENSE.txt) [![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sxmzhaogb@gmail.com) [![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)]() [![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)]()          
 
 
 # Usage
 
 ```sh      
 from PACMANCharge import pmcharge
-PACMaN.predict(cif_file="./test/Cu-BTC.cif",charge_type="DDEC6",digits=10,atom_type=True,neutral=True)
+PACMaN.predict(cif_file="./test/Cu-BTC.cif",charge_type="DDEC6",digits=6,atom_type=False,neutral=False)
 ```
 
 * cif_file: cif file (without partial atomic charges) **[cif path]**                                                            
 * charge-type (default: DDE6): DDEC6, Bader or CM5                                        
 * digits (default: 6): number of decimal places to print for partial atomic charges. ML models were trained on a 6-digit dataset.                                                                     
-* atom-type (default: True): keep the same partial atomic charge for the same atom types (based on the similarity of partial atomic charges up to 2 decimal places).                                                         
-* neutral (default: True): keep the net charge is zero. We use "mean" method to neuralize the system where the excess charges are equally distributed across all atoms.                                                                            
+* atom-type (default: False): keep the same partial atomic charge for the same atom types (based on the similarity of partial atomic charges up to 2 decimal places).                                                         
+* neutral (default: False): keep the net charge is zero. We use "mean" method to neuralize the system where the excess charges are equally distributed across all atoms.                                                                            
 
 # Website & Zenodo
 PACMAN-APP[link](https://gcn-charge-predicter-mtap.streamlit.app/)       
 DOWNLOAD full code and dataset[link](https://zenodo.org/records/10822403) But we will not update new vesion in Zenodo.            
 
 # Reference
 If you use PACMAN Charge, please cite this paper:
```

### Comparing `PACMAN-charge-0.1.8/setup.py` & `PACMAN-charge-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 from setuptools import setup, find_packages
 
 setup(
     name="PACMAN-charge",
-    version="0.1.8",
+    version="0.1.9",
     packages=find_packages(),
     description="Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)",
     author="Guobin Zhao",
     author_email="sxmzhaogb@gmai.com",
     url="https://github.com/sxm13/PACMAN",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `PACMAN-charge-0.1.8/test/Cu-BTC.cif` & `PACMAN-charge-0.1.9/test/Cu-BTC.cif`

 * *Files identical despite different names*

