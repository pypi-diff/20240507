# Comparing `tmp/luma-ml-0.7.2.tar.gz` & `tmp/luma-ml-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luma-ml-0.7.2.tar", last modified: Sun Apr 28 08:56:41 2024, max compression
+gzip compressed data, was "luma-ml-0.7.3.tar", last modified: Tue May  7 20:10:10 2024, max compression
```

## Comparing `luma-ml-0.7.2.tar` & `luma-ml-0.7.3.tar`

### file list

```diff
@@ -1,88 +1,93 @@
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.545930 luma-ml-0.7.2/
--rw-r--r--   0 chanlee    (501) staff       (20)    35149 2023-11-07 13:17:31.000000 luma-ml-0.7.2/LICENSE
--rw-r--r--   0 chanlee    (501) staff       (20)     5554 2024-04-28 08:56:41.545574 luma-ml-0.7.2/PKG-INFO
--rw-r--r--   0 chanlee    (501) staff       (20)     4948 2024-04-28 08:56:35.000000 luma-ml-0.7.2/README.md
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.517832 luma-ml-0.7.2/luma/
--rw-r--r--   0 chanlee    (501) staff       (20)    10290 2024-04-28 08:49:23.000000 luma-ml-0.7.2/luma/__import__.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1501 2024-03-17 16:24:24.000000 luma-ml-0.7.2/luma/__init__.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.521151 luma-ml-0.7.2/luma/classifier/
--rw-r--r--   0 chanlee    (501) staff       (20)    12302 2024-04-27 19:24:30.000000 luma-ml-0.7.2/luma/classifier/discriminant.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7629 2024-04-21 11:35:40.000000 luma-ml-0.7.2/luma/classifier/logistic.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5541 2024-04-21 11:35:39.000000 luma-ml-0.7.2/luma/classifier/naive_bayes.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8953 2024-04-21 11:35:43.000000 luma-ml-0.7.2/luma/classifier/neighbors.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8887 2024-04-21 11:35:41.000000 luma-ml-0.7.2/luma/classifier/svm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9536 2024-04-21 11:35:42.000000 luma-ml-0.7.2/luma/classifier/tree.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.525297 luma-ml-0.7.2/luma/clustering/
--rw-r--r--   0 chanlee    (501) staff       (20)    17291 2024-04-21 11:35:45.000000 luma-ml-0.7.2/luma/clustering/affinity.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17401 2024-04-21 11:35:47.000000 luma-ml-0.7.2/luma/clustering/density.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7672 2024-04-21 11:35:48.000000 luma-ml-0.7.2/luma/clustering/hierarchy.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17695 2024-04-21 11:35:49.000000 luma-ml-0.7.2/luma/clustering/kmeans.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8019 2024-04-21 11:35:50.000000 luma-ml-0.7.2/luma/clustering/mixture.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11404 2024-04-21 11:35:51.000000 luma-ml-0.7.2/luma/clustering/spectral.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.526201 luma-ml-0.7.2/luma/core/
--rw-r--r--   0 chanlee    (501) staff       (20)     5923 2024-04-28 07:19:53.000000 luma-ml-0.7.2/luma/core/base.py
--rw-r--r--   0 chanlee    (501) staff       (20)      394 2024-04-28 05:47:04.000000 luma-ml-0.7.2/luma/core/main.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11588 2024-04-28 08:33:36.000000 luma-ml-0.7.2/luma/core/super.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.528856 luma-ml-0.7.2/luma/ensemble/
--rw-r--r--   0 chanlee    (501) staff       (20)     9749 2024-04-21 11:35:52.000000 luma-ml-0.7.2/luma/ensemble/bagging.py
--rw-r--r--   0 chanlee    (501) staff       (20)    19258 2024-04-21 11:35:53.000000 luma-ml-0.7.2/luma/ensemble/boost.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9633 2024-04-21 11:35:54.000000 luma-ml-0.7.2/luma/ensemble/forest.py
--rw-r--r--   0 chanlee    (501) staff       (20)    13550 2024-04-21 11:35:55.000000 luma-ml-0.7.2/luma/ensemble/stack.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6513 2024-04-21 11:35:56.000000 luma-ml-0.7.2/luma/ensemble/vote.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.529747 luma-ml-0.7.2/luma/interface/
--rw-r--r--   0 chanlee    (501) staff       (20)     1294 2024-04-03 15:51:54.000000 luma-ml-0.7.2/luma/interface/exception.py
--rw-r--r--   0 chanlee    (501) staff       (20)     4881 2024-04-25 18:52:30.000000 luma-ml-0.7.2/luma/interface/typing.py
--rw-r--r--   0 chanlee    (501) staff       (20)    15126 2024-04-28 08:49:04.000000 luma-ml-0.7.2/luma/interface/util.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.530789 luma-ml-0.7.2/luma/metric/
--rw-r--r--   0 chanlee    (501) staff       (20)     1654 2024-04-24 15:30:21.000000 luma-ml-0.7.2/luma/metric/classification.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5821 2024-04-24 15:56:48.000000 luma-ml-0.7.2/luma/metric/clustering.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1788 2024-04-24 15:55:30.000000 luma-ml-0.7.2/luma/metric/distance.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1842 2024-04-24 15:57:32.000000 luma-ml-0.7.2/luma/metric/regression.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.530972 luma-ml-0.7.2/luma/migrate/
--rw-r--r--   0 chanlee    (501) staff       (20)     3425 2024-04-03 18:12:20.000000 luma-ml-0.7.2/luma/migrate/port.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.532778 luma-ml-0.7.2/luma/model_selection/
--rw-r--r--   0 chanlee    (501) staff       (20)     3269 2024-04-21 11:36:03.000000 luma-ml-0.7.2/luma/model_selection/cv.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7681 2024-04-21 11:36:04.000000 luma-ml-0.7.2/luma/model_selection/fold.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11846 2024-04-21 11:36:05.000000 luma-ml-0.7.2/luma/model_selection/search.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5221 2024-04-21 11:36:06.000000 luma-ml-0.7.2/luma/model_selection/split.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.534456 luma-ml-0.7.2/luma/neural/
--rw-r--r--   0 chanlee    (501) staff       (20)     4379 2024-04-28 05:47:17.000000 luma-ml-0.7.2/luma/neural/base.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1673 2024-04-24 13:56:17.000000 luma-ml-0.7.2/luma/neural/init.py
--rw-r--r--   0 chanlee    (501) staff       (20)    25256 2024-04-28 08:53:42.000000 luma-ml-0.7.2/luma/neural/layer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3111 2024-04-27 18:48:15.000000 luma-ml-0.7.2/luma/neural/loss.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6772 2024-04-28 08:56:03.000000 luma-ml-0.7.2/luma/neural/network.py
--rw-r--r--   0 chanlee    (501) staff       (20)    21132 2024-04-28 05:47:13.000000 luma-ml-0.7.2/luma/neural/optimizer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8210 2024-04-21 11:36:12.000000 luma-ml-0.7.2/luma/neural/single.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.534954 luma-ml-0.7.2/luma/pipe/
--rw-r--r--   0 chanlee    (501) staff       (20)     7219 2024-04-21 11:36:13.000000 luma-ml-0.7.2/luma/pipe/pipeline.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.536290 luma-ml-0.7.2/luma/preprocessing/
--rw-r--r--   0 chanlee    (501) staff       (20)     5295 2024-04-21 11:36:14.000000 luma-ml-0.7.2/luma/preprocessing/encoder.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5533 2024-04-21 11:36:15.000000 luma-ml-0.7.2/luma/preprocessing/imputer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3602 2024-04-21 11:36:16.000000 luma-ml-0.7.2/luma/preprocessing/outlier.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2555 2024-04-21 11:36:18.000000 luma-ml-0.7.2/luma/preprocessing/scaler.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.538502 luma-ml-0.7.2/luma/reduction/
--rw-r--r--   0 chanlee    (501) staff       (20)    18479 2024-04-21 11:36:19.000000 luma-ml-0.7.2/luma/reduction/linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)    39141 2024-04-21 11:36:22.000000 luma-ml-0.7.2/luma/reduction/manifold.py
--rw-r--r--   0 chanlee    (501) staff       (20)    16204 2024-04-21 11:36:23.000000 luma-ml-0.7.2/luma/reduction/selection.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.542136 luma-ml-0.7.2/luma/regressor/
--rw-r--r--   0 chanlee    (501) staff       (20)    19093 2024-04-21 11:36:25.000000 luma-ml-0.7.2/luma/regressor/general.py
--rw-r--r--   0 chanlee    (501) staff       (20)    12211 2024-04-21 11:36:26.000000 luma-ml-0.7.2/luma/regressor/linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6638 2024-04-21 11:36:27.000000 luma-ml-0.7.2/luma/regressor/neighbors.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2962 2024-04-21 11:36:28.000000 luma-ml-0.7.2/luma/regressor/poly.py
--rw-r--r--   0 chanlee    (501) staff       (20)    10680 2024-04-21 11:36:29.000000 luma-ml-0.7.2/luma/regressor/robust.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7519 2024-04-21 11:36:30.000000 luma-ml-0.7.2/luma/regressor/svm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7189 2024-04-21 11:36:31.000000 luma-ml-0.7.2/luma/regressor/tree.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.542703 luma-ml-0.7.2/luma/visual/
--rw-r--r--   0 chanlee    (501) staff       (20)     3045 2024-04-13 08:30:32.000000 luma-ml-0.7.2/luma/visual/eda.py
--rw-r--r--   0 chanlee    (501) staff       (20)    24473 2024-04-21 11:36:32.000000 luma-ml-0.7.2/luma/visual/evaluation.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.544224 luma-ml-0.7.2/luma_ml.egg-info/
--rw-r--r--   0 chanlee    (501) staff       (20)     5554 2024-04-28 08:56:41.000000 luma-ml-0.7.2/luma_ml.egg-info/PKG-INFO
--rw-r--r--   0 chanlee    (501) staff       (20)     1662 2024-04-28 08:56:41.000000 luma-ml-0.7.2/luma_ml.egg-info/SOURCES.txt
--rw-r--r--   0 chanlee    (501) staff       (20)        1 2024-04-28 08:56:41.000000 luma-ml-0.7.2/luma_ml.egg-info/dependency_links.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-04-28 08:56:41.000000 luma-ml-0.7.2/luma_ml.egg-info/requires.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       17 2024-04-28 08:56:41.000000 luma-ml-0.7.2/luma_ml.egg-info/top_level.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-04-28 08:56:41.545997 luma-ml-0.7.2/setup.cfg
--rw-r--r--   0 chanlee    (501) staff       (20)      842 2024-04-28 08:56:37.000000 luma-ml-0.7.2/setup.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.544858 luma-ml-0.7.2/test/
--rw-r--r--   0 chanlee    (501) staff       (20)      105 2024-04-20 19:16:53.000000 luma-ml-0.7.2/test/__local__.py
--rw-r--r--   0 chanlee    (501) staff       (20)      917 2024-04-28 08:55:29.000000 luma-ml-0.7.2/test/__test.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.377522 luma-ml-0.7.3/
+-rw-r--r--   0 chanlee    (501) staff       (20)    35149 2023-11-07 13:17:31.000000 luma-ml-0.7.3/LICENSE
+-rw-r--r--   0 chanlee    (501) staff       (20)     5552 2024-05-07 20:10:10.377108 luma-ml-0.7.3/PKG-INFO
+-rw-r--r--   0 chanlee    (501) staff       (20)     4946 2024-05-07 20:08:48.000000 luma-ml-0.7.3/README.md
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.344821 luma-ml-0.7.3/luma/
+-rw-r--r--   0 chanlee    (501) staff       (20)    10486 2024-05-07 19:27:37.000000 luma-ml-0.7.3/luma/__import__.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1501 2024-03-17 16:24:24.000000 luma-ml-0.7.3/luma/__init__.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.347799 luma-ml-0.7.3/luma/classifier/
+-rw-r--r--   0 chanlee    (501) staff       (20)    12302 2024-04-27 19:24:30.000000 luma-ml-0.7.3/luma/classifier/discriminant.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7629 2024-04-21 11:35:40.000000 luma-ml-0.7.3/luma/classifier/logistic.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5541 2024-04-21 11:35:39.000000 luma-ml-0.7.3/luma/classifier/naive_bayes.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8953 2024-04-21 11:35:43.000000 luma-ml-0.7.3/luma/classifier/neighbors.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8887 2024-04-21 11:35:41.000000 luma-ml-0.7.3/luma/classifier/svm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9536 2024-04-21 11:35:42.000000 luma-ml-0.7.3/luma/classifier/tree.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.351938 luma-ml-0.7.3/luma/clustering/
+-rw-r--r--   0 chanlee    (501) staff       (20)    17291 2024-04-21 11:35:45.000000 luma-ml-0.7.3/luma/clustering/affinity.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17401 2024-04-21 11:35:47.000000 luma-ml-0.7.3/luma/clustering/density.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7672 2024-04-21 11:35:48.000000 luma-ml-0.7.3/luma/clustering/hierarchy.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17695 2024-04-21 11:35:49.000000 luma-ml-0.7.3/luma/clustering/kmeans.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8019 2024-04-21 11:35:50.000000 luma-ml-0.7.3/luma/clustering/mixture.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11404 2024-04-21 11:35:51.000000 luma-ml-0.7.3/luma/clustering/spectral.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.353338 luma-ml-0.7.3/luma/core/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5923 2024-04-28 07:19:53.000000 luma-ml-0.7.3/luma/core/base.py
+-rw-r--r--   0 chanlee    (501) staff       (20)      394 2024-04-28 05:47:04.000000 luma-ml-0.7.3/luma/core/main.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    10856 2024-05-04 18:13:20.000000 luma-ml-0.7.3/luma/core/super.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.356246 luma-ml-0.7.3/luma/ensemble/
+-rw-r--r--   0 chanlee    (501) staff       (20)     9749 2024-04-21 11:35:52.000000 luma-ml-0.7.3/luma/ensemble/bagging.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    19258 2024-04-21 11:35:53.000000 luma-ml-0.7.3/luma/ensemble/boost.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9633 2024-04-21 11:35:54.000000 luma-ml-0.7.3/luma/ensemble/forest.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    13550 2024-04-21 11:35:55.000000 luma-ml-0.7.3/luma/ensemble/stack.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6513 2024-04-21 11:35:56.000000 luma-ml-0.7.3/luma/ensemble/vote.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.357343 luma-ml-0.7.3/luma/interface/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1294 2024-04-03 15:51:54.000000 luma-ml-0.7.3/luma/interface/exception.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     4881 2024-04-28 23:46:05.000000 luma-ml-0.7.3/luma/interface/typing.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    15102 2024-05-06 13:39:46.000000 luma-ml-0.7.3/luma/interface/util.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.359164 luma-ml-0.7.3/luma/metric/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1654 2024-04-24 15:30:21.000000 luma-ml-0.7.3/luma/metric/classification.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5821 2024-04-24 15:56:48.000000 luma-ml-0.7.3/luma/metric/clustering.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1788 2024-04-24 15:55:30.000000 luma-ml-0.7.3/luma/metric/distance.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1842 2024-04-24 15:57:32.000000 luma-ml-0.7.3/luma/metric/regression.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.359480 luma-ml-0.7.3/luma/migrate/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3425 2024-04-03 18:12:20.000000 luma-ml-0.7.3/luma/migrate/port.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.361291 luma-ml-0.7.3/luma/model_selection/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3269 2024-04-21 11:36:03.000000 luma-ml-0.7.3/luma/model_selection/cv.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7681 2024-04-21 11:36:04.000000 luma-ml-0.7.3/luma/model_selection/fold.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11846 2024-04-21 11:36:05.000000 luma-ml-0.7.3/luma/model_selection/search.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5221 2024-05-06 08:57:35.000000 luma-ml-0.7.3/luma/model_selection/split.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.363952 luma-ml-0.7.3/luma/neural/
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.364697 luma-ml-0.7.3/luma/neural/_models/
+-rw-r--r--   0 chanlee    (501) staff       (20)    11922 2024-05-07 20:02:13.000000 luma-ml-0.7.3/luma/neural/_models/_lenet.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9322 2024-05-07 19:26:47.000000 luma-ml-0.7.3/luma/neural/_models/_simple.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9429 2024-05-07 19:46:22.000000 luma-ml-0.7.3/luma/neural/base.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5281 2024-05-07 20:08:02.000000 luma-ml-0.7.3/luma/neural/block.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1673 2024-04-24 13:56:17.000000 luma-ml-0.7.3/luma/neural/init.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    25499 2024-05-07 20:08:04.000000 luma-ml-0.7.3/luma/neural/layer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3111 2024-05-04 07:19:22.000000 luma-ml-0.7.3/luma/neural/loss.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    16051 2024-05-07 20:00:11.000000 luma-ml-0.7.3/luma/neural/network.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    21132 2024-04-28 05:47:13.000000 luma-ml-0.7.3/luma/neural/optimizer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8210 2024-04-21 11:36:12.000000 luma-ml-0.7.3/luma/neural/single.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.364905 luma-ml-0.7.3/luma/pipe/
+-rw-r--r--   0 chanlee    (501) staff       (20)     7219 2024-04-21 11:36:13.000000 luma-ml-0.7.3/luma/pipe/pipeline.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.366483 luma-ml-0.7.3/luma/preprocessing/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5295 2024-04-21 11:36:14.000000 luma-ml-0.7.3/luma/preprocessing/encoder.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5533 2024-04-21 11:36:15.000000 luma-ml-0.7.3/luma/preprocessing/imputer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3602 2024-04-21 11:36:16.000000 luma-ml-0.7.3/luma/preprocessing/outlier.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2555 2024-04-21 11:36:18.000000 luma-ml-0.7.3/luma/preprocessing/scaler.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.369223 luma-ml-0.7.3/luma/reduction/
+-rw-r--r--   0 chanlee    (501) staff       (20)    18479 2024-04-21 11:36:19.000000 luma-ml-0.7.3/luma/reduction/linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    39141 2024-04-21 11:36:22.000000 luma-ml-0.7.3/luma/reduction/manifold.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    16204 2024-04-21 11:36:23.000000 luma-ml-0.7.3/luma/reduction/selection.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.373034 luma-ml-0.7.3/luma/regressor/
+-rw-r--r--   0 chanlee    (501) staff       (20)    19093 2024-04-21 11:36:25.000000 luma-ml-0.7.3/luma/regressor/general.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12211 2024-04-21 11:36:26.000000 luma-ml-0.7.3/luma/regressor/linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6638 2024-04-21 11:36:27.000000 luma-ml-0.7.3/luma/regressor/neighbors.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2962 2024-04-21 11:36:28.000000 luma-ml-0.7.3/luma/regressor/poly.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    10680 2024-04-21 11:36:29.000000 luma-ml-0.7.3/luma/regressor/robust.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7519 2024-04-21 11:36:30.000000 luma-ml-0.7.3/luma/regressor/svm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7189 2024-04-21 11:36:31.000000 luma-ml-0.7.3/luma/regressor/tree.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.373688 luma-ml-0.7.3/luma/visual/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3045 2024-04-13 08:30:32.000000 luma-ml-0.7.3/luma/visual/eda.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    24473 2024-04-21 11:36:32.000000 luma-ml-0.7.3/luma/visual/evaluation.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.374941 luma-ml-0.7.3/luma_ml.egg-info/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5552 2024-05-07 20:10:10.000000 luma-ml-0.7.3/luma_ml.egg-info/PKG-INFO
+-rw-r--r--   0 chanlee    (501) staff       (20)     1758 2024-05-07 20:10:10.000000 luma-ml-0.7.3/luma_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)        1 2024-05-07 20:10:10.000000 luma-ml-0.7.3/luma_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-07 20:10:10.000000 luma-ml-0.7.3/luma_ml.egg-info/requires.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       17 2024-05-07 20:10:10.000000 luma-ml-0.7.3/luma_ml.egg-info/top_level.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-07 20:10:10.377601 luma-ml-0.7.3/setup.cfg
+-rw-r--r--   0 chanlee    (501) staff       (20)      842 2024-05-07 20:09:55.000000 luma-ml-0.7.3/setup.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.376270 luma-ml-0.7.3/test/
+-rw-r--r--   0 chanlee    (501) staff       (20)      647 2024-04-29 02:58:00.000000 luma-ml-0.7.3/test/__act.py
+-rw-r--r--   0 chanlee    (501) staff       (20)      105 2024-04-20 19:16:53.000000 luma-ml-0.7.3/test/__local__.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1403 2024-05-07 20:09:50.000000 luma-ml-0.7.3/test/__test.py
```

### Comparing `luma-ml-0.7.2/LICENSE` & `luma-ml-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/PKG-INFO` & `luma-ml-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luma-ml
-Version: 0.7.2
+Version: 0.7.3
 Summary: A Comprehensive Python Module for Machine Learning and Data Science
 Home-page: https://github.com/ChanLumerico/luma
 Author: ChanLumerico
 Author-email: greensox284@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-5.13k-red">
+        <img src="https://img.shields.io/badge/total downloads-5.41k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -108,19 +108,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.7.2</td>
+                    <td>0.7.3</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~17.8K</td>
+                    <td>~18K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: luma-ml Version: 0.7.2 Summary: A Comprehensive
+Metadata-Version: 2.1 Name: luma-ml Version: 0.7.3 Summary: A Comprehensive
 Python Module for Machine Learning and Data Science Home-page: https://
 github.com/ChanLumerico/luma Author: ChanLumerico Author-email:
 greensox284@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.12
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy Requires-Dist: scipy Requires-Dist: pandas Requires-Dist: matplotlib
 Requires-Dist: seaborn
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-5.13k-red][GitHub code size in bytes][Code Style]
+5.41k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -33,12 +33,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.7.2
-Lines of Code  ~17.8K
+Latest Version 0.7.3
+Lines of Code  ~18K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.7.2/README.md` & `luma-ml-0.7.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-5.13k-red">
+        <img src="https://img.shields.io/badge/total downloads-5.41k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -89,19 +89,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.7.2</td>
+                    <td>0.7.3</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~17.8K</td>
+                    <td>~18K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-5.13k-red][GitHub code size in bytes][Code Style]
+5.41k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -24,12 +24,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.7.2
-Lines of Code  ~17.8K
+Latest Version 0.7.3
+Lines of Code  ~18K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.7.2/luma/__import__.py` & `luma-ml-0.7.3/luma/__import__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,10 @@
 from luma.core.main import Luma
 from luma.core.base import ModelBase, ParadigmBase, MetricBase, VisualBase
-from luma.core.super import (
-    Estimator,
-    Transformer,
-    Optimizer,
-    Evaluator,
-    Visualizer,
-    NeuralModel,
-)
+from luma.core.super import Estimator, Transformer, Optimizer, Evaluator, Visualizer
 from luma.core.super import Supervised, Unsupervised, Distance
 
 from luma.interface.exception import (
     NotFittedError,
     NotConvergedError,
     UnsupportedParameterError,
     ModelExtensionError,
@@ -74,38 +67,41 @@
 from luma.ensemble.forest import RandomForestClassifier, RandomForestRegressor
 from luma.ensemble.vote import VotingClassifier, VotingRegressor
 from luma.ensemble.bagging import BaggingClassifier, BaggingRegressor
 from luma.ensemble.boost import AdaBoostClassifier, AdaBoostRegressor
 from luma.ensemble.boost import GradientBoostingClassifier, GradientBoostingRegressor
 from luma.ensemble.stack import StackingClassifier, StackingRegressor
 
+from luma.neural.base import Layer, Loss, Initializer, NeuralModel
+from luma.neural.single import PerceptronClassifier, PerceptronRegressor
+from luma.neural.layer import (
+    Convolution,
+    Pooling,
+    Dense,
+    Dropout,
+    Flatten,
+    Activation,
+    Sequential,
+)
 from luma.neural.optimizer import (
     SGDOptimizer,
     MomentumOptimizer,
     RMSPropOptimizer,
     AdamOptimizer,
     AdaGradOptimizer,
     AdaDeltaOptimizer,
     AdaMaxOptimizer,
     AdamWOptimizer,
     NAdamOptimizer,
 )
-from luma.neural.single import PerceptronClassifier, PerceptronRegressor
-from luma.neural.base import Layer, Loss, Initializer
-from luma.neural.layer import (
-    Convolution,
-    Pooling,
-    Dense,
-    Dropout,
-    Flatten,
-    Activation,
-    Sequential,
-)
 from luma.neural.loss import CrossEntropy, BinaryCrossEntropy, MSELoss
 from luma.neural.init import KaimingInit, XavierInit
+from luma.neural.block import ConvBlock, DenseBlock
+from luma.neural.network import SimpleMLP, SimpleCNN
+from luma.neural.network import LeNet_1, LeNet_4
 
 from luma.metric.classification import Accuracy, Precision, Recall, F1Score, Specificity
 from luma.metric.regression import (
     MeanAbsoluteError,
     MeanSquaredError,
     RootMeanSquaredError,
     MeanAbsolutePercentageError,
@@ -180,15 +176,15 @@
 
     # ------------------- [ luma.core ] ------------------------
     Luma
 
     ModelBase, ParadigmBase, MetricBase, VisualBase
 
     Estimator, Transformer, Optimizer, Evaluator, Visualizer,
-    Supervised, Unsupervised, Distance, NeuralModel
+    Supervised, Unsupervised, Distance
 
     # ----------------- [ luma.interface ] ---------------------
     NotFittedError, NotConvergedError,
     UnsupportedParameterError, ModelExtensionError,
     InvalidRangeError
 
     TensorLike, Matrix, Vector, Tensor, Scalar, ClassType
@@ -242,23 +238,27 @@
     # ------------------- [ luma.neural ] ----------------------
     PerceptronClassifier, PerceptronRegressor
 
     SGDOptimizer, MomentumOptimizer, RMSPropOptimizer,
     AdamOptimizer, AdaGradOptimizer, AdaDeltaOptimizer,
     AdaMaxOptimizer, AdamWOptimizer, NAdamOptimizer
 
-    Layer, Loss, Initializer
+    Layer, Loss, Initializer, NeuralModel
 
     Convolution, Pooling, Dense, Dropout, Flatten, Activation,
     Sequential
 
     CrossEntropy, BinaryCrossEntropy, MSELoss
 
     KaimingInit, XavierInit
 
+    ConvBlock, DenseBlock
+
+    SimpleMLP, SimpleCNN, LeNet_1, LeNet_4
+
     # ------------------- [ luma.metric ] ----------------------
     Accuracy, Precision, Recall, F1Score, Specificity
 
     MeanAbsoluteError, MeanSquaredError, RootMeanSquaredError,
     MeanAbsolutePercentageError, RSquaredScore,
     AdjustedRSquaredScore
```

### Comparing `luma-ml-0.7.2/luma/__init__.py` & `luma-ml-0.7.3/luma/__init__.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/classifier/discriminant.py` & `luma-ml-0.7.3/luma/classifier/discriminant.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/classifier/logistic.py` & `luma-ml-0.7.3/luma/classifier/logistic.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/classifier/naive_bayes.py` & `luma-ml-0.7.3/luma/classifier/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/classifier/neighbors.py` & `luma-ml-0.7.3/luma/classifier/neighbors.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/classifier/svm.py` & `luma-ml-0.7.3/luma/classifier/svm.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/classifier/tree.py` & `luma-ml-0.7.3/luma/classifier/tree.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/clustering/affinity.py` & `luma-ml-0.7.3/luma/clustering/affinity.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/clustering/density.py` & `luma-ml-0.7.3/luma/clustering/density.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/clustering/hierarchy.py` & `luma-ml-0.7.3/luma/clustering/hierarchy.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/clustering/kmeans.py` & `luma-ml-0.7.3/luma/clustering/kmeans.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/clustering/mixture.py` & `luma-ml-0.7.3/luma/clustering/mixture.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/clustering/spectral.py` & `luma-ml-0.7.3/luma/clustering/spectral.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/core/base.py` & `luma-ml-0.7.3/luma/core/base.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/core/super.py` & `luma-ml-0.7.3/luma/core/super.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     "Transformer",
     "Optimizer",
     "Evaluator",
     "Visualizer",
     "Supervised",
     "Unsupervised",
     "Distance",
-    "NeuralModel",
 )
 
 
 class Estimator(ModelBase, metaclass=ABCMeta):
     """
     An estimator is a mathematical model or algorithm
     used to make predictions or estimates based on data.
@@ -367,28 +366,7 @@
         @abstractmethod
         def compute(*args) -> float
     ```
     """
 
     @abstractmethod
     def score(*args) -> float: ...
-
-
-class NeuralModel(NeuralBase, metaclass=ABCMeta):
-    """
-    Neural networks are computational models inspired by the human brain,
-    consisting of layers of interconnected nodes (neurons) that process
-    information through weighted connections. These models include an input
-    layer to receive data, hidden layers that perform computations, and an
-    output layer to deliver results.
-    """
-
-    def __init_model__(self) -> None:
-        self.running_loss_: list[float] = []
-        self.train_loss_: list[float] = []
-        self.valid_loss_: list[float] = []
-
-    @abstractmethod
-    def train(self, **kwargs) -> list[float]: ...
-
-    @abstractmethod
-    def eval(self, **kwargs) -> list[float]: ...
```

### Comparing `luma-ml-0.7.2/luma/ensemble/bagging.py` & `luma-ml-0.7.3/luma/ensemble/bagging.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/ensemble/boost.py` & `luma-ml-0.7.3/luma/ensemble/boost.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/ensemble/forest.py` & `luma-ml-0.7.3/luma/ensemble/forest.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/ensemble/stack.py` & `luma-ml-0.7.3/luma/ensemble/stack.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/ensemble/vote.py` & `luma-ml-0.7.3/luma/ensemble/vote.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/interface/exception.py` & `luma-ml-0.7.3/luma/interface/exception.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/interface/typing.py` & `luma-ml-0.7.3/luma/interface/typing.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/interface/util.py` & `luma-ml-0.7.3/luma/interface/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -461,32 +461,32 @@
     Property
     --------
     To get an iterable object from `rich.progress.Progress`:
     ```py
     (property) progress: (self: Self@TrainProgress) -> Iterable
     ```
 
-    Exmaples
+    Examples
     --------
     Create an instance for `TrainProgress`:
-    >>> train_prog = TrainProgress(n_epochs=100)
+    >>> train_prog = TrainProgress(n_iter=100)
 
     Generate a task and update the progress bar:
     ```py
     with train_prog.progress as progress:
         train_prog.add_task(progress=progress, model=AnyModelInstance)
 
-        for epoch in range(n_epochs):
-            train_prog.update(progress=progress, cur=epoch, losses=[...])
+        for i in range(n_iter):
+            train_prog.update(progress=progress, cur=i, losses=[...])
             # losses is a list of [train_loss, valid_loss]
     ```
     """
 
-    def __init__(self, n_epochs: int, bar_width: int = 50) -> None:
-        self.n_epochs = n_epochs
+    def __init__(self, n_iter: int, bar_width: int = 50) -> None:
+        self.n_iter = n_iter
         self.bar_width = bar_width
         self.task = None
 
     @property
     def progress(self) -> Iterable:
         return Progress(
             TextColumn("[progress.description]{task.description}"),
@@ -500,16 +500,16 @@
     def _check_task_exist(self) -> None:
         if self.task is None:
             raise RuntimeError(f"'{type(self).__name__}' does not have any tasks!")
 
     def add_task(self, progress: Progress, model: object) -> None:
         self.task = progress.add_task(
             f"[purple]Start {type(model).__name__} training "
-            + f"with {self.n_epochs} epochs.",
-            total=self.n_epochs,
+            + f"with {self.n_iter} epochs.",
+            total=self.n_iter,
             train_loss=0.0,
             valid_loss=0.0,
         )
 
     def update(
         self,
         progress: Progress,
@@ -518,10 +518,10 @@
     ) -> None:
         self._check_task_exist()
         progress.update(
             self.task,
             advance=1,
             train_loss=losses[0],
             valid_loss=losses[1],
-            description=f"Epoch: {cur}/{self.n_epochs} - "
+            description=f"Epoch: {cur}/{self.n_iter} - "
             + f"Train/Valid Loss: {losses[0]:.4f}/{losses[1]:.4f}",
         )
```

### Comparing `luma-ml-0.7.2/luma/metric/classification.py` & `luma-ml-0.7.3/luma/metric/classification.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/metric/clustering.py` & `luma-ml-0.7.3/luma/metric/clustering.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/metric/distance.py` & `luma-ml-0.7.3/luma/metric/distance.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/metric/regression.py` & `luma-ml-0.7.3/luma/metric/regression.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/migrate/port.py` & `luma-ml-0.7.3/luma/migrate/port.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/model_selection/cv.py` & `luma-ml-0.7.3/luma/model_selection/cv.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/model_selection/fold.py` & `luma-ml-0.7.3/luma/model_selection/fold.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/model_selection/search.py` & `luma-ml-0.7.3/luma/model_selection/search.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/model_selection/split.py` & `luma-ml-0.7.3/luma/model_selection/split.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/neural/init.py` & `luma-ml-0.7.3/luma/neural/init.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/neural/layer.py` & `luma-ml-0.7.3/luma/neural/layer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from enum import Enum
-from typing import Any, List, Literal, Self, Tuple, Type
+from typing import Any, List, Literal, Self, Tuple, Type, override
 import numpy as np
 
 from luma.core.super import Optimizer
-from luma.interface.typing import Matrix, Tensor, ClassType
+from luma.interface.typing import Matrix, Tensor, TensorLike, ClassType
 from luma.interface.util import InitUtil, Clone
 from luma.interface.exception import UnsupportedParameterError
 from luma.neural.base import Layer
 
 
 __all__ = (
     "Convolution",
@@ -90,17 +89,19 @@
                 "filter_size": ("0<,+inf", int),
                 "stride": ("0<,+inf", int),
                 "lambda_": ("0,+inf", None),
             }
         )
         self.check_param_ranges()
 
-    def forward(self, X: Tensor) -> Tensor:
+    def forward(self, X: Tensor, is_train: bool = False) -> Tensor:
+        _ = is_train
         self.input_ = X
         batch_size, channels, height, width = X.shape
+
         if self.in_channels != channels:
             raise ValueError(
                 f"channels of 'X' does not match with 'in_channels'! "
                 + f"({self.in_channels}!={channels})"
             )
 
         pad_h, pad_w, padded_h, padded_w = self._get_padding_dim(height, width)
@@ -246,17 +247,19 @@
             {
                 "filter_size": ("0<,+inf", int),
                 "stride": ("0<,+inf", int),
             }
         )
         self.check_param_ranges()
 
-    def forward(self, X: Tensor) -> Tensor:
+    def forward(self, X: Tensor, is_train: bool = False) -> Tensor:
+        _ = is_train
         self.input_ = X
         batch_size, channels, height, width = X.shape
+
         out_height = 1 + (height - self.filter_size) // self.stride
         out_width = 1 + (width - self.filter_size) // self.stride
 
         out: Tensor = np.zeros((batch_size, channels, out_height, out_width))
         self.out_shape = out.shape
 
         for i in range(out_height):
@@ -360,15 +363,16 @@
                 "in_features": ("0<,+inf", int),
                 "out_features": ("0<,+inf", int),
                 "lambda_": ("0,+inf", None),
             }
         )
         self.check_param_ranges()
 
-    def forward(self, X: Matrix) -> Matrix:
+    def forward(self, X: Matrix, is_train: bool = False) -> Matrix:
+        _ = is_train
         self.input_ = X
 
         out = np.dot(X, self.weights_) + self.biases_
         self.out_shape = out.shape
         return out
 
     def backward(self, d_out: Matrix) -> Matrix:
@@ -438,17 +442,19 @@
     - Use this class when using `Dense` layer.
         Flatten the tensor into matrix in order to feed-forward dense layer(s).
     """
 
     def __init__(self) -> None:
         super().__init__()
 
-    def forward(self, X: Tensor) -> Matrix:
+    def forward(self, X: Tensor, is_train: bool = False) -> Matrix:
+        _ = is_train
         self.input_ = X
         out = X.reshape(X.shape[0], -1)
+
         self.out_shape = out.shape
         return out
 
     def backward(self, d_out: Matrix) -> Tensor:
         dX = d_out.reshape(self.input_.shape)
         return dX
 
@@ -479,76 +485,82 @@
 
     type FuncType = Type
 
     class Linear(Layer):
         def __init__(self) -> None:
             super().__init__()
 
-        def forward(self, X: Tensor) -> Tensor:
+        def forward(self, X: Tensor, is_train: bool = False) -> Tensor:
+            _ = is_train
             return X
 
         def backward(self, d_out: Tensor) -> Tensor:
             self.dX = d_out
             return self.dX
 
     class ReLU(Layer):
         def __init__(self) -> None:
             super().__init__()
 
-        def forward(self, X: Tensor) -> Tensor:
+        def forward(self, X: Tensor, is_train: bool = False) -> Tensor:
+            _ = is_train
             self.input_ = X
             return np.maximum(0, X)
 
         def backward(self, d_out: Tensor) -> Tensor:
             self.dX = d_out.copy()
             self.dX[self.input_ <= 0] = 0
             return self.dX
 
     class Sigmoid(Layer):
         def __init__(self) -> None:
             super().__init__()
 
-        def forward(self, X: Tensor) -> Tensor:
+        def forward(self, X: Tensor, is_train: bool = False) -> Tensor:
+            _ = is_train
             self.output_ = 1 / (1 + np.exp(-X))
             return self.output_
 
         def backward(self, d_out: Tensor) -> Tensor:
             self.dX = d_out * self.output_ * (1 - self.output_)
             return self.dX
 
     class Tanh(Layer):
         def __init__(self) -> None:
             super().__init__()
 
-        def forward(self, X: Tensor) -> Tensor:
+        def forward(self, X: Tensor, is_train: bool = False) -> Tensor:
+            _ = is_train
             self.output_ = np.tanh(X)
             return self.output_
 
         def backward(self, d_out: Tensor) -> Tensor:
             self.dX = d_out * (1 - np.square(self.output_))
             return self.dX
 
     class LeakyReLU(Layer):
         def __init__(self, alpha: float = 0.01) -> None:
             super().__init__()
             self.alpha = alpha
 
-        def forward(self, X: Tensor) -> Tensor:
+        def forward(self, X: Tensor, is_train: bool = False) -> Tensor:
+            _ = is_train
             self.input_ = X
             return np.where(X > 0, X, X * self.alpha)
 
         def backward(self, d_out: Tensor) -> Tensor:
             self.dX = d_out * np.where(self.input_ > 0, 1, self.alpha)
             return self.dX
 
     class Softmax(Layer):
         def __init__(self) -> None:
             super().__init__()
 
-        def forward(self, X: Tensor) -> Tensor:
+        def forward(self, X: Tensor, is_train: bool = False) -> Tensor:
+            _ = is_train
             e_X = np.exp(X - np.max(X, axis=-1, keepdims=True))
             return e_X / np.sum(e_X, axis=-1, keepdims=True)
 
         def backward(self, d_out: Tensor) -> Tensor:
             self.dX = np.empty_like(d_out)
             for i, (y, dy) in enumerate(zip(self.output_, d_out)):
                 y = y.reshape(-1, 1)
@@ -559,15 +571,16 @@
             return self.dX
 
     class ELU(Layer):
         def __init__(self, alpha: float = 1.0) -> None:
             super().__init__()
             self.alpha = alpha
 
-        def forward(self, X: Tensor) -> Tensor:
+        def forward(self, X: Tensor, is_train: bool = False) -> Tensor:
+            _ = is_train
             self.input_ = X
             self.output_ = np.where(X > 0, X, self.alpha * (np.exp(X) - 1))
             return self.output_
 
         def backward(self, d_out: Tensor) -> Tensor:
             self.dX = d_out * np.where(
                 self.input_ > 0,
@@ -582,15 +595,16 @@
             lambda_: float = 1.0507,
             alpha: float = 1.67326,
         ) -> None:
             super().__init__()
             self.lambda_ = lambda_
             self.alpha = alpha
 
-        def forward(self, X: Tensor) -> Tensor:
+        def forward(self, X: Tensor, is_train: bool = False) -> Tensor:
+            _ = is_train
             self.input_ = X
             self.output_ = self.lambda_ * np.where(
                 X > 0, X, self.alpha * (np.exp(X) - 1)
             )
             return self.output_
 
         def backward(self, d_out: Tensor) -> Tensor:
@@ -605,36 +619,40 @@
             )
             return self.dX
 
     class Softplus(Layer):
         def __init__(self) -> None:
             super().__init__()
 
-        def forward(self, X: Tensor) -> Tensor:
+        def forward(self, X: Tensor, is_train: bool = False) -> Tensor:
+            _ = is_train
             self.output_ = np.log1p(np.exp(X))
             return self.output_
 
         def backward(self, d_out: Tensor) -> Tensor:
             self.dX = d_out * (1 - 1 / (1 + np.exp(self.output_)))
             return self.dX
 
     class Swish(Layer):
         def __init__(self, beta: float = 1.0) -> None:
             super().__init__()
             self.beta = beta
 
-        def forward(self, X: Tensor) -> Tensor:
+        def forward(self, X: Tensor, is_train: bool = False) -> Tensor:
+            _ = is_train
             self.input_ = X
             self.sigmoid = 1 / (1 + np.exp(-self.beta * X))
+
             self.output_ = X * self.sigmoid
             return self.output_
 
         def backward(self, d_out: Tensor) -> Tensor:
             self.dX = d_out * (
-                self.sigmoid + self.input_ * self.sigmoid * (1 - self.sigmoid)
+                self.sigmoid
+                + self.beta * self.input_ * self.sigmoid * (1 - self.sigmoid)
             )
             return self.dX
 
 
 class Sequential(Layer):
     """
     Sequential represents a linear arrangement of layers in a neural network
@@ -689,58 +707,49 @@
 
     out = model(X, is_train=True) # model.forward(X, is_train=True)
     model.backward(d_out) # assume d_out is the gradient w.r.t. loss
     model.update()
     ```
     """
 
-    @ClassType.non_instantiable()
-    class LayerType(Enum):
-        ONLY_TRAIN: Tuple[Layer] = (Dropout,)
-
     def __init__(self, *layers: Layer | Tuple[str, Layer]) -> None:
+        super().__init__()
         self.layers: List[Tuple[str, Layer]] = list()
         for layer in layers:
             self.add(layer)
 
-        self.optimizer = None
-        self.loss_func_ = None
-
-    def forward(self, X: Tensor, is_train: bool = False) -> Tensor:
+    def forward(self, X: TensorLike, is_train: bool = False) -> TensorLike:
         self.input_ = X
         out = X
-
         for _, layer in self.layers:
-            if Sequential._check_only_train(layer):
-                out = layer.forward(out, is_train=is_train)
-            else:
-                out = layer.forward(out)
+            out = layer(out, is_train=is_train)
 
         self.out_shape = out.shape
         return out
 
-    def backward(self, d_out: Matrix) -> None:
+    def backward(self, d_out: TensorLike) -> TensorLike:
         for _, layer in reversed(self.layers):
             d_out = layer.backward(d_out)
+        return d_out
 
     def update(self) -> None:
         self._check_no_optimizer()
         for _, layer in reversed(self.layers):
             layer.update()
 
     def set_optimizer(self, optimizer: Optimizer, **params: Any) -> None:
         self.optimizer = optimizer
         self.optimizer.set_params(**params, ignore_missing=True)
 
         for _, layer in self.layers:
-            layer.optimizer = Clone(self.optimizer).get
-
-    @classmethod
-    def _check_only_train(cls, layer: Layer) -> bool:
-        return type(layer) in cls.LayerType.ONLY_TRAIN.value
+            cloned_opt = Clone(self.optimizer).get
+            if hasattr(layer, "set_optimizer"):
+                layer.set_optimizer(cloned_opt)
+            else:
+                layer.optimizer = cloned_opt
 
     def _check_no_optimizer(self) -> None:
         if self.optimizer is None:
             raise RuntimeError(
                 f"'{self}' has no optimizer! "
                 + f"Call '{self}().set_optimizer' to assign an optimizer."
             )
@@ -748,30 +757,26 @@
     def add(self, layer: Layer | Tuple[str, Layer]) -> None:
         if not isinstance(layer, tuple):
             layer = (str(layer), layer)
         self.layers.append(layer)
 
         if self.optimizer is not None:
             self.set_optimizer(self.optimizer)
-        if self.loss_func_ is not None:
-            self.set_loss(self.loss_func_)
 
+    @override
     @property
     def param_size(self) -> Tuple[int, int]:
         w_size, b_size = 0, 0
         for _, layer in self.layers:
             w_, b_ = layer.param_size
             w_size += w_
             b_size += b_
 
         return w_size, b_size
 
-    def __call__(self, X: Tensor, is_train: bool = False) -> float:
-        return self.forward(X, is_train=is_train)
-
     def __add__(self, other: Layer | Self) -> Self:
         if isinstance(other, Layer):
             self.add(other)
         elif isinstance(other, Self):
             for layer in other.layers:
                 self.add(layer)
         else:
@@ -781,10 +786,7 @@
                 )
             )
 
         return self
 
     def __getitem__(self, index: int) -> Tuple[str, Layer]:
         return self.layers[index]
-
-    def __str__(self) -> str:
-        return super().__str__()
```

### Comparing `luma-ml-0.7.2/luma/neural/loss.py` & `luma-ml-0.7.3/luma/neural/loss.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/neural/optimizer.py` & `luma-ml-0.7.3/luma/neural/optimizer.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/neural/single.py` & `luma-ml-0.7.3/luma/neural/single.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/pipe/pipeline.py` & `luma-ml-0.7.3/luma/pipe/pipeline.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/preprocessing/encoder.py` & `luma-ml-0.7.3/luma/preprocessing/encoder.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/preprocessing/imputer.py` & `luma-ml-0.7.3/luma/preprocessing/imputer.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/preprocessing/outlier.py` & `luma-ml-0.7.3/luma/preprocessing/outlier.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/preprocessing/scaler.py` & `luma-ml-0.7.3/luma/preprocessing/scaler.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/reduction/linear.py` & `luma-ml-0.7.3/luma/reduction/linear.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/reduction/manifold.py` & `luma-ml-0.7.3/luma/reduction/manifold.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/reduction/selection.py` & `luma-ml-0.7.3/luma/reduction/selection.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/regressor/general.py` & `luma-ml-0.7.3/luma/regressor/general.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/regressor/linear.py` & `luma-ml-0.7.3/luma/regressor/linear.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/regressor/neighbors.py` & `luma-ml-0.7.3/luma/regressor/neighbors.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/regressor/poly.py` & `luma-ml-0.7.3/luma/regressor/poly.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/regressor/robust.py` & `luma-ml-0.7.3/luma/regressor/robust.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/regressor/svm.py` & `luma-ml-0.7.3/luma/regressor/svm.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/regressor/tree.py` & `luma-ml-0.7.3/luma/regressor/tree.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/visual/eda.py` & `luma-ml-0.7.3/luma/visual/eda.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma/visual/evaluation.py` & `luma-ml-0.7.3/luma/visual/evaluation.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.2/luma_ml.egg-info/PKG-INFO` & `luma-ml-0.7.3/luma_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luma-ml
-Version: 0.7.2
+Version: 0.7.3
 Summary: A Comprehensive Python Module for Machine Learning and Data Science
 Home-page: https://github.com/ChanLumerico/luma
 Author: ChanLumerico
 Author-email: greensox284@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-5.13k-red">
+        <img src="https://img.shields.io/badge/total downloads-5.41k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -108,19 +108,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.7.2</td>
+                    <td>0.7.3</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~17.8K</td>
+                    <td>~18K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: luma-ml Version: 0.7.2 Summary: A Comprehensive
+Metadata-Version: 2.1 Name: luma-ml Version: 0.7.3 Summary: A Comprehensive
 Python Module for Machine Learning and Data Science Home-page: https://
 github.com/ChanLumerico/luma Author: ChanLumerico Author-email:
 greensox284@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.12
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy Requires-Dist: scipy Requires-Dist: pandas Requires-Dist: matplotlib
 Requires-Dist: seaborn
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-5.13k-red][GitHub code size in bytes][Code Style]
+5.41k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -33,12 +33,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.7.2
-Lines of Code  ~17.8K
+Latest Version 0.7.3
+Lines of Code  ~18K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.7.2/luma_ml.egg-info/SOURCES.txt` & `luma-ml-0.7.3/luma_ml.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -32,20 +32,23 @@
 luma/metric/regression.py
 luma/migrate/port.py
 luma/model_selection/cv.py
 luma/model_selection/fold.py
 luma/model_selection/search.py
 luma/model_selection/split.py
 luma/neural/base.py
+luma/neural/block.py
 luma/neural/init.py
 luma/neural/layer.py
 luma/neural/loss.py
 luma/neural/network.py
 luma/neural/optimizer.py
 luma/neural/single.py
+luma/neural/_models/_lenet.py
+luma/neural/_models/_simple.py
 luma/pipe/pipeline.py
 luma/preprocessing/encoder.py
 luma/preprocessing/imputer.py
 luma/preprocessing/outlier.py
 luma/preprocessing/scaler.py
 luma/reduction/linear.py
 luma/reduction/manifold.py
@@ -60,9 +63,10 @@
 luma/visual/eda.py
 luma/visual/evaluation.py
 luma_ml.egg-info/PKG-INFO
 luma_ml.egg-info/SOURCES.txt
 luma_ml.egg-info/dependency_links.txt
 luma_ml.egg-info/requires.txt
 luma_ml.egg-info/top_level.txt
+test/__act.py
 test/__local__.py
 test/__test.py
```

### Comparing `luma-ml-0.7.2/setup.py` & `luma-ml-0.7.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="luma-ml",
-    version="0.7.2",
+    version="0.7.3",
     author="ChanLumerico",
     author_email="greensox284@gmail.com",
     description="A Comprehensive Python Module for Machine Learning and Data Science",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ChanLumerico/luma",
     packages=setuptools.find_namespace_packages(),
```

