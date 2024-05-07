# Comparing `tmp/tool_use-0.2.0.tar.gz` & `tmp/tool_use-0.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tool_use-0.2.0.tar", last modified: Sat Apr 27 01:47:26 2024, max compression
+gzip compressed data, was "tool_use-0.2.1rc1.tar", last modified: Tue May  7 08:24:11 2024, max compression
```

## Comparing `tool_use-0.2.0.tar` & `tool_use-0.2.1rc1.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-27 01:47:26.101899 tool_use-0.2.0/
--rw-r--r--   0 kimjaemin   (501) staff       (20)       30 2024-03-17 15:07:20.000000 tool_use-0.2.0/MANIFEST.in
--rw-r--r--   0 kimjaemin   (501) staff       (20)      106 2024-04-27 01:47:26.101645 tool_use-0.2.0/PKG-INFO
--rw-r--r--   0 kimjaemin   (501) staff       (20)      564 2024-04-22 14:29:43.000000 tool_use-0.2.0/README.md
--rw-r--r--   0 kimjaemin   (501) staff       (20)      553 2024-04-27 01:47:16.000000 tool_use-0.2.0/pyproject.toml
--rw-r--r--   0 kimjaemin   (501) staff       (20)       38 2024-04-27 01:47:26.101957 tool_use-0.2.0/setup.cfg
--rw-r--r--   0 kimjaemin   (501) staff       (20)      527 2024-04-27 01:47:09.000000 tool_use-0.2.0/setup.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-27 01:47:26.099503 tool_use-0.2.0/tests/
--rw-r--r--   0 kimjaemin   (501) staff       (20)        0 2024-02-06 11:51:51.000000 tool_use-0.2.0/tests/__init__.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)     9400 2024-04-26 08:03:24.000000 tool_use-0.2.0/tests/test_anthropic_tool_use.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)     1235 2024-04-22 14:29:43.000000 tool_use-0.2.0/tests/test_exception.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)     1016 2024-04-22 14:29:43.000000 tool_use-0.2.0/tests/test_openai_tool_use.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-27 01:47:26.099700 tool_use-0.2.0/tool_use/
--rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.2.0/tool_use/__init__.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-27 01:47:26.100947 tool_use-0.2.0/tool_use/tools/
--rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.2.0/tool_use/tools/__init__.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)    18131 2024-04-24 02:37:31.000000 tool_use-0.2.0/tool_use/tools/anthropic_tool_use.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)    22455 2024-04-22 14:44:36.000000 tool_use-0.2.0/tool_use/tools/openai_tool_use.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)      537 2024-03-17 15:07:20.000000 tool_use-0.2.0/tool_use/tools/utils.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-27 01:47:26.101209 tool_use-0.2.0/tool_use/yamls/
--rw-r--r--   0 kimjaemin   (501) staff       (20)      909 2024-04-22 14:29:43.000000 tool_use-0.2.0/tool_use/yamls/anthropic_tool_use.yaml
--rw-r--r--   0 kimjaemin   (501) staff       (20)     1512 2024-04-08 11:29:56.000000 tool_use-0.2.0/tool_use/yamls/openai_tool_use.yaml
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-27 01:47:26.101388 tool_use-0.2.0/tool_use.egg-info/
--rw-r--r--   0 kimjaemin   (501) staff       (20)      106 2024-04-27 01:47:26.000000 tool_use-0.2.0/tool_use.egg-info/PKG-INFO
--rw-r--r--   0 kimjaemin   (501) staff       (20)      531 2024-04-27 01:47:26.000000 tool_use-0.2.0/tool_use.egg-info/SOURCES.txt
--rw-r--r--   0 kimjaemin   (501) staff       (20)        1 2024-04-27 01:47:26.000000 tool_use-0.2.0/tool_use.egg-info/dependency_links.txt
--rw-r--r--   0 kimjaemin   (501) staff       (20)      135 2024-04-27 01:47:26.000000 tool_use-0.2.0/tool_use.egg-info/entry_points.txt
--rw-r--r--   0 kimjaemin   (501) staff       (20)       15 2024-04-27 01:47:26.000000 tool_use-0.2.0/tool_use.egg-info/top_level.txt
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-05-07 08:24:11.847451 tool_use-0.2.1rc1/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       30 2024-03-17 15:07:20.000000 tool_use-0.2.1rc1/MANIFEST.in
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      109 2024-05-07 08:24:11.847227 tool_use-0.2.1rc1/PKG-INFO
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      564 2024-04-22 14:29:43.000000 tool_use-0.2.1rc1/README.md
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      556 2024-05-07 08:23:45.000000 tool_use-0.2.1rc1/pyproject.toml
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       38 2024-05-07 08:24:11.847501 tool_use-0.2.1rc1/setup.cfg
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      530 2024-05-07 08:23:34.000000 tool_use-0.2.1rc1/setup.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-05-07 08:24:11.845041 tool_use-0.2.1rc1/tests/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)        0 2024-02-06 11:51:51.000000 tool_use-0.2.1rc1/tests/__init__.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     9400 2024-04-26 08:03:24.000000 tool_use-0.2.1rc1/tests/test_anthropic_tool_use.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     1235 2024-04-22 14:29:43.000000 tool_use-0.2.1rc1/tests/test_exception.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     1878 2024-05-07 08:23:11.000000 tool_use-0.2.1rc1/tests/test_file_system_loader.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     1016 2024-04-22 14:29:43.000000 tool_use-0.2.1rc1/tests/test_openai_tool_use.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-05-07 08:24:11.845173 tool_use-0.2.1rc1/tool_use/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.2.1rc1/tool_use/__init__.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-05-07 08:24:11.846471 tool_use-0.2.1rc1/tool_use/tools/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.2.1rc1/tool_use/tools/__init__.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)    18348 2024-05-07 08:23:11.000000 tool_use-0.2.1rc1/tool_use/tools/anthropic_tool_use.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)    22764 2024-05-07 08:23:11.000000 tool_use-0.2.1rc1/tool_use/tools/openai_tool_use.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      537 2024-03-17 15:07:20.000000 tool_use-0.2.1rc1/tool_use/tools/utils.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-05-07 08:24:11.846764 tool_use-0.2.1rc1/tool_use/yamls/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      982 2024-05-07 08:23:11.000000 tool_use-0.2.1rc1/tool_use/yamls/anthropic_tool_use.yaml
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     1585 2024-05-07 08:23:11.000000 tool_use-0.2.1rc1/tool_use/yamls/openai_tool_use.yaml
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-05-07 08:24:11.846979 tool_use-0.2.1rc1/tool_use.egg-info/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      109 2024-05-07 08:24:11.000000 tool_use-0.2.1rc1/tool_use.egg-info/PKG-INFO
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      564 2024-05-07 08:24:11.000000 tool_use-0.2.1rc1/tool_use.egg-info/SOURCES.txt
+-rw-r--r--   0 kimjaemin   (501) staff       (20)        1 2024-05-07 08:24:11.000000 tool_use-0.2.1rc1/tool_use.egg-info/dependency_links.txt
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      135 2024-05-07 08:24:11.000000 tool_use-0.2.1rc1/tool_use.egg-info/entry_points.txt
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       15 2024-05-07 08:24:11.000000 tool_use-0.2.1rc1/tool_use.egg-info/top_level.txt
```

### Comparing `tool_use-0.2.0/README.md` & `tool_use-0.2.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `tool_use-0.2.0/pyproject.toml` & `tool_use-0.2.1rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tool_use"
-version = "0.2.0"
+version = "0.2.1rc1"
 description = "Promptflow tool package for OpenAI/Anthropic"
 authors = ["ethan <ethan@wrtn.io>", "JaeminBest <mikjm98@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 anthropic = "^0.23.1"
```

### Comparing `tool_use-0.2.0/setup.py` & `tool_use-0.2.1rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 PACKAGE_NAME = "tool_use"
 
 setup(
     name=PACKAGE_NAME,
-    version="0.2.0",
+    version="0.2.1rc1",
     description="Promptflow tool package for OpenAI/Anthropic",
     packages=find_packages(),
     entry_points={
         "package_tools": [
             "openai_tool_use = tool_use.tools.utils:list_package_tools",
             "anthropic_tool_use = tool_use.tools.utils:list_package_tools",
         ],
```

### Comparing `tool_use-0.2.0/tests/test_anthropic_tool_use.py` & `tool_use-0.2.1rc1/tests/test_anthropic_tool_use.py`

 * *Files identical despite different names*

### Comparing `tool_use-0.2.0/tests/test_exception.py` & `tool_use-0.2.1rc1/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `tool_use-0.2.0/tests/test_openai_tool_use.py` & `tool_use-0.2.1rc1/tests/test_openai_tool_use.py`

 * *Files identical despite different names*

### Comparing `tool_use-0.2.0/tool_use/tools/anthropic_tool_use.py` & `tool_use-0.2.1rc1/tool_use/tools/anthropic_tool_use.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import asyncio
 import functools
 import inspect
 import json
+import os
 import re
 import time
 from enum import Enum
 from typing import Any, Dict, List, Literal, Optional, Tuple, TypedDict
 
+import jinja2
 from anthropic import (
     AnthropicError,
     APIConnectionError,
     APIStatusError,
     APITimeoutError,
     AsyncMessageStreamManager,
     AsyncMessageStreamT,
@@ -23,20 +25,15 @@
     ToolsBetaMessageParam,
 )
 from anthropic.types.message_param import MessageParam
 from promptflow import tool
 from promptflow.connections import CustomStrongTypeConnection
 from promptflow.contracts.types import PromptTemplate, Secret
 from promptflow.exceptions import SystemErrorException, UserErrorException
-from promptflow.tools.common import (
-    generate_retry_interval,
-    render_jinja_template,
-    to_bool,
-    validate_role,
-)
+from promptflow.tools.common import generate_retry_interval, to_bool, validate_role
 from promptflow.tools.exception import (
     ChatAPIInvalidFunctions,
     ExceedMaxRetryTimes,
     FunctionCallNotSupportedInStreamMode,
     LLMError,
     WrappedOpenAIError,
 )
@@ -199,15 +196,14 @@
         details_data[key] = value
     return details_data
 
 
 def _parse_chat(
     chat_str: str,
 ) -> Tuple[str | None, list[MessageParam | ToolsBetaMessageParam], bool]:
-
     valid_roles = ["system", "user", "assistant"]
     messages, is_tool_use = parse_template(chat_str, valid_roles)
 
     if messages[0]["role"] == "system":
         system = messages[0]["content"][0]["text"]
         chat_list = messages[1:]
     else:
@@ -406,19 +402,25 @@
     n: Optional[int] = None,
     stream: Optional[bool] = False,
     stop: Optional[list] = None,  # type: ignore
     user: Optional[str] = None,
     tools: Optional[list[ToolParam]] = None,  # type: ignore
     extra_headers: Optional[dict] = {},
     is_raw_output: Optional[bool] = False,
+    use_template_loader: Optional[bool] = False,
     **kwargs,
 ) -> str | dict | Message | AsyncMessageStreamManager:  # type: ignore
-    chat_str = render_jinja_template(
-        prompt, trim_blocks=True, keep_trailing_newline=True, **kwargs
+    file_loader = (
+        jinja2.FileSystemLoader(searchpath=os.getcwd()) if use_template_loader else None
+    )
+    env = jinja2.Environment(
+        trim_blocks=True, keep_trailing_newline=True, loader=file_loader
     )
+    template = env.from_string(prompt)
+    chat_str = template.render(**kwargs)
     system, messages, is_tool_use = _parse_chat(chat_str)
     # TODO: remove below type conversion after client can pass json rather than string.
     stream = to_bool(stream)
     params = {
         "model": model,
         "messages": messages,
         "max_tokens": int(max_tokens)
```

### Comparing `tool_use-0.2.0/tool_use/tools/openai_tool_use.py` & `tool_use-0.2.1rc1/tool_use/tools/openai_tool_use.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import asyncio
 import functools
 import inspect
 import json
+import os
 import re
 import time
 from ast import literal_eval
 from enum import Enum
 from typing import List, Optional, cast
 
+import jinja2
 from openai import (
     APIConnectionError,
     APIStatusError,
     APITimeoutError,
     OpenAIError,
     RateLimitError,
 )
@@ -23,15 +25,14 @@
 from promptflow.connections import AzureOpenAIConnection, OpenAIConnection
 from promptflow.contracts.types import PromptTemplate
 from promptflow.exceptions import SystemErrorException, UserErrorException
 from promptflow.tools.common import (
     generate_retry_interval,
     normalize_connection_config,
     process_function_call,
-    render_jinja_template,
     to_bool,
     to_content_str_or_list,
     try_parse_name_and_content,
     validate_functions,
     validate_role,
 )
 from promptflow.tools.exception import (
@@ -399,17 +400,20 @@
                 "Function calling has not been supported by stream mode yet."
             )
             raise FunctionCallNotSupportedInStreamMode(message=error_message)
 
         async def generator():
             async for chunk in completion:
                 if chunk.choices:
-                    yield chunk.choices[0].delta.content if hasattr(
-                        chunk.choices[0].delta, "content"
-                    ) and chunk.choices[0].delta.content is not None else ""
+                    yield (
+                        chunk.choices[0].delta.content
+                        if hasattr(chunk.choices[0].delta, "content")
+                        and chunk.choices[0].delta.content is not None
+                        else ""
+                    )
 
         return generator()
     else:
         # When calling function, function_call response will be returned as a field in message, so we need return
         # message directly. Otherwise, we only return content.
         if functions is not None:
             return completion.model_dump()["choices"][0]["message"]
@@ -437,19 +441,25 @@
     function_call: Optional[object] = None,
     functions: Optional[list] = None,  # type: ignore
     response_format: object = dict(type="text"),
     tools: Optional[list[ChatCompletionToolParam]] = None,  # type: ignore
     tool_choice: Optional[ChatCompletionNamedToolChoiceParam | str] = None,  # type: ignore
     extra_headers: Optional[dict] = {},
     is_raw_output: Optional[bool] = False,
+    use_template_loader: Optional[bool] = False,
     **kwargs,
 ) -> [str, dict]:  # type: ignore
-    chat_str = render_jinja_template(
-        prompt, trim_blocks=True, keep_trailing_newline=True, **kwargs
+    file_loader = (
+        jinja2.FileSystemLoader(searchpath=os.getcwd()) if use_template_loader else None
+    )
+    env = jinja2.Environment(
+        trim_blocks=True, keep_trailing_newline=True, loader=file_loader
     )
+    template = env.from_string(prompt)
+    chat_str = template.render(**kwargs)
     messages = _parse_chat(chat_str)
     # TODO: remove below type conversion after client can pass json rather than string.
     stream = to_bool(stream)
     params = {
         "model": model,
         "messages": messages,
         "temperature": float(temperature),
```

### Comparing `tool_use-0.2.0/tool_use/tools/utils.py` & `tool_use-0.2.1rc1/tool_use/tools/utils.py`

 * *Files identical despite different names*

### Comparing `tool_use-0.2.0/tool_use/yamls/anthropic_tool_use.yaml` & `tool_use-0.2.1rc1/tool_use/yamls/anthropic_tool_use.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -39,13 +39,17 @@
       type:
         - object
       optional: true
     is_raw_output:
       type:
         - bool
       optional: true
+    use_template_loader:
+      type:
+        - bool
+      optional: true
     stream:
       type:
         - bool
       optional: true
   module: tool_use.tools.anthropic_tool_use
   function: anthropic_tool_use
```

### Comparing `tool_use-0.2.0/tool_use/yamls/openai_tool_use.yaml` & `tool_use-0.2.1rc1/tool_use/yamls/openai_tool_use.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -73,13 +73,17 @@
       type:
         - object
       optional: true
     is_raw_output:
       type:
         - bool
       optional: true
+    use_template_loader:
+      type:
+        - bool
+      optional: true
     stream:
       type:
         - bool
       optional: true
   module: tool_use.tools.openai_tool_use
   function: openai_tool_use
```

### Comparing `tool_use-0.2.0/tool_use.egg-info/SOURCES.txt` & `tool_use-0.2.1rc1/tool_use.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 tests/__init__.py
 tests/test_anthropic_tool_use.py
 tests/test_exception.py
+tests/test_file_system_loader.py
 tests/test_openai_tool_use.py
 tool_use/__init__.py
 tool_use.egg-info/PKG-INFO
 tool_use.egg-info/SOURCES.txt
 tool_use.egg-info/dependency_links.txt
 tool_use.egg-info/entry_points.txt
 tool_use.egg-info/top_level.txt
```

