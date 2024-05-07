# Comparing `tmp/martian_adapters-4.2.2.tar.gz` & `tmp/martian_adapters-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martian_adapters-4.2.2.tar", max compression
+gzip compressed data, was "martian_adapters-4.3.0.tar", max compression
```

## Comparing `martian_adapters-4.2.2.tar` & `martian_adapters-4.3.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0    35149 2024-05-03 22:55:45.842763 martian_adapters-4.2.2/LICENSE
--rw-r--r--   0        0        0     3452 2024-05-03 22:55:45.842763 martian_adapters-4.2.2/README.md
--rw-r--r--   0        0        0      725 2024-05-03 22:55:45.842763 martian_adapters-4.2.2/adapters/__init__.py
--rw-r--r--   0        0        0      305 2024-05-03 22:55:45.842763 martian_adapters-4.2.2/adapters/abstract_adapters/__init__.py
--rw-r--r--   0        0        0     2117 2024-05-03 22:55:45.842763 martian_adapters-4.2.2/adapters/abstract_adapters/api_key_adapter_mixin.py
--rw-r--r--   0        0        0     3347 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/abstract_adapters/base_adapter.py
--rw-r--r--   0        0        0     1226 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/abstract_adapters/chat_http_api_adapter.py
--rw-r--r--   0        0        0     7525 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/abstract_adapters/http_api_adapter_mixin.py
--rw-r--r--   0        0        0     2386 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/abstract_adapters/openai_sdk_chat_adapter.py
--rw-r--r--   0        0        0     3419 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/abstract_adapters/provider_adapter_mixin.py
--rw-r--r--   0        0        0     5816 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/abstract_adapters/sdk_chat_adapter.py
--rw-r--r--   0        0        0     5812 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/adapter_factory.py
--rw-r--r--   0        0        0       59 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/concrete_adapters/__init__.py
--rw-r--r--   0        0        0     3429 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/concrete_adapters/you_com_rag_chat_adapter.py
--rw-r--r--   0        0        0      942 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/provider_adapters/__init__.py
--rw-r--r--   0        0        0     9225 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     4102 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2412 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2587 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     7317 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1836 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1757 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1331 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     4444 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2450 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2602 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0    10017 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/provider_adapters/together_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0        0 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/py.typed
--rw-r--r--   0        0        0      558 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/rate_limiter.py
--rw-r--r--   0        0        0      335 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/requirements.txt
--rw-r--r--   0        0        0     6903 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/types.py
--rw-r--r--   0        0        0        0 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/utils/__init__.py
--rw-r--r--   0        0        0      263 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/utils/adapter_stream_response.py
--rw-r--r--   0        0        0     1064 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/utils/general_utils.py
--rw-r--r--   0        0        0     2492 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/utils/network_utils.py
--rw-r--r--   0        0        0     8173 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/adapters/utils/openai_client_factory.py
--rw-r--r--   0        0        0     1170 2024-05-03 22:55:45.846763 martian_adapters-4.2.2/pyproject.toml
--rw-r--r--   0        0        0     4800 1970-01-01 00:00:00.000000 martian_adapters-4.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/LICENSE
+-rw-r--r--   0        0        0     3553 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/README.md
+-rw-r--r--   0        0        0      725 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/__init__.py
+-rw-r--r--   0        0        0      305 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/abstract_adapters/__init__.py
+-rw-r--r--   0        0        0     2188 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/abstract_adapters/api_key_adapter_mixin.py
+-rw-r--r--   0        0        0     3347 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/abstract_adapters/base_adapter.py
+-rw-r--r--   0        0        0     1226 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/abstract_adapters/chat_http_api_adapter.py
+-rw-r--r--   0        0        0     7525 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/abstract_adapters/http_api_adapter_mixin.py
+-rw-r--r--   0        0        0     2486 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/abstract_adapters/openai_sdk_chat_adapter.py
+-rw-r--r--   0        0        0     3419 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/abstract_adapters/provider_adapter_mixin.py
+-rw-r--r--   0        0        0     5816 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/abstract_adapters/sdk_chat_adapter.py
+-rw-r--r--   0        0        0     5812 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/adapter_factory.py
+-rw-r--r--   0        0        0       59 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/concrete_adapters/__init__.py
+-rw-r--r--   0        0        0     3429 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/concrete_adapters/you_com_rag_chat_adapter.py
+-rw-r--r--   0        0        0     1017 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/provider_adapters/__init__.py
+-rw-r--r--   0        0        0     9225 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     4102 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2412 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2587 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     7317 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1836 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2995 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/provider_adapters/lepton_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1757 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1331 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     4444 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2450 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2602 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0    10017 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/provider_adapters/together_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/py.typed
+-rw-r--r--   0        0        0      558 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/rate_limiter.py
+-rw-r--r--   0        0        0      335 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/requirements.txt
+-rw-r--r--   0        0        0     6903 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/types.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/utils/__init__.py
+-rw-r--r--   0        0        0      263 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/utils/adapter_stream_response.py
+-rw-r--r--   0        0        0     1064 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/utils/general_utils.py
+-rw-r--r--   0        0        0     2492 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/utils/network_utils.py
+-rw-r--r--   0        0        0     8173 2024-05-07 17:38:10.859197 martian_adapters-4.3.0/adapters/utils/openai_client_factory.py
+-rw-r--r--   0        0        0     1170 2024-05-07 17:38:10.863197 martian_adapters-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4901 1970-01-01 00:00:00.000000 martian_adapters-4.3.0/PKG-INFO
```

### Comparing `martian_adapters-4.2.2/LICENSE` & `martian_adapters-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.2/README.md` & `martian_adapters-4.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,22 +12,27 @@
 - [Poetry](https://python-poetry.org/docs/#installation)
 
 ### Installation
 
 1. **Install Python:** Ensure Python `3.11.6` is installed on your system.
 2. **Install Poetry:** Follow the installation guide on the [official Poetry website](https://python-poetry.org/docs/#installation).
 3. **Install Dependencies:**
+
    ```bash
    poetry install
    ```
+
 4. **Install Pre-commit Hooks:**
+
    ```bash
    poetry run pre-commit install
    ```
+
 5. **Run Commands via Poetry:**
+
    ```bash
    poetry run pytest
    ```
 
 ### Setting Up Pre-commit
 
 Pre-commit hooks help maintain code quality and standards. Install them with the following command:
@@ -38,14 +43,18 @@
 
 To run pre-commit manually:
 
 ```bash
 poetry run pre-commit run --all-files
 ```
 
+### Semantic Versioning
+
+For versioning we follow [Semantic Versioning](https://semver.org)
+
 ### Environment Configuration
 
 The package requires certain environment variables to be set by the users:
 
 - Copy `.env-example` to `.env` and populate it with appropriate values.
 
 ### Running Tests
@@ -71,14 +80,15 @@
 2. **Convert Input:**
 
    ```python
    adapter1.convert_to_input(prompt)
    ```
 
 3. **Execute Adapter:**
+
    ```python
    adapter1.execute_async(input_data)
    ```
 
 ### Disabling Specific Models
 
 To disable models, set the `ADAPTER_DISABLED_MODELS` environment variable:
@@ -107,17 +117,19 @@
    - For providers with different schemas, see the "_Anthropic_" provider class for guidance.
 
 ### Development Steps
 
 1. **Add the Provider and Model:** Update `provider_adapters/__init__.py` and test files accordingly.
 2. **Write Tests:** Add tests in the relevant directories. Use `@pytest.mark.vcr` for tests making network requests.
 3. **Run Tests:**
+
    ```bash
    poetry run pytest
    ```
+
 4. **Check-in Cassette Files:** Include any new cassette YAML files in your commit.
 5. **Send a Pull Request:** Ensure all tests pass before requesting a review.
 
 ### Re-creating Cassette Files
 
 Use the `--record-mode=rewrite` option with pytest to update cassette files.
```

### Comparing `martian_adapters-4.2.2/adapters/__init__.py` & `martian_adapters-4.3.0/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.2/adapters/abstract_adapters/api_key_adapter_mixin.py` & `martian_adapters-4.3.0/adapters/abstract_adapters/api_key_adapter_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 
     def __init__(self):
         api_keys = os.environ.get(f"{self.get_api_key_name()}_LIST", None)
         if api_keys:
             api_keys = api_keys.split(",")
             for key in api_keys:
                 if not self.get_api_key_pattern().match(key):
-                    raise ValueError(f"api_key {key} is not a valid key")
+                    raise ValueError(
+                        f"api_key {key[:4]}**********{key[-4:]} is not a valid key"
+                    )
+
             ApiKeyAdapterMixin._api_keys = api_keys
         else:
             self._api_keys = [os.environ.get(self.get_api_key_name())]
 
     @staticmethod
     @abstractmethod
     def get_api_key_name() -> str:
```

### Comparing `martian_adapters-4.2.2/adapters/abstract_adapters/base_adapter.py` & `martian_adapters-4.3.0/adapters/abstract_adapters/base_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.2/adapters/abstract_adapters/chat_http_api_adapter.py` & `martian_adapters-4.3.0/adapters/abstract_adapters/chat_http_api_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.2/adapters/abstract_adapters/http_api_adapter_mixin.py` & `martian_adapters-4.3.0/adapters/abstract_adapters/http_api_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.2/adapters/abstract_adapters/openai_sdk_chat_adapter.py` & `martian_adapters-4.3.0/adapters/abstract_adapters/openai_sdk_chat_adapter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 
 from openai import AsyncOpenAI, OpenAI
 from openai.types.chat import ChatCompletion
+from openai.types.chat.chat_completion_chunk import ChatCompletionChunk
 
 from adapters.abstract_adapters.api_key_adapter_mixin import ApiKeyAdapterMixin
 from adapters.abstract_adapters.sdk_chat_adapter import SDKChatAdapter
 from adapters.types import (
     ConversationRole,
     Cost,
     OpenAIChatAdapterResponse,
@@ -67,9 +68,9 @@
             cost=cost,
             token_counts=Cost(
                 prompt=prompt_tokens,
                 completion=completion_tokens,
             ),
         )
 
-    def extract_stream_response(self, request, response):
+    def extract_stream_response(self, request, response: ChatCompletionChunk) -> str:
         return f"data: {json.dumps(response.dict())}\n\n"
```

### Comparing `martian_adapters-4.2.2/adapters/abstract_adapters/provider_adapter_mixin.py` & `martian_adapters-4.3.0/adapters/abstract_adapters/provider_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.2/adapters/abstract_adapters/sdk_chat_adapter.py` & `martian_adapters-4.3.0/adapters/abstract_adapters/sdk_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.2/adapters/adapter_factory.py` & `martian_adapters-4.3.0/adapters/adapter_factory.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.2/adapters/concrete_adapters/you_com_rag_chat_adapter.py` & `martian_adapters-4.3.0/adapters/concrete_adapters/you_com_rag_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.2/adapters/provider_adapters/__init__.py` & `martian_adapters-4.3.0/adapters/provider_adapters/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .anthropic_sdk_chat_provider_adapter import AnthropicSDKChatProviderAdapter
 from .anyscale_sdk_chat_provider_adapter import AnyscaleSDKChatProviderAdapter
 from .deepinfra_sdk_chat_provider_adapter import DeepInfraSDKChatProviderAdapter
 from .fireworks_sdk_chat_provider_adapter import FireworksSDKChatProviderAdapter
 from .gemini_sdk_chat_provider_adapter import GeminiSDKChatProviderAdapter
 from .groq_sdk_chat_provider_adapter import GroqSDKChatProviderAdapter
+from .lepton_sdk_chat_provider_adapter import LeptonSDKChatProviderAdapter
 from .moonshot_sdk_chat_provider_adapter import MoonshotSDKChatProviderAdapter
 from .octoai_sdk_chat_provider_adapter import OctoaiSDKChatProviderAdapter
 from .openai_sdk_chat_provider_adapter import OpenAISDKChatProviderAdapter
 from .openrouter_sdk_chat_provider_adapter import OpenRouterSDKChatProviderAdapter
 from .perplexity_sdk_chat_provider_adapter import PerplexitySDKChatProviderAdapter
 from .together_sdk_chat_provider_adapter import TogetherSDKChatProviderAdapter
```

### Comparing `martian_adapters-4.2.2/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py` & `martian_adapters-4.3.0/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.2/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py` & `martian_adapters-4.3.0/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.2/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py` & `martian_adapters-4.3.0/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.2/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py` & `martian_adapters-4.3.0/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.2/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py` & `martian_adapters-4.3.0/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.2/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py` & `martian_adapters-4.3.0/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.2/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py` & `martian_adapters-4.3.0/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.2/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py` & `martian_adapters-4.3.0/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.2/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py` & `martian_adapters-4.3.0/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.2/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py` & `martian_adapters-4.3.0/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.2/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py` & `martian_adapters-4.3.0/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.2/adapters/provider_adapters/together_sdk_chat_provider_adapter.py` & `martian_adapters-4.3.0/adapters/provider_adapters/together_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.2/adapters/rate_limiter.py` & `martian_adapters-4.3.0/adapters/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.2/adapters/types.py` & `martian_adapters-4.3.0/adapters/types.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.2/adapters/utils/general_utils.py` & `martian_adapters-4.3.0/adapters/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.2/adapters/utils/network_utils.py` & `martian_adapters-4.3.0/adapters/utils/network_utils.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.2/adapters/utils/openai_client_factory.py` & `martian_adapters-4.3.0/adapters/utils/openai_client_factory.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.2/pyproject.toml` & `martian_adapters-4.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [tool.poetry]
 name = "martian-adapters"
-version = "4.2.2"
+version = "4.3.0"
 description = "Adapters as API gateways to Different LLM Models"
 authors = ["Martian team <team@withmartian.com>"]
 readme = "README.md"
 packages = [{include = "adapters", from = "."}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-aiohttp = "^3.8.5"
+aiohttp = "^3.9.4"
 aiolimiter = "^1.1.0"
 aiosignal = "^1.3.1"
 anthropic = "0.16.0"
 async-timeout = "^4.0.3"
 attrs = "^23.1.0"
 certifi = "^2023.7.22"
 charset-normalizer = "^3.2.0"
 frozenlist = "^1.4.0"
-idna = "^3.4"
+idna = "^3.7"
 isort = "^5.12.0"
 multidict = "^6.0.4"
 regex = "^2023.8.8"
 requests = "^2.31.0"
 yarl = "^1.9.2"
 asyncio = "^3.4.3"
 tiktoken = "^0.5.1"
 pydantic = "^2.4.2"
 together = "^0.2.6"
-transformers = "^4.35.0"
+transformers = "^4.36.0"
 sentencepiece = "^0.1.99"
 openai = "1.23.6"
 vcrpy = "^6.0.1"
 google-generativeai = "^0.3.2"
 
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `martian_adapters-4.2.2/PKG-INFO` & `martian_adapters-4.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: martian-adapters
-Version: 4.2.2
+Version: 4.3.0
 Summary: Adapters as API gateways to Different LLM Models
 Author: Martian team
 Author-email: team@withmartian.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
+Requires-Dist: aiohttp (>=3.9.4,<4.0.0)
 Requires-Dist: aiolimiter (>=1.1.0,<2.0.0)
 Requires-Dist: aiosignal (>=1.3.1,<2.0.0)
 Requires-Dist: anthropic (==0.16.0)
 Requires-Dist: async-timeout (>=4.0.3,<5.0.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
 Requires-Dist: certifi (>=2023.7.22,<2024.0.0)
 Requires-Dist: charset-normalizer (>=3.2.0,<4.0.0)
 Requires-Dist: frozenlist (>=1.4.0,<2.0.0)
 Requires-Dist: google-generativeai (>=0.3.2,<0.4.0)
-Requires-Dist: idna (>=3.4,<4.0)
+Requires-Dist: idna (>=3.7,<4.0)
 Requires-Dist: isort (>=5.12.0,<6.0.0)
 Requires-Dist: multidict (>=6.0.4,<7.0.0)
 Requires-Dist: openai (==1.23.6)
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
 Requires-Dist: regex (>=2023.8.8,<2024.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: sentencepiece (>=0.1.99,<0.2.0)
 Requires-Dist: tiktoken (>=0.5.1,<0.6.0)
 Requires-Dist: together (>=0.2.6,<0.3.0)
-Requires-Dist: transformers (>=4.35.0,<5.0.0)
+Requires-Dist: transformers (>=4.36.0,<5.0.0)
 Requires-Dist: vcrpy (>=6.0.1,<7.0.0)
 Requires-Dist: yarl (>=1.9.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Adapters Package Documentation
 
 ## Overview
@@ -47,22 +47,27 @@
 - [Poetry](https://python-poetry.org/docs/#installation)
 
 ### Installation
 
 1. **Install Python:** Ensure Python `3.11.6` is installed on your system.
 2. **Install Poetry:** Follow the installation guide on the [official Poetry website](https://python-poetry.org/docs/#installation).
 3. **Install Dependencies:**
+
    ```bash
    poetry install
    ```
+
 4. **Install Pre-commit Hooks:**
+
    ```bash
    poetry run pre-commit install
    ```
+
 5. **Run Commands via Poetry:**
+
    ```bash
    poetry run pytest
    ```
 
 ### Setting Up Pre-commit
 
 Pre-commit hooks help maintain code quality and standards. Install them with the following command:
@@ -73,14 +78,18 @@
 
 To run pre-commit manually:
 
 ```bash
 poetry run pre-commit run --all-files
 ```
 
+### Semantic Versioning
+
+For versioning we follow [Semantic Versioning](https://semver.org)
+
 ### Environment Configuration
 
 The package requires certain environment variables to be set by the users:
 
 - Copy `.env-example` to `.env` and populate it with appropriate values.
 
 ### Running Tests
@@ -106,14 +115,15 @@
 2. **Convert Input:**
 
    ```python
    adapter1.convert_to_input(prompt)
    ```
 
 3. **Execute Adapter:**
+
    ```python
    adapter1.execute_async(input_data)
    ```
 
 ### Disabling Specific Models
 
 To disable models, set the `ADAPTER_DISABLED_MODELS` environment variable:
@@ -142,17 +152,19 @@
    - For providers with different schemas, see the "_Anthropic_" provider class for guidance.
 
 ### Development Steps
 
 1. **Add the Provider and Model:** Update `provider_adapters/__init__.py` and test files accordingly.
 2. **Write Tests:** Add tests in the relevant directories. Use `@pytest.mark.vcr` for tests making network requests.
 3. **Run Tests:**
+
    ```bash
    poetry run pytest
    ```
+
 4. **Check-in Cassette Files:** Include any new cassette YAML files in your commit.
 5. **Send a Pull Request:** Ensure all tests pass before requesting a review.
 
 ### Re-creating Cassette Files
 
 Use the `--record-mode=rewrite` option with pytest to update cassette files.
```

