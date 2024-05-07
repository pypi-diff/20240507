# Comparing `tmp/llama_index_readers_openalex-0.1.3.tar.gz` & `tmp/llama_index_readers_openalex-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_openalex-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_readers_openalex-0.1.4.tar", max compression
```

## Comparing `llama_index_readers_openalex-0.1.3.tar` & `llama_index_readers_openalex-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1951 2024-02-13 13:53:01.846413 llama_index_readers_openalex-0.1.3/README.md
--rw-r--r--   0        0        0      108 2024-02-13 13:53:01.846914 llama_index_readers_openalex-0.1.3/llama_index/readers/openalex/__init__.py
--rw-r--r--   0        0        0     4406 2024-02-13 13:53:01.846974 llama_index_readers_openalex-0.1.3/llama_index/readers/openalex/base.py
--rw-r--r--   0        0        0     1545 2024-02-21 20:31:54.962967 llama_index_readers_openalex-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2644 1970-01-01 00:00:00.000000 llama_index_readers_openalex-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2008 2024-05-07 16:26:08.891052 llama_index_readers_openalex-0.1.4/README.md
+-rw-r--r--   0        0        0      108 2024-05-07 16:26:08.891052 llama_index_readers_openalex-0.1.4/llama_index/readers/openalex/__init__.py
+-rw-r--r--   0        0        0     4427 2024-05-07 16:26:08.891052 llama_index_readers_openalex-0.1.4/llama_index/readers/openalex/base.py
+-rw-r--r--   0        0        0     1545 2024-05-07 16:26:08.891052 llama_index_readers_openalex-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2650 1970-01-01 00:00:00.000000 llama_index_readers_openalex-0.1.4/PKG-INFO
```

### Comparing `llama_index_readers_openalex-0.1.3/README.md` & `llama_index_readers_openalex-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # OpenAlex Reader
 
+```bash
+pip install llama-index-readers-openalex
+```
+
 This loader will search for papers in OpenAlex and load them in llama-index. The main advantage of using OpenAlex is that you can search the full-text for Open Access papers as well.
 
 ## Usage
 
 ```python
-from llama_hub.openalex_loader import OpenAlexReader
+from llama_index.readers.openalex import OpenAlexReader
 
 openalex_reader = OpenAlexReader(email="shauryr@gmail.com")
 query = "biases in large language models"
 
 # changing this to full_text=True will let you search full-text
 documents = openalex_reader.load_data(query, full_text=False)
 ```
```

### Comparing `llama_index_readers_openalex-0.1.3/llama_index/readers/openalex/base.py` & `llama_index_readers_openalex-0.1.4/llama_index/readers/openalex/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import logging
 from typing import List
 
 import requests
 from llama_index.core.readers.base import BaseReader
 from llama_index.core.schema import Document
 
-logging.basicConfig(level=logging.ERROR)
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.ERROR)
 
 
 class OpenAlexReader(BaseReader):
     """
     This class is used to search and import data from OpenAlex.
 
     Parameters
@@ -42,19 +43,19 @@
             response = requests.get(full_url, timeout=10)
             response.raise_for_status()  # Check if request is successful
             data = response.json()  # Parse JSON data
             if "error" in data:
                 raise ValueError(f"API returned error: {data['error']}")
             return data
         except requests.exceptions.HTTPError as http_error:
-            logging.error(f"HTTP error occurred: {http_error}")
+            logger.error(f"HTTP error occurred: {http_error}")
         except requests.exceptions.RequestException as request_error:
-            logging.error(f"Error occurred: {request_error}")
+            logger.error(f"Error occurred: {request_error}")
         except ValueError as value_error:
-            logging.error(value_error)
+            logger.error(value_error)
         return None
 
     def _fulltext_search_openalex(self, query, fields):
         base_url = "https://api.openalex.org/works?filter=fulltext.search:"
         fields_param = f"&select={fields}"
         email_param = f"&mailto={self.email}"
         full_url = base_url + query + fields_param + email_param
@@ -62,19 +63,19 @@
             response = requests.get(full_url, timeout=10)
             response.raise_for_status()  # Check if request is successful
             data = response.json()  # Parse JSON data
             if "error" in data:
                 raise ValueError(f"API returned error: {data['error']}")
             return data
         except requests.exceptions.HTTPError as http_error:
-            logging.error(f"HTTP error occurred: {http_error}")
+            logger.error(f"HTTP error occurred: {http_error}")
         except requests.exceptions.RequestException as request_error:
-            logging.error(f"Error occurred: {request_error}")
+            logger.error(f"Error occurred: {request_error}")
         except ValueError as value_error:
-            logging.error(value_error)
+            logger.error(value_error)
         return None
 
     def _invert_abstract(self, inv_index):
         if inv_index is not None:
             l_inv = [(w, p) for w, pos in inv_index.items() for p in pos]
             return " ".join(x[0] for x in sorted(l_inv, key=lambda x: x[1]))
         return None
```

### Comparing `llama_index_readers_openalex-0.1.3/pyproject.toml` & `llama_index_readers_openalex-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 description = "llama-index readers openalex integration"
 exclude = ["**/BUILD"]
 keywords = ["academic papers", "open access", "openalex", "scientific papers"]
 license = "MIT"
 maintainers = ["shauryr"]
 name = "llama-index-readers-openalex"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
```

### Comparing `llama_index_readers_openalex-0.1.3/PKG-INFO` & `llama_index_readers_openalex-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-openalex
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index readers openalex integration
 License: MIT
 Keywords: academic papers,open access,openalex,scientific papers
 Author: Your Name
 Author-email: you@example.com
 Maintainer: shauryr
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Description-Content-Type: text/markdown
 
 # OpenAlex Reader
 
+```bash
+pip install llama-index-readers-openalex
+```
+
 This loader will search for papers in OpenAlex and load them in llama-index. The main advantage of using OpenAlex is that you can search the full-text for Open Access papers as well.
 
 ## Usage
 
 ```python
-from llama_hub.openalex_loader import OpenAlexReader
+from llama_index.readers.openalex import OpenAlexReader
 
 openalex_reader = OpenAlexReader(email="shauryr@gmail.com")
 query = "biases in large language models"
 
 # changing this to full_text=True will let you search full-text
 documents = openalex_reader.load_data(query, full_text=False)
 ```
```

