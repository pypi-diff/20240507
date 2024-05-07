# Comparing `tmp/special_agents-1.0.2.tar.gz` & `tmp/special_agents-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "special_agents-1.0.2.tar", last modified: Tue May  7 11:54:17 2024, max compression
+gzip compressed data, was "special_agents-1.0.3.tar", last modified: Tue May  7 12:01:29 2024, max compression
```

## Comparing `special_agents-1.0.2.tar` & `special_agents-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 11:54:17.371603 special_agents-1.0.2/
--rw-rw-rw-   0        0        0     4307 2024-05-07 11:00:25.000000 special_agents-1.0.2/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1065 2024-05-06 10:26:56.000000 special_agents-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       47 2024-05-06 13:58:26.000000 special_agents-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4452 2024-05-07 11:54:17.369585 special_agents-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3910 2024-05-07 11:27:20.000000 special_agents-1.0.2/README.md
--rw-rw-rw-   0        0        0       14 2024-05-07 11:14:15.000000 special_agents-1.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 11:54:17.372599 special_agents-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1026 2024-05-07 11:54:09.000000 special_agents-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 11:54:17.249817 special_agents-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-07 11:54:17.292592 special_agents-1.0.2/src/special_agents/
--rw-rw-rw-   0        0        0     1598 2024-05-07 11:46:36.000000 special_agents-1.0.2/src/special_agents/Agent.py
--rw-rw-rw-   0        0        0       43 2024-05-07 11:52:27.000000 special_agents-1.0.2/src/special_agents/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 11:54:17.363578 special_agents-1.0.2/src/special_agents/agents/
--rw-rw-rw-   0        0        0     5061 2024-05-07 10:48:03.000000 special_agents-1.0.2/src/special_agents/agents/ContentCreator.py
--rw-rw-rw-   0        0        0     4077 2024-05-07 10:48:12.000000 special_agents-1.0.2/src/special_agents/agents/FullStackDeveloper.py
--rw-rw-rw-   0        0        0     5915 2024-05-07 11:47:56.000000 special_agents-1.0.2/src/special_agents/agents/ProductManager.py
--rw-rw-rw-   0        0        0       95 2024-05-07 11:09:17.000000 special_agents-1.0.2/src/special_agents/agents/__init__.py
--rw-rw-rw-   0        0        0      310 2024-05-06 21:25:26.000000 special_agents-1.0.2/src/special_agents/config.py
--rw-rw-rw-   0        0        0     4427 2024-05-07 06:56:02.000000 special_agents-1.0.2/src/special_agents/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-07 11:54:17.366586 special_agents-1.0.2/src/special_agents.egg-info/
--rw-rw-rw-   0        0        0     4452 2024-05-07 11:54:17.000000 special_agents-1.0.2/src/special_agents.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      570 2024-05-07 11:54:17.000000 special_agents-1.0.2/src/special_agents.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 11:54:17.000000 special_agents-1.0.2/src/special_agents.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-07 11:54:17.000000 special_agents-1.0.2/src/special_agents.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-07 11:54:17.000000 special_agents-1.0.2/src/special_agents.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 12:01:29.254011 special_agents-1.0.3/
+-rw-rw-rw-   0        0        0     4307 2024-05-07 11:00:25.000000 special_agents-1.0.3/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1065 2024-05-06 10:26:56.000000 special_agents-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0       47 2024-05-06 13:58:26.000000 special_agents-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4452 2024-05-07 12:01:29.251894 special_agents-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3910 2024-05-07 11:27:20.000000 special_agents-1.0.3/README.md
+-rw-rw-rw-   0        0        0       14 2024-05-07 11:14:15.000000 special_agents-1.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 12:01:29.255011 special_agents-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1026 2024-05-07 12:01:17.000000 special_agents-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:01:29.117171 special_agents-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-07 12:01:29.146639 special_agents-1.0.3/src/special_agents/
+-rw-rw-rw-   0        0        0     1598 2024-05-07 11:46:36.000000 special_agents-1.0.3/src/special_agents/Agent.py
+-rw-rw-rw-   0        0        0       43 2024-05-07 11:52:27.000000 special_agents-1.0.3/src/special_agents/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:01:29.246785 special_agents-1.0.3/src/special_agents/agents/
+-rw-rw-rw-   0        0        0     5201 2024-05-07 12:01:07.000000 special_agents-1.0.3/src/special_agents/agents/ContentCreator.py
+-rw-rw-rw-   0        0        0     4217 2024-05-07 12:01:00.000000 special_agents-1.0.3/src/special_agents/agents/FullStackDeveloper.py
+-rw-rw-rw-   0        0        0     6059 2024-05-07 12:00:50.000000 special_agents-1.0.3/src/special_agents/agents/ProductManager.py
+-rw-rw-rw-   0        0        0       95 2024-05-07 11:09:17.000000 special_agents-1.0.3/src/special_agents/agents/__init__.py
+-rw-rw-rw-   0        0        0      310 2024-05-06 21:25:26.000000 special_agents-1.0.3/src/special_agents/config.py
+-rw-rw-rw-   0        0        0     4427 2024-05-07 06:56:02.000000 special_agents-1.0.3/src/special_agents/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:01:29.246785 special_agents-1.0.3/src/special_agents.egg-info/
+-rw-rw-rw-   0        0        0     4452 2024-05-07 12:01:29.000000 special_agents-1.0.3/src/special_agents.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      570 2024-05-07 12:01:29.000000 special_agents-1.0.3/src/special_agents.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 12:01:29.000000 special_agents-1.0.3/src/special_agents.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-07 12:01:29.000000 special_agents-1.0.3/src/special_agents.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-07 12:01:29.000000 special_agents-1.0.3/src/special_agents.egg-info/top_level.txt
```

### Comparing `special_agents-1.0.2/CONTRIBUTING.md` & `special_agents-1.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `special_agents-1.0.2/LICENSE` & `special_agents-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `special_agents-1.0.2/PKG-INFO` & `special_agents-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: special-agents
-Version: 1.0.2
+Version: 1.0.3
 Summary: An Open-source Library for pre-defined LLM powered specialized agents
 Home-page: https://github.com/IhabTag/special-agents
 Author: Ihab Tag
 Author-email: contact@ihabtag.com
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `special_agents-1.0.2/README.md` & `special_agents-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `special_agents-1.0.2/setup.py` & `special_agents-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     
 with open("requirements.txt", "r", encoding="utf-8") as f:
     req = f.readlines()
 req = [x.strip() for x in req if x.strip()]
 
 setup(
     name="special-agents", 
-    version="1.0.2",
+    version="1.0.3",
     author="Ihab Tag",
     author_email="contact@ihabtag.com",
     description="An Open-source Library for pre-defined LLM powered specialized agents",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/IhabTag/special-agents",
     # packages=setuptools.find_packages(),
```

### Comparing `special_agents-1.0.2/src/special_agents/Agent.py` & `special_agents-1.0.3/src/special_agents/Agent.py`

 * *Files identical despite different names*

### Comparing `special_agents-1.0.2/src/special_agents/agents/ContentCreator.py` & `special_agents-1.0.3/src/special_agents/agents/ContentCreator.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,16 @@
         Collaborate across teams to determine and solve campaign objectives
         Monitor digital engagement metrics
         Promote offerings to reach new audiences
         Research market trends and developments relevant to campaign subject matter
 
         """
 
+    def general_answer(self, question: str, context: str=None):
+        return super().general_answer(question=question, context=context)
 
     def write_linkedin_post(self, context: str): 
 
         task = """Considering your competencies and utilizing your capabilities, given the above CONTEXT, your task is to write a social media post that suits LinkedIn."""
         question = """Write a compelling LinkedIn post rich in details that considers the best practices and promotes users to engage and interact for the post to go viral for the audience most relevant to the CONTEXT."""
 
         response = openai_answer(role=self.role,
```

### Comparing `special_agents-1.0.2/src/special_agents/agents/FullStackDeveloper.py` & `special_agents-1.0.3/src/special_agents/agents/FullStackDeveloper.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,16 @@
         - Ensuring the technical feasibility of UI/UX designs.
         - Contribute to presentation layer standards and practices.
         - Contribute to testing and implementation approach for presentation layer.
         - Prototype future interfaces.
         - Collaborating closely with the product team and other team members and stakeholders .
         """
 
+    def general_answer(self, question: str, context: str=None):
+        return super().general_answer(question=question, context=context)
 
     def write_code_documentation(self, context: str): 
 
         task = """Considering your competencies and utilizing your capabilities, given the above CONTEXT, your task is to write the necessary code documentation"""
         question = """Add the necessary docstrings in google style and the important inline comments to the code presented in the CONTEXT WITHOUT changing the code itself"""
 
         response = openai_answer(role=self.role,
```

### Comparing `special_agents-1.0.2/src/special_agents/agents/ProductManager.py` & `special_agents-1.0.3/src/special_agents/agents/ProductManager.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,18 @@
         -Transforming ideas and feedback into a product vision and roadmap
         -Understanding with customer problems in order to collect user needs, requirements, and pain points
         -Utilizing performance metrics and data analysis to refine and improve product impact
         -Working closely with the Technical team to execute and deliver roadmap milestones.
         -Understand, communicate and drive optimization of all leading metrics and KPIs 
         """
 
+    def general_answer(self, question: str, context: str=None):
+        return super().general_answer(question=question, context=context)
+
+
     def write_user_story(self, context: str):
         """
         Write the best user story based on the given context.
 
         Args:
             context (str): The context for writing the user story.
```

### Comparing `special_agents-1.0.2/src/special_agents/utils.py` & `special_agents-1.0.3/src/special_agents/utils.py`

 * *Files identical despite different names*

### Comparing `special_agents-1.0.2/src/special_agents.egg-info/PKG-INFO` & `special_agents-1.0.3/src/special_agents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: special-agents
-Version: 1.0.2
+Version: 1.0.3
 Summary: An Open-source Library for pre-defined LLM powered specialized agents
 Home-page: https://github.com/IhabTag/special-agents
 Author: Ihab Tag
 Author-email: contact@ihabtag.com
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `special_agents-1.0.2/src/special_agents.egg-info/SOURCES.txt` & `special_agents-1.0.3/src/special_agents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

