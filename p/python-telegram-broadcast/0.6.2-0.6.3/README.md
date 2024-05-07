# Comparing `tmp/python-telegram-broadcast-0.6.2.tar.gz` & `tmp/python-telegram-broadcast-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-telegram-broadcast-0.6.2.tar", last modified: Tue May  7 02:01:19 2024, max compression
+gzip compressed data, was "python-telegram-broadcast-0.6.3.tar", last modified: Tue May  7 02:03:17 2024, max compression
```

## Comparing `python-telegram-broadcast-0.6.2.tar` & `python-telegram-broadcast-0.6.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 02:01:19.095337 python-telegram-broadcast-0.6.2/
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     1067 2024-05-06 01:52:00.000000 python-telegram-broadcast-0.6.2/LICENSE
--rw-r--r--   0 jonah     (1000) jonah     (1000)     1210 2024-05-07 02:01:19.095337 python-telegram-broadcast-0.6.2/PKG-INFO
--rw-rw-r--   0 jonah     (1000) jonah     (1000)      622 2024-05-07 02:00:34.000000 python-telegram-broadcast-0.6.2/README.md
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 02:01:19.095337 python-telegram-broadcast-0.6.2/python-telegram-broadcast/
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     2673 2024-05-06 08:59:24.000000 python-telegram-broadcast-0.6.2/python-telegram-broadcast/__init__.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     2963 2024-05-06 08:33:20.000000 python-telegram-broadcast-0.6.2/python-telegram-broadcast/custom_dataclass.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     1616 2024-05-06 08:35:01.000000 python-telegram-broadcast-0.6.2/python-telegram-broadcast/custom_exception.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     2236 2024-05-06 09:03:53.000000 python-telegram-broadcast-0.6.2/python-telegram-broadcast/custom_util.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     2417 2024-05-06 08:41:00.000000 python-telegram-broadcast-0.6.2/python-telegram-broadcast/main.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)    16983 2024-05-06 08:59:09.000000 python-telegram-broadcast-0.6.2/python-telegram-broadcast/send_method.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)    16160 2024-05-06 09:03:53.000000 python-telegram-broadcast-0.6.2/python-telegram-broadcast/strategy.py
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 02:01:19.095337 python-telegram-broadcast-0.6.2/python_telegram_broadcast.egg-info/
--rw-r--r--   0 jonah     (1000) jonah     (1000)     1210 2024-05-07 02:01:19.000000 python-telegram-broadcast-0.6.2/python_telegram_broadcast.egg-info/PKG-INFO
--rw-rw-r--   0 jonah     (1000) jonah     (1000)      554 2024-05-07 02:01:19.000000 python-telegram-broadcast-0.6.2/python_telegram_broadcast.egg-info/SOURCES.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)        1 2024-05-07 02:01:19.000000 python-telegram-broadcast-0.6.2/python_telegram_broadcast.egg-info/dependency_links.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)       33 2024-05-07 02:01:19.000000 python-telegram-broadcast-0.6.2/python_telegram_broadcast.egg-info/requires.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)       26 2024-05-07 02:01:19.000000 python-telegram-broadcast-0.6.2/python_telegram_broadcast.egg-info/top_level.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)       38 2024-05-07 02:01:19.095337 python-telegram-broadcast-0.6.2/setup.cfg
--rw-rw-r--   0 jonah     (1000) jonah     (1000)      952 2024-05-07 02:00:52.000000 python-telegram-broadcast-0.6.2/setup.py
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 02:03:17.301215 python-telegram-broadcast-0.6.3/
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     1067 2024-05-06 01:52:00.000000 python-telegram-broadcast-0.6.3/LICENSE
+-rw-r--r--   0 jonah     (1000) jonah     (1000)     1264 2024-05-07 02:03:17.297215 python-telegram-broadcast-0.6.3/PKG-INFO
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)      676 2024-05-07 02:02:51.000000 python-telegram-broadcast-0.6.3/README.md
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 02:03:17.297215 python-telegram-broadcast-0.6.3/python-telegram-broadcast/
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     2673 2024-05-06 08:59:24.000000 python-telegram-broadcast-0.6.3/python-telegram-broadcast/__init__.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     2963 2024-05-06 08:33:20.000000 python-telegram-broadcast-0.6.3/python-telegram-broadcast/custom_dataclass.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     1616 2024-05-06 08:35:01.000000 python-telegram-broadcast-0.6.3/python-telegram-broadcast/custom_exception.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     2236 2024-05-06 09:03:53.000000 python-telegram-broadcast-0.6.3/python-telegram-broadcast/custom_util.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     2417 2024-05-06 08:41:00.000000 python-telegram-broadcast-0.6.3/python-telegram-broadcast/main.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)    16983 2024-05-06 08:59:09.000000 python-telegram-broadcast-0.6.3/python-telegram-broadcast/send_method.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)    16160 2024-05-06 09:03:53.000000 python-telegram-broadcast-0.6.3/python-telegram-broadcast/strategy.py
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 02:03:17.297215 python-telegram-broadcast-0.6.3/python_telegram_broadcast.egg-info/
+-rw-r--r--   0 jonah     (1000) jonah     (1000)     1264 2024-05-07 02:03:17.000000 python-telegram-broadcast-0.6.3/python_telegram_broadcast.egg-info/PKG-INFO
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)      554 2024-05-07 02:03:17.000000 python-telegram-broadcast-0.6.3/python_telegram_broadcast.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)        1 2024-05-07 02:03:17.000000 python-telegram-broadcast-0.6.3/python_telegram_broadcast.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)       33 2024-05-07 02:03:17.000000 python-telegram-broadcast-0.6.3/python_telegram_broadcast.egg-info/requires.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)       26 2024-05-07 02:03:17.000000 python-telegram-broadcast-0.6.3/python_telegram_broadcast.egg-info/top_level.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)       38 2024-05-07 02:03:17.301215 python-telegram-broadcast-0.6.3/setup.cfg
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)      952 2024-05-07 02:03:04.000000 python-telegram-broadcast-0.6.3/setup.py
```

### Comparing `python-telegram-broadcast-0.6.2/LICENSE` & `python-telegram-broadcast-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-telegram-broadcast-0.6.2/PKG-INFO` & `python-telegram-broadcast-0.6.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: python-telegram-broadcast
-Version: 0.6.2
+Version: 0.6.3
 Summary: Package that wraps the python-telegram-bot library to make broadcasting easier.
 Author: jonah_whaler_2348
 Author-email: jk_saga@proton.me
 License: MIT
 Keywords: python,telegram,broadcast,bot
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-telegram-bot==21.1.1
 Requires-Dist: mypy
 
-![my-logo](./logo-mini.jpg "Python-Telegram-Broadcast-Logo")
+![my-logo](https://jonahtzuchi.github.io/python-telegram-broadcast/logo-mini.jpg "Python-Telegram-Broadcast-Logo")
 
 # Python Telegram Broadcast
 
 This is a simple Python package that build on top of [python-telegram-bot](https://pypi.org/project/python-telegram-bot/) to make broadcasting easier.
 
 
 ## Features
```

### Comparing `python-telegram-broadcast-0.6.2/python-telegram-broadcast/__init__.py` & `python-telegram-broadcast-0.6.3/python-telegram-broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `python-telegram-broadcast-0.6.2/python-telegram-broadcast/custom_dataclass.py` & `python-telegram-broadcast-0.6.3/python-telegram-broadcast/custom_dataclass.py`

 * *Files identical despite different names*

### Comparing `python-telegram-broadcast-0.6.2/python-telegram-broadcast/custom_exception.py` & `python-telegram-broadcast-0.6.3/python-telegram-broadcast/custom_exception.py`

 * *Files identical despite different names*

### Comparing `python-telegram-broadcast-0.6.2/python-telegram-broadcast/custom_util.py` & `python-telegram-broadcast-0.6.3/python-telegram-broadcast/custom_util.py`

 * *Files identical despite different names*

### Comparing `python-telegram-broadcast-0.6.2/python-telegram-broadcast/main.py` & `python-telegram-broadcast-0.6.3/python-telegram-broadcast/main.py`

 * *Files identical despite different names*

### Comparing `python-telegram-broadcast-0.6.2/python-telegram-broadcast/send_method.py` & `python-telegram-broadcast-0.6.3/python-telegram-broadcast/send_method.py`

 * *Files identical despite different names*

### Comparing `python-telegram-broadcast-0.6.2/python-telegram-broadcast/strategy.py` & `python-telegram-broadcast-0.6.3/python-telegram-broadcast/strategy.py`

 * *Files identical despite different names*

### Comparing `python-telegram-broadcast-0.6.2/python_telegram_broadcast.egg-info/PKG-INFO` & `python-telegram-broadcast-0.6.3/python_telegram_broadcast.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: python-telegram-broadcast
-Version: 0.6.2
+Version: 0.6.3
 Summary: Package that wraps the python-telegram-bot library to make broadcasting easier.
 Author: jonah_whaler_2348
 Author-email: jk_saga@proton.me
 License: MIT
 Keywords: python,telegram,broadcast,bot
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-telegram-bot==21.1.1
 Requires-Dist: mypy
 
-![my-logo](./logo-mini.jpg "Python-Telegram-Broadcast-Logo")
+![my-logo](https://jonahtzuchi.github.io/python-telegram-broadcast/logo-mini.jpg "Python-Telegram-Broadcast-Logo")
 
 # Python Telegram Broadcast
 
 This is a simple Python package that build on top of [python-telegram-bot](https://pypi.org/project/python-telegram-bot/) to make broadcasting easier.
 
 
 ## Features
```

### Comparing `python-telegram-broadcast-0.6.2/python_telegram_broadcast.egg-info/SOURCES.txt` & `python-telegram-broadcast-0.6.3/python_telegram_broadcast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-telegram-broadcast-0.6.2/setup.py` & `python-telegram-broadcast-0.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 DESCRIPTION = 'Package that wraps the python-telegram-bot library to make broadcasting easier.'
 
 # python3 setup.py sdist bdist_wheel
 # twine upload --skip-existing dist/*
 
-VERSION = '0.6.2'
+VERSION = '0.6.3'
 
 setup(
     name='python-telegram-broadcast',
     version=VERSION,
     packages=find_packages(),
     description=DESCRIPTION,
     long_description=open('README.md').read(),
```

