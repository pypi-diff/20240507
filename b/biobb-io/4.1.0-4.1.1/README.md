# Comparing `tmp/biobb_io-4.1.0.tar.gz` & `tmp/biobb_io-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobb_io-4.1.0.tar", last modified: Wed Sep  6 14:09:21 2023, max compression
+gzip compressed data, was "biobb_io-4.1.1.tar", last modified: Tue May  7 14:30:48 2024, max compression
```

## Comparing `biobb_io-4.1.0.tar` & `biobb_io-4.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-06 14:09:21.402013 biobb_io-4.1.0/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11358 2022-05-26 11:34:05.000000 biobb_io-4.1.0/LICENSE
--rw-r--r--   0 gbayarri (1147421021) 1791188573     6186 2023-09-06 14:09:21.401803 biobb_io-4.1.0/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573     5306 2023-09-06 14:06:46.000000 biobb_io-4.1.0/README.md
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-06 14:09:21.398403 biobb_io-4.1.0/biobb_io/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573       58 2023-09-06 14:06:18.000000 biobb_io-4.1.0/biobb_io/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-06 14:09:21.401468 biobb_io-4.1.0/biobb_io/api/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573      243 2023-04-12 15:24:32.000000 biobb_io-4.1.0/biobb_io/api/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5082 2023-04-12 15:36:10.000000 biobb_io-4.1.0/biobb_io/api/alphafold.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5527 2023-04-12 15:38:00.000000 biobb_io-4.1.0/biobb_io/api/api_binding_site.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5474 2023-04-12 15:39:47.000000 biobb_io-4.1.0/biobb_io/api/canonical_fasta.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13139 2023-04-17 07:52:28.000000 biobb_io-4.1.0/biobb_io/api/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     4942 2023-04-12 15:44:12.000000 biobb_io-4.1.0/biobb_io/api/drugbank.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5282 2023-04-12 15:52:03.000000 biobb_io-4.1.0/biobb_io/api/ideal_sdf.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5332 2023-05-03 08:22:17.000000 biobb_io-4.1.0/biobb_io/api/ligand.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     4856 2023-04-12 15:57:32.000000 biobb_io-4.1.0/biobb_io/api/memprotmd_sim.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     4821 2023-04-12 15:54:50.000000 biobb_io-4.1.0/biobb_io/api/memprotmd_sim_list.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7179 2023-04-12 15:56:06.000000 biobb_io-4.1.0/biobb_io/api/memprotmd_sim_search.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5366 2023-04-12 15:59:29.000000 biobb_io-4.1.0/biobb_io/api/mmcif.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5674 2023-04-12 16:04:54.000000 biobb_io-4.1.0/biobb_io/api/pdb.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7345 2023-04-12 16:01:22.000000 biobb_io-4.1.0/biobb_io/api/pdb_cluster_zip.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6948 2023-04-12 16:02:37.000000 biobb_io-4.1.0/biobb_io/api/pdb_variants.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5190 2023-04-12 16:06:10.000000 biobb_io-4.1.0/biobb_io/api/structure_info.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-06 14:09:21.401617 biobb_io-4.1.0/biobb_io/test/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-05-26 11:34:05.000000 biobb_io-4.1.0/biobb_io/test/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-06 14:09:21.399227 biobb_io-4.1.0/biobb_io.egg-info/
--rw-r--r--   0 gbayarri (1147421021) 1791188573     6186 2023-09-06 14:09:21.000000 biobb_io-4.1.0/biobb_io.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573      716 2023-09-06 14:09:21.000000 biobb_io-4.1.0/biobb_io.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2023-09-06 14:09:21.000000 biobb_io-4.1.0/biobb_io.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573      652 2023-09-06 14:09:21.000000 biobb_io-4.1.0/biobb_io.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       20 2023-09-06 14:09:21.000000 biobb_io-4.1.0/biobb_io.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573        9 2023-09-06 14:09:21.000000 biobb_io-4.1.0/biobb_io.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2023-09-06 14:09:21.402067 biobb_io-4.1.0/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) 1791188573     2101 2023-09-06 14:05:29.000000 biobb_io-4.1.0/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-07 14:30:48.786547 biobb_io-4.1.1/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11358 2022-05-26 11:34:05.000000 biobb_io-4.1.1/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6760 2024-05-07 14:30:48.786285 biobb_io-4.1.1/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5845 2024-05-07 14:27:42.000000 biobb_io-4.1.1/README.md
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-07 14:30:48.780159 biobb_io-4.1.1/biobb_io/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       58 2024-05-07 14:26:59.000000 biobb_io-4.1.1/biobb_io/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-07 14:30:48.785711 biobb_io-4.1.1/biobb_io/api/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      243 2023-04-12 15:24:32.000000 biobb_io-4.1.1/biobb_io/api/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5082 2023-04-12 15:36:10.000000 biobb_io-4.1.1/biobb_io/api/alphafold.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5527 2023-04-12 15:38:00.000000 biobb_io-4.1.1/biobb_io/api/api_binding_site.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5474 2023-04-12 15:39:47.000000 biobb_io-4.1.1/biobb_io/api/canonical_fasta.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    13075 2024-05-07 14:16:21.000000 biobb_io-4.1.1/biobb_io/api/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     4942 2023-04-12 15:44:12.000000 biobb_io-4.1.1/biobb_io/api/drugbank.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5282 2023-04-12 15:52:03.000000 biobb_io-4.1.1/biobb_io/api/ideal_sdf.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5332 2023-05-03 08:22:17.000000 biobb_io-4.1.1/biobb_io/api/ligand.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     4856 2023-04-12 15:57:32.000000 biobb_io-4.1.1/biobb_io/api/memprotmd_sim.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     4821 2023-04-12 15:54:50.000000 biobb_io-4.1.1/biobb_io/api/memprotmd_sim_list.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7179 2023-04-12 15:56:06.000000 biobb_io-4.1.1/biobb_io/api/memprotmd_sim_search.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5366 2023-04-12 15:59:29.000000 biobb_io-4.1.1/biobb_io/api/mmcif.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5674 2023-04-12 16:04:54.000000 biobb_io-4.1.1/biobb_io/api/pdb.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7345 2023-04-12 16:01:22.000000 biobb_io-4.1.1/biobb_io/api/pdb_cluster_zip.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6948 2023-04-12 16:02:37.000000 biobb_io-4.1.1/biobb_io/api/pdb_variants.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5190 2023-04-12 16:06:10.000000 biobb_io-4.1.1/biobb_io/api/structure_info.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-07 14:30:48.786002 biobb_io-4.1.1/biobb_io/test/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2022-05-26 11:34:05.000000 biobb_io-4.1.1/biobb_io/test/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-07 14:30:48.780968 biobb_io-4.1.1/biobb_io.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6760 2024-05-07 14:30:48.000000 biobb_io-4.1.1/biobb_io.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      716 2024-05-07 14:30:48.000000 biobb_io-4.1.1/biobb_io.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2024-05-07 14:30:48.000000 biobb_io-4.1.1/biobb_io.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      652 2024-05-07 14:30:48.000000 biobb_io-4.1.1/biobb_io.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       20 2024-05-07 14:30:48.000000 biobb_io-4.1.1/biobb_io.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        9 2024-05-07 14:30:48.000000 biobb_io-4.1.1/biobb_io.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2024-05-07 14:30:48.786599 biobb_io-4.1.1/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2101 2024-05-07 14:26:46.000000 biobb_io-4.1.1/setup.py
```

### Comparing `biobb_io-4.1.0/LICENSE` & `biobb_io-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.0/PKG-INFO` & `biobb_io-4.1.1/biobb_io.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
-Name: biobb_io
-Version: 4.1.0
+Name: biobb-io
+Version: 4.1.1
 Summary: Biobb_io is the Biobb module collection to fetch data to be consumed by the rest of the Biobb building blocks.
 Home-page: https://github.com/bioexcel/biobb_io
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
-Project-URL: Documentation, http://biobb_io.readthedocs.io/en/latest/
+Project-URL: Documentation, http://biobb-io.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: biobb_common==4.1.0
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_io?label=Version)](https://GitHub.com/bioexcel/biobb_io/tags/)
 [![](https://img.shields.io/pypi/v/biobb-io.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-io/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_io?label=Conda)](https://anaconda.org/bioconda/biobb_io)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_io?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_io)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_io?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_io:4.1.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_io:4.1.1--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_io)
 [![](https://img.shields.io/pypi/pyversions/biobb-io.svg?label=Python%20Versions)](https://pypi.org/project/biobb-io/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_io)
 
 [![](https://readthedocs.org/projects/biobb-io/badge/?version=latest&label=Docs)](https://biobb-io.readthedocs.io/en/latest/?badge=latest)
@@ -39,84 +40,91 @@
 
 [![](https://docs.bioexcel.eu/biobb_io/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_io/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_io/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_io/coverage/)
 [![](https://docs.bioexcel.eu/biobb_io/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_io/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_io?label=Last%20Commit)](https://github.com/bioexcel/biobb_io/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_io.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_io/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 # biobb_io
 
 ### Introduction
 Biobb_io is the Biobb module collection to fetch data to be consumed by the
 rest of the Biobb building blocks.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_io.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-io.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.3
+v4.1.1 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
-        pip install "biobb_io==4.1.0"
+        pip install "biobb_io==4.1.1"
         
 * Usage: [Python API documentation](https://biobb-io.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 * Installation:
 
 
-        conda install -c bioconda "biobb_io==4.1.0"
+        conda install -c bioconda "biobb_io==4.1.1"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-io.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-io.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_io:4.1.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_io:4.1.1--pyhdfd78af_0
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_io:4.1.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_io:4.1.1--pyhdfd78af_0 <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-io.readthedocs.io/en/latest/command_line.html).
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_io.sif https://depot.galaxyproject.org/singularity/biobb_io:4.1.0--pyhdfd78af_0
+        singularity pull --name biobb_io.sif https://depot.galaxyproject.org/singularity/biobb_io:4.1.1--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_io.sif <command>
 
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-io.readthedocs.io/en/latest/command_line.html).
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2024 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2024 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_io-4.1.0/README.md` & `biobb_io-4.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_io?label=Version)](https://GitHub.com/bioexcel/biobb_io/tags/)
 [![](https://img.shields.io/pypi/v/biobb-io.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-io/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_io?label=Conda)](https://anaconda.org/bioconda/biobb_io)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_io?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_io)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_io?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_io:4.1.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_io:4.1.1--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_io)
 [![](https://img.shields.io/pypi/pyversions/biobb-io.svg?label=Python%20Versions)](https://pypi.org/project/biobb-io/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_io)
 
 [![](https://readthedocs.org/projects/biobb-io/badge/?version=latest&label=Docs)](https://biobb-io.readthedocs.io/en/latest/?badge=latest)
@@ -18,84 +18,91 @@
 
 [![](https://docs.bioexcel.eu/biobb_io/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_io/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_io/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_io/coverage/)
 [![](https://docs.bioexcel.eu/biobb_io/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_io/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_io?label=Last%20Commit)](https://github.com/bioexcel/biobb_io/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_io.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_io/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 # biobb_io
 
 ### Introduction
 Biobb_io is the Biobb module collection to fetch data to be consumed by the
 rest of the Biobb building blocks.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_io.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-io.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.3
+v4.1.1 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
-        pip install "biobb_io==4.1.0"
+        pip install "biobb_io==4.1.1"
         
 * Usage: [Python API documentation](https://biobb-io.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 * Installation:
 
 
-        conda install -c bioconda "biobb_io==4.1.0"
+        conda install -c bioconda "biobb_io==4.1.1"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-io.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-io.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_io:4.1.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_io:4.1.1--pyhdfd78af_0
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_io:4.1.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_io:4.1.1--pyhdfd78af_0 <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-io.readthedocs.io/en/latest/command_line.html).
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_io.sif https://depot.galaxyproject.org/singularity/biobb_io:4.1.0--pyhdfd78af_0
+        singularity pull --name biobb_io.sif https://depot.galaxyproject.org/singularity/biobb_io:4.1.1--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_io.sif <command>
 
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-io.readthedocs.io/en/latest/command_line.html).
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2024 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2024 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_io-4.1.0/biobb_io/api/alphafold.py` & `biobb_io-4.1.1/biobb_io/api/alphafold.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.0/biobb_io/api/api_binding_site.py` & `biobb_io-4.1.1/biobb_io/api/api_binding_site.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.0/biobb_io/api/canonical_fasta.py` & `biobb_io-4.1.1/biobb_io/api/canonical_fasta.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.0/biobb_io/api/common.py` & `biobb_io-4.1.1/biobb_io/api/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         String: Content of the ligand file.
     """
 
     if api_id == 'mmb':
         url = "http://mmb.irbbarcelona.org/api/pdbMonomer/" + ligand_code.lower()
         text = requests.get(url, verify=False).content.decode('utf-8')
     elif api_id == 'pdbe':
-        url = "ftp://ftp.ebi.ac.uk/pub/databases/msd/pdbechem_v2/{0}/{1}/{1}_ideal.pdb".format(ligand_code.upper()[0], ligand_code.upper())
+        url = "https://www.ebi.ac.uk/pdbe/static/files/pdbechem_v2/" + ligand_code.upper() + "_ideal.pdb"
         text = urllib.request.urlopen(url).read().decode('utf-8')
 
     fu.log("Downloading %s from: %s" % (ligand_code, url), out_log, global_log)
 
     # removing useless empty lines at the end of the file
     text = os.linesep.join([s for s in text.splitlines() if s])
 
@@ -162,18 +162,18 @@
 def download_ideal_sdf(ligand_code, api_id, out_log=None, global_log=None):
     """
     Returns:
         String: Content of the ideal sdf file.
     """
 
     if api_id == 'pdb':
-        url = "https://files.rcsb.org/ligands/view/" + ligand_code.upper() + "_ideal.sdf"
+        url = "https://files.rcsb.org/ligands/download/" + ligand_code.upper() + "_ideal.sdf"
         text = requests.get(url, verify=False).content.decode('utf-8')
     elif api_id == 'pdbe':
-        url = "ftp://ftp.ebi.ac.uk/pub/databases/msd/pdbechem_v2/{0}/{1}/{1}_ideal.sdf".format(ligand_code.upper()[0], ligand_code.upper())
+        url = "https://www.ebi.ac.uk/pdbe/static/files/pdbechem_v2/" + ligand_code.upper() + "_ideal.sdf"
         text = urllib.request.urlopen(url).read().decode('utf-8')
 
     fu.log("Downloading %s from: %s" % (ligand_code, url), out_log, global_log)
 
     return text
```

### Comparing `biobb_io-4.1.0/biobb_io/api/drugbank.py` & `biobb_io-4.1.1/biobb_io/api/drugbank.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.0/biobb_io/api/ideal_sdf.py` & `biobb_io-4.1.1/biobb_io/api/ideal_sdf.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.0/biobb_io/api/ligand.py` & `biobb_io-4.1.1/biobb_io/api/ligand.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.0/biobb_io/api/memprotmd_sim.py` & `biobb_io-4.1.1/biobb_io/api/memprotmd_sim.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.0/biobb_io/api/memprotmd_sim_list.py` & `biobb_io-4.1.1/biobb_io/api/memprotmd_sim_list.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.0/biobb_io/api/memprotmd_sim_search.py` & `biobb_io-4.1.1/biobb_io/api/memprotmd_sim_search.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.0/biobb_io/api/mmcif.py` & `biobb_io-4.1.1/biobb_io/api/mmcif.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.0/biobb_io/api/pdb.py` & `biobb_io-4.1.1/biobb_io/api/pdb.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.0/biobb_io/api/pdb_cluster_zip.py` & `biobb_io-4.1.1/biobb_io/api/pdb_cluster_zip.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.0/biobb_io/api/pdb_variants.py` & `biobb_io-4.1.1/biobb_io/api/pdb_variants.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.0/biobb_io/api/structure_info.py` & `biobb_io-4.1.1/biobb_io/api/structure_info.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.0/biobb_io.egg-info/PKG-INFO` & `biobb_io-4.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
-Name: biobb-io
-Version: 4.1.0
+Name: biobb_io
+Version: 4.1.1
 Summary: Biobb_io is the Biobb module collection to fetch data to be consumed by the rest of the Biobb building blocks.
 Home-page: https://github.com/bioexcel/biobb_io
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
-Project-URL: Documentation, http://biobb_io.readthedocs.io/en/latest/
+Project-URL: Documentation, http://biobb-io.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: biobb_common==4.1.0
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_io?label=Version)](https://GitHub.com/bioexcel/biobb_io/tags/)
 [![](https://img.shields.io/pypi/v/biobb-io.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-io/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_io?label=Conda)](https://anaconda.org/bioconda/biobb_io)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_io?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_io)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_io?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_io:4.1.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_io:4.1.1--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_io)
 [![](https://img.shields.io/pypi/pyversions/biobb-io.svg?label=Python%20Versions)](https://pypi.org/project/biobb-io/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_io)
 
 [![](https://readthedocs.org/projects/biobb-io/badge/?version=latest&label=Docs)](https://biobb-io.readthedocs.io/en/latest/?badge=latest)
@@ -39,84 +40,91 @@
 
 [![](https://docs.bioexcel.eu/biobb_io/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_io/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_io/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_io/coverage/)
 [![](https://docs.bioexcel.eu/biobb_io/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_io/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_io?label=Last%20Commit)](https://github.com/bioexcel/biobb_io/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_io.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_io/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 # biobb_io
 
 ### Introduction
 Biobb_io is the Biobb module collection to fetch data to be consumed by the
 rest of the Biobb building blocks.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_io.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-io.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.3
+v4.1.1 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
-        pip install "biobb_io==4.1.0"
+        pip install "biobb_io==4.1.1"
         
 * Usage: [Python API documentation](https://biobb-io.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 * Installation:
 
 
-        conda install -c bioconda "biobb_io==4.1.0"
+        conda install -c bioconda "biobb_io==4.1.1"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-io.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-io.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_io:4.1.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_io:4.1.1--pyhdfd78af_0
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_io:4.1.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_io:4.1.1--pyhdfd78af_0 <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-io.readthedocs.io/en/latest/command_line.html).
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_io.sif https://depot.galaxyproject.org/singularity/biobb_io:4.1.0--pyhdfd78af_0
+        singularity pull --name biobb_io.sif https://depot.galaxyproject.org/singularity/biobb_io:4.1.1--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_io.sif <command>
 
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-io.readthedocs.io/en/latest/command_line.html).
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2024 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2024 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_io-4.1.0/biobb_io.egg-info/SOURCES.txt` & `biobb_io-4.1.1/biobb_io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.0/biobb_io.egg-info/entry_points.txt` & `biobb_io-4.1.1/biobb_io.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.0/setup.py` & `biobb_io-4.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_io",
-    version="4.1.0",
+    version="4.1.1",
     author="Biobb developers",
     author_email="pau.andrio@bsc.es",
     description="Biobb_io is the Biobb module collection to fetch data to be consumed by the rest of the Biobb building blocks.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_io",
     project_urls={
-        "Documentation": "http://biobb_io.readthedocs.io/en/latest/",
+        "Documentation": "http://biobb-io.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs', 'test']),
     install_requires=['biobb_common==4.1.0'],
     python_requires='>=3.8',
     entry_points={
         "console_scripts": [
```

