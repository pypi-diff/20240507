# Comparing `tmp/nonebot_plugin_mc_server_status-0.2.7.tar.gz` & `tmp/nonebot_plugin_mc_server_status-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mc_server_status-0.2.7.tar", max compression
+gzip compressed data, was "nonebot_plugin_mc_server_status-0.2.9.tar", max compression
```

## Comparing `nonebot_plugin_mc_server_status-0.2.7.tar` & `nonebot_plugin_mc_server_status-0.2.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     6882 2023-01-20 14:59:35.735943 nonebot_plugin_mc_server_status-0.2.7/nonebot_plugin_mc_server_status/__init__.py
--rw-r--r--   0        0        0     3873 2023-01-16 14:08:30.053854 nonebot_plugin_mc_server_status-0.2.7/nonebot_plugin_mc_server_status/config.py
--rw-r--r--   0        0        0      938 2023-01-20 14:59:57.526747 nonebot_plugin_mc_server_status-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     2521 2023-01-20 14:59:52.239137 nonebot_plugin_mc_server_status-0.2.7/README.md
--rw-r--r--   0        0        0     3354 1970-01-01 00:00:00.000000 nonebot_plugin_mc_server_status-0.2.7/setup.py
--rw-r--r--   0        0        0     3476 1970-01-01 00:00:00.000000 nonebot_plugin_mc_server_status-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     6944 2023-02-11 07:05:04.329046 nonebot_plugin_mc_server_status-0.2.9/nonebot_plugin_mc_server_status/__init__.py
+-rw-r--r--   0        0        0     3909 2023-01-24 15:20:25.794721 nonebot_plugin_mc_server_status-0.2.9/nonebot_plugin_mc_server_status/config.py
+-rw-r--r--   0        0        0      938 2023-02-11 07:06:01.320312 nonebot_plugin_mc_server_status-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     2759 2023-02-11 07:05:55.307038 nonebot_plugin_mc_server_status-0.2.9/README.md
+-rw-r--r--   0        0        0     3594 1970-01-01 00:00:00.000000 nonebot_plugin_mc_server_status-0.2.9/setup.py
+-rw-r--r--   0        0        0     3706 1970-01-01 00:00:00.000000 nonebot_plugin_mc_server_status-0.2.9/PKG-INFO
```

### Comparing `nonebot_plugin_mc_server_status-0.2.7/nonebot_plugin_mc_server_status/__init__.py` & `nonebot_plugin_mc_server_status-0.2.9/nonebot_plugin_mc_server_status/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from re import findall
 from mcstatus import BedrockServer, JavaServer
-from nonebot import on_fullmatch, on_regex
+from nonebot import on_command, on_regex
 from nonebot.adapters.onebot.v11 import (
     MessageSegment as MS,
     Bot,
     Message,
     GroupMessageEvent,
     MessageEvent,
 )
@@ -17,34 +17,34 @@
 from io import BytesIO
 from typing import Union
 
 __plugin_meta__ = PluginMetadata(
     name="MC服务器查询插件",
     description="如名",
     usage=f"""插件命令如下：
-信息  # 字面意思
+信息  # 字面意思，需要加命令前缀，默认/
+信息数据  # 查看已启用群以及服务器信息，需要加命令前缀，默认/
 添加服务器  # 字面意思
 删除服务器  # 字面意思
-信息数据  # 查看已启用群以及服务器信息
 """,
 )
 
 
 async def group_check(event: GroupMessageEvent, bot: Bot) -> bool:
     return event.group_id in var.group_list and bot == var.handle_bot
 
 
 async def admin_check(event: MessageEvent, bot: Bot) -> bool:
     return bot == var.handle_bot and event.user_id == pc.mc_status_admin_qqnum
 
 
-xinxi = on_fullmatch("信息", rule=group_check)
+xinxi = on_command("信息", rule=group_check)
+list_all = on_command("信息数据", rule=admin_check)
 add_server = on_regex(r"^添加服务器\s*((\d+)\s+(\S+)\s+(\S+)\s+(\S+))?", rule=admin_check)
 del_server = on_regex(r"^删除服务器\s*((\d+)\s+(\S+))?", rule=admin_check)
-list_all = on_fullmatch("信息数据", rule=admin_check)
 
 
 @xinxi.handle()
 async def handle_xinxi(event: GroupMessageEvent):
     group = event.group_id
     task_list = []
     for server_name in var.group_list[group]:
```

### Comparing `nonebot_plugin_mc_server_status-0.2.7/nonebot_plugin_mc_server_status/config.py` & `nonebot_plugin_mc_server_status-0.2.9/nonebot_plugin_mc_server_status/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                 var.handle_bot = bot
 
         # 没bot连就直接给
         else:
             var.handle_bot = bot
 
     # 不写就给第一个连的
-    elif not var.handle_bot:
+    elif not pc.mc_status_bot_qqnum_list and not var.handle_bot:
         var.handle_bot = bot
 
 
 # qq机器人断开时执行
 @driver.on_bot_disconnect
 async def on_bot_disconnect(bot: Bot):
     # 判断掉线的是否为handle bot
```

### Comparing `nonebot_plugin_mc_server_status-0.2.7/pyproject.toml` & `nonebot_plugin_mc_server_status-0.2.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_mc_server_status"
-version = "0.2.7"
+version = "0.2.9"
 description = "Nonebot2查询MC服务器在线信息插件"
 authors = ["nikissXI <1299577815@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_mc_server_status"}]
 homepage = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_mc_server_status"
 repository = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_mc_server_status"
```

### Comparing `nonebot_plugin_mc_server_status-0.2.7/README.md` & `nonebot_plugin_mc_server_status-0.2.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -44,26 +44,34 @@
 ```bash
 # 管理员的QQ号（别问我为什么要另外写）
 mc_status_admin_qqnum = 114514
 
 # 可选配置
 # 机器人的QQ号列表，如果有多个bot连接，会按照填写的list，左边的机器人QQ优先级最高 1234 > 5678 > 6666，会自动切换
 # 如果不填该配置则由第一个连上的bot响应
-tutu_bot_qqnum_list = [1234,5678,6666]
+tutu_bot_qqnum_list = [1234, 5678, 6666]
 ```
 
 ## 插件命令  
 | 指令 | 说明 |
 |:-----:|:----:|
-| 信息|所有人都能使用，查看当前群添加的服务器状态|
-| 添加服务器|字面意思，bot超级管理员用|
+| 信息|所有人都能使用，查看当前群添加的服务器状态，需要加命令前缀，默认/|
+| 信息数据|查看已添加的群和服务器信息，bot超级管理员用，需要加命令前缀，默认/|
+| 添加服务器|字面意思，bot超级管理员用，一个群可以添加多个服务器|
 | 删除服务器|字面意思，bot超级管理员用|
-| 信息数据|查看已添加的群和服务器信息，bot超级管理员用|
 
 ## 更新日志
+### 2023/2/11 \[v0.2.9]
+
+* 信息和信息数据的增加命令前缀
+
+### 2023/1/24 \[v0.2.8]
+
+* 修复多bot处理bug
+
 ### 2023/1/20 \[v0.2.7]
 
 * gocq插件版不支持base64图片发送，改为BytesIO发送服务器图标
 
 ### 2023/1/17 \[v0.2.4]
 
 * 又忘记删东西导致无法运行，已修复
```

#### html2text {}

```diff
@@ -12,18 +12,21 @@
 æ·»å äºæå¡å¨ä¿¡æ¯åï¼ä¼å¨botæ ¹ç®å½ä¸çdataç®å½åå»ºä¸ä¸ªmc_status_data.jsonæä»¶ï¼ç¨äºå­å¨æä»¶ä¿¡æ¯
 å¨botå¯¹åºç.envæä»¶ä¿®æ¹ ```bash #
 ç®¡çåçQQå·ï¼å«é®æä¸ºä»ä¹è¦å¦å¤åï¼ mc_status_admin_qqnum =
 114514 # å¯ééç½® #
 æºå¨äººçQQå·åè¡¨ï¼å¦ææå¤ä¸ªbotè¿æ¥ï¼ä¼æç§å¡«åçlistï¼å·¦è¾¹çæºå¨äººQQä¼åçº§æé«
 1234 > 5678 > 6666ï¼ä¼èªå¨åæ¢ #
 å¦æä¸å¡«è¯¥éç½®åç±ç¬¬ä¸ä¸ªè¿ä¸çbotååº tutu_bot_qqnum_list =
-[1234,5678,6666] ``` ## æä»¶å½ä»¤ | æä»¤ | è¯´æ | |:-----:|:----:| |
-ä¿¡æ¯|ææäººé½è½ä½¿ç¨ï¼æ¥çå½åç¾¤æ·»å çæå¡å¨ç¶æ| |
-æ·»å æå¡å¨|å­é¢ææï¼botè¶çº§ç®¡çåç¨| |
-å é¤æå¡å¨|å­é¢ææï¼botè¶çº§ç®¡çåç¨| |
-ä¿¡æ¯æ°æ®|æ¥çå·²æ·»å çç¾¤åæå¡å¨ä¿¡æ¯ï¼botè¶çº§ç®¡çåç¨|
-## æ´æ°æ¥å¿ ### 2023/1/20 \[v0.2.7] *
+[1234, 5678, 6666] ``` ## æä»¶å½ä»¤ | æä»¤ | è¯´æ | |:-----:|:----:| |
+ä¿¡æ¯|ææäººé½è½ä½¿ç¨ï¼æ¥çå½åç¾¤æ·»å çæå¡å¨ç¶æï¼éè¦å å½ä»¤åç¼ï¼é»è®¤/
+| |
+ä¿¡æ¯æ°æ®|æ¥çå·²æ·»å çç¾¤åæå¡å¨ä¿¡æ¯ï¼botè¶çº§ç®¡çåç¨ï¼éè¦å å½ä»¤åç¼ï¼é»è®¤/
+| |
+æ·»å æå¡å¨|å­é¢ææï¼botè¶çº§ç®¡çåç¨ï¼ä¸ä¸ªç¾¤å¯ä»¥æ·»å å¤ä¸ªæå¡å¨|
+| å é¤æå¡å¨|å­é¢ææï¼botè¶çº§ç®¡çåç¨| ## æ´æ°æ¥å¿ ###
+2023/2/11 \[v0.2.9] * ä¿¡æ¯åä¿¡æ¯æ°æ®çå¢å å½ä»¤åç¼ ### 2023/1/24
+\[v0.2.8] * ä¿®å¤å¤botå¤çbug ### 2023/1/20 \[v0.2.7] *
 gocqæä»¶çä¸æ¯æbase64å¾çåéï¼æ¹ä¸ºBytesIOåéæå¡å¨å¾æ 
 ### 2023/1/17 \[v0.2.4] * åå¿è®°å ä¸è¥¿å¯¼è´æ æ³è¿è¡ï¼å·²ä¿®å¤ ###
 2023/1/16 \[v0.2.3] * æä½pythonçæ¬å¼å®¹è³3.8 ### 2023/1/15 \[v0.2.2] *
 ä¼åå¤boté»è¾ï¼æºå¨äººqqå·éç½®æ¹ä¸ºå¯é ### 2023/1/15 \[v0.2.1] *
 æä»¶éæ
```

### Comparing `nonebot_plugin_mc_server_status-0.2.7/setup.py` & `nonebot_plugin_mc_server_status-0.2.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 install_requires = \
 ['mcstatus>=10.0.0,<11.0.0',
  'nonebot-adapter-onebot>=2.0.0,<3.0.0',
  'nonebot2>=2.0.0rc1,<3.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-mc-server-status',
-    'version': '0.2.7',
+    'version': '0.2.9',
     'description': 'Nonebot2查询MC服务器在线信息插件',
-    'long_description': '<p align="center">\n  <a href="https://v2.nonebot.dev/store">\n  <img src="https://user-images.githubusercontent.com/44545625/209862575-acdc9feb-3c76-471d-ad89-cc78927e5875.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n</p>\n\n<div align="center">\n\n# nonebot_plugin_mc_server_status\n\n_✨ Nonebot2查询MC服务器在线信息插件 ✨_\n\n</div>\n\n<p align="center">\n  <a href="https://opensource.org/licenses/MIT">\n    <img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="license">\n  </a>\n  <a href="https://v2.nonebot.dev/">\n    <img src="https://img.shields.io/static/v1?label=nonebot&message=v2rc1%2B&color=green" alt="nonebot2">\n  </a>\n  <img src="https://img.shields.io/static/v1?label=python+&message=3.8%2B&color=blue" alt="python">\n</p>\n\n## 简介\n使用mcstatus库，支持Java和Bedrock服务器的服务器查询。   \n\n<img width="300" src="https://raw.githubusercontent.com/nikissXI/nonebot_plugins/main/nonebot_plugin_mc_server_status/readme_img/xinxi.jpg"/>\n\n## 安装\n\n使用nb-cli安装\n```bash\nnb plugin install nonebot_plugin_mc_server_status\n```\n\n或者  \n直接把插件clone下来放进去plugins文件夹，记得把依赖装上 pip install mcstatus  \n\n## 使用\n\n添加了服务器信息后，会在bot根目录下的data目录创建一个mc_status_data.json文件，用于存储插件信息  \n在bot对应的.env文件修改\n\n```bash\n# 管理员的QQ号（别问我为什么要另外写）\nmc_status_admin_qqnum = 114514\n\n# 可选配置\n# 机器人的QQ号列表，如果有多个bot连接，会按照填写的list，左边的机器人QQ优先级最高 1234 > 5678 > 6666，会自动切换\n# 如果不填该配置则由第一个连上的bot响应\ntutu_bot_qqnum_list = [1234,5678,6666]\n```\n\n## 插件命令  \n| 指令 | 说明 |\n|:-----:|:----:|\n| 信息|所有人都能使用，查看当前群添加的服务器状态|\n| 添加服务器|字面意思，bot超级管理员用|\n| 删除服务器|字面意思，bot超级管理员用|\n| 信息数据|查看已添加的群和服务器信息，bot超级管理员用|\n\n## 更新日志\n### 2023/1/20 \\[v0.2.7]\n\n* gocq插件版不支持base64图片发送，改为BytesIO发送服务器图标\n\n### 2023/1/17 \\[v0.2.4]\n\n* 又忘记删东西导致无法运行，已修复\n\n### 2023/1/16 \\[v0.2.3]\n\n* 最低python版本兼容至3.8\n\n### 2023/1/15 \\[v0.2.2]\n\n* 优化多bot逻辑，机器人qq号配置改为可选\n\n### 2023/1/15 \\[v0.2.1]\n\n* 插件重构',
+    'long_description': '<p align="center">\n  <a href="https://v2.nonebot.dev/store">\n  <img src="https://user-images.githubusercontent.com/44545625/209862575-acdc9feb-3c76-471d-ad89-cc78927e5875.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n</p>\n\n<div align="center">\n\n# nonebot_plugin_mc_server_status\n\n_✨ Nonebot2查询MC服务器在线信息插件 ✨_\n\n</div>\n\n<p align="center">\n  <a href="https://opensource.org/licenses/MIT">\n    <img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="license">\n  </a>\n  <a href="https://v2.nonebot.dev/">\n    <img src="https://img.shields.io/static/v1?label=nonebot&message=v2rc1%2B&color=green" alt="nonebot2">\n  </a>\n  <img src="https://img.shields.io/static/v1?label=python+&message=3.8%2B&color=blue" alt="python">\n</p>\n\n## 简介\n使用mcstatus库，支持Java和Bedrock服务器的服务器查询。   \n\n<img width="300" src="https://raw.githubusercontent.com/nikissXI/nonebot_plugins/main/nonebot_plugin_mc_server_status/readme_img/xinxi.jpg"/>\n\n## 安装\n\n使用nb-cli安装\n```bash\nnb plugin install nonebot_plugin_mc_server_status\n```\n\n或者  \n直接把插件clone下来放进去plugins文件夹，记得把依赖装上 pip install mcstatus  \n\n## 使用\n\n添加了服务器信息后，会在bot根目录下的data目录创建一个mc_status_data.json文件，用于存储插件信息  \n在bot对应的.env文件修改\n\n```bash\n# 管理员的QQ号（别问我为什么要另外写）\nmc_status_admin_qqnum = 114514\n\n# 可选配置\n# 机器人的QQ号列表，如果有多个bot连接，会按照填写的list，左边的机器人QQ优先级最高 1234 > 5678 > 6666，会自动切换\n# 如果不填该配置则由第一个连上的bot响应\ntutu_bot_qqnum_list = [1234, 5678, 6666]\n```\n\n## 插件命令  \n| 指令 | 说明 |\n|:-----:|:----:|\n| 信息|所有人都能使用，查看当前群添加的服务器状态，需要加命令前缀，默认/|\n| 信息数据|查看已添加的群和服务器信息，bot超级管理员用，需要加命令前缀，默认/|\n| 添加服务器|字面意思，bot超级管理员用，一个群可以添加多个服务器|\n| 删除服务器|字面意思，bot超级管理员用|\n\n## 更新日志\n### 2023/2/11 \\[v0.2.9]\n\n* 信息和信息数据的增加命令前缀\n\n### 2023/1/24 \\[v0.2.8]\n\n* 修复多bot处理bug\n\n### 2023/1/20 \\[v0.2.7]\n\n* gocq插件版不支持base64图片发送，改为BytesIO发送服务器图标\n\n### 2023/1/17 \\[v0.2.4]\n\n* 又忘记删东西导致无法运行，已修复\n\n### 2023/1/16 \\[v0.2.3]\n\n* 最低python版本兼容至3.8\n\n### 2023/1/15 \\[v0.2.2]\n\n* 优化多bot逻辑，机器人qq号配置改为可选\n\n### 2023/1/15 \\[v0.2.1]\n\n* 插件重构',
     'author': 'nikissXI',
     'author_email': '1299577815@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_mc_server_status',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_mc_server_status'] package_data = \ {'': ['*']}
 install_requires = \ ['mcstatus>=10.0.0,<11.0.0', 'nonebot-adapter-
 onebot>=2.0.0,<3.0.0', 'nonebot2>=2.0.0rc1,<3.0.0'] setup_kwargs = { 'name':
-'nonebot-plugin-mc-server-status', 'version': '0.2.7', 'description':
+'nonebot-plugin-mc-server-status', 'version': '0.2.9', 'description':
 'Nonebot2æ¥è¯¢MCæå¡å¨å¨çº¿ä¿¡æ¯æä»¶', 'long_description': '
                           \n _\_n_ _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]\n
 \n\n
                  \n\n# nonebot_plugin_mc_server_status\n\n_â¨
              Nonebot2æ¥è¯¢MCæå¡å¨å¨çº¿ä¿¡æ¯æä»¶ â¨_\n\n
 \n\n
               \n _\_n_ _[_l_i_c_e_n_s_e_]_\_n_ \n _\_n_ _[_n_o_n_e_b_o_t_2_]_\_n_ \n [python]\n
@@ -21,20 +21,25 @@
 ä½¿ç¨\n\næ·»å äºæå¡å¨ä¿¡æ¯åï¼ä¼å¨botæ ¹ç®å½ä¸çdataç®å½åå»ºä¸ä¸ªmc_status_data.jsonæä»¶ï¼ç¨äºå­å¨æä»¶ä¿¡æ¯
 \nå¨botå¯¹åºç.envæä»¶ä¿®æ¹\n\n```bash\n#
 ç®¡çåçQQå·ï¼å«é®æä¸ºä»ä¹è¦å¦å¤åï¼\nmc_status_admin_qqnum =
 114514\n\n# å¯ééç½®\n#
 æºå¨äººçQQå·åè¡¨ï¼å¦ææå¤ä¸ªbotè¿æ¥ï¼ä¼æç§å¡«åçlistï¼å·¦è¾¹çæºå¨äººQQä¼åçº§æé«
 1234 > 5678 > 6666ï¼ä¼èªå¨åæ¢\n#
 å¦æä¸å¡«è¯¥éç½®åç±ç¬¬ä¸ä¸ªè¿ä¸çbotååº\ntutu_bot_qqnum_list =
-[1234,5678,6666]\n```\n\n## æä»¶å½ä»¤ \n| æä»¤ | è¯´æ |\n|:-----:|:----:
-|\n| ä¿¡æ¯|ææäººé½è½ä½¿ç¨ï¼æ¥çå½åç¾¤æ·»å çæå¡å¨ç¶æ|\n|
-æ·»å æå¡å¨|å­é¢ææï¼botè¶çº§ç®¡çåç¨|\n|
-å é¤æå¡å¨|å­é¢ææï¼botè¶çº§ç®¡çåç¨|\n|
-ä¿¡æ¯æ°æ®|æ¥çå·²æ·»å çç¾¤åæå¡å¨ä¿¡æ¯ï¼botè¶çº§ç®¡çåç¨|\n\n##
-æ´æ°æ¥å¿\n### 2023/1/20 \\[v0.2.7]\n\n*
+[1234, 5678, 6666]\n```\n\n## æä»¶å½ä»¤ \n| æä»¤ | è¯´æ |\n|:-----:|:---
+-:|\n|
+ä¿¡æ¯|ææäººé½è½ä½¿ç¨ï¼æ¥çå½åç¾¤æ·»å çæå¡å¨ç¶æï¼éè¦å å½ä»¤åç¼ï¼é»è®¤/
+|\n|
+ä¿¡æ¯æ°æ®|æ¥çå·²æ·»å çç¾¤åæå¡å¨ä¿¡æ¯ï¼botè¶çº§ç®¡çåç¨ï¼éè¦å å½ä»¤åç¼ï¼é»è®¤/
+|\n|
+æ·»å æå¡å¨|å­é¢ææï¼botè¶çº§ç®¡çåç¨ï¼ä¸ä¸ªç¾¤å¯ä»¥æ·»å å¤ä¸ªæå¡å¨|\n|
+å é¤æå¡å¨|å­é¢ææï¼botè¶çº§ç®¡çåç¨|\n\n## æ´æ°æ¥å¿\n###
+2023/2/11 \\[v0.2.9]\n\n* ä¿¡æ¯åä¿¡æ¯æ°æ®çå¢å å½ä»¤åç¼\n\n###
+2023/1/24 \\[v0.2.8]\n\n* ä¿®å¤å¤botå¤çbug\n\n### 2023/1/20 \\
+[v0.2.7]\n\n*
 gocqæä»¶çä¸æ¯æbase64å¾çåéï¼æ¹ä¸ºBytesIOåéæå¡å¨å¾æ \n\n###
 2023/1/17 \\[v0.2.4]\n\n*
 åå¿è®°å ä¸è¥¿å¯¼è´æ æ³è¿è¡ï¼å·²ä¿®å¤\n\n### 2023/1/16 \\
 [v0.2.3]\n\n* æä½pythonçæ¬å¼å®¹è³3.8\n\n### 2023/1/15 \\[v0.2.2]\n\n*
 ä¼åå¤boté»è¾ï¼æºå¨äººqqå·éç½®æ¹ä¸ºå¯é\n\n### 2023/1/15 \\
 [v0.2.1]\n\n* æä»¶éæ', 'author': 'nikissXI', 'author_email':
 '1299577815@qq.com', 'maintainer': 'None', 'maintainer_email': 'None', 'url':
```

### Comparing `nonebot_plugin_mc_server_status-0.2.7/PKG-INFO` & `nonebot_plugin_mc_server_status-0.2.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mc-server-status
-Version: 0.2.7
+Version: 0.2.9
 Summary: Nonebot2查询MC服务器在线信息插件
 Home-page: https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_mc_server_status
 License: MIT
 Author: nikissXI
 Author-email: 1299577815@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -66,26 +66,34 @@
 ```bash
 # 管理员的QQ号（别问我为什么要另外写）
 mc_status_admin_qqnum = 114514
 
 # 可选配置
 # 机器人的QQ号列表，如果有多个bot连接，会按照填写的list，左边的机器人QQ优先级最高 1234 > 5678 > 6666，会自动切换
 # 如果不填该配置则由第一个连上的bot响应
-tutu_bot_qqnum_list = [1234,5678,6666]
+tutu_bot_qqnum_list = [1234, 5678, 6666]
 ```
 
 ## 插件命令  
 | 指令 | 说明 |
 |:-----:|:----:|
-| 信息|所有人都能使用，查看当前群添加的服务器状态|
-| 添加服务器|字面意思，bot超级管理员用|
+| 信息|所有人都能使用，查看当前群添加的服务器状态，需要加命令前缀，默认/|
+| 信息数据|查看已添加的群和服务器信息，bot超级管理员用，需要加命令前缀，默认/|
+| 添加服务器|字面意思，bot超级管理员用，一个群可以添加多个服务器|
 | 删除服务器|字面意思，bot超级管理员用|
-| 信息数据|查看已添加的群和服务器信息，bot超级管理员用|
 
 ## 更新日志
+### 2023/2/11 \[v0.2.9]
+
+* 信息和信息数据的增加命令前缀
+
+### 2023/1/24 \[v0.2.8]
+
+* 修复多bot处理bug
+
 ### 2023/1/20 \[v0.2.7]
 
 * gocq插件版不支持base64图片发送，改为BytesIO发送服务器图标
 
 ### 2023/1/17 \[v0.2.4]
 
 * 又忘记删东西导致无法运行，已修复
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-mc-server-status Version: 0.2.7
+Metadata-Version: 2.1 Name: nonebot-plugin-mc-server-status Version: 0.2.9
 Summary: Nonebot2æ¥è¯¢MCæå¡å¨å¨çº¿ä¿¡æ¯æä»¶ Home-page: https://
 github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_mc_server_status
 License: MIT Author: nikissXI Author-email: 1299577815@qq.com Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -26,18 +26,21 @@
 æ·»å äºæå¡å¨ä¿¡æ¯åï¼ä¼å¨botæ ¹ç®å½ä¸çdataç®å½åå»ºä¸ä¸ªmc_status_data.jsonæä»¶ï¼ç¨äºå­å¨æä»¶ä¿¡æ¯
 å¨botå¯¹åºç.envæä»¶ä¿®æ¹ ```bash #
 ç®¡çåçQQå·ï¼å«é®æä¸ºä»ä¹è¦å¦å¤åï¼ mc_status_admin_qqnum =
 114514 # å¯ééç½® #
 æºå¨äººçQQå·åè¡¨ï¼å¦ææå¤ä¸ªbotè¿æ¥ï¼ä¼æç§å¡«åçlistï¼å·¦è¾¹çæºå¨äººQQä¼åçº§æé«
 1234 > 5678 > 6666ï¼ä¼èªå¨åæ¢ #
 å¦æä¸å¡«è¯¥éç½®åç±ç¬¬ä¸ä¸ªè¿ä¸çbotååº tutu_bot_qqnum_list =
-[1234,5678,6666] ``` ## æä»¶å½ä»¤ | æä»¤ | è¯´æ | |:-----:|:----:| |
-ä¿¡æ¯|ææäººé½è½ä½¿ç¨ï¼æ¥çå½åç¾¤æ·»å çæå¡å¨ç¶æ| |
-æ·»å æå¡å¨|å­é¢ææï¼botè¶çº§ç®¡çåç¨| |
-å é¤æå¡å¨|å­é¢ææï¼botè¶çº§ç®¡çåç¨| |
-ä¿¡æ¯æ°æ®|æ¥çå·²æ·»å çç¾¤åæå¡å¨ä¿¡æ¯ï¼botè¶çº§ç®¡çåç¨|
-## æ´æ°æ¥å¿ ### 2023/1/20 \[v0.2.7] *
+[1234, 5678, 6666] ``` ## æä»¶å½ä»¤ | æä»¤ | è¯´æ | |:-----:|:----:| |
+ä¿¡æ¯|ææäººé½è½ä½¿ç¨ï¼æ¥çå½åç¾¤æ·»å çæå¡å¨ç¶æï¼éè¦å å½ä»¤åç¼ï¼é»è®¤/
+| |
+ä¿¡æ¯æ°æ®|æ¥çå·²æ·»å çç¾¤åæå¡å¨ä¿¡æ¯ï¼botè¶çº§ç®¡çåç¨ï¼éè¦å å½ä»¤åç¼ï¼é»è®¤/
+| |
+æ·»å æå¡å¨|å­é¢ææï¼botè¶çº§ç®¡çåç¨ï¼ä¸ä¸ªç¾¤å¯ä»¥æ·»å å¤ä¸ªæå¡å¨|
+| å é¤æå¡å¨|å­é¢ææï¼botè¶çº§ç®¡çåç¨| ## æ´æ°æ¥å¿ ###
+2023/2/11 \[v0.2.9] * ä¿¡æ¯åä¿¡æ¯æ°æ®çå¢å å½ä»¤åç¼ ### 2023/1/24
+\[v0.2.8] * ä¿®å¤å¤botå¤çbug ### 2023/1/20 \[v0.2.7] *
 gocqæä»¶çä¸æ¯æbase64å¾çåéï¼æ¹ä¸ºBytesIOåéæå¡å¨å¾æ 
 ### 2023/1/17 \[v0.2.4] * åå¿è®°å ä¸è¥¿å¯¼è´æ æ³è¿è¡ï¼å·²ä¿®å¤ ###
 2023/1/16 \[v0.2.3] * æä½pythonçæ¬å¼å®¹è³3.8 ### 2023/1/15 \[v0.2.2] *
 ä¼åå¤boté»è¾ï¼æºå¨äººqqå·éç½®æ¹ä¸ºå¯é ### 2023/1/15 \[v0.2.1] *
 æä»¶éæ
```

