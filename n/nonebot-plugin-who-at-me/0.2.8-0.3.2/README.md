# Comparing `tmp/nonebot-plugin-who-at-me-0.2.8.tar.gz` & `tmp/nonebot-plugin-who-at-me-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-who-at-me-0.2.8.tar", max compression
+gzip compressed data, was "nonebot-plugin-who-at-me-0.3.2.tar", max compression
```

## Comparing `nonebot-plugin-who-at-me-0.2.8.tar` & `nonebot-plugin-who-at-me-0.3.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1063 2022-09-19 02:12:29.331868 nonebot-plugin-who-at-me-0.2.8/LICENSE
--rw-r--r--   0        0        0     1350 2022-09-19 02:12:29.331868 nonebot-plugin-who-at-me-0.2.8/README.md
--rw-r--r--   0        0        0     5544 2022-09-19 02:12:29.331868 nonebot-plugin-who-at-me-0.2.8/nonebot_plugin_who_at_me/__init__.py
--rw-r--r--   0        0        0      237 2022-09-19 02:12:29.331868 nonebot-plugin-who-at-me-0.2.8/nonebot_plugin_who_at_me/config.py
--rw-r--r--   0        0        0      394 2022-09-19 02:12:29.331868 nonebot-plugin-who-at-me-0.2.8/nonebot_plugin_who_at_me/data_source.py
--rw-r--r--   0        0        0      824 2022-09-19 02:12:29.331868 nonebot-plugin-who-at-me-0.2.8/nonebot_plugin_who_at_me/database.py
--rw-r--r--   0        0        0      301 2022-09-19 02:12:29.331868 nonebot-plugin-who-at-me-0.2.8/nonebot_plugin_who_at_me/rule.py
--rw-r--r--   0        0        0      467 2022-09-19 02:12:29.331868 nonebot-plugin-who-at-me-0.2.8/nonebot_plugin_who_at_me/utils.py
--rw-r--r--   0        0        0      721 2022-09-19 02:12:29.331868 nonebot-plugin-who-at-me-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 nonebot-plugin-who-at-me-0.2.8/setup.py
--rw-r--r--   0        0        0     2254 1970-01-01 00:00:00.000000 nonebot-plugin-who-at-me-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-07 09:00:57.113514 nonebot-plugin-who-at-me-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1350 2024-05-07 09:00:57.113514 nonebot-plugin-who-at-me-0.3.2/README.md
+-rw-r--r--   0        0        0     5902 2024-05-07 09:00:57.113514 nonebot-plugin-who-at-me-0.3.2/nonebot_plugin_who_at_me/__init__.py
+-rw-r--r--   0        0        0      237 2024-05-07 09:00:57.113514 nonebot-plugin-who-at-me-0.3.2/nonebot_plugin_who_at_me/config.py
+-rw-r--r--   0        0        0      711 2024-05-07 09:00:57.113514 nonebot-plugin-who-at-me-0.3.2/nonebot_plugin_who_at_me/data_source.py
+-rw-r--r--   0        0        0      824 2024-05-07 09:00:57.113514 nonebot-plugin-who-at-me-0.3.2/nonebot_plugin_who_at_me/database.py
+-rw-r--r--   0        0        0      323 2024-05-07 09:00:57.113514 nonebot-plugin-who-at-me-0.3.2/nonebot_plugin_who_at_me/rule.py
+-rw-r--r--   0        0        0      441 2024-05-07 09:00:57.113514 nonebot-plugin-who-at-me-0.3.2/nonebot_plugin_who_at_me/utils.py
+-rw-r--r--   0        0        0      664 2024-05-07 09:02:35.380434 nonebot-plugin-who-at-me-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2181 2024-05-07 09:02:40.027151 nonebot-plugin-who-at-me-0.3.2/setup.py
+-rw-r--r--   0        0        0     2262 2024-05-07 09:02:40.027354 nonebot-plugin-who-at-me-0.3.2/PKG-INFO
```

### Comparing `nonebot-plugin-who-at-me-0.2.8/LICENSE` & `nonebot-plugin-who-at-me-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-who-at-me-0.2.8/README.md` & `nonebot-plugin-who-at-me-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-who-at-me-0.2.8/nonebot_plugin_who_at_me/__init__.py` & `nonebot-plugin-who-at-me-0.3.2/nonebot_plugin_who_at_me/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 __plugin_meta__ = PluginMetadata(
     name="who_at_me",
     description="看看是谁又艾特了我",
     usage="直接发送 谁@我了？",
     extra={
         "author": "SEAFHMC <soku_ritsuki@outlook.com>",
-        "version": "0.2.7",
+        "version": "0.3.1",
     },
 )
 plugin_config = Config.parse_obj(get_driver().config)
 reminder_expire_time = (
     plugin_config.reminder_expire_time * 24 * 3600
     if plugin_config.reminder_expire_time
     else 3 * 24 * 3600
@@ -40,18 +40,22 @@
     message = Message()
     if event.reply:
         message.append(MessageSegment.reply(event.reply.message_id))
     for segment in event.message:
         if segment.type == "at":
             card = get_member_name(
                 await bot.get_group_member_info(
-                    group_id=event.group_id, user_id=segment.data["qq"]
+                    group_id=event.group_id, user_id=int(target_id)
                 )
             )
-            message.append(f"@{MessageSegment.text(card)}")
+            message.append(
+                f"@{MessageSegment.text(card)}"
+                if segment.data["qq"] != "all"
+                else "@全体成员"
+            )
             continue
         message.append(segment)
 
     MainTable.create(
         operator_id=event.user_id,
         operator_name=event.sender.card or event.sender.nickname,
         target_id=target_id,
@@ -61,18 +65,26 @@
         message_id=event.message_id,
     )
 
 
 @monitor.handle()
 async def _(bot: Bot, event: GroupMessageEvent, message=EventMessage()):
     if event.reply:
-        target_id = event.reply.sender.user_id
-        await create_record(bot=bot, event=event, target_id=target_id)
+        reply_qq = {segment.data["qq"] for segment in event.original_message["at"]}
+        for target_id in reply_qq:
+            await create_record(bot=bot, event=event, target_id=target_id)
         return
-    if member_at := extract_member_at(message=message):
+    member_at = [
+        target_id
+        for target_id in await extract_member_at(
+            event.group_id, message=message, bot=bot
+        )
+        if target_id != str(event.user_id)
+    ]
+    if member_at:
         for target_id in member_at:
             await create_record(bot=bot, event=event, target_id=target_id)
         return
 
 
 who_at_me = on_regex(r"谁.*(@|艾特|圈|[aA][tT])+.?我")
 
@@ -141,14 +153,14 @@
 async def handle_first_receive(matcher: Matcher, args: Message = CommandArg()):
     plain_text = args.extract_plain_text()
     if plain_text:
         matcher.set_arg("confirm", args)
 
 
 @clear_db_all.got("confirm", prompt="该操作将清楚数据库全部内容，是否继续？")
-async def _(YesNo: str = ArgPlainText("confirm")):
-    if YesNo in CHINESE_AGREE_WORD:
+async def _(yes_or_no: str = ArgPlainText("confirm")):
+    if yes_or_no in CHINESE_AGREE_WORD:
         MainTable.delete().where(MainTable.target_id).execute()
         await clear_db.finish("已清理全部数据库")
-    elif YesNo in CHINESE_DECLINE_WORD:
+    elif yes_or_no in CHINESE_DECLINE_WORD:
         await clear_db.finish("已取消操作")
     await clear_db.reject("不太明白你的意思呢")
```

### Comparing `nonebot-plugin-who-at-me-0.2.8/nonebot_plugin_who_at_me/database.py` & `nonebot-plugin-who-at-me-0.3.2/nonebot_plugin_who_at_me/database.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-who-at-me-0.2.8/pyproject.toml` & `nonebot-plugin-who-at-me-0.3.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 [tool.poetry]
 name = "nonebot-plugin-who-at-me"
-version = "0.2.8"
+version = "0.3.2"
 description = "Find who on earth has ated you"
 authors = ["SEAFHMC <soku_ritsuki@outlook.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/SEAFHMC/nonebot-plugin-who-at-me"
 repository = "https://github.com/SEAFHMC/nonebot-plugin-who-at-me"
 documentation = "https://github.com/SEAFHMC/nonebot-plugin-who-at-me/blob/main/README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nonebot2 = "^2.0.0-beta.4"
 nonebot-adapter-onebot = "^2.1.1"
 peewee = ">=3.14.4"
-Pillow = ">=8.3.1"
-
-[tool.poetry.group.dev.dependencies]
 black = "^22.8.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot-plugin-who-at-me-0.2.8/setup.py` & `nonebot-plugin-who-at-me-0.3.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 packages = \
 ['nonebot_plugin_who_at_me']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['Pillow>=8.3.1',
+['black>=22.8.0,<23.0.0',
  'nonebot-adapter-onebot>=2.1.1,<3.0.0',
  'nonebot2>=2.0.0-beta.4,<3.0.0',
  'peewee>=3.14.4']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-who-at-me',
-    'version': '0.2.8',
+    'version': '0.3.2',
     'description': 'Find who on earth has ated you',
     'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://s2.loli.net/2022/06/16/opBDE8Swad5rU3n.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot-plugin-who-at-me\n\n_✨ 看看是谁又在艾特我 ✨_\n</div>\n  \n # 说明\n 你是否遇到过这种情景：你点进一个99+的QQ群，发现有人艾特/回复过你，你满心期待地去查看，结果腾讯告诉你消息过多无法定义到上下文。现在你只需要部署一个机器人卧底即可找出到底是谁艾特了你。\n # 安装\n通过`pip`或`nb`安装；\n需要协议端支持转发合并消息。\n\n命令：\n```shell\npip install nonebot-plugin-who-at-me\n```\n```shell\nnb plugin install nonebot-plugin-who-at-me\n```\n# 配置\n记得配置SUPERUSERS\n```shell\nreminder_expire_time 合并转发消息记录的超时时间, 单位为天\n```\n# 使用\n<div align="center">\n\n（这里默认COMMAND_START为"/"）\n| 命令              | 描述              |\n| ------------------ | --------------- |\n|谁艾特我 | 查看到底是谁艾特了你       |\n|/clear_db     | 清理当前用户的消息记录 |\n|/clear_all     | 清理全部消息记录     |\n\n结果将以合并转发形式发送\n',
     'author': 'SEAFHMC',
     'author_email': 'soku_ritsuki@outlook.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
+    'maintainer': None,
+    'maintainer_email': None,
     'url': 'https://github.com/SEAFHMC/nonebot-plugin-who-at-me',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_who_at_me'] package_data = \ {'': ['*']} install_requires = \
-['Pillow>=8.3.1', 'nonebot-adapter-onebot>=2.1.1,<3.0.0', 'nonebot2>=2.0.0-
-beta.4,<3.0.0', 'peewee>=3.14.4'] setup_kwargs = { 'name': 'nonebot-plugin-who-
-at-me', 'version': '0.2.8', 'description': 'Find who on earth has ated you',
-'long_description': '
+['black>=22.8.0,<23.0.0', 'nonebot-adapter-onebot>=2.1.1,<3.0.0',
+'nonebot2>=2.0.0-beta.4,<3.0.0', 'peewee>=3.14.4'] setup_kwargs = { 'name':
+'nonebot-plugin-who-at-me', 'version': '0.3.2', 'description': 'Find who on
+earth has ated you', 'long_description': '
                            \n _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]\n
                                       \n
                               [NoneBotPluginText]
                                       \n
 \n\n
    \n\n# nonebot-plugin-who-at-me\n\n_â¨ ççæ¯è°åå¨è¾ç¹æ â¨_\n
 \n \n # è¯´æ\n
@@ -20,11 +20,11 @@
 éç½®\nè®°å¾éç½®SUPERUSERS\n```shell\nreminder_expire_time
 åå¹¶è½¬åæ¶æ¯è®°å½çè¶æ¶æ¶é´, åä½ä¸ºå¤©\n```\n# ä½¿ç¨\n
 \n\nï¼è¿éé»è®¤COMMAND_STARTä¸º"/"ï¼\n| å½ä»¤ | æè¿° |\n| -------------
 ----- | --------------- |\n|è°è¾ç¹æ | æ¥çå°åºæ¯è°è¾ç¹äºä½  |\n|/
          clear_db | æ¸çå½åç¨æ·çæ¶æ¯è®°å½ |\n|/clear_all |
     æ¸çå¨é¨æ¶æ¯è®°å½ |\n\nç»æå°ä»¥åå¹¶è½¬åå½¢å¼åé\n',
 'author': 'SEAFHMC', 'author_email': 'soku_ritsuki@outlook.com', 'maintainer':
-'None', 'maintainer_email': 'None', 'url': 'https://github.com/SEAFHMC/nonebot-
+  None, 'maintainer_email': None, 'url': 'https://github.com/SEAFHMC/nonebot-
     plugin-who-at-me', 'packages': packages, 'package_data': package_data,
 'install_requires': install_requires, 'python_requires': '>=3.8,<4.0', } setup
                                (**setup_kwargs)
```

### Comparing `nonebot-plugin-who-at-me-0.2.8/PKG-INFO` & `nonebot-plugin-who-at-me-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-who-at-me
-Version: 0.2.8
+Version: 0.3.2
 Summary: Find who on earth has ated you
 Home-page: https://github.com/SEAFHMC/nonebot-plugin-who-at-me
 License: MIT
 Author: SEAFHMC
 Author-email: soku_ritsuki@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: Pillow (>=8.3.1)
+Requires-Dist: black (>=22.8.0,<23.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.1,<3.0.0)
 Requires-Dist: nonebot2 (>=2.0.0-beta.4,<3.0.0)
 Requires-Dist: peewee (>=3.14.4)
 Project-URL: Documentation, https://github.com/SEAFHMC/nonebot-plugin-who-at-me/blob/main/README.md
 Project-URL: Repository, https://github.com/SEAFHMC/nonebot-plugin-who-at-me
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-who-at-me Version: 0.2.8 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-who-at-me Version: 0.3.2 Summary:
 Find who on earth has ated you Home-page: https://github.com/SEAFHMC/nonebot-
 plugin-who-at-me License: MIT Author: SEAFHMC Author-email:
 soku_ritsuki@outlook.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: Pillow (>=8.3.1) Requires-Dist: nonebot-adapter-onebot
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: black (>=22.8.0,<23.0.0) Requires-Dist: nonebot-adapter-onebot
 (>=2.1.1,<3.0.0) Requires-Dist: nonebot2 (>=2.0.0-beta.4,<3.0.0) Requires-Dist:
 peewee (>=3.14.4) Project-URL: Documentation, https://github.com/SEAFHMC/
 nonebot-plugin-who-at-me/blob/main/README.md Project-URL: Repository, https://
 github.com/SEAFHMC/nonebot-plugin-who-at-me Description-Content-Type: text/
 markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
```

