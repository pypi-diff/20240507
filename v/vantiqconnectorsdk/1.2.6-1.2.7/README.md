# Comparing `tmp/vantiqconnectorsdk-1.2.6.tar.gz` & `tmp/vantiqconnectorsdk-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantiqconnectorsdk-1.2.6.tar", last modified: Thu Apr 18 20:20:15 2024, max compression
+gzip compressed data, was "vantiqconnectorsdk-1.2.7.tar", last modified: Mon May  6 23:40:43 2024, max compression
```

## Comparing `vantiqconnectorsdk-1.2.6.tar` & `vantiqconnectorsdk-1.2.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-04-18 20:20:15.096558 vantiqconnectorsdk-1.2.6/
--rw-r--r--   0 fcarter    (501) staff       (20)     1079 2022-08-10 20:55:53.000000 vantiqconnectorsdk-1.2.6/LICENSE
--rw-r--r--   0 fcarter    (501) staff       (20)    19609 2024-04-18 20:20:15.093814 vantiqconnectorsdk-1.2.6/PKG-INFO
--rw-r--r--   0 fcarter    (501) staff       (20)    17913 2023-12-01 23:54:03.000000 vantiqconnectorsdk-1.2.6/README.md
--rw-r--r--   0 fcarter    (501) staff       (20)       80 2022-08-10 20:55:53.000000 vantiqconnectorsdk-1.2.6/pyproject.toml
--rw-r--r--   0 fcarter    (501) staff       (20)      714 2024-04-18 20:20:15.100232 vantiqconnectorsdk-1.2.6/setup.cfg
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-04-18 20:20:15.087446 vantiqconnectorsdk-1.2.6/src/
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-04-18 20:20:15.087603 vantiqconnectorsdk-1.2.6/src/main/
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-04-18 20:20:15.089689 vantiqconnectorsdk-1.2.6/src/main/python/
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-04-18 20:20:15.093178 vantiqconnectorsdk-1.2.6/src/main/python/vantiqconnectorsdk.egg-info/
--rw-r--r--   0 fcarter    (501) staff       (20)    19609 2024-04-18 20:20:15.000000 vantiqconnectorsdk-1.2.6/src/main/python/vantiqconnectorsdk.egg-info/PKG-INFO
--rw-r--r--   0 fcarter    (501) staff       (20)      369 2024-04-18 20:20:15.000000 vantiqconnectorsdk-1.2.6/src/main/python/vantiqconnectorsdk.egg-info/SOURCES.txt
--rw-r--r--   0 fcarter    (501) staff       (20)        1 2024-04-18 20:20:15.000000 vantiqconnectorsdk-1.2.6/src/main/python/vantiqconnectorsdk.egg-info/dependency_links.txt
--rw-r--r--   0 fcarter    (501) staff       (20)       33 2024-04-18 20:20:15.000000 vantiqconnectorsdk-1.2.6/src/main/python/vantiqconnectorsdk.egg-info/requires.txt
--rw-r--r--   0 fcarter    (501) staff       (20)       19 2024-04-18 20:20:15.000000 vantiqconnectorsdk-1.2.6/src/main/python/vantiqconnectorsdk.egg-info/top_level.txt
--rw-r--r--   0 fcarter    (501) staff       (20)    40374 2022-08-10 20:55:53.000000 vantiqconnectorsdk-1.2.6/src/main/python/vantiqconnectorsdk.py
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-05-06 23:40:43.832009 vantiqconnectorsdk-1.2.7/
+-rw-r--r--   0 fcarter    (501) staff       (20)     1079 2022-08-10 20:55:53.000000 vantiqconnectorsdk-1.2.7/LICENSE
+-rw-r--r--   0 fcarter    (501) staff       (20)    19609 2024-05-06 23:40:43.830255 vantiqconnectorsdk-1.2.7/PKG-INFO
+-rw-r--r--   0 fcarter    (501) staff       (20)    17913 2023-12-01 23:54:03.000000 vantiqconnectorsdk-1.2.7/README.md
+-rw-r--r--   0 fcarter    (501) staff       (20)       80 2022-08-10 20:55:53.000000 vantiqconnectorsdk-1.2.7/pyproject.toml
+-rw-r--r--   0 fcarter    (501) staff       (20)      714 2024-05-06 23:40:43.834070 vantiqconnectorsdk-1.2.7/setup.cfg
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-05-06 23:40:43.823006 vantiqconnectorsdk-1.2.7/src/
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-05-06 23:40:43.823119 vantiqconnectorsdk-1.2.7/src/main/
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-05-06 23:40:43.824867 vantiqconnectorsdk-1.2.7/src/main/python/
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-05-06 23:40:43.829593 vantiqconnectorsdk-1.2.7/src/main/python/vantiqconnectorsdk.egg-info/
+-rw-r--r--   0 fcarter    (501) staff       (20)    19609 2024-05-06 23:40:43.000000 vantiqconnectorsdk-1.2.7/src/main/python/vantiqconnectorsdk.egg-info/PKG-INFO
+-rw-r--r--   0 fcarter    (501) staff       (20)      369 2024-05-06 23:40:43.000000 vantiqconnectorsdk-1.2.7/src/main/python/vantiqconnectorsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 fcarter    (501) staff       (20)        1 2024-05-06 23:40:43.000000 vantiqconnectorsdk-1.2.7/src/main/python/vantiqconnectorsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 fcarter    (501) staff       (20)       33 2024-05-06 23:40:43.000000 vantiqconnectorsdk-1.2.7/src/main/python/vantiqconnectorsdk.egg-info/requires.txt
+-rw-r--r--   0 fcarter    (501) staff       (20)       19 2024-05-06 23:40:43.000000 vantiqconnectorsdk-1.2.7/src/main/python/vantiqconnectorsdk.egg-info/top_level.txt
+-rw-r--r--   0 fcarter    (501) staff       (20)    40374 2022-08-10 20:55:53.000000 vantiqconnectorsdk-1.2.7/src/main/python/vantiqconnectorsdk.py
```

### Comparing `vantiqconnectorsdk-1.2.6/LICENSE` & `vantiqconnectorsdk-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vantiqconnectorsdk-1.2.6/PKG-INFO` & `vantiqconnectorsdk-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantiqconnectorsdk
-Version: 1.2.6
+Version: 1.2.7
 Summary: SDK for building Vantiq extension sources/connectors in Python
 Home-page: https://github.com/Vantiq/vantiq-extension-sources
 Author: Vantiq, Inc
 Author-email: fcarter@vantiq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vantiqconnectorsdk-1.2.6/README.md` & `vantiqconnectorsdk-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `vantiqconnectorsdk-1.2.6/setup.cfg` & `vantiqconnectorsdk-1.2.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vantiqconnectorsdk
-version = 1.2.6
+version = 1.2.7
 description = SDK for building Vantiq extension sources/connectors in Python
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/Vantiq/vantiq-extension-sources
 author = Vantiq, Inc
 author_email = fcarter@vantiq.com
 license = MIT
```

### Comparing `vantiqconnectorsdk-1.2.6/src/main/python/vantiqconnectorsdk.egg-info/PKG-INFO` & `vantiqconnectorsdk-1.2.7/src/main/python/vantiqconnectorsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantiqconnectorsdk
-Version: 1.2.6
+Version: 1.2.7
 Summary: SDK for building Vantiq extension sources/connectors in Python
 Home-page: https://github.com/Vantiq/vantiq-extension-sources
 Author: Vantiq, Inc
 Author-email: fcarter@vantiq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vantiqconnectorsdk-1.2.6/src/main/python/vantiqconnectorsdk.py` & `vantiqconnectorsdk-1.2.7/src/main/python/vantiqconnectorsdk.py`

 * *Files identical despite different names*

