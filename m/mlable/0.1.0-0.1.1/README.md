# Comparing `tmp/mlable-0.1.0.tar.gz` & `tmp/mlable-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlable-0.1.0.tar", max compression
+gzip compressed data, was "mlable-0.1.1.tar", max compression
```

## Comparing `mlable-0.1.0.tar` & `mlable-0.1.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      360 2023-12-27 16:49:58.465979 mlable-0.1.0/.github/README.md
--rw-r--r--   0        0        0        0 2024-01-25 21:43:22.740044 mlable-0.1.0/mlable/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 20:33:11.034995 mlable-0.1.0/mlable/keras/__init__.py
--rw-r--r--   0        0        0     5219 2024-03-17 15:32:31.801607 mlable-0.1.0/mlable/keras/models.py
--rw-r--r--   0        0        0        0 2024-01-26 10:57:37.881478 mlable-0.1.0/mlable/models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 15:44:53.795021 mlable-0.1.0/mlable/models/colonel/__init__.py
--rw-r--r--   0        0        0    17241 2024-03-12 20:42:42.653388 mlable-0.1.0/mlable/models/gpm/README.md
--rw-r--r--   0        0        0        0 2024-02-04 22:08:59.205764 mlable-0.1.0/mlable/models/gpm/__init__.py
--rw-r--r--   0        0        0     9345 2024-03-12 21:16:09.662821 mlable-0.1.0/mlable/models/gpm/main.py
--rw-r--r--   0        0        0        0 2024-01-25 11:56:28.560613 mlable-0.1.0/mlable/models/gpt/__init__.py
--rw-r--r--   0        0        0     4609 2024-03-15 20:59:30.682559 mlable-0.1.0/mlable/models/gpt/rnn.torch.py
--rw-r--r--   0        0        0    33483 2024-02-05 23:20:39.711787 mlable-0.1.0/mlable/models/gpt/sat.keras.ipynb
--rw-r--r--   0        0        0     5407 2024-03-17 15:46:00.373875 mlable-0.1.0/mlable/models/gpt/sat.keras.py
--rw-r--r--   0        0        0     4642 2024-03-12 21:21:28.151800 mlable-0.1.0/mlable/models/gpt/sat.tensorflow.py
--rw-r--r--   0        0        0     4859 2024-03-16 16:19:19.458786 mlable-0.1.0/mlable/models/gpt/sat.torch.py
--rw-r--r--   0        0        0     8689 2024-01-07 22:39:32.640751 mlable-0.1.0/mlable/models/makemore/.old/mlp.batch.tensorflow.py
--rw-r--r--   0        0        0    11306 2024-01-07 22:39:21.714118 mlable-0.1.0/mlable/models/makemore/.old/mlp.regularization.tensorflow.py
--rw-r--r--   0        0        0    10543 2024-01-07 22:38:57.034242 mlable-0.1.0/mlable/models/makemore/.old/mlp.viz.tensorflow.py
--rw-r--r--   0        0        0        0 2024-01-25 21:44:14.973726 mlable-0.1.0/mlable/models/makemore/__init__.py
--rw-r--r--   0        0        0     7600 2024-01-14 14:50:05.071077 mlable-0.1.0/mlable/models/makemore/cnn.keras.py
--rw-r--r--   0        0        0    15313 2024-02-17 10:48:33.230500 mlable-0.1.0/mlable/models/makemore/cnn.tensorflow.py
--rw-r--r--   0        0        0    10039 2024-03-14 22:06:01.118763 mlable-0.1.0/mlable/models/makemore/cnn.torch.py
--rw-r--r--   0        0        0     6271 2024-01-22 21:19:30.047231 mlable-0.1.0/mlable/models/makemore/mlp.keras.py
--rw-r--r--   0        0        0    14087 2024-02-16 15:05:52.419701 mlable-0.1.0/mlable/models/makemore/mlp.tensorflow.py
--rw-r--r--   0        0        0        0 2024-04-09 09:50:53.069681 mlable-0.1.0/mlable/models/sold/__init__.py
--rw-r--r--   0        0        0     7419 2024-04-09 09:52:25.100652 mlable-0.1.0/mlable/models/sold/bytecode.py
--rw-r--r--   0        0        0     6669 2024-04-09 09:50:53.069681 mlable-0.1.0/mlable/models/sold/main.keras.py
--rw-r--r--   0        0        0     2387 2024-04-09 09:56:41.383364 mlable-0.1.0/mlable/models/sold/solidity.py
--rw-r--r--   0        0        0        0 2024-03-18 18:34:21.653083 mlable-0.1.0/mlable/models/tokun/__init__.py
--rw-r--r--   0        0        0     4321 2024-04-29 07:09:43.479546 mlable-0.1.0/mlable/models/tokun/layers.py
--rw-r--r--   0        0        0     4020 2024-05-02 07:00:17.075570 mlable-0.1.0/mlable/models/tokun/pipeline.py
--rw-r--r--   0        0        0 12878918 2024-05-02 11:01:32.760077 mlable-0.1.0/mlable/models/tokun/tokun.1.keras.ipynb
--rw-r--r--   0        0        0     9022 2024-05-04 08:39:42.186247 mlable-0.1.0/mlable/models/tokun/tokun.1.keras.py
--rw-r--r--   0        0        0 10227709 2024-05-02 11:01:26.420055 mlable-0.1.0/mlable/models/tokun/tokun.4.keras.ipynb
--rw-r--r--   0        0        0    10621 2024-05-02 09:26:01.860244 mlable-0.1.0/mlable/models/tokun/tokun.4.keras.py
--rw-r--r--   0        0        0   832982 2024-05-02 11:00:57.733286 mlable-0.1.0/mlable/models/tokun/tokun.4x4.keras.ipynb
--rw-r--r--   0        0        0    11288 2024-05-02 09:26:23.383872 mlable-0.1.0/mlable/models/tokun/tokun.4x4.keras.py
--rw-r--r--   0        0        0        0 2024-01-26 10:57:25.344821 mlable-0.1.0/mlable/tensorflow/__init__.py
--rw-r--r--   0        0        0      309 2024-02-16 18:02:23.195647 mlable-0.1.0/mlable/tensorflow/data.py
--rw-r--r--   0        0        0      532 2024-01-26 13:14:45.749598 mlable-0.1.0/mlable/tensorflow/initializers.py
--rw-r--r--   0        0        0      559 2024-04-29 12:29:16.563921 mlable-0.1.0/mlable/tensorflow/io.py
--rw-r--r--   0        0        0    12543 2024-04-26 18:19:13.446040 mlable-0.1.0/mlable/tensorflow/layers.py
--rw-r--r--   0        0        0        0 2024-01-26 12:54:06.355191 mlable-0.1.0/mlable/tensorflow/losses.py
--rw-r--r--   0        0        0     4622 2024-01-31 18:01:34.815819 mlable-0.1.0/mlable/tensorflow/models.py
--rw-r--r--   0        0        0     2843 2024-03-17 13:27:55.811876 mlable-0.1.0/mlable/tensorflow/optimizers.py
--rw-r--r--   0        0        0      608 2024-03-17 15:55:26.628912 mlable-0.1.0/mlable/tensorflow/sampling.py
--rw-r--r--   0        0        0     1073 2024-01-28 22:11:41.354437 mlable-0.1.0/mlable/tensorflow/summary.py
--rw-r--r--   0        0        0        0 2024-01-14 17:50:09.526979 mlable-0.1.0/mlable/tokens/__init__.py
--rw-r--r--   0        0        0     2387 2024-02-26 22:53:48.809185 mlable-0.1.0/mlable/tokens/bpe.py
--rw-r--r--   0        0        0     1743 2024-02-24 20:47:30.328705 mlable-0.1.0/mlable/tokens/ngrams.py
--rw-r--r--   0        0        0        0 2024-02-25 16:24:42.204319 mlable-0.1.0/mlable/torch/__init__.py
--rw-r--r--   0        0        0      252 2024-03-14 21:37:39.458099 mlable-0.1.0/mlable/torch/data.py
--rw-r--r--   0        0        0     9425 2024-03-16 16:18:40.985183 mlable-0.1.0/mlable/torch/layers.py
--rw-r--r--   0        0        0     2565 2024-03-16 16:03:36.844134 mlable-0.1.0/mlable/torch/optimizers.py
--rw-r--r--   0        0        0      612 2024-03-14 12:49:57.500345 mlable-0.1.0/mlable/torch/sampling.py
--rw-r--r--   0        0        0      453 2024-05-06 13:03:44.545940 mlable-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 mlable-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      360 2023-12-27 16:49:58.465979 mlable-0.1.1/.github/README.md
+-rw-r--r--   0        0        0        0 2024-01-25 21:43:22.740044 mlable-0.1.1/mlable/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 20:33:11.034995 mlable-0.1.1/mlable/keras/__init__.py
+-rw-r--r--   0        0        0     5219 2024-03-17 15:32:31.801607 mlable-0.1.1/mlable/keras/models.py
+-rw-r--r--   0        0        0        0 2024-01-26 10:57:37.881478 mlable-0.1.1/mlable/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 15:44:53.795021 mlable-0.1.1/mlable/models/colonel/__init__.py
+-rw-r--r--   0        0        0    17241 2024-03-12 20:42:42.653388 mlable-0.1.1/mlable/models/gpm/README.md
+-rw-r--r--   0        0        0        0 2024-02-04 22:08:59.205764 mlable-0.1.1/mlable/models/gpm/__init__.py
+-rw-r--r--   0        0        0     9345 2024-03-12 21:16:09.662821 mlable-0.1.1/mlable/models/gpm/main.py
+-rw-r--r--   0        0        0        0 2024-01-25 11:56:28.560613 mlable-0.1.1/mlable/models/gpt/__init__.py
+-rw-r--r--   0        0        0     4609 2024-03-15 20:59:30.682559 mlable-0.1.1/mlable/models/gpt/rnn.torch.py
+-rw-r--r--   0        0        0    33483 2024-02-05 23:20:39.711787 mlable-0.1.1/mlable/models/gpt/sat.keras.ipynb
+-rw-r--r--   0        0        0     5407 2024-03-17 15:46:00.373875 mlable-0.1.1/mlable/models/gpt/sat.keras.py
+-rw-r--r--   0        0        0     4642 2024-03-12 21:21:28.151800 mlable-0.1.1/mlable/models/gpt/sat.tensorflow.py
+-rw-r--r--   0        0        0     4859 2024-03-16 16:19:19.458786 mlable-0.1.1/mlable/models/gpt/sat.torch.py
+-rw-r--r--   0        0        0     8689 2024-01-07 22:39:32.640751 mlable-0.1.1/mlable/models/makemore/.old/mlp.batch.tensorflow.py
+-rw-r--r--   0        0        0    11306 2024-01-07 22:39:21.714118 mlable-0.1.1/mlable/models/makemore/.old/mlp.regularization.tensorflow.py
+-rw-r--r--   0        0        0    10543 2024-01-07 22:38:57.034242 mlable-0.1.1/mlable/models/makemore/.old/mlp.viz.tensorflow.py
+-rw-r--r--   0        0        0        0 2024-01-25 21:44:14.973726 mlable-0.1.1/mlable/models/makemore/__init__.py
+-rw-r--r--   0        0        0     7600 2024-01-14 14:50:05.071077 mlable-0.1.1/mlable/models/makemore/cnn.keras.py
+-rw-r--r--   0        0        0    15313 2024-02-17 10:48:33.230500 mlable-0.1.1/mlable/models/makemore/cnn.tensorflow.py
+-rw-r--r--   0        0        0    10039 2024-03-14 22:06:01.118763 mlable-0.1.1/mlable/models/makemore/cnn.torch.py
+-rw-r--r--   0        0        0     6271 2024-01-22 21:19:30.047231 mlable-0.1.1/mlable/models/makemore/mlp.keras.py
+-rw-r--r--   0        0        0    14087 2024-02-16 15:05:52.419701 mlable-0.1.1/mlable/models/makemore/mlp.tensorflow.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:50:53.069681 mlable-0.1.1/mlable/models/sold/__init__.py
+-rw-r--r--   0        0        0     7419 2024-04-09 09:52:25.100652 mlable-0.1.1/mlable/models/sold/bytecode.py
+-rw-r--r--   0        0        0     6669 2024-04-09 09:50:53.069681 mlable-0.1.1/mlable/models/sold/main.keras.py
+-rw-r--r--   0        0        0     2387 2024-04-09 09:56:41.383364 mlable-0.1.1/mlable/models/sold/solidity.py
+-rw-r--r--   0        0        0        0 2024-03-18 18:34:21.653083 mlable-0.1.1/mlable/models/tokun/__init__.py
+-rw-r--r--   0        0        0     4321 2024-04-29 07:09:43.479546 mlable-0.1.1/mlable/models/tokun/layers.py
+-rw-r--r--   0        0        0     4020 2024-05-02 07:00:17.075570 mlable-0.1.1/mlable/models/tokun/pipeline.py
+-rw-r--r--   0        0        0 12878918 2024-05-02 11:01:32.760077 mlable-0.1.1/mlable/models/tokun/tokun.1.keras.ipynb
+-rw-r--r--   0        0        0     9022 2024-05-04 08:39:42.186247 mlable-0.1.1/mlable/models/tokun/tokun.1.keras.py
+-rw-r--r--   0        0        0 10227709 2024-05-02 11:01:26.420055 mlable-0.1.1/mlable/models/tokun/tokun.4.keras.ipynb
+-rw-r--r--   0        0        0    10621 2024-05-02 09:26:01.860244 mlable-0.1.1/mlable/models/tokun/tokun.4.keras.py
+-rw-r--r--   0        0        0   832982 2024-05-02 11:00:57.733286 mlable-0.1.1/mlable/models/tokun/tokun.4x4.keras.ipynb
+-rw-r--r--   0        0        0    11288 2024-05-02 09:26:23.383872 mlable-0.1.1/mlable/models/tokun/tokun.4x4.keras.py
+-rw-r--r--   0        0        0        0 2024-01-26 10:57:25.344821 mlable-0.1.1/mlable/tensorflow/__init__.py
+-rw-r--r--   0        0        0      309 2024-02-16 18:02:23.195647 mlable-0.1.1/mlable/tensorflow/data.py
+-rw-r--r--   0        0        0      532 2024-01-26 13:14:45.749598 mlable-0.1.1/mlable/tensorflow/initializers.py
+-rw-r--r--   0        0        0      559 2024-04-29 12:29:16.563921 mlable-0.1.1/mlable/tensorflow/io.py
+-rw-r--r--   0        0        0    17551 2024-05-07 16:55:57.231436 mlable-0.1.1/mlable/tensorflow/layers.py
+-rw-r--r--   0        0        0        0 2024-01-26 12:54:06.355191 mlable-0.1.1/mlable/tensorflow/losses.py
+-rw-r--r--   0        0        0     4622 2024-01-31 18:01:34.815819 mlable-0.1.1/mlable/tensorflow/models.py
+-rw-r--r--   0        0        0     2843 2024-03-17 13:27:55.811876 mlable-0.1.1/mlable/tensorflow/optimizers.py
+-rw-r--r--   0        0        0      608 2024-03-17 15:55:26.628912 mlable-0.1.1/mlable/tensorflow/sampling.py
+-rw-r--r--   0        0        0     1073 2024-01-28 22:11:41.354437 mlable-0.1.1/mlable/tensorflow/summary.py
+-rw-r--r--   0        0        0        0 2024-01-14 17:50:09.526979 mlable-0.1.1/mlable/tokens/__init__.py
+-rw-r--r--   0        0        0     2387 2024-02-26 22:53:48.809185 mlable-0.1.1/mlable/tokens/bpe.py
+-rw-r--r--   0        0        0     1743 2024-02-24 20:47:30.328705 mlable-0.1.1/mlable/tokens/ngrams.py
+-rw-r--r--   0        0        0        0 2024-02-25 16:24:42.204319 mlable-0.1.1/mlable/torch/__init__.py
+-rw-r--r--   0        0        0      252 2024-03-14 21:37:39.458099 mlable-0.1.1/mlable/torch/data.py
+-rw-r--r--   0        0        0     9425 2024-03-16 16:18:40.985183 mlable-0.1.1/mlable/torch/layers.py
+-rw-r--r--   0        0        0     2565 2024-03-16 16:03:36.844134 mlable-0.1.1/mlable/torch/optimizers.py
+-rw-r--r--   0        0        0      612 2024-03-14 12:49:57.500345 mlable-0.1.1/mlable/torch/sampling.py
+-rw-r--r--   0        0        0      453 2024-05-07 16:56:51.438470 mlable-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 mlable-0.1.1/PKG-INFO
```

### Comparing `mlable-0.1.0/mlable/keras/models.py` & `mlable-0.1.1/mlable/keras/models.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/models/gpm/README.md` & `mlable-0.1.1/mlable/models/gpm/README.md`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/models/gpm/main.py` & `mlable-0.1.1/mlable/models/gpm/main.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/models/gpt/rnn.torch.py` & `mlable-0.1.1/mlable/models/gpt/rnn.torch.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/models/gpt/sat.keras.ipynb` & `mlable-0.1.1/mlable/models/gpt/sat.keras.ipynb`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/models/gpt/sat.keras.py` & `mlable-0.1.1/mlable/models/gpt/sat.keras.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/models/gpt/sat.tensorflow.py` & `mlable-0.1.1/mlable/models/gpt/sat.tensorflow.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/models/gpt/sat.torch.py` & `mlable-0.1.1/mlable/models/gpt/sat.torch.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/models/makemore/.old/mlp.batch.tensorflow.py` & `mlable-0.1.1/mlable/models/makemore/.old/mlp.batch.tensorflow.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/models/makemore/.old/mlp.regularization.tensorflow.py` & `mlable-0.1.1/mlable/models/makemore/.old/mlp.regularization.tensorflow.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/models/makemore/.old/mlp.viz.tensorflow.py` & `mlable-0.1.1/mlable/models/makemore/.old/mlp.viz.tensorflow.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/models/makemore/cnn.keras.py` & `mlable-0.1.1/mlable/models/makemore/cnn.keras.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/models/makemore/cnn.tensorflow.py` & `mlable-0.1.1/mlable/models/makemore/cnn.tensorflow.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/models/makemore/cnn.torch.py` & `mlable-0.1.1/mlable/models/makemore/cnn.torch.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/models/makemore/mlp.keras.py` & `mlable-0.1.1/mlable/models/makemore/mlp.keras.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/models/makemore/mlp.tensorflow.py` & `mlable-0.1.1/mlable/models/makemore/mlp.tensorflow.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/models/sold/bytecode.py` & `mlable-0.1.1/mlable/models/sold/bytecode.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/models/sold/main.keras.py` & `mlable-0.1.1/mlable/models/sold/main.keras.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/models/sold/solidity.py` & `mlable-0.1.1/mlable/models/sold/solidity.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/models/tokun/layers.py` & `mlable-0.1.1/mlable/models/tokun/layers.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/models/tokun/pipeline.py` & `mlable-0.1.1/mlable/models/tokun/pipeline.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/models/tokun/tokun.1.keras.ipynb` & `mlable-0.1.1/mlable/models/tokun/tokun.1.keras.ipynb`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/models/tokun/tokun.1.keras.py` & `mlable-0.1.1/mlable/models/tokun/tokun.1.keras.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/models/tokun/tokun.4.keras.ipynb` & `mlable-0.1.1/mlable/models/tokun/tokun.4.keras.ipynb`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/models/tokun/tokun.4.keras.py` & `mlable-0.1.1/mlable/models/tokun/tokun.4.keras.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/models/tokun/tokun.4x4.keras.ipynb` & `mlable-0.1.1/mlable/models/tokun/tokun.4x4.keras.ipynb`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/models/tokun/tokun.4x4.keras.py` & `mlable-0.1.1/mlable/models/tokun/tokun.4x4.keras.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/tensorflow/initializers.py` & `mlable-0.1.1/mlable/tensorflow/initializers.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/tensorflow/io.py` & `mlable-0.1.1/mlable/tensorflow/io.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/tensorflow/layers.py` & `mlable-0.1.1/mlable/tensorflow/layers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import keras
 import numpy as np
 import tensorflow as tf
 
 import mlable.tensorflow.initializers as _mti
 
 # NORMALIZATION ###############################################################
 
+@keras.saving.register_keras_serializable(package='layers')
 class BatchNormalization(tf.keras.layers.Layer):
     def __init__(
         self,
         axis: int=0,
         momentum: float=0.99,
         epsilon: float=0.001,
         **kwargs
@@ -23,18 +25,18 @@
         self._bias = None
 
     def build(self, input_shape: tuple):
         # shape
         __axis = self._axis % len(input_shape) # positive index even when the axis is specified negatively, like -2
         __shape = [1 if __i == __axis else __d for __i, __d in enumerate(input_shape)]
         # values
-        __mean_init = _mti.SmallNormal()
-        __stddev_init = _mti.SmallNormal()
-        __gain_init = _mti.SmallNormal()
-        __bias_init = _mti.SmallNormal()
+        __mean_init = tf.keras.initializers.GlorotNormal()
+        __stddev_init = tf.keras.initializers.GlorotNormal()
+        __gain_init = tf.keras.initializers.GlorotNormal()
+        __bias_init = tf.keras.initializers.Zeros()
         # tensors
         self._mean = self.add_weight("mean", shape=__shape, initializer=__mean_init)
         self._stddev = self.add_weight("stddev", shape=__shape, initializer=__stddev_init)
         self._gain = self.add_weight("gain", shape=__shape, initializer=__gain_init)
         self._bias = self.add_weight("bias", shape=__shape, initializer=__bias_init)
         # notify the model
         self.built = True
@@ -48,14 +50,27 @@
             self._mean = tf.stop_gradient(self._momentum * self._mean + (1. - self._momentum) * __batch_mean)
             self._stddev = tf.stop_gradient(self._momentum * self._stddev + (1. - self._momentum) * __batch_stddev)
         # normalize
         __normalized = tf.math.divide(inputs - self._mean, self._stddev + self._epsilon)
         # scale
         return tf.math.multiply(self._gain, __normalized) + self._bias
 
+    def get_config(self) -> dict:
+        __parent_config = super(BatchNormalization, self).get_config()
+        __child_config = {
+            'axis': self._axis,
+            'momentum': self._momentum,
+            'epsilon': self._epsilon}
+        return {**__parent_config, **__child_config}
+
+    @classmethod
+    def from_config(cls, config) -> tf.keras.layers.Layer:
+        return cls(**config)
+
+@keras.saving.register_keras_serializable(package='layers')
 class LayerNormalization(tf.keras.layers.Layer):
     def __init__(
         self,
         axis: int=-1,
         epsilon: float=0.001,
         **kwargs
     ):
@@ -65,16 +80,16 @@
         self._gain = None
         self._bias = None
 
     def build(self, input_shape: tuple):
         # shape
         __shape = [1] + input_shape[1:]
         # values
-        __gain_init = _mti.SmallNormal()
-        __bias_init = _mti.SmallNormal()
+        __gain_init = tf.keras.initializers.GlorotNormal()
+        __bias_init = tf.keras.initializers.Zeros()
         # tensors
         self._gain = self.add_weight("gain", shape=__shape, initializer=__gain_init)
         self._bias = self.add_weight("bias", shape=__shape, initializer=__bias_init)
         # notify the model
         self.built = True
 
     def call(self, inputs: tf.Tensor, training: bool=True, **kwargs):
@@ -82,20 +97,32 @@
         __layer_mean = tf.math.reduce_mean(inputs, axis=self._axis, keepdims=True)
         __layer_stddev = tf.math.reduce_std(inputs, axis=self._axis, keepdims=True)
         # normalize
         __normalized = tf.math.divide(inputs - __layer_mean, __layer_stddev + self._epsilon)
         # scale
         return tf.math.add(tf.math.multiply(self._gain, __normalized), self._bias)
 
+    def get_config(self) -> dict:
+        __parent_config = super(LayerNormalization, self).get_config()
+        __child_config = {
+            'axis': self._axis,
+            'epsilon': self._epsilon}
+        return {**__parent_config, **__child_config}
+
+    @classmethod
+    def from_config(cls, config) -> tf.keras.layers.Layer:
+        return cls(**config)
+
 # REGULARIZATION ##############################################################
 
 # dropout
 
 # LINEAR ######################################################################
 
+@keras.saving.register_keras_serializable(package='layers')
 class Dense(tf.keras.layers.Layer):
     def __init__(
         self,
         units: int,
         use_bias: bool=True,
         **kwargs
     ):
@@ -103,28 +130,40 @@
         self._units = units
         self._biased = use_bias
         self._kernel = None
         self._bias = None
 
     def build(self, input_shape: tuple):
         # kernel
-        __kernel_init = _mti.SmallNormal()
+        __kernel_init = tf.keras.initializers.GlorotNormal()
         self._kernel = self.add_weight("kernel", shape=[int(input_shape[-1]), self._units], initializer=__kernel_init)
         # bias
         if self._biased:
-            __bias_init = _mti.SmallNormal()
+            __bias_init = tf.keras.initializers.Zeros()
             self._bias = self.add_weight("bias", shape=[self._units], initializer=__bias_init)
         # notify the model
         self.built = True
 
     def call(self, inputs: tf.Tensor, **kwargs):
         return tf.matmul(inputs, self._kernel) + self._bias if (self._biased and self._bias is not None) else tf.matmul(inputs, self._kernel)
 
+    def get_config(self) -> dict:
+        __parent_config = super(Dense, self).get_config()
+        __child_config = {
+            'units': self._units,
+            'use_bias': self._biased}
+        return {**__parent_config, **__child_config}
+
+    @classmethod
+    def from_config(cls, config) -> tf.keras.layers.Layer:
+        return cls(**config)
+
 # QUADRATIC ###################################################################
 
+@keras.saving.register_keras_serializable(package='layers')
 class Attention(tf.keras.layers.Layer):
     def __init__(
         self,
         head_dim: int,
         head_count: int=1,
         **kwargs
     ):
@@ -135,17 +174,17 @@
         self._key = None
         self._query = None
         self._value = None
 
     def build(self, input_shape: tuple) -> None:
         self._time_dim = list(input_shape)[-2]
         # init
-        __key_init = _mti.SmallNormal()
-        __query_init = _mti.SmallNormal()
-        __value_init = _mti.SmallNormal()
+        __key_init = tf.keras.initializers.GlorotNormal()
+        __query_init = tf.keras.initializers.GlorotNormal()
+        __value_init = tf.keras.initializers.GlorotNormal()
         # kernels
         self._key = self.add_weight("key", shape=[int(input_shape[-1]), self._head_dim], initializer=__key_init)
         self._query = self.add_weight("query", shape=[int(input_shape[-1]), self._head_dim], initializer=__query_init)
         self._value = self.add_weight("value", shape=[self._time_dim, self._head_dim], initializer=__value_init)
         # notify the model
         self.built = True
 
@@ -165,41 +204,64 @@
         __u = tf.where(__m == 1., -np.inf, 0.) # (T, T)
         __l = tf.linalg.band_part(__w, num_lower=-1, num_upper=0) # (B, T, T) may fail because of the first dimension => diag of tensor with 3 axes
         # probabilities
         __w = tf.nn.softmax(__u + __l, axis=-1) # (T, T) + (B, T, T) = (B, T, T)
         # value
         return tf.matmul(__w, self._value) # (B, T, T) * (T, H) = (B, T, H)
 
+    def get_config(self) -> dict:
+        __parent_config = super(Attention, self).get_config()
+        __child_config = {
+            'head_dim': self._head_dim,
+            'head_count': self._head_count}
+        return {**__parent_config, **__child_config}
+
+    @classmethod
+    def from_config(cls, config) -> tf.keras.layers.Layer:
+        return cls(**config)
+
 # EMBEDDING ###################################################################
 
+@keras.saving.register_keras_serializable(package='layers')
 class Embedding(tf.keras.layers.Layer):
     def __init__(
         self,
         input_dim: int,
         output_dim: int,
         **kwargs
     ):
         super(Embedding, self).__init__(**kwargs)
         self._input_dim = input_dim
         self._output_dim = output_dim
         self._kernel = None
-        self._position_kernel = None
 
     def build(self, input_shape: tuple):
-        __kernel_init = _mti.SmallNormal()
+        __kernel_init = tf.keras.initializers.GlorotNormal()
         # register the weights
         self._kernel = self.add_weight(name="kernel", shape=[self._input_dim, self._output_dim], initializer=__kernel_init)
         # notify the model
         self.built = True
 
     def call(self, inputs: tf.Tensor, **kwargs):
         # content embedding
         __x = tf.one_hot(indices=inputs, depth=self._input_dim, dtype=tf.dtypes.float32)
         return tf.matmul(__x, self._kernel)
 
+    def get_config(self) -> dict:
+        __parent_config = super(Embedding, self).get_config()
+        __child_config = {
+            'input_dim': self._input_dim,
+            'output_dim': self._output_dim}
+        return {**__parent_config, **__child_config}
+
+    @classmethod
+    def from_config(cls, config) -> tf.keras.layers.Layer:
+        return cls(**config)
+
+@keras.saving.register_keras_serializable(package='layers')
 class PositionalEmbedding(tf.keras.layers.Layer):
     def __init__(
         self,
         input_axis: int=1, # axis of the sequence
         output_axis: int=-1, # axis of the embedding
         **kwargs
     ):
@@ -209,65 +271,99 @@
         self._kernel = None
 
     def build(self, input_shape: tuple):
         # shape
         __axes = [self._input_axis % len(input_shape), self._output_axis % len(input_shape)]
         __shape = [(__d if __i in __axes else 1) for __i, __d in enumerate(list(input_shape))]
         # init values
-        __kernel_init = _mti.SmallNormal()
+        __kernel_init = tf.keras.initializers.GlorotNormal()
         # register the weights
         self._kernel = self.add_weight(name="kernel", shape=__shape, initializer=__kernel_init)
         # notify the model
         self.built = True
 
     def call(self, inputs: tf.Tensor):
         return inputs + self._kernel # each index in the sequence axis has a dedicated bias (different from dense bias)
 
+    def get_config(self) -> dict:
+        __parent_config = super(PositionalEmbedding, self).get_config()
+        __child_config = {
+            'input_axis': self._input_axis,
+            'output_axis': self._output_axis}
+        return {**__parent_config, **__child_config}
+
+    @classmethod
+    def from_config(cls, config) -> tf.keras.layers.Layer:
+        return cls(**config)
+
 # RESIDUALS ###################################################################
 
 # ACTIVATION ##################################################################
 
+@keras.saving.register_keras_serializable(package='layers')
 class Activation(tf.keras.layers.Layer):
     def __init__(
         self,
         function: callable,
         **kwargs
     ):
         super(Activation, self).__init__(**kwargs)
         self._function = function
 
     def call(self, inputs: tf.Tensor, **kwargs):
         return self._function(inputs)
 
+    def get_config(self) -> dict:
+        __parent_config = super(Activation, self).get_config()
+        __child_config = {'function': keras.saving.serialize_keras_object(self._function),}
+        return {**__parent_config, **__child_config}
+
+    @classmethod
+    def from_config(cls, config) -> tf.keras.layers.Layer:
+        __fn_config = config.pop('function')
+        __fn = keras.saving.deserialize_keras_object(__fn_config)
+        return cls(function=__fn, **config)
+
+@keras.saving.register_keras_serializable(package='layers')
 class Softmax(tf.keras.layers.Layer):
     def __init__(
         self,
         axis: int=-1,
         **kwargs
     ):
         super(Softmax, self).__init__(**kwargs)
         self._axis = axis
 
     def call(self, inputs: tf.Tensor, **kwargs):
         return tf.nn.softmax(inputs, axis=self._axis)
 
+    def get_config(self) -> dict:
+        __parent_config = super(Softmax, self).get_config()
+        __child_config = {'axis': self._axis,}
+        return {**__parent_config, **__child_config}
+
+    @classmethod
+    def from_config(cls, config) -> tf.keras.layers.Layer:
+        return cls(**config)
+
 # RESHAPING ###################################################################
 
 def _normalize_shape(shape: list) -> list:
     return [-1 if __d is None else __d for __d in shape]
 
 def _normalize_dim(dim: int) -> int:
     return -1 if (dim is None or dim < 0) else dim
 
 def _multiply_dim(dim_l: int, dim_r: int) -> int:
     return -1 if (dim_l == -1 or dim_r == -1) else dim_l * dim_r
 
 def _divide_dim(dim_l: int, dim_r: int) -> int:
     return -1 if (dim_l == -1 or dim_r == -1) else dim_l // dim_r
 
+@keras.saving.register_keras_serializable(package='layers')
 class Divide(tf.keras.layers.Layer):
     def __init__(
         self,
         input_axis: int, # relative to the NEW shape / rank
         output_axis: int, # same
         factor: int,
         insert: bool=False,
@@ -290,14 +386,28 @@
         # option to group data on a new axis
         if self._insert: __shape.insert(__axis1, 1)
         # move data from axis 0 to axis 1
         __shape[__axis0] = _divide_dim(__shape[__axis0], self._factor)
         __shape[__axis1] = _multiply_dim(__shape[__axis1], self._factor)
         return tf.reshape(tensor=inputs, shape=__shape)
 
+    def get_config(self) -> dict:
+        __parent_config = super(Divide, self).get_config()
+        __child_config = {
+            'input_axis': self._input_axis,
+            'output_axis': self._output_axis,
+            'factor': self._factor,
+            'insert': self._insert}
+        return {**__parent_config, **__child_config}
+
+    @classmethod
+    def from_config(cls, config) -> tf.keras.layers.Layer:
+        return cls(**config)
+
+@keras.saving.register_keras_serializable(package='layers')
 class Merge(tf.keras.layers.Layer):
     def __init__(
         self,
         left_axis: int=-2,
         right_axis: int=-1,
         left: bool=True,
         **kwargs
@@ -320,18 +430,40 @@
         __axis_d = __axis_r if self._left else __axis_l # deleted axis
         # new shape
         __shape[__axis_k] = __dim
         __shape.pop(__axis_d)
         # actually merge the two axes
         return tf.reshape(tensor=inputs, shape=__shape)
 
+    def get_config(self) -> dict:
+        __parent_config = super(Merge, self).get_config()
+        __child_config = {
+            'left_axis': self._left_axis,
+            'right_axis': self._right_axis,
+            'left': self._left}
+        return {**__parent_config, **__child_config}
+
+    @classmethod
+    def from_config(cls, config) -> tf.keras.layers.Layer:
+        return cls(**config)
+
+@keras.saving.register_keras_serializable(package='layers')
 class Reshape(tf.keras.layers.Layer):
     def __init__(
         self,
         target_shape: tuple,
         **kwargs
     ) -> None:
         super(Reshape, self).__init__(**kwargs)
         self._shape = target_shape
 
     def call(self, inputs: tf.Tensor, **kwargs) -> tf.Tensor:
         return tf.reshape(inputs, self._shape)
+
+    def get_config(self) -> dict:
+        __parent_config = super(Reshape, self).get_config()
+        __child_config = {'target_shape': self._shape,}
+        return {**__parent_config, **__child_config}
+
+    @classmethod
+    def from_config(cls, config) -> tf.keras.layers.Layer:
+        return cls(**config)
```

### Comparing `mlable-0.1.0/mlable/tensorflow/models.py` & `mlable-0.1.1/mlable/tensorflow/models.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/tensorflow/optimizers.py` & `mlable-0.1.1/mlable/tensorflow/optimizers.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/tensorflow/sampling.py` & `mlable-0.1.1/mlable/tensorflow/sampling.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/tensorflow/summary.py` & `mlable-0.1.1/mlable/tensorflow/summary.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/tokens/bpe.py` & `mlable-0.1.1/mlable/tokens/bpe.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/tokens/ngrams.py` & `mlable-0.1.1/mlable/tokens/ngrams.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/torch/layers.py` & `mlable-0.1.1/mlable/torch/layers.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/torch/optimizers.py` & `mlable-0.1.1/mlable/torch/optimizers.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/mlable/torch/sampling.py` & `mlable-0.1.1/mlable/torch/sampling.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.0/PKG-INFO` & `mlable-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlable
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tensorflow and pyTorch libs + atomic projects and drafts.
 Author: apehex
 Author-email: apehex@protonmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

