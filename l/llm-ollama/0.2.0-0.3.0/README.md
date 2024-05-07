# Comparing `tmp/llm-ollama-0.2.0.tar.gz` & `tmp/llm_ollama-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-ollama-0.2.0.tar", last modified: Sun Jan 28 07:37:19 2024, max compression
+gzip compressed data, was "llm_ollama-0.3.0.tar", last modified: Tue May  7 08:20:54 2024, max compression
```

## Comparing `llm-ollama-0.2.0.tar` & `llm_ollama-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 07:37:19.589918 llm-ollama-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-28 07:37:11.000000 llm-ollama-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-01-28 07:37:19.589918 llm-ollama-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-01-28 07:37:11.000000 llm-ollama-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 07:37:19.589918 llm-ollama-0.2.0/llm_ollama.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-01-28 07:37:19.000000 llm-ollama-0.2.0/llm_ollama.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-01-28 07:37:19.000000 llm-ollama-0.2.0/llm_ollama.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-28 07:37:19.000000 llm-ollama-0.2.0/llm_ollama.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-28 07:37:19.000000 llm-ollama-0.2.0/llm_ollama.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-28 07:37:19.000000 llm-ollama-0.2.0/llm_ollama.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-28 07:37:19.000000 llm-ollama-0.2.0/llm_ollama.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-01-28 07:37:11.000000 llm-ollama-0.2.0/llm_ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-01-28 07:37:11.000000 llm-ollama-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-28 07:37:19.589918 llm-ollama-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 07:37:19.589918 llm-ollama-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-01-28 07:37:11.000000 llm-ollama-0.2.0/tests/test_ollama.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:20:54.749034 llm_ollama-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 08:20:49.000000 llm_ollama-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-07 08:20:54.749034 llm_ollama-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-07 08:20:49.000000 llm_ollama-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:20:54.749034 llm_ollama-0.3.0/llm_ollama.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-07 08:20:54.000000 llm_ollama-0.3.0/llm_ollama.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-07 08:20:54.000000 llm_ollama-0.3.0/llm_ollama.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 08:20:54.000000 llm_ollama-0.3.0/llm_ollama.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 08:20:54.000000 llm_ollama-0.3.0/llm_ollama.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 08:20:54.000000 llm_ollama-0.3.0/llm_ollama.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 08:20:54.000000 llm_ollama-0.3.0/llm_ollama.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-07 08:20:49.000000 llm_ollama-0.3.0/llm_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-07 08:20:49.000000 llm_ollama-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 08:20:54.749034 llm_ollama-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:20:54.749034 llm_ollama-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-07 08:20:49.000000 llm_ollama-0.3.0/tests/test_ollama.py
```

### Comparing `llm-ollama-0.2.0/LICENSE` & `llm_ollama-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-ollama-0.2.0/PKG-INFO` & `llm_ollama-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-ollama
-Version: 0.2.0
+Version: 0.3.0
 Summary: LLM plugin providing access to local Ollama models
 Author: Sergey Alexandrov
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/taketwo/llm-ollama
 Project-URL: Changelog, https://github.com/taketwo/llm-ollama/releases
 Project-URL: Issues, https://github.com/taketwo/llm-ollama/issues
 Project-URL: CI, https://github.com/taketwo/llm-ollama/actions
@@ -83,17 +83,20 @@
 ...
 
 Ollama: stable-code:3b (aliases: stable-code:code, stable-code:latest, stable-code)
 ```
 
 ## Model options
 
-All models accept the following options, using `-o name value` syntax:
+All models accept [Ollama modelfile parameters](https://github.com/ollama/ollama/blob/main/docs/modelfile.md#parameter) as options. Use the `-o name value` syntax to specify them, for example:
 
-- `-o temperature 0.8`: The temperature of the model. Increasing the temperature will make the model answer more creatively.
+- `-o temperature 0.8`: set the temperature of the model
+- `-o num_ctx 256000`: set the size of the context window used to generate the next token
+
+See the referenced page for the complete list with descriptions and default values.
 
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 
 ```bash
 cd llm-ollama
```

### Comparing `llm-ollama-0.2.0/README.md` & `llm_ollama-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -64,17 +64,20 @@
 ...
 
 Ollama: stable-code:3b (aliases: stable-code:code, stable-code:latest, stable-code)
 ```
 
 ## Model options
 
-All models accept the following options, using `-o name value` syntax:
+All models accept [Ollama modelfile parameters](https://github.com/ollama/ollama/blob/main/docs/modelfile.md#parameter) as options. Use the `-o name value` syntax to specify them, for example:
 
-- `-o temperature 0.8`: The temperature of the model. Increasing the temperature will make the model answer more creatively.
+- `-o temperature 0.8`: set the temperature of the model
+- `-o num_ctx 256000`: set the size of the context window used to generate the next token
+
+See the referenced page for the complete list with descriptions and default values.
 
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 
 ```bash
 cd llm-ollama
```

### Comparing `llm-ollama-0.2.0/llm_ollama.egg-info/PKG-INFO` & `llm_ollama-0.3.0/llm_ollama.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-ollama
-Version: 0.2.0
+Version: 0.3.0
 Summary: LLM plugin providing access to local Ollama models
 Author: Sergey Alexandrov
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/taketwo/llm-ollama
 Project-URL: Changelog, https://github.com/taketwo/llm-ollama/releases
 Project-URL: Issues, https://github.com/taketwo/llm-ollama/issues
 Project-URL: CI, https://github.com/taketwo/llm-ollama/actions
@@ -83,17 +83,20 @@
 ...
 
 Ollama: stable-code:3b (aliases: stable-code:code, stable-code:latest, stable-code)
 ```
 
 ## Model options
 
-All models accept the following options, using `-o name value` syntax:
+All models accept [Ollama modelfile parameters](https://github.com/ollama/ollama/blob/main/docs/modelfile.md#parameter) as options. Use the `-o name value` syntax to specify them, for example:
 
-- `-o temperature 0.8`: The temperature of the model. Increasing the temperature will make the model answer more creatively.
+- `-o temperature 0.8`: set the temperature of the model
+- `-o num_ctx 256000`: set the size of the context window used to generate the next token
+
+See the referenced page for the complete list with descriptions and default values.
 
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 
 ```bash
 cd llm-ollama
```

### Comparing `llm-ollama-0.2.0/pyproject.toml` & `llm_ollama-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llm-ollama"
-version = "0.2.0"
+version = "0.3.0"
 description = "LLM plugin providing access to local Ollama models"
 readme = "README.md"
 authors = [{ name = "Sergey Alexandrov" }]
 license = { text = "Apache-2.0" }
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 dependencies = ["llm", "ollama"]
 requires-python = ">=3.8"
```

### Comparing `llm-ollama-0.2.0/tests/test_ollama.py` & `llm_ollama-0.3.0/tests/test_ollama.py`

 * *Files identical despite different names*

