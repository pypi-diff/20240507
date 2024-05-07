# Comparing `tmp/devinci_pybuilder-0.0.3.tar.gz` & `tmp/devinci_pybuilder-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devinci_pybuilder-0.0.3.tar", last modified: Tue May  7 03:31:15 2024, max compression
+gzip compressed data, was "devinci_pybuilder-0.1.0.tar", last modified: Tue May  7 06:54:52 2024, max compression
```

## Comparing `devinci_pybuilder-0.0.3.tar` & `devinci_pybuilder-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 vince     (1001) vince     (1001)        0 2024-05-07 03:31:15.589667 devinci_pybuilder-0.0.3/
--rw-r--r--   0 vince     (1001) vince     (1001)     1249 2024-05-06 20:34:04.000000 devinci_pybuilder-0.0.3/LICENSE.md
--rw-r--r--   0 vince     (1001) vince     (1001)     1614 2024-05-07 03:31:15.589667 devinci_pybuilder-0.0.3/PKG-INFO
--rw-r--r--   0 vince     (1001) vince     (1001)     1311 2024-05-06 20:17:12.000000 devinci_pybuilder-0.0.3/README.md
-drwxr-xr-x   0 vince     (1001) vince     (1001)        0 2024-05-07 03:31:15.585667 devinci_pybuilder-0.0.3/devinci_pybuilder/
--rw-r--r--   0 vince     (1001) vince     (1001)       48 2024-05-07 00:04:03.000000 devinci_pybuilder-0.0.3/devinci_pybuilder/__init__.py
-drwxr-xr-x   0 vince     (1001) vince     (1001)        0 2024-05-07 03:31:15.589667 devinci_pybuilder-0.0.3/devinci_pybuilder/build_chores/
--rw-r--r--   0 vince     (1001) vince     (1001)       56 2024-05-07 02:14:03.000000 devinci_pybuilder-0.0.3/devinci_pybuilder/build_chores/__init__.py
--rw-r--r--   0 vince     (1001) vince     (1001)     3261 2024-05-06 23:57:31.000000 devinci_pybuilder-0.0.3/devinci_pybuilder/build_chores/custom_install_command.py
--rw-r--r--   0 vince     (1001) vince     (1001)     3874 2024-05-06 20:14:57.000000 devinci_pybuilder-0.0.3/devinci_pybuilder/builder.py
--rw-r--r--   0 vince     (1001) vince     (1001)     5101 2024-05-06 21:33:22.000000 devinci_pybuilder-0.0.3/devinci_pybuilder/devinci_pybuilder.py
--rw-r--r--   0 vince     (1001) vince     (1001)     1525 2024-05-06 20:35:33.000000 devinci_pybuilder-0.0.3/devinci_pybuilder/file_utils.py
--rw-r--r--   0 vince     (1001) vince     (1001)     6015 2024-05-07 03:09:00.000000 devinci_pybuilder-0.0.3/devinci_pybuilder/main.py
-drwxr-xr-x   0 vince     (1001) vince     (1001)        0 2024-05-07 03:31:15.589667 devinci_pybuilder-0.0.3/devinci_pybuilder/stub/
--rw-r--r--   0 vince     (1001) vince     (1001)     1300 2024-05-07 02:35:29.000000 devinci_pybuilder-0.0.3/devinci_pybuilder/stub/example-config.ini
-drwxr-xr-x   0 vince     (1001) vince     (1001)        0 2024-05-07 03:31:15.589667 devinci_pybuilder-0.0.3/devinci_pybuilder.egg-info/
--rw-r--r--   0 vince     (1001) vince     (1001)     1614 2024-05-07 03:31:15.000000 devinci_pybuilder-0.0.3/devinci_pybuilder.egg-info/PKG-INFO
--rw-r--r--   0 vince     (1001) vince     (1001)      575 2024-05-07 03:31:15.000000 devinci_pybuilder-0.0.3/devinci_pybuilder.egg-info/SOURCES.txt
--rw-r--r--   0 vince     (1001) vince     (1001)       40 2024-05-07 03:31:15.000000 devinci_pybuilder-0.0.3/devinci_pybuilder.egg-info/dependency_links.txt
--rw-r--r--   0 vince     (1001) vince     (1001)       64 2024-05-07 03:31:15.000000 devinci_pybuilder-0.0.3/devinci_pybuilder.egg-info/entry_points.txt
--rw-r--r--   0 vince     (1001) vince     (1001)       16 2024-05-07 03:31:15.000000 devinci_pybuilder-0.0.3/devinci_pybuilder.egg-info/requires.txt
--rw-r--r--   0 vince     (1001) vince     (1001)       18 2024-05-07 03:31:15.000000 devinci_pybuilder-0.0.3/devinci_pybuilder.egg-info/top_level.txt
--rw-r--r--   0 vince     (1001) vince     (1001)       38 2024-05-07 03:31:15.589667 devinci_pybuilder-0.0.3/setup.cfg
--rw-r--r--   0 vince     (1001) vince     (1001)     1054 2024-05-07 03:31:08.000000 devinci_pybuilder-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:54:52.176157 devinci_pybuilder-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-07 06:54:46.000000 devinci_pybuilder-0.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-07 06:54:52.176157 devinci_pybuilder-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-07 06:54:46.000000 devinci_pybuilder-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:54:52.176157 devinci_pybuilder-0.1.0/devinci_pybuilder/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-07 06:54:46.000000 devinci_pybuilder-0.1.0/devinci_pybuilder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:54:52.176157 devinci_pybuilder-0.1.0/devinci_pybuilder/build_chores/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-07 06:54:46.000000 devinci_pybuilder-0.1.0/devinci_pybuilder/build_chores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-07 06:54:46.000000 devinci_pybuilder-0.1.0/devinci_pybuilder/build_chores/custom_install_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-05-07 06:54:46.000000 devinci_pybuilder-0.1.0/devinci_pybuilder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-07 06:54:46.000000 devinci_pybuilder-0.1.0/devinci_pybuilder/devinci_pybuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-07 06:54:46.000000 devinci_pybuilder-0.1.0/devinci_pybuilder/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-07 06:54:46.000000 devinci_pybuilder-0.1.0/devinci_pybuilder/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:54:52.176157 devinci_pybuilder-0.1.0/devinci_pybuilder/stub/
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-07 06:54:46.000000 devinci_pybuilder-0.1.0/devinci_pybuilder/stub/example-config.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:54:52.176157 devinci_pybuilder-0.1.0/devinci_pybuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-07 06:54:52.000000 devinci_pybuilder-0.1.0/devinci_pybuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-07 06:54:52.000000 devinci_pybuilder-0.1.0/devinci_pybuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-07 06:54:52.000000 devinci_pybuilder-0.1.0/devinci_pybuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-07 06:54:52.000000 devinci_pybuilder-0.1.0/devinci_pybuilder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 06:54:52.000000 devinci_pybuilder-0.1.0/devinci_pybuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 06:54:52.000000 devinci_pybuilder-0.1.0/devinci_pybuilder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 06:54:52.176157 devinci_pybuilder-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-07 06:54:51.000000 devinci_pybuilder-0.1.0/setup.py
```

### Comparing `devinci_pybuilder-0.0.3/LICENSE.md` & `devinci_pybuilder-0.1.0/LICENSE.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# LICENSE.md
+d# LICENSE.md
 
 ***&copy; 2024 | [devinci-it](https://github.com/devinci-it)***
     
     
 <pre style="text-align:center; max-width: 55ch; margin: 0 auto;">
 
     Permission is hereby granted, free of charge, to any person obtaining
```

### Comparing `devinci_pybuilder-0.0.3/PKG-INFO` & `devinci_pybuilder-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devinci-pybuilder
-Version: 0.0.3
+Version: 0.1.0
 Summary: devinci_pybuilder is a Python package builder for managing project setup and generating setup.py files.
 Author: devinci-it
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: devinci_pyutils
```

### Comparing `devinci_pybuilder-0.0.3/README.md` & `devinci_pybuilder-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `devinci_pybuilder-0.0.3/devinci_pybuilder/build_chores/custom_install_command.py` & `devinci_pybuilder-0.1.0/devinci_pybuilder/build_chores/custom_install_command.py`

 * *Files identical despite different names*

### Comparing `devinci_pybuilder-0.0.3/devinci_pybuilder/builder.py` & `devinci_pybuilder-0.1.0/devinci_pybuilder/builder.py`

 * *Files identical despite different names*

### Comparing `devinci_pybuilder-0.0.3/devinci_pybuilder/devinci_pybuilder.py` & `devinci_pybuilder-0.1.0/devinci_pybuilder/devinci_pybuilder.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 - Ensure that the `config.ini` file and `requirements.txt` file are present in the project directory.
 - Customize the configurations in the `config.ini` file according to the project requirements.
 """
 
 
 import configparser
 from typing import List, Dict
-
+from devinci_pyutils import banner
 def _read_config_section(config_file: str = 'config.ini', section: str = 'General') -> Dict[str, str]:
     """
     Read a specific section from the configuration file and return it as a dictionary.
 
     Args:
         config_file (str): Path to the configuration file. Default is 'config.ini'.
         section (str): Name of the section to read from the configuration file. Default is 'General'.
```

### Comparing `devinci_pybuilder-0.0.3/devinci_pybuilder/file_utils.py` & `devinci_pybuilder-0.1.0/devinci_pybuilder/file_utils.py`

 * *Files identical despite different names*

### Comparing `devinci_pybuilder-0.0.3/devinci_pybuilder/main.py` & `devinci_pybuilder-0.1.0/devinci_pybuilder/main.py`

 * *Files identical despite different names*

### Comparing `devinci_pybuilder-0.0.3/devinci_pybuilder/stub/example-config.ini` & `devinci_pybuilder-0.1.0/devinci_pybuilder/stub/example-config.ini`

 * *Files identical despite different names*

### Comparing `devinci_pybuilder-0.0.3/devinci_pybuilder.egg-info/PKG-INFO` & `devinci_pybuilder-0.1.0/devinci_pybuilder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devinci-pybuilder
-Version: 0.0.3
+Version: 0.1.0
 Summary: devinci_pybuilder is a Python package builder for managing project setup and generating setup.py files.
 Author: devinci-it
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: devinci_pyutils
```

### Comparing `devinci_pybuilder-0.0.3/devinci_pybuilder.egg-info/SOURCES.txt` & `devinci_pybuilder-0.1.0/devinci_pybuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devinci_pybuilder-0.0.3/setup.py` & `devinci_pybuilder-0.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 import os
 from typing import Type
-from devinci_pybuilder.build_chores import CustomInstallCommand
+from devinci_pybuilder.build_chores.custom_install_command import CustomInstallCommand
 
 setup(
     name='devinci-pybuilder',
-    version='0.0.3',
+    version='v0.1.0',
     description='devinci_pybuilder is a Python package builder for managing project setup and generating setup.py files.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     license='MIT',
     author='devinci-it',
     packages=find_packages(),
     scripts=['devinci_pybuilder/builder.py', 'devinci_pybuilder/file_utils.py', 'devinci_pybuilder/main.py'],
```

