# Comparing `tmp/gennet_forked-2.0.0.1.tar.gz` & `tmp/gennet_forked-2.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gennet_forked-2.0.0.1.tar", last modified: Tue May  7 08:10:24 2024, max compression
+gzip compressed data, was "gennet_forked-2.0.0.2.tar", last modified: Tue May  7 08:18:14 2024, max compression
```

## Comparing `gennet_forked-2.0.0.1.tar` & `gennet_forked-2.0.0.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:10:24.820573 gennet_forked-2.0.0.1/
--rw-r--r--   0 mostafa    (501) staff       (20)    11357 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/LICENSE
--rw-r--r--   0 mostafa    (501) staff       (20)    16619 2024-05-07 08:10:24.820447 gennet_forked-2.0.0.1/PKG-INFO
--rw-r--r--   0 mostafa    (501) staff       (20)    10722 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/README.md
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:10:24.801380 gennet_forked-2.0.0.1/gennet/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-01 11:22:32.000000 gennet_forked-2.0.0.1/gennet/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)    13570 2024-05-01 14:01:03.000000 gennet_forked-2.0.0.1/gennet/cli.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:10:24.805517 gennet_forked-2.0.0.1/gennet/utils/
--rw-r--r--   0 mostafa    (501) staff       (20)    20576 2024-05-01 12:35:35.000000 gennet_forked-2.0.0.1/gennet/utils/Convert.py
--rw-r--r--   0 mostafa    (501) staff       (20)     1780 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/Convert_topology_npz.py
--rw-r--r--   0 mostafa    (501) staff       (20)    21944 2024-05-01 12:32:02.000000 gennet_forked-2.0.0.1/gennet/utils/Create_network.py
--rw-r--r--   0 mostafa    (501) staff       (20)    10411 2024-05-01 12:31:58.000000 gennet_forked-2.0.0.1/gennet/utils/Create_plots.py
--rw-r--r--   0 mostafa    (501) staff       (20)    11853 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/Dataloader.py
--rw-r--r--   0 mostafa    (501) staff       (20)    10782 2024-05-01 12:31:51.000000 gennet_forked-2.0.0.1/gennet/utils/Interpret.py
--rw-r--r--   0 mostafa    (501) staff       (20)    12219 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/LocallyDirected1D.py
--rw-r--r--   0 mostafa    (501) staff       (20)     9631 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/LocallyDirected1D_scatter.py
--rw-r--r--   0 mostafa    (501) staff       (20)    18812 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/LocallyDirectedConnected.py
--rw-r--r--   0 mostafa    (501) staff       (20)     4489 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/Normalization.py
--rw-r--r--   0 mostafa    (501) staff       (20)     9321 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/Topology.py
--rw-r--r--   0 mostafa    (501) staff       (20)    15793 2024-05-01 12:31:34.000000 gennet_forked-2.0.0.1/gennet/utils/Train_network.py
--rw-r--r--   0 mostafa    (501) staff       (20)     9453 2024-05-01 13:00:50.000000 gennet_forked-2.0.0.1/gennet/utils/Utility_functions.py
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:10:24.806489 gennet_forked-2.0.0.1/gennet/utils/hase/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-01 13:14:16.000000 gennet_forked-2.0.0.1/gennet/utils/hase/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)      191 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/hase/config.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:10:24.806732 gennet_forked-2.0.0.1/gennet/utils/hase/hase/
--rw-r--r--   0 mostafa    (501) staff       (20)     3080 2024-05-01 12:45:02.000000 gennet_forked-2.0.0.1/gennet/utils/hase/hase/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)    25995 2024-05-01 13:24:00.000000 gennet_forked-2.0.0.1/gennet/utils/hase/hase.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:10:24.809435 gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)    16406 2024-05-01 13:23:44.000000 gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/converter.py
--rw-r--r--   0 mostafa    (501) staff       (20)    44037 2024-05-01 12:44:32.000000 gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/data.py
--rw-r--r--   0 mostafa    (501) staff       (20)     4786 2024-05-01 13:24:14.000000 gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/fake.py
--rw-r--r--   0 mostafa    (501) staff       (20)    12156 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/hash.py
--rw-r--r--   0 mostafa    (501) staff       (20)     3880 2024-05-01 12:44:40.000000 gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/hdregression.py
--rw-r--r--   0 mostafa    (501) staff       (20)     7597 2024-05-01 12:44:44.000000 gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/pard.py
--rw-r--r--   0 mostafa    (501) staff       (20)      580 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/protocol.py
--rw-r--r--   0 mostafa    (501) staff       (20)     3935 2024-05-01 12:44:50.000000 gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/regression.py
--rw-r--r--   0 mostafa    (501) staff       (20)    35956 2024-05-01 12:44:54.000000 gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/tools.py
--rw-r--r--   0 mostafa    (501) staff       (20)      167 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/hase/setup.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:10:24.812367 gennet_forked-2.0.0.1/gennet/utils/hase/tools/
--rw-r--r--   0 mostafa    (501) staff       (20)     4594 2024-05-01 13:24:59.000000 gennet_forked-2.0.0.1/gennet/utils/hase/tools/VCF2hdf5.py
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/hase/tools/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     3010 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/hase/tools/addProbesInfo.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2038 2024-05-01 12:43:40.000000 gennet_forked-2.0.0.1/gennet/utils/hase/tools/analyzer.py
--rw-r--r--   0 mostafa    (501) staff       (20)     1545 2024-05-01 13:25:06.000000 gennet_forked-2.0.0.1/gennet/utils/hase/tools/fix_pheno_id.py
--rw-r--r--   0 mostafa    (501) staff       (20)      635 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/hase/tools/generator.py
--rw-r--r--   0 mostafa    (501) staff       (20)     1553 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/hase/tools/make_hase_phen.py
--rw-r--r--   0 mostafa    (501) staff       (20)    11194 2024-05-01 13:24:45.000000 gennet_forked-2.0.0.1/gennet/utils/hase/tools/mapper.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2943 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/hase/tools/merge_genotype.py
--rw-r--r--   0 mostafa    (501) staff       (20)     5720 2024-05-01 13:24:32.000000 gennet_forked-2.0.0.1/gennet/utils/hase/tools/minimac2hdf5.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2563 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/hase/tools/rm_subj.py
--rw-r--r--   0 mostafa    (501) staff       (20)      858 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/gennet/utils/hase/tools/tools.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:10:24.815342 gennet_forked-2.0.0.1/gennet_forked.egg-info/
--rw-r--r--   0 mostafa    (501) staff       (20)    16619 2024-05-07 08:10:24.000000 gennet_forked-2.0.0.1/gennet_forked.egg-info/PKG-INFO
--rw-r--r--   0 mostafa    (501) staff       (20)     2038 2024-05-07 08:10:24.000000 gennet_forked-2.0.0.1/gennet_forked.egg-info/SOURCES.txt
--rw-r--r--   0 mostafa    (501) staff       (20)        1 2024-05-07 08:10:24.000000 gennet_forked-2.0.0.1/gennet_forked.egg-info/dependency_links.txt
--rw-r--r--   0 mostafa    (501) staff       (20)       43 2024-05-07 08:10:24.000000 gennet_forked-2.0.0.1/gennet_forked.egg-info/entry_points.txt
--rw-r--r--   0 mostafa    (501) staff       (20)     3051 2024-05-07 08:10:24.000000 gennet_forked-2.0.0.1/gennet_forked.egg-info/requires.txt
--rw-r--r--   0 mostafa    (501) staff       (20)       22 2024-05-07 08:10:24.000000 gennet_forked-2.0.0.1/gennet_forked.egg-info/top_level.txt
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:10:24.814342 gennet_forked-2.0.0.1/interpretation/
--rw-r--r--   0 mostafa    (501) staff       (20)     2162 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/interpretation/DFIM.py
--rw-r--r--   0 mostafa    (501) staff       (20)     3530 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/interpretation/Epistasis_AUC.py
--rw-r--r--   0 mostafa    (501) staff       (20)     6069 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/interpretation/NID.py
--rw-r--r--   0 mostafa    (501) staff       (20)     7979 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/interpretation/RLIPP.py
--rw-r--r--   0 mostafa    (501) staff       (20)     5958 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/interpretation/RLIPP2.py
--rw-r--r--   0 mostafa    (501) staff       (20)    14631 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/interpretation/RLIPP_novel_v2.py
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/interpretation/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     4486 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/interpretation/weight_importance.py
--rw-r--r--   0 mostafa    (501) staff       (20)     3051 2024-05-07 08:06:02.000000 gennet_forked-2.0.0.1/requirements.txt
--rw-r--r--   0 mostafa    (501) staff       (20)      411 2024-05-03 13:21:58.000000 gennet_forked-2.0.0.1/requirements_GenNet.txt
--rw-r--r--   0 mostafa    (501) staff       (20)      536 2024-05-07 08:10:24.820844 gennet_forked-2.0.0.1/setup.cfg
--rw-r--r--   0 mostafa    (501) staff       (20)      230 2024-05-01 12:41:48.000000 gennet_forked-2.0.0.1/setup.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:10:24.815029 gennet_forked-2.0.0.1/tests/
--rw-r--r--   0 mostafa    (501) staff       (20)     8595 2024-05-01 12:41:55.000000 gennet_forked-2.0.0.1/tests/test_GenNet.py
--rw-r--r--   0 mostafa    (501) staff       (20)     1056 2024-05-01 12:41:55.000000 gennet_forked-2.0.0.1/tests/test_conversion.py
--rw-r--r--   0 mostafa    (501) staff       (20)       91 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.1/tests/test_import.py
--rw-r--r--   0 mostafa    (501) staff       (20)      980 2024-05-01 12:41:55.000000 gennet_forked-2.0.0.1/tests/test_interpret.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:18:14.769891 gennet_forked-2.0.0.2/
+-rw-r--r--   0 mostafa    (501) staff       (20)    11357 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/LICENSE
+-rw-r--r--   0 mostafa    (501) staff       (20)    16645 2024-05-07 08:18:14.769776 gennet_forked-2.0.0.2/PKG-INFO
+-rw-r--r--   0 mostafa    (501) staff       (20)    10722 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/README.md
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:18:14.755725 gennet_forked-2.0.0.2/gennet/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-01 11:22:32.000000 gennet_forked-2.0.0.2/gennet/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    13570 2024-05-01 14:01:03.000000 gennet_forked-2.0.0.2/gennet/cli.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:18:14.757759 gennet_forked-2.0.0.2/gennet/utils/
+-rw-r--r--   0 mostafa    (501) staff       (20)    20576 2024-05-01 12:35:35.000000 gennet_forked-2.0.0.2/gennet/utils/Convert.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     1780 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/gennet/utils/Convert_topology_npz.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    21944 2024-05-01 12:32:02.000000 gennet_forked-2.0.0.2/gennet/utils/Create_network.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    10411 2024-05-01 12:31:58.000000 gennet_forked-2.0.0.2/gennet/utils/Create_plots.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    11853 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/gennet/utils/Dataloader.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    10782 2024-05-01 12:31:51.000000 gennet_forked-2.0.0.2/gennet/utils/Interpret.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    12219 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/gennet/utils/LocallyDirected1D.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     9631 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/gennet/utils/LocallyDirected1D_scatter.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    18812 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/gennet/utils/LocallyDirectedConnected.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     4489 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/gennet/utils/Normalization.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     9321 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/gennet/utils/Topology.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    15793 2024-05-01 12:31:34.000000 gennet_forked-2.0.0.2/gennet/utils/Train_network.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     9453 2024-05-01 13:00:50.000000 gennet_forked-2.0.0.2/gennet/utils/Utility_functions.py
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/gennet/utils/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:18:14.758290 gennet_forked-2.0.0.2/gennet/utils/hase/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-01 13:14:16.000000 gennet_forked-2.0.0.2/gennet/utils/hase/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)      191 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/gennet/utils/hase/config.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:18:14.758437 gennet_forked-2.0.0.2/gennet/utils/hase/hase/
+-rw-r--r--   0 mostafa    (501) staff       (20)     3080 2024-05-01 12:45:02.000000 gennet_forked-2.0.0.2/gennet/utils/hase/hase/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    25995 2024-05-01 13:24:00.000000 gennet_forked-2.0.0.2/gennet/utils/hase/hase.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:18:14.760025 gennet_forked-2.0.0.2/gennet/utils/hase/hdgwas/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/gennet/utils/hase/hdgwas/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    16406 2024-05-01 13:23:44.000000 gennet_forked-2.0.0.2/gennet/utils/hase/hdgwas/converter.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    44037 2024-05-01 12:44:32.000000 gennet_forked-2.0.0.2/gennet/utils/hase/hdgwas/data.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     4786 2024-05-01 13:24:14.000000 gennet_forked-2.0.0.2/gennet/utils/hase/hdgwas/fake.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    12156 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/gennet/utils/hase/hdgwas/hash.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     3880 2024-05-01 12:44:40.000000 gennet_forked-2.0.0.2/gennet/utils/hase/hdgwas/hdregression.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     7597 2024-05-01 12:44:44.000000 gennet_forked-2.0.0.2/gennet/utils/hase/hdgwas/pard.py
+-rw-r--r--   0 mostafa    (501) staff       (20)      580 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/gennet/utils/hase/hdgwas/protocol.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     3935 2024-05-01 12:44:50.000000 gennet_forked-2.0.0.2/gennet/utils/hase/hdgwas/regression.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    35956 2024-05-01 12:44:54.000000 gennet_forked-2.0.0.2/gennet/utils/hase/hdgwas/tools.py
+-rw-r--r--   0 mostafa    (501) staff       (20)      167 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/gennet/utils/hase/setup.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:18:14.761821 gennet_forked-2.0.0.2/gennet/utils/hase/tools/
+-rw-r--r--   0 mostafa    (501) staff       (20)     4594 2024-05-01 13:24:59.000000 gennet_forked-2.0.0.2/gennet/utils/hase/tools/VCF2hdf5.py
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/gennet/utils/hase/tools/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     3010 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/gennet/utils/hase/tools/addProbesInfo.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2038 2024-05-01 12:43:40.000000 gennet_forked-2.0.0.2/gennet/utils/hase/tools/analyzer.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     1545 2024-05-01 13:25:06.000000 gennet_forked-2.0.0.2/gennet/utils/hase/tools/fix_pheno_id.py
+-rw-r--r--   0 mostafa    (501) staff       (20)      635 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/gennet/utils/hase/tools/generator.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     1553 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/gennet/utils/hase/tools/make_hase_phen.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    11194 2024-05-01 13:24:45.000000 gennet_forked-2.0.0.2/gennet/utils/hase/tools/mapper.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2943 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/gennet/utils/hase/tools/merge_genotype.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     5720 2024-05-01 13:24:32.000000 gennet_forked-2.0.0.2/gennet/utils/hase/tools/minimac2hdf5.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2563 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/gennet/utils/hase/tools/rm_subj.py
+-rw-r--r--   0 mostafa    (501) staff       (20)      858 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/gennet/utils/hase/tools/tools.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:18:14.764650 gennet_forked-2.0.0.2/gennet_forked.egg-info/
+-rw-r--r--   0 mostafa    (501) staff       (20)    16645 2024-05-07 08:18:14.000000 gennet_forked-2.0.0.2/gennet_forked.egg-info/PKG-INFO
+-rw-r--r--   0 mostafa    (501) staff       (20)     2038 2024-05-07 08:18:14.000000 gennet_forked-2.0.0.2/gennet_forked.egg-info/SOURCES.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)        1 2024-05-07 08:18:14.000000 gennet_forked-2.0.0.2/gennet_forked.egg-info/dependency_links.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)       43 2024-05-07 08:18:14.000000 gennet_forked-2.0.0.2/gennet_forked.egg-info/entry_points.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)     3080 2024-05-07 08:18:14.000000 gennet_forked-2.0.0.2/gennet_forked.egg-info/requires.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)       22 2024-05-07 08:18:14.000000 gennet_forked-2.0.0.2/gennet_forked.egg-info/top_level.txt
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:18:14.763928 gennet_forked-2.0.0.2/interpretation/
+-rw-r--r--   0 mostafa    (501) staff       (20)     2162 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/interpretation/DFIM.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     3530 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/interpretation/Epistasis_AUC.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     6069 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/interpretation/NID.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     7979 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/interpretation/RLIPP.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     5958 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/interpretation/RLIPP2.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    14631 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/interpretation/RLIPP_novel_v2.py
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/interpretation/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     4486 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/interpretation/weight_importance.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     3077 2024-05-07 08:17:24.000000 gennet_forked-2.0.0.2/requirements.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)      411 2024-05-03 13:21:58.000000 gennet_forked-2.0.0.2/requirements_GenNet.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)      536 2024-05-07 08:18:14.770142 gennet_forked-2.0.0.2/setup.cfg
+-rw-r--r--   0 mostafa    (501) staff       (20)      230 2024-05-01 12:41:48.000000 gennet_forked-2.0.0.2/setup.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 08:18:14.764439 gennet_forked-2.0.0.2/tests/
+-rw-r--r--   0 mostafa    (501) staff       (20)     8595 2024-05-01 12:41:55.000000 gennet_forked-2.0.0.2/tests/test_GenNet.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     1056 2024-05-01 12:41:55.000000 gennet_forked-2.0.0.2/tests/test_conversion.py
+-rw-r--r--   0 mostafa    (501) staff       (20)       91 2024-05-01 10:50:18.000000 gennet_forked-2.0.0.2/tests/test_import.py
+-rw-r--r--   0 mostafa    (501) staff       (20)      980 2024-05-01 12:41:55.000000 gennet_forked-2.0.0.2/tests/test_interpret.py
```

### Comparing `gennet_forked-2.0.0.1/LICENSE` & `gennet_forked-2.0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/PKG-INFO` & `gennet_forked-2.0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gennet-forked
-Version: 2.0.0.1
+Version: 2.0.0.2
 Summary: Framework for Interpretable Neural Networks
 Home-page: https://github.com/ArnovanHilten/GenNet
 Author: Arno van Hilten
 Author-email: arnovanhilten@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -151,15 +151,15 @@
 Requires-Dist: tables==3.9.2
 Requires-Dist: tenacity==8.2.3
 Requires-Dist: tensorboard==2.15.2
 Requires-Dist: tensorboard-data-server==0.7.2
 Requires-Dist: tensorflow==2.15.1
 Requires-Dist: tensorflow-estimator==2.15.0
 Requires-Dist: tensorflow-io-gcs-filesystem==0.37.0
-Requires-Dist: tensorflow-metal==1.1.0
+Requires-Dist: tensorflow-metal==1.1.0; sys_platform == "darwin"
 Requires-Dist: termcolor==2.4.0
 Requires-Dist: terminado==0.18.1
 Requires-Dist: threadpoolctl==3.5.0
 Requires-Dist: tinycss2==1.3.0
 Requires-Dist: tomli==2.0.1
 Requires-Dist: tornado==6.4
 Requires-Dist: tqdm==4.66.4
```

### Comparing `gennet_forked-2.0.0.1/README.md` & `gennet_forked-2.0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/cli.py` & `gennet_forked-2.0.0.2/gennet/cli.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/Convert.py` & `gennet_forked-2.0.0.2/gennet/utils/Convert.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/Convert_topology_npz.py` & `gennet_forked-2.0.0.2/gennet/utils/Convert_topology_npz.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/Create_network.py` & `gennet_forked-2.0.0.2/gennet/utils/Create_network.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/Create_plots.py` & `gennet_forked-2.0.0.2/gennet/utils/Create_plots.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/Dataloader.py` & `gennet_forked-2.0.0.2/gennet/utils/Dataloader.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/Interpret.py` & `gennet_forked-2.0.0.2/gennet/utils/Interpret.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/LocallyDirected1D.py` & `gennet_forked-2.0.0.2/gennet/utils/LocallyDirected1D.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/LocallyDirected1D_scatter.py` & `gennet_forked-2.0.0.2/gennet/utils/LocallyDirected1D_scatter.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/LocallyDirectedConnected.py` & `gennet_forked-2.0.0.2/gennet/utils/LocallyDirectedConnected.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/Normalization.py` & `gennet_forked-2.0.0.2/gennet/utils/Normalization.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/Topology.py` & `gennet_forked-2.0.0.2/gennet/utils/Topology.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/Train_network.py` & `gennet_forked-2.0.0.2/gennet/utils/Train_network.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/Utility_functions.py` & `gennet_forked-2.0.0.2/gennet/utils/Utility_functions.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/hase/hase/__init__.py` & `gennet_forked-2.0.0.2/gennet/utils/hase/hase/__init__.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/hase/hase.py` & `gennet_forked-2.0.0.2/gennet/utils/hase/hase.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/converter.py` & `gennet_forked-2.0.0.2/gennet/utils/hase/hdgwas/converter.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/data.py` & `gennet_forked-2.0.0.2/gennet/utils/hase/hdgwas/data.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/fake.py` & `gennet_forked-2.0.0.2/gennet/utils/hase/hdgwas/fake.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/hash.py` & `gennet_forked-2.0.0.2/gennet/utils/hase/hdgwas/hash.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/hdregression.py` & `gennet_forked-2.0.0.2/gennet/utils/hase/hdgwas/hdregression.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/pard.py` & `gennet_forked-2.0.0.2/gennet/utils/hase/hdgwas/pard.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/protocol.py` & `gennet_forked-2.0.0.2/gennet/utils/hase/hdgwas/protocol.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/regression.py` & `gennet_forked-2.0.0.2/gennet/utils/hase/hdgwas/regression.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/hase/hdgwas/tools.py` & `gennet_forked-2.0.0.2/gennet/utils/hase/hdgwas/tools.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/hase/tools/VCF2hdf5.py` & `gennet_forked-2.0.0.2/gennet/utils/hase/tools/VCF2hdf5.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/hase/tools/addProbesInfo.py` & `gennet_forked-2.0.0.2/gennet/utils/hase/tools/addProbesInfo.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/hase/tools/analyzer.py` & `gennet_forked-2.0.0.2/gennet/utils/hase/tools/analyzer.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/hase/tools/fix_pheno_id.py` & `gennet_forked-2.0.0.2/gennet/utils/hase/tools/fix_pheno_id.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/hase/tools/generator.py` & `gennet_forked-2.0.0.2/gennet/utils/hase/tools/generator.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/hase/tools/make_hase_phen.py` & `gennet_forked-2.0.0.2/gennet/utils/hase/tools/make_hase_phen.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/hase/tools/mapper.py` & `gennet_forked-2.0.0.2/gennet/utils/hase/tools/mapper.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/hase/tools/merge_genotype.py` & `gennet_forked-2.0.0.2/gennet/utils/hase/tools/merge_genotype.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/hase/tools/minimac2hdf5.py` & `gennet_forked-2.0.0.2/gennet/utils/hase/tools/minimac2hdf5.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/hase/tools/rm_subj.py` & `gennet_forked-2.0.0.2/gennet/utils/hase/tools/rm_subj.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet/utils/hase/tools/tools.py` & `gennet_forked-2.0.0.2/gennet/utils/hase/tools/tools.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet_forked.egg-info/PKG-INFO` & `gennet_forked-2.0.0.2/gennet_forked.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gennet-forked
-Version: 2.0.0.1
+Version: 2.0.0.2
 Summary: Framework for Interpretable Neural Networks
 Home-page: https://github.com/ArnovanHilten/GenNet
 Author: Arno van Hilten
 Author-email: arnovanhilten@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -151,15 +151,15 @@
 Requires-Dist: tables==3.9.2
 Requires-Dist: tenacity==8.2.3
 Requires-Dist: tensorboard==2.15.2
 Requires-Dist: tensorboard-data-server==0.7.2
 Requires-Dist: tensorflow==2.15.1
 Requires-Dist: tensorflow-estimator==2.15.0
 Requires-Dist: tensorflow-io-gcs-filesystem==0.37.0
-Requires-Dist: tensorflow-metal==1.1.0
+Requires-Dist: tensorflow-metal==1.1.0; sys_platform == "darwin"
 Requires-Dist: termcolor==2.4.0
 Requires-Dist: terminado==0.18.1
 Requires-Dist: threadpoolctl==3.5.0
 Requires-Dist: tinycss2==1.3.0
 Requires-Dist: tomli==2.0.1
 Requires-Dist: tornado==6.4
 Requires-Dist: tqdm==4.66.4
```

### Comparing `gennet_forked-2.0.0.1/gennet_forked.egg-info/SOURCES.txt` & `gennet_forked-2.0.0.2/gennet_forked.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/gennet_forked.egg-info/requires.txt` & `gennet_forked-2.0.0.2/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 tables==3.9.2
 tenacity==8.2.3
 tensorboard==2.15.2
 tensorboard-data-server==0.7.2
 tensorflow==2.15.1
 tensorflow-estimator==2.15.0
 tensorflow-io-gcs-filesystem==0.37.0
-tensorflow-metal==1.1.0
+tensorflow-metal==1.1.0; sys_platform == 'darwin'
 termcolor==2.4.0
 terminado==0.18.1
 threadpoolctl==3.5.0
 tinycss2==1.3.0
 tomli==2.0.1
 tornado==6.4
 tqdm==4.66.4
```

### Comparing `gennet_forked-2.0.0.1/interpretation/DFIM.py` & `gennet_forked-2.0.0.2/interpretation/DFIM.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/interpretation/Epistasis_AUC.py` & `gennet_forked-2.0.0.2/interpretation/Epistasis_AUC.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/interpretation/NID.py` & `gennet_forked-2.0.0.2/interpretation/NID.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/interpretation/RLIPP.py` & `gennet_forked-2.0.0.2/interpretation/RLIPP.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/interpretation/RLIPP2.py` & `gennet_forked-2.0.0.2/interpretation/RLIPP2.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/interpretation/RLIPP_novel_v2.py` & `gennet_forked-2.0.0.2/interpretation/RLIPP_novel_v2.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/interpretation/weight_importance.py` & `gennet_forked-2.0.0.2/interpretation/weight_importance.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/requirements.txt` & `gennet_forked-2.0.0.2/gennet_forked.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,14 @@
 tables==3.9.2
 tenacity==8.2.3
 tensorboard==2.15.2
 tensorboard-data-server==0.7.2
 tensorflow==2.15.1
 tensorflow-estimator==2.15.0
 tensorflow-io-gcs-filesystem==0.37.0
-tensorflow-metal==1.1.0
 termcolor==2.4.0
 terminado==0.18.1
 threadpoolctl==3.5.0
 tinycss2==1.3.0
 tomli==2.0.1
 tornado==6.4
 tqdm==4.66.4
@@ -163,7 +162,10 @@
 webcolors==1.13
 webencodings==0.5.1
 websocket-client==1.8.0
 Werkzeug==3.0.3
 widgetsnbextension==4.0.10
 wrapt==1.14.1
 zipp==3.18.1
+
+[:sys_platform == "darwin"]
+tensorflow-metal==1.1.0
```

### Comparing `gennet_forked-2.0.0.1/setup.cfg` & `gennet_forked-2.0.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gennet-forked
-version = 2.0.0.1
+version = 2.0.0.2
 author = Arno van Hilten
 author_email = arnovanhilten@gmail.com
 description = Framework for Interpretable Neural Networks
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = LICENSE
 url = https://github.com/ArnovanHilten/GenNet
```

### Comparing `gennet_forked-2.0.0.1/tests/test_GenNet.py` & `gennet_forked-2.0.0.2/tests/test_GenNet.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/tests/test_conversion.py` & `gennet_forked-2.0.0.2/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `gennet_forked-2.0.0.1/tests/test_interpret.py` & `gennet_forked-2.0.0.2/tests/test_interpret.py`

 * *Files identical despite different names*

