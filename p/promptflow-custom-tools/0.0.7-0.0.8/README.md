# Comparing `tmp/promptflow_custom_tools-0.0.7.tar.gz` & `tmp/promptflow_custom_tools-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptflow_custom_tools-0.0.7.tar", last modified: Tue May  7 18:13:37 2024, max compression
+gzip compressed data, was "promptflow_custom_tools-0.0.8.tar", last modified: Tue May  7 18:18:28 2024, max compression
```

## Comparing `promptflow_custom_tools-0.0.7.tar` & `promptflow_custom_tools-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 18:13:37.214721 promptflow_custom_tools-0.0.7/
--rw-rw-rw-   0        0        0     1072 2024-04-22 20:09:19.000000 promptflow_custom_tools-0.0.7/LICENSE
--rw-rw-rw-   0        0        0       44 2024-04-22 20:28:40.000000 promptflow_custom_tools-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      128 2024-05-07 18:13:37.214721 promptflow_custom_tools-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       25 2024-04-22 20:28:57.000000 promptflow_custom_tools-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 18:13:37.189866 promptflow_custom_tools-0.0.7/promptflow_custom_tools/
--rw-rw-rw-   0        0        0       82 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.7/promptflow_custom_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 18:13:37.212713 promptflow_custom_tools-0.0.7/promptflow_custom_tools/tools/
--rw-rw-rw-   0        0        0       82 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.7/promptflow_custom_tools/tools/__init__.py
--rw-rw-rw-   0        0        0     2434 2024-05-07 18:13:14.000000 promptflow_custom_tools-0.0.7/promptflow_custom_tools/tools/claude.py
--rw-rw-rw-   0        0        0      553 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.7/promptflow_custom_tools/tools/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-07 18:13:37.212713 promptflow_custom_tools-0.0.7/promptflow_custom_tools/yamls/
--rw-rw-rw-   0        0        0     6776 2024-05-07 17:47:45.000000 promptflow_custom_tools-0.0.7/promptflow_custom_tools/yamls/claude.yaml
-drwxrwxrwx   0        0        0        0 2024-05-07 18:13:37.210233 promptflow_custom_tools-0.0.7/promptflow_custom_tools.egg-info/
--rw-rw-rw-   0        0        0      128 2024-05-07 18:13:37.000000 promptflow_custom_tools-0.0.7/promptflow_custom_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      560 2024-05-07 18:13:37.000000 promptflow_custom_tools-0.0.7/promptflow_custom_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 18:13:37.000000 promptflow_custom_tools-0.0.7/promptflow_custom_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-05-07 18:13:37.000000 promptflow_custom_tools-0.0.7/promptflow_custom_tools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       38 2024-05-07 18:13:37.000000 promptflow_custom_tools-0.0.7/promptflow_custom_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2024-05-07 18:13:37.000000 promptflow_custom_tools-0.0.7/promptflow_custom_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 18:13:37.214721 promptflow_custom_tools-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      513 2024-05-07 18:13:34.000000 promptflow_custom_tools-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 18:13:37.213723 promptflow_custom_tools-0.0.7/tests/
--rw-rw-rw-   0        0        0        0 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.7/tests/__init__.py
--rw-rw-rw-   0        0        0      709 2024-04-22 20:27:24.000000 promptflow_custom_tools-0.0.7/tests/test_claude.py
+drwxrwxrwx   0        0        0        0 2024-05-07 18:18:28.630246 promptflow_custom_tools-0.0.8/
+-rw-rw-rw-   0        0        0     1072 2024-04-22 20:09:19.000000 promptflow_custom_tools-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0       44 2024-04-22 20:28:40.000000 promptflow_custom_tools-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      128 2024-05-07 18:18:28.630246 promptflow_custom_tools-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       25 2024-04-22 20:28:57.000000 promptflow_custom_tools-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 18:18:28.593915 promptflow_custom_tools-0.0.8/promptflow_custom_tools/
+-rw-rw-rw-   0        0        0       82 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.8/promptflow_custom_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 18:18:28.619535 promptflow_custom_tools-0.0.8/promptflow_custom_tools/tools/
+-rw-rw-rw-   0        0        0       82 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.8/promptflow_custom_tools/tools/__init__.py
+-rw-rw-rw-   0        0        0     2434 2024-05-07 18:13:14.000000 promptflow_custom_tools-0.0.8/promptflow_custom_tools/tools/claude.py
+-rw-rw-rw-   0        0        0      553 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.8/promptflow_custom_tools/tools/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-07 18:18:28.627760 promptflow_custom_tools-0.0.8/promptflow_custom_tools/yamls/
+-rw-rw-rw-   0        0        0     6798 2024-05-07 18:17:49.000000 promptflow_custom_tools-0.0.8/promptflow_custom_tools/yamls/claude.yaml
+drwxrwxrwx   0        0        0        0 2024-05-07 18:18:28.617981 promptflow_custom_tools-0.0.8/promptflow_custom_tools.egg-info/
+-rw-rw-rw-   0        0        0      128 2024-05-07 18:18:28.000000 promptflow_custom_tools-0.0.8/promptflow_custom_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      560 2024-05-07 18:18:28.000000 promptflow_custom_tools-0.0.8/promptflow_custom_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 18:18:28.000000 promptflow_custom_tools-0.0.8/promptflow_custom_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-07 18:18:28.000000 promptflow_custom_tools-0.0.8/promptflow_custom_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       38 2024-05-07 18:18:28.000000 promptflow_custom_tools-0.0.8/promptflow_custom_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2024-05-07 18:18:28.000000 promptflow_custom_tools-0.0.8/promptflow_custom_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 18:18:28.630246 promptflow_custom_tools-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      513 2024-05-07 18:18:26.000000 promptflow_custom_tools-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 18:18:28.629153 promptflow_custom_tools-0.0.8/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.8/tests/__init__.py
+-rw-rw-rw-   0        0        0      709 2024-04-22 20:27:24.000000 promptflow_custom_tools-0.0.8/tests/test_claude.py
```

### Comparing `promptflow_custom_tools-0.0.7/LICENSE` & `promptflow_custom_tools-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `promptflow_custom_tools-0.0.7/promptflow_custom_tools/tools/claude.py` & `promptflow_custom_tools-0.0.8/promptflow_custom_tools/tools/claude.py`

 * *Files identical despite different names*

### Comparing `promptflow_custom_tools-0.0.7/promptflow_custom_tools/tools/utils.py` & `promptflow_custom_tools-0.0.8/promptflow_custom_tools/tools/utils.py`

 * *Files identical despite different names*

### Comparing `promptflow_custom_tools-0.0.7/promptflow_custom_tools/yamls/claude.yaml` & `promptflow_custom_tools-0.0.8/promptflow_custom_tools/yamls/claude.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     temperature:
       type:
         - double
       default: '1'
     top_p:
       type:
         - double
+      optional: true
     max_tokens:
       type:
         - int
       default: '4096'
   description: Tool for interacting with Claude LLM
   module: promptflow_custom_tools.tools.claude
   function: generate
```

### Comparing `promptflow_custom_tools-0.0.7/promptflow_custom_tools.egg-info/SOURCES.txt` & `promptflow_custom_tools-0.0.8/promptflow_custom_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `promptflow_custom_tools-0.0.7/setup.py` & `promptflow_custom_tools-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 PACKAGE_NAME = "promptflow_custom_tools"
 
 setup(
     name=PACKAGE_NAME,
-    version="0.0.7",
+    version="0.0.8",
     description="This is my tools package",
     packages=find_packages(),
     entry_points={
         "package_tools": ["claude = promptflow_custom_tools.tools.utils:list_package_tools"],
     },
     include_package_data=True,   # This line tells setuptools to include files from MANIFEST.in
     install_requires=['promptflow', 'promptflow-tools', 'anthropic'],
```

### Comparing `promptflow_custom_tools-0.0.7/tests/test_claude.py` & `promptflow_custom_tools-0.0.8/tests/test_claude.py`

 * *Files identical despite different names*

