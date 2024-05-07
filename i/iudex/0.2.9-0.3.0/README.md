# Comparing `tmp/iudex-0.2.9.tar.gz` & `tmp/iudex-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iudex-0.2.9.tar", max compression
+gzip compressed data, was "iudex-0.3.0.tar", max compression
```

## Comparing `iudex-0.2.9.tar` & `iudex-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0    11357 2024-02-22 09:17:28.247197 iudex-0.2.9/LICENSE
--rw-r--r--   0        0        0     3717 2024-03-13 08:12:55.353436 iudex-0.2.9/README.md
--rw-r--r--   0        0        0       54 2024-02-22 09:17:28.247197 iudex-0.2.9/iudex/__init__.py
--rw-r--r--   0        0        0     7348 2024-03-18 06:54:50.870996 iudex-0.2.9/iudex/chat.py
--rw-r--r--   0        0        0     7141 2024-03-18 06:52:09.401008 iudex-0.2.9/iudex/client.py
--rw-r--r--   0        0        0     1653 2024-03-18 07:01:54.830966 iudex-0.2.9/iudex/functions.py
--rw-r--r--   0        0        0      236 2024-03-03 21:45:43.952527 iudex-0.2.9/iudex/resource.py
--rw-r--r--   0        0        0     4349 2024-03-18 06:42:51.051047 iudex-0.2.9/iudex/types/function.py
--rw-r--r--   0        0        0      137 2024-03-13 08:12:55.353436 iudex-0.2.9/iudex/utils.py
--rw-r--r--   0        0        0      392 2024-03-18 05:05:50.941459 iudex-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     4215 1970-01-01 00:00:00.000000 iudex-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-05 02:32:42.683184 iudex-0.3.0/LICENSE
+-rw-r--r--   0        0        0     8426 2024-05-07 17:48:23.958486 iudex-0.3.0/README.md
+-rw-r--r--   0        0        0       54 2024-03-05 02:32:42.685374 iudex-0.3.0/iudex/__init__.py
+-rw-r--r--   0        0        0     7348 2024-03-22 23:11:09.655241 iudex-0.3.0/iudex/chat.py
+-rw-r--r--   0        0        0     7295 2024-03-22 23:11:09.655456 iudex-0.3.0/iudex/client.py
+-rw-r--r--   0        0        0     1653 2024-03-22 23:11:09.655988 iudex-0.3.0/iudex/functions.py
+-rw-r--r--   0        0        0     1951 2024-05-07 18:02:51.101258 iudex-0.3.0/iudex/instrumentation/README.md
+-rw-r--r--   0        0        0        0 2024-05-07 18:53:14.946672 iudex-0.3.0/iudex/instrumentation/__init__.py
+-rw-r--r--   0        0        0     1605 2024-05-07 18:50:00.465742 iudex-0.3.0/iudex/instrumentation/fastapi_instrumentation.py
+-rw-r--r--   0        0        0      236 2024-03-05 02:32:42.686766 iudex-0.3.0/iudex/resource.py
+-rw-r--r--   0        0        0     4349 2024-03-22 23:11:09.656442 iudex-0.3.0/iudex/types/function.py
+-rw-r--r--   0        0        0      137 2024-03-06 19:49:41.321305 iudex-0.3.0/iudex/utils.py
+-rw-r--r--   0        0        0      607 2024-05-07 18:10:07.156763 iudex-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9170 1970-01-01 00:00:00.000000 iudex-0.3.0/PKG-INFO
```

### Comparing `iudex-0.2.9/LICENSE` & `iudex-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iudex-0.2.9/iudex/chat.py` & `iudex-0.3.0/iudex/chat.py`

 * *Files identical despite different names*

### Comparing `iudex-0.2.9/iudex/client.py` & `iudex-0.3.0/iudex/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,15 @@
 
         # loop until no more tool calls
         while True:
             # get next message
             res = self.chat.completions.create(
                 messages=messages,
                 model=model,
+                functions=True,  # HACK: force function calling, we should instead factor out a helper consumed by this method and chat completion
             )
             next_msg = res.choices[0].message
             messages.append(next_msg)
 
             tool_calls = next_msg.tool_calls
 
             # no more tool calls, so return text content
@@ -198,10 +199,10 @@
 
     @property
     def _openai_client(self) -> OpenAI:
         """Deferred OpenAI client instantiation.
 
         Requires `OPENAI_API_KEY` to be set in the environment.
         """
-        if not hasattr(self, "_openai_client"):
+        if not hasattr(self, "_cached_openai_client"):
             self._cached_openai_client = OpenAI()
         return self._cached_openai_client
```

### Comparing `iudex-0.2.9/iudex/functions.py` & `iudex-0.3.0/iudex/functions.py`

 * *Files identical despite different names*

### Comparing `iudex-0.2.9/iudex/types/function.py` & `iudex-0.3.0/iudex/types/function.py`

 * *Files identical despite different names*

