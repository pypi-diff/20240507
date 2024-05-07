# Comparing `tmp/llama_index_packs_raft_dataset-0.1.4.tar.gz` & `tmp/llama_index_packs_raft_dataset-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_packs_raft_dataset-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_packs_raft_dataset-0.1.5.tar", max compression
```

## Comparing `llama_index_packs_raft_dataset-0.1.4.tar` & `llama_index_packs_raft_dataset-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2896 2024-04-13 04:42:59.761415 llama_index_packs_raft_dataset-0.1.4/README.md
--rw-r--r--   0        0        0       95 2024-04-13 04:42:59.761415 llama_index_packs_raft_dataset-0.1.4/llama_index/packs/raft_dataset/__init__.py
--rw-r--r--   0        0        0     8458 2024-04-13 04:42:59.761415 llama_index_packs_raft_dataset-0.1.4/llama_index/packs/raft_dataset/base.py
--rw-r--r--   0        0        0     1567 2024-04-13 04:42:59.761415 llama_index_packs_raft_dataset-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3578 1970-01-01 00:00:00.000000 llama_index_packs_raft_dataset-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2896 2024-05-07 16:26:09.151053 llama_index_packs_raft_dataset-0.1.5/README.md
+-rw-r--r--   0        0        0       95 2024-05-07 16:26:09.151053 llama_index_packs_raft_dataset-0.1.5/llama_index/packs/raft_dataset/__init__.py
+-rw-r--r--   0        0        0     8483 2024-05-07 16:26:09.151053 llama_index_packs_raft_dataset-0.1.5/llama_index/packs/raft_dataset/base.py
+-rw-r--r--   0        0        0     1567 2024-05-07 16:26:09.151053 llama_index_packs_raft_dataset-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3578 1970-01-01 00:00:00.000000 llama_index_packs_raft_dataset-0.1.5/PKG-INFO
```

### Comparing `llama_index_packs_raft_dataset-0.1.4/README.md` & `llama_index_packs_raft_dataset-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_packs_raft_dataset-0.1.4/llama_index/packs/raft_dataset/base.py` & `llama_index_packs_raft_dataset-0.1.5/llama_index/packs/raft_dataset/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 from typing import Any, List
 import random
 import logging
 from datasets import Dataset
 
 # Configure logging to output to the console, with messages of level DEBUG and above
-logging.basicConfig(level=logging.INFO)
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.INFO)
 
 from llama_index.core.llama_pack.base import BaseLlamaPack
 from llama_index.core import SimpleDirectoryReader
 
 from llama_index.core.node_parser import SemanticSplitterNodeParser
 from llama_index.core.llms import ChatMessage
 from llama_index.llms.openai import OpenAI
@@ -195,20 +196,20 @@
             else:
                 self.ds = self.ds.add_item(datapt)
 
     def run(self) -> Any:
         """Run the pipeline."""
         chunks = self.get_chunks(self.file_path, self.chunk_size)
 
-        logging.info(f"Number of chunks created: {len(chunks)}")
+        logger.info(f"Number of chunks created: {len(chunks)}")
 
         self.num_distract_docs = (
             min(self.num_distract_docs, len(chunks)) - 1
         )  # should be less than number of chunks/ nodes created
 
         for index, chunk in enumerate(chunks):
-            logging.info(f"Processing chunk: {index}")
+            logger.info(f"Processing chunk: {index}")
             self.add_chunk_to_dataset(
                 chunks, chunk, self.num_questions_per_chunk, self.num_distract_docs
             )
 
         return self.ds
```

### Comparing `llama_index_packs_raft_dataset-0.1.4/pyproject.toml` & `llama_index_packs_raft_dataset-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 description = "llama-index packs RAFT Dataset paper implementation"
 exclude = ["**/BUILD"]
 keywords = ["finetuning", "raft", "raft_dataset"]
 license = "MIT"
 maintainers = ["ravi-theja"]
 name = "llama-index-packs-raft-dataset"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.0"
 datasets = "^2.18.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_packs_raft_dataset-0.1.4/PKG-INFO` & `llama_index_packs_raft_dataset-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-packs-raft-dataset
-Version: 0.1.4
+Version: 0.1.5
 Summary: llama-index packs RAFT Dataset paper implementation
 License: MIT
 Keywords: finetuning,raft,raft_dataset
 Author: Ravi Theja
 Author-email: ravi03071991@gmail.com
 Maintainer: ravi-theja
 Requires-Python: >=3.8.1,<4.0
```

