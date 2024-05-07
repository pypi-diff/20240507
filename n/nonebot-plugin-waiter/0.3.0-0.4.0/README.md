# Comparing `tmp/nonebot_plugin_waiter-0.3.0.tar.gz` & `tmp/nonebot_plugin_waiter-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_waiter-0.3.0.tar", last modified: Sun Mar 24 06:50:30 2024, max compression
+gzip compressed data, was "nonebot_plugin_waiter-0.4.0.tar", last modified: Tue May  7 17:57:35 2024, max compression
```

## Comparing `nonebot_plugin_waiter-0.3.0.tar` & `nonebot_plugin_waiter-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3677 2024-03-24 06:31:05.795303 nonebot_plugin_waiter-0.3.0/README.md
--rw-r--r--   0        0        0     1369 2024-03-24 06:50:30.598271 nonebot_plugin_waiter-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6090 2024-03-24 06:49:42.338141 nonebot_plugin_waiter-0.3.0/src/nonebot_plugin_waiter/__init__.py
--rw-r--r--   0        0        0      177 2024-03-24 06:49:37.131645 nonebot_plugin_waiter-0.3.0/src/nonebot_plugin_waiter/config.py
--rw-r--r--   0        0        0     3811 1970-01-01 00:00:00.000000 nonebot_plugin_waiter-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3662 2024-05-07 17:56:39.365545 nonebot_plugin_waiter-0.4.0/README.md
+-rw-r--r--   0        0        0     1387 2024-05-07 17:57:35.778962 nonebot_plugin_waiter-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7070 2024-05-07 17:54:45.790434 nonebot_plugin_waiter-0.4.0/src/nonebot_plugin_waiter/__init__.py
+-rw-r--r--   0        0        0      177 2024-03-24 06:49:37.131645 nonebot_plugin_waiter-0.4.0/src/nonebot_plugin_waiter/config.py
+-rw-r--r--   0        0        0     3796 1970-01-01 00:00:00.000000 nonebot_plugin_waiter-0.4.0/PKG-INFO
```

### Comparing `nonebot_plugin_waiter-0.3.0/README.md` & `nonebot_plugin_waiter-0.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 `waiter` 有如下参数：
 
 - waits: 等待的事件类型列表，可以是 `Event` 的类型或事件的 `get_type()` 返回值；
     如果 waits 为空则继承 `matcher` 参数的事件响应器类型
 - matcher: 所属的 `Matcher` 对象，如果不指定则使用当前上下文的 `Matcher`
 - parameterless: 非参数类型依赖列表
+- keep_session: 是否保持会话，即仅允许会话发起者响应
 
 ### 等待
 
 可直接用 `Waiter.wait` 等待函数返回结果：
 
 ```python
 resp = await check.wait(timeout=60, default=False)
@@ -54,31 +55,30 @@
 参数：
 
 - default: 超时时返回的默认值
 - timeout: 等待超时时间
 
 ## 示例
 
-等待用户输入数字，超时时间为 60 秒，此时 waits 接收所有消息事件。
+等待用户输入数字，超时时间为 60 秒，此时 waits 接收所有来自当前用户的消息事件。
 
 ```python
 from nonebot import on_command
 from nonebot.adapters import Event
 from nonebot_plugin_waiter import waiter
 
 test = on_command("test")
 
 @test.handle()
-async def _(event: Event):
+async def _():
     await test.send("请输入数字")
 
-    @waiter(waits=["message"])
-    async def check(event1: Event):
-        if event.get_session_id() == event1.get_session_id():
-            return event1.get_plaintext()
+    @waiter(waits=["message"], keep_session=True)
+    async def check(event: Event):
+        return event.get_plaintext()
 
     async for resp in check(timeout=60):
         if resp is None:
             await test.send("等待超时")
             break
         if not resp.isdigit():
             await test.send("请输入数字")
@@ -120,15 +120,15 @@
                 ],
             ]
         ),
     )
 
     @waiter(waits=[CallbackQueryEvent])
     async def check(event1: CallbackQueryEvent):
-        if event1.get_session_id() == event.get_session_id():
+        if ...:
             return event1.id, event1.message
 
     resp = await check.wait(timeout=30)
     if resp is None:
         await inline.finish("等待超时")
     _id, _message = resp
     if _message:
```

### Comparing `nonebot_plugin_waiter-0.3.0/pyproject.toml` & `nonebot_plugin_waiter-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "nonebot-plugin-waiter"
-version = "0.3.0"
+version = "0.4.0"
 description = "An alternative for got-and-reject in Nonebot"
 authors = [
     { name = "RF-Tar-Railt", email = "3165388245@qq.com" },
 ]
 dependencies = [
-    "nonebot2>=2.2.0",
+    "nonebot2>=2.3.0",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
@@ -24,35 +24,35 @@
 includes = [
     "src",
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort>=5.13.2",
-    "black>=23.12.1",
-    "ruff>=0.1.9",
-    "pre-commit>=3.6.0",
+    "black>=24.4.2",
+    "ruff>=0.4.3",
+    "pre-commit>=3.7.0",
     "nonebot-adapter-onebot>=2.4.3",
-    "nonebot2[fastapi]>=2.2.0",
+    "nonebot2[fastapi]>=2.3.0",
 ]
 
 [tool.pdm.scripts.format]
 composite = [
     "isort ./src/ ",
     "black ./src/ ",
     "ruff check ./src/",
 ]
 
 [tool.black]
 line-length = 110
 target-version = [
-    "py38",
     "py39",
     "py310",
     "py311",
+    "py312",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [tool.isort]
 profile = "black"
 line_length = 110
@@ -60,14 +60,18 @@
 skip_gitignore = true
 force_sort_within_sections = true
 extra_standard_library = [
     "typing_extensions",
 ]
 
 [tool.ruff]
+line-length = 110
+target-version = "py39"
+
+[tool.ruff.lint]
 select = [
     "E",
     "W",
     "F",
     "UP",
     "C",
     "T",
@@ -77,14 +81,12 @@
 ]
 ignore = [
     "C901",
     "T201",
     "E731",
     "E402",
 ]
-line-length = 110
-target-version = "py38"
 
 [tool.pyright]
 pythonVersion = "3.9"
 pythonPlatform = "All"
 typeCheckingMode = "basic"
```

### Comparing `nonebot_plugin_waiter-0.3.0/src/nonebot_plugin_waiter/__init__.py` & `nonebot_plugin_waiter-0.4.0/src/nonebot_plugin_waiter/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from __future__ import annotations
 
 import asyncio
 from typing_extensions import Self
-from typing import Any, Generic, TypeVar, Callable, Iterable, Awaitable, overload
+from collections.abc import Iterable, Awaitable
+from typing import Any, Generic, TypeVar, Callable, overload
 
 from nonebot.plugin.on import on
 from nonebot.matcher import Matcher
 from nonebot import get_plugin_config
 from nonebot.plugin import PluginMetadata
 from nonebot.dependencies import Dependent
 from nonebot.internal.adapter import Bot, Event
-from nonebot.internal.matcher import current_matcher
 from nonebot.typing import T_State, _DependentCallable
+from nonebot.internal.permission import User, Permission
+from nonebot.internal.matcher import current_event, current_matcher
 
 from .config import Config
 
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 
 __plugin_meta__ = PluginMetadata(
     name="Waiter 插件",
     description="提供一个 got-and-reject 会话控制的替代方案，可自由控制超时时间",
-    usage="unimsg: UniMsg",
+    usage="@waiter(waits: list[type[Event] | str], matcher: type[Matcher] | Matcher, parameterless: Iterable[Any] | None, keep_session: bool = False)",  # noqa: E501
     homepage="https://github.com/RF-Tar-Railt/nonebot-plugin-waiter",
     type="library",
     config=Config,
     supported_adapters=None,
     extra={
         "author": "RF-Tar-Railt",
         "priority": 1,
@@ -46,20 +48,18 @@
         self.timeout = timeout
         self.default = default
 
     def __aiter__(self) -> Self:
         return self
 
     @overload
-    def __anext__(self: WaiterIterator[R1, None]) -> Awaitable[R1 | None]:
-        ...
+    def __anext__(self: WaiterIterator[R1, None]) -> Awaitable[R1 | None]: ...
 
     @overload
-    def __anext__(self: WaiterIterator[R1, T1]) -> Awaitable[R1 | T1]:
-        ...
+    def __anext__(self: WaiterIterator[R1, T1]) -> Awaitable[R1 | T1]: ...
 
     def __anext__(self):  # type: ignore
         return self.waiter.wait(default=self.default, timeout=self.timeout)  # type: ignore
 
 
 class Waiter(Generic[R]):
     future: asyncio.Future
@@ -67,21 +67,24 @@
 
     def __init__(
         self,
         waits: list[type[Event] | str],
         handler: _DependentCallable[R],
         matcher: type[Matcher] | Matcher,
         parameterless: Iterable[Any] | None = None,
+        permission: Permission | None = None,
     ):
         if waits:
             event_types = tuple([e for e in waits if not isinstance(e, str)])
             event_str_types = tuple([e for e in waits if isinstance(e, str)])
+            self.event_type = event_str_types[0] if len(event_str_types) == 1 else ""
         else:
             event_types = ()
             event_str_types = (matcher.type,)
+            self.event_type = matcher.type
         self.future = asyncio.Future()
         _handler = Dependent[Any].parse(
             call=handler, parameterless=parameterless, allow_types=matcher.HANDLER_PARAM_TYPES
         )
 
         async def wrapper(matcher: Matcher, bot: Bot, event: Event, state: T_State):
             if event_types and not isinstance(event, event_types):
@@ -98,56 +101,56 @@
             )
             if result is not None and not self.future.done():
                 self.future.set_result(result)
                 matcher.stop_propagation()
                 await matcher.finish()
             matcher.skip()
 
+        wrapper.__annotations__ = {"matcher": Matcher, "bot": Bot, "event": Event, "state": T_State}
         self.handler = wrapper
+        self.permission = permission
 
     def __aiter__(self) -> WaiterIterator[R, None]:
         return WaiterIterator(self, None)
 
     @overload
-    def __call__(self, *, default: T, timeout: float = 120) -> WaiterIterator[R, T]:
-        ...
+    def __call__(self, *, default: T, timeout: float = 120) -> WaiterIterator[R, T]: ...
 
     @overload
-    def __call__(self, *, timeout: float = 120) -> WaiterIterator[R, None]:
-        ...
+    def __call__(self, *, timeout: float = 120) -> WaiterIterator[R, None]: ...
 
     def __call__(
         self, *, default: T | None = None, timeout: float = plugin_config.waiter_timeout
     ) -> WaiterIterator[R, T] | WaiterIterator[R, None]:
         """等待用户输入并返回结果
 
         参数:
             default: 超时时返回的默认值
             timeout: 等待超时时间
         """
         return WaiterIterator(self, default, timeout)  # type: ignore
 
     @overload
-    async def wait(self, *, default: R | T, timeout: float = plugin_config.waiter_timeout) -> R | T:
-        ...
+    async def wait(self, *, default: R | T, timeout: float = plugin_config.waiter_timeout) -> R | T: ...
 
     @overload
-    async def wait(self, *, timeout: float = plugin_config.waiter_timeout) -> R | None:
-        ...
+    async def wait(self, *, timeout: float = plugin_config.waiter_timeout) -> R | None: ...
 
     async def wait(
         self, *, default: R | T | None = None, timeout: float = plugin_config.waiter_timeout
     ) -> R | T | None:
         """等待用户输入并返回结果
 
         参数:
             default: 超时时返回的默认值
             timeout: 等待超时时间
         """
-        matcher = on(priority=0, block=False, handlers=[self.handler])
+        matcher = on(
+            type=self.event_type, permission=self.permission, priority=0, block=False, handlers=[self.handler]
+        )
         try:
             return await asyncio.wait_for(self.future, timeout)
         except asyncio.TimeoutError:
             return default
         finally:
             self.future = asyncio.Future()
             try:
@@ -156,28 +159,40 @@
                 pass
 
 
 def waiter(
     waits: list[type[Event] | str],
     matcher: type[Matcher] | Matcher | None = None,
     parameterless: Iterable[Any] | None = None,
+    keep_session: bool = False,
 ) -> Callable[[_DependentCallable[R]], Waiter[R]]:
     """装饰一个函数来创建一个 `Waiter` 对象用以等待用户输入
 
     函数内需要自行判断输入是否符合预期并返回结果
 
-    参数:
+    Args:
         waits: 等待的事件类型列表，可以是 `Event` 的类型或事件的 `get_type()` 返回值；
                 如果为空则继承 `matcher` 参数的事件响应器类型
         matcher: 所属的 `Matcher` 对象，如果不指定则使用当前上下文的 `Matcher`
         parameterless: 非参数类型依赖列表
+        keep_session: 是否保持会话，即仅允许会话发起者响应
     """
     if not matcher:
         try:
             matcher = current_matcher.get()
         except LookupError:
             raise RuntimeError("No matcher found.")
 
+    if not keep_session:
+        permission = None
+    else:
+        try:
+            event = current_event.get()
+        except LookupError:
+            permission = None
+        else:
+            permission = Permission(User.from_event(event, perm=matcher.permission))
+
     def wrapper(func: _DependentCallable[R]):
-        return Waiter(waits, func, matcher, parameterless)
+        return Waiter(waits, func, matcher, parameterless, permission)
 
     return wrapper
```

### Comparing `nonebot_plugin_waiter-0.3.0/PKG-INFO` & `nonebot_plugin_waiter-0.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-waiter
-Version: 0.3.0
+Version: 0.4.0
 Summary: An alternative for got-and-reject in Nonebot
 Author-Email: RF-Tar-Railt <3165388245@qq.com>
 License: MIT
 Requires-Python: >=3.9
-Requires-Dist: nonebot2>=2.2.0
+Requires-Dist: nonebot2>=2.3.0
 Description-Content-Type: text/markdown
 
 # nonebot-plugin-waiter
 
 该插件提供一个 got-and-reject 会话控制的替代方案，可自由控制超时时间
 
 ## 安装
@@ -41,14 +41,15 @@
 
 `waiter` 有如下参数：
 
 - waits: 等待的事件类型列表，可以是 `Event` 的类型或事件的 `get_type()` 返回值；
     如果 waits 为空则继承 `matcher` 参数的事件响应器类型
 - matcher: 所属的 `Matcher` 对象，如果不指定则使用当前上下文的 `Matcher`
 - parameterless: 非参数类型依赖列表
+- keep_session: 是否保持会话，即仅允许会话发起者响应
 
 ### 等待
 
 可直接用 `Waiter.wait` 等待函数返回结果：
 
 ```python
 resp = await check.wait(timeout=60, default=False)
@@ -64,31 +65,30 @@
 参数：
 
 - default: 超时时返回的默认值
 - timeout: 等待超时时间
 
 ## 示例
 
-等待用户输入数字，超时时间为 60 秒，此时 waits 接收所有消息事件。
+等待用户输入数字，超时时间为 60 秒，此时 waits 接收所有来自当前用户的消息事件。
 
 ```python
 from nonebot import on_command
 from nonebot.adapters import Event
 from nonebot_plugin_waiter import waiter
 
 test = on_command("test")
 
 @test.handle()
-async def _(event: Event):
+async def _():
     await test.send("请输入数字")
 
-    @waiter(waits=["message"])
-    async def check(event1: Event):
-        if event.get_session_id() == event1.get_session_id():
-            return event1.get_plaintext()
+    @waiter(waits=["message"], keep_session=True)
+    async def check(event: Event):
+        return event.get_plaintext()
 
     async for resp in check(timeout=60):
         if resp is None:
             await test.send("等待超时")
             break
         if not resp.isdigit():
             await test.send("请输入数字")
@@ -130,15 +130,15 @@
                 ],
             ]
         ),
     )
 
     @waiter(waits=[CallbackQueryEvent])
     async def check(event1: CallbackQueryEvent):
-        if event1.get_session_id() == event.get_session_id():
+        if ...:
             return event1.id, event1.message
 
     resp = await check.wait(timeout=30)
     if resp is None:
         await inline.finish("等待超时")
     _id, _message = resp
     if _message:
```

