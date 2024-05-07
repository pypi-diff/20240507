# Comparing `tmp/promptflow_custom_tools-0.0.5.tar.gz` & `tmp/promptflow_custom_tools-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptflow_custom_tools-0.0.5.tar", last modified: Tue Apr 23 13:34:41 2024, max compression
+gzip compressed data, was "promptflow_custom_tools-0.0.6.tar", last modified: Tue May  7 17:48:26 2024, max compression
```

## Comparing `promptflow_custom_tools-0.0.5.tar` & `promptflow_custom_tools-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 13:34:41.841949 promptflow_custom_tools-0.0.5/
--rw-rw-rw-   0        0        0     1072 2024-04-22 20:09:19.000000 promptflow_custom_tools-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       44 2024-04-22 20:28:40.000000 promptflow_custom_tools-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      128 2024-04-23 13:34:41.841949 promptflow_custom_tools-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       25 2024-04-22 20:28:57.000000 promptflow_custom_tools-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 13:34:41.765092 promptflow_custom_tools-0.0.5/promptflow_custom_tools/
--rw-rw-rw-   0        0        0       82 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.5/promptflow_custom_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 13:34:41.818955 promptflow_custom_tools-0.0.5/promptflow_custom_tools/tools/
--rw-rw-rw-   0        0        0       82 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.5/promptflow_custom_tools/tools/__init__.py
--rw-rw-rw-   0        0        0     1894 2024-04-22 21:17:52.000000 promptflow_custom_tools-0.0.5/promptflow_custom_tools/tools/claude.py
--rw-rw-rw-   0        0        0      553 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.5/promptflow_custom_tools/tools/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-23 13:34:41.828702 promptflow_custom_tools-0.0.5/promptflow_custom_tools/yamls/
--rw-rw-rw-   0        0        0     6657 2024-04-22 20:11:06.000000 promptflow_custom_tools-0.0.5/promptflow_custom_tools/yamls/claude.yaml
-drwxrwxrwx   0        0        0        0 2024-04-23 13:34:41.785743 promptflow_custom_tools-0.0.5/promptflow_custom_tools.egg-info/
--rw-rw-rw-   0        0        0      128 2024-04-23 13:34:41.000000 promptflow_custom_tools-0.0.5/promptflow_custom_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      560 2024-04-23 13:34:41.000000 promptflow_custom_tools-0.0.5/promptflow_custom_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 13:34:41.000000 promptflow_custom_tools-0.0.5/promptflow_custom_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-04-23 13:34:41.000000 promptflow_custom_tools-0.0.5/promptflow_custom_tools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       38 2024-04-23 13:34:41.000000 promptflow_custom_tools-0.0.5/promptflow_custom_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2024-04-23 13:34:41.000000 promptflow_custom_tools-0.0.5/promptflow_custom_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 13:34:41.843147 promptflow_custom_tools-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      513 2024-04-23 13:34:21.000000 promptflow_custom_tools-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 13:34:41.840949 promptflow_custom_tools-0.0.5/tests/
--rw-rw-rw-   0        0        0        0 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.5/tests/__init__.py
--rw-rw-rw-   0        0        0      709 2024-04-22 20:27:24.000000 promptflow_custom_tools-0.0.5/tests/test_claude.py
+drwxrwxrwx   0        0        0        0 2024-05-07 17:48:26.605556 promptflow_custom_tools-0.0.6/
+-rw-rw-rw-   0        0        0     1072 2024-04-22 20:09:19.000000 promptflow_custom_tools-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       44 2024-04-22 20:28:40.000000 promptflow_custom_tools-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      128 2024-05-07 17:48:26.605556 promptflow_custom_tools-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       25 2024-04-22 20:28:57.000000 promptflow_custom_tools-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 17:48:26.569035 promptflow_custom_tools-0.0.6/promptflow_custom_tools/
+-rw-rw-rw-   0        0        0       82 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.6/promptflow_custom_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 17:48:26.591624 promptflow_custom_tools-0.0.6/promptflow_custom_tools/tools/
+-rw-rw-rw-   0        0        0       82 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.6/promptflow_custom_tools/tools/__init__.py
+-rw-rw-rw-   0        0        0     2342 2024-04-25 19:01:57.000000 promptflow_custom_tools-0.0.6/promptflow_custom_tools/tools/claude.py
+-rw-rw-rw-   0        0        0      553 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.6/promptflow_custom_tools/tools/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-07 17:48:26.603401 promptflow_custom_tools-0.0.6/promptflow_custom_tools/yamls/
+-rw-rw-rw-   0        0        0     6776 2024-05-07 17:47:45.000000 promptflow_custom_tools-0.0.6/promptflow_custom_tools/yamls/claude.yaml
+drwxrwxrwx   0        0        0        0 2024-05-07 17:48:26.590118 promptflow_custom_tools-0.0.6/promptflow_custom_tools.egg-info/
+-rw-rw-rw-   0        0        0      128 2024-05-07 17:48:26.000000 promptflow_custom_tools-0.0.6/promptflow_custom_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      560 2024-05-07 17:48:26.000000 promptflow_custom_tools-0.0.6/promptflow_custom_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 17:48:26.000000 promptflow_custom_tools-0.0.6/promptflow_custom_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-07 17:48:26.000000 promptflow_custom_tools-0.0.6/promptflow_custom_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       38 2024-05-07 17:48:26.000000 promptflow_custom_tools-0.0.6/promptflow_custom_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2024-05-07 17:48:26.000000 promptflow_custom_tools-0.0.6/promptflow_custom_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 17:48:26.605556 promptflow_custom_tools-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      513 2024-05-07 17:48:03.000000 promptflow_custom_tools-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 17:48:26.604548 promptflow_custom_tools-0.0.6/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.6/tests/__init__.py
+-rw-rw-rw-   0        0        0      709 2024-04-22 20:27:24.000000 promptflow_custom_tools-0.0.6/tests/test_claude.py
```

### Comparing `promptflow_custom_tools-0.0.5/LICENSE` & `promptflow_custom_tools-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `promptflow_custom_tools-0.0.5/promptflow_custom_tools/tools/claude.py` & `promptflow_custom_tools-0.0.6/promptflow_custom_tools/tools/claude.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,32 @@
     :type api_key: Secret
     :param api_base: The api base.
     :type api_base: String
     """
     api_key: Secret
     api_base: str = "This is a fake api base."
 
+def get_models():
+    result = [
+        {
+            "value":"claude-3-opus-20240229",
+            "display_value": "claude-3-opus-20240229",
+        },
+        {
+            "value":"claude-3-sonnet-20240229",
+            "display_value": "claude-3-sonnet-20240229",
+        },
+        {
+            "value":"claude-3-haiku-20240307",
+            "display_value": "claude-3-haiku-20240307",
+        }
+    ]
+
+    return result
+
 @tool
 def generate(
     connection: ClaudeConnection,
     prompt: PromptTemplate,
     model: str = "claude-3-opus-20240229",
     temperature: float  = 1,
     top_p: float = 1.0,
```

### Comparing `promptflow_custom_tools-0.0.5/promptflow_custom_tools/tools/utils.py` & `promptflow_custom_tools-0.0.6/promptflow_custom_tools/tools/utils.py`

 * *Files identical despite different names*

### Comparing `promptflow_custom_tools-0.0.5/promptflow_custom_tools/yamls/claude.yaml` & `promptflow_custom_tools-0.0.6/promptflow_custom_tools/yamls/claude.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -7,22 +7,26 @@
       type:
         - CustomConnection
       custom_type:
         - ClaudeConnection
     model:
       type:
         - string
+      enum:
+        - claude-3-opus-20240229
+        - claude-3-sonnet-20240229
+        - claude-3-haiku-20240307
       default: claude-3-opus-20240229
     temperature:
       type:
         - double
       default: '1'
     top_p:
       type:
         - double
-      default: '1.0'
     max_tokens:
       type:
         - int
+      default: '4096'
   description: Tool for interacting with Claude LLM
   module: promptflow_custom_tools.tools.claude
   function: generate
```

### Comparing `promptflow_custom_tools-0.0.5/promptflow_custom_tools.egg-info/SOURCES.txt` & `promptflow_custom_tools-0.0.6/promptflow_custom_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `promptflow_custom_tools-0.0.5/setup.py` & `promptflow_custom_tools-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 PACKAGE_NAME = "promptflow_custom_tools"
 
 setup(
     name=PACKAGE_NAME,
-    version="0.0.5",
+    version="0.0.6",
     description="This is my tools package",
     packages=find_packages(),
     entry_points={
         "package_tools": ["claude = promptflow_custom_tools.tools.utils:list_package_tools"],
     },
     include_package_data=True,   # This line tells setuptools to include files from MANIFEST.in
     install_requires=['promptflow', 'promptflow-tools', 'anthropic'],
```

### Comparing `promptflow_custom_tools-0.0.5/tests/test_claude.py` & `promptflow_custom_tools-0.0.6/tests/test_claude.py`

 * *Files identical despite different names*

