# Comparing `tmp/nonebot_plugin_with_ai_agents-0.1.1.tar.gz` & `tmp/nonebot_plugin_with_ai_agents-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_with_ai_agents-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_with_ai_agents-0.1.2.tar", max compression
```

## Comparing `nonebot_plugin_with_ai_agents-0.1.1.tar` & `nonebot_plugin_with_ai_agents-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      414 2024-05-07 08:17:46.045650 nonebot_plugin_with_ai_agents-0.1.1/nonebot_plugin_with_ai_agents/__init__.py
--rw-r--r--   0        0        0      519 2024-05-06 07:05:33.777069 nonebot_plugin_with_ai_agents-0.1.1/nonebot_plugin_with_ai_agents/handler.py
--rw-r--r--   0        0        0        2 2024-05-06 07:05:33.777069 nonebot_plugin_with_ai_agents-0.1.1/nonebot_plugin_with_ai_agents/llm/__init__.py
--rw-r--r--   0        0        0     4529 2024-05-07 10:03:19.704778 nonebot_plugin_with_ai_agents-0.1.1/nonebot_plugin_with_ai_agents/llm/agents.py
--rw-r--r--   0        0        0     2866 2024-05-06 07:05:33.778077 nonebot_plugin_with_ai_agents-0.1.1/nonebot_plugin_with_ai_agents/llm/central_brain.py
--rw-r--r--   0        0        0      675 2024-05-06 07:05:33.778077 nonebot_plugin_with_ai_agents-0.1.1/nonebot_plugin_with_ai_agents/llm/config.py
--rw-r--r--   0        0        0      131 2024-05-06 07:05:33.778077 nonebot_plugin_with_ai_agents-0.1.1/nonebot_plugin_with_ai_agents/llm/llms/__init__.py
--rw-r--r--   0        0        0      453 2024-05-07 11:12:58.483693 nonebot_plugin_with_ai_agents-0.1.1/nonebot_plugin_with_ai_agents/llm/llms/base.py
--rw-r--r--   0        0        0     2277 2024-05-07 11:13:28.157800 nonebot_plugin_with_ai_agents-0.1.1/nonebot_plugin_with_ai_agents/llm/llms/dashscope.py
--rw-r--r--   0        0        0     1942 2024-05-07 11:13:28.219069 nonebot_plugin_with_ai_agents-0.1.1/nonebot_plugin_with_ai_agents/llm/llms/glm.py
--rw-r--r--   0        0        0     2046 2024-05-07 11:13:28.141789 nonebot_plugin_with_ai_agents-0.1.1/nonebot_plugin_with_ai_agents/llm/llms/openai.py
--rw-r--r--   0        0        0       19 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.1/nonebot_plugin_with_ai_agents/llm/mem_stores.py
--rw-r--r--   0        0        0      338 2024-05-07 08:06:18.016313 nonebot_plugin_with_ai_agents-0.1.1/nonebot_plugin_with_ai_agents/llm/services.py
--rw-r--r--   0        0        0        0 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.1/nonebot_plugin_with_ai_agents/llm/utils/__init__.py
--rw-r--r--   0        0        0     4648 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.1/nonebot_plugin_with_ai_agents/llm/utils/prompts.py
--rw-r--r--   0        0        0     3358 2024-05-07 10:03:19.714495 nonebot_plugin_with_ai_agents-0.1.1/nonebot_plugin_with_ai_agents/llm/utils/retrievers.py
--rw-r--r--   0        0        0      831 2024-05-07 16:05:11.991696 nonebot_plugin_with_ai_agents-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4310 2024-05-07 15:18:47.979516 nonebot_plugin_with_ai_agents-0.1.1/README.md
--rw-r--r--   0        0        0     5279 1970-01-01 00:00:00.000000 nonebot_plugin_with_ai_agents-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      414 2024-05-07 08:17:46.045650 nonebot_plugin_with_ai_agents-0.1.2/nonebot_plugin_with_ai_agents/__init__.py
+-rw-r--r--   0        0        0      519 2024-05-06 07:05:33.777069 nonebot_plugin_with_ai_agents-0.1.2/nonebot_plugin_with_ai_agents/handler.py
+-rw-r--r--   0        0        0        2 2024-05-06 07:05:33.777069 nonebot_plugin_with_ai_agents-0.1.2/nonebot_plugin_with_ai_agents/llm/__init__.py
+-rw-r--r--   0        0        0     4529 2024-05-07 10:03:19.704778 nonebot_plugin_with_ai_agents-0.1.2/nonebot_plugin_with_ai_agents/llm/agents.py
+-rw-r--r--   0        0        0     2866 2024-05-06 07:05:33.778077 nonebot_plugin_with_ai_agents-0.1.2/nonebot_plugin_with_ai_agents/llm/central_brain.py
+-rw-r--r--   0        0        0      675 2024-05-06 07:05:33.778077 nonebot_plugin_with_ai_agents-0.1.2/nonebot_plugin_with_ai_agents/llm/config.py
+-rw-r--r--   0        0        0      131 2024-05-06 07:05:33.778077 nonebot_plugin_with_ai_agents-0.1.2/nonebot_plugin_with_ai_agents/llm/llms/__init__.py
+-rw-r--r--   0        0        0      453 2024-05-07 11:12:58.483693 nonebot_plugin_with_ai_agents-0.1.2/nonebot_plugin_with_ai_agents/llm/llms/base.py
+-rw-r--r--   0        0        0     2277 2024-05-07 11:13:28.157800 nonebot_plugin_with_ai_agents-0.1.2/nonebot_plugin_with_ai_agents/llm/llms/dashscope.py
+-rw-r--r--   0        0        0     1942 2024-05-07 11:13:28.219069 nonebot_plugin_with_ai_agents-0.1.2/nonebot_plugin_with_ai_agents/llm/llms/glm.py
+-rw-r--r--   0        0        0     2046 2024-05-07 11:13:28.141789 nonebot_plugin_with_ai_agents-0.1.2/nonebot_plugin_with_ai_agents/llm/llms/openai.py
+-rw-r--r--   0        0        0       19 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.2/nonebot_plugin_with_ai_agents/llm/mem_stores.py
+-rw-r--r--   0        0        0      338 2024-05-07 08:06:18.016313 nonebot_plugin_with_ai_agents-0.1.2/nonebot_plugin_with_ai_agents/llm/services.py
+-rw-r--r--   0        0        0        0 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.2/nonebot_plugin_with_ai_agents/llm/utils/__init__.py
+-rw-r--r--   0        0        0     4648 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.2/nonebot_plugin_with_ai_agents/llm/utils/prompts.py
+-rw-r--r--   0        0        0     3358 2024-05-07 10:03:19.714495 nonebot_plugin_with_ai_agents-0.1.2/nonebot_plugin_with_ai_agents/llm/utils/retrievers.py
+-rw-r--r--   0        0        0      695 2024-05-07 16:26:32.357465 nonebot_plugin_with_ai_agents-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4310 2024-05-07 15:18:47.979516 nonebot_plugin_with_ai_agents-0.1.2/README.md
+-rw-r--r--   0        0        0     5143 1970-01-01 00:00:00.000000 nonebot_plugin_with_ai_agents-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_with_ai_agents-0.1.1/nonebot_plugin_with_ai_agents/handler.py` & `nonebot_plugin_with_ai_agents-0.1.2/nonebot_plugin_with_ai_agents/handler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.1/nonebot_plugin_with_ai_agents/llm/agents.py` & `nonebot_plugin_with_ai_agents-0.1.2/nonebot_plugin_with_ai_agents/llm/agents.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.1/nonebot_plugin_with_ai_agents/llm/central_brain.py` & `nonebot_plugin_with_ai_agents-0.1.2/nonebot_plugin_with_ai_agents/llm/central_brain.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.1/nonebot_plugin_with_ai_agents/llm/config.py` & `nonebot_plugin_with_ai_agents-0.1.2/nonebot_plugin_with_ai_agents/llm/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.1/nonebot_plugin_with_ai_agents/llm/llms/dashscope.py` & `nonebot_plugin_with_ai_agents-0.1.2/nonebot_plugin_with_ai_agents/llm/llms/dashscope.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.1/nonebot_plugin_with_ai_agents/llm/llms/glm.py` & `nonebot_plugin_with_ai_agents-0.1.2/nonebot_plugin_with_ai_agents/llm/llms/glm.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.1/nonebot_plugin_with_ai_agents/llm/llms/openai.py` & `nonebot_plugin_with_ai_agents-0.1.2/nonebot_plugin_with_ai_agents/llm/llms/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.1/nonebot_plugin_with_ai_agents/llm/utils/prompts.py` & `nonebot_plugin_with_ai_agents-0.1.2/nonebot_plugin_with_ai_agents/llm/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.1/nonebot_plugin_with_ai_agents/llm/utils/retrievers.py` & `nonebot_plugin_with_ai_agents-0.1.2/nonebot_plugin_with_ai_agents/llm/utils/retrievers.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.1/README.md` & `nonebot_plugin_with_ai_agents-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.1/PKG-INFO` & `nonebot_plugin_with_ai_agents-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-with-ai-agents
-Version: 0.1.1
-Summary: nonebot-plugin-with-ai-agents 是一个基于基本原理实现的 AI Agents（智能体），目前实现了联网搜索能力（实时搜索等）、页面内容提取并学习回答、命令执行（这个能力有一定的安全风险，毕竟初版所以暂时不打算解决）。这个模块现在以 Nonebot2 插件形式展现
+Version: 0.1.2
+Summary: nonebot_plugin_with_ai_agents 是一个基于基本原理实现的 AI Agents（智能体），拥有联网搜索能力（实时搜索等）、页面内容提取并学习回答、命令执行等功能
 Author: yejue
 Author-email: 1145331931@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-with-ai-agents Version: 0.1.1
-Summary: nonebot-plugin-with-ai-agents æ¯ä¸ä¸ªåºäºåºæ¬åçå®ç°ç AI
-Agentsï¼æºè½ä½ï¼ï¼ç®åå®ç°äºèç½æç´¢è½åï¼å®æ¶æç´¢ç­ï¼ãé¡µé¢åå®¹æåå¹¶å­¦ä¹ åç­ãå½ä»¤æ§è¡ï¼è¿ä¸ªè½åæä¸å®çå®å¨é£é©ï¼æ¯ç«åçæä»¥ææ¶ä¸æç®è§£å³ï¼ãè¿ä¸ªæ¨¡åç°å¨ä»¥
-Nonebot2 æä»¶å½¢å¼å±ç° Author: yejue Author-email: 1145331931@qq.com
-Requires-Python: >=3.8,<4.0 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.12 Requires-Dist: beautifulsoup4 Requires-Dist:
-nonebot2 (>=2.0,<3.0) Project-URL: homepage, https://github.com/yejue/nonebot-
-plugin-with-ai-agents Project-URL: repository, https://github.com/yejue/
-nonebot-plugin-with-ai-agents Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: nonebot-plugin-with-ai-agents Version: 0.1.2
+Summary: nonebot_plugin_with_ai_agents æ¯ä¸ä¸ªåºäºåºæ¬åçå®ç°ç AI
+Agentsï¼æºè½ä½ï¼ï¼æ¥æèç½æç´¢è½åï¼å®æ¶æç´¢ç­ï¼ãé¡µé¢åå®¹æåå¹¶å­¦ä¹ åç­ãå½ä»¤æ§è¡ç­åè½
+Author: yejue Author-email: 1145331931@qq.com Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: beautifulsoup4 Requires-Dist: nonebot2 (>=2.0,<3.0) Project-URL:
+homepage, https://github.com/yejue/nonebot-plugin-with-ai-agents Project-URL:
+repository, https://github.com/yejue/nonebot-plugin-with-ai-agents Description-
+Content-Type: text/markdown
                                    _[_n_o_n_e_b_o_t_]
                          ************ WWiitthh--AAII--AAggeennttss ************
 _â¨ NoneBot AI
 å©çæä»¶ï¼æé¡µé¢åå®¹å­¦ä¹ ãé¡µé¢åå®¹æåãèç½å®æ¶æ¥è¯¢åç­ãå¤©æ°æ¥è¯¢ãå½ä»¤æ§è¡ç­åè½
 â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## å¿«éå®è£ ```shell å¾æ´æ° ``` ## åè½æè¿° AI Agents
```

