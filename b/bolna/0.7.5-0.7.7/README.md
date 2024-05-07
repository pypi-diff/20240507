# Comparing `tmp/bolna-0.7.5.tar.gz` & `tmp/bolna-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bolna-0.7.5.tar", last modified: Sun Mar 24 20:35:14 2024, max compression
+gzip compressed data, was "bolna-0.7.7.tar", last modified: Tue May  7 18:45:57 2024, max compression
```

## Comparing `bolna-0.7.5.tar` & `bolna-0.7.7.tar`

### file list

```diff
@@ -1,77 +1,80 @@
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-03-24 20:35:14.710244 bolna-0.7.5/
--rw-r--r--   0 xan        (501) staff       (20)    34522 2024-03-11 19:09:56.000000 bolna-0.7.5/LICENSE
--rw-r--r--   0 xan        (501) staff       (20)    48259 2024-03-24 20:35:14.709873 bolna-0.7.5/PKG-INFO
--rw-r--r--   0 xan        (501) staff       (20)     7377 2024-03-22 13:50:32.000000 bolna-0.7.5/README.md
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-03-24 20:35:14.693939 bolna-0.7.5/bolna/
--rw-r--r--   0 xan        (501) staff       (20)      330 2024-03-24 20:33:42.000000 bolna-0.7.5/bolna/__init__.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-03-24 20:35:14.696370 bolna-0.7.5/bolna/agent_manager/
--rw-r--r--   0 xan        (501) staff       (20)      124 2024-01-07 06:26:49.000000 bolna-0.7.5/bolna/agent_manager/__init__.py
--rw-r--r--   0 xan        (501) staff       (20)     3040 2024-03-22 13:50:32.000000 bolna-0.7.5/bolna/agent_manager/assistant_manager.py
--rw-r--r--   0 xan        (501) staff       (20)      174 2024-01-07 16:40:54.000000 bolna-0.7.5/bolna/agent_manager/base_manager.py
--rw-r--r--   0 xan        (501) staff       (20)    59711 2024-03-24 20:33:20.000000 bolna-0.7.5/bolna/agent_manager/task_manager.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-03-24 20:35:14.698875 bolna-0.7.5/bolna/agent_types/
--rw-r--r--   0 xan        (501) staff       (20)      300 2024-03-22 13:50:32.000000 bolna-0.7.5/bolna/agent_types/__init__.py
--rw-r--r--   0 xan        (501) staff       (20)      176 2024-01-07 16:40:54.000000 bolna-0.7.5/bolna/agent_types/base_agent.py
--rw-r--r--   0 xan        (501) staff       (20)     1340 2024-02-08 16:20:46.000000 bolna-0.7.5/bolna/agent_types/contextual_conversational_agent.py
--rw-r--r--   0 xan        (501) staff       (20)      653 2024-02-08 16:20:46.000000 bolna-0.7.5/bolna/agent_types/extraction_agent.py
--rw-r--r--   0 xan        (501) staff       (20)     6302 2024-03-22 13:50:32.000000 bolna-0.7.5/bolna/agent_types/graph_based_conversational_agent.py
--rw-r--r--   0 xan        (501) staff       (20)      906 2024-03-22 13:50:32.000000 bolna-0.7.5/bolna/agent_types/summarization_agent.py
--rw-r--r--   0 xan        (501) staff       (20)     1199 2024-03-23 20:32:29.000000 bolna-0.7.5/bolna/agent_types/zapier_agent.py
--rw-r--r--   0 xan        (501) staff       (20)     1807 2024-01-19 12:02:21.000000 bolna-0.7.5/bolna/assistant.py
--rw-r--r--   0 xan        (501) staff       (20)      937 2024-03-22 13:50:32.000000 bolna-0.7.5/bolna/constants.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-03-24 20:35:14.700416 bolna-0.7.5/bolna/helpers/
--rw-r--r--   0 xan        (501) staff       (20)        0 2023-12-23 18:13:48.000000 bolna-0.7.5/bolna/helpers/__init__.py
--rw-r--r--   0 xan        (501) staff       (20)     9978 2024-03-22 13:50:32.000000 bolna-0.7.5/bolna/helpers/analytics_helpers.py
--rw-r--r--   0 xan        (501) staff       (20)        0 2024-01-12 18:42:30.000000 bolna-0.7.5/bolna/helpers/cache_helpers.py
--rw-r--r--   0 xan        (501) staff       (20)      548 2024-01-07 16:40:54.000000 bolna-0.7.5/bolna/helpers/logger_config.py
--rw-r--r--   0 xan        (501) staff       (20)    13039 2024-03-23 20:32:29.000000 bolna-0.7.5/bolna/helpers/utils.py
--rw-r--r--   0 xan        (501) staff       (20)     3929 2024-03-22 13:50:32.000000 bolna-0.7.5/bolna/helpers/vad.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-03-24 20:35:14.701388 bolna-0.7.5/bolna/input_handlers/
--rw-r--r--   0 xan        (501) staff       (20)      159 2024-03-22 13:50:32.000000 bolna-0.7.5/bolna/input_handlers/__init__.py
--rw-r--r--   0 xan        (501) staff       (20)     3368 2024-01-19 12:02:21.000000 bolna-0.7.5/bolna/input_handlers/default.py
--rw-r--r--   0 xan        (501) staff       (20)     4547 2024-03-22 13:50:32.000000 bolna-0.7.5/bolna/input_handlers/telephony.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-03-24 20:35:14.701908 bolna-0.7.5/bolna/input_handlers/telephony_providers/
--rw-r--r--   0 xan        (501) staff       (20)      664 2024-03-22 13:50:32.000000 bolna-0.7.5/bolna/input_handlers/telephony_providers/exotel.py
--rw-r--r--   0 xan        (501) staff       (20)      662 2024-03-22 13:50:32.000000 bolna-0.7.5/bolna/input_handlers/telephony_providers/twilio.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-03-24 20:35:14.703781 bolna-0.7.5/bolna/llms/
--rw-r--r--   0 xan        (501) staff       (20)       63 2023-12-23 22:38:43.000000 bolna-0.7.5/bolna/llms/__init__.py
--rw-r--r--   0 xan        (501) staff       (20)     3900 2024-03-23 20:32:29.000000 bolna-0.7.5/bolna/llms/litellm.py
--rw-r--r--   0 xan        (501) staff       (20)      424 2024-01-21 12:08:04.000000 bolna-0.7.5/bolna/llms/llm.py
--rw-r--r--   0 xan        (501) staff       (20)     4652 2024-03-23 20:32:29.000000 bolna-0.7.5/bolna/llms/openai_llm.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-03-24 20:35:14.690968 bolna-0.7.5/bolna/memory/
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-03-24 20:35:14.704726 bolna-0.7.5/bolna/memory/cache/
--rw-r--r--   0 xan        (501) staff       (20)      161 2024-01-12 18:42:30.000000 bolna-0.7.5/bolna/memory/cache/BaseCache.py
--rw-r--r--   0 xan        (501) staff       (20)       54 2024-01-12 18:42:30.000000 bolna-0.7.5/bolna/memory/cache/__init__.py
--rw-r--r--   0 xan        (501) staff       (20)      891 2024-01-12 18:42:30.000000 bolna-0.7.5/bolna/memory/cache/inmemory_scalar_cache.py
--rw-r--r--   0 xan        (501) staff       (20)     4033 2024-03-22 13:50:32.000000 bolna-0.7.5/bolna/models.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-03-24 20:35:14.705346 bolna-0.7.5/bolna/output_handlers/
--rw-r--r--   0 xan        (501) staff       (20)      162 2024-03-22 13:50:32.000000 bolna-0.7.5/bolna/output_handlers/__init__.py
--rw-r--r--   0 xan        (501) staff       (20)     1492 2024-03-22 13:50:32.000000 bolna-0.7.5/bolna/output_handlers/default.py
--rw-r--r--   0 xan        (501) staff       (20)     2028 2024-03-22 13:50:32.000000 bolna-0.7.5/bolna/output_handlers/telephony.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-03-24 20:35:14.705765 bolna-0.7.5/bolna/output_handlers/telephony_providers/
--rw-r--r--   0 xan        (501) staff       (20)     1360 2024-03-22 13:50:32.000000 bolna-0.7.5/bolna/output_handlers/telephony_providers/exotel.py
--rw-r--r--   0 xan        (501) staff       (20)     2291 2024-03-22 13:50:32.000000 bolna-0.7.5/bolna/output_handlers/telephony_providers/twilio.py
--rw-r--r--   0 xan        (501) staff       (20)     2649 2024-02-04 09:51:18.000000 bolna-0.7.5/bolna/prompts.py
--rw-r--r--   0 xan        (501) staff       (20)     1582 2024-03-22 13:50:32.000000 bolna-0.7.5/bolna/providers.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-03-24 20:35:14.707771 bolna-0.7.5/bolna/synthesizer/
--rw-r--r--   0 xan        (501) staff       (20)      306 2024-03-22 13:50:32.000000 bolna-0.7.5/bolna/synthesizer/__init__.py
--rw-r--r--   0 xan        (501) staff       (20)     1076 2024-03-22 13:50:32.000000 bolna-0.7.5/bolna/synthesizer/base_synthesizer.py
--rw-r--r--   0 xan        (501) staff       (20)     2758 2024-03-22 13:50:32.000000 bolna-0.7.5/bolna/synthesizer/deepgram_synthesizer.py
--rw-r--r--   0 xan        (501) staff       (20)     9696 2024-03-24 20:33:20.000000 bolna-0.7.5/bolna/synthesizer/elevenlabs_synthesizer.py
--rw-r--r--   0 xan        (501) staff       (20)     3483 2024-02-04 09:51:18.000000 bolna-0.7.5/bolna/synthesizer/fourie_synthesizer.py
--rw-r--r--   0 xan        (501) staff       (20)     4290 2024-02-24 08:10:37.000000 bolna-0.7.5/bolna/synthesizer/openai_synthesizer.py
--rw-r--r--   0 xan        (501) staff       (20)     3598 2024-03-23 20:32:29.000000 bolna-0.7.5/bolna/synthesizer/polly_synthesizer.py
--rw-r--r--   0 xan        (501) staff       (20)     7113 2024-02-24 08:10:37.000000 bolna-0.7.5/bolna/synthesizer/xtts_synthesizer.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-03-24 20:35:14.708684 bolna-0.7.5/bolna/transcriber/
--rw-r--r--   0 xan        (501) staff       (20)      100 2024-01-07 16:40:54.000000 bolna-0.7.5/bolna/transcriber/__init__.py
--rw-r--r--   0 xan        (501) staff       (20)     2243 2024-03-22 13:50:32.000000 bolna-0.7.5/bolna/transcriber/base_transcriber.py
--rw-r--r--   0 xan        (501) staff       (20)    20893 2024-03-24 20:33:20.000000 bolna-0.7.5/bolna/transcriber/deepgram_transcriber.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-03-24 20:35:14.709136 bolna-0.7.5/bolna.egg-info/
--rw-r--r--   0 xan        (501) staff       (20)    48259 2024-03-24 20:35:14.000000 bolna-0.7.5/bolna.egg-info/PKG-INFO
--rw-r--r--   0 xan        (501) staff       (20)     1918 2024-03-24 20:35:14.000000 bolna-0.7.5/bolna.egg-info/SOURCES.txt
--rw-r--r--   0 xan        (501) staff       (20)        1 2024-03-24 20:35:14.000000 bolna-0.7.5/bolna.egg-info/dependency_links.txt
--rw-r--r--   0 xan        (501) staff       (20)      357 2024-03-24 20:35:14.000000 bolna-0.7.5/bolna.egg-info/requires.txt
--rw-r--r--   0 xan        (501) staff       (20)        6 2024-03-24 20:35:14.000000 bolna-0.7.5/bolna.egg-info/top_level.txt
--rw-r--r--   0 xan        (501) staff       (20)     1164 2024-03-24 20:33:42.000000 bolna-0.7.5/pyproject.toml
--rw-r--r--   0 xan        (501) staff       (20)      339 2024-03-23 20:32:29.000000 bolna-0.7.5/requirements.txt
--rw-r--r--   0 xan        (501) staff       (20)       38 2024-03-24 20:35:14.710307 bolna-0.7.5/setup.cfg
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.910877 bolna-0.7.7/
+-rw-r--r--   0 xan        (501) staff       (20)    34522 2024-03-11 19:09:56.000000 bolna-0.7.7/LICENSE
+-rw-r--r--   0 xan        (501) staff       (20)    48383 2024-05-07 18:45:57.910668 bolna-0.7.7/PKG-INFO
+-rw-r--r--   0 xan        (501) staff       (20)     7456 2024-04-24 13:49:22.000000 bolna-0.7.7/README.md
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.898979 bolna-0.7.7/bolna/
+-rw-r--r--   0 xan        (501) staff       (20)      330 2024-05-07 18:45:43.000000 bolna-0.7.7/bolna/__init__.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.900712 bolna-0.7.7/bolna/agent_manager/
+-rw-r--r--   0 xan        (501) staff       (20)      124 2024-01-07 06:26:49.000000 bolna-0.7.7/bolna/agent_manager/__init__.py
+-rw-r--r--   0 xan        (501) staff       (20)     3040 2024-05-07 18:42:57.000000 bolna-0.7.7/bolna/agent_manager/assistant_manager.py
+-rw-r--r--   0 xan        (501) staff       (20)      174 2024-01-07 16:40:54.000000 bolna-0.7.7/bolna/agent_manager/base_manager.py
+-rw-r--r--   0 xan        (501) staff       (20)    82616 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/agent_manager/task_manager.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.902626 bolna-0.7.7/bolna/agent_types/
+-rw-r--r--   0 xan        (501) staff       (20)      300 2024-03-22 13:50:32.000000 bolna-0.7.7/bolna/agent_types/__init__.py
+-rw-r--r--   0 xan        (501) staff       (20)      176 2024-01-07 16:40:54.000000 bolna-0.7.7/bolna/agent_types/base_agent.py
+-rw-r--r--   0 xan        (501) staff       (20)     1353 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/agent_types/contextual_conversational_agent.py
+-rw-r--r--   0 xan        (501) staff       (20)      590 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/agent_types/extraction_agent.py
+-rw-r--r--   0 xan        (501) staff       (20)     6673 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/agent_types/graph_based_conversational_agent.py
+-rw-r--r--   0 xan        (501) staff       (20)      843 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/agent_types/summarization_agent.py
+-rw-r--r--   0 xan        (501) staff       (20)     1460 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/agent_types/zapier_agent.py
+-rw-r--r--   0 xan        (501) staff       (20)     1807 2024-01-19 12:02:21.000000 bolna-0.7.7/bolna/assistant.py
+-rw-r--r--   0 xan        (501) staff       (20)      937 2024-03-22 13:50:32.000000 bolna-0.7.7/bolna/constants.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.903714 bolna-0.7.7/bolna/helpers/
+-rw-r--r--   0 xan        (501) staff       (20)        0 2023-12-23 18:13:48.000000 bolna-0.7.7/bolna/helpers/__init__.py
+-rw-r--r--   0 xan        (501) staff       (20)     9978 2024-03-22 13:50:32.000000 bolna-0.7.7/bolna/helpers/analytics_helpers.py
+-rw-r--r--   0 xan        (501) staff       (20)        0 2024-01-12 18:42:30.000000 bolna-0.7.7/bolna/helpers/cache_helpers.py
+-rw-r--r--   0 xan        (501) staff       (20)      548 2024-01-07 16:40:54.000000 bolna-0.7.7/bolna/helpers/logger_config.py
+-rw-r--r--   0 xan        (501) staff       (20)    18542 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/helpers/utils.py
+-rw-r--r--   0 xan        (501) staff       (20)     3929 2024-03-22 13:50:32.000000 bolna-0.7.7/bolna/helpers/vad.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.904348 bolna-0.7.7/bolna/input_handlers/
+-rw-r--r--   0 xan        (501) staff       (20)      159 2024-03-22 13:50:32.000000 bolna-0.7.7/bolna/input_handlers/__init__.py
+-rw-r--r--   0 xan        (501) staff       (20)     3748 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/input_handlers/default.py
+-rw-r--r--   0 xan        (501) staff       (20)     4547 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/input_handlers/telephony.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.904633 bolna-0.7.7/bolna/input_handlers/telephony_providers/
+-rw-r--r--   0 xan        (501) staff       (20)      664 2024-03-22 13:50:32.000000 bolna-0.7.7/bolna/input_handlers/telephony_providers/exotel.py
+-rw-r--r--   0 xan        (501) staff       (20)      662 2024-03-22 13:50:32.000000 bolna-0.7.7/bolna/input_handlers/telephony_providers/twilio.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.905686 bolna-0.7.7/bolna/llms/
+-rw-r--r--   0 xan        (501) staff       (20)       63 2023-12-23 22:38:43.000000 bolna-0.7.7/bolna/llms/__init__.py
+-rw-r--r--   0 xan        (501) staff       (20)     3984 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/llms/litellm.py
+-rw-r--r--   0 xan        (501) staff       (20)      380 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/llms/llm.py
+-rw-r--r--   0 xan        (501) staff       (20)     4346 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/llms/openai_llm.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.896586 bolna-0.7.7/bolna/memory/
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.906361 bolna-0.7.7/bolna/memory/cache/
+-rw-r--r--   0 xan        (501) staff       (20)       54 2024-01-12 18:42:30.000000 bolna-0.7.7/bolna/memory/cache/__init__.py
+-rw-r--r--   0 xan        (501) staff       (20)      161 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/memory/cache/base_cache.py
+-rw-r--r--   0 xan        (501) staff       (20)     1014 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/memory/cache/inmemory_scalar_cache.py
+-rw-r--r--   0 xan        (501) staff       (20)     1254 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/memory/cache/vector_cache.py
+-rw-r--r--   0 xan        (501) staff       (20)     4673 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/models.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.906774 bolna-0.7.7/bolna/output_handlers/
+-rw-r--r--   0 xan        (501) staff       (20)      162 2024-03-22 13:50:32.000000 bolna-0.7.7/bolna/output_handlers/__init__.py
+-rw-r--r--   0 xan        (501) staff       (20)     1492 2024-03-22 13:50:32.000000 bolna-0.7.7/bolna/output_handlers/default.py
+-rw-r--r--   0 xan        (501) staff       (20)     2028 2024-03-22 13:50:32.000000 bolna-0.7.7/bolna/output_handlers/telephony.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.907060 bolna-0.7.7/bolna/output_handlers/telephony_providers/
+-rw-r--r--   0 xan        (501) staff       (20)     1360 2024-03-22 13:50:32.000000 bolna-0.7.7/bolna/output_handlers/telephony_providers/exotel.py
+-rw-r--r--   0 xan        (501) staff       (20)     2291 2024-03-30 13:29:33.000000 bolna-0.7.7/bolna/output_handlers/telephony_providers/twilio.py
+-rw-r--r--   0 xan        (501) staff       (20)     2781 2024-04-22 11:30:07.000000 bolna-0.7.7/bolna/prompts.py
+-rw-r--r--   0 xan        (501) staff       (20)     1673 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/providers.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.908963 bolna-0.7.7/bolna/synthesizer/
+-rw-r--r--   0 xan        (501) staff       (20)      306 2024-04-01 19:37:04.000000 bolna-0.7.7/bolna/synthesizer/__init__.py
+-rw-r--r--   0 xan        (501) staff       (20)     1096 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/synthesizer/base_synthesizer.py
+-rw-r--r--   0 xan        (501) staff       (20)     2786 2024-04-26 13:33:46.000000 bolna-0.7.7/bolna/synthesizer/deepgram_synthesizer.py
+-rw-r--r--   0 xan        (501) staff       (20)    10697 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/synthesizer/elevenlabs_synthesizer.py
+-rw-r--r--   0 xan        (501) staff       (20)     3483 2024-02-04 09:51:18.000000 bolna-0.7.7/bolna/synthesizer/fourie_synthesizer.py
+-rw-r--r--   0 xan        (501) staff       (20)     4287 2024-04-22 11:30:07.000000 bolna-0.7.7/bolna/synthesizer/openai_synthesizer.py
+-rw-r--r--   0 xan        (501) staff       (20)     4566 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/synthesizer/polly_synthesizer.py
+-rw-r--r--   0 xan        (501) staff       (20)     7100 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/synthesizer/xtts_synthesizer.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.909769 bolna-0.7.7/bolna/transcriber/
+-rw-r--r--   0 xan        (501) staff       (20)      100 2024-05-07 18:42:57.000000 bolna-0.7.7/bolna/transcriber/__init__.py
+-rw-r--r--   0 xan        (501) staff       (20)    17668 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/transcriber/azure_transcriber.py
+-rw-r--r--   0 xan        (501) staff       (20)     2242 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/transcriber/base_transcriber.py
+-rw-r--r--   0 xan        (501) staff       (20)    16058 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/transcriber/deepgram_transcriber.py
+-rw-r--r--   0 xan        (501) staff       (20)    18909 2024-04-26 13:37:59.000000 bolna-0.7.7/bolna/transcriber/hume_transcriber.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.910198 bolna-0.7.7/bolna.egg-info/
+-rw-r--r--   0 xan        (501) staff       (20)    48383 2024-05-07 18:45:57.000000 bolna-0.7.7/bolna.egg-info/PKG-INFO
+-rw-r--r--   0 xan        (501) staff       (20)     2031 2024-05-07 18:45:57.000000 bolna-0.7.7/bolna.egg-info/SOURCES.txt
+-rw-r--r--   0 xan        (501) staff       (20)        1 2024-05-07 18:45:57.000000 bolna-0.7.7/bolna.egg-info/dependency_links.txt
+-rw-r--r--   0 xan        (501) staff       (20)      387 2024-05-07 18:45:57.000000 bolna-0.7.7/bolna.egg-info/requires.txt
+-rw-r--r--   0 xan        (501) staff       (20)        6 2024-05-07 18:45:57.000000 bolna-0.7.7/bolna.egg-info/top_level.txt
+-rw-r--r--   0 xan        (501) staff       (20)     1164 2024-05-07 18:45:43.000000 bolna-0.7.7/pyproject.toml
+-rw-r--r--   0 xan        (501) staff       (20)      370 2024-05-07 18:42:54.000000 bolna-0.7.7/requirements.txt
+-rw-r--r--   0 xan        (501) staff       (20)       38 2024-05-07 18:45:57.910916 bolna-0.7.7/setup.cfg
```

### Comparing `bolna-0.7.5/LICENSE` & `bolna-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bolna-0.7.5/PKG-INFO` & `bolna-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bolna
-Version: 0.7.5
+Version: 0.7.7
 Author-email: Prateek Sachan <ps@prateeksachan.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -666,34 +666,35 @@
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.9.0
-Requires-Dist: aiocsv==1.3.1
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: aiohttp==3.9.1
 Requires-Dist: fastapi==0.108.0
+Requires-Dist: fastembed==0.2.7
 Requires-Dist: litellm==1.15.7
 Requires-Dist: numpy==1.26.1
-Requires-Dist: openai==1.3.5
-Requires-Dist: pydantic==2.5
+Requires-Dist: openai==1.10.0
+Requires-Dist: pydantic==2.5.3
 Requires-Dist: pydub==0.25.1
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: redis==5.0.1
 Requires-Dist: requests==2.31.0
-Requires-Dist: tiktoken==0.5.2
+Requires-Dist: tiktoken==0.6.0
 Requires-Dist: twilio==8.9.0
 Requires-Dist: uvicorn==0.22.0
-Requires-Dist: uvloop==0.19.0
 Requires-Dist: websockets==10.4
-Requires-Dist: onnxruntime==1.16.3
+Requires-Dist: onnxruntime>=1.16.3
 Requires-Dist: scipy==1.11.4
+Requires-Dist: uvloop==0.19.0
+Requires-Dist: semantic-router==0.0.37
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 
 <h1 align="center">
 </h1>
 <p align="center">
   <p align="center"><b>End-to-end open-source voice agents platform</b>: Quickly build LLM based voice driven conversational applications</p>
@@ -758,44 +759,45 @@
 1. Refer to the official [`Agent` API](https://docs.bolna.dev/api-reference/agent/create) to create an agent
 2. Initiate a call via API similar to [`Call` API](https://docs.bolna.dev/api-reference/calls/make) to receive a call
 
 
 ## Using your own providers
 You can populate the `.env` file to use your own keys for providers.
 
-<details>
+<details open>
 
 <summary>ASR Providers</summary><br>
 These are the current supported ASRs Providers:
 
 | Provider     | Environment variable to be added in `.env` file |
 |--------------|-------------------------------------------------|
 | Deepgram     | `DEEPGRAM_AUTH_TOKEN`                           |
 
 </details>
 &nbsp;<br>
 
-<details>
+<details open>
 <summary>LLM Providers</summary><br>
 Bolna uses LiteLLM package to support multiple LLM integrations.
 
 These are the current supported LLM Provider Family:
 https://github.com/bolna-ai/bolna/blob/c8a0d1428793d4df29133119e354bc2f85a7ca76/bolna/providers.py#L19-L28
 
 For LiteLLM based LLMs, add either of the following to the `.env` file depending on your use-case:<br><br>
-`LITELLM_MODEL_API_BASE`: API Key of the LLM<br>
-`LITELLM_MODEL_API_BASE`: URL of the hosted LLM
+`LITELLM_MODEL_API_KEY`: API Key of the LLM<br>
+`LITELLM_MODEL_API_BASE`: URL of the hosted LLM<br>
+`LITELLM_MODEL_API_VERSION`: API VERSION for LLMs like Azure
 
 For LLMs hosted via VLLM, add the following to the `.env` file:<br>
 `VLLM_SERVER_BASE_URL`: URL of the hosted LLM using VLLM
 
 </details>
 &nbsp;<br>
 
-<details>
+<details open>
 
 <summary>TTS Providers</summary><br>
 These are the current supported TTS Providers:
 https://github.com/bolna-ai/bolna/blob/c8a0d1428793d4df29133119e354bc2f85a7ca76/bolna/providers.py#L7-L14
 
 | Provider   | Environment variable to be added in `.env` file  |
 |------------|--------------------------------------------------|
```

### Comparing `bolna-0.7.5/README.md` & `bolna-0.7.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -63,44 +63,45 @@
 1. Refer to the official [`Agent` API](https://docs.bolna.dev/api-reference/agent/create) to create an agent
 2. Initiate a call via API similar to [`Call` API](https://docs.bolna.dev/api-reference/calls/make) to receive a call
 
 
 ## Using your own providers
 You can populate the `.env` file to use your own keys for providers.
 
-<details>
+<details open>
 
 <summary>ASR Providers</summary><br>
 These are the current supported ASRs Providers:
 
 | Provider     | Environment variable to be added in `.env` file |
 |--------------|-------------------------------------------------|
 | Deepgram     | `DEEPGRAM_AUTH_TOKEN`                           |
 
 </details>
 &nbsp;<br>
 
-<details>
+<details open>
 <summary>LLM Providers</summary><br>
 Bolna uses LiteLLM package to support multiple LLM integrations.
 
 These are the current supported LLM Provider Family:
 https://github.com/bolna-ai/bolna/blob/c8a0d1428793d4df29133119e354bc2f85a7ca76/bolna/providers.py#L19-L28
 
 For LiteLLM based LLMs, add either of the following to the `.env` file depending on your use-case:<br><br>
-`LITELLM_MODEL_API_BASE`: API Key of the LLM<br>
-`LITELLM_MODEL_API_BASE`: URL of the hosted LLM
+`LITELLM_MODEL_API_KEY`: API Key of the LLM<br>
+`LITELLM_MODEL_API_BASE`: URL of the hosted LLM<br>
+`LITELLM_MODEL_API_VERSION`: API VERSION for LLMs like Azure
 
 For LLMs hosted via VLLM, add the following to the `.env` file:<br>
 `VLLM_SERVER_BASE_URL`: URL of the hosted LLM using VLLM
 
 </details>
 &nbsp;<br>
 
-<details>
+<details open>
 
 <summary>TTS Providers</summary><br>
 These are the current supported TTS Providers:
 https://github.com/bolna-ai/bolna/blob/c8a0d1428793d4df29133119e354bc2f85a7ca76/bolna/providers.py#L7-L14
 
 | Provider   | Environment variable to be added in `.env` file  |
 |------------|--------------------------------------------------|
```

#### html2text {}

```diff
@@ -38,17 +38,18 @@
 LLM Providers
 Bolna uses LiteLLM package to support multiple LLM integrations. These are the
 current supported LLM Provider Family: https://github.com/bolna-ai/bolna/blob/
 c8a0d1428793d4df29133119e354bc2f85a7ca76/bolna/providers.py#L19-L28 For LiteLLM
 based LLMs, add either of the following to the `.env` file depending on your
 use-case:
 
-`LITELLM_MODEL_API_BASE`: API Key of the LLM
-`LITELLM_MODEL_API_BASE`: URL of the hosted LLM For LLMs hosted via VLLM, add
-the following to the `.env` file:
+`LITELLM_MODEL_API_KEY`: API Key of the LLM
+`LITELLM_MODEL_API_BASE`: URL of the hosted LLM
+`LITELLM_MODEL_API_VERSION`: API VERSION for LLMs like Azure For LLMs hosted
+via VLLM, add the following to the `.env` file:
 `VLLM_SERVER_BASE_URL`: URL of the hosted LLM using VLLM  
 TTS Providers
 These are the current supported TTS Providers: https://github.com/bolna-ai/
 bolna/blob/c8a0d1428793d4df29133119e354bc2f85a7ca76/bolna/providers.py#L7-L14 |
 Provider | Environment variable to be added in `.env` file | |------------|----
 ----------------------------------------------| | AWS Polly | Accessed from
 system wide credentials via ~/.aws | | Elevenlabs | `ELEVENLABS_API_KEY` | |
```

### Comparing `bolna-0.7.5/bolna/agent_manager/assistant_manager.py` & `bolna-0.7.7/bolna/agent_manager/assistant_manager.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from .task_manager import TaskManager
 from bolna.helpers.logger_config import configure_logger
 
 logger = configure_logger(__name__)
 
 enc = tiktoken.get_encoding("cl100k_base")
 
-
 class AssistantManager(BaseManager):
     def __init__(self, agent_config, ws=None, assistant_id=None, context_data=None, conversation_history=None,
                  connected_through_dashboard=None, cache=None, input_queue=None, output_queue=None, **kwargs):
         super().__init__()
         self.tools = {}
         self.websocket = ws
         self.agent_config = agent_config
@@ -24,14 +23,15 @@
         self.connected_through_dashboard = connected_through_dashboard
         self.cache = cache
         self.input_queue = input_queue
         self.output_queue = output_queue
         self.kwargs = kwargs
         self.conversation_history = conversation_history
 
+
     async def run(self, local=False, run_id=None):
         """
         Run will start all tasks in sequential format
         """
         if run_id:
             self.run_id = run_id
```

### Comparing `bolna-0.7.5/bolna/agent_manager/task_manager.py` & `bolna-0.7.7/bolna/agent_manager/task_manager.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 import asyncio
 from collections import defaultdict
+import os
+import random
 import traceback
 import time
 import json
 import uuid
 import copy
 from datetime import datetime
+
+from bolna.memory.cache.inmemory_scalar_cache import InmemoryScalarCache
+from bolna.memory.cache.vector_cache import VectorCache
 from .base_manager import BaseManager
 from bolna.agent_types import *
 from bolna.providers import *
-from bolna.helpers.utils import create_ws_data_packet, is_valid_md5, get_raw_audio_bytes_from_base64, \
-    get_required_input_types, format_messages, get_prompt_responses, update_prompt_with_context, get_md5_hash, clean_json_string, wav_bytes_to_pcm, write_request_logs, yield_chunks_from_memory
+from bolna.helpers.utils import calculate_audio_duration, create_ws_data_packet, get_file_names_in_directory, get_raw_audio_bytes, is_valid_md5, \
+    get_required_input_types, format_messages, get_prompt_responses, list_number_of_wav_files_in_directory, resample, save_audio_file_to_s3, update_prompt_with_context, get_md5_hash, clean_json_string, wav_bytes_to_pcm, write_request_logs, yield_chunks_from_memory
 from bolna.helpers.logger_config import configure_logger
-
+import uvloop
+asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
+from semantic_router import Route
+from semantic_router.layer import RouteLayer
+from semantic_router.encoders import FastEmbedEncoder
 
 asyncio.get_event_loop().set_debug(True)
 logger = configure_logger(__name__)
 
 
 class TaskManager(BaseManager):
     def __init__(self, assistant_name, task_id, task, ws, input_parameters=None, context_data=None,
@@ -56,24 +65,37 @@
             "agent_task"] == "conversation":
             self.textual_chat_agent = False
 
         # Assistant persistance stuff
         self.assistant_id = assistant_id
         self.run_id = run_id
         self.mark_set = set()
-
+        
         self.conversation_ended = False
 
         # Prompts
         self.prompts, self.system_prompt = {}, {}
         self.input_parameters = input_parameters
         
+        # Recording
+        self.should_record = False
+        self.conversation_recording= {
+            "input": {
+                'data': b'',
+                'started': time.time()
+            },
+            "output": [],
+            "metadata": {
+                "started": 0
+            }
+        }
         #IO HANDLERS
         if task_id == 0:
-            self.__setup_input_handlers(connected_through_dashboard, input_queue)
+            self.should_record = self.task_config["tools_config"]["output"]["provider"] == 'default' and self.enforce_streaming #In this case, this is a websocket connection and we should record 
+            self.__setup_input_handlers(connected_through_dashboard, input_queue, self.should_record)
         self.__setup_output_handlers(connected_through_dashboard, output_queue)
 
         # Agent stuff
         # Need to maintain current conversation history and overall persona/history kinda thing. 
         # Soon we will maintain a seperate history for this 
         self.history = [] if conversation_history is None else conversation_history 
         self.interim_history = copy.deepcopy(self.history.copy())
@@ -89,20 +111,20 @@
         self.current_request_id = None
         self.previous_request_id = None
         self.llm_rejected_request_ids = set()
         self.llm_processed_request_ids = set()
         self.was_long_pause = False
         self.buffers = []
         self.should_respond = False
-        self.start_response = False
         self.last_response_time = time.time()
         self.is_an_ivr_call = self._is_conversation_task() and self._is_preprocessed_flow() and not self.connected_through_dashboard
         self.consider_next_transcript_after = time.time()
-        self.duration_to_prevent_accidental_interruption = 3 if self.is_an_ivr_call else 1.5
+        self.duration_to_prevent_accidental_interruption = 3 if self.is_an_ivr_call else 0
         self.callee_speaking = False
+        self.callee_speaking_start_time = -1
 
         # Call conversations
         self.call_sid = None
         self.stream_sid = None
 
         # metering
         self.transcriber_duration = 0
@@ -117,16 +139,15 @@
         logger.info(f"TASK CONFIG {self.task_config['tools_config'] }")
         self.stream = (self.task_config["tools_config"]['synthesizer'] is not None and self.task_config["tools_config"]["synthesizer"]["stream"]) and (self.enforce_streaming or not self.connected_through_dashboard)
         #self.stream = not connected_through_dashboard #Currently we are allowing only realtime conversation based usecases. Hence it'll always be true unless connected through dashboard
         self.is_local = False
         llm_config = None
         if self.task_config["tools_config"]["llm_agent"] is not None:
             llm_config = {
-                "streaming_model": self.task_config["tools_config"]["llm_agent"]["streaming_model"],
-                "classification_model": self.task_config["tools_config"]["llm_agent"]["classification_model"],
+                "model": self.task_config["tools_config"]["llm_agent"]["model"],
                 "max_tokens": self.task_config["tools_config"]["llm_agent"]["max_tokens"]
             }
         
         # Output stuff
         self.output_task = None
         self.buffered_output_queue = asyncio.Queue()
 
@@ -143,51 +164,152 @@
         # setting synthesizer
         self.__setup_synthesizer(llm_config)
         # setting llm
         llm = self.__setup_llm(llm_config)
         #Setup tasks
         self.__setup_tasks(llm)
 
+
         #setup request logs
         self.request_logs = []
 
+        # for long pauses and rushing
+        
+        if task_id == 0:
+            self.output_chunk_size = 16384 if self.sampling_rate == 24000 else 4096 #0.5 second chunk size for calls 
+            # For nitro
+            self.nitro = True 
+            self.minimum_wait_duration = self.task_config["tools_config"]["transcriber"]["endpointing"]
+            logger.info(f"minimum wait duration {self.minimum_wait_duration}")
+            self.last_spoken_timestamp = time.time() * 1000
+            self.incremental_delay = task.get("incremental_delay", 100)
+            self.required_delay_before_speaking = max(self.minimum_wait_duration - self.incremental_delay, 0)  #Everytime we get a message we increase it by 100 miliseconds 
+            self.time_since_first_interim_result  = -1
+
+        #Cut conversation
+        self.hang_conversation_after = task.get("hangup_after_silence", 10)
+        self.last_transmitted_timesatamp = 0
+        self.let_remaining_audio_pass_through = False #Will be used to let remaining audio pass through in case of utterenceEnd event and there's still audio left to be sent
+        self.use_llm_to_determine_hangup = task.get("hangup_after_LLMCall", False)
+        self.check_for_completion_prompt = task.get("call_cancellation_prompt", None)
+        if self.check_for_completion_prompt is not None:
+            completion_json_format = {"answer": "A simple Yes or No based on if you should cut the phone or not"}
+            self.check_for_completion_prompt = f"{self.check_for_completion_prompt}\nYour response should be in the following json format\n{completion_json_format}"
+        self.check_for_completion_llm = os.getenv("CHECK_FOR_COMPLETION_LLM")
+        self.time_since_last_spoken_human_word = 0 
+
+        #Handling accidental interruption
+        self.number_of_words_for_interruption = task.get("number_of_words_for_interruption", 3)
+        self.started_transmitting_audio = False
+        #self.interruption_backoff_period = 1000 #task.get("interruption_backoff_period", 300) #this is the amount of time output loop will sleep before sending next audio
+        self.use_llm_for_hanging_up = task.get("hangup_after_LLMCall", False)
+        self.allow_extra_sleep = False #It'll help us to back off as soon as we hear interruption for a while
+
+        # Conversation
+        if task_id == 0:
+            self.routes = task['tools_config']['llm_agent'].get("routes", None)
+            self.route_layer = None
+            if self.routes:
+                self.__setup_routes(self.routes)
+        
+        #Backchanneling
+        self.should_backchannel = task.get("backchanneling", True)
+        self.backchanneling_task = None
+        self.backchanneling_start_delay = task.get("backchanneling_start_delay", 5)
+        self.backchanneling_message_gap = task.get("backchanneling_message_gap", 2) #Amount of duration co routine will sleep
+        if self.should_backchannel:
+            logger.info(f"Should backchannel")
+            self.backchanneling_audios = f'{kwargs.get("backchanneling_audio_location", os.getenv("BACKCHANNELING_PRESETS_DIR"))}/{self.synthesizer_voice.lower()}'
+            #self.num_files = list_number_of_wav_files_in_directory(self.backchanneling_audios)
+            try:
+                self.filenames = get_file_names_in_directory(self.backchanneling_audios)
+                logger.info(f"Backchanneling audio location {self.backchanneling_audios}")
+            except Exception as e:
+                logger.info(f"Something went wrong an putting should backchannel to false")
+                self.should_backchannel = False
+        else:
+            logger.info(f"Not setting up backchanneling")
+            self.backchanneling_audio_map = []
+            
+            
+    def __setup_routes(self, routes):
+        embedding_model = routes.get("embedding_model", os.getenv("ROUTE_EMBEDDING_MODEL"))
+        self.route_encoder = FastEmbedEncoder(name=embedding_model)
+
+        routes_list = []
+        self.vector_caches = {}
+        self.route_responses_dict = {}
+        for route in routes['routes']:
+            logger.info(f"Setting up route {route}")
+            utterances = route['utterances']
+            r = Route(
+                name = route['route_name'],
+                utterances= utterances,
+                score_threshold = route['score_threshold']
+            )
+            utterance_response_dict = {}
+            if type(route['response']) is list and len(route['response']) == len(route['utterances']):
+                for i, utterance in enumerate(utterances):
+                    utterance_response_dict[utterance] =  route['response'][i]
+                self.route_responses_dict[route['route_name']] = utterance_response_dict
+            elif type(route['response']) is str:
+                self.route_responses_dict[route['route_name']] = route['response']
+            else:
+                raise Exception("Invalid number of responses for the responses array")
+
+                
+            routes_list.append(r)
+            
+            if type(route['response']) is list:
+                logger.info(f"Setting up vector cache for {route} and embedding model {embedding_model}")
+                vector_cache = VectorCache(embedding_model = embedding_model)
+                vector_cache.set(utterances)
+                self.vector_caches[route['route_name']] = vector_cache
+            
+        self.route_layer = RouteLayer(encoder=self.route_encoder, routes=routes_list)
+        logger.info("Routes are set")
+
     def __setup_output_handlers(self, connected_through_dashboard, output_queue):
         output_kwargs = {"websocket": self.websocket}  
         
         if self.task_config["tools_config"]["output"] is None:
             logger.info("Not setting up any output handler as it is none")
         elif self.task_config["tools_config"]["output"]["provider"] in SUPPORTED_OUTPUT_HANDLERS.keys():
             if connected_through_dashboard:
                 logger.info("Connected through dashboard and hence using default output handler")
                 output_handler_class = SUPPORTED_OUTPUT_HANDLERS.get("default")
                 output_kwargs['queue'] = output_queue
+                self.sampling_rate = 24000
             else:
                 output_handler_class = SUPPORTED_OUTPUT_HANDLERS.get(self.task_config["tools_config"]["output"]["provider"])
             
                 if self.task_config["tools_config"]["output"]["provider"] in SUPPORTED_OUTPUT_TELEPHONY_HANDLERS.keys():
                     output_kwargs['mark_set'] = self.mark_set
                     logger.info(f"Making sure that the sampling rate for output handler is 8000")
                     self.task_config['tools_config']['synthesizer']['provider_config']['sampling_rate'] = 8000
                     self.task_config['tools_config']['synthesizer']['audio_format'] = 'pcm'
                 else:
                     self.task_config['tools_config']['synthesizer']['provider_config']['sampling_rate'] = 24000
                     output_kwargs['queue'] = output_queue
+                self.sampling_rate = self.task_config['tools_config']['synthesizer']['provider_config']['sampling_rate']
 
             self.tools["output"] = output_handler_class(**output_kwargs)
         else:
             raise "Other input handlers not supported yet"
 
-    def __setup_input_handlers(self, connected_through_dashboard, input_queue):
+    def __setup_input_handlers(self, connected_through_dashboard, input_queue, should_record):
         if self.task_config["tools_config"]["input"]["provider"] in SUPPORTED_INPUT_HANDLERS.keys():
             logger.info(f"Connected through dashboard {connected_through_dashboard}")
             input_kwargs = {"queues": self.queues,
                             "websocket": self.websocket,
                             "input_types": get_required_input_types(self.task_config),
                             "mark_set": self.mark_set,
                             "connected_through_dashboard": self.connected_through_dashboard}
+            if should_record:
+                input_kwargs['conversation_recording'] = self.conversation_recording
 
             if connected_through_dashboard:
                 logger.info("Connected through dashboard and hence using default input handler")
                 # If connected through dashboard get basic dashboard class
                 input_handler_class = SUPPORTED_INPUT_HANDLERS.get("default")
                 input_kwargs['queue'] = input_queue
             else:
@@ -211,38 +333,42 @@
                     self.task_config["tools_config"]["transcriber"]["stream"] = True if self.enforce_streaming else False
                     logger.info(f'self.task_config["tools_config"]["transcriber"]["stream"] {self.task_config["tools_config"]["transcriber"]["stream"]} self.enforce_streaming {self.enforce_streaming}')
                 transcriber_class = SUPPORTED_TRANSCRIBER_MODELS.get(
                     self.task_config["tools_config"]["transcriber"]["model"])
                 self.tools["transcriber"] = transcriber_class(provider, **self.task_config["tools_config"]["transcriber"], **self.kwargs)
 
     def __setup_synthesizer(self, llm_config):
+        self.synthesizer_cache = InmemoryScalarCache()
+        
         logger.info(f"Synthesizer config: {self.task_config['tools_config']['synthesizer']}")
         if self._is_conversation_task():
             self.kwargs["use_turbo"] = self.task_config["tools_config"]["transcriber"]["language"] == "en"
         if self.task_config["tools_config"]["synthesizer"] is not None:
             self.synthesizer_provider = self.task_config["tools_config"]["synthesizer"].pop("provider")
             synthesizer_class = SUPPORTED_SYNTHESIZER_MODELS.get(self.synthesizer_provider)
             provider_config = self.task_config["tools_config"]["synthesizer"].pop("provider_config")
+            self.synthesizer_voice = provider_config["voice"]
             if self.connected_through_dashboard:
                 self.task_config["tools_config"]["synthesizer"]["audio_format"] = "mp3" # Hard code mp3 if we're connected through dashboard
                 self.task_config["tools_config"]["synthesizer"]["stream"] = True if self.enforce_streaming else False #Hardcode stream to be False as we don't want to get blocked by a __listen_synthesizer co-routine
         
-            self.tools["synthesizer"] = synthesizer_class(**self.task_config["tools_config"]["synthesizer"], **provider_config, **self.kwargs)
+            self.tools["synthesizer"] = synthesizer_class(**self.task_config["tools_config"]["synthesizer"], **provider_config, **self.kwargs, cache = self.synthesizer_cache)
             if self.task_config["tools_config"]["llm_agent"] is not None:
                 llm_config["buffer_size"] = self.task_config["tools_config"]["synthesizer"].get('buffer_size')
 
     def __setup_llm(self, llm_config):
         if self.task_config["tools_config"]["llm_agent"] is not None:
-            if self.task_config["tools_config"]["llm_agent"]["family"] in SUPPORTED_LLM_MODELS.keys():
-                llm_class = SUPPORTED_LLM_MODELS.get(self.task_config["tools_config"]["llm_agent"]["family"])
+            logger.info(f'### PROVIDER {self.task_config["tools_config"]["llm_agent"]["provider"] }')
+            if self.task_config["tools_config"]["llm_agent"]["provider"] in SUPPORTED_LLM_PROVIDERS.keys():
+                llm_class = SUPPORTED_LLM_PROVIDERS.get(self.task_config["tools_config"]["llm_agent"]["provider"])
                 logger.info(f"LLM CONFIG {llm_config}")
                 llm = llm_class(**llm_config, **self.kwargs)
                 return llm
             else:
-                raise Exception(f'LLM {self.task_config["tools_config"]["llm_agent"]["family"]} not supported')
+                raise Exception(f'LLM {self.task_config["tools_config"]["llm_agent"]["provider"]} not supported')
 
     def __setup_tasks(self, llm):
         if self.task_config["task_type"] == "conversation":
             if self.task_config["tools_config"]["llm_agent"]["agent_flow_type"] == "streaming":
                 self.tools["llm_agent"] = StreamingContextualAgent(llm)
             elif self.task_config["tools_config"]["llm_agent"]["agent_flow_type"] in ("preprocessed", "formulaic"):
                 preprocessed = self.task_config["tools_config"]["llm_agent"]["agent_flow_type"] == "preprocessed"
@@ -275,15 +401,17 @@
         if "prompt" in self.task_config["tools_config"]["llm_agent"]:
             today = datetime.now().strftime("%A, %B %d, %Y")
             self.prompts = {
                 "system_prompt": f'{self.task_config["tools_config"]["llm_agent"]["prompt"]} \n### Date\n Today\'s Date is {today}'
             }
             logger.info(f"Prompt given in llm_agent and hence storing the prompt")
         else:
-            prompt_responses = await get_prompt_responses(assistant_id=self.assistant_id, local=self.is_local)
+            prompt_responses = kwargs.get('prompt_responses', None)
+            if not prompt_responses:
+                prompt_responses = await get_prompt_responses(assistant_id=self.assistant_id, local=self.is_local)
             self.prompts = prompt_responses["task_{}".format(task_id + 1)]
             if self.task_config["tools_config"]["llm_agent"]['agent_flow_type'] == "preprocessed":
                 self.tools["llm_agent"].load_prompts_and_create_graph(self.prompts)
 
         if "system_prompt" in self.prompts:
             # This isn't a graph based agent
             enriched_prompt = self.prompts["system_prompt"]
@@ -321,32 +449,45 @@
         return text_chunk
     
     async def process_interruption(self):
         logger.info(f"Handling interruption sequenxce ids {self.sequence_ids}")
         await self.__cleanup_downstream_tasks()    
 
     async def __cleanup_downstream_tasks(self):
+        logger.info(f"Cleaning up downstream task")
         start_time = time.time()
         await self.tools["output"].handle_interruption()
-        logger.info(f"Cleaning up downstream tasks sequenxce ids {self.sequence_ids}. Time taken to send a clear message {time.time() - start_time}")
         self.sequence_ids = set()
+        
+        #Stop the output loop first so that we do not transmit anything else
+        if self.output_task is not None:
+            logger.info(f"Cancelling output task")
+            self.output_task.cancel()
+
         if self.llm_task is not None:
             logger.info(f"Cancelling LLM Task")
             self.llm_task.cancel()
             self.llm_task = None
 
-        #self.synthesizer_task.cancel()
-        #self.synthesizer_task = asyncio.create_task(self.__listen_synthesizer())
+        # self.synthesizer_task.cancel()
+        # self.synthesizer_task = asyncio.create_task(self.__listen_synthesizer())
+        for task in self.synthesizer_tasks:
+            task.cancel()
+        
+        self.synthesizer_tasks = []
+
         logger.info(f"Synth Task cancelled seconds")
         if not self.buffered_output_queue.empty():
             logger.info(f"Output queue was not empty and hence emptying it")
             self.buffered_output_queue = asyncio.Queue()
-        # if "synthesizer" in self.tools:
-        #     self.tools["synthesizer"].clear_internal_queue()
-    
+        
+        #restart output task
+        self.output_task = asyncio.create_task(self.__process_output_loop())
+        logger.info(f"Cleaning up downstream tasks sequenxce ids {self.sequence_ids}. Time taken to send a clear message {time.time() - start_time}")
+
     def __get_updated_meta_info(self, meta_info = None):
         #This is used in case there's silence from callee's side
         if meta_info is None:
             meta_info = self.tools["transcriber"].get_meta_info()
         meta_info_copy = meta_info.copy()
         self.curr_sequence_id +=1
         meta_info_copy["sequence_id"] = self.curr_sequence_id
@@ -388,19 +529,19 @@
             return
 
         if "call_sid" in message['meta_info']:
             self.call_sid = message['meta_info']["call_sid"]
         if "stream_sid" in message:
             self.stream_sid = message['meta_info']["stream_sid"]
 
-    async def _process_followup_task(self, message = None):
+    async def _process_followup_task(self, message=None):
         logger.info(f" TASK CONFIG  {self.task_config['task_type']}")
         if self.task_config["task_type"] == "webhook":
             logger.info(f"Input patrameters {self.input_parameters}")
-            logger.info(f"DOINFG THE POST REQUEST TO ZAPIER WEBHOOK {self.input_parameters['extraction_details']}")
+            logger.info(f"DOING THE POST REQUEST TO ZAPIER WEBHOOK {self.input_parameters['extraction_details']}")
             self.webhook_response = await self.tools["webhook_agent"].execute(self.input_parameters['extraction_details'])
             logger.info(f"Response from the server {self.webhook_response}")
         else:
             message = format_messages(self.input_parameters["messages"])  # Remove the initial system prompt
             self.history.append({
                 'role': 'user',
                 'content': message
@@ -429,29 +570,14 @@
         await self.tools["input"].stop_handler()
         logger.info("Stopped input handler")
         if "transcriber" in self.tools and not self.connected_through_dashboard:
             logger.info("Stopping transcriber")
             await self.tools["transcriber"].toggle_connection()
             await asyncio.sleep(5)  # Making sure whatever message was passed is over
 
-    def __update_transcripts(self):
-        #Essentially check if last two are assistants
-        logger.info(f"Appending assistant message to the backend")
-        if len(self.history) > 0 and self.history[-1]['role'] == "user":
-            logger.info(f"Last message was user, and hence appending to it")
-            self.history.append(self.interim_history[-1].copy())
-        elif len(self.history) > 1 and self.history[-1]['role'] == "assistant" and self.history[-2]['role'] == "assistant":
-            logger.info("Last two are assistants and hence changing the last one")
-            self.history[-1] = self.interim_history[-1].copy()
-        elif len(self.history) == 2 and self.history[1]['role'] == "assistant" and self.history[0]['role'] == "system":
-            logger.info(f"Assistant response is already appended to the history")
-            self.history = [self.history[0], self.interim_history[1].copy(), self.history[1]]
-        else:
-            self.history.append(self.interim_history[-1].copy())
-            logger.info(f"Current history {self.history}, current interim history {self.interim_history} but it falls in else part")
 
     def __update_preprocessed_tree_node(self):
         logger.info(f"It's a preprocessed flow and hence updating current node")
         self.tools['llm_agent'].update_current_node()
     
     def __convert_to_request_log(self, message, meta_info, model, component = "transcriber", direction = 'response'):
         log = dict()
@@ -470,68 +596,66 @@
         asyncio.create_task(write_request_logs(log, self.run_id))
 
     ##############################################################
     # LLM task
     ##############################################################
     async def _handle_llm_output(self, next_step, text_chunk, should_bypass_synth, meta_info):
 
-        logger.info("received text from LLM for output processing: {} which belongs to sequence id".format(text_chunk))
+        logger.info("received text from LLM for output processing: {} which belongs to sequence id {}".format(text_chunk, meta_info['sequence_id']))
         if "request_id" not in meta_info:
             meta_info["request_id"] = str(uuid.uuid4())
         first_buffer_latency = time.time() - meta_info["llm_start_time"]
         #self.latency_dict[meta_info["request_id"]]["llm"] = first_buffer_latency
         meta_info["llm_first_buffer_generation_latency"] = first_buffer_latency
         if next_step == "synthesizer" and not should_bypass_synth:
-            task = asyncio.gather(self._synthesize(create_ws_data_packet(text_chunk, meta_info)))
+            task = asyncio.create_task(self._synthesize(create_ws_data_packet(text_chunk, meta_info)))
             self.synthesizer_tasks.append(asyncio.ensure_future(task))
         elif self.tools["output"] is not None:
+            logger.info("Synthesizer not the next step and hence simply returning back")
+            #self.history = copy.deepcopy(self.interim_history)
             await self.tools["output"].handle(create_ws_data_packet(text_chunk, meta_info))
 
     async def _process_conversation_preprocessed_task(self, message, sequence, meta_info):
         if self.task_config["tools_config"]["llm_agent"]['agent_flow_type'] == "preprocessed":
-            llm_response = ""
-            start_time = time.time()
-            self.interim_history.append({'role': 'user', 'content': message['data']})
-            logger.info(f"Starting LLM Agent {self.interim_history}")
+            messages = copy.deepcopy(self.history)
+            messages.append({'role': 'user', 'content': message['data']})
+            logger.info(f"Starting LLM Agent {messages}")
             #Expose get current classification_response method from the agent class and use it for the response log
-            self.__convert_to_request_log(message = format_messages(self.interim_history, use_system_prompt= True), meta_info= meta_info, component="llm", direction="request", model=self.task_config["tools_config"]["llm_agent"]["classification_model"])
-            async for text_chunk in self.tools['llm_agent'].generate(self.interim_history, stream=True, synthesize=True,
-                                                                     label_flow=self.label_flow):
-                if text_chunk == "<end_of_conversation>":
+            self.__convert_to_request_log(message = format_messages(messages, use_system_prompt= True), meta_info= meta_info, component="llm", direction="request", model=self.task_config["tools_config"]["llm_agent"]["model"])
+            async for next_state in self.tools['llm_agent'].generate(messages, label_flow=self.label_flow):
+                if next_state == "<end_of_conversation>":
                     meta_info["end_of_conversation"] = True
                     self.buffered_output_queue.put_nowait(create_ws_data_packet("<end_of_conversation>", meta_info))
                     return
                 
-                logger.info(f"Text chunk {text_chunk} callee speaking {self.callee_speaking}")
-                if is_valid_md5(text_chunk):
-                    self.synthesizer_tasks.append(asyncio.create_task(
-                        self._synthesize(create_ws_data_packet(text_chunk, meta_info, is_md5_hash=True))))
-                else:
-                    self.synthesizer_tasks.append(asyncio.create_task(
-                        self._synthesize(create_ws_data_packet(text_chunk, meta_info, is_md5_hash=False))))
-            
-            logger.info(f"Interim history after the LLM task {self.interim_history}")
-            self.__update_transcripts()
+                logger.info(f"Text chunk {next_state['text']}")
+                messages.append({'role': 'assistant', 'content': next_state['text']})
+                self.synthesizer_tasks.append(asyncio.create_task(
+                        self._synthesize(create_ws_data_packet(next_state['audio'], meta_info, is_md5_hash=True))))
+            logger.info(f"Interim history after the LLM task {messages}")
+            self.llm_response_generated = True
+            self.interim_history = copy.deepcopy(messages)
+            if self.callee_silent:
+                logger.info("When we got utterance end, maybe LLM was still generating response. So, copying into history")
+                self.history = copy.deepcopy(self.interim_history)
 
 
     async def _process_conversation_formulaic_task(self, message, sequence, meta_info):
-        start_time = time.time()
         llm_response = ""
         logger.info("Agent flow is formulaic and hence moving smoothly")
-        async for text_chunk in self.tools['llm_agent'].generate(self.history, stream=True, synthesize=True):
+        async for text_chunk in self.tools['llm_agent'].generate(self.history):
             if is_valid_md5(text_chunk):
                 self.synthesizer_tasks.append(asyncio.create_task(
                     self._synthesize(create_ws_data_packet(text_chunk, meta_info, is_md5_hash=True))))
             else:
                 # TODO Make it more modular
                 llm_response += " " +text_chunk
                 next_step = self._get_next_step(sequence, "llm")
                 if next_step == "synthesizer":
-                    task = asyncio.gather(self._synthesize(create_ws_data_packet(text_chunk, meta_info)))
-                    self.synthesizer_tasks.append(asyncio.ensure_future(task))
+                    self.synthesizer_tasks.append(asyncio.create_task(self._synthesize(create_ws_data_packet(text_chunk, meta_info))))
                 else:
                     logger.info(f"Sending output text {sequence}")
                     await self.tools["output"].handle(create_ws_data_packet(text_chunk, meta_info))
                     self.synthesizer_tasks.append(asyncio.create_task(
                         self._synthesize(create_ws_data_packet(text_chunk, meta_info, is_md5_hash=False))))
 
     async def _process_conversation_task(self, message, sequence, meta_info):
@@ -540,68 +664,113 @@
         logger.info("agent flow is not preprocessed")
         llm_response = ""
 
         start_time = time.time()
         should_bypass_synth = 'bypass_synth' in meta_info and meta_info['bypass_synth'] == True
         next_step = self._get_next_step(sequence, "llm")        
         meta_info['llm_start_time'] = time.time()
-        cache_response = self.cache.get(get_md5_hash(message['data'])) if self.cache is not None else None
-        if cache_response is not None:
-            logger.info("It was a cache hit and hence simply returning")
+        route = None
+        if self.route_layer is not None:
+            route = self.route_layer(message['data']).name
+            logger.info(f"Got route name {route}")
+        
+        if route is not None:
+            logger.info(f"It was a route hit and we've got to respond from cache hence simply returning and the route is {route}")
+            # Check if for the particular route if there's a vector store
+            # If not send the response else get the response from the vector store
+            logger.info(f"Vector caches {self.vector_caches}")
+            if route in self.vector_caches:
+                logger.info(f"Route {route} has a vector cache")
+                relevant_utterance = self.vector_caches[route].get(message['data'])
+                cache_response = self.route_responses_dict[route][relevant_utterance]
+                self.__convert_to_request_log(message = message['data'], meta_info= meta_info, component="llm", direction="request", model=self.task_config["tools_config"]["llm_agent"]["model"])
+                self.__convert_to_request_log(message = message['data'], meta_info= meta_info, component="llm", direction="response", model=self.task_config["tools_config"]["llm_agent"]["model"])
+                messages = copy.deepcopy(self.history)
+                messages += [{'role': 'user', 'content': message['data']},{'role': 'assistant', 'content': cache_response}]
+                self.interim_history = copy.deepcopy(messages)
+                self.llm_response_generated = True
+                if self.callee_silent:
+                    logger.info("##### When we got utterance end, maybe LLM was still generating response. So, copying into history")
+                    self.history = copy.deepcopy(self.interim_history)
+
+            else:
+                logger.info(f"Route doesn't have a vector cache, and hence simply returning back a given response")
+                cache_response = self.route_responses_dict[route]
+            
+            logger.info(f"Cached response {cache_response}")
+            meta_info['cached'] = True
+            meta_info["end_of_llm_stream"] = True
+                
             await self._handle_llm_output(next_step, cache_response, should_bypass_synth, meta_info)
+            self.llm_processed_request_ids.add(self.current_request_id)
         else:
-            #messages = [self.interim_history[0], {'role': 'user', 'content': format_messages(self.history)}]
-            self.interim_history.append({'role': 'user', 'content': message['data']})
+            messages = copy.deepcopy(self.history)
+            messages.append({'role': 'user', 'content': message['data']})
             ### TODO CHECK IF THIS IS EVEN REQUIRED
-            self.__convert_to_request_log(message=format_messages(self.interim_history, use_system_prompt= True), meta_info= meta_info, component="llm", direction="request", model=self.task_config["tools_config"]["llm_agent"]["streaming_model"])
+            self.__convert_to_request_log(message=format_messages(messages, use_system_prompt= True), meta_info= meta_info, component="llm", direction="request", model=self.task_config["tools_config"]["llm_agent"]["model"])
             
-            async for llm_message in self.tools['llm_agent'].generate(self.interim_history, synthesize=True):
+            async for llm_message in self.tools['llm_agent'].generate(messages, synthesize=True):
                 text_chunk, end_of_llm_stream = llm_message
-                logger.info(f"###### time to get the first chunk {time.time() - start_time} {text_chunk}")
                 llm_response += " " + text_chunk
                 if self.stream:
                     if end_of_llm_stream:
                         meta_info["end_of_llm_stream"] = True
                     text_chunk = self.__process_stop_words(text_chunk, meta_info)
+                    logger.info(f"##### O/P from LLM {text_chunk} {llm_response}")
                     await self._handle_llm_output(next_step, text_chunk, should_bypass_synth, meta_info)
                     
             if not self.stream:
                 meta_info["end_of_llm_stream"] = True
+                messages.append({"role": "assistant", "content": llm_response})
+                self.history = copy.deepcopy(messages)
                 await self._handle_llm_output(next_step, llm_response, should_bypass_synth, meta_info)
-                self.__convert_to_request_log(message = llm_response, meta_info= meta_info, component="llm", direction="response", model=self.task_config["tools_config"]["llm_agent"]["streaming_model"])
-
-        if self.current_request_id in self.llm_rejected_request_ids:
-            logger.info("User spoke while LLM was generating response")
-        else:
-            self.interim_history.append({"role": "assistant", "content": llm_response})
-            self.__convert_to_request_log(message=llm_response, meta_info= meta_info, component="llm", direction="response", model=self.task_config["tools_config"]["llm_agent"]["streaming_model"])
-            self.__update_transcripts()
+                self.__convert_to_request_log(message = llm_response, meta_info= meta_info, component="llm", direction="response", model=self.task_config["tools_config"]["llm_agent"]["model"])
+            else:    
+                if self.current_request_id in self.llm_rejected_request_ids:
+                    logger.info("##### User spoke while LLM was generating response")
+                else:
+                    messages.append({"role": "assistant", "content": llm_response})
+                    self.__convert_to_request_log(message=llm_response, meta_info= meta_info, component="llm", direction="response", model=self.task_config["tools_config"]["llm_agent"]["model"])
+                    self.interim_history = copy.deepcopy(messages)
+                    self.llm_response_generated = True
+                    if self.callee_silent:
+                        logger.info("##### When we got utterance end, maybe LLM was still generating response. So, copying into history")
+                        self.history = copy.deepcopy(self.interim_history)
+                    #self.__update_transcripts()
 
             # TODO : Write a better check for completion prompt 
-            #answer = await self.tools["llm_agent"].check_for_completion(self.history)
-            answer = False
-            if answer:
-                await self.__process_end_of_conversation()
-                return
+            if self.use_llm_to_determine_hangup and not self.connected_through_dashboard:
+                answer = await self.tools["llm_agent"].check_for_completion(self.history, self.check_for_completion_prompt)
+                should_hangup = answer['answer'].lower() == "yes"
+                prompt = [
+                        {'role': 'system', 'content': self.check_for_completion_prompt},
+                        {'role': 'user', 'content': format_messages(self.history, use_system_prompt= True)}]
+                logger.info(f"##### Answer from the LLM {answer}")
+                self.__convert_to_request_log(message=format_messages(prompt, use_system_prompt= True), meta_info= meta_info, component="llm", direction="request", model=self.task_config["tools_config"]["llm_agent"]["model"])
+                self.__convert_to_request_log(message=answer, meta_info= meta_info, component="llm", direction="response", model= self.check_for_completion_llm)
+                
+                if should_hangup:
+                    await self.__process_end_of_conversation()
+                    return
 
             self.llm_processed_request_ids.add(self.current_request_id)
             llm_response = ""
     
     async def _listen_llm_input_queue(self):
         logger.info(
             f"Starting listening to LLM queue as either Connected to dashboard = {self.connected_through_dashboard} or  it's a textual chat agent {self.textual_chat_agent}")
         while True:
             try:
                 ws_data_packet = await self.queues["llm"].get()
                 logger.info(f"ws_data_packet {ws_data_packet}")
                 meta_info = self.__get_updated_meta_info(ws_data_packet['meta_info'])
                 bos_packet = create_ws_data_packet("<beginning_of_stream>", meta_info)
                 await self.tools["output"].handle(bos_packet)
-                self.interim_history = self.history.copy()
-                self.history.append({'role': 'user', 'content': ws_data_packet['data']})
+                # self.interim_history = self.history.copy()
+                # self.history.append({'role': 'user', 'content': ws_data_packet['data']})
                 await self._run_llm_task(
                     create_ws_data_packet(ws_data_packet['data'], meta_info))
                 if self._is_preprocessed_flow():
                     self.__update_preprocessed_tree_node()
                 eos_packet = create_ws_data_packet("<end_of_stream>", meta_info)
                 await self.tools["output"].handle(eos_packet)
 
@@ -615,14 +784,17 @@
         logger.info(f"After adding {self.curr_sequence_id} into sequence id {self.sequence_ids} for message {message}")
 
         try:
             if self._is_extraction_task() or self._is_summarization_task():
                 await self._process_followup_task(message)
             elif self._is_conversation_task():
                 if self._is_preprocessed_flow():
+                    if time.time() < self.consider_next_transcript_after:
+                        logger.info("Not considering transcript as we're still in cool down period")
+                        await asyncio.sleep(self.consider_next_transcript_after - time.time())
                     logger.info(f"Running preprocessedf task")
                     await self._process_conversation_preprocessed_task(message, sequence, meta_info)
 
                 elif self._is_formulaic_flow():
                     await self._process_conversation_formulaic_task(message, sequence, meta_info)
                 else:
                     await self._process_conversation_task(message, sequence, meta_info)
@@ -651,16 +823,14 @@
             self.llm_rejected_request_ids.add(self.previous_request_id)
         else:
             skip_append_to_data = False
         return sequence
 
     async def _handle_transcriber_output(self, next_task, transcriber_message, meta_info):
         self.__convert_to_request_log(message=transcriber_message, meta_info= meta_info, model = "deepgram")
-        if time.time() < self.consider_next_transcript_after:
-            logger.info("Not considering transcript as we're still in cool down period")
         if next_task == "llm":
             logger.info(f"Running llm Tasks")
             meta_info["origin"] = "transcriber"
             self.llm_task = asyncio.create_task(
                 self._run_llm_task(create_ws_data_packet(transcriber_message, meta_info)))
         elif next_task == "synthesizer":
             self.synthesizer_tasks.append(asyncio.create_task(
@@ -668,91 +838,140 @@
         else:
             logger.info(f"Need to separate out output task")
 
     async def _listen_transcriber(self):
         transcriber_message = ""
         logger.info(f"Starting transcriber task")
         response_started = False
+        num_words = 0
         try:
             while True:
                 message = await self.transcriber_output_queue.get()
-                logger.info(f"Message from the transcriber class {message}")
+                logger.info(f"##### Message from the transcriber class {message}")
                 if message["data"].strip() == "":
                     continue
                 if message['data'] == "transcriber_connection_closed":
                     self.transcriber_duration += message['meta_info']["transcriber_duration"]
                     logger.info("transcriber connection closed")
                     break
-                
+
                 if self.stream:
                     self._set_call_details(message)
                     meta_info = message["meta_info"]
                     sequence = await self.process_transcriber_request(meta_info)
                     next_task = self._get_next_step(sequence, "transcriber")
+                    num_words = 0
                     if message['data'] == "TRANSCRIBER_BEGIN":
-                        self.callee_silent = False
-                        self.start_response = False #Make start response as false
-
-                        self.interim_history = copy.deepcopy(self.history)
-                        self.callee_speaking = True
                         response_started = False #This signifies if we've gotten the first bit of interim text for the given response or not
-                        if meta_info.get("should_interrupt", False):
-                            logger.info(f"Processing interruption from TRANSCRIBER_BEGIN")
+                        self.callee_silent = False
+                        if self.nitro:
+                            logger.info(f"Just a nitro thingy")
+                            should_interrupt = meta_info.get("should_interrupt", True)
+                            # if not should_interrupt and self.started_transmitting_audio:
+                            #     # Ideally is we are transmitting, we want to wait for x seconds here to make sure if we interrupt or not 
+                            #     # So, we send a clear message for sure but use a variable to make sure that we wait 
+                            #     # then if we haven't received interruption signal, we simply continue
+                            #     # If we have, we interrupt  
+                            #     # Send a clear message
+                            #     await self.tools["output"].handle_interruption()
+                            #     self.backoff_until = (time.time() * 1000) + self.interruption_backoff_period
+                            #     self.allow_extra_sleep = True
+                            #     logger.info(f"###### Sending interrupt to clear and allowing extra sleep to wait for more messages as we are transmitting audio right now. {self.backoff_until}")
+                        
+                        else:
+                            logger.info(f"###### Processing interruption from TRANSCRIBER_BEGIN for non nitro mode")
                             await self.process_interruption()
                     elif "speech_final" in meta_info and meta_info['speech_final'] and message['data'] != "":
                         logger.info(f"Starting the TRANSCRIBER_END TASK")
-                        self.start_response = True
+                        self.callee_speaking = False
+                        self.callee_silent = True
                         if self.output_task is None:
                             logger.info(f"Output task was none and hence starting it")
+                            self.output_task = asyncio.create_task(self.__process_output_loop())
 
                         if self._is_preprocessed_flow():
                             self.__update_preprocessed_tree_node()
-
-                        self.callee_speaking = False
-                        assistant_message = None
-
-                        # If last two messages are humans
-
-                        if ((len(self.history)  == 1 and self.history[-1]['role'] == "assistant")) or (len(self.history)  > 1 and self.history[-1]['role'] == 'assistant' and (self.history[-2]['role'] in ['assistant', 'system'] )):
-                            assistant_message = self.history[-1].copy()
-                            self.history = self.history[:-1]
-
-                        logger.info(f"APPENDING USER statement {message['data']}")
-                        self.history.append({'role': 'user', 'content': transcriber_message})
-                        if assistant_message is not None:
-                            self.history.append(assistant_message)
                         
+                        logger.info(f"INTERIM TRANSCRIPT WHEN EVERYTING IS OVER {self.interim_history}")
+                        if self.llm_response_generated:
+                            logger.info(f"LLM RESPONSE WAS GENERATED AND HENCE MOVING INTERIM HISTORY TO HISTORY")
+                            self.history = copy.deepcopy(self.interim_history)
                         meta_info = message['meta_info']
                         transcriber_message = ""
-                        continue
+                        self.let_remaining_audio_pass_through = True 
+
+                        if self.nitro:
+                            self.time_since_first_interim_result = -1
+                            self.required_delay_before_speaking = max(self.minimum_wait_duration - self.incremental_delay, 0)
+                            logger.info(f"#### Resetting time since first interim result and resetting required delay {self.required_delay_before_speaking}")
+                        
                     else:
+                        self.time_since_last_spoken_human_word = time.time()
                         logger.info(f'invoking next_task {next_task} with transcriber_message: {message["data"]}')
                         if transcriber_message.strip() == message['data'].strip():
-                            logger.info("Transcriber message and message data are same and hence not changing anything else")
+                            logger.info(f"###### Transcriber message and message data are same and hence not changing anything else. Probably just an is_final thingy. {message}")
                             continue
 
                         elif len(message['data'].strip()) != 0:
                             #Currently simply cancel the next task
-                            #TODO add more optimisation by just getting next x tokens or something similar
-                            await self.__cleanup_downstream_tasks()
+                            num_words += len(message['data'].split(" "))
+                            if self.callee_speaking is False:
+                                self.callee_speaking_start_time = time.time()
+                                self.callee_speaking = True
+                            # if self.started_transmitting_audio:
+                            #     # Ideally is we are transmitting, we want to wait for x seconds here to make sure if we interrupt or not 
+                            #     # So, we send a clear message for sure but use a variable to make sure that we wait 
+                            #     # then if we haven't received interruption signal, we simply continue
+                            #     # If we have, we interrupt  
+                            #     # Send a clear message
+                            #     await self.tools["output"].handle_interruption()
+                            #     self.backoff_until = (time.time() * 1000) + self.interruption_backoff_period
+                            #     self.allow_extra_sleep = True
+                            #     logger.info(f"Sending interrupt to clear and allowing extra sleep to wait for more messages as we are transmitting audio right now. {self.backoff_until}")
+
+                            
+                            # This means we are generating response from an interim transcript 
+                            # Hence we transmit quickly 
+                            if not self.started_transmitting_audio:
+                                logger.info("##### Haven't started transmitting audio and hence cleaning up downstream tasks")
+                                await self.__cleanup_downstream_tasks()
+                            
+                            # If we've started transmitting audio this is probably an interruption, so calculate number of words
+                            if self.nitro and self.started_transmitting_audio:
+                                if num_words > self.number_of_words_for_interruption:
+                                    #Process interruption only if number of words is higher than the threshold 
+                                    logger.info(f"###### Number of words {num_words} is higher than the required number of words for interruption, hence, definitely interrupting")
+                                    await self.__cleanup_downstream_tasks()
+                                else:
+                                    logger.info(f"Not starting a cleanup because {num_words} number of words are lesser {self.number_of_words_for_interruption} and hence continuing,")
+                                    continue
+                                    
                             self.last_response_time = time.time()
                             transcriber_message = message['data']
+                            
+                            # Use last spoken timestamp to give out endpointing in nitro
+                            logger.info(f"###### last spoken timestamp before changing {self.last_spoken_timestamp}")
+                            self.last_spoken_timestamp = time.time() * 1000
 
                             if not response_started:
                                 response_started = True
-                            elif self.kwargs['process_interim_results'] == "true":
+                            elif self.nitro:
+                                self.let_remaining_audio_pass_through = False
+                                logger.info(f"Increase the incremental delay time")
+                                self.required_delay_before_speaking += self.incremental_delay
+                                if self.time_since_first_interim_result == -1:
+                                    self.time_since_first_interim_result = time.time() * 1000
+                                    logger.info(f"###### Updating Time since first interim result {self.time_since_first_interim_result}")
                                 #In this case user has already started speaking
                                 # Hence check the previous message if it's user or assistant
                                 # If it's user, simply change user's message
                                 # If it's assistant remover assistant message and append user
-                                if self.interim_history[-1]['role'] == 'assistant':
-                                    self.interim_history = self.interim_history[:-1]
-                                else:
-                                    self.interim_history = self.interim_history[:-2]
-                            logger.info("Current transcript: {} Predicting next few tokens".format(transcriber_message))
+                                self.callee_silent = False
+                            self.llm_response_generated = False
+                            logger.info("###### Current transcript: {} Predicting next few tokens and changing last spoken timestampt to {}".format(transcriber_message, self.last_spoken_timestamp))
                             meta_info = self.__get_updated_meta_info(meta_info)
                             await self._handle_transcriber_output(next_task, transcriber_message, meta_info)
 
                         else:
                             logger.info(f"Got a null message")
                 else:
                     logger.info(f"Processing http transcription for message {message}")
@@ -768,24 +987,39 @@
         include_latency = meta_info.get("include_latency", False)
         if include_latency:
             self.latency_dict[meta_info['request_id']]["transcriber"] = {"total_latency":  meta_info["transcriber_latency"], "audio_duration": meta_info["audio_duration"], "last_vocal_frame_timestamp": meta_info["last_vocal_frame_timestamp"] }
 
         sequence = message["meta_info"]["sequence"]
         next_task = self._get_next_step(sequence, "transcriber")
         self.transcriber_duration += message["meta_info"]["transcriber_duration"] if "transcriber_duration" in message["meta_info"] else 0
-        self.history.append({'role': 'user', 'content': message['data']})
+        #self.history.append({'role': 'user', 'content': message['data']})
         if self._is_preprocessed_flow():
             self.__update_preprocessed_tree_node()
 
         await self._handle_transcriber_output(next_task, message['data'], meta_info)
 
 
     #################################################################
     # Synthesizer task
     #################################################################
+    def __enqueue_chunk(self, chunk, i, number_of_chunks, meta_info):
+        logger.info(f"Meta_info of chunk {meta_info} {i} {number_of_chunks}")
+        if i == 0 and "is_first_chunk" in meta_info and meta_info["is_first_chunk"]:
+            copied_meta_info = copy.deepcopy(meta_info)
+            logger.info(f"##### Sending first chunk")
+            copied_meta_info["is_first_chunk_of_entire_response"] = True
+            self.buffered_output_queue.put_nowait(create_ws_data_packet(chunk, copied_meta_info))
+        elif i == number_of_chunks and "end_of_synthesizer_stream" in meta_info and meta_info['end_of_synthesizer_stream']:
+            logger.info(f"##### Truly a final chunk")
+            copied_meta_info = meta_info.copy()
+            copied_meta_info["is_final_chunk_of_entire_response"] = True
+            self.buffered_output_queue.put_nowait(create_ws_data_packet(chunk, copied_meta_info))
+        else:
+            self.buffered_output_queue.put_nowait(create_ws_data_packet(chunk, meta_info))
+
     async def __listen_synthesizer(self):
         try:
             if self.stream and self.synthesizer_provider != "polly" and not self.is_an_ivr_call: 
                 logger.info("Opening websocket connection to synthesizer")
                 await self.tools["synthesizer"].open_connection()
             while True:
                 logger.info("Listening to synthesizer")
@@ -793,102 +1027,113 @@
                     meta_info = message["meta_info"]
                     if not self.conversation_ended and message["meta_info"]["sequence_id"] in self.sequence_ids:
                         logger.info(f"{message['meta_info']['sequence_id'] } is in sequence ids  {self.sequence_ids} and hence removing the sequence ids ")
                         if self.stream:   
                             if self.synthesizer_provider == "polly":
                                 if message['meta_info']['is_first_chunk']:
                                     first_chunk_generation_timestamp = time.time()
-                                    #self.latency_dict[message['meta_info']["request_id"]]['synthesizer'] = {"first_chunk_generation_latency": first_chunk_generation_timestamp - message['meta_info']['synthesizer_start_time'], "first_chunk_generation_timestamp": first_chunk_generation_timestamp}
                                     meta_info["synthesizer_first_chunk_latency"] = first_chunk_generation_timestamp - message['meta_info']['synthesizer_start_time']
                                 logger.info(f"Simply Storing in buffered output queue for now")
 
                                 if self.yield_chunks:
-                                    for chunk in yield_chunks_from_memory(message['data'], chunk_size=16384):
-                                        self.buffered_output_queue.put_nowait(create_ws_data_packet(chunk, meta_info))
-                                
+                                    logger.info(f"Yielding chunks")
+                                    number_of_chunks = (len(message['data'])//self.output_chunk_size)
+                                    i = 0
+                                    for chunk in yield_chunks_from_memory(message['data'], chunk_size=self.output_chunk_size):
+                                        self.__enqueue_chunk(chunk, i, number_of_chunks, meta_info)
+                                        i +=1
                                 else:
                                     self.buffered_output_queue.put_nowait(message)
                                 
                             else:
                                 if self.task_config["tools_config"]["output"]["provider"] in SUPPORTED_INPUT_TELEPHONY_HANDLERS.keys() and not self.connected_through_dashboard and self.synthesizer_provider == "elevenlabs":
                                     if meta_info.get('format', '') != 'mulaw':
                                         message['data'] = wav_bytes_to_pcm(message['data'])
                                 
                                 if "is_first_chunk" in message['meta_info'] and message['meta_info']['is_first_chunk']:
                                     first_chunk_generation_timestamp = time.time()
                                     meta_info["synthesizer_first_chunk_latency"] = first_chunk_generation_timestamp - message['meta_info']['synthesizer_start_time']
                                     #self.latency_dict[message['meta_info']["request_id"]]['synthesizer'] = {"first_chunk_generation_latency": first_chunk_generation_timestamp - message['meta_info']['synthesizer_start_time'], "first_chunk_generation_timestamp": first_chunk_generation_timestamp}
                                 
                                 if self.yield_chunks:
-                                    for chunk in yield_chunks_from_memory(message['data'], chunk_size=16384):
-                                        self.buffered_output_queue.put_nowait(create_ws_data_packet(chunk, meta_info))
+                                    number_of_chunks = (len(message['data'])/self.output_chunk_size)
+                                    i = 0
+                                    for chunk in yield_chunks_from_memory(message['data'], chunk_size=self.output_chunk_size):
+                                        i+=1
+                                        self.__enqueue_chunk(chunk, i, number_of_chunks, meta_info)
                                 else:
                                     self.buffered_output_queue.put_nowait(message)
-                                #await self.tools["output"].handle(message)
                             
                         else:
                             logger.info("Stream is not enabled and hence sending entire audio")
                             first_chunk_generation_timestamp = time.time()
                             self.latency_dict[message['meta_info']["request_id"]]['synthesizer'] = {"first_chunk_generation_latency": first_chunk_generation_timestamp - message['meta_info']['synthesizer_start_time'], "first_chunk_generation_timestamp": first_chunk_generation_timestamp}
+                            #self.history = copy.deepcopy(self.interim_history)
+                            logger.info(f"Changing history")
                             await self.tools["output"].handle(message)
                     else:
                         logger.info(f"{message['meta_info']['sequence_id']} is not in sequence ids  {self.sequence_ids} and hence not sending to output")                
-                    logger.info(f"Sleeping for 300 ms")
+                    logger.info(f"Sleeping for 100 ms")
                     await asyncio.sleep(0.3) #Sleeping for 100ms after receiving every chunk so other tasks can execute
 
         except Exception as e:
             traceback.print_exc()
             logger.error(f"Error in synthesizer {e}")
 
     async def __send_preprocessed_audio(self, meta_info, text):
         #TODO: Either load IVR audio into memory before call or user s3 iter_cunks
         # This will help with interruption in IVR
         if self.connected_through_dashboard or self.task_config['tools_config']['output'] == "default":
-            audio_chunk = await get_raw_audio_bytes_from_base64(self.assistant_name, text,
+            audio_chunk = await get_raw_audio_bytes(text, self.assistant_name,
                                                             self.task_config["tools_config"]["output"][
                                                                 "format"], local=self.is_local,
                                                             assistant_id=self.assistant_id)
-
+            logger.info("Sending preprocessed audio")
             await self.tools["output"].handle(create_ws_data_packet(audio_chunk, meta_info))
         else:
-            audio_chunk = await get_raw_audio_bytes_from_base64(self.assistant_name, text,
+            audio_chunk = await get_raw_audio_bytes( text, self.assistant_name,
                                                             'pcm', local=self.is_local,
                                                             assistant_id=self.assistant_id)
-
+            
             if not self.buffered_output_queue.empty():
                 logger.info(f"Output queue was not empty and hence emptying it")
                 self.buffered_output_queue = asyncio.Queue()
 
             if self.yield_chunks:
-                for chunk in yield_chunks_from_memory(audio_chunk, chunk_size=16384):
+                for chunk in yield_chunks_from_memory(audio_chunk, chunk_size=self.output_chunk_size):
                     logger.debug("Sending chunk to output queue")
                     message = create_ws_data_packet(chunk, meta_info)
                     self.buffered_output_queue.put_nowait(message)
             else:
                 message = create_ws_data_packet(audio_chunk, meta_info)
+                logger.info(f"Yield in chunks is false and hence sending a full")
                 self.buffered_output_queue.put_nowait(message)
 
     async def _synthesize(self, message):
         meta_info = message["meta_info"]
         text = message["data"]
         meta_info["type"] = "audio"
         meta_info["synthesizer_start_time"] = time.time()
         try:
             if not self.conversation_ended and message["meta_info"]["sequence_id"] in self.sequence_ids:
                 if meta_info["is_md5_hash"]:
                     logger.info('sending preprocessed audio response to {}'.format(self.task_config["tools_config"]["output"]["provider"]))
                     await self.__send_preprocessed_audio(meta_info, text)
-
+                    
                 elif self.synthesizer_provider in SUPPORTED_SYNTHESIZER_MODELS.keys():
                     # self.sequence_ids.add(meta_info["sequence_id"])
                     # logger.info(f"After adding into sequence id {self.sequence_ids}")
                     self.__convert_to_request_log(message = text, meta_info= meta_info, component="synthesizer", direction="request", model = self.synthesizer_provider)
-                    logger.info('sending text to {} for generation: {} '.format(self.synthesizer_provider, text))
-                    self.synthesizer_characters += len(text)
-                    await self.tools["synthesizer"].push(message)
+                    logger.info('##### sending text to {} for generation: {} '.format(self.synthesizer_provider, text))
+                    if 'cached' in message['meta_info'] and meta_info['cached'] == True:
+                        logger.info(f"Cached response and hence sending preprocessed text")
+                        await self.__send_preprocessed_audio(meta_info, get_md5_hash(text))
+                    else:
+                        self.synthesizer_characters += len(text)
+                        await self.tools["synthesizer"].push(message)
                 else:
                     logger.info("other synthesizer models not supported yet")
             else:
                 logger.info(f"{message['meta_info']['sequence_id']} is not in sequence ids  {self.sequence_ids} and hence not synthesizing this")                
 
         except Exception as e:
             traceback.print_exc()
@@ -902,33 +1147,70 @@
         await asyncio.sleep(5)
         if self.callee_silent and len(self.history) == 1 and len(self.interim_history) == 1:
             logger.info(f"Calee was silent and hence speaking Hello on callee's behalf")
             meta_info = self.__get_updated_meta_info()
             sequence = meta_info["sequence"]
             next_task = self._get_next_step(sequence, "transcriber")
             await self._handle_transcriber_output(next_task, "Hello", meta_info)
+            self.time_since_first_interim_result = (time.time() * 1000) - 1000
             
     #Currently this loop only closes in case of interruption 
     # but it shouldn't be the case. 
     async def __process_output_loop(self):
+        prev_message = None
+        current_message = None
         try:
             while True:
-                logger.info(f"Yielding to output handler")
-                message = await self.buffered_output_queue.get()
-                logger.info("Start response is True and hence starting to speak {} Current sequence ids".format(message['meta_info'], self.sequence_ids))
+                # Allow extra sleep allows us to have real time impact in when uer starts speaking
+                # if self.nitro and self.allow_extra_sleep and time.time() *1000 < self.backoff_until:
+                #     logger.info(f"##### sleeping for extra backoff period to see if user will start speaking something new or not after {self.interruption_backoff_period/1000}")
+                #     await asyncio.sleep(self.interruption_backoff_period/1000)
+                #     self.allow_extra_sleep = False
+                #     prev_message = current_message
+
+                if self.nitro and not self.let_remaining_audio_pass_through:
+                    time_since_first_interim_result = (time.time() *1000)- self.time_since_first_interim_result if self.time_since_first_interim_result != -1 else -1
+                    if  time_since_first_interim_result != -1 and time_since_first_interim_result < self.required_delay_before_speaking:
+                        logger.info(f"##### It's been {time_since_first_interim_result} ms since first  interim result and required time to wait for it is {self.required_delay_before_speaking}. Hence sleeping for 100ms. self.time_since_first_interim_result {self.time_since_first_interim_result}")
+                        await asyncio.sleep(0.1) #sleep for 100ms and continue 
+                        continue
+                    else:
+                        logger.info(f"First interim result hasn't been gotten yet and hence sleeping ")
+                        await asyncio.sleep(0.1)
+
+                    logger.info(f"##### Got to wait {self.required_delay_before_speaking} ms before speaking and alreasy waited {time_since_first_interim_result} since the first interim result")
+                else:
+                    logger.info(f"Started transmitting at {time.time()}")
+                if prev_message is None:
+                    message = await self.buffered_output_queue.get()   
+                    current_message = message 
+                else:
+                    logger.info(f'prev message is not none and hence getting prev message')
+                    message = prev_message
+                    prev_message = None
+                logger.info("##### Start response is True and hence starting to speak {} Current sequence ids".format(message['meta_info'], self.sequence_ids))
                 if "end_of_conversation" in message['meta_info']:
                     await self.__process_end_of_conversation()
                 
                 if 'sequence_id' in message['meta_info'] and message["meta_info"]["sequence_id"] in self.sequence_ids:
-                    await self.tools["output"].handle(message)
+                    await self.tools["output"].handle(message)                    
+                    duration = calculate_audio_duration(len(message["data"]), self.sampling_rate)
+                    logger.info(f"Duration of the byte {duration}")
+                    self.conversation_recording['output'].append({'data': message['data'], "start_time": time.time(), "duration": duration})
                 else:
                     logger.info(f'{message["meta_info"]["sequence_id"]} is not in {self.sequence_ids} and hence not speaking')
                     continue
-
-                if "is_first_chunk" in message['meta_info'] and message['meta_info']['is_first_chunk']:
+                
+                if "is_final_chunk_of_entire_response" in message['meta_info'] and message['meta_info']['is_final_chunk_of_entire_response']:
+                    self.started_transmitting_audio = False
+                    logger.info("##### End of synthesizer stream and ")                    
+
+                if "is_first_chunk_of_entire_response" in message['meta_info'] and message['meta_info']['is_first_chunk_of_entire_response']:
+                    logger.info(f"First chunk stuff")
+                    self.started_transmitting_audio = True
                     meta_info = message['meta_info']
                     self.consider_next_transcript_after = time.time() + self.duration_to_prevent_accidental_interruption
                     utterance_end = meta_info.get("utterance_end", None)
                     overall_first_byte_latency = time.time() - message['meta_info']['utterance_end'] if utterance_end is not None else 0
                     transcriber_latency = message["meta_info"]["transcriber_latency"] if utterance_end is not None else 0
                     first_llm_buffer_latency = message["meta_info"]["llm_first_buffer_generation_latency"] if utterance_end is not None else 0
                     synthesizer_first_chunk_latency = message["meta_info"]["synthesizer_first_chunk_latency"] if utterance_end is not None else 0
@@ -943,24 +1225,66 @@
                             },
                         "llm": {
                             "first_llm_buffer_latency" : first_llm_buffer_latency
                             },
                         "synthesizer": {
                             "synthesizer_first_chunk_latency": synthesizer_first_chunk_latency
                             },
-                        "overall_first_byte_latency": overall_first_byte_latency
+                        "overall_first_byte_latency": overall_first_byte_latency,
+                        
                         }
 
                     if message['meta_info']["request_id"] not in self.latency_dict:
                         self.latency_dict[message['meta_info']["request_id"]] = latency_metrics
                         logger.info("LATENCY METRICS FOR {} are {}".format(message['meta_info']["request_id"], latency_metrics))
+                    
+                    await asyncio.sleep(duration + 0.1) 
+                else:
+                    # Sleep until this particular audio frame is spoken only if the duration for the frame is atleast 500ms
+                    if duration > 0:
+                        logger.info(f"##### Sleeping for {duration} to maintain quueue on our side {self.sampling_rate}")
+                        await asyncio.sleep(duration - 0.010) #10 milliseconds less
+                        
+
+                    
+                self.last_transmitted_timesatamp = time.time()
+                logger.info(f"##### Updating Last transmitted timestamp to {self.last_transmitted_timesatamp}")
+                
         except Exception as e:
             traceback.print_exc()
             logger.error(f'Error in processing message output')
 
+    async def __check_for_completion(self):
+        while True:
+            await asyncio.sleep(2)
+
+            if self.last_transmitted_timesatamp == 0:
+                logger.info(f"Last transmitted timestamp is simply 0 and hence continuing")
+                continue
+
+            time_since_last_spoken_AI_word = (time.time() - self.last_transmitted_timesatamp) 
+            if time_since_last_spoken_AI_word > self.hang_conversation_after and self.time_since_last_spoken_human_word < self.last_transmitted_timesatamp:
+                logger.info(f"{time_since_last_spoken_AI_word} seconds since last spoken time stamp and hence cutting the phone call and last transmitted timestampt ws {self.last_transmitted_timesatamp} and time since last spoken human word {self.time_since_last_spoken_human_word}")
+                await self.__process_end_of_conversation()
+                break
+            else:
+                logger.info(f"Only {time_since_last_spoken_AI_word} seconds since last spoken time stamp and hence cutting the phone call and hence not cutting the phone call")
+    
+    async def __check_for_backchanneling(self):
+        while True:
+            if self.callee_speaking and time.time() - self.callee_speaking_start_time > self.backchanneling_start_delay:
+                filename = random.choice(self.filenames)
+                logger.info(f"Should send a random backchanneling words and sending them {filename}")
+                audio = await get_raw_audio_bytes(f"{self.backchanneling_audios}/{filename}", local= True, is_location=True)
+                if not self.connected_through_dashboard and self.task_config['tools_config']['output'] != "default":
+                    audio = resample(audio, target_sample_rate= 8000, format="wav")
+                await self.tools["output"].handle(create_ws_data_packet(audio, self.__get_updated_meta_info())) 
+            else:
+                logger.info(f"Callee isn't speaking and hence not sending or {time.time() - self.callee_speaking_start_time} is not greater than {self.backchanneling_start_delay}") 
+            await asyncio.sleep(self.backchanneling_message_gap) 
     async def run(self):
         try:
             if self.task_id == 0:
                 # Create transcriber and synthesizer tasks
                 logger.info("starting task_id {}".format(self.task_id))
                 tasks = [asyncio.create_task(self.tools['input'].handle())]
                 if not self.connected_through_dashboard:
@@ -978,15 +1302,19 @@
                     logger.info("Starting synthesizer task")
                     try:
                         self.synthesizer_task = asyncio.create_task(self.__listen_synthesizer())
                     except asyncio.CancelledError as e:
                         logger.error(f'Synth task got cancelled {e}')
                         traceback.print_exc()
                 if self._is_conversation_task():
-                    self.output_task = asyncio.create_task(self.__process_output_loop())         
+                    self.output_task = asyncio.create_task(self.__process_output_loop())
+                    if not self.use_llm_to_determine_hangup and not self.connected_through_dashboard :
+                        self.hangup_task = asyncio.create_task(self.__check_for_completion())
+                    if not self.connected_through_dashboard and self.should_backchannel:
+                        self.backchanneling_task = asyncio.create_task(self.__check_for_backchanneling())
                 try:
                     await asyncio.gather(*tasks)
                 except asyncio.CancelledError as e:
                     logger.error(f'task got cancelled {e}')
                     traceback.print_exc()
                 except Exception as e:
                     traceback.print_exc()
@@ -1015,21 +1343,33 @@
             self.handle_cancellation(f"Exception occurred {e}")
             raise Exception(e)
 
         finally:
             # Construct output
             if "synthesizer" in self.tools and self.synthesizer_task is not None:   
                 self.synthesizer_task.cancel()
+            if self.use_llm_to_determine_hangup is False and self._is_conversation_task() and not self.connected_through_dashboard:
+                self.hangup_task.cancel()
+            
+            if self._is_conversation_task():
+                self.output_task.cancel()
+            
+            if self._is_conversation_task() and self.backchanneling_task is not None:
+                self.backchanneling_task.cancel()
             
             if self.task_id == 0:
                 output = {"messages": self.history, "conversation_time": time.time() - self.start_time,
                           "label_flow": self.label_flow, "call_sid": self.call_sid, "stream_sid": self.stream_sid,
                           "transcriber_duration": self.transcriber_duration,
-                          "synthesizer_characters": self.synthesizer_characters, "ended_by_assistant": self.ended_by_assistant,
+                          "synthesizer_characters": self.tools['synthesizer'].get_synthesized_characters(), "ended_by_assistant": self.ended_by_assistant,
                           "latency_dict": self.latency_dict}
+
+                if self.should_record:
+                    output['recording_url'] = await save_audio_file_to_s3(self.conversation_recording, self.sampling_rate, self.assistant_id, self.run_id)
+
             else:
                 output = self.input_parameters
                 if self.task_config["task_type"] == "extraction":
                     output = { "extracted_data" : self.extracted_data, "task_type": "extraction"}
                 elif self.task_config["task_type"] == "summarization":
                     logger.info(f"self.summarized_data {self.summarized_data}")
                     output = {"summary" : self.summarized_data, "task_type": "summarization"}
```

### Comparing `bolna-0.7.5/bolna/agent_types/contextual_conversational_agent.py` & `bolna-0.7.7/bolna/agent_types/contextual_conversational_agent.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 logger = configure_logger(__name__)
 
 
 class StreamingContextualAgent(BaseAgent):
     def __init__(self, llm):
         super().__init__()
         self.llm = llm
-        self.conversation_completion_llm = OpenAiLLM(classification_model=os.getenv('CHECK_FOR_COMPLETION_LLM', llm.classification_model))
+        self.conversation_completion_llm = OpenAiLLM(model=os.getenv('CHECK_FOR_COMPLETION_LLM', llm.model))
         self.history = [{'content': ""}]
 
-    async def check_for_completion(self, messages):
+    async def check_for_completion(self, messages, check_for_completion_prompt = CHECK_FOR_COMPLETION_PROMPT):
         prompt = [
-            {'role': 'system', 'content': CHECK_FOR_COMPLETION_PROMPT},
-            {'role': 'user', 'content': format_messages(messages)}]
+            {'role': 'system', 'content': check_for_completion_prompt},
+            {'role': 'user', 'content': format_messages(messages, use_system_prompt=True)}]
 
         answer = None
-        response = await self.conversation_completion_llm.generate(prompt, True, False, request_json=True)
+        response = await self.conversation_completion_llm.generate(prompt, request_json=True)
         answer = json.loads(response)
 
         logger.info('Agent: {}'.format(answer['answer']))
-        return answer['answer'].lower() == "yes"
+        return answer
 
     async def generate(self, history, synthesize=False):
         async for token in self.llm.generate_stream(history, synthesize=synthesize):
             logger.info('Agent: {}'.format(token))
             yield token
```

### Comparing `bolna-0.7.5/bolna/agent_types/extraction_agent.py` & `bolna-0.7.7/bolna/agent_types/extraction_agent.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,11 +8,11 @@
     def __init__(self, llm, prompt=None):
         super().__init__()
         self.llm = llm
         self.current_messages = 0
         self.is_inference_on = False
         self.has_intro_been_sent = False
 
-    async def generate(self, history, stream=True, synthesize=False):
+    async def generate(self, history):
         logger.info("extracting json from the previous conversation data")
-        json_data = await self.llm.generate(history, stream=False, synthesize=False, request_json=True)
+        json_data = await self.llm.generate(history, request_json=True)
         return json_data
```

### Comparing `bolna-0.7.5/bolna/agent_types/graph_based_conversational_agent.py` & `bolna-0.7.7/bolna/agent_types/graph_based_conversational_agent.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,29 +19,36 @@
         self.classification_labels = classification_labels
         self.prompt = prompt
         self.need_response_generation = False
         self.milestone_check_prompt = milestone_check_prompt
 
 
 class Graph:
-    def __init__(self, conversation_data, preprocessed=False):
+    def __init__(self, conversation_data, preprocessed=False, context_data=None):
         self.preprocessed = preprocessed
         self.root = None
-        self.graph = self._create_graph(conversation_data)
+        self.graph = self._create_graph(conversation_data, context_data)
 
-    def _create_graph(self, data):
+    def _create_graph(self, data, context_data=None):
         logger.info(f"Creating graph")
         node_map = dict()
         for node_id, node_data in data.items():
+            prompt_parts = node_data.get("prompt").split('###Examples')
+            prompt = node_data.get('prompt')
+            if len(prompt_parts) == 2:
+                classification_prompt = prompt_parts[0]
+                user_prompt = update_prompt_with_context(prompt_parts[1], context_data)
+                prompt = '###Examples'.join([classification_prompt, user_prompt])
+
             node = Node(
                 node_id=node_id,
                 node_label=node_data["label"],
                 content=node_data["content"],
                 classification_labels=node_data.get("classification_labels", []),
-                prompt=node_data.get("prompt"),
+                prompt=prompt,
                 children=[],
                 milestone_check_prompt=node_data.get("milestone_check_prompt", ""),
             )
             node_map[node_id] = node
             if node_data["is_root"]:
                 self.root = node
 
@@ -64,15 +71,15 @@
         self.preprocessed = preprocessed
 
         # Goals
         self.graph = None
         self.conversation_intro_done = False
 
     def load_prompts_and_create_graph(self, prompts):
-        self.graph = Graph(prompts)
+        self.graph = Graph(prompts,  context_data=self.context_data)
         self.current_node = self.graph.root
         self.current_node_interim = self.graph.root #Handle interim node because we are dealing with interim results 
 
     def _get_audio_text_pair(self, node):
         ind = random.randint(0, len(node.content) - 1)
         audio_pair = node.content[ind]
         contextual_text = update_prompt_with_context(audio_pair['text'], self.context_data)
@@ -104,40 +111,40 @@
             # @TODO: Add summary of left out messages
             prev_messages = history[-6:]
         else:
             prev_messages = history[1:]
 
         message = [{"role": "system", "content": self.current_node.prompt}] + prev_messages
         # Get classification label from LLM
-        response = await self.llm.generate(message, True, False, request_json=True)
+        response = await self.llm.generate(message, request_json=True)
         logger.info(f"Classification response {response}")
         classification_result = json.loads(response)
         label = classification_result["classification_label"]
         for child in self.current_node.children:
             if child.node_label.strip().lower() == label.strip().lower():
                 self.current_node_interim = child
                 return self._get_audio_text_pair(child)
 
     def update_current_node(self):
         self.current_node = self.current_node_interim
-        
-    async def generate(self, history, stream=False, synthesize=False, label_flow=None):
+    
+    # Label flow is not being used right now as we're logging every request
+    async def generate(self, history, label_flow=None):
         try:
             if self.preprocessed:
                 logger.info(f"Current node {str(self.current_node)}")
                 if len(self.current_node.children) == 0:
                     ind = random.randint(0, len(self.current_node.content) - 1)
                     audio_pair = self.current_node.content[ind]
                     logger.info('Agent: {}'.format(audio_pair.get('text')))
-                    yield audio_pair["audio"]
+                    yield audio_pair
                 else:
                     next_state = await self._get_next_preprocessed_step(history)
                     logger.info('Agent: {}'.format(next_state))
-                    history.append({'role': 'assistant', 'content': next_state['text']})
-                    yield next_state["audio"]
+                    yield next_state
                 
                 if len(self.current_node.children) == 0:
                     await asyncio.sleep(1)
                     yield "<end_of_conversation>"
             else:
                 # @TODO add non-preprocessed flow
                 async for message in self._get_next_formulaic_agent_next_step(history, True, False):
```

### Comparing `bolna-0.7.5/bolna/agent_types/summarization_agent.py` & `bolna-0.7.7/bolna/agent_types/summarization_agent.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,18 +8,18 @@
     def __init__(self, llm, prompt=None):
         super().__init__()
         self.llm = llm
         self.current_messages = 0
         self.is_inference_on = False
         self.has_intro_been_sent = False
 
-    async def generate(self, history, stream=True, synthesize=False):
+    async def generate(self, history):
         summary = ""
         logger.info("extracting json from the previous conversation data")
         try:
-            summary = await self.llm.generate(history, stream=False, synthesize=False, request_json=False)
+            summary = await self.llm.generate(history, request_json=False)
             logger.info(f"summary {summary}")
         except Exception as e:
             import traceback
             traceback.print_exc()
             logger.error(f"error in generating summary: {e}")
         return {"summary": summary}
```

### Comparing `bolna-0.7.5/bolna/agent_types/zapier_agent.py` & `bolna-0.7.7/bolna/agent_types/zapier_agent.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,27 +8,32 @@
 class ZapierAgent(BaseAgent):
     def __init__(self, zap_url, payload=None):
         super().__init__()
         self.zap_url = zap_url
         self.payload = payload or {}
 
     async def __send_payload(self, payload):
-        logger.info(f"Sending a zapier post request {payload}")
-        async with aiohttp.ClientSession() as session:
-            if payload is not None:
-                async with session.post(self.zap_url, json=payload) as response:
-                    if response.status == 200:
-                        data = await response.json()
-                        return data
-                    else:
-                        logger.error(f"Error: {response.status} - {await response.text()}")
-                        return None
-            else:
-                logger.info("Payload was null")
-        return None
+        try:
+            logger.info(f"Sending a zapier post request {payload}")
+            async with aiohttp.ClientSession() as session:
+                if payload is not None:
+                    async with session.post(self.zap_url, json=payload) as response:
+                        if response.status == 200:
+                            # need to check if the returned response is json or not
+                            #data = await response.json()
+                            return True
+                        else:
+                            logger.error(f"Error: {response.status} - {await response.text()}")
+                            return None
+                else:
+                    logger.info("Payload was null")
+            return None
+        except Exception as e:
+            logger.error(f"Something went wrong with webhook {self.zap_url}, {payload}")
+
 
     async def execute(self, payload):
         if not self.zap_url:
             return None
         response = await self.__send_payload(payload)
         logger.info(f"Response {response}")
-        return response['status']
+        return response
```

### Comparing `bolna-0.7.5/bolna/assistant.py` & `bolna-0.7.7/bolna/assistant.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.5/bolna/constants.py` & `bolna-0.7.7/bolna/constants.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.5/bolna/helpers/analytics_helpers.py` & `bolna-0.7.7/bolna/helpers/analytics_helpers.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.5/bolna/helpers/logger_config.py` & `bolna-0.7.7/bolna/helpers/logger_config.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.5/bolna/helpers/utils.py` & `bolna-0.7.7/bolna/helpers/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import json
 import asyncio
+import math
 import re
 import copy
 import hashlib
 import os
 import traceback
 import io
+import wave
 import numpy as np
 import aiofiles
 import torch
 import torchaudio
 from scipy.io import wavfile
 from botocore.exceptions import BotoCoreError, ClientError
 from aiobotocore.session import AioSession
@@ -19,15 +21,16 @@
 from .logger_config import configure_logger
 from bolna.constants import PREPROCESS_DIR
 from pydub import AudioSegment
 
 logger = configure_logger(__name__)
 load_dotenv()
 BUCKET_NAME = os.getenv('BUCKET_NAME')
-
+RECORDING_BUCKET_NAME = os.getenv('RECORDING_BUCKET_NAME')
+RECORDING_BUCKET_URL = os.getenv('RECORDING_BUCKET_URL')
 
 class DictWithMissing(dict):
     def __missing__(self, key):
         return ''
 
 
 def load_file(file_path, is_json=False):
@@ -125,14 +128,29 @@
             response = await s3_client.get_object(Bucket=bucket_name, Key=file_key)
         except (BotoCoreError, ClientError) as error:
             logger.error(error)
         else:
             file_content = await response['Body'].read()
             return file_content
 
+async def delete_s3_file_by_prefix(bucket_name,file_key):
+    session = AioSession()
+    async with AsyncExitStack() as exit_stack:
+        s3_client = await exit_stack.enter_async_context(session.create_client('s3'))
+        try:
+            paginator = s3_client.get_paginator('list_objects')
+            async for result in paginator.paginate(Bucket=bucket_name, Prefix=file_key):
+                tasks = []
+                for file in result.get('Contents', []):
+                    tasks.append(s3_client.delete_object(Bucket=bucket_name, Key=file['Key']))
+                await asyncio.gather(*tasks)
+            return True
+        except (BotoCoreError, ClientError) as error:
+            logger.error(error)
+            return error
 
 async def store_file(bucket_name=None, file_key=None, file_data=None, content_type="json", local=False, preprocess_dir=None):
     if not local:
         session = AioSession()
 
         async with AsyncExitStack() as exit_stack:
             s3_client = await exit_stack.enter_async_context(session.create_client('s3'))
@@ -159,24 +177,31 @@
                 f.write(data)
         elif content_type in ["mp3", "wav", "pcm", "csv"]:
             with open(f"{dir_name}/{file_key}", 'w') as f:
                 data = file_data
                 f.write(data)
 
 
-async def get_raw_audio_bytes_from_base64(agent_name, b64_string, audio_format='mp3', assistant_id=None, local = False):
+async def get_raw_audio_bytes(filename, agent_name = None, audio_format='mp3', assistant_id=None, local = False, is_location = False):
     # we are already storing pcm formatted audio in the filler config. No need to encode/decode them further
     audio_data = None
     if local:
-        file_name = f"{PREPROCESS_DIR}/{agent_name}/{audio_format}/{b64_string}.{audio_format}"
+        if not is_location:
+            file_name = f"{PREPROCESS_DIR}/{agent_name}/{audio_format}/{filename}.{audio_format}"
+        else:
+            file_name = filename
         with open(file_name, 'rb') as file:
             # Read the entire file content into a variable
             audio_data = file.read()
     else:
-        object_key = f"{assistant_id}/audio/{b64_string}.{audio_format}"
+        if not is_location:
+            object_key = f"{assistant_id}/audio/{filename}.{audio_format}"
+        else:
+            object_key = filename
+            
         logger.info(f"Reading {object_key}")
         audio_data = await get_s3_file(BUCKET_NAME, object_key)
 
     return audio_data
 
 
 def get_md5_hash(text):
@@ -345,14 +370,34 @@
         audio_segment = AudioSegment.from_file(file_like_object, format="wav")
         combined += audio_segment
 
     buffer = io.BytesIO()
     combined.export(buffer, format="wav")
     return buffer.getvalue()
 
+def calculate_audio_duration(size_bytes, sampling_rate, bit_depth = 16, channels = 1):
+    bytes_per_sample = (bit_depth / 8) * channels
+    total_samples = size_bytes / bytes_per_sample
+    duration_seconds = total_samples / sampling_rate
+    return duration_seconds
+
+
+def create_empty_wav_file(duration_seconds, sampling_rate = 24000):
+    total_frames = duration_seconds * sampling_rate
+    wav_io = io.BytesIO()
+    with wave.open(wav_io, 'wb') as wav_file:
+        wav_file.setnchannels(1)
+        wav_file.setsampwidth(2) 
+        wav_file.setframerate(sampling_rate)
+        wav_file.setnframes(total_frames)
+        wav_file.writeframes(b'\x00' * total_frames * 2) 
+    wav_io.seek(0)
+    return wav_io
+
+
 
 '''
 Message type
 1. Component
 2. Request/Response
 3. conversation_leg_id
 4. data
@@ -382,7 +427,75 @@
     file_exists = os.path.exists(log_file_path)
     
     async with aiofiles.open(log_file_path, mode='a') as log_file:
         if not file_exists:
             await log_file.write(header+log_string)
         else:    
             await log_file.write(log_string)
+
+async def save_audio_file_to_s3(conversation_recording, sampling_rate = 24000, assistant_id = None, run_id = None):
+    last_frame_end_time = conversation_recording['output'][0]['start_time']
+    logger.info(f"LENGTH OF OUTPUT AUDIO {len(conversation_recording['output'])}")
+    initial_gap = (last_frame_end_time - conversation_recording["metadata"]["started"] ) *1000
+    logger.info(f"Initial gap {initial_gap}")
+    combined_audio = AudioSegment.silent(duration=initial_gap, frame_rate=sampling_rate)
+    for i, frame in enumerate(conversation_recording['output']):
+        frame_start_time =  frame['start_time']
+        logger.info(f"Processing frame {i}, fram start time = {last_frame_end_time}, frame start time= {frame_start_time}")
+        if last_frame_end_time < frame_start_time:
+            gap_duration_samples = frame_start_time - last_frame_end_time
+            silence = AudioSegment.silent(duration=gap_duration_samples*1000, frame_rate=sampling_rate)
+            combined_audio += silence
+        last_frame_end_time = frame_start_time + frame['duration']
+        frame_as = AudioSegment.from_file(io.BytesIO(frame['data']), format = "wav")
+        combined_audio +=frame_as
+
+    webm_segment = AudioSegment.from_file(io.BytesIO(conversation_recording['input']["data"]))
+    wav_bytes = io.BytesIO()
+    webm_segment.export(wav_bytes, format="wav")
+    wav_bytes.seek(0)  # Reset the pointer to the start
+    waveform, sample_rate = torchaudio.load(wav_bytes)
+    resampler = torchaudio.transforms.Resample(orig_freq=sample_rate, new_freq=sampling_rate)
+    downsampled_waveform = resampler(waveform)
+    torchaudio_wavio = io.BytesIO()
+    torchaudio.save(torchaudio_wavio, downsampled_waveform, sampling_rate, format= "wav")
+    audio_segment_bytes = io.BytesIO()
+    combined_audio.export(audio_segment_bytes, format="wav")
+    audio_segment_bytes.seek(0)
+    waveform_audio_segment, sample_rate = torchaudio.load(audio_segment_bytes)
+
+    if waveform_audio_segment.shape[0] > 1:
+        waveform_audio_segment = waveform_audio_segment[:1, :]
+
+    # Adjust shapes to be [1, N] if not already
+    downsampled_waveform = downsampled_waveform.unsqueeze(0) if downsampled_waveform.dim() == 1 else downsampled_waveform
+    waveform_audio_segment = waveform_audio_segment.unsqueeze(0) if waveform_audio_segment.dim() == 1 else waveform_audio_segment
+
+    # Ensure both waveforms have the same length
+    max_length = max(downsampled_waveform.size(1), waveform_audio_segment.size(1))
+    downsampled_waveform_padded = torch.nn.functional.pad(downsampled_waveform, (0, max_length - downsampled_waveform.size(1)))
+    waveform_audio_segment_padded = torch.nn.functional.pad(waveform_audio_segment, (0, max_length - waveform_audio_segment.size(1)))
+    stereo_waveform = torch.cat((downsampled_waveform_padded, waveform_audio_segment_padded), 0)
+
+    # Verify the stereo waveform shape is [2, M]
+    assert stereo_waveform.shape[0] == 2, "Stereo waveform should have 2 channels."
+    key = f'{assistant_id + run_id.split("#")[1]}.wav'
+
+    audio_buffer = io.BytesIO()
+    torchaudio.save(audio_buffer, stereo_waveform, 24000, format="wav")
+    audio_buffer.seek(0)
+
+    logger.info(f"Storing in {RECORDING_BUCKET_URL}{key}")
+    await store_file(bucket_name=RECORDING_BUCKET_NAME, file_key=key, file_data=audio_buffer, content_type="wav")
+    
+    return f'{RECORDING_BUCKET_URL}{key}'
+
+def list_number_of_wav_files_in_directory(directory):
+    count = 0
+    for filename in os.listdir(directory):
+        if filename.endswith(".mp3") or filename.endswith(".wav") or filename.endswith(".ogg"):
+            count += 1
+    return count
+
+def get_file_names_in_directory(directory):
+    return os.listdir(directory)
+
```

### Comparing `bolna-0.7.5/bolna/helpers/vad.py` & `bolna-0.7.7/bolna/helpers/vad.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.5/bolna/input_handlers/default.py` & `bolna-0.7.7/bolna/input_handlers/default.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import asyncio
 import base64
+import time
 from dotenv import load_dotenv
 from bolna.helpers.logger_config import configure_logger
 from bolna.helpers.utils import create_ws_data_packet
 
 logger = configure_logger(__name__)
 load_dotenv()
 
 
 class DefaultInputHandler:
-    def __init__(self, queues=None, websocket=None, input_types=None, mark_set = None, queue = None, connected_through_dashboard=False):
+    def __init__(self, queues=None, websocket=None, input_types=None, mark_set = None, queue = None, connected_through_dashboard=False, conversation_recording = None):
         self.queues = queues
         self.websocket = websocket
         self.input_types = input_types
         self.websocket_listen_task = None
         self.running = True
         self.connected_through_dashboard = connected_through_dashboard
         self.queue = queue
-
+        self.conversation_recording = conversation_recording
     async def stop_handler(self):
         self.running = False
         try:
             if not self.queue:
                 await self.websocket.close()
         except Exception as e:
             logger.error(f"Error closing WebSocket: {e}")
@@ -31,14 +32,18 @@
         ws_data_packet = create_ws_data_packet(
             data=data,
             meta_info={
                 'io': 'default',
                 'type': 'audio',
                 'sequence': self.input_types['audio']
             })
+        if self.conversation_recording:
+            if self.conversation_recording["metadata"]["started"] ==0:
+                self.conversation_recording["metadata"]["started"] = time.time()
+            self.conversation_recording['input']['data'] += data
 
         self.queues['transcriber'].put_nowait(ws_data_packet)
     
     def __process_text(self, text):
         logger.info(f"Sequences {self.input_types}")
         ws_data_packet = create_ws_data_packet(
             data=text,
@@ -55,15 +60,15 @@
     async def _listen(self):
         try:
             while self.running:
                 if self.queue is not None:
                     logger.info(f"self.queue is not None and hence listening to the queue")
                     request = await self.queue.get()
                 else:
-                    request = await self.websocket.receive_json()
+                    request = await self.websocket.receive_json()                    
                 await self.process_message(request)
         except Exception as e:
             # Send EOS message to transcriber to shut the connection
             ws_data_packet = create_ws_data_packet(
                 data=None,
                 meta_info={
                     'io': 'default',
```

### Comparing `bolna-0.7.5/bolna/input_handlers/telephony.py` & `bolna-0.7.7/bolna/input_handlers/telephony.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.5/bolna/input_handlers/telephony_providers/exotel.py` & `bolna-0.7.7/bolna/input_handlers/telephony_providers/exotel.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.5/bolna/input_handlers/telephony_providers/twilio.py` & `bolna-0.7.7/bolna/input_handlers/telephony_providers/twilio.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.5/bolna/llms/litellm.py` & `bolna-0.7.7/bolna/llms/litellm.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,27 +7,29 @@
 import time
 
 logger = configure_logger(__name__)
 load_dotenv()
 
 
 class LiteLLM(BaseLLM):
-    def __init__(self, streaming_model, max_tokens=30, buffer_size=40,
-                 classification_model=None, temperature=0.0, **kwargs):
+    def __init__(self, model, max_tokens=30, buffer_size=40,
+                 temperature=0.0, **kwargs):
         super().__init__(max_tokens, buffer_size)
-        self.model = streaming_model
+        self.model = model
         self.started_streaming = False
         self.model_args = {"max_tokens": max_tokens, "temperature": temperature, "model": self.model}
-
         self.api_key = kwargs.get("llm_key", os.getenv('LITELLM_MODEL_API_KEY'))
         self.api_base = kwargs.get("base_url", os.getenv('LITELLM_MODEL_API_BASE'))
+        self.api_version = kwargs.get("api_version", os.getenv('LITELLM_MODEL_API_VERSION'))
         if self.api_key:
             self.model_args["api_key"] = self.api_key
         if self.api_base:
             self.model_args["api_base"] = self.api_base
+        if self.api_version:
+            self.model_args["api_version"] = self.api_version
 
         if "top_k" in kwargs:
             self.model_args["top_k"] = kwargs["top_k"]
         if "top_p" in kwargs:
             self.model_args["top_p"] = kwargs["top_p"]
         if "stop" in kwargs:
             self.model_args["stop"] = kwargs["stop"]
@@ -36,16 +38,17 @@
         if "frequency_penalty" in kwargs:
             self.model_args["frequency_penalty"] = kwargs["frequency_penalty"]
 
         if len(kwargs) != 0:
             if "base_url" in kwargs:
                 self.model_args["api_base"] = kwargs["base_url"]
             if "llm_key" in kwargs:
-                self.model_args["llm_key"] = kwargs["llm_key"]
-        self.classification_model = classification_model
+                self.model_args["api_key"] = kwargs["llm_key"]
+            if "api_version" in kwargs:
+                self.model_args["api_version"] = kwargs["api_version"]
 
     async def generate_stream(self, messages, synthesize=True):
         answer, buffer = "", ""
         model_args = self.model_args.copy()
         model_args["messages"] = messages
         model_args["stream"] = True
 
@@ -69,18 +72,18 @@
             if buffer != "":
                 yield buffer, True
         else:
             yield answer, True
         self.started_streaming = False
         logger.info(f"Time to generate response {time.time() - start_time}")
 
-    async def generate(self, messages, classification_task=False, stream=False, synthesize=True, request_json=False):
+    async def generate(self, messages, stream=False, request_json=False):
         text = ""
         model_args = self.model_args.copy()
-        model_args["model"] = self.classification_model if classification_task is True else self.model
+        model_args["model"] = self.model
         model_args["messages"] = messages
         model_args["stream"] = stream
 
         if request_json is True:
             model_args['response_format'] = {
                 "type": "json_object",
                 "schema": json_to_pydantic_schema('{"classification_label": "classification label goes here"}')
```

### Comparing `bolna-0.7.5/bolna/llms/openai_llm.py` & `bolna-0.7.7/bolna/llms/openai_llm.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 from bolna.helpers.logger_config import configure_logger
 
 logger = configure_logger(__name__)
 load_dotenv()
 
 
 class OpenAiLLM(BaseLLM):
-    def __init__(self, max_tokens=100, buffer_size=40, streaming_model="gpt-3.5-turbo-16k",
-                 classification_model="gpt-3.5-turbo-1106", temperature= 0.1, **kwargs):
+    def __init__(self, max_tokens=100, buffer_size=40, model="gpt-3.5-turbo-16k", temperature= 0.1, **kwargs):
         super().__init__(max_tokens, buffer_size)
-        self.model = streaming_model
+        self.model = model
         self.started_streaming = False
         logger.info(f"Initializing OpenAI LLM with model: {self.model} and maxc tokens {max_tokens}")
         self.max_tokens = max_tokens
-        self.classification_model = classification_model
         self.temperature = temperature
         self.vllm_model = "vllm" in self.model
         self.model_args = { "max_tokens": self.max_tokens, "temperature": self.temperature, "model": self.model}
 
         if self.vllm_model:
-            base_url = kwargs.get("base_url", os.getenv("VLLM_SERVER_BASE_URL"))
+            base_url = kwargs.get("base_url", None)
+            if base_url is None:
+                raise Exception("Cannot run a custom LLM without base URL")
             api_key=kwargs.get('llm_key', None)
-            if len(api_key) > 0:
+            if api_key is not None and len(api_key) > 0:
                 api_key = api_key
             else:
                 api_key = "EMPTY"
             self.async_client = AsyncOpenAI( base_url=base_url, api_key= api_key)
             self.model = self.model[5:]
             self.model_args["model"] = self.model
             if "top_k" in kwargs:
@@ -48,22 +48,21 @@
         if "stop" in kwargs:
             self.model_args["stop"] = kwargs["stop"]        
         if "presence_penalty" in kwargs:
             self.model_args["presence_penalty"] = kwargs["presence_penalty"]
         if  "frequency_penalty" in kwargs:
             self.model_args["frequency_penalty"] = kwargs["frequency_penalty"]
 
-    async def generate_stream(self, messages, classification_task=False, synthesize=True, request_json=False):
+    async def generate_stream(self, messages, synthesize=True, request_json=False):
         if len(messages) == 0:
             raise Exception("No messages provided")
         
         response_format = self.get_response_format(request_json)
 
         answer, buffer = "", ""
-        model = self.classification_model if classification_task is True else self.model
         logger.info(f"request to open ai {messages} max tokens {self.max_tokens} ")
         model_args = self.model_args
         model_args["response_format"] = response_format
         model_args["messages"] = messages
         model_args["stream"] = True
         model_args["stop"] = ["User:"]
         async for chunk in await self.async_client.chat.completions.create(**model_args):
@@ -82,22 +81,21 @@
 
         if synthesize: # This is used only in streaming sense 
             yield buffer, True
         else:
             yield answer, True
         self.started_streaming = False
 
-    async def generate(self, messages, classification_task=False, stream=False, synthesize=True, request_json=False):
+    async def generate(self, messages, request_json=False):
         response_format = self.get_response_format(request_json)
         logger.info(f"request to open ai {messages}")
-        model = self.classification_model if classification_task is True else self.model
 
-        completion = await self.async_client.chat.completions.create(model=model, temperature=0.0, messages=messages,
+        completion = await self.async_client.chat.completions.create(model=self.model, temperature=0.0, messages=messages,
                                                                      stream=False, response_format=response_format)
         res = completion.choices[0].message.content
         return res
 
     def get_response_format(self, is_json_format: bool):
-        if is_json_format and self.classification_model in ('gpt-4-1106-preview', 'gpt-3.5-turbo-1106'):
+        if is_json_format and self.model in ('gpt-4-1106-preview', 'gpt-3.5-turbo-1106'):
             return {"type": "json_object"}
         else:
             return {"type": "text"}
```

### Comparing `bolna-0.7.5/bolna/models.py` & `bolna-0.7.7/bolna/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,45 +9,45 @@
         raise ValidationError(f"Invalid provider. Supported values: {', '.join(allowed_values)}")
     return value
 
 
 class PollyConfig(BaseModel):
     voice: str
     engine: str
-    sampling_rate: Optional[str] = "16000"
     language: str
+    # volume: Optional[str] = '0dB'
+    # rate: Optional[str] = '100%'
 
 
 class XTTSConfig(BaseModel):
     voice: str
     language: str
-    sampling_rate: Optional[str] ="24000"
 
 
 class ElevenLabsConfig(BaseModel):
     voice: str
     voice_id: str
     model: str
-    sampling_rate: Optional[str] = "16000"
+    temperature: Optional[float] = 0.5
+    similarity_boost: Optional[float] = 0.5
 
 
 class OpenAIConfig(BaseModel):
     voice: str
     model: str
-    sampling_rate: Optional[str] ="24000"
 
 
 class FourieConfig(BaseModel):
     voice_id: str
     gender: str
     voice: str
 
 
 class DeepgramConfig(BaseModel):
-    voice_id: str
+    voice: str
 
 
 class Transcriber(BaseModel):
     model: str
     language: Optional[str] = None
     stream: bool = False
     sampling_rate: Optional[int] = 16000
@@ -80,30 +80,42 @@
     provider: str
     format: str
 
     @validator("provider")
     def validate_provider(cls, value):
         return validate_attribute(value, ["twilio", "default", "database", "exotel"])
 
+# Can be used to route across multiple prompts as well
+class Route(BaseModel):
+    route_name: str
+    utterances: List[str]
+    response: Union[List[str], str] #If length of responses is less than utterances, a random sentence will be used as a response and if it's equal, respective index will be used to use it as FAQs caching
+    score_threshold: Optional[float] = 0.85 # this is the required threshold for cosine similarity 
+
+# Routes can be used for FAQs caching, prompt routing, guard rails, agent assist function calling
+class Routes(BaseModel):
+    embedding_model: Optional[str] = "Snowflake/snowflake-arctic-embed-l"
+    routes: List[Route]
 
 class LLM(BaseModel):
-    streaming_model: Optional[str] = "gpt-3.5-turbo-16k"
-    classification_model: Optional[str] = "gpt-4"
+    model: Optional[str] = "gpt-3.5-turbo-16k"
     max_tokens: Optional[int] = 100
     agent_flow_type: Optional[str] = "streaming"
-    use_fallback: Optional[bool] = False
     family: Optional[str] = "openai"
     temperature: Optional[float] = 0.1
     request_json: Optional[bool] = False
     stop: Optional[List[str]] = None
     top_k: Optional[int] = 0
     top_p: Optional[float] = 0.9
     min_p: Optional[float] = 0.1
-    frequency_penalty: Optional[float] = 0.0  
+    frequency_penalty: Optional[float] = 0.0
     presence_penalty: Optional[float] = 0.0
+    provider: Optional[str] = "openai"
+    base_url: Optional[str] = None
+    routes: Optional[Routes] = None
 
 class MessagingModel(BaseModel):
     provider: str
     template: str
 
 
 # Need to redefine it
```

### Comparing `bolna-0.7.5/bolna/output_handlers/default.py` & `bolna-0.7.7/bolna/output_handlers/default.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.5/bolna/output_handlers/telephony.py` & `bolna-0.7.7/bolna/output_handlers/telephony.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.5/bolna/output_handlers/telephony_providers/exotel.py` & `bolna-0.7.7/bolna/output_handlers/telephony_providers/exotel.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.5/bolna/output_handlers/telephony_providers/twilio.py` & `bolna-0.7.7/bolna/output_handlers/telephony_providers/twilio.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.5/bolna/prompts.py` & `bolna-0.7.7/bolna/prompts.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 SUMMARIZATION_PROMPT = """
 Given this transcript from the communication between user and an agent your task is to summarize the conversation.
 """
 
 completion_json_format = {"answer": "A simple Yes or No based on if you should cut the phone or not"}
 
 CHECK_FOR_COMPLETION_PROMPT = """
-You are an helpful AI assistant that's having a conversation with customer. 
+You are an helpful AI assistant that's having a conversation with customer on a phone call. 
 Based on the given transcript, should you cut the call?\n\n 
 RULES: 
-1. If user is not interested in talking, or is annoying or something, we need to cut the phone. 
-2. You are also provided with original prompt to make your decision if we need to cut the phone or not.  
+1. If user is not interested in talking, or is annoyed or is angry we might need to cut the phone. 
+2. You are also provided with original prompt use the content of original prompt to make your decision. For example if the purpose of the phone call is done and we have all the required content we need to cut the call.
 
 ### JSON Structure
 {}
 
 """.format(completion_json_format)
 
 EXTRACTION_PROMPT_GENERATION_PROMPT = """
```

### Comparing `bolna-0.7.5/bolna/providers.py` & `bolna-0.7.7/bolna/providers.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,23 +12,27 @@
     'fourie': FourieSynthesizer,
     'deepgram': DeepgramSynthesizer
 }
 SUPPORTED_TRANSCRIBER_MODELS = {
     'deepgram': DeepgramTranscriber,
     'whisper': DeepgramTranscriber #Seperate out a transcriber for https://github.com/bolna-ai/streaming-transcriber-server or build a deepgram compatible proxy
 }
-SUPPORTED_LLM_MODELS = {
+
+SUPPORTED_LLM_PROVIDERS = {
     'openai': OpenAiLLM,
     'cohere': LiteLLM,
     'ollama': LiteLLM,
-    'mistral': LiteLLM,
-    'llama': LiteLLM,
-    'zephyr': LiteLLM,
+    'deepinfra': LiteLLM,
+    'together': LiteLLM,
+    'fireworks': LiteLLM,
+    'azure-openai': LiteLLM,
     'perplexity': LiteLLM,
-    'vllm': OpenAiLLM
+    'vllm': OpenAiLLM,
+    'anyscale': LiteLLM,
+    'custom': OpenAiLLM
 }
 SUPPORTED_INPUT_HANDLERS = {
     'default': DefaultInputHandler,
     'twilio': TwilioInputHandler,
     'exotel': ExotelInputHandler
 }
 SUPPORTED_INPUT_TELEPHONY_HANDLERS = {
```

### Comparing `bolna-0.7.5/bolna/synthesizer/base_synthesizer.py` & `bolna-0.7.7/bolna/synthesizer/base_synthesizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import io
 import torchaudio
 from bolna.helpers.logger_config import configure_logger
 import asyncio
+
 logger = configure_logger(__name__)
 
 
 class BaseSynthesizer:
-    def __init__(self, stream=True, buffer_size=40):
+    def __init__(self, stream=True, buffer_size=40, event_loop= None):
         self.stream = stream
         self.buffer_size = buffer_size
         self.internal_queue = asyncio.Queue()
 
     def clear_internal_queue(self):
         logger.info(f"Clearing out internal queue")
         self.internal_queue = asyncio.Queue()
@@ -29,8 +30,8 @@
         waveform, orig_sample_rate = torchaudio.load(audio_buffer)
         resampler = torchaudio.transforms.Resample(orig_sample_rate, 8000)
         audio_waveform = resampler(waveform)
         audio_buffer = io.BytesIO()
         torchaudio.save(audio_buffer, audio_waveform, 8000, format="wav")
         audio_buffer.seek(0)
         audio_data = audio_buffer.read()
-        return audio_data
+        return audio_data
```

### Comparing `bolna-0.7.5/bolna/synthesizer/deepgram_synthesizer.py` & `bolna-0.7.7/bolna/synthesizer/deepgram_synthesizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 from dotenv import load_dotenv
 from bolna.helpers.logger_config import configure_logger
 from bolna.helpers.utils import create_ws_data_packet
 from .base_synthesizer import BaseSynthesizer
 
 logger = configure_logger(__name__)
 load_dotenv()
-DEEPGRAM_TTS_URL = "https://api.deepgram.com/v1/speak"
+DEEPGRAM_HOST = os.getenv('DEEPGRAM_HOST', 'api.deepgram.com')
+DEEPGRAM_TTS_URL = "https://{}/v1/speak".format(DEEPGRAM_HOST)
 
 
 class DeepgramSynthesizer(BaseSynthesizer):
-    def __init__(self, voice, language, audio_format="pcm", sampling_rate="8000", stream=False, buffer_size=400,
+    def __init__(self, voice, audio_format="pcm", sampling_rate="8000", stream=False, buffer_size=400,
                  **kwargs):
         super().__init__(stream, buffer_size)
         self.format = "linear16" if audio_format == "pcm" else audio_format
         self.voice = voice
-        self.language = language
         self.sample_rate = str(sampling_rate)
         self.first_chunk_generated = False
         self.api_key = kwargs.get("transcriber_key", os.getenv('DEEPGRAM_AUTH_TOKEN'))
 
     async def __generate_http(self, text):
         headers = {
             "Authorization": "Token {}".format(self.api_key),
```

### Comparing `bolna-0.7.5/bolna/synthesizer/elevenlabs_synthesizer.py` & `bolna-0.7.7/bolna/synthesizer/elevenlabs_synthesizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,37 +7,44 @@
 import os
 import traceback
 from collections import deque
 from .base_synthesizer import BaseSynthesizer
 from bolna.helpers.logger_config import configure_logger
 from bolna.helpers.utils import convert_audio_to_wav, create_ws_data_packet, pcm_to_wav_bytes, resample
 
+
 logger = configure_logger(__name__)
 
 
 class ElevenlabsSynthesizer(BaseSynthesizer):
     def __init__(self, voice, voice_id, model="eleven_multilingual_v1", audio_format="mp3", sampling_rate="16000",
-                 stream=False, buffer_size=400, synthesier_key=None, **kwargs):
+                 stream=False, buffer_size=400, temperature = 0.5, similarity_boost = 0.5, synthesier_key=None, 
+                 cache=None, **kwargs):
         super().__init__(stream)
         self.api_key = os.environ["ELEVENLABS_API_KEY"] if synthesier_key is None else synthesier_key
         self.voice = voice_id
         self.use_turbo = kwargs.get("use_turbo", False)
         self.model = "eleven_turbo_v2" if self.use_turbo else "eleven_multilingual_v2"
-        self.stream = stream  # Issue with elevenlabs streaming that we need to always send the text quickly
+        logger.info(f"Using turbo or not {self.model}")
+        self.stream = False  # Issue with elevenlabs streaming that we need to always send the text quickly
         self.websocket_connection = None
         self.connection_open = False
         self.sampling_rate = sampling_rate
         self.audio_format = "mp3"
         self.use_mulaw = kwargs.get("use_mulaw", False)
         self.ws_url = f"wss://api.elevenlabs.io/v1/text-to-speech/{self.voice}/stream-input?model_id={self.model}&optimize_streaming_latency=2&output_format={self.get_format(self.audio_format, self.sampling_rate)}"
         self.api_url = f"https://api.elevenlabs.io/v1/text-to-speech/{self.voice}?optimize_streaming_latency=2&output_format="
         self.first_chunk_generated = False
         self.last_text_sent = False
         self.text_queue = deque()
         self.meta_info = None
+        self.temperature = temperature
+        self.similarity_boost = similarity_boost
+        self.cache = cache
+        self.synthesized_characters = 0
 
     # Ensuring we only do wav output for now
     def get_format(self, format, sampling_rate):
         # Eleven labs only allow mp3_44100_64, mp3_44100_96, mp3_44100_128, mp3_44100_192, pcm_16000, pcm_22050,
         # pcm_24000, ulaw_8000
         if self.use_mulaw:
             return "ulaw_8000"
@@ -51,16 +58,16 @@
             await self.open_connection()
 
         if not self.connection_open:
             logger.info("Connecting to elevenlabs websocket...")
             bos_message = {
                 "text": " ",
                 "voice_settings": {
-                    "stability": 0.5,
-                    "similarity_boost": 0.5
+                    "stability": self.temperature,
+                    "similarity_boost": self.similarity_boost
                 },
                 "xi_api_key": self.api_key,
             }
             await self.websocket_connection.send(json.dumps(bos_message))
             self.connection_open = True
 
         if text != "":
@@ -124,22 +131,25 @@
     async def __generate_http(self, text, format=None):
         payload = None
         logger.info(f"text {text}")
         payload = {
             "text": text,
             "model_id": self.model,
             "voice_settings": {
-                "stability": 0.5,
+                "stability": 0.4,
                 "similarity_boost": 0.5,
                 "optimize_streaming_latency": 3
             }
         }
         response = await self.__send_payload(payload, format=format)
         return response
 
+    def get_synthesized_characters(self):
+        return self.synthesized_characters
+
     # Currently we are only supporting wav output but soon we will incorporate conver
     async def generate(self):
         try:
             if self.stream:
                 async for message in self.receiver():
                     logger.info(f"Received message from server")
 
@@ -163,39 +173,48 @@
                     if self.last_text_sent:
                         # Reset the last_text_sent and first_chunk converted to reset synth latency
                         self.first_chunk_generated = False
                         self.last_text_sent = True
 
                     if message == b'\x00':
                         logger.info("received null byte and hence end of stream")
-                        meta_info["end_of_synthesizer_stream"] = True
-                        yield create_ws_data_packet(resample(message, int(self.sampling_rate)), meta_info)
+                        self.meta_info["end_of_synthesizer_stream"] = True
+                        yield create_ws_data_packet(resample(message, int(self.sampling_rate)), self.meta_info)
                         self.first_chunk_generated = False
 
             else:
                 while True:
                     message = await self.internal_queue.get()
                     logger.info(f"Generating TTS response for message: {message}")
                     meta_info, text = message.get("meta_info"), message.get("data")
-                    audio = await self.__generate_http(text)
-
+                    if self.cache.get(text):
+                        logger.info(f"Cache hit and hence returning quickly {text}")
+                        message = self.cache.get(text)
+                    else:
+                        c = len(text)
+                        self.synthesized_characters += c
+                        logger.info(f"Not a cache hit {list(self.cache.data_dict)} and hence increasing characters by {c}")
+                        audio = await self.__generate_http(text)
+                        self.cache.set(text, audio)
+                        
                     meta_info['text'] = text
                     if not self.first_chunk_generated:
                         meta_info["is_first_chunk"] = True
                         self.first_chunk_generated = True
 
                     if "end_of_llm_stream" in meta_info and meta_info["end_of_llm_stream"]:
                         meta_info["end_of_synthesizer_stream"] = True
                         self.first_chunk_generated = False
 
                     if self.use_mulaw:
                         meta_info['format'] = "mulaw"
                     else:
                         meta_info['format'] = "wav"
                         wav_bytes = convert_audio_to_wav(audio, source_format="mp3")
+                        logger.info(f"self.sampling_rate {self.sampling_rate}")
                         audio = resample(wav_bytes, int(self.sampling_rate), format="wav")
                     yield create_ws_data_packet(audio, meta_info)
 
         except Exception as e:
             traceback.print_exc()
             logger.error(f"Error in eleven labs generate {e}")
```

### Comparing `bolna-0.7.5/bolna/synthesizer/fourie_synthesizer.py` & `bolna-0.7.7/bolna/synthesizer/fourie_synthesizer.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.5/bolna/synthesizer/openai_synthesizer.py` & `bolna-0.7.7/bolna/synthesizer/openai_synthesizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from collections import deque
 import os
 from dotenv import load_dotenv
-import audioop
 from bolna.helpers.logger_config import configure_logger
 from bolna.helpers.utils import convert_audio_to_wav, create_ws_data_packet, pcm_to_wav_bytes, resample
 from .base_synthesizer import BaseSynthesizer
 from openai import AsyncOpenAI
 import io
 
 logger = configure_logger(__name__)
@@ -19,15 +18,16 @@
         self.sample_rate = sampling_rate
         api_key = kwargs.get("synthesizer_key", os.getenv("OPENAI_API_KEY"))
         self.async_client = AsyncOpenAI(api_key= api_key)
         self.model = model
         self.first_chunk_generated = False 
         self.text_queue = deque()
         self.stream = False
-        logger.info(f"self sampling rate {self.sample_rate}")
+        if type(self.sample_rate) is str:
+            self.sample_rate = int(self.sample_rate)
         
     # Ensuring we can only do wav outputs becasue mulaw conversion for others messes up twilio
     def get_format(self, format):
         return "mp3"
     
     async def synthesize(self, text):
         #This is used for one off synthesis mainly for use cases like voice lab and IVR
@@ -84,15 +84,14 @@
                     if not self.first_chunk_generated:
                         meta_info["is_first_chunk"] = True
                         self.first_chunk_generated = True
                     
                     if "end_of_llm_stream" in meta_info and meta_info["end_of_llm_stream"]:
                         meta_info["end_of_synthesizer_stream"] = True
                         self.first_chunk_generated = False 
-                    
                     yield create_ws_data_packet(resample(convert_audio_to_wav(audio, 'mp3'), self.sample_rate, format="wav"), meta_info)
 
         except Exception as e:
                 logger.error(f"Error in openai generate {e}")
 
     async def open_connection(self):
         pass
```

### Comparing `bolna-0.7.5/bolna/synthesizer/polly_synthesizer.py` & `bolna-0.7.7/bolna/synthesizer/polly_synthesizer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,66 @@
-import asyncio
 from dotenv import load_dotenv
 from botocore.exceptions import BotoCoreError, ClientError
 from aiobotocore.session import AioSession
 from contextlib import AsyncExitStack
 import audioop
 from bolna.helpers.logger_config import configure_logger
 from bolna.helpers.utils import convert_audio_to_wav, create_ws_data_packet, pcm_to_wav_bytes, resample
 from .base_synthesizer import BaseSynthesizer
 
 logger = configure_logger(__name__)
 load_dotenv()
 
 
 class PollySynthesizer(BaseSynthesizer):
-    def __init__(self, voice, language, audio_format="pcm", sampling_rate="8000", stream=False, engine="neural",
-                 buffer_size=400, **kwargs):
+    def __init__(self, voice, language, audio_format="pcm", sampling_rate=8000, stream=False, engine="neural",
+                 buffer_size=400, speaking_rate = "100%", volume = "0dB", cache= None, **kwargs):
         super().__init__(stream, buffer_size)
         self.engine = engine
         self.format = self.get_format(audio_format.lower())
         self.voice = voice
         self.language = language
         self.sample_rate = str(sampling_rate)
         self.client = None
         self.first_chunk_generated = False
-
+        self.speaking_rate = speaking_rate
+        self.volume = volume
+        self.synthesized_characters = 0
+        self.cache = cache
+
+    def get_synthesized_characters(self):
+        return self.synthesized_characters
+    
     def get_format(self, audio_format):
         if audio_format == "pcm":
             return "pcm"
         else:
             return "mp3"
 
     @staticmethod
     async def create_client(service: str, session: AioSession, exit_stack: AsyncExitStack):
         # creates AWS session from system environment credentials & config
         return await exit_stack.enter_async_context(session.create_client(service))
 
     async def __generate_http(self, text):
+        self.synthesized_characters += len(text)
         session = AioSession()
         async with AsyncExitStack() as exit_stack:
             polly = await self.create_client("polly", session, exit_stack)
             logger.info(f"Generating TTS response for text: {text}, SampleRate {self.sample_rate} format {self.format}")
+            # input = f"""
+            # <speak> 
+            #     <amazon:auto-breaths volume= "x-loud" frequency="x-high" duration="x-long"> 
+            #         <prosody volume="{self.volume}" rate="{self.speaking_rate}"> {text} 
+            #         </prosody> 
+            #     </amazon:auto-breaths>
+            # </speak>
+            # """
+
+            logger.info(f"Sending text {input}")
             try:
                 response = await polly.synthesize_speech(
                     Engine=self.engine,
                     Text=text,
                     OutputFormat=self.format,
                     VoiceId=self.voice,
                     LanguageCode=self.language,
@@ -65,14 +82,19 @@
 
     async def generate(self):
         while True:
             logger.info("Generating TTS response")
             message = await self.internal_queue.get()
             logger.info(f"Generating TTS response for message: {message}")
             meta_info, text = message.get("meta_info"), message.get("data")
+            if self.cache.get(text):
+                logger.info(f"Cache hit and hence returning quickly {text}")
+                message = self.cache[text]
+            else:
+                logger.info(f"Not a cache hit {list(self.cache.data_dict)}")
             message = await self.__generate_http(text)
             if self.format == "mp3":
                 message = convert_audio_to_wav(message, source_format="mp3")
             if not self.first_chunk_generated:
                 meta_info["is_first_chunk"] = True
                 self.first_chunk_generated = True
             else:
```

### Comparing `bolna-0.7.5/bolna/synthesizer/xtts_synthesizer.py` & `bolna-0.7.7/bolna/synthesizer/xtts_synthesizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-import asyncio
 from collections import deque
 import aiohttp
 import websockets
 from websockets.exceptions import ConnectionClosed
 import json
 import os
 import audioop
 from dotenv import load_dotenv
 from .base_synthesizer import BaseSynthesizer
 from bolna.helpers.logger_config import configure_logger
 from bolna.helpers.utils import create_ws_data_packet
+
+
 logger = configure_logger(__name__)
 load_dotenv()
 
 
 
 class XTTSSynthesizer(BaseSynthesizer):
     def __init__(self, audio_format = "wav", stream = False, sampling_rate="24000", buffer_size=400, language = "en", voice = "rohan", **kwargs):
```

### Comparing `bolna-0.7.5/bolna/transcriber/base_transcriber.py` & `bolna-0.7.7/bolna/transcriber/base_transcriber.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import json
 import time
 import uuid
 from dotenv import load_dotenv
 from bolna.helpers.logger_config import configure_logger
 
-
 load_dotenv()
 logger = configure_logger(__name__)
 
 
 class BaseTranscriber:
     def __init__(self, input_queue=None):
         self.input_queue = input_queue
```

### Comparing `bolna-0.7.5/bolna/transcriber/deepgram_transcriber.py` & `bolna-0.7.7/bolna/transcriber/hume_transcriber.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,55 +9,58 @@
 import time
 from urllib.parse import urlencode
 from dotenv import load_dotenv
 from .base_transcriber import BaseTranscriber
 from bolna.helpers.logger_config import configure_logger
 from bolna.helpers.utils import create_ws_data_packet, int2float
 from bolna.helpers.vad import VAD
+from hume import HumeBatchClient
+
+
+import uvloop
+asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
+
 
 torch.set_num_threads(1)
 
 logger = configure_logger(__name__)
 load_dotenv()
 
 
-class DeepgramTranscriber(BaseTranscriber):
-    def __init__(self, provider, input_queue=None, model='deepgram', stream=True, language="en", endpointing="400",
+class HumeTranscriber(BaseTranscriber):
+    def __init__(self, provider, input_queue=None, model='hume', stream=True, language="en", endpointing="400",
                  sampling_rate="16000", encoding="linear16", output_queue=None, keywords=None,
                  process_interim_results="true", **kwargs):
+        logger.info(f"Initializing transcriber")
         super().__init__(input_queue)
         self.endpointing = endpointing
         self.language = language
         self.stream = stream
         self.provider = provider
         self.heartbeat_task = None
         self.sender_task = None
         self.model = 'deepgram'
         self.sampling_rate = sampling_rate
         self.encoding = encoding
         self.api_key = kwargs.get("transcriber_key", os.getenv('DEEPGRAM_AUTH_TOKEN'))
         self.transcriber_output_queue = output_queue
         self.transcription_task = None
         self.on_device_vad = kwargs.get("on_device_vad", False) if self.stream else False
-        self.keywords = keywords
         logger.info(f"self.stream: {self.stream}")
         if self.on_device_vad:
             self.vad_model = VAD()
             self.audio = []
             # logger.info("on_device_vad is TRue")
             # self.vad_model, self.vad_utils = torch.hub.load(repo_or_dir='snakers4/silero-vad', model='silero_vad', force_reload=False)
         self.voice_threshold = 0.5
         self.interruption_signalled = False
         self.sampling_rate = 16000
         if not self.stream:
             self.api_url = f"https://api.deepgram.com/v1/listen?model=nova-2&filler_words=true&language={self.language}"
             self.session = aiohttp.ClientSession()
-            if self.keywords is not None:
-                keyword_string = "&keywords=" + "&keywords=".join(self.keywords.split(","))
-                self.api_url = f"{self.api_url}{keyword_string}"
         self.audio_submitted = False
         self.audio_submission_time = None
         self.num_frames = 0
         self.connection_start_time = None
         self.process_interim_results = process_interim_results
         # Work on this soon
         self.last_utterance_time_stamp = time.time()
@@ -71,54 +74,16 @@
                 if 'words' in alternative:
                     for word_info in alternative['words']:
                         if word_info['speaker'] == 0:
                             transcript_words.append(word_info['word'])
 
         return ' '.join(transcript_words)
 
-    def get_deepgram_ws_url(self):
-        dg_params = {
-            'model': 'nova-2',
-            'filler_words': 'true',
-            'diarize': 'true',
-            'language': self.language
-        }
-
-        self.audio_frame_duration = 0.5  # We're sending 8k samples with a sample rate of 16k
-
-        if self.provider in ('twilio', 'exotel'):
-            self.encoding = 'mulaw' if self.provider == "twilio" else "linear16"
-            self.sampling_rate = 8000
-            self.audio_frame_duration = 0.2  # With twilio we are sending 200ms at a time
-
-            dg_params['encoding'] = self.encoding
-            dg_params['sample_rate'] = self.sampling_rate
-            dg_params['channels'] = "1"
-
-        if self.provider == "playground":
-            logger.info(f"CONNECTED THROUGH PLAYGROUND")
-            self.sampling_rate = 8000
-            self.audio_frame_duration = 0.0  # There's no streaming from the playground
-
-        if "en" not in self.language:
-            dg_params['language'] = self.language
-
-        if self.process_interim_results == "false":
-            dg_params['endpointing'] = self.endpointing
-        else:
-            dg_params['interim_results'] = self.process_interim_results
-            dg_params['utterance_end_ms'] = '1000'
-
-        if len(self.keywords.split(",")) > 0:
-            dg_params['keywords'] = "&keywords=".join(self.keywords.split(","))
-
-        websocket_api = 'wss://api.deepgram.com/v1/listen?'
-        websocket_url = websocket_api + urlencode(dg_params)
-        logger.info(f"Deepgram websocket url: {websocket_url}")
-        return websocket_url
+    def get_hume_ws_url(self):
+        return 'wss://api.hume.ai/v0/evi/chat'
 
     async def send_heartbeat(self, ws):
         try:
             while True:
                 data = {'type': 'KeepAlive'}
                 await ws.send(json.dumps(data))
                 await asyncio.sleep(5)  # Send a heartbeat message every 5 seconds
@@ -273,65 +238,59 @@
                         continue
                     logger.info(f"Signalling the Task manager to start speaking")
                     yield create_ws_data_packet(finalized_transcript, self.meta_info)
                     curr_message = ""
                     finalized_transcript = ""
                     continue
 
-                # if msg["type"] == "SpeechStarted":
-                #     if not self.on_device_vad:
-                #         logger.info("Not on device vad and hence inetrrupting")
-                #         yield create_ws_data_packet("TRANSCRIBER_BEGIN", self.meta_info)
-                #     continue
+                if msg["type"] == "SpeechStarted":
+                    if curr_message != "" and not self.process_interim_results:
+                        logger.info("Current messsage is null and hence inetrrupting")
+                        self.meta_info["should_interrupt"] = True
+                    elif self.process_interim_results:
+                        self.meta_info["should_interrupt"] = False
+                    logger.info(f"YIELDING TRANSCRIBER BEGIN")
+                    yield create_ws_data_packet("TRANSCRIBER_BEGIN", self.meta_info)
+                    await asyncio.sleep(0.05) #Sleep for 50ms to pass the control to task manager
+                    continue
 
                 transcript = msg['channel']['alternatives'][0]['transcript']
 
                 if transcript and len(transcript.strip()) == 0 or transcript == "":
                     continue
 
                 # TODO Remove the need for on_device_vad
                 # If interim message is not true and curr message is null, send a begin signal
                 if curr_message == "" and msg["is_final"] is False:
                     if not self.on_device_vad:
                         logger.info("Not on device vad and hence inetrrupting")
-                        self.meta_info["should_interrupt"] = True
+                        self.meta_info["should_interrupt"] = False
                     yield create_ws_data_packet("TRANSCRIBER_BEGIN", self.meta_info)
 
                     await asyncio.sleep(0.1)  # Enable taskmanager to interrupt
 
-                # Do not send back interim results, just send back interim message
-                if self.process_interim_results == "true" and msg["is_final"] is True:
-                    logger.info(f"Is final interim Transcriber message {msg}")
-                    # curr_message = self.__get_speaker_transcript(msg)
-                    finalized_transcript += " " + transcript  # Just get the whole transcript as there's mismatch at times
-                    self.meta_info["is_final"] = True
-                    if transcript.strip() != curr_message.strip():
-                        self.meta_info["utterance_end"] = self.__calculate_utterance_end(msg)
-                        self.meta_info["time_received"] = time.time()
-                        self.meta_info["transcriber_latency"] = self.meta_info["time_received"] - self.meta_info[
-                            "utterance_end"]
-                        yield create_ws_data_packet(curr_message, self.meta_info)
-                elif self.process_interim_results == "true":
+                if self.process_interim_results == "true":
                     # If we're not processing interim results
                     # Yield current transcript
                     # curr_message = self.__get_speaker_transcript(msg)
                     # Just yield the current transcript as we do not want to wait for is_final. Is_final is just to make 
                     curr_message = finalized_transcript + " " + transcript
                     logger.info(f"Yielding interim-message current_message = {curr_message}")
                     self.meta_info["include_latency"] = False
                     self.meta_info["utterance_end"] = self.__calculate_utterance_end(msg)
                     self.meta_info["time_received"] = time.time()
                     self.meta_info["transcriber_latency"] = self.meta_info["time_received"] - self.meta_info[
                         "utterance_end"]
                     yield create_ws_data_packet(curr_message, self.meta_info)
-                    # #If the current message is empty no need to send anything to the task manager
-                    # if curr_message == "":
-                    #     continue
-                    # yield create_ws_data_packet(curr_message, self.meta_info)
-                    # curr_message = ""
+                    
+                    # If is_final is true simply update the finalized transcript
+                    if  msg["is_final"] is True:
+                        finalized_transcript += " " + transcript  # Just get the whole transcript as there's mismatch at times
+                        self.meta_info["is_final"] = True
+
                 else:
                     curr_message += " " + transcript
                     # Process interim results is false and hence we need to be dependent on the endpointing
                     if msg["speech_final"] or not self.stream:
                         logger.info(f"Full Transcriber message from speech final {msg}")
                         yield create_ws_data_packet(curr_message, self.meta_info)
                         logger.info(f"Yielded {curr_message}")
@@ -365,47 +324,52 @@
                 logger.error(f"Error while getting transcriptions {e}")
                 self.interruption_signalled = False
                 yield create_ws_data_packet("TRANSCRIBER_END", self.meta_info)
 
     async def push_to_transcriber_queue(self, data_packet):
         await self.transcriber_output_queue.put(data_packet)
 
-    def deepgram_connect(self):
-        websocket_url = self.get_deepgram_ws_url()
+    def hume_connect(self):
+        websocket_url = self.get_hume_ws_url()
         extra_headers = {
-            'Authorization': 'Token {}'.format(os.getenv('DEEPGRAM_AUTH_TOKEN'))
+            "X-Hume-Api-Key": 'nODRW0JT515subWEe4GBGEOyXHoy0xV9ouN5jv6SRoETBolT',
+            "X-Hume-Client-Name": "python_sdk",
+            "X-Hume-Client-Version": "0.5.0",
         }
-        deepgram_ws = websockets.connect(websocket_url, extra_headers=extra_headers)
-        return deepgram_ws
+        hume_ws = websockets.connect(websocket_url, extra_headers=extra_headers)
+        return hume_ws
 
     async def run(self):
-        self.transcription_task = asyncio.create_task(self.transcribe())
-
+        try:
+            self.transcription_task = asyncio.create_task(self.transcribe())
+        except Exception as e:
+            logger.error(f"not working {e}")
     def __calculate_utterance_end(self, data):
         utterance_end = None
         if 'channel' in data and 'alternatives' in data['channel']:
             for alternative in data['channel']['alternatives']:
                 if 'words' in alternative:
                     final_word = alternative['words'][-1]
                     utterance_end = self.connection_start_time + final_word['end']
                     logger.info(f"Final word ended at {utterance_end}")
         return utterance_end
 
     async def transcribe(self):
+        logger.info(f"STARTED TRANSCRIBING")
         try:
-            async with self.deepgram_connect() as deepgram_ws:
+            async with self.hume_connect() as hume_ws:
                 if self.stream:
-                    self.sender_task = asyncio.create_task(self.sender_stream(deepgram_ws))
-                    self.heartbeat_task = asyncio.create_task(self.send_heartbeat(deepgram_ws))
-                    async for message in self.receiver(deepgram_ws):
+                    self.sender_task = asyncio.create_task(self.sender_stream(hume_ws))
+                    #self.heartbeat_task = asyncio.create_task(self.send_heartbeat(hume_ws))
+                    async for message in self.receiver(hume_ws):
                         if self.connection_on:
                             await self.push_to_transcriber_queue(message)
                         else:
                             logger.info("closing the deepgram connection")
-                            await self._close(deepgram_ws, data={"type": "CloseStream"})
+                            await self._close(hume_ws, data={"type": "CloseStream"})
                 else:
                     async for message in self.sender():
                         await self.push_to_transcriber_queue(message)
 
             await self.push_to_transcriber_queue(create_ws_data_packet("transcriber_connection_closed", self.meta_info))
         except Exception as e:
-            logger.error(f"Error in transcribe: {e}")
+            logger.error(f"Error in transcribe: {e}")
```

### Comparing `bolna-0.7.5/bolna.egg-info/PKG-INFO` & `bolna-0.7.7/bolna.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bolna
-Version: 0.7.5
+Version: 0.7.7
 Author-email: Prateek Sachan <ps@prateeksachan.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -666,34 +666,35 @@
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.9.0
-Requires-Dist: aiocsv==1.3.1
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: aiohttp==3.9.1
 Requires-Dist: fastapi==0.108.0
+Requires-Dist: fastembed==0.2.7
 Requires-Dist: litellm==1.15.7
 Requires-Dist: numpy==1.26.1
-Requires-Dist: openai==1.3.5
-Requires-Dist: pydantic==2.5
+Requires-Dist: openai==1.10.0
+Requires-Dist: pydantic==2.5.3
 Requires-Dist: pydub==0.25.1
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: redis==5.0.1
 Requires-Dist: requests==2.31.0
-Requires-Dist: tiktoken==0.5.2
+Requires-Dist: tiktoken==0.6.0
 Requires-Dist: twilio==8.9.0
 Requires-Dist: uvicorn==0.22.0
-Requires-Dist: uvloop==0.19.0
 Requires-Dist: websockets==10.4
-Requires-Dist: onnxruntime==1.16.3
+Requires-Dist: onnxruntime>=1.16.3
 Requires-Dist: scipy==1.11.4
+Requires-Dist: uvloop==0.19.0
+Requires-Dist: semantic-router==0.0.37
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 
 <h1 align="center">
 </h1>
 <p align="center">
   <p align="center"><b>End-to-end open-source voice agents platform</b>: Quickly build LLM based voice driven conversational applications</p>
@@ -758,44 +759,45 @@
 1. Refer to the official [`Agent` API](https://docs.bolna.dev/api-reference/agent/create) to create an agent
 2. Initiate a call via API similar to [`Call` API](https://docs.bolna.dev/api-reference/calls/make) to receive a call
 
 
 ## Using your own providers
 You can populate the `.env` file to use your own keys for providers.
 
-<details>
+<details open>
 
 <summary>ASR Providers</summary><br>
 These are the current supported ASRs Providers:
 
 | Provider     | Environment variable to be added in `.env` file |
 |--------------|-------------------------------------------------|
 | Deepgram     | `DEEPGRAM_AUTH_TOKEN`                           |
 
 </details>
 &nbsp;<br>
 
-<details>
+<details open>
 <summary>LLM Providers</summary><br>
 Bolna uses LiteLLM package to support multiple LLM integrations.
 
 These are the current supported LLM Provider Family:
 https://github.com/bolna-ai/bolna/blob/c8a0d1428793d4df29133119e354bc2f85a7ca76/bolna/providers.py#L19-L28
 
 For LiteLLM based LLMs, add either of the following to the `.env` file depending on your use-case:<br><br>
-`LITELLM_MODEL_API_BASE`: API Key of the LLM<br>
-`LITELLM_MODEL_API_BASE`: URL of the hosted LLM
+`LITELLM_MODEL_API_KEY`: API Key of the LLM<br>
+`LITELLM_MODEL_API_BASE`: URL of the hosted LLM<br>
+`LITELLM_MODEL_API_VERSION`: API VERSION for LLMs like Azure
 
 For LLMs hosted via VLLM, add the following to the `.env` file:<br>
 `VLLM_SERVER_BASE_URL`: URL of the hosted LLM using VLLM
 
 </details>
 &nbsp;<br>
 
-<details>
+<details open>
 
 <summary>TTS Providers</summary><br>
 These are the current supported TTS Providers:
 https://github.com/bolna-ai/bolna/blob/c8a0d1428793d4df29133119e354bc2f85a7ca76/bolna/providers.py#L7-L14
 
 | Provider   | Environment variable to be added in `.env` file  |
 |------------|--------------------------------------------------|
```

### Comparing `bolna-0.7.5/bolna.egg-info/SOURCES.txt` & `bolna-0.7.7/bolna.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -35,26 +35,29 @@
 bolna/input_handlers/telephony.py
 bolna/input_handlers/telephony_providers/exotel.py
 bolna/input_handlers/telephony_providers/twilio.py
 bolna/llms/__init__.py
 bolna/llms/litellm.py
 bolna/llms/llm.py
 bolna/llms/openai_llm.py
-bolna/memory/cache/BaseCache.py
 bolna/memory/cache/__init__.py
+bolna/memory/cache/base_cache.py
 bolna/memory/cache/inmemory_scalar_cache.py
+bolna/memory/cache/vector_cache.py
 bolna/output_handlers/__init__.py
 bolna/output_handlers/default.py
 bolna/output_handlers/telephony.py
 bolna/output_handlers/telephony_providers/exotel.py
 bolna/output_handlers/telephony_providers/twilio.py
 bolna/synthesizer/__init__.py
 bolna/synthesizer/base_synthesizer.py
 bolna/synthesizer/deepgram_synthesizer.py
 bolna/synthesizer/elevenlabs_synthesizer.py
 bolna/synthesizer/fourie_synthesizer.py
 bolna/synthesizer/openai_synthesizer.py
 bolna/synthesizer/polly_synthesizer.py
 bolna/synthesizer/xtts_synthesizer.py
 bolna/transcriber/__init__.py
+bolna/transcriber/azure_transcriber.py
 bolna/transcriber/base_transcriber.py
-bolna/transcriber/deepgram_transcriber.py
+bolna/transcriber/deepgram_transcriber.py
+bolna/transcriber/hume_transcriber.py
```

### Comparing `bolna-0.7.5/pyproject.toml` & `bolna-0.7.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bolna"
-version = "0.7.5"
+version = "0.7.7"
 readme = "README.md"
 authors = [
     { name = "Prateek Sachan", email = "ps@prateeksachan.com" }
 ]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU Affero General Public License v3",
@@ -26,15 +26,15 @@
 [tool.setuptools]
 package-dir = {"bolna" = "bolna"}
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
 [tool.bumpver]
-current_version = "0.7.5"
+current_version = "0.7.7"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump bolna version {old_version} -> {new_version}"
 tag_message = "bolna-{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

