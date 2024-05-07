# Comparing `tmp/weaver-core-0.4.8.tar.gz` & `tmp/weaver-core-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weaver-core-0.4.8.tar", last modified: Mon Dec 11 13:10:06 2023, max compression
+gzip compressed data, was "weaver-core-0.4.9.tar", last modified: Fri Dec 15 10:14:31 2023, max compression
```

## Comparing `weaver-core-0.4.8.tar` & `weaver-core-0.4.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:06.146450 weaver-core-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-12-11 13:09:22.000000 weaver-core-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16041 2023-12-11 13:10:06.146450 weaver-core-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15472 2023-12-11 13:09:22.000000 weaver-core-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-11 13:10:06.146450 weaver-core-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2023-12-11 13:09:22.000000 weaver-core-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:06.142450 weaver-core-0.4.8/weaver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 13:09:22.000000 weaver-core-0.4.8/weaver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:06.142450 weaver-core-0.4.8/weaver/nn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 13:09:22.000000 weaver-core-0.4.8/weaver/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:06.142450 weaver-core-0.4.8/weaver/nn/loss/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 13:09:22.000000 weaver-core-0.4.8/weaver/nn/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5514 2023-12-11 13:09:22.000000 weaver-core-0.4.8/weaver/nn/loss/focal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:06.142450 weaver-core-0.4.8/weaver/nn/model/
--rw-r--r--   0 runner    (1001) docker     (127)    35306 2023-12-11 13:09:22.000000 weaver-core-0.4.8/weaver/nn/model/ParticleNeXt.py
--rw-r--r--   0 runner    (1001) docker     (127)    10647 2023-12-11 13:09:22.000000 weaver-core-0.4.8/weaver/nn/model/ParticleNet.py
--rw-r--r--   0 runner    (1001) docker     (127)    30175 2023-12-11 13:09:22.000000 weaver-core-0.4.8/weaver/nn/model/ParticleTransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 13:09:22.000000 weaver-core-0.4.8/weaver/nn/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47000 2023-12-11 13:09:22.000000 weaver-core-0.4.8/weaver/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:06.146450 weaver-core-0.4.8/weaver/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 13:09:22.000000 weaver-core-0.4.8/weaver/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:06.146450 weaver-core-0.4.8/weaver/utils/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 13:09:22.000000 weaver-core-0.4.8/weaver/utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11841 2023-12-11 13:09:22.000000 weaver-core-0.4.8/weaver/utils/data/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2023-12-11 13:09:22.000000 weaver-core-0.4.8/weaver/utils/data/fileio.py
--rw-r--r--   0 runner    (1001) docker     (127)    14762 2023-12-11 13:09:22.000000 weaver-core-0.4.8/weaver/utils/data/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     4710 2023-12-11 13:09:22.000000 weaver-core-0.4.8/weaver/utils/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    17958 2023-12-11 13:09:22.000000 weaver-core-0.4.8/weaver/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    17989 2023-12-11 13:09:22.000000 weaver-core-0.4.8/weaver/utils/flops_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2023-12-11 13:09:22.000000 weaver-core-0.4.8/weaver/utils/import_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2023-12-11 13:09:22.000000 weaver-core-0.4.8/weaver/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    20846 2023-12-11 13:09:22.000000 weaver-core-0.4.8/weaver/utils/lr_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:06.146450 weaver-core-0.4.8/weaver/utils/nn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 13:09:22.000000 weaver-core-0.4.8/weaver/utils/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2023-12-11 13:09:22.000000 weaver-core-0.4.8/weaver/utils/nn/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:06.146450 weaver-core-0.4.8/weaver/utils/nn/optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 13:09:22.000000 weaver-core-0.4.8/weaver/utils/nn/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2023-12-11 13:09:22.000000 weaver-core-0.4.8/weaver/utils/nn/optimizer/lookahead.py
--rw-r--r--   0 runner    (1001) docker     (127)    10549 2023-12-11 13:09:22.000000 weaver-core-0.4.8/weaver/utils/nn/optimizer/radam.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2023-12-11 13:09:22.000000 weaver-core-0.4.8/weaver/utils/nn/optimizer/ranger.py
--rw-r--r--   0 runner    (1001) docker     (127)    20237 2023-12-11 13:09:22.000000 weaver-core-0.4.8/weaver/utils/nn/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:06.146450 weaver-core-0.4.8/weaver_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16041 2023-12-11 13:10:06.000000 weaver-core-0.4.8/weaver_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-12-11 13:10:06.000000 weaver-core-0.4.8/weaver_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 13:10:06.000000 weaver-core-0.4.8/weaver_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-11 13:10:06.000000 weaver-core-0.4.8/weaver_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 13:10:06.000000 weaver-core-0.4.8/weaver_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-12-11 13:10:06.000000 weaver-core-0.4.8/weaver_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-11 13:10:06.000000 weaver-core-0.4.8/weaver_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 10:14:31.297516 weaver-core-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-12-15 10:13:56.000000 weaver-core-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16041 2023-12-15 10:14:31.297516 weaver-core-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15472 2023-12-15 10:13:56.000000 weaver-core-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-15 10:14:31.297516 weaver-core-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2023-12-15 10:13:56.000000 weaver-core-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 10:14:31.293516 weaver-core-0.4.9/weaver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 10:13:56.000000 weaver-core-0.4.9/weaver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 10:14:31.293516 weaver-core-0.4.9/weaver/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 10:13:56.000000 weaver-core-0.4.9/weaver/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 10:14:31.293516 weaver-core-0.4.9/weaver/nn/loss/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 10:13:56.000000 weaver-core-0.4.9/weaver/nn/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5514 2023-12-15 10:13:56.000000 weaver-core-0.4.9/weaver/nn/loss/focal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 10:14:31.293516 weaver-core-0.4.9/weaver/nn/model/
+-rw-r--r--   0 runner    (1001) docker     (127)    35306 2023-12-15 10:13:56.000000 weaver-core-0.4.9/weaver/nn/model/ParticleNeXt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10647 2023-12-15 10:13:56.000000 weaver-core-0.4.9/weaver/nn/model/ParticleNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30175 2023-12-15 10:13:56.000000 weaver-core-0.4.9/weaver/nn/model/ParticleTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 10:13:56.000000 weaver-core-0.4.9/weaver/nn/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47163 2023-12-15 10:13:56.000000 weaver-core-0.4.9/weaver/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 10:14:31.293516 weaver-core-0.4.9/weaver/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 10:13:56.000000 weaver-core-0.4.9/weaver/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 10:14:31.293516 weaver-core-0.4.9/weaver/utils/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 10:13:56.000000 weaver-core-0.4.9/weaver/utils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11999 2023-12-15 10:13:56.000000 weaver-core-0.4.9/weaver/utils/data/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2023-12-15 10:13:56.000000 weaver-core-0.4.9/weaver/utils/data/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14762 2023-12-15 10:13:56.000000 weaver-core-0.4.9/weaver/utils/data/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4710 2023-12-15 10:13:56.000000 weaver-core-0.4.9/weaver/utils/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18082 2023-12-15 10:13:56.000000 weaver-core-0.4.9/weaver/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17989 2023-12-15 10:13:56.000000 weaver-core-0.4.9/weaver/utils/flops_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2023-12-15 10:13:56.000000 weaver-core-0.4.9/weaver/utils/import_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2023-12-15 10:13:56.000000 weaver-core-0.4.9/weaver/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20846 2023-12-15 10:13:56.000000 weaver-core-0.4.9/weaver/utils/lr_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 10:14:31.293516 weaver-core-0.4.9/weaver/utils/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 10:13:56.000000 weaver-core-0.4.9/weaver/utils/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2023-12-15 10:13:56.000000 weaver-core-0.4.9/weaver/utils/nn/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 10:14:31.297516 weaver-core-0.4.9/weaver/utils/nn/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 10:13:56.000000 weaver-core-0.4.9/weaver/utils/nn/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2023-12-15 10:13:56.000000 weaver-core-0.4.9/weaver/utils/nn/optimizer/lookahead.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10549 2023-12-15 10:13:56.000000 weaver-core-0.4.9/weaver/utils/nn/optimizer/radam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2023-12-15 10:13:56.000000 weaver-core-0.4.9/weaver/utils/nn/optimizer/ranger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20434 2023-12-15 10:13:56.000000 weaver-core-0.4.9/weaver/utils/nn/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 10:14:31.297516 weaver-core-0.4.9/weaver_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16041 2023-12-15 10:14:31.000000 weaver-core-0.4.9/weaver_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-12-15 10:14:31.000000 weaver-core-0.4.9/weaver_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-15 10:14:31.000000 weaver-core-0.4.9/weaver_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-15 10:14:31.000000 weaver-core-0.4.9/weaver_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-15 10:14:31.000000 weaver-core-0.4.9/weaver_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2023-12-15 10:14:31.000000 weaver-core-0.4.9/weaver_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-15 10:14:31.000000 weaver-core-0.4.9/weaver_core.egg-info/top_level.txt
```

### Comparing `weaver-core-0.4.8/LICENSE` & `weaver-core-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.8/PKG-INFO` & `weaver-core-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weaver-core
-Version: 0.4.8
+Version: 0.4.9
 Summary: A streamlined deep-learning framework for high energy physics
 Home-page: https://github.com/hqucms/weaver-core
 Author: H. Qu, C. Li
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `weaver-core-0.4.8/README.md` & `weaver-core-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.8/setup.py` & `weaver-core-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         if not line:
             continue
         if line.startswith('#'):
             continue
         install_requires.append(line)
 
 setup(name="weaver-core",
-      version='0.4.8',
+      version='0.4.9',
       description="A streamlined deep-learning framework for high energy physics",
       long_description_content_type="text/markdown",
       author="H. Qu, C. Li",
       url="https://github.com/hqucms/weaver-core",
       long_description=long_desc,
       entry_points={'console_scripts':
                     ['weaver = weaver.train:main']},
```

### Comparing `weaver-core-0.4.8/weaver/nn/loss/focal.py` & `weaver-core-0.4.9/weaver/nn/loss/focal.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.8/weaver/nn/model/ParticleNeXt.py` & `weaver-core-0.4.9/weaver/nn/model/ParticleNeXt.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.8/weaver/nn/model/ParticleNet.py` & `weaver-core-0.4.9/weaver/nn/model/ParticleNet.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.8/weaver/nn/model/ParticleTransformer.py` & `weaver-core-0.4.9/weaver/nn/model/ParticleTransformer.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.8/weaver/train.py` & `weaver-core-0.4.9/weaver/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -603,22 +603,24 @@
     from collections import defaultdict
     from weaver.utils.data.tools import _concat
     _logger.info('Start running IO test')
     monitor_info = defaultdict(list)
 
     for X, y, Z in tqdm(data_loader):
         for k, v in Z.items():
-            monitor_info[k].append(v.cpu().numpy())
+            monitor_info[k].append(v)
     monitor_info = {k: _concat(v) for k, v in monitor_info.items()}
     if monitor_info:
-        monitor_output_path = 'weaver_monitor_info.pkl'
-        import pickle
-        with open(monitor_output_path, 'wb') as f:
-            pickle.dump(monitor_info, f)
-        _logger.info('Monitor info written to %s' % monitor_output_path)
+        monitor_output_path = 'weaver_monitor_info.parquet'
+        try:
+            import awkward as ak
+            ak.to_parquet(ak.Array(monitor_info), monitor_output_path, compression='LZ4', compression_level=4)
+            _logger.info('Monitor info written to %s' % monitor_output_path, color='bold')
+        except Exception as e:
+            _logger.error('Error when writing output parquet file: \n' + str(e))
 
 
 def save_root(args, output_path, data_config, scores, labels, observers):
     """
     Saves as .root
     :param data_config:
     :param scores:
```

### Comparing `weaver-core-0.4.8/weaver/utils/data/config.py` & `weaver-core-0.4.9/weaver/utils/data/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,16 @@
                 if self.reweight_hists is not None:
                     for k, v in self.reweight_hists.items():
                         self.reweight_hists[k] = np.array(v, dtype='float32')
         # observers
         self.observer_names = tuple(opts['observers'])
         # monitor variables
         self.monitor_variables = tuple(opts['monitor_variables'])
+        if self.observer_names and self.monitor_variables:
+            raise RuntimeError('Cannot set `observers` and `monitor_variables` at the same time.')
         # Z variables: returned as `Z` in the dataloader (use monitor_variables for training, observers for eval)
         self.z_variables = self.observer_names if len(self.observer_names) > 0 else self.monitor_variables
 
         # remove self mapping from var_funcs
         for k, v in self.var_funcs.items():
             if k == v:
                 del self.var_funcs[k]
```

### Comparing `weaver-core-0.4.8/weaver/utils/data/fileio.py` & `weaver-core-0.4.9/weaver/utils/data/fileio.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.8/weaver/utils/data/preprocess.py` & `weaver-core-0.4.9/weaver/utils/data/preprocess.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.8/weaver/utils/data/tools.py` & `weaver-core-0.4.9/weaver/utils/data/tools.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.8/weaver/utils/dataset.py` & `weaver-core-0.4.9/weaver/utils/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 import numpy as np
 import awkward as ak
 import torch.utils.data
 
 from functools import partial
 from concurrent.futures.thread import ThreadPoolExecutor
 from .logger import _logger
-from .data.tools import _pad, _repeat_pad, _clip
+from .data.tools import _pad, _repeat_pad, _clip, _stack
 from .data.fileio import _read_files
 from .data.config import DataConfig, _md5
 from .data.preprocess import _apply_selection, _build_new_variables, _build_weights, AutoStandardizer, WeightMaker
 
 
+def _collate_awkward_array_fn(batch, *, collate_fn_map=None):
+    return _stack(batch, axis=0)
+
+
 def _finalize_inputs(table, data_config):
     output = {}
     # copy observer variables before transformation
     for k in data_config.z_variables:
         if k in data_config.observer_names:
-            a = ak.to_numpy(table[k])
-            if a.dtype in (np.uint16, np.uint32, np.uint64):
-                # FIXME: hack as torch only supports float64, float32, float16, complex64, complex128, int64, int32, int16, int8, uint8, and bool
-                a = a.astype('int64')
-            output[k] = a
+            output[k] = table[k]  # ak.Array
     # copy labels
     for k in data_config.label_names:
         output[k] = ak.to_numpy(table[k])
     # transformation
     for k, params in data_config.preprocess_params.items():
         if data_config._auto_standardization and params['center'] == 'auto':
             raise ValueError('No valid standardization params for %s' % k)
@@ -43,18 +43,18 @@
             table[k] = np.nan_to_num(table[k])
     # stack variables for each input group
     for k, names in data_config.input_dicts.items():
         if len(names) == 1 and data_config.preprocess_params[names[0]]['length'] is None:
             output['_' + k] = ak.to_numpy(ak.values_astype(table[names[0]], 'float32'))
         else:
             output['_' + k] = ak.to_numpy(np.stack([ak.to_numpy(table[n]).astype('float32') for n in names], axis=1))
-    # copy monitor variables
+    # copy monitor variables (after transformation)
     for k in data_config.z_variables:
-        if k not in output:
-            output[k] = ak.to_numpy(table[k])
+        if k in data_config.monitor_variables:
+            output[k] = table[k]  # ak.Array
     return output
 
 
 def _get_reweight_indices(weights, up_sample=True, max_resample=10, weight_scale=1):
     all_indices = np.arange(len(weights))
     randwgt = np.random.uniform(low=0, high=weight_scale, size=len(weights))
     keep_flags = randwgt < weights
@@ -63,15 +63,15 @@
     else:
         n_repeats = len(weights) // max(1, int(keep_flags.sum()))
         if n_repeats > max_resample:
             n_repeats = max_resample
         all_indices = np.repeat(np.arange(len(weights)), n_repeats)
         randwgt = np.random.uniform(low=0, high=weight_scale, size=len(weights) * n_repeats)
         keep_indices = all_indices[randwgt < np.repeat(weights, n_repeats)]
-    return keep_indices.copy()
+    return copy.deepcopy(keep_indices)
 
 
 def _check_labels(table):
     if np.all(table['_labelcheck_'] == 1):
         return
     else:
         if np.any(table['_labelcheck_'] == 0):
@@ -131,15 +131,15 @@
         self.prefetch = None
         self.table = None
         self.indices = []
         self.cursor = 0
 
         self._seed = None
         worker_info = torch.utils.data.get_worker_info()
-        file_dict = self._init_file_dict.copy()
+        file_dict = copy.deepcopy(self._init_file_dict)
         if worker_info is not None:
             # in a worker process
             self._name += '_worker%d' % worker_info.id
             self._seed = worker_info.seed & 0xFFFFFFFF
             np.random.seed(self._seed)
             # split workload by files
             new_file_dict = {}
@@ -152,15 +152,15 @@
         self.worker_filelist = sum(file_dict.values(), [])
         self.worker_info = worker_info
         self.restart()
 
     def restart(self):
         print('=== Restarting DataIter %s, seed=%s ===' % (self._name, self._seed))
         # re-shuffle filelist and load range if for training
-        filelist = self.worker_filelist.copy()
+        filelist = copy.deepcopy(self.worker_filelist)
         if self._sampler_options['shuffle']:
             np.random.shuffle(filelist)
         if self._file_fraction < 1:
             num_files = int(len(filelist) * self._file_fraction)
             filelist = filelist[:num_files]
         self.filelist = filelist
 
@@ -256,19 +256,19 @@
                                                  filelist, load_range, self._sampler_options)
         else:
             self.prefetch = _load_next(self._data_config, filelist, load_range, self._sampler_options)
         self.ipos += self._fetch_step
 
     def get_data(self, i):
         # inputs
-        X = {k: self.table['_' + k][i].copy() for k in self._data_config.input_names}
+        X = {k: copy.deepcopy(self.table['_' + k][i]) for k in self._data_config.input_names}
         # labels
-        y = {k: self.table[k][i].copy() for k in self._data_config.label_names}
+        y = {k: copy.deepcopy(self.table[k][i]) for k in self._data_config.label_names}
         # observers / monitor variables
-        Z = {k: self.table[k][i].copy() for k in self._data_config.z_variables}
+        Z = {k: copy.deepcopy(self.table[k][i]) for k in self._data_config.z_variables}
         return X, y, Z
 
 
 class SimpleIterDataset(torch.utils.data.IterableDataset):
     r"""Base IterableDataset.
 
     Handles dataloading.
@@ -311,14 +311,18 @@
         # ==== sampling parameters ====
         self._sampler_options = {
             'up_sample': up_sample,
             'weight_scale': weight_scale,
             'max_resample': max_resample,
         }
 
+        # ==== torch collate_fn map ====
+        from torch.utils.data._utils.collate import default_collate_fn_map
+        default_collate_fn_map.update({ak.Array: _collate_awkward_array_fn})
+
         if for_training:
             self._sampler_options.update(training=True, shuffle=True, reweight=True)
         else:
             self._sampler_options.update(training=False, shuffle=False, reweight=False)
 
         # discover auto-generated reweight file
         if '.auto.yaml' in data_config_file:
```

### Comparing `weaver-core-0.4.8/weaver/utils/flops_counter.py` & `weaver-core-0.4.9/weaver/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.8/weaver/utils/logger.py` & `weaver-core-0.4.9/weaver/utils/logger.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.8/weaver/utils/lr_finder.py` & `weaver-core-0.4.9/weaver/utils/lr_finder.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.8/weaver/utils/nn/metrics.py` & `weaver-core-0.4.9/weaver/utils/nn/metrics.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.8/weaver/utils/nn/optimizer/lookahead.py` & `weaver-core-0.4.9/weaver/utils/nn/optimizer/lookahead.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.8/weaver/utils/nn/optimizer/radam.py` & `weaver-core-0.4.9/weaver/utils/nn/optimizer/radam.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.8/weaver/utils/nn/tools.py` & `weaver-core-0.4.9/weaver/utils/nn/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,20 +55,22 @@
 
     data_config = train_loader.dataset.config
 
     label_counter = Counter()
     total_loss = 0
     num_batches = 0
     total_correct = 0
+    entry_count = 0
     count = 0
     start_time = time.time()
     with tqdm.tqdm(train_loader) as tq:
         for X, y, _ in tq:
             inputs = [X[k].to(dev) for k in data_config.input_names]
             label = y[data_config.label_names[0]].long().to(dev)
+            entry_count += label.shape[0]
             try:
                 mask = y[data_config.label_names[0] + '_mask'].bool().to(dev)
             except KeyError:
                 mask = None
             opt.zero_grad()
             with torch.cuda.amp.autocast(enabled=grad_scaler is not None):
                 model_output = model(*inputs)
@@ -113,15 +115,15 @@
                         tb_helper.custom_fn(model_output=model_output, model=model,
                                             epoch=epoch, i_batch=num_batches, mode='train')
 
             if steps_per_epoch is not None and num_batches >= steps_per_epoch:
                 break
 
     time_diff = time.time() - start_time
-    _logger.info('Processed %d entries in total (avg. speed %.1f entries/s)' % (count, count / time_diff))
+    _logger.info('Processed %d entries in total (avg. speed %.1f entries/s)' % (entry_count, entry_count / time_diff))
     _logger.info('Train AvgLoss: %.5f, AvgAcc: %.5f' % (total_loss / num_batches, total_correct / count))
     _logger.info('Train class distribution: \n    %s', str(sorted(label_counter.items())))
 
     if tb_helper:
         tb_helper.write_scalars([
             ("Loss/train (epoch)", total_loss / num_batches, epoch),
             ("Acc/train (epoch)", total_correct / count, epoch),
@@ -153,14 +155,15 @@
     labels = defaultdict(list)
     labels_counts = []
     observers = defaultdict(list)
     start_time = time.time()
     with torch.no_grad():
         with tqdm.tqdm(test_loader) as tq:
             for X, y, Z in tq:
+                # X, y: torch.Tensor; Z: ak.Array
                 inputs = [X[k].to(dev) for k in data_config.input_names]
                 label = y[data_config.label_names[0]].long().to(dev)
                 entry_count += label.shape[0]
                 try:
                     mask = y[data_config.label_names[0] + '_mask'].bool().to(dev)
                 except KeyError:
                     mask = None
@@ -170,15 +173,15 @@
 
                 if mask is not None:
                     mask = mask.cpu()
                 for k, v in y.items():
                     labels[k].append(_flatten_label(v, mask).numpy(force=True))
                 if not for_training:
                     for k, v in Z.items():
-                        observers[k].append(v.numpy(force=True))
+                        observers[k].append(v)
 
                 num_examples = label.shape[0]
                 label_counter.update(label.numpy(force=True))
                 if not for_training and mask is not None:
                     labels_counts.append(np.squeeze(mask.numpy(force=True).sum(axis=-1)))
 
                 _, preds = logits.max(1)
@@ -202,15 +205,15 @@
                             tb_helper.custom_fn(model_output=model_output, model=model, epoch=epoch,
                                                 i_batch=num_batches, mode='eval' if for_training else 'test')
 
                 if steps_per_epoch is not None and num_batches >= steps_per_epoch:
                     break
 
     time_diff = time.time() - start_time
-    _logger.info('Processed %d entries in total (avg. speed %.1f entries/s)' % (count, count / time_diff))
+    _logger.info('Processed %d entries in total (avg. speed %.1f entries/s)' % (entry_count, entry_count / time_diff))
     _logger.info('Evaluation class distribution: \n    %s', str(sorted(label_counter.items())))
 
     if tb_helper:
         tb_mode = 'eval' if for_training else 'test'
         tb_helper.write_scalars([
             ("Loss/%s (epoch)" % tb_mode, total_loss / count, epoch),
             ("Acc/%s (epoch)" % tb_mode, total_correct / count, epoch),
@@ -255,26 +258,27 @@
     count = 0
     scores = []
     labels = defaultdict(list)
     observers = defaultdict(list)
     start_time = time.time()
     with tqdm.tqdm(test_loader) as tq:
         for X, y, Z in tq:
-            inputs = {k: v.cpu().numpy() for k, v in X.items()}
-            label = y[data_config.label_names[0]].cpu().numpy()
+            # X, y: torch.Tensor; Z: ak.Array
+            inputs = {k: v.numpy(force=True) for k, v in X.items()}
+            label = y[data_config.label_names[0]].numpy(force=True)
             num_examples = label.shape[0]
             label_counter.update(label)
             score = sess.run([], inputs)[0]
             preds = score.argmax(1)
 
             scores.append(score)
             for k, v in y.items():
-                labels[k].append(v.cpu().numpy())
+                labels[k].append(v.numpy(force=True))
             for k, v in Z.items():
-                observers[k].append(v.cpu().numpy())
+                observers[k].append(v)
 
             correct = (preds == label).sum()
             total_correct += correct
             count += num_examples
 
             tq.set_postfix({
                 'Acc': '%.5f' % (correct / num_examples),
@@ -400,27 +404,28 @@
     scores = []
     labels = defaultdict(list)
     observers = defaultdict(list)
     start_time = time.time()
     with torch.no_grad():
         with tqdm.tqdm(test_loader) as tq:
             for X, y, Z in tq:
+                # X, y: torch.Tensor; Z: ak.Array
                 inputs = [X[k].to(dev) for k in data_config.input_names]
                 label = y[data_config.label_names[0]].float()
                 num_examples = label.shape[0]
                 label = label.to(dev)
                 model_output = model(*inputs)
                 preds = model_output.squeeze().float()
 
-                scores.append(preds.detach().cpu().numpy())
+                scores.append(preds.numpy(force=True))
                 for k, v in y.items():
-                    labels[k].append(v.cpu().numpy())
+                    labels[k].append(v.numpy(force=True))
                 if not for_training:
                     for k, v in Z.items():
-                        observers[k].append(v.cpu().numpy())
+                        observers[k].append(v)
 
                 loss = 0 if loss_func is None else loss_func(preds, label).item()
 
                 num_batches += 1
                 count += num_examples
                 total_loss += loss * num_examples
                 e = preds - label
```

### Comparing `weaver-core-0.4.8/weaver_core.egg-info/PKG-INFO` & `weaver-core-0.4.9/weaver_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weaver-core
-Version: 0.4.8
+Version: 0.4.9
 Summary: A streamlined deep-learning framework for high energy physics
 Home-page: https://github.com/hqucms/weaver-core
 Author: H. Qu, C. Li
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `weaver-core-0.4.8/weaver_core.egg-info/SOURCES.txt` & `weaver-core-0.4.9/weaver_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

