# Comparing `tmp/q-transformer-0.1.8.tar.gz` & `tmp/q-transformer-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q-transformer-0.1.8.tar", last modified: Fri Jan 26 17:57:10 2024, max compression
+gzip compressed data, was "q-transformer-0.1.9.tar", last modified: Tue Jan 30 17:52:57 2024, max compression
```

## Comparing `q-transformer-0.1.8.tar` & `q-transformer-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 17:57:10.016816 q-transformer-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-01-26 17:56:59.000000 q-transformer-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-01-26 17:57:10.016816 q-transformer-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-01-26 17:56:59.000000 q-transformer-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 17:57:10.012817 q-transformer-0.1.8/q_transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-01-26 17:56:59.000000 q-transformer-0.1.8/q_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9416 2024-01-26 17:56:59.000000 q-transformer-0.1.8/q_transformer/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-01-26 17:56:59.000000 q-transformer-0.1.8/q_transformer/attend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-01-26 17:56:59.000000 q-transformer-0.1.8/q_transformer/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-01-26 17:56:59.000000 q-transformer-0.1.8/q_transformer/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    19421 2024-01-26 17:56:59.000000 q-transformer-0.1.8/q_transformer/q_learner.py
--rw-r--r--   0 runner    (1001) docker     (127)    35520 2024-01-26 17:56:59.000000 q-transformer-0.1.8/q_transformer/q_robotic_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 17:57:10.016816 q-transformer-0.1.8/q_transformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-01-26 17:57:10.000000 q-transformer-0.1.8/q_transformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-01-26 17:57:10.000000 q-transformer-0.1.8/q_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 17:57:10.000000 q-transformer-0.1.8/q_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-01-26 17:57:10.000000 q-transformer-0.1.8/q_transformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-26 17:57:10.000000 q-transformer-0.1.8/q_transformer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-26 17:57:10.016816 q-transformer-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-01-26 17:56:59.000000 q-transformer-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 17:52:57.780114 q-transformer-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-01-30 17:52:42.000000 q-transformer-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-01-30 17:52:57.780114 q-transformer-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-01-30 17:52:42.000000 q-transformer-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 17:52:57.776114 q-transformer-0.1.9/q_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-01-30 17:52:42.000000 q-transformer-0.1.9/q_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9416 2024-01-30 17:52:42.000000 q-transformer-0.1.9/q_transformer/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-01-30 17:52:42.000000 q-transformer-0.1.9/q_transformer/attend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-01-30 17:52:42.000000 q-transformer-0.1.9/q_transformer/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-01-30 17:52:42.000000 q-transformer-0.1.9/q_transformer/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19421 2024-01-30 17:52:42.000000 q-transformer-0.1.9/q_transformer/q_learner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35498 2024-01-30 17:52:42.000000 q-transformer-0.1.9/q_transformer/q_robotic_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 17:52:57.780114 q-transformer-0.1.9/q_transformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-01-30 17:52:57.000000 q-transformer-0.1.9/q_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-01-30 17:52:57.000000 q-transformer-0.1.9/q_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 17:52:57.000000 q-transformer-0.1.9/q_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-01-30 17:52:57.000000 q-transformer-0.1.9/q_transformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-30 17:52:57.000000 q-transformer-0.1.9/q_transformer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 17:52:57.780114 q-transformer-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-01-30 17:52:42.000000 q-transformer-0.1.9/setup.py
```

### Comparing `q-transformer-0.1.8/LICENSE` & `q-transformer-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `q-transformer-0.1.8/PKG-INFO` & `q-transformer-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: q-transformer
-Version: 0.1.8
+Version: 0.1.9
 Summary: Q-Transformer
 Home-page: https://github.com/lucidrains/q-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanisms,transformers,q-learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `q-transformer-0.1.8/README.md` & `q-transformer-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `q-transformer-0.1.8/q_transformer/agent.py` & `q-transformer-0.1.9/q_transformer/agent.py`

 * *Files identical despite different names*

### Comparing `q-transformer-0.1.8/q_transformer/attend.py` & `q-transformer-0.1.9/q_transformer/attend.py`

 * *Files identical despite different names*

### Comparing `q-transformer-0.1.8/q_transformer/mocks.py` & `q-transformer-0.1.9/q_transformer/mocks.py`

 * *Files identical despite different names*

### Comparing `q-transformer-0.1.8/q_transformer/optimizer.py` & `q-transformer-0.1.9/q_transformer/optimizer.py`

 * *Files identical despite different names*

### Comparing `q-transformer-0.1.8/q_transformer/q_learner.py` & `q-transformer-0.1.9/q_transformer/q_learner.py`

 * *Files identical despite different names*

### Comparing `q-transformer-0.1.8/q_transformer/q_robotic_transformer.py` & `q-transformer-0.1.9/q_transformer/q_robotic_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -883,37 +883,36 @@
 
             q_values = values + (advantages - reduce(advantages, '... a -> ... 1', 'mean'))
         else:
             q_values = logits
 
         return q_values.sigmoid()
 
-    def get_random_actions(self, batch_size, num_action_bins = None):
-        num_action_bins = default(num_action_bins, self.action_bins)
-        return torch.randint(0, num_action_bins, (batch_size, num_action_bins), device = self.device)
+    def get_random_actions(self, batch_size, num_actions = None):
+        num_actions = default(num_actions, self.num_actions)
+        return torch.randint(0, self.action_bins, (batch_size, num_actions), device = self.device)
 
     @torch.no_grad()
     def get_optimal_actions(
         self,
         encoded_state,
         return_q_values = False,
         actions: Optional[Tensor] = None,
         prob_random_action: float = 0.5,
         **kwargs
     ):
         assert 0. <= prob_random_action <= 1.
         batch = encoded_state.shape[0]
 
         if prob_random_action == 1:
-            return self.get_random_actions(self, batch)
+            return self.get_random_actions(batch)
 
         sos_token = reduce(encoded_state, 'b ... d -> b 1 d', 'mean')
         tokens = self.maybe_append_actions(sos_token, actions = actions)
 
-
         action_bins = []
         cache = None
 
         for action_idx in range(self.num_actions):
 
             embed, cache = self.transformer(
                 tokens,
```

### Comparing `q-transformer-0.1.8/q_transformer.egg-info/PKG-INFO` & `q-transformer-0.1.9/q_transformer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: q-transformer
-Version: 0.1.8
+Version: 0.1.9
 Summary: Q-Transformer
 Home-page: https://github.com/lucidrains/q-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanisms,transformers,q-learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `q-transformer-0.1.8/setup.py` & `q-transformer-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'q-transformer',
   packages = find_packages(exclude=[]),
-  version = '0.1.8',
+  version = '0.1.9',
   license='MIT',
   description = 'Q-Transformer',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/q-transformer',
   keywords = [
```

