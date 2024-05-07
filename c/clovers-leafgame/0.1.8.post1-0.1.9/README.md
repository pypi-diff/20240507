# Comparing `tmp/clovers_leafgame-0.1.8.post1.tar.gz` & `tmp/clovers_leafgame-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clovers_leafgame-0.1.8.post1.tar", max compression
+gzip compressed data, was "clovers_leafgame-0.1.9.tar", max compression
```

## Comparing `clovers_leafgame-0.1.8.post1.tar` & `clovers_leafgame-0.1.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      300 2024-04-27 08:49:20.730233 clovers_leafgame-0.1.8.post1/clovers_leafgame/__init__.py
--rw-r--r--   0        0        0      682 2024-04-27 08:49:20.730233 clovers_leafgame-0.1.8.post1/clovers_leafgame/config.py
--rw-r--r--   0        0        0     4001 2024-05-01 06:15:17.412881 clovers_leafgame-0.1.8.post1/clovers_leafgame/core/clovers.py
--rw-r--r--   0        0        0     5568 2024-04-27 09:13:40.955639 clovers_leafgame-0.1.8.post1/clovers_leafgame/core/data.py
--rw-r--r--   0        0        0     1617 2024-04-27 08:49:20.731606 clovers_leafgame-0.1.8.post1/clovers_leafgame/item.py
--rw-r--r--   0        0        0     1151 2024-04-27 08:49:20.731606 clovers_leafgame-0.1.8.post1/clovers_leafgame/main.py
--rw-r--r--   0        0        0     6630 2024-05-01 02:31:44.190645 clovers_leafgame-0.1.8.post1/clovers_leafgame/manager.py
--rw-r--r--   0        0        0    14551 2024-05-01 01:41:25.978756 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/account/__init__.py
--rw-r--r--   0        0        0      347 2024-04-27 08:49:20.733113 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/account/config.py
--rw-r--r--   0        0        0    44586 2024-05-01 02:45:31.478949 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/__init__.py
--rw-r--r--   0        0        0      153 2024-04-27 08:49:20.733802 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/config.py
--rw-r--r--   0        0        0     8755 2024-04-27 08:49:20.734312 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/core.py
--rw-r--r--   0        0        0    10104 2024-04-27 08:49:20.734812 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/fortress/core.py
--rw-r--r--   0        0        0    12802 2024-04-27 08:49:20.735312 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/__init__.py
--rw-r--r--   0        0        0      447 2024-04-27 08:49:20.735312 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/config.py
--rw-r--r--   0        0        0     5817 2024-04-27 08:49:20.735812 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/Stand.json
--rw-r--r--   0        0        0     5728 2024-04-27 08:49:20.736312 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json
--rw-r--r--   0        0        0     2174 2024-04-27 08:49:20.736811 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json
--rw-r--r--   0        0        0     1231 2024-04-27 08:49:20.736811 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json
--rw-r--r--   0        0        0     2742 2024-04-27 08:49:20.737312 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json
--rw-r--r--   0        0        0     1606 2024-04-27 08:49:20.737312 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json
--rw-r--r--   0        0        0    25830 2024-04-27 08:49:20.737811 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json
--rw-r--r--   0        0        0     5180 2024-04-27 08:49:20.738314 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json
--rw-r--r--   0        0        0     1072 2024-04-27 08:49:20.738314 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json
--rw-r--r--   0        0        0     2294 2024-04-27 08:49:20.738812 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json
--rw-r--r--   0        0        0     7488 2024-04-27 08:49:20.738812 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/horse.py
--rw-r--r--   0        0        0      933 2024-04-27 08:49:20.739312 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/start.py
--rw-r--r--   0        0        0      754 2024-04-27 08:49:20.739812 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/tools.py
--rw-r--r--   0        0        0    18182 2024-04-27 08:49:20.740312 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/market/__init__.py
--rw-r--r--   0        0        0      457 2024-04-27 08:49:20.740820 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/market/config.py
--rw-r--r--   0        0        0    12681 2024-05-01 06:16:15.242569 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/prop/__init__.py
--rw-r--r--   0        0        0      271 2024-04-27 08:49:20.741311 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/prop/config.py
--rw-r--r--   0        0        0     2085 2024-04-27 08:49:20.741812 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/prop/core.py
--rw-r--r--   0        0        0     2681 2024-04-27 08:49:20.741812 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/prop/output.py
--rw-r--r--   0        0        0     4514 2024-05-01 06:19:53.256256 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/prop/props_library.json
--rw-r--r--   0        0        0     3958 2024-04-27 08:49:20.742812 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/ranklist/__init__.py
--rw-r--r--   0        0        0     1003 2024-04-27 08:49:20.742812 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/ranklist/output.py
--rw-r--r--   0        0        0     3587 2024-04-27 09:15:30.718836 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/task/__init__.py
--rw-r--r--   0        0        0     6592 2024-04-27 08:49:20.743811 clovers_leafgame-0.1.8.post1/clovers_leafgame/output.py
--rw-r--r--   0        0        0     1806 2024-04-27 09:12:59.164148 clovers_leafgame-0.1.8.post1/clovers_leafgame/props_library.json
--rw-r--r--   0        0        0     1086 2024-04-27 08:49:20.729233 clovers_leafgame-0.1.8.post1/LICENSE
--rw-r--r--   0        0        0      430 2024-05-01 06:21:17.767326 clovers_leafgame-0.1.8.post1/pyproject.toml
--rw-r--r--   0        0        0    18943 2024-04-27 15:58:16.641831 clovers_leafgame-0.1.8.post1/README.md
--rw-r--r--   0        0        0    18663 1970-01-01 00:00:00.000000 clovers_leafgame-0.1.8.post1/PKG-INFO
+-rw-r--r--   0        0        0      300 2024-04-27 08:49:20.730233 clovers_leafgame-0.1.9/clovers_leafgame/__init__.py
+-rw-r--r--   0        0        0      682 2024-04-27 08:49:20.730233 clovers_leafgame-0.1.9/clovers_leafgame/config.py
+-rw-r--r--   0        0        0     4001 2024-05-01 06:15:17.412881 clovers_leafgame-0.1.9/clovers_leafgame/core/clovers.py
+-rw-r--r--   0        0        0     5568 2024-04-27 09:13:40.955639 clovers_leafgame-0.1.9/clovers_leafgame/core/data.py
+-rw-r--r--   0        0        0     1617 2024-04-27 08:49:20.731606 clovers_leafgame-0.1.9/clovers_leafgame/item.py
+-rw-r--r--   0        0        0     1151 2024-04-27 08:49:20.731606 clovers_leafgame-0.1.9/clovers_leafgame/main.py
+-rw-r--r--   0        0        0     6630 2024-05-01 02:31:44.190645 clovers_leafgame-0.1.9/clovers_leafgame/manager.py
+-rw-r--r--   0        0        0    14551 2024-05-01 01:41:25.978756 clovers_leafgame-0.1.9/clovers_leafgame/modules/account/__init__.py
+-rw-r--r--   0        0        0      347 2024-04-27 08:49:20.733113 clovers_leafgame-0.1.9/clovers_leafgame/modules/account/config.py
+-rw-r--r--   0        0        0    44537 2024-05-01 07:58:51.681530 clovers_leafgame-0.1.9/clovers_leafgame/modules/game/__init__.py
+-rw-r--r--   0        0        0      153 2024-04-27 08:49:20.733802 clovers_leafgame-0.1.9/clovers_leafgame/modules/game/config.py
+-rw-r--r--   0        0        0     8755 2024-04-27 08:49:20.734312 clovers_leafgame-0.1.9/clovers_leafgame/modules/game/core.py
+-rw-r--r--   0        0        0    10104 2024-04-27 08:49:20.734812 clovers_leafgame-0.1.9/clovers_leafgame/modules/game/fortress/core.py
+-rw-r--r--   0        0        0    12802 2024-04-27 08:49:20.735312 clovers_leafgame-0.1.9/clovers_leafgame/modules/game/horse_race/__init__.py
+-rw-r--r--   0        0        0      447 2024-04-27 08:49:20.735312 clovers_leafgame-0.1.9/clovers_leafgame/modules/game/horse_race/config.py
+-rw-r--r--   0        0        0     5817 2024-04-27 08:49:20.735812 clovers_leafgame-0.1.9/clovers_leafgame/modules/game/horse_race/event_library/Stand.json
+-rw-r--r--   0        0        0     5728 2024-04-27 08:49:20.736312 clovers_leafgame-0.1.9/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json
+-rw-r--r--   0        0        0     2174 2024-04-27 08:49:20.736811 clovers_leafgame-0.1.9/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json
+-rw-r--r--   0        0        0     1231 2024-04-27 08:49:20.736811 clovers_leafgame-0.1.9/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json
+-rw-r--r--   0        0        0     2742 2024-04-27 08:49:20.737312 clovers_leafgame-0.1.9/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json
+-rw-r--r--   0        0        0     1606 2024-04-27 08:49:20.737312 clovers_leafgame-0.1.9/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json
+-rw-r--r--   0        0        0    25830 2024-04-27 08:49:20.737811 clovers_leafgame-0.1.9/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json
+-rw-r--r--   0        0        0     5180 2024-04-27 08:49:20.738314 clovers_leafgame-0.1.9/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json
+-rw-r--r--   0        0        0     1072 2024-04-27 08:49:20.738314 clovers_leafgame-0.1.9/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json
+-rw-r--r--   0        0        0     2294 2024-04-27 08:49:20.738812 clovers_leafgame-0.1.9/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json
+-rw-r--r--   0        0        0     7488 2024-04-27 08:49:20.738812 clovers_leafgame-0.1.9/clovers_leafgame/modules/game/horse_race/horse.py
+-rw-r--r--   0        0        0      933 2024-04-27 08:49:20.739312 clovers_leafgame-0.1.9/clovers_leafgame/modules/game/horse_race/start.py
+-rw-r--r--   0        0        0      754 2024-04-27 08:49:20.739812 clovers_leafgame-0.1.9/clovers_leafgame/modules/game/tools.py
+-rw-r--r--   0        0        0    18182 2024-04-27 08:49:20.740312 clovers_leafgame-0.1.9/clovers_leafgame/modules/market/__init__.py
+-rw-r--r--   0        0        0      457 2024-04-27 08:49:20.740820 clovers_leafgame-0.1.9/clovers_leafgame/modules/market/config.py
+-rw-r--r--   0        0        0    13046 2024-05-01 07:55:19.975141 clovers_leafgame-0.1.9/clovers_leafgame/modules/prop/__init__.py
+-rw-r--r--   0        0        0      271 2024-04-27 08:49:20.741311 clovers_leafgame-0.1.9/clovers_leafgame/modules/prop/config.py
+-rw-r--r--   0        0        0     2085 2024-04-27 08:49:20.741812 clovers_leafgame-0.1.9/clovers_leafgame/modules/prop/core.py
+-rw-r--r--   0        0        0     2681 2024-04-27 08:49:20.741812 clovers_leafgame-0.1.9/clovers_leafgame/modules/prop/output.py
+-rw-r--r--   0        0        0     4487 2024-05-01 07:49:44.252541 clovers_leafgame-0.1.9/clovers_leafgame/modules/prop/props_library.json
+-rw-r--r--   0        0        0     3958 2024-04-27 08:49:20.742812 clovers_leafgame-0.1.9/clovers_leafgame/modules/ranklist/__init__.py
+-rw-r--r--   0        0        0     1003 2024-04-27 08:49:20.742812 clovers_leafgame-0.1.9/clovers_leafgame/modules/ranklist/output.py
+-rw-r--r--   0        0        0     3587 2024-04-27 09:15:30.718836 clovers_leafgame-0.1.9/clovers_leafgame/modules/task/__init__.py
+-rw-r--r--   0        0        0     6592 2024-04-27 08:49:20.743811 clovers_leafgame-0.1.9/clovers_leafgame/output.py
+-rw-r--r--   0        0        0     1806 2024-04-27 09:12:59.164148 clovers_leafgame-0.1.9/clovers_leafgame/props_library.json
+-rw-r--r--   0        0        0     1086 2024-04-27 08:49:20.729233 clovers_leafgame-0.1.9/LICENSE
+-rw-r--r--   0        0        0      428 2024-05-01 08:01:30.942019 clovers_leafgame-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    18943 2024-04-27 15:58:16.641831 clovers_leafgame-0.1.9/README.md
+-rw-r--r--   0        0        0    18657 1970-01-01 00:00:00.000000 clovers_leafgame-0.1.9/PKG-INFO
```

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/config.py` & `clovers_leafgame-0.1.9/clovers_leafgame/config.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/core/clovers.py` & `clovers_leafgame-0.1.9/clovers_leafgame/core/clovers.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/core/data.py` & `clovers_leafgame-0.1.9/clovers_leafgame/core/data.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/item.py` & `clovers_leafgame-0.1.9/clovers_leafgame/item.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/main.py` & `clovers_leafgame-0.1.9/clovers_leafgame/main.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/manager.py` & `clovers_leafgame-0.1.9/clovers_leafgame/manager.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/account/__init__.py` & `clovers_leafgame-0.1.9/clovers_leafgame/modules/account/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/__init__.py` & `clovers_leafgame-0.1.9/clovers_leafgame/modules/game/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import random
 import asyncio
 from collections import Counter
-from clovers_leafgame.main import plugin, manager
+from clovers_leafgame.main import plugin, manager, build_result
 from clovers_leafgame.core.clovers import Event
 from clovers_leafgame.output import text_to_image, BytesIO
 from .core import Session, Game, to_int
 from .tools import random_poker, poker_suit, poker_point, poker_show
 
 place: dict[str, Session] = {}
 
@@ -675,45 +675,45 @@
 @blackjack.action(place)
 async def _(event: Event, session: Session):
     hand, pt = blackjack_hit(session)
     msg = f"你的手牌：\n{poker_show(hand,'\n')}\n合计:{pt}点"
     if pt > 21:
         await event.send_group_message(
             session.group_id,
-            plugin.build_result(session.end(msg)),
+            build_result(session.end(msg)),
         )
     if not event.is_private():
         msg = "请在私信抽牌\n" + msg
     return msg
 
 
 @plugin.handle({"停牌"}, {"user_id", "group_id", "send_group_message"})
 @blackjack.action(place)
 async def _(event: Event, session: Session):
     if session.round == 1:
         session.nextround()
         result = f"请{session.p2_nickname}抽牌|停牌|双倍停牌"
     else:
         result = blackjack_end(session)
-    await event.send_group_message(session.group_id, plugin.build_result(result))
+    await event.send_group_message(session.group_id, build_result(result))
 
 
 @plugin.handle({"双倍停牌"}, {"user_id", "group_id"})
 @blackjack.action(place)
 async def _(event: Event, session: Session):
     session.double_bet()
     hand, pt = blackjack_hit(session)
     if session.round > 1:
         return blackjack_end(session)
     session.nextround()
     msg = f"你的手牌：\n{poker_show(hand,'\n')}\n合计:{pt}点"
     if pt > 21:
-        await event.send_group_message(session.group_id, plugin.build_result(session.end(msg)))
+        await event.send_group_message(session.group_id, build_result(session.end(msg)))
     else:
-        await event.send_group_message(session.group_id, plugin.build_result(f"请{session.p2_nickname}{blackjack.action_tip}"))
+        await event.send_group_message(session.group_id, build_result(f"请{session.p2_nickname}{blackjack.action_tip}"))
         return msg
 
 
 western_duel = Game("西部对战", "装弹|开枪|闪避|闪避开枪|预判开枪")
 
 
 @plugin.handle({"西部对战"}, {"user_id", "group_id", "at"})
@@ -749,15 +749,15 @@
     session.nextround()
     session.data[MAG] += 1
     session.data[MAG] = min(session.data["MAG2"], 6)
     card = session.data["card"]
     if event.user_id == session.p1_uid:
         await event.send_group_message(
             session.group_id,
-            plugin.build_result(f"{session.p1_nickname}已行动，请{session.p2_nickname}开始行动。"),
+            build_result(f"{session.p1_nickname}已行动，请{session.p2_nickname}开始行动。"),
         )
         return tip
     if card in {"开枪", "闪枪"}:
         session.win = session.p1_uid
         return session.end(tip)
     return tip + "\n本轮平局。"
 
@@ -772,15 +772,15 @@
         return "行动失败。你的子弹不足"
     session.nextround()
     session.data[MAG] -= 1
     card = session.data["card"]
     if event.user_id == session.p1_uid:
         await event.send_group_message(
             session.group_id,
-            plugin.build_result(f"{session.p1_nickname}已行动，请{session.p2_nickname}开始行动。"),
+            build_result(f"{session.p1_nickname}已行动，请{session.p2_nickname}开始行动。"),
         )
         return tip
     if card == "闪枪":
         session.win = session.p1_uid
         return session.end(tip)
     if card in {"装弹", "预判开枪"}:
         session.win = session.p2_uid
@@ -795,15 +795,15 @@
     if not MAG:
         return tip
     session.nextround()
     card = session.data["card"]
     if event.user_id == session.p1_uid:
         await event.send_group_message(
             session.group_id,
-            plugin.build_result(f"{session.p1_nickname}已行动，请{session.p2_nickname}开始行动。"),
+            build_result(f"{session.p1_nickname}已行动，请{session.p2_nickname}开始行动。"),
         )
         return tip
     if card == "预判开枪":
         session.win = session.p1_uid
         return session.end(tip)
     return tip + "\n本轮平局。"
 
@@ -818,15 +818,15 @@
         return "行动失败。你的子弹不足"
     session.nextround()
     session.data[MAG] -= 1
     card = session.data["card"]
     if event.user_id == session.p1_uid:
         await event.send_group_message(
             session.group_id,
-            plugin.build_result(f"{session.p1_nickname}已行动，请{session.p2_nickname}开始行动。"),
+            build_result(f"{session.p1_nickname}已行动，请{session.p2_nickname}开始行动。"),
         )
         return tip
     if card == "预判开枪":
         session.win = session.p1_uid
         return session.end(tip)
     if card in {"装弹", "开枪"}:
         session.win = session.p2_uid
@@ -844,15 +844,15 @@
         return "行动失败。你的子弹不足"
     session.nextround()
     session.data[MAG] -= 1
     card = session.data["card"]
     if not card:
         await event.send_group_message(
             session.group_id,
-            plugin.build_result(f"{session.p1_nickname}已行动，请{session.p2_nickname}开始行动。"),
+            build_result(f"{session.p1_nickname}已行动，请{session.p2_nickname}开始行动。"),
         )
         return tip
     if card == "开枪":
         session.win = session.p1_uid
         return session.end(tip)
     if card in {"闪避", "闪枪"}:
         session.win = session.p2_uid
```

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/core.py` & `clovers_leafgame-0.1.9/clovers_leafgame/modules/game/core.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/fortress/core.py` & `clovers_leafgame-0.1.9/clovers_leafgame/modules/game/fortress/core.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/__init__.py` & `clovers_leafgame-0.1.9/clovers_leafgame/modules/game/horse_race/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/Stand.json` & `clovers_leafgame-0.1.9/clovers_leafgame/modules/game/horse_race/event_library/Stand.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json` & `clovers_leafgame-0.1.9/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json` & `clovers_leafgame-0.1.9/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json` & `clovers_leafgame-0.1.9/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json` & `clovers_leafgame-0.1.9/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json` & `clovers_leafgame-0.1.9/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json` & `clovers_leafgame-0.1.9/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json` & `clovers_leafgame-0.1.9/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json` & `clovers_leafgame-0.1.9/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json` & `clovers_leafgame-0.1.9/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/horse.py` & `clovers_leafgame-0.1.9/clovers_leafgame/modules/game/horse_race/horse.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/start.py` & `clovers_leafgame-0.1.9/clovers_leafgame/modules/game/horse_race/start.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/tools.py` & `clovers_leafgame-0.1.9/clovers_leafgame/modules/game/tools.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/market/__init__.py` & `clovers_leafgame-0.1.9/clovers_leafgame/modules/market/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/prop/__init__.py` & `clovers_leafgame-0.1.9/clovers_leafgame/modules/prop/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import random
 import asyncio
 from collections import Counter
+from clovers.core.plugin import Plugin
 from clovers_leafgame.core.clovers import Event, Check
 from clovers_leafgame.main import plugin, manager
 from clovers_leafgame.item import Prop, GOLD, STD_GOLD
 from .core import usage, gacha, AIR_PACK, RED_PACKET
 from clovers_leafgame.output import prop_card, bank_card
 from .output import report_card
 
@@ -244,19 +245,20 @@
     group_id = event.group_id
     user = manager.data.user(user_id)
     if user.bank[prop.id] < 1:
         return f"使用失败，你没有足够的{prop.name}"
     group_id = event.group_id
     rate = 1
 
-    @plugin.temp_handle(f"{user_id} {group_id}", extra_args={"user_id", "group_id"}, timeout=120)
-    async def _(event: Event, finish):
+    @plugin.temp_handle(f"{user_id} {group_id}", extra_args={"user_id", "group_id"}, timeout=60)
+    async def _(event: Event, finish: Plugin.Finish):
         if event.user_id != user_id or event.group_id != group_id:
             return
-        if event.raw_command == "取消":
+        command = event.raw_command
+        if command == "取消":
             finish()
             if rate == 1:
                 return f"你取消了恶魔轮盘"
 
             def rate_times_bank(bank: Counter, rate: int):
                 for k in bank.keys():
                     bank[k] *= rate
@@ -268,35 +270,37 @@
             for account_id in user.accounts_map.values():
                 account = manager.data.account_dict[account_id]
                 rate_times_bank(account.bank, rate)
                 counter += account.bank
             user.bank[STD_GOLD.id] += manager.stock_value(user.invest) * rate
 
             return ["这是你获得的道具", manager.info_card([prop_card(manager.props_data(counter))], user_id)]
+        elif command == "开枪":
+            finish.delay(60)
 
-        if event.raw_command != "开枪":
-            return
-
-        async def result():
-            bullet_lst = [0, 0, 0, 0, 0, 0]
-            for i in random.sample([0, 1, 2, 3, 4, 5], 3):
-                bullet_lst[i] = 1
-            index = random.randint(0, 5)
-            yield f"子弹列表{" ".join(str(x) for x in bullet_lst)}，你中了第{index+1}发子弹。"
-            await asyncio.sleep(0.5)
-            nonlocal rate
-            if bullet_lst[index] == 1:
-                if rate == 1:
-                    manager.data.cancel_user(user_id)
-                    finish()
-                    yield "砰！一团火从枪口喷出，你从这个世界上消失了。"
-                    return
-                rate //= 2
-                msg = "砰！一团火从枪口喷出...你被救活了..."
-            else:
-                rate *= 2
-                msg = "咔！你活了下来..."
-            yield msg + f"\n当前倍率：{rate}\n请继续开枪，或者取消。"
+            async def result():
+                bullet_lst = [0, 0, 0, 0, 0, 0]
+                for i in random.sample([0, 1, 2, 3, 4, 5], 3):
+                    bullet_lst[i] = 1
+                index = random.randint(0, 5)
+                yield f"子弹列表{" ".join(str(x) for x in bullet_lst)}，你中了第{index+1}发子弹。"
+                await asyncio.sleep(0.5)
+                nonlocal rate
+                if bullet_lst[index] == 1:
+                    if rate == 1:
+                        manager.data.cancel_user(user_id)
+                        finish()
+                        yield "砰！一团火从枪口喷出，你从这个世界上消失了。"
+                        return
+                    rate //= 2
+                    msg = "砰！一团火从枪口喷出...你被救活了..."
+                else:
+                    rate *= 2
+                    msg = "咔！你活了下来..."
+                yield msg + f"\n当前倍率：{rate}\n请继续开枪，或者取消。"
 
-        return result()
+            return result()
+        elif command.startswith(("群金库存", "群金库取", "发红包", "送道具", "使用道具")):
+            finish()
+            return "账户锁定中断，恶魔轮盘已取消。"
 
     return "你手中的左轮枪已经装好了子弹，请开枪，或者取消。"
```

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/prop/core.py` & `clovers_leafgame-0.1.9/clovers_leafgame/modules/prop/core.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/prop/output.py` & `clovers_leafgame-0.1.9/clovers_leafgame/modules/prop/output.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/prop/props_library.json` & `clovers_leafgame-0.1.9/clovers_leafgame/modules/prop/props_library.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970238095238095%*

 * *Differences: {"'0215'": "{'intro': '向自己开枪。如果你足够幸运躲过一劫，那么你所有账户的金币与股票都将翻倍。\\n如果你不幸中弹,你将会在这个世界上消失。'}"}*

```diff
@@ -3,15 +3,15 @@
         "color": "#85200C",
         "intro": "\u628a\u4f60\u7684\u4e2a\u4eba\u6570\u636e\u56de\u6eaf\u5230\u5230\u4efb\u610f\u65f6\u95f4\u8282\u70b9\u3002\n\u53ef\u56de\u6eaf\u7684\u65f6\u95f4\u8282\u70b9\u6709\u591a\u5c11\u53d6\u51b3\u4e8e\u670d\u52a1\u5668\u5907\u4efd\u8bbe\u7f6e",
         "name": "\u7eef\u7ea2\u8ff7\u96fe\u4e4b\u4e66",
         "tip": "\u673a\u5668\u4ebabug\u7814\u7a76\u4e2d\u5fc3"
     },
     "0215": {
         "color": "#0C343D",
-        "intro": "\u4f60\u53ef\u4ee5\u5bf9\u81ea\u5df1\u5f00\u4e00\u67aa\uff0c\u5982\u679c\u4f60\u8db3\u591f\u5e78\u8fd0\u8eb2\u8fc7\u4e00\u52ab\uff0c\u90a3\u4e48\u4f60\u7684\u540d\u4e0b\u6240\u6709\u8d26\u6237\u7684\u91d1\u5e01\u4e0e\u80a1\u7968\u51c0\u503c\u90fd\u5c06\u7ffb\u500d\u3002\n\u5982\u679c\u4f60\u4e0d\u5e78\u4e2d\u5f39,\u4f60\u5c06\u4f1a\u5728\u8fd9\u4e2a\u4e16\u754c\u4e0a\u6d88\u5931\u3002",
+        "intro": "\u5411\u81ea\u5df1\u5f00\u67aa\u3002\u5982\u679c\u4f60\u8db3\u591f\u5e78\u8fd0\u8eb2\u8fc7\u4e00\u52ab\uff0c\u90a3\u4e48\u4f60\u6240\u6709\u8d26\u6237\u7684\u91d1\u5e01\u4e0e\u80a1\u7968\u90fd\u5c06\u7ffb\u500d\u3002\n\u5982\u679c\u4f60\u4e0d\u5e78\u4e2d\u5f39,\u4f60\u5c06\u4f1a\u5728\u8fd9\u4e2a\u4e16\u754c\u4e0a\u6d88\u5931\u3002",
         "name": "\u6076\u9b54\u8f6e\u76d8",
         "tip": "\u4e00\u628a\u7834\u65e7\u7684\u5de6\u8f6e\u67aa"
     },
     "1213": {
         "color": "#66CCFF",
         "intro": "\u6bcf\u79cd\u7a7a\u6c14\u5404\u83b7\u5f97\u4e00\u4e2a",
         "name": "\u7a7a\u6c14\u793c\u5305",
```

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/ranklist/__init__.py` & `clovers_leafgame-0.1.9/clovers_leafgame/modules/ranklist/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/ranklist/output.py` & `clovers_leafgame-0.1.9/clovers_leafgame/modules/ranklist/output.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/task/__init__.py` & `clovers_leafgame-0.1.9/clovers_leafgame/modules/task/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/output.py` & `clovers_leafgame-0.1.9/clovers_leafgame/output.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/clovers_leafgame/props_library.json` & `clovers_leafgame-0.1.9/clovers_leafgame/props_library.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/LICENSE` & `clovers_leafgame-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/README.md` & `clovers_leafgame-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8.post1/PKG-INFO` & `clovers_leafgame-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: clovers-leafgame
-Version: 0.1.8.post1
+Version: 0.1.9
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: clovers-apscheduler (>=0.1.4,<0.2.0)
-Requires-Dist: clovers[linecard,tools] (>=0.1.8,<0.2.0)
+Requires-Dist: clovers[linecard,tools] (>=0.1.9,<0.2.0)
 Requires-Dist: mplfinance (>=0.12.10b0,<0.13.0)
 Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
 <div align="center">
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: clovers-leafgame Version: 0.1.8.post1 Summary:
-Author: KarisAya Author-email: 1048827424@qq.com Requires-Python: >=3.12,<4.0
+Metadata-Version: 2.1 Name: clovers-leafgame Version: 0.1.9 Summary: Author:
+KarisAya Author-email: 1048827424@qq.com Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3 Requires-Dist: clovers-
 apscheduler (>=0.1.4,<0.2.0) Requires-Dist: clovers[linecard,tools]
-(>=0.1.8,<0.2.0) Requires-Dist: mplfinance (>=0.12.10b0,<0.13.0) Requires-Dist:
+(>=0.1.9,<0.2.0) Requires-Dist: mplfinance (>=0.12.10b0,<0.13.0) Requires-Dist:
 pydantic (>=2.7.0,<3.0.0) Description-Content-Type: text/markdown
   # clovers-leafgame _â¨ æ¹èª [nonebot_plugin_russian](https://github.com/
    HibiKier/nonebot_plugin_russian) å [nonebot_plugin_horserace](https://
  github.com/shinianj/nonebot_plugin_horserace) çå°æ¸¸æåé â¨_[python]
                         _[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
 ## ð¿ å®è£ ```bash pip install clovers_leafgame ``` ## âï¸ éç½® å¨
 clovers éç½®æä»¶åæéæ·»å ä¸é¢çéç½®é¡¹ ```toml
```

