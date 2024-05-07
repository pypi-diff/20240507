# Comparing `tmp/python_telegram_broadcast-0.9.0.tar.gz` & `tmp/python_telegram_broadcast-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_telegram_broadcast-0.9.0.tar", last modified: Tue May  7 03:29:33 2024, max compression
+gzip compressed data, was "python_telegram_broadcast-0.9.1.tar", last modified: Tue May  7 04:10:30 2024, max compression
```

## Comparing `python_telegram_broadcast-0.9.0.tar` & `python_telegram_broadcast-0.9.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 03:29:33.335973 python_telegram_broadcast-0.9.0/
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     1067 2024-05-06 01:52:00.000000 python_telegram_broadcast-0.9.0/LICENSE
--rw-r--r--   0 jonah     (1000) jonah     (1000)     3920 2024-05-07 03:29:33.335973 python_telegram_broadcast-0.9.0/PKG-INFO
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     3331 2024-05-07 02:48:22.000000 python_telegram_broadcast-0.9.0/README.md
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 03:29:33.331973 python_telegram_broadcast-0.9.0/python_telegram_broadcast/
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     3051 2024-05-07 03:28:42.000000 python_telegram_broadcast-0.9.0/python_telegram_broadcast/__init__.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     2963 2024-05-06 08:33:20.000000 python_telegram_broadcast-0.9.0/python_telegram_broadcast/custom_dataclass.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     1616 2024-05-06 08:35:01.000000 python_telegram_broadcast-0.9.0/python_telegram_broadcast/custom_exception.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     2236 2024-05-06 09:03:53.000000 python_telegram_broadcast-0.9.0/python_telegram_broadcast/custom_util.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     2417 2024-05-06 08:41:00.000000 python_telegram_broadcast-0.9.0/python_telegram_broadcast/main.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)    16983 2024-05-06 08:59:09.000000 python_telegram_broadcast-0.9.0/python_telegram_broadcast/send_method.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)    16160 2024-05-06 09:03:53.000000 python_telegram_broadcast-0.9.0/python_telegram_broadcast/strategy.py
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 03:29:33.331973 python_telegram_broadcast-0.9.0/python_telegram_broadcast.egg-info/
--rw-r--r--   0 jonah     (1000) jonah     (1000)     3920 2024-05-07 03:29:33.000000 python_telegram_broadcast-0.9.0/python_telegram_broadcast.egg-info/PKG-INFO
--rw-rw-r--   0 jonah     (1000) jonah     (1000)      554 2024-05-07 03:29:33.000000 python_telegram_broadcast-0.9.0/python_telegram_broadcast.egg-info/SOURCES.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)        1 2024-05-07 03:29:33.000000 python_telegram_broadcast-0.9.0/python_telegram_broadcast.egg-info/dependency_links.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)       33 2024-05-07 03:29:33.000000 python_telegram_broadcast-0.9.0/python_telegram_broadcast.egg-info/requires.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)       26 2024-05-07 03:29:33.000000 python_telegram_broadcast-0.9.0/python_telegram_broadcast.egg-info/top_level.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)       38 2024-05-07 03:29:33.335973 python_telegram_broadcast-0.9.0/setup.cfg
--rw-rw-r--   0 jonah     (1000) jonah     (1000)      952 2024-05-07 03:29:23.000000 python_telegram_broadcast-0.9.0/setup.py
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 04:10:30.626105 python_telegram_broadcast-0.9.1/
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     1067 2024-05-06 01:52:00.000000 python_telegram_broadcast-0.9.1/LICENSE
+-rw-r--r--   0 jonah     (1000) jonah     (1000)     3920 2024-05-07 04:10:30.626105 python_telegram_broadcast-0.9.1/PKG-INFO
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     3331 2024-05-07 02:48:22.000000 python_telegram_broadcast-0.9.1/README.md
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 04:10:30.626105 python_telegram_broadcast-0.9.1/python_telegram_broadcast/
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     3051 2024-05-07 03:28:42.000000 python_telegram_broadcast-0.9.1/python_telegram_broadcast/__init__.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     2963 2024-05-06 08:33:20.000000 python_telegram_broadcast-0.9.1/python_telegram_broadcast/custom_dataclass.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     1616 2024-05-06 08:35:01.000000 python_telegram_broadcast-0.9.1/python_telegram_broadcast/custom_exception.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     2236 2024-05-06 09:03:53.000000 python_telegram_broadcast-0.9.1/python_telegram_broadcast/custom_util.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     2729 2024-05-07 04:08:53.000000 python_telegram_broadcast-0.9.1/python_telegram_broadcast/main.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)    16983 2024-05-06 08:59:09.000000 python_telegram_broadcast-0.9.1/python_telegram_broadcast/send_method.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)    16698 2024-05-07 04:08:30.000000 python_telegram_broadcast-0.9.1/python_telegram_broadcast/strategy.py
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 04:10:30.626105 python_telegram_broadcast-0.9.1/python_telegram_broadcast.egg-info/
+-rw-r--r--   0 jonah     (1000) jonah     (1000)     3920 2024-05-07 04:10:30.000000 python_telegram_broadcast-0.9.1/python_telegram_broadcast.egg-info/PKG-INFO
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)      554 2024-05-07 04:10:30.000000 python_telegram_broadcast-0.9.1/python_telegram_broadcast.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)        1 2024-05-07 04:10:30.000000 python_telegram_broadcast-0.9.1/python_telegram_broadcast.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)       33 2024-05-07 04:10:30.000000 python_telegram_broadcast-0.9.1/python_telegram_broadcast.egg-info/requires.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)       26 2024-05-07 04:10:30.000000 python_telegram_broadcast-0.9.1/python_telegram_broadcast.egg-info/top_level.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)       38 2024-05-07 04:10:30.626105 python_telegram_broadcast-0.9.1/setup.cfg
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)      952 2024-05-07 04:08:34.000000 python_telegram_broadcast-0.9.1/setup.py
```

### Comparing `python_telegram_broadcast-0.9.0/LICENSE` & `python_telegram_broadcast-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.0/PKG-INFO` & `python_telegram_broadcast-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_telegram_broadcast
-Version: 0.9.0
+Version: 0.9.1
 Summary: Package that wraps the python-telegram-bot library to make broadcasting easier.
 Author: jonah_whaler_2348
 Author-email: jk_saga@proton.me
 License: MIT
 Keywords: python,telegram,broadcast,bot
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `python_telegram_broadcast-0.9.0/README.md` & `python_telegram_broadcast-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.0/python_telegram_broadcast/__init__.py` & `python_telegram_broadcast-0.9.1/python_telegram_broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.0/python_telegram_broadcast/custom_dataclass.py` & `python_telegram_broadcast-0.9.1/python_telegram_broadcast/custom_dataclass.py`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.0/python_telegram_broadcast/custom_exception.py` & `python_telegram_broadcast-0.9.1/python_telegram_broadcast/custom_exception.py`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.0/python_telegram_broadcast/custom_util.py` & `python_telegram_broadcast-0.9.1/python_telegram_broadcast/custom_util.py`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.0/python_telegram_broadcast/main.py` & `python_telegram_broadcast-0.9.1/python_telegram_broadcast/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,22 +27,28 @@
 
 
 async def handle_broadcast(
         subscribers: list[Tuple[int, str]], bot_token: str, broadcast_method: BroadcastMethodType | BroadcastMethodTypeHint,
         broadcast_strategy: BroadcastStrategyType | Callable[
             [...], Coroutine[Any, Any, Tuple[list[JobResponse], list[JobResponse]]]
         ],
-        content: str, caption: str, **configuration
+        content: str | list[str], caption: str | list[str], **configuration
 ) -> tuple[list[JobResponse], list[JobResponse]]:
     use_multiproc = configuration.get("use_multiproc", False)
     use_nproc = configuration.get("use_nproc", os.cpu_count())
     seconds = configuration.get("seconds", 0.0)
     max_retry = configuration.get("max_retry", 5)
     async_callback: Optional[Callable[[int], Coroutine[Any, Any, None]]] = configuration.get("async_callback", None)
     try:
+        # If content or caption is a string, convert it to a list of strings with the same length as subscribers
+        if type(content) is str:
+            content = [content] * len(subscribers)
+        if type(caption) is str:
+            caption = [caption] * len(subscribers)
+
         # Pick the appropriate broadcast method
         if type(broadcast_method) is BroadcastMethodType:
             broadcast_method = select_broadcast_method(broadcast_method)
         # Pick the appropriate broadcast strategy
         if type(broadcast_strategy) is BroadcastStrategyType:
             broadcast_strategy = select_broadcast_strategy(broadcast_strategy)
         return await broadcast_strategy().execute(
```

### Comparing `python_telegram_broadcast-0.9.0/python_telegram_broadcast/send_method.py` & `python_telegram_broadcast-0.9.1/python_telegram_broadcast/send_method.py`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.0/python_telegram_broadcast/strategy.py` & `python_telegram_broadcast-0.9.1/python_telegram_broadcast/strategy.py`

 * *Files 10% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         seconds: float = configuration.get("seconds", 0.0)  # Sleep for a short time to avoid overloading the CPU
         max_retry: int = configuration.get("max_retry", 5)
 
         # If content or caption is a string, convert it to a list of strings with the same length as subscribers
         if type(content) is str:
             content = [content] * len(subscribers)
         if type(caption) is str:
-            caption = [caption] * len(content)
+            caption = [caption] * len(subscribers)
 
         result_list: list[JobResponse] = []
         # Iterate over each subscriber and send the message
         for (telegram_id, username), _payload, _caption in zip(subscribers, content, caption):
             try:
                 # Attempt to send the message
                 send_result = await method(bot, telegram_id, _payload, _caption, seconds, 0, max_retry)
@@ -217,52 +217,52 @@
                 print(f"Number of processes exceeds the number of CPUs. Using {os.cpu_count()} processes instead.")
             use_nproc = os.cpu_count()
 
         # If content or caption is a string, convert it to a list of strings with the same length as subscribers
         if type(content) is str:
             content = [content] * len(subscribers)
         if type(caption) is str:
-            caption = [caption] * len(content)
+            caption = [caption] * len(subscribers)
 
         res_list: Queue[JobResponse] = Queue()  # Queue to store the results
         # Use a process pool executor to send messages concurrently
         with concurrent.futures.ProcessPoolExecutor(max_workers=use_nproc) as executor:
             loop = asyncio.get_event_loop()
             futures = []
             # Iterate over each subscriber and send the message
-            for telegram_id, username in subscribers:
+            for (telegram_id, username), _payload, _caption in zip(subscribers, content, caption):
                 try:
                     # Attempt to send the message
                     future = loop.run_in_executor(
                         executor,
-                        partial(broadcast_method_wrapper, method, bot_token, telegram_id, content, caption, 0,
+                        partial(broadcast_method_wrapper, method, bot_token, telegram_id, _payload, _caption, 0,
                                 max_retry)
                     )
                     futures.append(future)
                     if seconds > 0:
                         await asyncio.sleep(seconds)  # Sleep for a short time to avoid overloading the CPU
                 except Exception as error:
                     # If an error occurs, append the error information to the result list
                     error_info = ErrorInformation(type(error).__name__, str(error), traceback.format_exc())
-                    res_list.put(JobResponse(telegram_id, username, content, error_info))
+                    res_list.put(JobResponse(telegram_id, username, _payload, error_info))
 
             # Process the results
-            for future, (telegram_id, username) in zip(futures, subscribers):
+            for future, (telegram_id, username), _payload in zip(futures, subscribers, content):
                 try:
                     result = await future
                     res_list.put(JobResponse(telegram_id, username, content, result))
 
-                    if isinstance(result, dict):
+                    if isinstance(result, ErrorInformation):
                         continue
 
                     if success_callback:
                         await success_callback(telegram_id)
                 except Exception as error:
                     error_info = ErrorInformation(type(error).__name__, str(error), traceback.format_exc())
-                    res_list.put(JobResponse(telegram_id, username, content, error_info))
+                    res_list.put(JobResponse(telegram_id, username, _payload, error_info))
 
         # Group the results by success and failure
         sent_list, failed_list = separate_result_queue(res_list)
         return sent_list, failed_list
 
 
 class AsyncMultiProcessingPool(BroadcastStrategy):
@@ -313,39 +313,49 @@
         max_retry: int = configuration.get("max_retry", 5)
 
         if use_nproc > os.cpu_count():
             if self.verbose:
                 print(f"Number of processes exceeds the number of CPUs. Using {os.cpu_count()} processes instead.")
             use_nproc = os.cpu_count()
 
+        # If content or caption is a string, convert it to a list of strings with the same length as subscribers
+        if type(content) is str:
+            content = [content] * len(subscribers)
+        if type(caption) is str:
+            caption = [caption] * len(subscribers)
+
         res_list: Queue[JobResponse] = Queue()
         with multiprocessing.Pool(processes=use_nproc) as pool:
             results = []
-            for telegram_id, username in subscribers:
+            for (telegram_id, username), _payload, _caption in zip(subscribers, content, caption):
                 result = pool.apply_async(
                     broadcast_method_wrapper,
-                    (method, bot_token, telegram_id, content, caption, 0.0, max_retry)
+                    (method, bot_token, telegram_id, _payload, _caption, 0.0, max_retry)
                 )
                 results.append((result, telegram_id, username))
                 if seconds > 0:
                     await asyncio.sleep(seconds)
             pool.close()
             pool.join()
 
-        for result, telegram_id, username in results:
+        for (result, telegram_id, username), _payload in zip(results, content):
             try:
                 send_result = result.get()
-                res_list.put(JobResponse(telegram_id, username, content, send_result))
+                res_list.put(JobResponse(telegram_id, username, _payload, send_result))
+
+                if isinstance(send_result, ErrorInformation):
+                    continue
+
                 if success_callback:
                     await success_callback(telegram_id)
             except Exception as error:
                 error_info = ErrorInformation(
                     type(error).__name__, str(error), traceback.format_exc()
                 )
-                res_list.put(JobResponse(telegram_id, username, content, error_info))
+                res_list.put(JobResponse(telegram_id, username, _payload, error_info))
 
         sent_list, failed_list = separate_result_queue(res_list)
         return sent_list, failed_list
 
 
 def select_broadcast_strategy(strategy: BroadcastStrategyType) -> Type[BroadcastStrategy]:
     """
```

### Comparing `python_telegram_broadcast-0.9.0/python_telegram_broadcast.egg-info/PKG-INFO` & `python_telegram_broadcast-0.9.1/python_telegram_broadcast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-telegram-broadcast
-Version: 0.9.0
+Version: 0.9.1
 Summary: Package that wraps the python-telegram-bot library to make broadcasting easier.
 Author: jonah_whaler_2348
 Author-email: jk_saga@proton.me
 License: MIT
 Keywords: python,telegram,broadcast,bot
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `python_telegram_broadcast-0.9.0/python_telegram_broadcast.egg-info/SOURCES.txt` & `python_telegram_broadcast-0.9.1/python_telegram_broadcast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.0/setup.py` & `python_telegram_broadcast-0.9.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 DESCRIPTION = 'Package that wraps the python-telegram-bot library to make broadcasting easier.'
 
 # python3 setup.py sdist bdist_wheel
 # twine upload --skip-existing dist/*
 
-VERSION = '0.9.0'
+VERSION = '0.9.1'
 
 setup(
     name='python_telegram_broadcast',
     version=VERSION,
     packages=find_packages(),
     description=DESCRIPTION,
     long_description=open('README.md').read(),
```

