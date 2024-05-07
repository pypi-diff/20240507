# Comparing `tmp/llm-bedrock-meta-0.1.7.tar.gz` & `tmp/llm_bedrock_meta-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-bedrock-meta-0.1.7.tar", last modified: Wed Nov 29 19:27:44 2023, max compression
+gzip compressed data, was "llm_bedrock_meta-0.1.8.tar", last modified: Tue May  7 12:58:51 2024, max compression
```

## Comparing `llm-bedrock-meta-0.1.7.tar` & `llm_bedrock_meta-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:27:44.229434 llm-bedrock-meta-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2023-11-29 19:27:32.000000 llm-bedrock-meta-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2023-11-29 19:27:44.229434 llm-bedrock-meta-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2023-11-29 19:27:32.000000 llm-bedrock-meta-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:27:44.229434 llm-bedrock-meta-0.1.7/llm_bedrock_meta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2023-11-29 19:27:44.000000 llm-bedrock-meta-0.1.7/llm_bedrock_meta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-11-29 19:27:44.000000 llm-bedrock-meta-0.1.7/llm_bedrock_meta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-29 19:27:44.000000 llm-bedrock-meta-0.1.7/llm_bedrock_meta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-11-29 19:27:44.000000 llm-bedrock-meta-0.1.7/llm_bedrock_meta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-11-29 19:27:44.000000 llm-bedrock-meta-0.1.7/llm_bedrock_meta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-11-29 19:27:44.000000 llm-bedrock-meta-0.1.7/llm_bedrock_meta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2023-11-29 19:27:32.000000 llm-bedrock-meta-0.1.7/llm_bedrock_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2023-11-29 19:27:32.000000 llm-bedrock-meta-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-29 19:27:44.229434 llm-bedrock-meta-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:27:44.229434 llm-bedrock-meta-0.1.7/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2023-11-29 19:27:32.000000 llm-bedrock-meta-0.1.7/test/test_bedrock_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:58:51.164744 llm_bedrock_meta-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-07 12:58:42.000000 llm_bedrock_meta-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-07 12:58:51.164744 llm_bedrock_meta-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-07 12:58:42.000000 llm_bedrock_meta-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:58:51.164744 llm_bedrock_meta-0.1.8/llm_bedrock_meta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-07 12:58:51.000000 llm_bedrock_meta-0.1.8/llm_bedrock_meta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-07 12:58:51.000000 llm_bedrock_meta-0.1.8/llm_bedrock_meta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 12:58:51.000000 llm_bedrock_meta-0.1.8/llm_bedrock_meta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 12:58:51.000000 llm_bedrock_meta-0.1.8/llm_bedrock_meta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 12:58:51.000000 llm_bedrock_meta-0.1.8/llm_bedrock_meta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 12:58:51.000000 llm_bedrock_meta-0.1.8/llm_bedrock_meta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8258 2024-05-07 12:58:42.000000 llm_bedrock_meta-0.1.8/llm_bedrock_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-07 12:58:42.000000 llm_bedrock_meta-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 12:58:51.164744 llm_bedrock_meta-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:58:51.164744 llm_bedrock_meta-0.1.8/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-07 12:58:42.000000 llm_bedrock_meta-0.1.8/test/test_bedrock_meta.py
```

### Comparing `llm-bedrock-meta-0.1.7/LICENSE` & `llm_bedrock_meta-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-bedrock-meta-0.1.7/PKG-INFO` & `llm_bedrock_meta-0.1.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-bedrock-meta
-Version: 0.1.7
+Version: 0.1.8
 Summary: LLM plugin for Meta Llama2 on AWS Bedrock
 Author: Fabian Labat
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/flabat/llm-bedrock-meta
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,15 +16,15 @@
 # llm-bedrock-meta
 
 [![PyPI](https://img.shields.io/pypi/v/llm-bedrock-meta.svg)](https://pypi.org/project/llm-bedrock-meta/)
 [![Changelog](https://img.shields.io/github/v/release/flabat/llm-bedrock-meta?include_prereleases&label=changelog)](https://github.com/flabat/llm-bedrock-meta/releases)
 [![Tests](https://github.com/flabat/llm-bedrock-meta/workflows/Test/badge.svg)](https://github.com/flabat/llm-bedrock-meta/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/flabat/llm-bedrock-meta/blob/main/LICENSE)
 
-Plugin for [LLM](https://llm.datasette.io/) adding support for Meta LLama 2's  models in Amazon Bedrock
+Plugin for [LLM](https://llm.datasette.io/) adding support for Meta LLama 2 and 3 models in Amazon Bedrock
 
 ## Installation
 
 Install this plugin in the same environment as LLM. From the current directory
 ```bash
 llm install llm-bedrock-meta
 ```
@@ -37,41 +37,49 @@
 ```bash
 export AWS_DEFAULT_REGION=us-west-2
 export AWS_PROFILE=personal
 ```
 
 ## Usage
 
-This plugin adds model called `bedrock-llama2-13b`. You can also use it with the alias `bl2`.
+This plugin adds models called `bedrock-llama2-13b`, `bedrock-llama2-70b`, `bedrock-llama3-8b-instruct`, and `bedrock-llama3-70b-instruct`. You can also use it with the aliases like `bl2` or `bl2-70`.
 
 You can query them like this:
 
 ```bash
-llm -m bedrock-llama2-13b "Ten great names for a new space station"
+llm -m bl3-70-i "Ten great names for a new space station"
 ```
 
 ```bash
-llm -m bl2 "Ten great names for a new space station"
+llm -m bl3-70-i "Ten great names for a new space station"
 ```
 
 You can also chat with the model:
 
 ```bash
-llm chat -m bl2
+llm chat -m bl3-70-i
 ```
 
 ## Options
 
 - `-o max_gen_len 1024`, default 2_048: The maximum number of tokens to generate before stopping.
 - `-o verbose 1`, default 0: Output more verbose logging.
 - `-o temperature 0.8`, default 0.6: Use a lower value to decrease randomness in the response.
 - `top_p`, default 0.9: Use a lower value to ignore less probable options. Set to 0 or 1.0 to disable.
 
 Use like this:
 ```bash
-llm -m bedrock-llama2-13b -o max_gen_len 20 "Sing me the alphabet"
- Here is the alphabet song:
+llm -m bl3-70-i -o max_gen_len 20 "Sing me the alphabet"
+ Ah, ah, ah! Here's the alphabet song for you:
 
-A B C D E F G
-H I J
+
+A, B, C, D, E, F, G,
+H, I, J, K, L, M, N, O,
+P, Q, R, S, T, U, V, W,
+X, Y, Z,
+Now I know my ABCs,
+Next time won't you sing with me?
+
+
+Hope that brought a smile to your face!
 ```
```

### Comparing `llm-bedrock-meta-0.1.7/llm_bedrock_meta.egg-info/PKG-INFO` & `llm_bedrock_meta-0.1.8/llm_bedrock_meta.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-bedrock-meta
-Version: 0.1.7
+Version: 0.1.8
 Summary: LLM plugin for Meta Llama2 on AWS Bedrock
 Author: Fabian Labat
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/flabat/llm-bedrock-meta
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,15 +16,15 @@
 # llm-bedrock-meta
 
 [![PyPI](https://img.shields.io/pypi/v/llm-bedrock-meta.svg)](https://pypi.org/project/llm-bedrock-meta/)
 [![Changelog](https://img.shields.io/github/v/release/flabat/llm-bedrock-meta?include_prereleases&label=changelog)](https://github.com/flabat/llm-bedrock-meta/releases)
 [![Tests](https://github.com/flabat/llm-bedrock-meta/workflows/Test/badge.svg)](https://github.com/flabat/llm-bedrock-meta/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/flabat/llm-bedrock-meta/blob/main/LICENSE)
 
-Plugin for [LLM](https://llm.datasette.io/) adding support for Meta LLama 2's  models in Amazon Bedrock
+Plugin for [LLM](https://llm.datasette.io/) adding support for Meta LLama 2 and 3 models in Amazon Bedrock
 
 ## Installation
 
 Install this plugin in the same environment as LLM. From the current directory
 ```bash
 llm install llm-bedrock-meta
 ```
@@ -37,41 +37,49 @@
 ```bash
 export AWS_DEFAULT_REGION=us-west-2
 export AWS_PROFILE=personal
 ```
 
 ## Usage
 
-This plugin adds model called `bedrock-llama2-13b`. You can also use it with the alias `bl2`.
+This plugin adds models called `bedrock-llama2-13b`, `bedrock-llama2-70b`, `bedrock-llama3-8b-instruct`, and `bedrock-llama3-70b-instruct`. You can also use it with the aliases like `bl2` or `bl2-70`.
 
 You can query them like this:
 
 ```bash
-llm -m bedrock-llama2-13b "Ten great names for a new space station"
+llm -m bl3-70-i "Ten great names for a new space station"
 ```
 
 ```bash
-llm -m bl2 "Ten great names for a new space station"
+llm -m bl3-70-i "Ten great names for a new space station"
 ```
 
 You can also chat with the model:
 
 ```bash
-llm chat -m bl2
+llm chat -m bl3-70-i
 ```
 
 ## Options
 
 - `-o max_gen_len 1024`, default 2_048: The maximum number of tokens to generate before stopping.
 - `-o verbose 1`, default 0: Output more verbose logging.
 - `-o temperature 0.8`, default 0.6: Use a lower value to decrease randomness in the response.
 - `top_p`, default 0.9: Use a lower value to ignore less probable options. Set to 0 or 1.0 to disable.
 
 Use like this:
 ```bash
-llm -m bedrock-llama2-13b -o max_gen_len 20 "Sing me the alphabet"
- Here is the alphabet song:
+llm -m bl3-70-i -o max_gen_len 20 "Sing me the alphabet"
+ Ah, ah, ah! Here's the alphabet song for you:
 
-A B C D E F G
-H I J
+
+A, B, C, D, E, F, G,
+H, I, J, K, L, M, N, O,
+P, Q, R, S, T, U, V, W,
+X, Y, Z,
+Now I know my ABCs,
+Next time won't you sing with me?
+
+
+Hope that brought a smile to your face!
 ```
```

### Comparing `llm-bedrock-meta-0.1.7/pyproject.toml` & `llm_bedrock_meta-0.1.8/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llm-bedrock-meta"
-version = "0.1.7"
+version = "0.1.8"
 
 description = "LLM plugin for Meta Llama2 on AWS Bedrock"
 readme = "README.md"
 authors = [{name = "Fabian Labat"}]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
@@ -18,8 +18,8 @@
 [project.urls]
 Homepage = "https://github.com/flabat/llm-bedrock-meta"
 
 [project.entry-points.llm]
 bedrock_llama = "llm_bedrock_meta"
 
 [project.optional-dependencies]
-test = ["pytest"]
+test = ["pytest"]
```

### Comparing `llm-bedrock-meta-0.1.7/test/test_bedrock_meta.py` & `llm_bedrock_meta-0.1.8/test/test_bedrock_meta.py`

 * *Files identical despite different names*

