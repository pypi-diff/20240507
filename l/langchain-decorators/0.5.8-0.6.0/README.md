# Comparing `tmp/langchain_decorators-0.5.8.tar.gz` & `tmp/langchain_decorators-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_decorators-0.5.8.tar", last modified: Thu Apr 18 12:02:23 2024, max compression
+gzip compressed data, was "langchain_decorators-0.6.0.tar", last modified: Mon May  6 22:30:56 2024, max compression
```

## Comparing `langchain_decorators-0.5.8.tar` & `langchain_decorators-0.6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-04-18 12:02:23.039862 langchain_decorators-0.5.8/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1066 2023-06-09 22:30:45.000000 langchain_decorators-0.5.8/LICENSE
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    23383 2024-04-18 12:02:23.039329 langchain_decorators-0.5.8/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    22976 2024-04-14 18:30:54.000000 langchain_decorators-0.5.8/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 langchain_decorators-0.5.8/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2024-04-18 12:02:23.041146 langchain_decorators-0.5.8/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1117 2023-06-11 12:35:54.000000 langchain_decorators-0.5.8/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-04-18 12:02:23.020949 langchain_decorators-0.5.8/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-04-18 12:02:23.034071 langchain_decorators-0.5.8/src/langchain_decorators/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      432 2024-04-18 12:02:00.000000 langchain_decorators-0.5.8/src/langchain_decorators/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    40823 2024-04-18 12:01:06.000000 langchain_decorators-0.5.8/src/langchain_decorators/chains.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    20495 2023-12-18 09:15:59.000000 langchain_decorators-0.5.8/src/langchain_decorators/common.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    21281 2024-04-14 15:47:14.000000 langchain_decorators-0.5.8/src/langchain_decorators/function_decorator.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    24793 2024-04-02 10:37:57.000000 langchain_decorators-0.5.8/src/langchain_decorators/output_parsers.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    24077 2024-04-18 08:01:29.000000 langchain_decorators-0.5.8/src/langchain_decorators/prompt_decorator.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    19606 2024-02-12 07:38:17.000000 langchain_decorators-0.5.8/src/langchain_decorators/prompt_template.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4544 2023-09-13 06:19:53.000000 langchain_decorators-0.5.8/src/langchain_decorators/pydantic_helpers.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4824 2024-04-16 20:33:14.000000 langchain_decorators-0.5.8/src/langchain_decorators/schema.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1844 2023-06-18 11:01:20.000000 langchain_decorators-0.5.8/src/langchain_decorators/streaming_context.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-04-18 12:02:23.038429 langchain_decorators-0.5.8/src/langchain_decorators.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    23383 2024-04-18 12:02:23.000000 langchain_decorators-0.5.8/src/langchain_decorators.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      739 2024-04-18 12:02:23.000000 langchain_decorators-0.5.8/src/langchain_decorators.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2024-04-18 12:02:23.000000 langchain_decorators-0.5.8/src/langchain_decorators.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-08 20:09:02.000000 langchain_decorators-0.5.8/src/langchain_decorators.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       22 2024-04-18 12:02:23.000000 langchain_decorators-0.5.8/src/langchain_decorators.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       21 2024-04-18 12:02:23.000000 langchain_decorators-0.5.8/src/langchain_decorators.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-05-06 22:30:56.949514 langchain_decorators-0.6.0/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1066 2023-06-09 22:30:45.000000 langchain_decorators-0.6.0/LICENSE
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    23383 2024-05-06 22:30:56.949275 langchain_decorators-0.6.0/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    22976 2024-04-14 18:30:54.000000 langchain_decorators-0.6.0/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 langchain_decorators-0.6.0/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2024-05-06 22:30:56.949557 langchain_decorators-0.6.0/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1117 2023-06-11 12:35:54.000000 langchain_decorators-0.6.0/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-05-06 22:30:56.942995 langchain_decorators-0.6.0/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-05-06 22:30:56.947611 langchain_decorators-0.6.0/src/langchain_decorators/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      432 2024-05-06 22:27:58.000000 langchain_decorators-0.6.0/src/langchain_decorators/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    42098 2024-05-05 14:26:27.000000 langchain_decorators-0.6.0/src/langchain_decorators/chains.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    20495 2024-05-01 17:10:31.000000 langchain_decorators-0.6.0/src/langchain_decorators/common.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    21281 2024-04-14 15:47:14.000000 langchain_decorators-0.6.0/src/langchain_decorators/function_decorator.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    24793 2024-04-02 10:37:57.000000 langchain_decorators-0.6.0/src/langchain_decorators/output_parsers.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    24077 2024-05-01 17:10:31.000000 langchain_decorators-0.6.0/src/langchain_decorators/prompt_decorator.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    19606 2024-02-12 07:38:17.000000 langchain_decorators-0.6.0/src/langchain_decorators/prompt_template.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4544 2023-09-13 06:19:53.000000 langchain_decorators-0.6.0/src/langchain_decorators/pydantic_helpers.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4824 2024-04-16 20:33:14.000000 langchain_decorators-0.6.0/src/langchain_decorators/schema.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1844 2023-06-18 11:01:20.000000 langchain_decorators-0.6.0/src/langchain_decorators/streaming_context.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-05-06 22:30:56.948976 langchain_decorators-0.6.0/src/langchain_decorators.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    23383 2024-05-06 22:30:56.000000 langchain_decorators-0.6.0/src/langchain_decorators.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      739 2024-05-06 22:30:56.000000 langchain_decorators-0.6.0/src/langchain_decorators.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2024-05-06 22:30:56.000000 langchain_decorators-0.6.0/src/langchain_decorators.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-08 20:09:02.000000 langchain_decorators-0.6.0/src/langchain_decorators.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       22 2024-05-06 22:30:56.000000 langchain_decorators-0.6.0/src/langchain_decorators.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       21 2024-05-06 22:30:56.000000 langchain_decorators-0.6.0/src/langchain_decorators.egg-info/top_level.txt
```

### Comparing `langchain_decorators-0.5.8/LICENSE` & `langchain_decorators-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_decorators-0.5.8/PKG-INFO` & `langchain_decorators-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-decorators
-Version: 0.5.8
+Version: 0.6.0
 Summary: syntactic sugar for langchain
 Home-page: https://github.com/ju-bezdek/langchain-decorators
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: langchain
 Requires-Python: >=3.9
```

### Comparing `langchain_decorators-0.5.8/README.md` & `langchain_decorators-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `langchain_decorators-0.5.8/setup.py` & `langchain_decorators-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `langchain_decorators-0.5.8/src/langchain_decorators/chains.py` & `langchain_decorators-0.6.0/src/langchain_decorators/chains.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import inspect
 import json
 import logging
-from typing import Any, Callable, Coroutine, Dict, List, Optional, Union
+from typing import Any, Callable, Coroutine, Dict, List, Optional, Union, cast
 
 import pydantic
 from langchain.callbacks.base import BaseCallbackHandler, BaseCallbackManager
 from langchain.callbacks.manager import (
     AsyncCallbackManagerForChainRun,
     CallbackManagerForChainRun,
     Callbacks,
@@ -15,19 +15,21 @@
 from langchain.prompts import PromptTemplate
 from langchain.prompts.base import StringPromptValue
 from langchain.prompts.chat import ChatPromptValue
 from langchain.schema import (
     AIMessage,
     BaseMessage,
     ChatGeneration,
+    Generation,
     HumanMessage,
     LLMResult,
 )
 from langchain.schema.output import LLMResult
 from langchain.tools.base import BaseTool
+from langchain_core.language_models import BaseLanguageModel, LanguageModelInput
 
 from .common import LlmSelector, LogColors, PromptTypes, PromptTypeSettings, print_log
 from .function_decorator import get_function_schema
 from .output_parsers import (
     BaseOutputParser,
     OpenAIFunctionsPydanticOutputParser,
     OutputParserExceptionWithOriginal,
@@ -503,37 +505,39 @@
         self,
         input_list: List[Dict[str, Any]],
         run_manager: Optional[AsyncCallbackManagerForChainRun] = None,
     ) -> LLMResult:
         """Generate LLM result from inputs."""
         prompts, stop = await self.aprep_prompts(input_list, run_manager=run_manager)
         llm = self.select_llm(prompts, input_list[0])
+        callbacks = run_manager.get_child() if run_manager else None
         additional_kwargs = self.llm_kwargs or {}
         if self.__should_use_json_response_format(llm):
             additional_kwargs["response_format"] = {"type": "json_object"}
         if self.llm_kwargs:
-            additional_kwargs["llm_kwargs"] = self.llm_kwargs
-        try:
+            additional_kwargs.update(self.llm_kwargs)
+        if isinstance(llm, BaseLanguageModel):
             return await llm.agenerate_prompt(
                 prompts,
                 stop,
-                callbacks=run_manager.get_child() if run_manager else None,
+                callbacks=callbacks,
                 **additional_kwargs,
             )
-        except RequestRetry as e:
-            if not self._is_retry == True:
-                self._is_retry = True
-                return await llm.agenerate_prompt(
-                    prompts,
-                    stop,
-                    callbacks=run_manager.get_child() if run_manager else None,
-                    **additional_kwargs,
-                )
-            else:
-                raise Exception(e.feedback)
+
+        else:
+            results = await llm.bind(stop=stop, **additional_kwargs).abatch(
+                cast(List, prompts), {"callbacks": callbacks}
+            )
+            generations: List[List[Generation]] = []
+            for res in results:
+                if isinstance(res, BaseMessage):
+                    generations.append([ChatGeneration(message=res)])
+                else:
+                    generations.append([Generation(text=res)])
+            return LLMResult(generations=generations)
 
 
 class LLMDecoratorChainWithFunctionSupport(LLMDecoratorChain):
 
     functions: Union[FunctionsProvider, List[Union[Callable, BaseTool]]]
     func_name_map: dict = None
 
@@ -696,38 +700,59 @@
         input_list: List[Dict[str, Any]],
         run_manager: Optional[AsyncCallbackManagerForChainRun] = None,
     ) -> LLMResult:
         """Generate LLM result from inputs."""
         additional_kwargs, final_function_schemas = self.preprocess_inputs(input_list)
 
         prompts, stop = await self.aprep_prompts(input_list, run_manager=run_manager)
-        chat_model: BaseChatModel = self.select_llm(prompts, input_list[0])
+        llm: BaseChatModel = self.select_llm(prompts, input_list[0])
+        callbacks = run_manager.get_child() if run_manager else None
 
         async def arun(additional_instruction: str = None):
+            # if final_function_schemas:
+            #     messages = [prompt.to_messages() for prompt in prompts]
+            #     if additional_instruction:
+            #         messages[0].append(AIMessage(content=additional_instruction))
+            #     return await llm.agenerate(
+            #         messages=messages,
+            #         stop=stop,
+            #         callbacks=run_manager.get_child() if run_manager else None,
+            #         functions=final_function_schemas,
+            #         **additional_kwargs,
+            #     )
+            # else:
             if final_function_schemas:
-                messages = [prompt.to_messages() for prompt in prompts]
-                if additional_instruction:
-                    messages[0].append(AIMessage(content=additional_instruction))
-                return await chat_model.agenerate(
-                    messages=messages,
-                    stop=stop,
-                    callbacks=run_manager.get_child() if run_manager else None,
-                    functions=final_function_schemas,
-                    **additional_kwargs,
-                )
-            else:
-                return await chat_model.agenerate_prompt(
-                    prompts,
-                    stop,
-                    callbacks=run_manager.get_child() if run_manager else None,
-                )
+                additional_kwargs["functions"] = final_function_schemas
+            if not isinstance(prompts, ChatPromptValue):
+
+                if isinstance(llm, BaseLanguageModel):
+                    return await llm.agenerate_prompt(
+                        prompts,
+                        stop,
+                        callbacks=callbacks,
+                        **additional_kwargs,
+                    )
+
+                else:
+                    results = await llm.bind(stop=stop, **additional_kwargs).abatch(
+                        cast(List, prompts), {"callbacks": callbacks}
+                    )
+                    generations: List[List[Generation]] = []
+                    for res in results:
+                        if isinstance(res, BaseMessage):
+                            generations.append([ChatGeneration(message=res)])
+                        else:
+                            generations.append([Generation(text=res)])
+                    return LLMResult(generations=generations)
 
         try:
             return await arun(additional_instruction=self._additional_instruction)
         except RequestRetry as e:
+            if not isinstance(prompts, ChatPromptValue):
+                raise  # supported only for chat
             if not self._is_retry == True:
                 self._is_retry = True
                 return await arun(self._additional_instruction)
             else:
                 raise Exception(e.feedback)
 
     def _create_output(self, generation):
```

### Comparing `langchain_decorators-0.5.8/src/langchain_decorators/common.py` & `langchain_decorators-0.6.0/src/langchain_decorators/common.py`

 * *Files identical despite different names*

### Comparing `langchain_decorators-0.5.8/src/langchain_decorators/function_decorator.py` & `langchain_decorators-0.6.0/src/langchain_decorators/function_decorator.py`

 * *Files identical despite different names*

### Comparing `langchain_decorators-0.5.8/src/langchain_decorators/output_parsers.py` & `langchain_decorators-0.6.0/src/langchain_decorators/output_parsers.py`

 * *Files identical despite different names*

### Comparing `langchain_decorators-0.5.8/src/langchain_decorators/prompt_decorator.py` & `langchain_decorators-0.6.0/src/langchain_decorators/prompt_decorator.py`

 * *Files identical despite different names*

### Comparing `langchain_decorators-0.5.8/src/langchain_decorators/prompt_template.py` & `langchain_decorators-0.6.0/src/langchain_decorators/prompt_template.py`

 * *Files identical despite different names*

### Comparing `langchain_decorators-0.5.8/src/langchain_decorators/pydantic_helpers.py` & `langchain_decorators-0.6.0/src/langchain_decorators/pydantic_helpers.py`

 * *Files identical despite different names*

### Comparing `langchain_decorators-0.5.8/src/langchain_decorators/schema.py` & `langchain_decorators-0.6.0/src/langchain_decorators/schema.py`

 * *Files identical despite different names*

### Comparing `langchain_decorators-0.5.8/src/langchain_decorators/streaming_context.py` & `langchain_decorators-0.6.0/src/langchain_decorators/streaming_context.py`

 * *Files identical despite different names*

### Comparing `langchain_decorators-0.5.8/src/langchain_decorators.egg-info/PKG-INFO` & `langchain_decorators-0.6.0/src/langchain_decorators.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-decorators
-Version: 0.5.8
+Version: 0.6.0
 Summary: syntactic sugar for langchain
 Home-page: https://github.com/ju-bezdek/langchain-decorators
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: langchain
 Requires-Python: >=3.9
```

### Comparing `langchain_decorators-0.5.8/src/langchain_decorators.egg-info/SOURCES.txt` & `langchain_decorators-0.6.0/src/langchain_decorators.egg-info/SOURCES.txt`

 * *Files identical despite different names*

