# Comparing `tmp/tangermeme-0.1.0rc0.tar.gz` & `tmp/tangermeme-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tangermeme-0.1.0rc0.tar", last modified: Thu Mar 28 15:12:47 2024, max compression
+gzip compressed data, was "tangermeme-0.2.0.tar", last modified: Tue May  7 17:20:42 2024, max compression
```

## Comparing `tangermeme-0.1.0rc0.tar` & `tangermeme-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,49 @@
-drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-03-28 15:12:46.243402 tangermeme-0.1.0rc0/
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     1072 2024-02-04 20:42:51.000000 tangermeme-0.1.0rc0/LICENSE
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      559 2024-03-28 15:12:46.235402 tangermeme-0.1.0rc0/PKG-INFO
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     3251 2024-03-28 05:30:44.000000 tangermeme-0.1.0rc0/README.md
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)       38 2024-03-28 15:12:46.243402 tangermeme-0.1.0rc0/setup.cfg
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      665 2024-03-28 15:11:06.000000 tangermeme-0.1.0rc0/setup.py
-drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-03-28 15:12:46.111402 tangermeme-0.1.0rc0/tangermeme/
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      114 2024-03-28 15:11:24.000000 tangermeme-0.1.0rc0/tangermeme/__init__.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    22259 2024-03-28 04:48:35.000000 tangermeme-0.1.0rc0/tangermeme/ersatz.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    14430 2024-03-28 04:48:35.000000 tangermeme-0.1.0rc0/tangermeme/io.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     3707 2024-03-28 04:48:35.000000 tangermeme-0.1.0rc0/tangermeme/ism.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6550 2024-02-18 21:52:53.000000 tangermeme-0.1.0rc0/tangermeme/kmers.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6991 2024-03-12 01:37:58.000000 tangermeme-0.1.0rc0/tangermeme/marginalize.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    12384 2024-02-16 06:07:44.000000 tangermeme-0.1.0rc0/tangermeme/match.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     5018 2024-02-16 06:07:44.000000 tangermeme-0.1.0rc0/tangermeme/plot.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6062 2024-03-28 04:48:35.000000 tangermeme-0.1.0rc0/tangermeme/predict.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     7703 2024-03-28 04:48:35.000000 tangermeme-0.1.0rc0/tangermeme/space.py
-drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-03-28 15:12:46.167402 tangermeme-0.1.0rc0/tangermeme/tools/
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)        0 2024-02-12 20:33:38.000000 tangermeme-0.1.0rc0/tangermeme/tools/__init__.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    13248 2024-02-19 18:37:49.000000 tangermeme-0.1.0rc0/tangermeme/tools/fimo.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     2445 2024-02-25 18:18:37.000000 tangermeme-0.1.0rc0/tangermeme/tools/tomtom.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     9101 2024-02-16 06:07:44.000000 tangermeme-0.1.0rc0/tangermeme/utils.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     5454 2024-03-28 04:48:35.000000 tangermeme-0.1.0rc0/tangermeme/variant_effect.py
-drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-03-28 15:12:46.227402 tangermeme-0.1.0rc0/tangermeme.egg-info/
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      559 2024-03-28 15:12:45.000000 tangermeme-0.1.0rc0/tangermeme.egg-info/PKG-INFO
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      744 2024-03-28 15:12:46.000000 tangermeme-0.1.0rc0/tangermeme.egg-info/SOURCES.txt
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)        1 2024-03-28 15:12:45.000000 tangermeme-0.1.0rc0/tangermeme.egg-info/dependency_links.txt
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      139 2024-03-28 15:12:45.000000 tangermeme-0.1.0rc0/tangermeme.egg-info/requires.txt
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)       28 2024-03-28 15:12:45.000000 tangermeme-0.1.0rc0/tangermeme.egg-info/top_level.txt
-drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-03-28 15:12:46.223402 tangermeme-0.1.0rc0/tests/
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    25611 2024-03-28 04:48:35.000000 tangermeme-0.1.0rc0/tests/test_ersatz.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    22795 2024-03-28 04:48:35.000000 tangermeme-0.1.0rc0/tests/test_io.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     5107 2024-03-28 05:30:44.000000 tangermeme-0.1.0rc0/tests/test_ism.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     1536 2024-02-19 00:37:13.000000 tangermeme-0.1.0rc0/tests/test_kmers.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    18843 2024-03-28 04:48:35.000000 tangermeme-0.1.0rc0/tests/test_marginalize.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    13448 2024-02-16 07:04:10.000000 tangermeme-0.1.0rc0/tests/test_match.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    12913 2024-02-16 07:04:20.000000 tangermeme-0.1.0rc0/tests/test_predict.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    19522 2024-03-28 04:48:35.000000 tangermeme-0.1.0rc0/tests/test_space.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6841 2024-02-16 07:04:33.000000 tangermeme-0.1.0rc0/tests/test_utils.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     7610 2024-03-28 04:48:35.000000 tangermeme-0.1.0rc0/tests/test_variant_effect.py
+drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-05-07 17:20:42.643109 tangermeme-0.2.0/
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     1072 2024-02-04 20:42:51.000000 tangermeme-0.2.0/LICENSE
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      591 2024-05-07 17:20:42.638109 tangermeme-0.2.0/PKG-INFO
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    16195 2024-05-07 17:13:13.000000 tangermeme-0.2.0/README.md
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)       38 2024-05-07 17:20:42.644109 tangermeme-0.2.0/setup.cfg
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      695 2024-05-07 17:13:13.000000 tangermeme-0.2.0/setup.py
+drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-05-07 17:20:42.446108 tangermeme-0.2.0/tangermeme/
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      111 2024-05-07 17:13:13.000000 tangermeme-0.2.0/tangermeme/__init__.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     5832 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tangermeme/ablate.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    27068 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tangermeme/deep_lift_shap.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6424 2024-04-19 03:17:23.000000 tangermeme-0.2.0/tangermeme/design.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    22259 2024-04-12 17:47:04.000000 tangermeme-0.2.0/tangermeme/ersatz.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    14430 2024-03-28 04:48:35.000000 tangermeme-0.2.0/tangermeme/io.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6729 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tangermeme/ism.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6550 2024-02-18 21:52:53.000000 tangermeme-0.2.0/tangermeme/kmers.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     4598 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tangermeme/marginalize.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    12384 2024-02-16 06:07:44.000000 tangermeme-0.2.0/tangermeme/match.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     5027 2024-05-03 22:57:28.000000 tangermeme-0.2.0/tangermeme/plot.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     3409 2024-04-01 23:34:04.000000 tangermeme-0.2.0/tangermeme/predict.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     4424 2024-04-01 23:49:41.000000 tangermeme-0.2.0/tangermeme/product.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    11906 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tangermeme/seqlet.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     3641 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tangermeme/space.py
+drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-05-07 17:20:42.495108 tangermeme-0.2.0/tangermeme/tools/
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)        0 2024-02-12 20:33:38.000000 tangermeme-0.2.0/tangermeme/tools/__init__.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    13248 2024-02-19 18:37:49.000000 tangermeme-0.2.0/tangermeme/tools/fimo.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     2445 2024-02-25 18:18:37.000000 tangermeme-0.2.0/tangermeme/tools/tomtom.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     9118 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tangermeme/utils.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    14343 2024-05-07 03:58:32.000000 tangermeme-0.2.0/tangermeme/variant_effect.py
+drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-05-07 17:20:42.633109 tangermeme-0.2.0/tangermeme.egg-info/
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      591 2024-05-07 17:20:42.000000 tangermeme-0.2.0/tangermeme.egg-info/PKG-INFO
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      951 2024-05-07 17:20:42.000000 tangermeme-0.2.0/tangermeme.egg-info/SOURCES.txt
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)        1 2024-05-07 17:20:42.000000 tangermeme-0.2.0/tangermeme.egg-info/dependency_links.txt
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      159 2024-05-07 17:20:42.000000 tangermeme-0.2.0/tangermeme.egg-info/requires.txt
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)       28 2024-05-07 17:20:42.000000 tangermeme-0.2.0/tangermeme.egg-info/top_level.txt
+drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-05-07 17:20:42.629109 tangermeme-0.2.0/tests/
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    28374 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tests/test_ablate.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    36846 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tests/test_deep_lift_shap.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    25611 2024-03-28 04:48:35.000000 tangermeme-0.2.0/tests/test_ersatz.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    22795 2024-03-28 04:48:35.000000 tangermeme-0.2.0/tests/test_io.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    12445 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tests/test_ism.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     1536 2024-02-19 00:37:13.000000 tangermeme-0.2.0/tests/test_kmers.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    21450 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tests/test_marginalize.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    13448 2024-02-16 07:04:10.000000 tangermeme-0.2.0/tests/test_match.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6967 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tests/test_predict.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    23116 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tests/test_product.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     8491 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tests/test_seqlet.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    22448 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tests/test_space.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6841 2024-02-16 07:04:33.000000 tangermeme-0.2.0/tests/test_utils.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     3541 2024-05-07 04:03:24.000000 tangermeme-0.2.0/tests/test_variant_effect.py
```

### Comparing `tangermeme-0.1.0rc0/LICENSE` & `tangermeme-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tangermeme-0.1.0rc0/PKG-INFO` & `tangermeme-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tangermeme
-Version: 0.1.0rc0
+Version: 0.2.0
 Summary: Biological sequence analysis for the modern age.
 Home-page: https://github.com/jmschrei/tangermeme
 Author: Jacob Schreiber
 Author-email: jmschreiber91@gmail.com
 License: LICENSE.txt
 License-File: LICENSE
 Requires-Dist: numpy>=1.14.2
@@ -13,7 +13,8 @@
 Requires-Dist: pyBigWig>=0.3.17
 Requires-Dist: torch>=1.9.0
 Requires-Dist: pyfaidx>=0.7.2.1
 Requires-Dist: tqdm>=4.64.1
 Requires-Dist: numba>=0.55.1
 Requires-Dist: logomaker
 Requires-Dist: joblib>=1.3.2
+Requires-Dist: scikit-learn>=1.2.2
```

### Comparing `tangermeme-0.1.0rc0/setup.py` & `tangermeme-0.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tangermeme',
-    version='0.1.0-rc',
+    version='0.2.0',
     author='Jacob Schreiber',
     author_email='jmschreiber91@gmail.com',
     packages=['tangermeme', 'tangermeme/tools'],
     scripts=[],
     url='https://github.com/jmschrei/tangermeme',
     license='LICENSE.txt',
     description='Biological sequence analysis for the modern age.',
@@ -16,10 +16,11 @@
         "pandas >= 1.3.3",
         "pyBigWig >= 0.3.17",
         "torch >= 1.9.0",
         "pyfaidx >= 0.7.2.1",
         "tqdm >= 4.64.1",
         "numba >= 0.55.1",
         "logomaker",
-        "joblib >= 1.3.2"
+        "joblib >= 1.3.2",
+        "scikit-learn >= 1.2.2"
     ],
 )
```

### Comparing `tangermeme-0.1.0rc0/tangermeme/ersatz.py` & `tangermeme-0.2.0/tangermeme/ersatz.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ablate.py
+# ersatz.py
 # Author: Jacob Schreiber <jmschreiber91@gmail.com>
 
 import numba
 import numpy
 import torch
 import pandas
```

### Comparing `tangermeme-0.1.0rc0/tangermeme/io.py` & `tangermeme-0.2.0/tangermeme/io.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.1.0rc0/tangermeme/ism.py` & `tangermeme-0.2.0/tangermeme/predict.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,129 +1,114 @@
-# ism.py
+# predict.py
 # Contact: Jacob Schreiber <jmschreiber91@gmail.com>
 
 import torch
 import itertools
 
-from .predict import predict
+from tqdm import trange
 
 
-def _edit_distance_one(X, start, end):
-	"""An internal function for generating all sequences of edit distance 1
+def predict(model, X, args=None, batch_size=32, device='cuda', verbose=False):
+	"""Make batched predictions in a memory-efficient manner.
 
-	This internal function, which is meant to be used for ISM, will take in a
-	one-hot encoded sequence and return all sequences that have an edit distance
-	of one. 
-
-
-	Parameters
-	----------
-	X: torch.Tensor, shape=(len(alphabet), sequence_length)
-		A single one-hot encoded sequence.
-
-	start: int
-		The first nucleotide to begin making edits on, inclusive.
-
-	end: int
-		The end of the span. Edits are not made on this nucleotide at this
-		index. Can be negative indexes.
-
-
-	Returns
-	-------
-	X_: torch.Tensor, shape=(length*len(alphabet), len(alphabet), length)
-		All one-hot encoded sequences that have an edit distance of 1 from the
-		original sequence. 
-	"""
-
-	end = end if end >= 0 else X.shape[-1] + 1 + end
-	X_ = X.repeat((end-start)*X.shape[0], 1, 1)
-
-	coords = itertools.product(range(X.shape[0]), range(start, end))
-	for i, (j, k) in enumerate(coords):
-		X_[i, :, k] = 0
-		X_[i, j, k] = 1
-
-	return X_
-
-
-@torch.no_grad
-def saturation_mutagenesis(model, X, args=None, start=0, end=-1, batch_size=32,
-	device='cuda', verbose=False):
-	"""Performs in-silico saturation mutagenesis on a set of sequences.
-
-	This function will perform in-silico saturation mutagenesis on a set of 
-	sequences and return the predictions on the original sequences and each
-	of the sequences with an edit distance of one on them.
+	This function will take a PyTorch model and make predictions from it using
+	the forward function, with optional additional arguments to the model. The
+	additional arguments must have the same batch size as the examples, and the
+	i-th example will be given to the model with the i-th index of each
+	additional argument. 
+
+	Before starting predictions, the model is moved to the specified device. As 
+	predictions are being made, each batch is also moved to the specified 
+	device and then moved back to the CPU after predictions are made. This is
+	to allow the function to work on massive numbers of examples that would
+	not necessarily each fit in memory. If the batches themselves do not fit
+	in memory, try lowering the batch size.
 
 
 	Parameters
 	----------
 	model: torch.nn.Module
 		The PyTorch model to use to make predictions.
 
 	X: torch.tensor, shape=(-1, len(alphabet), length)
 		A one-hot encoded set of sequences to make predictions for.
 
-	args: tuple or None, optional
+	args: tuple or list or None, optional
 		An optional set of additional arguments to pass into the model. If
 		provided, each element in the tuple or list is one input to the model
 		and the element must be formatted to be the same batch size as `X`. If
 		None, no additional arguments are passed into the forward function.
 		Default is None.
 
-	start: int, optional
-		The start of where to begin making perturbations to the sequence.
-		Default is 0.
-
-	end: int, optional
-		The end of where to to make perturbations to the sequence,
-		non-inclusive. Default is -1.
-
 	batch_size: int, optional
 		The number of examples to make predictions for at a time. Default is 32.
 
 	device: str or torch.device, optional
 		The device to move the model and batches to when making predictions. If
 		set to 'cuda' without a GPU, this function will crash and must be set
 		to 'cpu'. Default is 'cuda'. 
 
 	verbose: bool, optional
 		Whether to display a progress bar during predictions. Default is False.
 
 
 	Returns
 	-------
-	y0: torch.Tensor or list/tuple of torch.Tensors
-		The outputs from the model for the reference sequences.
-
-	y_hat: torch.Tensor or list/tuple of torch.Tensors
-		The outputs from the model for each of the perturbed sequences.
+	y: torch.Tensor or list/tuple of torch.Tensors
+		The output from the model for each input example. The precise format
+		is determined by the model. If the model outputs a single tensor,
+		y is a single tensor concatenated across all batches. If the model
+		outputs multiple tensors, y is a list of tensors which are each
+		concatenated across all batches.
 	"""
 
-	y0 = predict(model, X, args=args, device=device)
-	
-	y_hat = []
-	for i in range(X.shape[0]):
-		X_ = _edit_distance_one(X[i], start, end)
-
-		if args is not None:
-			args_ = tuple(a[i].repeat(X_.shape[0], *(1 for _ in a[i].shape)) 
-				for a in args)
-		else:
-			args_ = None
-
-		y_hat_ = predict(model, X_, args=args_, batch_size=batch_size, 
-			device=device, verbose=verbose)
-
-		y_hat.append(y_hat_)
-
-	if isinstance(y_hat[0], torch.Tensor):
-		y_hat = torch.stack(y_hat).reshape(X.shape[0], X.shape[1], end-start, 
-			*y_hat_.shape[1:])#.transpose(2, 1)
+	model = model.to(device).eval()
+
+	try:
+		dtype = next(model.parameters()).dtype
+	except:
+		dtype = X.dtype
+
+
+	if args is not None:
+		for arg in args:
+			if arg.shape[0] != X.shape[0]:
+				raise ValueError("Arguments must have the same first " +
+					"dimension as X")
+
+	###
+
+	y = []
+	with torch.no_grad():
+		batch_size = min(batch_size, X.shape[0])
+
+		for start in trange(0, X.shape[0], batch_size, disable=not verbose):
+			end = start + batch_size
+			X_ = X[start:end].to(device).type(dtype)
+
+			if X_.shape[0] == 0:
+				continue
+
+			if args is not None:
+				args_ = [a[start:end].to(device) for a in args]
+				y_ = model(X_, *args_)
+			else:
+				y_ = model(X_)
+
+			# Move to the CPU
+			if isinstance(y_, torch.Tensor):
+				y_ = y_.cpu()
+			elif isinstance(y_, (list, tuple)):
+				y_ = tuple(yi.cpu() for yi in y_)
+			else:
+				raise ValueError("Cannot interpret output from model.")
+
+			y.append(y_)
+
+
+	# Concatenate the outputs
+	if isinstance(y[0], torch.Tensor):
+		y = torch.cat(y)
 	else:
-		y_hat = [
-			torch.cat(y_).reshape(X.shape[0], X.shape[2], X.shape[1], 
-				*y_[0].shape[1:]).transpose(2, 1) for y_ in zip(*y_hat)
-		]
+		y = [torch.cat(y_) for y_ in list(zip(*y))]
 
-	return y0, y_hat
+	return y
```

### Comparing `tangermeme-0.1.0rc0/tangermeme/kmers.py` & `tangermeme-0.2.0/tangermeme/kmers.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.1.0rc0/tangermeme/match.py` & `tangermeme-0.2.0/tangermeme/match.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.1.0rc0/tangermeme/plot.py` & `tangermeme-0.2.0/tangermeme/plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,35 +108,36 @@
 	if annotations is not None:
 		annotations_ = annotations[annotations['start'] > start]
 		annotations_ = annotations_[annotations_['end'] < end]
 		annotations_ = annotations_.sort_values(["score"], ascending=False)
 
 		ylim = ylim or max(abs(X_attr.min()), abs(X_attr.max()))
 		plt.ylim(-ylim, ylim)
+		r = ylim*2
 
 		motifs = numpy.zeros((end-start, annotations_.shape[0]))
 		for _, row in annotations_.iterrows():
-			(motif, motif_start, motif_end, _, score, _, _) = row
+			motif, motif_start, motif_end, _, score = row[:5]
 			motif_start -= start
 			motif_end -= start
 			
 			y_offset = 0.1
 			for i in range(annotations_.shape[0]):
 				if motifs[motif_start:motif_end, i].max() == 0:
 					if i < n_tracks:
 						text = "{}: ({:3.3})".format(motif, score)
 						motifs[motif_start:motif_end, i] = 1
 						y_offset += 0.2*i
 						
 						xp = [motif_start, motif_end]
 						yp = [-ylim*y_offset, -ylim*y_offset]
 
-						plt.plot(xp, yp, color='0.7', linewidth=2)        
+						plt.plot(xp, yp, color='0.3', linewidth=2)        
 						plt.text(xp[0], -ylim*(y_offset+0.1), text, 
-							color='0.7', fontsize=9)
+							color='0.3', fontsize=9)
 						
 					elif show_extra:
 						s = motif_start
 
 						motifs[motif_start:motif_start+len(motif)*2, i] = 1
 						y_offset += -0.1 + 0.2*(n_tracks) + 0.1*(i-n_tracks)
```

### Comparing `tangermeme-0.1.0rc0/tangermeme/predict.py` & `tangermeme-0.2.0/tangermeme/design.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,139 +1,103 @@
-# predict.py
+# design.py
 # Contact: Jacob Schreiber <jmschreiber91@gmail.com>
 
+import time
+import numpy
 import torch
-import itertools
 
-from tqdm import trange
-
-
-def predict(model, X, args=None, batch_size=32, device='cuda', verbose=False):
-	"""Make batched predictions in a memory-efficient manner.
-
-	This function will take a PyTorch model and make predictions from it using
-	the forward function, with optional additional arguments to the model. The
-	additional arguments must have the same batch size as the examples, and the
-	i-th example will be given to the model with the i-th index of each
-	additional argument. 
-
-	Before starting predictions, the model is moved to the specified device. As 
-	predictions are being made, each batch is also moved to the specified 
-	device and then moved back to the CPU after predictions are made. This is
-	to allow the function to work on massive numbers of examples that would
-	not necessarily each fit in memory. If the batches themselves do not fit
-	in memory, try lowering the batch size.
+from .utils import one_hot_encode
+from .ersatz import substitute
+from .predict import predict
+
+
+def greedy_substitution(model, X, motifs, y, loss=torch.nn.MSELoss(
+	reduction='none'), mask=None, tol=1e-3, max_iter=-1, args=None, start=None, 
+	alphabet=['A', 'C', 'G', 'T'], batch_size=32, device='cuda', verbose=False):
+	"""Greedily add motifs to achieve a desired goal. 
+
+	This design function will greedily add motifs to achieve a desired output
+	from the model. Each round, the function will iterate through all possible
+	motifs, substitute each one with the given spacing, and keep the one whose
+	loss function is the smallest. This process will continue until either the
+	maximum number of iterations is reached (at which point, `max_iter` motifs
+	will have been inserted into the sequence) or the loss falls below `tol`.
+
+	Accordingly, the choice of loss function and desired output from the model
+	is crucial for good design. Usually, the loss function can be Euclidean
+	distance, but for models with more complex outputs or for subtle design
+	tasks one may want to use something else, such as Jensen-Shannon divergence.
 
 
 	Parameters
 	----------
 	model: torch.nn.Module
-		The PyTorch model to use to make predictions.
+		A PyTorch model to use for making predictions. These models can take in
+		any number of inputs and make any number of outputs. The additional
+		inputs must be specified in the `args` parameter.
+
+	X: torch.tensor, shape=(1, len(alphabet), length)
+		A one-hot encoded sequence to use as the base for design. This must be
+		a single sequence and has the first dimension for broadcasting reasons.
+
+	motifs: list of strings
+		A list of strings where each string is a motif that can be inserted into
+		the sequence. These strings will be one-hot encoded according to the
+		provided alphabet.
+
+	y: torch.Tensor or list of torch.Tensors
+		A tensor or list of Tensors providing the desired output from the model.
+		The type and shape must be compatible with the provided loss function
+		and comparable to the output from `model`. Each tensor should have a
+		shape of (1, n) where n is the number of outputs from the model. The 
+		first dimension is 1 to make broadcasting work correctly.
+
+	loss: function
+		This function must take in `y` and `y_hat` where `y` is the desired
+		output from the model and `y_hat` is the current prediction from the
+		model given the substitutions. By default, this is the 
+		torch.nn.MSELoss().
+
+	mask: torch.Tensor
+		A mask on the outputs from the model to consider. True means to include
+		the outputs in the loss, False means to exclude those outputs from the
+		loss. If None, use all outputs. Default is None.
+
+	spacing: int or list or tuple
+		The spacing between the substituted motifs or the range of spacings
+		to try when inserting each of the next motifs.
+
+	tol: float
+		A threshold on the amount of improvement necessary according to loss,
+		where the procedure will stop once the improvement is below. Default
+		is 1e-3.
+
+	max_iter: int
+		The maximum number of iterations to run before terminating the
+		procedure. Set to -1 for no limit. Default is -1.
 
-	X: torch.tensor, shape=(-1, len(alphabet), length)
-		A one-hot encoded set of sequences to make predictions for.
-
-	args: tuple or list or None, optional
+	args: tuple or list or None
 		An optional set of additional arguments to pass into the model. If
 		provided, each element in the tuple or list is one input to the model
 		and the element must be formatted to be the same batch size as `X`. If
 		None, no additional arguments are passed into the forward function.
 		Default is None.
 
-	batch_size: int, optional
-		The number of examples to make predictions for at a time. Default is 32.
-
-	device: str or torch.device, optional
-		The device to move the model and batches to when making predictions. If
-		set to 'cuda' without a GPU, this function will crash and must be set
-		to 'cpu'. Default is 'cuda'. 
-
-	verbose: bool, optional
-		Whether to display a progress bar during predictions. Default is False.
-
-
-	Returns
-	-------
-	y: torch.Tensor or list/tuple of torch.Tensors
-		The output from the model for each input example. The precise format
-		is determined by the model. If the model outputs a single tensor,
-		y is a single tensor concatenated across all batches. If the model
-		outputs multiple tensors, y is a list of tensors which are each
-		concatenated across all batches.
-	"""
-
-	model = model.to(device).eval()
-
-	try:
-		dtype = next(model.parameters()).dtype
-	except:
-		dtype = X.dtype
-
-	y = []
-
-	with torch.no_grad():
-		batch_size = min(batch_size, X.shape[0])
-
-		for start in trange(0, X.shape[0], batch_size, disable=not verbose):
-			end = start + batch_size
-			X_ = X[start:end].to(device).type(dtype)
-
-			if X_.shape[0] == 0:
-				continue
-
-			if args is not None:
-				args_ = [a[start:end].to(device) for a in args]
-				y_ = model(X_, *args_)
-			else:
-				y_ = model(X_)
-
-			# Move to the CPU
-			if isinstance(y_, torch.Tensor):
-				y_ = y_.cpu()
-			elif isinstance(y_, (list, tuple)):
-				y_ = tuple(yi.cpu() for yi in y_)
-			else:
-				raise ValueError("Cannot interpret output from model.")
-
-			y.append(y_)
-
-
-	# Concatenate the outputs
-	if isinstance(y[0], torch.Tensor):
-		y = torch.cat(y)
-	else:
-		y = [torch.cat(y_) for y_ in list(zip(*y))]
-
-	return y
-
-
-def predict_cross(model, X, args, batch_size=32, device='cuda', verbose=False):
-	"""Make predictions for the cross between X and args.
-
-	This function will make predictions for the cross between the elements in X
-	and the elements in args. More specifically, for each element in X,
-	predictions will be made for each element in args. This function is useful
-	when you need to make predictions for the same sequence across a range of
-	conditions, for instance.
-
-
-	Parameters
-	----------
-	model: torch.nn.Module
-		The PyTorch model to use to make predictions.
-
-	X: torch.tensor, shape=(-1, len(alphabet), length)
-		A one-hot encoded set of sequences to make predictions for.
-
-	args: tuple or list
-		An optional set of additional arguments to pass into the model. If
-		provided, each element in the tuple or list is one input to the model
-		and the element must be formatted to be the same batch size as `X`. If
-		None, no additional arguments are passed into the forward function.
-		Default is None.
+	start: int or None, optional
+		The starting position of where to insert the motif. If None, insert the
+		motif into the middle of the sequence such that the middle of the motif
+		occurs at the middle of the sequence. Default is None.
+
+	alphabet : set or tuple or list, optional
+		A pre-defined alphabet where the ordering of the symbols is the same
+		as the index into the returned tensor, i.e., for the alphabet ['A', 'B']
+		the returned tensor will have a 1 at index 0 if the character was 'A'.
+		Characters outside the alphabet are ignored and none of the indexes are
+		set to 1. This is not necessary or used if a one-hot encoded tensor is
+		provided for the motif. Default is ['A', 'C', 'G', 'T'].
 
 	batch_size: int, optional
 		The number of examples to make predictions for at a time. Default is 32.
 
 	device: str or torch.device
 		The device to move the model and batches to when making predictions. If
 		set to 'cuda' without a GPU, this function will crash and must be set
@@ -141,54 +105,75 @@
 
 	verbose: bool, optional
 		Whether to display a progress bar during predictions. Default is False.
 
 
 	Returns
 	-------
-	y: torch.Tensor or list/tuple of torch.Tensors
-		The output from the model for each input example. The precise format
-		is determined by the model. If the model outputs a single tensor,
-		y is a single tensor concatenated across all batches. If the model
-		outputs multiple tensors, y is a list of tensors which are each
-		concatenated across all batches.
+	X: torch.Tensor, shape=(-1, len(alphabet), length)
+		The edited sequence. 
 	"""
 
-	y = []
-	n_seqs, n_args = X.shape[0], len(args[0])
-	seq_idxs, arg_idxs = list(zip(*itertools.product(range(n_seqs), 
-		range(n_args))))
-
-	model = model.to(device).eval()
-
-	with torch.no_grad():
-		batch_size = min(batch_size, len(seq_idxs))
-		for start in trange(0, len(seq_idxs), batch_size, disable=not verbose):
-			end = start + batch_size
-			sidxs, aidxs = list(seq_idxs[start:end]), list(arg_idxs[start:end])
-
-			if len(sidxs) == 0:
-				continue
-
-			X_ = X[sidxs].to(device)
-			args_ = [a[aidxs].to(device) for a in args]
-			y_ = model(X_, *args_)
-
-			# Move to the CPU
-			if isinstance(y_, torch.Tensor):
-				y_ = y_.cpu()
-			elif isinstance(y_, (list, tuple)):
-				y_ = tuple(yi.cpu() for yi in y_)
-			else:
-				raise ValueError("Cannot interpret output from model.")
-
-			y.append(y_)
-
-	# Concatenate the outputs
-	if isinstance(y[0], torch.Tensor):
-		y = torch.cat(y).reshape(n_seqs, n_args, *y[0].shape[1:])
-	else:
-		y = [torch.cat(y_).reshape(n_seqs, n_args, *y_[0].shape[1:]) 
-			for y_ in list(zip(*y))]
+	tic = time.time()
+	iteration = 0
+
+	y_orig = predict(model, X, args=args, batch_size=batch_size, device=device, 
+		verbose=verbose)
+	y = y.to(device)
+
+	mask = mask if mask is not None else torch.ones(y_orig.shape[1], dtype=bool)
+	mask = mask.to(device)
+
+	loss_prev = loss(y[:, mask], y_orig[:, mask]).mean()
+	loss_orig = loss_prev
+
+	if verbose:
+		print(("Iteration 0 -- Loss: {:4.4}, Improvement: N/A, Idx: N/A, " +
+			"Time (s): 0s").format(loss_prev, time.time() - tic))
+
+	while True:
+		if iteration == max_iter:
+			break
+
+		tic = time.time()
+		best_improvement, best_motif_idx, best_pos = 0, -1, -1
+		for idx, motif in enumerate(motifs):
+			X_ = torch.cat([substitute(X, motif, start=start, 
+				alphabet=alphabet) for start in range(X.shape[-1] - len(motif))
+			])
+
+			y_hat = predict(model, X_, args=args, batch_size=batch_size, 
+				device=device, verbose=False)
+			
+			loss_curr = loss(
+				y[:, mask].expand_as(y_hat[:, mask]), 
+				y_hat[:, mask],
+			).mean(dim=tuple(range(1, len(y_hat.shape))))
+
+			pos = loss_curr.argmin()
+			loss_curr = loss_curr[pos]
+
+			improvement = loss_prev - loss_curr
+			if improvement > best_improvement:
+				best_improvement = improvement
+				best_motif_idx = idx
+				best_pos = pos
+				best_loss = loss_curr
+
+
+		if best_motif_idx != -1:
+			X = substitute(X, motifs[best_motif_idx], start=best_pos, 
+				alphabet=alphabet)
+			loss_prev = best_loss
+
+			if verbose:
+				print(("Iteration {} -- Loss: {:4.4}, Improvement: {:4.4}, " + 
+					"Motif Idx: {}, Pos Idx: {}, Time (s): {:4.4}").format(
+						iteration+1, best_loss, best_improvement, 
+						best_motif_idx, best_pos, time.time() - tic))
+
+		if best_improvement <= tol:
+			break
 
+		iteration += 1
 
-	return y
+	return X
```

### Comparing `tangermeme-0.1.0rc0/tangermeme/tools/fimo.py` & `tangermeme-0.2.0/tangermeme/tools/fimo.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.1.0rc0/tangermeme/tools/tomtom.py` & `tangermeme-0.2.0/tangermeme/tools/tomtom.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.1.0rc0/tangermeme/utils.py` & `tangermeme-0.2.0/tangermeme/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 			max_value))
 
 	if ohe:
 		values = torch.unique(X)
 		if len(values) != 2:
 			raise ValueError("{} must be one-hot encoded.".format(name))
 
-		if not all(values == torch.tensor([0, 1])):
+		if not all(values == torch.tensor([0, 1], device=X.device)):
 			raise ValueError("{} must be one-hot encoded.".format(name))
 
 		if not (X.sum(axis=ohe_dim) == 1).all():
 			raise ValueError("{} must be one-hot encoded ".format(name) +
 				"and cannot have unknown characters.")
```

### Comparing `tangermeme-0.1.0rc0/tangermeme.egg-info/PKG-INFO` & `tangermeme-0.2.0/tangermeme.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tangermeme
-Version: 0.1.0rc0
+Version: 0.2.0
 Summary: Biological sequence analysis for the modern age.
 Home-page: https://github.com/jmschrei/tangermeme
 Author: Jacob Schreiber
 Author-email: jmschreiber91@gmail.com
 License: LICENSE.txt
 License-File: LICENSE
 Requires-Dist: numpy>=1.14.2
@@ -13,7 +13,8 @@
 Requires-Dist: pyBigWig>=0.3.17
 Requires-Dist: torch>=1.9.0
 Requires-Dist: pyfaidx>=0.7.2.1
 Requires-Dist: tqdm>=4.64.1
 Requires-Dist: numba>=0.55.1
 Requires-Dist: logomaker
 Requires-Dist: joblib>=1.3.2
+Requires-Dist: scikit-learn>=1.2.2
```

### Comparing `tangermeme-0.1.0rc0/tangermeme.egg-info/SOURCES.txt` & `tangermeme-0.2.0/tangermeme.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 LICENSE
 README.md
 setup.py
 tangermeme/__init__.py
+tangermeme/ablate.py
+tangermeme/deep_lift_shap.py
+tangermeme/design.py
 tangermeme/ersatz.py
 tangermeme/io.py
 tangermeme/ism.py
 tangermeme/kmers.py
 tangermeme/marginalize.py
 tangermeme/match.py
 tangermeme/plot.py
 tangermeme/predict.py
+tangermeme/product.py
+tangermeme/seqlet.py
 tangermeme/space.py
 tangermeme/utils.py
 tangermeme/variant_effect.py
 tangermeme.egg-info/PKG-INFO
 tangermeme.egg-info/SOURCES.txt
 tangermeme.egg-info/dependency_links.txt
 tangermeme.egg-info/requires.txt
 tangermeme.egg-info/top_level.txt
 tangermeme/tools/__init__.py
 tangermeme/tools/fimo.py
 tangermeme/tools/tomtom.py
+tests/test_ablate.py
+tests/test_deep_lift_shap.py
 tests/test_ersatz.py
 tests/test_io.py
 tests/test_ism.py
 tests/test_kmers.py
 tests/test_marginalize.py
 tests/test_match.py
 tests/test_predict.py
+tests/test_product.py
+tests/test_seqlet.py
 tests/test_space.py
 tests/test_utils.py
 tests/test_variant_effect.py
```

### Comparing `tangermeme-0.1.0rc0/tests/test_ersatz.py` & `tangermeme-0.2.0/tests/test_ersatz.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.1.0rc0/tests/test_io.py` & `tangermeme-0.2.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.1.0rc0/tests/test_kmers.py` & `tangermeme-0.2.0/tests/test_kmers.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.1.0rc0/tests/test_match.py` & `tangermeme-0.2.0/tests/test_match.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.1.0rc0/tests/test_space.py` & `tangermeme-0.2.0/tests/test_product.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,33 @@
-# test_marginalize.py
+# test_predict.py
 # Contact: Jacob Schreiber <jmschreiber91@gmail.com>
 
 import numpy
 import torch
 import pytest
 
 from tangermeme.utils import one_hot_encode
 from tangermeme.utils import random_one_hot
 
 from tangermeme.space import space
-from tangermeme.space import space_cross
-
+from tangermeme.predict import predict
+from tangermeme.product import apply_product
 from tangermeme.marginalize import marginalize
-from tangermeme.marginalize import marginalize_cross
 
 from .toy_models import SumModel
 from .toy_models import FlattenDense
 from .toy_models import Conv
 from .toy_models import Scatter
 from .toy_models import ConvDense
 
 from numpy.testing import assert_raises
 from numpy.testing import assert_array_almost_equal
 
-
 torch.manual_seed(0)
-torch.use_deterministic_algorithms(True)
+torch.use_deterministic_algorithms(True, warn_only=True)
 
 
 @pytest.fixture
 def X():
 	return random_one_hot((64, 4, 100), random_state=0).type(torch.float32)
 
 
@@ -40,561 +38,745 @@
 
 @pytest.fixture
 def beta():
 	r = numpy.random.RandomState(1)
 	return torch.from_numpy(r.randn(64, 1)).type(torch.float32)
 
 
-##
-
-def test_space_summodel(X):
-	torch.manual_seed(0)
-	model = SumModel()
-	y_before, y_after = space(model, X, ["ACGTC", "GAGA"], 1, 
-		batch_size=5, device='cpu')
-
-	assert y_before.shape == (64, 4)
-	assert y_before.dtype == torch.float32
-	assert y_before.sum() == X.sum()
-	assert_array_almost_equal(y_before[:8], [
-		[25., 24., 19., 32.],
-        [26., 18., 29., 27.],
-        [28., 25., 21., 26.],
-        [21., 33., 19., 27.],
-        [27., 22., 23., 28.],
-        [31., 27., 21., 21.],
-        [26., 20., 21., 33.],
-        [21., 28., 31., 20.]])
-
-	assert y_after.shape == (64, 4)
-	assert y_after.dtype == torch.float32
-	assert y_after.sum() == X.sum()
-	assert_array_almost_equal(y_after[:8], [
-		[28., 22., 21., 29.],
-        [28., 18., 29., 25.],
-        [28., 24., 23., 25.],
-        [21., 34., 19., 26.],
-        [27., 22., 25., 26.],
-        [28., 29., 22., 21.],
-        [28., 17., 23., 32.],
-        [22., 28., 32., 18.]])
-
-	y_before2, y_after2 = space(model, X, ["ACGTC", "GAGA"], 1, 
-		batch_size=64, device='cpu')
-	assert_array_almost_equal(y_before, y_before2)
-	assert_array_almost_equal(y_after, y_after2)	
+###
 
 
-def test_space_flattendense(X):
+def test_apply_product_predict_flattendense_alpha(X, alpha, beta):
 	torch.manual_seed(0)
 	model = FlattenDense()
-	y_before, y_after = space(model, X, ["ACGTC", "GAGA"], 1, 
-		batch_size=5, device='cpu')
-
-	assert y_before.shape == (64, 3)
-	assert y_before.dtype == torch.float32
-	assert_array_almost_equal(y_before[:8], [
-		[ 0.1928,  0.2788, -0.1000],
-        [-0.0505,  0.0174, -0.1751],
-        [-0.1408,  0.0105,  0.0673],
-        [-0.2375, -0.0069,  0.0835],
-        [ 0.0442, -0.0692, -0.1565],
-        [-0.3489, -0.0876, -0.2994],
-        [-0.3894, -0.1332, -0.3717],
-        [-0.3682,  0.5173, -0.4089]], 4)
-
-	assert y_after.shape == (64, 3)
-	assert y_after.dtype == torch.float32
-	assert_array_almost_equal(y_after[:8], [
-		[ 0.1087,  0.3662,  0.0668],
-        [-0.1331,  0.0071, -0.0907],
-        [-0.3239,  0.0593,  0.1154],
-        [-0.3762,  0.0659,  0.0011],
-        [-0.1361, -0.0605, -0.0853],
-        [-0.4873, -0.1080, -0.3462],
-        [-0.3656, -0.0071, -0.1459],
-        [-0.4935,  0.6714, -0.3008]], 4)
-
-	y_before2, y_after2 = space(model, X, ["ACGTC", "GAGA"], 1, 
-		batch_size=64, device='cpu')
-	assert_array_almost_equal(y_before, y_before2)
-	assert_array_almost_equal(y_after, y_after2)
-
-
-def test_space_conv(X):
-	torch.manual_seed(0)
-	model = Conv()
-	y_before, y_after = space(model, X, ["ACGTC", "GAGA"], 1, 
-		start=0, batch_size=5, device='cpu')
-
-	assert y_before.shape == (64, 12, 98)
-	assert y_before.dtype == torch.float32
-	assert_array_almost_equal(y_before[:2, :4, :10], [
-		[[-0.2713, -0.5317, -0.3737, -0.4055, -0.3269, -0.3269, -0.1928,
-          -0.3509, -0.4816, -0.3197],
-         [-0.2988,  0.0980, -0.1013, -0.2560,  0.2595,  0.2595,  0.2167,
-           0.4330, -0.0124,  0.3218],
-         [-0.1247,  0.1433, -0.3111, -0.3220, -0.4084, -0.4084, -0.2111,
-          -0.3884, -0.3460, -0.3052],
-         [-0.1362, -0.0067,  0.5554,  0.1810,  0.2007,  0.2007, -0.1166,
-           0.0337,  0.1722, -0.3441]],
-
-        [[-0.4805, -0.1669, -0.5863, -0.0537, -0.2702, -0.1669, -0.4055,
-          -0.5078, -0.0848, -0.5863],
-         [-0.3709, -0.3077, -0.5910,  0.0165, -0.6573, -0.3077, -0.2560,
-          -0.0755,  0.1277, -0.5910],
-         [ 0.4396, -0.1558,  0.2097, -0.0929,  0.6608, -0.1558, -0.3220,
-           0.1234, -0.1761,  0.2097],
-         [-0.0027,  0.4644,  0.1406, -0.1111, -0.3111,  0.4644,  0.1810,
-           0.1603,  0.2667,  0.1406]]], 4)
-
-	assert y_after.shape == (64, 12, 98)
-	assert y_after.dtype == torch.float32
-	assert_array_almost_equal(y_after[:2, :4, :10], [
-		[[-0.3983, -0.2996, -0.2749, -0.3509, -0.5846, -0.1916, -0.1358,
-          -0.2702, -0.0328, -0.3983],
-         [-0.1937, -0.0358, -0.2188,  0.4330, -0.0807, -0.1418, -0.4189,
-          -0.6573, -0.3505, -0.1937],
-         [-0.2188, -0.0922, -0.1907, -0.3884, -0.4600,  0.5745, -0.0725,
-           0.6608,  0.0415, -0.2188],
-         [-0.3638,  0.0378,  0.0811,  0.0337,  0.1116, -0.2914,  0.0865,
-          -0.3111,  0.1471, -0.3638]],
-
-        [[-0.3983, -0.2996, -0.2749, -0.3197, -0.2685, -0.2737, -0.1358,
-          -0.2702, -0.1669, -0.5863],
-         [-0.1937, -0.0358, -0.2188,  0.3218, -0.1470, -0.5773, -0.4189,
-          -0.6573, -0.3077, -0.5910],
-         [-0.2188, -0.0922, -0.1907, -0.3052, -0.0089,  0.5948, -0.0725,
-           0.6608, -0.1558,  0.2097],
-         [-0.3638,  0.0378,  0.0811, -0.3441, -0.3401, -0.0938,  0.0865,
-          -0.3111,  0.4644,  0.1406]]], 4)
-
-	y_before2, y_after2 = space(model, X, ["ACGTC", "GAGA"], 1, 
-		start=0, batch_size=64, device='cpu')
-	assert_array_almost_equal(y_before, y_before2)
-	assert_array_almost_equal(y_after, y_after2)
-
-
-def test_space_scatter(X):
-	torch.manual_seed(0)
-	model = Scatter()
-	y_before, y_after = space(model, X, ["ACGTC", "GAGA"], 1, 
-		start=0, batch_size=8, device='cpu')
-
-	assert y_before.shape == (64, 100, 4)
-	assert y_before.dtype == torch.float32
-	assert y_before.sum() == X.sum()
-	assert (y_before.sum(axis=-1) == X.sum(axis=1)).all()
-	assert (y_before.sum(axis=1) == X.sum(axis=-1)).all()
-	assert_array_almost_equal(y_before[:4, :5], [
-		[[1., 0., 0., 0.],
-         [0., 0., 0., 1.],
-         [0., 1., 0., 0.],
-         [1., 0., 0., 0.],
-         [0., 0., 0., 1.]],
-
-        [[0., 1., 0., 0.],
-         [0., 0., 1., 0.],
-         [1., 0., 0., 0.],
-         [0., 0., 0., 1.],
-         [1., 0., 0., 0.]],
-
-        [[0., 1., 0., 0.],
-         [0., 0., 1., 0.],
-         [0., 0., 0., 1.],
-         [0., 0., 1., 0.],
-         [0., 0., 1., 0.]],
-
-        [[0., 1., 0., 0.],
-         [1., 0., 0., 0.],
-         [0., 0., 0., 1.],
-         [1., 0., 0., 0.],
-         [0., 0., 1., 0.]]], 4)
-
-	assert y_after.shape == (64, 100, 4)
-	assert y_after.dtype == torch.float32
-	assert y_after.sum() == X.sum()
-	assert_array_almost_equal(y_after[:4, :5], [
-		[[1., 0., 0., 0.],
-         [0., 1., 0., 0.],
-         [0., 0., 1., 0.],
-         [0., 0., 0., 1.],
-         [0., 1., 0., 0.]],
-
-        [[1., 0., 0., 0.],
-         [0., 1., 0., 0.],
-         [0., 0., 1., 0.],
-         [0., 0., 0., 1.],
-         [0., 1., 0., 0.]],
-
-        [[1., 0., 0., 0.],
-         [0., 1., 0., 0.],
-         [0., 0., 1., 0.],
-         [0., 0., 0., 1.],
-         [0., 1., 0., 0.]],
-
-        [[1., 0., 0., 0.],
-         [0., 1., 0., 0.],
-         [0., 0., 1., 0.],
-         [0., 0., 0., 1.],
-         [0., 1., 0., 0.]]], 4)
-
-	y_before2, y_after2 = space(model, X, ["ACGTC", "GAGA"], 1, 
-		start=0, batch_size=64, device='cpu')
-	assert_array_almost_equal(y_before, y_before2)
-	assert_array_almost_equal(y_after, y_after2)
+	y0 = predict(model, X, device='cpu').unsqueeze(1)
+	y = apply_product(predict, model, X, args=(alpha[:5],), device='cpu')
+	assert y.shape == (64, 5, 3)
+	assert y.dtype == torch.float32
+	assert_array_almost_equal(y, y0 + alpha[:5][None, :])
+	assert_array_almost_equal(y[:2], [
+		[[1.9569, 2.0429, 1.6640],
+		 [0.5930, 0.6790, 0.3001],
+		 [1.1715, 1.2575, 0.8787],
+		 [2.4337, 2.5197, 2.1409],
+		 [2.0604, 2.1464, 1.7675]],
+
+		[[1.7136, 1.7814, 1.5889],
+		 [0.3497, 0.4175, 0.2250],
+		 [0.9283, 0.9961, 0.8036],
+		 [2.1904, 2.2583, 2.0658],
+		 [1.8171, 1.8849, 1.6924]]], 4)
+
+
+	y = apply_product(predict, model, X, args=(alpha[5:10],), device='cpu')
+	assert y.shape == (64, 5, 3)
+	assert y.dtype == torch.float32
+	assert_array_almost_equal(y, y0 + alpha[5:10][None, :])
+	assert_array_almost_equal(y[:2], [
+		[[-0.7845, -0.6985, -1.0773],
+		 [ 1.1429,  1.2289,  0.8501],
+		 [ 0.0414,  0.1274, -0.2514],
+		 [ 0.0896,  0.1756, -0.2032],
+		 [ 0.6034,  0.6894,  0.3106]],
+
+		[[-1.0278, -0.9599, -1.1524],
+		 [ 0.8996,  0.9674,  0.7750],
+		 [-0.2018, -0.1340, -0.3265],
+		 [-0.1537, -0.0859, -0.2783],
+		 [ 0.3601,  0.4280,  0.2355]]], 4)
 
 
-def test_space_convdense(X):
+def test_apply_product_predict_flattendense_beta(X, alpha, beta):
 	torch.manual_seed(0)
-	model = ConvDense()
-	y_before, y_after = space(model, X, ["ACGTC", "GAGA"], 1, 
-		start=0, batch_size=2, device='cpu')
-
-	assert len(y_before) == 2
-	assert y_before[0].shape == (64, 12, 98)
-	assert y_before[1].shape == (64, 3)
-
-	assert y_before[0].dtype == torch.float32
-	assert y_before[1].dtype == torch.float32
+	model = FlattenDense()
+	alpha = torch.zeros(X.shape[0], 1)
 
-	assert_array_almost_equal(y_before[0][:2, :4, :4], [
-		[[-0.7757,  0.0397, -0.8799, -1.0194],
-         [ 0.0947,  0.2042, -0.2302, -0.3144],
-         [ 0.3781,  0.5009,  0.8585,  0.6738],
-         [-0.5986, -0.0296, -0.0995, -0.2718]],
-
-        [[-0.6676, -0.8873, -0.8696, -0.4684],
-         [-0.0768, -0.0089,  0.0244,  0.1355],
-         [ 0.4828,  0.5419,  0.3170,  0.3288],
-         [-0.1026, -0.4676, -0.3080, -0.2606]]], 4)
+	y0 = predict(model, X, device='cpu').unsqueeze(1)
+	y = apply_product(predict, model, X, args=(alpha[:1], beta[:5]), 
+		device='cpu')[:, 0]
+	
+	assert y.shape == (64, 5, 3)
+	assert y.dtype == torch.float32
+	assert_array_almost_equal(y, y0 * beta[:5][None, :])
+	assert_array_almost_equal(y[:2], [
+		[[ 0.3132,  0.4529, -0.1624],
+		 [-0.1179, -0.1706,  0.0612],
+		 [-0.1018, -0.1473,  0.0528],
+		 [-0.2069, -0.2991,  0.1073],
+		 [ 0.1669,  0.2413, -0.0865]],
+
+		[[-0.0820,  0.0282, -0.2845],
+		 [ 0.0309, -0.0106,  0.1071],
+		 [ 0.0267, -0.0092,  0.0925],
+		 [ 0.0542, -0.0186,  0.1879],
+		 [-0.0437,  0.0150, -0.1516]]], 4)
 
-	assert_array_almost_equal(y_before[1][:4], [
-		[ 0.1928,  0.2788, -0.1000],
-        [-0.0505,  0.0174, -0.1751],
-        [-0.1408,  0.0105,  0.0673],
-        [-0.2375, -0.0069,  0.0835]], 4)
 
-	assert len(y_after) == 2
-	assert y_after[0].shape == (64, 12, 98)
-	assert y_after[1].shape == (64, 3)
+	y = apply_product(predict, model, X, args=(alpha[:2], beta[5:10]), 
+		device='cpu')
+	assert y.shape == (64, 2, 5, 3)
+	assert y.dtype == torch.float32
+	assert_array_almost_equal(y[:, 0], y0 * beta[5:10][None, :])
+	assert_array_almost_equal(y[:2], [
+		[[[-0.4437, -0.6417,  0.2302],
+		  [ 0.3364,  0.4865, -0.1745],
+		  [-0.1468, -0.2122,  0.0761],
+		  [ 0.0615,  0.0889, -0.0319],
+		  [-0.0481, -0.0695,  0.0249]],
+
+		 [[-0.4437, -0.6417,  0.2302],
+		  [ 0.3364,  0.4865, -0.1745],
+		  [-0.1468, -0.2122,  0.0761],
+		  [ 0.0615,  0.0889, -0.0319],
+		  [-0.0481, -0.0695,  0.0249]]],
+
+
+		[[[ 0.1162, -0.0400,  0.4030],
+		  [-0.0881,  0.0303, -0.3056],
+		  [ 0.0384, -0.0132,  0.1333],
+		  [-0.0161,  0.0055, -0.0559],
+		  [ 0.0126, -0.0043,  0.0437]],
+
+		 [[ 0.1162, -0.0400,  0.4030],
+		  [-0.0881,  0.0303, -0.3056],
+		  [ 0.0384, -0.0132,  0.1333],
+		  [-0.0161,  0.0055, -0.0559],
+		  [ 0.0126, -0.0043,  0.0437]]]], 4)
 
-	assert y_after[0].dtype == torch.float32
-	assert y_after[1].dtype == torch.float32
 
-	assert_array_almost_equal(y_after[0][:2, :4, :4], [
-		[[-3.8092e-01, -8.1744e-01, -7.0452e-01, -1.1013e-01],
-         [-1.7080e-01, -4.1553e-01,  4.2124e-01, -1.3453e-01],
-         [ 4.8191e-01,  8.3968e-01,  1.5083e-01,  8.5779e-01],
-         [-7.7912e-01, -6.6461e-02, -6.1201e-01,  6.5689e-03]],
-
-        [[-3.8092e-01, -8.1744e-01, -7.0452e-01, -4.2652e-04],
-         [-1.7080e-01, -4.1553e-01,  4.2124e-01,  8.2816e-02],
-         [ 4.8191e-01,  8.3968e-01,  1.5083e-01,  4.4968e-01],
-         [-7.7912e-01, -6.6461e-02, -6.1201e-01, -2.8948e-01]]], 4)
+def test_apply_product_predict_flattendense_alpha_beta(X, alpha, beta):
+	torch.manual_seed(0)
+	model = FlattenDense()
+	y0 = predict(model, X, device='cpu').unsqueeze(1).unsqueeze(1)
+	y = apply_product(predict, model, X, args=(alpha[:5], beta[:4]), 
+		device='cpu')
 
-	assert_array_almost_equal(y_after[1][:4], [
-		[ 0.2248,  0.2780,  0.0710],
-        [-0.1218,  0.1338, -0.2101],
-        [-0.1292,  0.1851,  0.2033],
-        [-0.2042,  0.1904,  0.2121]], 4)
+	assert y.shape == (64, 5, 4, 3)
+	assert y.dtype == torch.float32
+	assert_array_almost_equal(y, y0 * beta[None, None, :4] + alpha[None, :5, None])
+	assert_array_almost_equal(y[:2], [[[[2.0772, 2.2169, 1.6016],
+		  [1.6461, 1.5935, 1.8252],
+		  [1.6622, 1.6168, 1.8169],
+		  [1.5572, 1.4649, 1.8714]],
+
+		 [[0.7133, 0.8530, 0.2377],
+		  [0.2822, 0.2296, 0.4613],
+		  [0.2983, 0.2529, 0.4530],
+		  [0.1933, 0.1010, 0.5075]],
+
+		 [[1.2919, 1.4316, 0.8163],
+		  [0.8608, 0.8082, 1.0399],
+		  [0.8769, 0.8315, 1.0316],
+		  [0.7719, 0.6796, 1.0860]],
+
+		 [[2.5541, 2.6938, 2.0784],
+		  [2.1229, 2.0703, 2.3021],
+		  [2.1391, 2.0936, 2.2937],
+		  [2.0340, 1.9417, 2.3482]],
+
+		 [[2.1807, 2.3204, 1.7051],
+		  [1.7496, 1.6970, 1.9287],
+		  [1.7657, 1.7203, 1.9204],
+		  [1.6607, 1.5684, 1.9749]]],
+
+
+		[[[1.6821, 1.7923, 1.4796],
+		  [1.7949, 1.7534, 1.8712],
+		  [1.7907, 1.7549, 1.8565],
+		  [1.8182, 1.7454, 1.9520]],
+
+		 [[0.3182, 0.4284, 0.1157],
+		  [0.4310, 0.3895, 0.5073],
+		  [0.4268, 0.3910, 0.4927],
+		  [0.4543, 0.3815, 0.5881]],
+
+		 [[0.8968, 1.0069, 0.6943],
+		  [1.0096, 0.9681, 1.0859],
+		  [1.0054, 0.9696, 1.0712],
+		  [1.0329, 0.9601, 1.1666]],
+
+		 [[2.1589, 2.2691, 1.9564],
+		  [2.2718, 2.2303, 2.3480],
+		  [2.2676, 2.2317, 2.3334],
+		  [2.2951, 2.2223, 2.4288]],
+
+		 [[1.7856, 1.8958, 1.5831],
+		  [1.8984, 1.8569, 1.9747],
+		  [1.8942, 1.8584, 1.9601],
+		  [1.9217, 1.8489, 2.0555]]]], 4)
 
 
-def test_space_convdense_batch_size(X):
+def test_apply_product_predict_convdense_alpha(X, alpha):
 	torch.manual_seed(0)
 	model = ConvDense()
-	y_before, y_after = space(model, X, ["ACGTC", "GAGA"], 1, 
-		batch_size=68, device='cpu')
 
-	assert len(y_before) == 2
-	assert y_before[0].shape == (64, 12, 98)
-	assert y_before[1].shape == (64, 3)
+	y = apply_product(predict, model, X, args=(alpha[:5, :, None],), 
+		batch_size=2, device='cpu')
 
-	assert len(y_after) == 2
-	assert y_after[0].shape == (64, 12, 98)
-	assert y_after[1].shape == (64, 3)
+	assert len(y) == 2
+	assert y[0].shape == (64, 5, 12, 98)
+	assert y[1].shape == (64, 5, 3)
 
+	assert y[0].dtype == torch.float32
+	assert y[1].dtype == torch.float32
 
-def test_space_scatter_batch_size(X):
-	torch.manual_seed(0)
-	model = Scatter()
-	y_before, y_after = space(model, X, ["ACGTC", "GAGA"], 1, 
-		batch_size=68, device='cpu')
+	assert_array_almost_equal(y[0][:2, :2, :3, :4], [
+		[[[ 0.9883,  1.8037,  0.8841,  0.7446],
+		  [ 1.8588,  1.9683,  1.5339,  1.4497],
+		  [ 2.1421,  2.2650,  2.6226,  2.4379]],
 
-	assert y_before.shape == (64, 100, 4)
-	assert y_after.shape == (64, 100, 4)
+		 [[-0.3756,  0.4398, -0.4798, -0.6192],
+		  [ 0.4949,  0.6044,  0.1700,  0.0858],
+		  [ 0.7782,  0.9011,  1.2587,  1.0740]]],
 
 
-def test_space_raises_shape(X):
-	torch.manual_seed(0)
-	model = Scatter()
-	assert_raises(ValueError, space, model, X[0], ["ACGTC", "ACC"], 0, 
-		device='cpu')
-	assert_raises(ValueError, space, model, X[:, 0], ["ACGTC", "ACC"], 0,
-		device='cpu')
-	assert_raises(ValueError, space, model, X.unsqueeze(0), ["ACGTC", "ACC"], 
-		0, device='cpu')
+		[[[ 1.0964,  0.8767,  0.8945,  1.2957],
+		  [ 1.6873,  1.7551,  1.7884,  1.8996],
+		  [ 2.2469,  2.3060,  2.0810,  2.0929]],
 
+		 [[-0.2675, -0.4872, -0.4694, -0.0682],
+		  [ 0.3234,  0.3912,  0.4245,  0.5357],
+		  [ 0.8830,  0.9421,  0.7171,  0.7290]]]], 4)
 
-def test_space_raises_args(X, alpha, beta):
-	torch.manual_seed(0)
-	model = FlattenDense()
-	assert_raises(ValueError, space, model, X, ["ACGTC", "ACC"], [0, 1], 
-		batch_size=2, device='cpu')
-	assert_raises(ValueError, space, model, X, ["ACGTC", "ACC"], [-5], 
-		batch_size=2, device='cpu')
-	assert_raises(ValueError, space, model, X, ["ACGTC", "ACC"], -3, 
-		batch_size=2, device='cpu')
-	assert_raises(ValueError, space, model, X, ["ACGTC", "ACC"], [], 
-		batch_size=2, device='cpu')
-	assert_raises(ValueError, space, model, X, ["ACGTC", "ACC"], [1500], 
-		batch_size=2, device='cpu')
-
-	assert_raises(TypeError, space, model, X, ["ACGTC", "ACC"], 0, 
-		batch_size=2, args=5, device='cpu')
-	assert_raises(TypeError, space, model, X, ["ACGTC", "ACC"], 0, 
-		batch_size=2, args=(5,), device='cpu')
-	assert_raises(TypeError, space, model, X, ["ACGTC", "ACC"], 0, 
-		batch_size=2, args=alpha, device='cpu')
-	assert_raises(RuntimeError, space, model, X, ["ACGTC", "ACC"], 0,
-		batch_size=2, args=(alpha[:5],), device='cpu')
-	assert_raises(RuntimeError, space, model, X, ["ACGTC", "ACC"], 0, 
-		batch_size=2, args=(alpha, beta[:5]), device='cpu')
+	assert_array_almost_equal(y[1][:4], [
+		[[ 0.1928,  0.2788, -0.1000],
+		 [ 0.1928,  0.2788, -0.1000],
+		 [ 0.1928,  0.2788, -0.1000],
+		 [ 0.1928,  0.2788, -0.1000],
+		 [ 0.1928,  0.2788, -0.1000]],
+
+		[[-0.0505,  0.0174, -0.1751],
+		 [-0.0505,  0.0174, -0.1751],
+		 [-0.0505,  0.0174, -0.1751],
+		 [-0.0505,  0.0174, -0.1751],
+		 [-0.0505,  0.0174, -0.1751]],
+
+		[[-0.1408,  0.0105,  0.0673],
+		 [-0.1408,  0.0105,  0.0673],
+		 [-0.1408,  0.0105,  0.0673],
+		 [-0.1408,  0.0105,  0.0673],
+		 [-0.1408,  0.0105,  0.0673]],
+
+		[[-0.2375, -0.0069,  0.0835],
+		 [-0.2375, -0.0069,  0.0835],
+		 [-0.2375, -0.0069,  0.0835],
+		 [-0.2375, -0.0069,  0.0835],
+		 [-0.2375, -0.0069,  0.0835]]], 4)
 
 
 ###
 
 
-def test_space_cross_flattendense_alpha(X, alpha, beta):
+def test_apply_product_marginalize_flattendense_alpha(X, alpha, beta):
 	torch.manual_seed(0)
 	model = FlattenDense()
-	y0_before, y0_after = space(model, X, ['ACGTGC', 'TGTT'], 3, 
-		device='cpu')
-	y_before, y_after = space_cross(model, X, ['ACGTGC', 'TGTT'], 3, 
-		(alpha[:5],), device='cpu')
+	y0_before, y0_after = marginalize(model, X, 'ACGTGC', device='cpu')
+	y_before, y_after = apply_product(marginalize, model, X, 'ACGTGC', 
+		args=(alpha[:5],), device='cpu')
 
 	assert y_before.shape == (64, 5, 3)
 	assert y_before.dtype == torch.float32
 	assert_array_almost_equal(y_before, y0_before[:, None] + alpha[:5][None, :])
 	assert_array_almost_equal(y_before[:2], [
 		[[1.9569, 2.0429, 1.6640],
-         [0.5930, 0.6790, 0.3001],
-         [1.1715, 1.2575, 0.8787],
-         [2.4337, 2.5197, 2.1409],
-         [2.0604, 2.1464, 1.7675]],
-
-        [[1.7136, 1.7814, 1.5889],
-         [0.3497, 0.4175, 0.2250],
-         [0.9283, 0.9961, 0.8036],
-         [2.1904, 2.2583, 2.0658],
-         [1.8171, 1.8849, 1.6924]]], 4)
-
+		 [0.5930, 0.6790, 0.3001],
+		 [1.1715, 1.2575, 0.8787],
+		 [2.4337, 2.5197, 2.1409],
+		 [2.0604, 2.1464, 1.7675]],
+
+		[[1.7136, 1.7814, 1.5889],
+		 [0.3497, 0.4175, 0.2250],
+		 [0.9283, 0.9961, 0.8036],
+		 [2.1904, 2.2583, 2.0658],
+		 [1.8171, 1.8849, 1.6924]]], 4)
 
 	assert y_after.shape == (64, 5, 3)
 	assert y_after.dtype == torch.float32
 	assert_array_almost_equal(y_after, y0_after[:, None] + alpha[:5][None, :])
 	assert_array_almost_equal(y_after[:2], [
-		[[1.9143, 1.9713, 1.6641],
-         [0.5504, 0.6074, 0.3002],
-         [1.1290, 1.1860, 0.8788],
-         [2.3912, 2.4481, 2.1409],
-         [2.0178, 2.0748, 1.7676]],
+		[[1.9098, 2.0546, 1.9081],
+		 [0.5459, 0.6907, 0.5442],
+		 [1.1245, 1.2693, 1.1228],
+		 [2.3867, 2.5314, 2.3850],
+		 [2.0133, 2.1581, 2.0116]],
 
-        [[1.7369, 1.6794, 1.6200],
-         [0.3730, 0.3156, 0.2561],
-         [0.9516, 0.8941, 0.8347],
-         [2.2137, 2.1563, 2.0968],
-         [1.8404, 1.7830, 1.7235]]], 4)
+		[[1.6194, 1.7230, 1.7036],
+		 [0.2555, 0.3591, 0.3397],
+		 [0.8341, 0.9377, 0.9183],
+		 [2.0962, 2.1999, 2.1805],
+		 [1.7229, 1.8265, 1.8071]]], 4)
 
 
 
-def test_space_cross_flattendense_beta(X, alpha, beta):
+def test_apply_product_marginalize_flattendense_beta(X, beta):
 	torch.manual_seed(0)
 	model = FlattenDense()
 	alpha = torch.zeros(X.shape[0], 1)
 
-	y0_before, y0_after = space(model, X, ['ACGTGC', 'TGTT'], 3, 
-		device='cpu')
-	y_before, y_after = space_cross(model, X, ['ACGTGC', 'TGTT'], 3, 
-		(alpha[:5], beta[:5]), device='cpu')
+	y0_before, y0_after = marginalize(model, X, 'ACGTGC', device='cpu')
+	y_before, y_after = apply_product(marginalize, model, X, 'ACGTGC', 
+		args=(alpha[:1], beta[:5]), device='cpu')
+	y_before, y_after = y_before[:, 0], y_after[:, 0]
 
 	assert y_before.shape == (64, 5, 3)
 	assert y_before.dtype == torch.float32
 	assert_array_almost_equal(y_before, y0_before[:, None] * beta[:5][None, :])
 	assert_array_almost_equal(y_before[:2], [
 		[[ 0.3132,  0.4529, -0.1624],
-         [-0.1179, -0.1706,  0.0612],
-         [-0.1018, -0.1473,  0.0528],
-         [-0.2069, -0.2991,  0.1073],
-         [ 0.1669,  0.2413, -0.0865]],
-
-        [[-0.0820,  0.0282, -0.2845],
-         [ 0.0309, -0.0106,  0.1071],
-         [ 0.0267, -0.0092,  0.0925],
-         [ 0.0542, -0.0186,  0.1879],
-         [-0.0437,  0.0150, -0.1516]]], 4)
+		 [-0.1179, -0.1706,  0.0612],
+		 [-0.1018, -0.1473,  0.0528],
+		 [-0.2069, -0.2991,  0.1073],
+		 [ 0.1669,  0.2413, -0.0865]],
+
+		[[-0.0820,  0.0282, -0.2845],
+		 [ 0.0309, -0.0106,  0.1071],
+		 [ 0.0267, -0.0092,  0.0925],
+		 [ 0.0542, -0.0186,  0.1879],
+		 [-0.0437,  0.0150, -0.1516]]], 4)
 
 	assert y_after.shape == (64, 5, 3)
 	assert y_after.dtype == torch.float32
 	assert_array_almost_equal(y_after, y0_after[:, None] * beta[:5][None, :])
 	assert_array_almost_equal(y_after[:2], [
-		[[ 0.2441,  0.3366, -0.1624],
-         [-0.0919, -0.1268,  0.0612],
-         [-0.0794, -0.1095,  0.0528],
-         [-0.1613, -0.2224,  0.1073],
-         [ 0.1301,  0.1793, -0.0865]],
-
-        [[-0.0441, -0.1374, -0.2340],
-         [ 0.0166,  0.0518,  0.0881],
-         [ 0.0143,  0.0447,  0.0761],
-         [ 0.0291,  0.0908,  0.1546],
-         [-0.0235, -0.0732, -0.1247]]], 4)
+		[[ 0.2368,  0.4720,  0.2340],
+		 [-0.0892, -0.1777, -0.0881],
+		 [-0.0770, -0.1535, -0.0761],
+		 [-0.1564, -0.3118, -0.1546],
+		 [ 0.1262,  0.2514,  0.1247]],
+
+		[[-0.2350, -0.0666, -0.0981],
+		 [ 0.0885,  0.0251,  0.0370],
+		 [ 0.0764,  0.0217,  0.0319],
+		 [ 0.1552,  0.0440,  0.0648],
+		 [-0.1252, -0.0355, -0.0523]]], 4)
 
 
-def test_space_cross_flattendense_alpha_beta(X, alpha, beta):
+def test_apply_product_marginalize_flattendense_alpha_beta(X, alpha, beta):
 	torch.manual_seed(0)
 	model = FlattenDense()
-	y0_before, y0_after = space(model, X, ['ACGTGC', 'TGTT'], 3, 
-		device='cpu')
-	y_before, y_after = space_cross(model, X, ['ACGTGC', 'TGTT'], 3, 
-		(alpha[:5], beta[:5]), device='cpu')
+	y0_before, y0_after = marginalize(model, X, 'ACGTGC', device='cpu')
+	y_before, y_after = apply_product(marginalize, model, X, 'ACGTGC', 
+		args=(alpha[:5], beta[:4]), device='cpu')
 
-	assert y_before.shape == (64, 5, 3)
+	assert y_before.shape == (64, 5, 4, 3)
 	assert y_before.dtype == torch.float32
-	assert_array_almost_equal(y_before, y0_before[:, None] * beta[:5][None, :]
-		+ alpha[:5][None, :])
-	assert_array_almost_equal(y_before[:2], [
-		[[2.0772, 2.2169, 1.6016],
-         [0.2822, 0.2296, 0.4613],
-         [0.8769, 0.8315, 1.0316],
-         [2.0340, 1.9417, 2.3482],
-         [2.0344, 2.1088, 1.7810]],
-
-        [[1.6821, 1.7923, 1.4796],
-         [0.4310, 0.3895, 0.5073],
-         [1.0054, 0.9696, 1.0712],
-         [2.2951, 2.2223, 2.4288],
-         [1.8239, 1.8826, 1.7160]]], 4)
+	assert_array_almost_equal(y_before, y0_before[:, None, None] * 
+		beta[:4][None, None, :] + alpha[:5][None, :, None])
+	assert_array_almost_equal(y_before[:2, :2], [
+		[[[2.0772, 2.2169, 1.6016],
+		  [1.6461, 1.5935, 1.8252],
+		  [1.6622, 1.6168, 1.8169],
+		  [1.5572, 1.4649, 1.8714]],
+
+		 [[0.7133, 0.8530, 0.2377],
+		  [0.2822, 0.2296, 0.4613],
+		  [0.2983, 0.2529, 0.4530],
+		  [0.1933, 0.1010, 0.5075]]],
+
+
+		[[[1.6821, 1.7923, 1.4796],
+		  [1.7949, 1.7534, 1.8712],
+		  [1.7907, 1.7549, 1.8565],
+		  [1.8182, 1.7454, 1.9520]],
+
+		 [[0.3182, 0.4284, 0.1157],
+		  [0.4310, 0.3895, 0.5073],
+		  [0.4268, 0.3910, 0.4927],
+		  [0.4543, 0.3815, 0.5881]]]], 4)
 
-	assert y_after.shape == (64, 5, 3)
+	assert y_after.shape == (64, 5, 4, 3)
 	assert y_after.dtype == torch.float32
-	assert_array_almost_equal(y_after, y0_after[:, None] * beta[:5][None, :]
-		+ alpha[:5][None, :])
-	assert_array_almost_equal(y_after[:2], [
-		[[2.0082, 2.1007, 1.6017],
-         [0.3082, 0.2734, 0.4613],
-         [0.8994, 0.8693, 1.0315],
-         [2.0796, 2.0185, 2.3482],
-         [1.9976, 2.0469, 1.7810]],
-
-        [[1.7199, 1.6266, 1.5301],
-         [0.4168, 0.4519, 0.4883],
-         [0.9931, 1.0234, 1.0548],
-         [2.2700, 2.3317, 2.3955],
-         [1.8441, 1.7943, 1.7429]]], 4)
+	assert_array_almost_equal(y_after, y0_after[:, None, None] * 
+		beta[:4][None, None, :] + alpha[:5][None, :, None])
+	assert_array_almost_equal(y_after[:2, :2], [
+		[[[2.0008, 2.2360, 1.9981],
+		  [1.6749, 1.5863, 1.6759],
+		  [1.6871, 1.6106, 1.6880],
+		  [1.6076, 1.4523, 1.6095]],
+
+		 [[0.6370, 0.8721, 0.6342],
+		  [0.3110, 0.2224, 0.3120],
+		  [0.3232, 0.2467, 0.3241],
+		  [0.2437, 0.0884, 0.2456]]],
+
+
+		[[[1.5291, 1.6974, 1.6659],
+		  [1.8526, 1.7891, 1.8010],
+		  [1.8405, 1.7857, 1.7960],
+		  [1.9193, 1.8081, 1.8289]],
+
+		 [[0.1652, 0.3335, 0.3020],
+		  [0.4887, 0.4252, 0.4371],
+		  [0.4766, 0.4218, 0.4321],
+		  [0.5554, 0.4442, 0.4650]]]], 4)
 
 
-def test_space_cross_convdense_alpha(X, alpha):
+def test_apply_product_marginalize_convdense_alpha(X, alpha):
 	torch.manual_seed(0)
 	model = ConvDense()
-	y_before, y_after = space_cross(model, X, ["ACGTGC", "TGGTT"], 3, 
-		start=0, args=(alpha[:5, :, None],), batch_size=2, device='cpu')
+	y_before, y_after = apply_product(marginalize, model, X, "ACGTGC", 0, 
+		args=(alpha[:5, :, None],), batch_size=2, device='cpu')
 
 	assert len(y_before) == 2
 	assert y_before[0].shape == (64, 5, 12, 98)
 	assert y_before[1].shape == (64, 5, 3)
 
 	assert y_before[0].dtype == torch.float32
 	assert y_before[1].dtype == torch.float32
 
 	assert_array_almost_equal(y_before[0][:2, :2, :3, :4], [
 		[[[ 0.9883,  1.8037,  0.8841,  0.7446],
-          [ 1.8588,  1.9683,  1.5339,  1.4497],
-          [ 2.1421,  2.2650,  2.6226,  2.4379]],
+		  [ 1.8588,  1.9683,  1.5339,  1.4497],
+		  [ 2.1421,  2.2650,  2.6226,  2.4379]],
 
-         [[-0.3756,  0.4398, -0.4798, -0.6192],
-          [ 0.4949,  0.6044,  0.1700,  0.0858],
-          [ 0.7782,  0.9011,  1.2587,  1.0740]]],
+		 [[-0.3756,  0.4398, -0.4798, -0.6192],
+		  [ 0.4949,  0.6044,  0.1700,  0.0858],
+		  [ 0.7782,  0.9011,  1.2587,  1.0740]]],
 
 
-        [[[ 1.0964,  0.8767,  0.8945,  1.2957],
-          [ 1.6873,  1.7551,  1.7884,  1.8996],
-          [ 2.2469,  2.3060,  2.0810,  2.0929]],
+		[[[ 1.0964,  0.8767,  0.8945,  1.2957],
+		  [ 1.6873,  1.7551,  1.7884,  1.8996],
+		  [ 2.2469,  2.3060,  2.0810,  2.0929]],
 
-         [[-0.2675, -0.4872, -0.4694, -0.0682],
-          [ 0.3234,  0.3912,  0.4245,  0.5357],
-          [ 0.8830,  0.9421,  0.7171,  0.7290]]]], 4)
+		 [[-0.2675, -0.4872, -0.4694, -0.0682],
+		  [ 0.3234,  0.3912,  0.4245,  0.5357],
+		  [ 0.8830,  0.9421,  0.7171,  0.7290]]]], 4)
 
 	assert_array_almost_equal(y_before[1][:4], [
 		[[ 0.1928,  0.2788, -0.1000],
-         [ 0.1928,  0.2788, -0.1000],
-         [ 0.1928,  0.2788, -0.1000],
-         [ 0.1928,  0.2788, -0.1000],
-         [ 0.1928,  0.2788, -0.1000]],
-
-        [[-0.0505,  0.0174, -0.1751],
-         [-0.0505,  0.0174, -0.1751],
-         [-0.0505,  0.0174, -0.1751],
-         [-0.0505,  0.0174, -0.1751],
-         [-0.0505,  0.0174, -0.1751]],
-
-        [[-0.1408,  0.0105,  0.0673],
-         [-0.1408,  0.0105,  0.0673],
-         [-0.1408,  0.0105,  0.0673],
-         [-0.1408,  0.0105,  0.0673],
-         [-0.1408,  0.0105,  0.0673]],
-
-        [[-0.2375, -0.0069,  0.0835],
-         [-0.2375, -0.0069,  0.0835],
-         [-0.2375, -0.0069,  0.0835],
-         [-0.2375, -0.0069,  0.0835],
-         [-0.2375, -0.0069,  0.0835]]], 4)
+		 [ 0.1928,  0.2788, -0.1000],
+		 [ 0.1928,  0.2788, -0.1000],
+		 [ 0.1928,  0.2788, -0.1000],
+		 [ 0.1928,  0.2788, -0.1000]],
+
+		[[-0.0505,  0.0174, -0.1751],
+		 [-0.0505,  0.0174, -0.1751],
+		 [-0.0505,  0.0174, -0.1751],
+		 [-0.0505,  0.0174, -0.1751],
+		 [-0.0505,  0.0174, -0.1751]],
+
+		[[-0.1408,  0.0105,  0.0673],
+		 [-0.1408,  0.0105,  0.0673],
+		 [-0.1408,  0.0105,  0.0673],
+		 [-0.1408,  0.0105,  0.0673],
+		 [-0.1408,  0.0105,  0.0673]],
+
+		[[-0.2375, -0.0069,  0.0835],
+		 [-0.2375, -0.0069,  0.0835],
+		 [-0.2375, -0.0069,  0.0835],
+		 [-0.2375, -0.0069,  0.0835],
+		 [-0.2375, -0.0069,  0.0835]]], 4)
 
 	assert len(y_after) == 2
 	assert y_after[0].shape == (64, 5, 12, 98)
 	assert y_after[1].shape == (64, 5, 3)
 
 	assert y_after[0].dtype == torch.float32
 	assert y_after[1].dtype == torch.float32
 
 	assert_array_almost_equal(y_after[0][:2, :2, :3, :4], [
 		[[[ 1.3831,  0.9466,  0.9256,  1.4921],
-          [ 1.5933,  1.3485,  1.9935,  1.9060],
-          [ 2.2460,  2.6037,  1.8025,  2.1864]],
+		  [ 1.5933,  1.3485,  1.9935,  1.9060],
+		  [ 2.2460,  2.6037,  1.8025,  2.1864]],
 
-         [[ 0.0192, -0.4173, -0.4383,  0.1282],
-          [ 0.2294, -0.0154,  0.6296,  0.5421],
-          [ 0.8821,  1.2398,  0.4386,  0.8225]]],
+		 [[ 0.0192, -0.4173, -0.4383,  0.1282],
+		  [ 0.2294, -0.0154,  0.6296,  0.5421],
+		  [ 0.8821,  1.2398,  0.4386,  0.8225]]],
 
 
-        [[[ 1.3831,  0.9466,  0.9256,  1.4921],
-          [ 1.5933,  1.3485,  1.9935,  1.9060],
-          [ 2.2460,  2.6037,  1.8025,  2.1864]],
+		[[[ 1.3831,  0.9466,  0.9256,  1.4921],
+		  [ 1.5933,  1.3485,  1.9935,  1.9060],
+		  [ 2.2460,  2.6037,  1.8025,  2.1864]],
 
-         [[ 0.0192, -0.4173, -0.4383,  0.1282],
-          [ 0.2294, -0.0154,  0.6296,  0.5421],
-          [ 0.8821,  1.2398,  0.4386,  0.8225]]]], 4)
+		 [[ 0.0192, -0.4173, -0.4383,  0.1282],
+		  [ 0.2294, -0.0154,  0.6296,  0.5421],
+		  [ 0.8821,  1.2398,  0.4386,  0.8225]]]], 4)
 
 	assert_array_almost_equal(y_after[1][:4], [
-		[[ 0.3324,  0.1149, -0.0712],
-         [ 0.3324,  0.1149, -0.0712],
-         [ 0.3324,  0.1149, -0.0712],
-         [ 0.3324,  0.1149, -0.0712],
-         [ 0.3324,  0.1149, -0.0712]],
-
-        [[-0.0377, -0.0666, -0.1223],
-         [-0.0377, -0.0666, -0.1223],
-         [-0.0377, -0.0666, -0.1223],
-         [-0.0377, -0.0666, -0.1223],
-         [-0.0377, -0.0666, -0.1223]],
-
-        [[-0.0393, -0.0238,  0.2462],
-         [-0.0393, -0.0238,  0.2462],
-         [-0.0393, -0.0238,  0.2462],
-         [-0.0393, -0.0238,  0.2462],
-         [-0.0393, -0.0238,  0.2462]],
-
-        [[-0.1770, -0.0393,  0.1683],
-         [-0.1770, -0.0393,  0.1683],
-         [-0.1770, -0.0393,  0.1683],
-         [-0.1770, -0.0393,  0.1683],
-         [-0.1770, -0.0393,  0.1683]]], 4)
+		[[ 0.2472,  0.1913, -0.0212],
+		 [ 0.2472,  0.1913, -0.0212],
+		 [ 0.2472,  0.1913, -0.0212],
+		 [ 0.2472,  0.1913, -0.0212],
+		 [ 0.2472,  0.1913, -0.0212]],
+
+		[[-0.1387,  0.0929, -0.1931],
+		 [-0.1387,  0.0929, -0.1931],
+		 [-0.1387,  0.0929, -0.1931],
+		 [-0.1387,  0.0929, -0.1931],
+		 [-0.1387,  0.0929, -0.1931]],
+
+		[[-0.1165,  0.0957,  0.1448],
+		 [-0.1165,  0.0957,  0.1448],
+		 [-0.1165,  0.0957,  0.1448],
+		 [-0.1165,  0.0957,  0.1448],
+		 [-0.1165,  0.0957,  0.1448]],
+
+		[[-0.2053,  0.0571,  0.1370],
+		 [-0.2053,  0.0571,  0.1370],
+		 [-0.2053,  0.0571,  0.1370],
+		 [-0.2053,  0.0571,  0.1370],
+		 [-0.2053,  0.0571,  0.1370]]], 4)
+
+
+###
+
+
+def test_apply_product_space_flattendense_alpha(X, alpha, beta):
+	torch.manual_seed(0)
+	model = FlattenDense()
+	y0_before, y0_after = space(model, X, ['ACGTGC', 'TGTT'], 3, 
+		device='cpu')
+	y_before, y_after = apply_product(space, model, X, ['ACGTGC', 'TGTT'], 3, 
+		args=(alpha[:5],), device='cpu')
+
+	assert y_before.shape == (64, 5, 3)
+	assert y_before.dtype == torch.float32
+	assert_array_almost_equal(y_before, y0_before[:, None] + alpha[:5][None, :])
+	assert_array_almost_equal(y_before[:2], [
+		[[1.9569, 2.0429, 1.6640],
+		 [0.5930, 0.6790, 0.3001],
+		 [1.1715, 1.2575, 0.8787],
+		 [2.4337, 2.5197, 2.1409],
+		 [2.0604, 2.1464, 1.7675]],
+
+		[[1.7136, 1.7814, 1.5889],
+		 [0.3497, 0.4175, 0.2250],
+		 [0.9283, 0.9961, 0.8036],
+		 [2.1904, 2.2583, 2.0658],
+		 [1.8171, 1.8849, 1.6924]]], 4)
+
+
+	assert y_after.shape == (64, 5, 3)
+	assert y_after.dtype == torch.float32
+	assert_array_almost_equal(y_after, y0_after[:, None] + alpha[:5][None, :])
+	assert_array_almost_equal(y_after[:2], [
+		[[1.9143, 1.9713, 1.6641],
+		 [0.5504, 0.6074, 0.3002],
+		 [1.1290, 1.1860, 0.8788],
+		 [2.3912, 2.4481, 2.1409],
+		 [2.0178, 2.0748, 1.7676]],
+
+		[[1.7369, 1.6794, 1.6200],
+		 [0.3730, 0.3156, 0.2561],
+		 [0.9516, 0.8941, 0.8347],
+		 [2.2137, 2.1563, 2.0968],
+		 [1.8404, 1.7830, 1.7235]]], 4)
+
+
+def test_apply_product_space_flattendense_beta(X, alpha, beta):
+	torch.manual_seed(0)
+	model = FlattenDense()
+	alpha = torch.zeros(X.shape[0], 1)
+
+	y0_before, y0_after = space(model, X, ['ACGTGC', 'TGTT'], 3, 
+		device='cpu')
+	y_before, y_after = apply_product(space, model, X, ['ACGTGC', 'TGTT'], 3, 
+		args=(alpha[:1], beta[:5]), device='cpu')
+	y_before, y_after = y_before[:, 0], y_after[:, 0]
+
+	assert y_before.shape == (64, 5, 3)
+	assert y_before.dtype == torch.float32
+	assert_array_almost_equal(y_before, y0_before[:, None] * beta[:5][None, :])
+	assert_array_almost_equal(y_before[:2], [
+		[[ 0.3132,  0.4529, -0.1624],
+		 [-0.1179, -0.1706,  0.0612],
+		 [-0.1018, -0.1473,  0.0528],
+		 [-0.2069, -0.2991,  0.1073],
+		 [ 0.1669,  0.2413, -0.0865]],
+
+		[[-0.0820,  0.0282, -0.2845],
+		 [ 0.0309, -0.0106,  0.1071],
+		 [ 0.0267, -0.0092,  0.0925],
+		 [ 0.0542, -0.0186,  0.1879],
+		 [-0.0437,  0.0150, -0.1516]]], 4)
+
+	assert y_after.shape == (64, 5, 3)
+	assert y_after.dtype == torch.float32
+	assert_array_almost_equal(y_after, y0_after[:, None] * beta[:5][None, :])
+	assert_array_almost_equal(y_after[:2], [
+		[[ 0.2441,  0.3366, -0.1624],
+		 [-0.0919, -0.1268,  0.0612],
+		 [-0.0794, -0.1095,  0.0528],
+		 [-0.1613, -0.2224,  0.1073],
+		 [ 0.1301,  0.1793, -0.0865]],
+
+		[[-0.0441, -0.1374, -0.2340],
+		 [ 0.0166,  0.0518,  0.0881],
+		 [ 0.0143,  0.0447,  0.0761],
+		 [ 0.0291,  0.0908,  0.1546],
+		 [-0.0235, -0.0732, -0.1247]]], 4)
+
+
+def test_apply_product_space_flattendense_alpha_beta(X, alpha, beta):
+	torch.manual_seed(0)
+	model = FlattenDense()
+	y0_before, y0_after = space(model, X, ['ACGTGC', 'TGTT'], 3, 
+		device='cpu')
+	y_before, y_after = apply_product(space, model, X, ['ACGTGC', 'TGTT'], 3, 
+		args=(alpha[:4], beta[:5]), device='cpu')
+
+	assert y_before.shape == (64, 4, 5, 3)
+	assert y_before.dtype == torch.float32
+	assert_array_almost_equal(y_before, y0_before[:, None, None] * 
+		beta[:5][None, None :] + alpha[:4][None, :, None])
+	assert_array_almost_equal(y_before[:2, :2], [
+		[[[2.0772, 2.2169, 1.6016],
+          [1.6461, 1.5935, 1.8252],
+          [1.6622, 1.6168, 1.8169],
+          [1.5572, 1.4649, 1.8714],
+          [1.9309, 2.0053, 1.6775]],
+
+         [[0.7133, 0.8530, 0.2377],
+          [0.2822, 0.2296, 0.4613],
+          [0.2983, 0.2529, 0.4530],
+          [0.1933, 0.1010, 0.5075],
+          [0.5670, 0.6414, 0.3136]]],
+
+
+        [[[1.6821, 1.7923, 1.4796],
+          [1.7949, 1.7534, 1.8712],
+          [1.7907, 1.7549, 1.8565],
+          [1.8182, 1.7454, 1.9520],
+          [1.7204, 1.7791, 1.6125]],
+
+         [[0.3182, 0.4284, 0.1157],
+          [0.4310, 0.3895, 0.5073],
+          [0.4268, 0.3910, 0.4927],
+          [0.4543, 0.3815, 0.5881],
+          [0.3565, 0.4152, 0.2486]]]], 4)
+
+	assert y_after.shape == (64, 4, 5, 3)
+	assert y_after.dtype == torch.float32
+	assert_array_almost_equal(y_after, y0_after[:, None, None] * 
+		beta[:5][None, None, :] + alpha[:4][None, :, None])
+	assert_array_almost_equal(y_after[:2, :2], [
+		[[[2.0082, 2.1007, 1.6017],
+          [1.6721, 1.6373, 1.8252],
+          [1.6847, 1.6546, 1.8169],
+          [1.6028, 1.5417, 1.8713],
+          [1.8941, 1.9434, 1.6775]],
+
+         [[0.6443, 0.7368, 0.2378],
+          [0.3082, 0.2734, 0.4613],
+          [0.3208, 0.2907, 0.4530],
+          [0.2389, 0.1778, 0.5074],
+          [0.5302, 0.5795, 0.3136]]],
+
+
+        [[[1.7199, 1.6266, 1.5301],
+          [1.7807, 1.8158, 1.8522],
+          [1.7784, 1.8087, 1.8401],
+          [1.7932, 1.8548, 1.9186],
+          [1.7405, 1.6908, 1.6394]],
+
+         [[0.3560, 0.2627, 0.1662],
+          [0.4168, 0.4519, 0.4883],
+          [0.4145, 0.4448, 0.4762],
+          [0.4293, 0.4909, 0.5547],
+          [0.3767, 0.3269, 0.2755]]]], 4)
+
+
+def test_apply_product_space_convdense_alpha(X, alpha):
+  torch.manual_seed(0)
+  model = ConvDense()
+  y_before, y_after = apply_product(space, model, X, ["ACGTGC", "TGGTT"], 3, 
+	0, args=(alpha[:5, :, None],), batch_size=2, device='cpu')
+
+  assert len(y_before) == 2
+  assert y_before[0].shape == (64, 5, 12, 98)
+  assert y_before[1].shape == (64, 5, 3)
+
+  assert y_before[0].dtype == torch.float32
+  assert y_before[1].dtype == torch.float32
+
+  assert_array_almost_equal(y_before[0][:2, :2, :3, :4], [
+	[[[ 0.9883,  1.8037,  0.8841,  0.7446],
+	  [ 1.8588,  1.9683,  1.5339,  1.4497],
+	  [ 2.1421,  2.2650,  2.6226,  2.4379]],
+
+	 [[-0.3756,  0.4398, -0.4798, -0.6192],
+	  [ 0.4949,  0.6044,  0.1700,  0.0858],
+	  [ 0.7782,  0.9011,  1.2587,  1.0740]]],
+
+
+	[[[ 1.0964,  0.8767,  0.8945,  1.2957],
+	  [ 1.6873,  1.7551,  1.7884,  1.8996],
+	  [ 2.2469,  2.3060,  2.0810,  2.0929]],
+
+	 [[-0.2675, -0.4872, -0.4694, -0.0682],
+	  [ 0.3234,  0.3912,  0.4245,  0.5357],
+	  [ 0.8830,  0.9421,  0.7171,  0.7290]]]], 4)
+
+  assert_array_almost_equal(y_before[1][:4], [
+	[[ 0.1928,  0.2788, -0.1000],
+	 [ 0.1928,  0.2788, -0.1000],
+	 [ 0.1928,  0.2788, -0.1000],
+	 [ 0.1928,  0.2788, -0.1000],
+	 [ 0.1928,  0.2788, -0.1000]],
+
+	[[-0.0505,  0.0174, -0.1751],
+	 [-0.0505,  0.0174, -0.1751],
+	 [-0.0505,  0.0174, -0.1751],
+	 [-0.0505,  0.0174, -0.1751],
+	 [-0.0505,  0.0174, -0.1751]],
+
+	[[-0.1408,  0.0105,  0.0673],
+	 [-0.1408,  0.0105,  0.0673],
+	 [-0.1408,  0.0105,  0.0673],
+	 [-0.1408,  0.0105,  0.0673],
+	 [-0.1408,  0.0105,  0.0673]],
+
+	[[-0.2375, -0.0069,  0.0835],
+	 [-0.2375, -0.0069,  0.0835],
+	 [-0.2375, -0.0069,  0.0835],
+	 [-0.2375, -0.0069,  0.0835],
+	 [-0.2375, -0.0069,  0.0835]]], 4)
+
+  assert len(y_after) == 2
+  assert y_after[0].shape == (64, 5, 12, 98)
+  assert y_after[1].shape == (64, 5, 3)
+
+  assert y_after[0].dtype == torch.float32
+  assert y_after[1].dtype == torch.float32
+
+  assert_array_almost_equal(y_after[0][:2, :2, :3, :4], [
+	[[[ 1.3831,  0.9466,  0.9256,  1.4921],
+	  [ 1.5933,  1.3485,  1.9935,  1.9060],
+	  [ 2.2460,  2.6037,  1.8025,  2.1864]],
+
+	 [[ 0.0192, -0.4173, -0.4383,  0.1282],
+	  [ 0.2294, -0.0154,  0.6296,  0.5421],
+	  [ 0.8821,  1.2398,  0.4386,  0.8225]]],
+
+
+	[[[ 1.3831,  0.9466,  0.9256,  1.4921],
+	  [ 1.5933,  1.3485,  1.9935,  1.9060],
+	  [ 2.2460,  2.6037,  1.8025,  2.1864]],
+
+	 [[ 0.0192, -0.4173, -0.4383,  0.1282],
+	  [ 0.2294, -0.0154,  0.6296,  0.5421],
+	  [ 0.8821,  1.2398,  0.4386,  0.8225]]]], 4)
+
+  assert_array_almost_equal(y_after[1][:4], [
+	[[ 0.3324,  0.1149, -0.0712],
+	 [ 0.3324,  0.1149, -0.0712],
+	 [ 0.3324,  0.1149, -0.0712],
+	 [ 0.3324,  0.1149, -0.0712],
+	 [ 0.3324,  0.1149, -0.0712]],
+
+	[[-0.0377, -0.0666, -0.1223],
+	 [-0.0377, -0.0666, -0.1223],
+	 [-0.0377, -0.0666, -0.1223],
+	 [-0.0377, -0.0666, -0.1223],
+	 [-0.0377, -0.0666, -0.1223]],
+
+	[[-0.0393, -0.0238,  0.2462],
+	 [-0.0393, -0.0238,  0.2462],
+	 [-0.0393, -0.0238,  0.2462],
+	 [-0.0393, -0.0238,  0.2462],
+	 [-0.0393, -0.0238,  0.2462]],
+
+	[[-0.1770, -0.0393,  0.1683],
+	 [-0.1770, -0.0393,  0.1683],
+	 [-0.1770, -0.0393,  0.1683],
+	 [-0.1770, -0.0393,  0.1683],
+	 [-0.1770, -0.0393,  0.1683]]], 4)
```

### Comparing `tangermeme-0.1.0rc0/tests/test_utils.py` & `tangermeme-0.2.0/tests/test_utils.py`

 * *Files identical despite different names*

