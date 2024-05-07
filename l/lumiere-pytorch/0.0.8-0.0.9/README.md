# Comparing `tmp/lumiere-pytorch-0.0.8.tar.gz` & `tmp/lumiere-pytorch-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumiere-pytorch-0.0.8.tar", last modified: Sat Feb 10 17:22:41 2024, max compression
+gzip compressed data, was "lumiere-pytorch-0.0.9.tar", last modified: Sat Feb 10 17:27:40 2024, max compression
```

## Comparing `lumiere-pytorch-0.0.8.tar` & `lumiere-pytorch-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 17:22:41.606073 lumiere-pytorch-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-02-10 17:22:29.000000 lumiere-pytorch-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-02-10 17:22:41.602073 lumiere-pytorch-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-02-10 17:22:29.000000 lumiere-pytorch-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 17:22:41.602073 lumiere-pytorch-0.0.8/lumiere_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-10 17:22:29.000000 lumiere-pytorch-0.0.8/lumiere_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8972 2024-02-10 17:22:29.000000 lumiere-pytorch-0.0.8/lumiere_pytorch/lumiere_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 17:22:41.602073 lumiere-pytorch-0.0.8/lumiere_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-02-10 17:22:41.000000 lumiere-pytorch-0.0.8/lumiere_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-02-10 17:22:41.000000 lumiere-pytorch-0.0.8/lumiere_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-10 17:22:41.000000 lumiere-pytorch-0.0.8/lumiere_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-10 17:22:41.000000 lumiere-pytorch-0.0.8/lumiere_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-10 17:22:41.000000 lumiere-pytorch-0.0.8/lumiere_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-10 17:22:41.606073 lumiere-pytorch-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-02-10 17:22:29.000000 lumiere-pytorch-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 17:27:40.960370 lumiere-pytorch-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-02-10 17:27:31.000000 lumiere-pytorch-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-02-10 17:27:40.960370 lumiere-pytorch-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-02-10 17:27:31.000000 lumiere-pytorch-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 17:27:40.956370 lumiere-pytorch-0.0.9/lumiere_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-10 17:27:31.000000 lumiere-pytorch-0.0.9/lumiere_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9010 2024-02-10 17:27:31.000000 lumiere-pytorch-0.0.9/lumiere_pytorch/lumiere_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 17:27:40.960370 lumiere-pytorch-0.0.9/lumiere_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-02-10 17:27:40.000000 lumiere-pytorch-0.0.9/lumiere_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-02-10 17:27:40.000000 lumiere-pytorch-0.0.9/lumiere_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-10 17:27:40.000000 lumiere-pytorch-0.0.9/lumiere_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-10 17:27:40.000000 lumiere-pytorch-0.0.9/lumiere_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-10 17:27:40.000000 lumiere-pytorch-0.0.9/lumiere_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-10 17:27:40.960370 lumiere-pytorch-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-02-10 17:27:31.000000 lumiere-pytorch-0.0.9/setup.py
```

### Comparing `lumiere-pytorch-0.0.8/LICENSE` & `lumiere-pytorch-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lumiere-pytorch-0.0.8/PKG-INFO` & `lumiere-pytorch-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumiere-pytorch
-Version: 0.0.8
+Version: 0.0.9
 Summary: Lumiere
 Home-page: https://github.com/lucidrains/lumiere-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,text-to-video
 Classifier: Development Status :: 4 - Beta
```

### Comparing `lumiere-pytorch-0.0.8/README.md` & `lumiere-pytorch-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `lumiere-pytorch-0.0.8/lumiere_pytorch/lumiere_pytorch.py` & `lumiere-pytorch-0.0.9/lumiere_pytorch/lumiere_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import torch
 from torch import nn, einsum, Tensor, is_tensor
 from torch.nn import Module, ModuleList
 import torch.nn.functional as F
 
 from beartype import beartype
 
-from einops import rearrange, pack, unpack
+from einops import rearrange, pack, unpack, repeat
 
 from optree import tree_flatten, tree_unflatten
 
 from x_transformers.x_transformers import (
     Attention,
     RMSNorm
 )
@@ -332,17 +332,17 @@
 
         all_args = (args, kwargs)
         all_args, pytree_spec = tree_flatten(all_args)
 
         # and repeat across for each frame of the video
         # so one conditions all images of each video with same input
 
-        for arg in all_args:
+        for ind, arg in enumerate(all_args):
             if is_tensor(arg):
-                arg = repeat(arg, 'b ... -> (b t)', t = time)
+                all_args[ind] = repeat(arg, 'b ... -> (b t) ...', t = time)
 
         # turn video into a stack of images
 
         images = rearrange(video, 'b c t h w -> (b t) c h w')
 
         # unflatten arguments to be passed into text-to-image model
```

### Comparing `lumiere-pytorch-0.0.8/lumiere_pytorch.egg-info/PKG-INFO` & `lumiere-pytorch-0.0.9/lumiere_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumiere-pytorch
-Version: 0.0.8
+Version: 0.0.9
 Summary: Lumiere
 Home-page: https://github.com/lucidrains/lumiere-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,text-to-video
 Classifier: Development Status :: 4 - Beta
```

### Comparing `lumiere-pytorch-0.0.8/setup.py` & `lumiere-pytorch-0.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'lumiere-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.8',
+  version = '0.0.9',
   license='MIT',
   description = 'Lumiere',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/lumiere-pytorch',
   keywords = [
```

