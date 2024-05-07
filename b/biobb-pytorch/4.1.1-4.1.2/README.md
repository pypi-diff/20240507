# Comparing `tmp/biobb_pytorch-4.1.1.tar.gz` & `tmp/biobb_pytorch-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobb_pytorch-4.1.1.tar", last modified: Mon May  6 22:21:54 2024, max compression
+gzip compressed data, was "biobb_pytorch-4.1.2.tar", last modified: Tue May  7 11:38:35 2024, max compression
```

## Comparing `biobb_pytorch-4.1.1.tar` & `biobb_pytorch-4.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-06 22:21:54.465362 biobb_pytorch-4.1.1/
--rwxr-xr-x   0 pau        (501) staff       (20)    11358 2024-01-25 14:13:16.000000 biobb_pytorch-4.1.1/LICENSE
--rw-r--r--   0 pau        (501) staff       (20)     6841 2024-05-06 22:21:54.464961 biobb_pytorch-4.1.1/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)     5927 2024-05-06 22:19:00.000000 biobb_pytorch-4.1.1/README.md
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-06 22:21:54.456355 biobb_pytorch-4.1.1/biobb_pytorch/
--rw-r--r--   0 pau        (501) staff       (20)       84 2024-05-06 22:17:31.000000 biobb_pytorch-4.1.1/biobb_pytorch/__init__.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-06 22:21:54.463657 biobb_pytorch-4.1.1/biobb_pytorch/mdae/
--rw-r--r--   0 pau        (501) staff       (20)      104 2024-04-25 12:20:08.000000 biobb_pytorch-4.1.1/biobb_pytorch/mdae/__init__.py
--rw-r--r--   0 pau        (501) staff       (20)    12008 2024-05-06 20:44:25.000000 biobb_pytorch-4.1.1/biobb_pytorch/mdae/apply_mdae.py
--rw-r--r--   0 pau        (501) staff       (20)     4284 2024-05-06 14:01:34.000000 biobb_pytorch-4.1.1/biobb_pytorch/mdae/common.py
--rw-r--r--   0 pau        (501) staff       (20)     2195 2024-04-17 09:27:04.000000 biobb_pytorch-4.1.1/biobb_pytorch/mdae/mdae.py
--rw-r--r--   0 pau        (501) staff       (20)     4608 2024-05-06 14:10:58.000000 biobb_pytorch-4.1.1/biobb_pytorch/mdae/plots.py
--rw-r--r--   0 pau        (501) staff       (20)    22194 2024-05-06 20:30:11.000000 biobb_pytorch-4.1.1/biobb_pytorch/mdae/train_mdae.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-06 22:21:54.464590 biobb_pytorch-4.1.1/biobb_pytorch/test/
--rwxr-xr-x   0 pau        (501) staff       (20)        0 2024-01-26 06:36:24.000000 biobb_pytorch-4.1.1/biobb_pytorch/test/__init__.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-06 22:21:54.459899 biobb_pytorch-4.1.1/biobb_pytorch.egg-info/
--rw-r--r--   0 pau        (501) staff       (20)     6841 2024-05-06 22:21:54.000000 biobb_pytorch-4.1.1/biobb_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)      488 2024-05-06 22:21:54.000000 biobb_pytorch-4.1.1/biobb_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 pau        (501) staff       (20)        1 2024-05-06 22:21:54.000000 biobb_pytorch-4.1.1/biobb_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 pau        (501) staff       (20)      114 2024-05-06 22:21:54.000000 biobb_pytorch-4.1.1/biobb_pytorch.egg-info/entry_points.txt
--rw-r--r--   0 pau        (501) staff       (20)       26 2024-05-06 22:21:54.000000 biobb_pytorch-4.1.1/biobb_pytorch.egg-info/requires.txt
--rw-r--r--   0 pau        (501) staff       (20)       14 2024-05-06 22:21:54.000000 biobb_pytorch-4.1.1/biobb_pytorch.egg-info/top_level.txt
--rw-r--r--   0 pau        (501) staff       (20)       38 2024-05-06 22:21:54.465456 biobb_pytorch-4.1.1/setup.cfg
--rw-r--r--   0 pau        (501) staff       (20)     1424 2024-05-06 22:17:01.000000 biobb_pytorch-4.1.1/setup.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-07 11:38:35.204196 biobb_pytorch-4.1.2/
+-rwxr-xr-x   0 pau        (501) staff       (20)    11358 2024-01-25 14:13:16.000000 biobb_pytorch-4.1.2/LICENSE
+-rw-r--r--   0 pau        (501) staff       (20)     6841 2024-05-07 11:38:35.203852 biobb_pytorch-4.1.2/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)     5927 2024-05-07 11:37:41.000000 biobb_pytorch-4.1.2/README.md
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-07 11:38:35.196556 biobb_pytorch-4.1.2/biobb_pytorch/
+-rw-r--r--   0 pau        (501) staff       (20)       84 2024-05-07 11:36:32.000000 biobb_pytorch-4.1.2/biobb_pytorch/__init__.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-07 11:38:35.202897 biobb_pytorch-4.1.2/biobb_pytorch/mdae/
+-rw-r--r--   0 pau        (501) staff       (20)      104 2024-04-25 12:20:08.000000 biobb_pytorch-4.1.2/biobb_pytorch/mdae/__init__.py
+-rw-r--r--   0 pau        (501) staff       (20)    12008 2024-05-06 20:44:25.000000 biobb_pytorch-4.1.2/biobb_pytorch/mdae/apply_mdae.py
+-rw-r--r--   0 pau        (501) staff       (20)     4284 2024-05-06 14:01:34.000000 biobb_pytorch-4.1.2/biobb_pytorch/mdae/common.py
+-rw-r--r--   0 pau        (501) staff       (20)     2195 2024-04-17 09:27:04.000000 biobb_pytorch-4.1.2/biobb_pytorch/mdae/mdae.py
+-rw-r--r--   0 pau        (501) staff       (20)     4608 2024-05-06 14:10:58.000000 biobb_pytorch-4.1.2/biobb_pytorch/mdae/plots.py
+-rw-r--r--   0 pau        (501) staff       (20)    23388 2024-05-07 11:16:27.000000 biobb_pytorch-4.1.2/biobb_pytorch/mdae/train_mdae.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-07 11:38:35.203435 biobb_pytorch-4.1.2/biobb_pytorch/test/
+-rwxr-xr-x   0 pau        (501) staff       (20)        0 2024-01-26 06:36:24.000000 biobb_pytorch-4.1.2/biobb_pytorch/test/__init__.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-07 11:38:35.199138 biobb_pytorch-4.1.2/biobb_pytorch.egg-info/
+-rw-r--r--   0 pau        (501) staff       (20)     6841 2024-05-07 11:38:35.000000 biobb_pytorch-4.1.2/biobb_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)      488 2024-05-07 11:38:35.000000 biobb_pytorch-4.1.2/biobb_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2024-05-07 11:38:35.000000 biobb_pytorch-4.1.2/biobb_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 pau        (501) staff       (20)      114 2024-05-07 11:38:35.000000 biobb_pytorch-4.1.2/biobb_pytorch.egg-info/entry_points.txt
+-rw-r--r--   0 pau        (501) staff       (20)       26 2024-05-07 11:38:35.000000 biobb_pytorch-4.1.2/biobb_pytorch.egg-info/requires.txt
+-rw-r--r--   0 pau        (501) staff       (20)       14 2024-05-07 11:38:35.000000 biobb_pytorch-4.1.2/biobb_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 pau        (501) staff       (20)       38 2024-05-07 11:38:35.204294 biobb_pytorch-4.1.2/setup.cfg
+-rw-r--r--   0 pau        (501) staff       (20)     1424 2024-05-07 11:36:10.000000 biobb_pytorch-4.1.2/setup.py
```

### Comparing `biobb_pytorch-4.1.1/LICENSE` & `biobb_pytorch-4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_pytorch-4.1.1/PKG-INFO` & `biobb_pytorch-4.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobb_pytorch
-Version: 4.1.1
+Version: 4.1.2
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
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.1--pyhdfd78af_1)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.2--pyhdfd78af_1)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_pytorch)
 [![](https://img.shields.io/pypi/pyversions/biobb-pytorch.svg?label=Python%20Versions)](https://pypi.org/project/biobb-pytorch/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_pytorch)
 
 [![](https://readthedocs.org/projects/biobb-pytorch/badge/?version=latest&label=Docs)](https://biobb-pytorch.readthedocs.io/en/latest/?badge=latest)
@@ -59,61 +59,61 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-pytorch.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.1 2024.2
+v4.1.2 2024.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_pytorch>=4.1.1"
+        pip install "biobb_pytorch>=4.1.2"
 
 
 * Usage: [Python API documentation](https://biobb-pytorch.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_pytorch>=4.1.1"
+        conda install -c bioconda "biobb_pytorch>=4.1.2"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-pytorch.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-pytorch.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_pytorch:4.1.1--pyhdfd78af_1
+        docker pull quay.io/biocontainers/biobb_pytorch:4.1.2--pyhdfd78af_1
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_pytorch:4.1.1--pyhdfd78af_1 <command>
+        docker run quay.io/biocontainers/biobb_pytorch:4.1.2--pyhdfd78af_1 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_pytorch.sif https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.1--pyhdfd78af_1
+        singularity pull --name biobb_pytorch.sif https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.2--pyhdfd78af_1
 
 
 * Usage:
 
 
         singularity exec biobb_pytorch.sif <command>
```

### Comparing `biobb_pytorch-4.1.1/README.md` & `biobb_pytorch-4.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_pytorch?label=Version)](https://GitHub.com/bioexcel/biobb_pytorch/tags/)
 [![](https://img.shields.io/pypi/v/biobb-pytorch.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-pytorch/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_pytorch?label=Conda)](https://anaconda.org/bioconda/biobb_pytorch)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_pytorch?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_pytorch)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_pytorch?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.1--pyhdfd78af_1)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.2--pyhdfd78af_1)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_pytorch)
 [![](https://img.shields.io/pypi/pyversions/biobb-pytorch.svg?label=Python%20Versions)](https://pypi.org/project/biobb-pytorch/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_pytorch)
 
 [![](https://readthedocs.org/projects/biobb-pytorch/badge/?version=latest&label=Docs)](https://biobb-pytorch.readthedocs.io/en/latest/?badge=latest)
@@ -37,61 +37,61 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-pytorch.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.1 2024.2
+v4.1.2 2024.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_pytorch>=4.1.1"
+        pip install "biobb_pytorch>=4.1.2"
 
 
 * Usage: [Python API documentation](https://biobb-pytorch.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_pytorch>=4.1.1"
+        conda install -c bioconda "biobb_pytorch>=4.1.2"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-pytorch.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-pytorch.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_pytorch:4.1.1--pyhdfd78af_1
+        docker pull quay.io/biocontainers/biobb_pytorch:4.1.2--pyhdfd78af_1
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_pytorch:4.1.1--pyhdfd78af_1 <command>
+        docker run quay.io/biocontainers/biobb_pytorch:4.1.2--pyhdfd78af_1 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_pytorch.sif https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.1--pyhdfd78af_1
+        singularity pull --name biobb_pytorch.sif https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.2--pyhdfd78af_1
 
 
 * Usage:
 
 
         singularity exec biobb_pytorch.sif <command>
```

### Comparing `biobb_pytorch-4.1.1/biobb_pytorch/mdae/apply_mdae.py` & `biobb_pytorch-4.1.2/biobb_pytorch/mdae/apply_mdae.py`

 * *Files identical despite different names*

### Comparing `biobb_pytorch-4.1.1/biobb_pytorch/mdae/common.py` & `biobb_pytorch-4.1.2/biobb_pytorch/mdae/common.py`

 * *Files identical despite different names*

### Comparing `biobb_pytorch-4.1.1/biobb_pytorch/mdae/mdae.py` & `biobb_pytorch-4.1.2/biobb_pytorch/mdae/mdae.py`

 * *Files identical despite different names*

### Comparing `biobb_pytorch-4.1.1/biobb_pytorch/mdae/plots.py` & `biobb_pytorch-4.1.2/biobb_pytorch/mdae/plots.py`

 * *Files identical despite different names*

### Comparing `biobb_pytorch-4.1.1/biobb_pytorch/mdae/train_mdae.py` & `biobb_pytorch-4.1.2/biobb_pytorch/mdae/train_mdae.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,17 @@
         input_model_pth_path (str) (Optional): Path to the input model file. File type: input. `Sample file <https://github.com/bioexcel/biobb_pytorch/raw/master/biobb_pytorch/test/reference/mdae/ref_output_model.pth>`_. Accepted formats: pth (edam:format_2333).
         output_train_data_npz_path (str) (Optional): Path to the output train data file. File type: output. `Sample file <https://github.com/bioexcel/biobb_pytorch/raw/master/biobb_pytorch/test/reference/mdae/ref_output_train_data.npz>`_. Accepted formats: npz (edam:format_4003).
         output_performance_npz_path (str) (Optional): Path to the output performance file. File type: output.  `Sample file <https://github.com/bioexcel/biobb_pytorch/raw/master/biobb_pytorch/test/reference/mdae/ref_output_performance.npz>`_. Accepted formats: npz (edam:format_4003).
         properties (dict - Python dictionary object containing the tool parameters, not input/output files):
             * **latent_dimensions** (*int*) - (2) min dimensionality of the latent space.
             * **num_layers** (*int*) - (4) number of layers in the encoder/decoder (4 to encode and 4 to decode).
             * **num_epochs** (*int*) - (100) number of epochs (iterations of whole dataset) for training.
-            * **lr** (*float*) - (0.001) learning rate.
+            * **lr** (*float*) - (0.0001) learning rate.
+            * **self.lr_step_size** (*int*) - (100) Period of learning rate decay.
+            * **self.gamma** (*float*) - (0.1) Multiplicative factor of learning rate decay.
             * **checkpoint_interval** (*int*) - (25) number of epochs interval to save model checkpoints o 0 to disable.
             * **output_checkpoint_prefix** (*str*) - ("checkpoint_epoch") prefix for the checkpoint files.
             * **partition** (*float*) - (0.8) 0.8 = 80% partition of the data for training and validation.
             * **batch_size** (*int*) - (1) number of samples/frames per batch.
             * **log_interval** (*int*) - (10) number of epochs interval to log the training progress.
             * **input_dimensions** (*int*) - (None) input dimensions by default it should be the number of features in the input data (number of atoms * 3 corresponding to x, y, z coordinates).
             * **output_dimensions** (*int*) - (None) output dimensions by default it should be the number of features in the input data (number of atoms * 3 corresponding to x, y, z coordinates).
@@ -45,15 +47,15 @@
 
             from biobb_pytorch.mdae.train_mdae import trainMDAE
 
             prop = {
                 'latent_dimensions': 2,
                 'num_layers': 4,
                 'num_epochs': 100,
-                'lr': 0.001,
+                'lr': 0.0001,
                 'checkpoint_interval': 25,
                 'partition': 0.8,
                 'batch_size': 1,
                 'log_interval': 10,
                 'input_dimensions': 3,
                 'output_dimensions': 3,
                 'loss_function': 'MSELoss',
@@ -95,15 +97,17 @@
             'out': {'output_model_pth_path': output_model_pth_path, 'output_train_data_npz_path': output_train_data_npz_path, 'output_performance_npz_path': output_performance_npz_path}
         }
 
         # Properties specific for BB
         self.latent_dimensions: int = int(properties.get('latent_dimensions', 2))  # min dimensionality of the latent space
         self.num_layers: int = int(properties.get('num_layers', 4))  # number of layers in the encoder/decoder (4 to encode and 4 to decode)
         self.num_epochs: int = int(properties.get('num_epochs', 100))  # number of epochs (iterations of whole dataset) for training
-        self.lr: float = float(properties.get('lr', 0.001))  # learning rate
+        self.lr: float = float(properties.get('lr', 0.0001))  # learning rate
+        self.lr_step_size: int = int(properties.get('lr_step_size', 100))  # Period of learning rate decay
+        self.gamma: float = float(properties.get('gamma', 0.1))  # Multiplicative factor of learning rate decay
         self.checkpoint_interval: int = int(properties.get('checkpoint_interval', 25))  # number of epochs interval to save model checkpoints o 0 to disable
         self.output_checkpoint_prefix: str = properties.get('output_checkpoint_prefix', 'checkpoint_epoch_')  # prefix for the checkpoint files,
         self.partition: float = float(properties.get('partition', 0.8))  # 0.8 = 80% partition of the data for training and validation
         self.batch_size: int = int(properties.get('batch_size', 1))  # number of samples/frames per batch
         self.log_interval: int = int(properties.get('log_interval', 10))  # number of epochs interval to log the training progress
 
         # Input data section
@@ -176,15 +180,15 @@
         # Setup Biobb
         if self.check_restart():
             return 0
 
         self.stage_files()
 
         # Train the model
-        train_losses, validation_losses = self.train_model()
+        train_losses, validation_losses, best_model, best_model_epoch = self.train_model()
         if self.stage_io_dict['out'].get('output_train_data_npz_path'):
             np.savez(self.stage_io_dict['out']['output_train_data_npz_path'], train_losses=np.array(train_losses), validation_losses=np.array(validation_losses))
             fu.log(f'Saving train data to: {self.stage_io_dict["out"]["output_train_data_npz_path"]}', self.out_log)
             fu.log(f'  File size: {human_readable_file_size(self.stage_io_dict["out"]["output_train_data_npz_path"])}', self.out_log)
 
         # Evaluate the model
         if self.stage_io_dict['out'].get('output_performance_npz_path'):
@@ -192,77 +196,91 @@
             denormalized_reconstructed_data = ndarray_denormalization(reconstructed_data, self.input_train_data_max_values, self.input_train_data_min_values)
             reshaped_reconstructed_data = np.reshape(denormalized_reconstructed_data, (len(denormalized_reconstructed_data), -1, 3))
             np.savez(self.stage_io_dict['out']['output_performance_npz_path'], evaluate_losses=np.array(evaluate_losses), latent_space=np.array(latent_space), denormalized_reconstructed_data=np.array(reshaped_reconstructed_data))
             fu.log(f'Saving evaluation data to: {self.stage_io_dict["out"]["output_performance_npz_path"]}', self.out_log)
             fu.log(f'  File size: {human_readable_file_size(self.stage_io_dict["out"]["output_performance_npz_path"])}', self.out_log)
 
         # Save the model
-        torch.save(self.model.state_dict(), self.stage_io_dict['out']['output_model_pth_path'])
-        fu.log(f'Saving model to: {self.stage_io_dict["out"]["output_model_pth_path"]}', self.out_log)
+        torch.save(best_model, self.stage_io_dict['out']['output_model_pth_path'])
+        fu.log(f'Saving best model to: {self.stage_io_dict["out"]["output_model_pth_path"]}', self.out_log)
+        fu.log(f'  Best model epoch: {best_model_epoch}', self.out_log)
         fu.log(f'  File size: {human_readable_file_size(self.stage_io_dict["out"]["output_model_pth_path"])}', self.out_log)
 
         # Copy files to host
         self.copy_to_host()
 
         # Remove temporal files
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
         return 0
 
-    def train_model(self) -> Tuple[List[float], List[float]]:
+    def train_model(self) -> Tuple[List[float], List[float], Dict, int]:
         self.model.to(self.model.device)
         train_losses: List[float] = []
         validation_losses: List[float] = []
+        best_valid_loss: float = float('inf')  # Initialize best valid loss to infinity
 
         start_time: float = time.time()
         fu.log("Start Training:", self.out_log)
         fu.log(f"  Device: {self.model.device}", self.out_log)
         fu.log(f"  Train input file: {self.stage_io_dict['in']['input_train_npy_path']}", self.out_log)
         fu.log(f"    File size: {human_readable_file_size(self.stage_io_dict['in']['input_train_npy_path'])}", self.out_log)
         fu.log(f"  Number of atoms: {int(len(next(iter(self.train_dataloader))[0][0])/3)}", self.out_log)
         fu.log(f"  Number of frames for training: {len(self.train_dataloader)}    Total number of frames: {int((len(self.train_dataloader)*self.train_dataloader.batch_size)/self.partition) if self.partition is not None else 'Unknown'}", self.out_log)  # type: ignore
         fu.log(f"  Number of epochs: {self.num_epochs}", self.out_log)
         fu.log(f"  Partition: {self.partition}", self.out_log)
         fu.log(f"  Batch size: {self.batch_size}", self.out_log)
         fu.log(f"  Learning rate: {self.lr}", self.out_log)
+        fu.log(f"  Learning rate step size: {self.lr_step_size}", self.out_log)
+        fu.log(f"  Learning rate gamma: {self.gamma}", self.out_log)
         fu.log(f"  Number of layers: {self.num_layers}", self.out_log)
         fu.log(f"  Input dimensions: {self.input_dimensions}", self.out_log)
         fu.log(f"  Latent dimensions: {self.latent_dimensions}", self.out_log)
         fu.log(f"  Loss function: {str(self.loss_function).split('(')[0]}", self.out_log)
         fu.log(f"  Optimizer: {str(self.optimizer).split('(')[0]}", self.out_log)
         fu.log(f"  Checkpoint interval: {self.checkpoint_interval}", self.out_log)
         fu.log(f"  Log interval: {self.log_interval}\n", self.out_log)
 
+        scheduler = torch.optim.lr_scheduler.StepLR(self.optimizer, step_size=self.lr_step_size, gamma=self.gamma)
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
                 epoch_time: float = time.time() - loop_start_time
-                fu.log(f'{"Epoch":>4} {epoch_index+1}/{self.num_epochs} - Train Loss: {avg_train_loss:.3f}, Validation Loss: {avg_validation_loss:.3f}, Duration: {format_time(epoch_time)}, Estimated remaining time: {format_time((self.num_epochs-(epoch_index+1))*epoch_time)}', self.out_log)
+                fu.log(f'{"Epoch":>4} {epoch_index+1}/{self.num_epochs} - Train Loss: {avg_train_loss:.3f}, Validation Loss: {avg_validation_loss:.3f}, LR: {scheduler.get_lr()}, Duration: {format_time(epoch_time)}, ETA: {format_time((self.num_epochs-(epoch_index+1))*epoch_time)}', self.out_log)
                 loop_start_time = time.time()
 
             # Save checkpoint
             if self.checkpoint_interval and (epoch_index % self.checkpoint_interval == 0 or epoch_index == self.num_epochs-1):
                 checkpoint_path = str(Path(self.stage_io_dict.get("unique_dir", '')).joinpath(f'{self.output_checkpoint_prefix}_{epoch_index}.pth'))
                 fu.log(f'{"Saving: ":>4} {checkpoint_path}', self.out_log)
                 torch.save(self.model.state_dict(), checkpoint_path)
 
-        fu.log(f"End Training, total time: {format_time((time.time() - start_time)/60)} minutes", self.out_log)
+            # Update learning rate
+            scheduler.step()
 
-        return train_losses, validation_losses
+            # Save best model
+            if avg_validation_loss < best_valid_loss:
+                best_valid_loss = avg_validation_loss
+                best_model: Dict = self.model.state_dict()
+                best_model_epoch: int = epoch_index
+
+        fu.log(f"End Training, total time: {format_time((time.time() - start_time))}", self.out_log)
+
+        return train_losses, validation_losses, best_model, best_model_epoch
 
     def training_step(self, dataloader: torch.utils.data.DataLoader, optimizer: torch.optim.Optimizer, loss_function: torch.nn.modules.loss._Loss) -> float:
         self.model.train()
         losses: List[float] = []
         for data in dataloader:
             data = data[0].to(self.model.device)
             _, output = self.model(data)
```

### Comparing `biobb_pytorch-4.1.1/biobb_pytorch.egg-info/PKG-INFO` & `biobb_pytorch-4.1.2/biobb_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobb-pytorch
-Version: 4.1.1
+Version: 4.1.2
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
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.1--pyhdfd78af_1)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.2--pyhdfd78af_1)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_pytorch)
 [![](https://img.shields.io/pypi/pyversions/biobb-pytorch.svg?label=Python%20Versions)](https://pypi.org/project/biobb-pytorch/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_pytorch)
 
 [![](https://readthedocs.org/projects/biobb-pytorch/badge/?version=latest&label=Docs)](https://biobb-pytorch.readthedocs.io/en/latest/?badge=latest)
@@ -59,61 +59,61 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-pytorch.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.1 2024.2
+v4.1.2 2024.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_pytorch>=4.1.1"
+        pip install "biobb_pytorch>=4.1.2"
 
 
 * Usage: [Python API documentation](https://biobb-pytorch.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_pytorch>=4.1.1"
+        conda install -c bioconda "biobb_pytorch>=4.1.2"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-pytorch.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-pytorch.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_pytorch:4.1.1--pyhdfd78af_1
+        docker pull quay.io/biocontainers/biobb_pytorch:4.1.2--pyhdfd78af_1
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_pytorch:4.1.1--pyhdfd78af_1 <command>
+        docker run quay.io/biocontainers/biobb_pytorch:4.1.2--pyhdfd78af_1 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_pytorch.sif https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.1--pyhdfd78af_1
+        singularity pull --name biobb_pytorch.sif https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.2--pyhdfd78af_1
 
 
 * Usage:
 
 
         singularity exec biobb_pytorch.sif <command>
```

### Comparing `biobb_pytorch-4.1.1/setup.py` & `biobb_pytorch-4.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_pytorch",
-    version="4.1.1",
+    version="4.1.2",
     author="Biobb developers",
     author_email="pau.andrio@bsc.es",
     description="biobb_pytorch is the Biobb module collection to create and train ML & DL models.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_pytorch",
```

