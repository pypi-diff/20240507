# Comparing `tmp/whyhow-0.0.4.tar.gz` & `tmp/whyhow-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whyhow-0.0.4.tar", last modified: Sun Apr 21 02:16:52 2024, max compression
+gzip compressed data, was "whyhow-0.0.5.tar", last modified: Tue May  7 04:21:22 2024, max compression
```

## Comparing `whyhow-0.0.4.tar` & `whyhow-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-21 02:16:52.966239 whyhow-0.0.4/
--rw-r--r--   0 tomsmoker   (501) staff       (20)     7907 2024-04-21 02:16:52.966003 whyhow-0.0.4/PKG-INFO
--rw-r--r--   0 tomsmoker   (501) staff       (20)     6778 2024-04-21 02:04:51.000000 whyhow-0.0.4/README.md
--rw-r--r--   0 tomsmoker   (501) staff       (20)     2061 2024-04-21 01:37:48.000000 whyhow-0.0.4/pyproject.toml
--rw-r--r--   0 tomsmoker   (501) staff       (20)       38 2024-04-21 02:16:52.966282 whyhow-0.0.4/setup.cfg
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-21 02:16:52.959864 whyhow-0.0.4/src/
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-21 02:16:52.961362 whyhow-0.0.4/src/whyhow/
--rw-r--r--   0 tomsmoker   (501) staff       (20)      125 2024-04-21 02:10:14.000000 whyhow-0.0.4/src/whyhow/__init__.py
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-21 02:16:52.963098 whyhow-0.0.4/src/whyhow/apis/
--rw-r--r--   0 tomsmoker   (501) staff       (20)       49 2024-03-30 23:23:35.000000 whyhow-0.0.4/src/whyhow/apis/__init__.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)      501 2024-04-04 06:55:34.000000 whyhow-0.0.4/src/whyhow/apis/base.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)     4797 2024-04-21 01:37:48.000000 whyhow-0.0.4/src/whyhow/apis/graph.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)     6707 2024-04-21 01:37:48.000000 whyhow-0.0.4/src/whyhow/client.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)      166 2024-03-30 23:23:35.000000 whyhow-0.0.4/src/whyhow/exceptions.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)        0 2024-03-30 23:23:35.000000 whyhow-0.0.4/src/whyhow/py.typed
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-21 02:16:52.964043 whyhow-0.0.4/src/whyhow/schemas/
--rw-r--r--   0 tomsmoker   (501) staff       (20)      189 2024-03-30 23:23:35.000000 whyhow-0.0.4/src/whyhow/schemas/__init__.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)      624 2024-03-30 23:23:35.000000 whyhow-0.0.4/src/whyhow/schemas/base.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)     5002 2024-04-21 01:37:48.000000 whyhow-0.0.4/src/whyhow/schemas/common.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)     1459 2024-04-21 01:37:48.000000 whyhow-0.0.4/src/whyhow/schemas/graph.py
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-21 02:16:52.964810 whyhow-0.0.4/src/whyhow.egg-info/
--rw-r--r--   0 tomsmoker   (501) staff       (20)     7907 2024-04-21 02:16:52.000000 whyhow-0.0.4/src/whyhow.egg-info/PKG-INFO
--rw-r--r--   0 tomsmoker   (501) staff       (20)      548 2024-04-21 02:16:52.000000 whyhow-0.0.4/src/whyhow.egg-info/SOURCES.txt
--rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-04-21 02:16:52.000000 whyhow-0.0.4/src/whyhow.egg-info/dependency_links.txt
--rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-03-31 17:56:30.000000 whyhow-0.0.4/src/whyhow.egg-info/not-zip-safe
--rw-r--r--   0 tomsmoker   (501) staff       (20)      218 2024-04-21 02:16:52.000000 whyhow-0.0.4/src/whyhow.egg-info/requires.txt
--rw-r--r--   0 tomsmoker   (501) staff       (20)        7 2024-04-21 02:16:52.000000 whyhow-0.0.4/src/whyhow.egg-info/top_level.txt
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-21 02:16:52.964631 whyhow-0.0.4/tests/
--rw-r--r--   0 tomsmoker   (501) staff       (20)     1431 2024-04-21 01:37:48.000000 whyhow-0.0.4/tests/test_client.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)       48 2024-03-30 23:23:35.000000 whyhow-0.0.4/tests/test_dummy.py
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-07 04:21:22.673420 whyhow-0.0.5/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     7907 2024-05-07 04:21:22.673212 whyhow-0.0.5/PKG-INFO
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     6778 2024-05-07 03:43:17.000000 whyhow-0.0.5/README.md
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     2061 2024-05-07 03:43:17.000000 whyhow-0.0.5/pyproject.toml
+-rw-r--r--   0 tomsmoker   (501) staff       (20)       38 2024-05-07 04:21:22.673464 whyhow-0.0.5/setup.cfg
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-07 04:21:22.666854 whyhow-0.0.5/src/
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-07 04:21:22.668275 whyhow-0.0.5/src/whyhow/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      125 2024-05-07 03:43:27.000000 whyhow-0.0.5/src/whyhow/__init__.py
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-07 04:21:22.669967 whyhow-0.0.5/src/whyhow/apis/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)       49 2024-03-30 23:23:35.000000 whyhow-0.0.5/src/whyhow/apis/__init__.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      501 2024-04-04 06:55:34.000000 whyhow-0.0.5/src/whyhow/apis/base.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     5024 2024-05-07 03:43:17.000000 whyhow-0.0.5/src/whyhow/apis/graph.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     6707 2024-04-21 01:37:48.000000 whyhow-0.0.5/src/whyhow/client.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      166 2024-03-30 23:23:35.000000 whyhow-0.0.5/src/whyhow/exceptions.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)        0 2024-03-30 23:23:35.000000 whyhow-0.0.5/src/whyhow/py.typed
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-07 04:21:22.671265 whyhow-0.0.5/src/whyhow/schemas/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      189 2024-03-30 23:23:35.000000 whyhow-0.0.5/src/whyhow/schemas/__init__.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      624 2024-03-30 23:23:35.000000 whyhow-0.0.5/src/whyhow/schemas/base.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     5002 2024-05-07 03:43:17.000000 whyhow-0.0.5/src/whyhow/schemas/common.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     2110 2024-05-07 03:43:17.000000 whyhow-0.0.5/src/whyhow/schemas/graph.py
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-07 04:21:22.672135 whyhow-0.0.5/src/whyhow.egg-info/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     7907 2024-05-07 04:21:22.000000 whyhow-0.0.5/src/whyhow.egg-info/PKG-INFO
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      548 2024-05-07 04:21:22.000000 whyhow-0.0.5/src/whyhow.egg-info/SOURCES.txt
+-rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-05-07 04:21:22.000000 whyhow-0.0.5/src/whyhow.egg-info/dependency_links.txt
+-rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-03-31 17:56:30.000000 whyhow-0.0.5/src/whyhow.egg-info/not-zip-safe
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      218 2024-05-07 04:21:22.000000 whyhow-0.0.5/src/whyhow.egg-info/requires.txt
+-rw-r--r--   0 tomsmoker   (501) staff       (20)        7 2024-05-07 04:21:22.000000 whyhow-0.0.5/src/whyhow.egg-info/top_level.txt
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-07 04:21:22.671803 whyhow-0.0.5/tests/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     1431 2024-05-07 03:43:17.000000 whyhow-0.0.5/tests/test_client.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)       48 2024-03-30 23:23:35.000000 whyhow-0.0.5/tests/test_dummy.py
```

### Comparing `whyhow-0.0.4/PKG-INFO` & `whyhow-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whyhow
-Version: 0.0.4
+Version: 0.0.5
 Summary: Whyhow automated KG SDK
 Author-email: Tom Smoker <tom@whyhow.ai>, Chris Rec <chris@whyhow.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/whyhow-ai/whyhow
 Keywords: SDK,KG
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

### Comparing `whyhow-0.0.4/README.md` & `whyhow-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.4/pyproject.toml` & `whyhow-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.4/src/whyhow/apis/graph.py` & `whyhow-0.0.5/src/whyhow/apis/graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from whyhow.schemas.graph import (
     AddDocumentsResponse,
     CreateGraphResponse,
     CreateQuestionGraphRequest,
     CreateSchemaGraphRequest,
     QueryGraphRequest,
     QueryGraphResponse,
-    QueryGraphReturn,
 )
 
 
 class GraphAPI(APIBase):
     """Interacting with the graph API synchronously."""
 
     def add_documents(self, namespace: str, documents: list[str]) -> str:
@@ -137,38 +136,48 @@
 
         raw_response.raise_for_status()
 
         response = CreateGraphResponse.model_validate(raw_response.json())
 
         return response.message
 
-    def query_graph(self, namespace: str, query: str) -> QueryGraphReturn:
+    def query_graph(
+        self,
+        namespace: str,
+        query: str,
+        include_triples: bool = False,
+        include_chunks: bool = False,
+    ) -> QueryGraphResponse:
         """Query the graph.
 
         Parameters
         ----------
         namespace : str
             The namespace of the graph.
 
         query : str
             The query to run.
 
         Returns
         -------
-        QueryGraphReturn
-            The answer, triples, and Cypher query.
+        QueryGraphResponse
+            The namespace, answer, triples, and chunks and Cypher query.
 
         """
-        request_body = QueryGraphRequest(query=query)
+        request_body = QueryGraphRequest(
+            query=query,
+            include_triples=include_triples,
+            include_chunks=include_chunks,
+        )
 
         raw_response = self.client.post(
             f"{self.prefix}/{namespace}/query",
             json=request_body.model_dump(),
         )
 
         raw_response.raise_for_status()
 
         response = QueryGraphResponse.model_validate(raw_response.json())
 
-        retval = QueryGraphReturn(answer=response.answer)
+        # retval = QueryGraphReturn(answer=response.answer)
 
-        return retval
+        return response
```

### Comparing `whyhow-0.0.4/src/whyhow/client.py` & `whyhow-0.0.5/src/whyhow/client.py`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.4/src/whyhow/schemas/base.py` & `whyhow-0.0.5/src/whyhow/schemas/base.py`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.4/src/whyhow/schemas/common.py` & `whyhow-0.0.5/src/whyhow/schemas/common.py`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.4/src/whyhow/schemas/graph.py` & `whyhow-0.0.5/src/whyhow/schemas/graph.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,20 +45,45 @@
     graph: Graph
 
 
 class QueryGraphRequest(BaseRequest):
     """Schema for the request body of the query graph endpoint."""
 
     query: str
+    include_triples: bool = False
+    include_chunks: bool = False
+
+
+class QueryGraphTripleResponse(BaseResponse):
+    """Schema for the triples within the query graph response."""
+
+    head: str
+    relation: str
+    tail: str
+
+
+class QueryGraphChunkResponse(BaseResponse):
+    """Schema for the triples within the query graph response."""
+
+    head: str
+    relation: str
+    tail: str
+    chunk_ids: list[str]
+    chunk_texts: list[str]
 
 
 class QueryGraphResponse(BaseResponse):
     """Schema for the response body of the query graph endpoint."""
 
     namespace: str
     answer: str
+    triples: list[QueryGraphTripleResponse] = []
+    chunks: list[QueryGraphChunkResponse] = []
 
 
 class QueryGraphReturn(BaseReturn):
     """Schema for the return value of the query graph endpoint."""
 
+    namespace: str
     answer: str
+    triples: list[QueryGraphTripleResponse] = []
+    chunks: list[QueryGraphChunkResponse] = []
```

### Comparing `whyhow-0.0.4/src/whyhow.egg-info/PKG-INFO` & `whyhow-0.0.5/src/whyhow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whyhow
-Version: 0.0.4
+Version: 0.0.5
 Summary: Whyhow automated KG SDK
 Author-email: Tom Smoker <tom@whyhow.ai>, Chris Rec <chris@whyhow.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/whyhow-ai/whyhow
 Keywords: SDK,KG
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

### Comparing `whyhow-0.0.4/src/whyhow.egg-info/SOURCES.txt` & `whyhow-0.0.5/src/whyhow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.4/tests/test_client.py` & `whyhow-0.0.5/tests/test_client.py`

 * *Files identical despite different names*

