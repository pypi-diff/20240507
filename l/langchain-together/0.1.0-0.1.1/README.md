# Comparing `tmp/langchain_together-0.1.0.tar.gz` & `tmp/langchain_together-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_together-0.1.0.tar", max compression
+gzip compressed data, was "langchain_together-0.1.1.tar", max compression
```

## Comparing `langchain_together-0.1.0.tar` & `langchain_together-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2024-04-09 19:24:18.852840 langchain_together-0.1.0/LICENSE
--rw-r--r--   0        0        0     1031 2024-04-09 19:24:18.852840 langchain_together-0.1.0/README.md
--rw-r--r--   0        0        0      233 2024-04-09 19:24:18.852840 langchain_together-0.1.0/langchain_together/__init__.py
--rw-r--r--   0        0        0     1657 2024-04-09 19:24:18.852840 langchain_together-0.1.0/langchain_together/embeddings.py
--rw-r--r--   0        0        0     8059 2024-04-09 19:24:18.852840 langchain_together-0.1.0/langchain_together/llms.py
--rw-r--r--   0        0        0        0 2024-04-09 19:24:18.852840 langchain_together-0.1.0/langchain_together/py.typed
--rw-r--r--   0        0        0      232 2024-04-09 19:24:18.852840 langchain_together-0.1.0/langchain_together/version.py
--rw-r--r--   0        0        0     2563 2024-04-09 19:24:18.852840 langchain_together-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1927 1970-01-01 00:00:00.000000 langchain_together-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-07 01:26:34.899991 langchain_together-0.1.1/LICENSE
+-rw-r--r--   0        0        0      905 2024-05-07 01:26:34.899991 langchain_together-0.1.1/README.md
+-rw-r--r--   0        0        0      224 2024-05-07 01:26:34.899991 langchain_together-0.1.1/langchain_together/__init__.py
+-rw-r--r--   0        0        0     3329 2024-05-07 01:26:34.903992 langchain_together-0.1.1/langchain_together/chat_models.py
+-rw-r--r--   0        0        0     9173 2024-05-07 01:26:34.903992 langchain_together-0.1.1/langchain_together/embeddings.py
+-rw-r--r--   0        0        0     7891 2024-05-07 01:26:34.903992 langchain_together-0.1.1/langchain_together/llms.py
+-rw-r--r--   0        0        0        0 2024-05-07 01:26:34.903992 langchain_together-0.1.1/langchain_together/py.typed
+-rw-r--r--   0        0        0     2765 2024-05-07 01:26:34.903992 langchain_together-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1816 1970-01-01 00:00:00.000000 langchain_together-0.1.1/PKG-INFO
```

### Comparing `langchain_together-0.1.0/LICENSE` & `langchain_together-0.1.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 LangChain, Inc.
+Copyright (c) 2024 LangChain, Inc.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `langchain_together-0.1.0/langchain_together/llms.py` & `langchain_together-0.1.1/langchain_together/llms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,77 +1,76 @@
 """Wrapper around Together AI's Completion API."""
+
 import logging
 import warnings
 from typing import Any, Dict, List, Optional
 
 import requests
 from aiohttp import ClientSession
 from langchain_core.callbacks import (
     AsyncCallbackManagerForLLMRun,
     CallbackManagerForLLMRun,
 )
 from langchain_core.language_models.llms import LLM
 from langchain_core.pydantic_v1 import Extra, SecretStr, root_validator
 from langchain_core.utils import convert_to_secret_str, get_from_dict_or_env
 
-from langchain_together.version import __version__
-
 logger = logging.getLogger(__name__)
 
 
 class Together(LLM):
     """LLM models from `Together`.
 
     To use, you'll need an API key which you can find here:
-    https://api.together.xyz/settings/api-keys. This can be passed in as init param
+    https://api.together.ai/settings/api-keys. This can be passed in as init param
     ``together_api_key`` or set as environment variable ``TOGETHER_API_KEY``.
 
     Together AI API reference: https://docs.together.ai/reference/completions
 
     Example:
         .. code-block:: python
 
             from langchain_together import Together
 
             model = Together(model_name="mistralai/Mixtral-8x7B-Instruct-v0.1")
     """
 
-    base_url: str = "https://api.together.xyz/v1/completions"
+    base_url: str = "https://api.together.ai/v1/completions"
     """Base completions API URL."""
     together_api_key: SecretStr
-    """Together AI API key. Get it here: https://api.together.xyz/settings/api-keys"""
+    """Together AI API key. Get it here: https://api.together.ai/settings/api-keys"""
     model: str
-    """Model name. Available models listed here: 
+    """Model name. Available models listed here:
         Base Models: https://docs.together.ai/docs/inference-models#language-models
         Chat Models: https://docs.together.ai/docs/inference-models#chat-models
     """
     temperature: Optional[float] = None
     """Model temperature."""
     top_p: Optional[float] = None
-    """Used to dynamically adjust the number of choices for each predicted token based 
-        on the cumulative probabilities. A value of 1 will always yield the same 
-        output. A temperature less than 1 favors more correctness and is appropriate 
-        for question answering or summarization. A value greater than 1 introduces more 
+    """Used to dynamically adjust the number of choices for each predicted token based
+        on the cumulative probabilities. A value of 1 will always yield the same
+        output. A temperature less than 1 favors more correctness and is appropriate
+        for question answering or summarization. A value greater than 1 introduces more
         randomness in the output.
     """
     top_k: Optional[int] = None
-    """Used to limit the number of choices for the next predicted word or token. It 
-        specifies the maximum number of tokens to consider at each step, based on their 
-        probability of occurrence. This technique helps to speed up the generation 
-        process and can improve the quality of the generated text by focusing on the 
+    """Used to limit the number of choices for the next predicted word or token. It
+        specifies the maximum number of tokens to consider at each step, based on their
+        probability of occurrence. This technique helps to speed up the generation
+        process and can improve the quality of the generated text by focusing on the
         most likely options.
     """
     max_tokens: Optional[int] = None
     """The maximum number of tokens to generate."""
     repetition_penalty: Optional[float] = None
-    """A number that controls the diversity of generated text by reducing the 
+    """A number that controls the diversity of generated text by reducing the
         likelihood of repeated sequences. Higher values decrease repetition.
     """
     logprobs: Optional[int] = None
-    """An integer that specifies how many top token log probabilities are included in 
+    """An integer that specifies how many top token log probabilities are included in
         the response for each token generation step.
     """
 
     class Config:
         """Configuration for this pydantic object."""
 
         extra = Extra.forbid
@@ -103,18 +102,14 @@
     def _llm_type(self) -> str:
         """Return type of model."""
         return "together"
 
     def _format_output(self, output: dict) -> str:
         return output["choices"][0]["text"]
 
-    @staticmethod
-    def get_user_agent() -> str:
-        return f"langchain-together/{__version__}"
-
     @property
     def default_params(self) -> Dict[str, Any]:
         return {
             "model": self.model,
             "temperature": self.temperature,
             "top_p": self.top_p,
             "top_k": self.top_k,
```

### Comparing `langchain_together-0.1.0/pyproject.toml` & `langchain_together-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 [tool.poetry]
 name = "langchain-together"
-version = "0.1.0"
-description = "An integration package connecting Together and LangChain"
+version = "0.1.1"
+description = "An integration package connecting Together AI and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/together"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1"
-together = "^0.2.10"
+langchain-core = "^0.1.44"
+langchain-openai = "^0.1.3"
 requests = "^2"
 aiohttp = "^3.9.1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 freezegun = "^1.2.2"
 pytest-mock = "^3.10.0"
 syrupy = "^4.0.2"
 pytest-watcher = "^0.3.4"
 pytest-asyncio = "^0.21.1"
+langchain-openai = { path = "../openai", develop = true }
 langchain-core = { path = "../../core", develop = true }
+docarray = "^0.32.1"
+pydantic = "^1.10.9"
+langchain-standard-tests = { path = "../../standard-tests", develop = true }
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
 
@@ -42,31 +46,33 @@
 
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.5"
 
+[tool.poetry.group.typing]
+optional = true
+
 [tool.poetry.group.typing.dependencies]
 mypy = "^0.991"
 langchain-core = { path = "../../core", develop = true }
 types-requests = "^2"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 langchain-core = { path = "../../core", develop = true }
 
-[tool.ruff.lint]
+[tool.ruff]
 select = [
-  "E",    # pycodestyle
-  "F",    # pyflakes
-  "I",    # isort
-  "T201", # print
+  "E", # pycodestyle
+  "F", # pyflakes
+  "I", # isort
 ]
 
 [tool.mypy]
 disallow_untyped_defs = "True"
 
 [tool.coverage.run]
 omit = ["tests/*"]
```

