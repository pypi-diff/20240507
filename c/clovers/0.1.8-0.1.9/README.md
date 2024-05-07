# Comparing `tmp/clovers-0.1.8.tar.gz` & `tmp/clovers-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clovers-0.1.8.tar", max compression
+gzip compressed data, was "clovers-0.1.9.tar", max compression
```

## Comparing `clovers-0.1.8.tar` & `clovers-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3417 2024-04-27 13:35:59.926811 clovers-0.1.8/clovers/__init__.py
--rw-r--r--   0        0        0     3250 2024-04-27 13:35:59.927312 clovers-0.1.8/clovers/core/adapter.py
--rw-r--r--   0        0        0      582 2024-04-27 13:35:59.927811 clovers-0.1.8/clovers/core/config.py
--rw-r--r--   0        0        0       57 2024-04-27 13:35:59.927811 clovers-0.1.8/clovers/core/logger.py
--rw-r--r--   0        0        0     6870 2024-04-27 14:18:55.214805 clovers-0.1.8/clovers/core/plugin.py
--rw-r--r--   0        0        0     2774 2024-04-27 13:35:59.928811 clovers-0.1.8/clovers/utils/library.py
--rw-r--r--   0        0        0    10961 2024-04-27 13:35:59.928811 clovers-0.1.8/clovers/utils/linecard.py
--rw-r--r--   0        0        0     1884 2024-04-27 13:35:59.929310 clovers-0.1.8/clovers/utils/tools.py
--rw-r--r--   0        0        0     1086 2024-04-27 13:35:59.926312 clovers-0.1.8/LICENSE
--rw-r--r--   0        0        0      645 2024-04-27 14:21:24.540341 clovers-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    10284 2024-04-27 13:35:59.926312 clovers-0.1.8/README.md
--rw-r--r--   0        0        0    10525 1970-01-01 00:00:00.000000 clovers-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     3417 2024-04-27 13:35:59.926811 clovers-0.1.9/clovers/__init__.py
+-rw-r--r--   0        0        0     3250 2024-04-27 13:35:59.927312 clovers-0.1.9/clovers/core/adapter.py
+-rw-r--r--   0        0        0      582 2024-04-27 13:35:59.927811 clovers-0.1.9/clovers/core/config.py
+-rw-r--r--   0        0        0       57 2024-04-27 13:35:59.927811 clovers-0.1.9/clovers/core/logger.py
+-rw-r--r--   0        0        0     7226 2024-05-01 07:53:17.032982 clovers-0.1.9/clovers/core/plugin.py
+-rw-r--r--   0        0        0     2774 2024-04-27 13:35:59.928811 clovers-0.1.9/clovers/utils/library.py
+-rw-r--r--   0        0        0    10961 2024-04-27 13:35:59.928811 clovers-0.1.9/clovers/utils/linecard.py
+-rw-r--r--   0        0        0     1884 2024-04-27 13:35:59.929310 clovers-0.1.9/clovers/utils/tools.py
+-rw-r--r--   0        0        0     1086 2024-04-27 13:35:59.926312 clovers-0.1.9/LICENSE
+-rw-r--r--   0        0        0      645 2024-05-01 07:56:04.736298 clovers-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    10284 2024-04-27 13:35:59.926312 clovers-0.1.9/README.md
+-rw-r--r--   0        0        0    10525 1970-01-01 00:00:00.000000 clovers-0.1.9/PKG-INFO
```

### Comparing `clovers-0.1.8/clovers/__init__.py` & `clovers-0.1.9/clovers/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.8/clovers/core/adapter.py` & `clovers-0.1.9/clovers/core/adapter.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.8/clovers/core/config.py` & `clovers-0.1.9/clovers/core/config.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.8/clovers/core/plugin.py` & `clovers-0.1.9/clovers/core/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         self.extra_args = extra_args
         self.get_extra_args = get_extra_args
 
     async def __call__(self, event: Event):
         return await self.func(event)
 
 
-PluginCommands = str | set[str] | re.Pattern | None
+PluginCommands = str | Iterable[str] | re.Pattern | None
 
 
 class Plugin:
     def __init__(
         self,
         name: str = "",
         build_event=None,
@@ -63,32 +63,33 @@
     def handle_warpper(self, func: Callable[..., Coroutine]):
         if build_event := self.build_event:
             middle_func = lambda e: func(build_event(e))
         else:
             middle_func = func
 
         if build_result := self.build_result:
+
             async def wrapper(event):
                 if result := await middle_func(event):
                     return build_result(result)
 
             return wrapper
         else:
             return middle_func
 
     def commands_register(self, commands: PluginCommands, key: int):
         if not commands:
             self.command_dict.setdefault("", set()).add(key)
-        elif isinstance(commands, set):
-            for command in commands:
-                self.command_dict.setdefault(command, set()).add(key)
         elif isinstance(commands, str):
             self.regex_dict.setdefault(re.compile(commands), set()).add(key)
         elif isinstance(commands, re.Pattern):
             self.regex_dict.setdefault(commands, set()).add(key)
+        elif isinstance(commands, Iterable):
+            for command in commands:
+                self.command_dict.setdefault(command, set()).add(key)
         else:
             raise PluginError(f"指令：{commands} 类型错误：{type(commands)}")
 
     def handle(
         self,
         commands: PluginCommands,
         extra_args: Iterable[str] = [],
@@ -99,28 +100,36 @@
             self.commands_register(commands, key)
             handle = Handle(extra_args, get_extra_args)
             handle.func = self.handle_warpper(func)
             self.handles[key] = handle
 
         return decorator
 
+    class Finish:
+        def __init__(self, plugin: "Plugin", key: str) -> None:
+            self.plugin = plugin
+            self.key = key
+
+        def __call__(self):
+            del self.plugin.temp_handles[self.key]
+
+        def delay(self, timeout: float | int = 30.0):
+            self.plugin.temp_handles[self.key] = (time.time() + timeout, self.plugin.temp_handles[self.key][1])
+
     def temp_handle(
         self,
         key: str,
         extra_args: Iterable[str] = [],
         get_extra_args: Iterable[str] = [],
         timeout: float | int = 30.0,
     ):
 
         def decorator(func: Callable[..., Coroutine]):
-            def finish():
-                del self.temp_handles[key]
-
             handle = Handle(extra_args, get_extra_args)
-            handle.func = self.handle_warpper(lambda e: func(e, finish))
+            handle.func = self.handle_warpper(lambda e: func(e, self.Finish(self, key)))
             self.temp_handles[key] = time.time() + timeout, handle
 
         return decorator
 
     def startup(self, func: Callable[[], Coroutine]):
         """注册一个启动任务"""
         self.startup_tasklist.append(func())
```

### Comparing `clovers-0.1.8/clovers/utils/library.py` & `clovers-0.1.9/clovers/utils/library.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.8/clovers/utils/linecard.py` & `clovers-0.1.9/clovers/utils/linecard.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.8/clovers/utils/tools.py` & `clovers-0.1.9/clovers/utils/tools.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.8/LICENSE` & `clovers-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `clovers-0.1.8/pyproject.toml` & `clovers-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clovers"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["KarisAya <1048827424@qq.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 toml = "^0.10.2"
```

### Comparing `clovers-0.1.8/README.md` & `clovers-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `clovers-0.1.8/PKG-INFO` & `clovers-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clovers
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: linecard
 Provides-Extra: tools
```

