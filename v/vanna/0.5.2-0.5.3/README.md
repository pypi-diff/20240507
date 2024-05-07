# Comparing `tmp/vanna-0.5.2.tar.gz` & `tmp/vanna-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanna-0.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vanna-0.5.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vanna-0.5.2.tar` & `vanna-0.5.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     8010 2024-05-06 13:24:20.218984 vanna-0.5.2/README.md
--rw-r--r--   0        0        0     1627 2024-05-06 13:24:20.234984 vanna-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     8725 2024-05-06 13:24:20.234984 vanna-0.5.2/src/vanna/ZhipuAI/ZhipuAI_Chat.py
--rw-r--r--   0        0        0     2849 2024-05-06 13:24:20.234984 vanna-0.5.2/src/vanna/ZhipuAI/ZhipuAI_embeddings.py
--rw-r--r--   0        0        0      116 2024-05-06 13:24:20.234984 vanna-0.5.2/src/vanna/ZhipuAI/__init__.py
--rw-r--r--   0        0        0     9248 2024-05-06 13:24:20.234984 vanna-0.5.2/src/vanna/__init__.py
--rw-r--r--   0        0        0       43 2024-05-06 13:24:20.234984 vanna-0.5.2/src/vanna/anthropic/__init__.py
--rw-r--r--   0        0        0     2615 2024-05-06 13:24:20.234984 vanna-0.5.2/src/vanna/anthropic/anthropic_chat.py
--rw-r--r--   0        0        0       28 2024-05-06 13:24:20.234984 vanna-0.5.2/src/vanna/base/__init__.py
--rw-r--r--   0        0        0    65593 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/base/base.py
--rw-r--r--   0        0        0       50 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/chromadb/__init__.py
--rw-r--r--   0        0        0     8792 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/chromadb/chromadb_vector.py
--rw-r--r--   0        0        0      685 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/exceptions/__init__.py
--rw-r--r--   0        0        0    25192 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/flask/__init__.py
--rw-r--r--   0        0        0   187711 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/flask/assets.py
--rw-r--r--   0        0        0     1246 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/flask/auth.py
--rw-r--r--   0        0        0       41 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/google/__init__.py
--rw-r--r--   0        0        0     1584 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/google/gemini_chat.py
--rw-r--r--   0        0        0       19 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/hf/__init__.py
--rw-r--r--   0        0        0     2703 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/hf/hf.py
--rw-r--r--   0        0        0      313 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/local.py
--rw-r--r--   0        0        0       37 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/marqo/__init__.py
--rw-r--r--   0        0        0     5242 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/marqo/marqo.py
--rw-r--r--   0        0        0       29 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/mistral/__init__.py
--rw-r--r--   0        0        0     1508 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/mistral/mistral.py
--rw-r--r--   0        0        0       27 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/ollama/__init__.py
--rw-r--r--   0        0        0     3790 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/ollama/ollama.py
--rw-r--r--   0        0        0       86 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/openai/__init__.py
--rw-r--r--   0        0        0     4764 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/openai/openai_chat.py
--rw-r--r--   0        0        0     1260 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/openai/openai_embeddings.py
--rw-r--r--   0        0        0       54 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/opensearch/__init__.py
--rw-r--r--   0        0        0    11980 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/opensearch/opensearch_vector.py
--rw-r--r--   0        0        0       73 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/qdrant/__init__.py
--rw-r--r--   0        0        0    12613 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/qdrant/qdrant.py
--rw-r--r--   0        0        0     1856 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/remote.py
--rw-r--r--   0        0        0     4957 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/types/__init__.py
--rw-r--r--   0        0        0     2247 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/utils.py
--rw-r--r--   0        0        0       48 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/vannadb/__init__.py
--rw-r--r--   0        0        0     6168 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/vannadb/vannadb_vector.py
--rw-r--r--   0        0        0       23 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/vllm/__init__.py
--rw-r--r--   0        0        0     2427 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/vllm/vllm.py
--rw-r--r--   0        0        0    11248 1970-01-01 00:00:00.000000 vanna-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     8010 2024-05-06 15:47:42.673345 vanna-0.5.3/README.md
+-rw-r--r--   0        0        0     1627 2024-05-06 15:47:42.689345 vanna-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     8725 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/ZhipuAI/ZhipuAI_Chat.py
+-rw-r--r--   0        0        0     2849 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/ZhipuAI/ZhipuAI_embeddings.py
+-rw-r--r--   0        0        0      116 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/ZhipuAI/__init__.py
+-rw-r--r--   0        0        0     9248 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/__init__.py
+-rw-r--r--   0        0        0       43 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/anthropic/__init__.py
+-rw-r--r--   0        0        0     2615 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/anthropic/anthropic_chat.py
+-rw-r--r--   0        0        0       28 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/base/__init__.py
+-rw-r--r--   0        0        0    65593 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/base/base.py
+-rw-r--r--   0        0        0       50 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/chromadb/__init__.py
+-rw-r--r--   0        0        0     8792 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/chromadb/chromadb_vector.py
+-rw-r--r--   0        0        0      685 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/exceptions/__init__.py
+-rw-r--r--   0        0        0    25192 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/flask/__init__.py
+-rw-r--r--   0        0        0   187711 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/flask/assets.py
+-rw-r--r--   0        0        0     1246 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/flask/auth.py
+-rw-r--r--   0        0        0       41 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/google/__init__.py
+-rw-r--r--   0        0        0     1584 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/google/gemini_chat.py
+-rw-r--r--   0        0        0       19 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/hf/__init__.py
+-rw-r--r--   0        0        0     2703 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/hf/hf.py
+-rw-r--r--   0        0        0      313 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/local.py
+-rw-r--r--   0        0        0       37 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/marqo/__init__.py
+-rw-r--r--   0        0        0     5242 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/marqo/marqo.py
+-rw-r--r--   0        0        0       29 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/mistral/__init__.py
+-rw-r--r--   0        0        0     1508 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/mistral/mistral.py
+-rw-r--r--   0        0        0       27 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/ollama/__init__.py
+-rw-r--r--   0        0        0     3794 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/ollama/ollama.py
+-rw-r--r--   0        0        0       86 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/openai/__init__.py
+-rw-r--r--   0        0        0     4764 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/openai/openai_chat.py
+-rw-r--r--   0        0        0     1260 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/openai/openai_embeddings.py
+-rw-r--r--   0        0        0       54 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/opensearch/__init__.py
+-rw-r--r--   0        0        0    11980 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/opensearch/opensearch_vector.py
+-rw-r--r--   0        0        0       73 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/qdrant/__init__.py
+-rw-r--r--   0        0        0    12613 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/qdrant/qdrant.py
+-rw-r--r--   0        0        0     1856 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/remote.py
+-rw-r--r--   0        0        0     4957 2024-05-06 15:47:42.689345 vanna-0.5.3/src/vanna/types/__init__.py
+-rw-r--r--   0        0        0     2247 2024-05-06 15:47:42.693345 vanna-0.5.3/src/vanna/utils.py
+-rw-r--r--   0        0        0       48 2024-05-06 15:47:42.693345 vanna-0.5.3/src/vanna/vannadb/__init__.py
+-rw-r--r--   0        0        0     6168 2024-05-06 15:47:42.693345 vanna-0.5.3/src/vanna/vannadb/vannadb_vector.py
+-rw-r--r--   0        0        0       23 2024-05-06 15:47:42.693345 vanna-0.5.3/src/vanna/vllm/__init__.py
+-rw-r--r--   0        0        0     2427 2024-05-06 15:47:42.693345 vanna-0.5.3/src/vanna/vllm/vllm.py
+-rw-r--r--   0        0        0    11248 1970-01-01 00:00:00.000000 vanna-0.5.3/PKG-INFO
```

### Comparing `vanna-0.5.2/README.md` & `vanna-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `vanna-0.5.2/pyproject.toml` & `vanna-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "vanna"
-version = "0.5.2"
+version = "0.5.3"
 authors = [
   { name="Zain Hoda", email="zain@vanna.ai" },
 ]
 
 description = "Generate SQL queries from natural language"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `vanna-0.5.2/src/vanna/ZhipuAI/ZhipuAI_Chat.py` & `vanna-0.5.3/src/vanna/ZhipuAI/ZhipuAI_Chat.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.2/src/vanna/ZhipuAI/ZhipuAI_embeddings.py` & `vanna-0.5.3/src/vanna/ZhipuAI/ZhipuAI_embeddings.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.2/src/vanna/__init__.py` & `vanna-0.5.3/src/vanna/__init__.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.2/src/vanna/anthropic/anthropic_chat.py` & `vanna-0.5.3/src/vanna/anthropic/anthropic_chat.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.2/src/vanna/base/base.py` & `vanna-0.5.3/src/vanna/base/base.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.2/src/vanna/chromadb/chromadb_vector.py` & `vanna-0.5.3/src/vanna/chromadb/chromadb_vector.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.2/src/vanna/exceptions/__init__.py` & `vanna-0.5.3/src/vanna/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.2/src/vanna/flask/__init__.py` & `vanna-0.5.3/src/vanna/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.2/src/vanna/flask/assets.py` & `vanna-0.5.3/src/vanna/flask/assets.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.2/src/vanna/flask/auth.py` & `vanna-0.5.3/src/vanna/flask/auth.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.2/src/vanna/google/gemini_chat.py` & `vanna-0.5.3/src/vanna/google/gemini_chat.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.2/src/vanna/hf/hf.py` & `vanna-0.5.3/src/vanna/hf/hf.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.2/src/vanna/marqo/marqo.py` & `vanna-0.5.3/src/vanna/marqo/marqo.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.2/src/vanna/mistral/mistral.py` & `vanna-0.5.3/src/vanna/mistral/mistral.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.2/src/vanna/ollama/ollama.py` & `vanna-0.5.3/src/vanna/ollama/ollama.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     if not config:
       raise ValueError("config must contain at least Ollama model")
     if 'model' not in config.keys():
       raise ValueError("config must contain at least Ollama model")
     self.host = config.get("ollama_host", "http://localhost:11434")
     self.model = config["model"]
-    if ":" in self.model:
+    if ":" not in self.model:
       self.model += ":latest"
 
     self.ollama_client = ollama.Client(self.host, timeout=Timeout(240.0))
     self.keep_alive = config.get('keep_alive', None)
     self.ollama_options = config.get('options', {})
     self.num_ctx = self.ollama_options.get('num_ctx', 2048)
     self.__pull_model_if_ne(self.ollama_client, self.model)
```

### Comparing `vanna-0.5.2/src/vanna/openai/openai_chat.py` & `vanna-0.5.3/src/vanna/openai/openai_chat.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.2/src/vanna/openai/openai_embeddings.py` & `vanna-0.5.3/src/vanna/openai/openai_embeddings.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.2/src/vanna/opensearch/opensearch_vector.py` & `vanna-0.5.3/src/vanna/opensearch/opensearch_vector.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.2/src/vanna/qdrant/qdrant.py` & `vanna-0.5.3/src/vanna/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.2/src/vanna/remote.py` & `vanna-0.5.3/src/vanna/remote.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.2/src/vanna/types/__init__.py` & `vanna-0.5.3/src/vanna/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.2/src/vanna/utils.py` & `vanna-0.5.3/src/vanna/utils.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.2/src/vanna/vannadb/vannadb_vector.py` & `vanna-0.5.3/src/vanna/vannadb/vannadb_vector.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.2/src/vanna/vllm/vllm.py` & `vanna-0.5.3/src/vanna/vllm/vllm.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.2/PKG-INFO` & `vanna-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vanna
-Version: 0.5.2
+Version: 0.5.3
 Summary: Generate SQL queries from natural language
 Author-email: Zain Hoda <zain@vanna.ai>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

