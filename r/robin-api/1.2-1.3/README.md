# Comparing `tmp/robin_api-1.2.tar.gz` & `tmp/robin_api-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robin_api-1.2.tar", last modified: Wed May  1 20:42:05 2024, max compression
+gzip compressed data, was "robin_api-1.3.tar", last modified: Tue May  7 04:34:06 2024, max compression
```

## Comparing `robin_api-1.2.tar` & `robin_api-1.3.tar`

### file list

```diff
@@ -1,31 +1,36 @@
-drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-01 20:42:05.371209 robin_api-1.2/
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    11337 2024-04-30 18:06:24.000000 robin_api-1.2/LICENSE
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      210 2024-05-01 19:41:22.000000 robin_api-1.2/MANIFEST.in
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     2958 2024-05-01 20:42:05.371209 robin_api-1.2/PKG-INFO
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     2511 2024-05-01 20:03:11.000000 robin_api-1.2/README.md
-drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-01 20:42:05.371209 robin_api-1.2/robin_api/
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      765 2024-05-01 02:52:51.000000 robin_api-1.2/robin_api/__init__.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     6473 2024-05-01 04:43:31.000000 robin_api-1.2/robin_api/_client.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     5102 2024-04-30 23:37:44.000000 robin_api-1.2/robin_api/_compat.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      404 2024-04-30 23:05:14.000000 robin_api-1.2/robin_api/_constants.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     3573 2024-04-30 20:26:30.000000 robin_api-1.2/robin_api/_exceptions.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    18240 2024-05-01 18:18:56.000000 robin_api-1.2/robin_api/_models.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      881 2024-05-01 04:56:26.000000 robin_api-1.2/robin_api/_resource.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     7217 2024-04-30 23:44:46.000000 robin_api-1.2/robin_api/_streaming.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     9696 2024-04-30 23:36:19.000000 robin_api-1.2/robin_api/_types.py
-drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-01 20:42:05.371209 robin_api-1.2/robin_api/_utils/
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      219 2024-05-01 02:38:52.000000 robin_api-1.2/robin_api/_utils/__init__.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     1553 2024-05-01 02:38:37.000000 robin_api-1.2/robin_api/_utils/_utils.py
-drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-01 20:42:05.371209 robin_api-1.2/robin_api/resources/
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      139 2024-05-01 00:03:13.000000 robin_api-1.2/robin_api/resources/__init__.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     3830 2024-05-01 20:13:11.000000 robin_api-1.2/robin_api/resources/completions.py
-drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-01 20:42:05.371209 robin_api-1.2/robin_api/types/
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      692 2024-05-01 17:26:33.000000 robin_api-1.2/robin_api/types/__init__.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     3781 2024-05-01 18:04:25.000000 robin_api-1.2/robin_api/types/chat_completion_chunk.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     1139 2024-05-01 16:49:41.000000 robin_api-1.2/robin_api/types/completion.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      928 2024-05-01 17:15:49.000000 robin_api-1.2/robin_api/types/completion_choice.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      401 2024-05-01 00:30:19.000000 robin_api-1.2/robin_api/types/completion_usage.py
-drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-01 20:42:05.371209 robin_api-1.2/robin_api.egg-info/
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      534 2024-05-01 20:42:05.000000 robin_api-1.2/robin_api.egg-info/SOURCES.txt
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)       38 2024-05-01 20:42:05.371209 robin_api-1.2/setup.cfg
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      725 2024-05-01 20:41:52.000000 robin_api-1.2/setup.py
+drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-07 04:34:06.602977 robin_api-1.3/
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    11337 2024-04-30 18:06:24.000000 robin_api-1.3/LICENSE
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      210 2024-05-01 19:41:22.000000 robin_api-1.3/MANIFEST.in
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    15167 2024-05-07 04:34:06.602977 robin_api-1.3/PKG-INFO
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    14720 2024-05-07 04:31:29.000000 robin_api-1.3/README.md
+drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-07 04:34:06.602977 robin_api-1.3/robin_api/
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      765 2024-05-02 19:33:54.000000 robin_api-1.3/robin_api/__init__.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    12382 2024-05-07 02:08:18.000000 robin_api-1.3/robin_api/_client.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     5102 2024-04-30 23:37:44.000000 robin_api-1.3/robin_api/_compat.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      404 2024-04-30 23:05:14.000000 robin_api-1.3/robin_api/_constants.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     3573 2024-04-30 20:26:30.000000 robin_api-1.3/robin_api/_exceptions.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    18240 2024-05-01 18:18:56.000000 robin_api-1.3/robin_api/_models.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      951 2024-05-02 19:39:40.000000 robin_api-1.3/robin_api/_resource.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     7217 2024-04-30 23:44:46.000000 robin_api-1.3/robin_api/_streaming.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     9696 2024-04-30 23:36:19.000000 robin_api-1.3/robin_api/_types.py
+drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-07 04:34:06.602977 robin_api-1.3/robin_api/_utils/
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      219 2024-05-01 02:38:52.000000 robin_api-1.3/robin_api/_utils/__init__.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     1553 2024-05-01 02:38:37.000000 robin_api-1.3/robin_api/_utils/_utils.py
+drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-07 04:34:06.602977 robin_api-1.3/robin_api/resources/
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      164 2024-05-06 00:49:45.000000 robin_api-1.3/robin_api/resources/__init__.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     5050 2024-05-07 03:00:16.000000 robin_api-1.3/robin_api/resources/completions.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     4260 2024-05-07 03:59:52.000000 robin_api-1.3/robin_api/resources/files.py
+drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-07 04:34:06.602977 robin_api-1.3/robin_api/types/
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      853 2024-05-07 00:28:45.000000 robin_api-1.3/robin_api/types/__init__.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     2025 2024-05-06 00:21:01.000000 robin_api-1.3/robin_api/types/chat_completion.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     3783 2024-05-06 00:07:24.000000 robin_api-1.3/robin_api/types/chat_completion_chunk.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     1241 2024-05-03 21:04:08.000000 robin_api-1.3/robin_api/types/chat_completion_message.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      866 2024-05-03 21:04:32.000000 robin_api-1.3/robin_api/types/chat_completion_message_tool_call.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     1139 2024-05-01 16:49:41.000000 robin_api-1.3/robin_api/types/completion.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      928 2024-05-01 17:15:49.000000 robin_api-1.3/robin_api/types/completion_choice.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      401 2024-05-01 00:30:19.000000 robin_api-1.3/robin_api/types/completion_usage.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      285 2024-05-07 00:28:29.000000 robin_api-1.3/robin_api/types/models_robin.py
+drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-07 04:34:06.602977 robin_api-1.3/robin_api.egg-info/
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      726 2024-05-07 04:34:06.000000 robin_api-1.3/robin_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)       38 2024-05-07 04:34:06.602977 robin_api-1.3/setup.cfg
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      725 2024-05-07 04:33:51.000000 robin_api-1.3/setup.py
```

### Comparing `robin_api-1.2/LICENSE` & `robin_api-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `robin_api-1.2/robin_api/__init__.py` & `robin_api-1.3/robin_api/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.2/robin_api/_compat.py` & `robin_api-1.3/robin_api/_compat.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.2/robin_api/_exceptions.py` & `robin_api-1.3/robin_api/_exceptions.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.2/robin_api/_models.py` & `robin_api-1.3/robin_api/_models.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.2/robin_api/_resource.py` & `robin_api-1.3/robin_api/_resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 
 class SyncAPIResource:
     _client: RobinAIClient
 
     def __init__(self, client: RobinAIClient) -> None:
         self._client = client
+        self._stream = client.stream
+        self._post = client.post
 
     def _sleep(self, seconds: float) -> None:
         time.sleep(seconds)
 
 #TODO
 class AsyncAPIResource:
     _client: AsyncRobinAIClient
```

### Comparing `robin_api-1.2/robin_api/_streaming.py` & `robin_api-1.3/robin_api/_streaming.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.2/robin_api/_types.py` & `robin_api-1.3/robin_api/_types.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.2/robin_api/_utils/_utils.py` & `robin_api-1.3/robin_api/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.2/robin_api/types/chat_completion_chunk.py` & `robin_api-1.3/robin_api/types/chat_completion_chunk.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,7 +112,9 @@
 
     system_fingerprint: Optional[str] = None
     """
     This fingerprint represents the backend configuration that the model runs with.
     Can be used in conjunction with the `seed` request parameter to understand when
     backend changes have been made that might impact determinism.
     """
+
+
```

### Comparing `robin_api-1.2/robin_api/types/completion.py` & `robin_api-1.3/robin_api/types/completion.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.2/robin_api/types/completion_choice.py` & `robin_api-1.3/robin_api/types/completion_choice.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.2/robin_api.egg-info/SOURCES.txt` & `robin_api-1.3/robin_api.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -11,12 +11,17 @@
 robin_api/_resource.py
 robin_api/_streaming.py
 robin_api/_types.py
 robin_api/_utils/__init__.py
 robin_api/_utils/_utils.py
 robin_api/resources/__init__.py
 robin_api/resources/completions.py
+robin_api/resources/files.py
 robin_api/types/__init__.py
+robin_api/types/chat_completion.py
 robin_api/types/chat_completion_chunk.py
+robin_api/types/chat_completion_message.py
+robin_api/types/chat_completion_message_tool_call.py
 robin_api/types/completion.py
 robin_api/types/completion_choice.py
-robin_api/types/completion_usage.py
+robin_api/types/completion_usage.py
+robin_api/types/models_robin.py
```

### Comparing `robin_api-1.2/setup.py` & `robin_api-1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 #packages=find_packages()
 #packages=['robin_api'],
 setup(
     name='robin_api',
-    version='1.2',
+    version='1.3',
     packages=find_packages(),
     description="file",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
         'httpx',
         'pydantic',
```

