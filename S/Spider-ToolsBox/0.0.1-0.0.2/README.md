# Comparing `tmp/Spider_ToolsBox-0.0.1.tar.gz` & `tmp/Spider_ToolsBox-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Spider_ToolsBox-0.0.1.tar", last modified: Tue May  7 14:53:32 2024, max compression
+gzip compressed data, was "dist\Spider_ToolsBox-0.0.2.tar", last modified: Tue May  7 14:56:39 2024, max compression
```

## Comparing `Spider_ToolsBox-0.0.1.tar` & `Spider_ToolsBox-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 14:53:32.000000 Spider_ToolsBox-0.0.1/
--rw-rw-rw-   0        0        0     1094 2024-05-07 12:20:53.000000 Spider_ToolsBox-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      910 2024-05-07 14:53:32.000000 Spider_ToolsBox-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      425 2024-05-07 11:22:55.000000 Spider_ToolsBox-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-07 14:53:32.000000 Spider_ToolsBox-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      841 2024-05-07 14:52:26.000000 Spider_ToolsBox-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 14:53:32.000000 Spider_ToolsBox-0.0.1/spidertools/
--rw-rw-rw-   0        0        0    26786 2024-05-07 14:26:43.000000 Spider_ToolsBox-0.0.1/spidertools/spider_tools.py
--rw-rw-rw-   0        0        0      204 2024-05-07 14:26:43.000000 Spider_ToolsBox-0.0.1/spidertools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 14:53:32.000000 Spider_ToolsBox-0.0.1/Spider_ToolsBox.egg-info/
--rw-rw-rw-   0        0        0        1 2024-05-07 14:53:32.000000 Spider_ToolsBox-0.0.1/Spider_ToolsBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      910 2024-05-07 14:53:32.000000 Spider_ToolsBox-0.0.1/Spider_ToolsBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-07 14:53:32.000000 Spider_ToolsBox-0.0.1/Spider_ToolsBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       12 2024-05-07 14:53:32.000000 Spider_ToolsBox-0.0.1/Spider_ToolsBox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 14:56:39.000000 Spider_ToolsBox-0.0.2/
+-rw-rw-rw-   0        0        0     1094 2024-05-07 12:20:53.000000 Spider_ToolsBox-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      910 2024-05-07 14:56:39.000000 Spider_ToolsBox-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2024-05-07 11:22:55.000000 Spider_ToolsBox-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-07 14:56:39.000000 Spider_ToolsBox-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      876 2024-05-07 14:56:29.000000 Spider_ToolsBox-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 14:56:39.000000 Spider_ToolsBox-0.0.2/spidertools/
+-rw-rw-rw-   0        0        0    26786 2024-05-07 14:26:43.000000 Spider_ToolsBox-0.0.2/spidertools/spider_tools.py
+-rw-rw-rw-   0        0        0      204 2024-05-07 14:26:43.000000 Spider_ToolsBox-0.0.2/spidertools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 14:56:39.000000 Spider_ToolsBox-0.0.2/Spider_ToolsBox.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-07 14:56:39.000000 Spider_ToolsBox-0.0.2/Spider_ToolsBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      910 2024-05-07 14:56:39.000000 Spider_ToolsBox-0.0.2/Spider_ToolsBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2024-05-07 14:56:39.000000 Spider_ToolsBox-0.0.2/Spider_ToolsBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      276 2024-05-07 14:56:39.000000 Spider_ToolsBox-0.0.2/Spider_ToolsBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       12 2024-05-07 14:56:39.000000 Spider_ToolsBox-0.0.2/Spider_ToolsBox.egg-info/top_level.txt
```

### Comparing `Spider_ToolsBox-0.0.1/LICENSE.txt` & `Spider_ToolsBox-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Spider_ToolsBox-0.0.1/PKG-INFO` & `Spider_ToolsBox-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Spider_ToolsBox
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package For Crawler
 Home-page: https://github.com/JOUUUSKA/SpiderToolBox.git
 Author: JOUUUSKA
 Author-email: 1393827820@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Spider_ToolsBox-0.0.1/setup.py` & `Spider_ToolsBox-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,22 +9,23 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Spider_ToolsBox",
-    version="0.0.1",
+    version="0.0.2",
     author="JOUUUSKA",
     author_email="1393827820@qq.com",
     description="Package For Crawler",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JOUUUSKA/SpiderToolBox.git",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
+    install_requires=['requests']
 )
```

### Comparing `Spider_ToolsBox-0.0.1/spidertools/spider_tools.py` & `Spider_ToolsBox-0.0.2/spidertools/spider_tools.py`

 * *Files identical despite different names*

### Comparing `Spider_ToolsBox-0.0.1/Spider_ToolsBox.egg-info/PKG-INFO` & `Spider_ToolsBox-0.0.2/Spider_ToolsBox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Spider-ToolsBox
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package For Crawler
 Home-page: https://github.com/JOUUUSKA/SpiderToolBox.git
 Author: JOUUUSKA
 Author-email: 1393827820@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

