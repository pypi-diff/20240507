# Comparing `tmp/werag-0.0.4.tar.gz` & `tmp/werag-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "werag-0.0.4.tar", max compression
+gzip compressed data, was "werag-0.0.5.tar", max compression
```

## Comparing `werag-0.0.4.tar` & `werag-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2024-04-27 05:08:57.889950 werag-0.0.4/README.md
--rw-r--r--   0        0        0      593 2024-04-28 12:22:16.471342 werag-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-04-27 00:27:15.120287 werag-0.0.4/werag/.DS_Store
--rw-r--r--   0        0        0       25 2024-04-27 03:23:00.642045 werag-0.0.4/werag/__init__.py
--rw-r--r--   0        0        0     5945 2024-04-28 12:22:08.296656 werag-0.0.4/werag/client.py
--rw-r--r--   0        0        0     3811 2024-04-27 04:23:52.514873 werag-0.0.4/werag/crud.py
--rw-r--r--   0        0        0      397 2024-04-27 04:09:42.508612 werag-0.0.4/werag/db.py
--rw-r--r--   0        0        0      976 2024-04-27 02:28:24.575438 werag-0.0.4/werag/schema.py
--rw-r--r--   0        0        0        0 2024-04-27 00:20:44.080530 werag-0.0.4/werag/schemas/__init__.py
--rw-r--r--   0        0        0      818 2024-04-27 00:20:44.080642 werag-0.0.4/werag/schemas/chunk.py
--rw-r--r--   0        0        0      183 2024-04-27 02:33:17.900723 werag-0.0.4/werag/utils.py
--rw-r--r--   0        0        0      798 1970-01-01 00:00:00.000000 werag-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-27 05:08:57.889950 werag-0.0.5/README.md
+-rw-r--r--   0        0        0      593 2024-05-07 02:50:52.045299 werag-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-04-27 00:27:15.120287 werag-0.0.5/werag/.DS_Store
+-rw-r--r--   0        0        0       25 2024-04-27 03:23:00.642045 werag-0.0.5/werag/__init__.py
+-rw-r--r--   0        0        0     6965 2024-05-07 02:50:44.539771 werag-0.0.5/werag/client.py
+-rw-r--r--   0        0        0     3811 2024-04-27 04:23:52.514873 werag-0.0.5/werag/crud.py
+-rw-r--r--   0        0        0      397 2024-04-27 04:09:42.508612 werag-0.0.5/werag/db.py
+-rw-r--r--   0        0        0      976 2024-04-27 02:28:24.575438 werag-0.0.5/werag/schema.py
+-rw-r--r--   0        0        0        0 2024-04-27 00:20:44.080530 werag-0.0.5/werag/schemas/__init__.py
+-rw-r--r--   0        0        0      818 2024-04-27 00:20:44.080642 werag-0.0.5/werag/schemas/chunk.py
+-rw-r--r--   0        0        0     1081 2024-05-07 01:58:02.427308 werag-0.0.5/werag/utils.py
+-rw-r--r--   0        0        0      798 1970-01-01 00:00:00.000000 werag-0.0.5/PKG-INFO
```

### Comparing `werag-0.0.4/pyproject.toml` & `werag-0.0.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "werag"
-version = "0.0.4"
+version = "0.0.5"
 description = "python rag for wechat application"
 authors = ["zhenhao-ma <bob0103779@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "<3.13,>=3.10"
 pydantic = "^2.3.0"
```

### Comparing `werag-0.0.4/werag/.DS_Store` & `werag-0.0.5/werag/.DS_Store`

 * *Files identical despite different names*

### Comparing `werag-0.0.4/werag/client.py` & `werag-0.0.5/werag/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,40 +13,55 @@
 from langchain_core.prompts import ChatPromptTemplate
 from langchain_core.runnables import RunnablePassthrough
 from wechatpy import parse_message, create_reply
 
 from .crud import CRUDChroma
 from .db import get_chroma
 from .schema import UserContent
+from .utils import limit_tokens
 
 logger = logging.getLogger(__name__)
 
 
 class WeRag:
     """Core Client for werag service"""
 
     def __init__(self, *,
                  persist_directory: str,
                  collection_name: str = "werag",
                  embedding_function: Embeddings,
                  chunk_size: int = 1000,
-                 chunk_overlap: int = 0):
+                 chunk_overlap: int = 0,
+                 context_size: int = 2000,  # 限制context的token数量
+                 question_size: int = 1000  # 限制question的token数量
+                 ):
         self._crud = CRUDChroma(chunk_size=chunk_size, chunk_overlap=chunk_overlap)
         self._chroma = get_chroma(collection_name=collection_name, persist_directory=persist_directory,
                                   embedding_function=embedding_function)
+        self.__question_size = question_size
+        self.__context_size = context_size
 
     def as_retriever(self, *, user: str,
                      content_type: Optional[str] = None,
                      search_type: Literal["similarity", "mmr", "similarity_score_threshold"] = "similarity",
                      **kwargs):
         return self._chroma.as_retriever(search_kwargs={
             "filter": self._crud.get_user_content_filter(user=user, content_type=content_type),
             **kwargs
         }, search_type=search_type)
 
+    def similarity_search(self, *, query: str, user: str,
+                          content_type: Optional[str] = None,
+                          limit: int = 4) -> List[Document]:
+        return self._chroma.similarity_search(
+            query=query,
+            filter=self._crud.get_user_content_filter(user=user, content_type=content_type),
+            k=limit
+        )
+
     def save_content(self, *, user: str, content: str,
                      content_type: Optional[str] = None) -> UserContent:
         """Save a content base on user id"""
         return self._crud.save_user_content(client=self._chroma, user=user, content_type=content_type, content=content)
 
     def save_documents(self, *, user: str, documents: List[Document],
                        content_type: Optional[str] = None) -> Optional[UserContent]:
@@ -111,27 +126,32 @@
         """
         if prompt_template is None:
             prompt_template = default_prompt_template
 
         parsed_message = parse_message(message)
         if parsed_message.type != "text": return create_reply("我目前只能响应文字内容", parsed_message, render=True)
 
+        # manually retrieve and limit tokens of RAG
+        docs = self.similarity_search(query=parsed_message.content, user=user, content_type=content_type)
+        context = limit_tokens("\n".join([doc.page_content for doc in docs]), max_token=self.__context_size)
+
         # Abstraction of Prompt
         prompt = ChatPromptTemplate.from_template(prompt_template)
 
         # Creating an LLM Chain
-
         llm_chain = LLMChain(llm=llm, prompt=prompt)
 
         # RAG Chain
         rag_chain = (
-                {"context": self.as_retriever(user=user, content_type=content_type),
+                {"context": context,  # self.as_retriever(user=user, content_type=content_type),
                  "question": RunnablePassthrough()}
                 | llm_chain
         )
         response_text = None
         try:
-            response_text = rag_chain.invoke(parsed_message.content)
+            response_text = rag_chain.invoke(
+                limit_tokens(parsed_message.content, max_token=self.__question_size)
+            )
             return create_reply(response_text['text'], parsed_message, render=True)
         except Exception as e:
             logger.critical(f"Failed to get response from LLM, exception: {e}, response: {response_text}")
             return create_reply("系统出错了，没有得到任何回复。请联系管理员", parsed_message, render=True)
```

### Comparing `werag-0.0.4/werag/crud.py` & `werag-0.0.5/werag/crud.py`

 * *Files identical despite different names*

### Comparing `werag-0.0.4/werag/schema.py` & `werag-0.0.5/werag/schema.py`

 * *Files identical despite different names*

### Comparing `werag-0.0.4/werag/schemas/chunk.py` & `werag-0.0.5/werag/schemas/chunk.py`

 * *Files identical despite different names*

### Comparing `werag-0.0.4/PKG-INFO` & `werag-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: werag
-Version: 0.0.4
+Version: 0.0.5
 Summary: python rag for wechat application
 Author: zhenhao-ma
 Author-email: bob0103779@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

