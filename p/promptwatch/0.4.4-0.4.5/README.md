# Comparing `tmp/promptwatch-0.4.4.tar.gz` & `tmp/promptwatch-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptwatch-0.4.4.tar", last modified: Mon Feb 12 07:42:05 2024, max compression
+gzip compressed data, was "promptwatch-0.4.5.tar", last modified: Mon May  6 22:22:02 2024, max compression
```

## Comparing `promptwatch-0.4.4.tar` & `promptwatch-0.4.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-02-12 07:42:05.102841 promptwatch-0.4.4/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2024-02-12 07:42:05.102670 promptwatch-0.4.4/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3584 2023-05-19 10:25:10.000000 promptwatch-0.4.4/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.4.4/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2024-02-12 07:42:05.102883 promptwatch-0.4.4/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1198 2023-05-24 21:47:14.000000 promptwatch-0.4.4/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-02-12 07:42:05.093989 promptwatch-0.4.4/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-02-12 07:42:05.098133 promptwatch-0.4.4/src/promptwatch/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      440 2024-02-12 07:40:32.000000 promptwatch-0.4.4/src/promptwatch/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    16570 2023-12-18 22:16:50.000000 promptwatch-0.4.4/src/promptwatch/caching.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     6214 2023-09-08 19:28:50.000000 promptwatch-0.4.4/src/promptwatch/client.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      260 2023-05-19 10:25:10.000000 promptwatch-0.4.4/src/promptwatch/constants.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     5701 2023-09-08 19:29:25.000000 promptwatch-0.4.4/src/promptwatch/data_model.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1555 2023-05-23 20:20:02.000000 promptwatch-0.4.4/src/promptwatch/decorators.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-02-12 07:42:05.100552 promptwatch-0.4.4/src/promptwatch/langchain/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      219 2023-05-30 19:26:54.000000 promptwatch-0.4.4/src/promptwatch/langchain/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    13208 2023-12-21 12:55:25.000000 promptwatch-0.4.4/src/promptwatch/langchain/caching.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    32492 2023-12-02 20:43:18.000000 promptwatch-0.4.4/src/promptwatch/langchain/langchain_support.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4277 2024-02-11 22:51:29.000000 promptwatch-0.4.4/src/promptwatch/langchain/unit_tests.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    21220 2023-12-21 12:52:52.000000 promptwatch-0.4.4/src/promptwatch/promptwatch_context.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-02-12 07:42:05.102049 promptwatch-0.4.4/src/promptwatch/unit_tests/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      162 2023-05-19 10:25:10.000000 promptwatch-0.4.4/src/promptwatch/unit_tests/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    13477 2024-02-11 22:52:28.000000 promptwatch-0.4.4/src/promptwatch/unit_tests/evaluation.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3247 2023-09-08 19:30:11.000000 promptwatch-0.4.4/src/promptwatch/unit_tests/schema.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    24610 2023-08-22 19:21:36.000000 promptwatch-0.4.4/src/promptwatch/unit_tests/unit_tests.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     2368 2023-06-17 16:42:18.000000 promptwatch-0.4.4/src/promptwatch/utils.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-02-12 07:42:05.099371 promptwatch-0.4.4/src/promptwatch.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2024-02-12 07:42:05.000000 promptwatch-0.4.4/src/promptwatch.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      819 2024-02-12 07:42:05.000000 promptwatch-0.4.4/src/promptwatch.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2024-02-12 07:42:05.000000 promptwatch-0.4.4/src/promptwatch.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.4.4/src/promptwatch.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       33 2024-02-12 07:42:05.000000 promptwatch-0.4.4/src/promptwatch.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2024-02-12 07:42:05.000000 promptwatch-0.4.4/src/promptwatch.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-05-06 22:22:02.049422 promptwatch-0.4.5/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2024-05-06 22:22:02.049281 promptwatch-0.4.5/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3584 2023-05-19 10:25:10.000000 promptwatch-0.4.5/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.4.5/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2024-05-06 22:22:02.049465 promptwatch-0.4.5/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1198 2023-05-24 21:47:14.000000 promptwatch-0.4.5/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-05-06 22:22:02.042999 promptwatch-0.4.5/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-05-06 22:22:02.045330 promptwatch-0.4.5/src/promptwatch/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      426 2024-05-06 22:21:51.000000 promptwatch-0.4.5/src/promptwatch/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    16570 2023-12-18 22:16:50.000000 promptwatch-0.4.5/src/promptwatch/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     6214 2023-09-08 19:28:50.000000 promptwatch-0.4.5/src/promptwatch/client.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      260 2023-05-19 10:25:10.000000 promptwatch-0.4.5/src/promptwatch/constants.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     5701 2023-09-08 19:29:25.000000 promptwatch-0.4.5/src/promptwatch/data_model.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1555 2023-05-23 20:20:02.000000 promptwatch-0.4.5/src/promptwatch/decorators.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-05-06 22:22:02.047490 promptwatch-0.4.5/src/promptwatch/langchain/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      219 2023-05-30 19:26:54.000000 promptwatch-0.4.5/src/promptwatch/langchain/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13208 2023-12-21 12:55:25.000000 promptwatch-0.4.5/src/promptwatch/langchain/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    33905 2024-05-06 22:11:06.000000 promptwatch-0.4.5/src/promptwatch/langchain/langchain_support.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4277 2024-02-11 22:51:29.000000 promptwatch-0.4.5/src/promptwatch/langchain/unit_tests.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    21913 2024-03-17 18:33:11.000000 promptwatch-0.4.5/src/promptwatch/promptwatch_context.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-05-06 22:22:02.048709 promptwatch-0.4.5/src/promptwatch/unit_tests/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      162 2023-05-19 10:25:10.000000 promptwatch-0.4.5/src/promptwatch/unit_tests/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13470 2024-02-12 08:46:35.000000 promptwatch-0.4.5/src/promptwatch/unit_tests/evaluation.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3247 2023-09-08 19:30:11.000000 promptwatch-0.4.5/src/promptwatch/unit_tests/schema.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    24610 2023-08-22 19:21:36.000000 promptwatch-0.4.5/src/promptwatch/unit_tests/unit_tests.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2497 2024-05-03 14:03:26.000000 promptwatch-0.4.5/src/promptwatch/utils.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-05-06 22:22:02.046362 promptwatch-0.4.5/src/promptwatch.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2024-05-06 22:22:02.000000 promptwatch-0.4.5/src/promptwatch.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      819 2024-05-06 22:22:02.000000 promptwatch-0.4.5/src/promptwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2024-05-06 22:22:02.000000 promptwatch-0.4.5/src/promptwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.4.5/src/promptwatch.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       33 2024-05-06 22:22:02.000000 promptwatch-0.4.5/src/promptwatch.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2024-05-06 22:22:02.000000 promptwatch-0.4.5/src/promptwatch.egg-info/top_level.txt
```

### Comparing `promptwatch-0.4.4/PKG-INFO` & `promptwatch-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.4.4
+Version: 0.4.5
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.4.4/README.md` & `promptwatch-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `promptwatch-0.4.4/setup.py` & `promptwatch-0.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.4.4/src/promptwatch/caching.py` & `promptwatch-0.4.5/src/promptwatch/caching.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.4.4/src/promptwatch/client.py` & `promptwatch-0.4.5/src/promptwatch/client.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.4.4/src/promptwatch/data_model.py` & `promptwatch-0.4.5/src/promptwatch/data_model.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.4.4/src/promptwatch/decorators.py` & `promptwatch-0.4.5/src/promptwatch/decorators.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.4.4/src/promptwatch/langchain/caching.py` & `promptwatch-0.4.5/src/promptwatch/langchain/caching.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.4.4/src/promptwatch/langchain/langchain_support.py` & `promptwatch-0.4.5/src/promptwatch/langchain/langchain_support.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,53 @@
 """A Tracer implementation that records to LangChain endpoint."""
 from __future__ import annotations
-from ast import Tuple
-from contextvars import ContextVar
+
+import datetime
 import re
-from abc import ABC
 import types
-from typing import Any, Dict, Optional, Union
-import datetime
+from abc import ABC
+from ast import Tuple
+from contextvars import ContextVar
+from typing import Any, Dict, List, Optional, Union
+
 import langchain
-from langchain.prompts.base import BasePromptTemplate
-from langchain.prompts.chat import ChatPromptTemplate, HumanMessagePromptTemplate, AIMessagePromptTemplate, SystemMessagePromptTemplate, MessagesPlaceholder, BaseMessagePromptTemplate
-from langchain.llms.base import LLM
-from langchain.chat_models.base import BaseChatModel
+from langchain.agents import Agent, BaseSingleActionAgent, Tool
+from langchain.callbacks.base import BaseCallbackHandler
 from langchain.chains import LLMChain
+from langchain.chains.base import Chain
+from langchain.chat_models.base import BaseChatModel
 from langchain.embeddings.base import Embeddings
-from langchain.schema import HumanMessage, ChatMessage as LangChainChatMessage, AIMessage, SystemMessage, BaseMessage 
-from langchain.prompts import ChatMessagePromptTemplate as LangChainChatMessagePromptTemplate
-from langchain.callbacks.base import BaseCallbackHandler
-from langchain.agents import Tool, Agent, BaseSingleActionAgent
+from langchain.llms.base import LLM
+from langchain.prompts import \
+    ChatMessagePromptTemplate as LangChainChatMessagePromptTemplate
+from langchain.prompts.base import BasePromptTemplate
+from langchain.prompts.chat import (AIMessagePromptTemplate,
+                                    BaseMessagePromptTemplate,
+                                    ChatPromptTemplate,
+                                    HumanMessagePromptTemplate,
+                                    MessagesPlaceholder,
+                                    SystemMessagePromptTemplate)
+from langchain.schema import AgentAction, AgentFinish, AIMessage, BaseMessage
+from langchain.schema import ChatMessage as LangChainChatMessage
+from langchain.schema import Document, HumanMessage, LLMResult, SystemMessage
 from langchain.tools.base import BaseTool
-from langchain.chains.base import Chain
+from openai import BaseModel
 
-from langchain.schema import AgentAction, AgentFinish, LLMResult,  Document
 from ..client import Client
-from ..data_model import NamedPromptTemplateDescription,PromptTemplateDescription, LlmPrompt, ParallelPrompt, ChainSequence, ChatMessage, Answer, Action, Question, RetrievedDocuments, DocumentSnippet, ChatMessagePromptTemplate
-from ..utils import find_the_caller_in_the_stack, wrap_a_method, copy_dict_serializable_values
-from .caching import CachedLLM, CachedChatLLM
-from ..decorators import FORMATTED_PROMPT_CONTEXT_KEY, TEMPLATE_NAME_CONTEXT_KEY, LLM_CHAIN_CONTEXT_KEY
-
-from typing import List, Dict
-from ..promptwatch_context import PromptWatch, ContextTrackerSingleton
-
+from ..data_model import (Action, Answer, ChainSequence, ChatMessage,
+                          ChatMessagePromptTemplate, DocumentSnippet,
+                          LlmPrompt, NamedPromptTemplateDescription,
+                          ParallelPrompt, PromptTemplateDescription, Question,
+                          RetrievedDocuments)
+from ..decorators import (FORMATTED_PROMPT_CONTEXT_KEY, LLM_CHAIN_CONTEXT_KEY,
+                          TEMPLATE_NAME_CONTEXT_KEY)
+from ..promptwatch_context import ContextTrackerSingleton, PromptWatch
+from ..utils import (copy_dict_serializable_values,
+                     find_the_caller_in_the_stack, wrap_a_method)
+from .caching import CachedChatLLM, CachedLLM
 
 
 class LangChainSupport:
 
     def __init__(self, promptwatch_context:PromptWatch) -> None:
         self.promptwatch_context=promptwatch_context
         self.langchain_callback_handler=None
@@ -113,15 +126,14 @@
                 cache_embeddings=embeddings, token_limit=token_limit, similarity_limit=similarity_limit)
         
     # def enable_global_cache(self, embeddings:Embeddings, token_limit:int, similarity_limit:float=0.97)->PromptWatchLlmCache:
     #     """Enable global cache for all LLMs"""
     #     prompt_cache = PromptWatchLlmCache(None, embeddings, token_limit, similarity_limit)
     #     langchain.llm_cache=prompt_cache
 
-   
 
 class LangChainCallbackHandler(BaseCallbackHandler, ABC):
     """An implementation of the PromptWatch handler that tracks langchain tracing events"""
 
 
     def __init__(self, 
                  
@@ -140,15 +152,17 @@
     def prompt_watch(self) -> PromptWatch:
         """Whether to call verbose callbacks even if verbose is False."""
         
         prompt_watch_context = ContextTrackerSingleton.get_current()
         if not prompt_watch_context:
             raise Exception("PromptWatch context could not be resolved")
         return prompt_watch_context
-
+    @property
+    def is_in_promptwatch_context(self) -> bool:
+        return bool(ContextTrackerSingleton.get_current())
 
     @property
     def always_verbose(self) -> bool:
         """Whether to call verbose callbacks even if verbose is False."""
         return True
     
     
@@ -164,22 +178,25 @@
         serialized: Dict[str, Any],
         messages: List[List[BaseMessage]],
         *,
         run_id,
         parent_run_id = None,
         **kwargs: Any,
     ) -> Any:
+        if not self.is_in_promptwatch_context:
+            return
         self.on_llm_start(serialized, messages, run_id=run_id, parent_run_id=parent_run_id, **kwargs)
     
 
     def on_llm_start(
         self, serialized: Dict[str, Any], prompts: List[str, List[BaseMessage]], **kwargs: Any
     ) -> Any:
         """Run when LLM starts running."""
-
+        if not self.is_in_promptwatch_context:
+            return
         prompt_template = None
         prompt_input_values=None
         llm_info=None
         info_message=None
         formatted_prompt=None
 
         if prompts and prompts[0] and isinstance(prompts[0][0],BaseMessage):
@@ -203,15 +220,19 @@
             # lets try to retrieve registered named template first... it's faster
             
 
             if not prompt_template:
                 # lets create anonymous prompt template description
                 prompt_template = create_prompt_template_description(current_llm_chain.prompt)
 
-            prompt_input_values = self.prompt_watch.current_activity.inputs
+            prompt_input_values = {}
+            for chain in self.prompt_watch.chain_hierarchy:
+                if chain.inputs:
+                    prompt_input_values.update(chain.inputs)
+            
 
             formatted_prompt = self.prompt_watch.get_context(FORMATTED_PROMPT_CONTEXT_KEY)
 
             
             if prompts and prompts[0] and isinstance(prompts[0][0],BaseMessage):
                 
                 prompts=[convert_chat_messages(prompts_set) for prompts_set in prompts]
@@ -279,14 +300,16 @@
     def on_llm_new_token(self, token: str, **kwargs: Any) -> Any:
         """Run on new LLM token. Only available when streaming is enabled."""
         pass
 
     
     def on_llm_end(self, response: LLMResult, **kwargs: Any) -> Any:
         """Run when LLM ends running."""
+        if not self.is_in_promptwatch_context:
+            return
         if len(response.generations)>1:
             prompts =  self.prompt_watch.current_activity.prompts
         else:
             prompts=[self.prompt_watch.current_activity]
         
         
         if not self.prompt_watch.current_activity.metadata:
@@ -315,59 +338,64 @@
         
 
     
     def on_llm_error(
         self, error: Union[Exception, KeyboardInterrupt], **kwargs: Any
     ) -> Any:
         """Run when LLM errors."""
+        if not self.is_in_promptwatch_context:
+            return
         self.prompt_watch._on_error(error, kwargs)
 
     
     def on_chain_start(
         self, serialized: Dict[str, Any], inputs: Dict[str, Any], **kwargs: Any
     ) -> Any:
         """Run when chain starts running."""
-        
+        if not self.is_in_promptwatch_context:
+            return
         chain_name = serialized.get("name") or  serialized.get("id",[None])[-1]
         if "LLM" in chain_name :
             current_llm_chain = find_the_caller_in_the_stack(chain_name)
             self.prompt_watch.add_context(LLM_CHAIN_CONTEXT_KEY,current_llm_chain)
 
         self.try_get_retrieved_documents(inputs)
                   
 
-        question = inputs["question"] if inputs.get("question") and len(inputs)==1 and type(inputs["question"])==str else None
+        question = inputs["question"] if  isinstance(inputs,dict) and inputs.get("question") and len(inputs)==1 and type(inputs["question"])==str else None
         if not question and "chat_history" in inputs:
             #try to get question from inputs
             question = next((v for k,v in inputs.items() if k!="chat_history"),None) if len(inputs)==2 else None
 
         if  question and not self.prompt_watch.chain_hierarchy:
             self.prompt_watch._add_activity(Question(text=question))
         if not self.prompt_watch.current_session.session_name:
             self.prompt_watch.current_session.session_name=question
             if not self.prompt_watch.current_session.start_time:
                 self.prompt_watch.current_session.start_time=datetime.datetime.now(tz=datetime.timezone.utc)
             
         
         
         current_chain=ChainSequence(
-                inputs=serialize_chain_inputs(inputs),
+                inputs=serialize_chain_inputs(inputs) if isinstance(inputs,(dict,BaseModel)) else {} ,
                 metadata={},
                 sequence_type=serialized.get("name") or "others"
             )
                                      
         if kwargs:
             current_chain.metadata["input_kwargs"]=kwargs
         self.prompt_watch._open_activity(current_chain)
         
 
         
 
         
     def try_get_retrieved_documents(self, inputs:dict):
+        if not isinstance(inputs,dict):
+            return
         retrieved_documents = next((val for key,val in inputs.items() if isinstance(val,list) and val and isinstance(val[0], Document)),None)
         if retrieved_documents:
             docs=[]
             for doc in retrieved_documents:
                 metadata = {key:val for key,val in doc.metadata.items() if key!="source"}  if doc.metadata else None
                 source = doc.metadata.get("source") if doc.metadata else None
                 docs.append(DocumentSnippet(
@@ -376,15 +404,16 @@
                     metadata=metadata if metadata else None # to not pass empty objects
                     ))
             self.prompt_watch._add_activity(RetrievedDocuments(documents=docs))
     
     def on_chain_end(self, outputs: Dict[str, Any], **kwargs: Any) -> Any:
         """Run when chain ends running."""
         
-        
+        if not self.is_in_promptwatch_context:
+            return
         self.prompt_watch._remove_context(LLM_CHAIN_CONTEXT_KEY)
         outputs = copy_dict_serializable_values(outputs)
         self.prompt_watch.current_activity.outputs=outputs
         if outputs.get("answer"):
             self.prompt_watch._add_activity(Answer(text=outputs["answer"]),as_root=True)
         if kwargs:
             self.prompt_watch.current_activity.metadata["output_kwargs"]=kwargs
@@ -406,34 +435,40 @@
         self.prompt_watch._on_error(error, kwargs)
 
     
     def on_tool_start(
         self, serialized: Dict[str, Any], input_str: str, **kwargs: Any
     ) -> Any:
         """Run when tool starts running."""
+        if not self.is_in_promptwatch_context:
+            return
         self.prompt_watch._open_activity(
                 Action(tool_type=serialized.get("name") or "undefined", input=input_str, input_data=kwargs)
             )
 
     
     def on_tool_end(self, output: str, **kwargs: Any) -> Any:
         """Run when tool ends running."""
+        if not self.is_in_promptwatch_context:
+            return
         self.prompt_watch.current_activity.output=output
         self.prompt_watch.current_activity.output_data=kwargs
         self.prompt_watch._close_current_activity()
 
 
         
     
 
     
     def on_tool_error(
         self, error: Union[Exception, KeyboardInterrupt], **kwargs: Any
     ) -> Any:
         """Run when tool errors."""
+        if not self.is_in_promptwatch_context:
+            return
         self.prompt_watch._on_error(error, kwargs)
 
     
     def on_text(self, text: str, **kwargs: Any) -> Any:
         """Run on arbitrary text."""
 
     
@@ -443,22 +478,22 @@
         
 
 
 
     
     def on_agent_finish(self, finish: AgentFinish, **kwargs: Any) -> Any:
         """Run on agent end."""
+        
         answer_text = finish[0].get("output")
         answer_activity = Answer(text=answer_text)
         self.prompt_watch._add_activity(answer_activity, as_root=True)
         if finish.return_values:
             answer_activity.metadata["outputs"]:finish.return_values
-        
-        
-    
+
+
 promptwatch_tracing_callback_var: ContextVar[Optional[LangChainCallbackHandler]] = ContextVar(  # noqa: E501
     "promptwatch_tracing_callback", default=None
 )
 try:
     import langchain.schema.callbacks.manager as langchain_callback_manager_module
     if hasattr(langchain_callback_manager_module,"register_configure_hook"):
         langchain_callback_manager_module.register_configure_hook(promptwatch_tracing_callback_var, True)
@@ -516,18 +551,14 @@
         prompt_template.__dict__["__template_name__"]=template_name
         prompt_template.__dict__["__template_version__"]=version
 
         PromptWatch.prompt_template_register_cache[template_name] = converted_template
         return prompt_template
 
 
-
-
-
-
 def find_templates_recursive(root_chain: Union[Chain,Tool, Agent], template_name_prefix:str, print_code=True, _ignore_chains:List[Chain]=[])-> Tuple[str,BasePromptTemplate]:
     """This will find all templates in the chain and its subchains, agents, tools recursively. 
     It return a tuple of (path_to_template, template)
 
     If print_code==True, it will also print the code to register all templates
 
 
@@ -578,16 +609,15 @@
         elif isinstance(field_value, BasePromptTemplate):
             if field_value.__dict__.get("__template_name__") :
                  continue
                  raise ValueError(f"PromptTemplate {field_value} has no name")
             if print_code:
                 print(f"register_prompt_template({template_name_prefix}.{field_key}, '{template_name_prefix}.{field_key}'")
             yield f"{template_name_prefix}.{field_key}", field_value
-        
-            
+
 
 def find_and_register_templates_recursive(root_chain: Chain, template_name_prefix:str, ignore_subpaths=[]):
     paths = []
     ignore=False
     for path, template in find_templates_recursive(root_chain, template_name_prefix, print_code=False):
         for subpath in ignore_subpaths:
             if subpath in path:
@@ -598,22 +628,14 @@
         paths.append(path)
     print(f"Registered {len(paths)} templates: ")
     print("\n".join(paths))
     print("WARNING: This method is not fit for production use as it might slow down the startup time.")
     print("         Please consider using find_and_register_templates_recursive() to generate a code to register all templates instead.")
 
 
-
-
-
-
-
-
-
-
 def convert_chat_messages( msg:Union[BaseMessage, List[BaseMessage]]):
         if isinstance(msg, BaseMessage):
                 metadata=None
                 if msg.additional_kwargs:
                     metadata = msg.additional_kwargs
                 if isinstance(msg,HumanMessage):
                     role="user"
@@ -628,15 +650,15 @@
                     metadata=(metadata or {})
                     metadata["name"]=msg.name
                 return (ChatMessage(role=role,text=msg.content, metadata=metadata))
         elif isinstance(msg, list):
             return [convert_chat_messages(m) for m in msg]
         else:
             raise ValueError("msg must be either BaseMessage or List[BaseMessage]")
-        
+
 def reconstruct_langchain_chat_messages( msg:Union[ChatMessage, List[ChatMessage]]):
         if isinstance(msg, ChatMessage):
                 if msg.role=="user":
                     return HumanMessage( content=msg.text)
                     
                 elif msg.role=="assistant":
                     return AIMessage( content=msg.text)
@@ -646,17 +668,19 @@
                     
                 else:    
                     return (LangChainChatMessage(role=msg.role,content=msg.text))
         elif isinstance(msg, list):
             return [reconstruct_langchain_chat_messages(msg) for msg in msg]
         else:
             raise ValueError("msg must be either ChatMessage or List[ChatMessage]")
-        
-def serialize_chain_inputs(inputs:dict):
+
+def serialize_chain_inputs(inputs:Union[dict, BaseModel]):
     res = {}
+    if isinstance(inputs,BaseModel):
+        return inputs.model_dump() if hasattr(inputs, "model_dump") else inputs.dict()
     for k,v in inputs.items():
         if isinstance(v, BaseMessage):
             res[k]=convert_chat_messages(v)
         elif isinstance(v, dict):
             res[k]=serialize_chain_inputs(v)
         elif isinstance(v, list):
             if v:
@@ -725,8 +749,7 @@
         if  hasattr(langchain_prompt_template,"template_format"):
             format=langchain_prompt_template.template_format
     if prompt_template:
         if template_name:
             return NamedPromptTemplateDescription(prompt_template=prompt_template, prompt_input_params=input_params, format=format, template_name=template_name ,template_version=template_version)
         else:
             return PromptTemplateDescription(prompt_template=prompt_template, prompt_input_params=input_params, format=format)
-
```

### Comparing `promptwatch-0.4.4/src/promptwatch/langchain/unit_tests.py` & `promptwatch-0.4.5/src/promptwatch/langchain/unit_tests.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.4.4/src/promptwatch/promptwatch_context.py` & `promptwatch-0.4.5/src/promptwatch/promptwatch_context.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,153 +1,187 @@
 """A Tracer implementation that records to LangChain endpoint."""
+
 from __future__ import annotations
+
+import asyncio
 import base64
-import threading
-from typing import Any, Dict, Optional,List, Union, Tuple, Callable,Any
+import contextvars
 import datetime
+import logging
 import os
 import re
-from .data_model import (ActivityBase, Log, Session)
-import logging
-from .data_model import Session, ActivityBase,  ChainSequence, Log, Answer, Action, Question, RetrievedDocuments, DocumentSnippet
-from uuid import uuid4
+import threading
 import types
-from .utils import wrap_a_method, classproperty
+from abc import ABCMeta
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+from uuid import uuid4
+
 from .caching import PromptWatchCacheManager
 from .constants import EnvVariables
-from abc import ABCMeta
-import contextvars
-import asyncio
+from .data_model import (
+    Action,
+    ActivityBase,
+    Answer,
+    ChainSequence,
+    DocumentSnippet,
+    Log,
+    Question,
+    RetrievedDocuments,
+    Session,
+)
+from .utils import classproperty, wrap_a_method
 
 session_context = contextvars.ContextVar("promptwatch_context")
 
-class ContextTrackerSingleton(ABCMeta,type):
+
+class ContextTrackerSingleton(ABCMeta, type):
     """
     Singleton metaclass for ensuring only one instance of a class per thread
     """
 
-    
-    _cross_thread_storage = {}
+    _cross_thread_storage = threading.local()
 
-    def __call__(cls, *args, **kwargs)->PromptWatch:
+    def __call__(cls, *args, **kwargs) -> PromptWatch:
         """Call method for the singleton metaclass."""
-        
-        prompt_watch_context =  ContextTrackerSingleton.get_current()
+
+        prompt_watch_context = ContextTrackerSingleton.get_current()
         if not prompt_watch_context:
-            prompt_watch_context = super(ContextTrackerSingleton, cls).__call__(*args, **kwargs)
+            prompt_watch_context = super(ContextTrackerSingleton, cls).__call__(
+                *args, **kwargs
+            )
             ContextTrackerSingleton.init_session(prompt_watch_context)
         return prompt_watch_context
-    
+
     def init_session(prompt_watch_context):
         prompt_watch_context_existing = session_context.get(None)
 
-        ContextTrackerSingleton._cross_thread_storage["current"]=prompt_watch_context
-        
-        if  prompt_watch_context_existing:
-            if prompt_watch_context_existing.session_id!=prompt_watch_context.session_id:
-                raise Exception("Current promptwatch context has different session_id ... previous session has not been property finished. Please report this as a bug.")
+        ContextTrackerSingleton._cross_thread_storage.current = prompt_watch_context
+
+        if prompt_watch_context_existing:
+            if (
+                prompt_watch_context_existing.session_id
+                != prompt_watch_context.session_id
+            ):
+                raise Exception(
+                    "Current promptwatch context has different session_id ... previous session has not been property finished. Please report this as a bug."
+                )
 
         else:
             if not prompt_watch_context.session_id:
-                raise Exception("PromptWatch: Session ID was not initialized. Please report this as a bug.")
-            
+                raise Exception(
+                    "PromptWatch: Session ID was not initialized. Please report this as a bug."
+                )
+
             session_context.set(prompt_watch_context)
-        
-   
 
-    def get_current()->PromptWatch:
-        """ return the current instance
+    def get_current() -> PromptWatch:
+        """return the current instance
         for sync context session_id is not required
         for async context session_id is required, otherwise it the instance wont be found
         """
-        prompt_watch_context =  session_context.get(None)
-        if not prompt_watch_context:
-            return ContextTrackerSingleton._cross_thread_storage.get("current")
+        prompt_watch_context = session_context.get(None)
+        if not prompt_watch_context and hasattr(
+            ContextTrackerSingleton._cross_thread_storage, "current"
+        ):
+            return ContextTrackerSingleton._cross_thread_storage.current
         else:
             return prompt_watch_context
 
     @classmethod
     def remove_active_instance(cls):
         session_context.set(None)
-        ContextTrackerSingleton._cross_thread_storage.clear()
+        ContextTrackerSingleton._cross_thread_storage.current = None
         # session_id = ContextTrackerSingleton._thread_local._instance.session_id
         # del ContextTrackerSingleton._cross_thread_storage[session_id]
-        # del ContextTrackerSingleton._thread_local._instance 
-
-
+        # del ContextTrackerSingleton._thread_local._instance
 
 
 class PromptWatch(metaclass=ContextTrackerSingleton):
-    
-    prompt_template_register_cache={}
 
-    def __init__(self, session_id: Optional[str] = None, tracking_project: Optional[str] = None, tracking_tenant: Optional[str] = None, api_key: Optional[str] = None):
+    prompt_template_register_cache = {}
+
+    def __init__(
+        self,
+        session_id: Optional[str] = None,
+        tracking_project: Optional[str] = None,
+        tracking_tenant: Optional[str] = None,
+        api_key: Optional[str] = None,
+    ):
         """
         PromptWatch context to track all the activities inside your LLM chain
 
         ## Parameters:
 
         session_id: Optional[str] - ID of previously used session. It can be assigned using uuid4 or uuid5, or you can save the generated session ID (PromptWatch.get_current_session().id) into the app context to retrieve it later.
         tracking_project: Optional[str] - Optional label for the session to pair it with a certain app or project. Use any arbitrary string (no whitespace and less than 256 chars).
         tracking_tenant: Optional[str] - Optional label for the session to pair it with a tenant (customer of yours). Use any arbitrary string (no whitespace and less than 256 chars). It can also be used to track costs attached to the customer.
         api_key: Optional[str] - API key for accessing the PromptWatch API.
 
-        
+
         ### Example of use:
         ```
         with PromptWatch(tracking_tenant="myCustomerTenantId", tracking_project="nameOfThisTrackingProject", api_key="<your api key>"):
-           agent.run(question) 
+           agent.run(question)
         ```
         """
         self.logger = logging.getLogger("PromptWatch")
         self.session_id = session_id
-        self.tracking_project=tracking_project or os.environ.get(EnvVariables.PROMPTWATCH_TRACKING_PROJECT)
-        self.tracking_tenant=tracking_tenant 
-        self._meta={}
-        
+        self.tracking_project = tracking_project or os.environ.get(
+            EnvVariables.PROMPTWATCH_TRACKING_PROJECT
+        )
+        self.tracking_tenant = tracking_tenant
+        self._meta = {}
+
         if not api_key:
-            api_key=os.environ.get(EnvVariables.PROMPTWATCH_API_KEY)
+            api_key = os.environ.get(EnvVariables.PROMPTWATCH_API_KEY)
         if not api_key:
-            raise Exception("Unable to find PromptWatch API key. Either set api key as a parameter to PromptWatch(api_key='<your api key>') or set it up as an env. variable PROMPTWATCH_API_KEY. You can generate your API key here: https://app.promptwatch.io/get-api-key")
+            raise Exception(
+                "Unable to find PromptWatch API key. Either set api key as a parameter to PromptWatch(api_key='<your api key>') or set it up as an env. variable PROMPTWATCH_API_KEY. You can generate your API key here: https://app.promptwatch.io/get-api-key"
+            )
         else:
-            tenant_id  = self._decode_tenant_from_api_key(api_key)
+            tenant_id = self._decode_tenant_from_api_key(api_key)
             if tenant_id.startswith("temp_"):
                 if session_id:
-                    self.logger.warn("Setting up session_id with a temporary PromptWatch API Key is not allowed. You session_id will be ignored")
+                    self.logger.warn(
+                        "Setting up session_id with a temporary PromptWatch API Key is not allowed. You session_id will be ignored"
+                    )
                 self.session_id = tenant_id[5:]
-                GREEN = '\033[32m'
-                RESET = '\033[0m'
-                print(f"{GREEN}You are using a temporary API key. Do not use in production.")
-                print(f"Visit the the detail of this session at https://www.promptwatch.io/sessions?temp-api-key={api_key} {RESET}")
-                
+                GREEN = "\033[32m"
+                RESET = "\033[0m"
+                print(
+                    f"{GREEN}You are using a temporary API key. Do not use in production."
+                )
+                print(
+                    f"Visit the the detail of this session at https://www.promptwatch.io/sessions?temp-api-key={api_key} {RESET}"
+                )
 
         from .client import Client
+
         self.client = Client(api_key=api_key)
-        
+
         # assign session_id if not provided
         # we will used to track the session across multiple threads
         if not self.session_id:
             self.session_id = str(uuid4())
-        
-        #self.chain_hierarchy_context = contextvars.ContextVar("chain_hierarchy")
-        #self.context_storage=contextvars.ContextVar("context_storage")
-        self.context={}
-        self.chain_hierarchy=[]
-
-        self.pending_session_save=True
-        self.pending_stack:List[ActivityBase]=[]
-        
-        self.current_session=None
+
+        # self.chain_hierarchy_context = contextvars.ContextVar("chain_hierarchy")
+        # self.context_storage=contextvars.ContextVar("context_storage")
+        self.context = {}
+        self.chain_hierarchy = []
+
+        self.pending_session_save = True
+        self.pending_stack: List[ActivityBase] = []
+
+        self.current_session = None
         self._cache_manager = PromptWatchCacheManager(self)
-        self.tracing_handlers={}
-        self.session_entered=False
+        self.tracing_handlers = {}
+        self.session_entered = False
 
-        #event handlers that lasts only
-        self.on_activity_event_handlers=[]
-        
+        # event handlers that lasts only
+        self.on_activity_event_handlers = []
 
     # @property
     # def context(self)->dict:
     #     current_context= self.context_storage.get(None)
     #     if not current_context:
     #         current_context={}
     #         self.context_storage.set(current_context)
@@ -160,153 +194,170 @@
     #         current_chain_hierarchy=[]
     #         self.chain_hierarchy_context.set(current_chain_hierarchy)
     #     return current_chain_hierarchy
 
     @property
     def caching(self):
         return self._cache_manager
-    
+
     @property
     def caching(self):
         return self._cache_manager
 
     @property
     def langchain(self):
-        if not hasattr(self,"_langchain"):
+        if not hasattr(self, "_langchain"):
             from .langchain.langchain_support import LangChainSupport
+
             self._langchain = LangChainSupport(self)
-            
-        
-        return self._langchain
-    
 
+        return self._langchain
 
     def __enter__(self):
         _ = self.chain_hierarchy
         if not self.tracing_handlers:
             # lets enable tracing by default
             self.langchain.init_tracing()
-            #raise Exception("PromptWatch: LangChain callback handler is not set. Please call langchain_tracing() before entering the context.")
+            # raise Exception("PromptWatch: LangChain callback handler is not set. Please call langchain_tracing() before entering the context.")
 
         if not self.current_session:
-            
+
             self.start_session()
-        
-        
-        
 
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         try:
             self.finish_session()
         except Exception as ex:
             self.logger.warn(f"Failed to persist the session: {ex}")
         # we will clear the handlers because we don't want to keep them in memory since PromptWatch is a singleton and lives for the whole app lifecycle
         ContextTrackerSingleton.remove_active_instance()
         self.on_activity_event_handlers.clear()
 
-    
-    def add_on_activity_callback(self, event_handler: Callable[[ActivityBase],Any]):
+    def add_on_activity_callback(self, event_handler: Callable[[ActivityBase], Any]):
         if event_handler not in self.on_activity_event_handlers:
             self.on_activity_event_handlers.append(event_handler)
 
-    def set_session_name(self, name:str):
+    def set_session_name(self, name: str):
         if self.current_session:
-            self.current_session.session_name=name
+            self.current_session.session_name = name
         else:
-            raise Exception("No active session. Please call this method inside PromptWatch context")
+            raise Exception(
+                "No active session. Please call this method inside PromptWatch context"
+            )
 
     @classmethod
     def get_current_session(cls) -> Session:
         """_summary_
 
         Raises:
             Exception: If called outside PromptWatch context
 
         Returns:
             Session: _description_
         """
         instance = cls.get_active_instance()
         if not instance:
-            raise Exception("No session is active. Run this method only inside with PromptWatch context block")
+            raise Exception(
+                "No session is active. Run this method only inside with PromptWatch context block"
+            )
         return instance.current_session
-    
+
     @classmethod
     def get_active_instance(cls) -> Optional[PromptWatch]:
         """
         Returns active instance of PromptWatch if run inside PromptWatch context
         """
         return ContextTrackerSingleton.get_current()
-    
+
     @classmethod
-    def log_user_question(cls, question_text:str, metadata:dict=None ):
+    def log_user_question(cls, question_text: str, metadata: dict = None):
         """_summary_
 
         Log user request message
 
         Args:
             question_text (str): _description_
         """
         question = Question(text=question_text, metadata=metadata)
         instance = PromptWatch.get_active_instance()
         if not instance:
             logging.warn(
-                "PromptWatch: Invalid operation - you must enter an session before logging")
+                "PromptWatch: Invalid operation - you must enter an session before logging"
+            )
             return
-            
-        if instance._meta.get("last_question") and instance._meta.get("last_question").text==question_text:
+
+        if (
+            instance._meta.get("last_question")
+            and instance._meta.get("last_question").text == question_text
+        ):
             # prevent duplicates, if the last answer is the same, take its id to force upsert
-            question.id=instance._meta.get("last_question").id
-        instance._meta["last_question"]=question
+            question.id = instance._meta.get("last_question").id
+        instance._meta["last_question"] = question
         instance._add_activity(question, as_root=True)
         return question
 
     @classmethod
-    def log_assistant_answer(cls, 
-                            answer_text:str, 
-                            feedback_label:Optional[int]=None,
-                            feedback_rating:Optional[int]=None,
-                            feedback_notes:Optional[str]=None,
-                            metadata:dict=None,
-    )->Answer:
+    def log_assistant_answer(
+        cls,
+        answer_text: str,
+        feedback_label: Optional[int] = None,
+        feedback_rating: Optional[int] = None,
+        feedback_notes: Optional[str] = None,
+        metadata: dict = None,
+    ) -> Answer:
         """_summary_
 
         Log assistant response
 
         Args:
             answer_text (str): _description_
         """
-        answer = Answer(text=answer_text, 
-                        feedback_label=feedback_label,
-                        feedback_rating=feedback_rating,
-                        feedback_notes=feedback_notes,
-                        metadata=metadata)
+        answer = Answer(
+            text=answer_text,
+            feedback_label=feedback_label,
+            feedback_rating=feedback_rating,
+            feedback_notes=feedback_notes,
+            metadata=metadata,
+        )
         instance = PromptWatch.get_active_instance()
         if not instance:
             logging.warn(
-                "PromptWatch: Invalid operation - you must enter an session before logging")
-        if instance._meta.get("last_answer") and  instance._meta.get("last_answer").text==answer_text:
+                "PromptWatch: Invalid operation - you must enter an session before logging"
+            )
+        if (
+            instance._meta.get("last_answer")
+            and instance._meta.get("last_answer").text == answer_text
+        ):
             # prevent duplicates, if the last answer is the same, take its id to force upsert
-            answer.id=instance._meta.get("last_answer").id
+            answer.id = instance._meta.get("last_answer").id
         instance._add_activity(answer, as_root=True)
-        instance._meta["last_answer"]=answer
+        instance._meta["last_answer"] = answer
         return answer
 
     @classmethod
-    def log(cls, text: str, error_msg:Optional[str]=None, metadata: Optional[Dict[str, Any]] = None):
+    def log(
+        cls,
+        text: str,
+        error_msg: Optional[str] = None,
+        metadata: Optional[Dict[str, Any]] = None,
+    ):
         """_summary_
 
         Log arbitrary text message
         """
 
-        cls.log_activity(Log(text=text, 
-                                error=error_msg,
-                                metadata=metadata, 
-                                ))
+        cls.log_activity(
+            Log(
+                text=text,
+                error=error_msg,
+                metadata=metadata,
+            )
+        )
 
     @classmethod
     def log_activity(cls, activity: ActivityBase):
         """
         Log any activity
 
         ## Example:
@@ -316,38 +367,38 @@
         with PromptWatch():
             PromptWatch.log_activity(Question(text="Who am I?"))
         ```
         """
         instance = PromptWatch.get_active_instance()
         if not instance:
             logging.warn(
-                "PromptWatch: Invalid operation - you must enter an session before logging")
+                "PromptWatch: Invalid operation - you must enter an session before logging"
+            )
             return
-        instance._add_activity(activity )
-
+        instance._add_activity(activity)
 
     @property
     def current_activity(self) -> ActivityBase:
         if self.chain_hierarchy:
             return self.chain_hierarchy[-1]
-        
-
 
-    def register_prompt_template(self,template_name:str,prompt_template, version:Optional[str]=None):
+    def register_prompt_template(
+        self, template_name: str, prompt_template, version: Optional[str] = None
+    ):
         """
         Register prompt template into context for more detailed tracking, versioning and evaluation
 
 
         Args:
             template_name (str): arbitrary unique template name (should not contain white spaces, max 126 chars)
             prompt_template (Union[BasePromptTemplate,BaseChatPromptTemplate]): Any langchain prompt template
             version (Optional[str], optional): Optional - (major) (SemVer) version of the template. Minor changes are tracked incrementally automatically. Useful if you are going to make a major change in the template, and you with to dive the version a distinct version number.
 
         ## Examples:
-        
+
         ### Registering regular prompt (completion)
 
         ```
         from promptwatch import PromptWatch
         from langchain import OpenAI, LLMChain, PromptTemplate
 
         prompt_template = PromptTemplate.from_template("Finish this sentence {input}")
@@ -358,176 +409,190 @@
             my_chain("The quick brown fox jumped over")
         ```
 
         ### Registering chat messages template (completion)
         ...
 
         """
-        
+
         from .langchain.langchain_support import register_prompt_template
-        register_prompt_template(template_name,prompt_template, version=version)
-        
 
+        register_prompt_template(template_name, prompt_template, version=version)
+
+    def add_context(self, key: str, value: Any):
+        self.context[key] = (self.current_activity, value)
 
-    def add_context(self, key:str, value:Any):
-        self.context[key]=(self.current_activity ,value)
-    
-    def get_context(self, key:str) -> Any:
+    def get_context(self, key: str) -> Any:
         if key in self.context:
-            (_, value) =  self.context[key]
+            (_, value) = self.context[key]
             return value
-    
+
     def _end_context_scope(self):
         keys_to_delete = []
         for key, val in self.context.items():
             activity, _ = val
             if activity == self.current_activity:
                 keys_to_delete.append(key)
 
         for key in keys_to_delete:
             del self.context[key]
 
-    def _remove_context(self, key:str):
-        """ Remove context at the end of current chain"""
+    def _remove_context(self, key: str):
+        """Remove context at the end of current chain"""
         if key in self.context:
             del self.context[key]
 
+    def _open_activity(self, activity: ActivityBase):
 
-        
-
-        
-
-    def _open_activity(self, activity:ActivityBase):
-
-        if not self.current_session.session_name and isinstance(activity,ChainSequence) and activity.inputs:
+        if (
+            not self.current_session.session_name
+            and isinstance(activity, ChainSequence)
+            and activity.inputs
+        ):
             # if current session doesn't have a name, use first non empty input of first chain
-            self.current_session.session_name = next((v for k,v in activity.inputs.items() if v and isinstance(v,str)), None)
+            self.current_session.session_name = next(
+                (v for k, v in activity.inputs.items() if v and isinstance(v, str)),
+                None,
+            )
 
         if not self.current_session.start_time:
             self.start_session()
-        self.current_session.steps_count+=1
-        activity.order=self.current_session.steps_count
+        self.current_session.steps_count += 1
+        activity.order = self.current_session.steps_count
 
         if self.current_activity:
-            if isinstance(self.current_activity,ChainSequence) or isinstance(self.current_activity,Action):
-                activity.parent_activity_id=self.current_activity.id
+            if isinstance(self.current_activity, ChainSequence) or isinstance(
+                self.current_activity, Action
+            ):
+                activity.parent_activity_id = self.current_activity.id
             else:
-                activity.parent_activity_id=self.current_activity.parent_activity_id
-        
+                activity.parent_activity_id = self.current_activity.parent_activity_id
+
         self.pending_stack.append(activity)
         self.chain_hierarchy.append(activity)
         return
-        
-    
 
-    def _add_activity(self, activity:ActivityBase, as_root:bool=False):
+    def _add_activity(self, activity: ActivityBase, as_root: bool = False):
 
-        if not self.current_session.session_name and isinstance(activity,Question) and activity.text:
+        if (
+            not self.current_session.session_name
+            and isinstance(activity, Question)
+            and activity.text
+        ):
             # if current session doesn't have a name, use first non empty input of first chain
             self.current_session.session_name = activity.text
 
         if not self.current_session.start_time:
             self.start_session()
-        
-        self.current_session.steps_count+=1
-        activity.order=self.current_session.steps_count
 
-        activity.end_time=datetime.datetime.now(tz=datetime.timezone.utc)
+        self.current_session.steps_count += 1
+        activity.order = self.current_session.steps_count
+
+        activity.end_time = datetime.datetime.now(tz=datetime.timezone.utc)
         if self.current_activity and not as_root:
-            if isinstance(self.current_activity,ChainSequence):
-                activity.parent_activity_id=self.current_activity.id
+            if isinstance(self.current_activity, ChainSequence):
+                activity.parent_activity_id = self.current_activity.id
             else:
-                activity.parent_activity_id=self.current_activity.parent_activity_id
+                activity.parent_activity_id = self.current_activity.parent_activity_id
 
         for handler in self.on_activity_event_handlers:
             try:
                 handler(activity)
             except Exception as ex:
-                self.logger.exception(f"Failed to execute on_activity_event_handlers handler {handler.__name__}: {ex}")
+                self.logger.exception(
+                    f"Failed to execute on_activity_event_handlers handler {handler.__name__}: {ex}"
+                )
 
         self.pending_stack.append(activity)
         if activity.parent_activity_id is None:
             self._flush_stack()
-        
-        
-        
-    
+
     def _close_current_activity(self):
         self._end_context_scope()
-        self.current_activity.end_time=datetime.datetime.now(tz=datetime.timezone.utc)
-        if self.chain_hierarchy and self.current_activity==self.current_activity:
+        self.current_activity.end_time = datetime.datetime.now(tz=datetime.timezone.utc)
+        if self.chain_hierarchy and self.current_activity == self.current_activity:
             closing_chain = self.chain_hierarchy.pop()
             closing_chain.end_time = datetime.datetime.now(tz=datetime.timezone.utc)
             if closing_chain not in self.pending_stack:
                 self.pending_stack.append(closing_chain)
-                
+
         for handler in self.on_activity_event_handlers:
             try:
                 handler(closing_chain)
             except Exception as ex:
-                self.logger.exception(f"Failed to execute on_activity_event_handlers handler {handler.__name__}: {ex}")
+                self.logger.exception(
+                    f"Failed to execute on_activity_event_handlers handler {handler.__name__}: {ex}"
+                )
         self._flush_stack()
 
     def _flush_stack(self):
-        if  self.pending_session_save and self.current_session.steps_count:
+        if self.pending_session_save and self.current_session.steps_count:
             try:
                 self.client.start_session(self.current_session)
-                self.pending_session_save=False
+                self.pending_session_save = False
             except Exception as ex:
                 self.logger.warn(f"Failed to persist the session: {ex}")
-            
-        if self.pending_stack and  not self.pending_session_save:
+
+        if self.pending_stack and not self.pending_session_save:
             try:
                 self.client.save_activities(self.current_session.id, self.pending_stack)
                 for activity in self.pending_stack:
                     if activity.end_time:
                         self.pending_stack.remove(activity)
             except Exception as ex:
                 self.logger.warn(f"Failed to persist activities to PromptWatch: {ex}")
 
-
-    def start_session(self, session_id:Optional[str]=None):
-        self._meta={}
+    def start_session(self, session_id: Optional[str] = None):
+        self._meta = {}
         self.session_id = session_id or self.session_id or str(uuid4())
         if self.current_session:
-            raise Exception("Session already started. Do not open PromptWatch context twice (probably nested with PromptWatch: ... calls)")
-        self.current_session=Session(id=self.session_id, start_time=datetime.datetime.now(tz=datetime.timezone.utc), tracking_project=self.tracking_project, tracking_tenant=self.tracking_tenant)
+            raise Exception(
+                "Session already started. Do not open PromptWatch context twice (probably nested with PromptWatch: ... calls)"
+            )
+        self.current_session = Session(
+            id=self.session_id,
+            start_time=datetime.datetime.now(tz=datetime.timezone.utc),
+            tracking_project=self.tracking_project,
+            tracking_tenant=self.tracking_tenant,
+        )
         self.logger.info(f"Starting PromptWatch session: {self.current_session.id}")
-        self.current_session.start_time=self.current_session.start_time or datetime.datetime.now(tz=datetime.timezone.utc)
-        self.pending_session_save=True
-        
+        self.current_session.start_time = (
+            self.current_session.start_time
+            or datetime.datetime.now(tz=datetime.timezone.utc)
+        )
+        self.pending_session_save = True
+
     def start_new_session(self):
         if self.current_session:
             self.finish_session()
         session_id = str(uuid4())
         self.start_session(session_id)
-  
 
     def finish_session(self):
         if self.current_session:
-            self.current_session.end_time=datetime.datetime.now(tz=datetime.timezone.utc)
+            self.current_session.end_time = datetime.datetime.now(
+                tz=datetime.timezone.utc
+            )
             self._flush_stack()
             if self.current_session.steps_count:
                 self.client.finish_session(self.current_session)
-            
-            self.current_session=None
+
+            self.current_session = None
 
     def _on_error(self, error, kwargs):
         if self.current_activity:
-            self.current_activity.error=str(error)
+            self.current_activity.error = str(error)
         if self.current_activity and kwargs:
             if not self.current_activity.metadata:
-                self.current_activity.metadata={}
-            self.current_activity.metadata["error_kwargs"]=kwargs
-        self.current_session.is_error=True
+                self.current_activity.metadata = {}
+            self.current_activity.metadata["error_kwargs"] = kwargs
+        self.current_session.is_error = True
         self._close_current_activity()
 
-    def _decode_tenant_from_api_key(self, api_key)->str:
+    def _decode_tenant_from_api_key(self, api_key) -> str:
         # Decrypt the encrypted API key value
         try:
-            decoded_api_key =base64.b64decode( api_key).decode("utf-8")
+            decoded_api_key = base64.b64decode(api_key).decode("utf-8")
             # Convert the decrypted bytes to string
             return decoded_api_key.split(":")[0]
         except:
             raise Exception("This doesn't seems to be a valid PromptWatch API Key")
-        
-
```

### Comparing `promptwatch-0.4.4/src/promptwatch/unit_tests/evaluation.py` & `promptwatch-0.4.5/src/promptwatch/unit_tests/evaluation.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
             
         ```
         
         """
         if self.iterations==0:
             # sanity checks
             try:
-                from langchain.chains import LLMChain
+                from langchain import LLMChain
                 if self.unit_test_session.unit_test_run.conditions and self.unit_test_session.unit_test_run.conditions.for_template_name:
                     # if we are running test for template, we expect to evaluate llm_chain.run method, not the instance itself
                     if isinstance(result_generator, LLMChain):
                         result_generator=result_generator.run
                     
             except ImportError as e:
                 # we ignore error if langchain cant be imported
```

### Comparing `promptwatch-0.4.4/src/promptwatch/unit_tests/schema.py` & `promptwatch-0.4.5/src/promptwatch/unit_tests/schema.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.4.4/src/promptwatch/unit_tests/unit_tests.py` & `promptwatch-0.4.5/src/promptwatch/unit_tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.4.4/src/promptwatch/utils.py` & `promptwatch-0.4.5/src/promptwatch/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import datetime
 from decimal import Decimal
 import inspect
 import types
+
+from pydantic import BaseModel
 def find_the_caller_in_the_stack(name:str=None, type:type = None):
         caller_frame = inspect.currentframe().f_back
         while caller_frame:
             caller_locals = caller_frame.f_locals
             caller_instance = caller_locals.get("self", None)
 
             if (name and name==caller_instance.__class__.__name__) or (type and isinstance(caller_instance, type)):
@@ -26,16 +28,18 @@
             elif isinstance(value, dict):
                 res[key] = copy_dict_serializable_values(value)
             elif isinstance(value, list):
                 res[key] = copy_list_serializable_values(value)
             elif isinstance(value, datetime.datetime):
                 res[key] = value.isoformat()
         return res
+    if isinstance(dict_value, BaseModel):
+        return dict_value.model_dump() if hasattr(dict_value, "model_dump") else dict_value.dict()
     else:
-        raise ValueError(f"Expected dict. Got: {dict_value}")
+        return {}
 
 def copy_list_serializable_values(list_value):
     if isinstance(list_value, list):
         value=[]
         for i, item in enumerate(list_value):
             if is_primitive_type(item):
                 value[i] = item
```

### Comparing `promptwatch-0.4.4/src/promptwatch.egg-info/PKG-INFO` & `promptwatch-0.4.5/src/promptwatch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.4.4
+Version: 0.4.5
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.4.4/src/promptwatch.egg-info/SOURCES.txt` & `promptwatch-0.4.5/src/promptwatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

