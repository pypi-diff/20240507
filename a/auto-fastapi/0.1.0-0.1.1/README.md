# Comparing `tmp/auto-fastapi-0.1.0.tar.gz` & `tmp/auto-fastapi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-fastapi-0.1.0.tar", last modified: Tue May  7 10:26:07 2024, max compression
+gzip compressed data, was "auto-fastapi-0.1.1.tar", last modified: Tue May  7 10:30:54 2024, max compression
```

## Comparing `auto-fastapi-0.1.0.tar` & `auto-fastapi-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 10:26:07.698661 auto-fastapi-0.1.0/
--rw-rw-rw-   0        0        0       44 2024-05-07 10:26:07.000000 auto-fastapi-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2073 2024-05-07 10:26:07.697661 auto-fastapi-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1037 2024-01-21 16:53:12.000000 auto-fastapi-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 10:26:07.691661 auto-fastapi-0.1.0/auto_fastapi/
--rw-rw-rw-   0        0        0      157 2024-05-07 10:26:00.000000 auto-fastapi-0.1.0/auto_fastapi/__init__.py
--rw-rw-rw-   0        0        0    24809 2024-01-21 19:24:16.000000 auto-fastapi-0.1.0/auto_fastapi/auto.py
--rw-rw-rw-   0        0        0     2699 2024-05-07 10:24:50.000000 auto-fastapi-0.1.0/auto_fastapi/automation.py
--rw-rw-rw-   0        0        0      768 2024-05-07 10:23:42.000000 auto-fastapi-0.1.0/auto_fastapi/base.py
--rw-rw-rw-   0        0        0     1252 2024-01-21 19:12:36.000000 auto-fastapi-0.1.0/auto_fastapi/server.py
-drwxrwxrwx   0        0        0        0 2024-05-07 10:26:07.696662 auto-fastapi-0.1.0/auto_fastapi.egg-info/
--rw-rw-rw-   0        0        0     2073 2024-05-07 10:26:07.000000 auto-fastapi-0.1.0/auto_fastapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2024-05-07 10:26:07.000000 auto-fastapi-0.1.0/auto_fastapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 10:26:07.000000 auto-fastapi-0.1.0/auto_fastapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-07 10:26:07.000000 auto-fastapi-0.1.0/auto_fastapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-07 10:26:07.000000 auto-fastapi-0.1.0/auto_fastapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 auto-fastapi-0.1.0/build.py
--rw-rw-rw-   0        0        0       27 2024-05-07 10:24:50.000000 auto-fastapi-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 10:26:07.698661 auto-fastapi-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1694 2024-05-07 10:26:06.000000 auto-fastapi-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 10:30:54.588912 auto-fastapi-0.1.1/
+-rw-rw-rw-   0        0        0       44 2024-05-07 10:30:54.000000 auto-fastapi-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2073 2024-05-07 10:30:54.587912 auto-fastapi-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1037 2024-01-21 16:53:12.000000 auto-fastapi-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 10:30:54.584165 auto-fastapi-0.1.1/auto_fastapi/
+-rw-rw-rw-   0        0        0      157 2024-05-07 10:26:00.000000 auto-fastapi-0.1.1/auto_fastapi/__init__.py
+-rw-rw-rw-   0        0        0    24809 2024-01-21 19:24:16.000000 auto-fastapi-0.1.1/auto_fastapi/auto.py
+-rw-rw-rw-   0        0        0     2699 2024-05-07 10:24:50.000000 auto-fastapi-0.1.1/auto_fastapi/automation.py
+-rw-rw-rw-   0        0        0      768 2024-05-07 10:23:42.000000 auto-fastapi-0.1.1/auto_fastapi/base.py
+-rw-rw-rw-   0        0        0     1252 2024-01-21 19:12:36.000000 auto-fastapi-0.1.1/auto_fastapi/server.py
+drwxrwxrwx   0        0        0        0 2024-05-07 10:30:54.587912 auto-fastapi-0.1.1/auto_fastapi.egg-info/
+-rw-rw-rw-   0        0        0     2073 2024-05-07 10:30:54.000000 auto-fastapi-0.1.1/auto_fastapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2024-05-07 10:30:54.000000 auto-fastapi-0.1.1/auto_fastapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 10:30:54.000000 auto-fastapi-0.1.1/auto_fastapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-07 10:30:54.000000 auto-fastapi-0.1.1/auto_fastapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-07 10:30:54.000000 auto-fastapi-0.1.1/auto_fastapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 auto-fastapi-0.1.1/build.py
+-rw-rw-rw-   0        0        0       27 2024-05-07 10:24:50.000000 auto-fastapi-0.1.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 10:30:54.588912 auto-fastapi-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1694 2024-05-07 10:30:51.000000 auto-fastapi-0.1.1/setup.py
```

### Comparing `auto-fastapi-0.1.0/PKG-INFO` & `auto-fastapi-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-fastapi
-Version: 0.1.0
+Version: 0.1.1
 Summary: A pythonic functional way to construct FastAPI applications be declaring endpoints in separation of their functional definition, enabeling to separate, replicate, and reuse functions in different APIs at the same time, and also run multiple of them.
 Home-page: https://github.com/Shahaf-F-S/auto-fastapi
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `auto-fastapi-0.1.0/README.md` & `auto-fastapi-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `auto-fastapi-0.1.0/auto_fastapi/auto.py` & `auto-fastapi-0.1.1/auto_fastapi/auto.py`

 * *Files identical despite different names*

### Comparing `auto-fastapi-0.1.0/auto_fastapi/automation.py` & `auto-fastapi-0.1.1/auto_fastapi/automation.py`

 * *Files identical despite different names*

### Comparing `auto-fastapi-0.1.0/auto_fastapi/base.py` & `auto-fastapi-0.1.1/auto_fastapi/base.py`

 * *Files identical despite different names*

### Comparing `auto-fastapi-0.1.0/auto_fastapi/server.py` & `auto-fastapi-0.1.1/auto_fastapi/server.py`

 * *Files identical despite different names*

### Comparing `auto-fastapi-0.1.0/auto_fastapi.egg-info/PKG-INFO` & `auto-fastapi-0.1.1/auto_fastapi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-fastapi
-Version: 0.1.0
+Version: 0.1.1
 Summary: A pythonic functional way to construct FastAPI applications be declaring endpoints in separation of their functional definition, enabeling to separate, replicate, and reuse functions in different APIs at the same time, and also run multiple of them.
 Home-page: https://github.com/Shahaf-F-S/auto-fastapi
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `auto-fastapi-0.1.0/build.py` & `auto-fastapi-0.1.1/build.py`

 * *Files identical despite different names*

### Comparing `auto-fastapi-0.1.0/setup.py` & `auto-fastapi-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='auto-fastapi',
-        version='0.1.0',
+        version='0.1.1',
         description=(
             "A pythonic functional way to construct FastAPI "
             "applications be declaring endpoints in separation "
             "of their functional definition, enabeling to separate, "
             "replicate, and reuse functions in different APIs at the "
             "same time, and also run multiple of them."
         ),
```

