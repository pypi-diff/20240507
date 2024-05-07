# Comparing `tmp/botifyme-0.1.3.tar.gz` & `tmp/botifyme-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botifyme-0.1.3.tar", max compression
+gzip compressed data, was "botifyme-0.1.4.tar", max compression
```

## Comparing `botifyme-0.1.3.tar` & `botifyme-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2024-02-22 03:29:19.473931 botifyme-0.1.3/LICENSE
--rw-r--r--   0        0        0      443 2024-02-22 03:29:19.474338 botifyme-0.1.3/README.md
--rw-r--r--   0        0        0      162 2024-04-23 20:15:22.599781 botifyme-0.1.3/botifyme/__init__.py
--rw-r--r--   0        0        0     3008 2024-05-04 06:02:47.290817 botifyme-0.1.3/botifyme/__main__.py
--rw-r--r--   0        0        0     1438 2024-04-23 20:15:22.599920 botifyme-0.1.3/botifyme/agent.py
--rw-r--r--   0        0        0    11826 2024-05-04 06:02:47.291215 botifyme-0.1.3/botifyme/config.py
--rw-r--r--   0        0        0     1045 2024-02-22 03:29:19.476022 botifyme-0.1.3/botifyme/registry.py
--rw-r--r--   0        0        0     4075 2024-05-03 05:36:25.537048 botifyme-0.1.3/botifyme/runtime.py
--rw-r--r--   0        0        0      475 2024-04-23 20:15:22.600500 botifyme-0.1.3/botifyme/utils/__init__.py
--rw-r--r--   0        0        0     3533 2024-03-14 23:09:57.824589 botifyme-0.1.3/botifyme/utils/tools.py
--rw-r--r--   0        0        0     3640 2024-04-23 22:21:27.280737 botifyme-0.1.3/botifyme/workflow.py
--rw-r--r--   0        0        0      869 2024-05-06 23:14:46.509546 botifyme-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1594 1970-01-01 00:00:00.000000 botifyme-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-22 03:29:19.473931 botifyme-0.1.4/LICENSE
+-rw-r--r--   0        0        0      443 2024-02-22 03:29:19.474338 botifyme-0.1.4/README.md
+-rw-r--r--   0        0        0      162 2024-04-23 20:15:22.599781 botifyme-0.1.4/botifyme/__init__.py
+-rw-r--r--   0        0        0     3139 2024-05-07 06:53:36.557351 botifyme-0.1.4/botifyme/__main__.py
+-rw-r--r--   0        0        0     1438 2024-04-23 20:15:22.599920 botifyme-0.1.4/botifyme/agent.py
+-rw-r--r--   0        0        0    11826 2024-05-04 06:02:47.291215 botifyme-0.1.4/botifyme/config.py
+-rw-r--r--   0        0        0     1045 2024-02-22 03:29:19.476022 botifyme-0.1.4/botifyme/registry.py
+-rw-r--r--   0        0        0     4075 2024-05-03 05:36:25.537048 botifyme-0.1.4/botifyme/runtime.py
+-rw-r--r--   0        0        0      475 2024-04-23 20:15:22.600500 botifyme-0.1.4/botifyme/utils/__init__.py
+-rw-r--r--   0        0        0     3533 2024-03-14 23:09:57.824589 botifyme-0.1.4/botifyme/utils/tools.py
+-rw-r--r--   0        0        0     3640 2024-04-23 22:21:27.280737 botifyme-0.1.4/botifyme/workflow.py
+-rw-r--r--   0        0        0      869 2024-05-07 06:54:12.200782 botifyme-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1594 1970-01-01 00:00:00.000000 botifyme-0.1.4/PKG-INFO
```

### Comparing `botifyme-0.1.3/LICENSE` & `botifyme-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `botifyme-0.1.3/botifyme/__main__.py` & `botifyme-0.1.4/botifyme/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import os
 import argparse
 import json
 from botifyme.runtime import generate_config, load_modules_from_directory
 from botifyme.config import get_tool, tool_registry
+from pydantic import BaseModel
 
 
 def execute_tool(tool_name, tool_args, temp_dir=None):
-    print("Function name", tool_name)
-    print("Args", tool_args, type(tool_args))
-
     kwargs = json.loads(tool_args) if tool_args else {}
 
     current_directory = os.getcwd()
     load_modules_from_directory(current_directory)
 
-    print("writing to temp dir", temp_dir)
-
     for _, tool in tool_registry.items():
         if tool.name == tool_name:
             try:
                 output = tool.func(**kwargs)
 
-                print("Output from tool", output)
-                print("Output type", type(output))
-
                 # If output is a dictionary or a pydantic model, convert it to a JSON string.
                 if isinstance(output, dict) or hasattr(output, "json"):
                     with open(
                         os.path.join(temp_dir, "output.json"), "w", encoding="utf-8"
                     ) as f:
                         json.dump(output, f)
 
+                # If output is a pydantic model, convert it to a JSON string.
+                if isinstance(output, BaseModel):
+                    with open(
+                        os.path.join(temp_dir, "output.json"), "w", encoding="utf-8"
+                    ) as f:
+                        f.write(output.model_dump_json())
+
                 if isinstance(output, str):
                     with open(
                         os.path.join(temp_dir, "output.txt"), "w", encoding="utf-8"
                     ) as f:
                         f.write(output)
 
             except Exception as e:
```

### Comparing `botifyme-0.1.3/botifyme/agent.py` & `botifyme-0.1.4/botifyme/agent.py`

 * *Files identical despite different names*

### Comparing `botifyme-0.1.3/botifyme/config.py` & `botifyme-0.1.4/botifyme/config.py`

 * *Files identical despite different names*

### Comparing `botifyme-0.1.3/botifyme/registry.py` & `botifyme-0.1.4/botifyme/registry.py`

 * *Files identical despite different names*

### Comparing `botifyme-0.1.3/botifyme/runtime.py` & `botifyme-0.1.4/botifyme/runtime.py`

 * *Files identical despite different names*

### Comparing `botifyme-0.1.3/botifyme/utils/tools.py` & `botifyme-0.1.4/botifyme/utils/tools.py`

 * *Files identical despite different names*

### Comparing `botifyme-0.1.3/botifyme/workflow.py` & `botifyme-0.1.4/botifyme/workflow.py`

 * *Files identical despite different names*

### Comparing `botifyme-0.1.3/pyproject.toml` & `botifyme-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "botifyme"
-version = "0.1.3"
+version = "0.1.4"
 description = "Toolkit for building Autonomous AI agents"
 authors = ["Arun Reddy <arun@botifyme.dev>"]
 license = "Apache License 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `botifyme-0.1.3/PKG-INFO` & `botifyme-0.1.4/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botifyme
-Version: 0.1.3
+Version: 0.1.4
 Summary: Toolkit for building Autonomous AI agents
 License: Apache-2.0
 Author: Arun Reddy
 Author-email: arun@botifyme.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

