# Comparing `tmp/nonebot_plugin_clovers-0.1.4.tar.gz` & `tmp/nonebot_plugin_clovers-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_clovers-0.1.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_clovers-0.1.5.tar", max compression
```

## Comparing `nonebot_plugin_clovers-0.1.4.tar` & `nonebot_plugin_clovers-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1086 2024-04-15 11:49:16.312798 nonebot_plugin_clovers-0.1.4/LICENSE
--rw-r--r--   0        0        0     3317 2024-04-25 17:12:21.573796 nonebot_plugin_clovers-0.1.4/nonebot_plugin_clovers/__init__.py
--rw-r--r--   0        0        0      843 2024-04-25 15:59:33.461893 nonebot_plugin_clovers-0.1.4/nonebot_plugin_clovers/adapters/main.py
--rw-r--r--   0        0        0     4241 2024-04-25 16:04:21.704665 nonebot_plugin_clovers-0.1.4/nonebot_plugin_clovers/adapters/onebot/v11.py
--rw-r--r--   0        0        0     1724 2024-04-25 16:00:47.948721 nonebot_plugin_clovers-0.1.4/nonebot_plugin_clovers/adapters/qq.py
--rw-r--r--   0        0        0      365 2024-04-25 17:15:05.004223 nonebot_plugin_clovers-0.1.4/nonebot_plugin_clovers/config.py
--rw-r--r--   0        0        0      570 2024-04-25 16:56:39.551479 nonebot_plugin_clovers-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2514 2024-04-15 11:57:25.353441 nonebot_plugin_clovers-0.1.4/README.md
--rw-r--r--   0        0        0     3065 1970-01-01 00:00:00.000000 nonebot_plugin_clovers-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-04-26 17:06:21.977609 nonebot_plugin_clovers-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3875 2024-05-07 15:54:05.585074 nonebot_plugin_clovers-0.1.5/nonebot_plugin_clovers/__init__.py
+-rw-r--r--   0        0        0      843 2024-04-26 17:06:21.979035 nonebot_plugin_clovers-0.1.5/nonebot_plugin_clovers/adapters/main.py
+-rw-r--r--   0        0        0     4487 2024-05-07 15:05:19.259504 nonebot_plugin_clovers-0.1.5/nonebot_plugin_clovers/adapters/onebot/v11.py
+-rw-r--r--   0        0        0     4443 2024-05-07 15:55:07.140433 nonebot_plugin_clovers-0.1.5/nonebot_plugin_clovers/adapters/qq.py
+-rw-r--r--   0        0        0     3994 2024-05-07 15:51:43.286426 nonebot_plugin_clovers-0.1.5/nonebot_plugin_clovers/adapters/satori.py
+-rw-r--r--   0        0        0      401 2024-05-07 13:27:03.174097 nonebot_plugin_clovers-0.1.5/nonebot_plugin_clovers/config.py
+-rw-r--r--   0        0        0      754 2024-05-07 16:00:59.680793 nonebot_plugin_clovers-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2514 2024-04-26 17:06:21.978242 nonebot_plugin_clovers-0.1.5/README.md
+-rw-r--r--   0        0        0     3137 1970-01-01 00:00:00.000000 nonebot_plugin_clovers-0.1.5/PKG-INFO
```

### Comparing `nonebot_plugin_clovers-0.1.4/LICENSE` & `nonebot_plugin_clovers-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_clovers-0.1.4/nonebot_plugin_clovers/__init__.py` & `nonebot_plugin_clovers-0.1.5/nonebot_plugin_clovers/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import os
 from pathlib import Path
 from nonebot import get_driver, get_plugin_config, on_message
 from nonebot.matcher import Matcher
 from nonebot.plugin import PluginMetadata
 from nonebot.log import LoguruHandler, logger
+from nonebot.adapters import (
+    Bot as BaseBot,
+    Event as BaseEvent,
+)
+from collections.abc import Callable
 from clovers.core.logger import logger as clovers_logger
 from clovers.core.adapter import Adapter
 from clovers.core.plugin import PluginLoader
 from .adapters.main import extract_command, new_clovers
 from .config import Config, ConfigClovers
 
 __plugin_meta__ = PluginMetadata(
     name="clovers插件框架",
     description="NoneBot clovers框架",
     usage="加载即用",
     type="application",
     homepage="https://github.com/KarisAya/nonebot_plugin_clovers",
     config=Config,
-    supported_adapters={
-        "nonebot.adapters.qq",
-        "nonebot.adapters.onebot.v11",
-    },
 )
 driver = get_driver()
 # 配置日志记录器
 log_level = driver.config.log_level
 clovers_logger.setLevel(log_level)
 clovers_logger.addHandler(LoguruHandler(log_level))
 # 加载配置
@@ -39,59 +40,75 @@
 from clovers.core.config import config as clovers_config
 
 config_key = __package__
 clovers_config_data = ConfigClovers.model_validate(clovers_config.get(config_key, {}))
 clovers_config[config_key] = clovers_config_data.model_dump()
 clovers_config.save()
 
-
 plugins_path = Path(clovers_config_data.plugins_path)
 plugins_path.mkdir(exist_ok=True, parents=True)
-
-loader = PluginLoader(plugins_path, clovers_config_data.plugins_list)
-
-clovers = new_clovers(loader.plugins)
-
+clovers = new_clovers(PluginLoader(plugins_path, clovers_config_data.plugins_list).plugins)
 driver.on_startup(clovers.startup)
 
-main = on_message(priority=clovers_priority, block=False)
-
 
-def add_response(Bot, Event, adapter: Adapter, adapter_key: str):
-    logger.info(f"加载适配器：{adapter_key}")
+def add_response(
+    main: type[Matcher],
+    Bot: type[BaseBot],
+    Event: type[BaseEvent],
+    adapter: Adapter,
+    adapter_key: str,
+):
     clovers.adapter_dict[adapter_key] = adapter
 
     @main.handle()
     async def _(matcher: Matcher, bot: Bot, event: Event):
         command = extract_command(event.get_plaintext())
         if await clovers.response(adapter_key, command, bot=bot, event=event):
             matcher.stop_propagation()
 
 
-using_adapters = config_data.using_adapters
+using_adapters = __plugin_meta__.supported_adapters = config_data.using_adapters
 
+main = on_message(priority=clovers_priority, block=False)
+
+if "nonebot.adapters.onebot.v11" in using_adapters:
+    try:
+        from nonebot.adapters.onebot.v11 import Bot, MessageEvent
+        from .adapters.onebot import v11
+
+        logger.success("nonebot.adapters.onebot.v11 加载成功！")
+        flag = True
+    except ModuleNotFoundError:
+        logger.error("nonebot.adapters.onebot.v11 加载失败...")
+        flag = False
 
-flag_name = lambda flag: "成功！" if flag else "失败..."
+    if flag:
+        add_response(main, Bot, MessageEvent, v11.adapter(main), "onebot.v11".upper())
 
 if "nonebot.adapters.qq" in using_adapters:
-    flag = True
     try:
+        from nonebot.adapters.qq import Bot, MessageCreateEvent
         from .adapters import qq
-        from nonebot.adapters.qq import Bot, MessageEvent
+
+        logger.success("nonebot.adapters.qq 加载成功！")
+        flag = True
     except ModuleNotFoundError:
         logger.error("nonebot.adapters.qq 加载失败...")
         flag = False
+
     if flag:
-        add_response(Bot, MessageEvent, qq.initializer(main), "QQ")
-        logger.success("nonebot.adapters.qq 加载成功！")
+        add_response(main, Bot, MessageCreateEvent, qq.adapter(main), "QQ")
 
-if "nonebot.adapters.onebot.v11" in using_adapters:
-    flag = True
+if "nonebot.adapters.satori" in using_adapters:
     try:
-        from .adapters.onebot import v11
-        from nonebot.adapters.onebot.v11 import Bot, MessageEvent
+        from nonebot.adapters.satori import Bot
+        from nonebot.adapters.satori.event import MessageCreatedEvent
+        from .adapters import satori
+
+        logger.success("nonebot.adapters.satori 加载成功！")
+        flag = True
     except ModuleNotFoundError:
+        logger.error("nonebot.adapters.satori 加载失败...")
         flag = False
-        logger.error("nonebot.adapters.onebot.v11 加载失败...")
+
     if flag:
-        add_response(Bot, MessageEvent, v11.initializer(main), "onebot.v11".upper())
-        logger.success("nonebot.adapters.onebot.v11 加载成功！")
+        add_response(main, Bot, MessageCreatedEvent, satori.adapter(main), "satori".upper())
```

### Comparing `nonebot_plugin_clovers-0.1.4/nonebot_plugin_clovers/adapters/main.py` & `nonebot_plugin_clovers-0.1.5/nonebot_plugin_clovers/adapters/main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_clovers-0.1.4/nonebot_plugin_clovers/adapters/onebot/v11.py` & `nonebot_plugin_clovers-0.1.5/nonebot_plugin_clovers/adapters/onebot/v11.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,47 +11,60 @@
     Message,
     MessageSegment,
     GROUP_ADMIN,
     GROUP_OWNER,
 )
 
 
-def initializer(main: type[Matcher]) -> Adapter:
+def adapter(main: type[Matcher]) -> Adapter:
     adapter = Adapter()
 
     @adapter.send("text")
     async def _(message: str, send: Callable[..., Coroutine] = main.send):
         """发送纯文本"""
         await send(message)
 
     @adapter.send("image")
-    async def _(message: BytesIO, send: Callable[..., Coroutine] = main.send):
+    async def _(message: bytes | BytesIO | str, send: Callable[..., Coroutine] = main.send):
         """发送图片"""
         await send(MessageSegment.image(message))
 
+    @adapter.send("voice")
+    async def _(message: bytes | BytesIO | str, send: Callable[..., Coroutine] = main.send):
+        """发送音频消息"""
+        await send(MessageSegment.record(message))
+
     @adapter.send("list")
     async def _(message: list[Result], send: Callable[..., Coroutine] = main.send):
         """发送图片文本混合信息，@信息在此发送"""
         msg = Message()
         for seg in message:
             match seg.send_method:
                 case "text":
-                    msg += seg.data
+                    msg += MessageSegment.text(seg.data)
                 case "image":
                     msg += MessageSegment.image(seg.data)
                 case "at":
                     msg += MessageSegment.at(seg.data)
         await send(msg)
 
     @adapter.send("segmented")
     async def _(message: AsyncGenerator[Result, None], send: Callable[..., Coroutine] = main.send):
         """发送分段信息"""
         async for seg in message:
             await adapter.send_dict[seg.send_method](seg.data, send)
 
+    @adapter.kwarg("send_group_message")
+    async def _(bot: Bot) -> Callable[[str, Result], Coroutine]:
+        async def send_group_message(group_id: str, result: Result):
+            send = lambda message: bot.send_group_msg(group_id=int(group_id), message=message)
+            await adapter.send_dict[result.send_method](result.data, send)
+
+        return send_group_message
+
     @adapter.kwarg("user_id")
     async def _(event: MessageEvent):
         return event.get_user_id()
 
     @adapter.kwarg("group_id")
     async def _(event: MessageEvent):
         group_id = getattr(event, "group_id", None)
@@ -92,22 +105,14 @@
             return 1
         return 0
 
     @adapter.kwarg("at")
     async def _(event: MessageEvent) -> list[str]:
         return [str(msg.data["qq"]) for msg in event.message if msg.type == "at"]
 
-    @adapter.kwarg("send_group_message")
-    async def _(bot: Bot) -> Callable[[int, Result], Coroutine]:
-        async def send_group_message(group_id: int, result: Result):
-            send = lambda message: bot.send_group_msg(group_id=group_id, message=message)
-            await adapter.send_dict[result.send_method](result.data, send)
-
-        return send_group_message
-
     @adapter.kwarg("group_member_list")
     async def _(bot: Bot, event: MessageEvent) -> None | list[dict]:
         if not isinstance(event, GroupMessageEvent):
             return None
         info_list = await bot.get_group_member_list(group_id=event.group_id)
         for user_info in info_list:
             user_id = str(user_info["user_id"])
```

### Comparing `nonebot_plugin_clovers-0.1.4/README.md` & `nonebot_plugin_clovers-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_clovers-0.1.4/PKG-INFO` & `nonebot_plugin_clovers-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-clovers
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: all
 Provides-Extra: onebot
 Provides-Extra: qq
+Provides-Extra: satori
 Requires-Dist: clovers (>=0.1.5,<0.2.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.4.3,<3.0.0) ; extra == "onebot"
-Requires-Dist: nonebot-adapter-qq (>=1.4.3,<2.0.0) ; extra == "qq"
+Requires-Dist: nonebot-adapter-onebot (>=2.4.3,<3.0.0) ; extra == "onebot" or extra == "all"
+Requires-Dist: nonebot-adapter-qq (>=1.4.3,<2.0.0) ; extra == "qq" or extra == "all"
+Requires-Dist: nonebot-adapter-satori (>=0.11.5,<0.12.0) ; extra == "satori" or extra == "all"
 Requires-Dist: nonebot2 (>=2.2.1,<3.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-clovers Version: 0.1.4 Summary:
-Author: KarisAya Author-email: 1048827424@qq.com Requires-Python: >=3.10,<4.0
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: onebot Provides-Extra: qq Requires-Dist: clovers
+Metadata-Version: 2.1 Name: nonebot-plugin-clovers Version: 0.1.5 Summary:
+Author: KarisAya Author-email: 1048827424@qq.com Requires-Python: >=3.12,<4.0
+Classifier: Programming Language :: Python :: 3 Provides-Extra: all Provides-
+Extra: onebot Provides-Extra: qq Provides-Extra: satori Requires-Dist: clovers
 (>=0.1.5,<0.2.0) Requires-Dist: nonebot-adapter-onebot (>=2.4.3,<3.0.0) ; extra
-== "onebot" Requires-Dist: nonebot-adapter-qq (>=1.4.3,<2.0.0) ; extra == "qq"
+== "onebot" or extra == "all" Requires-Dist: nonebot-adapter-qq
+(>=1.4.3,<2.0.0) ; extra == "qq" or extra == "all" Requires-Dist: nonebot-
+adapter-satori (>=0.11.5,<0.12.0) ; extra == "satori" or extra == "all"
 Requires-Dist: nonebot2 (>=2.2.1,<3.0.0) Requires-Dist: pydantic
 (>=2.7.1,<3.0.0) Description-Content-Type: text/markdown
                                    _[_n_o_n_e_b_o_t_]
         # nonebot_plugin_clovers[python]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
 ## ð¿ å®è£ æ¨èä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb
 plugin install nonebot_plugin_clovers ``` ä½¿ç¨åç®¡çå¨å®è£ pip ```bash
```

