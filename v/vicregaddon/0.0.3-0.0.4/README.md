# Comparing `tmp/vicregaddon-0.0.3.tar.gz` & `tmp/vicregaddon-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vicregaddon-0.0.3.tar", last modified: Sun Apr 28 00:17:39 2024, max compression
+gzip compressed data, was "vicregaddon-0.0.4.tar", last modified: Tue May  7 00:50:30 2024, max compression
```

## Comparing `vicregaddon-0.0.3.tar` & `vicregaddon-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 shawley    (501) staff       (20)        0 2024-04-28 00:17:39.053774 vicregaddon-0.0.3/
--rw-r--r--   0 shawley    (501) staff       (20)     1072 2023-06-04 17:06:51.000000 vicregaddon-0.0.3/LICENSE
--rw-r--r--   0 shawley    (501) staff       (20)     1139 2024-04-28 00:17:39.053646 vicregaddon-0.0.3/PKG-INFO
--rw-r--r--   0 shawley    (501) staff       (20)      763 2024-04-28 00:16:39.000000 vicregaddon-0.0.3/README.md
--rw-r--r--   0 shawley    (501) staff       (20)       38 2024-04-28 00:17:39.053820 vicregaddon-0.0.3/setup.cfg
--rw-r--r--   0 shawley    (501) staff       (20)      699 2024-04-28 00:16:53.000000 vicregaddon-0.0.3/setup.py
-drwxr-xr-x   0 shawley    (501) staff       (20)        0 2024-04-28 00:17:39.052726 vicregaddon-0.0.3/vicregaddon/
--rw-r--r--   0 shawley    (501) staff       (20)       28 2023-06-04 20:31:47.000000 vicregaddon-0.0.3/vicregaddon/__init__.py
--rw-r--r--   0 shawley    (501) staff       (20)    11820 2024-04-28 00:07:13.000000 vicregaddon-0.0.3/vicregaddon/vicregaddon.py
-drwxr-xr-x   0 shawley    (501) staff       (20)        0 2024-04-28 00:17:39.053446 vicregaddon-0.0.3/vicregaddon.egg-info/
--rw-r--r--   0 shawley    (501) staff       (20)     1139 2024-04-28 00:17:39.000000 vicregaddon-0.0.3/vicregaddon.egg-info/PKG-INFO
--rw-r--r--   0 shawley    (501) staff       (20)      251 2024-04-28 00:17:39.000000 vicregaddon-0.0.3/vicregaddon.egg-info/SOURCES.txt
--rw-r--r--   0 shawley    (501) staff       (20)        1 2024-04-28 00:17:39.000000 vicregaddon-0.0.3/vicregaddon.egg-info/dependency_links.txt
--rw-r--r--   0 shawley    (501) staff       (20)       13 2024-04-28 00:17:39.000000 vicregaddon-0.0.3/vicregaddon.egg-info/requires.txt
--rw-r--r--   0 shawley    (501) staff       (20)       12 2024-04-28 00:17:39.000000 vicregaddon-0.0.3/vicregaddon.egg-info/top_level.txt
+drwxr-xr-x   0 shawley    (501) staff       (20)        0 2024-05-07 00:50:30.668107 vicregaddon-0.0.4/
+-rw-r--r--   0 shawley    (501) staff       (20)     1072 2023-06-04 17:06:51.000000 vicregaddon-0.0.4/LICENSE
+-rw-r--r--   0 shawley    (501) staff       (20)     1287 2024-05-07 00:50:30.667908 vicregaddon-0.0.4/PKG-INFO
+-rw-r--r--   0 shawley    (501) staff       (20)      868 2024-05-07 00:37:08.000000 vicregaddon-0.0.4/README.md
+-rw-r--r--   0 shawley    (501) staff       (20)       38 2024-05-07 00:50:30.668145 vicregaddon-0.0.4/setup.cfg
+-rw-r--r--   0 shawley    (501) staff       (20)      699 2024-05-07 00:37:08.000000 vicregaddon-0.0.4/setup.py
+drwxr-xr-x   0 shawley    (501) staff       (20)        0 2024-05-07 00:50:30.666894 vicregaddon-0.0.4/vicregaddon/
+-rw-r--r--   0 shawley    (501) staff       (20)       28 2023-06-04 20:31:47.000000 vicregaddon-0.0.4/vicregaddon/__init__.py
+-rw-r--r--   0 shawley    (501) staff       (20)    11918 2024-05-07 00:37:08.000000 vicregaddon-0.0.4/vicregaddon/vicregaddon.py
+drwxr-xr-x   0 shawley    (501) staff       (20)        0 2024-05-07 00:50:30.667705 vicregaddon-0.0.4/vicregaddon.egg-info/
+-rw-r--r--   0 shawley    (501) staff       (20)     1287 2024-05-07 00:50:30.000000 vicregaddon-0.0.4/vicregaddon.egg-info/PKG-INFO
+-rw-r--r--   0 shawley    (501) staff       (20)      251 2024-05-07 00:50:30.000000 vicregaddon-0.0.4/vicregaddon.egg-info/SOURCES.txt
+-rw-r--r--   0 shawley    (501) staff       (20)        1 2024-05-07 00:50:30.000000 vicregaddon-0.0.4/vicregaddon.egg-info/dependency_links.txt
+-rw-r--r--   0 shawley    (501) staff       (20)       13 2024-05-07 00:50:30.000000 vicregaddon-0.0.4/vicregaddon.egg-info/requires.txt
+-rw-r--r--   0 shawley    (501) staff       (20)       12 2024-05-07 00:50:30.000000 vicregaddon-0.0.4/vicregaddon.egg-info/top_level.txt
```

### Comparing `vicregaddon-0.0.3/LICENSE` & `vicregaddon-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vicregaddon-0.0.3/PKG-INFO` & `vicregaddon-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 Metadata-Version: 2.1
 Name: vicregaddon
-Version: 0.0.3
+Version: 0.0.4
 Summary: A lightweight and modular parallel PyTorch implementation of VICReg (intended for audio, but will try to be general)
 Home-page: https://github.com/drscotthawley/vicregaddon
 Author: Scott H. Hawley
 Author-email: scott.hawley@belmont.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: torch
+Requires-Dist: einops
 
 # vicregaddon
 
 > *"vicreg add-on".  As in "Yeah, but are you getting it? vicregaddon it"*
 
 A lightweight and modular parallel PyTorch implementation of [VICReg](https://github.com/facebookresearch/vicreg). 
 
 (I intend this for audio, but could be used for other things)
 
 ## Installation: 
 
 ```bash
 pip install vicregaddon
 ```
+or, for the most recent version
+```
+pip install git+https://github.com/drscotthawley/vicregaddon.git
+```
 
 
 ## Usage:
 ```python
 from vicregaddon import *
 ```
```

### Comparing `vicregaddon-0.0.3/README.md` & `vicregaddon-0.0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 (I intend this for audio, but could be used for other things)
 
 ## Installation: 
 
 ```bash
 pip install vicregaddon
 ```
+or, for the most recent version
+```
+pip install git+https://github.com/drscotthawley/vicregaddon.git
+```
 
 
 ## Usage:
 ```python
 from vicregaddon import *
 ```
```

### Comparing `vicregaddon-0.0.3/setup.py` & `vicregaddon-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='vicregaddon',
-    version='0.0.3',
+    version='0.0.4',
     url = 'https://github.com/drscotthawley/vicregaddon',
     license='MIT',
     author='Scott H. Hawley',
     author_email='scott.hawley@belmont.edu', 
     description='A lightweight and modular parallel PyTorch implementation of VICReg (intended for audio, but will try to be general)',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `vicregaddon-0.0.3/vicregaddon/vicregaddon.py` & `vicregaddon-0.0.4/vicregaddon/vicregaddon.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,19 +135,21 @@
     "gets off-diagnonal elements of a square (covariance) matrix; used by vicreg_cov_loss "
     n, m = x.shape
     assert n == m, f"off_diagonal: matrix must be square but got shape: {x.shape}"  
     return x.flatten()[:-1].view(n - 1, n + 1)[:, 1:].flatten()
 
 def vicreg_cov_loss(z:torch.Tensor):
     "Covariance loss for VICReg. the sum of the off-diagaonal terms of the covariance matrix"
-    num_features = z.shape[1]*z.shape[2]  
-    cov_z = torch.cov(rearrange(z, 'b c t -> ( c t ) b'))   
+    num_features = torch.prod(torch.tensor(z.shape[1:]))
+    z_batch_last = z.view(z.shape[0],-1).T # flatten all but batch dim, .T puts batch dim last for cov
+    cov_z = torch.cov(z_batch_last)     
     return off_diagonal(cov_z).pow_(2).sum().div(num_features)
 
 
+
 # now a full class that does a lot of things for you
 class VICRegLoss(nn.Module):
     """
     Follows the loss APIs used in Harmonai's OOBLECK repo 
     VICReg, https://arxiv.org/abs/2105.04906, https://github.com/facebookresearch/vicreg/
     VICReg operates on the projections z of the autoencoder's latent encodings y.
     """
```

### Comparing `vicregaddon-0.0.3/vicregaddon.egg-info/PKG-INFO` & `vicregaddon-0.0.4/vicregaddon.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 Metadata-Version: 2.1
 Name: vicregaddon
-Version: 0.0.3
+Version: 0.0.4
 Summary: A lightweight and modular parallel PyTorch implementation of VICReg (intended for audio, but will try to be general)
 Home-page: https://github.com/drscotthawley/vicregaddon
 Author: Scott H. Hawley
 Author-email: scott.hawley@belmont.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: torch
+Requires-Dist: einops
 
 # vicregaddon
 
 > *"vicreg add-on".  As in "Yeah, but are you getting it? vicregaddon it"*
 
 A lightweight and modular parallel PyTorch implementation of [VICReg](https://github.com/facebookresearch/vicreg). 
 
 (I intend this for audio, but could be used for other things)
 
 ## Installation: 
 
 ```bash
 pip install vicregaddon
 ```
+or, for the most recent version
+```
+pip install git+https://github.com/drscotthawley/vicregaddon.git
+```
 
 
 ## Usage:
 ```python
 from vicregaddon import *
 ```
```

