# Comparing `tmp/llmsmith-0.4.0.tar.gz` & `tmp/llmsmith-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmsmith-0.4.0.tar", max compression
+gzip compressed data, was "llmsmith-0.5.0.tar", max compression
```

## Comparing `llmsmith-0.4.0.tar` & `llmsmith-0.5.0.tar`

### file list

```diff
@@ -1,43 +1,47 @@
--rw-r--r--   0        0        0     1101 2024-04-03 09:01:34.959168 llmsmith-0.4.0/LICENSE
--rw-r--r--   0        0        0     1506 2024-04-30 06:58:37.514663 llmsmith-0.4.0/README.md
--rw-r--r--   0        0        0       78 2024-03-15 04:21:07.861053 llmsmith-0.4.0/llmsmith/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 12:18:59.343170 llmsmith-0.4.0/llmsmith/agent/__init__.py
--rw-r--r--   0        0        0      209 2024-04-18 09:12:45.143269 llmsmith-0.4.0/llmsmith/agent/errors.py
--rw-r--r--   0        0        0        0 2024-04-15 12:19:30.041692 llmsmith-0.4.0/llmsmith/agent/function/__init__.py
--rw-r--r--   0        0        0     5934 2024-04-29 11:21:40.340274 llmsmith-0.4.0/llmsmith/agent/function/gemini.py
--rw-r--r--   0        0        0     8897 2024-04-30 06:33:06.377475 llmsmith-0.4.0/llmsmith/agent/function/openai.py
--rw-r--r--   0        0        0        0 2024-04-23 05:43:58.075908 llmsmith-0.4.0/llmsmith/agent/function/options/__init__.py
--rw-r--r--   0        0        0     1996 2024-04-30 04:53:53.672366 llmsmith-0.4.0/llmsmith/agent/function/options/openai.py
--rw-r--r--   0        0        0        0 2024-04-18 05:26:07.193675 llmsmith-0.4.0/llmsmith/agent/tool/__init__.py
--rw-r--r--   0        0        0     1013 2024-04-18 12:17:09.379744 llmsmith-0.4.0/llmsmith/agent/tool/gemini.py
--rw-r--r--   0        0        0     2001 2024-04-29 11:21:40.340139 llmsmith-0.4.0/llmsmith/agent/tool/openai.py
--rw-r--r--   0        0        0        0 2024-03-14 11:47:53.187559 llmsmith-0.4.0/llmsmith/job/__init__.py
--rw-r--r--   0        0        0     7428 2024-04-02 12:37:57.531013 llmsmith-0.4.0/llmsmith/job/base.py
--rw-r--r--   0        0        0     8550 2024-04-03 05:58:40.426172 llmsmith-0.4.0/llmsmith/job/job.py
--rw-r--r--   0        0        0        0 2024-04-30 12:02:50.437340 llmsmith-0.4.0/llmsmith/reranker/__init__.py
--rw-r--r--   0        0        0      575 2024-05-02 04:19:45.995736 llmsmith-0.4.0/llmsmith/reranker/base.py
--rw-r--r--   0        0        0     2848 2024-05-02 05:39:34.864251 llmsmith-0.4.0/llmsmith/reranker/cohere.py
--rw-r--r--   0        0        0        0 2024-05-02 03:46:41.851482 llmsmith-0.4.0/llmsmith/reranker/options/__init__.py
--rw-r--r--   0        0        0     1088 2024-05-02 04:19:45.995262 llmsmith-0.4.0/llmsmith/reranker/options/cohere.py
--rw-r--r--   0        0        0        0 2024-03-14 11:03:16.994184 llmsmith-0.4.0/llmsmith/task/__init__.py
--rw-r--r--   0        0        0     1329 2024-04-02 12:23:38.410395 llmsmith-0.4.0/llmsmith/task/base.py
--rw-r--r--   0        0        0      437 2024-04-22 10:15:31.395712 llmsmith-0.4.0/llmsmith/task/models.py
--rw-r--r--   0        0        0        0 2024-03-15 07:53:27.486482 llmsmith-0.4.0/llmsmith/task/retrieval/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 07:44:57.026421 llmsmith-0.4.0/llmsmith/task/retrieval/vector/__init__.py
--rw-r--r--   0        0        0      437 2024-05-01 10:16:21.291906 llmsmith-0.4.0/llmsmith/task/retrieval/vector/base.py
--rw-r--r--   0        0        0     3724 2024-05-01 10:16:21.291224 llmsmith-0.4.0/llmsmith/task/retrieval/vector/chromadb.py
--rw-r--r--   0        0        0        0 2024-04-09 12:03:40.797998 llmsmith-0.4.0/llmsmith/task/retrieval/vector/options/__init__.py
--rw-r--r--   0        0        0      906 2024-04-10 13:01:55.980002 llmsmith-0.4.0/llmsmith/task/retrieval/vector/options/chromadb.py
--rw-r--r--   0        0        0     1325 2024-04-10 05:42:08.573365 llmsmith-0.4.0/llmsmith/task/retrieval/vector/options/qdrant.py
--rw-r--r--   0        0        0     4304 2024-05-01 10:31:04.487709 llmsmith-0.4.0/llmsmith/task/retrieval/vector/qdrant.py
--rw-r--r--   0        0        0        0 2024-03-15 11:22:26.459597 llmsmith-0.4.0/llmsmith/task/textgen/__init__.py
--rw-r--r--   0        0        0     3042 2024-04-04 09:07:05.709627 llmsmith-0.4.0/llmsmith/task/textgen/claude.py
--rw-r--r--   0        0        0      681 2024-04-18 12:18:54.653626 llmsmith-0.4.0/llmsmith/task/textgen/errors.py
--rw-r--r--   0        0        0     7108 2024-04-29 11:21:40.339852 llmsmith-0.4.0/llmsmith/task/textgen/gemini.py
--rw-r--r--   0        0        0     6447 2024-04-29 11:21:40.339843 llmsmith-0.4.0/llmsmith/task/textgen/openai.py
--rw-r--r--   0        0        0        0 2024-03-19 08:37:09.919088 llmsmith-0.4.0/llmsmith/task/textgen/options/__init__.py
--rw-r--r--   0        0        0     1498 2024-04-04 09:30:06.753059 llmsmith-0.4.0/llmsmith/task/textgen/options/claude.py
--rw-r--r--   0        0        0     1346 2024-04-18 07:13:19.756541 llmsmith-0.4.0/llmsmith/task/textgen/options/gemini.py
--rw-r--r--   0        0        0     1890 2024-04-22 08:24:34.750821 llmsmith-0.4.0/llmsmith/task/textgen/options/openai.py
--rw-r--r--   0        0        0     1922 2024-05-03 11:25:28.691081 llmsmith-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3305 1970-01-01 00:00:00.000000 llmsmith-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1101 2024-04-03 09:01:34.959168 llmsmith-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1517 2024-05-07 11:18:28.748569 llmsmith-0.5.0/README.md
+-rw-r--r--   0        0        0       78 2024-03-15 04:21:07.861053 llmsmith-0.5.0/llmsmith/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 12:18:59.343170 llmsmith-0.5.0/llmsmith/agent/__init__.py
+-rw-r--r--   0        0        0      209 2024-04-18 09:12:45.143269 llmsmith-0.5.0/llmsmith/agent/errors.py
+-rw-r--r--   0        0        0        0 2024-04-15 12:19:30.041692 llmsmith-0.5.0/llmsmith/agent/function/__init__.py
+-rw-r--r--   0        0        0     5618 2024-05-07 11:09:56.773034 llmsmith-0.5.0/llmsmith/agent/function/cohere.py
+-rw-r--r--   0        0        0     5926 2024-05-07 11:14:41.988980 llmsmith-0.5.0/llmsmith/agent/function/gemini.py
+-rw-r--r--   0        0        0     8889 2024-05-07 11:14:54.558351 llmsmith-0.5.0/llmsmith/agent/function/openai.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:43:58.075908 llmsmith-0.5.0/llmsmith/agent/function/options/__init__.py
+-rw-r--r--   0        0        0     1985 2024-05-07 12:01:42.276643 llmsmith-0.5.0/llmsmith/agent/function/options/openai.py
+-rw-r--r--   0        0        0        0 2024-04-18 05:26:07.193675 llmsmith-0.5.0/llmsmith/agent/tool/__init__.py
+-rw-r--r--   0        0        0      898 2024-05-06 11:04:31.823036 llmsmith-0.5.0/llmsmith/agent/tool/cohere.py
+-rw-r--r--   0        0        0     1014 2024-05-07 11:15:14.677758 llmsmith-0.5.0/llmsmith/agent/tool/gemini.py
+-rw-r--r--   0        0        0     2002 2024-05-07 11:15:20.017868 llmsmith-0.5.0/llmsmith/agent/tool/openai.py
+-rw-r--r--   0        0        0        0 2024-03-14 11:47:53.187559 llmsmith-0.5.0/llmsmith/job/__init__.py
+-rw-r--r--   0        0        0     7428 2024-04-02 12:37:57.531013 llmsmith-0.5.0/llmsmith/job/base.py
+-rw-r--r--   0        0        0     8550 2024-04-03 05:58:40.426172 llmsmith-0.5.0/llmsmith/job/job.py
+-rw-r--r--   0        0        0        0 2024-04-30 12:02:50.437340 llmsmith-0.5.0/llmsmith/reranker/__init__.py
+-rw-r--r--   0        0        0      575 2024-05-02 04:19:45.995736 llmsmith-0.5.0/llmsmith/reranker/base.py
+-rw-r--r--   0        0        0     2849 2024-05-07 11:15:37.535755 llmsmith-0.5.0/llmsmith/reranker/cohere.py
+-rw-r--r--   0        0        0        0 2024-05-02 03:46:41.851482 llmsmith-0.5.0/llmsmith/reranker/options/__init__.py
+-rw-r--r--   0        0        0     1082 2024-05-07 11:15:49.065554 llmsmith-0.5.0/llmsmith/reranker/options/cohere.py
+-rw-r--r--   0        0        0        0 2024-03-14 11:03:16.994184 llmsmith-0.5.0/llmsmith/task/__init__.py
+-rw-r--r--   0        0        0     1329 2024-04-02 12:23:38.410395 llmsmith-0.5.0/llmsmith/task/base.py
+-rw-r--r--   0        0        0      437 2024-04-22 10:15:31.395712 llmsmith-0.5.0/llmsmith/task/models.py
+-rw-r--r--   0        0        0        0 2024-03-15 07:53:27.486482 llmsmith-0.5.0/llmsmith/task/retrieval/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 07:44:57.026421 llmsmith-0.5.0/llmsmith/task/retrieval/vector/__init__.py
+-rw-r--r--   0        0        0      437 2024-05-01 10:16:21.291906 llmsmith-0.5.0/llmsmith/task/retrieval/vector/base.py
+-rw-r--r--   0        0        0     3715 2024-05-07 11:16:01.033751 llmsmith-0.5.0/llmsmith/task/retrieval/vector/chromadb.py
+-rw-r--r--   0        0        0        0 2024-04-09 12:03:40.797998 llmsmith-0.5.0/llmsmith/task/retrieval/vector/options/__init__.py
+-rw-r--r--   0        0        0      897 2024-05-07 11:16:13.459211 llmsmith-0.5.0/llmsmith/task/retrieval/vector/options/chromadb.py
+-rw-r--r--   0        0        0     1316 2024-05-07 11:16:18.001301 llmsmith-0.5.0/llmsmith/task/retrieval/vector/options/qdrant.py
+-rw-r--r--   0        0        0     4295 2024-05-07 11:16:06.806987 llmsmith-0.5.0/llmsmith/task/retrieval/vector/qdrant.py
+-rw-r--r--   0        0        0        0 2024-03-15 11:22:26.459597 llmsmith-0.5.0/llmsmith/task/textgen/__init__.py
+-rw-r--r--   0        0        0     3036 2024-05-07 11:16:24.273688 llmsmith-0.5.0/llmsmith/task/textgen/claude.py
+-rw-r--r--   0        0        0     6108 2024-05-07 04:06:44.987359 llmsmith-0.5.0/llmsmith/task/textgen/cohere.py
+-rw-r--r--   0        0        0      681 2024-04-18 12:18:54.653626 llmsmith-0.5.0/llmsmith/task/textgen/errors.py
+-rw-r--r--   0        0        0     7102 2024-05-07 11:16:33.346249 llmsmith-0.5.0/llmsmith/task/textgen/gemini.py
+-rw-r--r--   0        0        0     6441 2024-05-07 11:16:37.844109 llmsmith-0.5.0/llmsmith/task/textgen/openai.py
+-rw-r--r--   0        0        0        0 2024-03-19 08:37:09.919088 llmsmith-0.5.0/llmsmith/task/textgen/options/__init__.py
+-rw-r--r--   0        0        0     1489 2024-05-07 11:16:43.800922 llmsmith-0.5.0/llmsmith/task/textgen/options/claude.py
+-rw-r--r--   0        0        0     2317 2024-05-07 12:16:46.722433 llmsmith-0.5.0/llmsmith/task/textgen/options/cohere.py
+-rw-r--r--   0        0        0     1337 2024-05-07 11:16:51.095809 llmsmith-0.5.0/llmsmith/task/textgen/options/gemini.py
+-rw-r--r--   0        0        0     1881 2024-05-07 11:16:55.681932 llmsmith-0.5.0/llmsmith/task/textgen/options/openai.py
+-rw-r--r--   0        0        0     1922 2024-05-07 13:09:53.143679 llmsmith-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3316 1970-01-01 00:00:00.000000 llmsmith-0.5.0/PKG-INFO
```

### Comparing `llmsmith-0.4.0/LICENSE` & `llmsmith-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llmsmith-0.4.0/README.md` & `llmsmith-0.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 Here's the list of extra dependencies supported by LLMSmith:
 - `openai`
 - `claude`
 - `gemini`
 - `chromadb`
 - `qdrant`
+- `cohere`
 - `all` (downloads all extra dependencies)
 
 ## Example
 
 Refer [this](https://llmsmith.readthedocs.io/en/latest/examples.html) page from the documentation to see examples on how LLMSmith can be used to build LLM powered functionalities.
 
 ## Documentation
```

### Comparing `llmsmith-0.4.0/llmsmith/agent/function/gemini.py` & `llmsmith-0.5.0/llmsmith/agent/function/gemini.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
         FunctionDeclaration,
         FunctionResponse,
         Tool,
     )
     from google.generativeai import GenerativeModel
 except ImportError:
     raise ImportError(
-        "The 'google.generativeai' library is required to use GeminiFunctionAgent. You can install it with `pip install \"llmsmith[gemini]\"`"
+        "The 'google.generativeai' library is required to use Gemini LLMs. You can install it with `pip install \"llmsmith[gemini]\"`"
     )
 
 import logging
 from typing import Callable, List
 from llmsmith.agent.errors import MaxTurnsReachedException
 from llmsmith.agent.tool.gemini import GeminiTool
 from llmsmith.task.base import Task
```

### Comparing `llmsmith-0.4.0/llmsmith/agent/function/openai.py` & `llmsmith-0.5.0/llmsmith/agent/function/openai.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 try:
     import openai
     from openai.types.beta import Assistant, Thread
     from openai.types.beta.threads import Run
 except ImportError:
     raise ImportError(
-        "The 'openai' library is required to use OpenAIFunctionAgent. You can install it with `pip install \"llmsmith[openai]\"`"
+        "The 'openai' library is required to use OpenAI LLMs. You can install it with `pip install \"llmsmith[openai]\"`"
     )
 
 import json
 import logging
 from typing import Callable, List
 
 from llmsmith.agent.errors import MaxTurnsReachedException
```

### Comparing `llmsmith-0.4.0/llmsmith/agent/function/options/openai.py` & `llmsmith-0.5.0/llmsmith/agent/function/options/openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     from openai._types import Headers, Query, Body
     from openai.types.beta.assistant_create_params import ToolResources
     from openai.types.beta.assistant_response_format_option_param import (
         AssistantResponseFormatOptionParam,
     )
 except ImportError:
     raise ImportError(
-        "The 'openai' library is required to use OpenAIAssistantOptions. You can install it with `pip install \"llmsmith[openai]\"`"
+        "The 'openai' library is required to use OpenAI LLMs. You can install it with `pip install \"llmsmith[openai]\"`"
     )
 
 
 class OpenAIAssistantOptions(TypedDict):
     """
     A dictionary of options to be passed into the OpenAI assistant APIs.
     The option names are same as the ones used in OpenAI client (except `system_prompt`, which replaces `instructions` option).
```

### Comparing `llmsmith-0.4.0/llmsmith/agent/tool/gemini.py` & `llmsmith-0.5.0/llmsmith/agent/tool/gemini.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Callable
 
 
 try:
     from google.ai.generativelanguage_v1beta.types import FunctionDeclaration
 except ImportError:
     raise ImportError(
-        "The 'google.generativeai' library is required to use GeminiTool. You can install it with `pip install \"llmsmith[gemini]\"`"
+        "The 'google.generativeai' library is required to use Gemini LLMs. You can install it with `pip install \"llmsmith[gemini]\"`"
     )
 
 
 class GeminiTool:
     """
     Wrapper for both function declaration and the actual callable to be used in Gemini LLMs.
```

### Comparing `llmsmith-0.4.0/llmsmith/agent/tool/openai.py` & `llmsmith-0.5.0/llmsmith/agent/tool/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 try:
     from openai.types.shared_params import FunctionDefinition
     from openai.types.beta.assistant_tool_param import AssistantToolParam
 except ImportError:
     raise ImportError(
-        "The 'openai' library is required to use OpenAITool. You can install it with `pip install \"llmsmith[openai]\"`"
+        "The 'openai' library is required to use OpenAI LLMs. You can install it with `pip install \"llmsmith[openai]\"`"
     )
 
 
 class OpenAIChatTool:
     """
     Wrapper for both function declaration and the actual callable to be used in chat completion APIs.
```

### Comparing `llmsmith-0.4.0/llmsmith/job/base.py` & `llmsmith-0.5.0/llmsmith/job/base.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.4.0/llmsmith/job/job.py` & `llmsmith-0.5.0/llmsmith/job/job.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.4.0/llmsmith/reranker/base.py` & `llmsmith-0.5.0/llmsmith/reranker/base.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.4.0/llmsmith/reranker/cohere.py` & `llmsmith-0.5.0/llmsmith/reranker/cohere.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     import cohere
     from cohere.types.rerank_request_documents_item import (
         RerankRequestDocumentsItemText,
     )
     from cohere.types.rerank_response import RerankResponse
 except ImportError:
     raise ImportError(
-        "The 'cohere' library is required to use CohereReranker. You can install it with `pip install \"llmsmith[cohere]\"`"
+        "The 'cohere' library is required to use Cohere reranker. You can install it with `pip install \"llmsmith[cohere]\"`"
     )
 
 
 log = logging.getLogger(__name__)
 
 
 class CohereReranker(Reranker):
```

### Comparing `llmsmith-0.4.0/llmsmith/reranker/options/cohere.py` & `llmsmith-0.5.0/llmsmith/reranker/options/cohere.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List, TypedDict, Union
 
 try:
     from cohere.core.request_options import RequestOptions
 except ImportError:
     raise ImportError(
-        "The 'cohere' library is required to use CohereRerankerOptions. You can install it with `pip install \"llmsmith[cohere]\"`"
+        "The 'cohere' library is required to use Cohere reranker. You can install it with `pip install \"llmsmith[cohere]\"`"
     )
 
 
 class CohereRerankerOptions(TypedDict):
     """
     A dictionary of options to be passed into Cohere reranker.
     The option names are same as the ones used in the reranker method of Cohere client.
```

### Comparing `llmsmith-0.4.0/llmsmith/task/base.py` & `llmsmith-0.5.0/llmsmith/task/base.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.4.0/llmsmith/task/retrieval/vector/chromadb.py` & `llmsmith-0.5.0/llmsmith/task/retrieval/vector/chromadb.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 )
 
 
 try:
     from chromadb import Collection, QueryResult
 except ImportError:
     raise ImportError(
-        "The 'chromadb-client' library is required to use ChromaDBRetriever. You can install it with `pip install \"llmsmith[chromadb]\"`"
+        "The 'chromadb-client' library is required to use ChromaDB. You can install it with `pip install \"llmsmith[chromadb]\"`"
     )
 
 
 log = logging.getLogger(__name__)
 
 # Default options for querying a Qdrant collection.
 default_options: ChromaDBQueryOptions = ChromaDBQueryOptions(n_results=10)
```

### Comparing `llmsmith-0.4.0/llmsmith/task/retrieval/vector/options/chromadb.py` & `llmsmith-0.5.0/llmsmith/task/retrieval/vector/options/chromadb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import TypedDict
 
 try:
     from chromadb import Where, WhereDocument
 except ImportError:
     raise ImportError(
-        "The 'chromadb-client' library is required to use ChromaDBRetriever. You can install it with `pip install \"llmsmith[chromadb]\"`"
+        "The 'chromadb-client' library is required to use ChromaDB. You can install it with `pip install \"llmsmith[chromadb]\"`"
     )
 
 
 class ChromaDBQueryOptions(TypedDict):
     """
     A dictionary of options to pass while querying a Chroma DB collection.
     The option names are same as the ones used in `query` method of ChromaDB `Collection` client.
```

### Comparing `llmsmith-0.4.0/llmsmith/task/retrieval/vector/options/qdrant.py` & `llmsmith-0.5.0/llmsmith/task/retrieval/vector/options/qdrant.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
         Filter,
         SearchParams,
         ReadConsistency,
         ShardKeySelector,
     )
 except ImportError:
     raise ImportError(
-        "The 'qdrant-client' library is required to use QdrantRetriever. You can install it with `pip install \"llmsmith[qdrant]\"`"
+        "The 'qdrant-client' library is required to use Qdrant. You can install it with `pip install \"llmsmith[qdrant]\"`"
     )
 
 
 class QdrantQueryOptions(TypedDict):
     """
     A dictionary of options to pass while querying a qdrant collection.
     The option names are same as the ones used in `search` method of AsyncQdrantClient.
```

### Comparing `llmsmith-0.4.0/llmsmith/task/retrieval/vector/qdrant.py` & `llmsmith-0.5.0/llmsmith/task/retrieval/vector/qdrant.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 )
 
 try:
     from qdrant_client import AsyncQdrantClient
     from qdrant_client.conversions.common_types import ScoredPoint
 except ImportError:
     raise ImportError(
-        "The 'qdrant-client' library is required to use QdrantRetriever. You can install it with `pip install \"llmsmith[qdrant]\"`"
+        "The 'qdrant-client' library is required to use Qdrant. You can install it with `pip install \"llmsmith[qdrant]\"`"
     )
 
 
 log = logging.getLogger(__name__)
 
 # Default options for querying a Qdrant collection.
 default_options: QdrantQueryOptions = QdrantQueryOptions(limit=10, with_vectors=False)
```

### Comparing `llmsmith-0.4.0/llmsmith/task/textgen/claude.py` & `llmsmith-0.5.0/llmsmith/task/textgen/claude.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import List
 
 try:
     import anthropic
     from anthropic.types.message import Message
 except ImportError:
     raise ImportError(
-        "The 'anthropic' library is required to use ClaudeTextGenTask. You can install it with `pip install \"llmsmith[claude]\"`"
+        "The 'anthropic' library is required to use Claude LLMs. You can install it with `pip install \"llmsmith[claude]\"`"
     )
 
 from llmsmith.task.base import Task
 from llmsmith.task.models import TaskInput, TaskOutput
 from llmsmith.task.textgen.options.claude import (
     ClaudeTextGenOptions,
     _completion_create_options_dict,
```

### Comparing `llmsmith-0.4.0/llmsmith/task/textgen/errors.py` & `llmsmith-0.5.0/llmsmith/task/textgen/errors.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.4.0/llmsmith/task/textgen/gemini.py` & `llmsmith-0.5.0/llmsmith/task/textgen/gemini.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from google.generativeai.types import GenerateContentResponse
     from google.generativeai.types.content_types import (
         ContentsType,
         FunctionLibraryType,
     )
 except ImportError:
     raise ImportError(
-        "The 'google.generativeai' library is required to use GeminiTextGenTask. You can install it with `pip install \"llmsmith[gemini]\"`"
+        "The 'google.generativeai' library is required to use Gemini LLMs. You can install it with `pip install \"llmsmith[gemini]\"`"
     )
 
 from llmsmith.task.base import Task
 from llmsmith.task.models import ChatResponse, TaskInput, TaskOutput
 from llmsmith.task.models import FunctionCall as LLMFunctionCall
 from llmsmith.task.textgen.options.gemini import (
     GeminiTextGenOptions,
```

### Comparing `llmsmith-0.4.0/llmsmith/task/textgen/openai.py` & `llmsmith-0.5.0/llmsmith/task/textgen/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from openai.types.chat.chat_completion import ChatCompletion
     from openai.types.chat.chat_completion_message_param import (
         ChatCompletionMessageParam,
     )
     from openai.types.chat.chat_completion_tool_param import ChatCompletionToolParam
 except ImportError:
     raise ImportError(
-        "The 'openai' library is required to use OpenAITextGenTask. You can install it with `pip install \"llmsmith[openai]\"`"
+        "The 'openai' library is required to use OpenAI LLMs. You can install it with `pip install \"llmsmith[openai]\"`"
     )
 
 from llmsmith.task.base import Task
 from llmsmith.task.models import ChatResponse, FunctionCall, TaskInput, TaskOutput
 from llmsmith.task.textgen.options.openai import (
     OpenAITextGenOptions,
     _completion_create_options_dict,
```

### Comparing `llmsmith-0.4.0/llmsmith/task/textgen/options/claude.py` & `llmsmith-0.5.0/llmsmith/task/textgen/options/claude.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List, Mapping, TypedDict, Union
 
 try:
     from anthropic.types.message_create_params import Metadata
 except ImportError:
     raise ImportError(
-        "The 'anthropic' library is required to use ClaudeTextGenOptions. You can install it with `pip install \"llmsmith[claude]\"`"
+        "The 'anthropic' library is required to use Claude LLMs. You can install it with `pip install \"llmsmith[claude]\"`"
     )
 
 
 class ClaudeTextGenOptions(TypedDict):
     """
     A dictionary of options to pass to the Anthropic Claude LLM for text generation.
     The option names are same as the ones used in Anthropic client.
```

### Comparing `llmsmith-0.4.0/llmsmith/task/textgen/options/gemini.py` & `llmsmith-0.5.0/llmsmith/task/textgen/options/gemini.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, TypedDict, Union
 
 try:
     from google.generativeai.types.generation_types import GenerationConfigType
     from google.generativeai.types.safety_types import SafetySettingOptions
 except ImportError:
     raise ImportError(
-        "The 'google.generativeai' library is required to use GeminiTextGenOptions. You can install it with `pip install \"llmsmith[gemini]\"`"
+        "The 'google.generativeai' library is required to use Gemini LLMs. You can install it with `pip install \"llmsmith[gemini]\"`"
     )
 
 
 class GeminiTextGenOptions(TypedDict):
     """
     A dictionary of options to pass to the Google Gemini LLM for text generation.
     The option names are same as the ones used in Gemini client.
```

### Comparing `llmsmith-0.4.0/llmsmith/task/textgen/options/openai.py` & `llmsmith-0.5.0/llmsmith/task/textgen/options/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 try:
     from openai.types.chat.completion_create_params import ResponseFormat
     from openai.types.chat.chat_completion_tool_choice_option_param import (
         ChatCompletionToolChoiceOptionParam,
     )
 except ImportError:
     raise ImportError(
-        "The 'openai' library is required to use OpenAITextGenOptions. You can install it with `pip install \"llmsmith[openai]\"`"
+        "The 'openai' library is required to use OpenAI LLMs. You can install it with `pip install \"llmsmith[openai]\"`"
     )
 
 
 class OpenAITextGenOptions(TypedDict):
     """
     A dictionary of options to pass to the OpenAI LLM for text generation.
     The option names are same as the ones used in OpenAI client (except `system_prompt`, which is an extra).
```

### Comparing `llmsmith-0.4.0/pyproject.toml` & `llmsmith-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "LLMSmith"
-version = "0.4.0"
+version = "0.5.0"
 description = "Lightweight Python library designed for developing functionalities powered by Large Language Models (LLMs)"
 authors = ["Dheeraj Gopinath <dheeraj.gopinath@gmail.com>"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `llmsmith-0.4.0/PKG-INFO` & `llmsmith-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LLMSmith
-Version: 0.4.0
+Version: 0.5.0
 Summary: Lightweight Python library designed for developing functionalities powered by Large Language Models (LLMs)
 Author: Dheeraj Gopinath
 Author-email: dheeraj.gopinath@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -54,14 +54,15 @@
 
 Here's the list of extra dependencies supported by LLMSmith:
 - `openai`
 - `claude`
 - `gemini`
 - `chromadb`
 - `qdrant`
+- `cohere`
 - `all` (downloads all extra dependencies)
 
 ## Example
 
 Refer [this](https://llmsmith.readthedocs.io/en/latest/examples.html) page from the documentation to see examples on how LLMSmith can be used to build LLM powered functionalities.
 
 ## Documentation
```

