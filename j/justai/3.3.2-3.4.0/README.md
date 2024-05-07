# Comparing `tmp/justai-3.3.2.tar.gz` & `tmp/justai-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "justai-3.3.2.tar", last modified: Sun May  5 14:42:02 2024, max compression
+gzip compressed data, was "justai-3.4.0.tar", last modified: Tue May  7 08:47:24 2024, max compression
```

## Comparing `justai-3.3.2.tar` & `justai-3.4.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-05 14:42:02.784314 justai-3.3.2/
--rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 justai-3.3.2/LICENSE
--rw-r--r--   0 hp         (501) staff       (20)      198 2024-02-20 10:20:38.000000 justai-3.3.2/MANIFEST.in
--rw-r--r--   0 hp         (501) staff       (20)     6448 2024-05-05 14:42:02.784103 justai-3.3.2/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)     4082 2024-05-05 14:42:01.000000 justai-3.3.2/README.md
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-05 14:42:02.776805 justai-3.3.2/justai/
--rw-r--r--   0 hp         (501) staff       (20)      579 2024-04-01 20:26:06.000000 justai-3.3.2/justai/__init__.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-05 14:42:02.778114 justai-3.3.2/justai/agent/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:05:20.000000 justai-3.3.2/justai/agent/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     5992 2024-03-31 21:07:33.000000 justai-3.3.2/justai/agent/agent.py
--rw-r--r--   0 hp         (501) staff       (20)      997 2024-03-05 16:49:21.000000 justai-3.3.2/justai/agent/message.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-05 14:42:02.779889 justai-3.3.2/justai/interactive/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:06:50.000000 justai-3.3.2/justai/interactive/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     5452 2024-02-07 19:49:01.000000 justai-3.3.2/justai/interactive/commands.py
--rw-r--r--   0 hp         (501) staff       (20)     1320 2024-03-05 16:26:44.000000 justai-3.3.2/justai/interactive/repl.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-05 14:42:02.781044 justai-3.3.2/justai/models/
--rw-r--r--   0 hp         (501) staff       (20)     2987 2024-04-30 15:37:24.000000 justai-3.3.2/justai/models/anthropic_models.py
--rw-r--r--   0 hp         (501) staff       (20)     2465 2024-05-02 08:28:02.000000 justai-3.3.2/justai/models/gguf_models.py
--rw-r--r--   0 hp         (501) staff       (20)      920 2024-04-30 15:42:29.000000 justai-3.3.2/justai/models/model.py
--rw-r--r--   0 hp         (501) staff       (20)      709 2024-03-06 13:20:05.000000 justai-3.3.2/justai/models/modelfactory.py
--rw-r--r--   0 hp         (501) staff       (20)     5907 2024-04-04 20:33:40.000000 justai-3.3.2/justai/models/openai_models.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-05 14:42:02.782073 justai-3.3.2/justai/tools/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:08:21.000000 justai-3.3.2/justai/tools/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     3815 2024-04-02 09:00:24.000000 justai-3.3.2/justai/tools/cache.py
--rw-r--r--   0 hp         (501) staff       (20)      563 2023-08-26 19:32:55.000000 justai-3.3.2/justai/tools/display.py
--rw-r--r--   0 hp         (501) staff       (20)     3479 2024-04-29 12:34:52.000000 justai-3.3.2/justai/tools/log.py
--rw-r--r--   0 hp         (501) staff       (20)      615 2024-02-09 15:06:31.000000 justai-3.3.2/justai/tools/prompts.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-05 14:42:02.783286 justai-3.3.2/justai/translator/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:11:10.000000 justai-3.3.2/justai/translator/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     4052 2024-02-13 10:39:31.000000 justai-3.3.2/justai/translator/languages.py
--rw-r--r--   0 hp         (501) staff       (20)     1759 2024-04-05 09:44:01.000000 justai-3.3.2/justai/translator/prompts.toml
--rw-r--r--   0 hp         (501) staff       (20)    16685 2024-05-05 14:41:25.000000 justai-3.3.2/justai/translator/translator.py
--rw-r--r--   0 hp         (501) staff       (20)     5243 2024-02-16 15:51:36.000000 justai-3.3.2/justai/translator/xliff.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-05 14:42:02.783551 justai-3.3.2/justai.egg-info/
--rw-r--r--   0 hp         (501) staff       (20)     6448 2024-05-05 14:42:02.000000 justai-3.3.2/justai.egg-info/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)      785 2024-05-05 14:42:02.000000 justai-3.3.2/justai.egg-info/SOURCES.txt
--rw-r--r--   0 hp         (501) staff       (20)        1 2024-05-05 14:42:02.000000 justai-3.3.2/justai.egg-info/dependency_links.txt
--rw-r--r--   0 hp         (501) staff       (20)      146 2024-05-05 14:42:02.000000 justai-3.3.2/justai.egg-info/requires.txt
--rw-r--r--   0 hp         (501) staff       (20)        7 2024-05-05 14:42:02.000000 justai-3.3.2/justai.egg-info/top_level.txt
--rw-r--r--   0 hp         (501) staff       (20)      894 2024-05-05 14:42:01.000000 justai-3.3.2/pyproject.toml
--rw-r--r--   0 hp         (501) staff       (20)       38 2024-05-05 14:42:02.784362 justai-3.3.2/setup.cfg
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-07 08:47:24.883391 justai-3.4.0/
+-rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 justai-3.4.0/LICENSE
+-rw-r--r--   0 hp         (501) staff       (20)      198 2024-02-20 10:20:38.000000 justai-3.4.0/MANIFEST.in
+-rw-r--r--   0 hp         (501) staff       (20)     6448 2024-05-07 08:47:24.883198 justai-3.4.0/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)     4082 2024-05-07 08:47:23.000000 justai-3.4.0/README.md
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-07 08:47:24.876045 justai-3.4.0/justai/
+-rw-r--r--   0 hp         (501) staff       (20)      579 2024-04-01 20:26:06.000000 justai-3.4.0/justai/__init__.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-07 08:47:24.877442 justai-3.4.0/justai/agent/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:05:20.000000 justai-3.4.0/justai/agent/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     6234 2024-05-07 08:29:10.000000 justai-3.4.0/justai/agent/agent.py
+-rw-r--r--   0 hp         (501) staff       (20)      997 2024-03-05 16:49:21.000000 justai-3.4.0/justai/agent/message.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-07 08:47:24.878236 justai-3.4.0/justai/interactive/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:06:50.000000 justai-3.4.0/justai/interactive/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     5452 2024-02-07 19:49:01.000000 justai-3.4.0/justai/interactive/commands.py
+-rw-r--r--   0 hp         (501) staff       (20)     1320 2024-03-05 16:26:44.000000 justai-3.4.0/justai/interactive/repl.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-07 08:47:24.879598 justai-3.4.0/justai/models/
+-rw-r--r--   0 hp         (501) staff       (20)     4055 2024-05-07 08:44:49.000000 justai-3.4.0/justai/models/anthropic_models.py
+-rw-r--r--   0 hp         (501) staff       (20)     2465 2024-05-02 08:28:02.000000 justai-3.4.0/justai/models/gguf_models.py
+-rw-r--r--   0 hp         (501) staff       (20)     1009 2024-05-07 08:29:10.000000 justai-3.4.0/justai/models/model.py
+-rw-r--r--   0 hp         (501) staff       (20)      709 2024-03-06 13:20:05.000000 justai-3.4.0/justai/models/modelfactory.py
+-rw-r--r--   0 hp         (501) staff       (20)     6242 2024-05-07 08:33:08.000000 justai-3.4.0/justai/models/openai_models.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-07 08:47:24.880810 justai-3.4.0/justai/tools/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:08:21.000000 justai-3.4.0/justai/tools/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     3815 2024-04-02 09:00:24.000000 justai-3.4.0/justai/tools/cache.py
+-rw-r--r--   0 hp         (501) staff       (20)      563 2023-08-26 19:32:55.000000 justai-3.4.0/justai/tools/display.py
+-rw-r--r--   0 hp         (501) staff       (20)     3479 2024-04-29 12:34:52.000000 justai-3.4.0/justai/tools/log.py
+-rw-r--r--   0 hp         (501) staff       (20)      615 2024-02-09 15:06:31.000000 justai-3.4.0/justai/tools/prompts.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-07 08:47:24.882037 justai-3.4.0/justai/translator/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:11:10.000000 justai-3.4.0/justai/translator/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     4052 2024-02-13 10:39:31.000000 justai-3.4.0/justai/translator/languages.py
+-rw-r--r--   0 hp         (501) staff       (20)     1759 2024-04-05 09:44:01.000000 justai-3.4.0/justai/translator/prompts.toml
+-rw-r--r--   0 hp         (501) staff       (20)    16685 2024-05-05 14:41:25.000000 justai-3.4.0/justai/translator/translator.py
+-rw-r--r--   0 hp         (501) staff       (20)     5243 2024-02-16 15:51:36.000000 justai-3.4.0/justai/translator/xliff.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-07 08:47:24.882477 justai-3.4.0/justai.egg-info/
+-rw-r--r--   0 hp         (501) staff       (20)     6448 2024-05-07 08:47:24.000000 justai-3.4.0/justai.egg-info/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)      785 2024-05-07 08:47:24.000000 justai-3.4.0/justai.egg-info/SOURCES.txt
+-rw-r--r--   0 hp         (501) staff       (20)        1 2024-05-07 08:47:24.000000 justai-3.4.0/justai.egg-info/dependency_links.txt
+-rw-r--r--   0 hp         (501) staff       (20)      146 2024-05-07 08:47:24.000000 justai-3.4.0/justai.egg-info/requires.txt
+-rw-r--r--   0 hp         (501) staff       (20)        7 2024-05-07 08:47:24.000000 justai-3.4.0/justai.egg-info/top_level.txt
+-rw-r--r--   0 hp         (501) staff       (20)      894 2024-05-07 08:47:23.000000 justai-3.4.0/pyproject.toml
+-rw-r--r--   0 hp         (501) staff       (20)       38 2024-05-07 08:47:24.883427 justai-3.4.0/setup.cfg
```

### Comparing `justai-3.3.2/LICENSE` & `justai-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `justai-3.3.2/PKG-INFO` & `justai-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: justai
-Version: 3.3.2
+Version: 3.4.0
 Summary: Makes working with OpenAI's GPT API and other LLM's super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -54,15 +54,15 @@
 Requires-Dist: llama-cpp-python; extra == "llama"
 
 # JustAI
 
 Package to make working with Large Language models in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 3.3.2
+Current version: 3.4.0
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install justai
 ~~~~
 2. Create an OpenAI acccount (for GPT3.5 / 4) [here](https://platform.openai.com/) or an Anthropic account [here](https://console.anthropic.com/)
```

### Comparing `justai-3.3.2/README.md` & `justai-3.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # JustAI
 
 Package to make working with Large Language models in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 3.3.2
+Current version: 3.4.0
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install justai
 ~~~~
 2. Create an OpenAI acccount (for GPT3.5 / 4) [here](https://platform.openai.com/) or an Anthropic account [here](https://console.anthropic.com/)
```

### Comparing `justai-3.3.2/justai/__init__.py` & `justai-3.4.0/justai/__init__.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.2/justai/agent/agent.py` & `justai-3.4.0/justai/agent/agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -80,14 +80,20 @@
         start_time = time.time()
         self.messages.append(Message('user', prompt))
         model_response = cached_llm_response(self.model, self.get_messages(), return_json=return_json, use_cache=cached)
         text, self.input_token_count, self.output_token_count = model_response
         self.messages.append(Message('assistant', text))
         self.last_response_time = time.time() - start_time
         return text
+    
+    async def chat_async(self, prompt):
+        self.messages.append(Message('user', prompt))
+        for answer_text in self.model.chat_async(messages=self.get_messages()): 
+            if answer_text:
+                yield answer_text
 
     def after_response(self):
         # content is in messages[-1]['completion']['choices'][0]['message']['content']
         return  # Can be overridden
 
     def save(self, name=None):
         if not name:
```

### Comparing `justai-3.3.2/justai/agent/message.py` & `justai-3.4.0/justai/agent/message.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.2/justai/interactive/commands.py` & `justai-3.4.0/justai/interactive/commands.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.2/justai/interactive/repl.py` & `justai-3.4.0/justai/interactive/repl.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.2/justai/models/gguf_models.py` & `justai-3.4.0/justai/models/gguf_models.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.2/justai/models/model.py` & `justai-3.4.0/justai/models/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,9 +21,13 @@
         setattr(self, key, value)
 
     @abstractmethod
     def chat(self, messages: list[dict], return_json: bool, max_retries: int = 3) -> tuple[[str | object], int, int]:
         pass
 
     @abstractmethod
+    def chat_async(self, messages: list[dict]) -> str:
+        pass
+
+    @abstractmethod
     def token_count(self, text: str) -> int:
         pass
```

### Comparing `justai-3.3.2/justai/models/modelfactory.py` & `justai-3.4.0/justai/models/modelfactory.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.2/justai/models/openai_models.py` & `justai-3.4.0/justai/models/openai_models.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class OpenAIModel(Model):
     def __init__(self, model_name: str, params: dict = None):
         system_message = f"You are {model_name}, a large language model trained by OpenAI."
         super().__init__(model_name, params, system_message)
 
         # Authentication
         if "OPENAI_API_KEY" in params:
-            api_key = params["OPENAI_API_KEY"]
+            openai.api_key = params["OPENAI_API_KEY"]
         else:
             if not os.getenv("OPENAI_API_KEY"):
                 load_dotenv()  # Load the .env file into the environment
             openai.api_key = os.getenv("OPENAI_API_KEY")
         if not openai.api_key:
             color_print("No OpenAI API key found. Create one at https://platform.openai.com/account/api-keys and " +
                         "set it in the .env file like OPENAI_API_KEY=here_comes_your_key.", color=ERROR_COLOR)
@@ -78,26 +78,15 @@
             color_print("\nRunning completion with these messages", color=DEBUG_COLOR1)
             [color_print(m, color=DEBUG_COLOR1) for m in messages if hasattr(m, 'text')]
             print()
 
         last_error = None
         for _ in range(max_retries):
             try:
-                completion = self.client.chat.completions.create(
-                    model=self.model_name,
-                    messages=messages,
-                    temperature=self.model_params['temperature'],
-                    max_tokens=self.model_params['max_tokens'],
-                    n=self.model_params['n'],
-                    top_p=self.model_params['top_p'],
-                    frequency_penalty=self.model_params['frequency_penalty'],
-                    presence_penalty=self.model_params['presence_penalty'],
-                    stop=self.model_params['stop'],
-                    response_format={"type": "json_object"} if return_json else NOT_GIVEN,
-                )
+                completion = self.completion(messages, return_json)
                 message_text = completion.choices[0].message.content
                 input_token_count = completion.usage.prompt_tokens
                 output_token_count = completion.usage.completion_tokens
                 break
             except APIConnectionError as e:
                 color_print("Connection error.", color=SYSTEM_COLOR)
                 last_error = e
@@ -114,11 +103,31 @@
         if message_text.startswith('```json'):
             message_text = message_text[7:-3]
         if self.debug:
             color_print(f"{message_text}", color=DEBUG_COLOR2)
 
         text = json.loads(message_text) if return_json else message_text
         return text, input_token_count, output_token_count
+    
+    def chat_async(self, messages: list[dict]):
+        for item in self.completion(messages, stream=True):
+            if hasattr(item.choices[0].delta, "content"):
+                yield item.choices[0].delta.content
+               
+    def completion(self, messages: list[dict], return_json: bool = False, stream: bool=False):
+        return self.client.chat.completions.create(
+            model=self.model_name,
+            messages=messages,
+            temperature=self.model_params['temperature'],
+            max_tokens=self.model_params['max_tokens'],
+            n=self.model_params['n'],
+            top_p=self.model_params['top_p'],
+            frequency_penalty=self.model_params['frequency_penalty'],
+            presence_penalty=self.model_params['presence_penalty'],
+            stop=self.model_params['stop'],
+            response_format={"type": "json_object"} if return_json else NOT_GIVEN,
+            stream = stream
+        )
 
     def token_count(self, text: str) -> int:
         encoding = tiktoken.encoding_for_model(self.model_name)
         return len(encoding.encode(text))
```

### Comparing `justai-3.3.2/justai/tools/cache.py` & `justai-3.4.0/justai/tools/cache.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.2/justai/tools/display.py` & `justai-3.4.0/justai/tools/display.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.2/justai/tools/log.py` & `justai-3.4.0/justai/tools/log.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.2/justai/tools/prompts.py` & `justai-3.4.0/justai/tools/prompts.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.2/justai/translator/languages.py` & `justai-3.4.0/justai/translator/languages.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.2/justai/translator/prompts.toml` & `justai-3.4.0/justai/translator/prompts.toml`

 * *Files identical despite different names*

### Comparing `justai-3.3.2/justai/translator/translator.py` & `justai-3.4.0/justai/translator/translator.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.2/justai/translator/xliff.py` & `justai-3.4.0/justai/translator/xliff.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.2/justai.egg-info/PKG-INFO` & `justai-3.4.0/justai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: justai
-Version: 3.3.2
+Version: 3.4.0
 Summary: Makes working with OpenAI's GPT API and other LLM's super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -54,15 +54,15 @@
 Requires-Dist: llama-cpp-python; extra == "llama"
 
 # JustAI
 
 Package to make working with Large Language models in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 3.3.2
+Current version: 3.4.0
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install justai
 ~~~~
 2. Create an OpenAI acccount (for GPT3.5 / 4) [here](https://platform.openai.com/) or an Anthropic account [here](https://console.anthropic.com/)
```

### Comparing `justai-3.3.2/justai.egg-info/SOURCES.txt` & `justai-3.4.0/justai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `justai-3.3.2/pyproject.toml` & `justai-3.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=69", "wheel>=0.42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "justai"
-version = "3.3.2"
+version = "3.4.0"
 description = "Makes working with OpenAI's GPT API and other LLM's super easy"
 readme = "README.md"
 authors = [{ name = "HP Harmsen", email = "hp@harmsen.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

