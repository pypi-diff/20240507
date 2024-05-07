# Comparing `tmp/gennet_forked-2.0.0.tar.gz` & `tmp/gennet_forked-2.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gennet_forked-2.0.0.tar", last modified: Mon May  6 08:00:48 2024, max compression
+gzip compressed data, was "gennet_forked-2.0.0.1.tar", last modified: Tue May  7 08:10:24 2024, max compression
```

## Comparing `gennet_forked-2.0.0.tar` & `gennet_forked-2.0.0.1.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 08:00:48.355708 gennet_forked-2.0.0/
--rw-r--r--   0 mostafa    (501) staff       (20)    11357 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/LICENSE
--rw-r--r--   0 mostafa    (501) staff       (20)    11847 2024-05-06 08:00:48.355605 gennet_forked-2.0.0/PKG-INFO
--rw-r--r--   0 mostafa    (501) staff       (20)    10722 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/README.md
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 08:00:48.340077 gennet_forked-2.0.0/gennet/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-01 11:22:32.000000 gennet_forked-2.0.0/gennet/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)    13570 2024-05-01 14:01:03.000000 gennet_forked-2.0.0/gennet/cli.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 08:00:48.344225 gennet_forked-2.0.0/gennet/utils/
--rw-r--r--   0 mostafa    (501) staff       (20)    20576 2024-05-01 12:35:35.000000 gennet_forked-2.0.0/gennet/utils/Convert.py
--rw-r--r--   0 mostafa    (501) staff       (20)     1780 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/gennet/utils/Convert_topology_npz.py
--rw-r--r--   0 mostafa    (501) staff       (20)    21944 2024-05-01 12:32:02.000000 gennet_forked-2.0.0/gennet/utils/Create_network.py
--rw-r--r--   0 mostafa    (501) staff       (20)    10411 2024-05-01 12:31:58.000000 gennet_forked-2.0.0/gennet/utils/Create_plots.py
--rw-r--r--   0 mostafa    (501) staff       (20)    11853 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/gennet/utils/Dataloader.py
--rw-r--r--   0 mostafa    (501) staff       (20)    10782 2024-05-01 12:31:51.000000 gennet_forked-2.0.0/gennet/utils/Interpret.py
--rw-r--r--   0 mostafa    (501) staff       (20)    12219 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/gennet/utils/LocallyDirected1D.py
--rw-r--r--   0 mostafa    (501) staff       (20)     9631 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/gennet/utils/LocallyDirected1D_scatter.py
--rw-r--r--   0 mostafa    (501) staff       (20)    18812 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/gennet/utils/LocallyDirectedConnected.py
--rw-r--r--   0 mostafa    (501) staff       (20)     4489 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/gennet/utils/Normalization.py
--rw-r--r--   0 mostafa    (501) staff       (20)     9321 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/gennet/utils/Topology.py
--rw-r--r--   0 mostafa    (501) staff       (20)    15793 2024-05-01 12:31:34.000000 gennet_forked-2.0.0/gennet/utils/Train_network.py
--rw-r--r--   0 mostafa    (501) staff       (20)     9453 2024-05-01 13:00:50.000000 gennet_forked-2.0.0/gennet/utils/Utility_functions.py
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/gennet/utils/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 08:00:48.345085 gennet_forked-2.0.0/gennet/utils/hase/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-01 13:14:16.000000 gennet_forked-2.0.0/gennet/utils/hase/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)      191 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/gennet/utils/hase/config.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 08:00:48.345343 gennet_forked-2.0.0/gennet/utils/hase/hase/
--rw-r--r--   0 mostafa    (501) staff       (20)     3080 2024-05-01 12:45:02.000000 gennet_forked-2.0.0/gennet/utils/hase/hase/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)    25995 2024-05-01 13:24:00.000000 gennet_forked-2.0.0/gennet/utils/hase/hase.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 08:00:48.348190 gennet_forked-2.0.0/gennet/utils/hase/hdgwas/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/gennet/utils/hase/hdgwas/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)    16406 2024-05-01 13:23:44.000000 gennet_forked-2.0.0/gennet/utils/hase/hdgwas/converter.py
--rw-r--r--   0 mostafa    (501) staff       (20)    44037 2024-05-01 12:44:32.000000 gennet_forked-2.0.0/gennet/utils/hase/hdgwas/data.py
--rw-r--r--   0 mostafa    (501) staff       (20)     4786 2024-05-01 13:24:14.000000 gennet_forked-2.0.0/gennet/utils/hase/hdgwas/fake.py
--rw-r--r--   0 mostafa    (501) staff       (20)    12156 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/gennet/utils/hase/hdgwas/hash.py
--rw-r--r--   0 mostafa    (501) staff       (20)     3880 2024-05-01 12:44:40.000000 gennet_forked-2.0.0/gennet/utils/hase/hdgwas/hdregression.py
--rw-r--r--   0 mostafa    (501) staff       (20)     7597 2024-05-01 12:44:44.000000 gennet_forked-2.0.0/gennet/utils/hase/hdgwas/pard.py
--rw-r--r--   0 mostafa    (501) staff       (20)      580 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/gennet/utils/hase/hdgwas/protocol.py
--rw-r--r--   0 mostafa    (501) staff       (20)     3935 2024-05-01 12:44:50.000000 gennet_forked-2.0.0/gennet/utils/hase/hdgwas/regression.py
--rw-r--r--   0 mostafa    (501) staff       (20)    35956 2024-05-01 12:44:54.000000 gennet_forked-2.0.0/gennet/utils/hase/hdgwas/tools.py
--rw-r--r--   0 mostafa    (501) staff       (20)      167 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/gennet/utils/hase/setup.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 08:00:48.351589 gennet_forked-2.0.0/gennet/utils/hase/tools/
--rw-r--r--   0 mostafa    (501) staff       (20)     4594 2024-05-01 13:24:59.000000 gennet_forked-2.0.0/gennet/utils/hase/tools/VCF2hdf5.py
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/gennet/utils/hase/tools/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     3010 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/gennet/utils/hase/tools/addProbesInfo.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2038 2024-05-01 12:43:40.000000 gennet_forked-2.0.0/gennet/utils/hase/tools/analyzer.py
--rw-r--r--   0 mostafa    (501) staff       (20)     1545 2024-05-01 13:25:06.000000 gennet_forked-2.0.0/gennet/utils/hase/tools/fix_pheno_id.py
--rw-r--r--   0 mostafa    (501) staff       (20)      635 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/gennet/utils/hase/tools/generator.py
--rw-r--r--   0 mostafa    (501) staff       (20)     1553 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/gennet/utils/hase/tools/make_hase_phen.py
--rw-r--r--   0 mostafa    (501) staff       (20)    11194 2024-05-01 13:24:45.000000 gennet_forked-2.0.0/gennet/utils/hase/tools/mapper.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2943 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/gennet/utils/hase/tools/merge_genotype.py
--rw-r--r--   0 mostafa    (501) staff       (20)     5720 2024-05-01 13:24:32.000000 gennet_forked-2.0.0/gennet/utils/hase/tools/minimac2hdf5.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2563 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/gennet/utils/hase/tools/rm_subj.py
--rw-r--r--   0 mostafa    (501) staff       (20)      858 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/gennet/utils/hase/tools/tools.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 08:00:48.355112 gennet_forked-2.0.0/gennet_forked.egg-info/
--rw-r--r--   0 mostafa    (501) staff       (20)    11847 2024-05-06 08:00:48.000000 gennet_forked-2.0.0/gennet_forked.egg-info/PKG-INFO
--rw-r--r--   0 mostafa    (501) staff       (20)     2021 2024-05-06 08:00:48.000000 gennet_forked-2.0.0/gennet_forked.egg-info/SOURCES.txt
--rw-r--r--   0 mostafa    (501) staff       (20)        1 2024-05-06 08:00:48.000000 gennet_forked-2.0.0/gennet_forked.egg-info/dependency_links.txt
--rw-r--r--   0 mostafa    (501) staff       (20)       43 2024-05-06 08:00:48.000000 gennet_forked-2.0.0/gennet_forked.egg-info/entry_points.txt
--rw-r--r--   0 mostafa    (501) staff       (20)      414 2024-05-06 08:00:48.000000 gennet_forked-2.0.0/gennet_forked.egg-info/requires.txt
--rw-r--r--   0 mostafa    (501) staff       (20)       22 2024-05-06 08:00:48.000000 gennet_forked-2.0.0/gennet_forked.egg-info/top_level.txt
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 08:00:48.353975 gennet_forked-2.0.0/interpretation/
--rw-r--r--   0 mostafa    (501) staff       (20)     2162 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/interpretation/DFIM.py
--rw-r--r--   0 mostafa    (501) staff       (20)     3530 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/interpretation/Epistasis_AUC.py
--rw-r--r--   0 mostafa    (501) staff       (20)     6069 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/interpretation/NID.py
--rw-r--r--   0 mostafa    (501) staff       (20)     7979 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/interpretation/RLIPP.py
--rw-r--r--   0 mostafa    (501) staff       (20)     5958 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/interpretation/RLIPP2.py
--rw-r--r--   0 mostafa    (501) staff       (20)    14631 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/interpretation/RLIPP_novel_v2.py
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/interpretation/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     4486 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/interpretation/weight_importance.py
--rw-r--r--   0 mostafa    (501) staff       (20)      411 2024-05-03 13:21:58.000000 gennet_forked-2.0.0/requirements_GenNet.txt
--rw-r--r--   0 mostafa    (501) staff       (20)      541 2024-05-06 08:00:48.356034 gennet_forked-2.0.0/setup.cfg
--rw-r--r--   0 mostafa    (501) staff       (20)      230 2024-05-01 12:41:48.000000 gennet_forked-2.0.0/setup.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 08:00:48.354885 gennet_forked-2.0.0/tests/
--rw-r--r--   0 mostafa    (501) staff       (20)     8595 2024-05-01 12:41:55.000000 gennet_forked-2.0.0/tests/test_GenNet.py
--rw-r--r--   0 mostafa    (501) staff       (20)     1056 2024-05-01 12:41:55.000000 gennet_forked-2.0.0/tests/test_conversion.py
--rw-r--r--   0 mostafa    (501) staff       (20)       91 2024-05-01 10:50:18.000000 gennet_forked-2.0.0/tests/test_import.py
--rw-r--r--   0 mostafa    (501) staff       (20)      980 2024-05-01 12:41:55.000000 gennet_forked-2.0.0/tests/test_interpret.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:10:24.820573 gennet_forked-2.0.0.1/
+-rw-r--r--   0 mostafa    (501) staff       (20)    11357 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/LICENSE
+-rw-r--r--   0 mostafa    (501) staff       (20)    16619 2024-05-07 08:10:24.820447 gennet_forked-2.0.0.1/PKG-INFO
+-rw-r--r--   0 mostafa    (501) staff       (20)    10722 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/README.md
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:10:24.801380 gennet_forked-2.0.0.1/gennet/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-01 11:22:32.000000 gennet_forked-2.0.0.1/gennet/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    13570 2024-05-01 14:01:03.000000 gennet_forked-2.0.0.1/gennet/cli.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:10:24.805517 gennet_forked-2.0.0.1/gennet/utils/
+-rw-r--r--   0 mostafa    (501) staff       (20)    20576 2024-05-01 12:35:35.000000 gennet_forked-2.0.0.1/gennet/utils/Convert.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     1780 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/Convert_topology_npz.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    21944 2024-05-01 12:32:02.000000 gennet_forked-2.0.0.1/gennet/utils/Create_network.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    10411 2024-05-01 12:31:58.000000 gennet_forked-2.0.0.1/gennet/utils/Create_plots.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    11853 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/Dataloader.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    10782 2024-05-01 12:31:51.000000 gennet_forked-2.0.0.1/gennet/utils/Interpret.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    12219 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/LocallyDirected1D.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     9631 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/LocallyDirected1D_scatter.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    18812 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/LocallyDirectedConnected.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     4489 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/Normalization.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     9321 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/Topology.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    15793 2024-05-01 12:31:34.000000 gennet_forked-2.0.0.1/gennet/utils/Train_network.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     9453 2024-05-01 13:00:50.000000 gennet_forked-2.0.0.1/gennet/utils/Utility_functions.py
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:10:24.806489 gennet_forked-2.0.0.1/gennet/utils/hase/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-01 13:14:16.000000 gennet_forked-2.0.0.1/gennet/utils/hase/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)      191 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/hase/config.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:10:24.806732 gennet_forked-2.0.0.1/gennet/utils/hase/hase/
+-rw-r--r--   0 mostafa    (501) staff       (20)     3080 2024-05-01 12:45:02.000000 gennet_forked-2.0.0.1/gennet/utils/hase/hase/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    25995 2024-05-01 13:24:00.000000 gennet_forked-2.0.0.1/gennet/utils/hase/hase.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:10:24.809435 gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    16406 2024-05-01 13:23:44.000000 gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/converter.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    44037 2024-05-01 12:44:32.000000 gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/data.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     4786 2024-05-01 13:24:14.000000 gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/fake.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    12156 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/hash.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     3880 2024-05-01 12:44:40.000000 gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/hdregression.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     7597 2024-05-01 12:44:44.000000 gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/pard.py
+-rw-r--r--   0 mostafa    (501) staff       (20)      580 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/protocol.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     3935 2024-05-01 12:44:50.000000 gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/regression.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    35956 2024-05-01 12:44:54.000000 gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/tools.py
+-rw-r--r--   0 mostafa    (501) staff       (20)      167 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/hase/setup.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:10:24.812367 gennet_forked-2.0.0.1/gennet/utils/hase/tools/
+-rw-r--r--   0 mostafa    (501) staff       (20)     4594 2024-05-01 13:24:59.000000 gennet_forked-2.0.0.1/gennet/utils/hase/tools/VCF2hdf5.py
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/hase/tools/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     3010 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/hase/tools/addProbesInfo.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2038 2024-05-01 12:43:40.000000 gennet_forked-2.0.0.1/gennet/utils/hase/tools/analyzer.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     1545 2024-05-01 13:25:06.000000 gennet_forked-2.0.0.1/gennet/utils/hase/tools/fix_pheno_id.py
+-rw-r--r--   0 mostafa    (501) staff       (20)      635 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/hase/tools/generator.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     1553 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/hase/tools/make_hase_phen.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    11194 2024-05-01 13:24:45.000000 gennet_forked-2.0.0.1/gennet/utils/hase/tools/mapper.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2943 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/hase/tools/merge_genotype.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     5720 2024-05-01 13:24:32.000000 gennet_forked-2.0.0.1/gennet/utils/hase/tools/minimac2hdf5.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2563 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/hase/tools/rm_subj.py
+-rw-r--r--   0 mostafa    (501) staff       (20)      858 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/hase/tools/tools.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:10:24.815342 gennet_forked-2.0.0.1/gennet_forked.egg-info/
+-rw-r--r--   0 mostafa    (501) staff       (20)    16619 2024-05-07 08:10:24.000000 gennet_forked-2.0.0.1/gennet_forked.egg-info/PKG-INFO
+-rw-r--r--   0 mostafa    (501) staff       (20)     2038 2024-05-07 08:10:24.000000 gennet_forked-2.0.0.1/gennet_forked.egg-info/SOURCES.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)        1 2024-05-07 08:10:24.000000 gennet_forked-2.0.0.1/gennet_forked.egg-info/dependency_links.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)       43 2024-05-07 08:10:24.000000 gennet_forked-2.0.0.1/gennet_forked.egg-info/entry_points.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)     3051 2024-05-07 08:10:24.000000 gennet_forked-2.0.0.1/gennet_forked.egg-info/requires.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)       22 2024-05-07 08:10:24.000000 gennet_forked-2.0.0.1/gennet_forked.egg-info/top_level.txt
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:10:24.814342 gennet_forked-2.0.0.1/interpretation/
+-rw-r--r--   0 mostafa    (501) staff       (20)     2162 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/interpretation/DFIM.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     3530 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/interpretation/Epistasis_AUC.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     6069 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/interpretation/NID.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     7979 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/interpretation/RLIPP.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     5958 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/interpretation/RLIPP2.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    14631 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/interpretation/RLIPP_novel_v2.py
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/interpretation/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     4486 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/interpretation/weight_importance.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     3051 2024-05-07 08:06:02.000000 gennet_forked-2.0.0.1/requirements.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)      411 2024-05-03 13:21:58.000000 gennet_forked-2.0.0.1/requirements_GenNet.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)      536 2024-05-07 08:10:24.820844 gennet_forked-2.0.0.1/setup.cfg
+-rw-r--r--   0 mostafa    (501) staff       (20)      230 2024-05-01 12:41:48.000000 gennet_forked-2.0.0.1/setup.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:10:24.815029 gennet_forked-2.0.0.1/tests/
+-rw-r--r--   0 mostafa    (501) staff       (20)     8595 2024-05-01 12:41:55.000000 gennet_forked-2.0.0.1/tests/test_GenNet.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     1056 2024-05-01 12:41:55.000000 gennet_forked-2.0.0.1/tests/test_conversion.py
+-rw-r--r--   0 mostafa    (501) staff       (20)       91 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/tests/test_import.py
+-rw-r--r--   0 mostafa    (501) staff       (20)      980 2024-05-01 12:41:55.000000 gennet_forked-2.0.0.1/tests/test_interpret.py
```

### Comparing `gennet_forked-2.0.0/LICENSE` & `gennet_forked-2.0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/PKG-INFO` & `gennet_forked-2.0.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,7 @@
-Metadata-Version: 2.1
-Name: gennet-forked
-Version: 2.0.0
-Summary: Framework for Interpretable Neural Networks
-Home-page: https://github.com/ArnovanHilten/GenNet
-Author: Arno van Hilten
-Author-email: arnovanhilten@gmail.com
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: h5py>=2.10.0
-Requires-Dist: joblib>=0.16.0
-Requires-Dist: Markdown>=3.2.1
-Requires-Dist: matplotlib>=3.3.2
-Requires-Dist: jupyter>=1.0.0
-Requires-Dist: numpy>=1.21
-Requires-Dist: pandas>=0.25.3
-Requires-Dist: Pillow>=7.2.0
-Requires-Dist: plotly>=4.12.0
-Requires-Dist: pyparsing>=2.4.7
-Requires-Dist: scikit-learn>=0.23.2
-Requires-Dist: scipy>=1.4.1
-Requires-Dist: seaborn>=0.10.1
-Requires-Dist: scikit-learn>=0.0
-Requires-Dist: tables>=3.6.1
-Requires-Dist: tqdm>=4.49.0
-Requires-Dist: zipp>=3.1.0
-Requires-Dist: pytest>=6.2.5
-Requires-Dist: protobuf>=3.20.3
-Requires-Dist: statsmodels
-Requires-Dist: shap
-Requires-Dist: path_explain
-Requires-Dist: psutil
-Requires-Dist: kaleido
-Requires-Dist: tensorflow==2.15.1
-Requires-Dist: tensorflow-metal==1.1.0; sys_platform == "darwin"
-Requires-Dist: bitarray
-
 [![DOI](https://zenodo.org/badge/240289809.svg)](https://zenodo.org/badge/latestdoi/240289809)
 ![Build](https://github.com/ArnovanHilten/GenNet/actions/workflows/tests.yml/badge.svg)
 
 # **GenNet**
 **Framework for Interpretable Neural Networks for Genetics**
 
 1. [What is GenNet?](https://github.com/ArnovanHilten/GenNet/#1-what-is-gennet)
```

### Comparing `gennet_forked-2.0.0/gennet/cli.py` & `gennet_forked-2.0.0.1/gennet/cli.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/Convert.py` & `gennet_forked-2.0.0.1/gennet/utils/Convert.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/Convert_topology_npz.py` & `gennet_forked-2.0.0.1/gennet/utils/Convert_topology_npz.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/Create_network.py` & `gennet_forked-2.0.0.1/gennet/utils/Create_network.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/Create_plots.py` & `gennet_forked-2.0.0.1/gennet/utils/Create_plots.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/Dataloader.py` & `gennet_forked-2.0.0.1/gennet/utils/Dataloader.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/Interpret.py` & `gennet_forked-2.0.0.1/gennet/utils/Interpret.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/LocallyDirected1D.py` & `gennet_forked-2.0.0.1/gennet/utils/LocallyDirected1D.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/LocallyDirected1D_scatter.py` & `gennet_forked-2.0.0.1/gennet/utils/LocallyDirected1D_scatter.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/LocallyDirectedConnected.py` & `gennet_forked-2.0.0.1/gennet/utils/LocallyDirectedConnected.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/Normalization.py` & `gennet_forked-2.0.0.1/gennet/utils/Normalization.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/Topology.py` & `gennet_forked-2.0.0.1/gennet/utils/Topology.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/Train_network.py` & `gennet_forked-2.0.0.1/gennet/utils/Train_network.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/Utility_functions.py` & `gennet_forked-2.0.0.1/gennet/utils/Utility_functions.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/hase/hase/__init__.py` & `gennet_forked-2.0.0.1/gennet/utils/hase/hase/__init__.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/hase/hase.py` & `gennet_forked-2.0.0.1/gennet/utils/hase/hase.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/hase/hdgwas/converter.py` & `gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/converter.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/hase/hdgwas/data.py` & `gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/data.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/hase/hdgwas/fake.py` & `gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/fake.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/hase/hdgwas/hash.py` & `gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/hash.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/hase/hdgwas/hdregression.py` & `gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/hdregression.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/hase/hdgwas/pard.py` & `gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/pard.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/hase/hdgwas/protocol.py` & `gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/protocol.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/hase/hdgwas/regression.py` & `gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/regression.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/hase/hdgwas/tools.py` & `gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/tools.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/hase/tools/VCF2hdf5.py` & `gennet_forked-2.0.0.1/gennet/utils/hase/tools/VCF2hdf5.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/hase/tools/addProbesInfo.py` & `gennet_forked-2.0.0.1/gennet/utils/hase/tools/addProbesInfo.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/hase/tools/analyzer.py` & `gennet_forked-2.0.0.1/gennet/utils/hase/tools/analyzer.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/hase/tools/fix_pheno_id.py` & `gennet_forked-2.0.0.1/gennet/utils/hase/tools/fix_pheno_id.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/hase/tools/generator.py` & `gennet_forked-2.0.0.1/gennet/utils/hase/tools/generator.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/hase/tools/make_hase_phen.py` & `gennet_forked-2.0.0.1/gennet/utils/hase/tools/make_hase_phen.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/hase/tools/mapper.py` & `gennet_forked-2.0.0.1/gennet/utils/hase/tools/mapper.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/hase/tools/merge_genotype.py` & `gennet_forked-2.0.0.1/gennet/utils/hase/tools/merge_genotype.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/hase/tools/minimac2hdf5.py` & `gennet_forked-2.0.0.1/gennet/utils/hase/tools/minimac2hdf5.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/hase/tools/rm_subj.py` & `gennet_forked-2.0.0.1/gennet/utils/hase/tools/rm_subj.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet/utils/hase/tools/tools.py` & `gennet_forked-2.0.0.1/gennet/utils/hase/tools/tools.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/gennet_forked.egg-info/SOURCES.txt` & `gennet_forked-2.0.0.1/gennet_forked.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+requirements.txt
 requirements_GenNet.txt
 setup.cfg
 setup.py
 gennet/__init__.py
 gennet/cli.py
 gennet/utils/Convert.py
 gennet/utils/Convert_topology_npz.py
```

### Comparing `gennet_forked-2.0.0/interpretation/DFIM.py` & `gennet_forked-2.0.0.1/interpretation/DFIM.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/interpretation/Epistasis_AUC.py` & `gennet_forked-2.0.0.1/interpretation/Epistasis_AUC.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/interpretation/NID.py` & `gennet_forked-2.0.0.1/interpretation/NID.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/interpretation/RLIPP.py` & `gennet_forked-2.0.0.1/interpretation/RLIPP.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/interpretation/RLIPP2.py` & `gennet_forked-2.0.0.1/interpretation/RLIPP2.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/interpretation/RLIPP_novel_v2.py` & `gennet_forked-2.0.0.1/interpretation/RLIPP_novel_v2.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/interpretation/weight_importance.py` & `gennet_forked-2.0.0.1/interpretation/weight_importance.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/setup.cfg` & `gennet_forked-2.0.0.1/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [metadata]
 name = gennet-forked
-version = 2.0.0
+version = 2.0.0.1
 author = Arno van Hilten
 author_email = arnovanhilten@gmail.com
 description = Framework for Interpretable Neural Networks
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = LICENSE
 url = https://github.com/ArnovanHilten/GenNet
 
 [options]
 python_requires = >= 3.8
-install_requires = file: requirements_GenNet.txt
+install_requires = file: requirements.txt
 
 [options.entry_points]
 console_scripts = 
 	gennet=gennet.cli:main
 
 [bdist_wheel]
 universal = 1
```

### Comparing `gennet_forked-2.0.0/tests/test_GenNet.py` & `gennet_forked-2.0.0.1/tests/test_GenNet.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/tests/test_conversion.py` & `gennet_forked-2.0.0.1/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0/tests/test_interpret.py` & `gennet_forked-2.0.0.1/tests/test_interpret.py`

 * *Files identical despite different names*

