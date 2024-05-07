# Comparing `tmp/sae_lens-1.5.0.tar.gz` & `tmp/sae_lens-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sae_lens-1.5.0.tar", max compression
+gzip compressed data, was "sae_lens-1.6.0.tar", max compression
```

## Comparing `sae_lens-1.5.0.tar` & `sae_lens-1.6.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1069 2024-05-07 12:00:14.107136 sae_lens-1.5.0/LICENSE
--rw-r--r--   0        0        0     2553 2024-05-07 12:00:14.107136 sae_lens-1.5.0/README.md
--rw-r--r--   0        0        0     1917 2024-05-07 12:00:15.451135 sae_lens-1.5.0/pyproject.toml
--rw-r--r--   0        0        0      939 2024-05-07 12:00:15.451135 sae_lens-1.5.0/sae_lens/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/analysis/__init__.py
--rw-r--r--   0        0        0    15645 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/analysis/dashboard_runner.py
--rw-r--r--   0        0        0     3535 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/analysis/feature_statistics.py
--rw-r--r--   0        0        0    17062 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/analysis/neuronpedia_integration.py
--rw-r--r--   0        0        0    20134 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/analysis/neuronpedia_runner.py
--rw-r--r--   0        0        0    18275 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/analysis/tsea.py
--rw-r--r--   0        0        0     1164 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/pretrained_saes.yaml
--rw-r--r--   0        0        0        0 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/toolkit/__init__.py
--rw-r--r--   0        0        0     2674 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/toolkit/pretrained_sae_loaders.py
--rw-r--r--   0        0        0     6643 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/toolkit/pretrained_saes.py
--rw-r--r--   0        0        0     1143 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/toolkit/pretrained_saes_directory.py
--rw-r--r--   0        0        0        0 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/__init__.py
--rw-r--r--   0        0        0      471 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/activation_functions.py
--rw-r--r--   0        0        0    20435 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/activations_store.py
--rw-r--r--   0        0        0     5974 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/cache_activations_runner.py
--rw-r--r--   0        0        0    12899 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/config.py
--rw-r--r--   0        0        0     7439 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/evals.py
--rw-r--r--   0        0        0     3747 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/geometric_median.py
--rw-r--r--   0        0        0     3069 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/lm_runner.py
--rw-r--r--   0        0        0     1020 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/load_model.py
--rw-r--r--   0        0        0     5065 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/optim.py
--rw-r--r--   0        0        0     8284 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/sae_group.py
--rw-r--r--   0        0        0     2319 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/session_loader.py
--rw-r--r--   0        0        0    20000 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/sparse_autoencoder.py
--rw-r--r--   0        0        0     3276 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/toy_model_runner.py
--rw-r--r--   0        0        0    17362 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/toy_models.py
--rw-r--r--   0        0        0    29388 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/train_sae_on_language_model.py
--rw-r--r--   0        0        0     5002 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/train_sae_on_toy_model.py
--rw-r--r--   0        0        0      423 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/utils.py
--rw-r--r--   0        0        0     4196 1970-01-01 00:00:00.000000 sae_lens-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-07 14:11:44.743109 sae_lens-1.6.0/LICENSE
+-rw-r--r--   0        0        0     2553 2024-05-07 14:11:44.743109 sae_lens-1.6.0/README.md
+-rw-r--r--   0        0        0     1917 2024-05-07 14:11:46.079116 sae_lens-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0      939 2024-05-07 14:11:46.079116 sae_lens-1.6.0/sae_lens/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/analysis/__init__.py
+-rw-r--r--   0        0        0    15645 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/analysis/dashboard_runner.py
+-rw-r--r--   0        0        0     3535 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/analysis/feature_statistics.py
+-rw-r--r--   0        0        0    17062 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/analysis/neuronpedia_integration.py
+-rw-r--r--   0        0        0    20134 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/analysis/neuronpedia_runner.py
+-rw-r--r--   0        0        0    18275 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/analysis/tsea.py
+-rw-r--r--   0        0        0     1164 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/pretrained_saes.yaml
+-rw-r--r--   0        0        0        0 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/toolkit/__init__.py
+-rw-r--r--   0        0        0     2674 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/toolkit/pretrained_sae_loaders.py
+-rw-r--r--   0        0        0     6643 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/toolkit/pretrained_saes.py
+-rw-r--r--   0        0        0     1143 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/toolkit/pretrained_saes_directory.py
+-rw-r--r--   0        0        0        0 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/__init__.py
+-rw-r--r--   0        0        0      471 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/activation_functions.py
+-rw-r--r--   0        0        0    20435 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/activations_store.py
+-rw-r--r--   0        0        0     5974 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/cache_activations_runner.py
+-rw-r--r--   0        0        0    12972 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/config.py
+-rw-r--r--   0        0        0     7439 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/evals.py
+-rw-r--r--   0        0        0     3747 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/geometric_median.py
+-rw-r--r--   0        0        0     3100 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/lm_runner.py
+-rw-r--r--   0        0        0     1020 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/load_model.py
+-rw-r--r--   0        0        0     5065 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/optim.py
+-rw-r--r--   0        0        0     8284 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/sae_group.py
+-rw-r--r--   0        0        0     2319 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/session_loader.py
+-rw-r--r--   0        0        0    20000 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/sparse_autoencoder.py
+-rw-r--r--   0        0        0     3276 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/toy_model_runner.py
+-rw-r--r--   0        0        0    17362 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/toy_models.py
+-rw-r--r--   0        0        0    30305 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/train_sae_on_language_model.py
+-rw-r--r--   0        0        0     5002 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/train_sae_on_toy_model.py
+-rw-r--r--   0        0        0      423 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/utils.py
+-rw-r--r--   0        0        0     4196 1970-01-01 00:00:00.000000 sae_lens-1.6.0/PKG-INFO
```

### Comparing `sae_lens-1.5.0/LICENSE` & `sae_lens-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sae_lens-1.5.0/README.md` & `sae_lens-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `sae_lens-1.5.0/pyproject.toml` & `sae_lens-1.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sae-lens"
-version = "1.5.0"
+version = "1.6.0"
 description = "Training and Analyzing Sparse Autoencoders (SAEs)"
 authors = ["Joseph Bloom"]
 readme = "README.md"
 packages = [{include = "sae_lens"}]
 include = ["pretrained_saes.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `sae_lens-1.5.0/sae_lens/__init__.py` & `sae_lens-1.6.0/sae_lens/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.5.0"
+__version__ = "1.6.0"
 
 from .training.activations_store import ActivationsStore
 from .training.cache_activations_runner import CacheActivationsRunner
 from .training.config import CacheActivationsRunnerConfig, LanguageModelSAERunnerConfig
 from .training.evals import run_evals
 from .training.lm_runner import language_model_sae_runner
 from .training.sae_group import SparseAutoencoderDictionary
```

### Comparing `sae_lens-1.5.0/sae_lens/analysis/dashboard_runner.py` & `sae_lens-1.6.0/sae_lens/analysis/dashboard_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.5.0/sae_lens/analysis/feature_statistics.py` & `sae_lens-1.6.0/sae_lens/analysis/feature_statistics.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.5.0/sae_lens/analysis/neuronpedia_integration.py` & `sae_lens-1.6.0/sae_lens/analysis/neuronpedia_integration.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.5.0/sae_lens/analysis/neuronpedia_runner.py` & `sae_lens-1.6.0/sae_lens/analysis/neuronpedia_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.5.0/sae_lens/analysis/tsea.py` & `sae_lens-1.6.0/sae_lens/analysis/tsea.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.5.0/sae_lens/pretrained_saes.yaml` & `sae_lens-1.6.0/sae_lens/pretrained_saes.yaml`

 * *Files identical despite different names*

### Comparing `sae_lens-1.5.0/sae_lens/toolkit/pretrained_sae_loaders.py` & `sae_lens-1.6.0/sae_lens/toolkit/pretrained_sae_loaders.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.5.0/sae_lens/toolkit/pretrained_saes.py` & `sae_lens-1.6.0/sae_lens/toolkit/pretrained_saes.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.5.0/sae_lens/toolkit/pretrained_saes_directory.py` & `sae_lens-1.6.0/sae_lens/toolkit/pretrained_saes_directory.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.5.0/sae_lens/training/activations_store.py` & `sae_lens-1.6.0/sae_lens/training/activations_store.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.5.0/sae_lens/training/cache_activations_runner.py` & `sae_lens-1.6.0/sae_lens/training/cache_activations_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.5.0/sae_lens/training/config.py` & `sae_lens-1.6.0/sae_lens/training/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     normalize_activations: bool = False
 
     # Misc
     device: str | torch.device = "cpu"
     seed: int = 42
     dtype: str | torch.dtype = "float32"  # type: ignore #
     prepend_bos: bool = True
+    autocast: bool = False  # autocast to autocast_dtype during training
 
     # Training Parameters
 
     ## Batch size
     train_batch_size: int = 4096
 
     ## Adam
```

### Comparing `sae_lens-1.5.0/sae_lens/training/evals.py` & `sae_lens-1.6.0/sae_lens/training/evals.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.5.0/sae_lens/training/geometric_median.py` & `sae_lens-1.6.0/sae_lens/training/geometric_median.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.5.0/sae_lens/training/lm_runner.py` & `sae_lens-1.6.0/sae_lens/training/lm_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,13 +80,14 @@
         training_run_state=training_run_state,
         batch_size=cfg.train_batch_size,
         n_checkpoints=cfg.n_checkpoints,
         feature_sampling_window=cfg.feature_sampling_window,
         use_wandb=cfg.log_to_wandb,
         wandb_log_frequency=cfg.wandb_log_frequency,
         eval_every_n_wandb_logs=cfg.eval_every_n_wandb_logs,
+        autocast=cfg.autocast,
     ).sae_group
 
     if cfg.log_to_wandb:
         wandb.finish()
 
     return sparse_autoencoder
```

### Comparing `sae_lens-1.5.0/sae_lens/training/load_model.py` & `sae_lens-1.6.0/sae_lens/training/load_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.5.0/sae_lens/training/optim.py` & `sae_lens-1.6.0/sae_lens/training/optim.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.5.0/sae_lens/training/sae_group.py` & `sae_lens-1.6.0/sae_lens/training/sae_group.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.5.0/sae_lens/training/session_loader.py` & `sae_lens-1.6.0/sae_lens/training/session_loader.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.5.0/sae_lens/training/sparse_autoencoder.py` & `sae_lens-1.6.0/sae_lens/training/sparse_autoencoder.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.5.0/sae_lens/training/toy_model_runner.py` & `sae_lens-1.6.0/sae_lens/training/toy_model_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.5.0/sae_lens/training/toy_models.py` & `sae_lens-1.6.0/sae_lens/training/toy_models.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.5.0/sae_lens/training/train_sae_on_language_model.py` & `sae_lens-1.6.0/sae_lens/training/train_sae_on_language_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import contextlib
 import os
 import pickle
 import random
 import signal
 from dataclasses import dataclass, field, fields
 from typing import Any, Optional, cast
 
@@ -182,28 +183,30 @@
     batch_size: int = 1024,
     n_checkpoints: int = 0,
     feature_sampling_window: int = 1000,  # how many training steps between resampling the features / considiring neurons dead
     dead_feature_threshold: float = 1e-8,  # how infrequently a feature has to be active to be considered dead
     use_wandb: bool = False,
     wandb_log_frequency: int = 50,
     eval_every_n_wandb_logs: int = 100,
+    autocast: bool = False,
 ) -> SparseAutoencoderDictionary:
     """
     @deprecated Use `train_sae_group_on_language_model` instead. This method is kept for backward compatibility.
     """
     return train_sae_group_on_language_model(
         model=model,
         sae_group=sae_group,
         activation_store=activation_store,
         batch_size=batch_size,
         n_checkpoints=n_checkpoints,
         feature_sampling_window=feature_sampling_window,
         use_wandb=use_wandb,
         wandb_log_frequency=wandb_log_frequency,
         eval_every_n_wandb_logs=eval_every_n_wandb_logs,
+        autocast=autocast,
     ).sae_group
 
 
 def get_total_training_tokens(sae_group: SparseAutoencoderDictionary) -> int:
     return sae_group.cfg.training_tokens + sae_group.cfg.finetuning_tokens
 
 
@@ -215,14 +218,15 @@
     training_run_state: Optional[SAETrainingRunState] = None,
     batch_size: int = 1024,
     n_checkpoints: int = 0,
     feature_sampling_window: int = 1000,  # how many training steps between resampling the features / considiring neurons dead
     use_wandb: bool = False,
     wandb_log_frequency: int = 50,
     eval_every_n_wandb_logs: int = 100,
+    autocast: bool = False,
 ) -> TrainSAEGroupOutput:
     total_training_tokens = get_total_training_tokens(sae_group=sae_group)
     _update_sae_lens_training_version(sae_group)
     total_training_steps = total_training_tokens // batch_size
 
     checkpoint_thresholds = []
     if n_checkpoints > 0:
@@ -285,14 +289,15 @@
                     ctx=ctx,
                     feature_sampling_window=feature_sampling_window,
                     use_wandb=use_wandb,
                     n_training_steps=training_run_state.n_training_steps,
                     all_layers=all_layers,
                     batch_size=batch_size,
                     wandb_suffix=wandb_suffix,
+                    autocast=autocast,
                 )
                 mse_losses.append(step_output.mse_loss)
                 l1_losses.append(step_output.l1_loss)
 
                 if use_wandb:
                     with torch.no_grad():
                         if (
@@ -535,14 +540,15 @@
     ctx: SAETrainContext,
     feature_sampling_window: int,  # how many training steps between resampling the features / considiring neurons dead
     use_wandb: bool,
     n_training_steps: int,
     all_layers: list[int],
     batch_size: int,
     wandb_suffix: str,
+    autocast: bool = True,
 ) -> TrainStepOutput:
     assert sparse_autoencoder.cfg.d_sae is not None  # keep pyright happy
     layer_id = all_layers.index(sparse_autoencoder.hook_point_layer)
     sae_in = layer_acts[:, layer_id, :]
 
     sparse_autoencoder.train()
     # Make sure the W_dec is still zero-norm
@@ -575,46 +581,63 @@
         )
         ctx.n_frac_active_tokens = 0
 
     ghost_grad_neuron_mask = (
         ctx.n_forward_passes_since_fired > sparse_autoencoder.cfg.dead_feature_window
     ).bool()
 
+    # Setup autocast if using
+    scaler = torch.cuda.amp.GradScaler(enabled=autocast)
+    if autocast:
+        autocast_if_enabled = torch.autocast(
+            device_type="cuda",
+            dtype=torch.bfloat16,
+            enabled=autocast,
+        )
+    else:
+        autocast_if_enabled = contextlib.nullcontext()
+
     # Forward and Backward Passes
-    (
-        sae_out,
-        feature_acts,
-        loss,
-        mse_loss,
-        l1_loss,
-        ghost_grad_loss,
-    ) = sparse_autoencoder(
-        sae_in,
-        ghost_grad_neuron_mask,
-    )
+    # for documentation on autocasting see:
+    # https://pytorch.org/tutorials/recipes/recipes/amp_recipe.html
+    with autocast_if_enabled:
+        (
+            sae_out,
+            feature_acts,
+            loss,
+            mse_loss,
+            l1_loss,
+            ghost_grad_loss,
+        ) = sparse_autoencoder(
+            sae_in,
+            ghost_grad_neuron_mask,
+        )
+
     did_fire = (feature_acts > 0).float().sum(-2) > 0
     ctx.n_forward_passes_since_fired += 1
     ctx.n_forward_passes_since_fired[did_fire] = 0
 
     with torch.no_grad():
         # Calculate the sparsities, and add it to a list, calculate sparsity metrics
         ctx.act_freq_scores += (feature_acts.abs() > 0).float().sum(0)
         ctx.n_frac_active_tokens += batch_size
 
-    ctx.optimizer.zero_grad()
-    loss.backward()
-
-    # clip grad norm
-    # TODO: Work out if this should be in config / how to test it.
+    # Scaler will rescale gradients if autocast is enabled
+    scaler.scale(loss).backward()  # loss.backward() if not autocasting
+    scaler.unscale_(ctx.optimizer)  # needed to clip correctly
+    # TODO: Work out if grad norm clipping should be in config / how to test it.
     torch.nn.utils.clip_grad_norm_(sparse_autoencoder.parameters(), 1.0)
+    scaler.step(ctx.optimizer)  # just ctx.optimizer.step() if not autocasting
+    scaler.update()
 
     if sparse_autoencoder.normalize_sae_decoder:
         sparse_autoencoder.remove_gradient_parallel_to_decoder_directions()
 
-    ctx.optimizer.step()
+    ctx.optimizer.zero_grad()
+
     ctx.lr_scheduler.step()
     ctx.l1_scheduler.step()
 
     return TrainStepOutput(
         sae_in=sae_in,
         sae_out=sae_out,
         feature_acts=feature_acts,
```

### Comparing `sae_lens-1.5.0/sae_lens/training/train_sae_on_toy_model.py` & `sae_lens-1.6.0/sae_lens/training/train_sae_on_toy_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.5.0/PKG-INFO` & `sae_lens-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sae-lens
-Version: 1.5.0
+Version: 1.6.0
 Summary: Training and Analyzing Sparse Autoencoders (SAEs)
 Author: Joseph Bloom
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

