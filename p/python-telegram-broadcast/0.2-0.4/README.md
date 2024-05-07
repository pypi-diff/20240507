# Comparing `tmp/python-telegram-broadcast-0.2.tar.gz` & `tmp/python-telegram-broadcast-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-telegram-broadcast-0.2.tar", last modified: Mon May  6 09:20:03 2024, max compression
+gzip compressed data, was "python-telegram-broadcast-0.4.tar", last modified: Mon May  6 10:47:16 2024, max compression
```

## Comparing `python-telegram-broadcast-0.2.tar` & `python-telegram-broadcast-0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-06 09:20:03.482513 python-telegram-broadcast-0.2/
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     1067 2024-05-06 01:52:00.000000 python-telegram-broadcast-0.2/LICENSE
--rw-r--r--   0 jonah     (1000) jonah     (1000)      614 2024-05-06 09:20:03.482513 python-telegram-broadcast-0.2/PKG-INFO
--rw-rw-r--   0 jonah     (1000) jonah     (1000)       27 2024-05-06 01:52:00.000000 python-telegram-broadcast-0.2/README.md
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-06 09:20:03.482513 python-telegram-broadcast-0.2/python-telegram-broadcast/
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     2673 2024-05-06 08:59:24.000000 python-telegram-broadcast-0.2/python-telegram-broadcast/__init__.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     2963 2024-05-06 08:33:20.000000 python-telegram-broadcast-0.2/python-telegram-broadcast/custom_dataclass.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     1616 2024-05-06 08:35:01.000000 python-telegram-broadcast-0.2/python-telegram-broadcast/custom_exception.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     2236 2024-05-06 09:03:53.000000 python-telegram-broadcast-0.2/python-telegram-broadcast/custom_util.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     2417 2024-05-06 08:41:00.000000 python-telegram-broadcast-0.2/python-telegram-broadcast/main.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)    16983 2024-05-06 08:59:09.000000 python-telegram-broadcast-0.2/python-telegram-broadcast/send_method.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)    16160 2024-05-06 09:03:53.000000 python-telegram-broadcast-0.2/python-telegram-broadcast/strategy.py
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-06 09:20:03.482513 python-telegram-broadcast-0.2/python_telegram_broadcast.egg-info/
--rw-r--r--   0 jonah     (1000) jonah     (1000)      614 2024-05-06 09:20:03.000000 python-telegram-broadcast-0.2/python_telegram_broadcast.egg-info/PKG-INFO
--rw-rw-r--   0 jonah     (1000) jonah     (1000)      554 2024-05-06 09:20:03.000000 python-telegram-broadcast-0.2/python_telegram_broadcast.egg-info/SOURCES.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)        1 2024-05-06 09:20:03.000000 python-telegram-broadcast-0.2/python_telegram_broadcast.egg-info/dependency_links.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)       33 2024-05-06 09:20:03.000000 python-telegram-broadcast-0.2/python_telegram_broadcast.egg-info/requires.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)       26 2024-05-06 09:20:03.000000 python-telegram-broadcast-0.2/python_telegram_broadcast.egg-info/top_level.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)       38 2024-05-06 09:20:03.482513 python-telegram-broadcast-0.2/setup.cfg
--rw-rw-r--   0 jonah     (1000) jonah     (1000)      869 2024-05-06 09:18:46.000000 python-telegram-broadcast-0.2/setup.py
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-06 10:47:16.132004 python-telegram-broadcast-0.4/
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     1067 2024-05-06 01:52:00.000000 python-telegram-broadcast-0.4/LICENSE
+-rw-r--r--   0 jonah     (1000) jonah     (1000)     1233 2024-05-06 10:47:16.132004 python-telegram-broadcast-0.4/PKG-INFO
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)      647 2024-05-06 10:34:26.000000 python-telegram-broadcast-0.4/README.md
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-06 10:47:16.132004 python-telegram-broadcast-0.4/python-telegram-broadcast/
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     2673 2024-05-06 08:59:24.000000 python-telegram-broadcast-0.4/python-telegram-broadcast/__init__.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     2963 2024-05-06 08:33:20.000000 python-telegram-broadcast-0.4/python-telegram-broadcast/custom_dataclass.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     1616 2024-05-06 08:35:01.000000 python-telegram-broadcast-0.4/python-telegram-broadcast/custom_exception.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     2236 2024-05-06 09:03:53.000000 python-telegram-broadcast-0.4/python-telegram-broadcast/custom_util.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     2417 2024-05-06 08:41:00.000000 python-telegram-broadcast-0.4/python-telegram-broadcast/main.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)    16983 2024-05-06 08:59:09.000000 python-telegram-broadcast-0.4/python-telegram-broadcast/send_method.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)    16160 2024-05-06 09:03:53.000000 python-telegram-broadcast-0.4/python-telegram-broadcast/strategy.py
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-06 10:47:16.132004 python-telegram-broadcast-0.4/python_telegram_broadcast.egg-info/
+-rw-r--r--   0 jonah     (1000) jonah     (1000)     1233 2024-05-06 10:47:16.000000 python-telegram-broadcast-0.4/python_telegram_broadcast.egg-info/PKG-INFO
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)      554 2024-05-06 10:47:16.000000 python-telegram-broadcast-0.4/python_telegram_broadcast.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)        1 2024-05-06 10:47:16.000000 python-telegram-broadcast-0.4/python_telegram_broadcast.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)       33 2024-05-06 10:47:16.000000 python-telegram-broadcast-0.4/python_telegram_broadcast.egg-info/requires.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)       26 2024-05-06 10:47:16.000000 python-telegram-broadcast-0.4/python_telegram_broadcast.egg-info/top_level.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)       38 2024-05-06 10:47:16.132004 python-telegram-broadcast-0.4/setup.cfg
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)      850 2024-05-06 10:45:25.000000 python-telegram-broadcast-0.4/setup.py
```

### Comparing `python-telegram-broadcast-0.2/LICENSE` & `python-telegram-broadcast-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-telegram-broadcast-0.2/python-telegram-broadcast/__init__.py` & `python-telegram-broadcast-0.4/python-telegram-broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `python-telegram-broadcast-0.2/python-telegram-broadcast/custom_dataclass.py` & `python-telegram-broadcast-0.4/python-telegram-broadcast/custom_dataclass.py`

 * *Files identical despite different names*

### Comparing `python-telegram-broadcast-0.2/python-telegram-broadcast/custom_exception.py` & `python-telegram-broadcast-0.4/python-telegram-broadcast/custom_exception.py`

 * *Files identical despite different names*

### Comparing `python-telegram-broadcast-0.2/python-telegram-broadcast/custom_util.py` & `python-telegram-broadcast-0.4/python-telegram-broadcast/custom_util.py`

 * *Files identical despite different names*

### Comparing `python-telegram-broadcast-0.2/python-telegram-broadcast/main.py` & `python-telegram-broadcast-0.4/python-telegram-broadcast/main.py`

 * *Files identical despite different names*

### Comparing `python-telegram-broadcast-0.2/python-telegram-broadcast/send_method.py` & `python-telegram-broadcast-0.4/python-telegram-broadcast/send_method.py`

 * *Files identical despite different names*

### Comparing `python-telegram-broadcast-0.2/python-telegram-broadcast/strategy.py` & `python-telegram-broadcast-0.4/python-telegram-broadcast/strategy.py`

 * *Files identical despite different names*

### Comparing `python-telegram-broadcast-0.2/python_telegram_broadcast.egg-info/SOURCES.txt` & `python-telegram-broadcast-0.4/python_telegram_broadcast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-telegram-broadcast-0.2/setup.py` & `python-telegram-broadcast-0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2'
 DESCRIPTION = 'Package that wraps the python-telegram-bot library to make broadcasting easier.'
 
 setup(
     name='python-telegram-broadcast',
-    version=VERSION,
+    version='0.4',
     packages=find_packages(),
     description=DESCRIPTION,
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='jonah_whaler_2348',
     author_email='jk_saga@proton.me',
     license='MIT',
```

