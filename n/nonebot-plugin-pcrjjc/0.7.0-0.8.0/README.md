# Comparing `tmp/nonebot_plugin_pcrjjc-0.7.0.tar.gz` & `tmp/nonebot_plugin_pcrjjc-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_pcrjjc-0.7.0.tar", last modified: Tue Apr 30 23:50:06 2024, max compression
+gzip compressed data, was "nonebot_plugin_pcrjjc-0.8.0.tar", last modified: Tue May  7 10:34:30 2024, max compression
```

## Comparing `nonebot_plugin_pcrjjc-0.7.0.tar` & `nonebot_plugin_pcrjjc-0.8.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:50:06.215087 nonebot_plugin_pcrjjc-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34510 2024-04-30 23:49:53.000000 nonebot_plugin_pcrjjc-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-30 23:50:06.215087 nonebot_plugin_pcrjjc-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-30 23:49:53.000000 nonebot_plugin_pcrjjc-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-30 23:49:53.000000 nonebot_plugin_pcrjjc-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 23:50:06.215087 nonebot_plugin_pcrjjc-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:50:06.215087 nonebot_plugin_pcrjjc-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:50:06.215087 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/
--rw-r--r--   0 runner    (1001) docker     (127)    40026 2024-04-30 23:49:53.000000 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-30 23:49:53.000000 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/aiorequests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-04-30 23:49:53.000000 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/bsgamesdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-30 23:49:53.000000 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-04-30 23:49:53.000000 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/pcrclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-04-30 23:49:53.000000 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-30 23:49:53.000000 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/rsacr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-30 23:49:53.000000 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/text2img.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:50:06.215087 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-30 23:50:06.000000 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-30 23:50:06.000000 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 23:50:06.000000 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 23:50:06.000000 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 23:50:06.000000 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:34:30.586241 nonebot_plugin_pcrjjc-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34510 2024-05-07 10:34:24.000000 nonebot_plugin_pcrjjc-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-07 10:34:30.586241 nonebot_plugin_pcrjjc-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-07 10:34:24.000000 nonebot_plugin_pcrjjc-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-07 10:34:24.000000 nonebot_plugin_pcrjjc-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 10:34:30.586241 nonebot_plugin_pcrjjc-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:34:30.582241 nonebot_plugin_pcrjjc-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:34:30.582241 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 10:34:24.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-07 10:34:24.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/aiorequests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-05-07 10:34:24.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/bsgamesdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-07 10:34:24.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41895 2024-05-07 10:34:24.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-05-07 10:34:24.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/pcrclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-05-07 10:34:24.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-07 10:34:24.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/rsacr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-07 10:34:24.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/text2img.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:34:30.586241 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-07 10:34:30.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-07 10:34:30.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 10:34:30.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-07 10:34:30.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 10:34:30.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc.egg-info/top_level.txt
```

### Comparing `nonebot_plugin_pcrjjc-0.7.0/LICENSE` & `nonebot_plugin_pcrjjc-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pcrjjc-0.7.0/PKG-INFO` & `nonebot_plugin_pcrjjc-0.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pcrjjc
-Version: 0.7.0
+Version: 0.8.0
 Summary: pcrjjc排名监测插件
 Author-email: reine-ishyanami <2402979195@qq.com>
 License: AGPL-3
 Project-URL: Homepage, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc
 Project-URL: Bug Tracker, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc/issues
 Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -15,15 +15,15 @@
 Classifier: Natural Language :: Chinese (Simplified)
 Requires-Python: <4.0,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: msgpack>=1.0.5
 Requires-Dist: requests>=2.30.0
 Requires-Dist: Pillow>=9.5.0
-Requires-Dist: pydantic>=2
+Requires-Dist: pydantic>=1.10.14
 Requires-Dist: python-dateutil>=2.8.2
 Requires-Dist: pycryptodome>=3.18.0
 Requires-Dist: nonebot2>=2.0.0
 Requires-Dist: nonebot-adapter-onebot>=2.2.3
 Requires-Dist: nonebot-plugin-apscheduler>=0.3.0
 
 # nonebot-plugin-pcrjjc
```

### Comparing `nonebot_plugin_pcrjjc-0.7.0/README.md` & `nonebot_plugin_pcrjjc-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pcrjjc-0.7.0/pyproject.toml` & `nonebot_plugin_pcrjjc-0.8.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [project]
 name = "nonebot-plugin-pcrjjc"
-version = "0.7.0"
+version = "0.8.0"
 authors = [
     {name="reine-ishyanami", email="2402979195@qq.com"}
 ]
 description = "pcrjjc排名监测插件"
 readme = "README.md"
 license = { text = "AGPL-3" }
 requires-python = ">=3.10, <4.0"
 dependencies = [
     "msgpack>=1.0.5",
     "requests>=2.30.0",
     "Pillow>=9.5.0",
-    "pydantic>=2",
+    "pydantic>=1.10.14",
     "python-dateutil>=2.8.2",
     "pycryptodome>=3.18.0",
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.2.3",
     "nonebot-plugin-apscheduler>=0.3.0"
 ]
 classifiers = [
```

### Comparing `nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/__init__.py` & `nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,58 +8,58 @@
     get_bot,
     get_driver,
     on_fullmatch,
     get_bots,
     logger,
     on_regex,
     require,
-    on_notice
+    on_notice,
 )
 from nonebot.adapters.onebot.v11 import (
     Bot,
     MessageEvent,
     MessageSegment,
     GroupMessageEvent,
     Message,
     PrivateMessageEvent,
     FriendAddNoticeEvent,
-    GroupDecreaseNoticeEvent
+    GroupDecreaseNoticeEvent,
 )
 from nonebot.internal.matcher import Matcher
 from nonebot.params import RegexGroup
 from nonebot.permission import SUPERUSER
 from nonebot.plugin import PluginMetadata
 
 from .config import config, Config
 from .query import queue, path
 from .text2img import image_draw
 
 require("nonebot_plugin_apscheduler")
 
-from nonebot_plugin_apscheduler import scheduler  
+from nonebot_plugin_apscheduler import scheduler  # noqa: E402
 
 __plugin_meta__ = PluginMetadata(
     name="pcrjjc",
     config=Config,
     description="公主连结（国服）排名监测工具",
     usage="发送 竞技场帮助 获取详细使用说明",
     type="application",
     homepage="https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc",
-    supported_adapters={"~onebot.v11"}
+    supported_adapters={"~onebot.v11"},
 )
 
 driver = get_driver()
 
 MAX_PRI = config.max_pri
 MAX_PCRID = config.max_pcrid
 MAX_HISTORY = config.max_history
 NOTICE_CD_MIN = config.notice_cd_min
 REFRESH_SECOND = config.refresh_second
 
-sv_help = f'''\t\t\t\t【竞技场帮助】
+sv_help = f"""\t\t\t\t【竞技场帮助】
 可以添加的订阅：[jjc][pjjc][排名上升][at][上线提醒]
 #排名上升提醒对jjc和pjjc同时生效
 #每个QQ号至多添加{MAX_PCRID}个uid的订阅
 #默认开启jjc、pjjc、at，关闭排名上升、上线提醒
 #手动查询时，返回昵称、jjc/pjjc排名、场次、
 jjc/pjjc当天排名上升次数、最后登录时间。
 #支持群聊使用。只允许群聊使用！！！
@@ -82,207 +82,246 @@
 #5个数字依次代表jjc、pjjc、排名上升、at、上线提醒
 #例如：“竞技场设置10111 2” “竞技场设置11110 0”
 #上线提醒：第5位表示上线提醒等级，可以写0~3
 0表示关闭，1表示{NOTICE_CD_MIN}分钟cd，仅在2点半~3点报，
 2表示{NOTICE_CD_MIN}分钟cd，全天报；3表示1分钟cd全天报。
 每天5点会把上线提醒等级3改成2，有需要的可以再次手动开启。
 12）在本群推送（限群聊发送，无需好友）
-'''
-sv_help_adm = '''------------------------------------------------
+"""
+sv_help_adm = """------------------------------------------------
 管理员帮助：
 1）pcrjjc负载查询
 2）pcrjjc删除绑定[qq号]
 3）pcrjjc关闭私聊推送
 4）pcrjjc关闭排名上升
-'''
+"""
 
 # 数据库对象初始化
 # JJCH = JJCHistoryStorage()
 friend_list = []
 pcrid_list = []
 admin = int(config.superusers[0]) if len(config.superusers) > 0 else 0
-config = join(path, 'binds.json')
-root = {'arena_bind': {}}
+config = join(path, "binds.json")
+root = {"arena_bind": {}}
 if exists(config):
     with open(config) as fp:
         root = load(fp)
 lck = Lock()
 lck_friend_list = Lock()
-bind_cache = root['arena_bind']
+bind_cache = root["arena_bind"]
 cache = {}
 jjc_log = {}
 query_cache = {}
 timeStamp = 0
 pri_user = 0
 today_notice = 0
 yesterday_notice = 0
 
 
-@on_fullmatch(msg='竞技场帮助').handle()
+@on_fullmatch(msg="竞技场帮助").handle()
 async def _(event: MessageEvent, matcher: Matcher):
     if event.user_id != admin:
         pic = image_draw(sv_help)
     else:
         pic = image_draw(sv_help + sv_help_adm)
     await matcher.finish(message=MessageSegment.image(pic))
 
 
-# ========================================查询========================================
+# ========================================Query========================================
 
-@on_fullmatch(msg='查询群数').handle()
+
+@on_fullmatch(msg="查询群数").handle()
 async def _(bot: Bot, event: GroupMessageEvent):
     global bind_cache, lck
     gid = event.group_id
     sid = bot.self_id
     async with lck:
         gl = await bot.get_group_list()
-        gl = [g['group_id'] for g in gl]
+        gl = [g["group_id"] for g in gl]
         try:
-            await bot.send_group_msg(group_id=gid, message=f"本Bot目前正在为【{len(gl)}】个群服务")
+            await bot.send_group_msg(
+                group_id=gid, message=f"本Bot目前正在为【{len(gl)}】个群服务"
+            )
         except Exception:
-            logger.info('bot账号{}不在群{}中，将忽略该消息', sid, gid)
+            logger.info("bot账号{}不在群{}中，将忽略该消息", sid, gid)
 
 
-@on_fullmatch(msg='查询竞技场订阅数').handle()
+@on_fullmatch(msg="查询竞技场订阅数").handle()
 async def _(matcher: Matcher):
     global bind_cache, lck
     async with lck:
-        await matcher.finish(f'当前竞技场已订阅的账号数量为【{len(bind_cache)}】个')
+        await matcher.finish(f"当前竞技场已订阅的账号数量为【{len(bind_cache)}】个")
 
 
-@on_regex(pattern=r'^竞技场查询 ?(\d+)?$').handle()
-async def _(bot: Bot, event: MessageEvent, matcher: Matcher, group: tuple = RegexGroup()):
+@on_regex(pattern=r"^竞技场查询 ?(\d+)?$").handle()
+async def _(
+    bot: Bot, event: MessageEvent, matcher: Matcher, group: tuple = RegexGroup()
+):
     global bind_cache, lck
     qid = str(event.user_id)
     try:
         pcrid = int(group[0])
         if (len(group[0])) != 13:
-            await matcher.finish('位数不对，uid是13位的！')
+            await matcher.finish("位数不对，uid是13位的！")
         else:
             manual_query_list = [pcrid]  # 手动查询的列表
             manual_query_list_name = [None]
     except TypeError:  # 只捕获强转异常
         if qid in bind_cache:
             manual_query_list = bind_cache[qid]["pcrid"]
             manual_query_list_name = bind_cache[qid]["pcrName"]
         else:
-            await matcher.finish('木有找到绑定信息，查询时不能省略13位uid！')
+            await matcher.finish("木有找到绑定信息，查询时不能省略13位uid！")
     logger.debug("manual_query_list: {}", manual_query_list)
     for i in range(len(manual_query_list)):
         query_cache[event.user_id] = []
         pcrid = manual_query_list[i]
-        await queue.put((3, (
-            jjc_query, pcrid, {"bot": bot, "event": event, "list": manual_query_list_name, "index": i, "uid": pcrid})))
-
-
-@on_regex(pattern=r'^竞技场查询\# ?(\d+)$').handle()
-async def _(bot: Bot, event: MessageEvent, matcher: Matcher, group: tuple = RegexGroup()):
+        await queue.put(
+            (
+                3,
+                (
+                    jjc_query,
+                    pcrid,
+                    {
+                        "bot": bot,
+                        "event": event,
+                        "list": manual_query_list_name,
+                        "index": i,
+                        "uid": pcrid,
+                    },
+                ),
+            )
+        )
+
+
+@on_regex(pattern=r"^竞技场查询\# ?(\d+)$").handle()
+async def _(
+    bot: Bot, event: MessageEvent, matcher: Matcher, group: tuple = RegexGroup()
+):
     global bind_cache, lck
     qid = str(event.user_id)
     lid = int(group[0])
     if qid in bind_cache:
         qid_pcrid_list = bind_cache[qid]["pcrid"]
         if 0 < lid <= len(qid_pcrid_list):
             manual_query_list = [bind_cache[qid]["pcrid"][lid - 1]]
             manual_query_list_name = [bind_cache[qid]["pcrName"][lid - 1]]
         else:
-            await matcher.finish('序号超出范围，请检查您绑定的竞技场列表')
+            await matcher.finish("序号超出范围，请检查您绑定的竞技场列表")
     else:
-        await matcher.finish('木有找到绑定信息，查询时不能省略13位uid！')
+        await matcher.finish("木有找到绑定信息，查询时不能省略13位uid！")
     logger.debug("manual_query_list: {}", manual_query_list)
     for i in range(len(manual_query_list)):
         query_cache[event.user_id] = []
         pcrid = manual_query_list[i]
-        await queue.put((3, (
-            jjc_query, pcrid,
-            {"bot": bot, "event": event, "list": manual_query_list_name, "index": i, "uid": pcrid, "only": lid - 1})))
+        await queue.put(
+            (
+                3,
+                (
+                    jjc_query,
+                    pcrid,
+                    {
+                        "bot": bot,
+                        "event": event,
+                        "list": manual_query_list_name,
+                        "index": i,
+                        "uid": pcrid,
+                        "only": lid - 1,
+                    },
+                ),
+            )
+        )
 
 
-@on_fullmatch(msg='竞技场订阅状态').handle()
+@on_fullmatch(msg="竞技场订阅状态").handle()
 async def _(bot: Bot, event: GroupMessageEvent, matcher: Matcher):
     global bind_cache
     qid = str(event.user_id)
     gid = event.group_id
     member_info = await bot.get_group_member_info(group_id=gid, user_id=int(qid))
     name = member_info["card"] or member_info["nickname"]
     if qid in bind_cache:
-        private = '私聊推送' if bind_cache[qid]["private"] else '群聊推送'
-        notice_on = '推送已开启' if bind_cache[qid]["notice_on"] else '推送未开启'
-        reply = f'{name}（{qid}）的竞技场订阅列表：\n\n'
+        private = "私聊推送" if bind_cache[qid]["private"] else "群聊推送"
+        notice_on = "推送已开启" if bind_cache[qid]["notice_on"] else "推送未开启"
+        reply = f"{name}（{qid}）的竞技场订阅列表：\n\n"
         reply += f'群号：{bind_cache[qid]["gid"]}\n'
-        reply += f'''推送方式：{private}\n状态：{notice_on}\n'''
+        reply += f"""推送方式：{private}\n状态：{notice_on}\n"""
         for pcrid_id in range(len(bind_cache[qid]["pcrid"])):
             reply += f'\n【{pcrid_id + 1:02}】{bind_cache[qid]["pcrName"][pcrid_id]}（{bind_cache[qid]["pcrid"][pcrid_id]}）\n'
             tmp = bind_cache[qid]["noticeType"][pcrid_id]
             atNotice, jjcNotice, pjjcNotice, riseNotice = await get_notice_type(tmp)
             onlineNotice = tmp % 10
-            noticeType = '推送内容：'
+            noticeType = "推送内容："
             if jjcNotice:
-                noticeType += 'jjc、'
+                noticeType += "jjc、"
             if pjjcNotice:
-                noticeType += 'pjjc、'
+                noticeType += "pjjc、"
             if riseNotice:
-                noticeType += '排名上升、'
+                noticeType += "排名上升、"
             if atNotice:
-                noticeType += '开启at、'
+                noticeType += "开启at、"
             if onlineNotice:
-                noticeType += '上线提醒LV' + str(onlineNotice) + '、'
-            if noticeType == '推送内容：':
-                noticeType += '无'
+                noticeType += "上线提醒LV" + str(onlineNotice) + "、"
+            if noticeType == "推送内容：":
+                noticeType += "无"
             else:
-                noticeType = noticeType.strip('、')
+                noticeType = noticeType.strip("、")
             reply += noticeType
-            reply += '\n'
-        reply += '\n###上线提醒LV越高，提醒越频繁。详情见竞技场帮助\n'
+            reply += "\n"
+        reply += "\n###上线提醒LV越高，提醒越频繁。详情见竞技场帮助\n"
         pic = image_draw(reply)
         await matcher.finish(MessageSegment.image(pic))
     else:
-        await matcher.finish('您还没有绑定竞技场！')
+        await matcher.finish("您还没有绑定竞技场！")
 
 
 async def get_notice_type(tmp):
     jjcNotice = True if tmp // 10000 else False
     pjjcNotice = True if (tmp % 10000) // 1000 else False
     riseNotice = True if (tmp % 1000) // 100 else False
     atNotice = True if (tmp % 100) // 10 else False
     return atNotice, jjcNotice, pjjcNotice, riseNotice
 
 
-@on_regex(r'^(?:击剑|竞技场)记录 ?(\d+)?$').handle()
-async def _(bot: Bot, event: GroupMessageEvent, matcher: Matcher, group: tuple = RegexGroup()):
+@on_regex(r"^(?:击剑|竞技场)记录 ?(\d+)?$").handle()
+async def _(
+    bot: Bot, event: GroupMessageEvent, matcher: Matcher, group: tuple = RegexGroup()
+):
     global jjc_log, bind_cache, MAX_HISTORY
     qid = str(event.user_id)
-    member_info = await bot.get_group_member_info(group_id=event.group_id, user_id=int(qid))
+    member_info = await bot.get_group_member_info(
+        group_id=event.group_id, user_id=int(qid)
+    )
     name = member_info["card"] or member_info["nickname"]
     print_all = False
     too_long = False
     if qid not in bind_cache:
-        await matcher.finish('您还没有绑定竞技场！')
-    pcrid_num = len(bind_cache[qid]['pcrid'])
+        await matcher.finish("您还没有绑定竞技场！")
+    pcrid_num = len(bind_cache[qid]["pcrid"])
     try:
         pcrid_id_input = int(group[0])
     except TypeError:
         if pcrid_num == 1:
             pcrid_id_input = 1
         else:
             print_all = True
     if not print_all:
         if pcrid_id_input == 0 or pcrid_id_input > pcrid_num:
-            await matcher.finish('序号超出范围，请检查您绑定的竞技场列表')
+            await matcher.finish("序号超出范围，请检查您绑定的竞技场列表")
     if print_all:
-        msg = f'''\t\t\t\t【{name}的击剑记录】\n'''
+        msg = f"""\t\t\t\t【{name}的击剑记录】\n"""
         jjc_log_cache = []
         len_pcrName = []
         for pcrid_id in range(pcrid_num):  # 复制相关的log，并排序
-            pcrid = bind_cache[qid]['pcrid'][pcrid_id]
-            pcrName = bind_cache[qid]['pcrName'][pcrid_id]
+            pcrid = bind_cache[qid]["pcrid"][pcrid_id]
+            pcrName = bind_cache[qid]["pcrName"][pcrid_id]
             if pcrid in jjc_log:  # 计算名字长度
                 width = 0
                 for c in pcrName:
-                    if len(c.encode('utf8')) == 3:  # 中文
+                    if len(c.encode("utf8")) == 3:  # 中文
                         width += 2
                     else:
                         width += 1
                 len_pcrName.append(width)
                 for log in jjc_log[pcrid]:
                     log_tmp = list(log)
                     log_tmp.append(pcrid_id)
@@ -299,383 +338,423 @@
                 too_long = True
                 jjc_log_cache_num = MAX_HISTORY
             for i in range(jjc_log_cache_num):
                 timeStamp = jjc_log_cache[i][0]
                 timeArray = time.localtime(timeStamp)
                 otherStyleTime = time.strftime("%Y-%m-%d %H:%M:%S", timeArray)
                 pcrid_id = jjc_log_cache[i][4]
-                pcrName = bind_cache[qid]['pcrName'][pcrid_id]
-                space = ' ' * len_pcrName[pcrid_id]
-                jjc_pjjc = 'jjc ' if jjc_log_cache[i][1] == 1 else 'pjjc'
+                pcrName = bind_cache[qid]["pcrName"][pcrid_id]
+                space = " " * len_pcrName[pcrid_id]
+                jjc_pjjc = "jjc " if jjc_log_cache[i][1] == 1 else "pjjc"
                 new = jjc_log_cache[i][2]
                 old = jjc_log_cache[i][3]
                 if new < old:
-                    change = f'''{old}->{new} [▲{old - new}]'''
+                    change = f"""{old}->{new} [▲{old - new}]"""
                 else:
-                    change = f'''{old}->{new} [▽{new - old}]'''
-                msg += f'''{otherStyleTime} {pcrName}{space} {jjc_pjjc}：{change}\n'''
+                    change = f"""{old}->{new} [▽{new - old}]"""
+                msg += f"""{otherStyleTime} {pcrName}{space} {jjc_pjjc}：{change}\n"""
             if too_long:
-                msg += '###由于您订阅了太多账号，记录显示不下嘞~\n###如有需要，可以在查询时加上序号。'
+                msg += "###由于您订阅了太多账号，记录显示不下嘞~\n###如有需要，可以在查询时加上序号。"
         else:
-            msg += '没有击剑记录！'
+            msg += "没有击剑记录！"
     else:
-        msg = f'''\t\t\t【{name}的击剑记录】\n'''
+        msg = f"""\t\t\t【{name}的击剑记录】\n"""
         pcrid_id = pcrid_id_input - 1
-        pcrid = bind_cache[qid]['pcrid'][pcrid_id]
-        pcrName = bind_cache[qid]['pcrName'][pcrid_id]
-        msg += f'''{pcrName}（{pcrid}）\n'''
+        pcrid = bind_cache[qid]["pcrid"][pcrid_id]
+        pcrName = bind_cache[qid]["pcrName"][pcrid_id]
+        msg += f"""{pcrName}（{pcrid}）\n"""
         if pcrid in jjc_log:
             jjc_log_num = len(jjc_log[pcrid])
             for i in range(jjc_log_num):
                 n = jjc_log_num - 1 - i  # 倒序输出，是最近的log在上面
                 timeStamp = jjc_log[pcrid][n][0]
                 timeArray = time.localtime(timeStamp)
                 otherStyleTime = time.strftime("%Y-%m-%d %H:%M:%S", timeArray)
-                jjc_pjjc = 'jjc' if jjc_log[pcrid][n][1] == 1 else 'pjjc'
+                jjc_pjjc = "jjc" if jjc_log[pcrid][n][1] == 1 else "pjjc"
                 new = jjc_log[pcrid][n][2]
                 old = jjc_log[pcrid][n][3]
                 if new < old:
-                    change = f'''{old}->{new} [▲{old - new}]'''
+                    change = f"""{old}->{new} [▲{old - new}]"""
                 else:
-                    change = f'''{old}->{new} [▽{new - old}]'''
-                msg += f'''{otherStyleTime} {jjc_pjjc}：{change}\n'''
+                    change = f"""{old}->{new} [▽{new - old}]"""
+                msg += f"""{otherStyleTime} {jjc_pjjc}：{change}\n"""
         else:
-            msg += '没有击剑记录！'
+            msg += "没有击剑记录！"
     pic = image_draw(msg)
     await matcher.finish(MessageSegment.image(pic))
 
 
-# ========================================竞技场绑定========================================
+# ========================================Bind========================================
 
-@on_regex(r'^竞技场绑定 ?(\d+) ?(\S+)?$').handle()
-async def _(bot: Bot, event: GroupMessageEvent, matcher: Matcher, group: tuple = RegexGroup()):
+
+@on_regex(r"^竞技场绑定 ?(\d+) ?(\S+)?$").handle()
+async def _(
+    bot: Bot, event: GroupMessageEvent, matcher: Matcher, group: tuple = RegexGroup()
+):
     global friend_list
     pcrid = int(group[0])
     if len(group[0]) != 13:
-        await matcher.finish('位数不对，uid是13位的！')
+        await matcher.finish("位数不对，uid是13位的！")
     else:
         try:  # 是否指定昵称
             if len(group[1]) <= 12:
                 nickname = group[1]
             else:
-                await matcher.finish('昵称不能超过12个字，换个短一点的昵称吧~')
+                await matcher.finish("昵称不能超过12个字，换个短一点的昵称吧~")
         except TypeError:
-            nickname = ''
-    await queue.put((4, (
-        member_add_sub, pcrid,
-        {"bot": bot, "event": event, 'nickname': nickname, 'uid': pcrid, 'friend_list': friend_list})))
+            nickname = ""
+    await queue.put(
+        (
+            4,
+            (
+                member_add_sub,
+                pcrid,
+                {
+                    "bot": bot,
+                    "event": event,
+                    "nickname": nickname,
+                    "uid": pcrid,
+                    "friend_list": friend_list,
+                },
+            ),
+        )
+    )
 
 
-@on_regex(pattern=r'^删除竞技场绑定 ?(\d+)?$').handle()
+@on_regex(pattern=r"^删除竞技场绑定 ?(\d+)?$").handle()
 async def _(event: GroupMessageEvent, matcher: Matcher, group: tuple = RegexGroup()):
     global bind_cache, lck
     qid = str(event.user_id)
     if group[0]:
         pcrid_id = int(group[0])
     else:
-        await matcher.finish('输入格式不对！“删除竞技场绑定+【序号】”（序号不可省略）')
+        await matcher.finish("输入格式不对！“删除竞技场绑定+【序号】”（序号不可省略）")
     async with lck:
         if qid in bind_cache:
             pcrid_num = len(bind_cache[qid]["pcrid"])
             if pcrid_num == 1:
-                await matcher.finish('您只有一个绑定的uid，请使用“清空竞技场绑定”删除')
+                await matcher.finish("您只有一个绑定的uid，请使用“清空竞技场绑定”删除")
             if 0 < pcrid_id <= pcrid_num:
                 pcrid_id -= 1
                 result = f'您已成功删除：【{pcrid_id + 1:02}】{bind_cache[qid]["pcrName"][pcrid_id]}（{bind_cache[qid]["pcrid"][pcrid_id]}）'
                 del bind_cache[qid]["pcrid"][pcrid_id]
                 del bind_cache[qid]["noticeType"][pcrid_id]
                 del bind_cache[qid]["pcrName"][pcrid_id]
                 save_binds()
                 await matcher.finish(result)
             else:
-                await matcher.finish('输入的序号超出范围！')
+                await matcher.finish("输入的序号超出范围！")
 
 
-@on_fullmatch(msg='清空竞技场绑定').handle()
+@on_fullmatch(msg="清空竞技场绑定").handle()
 async def _(event: GroupMessageEvent, matcher: Matcher):
     global bind_cache, lck
     qid = str(event.user_id)
     async with lck:
         if qid in bind_cache:
-            reply = '删除成功！\n'
+            reply = "删除成功！\n"
             for pcrid_id in range(len(bind_cache[qid]["pcrid"])):
-                reply += f'''【{pcrid_id + 1:02}】{bind_cache[qid]["pcrName"][pcrid_id]}\n（{bind_cache[qid]["pcrid"][pcrid_id]}）\n'''
+                reply += f"""【{pcrid_id + 1:02}】{bind_cache[qid]["pcrName"][pcrid_id]}\n（{bind_cache[qid]["pcrid"][pcrid_id]}）\n"""
             del bind_cache[qid]
         else:
-            reply = '您还没有绑定竞技场！'
+            reply = "您还没有绑定竞技场！"
             await matcher.finish(reply)
         save_binds()
     await matcher.finish(reply)
 
 
-# ========================================竞技场设置========================================
-@on_regex(pattern=r'^竞技场修改昵称 ?(\d+)? ?(\S+)$').handle()
+# ========================================Setting========================================
+@on_regex(pattern=r"^竞技场修改昵称 ?(\d+)? ?(\S+)$").handle()
 async def _(event: GroupMessageEvent, matcher: Matcher, group: tuple = RegexGroup()):
     global bind_cache, lck
     qid = str(event.user_id)
     if qid not in bind_cache:
-        reply = '您还没有绑定竞技场！'
+        reply = "您还没有绑定竞技场！"
         await matcher.finish(reply)
     try:
         pcrid_id = int(group[0])
     except TypeError:
         pcrid_id = None
     if len(group[1]) <= 12:
         name = group[1]
     else:
-        await matcher.finish('昵称不能超过12个字，换个短一点的昵称吧~')
+        await matcher.finish("昵称不能超过12个字，换个短一点的昵称吧~")
     pcrid_num = len(bind_cache[qid]["pcrid"])
     if pcrid_id is None:
         if pcrid_num == 1:
             pcrid_id = 1
         else:
-            await matcher.finish('您绑定了多个uid，更改昵称时需要加上序号。')
+            await matcher.finish("您绑定了多个uid，更改昵称时需要加上序号。")
     if pcrid_id == 0 or pcrid_id > pcrid_num:
-        await matcher.finish('序号超出范围，请检查您绑定的竞技场列表')
+        await matcher.finish("序号超出范围，请检查您绑定的竞技场列表")
     async with lck:
         pcrid_id -= 1
         bind_cache[qid]["pcrName"][pcrid_id] = name
         save_binds()
-    await matcher.finish('更改成功！')
+    await matcher.finish("更改成功！")
 
 
-@on_fullmatch(msg='在本群推送').handle()
+@on_fullmatch(msg="在本群推送").handle()
 async def _(event: GroupMessageEvent, matcher: Matcher):
     global bind_cache, lck
     qid = str(event.user_id)
     gid = event.group_id
     if qid in bind_cache:
         async with lck:
-            bind_cache[qid]['gid'] = gid
-            bind_cache[qid]['private'] = False
-            bind_cache[qid]['notice_on'] = True
-            reply = '设置成功！已为您开启推送。'
+            bind_cache[qid]["gid"] = gid
+            bind_cache[qid]["private"] = False
+            bind_cache[qid]["notice_on"] = True
+            reply = "设置成功！已为您开启推送。"
             save_binds()
     else:
-        reply = '您还没有绑定竞技场！'
+        reply = "您还没有绑定竞技场！"
     await matcher.finish(reply)
 
 
-@on_fullmatch(msg='换私聊推送').handle()
+@on_fullmatch(msg="换私聊推送").handle()
 async def _(bot: Bot, event: PrivateMessageEvent, matcher: Matcher):
     global bind_cache, lck, friend_list, pri_user, admin
     qid = str(event.user_id)
     for i in bind_cache:
-        if bind_cache[i]['notice_on'] and bind_cache[i]['private']:
+        if bind_cache[i]["notice_on"] and bind_cache[i]["private"]:
             pri_user += 1
     if pri_user >= MAX_PRI:
-        await matcher.finish('私聊推送用户已达上限！')
+        await matcher.finish("私聊推送用户已达上限！")
     if len(friend_list):
         await renew_friend_list()
     if qid not in friend_list:
         return
     async with lck:
-        bind_cache[qid]['private'] = True
-        bind_cache[qid]['notice_on'] = True
+        bind_cache[qid]["private"] = True
+        bind_cache[qid]["notice_on"] = True
         save_binds()
-    reply = '设置成功！已为您开启推送。已通知管理员！'
-    reply_adm = f'''{qid}开启了私聊jjc推送！'''
+    reply = "设置成功！已为您开启推送。已通知管理员！"
+    reply_adm = f"""{qid}开启了私聊jjc推送！"""
     await bot.send_private_msg(user_id=admin, message=reply_adm)
     await matcher.finish(reply)
 
 
-@on_regex(pattern=r'^竞技场设置 ?(开启|关闭) ?(jjc|pjjc|排名上升|at|上线提醒) ?(\d+)?$').handle()
+@on_regex(
+    pattern=r"^竞技场设置 ?(开启|关闭) ?(jjc|pjjc|排名上升|at|上线提醒) ?(\d+)?$"
+).handle()
 async def _(event: GroupMessageEvent, matcher: Matcher, group: tuple = RegexGroup()):
     global bind_cache, lck
     qid = str(event.user_id)
-    turn_on = True if str(group[0]) == '开启' else False
+    turn_on = True if str(group[0]) == "开启" else False
     change = group[1]
     pcrid_id = int(group[2]) if group[2] else None
 
     async with lck:
         if qid in bind_cache:
             pcrid_num = len(bind_cache[qid]["pcrid"])  # 这个qq号绑定的pcrid个数
             if pcrid_id is None:  # 只绑定1个uid时，绑定的序号可以不填。
                 if pcrid_num == 1:
                     pcrid_id = 1
                 else:
-                    reply = '您绑定了多个uid，更改设置时需要加上序号。'
+                    reply = "您绑定了多个uid，更改设置时需要加上序号。"
                     await matcher.finish(reply)
             if 0 <= pcrid_id <= pcrid_num:  # 设置成功！
                 if pcrid_id == 0:
                     for i in range(pcrid_num):
                         await set_notice_type_do(change, i, qid, turn_on)
                 else:
                     pcrid_id -= 1  # 从0开始计数，-1
                     await set_notice_type_do(change, pcrid_id, qid, turn_on)
-                reply = '设置成功！'
+                reply = "设置成功！"
                 save_binds()
             else:
-                reply = '序号超出范围，请检查您绑定的竞技场列表'
+                reply = "序号超出范围，请检查您绑定的竞技场列表"
         else:
-            reply = '您还没有绑定jjc，绑定方式：\n[竞技场绑定 uid] uid为pcr(b服)个人简介内13位数字'
+            reply = "您还没有绑定jjc，绑定方式：\n[竞技场绑定 uid] uid为pcr(b服)个人简介内13位数字"
     await matcher.finish(reply)
 
 
 async def set_notice_type_do(change, pcrid_id, qid, turn_on):
     global bind_cache
     tmp = int(bind_cache[qid]["noticeType"][pcrid_id])
     atNotice, jjcNotice, pjjcNotice, riseNotice = await get_notice_type(tmp)
     onlineNotice = True if tmp % 10 else False
-    if change == 'jjc':
+    if change == "jjc":
         jjcNotice = turn_on
-    elif change == 'pjjc':
+    elif change == "pjjc":
         pjjcNotice = turn_on
-    elif change == '排名上升':
+    elif change == "排名上升":
         riseNotice = turn_on
-    elif change == 'at':
+    elif change == "at":
         atNotice = turn_on
-    elif change == '上线提醒':
+    elif change == "上线提醒":
         onlineNotice = turn_on
-    tmp = jjcNotice * 10000 + pjjcNotice * 1000 + riseNotice * 100 + atNotice * 10 + onlineNotice
+    tmp = (
+        jjcNotice * 10000
+        + pjjcNotice * 1000
+        + riseNotice * 100
+        + atNotice * 10
+        + onlineNotice
+    )
     bind_cache[qid]["noticeType"][pcrid_id] = tmp
 
 
-@on_regex(pattern=r'^竞技场设置 ?([01]{4}[0123]) ?(\d+)?$').handle()
+@on_regex(pattern=r"^竞技场设置 ?([01]{4}[0123]) ?(\d+)?$").handle()
 async def _(event: GroupMessageEvent, matcher: Matcher, group: tuple = RegexGroup()):
     global bind_cache, lck
     qid = str(event.user_id)
     change = group[0]  # change: str
     pcrid_id = int(group[1]) if group[1] else None
     async with lck:
         if qid in bind_cache:
             pcrid_num = len(bind_cache[qid]["pcrid"])  # 这个qq号绑定的pcrid个数
             if pcrid_id is None:  # 只绑定1个uid时，绑定的序号可以不填。
                 if pcrid_num == 1:
                     pcrid_id = 1
                 else:
-                    reply = '您绑定了多个uid，更改设置时需要加上序号。'
+                    reply = "您绑定了多个uid，更改设置时需要加上序号。"
                     await matcher.finish(reply)
             if 0 <= pcrid_id <= pcrid_num:  # 设置成功！
                 change_quick_set = int(change)
                 if pcrid_id == 0:
                     for i in range(pcrid_num):
                         bind_cache[qid]["noticeType"][i] = change_quick_set
                 else:
                     pcrid_id -= 1  # 从0开始计数，-1
                     bind_cache[qid]["noticeType"][pcrid_id] = change_quick_set
-                reply = '设置成功！'
+                reply = "设置成功！"
                 save_binds()
             else:
-                reply = '序号超出范围，请检查您绑定的竞技场列表'
+                reply = "序号超出范围，请检查您绑定的竞技场列表"
         else:
-            reply = '您还没有绑定jjc，绑定方式：\n[竞技场绑定 uid] uid为pcr(b服)个人简介内13位数字'
+            reply = "您还没有绑定jjc，绑定方式：\n[竞技场绑定 uid] uid为pcr(b服)个人简介内13位数字"
     await matcher.finish(reply)
 
 
-@on_regex(pattern=r'^(开启|关闭)竞技场推送$').handle()
-async def _(bot: Bot, event: GroupMessageEvent, matcher: Matcher, group: tuple = RegexGroup()):
+@on_regex(pattern=r"^(开启|关闭)竞技场推送$").handle()
+async def _(
+    bot: Bot, event: GroupMessageEvent, matcher: Matcher, group: tuple = RegexGroup()
+):
     global bind_cache, lck, friend_list, pri_user, admin
     qid = str(event.user_id)
-    turn_on = True if group[0] == '开启' else False
+    turn_on = True if group[0] == "开启" else False
     async with lck:
         if qid in bind_cache:
             if bind_cache[qid]["notice_on"] == turn_on:
-                await matcher.finish(f'您的竞技场推送，已经是{group[0]}状态，不要重复{group[0]}！')
+                await matcher.finish(
+                    f"您的竞技场推送，已经是{group[0]}状态，不要重复{group[0]}！"
+                )
             else:
                 if turn_on:
                     if len(friend_list):
                         await renew_friend_list()
                     if bind_cache[qid]["private"]:
                         if qid not in friend_list:
-                            await matcher.finish('开启私聊推送需要先加好友！你也可以发送“在本群推送”，改为群聊推送。')
+                            await matcher.finish(
+                                "开启私聊推送需要先加好友！你也可以发送“在本群推送”，改为群聊推送。"
+                            )
                         else:
                             for i in bind_cache:
-                                if bind_cache[i]['notice_on'] and bind_cache[i]['private']:
+                                if (
+                                    bind_cache[i]["notice_on"]
+                                    and bind_cache[i]["private"]
+                                ):
                                     pri_user += 1
                             if pri_user >= MAX_PRI:
-                                await matcher.finish('私聊推送用户已达上限！')
-                            reply_adm = f'''{qid}开启了私聊jjc推送！'''
+                                await matcher.finish("私聊推送用户已达上限！")
+                            reply_adm = f"""{qid}开启了私聊jjc推送！"""
                             await bot.send_private_msg(user_id=admin, message=reply_adm)
-                            await matcher.finish('已通知管理员')
+                            await matcher.finish("已通知管理员")
                 bind_cache[qid]["notice_on"] = turn_on
         else:
-            await matcher.finish('您还没有绑定竞技场！')
+            await matcher.finish("您还没有绑定竞技场！")
         save_binds()
-    await matcher.finish(f'竞技场推送{group[0]}成功！')
+    await matcher.finish(f"竞技场推送{group[0]}成功！")
+
 
+# ========================================Admin========================================
 
-# ========================================管理员指令========================================
 
-@on_fullmatch(msg='pcrjjc负载查询', permission=SUPERUSER).handle()
+@on_fullmatch(msg="pcrjjc负载查询", permission=SUPERUSER).handle()
 async def _(matcher: Matcher):
     global bind_cache, today_notice, yesterday_notice
     qid_notice_on_private = 0
     qid_notice_on_group = 0
     pcrid_num_private = 0
     pcrid_num_group = 0
     for qid in bind_cache:
-        if bind_cache[qid]['notice_on']:
-            if bind_cache[qid]['private']:
+        if bind_cache[qid]["notice_on"]:
+            if bind_cache[qid]["private"]:
                 qid_notice_on_private += 1
-                pcrid_num_private += len(bind_cache[qid]['pcrid'])
+                pcrid_num_private += len(bind_cache[qid]["pcrid"])
             else:
                 qid_notice_on_group += 1
-                pcrid_num_group += len(bind_cache[qid]['pcrid'])
-    msg = f'''pcrjjc负载：\n群聊用户数量：{qid_notice_on_group} 群聊绑定的uid：{pcrid_num_group}个\n私聊用户数量：{qid_notice_on_private} 私聊绑定的uid：{pcrid_num_private}个\n昨天推送次数：{yesterday_notice} 今天推送次数：{today_notice}'''
+                pcrid_num_group += len(bind_cache[qid]["pcrid"])
+    msg = f"""pcrjjc负载：\n群聊用户数量：{qid_notice_on_group} 群聊绑定的uid：{pcrid_num_group}个\n私聊用户数量：{qid_notice_on_private} 私聊绑定的uid：{pcrid_num_private}个\n昨天推送次数：{yesterday_notice} 今天推送次数：{today_notice}"""
     pic = image_draw(msg)
     await matcher.finish(MessageSegment.image(pic))
 
 
-@on_fullmatch(msg='pcrjjc关闭私聊推送', permission=SUPERUSER).handle()
+@on_fullmatch(msg="pcrjjc关闭私聊推送", permission=SUPERUSER).handle()
 async def _(matcher: Matcher):
     global bind_cache, lck
     async with lck:
         for qid in bind_cache:
-            if bind_cache[qid]['private'] and bind_cache[qid]['notice_on']:
-                bind_cache[qid]['notice_on'] = False
+            if bind_cache[qid]["private"] and bind_cache[qid]["notice_on"]:
+                bind_cache[qid]["notice_on"] = False
         save_binds()
-    await matcher.finish('所有设置为私聊推送的用户的推送已关闭！')
+    await matcher.finish("所有设置为私聊推送的用户的推送已关闭！")
 
 
-@on_regex(pattern=r'^pcrjjc删除绑定 ?(\d{6,10})', permission=SUPERUSER).handle()
+@on_regex(pattern=r"^pcrjjc删除绑定 ?(\d{6,10})", permission=SUPERUSER).handle()
 async def _(matcher: Matcher, group: tuple = RegexGroup()):
     global bind_cache, lck
     qid = str(group[0])
     if qid in bind_cache:
         async with lck:
             del bind_cache[qid]
             save_binds()
-        reply = '删除成功！'
+        reply = "删除成功！"
     else:
-        reply = '绑定列表中找不到这个qq号！'
+        reply = "绑定列表中找不到这个qq号！"
     await matcher.finish(reply)
 
 
-@on_fullmatch(msg='pcrjjc关闭排名上升', permission=SUPERUSER).handle()
+@on_fullmatch(msg="pcrjjc关闭排名上升", permission=SUPERUSER).handle()
 async def _(matcher: Matcher):
     global bind_cache, lck
     async with lck:
         for qid in bind_cache:
-            for index, tmp in enumerate(bind_cache[qid]['noticeType']):
+            for index, tmp in enumerate(bind_cache[qid]["noticeType"]):
                 jjcNotice = True if tmp // 10000 else False
                 pjjcNotice = True if (tmp % 10000) // 1000 else False
                 riseNotice = 0
                 atNotice = True if (tmp % 100) // 10 else False
                 onlineNotice = tmp % 10
-                tmp = jjcNotice * 10000 + pjjcNotice * 1000 + riseNotice * 100 + atNotice * 10 + onlineNotice
-                bind_cache[qid]['noticeType'][index] = tmp
+                tmp = (
+                    jjcNotice * 10000
+                    + pjjcNotice * 1000
+                    + riseNotice * 100
+                    + atNotice * 10
+                    + onlineNotice
+                )
+                bind_cache[qid]["noticeType"][index] = tmp
         save_binds()
-    await matcher.finish('所有上升提醒推送已关闭！')
+    await matcher.finish("所有上升提醒推送已关闭！")
 
 
-# ========================================函数========================================
+# ========================================Function========================================
 def save_binds():
-    with open(config, 'w') as fp:
+    with open(config, "w") as fp:
         dump(root, fp, indent=4)
 
 
 def delete_arena(uid):
     """
     订阅删除方法
     """
     try:
         bind_cache.pop(uid)
         save_binds()
-    except:
+    except KeyError:
         logger.info("该用户可能已经不在订阅中")
 
 
 async def renew_pcrid_list():
     global bind_cache, pcrid_list, lck, lck_friend_list, friend_list
     pcrid_list = []
     async with lck_friend_list:
@@ -697,20 +776,26 @@
     pcrid_list = list(set(pcrid_list))
 
 
 async def query_schedule(data):
     global cache, timeStamp
     timeStamp = int(time.time())
     try:
-        info = data["res"]['user_info']
+        info = data["res"]["user_info"]
     except KeyError:
         return
     pcrid = data["uid"]
     # logger.info(f'渠query for {pcrid}') #debug
-    res = [int(info['arena_rank']), int(info['grand_arena_rank']), int(info['last_login_time']), 0, 0]
+    res = [
+        int(info["arena_rank"]),
+        int(info["grand_arena_rank"]),
+        int(info["last_login_time"]),
+        0,
+        0,
+    ]
     if pcrid not in cache:
         cache[pcrid] = res
     else:
         last = deepcopy(cache[pcrid])
         cache[pcrid][0] = res[0]
         cache[pcrid][1] = res[1]
         cache[pcrid][2] = res[2]
@@ -730,231 +815,266 @@
     global bind_cache, cache, lck
     bot = data["bot"]
     ev = data["event"]
     i = data["index"]
     pcrid = data["uid"]
     manual_query_list_name = data["list"]
     try:
-        res = data["res"]['user_info']
+        res = data["res"]["user_info"]
         query_list = query_cache[ev.user_id]
         last_login_hour = (int(res["last_login_time"]) % 86400 // 3600 + 8) % 24
         last_login_min = int(res["last_login_time"]) % 3600 // 60
-        last_login_min = '%02d' % last_login_min  # 分钟补零，变成2位
+        last_login_min = "%02d" % last_login_min  # 分钟补零，变成2位
         if manual_query_list_name[i]:
             res["user_name"] = manual_query_list_name[i]
-        extra = ''
+        extra = ""
         if pcrid in cache:
-            extra = f'''上升: {cache[pcrid][3]}次 / {cache[pcrid][4]}次\n'''
-        i = i if data.get("only") is None else data.get("only")  # 如果是查询单个，修改其序号
+            extra = f"""上升: {cache[pcrid][3]}次 / {cache[pcrid][4]}次\n"""
+        i = (
+            i if data.get("only") is None else data.get("only")
+        )  # 如果是查询单个，修改其序号
         query = f'【{i + 1:02}】{res["user_name"]}\n{res["arena_rank"]}({res["arena_group"]}场) / {res["grand_arena_rank"]}({res["grand_arena_group"]}场)\n{extra}最近上号{last_login_hour}：{last_login_min}\n\n'
         async with lck:
             query_list.append(query)
             if len(query_list) == len(manual_query_list_name):
                 query_list.sort()
-                pic = image_draw(''.join(query_list))
+                pic = image_draw("".join(query_list))
                 for sid in get_bots():
                     try:
-                        await bot.send_group_msg(self_id=sid, group_id=int(ev.group_id),
-                                                 message=MessageSegment.image(pic))
+                        await bot.send_group_msg(
+                            self_id=sid,
+                            group_id=int(ev.group_id),
+                            message=MessageSegment.image(pic),
+                        )
                         break
                     except Exception as e:
                         logger.debug(e)
     except KeyError:
-        await bot.send_group_msg(group_id=int(ev.group_id), message=f'找不到这个uid，大概率是你输错了！')
+        await bot.send_group_msg(
+            group_id=int(ev.group_id), message="找不到这个uid，大概率是你输错了！"
+        )
 
 
 async def member_add_sub(data):
     global bind_cache, lck, friend_list, MAX_PCRID
     bot = data["bot"]
     ev = data["event"]
     nickname = data["nickname"]
     pcrid = data["uid"]
-    friend_list = data['friend_list']
+    friend_list = data["friend_list"]
     try:
-        res = data["res"]['user_info']
+        res = data["res"]["user_info"]
         qid = str(ev.user_id)
         gid = ev.group_id
         async with lck:
             if qid in bind_cache:
                 bind_num = len(bind_cache[qid]["pcrid"])
                 if bind_num >= MAX_PCRID:
-                    reply = '您订阅了太多账号啦！'
+                    reply = "您订阅了太多账号啦！"
                 elif pcrid in bind_cache[qid]["pcrid"]:
-                    reply = '这个uid您已经订阅过了，不要重复订阅！'
+                    reply = "这个uid您已经订阅过了，不要重复订阅！"
                 else:
                     bind_cache[qid]["pcrid"].append(pcrid)
-                    bind_cache[qid]["pcrName"].append(nickname if nickname else res["user_name"])
+                    bind_cache[qid]["pcrName"].append(
+                        nickname if nickname else res["user_name"]
+                    )
                     bind_cache[qid]["noticeType"].append(11010)
-                    reply = '添加成功！'
+                    reply = "添加成功！"
             else:
                 bind_cache[qid] = {
                     "pcrid": [pcrid],
                     "noticeType": [11010],
                     "pcrName": [nickname if nickname else res["user_name"]],
                     "gid": gid,
                     "bot_id": 0,
                     "private": False,
-                    "notice_on": False
+                    "notice_on": False,
                 }
-                reply = '添加成功！'
+                reply = "添加成功！"
                 if gid == 0:
                     bind_cache[qid]["private"] = True
                     if len(friend_list):
                         await renew_friend_list()
                     if qid in friend_list:
                         pri_user = 0
                         for i in bind_cache:
-                            if bind_cache[i]['notice_on'] and bind_cache[i]['private']:
+                            if bind_cache[i]["notice_on"] and bind_cache[i]["private"]:
                                 pri_user += 1
                         if pri_user >= MAX_PRI:
-                            reply += '私聊推送用户已达上限！无法开启私聊推送。你可以发送“在本群推送”，改为群聊推送。'
+                            reply += "私聊推送用户已达上限！无法开启私聊推送。你可以发送“在本群推送”，改为群聊推送。"
                         else:
                             bind_cache[qid]["notice_on"] = True
-                            reply_adm = f'''{qid}添加了私聊pcrjjc推送'''
+                            reply_adm = f"""{qid}添加了私聊pcrjjc推送"""
                             await bot.send_private_msg(user_id=admin, message=reply_adm)
-                            reply += '已为您开启推送。由于是私聊推送，已通知管理员！'
+                            reply += "已为您开启推送。由于是私聊推送，已通知管理员！"
                     else:
-                        reply += '开启私聊推送需要先加好友！你也可以发送“在本群推送”，改为群聊推送。'
+                        reply += "开启私聊推送需要先加好友！你也可以发送“在本群推送”，改为群聊推送。"
                 else:
                     bind_cache[qid]["notice_on"] = True
-                    reply += '已为您开启群聊推送！'
+                    reply += "已为您开启群聊推送！"
             save_binds()
     except KeyError:
-        reply = f'找不到这个uid，大概率是你输错了！'
+        reply = "找不到这个uid，大概率是你输错了！"
     for sid in get_bots():
         try:
-            await bot.send_group_msg(self_id=sid, group_id=int(ev.group_id), message=reply)
+            await bot.send_group_msg(
+                self_id=sid, group_id=int(ev.group_id), message=reply
+            )
             break
         except Exception as e:
             logger.debug(e)
 
 
-async def send_notice(new: int, old: int, pcrid: int, notice_type: int):  # noticeType：1:jjc排名变动   2:pjjc排名变动  3:登录时间刷新
+async def send_notice(
+    new: int, old: int, pcrid: int, notice_type: int
+):  # noticeType：1:jjc排名变动   2:pjjc排名变动  3:登录时间刷新
     global bind_cache, timeStamp, jjc_log, today_notice, NOTICE_CD_MIN
     bot = get_bot()
     if notice_type == 3:
-        change = f'''上线了！[{time.strftime("%H:%M", time.localtime(new))}]'''
+        change = f"""上线了！[{time.strftime("%H:%M", time.localtime(new))}]"""
     else:
         jjc_log_new = (timeStamp, notice_type, new, old)
         if pcrid in jjc_log:
             if len(jjc_log[pcrid]) >= 20:
                 del jjc_log[pcrid][0]
             jjc_log[pcrid].append(jjc_log_new)
         else:
             jjc_log_new_tmp = [jjc_log_new]
             jjc_log[pcrid] = jjc_log_new_tmp
         if notice_type == 1:
-            change = '\njjc: '
+            change = "\njjc: "
         elif notice_type == 2:
-            change = '\npjjc: '
+            change = "\npjjc: "
         if new < old:
-            change += f'''{old}->{new} [▲{old - new}]'''
+            change += f"""{old}->{new} [▲{old - new}]"""
         else:
-            change += f'''{old}->{new} [▽{new - old}]'''
+            change += f"""{old}->{new} [▽{new - old}]"""
     # -----------------------------------------------------------------
     for qid in bind_cache:
         if not bind_cache[qid]["notice_on"]:
             continue
         for i in range(len(bind_cache[qid]["pcrid"])):
             if bind_cache[qid]["pcrid"][i] == pcrid:
                 tmp = bind_cache[qid]["noticeType"][i]
                 name = bind_cache[qid]["pcrName"][i]
                 atNotice, jjcNotice, pjjcNotice, riseNotice = await get_notice_type(tmp)
                 onlineNotice = False
                 if (OnlineType := tmp % 10) and notice_type == 3:
                     if (new - old) < (60 if OnlineType == 3 else 60 * NOTICE_CD_MIN):
                         cache[pcrid][2] = old  # 间隔太短，不更新缓存
                     elif OnlineType != 1 or (
-                            (new % 86400 // 3600 + 8) % 24 == 14 and new % 3600 // 60 >= 30):  # 类型1，只在特定时间播报
+                        (new % 86400 // 3600 + 8) % 24 == 14 and new % 3600 // 60 >= 30
+                    ):  # 类型1，只在特定时间播报
                         onlineNotice = True
-                if (((notice_type == 1 and jjcNotice) or (notice_type == 2 and pjjcNotice)) and (
-                        riseNotice or (new > old))) or (notice_type == 3 and onlineNotice):
-                    logger.info('sendNotice   sendNotice    sendNotice')
+                if (
+                    (
+                        (notice_type == 1 and jjcNotice)
+                        or (notice_type == 2 and pjjcNotice)
+                    )
+                    and (riseNotice or (new > old))
+                ) or (notice_type == 3 and onlineNotice):
+                    logger.info("sendNotice   sendNotice    sendNotice")
                     msg = Message()
                     msg.append(name + change)
                     today_notice += 1
                     if bind_cache[qid]["private"]:
                         for sid in get_bots():
                             try:
-                                await bot.send_private_msg(self_id=sid, user_id=int(qid), message=msg)
+                                await bot.send_private_msg(
+                                    self_id=sid, user_id=int(qid), message=msg
+                                )
                                 return
-                            except:
+                            except Exception:
                                 pass
                         bind_cache[qid]["notice_on"] = False
                     else:
                         if atNotice:
                             msg.append(MessageSegment.at(qid))
                         for sid in get_bots():
                             try:
-                                await bot.send_group_msg(self_id=sid, group_id=int(bind_cache[qid]["gid"]), message=msg)
+                                await bot.send_group_msg(
+                                    self_id=sid,
+                                    group_id=int(bind_cache[qid]["gid"]),
+                                    message=msg,
+                                )
                                 break
                             except Exception as e:
                                 logger.debug(e)
                 break
 
 
-# ========================================AUTO========================================
+# ========================================Auto========================================
+
 
 @driver.on_bot_connect
 async def _():
-    scheduler.add_job(renew_friend_list, 'interval', hours=5)
-    scheduler.add_job(on_arena_schedule, 'interval', seconds=REFRESH_SECOND)
-    scheduler.add_job(clear_ranking_rise_time, 'cron', hour='5')
+    scheduler.add_job(renew_friend_list, "interval", hours=5)
+    scheduler.add_job(on_arena_schedule, "interval", seconds=REFRESH_SECOND)
+    scheduler.add_job(clear_ranking_rise_time, "cron", hour="5")
 
 
 async def renew_friend_list():
     global friend_list, lck_friend_list
     bot = get_bot()
     old_friendList = friend_list
     for sid in get_bots():
         flist = await bot.get_friend_list(self_id=int(sid))
         async with lck_friend_list:
             friend_list = []
             for i in flist:
-                friend_list.append(str(i['user_id']))
+                friend_list.append(str(i["user_id"]))
             old_friendList = list(set(old_friendList))
             friend_list = list(set(friend_list))
 
 
 async def on_arena_schedule():
     await renew_pcrid_list()
     await queue.join()
-    await gather(*map(lambda uid: queue.put((10, (query_schedule, uid, {"uid": uid}))), pcrid_list))
+    await gather(
+        *map(
+            lambda uid: queue.put((10, (query_schedule, uid, {"uid": uid}))), pcrid_list
+        )
+    )
 
 
 async def clear_ranking_rise_time():
     global cache, today_notice, yesterday_notice
     yesterday_notice = today_notice
     today_notice = 0
     for pcrid in list(cache.keys()):
         if pcrid in pcrid_list:
             cache[pcrid][3] = 0
             cache[pcrid][4] = 0
         else:
             del cache[pcrid]
     async with lck:  # 上线提醒LV3改成2
         for qid in bind_cache:
-            for i in range(len(bind_cache[qid]['noticeType'])):
-                if bind_cache[qid]['noticeType'][i] % 10 == 3:
-                    bind_cache[qid]['noticeType'][i] -= 1
+            for i in range(len(bind_cache[qid]["noticeType"])):
+                if bind_cache[qid]["noticeType"][i] % 10 == 3:
+                    bind_cache[qid]["noticeType"][i] -= 1
         save_binds()
 
 
-@on_notice(rule=lambda event: event.notice_type == 'friend_add').handle()  # 新增好友时，不全部刷新好友列表
+@on_notice(
+    rule=lambda event: event.notice_type == "friend_add"
+).handle()  # 新增好友时，不全部刷新好友列表
 async def friend_add(event: FriendAddNoticeEvent):
     global friend_list
     new_friend = str(event.user_id)
     async with lck_friend_list:
         friend_list.append(new_friend)
 
 
-@on_notice(rule=lambda event: event.notice_type == 'group_decrease' and event.sub_type == 'leave').handle()
+@on_notice(
+    rule=lambda event: event.notice_type == "group_decrease"
+    and event.sub_type == "leave"
+).handle()
 async def leave_notice(event: GroupDecreaseNoticeEvent, matcher: Matcher):
     global lck, bind_cache
     uid = str(event.user_id)
     gid = str(event.group_id)
     async with lck:
         binds = deepcopy(bind_cache)
         info = binds[uid]
-        if uid in bind_cache and info['gid'] == gid:
+        if uid in bind_cache and info["gid"] == gid:
             delete_arena(uid)
-            await matcher.finish(f'{uid}退群了，已自动删除其绑定在本群的竞技场订阅推送')
+            await matcher.finish(f"{uid}退群了，已自动删除其绑定在本群的竞技场订阅推送")
```

### Comparing `nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/aiorequests.py` & `nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/aiorequests.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/bsgamesdk.py` & `nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/bsgamesdk.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/config.py` & `nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/pcrclient.py` & `nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/pcrclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,15 @@
                 match = search(
                     "\d\d\d\d-\d\d-\d\d \d\d:\d\d:\d\d", manifest["maintenance_message"]
                 ).group()
                 end = parse(match)
                 logger.info("server is in maintenance until {}", match)
                 while datetime.now() < end:
                     await sleep(1)
-            except:
+            except Exception:
                 logger.info("server is in maintenance. waiting for 60 secs")
                 await sleep(60)
 
         ver = manifest["required_manifest_ver"]
         logger.info("using manifest ver = {}", ver)
         self.headers["MANIFEST-VER"] = str(ver)
         l_res = await self.callapi(
```

### Comparing `nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/query.py` & `nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/query.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/text2img.py` & `nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/text2img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO` & `nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pcrjjc
-Version: 0.7.0
+Version: 0.8.0
 Summary: pcrjjc排名监测插件
 Author-email: reine-ishyanami <2402979195@qq.com>
 License: AGPL-3
 Project-URL: Homepage, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc
 Project-URL: Bug Tracker, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc/issues
 Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -15,15 +15,15 @@
 Classifier: Natural Language :: Chinese (Simplified)
 Requires-Python: <4.0,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: msgpack>=1.0.5
 Requires-Dist: requests>=2.30.0
 Requires-Dist: Pillow>=9.5.0
-Requires-Dist: pydantic>=2
+Requires-Dist: pydantic>=1.10.14
 Requires-Dist: python-dateutil>=2.8.2
 Requires-Dist: pycryptodome>=3.18.0
 Requires-Dist: nonebot2>=2.0.0
 Requires-Dist: nonebot-adapter-onebot>=2.2.3
 Requires-Dist: nonebot-plugin-apscheduler>=0.3.0
 
 # nonebot-plugin-pcrjjc
```

### Comparing `nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt` & `nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 src/nonebot_plugin_pcrjjc/__init__.py
 src/nonebot_plugin_pcrjjc/aiorequests.py
 src/nonebot_plugin_pcrjjc/bsgamesdk.py
 src/nonebot_plugin_pcrjjc/config.py
+src/nonebot_plugin_pcrjjc/main.py
 src/nonebot_plugin_pcrjjc/pcrclient.py
 src/nonebot_plugin_pcrjjc/query.py
 src/nonebot_plugin_pcrjjc/rsacr.py
 src/nonebot_plugin_pcrjjc/text2img.py
 src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO
 src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt
 src/nonebot_plugin_pcrjjc.egg-info/dependency_links.txt
```

