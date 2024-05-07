# Comparing `tmp/sae_lens-1.4.0.tar.gz` & `tmp/sae_lens-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sae_lens-1.4.0.tar", max compression
+gzip compressed data, was "sae_lens-1.5.0.tar", max compression
```

## Comparing `sae_lens-1.4.0.tar` & `sae_lens-1.5.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1069 2024-05-05 00:47:08.104824 sae_lens-1.4.0/LICENSE
--rw-r--r--   0        0        0     2553 2024-05-05 00:47:08.104824 sae_lens-1.4.0/README.md
--rw-r--r--   0        0        0     1889 2024-05-05 00:47:09.224817 sae_lens-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      943 2024-05-05 00:47:09.224817 sae_lens-1.4.0/sae_lens/__init__.py
--rw-r--r--   0        0        0        0 2024-05-05 00:47:08.112824 sae_lens-1.4.0/sae_lens/analysis/__init__.py
--rw-r--r--   0        0        0    15645 2024-05-05 00:47:08.112824 sae_lens-1.4.0/sae_lens/analysis/dashboard_runner.py
--rw-r--r--   0        0        0     3535 2024-05-05 00:47:08.112824 sae_lens-1.4.0/sae_lens/analysis/feature_statistics.py
--rw-r--r--   0        0        0    17062 2024-05-05 00:47:08.112824 sae_lens-1.4.0/sae_lens/analysis/neuronpedia_integration.py
--rw-r--r--   0        0        0    20134 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/analysis/neuronpedia_runner.py
--rw-r--r--   0        0        0    18275 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/analysis/tsea.py
--rw-r--r--   0        0        0     1164 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/pretrained_saes.yaml
--rw-r--r--   0        0        0        0 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/toolkit/__init__.py
--rw-r--r--   0        0        0     2674 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/toolkit/pretrained_sae_loaders.py
--rw-r--r--   0        0        0     6643 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/toolkit/pretrained_saes.py
--rw-r--r--   0        0        0     1143 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/toolkit/pretrained_saes_directory.py
--rw-r--r--   0        0        0        0 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/__init__.py
--rw-r--r--   0        0        0      471 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/activation_functions.py
--rw-r--r--   0        0        0    18342 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/activations_store.py
--rw-r--r--   0        0        0     2849 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/cache_activations_runner.py
--rw-r--r--   0        0        0    12089 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/config.py
--rw-r--r--   0        0        0     6169 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/evals.py
--rw-r--r--   0        0        0     3747 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/geometric_median.py
--rw-r--r--   0        0        0     3008 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/lm_runner.py
--rw-r--r--   0        0        0     1020 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/load_model.py
--rw-r--r--   0        0        0     3675 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/optim.py
--rw-r--r--   0        0        0     8284 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/sae_group.py
--rw-r--r--   0        0        0     2319 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/session_loader.py
--rw-r--r--   0        0        0    17503 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/sparse_autoencoder.py
--rw-r--r--   0        0        0     3276 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/toy_model_runner.py
--rw-r--r--   0        0        0    17362 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/toy_models.py
--rw-r--r--   0        0        0    28498 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/train_sae_on_language_model.py
--rw-r--r--   0        0        0     5002 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/train_sae_on_toy_model.py
--rw-r--r--   0        0        0     1628 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/utils.py
--rw-r--r--   0        0        0     4147 1970-01-01 00:00:00.000000 sae_lens-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-07 12:00:14.107136 sae_lens-1.5.0/LICENSE
+-rw-r--r--   0        0        0     2553 2024-05-07 12:00:14.107136 sae_lens-1.5.0/README.md
+-rw-r--r--   0        0        0     1917 2024-05-07 12:00:15.451135 sae_lens-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      939 2024-05-07 12:00:15.451135 sae_lens-1.5.0/sae_lens/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/analysis/__init__.py
+-rw-r--r--   0        0        0    15645 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/analysis/dashboard_runner.py
+-rw-r--r--   0        0        0     3535 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/analysis/feature_statistics.py
+-rw-r--r--   0        0        0    17062 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/analysis/neuronpedia_integration.py
+-rw-r--r--   0        0        0    20134 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/analysis/neuronpedia_runner.py
+-rw-r--r--   0        0        0    18275 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/analysis/tsea.py
+-rw-r--r--   0        0        0     1164 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/pretrained_saes.yaml
+-rw-r--r--   0        0        0        0 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/toolkit/__init__.py
+-rw-r--r--   0        0        0     2674 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/toolkit/pretrained_sae_loaders.py
+-rw-r--r--   0        0        0     6643 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/toolkit/pretrained_saes.py
+-rw-r--r--   0        0        0     1143 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/toolkit/pretrained_saes_directory.py
+-rw-r--r--   0        0        0        0 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/__init__.py
+-rw-r--r--   0        0        0      471 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/activation_functions.py
+-rw-r--r--   0        0        0    20435 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/activations_store.py
+-rw-r--r--   0        0        0     5974 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/cache_activations_runner.py
+-rw-r--r--   0        0        0    12899 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/config.py
+-rw-r--r--   0        0        0     7439 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/evals.py
+-rw-r--r--   0        0        0     3747 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/geometric_median.py
+-rw-r--r--   0        0        0     3069 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/lm_runner.py
+-rw-r--r--   0        0        0     1020 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/load_model.py
+-rw-r--r--   0        0        0     5065 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/optim.py
+-rw-r--r--   0        0        0     8284 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/sae_group.py
+-rw-r--r--   0        0        0     2319 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/session_loader.py
+-rw-r--r--   0        0        0    20000 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/sparse_autoencoder.py
+-rw-r--r--   0        0        0     3276 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/toy_model_runner.py
+-rw-r--r--   0        0        0    17362 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/toy_models.py
+-rw-r--r--   0        0        0    29388 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/train_sae_on_language_model.py
+-rw-r--r--   0        0        0     5002 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/train_sae_on_toy_model.py
+-rw-r--r--   0        0        0      423 2024-05-07 12:00:14.119136 sae_lens-1.5.0/sae_lens/training/utils.py
+-rw-r--r--   0        0        0     4196 1970-01-01 00:00:00.000000 sae_lens-1.5.0/PKG-INFO
```

### Comparing `sae_lens-1.4.0/LICENSE` & `sae_lens-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sae_lens-1.4.0/README.md` & `sae_lens-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `sae_lens-1.4.0/pyproject.toml` & `sae_lens-1.5.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sae-lens"
-version = "1.4.0"
+version = "1.5.0"
 description = "Training and Analyzing Sparse Autoencoders (SAEs)"
 authors = ["Joseph Bloom"]
 readme = "README.md"
 packages = [{include = "sae_lens"}]
 include = ["pretrained_saes.yaml"]
 
 [tool.poetry.dependencies]
@@ -31,14 +31,15 @@
 safetensors = "^0.4.2"
 typer = "^0.12.3"
 mamba-lens = { version = "^0.0.4", optional = true }
 pyzmq = "26.0.0"
 automated-interpretability = "^0.0.3"
 python-dotenv = "^1.0.1"
 pyyaml = "^6.0.1"
+pytest-profiling = "^1.7.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "24.4.0"
 pytest = "^8.0.2"
 pytest-cov = "^4.1.0"
 pre-commit = "^3.6.2"
```

### Comparing `sae_lens-1.4.0/sae_lens/__init__.py` & `sae_lens-1.5.0/sae_lens/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-__version__ = "1.4.0"
+__version__ = "1.5.0"
 
 from .training.activations_store import ActivationsStore
-from .training.cache_activations_runner import cache_activations_runner
+from .training.cache_activations_runner import CacheActivationsRunner
 from .training.config import CacheActivationsRunnerConfig, LanguageModelSAERunnerConfig
 from .training.evals import run_evals
 from .training.lm_runner import language_model_sae_runner
 from .training.sae_group import SparseAutoencoderDictionary
 from .training.session_loader import LMSparseAutoencoderSessionloader
 from .training.sparse_autoencoder import SparseAutoencoder
 from .training.train_sae_on_language_model import train_sae_group_on_language_model
@@ -14,11 +14,11 @@
     "LanguageModelSAERunnerConfig",
     "CacheActivationsRunnerConfig",
     "LMSparseAutoencoderSessionloader",
     "SparseAutoencoder",
     "SparseAutoencoderDictionary",
     "run_evals",
     "language_model_sae_runner",
-    "cache_activations_runner",
+    "CacheActivationsRunner",
     "ActivationsStore",
     "train_sae_group_on_language_model",
 ]
```

### Comparing `sae_lens-1.4.0/sae_lens/analysis/dashboard_runner.py` & `sae_lens-1.5.0/sae_lens/analysis/dashboard_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.4.0/sae_lens/analysis/feature_statistics.py` & `sae_lens-1.5.0/sae_lens/analysis/feature_statistics.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.4.0/sae_lens/analysis/neuronpedia_integration.py` & `sae_lens-1.5.0/sae_lens/analysis/neuronpedia_integration.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.4.0/sae_lens/analysis/neuronpedia_runner.py` & `sae_lens-1.5.0/sae_lens/analysis/neuronpedia_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.4.0/sae_lens/analysis/tsea.py` & `sae_lens-1.5.0/sae_lens/analysis/tsea.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.4.0/sae_lens/pretrained_saes.yaml` & `sae_lens-1.5.0/sae_lens/pretrained_saes.yaml`

 * *Files identical despite different names*

### Comparing `sae_lens-1.4.0/sae_lens/toolkit/pretrained_sae_loaders.py` & `sae_lens-1.5.0/sae_lens/toolkit/pretrained_sae_loaders.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.4.0/sae_lens/toolkit/pretrained_saes.py` & `sae_lens-1.5.0/sae_lens/toolkit/pretrained_saes.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.4.0/sae_lens/toolkit/pretrained_saes_directory.py` & `sae_lens-1.5.0/sae_lens/toolkit/pretrained_saes_directory.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.4.0/sae_lens/training/activations_store.py` & `sae_lens-1.5.0/sae_lens/training/activations_store.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from datasets import (
     Dataset,
     DatasetDict,
     IterableDataset,
     IterableDatasetDict,
     load_dataset,
 )
+from safetensors import safe_open
 from safetensors.torch import load_file, save_file
 from torch.utils.data import DataLoader
 from transformer_lens.hook_points import HookedRootModule
 
 from sae_lens.training.config import (
     CacheActivationsRunnerConfig,
     LanguageModelSAERunnerConfig,
@@ -51,68 +52,73 @@
             isinstance(cfg, LanguageModelSAERunnerConfig)
             and not cfg.use_cached_activations
         ):
             cached_activations_path = None
         return cls(
             model=model,
             dataset=dataset or cfg.dataset_path,
+            streaming=cfg.streaming,
             hook_point=cfg.hook_point,
             hook_point_layers=listify(cfg.hook_point_layer),
             hook_point_head_index=cfg.hook_point_head_index,
             context_size=cfg.context_size,
             d_in=cfg.d_in,
             n_batches_in_buffer=cfg.n_batches_in_buffer,
             total_training_tokens=cfg.training_tokens,
             store_batch_size=cfg.store_batch_size,
             train_batch_size=cfg.train_batch_size,
             prepend_bos=cfg.prepend_bos,
+            normalize_activations=cfg.normalize_activations,
             device=cfg.device,
             dtype=cfg.dtype,
             cached_activations_path=cached_activations_path,
             model_kwargs=cfg.model_kwargs,
         )
 
     def __init__(
         self,
         model: HookedRootModule,
         dataset: HfDataset | str,
+        streaming: bool,
         hook_point: str,
         hook_point_layers: list[int],
         hook_point_head_index: int | None,
         context_size: int,
         d_in: int,
         n_batches_in_buffer: int,
         total_training_tokens: int,
         store_batch_size: int,
         train_batch_size: int,
         prepend_bos: bool,
+        normalize_activations: bool,
         device: str | torch.device,
         dtype: str | torch.dtype,
         cached_activations_path: str | None = None,
         model_kwargs: dict[str, Any] | None = None,
     ):
         self.model = model
         if model_kwargs is None:
             model_kwargs = {}
         self.model_kwargs = model_kwargs
         self.dataset = (
-            load_dataset(dataset, split="train", streaming=True)
+            load_dataset(dataset, split="train", streaming=streaming)
             if isinstance(dataset, str)
             else dataset
         )
         self.hook_point = hook_point
         self.hook_point_layers = hook_point_layers
         self.hook_point_head_index = hook_point_head_index
         self.context_size = context_size
         self.d_in = d_in
         self.n_batches_in_buffer = n_batches_in_buffer
         self.total_training_tokens = total_training_tokens
         self.store_batch_size = store_batch_size
         self.train_batch_size = train_batch_size
         self.prepend_bos = prepend_bos
+        self.normalize_activations = normalize_activations
         self.device = device
         self.dtype = dtype
         self.cached_activations_path = cached_activations_path
 
         self.n_dataset_processed = 0
         self.iterable_dataset = iter(self.dataset)
 
@@ -131,41 +137,56 @@
             self.tokens_column = "text"
         else:
             raise ValueError(
                 "Dataset must have a 'tokens', 'input_ids', or 'text' column."
             )
         self.iterable_dataset = iter(self.dataset)  # Reset iterator after checking
 
-        if cached_activations_path is not None:  # EDIT: load from multi-layer acts
+        self.check_cached_activations_against_config()
+
+        # TODO add support for "mixed loading" (ie use cache until you run out, then switch over to streaming from HF)
+
+    def check_cached_activations_against_config(self):
+
+        if self.cached_activations_path is not None:  # EDIT: load from multi-layer acts
             assert self.cached_activations_path is not None  # keep pyright happy
             # Sanity check: does the cache directory exist?
             assert os.path.exists(
                 self.cached_activations_path
             ), f"Cache directory {self.cached_activations_path} does not exist. Consider double-checking your dataset, model, and hook names."
 
             self.next_cache_idx = 0  # which file to open next
             self.next_idx_within_buffer = 0  # where to start reading from in that file
 
             # Check that we have enough data on disk
-            first_buffer = torch.load(f"{self.cached_activations_path}/0.pt")
+            first_buffer = self.load_buffer(
+                f"{self.cached_activations_path}/{self.next_cache_idx}.safetensors"
+            )
+
             buffer_size_on_disk = first_buffer.shape[0]
             n_buffers_on_disk = len(os.listdir(self.cached_activations_path))
+
             # Note: we're assuming all files have the same number of tokens
             # (which seems reasonable imo since that's what our script does)
             n_activations_on_disk = buffer_size_on_disk * n_buffers_on_disk
             assert (
-                n_activations_on_disk > self.total_training_tokens
+                n_activations_on_disk >= self.total_training_tokens
             ), f"Only {n_activations_on_disk/1e6:.1f}M activations on disk, but total_training_tokens is {self.total_training_tokens/1e6:.1f}M."
 
-            # TODO add support for "mixed loading" (ie use cache until you run out, then switch over to streaming from HF)
+    def apply_norm_scaling_factor(self, activations: torch.Tensor) -> torch.Tensor:
+        return activations * self.estimated_norm_scaling_factor
+
+    def get_norm_scaling_factor(self, activations: torch.Tensor) -> torch.Tensor:
+        return (self.d_in**0.5) / activations.norm(dim=-1).mean()
 
     @property
     def storage_buffer(self) -> torch.Tensor:
         if self._storage_buffer is None:
             self._storage_buffer = self.get_buffer(self.n_batches_in_buffer // 2)
+
         return self._storage_buffer
 
     @property
     def dataloader(self) -> Iterator[Any]:
         if self._dataloader is None:
             self._dataloader = self.get_data_loader()
         return self._dataloader
@@ -247,34 +268,43 @@
         Returns activations of shape (batches, context, num_layers, d_in)
 
         d_in may result from a concatenated head dimension.
         """
         layers = self.hook_point_layers
         act_names = [self.hook_point.format(layer=layer) for layer in layers]
         hook_point_max_layer = max(layers)
+
         layerwise_activations = self.model.run_with_cache(
             batch_tokens,
             names_filter=act_names,
             stop_at_layer=hook_point_max_layer + 1,
             prepend_bos=self.prepend_bos,
             **self.model_kwargs,
         )[1]
-        activations_list = [layerwise_activations[act_name] for act_name in act_names]
-        if self.hook_point_head_index is not None:
-            activations_list = [
-                act[:, :, self.hook_point_head_index] for act in activations_list
-            ]
-        elif activations_list[0].ndim > 3:  # if we have a head dimension
-            # flatten the head dimension
-            activations_list = [
-                act.view(act.shape[0], act.shape[1], -1) for act in activations_list
-            ]
 
-        # Stack along a new dimension to keep separate layers distinct
-        stacked_activations = torch.stack(activations_list, dim=2)
+        n_batches, n_context = batch_tokens.shape
+
+        stacked_activations = torch.zeros(
+            (n_batches, n_context, len(layers), self.d_in)
+        )
+
+        for i, act_name in enumerate(act_names):
+
+            if self.hook_point_head_index is not None:
+                stacked_activations[:, :, i] = layerwise_activations[act_name][
+                    :, :, self.hook_point_head_index
+                ]
+            elif (
+                layerwise_activations[act_names[0]].ndim > 3
+            ):  # if we have a head dimension
+                stacked_activations[:, :, i] = layerwise_activations[act_name].view(
+                    n_batches, n_context, -1
+                )
+            else:
+                stacked_activations[:, :, i] = layerwise_activations[act_name]
 
         return stacked_activations
 
     def get_buffer(self, n_batches_in_buffer: int) -> torch.Tensor:
         context_size = self.context_size
         batch_size = self.store_batch_size
         d_in = self.d_in
@@ -291,15 +321,15 @@
                 device=self.device,
             )
             n_tokens_filled = 0
 
             # Assume activations for different layers are stored separately and need to be combined
             while n_tokens_filled < buffer_size:
                 if not os.path.exists(
-                    f"{self.cached_activations_path}/{self.next_cache_idx}.pt"
+                    f"{self.cached_activations_path}/{self.next_cache_idx}.safetensors"
                 ):
                     print(
                         "\n\nWarning: Ran out of cached activation files earlier than expected."
                     )
                     print(
                         f"Expected to have {buffer_size} activations, but only found {n_tokens_filled}."
                     )
@@ -308,16 +338,16 @@
                             "This might just be a rounding error — your batch_size * n_batches_in_buffer * context_size is not divisible by your total_training_tokens"
                         )
                     print(f"Returning a buffer of size {n_tokens_filled} instead.")
                     print("\n\n")
                     new_buffer = new_buffer[:n_tokens_filled, ...]
                     return new_buffer
 
-                activations = torch.load(
-                    f"{self.cached_activations_path}/{self.next_cache_idx}.pt"
+                activations = self.load_buffer(
+                    f"{self.cached_activations_path}/{self.next_cache_idx}.safetensors"
                 )
                 taking_subset_of_file = False
                 if n_tokens_filled + activations.shape[0] > buffer_size:
                     activations = activations[: buffer_size - n_tokens_filled, ...]
                     taking_subset_of_file = True
 
                 new_buffer[
@@ -350,16 +380,45 @@
             ] = refill_activations
 
             # pbar.update(1)
 
         new_buffer = new_buffer.reshape(-1, num_layers, d_in)
         new_buffer = new_buffer[torch.randperm(new_buffer.shape[0])]
 
+        # every buffer should be normalized:
+        if self.normalize_activations:
+            try:
+                # check if we've already estimated the norm scaling factor
+                assert self.estimated_norm_scaling_factor is not None
+            except AttributeError:
+                # if we haven't estimated it yet, do so.
+                assert (
+                    new_buffer.shape[0] > 3e5
+                ), "Warning: Storage buffer is too small to calculate norm scaling factor and expect it to be reliable."
+                self.estimated_norm_scaling_factor = self.get_norm_scaling_factor(
+                    new_buffer
+                )
+
+            new_buffer = self.apply_norm_scaling_factor(new_buffer)
+
         return new_buffer
 
+    def save_buffer(self, buffer: torch.Tensor, path: str):
+        """
+        Used by cached activations runner to save a buffer to disk.
+        For reuse by later workflows.
+        """
+        save_file({"activations": buffer}, path)
+
+    def load_buffer(self, path: str) -> torch.Tensor:
+
+        with safe_open(path, framework="pt", device=str(self.device)) as f:  # type: ignore
+            buffer = f.get_tensor("activations")
+        return buffer
+
     def get_data_loader(
         self,
     ) -> Iterator[Any]:
         """
         Return a torch.utils.dataloader which you can get batches from.
 
         Should automatically refill the buffer when it gets to n % full.
```

### Comparing `sae_lens-1.4.0/sae_lens/training/config.py` & `sae_lens-1.5.0/sae_lens/training/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     model_name: str = "gelu-2l"
     model_class_name: str = "HookedTransformer"
     hook_point: str = "blocks.{layer}.hook_mlp_out"
     hook_point_eval: str = "blocks.{layer}.attn.pattern"
     hook_point_layer: int | list[int] = 0
     hook_point_head_index: Optional[int] = None
     dataset_path: str = "NeelNanda/c4-tokenized-2b"
+    streaming: bool = True
     is_dataset_tokenized: bool = True
     context_size: int = 128
     use_cached_activations: bool = False
     cached_activations_path: Optional[str] = (
         None  # Defaults to "activations/{dataset}/{model}/{full_hook_name}_{hook_point_head_index}"
     )
 
@@ -43,21 +44,24 @@
     expansion_factor: int | list[int] = 4
     activation_fn: str = "relu"  # relu, tanh-relu
     normalize_sae_decoder: bool = True
     noise_scale: float = 0.0
     from_pretrained_path: Optional[str] = None
     apply_b_dec_to_input: bool = True
     decoder_orthogonal_init: bool = False
+    decoder_heuristic_init: bool = False
+    init_encoder_as_decoder_transpose: bool = False
 
     # Activation Store Parameters
     n_batches_in_buffer: int = 20
     training_tokens: int = 2_000_000
     finetuning_tokens: int = 0
     store_batch_size: int = 32
     train_batch_size: int = 4096
+    normalize_activations: bool = False
 
     # Misc
     device: str | torch.device = "cpu"
     seed: int = 42
     dtype: str | torch.dtype = "float32"  # type: ignore #
     prepend_bos: bool = True
 
@@ -70,14 +74,16 @@
     adam_beta1: float | list[float] = 0
     adam_beta2: float | list[float] = 0.999
 
     ## Loss Function
     mse_loss_normalization: Optional[str] = None
     l1_coefficient: float | list[float] = 1e-3
     lp_norm: float | list[float] = 1
+    scale_sparsity_penalty_by_decoder_norm: bool = False
+    l1_warm_up_steps: int | list[int] = 0
 
     ## Learning Rate Schedule
     lr: float | list[float] = 3e-4
     lr_scheduler_name: str | list[str] = (
         "constant"  # constant, cosineannealing, cosineannealingwarmrestarts
     )
     lr_warm_up_steps: int | list[int] = 500
@@ -104,14 +110,15 @@
     log_activations_store_to_wandb: bool = False
     log_optimizer_state_to_wandb: bool = False
     wandb_project: str = "mats_sae_training_language_model"
     wandb_id: Optional[str] = None
     run_name: Optional[str] = None
     wandb_entity: Optional[str] = None
     wandb_log_frequency: int = 10
+    eval_every_n_wandb_logs: int = 100  # logs every 1000 steps.
 
     # Misc
     resume: bool = False
     n_checkpoints: int = 0
     checkpoint_path: str = "checkpoints"
     verbose: bool = True
     model_kwargs: dict[str, Any] = field(default_factory=dict)
@@ -136,17 +143,23 @@
         if self.run_name is None:
             self.run_name = f"{self.d_sae}-L1-{self.l1_coefficient}-LR-{self.lr}-Tokens-{self.training_tokens:3.3e}"
 
         if self.b_dec_init_method not in ["geometric_median", "mean", "zeros"]:
             raise ValueError(
                 f"b_dec_init_method must be geometric_median, mean, or zeros. Got {self.b_dec_init_method}"
             )
-        if self.b_dec_init_method == "zeros":
-            print(
-                "Warning: We are initializing b_dec to zeros. This is probably not what you want."
+
+        if self.normalize_sae_decoder and self.decoder_heuristic_init:
+            raise ValueError(
+                "You can't normalize the decoder and use heuristic initialization."
+            )
+
+        if self.normalize_sae_decoder and self.scale_sparsity_penalty_by_decoder_norm:
+            raise ValueError(
+                "Weighting loss by decoder norm makes no sense if you are normalizing the decoder weight norms to 1"
             )
 
         if isinstance(self.dtype, str) and self.dtype not in DTYPE_MAP:
             raise ValueError(
                 f"dtype must be one of {list(DTYPE_MAP.keys())}. Got {self.dtype}"
             )
         elif isinstance(self.dtype, str):
@@ -270,28 +283,31 @@
     # Data Generating Function (Model + Training Distibuion)
     model_name: str = "gelu-2l"
     model_class_name: str = "HookedTransformer"
     hook_point: str = "blocks.{layer}.hook_mlp_out"
     hook_point_layer: int | list[int] = 0
     hook_point_head_index: Optional[int] = None
     dataset_path: str = "NeelNanda/c4-tokenized-2b"
+    streaming: bool = True
     is_dataset_tokenized: bool = True
     context_size: int = 128
-    cached_activations_path: Optional[str] = (
+    new_cached_activations_path: Optional[str] = (
         None  # Defaults to "activations/{dataset}/{model}/{full_hook_name}_{hook_point_head_index}"
     )
-
+    # dont' specify this since you don't want to load from disk with the cache runner.
+    cached_activations_path: Optional[str] = None
     # SAE Parameters
     d_in: int = 512
 
     # Activation Store Parameters
     n_batches_in_buffer: int = 20
     training_tokens: int = 2_000_000
     store_batch_size: int = 32
     train_batch_size: int = 4096
+    normalize_activations: bool = False
 
     # Misc
     device: str | torch.device = "cpu"
     seed: int = 42
     dtype: str | torch.dtype = "float32"
     prepend_bos: bool = True
 
@@ -300,16 +316,16 @@
     n_shuffles_with_last_section: int = 10
     n_shuffles_in_entire_dir: int = 10
     n_shuffles_final: int = 100
     model_kwargs: dict[str, Any] = field(default_factory=dict)
 
     def __post_init__(self):
         # Autofill cached_activations_path unless the user overrode it
-        if self.cached_activations_path is None:
-            self.cached_activations_path = _default_cached_activations_path(
+        if self.new_cached_activations_path is None:
+            self.new_cached_activations_path = _default_cached_activations_path(
                 self.dataset_path,
                 self.model_name,
                 self.hook_point,
                 self.hook_point_head_index,
             )
```

### Comparing `sae_lens-1.4.0/sae_lens/training/evals.py` & `sae_lens-1.5.0/sae_lens/training/evals.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         n_batches=10,
     )
 
     recons_score = losses_df["score"].mean()
     ntp_loss = losses_df["loss"].mean()
     recons_loss = losses_df["recons_loss"].mean()
     zero_abl_loss = losses_df["zero_abl_loss"].mean()
+    d_kl = losses_df["d_kl"].mean()
 
     # get cache
     _, cache = model.run_with_cache(
         eval_tokens,
         prepend_bos=False,
         names_filter=[hook_point_eval, hook_point],
         **sparse_autoencoder.cfg.model_kwargs,
@@ -64,23 +65,32 @@
 
     l2_norm_in = torch.norm(original_act, dim=-1)
     l2_norm_out = torch.norm(sae_out, dim=-1)
     l2_norm_in_for_div = l2_norm_in.clone()
     l2_norm_in_for_div[torch.abs(l2_norm_in_for_div) < 0.0001] = 1
     l2_norm_ratio = l2_norm_out / l2_norm_in_for_div
 
+    W_dec_norm_dist = sparse_autoencoder.W_dec.norm(dim=1).detach().cpu().numpy()
+    b_e_dist = sparse_autoencoder.b_enc.detach().cpu().numpy()
+
     metrics = {
         # l2 norms
         f"metrics/l2_norm{suffix}": l2_norm_out.mean().item(),
         f"metrics/l2_ratio{suffix}": l2_norm_ratio.mean().item(),
+        f"metrics/l2_norm_in{suffix}": l2_norm_in.mean().item(),
+        # More detail on loss.
+        f"weights/W_dec_norms{suffix}": wandb.Histogram(W_dec_norm_dist),
+        f"weights/b_e{suffix}": wandb.Histogram(b_e_dist),
         # CE Loss
         f"metrics/CE_loss_score{suffix}": recons_score,
         f"metrics/ce_loss_without_sae{suffix}": ntp_loss,
         f"metrics/ce_loss_with_sae{suffix}": recons_loss,
         f"metrics/ce_loss_with_ablation{suffix}": zero_abl_loss,
+        # KL divergence against intact model
+        f"metrics/kl_div{suffix}": d_kl,
     }
 
     if wandb.run is not None:
         wandb.log(
             metrics,
             step=n_training_steps,
         )
@@ -93,44 +103,47 @@
     model: HookedRootModule,
     activation_store: ActivationsStore,
     n_batches: int = 100,
 ):
     losses = []
     for _ in range(n_batches):
         batch_tokens = activation_store.get_batch_tokens()
-        score, loss, recons_loss, zero_abl_loss = get_recons_loss(
+        score, loss, recons_loss, zero_abl_loss, d_kl = get_recons_loss(
             sparse_autoencoder, model, batch_tokens
         )
         losses.append(
             (
                 score.mean().item(),
                 loss.mean().item(),
                 recons_loss.mean().item(),
                 zero_abl_loss.mean().item(),
+                d_kl.mean().item(),
             )
         )
 
     losses = pd.DataFrame(
-        losses, columns=cast(Any, ["score", "loss", "recons_loss", "zero_abl_loss"])
+        losses,
+        columns=cast(Any, ["score", "loss", "recons_loss", "zero_abl_loss", "d_kl"]),
     )
 
     return losses
 
 
 @torch.no_grad()
 def get_recons_loss(
     sparse_autoencoder: SparseAutoencoder,
     model: HookedRootModule,
     batch_tokens: torch.Tensor,
 ):
     hook_point = sparse_autoencoder.cfg.hook_point
-    loss = model(
-        batch_tokens, return_type="loss", **sparse_autoencoder.cfg.model_kwargs
+    model_outs = model(
+        batch_tokens, return_type="both", **sparse_autoencoder.cfg.model_kwargs
     )
     head_index = sparse_autoencoder.cfg.hook_point_head_index
+    loss = model_outs.loss
 
     def standard_replacement_hook(activations: torch.Tensor, hook: Any):
         activations = sparse_autoencoder.forward(activations).sae_out.to(
             activations.dtype
         )
         return activations
 
@@ -155,34 +168,50 @@
         if head_index is None:
             replacement_hook = all_head_replacement_hook
         else:
             replacement_hook = single_head_replacement_hook
     else:
         replacement_hook = standard_replacement_hook
 
-    recons_loss = model.run_with_hooks(
+    recons_outs = model.run_with_hooks(
         batch_tokens,
-        return_type="loss",
+        return_type="both",
         fwd_hooks=[(hook_point, partial(replacement_hook))],
         **sparse_autoencoder.cfg.model_kwargs,
     )
+    recons_loss = recons_outs.loss
 
     zero_abl_loss = model.run_with_hooks(
         batch_tokens,
         return_type="loss",
         fwd_hooks=[(hook_point, zero_ablate_hook)],
         **sparse_autoencoder.cfg.model_kwargs,
     )
 
     div_val = zero_abl_loss - loss
     div_val[torch.abs(div_val) < 0.0001] = 1.0
 
     score = (zero_abl_loss - recons_loss) / div_val
 
-    return score, loss, recons_loss, zero_abl_loss
+    # KL divergence
+    model_logits = model_outs.logits  # [batch, pos, d_vocab]
+    model_logprobs = torch.nn.functional.log_softmax(model_logits, dim=-1)
+    recons_logits = recons_outs.logits
+    recons_logprobs = torch.nn.functional.log_softmax(recons_logits, dim=-1)
+    # Note: PyTorch KL is backwards compared to the mathematical definition
+    # target distribution comes second, see
+    # https://pytorch.org/docs/stable/generated/torch.nn.functional.kl_div.html
+    d_kl = torch.nn.functional.kl_div(
+        recons_logprobs,
+        model_logprobs,
+        reduction="batchmean",
+        log_target=True,  # for numerics
+    )
+
+    return score, loss, recons_loss, zero_abl_loss, d_kl
 
 
 def zero_ablate_hook(activations: torch.Tensor, hook: Any):
     activations = torch.zeros_like(activations)
     return activations
```

### Comparing `sae_lens-1.4.0/sae_lens/training/geometric_median.py` & `sae_lens-1.5.0/sae_lens/training/geometric_median.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.4.0/sae_lens/training/lm_runner.py` & `sae_lens-1.5.0/sae_lens/training/lm_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,13 +79,14 @@
         train_contexts=train_contexts,
         training_run_state=training_run_state,
         batch_size=cfg.train_batch_size,
         n_checkpoints=cfg.n_checkpoints,
         feature_sampling_window=cfg.feature_sampling_window,
         use_wandb=cfg.log_to_wandb,
         wandb_log_frequency=cfg.wandb_log_frequency,
+        eval_every_n_wandb_logs=cfg.eval_every_n_wandb_logs,
     ).sae_group
 
     if cfg.log_to_wandb:
         wandb.finish()
 
     return sparse_autoencoder
```

### Comparing `sae_lens-1.4.0/sae_lens/training/load_model.py` & `sae_lens-1.5.0/sae_lens/training/load_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.4.0/sae_lens/training/optim.py` & `sae_lens-1.5.0/sae_lens/training/optim.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
 Took the LR scheduler from my previous work: https://github.com/jbloomAus/DecisionTransformerInterpretability/blob/ee55df35cdb92e81d689c72fb9dd5a7252893363/src/decision_transformer/utils.py#L425
 """
 
 import torch.optim as optim
 import torch.optim.lr_scheduler as lr_scheduler
 
+from sae_lens.training.sparse_autoencoder import SparseAutoencoder
+
 
 #  Constant
 #  Cosine Annealing with Warmup
 #  Cosine Annealing with Warmup / Restarts
 #  No default values specified so the type-checker can verify we don't forget any arguments.
-def get_scheduler(
+def get_lr_scheduler(
     scheduler_name: str,
     optimizer: optim.Optimizer,
     training_steps: int,
     lr: float,
     warm_up_steps: int,
     decay_steps: int,
     lr_end: float,
@@ -31,15 +33,15 @@
         warm_up_steps (int, optional): Number of linear warm up steps. Defaults to 0.
         decay_steps (int, optional): Number of linear decay steps to 0. Defaults to 0.
         num_cycles (int, optional): Number of cycles for cosine annealing with warm restarts. Defaults to 1.
         lr_end (float, optional): Final learning rate multiplier before decay. Defaults to 0.0.
     """
     base_scheduler_steps = training_steps - warm_up_steps - decay_steps
     norm_scheduler_name = scheduler_name.lower()
-    main_scheduler = _get_main_scheduler(
+    main_scheduler = _get_main_lr_scheduler(
         norm_scheduler_name,
         optimizer,
         steps=base_scheduler_steps,
         lr_end=lr_end,
         num_cycles=num_cycles,
     )
     if norm_scheduler_name == "constant":
@@ -75,15 +77,15 @@
     return lr_scheduler.SequentialLR(
         schedulers=schedulers,
         optimizer=optimizer,
         milestones=milestones,
     )
 
 
-def _get_main_scheduler(
+def _get_main_lr_scheduler(
     scheduler_name: str,
     optimizer: optim.Optimizer,
     steps: int,
     lr_end: float,
     num_cycles: int,
 ) -> lr_scheduler.LRScheduler:
     if scheduler_name == "constant":
@@ -92,7 +94,50 @@
         return lr_scheduler.CosineAnnealingLR(optimizer, T_max=steps, eta_min=lr_end)
     elif scheduler_name == "cosineannealingwarmrestarts":
         return lr_scheduler.CosineAnnealingWarmRestarts(
             optimizer, T_0=steps // num_cycles, eta_min=lr_end
         )
     else:
         raise ValueError(f"Unsupported scheduler: {scheduler_name}")
+
+
+class L1Scheduler:
+
+    def __init__(
+        self,
+        l1_warm_up_steps: float,
+        total_steps: int,
+        sparse_autoencoder: SparseAutoencoder,
+    ):
+
+        self.type = type
+        self.l1_warmup_steps = l1_warm_up_steps
+        self.total_steps = total_steps
+        self.sparse_autoencoder = sparse_autoencoder
+        self.final_l1_value = sparse_autoencoder.cfg.l1_coefficient
+        self.current_step = 0
+        assert isinstance(self.final_l1_value, float | int)
+
+        # assume using warm-up
+        if self.l1_warmup_steps != 0:
+            sparse_autoencoder.l1_coefficient = 0.0
+
+    def __repr__(self) -> str:
+        return (
+            f"L1Scheduler(final_l1_value={self.final_l1_value}, "
+            f"l1_warmup_steps={self.l1_warmup_steps}, "
+            f"total_steps={self.total_steps})"
+        )
+
+    def step(self):
+        """
+        Updates the l1 coefficient of the sparse autoencoder.
+        """
+        step = self.current_step
+        if step < self.l1_warmup_steps:
+            self.sparse_autoencoder.l1_coefficient = self.final_l1_value * (
+                (1 + step) / self.l1_warmup_steps
+            )  # type: ignore
+        else:
+            self.sparse_autoencoder.l1_coefficient = self.final_l1_value  # type: ignore
+
+        self.current_step += 1
```

### Comparing `sae_lens-1.4.0/sae_lens/training/sae_group.py` & `sae_lens-1.5.0/sae_lens/training/sae_group.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.4.0/sae_lens/training/session_loader.py` & `sae_lens-1.5.0/sae_lens/training/session_loader.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.4.0/sae_lens/training/sparse_autoencoder.py` & `sae_lens-1.5.0/sae_lens/training/sparse_autoencoder.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 class ForwardOutput(NamedTuple):
     sae_out: torch.Tensor
     feature_acts: torch.Tensor
     loss: torch.Tensor
     mse_loss: torch.Tensor
     l1_loss: torch.Tensor
-    ghost_grad_loss: torch.Tensor
+    ghost_grad_loss: torch.Tensor | float
 
 
 class SparseAutoencoder(HookedRootModule):
     """ """
 
     l1_coefficient: float
     lp_norm: float
@@ -83,54 +83,90 @@
         self.device = cfg.device
         self.use_ghost_grads = cfg.use_ghost_grads
         self.normalize_sae_decoder = cfg.normalize_sae_decoder
         self.hook_point_layer = cfg.hook_point_layer
         self.noise_scale = cfg.noise_scale
         self.activation_fn = get_activation_fn(cfg.activation_fn)
 
-        # NOTE: if using resampling neurons method, you must ensure that we initialise the weights in the order W_enc, b_enc, W_dec, b_dec
-        self.W_enc = nn.Parameter(
-            torch.nn.init.kaiming_uniform_(
-                torch.empty(self.d_in, self.d_sae, dtype=self.dtype, device=self.device)
-            )
-        )
+        if self.cfg.scale_sparsity_penalty_by_decoder_norm:
+            self.get_sparsity_loss_term = self.get_sparsity_loss_term_decoder_norm
+        else:
+            self.get_sparsity_loss_term = self.get_sparsity_loss_term_standard
+
+        self.initialize_weights()
+
+        self.hook_sae_in = HookPoint()
+        self.hook_hidden_pre = HookPoint()
+        self.hook_hidden_post = HookPoint()
+        self.hook_sae_out = HookPoint()
+
+        self.setup()  # Required for `HookedRootModule`s
+
+    def initialize_weights(self):
+        """
+        Wrapped around weight initialization code to make init cleaner.
+
+        """
+
+        # no config changes encoder bias init for now.
         self.b_enc = nn.Parameter(
             torch.zeros(self.d_sae, dtype=self.dtype, device=self.device)
         )
 
+        # Start with the default init strategy:
         self.W_dec = nn.Parameter(
             torch.nn.init.kaiming_uniform_(
                 torch.empty(self.d_sae, self.d_in, dtype=self.dtype, device=self.device)
             )
         )
-
         if self.cfg.decoder_orthogonal_init:
             self.W_dec.data = nn.init.orthogonal_(self.W_dec.data.T).T
 
+        elif self.cfg.decoder_heuristic_init:
+            self.W_dec = nn.Parameter(
+                torch.rand(self.d_sae, self.d_in, dtype=self.dtype, device=self.device)
+            )
+            self.initialize_decoder_norm_constant_norm()
+
+        elif self.cfg.normalize_sae_decoder:
+            self.set_decoder_norm_to_unit_norm()
+
+        self.W_enc = nn.Parameter(
+            torch.nn.init.kaiming_uniform_(
+                torch.empty(self.d_in, self.d_sae, dtype=self.dtype, device=self.device)
+            )
+        )
+
+        # Then we intialize the encoder weights (either as the transpose of decoder or not)
+        if self.cfg.init_encoder_as_decoder_transpose:
+            self.W_enc.data = self.W_dec.data.T.clone().contiguous()
+        else:
+            self.W_enc = nn.Parameter(
+                torch.nn.init.kaiming_uniform_(
+                    torch.empty(
+                        self.d_in, self.d_sae, dtype=self.dtype, device=self.device
+                    )
+                )
+            )
+
         if self.normalize_sae_decoder:
             with torch.no_grad():
                 # Anthropic normalize this to have unit columns
                 self.set_decoder_norm_to_unit_norm()
 
+        # methdods which change b_dec as a function of the dataset are implemented after init.
         self.b_dec = nn.Parameter(
             torch.zeros(self.d_in, dtype=self.dtype, device=self.device)
         )
 
         # scaling factor for fine-tuning (not to be used in initial training)
         self.scaling_factor = nn.Parameter(
             torch.ones(self.d_sae, dtype=self.dtype, device=self.device)
         )
 
-        self.hook_sae_in = HookPoint()
-        self.hook_hidden_pre = HookPoint()
-        self.hook_hidden_post = HookPoint()
-        self.hook_sae_out = HookPoint()
-
-        self.setup()  # Required for `HookedRootModule`s
-
     def encode(
         self, x: Float[torch.Tensor, "... d_in"]
     ) -> Float[torch.Tensor, "... d_sae"]:
         feature_acts, _ = self._encode_with_hidden_pre(x)
         return feature_acts
 
     def _encode_with_hidden_pre(
@@ -170,44 +206,67 @@
                 self.W_dec,
                 "... d_sae, d_sae d_in -> ... d_in",
             )
             + self.b_dec
         )
         return sae_out
 
+    def get_sparsity_loss_term_standard(
+        self, feature_acts: torch.Tensor
+    ) -> torch.Tensor:
+        """
+        Sparsity loss term calculated as the L1 norm of the feature activations.
+        """
+        sparsity = feature_acts.norm(p=self.lp_norm, dim=-1)
+        return sparsity
+
+    def get_sparsity_loss_term_decoder_norm(
+        self, feature_acts: torch.Tensor
+    ) -> torch.Tensor:
+        """
+        Sparsity loss term for decoder norm regularization.
+        """
+        weighted_feature_acts = feature_acts * self.W_dec.norm(dim=1)
+        sparsity = weighted_feature_acts.norm(
+            p=self.lp_norm, dim=-1
+        )  # sum over the feature dimension
+        return sparsity
+
     def forward(
         self, x: torch.Tensor, dead_neuron_mask: torch.Tensor | None = None
     ) -> ForwardOutput:
 
         feature_acts, hidden_pre = self._encode_with_hidden_pre(x)
         sae_out = self.decode(feature_acts)
 
         # add config for whether l2 is normalized:
         per_item_mse_loss = _per_item_mse_loss_with_target_norm(
             sae_out, x, self.cfg.mse_loss_normalization
         )
-        ghost_grad_loss = torch.tensor(0.0, dtype=self.dtype, device=self.device)
+
         # gate on config and training so evals is not slowed down.
         if (
             self.use_ghost_grads
             and self.training
             and dead_neuron_mask is not None
             and dead_neuron_mask.sum() > 0
         ):
             ghost_grad_loss = self.calculate_ghost_grad_loss(
                 x=x,
                 sae_out=sae_out,
                 per_item_mse_loss=per_item_mse_loss,
                 hidden_pre=hidden_pre,
                 dead_neuron_mask=dead_neuron_mask,
             )
+        else:
+            ghost_grad_loss = 0
 
-        mse_loss = per_item_mse_loss.mean()
-        sparsity = feature_acts.norm(p=self.lp_norm, dim=-1).mean()
-        l1_loss = self.l1_coefficient * sparsity
+        mse_loss = per_item_mse_loss.sum(dim=-1).mean()
+        sparsity = self.get_sparsity_loss_term(feature_acts)
+        l1_loss = (self.l1_coefficient * sparsity).mean()
         loss = mse_loss + l1_loss + ghost_grad_loss
 
         return ForwardOutput(
             sae_out=sae_out,
             feature_acts=feature_acts,
             loss=loss,
             mse_loss=mse_loss,
@@ -237,14 +296,26 @@
         self.b_dec.data = out.to(self.dtype).to(self.device)
 
     @torch.no_grad()
     def set_decoder_norm_to_unit_norm(self):
         self.W_dec.data /= torch.norm(self.W_dec.data, dim=1, keepdim=True)
 
     @torch.no_grad()
+    def initialize_decoder_norm_constant_norm(self, norm: float = 0.1):
+        """
+        A heuristic proceedure inspired by:
+        https://transformer-circuits.pub/2024/april-update/index.html#training-saes
+        """
+        # TODO: Parameterise this as a function of m and n
+
+        # ensure W_dec norms at unit norm
+        self.W_dec.data /= torch.norm(self.W_dec.data, dim=1, keepdim=True)
+        self.W_dec.data *= 0.1  # will break tests but do this for now.
+
+    @torch.no_grad()
     def remove_gradient_parallel_to_decoder_directions(self):
         """
         Update grads so that they remove the parallel component
             (d_sae, d_in) shape
         """
         assert self.W_dec.grad is not None  # keep pyright happy
 
@@ -470,15 +541,15 @@
 def _per_item_mse_loss_with_target_norm(
     preds: torch.Tensor,
     target: torch.Tensor,
     mse_loss_normalization: Optional[str] = None,
 ) -> torch.Tensor:
     """
     Calculate MSE loss per item in the batch, without taking a mean.
-    Then, normalizes by the L2 norm of the centered target.
+    Then, optionally, normalizes by the L2 norm of the centered target.
     This normalization seems to improve performance.
     """
     if mse_loss_normalization == "dense_batch":
         target_centered = target - target.mean(dim=0, keepdim=True)
         normalization = target_centered.norm(dim=-1, keepdim=True)
         return torch.nn.functional.mse_loss(preds, target, reduction="none") / (
             normalization + 1e-6
```

### Comparing `sae_lens-1.4.0/sae_lens/training/toy_model_runner.py` & `sae_lens-1.5.0/sae_lens/training/toy_model_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.4.0/sae_lens/training/toy_models.py` & `sae_lens-1.5.0/sae_lens/training/toy_models.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.4.0/sae_lens/training/train_sae_on_language_model.py` & `sae_lens-1.5.0/sae_lens/training/train_sae_on_language_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from transformer_lens.hook_points import HookedRootModule
 
 from sae_lens import __version__
 from sae_lens.training.activations_store import ActivationsStore, HfDataset
 from sae_lens.training.config import LanguageModelSAERunnerConfig
 from sae_lens.training.evals import run_evals
 from sae_lens.training.geometric_median import compute_geometric_median
-from sae_lens.training.optim import get_scheduler
+from sae_lens.training.optim import L1Scheduler, get_lr_scheduler
 from sae_lens.training.sae_group import SparseAutoencoderDictionary
 from sae_lens.training.sparse_autoencoder import (
     SAE_CFG_PATH,
     SAE_WEIGHTS_PATH,
     SPARSITY_PATH,
     SparseAutoencoder,
 )
@@ -48,15 +48,16 @@
     Context to track during training for a single SAE
     """
 
     act_freq_scores: torch.Tensor
     n_forward_passes_since_fired: torch.Tensor
     n_frac_active_tokens: int
     optimizer: Optimizer
-    scheduler: LRScheduler
+    lr_scheduler: LRScheduler
+    l1_scheduler: L1Scheduler
     finetuning: bool = False
 
     @property
     def feature_sparsity(self) -> torch.Tensor:
         return self.act_freq_scores / self.n_frac_active_tokens
 
     @property
@@ -180,27 +181,29 @@
     activation_store: ActivationsStore,
     batch_size: int = 1024,
     n_checkpoints: int = 0,
     feature_sampling_window: int = 1000,  # how many training steps between resampling the features / considiring neurons dead
     dead_feature_threshold: float = 1e-8,  # how infrequently a feature has to be active to be considered dead
     use_wandb: bool = False,
     wandb_log_frequency: int = 50,
+    eval_every_n_wandb_logs: int = 100,
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
+        eval_every_n_wandb_logs=eval_every_n_wandb_logs,
     ).sae_group
 
 
 def get_total_training_tokens(sae_group: SparseAutoencoderDictionary) -> int:
     return sae_group.cfg.training_tokens + sae_group.cfg.finetuning_tokens
 
 
@@ -211,14 +214,15 @@
     train_contexts: Optional[dict[str, SAETrainContext]] = None,
     training_run_state: Optional[SAETrainingRunState] = None,
     batch_size: int = 1024,
     n_checkpoints: int = 0,
     feature_sampling_window: int = 1000,  # how many training steps between resampling the features / considiring neurons dead
     use_wandb: bool = False,
     wandb_log_frequency: int = 50,
+    eval_every_n_wandb_logs: int = 100,
 ) -> TrainSAEGroupOutput:
     total_training_tokens = get_total_training_tokens(sae_group=sae_group)
     _update_sae_lens_training_version(sae_group)
     total_training_steps = total_training_tokens // batch_size
 
     checkpoint_thresholds = []
     if n_checkpoints > 0:
@@ -284,14 +288,15 @@
                     n_training_steps=training_run_state.n_training_steps,
                     all_layers=all_layers,
                     batch_size=batch_size,
                     wandb_suffix=wandb_suffix,
                 )
                 mse_losses.append(step_output.mse_loss)
                 l1_losses.append(step_output.l1_loss)
+
                 if use_wandb:
                     with torch.no_grad():
                         if (
                             training_run_state.n_training_steps + 1
                         ) % wandb_log_frequency == 0:
                             wandb.log(
                                 _build_train_step_log_dict(
@@ -302,15 +307,15 @@
                                     training_run_state.n_training_tokens,
                                 ),
                                 step=training_run_state.n_training_steps,
                             )
 
                         # record loss frequently, but not all the time.
                         if (training_run_state.n_training_steps + 1) % (
-                            wandb_log_frequency * 10
+                            wandb_log_frequency * eval_every_n_wandb_logs
                         ) == 0:
                             sparse_autoencoder.eval()
                             run_evals(
                                 sparse_autoencoder,
                                 activation_store,
                                 model,
                                 training_run_state.n_training_steps,
@@ -331,28 +336,30 @@
                     checkpoint_name=training_run_state.n_training_tokens,
                 )
                 checkpoint_thresholds.pop(0)
 
             ###############
 
             training_run_state.n_training_steps += 1
-            pbar.set_description(
-                f"{training_run_state.n_training_steps}| MSE Loss {torch.stack(mse_losses).mean().item():.3f} | L1 {torch.stack(l1_losses).mean().item():.3f}"
-            )
+            if training_run_state.n_training_steps % 100 == 0:
+                pbar.set_description(
+                    f"{training_run_state.n_training_steps}| MSE Loss {torch.stack(mse_losses).mean().item():.3f} | L1 {torch.stack(l1_losses).mean().item():.3f}"
+                )
             pbar.update(batch_size)
 
             ### If n_training_tokens > sae_group.cfg.training_tokens, then we should switch to fine-tuning (if we haven't already)
             if (not training_run_state.started_fine_tuning) and (
                 training_run_state.n_training_tokens > sae_group.cfg.training_tokens
             ):
                 training_run_state.started_fine_tuning = True
                 for name, sparse_autoencoder in sae_group.autoencoders.items():
                     ctx = train_contexts[name]
                     # this should turn grads on for the scaling factor and other parameters.
                     ctx.begin_finetuning(sae_group.autoencoders[name])
+
     except (KeyboardInterrupt, InterruptedException):
         print("interrupted, saving progress")
         checkpoint_name = training_run_state.n_training_tokens
         _save_checkpoint(
             sae_group,
             activation_store=activation_store,
             train_contexts=train_contexts,
@@ -441,31 +448,38 @@
         lr=sae.cfg.lr,
         betas=(
             sae.cfg.adam_beta1,  # type: ignore
             sae.cfg.adam_beta2,  # type: ignore
         ),
     )
     assert sae.cfg.lr_end is not None  # this is set in config post-init
-    scheduler = get_scheduler(
+    lr_scheduler = get_lr_scheduler(
         sae.cfg.lr_scheduler_name,
         lr=sae.cfg.lr,
         optimizer=optimizer,
         warm_up_steps=sae.cfg.lr_warm_up_steps,
         decay_steps=sae.cfg.lr_decay_steps,
         training_steps=total_training_steps,
         lr_end=sae.cfg.lr_end,
         num_cycles=sae.cfg.n_restart_cycles,
     )
 
+    l1_scheduler = L1Scheduler(
+        l1_warm_up_steps=sae.cfg.l1_warm_up_steps,  # type: ignore
+        total_steps=total_training_steps,
+        sparse_autoencoder=sae,
+    )
+
     return SAETrainContext(
         act_freq_scores=act_freq_scores,
         n_forward_passes_since_fired=n_forward_passes_since_fired,
         n_frac_active_tokens=n_frac_active_tokens,
         optimizer=optimizer,
-        scheduler=scheduler,
+        lr_scheduler=lr_scheduler,
+        l1_scheduler=l1_scheduler,
     )
 
 
 def _init_sae_group_b_decs(
     sae_group: SparseAutoencoderDictionary,
     activation_store: ActivationsStore,
     all_layers: list[int],
@@ -584,18 +598,25 @@
     with torch.no_grad():
         # Calculate the sparsities, and add it to a list, calculate sparsity metrics
         ctx.act_freq_scores += (feature_acts.abs() > 0).float().sum(0)
         ctx.n_frac_active_tokens += batch_size
 
     ctx.optimizer.zero_grad()
     loss.backward()
+
+    # clip grad norm
+    # TODO: Work out if this should be in config / how to test it.
+    torch.nn.utils.clip_grad_norm_(sparse_autoencoder.parameters(), 1.0)
+
     if sparse_autoencoder.normalize_sae_decoder:
         sparse_autoencoder.remove_gradient_parallel_to_decoder_directions()
+
     ctx.optimizer.step()
-    ctx.scheduler.step()
+    ctx.lr_scheduler.step()
+    ctx.l1_scheduler.step()
 
     return TrainStepOutput(
         sae_in=sae_in,
         sae_out=sae_out,
         feature_acts=feature_acts,
         loss=loss,
         mse_loss=mse_loss,
@@ -625,29 +646,32 @@
     l0 = (feature_acts > 0).float().sum(-1).mean()
     current_learning_rate = ctx.optimizer.param_groups[0]["lr"]
 
     per_token_l2_loss = (sae_out - sae_in).pow(2).sum(dim=-1).squeeze()
     total_variance = (sae_in - sae_in.mean(0)).pow(2).sum(-1)
     explained_variance = 1 - per_token_l2_loss / total_variance
 
+    if isinstance(ghost_grad_loss, torch.Tensor):
+        ghost_grad_loss = ghost_grad_loss.item()
     return {
         # losses
         f"losses/mse_loss{wandb_suffix}": mse_loss.item(),
         f"losses/l1_loss{wandb_suffix}": l1_loss.item()
         / sparse_autoencoder.l1_coefficient,  # normalize by l1 coefficient
-        f"losses/ghost_grad_loss{wandb_suffix}": ghost_grad_loss.item(),
+        f"losses/ghost_grad_loss{wandb_suffix}": ghost_grad_loss,
         f"losses/overall_loss{wandb_suffix}": loss.item(),
         # variance explained
         f"metrics/explained_variance{wandb_suffix}": explained_variance.mean().item(),
         f"metrics/explained_variance_std{wandb_suffix}": explained_variance.std().item(),
         f"metrics/l0{wandb_suffix}": l0.item(),
         # sparsity
         f"sparsity/mean_passes_since_fired{wandb_suffix}": ctx.n_forward_passes_since_fired.mean().item(),
         f"sparsity/dead_features{wandb_suffix}": ghost_grad_neuron_mask.sum().item(),
         f"details/current_learning_rate{wandb_suffix}": current_learning_rate,
+        f"details/current_l1_coefficient{wandb_suffix}": sparse_autoencoder.l1_coefficient,
         "details/n_training_tokens": n_training_tokens,
     }
 
 
 ACTIVATION_STORE_PATH = "activation_store.safetensors"
 TRAINING_RUN_STATE_PATH = "training_run_state.pkl"
 SAE_CONTEXT_PATH = "ctx.safetensors"
```

### Comparing `sae_lens-1.4.0/sae_lens/training/train_sae_on_toy_model.py` & `sae_lens-1.5.0/sae_lens/training/train_sae_on_toy_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.4.0/PKG-INFO` & `sae_lens-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sae-lens
-Version: 1.4.0
+Version: 1.5.0
 Summary: Training and Analyzing Sparse Autoencoders (SAEs)
 Author: Joseph Bloom
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -23,14 +23,15 @@
 Requires-Dist: mkdocs-section-index (>=0.3.8,<0.4.0)
 Requires-Dist: mkdocstrings (>=0.24.1,<0.25.0)
 Requires-Dist: mkdocstrings-python (>=1.9.0,<2.0.0)
 Requires-Dist: nbformat (>=5.9.2,<6.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: plotly (>=5.19.0,<6.0.0)
 Requires-Dist: plotly-express (>=0.4.1,<0.5.0)
+Requires-Dist: pytest-profiling (>=1.7.0,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: pyzmq (==26.0.0)
 Requires-Dist: sae-vis (>=0.2.18,<0.3.0)
 Requires-Dist: safetensors (>=0.4.2,<0.5.0)
 Requires-Dist: transformer-lens (>=1.14.0,<2.0.0)
 Requires-Dist: transformers (>=4.38.1,<5.0.0)
```

