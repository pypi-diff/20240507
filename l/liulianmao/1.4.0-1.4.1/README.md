# Comparing `tmp/liulianmao-1.4.0.tar.gz` & `tmp/liulianmao-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liulianmao-1.4.0.tar", max compression
+gzip compressed data, was "liulianmao-1.4.1.tar", max compression
```

## Comparing `liulianmao-1.4.0.tar` & `liulianmao-1.4.1.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0     1086 2024-03-20 13:24:32.980497 liulianmao-1.4.0/LICENSE
--rw-r--r--   0        0        0      781 2024-05-02 16:41:01.767151 liulianmao-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     6686 2024-05-02 16:18:09.075783 liulianmao-1.4.0/README.md
--rw-r--r--   0        0        0       46 2024-05-02 16:46:19.722762 liulianmao-1.4.0/src/liulianmao/__init__.py
--rw-r--r--   0        0        0     5361 2024-05-02 16:37:51.958253 liulianmao-1.4.0/src/liulianmao/__main__.py
--rw-r--r--   0        0        0       20 2024-05-02 10:57:42.700258 liulianmao-1.4.0/src/liulianmao/client/__init__.py
--rw-r--r--   0        0        0       23 2024-05-01 15:35:10.006780 liulianmao-1.4.0/src/liulianmao/client/api/__init__.py
--rw-r--r--   0        0        0      737 2024-05-02 15:54:50.285280 liulianmao-1.4.0/src/liulianmao/client/api/llama.py
--rw-r--r--   0        0        0    12236 2024-05-02 16:45:45.299436 liulianmao-1.4.0/src/liulianmao/client/api/openai.py
--rw-r--r--   0        0        0     1219 2024-05-02 16:07:58.953960 liulianmao-1.4.0/src/liulianmao/client/api/README.md
--rw-r--r--   0        0        0     9737 2024-05-02 16:34:36.458629 liulianmao-1.4.0/src/liulianmao/client/core.py
--rw-r--r--   0        0        0      608 2024-04-05 06:17:08.745870 liulianmao-1.4.0/src/liulianmao/client/langchain.py
--rw-r--r--   0        0        0      543 2024-05-02 15:48:15.958476 liulianmao-1.4.0/src/liulianmao/client/utils/config.py
--rw-r--r--   0        0        0       29 2024-05-02 16:41:00.037192 liulianmao-1.4.0/src/liulianmao/const.py
--rw-r--r--   0        0        0      119 2024-04-14 08:22:48.496972 liulianmao-1.4.0/src/liulianmao/module/__init__.py
--rw-r--r--   0        0        0     2864 2024-04-14 08:22:48.515590 liulianmao-1.4.0/src/liulianmao/module/authentication.py
--rw-r--r--   0        0        0      399 2024-04-01 15:16:20.555012 liulianmao-1.4.0/src/liulianmao/module/const.py
--rw-r--r--   0        0        0      605 2024-04-01 17:40:59.131588 liulianmao-1.4.0/src/liulianmao/module/log.py
--rw-r--r--   0        0        0     2347 2024-04-14 09:58:34.104170 liulianmao-1.4.0/src/liulianmao/module/model.py
--rw-r--r--   0        0        0     1647 2024-05-01 14:53:06.868641 liulianmao-1.4.0/src/liulianmao/module/storage.py
--rw-r--r--   0        0        0        0 2024-04-03 12:56:52.620830 liulianmao-1.4.0/src/liulianmao/tool/__init__.py
--rw-r--r--   0        0        0     3728 2024-04-01 11:33:08.073130 liulianmao-1.4.0/src/liulianmao/tool/ls.py
--rw-r--r--   0        0        0     7593 1970-01-01 00:00:00.000000 liulianmao-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-03-20 13:24:32.980497 liulianmao-1.4.1/LICENSE
+-rw-r--r--   0        0        0      781 2024-05-07 08:03:24.970255 liulianmao-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     6686 2024-05-02 16:18:09.075783 liulianmao-1.4.1/README.md
+-rw-r--r--   0        0        0       46 2024-05-02 16:46:19.722762 liulianmao-1.4.1/src/liulianmao/__init__.py
+-rw-r--r--   0        0        0     6520 2024-05-07 08:11:08.340750 liulianmao-1.4.1/src/liulianmao/__main__.py
+-rw-r--r--   0        0        0       20 2024-05-02 10:57:42.700258 liulianmao-1.4.1/src/liulianmao/client/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-01 15:35:10.006780 liulianmao-1.4.1/src/liulianmao/client/api/__init__.py
+-rw-r--r--   0        0        0      737 2024-05-07 07:26:48.042973 liulianmao-1.4.1/src/liulianmao/client/api/llama.py
+-rw-r--r--   0        0        0    13543 2024-05-07 07:45:00.136793 liulianmao-1.4.1/src/liulianmao/client/api/openai.py
+-rw-r--r--   0        0        0     1219 2024-05-02 16:07:58.953960 liulianmao-1.4.1/src/liulianmao/client/api/README.md
+-rw-r--r--   0        0        0     2057 2024-05-07 08:00:54.082890 liulianmao-1.4.1/src/liulianmao/client/api/zhipu.py
+-rw-r--r--   0        0        0    10959 2024-05-07 07:32:41.397693 liulianmao-1.4.1/src/liulianmao/client/core.py
+-rw-r--r--   0        0        0      608 2024-04-05 06:17:08.745870 liulianmao-1.4.1/src/liulianmao/client/langchain.py
+-rw-r--r--   0        0        0      543 2024-05-07 07:26:48.089449 liulianmao-1.4.1/src/liulianmao/client/utils/config.py
+-rw-r--r--   0        0        0       29 2024-05-07 08:03:14.713889 liulianmao-1.4.1/src/liulianmao/const.py
+-rw-r--r--   0        0        0      119 2024-04-14 08:22:48.496972 liulianmao-1.4.1/src/liulianmao/module/__init__.py
+-rw-r--r--   0        0        0     2864 2024-05-07 07:26:48.103961 liulianmao-1.4.1/src/liulianmao/module/authentication.py
+-rw-r--r--   0        0        0      399 2024-04-01 15:16:20.555012 liulianmao-1.4.1/src/liulianmao/module/const.py
+-rw-r--r--   0        0        0      605 2024-04-01 17:40:59.131588 liulianmao-1.4.1/src/liulianmao/module/log.py
+-rw-r--r--   0        0        0     2347 2024-05-07 07:26:48.102958 liulianmao-1.4.1/src/liulianmao/module/model.py
+-rw-r--r--   0        0        0     1647 2024-05-07 07:26:48.106032 liulianmao-1.4.1/src/liulianmao/module/storage.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:56:52.620830 liulianmao-1.4.1/src/liulianmao/tool/__init__.py
+-rw-r--r--   0        0        0      862 2024-05-07 06:37:11.604677 liulianmao-1.4.1/src/liulianmao/tool/continuous_chat.py
+-rw-r--r--   0        0        0     3728 2024-05-07 07:26:48.119147 liulianmao-1.4.1/src/liulianmao/tool/ls.py
+-rw-r--r--   0        0        0     7593 1970-01-01 00:00:00.000000 liulianmao-1.4.1/PKG-INFO
```

### Comparing `liulianmao-1.4.0/LICENSE` & `liulianmao-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `liulianmao-1.4.0/pyproject.toml` & `liulianmao-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "liulianmao"
-version = "1.4.0"
+version = "1.4.1"
 description = "A LLM client for use from the command line or IDE."
 authors = ["快乐的老鼠宝宝 <laoshubaby@protonmail.com>"]
 license = "MIT"
 repository = "https://github.com/LaoshuBaby/liulianmao"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `liulianmao-1.4.0/README.md` & `liulianmao-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `liulianmao-1.4.0/src/liulianmao/__main__.py` & `liulianmao-1.4.1/src/liulianmao/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import argparse
 import os
 import sys
 from typing import List
 
 from module.log import logger
 
+from const import LIULIANMAO_VERSION
+
 
 @logger.catch(level="CRITICAL")
 def init_env():
     """
     Initialize the execution environment by setting system paths.
 
     This function checks whether the script is running from a PyInstaller
@@ -48,15 +50,15 @@
         )
 
     if parent_dir not in sys.path:
         sys.path.append(parent_dir)
 
 
 @logger.catch(level="CRITICAL")
-def main(recipe: List[str], actions: List[str]):
+def main(recipe: List[str], actions: List[str], **kwargs):
     """Execute the operations specified in the recipe list.
 
     根据提供的recipe列表和actions列表执行一系列操作。
 
     Args:
         recipe: A list of strings representing the operations to be processed.默认为["init", "chat"]。
         actions: A list of strings representing additional actions to be taken.
@@ -66,14 +68,23 @@
 
         question_file_path = os.path.join(
             str(get_user_folder()), PROJECT_FOLDER, "terminal", "question.txt"
         )
         os.startfile(question_file_path)
         sys.exit(0)
 
+    if "answer" in actions:
+        from module.const import PROJECT_FOLDER, get_user_folder
+
+        answer_file_path = os.path.join(
+            str(get_user_folder()), PROJECT_FOLDER, "terminal", "answer.txt"
+        )
+        os.startfile(answer_file_path)
+        sys.exit(0)
+
     if "config" in actions:
         from module.const import PROJECT_FOLDER, get_user_folder
 
         config_file_path = os.path.join(
             str(get_user_folder()), PROJECT_FOLDER, "assets", "config.json"
         )
         os.startfile(config_file_path)
@@ -107,31 +118,43 @@
     }
 
     logger.debug(f"[Recipe]: {recipe}")
     for operation_name in recipe:
         operation = operations.get(operation_name)
         if operation:
             if operation_name == "ask":
-                operation(actions["question"])
+                operation("this is a question")
+            if operation_name == "chat" or operation_name == "default":
+                operation(model_series=kwargs.get("series", "").lower())
             else:
                 operation()
         else:
             print(f"Operation {operation_name} is not defined.")
 
 
 if __name__ == "__main__":
     init_env()
+    logger.success(f"=== LIULIANMAO:{LIULIANMAO_VERSION} ===")
     default_recipe = ["default"]
     parser = argparse.ArgumentParser(description="Process some operations.")
     parser.add_argument(
         "-q",
         "-question",
         "--question",
+        nargs="?",
+        const=True,
+        default=False,
+        help="Open the question.txt file with default program or pass a specific message",
+    )
+    parser.add_argument(
+        "-a",
+        "-answer",
+        "--answer",
         action="store_true",
-        help="Open the question.txt file with default program",
+        help="Open the answer.txt file with default program",
     )
     parser.add_argument(
         "-c",
         "-config",
         "--config",
         action="store_true",
         help="Open the config.txt file with default program",
@@ -148,30 +171,44 @@
         "-key",
         "--key",
         action="store_true",
         help="Open OPENAI_API_KEY and OPENAI_BASE_URL files with default program",
     )
     parser.add_argument(
         "-i",
+        "-input",
+        "--input",
         help="Specify input file, read this file as question, not default question.txt",
     )
     parser.add_argument(
         "-o",
+        "-output",
+        "--output",
         help="Specify output file, write answer to this file, not default answer.txt",
     )
     parser.add_argument(
         "-r",
         "-recipe",
         "--recipe",
         nargs="*",
         default=default_recipe,
         help="List of operations to process",
     )
+    parser.add_argument(
+        "-s",
+        "-series",
+        "--series",
+        type=str,
+        default="openai",
+        help="A string representing a series",
+    )
     args = parser.parse_args()
 
     actions = []
-    if args.question:
+    if args.question is True:
         actions.append("question")
-    if args.config:
+    if args.answer is True:
+        actions.append("answer")
+    if args.config is True:
         actions.append("config")
 
-    main(recipe=args.recipe, actions=actions)
+    main(recipe=args.recipe, actions=actions, series=args.series)
```

### Comparing `liulianmao-1.4.0/src/liulianmao/client/api/llama.py` & `liulianmao-1.4.1/src/liulianmao/client/api/llama.py`

 * *Files identical despite different names*

### Comparing `liulianmao-1.4.0/src/liulianmao/client/api/openai.py` & `liulianmao-1.4.1/src/liulianmao/client/api/openai.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import os
 import sys
 from datetime import datetime
-from typing import List
+from typing import List, Optional
 
 import requests
 
 current_dir = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(os.path.join(current_dir, "..", ".."))
 
-from client.utils.config import load_conf
+
 from module.authentication import API_KEY, API_URL
 from module.log import logger
-from module.model import select_model
 from module.storage import PROJECT_FOLDER, get_user_folder, init
 
 conversation = []
 
 
-def openai_models(model_series: str = ""):
+def openai_models(model_series: str = "") -> List[str]:
     logger.debug(f"[model_series]: {model_series}")
     headers = {
         "Authorization": f"Bearer {API_KEY}",
         "Content-Type": "application/json",
     }
     logger.trace("[Headers]\n" + f"{headers}")
 
@@ -127,56 +126,94 @@
             response.status_code,
             "\n",
             response.content.decode("utf-8"),
         )
 
 
 def openai_chat_completion(
-    question, available_models: List[str] = [], amount: int = 1
-):
-    config = load_conf()
-    model_type = config["model_type"]
-    system_content = config["system_message"]["content"]
-    temperature = float(config["settings"]["temperature"])
+    prompt_question,
+    prompt_system,
+    model,
+    temperature: float = 0.5,
+    max_tokens: int = 2048,
+    top_p: float = 1.0,
+    frequency_penalty: float = 0.0,
+    presence_penalty: float = 0.0,
+    stop=None,
+    amount: int = 1,
+    use_plugin: bool = False,  # 新增参数来控制是否使用插件
+) -> Optional[dict]:
+    def validate_temperature(temperature: float) -> float:
+        min_temperature = 0.0
+        max_temperature = 1.0
+        if temperature > max_temperature or temperature < min_temperature:
+            logger.error("temperature not supported")
+            return 0.5
+        else:
+            return temperature
 
     headers = {
         "Authorization": f"Bearer {API_KEY}",
         "Content-Type": "application/json",
     }
 
+    # 初始化payload
     payload = {
-        "model": select_model(model_type, available_models, direct_debug=True),
         "messages": (
-            [{"role": "system", "content": system_content}]
+            [{"role": "system", "content": prompt_system}]
             + conversation
-            + [{"role": "user", "content": question}]
+            + [{"role": "user", "content": prompt_question}]
         ),
-        "temperature": temperature,
-        "max_tokens": 2048,
-        "top_p": 1.0,
-        "frequency_penalty": 0.0,
-        "presence_penalty": 0.0,
-        "stop": None,
+        "model": model,
+        "temperature": validate_temperature(temperature),
+        "max_tokens": max_tokens,
+        "top_p": top_p,
+        "frequency_penalty": frequency_penalty,
+        "presence_penalty": presence_penalty,
+        "stop": stop,
         "n": amount,
-        # "plugins": [
-        #     {
-        #         "name": "plugin_name_here",
-        #         "parameters": {"param1": "value1", "param2": "value2"},
-        #     }
-        # ],
     }
 
+    # 如果启用插件，添加到payload中
+    if use_plugin:
+        payload["tools"] = [
+            {
+                "type": "function",
+                "function": {
+                    "name": "get_current_weather",
+                    "description": "Get the current weather in a given location",
+                    "parameters": {
+                        "type": "object",
+                        "properties": {
+                            "location": {
+                                "type": "string",
+                                "description": "The city and state, e.g. San Francisco, CA",
+                            },
+                            "unit": {
+                                "type": "string",
+                                "enum": ["celsius", "fahrenheit"],
+                            },
+                        },
+                        "required": ["location"],
+                    },
+                },
+            }
+        ]
+        payload["tool_choice"] = (
+            "auto",
+        )  # auto is default, but we'll be explicit
+
     logger.trace("[Headers]\n" + f"{headers}")
     logger.trace("[Payload]\n" + f"{payload}")
 
     flag_echo_input = False
     if flag_echo_input:
-        logger.debug("[Question]\n" + f"{question}")
+        logger.debug("[Question]\n" + f"{prompt_question}")
     else:
-        logger.trace("[Question]\n" + f"{question}")
+        logger.trace("[Question]\n" + f"{prompt_question}")
 
     response = requests.post(
         API_URL + "/v1/chat/completions", headers=headers, json=payload
     )
 
     if response.status_code == 200:
         logger.trace("[Debug] response.status_code == 200")
@@ -184,15 +221,15 @@
         try:
             logger.trace("[Response]\n" + str(response.json()))
         except Exception as e:
             logger.trace(e)
             logger.critical("RESPONSE NOT JSON")
         # judge schema
         try:
-            conversation.append({"role": "user", "content": question})
+            conversation.append({"role": "user", "content": prompt_question})
             conversation.append(
                 {
                     "role": "system",
                     "content": response.json()["choices"][0]["message"][
                         "content"
                     ],
                 }
@@ -211,28 +248,27 @@
 
 
 def openai_images_generations(
     prompt,
     model: str = "dall-e-3",
     size: str = "1024x1024",
     quality: str = "standard",
-    num: int = 1,
+    amount: int = 1,
 ):
-    config = load_conf()
     headers = {
         "Authorization": f"Bearer {API_KEY}",
         "Content-Type": "application/json",
     }
 
     payload = {
         "model": model,
         "prompt": prompt,
         "size": size,
         "quality": quality,
-        "n": num,
+        "n": amount,
     }
 
     logger.trace("[Headers]\n" + f"{headers}")
     logger.trace("[Payload]\n" + f"{payload}")
 
     response = requests.post(
         API_URL + "/v1/images/generations", headers=headers, json=payload
```

### Comparing `liulianmao-1.4.0/src/liulianmao/client/api/README.md` & `liulianmao-1.4.1/src/liulianmao/client/api/README.md`

 * *Files identical despite different names*

### Comparing `liulianmao-1.4.0/src/liulianmao/client/core.py` & `liulianmao-1.4.1/src/liulianmao/client/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,23 +5,31 @@
 
 from .api.openai import (
     openai_audio_speech,
     openai_chat_completion,
     openai_images_generations,
     openai_models,
 )
+from .api.zhipu import zhipu_completion
 
 current_dir = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(os.path.join(current_dir, ".."))
 
+from client.utils.config import load_conf
 from module.log import logger
+from module.model import select_model
 from module.storage import PROJECT_FOLDER, get_user_folder, init
 
 
-def ask(msg: str, available_models: List[str] = [], default_amount: int = 1):
+def ask(
+    msg: str,
+    available_models: List[str] = [],
+    default_amount: int = 1,
+    model_series: str = "openai",
+):
     """
     Sends a message to the OpenAI chat completion API and processes the response.
 
     This function sends a given message to the OpenAI API, specifying the models
     to be used and the default amount of completions to return. It processes the
     API's response, logs token usage, and returns the content of the choices.
 
@@ -46,14 +54,16 @@
 
     返回：
         一个字符串列表，包含来自API的响应内容。
 
     抛出：
         Exception: 处理API响应或记录时发生错误。
     """
+    logger.info(f"[model_series]: {model_series}")
+
     if msg == "":
         logger.warning(
             "\n"
             + "You run /client.core.ask() without pass a question to it."
             + "\n"
             + "Maybe you are run headless want a one-time-one-sentence ask and don't want to chat a lot"
         )
@@ -61,69 +71,84 @@
     if available_models == []:
         logger.info(
             "\n"
             + "You run /client.core.ask() without pass available model to it. "
             + "\n"
             + "Don't worry, liulianmao will auto fetch this."
         )
-        available_models = openai_models("gpt")
-    response = openai_chat_completion(
-        msg, available_models, amount=default_amount
-    )
+
+    config = load_conf()
+
+    if model_series == "openai":
+        response = openai_chat_completion(
+            prompt_question=msg,
+            prompt_system=config["system_message"]["content"],
+            model=select_model(
+                config["model_type"], available_models, direct_debug=True
+            ),
+            temperature=float(config["settings"]["temperature"]),
+            amount=default_amount,
+        )
+    elif model_series == "zhipu":
+        response = zhipu_completion(
+            prompt_question=msg,
+            prompt_system=config["system_message"]["content"],
+        )
+    else:
+        response = {"choices": [{"message": {"content": "啊哈？"}}]}
+
     try:
         choices = response.get("choices", [])
 
         # 使用.get()方法更安全地访问字典键值，以避免KeyError异常
         response_usage_completion_tokens = response.get("usage", {}).get(
             "completion_tokens", -1
         )
         response_usage_prompt_tokens = response.get("usage", {}).get(
             "prompt_tokens", -1
         )
         response_usage_total_tokens = response.get("usage", {}).get(
             "total_tokens", -1
         )
 
-        # 假设这里有一些处理response的代码
+        # 使用展平路径的变量名进行日志记录，仅在包含token记录时
+        logger.debug(
+            "[Token Usage]\n"
+            + json.dumps(
+                {
+                    "response_usage_completion_tokens": response_usage_completion_tokens,
+                    "response_usage_prompt_tokens": response_usage_prompt_tokens,
+                    "response_usage_total_tokens": response_usage_total_tokens,
+                    # 计算验证
+                    "verify": f"{response_usage_completion_tokens} + {response_usage_prompt_tokens} = {response_usage_completion_tokens + response_usage_prompt_tokens}",
+                },
+                indent=2,
+                ensure_ascii=False,
+                sort_keys=False,
+            )
+        )
 
     except Exception as e:
         # 记录关键错误信息而不是直接退出程序，提供更好的错误上下文
         logger.exception(f"An error occurred: {e}", exc_info=True)
         # 可以在这里处理特定的清理工作，如果有必要的话
         # 最后，可能会根据程序的需要选择是否退出
         # sys.exit()
 
-    # 使用展平路径的变量名进行日志记录
-    logger.debug(
-        "[Token Usage]\n"
-        + json.dumps(
-            {
-                "response_usage_completion_tokens": response_usage_completion_tokens,
-                "response_usage_prompt_tokens": response_usage_prompt_tokens,
-                "response_usage_total_tokens": response_usage_total_tokens,
-                # 计算验证
-                "verify": f"{response_usage_completion_tokens} + {response_usage_prompt_tokens} = {response_usage_completion_tokens + response_usage_prompt_tokens}",
-            },
-            indent=2,
-            ensure_ascii=False,
-            sort_keys=False,
-        )
-    )
-
     # 根据choices的数量来输出
     for i, choice in enumerate(choices):
         logger.success(
             f"[Answer] ({i + 1}/{len(choices)})\n{choice['message']['content']}"
         )
 
     # 为了保持函数的兼容性（返回单一或多个答案），返回整个choices列表的消息内容
     return [choice["message"]["content"] for choice in choices]
 
 
-def chat():
+def chat(model_series: str = "openai"):
     """
     Initiates a chat conversation by reading a question from a file and calling the OpenAI API.
 
     This function initializes the environment, reads a question from a specified file,
     and uses the OpenAI API to generate a conversation based on the available models.
     It handles user input for follow-up questions and writes the conversation to a file if desired.
 
@@ -133,27 +158,35 @@
 
     此功能初始化环境，从指定文件读取一个问题，并使用OpenAI API根据可用模型生成对话。
     它处理用户输入的后续问题，并在需要时将对话写入文件。
 
     没有参数或返回值。此功能通过文件IO和日志记录等副作用进行操作。
     """
     init()
-    available_models = openai_models("gpt")
+
+    if model_series == "openai":
+        available_models = openai_models("gpt")
+    elif model_series == "zhipu":
+        available_models = ["glm-4"]
+    elif model_series == "llama":
+        available_models = ["llama3"]
+    else:
+        available_models = []
 
     with open(
         os.path.join(
             get_user_folder(), PROJECT_FOLDER, "terminal", "question.txt"
         ),
         "r",
         encoding="utf-8",
     ) as file:
         msg = file.read()
 
     flag_continue = True
-    conversation = ask(msg, available_models)
+    conversation = ask(msg, available_models, model_series=model_series)
 
     if not flag_continue:
         with open(
             os.path.join(
                 get_user_folder(), PROJECT_FOLDER, "terminal", "answer.txt"
             ),
             "w",
@@ -169,15 +202,19 @@
             time.sleep(0.05)
             logger.info("[Interaction] 请输入追问")
             append_question = input()
             append_question_judge = append_question.replace("\n", "").replace(
                 " ", ""
             )
             if append_question_judge != "END" and append_question_judge != "":
-                conversation = ask(append_question, available_models)
+                conversation = ask(
+                    append_question,
+                    available_models,
+                    model_series=model_series,
+                )
             else:
                 flag_end = True
                 break
 
 
 def talk():
     """
```

### Comparing `liulianmao-1.4.0/src/liulianmao/client/langchain.py` & `liulianmao-1.4.1/src/liulianmao/client/langchain.py`

 * *Files identical despite different names*

### Comparing `liulianmao-1.4.0/src/liulianmao/client/utils/config.py` & `liulianmao-1.4.1/src/liulianmao/client/utils/config.py`

 * *Files identical despite different names*

### Comparing `liulianmao-1.4.0/src/liulianmao/module/authentication.py` & `liulianmao-1.4.1/src/liulianmao/module/authentication.py`

 * *Files identical despite different names*

### Comparing `liulianmao-1.4.0/src/liulianmao/module/log.py` & `liulianmao-1.4.1/src/liulianmao/module/log.py`

 * *Files identical despite different names*

### Comparing `liulianmao-1.4.0/src/liulianmao/module/model.py` & `liulianmao-1.4.1/src/liulianmao/module/model.py`

 * *Files identical despite different names*

### Comparing `liulianmao-1.4.0/src/liulianmao/module/storage.py` & `liulianmao-1.4.1/src/liulianmao/module/storage.py`

 * *Files identical despite different names*

### Comparing `liulianmao-1.4.0/src/liulianmao/tool/ls.py` & `liulianmao-1.4.1/src/liulianmao/tool/ls.py`

 * *Files identical despite different names*

### Comparing `liulianmao-1.4.0/PKG-INFO` & `liulianmao-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liulianmao
-Version: 1.4.0
+Version: 1.4.1
 Summary: A LLM client for use from the command line or IDE.
 Home-page: https://github.com/LaoshuBaby/liulianmao
 License: MIT
 Author: 快乐的老鼠宝宝
 Author-email: laoshubaby@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

