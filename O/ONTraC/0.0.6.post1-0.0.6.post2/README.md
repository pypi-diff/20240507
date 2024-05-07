# Comparing `tmp/ontrac-0.0.6.post1.tar.gz` & `tmp/ontrac-0.0.6.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontrac-0.0.6.post1.tar", last modified: Mon May  6 01:23:33 2024, max compression
+gzip compressed data, was "ontrac-0.0.6.post2.tar", last modified: Tue May  7 18:27:55 2024, max compression
```

## Comparing `ontrac-0.0.6.post1.tar` & `ontrac-0.0.6.post2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-06 01:23:33.619856 ontrac-0.0.6.post1/
--rw-r--r--   0 wwang      (501) staff       (20)     1116 2024-04-25 17:21:18.000000 ontrac-0.0.6.post1/LICENSE
--rw-r--r--   0 wwang      (501) staff       (20)       60 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/MANIFEST.in
--rw-r--r--   0 wwang      (501) staff       (20)     7220 2024-05-06 01:23:33.619647 ontrac-0.0.6.post1/PKG-INFO
--rw-r--r--   0 wwang      (501) staff       (20)     5930 2024-04-25 17:24:03.000000 ontrac-0.0.6.post1/README.md
--rw-r--r--   0 wwang      (501) staff       (20)     1754 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/pyproject.toml
--rw-r--r--   0 wwang      (501) staff       (20)       38 2024-05-06 01:23:33.619900 ontrac-0.0.6.post1/setup.cfg
-drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-06 01:23:33.610103 ontrac-0.0.6.post1/src/
-drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-06 01:23:33.611988 ontrac-0.0.6.post1/src/ONTraC/
--rw-r--r--   0 wwang      (501) staff       (20)       32 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/__init__.py
-drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-06 01:23:33.614163 ontrac-0.0.6.post1/src/ONTraC/analysis/
--rw-r--r--   0 wwang      (501) staff       (20)        0 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/analysis/__init__.py
--rw-r--r--   0 wwang      (501) staff       (20)    10179 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/analysis/cell_type.py
--rw-r--r--   0 wwang      (501) staff       (20)      114 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/analysis/constants.py
--rw-r--r--   0 wwang      (501) staff       (20)    13983 2024-05-06 01:20:12.000000 ontrac-0.0.6.post1/src/ONTraC/analysis/data.py
--rw-r--r--   0 wwang      (501) staff       (20)     2695 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/analysis/meta_info.py
--rw-r--r--   0 wwang      (501) staff       (20)     9716 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/analysis/niche_cluster.py
--rw-r--r--   0 wwang      (501) staff       (20)     5216 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/analysis/spatial.py
--rw-r--r--   0 wwang      (501) staff       (20)     1284 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/analysis/train_loss.py
--rw-r--r--   0 wwang      (501) staff       (20)      915 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/analysis/utils.py
-drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-06 01:23:33.615087 ontrac-0.0.6.post1/src/ONTraC/bin/
--rw-r--r--   0 wwang      (501) staff       (20)     3720 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/bin/GP.py
--rw-r--r--   0 wwang      (501) staff       (20)     1516 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/bin/NTScore.py
--rw-r--r--   0 wwang      (501) staff       (20)     4003 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/bin/ONTraC.py
--rwxr-xr-x   0 wwang      (501) staff       (20)     3357 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/bin/ONTraC_analysis.py
--rw-r--r--   0 wwang      (501) staff       (20)        0 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/bin/__init__.py
--rw-r--r--   0 wwang      (501) staff       (20)     1244 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/bin/createDataSet.py
--rw-r--r--   0 wwang      (501) staff       (20)     3725 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/data.py
--rw-r--r--   0 wwang      (501) staff       (20)      884 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/log.py
-drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-06 01:23:33.615793 ontrac-0.0.6.post1/src/ONTraC/model/
--rw-r--r--   0 wwang      (501) staff       (20)       21 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/model/__init__.py
--rw-r--r--   0 wwang      (501) staff       (20)     6500 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/model/_model.py
--rw-r--r--   0 wwang      (501) staff       (20)     6517 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/model/dmon_exp_pool.py
--rw-r--r--   0 wwang      (501) staff       (20)     3133 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/model/norm_dense_gcn_conv.py
-drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-06 01:23:33.616916 ontrac-0.0.6.post1/src/ONTraC/optparser/
--rw-r--r--   0 wwang      (501) staff       (20)     2232 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/optparser/_GP.py
--rw-r--r--   0 wwang      (501) staff       (20)     4108 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/optparser/_IO.py
--rw-r--r--   0 wwang      (501) staff       (20)     1489 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/optparser/_NT.py
--rw-r--r--   0 wwang      (501) staff       (20)     3198 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/optparser/_ONTraC.py
--rw-r--r--   0 wwang      (501) staff       (20)      260 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/optparser/__init__.py
--rw-r--r--   0 wwang      (501) staff       (20)     2899 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/optparser/_create_dataset.py
--rw-r--r--   0 wwang      (501) staff       (20)     7020 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/optparser/_train.py
-drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-06 01:23:33.617241 ontrac-0.0.6.post1/src/ONTraC/run/
--rw-r--r--   0 wwang      (501) staff       (20)        0 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/run/__init__.py
--rw-r--r--   0 wwang      (501) staff       (20)    10506 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/run/processes.py
-drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-06 01:23:33.618157 ontrac-0.0.6.post1/src/ONTraC/train/
--rw-r--r--   0 wwang      (501) staff       (20)       28 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/train/__init__.py
--rw-r--r--   0 wwang      (501) staff       (20)     9452 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/train/_batch_train.py
--rw-r--r--   0 wwang      (501) staff       (20)     5974 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/train/inspect_funcs.py
--rw-r--r--   0 wwang      (501) staff       (20)     4601 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/train/loss_funs.py
-drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-06 01:23:33.619097 ontrac-0.0.6.post1/src/ONTraC/utils/
--rw-r--r--   0 wwang      (501) staff       (20)     4993 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/utils/NTScore.py
--rw-r--r--   0 wwang      (501) staff       (20)       21 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/utils/__init__.py
--rw-r--r--   0 wwang      (501) staff       (20)     3049 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/utils/_utils.py
--rw-r--r--   0 wwang      (501) staff       (20)     3219 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/utils/decorators.py
--rw-r--r--   0 wwang      (501) staff       (20)     7489 2024-05-06 01:06:13.000000 ontrac-0.0.6.post1/src/ONTraC/utils/niche_net_constr.py
--rw-r--r--   0 wwang      (501) staff       (20)       27 2024-05-06 01:20:18.000000 ontrac-0.0.6.post1/src/ONTraC/version.py
-drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-06 01:23:33.619314 ontrac-0.0.6.post1/src/ONTraC.egg-info/
--rw-r--r--   0 wwang      (501) staff       (20)     7220 2024-05-06 01:23:33.000000 ontrac-0.0.6.post1/src/ONTraC.egg-info/PKG-INFO
--rw-r--r--   0 wwang      (501) staff       (20)     1470 2024-05-06 01:23:33.000000 ontrac-0.0.6.post1/src/ONTraC.egg-info/SOURCES.txt
--rw-r--r--   0 wwang      (501) staff       (20)        1 2024-05-06 01:23:33.000000 ontrac-0.0.6.post1/src/ONTraC.egg-info/dependency_links.txt
--rw-r--r--   0 wwang      (501) staff       (20)      204 2024-05-06 01:23:33.000000 ontrac-0.0.6.post1/src/ONTraC.egg-info/entry_points.txt
--rw-r--r--   0 wwang      (501) staff       (20)       95 2024-05-06 01:23:33.000000 ontrac-0.0.6.post1/src/ONTraC.egg-info/requires.txt
--rw-r--r--   0 wwang      (501) staff       (20)        7 2024-05-06 01:23:33.000000 ontrac-0.0.6.post1/src/ONTraC.egg-info/top_level.txt
+drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-07 18:27:55.543236 ontrac-0.0.6.post2/
+-rw-r--r--   0 wwang      (501) staff       (20)     1116 2024-04-25 17:21:18.000000 ontrac-0.0.6.post2/LICENSE
+-rw-r--r--   0 wwang      (501) staff       (20)       60 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/MANIFEST.in
+-rw-r--r--   0 wwang      (501) staff       (20)     7220 2024-05-07 18:27:55.543019 ontrac-0.0.6.post2/PKG-INFO
+-rw-r--r--   0 wwang      (501) staff       (20)     5930 2024-04-25 17:24:03.000000 ontrac-0.0.6.post2/README.md
+-rw-r--r--   0 wwang      (501) staff       (20)     1754 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/pyproject.toml
+-rw-r--r--   0 wwang      (501) staff       (20)       38 2024-05-07 18:27:55.543277 ontrac-0.0.6.post2/setup.cfg
+drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-07 18:27:55.532613 ontrac-0.0.6.post2/src/
+drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-07 18:27:55.534646 ontrac-0.0.6.post2/src/ONTraC/
+-rw-r--r--   0 wwang      (501) staff       (20)       32 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/__init__.py
+drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-07 18:27:55.537239 ontrac-0.0.6.post2/src/ONTraC/analysis/
+-rw-r--r--   0 wwang      (501) staff       (20)        0 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/analysis/__init__.py
+-rw-r--r--   0 wwang      (501) staff       (20)    10263 2024-05-07 18:24:02.000000 ontrac-0.0.6.post2/src/ONTraC/analysis/cell_type.py
+-rw-r--r--   0 wwang      (501) staff       (20)      114 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/analysis/constants.py
+-rw-r--r--   0 wwang      (501) staff       (20)    13983 2024-05-06 02:05:26.000000 ontrac-0.0.6.post2/src/ONTraC/analysis/data.py
+-rw-r--r--   0 wwang      (501) staff       (20)     2695 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/analysis/meta_info.py
+-rw-r--r--   0 wwang      (501) staff       (20)    15098 2024-05-07 18:24:02.000000 ontrac-0.0.6.post2/src/ONTraC/analysis/niche_cluster.py
+-rw-r--r--   0 wwang      (501) staff       (20)    11483 2024-05-07 18:24:02.000000 ontrac-0.0.6.post2/src/ONTraC/analysis/spatial.py
+-rw-r--r--   0 wwang      (501) staff       (20)     1284 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/analysis/train_loss.py
+-rw-r--r--   0 wwang      (501) staff       (20)      915 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/analysis/utils.py
+drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-07 18:27:55.538202 ontrac-0.0.6.post2/src/ONTraC/bin/
+-rw-r--r--   0 wwang      (501) staff       (20)     3720 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/bin/GP.py
+-rw-r--r--   0 wwang      (501) staff       (20)     1516 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/bin/NTScore.py
+-rw-r--r--   0 wwang      (501) staff       (20)     4003 2024-05-07 17:42:25.000000 ontrac-0.0.6.post2/src/ONTraC/bin/ONTraC.py
+-rwxr-xr-x   0 wwang      (501) staff       (20)     3755 2024-05-07 18:24:02.000000 ontrac-0.0.6.post2/src/ONTraC/bin/ONTraC_analysis.py
+-rw-r--r--   0 wwang      (501) staff       (20)        0 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/bin/__init__.py
+-rw-r--r--   0 wwang      (501) staff       (20)     1244 2024-05-07 17:42:25.000000 ontrac-0.0.6.post2/src/ONTraC/bin/createDataSet.py
+-rw-r--r--   0 wwang      (501) staff       (20)     3725 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/data.py
+-rw-r--r--   0 wwang      (501) staff       (20)      884 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/log.py
+drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-07 18:27:55.538963 ontrac-0.0.6.post2/src/ONTraC/model/
+-rw-r--r--   0 wwang      (501) staff       (20)       21 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/model/__init__.py
+-rw-r--r--   0 wwang      (501) staff       (20)     6500 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/model/_model.py
+-rw-r--r--   0 wwang      (501) staff       (20)     6517 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/model/dmon_exp_pool.py
+-rw-r--r--   0 wwang      (501) staff       (20)     3133 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/model/norm_dense_gcn_conv.py
+drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-07 18:27:55.540206 ontrac-0.0.6.post2/src/ONTraC/optparser/
+-rw-r--r--   0 wwang      (501) staff       (20)     2232 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/optparser/_GP.py
+-rw-r--r--   0 wwang      (501) staff       (20)     4521 2024-05-07 18:24:02.000000 ontrac-0.0.6.post2/src/ONTraC/optparser/_IO.py
+-rw-r--r--   0 wwang      (501) staff       (20)     1489 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/optparser/_NT.py
+-rw-r--r--   0 wwang      (501) staff       (20)     3198 2024-05-07 17:42:25.000000 ontrac-0.0.6.post2/src/ONTraC/optparser/_ONTraC.py
+-rw-r--r--   0 wwang      (501) staff       (20)      260 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/optparser/__init__.py
+-rw-r--r--   0 wwang      (501) staff       (20)     2899 2024-05-07 17:42:25.000000 ontrac-0.0.6.post2/src/ONTraC/optparser/_create_dataset.py
+-rw-r--r--   0 wwang      (501) staff       (20)     7020 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/optparser/_train.py
+drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-07 18:27:55.540531 ontrac-0.0.6.post2/src/ONTraC/run/
+-rw-r--r--   0 wwang      (501) staff       (20)        0 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/run/__init__.py
+-rw-r--r--   0 wwang      (501) staff       (20)    10506 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/run/processes.py
+drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-07 18:27:55.541417 ontrac-0.0.6.post2/src/ONTraC/train/
+-rw-r--r--   0 wwang      (501) staff       (20)       28 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/train/__init__.py
+-rw-r--r--   0 wwang      (501) staff       (20)     9452 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/train/_batch_train.py
+-rw-r--r--   0 wwang      (501) staff       (20)     5974 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/train/inspect_funcs.py
+-rw-r--r--   0 wwang      (501) staff       (20)     4601 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/train/loss_funs.py
+drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-07 18:27:55.542397 ontrac-0.0.6.post2/src/ONTraC/utils/
+-rw-r--r--   0 wwang      (501) staff       (20)     4993 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/utils/NTScore.py
+-rw-r--r--   0 wwang      (501) staff       (20)       21 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/utils/__init__.py
+-rw-r--r--   0 wwang      (501) staff       (20)     3049 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/utils/_utils.py
+-rw-r--r--   0 wwang      (501) staff       (20)     3219 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/utils/decorators.py
+-rw-r--r--   0 wwang      (501) staff       (20)     7673 2024-05-07 18:24:02.000000 ontrac-0.0.6.post2/src/ONTraC/utils/niche_net_constr.py
+-rw-r--r--   0 wwang      (501) staff       (20)       27 2024-05-07 18:24:24.000000 ontrac-0.0.6.post2/src/ONTraC/version.py
+drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-07 18:27:55.542667 ontrac-0.0.6.post2/src/ONTraC.egg-info/
+-rw-r--r--   0 wwang      (501) staff       (20)     7220 2024-05-07 18:27:55.000000 ontrac-0.0.6.post2/src/ONTraC.egg-info/PKG-INFO
+-rw-r--r--   0 wwang      (501) staff       (20)     1470 2024-05-07 18:27:55.000000 ontrac-0.0.6.post2/src/ONTraC.egg-info/SOURCES.txt
+-rw-r--r--   0 wwang      (501) staff       (20)        1 2024-05-07 18:27:55.000000 ontrac-0.0.6.post2/src/ONTraC.egg-info/dependency_links.txt
+-rw-r--r--   0 wwang      (501) staff       (20)      204 2024-05-07 18:27:55.000000 ontrac-0.0.6.post2/src/ONTraC.egg-info/entry_points.txt
+-rw-r--r--   0 wwang      (501) staff       (20)       95 2024-05-07 18:27:55.000000 ontrac-0.0.6.post2/src/ONTraC.egg-info/requires.txt
+-rw-r--r--   0 wwang      (501) staff       (20)        7 2024-05-07 18:27:55.000000 ontrac-0.0.6.post2/src/ONTraC.egg-info/top_level.txt
```

### Comparing `ontrac-0.0.6.post1/LICENSE` & `ontrac-0.0.6.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/PKG-INFO` & `ontrac-0.0.6.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ONTraC
-Version: 0.0.6.post1
+Version: 0.0.6.post2
 Summary: A niche-centered, machine learning method for constructing spatially continuous trajectories
 Author-email: Wen Wang <wwang.bio@gmail.com>, Shiwei Zheng <swzheng29@gmail.com>, Crystal Shin <sjcshin5040@gmail.com>, Guo-Cheng Yuan <gcyuan@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/gyuanlab/ONTraC
 Project-URL: Repository, https://github.com/gyuanlab/ONTraC
 Project-URL: Issue Tracker, https://github.com/gyuanlab/ONTraC/issues
 Keywords: deep-learning,pytorch,pytorch geometric,trajectory inference,spatial omics
```

### Comparing `ontrac-0.0.6.post1/README.md` & `ontrac-0.0.6.post2/README.md`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/pyproject.toml` & `ontrac-0.0.6.post2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/src/ONTraC/analysis/cell_type.py` & `ontrac-0.0.6.post2/src/ONTraC/analysis/cell_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from copy import deepcopy
-from typing import List, Optional, Tuple
+from typing import Optional, Tuple
 
 import matplotlib as mpl
 import numpy as np
 import pandas as pd
 
 mpl.rcParams['pdf.fonttype'] = 42
 mpl.rcParams['ps.fonttype'] = 42
@@ -42,15 +42,15 @@
                    common_norm=True,
                    legend=False,
                    ax=ax)
     ax.set_xlabel('Cell-level NT score')
     ax.set_ylabel('Cell Type')
     fig.tight_layout()
     if ana_data.options.output is not None:
-        fig.savefig(f'{ana_data.options.output}/cell_type_along_NT_score.pdf', transparent=True)
+        fig.savefig(f'{ana_data.options.output}/cell_type_along_NT_score_violin.pdf', transparent=True)
         return None
     else:
         return fig, ax
 
 
 def plot_kde_cell_type_along_NT_score(ana_data: AnaData) -> Optional[Tuple[plt.Figure, plt.Axes]]:
     """
@@ -146,15 +146,15 @@
         var_name='Cell type',
         value_vars=cell_type,  # type: ignore
         value_name='Number')
     # g = sns.catplot(cell_type_dis_melt_df, kind="bar", x="Number", y="Cell type", col="cluster", col_order= nc_order, height=4,
     g = sns.catplot(cell_type_dis_melt_df, kind="bar", x="Number", y="Cell type", col="cluster", height=4,
                     aspect=.5)  # type: ignore
     g.add_legend()
-    g.figure.figsize = (6.4, 20)
+    g.figure.figsize = (2 + len(cell_type) / 3, 20)
     g.tight_layout()
     g.set_xticklabels(rotation='vertical')
     if ana_data.options.output is not None:
         g.savefig(f'{ana_data.options.output}/cell_type_loading_in_niche_clusters.pdf', transparent=True)
         return None
     else:
         return g
@@ -164,15 +164,15 @@
                                          cell_type_dis_df: pd.DataFrame) -> Optional[Tuple[plt.Figure, plt.Axes]]:
     """
     Plot cell type distribution in each niche cluster.
     :param ana_data: AnaData, the data for analysis.
     :param cell_type_dis_df: pd.DataFrame, the cell type distribution in each niche cluster.
     :return: None or Tuple[plt.Figure, plt.Axes]
     """
-    fig, ax = plt.subplots(figsize=(6, 4))
+    fig, ax = plt.subplots(figsize=(2 + cell_type_dis_df.shape[1] / 3, 4))
     sns.heatmap(cell_type_dis_df.apply(lambda x: x / x.sum(), axis=1), ax=ax)
     ax.set_xlabel('Cell Type')
     ax.set_ylabel('Niche Cluster')
     fig.tight_layout()
     if ana_data.options.output is not None:
         fig.savefig(f'{ana_data.options.output}/cell_type_dis_in_niche_clusters.pdf', transparent=True)
         return None
@@ -184,15 +184,15 @@
                                         cell_type_dis_df: pd.DataFrame) -> Optional[Tuple[plt.Figure, plt.Axes]]:
     """
     Plot cell type distribution across niche cluster.
     :param ana_data: AnaData, the data for analysis.
     :param cell_type_dis_df: pd.DataFrame, the cell type distribution in each niche cluster.
     :return: None or Tuple[plt.Figure, plt.Axes]
     """
-    fig, ax = plt.subplots(figsize=(6, 4))
+    fig, ax = plt.subplots(figsize=(2 + cell_type_dis_df.shape[1] / 3, 4))
     sns.heatmap(cell_type_dis_df.apply(lambda x: x / x.sum(), axis=0), ax=ax)
     ax.set_xlabel('Cell Type')
     ax.set_ylabel('Niche Cluster')
     fig.tight_layout()
     if ana_data.options.output is not None:
         fig.savefig(f'{ana_data.options.output}/cell_type_dis_across_niche_cluster.pdf', transparent=True)
         return None
```

### Comparing `ontrac-0.0.6.post1/src/ONTraC/analysis/data.py` & `ontrac-0.0.6.post2/src/ONTraC/analysis/data.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/src/ONTraC/analysis/meta_info.py` & `ontrac-0.0.6.post2/src/ONTraC/analysis/meta_info.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/src/ONTraC/analysis/niche_cluster.py` & `ontrac-0.0.6.post2/src/ONTraC/analysis/niche_cluster.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional, Tuple
+from typing import List, Optional, Tuple, Union
 
 import matplotlib as mpl
 import networkx as nx
 import numpy as np
 import pandas as pd
 from matplotlib.cm import ScalarMappable
 from matplotlib.colors import Normalize
@@ -101,15 +101,15 @@
     if ana_data.options.output is not None:
         fig.savefig(f'{ana_data.options.output}/niche_cluster_proportion.pdf')
         return None
     else:
         return fig, ax
 
 
-def plot_niche_cluster_loadings(ana_data: AnaData) -> Optional[Tuple[plt.Figure, plt.Axes]]:
+def plot_niche_cluster_loadings_dataset(ana_data: AnaData) -> Optional[Tuple[plt.Figure, plt.Axes]]:
     """
     Plot niche cluster loadings for each cell.
     :param ana_data: AnaData, the data for analysis.
     :return: None or Tuple[plt.Figure, plt.Axes]
     """
 
     try:
@@ -144,15 +144,70 @@
     if ana_data.options.output is not None:
         fig.savefig(f'{ana_data.options.output}/niche_cluster_loadings.pdf')
         return None
     else:
         return fig, ax
 
 
-def plot_max_niche_cluster(ana_data: AnaData) -> Optional[Tuple[plt.Figure, plt.Axes]]:
+def plot_niche_cluster_loadings_sample(ana_data: AnaData) -> Optional[List[Tuple[plt.Figure, plt.Axes]]]:
+    """
+    Plot niche cluster loadings for each cell.
+    :param ana_data: AnaData, the data for analysis.
+    :return: None or List[Tuple[plt.Figure, plt.Axes]]
+    """
+
+    try:
+        if ana_data.niche_cluster_score is None or ana_data.cell_type_composition is None or ana_data.cell_level_niche_cluster_assign is None:
+            warning("No niche cluster score, cell type composition or cluster assign data found.")
+            return None
+    except FileNotFoundError as e:
+        warning(str(e))
+        return None
+
+    nc_scores = 1 - ana_data.niche_cluster_score if ana_data.options.reverse else ana_data.niche_cluster_score
+    samples: List[str] = ana_data.cell_type_composition['sample'].unique().tolist()
+
+    output = []
+    for sample in samples:
+        sample_df = ana_data.cell_level_niche_cluster_assign.loc[ana_data.cell_type_composition[
+            ana_data.cell_type_composition['sample'] == sample].index]
+        sample_df = sample_df.join(ana_data.cell_type_composition[['x', 'y']])
+        fig, axes = plt.subplots(1, nc_scores.shape[0], figsize=(3.3 * nc_scores.shape[0], 3))
+        for j, c_index in enumerate(nc_scores.argsort()):
+            ax = axes[j]  #  there should more than one niche cluster
+            scatter = ax.scatter(sample_df['x'],
+                                 sample_df['y'],
+                                 c=sample_df[f'NicheCluster_{c_index}'],
+                                 cmap='Reds',
+                                 vmin=0,
+                                 vmax=1,
+                                 s=4)
+            ax.set_title(f'{sample}: niche cluster {c_index}')
+            plt.colorbar(scatter)
+        fig.tight_layout()
+        output.append((fig, axes))
+        if ana_data.options.output is not None:
+            fig.savefig(f'{ana_data.options.output}/niche_cluster_loadings_{sample}.pdf')
+    return output if len(output) > 0 else None
+
+
+def plot_niche_cluster_loadings(
+        ana_data: AnaData) -> Optional[Union[List[Tuple[plt.Figure, plt.Axes]], Tuple[plt.Figure, plt.Axes]]]:
+    """
+    Plot niche cluster loadings for each cell.
+    :param ana_data: AnaData, the data for analysis.
+    :return: None or Tuple[plt.Figure, plt.Axes]
+    """
+    if hasattr(ana_data.options, 'sample') and ana_data.options.sample:
+        return plot_niche_cluster_loadings_sample(ana_data=ana_data)
+    else:
+        return plot_niche_cluster_loadings_dataset(ana_data=ana_data)
+
+
+def plot_max_niche_cluster_dataset(ana_data: AnaData) -> Optional[Tuple[plt.Figure, plt.Axes]]:
     """
     Plot the maximum niche cluster for each cell.
     :param ana_data: AnaData, the data for analysis.
     :return: None or Tuple[plt.Figure, plt.Axes]
     """
 
     try:
@@ -193,14 +248,74 @@
     if ana_data.options.output is not None:
         fig.savefig(f'{ana_data.options.output}/max_niche_cluster.pdf')
         return None
     else:
         return fig, axes
 
 
+def plot_max_niche_cluster_sample(ana_data: AnaData) -> Optional[List[Tuple[plt.Figure, plt.Axes]]]:
+    """
+    Plot the maximum niche cluster for each cell.
+    :param ana_data: AnaData, the data for analysis.
+    :return: None or List[Tuple[plt.Figure, plt.Axes]]
+    """
+
+    try:
+        if ana_data.niche_cluster_score is None or ana_data.cell_type_composition is None or ana_data.cell_level_max_niche_cluster is None:
+            warning("No niche cluster score, cell type composition or max niche cluster data found.")
+            return None
+    except FileNotFoundError as e:
+        warning(str(e))
+        return None
+
+    # colors
+    norm = Normalize(vmin=0, vmax=1)
+    sm = ScalarMappable(cmap=plt.cm.rainbow, norm=norm)  # type: ignore
+    nc_scores = 1 - ana_data.niche_cluster_score if ana_data.options.reverse else ana_data.niche_cluster_score
+    niche_cluster_colors = [sm.to_rgba(nc_scores[n]) for n in np.arange(ana_data.niche_cluster_score.shape[0])]
+    palette = {f'niche cluster {i}': niche_cluster_colors[i] for i in range(ana_data.niche_cluster_score.shape[0])}
+    samples: List[str] = ana_data.cell_type_composition['sample'].unique().tolist()
+
+    output = []
+    for sample in samples:
+        sample_df = ana_data.cell_level_max_niche_cluster.loc[ana_data.cell_type_composition[
+            ana_data.cell_type_composition['sample'] == sample].index]
+        sample_df = sample_df.join(ana_data.cell_type_composition[['x', 'y']])
+        sample_df['Niche_Cluster'] = 'niche cluster ' + sample_df['Niche_Cluster'].astype(str)
+        fig, ax = plt.subplots(1, 1, figsize=(5, 3))
+        sns.scatterplot(data=sample_df,
+                        x='x',
+                        y='y',
+                        hue='Niche_Cluster',
+                        hue_order=[f'niche cluster {j}' for j in nc_scores.argsort()],
+                        palette=palette,
+                        s=10,
+                        ax=ax)
+        ax.set_title(f'{sample}')
+        ax.legend(loc='upper left', bbox_to_anchor=(1, 1))
+        fig.tight_layout()
+        output.append((fig, ax))
+        if ana_data.options.output is not None:
+            fig.savefig(f'{ana_data.options.output}/max_niche_cluster_{sample}.pdf')
+    return output if len(output) > 0 else None
+
+
+def plot_max_niche_cluster(
+        ana_data: AnaData) -> Optional[Union[List[Tuple[plt.Figure, plt.Axes]], Tuple[plt.Figure, plt.Axes]]]:
+    """
+    Plot the maximum niche cluster for each cell.
+    :param ana_data: AnaData, the data for analysis.
+    :return: None or Tuple[plt.Figure, plt.Axes]
+    """
+    if hasattr(ana_data.options, 'sample') and ana_data.options.sample:
+        return plot_max_niche_cluster_sample(ana_data=ana_data)
+    else:
+        return plot_max_niche_cluster_dataset(ana_data=ana_data)
+
+
 def plot_niche_cluster_gini(ana_data: AnaData) -> Optional[Tuple[plt.Figure, plt.Axes]]:
     """
     Plot the Gini coefficient of each niche cluster.
     :param ana_data: AnaData, the data for analysis.
     :return: None or Tuple[plt.Figure, plt.Axes]
     """
     try:
@@ -244,8 +359,7 @@
     plot_niche_cluster_loadings(ana_data=ana_data)
 
     # 4. maximum niche cluster for each cell
     plot_max_niche_cluster(ana_data=ana_data)
 
     # 5. gini coefficient of each niche cluster
     plot_niche_cluster_gini(ana_data=ana_data)
-
```

### Comparing `ontrac-0.0.6.post1/src/ONTraC/analysis/train_loss.py` & `ontrac-0.0.6.post2/src/ONTraC/analysis/train_loss.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/src/ONTraC/analysis/utils.py` & `ontrac-0.0.6.post2/src/ONTraC/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/src/ONTraC/bin/GP.py` & `ontrac-0.0.6.post2/src/ONTraC/bin/GP.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/src/ONTraC/bin/NTScore.py` & `ontrac-0.0.6.post2/src/ONTraC/bin/NTScore.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/src/ONTraC/bin/ONTraC.py` & `ontrac-0.0.6.post2/src/ONTraC/bin/ONTraC.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/src/ONTraC/bin/ONTraC_analysis.py` & `ontrac-0.0.6.post2/src/ONTraC/bin/ONTraC_analysis.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,34 +50,42 @@
     optparser.add_option('-l', '--log', dest='log', type='string', help='Log file.')
     optparser.add_option('-r',
                          '--reverse',
                          dest='reverse',
                          action='store_true',
                          default=False,
                          help='Reverse the NT score.')
+    optparser.add_option('-s',
+                         '--sample',
+                         dest='sample',
+                         action='store_true',
+                         default=False,
+                         help='Plot each sample separately.')
     add_IO_options_group(optparser=optparser, io_options=IO_OPTIONS)
     return optparser
 
 
 def opt_validate(optparser: OptionParser) -> Values:
     """Validate options from a OptParser object.
 
     Args:
         optparser: OptParser object.
     """
     (options, args) = optparser.parse_args()
 
-    validate_io_options(optparser, options, IO_OPTIONS)
+    validate_io_options(optparser, options, IO_OPTIONS, overwrite_validation=False)
 
     if not options.output:
         error('Output directory is required.')
         sys.exit(1)
     if not os.path.isdir(options.output):
-        warning(f'Output directory not found: {options.output}')
+        info(f'Output directory not found: {options.output}, will create it.')
         os.makedirs(options.output)
+    else:
+        warning(f'Output directory already exists: {options.output}, will overwrite it.')
 
     if not options.log:
         error('Log file is required.')
         sys.exit(1)
     if not os.path.exists(options.log):
         error(f'Log file not found: {options.log}')
         sys.exit(1)
```

### Comparing `ontrac-0.0.6.post1/src/ONTraC/bin/createDataSet.py` & `ontrac-0.0.6.post2/src/ONTraC/bin/createDataSet.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/src/ONTraC/data.py` & `ontrac-0.0.6.post2/src/ONTraC/data.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/src/ONTraC/log.py` & `ontrac-0.0.6.post2/src/ONTraC/log.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/src/ONTraC/model/_model.py` & `ontrac-0.0.6.post2/src/ONTraC/model/_model.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/src/ONTraC/model/dmon_exp_pool.py` & `ontrac-0.0.6.post2/src/ONTraC/model/dmon_exp_pool.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/src/ONTraC/model/norm_dense_gcn_conv.py` & `ontrac-0.0.6.post2/src/ONTraC/model/norm_dense_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/src/ONTraC/optparser/_GP.py` & `ontrac-0.0.6.post2/src/ONTraC/optparser/_GP.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/src/ONTraC/optparser/_IO.py` & `ontrac-0.0.6.post2/src/ONTraC/optparser/_IO.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,18 @@
         group_io.add_option('--GNN-dir', dest='GNN_dir', type='string', help='Directory for the GNN output.')
     if 'NTScore_dir' in io_options:
         group_io.add_option('--NTScore-dir', dest='NTScore_dir', type='string', help='Directory for the NTScore output')
 
     optparser.add_option_group(group_io)
 
 
-def validate_io_options(optparser: OptionParser, options: Values, io_options: Optional[List[str]]) -> None:
+def validate_io_options(optparser: OptionParser,
+                        options: Values,
+                        io_options: Optional[List[str]],
+                        overwrite_validation: bool = True) -> None:
     """Validate IO options from a OptParser object.
 
     Ret: None
     """
     if io_options is None:
         return
     if 'dataset' in io_options:
@@ -54,40 +57,50 @@
 
     if 'preprocessing_dir' in io_options:
         if not options.preprocessing_dir:
             error('Please provide a directory for preprocessing outputs.')
             optparser.print_help()
             sys.exit(1)
         if os.path.isdir(options.preprocessing_dir):
-            warning(f'The directory ({options.preprocessing_dir}) you given already exists. It will be overwritten.')
+            if overwrite_validation:
+                warning(
+                    f'The directory ({options.preprocessing_dir}) you given already exists. It will be overwritten.')
+            else:
+                pass
         else:
             info(f'Creating directory: {options.preprocessing_dir}')
-            os.makedirs(options.preprocessing_dir)
+            os.makedirs(options.preprocessing_dir, exist_ok=True)
 
     if 'GNN_dir' in io_options:
         if not options.GNN_dir:
             error('Please provide a directory for the GNN output.')
             optparser.print_help()
             sys.exit(1)
         if os.path.isdir(options.GNN_dir):
-            warning(f'The directory ({options.GNN_dir}) you given already exists. It will be overwritten.')
+            if overwrite_validation:
+                warning(f'The directory ({options.GNN_dir}) you given already exists. It will be overwritten.')
+            else:
+                pass
         else:
             info(f'Creating directory: {options.GNN_dir}')
-            os.makedirs(options.GNN_dir)
+            os.makedirs(options.GNN_dir, exist_ok=True)
 
     if 'NTScore_dir' in io_options:
         if not options.NTScore_dir:
             error('Please provide a directory for the NTScore output.')
             optparser.print_help()
             sys.exit(1)
         if os.path.isdir(options.NTScore_dir):
-            warning(f'The directory ({options.NTScore_dir}) you given already exists. It will be overwritten.')
+            if overwrite_validation:
+                warning(f'The directory ({options.NTScore_dir}) you given already exists. It will be overwritten.')
+            else:
+                pass
         else:
             info(f'Creating directory: {options.NTScore_dir}')
-            os.makedirs(options.NTScore_dir)
+            os.makedirs(options.NTScore_dir, exist_ok=True)
 
 
 def write_io_options_memo(options: Values, io_options: Optional[List[str]]) -> None:
     """Write IO options to stdout.
 
     Ret: None
     """
```

### Comparing `ontrac-0.0.6.post1/src/ONTraC/optparser/_NT.py` & `ontrac-0.0.6.post2/src/ONTraC/optparser/_NT.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/src/ONTraC/optparser/_ONTraC.py` & `ontrac-0.0.6.post2/src/ONTraC/optparser/_ONTraC.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/src/ONTraC/optparser/_create_dataset.py` & `ontrac-0.0.6.post2/src/ONTraC/optparser/_create_dataset.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/src/ONTraC/optparser/_train.py` & `ontrac-0.0.6.post2/src/ONTraC/optparser/_train.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/src/ONTraC/run/processes.py` & `ontrac-0.0.6.post2/src/ONTraC/run/processes.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/src/ONTraC/train/_batch_train.py` & `ontrac-0.0.6.post2/src/ONTraC/train/_batch_train.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/src/ONTraC/train/inspect_funcs.py` & `ontrac-0.0.6.post2/src/ONTraC/train/inspect_funcs.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/src/ONTraC/train/loss_funs.py` & `ontrac-0.0.6.post2/src/ONTraC/train/loss_funs.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/src/ONTraC/utils/NTScore.py` & `ontrac-0.0.6.post2/src/ONTraC/utils/NTScore.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/src/ONTraC/utils/_utils.py` & `ontrac-0.0.6.post2/src/ONTraC/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/src/ONTraC/utils/decorators.py` & `ontrac-0.0.6.post2/src/ONTraC/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post1/src/ONTraC/utils/niche_net_constr.py` & `ontrac-0.0.6.post2/src/ONTraC/utils/niche_net_constr.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,18 @@
     if ori_data_df['Cell_ID'].isnull().any():
         raise ValueError(f'Duplicated Cell_ID within same sample found! Please check the original data file: {options.data_file}.')
 
     ori_data_df = ori_data_df.dropna(subset=['Cell_ID', 'Sample', 'Cell_Type', 'x', 'y'])
 
     # make the Cell_Type column categorical
     ori_data_df['Cell_Type'] = ori_data_df['Cell_Type'].astype('category')
+    # check if the cell type category number is less than 2
+    if len(ori_data_df['Cell_Type'].cat.categories) < 2:
+        raise ValueError('At least two cell types are required.')
+
     # save mappings of the categorical data
     cell_type_code = pd.DataFrame(enumerate(ori_data_df['Cell_Type'].cat.categories), columns=['Code', 'Cell_Type'])
     cell_type_code.to_csv(f'{options.preprocessing_dir}/cell_type_code.csv', index=False)
 
     return ori_data_df
```

### Comparing `ontrac-0.0.6.post1/src/ONTraC.egg-info/PKG-INFO` & `ontrac-0.0.6.post2/src/ONTraC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ONTraC
-Version: 0.0.6.post1
+Version: 0.0.6.post2
 Summary: A niche-centered, machine learning method for constructing spatially continuous trajectories
 Author-email: Wen Wang <wwang.bio@gmail.com>, Shiwei Zheng <swzheng29@gmail.com>, Crystal Shin <sjcshin5040@gmail.com>, Guo-Cheng Yuan <gcyuan@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/gyuanlab/ONTraC
 Project-URL: Repository, https://github.com/gyuanlab/ONTraC
 Project-URL: Issue Tracker, https://github.com/gyuanlab/ONTraC/issues
 Keywords: deep-learning,pytorch,pytorch geometric,trajectory inference,spatial omics
```

### Comparing `ontrac-0.0.6.post1/src/ONTraC.egg-info/SOURCES.txt` & `ontrac-0.0.6.post2/src/ONTraC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

