# Comparing `tmp/falcon_challenge-0.3.3.tar.gz` & `tmp/falcon_challenge-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falcon_challenge-0.3.3.tar", last modified: Thu May  2 23:45:22 2024, max compression
+gzip compressed data, was "falcon_challenge-0.3.4.tar", last modified: Tue May  7 02:38:06 2024, max compression
```

## Comparing `falcon_challenge-0.3.3.tar` & `falcon_challenge-0.3.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:45:22.188435 falcon_challenge-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-02 23:45:22.188435 falcon_challenge-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:45:22.184435 falcon_challenge-0.3.3/decoder_demos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/decoder_demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/decoder_demos/decoding_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/decoder_demos/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/decoder_demos/ndt2_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/decoder_demos/random_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/decoder_demos/rnn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    13694 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/decoder_demos/sklearn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/decoder_demos/sklearn_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:45:22.184435 falcon_challenge-0.3.3/falcon_challenge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/falcon_challenge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/falcon_challenge/challenge_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/falcon_challenge/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8212 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/falcon_challenge/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    26489 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/falcon_challenge/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/falcon_challenge/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:45:22.188435 falcon_challenge-0.3.3/falcon_challenge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-02 23:45:22.000000 falcon_challenge-0.3.3/falcon_challenge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-02 23:45:22.000000 falcon_challenge-0.3.3/falcon_challenge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 23:45:22.000000 falcon_challenge-0.3.3/falcon_challenge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-02 23:45:22.000000 falcon_challenge-0.3.3/falcon_challenge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 23:45:22.000000 falcon_challenge-0.3.3/falcon_challenge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:45:22.188435 falcon_challenge-0.3.3/preproc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/preproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/preproc/assemble_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/preproc/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/preproc/h2_preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/preproc/m1_fewshot_trial_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)    24166 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/preproc/m1_reachgrasp_preprocv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/preproc/m2_fewshot_trial_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)    16660 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/preproc/m2_preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/preproc/merge_answers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/preproc/nwb_create_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/preproc/wrapper_convert_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/preproc/zip_data.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 23:45:22.188435 falcon_challenge-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:38:06.886031 falcon_challenge-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-07 02:38:06.886031 falcon_challenge-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:38:06.882031 falcon_challenge-0.3.4/decoder_demos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/decoder_demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/decoder_demos/decoding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/decoder_demos/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/decoder_demos/ndt2_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/decoder_demos/random_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/decoder_demos/rnn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13694 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/decoder_demos/sklearn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/decoder_demos/sklearn_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:38:06.886031 falcon_challenge-0.3.4/falcon_challenge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/falcon_challenge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/falcon_challenge/challenge_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/falcon_challenge/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8212 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/falcon_challenge/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26588 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/falcon_challenge/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/falcon_challenge/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:38:06.886031 falcon_challenge-0.3.4/falcon_challenge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-07 02:38:06.000000 falcon_challenge-0.3.4/falcon_challenge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-07 02:38:06.000000 falcon_challenge-0.3.4/falcon_challenge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 02:38:06.000000 falcon_challenge-0.3.4/falcon_challenge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-07 02:38:06.000000 falcon_challenge-0.3.4/falcon_challenge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 02:38:06.000000 falcon_challenge-0.3.4/falcon_challenge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:38:06.886031 falcon_challenge-0.3.4/preproc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/preproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/preproc/assemble_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/preproc/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/preproc/h2_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/preproc/m1_fewshot_trial_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24166 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/preproc/m1_reachgrasp_preprocv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/preproc/m2_fewshot_trial_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16660 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/preproc/m2_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/preproc/merge_answers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/preproc/nwb_create_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/preproc/wrapper_convert_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/preproc/zip_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 02:38:06.890031 falcon_challenge-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/setup.py
```

### Comparing `falcon_challenge-0.3.3/LICENSE` & `falcon_challenge-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.3/PKG-INFO` & `falcon_challenge-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon_challenge
-Version: 0.3.3
+Version: 0.3.4
 Home-page: https://github.com/snel-repo/stability-benchmark
 Author: Joel Ye
 Author-email: joelye9@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: hydra-core
```

### Comparing `falcon_challenge-0.3.3/README.md` & `falcon_challenge-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.3/decoder_demos/decoding_utils.py` & `falcon_challenge-0.3.4/decoder_demos/decoding_utils.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.3/decoder_demos/filtering.py` & `falcon_challenge-0.3.4/decoder_demos/filtering.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.3/decoder_demos/ndt2_sample.py` & `falcon_challenge-0.3.4/decoder_demos/ndt2_sample.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,19 +33,25 @@
     )
     parser.add_argument(
         '--phase', choices=['minival', 'test'], default='minival'
     )
     parser.add_argument(
         '--batch-size', type=int, default=1
     )
+    parser.add_argument(
+        '--continual', action='store_true', default=False
+    )
+    
     args = parser.parse_args()
 
     evaluator = FalconEvaluator(
         eval_remote=args.evaluation == "remote",
-        split=args.split)
+        split=args.split,
+        continual=args.continual
+    )
 
     task = getattr(FalconTask, args.split)
     config = FalconConfig(task=task)
 
     decoder = NDT2Decoder(
         task_config=config,
         model_ckpt_path=args.model_path,
```

### Comparing `falcon_challenge-0.3.3/decoder_demos/random_decoder.py` & `falcon_challenge-0.3.4/decoder_demos/random_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.3/decoder_demos/rnn_decoder.py` & `falcon_challenge-0.3.4/decoder_demos/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.3/decoder_demos/sklearn_decoder.py` & `falcon_challenge-0.3.4/decoder_demos/sklearn_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.3/decoder_demos/sklearn_sample.py` & `falcon_challenge-0.3.4/decoder_demos/sklearn_sample.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.3/falcon_challenge/config.py` & `falcon_challenge-0.3.4/falcon_challenge/config.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.3/falcon_challenge/dataloaders.py` & `falcon_challenge-0.3.4/falcon_challenge/dataloaders.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.3/falcon_challenge/evaluator.py` & `falcon_challenge-0.3.4/falcon_challenge/evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,17 +273,18 @@
     trial_change = pad_sequence([torch.tensor(t) for t in trial_change], batch_first=False).numpy()
     eval_mask = pad_sequence([torch.tensor(t) for t in eval_mask], batch_first=False).numpy() # Serves as a mask for padding as well
     datafile_idx = np.array(datafile_idx)
     return data, targets, trial_change, eval_mask, datafile_idx
 
 class FalconEvaluator:
 
-    def __init__(self, eval_remote=False, split='h1'):
+    def __init__(self, eval_remote=False, split='h1', continual=False):
         self.eval_remote = eval_remote
         assert split in ['h1', 'h2', 'm1', 'm2'], "Split must be h1, h2, m1, or m2."
+        self.continual = continual
         self.dataset: FalconTask = getattr(FalconTask, split)
         self.cfg = FalconConfig(self.dataset)
 
     @staticmethod
     def get_eval_handles(is_remote: bool, dataset: FalconTask, phase: str = 'minival'):
         if is_remote: # i.e. definitely docker
             data_dir = os.environ.get("EVAL_DATA_PATH")
@@ -370,15 +371,16 @@
                 if self.dataset == FalconTask.h2:
                     assert neural_data.shape[1] == 1, "H2 expects batch size 1."
                     if step_mask[0]:
                         decoder.predict(neural_observations)
                     if trial_delta_obs[0]:
                         trial_preds.append(decoder.on_done(trial_delta_obs))
                 else:
-                    decoder.on_done(trial_delta_obs)
+                    if not self.continual:
+                        decoder.on_done(trial_delta_obs)
                     step_prediction = decoder.predict(neural_observations)
                     assert step_prediction.shape[1] == self.cfg.out_dim, f"Prediction shape mismatch: {step_prediction.shape[1]} vs {self.cfg.out_dim}."
                     trial_preds.append(step_prediction)
                     
                     # if step_mask.any():
                     #     trial_preds.append(decoder.predict(neural_observations))
                     # else:
```

### Comparing `falcon_challenge-0.3.3/falcon_challenge/interface.py` & `falcon_challenge-0.3.4/falcon_challenge/interface.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.3/falcon_challenge.egg-info/PKG-INFO` & `falcon_challenge-0.3.4/falcon_challenge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon_challenge
-Version: 0.3.3
+Version: 0.3.4
 Home-page: https://github.com/snel-repo/stability-benchmark
 Author: Joel Ye
 Author-email: joelye9@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: hydra-core
```

### Comparing `falcon_challenge-0.3.3/falcon_challenge.egg-info/SOURCES.txt` & `falcon_challenge-0.3.4/falcon_challenge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.3/preproc/assemble_data.py` & `falcon_challenge-0.3.4/preproc/assemble_data.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.3/preproc/filtering.py` & `falcon_challenge-0.3.4/preproc/filtering.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.3/preproc/h2_preproc.py` & `falcon_challenge-0.3.4/preproc/h2_preproc.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.3/preproc/m1_fewshot_trial_counts.py` & `falcon_challenge-0.3.4/preproc/m1_fewshot_trial_counts.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.3/preproc/m1_reachgrasp_preprocv2.py` & `falcon_challenge-0.3.4/preproc/m1_reachgrasp_preprocv2.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.3/preproc/m2_fewshot_trial_counts.py` & `falcon_challenge-0.3.4/preproc/m2_fewshot_trial_counts.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.3/preproc/m2_preproc.py` & `falcon_challenge-0.3.4/preproc/m2_preproc.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.3/preproc/merge_answers.py` & `falcon_challenge-0.3.4/preproc/merge_answers.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.3/preproc/nwb_create_utils.py` & `falcon_challenge-0.3.4/preproc/nwb_create_utils.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.3/preproc/wrapper_convert_batch.py` & `falcon_challenge-0.3.4/preproc/wrapper_convert_batch.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.3/preproc/zip_data.py` & `falcon_challenge-0.3.4/preproc/zip_data.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.3/setup.py` & `falcon_challenge-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='falcon_challenge',
-    version='0.3.3',
+    version='0.3.4',
 
     url='https://github.com/snel-repo/stability-benchmark',
     author='Joel Ye',
     author_email='joelye9@gmail.com',
 
     packages=find_packages(exclude=['data_demos', 'data']),
     install_requires=[
```

