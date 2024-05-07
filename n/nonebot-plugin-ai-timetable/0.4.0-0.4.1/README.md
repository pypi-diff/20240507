# Comparing `tmp/nonebot_plugin_ai_timetable-0.4.0.tar.gz` & `tmp/nonebot_plugin_ai_timetable-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ai_timetable-0.4.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_ai_timetable-0.4.1.tar", max compression
```

## Comparing `nonebot_plugin_ai_timetable-0.4.0.tar` & `nonebot_plugin_ai_timetable-0.4.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1065 2024-04-30 13:28:16.527808 nonebot_plugin_ai_timetable-0.4.0/LICENSE
--rw-r--r--   0        0        0    10826 2024-04-30 13:28:16.527808 nonebot_plugin_ai_timetable-0.4.0/README.md
--rw-r--r--   0        0        0     6237 2024-04-30 13:28:16.527808 nonebot_plugin_ai_timetable-0.4.0/nonebot_plugin_ai_timetable/__init__.py
--rw-r--r--   0        0        0      332 2024-04-30 13:28:16.527808 nonebot_plugin_ai_timetable-0.4.0/nonebot_plugin_ai_timetable/config.py
--rw-r--r--   0        0        0     6420 2024-04-30 13:28:16.527808 nonebot_plugin_ai_timetable-0.4.0/nonebot_plugin_ai_timetable/data_manager.py
--rw-r--r--   0        0        0     9714 2024-04-30 13:28:16.527808 nonebot_plugin_ai_timetable-0.4.0/nonebot_plugin_ai_timetable/manager.py
--rw-r--r--   0        0        0     2799 2024-04-30 13:28:16.527808 nonebot_plugin_ai_timetable-0.4.0/nonebot_plugin_ai_timetable/migrations/f67eb52d6a0f_init.py
--rw-r--r--   0        0        0     1774 2024-04-30 13:28:16.527808 nonebot_plugin_ai_timetable-0.4.0/nonebot_plugin_ai_timetable/model.py
--rw-r--r--   0        0        0     8203 2024-04-30 13:28:16.527808 nonebot_plugin_ai_timetable-0.4.0/nonebot_plugin_ai_timetable/reminder.py
--rw-r--r--   0        0        0      549 2024-04-30 13:28:16.527808 nonebot_plugin_ai_timetable-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    11637 1970-01-01 00:00:00.000000 nonebot_plugin_ai_timetable-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-07 11:19:16.247010 nonebot_plugin_ai_timetable-0.4.1/LICENSE
+-rw-r--r--   0        0        0    11222 2024-05-07 11:19:16.247010 nonebot_plugin_ai_timetable-0.4.1/README.md
+-rw-r--r--   0        0        0     6249 2024-05-07 11:19:16.247010 nonebot_plugin_ai_timetable-0.4.1/nonebot_plugin_ai_timetable/__init__.py
+-rw-r--r--   0        0        0      332 2024-05-07 11:19:16.247010 nonebot_plugin_ai_timetable-0.4.1/nonebot_plugin_ai_timetable/config.py
+-rw-r--r--   0        0        0     6582 2024-05-07 11:19:16.247010 nonebot_plugin_ai_timetable-0.4.1/nonebot_plugin_ai_timetable/data_manager.py
+-rw-r--r--   0        0        0     9908 2024-05-07 11:19:16.247010 nonebot_plugin_ai_timetable-0.4.1/nonebot_plugin_ai_timetable/manager.py
+-rw-r--r--   0        0        0     2799 2024-05-07 11:19:16.247010 nonebot_plugin_ai_timetable-0.4.1/nonebot_plugin_ai_timetable/migrations/f67eb52d6a0f_init.py
+-rw-r--r--   0        0        0     1774 2024-05-07 11:19:16.247010 nonebot_plugin_ai_timetable-0.4.1/nonebot_plugin_ai_timetable/model.py
+-rw-r--r--   0        0        0     8392 2024-05-07 11:19:16.247010 nonebot_plugin_ai_timetable-0.4.1/nonebot_plugin_ai_timetable/reminder.py
+-rw-r--r--   0        0        0      549 2024-05-07 11:19:16.247010 nonebot_plugin_ai_timetable-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    12033 1970-01-01 00:00:00.000000 nonebot_plugin_ai_timetable-0.4.1/PKG-INFO
```

### Comparing `nonebot_plugin_ai_timetable-0.4.0/LICENSE` & `nonebot_plugin_ai_timetable-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ai_timetable-0.4.0/README.md` & `nonebot_plugin_ai_timetable-0.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,79 +1,94 @@
-<p align="center">
-  <a href="https://nonebot.dev/"><img src="https://nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
-</p>
 <div align="center">
+  <a href="https://nonebot.dev/">
+    <img src="https://nonebot.dev/logo.png" width="200" height="200" alt="nonebot">
+  </a>
 
 # nonebot-plugin-ai-timetable
 
-✨*基于Nonebot2的对接小爱课程表的插件*✨
-  
-<a href="https://github.com/nonebot/nonebot2">
-  <img src="https://img.shields.io/badge/nonebot-v2-red" alt="nonebot">
-</a> 
-<a href="./LICENSE">
+✨ *基于Nonebot2的对接小爱课程表的插件* ✨
+
+
+  <a href="https://github.com/nonebot/nonebot2">
+    <img src="https://img.shields.io/badge/nonebot-v2-red" alt="nonebot">
+  </a>
+  <a href="./LICENSE">
     <img src="https://img.shields.io/github/license/maoxig/nonebot-plugin-ai-timetable" alt="license">
-</a>
-<a href="https://pypi.python.org/pypi/nonebot-plugin-ai-timetable">
+  </a>
+  <a href="https://pypi.python.org/pypi/nonebot-plugin-ai-timetable">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-ai-timetable" alt="pypi">
-</a>
-<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
-
-<div align="left">
+  </a>
+  <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+</div>
 
 ## 💿安装
 
 1. 通过`pip`或`nb`安装；
     - 使用nb(推荐)
   
        在机器人目录下命令行使用`nb plugin install nonebot_plugin_ai_timetable`
 
     - 使用pip:
   
       `pip plugin install nonebot_plugin_ai_timetable`
 
       然后在机器人`pyproject.toml`里的`plugins = []`列表追加`"nonebot_plugin_ai_timetable"`
 
-2. 数据存储使用[plugin-orm](https://github.com/nonebot/plugin-orm), 接入数据库，方便管理
+    - 使用其他包管理器：
 
-3. 第一次使用使用[plugin-orm](https://github.com/nonebot/plugin-orm)时，需要用`nb orm upgrade`升级数据库
+      根据包管理器的指令安装插件
+
+2. 数据存储使用[plugin-orm](https://github.com/nonebot/plugin-orm), 使用`nb orm upgrade`升级数据库
+
+> [!WARNING]
+> 第一次使用[plugin-orm](https://github.com/nonebot/plugin-orm)，或者插件定义的模型有所更新时，需要用`nb orm upgrade`升级数据库
 
 ## 📖简介
 
 1. 傻瓜式一键导入小爱课表，让你的bot实现小爱课表的功能
 
 2. 用户课表数据隔离，基于[plugin-rom](https://github.com/nonebot/plugin-orm), 接入数据库，无需担心课程时间冲突、不同学校课表不同等问题
 
 3. 适配多平台，即使是电报涩涩群也要好好学习！🥵🥵
 
 ## ⚙️插件配置
 
-这些配置都已设好默认值，如果想要修改配置，在机器人目录下的.env.*里面可以填写以下选项(可选)
+>[!NOTE] 可选的插件配置
+这些配置都已设好默认值，因此是可选的，如果想要修改配置，在机器人目录下的.env.*里面可以填写以下选项, 未来会考虑开放更多的配置项
 
 |         config          | type  | default |          example           | usage                                                                                                 |
 | :---------------------: | :---: | :-----: | :------------------------: | :---------------------------------------------------------------------------------------------------- |
 |      TIMETABLE_PIC      | bool  |  true   |    TIMETABLE_PIC=false     | 可选择某日课表以图片/文字发送，默认以图片发送(true)                                                   |
 | TIMETABLE_ALOCK_SOMEDAY |  int  |   22    | TIMETABLE_ALOCK_SOMEDAY=15 | 订阅某日课表的发送时间，必须是0-24的数字                                                              |
 |    TIMETABLE_ALOCK_8    |  int  |   21    |    TIMETABLE_ALOCK_8=16    | 订阅早八的发送时间，必须是0-24的数字.这里发送的都是第二天的，所以建议设置为18-23点                    |
 |   TIMETABLE_SEND_TIME   | float |   0.5   |   TIMETABLE_SEND_TIME=1    | 订阅课程提前发送的时间，单位是`小时`，可以是整数也可以是小数，建议不要设的太大，避免出现无法预料的bug |
 
+
 ## 💿依赖
-插件依赖会在安装时自动安装，如果安装失败，你可以按照以下指令手动再次安装
+
+> [!NOTE]
+> 插件依赖会在安装时自动安装，如果安装失败，你可以按照以下指令手动再次安装
+
 ```python
 nb plugin install nonebot_plugin_htmlrender
 nb plugin install nonebot_plugin_apscheduler
 nb plugin install nonebot_plugin_alconna
 nb plugin install nonebot_plugin_orm
 ```
 
 ## 🌙更新日志
 
 <details>
 <summary>点击展开</summary>
 
+- 0.4.1 / 2024-05-07:
+   1. 修复定时提醒一直发送的问题
+   2. 更新README.md
+   3. 修复type hint错误
+
 - 0.4.0 / 2024-04-30:
    1. 重构完成，将所有数据迁移到官方数据库插件[plugin-orm](https://github.com/nonebot/plugin-orm)，之前的数据失效
    2. 修改了插件触发指令和相关逻辑
    3. 重构所有代码，优化处理逻辑
    >该版本是破坏性更新，且仍在测试中，有任何疑问欢迎issue或pr
 
 - 0.3.8 / 2024-04-28:
@@ -139,55 +154,56 @@
 - 0.1.4 / 2023-03-05:
    1. 修复了无法取消订阅早八的bug
 
 </details>
 
 ## 🎉命令
 
-1. 课表帮助：获取本条帮助
+- 课表帮助：获取本条帮助
 
-2. 导入课表：需要有小爱课表分享出来的链接，打开小爱课程表，手动添加课程或从教务导入(已适配了大部分高校)课程后
+- 导入课表：需要有小爱课表分享出来的链接，打开小爱课程表，手动添加课程或从教务导入(已适配了大部分高校)课程后
 
     ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/export.jpg)
 
-    在基本设置里把开始上课时间等调整好之后(尤其是时间、节数)，把分享课表得到的链接发送给bot即可导入本地(分享前需要登录小米账户 [#1](https://github.com/maoxig/nonebot-plugin-ai-timetable/issues/1))
+    在基本设置里把开始上课时间等调整好之后(尤其是时间、节数)，把分享课表得到的链接发送给bot即可导入本地
 
-3. 更新课表；如果在小爱课程表里修改了课程，发送该条指令即可更新本地的课表，无需重新导入
-  
-4. 查询课表+[参数]：查询[参数]的课表，参数支持[本周/下周、周x、昨天/今天/明天/后天、早八、课程名]
+> [!NOTE]
+> 在分享前，你需要登录小米账户 [#1](https://github.com/maoxig/nonebot-plugin-ai-timetable/issues/1)
 
-5. 添加课程提醒+[参数]：参数支持[周x、早八、课程名]
+- 更新课表；如果在小爱课程表里修改了课程，发送该条指令即可更新本地的课表，无需重新导入
+  
+- 查询课表+[参数]：查询[参数]的课表，参数支持[本周/下周、周x、昨天/今天/明天/后天、早八、课程名、下节课]
 
-6. 删除课程提醒+[参数]：参数支持[全部、周x、早八、课程名]
+- 添加课程提醒+[参数]：参数支持[周x、早八、课程名]
 
-7. 查看课程提醒：查看当前已经添加的课程提醒
+- 删除课程提醒+[参数]：参数支持[全部、周x、早八、课程名]
 
+- 查看课程提醒：查看当前已经添加的课程提醒
 
 ## ⭐效果图
 
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/update.png)
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/query.png)
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/query1.png)
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/query1.png)
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/reminder.png)
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/reminder1.png)
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/someday_classes_pic.jpg)
 
-### 关于小爱课程表内的一些说明
+### 😥我不知道怎么使用小爱课程表
 
 如下图
 
-- 第一次使用本插件时，需要用`nb orm upgrade`升级数据库
 - 首先要登录上小米账户,否则可能获取到错误的课表信息 [#1](https://github.com/maoxig/nonebot-plugin-ai-timetable/issues/1)
 - 设置好开始上课时间
 - 设置好课程时间，可以修改每节课具体的时间，
 - 课表节数按自己需求调，一般教务导入的课表节数可能不符合实际，需要微调
-- 每周起始日建议默认的周一即可（周日起始没测试过可能有bug）
+- 每周起始日建议默认的周一即可
 - 如果导入课表后在小爱课表内修改了课程，直接给bot发送更新课表即可更新本地课表
-- 当你主页的课表和学校课表基本一致时，那么小爱课程表就被调教好了，可以导入了
+- 当你主页的课表和学校课表基本一致时，那么小爱课程表就被设置好了，可以导入了
 
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/settings.jpg)
 
 ## 🐦计划
 
 - [x] 查询下节课的信息
 
@@ -207,26 +223,30 @@
 
 - [ ] 适配更多课表、脱离小爱课表
 
 - [ ] 完善插件
 
 ## 🐛存在的问题
 
- ### 关于定时任务的持久化存储问题：
+> [!NOTE]
+> 在当前版本下，Bot重启后会失去之前创建过的任务，这个问题暂时无法解决
 
-众所周知，使用apscheduler添加的定时任务，会在bot重启后丢失，这是因为使用[nonebot-plugin-apscheduler](https://github.com/nonebot/plugin-apscheduler)创建出来的scheduler，默认使用的JobStore(即保存任务的方式)，是MemoryJobStore，也就是存在内存中，因此会导致重启丢任务。
+众所周知，使用apscheduler添加的定时任务，会在bot重启后丢失，这是因为使用[nonebot-plugin-apscheduler](https://github.com/nonebot/plugin-apscheduler)创建出来的`scheduler`，默认使用的`JobStore`(即保存任务的方式)，是`MemoryJobStore`，也就是存在内存中，因此会导致重启丢任务。
 
-因此参考[apscheduler](https://apscheduler.readthedocs.io/en/latest/userguide.html#configuring-the-scheduler)，你可以在bot的配置文件中添加配置项，让[nonebot-plugin-apscheduler](https://github.com/nonebot/plugin-apscheduler)创建出来的scheduler的默认 JobStore 改为使用数据库，这样就可以持久化存储任务，而不需要额外修改任何东西。
+因此参考[apscheduler](https://apscheduler.readthedocs.io/en/latest/userguide.html#configuring-the-scheduler)，你可以在bot的配置文件中添加配置项，让[nonebot-plugin-apscheduler](https://github.com/nonebot/plugin-apscheduler)创建出来的`scheduler`的默认 `JobStore` 改为使用数据库，这样就可以持久化存储任务，而不需要额外修改任何东西。
 
-然而，很不幸的是，在apscheduler4.0版本之前，所支持的数据库类JobStore都是使用**同步**引擎的，然而[plugin-orm](https://github.com/nonebot/plugin-orm)所采用的是异步引擎，因此你暂时还不能这样做。
+然而，很不幸的是，在`apscheduler4.0`版本之前，所支持的数据库类JobStore都是使用**同步**引擎的，不支持异步引擎，然而[plugin-orm](https://github.com/nonebot/plugin-orm)所采用的是异步引擎，因此你暂时还不能这样做。
 
-所以，暂时还无法解决定时任务的持久化存储问题，除非apscheduler正式发版4.0（目前还是alpha版本），你可以再等待，本插件会持续跟进更新。
+所以，暂时还无法解决定时任务的持久化存储问题，除非`apscheduler`正式发版4.0（目前还是alpha版本），你可以再等待，本插件会持续跟进更新。
 
 ## 🎉致谢
+
 - 感谢[nonebot-plugin-htmlrender](https://github.com/kexue-z/nonebot-plugin-htmlrender)提供的渲染工具
 - 感谢[plugin-orm](https://github.com/nonebot/plugin-orm)提供的异步数据库接口
 - 感谢[nonebot-plugin-apscheduler](https://github.com/nonebot/plugin-apscheduler)提供的定时任务接口
 - 感谢[nonebot-plugin-alconna](https://github.com/nonebot/plugin-alconna)
 - 感谢[Matcha](https://github.com/A-kirami/matcha)提供的简单好用的测试平台
-### 喜欢的话就点个star✨吧
+
+### ✨喜欢的话就点个star吧
+
 或者, 你也可以看我写的其他插件
-[nonebot-plugin-manga-translator](https://github.com/maoxig/nonebot-plugin-manga-translator)一个支持多api, 方便好用的图片/漫画翻译插件
+[nonebot-plugin-manga-translator](https://github.com/maoxig/nonebot-plugin-manga-translator)一个支持多api（包括离线部署）、跨平台、方便好用的图片/漫画翻译插件
```

#### html2text {}

```diff
@@ -1,45 +1,49 @@
-                                   _[_n_o_n_e_b_o_t_]
-                         # nonebot-plugin-ai-timetable
-â¨*åºäºNonebot2çå¯¹æ¥å°ç±è¯¾ç¨è¡¨çæä»¶*â¨_[_n_o_n_e_b_o_t_]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
+                  _[_n_o_n_e_b_o_t_]# nonebot-plugin-ai-timetable â¨
+ *åºäºNonebot2çå¯¹æ¥å°ç±è¯¾ç¨è¡¨çæä»¶* â¨_[_n_o_n_e_b_o_t_]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
                                    [python]
 ## ð¿å®è£ 1. éè¿`pip`æ`nb`å®è£ï¼ - ä½¿ç¨nb(æ¨è)
 å¨æºå¨äººç®å½ä¸å½ä»¤è¡ä½¿ç¨`nb plugin install
 nonebot_plugin_ai_timetable` - ä½¿ç¨pip: `pip plugin install
 nonebot_plugin_ai_timetable` ç¶åå¨æºå¨äºº`pyproject.toml`éç`plugins =
-[]`åè¡¨è¿½å `"nonebot_plugin_ai_timetable"` 2. æ°æ®å­å¨ä½¿ç¨[plugin-
-orm](https://github.com/nonebot/plugin-orm), æ¥å¥æ°æ®åºï¼æ¹ä¾¿ç®¡ç 3.
-ç¬¬ä¸æ¬¡ä½¿ç¨ä½¿ç¨[plugin-orm](https://github.com/nonebot/plugin-
-orm)æ¶ï¼éè¦ç¨`nb orm upgrade`åçº§æ°æ®åº ## ðç®ä» 1.
+[]`åè¡¨è¿½å `"nonebot_plugin_ai_timetable"` - ä½¿ç¨å¶ä»åç®¡çå¨ï¼
+æ ¹æ®åç®¡çå¨çæä»¤å®è£æä»¶ 2. æ°æ®å­å¨ä½¿ç¨[plugin-orm]
+(https://github.com/nonebot/plugin-orm), ä½¿ç¨`nb orm upgrade`åçº§æ°æ®åº
+> [!WARNING] > ç¬¬ä¸æ¬¡ä½¿ç¨[plugin-orm](https://github.com/nonebot/plugin-
+orm)ï¼æèæä»¶å®ä¹çæ¨¡åæææ´æ°æ¶ï¼éè¦ç¨`nb orm
+upgrade`åçº§æ°æ®åº ## ðç®ä» 1.
 å»çå¼ä¸é®å¯¼å¥å°ç±è¯¾è¡¨ï¼è®©ä½ çbotå®ç°å°ç±è¯¾è¡¨çåè½ 2.
 ç¨æ·è¯¾è¡¨æ°æ®éç¦»ï¼åºäº[plugin-rom](https://github.com/nonebot/
 plugin-orm),
 æ¥å¥æ°æ®åºï¼æ éæå¿è¯¾ç¨æ¶é´å²çªãä¸åå­¦æ ¡è¯¾è¡¨ä¸åç­é®é¢
 3. ééå¤å¹³å°ï¼å³ä½¿æ¯çµæ¥æ¶©æ¶©ç¾¤ä¹è¦å¥½å¥½å­¦ä¹ ï¼ð¥µð¥µ ##
-âï¸æä»¶éç½®
-è¿äºéç½®é½å·²è®¾å¥½é»è®¤å¼ï¼å¦ææ³è¦ä¿®æ¹éç½®ï¼å¨æºå¨äººç®å½ä¸ç.env.*éé¢å¯ä»¥å¡«åä»¥ä¸éé¡¹
-(å¯é) | config | type | default | example | usage | | :--------------------
--: | :---: | :-----: | :------------------------: | :--------------------------
--------------------------------------------------------------------------- | |
-TIMETABLE_PIC | bool | true | TIMETABLE_PIC=false |
-å¯éæ©ææ¥è¯¾è¡¨ä»¥å¾ç/æå­åéï¼é»è®¤ä»¥å¾çåé(true) | |
-TIMETABLE_ALOCK_SOMEDAY | int | 22 | TIMETABLE_ALOCK_SOMEDAY=15 |
+âï¸æä»¶éç½® >[!NOTE] å¯éçæä»¶éç½®
+è¿äºéç½®é½å·²è®¾å¥½é»è®¤å¼ï¼å æ­¤æ¯å¯éçï¼å¦ææ³è¦ä¿®æ¹éç½®ï¼å¨æºå¨äººç®å½ä¸ç.env.*éé¢å¯ä»¥å¡«åä»¥ä¸éé¡¹,
+æªæ¥ä¼èèå¼æ¾æ´å¤çéç½®é¡¹ | config | type | default | example |
+usage | | :---------------------: | :---: | :-----: | :-----------------------
+-: | :-------------------------------------------------------------------------
+--------------------------- | | TIMETABLE_PIC | bool | true |
+TIMETABLE_PIC=false | å¯éæ©ææ¥è¯¾è¡¨ä»¥å¾ç/
+æå­åéï¼é»è®¤ä»¥å¾çåé(true) | | TIMETABLE_ALOCK_SOMEDAY | int |
+22 | TIMETABLE_ALOCK_SOMEDAY=15 |
 è®¢éææ¥è¯¾è¡¨çåéæ¶é´ï¼å¿é¡»æ¯0-24çæ°å­ | |
 TIMETABLE_ALOCK_8 | int | 21 | TIMETABLE_ALOCK_8=16 |
 è®¢éæ©å«çåéæ¶é´ï¼å¿é¡»æ¯0-
 24çæ°å­.è¿éåéçé½æ¯ç¬¬äºå¤©çï¼æä»¥å»ºè®®è®¾ç½®ä¸º18-23ç¹ |
 | TIMETABLE_SEND_TIME | float | 0.5 | TIMETABLE_SEND_TIME=1 |
 è®¢éè¯¾ç¨æååéçæ¶é´ï¼åä½æ¯`å°æ¶`ï¼å¯ä»¥æ¯æ´æ°ä¹å¯ä»¥æ¯å°æ°ï¼å»ºè®®ä¸è¦è®¾çå¤ªå¤§ï¼é¿ååºç°æ æ³é¢æçbug
-| ## ð¿ä¾èµ
+| ## ð¿ä¾èµ > [!NOTE] >
 æä»¶ä¾èµä¼å¨å®è£æ¶èªå¨å®è£ï¼å¦æå®è£å¤±è´¥ï¼ä½ å¯ä»¥æç§ä»¥ä¸æä»¤æå¨åæ¬¡å®è£
 ```python nb plugin install nonebot_plugin_htmlrender nb plugin install
 nonebot_plugin_apscheduler nb plugin install nonebot_plugin_alconna nb plugin
-install nonebot_plugin_orm ``` ## ðæ´æ°æ¥å¿ ç¹å»å±å¼ - 0.4.0 / 2024-
-04-30: 1. éæå®æï¼å°æææ°æ®è¿ç§»å°å®æ¹æ°æ®åºæä»¶[plugin-
-orm](https://github.com/nonebot/plugin-orm)ï¼ä¹åçæ°æ®å¤±æ 2.
+install nonebot_plugin_orm ``` ## ðæ´æ°æ¥å¿ ç¹å»å±å¼ - 0.4.1 / 2024-
+05-07: 1. ä¿®å¤å®æ¶æéä¸ç´åéçé®é¢ 2. æ´æ°README.md 3.
+ä¿®å¤type hintéè¯¯ - 0.4.0 / 2024-04-30: 1.
+éæå®æï¼å°æææ°æ®è¿ç§»å°å®æ¹æ°æ®åºæä»¶[plugin-orm](https:
+//github.com/nonebot/plugin-orm)ï¼ä¹åçæ°æ®å¤±æ 2.
 ä¿®æ¹äºæä»¶è§¦åæä»¤åç¸å³é»è¾ 3.
 éæææä»£ç ï¼ä¼åå¤çé»è¾
 >è¯¥çæ¬æ¯ç ´åæ§æ´æ°ï¼ä¸ä»å¨æµè¯ä¸­ï¼æä»»ä½çé®æ¬¢è¿issueæpr
 - 0.3.8 / 2024-04-28: 1. ä¿®å¤è®¾ç½®éè¯¯ 2. éæä»£ç  - 0.3.7 / 2024-04-
 24: 1. æ´æ°Nonebot2çæ¬è³2.2.0 2. åºäº [nonebot-plugin-alconna](https://
 github.com/nonebot/plugin-alconna) ééå¤å¹³å° 3.
 æ¾å®½httpxéå¶ï¼ç§»é¤onebotä¾èµ - 0.3.6 / 2023-09-02: 1.
@@ -61,77 +65,78 @@
 æ°å¢3é¡¹éç½®é¡¹ï¼ææ¥è¯¾è¡¨å¯éæ©ä»¥å¾çåéï¼é»è®¤ä¸ºå¾çï¼
 - 0.1.8 / 2023-03-08: 1. ä¿®æ¹é¨åä»£ç ï¼ä¼åè¯¾è¡¨æ ¼å¼ 2.
 ä¿®å¤äºèæ°ä¸º11çè¯¾ä¼æå¨èæ°ä¸º2çè¯¾ç¨åé¢çbug
 (QAQå¤ªè ¢äºå«éªäºå«éªäº) - 0.1.7 / 2023-03-07: 1.
 ä¿®å¤äºæ¶é´ä¸ä¼èªå·±æ¹åçbug 2. æ°å¢äºä¸è¯¾/ä¸èè¯¾åè½ 3.
 ä¼åäºä¸äºå±å±±ä»£ç  - 0.1.5 / 2023-03-06: 1.
 æ°å¢äºç§èè®¢éè¯¾è¡¨|æ©å«çåè½ - 0.1.4 / 2023-03-05: 1.
-ä¿®å¤äºæ æ³åæ¶è®¢éæ©å«çbug ## ðå½ä»¤ 1.
-è¯¾è¡¨å¸®å©ï¼è·åæ¬æ¡å¸®å© 2.
+ä¿®å¤äºæ æ³åæ¶è®¢éæ©å«çbug ## ðå½ä»¤ -
+è¯¾è¡¨å¸®å©ï¼è·åæ¬æ¡å¸®å© -
 å¯¼å¥è¯¾è¡¨ï¼éè¦æå°ç±è¯¾è¡¨åäº«åºæ¥çé¾æ¥ï¼æå¼å°ç±è¯¾ç¨è¡¨ï¼æå¨æ·»å è¯¾ç¨æä»æå¡å¯¼å¥
 (å·²ééäºå¤§é¨åé«æ ¡)è¯¾ç¨å ![Image text](https://github.com/maoxig/
 nonebot-plugin-ai-timetable/blob/main/resource/export.jpg)
 å¨åºæ¬è®¾ç½®éæå¼å§ä¸è¯¾æ¶é´ç­è°æ´å¥½ä¹å
 (å°¤å¶æ¯æ¶é´ãèæ°)ï¼æåäº«è¯¾è¡¨å¾å°çé¾æ¥åéç»botå³å¯å¯¼å¥æ¬å°
-(åäº«åéè¦ç»å½å°ç±³è´¦æ· [#1](https://github.com/maoxig/nonebot-
-plugin-ai-timetable/issues/1)) 3.
+> [!NOTE] > å¨åäº«åï¼ä½ éè¦ç»å½å°ç±³è´¦æ· [#1](https://github.com/
+maoxig/nonebot-plugin-ai-timetable/issues/1) -
 æ´æ°è¯¾è¡¨ï¼å¦æå¨å°ç±è¯¾ç¨è¡¨éä¿®æ¹äºè¯¾ç¨ï¼åéè¯¥æ¡æä»¤å³å¯æ´æ°æ¬å°çè¯¾è¡¨ï¼æ ééæ°å¯¼å¥
-4. æ¥è¯¢è¯¾è¡¨+[åæ°]ï¼æ¥è¯¢[åæ°]çè¯¾è¡¨ï¼åæ°æ¯æ[æ¬å¨/
-ä¸å¨ãå¨xãæ¨å¤©/ä»å¤©/æå¤©/åå¤©ãæ©å«ãè¯¾ç¨å] 5.
-æ·»å è¯¾ç¨æé+[åæ°]ï¼åæ°æ¯æ[å¨xãæ©å«ãè¯¾ç¨å] 6.
+- æ¥è¯¢è¯¾è¡¨+[åæ°]ï¼æ¥è¯¢[åæ°]çè¯¾è¡¨ï¼åæ°æ¯æ[æ¬å¨/
+ä¸å¨ãå¨xãæ¨å¤©/ä»å¤©/æå¤©/åå¤©ãæ©å«ãè¯¾ç¨åãä¸èè¯¾] -
+æ·»å è¯¾ç¨æé+[åæ°]ï¼åæ°æ¯æ[å¨xãæ©å«ãè¯¾ç¨å] -
 å é¤è¯¾ç¨æé+[åæ°]ï¼åæ°æ¯æ[å¨é¨ãå¨xãæ©å«ãè¯¾ç¨å]
-7. æ¥çè¯¾ç¨æéï¼æ¥çå½åå·²ç»æ·»å çè¯¾ç¨æé ## â­ææå¾
+- æ¥çè¯¾ç¨æéï¼æ¥çå½åå·²ç»æ·»å çè¯¾ç¨æé ## â­ææå¾
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/
 resource/update.png) ![Image text](https://github.com/maoxig/nonebot-plugin-ai-
 timetable/blob/main/resource/query.png) ![Image text](https://github.com/
 maoxig/nonebot-plugin-ai-timetable/blob/main/resource/query1.png) ![Image text]
 (https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/
 query1.png) ![Image text](https://github.com/maoxig/nonebot-plugin-ai-
 timetable/blob/main/resource/reminder.png) ![Image text](https://github.com/
 maoxig/nonebot-plugin-ai-timetable/blob/main/resource/reminder1.png) ![Image
 text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/
-someday_classes_pic.jpg) ### å³äºå°ç±è¯¾ç¨è¡¨åçä¸äºè¯´æ å¦ä¸å¾
-- ç¬¬ä¸æ¬¡ä½¿ç¨æ¬æä»¶æ¶ï¼éè¦ç¨`nb orm upgrade`åçº§æ°æ®åº -
+someday_classes_pic.jpg) ### ð¥æä¸ç¥éæä¹ä½¿ç¨å°ç±è¯¾ç¨è¡¨
+å¦ä¸å¾ -
 é¦åè¦ç»å½ä¸å°ç±³è´¦æ·,å¦åå¯è½è·åå°éè¯¯çè¯¾è¡¨ä¿¡æ¯ [#1]
 (https://github.com/maoxig/nonebot-plugin-ai-timetable/issues/1) -
 è®¾ç½®å¥½å¼å§ä¸è¯¾æ¶é´ -
 è®¾ç½®å¥½è¯¾ç¨æ¶é´ï¼å¯ä»¥ä¿®æ¹æ¯èè¯¾å·ä½çæ¶é´ï¼ -
 è¯¾è¡¨èæ°æèªå·±éæ±è°ï¼ä¸è¬æå¡å¯¼å¥çè¯¾è¡¨èæ°å¯è½ä¸ç¬¦åå®éï¼éè¦å¾®è°
--
-æ¯å¨èµ·å§æ¥å»ºè®®é»è®¤çå¨ä¸å³å¯ï¼å¨æ¥èµ·å§æ²¡æµè¯è¿å¯è½æbugï¼
--
+- æ¯å¨èµ·å§æ¥å»ºè®®é»è®¤çå¨ä¸å³å¯ -
 å¦æå¯¼å¥è¯¾è¡¨åå¨å°ç±è¯¾è¡¨åä¿®æ¹äºè¯¾ç¨ï¼ç´æ¥ç»botåéæ´æ°è¯¾è¡¨å³å¯æ´æ°æ¬å°è¯¾è¡¨
 -
-å½ä½ ä¸»é¡µçè¯¾è¡¨åå­¦æ ¡è¯¾è¡¨åºæ¬ä¸è´æ¶ï¼é£ä¹å°ç±è¯¾ç¨è¡¨å°±è¢«è°æå¥½äºï¼å¯ä»¥å¯¼å¥äº
+å½ä½ ä¸»é¡µçè¯¾è¡¨åå­¦æ ¡è¯¾è¡¨åºæ¬ä¸è´æ¶ï¼é£ä¹å°ç±è¯¾ç¨è¡¨å°±è¢«è®¾ç½®å¥½äºï¼å¯ä»¥å¯¼å¥äº
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/
 resource/settings.jpg) ## ð¦è®¡å - [x] æ¥è¯¢ä¸èè¯¾çä¿¡æ¯ - [x]
 å¯éæ©æ¯å¦åéå¾çä»¥é¿åé£æ§ - [x] å¢å æ´å¤çéç½®é¡¹ - [x]
 éæä»£ç  - [x] è®¢éæå®çè¯¾ - [x] å¤å¹³å°éé, åºäº [nonebot-
 plugin-alconna](https://github.com/nonebot/plugin-alconna) - [x]
 æ¯æå®æ¶ä»»å¡æ¬å°å­å¨ - [x] éé[plugin-orm](https://github.com/
 nonebot/plugin-orm), æ¥å¥æ°æ®åº - [ ]
 ééæ´å¤è¯¾è¡¨ãè±ç¦»å°ç±è¯¾è¡¨ - [ ] å®åæä»¶ ##
-ðå­å¨çé®é¢ ### å³äºå®æ¶ä»»å¡çæä¹åå­å¨é®é¢ï¼
+ðå­å¨çé®é¢ > [!NOTE] >
+å¨å½åçæ¬ä¸ï¼Botéå¯åä¼å¤±å»ä¹ååå»ºè¿çä»»å¡ï¼è¿ä¸ªé®é¢ææ¶æ æ³è§£å³
 ä¼æå¨ç¥ï¼ä½¿ç¨apscheduleræ·»å çå®æ¶ä»»å¡ï¼ä¼å¨botéå¯åä¸¢å¤±ï¼è¿æ¯å ä¸ºä½¿ç¨
 [nonebot-plugin-apscheduler](https://github.com/nonebot/plugin-
-apscheduler)åå»ºåºæ¥çschedulerï¼é»è®¤ä½¿ç¨çJobStore
-(å³ä¿å­ä»»å¡çæ¹å¼)ï¼æ¯MemoryJobStoreï¼ä¹å°±æ¯å­å¨åå­ä¸­ï¼å æ­¤ä¼å¯¼è´éå¯ä¸¢ä»»å¡ã
+apscheduler)åå»ºåºæ¥ç`scheduler`ï¼é»è®¤ä½¿ç¨ç`JobStore`
+(å³ä¿å­ä»»å¡çæ¹å¼)ï¼æ¯`MemoryJobStore`ï¼ä¹å°±æ¯å­å¨åå­ä¸­ï¼å æ­¤ä¼å¯¼è´éå¯ä¸¢ä»»å¡ã
 å æ­¤åè[apscheduler](https://apscheduler.readthedocs.io/en/latest/
 userguide.html#configuring-the-
 scheduler)ï¼ä½ å¯ä»¥å¨botçéç½®æä»¶ä¸­æ·»å éç½®é¡¹ï¼è®©[nonebot-
 plugin-apscheduler](https://github.com/nonebot/plugin-
-apscheduler)åå»ºåºæ¥çschedulerçé»è®¤ JobStore
+apscheduler)åå»ºåºæ¥ç`scheduler`çé»è®¤ `JobStore`
 æ¹ä¸ºä½¿ç¨æ°æ®åºï¼è¿æ ·å°±å¯ä»¥æä¹åå­å¨ä»»å¡ï¼èä¸éè¦é¢å¤ä¿®æ¹ä»»ä½ä¸è¥¿ã
-ç¶èï¼å¾ä¸å¹¸çæ¯ï¼å¨apscheduler4.0çæ¬ä¹åï¼ææ¯æçæ°æ®åºç±»JobStoreé½æ¯ä½¿ç¨**åæ­¥**å¼æçï¼ç¶è
+ç¶èï¼å¾ä¸å¹¸çæ¯ï¼å¨`apscheduler4.0`çæ¬ä¹åï¼ææ¯æçæ°æ®åºç±»JobStoreé½æ¯ä½¿ç¨**åæ­¥**å¼æçï¼ä¸æ¯æå¼æ­¥å¼æï¼ç¶è
 [plugin-orm](https://github.com/nonebot/plugin-
 orm)æéç¨çæ¯å¼æ­¥å¼æï¼å æ­¤ä½ ææ¶è¿ä¸è½è¿æ ·åã
-æä»¥ï¼ææ¶è¿æ æ³è§£å³å®æ¶ä»»å¡çæä¹åå­å¨é®é¢ï¼é¤éapscheduleræ­£å¼åç4.0ï¼ç®åè¿æ¯alphaçæ¬ï¼ï¼ä½ å¯ä»¥åç­å¾ï¼æ¬æä»¶ä¼æç»­è·è¿æ´æ°ã
+æä»¥ï¼ææ¶è¿æ æ³è§£å³å®æ¶ä»»å¡çæä¹åå­å¨é®é¢ï¼é¤é`apscheduler`æ­£å¼åç4.0ï¼ç®åè¿æ¯alphaçæ¬ï¼ï¼ä½ å¯ä»¥åç­å¾ï¼æ¬æä»¶ä¼æç»­è·è¿æ´æ°ã
 ## ðè´è°¢ - æè°¢[nonebot-plugin-htmlrender](https://github.com/kexue-z/
 nonebot-plugin-htmlrender)æä¾çæ¸²æå·¥å· - æè°¢[plugin-orm](https://
 github.com/nonebot/plugin-orm)æä¾çå¼æ­¥æ°æ®åºæ¥å£ - æè°¢[nonebot-
 plugin-apscheduler](https://github.com/nonebot/plugin-
 apscheduler)æä¾çå®æ¶ä»»å¡æ¥å£ - æè°¢[nonebot-plugin-alconna](https:
 //github.com/nonebot/plugin-alconna) - æè°¢[Matcha](https://github.com/A-
 kirami/matcha)æä¾çç®åå¥½ç¨çæµè¯å¹³å° ###
-åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§ æè, ä½ ä¹å¯ä»¥çæåçå¶ä»æä»¶
+â¨åæ¬¢çè¯å°±ç¹ä¸ªstarå§ æè, ä½ ä¹å¯ä»¥çæåçå¶ä»æä»¶
 [nonebot-plugin-manga-translator](https://github.com/maoxig/nonebot-plugin-
-manga-translator)ä¸ä¸ªæ¯æå¤api, æ¹ä¾¿å¥½ç¨çå¾ç/æ¼«ç»ç¿»è¯æä»¶
+manga-
+translator)ä¸ä¸ªæ¯æå¤apiï¼åæ¬ç¦»çº¿é¨ç½²ï¼ãè·¨å¹³å°ãæ¹ä¾¿å¥½ç¨çå¾ç/
+æ¼«ç»ç¿»è¯æä»¶
```

### Comparing `nonebot_plugin_ai_timetable-0.4.0/nonebot_plugin_ai_timetable/__init__.py` & `nonebot_plugin_ai_timetable-0.4.1/nonebot_plugin_ai_timetable/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from .reminder import (
     check_scheduler,
     add_reminders,
     remove_reminders,
     query_reminders_by_uid,
 )
 
-__ai_timetable__usage__ = "## 小爱课表帮助:\n- 课表帮助：获取本条帮助\n- 导入课表: 使用小爱课程表分享的链接一键导入\n- 更新课表：导入课表后，若云端课表有修改，可直接更新本地课表\n-  查询课表+[参数]：查询[参数]的课表，参数支持[本周/下周、周x、昨天/今天/明天/后天、早八、课程名]\n- 添加课程提醒+[参数]：参数支持[周x、早八、课程名]\n- 删除课程提醒+[参数]：参数支持[全部、周x、早八、课程名]\n- 查看课程提醒：查看当前已经添加的课程提醒"
+__ai_timetable__usage__ = "## 小爱课表帮助:\n- 课表帮助：获取本条帮助\n- 导入课表: 使用小爱课程表分享的链接一键导入\n- 更新课表：导入课表后，若云端课表有修改，可直接更新本地课表\n-  查询课表+[参数]：查询[参数]的课表，参数支持[本周/下周、周x、昨天/今天/明天/后天、早八、课程名、下节课]\n- 添加课程提醒+[参数]：参数支持[周x、早八、课程名]\n- 删除课程提醒+[参数]：参数支持[全部、周x、早八、课程名]\n- 查看课程提醒：查看当前已经添加的课程提醒"
 
 
 __plugin_meta__ = PluginMetadata(
     name="小爱课表",
     description="一键导入课表、查看课表、提醒上课、查询课程，使用/课表帮助查看指令列表",
     usage=__ai_timetable__usage__,
     type="application",
```

### Comparing `nonebot_plugin_ai_timetable-0.4.0/nonebot_plugin_ai_timetable/data_manager.py` & `nonebot_plugin_ai_timetable-0.4.1/nonebot_plugin_ai_timetable/data_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,29 +3,30 @@
     select,
 )
 from nonebot import logger, require
 from sqlalchemy.orm import selectinload
 
 require("nonebot_plugin_orm")
 from nonebot_plugin_orm import get_session
-from typing import List
+from typing import List, Union
 from .model import User, Course
 import time
 
 
 async def add_user(user_id: str, base_url: str, response_url: str, user_data: dict):
     """在数据库中添加新用户,user_data是返回数据中的data部分"""
     async with get_session() as session:
         user_data.update(user_data["setting"])
         del user_data["setting"]
         user_orm = User()
         user_orm.user_id = user_id
         user_orm.base_url = base_url
         user_orm.response_url = response_url
         # 设置类的属性
+
         for key, value in user_data.items():
             if hasattr(User, key) and key != "courses":
                 setattr(user_orm, key, value)
         user_data["courses"].sort(key=lambda x: int(x["sections"].split(",")[0]))
         for course in user_data["courses"]:
             course_orm = Course()
             for key, value in course.items():
@@ -80,25 +81,28 @@
         )
         result = await session.execute(query)
         user_orm = result.scalar_one_or_none()
         if user_orm:
             # 删除用户的所有课程
             user_orm.courses.clear()
             # 删除用户对象
-            session.delete(user_orm)
+            await session.delete(user_orm)
             # 提交更改
             await session.commit()
 
 
 async def query_user_by_uid(user_id: str) -> User:
     """从数据库获取某个用户信息，只含信息，不含课表"""
     async with get_session() as session:
         query = select(User).filter(User.user_id == user_id)
         result = await session.execute(query)
         result = result.scalar()
+        if not result:
+            logger.warning("用户不在数据库中")
+            raise ValueError("用户信息不存在于数据库中") 
     return result
 
 
 async def query_course_by_day(user_id: str, day: int) -> List[Course]:
     """根据用户ID和日期查询课程
     参数：
         day: 周内日期[1,7]"""
```

### Comparing `nonebot_plugin_ai_timetable-0.4.0/nonebot_plugin_ai_timetable/manager.py` & `nonebot_plugin_ai_timetable-0.4.1/nonebot_plugin_ai_timetable/manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import httpx
 from datetime import datetime
 from typing import Union
 from nonebot.matcher import Matcher
-from nonebot import require, get_plugin_config
+from nonebot import require, get_plugin_config,logger
 from nonebot.adapters import Message, Event, Bot
 
 from nonebot_plugin_ai_timetable.data_manager import weekday_int
 
 require("nonebot_plugin_alconna")
 require("nonebot_plugin_htmlrender")
 
@@ -42,15 +42,15 @@
 """
 这个文件的函数都是一些工具函数，根据uid和相关参数，构建出所需要的课表信息，同时返回str，
 之后会调用send_table来根据设置决定发送图片还是文字
 
 """
 
 
-async def check_user(event: Event, matcher: Matcher) -> Event:
+async def check_user(event: Event, matcher: Matcher):
     """检查用户是否在课表系统中"""
     if not await check_user_in_table(event.get_user_id()):
         await matcher.finish("你还没有导入课表，发送/导入课表来导入吧！")
 
 
 async def check_base_url(key: str):
     text = key
@@ -74,31 +74,37 @@
 
         page.on(
             "response",
             response_listener,
         )
         await page.goto(url=base_url, wait_until="networkidle")
         if __response_url__:
-            async with httpx.AsyncClient() as client:
-                res = await client.get(__response_url__, headers=__headers__)
-            return res.json()["data"]
-
+            try:
+                async with httpx.AsyncClient() as client:
+                    res = await client.get(__response_url__, headers=__headers__)
+                return res.json()["data"]
+            except Exception as e:
+                logger.error(f"{e},res_url:{__response_url__}")
+        return {}
 
 async def update_table(uid: str, url: str):
     """导入课表，存在|不存在该用户"""
     user_data = await get_user_data(url)
+    if not __response_url__:
+        raise RuntimeError("没有监听到响应url")
     if await check_user_in_table(uid):
         await update_user(uid, url, __response_url__, user_data)
     else:
         await add_user(uid, url, __response_url__, user_data)
 
-async def update_offline_table_by_uid(uid:str):
+
+async def update_offline_table_by_uid(uid: str):
     user = await query_user_by_uid(uid)
-    base_url=user.base_url
-    await update_table(uid,base_url)
+    base_url = user.base_url
+    await update_table(uid, base_url)
 
 
 async def build_table(uid: str, key: str) -> Union[bytes, str]:
     """根据用户信息和参数，分发不同的处理函数，根据返回的列表进行处理，返回字符串或图片"""
     key = key.strip()
     courses = []
     user = await query_user_by_uid(uid)
@@ -110,21 +116,21 @@
     elif key == "本周":
         return await build_table_for_current_week(uid)
     elif key == "下周":
         return await build_table_for_next_week(uid)
     elif key == "早八":
         courses = await get_courses_for_morning(uid)
         if not courses:
-            return "你明天没有早八呢，好好休息吧"
+            return "你明天没有早八，好好休息吧"
     elif key == "下节课":
         current_courses = await get_courses_for_current_course(uid)
         current_msg = await build_table_by_courses_list(current_courses, user)
         next_courses = await get_courses_for_next_course(uid)
         next_msg = await build_table_by_courses_list(next_courses, user)
-        return f"- 当前的课程信息：\n\n {current_msg if current_courses else '当前没有课程呢'} \n\n- 下节课程信息：\n\n{next_msg if next_courses else '今天接下来没有课了呢'}"
+        return f"- 当前的课程信息：\n\n {current_msg if current_courses else '当前没有课程'} \n\n- 下节课程信息：\n\n{next_msg if next_courses else '今天接下来没有课了'}"
     else:
         courses = await get_courses_by_name(uid, key)
     course_msg = await build_table_by_courses_list(courses, user)
     return course_msg
 
 
 async def build_table_by_course(course: Course, user: User) -> str:
@@ -145,29 +151,29 @@
         course_msg = await build_table_by_course(course, user)
         msg += f"{course_msg}\n"
     return msg
 
 
 async def build_table_for_current_week(uid: str) -> bytes:
     """获取本周课表，以后考虑通过本地生成"""
-    user_data = await query_user_by_uid(uid)
+    user = await query_user_by_uid(uid)
     async with get_new_page(viewport={"width": 1000, "height": 1000}) as page:
-        await page.goto(user_data.base_url, wait_until="networkidle")
+        await page.goto(user.base_url, wait_until="networkidle")
         await page.evaluate(
             'var t = document.querySelector("#root>div>div.importSchedule___UjEKt>div.footer___1iAis.toUp___2mciB"); t.style.display = "none"'
         )
         pic = await page.screenshot(full_page=True, type="jpeg", quality=70)
         return pic
 
 
 async def build_table_for_next_week(uid: str) -> bytes:
     """获取本周课表，以后考虑通过本地生成"""
-    user_data = await query_user_by_uid(uid)
+    user = await query_user_by_uid(uid)
     async with get_new_page(viewport={"width": 1000, "height": 1000}) as page:
-        await page.goto(user_data.base_url, wait_until="networkidle")
+        await page.goto(user.base_url, wait_until="networkidle")
         await page.evaluate(
             'var t = document.querySelector("#root>div>div.importSchedule___UjEKt>div.footer___1iAis.toUp___2mciB"); t.style.display = "none"'
         )
         await page.click(
             "#schedule-view > div.header___26sI1 > div.presentWeek___-o65e > div.rightBtn___2ZhSY"
         )
         pic = await page.screenshot(full_page=True, type="jpeg", quality=70)
@@ -214,22 +220,21 @@
 
 async def get_courses_for_morning(uid: str) -> List[Course]:
     """为用户构建出第二天早八的所有课程"""
     day = weekday_int("明")
     week = await get_current_week(uid, day)
     if day < 0:
         day += 7
-    elif day > 7: 
+    elif day > 7:
         day -= 7
     courses = await query_course_by_day(uid, day)
     courses = [
         course
         for course in courses
-        if str(week) in course.weeks.split(",")
-        and "1" in course.sections.split(",")
+        if str(week) in course.weeks.split(",") and "1" in course.sections.split(",")
     ]  # 从当天的课中选出当周的
     return courses
 
 
 async def get_courses_for_current_course(uid: str) -> List[Course]:
     """获取现在的课程，返回列表"""
     day = weekday_int("今")
```

### Comparing `nonebot_plugin_ai_timetable-0.4.0/nonebot_plugin_ai_timetable/migrations/f67eb52d6a0f_init.py` & `nonebot_plugin_ai_timetable-0.4.1/nonebot_plugin_ai_timetable/migrations/f67eb52d6a0f_init.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ai_timetable-0.4.0/nonebot_plugin_ai_timetable/model.py` & `nonebot_plugin_ai_timetable-0.4.1/nonebot_plugin_ai_timetable/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ai_timetable-0.4.0/nonebot_plugin_ai_timetable/reminder.py` & `nonebot_plugin_ai_timetable-0.4.1/nonebot_plugin_ai_timetable/reminder.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,15 @@
 import random
 
 require("nonebot_plugin_orm")
 require("nonebot_plugin_apscheduler")
 require("nonebot_plugin_alconna")
 from nonebot_plugin_alconna import UniMessage
 from nonebot.exception import ActionFailed
-
-try:
-    from nonebot_plugin_apscheduler import scheduler
-except ImportError:
-    logger.opt(colors=True).info(
-        "未检测到软依赖<y>nonebot_plugin_apscheduler</y>,<r>禁用定时任务功能</r>"
-    )
-    scheduler = None
+from nonebot_plugin_apscheduler import scheduler
 from apscheduler.job import Job
 from apscheduler.triggers.cron import CronTrigger
 from datetime import datetime,timedelta
 from .data_manager import query_user_by_uid, weekday_int,query_course_by_name
 from .manager import (
     get_courses_by_day,
     build_table_by_courses_list,
@@ -65,41 +58,53 @@
 
 async def remove_reminders(uid: str, key: str):
     """移除提醒处理函数"""
     key = key.strip()
     if re.match(__day_pattern__, key):
         day = weekday_int(
             key
-        )  ##day是1-7的整数，但是也有可能是负数和大于7的数，用于判断周数
+        )  
         job_id = f"{uid},周{day}"
         if scheduler.get_job(job_id):
             scheduler.remove_job(job_id=job_id)
-            return "成功移除了一个提醒"
+            return "成功移除了你的1个提醒"
 
     elif key == "早八":
         count=0
         for i,job in enumerate(scheduler.get_jobs()):
-            if job.id.split(",") and len(job.id.split(","))==2 and "早八" in job.id.split(",")[1]:
+            job_name = job.id.split(",")
+            if job_name and len(job_name) == 2 and uid==job_name[0] and "早八" in job.id.split(",")[1]:
                 count += 1
                 scheduler.remove_job(job_id=job.id)
-        return f"成功移除了{i}个提醒"
+        return f"成功移除了你的{count}个提醒"
     elif key == "全部":
-        scheduler.remove_all_jobs()
-        return "成功移除了全部提醒"
+        count = 0
+        for i, job in enumerate(scheduler.get_jobs()):
+            job_name = job.id.split(",")
+            if (
+                job_name
+                and len(job_name) == 2
+                and uid == job_name[0]
+            ):
+                count += 1
+                scheduler.remove_job(job_id=job.id)
+        return f"成功移除了你的全部{count}提醒"
     else:
         count=0
         for i, job in enumerate(scheduler.get_jobs()):
+            job_name=job.id.split(",")
             if (
-                job.id.split(",")
-                and len(job.id.split(",")) == 2
-                and key in job.id.split(",")[1]
+                job_name
+                and len(job_name) == 2
+                and uid == job_name[0]
+                and key in job_name[1]
             ):
                 count+=1
                 scheduler.remove_job(job_id=job.id)
-        return f"成功移除了{count}个提醒"
+        return f"成功移除了你的{count}个提醒"
 
     return f"没有找到名为{key}的提醒"
 
 
 async def add_reminder_for_day(uid: str, day: int, bot: Bot, event: Event) -> List[Job]:
     """添加一周内，某一天的课程提醒，发送时间是前一天的设置时间"""
     job_list = []
@@ -107,14 +112,15 @@
     user = await query_user_by_uid(uid)
     course_msg = await build_table_by_courses_list(courses, user)
     job_day=day-1#0-6
     job_id = f"{uid},周{day}"
     send_day = (job_day-1) % 7
     cron = CronTrigger(
         hour=config.timetable_alock_someday,
+        minute=0,
         second=random.randint(0, 59),
         day_of_week=send_day,
     )
     kwargs = {"bot": bot, "event": event, "course_msg": course_msg}
     job = scheduler.add_job(
         func=send_reminder,
         trigger=cron,
@@ -142,18 +148,19 @@
             course_msg = await build_table_by_courses_list(courses, user)
         else:
             course_msg = "你明天没有早八，好好休息吧"
         job_id = f"{uid},早八{sending_day}"
         kwargs = {"bot": bot, "event": event, "course_msg": course_msg}
         cron = CronTrigger(
             hour=config.timetable_alock_8,
+            minute=0,
             second=random.randint(0, 59),
             day_of_week=sending_day,
         )
-        #logger.debug(job_id+course_msg)
+        # logger.debug(job_id+course_msg)
         job = scheduler.add_job(
             func=send_reminder,
             trigger=cron,
             id=job_id,
             kwargs=kwargs,
             replace_existing=True,
         )
```

### Comparing `nonebot_plugin_ai_timetable-0.4.0/pyproject.toml` & `nonebot_plugin_ai_timetable-0.4.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-ai-timetable"
-version = "0.4.0"
+version = "0.4.1"
 description = "小爱课程表"
 authors = ["maoxiog <674550338@qq.com>"]
 readme = "README.md"
 packages = [{include = "nonebot_plugin_ai_timetable"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `nonebot_plugin_ai_timetable-0.4.0/PKG-INFO` & `nonebot_plugin_ai_timetable-0.4.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-ai-timetable
-Version: 0.4.0
+Version: 0.4.1
 Summary: 小爱课程表
 Author: maoxiog
 Author-email: 674550338@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -15,86 +15,101 @@
 Requires-Dist: nonebot-plugin-alconna (>=0.40.1,<1.0.0)
 Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<1.0.0)
 Requires-Dist: nonebot-plugin-htmlrender (>=0.3.0,<0.4.0)
 Requires-Dist: nonebot-plugin-orm (>=0.7.1)
 Requires-Dist: nonebot2 (>=2.2.0,<3.0.0)
 Description-Content-Type: text/markdown
 
-<p align="center">
-  <a href="https://nonebot.dev/"><img src="https://nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
-</p>
 <div align="center">
+  <a href="https://nonebot.dev/">
+    <img src="https://nonebot.dev/logo.png" width="200" height="200" alt="nonebot">
+  </a>
 
 # nonebot-plugin-ai-timetable
 
-✨*基于Nonebot2的对接小爱课程表的插件*✨
-  
-<a href="https://github.com/nonebot/nonebot2">
-  <img src="https://img.shields.io/badge/nonebot-v2-red" alt="nonebot">
-</a> 
-<a href="./LICENSE">
+✨ *基于Nonebot2的对接小爱课程表的插件* ✨
+
+
+  <a href="https://github.com/nonebot/nonebot2">
+    <img src="https://img.shields.io/badge/nonebot-v2-red" alt="nonebot">
+  </a>
+  <a href="./LICENSE">
     <img src="https://img.shields.io/github/license/maoxig/nonebot-plugin-ai-timetable" alt="license">
-</a>
-<a href="https://pypi.python.org/pypi/nonebot-plugin-ai-timetable">
+  </a>
+  <a href="https://pypi.python.org/pypi/nonebot-plugin-ai-timetable">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-ai-timetable" alt="pypi">
-</a>
-<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
-
-<div align="left">
+  </a>
+  <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+</div>
 
 ## 💿安装
 
 1. 通过`pip`或`nb`安装；
     - 使用nb(推荐)
   
        在机器人目录下命令行使用`nb plugin install nonebot_plugin_ai_timetable`
 
     - 使用pip:
   
       `pip plugin install nonebot_plugin_ai_timetable`
 
       然后在机器人`pyproject.toml`里的`plugins = []`列表追加`"nonebot_plugin_ai_timetable"`
 
-2. 数据存储使用[plugin-orm](https://github.com/nonebot/plugin-orm), 接入数据库，方便管理
+    - 使用其他包管理器：
 
-3. 第一次使用使用[plugin-orm](https://github.com/nonebot/plugin-orm)时，需要用`nb orm upgrade`升级数据库
+      根据包管理器的指令安装插件
+
+2. 数据存储使用[plugin-orm](https://github.com/nonebot/plugin-orm), 使用`nb orm upgrade`升级数据库
+
+> [!WARNING]
+> 第一次使用[plugin-orm](https://github.com/nonebot/plugin-orm)，或者插件定义的模型有所更新时，需要用`nb orm upgrade`升级数据库
 
 ## 📖简介
 
 1. 傻瓜式一键导入小爱课表，让你的bot实现小爱课表的功能
 
 2. 用户课表数据隔离，基于[plugin-rom](https://github.com/nonebot/plugin-orm), 接入数据库，无需担心课程时间冲突、不同学校课表不同等问题
 
 3. 适配多平台，即使是电报涩涩群也要好好学习！🥵🥵
 
 ## ⚙️插件配置
 
-这些配置都已设好默认值，如果想要修改配置，在机器人目录下的.env.*里面可以填写以下选项(可选)
+>[!NOTE] 可选的插件配置
+这些配置都已设好默认值，因此是可选的，如果想要修改配置，在机器人目录下的.env.*里面可以填写以下选项, 未来会考虑开放更多的配置项
 
 |         config          | type  | default |          example           | usage                                                                                                 |
 | :---------------------: | :---: | :-----: | :------------------------: | :---------------------------------------------------------------------------------------------------- |
 |      TIMETABLE_PIC      | bool  |  true   |    TIMETABLE_PIC=false     | 可选择某日课表以图片/文字发送，默认以图片发送(true)                                                   |
 | TIMETABLE_ALOCK_SOMEDAY |  int  |   22    | TIMETABLE_ALOCK_SOMEDAY=15 | 订阅某日课表的发送时间，必须是0-24的数字                                                              |
 |    TIMETABLE_ALOCK_8    |  int  |   21    |    TIMETABLE_ALOCK_8=16    | 订阅早八的发送时间，必须是0-24的数字.这里发送的都是第二天的，所以建议设置为18-23点                    |
 |   TIMETABLE_SEND_TIME   | float |   0.5   |   TIMETABLE_SEND_TIME=1    | 订阅课程提前发送的时间，单位是`小时`，可以是整数也可以是小数，建议不要设的太大，避免出现无法预料的bug |
 
+
 ## 💿依赖
-插件依赖会在安装时自动安装，如果安装失败，你可以按照以下指令手动再次安装
+
+> [!NOTE]
+> 插件依赖会在安装时自动安装，如果安装失败，你可以按照以下指令手动再次安装
+
 ```python
 nb plugin install nonebot_plugin_htmlrender
 nb plugin install nonebot_plugin_apscheduler
 nb plugin install nonebot_plugin_alconna
 nb plugin install nonebot_plugin_orm
 ```
 
 ## 🌙更新日志
 
 <details>
 <summary>点击展开</summary>
 
+- 0.4.1 / 2024-05-07:
+   1. 修复定时提醒一直发送的问题
+   2. 更新README.md
+   3. 修复type hint错误
+
 - 0.4.0 / 2024-04-30:
    1. 重构完成，将所有数据迁移到官方数据库插件[plugin-orm](https://github.com/nonebot/plugin-orm)，之前的数据失效
    2. 修改了插件触发指令和相关逻辑
    3. 重构所有代码，优化处理逻辑
    >该版本是破坏性更新，且仍在测试中，有任何疑问欢迎issue或pr
 
 - 0.3.8 / 2024-04-28:
@@ -160,55 +175,56 @@
 - 0.1.4 / 2023-03-05:
    1. 修复了无法取消订阅早八的bug
 
 </details>
 
 ## 🎉命令
 
-1. 课表帮助：获取本条帮助
+- 课表帮助：获取本条帮助
 
-2. 导入课表：需要有小爱课表分享出来的链接，打开小爱课程表，手动添加课程或从教务导入(已适配了大部分高校)课程后
+- 导入课表：需要有小爱课表分享出来的链接，打开小爱课程表，手动添加课程或从教务导入(已适配了大部分高校)课程后
 
     ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/export.jpg)
 
-    在基本设置里把开始上课时间等调整好之后(尤其是时间、节数)，把分享课表得到的链接发送给bot即可导入本地(分享前需要登录小米账户 [#1](https://github.com/maoxig/nonebot-plugin-ai-timetable/issues/1))
+    在基本设置里把开始上课时间等调整好之后(尤其是时间、节数)，把分享课表得到的链接发送给bot即可导入本地
 
-3. 更新课表；如果在小爱课程表里修改了课程，发送该条指令即可更新本地的课表，无需重新导入
-  
-4. 查询课表+[参数]：查询[参数]的课表，参数支持[本周/下周、周x、昨天/今天/明天/后天、早八、课程名]
+> [!NOTE]
+> 在分享前，你需要登录小米账户 [#1](https://github.com/maoxig/nonebot-plugin-ai-timetable/issues/1)
 
-5. 添加课程提醒+[参数]：参数支持[周x、早八、课程名]
+- 更新课表；如果在小爱课程表里修改了课程，发送该条指令即可更新本地的课表，无需重新导入
+  
+- 查询课表+[参数]：查询[参数]的课表，参数支持[本周/下周、周x、昨天/今天/明天/后天、早八、课程名、下节课]
 
-6. 删除课程提醒+[参数]：参数支持[全部、周x、早八、课程名]
+- 添加课程提醒+[参数]：参数支持[周x、早八、课程名]
 
-7. 查看课程提醒：查看当前已经添加的课程提醒
+- 删除课程提醒+[参数]：参数支持[全部、周x、早八、课程名]
 
+- 查看课程提醒：查看当前已经添加的课程提醒
 
 ## ⭐效果图
 
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/update.png)
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/query.png)
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/query1.png)
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/query1.png)
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/reminder.png)
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/reminder1.png)
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/someday_classes_pic.jpg)
 
-### 关于小爱课程表内的一些说明
+### 😥我不知道怎么使用小爱课程表
 
 如下图
 
-- 第一次使用本插件时，需要用`nb orm upgrade`升级数据库
 - 首先要登录上小米账户,否则可能获取到错误的课表信息 [#1](https://github.com/maoxig/nonebot-plugin-ai-timetable/issues/1)
 - 设置好开始上课时间
 - 设置好课程时间，可以修改每节课具体的时间，
 - 课表节数按自己需求调，一般教务导入的课表节数可能不符合实际，需要微调
-- 每周起始日建议默认的周一即可（周日起始没测试过可能有bug）
+- 每周起始日建议默认的周一即可
 - 如果导入课表后在小爱课表内修改了课程，直接给bot发送更新课表即可更新本地课表
-- 当你主页的课表和学校课表基本一致时，那么小爱课程表就被调教好了，可以导入了
+- 当你主页的课表和学校课表基本一致时，那么小爱课程表就被设置好了，可以导入了
 
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/settings.jpg)
 
 ## 🐦计划
 
 - [x] 查询下节课的信息
 
@@ -228,27 +244,31 @@
 
 - [ ] 适配更多课表、脱离小爱课表
 
 - [ ] 完善插件
 
 ## 🐛存在的问题
 
- ### 关于定时任务的持久化存储问题：
+> [!NOTE]
+> 在当前版本下，Bot重启后会失去之前创建过的任务，这个问题暂时无法解决
 
-众所周知，使用apscheduler添加的定时任务，会在bot重启后丢失，这是因为使用[nonebot-plugin-apscheduler](https://github.com/nonebot/plugin-apscheduler)创建出来的scheduler，默认使用的JobStore(即保存任务的方式)，是MemoryJobStore，也就是存在内存中，因此会导致重启丢任务。
+众所周知，使用apscheduler添加的定时任务，会在bot重启后丢失，这是因为使用[nonebot-plugin-apscheduler](https://github.com/nonebot/plugin-apscheduler)创建出来的`scheduler`，默认使用的`JobStore`(即保存任务的方式)，是`MemoryJobStore`，也就是存在内存中，因此会导致重启丢任务。
 
-因此参考[apscheduler](https://apscheduler.readthedocs.io/en/latest/userguide.html#configuring-the-scheduler)，你可以在bot的配置文件中添加配置项，让[nonebot-plugin-apscheduler](https://github.com/nonebot/plugin-apscheduler)创建出来的scheduler的默认 JobStore 改为使用数据库，这样就可以持久化存储任务，而不需要额外修改任何东西。
+因此参考[apscheduler](https://apscheduler.readthedocs.io/en/latest/userguide.html#configuring-the-scheduler)，你可以在bot的配置文件中添加配置项，让[nonebot-plugin-apscheduler](https://github.com/nonebot/plugin-apscheduler)创建出来的`scheduler`的默认 `JobStore` 改为使用数据库，这样就可以持久化存储任务，而不需要额外修改任何东西。
 
-然而，很不幸的是，在apscheduler4.0版本之前，所支持的数据库类JobStore都是使用**同步**引擎的，然而[plugin-orm](https://github.com/nonebot/plugin-orm)所采用的是异步引擎，因此你暂时还不能这样做。
+然而，很不幸的是，在`apscheduler4.0`版本之前，所支持的数据库类JobStore都是使用**同步**引擎的，不支持异步引擎，然而[plugin-orm](https://github.com/nonebot/plugin-orm)所采用的是异步引擎，因此你暂时还不能这样做。
 
-所以，暂时还无法解决定时任务的持久化存储问题，除非apscheduler正式发版4.0（目前还是alpha版本），你可以再等待，本插件会持续跟进更新。
+所以，暂时还无法解决定时任务的持久化存储问题，除非`apscheduler`正式发版4.0（目前还是alpha版本），你可以再等待，本插件会持续跟进更新。
 
 ## 🎉致谢
+
 - 感谢[nonebot-plugin-htmlrender](https://github.com/kexue-z/nonebot-plugin-htmlrender)提供的渲染工具
 - 感谢[plugin-orm](https://github.com/nonebot/plugin-orm)提供的异步数据库接口
 - 感谢[nonebot-plugin-apscheduler](https://github.com/nonebot/plugin-apscheduler)提供的定时任务接口
 - 感谢[nonebot-plugin-alconna](https://github.com/nonebot/plugin-alconna)
 - 感谢[Matcha](https://github.com/A-kirami/matcha)提供的简单好用的测试平台
-### 喜欢的话就点个star✨吧
+
+### ✨喜欢的话就点个star吧
+
 或者, 你也可以看我写的其他插件
-[nonebot-plugin-manga-translator](https://github.com/maoxig/nonebot-plugin-manga-translator)一个支持多api, 方便好用的图片/漫画翻译插件
+[nonebot-plugin-manga-translator](https://github.com/maoxig/nonebot-plugin-manga-translator)一个支持多api（包括离线部署）、跨平台、方便好用的图片/漫画翻译插件
```

#### html2text {}

```diff
@@ -1,56 +1,60 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-ai-timetable Version: 0.4.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-ai-timetable Version: 0.4.1 Summary:
 å°ç±è¯¾ç¨è¡¨ Author: maoxiog Author-email: 674550338@qq.com Requires-Python:
 >=3.8,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: httpx (>=0.20.0,<1.0.0) Requires-Dist: nonebot-
 plugin-alconna (>=0.40.1,<1.0.0) Requires-Dist: nonebot-plugin-apscheduler
 (>=0.2.0,<1.0.0) Requires-Dist: nonebot-plugin-htmlrender (>=0.3.0,<0.4.0)
 Requires-Dist: nonebot-plugin-orm (>=0.7.1) Requires-Dist: nonebot2
 (>=2.2.0,<3.0.0) Description-Content-Type: text/markdown
-                                   _[_n_o_n_e_b_o_t_]
-                         # nonebot-plugin-ai-timetable
-â¨*åºäºNonebot2çå¯¹æ¥å°ç±è¯¾ç¨è¡¨çæä»¶*â¨_[_n_o_n_e_b_o_t_]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
+                  _[_n_o_n_e_b_o_t_]# nonebot-plugin-ai-timetable â¨
+ *åºäºNonebot2çå¯¹æ¥å°ç±è¯¾ç¨è¡¨çæä»¶* â¨_[_n_o_n_e_b_o_t_]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
                                    [python]
 ## ð¿å®è£ 1. éè¿`pip`æ`nb`å®è£ï¼ - ä½¿ç¨nb(æ¨è)
 å¨æºå¨äººç®å½ä¸å½ä»¤è¡ä½¿ç¨`nb plugin install
 nonebot_plugin_ai_timetable` - ä½¿ç¨pip: `pip plugin install
 nonebot_plugin_ai_timetable` ç¶åå¨æºå¨äºº`pyproject.toml`éç`plugins =
-[]`åè¡¨è¿½å `"nonebot_plugin_ai_timetable"` 2. æ°æ®å­å¨ä½¿ç¨[plugin-
-orm](https://github.com/nonebot/plugin-orm), æ¥å¥æ°æ®åºï¼æ¹ä¾¿ç®¡ç 3.
-ç¬¬ä¸æ¬¡ä½¿ç¨ä½¿ç¨[plugin-orm](https://github.com/nonebot/plugin-
-orm)æ¶ï¼éè¦ç¨`nb orm upgrade`åçº§æ°æ®åº ## ðç®ä» 1.
+[]`åè¡¨è¿½å `"nonebot_plugin_ai_timetable"` - ä½¿ç¨å¶ä»åç®¡çå¨ï¼
+æ ¹æ®åç®¡çå¨çæä»¤å®è£æä»¶ 2. æ°æ®å­å¨ä½¿ç¨[plugin-orm]
+(https://github.com/nonebot/plugin-orm), ä½¿ç¨`nb orm upgrade`åçº§æ°æ®åº
+> [!WARNING] > ç¬¬ä¸æ¬¡ä½¿ç¨[plugin-orm](https://github.com/nonebot/plugin-
+orm)ï¼æèæä»¶å®ä¹çæ¨¡åæææ´æ°æ¶ï¼éè¦ç¨`nb orm
+upgrade`åçº§æ°æ®åº ## ðç®ä» 1.
 å»çå¼ä¸é®å¯¼å¥å°ç±è¯¾è¡¨ï¼è®©ä½ çbotå®ç°å°ç±è¯¾è¡¨çåè½ 2.
 ç¨æ·è¯¾è¡¨æ°æ®éç¦»ï¼åºäº[plugin-rom](https://github.com/nonebot/
 plugin-orm),
 æ¥å¥æ°æ®åºï¼æ éæå¿è¯¾ç¨æ¶é´å²çªãä¸åå­¦æ ¡è¯¾è¡¨ä¸åç­é®é¢
 3. ééå¤å¹³å°ï¼å³ä½¿æ¯çµæ¥æ¶©æ¶©ç¾¤ä¹è¦å¥½å¥½å­¦ä¹ ï¼ð¥µð¥µ ##
-âï¸æä»¶éç½®
-è¿äºéç½®é½å·²è®¾å¥½é»è®¤å¼ï¼å¦ææ³è¦ä¿®æ¹éç½®ï¼å¨æºå¨äººç®å½ä¸ç.env.*éé¢å¯ä»¥å¡«åä»¥ä¸éé¡¹
-(å¯é) | config | type | default | example | usage | | :--------------------
--: | :---: | :-----: | :------------------------: | :--------------------------
--------------------------------------------------------------------------- | |
-TIMETABLE_PIC | bool | true | TIMETABLE_PIC=false |
-å¯éæ©ææ¥è¯¾è¡¨ä»¥å¾ç/æå­åéï¼é»è®¤ä»¥å¾çåé(true) | |
-TIMETABLE_ALOCK_SOMEDAY | int | 22 | TIMETABLE_ALOCK_SOMEDAY=15 |
+âï¸æä»¶éç½® >[!NOTE] å¯éçæä»¶éç½®
+è¿äºéç½®é½å·²è®¾å¥½é»è®¤å¼ï¼å æ­¤æ¯å¯éçï¼å¦ææ³è¦ä¿®æ¹éç½®ï¼å¨æºå¨äººç®å½ä¸ç.env.*éé¢å¯ä»¥å¡«åä»¥ä¸éé¡¹,
+æªæ¥ä¼èèå¼æ¾æ´å¤çéç½®é¡¹ | config | type | default | example |
+usage | | :---------------------: | :---: | :-----: | :-----------------------
+-: | :-------------------------------------------------------------------------
+--------------------------- | | TIMETABLE_PIC | bool | true |
+TIMETABLE_PIC=false | å¯éæ©ææ¥è¯¾è¡¨ä»¥å¾ç/
+æå­åéï¼é»è®¤ä»¥å¾çåé(true) | | TIMETABLE_ALOCK_SOMEDAY | int |
+22 | TIMETABLE_ALOCK_SOMEDAY=15 |
 è®¢éææ¥è¯¾è¡¨çåéæ¶é´ï¼å¿é¡»æ¯0-24çæ°å­ | |
 TIMETABLE_ALOCK_8 | int | 21 | TIMETABLE_ALOCK_8=16 |
 è®¢éæ©å«çåéæ¶é´ï¼å¿é¡»æ¯0-
 24çæ°å­.è¿éåéçé½æ¯ç¬¬äºå¤©çï¼æä»¥å»ºè®®è®¾ç½®ä¸º18-23ç¹ |
 | TIMETABLE_SEND_TIME | float | 0.5 | TIMETABLE_SEND_TIME=1 |
 è®¢éè¯¾ç¨æååéçæ¶é´ï¼åä½æ¯`å°æ¶`ï¼å¯ä»¥æ¯æ´æ°ä¹å¯ä»¥æ¯å°æ°ï¼å»ºè®®ä¸è¦è®¾çå¤ªå¤§ï¼é¿ååºç°æ æ³é¢æçbug
-| ## ð¿ä¾èµ
+| ## ð¿ä¾èµ > [!NOTE] >
 æä»¶ä¾èµä¼å¨å®è£æ¶èªå¨å®è£ï¼å¦æå®è£å¤±è´¥ï¼ä½ å¯ä»¥æç§ä»¥ä¸æä»¤æå¨åæ¬¡å®è£
 ```python nb plugin install nonebot_plugin_htmlrender nb plugin install
 nonebot_plugin_apscheduler nb plugin install nonebot_plugin_alconna nb plugin
-install nonebot_plugin_orm ``` ## ðæ´æ°æ¥å¿ ç¹å»å±å¼ - 0.4.0 / 2024-
-04-30: 1. éæå®æï¼å°æææ°æ®è¿ç§»å°å®æ¹æ°æ®åºæä»¶[plugin-
-orm](https://github.com/nonebot/plugin-orm)ï¼ä¹åçæ°æ®å¤±æ 2.
+install nonebot_plugin_orm ``` ## ðæ´æ°æ¥å¿ ç¹å»å±å¼ - 0.4.1 / 2024-
+05-07: 1. ä¿®å¤å®æ¶æéä¸ç´åéçé®é¢ 2. æ´æ°README.md 3.
+ä¿®å¤type hintéè¯¯ - 0.4.0 / 2024-04-30: 1.
+éæå®æï¼å°æææ°æ®è¿ç§»å°å®æ¹æ°æ®åºæä»¶[plugin-orm](https:
+//github.com/nonebot/plugin-orm)ï¼ä¹åçæ°æ®å¤±æ 2.
 ä¿®æ¹äºæä»¶è§¦åæä»¤åç¸å³é»è¾ 3.
 éæææä»£ç ï¼ä¼åå¤çé»è¾
 >è¯¥çæ¬æ¯ç ´åæ§æ´æ°ï¼ä¸ä»å¨æµè¯ä¸­ï¼æä»»ä½çé®æ¬¢è¿issueæpr
 - 0.3.8 / 2024-04-28: 1. ä¿®å¤è®¾ç½®éè¯¯ 2. éæä»£ç  - 0.3.7 / 2024-04-
 24: 1. æ´æ°Nonebot2çæ¬è³2.2.0 2. åºäº [nonebot-plugin-alconna](https://
 github.com/nonebot/plugin-alconna) ééå¤å¹³å° 3.
 æ¾å®½httpxéå¶ï¼ç§»é¤onebotä¾èµ - 0.3.6 / 2023-09-02: 1.
@@ -72,77 +76,78 @@
 æ°å¢3é¡¹éç½®é¡¹ï¼ææ¥è¯¾è¡¨å¯éæ©ä»¥å¾çåéï¼é»è®¤ä¸ºå¾çï¼
 - 0.1.8 / 2023-03-08: 1. ä¿®æ¹é¨åä»£ç ï¼ä¼åè¯¾è¡¨æ ¼å¼ 2.
 ä¿®å¤äºèæ°ä¸º11çè¯¾ä¼æå¨èæ°ä¸º2çè¯¾ç¨åé¢çbug
 (QAQå¤ªè ¢äºå«éªäºå«éªäº) - 0.1.7 / 2023-03-07: 1.
 ä¿®å¤äºæ¶é´ä¸ä¼èªå·±æ¹åçbug 2. æ°å¢äºä¸è¯¾/ä¸èè¯¾åè½ 3.
 ä¼åäºä¸äºå±å±±ä»£ç  - 0.1.5 / 2023-03-06: 1.
 æ°å¢äºç§èè®¢éè¯¾è¡¨|æ©å«çåè½ - 0.1.4 / 2023-03-05: 1.
-ä¿®å¤äºæ æ³åæ¶è®¢éæ©å«çbug ## ðå½ä»¤ 1.
-è¯¾è¡¨å¸®å©ï¼è·åæ¬æ¡å¸®å© 2.
+ä¿®å¤äºæ æ³åæ¶è®¢éæ©å«çbug ## ðå½ä»¤ -
+è¯¾è¡¨å¸®å©ï¼è·åæ¬æ¡å¸®å© -
 å¯¼å¥è¯¾è¡¨ï¼éè¦æå°ç±è¯¾è¡¨åäº«åºæ¥çé¾æ¥ï¼æå¼å°ç±è¯¾ç¨è¡¨ï¼æå¨æ·»å è¯¾ç¨æä»æå¡å¯¼å¥
 (å·²ééäºå¤§é¨åé«æ ¡)è¯¾ç¨å ![Image text](https://github.com/maoxig/
 nonebot-plugin-ai-timetable/blob/main/resource/export.jpg)
 å¨åºæ¬è®¾ç½®éæå¼å§ä¸è¯¾æ¶é´ç­è°æ´å¥½ä¹å
 (å°¤å¶æ¯æ¶é´ãèæ°)ï¼æåäº«è¯¾è¡¨å¾å°çé¾æ¥åéç»botå³å¯å¯¼å¥æ¬å°
-(åäº«åéè¦ç»å½å°ç±³è´¦æ· [#1](https://github.com/maoxig/nonebot-
-plugin-ai-timetable/issues/1)) 3.
+> [!NOTE] > å¨åäº«åï¼ä½ éè¦ç»å½å°ç±³è´¦æ· [#1](https://github.com/
+maoxig/nonebot-plugin-ai-timetable/issues/1) -
 æ´æ°è¯¾è¡¨ï¼å¦æå¨å°ç±è¯¾ç¨è¡¨éä¿®æ¹äºè¯¾ç¨ï¼åéè¯¥æ¡æä»¤å³å¯æ´æ°æ¬å°çè¯¾è¡¨ï¼æ ééæ°å¯¼å¥
-4. æ¥è¯¢è¯¾è¡¨+[åæ°]ï¼æ¥è¯¢[åæ°]çè¯¾è¡¨ï¼åæ°æ¯æ[æ¬å¨/
-ä¸å¨ãå¨xãæ¨å¤©/ä»å¤©/æå¤©/åå¤©ãæ©å«ãè¯¾ç¨å] 5.
-æ·»å è¯¾ç¨æé+[åæ°]ï¼åæ°æ¯æ[å¨xãæ©å«ãè¯¾ç¨å] 6.
+- æ¥è¯¢è¯¾è¡¨+[åæ°]ï¼æ¥è¯¢[åæ°]çè¯¾è¡¨ï¼åæ°æ¯æ[æ¬å¨/
+ä¸å¨ãå¨xãæ¨å¤©/ä»å¤©/æå¤©/åå¤©ãæ©å«ãè¯¾ç¨åãä¸èè¯¾] -
+æ·»å è¯¾ç¨æé+[åæ°]ï¼åæ°æ¯æ[å¨xãæ©å«ãè¯¾ç¨å] -
 å é¤è¯¾ç¨æé+[åæ°]ï¼åæ°æ¯æ[å¨é¨ãå¨xãæ©å«ãè¯¾ç¨å]
-7. æ¥çè¯¾ç¨æéï¼æ¥çå½åå·²ç»æ·»å çè¯¾ç¨æé ## â­ææå¾
+- æ¥çè¯¾ç¨æéï¼æ¥çå½åå·²ç»æ·»å çè¯¾ç¨æé ## â­ææå¾
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/
 resource/update.png) ![Image text](https://github.com/maoxig/nonebot-plugin-ai-
 timetable/blob/main/resource/query.png) ![Image text](https://github.com/
 maoxig/nonebot-plugin-ai-timetable/blob/main/resource/query1.png) ![Image text]
 (https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/
 query1.png) ![Image text](https://github.com/maoxig/nonebot-plugin-ai-
 timetable/blob/main/resource/reminder.png) ![Image text](https://github.com/
 maoxig/nonebot-plugin-ai-timetable/blob/main/resource/reminder1.png) ![Image
 text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/
-someday_classes_pic.jpg) ### å³äºå°ç±è¯¾ç¨è¡¨åçä¸äºè¯´æ å¦ä¸å¾
-- ç¬¬ä¸æ¬¡ä½¿ç¨æ¬æä»¶æ¶ï¼éè¦ç¨`nb orm upgrade`åçº§æ°æ®åº -
+someday_classes_pic.jpg) ### ð¥æä¸ç¥éæä¹ä½¿ç¨å°ç±è¯¾ç¨è¡¨
+å¦ä¸å¾ -
 é¦åè¦ç»å½ä¸å°ç±³è´¦æ·,å¦åå¯è½è·åå°éè¯¯çè¯¾è¡¨ä¿¡æ¯ [#1]
 (https://github.com/maoxig/nonebot-plugin-ai-timetable/issues/1) -
 è®¾ç½®å¥½å¼å§ä¸è¯¾æ¶é´ -
 è®¾ç½®å¥½è¯¾ç¨æ¶é´ï¼å¯ä»¥ä¿®æ¹æ¯èè¯¾å·ä½çæ¶é´ï¼ -
 è¯¾è¡¨èæ°æèªå·±éæ±è°ï¼ä¸è¬æå¡å¯¼å¥çè¯¾è¡¨èæ°å¯è½ä¸ç¬¦åå®éï¼éè¦å¾®è°
--
-æ¯å¨èµ·å§æ¥å»ºè®®é»è®¤çå¨ä¸å³å¯ï¼å¨æ¥èµ·å§æ²¡æµè¯è¿å¯è½æbugï¼
--
+- æ¯å¨èµ·å§æ¥å»ºè®®é»è®¤çå¨ä¸å³å¯ -
 å¦æå¯¼å¥è¯¾è¡¨åå¨å°ç±è¯¾è¡¨åä¿®æ¹äºè¯¾ç¨ï¼ç´æ¥ç»botåéæ´æ°è¯¾è¡¨å³å¯æ´æ°æ¬å°è¯¾è¡¨
 -
-å½ä½ ä¸»é¡µçè¯¾è¡¨åå­¦æ ¡è¯¾è¡¨åºæ¬ä¸è´æ¶ï¼é£ä¹å°ç±è¯¾ç¨è¡¨å°±è¢«è°æå¥½äºï¼å¯ä»¥å¯¼å¥äº
+å½ä½ ä¸»é¡µçè¯¾è¡¨åå­¦æ ¡è¯¾è¡¨åºæ¬ä¸è´æ¶ï¼é£ä¹å°ç±è¯¾ç¨è¡¨å°±è¢«è®¾ç½®å¥½äºï¼å¯ä»¥å¯¼å¥äº
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/
 resource/settings.jpg) ## ð¦è®¡å - [x] æ¥è¯¢ä¸èè¯¾çä¿¡æ¯ - [x]
 å¯éæ©æ¯å¦åéå¾çä»¥é¿åé£æ§ - [x] å¢å æ´å¤çéç½®é¡¹ - [x]
 éæä»£ç  - [x] è®¢éæå®çè¯¾ - [x] å¤å¹³å°éé, åºäº [nonebot-
 plugin-alconna](https://github.com/nonebot/plugin-alconna) - [x]
 æ¯æå®æ¶ä»»å¡æ¬å°å­å¨ - [x] éé[plugin-orm](https://github.com/
 nonebot/plugin-orm), æ¥å¥æ°æ®åº - [ ]
 ééæ´å¤è¯¾è¡¨ãè±ç¦»å°ç±è¯¾è¡¨ - [ ] å®åæä»¶ ##
-ðå­å¨çé®é¢ ### å³äºå®æ¶ä»»å¡çæä¹åå­å¨é®é¢ï¼
+ðå­å¨çé®é¢ > [!NOTE] >
+å¨å½åçæ¬ä¸ï¼Botéå¯åä¼å¤±å»ä¹ååå»ºè¿çä»»å¡ï¼è¿ä¸ªé®é¢ææ¶æ æ³è§£å³
 ä¼æå¨ç¥ï¼ä½¿ç¨apscheduleræ·»å çå®æ¶ä»»å¡ï¼ä¼å¨botéå¯åä¸¢å¤±ï¼è¿æ¯å ä¸ºä½¿ç¨
 [nonebot-plugin-apscheduler](https://github.com/nonebot/plugin-
-apscheduler)åå»ºåºæ¥çschedulerï¼é»è®¤ä½¿ç¨çJobStore
-(å³ä¿å­ä»»å¡çæ¹å¼)ï¼æ¯MemoryJobStoreï¼ä¹å°±æ¯å­å¨åå­ä¸­ï¼å æ­¤ä¼å¯¼è´éå¯ä¸¢ä»»å¡ã
+apscheduler)åå»ºåºæ¥ç`scheduler`ï¼é»è®¤ä½¿ç¨ç`JobStore`
+(å³ä¿å­ä»»å¡çæ¹å¼)ï¼æ¯`MemoryJobStore`ï¼ä¹å°±æ¯å­å¨åå­ä¸­ï¼å æ­¤ä¼å¯¼è´éå¯ä¸¢ä»»å¡ã
 å æ­¤åè[apscheduler](https://apscheduler.readthedocs.io/en/latest/
 userguide.html#configuring-the-
 scheduler)ï¼ä½ å¯ä»¥å¨botçéç½®æä»¶ä¸­æ·»å éç½®é¡¹ï¼è®©[nonebot-
 plugin-apscheduler](https://github.com/nonebot/plugin-
-apscheduler)åå»ºåºæ¥çschedulerçé»è®¤ JobStore
+apscheduler)åå»ºåºæ¥ç`scheduler`çé»è®¤ `JobStore`
 æ¹ä¸ºä½¿ç¨æ°æ®åºï¼è¿æ ·å°±å¯ä»¥æä¹åå­å¨ä»»å¡ï¼èä¸éè¦é¢å¤ä¿®æ¹ä»»ä½ä¸è¥¿ã
-ç¶èï¼å¾ä¸å¹¸çæ¯ï¼å¨apscheduler4.0çæ¬ä¹åï¼ææ¯æçæ°æ®åºç±»JobStoreé½æ¯ä½¿ç¨**åæ­¥**å¼æçï¼ç¶è
+ç¶èï¼å¾ä¸å¹¸çæ¯ï¼å¨`apscheduler4.0`çæ¬ä¹åï¼ææ¯æçæ°æ®åºç±»JobStoreé½æ¯ä½¿ç¨**åæ­¥**å¼æçï¼ä¸æ¯æå¼æ­¥å¼æï¼ç¶è
 [plugin-orm](https://github.com/nonebot/plugin-
 orm)æéç¨çæ¯å¼æ­¥å¼æï¼å æ­¤ä½ ææ¶è¿ä¸è½è¿æ ·åã
-æä»¥ï¼ææ¶è¿æ æ³è§£å³å®æ¶ä»»å¡çæä¹åå­å¨é®é¢ï¼é¤éapscheduleræ­£å¼åç4.0ï¼ç®åè¿æ¯alphaçæ¬ï¼ï¼ä½ å¯ä»¥åç­å¾ï¼æ¬æä»¶ä¼æç»­è·è¿æ´æ°ã
+æä»¥ï¼ææ¶è¿æ æ³è§£å³å®æ¶ä»»å¡çæä¹åå­å¨é®é¢ï¼é¤é`apscheduler`æ­£å¼åç4.0ï¼ç®åè¿æ¯alphaçæ¬ï¼ï¼ä½ å¯ä»¥åç­å¾ï¼æ¬æä»¶ä¼æç»­è·è¿æ´æ°ã
 ## ðè´è°¢ - æè°¢[nonebot-plugin-htmlrender](https://github.com/kexue-z/
 nonebot-plugin-htmlrender)æä¾çæ¸²æå·¥å· - æè°¢[plugin-orm](https://
 github.com/nonebot/plugin-orm)æä¾çå¼æ­¥æ°æ®åºæ¥å£ - æè°¢[nonebot-
 plugin-apscheduler](https://github.com/nonebot/plugin-
 apscheduler)æä¾çå®æ¶ä»»å¡æ¥å£ - æè°¢[nonebot-plugin-alconna](https:
 //github.com/nonebot/plugin-alconna) - æè°¢[Matcha](https://github.com/A-
 kirami/matcha)æä¾çç®åå¥½ç¨çæµè¯å¹³å° ###
-åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§ æè, ä½ ä¹å¯ä»¥çæåçå¶ä»æä»¶
+â¨åæ¬¢çè¯å°±ç¹ä¸ªstarå§ æè, ä½ ä¹å¯ä»¥çæåçå¶ä»æä»¶
 [nonebot-plugin-manga-translator](https://github.com/maoxig/nonebot-plugin-
-manga-translator)ä¸ä¸ªæ¯æå¤api, æ¹ä¾¿å¥½ç¨çå¾ç/æ¼«ç»ç¿»è¯æä»¶
+manga-
+translator)ä¸ä¸ªæ¯æå¤apiï¼åæ¬ç¦»çº¿é¨ç½²ï¼ãè·¨å¹³å°ãæ¹ä¾¿å¥½ç¨çå¾ç/
+æ¼«ç»ç¿»è¯æä»¶
```

