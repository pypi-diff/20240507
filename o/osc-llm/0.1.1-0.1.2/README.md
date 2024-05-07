# Comparing `tmp/osc_llm-0.1.1.tar.gz` & `tmp/osc_llm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osc_llm-0.1.1.tar", max compression
+gzip compressed data, was "osc_llm-0.1.2.tar", max compression
```

## Comparing `osc_llm-0.1.1.tar` & `osc_llm-0.1.2.tar`

### file list

```diff
@@ -1,45 +1,47 @@
--rw-r--r--   0        0        0      560 2024-04-29 01:55:20.518111 osc_llm-0.1.1/README.md
--rw-r--r--   0        0        0      253 2024-04-30 00:21:10.635963 osc_llm-0.1.1/osc_llm/__init__.py
--rw-r--r--   0        0        0       51 2024-04-27 15:22:11.337904 osc_llm-0.1.1/osc_llm/architectures/__init__.py
--rw-r--r--   0        0        0     8089 2024-04-27 15:21:42.709990 osc_llm-0.1.1/osc_llm/architectures/transformer_decoder.py
--rw-r--r--   0        0        0     4176 2024-04-30 14:09:39.718502 osc_llm-0.1.1/osc_llm/chat.py
--rw-r--r--   0        0        0      136 2024-04-29 08:59:09.247275 osc_llm-0.1.1/osc_llm/chat_templates/__init__.py
--rw-r--r--   0        0        0     1509 2024-04-30 01:49:42.527398 osc_llm-0.1.1/osc_llm/chat_templates/base.py
--rw-r--r--   0        0        0      891 2024-04-27 15:20:32.266209 osc_llm-0.1.1/osc_llm/chat_templates/chatml.py
--rw-r--r--   0        0        0     2751 2024-04-30 12:29:13.554688 osc_llm-0.1.1/osc_llm/chat_templates/llama.py
--rw-r--r--   0        0        0     6659 2024-04-28 23:27:52.946274 osc_llm-0.1.1/osc_llm/cli.py
--rw-r--r--   0        0        0     1314 2024-04-29 23:11:24.182541 osc_llm-0.1.1/osc_llm/config.py
--rw-r--r--   0        0        0       48 2024-04-27 15:57:52.529093 osc_llm-0.1.1/osc_llm/demos/__init__.py
--rw-r--r--   0        0        0     5517 2024-04-27 16:06:43.049671 osc_llm-0.1.1/osc_llm/demos/language_model.py
--rw-r--r--   0        0        0       83 2024-04-29 23:43:54.288202 osc_llm-0.1.1/osc_llm/engines/__init__.py
--rw-r--r--   0        0        0     1874 2024-04-30 14:10:01.673484 osc_llm-0.1.1/osc_llm/engines/base.py
--rw-r--r--   0        0        0     4185 2024-04-30 14:10:16.748812 osc_llm-0.1.1/osc_llm/engines/v1.py
--rw-r--r--   0        0        0     4916 2024-04-30 14:10:25.104449 osc_llm-0.1.1/osc_llm/engines/v2.py
--rw-r--r--   0        0        0      725 2024-04-27 15:10:30.684848 osc_llm-0.1.1/osc_llm/layers/__init__.py
--rw-r--r--   0        0        0      650 2024-04-27 15:10:30.656849 osc_llm-0.1.1/osc_llm/layers/activation.py
--rw-r--r--   0        0        0     6224 2024-04-27 15:10:30.680848 osc_llm-0.1.1/osc_llm/layers/attention.py
--rw-r--r--   0        0        0      186 2024-04-27 15:17:53.918752 osc_llm-0.1.1/osc_llm/layers/dropout.py
--rw-r--r--   0        0        0     2238 2024-04-27 15:10:30.684848 osc_llm-0.1.1/osc_llm/layers/embedding.py
--rw-r--r--   0        0        0     3371 2024-04-27 15:10:30.684848 osc_llm-0.1.1/osc_llm/layers/feedforward.py
--rw-r--r--   0        0        0      336 2024-04-27 15:10:30.684848 osc_llm-0.1.1/osc_llm/layers/head.py
--rw-r--r--   0        0        0     2745 2024-04-27 15:10:30.684848 osc_llm-0.1.1/osc_llm/layers/kv_cache.py
--rw-r--r--   0        0        0     5657 2024-04-27 15:10:30.688848 osc_llm-0.1.1/osc_llm/layers/linear.py
--rw-r--r--   0        0        0      823 2024-04-27 15:10:30.688848 osc_llm-0.1.1/osc_llm/layers/normalization.py
--rw-r--r--   0        0        0      416 2024-04-27 15:17:28.926844 osc_llm-0.1.1/osc_llm/model_helpers/__init__.py
--rw-r--r--   0        0        0     6262 2024-04-27 15:44:58.586217 osc_llm-0.1.1/osc_llm/model_helpers/base.py
--rw-r--r--   0        0        0     3054 2024-04-27 15:16:30.027073 osc_llm-0.1.1/osc_llm/model_helpers/llama.py
--rw-r--r--   0        0        0     3203 2024-04-27 15:34:51.665212 osc_llm-0.1.1/osc_llm/model_helpers/qwen.py
--rw-r--r--   0        0        0       46 2024-04-27 15:00:44.802617 osc_llm-0.1.1/osc_llm/optimizers/__init__.py
--rw-r--r--   0        0        0     1376 2024-04-27 15:00:44.802617 osc_llm-0.1.1/osc_llm/optimizers/scheduler.py
--rw-r--r--   0        0        0      159 2024-04-27 15:10:37.236808 osc_llm-0.1.1/osc_llm/quantizers/__init__.py
--rw-r--r--   0        0        0      717 2024-04-27 15:10:37.244808 osc_llm-0.1.1/osc_llm/quantizers/base.py
--rw-r--r--   0        0        0     8861 2024-04-27 15:33:29.096094 osc_llm-0.1.1/osc_llm/quantizers/int4.py
--rw-r--r--   0        0        0     3347 2024-04-27 15:33:57.584497 osc_llm-0.1.1/osc_llm/quantizers/int8.py
--rw-r--r--   0        0        0       74 2024-04-27 15:04:12.071947 osc_llm-0.1.1/osc_llm/samplers/__init__.py
--rw-r--r--   0        0        0      903 2024-04-27 15:04:12.079947 osc_llm-0.1.1/osc_llm/samplers/base.py
--rw-r--r--   0        0        0     1134 2024-04-27 15:04:12.083947 osc_llm-0.1.1/osc_llm/samplers/top_k.py
--rw-r--r--   0        0        0     1121 2024-04-27 15:04:12.083947 osc_llm-0.1.1/osc_llm/samplers/top_p.py
--rw-r--r--   0        0        0     7959 2024-04-30 11:45:44.712285 osc_llm-0.1.1/osc_llm/tokenizer.py
--rw-r--r--   0        0        0     6252 2024-04-29 07:31:58.187293 osc_llm-0.1.1/osc_llm/utils.py
--rw-r--r--   0        0        0      495 2024-04-30 14:22:42.505200 osc_llm-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 osc_llm-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      560 2024-04-29 01:55:20.518111 osc_llm-0.1.2/README.md
+-rw-r--r--   0        0        0      253 2024-04-30 00:21:10.635963 osc_llm-0.1.2/osc_llm/__init__.py
+-rw-r--r--   0        0        0       51 2024-04-27 15:22:11.337904 osc_llm-0.1.2/osc_llm/architectures/__init__.py
+-rw-r--r--   0        0        0     8089 2024-04-27 15:21:42.709990 osc_llm-0.1.2/osc_llm/architectures/transformer_decoder.py
+-rw-r--r--   0        0        0     4697 2024-05-06 06:38:02.866868 osc_llm-0.1.2/osc_llm/chat.py
+-rw-r--r--   0        0        0      136 2024-04-29 08:59:09.247275 osc_llm-0.1.2/osc_llm/chat_templates/__init__.py
+-rw-r--r--   0        0        0     1509 2024-04-30 01:49:42.527398 osc_llm-0.1.2/osc_llm/chat_templates/base.py
+-rw-r--r--   0        0        0      891 2024-04-27 15:20:32.266209 osc_llm-0.1.2/osc_llm/chat_templates/chatml.py
+-rw-r--r--   0        0        0     2751 2024-04-30 12:29:13.554688 osc_llm-0.1.2/osc_llm/chat_templates/llama.py
+-rw-r--r--   0        0        0     6733 2024-05-06 11:48:20.141468 osc_llm-0.1.2/osc_llm/cli.py
+-rw-r--r--   0        0        0     1314 2024-04-29 23:11:24.182541 osc_llm-0.1.2/osc_llm/config.py
+-rw-r--r--   0        0        0       48 2024-04-27 15:57:52.529093 osc_llm-0.1.2/osc_llm/demos/__init__.py
+-rw-r--r--   0        0        0     5517 2024-04-27 16:06:43.049671 osc_llm-0.1.2/osc_llm/demos/language_model.py
+-rw-r--r--   0        0        0       83 2024-04-29 23:43:54.288202 osc_llm-0.1.2/osc_llm/engines/__init__.py
+-rw-r--r--   0        0        0     2084 2024-05-06 06:50:35.853043 osc_llm-0.1.2/osc_llm/engines/base.py
+-rw-r--r--   0        0        0     4207 2024-05-07 01:00:24.504971 osc_llm-0.1.2/osc_llm/engines/v1.py
+-rw-r--r--   0        0        0     4916 2024-04-30 14:10:25.104449 osc_llm-0.1.2/osc_llm/engines/v2.py
+-rw-r--r--   0        0        0      725 2024-04-27 15:10:30.684848 osc_llm-0.1.2/osc_llm/layers/__init__.py
+-rw-r--r--   0        0        0      650 2024-04-27 15:10:30.656849 osc_llm-0.1.2/osc_llm/layers/activation.py
+-rw-r--r--   0        0        0     6224 2024-04-27 15:10:30.680848 osc_llm-0.1.2/osc_llm/layers/attention.py
+-rw-r--r--   0        0        0      186 2024-04-27 15:17:53.918752 osc_llm-0.1.2/osc_llm/layers/dropout.py
+-rw-r--r--   0        0        0     2238 2024-04-27 15:10:30.684848 osc_llm-0.1.2/osc_llm/layers/embedding.py
+-rw-r--r--   0        0        0     3371 2024-04-27 15:10:30.684848 osc_llm-0.1.2/osc_llm/layers/feedforward.py
+-rw-r--r--   0        0        0      336 2024-04-27 15:10:30.684848 osc_llm-0.1.2/osc_llm/layers/head.py
+-rw-r--r--   0        0        0     2745 2024-04-27 15:10:30.684848 osc_llm-0.1.2/osc_llm/layers/kv_cache.py
+-rw-r--r--   0        0        0     5657 2024-04-27 15:10:30.688848 osc_llm-0.1.2/osc_llm/layers/linear.py
+-rw-r--r--   0        0        0      823 2024-04-27 15:10:30.688848 osc_llm-0.1.2/osc_llm/layers/normalization.py
+-rw-r--r--   0        0        0      416 2024-04-27 15:17:28.926844 osc_llm-0.1.2/osc_llm/model_helpers/__init__.py
+-rw-r--r--   0        0        0     6262 2024-04-27 15:44:58.586217 osc_llm-0.1.2/osc_llm/model_helpers/base.py
+-rw-r--r--   0        0        0     3054 2024-04-27 15:16:30.027073 osc_llm-0.1.2/osc_llm/model_helpers/llama.py
+-rw-r--r--   0        0        0     3203 2024-04-27 15:34:51.665212 osc_llm-0.1.2/osc_llm/model_helpers/qwen.py
+-rw-r--r--   0        0        0       46 2024-04-27 15:00:44.802617 osc_llm-0.1.2/osc_llm/optimizers/__init__.py
+-rw-r--r--   0        0        0     1376 2024-04-27 15:00:44.802617 osc_llm-0.1.2/osc_llm/optimizers/scheduler.py
+-rw-r--r--   0        0        0      159 2024-04-27 15:10:37.236808 osc_llm-0.1.2/osc_llm/quantizers/__init__.py
+-rw-r--r--   0        0        0      717 2024-04-27 15:10:37.244808 osc_llm-0.1.2/osc_llm/quantizers/base.py
+-rw-r--r--   0        0        0     8861 2024-04-27 15:33:29.096094 osc_llm-0.1.2/osc_llm/quantizers/int4.py
+-rw-r--r--   0        0        0     3347 2024-04-27 15:33:57.584497 osc_llm-0.1.2/osc_llm/quantizers/int8.py
+-rw-r--r--   0        0        0       74 2024-04-27 15:04:12.071947 osc_llm-0.1.2/osc_llm/samplers/__init__.py
+-rw-r--r--   0        0        0      903 2024-04-27 15:04:12.079947 osc_llm-0.1.2/osc_llm/samplers/base.py
+-rw-r--r--   0        0        0     1134 2024-04-27 15:04:12.083947 osc_llm-0.1.2/osc_llm/samplers/top_k.py
+-rw-r--r--   0        0        0     1121 2024-04-27 15:04:12.083947 osc_llm-0.1.2/osc_llm/samplers/top_p.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:34:05.202914 osc_llm-0.1.2/osc_llm/servers/__init__.py
+-rw-r--r--   0        0        0     7635 2024-05-07 01:03:41.381436 osc_llm-0.1.2/osc_llm/servers/openai.py
+-rw-r--r--   0        0        0     8774 2024-05-07 02:27:53.539430 osc_llm-0.1.2/osc_llm/tokenizer.py
+-rw-r--r--   0        0        0     6405 2024-05-06 10:35:40.498735 osc_llm-0.1.2/osc_llm/utils.py
+-rw-r--r--   0        0        0      546 2024-05-07 02:47:55.169520 osc_llm-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1421 1970-01-01 00:00:00.000000 osc_llm-0.1.2/PKG-INFO
```

### Comparing `osc_llm-0.1.1/README.md` & `osc_llm-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.1/osc_llm/architectures/transformer_decoder.py` & `osc_llm-0.1.2/osc_llm/architectures/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.1/osc_llm/chat.py` & `osc_llm-0.1.2/osc_llm/chat.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from .tokenizer import Tokenizer
 from .chat_templates import Message
 from .samplers import TopK
 from .engines import LLMEngineV1, LLMEngine, LLMEngineV2
 import torch
 import time
-import sys
 from pathlib import Path
 from typing import Optional, Literal
+from itertools import chain
 
 
 
 torch.set_float32_matmul_precision('high')
     
 
 @torch.inference_mode()
@@ -50,24 +50,28 @@
         engine: LLMEngine = LLMEngineV2(checkpoint_dir=checkpoint_dir,
                                         sampler=sampler,
                                         max_length=max_length,
                                         devices=[device],
                                         compile=compile)
     engine.setup()
     
-            
+    if not hasattr(engine, "decode_model"):
+        model_size = sum([p.numel() * p.dtype.itemsize for p in chain(engine.model.parameters(), engine.model.buffers())])
+    else:
+        model_size = sum([p.numel() * p.dtype.itemsize for p in chain(engine.decode_model.parameters(), engine.decode_model.buffers())])
+    
     if compile:
         t = time.perf_counter()
         input_ids = tokenizer.encode_messages([Message(role='user', content="你好")])
         stream = engine.run(input_ids=input_ids, stop_ids=tokenizer.stop_ids)
         token_stream = tokenizer.decode_stream(stream=stream)
         for token in token_stream:
             pass
-        print(f"Time for warmup: {time.perf_counter() - t:.2f} seconds")
-        print("\n")
+        engine.fabric.print(f"Time for warmup: {time.perf_counter() - t:.2f} seconds")
+        engine.fabric.print("\n")
 
     messages = []
     pre_ids_len = 0 # 多轮对话过程中,对之前的对话历史做一个缓存,这样避免在prefill阶段重新kv cache
     while True:
         content = input("User (empty to exit): ")
         if content == "":
             break
@@ -76,28 +80,30 @@
         input_ids = tokenizer.encode_messages(messages)
         with engine.fabric.init_tensor():
             input_pos = torch.arange(pre_ids_len, len(input_ids))
         input_ids = input_ids[pre_ids_len:]
         
         stream = engine.run(input_ids=input_ids, stop_ids=tokenizer.stop_ids, input_pos=input_pos)
         generated_text = ""
-        print("Assistant: ")
+        engine.fabric.print("Assistant: ")
         time0 = time.perf_counter()
         token_stream = tokenizer.decode_stream(stream=stream)
         for token in token_stream:
             print(token, end='', flush=True)
             generated_text += token
         time1 = time.perf_counter()
         t = time1 - time0
         num_new_tokens = len(tokenizer.encode(generated_text).tolist())
+        tokens_sec = num_new_tokens / t
         
         if multi_turn:
             messages.append(Message(role='assistant', content=generated_text))
             pre_ids_len += len(input_ids)
         else:
             messages = []
             pre_ids_len = 0
         
-        print("\n")
-        print(f"Generated {num_new_tokens} tokens in {t:.02f} seconds, {(num_new_tokens / t):.2f} tokens/second", file=sys.stderr)
-        print(f"Memory used: {torch.cuda.max_memory_allocated() / 1e9:.02f} GB", file=sys.stderr)
-        print("\n")
+        engine.fabric.print("\n")
+        engine.fabric.print(f"Generated {num_new_tokens} tokens in {t:.02f} seconds, {(num_new_tokens / t):.2f} tokens/second")
+        engine.fabric.print(f"Memory used: {torch.cuda.max_memory_allocated() / 1e9:.02f} GB")
+        engine.fabric.print(f"Bandwidth Achieved: {model_size * tokens_sec / 1e9:.02f} GB/s")
+        engine.fabric.print("\n")
```

### Comparing `osc_llm-0.1.1/osc_llm/chat_templates/base.py` & `osc_llm-0.1.2/osc_llm/chat_templates/base.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.1/osc_llm/chat_templates/chatml.py` & `osc_llm-0.1.2/osc_llm/chat_templates/chatml.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.1/osc_llm/chat_templates/llama.py` & `osc_llm-0.1.2/osc_llm/chat_templates/llama.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.1/osc_llm/cli.py` & `osc_llm-0.1.2/osc_llm/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from jsonargparse import CLI 
 from .chat import main as chat_main
+from .servers.openai import main as openai_main
 from .model_helpers import get_supported_architectures
 from .model_helpers.base import HFModelHelper
 from .quantizers import WeightOnlyInt8Quantizer, WeightOnlyInt4Quantizer
 from .tokenizer import Tokenizer
 from .config import registry
 from .utils import build_from_checkpoint
 from pathlib import Path
@@ -162,14 +163,15 @@
         "lora": lambda: print("lora"),
         "full": lambda: print("full")
     },
     "convert": convert,
     "quantize": {
         "int8": quantize_int8,
         "int4": quantize_int4
-    }
+    },
+    "serve": openai_main
 }
 
 
 
 def run_cli():
     CLI(components=commands, as_positional=False)
```

### Comparing `osc_llm-0.1.1/osc_llm/config.py` & `osc_llm-0.1.2/osc_llm/config.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.1/osc_llm/demos/language_model.py` & `osc_llm-0.1.2/osc_llm/demos/language_model.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.1/osc_llm/engines/base.py` & `osc_llm-0.1.2/osc_llm/engines/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 from typing import Union, List, Optional, Generator
 from lightning import Fabric
 from time import perf_counter
 import sys
 from ..samplers import Sampler, TopK
 from abc import ABC, abstractmethod
+import torch
+from ..utils import get_default_supported_precision
 
 
 class LLMEngine(ABC):
     """语言模型引擎: 控制着大模型加载,编译,运转以及停止。
     """
     
     def __init__(
         self,
         checkpoint_dir: str,
         sampler: Optional[Sampler] = None,
         max_length: Optional[int] = None,
         devices: Union[int, List[int]] = 1,
         accelerator: str = "auto",
         compile: bool = True,
+        precision: Optional[str] = None
     ):
 
-        self.fabric = Fabric(devices=devices, accelerator=accelerator, precision="bf16-true")
+        if not precision:
+            precision = get_default_supported_precision(training=False)
+        self.fabric = Fabric(devices=devices, accelerator=accelerator, precision=precision)
         
         self.sampler = sampler if sampler else TopK(temperature=0.8, k=200)
         self.max_length = max_length
         
         self.compile = compile
         
         self.checkpoint_dir = checkpoint_dir
@@ -36,15 +41,15 @@
     def compile_model(self) -> None:
         raise NotImplementedError
     
     def setup_model(self) -> None:
         raise NotImplementedError
     
     @abstractmethod
-    def run(self, **model_inputs) -> Generator[str, None, None]:
+    def run(self, **model_inputs) -> Generator[torch.Tensor, None, None]:
         raise NotImplementedError
     
     def setup(self) -> None:
         t = perf_counter()
         self.load_model()
         self.fabric.print(f"load model in {perf_counter() - t:.02f} seconds", file=sys.stderr)
         if self.compile:
```

### Comparing `osc_llm-0.1.1/osc_llm/engines/v1.py` & `osc_llm-0.1.2/osc_llm/engines/v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,18 +36,22 @@
             self.model.setup_kv_cache(batch_size=1, max_length=self.max_length, dtype=torch.bfloat16)
             
         
     def compile_model(self) -> None:
         torch._inductor.config.coordinate_descent_tuning = True
         torch._inductor.config.triton.unique_kernel_names = True
         torch._inductor.config.fx_graph_cache = True # Experimental feature to reduce compilation times, will be on by default in future
+        torch._inductor.config.triton.cudagraph_trees = False # 目前用作server的时候有bug
+        
         torch._dynamo.config.automatic_dynamic_shapes = True
-        torch._dynamo.config.suppress_errors = True
+        
+        
         self.model: TransformerDecoder = torch.compile(self.model, dynamic=True, fullgraph=True, mode="reduce-overhead")
-    
+
+        
     def setup_model(self) -> None:
         self.model = self.fabric.setup_module(self.model)
     
     @torch.inference_mode()
     def run(self, input_ids: torch.Tensor, stop_ids: List[torch.Tensor], input_pos: Optional[torch.Tensor] = None) -> Generator[str, None, None]:
         
         # 确保输入在设备上
@@ -79,18 +83,16 @@
                             return 
                 if len(yield_ids) >= max_stop_len:
                     yield from yield_ids
                     yield_ids = []
             input_pos = input_pos.add_(1)
             input_ids = next_token_id
         
-    @torch.inference_mode()
     def prefill(self, **model_inputs) -> torch.Tensor:
         logits = self.model(**model_inputs)[0, -1]
         idx = self.sampler.sample(logits=logits)
         return idx
     
-    @torch.inference_mode()
     def decode(self, **model_inputs) -> torch.Tensor:
         logits = self.model(**model_inputs)[0, -1]
         idx = self.sampler.sample(logits=logits)
         return idx
```

### Comparing `osc_llm-0.1.1/osc_llm/engines/v2.py` & `osc_llm-0.1.2/osc_llm/engines/v2.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.1/osc_llm/layers/__init__.py` & `osc_llm-0.1.2/osc_llm/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.1/osc_llm/layers/activation.py` & `osc_llm-0.1.2/osc_llm/layers/activation.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.1/osc_llm/layers/attention.py` & `osc_llm-0.1.2/osc_llm/layers/attention.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.1/osc_llm/layers/embedding.py` & `osc_llm-0.1.2/osc_llm/layers/embedding.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.1/osc_llm/layers/feedforward.py` & `osc_llm-0.1.2/osc_llm/layers/feedforward.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.1/osc_llm/layers/kv_cache.py` & `osc_llm-0.1.2/osc_llm/layers/kv_cache.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.1/osc_llm/layers/linear.py` & `osc_llm-0.1.2/osc_llm/layers/linear.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.1/osc_llm/layers/normalization.py` & `osc_llm-0.1.2/osc_llm/layers/normalization.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.1/osc_llm/model_helpers/base.py` & `osc_llm-0.1.2/osc_llm/model_helpers/base.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.1/osc_llm/model_helpers/llama.py` & `osc_llm-0.1.2/osc_llm/model_helpers/llama.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.1/osc_llm/model_helpers/qwen.py` & `osc_llm-0.1.2/osc_llm/model_helpers/qwen.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.1/osc_llm/optimizers/scheduler.py` & `osc_llm-0.1.2/osc_llm/optimizers/scheduler.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.1/osc_llm/quantizers/base.py` & `osc_llm-0.1.2/osc_llm/quantizers/base.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.1/osc_llm/quantizers/int4.py` & `osc_llm-0.1.2/osc_llm/quantizers/int4.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.1/osc_llm/quantizers/int8.py` & `osc_llm-0.1.2/osc_llm/quantizers/int8.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.1/osc_llm/samplers/base.py` & `osc_llm-0.1.2/osc_llm/samplers/base.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.1/osc_llm/samplers/top_k.py` & `osc_llm-0.1.2/osc_llm/samplers/top_k.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.1/osc_llm/samplers/top_p.py` & `osc_llm-0.1.2/osc_llm/samplers/top_p.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.1/osc_llm/tokenizer.py` & `osc_llm-0.1.2/osc_llm/tokenizer.py`

 * *Files 13% similar despite different names*

```diff
@@ -126,33 +126,41 @@
         return self.processor.decode(tokens)
     
     def decode_stream(
         self,
         stream: Generator[torch.Tensor, None, None],
     ) -> Generator[str, None, None]:
         if self.backend == "huggingface":
+            buffer = torch.tensor([], dtype=torch.long)
             text = ''
             try:
                 for token in stream:
-                    t = self.decode(token)
-                    yield t
-                    text += t
+                    buffer = buffer.to(device=token.device)
+                    buffer = torch.cat((buffer, token.view(-1)))
+                    t = self.decode(buffer)
+                    if not self.has_special_chars(t):
+                        yield t
+                        text += t
+                        buffer = torch.tensor([], dtype=torch.long)
             except KeyboardInterrupt:
                 # support stopping generation
                 return text
         elif self.backend == "sentencepiece":
             # sentencepiece does not support decoding token-by-token because it adds spaces based on the surrounding tokens
             # meaning that we need to decode everything each time
             so_far = torch.tensor([], dtype=torch.long)
             decoded_so_far = ""
             try:
                 for token in stream:
                     so_far = so_far.to(device=token.device)
                     so_far = torch.cat((so_far, token.view(-1)))
                     decoded_new = self.decode(so_far)
+                    if self.has_special_chars(decoded_new):
+                        # if the text contains special characters, it means that the tokenization is not complete
+                        continue
                     yield decoded_new[len(decoded_so_far):]
                     decoded_so_far = decoded_new
             except KeyboardInterrupt:
                 # support stopping generation
                 return decoded_so_far
         else:
             raise NotImplementedError(self.backend)
@@ -170,8 +178,14 @@
             shutil.copyfile(self.tokenizer_path, save_dir / self.tokenizer_path.name)
             
     @property
     def stop_ids(self) -> List[List[int]]:
         stop_ids = [[torch.tensor([self.eos_id], dtype=torch.int)]]
         if self.chat_template:
             stop_ids.extend([[self.encode(text)] for text in self.chat_template.stop_texts])
-        return stop_ids
+        return stop_ids
+    
+    def has_special_chars(self, text: str) -> bool:
+        """使用sentencepiece时，检查文本中是否包含特殊字符�.这种情况通常是由于一个中文字符被分割为几个token,而解码时没有合并回去导致的.
+        """
+        return '�' in text
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `osc_llm-0.1.1/osc_llm/utils.py` & `osc_llm-0.1.2/osc_llm/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,22 @@
 from pathlib import Path
 from .config import registry, Config
 from typing import Optional, Union, Dict, Tuple
 from wasabi import msg
 import statistics
 import torch
+import uuid
 
 
 
 def find_multiple(n: int, k: int) -> int:
     assert k > 0
     if n % k == 0:
         return n
     return n + k - (n % k)
-
-
-def get_default_supported_precision(training: bool) -> str:
-    """Return default precision that is supported by the hardware.
-
-    Args:
-        training: `-mixed` or `-true` version of the precision to use
-        tpu: whether TPU device is used
-
-    Returns:
-        default precision that is suitable for the task and is supported by the hardware
-    """
-    
-    if not torch.cuda.is_available() or torch.cuda.is_bf16_supported():
-        return "bf16-mixed" if training else "bf16-true"
-    return "16-mixed" if training else "16-true"
         
         
 def get_chat_template(name) -> Optional[Config]:
     """在一个checkpoint的名称中获取chat模板"""
     for k, v in registry.chat_templates.get_all().items():
         if k in name:
             return v
@@ -139,8 +124,28 @@
         times.append(start.elapsed_time(end) / 1000)
     msg.info(f"Number of iterations: {num_iters}.")
     all_time = sum(times)
     msg.info(f"Total time: {all_time:.4f} s")
     mean_time = statistics.mean(times)
     msg.info(f"Mean time: {mean_time:.4f} s")
     median_time = statistics.median(times)
-    msg.info(f"Median time: {median_time:.4f} s")
+    msg.info(f"Median time: {median_time:.4f} s")
+    
+
+def get_default_supported_precision(training: bool) -> str:
+    """Return default precision that is supported by the hardware: either `bf16` or `16`.
+
+    Args:
+        training: `-mixed` or `-true` version of the precision to use
+
+    Returns:
+        default precision that is suitable for the task and is supported by the hardware
+    """
+    from lightning.fabric.accelerators import MPSAccelerator
+
+    if MPSAccelerator.is_available() or (torch.cuda.is_available() and not torch.cuda.is_bf16_supported()):
+        return "16-mixed" if training else "16-true"
+    return "bf16-mixed" if training else "bf16-true"
+
+
+def random_uuid() -> str:
+    return str(uuid.uuid4().hex)
```

### Comparing `osc_llm-0.1.1/PKG-INFO` & `osc_llm-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osc-llm
-Version: 0.1.1
+Version: 0.1.2
 Summary: 大模型训练,推理,部署工具
 License: MIT
 Author: wangmengdi
 Author-email: 790990241@qq.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: catalogue (>=2.0.10)
 Requires-Dist: confection (>=0.1.4)
 Requires-Dist: jsonargparse (>=4.28.0)
 Requires-Dist: lightning (>=2.2.0)
+Requires-Dist: sentencepiece (>=0.2.0)
+Requires-Dist: tokenizers (>=0.19.1)
 Requires-Dist: torch (>=2.3.0)
 Requires-Dist: wasabi (>=1.1.2)
 Description-Content-Type: text/markdown
 
 # OSC-LLM
 
 osc-llm旨在成为一个简单易用的大模型训练、评估、部署工具，支持目前主流的大模型。
```

