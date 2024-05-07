# Comparing `tmp/promptflow_custom_tools-0.0.6.tar.gz` & `tmp/promptflow_custom_tools-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptflow_custom_tools-0.0.6.tar", last modified: Tue May  7 17:48:26 2024, max compression
+gzip compressed data, was "promptflow_custom_tools-0.0.7.tar", last modified: Tue May  7 18:13:37 2024, max compression
```

## Comparing `promptflow_custom_tools-0.0.6.tar` & `promptflow_custom_tools-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 17:48:26.605556 promptflow_custom_tools-0.0.6/
--rw-rw-rw-   0        0        0     1072 2024-04-22 20:09:19.000000 promptflow_custom_tools-0.0.6/LICENSE
--rw-rw-rw-   0        0        0       44 2024-04-22 20:28:40.000000 promptflow_custom_tools-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      128 2024-05-07 17:48:26.605556 promptflow_custom_tools-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       25 2024-04-22 20:28:57.000000 promptflow_custom_tools-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 17:48:26.569035 promptflow_custom_tools-0.0.6/promptflow_custom_tools/
--rw-rw-rw-   0        0        0       82 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.6/promptflow_custom_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 17:48:26.591624 promptflow_custom_tools-0.0.6/promptflow_custom_tools/tools/
--rw-rw-rw-   0        0        0       82 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.6/promptflow_custom_tools/tools/__init__.py
--rw-rw-rw-   0        0        0     2342 2024-04-25 19:01:57.000000 promptflow_custom_tools-0.0.6/promptflow_custom_tools/tools/claude.py
--rw-rw-rw-   0        0        0      553 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.6/promptflow_custom_tools/tools/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-07 17:48:26.603401 promptflow_custom_tools-0.0.6/promptflow_custom_tools/yamls/
--rw-rw-rw-   0        0        0     6776 2024-05-07 17:47:45.000000 promptflow_custom_tools-0.0.6/promptflow_custom_tools/yamls/claude.yaml
-drwxrwxrwx   0        0        0        0 2024-05-07 17:48:26.590118 promptflow_custom_tools-0.0.6/promptflow_custom_tools.egg-info/
--rw-rw-rw-   0        0        0      128 2024-05-07 17:48:26.000000 promptflow_custom_tools-0.0.6/promptflow_custom_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      560 2024-05-07 17:48:26.000000 promptflow_custom_tools-0.0.6/promptflow_custom_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 17:48:26.000000 promptflow_custom_tools-0.0.6/promptflow_custom_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-05-07 17:48:26.000000 promptflow_custom_tools-0.0.6/promptflow_custom_tools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       38 2024-05-07 17:48:26.000000 promptflow_custom_tools-0.0.6/promptflow_custom_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2024-05-07 17:48:26.000000 promptflow_custom_tools-0.0.6/promptflow_custom_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 17:48:26.605556 promptflow_custom_tools-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      513 2024-05-07 17:48:03.000000 promptflow_custom_tools-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 17:48:26.604548 promptflow_custom_tools-0.0.6/tests/
--rw-rw-rw-   0        0        0        0 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.6/tests/__init__.py
--rw-rw-rw-   0        0        0      709 2024-04-22 20:27:24.000000 promptflow_custom_tools-0.0.6/tests/test_claude.py
+drwxrwxrwx   0        0        0        0 2024-05-07 18:13:37.214721 promptflow_custom_tools-0.0.7/
+-rw-rw-rw-   0        0        0     1072 2024-04-22 20:09:19.000000 promptflow_custom_tools-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0       44 2024-04-22 20:28:40.000000 promptflow_custom_tools-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      128 2024-05-07 18:13:37.214721 promptflow_custom_tools-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       25 2024-04-22 20:28:57.000000 promptflow_custom_tools-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 18:13:37.189866 promptflow_custom_tools-0.0.7/promptflow_custom_tools/
+-rw-rw-rw-   0        0        0       82 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.7/promptflow_custom_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 18:13:37.212713 promptflow_custom_tools-0.0.7/promptflow_custom_tools/tools/
+-rw-rw-rw-   0        0        0       82 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.7/promptflow_custom_tools/tools/__init__.py
+-rw-rw-rw-   0        0        0     2434 2024-05-07 18:13:14.000000 promptflow_custom_tools-0.0.7/promptflow_custom_tools/tools/claude.py
+-rw-rw-rw-   0        0        0      553 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.7/promptflow_custom_tools/tools/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-07 18:13:37.212713 promptflow_custom_tools-0.0.7/promptflow_custom_tools/yamls/
+-rw-rw-rw-   0        0        0     6776 2024-05-07 17:47:45.000000 promptflow_custom_tools-0.0.7/promptflow_custom_tools/yamls/claude.yaml
+drwxrwxrwx   0        0        0        0 2024-05-07 18:13:37.210233 promptflow_custom_tools-0.0.7/promptflow_custom_tools.egg-info/
+-rw-rw-rw-   0        0        0      128 2024-05-07 18:13:37.000000 promptflow_custom_tools-0.0.7/promptflow_custom_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      560 2024-05-07 18:13:37.000000 promptflow_custom_tools-0.0.7/promptflow_custom_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 18:13:37.000000 promptflow_custom_tools-0.0.7/promptflow_custom_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-07 18:13:37.000000 promptflow_custom_tools-0.0.7/promptflow_custom_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       38 2024-05-07 18:13:37.000000 promptflow_custom_tools-0.0.7/promptflow_custom_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2024-05-07 18:13:37.000000 promptflow_custom_tools-0.0.7/promptflow_custom_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 18:13:37.214721 promptflow_custom_tools-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      513 2024-05-07 18:13:34.000000 promptflow_custom_tools-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 18:13:37.213723 promptflow_custom_tools-0.0.7/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.7/tests/__init__.py
+-rw-rw-rw-   0        0        0      709 2024-04-22 20:27:24.000000 promptflow_custom_tools-0.0.7/tests/test_claude.py
```

### Comparing `promptflow_custom_tools-0.0.6/LICENSE` & `promptflow_custom_tools-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `promptflow_custom_tools-0.0.6/promptflow_custom_tools/tools/claude.py` & `promptflow_custom_tools-0.0.7/promptflow_custom_tools/tools/claude.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,16 +38,16 @@
 
 @tool
 def generate(
     connection: ClaudeConnection,
     prompt: PromptTemplate,
     model: str = "claude-3-opus-20240229",
     temperature: float  = 1,
-    top_p: float = 1.0,
-    max_tokens: int = 1024,
+    top_p: float = None,
+    max_tokens: int = 4096,
     **kwargs
 ) -> str:
     
     # Replace with your tool code, customise your own code to handle and use the prompt here.
     # Usually connection contains configs to connect to an API.
     # Not all tools need a connection. You can remove it if you don't need it.
     prompt = render_jinja_template(prompt, trim_blocks=True, keep_trailing_newline=True, **kwargs)
@@ -63,21 +63,26 @@
 
     for i in messages:
         if i['role'] == 'system':
             system = i['content']
         else:
             updatedMessages.append(i)
 
-    message = client.messages.create(
-        model=model,
-        max_tokens=max_tokens,
-        temperature=temperature,
-        top_p=top_p,
-        system=system,
-        messages=updatedMessages
-    )
+
+    arguments = {
+        "model":model,
+        "max_tokens":max_tokens,
+        "temperature":temperature,
+        "system":system,
+        "messages":updatedMessages
+    }      
+
+    if top_p != None:
+        arguments['top_p'] = top_p 
+
+    message = client.messages.create(**arguments)
 
     response = ''
     for txt in message.content:
         response = response + txt.text
 
     return response
```

### Comparing `promptflow_custom_tools-0.0.6/promptflow_custom_tools/tools/utils.py` & `promptflow_custom_tools-0.0.7/promptflow_custom_tools/tools/utils.py`

 * *Files identical despite different names*

### Comparing `promptflow_custom_tools-0.0.6/promptflow_custom_tools/yamls/claude.yaml` & `promptflow_custom_tools-0.0.7/promptflow_custom_tools/yamls/claude.yaml`

 * *Files identical despite different names*

### Comparing `promptflow_custom_tools-0.0.6/promptflow_custom_tools.egg-info/SOURCES.txt` & `promptflow_custom_tools-0.0.7/promptflow_custom_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `promptflow_custom_tools-0.0.6/setup.py` & `promptflow_custom_tools-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 PACKAGE_NAME = "promptflow_custom_tools"
 
 setup(
     name=PACKAGE_NAME,
-    version="0.0.6",
+    version="0.0.7",
     description="This is my tools package",
     packages=find_packages(),
     entry_points={
         "package_tools": ["claude = promptflow_custom_tools.tools.utils:list_package_tools"],
     },
     include_package_data=True,   # This line tells setuptools to include files from MANIFEST.in
     install_requires=['promptflow', 'promptflow-tools', 'anthropic'],
```

### Comparing `promptflow_custom_tools-0.0.6/tests/test_claude.py` & `promptflow_custom_tools-0.0.7/tests/test_claude.py`

 * *Files identical despite different names*

