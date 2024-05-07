# Comparing `tmp/modnet-0.4.3.tar.gz` & `tmp/modnet-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/modnet-0.4.3.tar", last modified: Fri Apr  5 10:43:47 2024, max compression
+gzip compressed data, was "modnet-0.4.4.tar", last modified: Tue May  7 14:09:53 2024, max compression
```

## Comparing `modnet-0.4.3.tar` & `modnet-0.4.4.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-05 10:43:47.000000 modnet-0.4.3/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     1078 2022-01-10 10:10:32.000000 modnet-0.4.3/LICENSE.md
--rw-r--r--   0 ppdebreuck   (501) staff       (20)       48 2022-01-10 10:10:32.000000 modnet-0.4.3/MANIFEST.in
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     6057 2024-04-05 10:43:47.000000 modnet-0.4.3/PKG-INFO
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     4243 2023-07-11 13:21:01.000000 modnet-0.4.3/README.md
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-05 10:43:46.000000 modnet-0.4.3/modnet/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)       22 2024-04-05 10:41:33.000000 modnet-0.4.3/modnet/__init__.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-05 10:43:46.000000 modnet-0.4.3/modnet/data/
--rw-r--r--   0 ppdebreuck   (501) staff       (20) 13666623 2021-11-08 13:57:41.000000 modnet-0.4.3/modnet/data/Features_cross
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     4055 2022-05-12 10:28:50.000000 modnet-0.4.3/modnet/ext_data.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-05 10:43:47.000000 modnet-0.4.3/modnet/featurizers/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      264 2021-02-15 14:07:41.000000 modnet-0.4.3/modnet/featurizers/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    12908 2024-04-02 15:48:26.000000 modnet-0.4.3/modnet/featurizers/featurizers.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-05 10:43:47.000000 modnet-0.4.3/modnet/featurizers/presets/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      978 2023-07-11 13:21:01.000000 modnet-0.4.3/modnet/featurizers/presets/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    10080 2023-07-28 12:09:44.000000 modnet-0.4.3/modnet/featurizers/presets/debreuck_2020.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     9303 2023-07-28 12:09:44.000000 modnet-0.4.3/modnet/featurizers/presets/matminer_2023.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    16049 2023-07-28 12:09:44.000000 modnet-0.4.3/modnet/featurizers/presets/matminer_all_2023.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      623 2023-07-28 12:09:44.000000 modnet-0.4.3/modnet/featurizers/utils.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-05 10:43:47.000000 modnet-0.4.3/modnet/hyper_opt/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)       63 2022-01-12 21:23:06.000000 modnet-0.4.3/modnet/hyper_opt/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    27301 2024-03-28 10:26:50.000000 modnet-0.4.3/modnet/hyper_opt/fit_genetic.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-05 10:43:47.000000 modnet-0.4.3/modnet/matbench/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      116 2021-02-15 14:07:41.000000 modnet-0.4.3/modnet/matbench/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    11640 2023-07-11 13:21:01.000000 modnet-0.4.3/modnet/matbench/benchmark.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-05 10:43:47.000000 modnet-0.4.3/modnet/model_presets/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      166 2022-01-10 10:10:32.000000 modnet-0.4.3/modnet/model_presets/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     2292 2021-08-16 13:22:38.000000 modnet-0.4.3/modnet/model_presets/presets.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-05 10:43:47.000000 modnet-0.4.3/modnet/models/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      402 2024-02-07 15:47:41.000000 modnet-0.4.3/modnet/models/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    15169 2024-04-02 15:48:26.000000 modnet-0.4.3/modnet/models/bayesian.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    17887 2024-03-28 10:26:50.000000 modnet-0.4.3/modnet/models/ensemble.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    60336 2024-04-05 10:41:01.000000 modnet-0.4.3/modnet/models/vanilla.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    41991 2024-03-28 10:26:50.000000 modnet-0.4.3/modnet/preprocessing.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     6344 2024-03-28 10:26:50.000000 modnet-0.4.3/modnet/sklearn.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-05 10:43:47.000000 modnet-0.4.3/modnet/tests/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)        0 2020-09-16 10:22:36.000000 modnet-0.4.3/modnet/tests/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     4550 2024-04-02 15:48:26.000000 modnet-0.4.3/modnet/tests/conftest.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     4444 2023-07-11 13:21:01.000000 modnet-0.4.3/modnet/tests/test_benchmark.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      563 2021-01-14 10:39:09.000000 modnet-0.4.3/modnet/tests/test_ext_data.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      771 2024-04-02 15:48:22.000000 modnet-0.4.3/modnet/tests/test_hyper_opt.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    10034 2024-04-05 10:41:01.000000 modnet-0.4.3/modnet/tests/test_model.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    17907 2024-04-02 15:48:26.000000 modnet-0.4.3/modnet/tests/test_preprocessing.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     3110 2022-05-19 13:18:13.000000 modnet-0.4.3/modnet/tests/test_sklearn.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      737 2021-02-15 14:07:41.000000 modnet-0.4.3/modnet/utils.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-05 10:43:46.000000 modnet-0.4.3/modnet.egg-info/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     6057 2024-04-05 10:43:46.000000 modnet-0.4.3/modnet.egg-info/PKG-INFO
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     1110 2024-04-05 10:43:46.000000 modnet-0.4.3/modnet.egg-info/SOURCES.txt
--rw-r--r--   0 ppdebreuck   (501) staff       (20)        1 2024-04-05 10:43:46.000000 modnet-0.4.3/modnet.egg-info/dependency_links.txt
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      206 2024-04-05 10:43:46.000000 modnet-0.4.3/modnet.egg-info/requires.txt
--rw-r--r--   0 ppdebreuck   (501) staff       (20)        7 2024-04-05 10:43:46.000000 modnet-0.4.3/modnet.egg-info/top_level.txt
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      118 2024-04-05 10:43:47.000000 modnet-0.4.3/setup.cfg
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     1877 2024-04-02 15:48:26.000000 modnet-0.4.3/setup.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-05-07 14:09:53.417538 modnet-0.4.4/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     1078 2022-01-10 10:10:32.000000 modnet-0.4.4/LICENSE.md
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)       48 2022-01-10 10:10:32.000000 modnet-0.4.4/MANIFEST.in
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     5234 2024-05-07 14:09:53.417857 modnet-0.4.4/PKG-INFO
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     4243 2023-07-11 13:21:01.000000 modnet-0.4.4/README.md
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-05-07 14:09:53.353798 modnet-0.4.4/modnet/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)       22 2024-05-07 14:07:55.000000 modnet-0.4.4/modnet/__init__.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-05-07 14:09:53.356560 modnet-0.4.4/modnet/data/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20) 13666623 2021-11-08 13:57:41.000000 modnet-0.4.4/modnet/data/Features_cross
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     4055 2022-05-12 10:28:50.000000 modnet-0.4.4/modnet/ext_data.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-05-07 14:09:53.384879 modnet-0.4.4/modnet/featurizers/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      264 2021-02-15 14:07:41.000000 modnet-0.4.4/modnet/featurizers/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    12908 2024-04-02 15:48:26.000000 modnet-0.4.4/modnet/featurizers/featurizers.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-05-07 14:09:53.393173 modnet-0.4.4/modnet/featurizers/presets/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      978 2023-07-11 13:21:01.000000 modnet-0.4.4/modnet/featurizers/presets/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    10080 2023-07-28 12:09:44.000000 modnet-0.4.4/modnet/featurizers/presets/debreuck_2020.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     9303 2023-07-28 12:09:44.000000 modnet-0.4.4/modnet/featurizers/presets/matminer_2023.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     7620 2024-05-07 14:07:32.000000 modnet-0.4.4/modnet/featurizers/presets/matminer_2024_fast.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    16049 2023-07-28 12:09:44.000000 modnet-0.4.4/modnet/featurizers/presets/matminer_all_2023.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      623 2023-07-28 12:09:44.000000 modnet-0.4.4/modnet/featurizers/utils.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-05-07 14:09:53.395248 modnet-0.4.4/modnet/hyper_opt/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)       63 2022-01-12 21:23:06.000000 modnet-0.4.4/modnet/hyper_opt/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    27301 2024-03-28 10:26:50.000000 modnet-0.4.4/modnet/hyper_opt/fit_genetic.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-05-07 14:09:53.397627 modnet-0.4.4/modnet/matbench/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      116 2021-02-15 14:07:41.000000 modnet-0.4.4/modnet/matbench/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    11640 2023-07-11 13:21:01.000000 modnet-0.4.4/modnet/matbench/benchmark.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-05-07 14:09:53.400165 modnet-0.4.4/modnet/model_presets/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      166 2022-01-10 10:10:32.000000 modnet-0.4.4/modnet/model_presets/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     2292 2021-08-16 13:22:38.000000 modnet-0.4.4/modnet/model_presets/presets.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-05-07 14:09:53.406868 modnet-0.4.4/modnet/models/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      402 2024-02-07 15:47:41.000000 modnet-0.4.4/modnet/models/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    15169 2024-04-02 15:48:26.000000 modnet-0.4.4/modnet/models/bayesian.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    18167 2024-05-07 14:07:32.000000 modnet-0.4.4/modnet/models/ensemble.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    60644 2024-05-07 14:07:32.000000 modnet-0.4.4/modnet/models/vanilla.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    42343 2024-05-07 14:07:32.000000 modnet-0.4.4/modnet/preprocessing.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     6344 2024-03-28 10:26:50.000000 modnet-0.4.4/modnet/sklearn.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-05-07 14:09:53.416700 modnet-0.4.4/modnet/tests/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)        0 2020-09-16 10:22:36.000000 modnet-0.4.4/modnet/tests/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     4550 2024-04-02 15:48:26.000000 modnet-0.4.4/modnet/tests/conftest.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     4444 2023-07-11 13:21:01.000000 modnet-0.4.4/modnet/tests/test_benchmark.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      563 2021-01-14 10:39:09.000000 modnet-0.4.4/modnet/tests/test_ext_data.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      771 2024-04-02 15:48:22.000000 modnet-0.4.4/modnet/tests/test_hyper_opt.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    10034 2024-04-05 10:41:01.000000 modnet-0.4.4/modnet/tests/test_model.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    17907 2024-04-02 15:48:26.000000 modnet-0.4.4/modnet/tests/test_preprocessing.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     3110 2022-05-19 13:18:13.000000 modnet-0.4.4/modnet/tests/test_sklearn.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      737 2021-02-15 14:07:41.000000 modnet-0.4.4/modnet/utils.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-05-07 14:09:53.356038 modnet-0.4.4/modnet.egg-info/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     5234 2024-05-07 14:09:53.000000 modnet-0.4.4/modnet.egg-info/PKG-INFO
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     1159 2024-05-07 14:09:53.000000 modnet-0.4.4/modnet.egg-info/SOURCES.txt
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)        1 2024-05-07 14:09:53.000000 modnet-0.4.4/modnet.egg-info/dependency_links.txt
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      206 2024-05-07 14:09:53.000000 modnet-0.4.4/modnet.egg-info/requires.txt
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)        7 2024-05-07 14:09:53.000000 modnet-0.4.4/modnet.egg-info/top_level.txt
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      118 2024-05-07 14:09:53.418790 modnet-0.4.4/setup.cfg
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     1877 2024-04-02 15:48:26.000000 modnet-0.4.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `modnet-0.4.3/LICENSE.md` & `modnet-0.4.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `modnet-0.4.3/PKG-INFO` & `modnet-0.4.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,125 +1,124 @@
 Metadata-Version: 2.1
 Name: modnet
-Version: 0.4.3
+Version: 0.4.4
 Summary: MODNet, the Material Optimal Descriptor Network for materials properties prediction. 
 Home-page: https://github.com/ppdebreuck/modnet
 Author: Pierre-Paul De Breuck
 Author-email: pierre-paul.debreuck@uclouvain.be
-License: UNKNOWN
 Project-URL: GitHub, https://github.com/ppdebreuck/modnet
 Project-URL: Documentation, https://modnet.readthedocs.io
-Description: <div align="center">
-            <img src="img/modnet_logo.svg" alt="modnet-logo"  width=200>
-            <br>
-        
-        # MODNet: Material Optimal Descriptor Network
-        
-        [![arXiv](https://img.shields.io/badge/arXiv-2004.14766-brightgreen)](https://arxiv.org/abs/2004.14766) [![Build Status](https://img.shields.io/github/actions/workflow/status/ppdebreuck/modnet/ci.yml?logo=github&branch=main)](https://github.com/ppdebreuck/modnet/actions?query=branch%3Amaster+) [![Read the Docs](https://img.shields.io/readthedocs/modnet)](https://modnet.readthedocs.io/en/latest/)
-        
-        </div>
-        
-        <a name="introduction"></a>
-        ## Introduction
-        This repository contains the Python (3.8+) package implementing the Material Optimal Descriptor Network (MODNet).
-        It is a supervised machine learning framework for **learning material properties** from
-        either the **composition** or  **crystal structure**. The framework is well suited for **limited datasets**
-        and can be used for learning *multiple* properties together by using **joint learning**.
-        
-        MODNet appears on the [MatBench leaderboard](https://matbench.materialsproject.org/). As of 11/11/2021, MODNet provides the best performance of all submitted models on 7 out of 13 tasks.
-        
-        This repository also contains two [pretrained models](#pretrained) that can be used for predicting
-        the refractive index and vibrational thermodynamics from any crystal structure.
-        
-        See the MODNet papers and repositories below for more details:
-        
-        - De Breuck *et al.*, "Materials property prediction for limited datasets enabled by feature selection and joint learning with MODNet." *npj Comput Mater* **7**, 83 (2021). [10.1038/s41524-021-00552-2](https://doi.org/10.1038/s41524-021-00552-2) (preprint: [arXiv:2004.14766](https://arxiv.org/abs/2004.14766)).
-        - De Breuck *et al.*, "Robust model benchmarking and bias-imbalance in data-driven materials science: a case study on MODNet." *J. Phys.: Condens. Matter* **33** 404002,  (2021), [10.1088/1361-648X/ac1280](https://doi.org/10.1088/1361-648X/ac1280) (preprint: [arXiv:2102.02263](https://arxiv.org/abs/2102.02263)).
-        - MatBench benchmarking data repository: [modl-uclouvain/modnet-matbench](https://github.com/modl-uclouvain/modnet-matbench).
-        
-        
-        
-        <p align='center'>
-        <img src="img/MODNet_schematic.PNG" alt="MODNet schematic" />
-        </p>
-        <div align='center'>
-        <strong>Figure 1. Schematic representation of the MODNet.</strong>
-        </div>
-        
-        
-        <a name="install"></a>
-        ## How to install
-        
-        First, create a virtual environment (e.g., named modnet) with Python (3.8+) using
-        your favourite environment manager (the following instructions use
-        [conda](https://docs.conda.io/)):
-        
-        ```shell
-        conda create -n modnet python=3.9
-        ```
-        
-        Activate the environment:
-        
-        ```shell
-        conda activate modnet
-        ```
-        
-        Finally, install MODNet from PyPI with `pip`:
-        
-        ```shell
-        pip install modnet
-        ```
-        
-        >**Warning**
-        >We strongly recommend pinning your Python environment when using MODNet
-        >across multiple machines, or multiple MODNet versions, as changes to the
-        >dependencies and sub-dependencies can lead to different values for particular
-        >features.
-        >
-        >This can be achieved with `conda export` or `pip freeze`.
-        
-        For development (or if you wish to use pinned versions of direct dependencies that
-        MODNet has been tested with), you can clone this git repository and make an
-        editable install inside your chosen environment with `pip`:
-        
-        ```shell
-        git clone git@github.com:ppdebreuck/modnet
-        cd modnet
-        conda create -n modnet python=3.9
-        conda activate modnet
-        pip install -r requirements.txt  # optionally use pinned requirements
-        pip install -e .
-        ```
-        
-        
-        <a name="documentation"></a>
-        ## Documentation
-        The documentation is available at [ReadTheDocs](https://modnet.readthedocs.io).
-        
-        <a name="changelog"></a>
-        ## Changelog
-        A brief changelog can be found in the [release summaries on GitHub](https://github.com/ppdebreuck/modnet/releases).
-        
-        <a name="author"></a>
-        ## Author
-        This software was written by [Pierre-Paul De Breuck](mailto:pierre-paul.debreuck@uclouvain.be) and [Matthew Evans](https://www.github.com/ml-evs) with contributions from David Waroquiers and  Gregoire Heymans.
-        For an up-to-date list, see the [Contributors on GitHub](https://github.com/ppdebreuck/modnet/graphs/contributors).
-        
-        <a name="License"></a>
-        ## License
-        
-        MODNet is released under the MIT License.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: bayesian
 Provides-Extra: test
 Provides-Extra: dev
+License-File: LICENSE.md
+
+<div align="center">
+    <img src="img/modnet_logo.svg" alt="modnet-logo"  width=200>
+    <br>
+
+# MODNet: Material Optimal Descriptor Network
+
+[![arXiv](https://img.shields.io/badge/arXiv-2004.14766-brightgreen)](https://arxiv.org/abs/2004.14766) [![Build Status](https://img.shields.io/github/actions/workflow/status/ppdebreuck/modnet/ci.yml?logo=github&branch=main)](https://github.com/ppdebreuck/modnet/actions?query=branch%3Amaster+) [![Read the Docs](https://img.shields.io/readthedocs/modnet)](https://modnet.readthedocs.io/en/latest/)
+
+</div>
+
+<a name="introduction"></a>
+## Introduction
+This repository contains the Python (3.8+) package implementing the Material Optimal Descriptor Network (MODNet).
+It is a supervised machine learning framework for **learning material properties** from
+either the **composition** or  **crystal structure**. The framework is well suited for **limited datasets**
+and can be used for learning *multiple* properties together by using **joint learning**.
+
+MODNet appears on the [MatBench leaderboard](https://matbench.materialsproject.org/). As of 11/11/2021, MODNet provides the best performance of all submitted models on 7 out of 13 tasks.
+
+This repository also contains two [pretrained models](#pretrained) that can be used for predicting
+the refractive index and vibrational thermodynamics from any crystal structure.
+
+See the MODNet papers and repositories below for more details:
+
+- De Breuck *et al.*, "Materials property prediction for limited datasets enabled by feature selection and joint learning with MODNet." *npj Comput Mater* **7**, 83 (2021). [10.1038/s41524-021-00552-2](https://doi.org/10.1038/s41524-021-00552-2) (preprint: [arXiv:2004.14766](https://arxiv.org/abs/2004.14766)).
+- De Breuck *et al.*, "Robust model benchmarking and bias-imbalance in data-driven materials science: a case study on MODNet." *J. Phys.: Condens. Matter* **33** 404002,  (2021), [10.1088/1361-648X/ac1280](https://doi.org/10.1088/1361-648X/ac1280) (preprint: [arXiv:2102.02263](https://arxiv.org/abs/2102.02263)).
+- MatBench benchmarking data repository: [modl-uclouvain/modnet-matbench](https://github.com/modl-uclouvain/modnet-matbench).
+
+
+
+<p align='center'>
+<img src="img/MODNet_schematic.PNG" alt="MODNet schematic" />
+</p>
+<div align='center'>
+<strong>Figure 1. Schematic representation of the MODNet.</strong>
+</div>
+
+
+<a name="install"></a>
+## How to install
+
+First, create a virtual environment (e.g., named modnet) with Python (3.8+) using
+your favourite environment manager (the following instructions use
+[conda](https://docs.conda.io/)):
+
+```shell
+conda create -n modnet python=3.9
+```
+
+Activate the environment:
+
+```shell
+conda activate modnet
+```
+
+Finally, install MODNet from PyPI with `pip`:
+
+```shell
+pip install modnet
+```
+
+>**Warning**
+>We strongly recommend pinning your Python environment when using MODNet
+>across multiple machines, or multiple MODNet versions, as changes to the
+>dependencies and sub-dependencies can lead to different values for particular
+>features.
+>
+>This can be achieved with `conda export` or `pip freeze`.
+
+For development (or if you wish to use pinned versions of direct dependencies that
+MODNet has been tested with), you can clone this git repository and make an
+editable install inside your chosen environment with `pip`:
+
+```shell
+git clone git@github.com:ppdebreuck/modnet
+cd modnet
+conda create -n modnet python=3.9
+conda activate modnet
+pip install -r requirements.txt  # optionally use pinned requirements
+pip install -e .
+```
+
+
+<a name="documentation"></a>
+## Documentation
+The documentation is available at [ReadTheDocs](https://modnet.readthedocs.io).
+
+<a name="changelog"></a>
+## Changelog
+A brief changelog can be found in the [release summaries on GitHub](https://github.com/ppdebreuck/modnet/releases).
+
+<a name="author"></a>
+## Author
+This software was written by [Pierre-Paul De Breuck](mailto:pierre-paul.debreuck@uclouvain.be) and [Matthew Evans](https://www.github.com/ml-evs) with contributions from David Waroquiers and  Gregoire Heymans.
+For an up-to-date list, see the [Contributors on GitHub](https://github.com/ppdebreuck/modnet/graphs/contributors).
+
+<a name="License"></a>
+## License
+
+MODNet is released under the MIT License.
```

### Comparing `modnet-0.4.3/README.md` & `modnet-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `modnet-0.4.3/modnet/data/Features_cross` & `modnet-0.4.4/modnet/data/Features_cross`

 * *Files identical despite different names*

### Comparing `modnet-0.4.3/modnet/ext_data.py` & `modnet-0.4.4/modnet/ext_data.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.3/modnet/featurizers/featurizers.py` & `modnet-0.4.4/modnet/featurizers/featurizers.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.3/modnet/featurizers/presets/__init__.py` & `modnet-0.4.4/modnet/featurizers/presets/__init__.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.3/modnet/featurizers/presets/debreuck_2020.py` & `modnet-0.4.4/modnet/featurizers/presets/debreuck_2020.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.3/modnet/featurizers/presets/matminer_2023.py` & `modnet-0.4.4/modnet/featurizers/presets/matminer_2023.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.3/modnet/featurizers/presets/matminer_all_2023.py` & `modnet-0.4.4/modnet/featurizers/presets/matminer_all_2023.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.3/modnet/featurizers/utils.py` & `modnet-0.4.4/modnet/featurizers/utils.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.3/modnet/hyper_opt/fit_genetic.py` & `modnet-0.4.4/modnet/hyper_opt/fit_genetic.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.3/modnet/matbench/benchmark.py` & `modnet-0.4.4/modnet/matbench/benchmark.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.3/modnet/model_presets/presets.py` & `modnet-0.4.4/modnet/model_presets/presets.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.3/modnet/models/bayesian.py` & `modnet-0.4.4/modnet/models/bayesian.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.3/modnet/models/ensemble.py` & `modnet-0.4.4/modnet/models/ensemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,34 +140,43 @@
                 for k in model.history.keys():
                     model_summary += "{}: {:.4f}\t".format(k, model.history[k][-1])
                 LOG.info(model_summary)
             pool.close()
             pool.join()
 
     def predict(
-        self, test_data: MODData, return_unc=False, return_prob=False
+        self,
+        test_data: MODData,
+        return_unc: bool = False,
+        return_prob: bool = False,
+        remap_out_of_bounds: bool = True,
     ) -> pd.DataFrame:
         """Predict the target values for the passed MODData.
 
         Parameters:
             test_data: A featurized and feature-selected `MODData`
                 object containing the descriptors used in training.
             return_prob: For a classification task only: whether to return the probability of each
                 class OR only return the most probable class.
             return_unc: whether to return a second dataframe containing the uncertainties
+            remap_out_of_bounds: whether to remap out-of-bounds values to the nearest bound.
 
         Returns:
             A `pandas.DataFrame` containing the predicted values of the targets.
 
 
         """
 
         all_predictions = []
         for i in range(self.n_models):
-            p = self.models[i].predict(test_data, return_prob=return_prob)
+            p = self.models[i].predict(
+                test_data,
+                return_prob=return_prob,
+                remap_out_of_bounds=remap_out_of_bounds,
+            )
             all_predictions.append(p.values)
 
         p_mean = np.array(all_predictions).mean(axis=0)
         p_std = np.array(all_predictions).std(axis=0)
 
         df_mean = pd.DataFrame(p_mean, index=p.index, columns=p.columns)
         df_std = pd.DataFrame(p_std, index=p.index, columns=p.columns)
```

### Comparing `modnet-0.4.3/modnet/models/vanilla.py` & `modnet-0.4.4/modnet/models/vanilla.py`

 * *Files 2% similar despite different names*

```diff
@@ -689,22 +689,28 @@
             self._imputer = best_model._imputer
             self._scale_impute = best_model._scale_impute
 
         os.environ["TF_CPP_MIN_LOG_LEVEL"] = "0"  # reset
 
         return models, val_losses, best_learning_curve, learning_curves, best_preset
 
-    def predict(self, test_data: MODData, return_prob=False) -> pd.DataFrame:
+    def predict(
+        self,
+        test_data: MODData,
+        return_prob: bool = False,
+        remap_out_of_bounds: bool = True,
+    ) -> pd.DataFrame:
         """Predict the target values for the passed MODData.
 
         Parameters:
             test_data: A featurized and feature-selected `MODData`
                 object containing the descriptors used in training.
             return_prob: For a classification tasks only: whether to return the probability of each
                 class OR only return the most probable class.
+            remap_out_of_bounds: Whether to remap out-of-bounds predictions to the training data distribution.
 
         Returns:
             A `pandas.DataFrame` containing the predicted values of the targets.
 
 
         """
         # prevents Nan predictions if some features are inf
@@ -720,28 +726,30 @@
 
         p = self.model.predict(x)
 
         if len(self.targets_groups) == 1:
             p = [p]
 
         # post-process based on training data
-        if max(self.num_classes.values()) <= 2:  # regression
-            for i, vals in enumerate(p):
-                yrange = self.max_y[i] - self.min_y[i]
-                upper_bound = self.max_y[i] + 0.25 * yrange
-                lower_bound = self.min_y[i] - 0.25 * yrange
-                for j in range(len(self.targets_groups[i])):
-                    out_of_range_idxs = np.where(
-                        (vals[:, j] < lower_bound[j]) | (vals[:, j] > upper_bound[j])
-                    )
-                    vals[out_of_range_idxs, j] = (
-                        np.random.uniform(0, 1, size=len(out_of_range_idxs[0]))
-                        * (yrange[j])
-                        + self.min_y[i][j]
-                    )
+        if remap_out_of_bounds:
+            if max(self.num_classes.values()) <= 2:  # regression
+                for i, vals in enumerate(p):
+                    yrange = self.max_y[i] - self.min_y[i]
+                    upper_bound = self.max_y[i] + 0.25 * yrange
+                    lower_bound = self.min_y[i] - 0.25 * yrange
+                    for j in range(len(self.targets_groups[i])):
+                        out_of_range_idxs = np.where(
+                            (vals[:, j] < lower_bound[j])
+                            | (vals[:, j] > upper_bound[j])
+                        )
+                        vals[out_of_range_idxs, j] = (
+                            np.random.uniform(0, 1, size=len(out_of_range_idxs[0]))
+                            * (yrange[j])
+                            + self.min_y[i][j]
+                        )
 
         p_dic = {}
 
         for i, props in enumerate(self.targets_groups):
             name = props[0]
             if self.num_classes[name] >= 2:
                 if return_prob:
```

### Comparing `modnet-0.4.3/modnet/preprocessing.py` & `modnet-0.4.4/modnet/preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -660,16 +660,20 @@
             else:
                 self.featurizer = FEATURIZER_PRESETS[DEFAULT_FEATURIZER]()
 
         if self.featurizer is not None:
             LOG.info(f"Loaded {self.featurizer.__class__.__name__} featurizer.")
 
         if target_names is not None:
+            if isinstance(target_names, str):
+                target_names = [target_names]
             if np.shape(targets)[-1] != len(target_names):
-                raise ValueError("Target names must be supplied for every target.")
+                raise ValueError(
+                    f"Target names must be supplied for every target: {np.shape(targets)} vs {target_names=}"
+                )
         elif targets is not None:
             if len(np.shape(targets)) == 1:
                 target_names = ["prop0"]
             else:
                 target_names = ["prop" + str(i) for i in range(np.shape(targets)[1])]
 
         if structure_ids is not None:
@@ -677,24 +681,28 @@
             # IDs, so they can be used when loading from a database file
             # check ids are unique
             if len(set(structure_ids)) != len(structure_ids):
                 raise ValueError(
                     "List of IDs (`structure_ids`) provided must be unique."
                 )
 
-            if len(structure_ids) != len(materials):
-                raise ValueError(
-                    "List of IDs (`structure_ids`) must have same length as list of structure."
-                )
+            if materials is not None:
+                if len(structure_ids) != len(materials):
+                    raise ValueError(
+                        "List of IDs (`structure_ids`) must have same length as list of structure."
+                    )
 
         else:
-            num_entries = (
-                len(materials) if materials is not None else len(df_featurized)
-            )
-            structure_ids = [f"id{i}" for i in range(num_entries)]
+            if df_featurized is not None:
+                structure_ids = df_featurized.index
+            else:
+                num_entries = (
+                    len(materials) if materials is not None else len(df_featurized)
+                )
+                structure_ids = [f"id{i}" for i in range(num_entries)]
 
         if targets is not None:
             # set up dataframe for targets with columns (id, property_1, ..., property_n)
             self.df_targets = pd.DataFrame(
                 targets, index=structure_ids, columns=target_names
             )
             # set up number of classes
```

### Comparing `modnet-0.4.3/modnet/sklearn.py` & `modnet-0.4.4/modnet/sklearn.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.3/modnet/tests/conftest.py` & `modnet-0.4.4/modnet/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.3/modnet/tests/test_benchmark.py` & `modnet-0.4.4/modnet/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.3/modnet/tests/test_ext_data.py` & `modnet-0.4.4/modnet/tests/test_ext_data.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.3/modnet/tests/test_hyper_opt.py` & `modnet-0.4.4/modnet/tests/test_hyper_opt.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.3/modnet/tests/test_model.py` & `modnet-0.4.4/modnet/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.3/modnet/tests/test_preprocessing.py` & `modnet-0.4.4/modnet/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.3/modnet/tests/test_sklearn.py` & `modnet-0.4.4/modnet/tests/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.3/modnet/utils.py` & `modnet-0.4.4/modnet/utils.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.3/modnet.egg-info/PKG-INFO` & `modnet-0.4.4/modnet.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,125 +1,124 @@
 Metadata-Version: 2.1
 Name: modnet
-Version: 0.4.3
+Version: 0.4.4
 Summary: MODNet, the Material Optimal Descriptor Network for materials properties prediction. 
 Home-page: https://github.com/ppdebreuck/modnet
 Author: Pierre-Paul De Breuck
 Author-email: pierre-paul.debreuck@uclouvain.be
-License: UNKNOWN
 Project-URL: GitHub, https://github.com/ppdebreuck/modnet
 Project-URL: Documentation, https://modnet.readthedocs.io
-Description: <div align="center">
-            <img src="img/modnet_logo.svg" alt="modnet-logo"  width=200>
-            <br>
-        
-        # MODNet: Material Optimal Descriptor Network
-        
-        [![arXiv](https://img.shields.io/badge/arXiv-2004.14766-brightgreen)](https://arxiv.org/abs/2004.14766) [![Build Status](https://img.shields.io/github/actions/workflow/status/ppdebreuck/modnet/ci.yml?logo=github&branch=main)](https://github.com/ppdebreuck/modnet/actions?query=branch%3Amaster+) [![Read the Docs](https://img.shields.io/readthedocs/modnet)](https://modnet.readthedocs.io/en/latest/)
-        
-        </div>
-        
-        <a name="introduction"></a>
-        ## Introduction
-        This repository contains the Python (3.8+) package implementing the Material Optimal Descriptor Network (MODNet).
-        It is a supervised machine learning framework for **learning material properties** from
-        either the **composition** or  **crystal structure**. The framework is well suited for **limited datasets**
-        and can be used for learning *multiple* properties together by using **joint learning**.
-        
-        MODNet appears on the [MatBench leaderboard](https://matbench.materialsproject.org/). As of 11/11/2021, MODNet provides the best performance of all submitted models on 7 out of 13 tasks.
-        
-        This repository also contains two [pretrained models](#pretrained) that can be used for predicting
-        the refractive index and vibrational thermodynamics from any crystal structure.
-        
-        See the MODNet papers and repositories below for more details:
-        
-        - De Breuck *et al.*, "Materials property prediction for limited datasets enabled by feature selection and joint learning with MODNet." *npj Comput Mater* **7**, 83 (2021). [10.1038/s41524-021-00552-2](https://doi.org/10.1038/s41524-021-00552-2) (preprint: [arXiv:2004.14766](https://arxiv.org/abs/2004.14766)).
-        - De Breuck *et al.*, "Robust model benchmarking and bias-imbalance in data-driven materials science: a case study on MODNet." *J. Phys.: Condens. Matter* **33** 404002,  (2021), [10.1088/1361-648X/ac1280](https://doi.org/10.1088/1361-648X/ac1280) (preprint: [arXiv:2102.02263](https://arxiv.org/abs/2102.02263)).
-        - MatBench benchmarking data repository: [modl-uclouvain/modnet-matbench](https://github.com/modl-uclouvain/modnet-matbench).
-        
-        
-        
-        <p align='center'>
-        <img src="img/MODNet_schematic.PNG" alt="MODNet schematic" />
-        </p>
-        <div align='center'>
-        <strong>Figure 1. Schematic representation of the MODNet.</strong>
-        </div>
-        
-        
-        <a name="install"></a>
-        ## How to install
-        
-        First, create a virtual environment (e.g., named modnet) with Python (3.8+) using
-        your favourite environment manager (the following instructions use
-        [conda](https://docs.conda.io/)):
-        
-        ```shell
-        conda create -n modnet python=3.9
-        ```
-        
-        Activate the environment:
-        
-        ```shell
-        conda activate modnet
-        ```
-        
-        Finally, install MODNet from PyPI with `pip`:
-        
-        ```shell
-        pip install modnet
-        ```
-        
-        >**Warning**
-        >We strongly recommend pinning your Python environment when using MODNet
-        >across multiple machines, or multiple MODNet versions, as changes to the
-        >dependencies and sub-dependencies can lead to different values for particular
-        >features.
-        >
-        >This can be achieved with `conda export` or `pip freeze`.
-        
-        For development (or if you wish to use pinned versions of direct dependencies that
-        MODNet has been tested with), you can clone this git repository and make an
-        editable install inside your chosen environment with `pip`:
-        
-        ```shell
-        git clone git@github.com:ppdebreuck/modnet
-        cd modnet
-        conda create -n modnet python=3.9
-        conda activate modnet
-        pip install -r requirements.txt  # optionally use pinned requirements
-        pip install -e .
-        ```
-        
-        
-        <a name="documentation"></a>
-        ## Documentation
-        The documentation is available at [ReadTheDocs](https://modnet.readthedocs.io).
-        
-        <a name="changelog"></a>
-        ## Changelog
-        A brief changelog can be found in the [release summaries on GitHub](https://github.com/ppdebreuck/modnet/releases).
-        
-        <a name="author"></a>
-        ## Author
-        This software was written by [Pierre-Paul De Breuck](mailto:pierre-paul.debreuck@uclouvain.be) and [Matthew Evans](https://www.github.com/ml-evs) with contributions from David Waroquiers and  Gregoire Heymans.
-        For an up-to-date list, see the [Contributors on GitHub](https://github.com/ppdebreuck/modnet/graphs/contributors).
-        
-        <a name="License"></a>
-        ## License
-        
-        MODNet is released under the MIT License.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: bayesian
 Provides-Extra: test
 Provides-Extra: dev
+License-File: LICENSE.md
+
+<div align="center">
+    <img src="img/modnet_logo.svg" alt="modnet-logo"  width=200>
+    <br>
+
+# MODNet: Material Optimal Descriptor Network
+
+[![arXiv](https://img.shields.io/badge/arXiv-2004.14766-brightgreen)](https://arxiv.org/abs/2004.14766) [![Build Status](https://img.shields.io/github/actions/workflow/status/ppdebreuck/modnet/ci.yml?logo=github&branch=main)](https://github.com/ppdebreuck/modnet/actions?query=branch%3Amaster+) [![Read the Docs](https://img.shields.io/readthedocs/modnet)](https://modnet.readthedocs.io/en/latest/)
+
+</div>
+
+<a name="introduction"></a>
+## Introduction
+This repository contains the Python (3.8+) package implementing the Material Optimal Descriptor Network (MODNet).
+It is a supervised machine learning framework for **learning material properties** from
+either the **composition** or  **crystal structure**. The framework is well suited for **limited datasets**
+and can be used for learning *multiple* properties together by using **joint learning**.
+
+MODNet appears on the [MatBench leaderboard](https://matbench.materialsproject.org/). As of 11/11/2021, MODNet provides the best performance of all submitted models on 7 out of 13 tasks.
+
+This repository also contains two [pretrained models](#pretrained) that can be used for predicting
+the refractive index and vibrational thermodynamics from any crystal structure.
+
+See the MODNet papers and repositories below for more details:
+
+- De Breuck *et al.*, "Materials property prediction for limited datasets enabled by feature selection and joint learning with MODNet." *npj Comput Mater* **7**, 83 (2021). [10.1038/s41524-021-00552-2](https://doi.org/10.1038/s41524-021-00552-2) (preprint: [arXiv:2004.14766](https://arxiv.org/abs/2004.14766)).
+- De Breuck *et al.*, "Robust model benchmarking and bias-imbalance in data-driven materials science: a case study on MODNet." *J. Phys.: Condens. Matter* **33** 404002,  (2021), [10.1088/1361-648X/ac1280](https://doi.org/10.1088/1361-648X/ac1280) (preprint: [arXiv:2102.02263](https://arxiv.org/abs/2102.02263)).
+- MatBench benchmarking data repository: [modl-uclouvain/modnet-matbench](https://github.com/modl-uclouvain/modnet-matbench).
+
+
+
+<p align='center'>
+<img src="img/MODNet_schematic.PNG" alt="MODNet schematic" />
+</p>
+<div align='center'>
+<strong>Figure 1. Schematic representation of the MODNet.</strong>
+</div>
+
+
+<a name="install"></a>
+## How to install
+
+First, create a virtual environment (e.g., named modnet) with Python (3.8+) using
+your favourite environment manager (the following instructions use
+[conda](https://docs.conda.io/)):
+
+```shell
+conda create -n modnet python=3.9
+```
+
+Activate the environment:
+
+```shell
+conda activate modnet
+```
+
+Finally, install MODNet from PyPI with `pip`:
+
+```shell
+pip install modnet
+```
+
+>**Warning**
+>We strongly recommend pinning your Python environment when using MODNet
+>across multiple machines, or multiple MODNet versions, as changes to the
+>dependencies and sub-dependencies can lead to different values for particular
+>features.
+>
+>This can be achieved with `conda export` or `pip freeze`.
+
+For development (or if you wish to use pinned versions of direct dependencies that
+MODNet has been tested with), you can clone this git repository and make an
+editable install inside your chosen environment with `pip`:
+
+```shell
+git clone git@github.com:ppdebreuck/modnet
+cd modnet
+conda create -n modnet python=3.9
+conda activate modnet
+pip install -r requirements.txt  # optionally use pinned requirements
+pip install -e .
+```
+
+
+<a name="documentation"></a>
+## Documentation
+The documentation is available at [ReadTheDocs](https://modnet.readthedocs.io).
+
+<a name="changelog"></a>
+## Changelog
+A brief changelog can be found in the [release summaries on GitHub](https://github.com/ppdebreuck/modnet/releases).
+
+<a name="author"></a>
+## Author
+This software was written by [Pierre-Paul De Breuck](mailto:pierre-paul.debreuck@uclouvain.be) and [Matthew Evans](https://www.github.com/ml-evs) with contributions from David Waroquiers and  Gregoire Heymans.
+For an up-to-date list, see the [Contributors on GitHub](https://github.com/ppdebreuck/modnet/graphs/contributors).
+
+<a name="License"></a>
+## License
+
+MODNet is released under the MIT License.
```

### Comparing `modnet-0.4.3/modnet.egg-info/SOURCES.txt` & `modnet-0.4.4/modnet.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 modnet/data/Features_cross
 modnet/featurizers/__init__.py
 modnet/featurizers/featurizers.py
 modnet/featurizers/utils.py
 modnet/featurizers/presets/__init__.py
 modnet/featurizers/presets/debreuck_2020.py
 modnet/featurizers/presets/matminer_2023.py
+modnet/featurizers/presets/matminer_2024_fast.py
 modnet/featurizers/presets/matminer_all_2023.py
 modnet/hyper_opt/__init__.py
 modnet/hyper_opt/fit_genetic.py
 modnet/matbench/__init__.py
 modnet/matbench/benchmark.py
 modnet/model_presets/__init__.py
 modnet/model_presets/presets.py
```

### Comparing `modnet-0.4.3/setup.py` & `modnet-0.4.4/setup.py`

 * *Files identical despite different names*

