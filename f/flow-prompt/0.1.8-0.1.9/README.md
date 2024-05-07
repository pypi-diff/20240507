# Comparing `tmp/flow_prompt-0.1.8.tar.gz` & `tmp/flow_prompt-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow_prompt-0.1.8.tar", max compression
+gzip compressed data, was "flow_prompt-0.1.9.tar", max compression
```

## Comparing `flow_prompt-0.1.8.tar` & `flow_prompt-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11356 2024-01-29 13:54:07.475880 flow_prompt-0.1.8/LICENSE
--rw-r--r--   0        0        0     6598 2024-03-13 11:37:24.807443 flow_prompt-0.1.8/README.md
--rw-r--r--   0        0        0      997 2024-03-13 12:06:06.341438 flow_prompt-0.1.8/flow_prompt/__init__.py
--rw-r--r--   0        0        0        0 2024-01-29 13:53:51.433509 flow_prompt-0.1.8/flow_prompt/ai_models/__init__.py
--rw-r--r--   0        0        0     1029 2024-03-14 14:33:40.355847 flow_prompt-0.1.8/flow_prompt/ai_models/ai_model.py
--rw-r--r--   0        0        0     1433 2024-02-08 12:46:19.795281 flow_prompt-0.1.8/flow_prompt/ai_models/attempt_to_call.py
--rw-r--r--   0        0        0     2274 2024-02-17 12:45:19.512114 flow_prompt-0.1.8/flow_prompt/ai_models/behaviour.py
--rw-r--r--   0        0        0        0 2024-02-11 15:22:24.848255 flow_prompt-0.1.8/flow_prompt/ai_models/openai/__init__.py
--rw-r--r--   0        0        0     3329 2024-03-13 12:06:23.401477 flow_prompt-0.1.8/flow_prompt/ai_models/openai/azure_models.py
--rw-r--r--   0        0        0     2739 2024-02-16 09:15:46.015918 flow_prompt-0.1.8/flow_prompt/ai_models/openai/behaviours.py
--rw-r--r--   0        0        0      803 2024-01-29 13:53:51.435506 flow_prompt-0.1.8/flow_prompt/ai_models/openai/exceptions.py
--rw-r--r--   0        0        0     6067 2024-03-12 09:17:59.803058 flow_prompt-0.1.8/flow_prompt/ai_models/openai/openai_models.py
--rw-r--r--   0        0        0     2080 2024-03-12 09:17:59.804474 flow_prompt-0.1.8/flow_prompt/ai_models/openai/responses.py
--rw-r--r--   0        0        0     1616 2024-02-16 09:15:46.016998 flow_prompt-0.1.8/flow_prompt/ai_models/openai/utils.py
--rw-r--r--   0        0        0      500 2024-02-16 09:15:46.017253 flow_prompt-0.1.8/flow_prompt/exceptions.py
--rw-r--r--   0        0        0        0 2024-01-29 13:53:02.528231 flow_prompt-0.1.8/flow_prompt/prompt/__init__.py
--rw-r--r--   0        0        0     2347 2024-03-26 16:49:59.672325 flow_prompt-0.1.8/flow_prompt/prompt/base_prompt.py
--rw-r--r--   0        0        0     5556 2024-02-16 09:15:46.017767 flow_prompt-0.1.8/flow_prompt/prompt/chat.py
--rw-r--r--   0        0        0     7808 2024-03-15 09:30:16.913961 flow_prompt-0.1.8/flow_prompt/prompt/flow_prompt.py
--rw-r--r--   0        0        0     4264 2024-03-25 09:09:27.436692 flow_prompt-0.1.8/flow_prompt/prompt/pipe_prompt.py
--rw-r--r--   0        0        0    10760 2024-03-12 09:17:59.810714 flow_prompt-0.1.8/flow_prompt/prompt/user_prompt.py
--rw-r--r--   0        0        0      936 2024-03-16 12:03:11.110348 flow_prompt-0.1.8/flow_prompt/responses.py
--rw-r--r--   0        0        0     1323 2024-03-15 09:30:11.152268 flow_prompt-0.1.8/flow_prompt/services/SaveWorker.py
--rw-r--r--   0        0        0        0 2024-01-29 13:53:02.529439 flow_prompt-0.1.8/flow_prompt/services/__init__.py
--rw-r--r--   0        0        0     5243 2024-03-17 17:43:38.933608 flow_prompt-0.1.8/flow_prompt/services/flow_prompt/__init__.py
--rw-r--r--   0        0        0     1707 2024-03-21 18:18:50.777475 flow_prompt-0.1.8/flow_prompt/settings.py
--rw-r--r--   0        0        0      678 2024-02-16 09:15:46.020056 flow_prompt-0.1.8/flow_prompt/utils.py
--rw-r--r--   0        0        0      543 2024-03-26 17:25:59.726786 flow_prompt-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     7129 1970-01-01 00:00:00.000000 flow_prompt-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-01-29 13:54:07.475880 flow_prompt-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2550 2024-03-26 19:33:05.507859 flow_prompt-0.1.9/README.md
+-rw-r--r--   0        0        0      997 2024-03-13 12:06:06.341438 flow_prompt-0.1.9/flow_prompt/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-29 13:53:51.433509 flow_prompt-0.1.9/flow_prompt/ai_models/__init__.py
+-rw-r--r--   0        0        0     1029 2024-03-14 14:33:40.355847 flow_prompt-0.1.9/flow_prompt/ai_models/ai_model.py
+-rw-r--r--   0        0        0     1433 2024-02-08 12:46:19.795281 flow_prompt-0.1.9/flow_prompt/ai_models/attempt_to_call.py
+-rw-r--r--   0        0        0     2274 2024-02-17 12:45:19.512114 flow_prompt-0.1.9/flow_prompt/ai_models/behaviour.py
+-rw-r--r--   0        0        0        0 2024-02-11 15:22:24.848255 flow_prompt-0.1.9/flow_prompt/ai_models/openai/__init__.py
+-rw-r--r--   0        0        0     3297 2024-03-26 19:18:01.677112 flow_prompt-0.1.9/flow_prompt/ai_models/openai/azure_models.py
+-rw-r--r--   0        0        0     2739 2024-02-16 09:15:46.015918 flow_prompt-0.1.9/flow_prompt/ai_models/openai/behaviours.py
+-rw-r--r--   0        0        0      803 2024-01-29 13:53:51.435506 flow_prompt-0.1.9/flow_prompt/ai_models/openai/exceptions.py
+-rw-r--r--   0        0        0     6067 2024-03-12 09:17:59.803058 flow_prompt-0.1.9/flow_prompt/ai_models/openai/openai_models.py
+-rw-r--r--   0        0        0     2080 2024-03-12 09:17:59.804474 flow_prompt-0.1.9/flow_prompt/ai_models/openai/responses.py
+-rw-r--r--   0        0        0     1616 2024-02-16 09:15:46.016998 flow_prompt-0.1.9/flow_prompt/ai_models/openai/utils.py
+-rw-r--r--   0        0        0      500 2024-02-16 09:15:46.017253 flow_prompt-0.1.9/flow_prompt/exceptions.py
+-rw-r--r--   0        0        0        0 2024-01-29 13:53:02.528231 flow_prompt-0.1.9/flow_prompt/prompt/__init__.py
+-rw-r--r--   0        0        0     2347 2024-03-26 16:49:59.672325 flow_prompt-0.1.9/flow_prompt/prompt/base_prompt.py
+-rw-r--r--   0        0        0     5556 2024-02-16 09:15:46.017767 flow_prompt-0.1.9/flow_prompt/prompt/chat.py
+-rw-r--r--   0        0        0     7794 2024-03-26 19:12:37.357209 flow_prompt-0.1.9/flow_prompt/prompt/flow_prompt.py
+-rw-r--r--   0        0        0     4264 2024-03-25 09:09:27.436692 flow_prompt-0.1.9/flow_prompt/prompt/pipe_prompt.py
+-rw-r--r--   0        0        0    10760 2024-03-12 09:17:59.810714 flow_prompt-0.1.9/flow_prompt/prompt/user_prompt.py
+-rw-r--r--   0        0        0      936 2024-03-16 12:03:11.110348 flow_prompt-0.1.9/flow_prompt/responses.py
+-rw-r--r--   0        0        0     1323 2024-03-15 09:30:11.152268 flow_prompt-0.1.9/flow_prompt/services/SaveWorker.py
+-rw-r--r--   0        0        0        0 2024-01-29 13:53:02.529439 flow_prompt-0.1.9/flow_prompt/services/__init__.py
+-rw-r--r--   0        0        0     5243 2024-03-17 17:43:38.933608 flow_prompt-0.1.9/flow_prompt/services/flow_prompt/__init__.py
+-rw-r--r--   0        0        0     1693 2024-03-26 19:12:37.356666 flow_prompt-0.1.9/flow_prompt/settings.py
+-rw-r--r--   0        0        0      678 2024-02-16 09:15:46.020056 flow_prompt-0.1.9/flow_prompt/utils.py
+-rw-r--r--   0        0        0      543 2024-03-26 19:36:37.104792 flow_prompt-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 flow_prompt-0.1.9/PKG-INFO
```

### Comparing `flow_prompt-0.1.8/LICENSE` & `flow_prompt-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flow_prompt-0.1.8/flow_prompt/__init__.py` & `flow_prompt-0.1.9/flow_prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `flow_prompt-0.1.8/flow_prompt/ai_models/ai_model.py` & `flow_prompt-0.1.9/flow_prompt/ai_models/ai_model.py`

 * *Files identical despite different names*

### Comparing `flow_prompt-0.1.8/flow_prompt/ai_models/attempt_to_call.py` & `flow_prompt-0.1.9/flow_prompt/ai_models/attempt_to_call.py`

 * *Files identical despite different names*

### Comparing `flow_prompt-0.1.8/flow_prompt/ai_models/behaviour.py` & `flow_prompt-0.1.9/flow_prompt/ai_models/behaviour.py`

 * *Files identical despite different names*

### Comparing `flow_prompt-0.1.8/flow_prompt/ai_models/openai/azure_models.py` & `flow_prompt-0.1.9/flow_prompt/ai_models/openai/azure_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import logging
 import typing as t
 from dataclasses import dataclass
 
-from openai import AzureOpenAI
-
 from flow_prompt import settings
 from flow_prompt.ai_models.ai_model import AI_MODELS_PROVIDER
 from flow_prompt.ai_models.openai.openai_models import FamilyModel, OpenAIModel
 from flow_prompt.exceptions import ProviderNotFoundException
 
 logger = logging.getLogger(__name__)
```

### Comparing `flow_prompt-0.1.8/flow_prompt/ai_models/openai/behaviours.py` & `flow_prompt-0.1.9/flow_prompt/ai_models/openai/behaviours.py`

 * *Files identical despite different names*

### Comparing `flow_prompt-0.1.8/flow_prompt/ai_models/openai/exceptions.py` & `flow_prompt-0.1.9/flow_prompt/ai_models/openai/exceptions.py`

 * *Files identical despite different names*

### Comparing `flow_prompt-0.1.8/flow_prompt/ai_models/openai/openai_models.py` & `flow_prompt-0.1.9/flow_prompt/ai_models/openai/openai_models.py`

 * *Files identical despite different names*

### Comparing `flow_prompt-0.1.8/flow_prompt/ai_models/openai/responses.py` & `flow_prompt-0.1.9/flow_prompt/ai_models/openai/responses.py`

 * *Files identical despite different names*

### Comparing `flow_prompt-0.1.8/flow_prompt/ai_models/openai/utils.py` & `flow_prompt-0.1.9/flow_prompt/ai_models/openai/utils.py`

 * *Files identical despite different names*

### Comparing `flow_prompt-0.1.8/flow_prompt/prompt/base_prompt.py` & `flow_prompt-0.1.9/flow_prompt/prompt/base_prompt.py`

 * *Files identical despite different names*

### Comparing `flow_prompt-0.1.8/flow_prompt/prompt/chat.py` & `flow_prompt-0.1.9/flow_prompt/prompt/chat.py`

 * *Files identical despite different names*

### Comparing `flow_prompt-0.1.8/flow_prompt/prompt/flow_prompt.py` & `flow_prompt-0.1.9/flow_prompt/prompt/flow_prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,17 +30,17 @@
     openai_org: str = None
     azure_keys: t.Dict[str, str] = None
     secrets: Secrets = None
 
     def __post_init__(self):
         self.secrets = Secrets()
         if not self.azure_keys:
-            if self.secrets.AZURE_OPENAI_KEYS:
+            if self.secrets.azure_keys:
                 logger.debug(f"Using Azure keys from secrets")
-                self.azure_keys = self.secrets.AZURE_OPENAI_KEYS
+                self.azure_keys = self.secrets.azure_keys
             else:
                 logger.debug(f"Azure keys not found in secrets")
         if not self.api_token and self.secrets.API_TOKEN:
             logger.debug(f"Using API token from secrets")
             self.api_token = self.secrets.API_TOKEN
         if not self.openai_api_key and self.secrets.OPENAI_API_KEY:
             logger.debug(f"Using OpenAI API key from secrets")
```

### Comparing `flow_prompt-0.1.8/flow_prompt/prompt/pipe_prompt.py` & `flow_prompt-0.1.9/flow_prompt/prompt/pipe_prompt.py`

 * *Files identical despite different names*

### Comparing `flow_prompt-0.1.8/flow_prompt/prompt/user_prompt.py` & `flow_prompt-0.1.9/flow_prompt/prompt/user_prompt.py`

 * *Files identical despite different names*

### Comparing `flow_prompt-0.1.8/flow_prompt/responses.py` & `flow_prompt-0.1.9/flow_prompt/responses.py`

 * *Files identical despite different names*

### Comparing `flow_prompt-0.1.8/flow_prompt/services/SaveWorker.py` & `flow_prompt-0.1.9/flow_prompt/services/SaveWorker.py`

 * *Files identical despite different names*

### Comparing `flow_prompt-0.1.8/flow_prompt/services/flow_prompt/__init__.py` & `flow_prompt-0.1.9/flow_prompt/services/flow_prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `flow_prompt-0.1.8/flow_prompt/settings.py` & `flow_prompt-0.1.9/flow_prompt/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,9 +35,9 @@
 
 
 @dataclass
 class Secrets:
     API_TOKEN: str = field(default_factory=lambda: os.getenv("FLOW_PROMPT_API_TOKEN"))
     OPENAI_API_KEY: str = field(default_factory=lambda: os.getenv("OPENAI_API_KEY"))
     OPENAI_ORG: str = field(default_factory=lambda: os.getenv("OPENAI_ORG"))
-    AZURE_OPENAI_KEYS: dict = field(default_factory=lambda: json.loads(os.getenv("AZURE_OPENAI_KEYS", "{}")))
+    azure_keys: dict = field(default_factory=lambda: json.loads(os.getenv("azure_keys", "{}")))
```

### Comparing `flow_prompt-0.1.8/flow_prompt/utils.py` & `flow_prompt-0.1.9/flow_prompt/utils.py`

 * *Files identical despite different names*

### Comparing `flow_prompt-0.1.8/pyproject.toml` & `flow_prompt-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flow-prompt"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Flow-prompt Engineering Team <engineering@flow-prompt.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 tiktoken = ">=0.5.2"
```

