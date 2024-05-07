# Comparing `tmp/special_agents-1.0.0.tar.gz` & `tmp/special_agents-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "special_agents-1.0.0.tar", last modified: Tue May  7 11:14:42 2024, max compression
+gzip compressed data, was "special_agents-1.0.1.tar", last modified: Tue May  7 11:27:41 2024, max compression
```

## Comparing `special_agents-1.0.0.tar` & `special_agents-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 11:14:42.565980 special_agents-1.0.0/
--rw-rw-rw-   0        0        0     4307 2024-05-07 11:00:25.000000 special_agents-1.0.0/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1065 2024-05-06 10:26:56.000000 special_agents-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       47 2024-05-06 13:58:26.000000 special_agents-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4446 2024-05-07 11:14:42.558901 special_agents-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3904 2024-05-07 11:08:29.000000 special_agents-1.0.0/README.md
--rw-rw-rw-   0        0        0       14 2024-05-07 11:14:15.000000 special_agents-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 11:14:42.565980 special_agents-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      986 2024-05-07 11:09:34.000000 special_agents-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 11:14:42.461799 special_agents-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-07 11:14:42.497796 special_agents-1.0.0/src/special_agents/
--rw-rw-rw-   0        0        0     1598 2024-05-07 08:55:14.000000 special_agents-1.0.0/src/special_agents/Agent.py
--rw-rw-rw-   0        0        0       21 2024-05-07 09:14:33.000000 special_agents-1.0.0/src/special_agents/__init__.py
--rw-rw-rw-   0        0        0      310 2024-05-06 21:25:26.000000 special_agents-1.0.0/src/special_agents/config.py
--rw-rw-rw-   0        0        0     4427 2024-05-07 06:56:02.000000 special_agents-1.0.0/src/special_agents/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-07 11:14:42.555611 special_agents-1.0.0/src/special_agents.egg-info/
--rw-rw-rw-   0        0        0     4446 2024-05-07 11:14:42.000000 special_agents-1.0.0/src/special_agents.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2024-05-07 11:14:42.000000 special_agents-1.0.0/src/special_agents.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 11:14:42.000000 special_agents-1.0.0/src/special_agents.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-07 11:14:42.000000 special_agents-1.0.0/src/special_agents.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-07 11:14:42.000000 special_agents-1.0.0/src/special_agents.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 11:27:41.379482 special_agents-1.0.1/
+-rw-rw-rw-   0        0        0     4307 2024-05-07 11:00:25.000000 special_agents-1.0.1/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1065 2024-05-06 10:26:56.000000 special_agents-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       47 2024-05-06 13:58:26.000000 special_agents-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4452 2024-05-07 11:27:41.379482 special_agents-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3910 2024-05-07 11:27:20.000000 special_agents-1.0.1/README.md
+-rw-rw-rw-   0        0        0       14 2024-05-07 11:14:15.000000 special_agents-1.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 11:27:41.383167 special_agents-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1026 2024-05-07 11:26:23.000000 special_agents-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 11:27:41.280385 special_agents-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-07 11:27:41.310399 special_agents-1.0.1/src/special_agents/
+-rw-rw-rw-   0        0        0     1598 2024-05-07 08:55:14.000000 special_agents-1.0.1/src/special_agents/Agent.py
+-rw-rw-rw-   0        0        0       21 2024-05-07 09:14:33.000000 special_agents-1.0.1/src/special_agents/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 11:27:41.373413 special_agents-1.0.1/src/special_agents/agents/
+-rw-rw-rw-   0        0        0     5061 2024-05-07 10:48:03.000000 special_agents-1.0.1/src/special_agents/agents/ContentCreator.py
+-rw-rw-rw-   0        0        0     4077 2024-05-07 10:48:12.000000 special_agents-1.0.1/src/special_agents/agents/FullStackDeveloper.py
+-rw-rw-rw-   0        0        0     5917 2024-05-07 10:48:25.000000 special_agents-1.0.1/src/special_agents/agents/ProductManager.py
+-rw-rw-rw-   0        0        0       95 2024-05-07 11:09:17.000000 special_agents-1.0.1/src/special_agents/agents/__init__.py
+-rw-rw-rw-   0        0        0      310 2024-05-06 21:25:26.000000 special_agents-1.0.1/src/special_agents/config.py
+-rw-rw-rw-   0        0        0     4427 2024-05-07 06:56:02.000000 special_agents-1.0.1/src/special_agents/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-07 11:27:41.378096 special_agents-1.0.1/src/special_agents.egg-info/
+-rw-rw-rw-   0        0        0     4452 2024-05-07 11:27:41.000000 special_agents-1.0.1/src/special_agents.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      570 2024-05-07 11:27:41.000000 special_agents-1.0.1/src/special_agents.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 11:27:41.000000 special_agents-1.0.1/src/special_agents.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-07 11:27:41.000000 special_agents-1.0.1/src/special_agents.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-07 11:27:41.000000 special_agents-1.0.1/src/special_agents.egg-info/top_level.txt
```

### Comparing `special_agents-1.0.0/CONTRIBUTING.md` & `special_agents-1.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `special_agents-1.0.0/LICENSE` & `special_agents-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `special_agents-1.0.0/PKG-INFO` & `special_agents-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: special-agents
-Version: 1.0.0
+Version: 1.0.1
 Summary: An Open-source Library for pre-defined LLM powered specialized agents
 Home-page: https://github.com/IhabTag/special-agents
 Author: Ihab Tag
 Author-email: contact@ihabtag.com
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -90,15 +90,15 @@
 
 We welcome contributions from the community. Here are some ways you can contribute:
 
 -   Reporting bugs
 -   Suggesting enhancements
 -   Pull requests
 
-Please read [CONTRIBUTING.md](https://github.com/IhabTag/special-agents/blob/master/README.md) for details on our code of conduct, and the process for submitting pull requests to us.
+Please read [CONTRIBUTING.md](https://github.com/IhabTag/special-agents/blob/master/CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](https://github.com/IhabTag/special-agents/blob/master/LICENSE) file for details.
 
 ## Support
```

### Comparing `special_agents-1.0.0/README.md` & `special_agents-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
 We welcome contributions from the community. Here are some ways you can contribute:
 
 -   Reporting bugs
 -   Suggesting enhancements
 -   Pull requests
 
-Please read [CONTRIBUTING.md](https://github.com/IhabTag/special-agents/blob/master/README.md) for details on our code of conduct, and the process for submitting pull requests to us.
+Please read [CONTRIBUTING.md](https://github.com/IhabTag/special-agents/blob/master/CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](https://github.com/IhabTag/special-agents/blob/master/LICENSE) file for details.
 
 ## Support
```

### Comparing `special_agents-1.0.0/setup.py` & `special_agents-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 with open("requirements.txt", "r", encoding="utf-8") as f:
     req = f.readlines()
 req = [x.strip() for x in req if x.strip()]
 
 setup(
     name="special-agents", 
-    version="1.0.0",
+    version="1.0.1",
     author="Ihab Tag",
     author_email="contact@ihabtag.com",
     description="An Open-source Library for pre-defined LLM powered specialized agents",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/IhabTag/special-agents",
     # packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
-    packages = ['special_agents'],
+    packages = ['special_agents', 'special_agents.agents'],
     python_requires='>=3.6',
     license='MIT license',
     install_requires=req
 )
```

### Comparing `special_agents-1.0.0/src/special_agents/Agent.py` & `special_agents-1.0.1/src/special_agents/Agent.py`

 * *Files identical despite different names*

### Comparing `special_agents-1.0.0/src/special_agents/utils.py` & `special_agents-1.0.1/src/special_agents/utils.py`

 * *Files identical despite different names*

### Comparing `special_agents-1.0.0/src/special_agents.egg-info/PKG-INFO` & `special_agents-1.0.1/src/special_agents.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: special-agents
-Version: 1.0.0
+Version: 1.0.1
 Summary: An Open-source Library for pre-defined LLM powered specialized agents
 Home-page: https://github.com/IhabTag/special-agents
 Author: Ihab Tag
 Author-email: contact@ihabtag.com
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -90,15 +90,15 @@
 
 We welcome contributions from the community. Here are some ways you can contribute:
 
 -   Reporting bugs
 -   Suggesting enhancements
 -   Pull requests
 
-Please read [CONTRIBUTING.md](https://github.com/IhabTag/special-agents/blob/master/README.md) for details on our code of conduct, and the process for submitting pull requests to us.
+Please read [CONTRIBUTING.md](https://github.com/IhabTag/special-agents/blob/master/CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](https://github.com/IhabTag/special-agents/blob/master/LICENSE) file for details.
 
 ## Support
```

