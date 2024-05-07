# Comparing `tmp/sema_toolchain-0.0.6.tar.gz` & `tmp/sema_toolchain-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sema_toolchain-0.0.6.tar", last modified: Tue Apr 30 11:32:52 2024, max compression
+gzip compressed data, was "sema_toolchain-0.0.7.tar", last modified: Tue May  7 14:12:47 2024, max compression
```

## Comparing `sema_toolchain-0.0.6.tar` & `sema_toolchain-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 manon     (1000) manon     (1000)        0 2024-04-30 11:32:52.022475 sema_toolchain-0.0.6/
--rw-rw-r--   0 manon     (1000) manon     (1000)     1332 2024-04-16 10:03:35.000000 sema_toolchain-0.0.6/LICENSE
--rw-r--r--   0 manon     (1000) manon     (1000)    18056 2024-04-30 11:32:52.022475 sema_toolchain-0.0.6/PKG-INFO
--rw-rw-r--   0 manon     (1000) manon     (1000)    14818 2024-04-30 11:31:59.000000 sema_toolchain-0.0.6/README.md
--rw-rw-r--   0 manon     (1000) manon     (1000)     1542 2024-04-30 11:32:46.000000 sema_toolchain-0.0.6/pyproject.toml
-drwxrwxr-x   0 manon     (1000) manon     (1000)        0 2024-04-30 11:32:52.022475 sema_toolchain-0.0.6/sema_toolchain.egg-info/
--rw-r--r--   0 manon     (1000) manon     (1000)    18056 2024-04-30 11:32:52.000000 sema_toolchain-0.0.6/sema_toolchain.egg-info/PKG-INFO
--rw-rw-r--   0 manon     (1000) manon     (1000)      221 2024-04-30 11:32:52.000000 sema_toolchain-0.0.6/sema_toolchain.egg-info/SOURCES.txt
--rw-rw-r--   0 manon     (1000) manon     (1000)        1 2024-04-30 11:32:52.000000 sema_toolchain-0.0.6/sema_toolchain.egg-info/dependency_links.txt
--rw-rw-r--   0 manon     (1000) manon     (1000)      520 2024-04-30 11:32:52.000000 sema_toolchain-0.0.6/sema_toolchain.egg-info/requires.txt
--rw-rw-r--   0 manon     (1000) manon     (1000)       39 2024-04-30 11:32:52.000000 sema_toolchain-0.0.6/sema_toolchain.egg-info/top_level.txt
--rw-rw-r--   0 manon     (1000) manon     (1000)       38 2024-04-30 11:32:52.022475 sema_toolchain-0.0.6/setup.cfg
+drwxrwxr-x   0 manon     (1000) manon     (1000)        0 2024-05-07 14:12:47.428660 sema_toolchain-0.0.7/
+-rw-rw-r--   0 manon     (1000) manon     (1000)     1332 2024-04-16 10:03:35.000000 sema_toolchain-0.0.7/LICENSE
+-rw-r--r--   0 manon     (1000) manon     (1000)    18083 2024-05-07 14:12:47.428660 sema_toolchain-0.0.7/PKG-INFO
+-rw-rw-r--   0 manon     (1000) manon     (1000)    14818 2024-04-30 11:40:38.000000 sema_toolchain-0.0.7/README.md
+-rw-rw-r--   0 manon     (1000) manon     (1000)     1561 2024-05-07 14:12:43.000000 sema_toolchain-0.0.7/pyproject.toml
+drwxrwxr-x   0 manon     (1000) manon     (1000)        0 2024-05-07 14:12:47.428660 sema_toolchain-0.0.7/sema_toolchain.egg-info/
+-rw-r--r--   0 manon     (1000) manon     (1000)    18083 2024-05-07 14:12:47.000000 sema_toolchain-0.0.7/sema_toolchain.egg-info/PKG-INFO
+-rw-rw-r--   0 manon     (1000) manon     (1000)      221 2024-05-07 14:12:47.000000 sema_toolchain-0.0.7/sema_toolchain.egg-info/SOURCES.txt
+-rw-rw-r--   0 manon     (1000) manon     (1000)        1 2024-05-07 14:12:47.000000 sema_toolchain-0.0.7/sema_toolchain.egg-info/dependency_links.txt
+-rw-rw-r--   0 manon     (1000) manon     (1000)      532 2024-05-07 14:12:47.000000 sema_toolchain-0.0.7/sema_toolchain.egg-info/requires.txt
+-rw-rw-r--   0 manon     (1000) manon     (1000)       39 2024-05-07 14:12:47.000000 sema_toolchain-0.0.7/sema_toolchain.egg-info/top_level.txt
+-rw-rw-r--   0 manon     (1000) manon     (1000)       38 2024-05-07 14:12:47.428660 sema_toolchain-0.0.7/setup.cfg
```

### Comparing `sema_toolchain-0.0.6/LICENSE` & `sema_toolchain-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sema_toolchain-0.0.6/PKG-INFO` & `sema_toolchain-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sema_toolchain
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python symbolic execution package
 Author-email: Manon-Oreins <manon.oreins@gmail.com>
 License: BSD 2-Clause License
         
         Copyright (c) 2022, UCL-Cybersecurity team
         All rights reserved.
         
@@ -76,14 +76,15 @@
 Requires-Dist: seaborn
 Requires-Dist: scikit-learn
 Requires-Dist: progressbar
 Requires-Dist: gensim
 Requires-Dist: grakel
 Requires-Dist: numpy
 Requires-Dist: torch
+Requires-Dist: torchvision
 Requires-Dist: flask_session
 Requires-Dist: django
 Requires-Dist: Flask-Cors
 Requires-Dist: npf-web-extension
 
 # :skull_and_crossbones: SEMA :skull_and_crossbones: - ToolChain using Symbolic Execution for Malware Analysis.
```

### Comparing `sema_toolchain-0.0.6/README.md` & `sema_toolchain-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `sema_toolchain-0.0.6/pyproject.toml` & `sema_toolchain-0.0.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 py-modules = ["sema_scdg", "sema_web_app", "sema_classifier"]
 
 [project]
 name = "sema_toolchain"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Manon-Oreins", email="manon.oreins@gmail.com" },
 ]
 description = "Python symbolic execution package"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
@@ -61,14 +61,15 @@
     "seaborn",
     "scikit-learn",
     "progressbar",
     "gensim",
     "grakel",
     "numpy",
     "torch",
+    "torchvision",
     "flask_session",
     "django",
     "Flask-Cors",
     "npf-web-extension"
 ]
```

### Comparing `sema_toolchain-0.0.6/sema_toolchain.egg-info/PKG-INFO` & `sema_toolchain-0.0.7/sema_toolchain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sema_toolchain
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python symbolic execution package
 Author-email: Manon-Oreins <manon.oreins@gmail.com>
 License: BSD 2-Clause License
         
         Copyright (c) 2022, UCL-Cybersecurity team
         All rights reserved.
         
@@ -76,14 +76,15 @@
 Requires-Dist: seaborn
 Requires-Dist: scikit-learn
 Requires-Dist: progressbar
 Requires-Dist: gensim
 Requires-Dist: grakel
 Requires-Dist: numpy
 Requires-Dist: torch
+Requires-Dist: torchvision
 Requires-Dist: flask_session
 Requires-Dist: django
 Requires-Dist: Flask-Cors
 Requires-Dist: npf-web-extension
 
 # :skull_and_crossbones: SEMA :skull_and_crossbones: - ToolChain using Symbolic Execution for Malware Analysis.
```

### Comparing `sema_toolchain-0.0.6/sema_toolchain.egg-info/requires.txt` & `sema_toolchain-0.0.7/sema_toolchain.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -38,11 +38,12 @@
 seaborn
 scikit-learn
 progressbar
 gensim
 grakel
 numpy
 torch
+torchvision
 flask_session
 django
 Flask-Cors
 npf-web-extension
```

