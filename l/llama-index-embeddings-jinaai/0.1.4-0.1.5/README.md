# Comparing `tmp/llama_index_embeddings_jinaai-0.1.4.tar.gz` & `tmp/llama_index_embeddings_jinaai-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_embeddings_jinaai-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_embeddings_jinaai-0.1.5.tar", max compression
```

## Comparing `llama_index_embeddings_jinaai-0.1.4.tar` & `llama_index_embeddings_jinaai-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       44 2024-05-03 18:27:21.554168 llama_index_embeddings_jinaai-0.1.4/README.md
--rw-r--r--   0        0        0       90 2024-05-03 18:27:21.554168 llama_index_embeddings_jinaai-0.1.4/llama_index/embeddings/jinaai/__init__.py
--rw-r--r--   0        0        0     6399 2024-05-03 18:27:21.554168 llama_index_embeddings_jinaai-0.1.4/llama_index/embeddings/jinaai/base.py
--rw-r--r--   0        0        0     1446 2024-05-03 18:27:21.554168 llama_index_embeddings_jinaai-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      603 1970-01-01 00:00:00.000000 llama_index_embeddings_jinaai-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       44 2024-05-07 16:41:03.253788 llama_index_embeddings_jinaai-0.1.5/README.md
+-rw-r--r--   0        0        0       90 2024-05-07 16:41:03.253788 llama_index_embeddings_jinaai-0.1.5/llama_index/embeddings/jinaai/__init__.py
+-rw-r--r--   0        0        0     6616 2024-05-07 16:41:03.253788 llama_index_embeddings_jinaai-0.1.5/llama_index/embeddings/jinaai/base.py
+-rw-r--r--   0        0        0     1446 2024-05-07 16:41:03.253788 llama_index_embeddings_jinaai-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      603 1970-01-01 00:00:00.000000 llama_index_embeddings_jinaai-0.1.5/PKG-INFO
```

### Comparing `llama_index_embeddings_jinaai-0.1.4/llama_index/embeddings/jinaai/base.py` & `llama_index_embeddings_jinaai-0.1.5/llama_index/embeddings/jinaai/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from llama_index.core.callbacks.base import CallbackManager
 from llama_index.core.base.llms.generic_utils import get_from_param_or_env
 
 MAX_BATCH_SIZE = 2048
 
 API_URL = "https://api.jina.ai/v1/embeddings"
 
-
 VALID_ENCODING = ["float", "ubinary", "binary"]
 
 
 class JinaEmbedding(BaseEmbedding):
     """JinaAI class for embeddings.
 
     Args:
@@ -74,42 +73,47 @@
 
     @classmethod
     def class_name(cls) -> str:
         return "JinaAIEmbedding"
 
     def _get_query_embedding(self, query: str) -> List[float]:
         """Get query embedding."""
-        return self._get_text_embeddings([query], encoding_type=self._encoding_queries)[
-            0
-        ]
+        return self._get_embeddings([query], encoding_type=self._encoding_queries)[0]
 
     async def _aget_query_embedding(self, query: str) -> List[float]:
         """The asynchronous version of _get_query_embedding."""
-        result = await self._aget_text_embeddings(
+        result = await self._aget_embeddings(
             [query], encoding_type=self._encoding_queries
         )
         return result[0]
 
     def _get_text_embedding(self, text: str) -> List[float]:
         """Get text embedding."""
-        return self._get_text_embeddings(
-            [text], encoding_type=self._encoding_documents
-        )[0]
+        return self._get_text_embeddings([text])[0]
 
     async def _aget_text_embedding(self, text: str) -> List[float]:
         """Asynchronously get text embedding."""
-        result = await self._aget_text_embeddings(
-            [text], encoding_type=self._encoding_documents
-        )
+        result = await self._aget_text_embeddings([text])
         return result[0]
 
-    def _get_text_embeddings(
+    def _get_text_embeddings(self, texts: List[str]) -> List[List[float]]:
+        return self._get_embeddings(texts=texts, encoding_type=self._encoding_documents)
+
+    async def _aget_text_embeddings(
+        self,
+        texts: List[str],
+    ) -> List[List[float]]:
+        return await self._aget_embeddings(
+            texts=texts, encoding_type=self._encoding_documents
+        )
+
+    def _get_embeddings(
         self, texts: List[str], encoding_type: str = "float"
     ) -> List[List[float]]:
-        """Get text embeddings."""
+        """Get embeddings."""
         # Call Jina AI Embedding API
         resp = self._session.post(  # type: ignore
             API_URL,
             json={"input": texts, "model": self.model, "encoding_type": encoding_type},
         ).json()
         if "data" not in resp:
             raise RuntimeError(resp["detail"])
@@ -130,15 +134,15 @@
                 np.unpackbits(
                     (np.array(result["embedding"]) + 128).astype("uint8")
                 ).tolist()
                 for result in sorted_embeddings
             ]
         return [result["embedding"] for result in sorted_embeddings]
 
-    async def _aget_text_embeddings(
+    async def _aget_embeddings(
         self, texts: List[str], encoding_type: str = "float"
     ) -> List[List[float]]:
         """Asynchronously get text embeddings."""
         import aiohttp
 
         async with aiohttp.ClientSession(trust_env=True) as session:
             headers = {
```

### Comparing `llama_index_embeddings_jinaai-0.1.4/pyproject.toml` & `llama_index_embeddings_jinaai-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index embeddings jinaai integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-embeddings-jinaai"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
```

### Comparing `llama_index_embeddings_jinaai-0.1.4/PKG-INFO` & `llama_index_embeddings_jinaai-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-embeddings-jinaai
-Version: 0.1.4
+Version: 0.1.5
 Summary: llama-index embeddings jinaai integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

