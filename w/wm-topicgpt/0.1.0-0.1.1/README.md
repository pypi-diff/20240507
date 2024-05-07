# Comparing `tmp/wm_topicgpt-0.1.0.tar.gz` & `tmp/wm_topicgpt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wm_topicgpt-0.1.0.tar", last modified: Tue Apr 23 16:44:45 2024, max compression
+gzip compressed data, was "wm_topicgpt-0.1.1.tar", last modified: Tue May  7 14:28:45 2024, max compression
```

## Comparing `wm_topicgpt-0.1.0.tar` & `wm_topicgpt-0.1.1.tar`

### file list

```diff
@@ -1,45 +1,38 @@
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 16:44:45.704513 wm_topicgpt-0.1.0/
--rw-r--r--   0 y0h07pr    (503) staff       (20)     4753 2024-04-23 16:44:45.703970 wm_topicgpt-0.1.0/PKG-INFO
--rw-r--r--   0 y0h07pr    (503) staff       (20)       38 2024-04-23 16:44:45.704569 wm_topicgpt-0.1.0/setup.cfg
--rw-r--r--   0 y0h07pr    (503) staff       (20)      601 2024-04-23 16:43:50.000000 wm_topicgpt-0.1.0/setup.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 16:44:45.658333 wm_topicgpt-0.1.0/test/
--rw-r--r--   0 y0h07pr    (503) staff       (20)     1523 2024-04-08 01:24:06.000000 wm_topicgpt-0.1.0/test/test_approach.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     2315 2024-04-05 21:17:40.000000 wm_topicgpt-0.1.0/test/test_functions.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 16:44:45.661986 wm_topicgpt-0.1.0/topicgpt/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      194 2024-04-08 17:46:49.000000 wm_topicgpt-0.1.0/topicgpt/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      260 2024-04-02 16:48:50.000000 wm_topicgpt-0.1.0/topicgpt/_config.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      276 2024-04-05 18:53:52.000000 wm_topicgpt-0.1.0/topicgpt/base.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 16:44:45.663432 wm_topicgpt-0.1.0/topicgpt/classification/
--rw-r--r--   0 y0h07pr    (503) staff       (20)       71 2024-04-19 15:12:14.000000 wm_topicgpt-0.1.0/topicgpt/classification/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     3753 2024-04-22 21:21:46.000000 wm_topicgpt-0.1.0/topicgpt/classification/_classification.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 16:44:45.667437 wm_topicgpt-0.1.0/topicgpt/embedding/
--rw-r--r--   0 y0h07pr    (503) staff       (20)       74 2024-04-05 15:01:57.000000 wm_topicgpt-0.1.0/topicgpt/embedding/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      944 2024-04-22 21:20:15.000000 wm_topicgpt-0.1.0/topicgpt/embedding/_embed_model.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 16:44:45.670096 wm_topicgpt-0.1.0/topicgpt/feature_extraction/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      110 2024-04-08 21:26:03.000000 wm_topicgpt-0.1.0/topicgpt/feature_extraction/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     3384 2024-04-23 15:24:16.000000 wm_topicgpt-0.1.0/topicgpt/feature_extraction/_keywords.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     1505 2024-04-08 22:13:17.000000 wm_topicgpt-0.1.0/topicgpt/feature_extraction/_summary.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 16:44:45.671228 wm_topicgpt-0.1.0/topicgpt/pipeline/
--rw-r--r--   0 y0h07pr    (503) staff       (20)       74 2024-04-23 15:10:49.000000 wm_topicgpt-0.1.0/topicgpt/pipeline/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     8595 2024-04-23 15:24:15.000000 wm_topicgpt-0.1.0/topicgpt/pipeline/_pipeline.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 16:44:45.672448 wm_topicgpt-0.1.0/topicgpt/preprocessing/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      108 2024-04-04 04:34:46.000000 wm_topicgpt-0.1.0/topicgpt/preprocessing/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     2854 2024-04-22 21:16:47.000000 wm_topicgpt-0.1.0/topicgpt/preprocessing/_data.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 16:44:45.676131 wm_topicgpt-0.1.0/topicgpt/topic/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      284 2024-04-08 19:59:45.000000 wm_topicgpt-0.1.0/topicgpt/topic/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      431 2024-04-23 04:44:41.000000 wm_topicgpt-0.1.0/topicgpt/topic/_cluster_base.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     5205 2024-04-23 13:17:52.000000 wm_topicgpt-0.1.0/topicgpt/topic/_hdbscan_approach.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     3981 2024-04-23 15:05:47.000000 wm_topicgpt-0.1.0/topicgpt/topic/_kmeans_appproach.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     5558 2024-04-23 13:12:05.000000 wm_topicgpt-0.1.0/topicgpt/topic/_topic.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      412 2024-04-19 14:52:51.000000 wm_topicgpt-0.1.0/topicgpt/utils.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 16:44:45.678407 wm_topicgpt-0.1.0/topicgpt/walmart_llm/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      115 2024-04-05 21:44:12.000000 wm_topicgpt-0.1.0/topicgpt/walmart_llm/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     9052 2024-04-12 20:33:35.000000 wm_topicgpt-0.1.0/topicgpt/walmart_llm/_chat_model.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     8079 2024-03-28 16:26:16.000000 wm_topicgpt-0.1.0/topicgpt/walmart_llm/_embed_model.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     7000 2024-04-23 05:25:54.000000 wm_topicgpt-0.1.0/topicgpt/walmart_llm/_llm_client.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 16:44:45.703268 wm_topicgpt-0.1.0/wm_topicgpt.egg-info/
--rw-r--r--   0 y0h07pr    (503) staff       (20)     4753 2024-04-23 16:44:45.000000 wm_topicgpt-0.1.0/wm_topicgpt.egg-info/PKG-INFO
--rw-r--r--   0 y0h07pr    (503) staff       (20)      995 2024-04-23 16:44:45.000000 wm_topicgpt-0.1.0/wm_topicgpt.egg-info/SOURCES.txt
--rw-r--r--   0 y0h07pr    (503) staff       (20)        1 2024-04-23 16:44:45.000000 wm_topicgpt-0.1.0/wm_topicgpt.egg-info/dependency_links.txt
--rw-r--r--   0 y0h07pr    (503) staff       (20)      267 2024-04-23 16:44:45.000000 wm_topicgpt-0.1.0/wm_topicgpt.egg-info/requires.txt
--rw-r--r--   0 y0h07pr    (503) staff       (20)        9 2024-04-23 16:44:45.000000 wm_topicgpt-0.1.0/wm_topicgpt.egg-info/top_level.txt
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:28:45.781172 wm_topicgpt-0.1.1/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     7103 2024-05-07 14:28:45.780643 wm_topicgpt-0.1.1/PKG-INFO
+-rw-r--r--   0 y0h07pr    (503) staff       (20)       38 2024-05-07 14:28:45.781237 wm_topicgpt-0.1.1/setup.cfg
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      601 2024-05-07 14:26:28.000000 wm_topicgpt-0.1.1/setup.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:28:45.752493 wm_topicgpt-0.1.1/topicgpt/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      209 2024-05-07 14:20:30.000000 wm_topicgpt-0.1.1/topicgpt/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      312 2024-05-05 05:35:46.000000 wm_topicgpt-0.1.1/topicgpt/_config.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      276 2024-05-04 00:03:35.000000 wm_topicgpt-0.1.1/topicgpt/base.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:28:45.755743 wm_topicgpt-0.1.1/topicgpt/clustering/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      191 2024-05-05 22:35:15.000000 wm_topicgpt-0.1.1/topicgpt/clustering/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      428 2024-05-06 03:49:21.000000 wm_topicgpt-0.1.1/topicgpt/clustering/_base_cluster.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     3035 2024-05-06 14:14:30.000000 wm_topicgpt-0.1.1/topicgpt/clustering/_hdbscan.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)    10045 2024-05-06 18:24:02.000000 wm_topicgpt-0.1.1/topicgpt/clustering/_kmeans.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     2285 2024-05-05 03:15:39.000000 wm_topicgpt-0.1.1/topicgpt/clustering/_sampling.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:28:45.757913 wm_topicgpt-0.1.1/topicgpt/generation/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      138 2024-05-06 16:56:29.000000 wm_topicgpt-0.1.1/topicgpt/generation/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     2910 2024-05-07 01:27:18.000000 wm_topicgpt-0.1.1/topicgpt/generation/_keywords.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     5501 2024-05-06 19:42:11.000000 wm_topicgpt-0.1.1/topicgpt/generation/_topic.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:28:45.761834 wm_topicgpt-0.1.1/topicgpt/persistence/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      330 2024-05-07 01:26:00.000000 wm_topicgpt-0.1.1/topicgpt/persistence/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     1012 2024-05-06 03:42:53.000000 wm_topicgpt-0.1.1/topicgpt/persistence/_plot.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     4297 2024-05-07 03:09:02.000000 wm_topicgpt-0.1.1/topicgpt/persistence/_save.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     5360 2024-05-07 14:20:10.000000 wm_topicgpt-0.1.1/topicgpt/pipeline.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:28:45.764564 wm_topicgpt-0.1.1/topicgpt/preprocessing/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      108 2024-05-03 23:14:55.000000 wm_topicgpt-0.1.1/topicgpt/preprocessing/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     2854 2024-05-03 23:14:55.000000 wm_topicgpt-0.1.1/topicgpt/preprocessing/_data.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      412 2024-05-06 00:04:30.000000 wm_topicgpt-0.1.1/topicgpt/utils.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:28:45.771575 wm_topicgpt-0.1.1/topicgpt/walmart_llm/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      153 2024-05-03 23:24:30.000000 wm_topicgpt-0.1.1/topicgpt/walmart_llm/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     9052 2024-05-03 23:35:49.000000 wm_topicgpt-0.1.1/topicgpt/walmart_llm/_chat_model.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     8079 2024-05-03 20:57:39.000000 wm_topicgpt-0.1.1/topicgpt/walmart_llm/_embed_model.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     7922 2024-05-03 23:35:53.000000 wm_topicgpt-0.1.1/topicgpt/walmart_llm/_llm_client.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:28:45.779908 wm_topicgpt-0.1.1/wm_topicgpt.egg-info/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     7103 2024-05-07 14:28:45.000000 wm_topicgpt-0.1.1/wm_topicgpt.egg-info/PKG-INFO
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      841 2024-05-07 14:28:45.000000 wm_topicgpt-0.1.1/wm_topicgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 y0h07pr    (503) staff       (20)        1 2024-05-07 14:28:45.000000 wm_topicgpt-0.1.1/wm_topicgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      360 2024-05-07 14:28:45.000000 wm_topicgpt-0.1.1/wm_topicgpt.egg-info/requires.txt
+-rw-r--r--   0 y0h07pr    (503) staff       (20)        9 2024-05-07 14:28:45.000000 wm_topicgpt-0.1.1/wm_topicgpt.egg-info/top_level.txt
```

### Comparing `wm_topicgpt-0.1.0/setup.py` & `wm_topicgpt-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     install_requires = f.read().splitlines()
 
 with open("topicgpt/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='wm_topicgpt',
-    version='0.1.0',
+    version='0.1.1',
     description='This is a package to generate topics for the text corpus.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=install_requires,
     python_requires='>=3.9',
 )
```

### Comparing `wm_topicgpt-0.1.0/topicgpt/preprocessing/_data.py` & `wm_topicgpt-0.1.1/topicgpt/preprocessing/_data.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.1.0/topicgpt/walmart_llm/_chat_model.py` & `wm_topicgpt-0.1.1/topicgpt/walmart_llm/_chat_model.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.1.0/topicgpt/walmart_llm/_embed_model.py` & `wm_topicgpt-0.1.1/topicgpt/walmart_llm/_embed_model.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.1.0/topicgpt/walmart_llm/_llm_client.py` & `wm_topicgpt-0.1.1/topicgpt/walmart_llm/_llm_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from Crypto.Hash import SHA256
 from Crypto.PublicKey import RSA
 from Crypto.Signature import PKCS1_v1_5
 from base64 import b64encode
 from langchain.schema import HumanMessage
 from topicgpt.walmart_llm._chat_model import WalmartAzureOpenAiChatModels
 from topicgpt.walmart_llm._embed_model import WalmartAzureOpenaiEmbeddings
+from langchain_community.embeddings import HuggingFaceBgeEmbeddings
 from topicgpt import config
 
 
 def test_config():
     if config.consumer_id is None:
         raise ValueError("Please set up config.consumer_id!")
     if config.private_key_path is None:
@@ -182,8 +183,31 @@
         for idx in tqdm(range(0, len(documents), self.batch_size), total=num_batch):
             batch_documents = documents[idx: idx+self.batch_size]
             batch_embeddings = self.retry_embed_documents(batch_documents)
             embeddings.extend(batch_embeddings)
         return embeddings
     
     def embed_query(self, document):
-        return self.model.embed_query(document)
+        return self.model.embed_query(document)
+    
+
+class BGEEmbedModel:
+
+    def __init__(self, batch_size=500, device="cpu", model_name="BAAI/bge-small-en-v1.5"):
+        self.batch_size = batch_size
+        self.model = HuggingFaceBgeEmbeddings(
+            model_name=model_name, model_kwargs={"device": device}, encode_kwargs={"normalize_embeddings": True}
+        )
+
+    def embed_documents(self, documents):
+        embeddings = []
+        num_batch = math.ceil(len(documents) / self.batch_size)
+        for idx in tqdm(range(0, len(documents), self.batch_size), total=num_batch):
+            batch_documents = documents[idx: idx+self.batch_size]
+            batch_embeddings = self.model.embed_documents(batch_documents)
+            embeddings.extend(batch_embeddings)
+        return embeddings
+    
+    def embed_query(self, document):
+        return self.model.embed_query(document)
+    
+
```

