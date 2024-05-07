# Comparing `tmp/python_telegram_broadcast-0.9.2.tar.gz` & `tmp/python_telegram_broadcast-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_telegram_broadcast-0.9.2.tar", last modified: Tue May  7 06:42:32 2024, max compression
+gzip compressed data, was "python_telegram_broadcast-0.9.3.tar", last modified: Tue May  7 07:02:19 2024, max compression
```

## Comparing `python_telegram_broadcast-0.9.2.tar` & `python_telegram_broadcast-0.9.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 06:42:32.984118 python_telegram_broadcast-0.9.2/
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     1067 2024-05-06 01:52:00.000000 python_telegram_broadcast-0.9.2/LICENSE
--rw-r--r--   0 jonah     (1000) jonah     (1000)     3920 2024-05-07 06:42:32.984118 python_telegram_broadcast-0.9.2/PKG-INFO
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     3331 2024-05-07 02:48:22.000000 python_telegram_broadcast-0.9.2/README.md
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 06:42:32.980118 python_telegram_broadcast-0.9.2/python_telegram_broadcast/
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     3051 2024-05-07 03:28:42.000000 python_telegram_broadcast-0.9.2/python_telegram_broadcast/__init__.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     2963 2024-05-06 08:33:20.000000 python_telegram_broadcast-0.9.2/python_telegram_broadcast/custom_dataclass.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     1616 2024-05-06 08:35:01.000000 python_telegram_broadcast-0.9.2/python_telegram_broadcast/custom_exception.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     2236 2024-05-06 09:03:53.000000 python_telegram_broadcast-0.9.2/python_telegram_broadcast/custom_util.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     2757 2024-05-07 06:32:49.000000 python_telegram_broadcast-0.9.2/python_telegram_broadcast/main.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)    16983 2024-05-06 08:59:09.000000 python_telegram_broadcast-0.9.2/python_telegram_broadcast/send_method.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)    16782 2024-05-07 06:41:55.000000 python_telegram_broadcast-0.9.2/python_telegram_broadcast/strategy.py
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 06:42:32.980118 python_telegram_broadcast-0.9.2/python_telegram_broadcast.egg-info/
--rw-r--r--   0 jonah     (1000) jonah     (1000)     3920 2024-05-07 06:42:32.000000 python_telegram_broadcast-0.9.2/python_telegram_broadcast.egg-info/PKG-INFO
--rw-rw-r--   0 jonah     (1000) jonah     (1000)      554 2024-05-07 06:42:32.000000 python_telegram_broadcast-0.9.2/python_telegram_broadcast.egg-info/SOURCES.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)        1 2024-05-07 06:42:32.000000 python_telegram_broadcast-0.9.2/python_telegram_broadcast.egg-info/dependency_links.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)       33 2024-05-07 06:42:32.000000 python_telegram_broadcast-0.9.2/python_telegram_broadcast.egg-info/requires.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)       26 2024-05-07 06:42:32.000000 python_telegram_broadcast-0.9.2/python_telegram_broadcast.egg-info/top_level.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)       38 2024-05-07 06:42:32.984118 python_telegram_broadcast-0.9.2/setup.cfg
--rw-rw-r--   0 jonah     (1000) jonah     (1000)      952 2024-05-07 06:42:17.000000 python_telegram_broadcast-0.9.2/setup.py
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 07:02:19.528690 python_telegram_broadcast-0.9.3/
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     1067 2024-05-06 01:52:00.000000 python_telegram_broadcast-0.9.3/LICENSE
+-rw-r--r--   0 jonah     (1000) jonah     (1000)     3920 2024-05-07 07:02:19.528690 python_telegram_broadcast-0.9.3/PKG-INFO
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     3331 2024-05-07 02:48:22.000000 python_telegram_broadcast-0.9.3/README.md
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 07:02:19.528690 python_telegram_broadcast-0.9.3/python_telegram_broadcast/
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     4268 2024-05-07 07:01:41.000000 python_telegram_broadcast-0.9.3/python_telegram_broadcast/__init__.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     4039 2024-05-07 06:58:19.000000 python_telegram_broadcast-0.9.3/python_telegram_broadcast/custom_dataclass.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     1616 2024-05-06 08:35:01.000000 python_telegram_broadcast-0.9.3/python_telegram_broadcast/custom_exception.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     3338 2024-05-07 06:58:49.000000 python_telegram_broadcast-0.9.3/python_telegram_broadcast/custom_util.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     3859 2024-05-07 06:57:58.000000 python_telegram_broadcast-0.9.3/python_telegram_broadcast/main.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)    18085 2024-05-07 06:57:43.000000 python_telegram_broadcast-0.9.3/python_telegram_broadcast/send_method.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)    17860 2024-05-07 06:57:50.000000 python_telegram_broadcast-0.9.3/python_telegram_broadcast/strategy.py
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 07:02:19.528690 python_telegram_broadcast-0.9.3/python_telegram_broadcast.egg-info/
+-rw-r--r--   0 jonah     (1000) jonah     (1000)     3920 2024-05-07 07:02:19.000000 python_telegram_broadcast-0.9.3/python_telegram_broadcast.egg-info/PKG-INFO
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)      554 2024-05-07 07:02:19.000000 python_telegram_broadcast-0.9.3/python_telegram_broadcast.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)        1 2024-05-07 07:02:19.000000 python_telegram_broadcast-0.9.3/python_telegram_broadcast.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)       33 2024-05-07 07:02:19.000000 python_telegram_broadcast-0.9.3/python_telegram_broadcast.egg-info/requires.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)       26 2024-05-07 07:02:19.000000 python_telegram_broadcast-0.9.3/python_telegram_broadcast.egg-info/top_level.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)       38 2024-05-07 07:02:19.528690 python_telegram_broadcast-0.9.3/setup.cfg
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)      952 2024-05-07 07:01:58.000000 python_telegram_broadcast-0.9.3/setup.py
```

### Comparing `python_telegram_broadcast-0.9.2/LICENSE` & `python_telegram_broadcast-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.2/PKG-INFO` & `python_telegram_broadcast-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_telegram_broadcast
-Version: 0.9.2
+Version: 0.9.3
 Summary: Package that wraps the python-telegram-bot library to make broadcasting easier.
 Author: jonah_whaler_2348
 Author-email: jk_saga@proton.me
 License: MIT
 Keywords: python,telegram,broadcast,bot
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `python_telegram_broadcast-0.9.2/README.md` & `python_telegram_broadcast-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.2/python_telegram_broadcast/custom_exception.py` & `python_telegram_broadcast-0.9.3/python_telegram_broadcast/custom_exception.py`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.2/python_telegram_broadcast/send_method.py` & `python_telegram_broadcast-0.9.3/python_telegram_broadcast/send_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+"""
+MIT License
+
+Copyright (c) 2024 Jonah Whaler
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
 import asyncio
 import time
 import traceback
 from enum import Enum
 
 import telegram
 from telegram import Message, PhotoSize, Document, Video
```

### Comparing `python_telegram_broadcast-0.9.2/python_telegram_broadcast/strategy.py` & `python_telegram_broadcast-0.9.3/python_telegram_broadcast/strategy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+"""
+MIT License
+
+Copyright (c) 2024 Jonah Whaler
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
 import os
 import traceback
 import asyncio
 
 import concurrent.futures
 from functools import partial
```

### Comparing `python_telegram_broadcast-0.9.2/python_telegram_broadcast.egg-info/PKG-INFO` & `python_telegram_broadcast-0.9.3/python_telegram_broadcast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-telegram-broadcast
-Version: 0.9.2
+Version: 0.9.3
 Summary: Package that wraps the python-telegram-bot library to make broadcasting easier.
 Author: jonah_whaler_2348
 Author-email: jk_saga@proton.me
 License: MIT
 Keywords: python,telegram,broadcast,bot
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `python_telegram_broadcast-0.9.2/python_telegram_broadcast.egg-info/SOURCES.txt` & `python_telegram_broadcast-0.9.3/python_telegram_broadcast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.2/setup.py` & `python_telegram_broadcast-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 DESCRIPTION = 'Package that wraps the python-telegram-bot library to make broadcasting easier.'
 
 # python3 setup.py sdist bdist_wheel
 # twine upload --skip-existing dist/*
 
-VERSION = '0.9.2'
+VERSION = '0.9.3'
 
 setup(
     name='python_telegram_broadcast',
     version=VERSION,
     packages=find_packages(),
     description=DESCRIPTION,
     long_description=open('README.md').read(),
```

