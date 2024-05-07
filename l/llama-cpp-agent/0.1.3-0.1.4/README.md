# Comparing `tmp/llama_cpp_agent-0.1.3.tar.gz` & `tmp/llama_cpp_agent-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_cpp_agent-0.1.3.tar", last modified: Sun May  5 20:53:57 2024, max compression
+gzip compressed data, was "llama_cpp_agent-0.1.4.tar", last modified: Tue May  7 18:10:28 2024, max compression
```

## Comparing `llama_cpp_agent-0.1.3.tar` & `llama_cpp_agent-0.1.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:53:57.788381 llama_cpp_agent-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    43536 2024-05-05 20:53:57.788381 llama_cpp_agent-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    42505 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/ReadMe.md
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 20:53:57.788381 llama_cpp_agent-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:53:57.780381 llama_cpp_agent-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:53:57.784381 llama_cpp_agent-0.1.3/src/llama_cpp_agent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:53:57.784381 llama_cpp_agent-0.1.3/src/llama_cpp_agent/agent_memory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/agent_memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/agent_memory/core_memory_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/agent_memory/event_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/agent_memory/event_memory_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     9662 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/agent_memory/memory_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/agent_memory/retrieval_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    13281 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)    30607 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/function_calling.py
--rw-r--r--   0 runner    (1001) docker     (127)    19012 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/function_calling_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:53:57.784381 llama_cpp_agent-0.1.3/src/llama_cpp_agent/gbnf_grammar_generator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/gbnf_grammar_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    69482 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    13114 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/hermes_2_pro_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    71969 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/llm_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/llm_prompt_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/llm_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     8390 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)    21539 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/messages_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/mixtral_8x22b_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/output_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:53:57.784381 llama_cpp_agent-0.1.3/src/llama_cpp_agent/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6910 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/providers/kobold_cpp_endpoint_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    14216 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/providers/llama_cpp_endpoint_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     9458 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/providers/openai_endpoint_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     9785 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/providers/provider_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:53:57.788381 llama_cpp_agent-0.1.3/src/llama_cpp_agent/rag/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/rag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/rag/rag_colbert_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/rag/text_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10885 2024-05-05 20:53:53.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent/structured_output_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:53:57.788381 llama_cpp_agent-0.1.3/src/llama_cpp_agent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43536 2024-05-05 20:53:57.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-05 20:53:57.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 20:53:57.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-05 20:53:57.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-05 20:53:57.000000 llama_cpp_agent-0.1.3/src/llama_cpp_agent.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 18:10:28.579935 llama_cpp_agent-0.1.4/
+-rw-rw-rw-   0        0        0     1115 2023-12-31 18:08:30.000000 llama_cpp_agent-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0    10696 2024-05-07 18:10:28.578935 llama_cpp_agent-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9639 2024-05-07 18:09:11.000000 llama_cpp_agent-0.1.4/ReadMe.md
+-rw-rw-rw-   0        0        0      990 2024-05-07 18:09:11.000000 llama_cpp_agent-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-07 18:10:28.579935 llama_cpp_agent-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-07 18:10:28.543169 llama_cpp_agent-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-07 18:10:28.558793 llama_cpp_agent-0.1.4/src/llama_cpp_agent/
+-rw-rw-rw-   0        0        0        0 2024-01-04 14:13:41.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 18:10:28.569317 llama_cpp_agent-0.1.4/src/llama_cpp_agent/agent_memory/
+-rw-rw-rw-   0        0        0        0 2023-12-31 14:27:21.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/agent_memory/__init__.py
+-rw-rw-rw-   0        0        0     3408 2024-03-29 17:24:31.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/agent_memory/core_memory_manager.py
+-rw-rw-rw-   0        0        0     1636 2024-03-29 17:24:31.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/agent_memory/event_memory.py
+-rw-rw-rw-   0        0        0     3876 2024-05-05 05:07:17.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/agent_memory/event_memory_manager.py
+-rw-rw-rw-   0        0        0     9949 2024-03-29 17:24:31.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/agent_memory/memory_tools.py
+-rw-rw-rw-   0        0        0     5031 2024-04-18 21:27:19.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/agent_memory/retrieval_memory.py
+-rw-rw-rw-   0        0        0     1640 2024-03-29 17:24:31.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py
+-rw-rw-rw-   0        0        0    13499 2024-05-06 00:08:47.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/chain.py
+-rw-rw-rw-   0        0        0    31285 2024-05-05 20:17:34.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/function_calling.py
+-rw-rw-rw-   0        0        0    19446 2024-05-05 20:26:45.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/function_calling_agent.py
+drwxrwxrwx   0        0        0        0 2024-05-07 18:10:28.570316 llama_cpp_agent-0.1.4/src/llama_cpp_agent/gbnf_grammar_generator/
+-rw-rw-rw-   0        0        0        0 2023-12-27 02:55:26.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/gbnf_grammar_generator/__init__.py
+-rw-rw-rw-   0        0        0    71258 2024-05-05 20:17:35.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py
+-rw-rw-rw-   0        0        0    13437 2024-05-05 20:17:34.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/hermes_2_pro_agent.py
+-rw-rw-rw-   0        0        0    73714 2024-05-05 20:17:35.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/llm_agent.py
+-rw-rw-rw-   0        0        0     7027 2024-03-29 17:24:31.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/llm_prompt_template.py
+-rw-rw-rw-   0        0        0     6022 2024-05-01 05:39:37.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/llm_settings.py
+-rw-rw-rw-   0        0        0     8664 2024-05-05 20:17:34.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/messages.py
+-rw-rw-rw-   0        0        0    22118 2024-05-05 20:17:34.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/messages_formatter.py
+-rw-rw-rw-   0        0        0     4313 2024-05-05 20:17:34.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/mixtral_8x22b_agent.py
+-rw-rw-rw-   0        0        0     3613 2024-04-18 21:27:19.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/output_parser.py
+drwxrwxrwx   0        0        0        0 2024-05-07 18:10:28.574440 llama_cpp_agent-0.1.4/src/llama_cpp_agent/providers/
+-rw-rw-rw-   0        0        0        0 2024-01-08 13:25:58.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/providers/__init__.py
+-rw-rw-rw-   0        0        0     7135 2024-05-05 05:07:17.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/providers/kobold_cpp_endpoint_provider.py
+-rw-rw-rw-   0        0        0    14586 2024-05-05 20:17:34.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/providers/llama_cpp_endpoint_provider.py
+-rw-rw-rw-   0        0        0     9740 2024-05-05 20:17:34.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/providers/openai_endpoint_provider.py
+-rw-rw-rw-   0        0        0    10078 2024-05-05 20:17:34.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/providers/provider_base.py
+drwxrwxrwx   0        0        0        0 2024-05-07 18:10:28.577423 llama_cpp_agent-0.1.4/src/llama_cpp_agent/rag/
+-rw-rw-rw-   0        0        0        0 2024-05-05 05:07:17.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/rag/__init__.py
+-rw-rw-rw-   0        0        0     2359 2024-05-05 05:07:17.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/rag/rag_colbert_reranker.py
+-rw-rw-rw-   0        0        0     3945 2024-05-05 20:17:34.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/rag/text_utils.py
+-rw-rw-rw-   0        0        0    11126 2024-05-05 20:17:34.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/structured_output_agent.py
+drwxrwxrwx   0        0        0        0 2024-05-07 18:10:28.577930 llama_cpp_agent-0.1.4/src/llama_cpp_agent.egg-info/
+-rw-rw-rw-   0        0        0    10696 2024-05-07 18:10:28.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1645 2024-05-07 18:10:28.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 18:10:28.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      150 2024-05-07 18:10:28.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-07 18:10:28.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent.egg-info/top_level.txt
```

### Comparing `llama_cpp_agent-0.1.3/LICENSE` & `llama_cpp_agent-0.1.4/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-llama-cpp-agent
-MIT License
-
-Copyright (c) 2023-2024 Maximilian Winter
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+llama-cpp-agent
+MIT License
+
+Copyright (c) 2023-2024 Maximilian Winter
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `llama_cpp_agent-0.1.3/pyproject.toml` & `llama_cpp_agent-0.1.4/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-[build-system]
-requires = [  "setuptools>=42"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "llama-cpp-agent"
-version = "0.1.3"
-description = "A framework for building LLM based AI agents with llama.cpp."
-
-readme = "ReadMe.md"
-dependencies = [
-    "llama-cpp-python>=0.2.60",
-    "pydantic>=2.5.3",
-    "requests>=2.31.0",
-    "docstring_parser",
-    "aiohttp"
-]
-
-requires-python = ">=3.10"
-classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent" ]
-[[project.authors]]
-name = "Maximilian Winter"
-email = "maximilian.winter.91@gmail.com"
-
-
-[project.optional-dependencies]
-agent_memory = ["chromadb", "SQLAlchemy", "numpy", "scipy"]
-rag = ["ragatouille"]
-
-[project.urls]
-Homepage = "https://github.com/Maximilian-Winter/llama-cpp-agent"
-"Bug Tracker" = "https://github.com/Maximilian-Winter/llama-cpp-agent/issues"
-
-[tool.setuptools.packages.find]
-where = ["src"]
-
+[build-system]
+requires = [  "setuptools>=42"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "llama-cpp-agent"
+version = "0.1.4"
+description = "A framework for building LLM based AI agents with llama.cpp."
+
+readme = "ReadMe.md"
+dependencies = [
+    "llama-cpp-python>=0.2.60",
+    "pydantic>=2.5.3",
+    "requests>=2.31.0",
+    "docstring_parser",
+    "aiohttp"
+]
+
+requires-python = ">=3.10"
+classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent" ]
+[[project.authors]]
+name = "Maximilian Winter"
+email = "maximilian.winter.91@gmail.com"
+
+
+[project.optional-dependencies]
+agent_memory = ["chromadb", "SQLAlchemy", "numpy", "scipy"]
+rag = ["ragatouille"]
+
+[project.urls]
+Homepage = "https://github.com/Maximilian-Winter/llama-cpp-agent"
+"Bug Tracker" = "https://github.com/Maximilian-Winter/llama-cpp-agent/issues"
+
+[tool.setuptools.packages.find]
+where = ["src"]
+
```

### Comparing `llama_cpp_agent-0.1.3/src/llama_cpp_agent/agent_memory/core_memory_manager.py` & `llama_cpp_agent-0.1.4/src/llama_cpp_agent/agent_memory/core_memory_manager.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-import datetime
-import json
-
-
-class CoreMemoryManager:
-    def __init__(self, core_memory: dict):
-        self.core_memory = core_memory
-        self.last_modified = "Never"
-
-    def add_to_core_memory(self, key: str, child_key: str, value) -> str:
-        """
-        Adds or updates an entry in the IAM.
-        """
-        if key not in self.core_memory:
-            self.core_memory[key] = {}
-        self.core_memory[key][child_key] = value
-        self.last_modified = datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")
-        return f"Core memory updated. Key: {key}, Child Key: {child_key}"
-
-    def replace_in_core_memory(self, key: str, child_key: str, new_value) -> str:
-        """
-        Replaces an existing entry in the IAM.
-        """
-        if key in self.core_memory and child_key in self.core_memory[key]:
-            self.core_memory[key][child_key] = new_value
-            self.last_modified = datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")
-            return f"Core memory replaced. Key: {key}, Child Key: {child_key}"
-        else:
-            return "Key or child key not found in Core memory."
-
-    def remove_from_core_memory(self, key: str, child_key: str) -> str:
-        """
-        Removes a specific field from a IAM entry.
-        """
-        if key in self.core_memory and child_key in self.core_memory[key]:
-            del self.core_memory[key][child_key]
-            self.last_modified = datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")
-            return f"Core memory entry removed. Key: {key}, Child Key: {child_key}"
-        else:
-            return "Key or child key not found in Core memory."
-
-    def build_core_memory_context(self):
-        context = ""
-        # for key, item in self.core_memory.items():
-        #     context += f"""#### {key} ####\n"""
-        #     for key2, item2 in item.items():
-        #         context += f"""{key2}:\n{self.format_multiline_description(item2.strip(), 0)}\n\n"""
-        #     if item == {}:
-        #         context += "Empty Section\n"
-        # context = json.dumps(self.core_memory, indent=2)
-        for key, item in self.core_memory.items():
-            context += f"""<{key}>\n"""
-            for key2, item2 in item.items():
-                context += f"""  <{key2}>\n{self.format_multiline_description(item2.strip(), 1)}\n  </{key2}>\n"""
-            context += f"</{key}>\n"
-        if context == "":
-            context = "No Core Memories!"
-        return context
-
-    def format_multiline_description(self, description: str, indent_level: int) -> str:
-        """
-        Format a multiline description with proper indentation.
-
-        Args:
-            description (str): Multiline description.
-            indent_level (int): Indentation level.
-
-        Returns:
-            str: Formatted multiline description.
-        """
-        indent = "    " * indent_level
-        return indent + description.replace("\n", "\n" + indent)
-
-    def load(self, file_path):
-        with open(file_path, "r", encoding="utf-8") as file:
-            self.core_memory = json.load(file)
-        self.last_modified = datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")
-
-    def save(self, filepath):
-        with open(filepath, "w", encoding="utf-8") as file:
-            json.dump(self.core_memory, file, indent=4)
+import datetime
+import json
+
+
+class CoreMemoryManager:
+    def __init__(self, core_memory: dict):
+        self.core_memory = core_memory
+        self.last_modified = "Never"
+
+    def add_to_core_memory(self, key: str, child_key: str, value) -> str:
+        """
+        Adds or updates an entry in the IAM.
+        """
+        if key not in self.core_memory:
+            self.core_memory[key] = {}
+        self.core_memory[key][child_key] = value
+        self.last_modified = datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")
+        return f"Core memory updated. Key: {key}, Child Key: {child_key}"
+
+    def replace_in_core_memory(self, key: str, child_key: str, new_value) -> str:
+        """
+        Replaces an existing entry in the IAM.
+        """
+        if key in self.core_memory and child_key in self.core_memory[key]:
+            self.core_memory[key][child_key] = new_value
+            self.last_modified = datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")
+            return f"Core memory replaced. Key: {key}, Child Key: {child_key}"
+        else:
+            return "Key or child key not found in Core memory."
+
+    def remove_from_core_memory(self, key: str, child_key: str) -> str:
+        """
+        Removes a specific field from a IAM entry.
+        """
+        if key in self.core_memory and child_key in self.core_memory[key]:
+            del self.core_memory[key][child_key]
+            self.last_modified = datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")
+            return f"Core memory entry removed. Key: {key}, Child Key: {child_key}"
+        else:
+            return "Key or child key not found in Core memory."
+
+    def build_core_memory_context(self):
+        context = ""
+        # for key, item in self.core_memory.items():
+        #     context += f"""#### {key} ####\n"""
+        #     for key2, item2 in item.items():
+        #         context += f"""{key2}:\n{self.format_multiline_description(item2.strip(), 0)}\n\n"""
+        #     if item == {}:
+        #         context += "Empty Section\n"
+        # context = json.dumps(self.core_memory, indent=2)
+        for key, item in self.core_memory.items():
+            context += f"""<{key}>\n"""
+            for key2, item2 in item.items():
+                context += f"""  <{key2}>\n{self.format_multiline_description(item2.strip(), 1)}\n  </{key2}>\n"""
+            context += f"</{key}>\n"
+        if context == "":
+            context = "No Core Memories!"
+        return context
+
+    def format_multiline_description(self, description: str, indent_level: int) -> str:
+        """
+        Format a multiline description with proper indentation.
+
+        Args:
+            description (str): Multiline description.
+            indent_level (int): Indentation level.
+
+        Returns:
+            str: Formatted multiline description.
+        """
+        indent = "    " * indent_level
+        return indent + description.replace("\n", "\n" + indent)
+
+    def load(self, file_path):
+        with open(file_path, "r", encoding="utf-8") as file:
+            self.core_memory = json.load(file)
+        self.last_modified = datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")
+
+    def save(self, filepath):
+        with open(filepath, "w", encoding="utf-8") as file:
+            json.dump(self.core_memory, file, indent=4)
```

### Comparing `llama_cpp_agent-0.1.3/src/llama_cpp_agent/agent_memory/memory_tools.py` & `llama_cpp_agent-0.1.4/src/llama_cpp_agent/agent_memory/memory_tools.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,287 +1,287 @@
-from datetime import datetime
-from enum import Enum
-from typing import List, Optional
-
-from pydantic import BaseModel, Field
-from sqlalchemy import create_engine
-from sqlalchemy.orm import sessionmaker, scoped_session
-
-from .event_memory import EventType, Base
-from .event_memory_manager import EventMemoryManager
-from ..function_calling import LlamaCppFunctionTool
-from .core_memory_manager import CoreMemoryManager
-from .retrieval_memory_manager import RetrievalMemoryManager, RetrievalMemory
-
-
-class CoreMemoryKey(Enum):
-    PERSONA: str = "persona"
-    HUMAN: str = "human"
-
-
-class core_memory_append(BaseModel):
-    """
-    Append a new entry to the Core Memory.
-    """
-
-    key: str = Field(..., description="The key identifier of the core memory.")
-    field: str = Field(..., description="The field within the core memory.")
-    value: str = Field(
-        ...,
-        description="The value or data to be stored in the specified core memory entry.",
-    )
-
-    def run(self, core_memory_manager: CoreMemoryManager):
-        return core_memory_manager.add_to_core_memory(
-            self.key.value, self.field, self.value
-        )
-
-
-class core_memory_replace(BaseModel):
-    """
-    Replace an entry in the Core Memory.
-    """
-
-    key: str = Field(..., description="The key identifier of the core memory.")
-    field: str = Field(..., description="The field within the core memory.")
-    new_value: str = Field(
-        ...,
-        description="The new value to replace with the existing data in the specified Core Memory field.",
-    )
-
-    def run(self, core_memory_manager: CoreMemoryManager):
-        return core_memory_manager.replace_in_core_memory(
-            self.key.value, self.field, self.new_value
-        )
-
-
-class core_memory_remove(BaseModel):
-    """
-    Remove an entry from the Core Memory.
-    """
-
-    key: str = Field(..., description="The key identifier of the core memory.")
-    field: str = Field(..., description="The field within the core memory.")
-
-    def run(self, core_memory_manager: CoreMemoryManager):
-        return core_memory_manager.remove_from_core_memory(self.key.value, self.field)
-
-
-class conversation_search(BaseModel):
-    """
-    Search prior conversation history using case-insensitive string matching.
-    """
-
-    keywords: List[str] = Field(
-        ...,
-        description='Keywords that the messages have to contain. Eg. ["hello", "world"]',
-    )
-    page: Optional[int] = Field(
-        ...,
-        description="Allows you to page through results. Only use on a follow-up query. Defaults to 0 (first page).",
-    )
-
-    def run(self, event_memory_manager: EventMemoryManager):
-        parsed_start_datetime = None
-        parsed_end_datetime = None
-        if self.page is None:
-            self.page = 0
-        return event_memory_manager.query_events(
-            event_types=[
-                EventType.UserMessage,
-                EventType.AgentMessage,
-                EventType.SystemMessage,
-                EventType.FunctionMessage,
-            ],
-            content_keywords=self.keywords,
-            start_date=parsed_start_datetime,
-            end_date=parsed_end_datetime,
-            page=self.page,
-        )
-
-
-class conversation_search_date(BaseModel):
-    """
-    Search prior conversation history using a date range.
-    """
-
-    start_date: str = Field(
-        ...,
-        description='The start of the date range to search, in the format "dd/mm/YYYY, H:M:S" eg. "01/01/2024, 08:00:30"',
-    )
-    end_date: str = Field(
-        ...,
-        description='The end of the date range to search, in the format "dd/mm/YYYY, H:M:S" eg. "04/02/2024, 18:57:29"',
-    )
-    page: Optional[int] = Field(
-        ...,
-        description="Allows you to page through results. Only use on a follow-up query. Defaults to 0 (first page).",
-    )
-
-    def run(self, event_memory_manager: EventMemoryManager):
-        parsed_start_datetime = None
-        parsed_end_datetime = None
-        if self.start_date:
-            parsed_start_datetime = datetime.strptime(
-                self.start_date, "%d/%m/%Y, %H:%M:%S"
-            )
-        if self.end_date:
-            parsed_end_datetime = datetime.strptime(self.end_date, "%d/%m/%Y, %H:%M:%S")
-        if self.page is None:
-            self.page = 0
-
-        return event_memory_manager.query_events(
-            event_types=[
-                EventType.UserMessage,
-                EventType.AgentMessage,
-                EventType.SystemMessage,
-                EventType.FunctionMessage,
-            ],
-            start_date=parsed_start_datetime,
-            end_date=parsed_end_datetime,
-            page=self.page,
-        )
-
-
-class archival_memory_search(BaseModel):
-    """
-    Search archival memory using semantic (embedding-based) search.
-    """
-
-    query: str = Field(
-        ...,
-        description="String to search for. The search will return the most semantically similar memories to this query.",
-    )
-    page: Optional[int] = Field(
-        ...,
-        description="Allows you to page through results. Only use on a follow-up query. Defaults to 0 (first page).",
-    )
-
-    def run(self, retrieval_memory_manager: RetrievalMemoryManager):
-        return retrieval_memory_manager.retrieve_memories(self.query)
-
-
-class archival_memory_insert(BaseModel):
-    """
-    Add to archival memory. Make sure to phrase the memory contents such that it can be easily queried later.
-    """
-
-    memory: str = Field(
-        ...,
-        description="Content to write to the memory. All unicode (including emojis) are supported.",
-    )
-    importance: float = Field(
-        ...,
-        description="A value from 1.0 to 10.0 indicating the importance of the memory.",
-    )
-
-    def run(self, retrieval_memory_manager: RetrievalMemoryManager):
-        return retrieval_memory_manager.add_memory_to_retrieval(
-            self.memory, self.importance
-        )
-
-
-class AgentRetrievalMemory:
-    def __init__(
-        self,
-        persistent_db_path="./retrieval_memory",
-        embedding_model_name="all-MiniLM-L6-v2",
-        collection_name="retrieval_memory_collection",
-    ):
-        self.retrieval_memory = RetrievalMemory(
-            persistent_db_path, embedding_model_name, collection_name
-        )
-        self.retrieval_memory_manager = RetrievalMemoryManager(self.retrieval_memory)
-        self.retrieve_memories_tool = LlamaCppFunctionTool(
-            archival_memory_search,
-            retrieval_memory_manager=self.retrieval_memory_manager,
-        )
-        self.add_retrieval_memory_tool = LlamaCppFunctionTool(
-            archival_memory_insert,
-            retrieval_memory_manager=self.retrieval_memory_manager,
-        )
-
-    def get_tool_list(self):
-        return [self.retrieve_memories_tool, self.add_retrieval_memory_tool]
-
-    def get_retrieve_memories_tool(self):
-        return self.retrieve_memories_tool
-
-    def get_add_retrieval_memory_tool(self):
-        return self.add_retrieval_memory_tool
-
-
-class AgentCoreMemory:
-    def __init__(self, core_memory=None, core_memory_file=None):
-        if core_memory is None:
-            core_memory = {}
-
-        self.core_memory_manager = CoreMemoryManager(core_memory)
-        if core_memory_file is not None:
-            self.core_memory_manager.load(core_memory_file)
-
-        self.add_core_memory_tool = LlamaCppFunctionTool(
-            core_memory_append, core_memory_manager=self.core_memory_manager
-        )
-        self.remove_core_memory_tool = LlamaCppFunctionTool(
-            core_memory_remove, core_memory_manager=self.core_memory_manager
-        )
-        self.replace_core_memory_tool = LlamaCppFunctionTool(
-            core_memory_replace, core_memory_manager=self.core_memory_manager
-        )
-
-    def get_core_memory_manager(self):
-        return self.core_memory_manager
-
-    def get_tool_list(self):
-        return [
-            self.add_core_memory_tool,
-            self.remove_core_memory_tool,
-            self.replace_core_memory_tool,
-        ]
-
-    def get_add_core_memory_tool(self):
-        return self.add_core_memory_tool
-
-    def get_remove_core_memory_tool(self):
-        return self.remove_core_memory_tool
-
-    def get_replace_core_memory_tool(self):
-        return self.replace_core_memory_tool
-
-    def save_core_memory(self, file_path):
-        self.core_memory_manager.save(file_path)
-
-    def load_core_memory(self, file_path):
-        self.core_memory_manager.load(file_path)
-
-
-class AgentEventMemory:
-    def __init__(self, event_queue_file=None, db_path="sqlite:///events.db"):
-        self.engine = create_engine(db_path)
-        session_factory = sessionmaker(bind=self.engine)
-        Base.metadata.create_all(self.engine)
-        self.Session = scoped_session(session_factory)
-        self.session = self.Session()
-        self.event_memory_manager = EventMemoryManager(self.session)
-
-        if event_queue_file is not None:
-            self.event_memory_manager.load_event_queue(event_queue_file)
-        self.search_event_memory_manager_tool = LlamaCppFunctionTool(
-            conversation_search, event_memory_manager=self.event_memory_manager
-        )
-
-        self.search_event_memory_manager_tool_date = LlamaCppFunctionTool(
-            conversation_search_date, event_memory_manager=self.event_memory_manager
-        )
-
-    def get_event_memory_manager(self):
-        return self.event_memory_manager
-
-    def get_tool_list(self):
-        return [
-            self.search_event_memory_manager_tool,
-            self.search_event_memory_manager_tool_date,
-        ]
-
-    def get_search_event_memory_manager_tool(self):
-        return self.search_event_memory_manager_tool
+from datetime import datetime
+from enum import Enum
+from typing import List, Optional
+
+from pydantic import BaseModel, Field
+from sqlalchemy import create_engine
+from sqlalchemy.orm import sessionmaker, scoped_session
+
+from .event_memory import EventType, Base
+from .event_memory_manager import EventMemoryManager
+from ..function_calling import LlamaCppFunctionTool
+from .core_memory_manager import CoreMemoryManager
+from .retrieval_memory_manager import RetrievalMemoryManager, RetrievalMemory
+
+
+class CoreMemoryKey(Enum):
+    PERSONA: str = "persona"
+    HUMAN: str = "human"
+
+
+class core_memory_append(BaseModel):
+    """
+    Append a new entry to the Core Memory.
+    """
+
+    key: str = Field(..., description="The key identifier of the core memory.")
+    field: str = Field(..., description="The field within the core memory.")
+    value: str = Field(
+        ...,
+        description="The value or data to be stored in the specified core memory entry.",
+    )
+
+    def run(self, core_memory_manager: CoreMemoryManager):
+        return core_memory_manager.add_to_core_memory(
+            self.key.value, self.field, self.value
+        )
+
+
+class core_memory_replace(BaseModel):
+    """
+    Replace an entry in the Core Memory.
+    """
+
+    key: str = Field(..., description="The key identifier of the core memory.")
+    field: str = Field(..., description="The field within the core memory.")
+    new_value: str = Field(
+        ...,
+        description="The new value to replace with the existing data in the specified Core Memory field.",
+    )
+
+    def run(self, core_memory_manager: CoreMemoryManager):
+        return core_memory_manager.replace_in_core_memory(
+            self.key.value, self.field, self.new_value
+        )
+
+
+class core_memory_remove(BaseModel):
+    """
+    Remove an entry from the Core Memory.
+    """
+
+    key: str = Field(..., description="The key identifier of the core memory.")
+    field: str = Field(..., description="The field within the core memory.")
+
+    def run(self, core_memory_manager: CoreMemoryManager):
+        return core_memory_manager.remove_from_core_memory(self.key.value, self.field)
+
+
+class conversation_search(BaseModel):
+    """
+    Search prior conversation history using case-insensitive string matching.
+    """
+
+    keywords: List[str] = Field(
+        ...,
+        description='Keywords that the messages have to contain. Eg. ["hello", "world"]',
+    )
+    page: Optional[int] = Field(
+        ...,
+        description="Allows you to page through results. Only use on a follow-up query. Defaults to 0 (first page).",
+    )
+
+    def run(self, event_memory_manager: EventMemoryManager):
+        parsed_start_datetime = None
+        parsed_end_datetime = None
+        if self.page is None:
+            self.page = 0
+        return event_memory_manager.query_events(
+            event_types=[
+                EventType.UserMessage,
+                EventType.AgentMessage,
+                EventType.SystemMessage,
+                EventType.FunctionMessage,
+            ],
+            content_keywords=self.keywords,
+            start_date=parsed_start_datetime,
+            end_date=parsed_end_datetime,
+            page=self.page,
+        )
+
+
+class conversation_search_date(BaseModel):
+    """
+    Search prior conversation history using a date range.
+    """
+
+    start_date: str = Field(
+        ...,
+        description='The start of the date range to search, in the format "dd/mm/YYYY, H:M:S" eg. "01/01/2024, 08:00:30"',
+    )
+    end_date: str = Field(
+        ...,
+        description='The end of the date range to search, in the format "dd/mm/YYYY, H:M:S" eg. "04/02/2024, 18:57:29"',
+    )
+    page: Optional[int] = Field(
+        ...,
+        description="Allows you to page through results. Only use on a follow-up query. Defaults to 0 (first page).",
+    )
+
+    def run(self, event_memory_manager: EventMemoryManager):
+        parsed_start_datetime = None
+        parsed_end_datetime = None
+        if self.start_date:
+            parsed_start_datetime = datetime.strptime(
+                self.start_date, "%d/%m/%Y, %H:%M:%S"
+            )
+        if self.end_date:
+            parsed_end_datetime = datetime.strptime(self.end_date, "%d/%m/%Y, %H:%M:%S")
+        if self.page is None:
+            self.page = 0
+
+        return event_memory_manager.query_events(
+            event_types=[
+                EventType.UserMessage,
+                EventType.AgentMessage,
+                EventType.SystemMessage,
+                EventType.FunctionMessage,
+            ],
+            start_date=parsed_start_datetime,
+            end_date=parsed_end_datetime,
+            page=self.page,
+        )
+
+
+class archival_memory_search(BaseModel):
+    """
+    Search archival memory using semantic (embedding-based) search.
+    """
+
+    query: str = Field(
+        ...,
+        description="String to search for. The search will return the most semantically similar memories to this query.",
+    )
+    page: Optional[int] = Field(
+        ...,
+        description="Allows you to page through results. Only use on a follow-up query. Defaults to 0 (first page).",
+    )
+
+    def run(self, retrieval_memory_manager: RetrievalMemoryManager):
+        return retrieval_memory_manager.retrieve_memories(self.query)
+
+
+class archival_memory_insert(BaseModel):
+    """
+    Add to archival memory. Make sure to phrase the memory contents such that it can be easily queried later.
+    """
+
+    memory: str = Field(
+        ...,
+        description="Content to write to the memory. All unicode (including emojis) are supported.",
+    )
+    importance: float = Field(
+        ...,
+        description="A value from 1.0 to 10.0 indicating the importance of the memory.",
+    )
+
+    def run(self, retrieval_memory_manager: RetrievalMemoryManager):
+        return retrieval_memory_manager.add_memory_to_retrieval(
+            self.memory, self.importance
+        )
+
+
+class AgentRetrievalMemory:
+    def __init__(
+        self,
+        persistent_db_path="./retrieval_memory",
+        embedding_model_name="all-MiniLM-L6-v2",
+        collection_name="retrieval_memory_collection",
+    ):
+        self.retrieval_memory = RetrievalMemory(
+            persistent_db_path, embedding_model_name, collection_name
+        )
+        self.retrieval_memory_manager = RetrievalMemoryManager(self.retrieval_memory)
+        self.retrieve_memories_tool = LlamaCppFunctionTool(
+            archival_memory_search,
+            retrieval_memory_manager=self.retrieval_memory_manager,
+        )
+        self.add_retrieval_memory_tool = LlamaCppFunctionTool(
+            archival_memory_insert,
+            retrieval_memory_manager=self.retrieval_memory_manager,
+        )
+
+    def get_tool_list(self):
+        return [self.retrieve_memories_tool, self.add_retrieval_memory_tool]
+
+    def get_retrieve_memories_tool(self):
+        return self.retrieve_memories_tool
+
+    def get_add_retrieval_memory_tool(self):
+        return self.add_retrieval_memory_tool
+
+
+class AgentCoreMemory:
+    def __init__(self, core_memory=None, core_memory_file=None):
+        if core_memory is None:
+            core_memory = {}
+
+        self.core_memory_manager = CoreMemoryManager(core_memory)
+        if core_memory_file is not None:
+            self.core_memory_manager.load(core_memory_file)
+
+        self.add_core_memory_tool = LlamaCppFunctionTool(
+            core_memory_append, core_memory_manager=self.core_memory_manager
+        )
+        self.remove_core_memory_tool = LlamaCppFunctionTool(
+            core_memory_remove, core_memory_manager=self.core_memory_manager
+        )
+        self.replace_core_memory_tool = LlamaCppFunctionTool(
+            core_memory_replace, core_memory_manager=self.core_memory_manager
+        )
+
+    def get_core_memory_manager(self):
+        return self.core_memory_manager
+
+    def get_tool_list(self):
+        return [
+            self.add_core_memory_tool,
+            self.remove_core_memory_tool,
+            self.replace_core_memory_tool,
+        ]
+
+    def get_add_core_memory_tool(self):
+        return self.add_core_memory_tool
+
+    def get_remove_core_memory_tool(self):
+        return self.remove_core_memory_tool
+
+    def get_replace_core_memory_tool(self):
+        return self.replace_core_memory_tool
+
+    def save_core_memory(self, file_path):
+        self.core_memory_manager.save(file_path)
+
+    def load_core_memory(self, file_path):
+        self.core_memory_manager.load(file_path)
+
+
+class AgentEventMemory:
+    def __init__(self, event_queue_file=None, db_path="sqlite:///events.db"):
+        self.engine = create_engine(db_path)
+        session_factory = sessionmaker(bind=self.engine)
+        Base.metadata.create_all(self.engine)
+        self.Session = scoped_session(session_factory)
+        self.session = self.Session()
+        self.event_memory_manager = EventMemoryManager(self.session)
+
+        if event_queue_file is not None:
+            self.event_memory_manager.load_event_queue(event_queue_file)
+        self.search_event_memory_manager_tool = LlamaCppFunctionTool(
+            conversation_search, event_memory_manager=self.event_memory_manager
+        )
+
+        self.search_event_memory_manager_tool_date = LlamaCppFunctionTool(
+            conversation_search_date, event_memory_manager=self.event_memory_manager
+        )
+
+    def get_event_memory_manager(self):
+        return self.event_memory_manager
+
+    def get_tool_list(self):
+        return [
+            self.search_event_memory_manager_tool,
+            self.search_event_memory_manager_tool_date,
+        ]
+
+    def get_search_event_memory_manager_tool(self):
+        return self.search_event_memory_manager_tool
```

### Comparing `llama_cpp_agent-0.1.3/src/llama_cpp_agent/agent_memory/retrieval_memory.py` & `llama_cpp_agent-0.1.4/src/llama_cpp_agent/agent_memory/retrieval_memory.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,144 +1,144 @@
-import datetime
-import uuid
-
-import chromadb
-import numpy as np
-from chromadb.utils import embedding_functions
-from scipy.spatial.distance import cosine
-
-
-class RetrievalMemory:
-    def __init__(
-        self,
-        persistent_db_path="./retrieval_memory",
-        embedding_model_name="BAAI/bge-small-en-v1.5",
-        collection_name="retrieval_memory_collection",
-        decay_factor=0.99,
-    ):
-        self.client = chromadb.PersistentClient(path=persistent_db_path)
-        self.sentence_transformer_ef = (
-            embedding_functions.SentenceTransformerEmbeddingFunction(
-                model_name=embedding_model_name
-            )
-        )
-        self.collection = self.client.get_or_create_collection(
-            name=collection_name, embedding_function=self.sentence_transformer_ef
-        )
-        self.decay_factor = decay_factor
-
-    def add_memory(
-        self,
-        description: str,
-        date: datetime.datetime = datetime.datetime.now(),
-        importance: float = 1.0,
-    ):
-        """Add a memory with a given description and importance to the memory stream."""
-        mem = [description]
-        ids = [str(self.generate_unique_id())]
-        metadata = {
-            "memory_id": ids[0],
-            "memory": description,
-            "importance": importance,
-            "creation_timestamp": date.strftime("%Y-%m-%d %H:%M:%S"),
-            "last_access_timestamp": date.strftime("%Y-%m-%d %H:%M:%S"),
-        }
-        self.collection.add(documents=mem, metadatas=metadata, ids=ids)
-
-    def retrieve_memories(
-        self,
-        query: str,
-        k,
-        date=datetime.datetime.now(),
-        alpha_recency=1,
-        alpha_relevance=1,
-        alpha_importance=1,
-    ):
-        query_embedding = self.sentence_transformer_ef([query])
-        query_result = self.collection.query(
-            query_embedding,
-            n_results=k * 4,
-            include=["metadatas", "embeddings", "documents", "distances"],
-        )  # Increase candidate pool size
-        if len(query_result["metadatas"][0]) == 0:
-            return []
-        # Step 2: Apply scoring to the candidate memories
-        scores = []
-        for index in range(len(query_result["metadatas"][0])):
-            scores.append(
-                self.compute_memory_score(
-                    query_result["metadatas"][0][index],
-                    query_result["embeddings"][0][index],
-                    query_embedding,
-                    date,
-                    alpha_recency,
-                    alpha_relevance,
-                    alpha_importance,
-                )
-            )
-
-        # Normalize and select top k memories based on scores
-        normalized_scores = self.normalize_scores(np.array(scores))
-        top_indices = self.get_top_indices(normalized_scores, k)
-        retrieved_memories = [query_result["metadatas"][0][i] for i in top_indices]
-
-        # Update last access time
-        for memory in retrieved_memories:
-            memory = self.update_last_access(memory, date)
-            self.collection.upsert(
-                ids=memory["memory_id"], documents=[memory["memory"]], metadatas=memory
-            )
-        return retrieved_memories
-
-    @staticmethod
-    def generate_unique_id():
-        unique_id = str(uuid.uuid4())
-        return unique_id
-
-    def compute_memory_score(
-        self,
-        metadata,
-        memory_embedding,
-        query_embedding,
-        date,
-        alpha_recency,
-        alpha_relevance,
-        alpha_importance,
-    ):
-        recency = self.compute_recency(metadata, date)
-        relevance = self.compute_relevance(memory_embedding, query_embedding)
-        importance = metadata["importance"]
-        return (
-            alpha_recency * recency
-            + alpha_relevance * relevance
-            + alpha_importance * importance
-        )
-
-    @staticmethod
-    def update_last_access(metadata, date):
-        metadata["last_access_timestamp"] = date.strftime("%Y-%m-%d %H:%M:%S")
-        return metadata
-
-    def compute_recency(self, metadata, date):
-        decay_factor = self.decay_factor
-        time_diff = date - datetime.datetime.strptime(
-            metadata["last_access_timestamp"], "%Y-%m-%d %H:%M:%S"
-        )
-        hours_diff = time_diff.total_seconds() / 3600
-        recency = decay_factor**hours_diff
-        return recency
-
-    @staticmethod
-    def compute_relevance(memory_embedding, query_embedding):
-        relevance = 1 - cosine(memory_embedding, query_embedding[0])
-        return relevance
-
-    @staticmethod
-    def normalize_scores(scores):
-        min_score, max_score = np.min(scores), np.max(scores)
-        if min_score == max_score:
-            return np.zeros_like(scores)
-        return (scores - min_score) / (max_score - min_score)
-
-    @staticmethod
-    def get_top_indices(scores, k):
-        return scores.argsort()[-k:][::-1]
+import datetime
+import uuid
+
+import chromadb
+import numpy as np
+from chromadb.utils import embedding_functions
+from scipy.spatial.distance import cosine
+
+
+class RetrievalMemory:
+    def __init__(
+        self,
+        persistent_db_path="./retrieval_memory",
+        embedding_model_name="BAAI/bge-small-en-v1.5",
+        collection_name="retrieval_memory_collection",
+        decay_factor=0.99,
+    ):
+        self.client = chromadb.PersistentClient(path=persistent_db_path)
+        self.sentence_transformer_ef = (
+            embedding_functions.SentenceTransformerEmbeddingFunction(
+                model_name=embedding_model_name
+            )
+        )
+        self.collection = self.client.get_or_create_collection(
+            name=collection_name, embedding_function=self.sentence_transformer_ef
+        )
+        self.decay_factor = decay_factor
+
+    def add_memory(
+        self,
+        description: str,
+        date: datetime.datetime = datetime.datetime.now(),
+        importance: float = 1.0,
+    ):
+        """Add a memory with a given description and importance to the memory stream."""
+        mem = [description]
+        ids = [str(self.generate_unique_id())]
+        metadata = {
+            "memory_id": ids[0],
+            "memory": description,
+            "importance": importance,
+            "creation_timestamp": date.strftime("%Y-%m-%d %H:%M:%S"),
+            "last_access_timestamp": date.strftime("%Y-%m-%d %H:%M:%S"),
+        }
+        self.collection.add(documents=mem, metadatas=metadata, ids=ids)
+
+    def retrieve_memories(
+        self,
+        query: str,
+        k,
+        date=datetime.datetime.now(),
+        alpha_recency=1,
+        alpha_relevance=1,
+        alpha_importance=1,
+    ):
+        query_embedding = self.sentence_transformer_ef([query])
+        query_result = self.collection.query(
+            query_embedding,
+            n_results=k * 4,
+            include=["metadatas", "embeddings", "documents", "distances"],
+        )  # Increase candidate pool size
+        if len(query_result["metadatas"][0]) == 0:
+            return []
+        # Step 2: Apply scoring to the candidate memories
+        scores = []
+        for index in range(len(query_result["metadatas"][0])):
+            scores.append(
+                self.compute_memory_score(
+                    query_result["metadatas"][0][index],
+                    query_result["embeddings"][0][index],
+                    query_embedding,
+                    date,
+                    alpha_recency,
+                    alpha_relevance,
+                    alpha_importance,
+                )
+            )
+
+        # Normalize and select top k memories based on scores
+        normalized_scores = self.normalize_scores(np.array(scores))
+        top_indices = self.get_top_indices(normalized_scores, k)
+        retrieved_memories = [query_result["metadatas"][0][i] for i in top_indices]
+
+        # Update last access time
+        for memory in retrieved_memories:
+            memory = self.update_last_access(memory, date)
+            self.collection.upsert(
+                ids=memory["memory_id"], documents=[memory["memory"]], metadatas=memory
+            )
+        return retrieved_memories
+
+    @staticmethod
+    def generate_unique_id():
+        unique_id = str(uuid.uuid4())
+        return unique_id
+
+    def compute_memory_score(
+        self,
+        metadata,
+        memory_embedding,
+        query_embedding,
+        date,
+        alpha_recency,
+        alpha_relevance,
+        alpha_importance,
+    ):
+        recency = self.compute_recency(metadata, date)
+        relevance = self.compute_relevance(memory_embedding, query_embedding)
+        importance = metadata["importance"]
+        return (
+            alpha_recency * recency
+            + alpha_relevance * relevance
+            + alpha_importance * importance
+        )
+
+    @staticmethod
+    def update_last_access(metadata, date):
+        metadata["last_access_timestamp"] = date.strftime("%Y-%m-%d %H:%M:%S")
+        return metadata
+
+    def compute_recency(self, metadata, date):
+        decay_factor = self.decay_factor
+        time_diff = date - datetime.datetime.strptime(
+            metadata["last_access_timestamp"], "%Y-%m-%d %H:%M:%S"
+        )
+        hours_diff = time_diff.total_seconds() / 3600
+        recency = decay_factor**hours_diff
+        return recency
+
+    @staticmethod
+    def compute_relevance(memory_embedding, query_embedding):
+        relevance = 1 - cosine(memory_embedding, query_embedding[0])
+        return relevance
+
+    @staticmethod
+    def normalize_scores(scores):
+        min_score, max_score = np.min(scores), np.max(scores)
+        if min_score == max_score:
+            return np.zeros_like(scores)
+        return (scores - min_score) / (max_score - min_score)
+
+    @staticmethod
+    def get_top_indices(scores, k):
+        return scores.argsort()[-k:][::-1]
```

### Comparing `llama_cpp_agent-0.1.3/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py` & `llama_cpp_agent-0.1.4/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-import json
-
-from .retrieval_memory import RetrievalMemory
-
-
-class RetrievalMemoryManager:
-    def __init__(self, retrieval_memory: RetrievalMemory):
-        self.retrieval_memory = retrieval_memory
-
-    def add_memory_to_retrieval(self, description: str, importance: float = 1.0) -> str:
-        """
-        Adds a memory with a given description and importance to the memory stream.
-        """
-        self.retrieval_memory.add_memory(description, importance=importance)
-        return f"Information added to archival memory."
-
-    def retrieve_memories(
-        self, query: str, max_results: int = 5, page: int = 1, page_size: int = 5
-    ) -> str:
-        """
-        Retrieves memories from the memory stream based on a query.
-        """
-        memories = self.retrieval_memory.retrieve_memories(query, max_results)
-        # Calculate start and end indices for slicing the memories list for pagination
-        start_index = (page - 1) * page_size
-        end_index = start_index + page_size
-
-        # Slice the list to get the paginated results
-        paginated_memories = memories[start_index:end_index]
-        formatted_memories = ""
-        for memory in paginated_memories:
-            formatted_memories += (
-                f'{memory["creation_timestamp"]}: {memory["memory"]}\n'
-            )
-
-        if formatted_memories != "":
-            formatted_memories += f"\n\nPage {page} of {len(memories) // page_size + 1}"
-        return (
-            formatted_memories
-            if formatted_memories
-            else "No archival memories found matching the query."
-        )
+import json
+
+from .retrieval_memory import RetrievalMemory
+
+
+class RetrievalMemoryManager:
+    def __init__(self, retrieval_memory: RetrievalMemory):
+        self.retrieval_memory = retrieval_memory
+
+    def add_memory_to_retrieval(self, description: str, importance: float = 1.0) -> str:
+        """
+        Adds a memory with a given description and importance to the memory stream.
+        """
+        self.retrieval_memory.add_memory(description, importance=importance)
+        return f"Information added to archival memory."
+
+    def retrieve_memories(
+        self, query: str, max_results: int = 5, page: int = 1, page_size: int = 5
+    ) -> str:
+        """
+        Retrieves memories from the memory stream based on a query.
+        """
+        memories = self.retrieval_memory.retrieve_memories(query, max_results)
+        # Calculate start and end indices for slicing the memories list for pagination
+        start_index = (page - 1) * page_size
+        end_index = start_index + page_size
+
+        # Slice the list to get the paginated results
+        paginated_memories = memories[start_index:end_index]
+        formatted_memories = ""
+        for memory in paginated_memories:
+            formatted_memories += (
+                f'{memory["creation_timestamp"]}: {memory["memory"]}\n'
+            )
+
+        if formatted_memories != "":
+            formatted_memories += f"\n\nPage {page} of {len(memories) // page_size + 1}"
+        return (
+            formatted_memories
+            if formatted_memories
+            else "No archival memories found matching the query."
+        )
```

### Comparing `llama_cpp_agent-0.1.3/src/llama_cpp_agent/chain.py` & `llama_cpp_agent-0.1.4/src/llama_cpp_agent/chain.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,256 +1,253 @@
-from typing import List, Callable
-
-from llama_cpp_agent.function_calling import LlamaCppFunctionTool
-from llama_cpp_agent.llm_agent import LlamaCppAgent
-from llama_cpp_agent.llm_prompt_template import PromptTemplate
-
-
-class AgentChainElement:
-    """
-    Represents a single element in the chain of an agent-based framework. This element holds all necessary data to
-    manage the prompt, process the input/output, and adjust the processing behavior based on given parameters.
-
-    Attributes:
-        output_identifier (str): Unique identifier for the output of this chain element.
-        system_prompt (str): Template string for the system prompt.
-        prompt (str): Template string for the main prompt to the language model.
-        grammar (str, optional): GBNF-Grammar to constrain the language model's output.
-        preprocessor (Callable[[str, str, dict], tuple[str, str, dict]], optional): Function to preprocess the input
-                before sending it to the language model. Takes the system prompt with template fields replaced, the prompt
-                with template fields replaced, and the additional information dictionary as arguments and returns the
-                modified tuple of it.
-        postprocessor (Callable[[str, str, dict, str], str], optional): Function to postprocess the output from
-                the language model. Takes the system prompt, the prompt, the additional information dictionary and the
-                result as arguments and returns the modified result.
-        function_tool_registry (LlamaCppFunctionToolRegistry): Registry for LlamaCppFunctionTool and enables function calling.
-        add_prompt_to_chat_history (bool): Flag to determine if the prompt should be added to the chat history.
-        add_response_to_chat_history (bool): Flag to determine if the response should be added to the chat history.
-        temperature (float): Controls randomness in the generation process. Lower values make responses more deterministic.
-        top_p (float): Controls diversity via nucleus sampling: smaller values make responses more focused.
-        top_k (int): Controls diversity via top-k sampling: the number of highest probability vocabulary tokens considered.
-    Methods:
-        __init__: Constructs an instance of the AgentChain class.
-    """
-
-    def __init__(
-        self,
-        output_identifier: str,
-        system_prompt: str,
-        prompt: str,
-        tools: List[LlamaCppFunctionTool] = None,
-        grammar: str = None,
-        preprocessor: Callable[[str, str, dict], tuple[str, str, dict]] = None,
-        postprocessor: Callable[[str, str, dict, str], str] = None,
-        add_prompt_to_chat_history: bool = False,
-        add_response_to_chat_history: bool = False,
-        temperature: float = 0.35,
-        top_p: float = 1.0,
-        top_k: int = 0,
-    ):
-        """
-        Constructs an instance of the AgentChainElement class.
-
-        Args:
-            output_identifier (str): Unique identifier for the output of this chain element.
-            system_prompt (str): Template string for the system prompt.
-            prompt (str): Template string for the main prompt to the language model.
-            tools (List[LlamaCppFunctionTool], optional): List of function tools available for use in this chain element.
-            grammar (str, optional): GBNF-Grammar to constrain the language model's output.
-            preprocessor (Callable[[str, str, dict], tuple[str, str, dict]], optional): Function to preprocess the input
-                before sending it to the language model. Takes the system prompt with template fields replaced, the prompt
-                with template fields replaced, and the additional information dictionary as arguments and returns the
-                modified tuple of it.
-            postprocessor (Callable[[str, str, dict, str], str], optional): Function to postprocess the output from
-                the language model. Takes the system prompt, the prompt, the additional information dictionary and the
-                result as arguments and returns the modified result.
-            add_prompt_to_chat_history (bool): Flag to determine if the prompt should be added to the chat history.
-            add_response_to_chat_history (bool): Flag to determine if the response should be added to the chat history.
-            temperature (float): Controls randomness in the generation process. Lower values make responses more deterministic.
-            top_p (float): Controls diversity via nucleus sampling: smaller values make responses more focused.
-            top_k (int): Controls diversity via top-k sampling: the number of highest probability vocabulary tokens considered.
-        """
-        self.output_identifier = output_identifier
-        self.system_prompt = system_prompt
-        self.prompt = prompt
-        self.add_prompt_to_chat_history = add_prompt_to_chat_history
-        self.add_response_to_chat_history = add_response_to_chat_history
-        self.grammar = grammar
-        self.preprocessor = preprocessor
-        self.postprocessor = postprocessor
-        self.function_tool_registry = None
-        if tools is not None:
-            self.function_tool_registry = LlamaCppAgent.get_function_tool_registry(
-                tools
-            )
-        self.temperature = temperature
-        self.top_p = top_p
-        self.top_k = top_k
-
-
-class AgentChain:
-    """
-    Represents a chain of AgentChainElements that are processed in a sequence to handle an interaction within an
-    agent-based system.
-
-    Attributes:
-        agent (LlamaCppAgent): The agent responsible for managing and processing the chain.
-        chain (List[AgentChainElement]): A list of AgentChainElement instances that make up the chain.
-
-    Methods:
-        __init__: Constructs an instance of the AgentChain class.
-        run_chain: Processes the entire chain of elements using provided inputs.
-    """
-
-    def __init__(self, agent: LlamaCppAgent, chain_elements: List[AgentChainElement]):
-        """
-        Constructs an instance of the AgentChain class.
-        Args:
-            agent (LlamaCppAgent): The agent responsible for managing and processing the chain.
-            chain_elements (List[AgentChainElement]): A list of AgentChainElement instances that make up the chain.
-        """
-        self.agent = agent
-        self.chain = chain_elements
-
-    def run_chain(self, user_message: str = None, additional_fields: dict = None):
-        """
-        Executes the chain of agent elements using the initial user message and additional fields, and
-        returns the final output and state of the outputs dictionary.
-
-        Args:
-            user_message (str, optional): Initial user message to be processed by the chain.
-            additional_fields (dict, optional): Dictionary of additional data to be used in the processing of the chain.
-
-        Returns:
-            tuple[str, dict]: A tuple containing the concatenated output string from the final element and
-            the dictionary of all outputs.
-        """
-        outputs = {}
-
-        if user_message is not None:
-            outputs["user_message"] = user_message
-
-        if additional_fields is not None:
-            for field, value in additional_fields.items():
-                outputs[field] = value
-
-        for chain_element in self.chain:
-            sys_prompter = PromptTemplate.from_string(chain_element.system_prompt)
-            sys_prompt = sys_prompter.generate_prompt(outputs)
-            prompter = PromptTemplate.from_string(chain_element.prompt)
-            prompt = prompter.generate_prompt(outputs)
-            if chain_element.function_tool_registry is not None:
-                sys_prompt += f"\n\nYou can call functions in JSON format.\n\nAvailable Function Tools:\n\n{chain_element.function_tool_registry.get_documentation()}"
-            if chain_element.preprocessor is not None:
-                sys_prompt, prompt, outputs = chain_element.preprocessor(
-                    sys_prompt, prompt, outputs
-                )
-
-            outputs[chain_element.output_identifier] = self.agent.get_chat_response(
-                prompt,
-                system_prompt=sys_prompt,
-                penalize_nl=False,
-                temperature=chain_element.temperature,
-                top_p=chain_element.top_p,
-                top_k=chain_element.top_k,
-                function_tool_registry=chain_element.function_tool_registry,
-                grammar=chain_element.grammar,
-                add_response_to_chat_history=chain_element.add_response_to_chat_history,
-                add_message_to_chat_history=chain_element.add_prompt_to_chat_history,
-            )
-            if chain_element.function_tool_registry is not None:
-                outputs[chain_element.output_identifier] = outputs[
-                    chain_element.output_identifier
-                ][0]["return_value"]
-            if chain_element.postprocessor is not None:
-                outputs[chain_element.output_identifier] = (
-                    chain_element.postprocessor
-                ) = chain_element.postprocessor(
-                    sys_prompt,
-                    prompt,
-                    outputs,
-                    outputs[chain_element.output_identifier],
-                )
-        output = "\n".join(
-            [val if isinstance(val, str) else str(val) for val in outputs.values()]
-        )
-        return output, outputs
-
-
-class MapChain:
-    """
-    Represents a specialized chain that maps over a list of items and then combines the results using another chain.
-
-    Attributes:
-        agent (LlamaCppAgent): The agent responsible for managing and processing the map and combine chains.
-        map_chain (AgentChain): An AgentChain instance used to process each item in the list.
-        combine_chain (AgentChain): An AgentChain instance used to combine the results of the map chain.
-        item_identifier (str): The identifier used to insert each item into the additional_fields dictionary.
-        map_output_identifier (str): The identifier used to store the results of the map chain before passing to the
-        combine chain.
-
-    Methods:
-        __init__: Constructs an instance of the MapChain class.
-        run_map_chain: Executes the map chain on a list of items and then processes the results with the combine chain.
-    """
-
-    def __init__(
-        self,
-        agent: LlamaCppAgent,
-        map_chain: List[AgentChainElement],
-        combine_chain: List[AgentChainElement],
-        item_identifier: str = "item",
-        map_output_identifier: str = "map_output",
-    ):
-        """
-        Constructs an instance of the MapChain class. This class is designed to process a list of items through
-        a mapping chain and then combine the results using a combining chain.
-
-        Args:
-            agent (LlamaCppAgent): The agent responsible for managing and processing the map and combine chains.
-            map_chain (List[AgentChainElement]): A list of AgentChainElement instances that make up the map chain.
-            combine_chain (List[AgentChainElement]): A list of AgentChainElement instances that make up the combine chain.
-            item_identifier (str, optional): The identifier used to insert each item into the additional_fields dictionary.
-            map_output_identifier (str, optional): The identifier used to store the results of the map chain before passing to the combine chain.
-        """
-        self.agent = agent
-        self.map_chain = AgentChain(agent, map_chain)
-        self.combine_chain = AgentChain(agent, combine_chain)
-        self.item_identifier = item_identifier
-        self.map_output_identifier = map_output_identifier
-
-    def run_map_chain(
-        self,
-        items_to_map: list[str],
-        user_message: str = None,
-        additional_fields: dict = None,
-    ):
-        """
-        Executes the map chain over a list of items and then uses the combine chain to process the concatenated
-        results.
-
-        Args:
-            items_to_map (list[str]): List of strings to be individually processed by the map chain.
-            user_message (str, optional): Initial user message to be included in the processing.
-            additional_fields (dict, optional): Additional data to be used throughout the map and combine chains.
-
-        Returns:
-            tuple: A tuple containing the final output string from the combine chain and the outputs dictionary.
-        """
-        outputs = {}
-        if user_message is not None:
-            outputs["user_message"] = user_message
-
-        if additional_fields is not None:
-            for field, value in additional_fields.items():
-                outputs[field] = value
-        else:
-            additional_fields = {}
-        results = []
-        for item in items_to_map:
-            additional_fields[self.item_identifier] = item
-            result, result_dic = self.map_chain.run_chain(
-                additional_fields=additional_fields
-            )
-            results.append(result_dic[self.map_chain.chain[-1].output_identifier])
-        additional_fields[self.map_output_identifier] = "\n\n".join(results)
-        return self.combine_chain.run_chain(additional_fields=additional_fields)
+from typing import List, Callable
+
+from llama_cpp_agent.function_calling import LlamaCppFunctionTool
+from llama_cpp_agent.llm_agent import LlamaCppAgent
+from llama_cpp_agent.llm_prompt_template import PromptTemplate
+
+
+class AgentChainElement:
+    """
+    Represents a single element in the chain of an agent-based framework. This element holds all necessary data to
+    manage the prompt, process the input/output, and adjust the processing behavior based on given parameters.
+
+    Attributes:
+        output_identifier (str): Unique identifier for the output of this chain element.
+        system_prompt (str): Template string for the system prompt.
+        prompt (str): Template string for the main prompt to the language model.
+        grammar (str, optional): GBNF-Grammar to constrain the language model's output.
+        preprocessor (Callable[[str, str, dict], tuple[str, str, dict]], optional): Function to preprocess the input
+                before sending it to the language model. Takes the system prompt with template fields replaced, the prompt
+                with template fields replaced, and the additional information dictionary as arguments and returns the
+                modified tuple of it.
+        postprocessor (Callable[[str, str, dict, str], str], optional): Function to postprocess the output from
+                the language model. Takes the system prompt, the prompt, the additional information dictionary and the
+                result as arguments and returns the modified result.
+        function_tool_registry (LlamaCppFunctionToolRegistry): Registry for LlamaCppFunctionTool and enables function calling.
+        add_prompt_to_chat_history (bool): Flag to determine if the prompt should be added to the chat history.
+        add_response_to_chat_history (bool): Flag to determine if the response should be added to the chat history.
+        temperature (float): Controls randomness in the generation process. Lower values make responses more deterministic.
+        top_p (float): Controls diversity via nucleus sampling: smaller values make responses more focused.
+        top_k (int): Controls diversity via top-k sampling: the number of highest probability vocabulary tokens considered.
+    Methods:
+        __init__: Constructs an instance of the AgentChain class.
+    """
+
+    def __init__(
+        self,
+        output_identifier: str,
+        system_prompt: str,
+        prompt: str,
+        tools: List[LlamaCppFunctionTool] = None,
+        grammar: str = None,
+        preprocessor: Callable[[str, str, dict], tuple[str, str, dict]] = None,
+        postprocessor: Callable[[str, str, dict, str], str] = None,
+        add_prompt_to_chat_history: bool = False,
+        add_response_to_chat_history: bool = False,
+        temperature: float = 0.35,
+        top_p: float = 1.0,
+        top_k: int = 0,
+    ):
+        """
+        Constructs an instance of the AgentChainElement class.
+
+        Args:
+            output_identifier (str): Unique identifier for the output of this chain element.
+            system_prompt (str): Template string for the system prompt.
+            prompt (str): Template string for the main prompt to the language model.
+            tools (List[LlamaCppFunctionTool], optional): List of function tools available for use in this chain element.
+            grammar (str, optional): GBNF-Grammar to constrain the language model's output.
+            preprocessor (Callable[[str, str, dict], tuple[str, str, dict]], optional): Function to preprocess the input
+                before sending it to the language model. Takes the system prompt with template fields replaced, the prompt
+                with template fields replaced, and the additional information dictionary as arguments and returns the
+                modified tuple of it.
+            postprocessor (Callable[[str, str, dict, str], str], optional): Function to postprocess the output from
+                the language model. Takes the system prompt, the prompt, the additional information dictionary and the
+                result as arguments and returns the modified result.
+            add_prompt_to_chat_history (bool): Flag to determine if the prompt should be added to the chat history.
+            add_response_to_chat_history (bool): Flag to determine if the response should be added to the chat history.
+            temperature (float): Controls randomness in the generation process. Lower values make responses more deterministic.
+            top_p (float): Controls diversity via nucleus sampling: smaller values make responses more focused.
+            top_k (int): Controls diversity via top-k sampling: the number of highest probability vocabulary tokens considered.
+        """
+        self.output_identifier = output_identifier
+        self.system_prompt = system_prompt
+        self.prompt = prompt
+        self.add_prompt_to_chat_history = add_prompt_to_chat_history
+        self.add_response_to_chat_history = add_response_to_chat_history
+        self.grammar = grammar
+        self.preprocessor = preprocessor
+        self.postprocessor = postprocessor
+        self.function_tool_registry = None
+        if tools is not None:
+            self.function_tool_registry = LlamaCppAgent.get_function_tool_registry(
+                tools
+            )
+        self.temperature = temperature
+        self.top_p = top_p
+        self.top_k = top_k
+
+
+class AgentChain:
+    """
+    Represents a chain of AgentChainElements that are processed in a sequence to handle an interaction within an
+    agent-based system.
+
+    Attributes:
+        agent (LlamaCppAgent): The agent responsible for managing and processing the chain.
+        chain (List[AgentChainElement]): A list of AgentChainElement instances that make up the chain.
+
+    Methods:
+        __init__: Constructs an instance of the AgentChain class.
+        run_chain: Processes the entire chain of elements using provided inputs.
+    """
+
+    def __init__(self, agent: LlamaCppAgent, chain_elements: List[AgentChainElement]):
+        """
+        Constructs an instance of the AgentChain class.
+        Args:
+            agent (LlamaCppAgent): The agent responsible for managing and processing the chain.
+            chain_elements (List[AgentChainElement]): A list of AgentChainElement instances that make up the chain.
+        """
+        self.agent = agent
+        self.chain = chain_elements
+
+    def run_chain(self, user_message: str = None, additional_fields: dict = None):
+        """
+        Executes the chain of agent elements using the initial user message and additional fields, and
+        returns the final output and state of the outputs dictionary.
+
+        Args:
+            user_message (str, optional): Initial user message to be processed by the chain.
+            additional_fields (dict, optional): Dictionary of additional data to be used in the processing of the chain.
+
+        Returns:
+            tuple[str, dict]: A tuple containing the concatenated output string from the final element and
+            the dictionary of all outputs.
+        """
+        outputs = {}
+
+        if additional_fields is not None:
+            for field, value in additional_fields.items():
+                outputs[field] = value
+
+        for chain_element in self.chain:
+            sys_prompter = PromptTemplate.from_string(chain_element.system_prompt)
+            sys_prompt = sys_prompter.generate_prompt(outputs)
+            prompter = PromptTemplate.from_string(chain_element.prompt)
+            prompt = prompter.generate_prompt(outputs)
+            if chain_element.function_tool_registry is not None:
+                sys_prompt += f"\n\nYou can call functions in JSON format.\n\nAvailable Function Tools:\n\n{chain_element.function_tool_registry.get_documentation().strip()}"
+            if chain_element.preprocessor is not None:
+                sys_prompt, prompt, outputs = chain_element.preprocessor(
+                    sys_prompt, prompt, outputs
+                )
+
+            outputs[chain_element.output_identifier] = self.agent.get_chat_response(
+                user_message if user_message is not None else prompt,
+                system_prompt=sys_prompt,
+                penalize_nl=False,
+                temperature=chain_element.temperature,
+                top_p=chain_element.top_p,
+                top_k=chain_element.top_k,
+                function_tool_registry=chain_element.function_tool_registry,
+                grammar=chain_element.grammar,
+                add_response_to_chat_history=chain_element.add_response_to_chat_history,
+                add_message_to_chat_history=chain_element.add_prompt_to_chat_history,
+            )
+            if chain_element.function_tool_registry is not None:
+                outputs[chain_element.output_identifier] = outputs[
+                    chain_element.output_identifier
+                ][0]["return_value"]
+            if chain_element.postprocessor is not None:
+                outputs[chain_element.output_identifier] = (
+                    chain_element.postprocessor
+                ) = chain_element.postprocessor(
+                    sys_prompt,
+                    prompt,
+                    outputs,
+                    outputs[chain_element.output_identifier],
+                )
+        output = "\n".join(
+            [val if isinstance(val, str) else str(val) for val in outputs.values()]
+        )
+        return output, outputs
+
+
+class MapChain:
+    """
+    Represents a specialized chain that maps over a list of items and then combines the results using another chain.
+
+    Attributes:
+        agent (LlamaCppAgent): The agent responsible for managing and processing the map and combine chains.
+        map_chain (AgentChain): An AgentChain instance used to process each item in the list.
+        combine_chain (AgentChain): An AgentChain instance used to combine the results of the map chain.
+        item_identifier (str): The identifier used to insert each item into the additional_fields dictionary.
+        map_output_identifier (str): The identifier used to store the results of the map chain before passing to the
+        combine chain.
+
+    Methods:
+        __init__: Constructs an instance of the MapChain class.
+        run_map_chain: Executes the map chain on a list of items and then processes the results with the combine chain.
+    """
+
+    def __init__(
+        self,
+        agent: LlamaCppAgent,
+        map_chain: List[AgentChainElement],
+        combine_chain: List[AgentChainElement],
+        item_identifier: str = "item",
+        map_output_identifier: str = "map_output",
+    ):
+        """
+        Constructs an instance of the MapChain class. This class is designed to process a list of items through
+        a mapping chain and then combine the results using a combining chain.
+
+        Args:
+            agent (LlamaCppAgent): The agent responsible for managing and processing the map and combine chains.
+            map_chain (List[AgentChainElement]): A list of AgentChainElement instances that make up the map chain.
+            combine_chain (List[AgentChainElement]): A list of AgentChainElement instances that make up the combine chain.
+            item_identifier (str, optional): The identifier used to insert each item into the additional_fields dictionary.
+            map_output_identifier (str, optional): The identifier used to store the results of the map chain before passing to the combine chain.
+        """
+        self.agent = agent
+        self.map_chain = AgentChain(agent, map_chain)
+        self.combine_chain = AgentChain(agent, combine_chain)
+        self.item_identifier = item_identifier
+        self.map_output_identifier = map_output_identifier
+
+    def run_map_chain(
+        self,
+        items_to_map: list[str],
+        user_message: str = None,
+        additional_fields: dict = None,
+    ):
+        """
+        Executes the map chain over a list of items and then uses the combine chain to process the concatenated
+        results.
+
+        Args:
+            items_to_map (list[str]): List of strings to be individually processed by the map chain.
+            user_message (str, optional): Initial user message to be included in the processing.
+            additional_fields (dict, optional): Additional data to be used throughout the map and combine chains.
+
+        Returns:
+            tuple: A tuple containing the final output string from the combine chain and the outputs dictionary.
+        """
+        outputs = {}
+        if user_message is not None:
+            outputs["user_message"] = user_message
+
+        if additional_fields is not None:
+            for field, value in additional_fields.items():
+                outputs[field] = value
+        else:
+            additional_fields = {}
+        results = []
+        for item in items_to_map:
+            additional_fields[self.item_identifier] = item
+            result, result_dic = self.map_chain.run_chain(
+                additional_fields=additional_fields
+            )
+            results.append(result_dic[self.map_chain.chain[-1].output_identifier])
+        additional_fields[self.map_output_identifier] = "\n\n".join(results)
+        return self.combine_chain.run_chain(additional_fields=additional_fields)
```

### Comparing `llama_cpp_agent-0.1.3/src/llama_cpp_agent/function_calling_agent.py` & `llama_cpp_agent-0.1.4/src/llama_cpp_agent/function_calling_agent.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,434 +1,434 @@
-import datetime
-import json
-import os
-from copy import copy
-from typing import Type, List, Callable, Union, Literal
-
-from llama_cpp import Llama
-from pydantic import BaseModel, Field
-
-from .llm_settings import LlamaLLMGenerationSettings, LlamaLLMSettings
-from .llm_agent import LlamaCppAgent, StreamingResponse
-from .messages_formatter import MessagesFormatterType, MessagesFormatter
-from .function_calling import LlamaCppFunctionTool
-from .gbnf_grammar_generator.gbnf_grammar_from_pydantic_models import (
-    create_dynamic_model_from_function,
-    create_dynamic_models_from_dictionaries,
-    add_run_method_to_dynamic_model,
-)
-from .providers.llama_cpp_endpoint_provider import (
-    LlamaCppGenerationSettings,
-    LlamaCppEndpointSettings,
-)
-from .providers.openai_endpoint_provider import (
-    OpenAIGenerationSettings,
-    OpenAIEndpointSettings,
-)
-
-
-class activate_message_mode(BaseModel):
-    """
-    Activates message mode.
-    """
-
-    def run(self, agent: "FunctionCallingAgent"):
-        agent.without_grammar_mode = True
-        agent.prompt_suffix = "\nWrite message in plain text format:"
-        agent.without_grammar_mode_function.append(agent.send_message_to_user)
-        return True
-
-
-class send_message(BaseModel):
-    """
-    Sends a message to the user.
-    """
-
-    content: str = Field(..., description="Content of the message to be sent.")
-
-    def run(self, agent: "FunctionCallingAgent"):
-        agent.send_message_to_user(self.content)
-        return "Message sent."
-
-
-class write_text_file(BaseModel):
-    """
-    Writes content to a file.
-    """
-
-    file_path: str = Field(..., description="The path to the file.")
-    content: str = Field(..., description="The content to write to the file.")
-
-    def run(self, agent: "FunctionCallingAgent"):
-        self.write_file(self.content)
-        return True
-
-    def write_file(self, content: str):
-        """
-        Write content to a file.
-
-        Args:
-            content (str): The content to write to the file.
-        """
-        with open(self.file_path, "w", encoding="utf-8") as file:
-            file.write(content)
-        return None
-
-
-class read_text_file(BaseModel):
-    """
-    Reads the content of a file.
-    """
-
-    file_path: str = Field(..., description="The path to the file.")
-
-    def run(self):
-        return self.read_file()
-
-    def read_file(self):
-        """
-        Reads the content of a file.
-        """
-        if os.path.exists(self.file_path):
-            with open(self.file_path, "r", encoding="utf-8") as file:
-                return file.read()
-        else:
-            return f"File not found."
-
-
-class FunctionCallingAgent:
-    """
-    An agent that uses function calling to interact with its environment and the user.
-
-    Args:
-        llama_llm (Llama | LlamaLLMSettings | LlamaCppEndpointSettings | OpenAIEndpointSettings): An instance of Llama, LlamaLLMSettings, LlamaCppEndpointSettings or LlamaCppServerLLMSettings as LLM.
-        llama_generation_settings (LlamaLLMGenerationSettings | LlamaCppGenerationSettings | OpenAIGenerationSettings): Generation settings for Llama.
-        messages_formatter_type (MessagesFormatterType): Type of messages formatter.
-        custom_messages_formatter (MessagesFormatter): Optional Custom messages formatter.
-        streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
-        k_last_messages_from_chat_history (int): Number of last messages to consider from chat history.
-        system_prompt (str): System prompt for interaction.
-        llama_cpp_function_tools(List[LlamaCppFunctionTool]): List of LlamaCppFunctionTool instances.
-        allow_parallel_function_calling (bool): Allow parallel function calling (Default=False)
-        add_send_message_to_user_function (bool): Flag to add send_message_to_user function.
-        send_message_to_user_callback (Callable[[str], None]): Callback for sending a message to the user.
-        debug_output (bool): Enable debug output.
-
-    Attributes:
-        send_message_to_user_callback (Callable[[str], None]): Callback for sending a message to the user.
-        llama_cpp_tools (List[LlamaCppFunctionTool]): List of LlamaCppFunctionTool instances.
-        tool_registry (LlamaCppFunctionToolRegistry): Function tool registry.
-        llama_generation_settings (LlamaLLMGenerationSettings): Generation settings for Llama.
-        system_prompt (str): System prompt for interaction.
-        llama_cpp_agent (LlamaCppAgent): LlamaCppAgent instance for interaction.
-        k_last_messages_from_chat_history (int): Number of last messages to consider from chat history.
-        streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
-
-    Methods:
-        save(file_path: str): Save the agent's state to a file.
-        load_from_file(file_path: str, llama_llm, python_functions, pydantic_functions, send_message_to_user_callback, streaming_callback) -> FunctionCallingAgent:
-            Load the agent's state from a file.
-        load_from_dict(agent_dict: dict) -> FunctionCallingAgent: Load the agent's state from a dictionary.
-        as_dict() -> dict: Convert the agent's state to a dictionary.
-        generate_response(message: str): Generate a response based on the input message.
-        send_message_to_user(message: str): Send a message to the user.
-
-    """
-
-    def __init__(
-        self,
-        llama_llm: Union[
-            Llama, LlamaLLMSettings, LlamaCppEndpointSettings, OpenAIEndpointSettings
-        ],
-        llama_generation_settings: Union[
-            LlamaLLMGenerationSettings,
-            LlamaCppGenerationSettings,
-            OpenAIGenerationSettings,
-        ] = None,
-        messages_formatter_type: MessagesFormatterType = MessagesFormatterType.CHATML,
-        custom_messages_formatter: MessagesFormatter = None,
-        streaming_callback: Callable[[StreamingResponse], None] = None,
-        k_last_messages_from_chat_history: int = 0,
-        system_prompt: str = None,
-        llama_cpp_function_tools: [LlamaCppFunctionTool] = None,
-        basic_file_tools: bool = False,
-        allow_parallel_function_calling=False,
-        add_send_message_to_user_function: bool = True,
-        send_message_to_user_callback: Callable[[str], None] = None,
-        debug_output: bool = False,
-    ):
-        """
-        Initialize the FunctionCallingAgent.
-
-        Args:
-            llama_llm (Llama | LlamaLLMSettings | LlamaCppEndpointSettings | OpenAIEndpointSettings): An instance of Llama, LlamaLLMSettings, LlamaCppEndpointSettings or LlamaCppServerLLMSettings as LLM.
-            llama_generation_settings (LlamaLLMGenerationSettings | LlamaCppGenerationSettings | OpenAIGenerationSettings): Generation settings for Llama.
-            messages_formatter_type (MessagesFormatterType): Type of messages formatter.
-            custom_messages_formatter (MessagesFormatter): Optional Custom messages formatter.
-            streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
-            k_last_messages_from_chat_history (int): Number of last messages to consider from chat history.
-            system_prompt (str): System prompt for interaction.
-            llama_cpp_function_tools(List[LlamaCppFunctionTool]): List of LlamaCppFunctionTool instances.
-            allow_parallel_function_calling (bool): Allow parallel function calling (Default=False)
-            add_send_message_to_user_function (bool): Flag to add send_message_to_user function.
-            send_message_to_user_callback (Callable[[str], None]): Callback for sending a message to the user.
-            debug_output (bool): Enable debug output.
-        """
-        self.llama_cpp_tools = []
-        if llama_cpp_function_tools:
-            self.llama_cpp_tools = llama_cpp_function_tools
-
-        self.send_message_to_user_callback = send_message_to_user_callback
-        if add_send_message_to_user_function:
-            self.llama_cpp_tools.append(LlamaCppFunctionTool(send_message, agent=self))
-
-        if basic_file_tools:
-            self.llama_cpp_tools.append(LlamaCppFunctionTool(read_text_file))
-            self.llama_cpp_tools.append(
-                LlamaCppFunctionTool(write_text_file, agent=self)
-            )
-
-        self.tool_registry = LlamaCppAgent.get_function_tool_registry(
-            self.llama_cpp_tools,
-            add_inner_thoughts=True,
-            allow_inner_thoughts_only=False,
-            allow_parallel_function_calling=allow_parallel_function_calling,
-        )
-
-        if llama_generation_settings is None:
-            if isinstance(llama_llm, Llama) or isinstance(llama_llm, LlamaLLMSettings):
-                llama_generation_settings = LlamaLLMGenerationSettings()
-            elif isinstance(llama_llm, OpenAIEndpointSettings):
-                llama_generation_settings = OpenAIGenerationSettings()
-            else:
-                llama_generation_settings = LlamaCppGenerationSettings()
-
-        if isinstance(
-            llama_generation_settings, LlamaLLMGenerationSettings
-        ) and isinstance(llama_llm, LlamaCppEndpointSettings):
-            raise Exception(
-                "Wrong generation settings for llama.cpp server endpoint, use LlamaCppServerGenerationSettings under llama_cpp_agent.providers.llama_cpp_server_provider!"
-            )
-        if (
-            isinstance(llama_llm, Llama) or isinstance(llama_llm, LlamaLLMSettings)
-        ) and isinstance(llama_generation_settings, LlamaCppGenerationSettings):
-            raise Exception(
-                "Wrong generation settings for llama-cpp-python, use LlamaLLMGenerationSettings under llama_cpp_agent.llm_settings!"
-            )
-
-        if isinstance(llama_llm, OpenAIEndpointSettings) and not isinstance(
-            llama_generation_settings, OpenAIGenerationSettings
-        ):
-            raise Exception(
-                "Wrong generation settings for OpenAI endpoint, use OpenAIGenerationSettings under llama_cpp_agent.providers.openai_endpoint_provider!"
-            )
-
-        self.llama_generation_settings = llama_generation_settings
-
-        self.without_grammar_mode = False
-        self.without_grammar_mode_function = []
-        self.prompt_suffix = ""
-        if system_prompt is not None:
-            self.system_prompt = system_prompt
-        else:
-            # You can also request to return control back to you after a function call is executed by setting the 'return_control' flag in a function call object.
-            self.system_prompt = (
-                """You are Funky, an AI assistant that calls functions to perform tasks.
-
-To call functions, you respond with a JSON object containing three fields:
-"thoughts_and_reasoning": Your thoughts and reasoning behind the function call.
-"function": The name of the function you want to call.
-"parameters": The arguments required for the function.
-
-After performing a function call, you will receive a response containing the return values of the function calls.
-
-### Functions:
-Below is a list of functions you can use to interact with the system. Each function has specific parameters and requirements. Make sure to follow the instructions for each function carefully.
-Choose the appropriate function based on the task you want to perform. Provide your function calls in JSON format.
-
-"""
-                + self.tool_registry.get_documentation().strip()
-            )
-        self.llama_cpp_agent = LlamaCppAgent(
-            llama_llm,
-            debug_output=debug_output,
-            system_prompt="",
-            predefined_messages_formatter_type=messages_formatter_type,
-            custom_messages_formatter=custom_messages_formatter,
-        )
-
-        self.k_last_messages_from_chat_history = k_last_messages_from_chat_history
-        self.streaming_callback = streaming_callback
-
-    def save(self, file_path: str):
-        """
-        Save the agent's state to a file.
-
-        Args:
-            file_path (str): The path to the file.
-        """
-        with open(file_path, "w", encoding="utf-8") as file:
-            dic = copy(self.as_dict())
-            del dic["llama_cpp_agent"]
-            del dic["streaming_callback"]
-            del dic["tool_registry"]
-            del dic["llama_cpp_tools"]
-            del dic["send_message_to_user_callback"]
-            del dic["without_grammar_mode_function"]
-            dic["debug_output"] = self.llama_cpp_agent.debug_output
-            dic["messages"] = self.llama_cpp_agent.messages
-            dic["llama_generation_settings"] = self.llama_generation_settings.as_dict()
-            dic["custom_messages_formatter"] = (
-                self.llama_cpp_agent.messages_formatter.as_dict()
-            )
-            json.dump(dic, file, indent=4)
-
-    @staticmethod
-    def load_from_file(
-        file_path: str,
-        llama_llm: Union[Llama, LlamaLLMSettings],
-        open_ai_functions: (List[dict], List[Callable]) = None,
-        python_functions: List[Callable] = None,
-        pydantic_functions: List[Type[BaseModel]] = None,
-        send_message_to_user_callback: Callable[[str], None] = None,
-        streaming_callback: Callable[[StreamingResponse], None] = None,
-    ) -> "FunctionCallingAgent":
-        """
-        Load the agent's state from a file.
-
-        Args:
-            file_path (str): The path to the file.
-            llama_llm: LLM to use
-            open_ai_functions (Tuple[List[dict], List[Callable]]): OpenAI function definitions, and a list of the actual functions as tuple.
-            python_functions (List[Callable]): Python functions for interaction.
-            pydantic_functions (List[Type[BaseModel]]): Pydantic models representing functions.
-            send_message_to_user_callback (Callable[[str], None]): Callback for sending a message to the user.
-            streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
-
-        Returns:
-            FunctionCallingAgent: The loaded FunctionCallingAgent instance.
-        """
-
-        with open(file_path, "r", encoding="utf-8") as file:
-            loaded_agent = json.load(file)
-            loaded_agent["llama_llm"] = llama_llm
-            loaded_agent["streaming_callback"] = streaming_callback
-            loaded_agent["python_functions"] = python_functions
-            loaded_agent["pydantic_functions"] = pydantic_functions
-            loaded_agent["open_ai_functions"] = open_ai_functions
-            messages = copy(loaded_agent["messages"])
-            del loaded_agent["messages"]
-            loaded_agent["send_message_to_user_callback"] = (
-                send_message_to_user_callback
-            )
-            loaded_agent["llama_generation_settings"] = (
-                LlamaLLMGenerationSettings.load_from_dict(
-                    loaded_agent["llama_generation_settings"]
-                )
-            )
-            loaded_agent["custom_messages_formatter"] = (
-                MessagesFormatter.load_from_dict(
-                    loaded_agent["custom_messages_formatter"]
-                )
-            )
-            agent = FunctionCallingAgent(**loaded_agent)
-
-            agent.llama_cpp_agent.messages = messages
-            return agent
-
-    @staticmethod
-    def load_from_dict(agent_dict: dict) -> "FunctionCallingAgent":
-        """
-        Load the agent's state from a dictionary.
-
-        Args:
-            agent_dict (dict): The dictionary containing the agent's state.
-
-        Returns:
-            FunctionCallingAgent: The loaded FunctionCallingAgent instance.
-        """
-        return FunctionCallingAgent(**agent_dict)
-
-    def as_dict(self) -> dict:
-        """
-        Convert the agent's state to a dictionary.
-
-        Returns:
-           dict: The dictionary representation of the agent's state.
-        """
-        return self.__dict__
-
-    def generate_response(
-        self, message: str, additional_stop_sequences: List[str] = None
-    ):
-        self.llama_cpp_agent.add_message(role="user", message=message)
-
-        result = self.intern_get_response(
-            additional_stop_sequences=additional_stop_sequences
-        )
-
-        while True:
-            if isinstance(result, str):
-                if len(self.without_grammar_mode_function) > 0:
-                    func_list = []
-                    for func in self.without_grammar_mode_function:
-                        if func.__name__ not in func_list:
-                            func(result.strip())
-                            func_list.append(func.__name__)
-                break
-            function_message = f"""Function Calling Results:\n\n"""
-            count = 0
-            if result is not None:
-                agent_sent_message = False
-                for res in result:
-                    count += 1
-                    if res["function"] == "send_message":
-                        agent_sent_message = True
-                    if not isinstance(res, str):
-                        if "params" in res:
-                            function_message += f"""{count}. Function: "{res["function"]}"\nArguments: "{res["params"]}"\nReturn Value: {res["return_value"]}\n\n"""
-                        else:
-                            function_message += f"""{count}. Function: "{res["function"]}"\nReturn Value: {res["return_value"]}\n\n"""
-                    else:
-                        function_message += f"{count}. " + res + "\n\n"
-                self.llama_cpp_agent.add_message(
-                    role="function", message=function_message.strip()
-                )
-                if agent_sent_message:
-                    break
-            result = self.intern_get_response(
-                additional_stop_sequences=additional_stop_sequences
-            )
-        return result
-
-    def intern_get_response(self, additional_stop_sequences: List[str] = None):
-        without_grammar_mode = False
-        if self.without_grammar_mode:
-            without_grammar_mode = True
-            self.without_grammar_mode = False
-        if additional_stop_sequences is None:
-            additional_stop_sequences = []
-        additional_stop_sequences.append("(End of message)")
-        result = self.llama_cpp_agent.get_chat_response(
-            system_prompt=self.system_prompt,
-            streaming_callback=self.streaming_callback,
-            function_tool_registry=(
-                self.tool_registry if not without_grammar_mode else None
-            ),
-            additional_stop_sequences=additional_stop_sequences,
-            **self.llama_generation_settings.as_dict(),
-        )
-        if without_grammar_mode:
-            self.prompt_suffix = ""
-        return result
-
-    def send_message_to_user(self, message: str):
-        """
-        Send a message to the user.
-
-        Args:
-            message: The message send to the user.
-        """
-        if self.send_message_to_user_callback:
-            self.send_message_to_user_callback(message)
-        else:
-            print(message)
+import datetime
+import json
+import os
+from copy import copy
+from typing import Type, List, Callable, Union, Literal
+
+from llama_cpp import Llama
+from pydantic import BaseModel, Field
+
+from .llm_settings import LlamaLLMGenerationSettings, LlamaLLMSettings
+from .llm_agent import LlamaCppAgent, StreamingResponse
+from .messages_formatter import MessagesFormatterType, MessagesFormatter
+from .function_calling import LlamaCppFunctionTool
+from .gbnf_grammar_generator.gbnf_grammar_from_pydantic_models import (
+    create_dynamic_model_from_function,
+    create_dynamic_models_from_dictionaries,
+    add_run_method_to_dynamic_model,
+)
+from .providers.llama_cpp_endpoint_provider import (
+    LlamaCppGenerationSettings,
+    LlamaCppEndpointSettings,
+)
+from .providers.openai_endpoint_provider import (
+    OpenAIGenerationSettings,
+    OpenAIEndpointSettings,
+)
+
+
+class activate_message_mode(BaseModel):
+    """
+    Activates message mode.
+    """
+
+    def run(self, agent: "FunctionCallingAgent"):
+        agent.without_grammar_mode = True
+        agent.prompt_suffix = "\nWrite message in plain text format:"
+        agent.without_grammar_mode_function.append(agent.send_message_to_user)
+        return True
+
+
+class send_message(BaseModel):
+    """
+    Sends a message to the user.
+    """
+
+    content: str = Field(..., description="Content of the message to be sent.")
+
+    def run(self, agent: "FunctionCallingAgent"):
+        agent.send_message_to_user(self.content)
+        return "Message sent."
+
+
+class write_text_file(BaseModel):
+    """
+    Writes content to a file.
+    """
+
+    file_path: str = Field(..., description="The path to the file.")
+    content: str = Field(..., description="The content to write to the file.")
+
+    def run(self, agent: "FunctionCallingAgent"):
+        self.write_file(self.content)
+        return True
+
+    def write_file(self, content: str):
+        """
+        Write content to a file.
+
+        Args:
+            content (str): The content to write to the file.
+        """
+        with open(self.file_path, "w", encoding="utf-8") as file:
+            file.write(content)
+        return None
+
+
+class read_text_file(BaseModel):
+    """
+    Reads the content of a file.
+    """
+
+    file_path: str = Field(..., description="The path to the file.")
+
+    def run(self):
+        return self.read_file()
+
+    def read_file(self):
+        """
+        Reads the content of a file.
+        """
+        if os.path.exists(self.file_path):
+            with open(self.file_path, "r", encoding="utf-8") as file:
+                return file.read()
+        else:
+            return f"File not found."
+
+
+class FunctionCallingAgent:
+    """
+    An agent that uses function calling to interact with its environment and the user.
+
+    Args:
+        llama_llm (Llama | LlamaLLMSettings | LlamaCppEndpointSettings | OpenAIEndpointSettings): An instance of Llama, LlamaLLMSettings, LlamaCppEndpointSettings or LlamaCppServerLLMSettings as LLM.
+        llama_generation_settings (LlamaLLMGenerationSettings | LlamaCppGenerationSettings | OpenAIGenerationSettings): Generation settings for Llama.
+        messages_formatter_type (MessagesFormatterType): Type of messages formatter.
+        custom_messages_formatter (MessagesFormatter): Optional Custom messages formatter.
+        streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
+        k_last_messages_from_chat_history (int): Number of last messages to consider from chat history.
+        system_prompt (str): System prompt for interaction.
+        llama_cpp_function_tools(List[LlamaCppFunctionTool]): List of LlamaCppFunctionTool instances.
+        allow_parallel_function_calling (bool): Allow parallel function calling (Default=False)
+        add_send_message_to_user_function (bool): Flag to add send_message_to_user function.
+        send_message_to_user_callback (Callable[[str], None]): Callback for sending a message to the user.
+        debug_output (bool): Enable debug output.
+
+    Attributes:
+        send_message_to_user_callback (Callable[[str], None]): Callback for sending a message to the user.
+        llama_cpp_tools (List[LlamaCppFunctionTool]): List of LlamaCppFunctionTool instances.
+        tool_registry (LlamaCppFunctionToolRegistry): Function tool registry.
+        llama_generation_settings (LlamaLLMGenerationSettings): Generation settings for Llama.
+        system_prompt (str): System prompt for interaction.
+        llama_cpp_agent (LlamaCppAgent): LlamaCppAgent instance for interaction.
+        k_last_messages_from_chat_history (int): Number of last messages to consider from chat history.
+        streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
+
+    Methods:
+        save(file_path: str): Save the agent's state to a file.
+        load_from_file(file_path: str, llama_llm, python_functions, pydantic_functions, send_message_to_user_callback, streaming_callback) -> FunctionCallingAgent:
+            Load the agent's state from a file.
+        load_from_dict(agent_dict: dict) -> FunctionCallingAgent: Load the agent's state from a dictionary.
+        as_dict() -> dict: Convert the agent's state to a dictionary.
+        generate_response(message: str): Generate a response based on the input message.
+        send_message_to_user(message: str): Send a message to the user.
+
+    """
+
+    def __init__(
+        self,
+        llama_llm: Union[
+            Llama, LlamaLLMSettings, LlamaCppEndpointSettings, OpenAIEndpointSettings
+        ],
+        llama_generation_settings: Union[
+            LlamaLLMGenerationSettings,
+            LlamaCppGenerationSettings,
+            OpenAIGenerationSettings,
+        ] = None,
+        messages_formatter_type: MessagesFormatterType = MessagesFormatterType.CHATML,
+        custom_messages_formatter: MessagesFormatter = None,
+        streaming_callback: Callable[[StreamingResponse], None] = None,
+        k_last_messages_from_chat_history: int = 0,
+        system_prompt: str = None,
+        llama_cpp_function_tools: [LlamaCppFunctionTool] = None,
+        basic_file_tools: bool = False,
+        allow_parallel_function_calling=False,
+        add_send_message_to_user_function: bool = True,
+        send_message_to_user_callback: Callable[[str], None] = None,
+        debug_output: bool = False,
+    ):
+        """
+        Initialize the FunctionCallingAgent.
+
+        Args:
+            llama_llm (Llama | LlamaLLMSettings | LlamaCppEndpointSettings | OpenAIEndpointSettings): An instance of Llama, LlamaLLMSettings, LlamaCppEndpointSettings or LlamaCppServerLLMSettings as LLM.
+            llama_generation_settings (LlamaLLMGenerationSettings | LlamaCppGenerationSettings | OpenAIGenerationSettings): Generation settings for Llama.
+            messages_formatter_type (MessagesFormatterType): Type of messages formatter.
+            custom_messages_formatter (MessagesFormatter): Optional Custom messages formatter.
+            streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
+            k_last_messages_from_chat_history (int): Number of last messages to consider from chat history.
+            system_prompt (str): System prompt for interaction.
+            llama_cpp_function_tools(List[LlamaCppFunctionTool]): List of LlamaCppFunctionTool instances.
+            allow_parallel_function_calling (bool): Allow parallel function calling (Default=False)
+            add_send_message_to_user_function (bool): Flag to add send_message_to_user function.
+            send_message_to_user_callback (Callable[[str], None]): Callback for sending a message to the user.
+            debug_output (bool): Enable debug output.
+        """
+        self.llama_cpp_tools = []
+        if llama_cpp_function_tools:
+            self.llama_cpp_tools = llama_cpp_function_tools
+
+        self.send_message_to_user_callback = send_message_to_user_callback
+        if add_send_message_to_user_function:
+            self.llama_cpp_tools.append(LlamaCppFunctionTool(send_message, agent=self))
+
+        if basic_file_tools:
+            self.llama_cpp_tools.append(LlamaCppFunctionTool(read_text_file))
+            self.llama_cpp_tools.append(
+                LlamaCppFunctionTool(write_text_file, agent=self)
+            )
+
+        self.tool_registry = LlamaCppAgent.get_function_tool_registry(
+            self.llama_cpp_tools,
+            add_inner_thoughts=True,
+            allow_inner_thoughts_only=False,
+            allow_parallel_function_calling=allow_parallel_function_calling,
+        )
+
+        if llama_generation_settings is None:
+            if isinstance(llama_llm, Llama) or isinstance(llama_llm, LlamaLLMSettings):
+                llama_generation_settings = LlamaLLMGenerationSettings()
+            elif isinstance(llama_llm, OpenAIEndpointSettings):
+                llama_generation_settings = OpenAIGenerationSettings()
+            else:
+                llama_generation_settings = LlamaCppGenerationSettings()
+
+        if isinstance(
+            llama_generation_settings, LlamaLLMGenerationSettings
+        ) and isinstance(llama_llm, LlamaCppEndpointSettings):
+            raise Exception(
+                "Wrong generation settings for llama.cpp server endpoint, use LlamaCppServerGenerationSettings under llama_cpp_agent.providers.llama_cpp_server_provider!"
+            )
+        if (
+            isinstance(llama_llm, Llama) or isinstance(llama_llm, LlamaLLMSettings)
+        ) and isinstance(llama_generation_settings, LlamaCppGenerationSettings):
+            raise Exception(
+                "Wrong generation settings for llama-cpp-python, use LlamaLLMGenerationSettings under llama_cpp_agent.llm_settings!"
+            )
+
+        if isinstance(llama_llm, OpenAIEndpointSettings) and not isinstance(
+            llama_generation_settings, OpenAIGenerationSettings
+        ):
+            raise Exception(
+                "Wrong generation settings for OpenAI endpoint, use OpenAIGenerationSettings under llama_cpp_agent.providers.openai_endpoint_provider!"
+            )
+
+        self.llama_generation_settings = llama_generation_settings
+
+        self.without_grammar_mode = False
+        self.without_grammar_mode_function = []
+        self.prompt_suffix = ""
+        if system_prompt is not None:
+            self.system_prompt = system_prompt
+        else:
+            # You can also request to return control back to you after a function call is executed by setting the 'return_control' flag in a function call object.
+            self.system_prompt = (
+                """You are Funky, an AI assistant that calls functions to perform tasks.
+
+To call functions, you respond with a JSON object containing three fields:
+"thoughts_and_reasoning": Your thoughts and reasoning behind the function call.
+"function": The name of the function you want to call.
+"parameters": The arguments required for the function.
+
+After performing a function call, you will receive a response containing the return values of the function calls.
+
+### Functions:
+Below is a list of functions you can use to interact with the system. Each function has specific parameters and requirements. Make sure to follow the instructions for each function carefully.
+Choose the appropriate function based on the task you want to perform. Provide your function calls in JSON format.
+
+"""
+                + self.tool_registry.get_documentation().strip()
+            )
+        self.llama_cpp_agent = LlamaCppAgent(
+            llama_llm,
+            debug_output=debug_output,
+            system_prompt="",
+            predefined_messages_formatter_type=messages_formatter_type,
+            custom_messages_formatter=custom_messages_formatter,
+        )
+
+        self.k_last_messages_from_chat_history = k_last_messages_from_chat_history
+        self.streaming_callback = streaming_callback
+
+    def save(self, file_path: str):
+        """
+        Save the agent's state to a file.
+
+        Args:
+            file_path (str): The path to the file.
+        """
+        with open(file_path, "w", encoding="utf-8") as file:
+            dic = copy(self.as_dict())
+            del dic["llama_cpp_agent"]
+            del dic["streaming_callback"]
+            del dic["tool_registry"]
+            del dic["llama_cpp_tools"]
+            del dic["send_message_to_user_callback"]
+            del dic["without_grammar_mode_function"]
+            dic["debug_output"] = self.llama_cpp_agent.debug_output
+            dic["messages"] = self.llama_cpp_agent.messages
+            dic["llama_generation_settings"] = self.llama_generation_settings.as_dict()
+            dic["custom_messages_formatter"] = (
+                self.llama_cpp_agent.messages_formatter.as_dict()
+            )
+            json.dump(dic, file, indent=4)
+
+    @staticmethod
+    def load_from_file(
+        file_path: str,
+        llama_llm: Union[Llama, LlamaLLMSettings],
+        open_ai_functions: (List[dict], List[Callable]) = None,
+        python_functions: List[Callable] = None,
+        pydantic_functions: List[Type[BaseModel]] = None,
+        send_message_to_user_callback: Callable[[str], None] = None,
+        streaming_callback: Callable[[StreamingResponse], None] = None,
+    ) -> "FunctionCallingAgent":
+        """
+        Load the agent's state from a file.
+
+        Args:
+            file_path (str): The path to the file.
+            llama_llm: LLM to use
+            open_ai_functions (Tuple[List[dict], List[Callable]]): OpenAI function definitions, and a list of the actual functions as tuple.
+            python_functions (List[Callable]): Python functions for interaction.
+            pydantic_functions (List[Type[BaseModel]]): Pydantic models representing functions.
+            send_message_to_user_callback (Callable[[str], None]): Callback for sending a message to the user.
+            streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
+
+        Returns:
+            FunctionCallingAgent: The loaded FunctionCallingAgent instance.
+        """
+
+        with open(file_path, "r", encoding="utf-8") as file:
+            loaded_agent = json.load(file)
+            loaded_agent["llama_llm"] = llama_llm
+            loaded_agent["streaming_callback"] = streaming_callback
+            loaded_agent["python_functions"] = python_functions
+            loaded_agent["pydantic_functions"] = pydantic_functions
+            loaded_agent["open_ai_functions"] = open_ai_functions
+            messages = copy(loaded_agent["messages"])
+            del loaded_agent["messages"]
+            loaded_agent["send_message_to_user_callback"] = (
+                send_message_to_user_callback
+            )
+            loaded_agent["llama_generation_settings"] = (
+                LlamaLLMGenerationSettings.load_from_dict(
+                    loaded_agent["llama_generation_settings"]
+                )
+            )
+            loaded_agent["custom_messages_formatter"] = (
+                MessagesFormatter.load_from_dict(
+                    loaded_agent["custom_messages_formatter"]
+                )
+            )
+            agent = FunctionCallingAgent(**loaded_agent)
+
+            agent.llama_cpp_agent.messages = messages
+            return agent
+
+    @staticmethod
+    def load_from_dict(agent_dict: dict) -> "FunctionCallingAgent":
+        """
+        Load the agent's state from a dictionary.
+
+        Args:
+            agent_dict (dict): The dictionary containing the agent's state.
+
+        Returns:
+            FunctionCallingAgent: The loaded FunctionCallingAgent instance.
+        """
+        return FunctionCallingAgent(**agent_dict)
+
+    def as_dict(self) -> dict:
+        """
+        Convert the agent's state to a dictionary.
+
+        Returns:
+           dict: The dictionary representation of the agent's state.
+        """
+        return self.__dict__
+
+    def generate_response(
+        self, message: str, additional_stop_sequences: List[str] = None
+    ):
+        self.llama_cpp_agent.add_message(role="user", message=message)
+
+        result = self.intern_get_response(
+            additional_stop_sequences=additional_stop_sequences
+        )
+
+        while True:
+            if isinstance(result, str):
+                if len(self.without_grammar_mode_function) > 0:
+                    func_list = []
+                    for func in self.without_grammar_mode_function:
+                        if func.__name__ not in func_list:
+                            func(result.strip())
+                            func_list.append(func.__name__)
+                break
+            function_message = f"""Function Calling Results:\n\n"""
+            count = 0
+            if result is not None:
+                agent_sent_message = False
+                for res in result:
+                    count += 1
+                    if res["function"] == "send_message":
+                        agent_sent_message = True
+                    if not isinstance(res, str):
+                        if "params" in res:
+                            function_message += f"""{count}. Function: "{res["function"]}"\nArguments: "{res["params"]}"\nReturn Value: {res["return_value"]}\n\n"""
+                        else:
+                            function_message += f"""{count}. Function: "{res["function"]}"\nReturn Value: {res["return_value"]}\n\n"""
+                    else:
+                        function_message += f"{count}. " + res + "\n\n"
+                self.llama_cpp_agent.add_message(
+                    role="function", message=function_message.strip()
+                )
+                if agent_sent_message:
+                    break
+            result = self.intern_get_response(
+                additional_stop_sequences=additional_stop_sequences
+            )
+        return result
+
+    def intern_get_response(self, additional_stop_sequences: List[str] = None):
+        without_grammar_mode = False
+        if self.without_grammar_mode:
+            without_grammar_mode = True
+            self.without_grammar_mode = False
+        if additional_stop_sequences is None:
+            additional_stop_sequences = []
+        additional_stop_sequences.append("(End of message)")
+        result = self.llama_cpp_agent.get_chat_response(
+            system_prompt=self.system_prompt,
+            streaming_callback=self.streaming_callback,
+            function_tool_registry=(
+                self.tool_registry if not without_grammar_mode else None
+            ),
+            additional_stop_sequences=additional_stop_sequences,
+            **self.llama_generation_settings.as_dict(),
+        )
+        if without_grammar_mode:
+            self.prompt_suffix = ""
+        return result
+
+    def send_message_to_user(self, message: str):
+        """
+        Send a message to the user.
+
+        Args:
+            message: The message send to the user.
+        """
+        if self.send_message_to_user_callback:
+            self.send_message_to_user_callback(message)
+        else:
+            print(message)
```

### Comparing `llama_cpp_agent-0.1.3/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py` & `llama_cpp_agent-0.1.4/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,1776 +1,1776 @@
-from __future__ import annotations
-
-import inspect
-import json
-import re
-import typing
-from copy import copy
-from enum import Enum
-from inspect import getdoc, isclass
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    List,
-    Optional,
-    Union,
-    get_args,
-    get_origin,
-    get_type_hints,
-)
-
-from docstring_parser import parse
-from pydantic import BaseModel, Field, create_model
-
-if TYPE_CHECKING:
-    from types import GenericAlias
-    from types import UnionType
-else:
-    # python 3.8 compat
-    from typing import _GenericAlias as GenericAlias
-    from types import UnionType
-
-
-class PydanticDataType(Enum):
-    """
-    Defines the data types supported by the grammar_generator.
-
-    Attributes:
-        STRING (str): Represents a string data type.
-        BOOLEAN (str): Represents a boolean data type.
-        INTEGER (str): Represents an integer data type.
-        FLOAT (str): Represents a float data type.
-        OBJECT (str): Represents an object data type.
-        ARRAY (str): Represents an array data type.
-        ENUM (str): Represents an enum data type.
-        CUSTOM_CLASS (str): Represents a custom class data type.
-    """
-
-    STRING = "string"
-    TRIPLE_QUOTED_STRING = "triple_quoted_string"
-    MARKDOWN_CODE_BLOCK = "markdown_code_block"
-    BOOLEAN = "boolean"
-    INTEGER = "number"
-    FLOAT = "number"
-    OBJECT = "object"
-    ARRAY = "array"
-    ENUM = "enum"
-    ANY = "any"
-    NULL = "null"
-    CUSTOM_CLASS = "custom-class"
-    CUSTOM_DICT = "custom-dict"
-    SET = "set"
-
-
-def map_pydantic_type_to_gbnf(pydantic_type: type[Any]) -> str:
-    if isclass(pydantic_type) and issubclass(pydantic_type, str):
-        return PydanticDataType.STRING.value
-    elif isclass(pydantic_type) and issubclass(pydantic_type, bool):
-        return PydanticDataType.BOOLEAN.value
-    elif isclass(pydantic_type) and issubclass(pydantic_type, int):
-        return PydanticDataType.INTEGER.value
-    elif isclass(pydantic_type) and issubclass(pydantic_type, float):
-        return PydanticDataType.FLOAT.value
-    elif isclass(pydantic_type) and issubclass(pydantic_type, Enum):
-        return PydanticDataType.ENUM.value
-
-    elif isclass(pydantic_type) and issubclass(pydantic_type, BaseModel):
-        return format_model_and_field_name(pydantic_type.__name__)
-    elif get_origin(pydantic_type) is list:
-        element_type = get_args(pydantic_type)[0]
-        return f"{map_pydantic_type_to_gbnf(element_type)}-list"
-    elif get_origin(pydantic_type) is set:
-        element_type = get_args(pydantic_type)[0]
-        return f"{map_pydantic_type_to_gbnf(element_type)}-set"
-    elif get_origin(pydantic_type) is Union or isinstance(pydantic_type, UnionType):
-        union_types = get_args(pydantic_type)
-        union_rules = [map_pydantic_type_to_gbnf(ut) for ut in union_types]
-        return f"union-{'-or-'.join(union_rules)}"
-    elif get_origin(pydantic_type) is Optional:
-        element_type = get_args(pydantic_type)[0]
-        return f"optional-{map_pydantic_type_to_gbnf(element_type)}"
-    elif isclass(pydantic_type):
-        return f"{PydanticDataType.CUSTOM_CLASS.value}-{format_model_and_field_name(pydantic_type.__name__)}"
-    elif get_origin(pydantic_type) is dict:
-        key_type, value_type = get_args(pydantic_type)
-        return f"custom-dict-key-type-{format_model_and_field_name(map_pydantic_type_to_gbnf(key_type))}-value-type-{format_model_and_field_name(map_pydantic_type_to_gbnf(value_type))}"
-    else:
-        return "unknown"
-
-
-def format_model_and_field_name(model_name: str) -> str:
-    parts = re.findall("[A-Z][^A-Z]*", model_name)
-    if not parts:  # Check if the list is empty
-        return model_name.lower().replace("_", "-")
-    return "-".join(part.lower().replace("_", "-") for part in parts)
-
-
-def generate_list_rule(element_type):
-    """
-    Generate a GBNF rule for a list of a given element type.
-
-    :param element_type: The type of the elements in the list (e.g., 'string').
-    :return: A string representing the GBNF rule for a list of the given type.
-    """
-    rule_name = f"{map_pydantic_type_to_gbnf(element_type)}-list"
-    element_rule = map_pydantic_type_to_gbnf(element_type)
-    list_rule = rf'{rule_name} ::= "["  {element_rule} (","  {element_rule})* "]"'
-    return list_rule
-
-
-def get_members_structure(cls, rule_name):
-    if issubclass(cls, Enum):
-        # Handle Enum types
-        members = [
-            f'"\\"{member.value}\\""' for name, member in cls.__members__.items()
-        ]
-        return f"{cls.__name__.lower()} ::= " + " | ".join(members)
-    if cls.__annotations__ and cls.__annotations__ != {}:
-        result = f'{rule_name} ::= "{{"'
-        # Modify this comprehension
-        members = [
-            f'  "\\"{name}\\"" ":"  {map_pydantic_type_to_gbnf(param_type)}'
-            for name, param_type in cls.__annotations__.items()
-            if name != "self"
-        ]
-
-        result += '"," '.join(members)
-        result += '  "}"'
-        return result
-    if rule_name == "custom-class-any":
-        result = f"{rule_name} ::= "
-        result += "value"
-        return result
-
-    init_signature = inspect.signature(cls.__init__)
-    parameters = init_signature.parameters
-    result = f'{rule_name} ::=  "{{"'
-    # Modify this comprehension too
-    members = [
-        f'  "\\"{name}\\"" ":"  {map_pydantic_type_to_gbnf(param.annotation)}'
-        for name, param in parameters.items()
-        if name != "self" and param.annotation != inspect.Parameter.empty
-    ]
-
-    result += '", "'.join(members)
-    result += '  "}"'
-    return result
-
-
-def regex_to_gbnf(regex_pattern: str) -> str:
-    """
-    Translate a basic regex pattern to a GBNF rule.
-    Note: This function handles only a subset of simple regex patterns.
-    """
-    gbnf_rule = regex_pattern
-
-    # Translate common regex components to GBNF
-    gbnf_rule = gbnf_rule.replace("\\d", "[0-9]")
-    gbnf_rule = gbnf_rule.replace("\\s", "[ \t\n]")
-
-    # Handle quantifiers and other regex syntax that is similar in GBNF
-    # (e.g., '*', '+', '?', character classes)
-
-    return gbnf_rule
-
-
-def generate_gbnf_integer_rules(max_digit=None, min_digit=None):
-    """
-
-    Generate GBNF Integer Rules
-
-    Generates GBNF (Generalized Backus-Naur Form) rules for integers based on the given maximum and minimum digits.
-
-    Parameters:
-        max_digit (int): The maximum number of digits for the integer. Default is None.
-        min_digit (int): The minimum number of digits for the integer. Default is None.
-
-    Returns:
-        integer_rule (str): The identifier for the integer rule generated.
-        additional_rules (list): A list of additional rules generated based on the given maximum and minimum digits.
-
-    """
-    additional_rules = []
-
-    # Define the rule identifier based on max_digit and min_digit
-    integer_rule = "integer-part"
-    if max_digit is not None:
-        integer_rule += f"-max{max_digit}"
-    if min_digit is not None:
-        integer_rule += f"-min{min_digit}"
-
-    # Handling Integer Rules
-    if max_digit is not None or min_digit is not None:
-        # Start with an empty rule part
-        integer_rule_part = ""
-
-        # Add mandatory digits as per min_digit
-        if min_digit is not None:
-            integer_rule_part += "[0-9] " * min_digit
-
-        # Add optional digits up to max_digit
-        if max_digit is not None:
-            optional_digits = max_digit - (min_digit if min_digit is not None else 0)
-            integer_rule_part += "".join(["[0-9]? " for _ in range(optional_digits)])
-
-        # Trim the rule part and append it to additional rules
-        integer_rule_part = integer_rule_part.strip()
-        if integer_rule_part:
-            additional_rules.append(f"{integer_rule} ::= {integer_rule_part}")
-
-    return integer_rule, additional_rules
-
-
-def generate_gbnf_float_rules(
-    max_digit=None, min_digit=None, max_precision=None, min_precision=None
-):
-    """
-    Generate GBNF float rules based on the given constraints.
-
-    :param max_digit: Maximum number of digits in the integer part (default: None)
-    :param min_digit: Minimum number of digits in the integer part (default: None)
-    :param max_precision: Maximum number of digits in the fractional part (default: None)
-    :param min_precision: Minimum number of digits in the fractional part (default: None)
-    :return: A tuple containing the float rule and additional rules as a list
-
-    Example Usage:
-    max_digit = 3
-    min_digit = 1
-    max_precision = 2
-    min_precision = 1
-    generate_gbnf_float_rules(max_digit, min_digit, max_precision, min_precision)
-
-    Output:
-    ('float-3-1-2-1', ['integer-part-max3-min1 ::= [0-9] [0-9] [0-9]?', 'fractional-part-max2-min1 ::= [0-9] [0-9]?', 'float-3-1-2-1 ::= integer-part-max3-min1 "." fractional-part-max2-min
-    *1'])
-
-    Note:
-    GBNF stands for Generalized Backus-Naur Form, which is a notation technique to specify the syntax of programming languages or other formal grammars.
-    """
-    additional_rules = []
-
-    # Define the integer part rule
-    integer_part_rule = (
-        "integer-part"
-        + (f"-max{max_digit}" if max_digit is not None else "")
-        + (f"-min{min_digit}" if min_digit is not None else "")
-    )
-
-    # Define the fractional part rule based on precision constraints
-    fractional_part_rule = "fractional-part"
-    fractional_rule_part = ""
-    if max_precision is not None or min_precision is not None:
-        fractional_part_rule += (
-            f"-max{max_precision}" if max_precision is not None else ""
-        ) + (f"-min{min_precision}" if min_precision is not None else "")
-        # Minimum number of digits
-        fractional_rule_part = "[0-9]" * (
-            min_precision if min_precision is not None else 1
-        )
-        # Optional additional digits
-        fractional_rule_part += "".join(
-            [" [0-9]?"]
-            * (
-                (max_precision - (min_precision if min_precision is not None else 1))
-                if max_precision is not None
-                else 0
-            )
-        )
-        additional_rules.append(f"{fractional_part_rule} ::= {fractional_rule_part}")
-
-    # Define the float rule
-    float_rule = f"float-{max_digit if max_digit is not None else 'X'}-{min_digit if min_digit is not None else 'X'}-{max_precision if max_precision is not None else 'X'}-{min_precision if min_precision is not None else 'X'}"
-    additional_rules.append(
-        f'{float_rule} ::= {integer_part_rule} "." {fractional_part_rule}'
-    )
-
-    # Generating the integer part rule definition, if necessary
-    if max_digit is not None or min_digit is not None:
-        integer_rule_part = "[0-9]"
-        if min_digit is not None and min_digit > 1:
-            integer_rule_part += " [0-9]" * (min_digit - 1)
-        if max_digit is not None:
-            integer_rule_part += "".join(
-                [" [0-9]?"] * (max_digit - (min_digit if min_digit is not None else 1))
-            )
-        additional_rules.append(f"{integer_part_rule} ::= {integer_rule_part.strip()}")
-
-    return float_rule, additional_rules
-
-
-def generate_gbnf_rule_for_type(
-    model_name,
-    field_name,
-    field_type,
-    is_optional,
-    processed_models,
-    created_rules,
-    field_info=None,
-) -> tuple[str, list[str]]:
-    """
-    Generate GBNF rule for a given field type.
-
-    :param model_name: Name of the model.
-
-    :param field_name: Name of the field.
-    :param field_type: Type of the field.
-    :param is_optional: Whether the field is optional.
-    :param processed_models: List of processed models.
-    :param created_rules: List of created rules.
-    :param field_info: Additional information about the field (optional).
-
-    :return: Tuple containing the GBNF type and a list of additional rules.
-    :rtype: tuple[str, list]
-    """
-    rules = []
-
-    field_name = format_model_and_field_name(field_name)
-    gbnf_type = map_pydantic_type_to_gbnf(field_type)
-
-    if isclass(field_type) and issubclass(field_type, BaseModel):
-        nested_model_name = format_model_and_field_name(field_type.__name__)
-        nested_model_rules, _ = generate_gbnf_grammar(
-            field_type, processed_models, created_rules
-        )
-        rules.extend(nested_model_rules)
-        gbnf_type, rules = nested_model_name, rules
-    elif isclass(field_type) and issubclass(field_type, Enum):
-        enum_values = [
-            f'"\\"{e.value}\\""' for e in field_type
-        ]  # Adding escaped quotes
-        enum_rule = f"{model_name}-{field_name} ::= {' | '.join(enum_values)}"
-        rules.append(enum_rule)
-        gbnf_type, rules = model_name + "-" + field_name, rules
-    elif get_origin(field_type) == list:  # Array
-        element_type = get_args(field_type)[0]
-        element_rule_name, additional_rules = generate_gbnf_rule_for_type(
-            model_name,
-            f"{field_name}-element",
-            element_type,
-            is_optional,
-            processed_models,
-            created_rules,
-        )
-        rules.extend(additional_rules)
-        array_rule = rf"""{model_name}-{field_name} ::= "[" ws ({element_rule_name})? ("," ws {element_rule_name})* ws "]" """
-        rules.append(array_rule)
-        gbnf_type, rules = model_name + "-" + field_name, rules
-
-    elif get_origin(field_type) == set or field_type == set:  # Array
-        element_type = get_args(field_type)[0]
-        element_rule_name, additional_rules = generate_gbnf_rule_for_type(
-            model_name,
-            f"{field_name}-element",
-            element_type,
-            is_optional,
-            processed_models,
-            created_rules,
-        )
-        rules.extend(additional_rules)
-        array_rule = rf"""{model_name}-{field_name} ::= "[" ws ({element_rule_name})? ("," ws {element_rule_name})* ws "]" """
-        rules.append(array_rule)
-        gbnf_type, rules = model_name + "-" + field_name, rules
-
-    elif gbnf_type.startswith("custom-class-"):
-        rules.append(get_members_structure(field_type, gbnf_type))
-    elif gbnf_type.startswith("custom-dict-"):
-        key_type, value_type = get_args(field_type)
-
-        additional_key_type, additional_key_rules = generate_gbnf_rule_for_type(
-            model_name,
-            f"{field_name}-key-type",
-            key_type,
-            is_optional,
-            processed_models,
-            created_rules,
-        )
-        additional_value_type, additional_value_rules = generate_gbnf_rule_for_type(
-            model_name,
-            f"{field_name}-value-type",
-            value_type,
-            is_optional,
-            processed_models,
-            created_rules,
-        )
-        rules.extend(
-            [
-                rf'{gbnf_type} ::= "{{"  ( {additional_key_type} ": "  {additional_value_type} ("," "\n" ws {additional_key_type} ":"  {additional_value_type})*  )? "}}" '
-            ]
-        )
-        rules.extend(additional_key_rules)
-        rules.extend(additional_value_rules)
-    elif gbnf_type.startswith("union-"):
-        union_types = get_args(field_type)
-        union_rules = []
-
-        for union_type in union_types:
-            if isinstance(union_type, GenericAlias):
-                union_gbnf_type, union_rules_list = generate_gbnf_rule_for_type(
-                    model_name,
-                    field_name,
-                    union_type,
-                    False,
-                    processed_models,
-                    created_rules,
-                )
-                union_rules.append(union_gbnf_type)
-                rules.extend(union_rules_list)
-
-            elif not issubclass(union_type, type(None)):
-                union_gbnf_type, union_rules_list = generate_gbnf_rule_for_type(
-                    model_name,
-                    field_name,
-                    union_type,
-                    False,
-                    processed_models,
-                    created_rules,
-                )
-                union_rules.append(union_gbnf_type)
-                rules.extend(union_rules_list)
-
-        # Defining the union grammar rule separately
-        if len(union_rules) == 1:
-            union_grammar_rule = f"{model_name}-{field_name}-optional ::= {' | '.join(union_rules)} | null"
-        else:
-            uni = []
-            for rule in union_rules:
-                if rule not in uni:
-                    uni.append(rule)
-            union_grammar_rule = (
-                f"{model_name}-{field_name}-union ::= {' | '.join(uni)}"
-            )
-        rules.append(union_grammar_rule)
-        if len(union_rules) == 1:
-            gbnf_type = f"{model_name}-{field_name}-optional"
-        else:
-            gbnf_type = f"{model_name}-{field_name}-union"
-    elif isclass(field_type) and issubclass(field_type, str):
-        if (
-            field_info
-            and hasattr(field_info, "json_schema_extra")
-            and field_info.json_schema_extra is not None
-        ):
-            triple_quoted_string = field_info.json_schema_extra.get(
-                "triple_quoted_string", False
-            )
-            markdown_string = field_info.json_schema_extra.get(
-                "markdown_code_block", False
-            )
-
-            gbnf_type = (
-                PydanticDataType.TRIPLE_QUOTED_STRING.value
-                if triple_quoted_string
-                else PydanticDataType.STRING.value
-            )
-            gbnf_type = (
-                PydanticDataType.MARKDOWN_CODE_BLOCK.value
-                if markdown_string
-                else gbnf_type
-            )
-
-        elif field_info and hasattr(field_info, "pattern"):
-            # Convert regex pattern to grammar rule
-            regex_pattern = field_info.regex.pattern
-            gbnf_type = f"pattern-{field_name} ::= {regex_to_gbnf(regex_pattern)}"
-        else:
-            gbnf_type = PydanticDataType.STRING.value
-
-    elif (
-        isclass(field_type)
-        and issubclass(field_type, float)
-        and field_info
-        and hasattr(field_info, "json_schema_extra")
-        and field_info.json_schema_extra is not None
-    ):
-        # Retrieve precision attributes for floats
-        max_precision = (
-            field_info.json_schema_extra.get("max_precision")
-            if field_info and hasattr(field_info, "json_schema_extra")
-            else None
-        )
-        min_precision = (
-            field_info.json_schema_extra.get("min_precision")
-            if field_info and hasattr(field_info, "json_schema_extra")
-            else None
-        )
-        max_digits = (
-            field_info.json_schema_extra.get("max_digit")
-            if field_info and hasattr(field_info, "json_schema_extra")
-            else None
-        )
-        min_digits = (
-            field_info.json_schema_extra.get("min_digit")
-            if field_info and hasattr(field_info, "json_schema_extra")
-            else None
-        )
-
-        # Generate GBNF rule for float with given attributes
-        gbnf_type, rules = generate_gbnf_float_rules(
-            max_digit=max_digits,
-            min_digit=min_digits,
-            max_precision=max_precision,
-            min_precision=min_precision,
-        )
-
-    elif (
-        isclass(field_type)
-        and issubclass(field_type, int)
-        and field_info
-        and hasattr(field_info, "json_schema_extra")
-        and field_info.json_schema_extra is not None
-    ):
-        # Retrieve digit attributes for integers
-        max_digits = (
-            field_info.json_schema_extra.get("max_digit")
-            if field_info and hasattr(field_info, "json_schema_extra")
-            else None
-        )
-        min_digits = (
-            field_info.json_schema_extra.get("min_digit")
-            if field_info and hasattr(field_info, "json_schema_extra")
-            else None
-        )
-
-        # Generate GBNF rule for integer with given attributes
-        gbnf_type, rules = generate_gbnf_integer_rules(
-            max_digit=max_digits, min_digit=min_digits
-        )
-    else:
-        gbnf_type, rules = gbnf_type, []
-
-    return gbnf_type, rules
-
-
-def generate_gbnf_grammar(
-    model: type[BaseModel],
-    processed_models: set[type[BaseModel]],
-    created_rules: dict[str, list[str]],
-) -> tuple[list[str], bool]:
-    """
-
-    Generate GBnF Grammar
-
-    Generates a GBnF grammar for a given model.
-
-    :param model: A Pydantic model class to generate the grammar for. Must be a subclass of BaseModel.
-    :param processed_models: A set of already processed models to prevent infinite recursion.
-    :param created_rules: A dict containing already created rules to prevent duplicates.
-    :return: A list of GBnF grammar rules in string format. And two booleans indicating if an extra markdown or triple quoted string is in the grammar.
-    Example Usage:
-    ```
-    model = MyModel
-    processed_models = set()
-    created_rules = dict()
-
-    gbnf_grammar = generate_gbnf_grammar(model, processed_models, created_rules)
-    ```
-    """
-    if model in processed_models:
-        return [], False
-
-    processed_models.add(model)
-    model_name = format_model_and_field_name(model.__name__)
-
-    if not issubclass(model, BaseModel):
-        # For non-Pydantic classes, generate model_fields from __annotations__ or __init__
-        if hasattr(model, "__annotations__") and model.__annotations__:
-            model_fields = {
-                name: (typ, ...) for name, typ in model.__annotations__.items()
-            }
-        else:
-            init_signature = inspect.signature(model.__init__)
-            parameters = init_signature.parameters
-            model_fields = {
-                name: (param.annotation, param.default)
-                for name, param in parameters.items()
-                if name != "self"
-            }
-    else:
-        # For Pydantic models, use model_fields and check for ellipsis (required fields)
-        model_fields = model.__annotations__
-
-    model_rule_parts = []
-    nested_rules = []
-    has_markdown_code_block = False
-    has_triple_quoted_string = False
-    look_for_markdown_code_block = False
-    look_for_triple_quoted_string = False
-    for field_name, field_info in model_fields.items():
-        if not issubclass(model, BaseModel):
-            field_type, default_value = field_info
-            # Check if the field is optional (not required)
-            is_optional = (default_value is not inspect.Parameter.empty) and (
-                default_value is not Ellipsis
-            )
-        else:
-            field_type = field_info
-            field_info = model.model_fields[field_name]
-            is_optional = (
-                field_info.is_required is False and get_origin(field_type) is Optional
-            )
-        rule_name, additional_rules = generate_gbnf_rule_for_type(
-            model_name,
-            format_model_and_field_name(field_name),
-            field_type,
-            is_optional,
-            processed_models,
-            created_rules,
-            field_info,
-        )
-        look_for_markdown_code_block = (
-            True if rule_name == "markdown_code_block" else False
-        )
-        look_for_triple_quoted_string = (
-            True if rule_name == "triple_quoted_string" else False
-        )
-        if not look_for_markdown_code_block and not look_for_triple_quoted_string:
-            if rule_name not in created_rules:
-                created_rules[rule_name] = additional_rules
-            model_rule_parts.append(
-                f' ws "\\"{field_name}\\"" ": " {rule_name}'
-            )  # Adding escaped quotes
-            nested_rules.extend(additional_rules)
-        else:
-            has_triple_quoted_string = look_for_triple_quoted_string
-            has_markdown_code_block = look_for_markdown_code_block
-
-    fields_joined = r' "," '.join(model_rule_parts)
-    if fields_joined != "":
-        model_rule = rf'{model_name} ::= "{{" {fields_joined} ws "}}"'
-    else:
-        model_rule = rf'{model_name} ::= "{{" "}}"'
-
-    has_special_string = False
-    if has_triple_quoted_string:
-        model_rule += '"\\n" ws "}"'
-        model_rule += '"\\n" triple-quoted-string'
-        has_special_string = True
-    if has_markdown_code_block:
-        model_rule += '"\\n" ws "}"'
-        model_rule += '"\\n" markdown-code-block'
-        has_special_string = True
-    all_rules = [model_rule] + nested_rules
-
-    return all_rules, has_special_string
-
-
-def generate_gbnf_grammar_from_pydantic_models(
-    models: list[type[BaseModel]],
-    outer_object_name: str | None = None,
-    outer_object_content: str | None = None,
-    list_of_outputs: bool = False,
-    add_inner_thoughts: bool = True,
-    allow_only_inner_thoughts: bool = True,
-    inner_thought_field_name: str = "chain_of_thought",
-    add_request_heartbeat: bool = True,
-    request_heartbeat_field_name: str = "request_heartbeat",
-    request_heartbeat_models: list[str] = None,
-) -> str:
-    """
-    Generate GBNF Grammar from Pydantic Models.
-
-    This method takes a list of Pydantic models and uses them to generate a GBNF grammar string. The generated grammar string can be used for parsing and validating data using the generated
-    * grammar.
-
-    Args:
-        models (list[type[BaseModel]]): A list of Pydantic models to generate the grammar from.
-        outer_object_name (str): Outer object name for the GBNF grammar. If None, no outer object will be generated. Eg. "function" for function calling.
-        outer_object_content (str): Content for the outer rule in the GBNF grammar. Eg. "function_parameters" or "params" for function calling.
-        list_of_outputs (str, optional): Allows a list of output objects
-        add_inner_thoughts (bool, optional): Add inner thoughts to the grammar. Defaults to True.
-        allow_only_inner_thoughts (bool, optional): Allow only inner thoughts. Defaults to True.
-    Returns:
-        str: The generated GBNF grammar string.
-
-    Examples:
-        models = [UserModel, PostModel]
-        grammar = generate_gbnf_grammar_from_pydantic(models)
-        print(grammar)
-        # Output:
-        # root ::= UserModel | PostModel
-        # ...
-    """
-    if request_heartbeat_models is None:
-        request_heartbeat_models = []
-    processed_models: set[type[BaseModel]] = set()
-    all_rules = []
-    created_rules: dict[str, list[str]] = {}
-    if outer_object_name is None:
-        for model in models:
-            model_rules, _ = generate_gbnf_grammar(
-                model, processed_models, created_rules
-            )
-            all_rules.extend(model_rules)
-
-        if list_of_outputs:
-            root_rule = (
-                r'root ::= (" "| "\n") "[" ws grammar-models ("," ws grammar-models)* "\n" "]"'
-                + "\n"
-            )
-        else:
-            root_rule = r'root ::= (" "| "\n") grammar-models' + "\n"
-        root_rule += "grammar-models ::= " + " | ".join(
-            [format_model_and_field_name(model.__name__) for model in models]
-        )
-        all_rules.insert(0, root_rule)
-        return "\n".join(all_rules)
-    elif outer_object_name is not None:
-        if list_of_outputs:
-            root_rule = (
-                rf'root ::= (" "| "\n") "[" ws {format_model_and_field_name(outer_object_name)} ("," ws {format_model_and_field_name(outer_object_name)})* "\n" "]"'
-                + "\n"
-            )
-        else:
-            root_rule = f"root ::= {format_model_and_field_name(outer_object_name)}\n"
-
-        if add_inner_thoughts:
-            if allow_only_inner_thoughts:
-                model_rule = rf'{format_model_and_field_name(outer_object_name)} ::= (" "| "\n") "{{" ws "\"{inner_thought_field_name}\""  ":" ws string (("," ws "\"{outer_object_name}\""  ":" ws grammar-models)? | ws "}}")'
-            else:
-                model_rule = rf'{format_model_and_field_name(outer_object_name)} ::= (" "| "\n") "{{" ws "\"{inner_thought_field_name}\""  ":" ws string "," ws "\"{outer_object_name}\""  ":" ws grammar-models '
-        else:
-            model_rule = rf'{format_model_and_field_name(outer_object_name)} ::= (" "| "\n") "{{" ws "\"{outer_object_name}\""  ": " ws grammar-models'
-
-        fields_joined = " | ".join(
-            [
-                rf"{format_model_and_field_name(model.__name__)}-grammar-model"
-                for model in models
-            ]
-        )
-
-        grammar_model_rules = f"\ngrammar-models ::= {fields_joined}"
-        mod_rules = []
-        for model in models:
-            mod_rule = (
-                rf"{format_model_and_field_name(model.__name__)}-grammar-model ::= "
-            )
-            mod_rule += (
-                rf'"\"{model.__name__}\"" "," ws "\"{outer_object_content}\"" ": " {format_model_and_field_name(model.__name__)}'
-                + "\n"
-            )
-            mod_rules.append(mod_rule)
-        grammar_model_rules += "\n" + "\n".join(mod_rules)
-
-        for model in models:
-            model_rules, has_special_string = generate_gbnf_grammar(
-                model, processed_models, created_rules
-            )
-            if add_request_heartbeat and model.__name__ in request_heartbeat_models:
-                model_rules[
-                    0
-                ] += rf' "," ws "\"{request_heartbeat_field_name}\""  ":" ws boolean '
-            if not has_special_string:
-                model_rules[0] += r' ws "}"'
-
-            all_rules.extend(model_rules)
-
-        all_rules.insert(0, root_rule + model_rule + grammar_model_rules)
-        return "\n".join(all_rules)
-
-
-def get_primitive_grammar(grammar):
-    """
-    Returns the needed GBNF primitive grammar for a given GBNF grammar string.
-
-    Args:
-        grammar (str): The string containing the GBNF grammar.
-
-    Returns:
-        str: GBNF primitive grammar string.
-    """
-    type_list: list[type[object]] = []
-    if "string-list" in grammar:
-        type_list.append(str)
-    if "boolean-list" in grammar:
-        type_list.append(bool)
-    if "integer-list" in grammar:
-        type_list.append(int)
-    if "float-list" in grammar:
-        type_list.append(float)
-    additional_grammar = [generate_list_rule(t) for t in type_list]
-    primitive_grammar = r"""
-boolean ::= "true" | "false"
-null ::= "null"
-string ::= "\"" (
-        [^"\\] |
-        "\\" (["\\/bfnrt] | "u" [0-9a-fA-F] [0-9a-fA-F] [0-9a-fA-F] [0-9a-fA-F])
-      )* "\""
-ws ::= ([ \t\n]+)
-number ::= "-"? ([0-9]+ | [0-9]+ "." [0-9]+) ([eE] [-+]? [0-9]+)?"""
-
-    any_block = ""
-    if "custom-class-any" in grammar:
-        any_block = """
-value ::= object | array | string | number | boolean | null
-
-object ::=
-  "{" ws (
-            string ":" ws value
-    ("," ws string ":" ws value)*
-  )? "}"
-
-array  ::=
-  "[" ws (
-            value
-    ("," ws value)*
-  )? "]"
-"""
-
-    markdown_code_block_grammar = ""
-    if "markdown-code-block" in grammar:
-        markdown_code_block_grammar = r'''
-markdown-code-block ::= opening-triple-ticks markdown-code-block-content closing-triple-ticks
-markdown-code-block-content ::= ( [^`] | "`" [^`] |  "`"  "`" [^`]  )*
-opening-triple-ticks ::= "```" "python" "\n" | "```" "c" "\n" | "```" "cpp" "\n" | "```" "txt" "\n" | "```" "text" "\n" | "```" "json" "\n" | "```" "javascript" "\n" | "```" "css" "\n" | "```" "html" "\n" | "```" "markdown" "\n"
-closing-triple-ticks ::= "```" "\n"'''
-
-    if "triple-quoted-string" in grammar:
-        markdown_code_block_grammar = r"""
-triple-quoted-string ::= triple-quotes triple-quoted-string-content triple-quotes
-triple-quoted-string-content ::= ( [^'] | "'" [^'] |  "'"  "'" [^']  )*
-triple-quotes ::= "'''" """
-    return (
-        "\n"
-        + "\n".join(additional_grammar)
-        + any_block
-        + primitive_grammar
-        + markdown_code_block_grammar
-    )
-
-
-def generate_markdown_documentation(
-    pydantic_models: list[type[BaseModel]],
-    model_prefix="Model",
-    fields_prefix="Fields",
-    documentation_with_field_description=True,
-) -> str:
-    """
-    Generate markdown documentation for a list of Pydantic models.
-
-    Args:
-        pydantic_models (list[type[BaseModel]]): list of Pydantic model classes.
-        model_prefix (str): Prefix for the model section.
-        fields_prefix (str): Prefix for the fields section.
-        documentation_with_field_description (bool): Include field descriptions in the documentation.
-
-    Returns:
-        str: Generated text documentation.
-    """
-    documentation = "## Functions\n\n"
-    pyd_models = [(model, True) for model in pydantic_models]
-    for model, add_prefix in pyd_models:
-        if add_prefix:
-            documentation += f"### {model.__name__}\n"
-        else:
-            documentation += f"### {model.__name__}\n"
-
-        # Handling multi-line model description with proper indentation
-
-        class_doc = getdoc(model)
-        base_class_doc = getdoc(BaseModel)
-        class_description = (
-            class_doc if class_doc and class_doc != base_class_doc else ""
-        )
-        if class_description != "":
-            documentation += format_multiline_description(class_description, 0) + "\n"
-
-        if add_prefix:
-            # Indenting the fields section
-            documentation += f"{fields_prefix}:\n"
-        else:
-            documentation += f"Fields:\n"
-        if isclass(model) and issubclass(model, BaseModel):
-            for name, field_type in model.__annotations__.items():
-                # if name == "markdown_code_block":
-                #    continue
-                if get_origin(field_type) == list:
-                    element_type = get_args(field_type)[0]
-                    if isclass(element_type) and issubclass(element_type, BaseModel):
-                        pyd_models.append((element_type, False))
-                if get_origin(field_type) == Union:
-                    element_types = get_args(field_type)
-                    for element_type in element_types:
-                        if isclass(element_type) and issubclass(
-                            element_type, BaseModel
-                        ):
-                            pyd_models.append((element_type, False))
-                documentation += generate_field_markdown(
-                    name,
-                    field_type,
-                    model,
-                    documentation_with_field_description=documentation_with_field_description,
-                )
-            if add_prefix:
-                if documentation.endswith(f"{fields_prefix}:\n"):
-                    documentation += "none\n"
-            else:
-                if documentation.endswith("Fields:\n"):
-                    documentation += "none\n"
-            documentation += "\n"
-
-        if (
-            hasattr(model, "Config")
-            and hasattr(model.Config, "json_schema_extra")
-            and "example" in model.Config.json_schema_extra
-        ):
-            documentation += f"  Expected Example Output for {format_model_and_field_name(model.__name__)}:\n"
-            json_example = json.dumps(model.Config.json_schema_extra["example"])
-            documentation += format_multiline_description(json_example, 2) + "\n"
-
-    return documentation
-
-
-def generate_field_markdown(
-    field_name: str,
-    field_type: type[Any],
-    model: type[BaseModel],
-    depth=1,
-    documentation_with_field_description=True,
-) -> str:
-    """
-    Generate markdown documentation for a Pydantic model field.
-
-    Args:
-        field_name (str): Name of the field.
-        field_type (type[Any]): Type of the field.
-        model (type[BaseModel]): Pydantic model class.
-        depth (int): Indentation depth in the documentation.
-        documentation_with_field_description (bool): Include field descriptions in the documentation.
-
-    Returns:
-        str: Generated text documentation for the field.
-    """
-    indent = "  " * depth
-
-    field_info = model.model_fields.get(field_name)
-    field_description = (
-        field_info.description if field_info and field_info.description else ""
-    )
-
-    if get_origin(field_type) == list:
-        element_type = get_args(field_type)[0]
-        field_text = f"{indent}{field_name} ({format_model_and_field_name(field_type.__name__)} of {format_model_and_field_name(element_type.__name__)})"
-        if field_description != "":
-            field_text += ": "
-        else:
-            field_text += "\n"
-    elif get_origin(field_type) == Union or isinstance(field_type, UnionType):
-        element_types = get_args(field_type)
-        types = []
-        for element_type in element_types:
-            if element_type.__name__ == "NoneType":
-                types.append("null")
-            else:
-                types.append(format_model_and_field_name(element_type.__name__))
-        field_text = f"{indent}{field_name} ({' or '.join(types)})"
-        if field_description != "":
-            field_text += ": "
-        else:
-            field_text += "\n"
-
-    elif issubclass(field_type, Enum):
-        enum_values = [f"'{str(member.value)}'" for member in field_type]
-
-        field_text = f"{indent}{field_name} ({' or '.join(enum_values)})"
-        if field_description != "":
-            field_text += ": "
-        else:
-            field_text += "\n"
-
-    else:
-        field_text = (
-            f"{indent}{field_name} ({format_model_and_field_name(field_type.__name__)})"
-        )
-        if field_description != "":
-            field_text += ": "
-        else:
-            field_text += "\n"
-
-    if not documentation_with_field_description:
-        return field_text
-
-    if field_description != "":
-        field_text += field_description + "\n"
-
-    # Check for and include field-specific examples if available
-    if (
-        hasattr(model, "Config")
-        and hasattr(model.Config, "json_schema_extra")
-        and "example" in model.Config.json_schema_extra
-    ):
-        field_example = model.Config.json_schema_extra["example"].get(field_name)
-        if field_example is not None:
-            example_text = (
-                f"'{field_example}'"
-                if isinstance(field_example, str)
-                else field_example
-            )
-            field_text += f"{indent}  Example: {example_text}\n"
-
-    if isclass(field_type) and issubclass(field_type, BaseModel):
-        field_text += f"{indent}  Details:\n"
-        for name, type_ in field_type.__annotations__.items():
-            field_text += generate_field_markdown(name, type_, field_type, depth + 2)
-
-    return field_text
-
-
-def format_json_example(example: dict[str, Any], depth: int) -> str:
-    """
-    Format a JSON example into a readable string with indentation.
-
-    Args:
-        example (dict): JSON example to be formatted.
-        depth (int): Indentation depth.
-
-    Returns:
-        str: Formatted JSON example string.
-    """
-    indent = "    " * depth
-    formatted_example = "{\n"
-    for key, value in example.items():
-        value_text = f"'{value}'" if isinstance(value, str) else value
-        formatted_example += f"{indent}{key}: {value_text},\n"
-    formatted_example = formatted_example.rstrip(",\n") + "\n" + indent + "}"
-    return formatted_example
-
-
-def generate_text_documentation(
-    pydantic_models: list[type[BaseModel]],
-    model_prefix="Model",
-    fields_prefix="Fields",
-    documentation_with_field_description=True,
-) -> str:
-    """
-    Generate markdown documentation for a list of Pydantic models.
-
-    Args:
-        pydantic_models (list[type[BaseModel]]): list of Pydantic model classes.
-        model_prefix (str): Prefix for the model section.
-        fields_prefix (str): Prefix for the fields section.
-        documentation_with_field_description (bool): Include field descriptions in the documentation.
-
-    Returns:
-        str: Generated text documentation.
-    """
-    documentation = ""
-    pyd_models = [(model, True) for model in pydantic_models]
-    for model, add_prefix in pyd_models:
-        if add_prefix:
-            documentation += f"{model_prefix}: {model.__name__}\n"
-        else:
-            documentation += f"model: {model.__name__}\n"
-
-        # Handling multi-line model description with proper indentation
-
-        class_doc = getdoc(model)
-        base_class_doc = getdoc(BaseModel)
-        class_description = (
-            class_doc if class_doc and class_doc != base_class_doc else ""
-        )
-        if class_description != "":
-            documentation += "  description: "
-            documentation += format_multiline_description(class_description, 2) + "\n"
-
-        if add_prefix:
-            # Indenting the fields section
-            documentation += f"  {fields_prefix}:\n"
-        else:
-            documentation += f"  fields:\n"
-        if isclass(model) and issubclass(model, BaseModel):
-            for name, field_type in model.__annotations__.items():
-                # if name == "markdown_code_block":
-                #    continue
-                if get_origin(field_type) == list:
-                    element_type = get_args(field_type)[0]
-                    if isclass(element_type) and issubclass(element_type, BaseModel):
-                        pyd_models.append((element_type, False))
-                    if get_origin(element_type) == Union or isinstance(
-                        element_type, UnionType
-                    ):
-                        element_types = get_args(element_type)
-                        for element_type in element_types:
-                            if isclass(element_type) and issubclass(
-                                element_type, BaseModel
-                            ):
-                                pyd_models.append((element_type, False))
-                            if get_origin(element_type) == list:
-                                element_type = get_args(element_type)[0]
-                                if isclass(element_type) and issubclass(
-                                    element_type, BaseModel
-                                ):
-                                    pyd_models.append((element_type, False))
-                if get_origin(field_type) == Union or isinstance(field_type, UnionType):
-                    element_types = get_args(field_type)
-                    for element_type in element_types:
-                        if isclass(element_type) and issubclass(
-                            element_type, BaseModel
-                        ):
-                            pyd_models.append((element_type, False))
-                        if get_origin(element_type) == list:
-                            element_type = get_args(element_type)[0]
-                            if isclass(element_type) and issubclass(
-                                element_type, BaseModel
-                            ):
-                                pyd_models.append((element_type, False))
-                if isclass(field_type) and issubclass(field_type, BaseModel):
-                    pyd_models.append((field_type, False))
-                documentation += generate_field_text(
-                    name,
-                    field_type,
-                    model,
-                    documentation_with_field_description=documentation_with_field_description,
-                )
-            if add_prefix:
-                if documentation.endswith(f"{fields_prefix}:\n"):
-                    documentation += "    none\n"
-            else:
-                if documentation.endswith("fields:\n"):
-                    documentation += "    none\n"
-            documentation += "\n"
-
-        if (
-            hasattr(model, "Config")
-            and hasattr(model.Config, "json_schema_extra")
-            and "example" in model.Config.json_schema_extra
-        ):
-            documentation += f"  Expected Example Output for {format_model_and_field_name(model.__name__)}:\n"
-            json_example = json.dumps(model.Config.json_schema_extra["example"])
-            documentation += format_multiline_description(json_example, 2) + "\n"
-
-    return documentation
-
-
-def generate_field_text(
-    field_name: str,
-    field_type: type[Any],
-    model: type[BaseModel],
-    depth=1,
-    documentation_with_field_description=True,
-) -> str:
-    """
-    Generate markdown documentation for a Pydantic model field.
-
-    Args:
-        field_name (str): Name of the field.
-        field_type (type[Any]): Type of the field.
-        model (type[BaseModel]): Pydantic model class.
-        depth (int): Indentation depth in the documentation.
-        documentation_with_field_description (bool): Include field descriptions in the documentation.
-
-    Returns:
-        str: Generated text documentation for the field.
-    """
-    indent = "    " * depth
-
-    field_info = model.model_fields.get(field_name)
-    field_description = (
-        field_info.description if field_info and field_info.description else ""
-    )
-
-    if get_origin(field_type) == list:
-        element_type = get_args(field_type)[0]
-        if get_origin(element_type) == Union or isinstance(element_type, UnionType):
-            element_types = get_args(element_type)
-            types = []
-            for element_type in element_types:
-                if element_type.__name__ == "NoneType":
-                    types.append("null")
-                else:
-                    if isclass(element_type) and issubclass(element_type, Enum):
-                        enum_values = [
-                            f"'{str(member.value)}'" for member in element_type
-                        ]
-                        for enum_value in enum_values:
-                            types.append(enum_value)
-
-                    else:
-                        if get_origin(element_type) == list:
-                            element_type = get_args(element_type)[0]
-                            types.append(f"(list of {element_type.__name__})")
-                        else:
-                            types.append(element_type.__name__)
-            field_text = f"({' or '.join(types)})"
-            field_text = f"{indent}{field_name} ({field_type.__name__} of {field_text})"
-            if field_description != "":
-                field_text += ": "
-            else:
-                field_text += "\n"
-        else:
-            field_text = f"{indent}{field_name} ({field_type.__name__} of {element_type.__name__})"
-            if field_description != "":
-                field_text += ": "
-            else:
-                field_text += "\n"
-    elif get_origin(field_type) == Union:
-        element_types = get_args(field_type)
-        types = []
-        for element_type in element_types:
-            if element_type.__name__ == "NoneType":
-                types.append("null")
-            else:
-                if isclass(element_type) and issubclass(element_type, Enum):
-                    enum_values = [f"'{str(member.value)}'" for member in element_type]
-                    for enum_value in enum_values:
-                        types.append(enum_value)
-
-                else:
-                    if get_origin(element_type) == list:
-                        element_type = get_args(element_type)[0]
-                        types.append(f"(list of {element_type.__name__})")
-                    else:
-                        types.append(element_type.__name__)
-        field_text = f"{indent}{field_name} ({' or '.join(types)})"
-        if field_description != "":
-            field_text += ": "
-        else:
-            field_text += "\n"
-    elif isinstance(field_type, GenericAlias):
-        if field_type.__origin__ == dict:
-            key_type, value_type = get_args(field_type)
-
-            additional_key_type = key_type.__name__
-            additional_value_type = value_type.__name__
-            field_text = f"{indent}{field_name} (dict of {additional_key_type} to {additional_value_type})"
-            if field_description != "":
-                field_text += ": "
-            else:
-                field_text += "\n"
-        elif field_type.__origin__ == list:
-            element_type = get_args(field_type)[0]
-            field_text = f"{indent}{field_name} (list of {element_type.__name__})"
-            if field_description != "":
-                field_text += ": "
-            else:
-                field_text += "\n"
-    elif issubclass(field_type, Enum):
-        enum_values = [f"'{str(member.value)}'" for member in field_type]
-
-        field_text = f"{indent}{field_name} ({' or '.join(enum_values)})"
-        if field_description != "":
-            field_text += ": "
-        else:
-            field_text += "\n"
-
-    else:
-        field_text = (
-            f"{indent}{field_name} ({format_model_and_field_name(field_type.__name__)})"
-        )
-        if field_description != "":
-            field_text += ": "
-        else:
-            field_text += "\n"
-
-    if not documentation_with_field_description:
-        return field_text
-
-    if field_description != "":
-        field_text += field_description + "\n"
-
-    # Check for and include field-specific examples if available
-    if (
-        hasattr(model, "Config")
-        and hasattr(model.Config, "json_schema_extra")
-        and "example" in model.Config.json_schema_extra
-    ):
-        field_example = model.Config.json_schema_extra["example"].get(field_name)
-        if field_example is not None:
-            example_text = (
-                f"'{field_example}'"
-                if isinstance(field_example, str)
-                else field_example
-            )
-            field_text += f"{indent}  Example: {example_text}\n"
-
-    return field_text
-
-
-def format_multiline_description(description: str, indent_level: int) -> str:
-    """
-    Format a multiline description with proper indentation.
-
-    Args:
-        description (str): Multiline description.
-        indent_level (int): Indentation level.
-
-    Returns:
-        str: Formatted multiline description.
-    """
-    indent = "  " * indent_level
-    return description.replace("\n", "\n" + indent)
-
-
-def save_gbnf_grammar_and_documentation(
-    grammar,
-    documentation,
-    grammar_file_path="./grammar.gbnf",
-    documentation_file_path="./grammar_documentation.md",
-):
-    """
-    Save GBNF grammar and documentation to specified files.
-
-    Args:
-        grammar (str): GBNF grammar string.
-        documentation (str): Documentation string.
-        grammar_file_path (str): File path to save the GBNF grammar.
-        documentation_file_path (str): File path to save the documentation.
-
-    Returns:
-        None
-    """
-    try:
-        with open(grammar_file_path, "w") as file:
-            file.write(grammar + get_primitive_grammar(grammar))
-        print(f"Grammar successfully saved to {grammar_file_path}")
-    except IOError as e:
-        print(f"An error occurred while saving the grammar file: {e}")
-
-    try:
-        with open(documentation_file_path, "w") as file:
-            file.write(documentation)
-        print(f"Documentation successfully saved to {documentation_file_path}")
-    except IOError as e:
-        print(f"An error occurred while saving the documentation file: {e}")
-
-
-def remove_empty_lines(string):
-    """
-    Remove empty lines from a string.
-
-    Args:
-        string (str): Input string.
-
-    Returns:
-        str: String with empty lines removed.
-    """
-    lines = string.splitlines()
-    non_empty_lines = [line for line in lines if line.strip() != ""]
-    string_no_empty_lines = "\n".join(non_empty_lines)
-    return string_no_empty_lines
-
-
-def generate_and_save_gbnf_grammar_and_documentation(
-    pydantic_model_list,
-    grammar_file_path="./generated_grammar.gbnf",
-    documentation_file_path="./generated_grammar_documentation.md",
-    outer_object_name: str | None = None,
-    outer_object_content: str | None = None,
-    model_prefix: str = "Output Model",
-    fields_prefix: str = "Output Fields",
-    list_of_outputs: bool = False,
-    documentation_with_field_description=True,
-    add_inner_thoughts: bool = False,
-    allow_only_inner_thoughts: bool = False,
-    inner_thoughts_field_name: str = "thoughts_and_reasoning",
-    add_request_heartbeat: bool = False,
-    request_heartbeat_field_name: str = "request_heartbeat",
-    request_heartbeat_models: List[str] = None,
-):
-    """
-    Generate GBNF grammar and documentation, and save them to specified files.
-
-    Args:
-        pydantic_model_list: List of Pydantic model classes.
-        grammar_file_path (str): File path to save the generated GBNF grammar.
-        documentation_file_path (str): File path to save the generated documentation.
-        outer_object_name (str): Outer object name for the GBNF grammar. If None, no outer object will be generated. Eg. "function" for function calling.
-        outer_object_content (str): Content for the outer rule in the GBNF grammar. Eg. "function_parameters" or "params" for function calling.
-        model_prefix (str): Prefix for the model section in the documentation.
-        fields_prefix (str): Prefix for the fields section in the documentation.
-        list_of_outputs (bool): Whether the output is a list of items.
-        documentation_with_field_description (bool): Include field descriptions in the documentation.
-        add_inner_thoughts (bool): Add inner thoughts to the grammar. This is useful for adding comments or reasoning to the output.
-        allow_only_inner_thoughts (bool): Allow only inner thoughts. If True, only inner thoughts will be allowed in the output.
-        inner_thoughts_field_name (str): Field name for inner thoughts. Default is "thoughts_and_reasoning".
-        add_request_heartbeat (bool): Add request heartbeat to the grammar. This allows the LLM to decide when to return control to the system.
-        request_heartbeat_field_name (str): Field name for request heartbeat. Default is "request_heartbeat".
-        request_heartbeat_models (List[str]): List of models that will have a request heartbeat field.
-    Returns:
-        None
-    """
-    documentation = generate_markdown_documentation(
-        pydantic_model_list,
-        model_prefix,
-        fields_prefix,
-        documentation_with_field_description=documentation_with_field_description,
-    )
-    grammar = generate_gbnf_grammar_from_pydantic_models(
-        pydantic_model_list,
-        outer_object_name,
-        outer_object_content,
-        list_of_outputs,
-        add_inner_thoughts,
-        allow_only_inner_thoughts,
-        inner_thoughts_field_name,
-        add_request_heartbeat,
-        request_heartbeat_field_name,
-        request_heartbeat_models,
-    )
-    grammar = remove_empty_lines(grammar)
-    save_gbnf_grammar_and_documentation(
-        grammar, documentation, grammar_file_path, documentation_file_path
-    )
-
-
-def generate_gbnf_grammar_and_documentation(
-    pydantic_model_list,
-    outer_object_name: str | None = None,
-    outer_object_content: str | None = None,
-    model_prefix: str = "Output Model",
-    fields_prefix: str = "Output Fields",
-    list_of_outputs: bool = False,
-    documentation_with_field_description=True,
-    add_inner_thoughts: bool = False,
-    allow_only_inner_thoughts: bool = False,
-    inner_thoughts_field_name: str = "thoughts_and_reasoning",
-    add_request_heartbeat: bool = False,
-    request_heartbeat_field_name: str = "request_heartbeat",
-    request_heartbeat_models: List[str] = None,
-):
-    """
-    Generate GBNF grammar and documentation for a list of Pydantic models.
-
-    Args:
-        pydantic_model_list: List of Pydantic model classes.
-        outer_object_name (str): Outer object name for the GBNF grammar. If None, no outer object will be generated. Eg. "function" for function calling.
-        outer_object_content (str): Content for the outer rule in the GBNF grammar. E.g., "function_parameters" or "params" for function calling.
-        model_prefix (str): Prefix for the model section in the documentation.
-        fields_prefix (str): Prefix for the fields section in the documentation.
-        list_of_outputs (bool): Whether the output is a list of items.
-        documentation_with_field_description (bool): Include field descriptions in the documentation.
-        add_inner_thoughts (bool): Add inner thoughts to the grammar. This is useful for adding comments or reasoning to the output.
-        allow_only_inner_thoughts (bool): Allow only inner thoughts. If True, only inner thoughts will be allowed in the output.
-        inner_thoughts_field_name (str): Field name for inner thoughts. Default is "thoughts_and_reasoning".
-        add_request_heartbeat (bool): Add request heartbeat to the grammar. This allows the LLM to decide when to return control to the system.
-        request_heartbeat_field_name (str): Field name for request heartbeat. Default is "request_heartbeat".
-        request_heartbeat_models (List[str]): List of models that will have a request heartbeat field.
-
-    Returns:
-        tuple: GBNF grammar string, documentation string.
-    """
-    documentation = generate_text_documentation(
-        copy(pydantic_model_list),
-        model_prefix,
-        fields_prefix,
-        documentation_with_field_description=documentation_with_field_description,
-    )
-    grammar = generate_gbnf_grammar_from_pydantic_models(
-        pydantic_model_list,
-        outer_object_name,
-        outer_object_content,
-        list_of_outputs,
-        add_inner_thoughts,
-        allow_only_inner_thoughts,
-        inner_thoughts_field_name,
-        add_request_heartbeat,
-        request_heartbeat_field_name,
-        request_heartbeat_models,
-    )
-    grammar = remove_empty_lines(grammar + get_primitive_grammar(grammar))
-    return grammar, documentation
-
-
-def generate_gbnf_grammar_and_documentation_from_dictionaries(
-    dictionaries: list[dict[str, Any]],
-    outer_object_name: str | None = None,
-    outer_object_content: str | None = None,
-    model_prefix: str = "Output Model",
-    fields_prefix: str = "Output Fields",
-    list_of_outputs: bool = False,
-    documentation_with_field_description=True,
-    add_inner_thoughts: bool = False,
-    allow_only_inner_thoughts: bool = False,
-    inner_thoughts_field_name: str = "thoughts_and_reasoning",
-    add_request_heartbeat: bool = False,
-    request_heartbeat_field_name: str = "request_heartbeat",
-    request_heartbeat_models: List[str] = None,
-):
-    """
-    Generate GBNF grammar and documentation from a list of dictionaries.
-
-    Args:
-        dictionaries (list[dict]): List of dictionaries representing Pydantic models.
-        outer_object_name (str): Outer object name for the GBNF grammar. If None, no outer object will be generated. Eg. "function" for function calling.
-        outer_object_content (str): Content for the outer rule in the GBNF grammar. Eg. "function_parameters" or "params" for function calling.
-        model_prefix (str): Prefix for the model section in the documentation.
-        fields_prefix (str): Prefix for the fields section in the documentation.
-        list_of_outputs (bool): Whether the output is a list of items.
-        documentation_with_field_description (bool): Include field descriptions in the documentation.
-        add_inner_thoughts (bool): Add inner thoughts to the grammar. This is useful for adding comments or reasoning to the output.
-        allow_only_inner_thoughts (bool): Allow only inner thoughts. If True, only inner thoughts will be allowed in the output.
-        inner_thoughts_field_name (str): Field name for inner thoughts. Default is "thoughts_and_reasoning".
-        add_request_heartbeat (bool): Add request heartbeat to the grammar. This allows the LLM to decide when to return control to the system.
-        request_heartbeat_field_name (str): Field name for request heartbeat. Default is "request_heartbeat".
-        request_heartbeat_models (List[str]): List of models that will have a request heartbeat field.
-
-    Returns:
-        tuple: GBNF grammar string, documentation string.
-    """
-    pydantic_model_list = create_dynamic_models_from_dictionaries(dictionaries)
-    documentation = generate_markdown_documentation(
-        copy(pydantic_model_list),
-        model_prefix,
-        fields_prefix,
-        documentation_with_field_description=documentation_with_field_description,
-    )
-    grammar = generate_gbnf_grammar_from_pydantic_models(
-        pydantic_model_list,
-        outer_object_name,
-        outer_object_content,
-        list_of_outputs,
-        add_inner_thoughts,
-        allow_only_inner_thoughts,
-        inner_thoughts_field_name,
-        add_request_heartbeat,
-        request_heartbeat_field_name,
-        request_heartbeat_models,
-    )
-    grammar = remove_empty_lines(grammar + get_primitive_grammar(grammar))
-    return grammar, documentation
-
-
-def create_dynamic_model_from_function(
-    func: Callable[..., Any],
-    add_inner_thoughts: bool = False,
-    inner_thoughts_field_name: str = "inner_thoughts",
-):
-    """
-    Creates a dynamic Pydantic model from a given function's type hints and adds the function as a 'run' method.
-
-    Args:
-        func (Callable): A function with type hints from which to create the model.
-        add_inner_thoughts (bool): Add an 'inner_thoughts' field at the params level to the model. Default is False.
-        inner_thoughts_field_name (str): Field name for inner thoughts. Default is "inner_thoughts".
-
-    Returns:
-        A dynamic Pydantic model class with the provided function as a 'run' method.
-    """
-
-    # Get the signature of the function
-    sig = inspect.signature(func)
-
-    # Parse the docstring
-    assert func.__doc__ is not None
-    docstring = parse(func.__doc__)
-
-    dynamic_fields = {}
-    param_docs = []
-    if add_inner_thoughts:
-        dynamic_fields[inner_thoughts_field_name] = (str, None)
-    for param in sig.parameters.values():
-        # Exclude 'self' parameter
-        if param.name == "self":
-            continue
-
-        # Assert that the parameter has a type annotation
-        if param.annotation == inspect.Parameter.empty:
-            raise TypeError(
-                f"Parameter '{param.name}' in function '{func.__name__}' lacks a type annotation"
-            )
-
-        # Find the parameter's description in the docstring
-        param_doc = next(
-            (d for d in docstring.params if d.arg_name == param.name), None
-        )
-
-        # Assert that the parameter has a description
-        if not param_doc or not param_doc.description:
-            raise ValueError(
-                f"Parameter '{param.name}' in function '{func.__name__}' lacks a description in the docstring"
-            )
-
-        # Add parameter details to the schema
-        param_docs.append((param.name, param_doc))
-        if param.default == inspect.Parameter.empty:
-            default_value = ...
-        else:
-            default_value = param.default
-        dynamic_fields[param.name] = (
-            param.annotation if param.annotation != inspect.Parameter.empty else str,
-            default_value,
-        )
-
-    # Creating the dynamic model
-    dynamic_model = create_model(f"{func.__name__}", **dynamic_fields)  # type: ignore[call-overload]
-    if add_inner_thoughts:
-        dynamic_model.model_fields[inner_thoughts_field_name].description = (
-            "Deep inner monologue private to you only."
-        )
-    for name, param_doc in param_docs:
-        dynamic_model.model_fields[name].description = param_doc.description
-
-    dynamic_model.__doc__ = (
-        (docstring.short_description if docstring.short_description is not None else "")
-        + "\n"
-        + (docstring.long_description if docstring.long_description is not None else "")
-    )
-
-    def run_method_wrapper(self):
-        func_args = {name: getattr(self, name) for name, _ in dynamic_fields.items()}
-        return func(**func_args)
-
-    # Adding the wrapped function as a 'run' method
-    setattr(dynamic_model, "run", run_method_wrapper)
-    return dynamic_model
-
-
-def add_run_method_to_dynamic_model(model: type[BaseModel], func: Callable[..., Any]):
-    """
-    Add a 'run' method to a dynamic Pydantic model, using the provided function.
-
-    Args:
-        model (type[BaseModel]): Dynamic Pydantic model class.
-        func (Callable): Function to be added as a 'run' method to the model.
-
-    Returns:
-        type[BaseModel]: Pydantic model class with the added 'run' method.
-    """
-
-    def run_method_wrapper(self):
-        func_args = {name: getattr(self, name) for name in model.model_fields}
-        return func(**func_args)
-
-    # Adding the wrapped function as a 'run' method
-    setattr(model, "run", run_method_wrapper)
-
-    return model
-
-
-def create_dynamic_models_from_dictionaries(dictionaries: list[dict[str, Any]]):
-    """
-    Create a list of dynamic Pydantic model classes from a list of dictionaries.
-
-    Args:
-        dictionaries (list[dict]): List of dictionaries representing model structures.
-
-    Returns:
-        list[Type[BaseModel]]: List of generated dynamic Pydantic model classes.
-    """
-    dynamic_models = []
-    for func in dictionaries:
-        model_name = format_model_and_field_name(func.get("name", ""))
-        dyn_model = convert_dictionary_to_pydantic_model(func, model_name)
-        dynamic_models.append(dyn_model)
-    return dynamic_models
-
-
-def map_grammar_names_to_pydantic_model_class(pydantic_model_list):
-    output = {}
-    for model in pydantic_model_list:
-        output[format_model_and_field_name(model.__name__)] = model
-
-    return output
-
-
-from enum import Enum
-
-
-def json_schema_to_python_types(schema):
-    type_map = {
-        "any": Any,
-        "string": str,
-        "number": float,
-        "integer": int,
-        "boolean": bool,
-        "array": list,
-    }
-    return type_map[schema]
-
-
-def list_to_enum(enum_name, values):
-    return Enum(enum_name, {value: value for value in values})
-
-
-def convert_dictionary_to_pydantic_model(
-    dictionary: dict[str, Any],
-    model_name: str = "CustomModel",
-    docs: dict[str, str] = None,
-    docs_function: dict[str, str] = None,
-) -> type[Any]:
-    """
-    Convert a dictionary to a Pydantic model class.
-
-    Args:
-        dictionary (dict): Dictionary representing the model structure.
-        model_name (str): Name of the generated Pydantic model.
-
-    Returns:
-        type[BaseModel]: Generated Pydantic model class.
-    """
-    fields: dict[str, Any] = {}
-    if docs is None:
-        docs = {}
-    if docs_function is None:
-        docs_function = {}
-    if "properties" in dictionary:
-        for field_name, field_data in dictionary.get("properties", {}).items():
-            if field_data == "object":
-                submodel = convert_dictionary_to_pydantic_model(
-                    dictionary, f"{model_name}_{field_name}", docs, docs_function
-                )
-                fields[field_name] = (submodel, ...)
-
-            else:
-                field_type = field_data.get("type", "string")
-                if field_data.get("description", None):
-                    docs[field_name] = field_data["description"]
-                if field_data.get("enum", []):
-                    fields[field_name] = (
-                        list_to_enum(field_name, field_data.get("enum", [])),
-                        ...,
-                    )
-                elif field_type == "array":
-                    items = field_data.get("items", {})
-                    if items != {}:
-                        array = {"properties": items}
-                        array_type = convert_dictionary_to_pydantic_model(
-                            array,
-                            f"{model_name}_{field_name}_items",
-                            docs,
-                            docs_function,
-                        )
-                        fields[field_name] = (List[array_type], ...)  # type: ignore[valid-type]
-                    else:
-                        fields[field_name] = (list, ...)
-                elif field_type == "object":
-                    submodel = convert_dictionary_to_pydantic_model(
-                        field_data, f"{model_name}_{field_name}", docs, docs_function
-                    )
-                    fields[field_name] = (submodel, ...)
-                elif field_type == "required":
-                    required = field_data
-                    for key, field in fields.items():
-                        if key not in required:
-                            fields[key] = (Optional[fields[key][0]], ...)
-                else:
-                    field_type = json_schema_to_python_types(field_type)
-                    fields[field_name] = (field_type, ...)
-    if "function" in dictionary:
-        for field_name, field_data in dictionary.get("function", {}).items():
-            if field_name == "name":
-                model_name = field_data
-            elif field_name == "description":
-                docs_function["__doc__"] = field_data
-            elif field_name == "parameters":
-                return convert_dictionary_to_pydantic_model(
-                    field_data, f"{model_name}", docs, docs_function
-                )
-
-    if "parameters" in dictionary:
-        field_data = {"function": dictionary}
-        return convert_dictionary_to_pydantic_model(
-            field_data, f"{model_name}", docs, docs_function
-        )
-    if "required" in dictionary:
-        required = dictionary.get("required", [])
-        for key, field in fields.items():
-            if key not in required:
-                fields[key] = (Optional[fields[key][0]], ...)
-    custom_model = create_model(model_name, **fields)
-
-    if "__doc__" in docs_function:
-        custom_model.__doc__ = docs_function["__doc__"]
-    for field_name, doc in docs.items():
-        custom_model.model_fields[field_name].description = doc
-
-    return custom_model
+from __future__ import annotations
+
+import inspect
+import json
+import re
+import typing
+from copy import copy
+from enum import Enum
+from inspect import getdoc, isclass
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    List,
+    Optional,
+    Union,
+    get_args,
+    get_origin,
+    get_type_hints,
+)
+
+from docstring_parser import parse
+from pydantic import BaseModel, Field, create_model
+
+if TYPE_CHECKING:
+    from types import GenericAlias
+    from types import UnionType
+else:
+    # python 3.8 compat
+    from typing import _GenericAlias as GenericAlias
+    from types import UnionType
+
+
+class PydanticDataType(Enum):
+    """
+    Defines the data types supported by the grammar_generator.
+
+    Attributes:
+        STRING (str): Represents a string data type.
+        BOOLEAN (str): Represents a boolean data type.
+        INTEGER (str): Represents an integer data type.
+        FLOAT (str): Represents a float data type.
+        OBJECT (str): Represents an object data type.
+        ARRAY (str): Represents an array data type.
+        ENUM (str): Represents an enum data type.
+        CUSTOM_CLASS (str): Represents a custom class data type.
+    """
+
+    STRING = "string"
+    TRIPLE_QUOTED_STRING = "triple_quoted_string"
+    MARKDOWN_CODE_BLOCK = "markdown_code_block"
+    BOOLEAN = "boolean"
+    INTEGER = "number"
+    FLOAT = "number"
+    OBJECT = "object"
+    ARRAY = "array"
+    ENUM = "enum"
+    ANY = "any"
+    NULL = "null"
+    CUSTOM_CLASS = "custom-class"
+    CUSTOM_DICT = "custom-dict"
+    SET = "set"
+
+
+def map_pydantic_type_to_gbnf(pydantic_type: type[Any]) -> str:
+    if isclass(pydantic_type) and issubclass(pydantic_type, str):
+        return PydanticDataType.STRING.value
+    elif isclass(pydantic_type) and issubclass(pydantic_type, bool):
+        return PydanticDataType.BOOLEAN.value
+    elif isclass(pydantic_type) and issubclass(pydantic_type, int):
+        return PydanticDataType.INTEGER.value
+    elif isclass(pydantic_type) and issubclass(pydantic_type, float):
+        return PydanticDataType.FLOAT.value
+    elif isclass(pydantic_type) and issubclass(pydantic_type, Enum):
+        return PydanticDataType.ENUM.value
+
+    elif isclass(pydantic_type) and issubclass(pydantic_type, BaseModel):
+        return format_model_and_field_name(pydantic_type.__name__)
+    elif get_origin(pydantic_type) is list:
+        element_type = get_args(pydantic_type)[0]
+        return f"{map_pydantic_type_to_gbnf(element_type)}-list"
+    elif get_origin(pydantic_type) is set:
+        element_type = get_args(pydantic_type)[0]
+        return f"{map_pydantic_type_to_gbnf(element_type)}-set"
+    elif get_origin(pydantic_type) is Union or isinstance(pydantic_type, UnionType):
+        union_types = get_args(pydantic_type)
+        union_rules = [map_pydantic_type_to_gbnf(ut) for ut in union_types]
+        return f"union-{'-or-'.join(union_rules)}"
+    elif get_origin(pydantic_type) is Optional:
+        element_type = get_args(pydantic_type)[0]
+        return f"optional-{map_pydantic_type_to_gbnf(element_type)}"
+    elif isclass(pydantic_type):
+        return f"{PydanticDataType.CUSTOM_CLASS.value}-{format_model_and_field_name(pydantic_type.__name__)}"
+    elif get_origin(pydantic_type) is dict:
+        key_type, value_type = get_args(pydantic_type)
+        return f"custom-dict-key-type-{format_model_and_field_name(map_pydantic_type_to_gbnf(key_type))}-value-type-{format_model_and_field_name(map_pydantic_type_to_gbnf(value_type))}"
+    else:
+        return "unknown"
+
+
+def format_model_and_field_name(model_name: str) -> str:
+    parts = re.findall("[A-Z][^A-Z]*", model_name)
+    if not parts:  # Check if the list is empty
+        return model_name.lower().replace("_", "-")
+    return "-".join(part.lower().replace("_", "-") for part in parts)
+
+
+def generate_list_rule(element_type):
+    """
+    Generate a GBNF rule for a list of a given element type.
+
+    :param element_type: The type of the elements in the list (e.g., 'string').
+    :return: A string representing the GBNF rule for a list of the given type.
+    """
+    rule_name = f"{map_pydantic_type_to_gbnf(element_type)}-list"
+    element_rule = map_pydantic_type_to_gbnf(element_type)
+    list_rule = rf'{rule_name} ::= "["  {element_rule} (","  {element_rule})* "]"'
+    return list_rule
+
+
+def get_members_structure(cls, rule_name):
+    if issubclass(cls, Enum):
+        # Handle Enum types
+        members = [
+            f'"\\"{member.value}\\""' for name, member in cls.__members__.items()
+        ]
+        return f"{cls.__name__.lower()} ::= " + " | ".join(members)
+    if cls.__annotations__ and cls.__annotations__ != {}:
+        result = f'{rule_name} ::= "{{"'
+        # Modify this comprehension
+        members = [
+            f'  "\\"{name}\\"" ":"  {map_pydantic_type_to_gbnf(param_type)}'
+            for name, param_type in cls.__annotations__.items()
+            if name != "self"
+        ]
+
+        result += '"," '.join(members)
+        result += '  "}"'
+        return result
+    if rule_name == "custom-class-any":
+        result = f"{rule_name} ::= "
+        result += "value"
+        return result
+
+    init_signature = inspect.signature(cls.__init__)
+    parameters = init_signature.parameters
+    result = f'{rule_name} ::=  "{{"'
+    # Modify this comprehension too
+    members = [
+        f'  "\\"{name}\\"" ":"  {map_pydantic_type_to_gbnf(param.annotation)}'
+        for name, param in parameters.items()
+        if name != "self" and param.annotation != inspect.Parameter.empty
+    ]
+
+    result += '", "'.join(members)
+    result += '  "}"'
+    return result
+
+
+def regex_to_gbnf(regex_pattern: str) -> str:
+    """
+    Translate a basic regex pattern to a GBNF rule.
+    Note: This function handles only a subset of simple regex patterns.
+    """
+    gbnf_rule = regex_pattern
+
+    # Translate common regex components to GBNF
+    gbnf_rule = gbnf_rule.replace("\\d", "[0-9]")
+    gbnf_rule = gbnf_rule.replace("\\s", "[ \t\n]")
+
+    # Handle quantifiers and other regex syntax that is similar in GBNF
+    # (e.g., '*', '+', '?', character classes)
+
+    return gbnf_rule
+
+
+def generate_gbnf_integer_rules(max_digit=None, min_digit=None):
+    """
+
+    Generate GBNF Integer Rules
+
+    Generates GBNF (Generalized Backus-Naur Form) rules for integers based on the given maximum and minimum digits.
+
+    Parameters:
+        max_digit (int): The maximum number of digits for the integer. Default is None.
+        min_digit (int): The minimum number of digits for the integer. Default is None.
+
+    Returns:
+        integer_rule (str): The identifier for the integer rule generated.
+        additional_rules (list): A list of additional rules generated based on the given maximum and minimum digits.
+
+    """
+    additional_rules = []
+
+    # Define the rule identifier based on max_digit and min_digit
+    integer_rule = "integer-part"
+    if max_digit is not None:
+        integer_rule += f"-max{max_digit}"
+    if min_digit is not None:
+        integer_rule += f"-min{min_digit}"
+
+    # Handling Integer Rules
+    if max_digit is not None or min_digit is not None:
+        # Start with an empty rule part
+        integer_rule_part = ""
+
+        # Add mandatory digits as per min_digit
+        if min_digit is not None:
+            integer_rule_part += "[0-9] " * min_digit
+
+        # Add optional digits up to max_digit
+        if max_digit is not None:
+            optional_digits = max_digit - (min_digit if min_digit is not None else 0)
+            integer_rule_part += "".join(["[0-9]? " for _ in range(optional_digits)])
+
+        # Trim the rule part and append it to additional rules
+        integer_rule_part = integer_rule_part.strip()
+        if integer_rule_part:
+            additional_rules.append(f"{integer_rule} ::= {integer_rule_part}")
+
+    return integer_rule, additional_rules
+
+
+def generate_gbnf_float_rules(
+    max_digit=None, min_digit=None, max_precision=None, min_precision=None
+):
+    """
+    Generate GBNF float rules based on the given constraints.
+
+    :param max_digit: Maximum number of digits in the integer part (default: None)
+    :param min_digit: Minimum number of digits in the integer part (default: None)
+    :param max_precision: Maximum number of digits in the fractional part (default: None)
+    :param min_precision: Minimum number of digits in the fractional part (default: None)
+    :return: A tuple containing the float rule and additional rules as a list
+
+    Example Usage:
+    max_digit = 3
+    min_digit = 1
+    max_precision = 2
+    min_precision = 1
+    generate_gbnf_float_rules(max_digit, min_digit, max_precision, min_precision)
+
+    Output:
+    ('float-3-1-2-1', ['integer-part-max3-min1 ::= [0-9] [0-9] [0-9]?', 'fractional-part-max2-min1 ::= [0-9] [0-9]?', 'float-3-1-2-1 ::= integer-part-max3-min1 "." fractional-part-max2-min
+    *1'])
+
+    Note:
+    GBNF stands for Generalized Backus-Naur Form, which is a notation technique to specify the syntax of programming languages or other formal grammars.
+    """
+    additional_rules = []
+
+    # Define the integer part rule
+    integer_part_rule = (
+        "integer-part"
+        + (f"-max{max_digit}" if max_digit is not None else "")
+        + (f"-min{min_digit}" if min_digit is not None else "")
+    )
+
+    # Define the fractional part rule based on precision constraints
+    fractional_part_rule = "fractional-part"
+    fractional_rule_part = ""
+    if max_precision is not None or min_precision is not None:
+        fractional_part_rule += (
+            f"-max{max_precision}" if max_precision is not None else ""
+        ) + (f"-min{min_precision}" if min_precision is not None else "")
+        # Minimum number of digits
+        fractional_rule_part = "[0-9]" * (
+            min_precision if min_precision is not None else 1
+        )
+        # Optional additional digits
+        fractional_rule_part += "".join(
+            [" [0-9]?"]
+            * (
+                (max_precision - (min_precision if min_precision is not None else 1))
+                if max_precision is not None
+                else 0
+            )
+        )
+        additional_rules.append(f"{fractional_part_rule} ::= {fractional_rule_part}")
+
+    # Define the float rule
+    float_rule = f"float-{max_digit if max_digit is not None else 'X'}-{min_digit if min_digit is not None else 'X'}-{max_precision if max_precision is not None else 'X'}-{min_precision if min_precision is not None else 'X'}"
+    additional_rules.append(
+        f'{float_rule} ::= {integer_part_rule} "." {fractional_part_rule}'
+    )
+
+    # Generating the integer part rule definition, if necessary
+    if max_digit is not None or min_digit is not None:
+        integer_rule_part = "[0-9]"
+        if min_digit is not None and min_digit > 1:
+            integer_rule_part += " [0-9]" * (min_digit - 1)
+        if max_digit is not None:
+            integer_rule_part += "".join(
+                [" [0-9]?"] * (max_digit - (min_digit if min_digit is not None else 1))
+            )
+        additional_rules.append(f"{integer_part_rule} ::= {integer_rule_part.strip()}")
+
+    return float_rule, additional_rules
+
+
+def generate_gbnf_rule_for_type(
+    model_name,
+    field_name,
+    field_type,
+    is_optional,
+    processed_models,
+    created_rules,
+    field_info=None,
+) -> tuple[str, list[str]]:
+    """
+    Generate GBNF rule for a given field type.
+
+    :param model_name: Name of the model.
+
+    :param field_name: Name of the field.
+    :param field_type: Type of the field.
+    :param is_optional: Whether the field is optional.
+    :param processed_models: List of processed models.
+    :param created_rules: List of created rules.
+    :param field_info: Additional information about the field (optional).
+
+    :return: Tuple containing the GBNF type and a list of additional rules.
+    :rtype: tuple[str, list]
+    """
+    rules = []
+
+    field_name = format_model_and_field_name(field_name)
+    gbnf_type = map_pydantic_type_to_gbnf(field_type)
+
+    if isclass(field_type) and issubclass(field_type, BaseModel):
+        nested_model_name = format_model_and_field_name(field_type.__name__)
+        nested_model_rules, _ = generate_gbnf_grammar(
+            field_type, processed_models, created_rules
+        )
+        rules.extend(nested_model_rules)
+        gbnf_type, rules = nested_model_name, rules
+    elif isclass(field_type) and issubclass(field_type, Enum):
+        enum_values = [
+            f'"\\"{e.value}\\""' for e in field_type
+        ]  # Adding escaped quotes
+        enum_rule = f"{model_name}-{field_name} ::= {' | '.join(enum_values)}"
+        rules.append(enum_rule)
+        gbnf_type, rules = model_name + "-" + field_name, rules
+    elif get_origin(field_type) == list:  # Array
+        element_type = get_args(field_type)[0]
+        element_rule_name, additional_rules = generate_gbnf_rule_for_type(
+            model_name,
+            f"{field_name}-element",
+            element_type,
+            is_optional,
+            processed_models,
+            created_rules,
+        )
+        rules.extend(additional_rules)
+        array_rule = rf"""{model_name}-{field_name} ::= "[" ws ({element_rule_name})? ("," ws {element_rule_name})* ws "]" """
+        rules.append(array_rule)
+        gbnf_type, rules = model_name + "-" + field_name, rules
+
+    elif get_origin(field_type) == set or field_type == set:  # Array
+        element_type = get_args(field_type)[0]
+        element_rule_name, additional_rules = generate_gbnf_rule_for_type(
+            model_name,
+            f"{field_name}-element",
+            element_type,
+            is_optional,
+            processed_models,
+            created_rules,
+        )
+        rules.extend(additional_rules)
+        array_rule = rf"""{model_name}-{field_name} ::= "[" ws ({element_rule_name})? ("," ws {element_rule_name})* ws "]" """
+        rules.append(array_rule)
+        gbnf_type, rules = model_name + "-" + field_name, rules
+
+    elif gbnf_type.startswith("custom-class-"):
+        rules.append(get_members_structure(field_type, gbnf_type))
+    elif gbnf_type.startswith("custom-dict-"):
+        key_type, value_type = get_args(field_type)
+
+        additional_key_type, additional_key_rules = generate_gbnf_rule_for_type(
+            model_name,
+            f"{field_name}-key-type",
+            key_type,
+            is_optional,
+            processed_models,
+            created_rules,
+        )
+        additional_value_type, additional_value_rules = generate_gbnf_rule_for_type(
+            model_name,
+            f"{field_name}-value-type",
+            value_type,
+            is_optional,
+            processed_models,
+            created_rules,
+        )
+        rules.extend(
+            [
+                rf'{gbnf_type} ::= "{{"  ( {additional_key_type} ": "  {additional_value_type} ("," "\n" ws {additional_key_type} ":"  {additional_value_type})*  )? "}}" '
+            ]
+        )
+        rules.extend(additional_key_rules)
+        rules.extend(additional_value_rules)
+    elif gbnf_type.startswith("union-"):
+        union_types = get_args(field_type)
+        union_rules = []
+
+        for union_type in union_types:
+            if isinstance(union_type, GenericAlias):
+                union_gbnf_type, union_rules_list = generate_gbnf_rule_for_type(
+                    model_name,
+                    field_name,
+                    union_type,
+                    False,
+                    processed_models,
+                    created_rules,
+                )
+                union_rules.append(union_gbnf_type)
+                rules.extend(union_rules_list)
+
+            elif not issubclass(union_type, type(None)):
+                union_gbnf_type, union_rules_list = generate_gbnf_rule_for_type(
+                    model_name,
+                    field_name,
+                    union_type,
+                    False,
+                    processed_models,
+                    created_rules,
+                )
+                union_rules.append(union_gbnf_type)
+                rules.extend(union_rules_list)
+
+        # Defining the union grammar rule separately
+        if len(union_rules) == 1:
+            union_grammar_rule = f"{model_name}-{field_name}-optional ::= {' | '.join(union_rules)} | null"
+        else:
+            uni = []
+            for rule in union_rules:
+                if rule not in uni:
+                    uni.append(rule)
+            union_grammar_rule = (
+                f"{model_name}-{field_name}-union ::= {' | '.join(uni)}"
+            )
+        rules.append(union_grammar_rule)
+        if len(union_rules) == 1:
+            gbnf_type = f"{model_name}-{field_name}-optional"
+        else:
+            gbnf_type = f"{model_name}-{field_name}-union"
+    elif isclass(field_type) and issubclass(field_type, str):
+        if (
+            field_info
+            and hasattr(field_info, "json_schema_extra")
+            and field_info.json_schema_extra is not None
+        ):
+            triple_quoted_string = field_info.json_schema_extra.get(
+                "triple_quoted_string", False
+            )
+            markdown_string = field_info.json_schema_extra.get(
+                "markdown_code_block", False
+            )
+
+            gbnf_type = (
+                PydanticDataType.TRIPLE_QUOTED_STRING.value
+                if triple_quoted_string
+                else PydanticDataType.STRING.value
+            )
+            gbnf_type = (
+                PydanticDataType.MARKDOWN_CODE_BLOCK.value
+                if markdown_string
+                else gbnf_type
+            )
+
+        elif field_info and hasattr(field_info, "pattern"):
+            # Convert regex pattern to grammar rule
+            regex_pattern = field_info.regex.pattern
+            gbnf_type = f"pattern-{field_name} ::= {regex_to_gbnf(regex_pattern)}"
+        else:
+            gbnf_type = PydanticDataType.STRING.value
+
+    elif (
+        isclass(field_type)
+        and issubclass(field_type, float)
+        and field_info
+        and hasattr(field_info, "json_schema_extra")
+        and field_info.json_schema_extra is not None
+    ):
+        # Retrieve precision attributes for floats
+        max_precision = (
+            field_info.json_schema_extra.get("max_precision")
+            if field_info and hasattr(field_info, "json_schema_extra")
+            else None
+        )
+        min_precision = (
+            field_info.json_schema_extra.get("min_precision")
+            if field_info and hasattr(field_info, "json_schema_extra")
+            else None
+        )
+        max_digits = (
+            field_info.json_schema_extra.get("max_digit")
+            if field_info and hasattr(field_info, "json_schema_extra")
+            else None
+        )
+        min_digits = (
+            field_info.json_schema_extra.get("min_digit")
+            if field_info and hasattr(field_info, "json_schema_extra")
+            else None
+        )
+
+        # Generate GBNF rule for float with given attributes
+        gbnf_type, rules = generate_gbnf_float_rules(
+            max_digit=max_digits,
+            min_digit=min_digits,
+            max_precision=max_precision,
+            min_precision=min_precision,
+        )
+
+    elif (
+        isclass(field_type)
+        and issubclass(field_type, int)
+        and field_info
+        and hasattr(field_info, "json_schema_extra")
+        and field_info.json_schema_extra is not None
+    ):
+        # Retrieve digit attributes for integers
+        max_digits = (
+            field_info.json_schema_extra.get("max_digit")
+            if field_info and hasattr(field_info, "json_schema_extra")
+            else None
+        )
+        min_digits = (
+            field_info.json_schema_extra.get("min_digit")
+            if field_info and hasattr(field_info, "json_schema_extra")
+            else None
+        )
+
+        # Generate GBNF rule for integer with given attributes
+        gbnf_type, rules = generate_gbnf_integer_rules(
+            max_digit=max_digits, min_digit=min_digits
+        )
+    else:
+        gbnf_type, rules = gbnf_type, []
+
+    return gbnf_type, rules
+
+
+def generate_gbnf_grammar(
+    model: type[BaseModel],
+    processed_models: set[type[BaseModel]],
+    created_rules: dict[str, list[str]],
+) -> tuple[list[str], bool]:
+    """
+
+    Generate GBnF Grammar
+
+    Generates a GBnF grammar for a given model.
+
+    :param model: A Pydantic model class to generate the grammar for. Must be a subclass of BaseModel.
+    :param processed_models: A set of already processed models to prevent infinite recursion.
+    :param created_rules: A dict containing already created rules to prevent duplicates.
+    :return: A list of GBnF grammar rules in string format. And two booleans indicating if an extra markdown or triple quoted string is in the grammar.
+    Example Usage:
+    ```
+    model = MyModel
+    processed_models = set()
+    created_rules = dict()
+
+    gbnf_grammar = generate_gbnf_grammar(model, processed_models, created_rules)
+    ```
+    """
+    if model in processed_models:
+        return [], False
+
+    processed_models.add(model)
+    model_name = format_model_and_field_name(model.__name__)
+
+    if not issubclass(model, BaseModel):
+        # For non-Pydantic classes, generate model_fields from __annotations__ or __init__
+        if hasattr(model, "__annotations__") and model.__annotations__:
+            model_fields = {
+                name: (typ, ...) for name, typ in model.__annotations__.items()
+            }
+        else:
+            init_signature = inspect.signature(model.__init__)
+            parameters = init_signature.parameters
+            model_fields = {
+                name: (param.annotation, param.default)
+                for name, param in parameters.items()
+                if name != "self"
+            }
+    else:
+        # For Pydantic models, use model_fields and check for ellipsis (required fields)
+        model_fields = model.__annotations__
+
+    model_rule_parts = []
+    nested_rules = []
+    has_markdown_code_block = False
+    has_triple_quoted_string = False
+    look_for_markdown_code_block = False
+    look_for_triple_quoted_string = False
+    for field_name, field_info in model_fields.items():
+        if not issubclass(model, BaseModel):
+            field_type, default_value = field_info
+            # Check if the field is optional (not required)
+            is_optional = (default_value is not inspect.Parameter.empty) and (
+                default_value is not Ellipsis
+            )
+        else:
+            field_type = field_info
+            field_info = model.model_fields[field_name]
+            is_optional = (
+                field_info.is_required is False and get_origin(field_type) is Optional
+            )
+        rule_name, additional_rules = generate_gbnf_rule_for_type(
+            model_name,
+            format_model_and_field_name(field_name),
+            field_type,
+            is_optional,
+            processed_models,
+            created_rules,
+            field_info,
+        )
+        look_for_markdown_code_block = (
+            True if rule_name == "markdown_code_block" else False
+        )
+        look_for_triple_quoted_string = (
+            True if rule_name == "triple_quoted_string" else False
+        )
+        if not look_for_markdown_code_block and not look_for_triple_quoted_string:
+            if rule_name not in created_rules:
+                created_rules[rule_name] = additional_rules
+            model_rule_parts.append(
+                f' ws "\\"{field_name}\\"" ": " {rule_name}'
+            )  # Adding escaped quotes
+            nested_rules.extend(additional_rules)
+        else:
+            has_triple_quoted_string = look_for_triple_quoted_string
+            has_markdown_code_block = look_for_markdown_code_block
+
+    fields_joined = r' "," '.join(model_rule_parts)
+    if fields_joined != "":
+        model_rule = rf'{model_name} ::= "{{" {fields_joined} ws "}}"'
+    else:
+        model_rule = rf'{model_name} ::= "{{" "}}"'
+
+    has_special_string = False
+    if has_triple_quoted_string:
+        model_rule += '"\\n" ws "}"'
+        model_rule += '"\\n" triple-quoted-string'
+        has_special_string = True
+    if has_markdown_code_block:
+        model_rule += '"\\n" ws "}"'
+        model_rule += '"\\n" markdown-code-block'
+        has_special_string = True
+    all_rules = [model_rule] + nested_rules
+
+    return all_rules, has_special_string
+
+
+def generate_gbnf_grammar_from_pydantic_models(
+    models: list[type[BaseModel]],
+    outer_object_name: str | None = None,
+    outer_object_content: str | None = None,
+    list_of_outputs: bool = False,
+    add_inner_thoughts: bool = True,
+    allow_only_inner_thoughts: bool = True,
+    inner_thought_field_name: str = "chain_of_thought",
+    add_request_heartbeat: bool = True,
+    request_heartbeat_field_name: str = "request_heartbeat",
+    request_heartbeat_models: list[str] = None,
+) -> str:
+    """
+    Generate GBNF Grammar from Pydantic Models.
+
+    This method takes a list of Pydantic models and uses them to generate a GBNF grammar string. The generated grammar string can be used for parsing and validating data using the generated
+    * grammar.
+
+    Args:
+        models (list[type[BaseModel]]): A list of Pydantic models to generate the grammar from.
+        outer_object_name (str): Outer object name for the GBNF grammar. If None, no outer object will be generated. Eg. "function" for function calling.
+        outer_object_content (str): Content for the outer rule in the GBNF grammar. Eg. "function_parameters" or "params" for function calling.
+        list_of_outputs (str, optional): Allows a list of output objects
+        add_inner_thoughts (bool, optional): Add inner thoughts to the grammar. Defaults to True.
+        allow_only_inner_thoughts (bool, optional): Allow only inner thoughts. Defaults to True.
+    Returns:
+        str: The generated GBNF grammar string.
+
+    Examples:
+        models = [UserModel, PostModel]
+        grammar = generate_gbnf_grammar_from_pydantic(models)
+        print(grammar)
+        # Output:
+        # root ::= UserModel | PostModel
+        # ...
+    """
+    if request_heartbeat_models is None:
+        request_heartbeat_models = []
+    processed_models: set[type[BaseModel]] = set()
+    all_rules = []
+    created_rules: dict[str, list[str]] = {}
+    if outer_object_name is None:
+        for model in models:
+            model_rules, _ = generate_gbnf_grammar(
+                model, processed_models, created_rules
+            )
+            all_rules.extend(model_rules)
+
+        if list_of_outputs:
+            root_rule = (
+                r'root ::= (" "| "\n") "[" ws grammar-models ("," ws grammar-models)* "\n" "]"'
+                + "\n"
+            )
+        else:
+            root_rule = r'root ::= (" "| "\n") grammar-models' + "\n"
+        root_rule += "grammar-models ::= " + " | ".join(
+            [format_model_and_field_name(model.__name__) for model in models]
+        )
+        all_rules.insert(0, root_rule)
+        return "\n".join(all_rules)
+    elif outer_object_name is not None:
+        if list_of_outputs:
+            root_rule = (
+                rf'root ::= (" "| "\n") "[" ws {format_model_and_field_name(outer_object_name)} ("," ws {format_model_and_field_name(outer_object_name)})* "\n" "]"'
+                + "\n"
+            )
+        else:
+            root_rule = f"root ::= {format_model_and_field_name(outer_object_name)}\n"
+
+        if add_inner_thoughts:
+            if allow_only_inner_thoughts:
+                model_rule = rf'{format_model_and_field_name(outer_object_name)} ::= (" "| "\n") "{{" ws "\"{inner_thought_field_name}\""  ":" ws string (("," ws "\"{outer_object_name}\""  ":" ws grammar-models)? | ws "}}")'
+            else:
+                model_rule = rf'{format_model_and_field_name(outer_object_name)} ::= (" "| "\n") "{{" ws "\"{inner_thought_field_name}\""  ":" ws string "," ws "\"{outer_object_name}\""  ":" ws grammar-models '
+        else:
+            model_rule = rf'{format_model_and_field_name(outer_object_name)} ::= (" "| "\n") "{{" ws "\"{outer_object_name}\""  ": " ws grammar-models'
+
+        fields_joined = " | ".join(
+            [
+                rf"{format_model_and_field_name(model.__name__)}-grammar-model"
+                for model in models
+            ]
+        )
+
+        grammar_model_rules = f"\ngrammar-models ::= {fields_joined}"
+        mod_rules = []
+        for model in models:
+            mod_rule = (
+                rf"{format_model_and_field_name(model.__name__)}-grammar-model ::= "
+            )
+            mod_rule += (
+                rf'"\"{model.__name__}\"" "," ws "\"{outer_object_content}\"" ": " {format_model_and_field_name(model.__name__)}'
+                + "\n"
+            )
+            mod_rules.append(mod_rule)
+        grammar_model_rules += "\n" + "\n".join(mod_rules)
+
+        for model in models:
+            model_rules, has_special_string = generate_gbnf_grammar(
+                model, processed_models, created_rules
+            )
+            if add_request_heartbeat and model.__name__ in request_heartbeat_models:
+                model_rules[
+                    0
+                ] += rf' "," ws "\"{request_heartbeat_field_name}\""  ":" ws boolean '
+            if not has_special_string:
+                model_rules[0] += r' ws "}"'
+
+            all_rules.extend(model_rules)
+
+        all_rules.insert(0, root_rule + model_rule + grammar_model_rules)
+        return "\n".join(all_rules)
+
+
+def get_primitive_grammar(grammar):
+    """
+    Returns the needed GBNF primitive grammar for a given GBNF grammar string.
+
+    Args:
+        grammar (str): The string containing the GBNF grammar.
+
+    Returns:
+        str: GBNF primitive grammar string.
+    """
+    type_list: list[type[object]] = []
+    if "string-list" in grammar:
+        type_list.append(str)
+    if "boolean-list" in grammar:
+        type_list.append(bool)
+    if "integer-list" in grammar:
+        type_list.append(int)
+    if "float-list" in grammar:
+        type_list.append(float)
+    additional_grammar = [generate_list_rule(t) for t in type_list]
+    primitive_grammar = r"""
+boolean ::= "true" | "false"
+null ::= "null"
+string ::= "\"" (
+        [^"\\] |
+        "\\" (["\\/bfnrt] | "u" [0-9a-fA-F] [0-9a-fA-F] [0-9a-fA-F] [0-9a-fA-F])
+      )* "\""
+ws ::= ([ \t\n]+)
+number ::= "-"? ([0-9]+ | [0-9]+ "." [0-9]+) ([eE] [-+]? [0-9]+)?"""
+
+    any_block = ""
+    if "custom-class-any" in grammar:
+        any_block = """
+value ::= object | array | string | number | boolean | null
+
+object ::=
+  "{" ws (
+            string ":" ws value
+    ("," ws string ":" ws value)*
+  )? "}"
+
+array  ::=
+  "[" ws (
+            value
+    ("," ws value)*
+  )? "]"
+"""
+
+    markdown_code_block_grammar = ""
+    if "markdown-code-block" in grammar:
+        markdown_code_block_grammar = r'''
+markdown-code-block ::= opening-triple-ticks markdown-code-block-content closing-triple-ticks
+markdown-code-block-content ::= ( [^`] | "`" [^`] |  "`"  "`" [^`]  )*
+opening-triple-ticks ::= "```" "python" "\n" | "```" "c" "\n" | "```" "cpp" "\n" | "```" "txt" "\n" | "```" "text" "\n" | "```" "json" "\n" | "```" "javascript" "\n" | "```" "css" "\n" | "```" "html" "\n" | "```" "markdown" "\n"
+closing-triple-ticks ::= "```" "\n"'''
+
+    if "triple-quoted-string" in grammar:
+        markdown_code_block_grammar = r"""
+triple-quoted-string ::= triple-quotes triple-quoted-string-content triple-quotes
+triple-quoted-string-content ::= ( [^'] | "'" [^'] |  "'"  "'" [^']  )*
+triple-quotes ::= "'''" """
+    return (
+        "\n"
+        + "\n".join(additional_grammar)
+        + any_block
+        + primitive_grammar
+        + markdown_code_block_grammar
+    )
+
+
+def generate_markdown_documentation(
+    pydantic_models: list[type[BaseModel]],
+    model_prefix="Model",
+    fields_prefix="Fields",
+    documentation_with_field_description=True,
+) -> str:
+    """
+    Generate markdown documentation for a list of Pydantic models.
+
+    Args:
+        pydantic_models (list[type[BaseModel]]): list of Pydantic model classes.
+        model_prefix (str): Prefix for the model section.
+        fields_prefix (str): Prefix for the fields section.
+        documentation_with_field_description (bool): Include field descriptions in the documentation.
+
+    Returns:
+        str: Generated text documentation.
+    """
+    documentation = "## Functions\n\n"
+    pyd_models = [(model, True) for model in pydantic_models]
+    for model, add_prefix in pyd_models:
+        if add_prefix:
+            documentation += f"### {model.__name__}\n"
+        else:
+            documentation += f"### {model.__name__}\n"
+
+        # Handling multi-line model description with proper indentation
+
+        class_doc = getdoc(model)
+        base_class_doc = getdoc(BaseModel)
+        class_description = (
+            class_doc if class_doc and class_doc != base_class_doc else ""
+        )
+        if class_description != "":
+            documentation += format_multiline_description(class_description, 0) + "\n"
+
+        if add_prefix:
+            # Indenting the fields section
+            documentation += f"{fields_prefix}:\n"
+        else:
+            documentation += f"Fields:\n"
+        if isclass(model) and issubclass(model, BaseModel):
+            for name, field_type in model.__annotations__.items():
+                # if name == "markdown_code_block":
+                #    continue
+                if get_origin(field_type) == list:
+                    element_type = get_args(field_type)[0]
+                    if isclass(element_type) and issubclass(element_type, BaseModel):
+                        pyd_models.append((element_type, False))
+                if get_origin(field_type) == Union:
+                    element_types = get_args(field_type)
+                    for element_type in element_types:
+                        if isclass(element_type) and issubclass(
+                            element_type, BaseModel
+                        ):
+                            pyd_models.append((element_type, False))
+                documentation += generate_field_markdown(
+                    name,
+                    field_type,
+                    model,
+                    documentation_with_field_description=documentation_with_field_description,
+                )
+            if add_prefix:
+                if documentation.endswith(f"{fields_prefix}:\n"):
+                    documentation += "none\n"
+            else:
+                if documentation.endswith("Fields:\n"):
+                    documentation += "none\n"
+            documentation += "\n"
+
+        if (
+            hasattr(model, "Config")
+            and hasattr(model.Config, "json_schema_extra")
+            and "example" in model.Config.json_schema_extra
+        ):
+            documentation += f"  Expected Example Output for {format_model_and_field_name(model.__name__)}:\n"
+            json_example = json.dumps(model.Config.json_schema_extra["example"])
+            documentation += format_multiline_description(json_example, 2) + "\n"
+
+    return documentation
+
+
+def generate_field_markdown(
+    field_name: str,
+    field_type: type[Any],
+    model: type[BaseModel],
+    depth=1,
+    documentation_with_field_description=True,
+) -> str:
+    """
+    Generate markdown documentation for a Pydantic model field.
+
+    Args:
+        field_name (str): Name of the field.
+        field_type (type[Any]): Type of the field.
+        model (type[BaseModel]): Pydantic model class.
+        depth (int): Indentation depth in the documentation.
+        documentation_with_field_description (bool): Include field descriptions in the documentation.
+
+    Returns:
+        str: Generated text documentation for the field.
+    """
+    indent = "  " * depth
+
+    field_info = model.model_fields.get(field_name)
+    field_description = (
+        field_info.description if field_info and field_info.description else ""
+    )
+
+    if get_origin(field_type) == list:
+        element_type = get_args(field_type)[0]
+        field_text = f"{indent}{field_name} ({format_model_and_field_name(field_type.__name__)} of {format_model_and_field_name(element_type.__name__)})"
+        if field_description != "":
+            field_text += ": "
+        else:
+            field_text += "\n"
+    elif get_origin(field_type) == Union or isinstance(field_type, UnionType):
+        element_types = get_args(field_type)
+        types = []
+        for element_type in element_types:
+            if element_type.__name__ == "NoneType":
+                types.append("null")
+            else:
+                types.append(format_model_and_field_name(element_type.__name__))
+        field_text = f"{indent}{field_name} ({' or '.join(types)})"
+        if field_description != "":
+            field_text += ": "
+        else:
+            field_text += "\n"
+
+    elif issubclass(field_type, Enum):
+        enum_values = [f"'{str(member.value)}'" for member in field_type]
+
+        field_text = f"{indent}{field_name} ({' or '.join(enum_values)})"
+        if field_description != "":
+            field_text += ": "
+        else:
+            field_text += "\n"
+
+    else:
+        field_text = (
+            f"{indent}{field_name} ({format_model_and_field_name(field_type.__name__)})"
+        )
+        if field_description != "":
+            field_text += ": "
+        else:
+            field_text += "\n"
+
+    if not documentation_with_field_description:
+        return field_text
+
+    if field_description != "":
+        field_text += field_description + "\n"
+
+    # Check for and include field-specific examples if available
+    if (
+        hasattr(model, "Config")
+        and hasattr(model.Config, "json_schema_extra")
+        and "example" in model.Config.json_schema_extra
+    ):
+        field_example = model.Config.json_schema_extra["example"].get(field_name)
+        if field_example is not None:
+            example_text = (
+                f"'{field_example}'"
+                if isinstance(field_example, str)
+                else field_example
+            )
+            field_text += f"{indent}  Example: {example_text}\n"
+
+    if isclass(field_type) and issubclass(field_type, BaseModel):
+        field_text += f"{indent}  Details:\n"
+        for name, type_ in field_type.__annotations__.items():
+            field_text += generate_field_markdown(name, type_, field_type, depth + 2)
+
+    return field_text
+
+
+def format_json_example(example: dict[str, Any], depth: int) -> str:
+    """
+    Format a JSON example into a readable string with indentation.
+
+    Args:
+        example (dict): JSON example to be formatted.
+        depth (int): Indentation depth.
+
+    Returns:
+        str: Formatted JSON example string.
+    """
+    indent = "    " * depth
+    formatted_example = "{\n"
+    for key, value in example.items():
+        value_text = f"'{value}'" if isinstance(value, str) else value
+        formatted_example += f"{indent}{key}: {value_text},\n"
+    formatted_example = formatted_example.rstrip(",\n") + "\n" + indent + "}"
+    return formatted_example
+
+
+def generate_text_documentation(
+    pydantic_models: list[type[BaseModel]],
+    model_prefix="Model",
+    fields_prefix="Fields",
+    documentation_with_field_description=True,
+) -> str:
+    """
+    Generate markdown documentation for a list of Pydantic models.
+
+    Args:
+        pydantic_models (list[type[BaseModel]]): list of Pydantic model classes.
+        model_prefix (str): Prefix for the model section.
+        fields_prefix (str): Prefix for the fields section.
+        documentation_with_field_description (bool): Include field descriptions in the documentation.
+
+    Returns:
+        str: Generated text documentation.
+    """
+    documentation = ""
+    pyd_models = [(model, True) for model in pydantic_models]
+    for model, add_prefix in pyd_models:
+        if add_prefix:
+            documentation += f"{model_prefix}: {model.__name__}\n"
+        else:
+            documentation += f"model: {model.__name__}\n"
+
+        # Handling multi-line model description with proper indentation
+
+        class_doc = getdoc(model)
+        base_class_doc = getdoc(BaseModel)
+        class_description = (
+            class_doc if class_doc and class_doc != base_class_doc else ""
+        )
+        if class_description != "":
+            documentation += "  description: "
+            documentation += format_multiline_description(class_description, 2) + "\n"
+
+        if add_prefix:
+            # Indenting the fields section
+            documentation += f"  {fields_prefix}:\n"
+        else:
+            documentation += f"  fields:\n"
+        if isclass(model) and issubclass(model, BaseModel):
+            for name, field_type in model.__annotations__.items():
+                # if name == "markdown_code_block":
+                #    continue
+                if get_origin(field_type) == list:
+                    element_type = get_args(field_type)[0]
+                    if isclass(element_type) and issubclass(element_type, BaseModel):
+                        pyd_models.append((element_type, False))
+                    if get_origin(element_type) == Union or isinstance(
+                        element_type, UnionType
+                    ):
+                        element_types = get_args(element_type)
+                        for element_type in element_types:
+                            if isclass(element_type) and issubclass(
+                                element_type, BaseModel
+                            ):
+                                pyd_models.append((element_type, False))
+                            if get_origin(element_type) == list:
+                                element_type = get_args(element_type)[0]
+                                if isclass(element_type) and issubclass(
+                                    element_type, BaseModel
+                                ):
+                                    pyd_models.append((element_type, False))
+                if get_origin(field_type) == Union or isinstance(field_type, UnionType):
+                    element_types = get_args(field_type)
+                    for element_type in element_types:
+                        if isclass(element_type) and issubclass(
+                            element_type, BaseModel
+                        ):
+                            pyd_models.append((element_type, False))
+                        if get_origin(element_type) == list:
+                            element_type = get_args(element_type)[0]
+                            if isclass(element_type) and issubclass(
+                                element_type, BaseModel
+                            ):
+                                pyd_models.append((element_type, False))
+                if isclass(field_type) and issubclass(field_type, BaseModel):
+                    pyd_models.append((field_type, False))
+                documentation += generate_field_text(
+                    name,
+                    field_type,
+                    model,
+                    documentation_with_field_description=documentation_with_field_description,
+                )
+            if add_prefix:
+                if documentation.endswith(f"{fields_prefix}:\n"):
+                    documentation += "    none\n"
+            else:
+                if documentation.endswith("fields:\n"):
+                    documentation += "    none\n"
+            documentation += "\n"
+
+        if (
+            hasattr(model, "Config")
+            and hasattr(model.Config, "json_schema_extra")
+            and "example" in model.Config.json_schema_extra
+        ):
+            documentation += f"  Expected Example Output for {format_model_and_field_name(model.__name__)}:\n"
+            json_example = json.dumps(model.Config.json_schema_extra["example"])
+            documentation += format_multiline_description(json_example, 2) + "\n"
+
+    return documentation
+
+
+def generate_field_text(
+    field_name: str,
+    field_type: type[Any],
+    model: type[BaseModel],
+    depth=1,
+    documentation_with_field_description=True,
+) -> str:
+    """
+    Generate markdown documentation for a Pydantic model field.
+
+    Args:
+        field_name (str): Name of the field.
+        field_type (type[Any]): Type of the field.
+        model (type[BaseModel]): Pydantic model class.
+        depth (int): Indentation depth in the documentation.
+        documentation_with_field_description (bool): Include field descriptions in the documentation.
+
+    Returns:
+        str: Generated text documentation for the field.
+    """
+    indent = "    " * depth
+
+    field_info = model.model_fields.get(field_name)
+    field_description = (
+        field_info.description if field_info and field_info.description else ""
+    )
+
+    if get_origin(field_type) == list:
+        element_type = get_args(field_type)[0]
+        if get_origin(element_type) == Union or isinstance(element_type, UnionType):
+            element_types = get_args(element_type)
+            types = []
+            for element_type in element_types:
+                if element_type.__name__ == "NoneType":
+                    types.append("null")
+                else:
+                    if isclass(element_type) and issubclass(element_type, Enum):
+                        enum_values = [
+                            f"'{str(member.value)}'" for member in element_type
+                        ]
+                        for enum_value in enum_values:
+                            types.append(enum_value)
+
+                    else:
+                        if get_origin(element_type) == list:
+                            element_type = get_args(element_type)[0]
+                            types.append(f"(list of {element_type.__name__})")
+                        else:
+                            types.append(element_type.__name__)
+            field_text = f"({' or '.join(types)})"
+            field_text = f"{indent}{field_name} ({field_type.__name__} of {field_text})"
+            if field_description != "":
+                field_text += ": "
+            else:
+                field_text += "\n"
+        else:
+            field_text = f"{indent}{field_name} ({field_type.__name__} of {element_type.__name__})"
+            if field_description != "":
+                field_text += ": "
+            else:
+                field_text += "\n"
+    elif get_origin(field_type) == Union:
+        element_types = get_args(field_type)
+        types = []
+        for element_type in element_types:
+            if element_type.__name__ == "NoneType":
+                types.append("null")
+            else:
+                if isclass(element_type) and issubclass(element_type, Enum):
+                    enum_values = [f"'{str(member.value)}'" for member in element_type]
+                    for enum_value in enum_values:
+                        types.append(enum_value)
+
+                else:
+                    if get_origin(element_type) == list:
+                        element_type = get_args(element_type)[0]
+                        types.append(f"(list of {element_type.__name__})")
+                    else:
+                        types.append(element_type.__name__)
+        field_text = f"{indent}{field_name} ({' or '.join(types)})"
+        if field_description != "":
+            field_text += ": "
+        else:
+            field_text += "\n"
+    elif isinstance(field_type, GenericAlias):
+        if field_type.__origin__ == dict:
+            key_type, value_type = get_args(field_type)
+
+            additional_key_type = key_type.__name__
+            additional_value_type = value_type.__name__
+            field_text = f"{indent}{field_name} (dict of {additional_key_type} to {additional_value_type})"
+            if field_description != "":
+                field_text += ": "
+            else:
+                field_text += "\n"
+        elif field_type.__origin__ == list:
+            element_type = get_args(field_type)[0]
+            field_text = f"{indent}{field_name} (list of {element_type.__name__})"
+            if field_description != "":
+                field_text += ": "
+            else:
+                field_text += "\n"
+    elif issubclass(field_type, Enum):
+        enum_values = [f"'{str(member.value)}'" for member in field_type]
+
+        field_text = f"{indent}{field_name} ({' or '.join(enum_values)})"
+        if field_description != "":
+            field_text += ": "
+        else:
+            field_text += "\n"
+
+    else:
+        field_text = (
+            f"{indent}{field_name} ({format_model_and_field_name(field_type.__name__)})"
+        )
+        if field_description != "":
+            field_text += ": "
+        else:
+            field_text += "\n"
+
+    if not documentation_with_field_description:
+        return field_text
+
+    if field_description != "":
+        field_text += field_description + "\n"
+
+    # Check for and include field-specific examples if available
+    if (
+        hasattr(model, "Config")
+        and hasattr(model.Config, "json_schema_extra")
+        and "example" in model.Config.json_schema_extra
+    ):
+        field_example = model.Config.json_schema_extra["example"].get(field_name)
+        if field_example is not None:
+            example_text = (
+                f"'{field_example}'"
+                if isinstance(field_example, str)
+                else field_example
+            )
+            field_text += f"{indent}  Example: {example_text}\n"
+
+    return field_text
+
+
+def format_multiline_description(description: str, indent_level: int) -> str:
+    """
+    Format a multiline description with proper indentation.
+
+    Args:
+        description (str): Multiline description.
+        indent_level (int): Indentation level.
+
+    Returns:
+        str: Formatted multiline description.
+    """
+    indent = "  " * indent_level
+    return description.replace("\n", "\n" + indent)
+
+
+def save_gbnf_grammar_and_documentation(
+    grammar,
+    documentation,
+    grammar_file_path="./grammar.gbnf",
+    documentation_file_path="./grammar_documentation.md",
+):
+    """
+    Save GBNF grammar and documentation to specified files.
+
+    Args:
+        grammar (str): GBNF grammar string.
+        documentation (str): Documentation string.
+        grammar_file_path (str): File path to save the GBNF grammar.
+        documentation_file_path (str): File path to save the documentation.
+
+    Returns:
+        None
+    """
+    try:
+        with open(grammar_file_path, "w") as file:
+            file.write(grammar + get_primitive_grammar(grammar))
+        print(f"Grammar successfully saved to {grammar_file_path}")
+    except IOError as e:
+        print(f"An error occurred while saving the grammar file: {e}")
+
+    try:
+        with open(documentation_file_path, "w") as file:
+            file.write(documentation)
+        print(f"Documentation successfully saved to {documentation_file_path}")
+    except IOError as e:
+        print(f"An error occurred while saving the documentation file: {e}")
+
+
+def remove_empty_lines(string):
+    """
+    Remove empty lines from a string.
+
+    Args:
+        string (str): Input string.
+
+    Returns:
+        str: String with empty lines removed.
+    """
+    lines = string.splitlines()
+    non_empty_lines = [line for line in lines if line.strip() != ""]
+    string_no_empty_lines = "\n".join(non_empty_lines)
+    return string_no_empty_lines
+
+
+def generate_and_save_gbnf_grammar_and_documentation(
+    pydantic_model_list,
+    grammar_file_path="./generated_grammar.gbnf",
+    documentation_file_path="./generated_grammar_documentation.md",
+    outer_object_name: str | None = None,
+    outer_object_content: str | None = None,
+    model_prefix: str = "Output Model",
+    fields_prefix: str = "Output Fields",
+    list_of_outputs: bool = False,
+    documentation_with_field_description=True,
+    add_inner_thoughts: bool = False,
+    allow_only_inner_thoughts: bool = False,
+    inner_thoughts_field_name: str = "thoughts_and_reasoning",
+    add_request_heartbeat: bool = False,
+    request_heartbeat_field_name: str = "request_heartbeat",
+    request_heartbeat_models: List[str] = None,
+):
+    """
+    Generate GBNF grammar and documentation, and save them to specified files.
+
+    Args:
+        pydantic_model_list: List of Pydantic model classes.
+        grammar_file_path (str): File path to save the generated GBNF grammar.
+        documentation_file_path (str): File path to save the generated documentation.
+        outer_object_name (str): Outer object name for the GBNF grammar. If None, no outer object will be generated. Eg. "function" for function calling.
+        outer_object_content (str): Content for the outer rule in the GBNF grammar. Eg. "function_parameters" or "params" for function calling.
+        model_prefix (str): Prefix for the model section in the documentation.
+        fields_prefix (str): Prefix for the fields section in the documentation.
+        list_of_outputs (bool): Whether the output is a list of items.
+        documentation_with_field_description (bool): Include field descriptions in the documentation.
+        add_inner_thoughts (bool): Add inner thoughts to the grammar. This is useful for adding comments or reasoning to the output.
+        allow_only_inner_thoughts (bool): Allow only inner thoughts. If True, only inner thoughts will be allowed in the output.
+        inner_thoughts_field_name (str): Field name for inner thoughts. Default is "thoughts_and_reasoning".
+        add_request_heartbeat (bool): Add request heartbeat to the grammar. This allows the LLM to decide when to return control to the system.
+        request_heartbeat_field_name (str): Field name for request heartbeat. Default is "request_heartbeat".
+        request_heartbeat_models (List[str]): List of models that will have a request heartbeat field.
+    Returns:
+        None
+    """
+    documentation = generate_markdown_documentation(
+        pydantic_model_list,
+        model_prefix,
+        fields_prefix,
+        documentation_with_field_description=documentation_with_field_description,
+    )
+    grammar = generate_gbnf_grammar_from_pydantic_models(
+        pydantic_model_list,
+        outer_object_name,
+        outer_object_content,
+        list_of_outputs,
+        add_inner_thoughts,
+        allow_only_inner_thoughts,
+        inner_thoughts_field_name,
+        add_request_heartbeat,
+        request_heartbeat_field_name,
+        request_heartbeat_models,
+    )
+    grammar = remove_empty_lines(grammar)
+    save_gbnf_grammar_and_documentation(
+        grammar, documentation, grammar_file_path, documentation_file_path
+    )
+
+
+def generate_gbnf_grammar_and_documentation(
+    pydantic_model_list,
+    outer_object_name: str | None = None,
+    outer_object_content: str | None = None,
+    model_prefix: str = "Output Model",
+    fields_prefix: str = "Output Fields",
+    list_of_outputs: bool = False,
+    documentation_with_field_description=True,
+    add_inner_thoughts: bool = False,
+    allow_only_inner_thoughts: bool = False,
+    inner_thoughts_field_name: str = "thoughts_and_reasoning",
+    add_request_heartbeat: bool = False,
+    request_heartbeat_field_name: str = "request_heartbeat",
+    request_heartbeat_models: List[str] = None,
+):
+    """
+    Generate GBNF grammar and documentation for a list of Pydantic models.
+
+    Args:
+        pydantic_model_list: List of Pydantic model classes.
+        outer_object_name (str): Outer object name for the GBNF grammar. If None, no outer object will be generated. Eg. "function" for function calling.
+        outer_object_content (str): Content for the outer rule in the GBNF grammar. E.g., "function_parameters" or "params" for function calling.
+        model_prefix (str): Prefix for the model section in the documentation.
+        fields_prefix (str): Prefix for the fields section in the documentation.
+        list_of_outputs (bool): Whether the output is a list of items.
+        documentation_with_field_description (bool): Include field descriptions in the documentation.
+        add_inner_thoughts (bool): Add inner thoughts to the grammar. This is useful for adding comments or reasoning to the output.
+        allow_only_inner_thoughts (bool): Allow only inner thoughts. If True, only inner thoughts will be allowed in the output.
+        inner_thoughts_field_name (str): Field name for inner thoughts. Default is "thoughts_and_reasoning".
+        add_request_heartbeat (bool): Add request heartbeat to the grammar. This allows the LLM to decide when to return control to the system.
+        request_heartbeat_field_name (str): Field name for request heartbeat. Default is "request_heartbeat".
+        request_heartbeat_models (List[str]): List of models that will have a request heartbeat field.
+
+    Returns:
+        tuple: GBNF grammar string, documentation string.
+    """
+    documentation = generate_text_documentation(
+        copy(pydantic_model_list),
+        model_prefix,
+        fields_prefix,
+        documentation_with_field_description=documentation_with_field_description,
+    )
+    grammar = generate_gbnf_grammar_from_pydantic_models(
+        pydantic_model_list,
+        outer_object_name,
+        outer_object_content,
+        list_of_outputs,
+        add_inner_thoughts,
+        allow_only_inner_thoughts,
+        inner_thoughts_field_name,
+        add_request_heartbeat,
+        request_heartbeat_field_name,
+        request_heartbeat_models,
+    )
+    grammar = remove_empty_lines(grammar + get_primitive_grammar(grammar))
+    return grammar, documentation
+
+
+def generate_gbnf_grammar_and_documentation_from_dictionaries(
+    dictionaries: list[dict[str, Any]],
+    outer_object_name: str | None = None,
+    outer_object_content: str | None = None,
+    model_prefix: str = "Output Model",
+    fields_prefix: str = "Output Fields",
+    list_of_outputs: bool = False,
+    documentation_with_field_description=True,
+    add_inner_thoughts: bool = False,
+    allow_only_inner_thoughts: bool = False,
+    inner_thoughts_field_name: str = "thoughts_and_reasoning",
+    add_request_heartbeat: bool = False,
+    request_heartbeat_field_name: str = "request_heartbeat",
+    request_heartbeat_models: List[str] = None,
+):
+    """
+    Generate GBNF grammar and documentation from a list of dictionaries.
+
+    Args:
+        dictionaries (list[dict]): List of dictionaries representing Pydantic models.
+        outer_object_name (str): Outer object name for the GBNF grammar. If None, no outer object will be generated. Eg. "function" for function calling.
+        outer_object_content (str): Content for the outer rule in the GBNF grammar. Eg. "function_parameters" or "params" for function calling.
+        model_prefix (str): Prefix for the model section in the documentation.
+        fields_prefix (str): Prefix for the fields section in the documentation.
+        list_of_outputs (bool): Whether the output is a list of items.
+        documentation_with_field_description (bool): Include field descriptions in the documentation.
+        add_inner_thoughts (bool): Add inner thoughts to the grammar. This is useful for adding comments or reasoning to the output.
+        allow_only_inner_thoughts (bool): Allow only inner thoughts. If True, only inner thoughts will be allowed in the output.
+        inner_thoughts_field_name (str): Field name for inner thoughts. Default is "thoughts_and_reasoning".
+        add_request_heartbeat (bool): Add request heartbeat to the grammar. This allows the LLM to decide when to return control to the system.
+        request_heartbeat_field_name (str): Field name for request heartbeat. Default is "request_heartbeat".
+        request_heartbeat_models (List[str]): List of models that will have a request heartbeat field.
+
+    Returns:
+        tuple: GBNF grammar string, documentation string.
+    """
+    pydantic_model_list = create_dynamic_models_from_dictionaries(dictionaries)
+    documentation = generate_markdown_documentation(
+        copy(pydantic_model_list),
+        model_prefix,
+        fields_prefix,
+        documentation_with_field_description=documentation_with_field_description,
+    )
+    grammar = generate_gbnf_grammar_from_pydantic_models(
+        pydantic_model_list,
+        outer_object_name,
+        outer_object_content,
+        list_of_outputs,
+        add_inner_thoughts,
+        allow_only_inner_thoughts,
+        inner_thoughts_field_name,
+        add_request_heartbeat,
+        request_heartbeat_field_name,
+        request_heartbeat_models,
+    )
+    grammar = remove_empty_lines(grammar + get_primitive_grammar(grammar))
+    return grammar, documentation
+
+
+def create_dynamic_model_from_function(
+    func: Callable[..., Any],
+    add_inner_thoughts: bool = False,
+    inner_thoughts_field_name: str = "inner_thoughts",
+):
+    """
+    Creates a dynamic Pydantic model from a given function's type hints and adds the function as a 'run' method.
+
+    Args:
+        func (Callable): A function with type hints from which to create the model.
+        add_inner_thoughts (bool): Add an 'inner_thoughts' field at the params level to the model. Default is False.
+        inner_thoughts_field_name (str): Field name for inner thoughts. Default is "inner_thoughts".
+
+    Returns:
+        A dynamic Pydantic model class with the provided function as a 'run' method.
+    """
+
+    # Get the signature of the function
+    sig = inspect.signature(func)
+
+    # Parse the docstring
+    assert func.__doc__ is not None
+    docstring = parse(func.__doc__)
+
+    dynamic_fields = {}
+    param_docs = []
+    if add_inner_thoughts:
+        dynamic_fields[inner_thoughts_field_name] = (str, None)
+    for param in sig.parameters.values():
+        # Exclude 'self' parameter
+        if param.name == "self":
+            continue
+
+        # Assert that the parameter has a type annotation
+        if param.annotation == inspect.Parameter.empty:
+            raise TypeError(
+                f"Parameter '{param.name}' in function '{func.__name__}' lacks a type annotation"
+            )
+
+        # Find the parameter's description in the docstring
+        param_doc = next(
+            (d for d in docstring.params if d.arg_name == param.name), None
+        )
+
+        # Assert that the parameter has a description
+        if not param_doc or not param_doc.description:
+            raise ValueError(
+                f"Parameter '{param.name}' in function '{func.__name__}' lacks a description in the docstring"
+            )
+
+        # Add parameter details to the schema
+        param_docs.append((param.name, param_doc))
+        if param.default == inspect.Parameter.empty:
+            default_value = ...
+        else:
+            default_value = param.default
+        dynamic_fields[param.name] = (
+            param.annotation if param.annotation != inspect.Parameter.empty else str,
+            default_value,
+        )
+
+    # Creating the dynamic model
+    dynamic_model = create_model(f"{func.__name__}", **dynamic_fields)  # type: ignore[call-overload]
+    if add_inner_thoughts:
+        dynamic_model.model_fields[inner_thoughts_field_name].description = (
+            "Deep inner monologue private to you only."
+        )
+    for name, param_doc in param_docs:
+        dynamic_model.model_fields[name].description = param_doc.description
+
+    dynamic_model.__doc__ = (
+        (docstring.short_description if docstring.short_description is not None else "")
+        + "\n"
+        + (docstring.long_description if docstring.long_description is not None else "")
+    )
+
+    def run_method_wrapper(self):
+        func_args = {name: getattr(self, name) for name, _ in dynamic_fields.items()}
+        return func(**func_args)
+
+    # Adding the wrapped function as a 'run' method
+    setattr(dynamic_model, "run", run_method_wrapper)
+    return dynamic_model
+
+
+def add_run_method_to_dynamic_model(model: type[BaseModel], func: Callable[..., Any]):
+    """
+    Add a 'run' method to a dynamic Pydantic model, using the provided function.
+
+    Args:
+        model (type[BaseModel]): Dynamic Pydantic model class.
+        func (Callable): Function to be added as a 'run' method to the model.
+
+    Returns:
+        type[BaseModel]: Pydantic model class with the added 'run' method.
+    """
+
+    def run_method_wrapper(self):
+        func_args = {name: getattr(self, name) for name in model.model_fields}
+        return func(**func_args)
+
+    # Adding the wrapped function as a 'run' method
+    setattr(model, "run", run_method_wrapper)
+
+    return model
+
+
+def create_dynamic_models_from_dictionaries(dictionaries: list[dict[str, Any]]):
+    """
+    Create a list of dynamic Pydantic model classes from a list of dictionaries.
+
+    Args:
+        dictionaries (list[dict]): List of dictionaries representing model structures.
+
+    Returns:
+        list[Type[BaseModel]]: List of generated dynamic Pydantic model classes.
+    """
+    dynamic_models = []
+    for func in dictionaries:
+        model_name = format_model_and_field_name(func.get("name", ""))
+        dyn_model = convert_dictionary_to_pydantic_model(func, model_name)
+        dynamic_models.append(dyn_model)
+    return dynamic_models
+
+
+def map_grammar_names_to_pydantic_model_class(pydantic_model_list):
+    output = {}
+    for model in pydantic_model_list:
+        output[format_model_and_field_name(model.__name__)] = model
+
+    return output
+
+
+from enum import Enum
+
+
+def json_schema_to_python_types(schema):
+    type_map = {
+        "any": Any,
+        "string": str,
+        "number": float,
+        "integer": int,
+        "boolean": bool,
+        "array": list,
+    }
+    return type_map[schema]
+
+
+def list_to_enum(enum_name, values):
+    return Enum(enum_name, {value: value for value in values})
+
+
+def convert_dictionary_to_pydantic_model(
+    dictionary: dict[str, Any],
+    model_name: str = "CustomModel",
+    docs: dict[str, str] = None,
+    docs_function: dict[str, str] = None,
+) -> type[Any]:
+    """
+    Convert a dictionary to a Pydantic model class.
+
+    Args:
+        dictionary (dict): Dictionary representing the model structure.
+        model_name (str): Name of the generated Pydantic model.
+
+    Returns:
+        type[BaseModel]: Generated Pydantic model class.
+    """
+    fields: dict[str, Any] = {}
+    if docs is None:
+        docs = {}
+    if docs_function is None:
+        docs_function = {}
+    if "properties" in dictionary:
+        for field_name, field_data in dictionary.get("properties", {}).items():
+            if field_data == "object":
+                submodel = convert_dictionary_to_pydantic_model(
+                    dictionary, f"{model_name}_{field_name}", docs, docs_function
+                )
+                fields[field_name] = (submodel, ...)
+
+            else:
+                field_type = field_data.get("type", "string")
+                if field_data.get("description", None):
+                    docs[field_name] = field_data["description"]
+                if field_data.get("enum", []):
+                    fields[field_name] = (
+                        list_to_enum(field_name, field_data.get("enum", [])),
+                        ...,
+                    )
+                elif field_type == "array":
+                    items = field_data.get("items", {})
+                    if items != {}:
+                        array = {"properties": items}
+                        array_type = convert_dictionary_to_pydantic_model(
+                            array,
+                            f"{model_name}_{field_name}_items",
+                            docs,
+                            docs_function,
+                        )
+                        fields[field_name] = (List[array_type], ...)  # type: ignore[valid-type]
+                    else:
+                        fields[field_name] = (list, ...)
+                elif field_type == "object":
+                    submodel = convert_dictionary_to_pydantic_model(
+                        field_data, f"{model_name}_{field_name}", docs, docs_function
+                    )
+                    fields[field_name] = (submodel, ...)
+                elif field_type == "required":
+                    required = field_data
+                    for key, field in fields.items():
+                        if key not in required:
+                            fields[key] = (Optional[fields[key][0]], ...)
+                else:
+                    field_type = json_schema_to_python_types(field_type)
+                    fields[field_name] = (field_type, ...)
+    if "function" in dictionary:
+        for field_name, field_data in dictionary.get("function", {}).items():
+            if field_name == "name":
+                model_name = field_data
+            elif field_name == "description":
+                docs_function["__doc__"] = field_data
+            elif field_name == "parameters":
+                return convert_dictionary_to_pydantic_model(
+                    field_data, f"{model_name}", docs, docs_function
+                )
+
+    if "parameters" in dictionary:
+        field_data = {"function": dictionary}
+        return convert_dictionary_to_pydantic_model(
+            field_data, f"{model_name}", docs, docs_function
+        )
+    if "required" in dictionary:
+        required = dictionary.get("required", [])
+        for key, field in fields.items():
+            if key not in required:
+                fields[key] = (Optional[fields[key][0]], ...)
+    custom_model = create_model(model_name, **fields)
+
+    if "__doc__" in docs_function:
+        custom_model.__doc__ = docs_function["__doc__"]
+    for field_name, doc in docs.items():
+        custom_model.model_fields[field_name].description = doc
+
+    return custom_model
```

### Comparing `llama_cpp_agent-0.1.3/src/llama_cpp_agent/hermes_2_pro_agent.py` & `llama_cpp_agent-0.1.4/src/llama_cpp_agent/hermes_2_pro_agent.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,323 +1,323 @@
-import json
-import random
-import re
-import string
-import uuid
-from enum import Enum
-from typing import List, Dict, Literal, Tuple
-
-from llama_cpp import Llama
-from pydantic import ValidationError
-from transformers import AutoTokenizer
-
-from llama_cpp_agent.function_calling import LlamaCppFunctionTool
-from llama_cpp_agent.llm_agent import LlamaCppAgent
-from llama_cpp_agent.llm_prompt_template import PromptTemplate
-from llama_cpp_agent.llm_settings import LlamaLLMSettings
-from llama_cpp_agent.messages import (
-    ToolCall,
-    FunctionCall,
-    ToolMessage,
-    AssistantMessage,
-    UserMessage,
-    ChatMessage,
-    convert_messages_to_list_of_dictionaries,
-    SystemMessage,
-)
-from llama_cpp_agent.messages_formatter import (
-    MessagesFormatterType,
-    get_predefined_messages_formatter,
-)
-from llama_cpp_agent.providers.llama_cpp_endpoint_provider import (
-    LlamaCppEndpointSettings,
-)
-from llama_cpp_agent.providers.openai_endpoint_provider import OpenAIEndpointSettings
-
-
-def generate_id(length=8):
-    # Characters to use in the ID
-    characters = string.ascii_letters + string.digits
-    # Random choice of characters
-    return "".join(random.choice(characters) for _ in range(length))
-
-
-def parse_tool_calls(text):
-    # List to hold all extracted dictionaries
-    json_dicts = []
-
-    # Regular expression to find <tool_call>...</tool_call> patterns
-    tool_call_pattern = r"<tool_call>(.*?)</tool_call>"
-
-    # Find all occurrences of the pattern
-    tool_calls = re.findall(tool_call_pattern, text, re.DOTALL)
-
-    # Process each JSON within the found tags
-    for json_text in tool_calls:
-        json_text = json_text.strip()
-        try:
-            json_dict = json.loads(json_text)
-            json_dicts.append(json_dict)
-        except json.JSONDecodeError as e:
-            print(f"Error decoding JSON: {e}")
-
-    return json_dicts
-
-
-class Hermes2ProMessageFormatter:
-    """
-    Class representing a messages formatter for LLMs.
-    """
-
-    def __init__(self):
-        """
-        Initializes a new MessagesFormatter object.
-        """
-        SYS_PROMPT_START_MIXTRAL = """"""
-        SYS_PROMPT_END_MIXTRAL = """\n\n"""
-        USER_PROMPT_START_MIXTRAL = """[INST] """
-        USER_PROMPT_END_MIXTRAL = """ """
-        ASSISTANT_PROMPT_START_MIXTRAL = """[/INST] """
-        ASSISTANT_PROMPT_END_MIXTRAL = """</s>"""
-        FUNCTION_PROMPT_START_MIXTRAL = """"""
-        FUNCTION_PROMPT_END_MIXTRAL = """"""
-        DEFAULT_MIXTRAL_STOP_SEQUENCES = ["</s>"]
-        self.PRE_PROMPT = ""
-        self.SYS_PROMPT_START = "<|im_start|>system\n"
-        self.SYS_PROMPT_END = "<|im_end|>\n"
-        self.USER_PROMPT_START = "<|im_start|>user\n"
-        self.USER_PROMPT_END = "<|im_end|>\n"
-        self.ASSISTANT_PROMPT_START = "<|im_start|>assistant\n"
-        self.ASSISTANT_PROMPT_END = "<|im_end|>\n"
-        self.INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE = False
-
-        self.DEFAULT_STOP_SEQUENCES = [
-            "<|im_end|>",
-            "<|im_start|>assistant",
-            "<|im_start|>user",
-            "<|im_start|>system",
-            "<|im_start|>tool",
-        ]
-        self.FUNCTION_PROMPT_START = "<|im_start|>tool\n"
-        self.FUNCTION_PROMPT_END = "<|im_end|>\n"
-        self.USE_USER_ROLE_FUNCTION_CALL_RESULT = False
-        self.STRIP_PROMPT = True
-
-    def format_messages(
-        self,
-        messages: List[Dict[str, str]],
-        response_role: Literal["user", "assistant"] | None = None,
-    ) -> Tuple[str, str]:
-        """
-        Formats a list of messages into a conversation string.
-
-        Args:
-            messages (List[Dict[str, str]]): List of messages with role and content.
-            response_role(Literal["system", "user", "assistant", "function"]|None): Forces the response role to be "system", "user" or "assistant".
-        Returns:
-            Tuple[str, str]: Formatted conversation string and the role of the last message.
-        """
-        formatted_messages = self.PRE_PROMPT
-        last_role = "assistant"
-
-        no_user_prompt_start = False
-        for message in messages:
-            if message["role"] == "system":
-                formatted_messages += (
-                    self.SYS_PROMPT_START + message["content"] + self.SYS_PROMPT_END
-                )
-                last_role = "system"
-                if self.INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE:
-                    formatted_messages = self.USER_PROMPT_START + formatted_messages
-                    no_user_prompt_start = True
-            elif message["role"] == "user":
-                if no_user_prompt_start:
-                    no_user_prompt_start = False
-                    formatted_messages += message["content"] + self.USER_PROMPT_END
-                else:
-                    formatted_messages += (
-                        self.USER_PROMPT_START
-                        + message["content"]
-                        + self.USER_PROMPT_END
-                    )
-                last_role = "user"
-            elif message["role"] == "assistant":
-                if self.STRIP_PROMPT:
-                    message["content"] = message["content"].strip()
-                formatted_messages += (
-                    self.ASSISTANT_PROMPT_START
-                    + message["content"]
-                    + self.ASSISTANT_PROMPT_END
-                )
-                last_role = "assistant"
-            elif message["role"] == "tool":
-                if isinstance(message["content"], list):
-                    message["content"] = "\n".join(
-                        [json.dumps(m, indent=2) for m in message["content"]]
-                    )
-                if self.USE_USER_ROLE_FUNCTION_CALL_RESULT:
-                    formatted_messages += (
-                        self.USER_PROMPT_START
-                        + message["content"]
-                        + self.USER_PROMPT_END
-                    )
-                    last_role = "user"
-                else:
-                    formatted_messages += (
-                        self.FUNCTION_PROMPT_START
-                        + message["content"]
-                        + self.FUNCTION_PROMPT_END
-                    )
-                    last_role = "tool"
-        if last_role == "system" or last_role == "user" or last_role == "tool":
-            if self.STRIP_PROMPT:
-                if response_role is not None:
-                    if response_role == "assistant":
-                        return (
-                            formatted_messages + self.ASSISTANT_PROMPT_START.strip(),
-                            "assistant",
-                        )
-                    if response_role == "user":
-                        return (
-                            formatted_messages + self.USER_PROMPT_START.strip(),
-                            "user",
-                        )
-                else:
-                    return (
-                        formatted_messages + self.ASSISTANT_PROMPT_START.strip(),
-                        "assistant",
-                    )
-            else:
-                if response_role is not None:
-                    if response_role == "assistant":
-                        return (
-                            formatted_messages + self.ASSISTANT_PROMPT_START,
-                            "assistant",
-                        )
-                    if response_role == "user":
-                        return formatted_messages + self.USER_PROMPT_START, "user"
-                else:
-                    return formatted_messages + self.ASSISTANT_PROMPT_START, "assistant"
-        if self.STRIP_PROMPT:
-            if response_role is not None:
-                if response_role == "assistant":
-                    return (
-                        formatted_messages + self.ASSISTANT_PROMPT_START.strip(),
-                        "assistant",
-                    )
-                if response_role == "user":
-                    return formatted_messages + self.USER_PROMPT_START.strip(), "user"
-            else:
-                return formatted_messages + self.USER_PROMPT_START.strip(), "user"
-        else:
-            if response_role is not None:
-                if response_role == "assistant":
-                    return formatted_messages + self.ASSISTANT_PROMPT_START, "assistant"
-                if response_role == "user":
-                    return formatted_messages + self.USER_PROMPT_START, "user"
-            else:
-                return formatted_messages + self.USER_PROMPT_START, "user"
-
-
-class Hermes2ProAgent:
-    def __init__(
-        self,
-        model: (
-            Llama | LlamaLLMSettings | LlamaCppEndpointSettings | OpenAIEndpointSettings
-        ),
-        system_prompt: str = None,
-        debug_output: bool = False,
-    ):
-        self.messages: list[ChatMessage] = []
-        self.agent = LlamaCppAgent(model, debug_output=debug_output)
-        self.debug_output = debug_output
-        if system_prompt is not None:
-            self.system_prompt = system_prompt
-        else:
-            self.system_prompt = "You are a function calling AI model. You are provided with function signatures within <tools></tools> XML tags. You may call one or more functions to assist with the user query. Don't make assumptions about what values to plug into functions.\nHere are the available tools:"
-        self.messages.append(SystemMessage(content="system_prompt"))
-        self.messages_formatter = Hermes2ProMessageFormatter()
-        self.sys_prompt_template = """{system_prompt} <tools> {tools} </tools>
-Use the following pydantic model json schema for each tool call you will make: {"properties": {"arguments": {"title": "Arguments", "type": "object"}, "name": {"title": "Name", "type": "string"}}, "required": ["arguments", "name"], "title": "FunctionCall", "type": "object"} 
-For each function call return a json object with function name and arguments within <tool_call></tool_call> XML tags as follows:
-<tool_call>
-{"arguments": <args-dict>, "name": <function-name>}
-</tool_call>
-"""
-        self.system_prompter = PromptTemplate.from_string(self.sys_prompt_template)
-
-    def get_response(
-        self,
-        message=None,
-        tools: list[LlamaCppFunctionTool] = None,
-        temperature=0.7,
-        top_p=1.0,
-    ):
-        if tools is None:
-            tools = []
-        if message is not None:
-            msg = UserMessage(content=message)
-            self.messages.append(msg)
-        openai_tools = []
-        openai_tool_mapping = {}
-        for tool in tools:
-            openai_tools.append(tool.to_openai_tool())
-            openai_tool_mapping[tool.model.__name__] = tool
-
-        self.messages[0].content = self.system_prompter.generate_prompt(
-            {"tools": json.dumps(openai_tools), "system_prompt": self.system_prompt}
-        )
-        text, role = self.messages_formatter.format_messages(
-            convert_messages_to_list_of_dictionaries(self.messages)
-        )
-
-        if self.debug_output:
-            print(text)
-        result = self.agent.get_text_response(
-            text,
-            temperature=temperature,
-            top_p=top_p,
-            stop_sequences=self.messages_formatter.DEFAULT_STOP_SEQUENCES,
-            stream=self.debug_output,
-            print_output=self.debug_output,
-        )
-
-        if "<tool_call>" in result:
-            tool_calls = []
-            if result.strip().endswith("</tool_call"):
-                result += ">"
-            function_calls = parse_tool_calls(result)
-            tool_messages = []
-            for function_call in function_calls:
-                tool = openai_tool_mapping[function_call["name"]]
-                cls = tool.model
-                call_parameters = function_call["arguments"]
-                try:
-                    call = cls(**call_parameters)
-                    output = call.run(**tool.additional_parameters)
-                    tool_call_id = generate_id(length=9)
-                    tool_calls.append(
-                        ToolCall(
-                            function=FunctionCall(
-                                name=function_call["name"],
-                                arguments=json.dumps(call_parameters),
-                            ),
-                            id=tool_call_id,
-                        )
-                    )
-                    tool_messages.append(
-                        ToolMessage(content=str(output), tool_call_id=tool_call_id)
-                    )
-                except ValidationError as e:
-                    tool_messages.append(ToolMessage(content=str(e), tool_call_id="-1"))
-                    self.messages.append(
-                        AssistantMessage(content=result, tool_calls=tool_calls)
-                    )
-                    self.messages.extend(tool_messages)
-            self.messages.append(
-                AssistantMessage(content=result, tool_calls=tool_calls)
-            )
-            self.messages.extend(tool_messages)
-            return self.get_response(tools=tools)
-        else:
-            self.messages.append(AssistantMessage(content=result.strip()))
-            return result.strip()
+import json
+import random
+import re
+import string
+import uuid
+from enum import Enum
+from typing import List, Dict, Literal, Tuple
+
+from llama_cpp import Llama
+from pydantic import ValidationError
+from transformers import AutoTokenizer
+
+from llama_cpp_agent.function_calling import LlamaCppFunctionTool
+from llama_cpp_agent.llm_agent import LlamaCppAgent
+from llama_cpp_agent.llm_prompt_template import PromptTemplate
+from llama_cpp_agent.llm_settings import LlamaLLMSettings
+from llama_cpp_agent.messages import (
+    ToolCall,
+    FunctionCall,
+    ToolMessage,
+    AssistantMessage,
+    UserMessage,
+    ChatMessage,
+    convert_messages_to_list_of_dictionaries,
+    SystemMessage,
+)
+from llama_cpp_agent.messages_formatter import (
+    MessagesFormatterType,
+    get_predefined_messages_formatter,
+)
+from llama_cpp_agent.providers.llama_cpp_endpoint_provider import (
+    LlamaCppEndpointSettings,
+)
+from llama_cpp_agent.providers.openai_endpoint_provider import OpenAIEndpointSettings
+
+
+def generate_id(length=8):
+    # Characters to use in the ID
+    characters = string.ascii_letters + string.digits
+    # Random choice of characters
+    return "".join(random.choice(characters) for _ in range(length))
+
+
+def parse_tool_calls(text):
+    # List to hold all extracted dictionaries
+    json_dicts = []
+
+    # Regular expression to find <tool_call>...</tool_call> patterns
+    tool_call_pattern = r"<tool_call>(.*?)</tool_call>"
+
+    # Find all occurrences of the pattern
+    tool_calls = re.findall(tool_call_pattern, text, re.DOTALL)
+
+    # Process each JSON within the found tags
+    for json_text in tool_calls:
+        json_text = json_text.strip()
+        try:
+            json_dict = json.loads(json_text)
+            json_dicts.append(json_dict)
+        except json.JSONDecodeError as e:
+            print(f"Error decoding JSON: {e}")
+
+    return json_dicts
+
+
+class Hermes2ProMessageFormatter:
+    """
+    Class representing a messages formatter for LLMs.
+    """
+
+    def __init__(self):
+        """
+        Initializes a new MessagesFormatter object.
+        """
+        SYS_PROMPT_START_MIXTRAL = """"""
+        SYS_PROMPT_END_MIXTRAL = """\n\n"""
+        USER_PROMPT_START_MIXTRAL = """[INST] """
+        USER_PROMPT_END_MIXTRAL = """ """
+        ASSISTANT_PROMPT_START_MIXTRAL = """[/INST] """
+        ASSISTANT_PROMPT_END_MIXTRAL = """</s>"""
+        FUNCTION_PROMPT_START_MIXTRAL = """"""
+        FUNCTION_PROMPT_END_MIXTRAL = """"""
+        DEFAULT_MIXTRAL_STOP_SEQUENCES = ["</s>"]
+        self.PRE_PROMPT = ""
+        self.SYS_PROMPT_START = "<|im_start|>system\n"
+        self.SYS_PROMPT_END = "<|im_end|>\n"
+        self.USER_PROMPT_START = "<|im_start|>user\n"
+        self.USER_PROMPT_END = "<|im_end|>\n"
+        self.ASSISTANT_PROMPT_START = "<|im_start|>assistant\n"
+        self.ASSISTANT_PROMPT_END = "<|im_end|>\n"
+        self.INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE = False
+
+        self.DEFAULT_STOP_SEQUENCES = [
+            "<|im_end|>",
+            "<|im_start|>assistant",
+            "<|im_start|>user",
+            "<|im_start|>system",
+            "<|im_start|>tool",
+        ]
+        self.FUNCTION_PROMPT_START = "<|im_start|>tool\n"
+        self.FUNCTION_PROMPT_END = "<|im_end|>\n"
+        self.USE_USER_ROLE_FUNCTION_CALL_RESULT = False
+        self.STRIP_PROMPT = True
+
+    def format_messages(
+        self,
+        messages: List[Dict[str, str]],
+        response_role: Literal["user", "assistant"] | None = None,
+    ) -> Tuple[str, str]:
+        """
+        Formats a list of messages into a conversation string.
+
+        Args:
+            messages (List[Dict[str, str]]): List of messages with role and content.
+            response_role(Literal["system", "user", "assistant", "function"]|None): Forces the response role to be "system", "user" or "assistant".
+        Returns:
+            Tuple[str, str]: Formatted conversation string and the role of the last message.
+        """
+        formatted_messages = self.PRE_PROMPT
+        last_role = "assistant"
+
+        no_user_prompt_start = False
+        for message in messages:
+            if message["role"] == "system":
+                formatted_messages += (
+                    self.SYS_PROMPT_START + message["content"] + self.SYS_PROMPT_END
+                )
+                last_role = "system"
+                if self.INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE:
+                    formatted_messages = self.USER_PROMPT_START + formatted_messages
+                    no_user_prompt_start = True
+            elif message["role"] == "user":
+                if no_user_prompt_start:
+                    no_user_prompt_start = False
+                    formatted_messages += message["content"] + self.USER_PROMPT_END
+                else:
+                    formatted_messages += (
+                        self.USER_PROMPT_START
+                        + message["content"]
+                        + self.USER_PROMPT_END
+                    )
+                last_role = "user"
+            elif message["role"] == "assistant":
+                if self.STRIP_PROMPT:
+                    message["content"] = message["content"].strip()
+                formatted_messages += (
+                    self.ASSISTANT_PROMPT_START
+                    + message["content"]
+                    + self.ASSISTANT_PROMPT_END
+                )
+                last_role = "assistant"
+            elif message["role"] == "tool":
+                if isinstance(message["content"], list):
+                    message["content"] = "\n".join(
+                        [json.dumps(m, indent=2) for m in message["content"]]
+                    )
+                if self.USE_USER_ROLE_FUNCTION_CALL_RESULT:
+                    formatted_messages += (
+                        self.USER_PROMPT_START
+                        + message["content"]
+                        + self.USER_PROMPT_END
+                    )
+                    last_role = "user"
+                else:
+                    formatted_messages += (
+                        self.FUNCTION_PROMPT_START
+                        + message["content"]
+                        + self.FUNCTION_PROMPT_END
+                    )
+                    last_role = "tool"
+        if last_role == "system" or last_role == "user" or last_role == "tool":
+            if self.STRIP_PROMPT:
+                if response_role is not None:
+                    if response_role == "assistant":
+                        return (
+                            formatted_messages + self.ASSISTANT_PROMPT_START.strip(),
+                            "assistant",
+                        )
+                    if response_role == "user":
+                        return (
+                            formatted_messages + self.USER_PROMPT_START.strip(),
+                            "user",
+                        )
+                else:
+                    return (
+                        formatted_messages + self.ASSISTANT_PROMPT_START.strip(),
+                        "assistant",
+                    )
+            else:
+                if response_role is not None:
+                    if response_role == "assistant":
+                        return (
+                            formatted_messages + self.ASSISTANT_PROMPT_START,
+                            "assistant",
+                        )
+                    if response_role == "user":
+                        return formatted_messages + self.USER_PROMPT_START, "user"
+                else:
+                    return formatted_messages + self.ASSISTANT_PROMPT_START, "assistant"
+        if self.STRIP_PROMPT:
+            if response_role is not None:
+                if response_role == "assistant":
+                    return (
+                        formatted_messages + self.ASSISTANT_PROMPT_START.strip(),
+                        "assistant",
+                    )
+                if response_role == "user":
+                    return formatted_messages + self.USER_PROMPT_START.strip(), "user"
+            else:
+                return formatted_messages + self.USER_PROMPT_START.strip(), "user"
+        else:
+            if response_role is not None:
+                if response_role == "assistant":
+                    return formatted_messages + self.ASSISTANT_PROMPT_START, "assistant"
+                if response_role == "user":
+                    return formatted_messages + self.USER_PROMPT_START, "user"
+            else:
+                return formatted_messages + self.USER_PROMPT_START, "user"
+
+
+class Hermes2ProAgent:
+    def __init__(
+        self,
+        model: (
+            Llama | LlamaLLMSettings | LlamaCppEndpointSettings | OpenAIEndpointSettings
+        ),
+        system_prompt: str = None,
+        debug_output: bool = False,
+    ):
+        self.messages: list[ChatMessage] = []
+        self.agent = LlamaCppAgent(model, debug_output=debug_output)
+        self.debug_output = debug_output
+        if system_prompt is not None:
+            self.system_prompt = system_prompt
+        else:
+            self.system_prompt = "You are a function calling AI model. You are provided with function signatures within <tools></tools> XML tags. You may call one or more functions to assist with the user query. Don't make assumptions about what values to plug into functions.\nHere are the available tools:"
+        self.messages.append(SystemMessage(content="system_prompt"))
+        self.messages_formatter = Hermes2ProMessageFormatter()
+        self.sys_prompt_template = """{system_prompt} <tools> {tools} </tools>
+Use the following pydantic model json schema for each tool call you will make: {"properties": {"arguments": {"title": "Arguments", "type": "object"}, "name": {"title": "Name", "type": "string"}}, "required": ["arguments", "name"], "title": "FunctionCall", "type": "object"} 
+For each function call return a json object with function name and arguments within <tool_call></tool_call> XML tags as follows:
+<tool_call>
+{"arguments": <args-dict>, "name": <function-name>}
+</tool_call>
+"""
+        self.system_prompter = PromptTemplate.from_string(self.sys_prompt_template)
+
+    def get_response(
+        self,
+        message=None,
+        tools: list[LlamaCppFunctionTool] = None,
+        temperature=0.7,
+        top_p=1.0,
+    ):
+        if tools is None:
+            tools = []
+        if message is not None:
+            msg = UserMessage(content=message)
+            self.messages.append(msg)
+        openai_tools = []
+        openai_tool_mapping = {}
+        for tool in tools:
+            openai_tools.append(tool.to_openai_tool())
+            openai_tool_mapping[tool.model.__name__] = tool
+
+        self.messages[0].content = self.system_prompter.generate_prompt(
+            {"tools": json.dumps(openai_tools), "system_prompt": self.system_prompt}
+        )
+        text, role = self.messages_formatter.format_messages(
+            convert_messages_to_list_of_dictionaries(self.messages)
+        )
+
+        if self.debug_output:
+            print(text)
+        result = self.agent.get_text_response(
+            text,
+            temperature=temperature,
+            top_p=top_p,
+            stop_sequences=self.messages_formatter.DEFAULT_STOP_SEQUENCES,
+            stream=self.debug_output,
+            print_output=self.debug_output,
+        )
+
+        if "<tool_call>" in result:
+            tool_calls = []
+            if result.strip().endswith("</tool_call"):
+                result += ">"
+            function_calls = parse_tool_calls(result)
+            tool_messages = []
+            for function_call in function_calls:
+                tool = openai_tool_mapping[function_call["name"]]
+                cls = tool.model
+                call_parameters = function_call["arguments"]
+                try:
+                    call = cls(**call_parameters)
+                    output = call.run(**tool.additional_parameters)
+                    tool_call_id = generate_id(length=9)
+                    tool_calls.append(
+                        ToolCall(
+                            function=FunctionCall(
+                                name=function_call["name"],
+                                arguments=json.dumps(call_parameters),
+                            ),
+                            id=tool_call_id,
+                        )
+                    )
+                    tool_messages.append(
+                        ToolMessage(content=str(output), tool_call_id=tool_call_id)
+                    )
+                except ValidationError as e:
+                    tool_messages.append(ToolMessage(content=str(e), tool_call_id="-1"))
+                    self.messages.append(
+                        AssistantMessage(content=result, tool_calls=tool_calls)
+                    )
+                    self.messages.extend(tool_messages)
+            self.messages.append(
+                AssistantMessage(content=result, tool_calls=tool_calls)
+            )
+            self.messages.extend(tool_messages)
+            return self.get_response(tools=tools)
+        else:
+            self.messages.append(AssistantMessage(content=result.strip()))
+            return result.strip()
```

### Comparing `llama_cpp_agent-0.1.3/src/llama_cpp_agent/llm_agent.py` & `llama_cpp_agent-0.1.4/src/llama_cpp_agent/llm_agent.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,1745 +1,1745 @@
-import json
-from copy import copy
-from dataclasses import dataclass
-from typing import List, Dict, Literal, Callable, Union
-
-from llama_cpp import Llama, LlamaGrammar
-
-from .llm_settings import LlamaLLMSettings, LlamaLLMGenerationSettings
-from .messages_formatter import (
-    MessagesFormatterType,
-    get_predefined_messages_formatter,
-    MessagesFormatter,
-)
-from .function_calling import LlamaCppFunctionTool, LlamaCppFunctionToolRegistry
-from .providers.llama_cpp_endpoint_provider import (
-    LlamaCppEndpointSettings,
-    LlamaCppGenerationSettings,
-)
-from .providers.openai_endpoint_provider import (
-    OpenAIEndpointSettings,
-    OpenAIGenerationSettings,
-)
-
-
-@dataclass
-class StreamingResponse:
-    """
-    Represents a streaming response with text and an indicator for the last response.
-    """
-
-    text: str
-    is_last_response: bool
-
-    def __init__(self, text: str, is_last_response: bool):
-        """
-        Initializes a new StreamingResponse object.
-
-        Args:
-            text (str): The text content of the streaming response.
-            is_last_response (bool): Indicates whether this is the last response in the stream.
-        """
-        self.text = text
-        self.is_last_response = is_last_response
-
-
-class LlamaCppAgent:
-    """
-    A base agent that can be used for chat, structured output and function calling.
-     Is used as part of all other agents.
-    """
-
-    def __init__(
-        self,
-        model: Union[
-            Llama, LlamaLLMSettings, LlamaCppEndpointSettings, OpenAIEndpointSettings
-        ],
-        name: str = "llamacpp_agent",
-        system_prompt: str = "You are a helpful assistant.",
-        predefined_messages_formatter_type: MessagesFormatterType = MessagesFormatterType.CHATML,
-        custom_messages_formatter: MessagesFormatter = None,
-        debug_output: bool = False,
-        function_tool_registry: LlamaCppFunctionToolRegistry = None,
-    ):
-        """
-        Initializes a new LlamaCppAgent object.
-
-        Args:
-           model (Union[Llama, LlamaLLMSettings, LlamaCppEndpointSettings]):The underlying Llama model or settings.
-           name (str): The name of the agent.
-           system_prompt (str): The system prompt used in chat interactions.
-           predefined_messages_formatter_type (MessagesFormatterType): The type of predefined messages formatter.
-           custom_messages_formatter (MessagesFormatter): Custom messages formatter.
-           debug_output (bool): Indicates whether debug output should be enabled.
-           function_tool_registry (LlamaCppFunctionToolRegistry): The Llama function tool registry.
-        """
-        if isinstance(model, LlamaLLMSettings):
-            model = Llama(**model.as_dict())
-        self.model = model
-        self.name = name
-        self.system_prompt = system_prompt
-        self.debug_output = debug_output
-        self.messages = []
-        self.grammar_cache = {}
-        if custom_messages_formatter is not None:
-            self.messages_formatter = custom_messages_formatter
-        else:
-            self.messages_formatter = get_predefined_messages_formatter(
-                predefined_messages_formatter_type
-            )
-        self.last_response = ""
-        self.function_tool_registry = function_tool_registry
-
-    @staticmethod
-    def get_function_tool_registry(
-        function_tool_list: List[LlamaCppFunctionTool],
-        allow_parallel_function_calling=False,
-        add_inner_thoughts=False,
-        allow_inner_thoughts_only=False,
-        add_request_heartbeat=False,
-        tool_root="function",
-        tool_rule_content="parameters",
-        model_prefix="function",
-        fields_prefix="parameters",
-        inner_thoughts_field_name="thoughts_and_reasoning",
-        request_heartbeat_field_name="request_heartbeat",
-    ):
-        """
-        Creates and returns a function tool registry from a list of LlamaCppFunctionTool instances.
-
-        Args:
-            function_tool_list (List[LlamaCppFunctionTool]): List of function tools to register.
-            allow_parallel_function_calling: Allow parallel function calling (Default=False)
-            add_inner_thoughts: Add inner thoughts field (Default=False)
-            allow_inner_thoughts_only: Allow inner thoughts only (Default=False)
-            add_request_heartbeat: Add request heartbeat field (Default=False)
-            tool_root: The root name of the tool (Default="function")
-            tool_rule_content: The content of the tool rule (Default="parameters")
-            model_prefix: The prefix for the model in the documentation (Default="function")
-            fields_prefix: The prefix for the fields in the documentation (Default="parameters")
-            inner_thoughts_field_name: The name of the inner thoughts field (Default="thoughts_and_reasoning")
-            request_heartbeat_field_name: The name of the request heartbeat field (Default="request_heartbeat")
-        Returns:
-            LlamaCppFunctionToolRegistry: The created function tool registry.
-        """
-        function_tool_registry = LlamaCppFunctionToolRegistry(
-            allow_parallel_function_calling,
-            add_inner_thoughts,
-            allow_inner_thoughts_only,
-            add_request_heartbeat,
-            tool_root,
-            tool_rule_content,
-            model_prefix,
-            fields_prefix,
-            inner_thoughts_field_name,
-            request_heartbeat_field_name,
-        )
-
-        for function_tool in function_tool_list:
-            function_tool_registry.register_function_tool(function_tool)
-        function_tool_registry.finalize()
-        return function_tool_registry
-
-    def add_message(
-        self,
-        message: str,
-        role: (
-            Literal["system"]
-            | Literal["user"]
-            | Literal["assistant"]
-            | Literal["function"]
-        ) = "user",
-    ):
-        """
-        Adds a message to the chat history.
-
-        Args:
-            message (str): The content of the message.
-            role (Literal["system"] | Literal["user"] | Literal["assistant"]): The role of the message sender.
-        """
-        self.messages.append(
-            {
-                "role": role,
-                "content": message,
-            },
-        )
-
-    def get_text_response(
-        self,
-        prompt: str | list[int] = None,
-        grammar: str = None,
-        function_tool_registry: LlamaCppFunctionToolRegistry = None,
-        do_not_use_grammar: bool = False,
-        streaming_callback: Callable[[StreamingResponse], None] = None,
-        max_tokens: int = 0,
-        temperature: float = 0.4,
-        top_k: int = 0,
-        top_p: float = 1.0,
-        min_p: float = 0.05,
-        typical_p: float = 1.0,
-        repeat_penalty: float = 1.0,
-        mirostat_mode: int = 0,
-        mirostat_tau: float = 5.0,
-        mirostat_eta: float = 0.1,
-        tfs_z: float = 1.0,
-        stop_sequences: List[str] = None,
-        additional_stop_sequences: List[str] = None,
-        stream: bool = True,
-        print_output: bool = False,
-        # Llama Cpp Server and Open AI endpoint settings
-        n_predict: int = -1,
-        n_keep: int = 0,
-        repeat_last_n: int = 64,
-        penalize_nl: bool = True,
-        presence_penalty: float = 0.0,
-        frequency_penalty: float = 0.0,
-        penalty_prompt: Union[None, str, List[int]] = None,
-        seed: int = -1,
-        ignore_eos: bool = False,
-        echo: bool = False,
-        logprobs: int = None,
-        logit_bias: Dict[str, float] = None,
-        logit_bias_type: Literal["input_ids", "tokens"] = None,
-        samplers: List[str] = None,
-    ):
-        """ """
-        if function_tool_registry is None and do_not_use_grammar is False:
-            if self.function_tool_registry is not None:
-                function_tool_registry = self.function_tool_registry
-
-        if function_tool_registry is not None:
-            grammar = function_tool_registry.gbnf_grammar
-
-        if self.debug_output:
-            if type(prompt) is str:
-                print(prompt, end="")
-        if stop_sequences is None:
-            stop_sequences = self.messages_formatter.DEFAULT_STOP_SEQUENCES
-
-        if additional_stop_sequences is not None:
-            stop_sequences.extend(additional_stop_sequences)
-
-        if self.model:
-            completion = self.get_text_completion(
-                grammar=grammar,
-                prompt=prompt,
-                max_tokens=max_tokens,
-                temperature=temperature,
-                top_k=top_k,
-                top_p=top_p,
-                min_p=min_p,
-                typical_p=typical_p,
-                repeat_penalty=repeat_penalty,
-                mirostat_mode=mirostat_mode,
-                mirostat_tau=mirostat_tau,
-                mirostat_eta=mirostat_eta,
-                tfs_z=tfs_z,
-                stop_sequences=stop_sequences,
-                repeat_last_n=repeat_last_n,
-                penalize_nl=penalize_nl,
-                presence_penalty=presence_penalty,
-                frequency_penalty=frequency_penalty,
-                penalty_prompt=penalty_prompt,
-                ignore_eos=ignore_eos,
-                echo=echo,
-                logprobs=logprobs,
-                logit_bias=logit_bias,
-                logit_bias_type=logit_bias_type,
-                samplers=samplers,
-                n_predict=n_predict,
-                n_keep=n_keep,
-                seed=seed,
-            )
-            if stream:
-                full_response = ""
-                for out in completion:
-                    text = out["choices"][0]["text"]
-                    full_response += text
-                    if streaming_callback is not None:
-                        streaming_callback(
-                            StreamingResponse(text=text, is_last_response=False)
-                        )
-                    if print_output:
-                        print(text, end="")
-                if streaming_callback is not None:
-                    streaming_callback(
-                        StreamingResponse(text="", is_last_response=True)
-                    )
-                if print_output:
-                    print("")
-                self.last_response = full_response
-                if function_tool_registry is not None:
-                    full_response = function_tool_registry.handle_function_call(
-                        full_response
-                    )
-                return full_response if full_response else None
-            else:
-                full_response = ""
-                text = completion["choices"][0]["text"]
-                full_response += text
-                if print_output:
-                    print(full_response)
-                self.last_response = full_response
-                if function_tool_registry is not None:
-                    full_response = function_tool_registry.handle_function_call(
-                        full_response
-                    )
-                return full_response if full_response else None
-        return "Error: No model loaded!"
-
-    def get_text_response_generator(
-        self,
-        prompt: str | list[int] = None,
-        grammar: str = None,
-        function_tool_registry: LlamaCppFunctionToolRegistry = None,
-        do_not_use_grammar: bool = False,
-        streaming_callback: Callable[[StreamingResponse], None] = None,
-        max_tokens: int = 0,
-        temperature: float = 0.4,
-        top_k: int = 0,
-        top_p: float = 1.0,
-        min_p: float = 0.05,
-        typical_p: float = 1.0,
-        repeat_penalty: float = 1.0,
-        mirostat_mode: int = 0,
-        mirostat_tau: float = 5.0,
-        mirostat_eta: float = 0.1,
-        tfs_z: float = 1.0,
-        stop_sequences: List[str] = None,
-        print_output: bool = True,
-        # Llama Cpp Server and Open AI endpoint settings
-        n_predict: int = -1,
-        n_keep: int = 0,
-        repeat_last_n: int = 64,
-        penalize_nl: bool = True,
-        presence_penalty: float = 0.0,
-        frequency_penalty: float = 0.0,
-        penalty_prompt: Union[None, str, List[int]] = None,
-        seed: int = -1,
-        ignore_eos: bool = False,
-        echo: bool = False,
-        logprobs: int = None,
-        logit_bias: Dict[str, float] = None,
-        logit_bias_type: Literal["input_ids", "tokens"] = None,
-        samplers: List[str] = None,
-    ):
-        """ """
-        if function_tool_registry is None and do_not_use_grammar is False:
-            if self.function_tool_registry is not None:
-                function_tool_registry = self.function_tool_registry
-
-        if function_tool_registry is not None:
-            grammar = function_tool_registry.gbnf_grammar
-
-        if self.debug_output:
-            if type(prompt) is str:
-                print(prompt, end="")
-        if stop_sequences is None:
-            stop_sequences = []
-
-        if self.model:
-            completion = self.get_text_completion(
-                grammar=grammar,
-                prompt=prompt,
-                max_tokens=max_tokens,
-                temperature=temperature,
-                top_k=top_k,
-                top_p=top_p,
-                min_p=min_p,
-                typical_p=typical_p,
-                repeat_penalty=repeat_penalty,
-                mirostat_mode=mirostat_mode,
-                mirostat_tau=mirostat_tau,
-                mirostat_eta=mirostat_eta,
-                tfs_z=tfs_z,
-                stop_sequences=stop_sequences,
-                repeat_last_n=repeat_last_n,
-                penalize_nl=penalize_nl,
-                presence_penalty=presence_penalty,
-                frequency_penalty=frequency_penalty,
-                penalty_prompt=penalty_prompt,
-                ignore_eos=ignore_eos,
-                echo=echo,
-                logprobs=logprobs,
-                logit_bias=logit_bias,
-                logit_bias_type=logit_bias_type,
-                samplers=samplers,
-                n_predict=n_predict,
-                n_keep=n_keep,
-                seed=seed,
-            )
-            full_response = ""
-            for out in completion:
-                text = out["choices"][0]["text"]
-                full_response += text
-                yield text
-                if streaming_callback is not None:
-                    streaming_callback(
-                        StreamingResponse(text=text, is_last_response=False)
-                    )
-                if print_output:
-                    print(text, end="")
-            if streaming_callback is not None:
-                streaming_callback(StreamingResponse(text="", is_last_response=True))
-            if print_output:
-                print("")
-            self.last_response = full_response
-            if function_tool_registry is not None:
-                full_response = function_tool_registry.handle_function_call(
-                    full_response
-                )
-                yield full_response if full_response else None
-            return
-        return "Error: No model loaded!"
-
-    def get_chat_response(
-        self,
-        message: str = None,
-        role: Literal["system", "user", "assistant", "function"] = "user",
-        response_role: Literal["user", "assistant"] | None = None,
-        system_prompt: str = None,
-        prompt_suffix: str = None,
-        add_message_to_chat_history: bool = True,
-        add_response_to_chat_history: bool = True,
-        grammar: str = None,
-        function_tool_registry: LlamaCppFunctionToolRegistry = None,
-        do_not_use_grammar: bool = False,
-        streaming_callback: Callable[[StreamingResponse], None] = None,
-        max_tokens: int = 0,
-        temperature: float = 0.4,
-        top_k: int = 0,
-        top_p: float = 1.0,
-        min_p: float = 0.05,
-        typical_p: float = 1.0,
-        repeat_penalty: float = 1.0,
-        mirostat_mode: int = 0,
-        mirostat_tau: float = 5.0,
-        mirostat_eta: float = 0.1,
-        tfs_z: float = 1.0,
-        stop_sequences: List[str] = None,
-        additional_stop_sequences: List[str] = None,
-        stream: bool = True,
-        print_output: bool = True,
-        k_last_messages: int = 0,
-        # Llama Cpp Server and Open AI endpoint settings
-        n_predict: int = -1,
-        n_keep: int = 0,
-        repeat_last_n: int = 64,
-        penalize_nl: bool = True,
-        presence_penalty: float = 0.0,
-        frequency_penalty: float = 0.0,
-        penalty_prompt: Union[None, str, List[int]] = None,
-        seed: int = -1,
-        ignore_eos: bool = False,
-        echo: bool = False,
-        logprobs: int = None,
-        logit_bias: Dict[str, float] = None,
-        logit_bias_type: Literal["input_ids", "tokens"] = None,
-        cache_prompt: bool = False,
-        samplers: List[str] = None,
-    ):
-        """
-        Gets a chat response based on the input message and context.
-
-        Args:
-            message (str): The input message.
-            role (Literal["system", "user", "assistant", "function"]): The role of the message sender.
-            response_role (Literal["user", "assistant"]): The role of the message response.
-            system_prompt (str): The system prompt used in chat interactions.
-            prompt_suffix: Suffix to append after the prompt.
-            add_message_to_chat_history (bool): Indicates whether to add the input message to the chat history.
-            add_response_to_chat_history (bool): Indicates whether to add the generated response to the chat history.
-            grammar (str): The grammar for generating responses in string format.
-            function_tool_registry (LlamaCppFunctionToolRegistry): The function tool registry for handling function calls.
-            do_not_use_grammar (bool): Indicates whether to use grammar when generating responses.
-            streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
-
-            max_tokens (int): The maximum number of tokens in the generated response.
-            temperature (float): The temperature parameter for response generation.
-            top_k (int): Top-k parameter for response generation.
-            top_p (float): Top-p parameter for response generation.
-            min_p (float): Minimum probability parameter for response generation.
-            typical_p (float): Typical probability parameter for response generation.
-            repeat_penalty (float): Penalty for repeating tokens in response generation.
-            mirostat_mode (int): Mirostat mode for response generation.
-            mirostat_tau (float): Mirostat tau parameter for response generation.
-            mirostat_eta (float): Mirostat eta parameter for response generation.
-            tfs_z (float): TFS Z parameter for response generation.
-            stop_sequences (List[str]): List of stop sequences for response generation. Overwrites default stop sequences!
-            additional_stop_sequences (List[str]): List of stop sequences for response generation, additional to the default ones.
-            stream (bool): Indicates whether to stream the response.
-            print_output (bool): Indicates whether to print the generated response.
-            k_last_messages (int): Number of last messages to consider from the chat history.
-
-
-            Additional parameters for llama.cpp server backends and OpenAI endpoints
-            n_predict (int): Number of predictions to generate for each completion.
-            n_keep (int): Number of completions to keep.
-            repeat_last_n (int): Number of tokens to consider for repeat penalty.
-            penalize_nl (bool): Indicates whether to penalize newline characters in response generation.
-            presence_penalty (float): Presence penalty parameter for response generation.
-            frequency_penalty (float): Frequency penalty parameter for response generation.
-            penalty_prompt (Union[None, str, List[int]]): Penalty prompt for response generation.
-            seed (int): Seed for random number generation.
-            ignore_eos (bool): Indicates whether to ignore end-of-sequence tokens.
-            echo: bool = False,
-            logprobs: int = None,
-            logit_bias: Dict[str, float] = None,
-            logit_bias_type:Literal["input_ids", "tokens"] = None
-            cache_prompt: bool = False,
-            samplers: List[str] = None
-        Returns:
-            list[dict]|str: The generated chat response.
-        """
-        if function_tool_registry is None and do_not_use_grammar is False:
-            if self.function_tool_registry is not None:
-                function_tool_registry = self.function_tool_registry
-        completion, response_role = self.get_response_role_and_completion(
-            function_tool_registry=function_tool_registry,
-            system_prompt=system_prompt,
-            message=message,
-            add_message_to_chat_history=add_message_to_chat_history,
-            role=role,
-            response_role=response_role,
-            grammar=grammar,
-            prompt_suffix=prompt_suffix,
-            max_tokens=max_tokens,
-            temperature=temperature,
-            top_k=top_k,
-            top_p=top_p,
-            min_p=min_p,
-            typical_p=typical_p,
-            repeat_penalty=repeat_penalty,
-            mirostat_mode=mirostat_mode,
-            mirostat_tau=mirostat_tau,
-            mirostat_eta=mirostat_eta,
-            tfs_z=tfs_z,
-            stop_sequences=stop_sequences,
-            additional_stop_sequences=additional_stop_sequences,
-            stream=stream,
-            k_last_messages=k_last_messages,
-            n_predict=n_predict,
-            n_keep=n_keep,
-            repeat_last_n=repeat_last_n,
-            penalize_nl=penalize_nl,
-            presence_penalty=presence_penalty,
-            frequency_penalty=frequency_penalty,
-            penalty_prompt=penalty_prompt,
-            seed=seed,
-            ignore_eos=ignore_eos,
-            echo=echo,
-            logprobs=logprobs,
-            logit_bias=logit_bias,
-            logit_bias_type=logit_bias_type,
-            cache_prompt=cache_prompt,
-            samplers=samplers,
-        )
-        if self.model:
-            if stream:
-                full_response = ""
-                for out in completion:
-                    text = out["choices"][0]["text"]
-                    full_response += text
-                    if streaming_callback is not None:
-                        streaming_callback(
-                            StreamingResponse(text=text, is_last_response=False)
-                        )
-                    if print_output:
-                        print(text, end="")
-                if streaming_callback is not None:
-                    streaming_callback(
-                        StreamingResponse(text="", is_last_response=True)
-                    )
-                if print_output:
-                    print("")
-
-                self.last_response = full_response
-                if add_response_to_chat_history:
-                    self.messages.append(
-                        {
-                            "role": response_role,
-                            "content": full_response,
-                        },
-                    )
-                if function_tool_registry is not None:
-                    full_response = function_tool_registry.handle_function_call(
-                        full_response
-                    )
-                return full_response if full_response else None
-            else:
-                text = completion["choices"][0]["text"]
-                if print_output:
-                    print(text)
-                self.last_response = text
-                if add_response_to_chat_history:
-                    self.messages.append(
-                        {
-                            "role": response_role,
-                            "content": text,
-                        },
-                    )
-                if function_tool_registry is not None:
-                    text = function_tool_registry.handle_function_call(text)
-                return text if text else None
-        return "Error: No model loaded!"
-
-    def get_chat_response_generator(
-        self,
-        message: str = None,
-        role: Literal["system", "user", "assistant", "function"] = "user",
-        response_role: Literal["user", "assistant"] | None = None,
-        system_prompt: str = None,
-        prompt_suffix: str = None,
-        add_message_to_chat_history: bool = True,
-        add_response_to_chat_history: bool = True,
-        grammar: str = None,
-        function_tool_registry: LlamaCppFunctionToolRegistry = None,
-        do_not_use_grammar: bool = False,
-        streaming_callback: Callable[[StreamingResponse], None] = None,
-        max_tokens: int = 0,
-        temperature: float = 0.4,
-        top_k: int = 0,
-        top_p: float = 1.0,
-        min_p: float = 0.05,
-        typical_p: float = 1.0,
-        repeat_penalty: float = 1.0,
-        mirostat_mode: int = 0,
-        mirostat_tau: float = 5.0,
-        mirostat_eta: float = 0.1,
-        tfs_z: float = 1.0,
-        stop_sequences: List[str] = None,
-        additional_stop_sequences: List[str] = None,
-        print_output: bool = True,
-        k_last_messages: int = 0,
-        # Llama Cpp Server and Open AI endpoint settings
-        n_predict: int = -1,
-        n_keep: int = 0,
-        repeat_last_n: int = 64,
-        penalize_nl: bool = True,
-        presence_penalty: float = 0.0,
-        frequency_penalty: float = 0.0,
-        penalty_prompt: Union[None, str, List[int]] = None,
-        seed: int = -1,
-        ignore_eos: bool = False,
-        echo: bool = False,
-        logprobs: int = None,
-        logit_bias: Dict[str, float] = None,
-        logit_bias_type: Literal["input_ids", "tokens"] = None,
-        cache_prompt: bool = False,
-        samplers: List[str] = None,
-    ):
-        """
-        Gets a chat response based on the input message and context.
-
-        Args:
-            message (str): The input message.
-            role (Literal["system", "user", "assistant", "function"]): The role of the message sender.
-            response_role (Literal["user", "assistant"]): The role of the message response.
-            system_prompt (str): The system prompt used in chat interactions.
-            prompt_suffix: Suffix to append after the prompt.
-            add_message_to_chat_history (bool): Indicates whether to add the input message to the chat history.
-            add_response_to_chat_history (bool): Indicates whether to add the generated response to the chat history.
-            grammar (str): The grammar for generating responses in string format.
-            function_tool_registry (LlamaCppFunctionToolRegistry): The function tool registry for handling function calls.
-            do_not_use_grammar (bool): Indicates whether to use grammar when generating responses.
-            streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
-            max_tokens (int): The maximum number of tokens in the generated response.
-            temperature (float): The temperature parameter for response generation.
-            top_k (int): Top-k parameter for response generation.
-            top_p (float): Top-p parameter for response generation.
-            min_p (float): Minimum probability parameter for response generation.
-            typical_p (float): Typical probability parameter for response generation.
-            repeat_penalty (float): Penalty for repeating tokens in response generation.
-            mirostat_mode (int): Mirostat mode for response generation.
-            mirostat_tau (float): Mirostat tau parameter for response generation.
-            mirostat_eta (float): Mirostat eta parameter for response generation.
-            tfs_z (float): TFS Z parameter for response generation.
-            stop_sequences (List[str]): List of stop sequences for response generation. Overwrites default stop sequences!
-            additional_stop_sequences (List[str]): List of stop sequences for response generation, additional to the default ones.
-            print_output (bool): Indicates whether to print the generated response.
-            k_last_messages (int): Number of last messages to consider from the chat history.
-
-
-            Additional parameters for llama.cpp server backends and OpenAI endpoints
-            n_predict (int): Number of predictions to generate for each completion.
-            n_keep (int): Number of completions to keep.
-            repeat_last_n (int): Number of tokens to consider for repeat penalty.
-            penalize_nl (bool): Indicates whether to penalize newline characters in response generation.
-            presence_penalty (float): Presence penalty parameter for response generation.
-            frequency_penalty (float): Frequency penalty parameter for response generation.
-            penalty_prompt (Union[None, str, List[int]]): Penalty prompt for response generation.
-            seed (int): Seed for random number generation.
-            ignore_eos (bool): Indicates whether to ignore end-of-sequence tokens.
-            echo: bool = False,
-            logprobs: int = None,
-            logit_bias: Dict[str, float] = None,
-            logit_bias_type:Literal["input_ids", "tokens"] = None
-            cache_prompt: bool = False,
-            samplers: List[str] = None
-        Returns:
-            list[dict]: The generated chat response.
-        """
-        if function_tool_registry is None and do_not_use_grammar is False:
-            if self.function_tool_registry is not None:
-                function_tool_registry = self.function_tool_registry
-
-        completion, response_role = self.get_response_role_and_completion(
-            function_tool_registry=function_tool_registry,
-            system_prompt=system_prompt,
-            message=message,
-            add_message_to_chat_history=add_message_to_chat_history,
-            role=role,
-            response_role=response_role,
-            grammar=grammar,
-            prompt_suffix=prompt_suffix,
-            max_tokens=max_tokens,
-            temperature=temperature,
-            top_k=top_k,
-            top_p=top_p,
-            min_p=min_p,
-            typical_p=typical_p,
-            repeat_penalty=repeat_penalty,
-            mirostat_mode=mirostat_mode,
-            mirostat_tau=mirostat_tau,
-            mirostat_eta=mirostat_eta,
-            tfs_z=tfs_z,
-            stop_sequences=stop_sequences,
-            additional_stop_sequences=additional_stop_sequences,
-            stream=True,
-            k_last_messages=k_last_messages,
-            n_predict=n_predict,
-            n_keep=n_keep,
-            repeat_last_n=repeat_last_n,
-            penalize_nl=penalize_nl,
-            presence_penalty=presence_penalty,
-            frequency_penalty=frequency_penalty,
-            penalty_prompt=penalty_prompt,
-            seed=seed,
-            ignore_eos=ignore_eos,
-            echo=echo,
-            logprobs=logprobs,
-            logit_bias=logit_bias,
-            logit_bias_type=logit_bias_type,
-            cache_prompt=cache_prompt,
-            samplers=samplers,
-        )
-        if self.model:
-            full_response = ""
-            for out in completion:
-                text = out["choices"][0]["text"]
-                full_response += text
-                yield text
-                if streaming_callback is not None:
-                    streaming_callback(
-                        StreamingResponse(text=text, is_last_response=False)
-                    )
-                if print_output:
-                    print(text, end="")
-            if streaming_callback is not None:
-                streaming_callback(StreamingResponse(text="", is_last_response=True))
-            if print_output:
-                print("")
-
-            self.last_response = full_response
-            if add_response_to_chat_history:
-                self.messages.append(
-                    {
-                        "role": response_role,
-                        "content": full_response,
-                    },
-                )
-            if function_tool_registry is not None:
-                full_response = function_tool_registry.handle_function_call(
-                    full_response
-                )
-                yield full_response if full_response else None
-            return
-        return "Error: No model loaded!"
-
-    def get_text_completion(
-        self,
-        prompt: str | list[int] = None,
-        grammar: str = None,
-        max_tokens: int = 0,
-        temperature: float = 0.4,
-        top_k: int = 0,
-        top_p: float = 1.0,
-        min_p: float = 0.05,
-        typical_p: float = 1.0,
-        repeat_penalty: float = 1.0,
-        mirostat_mode: int = 0,
-        mirostat_tau: float = 5.0,
-        mirostat_eta: float = 0.1,
-        tfs_z: float = 1.0,
-        # Llama Cpp Server and Open AI endpoint settings
-        n_predict: int = -1,
-        n_keep: int = 0,
-        repeat_last_n: int = 64,
-        penalize_nl: bool = True,
-        presence_penalty: float = 0.0,
-        frequency_penalty: float = 0.0,
-        penalty_prompt: Union[None, str, List[int]] = None,
-        seed: int = -1,
-        ignore_eos: bool = False,
-        echo: bool = False,
-        logprobs: int = None,
-        logit_bias: Dict[str, float] = None,
-        logit_bias_type: Literal["input_ids", "tokens"] = None,
-        samplers: List[str] = None,
-        stop_sequences: List[str] = None,
-    ):
-        if isinstance(self.model, LlamaCppEndpointSettings):
-            completion = self.model.create_completion(
-                prompt=prompt,
-                grammar=grammar,
-                generation_settings=LlamaCppGenerationSettings(
-                    temperature=temperature,
-                    top_k=top_k,
-                    top_p=top_p,
-                    min_p=min_p,
-                    n_predict=n_predict,
-                    n_keep=n_keep,
-                    stream=True,
-                    stop_sequences=stop_sequences,
-                    tfs_z=tfs_z,
-                    typical_p=typical_p,
-                    repeat_penalty=repeat_penalty,
-                    repeat_last_n=repeat_last_n,
-                    penalize_nl=penalize_nl,
-                    presence_penalty=presence_penalty,
-                    frequency_penalty=frequency_penalty,
-                    penalty_prompt=penalty_prompt,
-                    mirostat_mode=mirostat_mode,
-                    mirostat_tau=mirostat_tau,
-                    mirostat_eta=mirostat_eta,
-                    seed=seed,
-                    samplers=samplers,
-                    ignore_eos=ignore_eos,
-                ),
-            )
-        elif isinstance(self.model, OpenAIEndpointSettings):
-            completion = self.model.create_completion(
-                prompt=prompt,
-                grammar=grammar,
-                generation_settings=OpenAIGenerationSettings(
-                    temperature=temperature,
-                    top_k=top_k,
-                    top_p=top_p,
-                    min_p=min_p,
-                    stream=True,
-                    stop_sequences=stop_sequences,
-                    echo=echo,
-                    repeat_penalty=repeat_penalty,
-                    logprobs=logprobs,
-                    presence_penalty=presence_penalty,
-                    frequency_penalty=frequency_penalty,
-                    logit_bias=logit_bias,
-                    logit_bias_type=logit_bias_type,
-                    mirostat_mode=mirostat_mode,
-                    mirostat_tau=mirostat_tau,
-                    mirostat_eta=mirostat_eta,
-                    seed=seed,
-                ),
-            )
-        else:
-            if isinstance(grammar, str):
-                if grammar in self.grammar_cache:
-                    grammar = self.grammar_cache[grammar]
-                else:
-                    grammar_string = grammar
-                    grammar = LlamaGrammar.from_string(grammar, False)
-                    self.grammar_cache[grammar_string] = grammar
-            completion = self.model.create_completion(
-                prompt=prompt,
-                max_tokens=max_tokens,
-                stream=True,
-                stop=stop_sequences,
-                temperature=temperature,
-                top_k=top_k,
-                top_p=top_p,
-                min_p=min_p,
-                typical_p=typical_p,
-                mirostat_mode=mirostat_mode,
-                mirostat_tau=mirostat_tau,
-                mirostat_eta=mirostat_eta,
-                tfs_z=tfs_z,
-                repeat_penalty=repeat_penalty,
-                grammar=grammar,
-            )
-        return completion
-
-    def get_response_role_and_completion(
-        self,
-        function_tool_registry: LlamaCppFunctionToolRegistry = None,
-        system_prompt: str = None,
-        message: str = None,
-        add_message_to_chat_history: bool = True,
-        role: Literal["system", "user", "assistant", "function"] = "user",
-        response_role: Literal["user", "assistant"] | None = None,
-        grammar: str = None,
-        prompt_suffix: str = None,
-        max_tokens: int = 0,
-        temperature: float = 0.4,
-        top_k: int = 0,
-        top_p: float = 1.0,
-        min_p: float = 0.05,
-        typical_p: float = 1.0,
-        repeat_penalty: float = 1.0,
-        mirostat_mode: int = 0,
-        mirostat_tau: float = 5.0,
-        mirostat_eta: float = 0.1,
-        tfs_z: float = 1.0,
-        stop_sequences: List[str] = None,
-        additional_stop_sequences: List[str] = None,
-        stream: bool = True,
-        k_last_messages: int = 0,
-        n_predict: int = -1,
-        n_keep: int = 0,
-        repeat_last_n: int = 64,
-        penalize_nl: bool = True,
-        presence_penalty: float = 0.0,
-        frequency_penalty: float = 0.0,
-        penalty_prompt: Union[None, str, List[int]] = None,
-        seed: int = -1,
-        ignore_eos: bool = False,
-        echo: bool = False,
-        logprobs: int = None,
-        logit_bias: Dict[str, float] = None,
-        logit_bias_type: Literal["input_ids", "tokens"] = None,
-        cache_prompt: bool = False,
-        samplers: List[str] = None,
-    ):
-        if function_tool_registry is not None:
-            grammar = function_tool_registry.gbnf_grammar
-
-        if system_prompt is None:
-            system_prompt = self.system_prompt
-        messages = [
-            {
-                "role": "system",
-                "content": system_prompt,
-            },
-        ]
-        if message is not None and add_message_to_chat_history:
-            self.messages.append(
-                {
-                    "role": role,
-                    "content": message,
-                },
-            )
-        if not add_message_to_chat_history and message is not None:
-            messages.append(
-                {
-                    "role": role,
-                    "content": message,
-                },
-            )
-        if k_last_messages > 0:
-            messages.extend(self.messages[-k_last_messages:])
-        else:
-            messages.extend(self.messages)
-
-        prompt, response_role = self.messages_formatter.format_messages(
-            messages, response_role
-        )
-
-        if prompt_suffix:
-            prompt += prompt_suffix
-
-        if self.debug_output:
-            print(prompt, end="")
-
-        if stop_sequences is None:
-            stop_sequences = self.messages_formatter.DEFAULT_STOP_SEQUENCES
-
-        if additional_stop_sequences is not None:
-            stop_sequences.extend(additional_stop_sequences)
-
-        if self.model:
-            if isinstance(self.model, LlamaCppEndpointSettings):
-                completion = self.model.create_completion(
-                    prompt=prompt,
-                    grammar=grammar,
-                    generation_settings=LlamaCppGenerationSettings(
-                        temperature=temperature,
-                        top_k=top_k,
-                        top_p=top_p,
-                        min_p=min_p,
-                        n_predict=n_predict,
-                        n_keep=n_keep,
-                        stream=stream,
-                        stop_sequences=stop_sequences,
-                        tfs_z=tfs_z,
-                        typical_p=typical_p,
-                        repeat_penalty=repeat_penalty,
-                        repeat_last_n=repeat_last_n,
-                        penalize_nl=penalize_nl,
-                        presence_penalty=presence_penalty,
-                        frequency_penalty=frequency_penalty,
-                        penalty_prompt=penalty_prompt,
-                        mirostat_mode=mirostat_mode,
-                        mirostat_tau=mirostat_tau,
-                        mirostat_eta=mirostat_eta,
-                        samplers=samplers,
-                        seed=seed,
-                        cache_prompt=cache_prompt,
-                        ignore_eos=ignore_eos,
-                    ),
-                )
-            elif isinstance(self.model, OpenAIEndpointSettings):
-                completion = self.model.create_completion(
-                    prompt=prompt,
-                    grammar=grammar,
-                    generation_settings=OpenAIGenerationSettings(
-                        temperature=temperature,
-                        top_k=top_k,
-                        top_p=top_p,
-                        min_p=min_p,
-                        stream=stream,
-                        stop_sequences=stop_sequences,
-                        echo=echo,
-                        repeat_penalty=repeat_penalty,
-                        logprobs=logprobs,
-                        presence_penalty=presence_penalty,
-                        frequency_penalty=frequency_penalty,
-                        logit_bias=logit_bias,
-                        logit_bias_type=logit_bias_type,
-                        mirostat_mode=mirostat_mode,
-                        mirostat_tau=mirostat_tau,
-                        mirostat_eta=mirostat_eta,
-                        seed=seed,
-                    ),
-                )
-            else:
-                if isinstance(grammar, str):
-                    if grammar in self.grammar_cache:
-                        grammar = self.grammar_cache[grammar]
-                    else:
-                        grammar_string = grammar
-                        grammar = LlamaGrammar.from_string(grammar, False)
-                        self.grammar_cache[grammar_string] = grammar
-                completion = self.model.create_completion(
-                    prompt=prompt,
-                    max_tokens=max_tokens,
-                    stream=stream,
-                    stop=stop_sequences,
-                    temperature=temperature,
-                    top_k=top_k,
-                    top_p=top_p,
-                    min_p=min_p,
-                    typical_p=typical_p,
-                    mirostat_mode=mirostat_mode,
-                    mirostat_tau=mirostat_tau,
-                    mirostat_eta=mirostat_eta,
-                    tfs_z=tfs_z,
-                    repeat_penalty=repeat_penalty,
-                    grammar=grammar,
-                )
-            return completion, response_role
-        return "Error: No model loaded!"
-
-    async def async_get_text_response(
-        self,
-        prompt: str | list[int] = None,
-        grammar: str = None,
-        function_tool_registry: LlamaCppFunctionToolRegistry = None,
-        do_not_use_grammar: bool = False,
-        streaming_callback: Callable[[StreamingResponse], None] = None,
-        max_tokens: int = 0,
-        temperature: float = 0.4,
-        top_k: int = 0,
-        top_p: float = 1.0,
-        min_p: float = 0.05,
-        typical_p: float = 1.0,
-        repeat_penalty: float = 1.0,
-        mirostat_mode: int = 0,
-        mirostat_tau: float = 5.0,
-        mirostat_eta: float = 0.1,
-        tfs_z: float = 1.0,
-        stop_sequences: List[str] = None,
-        additional_stop_sequences: List[str] = None,
-        stream: bool = True,
-        print_output: bool = True,
-        # Llama Cpp Server and Open AI endpoint settings
-        n_predict: int = -1,
-        n_keep: int = 0,
-        repeat_last_n: int = 64,
-        penalize_nl: bool = True,
-        presence_penalty: float = 0.0,
-        frequency_penalty: float = 0.0,
-        penalty_prompt: Union[None, str, List[int]] = None,
-        seed: int = -1,
-        ignore_eos: bool = False,
-        echo: bool = False,
-        logprobs: int = None,
-        logit_bias: Dict[str, float] = None,
-        logit_bias_type: Literal["input_ids", "tokens"] = None,
-        samplers: List[str] = None,
-    ):
-        """ """
-        if function_tool_registry is None and do_not_use_grammar is False:
-            if self.function_tool_registry is not None:
-                function_tool_registry = self.function_tool_registry
-
-        if function_tool_registry is not None:
-            grammar = function_tool_registry.gbnf_grammar
-
-        if self.debug_output:
-            if type(prompt) is str:
-                print(prompt, end="")
-        if stop_sequences is None:
-            stop_sequences = self.messages_formatter.DEFAULT_STOP_SEQUENCES
-
-        if additional_stop_sequences is not None:
-            stop_sequences.extend(additional_stop_sequences)
-
-        if self.model:
-            completion = await self.async_get_text_completion(
-                grammar=grammar,
-                prompt=prompt,
-                max_tokens=max_tokens,
-                temperature=temperature,
-                top_k=top_k,
-                top_p=top_p,
-                min_p=min_p,
-                typical_p=typical_p,
-                repeat_penalty=repeat_penalty,
-                mirostat_mode=mirostat_mode,
-                mirostat_tau=mirostat_tau,
-                mirostat_eta=mirostat_eta,
-                tfs_z=tfs_z,
-                stop_sequences=stop_sequences,
-                repeat_last_n=repeat_last_n,
-                penalize_nl=penalize_nl,
-                presence_penalty=presence_penalty,
-                frequency_penalty=frequency_penalty,
-                penalty_prompt=penalty_prompt,
-                ignore_eos=ignore_eos,
-                echo=echo,
-                logprobs=logprobs,
-                logit_bias=logit_bias,
-                logit_bias_type=logit_bias_type,
-                samplers=samplers,
-                n_predict=n_predict,
-                n_keep=n_keep,
-                seed=seed,
-                stream=stream,
-            )
-            if stream:
-                full_response = ""
-                async for out in completion:
-                    text = out["choices"][0]["text"]
-                    full_response += text
-                    if streaming_callback is not None:
-                        streaming_callback(
-                            StreamingResponse(text=text, is_last_response=False)
-                        )
-                    if print_output:
-                        print(text, end="")
-                if streaming_callback is not None:
-                    streaming_callback(
-                        StreamingResponse(text="", is_last_response=True)
-                    )
-                if print_output:
-                    print("")
-                self.last_response = full_response
-                if function_tool_registry is not None:
-                    full_response = function_tool_registry.handle_function_call(
-                        full_response
-                    )
-                    return full_response if full_response else None
-                return full_response if full_response else None
-            else:
-                text = completion["choices"][0]["text"]
-                self.last_response = text
-                if print_output:
-                    print(text)
-                if function_tool_registry is not None:
-                    text = function_tool_registry.handle_function_call(text)
-                    return text if text else None
-                return text if text else None
-        return "Error: No model loaded!"
-
-    async def async_get_chat_response(
-        self,
-        message: str = None,
-        role: Literal["system", "user", "assistant", "function"] = "user",
-        response_role: Literal["user", "assistant"] | None = None,
-        system_prompt: str = None,
-        prompt_suffix: str = None,
-        add_message_to_chat_history: bool = True,
-        add_response_to_chat_history: bool = True,
-        grammar: str = None,
-        function_tool_registry: LlamaCppFunctionToolRegistry = None,
-        do_not_use_grammar: bool = False,
-        streaming_callback: Callable[[StreamingResponse], None] = None,
-        max_tokens: int = 0,
-        temperature: float = 0.4,
-        top_k: int = 0,
-        top_p: float = 1.0,
-        min_p: float = 0.05,
-        typical_p: float = 1.0,
-        repeat_penalty: float = 1.0,
-        mirostat_mode: int = 0,
-        mirostat_tau: float = 5.0,
-        mirostat_eta: float = 0.1,
-        tfs_z: float = 1.0,
-        stop_sequences: List[str] = None,
-        additional_stop_sequences: List[str] = None,
-        stream: bool = False,
-        print_output: bool = True,
-        k_last_messages: int = 0,
-        # Llama Cpp Server and Open AI endpoint settings
-        n_predict: int = -1,
-        n_keep: int = 0,
-        repeat_last_n: int = 64,
-        penalize_nl: bool = True,
-        presence_penalty: float = 0.0,
-        frequency_penalty: float = 0.0,
-        penalty_prompt: Union[None, str, List[int]] = None,
-        seed: int = -1,
-        ignore_eos: bool = False,
-        echo: bool = False,
-        logprobs: int = None,
-        logit_bias: Dict[str, float] = None,
-        logit_bias_type: Literal["input_ids", "tokens"] = None,
-        cache_prompt: bool = False,
-        samplers: List[str] = None,
-    ):
-        """
-        Gets a chat response based on the input message and context.
-
-        Args:
-            message (str): The input message.
-            role (Literal["system", "user", "assistant", "function"]): The role of the message sender.
-            response_role (Literal["user", "assistant"]): The role of the message response.
-            system_prompt (str): The system prompt used in chat interactions.
-            prompt_suffix: Suffix to append after the prompt.
-            add_message_to_chat_history (bool): Indicates whether to add the input message to the chat history.
-            add_response_to_chat_history (bool): Indicates whether to add the generated response to the chat history.
-            grammar (str): The grammar for generating responses in string format.
-            function_tool_registry (LlamaCppFunctionToolRegistry): The function tool registry for handling function calls.
-            do_not_use_grammar (bool): Indicates whether to use grammar when generating responses.
-            streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
-
-            max_tokens (int): The maximum number of tokens in the generated response.
-            temperature (float): The temperature parameter for response generation.
-            top_k (int): Top-k parameter for response generation.
-            top_p (float): Top-p parameter for response generation.
-            min_p (float): Minimum probability parameter for response generation.
-            typical_p (float): Typical probability parameter for response generation.
-            repeat_penalty (float): Penalty for repeating tokens in response generation.
-            mirostat_mode (int): Mirostat mode for response generation.
-            mirostat_tau (float): Mirostat tau parameter for response generation.
-            mirostat_eta (float): Mirostat eta parameter for response generation.
-            tfs_z (float): TFS Z parameter for response generation.
-            stop_sequences (List[str]): List of stop sequences for response generation. Overwrites default stop sequences!
-            additional_stop_sequences (List[str]): List of stop sequences for response generation, additional to the default ones.
-            stream (bool): Indicates whether to stream the response.
-            print_output (bool): Indicates whether to print the generated response.
-            k_last_messages (int): Number of last messages to consider from the chat history.
-
-
-            Additional parameters for llama.cpp server backends and OpenAI endpoints
-            n_predict (int): Number of predictions to generate for each completion.
-            n_keep (int): Number of completions to keep.
-            repeat_last_n (int): Number of tokens to consider for repeat penalty.
-            penalize_nl (bool): Indicates whether to penalize newline characters in response generation.
-            presence_penalty (float): Presence penalty parameter for response generation.
-            frequency_penalty (float): Frequency penalty parameter for response generation.
-            penalty_prompt (Union[None, str, List[int]]): Penalty prompt for response generation.
-            seed (int): Seed for random number generation.
-            ignore_eos (bool): Indicates whether to ignore end-of-sequence tokens.
-            echo: bool = False,
-            logprobs: int = None,
-            logit_bias: Dict[str, float] = None,
-            logit_bias_type:Literal["input_ids", "tokens"] = None
-            cache_prompt: bool = False,
-            samplers: List[str] = None
-        Returns:
-            list[dict]|str: The generated chat response.
-        """
-        if function_tool_registry is None and do_not_use_grammar is False:
-            if self.function_tool_registry is not None:
-                function_tool_registry = self.function_tool_registry
-        completion, response_role = await self.async_get_response_role_and_completion(
-            function_tool_registry=function_tool_registry,
-            system_prompt=system_prompt,
-            message=message,
-            add_message_to_chat_history=add_message_to_chat_history,
-            role=role,
-            response_role=response_role,
-            grammar=grammar,
-            prompt_suffix=prompt_suffix,
-            max_tokens=max_tokens,
-            temperature=temperature,
-            top_k=top_k,
-            top_p=top_p,
-            min_p=min_p,
-            typical_p=typical_p,
-            repeat_penalty=repeat_penalty,
-            mirostat_mode=mirostat_mode,
-            mirostat_tau=mirostat_tau,
-            mirostat_eta=mirostat_eta,
-            tfs_z=tfs_z,
-            stop_sequences=stop_sequences,
-            additional_stop_sequences=additional_stop_sequences,
-            stream=stream,
-            k_last_messages=k_last_messages,
-            n_predict=n_predict,
-            n_keep=n_keep,
-            repeat_last_n=repeat_last_n,
-            penalize_nl=penalize_nl,
-            presence_penalty=presence_penalty,
-            frequency_penalty=frequency_penalty,
-            penalty_prompt=penalty_prompt,
-            seed=seed,
-            ignore_eos=ignore_eos,
-            echo=echo,
-            logprobs=logprobs,
-            logit_bias=logit_bias,
-            logit_bias_type=logit_bias_type,
-            cache_prompt=cache_prompt,
-            samplers=samplers,
-        )
-        if self.model:
-            if stream:
-                full_response = ""
-                async for out in completion:
-                    text = out["choices"][0]["text"]
-                    full_response += text
-                    if streaming_callback is not None:
-                        streaming_callback(
-                            StreamingResponse(text=text, is_last_response=False)
-                        )
-                    if print_output:
-                        print(text, end="")
-                if streaming_callback is not None:
-                    streaming_callback(
-                        StreamingResponse(text="", is_last_response=True)
-                    )
-                if print_output:
-                    print("")
-
-                self.last_response = full_response
-                if add_response_to_chat_history:
-                    self.messages.append(
-                        {
-                            "role": response_role,
-                            "content": full_response,
-                        },
-                    )
-                if function_tool_registry is not None:
-                    full_response = function_tool_registry.handle_function_call(
-                        full_response
-                    )
-                    return full_response if full_response else None
-                return full_response if full_response else None
-            else:
-                text = completion["choices"][0]["text"]
-                if print_output:
-                    print(text)
-                self.last_response = text
-                if add_response_to_chat_history:
-                    self.messages.append(
-                        {
-                            "role": response_role,
-                            "content": text,
-                        },
-                    )
-                if function_tool_registry is not None:
-                    text = function_tool_registry.handle_function_call(text)
-                    return text if text else None
-                return text if text else None
-        return "Error: No model loaded!"
-
-    async def async_get_text_completion(
-        self,
-        prompt: str | list[int] = None,
-        grammar: str = None,
-        max_tokens: int = 0,
-        temperature: float = 0.4,
-        top_k: int = 0,
-        top_p: float = 1.0,
-        min_p: float = 0.05,
-        typical_p: float = 1.0,
-        repeat_penalty: float = 1.0,
-        mirostat_mode: int = 0,
-        mirostat_tau: float = 5.0,
-        mirostat_eta: float = 0.1,
-        tfs_z: float = 1.0,
-        stream: bool = False,
-        # Llama Cpp Server and Open AI endpoint settings
-        n_predict: int = -1,
-        n_keep: int = 0,
-        repeat_last_n: int = 64,
-        penalize_nl: bool = True,
-        presence_penalty: float = 0.0,
-        frequency_penalty: float = 0.0,
-        penalty_prompt: Union[None, str, List[int]] = None,
-        seed: int = -1,
-        ignore_eos: bool = False,
-        echo: bool = False,
-        logprobs: int = None,
-        logit_bias: Dict[str, float] = None,
-        logit_bias_type: Literal["input_ids", "tokens"] = None,
-        samplers: List[str] = None,
-        stop_sequences: List[str] = None,
-    ):
-        if isinstance(self.model, LlamaCppEndpointSettings):
-            completion = await self.model.async_create_completion(
-                prompt=prompt,
-                grammar=grammar,
-                generation_settings=LlamaCppGenerationSettings(
-                    temperature=temperature,
-                    top_k=top_k,
-                    top_p=top_p,
-                    min_p=min_p,
-                    n_predict=n_predict,
-                    n_keep=n_keep,
-                    stream=stream,
-                    stop_sequences=stop_sequences,
-                    tfs_z=tfs_z,
-                    typical_p=typical_p,
-                    repeat_penalty=repeat_penalty,
-                    repeat_last_n=repeat_last_n,
-                    penalize_nl=penalize_nl,
-                    presence_penalty=presence_penalty,
-                    frequency_penalty=frequency_penalty,
-                    penalty_prompt=penalty_prompt,
-                    mirostat_mode=mirostat_mode,
-                    mirostat_tau=mirostat_tau,
-                    mirostat_eta=mirostat_eta,
-                    seed=seed,
-                    samplers=samplers,
-                    ignore_eos=ignore_eos,
-                ),
-            )
-        elif isinstance(self.model, OpenAIEndpointSettings):
-            completion = await self.model.async_create_completion(
-                prompt=prompt,
-                grammar=grammar,
-                generation_settings=OpenAIGenerationSettings(
-                    temperature=temperature,
-                    top_k=top_k,
-                    top_p=top_p,
-                    min_p=min_p,
-                    stream=stream,
-                    stop_sequences=stop_sequences,
-                    echo=echo,
-                    repeat_penalty=repeat_penalty,
-                    logprobs=logprobs,
-                    presence_penalty=presence_penalty,
-                    frequency_penalty=frequency_penalty,
-                    logit_bias=logit_bias,
-                    logit_bias_type=logit_bias_type,
-                    mirostat_mode=mirostat_mode,
-                    mirostat_tau=mirostat_tau,
-                    mirostat_eta=mirostat_eta,
-                    seed=seed,
-                ),
-            )
-        else:
-            if isinstance(grammar, str):
-                if grammar in self.grammar_cache:
-                    grammar = self.grammar_cache[grammar]
-                else:
-                    grammar_string = grammar
-                    grammar = LlamaGrammar.from_string(grammar, False)
-                    self.grammar_cache[grammar_string] = grammar
-            completion = self.model.create_completion(
-                prompt=prompt,
-                max_tokens=max_tokens,
-                stream=stream,
-                stop=stop_sequences,
-                temperature=temperature,
-                top_k=top_k,
-                top_p=top_p,
-                min_p=min_p,
-                typical_p=typical_p,
-                mirostat_mode=mirostat_mode,
-                mirostat_tau=mirostat_tau,
-                mirostat_eta=mirostat_eta,
-                tfs_z=tfs_z,
-                repeat_penalty=repeat_penalty,
-                grammar=grammar,
-            )
-        return completion
-
-    async def async_get_response_role_and_completion(
-        self,
-        function_tool_registry: LlamaCppFunctionToolRegistry = None,
-        system_prompt: str = None,
-        message: str = None,
-        add_message_to_chat_history: bool = True,
-        role: Literal["system", "user", "assistant", "function"] = "user",
-        response_role: Literal["user", "assistant"] | None = None,
-        grammar: str = None,
-        prompt_suffix: str = None,
-        max_tokens: int = 0,
-        temperature: float = 0.4,
-        top_k: int = 0,
-        top_p: float = 1.0,
-        min_p: float = 0.05,
-        typical_p: float = 1.0,
-        repeat_penalty: float = 1.0,
-        mirostat_mode: int = 0,
-        mirostat_tau: float = 5.0,
-        mirostat_eta: float = 0.1,
-        tfs_z: float = 1.0,
-        stop_sequences: List[str] = None,
-        additional_stop_sequences: List[str] = None,
-        stream: bool = True,
-        k_last_messages: int = 0,
-        n_predict: int = -1,
-        n_keep: int = 0,
-        repeat_last_n: int = 64,
-        penalize_nl: bool = True,
-        presence_penalty: float = 0.0,
-        frequency_penalty: float = 0.0,
-        penalty_prompt: Union[None, str, List[int]] = None,
-        seed: int = -1,
-        ignore_eos: bool = False,
-        echo: bool = False,
-        logprobs: int = None,
-        logit_bias: Dict[str, float] = None,
-        logit_bias_type: Literal["input_ids", "tokens"] = None,
-        cache_prompt: bool = False,
-        samplers: List[str] = None,
-    ):
-        if function_tool_registry is not None:
-            grammar = function_tool_registry.gbnf_grammar
-
-        if system_prompt is None:
-            system_prompt = self.system_prompt
-        messages = [
-            {
-                "role": "system",
-                "content": system_prompt,
-            },
-        ]
-        if message is not None and add_message_to_chat_history:
-            self.messages.append(
-                {
-                    "role": role,
-                    "content": message,
-                },
-            )
-        if not add_message_to_chat_history and message is not None:
-            messages.append(
-                {
-                    "role": role,
-                    "content": message,
-                },
-            )
-        if k_last_messages > 0:
-            messages.extend(self.messages[-k_last_messages:])
-        else:
-            messages.extend(self.messages)
-
-        prompt, response_role = self.messages_formatter.format_messages(
-            messages, response_role
-        )
-
-        if prompt_suffix:
-            prompt += prompt_suffix
-
-        if self.debug_output:
-            print(prompt, end="")
-
-        if stop_sequences is None:
-            stop_sequences = self.messages_formatter.DEFAULT_STOP_SEQUENCES
-
-        if additional_stop_sequences is not None:
-            stop_sequences.extend(additional_stop_sequences)
-
-        if self.model:
-            if isinstance(self.model, LlamaCppEndpointSettings):
-                completion = await self.model.async_create_completion(
-                    prompt=prompt,
-                    grammar=grammar,
-                    generation_settings=LlamaCppGenerationSettings(
-                        temperature=temperature,
-                        top_k=top_k,
-                        top_p=top_p,
-                        min_p=min_p,
-                        n_predict=n_predict,
-                        n_keep=n_keep,
-                        stream=stream,
-                        stop_sequences=stop_sequences,
-                        tfs_z=tfs_z,
-                        typical_p=typical_p,
-                        repeat_penalty=repeat_penalty,
-                        repeat_last_n=repeat_last_n,
-                        penalize_nl=penalize_nl,
-                        presence_penalty=presence_penalty,
-                        frequency_penalty=frequency_penalty,
-                        penalty_prompt=penalty_prompt,
-                        mirostat_mode=mirostat_mode,
-                        mirostat_tau=mirostat_tau,
-                        mirostat_eta=mirostat_eta,
-                        samplers=samplers,
-                        seed=seed,
-                        cache_prompt=cache_prompt,
-                        ignore_eos=ignore_eos,
-                    ),
-                )
-            elif isinstance(self.model, OpenAIEndpointSettings):
-                completion = await self.model.async_create_completion(
-                    prompt=prompt,
-                    grammar=grammar,
-                    generation_settings=OpenAIGenerationSettings(
-                        temperature=temperature,
-                        top_k=top_k,
-                        top_p=top_p,
-                        min_p=min_p,
-                        stream=stream,
-                        stop_sequences=stop_sequences,
-                        echo=echo,
-                        repeat_penalty=repeat_penalty,
-                        logprobs=logprobs,
-                        presence_penalty=presence_penalty,
-                        frequency_penalty=frequency_penalty,
-                        logit_bias=logit_bias,
-                        logit_bias_type=logit_bias_type,
-                        mirostat_mode=mirostat_mode,
-                        mirostat_tau=mirostat_tau,
-                        mirostat_eta=mirostat_eta,
-                        seed=seed,
-                    ),
-                )
-            else:
-                if isinstance(grammar, str):
-                    if grammar in self.grammar_cache:
-                        grammar = self.grammar_cache[grammar]
-                    else:
-                        grammar_string = grammar
-                        grammar = LlamaGrammar.from_string(grammar, False)
-                        self.grammar_cache[grammar_string] = grammar
-                completion = self.model.create_completion(
-                    prompt=prompt,
-                    max_tokens=max_tokens,
-                    stream=stream,
-                    stop=stop_sequences,
-                    temperature=temperature,
-                    top_k=top_k,
-                    top_p=top_p,
-                    min_p=min_p,
-                    typical_p=typical_p,
-                    mirostat_mode=mirostat_mode,
-                    mirostat_tau=mirostat_tau,
-                    mirostat_eta=mirostat_eta,
-                    tfs_z=tfs_z,
-                    repeat_penalty=repeat_penalty,
-                    grammar=grammar,
-                )
-            return completion, response_role
-        return "Error: No model loaded!"
-
-    def remove_last_k_chat_messages(self, k: int):
-        """
-        Removes the last k messages from the chat history.
-
-        Args:
-            k (int): Number of last messages to remove.
-        """
-        # Ensure k is not greater than the length of the messages list
-        k = min(k, len(self.messages))
-
-        # Remove the last k elements
-        self.messages = self.messages[:-k] if k > 0 else self.messages
-
-    def remove_first_k_chat_messages(self, k: int):
-        """
-        Removes the first k messages from the chat history.
-
-        Args:
-            k (int): Number of first messages to remove.
-        """
-        # Ensure k is not greater than the length of the messages list
-        k = min(k, len(self.messages))
-
-        # Remove the first k elements
-        self.messages = self.messages[k:] if k > 0 else self.messages
-
-    def save_messages(self, file_path: str):
-        """
-        Saves the chat history messages to a file.
-
-        Args:
-           file_path (str): The file path to save the messages.
-        """
-        with open(file_path, "w", encoding="utf-8") as file:
-            json.dump(self.messages, file, indent=4)
-
-    def load_messages(self, file_path: str):
-        """
-        Loads chat history messages from a file.
-
-        Args:
-            file_path (str): The file path to load the messages from.
-        """
-        with open(file_path, "r", encoding="utf-8") as file:
-            loaded_messages = json.load(file)
-            self.messages.extend(loaded_messages)
-
-    @staticmethod
-    def agent_conversation(
-        agent_1: "LlamaCppAgent",
-        agent_2: "LlamaCppAgent",
-        agent_1_initial_message: str,
-        number_of_exchanges: int = 15,
-    ):
-        current_message = agent_1_initial_message
-        current_agent, next_agent = agent_2, agent_1
-
-        for _ in range(number_of_exchanges):
-            # Current agent responds to the last message
-            response = current_agent.get_chat_response(
-                message=current_message,
-                role="user",
-                add_response_to_chat_history=True,
-                print_output=True,
-                top_p=0.8,
-                top_k=40,
-            )
-
-            # Update the message for the next turn
-            current_message = response
-
-            # Swap the agents for the next turn
-            current_agent, next_agent = next_agent, current_agent
-
-        print("Conversation ended.")
-
-    @staticmethod
-    def group_conversation(
-        agent_list: list["LlamaCppAgent"],
-        initial_message: str,
-        number_of_turns: int = 4,
-    ):
-        responses = [
-            {
-                "role": "user",
-                "content": initial_message,
-            }
-        ]
-        for _ in range(number_of_turns):
-            for a in agent_list:
-                a.messages = copy(responses)
-                for response in a.messages:
-                    if response["content"].strip().startswith(a.name):
-                        response["role"] = "assistant"
-                response = a.get_chat_response(
-                    add_response_to_chat_history=False,
-                    add_message_to_chat_history=False,
-                    prompt_suffix=f"\n{a.name}:",
-                )
-                response = f"{a.name}:{response[0]}"
-                responses.append(
-                    {
-                        "role": "user",
-                        "content": response,
-                    }
-                )
-        print("Conversation ended.")
+import json
+from copy import copy
+from dataclasses import dataclass
+from typing import List, Dict, Literal, Callable, Union
+
+from llama_cpp import Llama, LlamaGrammar
+
+from .llm_settings import LlamaLLMSettings, LlamaLLMGenerationSettings
+from .messages_formatter import (
+    MessagesFormatterType,
+    get_predefined_messages_formatter,
+    MessagesFormatter,
+)
+from .function_calling import LlamaCppFunctionTool, LlamaCppFunctionToolRegistry
+from .providers.llama_cpp_endpoint_provider import (
+    LlamaCppEndpointSettings,
+    LlamaCppGenerationSettings,
+)
+from .providers.openai_endpoint_provider import (
+    OpenAIEndpointSettings,
+    OpenAIGenerationSettings,
+)
+
+
+@dataclass
+class StreamingResponse:
+    """
+    Represents a streaming response with text and an indicator for the last response.
+    """
+
+    text: str
+    is_last_response: bool
+
+    def __init__(self, text: str, is_last_response: bool):
+        """
+        Initializes a new StreamingResponse object.
+
+        Args:
+            text (str): The text content of the streaming response.
+            is_last_response (bool): Indicates whether this is the last response in the stream.
+        """
+        self.text = text
+        self.is_last_response = is_last_response
+
+
+class LlamaCppAgent:
+    """
+    A base agent that can be used for chat, structured output and function calling.
+     Is used as part of all other agents.
+    """
+
+    def __init__(
+        self,
+        model: Union[
+            Llama, LlamaLLMSettings, LlamaCppEndpointSettings, OpenAIEndpointSettings
+        ],
+        name: str = "llamacpp_agent",
+        system_prompt: str = "You are a helpful assistant.",
+        predefined_messages_formatter_type: MessagesFormatterType = MessagesFormatterType.CHATML,
+        custom_messages_formatter: MessagesFormatter = None,
+        debug_output: bool = False,
+        function_tool_registry: LlamaCppFunctionToolRegistry = None,
+    ):
+        """
+        Initializes a new LlamaCppAgent object.
+
+        Args:
+           model (Union[Llama, LlamaLLMSettings, LlamaCppEndpointSettings]):The underlying Llama model or settings.
+           name (str): The name of the agent.
+           system_prompt (str): The system prompt used in chat interactions.
+           predefined_messages_formatter_type (MessagesFormatterType): The type of predefined messages formatter.
+           custom_messages_formatter (MessagesFormatter): Custom messages formatter.
+           debug_output (bool): Indicates whether debug output should be enabled.
+           function_tool_registry (LlamaCppFunctionToolRegistry): The Llama function tool registry.
+        """
+        if isinstance(model, LlamaLLMSettings):
+            model = Llama(**model.as_dict())
+        self.model = model
+        self.name = name
+        self.system_prompt = system_prompt
+        self.debug_output = debug_output
+        self.messages = []
+        self.grammar_cache = {}
+        if custom_messages_formatter is not None:
+            self.messages_formatter = custom_messages_formatter
+        else:
+            self.messages_formatter = get_predefined_messages_formatter(
+                predefined_messages_formatter_type
+            )
+        self.last_response = ""
+        self.function_tool_registry = function_tool_registry
+
+    @staticmethod
+    def get_function_tool_registry(
+        function_tool_list: List[LlamaCppFunctionTool],
+        allow_parallel_function_calling=False,
+        add_inner_thoughts=False,
+        allow_inner_thoughts_only=False,
+        add_request_heartbeat=False,
+        tool_root="function",
+        tool_rule_content="parameters",
+        model_prefix="function",
+        fields_prefix="parameters",
+        inner_thoughts_field_name="thoughts_and_reasoning",
+        request_heartbeat_field_name="request_heartbeat",
+    ):
+        """
+        Creates and returns a function tool registry from a list of LlamaCppFunctionTool instances.
+
+        Args:
+            function_tool_list (List[LlamaCppFunctionTool]): List of function tools to register.
+            allow_parallel_function_calling: Allow parallel function calling (Default=False)
+            add_inner_thoughts: Add inner thoughts field (Default=False)
+            allow_inner_thoughts_only: Allow inner thoughts only (Default=False)
+            add_request_heartbeat: Add request heartbeat field (Default=False)
+            tool_root: The root name of the tool (Default="function")
+            tool_rule_content: The content of the tool rule (Default="parameters")
+            model_prefix: The prefix for the model in the documentation (Default="function")
+            fields_prefix: The prefix for the fields in the documentation (Default="parameters")
+            inner_thoughts_field_name: The name of the inner thoughts field (Default="thoughts_and_reasoning")
+            request_heartbeat_field_name: The name of the request heartbeat field (Default="request_heartbeat")
+        Returns:
+            LlamaCppFunctionToolRegistry: The created function tool registry.
+        """
+        function_tool_registry = LlamaCppFunctionToolRegistry(
+            allow_parallel_function_calling,
+            add_inner_thoughts,
+            allow_inner_thoughts_only,
+            add_request_heartbeat,
+            tool_root,
+            tool_rule_content,
+            model_prefix,
+            fields_prefix,
+            inner_thoughts_field_name,
+            request_heartbeat_field_name,
+        )
+
+        for function_tool in function_tool_list:
+            function_tool_registry.register_function_tool(function_tool)
+        function_tool_registry.finalize()
+        return function_tool_registry
+
+    def add_message(
+        self,
+        message: str,
+        role: (
+            Literal["system"]
+            | Literal["user"]
+            | Literal["assistant"]
+            | Literal["function"]
+        ) = "user",
+    ):
+        """
+        Adds a message to the chat history.
+
+        Args:
+            message (str): The content of the message.
+            role (Literal["system"] | Literal["user"] | Literal["assistant"]): The role of the message sender.
+        """
+        self.messages.append(
+            {
+                "role": role,
+                "content": message,
+            },
+        )
+
+    def get_text_response(
+        self,
+        prompt: str | list[int] = None,
+        grammar: str = None,
+        function_tool_registry: LlamaCppFunctionToolRegistry = None,
+        do_not_use_grammar: bool = False,
+        streaming_callback: Callable[[StreamingResponse], None] = None,
+        max_tokens: int = 0,
+        temperature: float = 0.4,
+        top_k: int = 0,
+        top_p: float = 1.0,
+        min_p: float = 0.05,
+        typical_p: float = 1.0,
+        repeat_penalty: float = 1.0,
+        mirostat_mode: int = 0,
+        mirostat_tau: float = 5.0,
+        mirostat_eta: float = 0.1,
+        tfs_z: float = 1.0,
+        stop_sequences: List[str] = None,
+        additional_stop_sequences: List[str] = None,
+        stream: bool = True,
+        print_output: bool = False,
+        # Llama Cpp Server and Open AI endpoint settings
+        n_predict: int = -1,
+        n_keep: int = 0,
+        repeat_last_n: int = 64,
+        penalize_nl: bool = True,
+        presence_penalty: float = 0.0,
+        frequency_penalty: float = 0.0,
+        penalty_prompt: Union[None, str, List[int]] = None,
+        seed: int = -1,
+        ignore_eos: bool = False,
+        echo: bool = False,
+        logprobs: int = None,
+        logit_bias: Dict[str, float] = None,
+        logit_bias_type: Literal["input_ids", "tokens"] = None,
+        samplers: List[str] = None,
+    ):
+        """ """
+        if function_tool_registry is None and do_not_use_grammar is False:
+            if self.function_tool_registry is not None:
+                function_tool_registry = self.function_tool_registry
+
+        if function_tool_registry is not None:
+            grammar = function_tool_registry.gbnf_grammar
+
+        if self.debug_output:
+            if type(prompt) is str:
+                print(prompt, end="")
+        if stop_sequences is None:
+            stop_sequences = self.messages_formatter.DEFAULT_STOP_SEQUENCES
+
+        if additional_stop_sequences is not None:
+            stop_sequences.extend(additional_stop_sequences)
+
+        if self.model:
+            completion = self.get_text_completion(
+                grammar=grammar,
+                prompt=prompt,
+                max_tokens=max_tokens,
+                temperature=temperature,
+                top_k=top_k,
+                top_p=top_p,
+                min_p=min_p,
+                typical_p=typical_p,
+                repeat_penalty=repeat_penalty,
+                mirostat_mode=mirostat_mode,
+                mirostat_tau=mirostat_tau,
+                mirostat_eta=mirostat_eta,
+                tfs_z=tfs_z,
+                stop_sequences=stop_sequences,
+                repeat_last_n=repeat_last_n,
+                penalize_nl=penalize_nl,
+                presence_penalty=presence_penalty,
+                frequency_penalty=frequency_penalty,
+                penalty_prompt=penalty_prompt,
+                ignore_eos=ignore_eos,
+                echo=echo,
+                logprobs=logprobs,
+                logit_bias=logit_bias,
+                logit_bias_type=logit_bias_type,
+                samplers=samplers,
+                n_predict=n_predict,
+                n_keep=n_keep,
+                seed=seed,
+            )
+            if stream:
+                full_response = ""
+                for out in completion:
+                    text = out["choices"][0]["text"]
+                    full_response += text
+                    if streaming_callback is not None:
+                        streaming_callback(
+                            StreamingResponse(text=text, is_last_response=False)
+                        )
+                    if print_output:
+                        print(text, end="")
+                if streaming_callback is not None:
+                    streaming_callback(
+                        StreamingResponse(text="", is_last_response=True)
+                    )
+                if print_output:
+                    print("")
+                self.last_response = full_response
+                if function_tool_registry is not None:
+                    full_response = function_tool_registry.handle_function_call(
+                        full_response
+                    )
+                return full_response if full_response else None
+            else:
+                full_response = ""
+                text = completion["choices"][0]["text"]
+                full_response += text
+                if print_output:
+                    print(full_response)
+                self.last_response = full_response
+                if function_tool_registry is not None:
+                    full_response = function_tool_registry.handle_function_call(
+                        full_response
+                    )
+                return full_response if full_response else None
+        return "Error: No model loaded!"
+
+    def get_text_response_generator(
+        self,
+        prompt: str | list[int] = None,
+        grammar: str = None,
+        function_tool_registry: LlamaCppFunctionToolRegistry = None,
+        do_not_use_grammar: bool = False,
+        streaming_callback: Callable[[StreamingResponse], None] = None,
+        max_tokens: int = 0,
+        temperature: float = 0.4,
+        top_k: int = 0,
+        top_p: float = 1.0,
+        min_p: float = 0.05,
+        typical_p: float = 1.0,
+        repeat_penalty: float = 1.0,
+        mirostat_mode: int = 0,
+        mirostat_tau: float = 5.0,
+        mirostat_eta: float = 0.1,
+        tfs_z: float = 1.0,
+        stop_sequences: List[str] = None,
+        print_output: bool = True,
+        # Llama Cpp Server and Open AI endpoint settings
+        n_predict: int = -1,
+        n_keep: int = 0,
+        repeat_last_n: int = 64,
+        penalize_nl: bool = True,
+        presence_penalty: float = 0.0,
+        frequency_penalty: float = 0.0,
+        penalty_prompt: Union[None, str, List[int]] = None,
+        seed: int = -1,
+        ignore_eos: bool = False,
+        echo: bool = False,
+        logprobs: int = None,
+        logit_bias: Dict[str, float] = None,
+        logit_bias_type: Literal["input_ids", "tokens"] = None,
+        samplers: List[str] = None,
+    ):
+        """ """
+        if function_tool_registry is None and do_not_use_grammar is False:
+            if self.function_tool_registry is not None:
+                function_tool_registry = self.function_tool_registry
+
+        if function_tool_registry is not None:
+            grammar = function_tool_registry.gbnf_grammar
+
+        if self.debug_output:
+            if type(prompt) is str:
+                print(prompt, end="")
+        if stop_sequences is None:
+            stop_sequences = []
+
+        if self.model:
+            completion = self.get_text_completion(
+                grammar=grammar,
+                prompt=prompt,
+                max_tokens=max_tokens,
+                temperature=temperature,
+                top_k=top_k,
+                top_p=top_p,
+                min_p=min_p,
+                typical_p=typical_p,
+                repeat_penalty=repeat_penalty,
+                mirostat_mode=mirostat_mode,
+                mirostat_tau=mirostat_tau,
+                mirostat_eta=mirostat_eta,
+                tfs_z=tfs_z,
+                stop_sequences=stop_sequences,
+                repeat_last_n=repeat_last_n,
+                penalize_nl=penalize_nl,
+                presence_penalty=presence_penalty,
+                frequency_penalty=frequency_penalty,
+                penalty_prompt=penalty_prompt,
+                ignore_eos=ignore_eos,
+                echo=echo,
+                logprobs=logprobs,
+                logit_bias=logit_bias,
+                logit_bias_type=logit_bias_type,
+                samplers=samplers,
+                n_predict=n_predict,
+                n_keep=n_keep,
+                seed=seed,
+            )
+            full_response = ""
+            for out in completion:
+                text = out["choices"][0]["text"]
+                full_response += text
+                yield text
+                if streaming_callback is not None:
+                    streaming_callback(
+                        StreamingResponse(text=text, is_last_response=False)
+                    )
+                if print_output:
+                    print(text, end="")
+            if streaming_callback is not None:
+                streaming_callback(StreamingResponse(text="", is_last_response=True))
+            if print_output:
+                print("")
+            self.last_response = full_response
+            if function_tool_registry is not None:
+                full_response = function_tool_registry.handle_function_call(
+                    full_response
+                )
+                yield full_response if full_response else None
+            return
+        return "Error: No model loaded!"
+
+    def get_chat_response(
+        self,
+        message: str = None,
+        role: Literal["system", "user", "assistant", "function"] = "user",
+        response_role: Literal["user", "assistant"] | None = None,
+        system_prompt: str = None,
+        prompt_suffix: str = None,
+        add_message_to_chat_history: bool = True,
+        add_response_to_chat_history: bool = True,
+        grammar: str = None,
+        function_tool_registry: LlamaCppFunctionToolRegistry = None,
+        do_not_use_grammar: bool = False,
+        streaming_callback: Callable[[StreamingResponse], None] = None,
+        max_tokens: int = 0,
+        temperature: float = 0.4,
+        top_k: int = 0,
+        top_p: float = 1.0,
+        min_p: float = 0.05,
+        typical_p: float = 1.0,
+        repeat_penalty: float = 1.0,
+        mirostat_mode: int = 0,
+        mirostat_tau: float = 5.0,
+        mirostat_eta: float = 0.1,
+        tfs_z: float = 1.0,
+        stop_sequences: List[str] = None,
+        additional_stop_sequences: List[str] = None,
+        stream: bool = True,
+        print_output: bool = True,
+        k_last_messages: int = 0,
+        # Llama Cpp Server and Open AI endpoint settings
+        n_predict: int = -1,
+        n_keep: int = 0,
+        repeat_last_n: int = 64,
+        penalize_nl: bool = True,
+        presence_penalty: float = 0.0,
+        frequency_penalty: float = 0.0,
+        penalty_prompt: Union[None, str, List[int]] = None,
+        seed: int = -1,
+        ignore_eos: bool = False,
+        echo: bool = False,
+        logprobs: int = None,
+        logit_bias: Dict[str, float] = None,
+        logit_bias_type: Literal["input_ids", "tokens"] = None,
+        cache_prompt: bool = False,
+        samplers: List[str] = None,
+    ):
+        """
+        Gets a chat response based on the input message and context.
+
+        Args:
+            message (str): The input message.
+            role (Literal["system", "user", "assistant", "function"]): The role of the message sender.
+            response_role (Literal["user", "assistant"]): The role of the message response.
+            system_prompt (str): The system prompt used in chat interactions.
+            prompt_suffix: Suffix to append after the prompt.
+            add_message_to_chat_history (bool): Indicates whether to add the input message to the chat history.
+            add_response_to_chat_history (bool): Indicates whether to add the generated response to the chat history.
+            grammar (str): The grammar for generating responses in string format.
+            function_tool_registry (LlamaCppFunctionToolRegistry): The function tool registry for handling function calls.
+            do_not_use_grammar (bool): Indicates whether to use grammar when generating responses.
+            streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
+
+            max_tokens (int): The maximum number of tokens in the generated response.
+            temperature (float): The temperature parameter for response generation.
+            top_k (int): Top-k parameter for response generation.
+            top_p (float): Top-p parameter for response generation.
+            min_p (float): Minimum probability parameter for response generation.
+            typical_p (float): Typical probability parameter for response generation.
+            repeat_penalty (float): Penalty for repeating tokens in response generation.
+            mirostat_mode (int): Mirostat mode for response generation.
+            mirostat_tau (float): Mirostat tau parameter for response generation.
+            mirostat_eta (float): Mirostat eta parameter for response generation.
+            tfs_z (float): TFS Z parameter for response generation.
+            stop_sequences (List[str]): List of stop sequences for response generation. Overwrites default stop sequences!
+            additional_stop_sequences (List[str]): List of stop sequences for response generation, additional to the default ones.
+            stream (bool): Indicates whether to stream the response.
+            print_output (bool): Indicates whether to print the generated response.
+            k_last_messages (int): Number of last messages to consider from the chat history.
+
+
+            Additional parameters for llama.cpp server backends and OpenAI endpoints
+            n_predict (int): Number of predictions to generate for each completion.
+            n_keep (int): Number of completions to keep.
+            repeat_last_n (int): Number of tokens to consider for repeat penalty.
+            penalize_nl (bool): Indicates whether to penalize newline characters in response generation.
+            presence_penalty (float): Presence penalty parameter for response generation.
+            frequency_penalty (float): Frequency penalty parameter for response generation.
+            penalty_prompt (Union[None, str, List[int]]): Penalty prompt for response generation.
+            seed (int): Seed for random number generation.
+            ignore_eos (bool): Indicates whether to ignore end-of-sequence tokens.
+            echo: bool = False,
+            logprobs: int = None,
+            logit_bias: Dict[str, float] = None,
+            logit_bias_type:Literal["input_ids", "tokens"] = None
+            cache_prompt: bool = False,
+            samplers: List[str] = None
+        Returns:
+            list[dict]|str: The generated chat response.
+        """
+        if function_tool_registry is None and do_not_use_grammar is False:
+            if self.function_tool_registry is not None:
+                function_tool_registry = self.function_tool_registry
+        completion, response_role = self.get_response_role_and_completion(
+            function_tool_registry=function_tool_registry,
+            system_prompt=system_prompt,
+            message=message,
+            add_message_to_chat_history=add_message_to_chat_history,
+            role=role,
+            response_role=response_role,
+            grammar=grammar,
+            prompt_suffix=prompt_suffix,
+            max_tokens=max_tokens,
+            temperature=temperature,
+            top_k=top_k,
+            top_p=top_p,
+            min_p=min_p,
+            typical_p=typical_p,
+            repeat_penalty=repeat_penalty,
+            mirostat_mode=mirostat_mode,
+            mirostat_tau=mirostat_tau,
+            mirostat_eta=mirostat_eta,
+            tfs_z=tfs_z,
+            stop_sequences=stop_sequences,
+            additional_stop_sequences=additional_stop_sequences,
+            stream=stream,
+            k_last_messages=k_last_messages,
+            n_predict=n_predict,
+            n_keep=n_keep,
+            repeat_last_n=repeat_last_n,
+            penalize_nl=penalize_nl,
+            presence_penalty=presence_penalty,
+            frequency_penalty=frequency_penalty,
+            penalty_prompt=penalty_prompt,
+            seed=seed,
+            ignore_eos=ignore_eos,
+            echo=echo,
+            logprobs=logprobs,
+            logit_bias=logit_bias,
+            logit_bias_type=logit_bias_type,
+            cache_prompt=cache_prompt,
+            samplers=samplers,
+        )
+        if self.model:
+            if stream:
+                full_response = ""
+                for out in completion:
+                    text = out["choices"][0]["text"]
+                    full_response += text
+                    if streaming_callback is not None:
+                        streaming_callback(
+                            StreamingResponse(text=text, is_last_response=False)
+                        )
+                    if print_output:
+                        print(text, end="")
+                if streaming_callback is not None:
+                    streaming_callback(
+                        StreamingResponse(text="", is_last_response=True)
+                    )
+                if print_output:
+                    print("")
+
+                self.last_response = full_response
+                if add_response_to_chat_history:
+                    self.messages.append(
+                        {
+                            "role": response_role,
+                            "content": full_response,
+                        },
+                    )
+                if function_tool_registry is not None:
+                    full_response = function_tool_registry.handle_function_call(
+                        full_response
+                    )
+                return full_response if full_response else None
+            else:
+                text = completion["choices"][0]["text"]
+                if print_output:
+                    print(text)
+                self.last_response = text
+                if add_response_to_chat_history:
+                    self.messages.append(
+                        {
+                            "role": response_role,
+                            "content": text,
+                        },
+                    )
+                if function_tool_registry is not None:
+                    text = function_tool_registry.handle_function_call(text)
+                return text if text else None
+        return "Error: No model loaded!"
+
+    def get_chat_response_generator(
+        self,
+        message: str = None,
+        role: Literal["system", "user", "assistant", "function"] = "user",
+        response_role: Literal["user", "assistant"] | None = None,
+        system_prompt: str = None,
+        prompt_suffix: str = None,
+        add_message_to_chat_history: bool = True,
+        add_response_to_chat_history: bool = True,
+        grammar: str = None,
+        function_tool_registry: LlamaCppFunctionToolRegistry = None,
+        do_not_use_grammar: bool = False,
+        streaming_callback: Callable[[StreamingResponse], None] = None,
+        max_tokens: int = 0,
+        temperature: float = 0.4,
+        top_k: int = 0,
+        top_p: float = 1.0,
+        min_p: float = 0.05,
+        typical_p: float = 1.0,
+        repeat_penalty: float = 1.0,
+        mirostat_mode: int = 0,
+        mirostat_tau: float = 5.0,
+        mirostat_eta: float = 0.1,
+        tfs_z: float = 1.0,
+        stop_sequences: List[str] = None,
+        additional_stop_sequences: List[str] = None,
+        print_output: bool = True,
+        k_last_messages: int = 0,
+        # Llama Cpp Server and Open AI endpoint settings
+        n_predict: int = -1,
+        n_keep: int = 0,
+        repeat_last_n: int = 64,
+        penalize_nl: bool = True,
+        presence_penalty: float = 0.0,
+        frequency_penalty: float = 0.0,
+        penalty_prompt: Union[None, str, List[int]] = None,
+        seed: int = -1,
+        ignore_eos: bool = False,
+        echo: bool = False,
+        logprobs: int = None,
+        logit_bias: Dict[str, float] = None,
+        logit_bias_type: Literal["input_ids", "tokens"] = None,
+        cache_prompt: bool = False,
+        samplers: List[str] = None,
+    ):
+        """
+        Gets a chat response based on the input message and context.
+
+        Args:
+            message (str): The input message.
+            role (Literal["system", "user", "assistant", "function"]): The role of the message sender.
+            response_role (Literal["user", "assistant"]): The role of the message response.
+            system_prompt (str): The system prompt used in chat interactions.
+            prompt_suffix: Suffix to append after the prompt.
+            add_message_to_chat_history (bool): Indicates whether to add the input message to the chat history.
+            add_response_to_chat_history (bool): Indicates whether to add the generated response to the chat history.
+            grammar (str): The grammar for generating responses in string format.
+            function_tool_registry (LlamaCppFunctionToolRegistry): The function tool registry for handling function calls.
+            do_not_use_grammar (bool): Indicates whether to use grammar when generating responses.
+            streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
+            max_tokens (int): The maximum number of tokens in the generated response.
+            temperature (float): The temperature parameter for response generation.
+            top_k (int): Top-k parameter for response generation.
+            top_p (float): Top-p parameter for response generation.
+            min_p (float): Minimum probability parameter for response generation.
+            typical_p (float): Typical probability parameter for response generation.
+            repeat_penalty (float): Penalty for repeating tokens in response generation.
+            mirostat_mode (int): Mirostat mode for response generation.
+            mirostat_tau (float): Mirostat tau parameter for response generation.
+            mirostat_eta (float): Mirostat eta parameter for response generation.
+            tfs_z (float): TFS Z parameter for response generation.
+            stop_sequences (List[str]): List of stop sequences for response generation. Overwrites default stop sequences!
+            additional_stop_sequences (List[str]): List of stop sequences for response generation, additional to the default ones.
+            print_output (bool): Indicates whether to print the generated response.
+            k_last_messages (int): Number of last messages to consider from the chat history.
+
+
+            Additional parameters for llama.cpp server backends and OpenAI endpoints
+            n_predict (int): Number of predictions to generate for each completion.
+            n_keep (int): Number of completions to keep.
+            repeat_last_n (int): Number of tokens to consider for repeat penalty.
+            penalize_nl (bool): Indicates whether to penalize newline characters in response generation.
+            presence_penalty (float): Presence penalty parameter for response generation.
+            frequency_penalty (float): Frequency penalty parameter for response generation.
+            penalty_prompt (Union[None, str, List[int]]): Penalty prompt for response generation.
+            seed (int): Seed for random number generation.
+            ignore_eos (bool): Indicates whether to ignore end-of-sequence tokens.
+            echo: bool = False,
+            logprobs: int = None,
+            logit_bias: Dict[str, float] = None,
+            logit_bias_type:Literal["input_ids", "tokens"] = None
+            cache_prompt: bool = False,
+            samplers: List[str] = None
+        Returns:
+            list[dict]: The generated chat response.
+        """
+        if function_tool_registry is None and do_not_use_grammar is False:
+            if self.function_tool_registry is not None:
+                function_tool_registry = self.function_tool_registry
+
+        completion, response_role = self.get_response_role_and_completion(
+            function_tool_registry=function_tool_registry,
+            system_prompt=system_prompt,
+            message=message,
+            add_message_to_chat_history=add_message_to_chat_history,
+            role=role,
+            response_role=response_role,
+            grammar=grammar,
+            prompt_suffix=prompt_suffix,
+            max_tokens=max_tokens,
+            temperature=temperature,
+            top_k=top_k,
+            top_p=top_p,
+            min_p=min_p,
+            typical_p=typical_p,
+            repeat_penalty=repeat_penalty,
+            mirostat_mode=mirostat_mode,
+            mirostat_tau=mirostat_tau,
+            mirostat_eta=mirostat_eta,
+            tfs_z=tfs_z,
+            stop_sequences=stop_sequences,
+            additional_stop_sequences=additional_stop_sequences,
+            stream=True,
+            k_last_messages=k_last_messages,
+            n_predict=n_predict,
+            n_keep=n_keep,
+            repeat_last_n=repeat_last_n,
+            penalize_nl=penalize_nl,
+            presence_penalty=presence_penalty,
+            frequency_penalty=frequency_penalty,
+            penalty_prompt=penalty_prompt,
+            seed=seed,
+            ignore_eos=ignore_eos,
+            echo=echo,
+            logprobs=logprobs,
+            logit_bias=logit_bias,
+            logit_bias_type=logit_bias_type,
+            cache_prompt=cache_prompt,
+            samplers=samplers,
+        )
+        if self.model:
+            full_response = ""
+            for out in completion:
+                text = out["choices"][0]["text"]
+                full_response += text
+                yield text
+                if streaming_callback is not None:
+                    streaming_callback(
+                        StreamingResponse(text=text, is_last_response=False)
+                    )
+                if print_output:
+                    print(text, end="")
+            if streaming_callback is not None:
+                streaming_callback(StreamingResponse(text="", is_last_response=True))
+            if print_output:
+                print("")
+
+            self.last_response = full_response
+            if add_response_to_chat_history:
+                self.messages.append(
+                    {
+                        "role": response_role,
+                        "content": full_response,
+                    },
+                )
+            if function_tool_registry is not None:
+                full_response = function_tool_registry.handle_function_call(
+                    full_response
+                )
+                yield full_response if full_response else None
+            return
+        return "Error: No model loaded!"
+
+    def get_text_completion(
+        self,
+        prompt: str | list[int] = None,
+        grammar: str = None,
+        max_tokens: int = 0,
+        temperature: float = 0.4,
+        top_k: int = 0,
+        top_p: float = 1.0,
+        min_p: float = 0.05,
+        typical_p: float = 1.0,
+        repeat_penalty: float = 1.0,
+        mirostat_mode: int = 0,
+        mirostat_tau: float = 5.0,
+        mirostat_eta: float = 0.1,
+        tfs_z: float = 1.0,
+        # Llama Cpp Server and Open AI endpoint settings
+        n_predict: int = -1,
+        n_keep: int = 0,
+        repeat_last_n: int = 64,
+        penalize_nl: bool = True,
+        presence_penalty: float = 0.0,
+        frequency_penalty: float = 0.0,
+        penalty_prompt: Union[None, str, List[int]] = None,
+        seed: int = -1,
+        ignore_eos: bool = False,
+        echo: bool = False,
+        logprobs: int = None,
+        logit_bias: Dict[str, float] = None,
+        logit_bias_type: Literal["input_ids", "tokens"] = None,
+        samplers: List[str] = None,
+        stop_sequences: List[str] = None,
+    ):
+        if isinstance(self.model, LlamaCppEndpointSettings):
+            completion = self.model.create_completion(
+                prompt=prompt,
+                grammar=grammar,
+                generation_settings=LlamaCppGenerationSettings(
+                    temperature=temperature,
+                    top_k=top_k,
+                    top_p=top_p,
+                    min_p=min_p,
+                    n_predict=n_predict,
+                    n_keep=n_keep,
+                    stream=True,
+                    stop_sequences=stop_sequences,
+                    tfs_z=tfs_z,
+                    typical_p=typical_p,
+                    repeat_penalty=repeat_penalty,
+                    repeat_last_n=repeat_last_n,
+                    penalize_nl=penalize_nl,
+                    presence_penalty=presence_penalty,
+                    frequency_penalty=frequency_penalty,
+                    penalty_prompt=penalty_prompt,
+                    mirostat_mode=mirostat_mode,
+                    mirostat_tau=mirostat_tau,
+                    mirostat_eta=mirostat_eta,
+                    seed=seed,
+                    samplers=samplers,
+                    ignore_eos=ignore_eos,
+                ),
+            )
+        elif isinstance(self.model, OpenAIEndpointSettings):
+            completion = self.model.create_completion(
+                prompt=prompt,
+                grammar=grammar,
+                generation_settings=OpenAIGenerationSettings(
+                    temperature=temperature,
+                    top_k=top_k,
+                    top_p=top_p,
+                    min_p=min_p,
+                    stream=True,
+                    stop_sequences=stop_sequences,
+                    echo=echo,
+                    repeat_penalty=repeat_penalty,
+                    logprobs=logprobs,
+                    presence_penalty=presence_penalty,
+                    frequency_penalty=frequency_penalty,
+                    logit_bias=logit_bias,
+                    logit_bias_type=logit_bias_type,
+                    mirostat_mode=mirostat_mode,
+                    mirostat_tau=mirostat_tau,
+                    mirostat_eta=mirostat_eta,
+                    seed=seed,
+                ),
+            )
+        else:
+            if isinstance(grammar, str):
+                if grammar in self.grammar_cache:
+                    grammar = self.grammar_cache[grammar]
+                else:
+                    grammar_string = grammar
+                    grammar = LlamaGrammar.from_string(grammar, False)
+                    self.grammar_cache[grammar_string] = grammar
+            completion = self.model.create_completion(
+                prompt=prompt,
+                max_tokens=max_tokens,
+                stream=True,
+                stop=stop_sequences,
+                temperature=temperature,
+                top_k=top_k,
+                top_p=top_p,
+                min_p=min_p,
+                typical_p=typical_p,
+                mirostat_mode=mirostat_mode,
+                mirostat_tau=mirostat_tau,
+                mirostat_eta=mirostat_eta,
+                tfs_z=tfs_z,
+                repeat_penalty=repeat_penalty,
+                grammar=grammar,
+            )
+        return completion
+
+    def get_response_role_and_completion(
+        self,
+        function_tool_registry: LlamaCppFunctionToolRegistry = None,
+        system_prompt: str = None,
+        message: str = None,
+        add_message_to_chat_history: bool = True,
+        role: Literal["system", "user", "assistant", "function"] = "user",
+        response_role: Literal["user", "assistant"] | None = None,
+        grammar: str = None,
+        prompt_suffix: str = None,
+        max_tokens: int = 0,
+        temperature: float = 0.4,
+        top_k: int = 0,
+        top_p: float = 1.0,
+        min_p: float = 0.05,
+        typical_p: float = 1.0,
+        repeat_penalty: float = 1.0,
+        mirostat_mode: int = 0,
+        mirostat_tau: float = 5.0,
+        mirostat_eta: float = 0.1,
+        tfs_z: float = 1.0,
+        stop_sequences: List[str] = None,
+        additional_stop_sequences: List[str] = None,
+        stream: bool = True,
+        k_last_messages: int = 0,
+        n_predict: int = -1,
+        n_keep: int = 0,
+        repeat_last_n: int = 64,
+        penalize_nl: bool = True,
+        presence_penalty: float = 0.0,
+        frequency_penalty: float = 0.0,
+        penalty_prompt: Union[None, str, List[int]] = None,
+        seed: int = -1,
+        ignore_eos: bool = False,
+        echo: bool = False,
+        logprobs: int = None,
+        logit_bias: Dict[str, float] = None,
+        logit_bias_type: Literal["input_ids", "tokens"] = None,
+        cache_prompt: bool = False,
+        samplers: List[str] = None,
+    ):
+        if function_tool_registry is not None:
+            grammar = function_tool_registry.gbnf_grammar
+
+        if system_prompt is None:
+            system_prompt = self.system_prompt
+        messages = [
+            {
+                "role": "system",
+                "content": system_prompt,
+            },
+        ]
+        if message is not None and add_message_to_chat_history:
+            self.messages.append(
+                {
+                    "role": role,
+                    "content": message,
+                },
+            )
+        if not add_message_to_chat_history and message is not None:
+            messages.append(
+                {
+                    "role": role,
+                    "content": message,
+                },
+            )
+        if k_last_messages > 0:
+            messages.extend(self.messages[-k_last_messages:])
+        else:
+            messages.extend(self.messages)
+
+        prompt, response_role = self.messages_formatter.format_messages(
+            messages, response_role
+        )
+
+        if prompt_suffix:
+            prompt += prompt_suffix
+
+        if self.debug_output:
+            print(prompt, end="")
+
+        if stop_sequences is None:
+            stop_sequences = self.messages_formatter.DEFAULT_STOP_SEQUENCES
+
+        if additional_stop_sequences is not None:
+            stop_sequences.extend(additional_stop_sequences)
+
+        if self.model:
+            if isinstance(self.model, LlamaCppEndpointSettings):
+                completion = self.model.create_completion(
+                    prompt=prompt,
+                    grammar=grammar,
+                    generation_settings=LlamaCppGenerationSettings(
+                        temperature=temperature,
+                        top_k=top_k,
+                        top_p=top_p,
+                        min_p=min_p,
+                        n_predict=n_predict,
+                        n_keep=n_keep,
+                        stream=stream,
+                        stop_sequences=stop_sequences,
+                        tfs_z=tfs_z,
+                        typical_p=typical_p,
+                        repeat_penalty=repeat_penalty,
+                        repeat_last_n=repeat_last_n,
+                        penalize_nl=penalize_nl,
+                        presence_penalty=presence_penalty,
+                        frequency_penalty=frequency_penalty,
+                        penalty_prompt=penalty_prompt,
+                        mirostat_mode=mirostat_mode,
+                        mirostat_tau=mirostat_tau,
+                        mirostat_eta=mirostat_eta,
+                        samplers=samplers,
+                        seed=seed,
+                        cache_prompt=cache_prompt,
+                        ignore_eos=ignore_eos,
+                    ),
+                )
+            elif isinstance(self.model, OpenAIEndpointSettings):
+                completion = self.model.create_completion(
+                    prompt=prompt,
+                    grammar=grammar,
+                    generation_settings=OpenAIGenerationSettings(
+                        temperature=temperature,
+                        top_k=top_k,
+                        top_p=top_p,
+                        min_p=min_p,
+                        stream=stream,
+                        stop_sequences=stop_sequences,
+                        echo=echo,
+                        repeat_penalty=repeat_penalty,
+                        logprobs=logprobs,
+                        presence_penalty=presence_penalty,
+                        frequency_penalty=frequency_penalty,
+                        logit_bias=logit_bias,
+                        logit_bias_type=logit_bias_type,
+                        mirostat_mode=mirostat_mode,
+                        mirostat_tau=mirostat_tau,
+                        mirostat_eta=mirostat_eta,
+                        seed=seed,
+                    ),
+                )
+            else:
+                if isinstance(grammar, str):
+                    if grammar in self.grammar_cache:
+                        grammar = self.grammar_cache[grammar]
+                    else:
+                        grammar_string = grammar
+                        grammar = LlamaGrammar.from_string(grammar, False)
+                        self.grammar_cache[grammar_string] = grammar
+                completion = self.model.create_completion(
+                    prompt=prompt,
+                    max_tokens=max_tokens,
+                    stream=stream,
+                    stop=stop_sequences,
+                    temperature=temperature,
+                    top_k=top_k,
+                    top_p=top_p,
+                    min_p=min_p,
+                    typical_p=typical_p,
+                    mirostat_mode=mirostat_mode,
+                    mirostat_tau=mirostat_tau,
+                    mirostat_eta=mirostat_eta,
+                    tfs_z=tfs_z,
+                    repeat_penalty=repeat_penalty,
+                    grammar=grammar,
+                )
+            return completion, response_role
+        return "Error: No model loaded!"
+
+    async def async_get_text_response(
+        self,
+        prompt: str | list[int] = None,
+        grammar: str = None,
+        function_tool_registry: LlamaCppFunctionToolRegistry = None,
+        do_not_use_grammar: bool = False,
+        streaming_callback: Callable[[StreamingResponse], None] = None,
+        max_tokens: int = 0,
+        temperature: float = 0.4,
+        top_k: int = 0,
+        top_p: float = 1.0,
+        min_p: float = 0.05,
+        typical_p: float = 1.0,
+        repeat_penalty: float = 1.0,
+        mirostat_mode: int = 0,
+        mirostat_tau: float = 5.0,
+        mirostat_eta: float = 0.1,
+        tfs_z: float = 1.0,
+        stop_sequences: List[str] = None,
+        additional_stop_sequences: List[str] = None,
+        stream: bool = True,
+        print_output: bool = True,
+        # Llama Cpp Server and Open AI endpoint settings
+        n_predict: int = -1,
+        n_keep: int = 0,
+        repeat_last_n: int = 64,
+        penalize_nl: bool = True,
+        presence_penalty: float = 0.0,
+        frequency_penalty: float = 0.0,
+        penalty_prompt: Union[None, str, List[int]] = None,
+        seed: int = -1,
+        ignore_eos: bool = False,
+        echo: bool = False,
+        logprobs: int = None,
+        logit_bias: Dict[str, float] = None,
+        logit_bias_type: Literal["input_ids", "tokens"] = None,
+        samplers: List[str] = None,
+    ):
+        """ """
+        if function_tool_registry is None and do_not_use_grammar is False:
+            if self.function_tool_registry is not None:
+                function_tool_registry = self.function_tool_registry
+
+        if function_tool_registry is not None:
+            grammar = function_tool_registry.gbnf_grammar
+
+        if self.debug_output:
+            if type(prompt) is str:
+                print(prompt, end="")
+        if stop_sequences is None:
+            stop_sequences = self.messages_formatter.DEFAULT_STOP_SEQUENCES
+
+        if additional_stop_sequences is not None:
+            stop_sequences.extend(additional_stop_sequences)
+
+        if self.model:
+            completion = await self.async_get_text_completion(
+                grammar=grammar,
+                prompt=prompt,
+                max_tokens=max_tokens,
+                temperature=temperature,
+                top_k=top_k,
+                top_p=top_p,
+                min_p=min_p,
+                typical_p=typical_p,
+                repeat_penalty=repeat_penalty,
+                mirostat_mode=mirostat_mode,
+                mirostat_tau=mirostat_tau,
+                mirostat_eta=mirostat_eta,
+                tfs_z=tfs_z,
+                stop_sequences=stop_sequences,
+                repeat_last_n=repeat_last_n,
+                penalize_nl=penalize_nl,
+                presence_penalty=presence_penalty,
+                frequency_penalty=frequency_penalty,
+                penalty_prompt=penalty_prompt,
+                ignore_eos=ignore_eos,
+                echo=echo,
+                logprobs=logprobs,
+                logit_bias=logit_bias,
+                logit_bias_type=logit_bias_type,
+                samplers=samplers,
+                n_predict=n_predict,
+                n_keep=n_keep,
+                seed=seed,
+                stream=stream,
+            )
+            if stream:
+                full_response = ""
+                async for out in completion:
+                    text = out["choices"][0]["text"]
+                    full_response += text
+                    if streaming_callback is not None:
+                        streaming_callback(
+                            StreamingResponse(text=text, is_last_response=False)
+                        )
+                    if print_output:
+                        print(text, end="")
+                if streaming_callback is not None:
+                    streaming_callback(
+                        StreamingResponse(text="", is_last_response=True)
+                    )
+                if print_output:
+                    print("")
+                self.last_response = full_response
+                if function_tool_registry is not None:
+                    full_response = function_tool_registry.handle_function_call(
+                        full_response
+                    )
+                    return full_response if full_response else None
+                return full_response if full_response else None
+            else:
+                text = completion["choices"][0]["text"]
+                self.last_response = text
+                if print_output:
+                    print(text)
+                if function_tool_registry is not None:
+                    text = function_tool_registry.handle_function_call(text)
+                    return text if text else None
+                return text if text else None
+        return "Error: No model loaded!"
+
+    async def async_get_chat_response(
+        self,
+        message: str = None,
+        role: Literal["system", "user", "assistant", "function"] = "user",
+        response_role: Literal["user", "assistant"] | None = None,
+        system_prompt: str = None,
+        prompt_suffix: str = None,
+        add_message_to_chat_history: bool = True,
+        add_response_to_chat_history: bool = True,
+        grammar: str = None,
+        function_tool_registry: LlamaCppFunctionToolRegistry = None,
+        do_not_use_grammar: bool = False,
+        streaming_callback: Callable[[StreamingResponse], None] = None,
+        max_tokens: int = 0,
+        temperature: float = 0.4,
+        top_k: int = 0,
+        top_p: float = 1.0,
+        min_p: float = 0.05,
+        typical_p: float = 1.0,
+        repeat_penalty: float = 1.0,
+        mirostat_mode: int = 0,
+        mirostat_tau: float = 5.0,
+        mirostat_eta: float = 0.1,
+        tfs_z: float = 1.0,
+        stop_sequences: List[str] = None,
+        additional_stop_sequences: List[str] = None,
+        stream: bool = False,
+        print_output: bool = True,
+        k_last_messages: int = 0,
+        # Llama Cpp Server and Open AI endpoint settings
+        n_predict: int = -1,
+        n_keep: int = 0,
+        repeat_last_n: int = 64,
+        penalize_nl: bool = True,
+        presence_penalty: float = 0.0,
+        frequency_penalty: float = 0.0,
+        penalty_prompt: Union[None, str, List[int]] = None,
+        seed: int = -1,
+        ignore_eos: bool = False,
+        echo: bool = False,
+        logprobs: int = None,
+        logit_bias: Dict[str, float] = None,
+        logit_bias_type: Literal["input_ids", "tokens"] = None,
+        cache_prompt: bool = False,
+        samplers: List[str] = None,
+    ):
+        """
+        Gets a chat response based on the input message and context.
+
+        Args:
+            message (str): The input message.
+            role (Literal["system", "user", "assistant", "function"]): The role of the message sender.
+            response_role (Literal["user", "assistant"]): The role of the message response.
+            system_prompt (str): The system prompt used in chat interactions.
+            prompt_suffix: Suffix to append after the prompt.
+            add_message_to_chat_history (bool): Indicates whether to add the input message to the chat history.
+            add_response_to_chat_history (bool): Indicates whether to add the generated response to the chat history.
+            grammar (str): The grammar for generating responses in string format.
+            function_tool_registry (LlamaCppFunctionToolRegistry): The function tool registry for handling function calls.
+            do_not_use_grammar (bool): Indicates whether to use grammar when generating responses.
+            streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
+
+            max_tokens (int): The maximum number of tokens in the generated response.
+            temperature (float): The temperature parameter for response generation.
+            top_k (int): Top-k parameter for response generation.
+            top_p (float): Top-p parameter for response generation.
+            min_p (float): Minimum probability parameter for response generation.
+            typical_p (float): Typical probability parameter for response generation.
+            repeat_penalty (float): Penalty for repeating tokens in response generation.
+            mirostat_mode (int): Mirostat mode for response generation.
+            mirostat_tau (float): Mirostat tau parameter for response generation.
+            mirostat_eta (float): Mirostat eta parameter for response generation.
+            tfs_z (float): TFS Z parameter for response generation.
+            stop_sequences (List[str]): List of stop sequences for response generation. Overwrites default stop sequences!
+            additional_stop_sequences (List[str]): List of stop sequences for response generation, additional to the default ones.
+            stream (bool): Indicates whether to stream the response.
+            print_output (bool): Indicates whether to print the generated response.
+            k_last_messages (int): Number of last messages to consider from the chat history.
+
+
+            Additional parameters for llama.cpp server backends and OpenAI endpoints
+            n_predict (int): Number of predictions to generate for each completion.
+            n_keep (int): Number of completions to keep.
+            repeat_last_n (int): Number of tokens to consider for repeat penalty.
+            penalize_nl (bool): Indicates whether to penalize newline characters in response generation.
+            presence_penalty (float): Presence penalty parameter for response generation.
+            frequency_penalty (float): Frequency penalty parameter for response generation.
+            penalty_prompt (Union[None, str, List[int]]): Penalty prompt for response generation.
+            seed (int): Seed for random number generation.
+            ignore_eos (bool): Indicates whether to ignore end-of-sequence tokens.
+            echo: bool = False,
+            logprobs: int = None,
+            logit_bias: Dict[str, float] = None,
+            logit_bias_type:Literal["input_ids", "tokens"] = None
+            cache_prompt: bool = False,
+            samplers: List[str] = None
+        Returns:
+            list[dict]|str: The generated chat response.
+        """
+        if function_tool_registry is None and do_not_use_grammar is False:
+            if self.function_tool_registry is not None:
+                function_tool_registry = self.function_tool_registry
+        completion, response_role = await self.async_get_response_role_and_completion(
+            function_tool_registry=function_tool_registry,
+            system_prompt=system_prompt,
+            message=message,
+            add_message_to_chat_history=add_message_to_chat_history,
+            role=role,
+            response_role=response_role,
+            grammar=grammar,
+            prompt_suffix=prompt_suffix,
+            max_tokens=max_tokens,
+            temperature=temperature,
+            top_k=top_k,
+            top_p=top_p,
+            min_p=min_p,
+            typical_p=typical_p,
+            repeat_penalty=repeat_penalty,
+            mirostat_mode=mirostat_mode,
+            mirostat_tau=mirostat_tau,
+            mirostat_eta=mirostat_eta,
+            tfs_z=tfs_z,
+            stop_sequences=stop_sequences,
+            additional_stop_sequences=additional_stop_sequences,
+            stream=stream,
+            k_last_messages=k_last_messages,
+            n_predict=n_predict,
+            n_keep=n_keep,
+            repeat_last_n=repeat_last_n,
+            penalize_nl=penalize_nl,
+            presence_penalty=presence_penalty,
+            frequency_penalty=frequency_penalty,
+            penalty_prompt=penalty_prompt,
+            seed=seed,
+            ignore_eos=ignore_eos,
+            echo=echo,
+            logprobs=logprobs,
+            logit_bias=logit_bias,
+            logit_bias_type=logit_bias_type,
+            cache_prompt=cache_prompt,
+            samplers=samplers,
+        )
+        if self.model:
+            if stream:
+                full_response = ""
+                async for out in completion:
+                    text = out["choices"][0]["text"]
+                    full_response += text
+                    if streaming_callback is not None:
+                        streaming_callback(
+                            StreamingResponse(text=text, is_last_response=False)
+                        )
+                    if print_output:
+                        print(text, end="")
+                if streaming_callback is not None:
+                    streaming_callback(
+                        StreamingResponse(text="", is_last_response=True)
+                    )
+                if print_output:
+                    print("")
+
+                self.last_response = full_response
+                if add_response_to_chat_history:
+                    self.messages.append(
+                        {
+                            "role": response_role,
+                            "content": full_response,
+                        },
+                    )
+                if function_tool_registry is not None:
+                    full_response = function_tool_registry.handle_function_call(
+                        full_response
+                    )
+                    return full_response if full_response else None
+                return full_response if full_response else None
+            else:
+                text = completion["choices"][0]["text"]
+                if print_output:
+                    print(text)
+                self.last_response = text
+                if add_response_to_chat_history:
+                    self.messages.append(
+                        {
+                            "role": response_role,
+                            "content": text,
+                        },
+                    )
+                if function_tool_registry is not None:
+                    text = function_tool_registry.handle_function_call(text)
+                    return text if text else None
+                return text if text else None
+        return "Error: No model loaded!"
+
+    async def async_get_text_completion(
+        self,
+        prompt: str | list[int] = None,
+        grammar: str = None,
+        max_tokens: int = 0,
+        temperature: float = 0.4,
+        top_k: int = 0,
+        top_p: float = 1.0,
+        min_p: float = 0.05,
+        typical_p: float = 1.0,
+        repeat_penalty: float = 1.0,
+        mirostat_mode: int = 0,
+        mirostat_tau: float = 5.0,
+        mirostat_eta: float = 0.1,
+        tfs_z: float = 1.0,
+        stream: bool = False,
+        # Llama Cpp Server and Open AI endpoint settings
+        n_predict: int = -1,
+        n_keep: int = 0,
+        repeat_last_n: int = 64,
+        penalize_nl: bool = True,
+        presence_penalty: float = 0.0,
+        frequency_penalty: float = 0.0,
+        penalty_prompt: Union[None, str, List[int]] = None,
+        seed: int = -1,
+        ignore_eos: bool = False,
+        echo: bool = False,
+        logprobs: int = None,
+        logit_bias: Dict[str, float] = None,
+        logit_bias_type: Literal["input_ids", "tokens"] = None,
+        samplers: List[str] = None,
+        stop_sequences: List[str] = None,
+    ):
+        if isinstance(self.model, LlamaCppEndpointSettings):
+            completion = await self.model.async_create_completion(
+                prompt=prompt,
+                grammar=grammar,
+                generation_settings=LlamaCppGenerationSettings(
+                    temperature=temperature,
+                    top_k=top_k,
+                    top_p=top_p,
+                    min_p=min_p,
+                    n_predict=n_predict,
+                    n_keep=n_keep,
+                    stream=stream,
+                    stop_sequences=stop_sequences,
+                    tfs_z=tfs_z,
+                    typical_p=typical_p,
+                    repeat_penalty=repeat_penalty,
+                    repeat_last_n=repeat_last_n,
+                    penalize_nl=penalize_nl,
+                    presence_penalty=presence_penalty,
+                    frequency_penalty=frequency_penalty,
+                    penalty_prompt=penalty_prompt,
+                    mirostat_mode=mirostat_mode,
+                    mirostat_tau=mirostat_tau,
+                    mirostat_eta=mirostat_eta,
+                    seed=seed,
+                    samplers=samplers,
+                    ignore_eos=ignore_eos,
+                ),
+            )
+        elif isinstance(self.model, OpenAIEndpointSettings):
+            completion = await self.model.async_create_completion(
+                prompt=prompt,
+                grammar=grammar,
+                generation_settings=OpenAIGenerationSettings(
+                    temperature=temperature,
+                    top_k=top_k,
+                    top_p=top_p,
+                    min_p=min_p,
+                    stream=stream,
+                    stop_sequences=stop_sequences,
+                    echo=echo,
+                    repeat_penalty=repeat_penalty,
+                    logprobs=logprobs,
+                    presence_penalty=presence_penalty,
+                    frequency_penalty=frequency_penalty,
+                    logit_bias=logit_bias,
+                    logit_bias_type=logit_bias_type,
+                    mirostat_mode=mirostat_mode,
+                    mirostat_tau=mirostat_tau,
+                    mirostat_eta=mirostat_eta,
+                    seed=seed,
+                ),
+            )
+        else:
+            if isinstance(grammar, str):
+                if grammar in self.grammar_cache:
+                    grammar = self.grammar_cache[grammar]
+                else:
+                    grammar_string = grammar
+                    grammar = LlamaGrammar.from_string(grammar, False)
+                    self.grammar_cache[grammar_string] = grammar
+            completion = self.model.create_completion(
+                prompt=prompt,
+                max_tokens=max_tokens,
+                stream=stream,
+                stop=stop_sequences,
+                temperature=temperature,
+                top_k=top_k,
+                top_p=top_p,
+                min_p=min_p,
+                typical_p=typical_p,
+                mirostat_mode=mirostat_mode,
+                mirostat_tau=mirostat_tau,
+                mirostat_eta=mirostat_eta,
+                tfs_z=tfs_z,
+                repeat_penalty=repeat_penalty,
+                grammar=grammar,
+            )
+        return completion
+
+    async def async_get_response_role_and_completion(
+        self,
+        function_tool_registry: LlamaCppFunctionToolRegistry = None,
+        system_prompt: str = None,
+        message: str = None,
+        add_message_to_chat_history: bool = True,
+        role: Literal["system", "user", "assistant", "function"] = "user",
+        response_role: Literal["user", "assistant"] | None = None,
+        grammar: str = None,
+        prompt_suffix: str = None,
+        max_tokens: int = 0,
+        temperature: float = 0.4,
+        top_k: int = 0,
+        top_p: float = 1.0,
+        min_p: float = 0.05,
+        typical_p: float = 1.0,
+        repeat_penalty: float = 1.0,
+        mirostat_mode: int = 0,
+        mirostat_tau: float = 5.0,
+        mirostat_eta: float = 0.1,
+        tfs_z: float = 1.0,
+        stop_sequences: List[str] = None,
+        additional_stop_sequences: List[str] = None,
+        stream: bool = True,
+        k_last_messages: int = 0,
+        n_predict: int = -1,
+        n_keep: int = 0,
+        repeat_last_n: int = 64,
+        penalize_nl: bool = True,
+        presence_penalty: float = 0.0,
+        frequency_penalty: float = 0.0,
+        penalty_prompt: Union[None, str, List[int]] = None,
+        seed: int = -1,
+        ignore_eos: bool = False,
+        echo: bool = False,
+        logprobs: int = None,
+        logit_bias: Dict[str, float] = None,
+        logit_bias_type: Literal["input_ids", "tokens"] = None,
+        cache_prompt: bool = False,
+        samplers: List[str] = None,
+    ):
+        if function_tool_registry is not None:
+            grammar = function_tool_registry.gbnf_grammar
+
+        if system_prompt is None:
+            system_prompt = self.system_prompt
+        messages = [
+            {
+                "role": "system",
+                "content": system_prompt,
+            },
+        ]
+        if message is not None and add_message_to_chat_history:
+            self.messages.append(
+                {
+                    "role": role,
+                    "content": message,
+                },
+            )
+        if not add_message_to_chat_history and message is not None:
+            messages.append(
+                {
+                    "role": role,
+                    "content": message,
+                },
+            )
+        if k_last_messages > 0:
+            messages.extend(self.messages[-k_last_messages:])
+        else:
+            messages.extend(self.messages)
+
+        prompt, response_role = self.messages_formatter.format_messages(
+            messages, response_role
+        )
+
+        if prompt_suffix:
+            prompt += prompt_suffix
+
+        if self.debug_output:
+            print(prompt, end="")
+
+        if stop_sequences is None:
+            stop_sequences = self.messages_formatter.DEFAULT_STOP_SEQUENCES
+
+        if additional_stop_sequences is not None:
+            stop_sequences.extend(additional_stop_sequences)
+
+        if self.model:
+            if isinstance(self.model, LlamaCppEndpointSettings):
+                completion = await self.model.async_create_completion(
+                    prompt=prompt,
+                    grammar=grammar,
+                    generation_settings=LlamaCppGenerationSettings(
+                        temperature=temperature,
+                        top_k=top_k,
+                        top_p=top_p,
+                        min_p=min_p,
+                        n_predict=n_predict,
+                        n_keep=n_keep,
+                        stream=stream,
+                        stop_sequences=stop_sequences,
+                        tfs_z=tfs_z,
+                        typical_p=typical_p,
+                        repeat_penalty=repeat_penalty,
+                        repeat_last_n=repeat_last_n,
+                        penalize_nl=penalize_nl,
+                        presence_penalty=presence_penalty,
+                        frequency_penalty=frequency_penalty,
+                        penalty_prompt=penalty_prompt,
+                        mirostat_mode=mirostat_mode,
+                        mirostat_tau=mirostat_tau,
+                        mirostat_eta=mirostat_eta,
+                        samplers=samplers,
+                        seed=seed,
+                        cache_prompt=cache_prompt,
+                        ignore_eos=ignore_eos,
+                    ),
+                )
+            elif isinstance(self.model, OpenAIEndpointSettings):
+                completion = await self.model.async_create_completion(
+                    prompt=prompt,
+                    grammar=grammar,
+                    generation_settings=OpenAIGenerationSettings(
+                        temperature=temperature,
+                        top_k=top_k,
+                        top_p=top_p,
+                        min_p=min_p,
+                        stream=stream,
+                        stop_sequences=stop_sequences,
+                        echo=echo,
+                        repeat_penalty=repeat_penalty,
+                        logprobs=logprobs,
+                        presence_penalty=presence_penalty,
+                        frequency_penalty=frequency_penalty,
+                        logit_bias=logit_bias,
+                        logit_bias_type=logit_bias_type,
+                        mirostat_mode=mirostat_mode,
+                        mirostat_tau=mirostat_tau,
+                        mirostat_eta=mirostat_eta,
+                        seed=seed,
+                    ),
+                )
+            else:
+                if isinstance(grammar, str):
+                    if grammar in self.grammar_cache:
+                        grammar = self.grammar_cache[grammar]
+                    else:
+                        grammar_string = grammar
+                        grammar = LlamaGrammar.from_string(grammar, False)
+                        self.grammar_cache[grammar_string] = grammar
+                completion = self.model.create_completion(
+                    prompt=prompt,
+                    max_tokens=max_tokens,
+                    stream=stream,
+                    stop=stop_sequences,
+                    temperature=temperature,
+                    top_k=top_k,
+                    top_p=top_p,
+                    min_p=min_p,
+                    typical_p=typical_p,
+                    mirostat_mode=mirostat_mode,
+                    mirostat_tau=mirostat_tau,
+                    mirostat_eta=mirostat_eta,
+                    tfs_z=tfs_z,
+                    repeat_penalty=repeat_penalty,
+                    grammar=grammar,
+                )
+            return completion, response_role
+        return "Error: No model loaded!"
+
+    def remove_last_k_chat_messages(self, k: int):
+        """
+        Removes the last k messages from the chat history.
+
+        Args:
+            k (int): Number of last messages to remove.
+        """
+        # Ensure k is not greater than the length of the messages list
+        k = min(k, len(self.messages))
+
+        # Remove the last k elements
+        self.messages = self.messages[:-k] if k > 0 else self.messages
+
+    def remove_first_k_chat_messages(self, k: int):
+        """
+        Removes the first k messages from the chat history.
+
+        Args:
+            k (int): Number of first messages to remove.
+        """
+        # Ensure k is not greater than the length of the messages list
+        k = min(k, len(self.messages))
+
+        # Remove the first k elements
+        self.messages = self.messages[k:] if k > 0 else self.messages
+
+    def save_messages(self, file_path: str):
+        """
+        Saves the chat history messages to a file.
+
+        Args:
+           file_path (str): The file path to save the messages.
+        """
+        with open(file_path, "w", encoding="utf-8") as file:
+            json.dump(self.messages, file, indent=4)
+
+    def load_messages(self, file_path: str):
+        """
+        Loads chat history messages from a file.
+
+        Args:
+            file_path (str): The file path to load the messages from.
+        """
+        with open(file_path, "r", encoding="utf-8") as file:
+            loaded_messages = json.load(file)
+            self.messages.extend(loaded_messages)
+
+    @staticmethod
+    def agent_conversation(
+        agent_1: "LlamaCppAgent",
+        agent_2: "LlamaCppAgent",
+        agent_1_initial_message: str,
+        number_of_exchanges: int = 15,
+    ):
+        current_message = agent_1_initial_message
+        current_agent, next_agent = agent_2, agent_1
+
+        for _ in range(number_of_exchanges):
+            # Current agent responds to the last message
+            response = current_agent.get_chat_response(
+                message=current_message,
+                role="user",
+                add_response_to_chat_history=True,
+                print_output=True,
+                top_p=0.8,
+                top_k=40,
+            )
+
+            # Update the message for the next turn
+            current_message = response
+
+            # Swap the agents for the next turn
+            current_agent, next_agent = next_agent, current_agent
+
+        print("Conversation ended.")
+
+    @staticmethod
+    def group_conversation(
+        agent_list: list["LlamaCppAgent"],
+        initial_message: str,
+        number_of_turns: int = 4,
+    ):
+        responses = [
+            {
+                "role": "user",
+                "content": initial_message,
+            }
+        ]
+        for _ in range(number_of_turns):
+            for a in agent_list:
+                a.messages = copy(responses)
+                for response in a.messages:
+                    if response["content"].strip().startswith(a.name):
+                        response["role"] = "assistant"
+                response = a.get_chat_response(
+                    add_response_to_chat_history=False,
+                    add_message_to_chat_history=False,
+                    prompt_suffix=f"\n{a.name}:",
+                )
+                response = f"{a.name}:{response[0]}"
+                responses.append(
+                    {
+                        "role": "user",
+                        "content": response,
+                    }
+                )
+        print("Conversation ended.")
```

### Comparing `llama_cpp_agent-0.1.3/src/llama_cpp_agent/llm_prompt_template.py` & `llama_cpp_agent-0.1.4/src/llama_cpp_agent/llm_prompt_template.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,199 +1,199 @@
-import re
-from dataclasses import dataclass
-from typing import List, Dict, Union
-
-
-@dataclass
-class PromptTemplateField:
-    """
-    Data class representing a field in a prompt template.
-
-    Attributes:
-        name (str): The name of the template field.
-        value (str): The value associated with the template field.
-    """
-
-    name: str
-    value: str
-
-
-class PromptTemplateFields:
-    """
-    Class representing a collection of PromptTemplateField objects.
-
-    Methods:
-        add_field(name: str, value: str): Add a new field to the collection.
-        remove_field(name: str): Remove a field by name from the collection.
-        edit_field(name: str, new_value: str): Edit the value of an existing field.
-        find_field(name: str) -> PromptTemplateField: Find and return a field by name.
-        list_fields() -> List[PromptTemplateField]: Get a list of all fields in the collection.
-        get_fields_dict() -> Dict[str, str]: Get a dictionary representation of the fields.
-        set_fields_from_dict(field_dict: Dict[str, str]): Set the fields using a dictionary.
-
-    Attributes:
-        fields (List[PromptTemplateField]): List of PromptTemplateField objects.
-    """
-
-    def __init__(self):
-        self.fields: List[PromptTemplateField] = []
-
-    def add_field(self, name: str, value: str):
-        """Add a new field to the collection."""
-        self.fields.append(PromptTemplateField(name, value))
-
-    def remove_field(self, name: str):
-        """Remove a field by name from the collection."""
-        self.fields = [field for field in self.fields if field.name != name]
-
-    def edit_field(self, name: str, new_value: str):
-        """Edit the value of an existing field."""
-        field = self.find_field(name)
-        if field:
-            field.value = new_value
-        else:
-            raise ValueError(f"Field '{name}' not found.")
-
-    def find_field(self, name: str) -> PromptTemplateField:
-        """Find and return a field by name."""
-        for field in self.fields:
-            if field.name == name:
-                return field
-        return None
-
-    def list_fields(self):
-        """Get a list of all fields in the collection."""
-        return self.fields
-
-    def get_fields_dict(self) -> Dict[str, str]:
-        """Get a dictionary representation of the fields."""
-        return {field.name: field.value for field in self.fields}
-
-    def set_fields_from_dict(self, field_dict: Dict[str, str]):
-        """Set the fields using a dictionary."""
-        self.fields.clear()
-        for name, value in field_dict.items():
-            self.add_field(name, value)
-
-
-class PromptTemplate:
-    """
-    Class representing a prompt template.
-
-    Methods:
-        generate_prompt(template_fields: Union[dict, PromptTemplateFields], remove_empty_template_field=True) -> str:
-        Generate a prompt by replacing placeholders in the template with values.
-
-    Class Methods:
-        from_string(template_string: str) -> PromptTemplate:
-        Create a PromptTemplate from a string.
-        from_file(template_file: str) -> PromptTemplate:
-        Create a PromptTemplate from a file.
-
-    Attributes:
-        template (str): The template string containing placeholders.
-    """
-
-    def __init__(self, template_file=None, template_string=None):
-        """
-        Initialize a PromptTemplate instance.
-
-        Args:
-            template_file (str): The path to a file containing the template.
-            template_string (str): The template string.
-        """
-        if template_file:
-            with open(template_file, "r") as file:
-                self.template = file.read()
-        elif template_string:
-            self.template = template_string
-        else:
-            raise ValueError(
-                "Either 'template_file' or 'template_string' must be provided"
-            )
-
-    @classmethod
-    def from_string(cls, template_string):
-        """
-        Create a PromptTemplate instance from a string.
-
-        Args:
-            template_string (str): The template string.
-
-        Returns:
-            PromptTemplate: Created PromptTemplate instance.
-        """
-        return cls(template_string=template_string)
-
-    @classmethod
-    def from_file(cls, template_file):
-        """
-        Create a PromptTemplate instance from a file.
-
-        Args:
-            template_file (str): The path to a file containing the template.
-
-        Returns:
-            PromptTemplate: Created PromptTemplate instance.
-        """
-        with open(template_file, "r") as file:
-            template_string = file.read()
-        return cls(template_string=template_string)
-
-    def _remove_empty_placeholders(self, text):
-        """
-        Remove lines that contain only the empty placeholder.
-
-        Args:
-            text (str): The text containing placeholders.
-
-        Returns:
-            str: Text with empty placeholders removed.
-        """
-        # Remove lines that contain only the empty placeholder
-        text = re.sub(rf'^{"__EMPTY_TEMPLATE_FIELD__"}$', "", text, flags=re.MULTILINE)
-        # Remove the empty placeholder from lines with other content
-        text = re.sub(rf'{"__EMPTY_TEMPLATE_FIELD__"}', "", text)
-        return text
-
-    def generate_prompt(
-        self,
-        template_fields: Union[dict, PromptTemplateFields],
-        remove_empty_template_field=True,
-    ) -> str:
-        """
-        Generate a prompt by replacing placeholders in the template with values.
-
-        Args:
-            template_fields (Union[dict, PromptTemplateFields]): The template fields.
-            remove_empty_template_field (bool): If True, removes lines with empty placeholders.
-
-        Returns:
-            str: The generated prompt.
-        """
-        cleaned_fields = {}
-        for key, value in template_fields.items():
-            cleaned_fields[key] = str(value) if not isinstance(value, str) else value
-
-        template_fields = cleaned_fields
-        if isinstance(template_fields, PromptTemplateFields):
-            template_fields = template_fields.get_fields_dict()
-
-        if not remove_empty_template_field:
-
-            def replace_placeholder(match):
-                placeholder = match.group(1)
-                return template_fields.get(placeholder, match.group(0))
-
-            prompt = re.sub(r"\{(\w+)\}", replace_placeholder, self.template)
-            return prompt
-
-        def replace_placeholder(match):
-            placeholder = match.group(1)
-            if template_fields.get(placeholder, match.group(0)) != "":
-                return template_fields.get(placeholder, match.group(0))
-            return "__EMPTY_TEMPLATE_FIELD__"
-
-        # Initial placeholder replacement
-        prompt = re.sub(r"\{(\w+)\}", replace_placeholder, self.template)
-
-        return self._remove_empty_placeholders(prompt)
+import re
+from dataclasses import dataclass
+from typing import List, Dict, Union
+
+
+@dataclass
+class PromptTemplateField:
+    """
+    Data class representing a field in a prompt template.
+
+    Attributes:
+        name (str): The name of the template field.
+        value (str): The value associated with the template field.
+    """
+
+    name: str
+    value: str
+
+
+class PromptTemplateFields:
+    """
+    Class representing a collection of PromptTemplateField objects.
+
+    Methods:
+        add_field(name: str, value: str): Add a new field to the collection.
+        remove_field(name: str): Remove a field by name from the collection.
+        edit_field(name: str, new_value: str): Edit the value of an existing field.
+        find_field(name: str) -> PromptTemplateField: Find and return a field by name.
+        list_fields() -> List[PromptTemplateField]: Get a list of all fields in the collection.
+        get_fields_dict() -> Dict[str, str]: Get a dictionary representation of the fields.
+        set_fields_from_dict(field_dict: Dict[str, str]): Set the fields using a dictionary.
+
+    Attributes:
+        fields (List[PromptTemplateField]): List of PromptTemplateField objects.
+    """
+
+    def __init__(self):
+        self.fields: List[PromptTemplateField] = []
+
+    def add_field(self, name: str, value: str):
+        """Add a new field to the collection."""
+        self.fields.append(PromptTemplateField(name, value))
+
+    def remove_field(self, name: str):
+        """Remove a field by name from the collection."""
+        self.fields = [field for field in self.fields if field.name != name]
+
+    def edit_field(self, name: str, new_value: str):
+        """Edit the value of an existing field."""
+        field = self.find_field(name)
+        if field:
+            field.value = new_value
+        else:
+            raise ValueError(f"Field '{name}' not found.")
+
+    def find_field(self, name: str) -> PromptTemplateField:
+        """Find and return a field by name."""
+        for field in self.fields:
+            if field.name == name:
+                return field
+        return None
+
+    def list_fields(self):
+        """Get a list of all fields in the collection."""
+        return self.fields
+
+    def get_fields_dict(self) -> Dict[str, str]:
+        """Get a dictionary representation of the fields."""
+        return {field.name: field.value for field in self.fields}
+
+    def set_fields_from_dict(self, field_dict: Dict[str, str]):
+        """Set the fields using a dictionary."""
+        self.fields.clear()
+        for name, value in field_dict.items():
+            self.add_field(name, value)
+
+
+class PromptTemplate:
+    """
+    Class representing a prompt template.
+
+    Methods:
+        generate_prompt(template_fields: Union[dict, PromptTemplateFields], remove_empty_template_field=True) -> str:
+        Generate a prompt by replacing placeholders in the template with values.
+
+    Class Methods:
+        from_string(template_string: str) -> PromptTemplate:
+        Create a PromptTemplate from a string.
+        from_file(template_file: str) -> PromptTemplate:
+        Create a PromptTemplate from a file.
+
+    Attributes:
+        template (str): The template string containing placeholders.
+    """
+
+    def __init__(self, template_file=None, template_string=None):
+        """
+        Initialize a PromptTemplate instance.
+
+        Args:
+            template_file (str): The path to a file containing the template.
+            template_string (str): The template string.
+        """
+        if template_file:
+            with open(template_file, "r") as file:
+                self.template = file.read()
+        elif template_string:
+            self.template = template_string
+        else:
+            raise ValueError(
+                "Either 'template_file' or 'template_string' must be provided"
+            )
+
+    @classmethod
+    def from_string(cls, template_string):
+        """
+        Create a PromptTemplate instance from a string.
+
+        Args:
+            template_string (str): The template string.
+
+        Returns:
+            PromptTemplate: Created PromptTemplate instance.
+        """
+        return cls(template_string=template_string)
+
+    @classmethod
+    def from_file(cls, template_file):
+        """
+        Create a PromptTemplate instance from a file.
+
+        Args:
+            template_file (str): The path to a file containing the template.
+
+        Returns:
+            PromptTemplate: Created PromptTemplate instance.
+        """
+        with open(template_file, "r") as file:
+            template_string = file.read()
+        return cls(template_string=template_string)
+
+    def _remove_empty_placeholders(self, text):
+        """
+        Remove lines that contain only the empty placeholder.
+
+        Args:
+            text (str): The text containing placeholders.
+
+        Returns:
+            str: Text with empty placeholders removed.
+        """
+        # Remove lines that contain only the empty placeholder
+        text = re.sub(rf'^{"__EMPTY_TEMPLATE_FIELD__"}$', "", text, flags=re.MULTILINE)
+        # Remove the empty placeholder from lines with other content
+        text = re.sub(rf'{"__EMPTY_TEMPLATE_FIELD__"}', "", text)
+        return text
+
+    def generate_prompt(
+        self,
+        template_fields: Union[dict, PromptTemplateFields],
+        remove_empty_template_field=True,
+    ) -> str:
+        """
+        Generate a prompt by replacing placeholders in the template with values.
+
+        Args:
+            template_fields (Union[dict, PromptTemplateFields]): The template fields.
+            remove_empty_template_field (bool): If True, removes lines with empty placeholders.
+
+        Returns:
+            str: The generated prompt.
+        """
+        cleaned_fields = {}
+        for key, value in template_fields.items():
+            cleaned_fields[key] = str(value) if not isinstance(value, str) else value
+
+        template_fields = cleaned_fields
+        if isinstance(template_fields, PromptTemplateFields):
+            template_fields = template_fields.get_fields_dict()
+
+        if not remove_empty_template_field:
+
+            def replace_placeholder(match):
+                placeholder = match.group(1)
+                return template_fields.get(placeholder, match.group(0))
+
+            prompt = re.sub(r"\{(\w+)\}", replace_placeholder, self.template)
+            return prompt
+
+        def replace_placeholder(match):
+            placeholder = match.group(1)
+            if template_fields.get(placeholder, match.group(0)) != "":
+                return template_fields.get(placeholder, match.group(0))
+            return "__EMPTY_TEMPLATE_FIELD__"
+
+        # Initial placeholder replacement
+        prompt = re.sub(r"\{(\w+)\}", replace_placeholder, self.template)
+
+        return self._remove_empty_placeholders(prompt)
```

### Comparing `llama_cpp_agent-0.1.3/src/llama_cpp_agent/llm_settings.py` & `llama_cpp_agent-0.1.4/src/llama_cpp_agent/llm_settings.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,169 +1,169 @@
-import json
-from dataclasses import dataclass
-from typing import List
-
-
-@dataclass
-class LlamaLLMGenerationSettings:
-    """
-    Data class representing generation settings for the Llama language model.
-
-    Attributes:
-        max_tokens (int): The maximum number of tokens to generate.
-        temperature (float): Controls the randomness of the generated output (higher values increase randomness).
-        top_k (int): Controls the diversity of the generated output by limiting the top-k tokens considered.
-        top_p (float): Controls the diversity of the generated output by limiting the cumulative probability of tokens.
-        min_p (float): Minimum probability threshold for token selection.
-        typical_p (float): Typical probability used for token selection.
-        repeat_penalty (float): Penalty for repeating the same token in the output.
-        mirostat_mode (int): Mode for using Mirostat, if enabled.
-        mirostat_tau (float): Mirostat hyperparameter tau.
-        mirostat_eta (float): Mirostat hyperparameter eta.
-        tfs_z (float): TFS Z hyperparameter.
-        stop_sequences (List[str]): List of stop sequences to indicate the end of generation.
-        stream (bool): If True, generates output as a stream (partial responses); if False, generates complete responses.
-        print_output (bool): If True, prints the generated output.
-    """
-
-    max_tokens: int = 0
-    temperature: float = 0.35
-    top_k: int = 0
-    top_p: float = 1.0
-    min_p: float = 0.05
-    typical_p: float = 1.0
-    repeat_penalty: float = 1.0
-    mirostat_mode: int = 0
-    mirostat_tau: float = 5.0
-    mirostat_eta: float = 0.1
-    tfs_z: float = 1.0
-    stop_sequences: List[str] = None
-    stream: bool = True
-    print_output: bool = True
-
-    def save(self, file_path: str):
-        """
-        Save the LlamaLLMGenerationSettings object to a JSON file.
-
-        Args:
-            file_path (str): The path to the JSON file.
-        """
-        with open(file_path, "w", encoding="utf-8") as file:
-            json.dump(self.as_dict(), file, indent=4)
-
-    @staticmethod
-    def load_from_file(file_path: str) -> "LlamaLLMGenerationSettings":
-        """
-        Load LlamaLLMGenerationSettings from a JSON file.
-
-        Args:
-            file_path (str): The path to the JSON file.
-
-        Returns:
-            LlamaLLMGenerationSettings: Loaded LlamaLLMGenerationSettings object.
-        """
-        with open(file_path, "r", encoding="utf-8") as file:
-            loaded_settings = json.load(file)
-            return LlamaLLMGenerationSettings(**loaded_settings)
-
-    @staticmethod
-    def load_from_dict(settings: dict) -> "LlamaLLMGenerationSettings":
-        """
-        Create LlamaLLMGenerationSettings from a dictionary.
-
-        Args:
-            settings (dict): Dictionary containing LlamaLLMGenerationSettings attributes.
-
-        Returns:
-            LlamaLLMGenerationSettings: Created LlamaLLMGenerationSettings object.
-        """
-        return LlamaLLMGenerationSettings(**settings)
-
-    def as_dict(self) -> dict:
-        """
-        Convert LlamaLLMGenerationSettings to a dictionary.
-
-        Returns:
-            dict: Dictionary representation of the object.
-        """
-        return self.__dict__
-
-
-@dataclass
-class LlamaLLMSettings:
-    """
-    Data class representing settings for the Llama language model.
-
-    Attributes:
-        model_path (str): The path to the Llama language model.
-        n_gpu_layers (int): Number of GPU layers.
-        f16_kv (bool): If True, uses float16 for key and value tensors in self-attention layers.
-        offload_kqv (bool): If True, offloads key, query, and value tensors to CPU in self-attention layers.
-        use_mlock (bool): If True, uses mlock to lock model weights in RAM.
-        embedding (bool): If True, enables ability to get embeddings from the model.
-        n_threads (int): Number of threads to use (None for automatic).
-        n_batch (int): Batch size.
-        n_ctx (int): Context size.
-        last_n_tokens_size (int): Size of the buffer for last n tokens.
-        verbose (bool): If True, enables verbose mode.
-        seed (int): Random seed for reproducibility.
-    """
-
-    model_path: str
-    n_gpu_layers: int = 0
-    f16_kv: bool = True
-    offload_kqv: bool = True
-    use_mlock: bool = False
-    embedding: bool = False
-    n_threads: int = None
-    n_batch: int = 512
-    n_ctx: int = 512
-    last_n_tokens_size: int = 64
-    verbose: bool = False
-    seed: int = -1
-
-    def save(self, file_path: str):
-        """
-        Save the LlamaLLMSettings object to a JSON file.
-
-        Args:
-            file_path (str): The path to the JSON file.
-        """
-        with open(file_path, "w", encoding="utf-8") as file:
-            json.dump(self.as_dict(), file, indent=4)
-
-    @staticmethod
-    def load_from_file(file_path: str) -> "LlamaLLMSettings":
-        """
-        Load LlamaLLMSettings from a JSON file.
-
-        Args:
-            file_path (str): The path to the JSON file.
-
-        Returns:
-            LlamaLLMSettings: Loaded LlamaLLMSettings object.
-        """
-        with open(file_path, "r", encoding="utf-8") as file:
-            loaded_settings = json.load(file)
-            return LlamaLLMSettings(**loaded_settings)
-
-    @staticmethod
-    def load_from_dict(settings: dict) -> "LlamaLLMSettings":
-        """
-        Create LlamaLLMSettings from a dictionary.
-
-        Args:
-            settings (dict): Dictionary containing LlamaLLMSettings attributes.
-
-        Returns:
-            LlamaLLMSettings: Created LlamaLLMSettings object.
-        """
-        return LlamaLLMSettings(**settings)
-
-    def as_dict(self) -> dict:
-        """
-        Convert LlamaLLMSettings to a dictionary.
-
-        Returns:
-            dict: Dictionary representation of the object.
-        """
-        return self.__dict__
+import json
+from dataclasses import dataclass
+from typing import List
+
+
+@dataclass
+class LlamaLLMGenerationSettings:
+    """
+    Data class representing generation settings for the Llama language model.
+
+    Attributes:
+        max_tokens (int): The maximum number of tokens to generate.
+        temperature (float): Controls the randomness of the generated output (higher values increase randomness).
+        top_k (int): Controls the diversity of the generated output by limiting the top-k tokens considered.
+        top_p (float): Controls the diversity of the generated output by limiting the cumulative probability of tokens.
+        min_p (float): Minimum probability threshold for token selection.
+        typical_p (float): Typical probability used for token selection.
+        repeat_penalty (float): Penalty for repeating the same token in the output.
+        mirostat_mode (int): Mode for using Mirostat, if enabled.
+        mirostat_tau (float): Mirostat hyperparameter tau.
+        mirostat_eta (float): Mirostat hyperparameter eta.
+        tfs_z (float): TFS Z hyperparameter.
+        stop_sequences (List[str]): List of stop sequences to indicate the end of generation.
+        stream (bool): If True, generates output as a stream (partial responses); if False, generates complete responses.
+        print_output (bool): If True, prints the generated output.
+    """
+
+    max_tokens: int = 0
+    temperature: float = 0.35
+    top_k: int = 0
+    top_p: float = 1.0
+    min_p: float = 0.05
+    typical_p: float = 1.0
+    repeat_penalty: float = 1.0
+    mirostat_mode: int = 0
+    mirostat_tau: float = 5.0
+    mirostat_eta: float = 0.1
+    tfs_z: float = 1.0
+    stop_sequences: List[str] = None
+    stream: bool = True
+    print_output: bool = True
+
+    def save(self, file_path: str):
+        """
+        Save the LlamaLLMGenerationSettings object to a JSON file.
+
+        Args:
+            file_path (str): The path to the JSON file.
+        """
+        with open(file_path, "w", encoding="utf-8") as file:
+            json.dump(self.as_dict(), file, indent=4)
+
+    @staticmethod
+    def load_from_file(file_path: str) -> "LlamaLLMGenerationSettings":
+        """
+        Load LlamaLLMGenerationSettings from a JSON file.
+
+        Args:
+            file_path (str): The path to the JSON file.
+
+        Returns:
+            LlamaLLMGenerationSettings: Loaded LlamaLLMGenerationSettings object.
+        """
+        with open(file_path, "r", encoding="utf-8") as file:
+            loaded_settings = json.load(file)
+            return LlamaLLMGenerationSettings(**loaded_settings)
+
+    @staticmethod
+    def load_from_dict(settings: dict) -> "LlamaLLMGenerationSettings":
+        """
+        Create LlamaLLMGenerationSettings from a dictionary.
+
+        Args:
+            settings (dict): Dictionary containing LlamaLLMGenerationSettings attributes.
+
+        Returns:
+            LlamaLLMGenerationSettings: Created LlamaLLMGenerationSettings object.
+        """
+        return LlamaLLMGenerationSettings(**settings)
+
+    def as_dict(self) -> dict:
+        """
+        Convert LlamaLLMGenerationSettings to a dictionary.
+
+        Returns:
+            dict: Dictionary representation of the object.
+        """
+        return self.__dict__
+
+
+@dataclass
+class LlamaLLMSettings:
+    """
+    Data class representing settings for the Llama language model.
+
+    Attributes:
+        model_path (str): The path to the Llama language model.
+        n_gpu_layers (int): Number of GPU layers.
+        f16_kv (bool): If True, uses float16 for key and value tensors in self-attention layers.
+        offload_kqv (bool): If True, offloads key, query, and value tensors to CPU in self-attention layers.
+        use_mlock (bool): If True, uses mlock to lock model weights in RAM.
+        embedding (bool): If True, enables ability to get embeddings from the model.
+        n_threads (int): Number of threads to use (None for automatic).
+        n_batch (int): Batch size.
+        n_ctx (int): Context size.
+        last_n_tokens_size (int): Size of the buffer for last n tokens.
+        verbose (bool): If True, enables verbose mode.
+        seed (int): Random seed for reproducibility.
+    """
+
+    model_path: str
+    n_gpu_layers: int = 0
+    f16_kv: bool = True
+    offload_kqv: bool = True
+    use_mlock: bool = False
+    embedding: bool = False
+    n_threads: int = None
+    n_batch: int = 512
+    n_ctx: int = 512
+    last_n_tokens_size: int = 64
+    verbose: bool = False
+    seed: int = -1
+
+    def save(self, file_path: str):
+        """
+        Save the LlamaLLMSettings object to a JSON file.
+
+        Args:
+            file_path (str): The path to the JSON file.
+        """
+        with open(file_path, "w", encoding="utf-8") as file:
+            json.dump(self.as_dict(), file, indent=4)
+
+    @staticmethod
+    def load_from_file(file_path: str) -> "LlamaLLMSettings":
+        """
+        Load LlamaLLMSettings from a JSON file.
+
+        Args:
+            file_path (str): The path to the JSON file.
+
+        Returns:
+            LlamaLLMSettings: Loaded LlamaLLMSettings object.
+        """
+        with open(file_path, "r", encoding="utf-8") as file:
+            loaded_settings = json.load(file)
+            return LlamaLLMSettings(**loaded_settings)
+
+    @staticmethod
+    def load_from_dict(settings: dict) -> "LlamaLLMSettings":
+        """
+        Create LlamaLLMSettings from a dictionary.
+
+        Args:
+            settings (dict): Dictionary containing LlamaLLMSettings attributes.
+
+        Returns:
+            LlamaLLMSettings: Created LlamaLLMSettings object.
+        """
+        return LlamaLLMSettings(**settings)
+
+    def as_dict(self) -> dict:
+        """
+        Convert LlamaLLMSettings to a dictionary.
+
+        Returns:
+            dict: Dictionary representation of the object.
+        """
+        return self.__dict__
```

### Comparing `llama_cpp_agent-0.1.3/src/llama_cpp_agent/messages.py` & `llama_cpp_agent-0.1.4/src/llama_cpp_agent/messages.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,274 +1,274 @@
-import json
-import string
-from abc import ABC, abstractmethod
-from enum import Enum
-import random
-from typing import Literal, Union, List, Optional, Annotated, Dict, Any
-
-from pydantic import BaseModel, Field, parse_obj_as
-
-from llama_cpp_agent.providers.provider_base import LLMProviderBase
-
-
-def generate_id(length=9):
-    # Characters to use in the ID
-    characters = string.ascii_letters + string.digits
-    # Random choice of characters
-    return "".join(random.choice(characters) for _ in range(length))
-
-
-class ToolType(Enum):
-    function = "function"
-
-
-class FunctionCall(BaseModel):
-    name: str
-    arguments: str
-
-
-class ToolCall(BaseModel):
-    id: str
-    type: ToolType = ToolType.function
-    function: FunctionCall
-
-
-class Roles(Enum):
-    system = "system"
-    user = "user"
-    assistant = "assistant"
-    tool = "tool"
-
-
-class BaseMessage(BaseModel):
-    role: Literal[Roles.system, Roles.user, Roles.assistant, Roles.tool]
-
-
-class UserMessage(BaseMessage):
-    role: Literal[Roles.user] = Roles.user
-    content: str
-
-
-class SystemMessage(BaseMessage):
-    role: Literal[Roles.system] = Roles.system
-    content: str
-
-
-class AssistantMessage(BaseMessage):
-    role: Literal[Roles.assistant] = Roles.assistant
-    content: Optional[str] = None
-    tool_calls: Optional[List[ToolCall]] = None
-
-
-class ToolMessage(BaseMessage):
-    tool_call_id: str
-    role: Literal[Roles.tool] = Roles.tool
-    content: str
-
-
-ChatMessage = Annotated[
-    Union[SystemMessage, UserMessage, AssistantMessage, ToolMessage],
-    Field(discriminator="role"),
-]
-
-
-class ChatHistory(ABC):
-    @abstractmethod
-    def get_chat_messages(self):
-        pass
-
-
-class ChatMessageStore(ABC):
-
-    @abstractmethod
-    def add_message(self, message: ChatMessage):
-        pass
-
-    @abstractmethod
-    def add_user_message(self, message: str):
-        pass
-
-    @abstractmethod
-    def add_system_message(self, message: str):
-        pass
-
-    @abstractmethod
-    def remove_last_message(self):
-        pass
-
-    @abstractmethod
-    def remove_last_k_message(self, k: int):
-        pass
-
-    @abstractmethod
-    def pop_message(self, k: int) -> ChatMessage:
-        pass
-
-    @abstractmethod
-    def get_message(self, k: int) -> ChatMessage:
-        pass
-
-    @abstractmethod
-    def get_last_message(self) -> ChatMessage:
-        pass
-
-    @abstractmethod
-    def get_last_k_messages(self, k: int) -> List[ChatMessage]:
-        pass
-
-    @abstractmethod
-    def get_messages(self, k: int) -> List[ChatMessage]:
-        pass
-
-    @abstractmethod
-    def get_all_messages(self) -> List[ChatMessage]:
-        pass
-
-
-# Function to convert messages to list of dictionary format
-def convert_messages_to_list_of_dictionaries(
-    messages: List[ChatMessage],
-) -> List[Dict[str, str]]:
-    """
-    Converts a list of messages to a list of dictionaries.
-    Args:
-        messages (List[ChatMessage]): The list of messages.
-    Returns:
-        List[Dict[str, str]]: A list of dictionaries.
-    """
-    result = []
-    for message in messages:
-        # Determine the appropriate content to include
-        content = ""
-        if isinstance(message, AssistantMessage):
-            if message.content is not None:
-                content = message.content
-            elif message.tool_calls is not None:
-                if len(message.tool_calls) > 1:
-                    content = "Function Calls:\n"
-                    count = 1
-                    for tool_call in message.tool_calls:
-                        content += f"{count}. Function: {tool_call.function.name}\nArguments: {tool_call.function.arguments}\n"
-                        count += 1
-                else:
-                    content = f"Function Call:\nFunction: {message.tool_calls[0].function.name}\nArguments: {message.tool_calls[0].function.arguments}\n"
-        elif isinstance(message, ToolMessage):
-            content = f"Function Call Result:\nResult: {message.content}\n"
-        else:
-            content = f"{message.content}"
-        # Construct the dictionary for the current message
-        msg_dict = {"role": message.role.value, "content": content}
-        result.append(msg_dict)
-    return result
-
-
-class BasicChatMessageStore(ChatMessageStore):
-
-    def __init__(self, messages: List[ChatMessage] = None):
-        if messages is None:
-            messages = []
-        self.messages: List[ChatMessage] = messages
-
-    def add_message(self, message: ChatMessage):
-        self.messages.append(message)
-
-    def add_user_message(self, message: str):
-        self.messages.append(UserMessage(role=Roles.user, content=message))
-
-    def add_system_message(self, message: str):
-        self.messages.append(SystemMessage(role=Roles.system, content=message))
-
-    def remove_last_message(self):
-        self.messages = self.messages[:-1]
-
-    def remove_last_k_message(self, k: int):
-        self.messages = self.messages[:-k]
-
-    def pop_message(self, k: int) -> ChatMessage:
-        return self.messages.pop(k)
-
-    def get_message(self, k: int) -> ChatMessage:
-        return self.messages[k]
-
-    def get_last_message(self) -> ChatMessage:
-        return self.messages[-1]
-
-    def get_last_k_messages(self, k: int) -> List[ChatMessage]:
-        return self.messages[-k:]
-
-    def get_messages(self, k: int) -> List[ChatMessage]:
-        return self.messages[k:]
-
-    def get_all_messages(self) -> List[ChatMessage]:
-        return self.messages
-
-    def save_to_json(self, file_path: str):
-        # Convert messages to a list of dictionaries using pydantic's model_dump() method
-        messages_dict = [message.model_dump() for message in self.messages]
-        # Write the list of dictionaries to a JSON file
-        with open(file_path, "w") as file:
-            json.dump(messages_dict, file, indent=4)
-
-    def load_from_json(self, file_path: str):
-        # Read the list of dictionaries from a JSON file
-        with open(file_path, "r") as file:
-            messages_dict = json.load(file)
-        # Convert dictionaries back to ChatMessage instances
-        self.messages = [
-            parse_obj_as(ChatMessage, message) for message in messages_dict
-        ]
-
-
-class BasicChatHistoryStrategy(Enum):
-    last_k_messages: str = "last_k_messages"
-    last_k_tokens: str = "last_k_tokens"
-
-
-class BasicChatHistory(ChatHistory):
-    def __init__(
-        self,
-        chat_history_strategy: BasicChatHistoryStrategy = BasicChatHistoryStrategy.last_k_messages,
-        k: int = 10,
-        llm_provider: LLMProviderBase = None,
-        message_store: ChatMessageStore = None,
-    ):
-        if message_store is None:
-            message_store = BasicChatMessageStore()
-        self.message_store: ChatMessageStore = message_store
-        self.k = k
-        self.strategy = chat_history_strategy
-        self.llm_provider = llm_provider
-        if (
-            chat_history_strategy == BasicChatHistoryStrategy.last_k_tokens
-            and llm_provider is None
-        ):
-            raise Exception(
-                "Please pass a LLM provider to BasicChatHistory when using last k tokens as memory strategy!"
-            )
-
-    def get_chat_messages(self) -> List[Dict[str, str]]:
-        if self.strategy == BasicChatHistoryStrategy.last_k_messages:
-            return convert_messages_to_list_of_dictionaries(
-                self.message_store.get_last_k_messages(self.k)
-            )
-        elif self.strategy == BasicChatHistoryStrategy.last_k_tokens:
-            total_tokens = 0
-            selected_messages = []
-            converted_messages = convert_messages_to_list_of_dictionaries(
-                self.message_store.get_all_messages()
-            )
-            sys_message = None
-            if converted_messages[0]["role"] == "system":
-                sys_message = converted_messages.pop(0)
-            for message in reversed(converted_messages):
-                tokens = self.llm_provider.tokenize(message["content"])
-                total_tokens += len(tokens)
-                if total_tokens >= self.k:
-                    if len(selected_messages) == 0:
-                        selected_messages.append(message)
-                    break
-                else:
-                    selected_messages.append(message)
-            if sys_message is not None:
-                selected_messages.append(sys_message)
-            return list(reversed(selected_messages))
-        return []
+import json
+import string
+from abc import ABC, abstractmethod
+from enum import Enum
+import random
+from typing import Literal, Union, List, Optional, Annotated, Dict, Any
+
+from pydantic import BaseModel, Field, parse_obj_as
+
+from llama_cpp_agent.providers.provider_base import LLMProviderBase
+
+
+def generate_id(length=9):
+    # Characters to use in the ID
+    characters = string.ascii_letters + string.digits
+    # Random choice of characters
+    return "".join(random.choice(characters) for _ in range(length))
+
+
+class ToolType(Enum):
+    function = "function"
+
+
+class FunctionCall(BaseModel):
+    name: str
+    arguments: str
+
+
+class ToolCall(BaseModel):
+    id: str
+    type: ToolType = ToolType.function
+    function: FunctionCall
+
+
+class Roles(Enum):
+    system = "system"
+    user = "user"
+    assistant = "assistant"
+    tool = "tool"
+
+
+class BaseMessage(BaseModel):
+    role: Literal[Roles.system, Roles.user, Roles.assistant, Roles.tool]
+
+
+class UserMessage(BaseMessage):
+    role: Literal[Roles.user] = Roles.user
+    content: str
+
+
+class SystemMessage(BaseMessage):
+    role: Literal[Roles.system] = Roles.system
+    content: str
+
+
+class AssistantMessage(BaseMessage):
+    role: Literal[Roles.assistant] = Roles.assistant
+    content: Optional[str] = None
+    tool_calls: Optional[List[ToolCall]] = None
+
+
+class ToolMessage(BaseMessage):
+    tool_call_id: str
+    role: Literal[Roles.tool] = Roles.tool
+    content: str
+
+
+ChatMessage = Annotated[
+    Union[SystemMessage, UserMessage, AssistantMessage, ToolMessage],
+    Field(discriminator="role"),
+]
+
+
+class ChatHistory(ABC):
+    @abstractmethod
+    def get_chat_messages(self):
+        pass
+
+
+class ChatMessageStore(ABC):
+
+    @abstractmethod
+    def add_message(self, message: ChatMessage):
+        pass
+
+    @abstractmethod
+    def add_user_message(self, message: str):
+        pass
+
+    @abstractmethod
+    def add_system_message(self, message: str):
+        pass
+
+    @abstractmethod
+    def remove_last_message(self):
+        pass
+
+    @abstractmethod
+    def remove_last_k_message(self, k: int):
+        pass
+
+    @abstractmethod
+    def pop_message(self, k: int) -> ChatMessage:
+        pass
+
+    @abstractmethod
+    def get_message(self, k: int) -> ChatMessage:
+        pass
+
+    @abstractmethod
+    def get_last_message(self) -> ChatMessage:
+        pass
+
+    @abstractmethod
+    def get_last_k_messages(self, k: int) -> List[ChatMessage]:
+        pass
+
+    @abstractmethod
+    def get_messages(self, k: int) -> List[ChatMessage]:
+        pass
+
+    @abstractmethod
+    def get_all_messages(self) -> List[ChatMessage]:
+        pass
+
+
+# Function to convert messages to list of dictionary format
+def convert_messages_to_list_of_dictionaries(
+    messages: List[ChatMessage],
+) -> List[Dict[str, str]]:
+    """
+    Converts a list of messages to a list of dictionaries.
+    Args:
+        messages (List[ChatMessage]): The list of messages.
+    Returns:
+        List[Dict[str, str]]: A list of dictionaries.
+    """
+    result = []
+    for message in messages:
+        # Determine the appropriate content to include
+        content = ""
+        if isinstance(message, AssistantMessage):
+            if message.content is not None:
+                content = message.content
+            elif message.tool_calls is not None:
+                if len(message.tool_calls) > 1:
+                    content = "Function Calls:\n"
+                    count = 1
+                    for tool_call in message.tool_calls:
+                        content += f"{count}. Function: {tool_call.function.name}\nArguments: {tool_call.function.arguments}\n"
+                        count += 1
+                else:
+                    content = f"Function Call:\nFunction: {message.tool_calls[0].function.name}\nArguments: {message.tool_calls[0].function.arguments}\n"
+        elif isinstance(message, ToolMessage):
+            content = f"Function Call Result:\nResult: {message.content}\n"
+        else:
+            content = f"{message.content}"
+        # Construct the dictionary for the current message
+        msg_dict = {"role": message.role.value, "content": content}
+        result.append(msg_dict)
+    return result
+
+
+class BasicChatMessageStore(ChatMessageStore):
+
+    def __init__(self, messages: List[ChatMessage] = None):
+        if messages is None:
+            messages = []
+        self.messages: List[ChatMessage] = messages
+
+    def add_message(self, message: ChatMessage):
+        self.messages.append(message)
+
+    def add_user_message(self, message: str):
+        self.messages.append(UserMessage(role=Roles.user, content=message))
+
+    def add_system_message(self, message: str):
+        self.messages.append(SystemMessage(role=Roles.system, content=message))
+
+    def remove_last_message(self):
+        self.messages = self.messages[:-1]
+
+    def remove_last_k_message(self, k: int):
+        self.messages = self.messages[:-k]
+
+    def pop_message(self, k: int) -> ChatMessage:
+        return self.messages.pop(k)
+
+    def get_message(self, k: int) -> ChatMessage:
+        return self.messages[k]
+
+    def get_last_message(self) -> ChatMessage:
+        return self.messages[-1]
+
+    def get_last_k_messages(self, k: int) -> List[ChatMessage]:
+        return self.messages[-k:]
+
+    def get_messages(self, k: int) -> List[ChatMessage]:
+        return self.messages[k:]
+
+    def get_all_messages(self) -> List[ChatMessage]:
+        return self.messages
+
+    def save_to_json(self, file_path: str):
+        # Convert messages to a list of dictionaries using pydantic's model_dump() method
+        messages_dict = [message.model_dump() for message in self.messages]
+        # Write the list of dictionaries to a JSON file
+        with open(file_path, "w") as file:
+            json.dump(messages_dict, file, indent=4)
+
+    def load_from_json(self, file_path: str):
+        # Read the list of dictionaries from a JSON file
+        with open(file_path, "r") as file:
+            messages_dict = json.load(file)
+        # Convert dictionaries back to ChatMessage instances
+        self.messages = [
+            parse_obj_as(ChatMessage, message) for message in messages_dict
+        ]
+
+
+class BasicChatHistoryStrategy(Enum):
+    last_k_messages: str = "last_k_messages"
+    last_k_tokens: str = "last_k_tokens"
+
+
+class BasicChatHistory(ChatHistory):
+    def __init__(
+        self,
+        chat_history_strategy: BasicChatHistoryStrategy = BasicChatHistoryStrategy.last_k_messages,
+        k: int = 10,
+        llm_provider: LLMProviderBase = None,
+        message_store: ChatMessageStore = None,
+    ):
+        if message_store is None:
+            message_store = BasicChatMessageStore()
+        self.message_store: ChatMessageStore = message_store
+        self.k = k
+        self.strategy = chat_history_strategy
+        self.llm_provider = llm_provider
+        if (
+            chat_history_strategy == BasicChatHistoryStrategy.last_k_tokens
+            and llm_provider is None
+        ):
+            raise Exception(
+                "Please pass a LLM provider to BasicChatHistory when using last k tokens as memory strategy!"
+            )
+
+    def get_chat_messages(self) -> List[Dict[str, str]]:
+        if self.strategy == BasicChatHistoryStrategy.last_k_messages:
+            return convert_messages_to_list_of_dictionaries(
+                self.message_store.get_last_k_messages(self.k)
+            )
+        elif self.strategy == BasicChatHistoryStrategy.last_k_tokens:
+            total_tokens = 0
+            selected_messages = []
+            converted_messages = convert_messages_to_list_of_dictionaries(
+                self.message_store.get_all_messages()
+            )
+            sys_message = None
+            if converted_messages[0]["role"] == "system":
+                sys_message = converted_messages.pop(0)
+            for message in reversed(converted_messages):
+                tokens = self.llm_provider.tokenize(message["content"])
+                total_tokens += len(tokens)
+                if total_tokens >= self.k:
+                    if len(selected_messages) == 0:
+                        selected_messages.append(message)
+                    break
+                else:
+                    selected_messages.append(message)
+            if sys_message is not None:
+                selected_messages.append(sys_message)
+            return list(reversed(selected_messages))
+        return []
```

### Comparing `llama_cpp_agent-0.1.3/src/llama_cpp_agent/messages_formatter.py` & `llama_cpp_agent-0.1.4/src/llama_cpp_agent/messages_formatter.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,579 +1,579 @@
-import json
-from enum import Enum
-from typing import List, Dict, Tuple, Literal
-
-SYS_PROMPT_START_MIXTRAL = """"""
-SYS_PROMPT_END_MIXTRAL = """\n\n"""
-USER_PROMPT_START_MIXTRAL = """[INST] """
-USER_PROMPT_END_MIXTRAL = """ """
-ASSISTANT_PROMPT_START_MIXTRAL = """[/INST] """
-ASSISTANT_PROMPT_END_MIXTRAL = """</s>"""
-FUNCTION_PROMPT_START_MIXTRAL = """"""
-FUNCTION_PROMPT_END_MIXTRAL = """"""
-DEFAULT_MIXTRAL_STOP_SEQUENCES = ["</s>"]
-
-MIXTRAL_8x22_TOOL_JINJA_TEMPLATE = "{{bos_token}}{% set user_messages = messages | selectattr('role', 'equalto', 'user') | list %}{% for message in messages %}{% if message['role'] == 'user' %}{% if message == user_messages[-1] %}{{ '[AVAILABLE_TOOLS]'}}{% for tool in tools %}{{ tool }}{% endfor %}{{ '[/AVAILABLE_TOOLS]'}}{{ '[INST]' + message['content'] + '[/INST]' }}{% else %}{{ '[INST]' + message['content'] + '[/INST]' }}{% endif %}{% elif message['role'] == 'assistant' %}{{ ' ' + message['content'] + ' ' + eos_token}}{% elif message['role'] == 'tool_results' %}{{'[TOOL_RESULTS]' + message['content']|string + '[/TOOL_RESULTS]'}}{% elif message['role'] == 'tool_calls' %}{{'[TOOL_CALLS]' + message['content']|string + eos_token}}{% endif %}{% endfor %}"
-MIXTRAL_8x22_DEFAULT_JINJA_TEMPLATE = "{{bos_token}}{% for message in messages %}{% if (message['role'] == 'user') != (loop.index0 % 2 == 0) %}{{ raise_exception('Conversation roles must alternate user/assistant/user/assistant/...') }}{% endif %}{% if message['role'] == 'user' %}{{ ' [INST] ' + message['content'] + ' [/INST]' }}{% elif message['role'] == 'assistant' %}{{ ' ' + message['content'] + ' ' + eos_token}}{% else %}{{ raise_exception('Only user and assistant roles are supported!') }}{% endif %}{% endfor %}"
-CHATML_JINJA_TEMPLATE = "{% for message in messages %}{{'<|im_start|>' + message['role'] + '\n' + message['content'] + '<|im_end|>' + '\n'}}{% endfor %}{% if add_generation_prompt %}{{ '<|im_start|>assistant\n' }}{% endif %}"
-SYS_PROMPT_START_CHATML = """<|im_start|>system\n"""
-SYS_PROMPT_END_CHATML = """<|im_end|>\n"""
-USER_PROMPT_START_CHATML = """<|im_start|>user\n"""
-USER_PROMPT_END_CHATML = """<|im_end|>\n"""
-ASSISTANT_PROMPT_START_CHATML = """<|im_start|>assistant\n"""
-ASSISTANT_PROMPT_END_CHATML = """<|im_end|>\n"""
-
-FUNCTION_PROMPT_START_CHATML = """<|im_start|>function\n"""
-FUNCTION_PROMPT_END_CHATML = """<|im_end|>\n"""
-DEFAULT_CHATML_STOP_SEQUENCES = [
-    "<|im_end|>",
-    "<|im_start|>assistant",
-    "<|im_start|>user",
-    "<|im_start|>system",
-]
-
-SYS_PROMPT_START_VICUNA = """"""
-SYS_PROMPT_END_VICUNA = """\n\n"""
-USER_PROMPT_START_VICUNA = """USER:"""
-USER_PROMPT_END_VICUNA = """\n"""
-ASSISTANT_PROMPT_START_VICUNA = """ASSISTANT:"""
-ASSISTANT_PROMPT_END_VICUNA = """"""
-FUNCTION_PROMPT_START_VICUNA = """"""
-FUNCTION_PROMPT_END_VICUNA = """"""
-DEFAULT_VICUNA_STOP_SEQUENCES = ["</s>", "USER:"]
-USER_PROMPT_START_LLAMA_2, USER_PROMPT_END_LLAMA_2 = "[INST] ", " [/INST]"
-
-ASSISTANT_PROMPT_START_LLAMA_2, ASSISTANT_PROMPT_END_LLAMA_2 = " ", " </s>"
-SYS_PROMPT_START_LLAMA_2, SYS_PROMPT_END_LLAMA_2 = "<<SYS>>\n", "\n<</SYS>>\n\n"
-FUNCTION_PROMPT_START_LLAMA_2, FUNCTION_PROMPT_END_LLAMA_2 = "", ""
-DEFAULT_LLAMA_2_STOP_SEQUENCES = ["</s>", "[INST]"]
-
-SYS_PROMPT_START_SYNTHIA = """SYSTEM: """
-SYS_PROMPT_END_SYNTHIA = """\n"""
-USER_PROMPT_START_SYNTHIA = """USER: """
-USER_PROMPT_END_SYNTHIA = """\n"""
-ASSISTANT_PROMPT_START_SYNTHIA = """ASSISTANT:"""
-ASSISTANT_PROMPT_END_SYNTHIA = """\n"""
-FUNCTION_PROMPT_START_SYNTHIA = """"""
-FUNCTION_PROMPT_END_SYNTHIA = """"""
-
-SYS_PROMPT_START_ALPACA = """### Instruction:\n"""
-SYS_PROMPT_END_ALPACA = """\n"""
-USER_PROMPT_START_ALPACA = """### Input:\n"""
-USER_PROMPT_END_ALPACA = """ \n"""
-ASSISTANT_PROMPT_START_ALPACA = """### Response:\n"""
-ASSISTANT_PROMPT_END_ALPACA = """\n"""
-FUNCTION_PROMPT_START_ALPACA = """"""
-FUNCTION_PROMPT_END_ALPACA = """"""
-DEFAULT_ALPACA_STOP_SEQUENCES = ["### Instruction:", "### Input:", "### Response:"]
-
-SYS_PROMPT_START_NEURAL_CHAT = """### System:\n"""
-SYS_PROMPT_END_NEURAL_CHAT = """\n"""
-USER_PROMPT_START_NEURAL_CHAT = """### User:\n"""
-USER_PROMPT_END_NEURAL_CHAT = """ \n"""
-ASSISTANT_PROMPT_START_NEURAL_CHAT = """### Assistant:\n"""
-ASSISTANT_PROMPT_END_NEURAL_CHAT = """\n"""
-FUNCTION_PROMPT_START_NEURAL_CHAT = """"""
-FUNCTION_PROMPT_END_NEURAL_CHAT = """"""
-DEFAULT_NEURAL_CHAT_STOP_SEQUENCES = ["### User:"]
-
-SYS_PROMPT_START_22B = """### System: """
-SYS_PROMPT_END_22B = """\n"""
-USER_PROMPT_START_22B = """### User: """
-USER_PROMPT_END_22B = """ \n"""
-ASSISTANT_PROMPT_START_22B = """### Assistant:"""
-ASSISTANT_PROMPT_END_22B = """\n"""
-FUNCTION_PROMPT_START_22B = """"""
-FUNCTION_PROMPT_END_22B = """"""
-DEFAULT_22B_STOP_SEQUENCES = ["### User:"]
-
-SYS_PROMPT_START_CODE_DS = """"""
-SYS_PROMPT_END_CODE_DS = """\n\n"""
-USER_PROMPT_START_CODE_DS = """@@ Instruction\n"""
-USER_PROMPT_END_CODE_DS = """\n\n"""
-ASSISTANT_PROMPT_START_CODE_DS = """@@ Response\n"""
-ASSISTANT_PROMPT_END_CODE_DS = """\n\n"""
-
-DEFAULT_CODE_DS_STOP_SEQUENCES = ["@@ Instruction"]
-
-SYS_PROMPT_START_LLAMA3 = """<|start_header_id|>system<|end_header_id|>\n"""
-SYS_PROMPT_END_LLAMA3 = """<|eot_id|>"""
-USER_PROMPT_START_LLAMA3 = """<|start_header_id|>user<|end_header_id|>\n"""
-USER_PROMPT_END_LLAMA3 = """<|eot_id|>"""
-ASSISTANT_PROMPT_START_LLAMA3 = """<|start_header_id|>assistant<|end_header_id|>\n"""
-ASSISTANT_PROMPT_END_LLAMA3 = """<|eot_id|>"""
-FUNCTION_PROMPT_START_LLAMA3 = (
-    """<|start_header_id|>function_calling_results<|end_header_id|>\n"""
-)
-FUNCTION_PROMPT_END_LLAMA3 = """<|eot_id|>"""
-DEFAULT_LLAMA3_STOP_SEQUENCES = ["assistant", "<|eot_id|>"]
-
-SYS_PROMPT_START_SOLAR = """"""
-SYS_PROMPT_END_SOLAR = """\n"""
-USER_PROMPT_START_SOLAR = """### User:\n"""
-USER_PROMPT_END_SOLAR = """ \n"""
-ASSISTANT_PROMPT_START_SOLAR = """### Assistant:\n"""
-ASSISTANT_PROMPT_END_SOLAR = """\n"""
-FUNCTION_PROMPT_START_SOLAR = """"""
-FUNCTION_PROMPT_END_SOLAR = """"""
-DEFAULT_SOLAR_STOP_SEQUENCES = ["### User:"]
-
-SYS_PROMPT_START_OPEN_CHAT = """"""
-SYS_PROMPT_END_OPEN_CHAT = """  """
-USER_PROMPT_START_OPEN_CHAT = """GPT4 Correct User: """
-USER_PROMPT_END_OPEN_CHAT = """<|end_of_turn|>"""
-ASSISTANT_PROMPT_START_OPEN_CHAT = """GPT4 Correct Assistant: """
-ASSISTANT_PROMPT_END_OPEN_CHAT = """<|end_of_turn|>"""
-FUNCTION_PROMPT_START_OPEN_CHAT = """"""
-FUNCTION_PROMPT_END_OPEN_CHAT = """"""
-DEFAULT_OPEN_CHAT_STOP_SEQUENCES = ["<|end_of_turn|>"]
-
-SYS_PROMPT_START_PHI_3 = """"""
-SYS_PROMPT_END_PHI_3 = """\n\n"""
-USER_PROMPT_START_PHI_3 = """<|user|>"""
-USER_PROMPT_END_PHI_3 = """<|end|>\n"""
-ASSISTANT_PROMPT_START_PHI_3 = """<|assistant|>"""
-ASSISTANT_PROMPT_END_PHI_3 = """<|end|>\n"""
-FUNCTION_PROMPT_START_PHI_3 = """"""
-FUNCTION_PROMPT_END_PHI_3 = """"""
-DEFAULT_PHI_3_STOP_SEQUENCES = ["<|end|>", "<|end_of_turn|>"]
-
-
-class MessagesFormatterType(Enum):
-    """
-    Enum representing different types of predefined messages formatters.
-    """
-
-    MIXTRAL = 1
-    CHATML = 2
-    VICUNA = 3
-    LLAMA_2 = 4
-    SYNTHIA = 5
-    NEURAL_CHAT = 6
-    SOLAR = 7
-    OPEN_CHAT = 8
-    ALPACA = 9
-    CODE_DS = 10
-    B22 = 11
-    LLAMA_3 = 12
-    PHI_3 = 13
-
-
-class MessagesFormatter:
-    """
-    Class representing a messages formatter for LLMs.
-    """
-
-    def __init__(
-        self,
-        PRE_PROMPT: str,
-        SYS_PROMPT_START: str,
-        SYS_PROMPT_END: str,
-        USER_PROMPT_START: str,
-        USER_PROMPT_END: str,
-        ASSISTANT_PROMPT_START: str,
-        ASSISTANT_PROMPT_END: str,
-        INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE: bool,
-        DEFAULT_STOP_SEQUENCES: List[str],
-        USE_USER_ROLE_FUNCTION_CALL_RESULT: bool = True,
-        FUNCTION_PROMPT_START: str = "",
-        FUNCTION_PROMPT_END: str = "",
-        STRIP_PROMPT: bool = True,
-    ):
-        """
-        Initializes a new MessagesFormatter object.
-
-        Args:
-            PRE_PROMPT (str): The pre-prompt content.
-            SYS_PROMPT_START (str): The system prompt start.
-            SYS_PROMPT_END (str): The system prompt end.
-            USER_PROMPT_START (str): The user prompt start.
-            USER_PROMPT_END (str): The user prompt end.
-            ASSISTANT_PROMPT_START (str): The assistant prompt start.
-            ASSISTANT_PROMPT_END (str): The assistant prompt end.
-            INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE (bool): Indicates whether to include the system prompt
-                                                             in the first user message.
-            DEFAULT_STOP_SEQUENCES (List[str]): List of default stop sequences.
-            USE_USER_ROLE_FUNCTION_CALL_RESULT (bool): Indicates whether to use user role for function call results.
-            FUNCTION_PROMPT_START (str): The function prompt start.
-            FUNCTION_PROMPT_END (str): The function prompt end.
-        """
-        self.PRE_PROMPT = PRE_PROMPT
-        self.SYS_PROMPT_START = SYS_PROMPT_START
-        self.SYS_PROMPT_END = SYS_PROMPT_END
-        self.USER_PROMPT_START = USER_PROMPT_START
-        self.USER_PROMPT_END = USER_PROMPT_END
-        self.ASSISTANT_PROMPT_START = ASSISTANT_PROMPT_START
-        self.ASSISTANT_PROMPT_END = ASSISTANT_PROMPT_END
-        self.INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE = (
-            INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE
-        )
-        self.DEFAULT_STOP_SEQUENCES = DEFAULT_STOP_SEQUENCES
-        self.FUNCTION_PROMPT_START = FUNCTION_PROMPT_START
-        self.FUNCTION_PROMPT_END = FUNCTION_PROMPT_END
-        self.USE_USER_ROLE_FUNCTION_CALL_RESULT = USE_USER_ROLE_FUNCTION_CALL_RESULT
-        self.STRIP_PROMPT = STRIP_PROMPT
-
-    def format_messages(
-        self,
-        messages: List[Dict[str, str]],
-        response_role: Literal["user", "assistant"] | None = None,
-    ) -> Tuple[str, str]:
-        """
-        Formats a list of messages into a conversation string.
-
-        Args:
-            messages (List[Dict[str, str]]): List of messages with role and content.
-            response_role(Literal["system", "user", "assistant", "function"]|None): Forces the response role to be "system", "user" or "assistant".
-        Returns:
-            Tuple[str, str]: Formatted conversation string and the role of the last message.
-        """
-        formatted_messages = self.PRE_PROMPT
-        last_role = "assistant"
-
-        no_user_prompt_start = False
-        for message in messages:
-            if message["role"] == "system":
-                formatted_messages += (
-                    self.SYS_PROMPT_START + message["content"] + self.SYS_PROMPT_END
-                )
-                last_role = "system"
-                if self.INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE:
-                    formatted_messages = self.USER_PROMPT_START + formatted_messages
-                    no_user_prompt_start = True
-            elif message["role"] == "user":
-                if no_user_prompt_start:
-                    no_user_prompt_start = False
-                    formatted_messages += message["content"] + self.USER_PROMPT_END
-                else:
-                    formatted_messages += (
-                        self.USER_PROMPT_START
-                        + message["content"]
-                        + self.USER_PROMPT_END
-                    )
-                last_role = "user"
-            elif message["role"] == "assistant":
-                if self.STRIP_PROMPT:
-                    message["content"] = message["content"].strip()
-                formatted_messages += (
-                    self.ASSISTANT_PROMPT_START
-                    + message["content"]
-                    + self.ASSISTANT_PROMPT_END
-                )
-                last_role = "assistant"
-            elif message["role"] == "function":
-                if isinstance(message["content"], list):
-                    message["content"] = "\n".join(
-                        [json.dumps(m, indent=2) for m in message["content"]]
-                    )
-                if self.USE_USER_ROLE_FUNCTION_CALL_RESULT:
-                    formatted_messages += (
-                        self.USER_PROMPT_START
-                        + message["content"]
-                        + self.USER_PROMPT_END
-                    )
-                    last_role = "user"
-                else:
-                    formatted_messages += (
-                        self.FUNCTION_PROMPT_START
-                        + message["content"]
-                        + self.FUNCTION_PROMPT_END
-                    )
-                    last_role = "function"
-        if last_role == "system" or last_role == "user" or last_role == "function":
-            if self.STRIP_PROMPT:
-                if response_role is not None:
-                    if response_role == "assistant":
-                        return (
-                            formatted_messages + self.ASSISTANT_PROMPT_START.strip(),
-                            "assistant",
-                        )
-                    if response_role == "user":
-                        return (
-                            formatted_messages + self.USER_PROMPT_START.strip(),
-                            "user",
-                        )
-                else:
-                    return (
-                        formatted_messages + self.ASSISTANT_PROMPT_START.strip(),
-                        "assistant",
-                    )
-            else:
-                if response_role is not None:
-                    if response_role == "assistant":
-                        return (
-                            formatted_messages + self.ASSISTANT_PROMPT_START,
-                            "assistant",
-                        )
-                    if response_role == "user":
-                        return formatted_messages + self.USER_PROMPT_START, "user"
-                else:
-                    return formatted_messages + self.ASSISTANT_PROMPT_START, "assistant"
-        if self.STRIP_PROMPT:
-            if response_role is not None:
-                if response_role == "assistant":
-                    return (
-                        formatted_messages + self.ASSISTANT_PROMPT_START.strip(),
-                        "assistant",
-                    )
-                if response_role == "user":
-                    return formatted_messages + self.USER_PROMPT_START.strip(), "user"
-            else:
-                return formatted_messages + self.USER_PROMPT_START.strip(), "user"
-        else:
-            if response_role is not None:
-                if response_role == "assistant":
-                    return formatted_messages + self.ASSISTANT_PROMPT_START, "assistant"
-                if response_role == "user":
-                    return formatted_messages + self.USER_PROMPT_START, "user"
-            else:
-                return formatted_messages + self.USER_PROMPT_START, "user"
-
-    def save(self, file_path: str):
-        """
-        Saves the messages formatter configuration to a file.
-
-        Args:
-           file_path (str): The file path to save the configuration.
-        """
-        with open(file_path, "w", encoding="utf-8") as file:
-            json.dump(self.as_dict(), file, indent=4)
-
-    @staticmethod
-    def load_from_file(file_path: str) -> "MessagesFormatter":
-        """
-        Loads a messages formatter configuration from a file.
-
-        Args:
-            file_path (str): The file path to load the configuration from.
-
-        Returns:
-            MessagesFormatter: Loaded messages formatter.
-        """
-        with open(file_path, "r", encoding="utf-8") as file:
-            loaded_messages_formatter = json.load(file)
-            return MessagesFormatter(**loaded_messages_formatter)
-
-    @staticmethod
-    def load_from_dict(loaded_messages_formatter: dict) -> "MessagesFormatter":
-        """
-        Creates a messages formatter from a dictionary.
-
-        Args:
-            loaded_messages_formatter (dict): Dictionary representing the messages formatter.
-
-        Returns:
-            MessagesFormatter: Created messages formatter.
-        """
-        return MessagesFormatter(**loaded_messages_formatter)
-
-    def as_dict(self) -> dict:
-        """
-        Converts the messages formatter to a dictionary.
-
-        Returns:
-            dict: Dictionary representation of the messages formatter.
-        """
-        return self.__dict__
-
-
-mixtral_formatter = MessagesFormatter(
-    "",
-    SYS_PROMPT_START_MIXTRAL,
-    SYS_PROMPT_END_MIXTRAL,
-    USER_PROMPT_START_MIXTRAL,
-    USER_PROMPT_END_MIXTRAL,
-    ASSISTANT_PROMPT_START_MIXTRAL,
-    ASSISTANT_PROMPT_END_MIXTRAL,
-    True,
-    DEFAULT_MIXTRAL_STOP_SEQUENCES,
-)
-chatml_formatter = MessagesFormatter(
-    "",
-    SYS_PROMPT_START_CHATML,
-    SYS_PROMPT_END_CHATML,
-    USER_PROMPT_START_CHATML,
-    USER_PROMPT_END_CHATML,
-    ASSISTANT_PROMPT_START_CHATML,
-    ASSISTANT_PROMPT_END_CHATML,
-    False,
-    DEFAULT_CHATML_STOP_SEQUENCES,
-    False,
-    FUNCTION_PROMPT_START_CHATML,
-    FUNCTION_PROMPT_END_CHATML,
-)
-vicuna_formatter = MessagesFormatter(
-    "",
-    SYS_PROMPT_START_VICUNA,
-    SYS_PROMPT_END_VICUNA,
-    USER_PROMPT_START_VICUNA,
-    USER_PROMPT_END_VICUNA,
-    ASSISTANT_PROMPT_START_VICUNA,
-    ASSISTANT_PROMPT_END_VICUNA,
-    False,
-    DEFAULT_VICUNA_STOP_SEQUENCES,
-)
-
-llama_2_formatter = MessagesFormatter(
-    "",
-    SYS_PROMPT_START_LLAMA_2,
-    SYS_PROMPT_END_LLAMA_2,
-    USER_PROMPT_START_LLAMA_2,
-    USER_PROMPT_END_LLAMA_2,
-    ASSISTANT_PROMPT_START_LLAMA_2,
-    ASSISTANT_PROMPT_END_LLAMA_2,
-    True,
-    DEFAULT_LLAMA_2_STOP_SEQUENCES,
-)
-
-llama_3_formatter = MessagesFormatter(
-    "",
-    SYS_PROMPT_START_LLAMA3,
-    SYS_PROMPT_END_LLAMA3,
-    USER_PROMPT_START_LLAMA3,
-    USER_PROMPT_END_LLAMA3,
-    ASSISTANT_PROMPT_START_LLAMA3,
-    ASSISTANT_PROMPT_END_LLAMA3,
-    False,
-    DEFAULT_LLAMA3_STOP_SEQUENCES,
-    USE_USER_ROLE_FUNCTION_CALL_RESULT=False,
-    FUNCTION_PROMPT_START=FUNCTION_PROMPT_START_LLAMA3,
-    FUNCTION_PROMPT_END=FUNCTION_PROMPT_END_LLAMA3,
-    STRIP_PROMPT=True,
-)
-
-synthia_formatter = MessagesFormatter(
-    "",
-    SYS_PROMPT_START_SYNTHIA,
-    SYS_PROMPT_END_SYNTHIA,
-    USER_PROMPT_START_SYNTHIA,
-    USER_PROMPT_END_SYNTHIA,
-    ASSISTANT_PROMPT_START_SYNTHIA,
-    ASSISTANT_PROMPT_END_SYNTHIA,
-    False,
-    DEFAULT_VICUNA_STOP_SEQUENCES,
-)
-
-neural_chat_formatter = MessagesFormatter(
-    "",
-    SYS_PROMPT_START_NEURAL_CHAT,
-    SYS_PROMPT_END_NEURAL_CHAT,
-    USER_PROMPT_START_NEURAL_CHAT,
-    USER_PROMPT_END_NEURAL_CHAT,
-    ASSISTANT_PROMPT_START_NEURAL_CHAT,
-    ASSISTANT_PROMPT_END_NEURAL_CHAT,
-    False,
-    DEFAULT_NEURAL_CHAT_STOP_SEQUENCES,
-    STRIP_PROMPT=False,
-)
-code_ds_formatter = MessagesFormatter(
-    "",
-    SYS_PROMPT_START_CODE_DS,
-    SYS_PROMPT_END_CODE_DS,
-    USER_PROMPT_START_CODE_DS,
-    USER_PROMPT_END_CODE_DS,
-    ASSISTANT_PROMPT_START_CODE_DS,
-    ASSISTANT_PROMPT_END_CODE_DS,
-    True,
-    DEFAULT_CODE_DS_STOP_SEQUENCES,
-)
-
-solar_formatter = MessagesFormatter(
-    "",
-    SYS_PROMPT_START_SOLAR,
-    SYS_PROMPT_END_SOLAR,
-    USER_PROMPT_START_SOLAR,
-    USER_PROMPT_END_SOLAR,
-    ASSISTANT_PROMPT_START_SOLAR,
-    ASSISTANT_PROMPT_END_SOLAR,
-    True,
-    DEFAULT_SOLAR_STOP_SEQUENCES,
-)
-
-open_chat_formatter = MessagesFormatter(
-    "",
-    SYS_PROMPT_START_OPEN_CHAT,
-    SYS_PROMPT_END_OPEN_CHAT,
-    USER_PROMPT_START_OPEN_CHAT,
-    USER_PROMPT_END_OPEN_CHAT,
-    ASSISTANT_PROMPT_START_OPEN_CHAT,
-    ASSISTANT_PROMPT_END_OPEN_CHAT,
-    True,
-    DEFAULT_OPEN_CHAT_STOP_SEQUENCES,
-    True,
-    FUNCTION_PROMPT_START_OPEN_CHAT,
-    FUNCTION_PROMPT_END_OPEN_CHAT,
-)
-
-alpaca_formatter = MessagesFormatter(
-    "",
-    SYS_PROMPT_START_ALPACA,
-    SYS_PROMPT_END_ALPACA,
-    USER_PROMPT_START_ALPACA,
-    USER_PROMPT_END_ALPACA,
-    ASSISTANT_PROMPT_START_ALPACA,
-    ASSISTANT_PROMPT_END_ALPACA,
-    False,
-    DEFAULT_ALPACA_STOP_SEQUENCES,
-    False,
-    FUNCTION_PROMPT_START_CHATML,
-    FUNCTION_PROMPT_END_CHATML,
-)
-
-b22_chat_formatter = MessagesFormatter(
-    "",
-    SYS_PROMPT_START_22B,
-    SYS_PROMPT_END_22B,
-    USER_PROMPT_START_22B,
-    USER_PROMPT_END_22B,
-    ASSISTANT_PROMPT_START_22B,
-    ASSISTANT_PROMPT_END_22B,
-    False,
-    DEFAULT_22B_STOP_SEQUENCES,
-    STRIP_PROMPT=False,
-)
-
-phi_3_chat_formatter = MessagesFormatter(
-    "",
-    SYS_PROMPT_START_PHI_3,
-    SYS_PROMPT_END_PHI_3,
-    USER_PROMPT_START_PHI_3,
-    USER_PROMPT_END_PHI_3,
-    ASSISTANT_PROMPT_START_PHI_3,
-    ASSISTANT_PROMPT_END_PHI_3,
-    True,
-    DEFAULT_PHI_3_STOP_SEQUENCES,
-    True,
-    FUNCTION_PROMPT_START_PHI_3,
-    FUNCTION_PROMPT_END_PHI_3,
-)
-
-predefined_formatter = {
-    MessagesFormatterType.MIXTRAL: mixtral_formatter,
-    MessagesFormatterType.CHATML: chatml_formatter,
-    MessagesFormatterType.VICUNA: vicuna_formatter,
-    MessagesFormatterType.LLAMA_2: llama_2_formatter,
-    MessagesFormatterType.SYNTHIA: synthia_formatter,
-    MessagesFormatterType.NEURAL_CHAT: neural_chat_formatter,
-    MessagesFormatterType.SOLAR: solar_formatter,
-    MessagesFormatterType.OPEN_CHAT: open_chat_formatter,
-    MessagesFormatterType.ALPACA: alpaca_formatter,
-    MessagesFormatterType.CODE_DS: code_ds_formatter,
-    MessagesFormatterType.B22: b22_chat_formatter,
-    MessagesFormatterType.LLAMA_3: llama_3_formatter,
-    MessagesFormatterType.PHI_3: phi_3_chat_formatter,
-}
-
-
-def get_predefined_messages_formatter(
-    formatter_type: MessagesFormatterType,
-) -> MessagesFormatter:
-    """
-    Gets a predefined messages formatter based on the formatter type.
-
-    Args:
-        formatter_type (MessagesFormatterType): The type of messages formatter.
-
-    Returns:
-        MessagesFormatter: The predefined messages formatter.
-    """
-    return predefined_formatter[formatter_type]
+import json
+from enum import Enum
+from typing import List, Dict, Tuple, Literal
+
+SYS_PROMPT_START_MIXTRAL = """"""
+SYS_PROMPT_END_MIXTRAL = """\n\n"""
+USER_PROMPT_START_MIXTRAL = """[INST] """
+USER_PROMPT_END_MIXTRAL = """ """
+ASSISTANT_PROMPT_START_MIXTRAL = """[/INST] """
+ASSISTANT_PROMPT_END_MIXTRAL = """</s>"""
+FUNCTION_PROMPT_START_MIXTRAL = """"""
+FUNCTION_PROMPT_END_MIXTRAL = """"""
+DEFAULT_MIXTRAL_STOP_SEQUENCES = ["</s>"]
+
+MIXTRAL_8x22_TOOL_JINJA_TEMPLATE = "{{bos_token}}{% set user_messages = messages | selectattr('role', 'equalto', 'user') | list %}{% for message in messages %}{% if message['role'] == 'user' %}{% if message == user_messages[-1] %}{{ '[AVAILABLE_TOOLS]'}}{% for tool in tools %}{{ tool }}{% endfor %}{{ '[/AVAILABLE_TOOLS]'}}{{ '[INST]' + message['content'] + '[/INST]' }}{% else %}{{ '[INST]' + message['content'] + '[/INST]' }}{% endif %}{% elif message['role'] == 'assistant' %}{{ ' ' + message['content'] + ' ' + eos_token}}{% elif message['role'] == 'tool_results' %}{{'[TOOL_RESULTS]' + message['content']|string + '[/TOOL_RESULTS]'}}{% elif message['role'] == 'tool_calls' %}{{'[TOOL_CALLS]' + message['content']|string + eos_token}}{% endif %}{% endfor %}"
+MIXTRAL_8x22_DEFAULT_JINJA_TEMPLATE = "{{bos_token}}{% for message in messages %}{% if (message['role'] == 'user') != (loop.index0 % 2 == 0) %}{{ raise_exception('Conversation roles must alternate user/assistant/user/assistant/...') }}{% endif %}{% if message['role'] == 'user' %}{{ ' [INST] ' + message['content'] + ' [/INST]' }}{% elif message['role'] == 'assistant' %}{{ ' ' + message['content'] + ' ' + eos_token}}{% else %}{{ raise_exception('Only user and assistant roles are supported!') }}{% endif %}{% endfor %}"
+CHATML_JINJA_TEMPLATE = "{% for message in messages %}{{'<|im_start|>' + message['role'] + '\n' + message['content'] + '<|im_end|>' + '\n'}}{% endfor %}{% if add_generation_prompt %}{{ '<|im_start|>assistant\n' }}{% endif %}"
+SYS_PROMPT_START_CHATML = """<|im_start|>system\n"""
+SYS_PROMPT_END_CHATML = """<|im_end|>\n"""
+USER_PROMPT_START_CHATML = """<|im_start|>user\n"""
+USER_PROMPT_END_CHATML = """<|im_end|>\n"""
+ASSISTANT_PROMPT_START_CHATML = """<|im_start|>assistant\n"""
+ASSISTANT_PROMPT_END_CHATML = """<|im_end|>\n"""
+
+FUNCTION_PROMPT_START_CHATML = """<|im_start|>function\n"""
+FUNCTION_PROMPT_END_CHATML = """<|im_end|>\n"""
+DEFAULT_CHATML_STOP_SEQUENCES = [
+    "<|im_end|>",
+    "<|im_start|>assistant",
+    "<|im_start|>user",
+    "<|im_start|>system",
+]
+
+SYS_PROMPT_START_VICUNA = """"""
+SYS_PROMPT_END_VICUNA = """\n\n"""
+USER_PROMPT_START_VICUNA = """USER:"""
+USER_PROMPT_END_VICUNA = """\n"""
+ASSISTANT_PROMPT_START_VICUNA = """ASSISTANT:"""
+ASSISTANT_PROMPT_END_VICUNA = """"""
+FUNCTION_PROMPT_START_VICUNA = """"""
+FUNCTION_PROMPT_END_VICUNA = """"""
+DEFAULT_VICUNA_STOP_SEQUENCES = ["</s>", "USER:"]
+USER_PROMPT_START_LLAMA_2, USER_PROMPT_END_LLAMA_2 = "[INST] ", " [/INST]"
+
+ASSISTANT_PROMPT_START_LLAMA_2, ASSISTANT_PROMPT_END_LLAMA_2 = " ", " </s>"
+SYS_PROMPT_START_LLAMA_2, SYS_PROMPT_END_LLAMA_2 = "<<SYS>>\n", "\n<</SYS>>\n\n"
+FUNCTION_PROMPT_START_LLAMA_2, FUNCTION_PROMPT_END_LLAMA_2 = "", ""
+DEFAULT_LLAMA_2_STOP_SEQUENCES = ["</s>", "[INST]"]
+
+SYS_PROMPT_START_SYNTHIA = """SYSTEM: """
+SYS_PROMPT_END_SYNTHIA = """\n"""
+USER_PROMPT_START_SYNTHIA = """USER: """
+USER_PROMPT_END_SYNTHIA = """\n"""
+ASSISTANT_PROMPT_START_SYNTHIA = """ASSISTANT:"""
+ASSISTANT_PROMPT_END_SYNTHIA = """\n"""
+FUNCTION_PROMPT_START_SYNTHIA = """"""
+FUNCTION_PROMPT_END_SYNTHIA = """"""
+
+SYS_PROMPT_START_ALPACA = """### Instruction:\n"""
+SYS_PROMPT_END_ALPACA = """\n"""
+USER_PROMPT_START_ALPACA = """### Input:\n"""
+USER_PROMPT_END_ALPACA = """ \n"""
+ASSISTANT_PROMPT_START_ALPACA = """### Response:\n"""
+ASSISTANT_PROMPT_END_ALPACA = """\n"""
+FUNCTION_PROMPT_START_ALPACA = """"""
+FUNCTION_PROMPT_END_ALPACA = """"""
+DEFAULT_ALPACA_STOP_SEQUENCES = ["### Instruction:", "### Input:", "### Response:"]
+
+SYS_PROMPT_START_NEURAL_CHAT = """### System:\n"""
+SYS_PROMPT_END_NEURAL_CHAT = """\n"""
+USER_PROMPT_START_NEURAL_CHAT = """### User:\n"""
+USER_PROMPT_END_NEURAL_CHAT = """ \n"""
+ASSISTANT_PROMPT_START_NEURAL_CHAT = """### Assistant:\n"""
+ASSISTANT_PROMPT_END_NEURAL_CHAT = """\n"""
+FUNCTION_PROMPT_START_NEURAL_CHAT = """"""
+FUNCTION_PROMPT_END_NEURAL_CHAT = """"""
+DEFAULT_NEURAL_CHAT_STOP_SEQUENCES = ["### User:"]
+
+SYS_PROMPT_START_22B = """### System: """
+SYS_PROMPT_END_22B = """\n"""
+USER_PROMPT_START_22B = """### User: """
+USER_PROMPT_END_22B = """ \n"""
+ASSISTANT_PROMPT_START_22B = """### Assistant:"""
+ASSISTANT_PROMPT_END_22B = """\n"""
+FUNCTION_PROMPT_START_22B = """"""
+FUNCTION_PROMPT_END_22B = """"""
+DEFAULT_22B_STOP_SEQUENCES = ["### User:"]
+
+SYS_PROMPT_START_CODE_DS = """"""
+SYS_PROMPT_END_CODE_DS = """\n\n"""
+USER_PROMPT_START_CODE_DS = """@@ Instruction\n"""
+USER_PROMPT_END_CODE_DS = """\n\n"""
+ASSISTANT_PROMPT_START_CODE_DS = """@@ Response\n"""
+ASSISTANT_PROMPT_END_CODE_DS = """\n\n"""
+
+DEFAULT_CODE_DS_STOP_SEQUENCES = ["@@ Instruction"]
+
+SYS_PROMPT_START_LLAMA3 = """<|start_header_id|>system<|end_header_id|>\n"""
+SYS_PROMPT_END_LLAMA3 = """<|eot_id|>"""
+USER_PROMPT_START_LLAMA3 = """<|start_header_id|>user<|end_header_id|>\n"""
+USER_PROMPT_END_LLAMA3 = """<|eot_id|>"""
+ASSISTANT_PROMPT_START_LLAMA3 = """<|start_header_id|>assistant<|end_header_id|>\n"""
+ASSISTANT_PROMPT_END_LLAMA3 = """<|eot_id|>"""
+FUNCTION_PROMPT_START_LLAMA3 = (
+    """<|start_header_id|>function_calling_results<|end_header_id|>\n"""
+)
+FUNCTION_PROMPT_END_LLAMA3 = """<|eot_id|>"""
+DEFAULT_LLAMA3_STOP_SEQUENCES = ["assistant", "<|eot_id|>"]
+
+SYS_PROMPT_START_SOLAR = """"""
+SYS_PROMPT_END_SOLAR = """\n"""
+USER_PROMPT_START_SOLAR = """### User:\n"""
+USER_PROMPT_END_SOLAR = """ \n"""
+ASSISTANT_PROMPT_START_SOLAR = """### Assistant:\n"""
+ASSISTANT_PROMPT_END_SOLAR = """\n"""
+FUNCTION_PROMPT_START_SOLAR = """"""
+FUNCTION_PROMPT_END_SOLAR = """"""
+DEFAULT_SOLAR_STOP_SEQUENCES = ["### User:"]
+
+SYS_PROMPT_START_OPEN_CHAT = """"""
+SYS_PROMPT_END_OPEN_CHAT = """  """
+USER_PROMPT_START_OPEN_CHAT = """GPT4 Correct User: """
+USER_PROMPT_END_OPEN_CHAT = """<|end_of_turn|>"""
+ASSISTANT_PROMPT_START_OPEN_CHAT = """GPT4 Correct Assistant: """
+ASSISTANT_PROMPT_END_OPEN_CHAT = """<|end_of_turn|>"""
+FUNCTION_PROMPT_START_OPEN_CHAT = """"""
+FUNCTION_PROMPT_END_OPEN_CHAT = """"""
+DEFAULT_OPEN_CHAT_STOP_SEQUENCES = ["<|end_of_turn|>"]
+
+SYS_PROMPT_START_PHI_3 = """"""
+SYS_PROMPT_END_PHI_3 = """\n\n"""
+USER_PROMPT_START_PHI_3 = """<|user|>"""
+USER_PROMPT_END_PHI_3 = """<|end|>\n"""
+ASSISTANT_PROMPT_START_PHI_3 = """<|assistant|>"""
+ASSISTANT_PROMPT_END_PHI_3 = """<|end|>\n"""
+FUNCTION_PROMPT_START_PHI_3 = """"""
+FUNCTION_PROMPT_END_PHI_3 = """"""
+DEFAULT_PHI_3_STOP_SEQUENCES = ["<|end|>", "<|end_of_turn|>"]
+
+
+class MessagesFormatterType(Enum):
+    """
+    Enum representing different types of predefined messages formatters.
+    """
+
+    MIXTRAL = 1
+    CHATML = 2
+    VICUNA = 3
+    LLAMA_2 = 4
+    SYNTHIA = 5
+    NEURAL_CHAT = 6
+    SOLAR = 7
+    OPEN_CHAT = 8
+    ALPACA = 9
+    CODE_DS = 10
+    B22 = 11
+    LLAMA_3 = 12
+    PHI_3 = 13
+
+
+class MessagesFormatter:
+    """
+    Class representing a messages formatter for LLMs.
+    """
+
+    def __init__(
+        self,
+        PRE_PROMPT: str,
+        SYS_PROMPT_START: str,
+        SYS_PROMPT_END: str,
+        USER_PROMPT_START: str,
+        USER_PROMPT_END: str,
+        ASSISTANT_PROMPT_START: str,
+        ASSISTANT_PROMPT_END: str,
+        INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE: bool,
+        DEFAULT_STOP_SEQUENCES: List[str],
+        USE_USER_ROLE_FUNCTION_CALL_RESULT: bool = True,
+        FUNCTION_PROMPT_START: str = "",
+        FUNCTION_PROMPT_END: str = "",
+        STRIP_PROMPT: bool = True,
+    ):
+        """
+        Initializes a new MessagesFormatter object.
+
+        Args:
+            PRE_PROMPT (str): The pre-prompt content.
+            SYS_PROMPT_START (str): The system prompt start.
+            SYS_PROMPT_END (str): The system prompt end.
+            USER_PROMPT_START (str): The user prompt start.
+            USER_PROMPT_END (str): The user prompt end.
+            ASSISTANT_PROMPT_START (str): The assistant prompt start.
+            ASSISTANT_PROMPT_END (str): The assistant prompt end.
+            INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE (bool): Indicates whether to include the system prompt
+                                                             in the first user message.
+            DEFAULT_STOP_SEQUENCES (List[str]): List of default stop sequences.
+            USE_USER_ROLE_FUNCTION_CALL_RESULT (bool): Indicates whether to use user role for function call results.
+            FUNCTION_PROMPT_START (str): The function prompt start.
+            FUNCTION_PROMPT_END (str): The function prompt end.
+        """
+        self.PRE_PROMPT = PRE_PROMPT
+        self.SYS_PROMPT_START = SYS_PROMPT_START
+        self.SYS_PROMPT_END = SYS_PROMPT_END
+        self.USER_PROMPT_START = USER_PROMPT_START
+        self.USER_PROMPT_END = USER_PROMPT_END
+        self.ASSISTANT_PROMPT_START = ASSISTANT_PROMPT_START
+        self.ASSISTANT_PROMPT_END = ASSISTANT_PROMPT_END
+        self.INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE = (
+            INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE
+        )
+        self.DEFAULT_STOP_SEQUENCES = DEFAULT_STOP_SEQUENCES
+        self.FUNCTION_PROMPT_START = FUNCTION_PROMPT_START
+        self.FUNCTION_PROMPT_END = FUNCTION_PROMPT_END
+        self.USE_USER_ROLE_FUNCTION_CALL_RESULT = USE_USER_ROLE_FUNCTION_CALL_RESULT
+        self.STRIP_PROMPT = STRIP_PROMPT
+
+    def format_messages(
+        self,
+        messages: List[Dict[str, str]],
+        response_role: Literal["user", "assistant"] | None = None,
+    ) -> Tuple[str, str]:
+        """
+        Formats a list of messages into a conversation string.
+
+        Args:
+            messages (List[Dict[str, str]]): List of messages with role and content.
+            response_role(Literal["system", "user", "assistant", "function"]|None): Forces the response role to be "system", "user" or "assistant".
+        Returns:
+            Tuple[str, str]: Formatted conversation string and the role of the last message.
+        """
+        formatted_messages = self.PRE_PROMPT
+        last_role = "assistant"
+
+        no_user_prompt_start = False
+        for message in messages:
+            if message["role"] == "system":
+                formatted_messages += (
+                    self.SYS_PROMPT_START + message["content"] + self.SYS_PROMPT_END
+                )
+                last_role = "system"
+                if self.INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE:
+                    formatted_messages = self.USER_PROMPT_START + formatted_messages
+                    no_user_prompt_start = True
+            elif message["role"] == "user":
+                if no_user_prompt_start:
+                    no_user_prompt_start = False
+                    formatted_messages += message["content"] + self.USER_PROMPT_END
+                else:
+                    formatted_messages += (
+                        self.USER_PROMPT_START
+                        + message["content"]
+                        + self.USER_PROMPT_END
+                    )
+                last_role = "user"
+            elif message["role"] == "assistant":
+                if self.STRIP_PROMPT:
+                    message["content"] = message["content"].strip()
+                formatted_messages += (
+                    self.ASSISTANT_PROMPT_START
+                    + message["content"]
+                    + self.ASSISTANT_PROMPT_END
+                )
+                last_role = "assistant"
+            elif message["role"] == "function":
+                if isinstance(message["content"], list):
+                    message["content"] = "\n".join(
+                        [json.dumps(m, indent=2) for m in message["content"]]
+                    )
+                if self.USE_USER_ROLE_FUNCTION_CALL_RESULT:
+                    formatted_messages += (
+                        self.USER_PROMPT_START
+                        + message["content"]
+                        + self.USER_PROMPT_END
+                    )
+                    last_role = "user"
+                else:
+                    formatted_messages += (
+                        self.FUNCTION_PROMPT_START
+                        + message["content"]
+                        + self.FUNCTION_PROMPT_END
+                    )
+                    last_role = "function"
+        if last_role == "system" or last_role == "user" or last_role == "function":
+            if self.STRIP_PROMPT:
+                if response_role is not None:
+                    if response_role == "assistant":
+                        return (
+                            formatted_messages + self.ASSISTANT_PROMPT_START.strip(),
+                            "assistant",
+                        )
+                    if response_role == "user":
+                        return (
+                            formatted_messages + self.USER_PROMPT_START.strip(),
+                            "user",
+                        )
+                else:
+                    return (
+                        formatted_messages + self.ASSISTANT_PROMPT_START.strip(),
+                        "assistant",
+                    )
+            else:
+                if response_role is not None:
+                    if response_role == "assistant":
+                        return (
+                            formatted_messages + self.ASSISTANT_PROMPT_START,
+                            "assistant",
+                        )
+                    if response_role == "user":
+                        return formatted_messages + self.USER_PROMPT_START, "user"
+                else:
+                    return formatted_messages + self.ASSISTANT_PROMPT_START, "assistant"
+        if self.STRIP_PROMPT:
+            if response_role is not None:
+                if response_role == "assistant":
+                    return (
+                        formatted_messages + self.ASSISTANT_PROMPT_START.strip(),
+                        "assistant",
+                    )
+                if response_role == "user":
+                    return formatted_messages + self.USER_PROMPT_START.strip(), "user"
+            else:
+                return formatted_messages + self.USER_PROMPT_START.strip(), "user"
+        else:
+            if response_role is not None:
+                if response_role == "assistant":
+                    return formatted_messages + self.ASSISTANT_PROMPT_START, "assistant"
+                if response_role == "user":
+                    return formatted_messages + self.USER_PROMPT_START, "user"
+            else:
+                return formatted_messages + self.USER_PROMPT_START, "user"
+
+    def save(self, file_path: str):
+        """
+        Saves the messages formatter configuration to a file.
+
+        Args:
+           file_path (str): The file path to save the configuration.
+        """
+        with open(file_path, "w", encoding="utf-8") as file:
+            json.dump(self.as_dict(), file, indent=4)
+
+    @staticmethod
+    def load_from_file(file_path: str) -> "MessagesFormatter":
+        """
+        Loads a messages formatter configuration from a file.
+
+        Args:
+            file_path (str): The file path to load the configuration from.
+
+        Returns:
+            MessagesFormatter: Loaded messages formatter.
+        """
+        with open(file_path, "r", encoding="utf-8") as file:
+            loaded_messages_formatter = json.load(file)
+            return MessagesFormatter(**loaded_messages_formatter)
+
+    @staticmethod
+    def load_from_dict(loaded_messages_formatter: dict) -> "MessagesFormatter":
+        """
+        Creates a messages formatter from a dictionary.
+
+        Args:
+            loaded_messages_formatter (dict): Dictionary representing the messages formatter.
+
+        Returns:
+            MessagesFormatter: Created messages formatter.
+        """
+        return MessagesFormatter(**loaded_messages_formatter)
+
+    def as_dict(self) -> dict:
+        """
+        Converts the messages formatter to a dictionary.
+
+        Returns:
+            dict: Dictionary representation of the messages formatter.
+        """
+        return self.__dict__
+
+
+mixtral_formatter = MessagesFormatter(
+    "",
+    SYS_PROMPT_START_MIXTRAL,
+    SYS_PROMPT_END_MIXTRAL,
+    USER_PROMPT_START_MIXTRAL,
+    USER_PROMPT_END_MIXTRAL,
+    ASSISTANT_PROMPT_START_MIXTRAL,
+    ASSISTANT_PROMPT_END_MIXTRAL,
+    True,
+    DEFAULT_MIXTRAL_STOP_SEQUENCES,
+)
+chatml_formatter = MessagesFormatter(
+    "",
+    SYS_PROMPT_START_CHATML,
+    SYS_PROMPT_END_CHATML,
+    USER_PROMPT_START_CHATML,
+    USER_PROMPT_END_CHATML,
+    ASSISTANT_PROMPT_START_CHATML,
+    ASSISTANT_PROMPT_END_CHATML,
+    False,
+    DEFAULT_CHATML_STOP_SEQUENCES,
+    False,
+    FUNCTION_PROMPT_START_CHATML,
+    FUNCTION_PROMPT_END_CHATML,
+)
+vicuna_formatter = MessagesFormatter(
+    "",
+    SYS_PROMPT_START_VICUNA,
+    SYS_PROMPT_END_VICUNA,
+    USER_PROMPT_START_VICUNA,
+    USER_PROMPT_END_VICUNA,
+    ASSISTANT_PROMPT_START_VICUNA,
+    ASSISTANT_PROMPT_END_VICUNA,
+    False,
+    DEFAULT_VICUNA_STOP_SEQUENCES,
+)
+
+llama_2_formatter = MessagesFormatter(
+    "",
+    SYS_PROMPT_START_LLAMA_2,
+    SYS_PROMPT_END_LLAMA_2,
+    USER_PROMPT_START_LLAMA_2,
+    USER_PROMPT_END_LLAMA_2,
+    ASSISTANT_PROMPT_START_LLAMA_2,
+    ASSISTANT_PROMPT_END_LLAMA_2,
+    True,
+    DEFAULT_LLAMA_2_STOP_SEQUENCES,
+)
+
+llama_3_formatter = MessagesFormatter(
+    "",
+    SYS_PROMPT_START_LLAMA3,
+    SYS_PROMPT_END_LLAMA3,
+    USER_PROMPT_START_LLAMA3,
+    USER_PROMPT_END_LLAMA3,
+    ASSISTANT_PROMPT_START_LLAMA3,
+    ASSISTANT_PROMPT_END_LLAMA3,
+    False,
+    DEFAULT_LLAMA3_STOP_SEQUENCES,
+    USE_USER_ROLE_FUNCTION_CALL_RESULT=False,
+    FUNCTION_PROMPT_START=FUNCTION_PROMPT_START_LLAMA3,
+    FUNCTION_PROMPT_END=FUNCTION_PROMPT_END_LLAMA3,
+    STRIP_PROMPT=True,
+)
+
+synthia_formatter = MessagesFormatter(
+    "",
+    SYS_PROMPT_START_SYNTHIA,
+    SYS_PROMPT_END_SYNTHIA,
+    USER_PROMPT_START_SYNTHIA,
+    USER_PROMPT_END_SYNTHIA,
+    ASSISTANT_PROMPT_START_SYNTHIA,
+    ASSISTANT_PROMPT_END_SYNTHIA,
+    False,
+    DEFAULT_VICUNA_STOP_SEQUENCES,
+)
+
+neural_chat_formatter = MessagesFormatter(
+    "",
+    SYS_PROMPT_START_NEURAL_CHAT,
+    SYS_PROMPT_END_NEURAL_CHAT,
+    USER_PROMPT_START_NEURAL_CHAT,
+    USER_PROMPT_END_NEURAL_CHAT,
+    ASSISTANT_PROMPT_START_NEURAL_CHAT,
+    ASSISTANT_PROMPT_END_NEURAL_CHAT,
+    False,
+    DEFAULT_NEURAL_CHAT_STOP_SEQUENCES,
+    STRIP_PROMPT=False,
+)
+code_ds_formatter = MessagesFormatter(
+    "",
+    SYS_PROMPT_START_CODE_DS,
+    SYS_PROMPT_END_CODE_DS,
+    USER_PROMPT_START_CODE_DS,
+    USER_PROMPT_END_CODE_DS,
+    ASSISTANT_PROMPT_START_CODE_DS,
+    ASSISTANT_PROMPT_END_CODE_DS,
+    True,
+    DEFAULT_CODE_DS_STOP_SEQUENCES,
+)
+
+solar_formatter = MessagesFormatter(
+    "",
+    SYS_PROMPT_START_SOLAR,
+    SYS_PROMPT_END_SOLAR,
+    USER_PROMPT_START_SOLAR,
+    USER_PROMPT_END_SOLAR,
+    ASSISTANT_PROMPT_START_SOLAR,
+    ASSISTANT_PROMPT_END_SOLAR,
+    True,
+    DEFAULT_SOLAR_STOP_SEQUENCES,
+)
+
+open_chat_formatter = MessagesFormatter(
+    "",
+    SYS_PROMPT_START_OPEN_CHAT,
+    SYS_PROMPT_END_OPEN_CHAT,
+    USER_PROMPT_START_OPEN_CHAT,
+    USER_PROMPT_END_OPEN_CHAT,
+    ASSISTANT_PROMPT_START_OPEN_CHAT,
+    ASSISTANT_PROMPT_END_OPEN_CHAT,
+    True,
+    DEFAULT_OPEN_CHAT_STOP_SEQUENCES,
+    True,
+    FUNCTION_PROMPT_START_OPEN_CHAT,
+    FUNCTION_PROMPT_END_OPEN_CHAT,
+)
+
+alpaca_formatter = MessagesFormatter(
+    "",
+    SYS_PROMPT_START_ALPACA,
+    SYS_PROMPT_END_ALPACA,
+    USER_PROMPT_START_ALPACA,
+    USER_PROMPT_END_ALPACA,
+    ASSISTANT_PROMPT_START_ALPACA,
+    ASSISTANT_PROMPT_END_ALPACA,
+    False,
+    DEFAULT_ALPACA_STOP_SEQUENCES,
+    False,
+    FUNCTION_PROMPT_START_CHATML,
+    FUNCTION_PROMPT_END_CHATML,
+)
+
+b22_chat_formatter = MessagesFormatter(
+    "",
+    SYS_PROMPT_START_22B,
+    SYS_PROMPT_END_22B,
+    USER_PROMPT_START_22B,
+    USER_PROMPT_END_22B,
+    ASSISTANT_PROMPT_START_22B,
+    ASSISTANT_PROMPT_END_22B,
+    False,
+    DEFAULT_22B_STOP_SEQUENCES,
+    STRIP_PROMPT=False,
+)
+
+phi_3_chat_formatter = MessagesFormatter(
+    "",
+    SYS_PROMPT_START_PHI_3,
+    SYS_PROMPT_END_PHI_3,
+    USER_PROMPT_START_PHI_3,
+    USER_PROMPT_END_PHI_3,
+    ASSISTANT_PROMPT_START_PHI_3,
+    ASSISTANT_PROMPT_END_PHI_3,
+    True,
+    DEFAULT_PHI_3_STOP_SEQUENCES,
+    True,
+    FUNCTION_PROMPT_START_PHI_3,
+    FUNCTION_PROMPT_END_PHI_3,
+)
+
+predefined_formatter = {
+    MessagesFormatterType.MIXTRAL: mixtral_formatter,
+    MessagesFormatterType.CHATML: chatml_formatter,
+    MessagesFormatterType.VICUNA: vicuna_formatter,
+    MessagesFormatterType.LLAMA_2: llama_2_formatter,
+    MessagesFormatterType.SYNTHIA: synthia_formatter,
+    MessagesFormatterType.NEURAL_CHAT: neural_chat_formatter,
+    MessagesFormatterType.SOLAR: solar_formatter,
+    MessagesFormatterType.OPEN_CHAT: open_chat_formatter,
+    MessagesFormatterType.ALPACA: alpaca_formatter,
+    MessagesFormatterType.CODE_DS: code_ds_formatter,
+    MessagesFormatterType.B22: b22_chat_formatter,
+    MessagesFormatterType.LLAMA_3: llama_3_formatter,
+    MessagesFormatterType.PHI_3: phi_3_chat_formatter,
+}
+
+
+def get_predefined_messages_formatter(
+    formatter_type: MessagesFormatterType,
+) -> MessagesFormatter:
+    """
+    Gets a predefined messages formatter based on the formatter type.
+
+    Args:
+        formatter_type (MessagesFormatterType): The type of messages formatter.
+
+    Returns:
+        MessagesFormatter: The predefined messages formatter.
+    """
+    return predefined_formatter[formatter_type]
```

### Comparing `llama_cpp_agent-0.1.3/src/llama_cpp_agent/mixtral_8x22b_agent.py` & `llama_cpp_agent-0.1.4/src/llama_cpp_agent/mixtral_8x22b_agent.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,117 +1,117 @@
-import json
-import random
-import string
-import uuid
-from enum import Enum
-
-from llama_cpp import Llama
-from mistral_common.protocol.instruct.messages import (
-    UserMessage,
-    SystemMessage,
-    AssistantMessage,
-    ToolMessage,
-)
-from mistral_common.protocol.instruct.request import ChatCompletionRequest
-from mistral_common.protocol.instruct.tool_calls import ToolCall, FunctionCall
-from mistral_common.tokens.tokenizers.mistral import MistralTokenizer
-from mistralai.client import MistralClient
-
-from llama_cpp_agent.function_calling import LlamaCppFunctionTool
-from llama_cpp_agent.llm_agent import LlamaCppAgent
-from llama_cpp_agent.llm_settings import LlamaLLMSettings
-from llama_cpp_agent.providers.llama_cpp_endpoint_provider import (
-    LlamaCppEndpointSettings,
-)
-from llama_cpp_agent.providers.openai_endpoint_provider import OpenAIEndpointSettings
-
-
-def generate_id(length=8):
-    # Characters to use in the ID
-    characters = string.ascii_letters + string.digits
-    # Random choice of characters
-    return "".join(random.choice(characters) for _ in range(length))
-
-
-class Mixtral8x22BAgent:
-    def __init__(
-        self,
-        model: (
-            Llama | LlamaLLMSettings | LlamaCppEndpointSettings | OpenAIEndpointSettings
-        ),
-        system_prompt: str = None,
-        debug_output: bool = False,
-    ):
-        self.messages: list[
-            SystemMessage | UserMessage | AssistantMessage | ToolMessage
-        ] = []
-        self.agent = LlamaCppAgent(model, debug_output=debug_output)
-        self.debug_output = debug_output
-        if system_prompt is not None:
-            self.messages.append(SystemMessage(content=system_prompt))
-        self.tokenizer_v3 = MistralTokenizer.v3()
-
-    def get_response(
-        self,
-        message=None,
-        tools: list[LlamaCppFunctionTool] = None,
-        temperature=0.7,
-        top_p=1.0,
-    ):
-        if tools is None:
-            tools = []
-        if message is not None:
-            msg = UserMessage(content=message)
-            self.messages.append(msg)
-        mistral_tools = []
-        mistral_tool_mapping = {}
-        for tool in tools:
-            mistral_tools.append(tool.to_mistral_tool())
-            mistral_tool_mapping[tool.model.__name__] = tool
-        request = ChatCompletionRequest(
-            tools=mistral_tools,
-            messages=self.messages,
-            model="open-mixtral-8x22b",
-        )
-        tokenized = self.tokenizer_v3.encode_chat_completion(request)
-        tokens, text = tokenized.tokens, tokenized.text
-        if self.debug_output:
-            print(text)
-        result = self.agent.get_text_response(
-            tokens,
-            temperature=temperature,
-            top_p=top_p,
-            stream=self.debug_output,
-            print_output=self.debug_output,
-        )
-
-        if result.strip().startswith("[TOOL_CALLS]"):
-            tool_calls = []
-
-            result = result.replace("[TOOL_CALLS]", "")
-            function_calls = json.loads(result.strip())
-            tool_messages = []
-            for function_call in function_calls:
-                tool = mistral_tool_mapping[function_call["name"]]
-                cls = tool.model
-                call_parameters = function_call["arguments"]
-                call = cls(**call_parameters)
-                output = call.run(**tool.additional_parameters)
-                tool_call_id = generate_id(length=9)
-                tool_calls.append(
-                    ToolCall(
-                        function=FunctionCall(
-                            name=function_call["name"],
-                            arguments=json.dumps(call_parameters),
-                        ),
-                        id=tool_call_id,
-                    )
-                )
-                tool_messages.append(
-                    ToolMessage(content=str(output), tool_call_id=tool_call_id)
-                )
-            self.messages.append(AssistantMessage(content=None, tool_calls=tool_calls))
-            self.messages.extend(tool_messages)
-            return self.get_response()
-        else:
-            self.messages.append(AssistantMessage(content=result.strip()))
-            return result.strip()
+import json
+import random
+import string
+import uuid
+from enum import Enum
+
+from llama_cpp import Llama
+from mistral_common.protocol.instruct.messages import (
+    UserMessage,
+    SystemMessage,
+    AssistantMessage,
+    ToolMessage,
+)
+from mistral_common.protocol.instruct.request import ChatCompletionRequest
+from mistral_common.protocol.instruct.tool_calls import ToolCall, FunctionCall
+from mistral_common.tokens.tokenizers.mistral import MistralTokenizer
+from mistralai.client import MistralClient
+
+from llama_cpp_agent.function_calling import LlamaCppFunctionTool
+from llama_cpp_agent.llm_agent import LlamaCppAgent
+from llama_cpp_agent.llm_settings import LlamaLLMSettings
+from llama_cpp_agent.providers.llama_cpp_endpoint_provider import (
+    LlamaCppEndpointSettings,
+)
+from llama_cpp_agent.providers.openai_endpoint_provider import OpenAIEndpointSettings
+
+
+def generate_id(length=8):
+    # Characters to use in the ID
+    characters = string.ascii_letters + string.digits
+    # Random choice of characters
+    return "".join(random.choice(characters) for _ in range(length))
+
+
+class Mixtral8x22BAgent:
+    def __init__(
+        self,
+        model: (
+            Llama | LlamaLLMSettings | LlamaCppEndpointSettings | OpenAIEndpointSettings
+        ),
+        system_prompt: str = None,
+        debug_output: bool = False,
+    ):
+        self.messages: list[
+            SystemMessage | UserMessage | AssistantMessage | ToolMessage
+        ] = []
+        self.agent = LlamaCppAgent(model, debug_output=debug_output)
+        self.debug_output = debug_output
+        if system_prompt is not None:
+            self.messages.append(SystemMessage(content=system_prompt))
+        self.tokenizer_v3 = MistralTokenizer.v3()
+
+    def get_response(
+        self,
+        message=None,
+        tools: list[LlamaCppFunctionTool] = None,
+        temperature=0.7,
+        top_p=1.0,
+    ):
+        if tools is None:
+            tools = []
+        if message is not None:
+            msg = UserMessage(content=message)
+            self.messages.append(msg)
+        mistral_tools = []
+        mistral_tool_mapping = {}
+        for tool in tools:
+            mistral_tools.append(tool.to_mistral_tool())
+            mistral_tool_mapping[tool.model.__name__] = tool
+        request = ChatCompletionRequest(
+            tools=mistral_tools,
+            messages=self.messages,
+            model="open-mixtral-8x22b",
+        )
+        tokenized = self.tokenizer_v3.encode_chat_completion(request)
+        tokens, text = tokenized.tokens, tokenized.text
+        if self.debug_output:
+            print(text)
+        result = self.agent.get_text_response(
+            tokens,
+            temperature=temperature,
+            top_p=top_p,
+            stream=self.debug_output,
+            print_output=self.debug_output,
+        )
+
+        if result.strip().startswith("[TOOL_CALLS]"):
+            tool_calls = []
+
+            result = result.replace("[TOOL_CALLS]", "")
+            function_calls = json.loads(result.strip())
+            tool_messages = []
+            for function_call in function_calls:
+                tool = mistral_tool_mapping[function_call["name"]]
+                cls = tool.model
+                call_parameters = function_call["arguments"]
+                call = cls(**call_parameters)
+                output = call.run(**tool.additional_parameters)
+                tool_call_id = generate_id(length=9)
+                tool_calls.append(
+                    ToolCall(
+                        function=FunctionCall(
+                            name=function_call["name"],
+                            arguments=json.dumps(call_parameters),
+                        ),
+                        id=tool_call_id,
+                    )
+                )
+                tool_messages.append(
+                    ToolMessage(content=str(output), tool_call_id=tool_call_id)
+                )
+            self.messages.append(AssistantMessage(content=None, tool_calls=tool_calls))
+            self.messages.extend(tool_messages)
+            return self.get_response()
+        else:
+            self.messages.append(AssistantMessage(content=result.strip()))
+            return result.strip()
```

### Comparing `llama_cpp_agent-0.1.3/src/llama_cpp_agent/output_parser.py` & `llama_cpp_agent-0.1.4/src/llama_cpp_agent/output_parser.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-import json
-import re
-
-
-def preprocess_json_string(json_string):
-    # Regular expression to find string values in JSON (this is a simplification and might not cover all edge cases)
-    string_regex = r'"([^"]*)"'
-
-    # Function to escape newlines within string values
-    def escape_newlines(match):
-        escaped_string = match.group(0).replace("\n", "\\n")
-        return escaped_string
-
-    # Replace unescaped newlines in string values
-    processed_string = re.sub(string_regex, escape_newlines, json_string)
-    return processed_string
-
-
-def sanitize_and_load_json(input_json):
-    fixed_json = preprocess_json_string(input_json)
-    fixed_json = fixed_json.replace("\r", "\\r")
-
-    try:
-        return json.loads(fixed_json)
-    except json.JSONDecodeError as e:
-        print(f"Error parsing JSON: {e}")
-        return None
-
-
-def is_empty_or_whitespace(s):
-    """
-    Checks if a string is empty or contains only whitespace.
-
-    Args:
-        s (str): The input string.
-
-    Returns:
-        bool: True if the string is empty or contains only whitespace, False otherwise.
-    """
-    return not s.strip()
-
-
-def parse_json_response(response: str):
-    """
-    Parses a JSON response string.
-
-    Args:
-        response (str): The JSON response string.
-
-    Returns:
-        dict: The parsed JSON object.
-    """
-
-    response_lines = response.split("\n")
-    while is_empty_or_whitespace(response_lines[0]):
-        response_lines.pop(0)
-    response = "\n".join(response_lines)
-    json_object = sanitize_and_load_json(response.strip())
-    return json_object
-
-
-def parse_json_response_with_markdown_code_block_or_triple_quoted_string(
-    json_response, marker
-):
-    """
-    Parses a JSON response string followed by a Markdown code block or triple-quoted string.
-
-    Args:
-        json_response (str): The JSON response string followed by a Markdown code block or triple-quoted string.
-        marker(str): Triple quotes (''') or triple back ticks (```)
-
-    Returns:
-        Tuple[dict, str]: The parsed JSON object and the content of the Markdown code block or triple-quoted string.
-    """
-    response_lines = json_response.split("\n")
-
-    if is_empty_or_whitespace(response_lines[0]):
-        response_lines.pop(0)
-
-    # Get the first line JSON object
-    response = response_lines[0]
-    # Remove the first line
-    response_lines.pop(0)
-    count = len(response_lines)
-    for _ in range(count):
-        if response_lines[0].startswith(marker):
-            break
-        else:
-            line = response_lines.pop(0)
-            response += "\n" + line
-
-    if len(response_lines) == 0:
-        return None, None
-    # Remove the first line Markdown code block marker
-    response_lines.pop(0)
-    # Remove the last line Markdown code block marker
-    response_lines.pop(-1)
-    response_lines.pop(-1)
-    # Combine lines into a single string
-    markdown_code_block_content = "\n".join(response_lines)
-    json_object = parse_json_response(response)
-
-    return json_object, markdown_code_block_content
-
-
-def extract_object_from_response(response: str, object_clas: type):
-    """
-    Extracts an object of the specified class from a JSON response string.
-
-    Args:
-        response (str): The JSON response string.
-        object_clas (type): The class of the object to be extracted.
-
-    Returns:
-        object_clas: An instance of the specified class.
-    """
-    obj = parse_json_response(response)
-    cls = object_clas
-    obj = cls(**obj)
-    return obj
+import json
+import re
+
+
+def preprocess_json_string(json_string):
+    # Regular expression to find string values in JSON (this is a simplification and might not cover all edge cases)
+    string_regex = r'"([^"]*)"'
+
+    # Function to escape newlines within string values
+    def escape_newlines(match):
+        escaped_string = match.group(0).replace("\n", "\\n")
+        return escaped_string
+
+    # Replace unescaped newlines in string values
+    processed_string = re.sub(string_regex, escape_newlines, json_string)
+    return processed_string
+
+
+def sanitize_and_load_json(input_json):
+    fixed_json = preprocess_json_string(input_json)
+    fixed_json = fixed_json.replace("\r", "\\r")
+
+    try:
+        return json.loads(fixed_json)
+    except json.JSONDecodeError as e:
+        print(f"Error parsing JSON: {e}")
+        return None
+
+
+def is_empty_or_whitespace(s):
+    """
+    Checks if a string is empty or contains only whitespace.
+
+    Args:
+        s (str): The input string.
+
+    Returns:
+        bool: True if the string is empty or contains only whitespace, False otherwise.
+    """
+    return not s.strip()
+
+
+def parse_json_response(response: str):
+    """
+    Parses a JSON response string.
+
+    Args:
+        response (str): The JSON response string.
+
+    Returns:
+        dict: The parsed JSON object.
+    """
+
+    response_lines = response.split("\n")
+    while is_empty_or_whitespace(response_lines[0]):
+        response_lines.pop(0)
+    response = "\n".join(response_lines)
+    json_object = sanitize_and_load_json(response.strip())
+    return json_object
+
+
+def parse_json_response_with_markdown_code_block_or_triple_quoted_string(
+    json_response, marker
+):
+    """
+    Parses a JSON response string followed by a Markdown code block or triple-quoted string.
+
+    Args:
+        json_response (str): The JSON response string followed by a Markdown code block or triple-quoted string.
+        marker(str): Triple quotes (''') or triple back ticks (```)
+
+    Returns:
+        Tuple[dict, str]: The parsed JSON object and the content of the Markdown code block or triple-quoted string.
+    """
+    response_lines = json_response.split("\n")
+
+    if is_empty_or_whitespace(response_lines[0]):
+        response_lines.pop(0)
+
+    # Get the first line JSON object
+    response = response_lines[0]
+    # Remove the first line
+    response_lines.pop(0)
+    count = len(response_lines)
+    for _ in range(count):
+        if response_lines[0].startswith(marker):
+            break
+        else:
+            line = response_lines.pop(0)
+            response += "\n" + line
+
+    if len(response_lines) == 0:
+        return None, None
+    # Remove the first line Markdown code block marker
+    response_lines.pop(0)
+    # Remove the last line Markdown code block marker
+    response_lines.pop(-1)
+    response_lines.pop(-1)
+    # Combine lines into a single string
+    markdown_code_block_content = "\n".join(response_lines)
+    json_object = parse_json_response(response)
+
+    return json_object, markdown_code_block_content
+
+
+def extract_object_from_response(response: str, object_clas: type):
+    """
+    Extracts an object of the specified class from a JSON response string.
+
+    Args:
+        response (str): The JSON response string.
+        object_clas (type): The class of the object to be extracted.
+
+    Returns:
+        object_clas: An instance of the specified class.
+    """
+    obj = parse_json_response(response)
+    cls = object_clas
+    obj = cls(**obj)
+    return obj
```

### Comparing `llama_cpp_agent-0.1.3/src/llama_cpp_agent/providers/kobold_cpp_endpoint_provider.py` & `llama_cpp_agent-0.1.4/src/llama_cpp_agent/providers/kobold_cpp_endpoint_provider.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,225 +1,225 @@
-import json
-from copy import copy
-from dataclasses import dataclass, field
-from typing import List, Optional, Union
-
-import requests
-
-
-@dataclass
-class KoboldCppGenerationSettings:
-    max_context_length: int
-    max_length: int
-    prompt: str
-    rep_pen: float
-    rep_pen_range: int
-    sampler_order: List[int]
-    sampler_seed: int
-    stop_sequence: List[str]
-    temperature: float
-    tfs: float
-    top_a: float
-    top_k: int
-    top_p: float
-    min_p: float
-    typical: float
-    stream: bool = True
-    use_default_badwordsids: bool = False
-    dynatemp_range: float = 0
-    mirostat: Optional[int] = None
-    mirostat_tau: float = 0
-    mirostat_eta: float = 0
-    genkey: Optional[str] = None
-    grammar_retain_state: bool = False
-    memory: Optional[str] = None
-    trim_stop: bool = False
-    logit_bias: Optional[dict] = field(default_factory=dict)
-
-    def save(self, file_path: str):
-        """
-        Save the settings to a file.
-
-        Args:
-            file_path (str): The path to the file.
-        """
-        with open(file_path, "w", encoding="utf-8") as file:
-            json.dump(self.as_dict(), file, indent=4)
-
-    @staticmethod
-    def load_from_file(file_path: str) -> "KoboldCppGenerationSettings":
-        """
-        Load the settings from a file.
-
-        Args:
-            file_path (str): The path to the file.
-
-        Returns:
-            KoboldCppGenerationSettings: The loaded settings.
-        """
-        with open(file_path, "r", encoding="utf-8") as file:
-            loaded_settings = json.load(file)
-            return KoboldCppGenerationSettings(**loaded_settings)
-
-    @staticmethod
-    def load_from_dict(settings: dict) -> "KoboldCppGenerationSettings":
-        """
-        Load the settings from a dictionary.
-
-        Args:
-            settings (dict): The dictionary containing the settings.
-
-        Returns:
-            KoboldCppGenerationSettings: The loaded settings.
-        """
-        return KoboldCppGenerationSettings(**settings)
-
-    def as_dict(self) -> dict:
-        """
-        Convert the settings to a dictionary.
-
-        Returns:
-            dict: The dictionary representation of the settings.
-        """
-        return self.__dict__
-
-
-@dataclass
-class KoboldCppEndpointSettings:
-    """
-    Settings for interacting with the kobold.cpp server.
-
-    Args:
-        completions_endpoint_url (str): The URL for the completions endpoint.
-
-    Attributes:
-        completions_endpoint_url (str): The URL for the completions endpoint.
-
-    Methods:
-        save(file_path: str): Save the settings to a file.
-        load_from_file(file_path: str) -> LlamaCppServerLLMSettings: Load the settings from a file.
-        load_from_dict(settings: dict) -> LlamaCppServerLLMSettings: Load the settings from a dictionary.
-        as_dict() -> dict: Convert the settings to a dictionary.
-        create_completion(prompt, grammar, generation_settings: LlamaCppServerGenerationSettings): Create a completion using the server.
-
-    """
-
-    completions_endpoint_url: str
-
-    def save(self, file_path: str):
-        """
-        Save the settings to a file.
-
-        Args:
-            file_path (str): The path to the file.
-        """
-        with open(file_path, "w", encoding="utf-8") as file:
-            json.dump(self.as_dict(), file, indent=4)
-
-    @staticmethod
-    def load_from_file(file_path: str) -> "KoboldCppEndpointSettings":
-        """
-        Load the settings from a file.
-
-        Args:
-            file_path (str): The path to the file.
-
-        Returns:
-            KoboldCppEndpointSettings: The loaded settings.
-        """
-        with open(file_path, "r", encoding="utf-8") as file:
-            loaded_settings = json.load(file)
-            return KoboldCppEndpointSettings(**loaded_settings)
-
-    @staticmethod
-    def load_from_dict(settings: dict) -> "KoboldCppEndpointSettings":
-        """
-        Load the settings from a dictionary.
-
-        Args:
-            settings (dict): The dictionary containing the settings.
-
-        Returns:
-            KoboldCppEndpointSettings: The loaded settings.
-        """
-        return KoboldCppEndpointSettings(**settings)
-
-    def as_dict(self) -> dict:
-        """
-        Convert the settings to a dictionary.
-
-        Returns:
-            dict: The dictionary representation of the settings.
-        """
-        return self.__dict__
-
-    def create_completion(
-        self, prompt, grammar, generation_settings: KoboldCppGenerationSettings
-    ):
-        """
-        Create a completion using the Llama.cpp server.
-
-        Args:
-            prompt: The input prompt.
-            grammar: The grammar for completion.
-            generation_settings (LlamaCppGenerationSettings): The generation settings.
-
-        Returns:
-            dict or generator: The completion response.
-        """
-        if generation_settings.stream:
-            return self.get_response_stream(prompt, grammar, generation_settings)
-
-        headers = {"Content-Type": "application/json"}
-
-        data = generation_settings.as_dict()
-        data["prompt"] = prompt
-        data["grammar"] = grammar
-        data["mirostat"] = data["mirostat_mode"]
-        data["stop"] = data["stop_sequences"]
-        del data["mirostat_mode"]
-        del data["stop_sequences"]
-
-        response = requests.post(
-            self.completions_endpoint_url, headers=headers, json=data
-        )
-        data = response.json()
-
-        returned_data = {"choices": [{"text": data["content"]}]}
-        return returned_data
-
-    def get_response_stream(self, prompt, grammar, generation_settings):
-        headers = {"Content-Type": "application/json"}
-
-        data = copy(generation_settings.as_dict())
-        data["prompt"] = prompt
-        data["grammar"] = grammar
-        data["mirostat"] = data["mirostat_mode"]
-        data["stop_sequence"] = data["stop_sequences"]
-        del data["mirostat_mode"]
-        del data["stop_sequences"]
-        response = requests.post(
-            self.completions_endpoint_url,
-            headers=headers,
-            json=data,
-            stream=generation_settings.stream,
-        )
-
-        # Check if the request was successful
-        response.raise_for_status()
-
-        # Define a generator function to yield text chunks
-        def generate_text_chunks():
-            try:
-                decoded_chunk = ""
-                for chunk in response.iter_lines():
-                    if chunk:
-                        decoded_chunk += chunk.decode("utf-8")
-                        new_data = json.loads(decoded_chunk.replace("data: ", ""))
-                        returned_data = {"choices": [{"text": new_data["content"]}]}
-                        yield returned_data
-                        decoded_chunk = ""
-
-            except requests.exceptions.RequestException as e:
-                print(f"Request failed: {e}")
-
-        return generate_text_chunks()
+import json
+from copy import copy
+from dataclasses import dataclass, field
+from typing import List, Optional, Union
+
+import requests
+
+
+@dataclass
+class KoboldCppGenerationSettings:
+    max_context_length: int
+    max_length: int
+    prompt: str
+    rep_pen: float
+    rep_pen_range: int
+    sampler_order: List[int]
+    sampler_seed: int
+    stop_sequence: List[str]
+    temperature: float
+    tfs: float
+    top_a: float
+    top_k: int
+    top_p: float
+    min_p: float
+    typical: float
+    stream: bool = True
+    use_default_badwordsids: bool = False
+    dynatemp_range: float = 0
+    mirostat: Optional[int] = None
+    mirostat_tau: float = 0
+    mirostat_eta: float = 0
+    genkey: Optional[str] = None
+    grammar_retain_state: bool = False
+    memory: Optional[str] = None
+    trim_stop: bool = False
+    logit_bias: Optional[dict] = field(default_factory=dict)
+
+    def save(self, file_path: str):
+        """
+        Save the settings to a file.
+
+        Args:
+            file_path (str): The path to the file.
+        """
+        with open(file_path, "w", encoding="utf-8") as file:
+            json.dump(self.as_dict(), file, indent=4)
+
+    @staticmethod
+    def load_from_file(file_path: str) -> "KoboldCppGenerationSettings":
+        """
+        Load the settings from a file.
+
+        Args:
+            file_path (str): The path to the file.
+
+        Returns:
+            KoboldCppGenerationSettings: The loaded settings.
+        """
+        with open(file_path, "r", encoding="utf-8") as file:
+            loaded_settings = json.load(file)
+            return KoboldCppGenerationSettings(**loaded_settings)
+
+    @staticmethod
+    def load_from_dict(settings: dict) -> "KoboldCppGenerationSettings":
+        """
+        Load the settings from a dictionary.
+
+        Args:
+            settings (dict): The dictionary containing the settings.
+
+        Returns:
+            KoboldCppGenerationSettings: The loaded settings.
+        """
+        return KoboldCppGenerationSettings(**settings)
+
+    def as_dict(self) -> dict:
+        """
+        Convert the settings to a dictionary.
+
+        Returns:
+            dict: The dictionary representation of the settings.
+        """
+        return self.__dict__
+
+
+@dataclass
+class KoboldCppEndpointSettings:
+    """
+    Settings for interacting with the kobold.cpp server.
+
+    Args:
+        completions_endpoint_url (str): The URL for the completions endpoint.
+
+    Attributes:
+        completions_endpoint_url (str): The URL for the completions endpoint.
+
+    Methods:
+        save(file_path: str): Save the settings to a file.
+        load_from_file(file_path: str) -> LlamaCppServerLLMSettings: Load the settings from a file.
+        load_from_dict(settings: dict) -> LlamaCppServerLLMSettings: Load the settings from a dictionary.
+        as_dict() -> dict: Convert the settings to a dictionary.
+        create_completion(prompt, grammar, generation_settings: LlamaCppServerGenerationSettings): Create a completion using the server.
+
+    """
+
+    completions_endpoint_url: str
+
+    def save(self, file_path: str):
+        """
+        Save the settings to a file.
+
+        Args:
+            file_path (str): The path to the file.
+        """
+        with open(file_path, "w", encoding="utf-8") as file:
+            json.dump(self.as_dict(), file, indent=4)
+
+    @staticmethod
+    def load_from_file(file_path: str) -> "KoboldCppEndpointSettings":
+        """
+        Load the settings from a file.
+
+        Args:
+            file_path (str): The path to the file.
+
+        Returns:
+            KoboldCppEndpointSettings: The loaded settings.
+        """
+        with open(file_path, "r", encoding="utf-8") as file:
+            loaded_settings = json.load(file)
+            return KoboldCppEndpointSettings(**loaded_settings)
+
+    @staticmethod
+    def load_from_dict(settings: dict) -> "KoboldCppEndpointSettings":
+        """
+        Load the settings from a dictionary.
+
+        Args:
+            settings (dict): The dictionary containing the settings.
+
+        Returns:
+            KoboldCppEndpointSettings: The loaded settings.
+        """
+        return KoboldCppEndpointSettings(**settings)
+
+    def as_dict(self) -> dict:
+        """
+        Convert the settings to a dictionary.
+
+        Returns:
+            dict: The dictionary representation of the settings.
+        """
+        return self.__dict__
+
+    def create_completion(
+        self, prompt, grammar, generation_settings: KoboldCppGenerationSettings
+    ):
+        """
+        Create a completion using the Llama.cpp server.
+
+        Args:
+            prompt: The input prompt.
+            grammar: The grammar for completion.
+            generation_settings (LlamaCppGenerationSettings): The generation settings.
+
+        Returns:
+            dict or generator: The completion response.
+        """
+        if generation_settings.stream:
+            return self.get_response_stream(prompt, grammar, generation_settings)
+
+        headers = {"Content-Type": "application/json"}
+
+        data = generation_settings.as_dict()
+        data["prompt"] = prompt
+        data["grammar"] = grammar
+        data["mirostat"] = data["mirostat_mode"]
+        data["stop"] = data["stop_sequences"]
+        del data["mirostat_mode"]
+        del data["stop_sequences"]
+
+        response = requests.post(
+            self.completions_endpoint_url, headers=headers, json=data
+        )
+        data = response.json()
+
+        returned_data = {"choices": [{"text": data["content"]}]}
+        return returned_data
+
+    def get_response_stream(self, prompt, grammar, generation_settings):
+        headers = {"Content-Type": "application/json"}
+
+        data = copy(generation_settings.as_dict())
+        data["prompt"] = prompt
+        data["grammar"] = grammar
+        data["mirostat"] = data["mirostat_mode"]
+        data["stop_sequence"] = data["stop_sequences"]
+        del data["mirostat_mode"]
+        del data["stop_sequences"]
+        response = requests.post(
+            self.completions_endpoint_url,
+            headers=headers,
+            json=data,
+            stream=generation_settings.stream,
+        )
+
+        # Check if the request was successful
+        response.raise_for_status()
+
+        # Define a generator function to yield text chunks
+        def generate_text_chunks():
+            try:
+                decoded_chunk = ""
+                for chunk in response.iter_lines():
+                    if chunk:
+                        decoded_chunk += chunk.decode("utf-8")
+                        new_data = json.loads(decoded_chunk.replace("data: ", ""))
+                        returned_data = {"choices": [{"text": new_data["content"]}]}
+                        yield returned_data
+                        decoded_chunk = ""
+
+            except requests.exceptions.RequestException as e:
+                print(f"Request failed: {e}")
+
+        return generate_text_chunks()
```

### Comparing `llama_cpp_agent-0.1.3/src/llama_cpp_agent/providers/llama_cpp_endpoint_provider.py` & `llama_cpp_agent-0.1.4/src/llama_cpp_agent/providers/llama_cpp_endpoint_provider.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,370 +1,370 @@
-import json
-from copy import copy
-
-import requests
-import aiohttp
-import json
-from dataclasses import dataclass, field
-from typing import List, Union
-
-
-@dataclass
-class LlamaCppGenerationSettings:
-    """
-    Settings for generating completions using the Llama.cpp server.
-
-    Args:
-        temperature (float): Controls the randomness of the generated completions. Higher values make the output more random.
-        top_k (int): Controls the diversity of the top-k sampling. Higher values result in more diverse completions.
-        top_p (float): Controls the diversity of the nucleus sampling. Higher values result in more diverse completions.
-        min_p (float): Minimum probability for nucleus sampling. Lower values result in more focused completions.
-        n_predict (int): Number of completions to predict. Set to -1 to use the default value.
-        n_keep (int): Number of completions to keep. Set to 0 for all predictions.
-        stream (bool): Enable streaming for long completions.
-        stop_sequences (List[str]): List of stop sequences to finish completion generation.
-        tfs_z (float): Controls the temperature for top frequent sampling.
-        typical_p (float): Typical probability for top frequent sampling.
-        repeat_penalty (float): Penalty for repeating tokens in completions.
-        repeat_last_n (int): Number of tokens to consider for repeat penalty.
-        penalize_nl (bool): Enable penalizing newlines in completions.
-        presence_penalty (float): Penalty for presence of certain tokens.
-        frequency_penalty (float): Penalty based on token frequency.
-        penalty_prompt (Union[None, str, List[int]]): Prompts to apply penalty for certain tokens.
-        mirostat_mode (int): Mirostat level.
-        mirostat_tau (float): Mirostat temperature.
-        mirostat_eta (float): Mirostat eta parameter.
-        seed (int): Seed for randomness. Set to -1 for no seed.
-        ignore_eos (bool): Ignore end-of-sequence token.
-
-    Attributes:
-        temperature (float): Controls the randomness of the generated completions. Higher values make the output more random.
-        top_k (int): Controls the diversity of the top-k sampling. Higher values result in more diverse completions.
-        top_p (float): Controls the diversity of the nucleus sampling. Higher values result in more diverse completions.
-        min_p (float): Minimum probability for nucleus sampling. Lower values result in more focused completions.
-        n_predict (int): Number of completions to predict. Set to -1 to use the default value.
-        n_keep (int): Number of completions to keep. Set to 0 for all predictions.
-        stream (bool): Enable streaming for long completions.
-        stop_sequences (List[str]): List of stop sequences to finish completion generation.
-        tfs_z (float): Controls the temperature for top frequent sampling.
-        typical_p (float): Typical probability for top frequent sampling.
-        repeat_penalty (float): Penalty for repeating tokens in completions.
-        repeat_last_n (int): Number of tokens to consider for repeat penalty.
-        penalize_nl (bool): Enable penalizing newlines in completions.
-        presence_penalty (float): Penalty for presence of certain tokens.
-        frequency_penalty (float): Penalty based on token frequency.
-        penalty_prompt (Union[None, str, List[int]]): Prompts to apply penalty for certain tokens.
-        mirostat_mode (int): Mirostat level.
-        mirostat_tau (float): Mirostat temperature.
-        mirostat_eta (float): Mirostat eta parameter.
-        seed (int): Seed for randomness. Set to -1 for no seed.
-        ignore_eos (bool): Ignore end-of-sequence token.
-    Methods:
-        save(file_path: str): Save the settings to a file.
-        load_from_file(file_path: str) -> LlamaCppServerGenerationSettings: Load the settings from a file.
-        load_from_dict(settings: dict) -> LlamaCppServerGenerationSettings: Load the settings from a dictionary.
-        as_dict() -> dict: Convert the settings to a dictionary.
-
-    """
-
-    temperature: float = 0.8
-    top_k: int = 40
-    top_p: float = 0.95
-    min_p: float = 0.05
-    n_predict: int = -1
-    n_keep: int = 0
-    stream: bool = False
-    stop_sequences: List[str] = None
-    tfs_z: float = 1.0
-    typical_p: float = 1.0
-    repeat_penalty: float = 1.1
-    repeat_last_n: int = -1
-    penalize_nl: bool = False
-    presence_penalty: float = 0.0
-    frequency_penalty: float = 0.0
-    penalty_prompt: Union[None, str, List[int]] = None
-    mirostat_mode: int = 0
-    mirostat_tau: float = 5.0
-    mirostat_eta: float = 0.1
-    cache_prompt: bool = True
-    seed: int = -1
-    ignore_eos: bool = False
-    samplers: List[str] = None
-
-    def save(self, file_path: str):
-        """
-        Save the settings to a file.
-
-        Args:
-            file_path (str): The path to the file.
-        """
-        with open(file_path, "w", encoding="utf-8") as file:
-            json.dump(self.as_dict(), file, indent=4)
-
-    @staticmethod
-    def load_from_file(file_path: str) -> "LlamaCppGenerationSettings":
-        """
-        Load the settings from a file.
-
-        Args:
-            file_path (str): The path to the file.
-
-        Returns:
-            LlamaCppGenerationSettings: The loaded settings.
-        """
-        with open(file_path, "r", encoding="utf-8") as file:
-            loaded_settings = json.load(file)
-            return LlamaCppGenerationSettings(**loaded_settings)
-
-    @staticmethod
-    def load_from_dict(settings: dict) -> "LlamaCppGenerationSettings":
-        """
-        Load the settings from a dictionary.
-
-        Args:
-            settings (dict): The dictionary containing the settings.
-
-        Returns:
-            LlamaCppGenerationSettings: The loaded settings.
-        """
-        return LlamaCppGenerationSettings(**settings)
-
-    def as_dict(self) -> dict:
-        """
-        Convert the settings to a dictionary.
-
-        Returns:
-            dict: The dictionary representation of the settings.
-        """
-        return self.__dict__
-
-
-@dataclass
-class LlamaCppEndpointSettings:
-    """
-    Settings for interacting with the Llama.cpp server.
-
-    Args:
-        completions_endpoint_url (str): The URL for the completions endpoint.
-
-    Attributes:
-        completions_endpoint_url (str): The URL for the completions endpoint.
-
-    Methods:
-        save(file_path: str): Save the settings to a file.
-        load_from_file(file_path: str) -> LlamaCppServerLLMSettings: Load the settings from a file.
-        load_from_dict(settings: dict) -> LlamaCppServerLLMSettings: Load the settings from a dictionary.
-        as_dict() -> dict: Convert the settings to a dictionary.
-        create_completion(prompt, grammar, generation_settings: LlamaCppServerGenerationSettings): Create a completion using the server.
-
-    """
-
-    completions_endpoint_url: str
-
-    def save(self, file_path: str):
-        """
-        Save the settings to a file.
-
-        Args:
-            file_path (str): The path to the file.
-        """
-        with open(file_path, "w", encoding="utf-8") as file:
-            json.dump(self.as_dict(), file, indent=4)
-
-    @staticmethod
-    def load_from_file(file_path: str) -> "LlamaCppEndpointSettings":
-        """
-        Load the settings from a file.
-
-        Args:
-            file_path (str): The path to the file.
-
-        Returns:
-            LlamaCppEndpointSettings: The loaded settings.
-        """
-        with open(file_path, "r", encoding="utf-8") as file:
-            loaded_settings = json.load(file)
-            return LlamaCppEndpointSettings(**loaded_settings)
-
-    @staticmethod
-    def load_from_dict(settings: dict) -> "LlamaCppEndpointSettings":
-        """
-        Load the settings from a dictionary.
-
-        Args:
-            settings (dict): The dictionary containing the settings.
-
-        Returns:
-            LlamaCppEndpointSettings: The loaded settings.
-        """
-        return LlamaCppEndpointSettings(**settings)
-
-    def as_dict(self) -> dict:
-        """
-        Convert the settings to a dictionary.
-
-        Returns:
-            dict: The dictionary representation of the settings.
-        """
-        return self.__dict__
-
-    def create_completion(
-        self, prompt, grammar, generation_settings: LlamaCppGenerationSettings
-    ):
-        """
-        Create a completion using the Llama.cpp server.
-
-        Args:
-            prompt: The input prompt.
-            grammar: The grammar for completion.
-            generation_settings (LlamaCppGenerationSettings): The generation settings.
-
-        Returns:
-            dict or generator: The completion response.
-        """
-        if generation_settings.stream:
-            return self.get_response_stream(prompt, grammar, generation_settings)
-
-        headers = {"Content-Type": "application/json"}
-
-        data = copy(generation_settings.as_dict())
-        data["prompt"] = prompt
-        data["grammar"] = grammar
-        data["mirostat"] = data["mirostat_mode"]
-        data["stop"] = data["stop_sequences"]
-        del data["mirostat_mode"]
-        del data["stop_sequences"]
-        if "samplers" not in data or data["samplers"] is None:
-            data["samplers"] = [
-                "top_k",
-                "tfs_z",
-                "typical_p",
-                "top_p",
-                "min_p",
-                "temperature",
-            ]
-        response = requests.post(
-            self.completions_endpoint_url, headers=headers, json=data
-        )
-        data = response.json()
-
-        returned_data = {"choices": [{"text": data["content"]}]}
-        return returned_data
-
-    def get_response_stream(self, prompt, grammar, generation_settings):
-        headers = {"Content-Type": "application/json"}
-
-        data = copy(generation_settings.as_dict())
-        data["prompt"] = prompt
-        data["grammar"] = grammar
-        data["mirostat"] = data["mirostat_mode"]
-        data["stop"] = data["stop_sequences"]
-        del data["mirostat_mode"]
-        del data["stop_sequences"]
-        if "samplers" not in data or data["samplers"] is None:
-            data["samplers"] = [
-                "top_k",
-                "tfs_z",
-                "typical_p",
-                "top_p",
-                "min_p",
-                "temperature",
-            ]
-        response = requests.post(
-            self.completions_endpoint_url,
-            headers=headers,
-            json=data,
-            stream=generation_settings.stream,
-        )
-
-        # Check if the request was successful
-        response.raise_for_status()
-
-        # Define a generator function to yield text chunks
-        def generate_text_chunks():
-            try:
-                decoded_chunk = ""
-                for chunk in response.iter_lines():
-                    if chunk:
-                        decoded_chunk += chunk.decode("utf-8")
-                        new_data = json.loads(decoded_chunk.replace("data: ", ""))
-                        returned_data = {"choices": [{"text": new_data["content"]}]}
-                        yield returned_data
-                        decoded_chunk = ""
-
-            except requests.exceptions.RequestException as e:
-                print(f"Request failed: {e}")
-
-        return generate_text_chunks()
-
-    async def async_create_completion(
-        self, prompt, grammar, generation_settings: LlamaCppGenerationSettings
-    ):
-        """
-        Create a completion using the Llama.cpp server asynchronously.
-
-        Args:
-            prompt: The input prompt.
-            grammar: The grammar for completion.
-            generation_settings (LlamaCppGenerationSettings): The generation settings.
-
-        Returns:
-            dict or async generator: The completion response.
-        """
-        if generation_settings.stream:
-            return await self.async_get_response_stream(
-                prompt, grammar, generation_settings
-            )
-
-        headers = {"Content-Type": "application/json"}
-
-        data = copy(generation_settings.as_dict())
-        data["prompt"] = prompt
-        data["grammar"] = grammar
-        data["mirostat"] = data["mirostat_mode"]
-        data["stop"] = data["stop_sequences"]
-        del data["mirostat_mode"]
-        del data["stop_sequences"]
-
-        async with aiohttp.ClientSession() as session:
-            async with session.post(
-                self.completions_endpoint_url, headers=headers, json=data
-            ) as response:
-                response_data = await response.json()
-
-        returned_data = {"choices": [{"text": response_data["content"]}]}
-        return returned_data
-
-    async def async_get_response_stream(self, prompt, grammar, generation_settings):
-        headers = {"Content-Type": "application/json"}
-
-        data = copy(generation_settings.as_dict())
-        data["prompt"] = prompt
-        data["grammar"] = grammar
-        data["mirostat"] = data["mirostat_mode"]
-        data["stop"] = data["stop_sequences"]
-        del data["mirostat_mode"]
-        del data["stop_sequences"]
-
-        async with aiohttp.ClientSession() as session:
-            async with session.post(
-                self.completions_endpoint_url, headers=headers, json=data
-            ) as response:
-                response.raise_for_status()
-
-                async def generate_text_chunks():
-                    try:
-                        # Since aiohttp doesn't separate 'stream' mode like requests, we directly handle chunk reading
-                        async for chunk in response.content.iter_any():
-                            if chunk:
-                                decoded_chunk = chunk.decode("utf-8")
-                                # Assuming JSON lines format; customize based on actual response format
-                                new_data = json.loads(decoded_chunk)
-                                returned_data = {
-                                    "choices": [{"text": new_data["content"]}]
-                                }
-                                yield returned_data
-
-                    except aiohttp.ClientError as e:
-                        print(f"HTTP request failed: {e}")
-
-                return generate_text_chunks()
+import json
+from copy import copy
+
+import requests
+import aiohttp
+import json
+from dataclasses import dataclass, field
+from typing import List, Union
+
+
+@dataclass
+class LlamaCppGenerationSettings:
+    """
+    Settings for generating completions using the Llama.cpp server.
+
+    Args:
+        temperature (float): Controls the randomness of the generated completions. Higher values make the output more random.
+        top_k (int): Controls the diversity of the top-k sampling. Higher values result in more diverse completions.
+        top_p (float): Controls the diversity of the nucleus sampling. Higher values result in more diverse completions.
+        min_p (float): Minimum probability for nucleus sampling. Lower values result in more focused completions.
+        n_predict (int): Number of completions to predict. Set to -1 to use the default value.
+        n_keep (int): Number of completions to keep. Set to 0 for all predictions.
+        stream (bool): Enable streaming for long completions.
+        stop_sequences (List[str]): List of stop sequences to finish completion generation.
+        tfs_z (float): Controls the temperature for top frequent sampling.
+        typical_p (float): Typical probability for top frequent sampling.
+        repeat_penalty (float): Penalty for repeating tokens in completions.
+        repeat_last_n (int): Number of tokens to consider for repeat penalty.
+        penalize_nl (bool): Enable penalizing newlines in completions.
+        presence_penalty (float): Penalty for presence of certain tokens.
+        frequency_penalty (float): Penalty based on token frequency.
+        penalty_prompt (Union[None, str, List[int]]): Prompts to apply penalty for certain tokens.
+        mirostat_mode (int): Mirostat level.
+        mirostat_tau (float): Mirostat temperature.
+        mirostat_eta (float): Mirostat eta parameter.
+        seed (int): Seed for randomness. Set to -1 for no seed.
+        ignore_eos (bool): Ignore end-of-sequence token.
+
+    Attributes:
+        temperature (float): Controls the randomness of the generated completions. Higher values make the output more random.
+        top_k (int): Controls the diversity of the top-k sampling. Higher values result in more diverse completions.
+        top_p (float): Controls the diversity of the nucleus sampling. Higher values result in more diverse completions.
+        min_p (float): Minimum probability for nucleus sampling. Lower values result in more focused completions.
+        n_predict (int): Number of completions to predict. Set to -1 to use the default value.
+        n_keep (int): Number of completions to keep. Set to 0 for all predictions.
+        stream (bool): Enable streaming for long completions.
+        stop_sequences (List[str]): List of stop sequences to finish completion generation.
+        tfs_z (float): Controls the temperature for top frequent sampling.
+        typical_p (float): Typical probability for top frequent sampling.
+        repeat_penalty (float): Penalty for repeating tokens in completions.
+        repeat_last_n (int): Number of tokens to consider for repeat penalty.
+        penalize_nl (bool): Enable penalizing newlines in completions.
+        presence_penalty (float): Penalty for presence of certain tokens.
+        frequency_penalty (float): Penalty based on token frequency.
+        penalty_prompt (Union[None, str, List[int]]): Prompts to apply penalty for certain tokens.
+        mirostat_mode (int): Mirostat level.
+        mirostat_tau (float): Mirostat temperature.
+        mirostat_eta (float): Mirostat eta parameter.
+        seed (int): Seed for randomness. Set to -1 for no seed.
+        ignore_eos (bool): Ignore end-of-sequence token.
+    Methods:
+        save(file_path: str): Save the settings to a file.
+        load_from_file(file_path: str) -> LlamaCppServerGenerationSettings: Load the settings from a file.
+        load_from_dict(settings: dict) -> LlamaCppServerGenerationSettings: Load the settings from a dictionary.
+        as_dict() -> dict: Convert the settings to a dictionary.
+
+    """
+
+    temperature: float = 0.8
+    top_k: int = 40
+    top_p: float = 0.95
+    min_p: float = 0.05
+    n_predict: int = -1
+    n_keep: int = 0
+    stream: bool = False
+    stop_sequences: List[str] = None
+    tfs_z: float = 1.0
+    typical_p: float = 1.0
+    repeat_penalty: float = 1.1
+    repeat_last_n: int = -1
+    penalize_nl: bool = False
+    presence_penalty: float = 0.0
+    frequency_penalty: float = 0.0
+    penalty_prompt: Union[None, str, List[int]] = None
+    mirostat_mode: int = 0
+    mirostat_tau: float = 5.0
+    mirostat_eta: float = 0.1
+    cache_prompt: bool = True
+    seed: int = -1
+    ignore_eos: bool = False
+    samplers: List[str] = None
+
+    def save(self, file_path: str):
+        """
+        Save the settings to a file.
+
+        Args:
+            file_path (str): The path to the file.
+        """
+        with open(file_path, "w", encoding="utf-8") as file:
+            json.dump(self.as_dict(), file, indent=4)
+
+    @staticmethod
+    def load_from_file(file_path: str) -> "LlamaCppGenerationSettings":
+        """
+        Load the settings from a file.
+
+        Args:
+            file_path (str): The path to the file.
+
+        Returns:
+            LlamaCppGenerationSettings: The loaded settings.
+        """
+        with open(file_path, "r", encoding="utf-8") as file:
+            loaded_settings = json.load(file)
+            return LlamaCppGenerationSettings(**loaded_settings)
+
+    @staticmethod
+    def load_from_dict(settings: dict) -> "LlamaCppGenerationSettings":
+        """
+        Load the settings from a dictionary.
+
+        Args:
+            settings (dict): The dictionary containing the settings.
+
+        Returns:
+            LlamaCppGenerationSettings: The loaded settings.
+        """
+        return LlamaCppGenerationSettings(**settings)
+
+    def as_dict(self) -> dict:
+        """
+        Convert the settings to a dictionary.
+
+        Returns:
+            dict: The dictionary representation of the settings.
+        """
+        return self.__dict__
+
+
+@dataclass
+class LlamaCppEndpointSettings:
+    """
+    Settings for interacting with the Llama.cpp server.
+
+    Args:
+        completions_endpoint_url (str): The URL for the completions endpoint.
+
+    Attributes:
+        completions_endpoint_url (str): The URL for the completions endpoint.
+
+    Methods:
+        save(file_path: str): Save the settings to a file.
+        load_from_file(file_path: str) -> LlamaCppServerLLMSettings: Load the settings from a file.
+        load_from_dict(settings: dict) -> LlamaCppServerLLMSettings: Load the settings from a dictionary.
+        as_dict() -> dict: Convert the settings to a dictionary.
+        create_completion(prompt, grammar, generation_settings: LlamaCppServerGenerationSettings): Create a completion using the server.
+
+    """
+
+    completions_endpoint_url: str
+
+    def save(self, file_path: str):
+        """
+        Save the settings to a file.
+
+        Args:
+            file_path (str): The path to the file.
+        """
+        with open(file_path, "w", encoding="utf-8") as file:
+            json.dump(self.as_dict(), file, indent=4)
+
+    @staticmethod
+    def load_from_file(file_path: str) -> "LlamaCppEndpointSettings":
+        """
+        Load the settings from a file.
+
+        Args:
+            file_path (str): The path to the file.
+
+        Returns:
+            LlamaCppEndpointSettings: The loaded settings.
+        """
+        with open(file_path, "r", encoding="utf-8") as file:
+            loaded_settings = json.load(file)
+            return LlamaCppEndpointSettings(**loaded_settings)
+
+    @staticmethod
+    def load_from_dict(settings: dict) -> "LlamaCppEndpointSettings":
+        """
+        Load the settings from a dictionary.
+
+        Args:
+            settings (dict): The dictionary containing the settings.
+
+        Returns:
+            LlamaCppEndpointSettings: The loaded settings.
+        """
+        return LlamaCppEndpointSettings(**settings)
+
+    def as_dict(self) -> dict:
+        """
+        Convert the settings to a dictionary.
+
+        Returns:
+            dict: The dictionary representation of the settings.
+        """
+        return self.__dict__
+
+    def create_completion(
+        self, prompt, grammar, generation_settings: LlamaCppGenerationSettings
+    ):
+        """
+        Create a completion using the Llama.cpp server.
+
+        Args:
+            prompt: The input prompt.
+            grammar: The grammar for completion.
+            generation_settings (LlamaCppGenerationSettings): The generation settings.
+
+        Returns:
+            dict or generator: The completion response.
+        """
+        if generation_settings.stream:
+            return self.get_response_stream(prompt, grammar, generation_settings)
+
+        headers = {"Content-Type": "application/json"}
+
+        data = copy(generation_settings.as_dict())
+        data["prompt"] = prompt
+        data["grammar"] = grammar
+        data["mirostat"] = data["mirostat_mode"]
+        data["stop"] = data["stop_sequences"]
+        del data["mirostat_mode"]
+        del data["stop_sequences"]
+        if "samplers" not in data or data["samplers"] is None:
+            data["samplers"] = [
+                "top_k",
+                "tfs_z",
+                "typical_p",
+                "top_p",
+                "min_p",
+                "temperature",
+            ]
+        response = requests.post(
+            self.completions_endpoint_url, headers=headers, json=data
+        )
+        data = response.json()
+
+        returned_data = {"choices": [{"text": data["content"]}]}
+        return returned_data
+
+    def get_response_stream(self, prompt, grammar, generation_settings):
+        headers = {"Content-Type": "application/json"}
+
+        data = copy(generation_settings.as_dict())
+        data["prompt"] = prompt
+        data["grammar"] = grammar
+        data["mirostat"] = data["mirostat_mode"]
+        data["stop"] = data["stop_sequences"]
+        del data["mirostat_mode"]
+        del data["stop_sequences"]
+        if "samplers" not in data or data["samplers"] is None:
+            data["samplers"] = [
+                "top_k",
+                "tfs_z",
+                "typical_p",
+                "top_p",
+                "min_p",
+                "temperature",
+            ]
+        response = requests.post(
+            self.completions_endpoint_url,
+            headers=headers,
+            json=data,
+            stream=generation_settings.stream,
+        )
+
+        # Check if the request was successful
+        response.raise_for_status()
+
+        # Define a generator function to yield text chunks
+        def generate_text_chunks():
+            try:
+                decoded_chunk = ""
+                for chunk in response.iter_lines():
+                    if chunk:
+                        decoded_chunk += chunk.decode("utf-8")
+                        new_data = json.loads(decoded_chunk.replace("data: ", ""))
+                        returned_data = {"choices": [{"text": new_data["content"]}]}
+                        yield returned_data
+                        decoded_chunk = ""
+
+            except requests.exceptions.RequestException as e:
+                print(f"Request failed: {e}")
+
+        return generate_text_chunks()
+
+    async def async_create_completion(
+        self, prompt, grammar, generation_settings: LlamaCppGenerationSettings
+    ):
+        """
+        Create a completion using the Llama.cpp server asynchronously.
+
+        Args:
+            prompt: The input prompt.
+            grammar: The grammar for completion.
+            generation_settings (LlamaCppGenerationSettings): The generation settings.
+
+        Returns:
+            dict or async generator: The completion response.
+        """
+        if generation_settings.stream:
+            return await self.async_get_response_stream(
+                prompt, grammar, generation_settings
+            )
+
+        headers = {"Content-Type": "application/json"}
+
+        data = copy(generation_settings.as_dict())
+        data["prompt"] = prompt
+        data["grammar"] = grammar
+        data["mirostat"] = data["mirostat_mode"]
+        data["stop"] = data["stop_sequences"]
+        del data["mirostat_mode"]
+        del data["stop_sequences"]
+
+        async with aiohttp.ClientSession() as session:
+            async with session.post(
+                self.completions_endpoint_url, headers=headers, json=data
+            ) as response:
+                response_data = await response.json()
+
+        returned_data = {"choices": [{"text": response_data["content"]}]}
+        return returned_data
+
+    async def async_get_response_stream(self, prompt, grammar, generation_settings):
+        headers = {"Content-Type": "application/json"}
+
+        data = copy(generation_settings.as_dict())
+        data["prompt"] = prompt
+        data["grammar"] = grammar
+        data["mirostat"] = data["mirostat_mode"]
+        data["stop"] = data["stop_sequences"]
+        del data["mirostat_mode"]
+        del data["stop_sequences"]
+
+        async with aiohttp.ClientSession() as session:
+            async with session.post(
+                self.completions_endpoint_url, headers=headers, json=data
+            ) as response:
+                response.raise_for_status()
+
+                async def generate_text_chunks():
+                    try:
+                        # Since aiohttp doesn't separate 'stream' mode like requests, we directly handle chunk reading
+                        async for chunk in response.content.iter_any():
+                            if chunk:
+                                decoded_chunk = chunk.decode("utf-8")
+                                # Assuming JSON lines format; customize based on actual response format
+                                new_data = json.loads(decoded_chunk)
+                                returned_data = {
+                                    "choices": [{"text": new_data["content"]}]
+                                }
+                                yield returned_data
+
+                    except aiohttp.ClientError as e:
+                        print(f"HTTP request failed: {e}")
+
+                return generate_text_chunks()
```

### Comparing `llama_cpp_agent-0.1.3/src/llama_cpp_agent/providers/provider_base.py` & `llama_cpp_agent-0.1.4/src/llama_cpp_agent/providers/provider_base.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,293 +1,293 @@
-import json
-from abc import ABC, abstractmethod
-from copy import copy
-from dataclasses import dataclass
-from typing import Any, Dict, List
-
-import requests
-from pydantic import BaseModel
-
-
-@dataclass
-class LLMGenerationSetting:
-    name: str
-    value: Any
-
-
-class LLMGenerationSettings(BaseModel):
-    settings: Dict[str, LLMGenerationSetting]
-
-    def get_settings_dict(self) -> Dict[str, Any]:
-        """Get the current settings as a dictionary."""
-        return {name: setting.value for name, setting in self.settings.items()}
-
-    def set_setting(self, name: str, value: Any):
-        """Set a setting to the given value."""
-        if name in self.settings:
-            self.settings[name].value = value
-        else:
-            self.settings[name] = LLMGenerationSetting(name=name, value=value)
-
-    def get_setting(self, name: str) -> Any:
-        """Get a setting from the given name."""
-        if name in self.settings:
-            return self.settings[name].value
-        return None
-
-    def __getattr__(self, name: str) -> Any:
-        """Access a setting from the given name as an attribute."""
-        if name in self.settings:
-            return self.settings[name].value
-        else:
-            raise AttributeError(
-                f"'{type(self).__name__}' object has no attribute '{name}'"
-            )
-
-    def as_dict(self) -> Dict[str, Any]:
-        """Get the current settings as a dictionary."""
-        return self.get_settings_dict()
-
-
-class LLMProviderBase(ABC):
-    """
-    Abstract base class for all LLM providers.
-    """
-
-    @abstractmethod
-    def get_default_generation_settings(self) -> LLMGenerationSettings:
-        """Get the default generation settings for the LLM provider."""
-        pass
-
-    @abstractmethod
-    def create_completion(
-        self, prompt: str, grammar: str, settings: LLMGenerationSettings
-    ):
-        """Create a completion request with the LLM provider and returns the result."""
-        pass
-
-    @abstractmethod
-    def create_chat_completion(
-        self,
-        messages: List[Dict[str, str]],
-        grammar: str,
-        settings: LLMGenerationSettings,
-    ):
-        """Create a chat completion request with the LLM provider and returns the result."""
-        pass
-
-    @abstractmethod
-    def tokenize(self, prompt: str):
-        """Tokenize the given prompt."""
-        pass
-
-
-class LlamaCppServerProvider(LLMProviderBase):
-    def __init__(
-        self,
-        server_address: str,
-        api_key: str = None,
-        llama_cpp_python_server: bool = False,
-    ):
-        self.server_address = server_address
-        if llama_cpp_python_server:
-            self.server_completion_endpoint = (
-                self.server_address + "/v1/engines/copilot-codex/completions"
-            )
-        else:
-            self.server_completion_endpoint = self.server_address + "/completion"
-
-        self.server_chat_completion_endpoint = (
-            self.server_address + "/v1/chat/completions"
-        )
-        if llama_cpp_python_server:
-            self.server_tokenize_endpoint = self.server_address + "/extras/tokenize"
-        else:
-            self.server_tokenize_endpoint = self.server_address + "/tokenize"
-        self.api_key = api_key
-        self.llama_cpp_python_server = llama_cpp_python_server
-
-    def get_default_generation_settings(self) -> LLMGenerationSettings:
-        default_settings = LLMGenerationSettings()
-        if self.llama_cpp_python_server:
-            dic = {
-                "temperature": 0.8,
-                "top_k": 40,
-                "top_p": 0.95,
-                "min_p": 0.05,
-                "max_tokens": -1,
-                "stream": False,
-                "stop_sequences": [],
-                "repeat_penalty": 1.1,
-                "presence_penalty": 0.0,
-                "frequency_penalty": 0.0,
-                "mirostat_mode": 0,
-                "mirostat_tau": 5.0,
-                "mirostat_eta": 0.1,
-                "seed": -1,
-            }
-        else:
-            dic = {
-                "temperature": 0.8,
-                "top_k": 40,
-                "top_p": 0.95,
-                "min_p": 0.05,
-                "n_predict": -1,
-                "n_keep": 0,
-                "stream": False,
-                "stop_sequences": [],
-                "tfs_z": 1.0,
-                "typical_p": 1.0,
-                "repeat_penalty": 1.1,
-                "repeat_last_n": -1,
-                "penalize_nl": False,
-                "presence_penalty": 0.0,
-                "frequency_penalty": 0.0,
-                "penalty_prompt": None,
-                "mirostat_mode": 0,
-                "mirostat_tau": 5.0,
-                "mirostat_eta": 0.1,
-                "seed": -1,
-                "ignore_eos": False,
-            }
-        # Populate the LLMGenerationSettings instance
-        for key, value in dic.items():
-            default_settings.set_setting(key, value)
-
-        return default_settings
-
-    def create_completion(
-        self, prompt: str, grammar: str, settings: LLMGenerationSettings
-    ):
-        if self.api_key is not None:
-            headers = {
-                "Content-Type": "application/json",
-                "Authorization": f"Bearer {self.api_key}",  # Add API key as bearer token
-            }
-        else:
-            headers = {"Content-Type": "application/json"}
-
-        data = copy(settings.as_dict())
-        data["prompt"] = prompt
-        data["grammar"] = grammar
-        if not self.llama_cpp_python_server:
-            data["mirostat"] = data.pop("mirostat_mode")
-        data["stop"] = data.pop("stop_sequences")
-        if not self.llama_cpp_python_server:
-            if "samplers" not in data or data["samplers"] is None:
-                data["samplers"] = [
-                    "top_k",
-                    "tfs_z",
-                    "typical_p",
-                    "top_p",
-                    "min_p",
-                    "temperature",
-                ]
-        if settings.stream:
-            return self.get_response_stream(
-                headers, data, self.server_completion_endpoint
-            )
-
-        response = requests.post(
-            self.server_completion_endpoint, headers=headers, json=data
-        )
-        data = response.json()
-
-        returned_data = {"choices": [{"text": data["content"]}]}
-        return returned_data
-
-    def create_chat_completion(
-        self,
-        messages: List[Dict[str, str]],
-        grammar: str,
-        settings: LLMGenerationSettings,
-    ):
-        if self.api_key is not None:
-            headers = {
-                "Content-Type": "application/json",
-                "Authorization": f"Bearer {self.api_key}",  # Add API key as bearer token
-            }
-        else:
-            headers = {"Content-Type": "application/json"}
-
-        data = copy(settings.as_dict())
-        data["messages"] = messages
-        data["grammar"] = grammar
-        if not self.llama_cpp_python_server:
-            data["mirostat"] = data.pop("mirostat_mode")
-        data["stop"] = data.pop("stop_sequences")
-        if not self.llama_cpp_python_server:
-            if "samplers" not in data or data["samplers"] is None:
-                data["samplers"] = [
-                    "top_k",
-                    "tfs_z",
-                    "typical_p",
-                    "top_p",
-                    "min_p",
-                    "temperature",
-                ]
-        if settings.stream:
-            return self.get_response_stream(
-                headers, data, self.server_chat_completion_endpoint
-            )
-
-        response = requests.post(
-            self.server_chat_completion_endpoint, headers=headers, json=data
-        )
-        data = response.json()
-
-        returned_data = {"choices": [{"text": data["content"]}]}
-        return returned_data
-
-    def tokenize(self, prompt: str) -> list[int]:
-        if self.api_key is not None:
-            headers = {
-                "Content-Type": "application/json",
-                "Authorization": f"Bearer {self.api_key}",  # Add API key as bearer token
-            }
-        else:
-            headers = {"Content-Type": "application/json"}
-        if self.llama_cpp_python_server:
-            response = requests.post(
-                self.server_tokenize_endpoint, headers=headers, json={"input": prompt}
-            )
-        else:
-            response = requests.post(
-                self.server_tokenize_endpoint, headers=headers, json={"content": prompt}
-            )
-        if response.status_code == 200:
-            tokens = response.json()["tokens"]
-            return tokens
-        else:
-            raise Exception(
-                f"Tokenization request failed. Status code: {response.status_code}\nResponse: {response.text}"
-            )
-
-    @staticmethod
-    def get_response_stream(headers, data, endpoint_address):
-
-        response = requests.post(
-            endpoint_address,
-            headers=headers,
-            json=data,
-            stream=True,
-        )
-
-        # Check if the request was successful
-        response.raise_for_status()
-
-        # Define a generator function to yield text chunks
-        def generate_text_chunks():
-            try:
-                decoded_chunk = ""
-                for chunk in response.iter_lines():
-                    if chunk:
-                        decoded_chunk += chunk.decode("utf-8")
-                        new_data = json.loads(decoded_chunk.replace("data: ", ""))
-                        returned_data = {"choices": [{"text": new_data["content"]}]}
-                        yield returned_data
-                        decoded_chunk = ""
-
-            except requests.exceptions.RequestException as e:
-                print(f"Request failed: {e}")
-
-        return generate_text_chunks()
+import json
+from abc import ABC, abstractmethod
+from copy import copy
+from dataclasses import dataclass
+from typing import Any, Dict, List
+
+import requests
+from pydantic import BaseModel
+
+
+@dataclass
+class LLMGenerationSetting:
+    name: str
+    value: Any
+
+
+class LLMGenerationSettings(BaseModel):
+    settings: Dict[str, LLMGenerationSetting]
+
+    def get_settings_dict(self) -> Dict[str, Any]:
+        """Get the current settings as a dictionary."""
+        return {name: setting.value for name, setting in self.settings.items()}
+
+    def set_setting(self, name: str, value: Any):
+        """Set a setting to the given value."""
+        if name in self.settings:
+            self.settings[name].value = value
+        else:
+            self.settings[name] = LLMGenerationSetting(name=name, value=value)
+
+    def get_setting(self, name: str) -> Any:
+        """Get a setting from the given name."""
+        if name in self.settings:
+            return self.settings[name].value
+        return None
+
+    def __getattr__(self, name: str) -> Any:
+        """Access a setting from the given name as an attribute."""
+        if name in self.settings:
+            return self.settings[name].value
+        else:
+            raise AttributeError(
+                f"'{type(self).__name__}' object has no attribute '{name}'"
+            )
+
+    def as_dict(self) -> Dict[str, Any]:
+        """Get the current settings as a dictionary."""
+        return self.get_settings_dict()
+
+
+class LLMProviderBase(ABC):
+    """
+    Abstract base class for all LLM providers.
+    """
+
+    @abstractmethod
+    def get_default_generation_settings(self) -> LLMGenerationSettings:
+        """Get the default generation settings for the LLM provider."""
+        pass
+
+    @abstractmethod
+    def create_completion(
+        self, prompt: str, grammar: str, settings: LLMGenerationSettings
+    ):
+        """Create a completion request with the LLM provider and returns the result."""
+        pass
+
+    @abstractmethod
+    def create_chat_completion(
+        self,
+        messages: List[Dict[str, str]],
+        grammar: str,
+        settings: LLMGenerationSettings,
+    ):
+        """Create a chat completion request with the LLM provider and returns the result."""
+        pass
+
+    @abstractmethod
+    def tokenize(self, prompt: str):
+        """Tokenize the given prompt."""
+        pass
+
+
+class LlamaCppServerProvider(LLMProviderBase):
+    def __init__(
+        self,
+        server_address: str,
+        api_key: str = None,
+        llama_cpp_python_server: bool = False,
+    ):
+        self.server_address = server_address
+        if llama_cpp_python_server:
+            self.server_completion_endpoint = (
+                self.server_address + "/v1/engines/copilot-codex/completions"
+            )
+        else:
+            self.server_completion_endpoint = self.server_address + "/completion"
+
+        self.server_chat_completion_endpoint = (
+            self.server_address + "/v1/chat/completions"
+        )
+        if llama_cpp_python_server:
+            self.server_tokenize_endpoint = self.server_address + "/extras/tokenize"
+        else:
+            self.server_tokenize_endpoint = self.server_address + "/tokenize"
+        self.api_key = api_key
+        self.llama_cpp_python_server = llama_cpp_python_server
+
+    def get_default_generation_settings(self) -> LLMGenerationSettings:
+        default_settings = LLMGenerationSettings()
+        if self.llama_cpp_python_server:
+            dic = {
+                "temperature": 0.8,
+                "top_k": 40,
+                "top_p": 0.95,
+                "min_p": 0.05,
+                "max_tokens": -1,
+                "stream": False,
+                "stop_sequences": [],
+                "repeat_penalty": 1.1,
+                "presence_penalty": 0.0,
+                "frequency_penalty": 0.0,
+                "mirostat_mode": 0,
+                "mirostat_tau": 5.0,
+                "mirostat_eta": 0.1,
+                "seed": -1,
+            }
+        else:
+            dic = {
+                "temperature": 0.8,
+                "top_k": 40,
+                "top_p": 0.95,
+                "min_p": 0.05,
+                "n_predict": -1,
+                "n_keep": 0,
+                "stream": False,
+                "stop_sequences": [],
+                "tfs_z": 1.0,
+                "typical_p": 1.0,
+                "repeat_penalty": 1.1,
+                "repeat_last_n": -1,
+                "penalize_nl": False,
+                "presence_penalty": 0.0,
+                "frequency_penalty": 0.0,
+                "penalty_prompt": None,
+                "mirostat_mode": 0,
+                "mirostat_tau": 5.0,
+                "mirostat_eta": 0.1,
+                "seed": -1,
+                "ignore_eos": False,
+            }
+        # Populate the LLMGenerationSettings instance
+        for key, value in dic.items():
+            default_settings.set_setting(key, value)
+
+        return default_settings
+
+    def create_completion(
+        self, prompt: str, grammar: str, settings: LLMGenerationSettings
+    ):
+        if self.api_key is not None:
+            headers = {
+                "Content-Type": "application/json",
+                "Authorization": f"Bearer {self.api_key}",  # Add API key as bearer token
+            }
+        else:
+            headers = {"Content-Type": "application/json"}
+
+        data = copy(settings.as_dict())
+        data["prompt"] = prompt
+        data["grammar"] = grammar
+        if not self.llama_cpp_python_server:
+            data["mirostat"] = data.pop("mirostat_mode")
+        data["stop"] = data.pop("stop_sequences")
+        if not self.llama_cpp_python_server:
+            if "samplers" not in data or data["samplers"] is None:
+                data["samplers"] = [
+                    "top_k",
+                    "tfs_z",
+                    "typical_p",
+                    "top_p",
+                    "min_p",
+                    "temperature",
+                ]
+        if settings.stream:
+            return self.get_response_stream(
+                headers, data, self.server_completion_endpoint
+            )
+
+        response = requests.post(
+            self.server_completion_endpoint, headers=headers, json=data
+        )
+        data = response.json()
+
+        returned_data = {"choices": [{"text": data["content"]}]}
+        return returned_data
+
+    def create_chat_completion(
+        self,
+        messages: List[Dict[str, str]],
+        grammar: str,
+        settings: LLMGenerationSettings,
+    ):
+        if self.api_key is not None:
+            headers = {
+                "Content-Type": "application/json",
+                "Authorization": f"Bearer {self.api_key}",  # Add API key as bearer token
+            }
+        else:
+            headers = {"Content-Type": "application/json"}
+
+        data = copy(settings.as_dict())
+        data["messages"] = messages
+        data["grammar"] = grammar
+        if not self.llama_cpp_python_server:
+            data["mirostat"] = data.pop("mirostat_mode")
+        data["stop"] = data.pop("stop_sequences")
+        if not self.llama_cpp_python_server:
+            if "samplers" not in data or data["samplers"] is None:
+                data["samplers"] = [
+                    "top_k",
+                    "tfs_z",
+                    "typical_p",
+                    "top_p",
+                    "min_p",
+                    "temperature",
+                ]
+        if settings.stream:
+            return self.get_response_stream(
+                headers, data, self.server_chat_completion_endpoint
+            )
+
+        response = requests.post(
+            self.server_chat_completion_endpoint, headers=headers, json=data
+        )
+        data = response.json()
+
+        returned_data = {"choices": [{"text": data["content"]}]}
+        return returned_data
+
+    def tokenize(self, prompt: str) -> list[int]:
+        if self.api_key is not None:
+            headers = {
+                "Content-Type": "application/json",
+                "Authorization": f"Bearer {self.api_key}",  # Add API key as bearer token
+            }
+        else:
+            headers = {"Content-Type": "application/json"}
+        if self.llama_cpp_python_server:
+            response = requests.post(
+                self.server_tokenize_endpoint, headers=headers, json={"input": prompt}
+            )
+        else:
+            response = requests.post(
+                self.server_tokenize_endpoint, headers=headers, json={"content": prompt}
+            )
+        if response.status_code == 200:
+            tokens = response.json()["tokens"]
+            return tokens
+        else:
+            raise Exception(
+                f"Tokenization request failed. Status code: {response.status_code}\nResponse: {response.text}"
+            )
+
+    @staticmethod
+    def get_response_stream(headers, data, endpoint_address):
+
+        response = requests.post(
+            endpoint_address,
+            headers=headers,
+            json=data,
+            stream=True,
+        )
+
+        # Check if the request was successful
+        response.raise_for_status()
+
+        # Define a generator function to yield text chunks
+        def generate_text_chunks():
+            try:
+                decoded_chunk = ""
+                for chunk in response.iter_lines():
+                    if chunk:
+                        decoded_chunk += chunk.decode("utf-8")
+                        new_data = json.loads(decoded_chunk.replace("data: ", ""))
+                        returned_data = {"choices": [{"text": new_data["content"]}]}
+                        yield returned_data
+                        decoded_chunk = ""
+
+            except requests.exceptions.RequestException as e:
+                print(f"Request failed: {e}")
+
+        return generate_text_chunks()
```

### Comparing `llama_cpp_agent-0.1.3/src/llama_cpp_agent/rag/text_utils.py` & `llama_cpp_agent-0.1.4/src/llama_cpp_agent/rag/text_utils.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-class TextChunker:
-    def __init__(self, text, chunk_size, overlap=0):
-        """
-        Initializes the TextChunker instance.
-
-        Parameters:
-            text (str): The text to be chunked.
-            chunk_size (int): The length of each text chunk.
-            overlap (int): The number of characters that should overlap between consecutive chunks.
-        """
-        self.text = text
-        self.chunk_size = chunk_size
-        self.overlap = overlap
-
-    def get_chunks(self):
-        """
-        Generates the text chunks based on the specified chunk size and overlap.
-
-        Returns:
-            list[str]: A list of chunked text segments.
-        """
-        chunks = []
-        start = 0
-        while start < len(self.text):
-            # Calculate end index of the chunk
-            end = start + self.chunk_size
-            # Append chunk to the list
-            chunks.append(self.text[start:end])
-            # Update start index for the next chunk
-            start = end - self.overlap if self.overlap < self.chunk_size else start + 1
-            # Prevent infinite loop in case overlap is not less than chunk_size
-            if self.chunk_size <= self.overlap:
-                raise ValueError(
-                    "Overlap must be less than chunk size to prevent infinite loops."
-                )
-        return chunks
-
-
-import re
-
-
-class RecursiveCharacterTextSplitter:
-    def __init__(
-        self,
-        separators,
-        chunk_size,
-        chunk_overlap,
-        length_function=len,
-        keep_separator=False,
-    ):
-        self.separators = separators
-        self.chunk_size = chunk_size
-        self.chunk_overlap = chunk_overlap
-        self.length_function = length_function
-        self.keep_separator = keep_separator
-
-    def split_text(self, text, depth=0):
-        if depth == len(self.separators):
-            return self._split_into_fixed_size(text)
-
-        current_separator = self.separators[depth]
-        if current_separator == "":
-            return list(text)
-
-        if self.keep_separator:
-            # Use regex to keep separators with the text
-            pieces = re.split(f"({re.escape(current_separator)})", text)
-            # Reattach separators to the chunks
-            pieces = [
-                (
-                    pieces[i] + pieces[i + 1]
-                    if i + 1 < len(pieces) and pieces[i + 1] == current_separator
-                    else pieces[i]
-                )
-                for i in range(0, len(pieces), 2)
-            ]
-        else:
-            pieces = text.split(current_separator)
-
-        refined_pieces = []
-
-        for piece in pieces:
-            if self.length_function(piece) > self.chunk_size:
-                refined_pieces.extend(self.split_text(piece, depth + 1))
-            else:
-                refined_pieces.append(piece)
-
-        return self._merge_pieces(refined_pieces) if depth == 0 else refined_pieces
-
-    def _split_into_fixed_size(self, text):
-        size = self.chunk_size
-        overlap = self.chunk_overlap
-        chunks = [text[i : i + size] for i in range(0, len(text), size - overlap)]
-        if chunks and len(chunks[-1]) < overlap:
-            chunks[-2] += chunks[-1]
-            chunks.pop()
-        return chunks
-
-    def _merge_pieces(self, pieces):
-        merged = []
-        current_chunk = pieces[0]
-
-        for piece in pieces[1:]:
-            if self.length_function(current_chunk + piece) <= self.chunk_size:
-                current_chunk += piece
-            else:
-                merged.append(current_chunk)
-                if len(current_chunk) == self.chunk_size:
-                    current_chunk = current_chunk[-self.chunk_overlap :] + piece
-                else:
-                    current_chunk = piece
-
-        merged.append(current_chunk)
-        return merged
+class TextChunker:
+    def __init__(self, text, chunk_size, overlap=0):
+        """
+        Initializes the TextChunker instance.
+
+        Parameters:
+            text (str): The text to be chunked.
+            chunk_size (int): The length of each text chunk.
+            overlap (int): The number of characters that should overlap between consecutive chunks.
+        """
+        self.text = text
+        self.chunk_size = chunk_size
+        self.overlap = overlap
+
+    def get_chunks(self):
+        """
+        Generates the text chunks based on the specified chunk size and overlap.
+
+        Returns:
+            list[str]: A list of chunked text segments.
+        """
+        chunks = []
+        start = 0
+        while start < len(self.text):
+            # Calculate end index of the chunk
+            end = start + self.chunk_size
+            # Append chunk to the list
+            chunks.append(self.text[start:end])
+            # Update start index for the next chunk
+            start = end - self.overlap if self.overlap < self.chunk_size else start + 1
+            # Prevent infinite loop in case overlap is not less than chunk_size
+            if self.chunk_size <= self.overlap:
+                raise ValueError(
+                    "Overlap must be less than chunk size to prevent infinite loops."
+                )
+        return chunks
+
+
+import re
+
+
+class RecursiveCharacterTextSplitter:
+    def __init__(
+        self,
+        separators,
+        chunk_size,
+        chunk_overlap,
+        length_function=len,
+        keep_separator=False,
+    ):
+        self.separators = separators
+        self.chunk_size = chunk_size
+        self.chunk_overlap = chunk_overlap
+        self.length_function = length_function
+        self.keep_separator = keep_separator
+
+    def split_text(self, text, depth=0):
+        if depth == len(self.separators):
+            return self._split_into_fixed_size(text)
+
+        current_separator = self.separators[depth]
+        if current_separator == "":
+            return list(text)
+
+        if self.keep_separator:
+            # Use regex to keep separators with the text
+            pieces = re.split(f"({re.escape(current_separator)})", text)
+            # Reattach separators to the chunks
+            pieces = [
+                (
+                    pieces[i] + pieces[i + 1]
+                    if i + 1 < len(pieces) and pieces[i + 1] == current_separator
+                    else pieces[i]
+                )
+                for i in range(0, len(pieces), 2)
+            ]
+        else:
+            pieces = text.split(current_separator)
+
+        refined_pieces = []
+
+        for piece in pieces:
+            if self.length_function(piece) > self.chunk_size:
+                refined_pieces.extend(self.split_text(piece, depth + 1))
+            else:
+                refined_pieces.append(piece)
+
+        return self._merge_pieces(refined_pieces) if depth == 0 else refined_pieces
+
+    def _split_into_fixed_size(self, text):
+        size = self.chunk_size
+        overlap = self.chunk_overlap
+        chunks = [text[i : i + size] for i in range(0, len(text), size - overlap)]
+        if chunks and len(chunks[-1]) < overlap:
+            chunks[-2] += chunks[-1]
+            chunks.pop()
+        return chunks
+
+    def _merge_pieces(self, pieces):
+        merged = []
+        current_chunk = pieces[0]
+
+        for piece in pieces[1:]:
+            if self.length_function(current_chunk + piece) <= self.chunk_size:
+                current_chunk += piece
+            else:
+                merged.append(current_chunk)
+                if len(current_chunk) == self.chunk_size:
+                    current_chunk = current_chunk[-self.chunk_overlap :] + piece
+                else:
+                    current_chunk = piece
+
+        merged.append(current_chunk)
+        return merged
```

### Comparing `llama_cpp_agent-0.1.3/src/llama_cpp_agent/structured_output_agent.py` & `llama_cpp_agent-0.1.4/src/llama_cpp_agent/structured_output_agent.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,241 +1,241 @@
-import json
-from copy import copy
-from typing import Type, Callable, Union
-
-from llama_cpp import Llama, LlamaGrammar
-from pydantic import BaseModel
-
-from .llm_agent import LlamaCppAgent, StreamingResponse
-from .llm_prompt_template import PromptTemplate
-from .llm_settings import LlamaLLMGenerationSettings, LlamaLLMSettings
-from .output_parser import extract_object_from_response
-from .messages_formatter import MessagesFormatterType, MessagesFormatter
-from .gbnf_grammar_generator.gbnf_grammar_from_pydantic_models import (
-    generate_gbnf_grammar_and_documentation,
-)
-from .providers.llama_cpp_endpoint_provider import (
-    LlamaCppEndpointSettings,
-    LlamaCppGenerationSettings,
-)
-from .providers.openai_endpoint_provider import (
-    OpenAIGenerationSettings,
-    OpenAIEndpointSettings,
-)
-
-
-class StructuredOutputAgent:
-    """
-    An agent that creates structured output based on pydantic models from unstructured text.
-
-    Args:
-        llama_llm (Union[Llama, LlamaLLMSettings, LlamaCppEndpointSettings, OpenAIEndpointSettings]): An instance of Llama, LlamaLLMSettings, LlamaCppServerLLMSettings, OpenAIEndpointSettings as LLM.
-        llama_generation_settings (Union[LlamaLLMGenerationSettings, LlamaCppGenerationSettings, OpenAIGenerationSettings]): Generation settings for Llama or LlamaCppServer.
-        messages_formatter_type (MessagesFormatterType): Type of messages formatter.
-        custom_messages_formatter (MessagesFormatter): Custom messages formatter.
-        streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
-        debug_output (bool): Enable debug output.
-
-    Attributes:
-        llama_generation_settings (Union[LlamaLLMGenerationSettings, LlamaCppServerGenerationSettings]): Generation settings for Llama or LlamaCppServer.
-        grammar_cache (dict): Cache for generated grammars.
-        system_prompt_template (PromptTemplate): Template for the system prompt.
-        creation_prompt_template (PromptTemplate): Template for the creation prompt.
-        llama_cpp_agent (LlamaCppAgent): LlamaCppAgent instance for interaction.
-        streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
-
-    Methods:
-        save(file_path: str): Save the agent's state to a file.
-        load_from_file(file_path: str, llama_llm, streaming_callback) -> StructuredOutputAgent: Load the agent's state from a file.
-        load_from_dict(agent_dict: dict) -> StructuredOutputAgent: Load the agent's state from a dictionary.
-        as_dict() -> dict: Convert the agent's state to a dictionary.
-        create_object(model: Type[BaseModel], data: str = "") -> object: Create an object of the given model from the given data.
-
-    """
-
-    def __init__(
-        self,
-        llama_llm: Union[
-            Llama, LlamaLLMSettings, LlamaCppEndpointSettings, OpenAIEndpointSettings
-        ],
-        llama_generation_settings: Union[
-            LlamaLLMGenerationSettings,
-            LlamaCppGenerationSettings,
-            OpenAIGenerationSettings,
-        ] = None,
-        messages_formatter_type: MessagesFormatterType = MessagesFormatterType.CHATML,
-        custom_messages_formatter: MessagesFormatter = None,
-        streaming_callback: Callable[[StreamingResponse], None] = None,
-        debug_output: bool = False,
-    ):
-        """
-        Initialize the StructuredOutputAgent.
-
-        Args:
-            llama_llm (Union[Llama, LlamaLLMSettings, LlamaCppEndpointSettings, OpenAIEndpointSettings]): An instance of Llama, LlamaLLMSettings, or LlamaCppServerLLMSettings as LLM.
-            llama_generation_settings (Union[LlamaLLMGenerationSettings, LlamaCppGenerationSettings, OpenAIGenerationSettings]): Generation settings for Llama or LlamaCppServer or OpenAIEndpoint.
-            messages_formatter_type (MessagesFormatterType): Type of messages formatter.
-            custom_messages_formatter (MessagesFormatter): Custom messages formatter.
-            streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
-            debug_output (bool): Enable debug output.
-        """
-        if llama_generation_settings is None:
-            if isinstance(llama_llm, Llama) or isinstance(llama_llm, LlamaLLMSettings):
-                llama_generation_settings = LlamaLLMGenerationSettings()
-            elif isinstance(llama_llm, OpenAIEndpointSettings):
-                llama_generation_settings = OpenAIGenerationSettings()
-            else:
-                llama_generation_settings = LlamaCppGenerationSettings()
-
-        if isinstance(
-            llama_generation_settings, LlamaLLMGenerationSettings
-        ) and isinstance(llama_llm, LlamaCppEndpointSettings):
-            raise Exception(
-                "Wrong generation settings for llama.cpp server endpoint, use LlamaCppServerGenerationSettings under llama_cpp_agent.providers.llama_cpp_server_provider!"
-            )
-        if (
-            isinstance(llama_llm, Llama) or isinstance(llama_llm, LlamaLLMSettings)
-        ) and isinstance(llama_generation_settings, LlamaCppGenerationSettings):
-            raise Exception(
-                "Wrong generation settings for llama-cpp-python, use LlamaLLMGenerationSettings under llama_cpp_agent.llm_settings!"
-            )
-
-        if isinstance(llama_llm, OpenAIEndpointSettings) and not isinstance(
-            llama_generation_settings, OpenAIGenerationSettings
-        ):
-            raise Exception(
-                "Wrong generation settings for OpenAI endpoint, use CompletionRequestSettings under llama_cpp_agent.providers.openai_endpoint_provider!"
-            )
-
-        self.llama_generation_settings = llama_generation_settings
-        self.grammar_cache = {}
-        self.system_prompt_template = PromptTemplate.from_string(
-            "You are an advanced AI agent. You are tasked to assist the user by creating structured output in JSON format.\n\n{documentation}"
-        )
-        self.creation_prompt_template = PromptTemplate.from_string(
-            "Create an JSON response based on the following input.\n\nInput:\n\n{user_input}"
-        )
-
-        self.llama_cpp_agent = LlamaCppAgent(
-            llama_llm,
-            debug_output=debug_output,
-            system_prompt="",
-            predefined_messages_formatter_type=messages_formatter_type,
-            custom_messages_formatter=custom_messages_formatter,
-        )
-        self.streaming_callback = streaming_callback
-
-    def save(self, file_path: str):
-        """
-        Save the agent's state to a file.
-
-        Args:
-            file_path (str): The path to the file.
-        """
-        with open(file_path, "w", encoding="utf-8") as file:
-            dic = copy(self.as_dict())
-            del dic["llama_cpp_agent"]
-            del dic["grammar_cache"]
-            del dic["system_prompt_template"]
-            del dic["creation_prompt_template"]
-            del dic["streaming_callback"]
-            dic["debug_output"] = self.llama_cpp_agent.debug_output
-            dic["llama_generation_settings"] = self.llama_generation_settings.as_dict()
-            dic["custom_messages_formatter"] = (
-                self.llama_cpp_agent.messages_formatter.as_dict()
-            )
-            json.dump(dic, file, indent=4)
-
-    @staticmethod
-    def load_from_file(
-        file_path: str,
-        llama_llm: Union[Llama, LlamaLLMSettings],
-        streaming_callback: Callable[[StreamingResponse], None] = None,
-    ) -> "StructuredOutputAgent":
-        """
-        Load the agent's state from a file.
-
-        Args:
-            file_path (str): The path to the file.
-            llama_llm (Union[Llama, LlamaLLMSettings, LlamaCppEndpointSettings]): An instance of Llama, LlamaLLMSettings, or LlamaCppServerLLMSettings as LLM.
-            streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
-
-        Returns:
-            StructuredOutputAgent: The loaded StructuredOutputAgent instance.
-        """
-        with open(file_path, "r", encoding="utf-8") as file:
-            loaded_agent = json.load(file)
-            loaded_agent["llama_llm"] = llama_llm
-            loaded_agent["streaming_callback"] = streaming_callback
-            loaded_agent["llama_generation_settings"] = (
-                LlamaLLMGenerationSettings.load_from_dict(
-                    loaded_agent["llama_generation_settings"]
-                )
-            )
-            loaded_agent["custom_messages_formatter"] = (
-                MessagesFormatter.load_from_dict(
-                    loaded_agent["custom_messages_formatter"]
-                )
-            )
-            return StructuredOutputAgent(**loaded_agent)
-
-    @staticmethod
-    def load_from_dict(agent_dict: dict) -> "StructuredOutputAgent":
-        """
-        Load the agent's state from a dictionary.
-
-        Args:
-            agent_dict (dict): The dictionary containing the agent's state.
-
-        Returns:
-            StructuredOutputAgent: The loaded StructuredOutputAgent instance.
-        """
-        return StructuredOutputAgent(**agent_dict)
-
-    def as_dict(self) -> dict:
-        """
-        Convert the agent's state to a dictionary.
-
-        Returns:
-            dict: The dictionary representation of the agent's state.
-        """
-        return self.__dict__
-
-    def create_object(self, model: Type[BaseModel], data: str = "") -> object:
-        """
-        Creates an object of the given model from the given data.
-
-        Args:
-            model (Type[BaseModel]): The model to create the object from.
-            data (str): The data to create the object from.
-
-        Returns:
-            object: The created object.
-        """
-        if model not in self.grammar_cache:
-            grammar, documentation = generate_gbnf_grammar_and_documentation(
-                [model],
-                model_prefix="Response Model",
-                fields_prefix="Response Model Field",
-            )
-
-            self.grammar_cache[model] = grammar, documentation
-        else:
-            grammar, documentation = self.grammar_cache[model]
-
-        system_prompt = self.system_prompt_template.generate_prompt(
-            {"documentation": documentation}
-        )
-        if data == "":
-            prompt = "Create a random JSON response based on the response model."
-        else:
-            prompt = self.creation_prompt_template.generate_prompt({"user_input": data})
-        response = self.llama_cpp_agent.get_chat_response(
-            prompt,
-            system_prompt=system_prompt,
-            grammar=grammar,
-            add_response_to_chat_history=False,
-            add_message_to_chat_history=False,
-            streaming_callback=self.streaming_callback,
-            **self.llama_generation_settings.as_dict(),
-        )
-        return extract_object_from_response(response, model)
+import json
+from copy import copy
+from typing import Type, Callable, Union
+
+from llama_cpp import Llama, LlamaGrammar
+from pydantic import BaseModel
+
+from .llm_agent import LlamaCppAgent, StreamingResponse
+from .llm_prompt_template import PromptTemplate
+from .llm_settings import LlamaLLMGenerationSettings, LlamaLLMSettings
+from .output_parser import extract_object_from_response
+from .messages_formatter import MessagesFormatterType, MessagesFormatter
+from .gbnf_grammar_generator.gbnf_grammar_from_pydantic_models import (
+    generate_gbnf_grammar_and_documentation,
+)
+from .providers.llama_cpp_endpoint_provider import (
+    LlamaCppEndpointSettings,
+    LlamaCppGenerationSettings,
+)
+from .providers.openai_endpoint_provider import (
+    OpenAIGenerationSettings,
+    OpenAIEndpointSettings,
+)
+
+
+class StructuredOutputAgent:
+    """
+    An agent that creates structured output based on pydantic models from unstructured text.
+
+    Args:
+        llama_llm (Union[Llama, LlamaLLMSettings, LlamaCppEndpointSettings, OpenAIEndpointSettings]): An instance of Llama, LlamaLLMSettings, LlamaCppServerLLMSettings, OpenAIEndpointSettings as LLM.
+        llama_generation_settings (Union[LlamaLLMGenerationSettings, LlamaCppGenerationSettings, OpenAIGenerationSettings]): Generation settings for Llama or LlamaCppServer.
+        messages_formatter_type (MessagesFormatterType): Type of messages formatter.
+        custom_messages_formatter (MessagesFormatter): Custom messages formatter.
+        streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
+        debug_output (bool): Enable debug output.
+
+    Attributes:
+        llama_generation_settings (Union[LlamaLLMGenerationSettings, LlamaCppServerGenerationSettings]): Generation settings for Llama or LlamaCppServer.
+        grammar_cache (dict): Cache for generated grammars.
+        system_prompt_template (PromptTemplate): Template for the system prompt.
+        creation_prompt_template (PromptTemplate): Template for the creation prompt.
+        llama_cpp_agent (LlamaCppAgent): LlamaCppAgent instance for interaction.
+        streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
+
+    Methods:
+        save(file_path: str): Save the agent's state to a file.
+        load_from_file(file_path: str, llama_llm, streaming_callback) -> StructuredOutputAgent: Load the agent's state from a file.
+        load_from_dict(agent_dict: dict) -> StructuredOutputAgent: Load the agent's state from a dictionary.
+        as_dict() -> dict: Convert the agent's state to a dictionary.
+        create_object(model: Type[BaseModel], data: str = "") -> object: Create an object of the given model from the given data.
+
+    """
+
+    def __init__(
+        self,
+        llama_llm: Union[
+            Llama, LlamaLLMSettings, LlamaCppEndpointSettings, OpenAIEndpointSettings
+        ],
+        llama_generation_settings: Union[
+            LlamaLLMGenerationSettings,
+            LlamaCppGenerationSettings,
+            OpenAIGenerationSettings,
+        ] = None,
+        messages_formatter_type: MessagesFormatterType = MessagesFormatterType.CHATML,
+        custom_messages_formatter: MessagesFormatter = None,
+        streaming_callback: Callable[[StreamingResponse], None] = None,
+        debug_output: bool = False,
+    ):
+        """
+        Initialize the StructuredOutputAgent.
+
+        Args:
+            llama_llm (Union[Llama, LlamaLLMSettings, LlamaCppEndpointSettings, OpenAIEndpointSettings]): An instance of Llama, LlamaLLMSettings, or LlamaCppServerLLMSettings as LLM.
+            llama_generation_settings (Union[LlamaLLMGenerationSettings, LlamaCppGenerationSettings, OpenAIGenerationSettings]): Generation settings for Llama or LlamaCppServer or OpenAIEndpoint.
+            messages_formatter_type (MessagesFormatterType): Type of messages formatter.
+            custom_messages_formatter (MessagesFormatter): Custom messages formatter.
+            streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
+            debug_output (bool): Enable debug output.
+        """
+        if llama_generation_settings is None:
+            if isinstance(llama_llm, Llama) or isinstance(llama_llm, LlamaLLMSettings):
+                llama_generation_settings = LlamaLLMGenerationSettings()
+            elif isinstance(llama_llm, OpenAIEndpointSettings):
+                llama_generation_settings = OpenAIGenerationSettings()
+            else:
+                llama_generation_settings = LlamaCppGenerationSettings()
+
+        if isinstance(
+            llama_generation_settings, LlamaLLMGenerationSettings
+        ) and isinstance(llama_llm, LlamaCppEndpointSettings):
+            raise Exception(
+                "Wrong generation settings for llama.cpp server endpoint, use LlamaCppServerGenerationSettings under llama_cpp_agent.providers.llama_cpp_server_provider!"
+            )
+        if (
+            isinstance(llama_llm, Llama) or isinstance(llama_llm, LlamaLLMSettings)
+        ) and isinstance(llama_generation_settings, LlamaCppGenerationSettings):
+            raise Exception(
+                "Wrong generation settings for llama-cpp-python, use LlamaLLMGenerationSettings under llama_cpp_agent.llm_settings!"
+            )
+
+        if isinstance(llama_llm, OpenAIEndpointSettings) and not isinstance(
+            llama_generation_settings, OpenAIGenerationSettings
+        ):
+            raise Exception(
+                "Wrong generation settings for OpenAI endpoint, use CompletionRequestSettings under llama_cpp_agent.providers.openai_endpoint_provider!"
+            )
+
+        self.llama_generation_settings = llama_generation_settings
+        self.grammar_cache = {}
+        self.system_prompt_template = PromptTemplate.from_string(
+            "You are an advanced AI agent. You are tasked to assist the user by creating structured output in JSON format.\n\n{documentation}"
+        )
+        self.creation_prompt_template = PromptTemplate.from_string(
+            "Create an JSON response based on the following input.\n\nInput:\n\n{user_input}"
+        )
+
+        self.llama_cpp_agent = LlamaCppAgent(
+            llama_llm,
+            debug_output=debug_output,
+            system_prompt="",
+            predefined_messages_formatter_type=messages_formatter_type,
+            custom_messages_formatter=custom_messages_formatter,
+        )
+        self.streaming_callback = streaming_callback
+
+    def save(self, file_path: str):
+        """
+        Save the agent's state to a file.
+
+        Args:
+            file_path (str): The path to the file.
+        """
+        with open(file_path, "w", encoding="utf-8") as file:
+            dic = copy(self.as_dict())
+            del dic["llama_cpp_agent"]
+            del dic["grammar_cache"]
+            del dic["system_prompt_template"]
+            del dic["creation_prompt_template"]
+            del dic["streaming_callback"]
+            dic["debug_output"] = self.llama_cpp_agent.debug_output
+            dic["llama_generation_settings"] = self.llama_generation_settings.as_dict()
+            dic["custom_messages_formatter"] = (
+                self.llama_cpp_agent.messages_formatter.as_dict()
+            )
+            json.dump(dic, file, indent=4)
+
+    @staticmethod
+    def load_from_file(
+        file_path: str,
+        llama_llm: Union[Llama, LlamaLLMSettings],
+        streaming_callback: Callable[[StreamingResponse], None] = None,
+    ) -> "StructuredOutputAgent":
+        """
+        Load the agent's state from a file.
+
+        Args:
+            file_path (str): The path to the file.
+            llama_llm (Union[Llama, LlamaLLMSettings, LlamaCppEndpointSettings]): An instance of Llama, LlamaLLMSettings, or LlamaCppServerLLMSettings as LLM.
+            streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
+
+        Returns:
+            StructuredOutputAgent: The loaded StructuredOutputAgent instance.
+        """
+        with open(file_path, "r", encoding="utf-8") as file:
+            loaded_agent = json.load(file)
+            loaded_agent["llama_llm"] = llama_llm
+            loaded_agent["streaming_callback"] = streaming_callback
+            loaded_agent["llama_generation_settings"] = (
+                LlamaLLMGenerationSettings.load_from_dict(
+                    loaded_agent["llama_generation_settings"]
+                )
+            )
+            loaded_agent["custom_messages_formatter"] = (
+                MessagesFormatter.load_from_dict(
+                    loaded_agent["custom_messages_formatter"]
+                )
+            )
+            return StructuredOutputAgent(**loaded_agent)
+
+    @staticmethod
+    def load_from_dict(agent_dict: dict) -> "StructuredOutputAgent":
+        """
+        Load the agent's state from a dictionary.
+
+        Args:
+            agent_dict (dict): The dictionary containing the agent's state.
+
+        Returns:
+            StructuredOutputAgent: The loaded StructuredOutputAgent instance.
+        """
+        return StructuredOutputAgent(**agent_dict)
+
+    def as_dict(self) -> dict:
+        """
+        Convert the agent's state to a dictionary.
+
+        Returns:
+            dict: The dictionary representation of the agent's state.
+        """
+        return self.__dict__
+
+    def create_object(self, model: Type[BaseModel], data: str = "") -> object:
+        """
+        Creates an object of the given model from the given data.
+
+        Args:
+            model (Type[BaseModel]): The model to create the object from.
+            data (str): The data to create the object from.
+
+        Returns:
+            object: The created object.
+        """
+        if model not in self.grammar_cache:
+            grammar, documentation = generate_gbnf_grammar_and_documentation(
+                [model],
+                model_prefix="Response Model",
+                fields_prefix="Response Model Field",
+            )
+
+            self.grammar_cache[model] = grammar, documentation
+        else:
+            grammar, documentation = self.grammar_cache[model]
+
+        system_prompt = self.system_prompt_template.generate_prompt(
+            {"documentation": documentation}
+        )
+        if data == "":
+            prompt = "Create a random JSON response based on the response model."
+        else:
+            prompt = self.creation_prompt_template.generate_prompt({"user_input": data})
+        response = self.llama_cpp_agent.get_chat_response(
+            prompt,
+            system_prompt=system_prompt,
+            grammar=grammar,
+            add_response_to_chat_history=False,
+            add_message_to_chat_history=False,
+            streaming_callback=self.streaming_callback,
+            **self.llama_generation_settings.as_dict(),
+        )
+        return extract_object_from_response(response, model)
```

### Comparing `llama_cpp_agent-0.1.3/src/llama_cpp_agent.egg-info/SOURCES.txt` & `llama_cpp_agent-0.1.4/src/llama_cpp_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

