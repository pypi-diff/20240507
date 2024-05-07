# Comparing `tmp/rlanutils-0.1.8.tar.gz` & `tmp/rlanutils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlanutils-0.1.8.tar", last modified: Mon Apr 29 07:50:54 2024, max compression
+gzip compressed data, was "rlanutils-0.1.9.tar", last modified: Tue May  7 03:08:05 2024, max compression
```

## Comparing `rlanutils-0.1.8.tar` & `rlanutils-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 07:50:54.048966 rlanutils-0.1.8/
--rw-r--r--   0 rlan       (501) staff       (20)      343 2024-04-29 07:50:54.048804 rlanutils-0.1.8/PKG-INFO
--rw-r--r--   0 rlan       (501) staff       (20)       78 2024-04-28 07:35:44.000000 rlanutils-0.1.8/README.md
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 07:50:54.044304 rlanutils-0.1.8/rlanutils/
--rw-r--r--   0 rlan       (501) staff       (20)        0 2024-04-28 06:25:11.000000 rlanutils-0.1.8/rlanutils/__init__.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 07:50:54.045791 rlanutils-0.1.8/rlanutils/cv/
--rw-r--r--   0 rlan       (501) staff       (20)        0 2024-04-29 03:30:45.000000 rlanutils-0.1.8/rlanutils/cv/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)     3433 2024-04-29 07:28:15.000000 rlanutils-0.1.8/rlanutils/cv/geometry.py
--rw-r--r--   0 rlan       (501) staff       (20)     2900 2024-04-28 08:49:32.000000 rlanutils-0.1.8/rlanutils/cv/graphics.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 07:50:54.046169 rlanutils-0.1.8/rlanutils/data_structure/
--rw-r--r--   0 rlan       (501) staff       (20)        0 2024-04-29 03:31:00.000000 rlanutils-0.1.8/rlanutils/data_structure/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)      646 2024-04-28 07:15:05.000000 rlanutils-0.1.8/rlanutils/data_structure/set.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 07:50:54.047597 rlanutils-0.1.8/rlanutils/io/
--rw-r--r--   0 rlan       (501) staff       (20)        0 2024-04-29 03:30:50.000000 rlanutils-0.1.8/rlanutils/io/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)      671 2024-04-29 03:19:35.000000 rlanutils-0.1.8/rlanutils/io/args.py
--rw-r--r--   0 rlan       (501) staff       (20)     1487 2024-04-28 07:19:30.000000 rlanutils-0.1.8/rlanutils/io/fs.py
--rw-r--r--   0 rlan       (501) staff       (20)     2686 2024-04-28 07:16:44.000000 rlanutils-0.1.8/rlanutils/io/indices.py
--rw-r--r--   0 rlan       (501) staff       (20)      682 2024-04-28 07:16:21.000000 rlanutils-0.1.8/rlanutils/io/network.py
--rw-r--r--   0 rlan       (501) staff       (20)     1441 2024-04-28 07:16:14.000000 rlanutils-0.1.8/rlanutils/io/parallelism.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 07:50:54.048439 rlanutils-0.1.8/rlanutils/plot/
--rw-r--r--   0 rlan       (501) staff       (20)      118 2024-04-28 07:15:29.000000 rlanutils-0.1.8/rlanutils/plot/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)     1256 2024-04-28 07:17:37.000000 rlanutils-0.1.8/rlanutils/plot/color.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 07:50:54.045249 rlanutils-0.1.8/rlanutils.egg-info/
--rw-r--r--   0 rlan       (501) staff       (20)      343 2024-04-29 07:50:53.000000 rlanutils-0.1.8/rlanutils.egg-info/PKG-INFO
--rw-r--r--   0 rlan       (501) staff       (20)      540 2024-04-29 07:50:54.000000 rlanutils-0.1.8/rlanutils.egg-info/SOURCES.txt
--rw-r--r--   0 rlan       (501) staff       (20)        1 2024-04-29 07:50:53.000000 rlanutils-0.1.8/rlanutils.egg-info/dependency_links.txt
--rw-r--r--   0 rlan       (501) staff       (20)       35 2024-04-29 07:50:53.000000 rlanutils-0.1.8/rlanutils.egg-info/requires.txt
--rw-r--r--   0 rlan       (501) staff       (20)       10 2024-04-29 07:50:53.000000 rlanutils-0.1.8/rlanutils.egg-info/top_level.txt
--rw-r--r--   0 rlan       (501) staff       (20)       38 2024-04-29 07:50:54.049019 rlanutils-0.1.8/setup.cfg
--rw-r--r--   0 rlan       (501) staff       (20)      538 2024-04-29 07:50:35.000000 rlanutils-0.1.8/setup.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-07 03:08:05.240431 rlanutils-0.1.9/
+-rw-r--r--   0 rlan       (501) staff       (20)      475 2024-05-07 03:08:05.240167 rlanutils-0.1.9/PKG-INFO
+-rw-r--r--   0 rlan       (501) staff       (20)       78 2024-04-28 07:35:44.000000 rlanutils-0.1.9/README.md
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-07 03:08:05.237520 rlanutils-0.1.9/rlanutils/
+-rw-r--r--   0 rlan       (501) staff       (20)        0 2024-04-28 06:25:11.000000 rlanutils-0.1.9/rlanutils/__init__.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-07 03:08:05.238500 rlanutils-0.1.9/rlanutils/cv/
+-rw-r--r--   0 rlan       (501) staff       (20)        0 2024-04-29 03:30:45.000000 rlanutils-0.1.9/rlanutils/cv/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)     3433 2024-04-29 07:28:15.000000 rlanutils-0.1.9/rlanutils/cv/geometry.py
+-rw-r--r--   0 rlan       (501) staff       (20)     2900 2024-04-28 08:49:32.000000 rlanutils-0.1.9/rlanutils/cv/graphics.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-07 03:08:05.238715 rlanutils-0.1.9/rlanutils/data_structure/
+-rw-r--r--   0 rlan       (501) staff       (20)        0 2024-04-29 03:31:00.000000 rlanutils-0.1.9/rlanutils/data_structure/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)      646 2024-04-28 07:15:05.000000 rlanutils-0.1.9/rlanutils/data_structure/set.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-07 03:08:05.239628 rlanutils-0.1.9/rlanutils/io/
+-rw-r--r--   0 rlan       (501) staff       (20)        0 2024-04-29 03:30:50.000000 rlanutils-0.1.9/rlanutils/io/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)      671 2024-04-29 03:19:35.000000 rlanutils-0.1.9/rlanutils/io/args.py
+-rw-r--r--   0 rlan       (501) staff       (20)     1624 2024-05-07 03:05:59.000000 rlanutils-0.1.9/rlanutils/io/fs.py
+-rw-r--r--   0 rlan       (501) staff       (20)     2686 2024-04-28 07:16:44.000000 rlanutils-0.1.9/rlanutils/io/indices.py
+-rw-r--r--   0 rlan       (501) staff       (20)      682 2024-04-28 07:16:21.000000 rlanutils-0.1.9/rlanutils/io/network.py
+-rw-r--r--   0 rlan       (501) staff       (20)     1441 2024-04-28 07:16:14.000000 rlanutils-0.1.9/rlanutils/io/parallelism.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-07 03:08:05.239882 rlanutils-0.1.9/rlanutils/plot/
+-rw-r--r--   0 rlan       (501) staff       (20)      118 2024-04-28 07:15:29.000000 rlanutils-0.1.9/rlanutils/plot/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)     1256 2024-04-28 07:17:37.000000 rlanutils-0.1.9/rlanutils/plot/color.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-07 03:08:05.238073 rlanutils-0.1.9/rlanutils.egg-info/
+-rw-r--r--   0 rlan       (501) staff       (20)      475 2024-05-07 03:08:05.000000 rlanutils-0.1.9/rlanutils.egg-info/PKG-INFO
+-rw-r--r--   0 rlan       (501) staff       (20)      540 2024-05-07 03:08:05.000000 rlanutils-0.1.9/rlanutils.egg-info/SOURCES.txt
+-rw-r--r--   0 rlan       (501) staff       (20)        1 2024-05-07 03:08:05.000000 rlanutils-0.1.9/rlanutils.egg-info/dependency_links.txt
+-rw-r--r--   0 rlan       (501) staff       (20)       42 2024-05-07 03:08:05.000000 rlanutils-0.1.9/rlanutils.egg-info/requires.txt
+-rw-r--r--   0 rlan       (501) staff       (20)       10 2024-05-07 03:08:05.000000 rlanutils-0.1.9/rlanutils.egg-info/top_level.txt
+-rw-r--r--   0 rlan       (501) staff       (20)       38 2024-05-07 03:08:05.240481 rlanutils-0.1.9/setup.cfg
+-rw-r--r--   0 rlan       (501) staff       (20)      556 2024-05-07 01:57:01.000000 rlanutils-0.1.9/setup.py
```

### Comparing `rlanutils-0.1.8/rlanutils/cv/geometry.py` & `rlanutils-0.1.9/rlanutils/cv/geometry.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.8/rlanutils/cv/graphics.py` & `rlanutils-0.1.9/rlanutils/cv/graphics.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.8/rlanutils/data_structure/set.py` & `rlanutils-0.1.9/rlanutils/data_structure/set.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.8/rlanutils/io/args.py` & `rlanutils-0.1.9/rlanutils/io/args.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.8/rlanutils/io/fs.py` & `rlanutils-0.1.9/rlanutils/io/fs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pathlib import Path
 import functools
 import tempfile
 import json
+import yaml
 from typing import List, Dict, Union
 
 
 def read_json(path: Path) -> Union[Dict, List[Dict]]:
     with open(path) as f:
         j = json.load(f)
     return j
@@ -15,14 +16,20 @@
     with open(path, "w") as f:
         if prettify:
             json.dump(json_data, f, indent=4)
         else:
             json.dump(json_data, f)
 
 
+def read_yaml(path: Path) -> Union[Dict, List[Dict]]:
+    with open(path) as f:
+        y = yaml.safe_load(f)
+    return y
+
+
 def create_empty_temp_file(prefix=None, suffix=None) -> Path:
     _, path = tempfile.mkstemp(prefix=prefix, suffix=suffix, text=True)
     return Path(path)
 
 
 def mktmpdir():
     tmp_dir = Path(tempfile.mktemp())
```

### Comparing `rlanutils-0.1.8/rlanutils/io/indices.py` & `rlanutils-0.1.9/rlanutils/io/indices.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.8/rlanutils/io/network.py` & `rlanutils-0.1.9/rlanutils/io/network.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.8/rlanutils/io/parallelism.py` & `rlanutils-0.1.9/rlanutils/io/parallelism.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.8/rlanutils/plot/color.py` & `rlanutils-0.1.9/rlanutils/plot/color.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.8/rlanutils.egg-info/SOURCES.txt` & `rlanutils-0.1.9/rlanutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.8/setup.py` & `rlanutils-0.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='rlanutils',
-    version='0.1.8',
+    version='0.1.9',
     packages=find_packages(),
     description='A handy tool that make your day to day programming much easier. ',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='brianlan',
     author_email='brianlanbo@gmail.com',
     url='https://gitlab.com/rlan/rlanutils',
     install_requires=[
         "numpy",
         "scipy",
         "tqdm",
         "matplotlib",
         "pytest",
+        "pyyaml",
     ],
 )
```

