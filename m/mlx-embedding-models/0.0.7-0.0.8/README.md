# Comparing `tmp/mlx_embedding_models-0.0.7.tar.gz` & `tmp/mlx_embedding_models-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlx_embedding_models-0.0.7.tar", last modified: Tue Feb 13 00:46:36 2024, max compression
+gzip compressed data, was "mlx_embedding_models-0.0.8.tar", last modified: Tue May  7 16:56:02 2024, max compression
```

## Comparing `mlx_embedding_models-0.0.7.tar` & `mlx_embedding_models-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2024-02-13 00:46:36.612353 mlx_embedding_models-0.0.7/
--rw-r--r--   0 benjamin   (501) staff       (20)     1066 2024-02-10 06:19:21.000000 mlx_embedding_models-0.0.7/LICENSE
--rw-r--r--   0 benjamin   (501) staff       (20)      994 2024-02-13 00:46:36.612150 mlx_embedding_models-0.0.7/PKG-INFO
--rw-r--r--   0 benjamin   (501) staff       (20)      608 2024-02-11 19:46:40.000000 mlx_embedding_models-0.0.7/README.md
--rw-r--r--   0 benjamin   (501) staff       (20)      443 2024-02-13 00:46:19.000000 mlx_embedding_models-0.0.7/pyproject.toml
--rw-r--r--   0 benjamin   (501) staff       (20)       38 2024-02-13 00:46:36.612394 mlx_embedding_models-0.0.7/setup.cfg
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2024-02-13 00:46:36.609379 mlx_embedding_models-0.0.7/src/
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2024-02-13 00:46:36.610745 mlx_embedding_models-0.0.7/src/mlx_embedding_models/
--rw-r--r--   0 benjamin   (501) staff       (20)     5592 2024-02-11 02:38:05.000000 mlx_embedding_models-0.0.7/src/mlx_embedding_models/embedding.py
--rw-r--r--   0 benjamin   (501) staff       (20)      972 2024-02-10 20:48:06.000000 mlx_embedding_models-0.0.7/src/mlx_embedding_models/load_utils.py
--rw-r--r--   0 benjamin   (501) staff       (20)     4335 2024-02-12 21:30:26.000000 mlx_embedding_models-0.0.7/src/mlx_embedding_models/model.py
--rw-r--r--   0 benjamin   (501) staff       (20)     1401 2024-02-11 19:08:35.000000 mlx_embedding_models-0.0.7/src/mlx_embedding_models/registry.py
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2024-02-13 00:46:36.611939 mlx_embedding_models-0.0.7/src/mlx_embedding_models.egg-info/
--rw-r--r--   0 benjamin   (501) staff       (20)      994 2024-02-13 00:46:36.000000 mlx_embedding_models-0.0.7/src/mlx_embedding_models.egg-info/PKG-INFO
--rw-r--r--   0 benjamin   (501) staff       (20)      419 2024-02-13 00:46:36.000000 mlx_embedding_models-0.0.7/src/mlx_embedding_models.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin   (501) staff       (20)        1 2024-02-13 00:46:36.000000 mlx_embedding_models-0.0.7/src/mlx_embedding_models.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin   (501) staff       (20)       42 2024-02-13 00:46:36.000000 mlx_embedding_models-0.0.7/src/mlx_embedding_models.egg-info/requires.txt
--rw-r--r--   0 benjamin   (501) staff       (20)       21 2024-02-13 00:46:36.000000 mlx_embedding_models-0.0.7/src/mlx_embedding_models.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2024-05-07 16:56:02.308948 mlx_embedding_models-0.0.8/
+-rw-r--r--   0 benjamin   (501) staff       (20)     1066 2024-02-10 06:19:21.000000 mlx_embedding_models-0.0.8/LICENSE
+-rw-r--r--   0 benjamin   (501) staff       (20)     1022 2024-05-07 16:56:02.308778 mlx_embedding_models-0.0.8/PKG-INFO
+-rw-r--r--   0 benjamin   (501) staff       (20)      608 2024-02-11 19:46:40.000000 mlx_embedding_models-0.0.8/README.md
+-rw-r--r--   0 benjamin   (501) staff       (20)      463 2024-05-07 16:55:55.000000 mlx_embedding_models-0.0.8/pyproject.toml
+-rw-r--r--   0 benjamin   (501) staff       (20)       38 2024-05-07 16:56:02.308992 mlx_embedding_models-0.0.8/setup.cfg
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2024-05-07 16:56:02.305755 mlx_embedding_models-0.0.8/src/
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2024-05-07 16:56:02.307611 mlx_embedding_models-0.0.8/src/mlx_embedding_models/
+-rw-r--r--   0 benjamin   (501) staff       (20)    12078 2024-05-07 03:44:29.000000 mlx_embedding_models-0.0.8/src/mlx_embedding_models/embedding.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     4879 2024-03-18 17:56:39.000000 mlx_embedding_models-0.0.8/src/mlx_embedding_models/load_utils.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     7194 2024-03-08 00:29:04.000000 mlx_embedding_models-0.0.8/src/mlx_embedding_models/model.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     9624 2024-05-07 16:55:04.000000 mlx_embedding_models-0.0.8/src/mlx_embedding_models/nomic_model.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     3548 2024-05-03 20:33:59.000000 mlx_embedding_models-0.0.8/src/mlx_embedding_models/registry.py
+-rw-r--r--   0 benjamin   (501) staff       (20)        0 2024-03-17 17:34:49.000000 mlx_embedding_models-0.0.8/src/mlx_embedding_models/test_mteb.py
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2024-05-07 16:56:02.308570 mlx_embedding_models-0.0.8/src/mlx_embedding_models.egg-info/
+-rw-r--r--   0 benjamin   (501) staff       (20)     1022 2024-05-07 16:56:02.000000 mlx_embedding_models-0.0.8/src/mlx_embedding_models.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin   (501) staff       (20)      497 2024-05-07 16:56:02.000000 mlx_embedding_models-0.0.8/src/mlx_embedding_models.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)        1 2024-05-07 16:56:02.000000 mlx_embedding_models-0.0.8/src/mlx_embedding_models.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)       55 2024-05-07 16:56:02.000000 mlx_embedding_models-0.0.8/src/mlx_embedding_models.egg-info/requires.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)       21 2024-05-07 16:56:02.000000 mlx_embedding_models-0.0.8/src/mlx_embedding_models.egg-info/top_level.txt
```

### Comparing `mlx_embedding_models-0.0.7/LICENSE` & `mlx_embedding_models-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mlx_embedding_models-0.0.7/PKG-INFO` & `mlx_embedding_models-0.0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: mlx_embedding_models
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python utility for text embeddings in MLX.
 Author-email: Benjamin Anderson <ben@trytaylor.ai>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: transformers
-Requires-Dist: mlx
+Requires-Dist: mlx>=0.6.0
 Requires-Dist: awkward
 Requires-Dist: numpy
+Requires-Dist: scipy
 Requires-Dist: tqdm
 
 # MLX Embedding Models
 Run text embeddings on your Apple Silicon GPU. Supports any BERT- or RoBERTa-based embedding model, with a curated registry of high-performing models that just work off the shelf.
 
 Get started by installing from PyPI:
 ```
```

### Comparing `mlx_embedding_models-0.0.7/README.md` & `mlx_embedding_models-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `mlx_embedding_models-0.0.7/src/mlx_embedding_models/model.py` & `mlx_embedding_models-0.0.8/src/mlx_embedding_models/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,43 @@
 # modeling code adapted from mlx-examples (MIT License)
 # https://github.com/ml-explore/mlx-examples
 
 import tempfile
-from typing import Tuple, Union
+from typing import Tuple, Union, Optional
 import mlx.core as mx
 import mlx.nn as nn
 import numpy as np
-from transformers import AutoConfig, BertConfig, RobertaConfig
-from .load_utils import convert
+from transformers import AutoConfig, BertConfig, RobertaConfig, DistilBertConfig
+from .load_utils import convert, convert_distilbert, bert_config_from_distilbert
+
+
+# class FastAttention(nn.Module):
+#     def __init__(self, config: Union[BertConfig, RobertaConfig]):
+#         super().__init__()
+#         self.num_heads = config.num_attention_heads
+#         self.query_proj = nn.Linear(config.hidden_size, config.hidden_size, bias=True)
+#         self.key_proj = nn.Linear(config.hidden_size, config.hidden_size, bias=True)
+#         self.value_proj = nn.Linear(config.hidden_size, config.hidden_size, bias=True)
+#         self.out_proj = nn.Linear(config.hidden_size, config.hidden_size, bias=True)
+#         self.scale = 1 / (config.hidden_size ** 0.5)
+    
+#     def shape(self, tensor: mx.array):
+#         B, L, D = tensor.shape
+#         tensor = tensor.reshape(B, L, self.num_heads, D // self.num_heads)
+#         return tensor.transpose(0, 2, 1, 3)
+
+#     def __call__(self, x, mask):
+#         q = self.query_proj(x)
+#         k = self.key_proj(x)
+#         v = self.value_proj(x)
+#         q, k, v = map(self.shape, (q, k, v))
+#         attn_out = mx.fast.scaled_dot_product_attention(
+#             q, k, v, mask, self.scale
+#         )
+#         return self.out_proj(attn_out)
 
 class TransformerEncoderLayer(nn.Module):
     """
     A transformer encoder layer with (the original BERT) post-normalization.
     """
 
     def __init__(
@@ -19,28 +45,28 @@
         config: Union[BertConfig, RobertaConfig],
         # dims: int,
         # num_heads: int,
         # mlp_dims: Optional[int] = None,
         # layer_norm_eps: float = 1e-12,
     ):
         super().__init__()
-        # mlp_dims = mlp_dims or dims * 4
         self.attention = nn.MultiHeadAttention(
             config.hidden_size, 
             config.num_attention_heads, 
             bias=True
         )
+        # self.attention = FastAttention(config)
         self.ln1 = nn.LayerNorm(config.hidden_size, eps=config.layer_norm_eps)
         self.ln2 = nn.LayerNorm(config.hidden_size, eps=config.layer_norm_eps)
         self.linear1 = nn.Linear(config.hidden_size, config.intermediate_size)
         self.linear2 = nn.Linear(config.intermediate_size, config.hidden_size)
         self.gelu = nn.GELU()
 
     def __call__(self, x, mask):
-        attention_out = self.attention(x, x, x, mask)
+        attention_out = self.attention(x, x, x, mask) # x, x, x, mask
         add_and_norm = self.ln1(x + attention_out)
 
         ff = self.linear1(add_and_norm)
         ff_gelu = self.gelu(ff)
         ff_out = self.linear2(ff_gelu)
         x = self.ln2(ff_out + add_and_norm)
 
@@ -61,66 +87,104 @@
         for layer in self.layers:
             x = layer(x, mask)
 
         return x
 
 
 class BertEmbeddings(nn.Module):
-    def __init__(self, config: Union[BertConfig, RobertaConfig]):
+    def __init__(self, config: Union[BertConfig, RobertaConfig, DistilBertConfig]):
         self.word_embeddings = nn.Embedding(config.vocab_size, config.hidden_size)
-        self.token_type_embeddings = nn.Embedding(config.type_vocab_size, config.hidden_size)
+        self.token_type_embeddings = nn.Embedding(config.type_vocab_size, config.hidden_size) if config.type_vocab_size > 0 else None
         self.position_embeddings = nn.Embedding(
             config.max_position_embeddings, config.hidden_size
         )
         self.norm = nn.LayerNorm(config.hidden_size, eps=config.layer_norm_eps)
 
-    def __call__(self, input_ids: mx.array, token_type_ids: mx.array) -> mx.array:
+    def __call__(self, input_ids: mx.array, token_type_ids: Optional[mx.array]) -> mx.array:
         words = self.word_embeddings(input_ids)
         position = self.position_embeddings(
             mx.broadcast_to(mx.arange(input_ids.shape[1]), input_ids.shape)
         )
-        token_types = self.token_type_embeddings(token_type_ids)
-
-        embeddings = position + words + token_types
+        if token_type_ids is not None and self.token_type_embeddings is not None:
+            token_types = self.token_type_embeddings(token_type_ids)
+            embeddings = position + words + token_types
+        else:
+            embeddings = position + words
         return self.norm(embeddings)
+    
+class LMHead(nn.Module):
+    def __init__(self, config: Union[BertConfig, RobertaConfig]):
+        super().__init__()
+        self.dense = nn.Linear(config.hidden_size, config.hidden_size, bias=True)
+        self.gelu = nn.GELU()
+        self.ln = nn.LayerNorm(config.hidden_size, eps=config.layer_norm_eps)
+        self.decoder = nn.Linear(config.hidden_size, config.vocab_size, bias=True)
 
+    def __call__(self, x: mx.array) -> mx.array:
+        x = self.dense(x)
+        x = self.gelu(x)
+        x = self.ln(x)
+        x = self.decoder(x)
+        return x
 
 class Bert(nn.Module):
-    def __init__(self, config: Union[BertConfig, RobertaConfig]):
+    def __init__(self, config: Union[BertConfig, RobertaConfig], lm_head: bool = False):
         self.embeddings = BertEmbeddings(config)
         self.encoder = TransformerEncoder(
             config
         )
-        self.pooler = nn.Linear(config.hidden_size, config.hidden_size)
+        
+        if lm_head:
+            self.lm_head = LMHead(config)
+            self.pooler = None
+        else:
+            self.lm_head = None
+            self.pooler = nn.Linear(config.hidden_size, config.hidden_size)
 
     def __call__(
         self,
         input_ids: mx.array,
-        token_type_ids: mx.array,
-        attention_mask: mx.array = None,
+        token_type_ids: Optional[mx.array] = None,
+        attention_mask: Optional[mx.array] = None,
     ) -> Tuple[mx.array, mx.array]:
         x = self.embeddings(input_ids, token_type_ids)
 
         if attention_mask is not None:
             # convert 0's to -infs, 1's to 0's, and make it broadcastable
             attention_mask = mx.log(attention_mask)
             attention_mask = mx.expand_dims(attention_mask, (1, 2))
 
-        y = self.encoder(x, attention_mask)
-        return y, mx.tanh(self.pooler(y[:, 0]))
+        # mlm output
+        if self.lm_head is not None:
+            y = self.encoder(x, attention_mask)
+            return self.lm_head(y), None # no pooler output
+        
+        # pooler output
+        else:
+            y = self.encoder(x, attention_mask)
+            return y, mx.tanh(self.pooler(y[:, 0]))
     
     @classmethod
-    def from_pretrained(cls, model_path: str):
+    def from_pretrained(cls, model_path: str, lm_head: bool = False):
         config = AutoConfig.from_pretrained(model_path)
         # check if it's a bert or roberta model
         if isinstance(config, BertConfig):
             config = BertConfig.from_pretrained(model_path)
+            tensors = convert(model_path, lm_head=lm_head)
         elif isinstance(config, RobertaConfig):
             config = RobertaConfig.from_pretrained(model_path)
-        model = cls(config)
-        tensors = convert(model_path)
+            tensors = convert(model_path, lm_head=lm_head)
+        elif isinstance(config, DistilBertConfig):
+            config = DistilBertConfig.from_pretrained(model_path)
+            config = bert_config_from_distilbert(config)
+            tensors = convert_distilbert(model_path, lm_head=lm_head)
+        model = cls(config, lm_head=lm_head)
+
+        # print all keys in model
+        # print(model)
+        
         # use npz extension
         with tempfile.NamedTemporaryFile(suffix=".npz") as f:
             np.savez(f, **tensors)
             f.seek(0)
             model.load_weights(f.name)
         return model
```

### Comparing `mlx_embedding_models-0.0.7/src/mlx_embedding_models.egg-info/PKG-INFO` & `mlx_embedding_models-0.0.8/src/mlx_embedding_models.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: mlx_embedding_models
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python utility for text embeddings in MLX.
 Author-email: Benjamin Anderson <ben@trytaylor.ai>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: transformers
-Requires-Dist: mlx
+Requires-Dist: mlx>=0.6.0
 Requires-Dist: awkward
 Requires-Dist: numpy
+Requires-Dist: scipy
 Requires-Dist: tqdm
 
 # MLX Embedding Models
 Run text embeddings on your Apple Silicon GPU. Supports any BERT- or RoBERTa-based embedding model, with a curated registry of high-performing models that just work off the shelf.
 
 Get started by installing from PyPI:
 ```
```

