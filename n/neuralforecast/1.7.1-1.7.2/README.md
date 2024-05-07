# Comparing `tmp/neuralforecast-1.7.1.tar.gz` & `tmp/neuralforecast-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralforecast-1.7.1.tar", last modified: Thu Apr 11 00:17:20 2024, max compression
+gzip compressed data, was "neuralforecast-1.7.2.tar", last modified: Tue May  7 16:36:55 2024, max compression
```

## Comparing `neuralforecast-1.7.1.tar` & `neuralforecast-1.7.2.tar`

### file list

```diff
@@ -1,67 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:17:20.670120 neuralforecast-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16125 2024-04-11 00:17:20.670120 neuralforecast-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14456 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:17:20.658120 neuralforecast-1.7.1/neuralforecast/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   176475 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (127)    59758 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/auto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:17:20.662120 neuralforecast-1.7.1/neuralforecast/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17381 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/common/_base_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)    12285 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/common/_base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    21416 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/common/_base_multivariate.py
--rw-r--r--   0 runner    (1001) docker     (127)    22755 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/common/_base_recurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    27930 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/common/_base_windows.py
--rw-r--r--   0 runner    (1001) docker     (127)    15003 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/common/_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    18531 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/common/_scalers.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    53238 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:17:20.662120 neuralforecast-1.7.1/neuralforecast/losses/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15633 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/losses/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    84578 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/losses/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:17:20.670120 neuralforecast-1.7.1/neuralforecast/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26697 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/autoformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/bitcn.py
--rw-r--r--   0 runner    (1001) docker     (127)    22226 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/deepar.py
--rw-r--r--   0 runner    (1001) docker     (127)    18805 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/dilated_rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/dlinear.py
--rw-r--r--   0 runner    (1001) docker     (127)    26074 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/fedformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9120 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/gru.py
--rw-r--r--   0 runner    (1001) docker     (127)    11380 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/hint.py
--rw-r--r--   0 runner    (1001) docker     (127)    17307 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/informer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11112 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/itransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/mlpmultivariate.py
--rw-r--r--   0 runner    (1001) docker     (127)    17376 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/nbeats.py
--rw-r--r--   0 runner    (1001) docker     (127)    22410 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/nbeatsx.py
--rw-r--r--   0 runner    (1001) docker     (127)    17853 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/nhits.py
--rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/nlinear.py
--rw-r--r--   0 runner    (1001) docker     (127)    36647 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/patchtst.py
--rw-r--r--   0 runner    (1001) docker     (127)     9175 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    15056 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/stemgnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/tcn.py
--rw-r--r--   0 runner    (1001) docker     (127)    23669 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/tft.py
--rw-r--r--   0 runner    (1001) docker     (127)    20157 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/timellm.py
--rw-r--r--   0 runner    (1001) docker     (127)    12625 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/timesnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/tsmixer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17293 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/tsmixerx.py
--rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/vanillatransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16128 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/tsdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    12581 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:17:20.670120 neuralforecast-1.7.1/neuralforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16125 2024-04-11 00:17:20.000000 neuralforecast-1.7.1/neuralforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-11 00:17:20.000000 neuralforecast-1.7.1/neuralforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 00:17:20.000000 neuralforecast-1.7.1/neuralforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-11 00:17:20.000000 neuralforecast-1.7.1/neuralforecast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 00:17:20.000000 neuralforecast-1.7.1/neuralforecast.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-11 00:17:20.000000 neuralforecast-1.7.1/neuralforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 00:17:20.000000 neuralforecast-1.7.1/neuralforecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/settings.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 00:17:20.670120 neuralforecast-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:36:55.275712 neuralforecast-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16125 2024-05-07 16:36:55.275712 neuralforecast-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14456 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:36:55.263712 neuralforecast-1.7.2/neuralforecast/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   180134 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64387 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/auto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:36:55.267712 neuralforecast-1.7.2/neuralforecast/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17375 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/common/_base_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/common/_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21636 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/common/_base_multivariate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22826 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/common/_base_recurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28177 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/common/_base_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15003 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/common/_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18565 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/common/_scalers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54452 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:36:55.267712 neuralforecast-1.7.2/neuralforecast/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15633 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/losses/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84603 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/losses/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:36:55.271712 neuralforecast-1.7.2/neuralforecast/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26697 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/autoformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/bitcn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22469 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/deepar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10072 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/deepnpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18805 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/dilated_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/dlinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26074 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/fedformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9120 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/gru.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11380 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/hint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17307 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/informer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11112 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/itransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/mlpmultivariate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17663 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/nbeats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22410 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/nbeatsx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17853 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/nhits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/nlinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36647 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/patchtst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9175 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15056 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/stemgnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/tcn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23669 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/tft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12648 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/tide.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20157 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/timellm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12625 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/timesnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/tsmixer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17293 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/tsmixerx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/models/vanillatransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16381 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/tsdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12581 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/neuralforecast/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:36:55.271712 neuralforecast-1.7.2/neuralforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16125 2024-05-07 16:36:55.000000 neuralforecast-1.7.2/neuralforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-07 16:36:55.000000 neuralforecast-1.7.2/neuralforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 16:36:55.000000 neuralforecast-1.7.2/neuralforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-07 16:36:55.000000 neuralforecast-1.7.2/neuralforecast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 16:36:55.000000 neuralforecast-1.7.2/neuralforecast.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-07 16:36:55.000000 neuralforecast-1.7.2/neuralforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-07 16:36:55.000000 neuralforecast-1.7.2/neuralforecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 16:36:55.275712 neuralforecast-1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-07 16:36:51.000000 neuralforecast-1.7.2/setup.py
```

### Comparing `neuralforecast-1.7.1/LICENSE` & `neuralforecast-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/PKG-INFO` & `neuralforecast-1.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralforecast
-Version: 1.7.1
+Version: 1.7.2
 Summary: Time series forecasting suite using deep learning models
 Home-page: https://github.com/Nixtla/neuralforecast/
 Author: Nixtla
 Author-email: business@nixtla.io
 License: Apache Software License 2.0
 Keywords: time-series forecasting deep-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `neuralforecast-1.7.1/README.md` & `neuralforecast-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/_modidx.py` & `neuralforecast-1.7.2/neuralforecast/_modidx.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,19 @@
                                      'neuralforecast.auto.AutoDLinear.get_default_config': ( 'models.html#autodlinear.get_default_config',
                                                                                              'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoDeepAR': ('models.html#autodeepar', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoDeepAR.__init__': ( 'models.html#autodeepar.__init__',
                                                                                   'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoDeepAR.get_default_config': ( 'models.html#autodeepar.get_default_config',
                                                                                             'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoDeepNPTS': ('models.html#autodeepnpts', 'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoDeepNPTS.__init__': ( 'models.html#autodeepnpts.__init__',
+                                                                                    'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoDeepNPTS.get_default_config': ( 'models.html#autodeepnpts.get_default_config',
+                                                                                              'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoDilatedRNN': ('models.html#autodilatedrnn', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoDilatedRNN.__init__': ( 'models.html#autodilatedrnn.__init__',
                                                                                       'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoDilatedRNN.get_default_config': ( 'models.html#autodilatedrnn.get_default_config',
                                                                                                 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoFEDformer': ('models.html#autofedformer', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoFEDformer.__init__': ( 'models.html#autofedformer.__init__',
@@ -110,14 +115,18 @@
                                      'neuralforecast.auto.AutoTSMixer.get_default_config': ( 'models.html#autotsmixer.get_default_config',
                                                                                              'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoTSMixerx': ('models.html#autotsmixerx', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoTSMixerx.__init__': ( 'models.html#autotsmixerx.__init__',
                                                                                     'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoTSMixerx.get_default_config': ( 'models.html#autotsmixerx.get_default_config',
                                                                                               'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoTiDE': ('models.html#autotide', 'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoTiDE.__init__': ('models.html#autotide.__init__', 'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoTiDE.get_default_config': ( 'models.html#autotide.get_default_config',
+                                                                                          'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoTimesNet': ('models.html#autotimesnet', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoTimesNet.__init__': ( 'models.html#autotimesnet.__init__',
                                                                                     'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoTimesNet.get_default_config': ( 'models.html#autotimesnet.get_default_config',
                                                                                               'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoVanillaTransformer': ( 'models.html#autovanillatransformer',
                                                                                      'neuralforecast/auto.py'),
@@ -504,14 +513,20 @@
                                                                                                     'neuralforecast/models/deepar.py'),
                                               'neuralforecast.models.deepar.DeepAR.train_forward': ( 'models.deepar.html#deepar.train_forward',
                                                                                                      'neuralforecast/models/deepar.py'),
                                               'neuralforecast.models.deepar.DeepAR.training_step': ( 'models.deepar.html#deepar.training_step',
                                                                                                      'neuralforecast/models/deepar.py'),
                                               'neuralforecast.models.deepar.DeepAR.validation_step': ( 'models.deepar.html#deepar.validation_step',
                                                                                                        'neuralforecast/models/deepar.py')},
+            'neuralforecast.models.deepnpts': { 'neuralforecast.models.deepnpts.DeepNPTS': ( 'models.deepnpts.html#deepnpts',
+                                                                                             'neuralforecast/models/deepnpts.py'),
+                                                'neuralforecast.models.deepnpts.DeepNPTS.__init__': ( 'models.deepnpts.html#deepnpts.__init__',
+                                                                                                      'neuralforecast/models/deepnpts.py'),
+                                                'neuralforecast.models.deepnpts.DeepNPTS.forward': ( 'models.deepnpts.html#deepnpts.forward',
+                                                                                                     'neuralforecast/models/deepnpts.py')},
             'neuralforecast.models.dilated_rnn': { 'neuralforecast.models.dilated_rnn.AttentiveLSTMLayer': ( 'models.dilated_rnn.html#attentivelstmlayer',
                                                                                                              'neuralforecast/models/dilated_rnn.py'),
                                                    'neuralforecast.models.dilated_rnn.AttentiveLSTMLayer.__init__': ( 'models.dilated_rnn.html#attentivelstmlayer.__init__',
                                                                                                                       'neuralforecast/models/dilated_rnn.py'),
                                                    'neuralforecast.models.dilated_rnn.AttentiveLSTMLayer.forward': ( 'models.dilated_rnn.html#attentivelstmlayer.forward',
                                                                                                                      'neuralforecast/models/dilated_rnn.py'),
                                                    'neuralforecast.models.dilated_rnn.DRNN': ( 'models.dilated_rnn.html#drnn',
@@ -1017,14 +1032,25 @@
                                                                                                         'neuralforecast/models/tft.py'),
                                            'neuralforecast.models.tft.VariableSelectionNetwork': ( 'models.tft.html#variableselectionnetwork',
                                                                                                    'neuralforecast/models/tft.py'),
                                            'neuralforecast.models.tft.VariableSelectionNetwork.__init__': ( 'models.tft.html#variableselectionnetwork.__init__',
                                                                                                             'neuralforecast/models/tft.py'),
                                            'neuralforecast.models.tft.VariableSelectionNetwork.forward': ( 'models.tft.html#variableselectionnetwork.forward',
                                                                                                            'neuralforecast/models/tft.py')},
+            'neuralforecast.models.tide': { 'neuralforecast.models.tide.MLPResidual': ( 'models.tide.html#mlpresidual',
+                                                                                        'neuralforecast/models/tide.py'),
+                                            'neuralforecast.models.tide.MLPResidual.__init__': ( 'models.tide.html#mlpresidual.__init__',
+                                                                                                 'neuralforecast/models/tide.py'),
+                                            'neuralforecast.models.tide.MLPResidual.forward': ( 'models.tide.html#mlpresidual.forward',
+                                                                                                'neuralforecast/models/tide.py'),
+                                            'neuralforecast.models.tide.TiDE': ('models.tide.html#tide', 'neuralforecast/models/tide.py'),
+                                            'neuralforecast.models.tide.TiDE.__init__': ( 'models.tide.html#tide.__init__',
+                                                                                          'neuralforecast/models/tide.py'),
+                                            'neuralforecast.models.tide.TiDE.forward': ( 'models.tide.html#tide.forward',
+                                                                                         'neuralforecast/models/tide.py')},
             'neuralforecast.models.timellm': { 'neuralforecast.models.timellm.FlattenHead': ( 'models.timellm.html#flattenhead',
                                                                                               'neuralforecast/models/timellm.py'),
                                                'neuralforecast.models.timellm.FlattenHead.__init__': ( 'models.timellm.html#flattenhead.__init__',
                                                                                                        'neuralforecast/models/timellm.py'),
                                                'neuralforecast.models.timellm.FlattenHead.forward': ( 'models.timellm.html#flattenhead.forward',
                                                                                                       'neuralforecast/models/timellm.py'),
                                                'neuralforecast.models.timellm.Normalize': ( 'models.timellm.html#normalize',
@@ -1205,14 +1231,16 @@
                                                                                                       'neuralforecast/tsdataset.py'),
                                           'neuralforecast.tsdataset.TimeSeriesDataset.__init__': ( 'tsdataset.html#timeseriesdataset.__init__',
                                                                                                    'neuralforecast/tsdataset.py'),
                                           'neuralforecast.tsdataset.TimeSeriesDataset.__len__': ( 'tsdataset.html#timeseriesdataset.__len__',
                                                                                                   'neuralforecast/tsdataset.py'),
                                           'neuralforecast.tsdataset.TimeSeriesDataset.__repr__': ( 'tsdataset.html#timeseriesdataset.__repr__',
                                                                                                    'neuralforecast/tsdataset.py'),
+                                          'neuralforecast.tsdataset.TimeSeriesDataset._as_torch_copy': ( 'tsdataset.html#timeseriesdataset._as_torch_copy',
+                                                                                                         'neuralforecast/tsdataset.py'),
                                           'neuralforecast.tsdataset.TimeSeriesDataset.align': ( 'tsdataset.html#timeseriesdataset.align',
                                                                                                 'neuralforecast/tsdataset.py'),
                                           'neuralforecast.tsdataset.TimeSeriesDataset.append': ( 'tsdataset.html#timeseriesdataset.append',
                                                                                                  'neuralforecast/tsdataset.py'),
                                           'neuralforecast.tsdataset.TimeSeriesDataset.from_df': ( 'tsdataset.html#timeseriesdataset.from_df',
                                                                                                   'neuralforecast/tsdataset.py'),
                                           'neuralforecast.tsdataset.TimeSeriesDataset.trim_dataset': ( 'tsdataset.html#timeseriesdataset.trim_dataset',
```

### Comparing `neuralforecast-1.7.1/neuralforecast/auto.py` & `neuralforecast-1.7.2/neuralforecast/auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/models.ipynb.
 
 # %% auto 0
 __all__ = ['AutoRNN', 'AutoLSTM', 'AutoGRU', 'AutoTCN', 'AutoDeepAR', 'AutoDilatedRNN', 'AutoBiTCN', 'AutoMLP', 'AutoNBEATS',
-           'AutoNBEATSx', 'AutoNHITS', 'AutoDLinear', 'AutoNLinear', 'AutoTFT', 'AutoVanillaTransformer',
-           'AutoInformer', 'AutoAutoformer', 'AutoFEDformer', 'AutoPatchTST', 'AutoiTransformer', 'AutoTimesNet',
-           'AutoStemGNN', 'AutoHINT', 'AutoTSMixer', 'AutoTSMixerx', 'AutoMLPMultivariate']
+           'AutoNBEATSx', 'AutoNHITS', 'AutoDLinear', 'AutoNLinear', 'AutoTiDE', 'AutoDeepNPTS', 'AutoTFT',
+           'AutoVanillaTransformer', 'AutoInformer', 'AutoAutoformer', 'AutoFEDformer', 'AutoPatchTST',
+           'AutoiTransformer', 'AutoTimesNet', 'AutoStemGNN', 'AutoHINT', 'AutoTSMixer', 'AutoTSMixerx',
+           'AutoMLPMultivariate']
 
 # %% ../nbs/models.ipynb 2
 from os import cpu_count
 import torch
 
 from ray import tune
 from ray.tune.search.basic_variant import BasicVariantGenerator
@@ -26,14 +27,16 @@
 
 from .models.mlp import MLP
 from .models.nbeats import NBEATS
 from .models.nbeatsx import NBEATSx
 from .models.nhits import NHITS
 from .models.dlinear import DLinear
 from .models.nlinear import NLinear
+from .models.tide import TiDE
+from .models.deepnpts import DeepNPTS
 
 from .models.tft import TFT
 from .models.vanillatransformer import VanillaTransformer
 from .models.informer import Informer
 from .models.autoformer import Autoformer
 from .models.fedformer import FEDformer
 from .models.patchtst import PatchTST
@@ -954,15 +957,158 @@
         config["step_size"] = tune.choice([1, h])
         del config["input_size_multiplier"]
         if backend == "optuna":
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 67
+# %% ../nbs/models.ipynb 66
+class AutoTiDE(BaseAuto):
+
+    default_config = {
+        "input_size_multiplier": [1, 2, 3, 4, 5],
+        "h": None,
+        "hidden_size": tune.choice([256, 512, 1024]),
+        "decoder_output_dim": tune.choice([8, 16, 32]),
+        "temporal_decoder_dim": tune.choice([32, 64, 128]),
+        "num_encoder_layers": tune.choice([1, 2, 3]),
+        "num_decoder_layers": tune.choice([1, 2, 3]),
+        "temporal_width": tune.choice([4, 8, 16]),
+        "dropout": tune.choice([0.0, 0.1, 0.2, 0.3, 0.5]),
+        "layernorm": tune.choice([True, False]),
+        "learning_rate": tune.loguniform(1e-5, 1e-2),
+        "scaler_type": tune.choice([None, "robust", "standard"]),
+        "max_steps": tune.quniform(lower=500, upper=1500, q=100),
+        "batch_size": tune.choice([32, 64, 128, 256]),
+        "windows_batch_size": tune.choice([128, 256, 512, 1024]),
+        "loss": None,
+        "random_seed": tune.randint(lower=1, upper=20),
+    }
+
+    def __init__(
+        self,
+        h,
+        loss=MAE(),
+        valid_loss=None,
+        config=None,
+        search_alg=BasicVariantGenerator(random_state=1),
+        num_samples=10,
+        refit_with_val=False,
+        cpus=cpu_count(),
+        gpus=torch.cuda.device_count(),
+        verbose=False,
+        alias=None,
+        backend="ray",
+        callbacks=None,
+    ):
+
+        # Define search space, input/output sizes
+        if config is None:
+            config = self.get_default_config(h=h, backend=backend)
+
+        super(AutoTiDE, self).__init__(
+            cls_model=TiDE,
+            h=h,
+            loss=loss,
+            valid_loss=valid_loss,
+            config=config,
+            search_alg=search_alg,
+            num_samples=num_samples,
+            refit_with_val=refit_with_val,
+            cpus=cpus,
+            gpus=gpus,
+            verbose=verbose,
+            alias=alias,
+            backend=backend,
+            callbacks=callbacks,
+        )
+
+    @classmethod
+    def get_default_config(cls, h, backend, n_series=None):
+        config = cls.default_config.copy()
+        config["input_size"] = tune.choice(
+            [h * x for x in config["input_size_multiplier"]]
+        )
+        config["step_size"] = tune.choice([1, h])
+        del config["input_size_multiplier"]
+        if backend == "optuna":
+            config = cls._ray_config_to_optuna(config)
+
+        return config
+
+# %% ../nbs/models.ipynb 70
+class AutoDeepNPTS(BaseAuto):
+
+    default_config = {
+        "input_size_multiplier": [1, 2, 3, 4, 5],
+        "h": None,
+        "hidden_size": tune.choice([16, 32, 64]),
+        "dropout": tune.uniform(0.0, 0.99),
+        "n_layers": tune.choice([1, 2, 4]),
+        "learning_rate": tune.loguniform(1e-4, 1e-1),
+        "scaler_type": tune.choice([None, "robust", "standard"]),
+        "max_steps": tune.quniform(lower=500, upper=1500, q=100),
+        "batch_size": tune.choice([32, 64, 128, 256]),
+        "windows_batch_size": tune.choice([128, 256, 512, 1024]),
+        "loss": None,
+        "random_seed": tune.randint(lower=1, upper=20),
+    }
+
+    def __init__(
+        self,
+        h,
+        loss=MAE(),
+        valid_loss=None,
+        config=None,
+        search_alg=BasicVariantGenerator(random_state=1),
+        num_samples=10,
+        refit_with_val=False,
+        cpus=cpu_count(),
+        gpus=torch.cuda.device_count(),
+        verbose=False,
+        alias=None,
+        backend="ray",
+        callbacks=None,
+    ):
+
+        # Define search space, input/output sizes
+        if config is None:
+            config = self.get_default_config(h=h, backend=backend)
+
+        super(AutoDeepNPTS, self).__init__(
+            cls_model=DeepNPTS,
+            h=h,
+            loss=loss,
+            valid_loss=valid_loss,
+            config=config,
+            search_alg=search_alg,
+            num_samples=num_samples,
+            refit_with_val=refit_with_val,
+            cpus=cpus,
+            gpus=gpus,
+            verbose=verbose,
+            alias=alias,
+            backend=backend,
+            callbacks=callbacks,
+        )
+
+    @classmethod
+    def get_default_config(cls, h, backend, n_series=None):
+        config = cls.default_config.copy()
+        config["input_size"] = tune.choice(
+            [h * x for x in config["input_size_multiplier"]]
+        )
+        config["step_size"] = tune.choice([1, h])
+        del config["input_size_multiplier"]
+        if backend == "optuna":
+            config = cls._ray_config_to_optuna(config)
+
+        return config
+
+# %% ../nbs/models.ipynb 75
 class AutoTFT(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "hidden_size": tune.choice([64, 128, 256]),
         "n_head": tune.choice([4, 8]),
@@ -1022,15 +1168,15 @@
         config["step_size"] = tune.choice([1, h])
         del config["input_size_multiplier"]
         if backend == "optuna":
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 71
+# %% ../nbs/models.ipynb 79
 class AutoVanillaTransformer(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "hidden_size": tune.choice([64, 128, 256]),
         "n_head": tune.choice([4, 8]),
@@ -1090,15 +1236,15 @@
         config["step_size"] = tune.choice([1, h])
         del config["input_size_multiplier"]
         if backend == "optuna":
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 75
+# %% ../nbs/models.ipynb 83
 class AutoInformer(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "hidden_size": tune.choice([64, 128, 256]),
         "n_head": tune.choice([4, 8]),
@@ -1158,15 +1304,15 @@
         config["step_size"] = tune.choice([1, h])
         del config["input_size_multiplier"]
         if backend == "optuna":
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 79
+# %% ../nbs/models.ipynb 87
 class AutoAutoformer(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "hidden_size": tune.choice([64, 128, 256]),
         "n_head": tune.choice([4, 8]),
@@ -1226,15 +1372,15 @@
         config["step_size"] = tune.choice([1, h])
         del config["input_size_multiplier"]
         if backend == "optuna":
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 83
+# %% ../nbs/models.ipynb 91
 class AutoFEDformer(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "hidden_size": tune.choice([64, 128, 256]),
         "learning_rate": tune.loguniform(1e-4, 1e-1),
@@ -1293,15 +1439,15 @@
         config["step_size"] = tune.choice([1, h])
         del config["input_size_multiplier"]
         if backend == "optuna":
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 87
+# %% ../nbs/models.ipynb 95
 class AutoPatchTST(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3],
         "h": None,
         "hidden_size": tune.choice([16, 128, 256]),
         "n_heads": tune.choice([4, 16]),
@@ -1363,15 +1509,15 @@
         config["step_size"] = tune.choice([1, h])
         del config["input_size_multiplier"]
         if backend == "optuna":
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 91
+# %% ../nbs/models.ipynb 99
 class AutoiTransformer(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "n_series": None,
         "hidden_size": tune.choice([64, 128, 256]),
@@ -1448,15 +1594,15 @@
         if backend == "optuna":
             # Always use n_series from parameters
             config["n_series"] = n_series
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 96
+# %% ../nbs/models.ipynb 104
 class AutoTimesNet(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "hidden_size": tune.choice([32, 64, 128]),
         "conv_hidden_size": tune.choice([32, 64, 128]),
@@ -1516,15 +1662,15 @@
         config["step_size"] = tune.choice([1, h])
         del config["input_size_multiplier"]
         if backend == "optuna":
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 101
+# %% ../nbs/models.ipynb 109
 class AutoStemGNN(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4],
         "h": None,
         "n_series": None,
         "n_stacks": tune.choice([2]),
@@ -1601,15 +1747,15 @@
         if backend == "optuna":
             # Always use n_series from parameters
             config["n_series"] = n_series
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 105
+# %% ../nbs/models.ipynb 113
 class AutoHINT(BaseAuto):
 
     def __init__(
         self,
         cls_model,
         h,
         loss,
@@ -1673,15 +1819,15 @@
         )
         return model
 
     @classmethod
     def get_default_config(cls, h, backend, n_series=None):
         raise Exception("AutoHINT has no default configuration.")
 
-# %% ../nbs/models.ipynb 110
+# %% ../nbs/models.ipynb 118
 class AutoTSMixer(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4],
         "h": None,
         "n_series": None,
         "n_block": tune.choice([1, 2, 4, 6, 8]),
@@ -1759,15 +1905,15 @@
         if backend == "optuna":
             # Always use n_series from parameters
             config["n_series"] = n_series
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 114
+# %% ../nbs/models.ipynb 122
 class AutoTSMixerx(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4],
         "h": None,
         "n_series": None,
         "n_block": tune.choice([1, 2, 4, 6, 8]),
@@ -1845,15 +1991,15 @@
         if backend == "optuna":
             # Always use n_series from parameters
             config["n_series"] = n_series
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 118
+# %% ../nbs/models.ipynb 126
 class AutoMLPMultivariate(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "n_series": None,
         "hidden_size": tune.choice([256, 512, 1024]),
```

### Comparing `neuralforecast-1.7.1/neuralforecast/common/_base_auto.py` & `neuralforecast-1.7.2/neuralforecast/common/_base_auto.py`

 * *Files 0% similar despite different names*

```diff
@@ -421,15 +421,15 @@
                 distributed_config=distributed_config,
             )
             best_config = results.best_trial.user_attrs["ALL_PARAMS"]
         self.model = self._fit_model(
             cls_model=self.cls_model,
             config=best_config,
             dataset=dataset,
-            val_size=val_size * (1 - self.refit_with_val),
+            val_size=val_size * self.refit_with_val,
             test_size=test_size,
             distributed_config=distributed_config,
         )
         self.results = results
 
         # Added attributes for compatibility with NeuralForecast core
         self.futr_exog_list = self.model.futr_exog_list
```

### Comparing `neuralforecast-1.7.1/neuralforecast/common/_base_model.py` & `neuralforecast-1.7.2/neuralforecast/common/_base_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,15 +74,19 @@
         hist_exog_list,
         stat_exog_list,
         max_steps,
         early_stop_patience_steps,
         **trainer_kwargs,
     ):
         super().__init__()
-        self.save_hyperparameters()  # Allows instantiation from a checkpoint from class
+        with warnings.catch_warnings(record=False):
+            warnings.filterwarnings("ignore")
+            # the following line issues a warning about the loss attribute being saved
+            # but we do want to save it
+            self.save_hyperparameters()  # Allows instantiation from a checkpoint from class
         self.random_seed = random_seed
         pl.seed_everything(self.random_seed, workers=True)
 
         # Loss
         self.loss = loss
         if valid_loss is None:
             self.valid_loss = loss
@@ -198,16 +202,16 @@
             num_workers=self.num_workers_loader,
             drop_last=self.drop_last_loader,
             shuffle_train=shuffle_train,
         )
 
         if self.val_check_steps > self.max_steps:
             warnings.warn(
-                "val_check_steps is greater than max_steps, \
-                    setting val_check_steps to max_steps"
+                "val_check_steps is greater than max_steps, "
+                "setting val_check_steps to max_steps."
             )
         val_check_interval = min(self.val_check_steps, self.max_steps)
         self.trainer_kwargs["val_check_interval"] = int(val_check_interval)
         self.trainer_kwargs["check_val_every_n_epoch"] = None
 
         if is_local:
             model = self
@@ -316,17 +320,23 @@
 
     def set_test_size(self, test_size):
         self.test_size = test_size
 
     def on_validation_epoch_end(self):
         if self.val_size == 0:
             return
-        avg_loss = torch.stack(self.validation_step_outputs).mean()
-        self.log("ptl/val_loss", avg_loss, sync_dist=True)
-        self.valid_trajectories.append((self.global_step, float(avg_loss)))
+        losses = torch.stack(self.validation_step_outputs)
+        avg_loss = losses.mean().item()
+        self.log(
+            "ptl/val_loss",
+            avg_loss,
+            batch_size=losses.size(0),
+            sync_dist=True,
+        )
+        self.valid_trajectories.append((self.global_step, avg_loss))
         self.validation_step_outputs.clear()  # free memory (compute `avg_loss` per epoch)
 
     def save(self, path):
         with fsspec.open(path, "wb") as f:
             torch.save(
                 {"hyper_parameters": self.hparams, "state_dict": self.state_dict()},
                 f,
```

### Comparing `neuralforecast-1.7.1/neuralforecast/common/_base_multivariate.py` & `neuralforecast-1.7.2/neuralforecast/common/_base_multivariate.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,16 +379,22 @@
         if torch.isnan(loss):
             print("Model Parameters", self.hparams)
             print("insample_y", torch.isnan(insample_y).sum())
             print("outsample_y", torch.isnan(outsample_y).sum())
             print("output", torch.isnan(output).sum())
             raise Exception("Loss is NaN, training stopped.")
 
-        self.log("train_loss", loss, prog_bar=True, on_epoch=True)
-        self.train_trajectories.append((self.global_step, float(loss)))
+        self.log(
+            "train_loss",
+            loss.item(),
+            batch_size=outsample_y.size(0),
+            prog_bar=True,
+            on_epoch=True,
+        )
+        self.train_trajectories.append((self.global_step, loss.item()))
         return loss
 
     def validation_step(self, batch, batch_idx):
         if self.val_size == 0:
             return np.nan
 
         # Create and normalize windows [Ws, L+H, C]
@@ -440,15 +446,21 @@
             valid_loss = self.valid_loss(
                 y=outsample_y, y_hat=output, mask=outsample_mask
             )
 
         if torch.isnan(valid_loss):
             raise Exception("Loss is NaN, training stopped.")
 
-        self.log("valid_loss", valid_loss, prog_bar=True, on_epoch=True)
+        self.log(
+            "valid_loss",
+            valid_loss.item(),
+            batch_size=outsample_y.size(0),
+            prog_bar=True,
+            on_epoch=True,
+        )
         self.validation_step_outputs.append(valid_loss)
         return valid_loss
 
     def predict_step(self, batch, batch_idx):
         # Create and normalize windows [Ws, L+H, C]
         windows = self._create_windows(batch, step="predict")
         y_idx = batch["y_idx"]
```

### Comparing `neuralforecast-1.7.1/neuralforecast/common/_base_recurrent.py` & `neuralforecast-1.7.2/neuralforecast/common/_base_recurrent.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,17 +339,21 @@
             print("Model Parameters", self.hparams)
             print("insample_y", torch.isnan(insample_y).sum())
             print("outsample_y", torch.isnan(outsample_y).sum())
             print("output", torch.isnan(output).sum())
             raise Exception("Loss is NaN, training stopped.")
 
         self.log(
-            "train_loss", loss, batch_size=self.batch_size, prog_bar=True, on_epoch=True
+            "train_loss",
+            loss.item(),
+            batch_size=outsample_y.size(0),
+            prog_bar=True,
+            on_epoch=True,
         )
-        self.train_trajectories.append((self.global_step, float(loss)))
+        self.train_trajectories.append((self.global_step, loss.item()))
         return loss
 
     def validation_step(self, batch, batch_idx):
         if self.val_size == 0:
             return np.nan
 
         # Create and normalize windows [Ws, L+H, C]
@@ -434,16 +438,16 @@
             )
 
         if torch.isnan(valid_loss):
             raise Exception("Loss is NaN, training stopped.")
 
         self.log(
             "valid_loss",
-            valid_loss,
-            batch_size=self.batch_size,
+            valid_loss.item(),
+            batch_size=outsample_y.size(0),
             prog_bar=True,
             on_epoch=True,
         )
         self.validation_step_outputs.append(valid_loss)
         return valid_loss
 
     def predict_step(self, batch, batch_idx):
```

### Comparing `neuralforecast-1.7.1/neuralforecast/common/_base_windows.py` & `neuralforecast-1.7.2/neuralforecast/common/_base_windows.py`

 * *Files 1% similar despite different names*

```diff
@@ -430,16 +430,22 @@
         if torch.isnan(loss):
             print("Model Parameters", self.hparams)
             print("insample_y", torch.isnan(insample_y).sum())
             print("outsample_y", torch.isnan(outsample_y).sum())
             print("output", torch.isnan(output).sum())
             raise Exception("Loss is NaN, training stopped.")
 
-        self.log("train_loss", loss, prog_bar=True, on_epoch=True)
-        self.train_trajectories.append((self.global_step, float(loss)))
+        self.log(
+            "train_loss",
+            loss.item(),
+            batch_size=outsample_y.size(0),
+            prog_bar=True,
+            on_epoch=True,
+        )
+        self.train_trajectories.append((self.global_step, loss.item()))
         return loss
 
     def _compute_valid_loss(
         self, outsample_y, output, outsample_mask, temporal_cols, y_idx
     ):
         if self.loss.is_distribution_output:
             _, y_loc, y_scale = self._inv_normalization(
@@ -527,21 +533,28 @@
                 temporal_cols=batch["temporal_cols"],
                 y_idx=batch["y_idx"],
             )
             valid_losses.append(valid_loss_batch)
             batch_sizes.append(len(output_batch))
 
         valid_loss = torch.stack(valid_losses)
-        batch_sizes = torch.tensor(batch_sizes).to(valid_loss.device)
-        valid_loss = torch.sum(valid_loss * batch_sizes) / torch.sum(batch_sizes)
+        batch_sizes = torch.tensor(batch_sizes, device=valid_loss.device)
+        batch_size = torch.sum(batch_sizes)
+        valid_loss = torch.sum(valid_loss * batch_sizes) / batch_size
 
         if torch.isnan(valid_loss):
             raise Exception("Loss is NaN, training stopped.")
 
-        self.log("valid_loss", valid_loss, prog_bar=True, on_epoch=True)
+        self.log(
+            "valid_loss",
+            valid_loss.item(),
+            batch_size=batch_size,
+            prog_bar=True,
+            on_epoch=True,
+        )
         self.validation_step_outputs.append(valid_loss)
         return valid_loss
 
     def predict_step(self, batch, batch_idx):
 
         # TODO: Hack to compute number of windows
         windows = self._create_windows(batch, step="predict")
```

### Comparing `neuralforecast-1.7.1/neuralforecast/common/_modules.py` & `neuralforecast-1.7.2/neuralforecast/common/_modules.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/common/_scalers.py` & `neuralforecast-1.7.2/neuralforecast/common/_scalers.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,16 +309,16 @@
     **Returns:**<br>
     `x`: original torch.Tensor `x`.
     """
     # Collapse dim dimension
     shape = list(x.shape)
     shape[dim] = 1
 
-    x_shift = torch.zeros(shape)
-    x_scale = torch.ones(shape)
+    x_shift = torch.zeros(shape, device=x.device)
+    x_scale = torch.ones(shape, device=x.device)
 
     return x_shift, x_scale
 
 # %% ../../nbs/common.scalers.ipynb 30
 def identity_scaler(x, x_shift, x_scale):
     return x
```

### Comparing `neuralforecast-1.7.1/neuralforecast/core.py` & `neuralforecast-1.7.2/neuralforecast/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from copy import deepcopy
 from itertools import chain
 from typing import Any, Dict, List, Optional, Union
 
 import fsspec
 import numpy as np
 import pandas as pd
+import pytorch_lightning as pl
 import torch
 import utilsforecast.processing as ufp
 from coreforecast.grouped_array import GroupedArray
 from coreforecast.scalers import (
     LocalBoxCoxScaler,
     LocalMinMaxScaler,
     LocalRobustScaler,
@@ -52,17 +53,24 @@
     TimesNet,
     TimeLLM,
     TSMixer,
     TSMixerx,
     MLPMultivariate,
     iTransformer,
     BiTCN,
+    TiDE,
+    DeepNPTS,
 )
 
 # %% ../nbs/core.ipynb 5
+# this disables warnings about the number of workers in the dataloaders
+# which the user can't control
+pl.disable_possible_user_warnings()
+
+
 def _insample_times(
     times: np.ndarray,
     uids: Series,
     indptr: np.ndarray,
     h: int,
     freq: Union[int, str, pd.offsets.BaseOffset],
     step_size: int = 1,
@@ -160,14 +168,18 @@
     "autotsmixerx": TSMixerx,
     "mlpmultivariate": MLPMultivariate,
     "automlpmultivariate": MLPMultivariate,
     "itransformer": iTransformer,
     "autoitransformer": iTransformer,
     "bitcn": BiTCN,
     "autobitcn": BiTCN,
+    "tide": TiDE,
+    "autotide": TiDE,
+    "deepnpts": DeepNPTS,
+    "autodeepnpts": DeepNPTS,
 }
 
 # %% ../nbs/core.ipynb 8
 _type2scaler = {
     "standard": LocalStandardScaler,
     "robust": lambda: LocalRobustScaler(scale="mad"),
     "robust-iqr": lambda: LocalRobustScaler(scale="iqr"),
@@ -864,19 +876,37 @@
                 self.dataset, step_size=step_size, **data_kwargs
             )
 
             # Append predictions in memory placeholder
             output_length = len(model.loss.output_names)
             fcsts[:, col_idx : (col_idx + output_length)] = model_fcsts
             col_idx += output_length
-        if self.scalers_:
-            indptr = np.append(
-                0, np.full(self.dataset.n_groups, self.h * n_windows).cumsum()
-            )
-            fcsts = self._scalers_target_inverse_transform(fcsts, indptr)
+        # we may have allocated more space than needed
+        # each serie can produce at most (serie.size - 1) // self.h CV windows
+        effective_sizes = ufp.counts_by_id(fcsts_df, id_col)["counts"].to_numpy()
+        needs_trim = effective_sizes.sum() != fcsts.shape[0]
+        if self.scalers_ or needs_trim:
+            indptr = np.arange(
+                0,
+                n_windows * self.h * (self.dataset.n_groups + 1),
+                n_windows * self.h,
+                dtype=np.int32,
+            )
+            if self.scalers_:
+                fcsts = self._scalers_target_inverse_transform(fcsts, indptr)
+            if needs_trim:
+                # we keep only the effective samples of each serie from the cv results
+                trimmed = np.empty_like(
+                    fcsts, shape=(effective_sizes.sum(), fcsts.shape[1])
+                )
+                cv_indptr = np.append(0, effective_sizes).cumsum(dtype=np.int32)
+                for i in range(fcsts.shape[1]):
+                    ga = GroupedArray(fcsts[:, i], indptr)
+                    trimmed[:, i] = ga._tails(cv_indptr)
+                fcsts = trimmed
 
         self._fitted = True
 
         # Add predictions to forecasts DataFrame
         if isinstance(self.uids, pl_Series):
             fcsts = pl_DataFrame(dict(zip(cols, fcsts.T)))
         else:
```

### Comparing `neuralforecast-1.7.1/neuralforecast/losses/numpy.py` & `neuralforecast-1.7.2/neuralforecast/losses/numpy.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/losses/pytorch.py` & `neuralforecast-1.7.2/neuralforecast/losses/pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,21 @@
 
 import math
 import numpy as np
 import torch
 
 import torch.nn.functional as F
 from torch.distributions import Distribution
-from torch.distributions import Bernoulli, Normal, StudentT, Poisson, NegativeBinomial
+from torch.distributions import (
+    Bernoulli,
+    Normal,
+    StudentT,
+    Poisson,
+    NegativeBinomial,
+)
 
 from torch.distributions import constraints
 
 # %% ../../nbs/losses.pytorch.ipynb 6
 def _divide_no_nan(a: torch.Tensor, b: torch.Tensor) -> torch.Tensor:
     """
     Auxiliary funtion to handle divide by 0
```

### Comparing `neuralforecast-1.7.1/neuralforecast/models/__init__.py` & `neuralforecast-1.7.2/neuralforecast/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __all__ = ['RNN', 'GRU', 'LSTM', 'TCN', 'DeepAR', 'DilatedRNN',
            'MLP', 'NHITS', 'NBEATS', 'NBEATSx', 'DLinear', 'NLinear',
            'TFT', 'VanillaTransformer', 'Informer', 'Autoformer', 'PatchTST', 'FEDformer',
            'StemGNN', 'HINT', 'TimesNet', 'TimeLLM', 'TSMixer', 'TSMixerx', 'MLPMultivariate',
-           'iTransformer', 'BiTCN',
+           'iTransformer', 'BiTCN', 'TiDE', 'DeepNPTS'
            ]
 
 from .rnn import RNN
 from .gru import GRU
 from .lstm import LSTM
 from .tcn import TCN
 from .deepar import DeepAR
@@ -28,8 +28,9 @@
 from .timesnet import TimesNet
 from .timellm import TimeLLM
 from .tsmixer import TSMixer
 from .tsmixerx import TSMixerx
 from .mlpmultivariate import MLPMultivariate
 from .itransformer import iTransformer
 from .bitcn import BiTCN
-
+from .tide import TiDE
+from .deepnpts import DeepNPTS
```

### Comparing `neuralforecast-1.7.1/neuralforecast/models/autoformer.py` & `neuralforecast-1.7.2/neuralforecast/models/autoformer.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/models/bitcn.py` & `neuralforecast-1.7.2/neuralforecast/models/bitcn.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/models/deepar.py` & `neuralforecast-1.7.2/neuralforecast/models/deepar.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,16 +274,22 @@
         if torch.isnan(loss):
             print("Model Parameters", self.hparams)
             print("insample_y", torch.isnan(insample_y).sum())
             print("outsample_y", torch.isnan(outsample_y).sum())
             print("output", torch.isnan(output).sum())
             raise Exception("Loss is NaN, training stopped.")
 
-        self.log("train_loss", loss, prog_bar=True, on_epoch=True)
-        self.train_trajectories.append((self.global_step, float(loss)))
+        self.log(
+            "train_loss",
+            loss.item(),
+            batch_size=outsample_y.size(0),
+            prog_bar=True,
+            on_epoch=True,
+        )
+        self.train_trajectories.append((self.global_step, loss.item()))
 
         self.h = self.horizon_backup  # Restore horizon
         return loss
 
     def validation_step(self, batch, batch_idx):
 
         self.h == self.horizon_backup
@@ -335,20 +341,27 @@
                 y=original_outsample_y, y_hat=output_batch, mask=outsample_mask
             )
             valid_losses.append(valid_loss_batch)
             batch_sizes.append(len(output_batch))
 
         valid_loss = torch.stack(valid_losses)
         batch_sizes = torch.tensor(batch_sizes, device=valid_loss.device)
-        valid_loss = torch.sum(valid_loss * batch_sizes) / torch.sum(batch_sizes)
+        batch_size = torch.sum(batch_sizes)
+        valid_loss = torch.sum(valid_loss * batch_sizes) / batch_size
 
         if torch.isnan(valid_loss):
             raise Exception("Loss is NaN, training stopped.")
 
-        self.log("valid_loss", valid_loss, prog_bar=True, on_epoch=True)
+        self.log(
+            "valid_loss",
+            valid_loss.item(),
+            batch_size=batch_size,
+            prog_bar=True,
+            on_epoch=True,
+        )
         self.validation_step_outputs.append(valid_loss)
         return valid_loss
 
     def predict_step(self, batch, batch_idx):
 
         self.h == self.horizon_backup
```

### Comparing `neuralforecast-1.7.1/neuralforecast/models/dilated_rnn.py` & `neuralforecast-1.7.2/neuralforecast/models/dilated_rnn.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/models/dlinear.py` & `neuralforecast-1.7.2/neuralforecast/models/dlinear.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/models/fedformer.py` & `neuralforecast-1.7.2/neuralforecast/models/fedformer.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/models/gru.py` & `neuralforecast-1.7.2/neuralforecast/models/gru.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/models/hint.py` & `neuralforecast-1.7.2/neuralforecast/models/hint.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/models/informer.py` & `neuralforecast-1.7.2/neuralforecast/models/informer.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/models/itransformer.py` & `neuralforecast-1.7.2/neuralforecast/models/itransformer.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/models/lstm.py` & `neuralforecast-1.7.2/neuralforecast/models/lstm.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/models/mlp.py` & `neuralforecast-1.7.2/neuralforecast/models/mlp.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/models/mlpmultivariate.py` & `neuralforecast-1.7.2/neuralforecast/models/mlpmultivariate.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/models/nbeats.py` & `neuralforecast-1.7.2/neuralforecast/models/nbeats.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,14 +270,20 @@
         num_workers_loader: int = 0,
         drop_last_loader: bool = False,
         optimizer=None,
         optimizer_kwargs=None,
         **trainer_kwargs,
     ):
 
+        # Protect horizon collapsed seasonality and trend NBEATSx-i basis
+        if h == 1 and (("seasonality" in stack_types) or ("trend" in stack_types)):
+            raise Exception(
+                "Horizon `h=1` incompatible with `seasonality` or `trend` in stacks"
+            )
+
         # Inherit BaseWindows class
         super(NBEATS, self).__init__(
             h=h,
             input_size=input_size,
             loss=loss,
             valid_loss=valid_loss,
             max_steps=max_steps,
```

### Comparing `neuralforecast-1.7.1/neuralforecast/models/nbeatsx.py` & `neuralforecast-1.7.2/neuralforecast/models/nbeatsx.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/models/nhits.py` & `neuralforecast-1.7.2/neuralforecast/models/nhits.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/models/nlinear.py` & `neuralforecast-1.7.2/neuralforecast/models/nlinear.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/models/patchtst.py` & `neuralforecast-1.7.2/neuralforecast/models/patchtst.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/models/rnn.py` & `neuralforecast-1.7.2/neuralforecast/models/rnn.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/models/stemgnn.py` & `neuralforecast-1.7.2/neuralforecast/models/stemgnn.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/models/tcn.py` & `neuralforecast-1.7.2/neuralforecast/models/tcn.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/models/tft.py` & `neuralforecast-1.7.2/neuralforecast/models/tft.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/models/timellm.py` & `neuralforecast-1.7.2/neuralforecast/models/timellm.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/models/timesnet.py` & `neuralforecast-1.7.2/neuralforecast/models/timesnet.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/models/tsmixer.py` & `neuralforecast-1.7.2/neuralforecast/models/tsmixer.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/models/tsmixerx.py` & `neuralforecast-1.7.2/neuralforecast/models/tsmixerx.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/models/vanillatransformer.py` & `neuralforecast-1.7.2/neuralforecast/models/vanillatransformer.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast/tsdataset.py` & `neuralforecast-1.7.2/neuralforecast/tsdataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # %% auto 0
 __all__ = ['TimeSeriesLoader', 'TimeSeriesDataset', 'TimeSeriesDataModule']
 
 # %% ../nbs/tsdataset.ipynb 4
 import warnings
 from collections.abc import Mapping
-from typing import List, Optional
+from typing import List, Optional, Union
 
 import numpy as np
 import pandas as pd
 import pytorch_lightning as pl
 import torch
 import utilsforecast.processing as ufp
 from torch.utils.data import Dataset, DataLoader
@@ -85,19 +85,19 @@
         min_size: int,
         y_idx: int,
         static=None,
         static_cols=None,
         sorted=False,
     ):
         super().__init__()
-        self.temporal = torch.tensor(temporal, dtype=torch.float)
+        self.temporal = self._as_torch_copy(temporal)
         self.temporal_cols = pd.Index(list(temporal_cols))
 
         if static is not None:
-            self.static = torch.tensor(static, dtype=torch.float)
+            self.static = self._as_torch_copy(static)
             self.static_cols = static_cols
         else:
             self.static = static
             self.static_cols = static_cols
 
         self.indptr = indptr
         self.n_groups = self.indptr.size - 1
@@ -141,14 +141,23 @@
     def __eq__(self, other):
         if not hasattr(other, "data") or not hasattr(other, "indptr"):
             return False
         return np.allclose(self.data, other.data) and np.array_equal(
             self.indptr, other.indptr
         )
 
+    def _as_torch_copy(
+        self,
+        x: Union[np.ndarray, torch.Tensor],
+        dtype: torch.dtype = torch.float32,
+    ) -> torch.Tensor:
+        if isinstance(x, np.ndarray):
+            x = torch.from_numpy(x)
+        return x.to(dtype, copy=False).clone()
+
     def align(
         self, df: DataFrame, id_col: str, time_col: str, target_col: str
     ) -> "TimeSeriesDataset":
         # Protect consistency
         df = ufp.copy_if_pandas(df, deep=False)
 
         # Add Nones to missing columns (without available_mask)
@@ -252,15 +261,15 @@
         new_max_size = dataset.max_size - left_trim - right_trim
         new_min_size = dataset.min_size - left_trim - right_trim
 
         # Define new dataset
         updated_dataset = TimeSeriesDataset(
             temporal=new_temporal,
             temporal_cols=dataset.temporal_cols.copy(),
-            indptr=np.array(new_indptr).astype(np.int32),
+            indptr=np.array(new_indptr, dtype=np.int32),
             max_size=new_max_size,
             min_size=new_min_size,
             y_idx=dataset.y_idx,
             static=dataset.static,
             static_cols=dataset.static_cols,
             sorted=dataset.sorted,
         )
```

### Comparing `neuralforecast-1.7.1/neuralforecast/utils.py` & `neuralforecast-1.7.2/neuralforecast/utils.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/neuralforecast.egg-info/PKG-INFO` & `neuralforecast-1.7.2/neuralforecast.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralforecast
-Version: 1.7.1
+Version: 1.7.2
 Summary: Time series forecasting suite using deep learning models
 Home-page: https://github.com/Nixtla/neuralforecast/
 Author: Nixtla
 Author-email: business@nixtla.io
 License: Apache Software License 2.0
 Keywords: time-series forecasting deep-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `neuralforecast-1.7.1/neuralforecast.egg-info/SOURCES.txt` & `neuralforecast-1.7.2/neuralforecast.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 neuralforecast/losses/__init__.py
 neuralforecast/losses/numpy.py
 neuralforecast/losses/pytorch.py
 neuralforecast/models/__init__.py
 neuralforecast/models/autoformer.py
 neuralforecast/models/bitcn.py
 neuralforecast/models/deepar.py
+neuralforecast/models/deepnpts.py
 neuralforecast/models/dilated_rnn.py
 neuralforecast/models/dlinear.py
 neuralforecast/models/fedformer.py
 neuralforecast/models/gru.py
 neuralforecast/models/hint.py
 neuralforecast/models/informer.py
 neuralforecast/models/itransformer.py
@@ -48,12 +49,13 @@
 neuralforecast/models/nhits.py
 neuralforecast/models/nlinear.py
 neuralforecast/models/patchtst.py
 neuralforecast/models/rnn.py
 neuralforecast/models/stemgnn.py
 neuralforecast/models/tcn.py
 neuralforecast/models/tft.py
+neuralforecast/models/tide.py
 neuralforecast/models/timellm.py
 neuralforecast/models/timesnet.py
 neuralforecast/models/tsmixer.py
 neuralforecast/models/tsmixerx.py
 neuralforecast/models/vanillatransformer.py
```

### Comparing `neuralforecast-1.7.1/pyproject.toml` & `neuralforecast-1.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.1/settings.ini` & `neuralforecast-1.7.2/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 user = Nixtla
 description = Time series forecasting suite using deep learning models
 keywords = time-series forecasting deep-learning 
 author = Nixtla
 author_email = business@nixtla.io
 copyright = Nixtla Inc.
 branch = main
-version = 1.7.1
+version = 1.7.2
 min_python = 3.8
 audience = Developers
 language = English
 custom_sidebar = True
 license = apache2
 status = 2
 requirements = coreforecast>=0.0.6 fsspec numpy>=1.21.6 pandas>=1.3.5 torch>=2.0.0 pytorch-lightning>=2.0.0 ray[tune]>=2.2.0 optuna utilsforecast>=0.0.25
```

### Comparing `neuralforecast-1.7.1/setup.py` & `neuralforecast-1.7.2/setup.py`

 * *Files identical despite different names*

