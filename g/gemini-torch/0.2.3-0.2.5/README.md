# Comparing `tmp/gemini_torch-0.2.3.tar.gz` & `tmp/gemini_torch-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemini_torch-0.2.3.tar", max compression
+gzip compressed data, was "gemini_torch-0.2.5.tar", max compression
```

## Comparing `gemini_torch-0.2.3.tar` & `gemini_torch-0.2.5.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1074 2023-08-29 00:11:15.714548 gemini_torch-0.2.3/LICENSE
--rw-r--r--   0        0        0     7203 2024-02-20 02:18:48.699403 gemini_torch-0.2.3/README.md
--rw-r--r--   0        0        0      303 2024-02-20 19:26:21.888466 gemini_torch-0.2.3/gemini_torch/__init__.py
--rw-r--r--   0        0        0     6116 2024-02-20 19:22:47.864741 gemini_torch-0.2.3/gemini_torch/long_gemini.py
--rw-r--r--   0        0        0     6577 2024-02-20 19:22:44.999940 gemini_torch-0.2.3/gemini_torch/model.py
--rw-r--r--   0        0        0     5248 2024-02-20 02:18:48.849702 gemini_torch-0.2.3/gemini_torch/tokenizer.py
--rw-r--r--   0        0        0    52008 2024-02-20 02:18:53.601422 gemini_torch-0.2.3/gemini_torch/transformer.py
--rw-r--r--   0        0        0     1333 2024-02-20 21:06:52.842834 gemini_torch-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     8106 1970-01-01 00:00:00.000000 gemini_torch-0.2.3/setup.py
--rw-r--r--   0        0        0     8302 1970-01-01 00:00:00.000000 gemini_torch-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-08-29 00:11:15.714548 gemini_torch-0.2.5/LICENSE
+-rw-r--r--   0        0        0     7991 2024-05-07 14:09:40.722698 gemini_torch-0.2.5/README.md
+-rw-r--r--   0        0        0      303 2024-02-20 19:26:21.888466 gemini_torch-0.2.5/gemini_torch/__init__.py
+-rw-r--r--   0        0        0     6242 2024-05-07 14:09:40.723669 gemini_torch-0.2.5/gemini_torch/long_gemini.py
+-rw-r--r--   0        0        0     6577 2024-02-20 19:22:44.999940 gemini_torch-0.2.5/gemini_torch/model.py
+-rw-r--r--   0        0        0     2407 2024-05-07 14:09:40.724547 gemini_torch-0.2.5/gemini_torch/omni_modality_processor.py
+-rw-r--r--   0        0        0     5248 2024-02-20 02:18:48.849702 gemini_torch-0.2.5/gemini_torch/tokenizer.py
+-rw-r--r--   0        0        0    52008 2024-02-20 02:18:53.601422 gemini_torch-0.2.5/gemini_torch/transformer.py
+-rw-r--r--   0        0        0     1333 2024-05-07 17:43:31.748769 gemini_torch-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     8923 1970-01-01 00:00:00.000000 gemini_torch-0.2.5/setup.py
+-rw-r--r--   0        0        0     9090 1970-01-01 00:00:00.000000 gemini_torch-0.2.5/PKG-INFO
```

### Comparing `gemini_torch-0.2.3/LICENSE` & `gemini_torch-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gemini_torch-0.2.3/README.md` & `gemini_torch-0.2.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -111,14 +111,43 @@
 text = tokenize(texts)
 logits = model(text)
 text = detokenize(logits)
 ```
 ------
 
 
+## LongGemini
+An implementation of Gemini with Ring Attention, no multi-modality processing yet.
+
+```python
+import torch
+from gemini_torch import LongGemini
+
+# Text tokens
+x = torch.randint(0, 10000, (1, 1024))
+
+# Create an instance of the LongGemini model
+model = LongGemini(
+    dim=512,  # Dimension of the input tensor
+    depth=32,  # Number of transformer blocks
+    dim_head=128,  # Dimension of the query, key, and value vectors
+    long_gemini_depth=9,  # Number of long gemini transformer blocks
+    heads=24,  # Number of attention heads
+    qk_norm=True,  # Whether to apply layer normalization to query and key vectors
+    ring_seq_size=512,  # The size of the ring sequence
+)
+
+# Apply the model to the input tensor
+out = model(x)
+
+# Print the output tensor
+print(out)
+
+```
+
 
 ## Tokenizer
 - Sentencepiece, tokenizer
 - We're using the same tokenizer as LLAMA with special tokens denoting the beginning and end of the multi modality tokens.
 - Does not fully process img, audio, or videos now we need help on that
 
 ```python
```

### Comparing `gemini_torch-0.2.3/gemini_torch/long_gemini.py` & `gemini_torch-0.2.5/gemini_torch/long_gemini.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import torch
 from ring_attention_pytorch import RingAttention
 from torch import Tensor, nn
 from zeta.nn import FeedForward, OutputHead
 
 
 def exists(val):
     return val is not None
@@ -88,15 +89,15 @@
         Returns:
             Tensor: The output tensor.
 
         """
         x = self.norm(x)
 
         # Attention
-        x = self.attn(x)
+        x = self.attn(x) + x
 
         # Feedforward
         x = self.ffn(x) + x
 
         return x
 
 
@@ -166,14 +167,17 @@
                 for _ in range(long_gemini_depth)
             ]
         )
 
         # Embedding layer for the model
         self.embed = nn.Embedding(num_tokens, dim)
 
+        # Norm
+        self.norm = nn.LayerNorm(dim)
+
     def forward(
         self,
         text: Tensor,
         *args,
         **kwargs,
     ):
         """
@@ -185,13 +189,16 @@
             **kwargs: Arbitrary keyword arguments.
 
         Returns:
             Tensor: Output tensor.
         """
         # Text embedding
         x = self.embed(text)
+        x = self.norm(x)
 
         # Apply the layers
         for layer in self.layers:
             x = layer(x)
+            x = self.norm(x)
 
         return self.output_head(x)
+
```

### Comparing `gemini_torch-0.2.3/gemini_torch/model.py` & `gemini_torch-0.2.5/gemini_torch/model.py`

 * *Files identical despite different names*

### Comparing `gemini_torch-0.2.3/gemini_torch/tokenizer.py` & `gemini_torch-0.2.5/gemini_torch/tokenizer.py`

 * *Files identical despite different names*

### Comparing `gemini_torch-0.2.3/gemini_torch/transformer.py` & `gemini_torch-0.2.5/gemini_torch/transformer.py`

 * *Files identical despite different names*

### Comparing `gemini_torch-0.2.3/pyproject.toml` & `gemini_torch-0.2.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "gemini-torch"
-version = "0.2.3"
+version = "0.2.5"
 description = "Gemini - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/kyegomez/Gemini"
 documentation = "https://github.com/kyegomez/Gemini"  # Add this if you have documentation.
 readme = "README.md"  # Assuming you have a README.md
 repository = "https://github.com/kyegomez/Gemini"
@@ -28,15 +28,15 @@
 einops = "*"
 torchvision = "*"
 sentencepiece = "*"
 pytest = "*"
 ring-attention-pytorch = "*"
 
 [tool.poetry.group.lint.dependencies]
-ruff = ">=0.1.6,<0.3.0"
+ruff = ">=0.1.6,<0.4.0"
 types-toml = "^0.10.8.1"
 types-redis = "^4.3.21.6"
 types-pytz = ">=2023.3,<2025.0"
 black = ">=23.1,<25.0"
 types-chardet = "^5.0.4.6"
 mypy-protobuf = "^3.0.0"
```

### Comparing `gemini_torch-0.2.3/setup.py` & `gemini_torch-0.2.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,17 +14,17 @@
  'sentencepiece',
  'torch',
  'torchvision',
  'zetascale']
 
 setup_kwargs = {
     'name': 'gemini-torch',
-    'version': '0.2.3',
+    'version': '0.2.5',
     'description': 'Gemini - Pytorch',
-    'long_description': '[![Multi-Modality](agorabanner.png)](https://discord.gg/qUtxnK2NMf)\n\n# Gemini\n\n![gemini](gemini.png)\n\nThe open source implementation of Gemini, the model that will "eclipse ChatGPT", it seems to work by directly taking in all modalities all at once into a transformer with special decoders for text or img generation!\n\n[Join the Agora discord channel to help with the implementation!](https://discord.gg/CMDpRxCV8g) and [Here is the project board:](https://github.com/users/kyegomez/projects/11/views/1)\n\nThe input sequences for Gemini consist of texts, audio, images, and videos. These inputs are transformed into tokens, which are then processed by a transformer. Subsequently, conditional decoding takes place to generate image outputs. Interestingly, the architecture of Gemini bears resemblance to Fuyu\'s architecture but is expanded to encompass multiple modalities. Instead of utilizing a visual transformer (vit) encoder, Gemini simply feeds image embeddings directly into the transformer. For Gemini, the token inputs will likely be indicated by special modality tokens such as [IMG], <img>, [AUDIO], or <audio>. Codi, a component of Gemini, also employs conditional generation and makes use of the tokenized outputs. To implement this model effectively, I intend to initially focus on the image embeddings to ensure their smooth integration. Subsequently, I will proceed with incorporating audio embeddings and then video embeddings.\n\n# Install\n`pip3 install gemini-torch`\n\n\n## Usage\n\n### Gemini Transformer Usage\n- Base transformer\n- Multi Grouped Query Attn / flash attn\n- rope\n- alibi\n- xpos\n- qk norm\n- no pos embeds\n- kv cache\n\n```python\nimport torch\n\nfrom gemini_torch.model import Gemini\n\n# Initialize model with smaller dimensions\nmodel = Gemini(\n    num_tokens=50432,\n    max_seq_len=4096,  # Reduced from 8192\n    dim=1280,  # Reduced from 2560\n    depth=16,  # Reduced from 32\n    dim_head=64,  # Reduced from 128\n    heads=12,  # Reduced from 24\n    use_abs_pos_emb=False,\n    attn_flash=True,\n    attn_kv_heads=2,\n    qk_norm=True,\n    attn_qk_norm=True,\n    attn_qk_norm_dim_scale=True,\n)\n\n# Text shape: [batch, seq_len, dim]\ntext = torch.randint(0, 50432, (1, 4096))  # Reduced seq_len from 8192\n\n# Apply model to text\ny = model(\n    text,\n)\n\n# Output shape: [batch, seq_len, dim]\nprint(y)\n```\n--------\n\n### Full Multi-Modal Gemini \n- Processes images and audio through a series of reshapes\n- Ready to train for production grade usage\n- Hyper optimized with flash attention, qk norm, and other methods\n\n```python\nimport torch\n\nfrom gemini_torch.model import Gemini\n\n# Initialize model with smaller dimensions\nmodel = Gemini(\n    num_tokens=10000,  # Reduced from 50432\n    max_seq_len=1024,  # Reduced from 4096\n    dim=320,  # Reduced from 1280\n    depth=8,  # Reduced from 16\n    dim_head=32,  # Reduced from 64\n    heads=6,  # Reduced from 12\n    use_abs_pos_emb=False,\n    attn_flash=True,\n    attn_kv_heads=2,\n    qk_norm=True,\n    attn_qk_norm=True,\n    attn_qk_norm_dim_scale=True,\n    post_fusion_norm=True,\n    post_modal_transform_norm=True,\n)\n\n# Text shape: [batch, seq_len, dim]\ntext = torch.randint(0, 10000, (1, 1024))  # Reduced seq_len from 4096\n\n# Img shape: [batch, channels, height, width]\nimg = torch.randn(1, 3, 64, 64)  # Reduced height and width from 128\n\n# Audio shape: [batch, audio_seq_len, dim]\naudio = torch.randn(1, 32)  # Reduced audio_seq_len from 64\n\n# Apply model to text and img\ny, _ = model(text=text, img=img, audio=audio)\n\n# Output shape: [batch, seq_len, dim]\nprint(y)\nprint(y.shape)\n\n\n# After much training\nmodel.eval()\n\ntext = tokenize(texts)\nlogits = model(text)\ntext = detokenize(logits)\n```\n------\n\n\n\n## Tokenizer\n- Sentencepiece, tokenizer\n- We\'re using the same tokenizer as LLAMA with special tokens denoting the beginning and end of the multi modality tokens.\n- Does not fully process img, audio, or videos now we need help on that\n\n```python\nfrom gemini_torch.tokenizer import MultimodalSentencePieceTokenizer\n\n# Example usage\ntokenizer_name = "hf-internal-testing/llama-tokenizer"\ntokenizer = MultimodalSentencePieceTokenizer(tokenizer_name=tokenizer_name)\n\n# Encoding and decoding examples\nencoded_audio = tokenizer.encode("Audio description", modality="audio")\ndecoded_audio = tokenizer.decode(encoded_audio)\n\nprint("Encoded audio:", encoded_audio)\nprint("Decoded audio:", decoded_audio)\n```\n\n\n\n# References\n* Combine Reinforcment learning with modular pretrained transformer, multi-modal capabilities, image, audio, \n* self improving mechanisms like robocat\n* PPO? or MPO\n* get good at backtracking and exploring alternative paths\n* speculative decoding\n* Algorithm of Thoughts\n* RLHF\n* [Gemini Report](https://storage.googleapis.com/deepmind-media/gemini/gemini_1_report.pdf)\n* [Gemini Landing Page](https://deepmind.google/technologies/gemini/#introduction)\n\n\n# Todo\n\n- [ ] [Check out the project board for more todos](https://github.com/users/kyegomez/projects/11/views/1)\n\n\n- [x] Implement the img feature embedder and align imgs with text and pass into transformer: ```Gemini models are trained to accommodate textual input interleaved with a wide variety of audio and visual inputs, such as natural images, charts, screenshots, PDFs, and videos, and they can produce\ntext and image outputs (see Figure 2). The visual encoding of Gemini models is inspired by our own\nfoundational work on Flamingo (Alayrac et al., 2022), CoCa (Yu et al., 2022a), and PaLI (Chen et al.,\n2022), with the important distinction that the models are multimodal from the beginning and can\nnatively output images using discrete image tokens (Ramesh et al., 2021; Yu et al., 2022b).```\n\n- [x] Implement the audio processing using USM by Google:```In addition, Gemini can directly ingest audio signals at\n16kHz from Universal Speech Model (USM) (Zhang et al., 2023) features. This enables the model to\ncapture nuances that are typically lost when the audio is naively mapped to a text input (for example,\nsee audio understanding demo on the website).```\n\n\n- [ ] Video Processing Technique: "\nVideo understanding is accomplished by encoding the video as a sequence of frames in the large\ncontext window. Video frames or images can be interleaved naturally with text or audio as part of the\nmodel input"\n\n- [ ] Prompting Technique: ``` We find Gemini Ultra achieves highest\naccuracy when used in combination with a chain-of-thought prompting approach (Wei et al., 2022)\nthat accounts for model uncertainty. The model produces a chain of thought with k samples, for\nexample 8 or 32. If there is a consensus above a preset threshold (selected based on the validation\nsplit), it selects this answer, otherwise it reverts to a greedy sample based on maximum likelihood\nchoice without chain of thought. We refer the reader to appendix for a detailed breakdown of how\nthis approach compares with only chain-of-thought prompting or only greedy sampling.```\n\n\n\n- [ ] Train a 1.8B + 3.25 Model: ```Nano-1 and Nano-2 model sizes are only 1.8B and 3.25B\nparameters respectively. Despite their size, they show exceptionally strong performance on factuality,\ni.e. retrieval-related tasks, and significant performance on reasoning, STEM, coding, multimodal and```\n',
+    'long_description': '[![Multi-Modality](agorabanner.png)](https://discord.gg/qUtxnK2NMf)\n\n# Gemini\n\n![gemini](gemini.png)\n\nThe open source implementation of Gemini, the model that will "eclipse ChatGPT", it seems to work by directly taking in all modalities all at once into a transformer with special decoders for text or img generation!\n\n[Join the Agora discord channel to help with the implementation!](https://discord.gg/CMDpRxCV8g) and [Here is the project board:](https://github.com/users/kyegomez/projects/11/views/1)\n\nThe input sequences for Gemini consist of texts, audio, images, and videos. These inputs are transformed into tokens, which are then processed by a transformer. Subsequently, conditional decoding takes place to generate image outputs. Interestingly, the architecture of Gemini bears resemblance to Fuyu\'s architecture but is expanded to encompass multiple modalities. Instead of utilizing a visual transformer (vit) encoder, Gemini simply feeds image embeddings directly into the transformer. For Gemini, the token inputs will likely be indicated by special modality tokens such as [IMG], <img>, [AUDIO], or <audio>. Codi, a component of Gemini, also employs conditional generation and makes use of the tokenized outputs. To implement this model effectively, I intend to initially focus on the image embeddings to ensure their smooth integration. Subsequently, I will proceed with incorporating audio embeddings and then video embeddings.\n\n# Install\n`pip3 install gemini-torch`\n\n\n## Usage\n\n### Gemini Transformer Usage\n- Base transformer\n- Multi Grouped Query Attn / flash attn\n- rope\n- alibi\n- xpos\n- qk norm\n- no pos embeds\n- kv cache\n\n```python\nimport torch\n\nfrom gemini_torch.model import Gemini\n\n# Initialize model with smaller dimensions\nmodel = Gemini(\n    num_tokens=50432,\n    max_seq_len=4096,  # Reduced from 8192\n    dim=1280,  # Reduced from 2560\n    depth=16,  # Reduced from 32\n    dim_head=64,  # Reduced from 128\n    heads=12,  # Reduced from 24\n    use_abs_pos_emb=False,\n    attn_flash=True,\n    attn_kv_heads=2,\n    qk_norm=True,\n    attn_qk_norm=True,\n    attn_qk_norm_dim_scale=True,\n)\n\n# Text shape: [batch, seq_len, dim]\ntext = torch.randint(0, 50432, (1, 4096))  # Reduced seq_len from 8192\n\n# Apply model to text\ny = model(\n    text,\n)\n\n# Output shape: [batch, seq_len, dim]\nprint(y)\n```\n--------\n\n### Full Multi-Modal Gemini \n- Processes images and audio through a series of reshapes\n- Ready to train for production grade usage\n- Hyper optimized with flash attention, qk norm, and other methods\n\n```python\nimport torch\n\nfrom gemini_torch.model import Gemini\n\n# Initialize model with smaller dimensions\nmodel = Gemini(\n    num_tokens=10000,  # Reduced from 50432\n    max_seq_len=1024,  # Reduced from 4096\n    dim=320,  # Reduced from 1280\n    depth=8,  # Reduced from 16\n    dim_head=32,  # Reduced from 64\n    heads=6,  # Reduced from 12\n    use_abs_pos_emb=False,\n    attn_flash=True,\n    attn_kv_heads=2,\n    qk_norm=True,\n    attn_qk_norm=True,\n    attn_qk_norm_dim_scale=True,\n    post_fusion_norm=True,\n    post_modal_transform_norm=True,\n)\n\n# Text shape: [batch, seq_len, dim]\ntext = torch.randint(0, 10000, (1, 1024))  # Reduced seq_len from 4096\n\n# Img shape: [batch, channels, height, width]\nimg = torch.randn(1, 3, 64, 64)  # Reduced height and width from 128\n\n# Audio shape: [batch, audio_seq_len, dim]\naudio = torch.randn(1, 32)  # Reduced audio_seq_len from 64\n\n# Apply model to text and img\ny, _ = model(text=text, img=img, audio=audio)\n\n# Output shape: [batch, seq_len, dim]\nprint(y)\nprint(y.shape)\n\n\n# After much training\nmodel.eval()\n\ntext = tokenize(texts)\nlogits = model(text)\ntext = detokenize(logits)\n```\n------\n\n\n## LongGemini\nAn implementation of Gemini with Ring Attention, no multi-modality processing yet.\n\n```python\nimport torch\nfrom gemini_torch import LongGemini\n\n# Text tokens\nx = torch.randint(0, 10000, (1, 1024))\n\n# Create an instance of the LongGemini model\nmodel = LongGemini(\n    dim=512,  # Dimension of the input tensor\n    depth=32,  # Number of transformer blocks\n    dim_head=128,  # Dimension of the query, key, and value vectors\n    long_gemini_depth=9,  # Number of long gemini transformer blocks\n    heads=24,  # Number of attention heads\n    qk_norm=True,  # Whether to apply layer normalization to query and key vectors\n    ring_seq_size=512,  # The size of the ring sequence\n)\n\n# Apply the model to the input tensor\nout = model(x)\n\n# Print the output tensor\nprint(out)\n\n```\n\n\n## Tokenizer\n- Sentencepiece, tokenizer\n- We\'re using the same tokenizer as LLAMA with special tokens denoting the beginning and end of the multi modality tokens.\n- Does not fully process img, audio, or videos now we need help on that\n\n```python\nfrom gemini_torch.tokenizer import MultimodalSentencePieceTokenizer\n\n# Example usage\ntokenizer_name = "hf-internal-testing/llama-tokenizer"\ntokenizer = MultimodalSentencePieceTokenizer(tokenizer_name=tokenizer_name)\n\n# Encoding and decoding examples\nencoded_audio = tokenizer.encode("Audio description", modality="audio")\ndecoded_audio = tokenizer.decode(encoded_audio)\n\nprint("Encoded audio:", encoded_audio)\nprint("Decoded audio:", decoded_audio)\n```\n\n\n\n# References\n* Combine Reinforcment learning with modular pretrained transformer, multi-modal capabilities, image, audio, \n* self improving mechanisms like robocat\n* PPO? or MPO\n* get good at backtracking and exploring alternative paths\n* speculative decoding\n* Algorithm of Thoughts\n* RLHF\n* [Gemini Report](https://storage.googleapis.com/deepmind-media/gemini/gemini_1_report.pdf)\n* [Gemini Landing Page](https://deepmind.google/technologies/gemini/#introduction)\n\n\n# Todo\n\n- [ ] [Check out the project board for more todos](https://github.com/users/kyegomez/projects/11/views/1)\n\n\n- [x] Implement the img feature embedder and align imgs with text and pass into transformer: ```Gemini models are trained to accommodate textual input interleaved with a wide variety of audio and visual inputs, such as natural images, charts, screenshots, PDFs, and videos, and they can produce\ntext and image outputs (see Figure 2). The visual encoding of Gemini models is inspired by our own\nfoundational work on Flamingo (Alayrac et al., 2022), CoCa (Yu et al., 2022a), and PaLI (Chen et al.,\n2022), with the important distinction that the models are multimodal from the beginning and can\nnatively output images using discrete image tokens (Ramesh et al., 2021; Yu et al., 2022b).```\n\n- [x] Implement the audio processing using USM by Google:```In addition, Gemini can directly ingest audio signals at\n16kHz from Universal Speech Model (USM) (Zhang et al., 2023) features. This enables the model to\ncapture nuances that are typically lost when the audio is naively mapped to a text input (for example,\nsee audio understanding demo on the website).```\n\n\n- [ ] Video Processing Technique: "\nVideo understanding is accomplished by encoding the video as a sequence of frames in the large\ncontext window. Video frames or images can be interleaved naturally with text or audio as part of the\nmodel input"\n\n- [ ] Prompting Technique: ``` We find Gemini Ultra achieves highest\naccuracy when used in combination with a chain-of-thought prompting approach (Wei et al., 2022)\nthat accounts for model uncertainty. The model produces a chain of thought with k samples, for\nexample 8 or 32. If there is a consensus above a preset threshold (selected based on the validation\nsplit), it selects this answer, otherwise it reverts to a greedy sample based on maximum likelihood\nchoice without chain of thought. We refer the reader to appendix for a detailed breakdown of how\nthis approach compares with only chain-of-thought prompting or only greedy sampling.```\n\n\n\n- [ ] Train a 1.8B + 3.25 Model: ```Nano-1 and Nano-2 model sizes are only 1.8B and 3.25B\nparameters respectively. Despite their size, they show exceptionally strong performance on factuality,\ni.e. retrieval-related tasks, and significant performance on reasoning, STEM, coding, multimodal and```\n',
     'author': 'Kye Gomez',
     'author_email': 'kye@apac.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kyegomez/Gemini',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `gemini_torch-0.2.3/PKG-INFO` & `gemini_torch-0.2.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemini-torch
-Version: 0.2.3
+Version: 0.2.5
 Summary: Gemini - Pytorch
 Home-page: https://github.com/kyegomez/Gemini
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Author: Kye Gomez
 Author-email: kye@apac.ai
 Requires-Python: >=3.9,<4.0
@@ -141,14 +141,43 @@
 text = tokenize(texts)
 logits = model(text)
 text = detokenize(logits)
 ```
 ------
 
 
+## LongGemini
+An implementation of Gemini with Ring Attention, no multi-modality processing yet.
+
+```python
+import torch
+from gemini_torch import LongGemini
+
+# Text tokens
+x = torch.randint(0, 10000, (1, 1024))
+
+# Create an instance of the LongGemini model
+model = LongGemini(
+    dim=512,  # Dimension of the input tensor
+    depth=32,  # Number of transformer blocks
+    dim_head=128,  # Dimension of the query, key, and value vectors
+    long_gemini_depth=9,  # Number of long gemini transformer blocks
+    heads=24,  # Number of attention heads
+    qk_norm=True,  # Whether to apply layer normalization to query and key vectors
+    ring_seq_size=512,  # The size of the ring sequence
+)
+
+# Apply the model to the input tensor
+out = model(x)
+
+# Print the output tensor
+print(out)
+
+```
+
 
 ## Tokenizer
 - Sentencepiece, tokenizer
 - We're using the same tokenizer as LLAMA with special tokens denoting the beginning and end of the multi modality tokens.
 - Does not fully process img, audio, or videos now we need help on that
 
 ```python
```

