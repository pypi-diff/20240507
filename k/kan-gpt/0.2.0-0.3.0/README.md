# Comparing `tmp/kan_gpt-0.2.0.tar.gz` & `tmp/kan_gpt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kan_gpt-0.2.0.tar", last modified: Sat May  4 18:07:51 2024, max compression
+gzip compressed data, was "kan_gpt-0.3.0.tar", last modified: Tue May  7 19:30:44 2024, max compression
```

## Comparing `kan_gpt-0.2.0.tar` & `kan_gpt-0.3.0.tar`

### file list

```diff
@@ -1,68 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:07:51.580212 kan_gpt-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-05-04 18:07:51.580212 kan_gpt-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:07:51.572212 kan_gpt-0.2.0/kan_gpt/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:07:51.572212 kan_gpt-0.2.0/kan_gpt/efficient_kan/
--rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/efficient_kan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:07:51.572212 kan_gpt-0.2.0/kan_gpt/kan/
--rw-r--r--   0 runner    (1001) docker     (127)    57710 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/kan/KAN.py
--rw-r--r--   0 runner    (1001) docker     (127)    16546 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/kan/KANLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17589 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/kan/LBFGS.py
--rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/kan/Symbolic_KANLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/kan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:07:51.576212 kan_gpt-0.2.0/kan_gpt/kan/figures/
--rw-r--r--   0 runner    (1001) docker     (127)    20912 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/kan/figures/sp_0_0_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/kan/figures/sp_0_0_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/kan/figures/sp_0_0_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    24594 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/kan/figures/sp_0_0_3.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/kan/figures/sp_0_0_4.png
--rw-r--r--   0 runner    (1001) docker     (127)    20473 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/kan/figures/sp_0_1_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/kan/figures/sp_0_1_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/kan/figures/sp_0_1_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    23921 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/kan/figures/sp_0_1_3.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/kan/figures/sp_0_1_4.png
--rw-r--r--   0 runner    (1001) docker     (127)    15795 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/kan/figures/sp_1_0_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/kan/figures/sp_1_1_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/kan/figures/sp_1_2_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    19253 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/kan/figures/sp_1_3_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/kan/figures/sp_1_4_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/kan/spline.py
--rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/kan/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:07:51.576212 kan_gpt-0.2.0/kan_gpt/mingpt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/mingpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16284 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/mingpt/bpe.py
--rw-r--r--   0 runner    (1001) docker     (127)    16530 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/mingpt/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/mingpt/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/mingpt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19569 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/kan_gpt/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:07:51.576212 kan_gpt-0.2.0/kan_gpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-05-04 18:07:51.000000 kan_gpt-0.2.0/kan_gpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-04 18:07:51.000000 kan_gpt-0.2.0/kan_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 18:07:51.000000 kan_gpt-0.2.0/kan_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-04 18:07:51.000000 kan_gpt-0.2.0/kan_gpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-04 18:07:51.000000 kan_gpt-0.2.0/kan_gpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 18:07:51.000000 kan_gpt-0.2.0/kan_gpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 18:07:51.580212 kan_gpt-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:07:51.576212 kan_gpt-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/tests/test_efficient_kan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/tests/test_gpt_kan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/tests/test_gpt_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/tests/test_kan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-04 18:07:37.000000 kan_gpt-0.2.0/tests/test_train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:44.100051 kan_gpt-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-07 19:30:44.100051 kan_gpt-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:44.092052 kan_gpt-0.3.0/kan_gpt/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:44.092052 kan_gpt-0.3.0/kan_gpt/efficient_kan/
+-rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/efficient_kan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:44.096052 kan_gpt-0.3.0/kan_gpt/kan/
+-rw-r--r--   0 runner    (1001) docker     (127)    57710 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/KAN.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16546 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/KANLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17589 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/LBFGS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/Symbolic_KANLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:44.096052 kan_gpt-0.3.0/kan_gpt/kan/figures/
+-rw-r--r--   0 runner    (1001) docker     (127)    20912 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_0_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_0_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_0_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24594 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_0_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_0_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20473 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_1_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_1_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_1_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23921 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_1_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_1_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15795 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_1_0_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_1_1_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_1_2_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19253 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_1_3_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_1_4_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/spline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:44.100051 kan_gpt-0.3.0/kan_gpt/mingpt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/mingpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16284 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/mingpt/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16530 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/mingpt/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/mingpt/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/mingpt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19763 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:44.100051 kan_gpt-0.3.0/kan_gpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-07 19:30:44.000000 kan_gpt-0.3.0/kan_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-07 19:30:44.000000 kan_gpt-0.3.0/kan_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:30:44.000000 kan_gpt-0.3.0/kan_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-07 19:30:44.000000 kan_gpt-0.3.0/kan_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-07 19:30:44.000000 kan_gpt-0.3.0/kan_gpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 19:30:44.000000 kan_gpt-0.3.0/kan_gpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 19:30:44.100051 kan_gpt-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:44.100051 kan_gpt-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/tests/test_efficient_kan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/tests/test_gpt_kan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/tests/test_gpt_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/tests/test_kan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/tests/test_train.py
```

### Comparing `kan_gpt-0.2.0/HISTORY.md` & `kan_gpt-0.3.0/HISTORY.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Docs(README.md): dataset mention. [Aditya NG]
+- Feat(sweep): sweep script for getting a vast hyperparam sweep. [Aditya
+  NG]
+- Feat(tinyshakespeare): support for another dataset. [Aditya NG]
+- Test(tests/test_prompt.py): eval code. [Aditya NG]
+- Test(efficient_kan,original_kan): coverage. [Aditya NG]
+
+
+0.2.0 (2024-05-04)
+------------------
+- Release: version 0.2.0 🚀 [Aditya NG]
 - Version increment. [Aditya NG]
 - Docs(KAN_GPT.ipynb): benchmark runs between mlp and kan gpts. [Aditya
   NG]
 - Feat(train): date id of asset. [Aditya NG]
 - Feat(train,prompt): saving model after training, prompting a model
   given the saved model path. [Aditya NG]
 - Feat(kan_gpt/dataset.py): lengthwise dataset iteration. [Aditya NG]
```

### Comparing `kan_gpt-0.2.0/LICENSE` & `kan_gpt-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/PKG-INFO` & `kan_gpt-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kan_gpt
-Version: 0.2.0
+Version: 0.3.0
 Summary: Awesome kan_gpt created by AdityaNG
 Home-page: https://github.com/AdityaNG/kan-gpt/
 Author: AdityaNG
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib==3.6.2
 Requires-Dist: numpy==1.24.4
@@ -94,16 +94,16 @@
 pip install -e .
 ```
 
 ## Train
 
 Use the following dummy script to make sure everything is working as expected
 ```bash
-WANDB_MODE=offline CUDA_VISIBLE_DEVICE="" python3 -m kan_gpt.train --architecture MLP --batch_size 1 --dummy_dataset --device cpu
-WANDB_MODE=offline CUDA_VISIBLE_DEVICE="" python3 -m kan_gpt.train --architecture KAN --batch_size 1 --dummy_dataset --device cpu
+WANDB_MODE=offline CUDA_VISIBLE_DEVICE="" python3 -m kan_gpt.train --architecture MLP --batch_size 1 --dummy_dataset --device cpu --max_iters 200
+WANDB_MODE=offline CUDA_VISIBLE_DEVICE="" python3 -m kan_gpt.train --architecture KAN --batch_size 1 --dummy_dataset --device cpu --max_iters 200
 ```
 
 Then make use of the training script
 ```bash
 python -m kan_gpt.train
 ```
 
@@ -115,22 +115,26 @@
 ```
 
 ## TODOs
 
 - [x] Integrate [minGPT](https://github.com/karpathy/minGPT) and [pykan](https://github.com/KindXiaoming/pykan)
 - [x] Dataset downloading script for [WebText](https://github.com/openai/gpt-2-output-dataset)
 - [x] PyTorch Dataset parser for [WebText](https://github.com/openai/gpt-2-output-dataset)
+- [x] PyTorch Dataset parser for [tinyshakespeare](https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt)
 - [x] Mini training POC for KAN-GPT
   - [x] Integrate KAN training logic from `KAN.train_kan`
   - [x] Train a dummy batch w/o any memory issues
 - [x] Mini training POC for MLP-GPT
 - [x] Train MLP-GPT on the webtext dataset as a baseline
+- [x] Train KAN-GPT on the webtext dataset as a baseline
+- [ ] Metrics comparing KAN-GPT and MLP-GPT
 - [x] Auto Save checkpoints
 - [x] Auto Save checkpoints to W&B
 - [ ] Auto Download model weights from git / huggingface
+- [x] W&B hyperparam sweep script
 - [x] Script to load checkpoint in interactive mode
 - [ ] Training script to PyTorch Lighting
 - [x] Integrate with [efficient-kan](https://github.com/Blealtan/efficient-kan/blob/master/src/efficient_kan/kan.py)
 - [x] Test Cases
   - [x] KAN: Forward-Backward test
   - [x] GPT: Forward-Backward test
   - [x] KAN_GPT: Forward-Backward test
@@ -140,8 +144,9 @@
 
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## References
 
 - [minGPT](https://github.com/karpathy/minGPT)
 - [pykan](https://github.com/KindXiaoming/pykan)
-- [WebText](https://github.com/openai/gpt-2-output-dataset)
+- [webtext](https://github.com/openai/gpt-2-output-dataset)
+- [tinyshakespeare](https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt)
```

### Comparing `kan_gpt-0.2.0/README.md` & `kan_gpt-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -62,16 +62,16 @@
 pip install -e .
 ```
 
 ## Train
 
 Use the following dummy script to make sure everything is working as expected
 ```bash
-WANDB_MODE=offline CUDA_VISIBLE_DEVICE="" python3 -m kan_gpt.train --architecture MLP --batch_size 1 --dummy_dataset --device cpu
-WANDB_MODE=offline CUDA_VISIBLE_DEVICE="" python3 -m kan_gpt.train --architecture KAN --batch_size 1 --dummy_dataset --device cpu
+WANDB_MODE=offline CUDA_VISIBLE_DEVICE="" python3 -m kan_gpt.train --architecture MLP --batch_size 1 --dummy_dataset --device cpu --max_iters 200
+WANDB_MODE=offline CUDA_VISIBLE_DEVICE="" python3 -m kan_gpt.train --architecture KAN --batch_size 1 --dummy_dataset --device cpu --max_iters 200
 ```
 
 Then make use of the training script
 ```bash
 python -m kan_gpt.train
 ```
 
@@ -83,22 +83,26 @@
 ```
 
 ## TODOs
 
 - [x] Integrate [minGPT](https://github.com/karpathy/minGPT) and [pykan](https://github.com/KindXiaoming/pykan)
 - [x] Dataset downloading script for [WebText](https://github.com/openai/gpt-2-output-dataset)
 - [x] PyTorch Dataset parser for [WebText](https://github.com/openai/gpt-2-output-dataset)
+- [x] PyTorch Dataset parser for [tinyshakespeare](https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt)
 - [x] Mini training POC for KAN-GPT
   - [x] Integrate KAN training logic from `KAN.train_kan`
   - [x] Train a dummy batch w/o any memory issues
 - [x] Mini training POC for MLP-GPT
 - [x] Train MLP-GPT on the webtext dataset as a baseline
+- [x] Train KAN-GPT on the webtext dataset as a baseline
+- [ ] Metrics comparing KAN-GPT and MLP-GPT
 - [x] Auto Save checkpoints
 - [x] Auto Save checkpoints to W&B
 - [ ] Auto Download model weights from git / huggingface
+- [x] W&B hyperparam sweep script
 - [x] Script to load checkpoint in interactive mode
 - [ ] Training script to PyTorch Lighting
 - [x] Integrate with [efficient-kan](https://github.com/Blealtan/efficient-kan/blob/master/src/efficient_kan/kan.py)
 - [x] Test Cases
   - [x] KAN: Forward-Backward test
   - [x] GPT: Forward-Backward test
   - [x] KAN_GPT: Forward-Backward test
@@ -108,8 +112,9 @@
 
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## References
 
 - [minGPT](https://github.com/karpathy/minGPT)
 - [pykan](https://github.com/KindXiaoming/pykan)
-- [WebText](https://github.com/openai/gpt-2-output-dataset)
+- [webtext](https://github.com/openai/gpt-2-output-dataset)
+- [tinyshakespeare](https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt)
```

### Comparing `kan_gpt-0.2.0/kan_gpt/cli.py` & `kan_gpt-0.3.0/kan_gpt/cli.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/efficient_kan/model.py` & `kan_gpt-0.3.0/kan_gpt/efficient_kan/model.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/kan/KAN.py` & `kan_gpt-0.3.0/kan_gpt/kan/KAN.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/kan/KANLayer.py` & `kan_gpt-0.3.0/kan_gpt/kan/KANLayer.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/kan/LBFGS.py` & `kan_gpt-0.3.0/kan_gpt/kan/LBFGS.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/kan/Symbolic_KANLayer.py` & `kan_gpt-0.3.0/kan_gpt/kan/Symbolic_KANLayer.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/kan/figures/sp_0_0_0.png` & `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_0_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/kan/figures/sp_0_0_1.png` & `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_0_1.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/kan/figures/sp_0_0_2.png` & `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_0_2.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/kan/figures/sp_0_0_3.png` & `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_0_3.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/kan/figures/sp_0_0_4.png` & `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_0_4.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/kan/figures/sp_0_1_0.png` & `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_1_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/kan/figures/sp_0_1_1.png` & `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_1_1.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/kan/figures/sp_0_1_2.png` & `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_1_2.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/kan/figures/sp_0_1_3.png` & `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_1_3.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/kan/figures/sp_0_1_4.png` & `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_1_4.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/kan/figures/sp_1_0_0.png` & `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_1_0_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/kan/figures/sp_1_1_0.png` & `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_1_1_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/kan/figures/sp_1_2_0.png` & `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_1_2_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/kan/figures/sp_1_3_0.png` & `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_1_3_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/kan/figures/sp_1_4_0.png` & `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_1_4_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/kan/spline.py` & `kan_gpt-0.3.0/kan_gpt/kan/spline.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/kan/utils.py` & `kan_gpt-0.3.0/kan_gpt/kan/utils.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/mingpt/bpe.py` & `kan_gpt-0.3.0/kan_gpt/mingpt/bpe.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/mingpt/model.py` & `kan_gpt-0.3.0/kan_gpt/mingpt/model.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/mingpt/trainer.py` & `kan_gpt-0.3.0/kan_gpt/mingpt/trainer.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/mingpt/utils.py` & `kan_gpt-0.3.0/kan_gpt/mingpt/utils.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/model.py` & `kan_gpt-0.3.0/kan_gpt/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,18 +16,23 @@
 from torch.nn import functional as F
 
 from kan_gpt.efficient_kan.model import KAN as EFFICIENT_KAN
 from kan_gpt.kan.KAN import KAN as ORIGINAL_KAN
 from kan_gpt.mingpt.utils import CfgNode as CN
 from kan_gpt.settings import settings
 
-if settings.kan.KAN_IMPLEMENTATION == "EFFICIENT_KAN":
-    KAN = EFFICIENT_KAN  # type: ignore
-elif settings.kan.KAN_IMPLEMENTATION == "ORIGINAL_KAN":
-    KAN = ORIGINAL_KAN  # type: ignore
+
+def get_KAN():
+    if settings.kan.KAN_IMPLEMENTATION == "EFFICIENT_KAN":
+        KAN = EFFICIENT_KAN  # type: ignore
+    elif settings.kan.KAN_IMPLEMENTATION == "ORIGINAL_KAN":
+        KAN = ORIGINAL_KAN  # type: ignore
+
+    return KAN
+
 
 # -----------------------------------------------------------------------------
 
 
 class NewGELU(nn.Module):
     """
     Implementation of the GELU activation function currently in Google BERT
@@ -56,14 +61,16 @@
     the end. It is possible to use torch.nn.MultiheadAttention here but I am
     including an explicit implementation here to show that there is nothing
     too scary here.
     """
 
     def __init__(self, config):
         super().__init__()
+        KAN = get_KAN()
+
         assert config.n_embd % config.n_head == 0
         # key, query, value projections for all heads, but in a batch
         self.c_attn = KAN(width=[config.n_embd, 3 * config.n_embd])
         # output projection
         self.c_proj = KAN(width=[config.n_embd, config.n_embd])
         # regularization
         self.attn_dropout = nn.Dropout(config.attn_pdrop)
@@ -114,14 +121,15 @@
 
 
 class Block(nn.Module):
     """an unassuming Transformer block"""
 
     def __init__(self, config):
         super().__init__()
+        KAN = get_KAN()
         self.ln_1 = nn.LayerNorm(config.n_embd)
         self.attn = CausalSelfAttention(config)
         self.ln_2 = nn.LayerNorm(config.n_embd)
         self.mlp = nn.ModuleDict(
             dict(
                 c_fc=KAN(width=[config.n_embd, 4 * config.n_embd]),
                 c_proj=KAN(width=[4 * config.n_embd, config.n_embd]),
@@ -216,14 +224,15 @@
                 drop=nn.Dropout(config.embd_pdrop),
                 h=nn.ModuleList(
                     [Block(config) for _ in range(config.n_layer)]
                 ),
                 ln_f=nn.LayerNorm(config.n_embd),
             )
         )
+        KAN = get_KAN()
         self.lm_head = KAN(
             width=[config.n_embd, config.vocab_size], bias_trainable=False
         )
 
         # init all weights, and apply a special scaled init to the residual
         # projections, per GPT-2 paper
         self.apply(self._init_weights)
@@ -281,23 +290,25 @@
                 )
                 reg_ += lamb_coef * coeff_l1 + lamb_coefdiff * coeff_diff_l1
 
             return reg_
 
         total_reg = torch.tensor(0.0).to(device=x.device, dtype=torch.float32)
         size = 0
+        KAN = get_KAN()
         for mod in self.modules():
             if isinstance(mod, KAN):
                 total_reg += reg(mod)
                 size += 1
 
         mean_reg = total_reg / size
         return mean_reg
 
     def _init_weights(self, module):
+        KAN = get_KAN()
         if isinstance(module, KAN):
             # torch.nn.init.normal_(module.weight, mean=0.0, std=0.02)
             # if module.bias is not None:
             #     torch.nn.init.zeros_(module.bias)
             # TODO: init weights
             pass
         elif isinstance(module, nn.Embedding):
@@ -365,14 +376,15 @@
         weights). We are then returning the PyTorch optimizer object.
         """
 
         # separate out all parameters to those that will and won't experience
         # regularizing weight decay
         decay = set()
         no_decay = set()
+        KAN = get_KAN()
         whitelist_weight_modules = (KAN,)
         blacklist_weight_modules = (torch.nn.LayerNorm, torch.nn.Embedding)
         for mn, m in self.named_modules():
             for pn, p in m.named_parameters():
                 fpn = "%s.%s" % (mn, pn) if mn else pn  # full param name
                 # random note: because named_modules and named_parameters
                 # are recursive we will see the same tensors p many many
```

### Comparing `kan_gpt-0.2.0/kan_gpt/prompt.py` & `kan_gpt-0.3.0/kan_gpt/prompt.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/kan_gpt/train.py` & `kan_gpt-0.3.0/kan_gpt/train.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import torch
 from torch.utils.data.dataloader import DataLoader
 from wandb.sdk.lib import RunDisabled
 from wandb.sdk.wandb_run import Run
 
 import wandb
-from kan_gpt.dataset import WebTextDataset
+from kan_gpt.dataset import TinyShakespeareDataset, WebTextDataset
 from kan_gpt.mingpt.model import GPT as MLP_GPT
 from kan_gpt.mingpt.trainer import Trainer
 from kan_gpt.model import GPT as KAN_GPT
 from kan_gpt.settings import settings
 
 
 def eval_split(
@@ -58,35 +58,41 @@
         run.log_artifact(artifact)
     else:
         print("Model NOT uploaded to wandb")
 
     return save_path
 
 
-def main(args):
+def main(args, run=None):
     config = {
         "model_type": args.model_type,
         "batch_size": args.batch_size,
         "dummy_dataset": args.dummy_dataset,
         "learning_rate": args.learning_rate,
         "max_iters": args.max_iters,
         "num_workers": args.num_workers,
+        "dataset": args.dataset,
         "architecture": args.architecture,
         "device": args.device,
     }
 
     model_type = args.model_type
 
+    if args.dataset == "webtext":
+        Dataset = WebTextDataset
+    elif args.dataset == "tinyshakespeare":
+        Dataset = TinyShakespeareDataset
+
     # print an example instance of the dataset
     if args.dummy_dataset:
-        train_dataset = WebTextDataset("test", "gpt2")
+        train_dataset = Dataset("test", "gpt2")
     else:
-        train_dataset = WebTextDataset("train", "gpt2")
+        train_dataset = Dataset("train", "gpt2")
 
-    test_dataset = WebTextDataset("test", "gpt2")
+    test_dataset = Dataset("test", "gpt2")
 
     print("test_dataset: ", len(test_dataset))
     print("train_dataset: ", len(train_dataset))
 
     if args.architecture == "KAN":
         GPT = KAN_GPT
     else:
@@ -106,15 +112,16 @@
     )  # the model we're using is so small that we can go a bit faster
     train_config.max_iters = int(args.max_iters)
     train_config.num_workers = int(args.num_workers)
     train_config.batch_size = int(args.batch_size)
     train_config.device = args.device
     trainer = Trainer(train_config, model, train_dataset)
 
-    run = wandb.init(project="KAN-GPT", config=config)
+    if run is None:
+        run = wandb.init(project="KAN-GPT", config=config)
     wandb.watch(model)
 
     def batch_end_callback(trainer):
         # TODO: Add W&B Hooks
         if trainer.iter_num % 100 == 0:
             print(
                 f"iter_dt {trainer.iter_dt * 1000:.2f}ms; "
@@ -176,14 +183,19 @@
     parser.add_argument("--dummy_dataset", action="store_true")
     parser.add_argument("--learning_rate", default=5e-3)
     parser.add_argument("--max_iters", default=2000)
     parser.add_argument("--num_workers", default=0)
     parser.add_argument("--batch_size", default=64)
 
     parser.add_argument(
+        "--dataset",
+        choices=["webtext", "tinyshakespeare"],
+        default="tinyshakespeare",
+    )
+    parser.add_argument(
         "--architecture", choices=["MLP", "KAN"], default="KAN"
     )
     parser.add_argument(
         "--device", choices=["auto", "cpu", "cuda"], default="auto"
     )
 
     args = parser.parse_args()
```

### Comparing `kan_gpt-0.2.0/kan_gpt.egg-info/PKG-INFO` & `kan_gpt-0.3.0/kan_gpt.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kan_gpt
-Version: 0.2.0
+Version: 0.3.0
 Summary: Awesome kan_gpt created by AdityaNG
 Home-page: https://github.com/AdityaNG/kan-gpt/
 Author: AdityaNG
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib==3.6.2
 Requires-Dist: numpy==1.24.4
@@ -94,16 +94,16 @@
 pip install -e .
 ```
 
 ## Train
 
 Use the following dummy script to make sure everything is working as expected
 ```bash
-WANDB_MODE=offline CUDA_VISIBLE_DEVICE="" python3 -m kan_gpt.train --architecture MLP --batch_size 1 --dummy_dataset --device cpu
-WANDB_MODE=offline CUDA_VISIBLE_DEVICE="" python3 -m kan_gpt.train --architecture KAN --batch_size 1 --dummy_dataset --device cpu
+WANDB_MODE=offline CUDA_VISIBLE_DEVICE="" python3 -m kan_gpt.train --architecture MLP --batch_size 1 --dummy_dataset --device cpu --max_iters 200
+WANDB_MODE=offline CUDA_VISIBLE_DEVICE="" python3 -m kan_gpt.train --architecture KAN --batch_size 1 --dummy_dataset --device cpu --max_iters 200
 ```
 
 Then make use of the training script
 ```bash
 python -m kan_gpt.train
 ```
 
@@ -115,22 +115,26 @@
 ```
 
 ## TODOs
 
 - [x] Integrate [minGPT](https://github.com/karpathy/minGPT) and [pykan](https://github.com/KindXiaoming/pykan)
 - [x] Dataset downloading script for [WebText](https://github.com/openai/gpt-2-output-dataset)
 - [x] PyTorch Dataset parser for [WebText](https://github.com/openai/gpt-2-output-dataset)
+- [x] PyTorch Dataset parser for [tinyshakespeare](https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt)
 - [x] Mini training POC for KAN-GPT
   - [x] Integrate KAN training logic from `KAN.train_kan`
   - [x] Train a dummy batch w/o any memory issues
 - [x] Mini training POC for MLP-GPT
 - [x] Train MLP-GPT on the webtext dataset as a baseline
+- [x] Train KAN-GPT on the webtext dataset as a baseline
+- [ ] Metrics comparing KAN-GPT and MLP-GPT
 - [x] Auto Save checkpoints
 - [x] Auto Save checkpoints to W&B
 - [ ] Auto Download model weights from git / huggingface
+- [x] W&B hyperparam sweep script
 - [x] Script to load checkpoint in interactive mode
 - [ ] Training script to PyTorch Lighting
 - [x] Integrate with [efficient-kan](https://github.com/Blealtan/efficient-kan/blob/master/src/efficient_kan/kan.py)
 - [x] Test Cases
   - [x] KAN: Forward-Backward test
   - [x] GPT: Forward-Backward test
   - [x] KAN_GPT: Forward-Backward test
@@ -140,8 +144,9 @@
 
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## References
 
 - [minGPT](https://github.com/karpathy/minGPT)
 - [pykan](https://github.com/KindXiaoming/pykan)
-- [WebText](https://github.com/openai/gpt-2-output-dataset)
+- [webtext](https://github.com/openai/gpt-2-output-dataset)
+- [tinyshakespeare](https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt)
```

### Comparing `kan_gpt-0.2.0/kan_gpt.egg-info/SOURCES.txt` & `kan_gpt-0.3.0/kan_gpt.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 kan_gpt/__main__.py
 kan_gpt/base.py
 kan_gpt/cli.py
 kan_gpt/dataset.py
 kan_gpt/model.py
 kan_gpt/prompt.py
 kan_gpt/settings.py
+kan_gpt/sweep.py
 kan_gpt/train.py
 kan_gpt.egg-info/PKG-INFO
 kan_gpt.egg-info/SOURCES.txt
 kan_gpt.egg-info/dependency_links.txt
 kan_gpt.egg-info/entry_points.txt
 kan_gpt.egg-info/requires.txt
 kan_gpt.egg-info/top_level.txt
@@ -51,8 +52,9 @@
 tests/__init__.py
 tests/conftest.py
 tests/test_base.py
 tests/test_efficient_kan.py
 tests/test_gpt_kan.py
 tests/test_gpt_mlp.py
 tests/test_kan.py
+tests/test_prompt.py
 tests/test_train.py
```

### Comparing `kan_gpt-0.2.0/setup.py` & `kan_gpt-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/tests/test_efficient_kan.py` & `kan_gpt-0.3.0/tests/test_efficient_kan.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.2.0/tests/test_gpt_kan.py` & `kan_gpt-0.3.0/tests/test_kan.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,73 @@
 import torch
-from kan_gpt.model import GPT as KAN_GPT
-
-VOCAB_SIZE = 8
-BLOCK_SIZE = 16
-MODEL_TYPE = "gpt-pico"
-
-
-def get_gpt_model() -> KAN_GPT:
-    model_config = KAN_GPT.get_default_config()
-    model_config.model_type = MODEL_TYPE
-    model_config.vocab_size = VOCAB_SIZE
-    model_config.block_size = BLOCK_SIZE
-    model = KAN_GPT(model_config)
-    return model
+from kan_gpt.kan.KAN import KAN
 
 
 def test_forward():
     with torch.no_grad():
-        model = get_gpt_model()
-        x = torch.zeros((1, BLOCK_SIZE), dtype=torch.long)
+        model = KAN(width=[2, 5, 2])
+        x = torch.zeros((1, 1, 2), dtype=torch.float32)
 
-        y, loss = model.forward(x)
+        y = model.forward(x)
 
-        assert y.shape == (
-            1,
-            BLOCK_SIZE,
-            VOCAB_SIZE,
-        ), f"Shape mismatch: {y.shape}"
+        assert y.shape == (1, 1, 2), f"Shape mismatch: {y.shape}"
 
 
 def test_backward():
-    model = get_gpt_model()
-    x = torch.zeros((1, BLOCK_SIZE), dtype=torch.long)
-    y_gt = torch.zeros((1, BLOCK_SIZE), dtype=torch.long)
+    model = KAN(width=[2, 5, 2])
+    x = torch.zeros((1, 1, 2), dtype=torch.float32)
 
     # Make sure grads exist
     requires_grad_set = set()
     for param in model.parameters():
         if param.requires_grad:
             requires_grad_set.add(param)
     assert len(requires_grad_set) > 0, "requires_grad is not set"
 
-    y, loss = model.forward(x, y_gt)
+    y = model.forward(x)
 
-    assert y.shape == (1, BLOCK_SIZE, VOCAB_SIZE), f"Shape mismatch: {y.shape}"
+    assert y.shape == (1, 1, 2), f"Shape mismatch: {y.shape}"
 
+    loss = y.mean()
     loss.backward()
 
     # Make sure grads exist
     grad_set = set()
     for param in model.parameters():
         if isinstance(param.grad, torch.Tensor):
             grad_set.add(param)
     assert len(grad_set) > 0, f"Tensor.grad missing"
 
 
 def test_forward_batched():
     with torch.no_grad():
-        model = get_gpt_model()
-        x = torch.zeros((2, BLOCK_SIZE), dtype=torch.long)
+        model = KAN(width=[2, 5, 2])
+        x = torch.zeros((2, 1, 2), dtype=torch.float32)
 
-        y, loss = model.forward(x)
+        y = model.forward(x)
 
-        assert y.shape == (
-            2,
-            BLOCK_SIZE,
-            VOCAB_SIZE,
-        ), f"Shape mismatch: {y.shape}"
+        assert y.shape == (2, 1, 2), f"Shape mismatch: {y.shape}"
 
 
 def test_backward_batched():
-    model = get_gpt_model()
-    x = torch.zeros((2, BLOCK_SIZE), dtype=torch.long)
-    y_gt = torch.zeros((2, BLOCK_SIZE), dtype=torch.long)
+    model = KAN(width=[2, 5, 2])
+    x = torch.zeros((2, 1, 2), dtype=torch.float32)
 
     # Make sure grads exist
     requires_grad_set = set()
     for param in model.parameters():
         if param.requires_grad:
             requires_grad_set.add(param)
     assert len(requires_grad_set) > 0, "requires_grad is not set"
 
-    y, loss = model.forward(x, y_gt)
+    y = model.forward(x)
 
-    assert y.shape == (2, BLOCK_SIZE, VOCAB_SIZE), f"Shape mismatch: {y.shape}"
+    assert y.shape == (2, 1, 2), f"Shape mismatch: {y.shape}"
 
+    loss = y.mean()
     loss.backward()
 
     # Make sure grads exist
     grad_set = set()
     for param in model.parameters():
         if isinstance(param.grad, torch.Tensor):
             grad_set.add(param)
```

### Comparing `kan_gpt-0.2.0/tests/test_gpt_mlp.py` & `kan_gpt-0.3.0/tests/test_gpt_mlp.py`

 * *Files identical despite different names*

