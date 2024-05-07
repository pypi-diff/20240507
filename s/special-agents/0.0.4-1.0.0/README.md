# Comparing `tmp/special_agents-0.0.4.tar.gz` & `tmp/special_agents-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "special_agents-0.0.4.tar", last modified: Mon May  6 15:01:18 2024, max compression
+gzip compressed data, was "special_agents-1.0.0.tar", last modified: Tue May  7 11:14:42 2024, max compression
```

## Comparing `special_agents-0.0.4.tar` & `special_agents-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 15:01:18.566585 special_agents-0.0.4/
--rw-rw-rw-   0        0        0     1065 2024-05-06 10:26:56.000000 special_agents-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       47 2024-05-06 13:58:26.000000 special_agents-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1145 2024-05-06 15:01:18.560900 special_agents-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       16 2024-05-06 10:26:56.000000 special_agents-0.0.4/README.md
--rw-rw-rw-   0        0        0      333 2024-05-06 13:52:29.000000 special_agents-0.0.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 15:01:18.566585 special_agents-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      986 2024-05-06 15:00:45.000000 special_agents-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 15:01:18.493236 special_agents-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 15:01:18.510877 special_agents-0.0.4/src/special_agents/
--rw-rw-rw-   0        0        0       30 2024-05-06 15:01:06.000000 special_agents-0.0.4/src/special_agents/__init__.py
--rw-rw-rw-   0        0        0     2412 2024-05-06 12:05:56.000000 special_agents-0.0.4/src/special_agents/product_manager.py
-drwxrwxrwx   0        0        0        0 2024-05-06 15:01:18.557842 special_agents-0.0.4/src/special_agents.egg-info/
--rw-rw-rw-   0        0        0     1145 2024-05-06 15:01:18.000000 special_agents-0.0.4/src/special_agents.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2024-05-06 15:01:18.000000 special_agents-0.0.4/src/special_agents.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 15:01:18.000000 special_agents-0.0.4/src/special_agents.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      314 2024-05-06 15:01:18.000000 special_agents-0.0.4/src/special_agents.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-06 15:01:18.000000 special_agents-0.0.4/src/special_agents.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 11:14:42.565980 special_agents-1.0.0/
+-rw-rw-rw-   0        0        0     4307 2024-05-07 11:00:25.000000 special_agents-1.0.0/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1065 2024-05-06 10:26:56.000000 special_agents-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0       47 2024-05-06 13:58:26.000000 special_agents-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4446 2024-05-07 11:14:42.558901 special_agents-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3904 2024-05-07 11:08:29.000000 special_agents-1.0.0/README.md
+-rw-rw-rw-   0        0        0       14 2024-05-07 11:14:15.000000 special_agents-1.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 11:14:42.565980 special_agents-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      986 2024-05-07 11:09:34.000000 special_agents-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 11:14:42.461799 special_agents-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-07 11:14:42.497796 special_agents-1.0.0/src/special_agents/
+-rw-rw-rw-   0        0        0     1598 2024-05-07 08:55:14.000000 special_agents-1.0.0/src/special_agents/Agent.py
+-rw-rw-rw-   0        0        0       21 2024-05-07 09:14:33.000000 special_agents-1.0.0/src/special_agents/__init__.py
+-rw-rw-rw-   0        0        0      310 2024-05-06 21:25:26.000000 special_agents-1.0.0/src/special_agents/config.py
+-rw-rw-rw-   0        0        0     4427 2024-05-07 06:56:02.000000 special_agents-1.0.0/src/special_agents/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-07 11:14:42.555611 special_agents-1.0.0/src/special_agents.egg-info/
+-rw-rw-rw-   0        0        0     4446 2024-05-07 11:14:42.000000 special_agents-1.0.0/src/special_agents.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2024-05-07 11:14:42.000000 special_agents-1.0.0/src/special_agents.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 11:14:42.000000 special_agents-1.0.0/src/special_agents.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-07 11:14:42.000000 special_agents-1.0.0/src/special_agents.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-07 11:14:42.000000 special_agents-1.0.0/src/special_agents.egg-info/top_level.txt
```

### Comparing `special_agents-0.0.4/LICENSE` & `special_agents-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `special_agents-0.0.4/setup.py` & `special_agents-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     
 with open("requirements.txt", "r", encoding="utf-8") as f:
     req = f.readlines()
 req = [x.strip() for x in req if x.strip()]
 
 setup(
     name="special-agents", 
-    version="0.0.4",
+    version="1.0.0",
     author="Ihab Tag",
     author_email="contact@ihabtag.com",
     description="An Open-source Library for pre-defined LLM powered specialized agents",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/IhabTag/special-agents",
     # packages=setuptools.find_packages(),
```

