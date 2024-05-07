# Comparing `tmp/moltx-0.9.8.tar.gz` & `tmp/moltx-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moltx-0.9.8.tar", last modified: Fri Apr 26 13:18:08 2024, max compression
+gzip compressed data, was "moltx-1.0.0.tar", last modified: Tue May  7 15:06:08 2024, max compression
```

## Comparing `moltx-0.9.8.tar` & `moltx-1.0.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:18:08.931977 moltx-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 13:18:03.000000 moltx-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-26 13:18:08.931977 moltx-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-04-26 13:18:03.000000 moltx-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:18:08.927977 moltx-0.9.8/moltx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:18:03.000000 moltx-0.9.8/moltx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 13:18:03.000000 moltx-0.9.8/moltx/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:18:08.927977 moltx-0.9.8/moltx/data/
--rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-04-26 13:18:03.000000 moltx-0.9.8/moltx/data/spe_safe.txt
--rw-r--r--   0 runner    (1001) docker     (127)    27879 2024-04-26 13:18:03.000000 moltx-0.9.8/moltx/data/spe_smiles.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-04-26 13:18:03.000000 moltx-0.9.8/moltx/data/tks_safe.json
--rw-r--r--   0 runner    (1001) docker     (127)    36304 2024-04-26 13:18:03.000000 moltx-0.9.8/moltx/data/tks_smiles.json
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-26 13:18:03.000000 moltx-0.9.8/moltx/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-26 13:18:03.000000 moltx-0.9.8/moltx/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-26 13:18:03.000000 moltx-0.9.8/moltx/nets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-04-26 13:18:03.000000 moltx-0.9.8/moltx/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-04-26 13:18:03.000000 moltx-0.9.8/moltx/tokenizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:18:08.931977 moltx-0.9.8/moltx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-26 13:18:08.000000 moltx-0.9.8/moltx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-26 13:18:08.000000 moltx-0.9.8/moltx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 13:18:08.000000 moltx-0.9.8/moltx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-26 13:18:08.000000 moltx-0.9.8/moltx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 13:18:08.000000 moltx-0.9.8/moltx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-26 13:18:03.000000 moltx-0.9.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-26 13:18:08.931977 moltx-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 13:18:03.000000 moltx-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:18:08.927977 moltx-0.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-26 13:18:03.000000 moltx-0.9.8/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-26 13:18:03.000000 moltx-0.9.8/tests/test_nets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-26 13:18:03.000000 moltx-0.9.8/tests/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-26 13:18:03.000000 moltx-0.9.8/tests/test_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:06:08.320443 moltx-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 15:05:59.000000 moltx-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-05-07 15:06:08.320443 moltx-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-05-07 15:05:59.000000 moltx-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:06:08.320443 moltx-1.0.0/moltx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:05:59.000000 moltx-1.0.0/moltx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 15:05:59.000000 moltx-1.0.0/moltx/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:06:08.320443 moltx-1.0.0/moltx/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-05-07 15:05:59.000000 moltx-1.0.0/moltx/data/spe_safe.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    27879 2024-05-07 15:05:59.000000 moltx-1.0.0/moltx/data/spe_smiles.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-05-07 15:05:59.000000 moltx-1.0.0/moltx/data/tks_safe.json
+-rw-r--r--   0 runner    (1001) docker     (127)    36304 2024-05-07 15:05:59.000000 moltx-1.0.0/moltx/data/tks_smiles.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-05-07 15:05:59.000000 moltx-1.0.0/moltx/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-05-07 15:05:59.000000 moltx-1.0.0/moltx/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-07 15:05:59.000000 moltx-1.0.0/moltx/nets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-07 15:05:59.000000 moltx-1.0.0/moltx/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-07 15:05:59.000000 moltx-1.0.0/moltx/tokenizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:06:08.320443 moltx-1.0.0/moltx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-05-07 15:06:08.000000 moltx-1.0.0/moltx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-07 15:06:08.000000 moltx-1.0.0/moltx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 15:06:08.000000 moltx-1.0.0/moltx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 15:06:08.000000 moltx-1.0.0/moltx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 15:06:08.000000 moltx-1.0.0/moltx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 15:05:59.000000 moltx-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-07 15:06:08.324442 moltx-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 15:05:59.000000 moltx-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:06:08.320443 moltx-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-07 15:05:59.000000 moltx-1.0.0/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-07 15:05:59.000000 moltx-1.0.0/tests/test_nets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-05-07 15:05:59.000000 moltx-1.0.0/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-07 15:05:59.000000 moltx-1.0.0/tests/test_tokenizer.py
```

### Comparing `moltx-0.9.8/LICENSE` & `moltx-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moltx-0.9.8/PKG-INFO` & `moltx-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: moltx
-Version: 0.9.8
+Version: 1.0.0
 Summary: Molcule Transformer X Model
 Author: Michael Ding
 Author-email: yandy.ding@gmail.com
-License: Apache-2.0
 Keywords: molcule,AI,deep learning,transformer
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rdkit~=2023.9.1
 Requires-Dist: torch~=2.2.0
 
 # MolTx
```

### Comparing `moltx-0.9.8/README.md` & `moltx-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `moltx-0.9.8/moltx/data/spe_safe.txt` & `moltx-1.0.0/moltx/data/spe_safe.txt`

 * *Files identical despite different names*

### Comparing `moltx-0.9.8/moltx/data/spe_smiles.txt` & `moltx-1.0.0/moltx/data/spe_smiles.txt`

 * *Files identical despite different names*

### Comparing `moltx-0.9.8/moltx/data/tks_safe.json` & `moltx-1.0.0/moltx/data/tks_safe.json`

 * *Files identical despite different names*

### Comparing `moltx-0.9.8/moltx/data/tks_smiles.json` & `moltx-1.0.0/moltx/data/tks_smiles.json`

 * *Files identical despite different names*

### Comparing `moltx-0.9.8/moltx/datasets.py` & `moltx-1.0.0/moltx/datasets.py`

 * *Files 25% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         tgt = self._tokenize(
             [f"{self.tokenizer.BOS}{smi}{self.tokenizer.EOS}" for smi in smiles])
         out = torch.tensor(labels, device=self.device).unsqueeze(-1)
         return src, tgt, out
 
 
 class AdaMRRegression(AdaMR):
-    def __call__(self, smiles: typing.Sequence[str], values: typing.Sequence[int]) -> typing.Tuple[torch.Tensor]:
+    def __call__(self, smiles: typing.Sequence[str], values: typing.Sequence[float]) -> typing.Tuple[torch.Tensor]:
         if len(smiles) != len(values):
             raise RuntimeError(
                 "the length of smiles and values must be the same!")
         src = self._tokenize(smiles)
         tgt = self._tokenize(
             [f"{self.tokenizer.BOS}{smi}{self.tokenizer.EOS}" for smi in smiles])
         out = torch.tensor(values, device=self.device).unsqueeze(-1)
@@ -72,7 +72,62 @@
         if len(smiles) != len(goals):
             raise RuntimeError(
                 "the length of smiles and goals must be the same!")
         head = [self.tokenizer.CLS for _ in range(len(smiles))]
         src, tgt, out = super().__call__(head, smiles)
         goal = torch.tensor(goals, device=self.device).unsqueeze(-1)
         return goal, src, tgt, out
+
+
+class AdaMR2(Base):
+    def __call__(self, s1: typing.Sequence[str], s2: typing.Sequence[str]) -> typing.Tuple[torch.Tensor]:
+        if len(s1) != len(s2):
+            raise RuntimeError("the length of s1 and s2 must be the same!")
+        bos = self.tokenizer[self.tokenizer.BOS]
+        eos = self.tokenizer[self.tokenizer.EOS]
+        s1tokens = [self.tokenizer(smi) for smi in s1]
+        s2tokens = [self.tokenizer(smi) for smi in s2]
+        tgt_tokens = [tks1 + [bos] + tks2 for tks1, tks2 in zip(s1tokens, s2tokens)]
+        out_tokens = [[0] * len(tks1) + tks2 + [eos] for tks1, tks2 in zip(s1tokens, s2tokens)]
+        size = max(map(len, out_tokens))
+        tgt = torch.concat([self._tokens2tensor(tks, size).unsqueeze(0) for tks in tgt_tokens])
+        out = torch.concat([self._tokens2tensor(tks, size).unsqueeze(0) for tks in out_tokens])
+        return tgt, out
+
+
+class AdaMR2Classifier(AdaMR2):
+    def __call__(self, smiles: typing.Sequence[str], labels: typing.Sequence[int]) -> typing.Tuple[torch.Tensor]:
+        if len(smiles) != len(labels):
+            raise RuntimeError(
+                "the length of smiles and labels must be the same!")
+        tgt = self._tokenize(
+            [f"{self.tokenizer.BOS}{smi}{self.tokenizer.EOS}" for smi in smiles])
+        out = torch.tensor(labels, device=self.device).unsqueeze(-1)
+        return tgt, out
+
+
+class AdaMR2Regression(AdaMR2):
+    def __call__(self, smiles: typing.Sequence[str], values: typing.Sequence[float]) -> typing.Tuple[torch.Tensor]:
+        if len(smiles) != len(values):
+            raise RuntimeError(
+                "the length of smiles and values must be the same!")
+        tgt = self._tokenize(
+            [f"{self.tokenizer.BOS}{smi}{self.tokenizer.EOS}" for smi in smiles])
+        out = torch.tensor(values, device=self.device).unsqueeze(-1)
+        return tgt, out
+
+
+class AdaMR2DistGeneration(AdaMR2):
+    def __call__(self, smiles: typing.Sequence[str]) -> typing.Tuple[torch.Tensor]:
+        head = [self.tokenizer.CLS for _ in range(len(smiles))]
+        return super().__call__(head, smiles)
+
+
+class AdaMR2GoalGeneration(AdaMR2):
+    def __call__(self, smiles: typing.Sequence[str], goals: typing.Sequence[float]) -> typing.Tuple[torch.Tensor]:
+        if len(smiles) != len(goals):
+            raise RuntimeError(
+                "the length of smiles and goals must be the same!")
+        head = [self.tokenizer.CLS for _ in range(len(smiles))]
+        tgt, out = super().__call__(head, smiles)
+        goal = torch.tensor(goals, device=self.device).unsqueeze(-1)
+        return goal, tgt, out
```

### Comparing `moltx-0.9.8/moltx/models.py` & `moltx-1.0.0/moltx/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import typing
 import torch
 import torch.nn as nn
 from moltx import nets, tokenizers
 
 
 class AdaMRTokenizerConfig:
     Pretrain = tokenizers.MoltxPretrainConfig(
@@ -68,15 +67,15 @@
             nn.Dropout(conf.dropout),
             nn.Linear(conf.d_model, d_hidden, dtype=conf.dtype),
             nn.Tanh(),
             nn.Dropout(conf.dropout),
             nn.Linear(d_hidden, num_classes, dtype=conf.dtype)
         )
 
-    def load_ckpt(self, ckpt_files: typing.Sequence[str]) -> None:
+    def load_ckpt(self, *ckpt_files: str) -> None:
         self.load_state_dict(torch.load(
             ckpt_files[0], map_location=torch.device('cpu')), strict=False)
 
     def forward(self, src: torch.Tensor, tgt: torch.Tensor) -> torch.Tensor:
         feats = super().forward_feature(src, tgt)
         return self.fc(feats)
 
@@ -116,7 +115,96 @@
         tgt = self.embedding(tgt)
         if is_batched:
             src[:, 0] = src[:, 0] * goal
         else:
             src[0] = src[0] * goal
         out = self.transformer(src, tgt, tgt_mask=mask, tgt_is_causal=True)
         return self.token_output(out)
+
+
+class AdaMR2(nets.AbsPosEncoderCausal):
+    CONFIG_LARGE = nets.AbsPosEncoderCausalConfig(
+        token_size=512,  # max(spe_merge) = 240
+        max_len=512,
+        d_model=768,
+        nhead=12,
+        num_layers=12,
+        dropout=0.1,
+        dtype=torch.float32
+    )
+
+    CONFIG_BASE = nets.AbsPosEncoderCausalConfig(
+        token_size=512,  # max(spe_merge) = 240
+        max_len=512,
+        d_model=768,
+        nhead=8,
+        num_layers=6,
+        dropout=0.1,
+        dtype=torch.float32
+    )
+
+    def __init__(self, conf: nets.AbsPosEncoderCausalConfig = CONFIG_LARGE) -> None:
+        super().__init__(conf=conf)
+
+    def forward(self, tgt: torch.Tensor) -> torch.Tensor:
+        return super().forward_generation(tgt)
+
+
+class AdaMR2Classifier(AdaMR2):
+    def __init__(self, num_classes: int, conf: nets.AbsPosEncoderDecoderConfig) -> None:
+        super().__init__(conf=conf)
+        d_hidden = conf.d_model // 2
+        self.fc = nn.Sequential(
+            nn.Dropout(conf.dropout),
+            nn.Linear(conf.d_model, d_hidden, dtype=conf.dtype),
+            nn.Tanh(),
+            nn.Dropout(conf.dropout),
+            nn.Linear(d_hidden, num_classes, dtype=conf.dtype)
+        )
+
+    def load_ckpt(self, *ckpt_files: str) -> None:
+        self.load_state_dict(torch.load(
+            ckpt_files[0], map_location=torch.device('cpu')), strict=False)
+
+    def forward(self, tgt: torch.Tensor) -> torch.Tensor:
+        feats = super().forward_feature(tgt)
+        return self.fc(feats)
+
+
+class AdaMR2Regression(AdaMR2):
+    def __init__(self, conf: nets.AbsPosEncoderDecoderConfig) -> None:
+        super().__init__(conf=conf)
+        d_hidden = conf.d_model // 2
+        self.fc = nn.Sequential(
+            nn.Dropout(conf.dropout),
+            nn.Linear(conf.d_model, d_hidden, dtype=conf.dtype),
+            nn.Tanh(),
+            nn.Dropout(conf.dropout),
+            nn.Linear(d_hidden, 1, dtype=conf.dtype)
+        )
+
+    def load_ckpt(self, *ckpt_files: str) -> None:
+        self.load_state_dict(torch.load(
+            ckpt_files[0], map_location=torch.device('cpu')), strict=False)
+
+    def forward(self, tgt: torch.Tensor) -> torch.Tensor:
+        feats = super().forward_feature(tgt)
+        return self.fc(feats)
+
+
+class AdaMR2DistGeneration(AdaMR2):
+    def forward(self, tgt: torch.Tensor) -> torch.Tensor:
+        return super().forward_generation(tgt)
+
+
+class AdaMR2GoalGeneration(AdaMR2):
+    def forward(self, goal: torch.Tensor, tgt: torch.Tensor) -> torch.Tensor:
+        is_batched = tgt.dim() == 2
+        mask = nn.Transformer.generate_square_subsequent_mask(
+            tgt.size(-1), device=tgt.device)
+        tgt = self.embedding(tgt)
+        if is_batched:
+            tgt[:, 0] = tgt[:, 0] * goal
+        else:
+            tgt[0] = tgt[0] * goal
+        out = self.transformer(tgt, mask=mask, is_causal=True)
+        return self.token_output(out)
```

### Comparing `moltx-0.9.8/moltx/nets.py` & `moltx-1.0.0/moltx/nets.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,23 +90,23 @@
         self.token_output = nn.Linear(
             conf.d_model, conf.token_size, bias=False, dtype=conf.dtype)
 
     def load_ckpt(self, *ckpt_files: str) -> None:
         self.load_state_dict(torch.load(
             ckpt_files[0], map_location=torch.device('cpu')))
 
-    def forward_(self, x: torch.Tensor) -> torch.Tensor:
+    def forward_(self, tgt: torch.Tensor) -> torch.Tensor:
         mask = nn.Transformer.generate_square_subsequent_mask(
-            x.size(-1), device=x.device)
-        x = self.embedding(x)
-        return self.transformer(x, mask=mask, is_causal=True)
+            tgt.size(-1), device=tgt.device)
+        tgt = self.embedding(tgt)
+        return self.transformer(tgt, mask=mask, is_causal=True)
 
-    def forward_feature(self, x: torch.Tensor) -> torch.Tensor:
-        out = self.forward_(x)
-        indices = (x > 0).sum(dim=-1, keepdim=True) - 1
+    def forward_feature(self, tgt: torch.Tensor) -> torch.Tensor:
+        out = self.forward_(tgt)
+        indices = (tgt > 0).sum(dim=-1, keepdim=True) - 1
         indices = indices.unsqueeze(-1).repeat(*
-                                               [1 for _ in range(x.dim())], out.shape[-1])
+                                               [1 for _ in range(tgt.dim())], out.shape[-1])
         return torch.gather(input=out, dim=-2, index=indices).squeeze()
 
-    def forward_generation(self, x: torch.Tensor) -> torch.Tensor:
-        out = self.forward_(x)
+    def forward_generation(self, tgt: torch.Tensor) -> torch.Tensor:
+        out = self.forward_(tgt)
         return self.token_output(out)
```

### Comparing `moltx-0.9.8/moltx/pipelines.py` & `moltx-1.0.0/moltx/pipelines.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,127 +25,136 @@
         for i, tk in enumerate(tokens):
             out[i] = tk
         return out.to(self.device)
 
     @torch.no_grad()
     def _greedy_search(self, tgt: torch.Tensor, **kwds: torch.Tensor) -> typing.Tuple[typing.Sequence[int], float]:
         maxlen = self.model.conf.max_len
+        prefixlen = tgt.size(-1)
         eos = self.tokenizer[self.tokenizer.EOS]
         log_prob = torch.zeros(1, device=self.device)
         for _ in range(maxlen - tgt.size(-1)):
             next_log_prob, next_token = self.model(
                 tgt=tgt, **kwds)[-1].log_softmax(-1).max(-1, keepdims=True)  # [token_size] max-> []
             if next_token.item() == eos:
                 break
             log_prob += next_log_prob
             tgt = torch.concat((tgt, next_token), dim=-1)
-        return self.tokenizer.decode(tgt[1:].tolist()), log_prob.exp().item()
+        return self.tokenizer.decode(tgt[prefixlen:].tolist()), log_prob.exp().item()
 
     @torch.no_grad()
     def _random_sample(self, tgt: torch.Tensor, temperature=1, **kwds: torch.Tensor):
         maxlen = self.model.conf.max_len
+        prefixlen = tgt.size(-1)
         eos = self.tokenizer[self.tokenizer.EOS]
         log_prob = torch.zeros(1, device=self.device)
         for _ in range(maxlen - tgt.size(-1)):
             next_log_probs = (self.model(tgt=tgt, **kwds)
                               [-1] / temperature).softmax(-1)  # [token_size]
             rand_num = torch.rand((), device=self.device)
             next_token = (next_log_probs.cumsum(-1) <
                           rand_num).sum(-1, keepdims=True)  # [1]
             if next_token.item() == eos:
                 break
             log_prob += next_log_probs[next_token].log()
             tgt = torch.concat((tgt, next_token), dim=-1)
-        return self.tokenizer.decode(tgt[1:].tolist()), log_prob.exp().item()
+        return self.tokenizer.decode(tgt[prefixlen:].tolist()), log_prob.exp().item()
 
     @torch.no_grad()
-    def _beam_search(self, tgt: torch.Tensor, **kwds: torch.Tensor):
-        # tgt: [beam, seqlen]
+    def _beam_search(self, tgt: torch.Tensor, beam_width: int = 3, **kwds: torch.Tensor):
+        # tgt: [seqlen]
         # when beam_width == 1, beam search is equal to greedy search
-        if tgt.dim() != 2:
-            raise RuntimeError("tgt must be batched!")
         maxlen = self.model.conf.max_len
+        prefixlen = tgt.size(-1)
         eos = self.tokenizer[self.tokenizer.EOS]
         token_size = self.model.conf.token_size
-        beam_width = tgt.size(0)
-        log_probs = torch.zeros(beam_width, 1, device=self.device)
-        meet_end = torch.zeros_like(log_probs, dtype=torch.bool)
+        smiles = []
+        probs = []
+        log_probs, next_tokens = self.model(tgt=tgt, **kwds)[-1].log_softmax(-1).topk(k=beam_width, dim=0)  # [beam]
+        tgt = torch.concat((tgt.unsqueeze(0).repeat(beam_width, 1), next_tokens.unsqueeze(-1)), dim=-1)
+        if 'src' in kwds:
+            kwds['src'] = kwds['src'].unsqueeze(0).repeat(beam_width, 1)
+        log_probs = log_probs.unsqueeze(-1)
         for _ in range(maxlen - tgt.size(-1)):
             next_log_probs = self.model(
                 tgt=tgt, **kwds)[:, -1].log_softmax(-1)  # [beam, token_size]
-            # [beam * tokensize, 1]
-            next_log_probs = (next_log_probs + log_probs).view(-1, 1)
+            next_log_probs = (next_log_probs + log_probs).view(-1, 1)  # [beam * tokensize, 1]
             log_probs, idx = next_log_probs.topk(
                 k=beam_width, dim=0)  # [beam, 1]
             tgt_idx = idx.div(token_size, rounding_mode="floor")  # [beam, 1]
             next_tokens = idx - tgt_idx * token_size  # [beam, 1]
-            meet_end |= next_tokens.eq(eos)
-            tgt = tgt[tgt_idx.squeeze()]
+            meet_end = (next_tokens.squeeze(1).eq(eos).nonzero()).squeeze(1)
+            if meet_end.numel() > 0:
+                beam_width -= meet_end.size(0)
+                probs.extend(log_probs.index_select(0, meet_end).squeeze(1).exp().tolist())
+                end_tgt = tgt.index_select(0, tgt_idx.index_select(0, meet_end).squeeze(1))
+                smiles.extend(map(self.tokenizer.decode, end_tgt[:, prefixlen:].tolist()))
+                if beam_width == 0:
+                    return smiles, probs
+            not_end = (next_tokens.squeeze(1).ne(eos).nonzero()).squeeze(1)
+            log_probs = log_probs.index_select(0, not_end)
+            next_tokens = next_tokens.index_select(0, not_end)
+            tgt = tgt.index_select(0, tgt_idx.index_select(0, not_end).squeeze(1))
             tgt = torch.concat((tgt, next_tokens), dim=-1)
-            if meet_end.all():
-                break
-        probs = log_probs.squeeze().exp().tolist()
-        smiles = []
-        for line in tgt:
-            idx = (line == eos).nonzero(as_tuple=True)[0]
-            if idx.numel() > 0:
-                smiles.append(self.tokenizer.decode(line[1:idx[0]].tolist()))
-            else:
-                smiles.append(self.tokenizer.decode(line[1:].tolist()))
+            if 'src' in kwds:
+                kwds['src'] = kwds['src'].index_select(0, tgt_idx.index_select(0, not_end).squeeze(1))
+        probs.extend(log_probs.squeeze(1).exp().tolist())
+        smiles.extend(map(self.tokenizer.decode, tgt[:, prefixlen:].tolist()))
         return smiles, probs
 
 
 class AdaMR(Base):
 
-    def _model_args(self, s1: str, s2: typing.Optional[str] = None) -> typing.Tuple[torch.Tensor]:
-        src = self._tokenize(s1)
-        if s2 is None:
-            tgt = self._tokenize(self.tokenizer.BOS)
-            return src, tgt
-        tgt = self._tokenize(f"{self.tokenizer.BOS}{s2}")
+    def _model_args(self, smiles: str) -> typing.Tuple[torch.Tensor]:
+        src = self._tokenize(smiles)
+        tgt = self._tokenize(self.tokenizer.BOS)
         return src, tgt
 
     # gentype: greedy, beam
-    def __call__(self, smiles: str, gentype: str = 'greedy') -> typing.Mapping:
+    def __call__(self, smiles: str = "") -> typing.Mapping:
         src, tgt = self._model_args(smiles)
-        m = getattr(self, f"_call_{gentype}")
-        smi, prob = m(src, tgt)
+        if len(smiles) > 0:
+            meth = self._do_canonicalize
+        else:
+            meth = self._do_generate
+        smi, prob = meth(src, tgt)
         return {
             'smiles': smi,
             'probability': prob
         }
 
-    def _call_greedy(self, src: torch.Tensor, tgt: torch.Tensor) -> typing.Mapping:
-        return self._greedy_search(src=src, tgt=tgt)
+    def _do_generate(self, src: torch.Tensor, tgt: torch.Tensor) -> typing.Mapping:
+        return self._random_sample(src=src, tgt=tgt)
 
-    def _call_beam(self, src: torch.Tensor, tgt: torch.Tensor) -> typing.Mapping:
-        beam_k = 3
-        src = src.unsqueeze(0).repeat(beam_k, 1)
-        tgt = tgt.unsqueeze(0).repeat(beam_k, 1)
-        smiles, probs = self._beam_search(src=src, tgt=tgt)
+    def _do_canonicalize(self, src: torch.Tensor, tgt: torch.Tensor) -> typing.Mapping:
+        smiles, probs = self._beam_search(src=src, tgt=tgt, beam_width=3)
         return smiles[0], probs[0]
 
 
 class AdaMRClassifier(AdaMR):
     def _model_args(self, smiles: str) -> typing.Tuple[torch.Tensor]:
-        return super()._model_args(smiles, f"{smiles}{self.tokenizer.EOS}")
+        src = self._tokenize(smiles)
+        tgt = self._tokenize(f"{self.tokenizer.BOS}{smiles}{self.tokenizer.EOS}")
+        return src, tgt
 
     def __call__(self, smiles: str) -> typing.Mapping:
         args = self._model_args(smiles)
         out = self.model(*args)
         prob, label = out.softmax(-1).max(-1)
         return {
             'label': label.item(),
             'probability': prob.item()
         }
 
 
 class AdaMRRegression(AdaMR):
     def _model_args(self, smiles: str) -> typing.Tuple[torch.Tensor]:
-        return super()._model_args(smiles, f"{smiles}{self.tokenizer.EOS}")
+        src = self._tokenize(smiles)
+        tgt = self._tokenize(f"{self.tokenizer.BOS}{smiles}{self.tokenizer.EOS}")
+        return src, tgt
 
     def __call__(self, smiles: str) -> typing.Mapping:
         args = self._model_args(smiles)
         out = self.model(*args)
         return {
             'value': out.item()
         }
@@ -182,7 +191,86 @@
             smi, prob = self._random_sample(goal=goal, src=src, tgt=tgt)
             smis.append(smi)
             probs.append(prob)
         return {
             'smiles': smis,
             'probabilities': probs
         }
+
+
+class AdaMR2(Base):
+
+    # gentype: greedy, beam
+    def __call__(self, smiles: str = "") -> typing.Mapping:
+        tgt = self._tokenize(f"{smiles}{self.tokenizer.BOS}")
+        if len(smiles) > 0:
+            meth = self._do_canonicalize
+        else:
+            meth = self._do_generate
+
+        smi, prob = meth(tgt)
+        return {
+            'smiles': smi,
+            'probability': prob
+        }
+
+    def _do_generate(self, tgt: torch.Tensor) -> typing.Mapping:
+        return self._random_sample(tgt=tgt)
+
+    def _do_canonicalize(self, tgt: torch.Tensor) -> typing.Mapping:
+        smiles, probs = self._beam_search(tgt=tgt)
+        return smiles[0], probs[0]
+
+
+class AdaMR2Classifier(AdaMR):
+
+    def __call__(self, smiles: str) -> typing.Mapping:
+        tgt = self._tokenize(f"{self.tokenizer.BOS}{smiles}{self.tokenizer.EOS}")
+        out = self.model(tgt)
+        prob, label = out.softmax(-1).max(-1)
+        return {
+            'label': label.item(),
+            'probability': prob.item()
+        }
+
+
+class AdaMR2Regression(AdaMR):
+
+    def __call__(self, smiles: str) -> typing.Mapping:
+        tgt = self._tokenize(f"{self.tokenizer.BOS}{smiles}{self.tokenizer.EOS}")
+        out = self.model(tgt)
+        return {
+            'value': out.item()
+        }
+
+
+class AdaMR2DistGeneration(AdaMR):
+
+    def __call__(self, k: int = 1) -> typing.Mapping:
+        assert k <= 10
+        tgt = self._tokenize(f"{self.tokenizer.CLS}{self.tokenizer.BOS}")
+        smis, probs = [], []
+        for _ in range(k):
+            smi, prob = self._random_sample(tgt=tgt)
+            smis.append(smi)
+            probs.append(prob)
+        return {
+            'smiles': smis,
+            'probabilities': probs
+        }
+
+
+class AdaMR2GoalGeneration(AdaMR):
+
+    def __call__(self, goal: float, k: int = 1) -> typing.Mapping:
+        assert k <= 10
+        tgt = self._tokenize(f"{self.tokenizer.CLS}{self.tokenizer.BOS}")
+        goal = torch.tensor(goal, device=self.device)
+        smis, probs = [], []
+        for _ in range(k):
+            smi, prob = self._random_sample(goal=goal, tgt=tgt)
+            smis.append(smi)
+            probs.append(prob)
+        return {
+            'smiles': smis,
+            'probabilities': probs
+        }
```

### Comparing `moltx-0.9.8/moltx/tokenizers.py` & `moltx-1.0.0/moltx/tokenizers.py`

 * *Files identical despite different names*

### Comparing `moltx-0.9.8/moltx.egg-info/PKG-INFO` & `moltx-1.0.0/moltx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: moltx
-Version: 0.9.8
+Version: 1.0.0
 Summary: Molcule Transformer X Model
 Author: Michael Ding
 Author-email: yandy.ding@gmail.com
-License: Apache-2.0
 Keywords: molcule,AI,deep learning,transformer
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rdkit~=2023.9.1
 Requires-Dist: torch~=2.2.0
 
 # MolTx
```

### Comparing `moltx-0.9.8/moltx.egg-info/SOURCES.txt` & `moltx-1.0.0/moltx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moltx-0.9.8/tests/test_datasets.py` & `moltx-1.0.0/tests/test_datasets.py`

 * *Files 22% similar despite different names*

```diff
@@ -61,7 +61,63 @@
     smiles = ["CC[N+]CCBr", "c1ccc1"]
     goals = [1.1, 1.2]
     goal, src, tgt, out = ds(smiles, goals)
     assert goal.shape == (2, 1)
     assert src.shape == (2, 1)
     assert tgt.shape == (2, 7)
     assert out.shape == (2, 7)
+
+def test_AdaMR2(tokenizer):
+    ds = datasets.AdaMR2(tokenizer)
+    s1 = ["CC[N+]CCBr", "c1ccccc1"]
+    s2 = ["CC[N+]CCBr"]
+    with pytest.raises(RuntimeError):
+        ds(s1, s2)
+    s2 = ["CC[N+](C)(C)Br", ""]
+    tgt, out = ds(s1, s2)
+    assert tgt.shape == out.shape
+    assert tgt.size(0) == 2 and tgt.size(1) == 17
+    assert tgt[0, 7:].eq(out[0, 6:-1]).all()
+    assert out[0, :6].eq(0).all()
+
+def test_AdaMR2Classifier(tokenizer):
+    ds = datasets.AdaMR2Classifier(tokenizer)
+    smiles = ["CC[N+]CCBr", "Cc1ccc1"]
+    labels = [1, 2]
+    with pytest.raises(RuntimeError):
+        ds(smiles, labels[:1])
+    tgt, out = ds(smiles, labels)
+    assert tgt.shape == (2, 9)
+    assert out.shape == (2, 1)
+
+def test_AdaMR2Regression(tokenizer):
+    ds = datasets.AdaMR2Regression(tokenizer)
+    smiles = ["CC[N+]CCBr", "Cc1ccc1"]
+    values = [1.1, 1.2]
+    with pytest.raises(RuntimeError):
+        ds(smiles, values[:1])
+    tgt, out = ds(smiles, values)
+    assert tgt.shape == (2, 9)
+    assert out.shape == (2, 1)
+
+
+def test_AdaMR2DistGeneration(tokenizer):
+    ds = datasets.AdaMR2DistGeneration(tokenizer)
+    smiles = ["CC[N+]CCBr", "c1ccc1"]
+    tgt, out = ds(smiles)
+    assert tgt.shape == (2, 8)
+    assert out.shape == (2, 8)
+    assert out[0, 0].item() == 0
+    assert tgt[0, 2:].eq(out[0, 1:-1]).all()
+
+
+def test_AdaMR2GoalGeneration(tokenizer):
+    ds = datasets.AdaMR2GoalGeneration(tokenizer)
+    smiles = ["CC[N+]CCBr", "c1ccc1"]
+    goals = [1.1, 1.2]
+    goal, tgt, out = ds(smiles, goals)
+    assert goal.shape == (2, 1)
+    assert tgt.shape == (2, 8)
+    assert out.shape == (2, 8)
+    assert out[0, 0].item() == 0
+    assert tgt[0, 2:].eq(out[0, 1:-1]).all()
+
```

### Comparing `moltx-0.9.8/tests/test_nets.py` & `moltx-1.0.0/tests/test_nets.py`

 * *Files identical despite different names*

### Comparing `moltx-0.9.8/tests/test_pipelines.py` & `moltx-1.0.0/tests/test_pipelines.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,111 @@
 import pytest
-from moltx import pipelines, models
+from moltx import pipelines, models, nets
 
 
-def test_AdaMR(tokenizer, model_conf):
-    pipeline = pipelines.AdaMR(tokenizer, models.AdaMR(model_conf))
+@pytest.fixture
+def adamr_conf():
+    return nets.AbsPosEncoderDecoderConfig(
+        token_size=16, max_len=32, d_model=8, nhead=2,
+        num_encoder_layers=2, num_decoder_layers=2)
+
+
+@pytest.fixture
+def adamr2_conf():
+    return nets.AbsPosEncoderCausalConfig(
+        token_size=16, max_len=32, d_model=8, nhead=2,num_layers=2)
+
+
+def test_AdaMR(tokenizer, adamr_conf):
+    pipeline = pipelines.AdaMR(tokenizer, models.AdaMR(adamr_conf))
     out = pipeline("CC[N+](C)(C)Br")
     assert 'smiles' in out and 'probability' in out
     assert isinstance(out['smiles'], str)
 
-    out = pipeline("CC[N+](C)(C)Br", gentype='beam')
+    out = pipeline("")
     assert 'smiles' in out and 'probability' in out
     assert isinstance(out['smiles'], str)
 
 
-def test_AdaMRClassifier(tokenizer, model_conf):
+def test_AdaMRClassifier(tokenizer, adamr_conf):
     pipeline = pipelines.AdaMRClassifier(
-        tokenizer, models.AdaMRClassifier(num_classes=2, conf=model_conf))
+        tokenizer, models.AdaMRClassifier(num_classes=2, conf=adamr_conf))
     out = pipeline("CC[N+](C)(C)Br")
     assert 'label' in out and 'probability' in out
     assert isinstance(out['label'], int) and isinstance(out['probability'], float)
     assert out['label'] in range(2)
 
 
-def test_AdaMRRegression(tokenizer, model_conf):
+def test_AdaMRRegression(tokenizer, adamr_conf):
     pipeline = pipelines.AdaMRRegression(
-        tokenizer, models.AdaMRRegression(conf=model_conf))
+        tokenizer, models.AdaMRRegression(conf=adamr_conf))
     out = pipeline("CC[N+](C)(C)Br")
     assert 'value' in out
     assert isinstance(out['value'], float)
 
 
-def test_AdaMRDistGeneration(tokenizer, model_conf):
+def test_AdaMRDistGeneration(tokenizer, adamr_conf):
     pipeline = pipelines.AdaMRDistGeneration(
-        tokenizer, models.AdaMRDistGeneration(model_conf))
+        tokenizer, models.AdaMRDistGeneration(adamr_conf))
     out = pipeline(k=1)
     assert 'smiles' in out and 'probabilities' in out
     assert isinstance(out['smiles'], list) and len(out['smiles']) == 1 and isinstance(out['smiles'][0], str)
     assert isinstance(out['probabilities'], list) and len(
         out['probabilities']) == 1
 
 
-def test_AdaMRGoalGeneration(tokenizer, model_conf):
+def test_AdaMRGoalGeneration(tokenizer, adamr_conf):
     pipeline = pipelines.AdaMRGoalGeneration(
-        tokenizer, models.AdaMRGoalGeneration(model_conf))
+        tokenizer, models.AdaMRGoalGeneration(adamr_conf))
+    out = pipeline(0.48, k=2)
+    assert 'smiles' in out and 'probabilities' in out
+    assert isinstance(out['smiles'], list) and len(out['smiles']) == 2 and isinstance(out['smiles'][0], str)
+    assert isinstance(out['probabilities'], list) and len(
+        out['probabilities']) == 2
+
+
+def test_AdaMR2(tokenizer, adamr2_conf):
+    pipeline = pipelines.AdaMR2(tokenizer, models.AdaMR2(adamr2_conf))
+    out = pipeline("CC[N+](C)(C)Br")
+    assert 'smiles' in out and 'probability' in out
+    assert isinstance(out['smiles'], str)
+
+    out = pipeline("")
+    assert 'smiles' in out and 'probability' in out
+    assert isinstance(out['smiles'], str)
+
+
+def test_AdaMR2Classifier(tokenizer, adamr2_conf):
+    pipeline = pipelines.AdaMR2Classifier(
+        tokenizer, models.AdaMR2Classifier(num_classes=2, conf=adamr2_conf))
+    out = pipeline("CC[N+](C)(C)Br")
+    assert 'label' in out and 'probability' in out
+    assert isinstance(out['label'], int) and isinstance(out['probability'], float)
+    assert out['label'] in range(2)
+
+
+def test_AdaMR2Regression(tokenizer, adamr2_conf):
+    pipeline = pipelines.AdaMR2Regression(
+        tokenizer, models.AdaMR2Regression(conf=adamr2_conf))
+    out = pipeline("CC[N+](C)(C)Br")
+    assert 'value' in out
+    assert isinstance(out['value'], float)
+
+
+def test_AdaMR2DistGeneration(tokenizer, adamr2_conf):
+    pipeline = pipelines.AdaMR2DistGeneration(
+        tokenizer, models.AdaMR2DistGeneration(adamr2_conf))
+    out = pipeline(k=1)
+    assert 'smiles' in out and 'probabilities' in out
+    assert isinstance(out['smiles'], list) and len(out['smiles']) == 1 and isinstance(out['smiles'][0], str)
+    assert isinstance(out['probabilities'], list) and len(
+        out['probabilities']) == 1
+
+
+def test_AdaMR2GoalGeneration(tokenizer, adamr2_conf):
+    pipeline = pipelines.AdaMR2GoalGeneration(
+        tokenizer, models.AdaMR2GoalGeneration(adamr2_conf))
     out = pipeline(0.48, k=2)
     assert 'smiles' in out and 'probabilities' in out
     assert isinstance(out['smiles'], list) and len(out['smiles']) == 2 and isinstance(out['smiles'][0], str)
     assert isinstance(out['probabilities'], list) and len(
         out['probabilities']) == 2
```

### Comparing `moltx-0.9.8/tests/test_tokenizer.py` & `moltx-1.0.0/tests/test_tokenizer.py`

 * *Files identical despite different names*

