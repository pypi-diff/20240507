# Comparing `tmp/auto-fastapi-0.0.3.tar.gz` & `tmp/auto-fastapi-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-fastapi-0.0.3.tar", last modified: Sun Jan 21 19:46:21 2024, max compression
+gzip compressed data, was "auto-fastapi-0.1.0.tar", last modified: Tue May  7 10:26:07 2024, max compression
```

## Comparing `auto-fastapi-0.0.3.tar` & `auto-fastapi-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-01-21 19:46:21.726359 auto-fastapi-0.0.3/
--rw-rw-rw-   0        0        0       74 2024-01-21 19:46:21.000000 auto-fastapi-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2162 2024-01-21 19:46:21.726359 auto-fastapi-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1037 2024-01-21 16:53:12.000000 auto-fastapi-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-01-21 19:46:21.721359 auto-fastapi-0.0.3/auto_fastapi/
--rw-rw-rw-   0        0        0       85 2024-01-13 10:28:58.000000 auto-fastapi-0.0.3/auto_fastapi/__init__.py
--rw-rw-rw-   0        0        0    24809 2024-01-21 19:24:16.000000 auto-fastapi-0.0.3/auto_fastapi/auto.py
--rw-rw-rw-   0        0        0     1252 2024-01-21 19:12:36.000000 auto-fastapi-0.0.3/auto_fastapi/server.py
-drwxrwxrwx   0        0        0        0 2024-01-21 19:46:21.725359 auto-fastapi-0.0.3/auto_fastapi.egg-info/
--rw-rw-rw-   0        0        0     2162 2024-01-21 19:46:21.000000 auto-fastapi-0.0.3/auto_fastapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2024-01-21 19:46:21.000000 auto-fastapi-0.0.3/auto_fastapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-21 19:46:21.000000 auto-fastapi-0.0.3/auto_fastapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-01-21 19:46:21.000000 auto-fastapi-0.0.3/auto_fastapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-01-21 19:46:21.000000 auto-fastapi-0.0.3/auto_fastapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12832 2023-11-23 19:36:32.000000 auto-fastapi-0.0.3/build.py
--rw-rw-rw-   0        0        0       40 2024-01-12 18:44:11.000000 auto-fastapi-0.0.3/requirements-dev.txt
--rw-rw-rw-   0        0        0       16 2024-01-12 18:44:11.000000 auto-fastapi-0.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-01-21 19:46:21.726359 auto-fastapi-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1694 2024-01-21 19:46:16.000000 auto-fastapi-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 10:26:07.698661 auto-fastapi-0.1.0/
+-rw-rw-rw-   0        0        0       44 2024-05-07 10:26:07.000000 auto-fastapi-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2073 2024-05-07 10:26:07.697661 auto-fastapi-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1037 2024-01-21 16:53:12.000000 auto-fastapi-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 10:26:07.691661 auto-fastapi-0.1.0/auto_fastapi/
+-rw-rw-rw-   0        0        0      157 2024-05-07 10:26:00.000000 auto-fastapi-0.1.0/auto_fastapi/__init__.py
+-rw-rw-rw-   0        0        0    24809 2024-01-21 19:24:16.000000 auto-fastapi-0.1.0/auto_fastapi/auto.py
+-rw-rw-rw-   0        0        0     2699 2024-05-07 10:24:50.000000 auto-fastapi-0.1.0/auto_fastapi/automation.py
+-rw-rw-rw-   0        0        0      768 2024-05-07 10:23:42.000000 auto-fastapi-0.1.0/auto_fastapi/base.py
+-rw-rw-rw-   0        0        0     1252 2024-01-21 19:12:36.000000 auto-fastapi-0.1.0/auto_fastapi/server.py
+drwxrwxrwx   0        0        0        0 2024-05-07 10:26:07.696662 auto-fastapi-0.1.0/auto_fastapi.egg-info/
+-rw-rw-rw-   0        0        0     2073 2024-05-07 10:26:07.000000 auto-fastapi-0.1.0/auto_fastapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2024-05-07 10:26:07.000000 auto-fastapi-0.1.0/auto_fastapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 10:26:07.000000 auto-fastapi-0.1.0/auto_fastapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-07 10:26:07.000000 auto-fastapi-0.1.0/auto_fastapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-07 10:26:07.000000 auto-fastapi-0.1.0/auto_fastapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 auto-fastapi-0.1.0/build.py
+-rw-rw-rw-   0        0        0       27 2024-05-07 10:24:50.000000 auto-fastapi-0.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 10:26:07.698661 auto-fastapi-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1694 2024-05-07 10:26:06.000000 auto-fastapi-0.1.0/setup.py
```

### Comparing `auto-fastapi-0.0.3/PKG-INFO` & `auto-fastapi-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-fastapi
-Version: 0.0.3
+Version: 0.1.0
 Summary: A pythonic functional way to construct FastAPI applications be declaring endpoints in separation of their functional definition, enabeling to separate, replicate, and reuse functions in different APIs at the same time, and also run multiple of them.
 Home-page: https://github.com/Shahaf-F-S/auto-fastapi
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,18 +14,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
+Requires-Dist: dataplace
 Provides-Extra: dev
-Requires-Dist: pdoc3; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
 
 # auto-fastapi
 
 > A pythonic functional way to construct FastAPI applications be declaring endpoints in separation of their functional definition, enabeling to separate, replicate, and reuse functions in different APIs at the same time, and also run multiple of them.
 
 ## Installation
 ```
```

### Comparing `auto-fastapi-0.0.3/README.md` & `auto-fastapi-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `auto-fastapi-0.0.3/auto_fastapi/auto.py` & `auto-fastapi-0.1.0/auto_fastapi/auto.py`

 * *Files identical despite different names*

### Comparing `auto-fastapi-0.0.3/auto_fastapi/server.py` & `auto-fastapi-0.1.0/auto_fastapi/server.py`

 * *Files identical despite different names*

### Comparing `auto-fastapi-0.0.3/auto_fastapi.egg-info/PKG-INFO` & `auto-fastapi-0.1.0/auto_fastapi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-fastapi
-Version: 0.0.3
+Version: 0.1.0
 Summary: A pythonic functional way to construct FastAPI applications be declaring endpoints in separation of their functional definition, enabeling to separate, replicate, and reuse functions in different APIs at the same time, and also run multiple of them.
 Home-page: https://github.com/Shahaf-F-S/auto-fastapi
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,18 +14,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
+Requires-Dist: dataplace
 Provides-Extra: dev
-Requires-Dist: pdoc3; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
 
 # auto-fastapi
 
 > A pythonic functional way to construct FastAPI applications be declaring endpoints in separation of their functional definition, enabeling to separate, replicate, and reuse functions in different APIs at the same time, and also run multiple of them.
 
 ## Installation
 ```
```

### Comparing `auto-fastapi-0.0.3/setup.py` & `auto-fastapi-0.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='auto-fastapi',
-        version='0.0.3',
+        version='0.1.0',
         description=(
             "A pythonic functional way to construct FastAPI "
             "applications be declaring endpoints in separation "
             "of their functional definition, enabeling to separate, "
             "replicate, and reuse functions in different APIs at the "
             "same time, and also run multiple of them."
         ),
```

