# Comparing `tmp/biobb_pytorch-4.1.0.tar.gz` & `tmp/biobb_pytorch-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobb_pytorch-4.1.0.tar", last modified: Thu Apr 25 12:42:28 2024, max compression
+gzip compressed data, was "biobb_pytorch-4.1.1.tar", last modified: Mon May  6 22:21:54 2024, max compression
```

## Comparing `biobb_pytorch-4.1.0.tar` & `biobb_pytorch-4.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-04-25 12:42:28.996745 biobb_pytorch-4.1.0/
--rwxr-xr-x   0 pau        (501) staff       (20)    11358 2024-01-25 14:13:16.000000 biobb_pytorch-4.1.0/LICENSE
--rw-r--r--   0 pau        (501) staff       (20)     6301 2024-04-25 12:42:28.996406 biobb_pytorch-4.1.0/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)     5387 2024-01-26 06:58:13.000000 biobb_pytorch-4.1.0/README.md
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-04-25 12:42:28.987072 biobb_pytorch-4.1.0/biobb_pytorch/
--rw-r--r--   0 pau        (501) staff       (20)       84 2024-04-16 10:39:41.000000 biobb_pytorch-4.1.0/biobb_pytorch/__init__.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-04-25 12:42:28.995018 biobb_pytorch-4.1.0/biobb_pytorch/mdae/
--rw-r--r--   0 pau        (501) staff       (20)      104 2024-04-25 12:20:08.000000 biobb_pytorch-4.1.0/biobb_pytorch/mdae/__init__.py
--rw-r--r--   0 pau        (501) staff       (20)    10614 2024-04-17 09:29:56.000000 biobb_pytorch-4.1.0/biobb_pytorch/mdae/apply_mdae.py
--rw-r--r--   0 pau        (501) staff       (20)     3311 2024-04-04 21:15:15.000000 biobb_pytorch-4.1.0/biobb_pytorch/mdae/common.py
--rw-r--r--   0 pau        (501) staff       (20)     2195 2024-04-17 09:27:04.000000 biobb_pytorch-4.1.0/biobb_pytorch/mdae/mdae.py
--rw-r--r--   0 pau        (501) staff       (20)     4285 2024-04-16 11:49:27.000000 biobb_pytorch-4.1.0/biobb_pytorch/mdae/plots.py
--rw-r--r--   0 pau        (501) staff       (20)    19923 2024-04-17 09:31:08.000000 biobb_pytorch-4.1.0/biobb_pytorch/mdae/train_mdae.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-04-25 12:42:28.996053 biobb_pytorch-4.1.0/biobb_pytorch/test/
--rwxr-xr-x   0 pau        (501) staff       (20)        0 2024-01-26 06:36:24.000000 biobb_pytorch-4.1.0/biobb_pytorch/test/__init__.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-04-25 12:42:28.990137 biobb_pytorch-4.1.0/biobb_pytorch.egg-info/
--rw-r--r--   0 pau        (501) staff       (20)     6301 2024-04-25 12:42:28.000000 biobb_pytorch-4.1.0/biobb_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)      488 2024-04-25 12:42:28.000000 biobb_pytorch-4.1.0/biobb_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 pau        (501) staff       (20)        1 2024-04-25 12:42:28.000000 biobb_pytorch-4.1.0/biobb_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 pau        (501) staff       (20)      114 2024-04-25 12:42:28.000000 biobb_pytorch-4.1.0/biobb_pytorch.egg-info/entry_points.txt
--rw-r--r--   0 pau        (501) staff       (20)       26 2024-04-25 12:42:28.000000 biobb_pytorch-4.1.0/biobb_pytorch.egg-info/requires.txt
--rw-r--r--   0 pau        (501) staff       (20)       14 2024-04-25 12:42:28.000000 biobb_pytorch-4.1.0/biobb_pytorch.egg-info/top_level.txt
--rw-r--r--   0 pau        (501) staff       (20)       38 2024-04-25 12:42:28.996861 biobb_pytorch-4.1.0/setup.cfg
--rw-r--r--   0 pau        (501) staff       (20)     1424 2024-04-04 22:55:33.000000 biobb_pytorch-4.1.0/setup.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-06 22:21:54.465362 biobb_pytorch-4.1.1/
+-rwxr-xr-x   0 pau        (501) staff       (20)    11358 2024-01-25 14:13:16.000000 biobb_pytorch-4.1.1/LICENSE
+-rw-r--r--   0 pau        (501) staff       (20)     6841 2024-05-06 22:21:54.464961 biobb_pytorch-4.1.1/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)     5927 2024-05-06 22:19:00.000000 biobb_pytorch-4.1.1/README.md
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-06 22:21:54.456355 biobb_pytorch-4.1.1/biobb_pytorch/
+-rw-r--r--   0 pau        (501) staff       (20)       84 2024-05-06 22:17:31.000000 biobb_pytorch-4.1.1/biobb_pytorch/__init__.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-06 22:21:54.463657 biobb_pytorch-4.1.1/biobb_pytorch/mdae/
+-rw-r--r--   0 pau        (501) staff       (20)      104 2024-04-25 12:20:08.000000 biobb_pytorch-4.1.1/biobb_pytorch/mdae/__init__.py
+-rw-r--r--   0 pau        (501) staff       (20)    12008 2024-05-06 20:44:25.000000 biobb_pytorch-4.1.1/biobb_pytorch/mdae/apply_mdae.py
+-rw-r--r--   0 pau        (501) staff       (20)     4284 2024-05-06 14:01:34.000000 biobb_pytorch-4.1.1/biobb_pytorch/mdae/common.py
+-rw-r--r--   0 pau        (501) staff       (20)     2195 2024-04-17 09:27:04.000000 biobb_pytorch-4.1.1/biobb_pytorch/mdae/mdae.py
+-rw-r--r--   0 pau        (501) staff       (20)     4608 2024-05-06 14:10:58.000000 biobb_pytorch-4.1.1/biobb_pytorch/mdae/plots.py
+-rw-r--r--   0 pau        (501) staff       (20)    22194 2024-05-06 20:30:11.000000 biobb_pytorch-4.1.1/biobb_pytorch/mdae/train_mdae.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-06 22:21:54.464590 biobb_pytorch-4.1.1/biobb_pytorch/test/
+-rwxr-xr-x   0 pau        (501) staff       (20)        0 2024-01-26 06:36:24.000000 biobb_pytorch-4.1.1/biobb_pytorch/test/__init__.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-06 22:21:54.459899 biobb_pytorch-4.1.1/biobb_pytorch.egg-info/
+-rw-r--r--   0 pau        (501) staff       (20)     6841 2024-05-06 22:21:54.000000 biobb_pytorch-4.1.1/biobb_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)      488 2024-05-06 22:21:54.000000 biobb_pytorch-4.1.1/biobb_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2024-05-06 22:21:54.000000 biobb_pytorch-4.1.1/biobb_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 pau        (501) staff       (20)      114 2024-05-06 22:21:54.000000 biobb_pytorch-4.1.1/biobb_pytorch.egg-info/entry_points.txt
+-rw-r--r--   0 pau        (501) staff       (20)       26 2024-05-06 22:21:54.000000 biobb_pytorch-4.1.1/biobb_pytorch.egg-info/requires.txt
+-rw-r--r--   0 pau        (501) staff       (20)       14 2024-05-06 22:21:54.000000 biobb_pytorch-4.1.1/biobb_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 pau        (501) staff       (20)       38 2024-05-06 22:21:54.465456 biobb_pytorch-4.1.1/setup.cfg
+-rw-r--r--   0 pau        (501) staff       (20)     1424 2024-05-06 22:17:01.000000 biobb_pytorch-4.1.1/setup.py
```

### Comparing `biobb_pytorch-4.1.0/LICENSE` & `biobb_pytorch-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_pytorch-4.1.0/PKG-INFO` & `biobb_pytorch-4.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobb_pytorch
-Version: 4.1.0
+Version: 4.1.1
 Summary: biobb_pytorch is the Biobb module collection to create and train ML & DL models.
 Home-page: https://github.com/bioexcel/biobb_pytorch
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
 Project-URL: Documentation, http://biobb-pytorch.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
@@ -21,15 +21,15 @@
 License-File: LICENSE
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_pytorch?label=Version)](https://GitHub.com/bioexcel/biobb_pytorch/tags/)
 [![](https://img.shields.io/pypi/v/biobb-pytorch.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-pytorch/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_pytorch?label=Conda)](https://anaconda.org/bioconda/biobb_pytorch)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_pytorch?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_pytorch)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_pytorch?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.0--pyhdfd78af_1)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.1--pyhdfd78af_1)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_pytorch)
 [![](https://img.shields.io/pypi/pyversions/biobb-pytorch.svg?label=Python%20Versions)](https://pypi.org/project/biobb-pytorch/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_pytorch)
 
 [![](https://readthedocs.org/projects/biobb-pytorch/badge/?version=latest&label=Docs)](https://biobb-pytorch.readthedocs.io/en/latest/?badge=latest)
@@ -40,73 +40,80 @@
 
 [![](https://docs.bioexcel.eu/biobb_pytorch/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_pytorch/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_pytorch/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_pytorch/coverage/)
 [![](https://docs.bioexcel.eu/biobb_pytorch/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_pytorch/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_pytorch?label=Last%20Commit)](https://github.com/bioexcel/biobb_pytorch/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_pytorch.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_pytorch/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+ [//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractives URL)
+
 
 # biobb_pytorch
 
 ### Introduction
 biobb_pytorch is the Biobb module collection to create and train ML & DL models using the popular [PyTorch](https://pytorch.org/) Python library.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-pytorch.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2024.1
+v4.1.1 2024.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_pytorch>=4.1.0"
+        pip install "biobb_pytorch>=4.1.1"
 
 
 * Usage: [Python API documentation](https://biobb-pytorch.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_pytorch>=4.1.0"
+        conda install -c bioconda "biobb_pytorch>=4.1.1"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-pytorch.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-pytorch.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_pytorch:4.1.0--pyhdfd78af_1
+        docker pull quay.io/biocontainers/biobb_pytorch:4.1.1--pyhdfd78af_1
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_pytorch:4.1.0--pyhdfd78af_1 <command>
+        docker run quay.io/biocontainers/biobb_pytorch:4.1.1--pyhdfd78af_1 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_pytorch.sif https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.0--pyhdfd78af_1
+        singularity pull --name biobb_pytorch.sif https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.1--pyhdfd78af_1
 
 
 * Usage:
 
 
         singularity exec biobb_pytorch.sif <command>
```

### Comparing `biobb_pytorch-4.1.0/README.md` & `biobb_pytorch-4.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_pytorch?label=Version)](https://GitHub.com/bioexcel/biobb_pytorch/tags/)
 [![](https://img.shields.io/pypi/v/biobb-pytorch.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-pytorch/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_pytorch?label=Conda)](https://anaconda.org/bioconda/biobb_pytorch)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_pytorch?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_pytorch)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_pytorch?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.0--pyhdfd78af_1)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.1--pyhdfd78af_1)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_pytorch)
 [![](https://img.shields.io/pypi/pyversions/biobb-pytorch.svg?label=Python%20Versions)](https://pypi.org/project/biobb-pytorch/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_pytorch)
 
 [![](https://readthedocs.org/projects/biobb-pytorch/badge/?version=latest&label=Docs)](https://biobb-pytorch.readthedocs.io/en/latest/?badge=latest)
@@ -18,73 +18,80 @@
 
 [![](https://docs.bioexcel.eu/biobb_pytorch/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_pytorch/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_pytorch/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_pytorch/coverage/)
 [![](https://docs.bioexcel.eu/biobb_pytorch/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_pytorch/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_pytorch?label=Last%20Commit)](https://github.com/bioexcel/biobb_pytorch/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_pytorch.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_pytorch/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+ [//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractives URL)
+
 
 # biobb_pytorch
 
 ### Introduction
 biobb_pytorch is the Biobb module collection to create and train ML & DL models using the popular [PyTorch](https://pytorch.org/) Python library.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-pytorch.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2024.1
+v4.1.1 2024.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_pytorch>=4.1.0"
+        pip install "biobb_pytorch>=4.1.1"
 
 
 * Usage: [Python API documentation](https://biobb-pytorch.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_pytorch>=4.1.0"
+        conda install -c bioconda "biobb_pytorch>=4.1.1"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-pytorch.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-pytorch.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_pytorch:4.1.0--pyhdfd78af_1
+        docker pull quay.io/biocontainers/biobb_pytorch:4.1.1--pyhdfd78af_1
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_pytorch:4.1.0--pyhdfd78af_1 <command>
+        docker run quay.io/biocontainers/biobb_pytorch:4.1.1--pyhdfd78af_1 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_pytorch.sif https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.0--pyhdfd78af_1
+        singularity pull --name biobb_pytorch.sif https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.1--pyhdfd78af_1
 
 
 * Usage:
 
 
         singularity exec biobb_pytorch.sif <command>
```

### Comparing `biobb_pytorch-4.1.0/biobb_pytorch/mdae/apply_mdae.py` & `biobb_pytorch-4.1.1/biobb_pytorch/mdae/apply_mdae.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import torch
 import numpy as np
 import argparse
+import time
 from typing import Optional, Tuple, Dict
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
 from biobb_pytorch.mdae.mdae import MDAE
-from biobb_pytorch.mdae.common import ndarray_normalization, ndarray_denormalization, execute_model
+from biobb_pytorch.mdae.common import ndarray_normalization, ndarray_denormalization, execute_model, format_time, human_readable_file_size
 
 
 class ApplyMDAE(BiobbObject):
     """
     | biobb_pytorch ApplyMDAE
     | Apply a Molecular Dynamics AutoEncoder (MDAE) PyTorch model.
     | Apply a Molecular Dynamics AutoEncoder (MDAE) PyTorch model, the resulting denoised molecular dynamics or the reduced the dimensionality of molecular dynamics data can be used to analyze the dynamic properties of the system.
@@ -105,32 +106,50 @@
 
         self.stage_files()
 
         fu.log(f'Applying MDAE model reducing dimensionality from {self.input_dimensions} to {self.latent_dimensions} and reconstructing.', self.out_log)
         latent_space, reconstructed_data = self.apply_model(self.data_loader)
         denormalized_reconstructed_data = ndarray_denormalization(reconstructed_data, self.input_data_max_values, self.input_data_min_values)
         reshaped_reconstructed_data = np.reshape(denormalized_reconstructed_data, (len(denormalized_reconstructed_data), -1, 3))
-        fu.log(f'Saving reconstructed data to {self.stage_io_dict["out"]["output_reconstructed_data_npy_path"]}', self.out_log)
         np.save(self.stage_io_dict['out']['output_reconstructed_data_npy_path'], np.array(reshaped_reconstructed_data))
+        fu.log(f'Saving reconstructed data to: {self.stage_io_dict["out"]["output_reconstructed_data_npy_path"]}', self.out_log)
+        fu.log(f'  File size: {human_readable_file_size(self.stage_io_dict["out"]["output_reconstructed_data_npy_path"])}', self.out_log)
 
-        if self.io_dict['out'].get('output_latent_space_npy_path'):
-            fu.log(f'Saving latent space to {self.io_dict["out"]["output_latent_space_npy_path"]}', self.out_log)
-            np.save(self.io_dict['out']['output_latent_space_npy_path'], np.array(latent_space))
+        if self.stage_io_dict['out'].get('output_latent_space_npy_path'):
+            np.save(self.stage_io_dict['out']['output_latent_space_npy_path'], np.array(latent_space))
+            fu.log(f'Saving latent space to: {self.stage_io_dict["out"]["output_latent_space_npy_path"]}', self.out_log)
+            fu.log(f'  File size: {human_readable_file_size(self.stage_io_dict["out"]["output_latent_space_npy_path"])}', self.out_log)
 
         # Copy files to host
         self.copy_to_host()
 
         # Remove temporal files
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
         return 0
 
     def apply_model(self, dataloader: torch.utils.data.DataLoader) -> Tuple[np.ndarray, np.ndarray]:
-        return execute_model(self.model, dataloader, self.input_dimensions, self.latent_dimensions)[1:]
+        self.model.to(self.model.device)
+        start_time: float = time.time()
+        fu.log("Applying model:", self.out_log)
+        fu.log(f"  Device: {self.model.device}", self.out_log)
+        fu.log(f"  Input file: {self.stage_io_dict['in']['input_data_npy_path']}", self.out_log)
+        fu.log(f"    File size: {human_readable_file_size(self.stage_io_dict['in']['input_data_npy_path'])}", self.out_log)
+        fu.log(f"  Number of atoms: {int(len(next(iter(dataloader))[0][0])/3)}", self.out_log)
+        fu.log(f"  Number of frames: {int(len(dataloader)*dataloader.batch_size)}", self.out_log)  # type: ignore
+        fu.log(f"  Batch size: {self.batch_size}", self.out_log)
+        fu.log(f"  Number of layers: {self.num_layers}", self.out_log)
+        fu.log(f"  Input dimensions: {self.input_dimensions}", self.out_log)
+        fu.log(f"  Latent dimensions: {self.latent_dimensions}", self.out_log)
+
+        execution_tuple = execute_model(self.model, dataloader, self.input_dimensions, self.latent_dimensions)[1:]
+
+        fu.log(f"  Execution time: {format_time(time.time() - start_time)}", self.out_log)
+        return execution_tuple
 
 
 def applyMDAE(input_data_npy_path: str, input_model_pth_path: str,
               output_reconstructed_data_npy_path: str, output_latent_space_npy_path: Optional[str] = None,
               properties: Optional[Dict] = None, **kwargs) -> int:
     """Execute the :class:`ApplyMDAE <mdae.apply_mdae.ApplyMDAE>` class and
     execute the :meth:`launch() <mdae.apply_mdae.ApplyMDAE.launch>` method."""
```

### Comparing `biobb_pytorch-4.1.0/biobb_pytorch/mdae/common.py` & `biobb_pytorch-4.1.1/biobb_pytorch/mdae/common.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ Common functions for package biobb_pytorch.models """
 import numpy as np
 import torch
-from typing import Callable, List, Optional, Tuple
+from pathlib import Path
+from typing import Callable, List, Optional, Tuple, Union
 
 
 def ndarray_normalization(ndarray: np.ndarray, max_values: np.ndarray, min_values: np.ndarray) -> np.ndarray:
     """
     Normalize an ndarray along a specified axis.
 
     Args:
@@ -82,7 +83,31 @@
                 losses.append(loss.item())
             z_list.append(latent.cpu().numpy())
             x_hat_list.append(output.cpu().numpy())
     loss = float(np.mean(losses)) if losses else -1.0
     latent_space: np.ndarray = np.reshape(np.concatenate(z_list, axis=0), (-1, latent_dimensions))
     reconstructed_data: np.ndarray = np.reshape(np.concatenate(x_hat_list, axis=0), (-1, input_dimensions))
     return loss, latent_space, reconstructed_data
+
+
+def format_time(seconds: Union[float, int]) -> str:
+    """Converts time in seconds to a string of the format 'HH:MM:SS'."""
+    hours, remainder = divmod(seconds, 3600)
+    minutes, seconds = divmod(remainder, 60)
+    if hours:
+        return "{:02}h {:02}m {:02}s".format(int(hours), int(minutes), int(seconds))
+    elif minutes:
+        return "{:02}m {:02}s".format(int(minutes), int(seconds))
+    else:
+        return "{:02}s".format(int(seconds))
+
+
+def human_readable_file_size(file_path: Union[str, Path]) -> str:
+    """Get the size of a file and return it in a human-readable format."""
+    file_path = Path(file_path)  # Ensure file_path is a Path object
+    size_in_bytes: float = file_path.stat().st_size
+    units = ['Bytes', 'KB', 'MB', 'GB', 'PB']
+    for unit in units:
+        if size_in_bytes < 1024:
+            return f"{size_in_bytes:.2f} {unit}"
+        size_in_bytes /= 1024
+    return f"{size_in_bytes:.2f} {unit}"
```

### Comparing `biobb_pytorch-4.1.0/biobb_pytorch/mdae/mdae.py` & `biobb_pytorch-4.1.1/biobb_pytorch/mdae/mdae.py`

 * *Files identical despite different names*

### Comparing `biobb_pytorch-4.1.0/biobb_pytorch/mdae/plots.py` & `biobb_pytorch-4.1.1/biobb_pytorch/mdae/plots.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import matplotlib.pyplot as plt  # type: ignore
-import matplotlib.gridspec as gridspec
-
-
+import matplotlib.gridspec as gridspec  # type: ignore
+from matplotlib.markers import MarkerStyle  # type: ignore
 import numpy as np
 
 
 def plot_loss(output_train_data_npz_path: str) -> None:
     """
     Plot the training and validation losses from the given npz file.
 
@@ -15,16 +14,16 @@
     npz_file = np.load(output_train_data_npz_path)
     train_loss = npz_file['train_losses']
     val_loss = npz_file['validation_losses']
     min_train_loss_idx = np.argmin(train_loss)
     min_val_loss_idx = np.argmin(val_loss)
     plt.plot(range(len(train_loss)), train_loss, label=f"Training (min.: {min_train_loss_idx})", color='blue')
     plt.plot(range(len(val_loss)), val_loss, label=f"Validation (min.: {min_val_loss_idx})", color='orange')
-    plt.scatter(min_train_loss_idx, train_loss[min_train_loss_idx], color='blue', marker='v', s=50)
-    plt.scatter(min_val_loss_idx, val_loss[min_val_loss_idx], color='orange', marker='v', s=50)
+    plt.scatter(min_train_loss_idx, train_loss[min_train_loss_idx], color='blue', marker=MarkerStyle('v'), s=50)
+    plt.scatter(min_val_loss_idx, val_loss[min_val_loss_idx], color='orange', marker=MarkerStyle('v'), s=50)
     plt.legend()
     plt.ylabel('Total Loss')
     plt.xlabel('Epochs')
     plt.title('Training/Validation')
     plt.show()
 
 
@@ -72,30 +71,34 @@
 
 
 def _numpy_rmsf_by_atom(trajectory):
     return np.sqrt(np.mean(np.sum((trajectory - np.mean(trajectory, axis=0)) ** 2, axis=2), axis=0))
 
 
 def plot_rmsf(original_traj_npy_file, mutated_reconstructed_traj_npy_file):
-    rmsf_trajectory = _numpy_rmsf_by_atom(original_traj_npy_file)
-    rmsf_output = _numpy_rmsf_by_atom(mutated_reconstructed_traj_npy_file)
+    original_traj = np.load(original_traj_npy_file)
+    mutated_reconstructed_traj = np.load(mutated_reconstructed_traj_npy_file)
+    rmsf_trajectory = _numpy_rmsf_by_atom(original_traj)
+    rmsf_output = _numpy_rmsf_by_atom(mutated_reconstructed_traj)
     fig, ax = plt.subplots(figsize=(20, 6))
     indices = np.arange(len(rmsf_trajectory))
     ax.plot(indices, rmsf_trajectory, color='blue', linewidth=1, label='Original')
     ax.plot(indices, rmsf_output, color='red', linewidth=1, label='Reconstruction')
     ax.set_xlabel('# Atom')
     ax.set_ylabel('RMSD (Å) Average structure as reference')
     plt.title('RMSF Plot')
     plt.legend()
     plt.show()
 
 
 def plot_rmsf_difference(original_traj_npy_file, mutated_reconstructed_traj_npy_file):
-    rmsf_trajectory = _numpy_rmsf_by_atom(original_traj_npy_file)
-    rmsf_output = _numpy_rmsf_by_atom(mutated_reconstructed_traj_npy_file)
+    original_traj = np.load(original_traj_npy_file)
+    mutated_reconstructed_traj = np.load(mutated_reconstructed_traj_npy_file)
+    rmsf_trajectory = _numpy_rmsf_by_atom(original_traj)
+    rmsf_output = _numpy_rmsf_by_atom(mutated_reconstructed_traj)
     fig, ax = plt.subplots(figsize=(20, 6))
     indices = np.arange(len(rmsf_trajectory))
     # Plot RMSF for diference between input and output
     ax.plot(indices, (rmsf_trajectory - rmsf_output), color='orange', linewidth=1, label='DIO')
     ax.set_xlabel('# Atom')
     ax.set_ylabel('RMSD (Å)')
     plt.title('RMSF Plot')
```

### Comparing `biobb_pytorch-4.1.0/biobb_pytorch/mdae/train_mdae.py` & `biobb_pytorch-4.1.1/biobb_pytorch/mdae/train_mdae.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import argparse
 from typing import Optional, List, Tuple, Dict
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
 from biobb_pytorch.mdae.mdae import MDAE
-from biobb_pytorch.mdae.common import get_loss_function, get_optimizer_function, ndarray_normalization, ndarray_denormalization, execute_model
+from biobb_pytorch.mdae.common import get_loss_function, get_optimizer_function, ndarray_normalization, ndarray_denormalization, execute_model, format_time, human_readable_file_size
 from pathlib import Path
 
 
 class TrainMDAE(BiobbObject):
     """
     | biobb_pytorch TrainMDAE
     | Train a Molecular Dynamics AutoEncoder (MDAE) PyTorch model.
@@ -177,28 +177,32 @@
         if self.check_restart():
             return 0
 
         self.stage_files()
 
         # Train the model
         train_losses, validation_losses = self.train_model()
-        print(train_losses)
         if self.stage_io_dict['out'].get('output_train_data_npz_path'):
             np.savez(self.stage_io_dict['out']['output_train_data_npz_path'], train_losses=np.array(train_losses), validation_losses=np.array(validation_losses))
+            fu.log(f'Saving train data to: {self.stage_io_dict["out"]["output_train_data_npz_path"]}', self.out_log)
+            fu.log(f'  File size: {human_readable_file_size(self.stage_io_dict["out"]["output_train_data_npz_path"])}', self.out_log)
 
         # Evaluate the model
         if self.stage_io_dict['out'].get('output_performance_npz_path'):
             evaluate_losses, latent_space, reconstructed_data = self.evaluate_model(self.performance_dataloader, self.loss_function)
             denormalized_reconstructed_data = ndarray_denormalization(reconstructed_data, self.input_train_data_max_values, self.input_train_data_min_values)
             reshaped_reconstructed_data = np.reshape(denormalized_reconstructed_data, (len(denormalized_reconstructed_data), -1, 3))
             np.savez(self.stage_io_dict['out']['output_performance_npz_path'], evaluate_losses=np.array(evaluate_losses), latent_space=np.array(latent_space), denormalized_reconstructed_data=np.array(reshaped_reconstructed_data))
+            fu.log(f'Saving evaluation data to: {self.stage_io_dict["out"]["output_performance_npz_path"]}', self.out_log)
+            fu.log(f'  File size: {human_readable_file_size(self.stage_io_dict["out"]["output_performance_npz_path"])}', self.out_log)
 
         # Save the model
-        fu.log(f'Saving model to: {self.stage_io_dict["out"]["output_model_pth_path"]}', self.out_log)
         torch.save(self.model.state_dict(), self.stage_io_dict['out']['output_model_pth_path'])
+        fu.log(f'Saving model to: {self.stage_io_dict["out"]["output_model_pth_path"]}', self.out_log)
+        fu.log(f'  File size: {human_readable_file_size(self.stage_io_dict["out"]["output_model_pth_path"])}', self.out_log)
 
         # Copy files to host
         self.copy_to_host()
 
         # Remove temporal files
         self.remove_tmp_files()
 
@@ -207,39 +211,56 @@
 
     def train_model(self) -> Tuple[List[float], List[float]]:
         self.model.to(self.model.device)
         train_losses: List[float] = []
         validation_losses: List[float] = []
 
         start_time: float = time.time()
-
         fu.log("Start Training:", self.out_log)
+        fu.log(f"  Device: {self.model.device}", self.out_log)
+        fu.log(f"  Train input file: {self.stage_io_dict['in']['input_train_npy_path']}", self.out_log)
+        fu.log(f"    File size: {human_readable_file_size(self.stage_io_dict['in']['input_train_npy_path'])}", self.out_log)
+        fu.log(f"  Number of atoms: {int(len(next(iter(self.train_dataloader))[0][0])/3)}", self.out_log)
+        fu.log(f"  Number of frames for training: {len(self.train_dataloader)}    Total number of frames: {int((len(self.train_dataloader)*self.train_dataloader.batch_size)/self.partition) if self.partition is not None else 'Unknown'}", self.out_log)  # type: ignore
+        fu.log(f"  Number of epochs: {self.num_epochs}", self.out_log)
+        fu.log(f"  Partition: {self.partition}", self.out_log)
+        fu.log(f"  Batch size: {self.batch_size}", self.out_log)
+        fu.log(f"  Learning rate: {self.lr}", self.out_log)
+        fu.log(f"  Number of layers: {self.num_layers}", self.out_log)
+        fu.log(f"  Input dimensions: {self.input_dimensions}", self.out_log)
+        fu.log(f"  Latent dimensions: {self.latent_dimensions}", self.out_log)
+        fu.log(f"  Loss function: {str(self.loss_function).split('(')[0]}", self.out_log)
+        fu.log(f"  Optimizer: {str(self.optimizer).split('(')[0]}", self.out_log)
+        fu.log(f"  Checkpoint interval: {self.checkpoint_interval}", self.out_log)
+        fu.log(f"  Log interval: {self.log_interval}\n", self.out_log)
+
         for epoch_index in range(self.num_epochs):
             loop_start_time: float = time.time()
 
             # Training step
             avg_train_loss: float = self.training_step(self.train_dataloader, self.optimizer, self.loss_function)
             train_losses.append(avg_train_loss)
 
             # Validation step
             avg_validation_loss, _, _ = self.evaluate_model(self.validation_dataloader, self.loss_function)
             validation_losses.append(avg_validation_loss)
 
             # Logging
             if self.log_interval and (epoch_index % self.log_interval == 0 or epoch_index == self.num_epochs-1):
-                fu.log(f'{"Epoch":>4} {epoch_index+1}/{self.num_epochs} - Train Loss: {avg_train_loss:.3f}, Validation Loss: {avg_validation_loss:.3f}, Duration: {time.time() - loop_start_time:.2f}s', self.out_log)
+                epoch_time: float = time.time() - loop_start_time
+                fu.log(f'{"Epoch":>4} {epoch_index+1}/{self.num_epochs} - Train Loss: {avg_train_loss:.3f}, Validation Loss: {avg_validation_loss:.3f}, Duration: {format_time(epoch_time)}, Estimated remaining time: {format_time((self.num_epochs-(epoch_index+1))*epoch_time)}', self.out_log)
                 loop_start_time = time.time()
 
             # Save checkpoint
             if self.checkpoint_interval and (epoch_index % self.checkpoint_interval == 0 or epoch_index == self.num_epochs-1):
                 checkpoint_path = str(Path(self.stage_io_dict.get("unique_dir", '')).joinpath(f'{self.output_checkpoint_prefix}_{epoch_index}.pth'))
                 fu.log(f'{"Saving: ":>4} {checkpoint_path}', self.out_log)
                 torch.save(self.model.state_dict(), checkpoint_path)
 
-        fu.log(f"End Training, total time: {((time.time() - start_time)/60):.2f} minutes", self.out_log)
+        fu.log(f"End Training, total time: {format_time((time.time() - start_time)/60)} minutes", self.out_log)
 
         return train_losses, validation_losses
 
     def training_step(self, dataloader: torch.utils.data.DataLoader, optimizer: torch.optim.Optimizer, loss_function: torch.nn.modules.loss._Loss) -> float:
         self.model.train()
         losses: List[float] = []
         for data in dataloader:
```

### Comparing `biobb_pytorch-4.1.0/biobb_pytorch.egg-info/PKG-INFO` & `biobb_pytorch-4.1.1/biobb_pytorch.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobb-pytorch
-Version: 4.1.0
+Version: 4.1.1
 Summary: biobb_pytorch is the Biobb module collection to create and train ML & DL models.
 Home-page: https://github.com/bioexcel/biobb_pytorch
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
 Project-URL: Documentation, http://biobb-pytorch.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
@@ -21,15 +21,15 @@
 License-File: LICENSE
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_pytorch?label=Version)](https://GitHub.com/bioexcel/biobb_pytorch/tags/)
 [![](https://img.shields.io/pypi/v/biobb-pytorch.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-pytorch/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_pytorch?label=Conda)](https://anaconda.org/bioconda/biobb_pytorch)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_pytorch?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_pytorch)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_pytorch?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.0--pyhdfd78af_1)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.1--pyhdfd78af_1)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_pytorch)
 [![](https://img.shields.io/pypi/pyversions/biobb-pytorch.svg?label=Python%20Versions)](https://pypi.org/project/biobb-pytorch/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_pytorch)
 
 [![](https://readthedocs.org/projects/biobb-pytorch/badge/?version=latest&label=Docs)](https://biobb-pytorch.readthedocs.io/en/latest/?badge=latest)
@@ -40,73 +40,80 @@
 
 [![](https://docs.bioexcel.eu/biobb_pytorch/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_pytorch/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_pytorch/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_pytorch/coverage/)
 [![](https://docs.bioexcel.eu/biobb_pytorch/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_pytorch/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_pytorch?label=Last%20Commit)](https://github.com/bioexcel/biobb_pytorch/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_pytorch.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_pytorch/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+ [//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractives URL)
+
 
 # biobb_pytorch
 
 ### Introduction
 biobb_pytorch is the Biobb module collection to create and train ML & DL models using the popular [PyTorch](https://pytorch.org/) Python library.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-pytorch.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2024.1
+v4.1.1 2024.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_pytorch>=4.1.0"
+        pip install "biobb_pytorch>=4.1.1"
 
 
 * Usage: [Python API documentation](https://biobb-pytorch.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_pytorch>=4.1.0"
+        conda install -c bioconda "biobb_pytorch>=4.1.1"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-pytorch.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-pytorch.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_pytorch:4.1.0--pyhdfd78af_1
+        docker pull quay.io/biocontainers/biobb_pytorch:4.1.1--pyhdfd78af_1
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_pytorch:4.1.0--pyhdfd78af_1 <command>
+        docker run quay.io/biocontainers/biobb_pytorch:4.1.1--pyhdfd78af_1 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_pytorch.sif https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.0--pyhdfd78af_1
+        singularity pull --name biobb_pytorch.sif https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.1--pyhdfd78af_1
 
 
 * Usage:
 
 
         singularity exec biobb_pytorch.sif <command>
```

### Comparing `biobb_pytorch-4.1.0/setup.py` & `biobb_pytorch-4.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_pytorch",
-    version="4.1.0",
+    version="4.1.1",
     author="Biobb developers",
     author_email="pau.andrio@bsc.es",
     description="biobb_pytorch is the Biobb module collection to create and train ML & DL models.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_pytorch",
```

