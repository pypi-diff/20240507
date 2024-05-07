# Comparing `tmp/livedc-0.0.3.tar.gz` & `tmp/livedc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livedc-0.0.3.tar", last modified: Fri May  3 16:38:09 2024, max compression
+gzip compressed data, was "livedc-0.0.4.tar", last modified: Tue May  7 00:58:38 2024, max compression
```

## Comparing `livedc-0.0.3.tar` & `livedc-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 16:38:09.349228 livedc-0.0.3/
--rw-rw-rw-   0        0        0     1091 2024-05-03 13:31:15.000000 livedc-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2089 2024-05-03 16:38:09.347239 livedc-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       83 2024-05-03 13:31:15.000000 livedc-0.0.3/README.md
--rw-rw-rw-   0        0        0      854 2024-05-03 16:38:09.000000 livedc-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-03 16:38:09.349228 livedc-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1079 2024-05-03 13:54:21.000000 livedc-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 16:38:09.317617 livedc-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-03 16:38:09.329614 livedc-0.0.3/src/livedc/
--rw-rw-rw-   0        0        0       51 2024-05-03 16:34:46.000000 livedc-0.0.3/src/livedc/__init__.py
--rw-rw-rw-   0        0        0     1587 2024-05-03 16:17:07.000000 livedc-0.0.3/src/livedc/desc.py
-drwxrwxrwx   0        0        0        0 2024-05-03 16:38:09.318609 livedc-0.0.3/src/livedc/math/
-drwxrwxrwx   0        0        0        0 2024-05-03 16:38:09.342524 livedc-0.0.3/src/livedc/math/financial/
--rw-rw-rw-   0        0        0     2585 2024-05-03 16:33:47.000000 livedc-0.0.3/src/livedc/math/financial/compound.py
-drwxrwxrwx   0        0        0        0 2024-05-03 16:38:09.345438 livedc-0.0.3/src/livedc.egg-info/
--rw-rw-rw-   0        0        0     2089 2024-05-03 16:38:09.000000 livedc-0.0.3/src/livedc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2024-05-03 16:38:09.000000 livedc-0.0.3/src/livedc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 16:38:09.000000 livedc-0.0.3/src/livedc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-03 16:38:09.000000 livedc-0.0.3/src/livedc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       61 2024-05-03 16:38:09.000000 livedc-0.0.3/src/livedc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-03 16:38:09.000000 livedc-0.0.3/src/livedc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 00:58:38.786795 livedc-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2024-05-03 13:31:15.000000 livedc-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2132 2024-05-07 00:58:38.784802 livedc-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       83 2024-05-03 13:31:15.000000 livedc-0.0.4/README.md
+-rw-rw-rw-   0        0        0      868 2024-05-07 00:58:38.000000 livedc-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-07 00:58:38.787161 livedc-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1079 2024-05-03 13:54:21.000000 livedc-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 00:58:38.754959 livedc-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-07 00:58:38.767862 livedc-0.0.4/src/livedc/
+-rw-rw-rw-   0        0        0       51 2024-05-07 00:57:36.000000 livedc-0.0.4/src/livedc/__init__.py
+-rw-rw-rw-   0        0        0     1587 2024-05-03 16:17:07.000000 livedc-0.0.4/src/livedc/desc.py
+drwxrwxrwx   0        0        0        0 2024-05-07 00:58:38.755952 livedc-0.0.4/src/livedc/math/
+drwxrwxrwx   0        0        0        0 2024-05-07 00:58:38.779436 livedc-0.0.4/src/livedc/math/financial/
+-rw-rw-rw-   0        0        0     2585 2024-05-03 16:33:47.000000 livedc-0.0.4/src/livedc/math/financial/compound.py
+drwxrwxrwx   0        0        0        0 2024-05-07 00:58:38.782810 livedc-0.0.4/src/livedc.egg-info/
+-rw-rw-rw-   0        0        0     2132 2024-05-07 00:58:38.000000 livedc-0.0.4/src/livedc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2024-05-07 00:58:38.000000 livedc-0.0.4/src/livedc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 00:58:38.000000 livedc-0.0.4/src/livedc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-07 00:58:38.000000 livedc-0.0.4/src/livedc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       72 2024-05-07 00:58:38.000000 livedc-0.0.4/src/livedc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-07 00:58:38.000000 livedc-0.0.4/src/livedc.egg-info/top_level.txt
```

### Comparing `livedc-0.0.3/LICENSE` & `livedc-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `livedc-0.0.3/PKG-INFO` & `livedc-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livedc
-Version: 0.0.3
+Version: 0.0.4
 Summary: Useful mathmatical models/caculators for daily life and cloud deployment
 Author-email: jinsanity <jinsanityff@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 jinsanity07git
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,16 +29,17 @@
 Keywords: cpu,gpu,benchmark
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: nodespecs>=0.0.14
+Requires-Dist: nodespecs>=0.0.15
 Provides-Extra: dev
 Requires-Dist: GPUtil; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: psutil>=5.9.5; extra == "dev"
 Requires-Dist: toml; extra == "dev"
+Requires-Dist: pyomo==6.2; extra == "dev"
 
 # livedc
  useful mathmatical models/caculators for daily life and cloud deployment
```

### Comparing `livedc-0.0.3/pyproject.toml` & `livedc-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = [ "setuptools>=61.0.0", "wheel", "toml",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "livedc"
-version = "0.0.3"
+version = "0.0.4"
 description = "Useful mathmatical models/caculators for daily life and cloud deployment"
 readme = "README.md"
 classifiers = [ "License :: OSI Approved :: MIT License", "Programming Language :: Python", "Programming Language :: Python :: 3",]
 keywords = [ "cpu", "gpu", "benchmark",]
-dependencies = [ "nodespecs >= 0.0.14",]
+dependencies = [ "nodespecs >= 0.0.15",]
 requires-python = ">=3.6"
 [[project.authors]]
 name = "jinsanity"
 email = "jinsanityff@gmail.com"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
-dev = [ "GPUtil", "pip-tools", "psutil >= 5.9.5", "toml",]
+dev = [ "GPUtil", "pip-tools", "psutil >= 5.9.5", "toml", "pyomo==6.2",]
 
 [project.urls]
 Homepage = "https://github.com/jinsanity07git/livedc"
 
 [project.scripts]
 realpython = "specs.__main__:main"
```

### Comparing `livedc-0.0.3/setup.py` & `livedc-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `livedc-0.0.3/src/livedc/desc.py` & `livedc-0.0.4/src/livedc/desc.py`

 * *Files identical despite different names*

### Comparing `livedc-0.0.3/src/livedc/math/financial/compound.py` & `livedc-0.0.4/src/livedc/math/financial/compound.py`

 * *Files identical despite different names*

### Comparing `livedc-0.0.3/src/livedc.egg-info/PKG-INFO` & `livedc-0.0.4/src/livedc.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livedc
-Version: 0.0.3
+Version: 0.0.4
 Summary: Useful mathmatical models/caculators for daily life and cloud deployment
 Author-email: jinsanity <jinsanityff@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 jinsanity07git
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,16 +29,17 @@
 Keywords: cpu,gpu,benchmark
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: nodespecs>=0.0.14
+Requires-Dist: nodespecs>=0.0.15
 Provides-Extra: dev
 Requires-Dist: GPUtil; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: psutil>=5.9.5; extra == "dev"
 Requires-Dist: toml; extra == "dev"
+Requires-Dist: pyomo==6.2; extra == "dev"
 
 # livedc
  useful mathmatical models/caculators for daily life and cloud deployment
```

