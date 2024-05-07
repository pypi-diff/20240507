# Comparing `tmp/magvit2_pytorch-0.4.2.tar.gz` & `tmp/magvit2_pytorch-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magvit2_pytorch-0.4.2.tar", last modified: Fri May  3 17:30:40 2024, max compression
+gzip compressed data, was "magvit2_pytorch-0.4.3.tar", last modified: Tue May  7 14:16:40 2024, max compression
```

## Comparing `magvit2_pytorch-0.4.2.tar` & `magvit2_pytorch-0.4.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:30:40.842503 magvit2_pytorch-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-03 17:30:36.000000 magvit2_pytorch-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-03 17:30:40.842503 magvit2_pytorch-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-05-03 17:30:36.000000 magvit2_pytorch-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:30:40.842503 magvit2_pytorch-0.4.2/magvit2_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-03 17:30:36.000000 magvit2_pytorch-0.4.2/magvit2_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-05-03 17:30:36.000000 magvit2_pytorch-0.4.2/magvit2_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-03 17:30:36.000000 magvit2_pytorch-0.4.2/magvit2_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    56410 2024-05-03 17:30:36.000000 magvit2_pytorch-0.4.2/magvit2_pytorch/magvit2_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-03 17:30:36.000000 magvit2_pytorch-0.4.2/magvit2_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-05-03 17:30:36.000000 magvit2_pytorch-0.4.2/magvit2_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 17:30:36.000000 magvit2_pytorch-0.4.2/magvit2_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:30:40.842503 magvit2_pytorch-0.4.2/magvit2_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-03 17:30:40.000000 magvit2_pytorch-0.4.2/magvit2_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-03 17:30:40.000000 magvit2_pytorch-0.4.2/magvit2_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:30:40.000000 magvit2_pytorch-0.4.2/magvit2_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-03 17:30:40.000000 magvit2_pytorch-0.4.2/magvit2_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 17:30:40.000000 magvit2_pytorch-0.4.2/magvit2_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 17:30:40.842503 magvit2_pytorch-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-03 17:30:36.000000 magvit2_pytorch-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:16:40.628078 magvit2_pytorch-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-07 14:16:36.000000 magvit2_pytorch-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-07 14:16:40.628078 magvit2_pytorch-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-05-07 14:16:36.000000 magvit2_pytorch-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:16:40.624078 magvit2_pytorch-0.4.3/magvit2_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-07 14:16:36.000000 magvit2_pytorch-0.4.3/magvit2_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-05-07 14:16:36.000000 magvit2_pytorch-0.4.3/magvit2_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-07 14:16:36.000000 magvit2_pytorch-0.4.3/magvit2_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56410 2024-05-07 14:16:36.000000 magvit2_pytorch-0.4.3/magvit2_pytorch/magvit2_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-07 14:16:36.000000 magvit2_pytorch-0.4.3/magvit2_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16817 2024-05-07 14:16:36.000000 magvit2_pytorch-0.4.3/magvit2_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 14:16:36.000000 magvit2_pytorch-0.4.3/magvit2_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:16:40.628078 magvit2_pytorch-0.4.3/magvit2_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-07 14:16:40.000000 magvit2_pytorch-0.4.3/magvit2_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-07 14:16:40.000000 magvit2_pytorch-0.4.3/magvit2_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:16:40.000000 magvit2_pytorch-0.4.3/magvit2_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-07 14:16:40.000000 magvit2_pytorch-0.4.3/magvit2_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 14:16:40.000000 magvit2_pytorch-0.4.3/magvit2_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 14:16:40.628078 magvit2_pytorch-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-07 14:16:36.000000 magvit2_pytorch-0.4.3/setup.py
```

### Comparing `magvit2_pytorch-0.4.2/LICENSE` & `magvit2_pytorch-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `magvit2_pytorch-0.4.2/PKG-INFO` & `magvit2_pytorch-0.4.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magvit2-pytorch
-Version: 0.4.2
+Version: 0.4.3
 Summary: MagViT2 - Pytorch
 Home-page: https://github.com/lucidrains/magvit2-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformer,attention mechanisms,generative video model
 Classifier: Development Status :: 4 - Beta
```

### Comparing `magvit2_pytorch-0.4.2/README.md` & `magvit2_pytorch-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `magvit2_pytorch-0.4.2/magvit2_pytorch/attend.py` & `magvit2_pytorch-0.4.3/magvit2_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `magvit2_pytorch-0.4.2/magvit2_pytorch/data.py` & `magvit2_pytorch-0.4.3/magvit2_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `magvit2_pytorch-0.4.2/magvit2_pytorch/magvit2_pytorch.py` & `magvit2_pytorch-0.4.3/magvit2_pytorch/magvit2_pytorch.py`

 * *Files identical despite different names*

### Comparing `magvit2_pytorch-0.4.2/magvit2_pytorch/optimizer.py` & `magvit2_pytorch-0.4.3/magvit2_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `magvit2_pytorch-0.4.2/magvit2_pytorch/trainer.py` & `magvit2_pytorch-0.4.3/magvit2_pytorch/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,14 +263,18 @@
     def is_main(self):
         return self.accelerator.is_main_process
 
     @property
     def is_local_main(self):
         return self.accelerator.is_local_main_process
 
+    @property
+    def unwrapped_model(self):
+        return self.accelerator.unwrap_model(self.model)
+
     def wait(self):
         return self.accelerator.wait_for_everyone()
 
     def print(self, msg):
         return self.accelerator.print(msg)
 
     @property
@@ -457,15 +461,15 @@
         recon_videos = []
 
         for _ in range(self.grad_accum_every):
             valid_video, = next(dl_iter)
             valid_video = valid_video.to(self.device)
 
             with self.accelerator.autocast():
-                loss, _ = self.model(valid_video, return_recon_loss_only = True)
+                loss, _ = self.unwrapped_model(valid_video, return_recon_loss_only = True)
                 ema_loss, ema_recon_video = self.ema_model(valid_video, return_recon_loss_only = True)
 
             recon_loss += loss / self.grad_accum_every
             ema_recon_loss += ema_loss / self.grad_accum_every
 
             if valid_video.ndim == 4:
                 valid_video = rearrange(valid_video, 'b c h w -> b c 1 h w')
```

### Comparing `magvit2_pytorch-0.4.2/magvit2_pytorch.egg-info/PKG-INFO` & `magvit2_pytorch-0.4.3/magvit2_pytorch.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magvit2-pytorch
-Version: 0.4.2
+Version: 0.4.3
 Summary: MagViT2 - Pytorch
 Home-page: https://github.com/lucidrains/magvit2-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformer,attention mechanisms,generative video model
 Classifier: Development Status :: 4 - Beta
```

### Comparing `magvit2_pytorch-0.4.2/setup.py` & `magvit2_pytorch-0.4.3/setup.py`

 * *Files identical despite different names*

