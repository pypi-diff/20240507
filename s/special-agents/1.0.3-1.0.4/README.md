# Comparing `tmp/special_agents-1.0.3.tar.gz` & `tmp/special_agents-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "special_agents-1.0.3.tar", last modified: Tue May  7 12:01:29 2024, max compression
+gzip compressed data, was "special_agents-1.0.4.tar", last modified: Tue May  7 12:06:51 2024, max compression
```

## Comparing `special_agents-1.0.3.tar` & `special_agents-1.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 12:01:29.254011 special_agents-1.0.3/
--rw-rw-rw-   0        0        0     4307 2024-05-07 11:00:25.000000 special_agents-1.0.3/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1065 2024-05-06 10:26:56.000000 special_agents-1.0.3/LICENSE
--rw-rw-rw-   0        0        0       47 2024-05-06 13:58:26.000000 special_agents-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4452 2024-05-07 12:01:29.251894 special_agents-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3910 2024-05-07 11:27:20.000000 special_agents-1.0.3/README.md
--rw-rw-rw-   0        0        0       14 2024-05-07 11:14:15.000000 special_agents-1.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 12:01:29.255011 special_agents-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1026 2024-05-07 12:01:17.000000 special_agents-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 12:01:29.117171 special_agents-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-07 12:01:29.146639 special_agents-1.0.3/src/special_agents/
--rw-rw-rw-   0        0        0     1598 2024-05-07 11:46:36.000000 special_agents-1.0.3/src/special_agents/Agent.py
--rw-rw-rw-   0        0        0       43 2024-05-07 11:52:27.000000 special_agents-1.0.3/src/special_agents/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 12:01:29.246785 special_agents-1.0.3/src/special_agents/agents/
--rw-rw-rw-   0        0        0     5201 2024-05-07 12:01:07.000000 special_agents-1.0.3/src/special_agents/agents/ContentCreator.py
--rw-rw-rw-   0        0        0     4217 2024-05-07 12:01:00.000000 special_agents-1.0.3/src/special_agents/agents/FullStackDeveloper.py
--rw-rw-rw-   0        0        0     6059 2024-05-07 12:00:50.000000 special_agents-1.0.3/src/special_agents/agents/ProductManager.py
--rw-rw-rw-   0        0        0       95 2024-05-07 11:09:17.000000 special_agents-1.0.3/src/special_agents/agents/__init__.py
--rw-rw-rw-   0        0        0      310 2024-05-06 21:25:26.000000 special_agents-1.0.3/src/special_agents/config.py
--rw-rw-rw-   0        0        0     4427 2024-05-07 06:56:02.000000 special_agents-1.0.3/src/special_agents/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-07 12:01:29.246785 special_agents-1.0.3/src/special_agents.egg-info/
--rw-rw-rw-   0        0        0     4452 2024-05-07 12:01:29.000000 special_agents-1.0.3/src/special_agents.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      570 2024-05-07 12:01:29.000000 special_agents-1.0.3/src/special_agents.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 12:01:29.000000 special_agents-1.0.3/src/special_agents.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-07 12:01:29.000000 special_agents-1.0.3/src/special_agents.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-07 12:01:29.000000 special_agents-1.0.3/src/special_agents.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 12:06:51.080792 special_agents-1.0.4/
+-rw-rw-rw-   0        0        0     4307 2024-05-07 11:00:25.000000 special_agents-1.0.4/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1065 2024-05-06 10:26:56.000000 special_agents-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0       47 2024-05-06 13:58:26.000000 special_agents-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4452 2024-05-07 12:06:51.078825 special_agents-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3910 2024-05-07 11:27:20.000000 special_agents-1.0.4/README.md
+-rw-rw-rw-   0        0        0       14 2024-05-07 11:14:15.000000 special_agents-1.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 12:06:51.080792 special_agents-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1026 2024-05-07 12:06:18.000000 special_agents-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:06:50.937442 special_agents-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-07 12:06:50.982322 special_agents-1.0.4/src/special_agents/
+-rw-rw-rw-   0        0        0     1598 2024-05-07 11:46:36.000000 special_agents-1.0.4/src/special_agents/Agent.py
+-rw-rw-rw-   0        0        0       88 2024-05-07 12:04:20.000000 special_agents-1.0.4/src/special_agents/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:06:51.072813 special_agents-1.0.4/src/special_agents/agents/
+-rw-rw-rw-   0        0        0     5205 2024-05-07 12:06:28.000000 special_agents-1.0.4/src/special_agents/agents/ContentCreator.py
+-rw-rw-rw-   0        0        0     4221 2024-05-07 12:06:33.000000 special_agents-1.0.4/src/special_agents/agents/FullStackDeveloper.py
+-rw-rw-rw-   0        0        0     6063 2024-05-07 12:06:37.000000 special_agents-1.0.4/src/special_agents/agents/ProductManager.py
+-rw-rw-rw-   0        0        0       95 2024-05-07 11:09:17.000000 special_agents-1.0.4/src/special_agents/agents/__init__.py
+-rw-rw-rw-   0        0        0      310 2024-05-06 21:25:26.000000 special_agents-1.0.4/src/special_agents/config.py
+-rw-rw-rw-   0        0        0     4427 2024-05-07 06:56:02.000000 special_agents-1.0.4/src/special_agents/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:06:51.074501 special_agents-1.0.4/src/special_agents.egg-info/
+-rw-rw-rw-   0        0        0     4452 2024-05-07 12:06:50.000000 special_agents-1.0.4/src/special_agents.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      570 2024-05-07 12:06:50.000000 special_agents-1.0.4/src/special_agents.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 12:06:50.000000 special_agents-1.0.4/src/special_agents.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-07 12:06:50.000000 special_agents-1.0.4/src/special_agents.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-07 12:06:50.000000 special_agents-1.0.4/src/special_agents.egg-info/top_level.txt
```

### Comparing `special_agents-1.0.3/CONTRIBUTING.md` & `special_agents-1.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `special_agents-1.0.3/LICENSE` & `special_agents-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `special_agents-1.0.3/PKG-INFO` & `special_agents-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: special-agents
-Version: 1.0.3
+Version: 1.0.4
 Summary: An Open-source Library for pre-defined LLM powered specialized agents
 Home-page: https://github.com/IhabTag/special-agents
 Author: Ihab Tag
 Author-email: contact@ihabtag.com
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `special_agents-1.0.3/README.md` & `special_agents-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `special_agents-1.0.3/setup.py` & `special_agents-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     
 with open("requirements.txt", "r", encoding="utf-8") as f:
     req = f.readlines()
 req = [x.strip() for x in req if x.strip()]
 
 setup(
     name="special-agents", 
-    version="1.0.3",
+    version="1.0.4",
     author="Ihab Tag",
     author_email="contact@ihabtag.com",
     description="An Open-source Library for pre-defined LLM powered specialized agents",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/IhabTag/special-agents",
     # packages=setuptools.find_packages(),
```

### Comparing `special_agents-1.0.3/src/special_agents/Agent.py` & `special_agents-1.0.4/src/special_agents/Agent.py`

 * *Files identical despite different names*

### Comparing `special_agents-1.0.3/src/special_agents/agents/ContentCreator.py` & `special_agents-1.0.4/src/special_agents/agents/ContentCreator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from utils import *
-from Agent import Agent as BaseAgent
+from ..utils import *
+from ..Agent import Agent as BaseAgent
 
 class ContentCreator(BaseAgent):
 
     def __init__(self, role= '', 
                  competencies='', 
                  capabilities= '',
                  tone= '',
```

### Comparing `special_agents-1.0.3/src/special_agents/agents/FullStackDeveloper.py` & `special_agents-1.0.4/src/special_agents/agents/FullStackDeveloper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from utils import *
-from Agent import Agent as BaseAgent
+from ..utils import *
+from ..Agent import Agent as BaseAgent
 
 class FullStackDeveloper(BaseAgent):
 
     def __init__(self, role= '', 
                  competencies='', 
                  capabilities= '',
                  tone= '',
```

### Comparing `special_agents-1.0.3/src/special_agents/agents/ProductManager.py` & `special_agents-1.0.4/src/special_agents/agents/ProductManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from utils import *
-from Agent import Agent as BaseAgent
+from ..utils import *
+from ..Agent import Agent as BaseAgent
 
 class ProductManager(BaseAgent):
 
     def __init__(self, role= '', 
                  competencies='', 
                  capabilities= '',
                  tone= '',
```

### Comparing `special_agents-1.0.3/src/special_agents/utils.py` & `special_agents-1.0.4/src/special_agents/utils.py`

 * *Files identical despite different names*

### Comparing `special_agents-1.0.3/src/special_agents.egg-info/PKG-INFO` & `special_agents-1.0.4/src/special_agents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: special-agents
-Version: 1.0.3
+Version: 1.0.4
 Summary: An Open-source Library for pre-defined LLM powered specialized agents
 Home-page: https://github.com/IhabTag/special-agents
 Author: Ihab Tag
 Author-email: contact@ihabtag.com
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `special_agents-1.0.3/src/special_agents.egg-info/SOURCES.txt` & `special_agents-1.0.4/src/special_agents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

