# Comparing `tmp/abstract_logs-0.0.0.2.tar.gz` & `tmp/abstract_logs-0.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_logs-0.0.0.2.tar", last modified: Sun Apr 28 05:02:15 2024, max compression
+gzip compressed data, was "abstract_logs-0.0.0.3.tar", last modified: Tue May  7 01:29:43 2024, max compression
```

## Comparing `abstract_logs-0.0.0.2.tar` & `abstract_logs-0.0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:02:15.277382 abstract_logs-0.0.0.2/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      505 2024-04-28 05:02:15.277382 abstract_logs-0.0.0.2/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_logs-0.0.0.2/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-04-28 05:02:15.277382 abstract_logs-0.0.0.2/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      924 2024-04-28 04:53:37.000000 abstract_logs-0.0.0.2/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:02:15.273382 abstract_logs-0.0.0.2/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:02:15.273382 abstract_logs-0.0.0.2/src/abstract_logs/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-28 04:53:57.000000 abstract_logs-0.0.0.2/src/abstract_logs/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     5985 2024-04-24 17:22:55.000000 abstract_logs-0.0.0.2/src/abstract_logs/abstract_logs.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      381 2024-04-24 17:20:38.000000 abstract_logs-0.0.0.2/src/abstract_logs/main.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:02:15.273382 abstract_logs-0.0.0.2/src/abstract_logs.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      505 2024-04-28 05:02:15.000000 abstract_logs-0.0.0.2/src/abstract_logs.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      313 2024-04-28 05:02:15.000000 abstract_logs-0.0.0.2/src/abstract_logs.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-04-28 05:02:15.000000 abstract_logs-0.0.0.2/src/abstract_logs.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       19 2024-04-28 05:02:15.000000 abstract_logs-0.0.0.2/src/abstract_logs.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       14 2024-04-28 05:02:15.000000 abstract_logs-0.0.0.2/src/abstract_logs.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-07 01:29:43.893105 abstract_logs-0.0.0.3/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      505 2024-05-07 01:29:43.893105 abstract_logs-0.0.0.3/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_logs-0.0.0.3/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-07 01:29:43.893105 abstract_logs-0.0.0.3/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      924 2024-05-07 01:29:36.000000 abstract_logs-0.0.0.3/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-07 01:29:43.893105 abstract_logs-0.0.0.3/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-07 01:29:43.893105 abstract_logs-0.0.0.3/src/abstract_logs/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-28 04:53:57.000000 abstract_logs-0.0.0.3/src/abstract_logs/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     2739 2024-05-07 01:29:27.000000 abstract_logs-0.0.0.3/src/abstract_logs/abstract_logs.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      381 2024-04-24 17:20:38.000000 abstract_logs-0.0.0.3/src/abstract_logs/main.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-07 01:29:43.893105 abstract_logs-0.0.0.3/src/abstract_logs.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      505 2024-05-07 01:29:43.000000 abstract_logs-0.0.0.3/src/abstract_logs.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      313 2024-05-07 01:29:43.000000 abstract_logs-0.0.0.3/src/abstract_logs.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-07 01:29:43.000000 abstract_logs-0.0.0.3/src/abstract_logs.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       19 2024-05-07 01:29:43.000000 abstract_logs-0.0.0.3/src/abstract_logs.egg-info/requires.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       14 2024-05-07 01:29:43.000000 abstract_logs-0.0.0.3/src/abstract_logs.egg-info/top_level.txt
```

### Comparing `abstract_logs-0.0.0.2/setup.py` & `abstract_logs-0.0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_logs',
-    version='0.0.0.2',
+    version='0.0.0.3',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
```

