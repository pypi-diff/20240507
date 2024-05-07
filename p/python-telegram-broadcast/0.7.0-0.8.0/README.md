# Comparing `tmp/python-telegram-broadcast-0.7.0.tar.gz` & `tmp/python_telegram_broadcast-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-telegram-broadcast-0.7.0.tar", last modified: Tue May  7 02:38:51 2024, max compression
+gzip compressed data, was "python_telegram_broadcast-0.8.0.tar", last modified: Tue May  7 02:49:03 2024, max compression
```

## Comparing `python-telegram-broadcast-0.7.0.tar` & `python_telegram_broadcast-0.8.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 02:38:51.667337 python-telegram-broadcast-0.7.0/
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     1067 2024-05-06 01:52:00.000000 python-telegram-broadcast-0.7.0/LICENSE
--rw-r--r--   0 jonah     (1000) jonah     (1000)     3920 2024-05-07 02:38:51.667337 python-telegram-broadcast-0.7.0/PKG-INFO
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     3331 2024-05-07 02:37:41.000000 python-telegram-broadcast-0.7.0/README.md
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 02:38:51.667337 python-telegram-broadcast-0.7.0/python-telegram-broadcast/
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     2919 2024-05-07 02:37:28.000000 python-telegram-broadcast-0.7.0/python-telegram-broadcast/__init__.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     2963 2024-05-06 08:33:20.000000 python-telegram-broadcast-0.7.0/python-telegram-broadcast/custom_dataclass.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     1616 2024-05-06 08:35:01.000000 python-telegram-broadcast-0.7.0/python-telegram-broadcast/custom_exception.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     2236 2024-05-06 09:03:53.000000 python-telegram-broadcast-0.7.0/python-telegram-broadcast/custom_util.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     2417 2024-05-06 08:41:00.000000 python-telegram-broadcast-0.7.0/python-telegram-broadcast/main.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)    16983 2024-05-06 08:59:09.000000 python-telegram-broadcast-0.7.0/python-telegram-broadcast/send_method.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)    16160 2024-05-06 09:03:53.000000 python-telegram-broadcast-0.7.0/python-telegram-broadcast/strategy.py
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 02:38:51.667337 python-telegram-broadcast-0.7.0/python_telegram_broadcast.egg-info/
--rw-r--r--   0 jonah     (1000) jonah     (1000)     3920 2024-05-07 02:38:51.000000 python-telegram-broadcast-0.7.0/python_telegram_broadcast.egg-info/PKG-INFO
--rw-rw-r--   0 jonah     (1000) jonah     (1000)      554 2024-05-07 02:38:51.000000 python-telegram-broadcast-0.7.0/python_telegram_broadcast.egg-info/SOURCES.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)        1 2024-05-07 02:38:51.000000 python-telegram-broadcast-0.7.0/python_telegram_broadcast.egg-info/dependency_links.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)       33 2024-05-07 02:38:51.000000 python-telegram-broadcast-0.7.0/python_telegram_broadcast.egg-info/requires.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)       26 2024-05-07 02:38:51.000000 python-telegram-broadcast-0.7.0/python_telegram_broadcast.egg-info/top_level.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)       38 2024-05-07 02:38:51.667337 python-telegram-broadcast-0.7.0/setup.cfg
--rw-rw-r--   0 jonah     (1000) jonah     (1000)      952 2024-05-07 02:38:34.000000 python-telegram-broadcast-0.7.0/setup.py
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 02:49:03.307685 python_telegram_broadcast-0.8.0/
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     1067 2024-05-06 01:52:00.000000 python_telegram_broadcast-0.8.0/LICENSE
+-rw-r--r--   0 jonah     (1000) jonah     (1000)     3920 2024-05-07 02:49:03.307685 python_telegram_broadcast-0.8.0/PKG-INFO
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     3331 2024-05-07 02:48:22.000000 python_telegram_broadcast-0.8.0/README.md
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 02:49:03.307685 python_telegram_broadcast-0.8.0/python_telegram_broadcast/
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     2919 2024-05-07 02:48:22.000000 python_telegram_broadcast-0.8.0/python_telegram_broadcast/__init__.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     2963 2024-05-06 08:33:20.000000 python_telegram_broadcast-0.8.0/python_telegram_broadcast/custom_dataclass.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     1616 2024-05-06 08:35:01.000000 python_telegram_broadcast-0.8.0/python_telegram_broadcast/custom_exception.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     2236 2024-05-06 09:03:53.000000 python_telegram_broadcast-0.8.0/python_telegram_broadcast/custom_util.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     2417 2024-05-06 08:41:00.000000 python_telegram_broadcast-0.8.0/python_telegram_broadcast/main.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)    16983 2024-05-06 08:59:09.000000 python_telegram_broadcast-0.8.0/python_telegram_broadcast/send_method.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)    16160 2024-05-06 09:03:53.000000 python_telegram_broadcast-0.8.0/python_telegram_broadcast/strategy.py
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 02:49:03.307685 python_telegram_broadcast-0.8.0/python_telegram_broadcast.egg-info/
+-rw-r--r--   0 jonah     (1000) jonah     (1000)     3920 2024-05-07 02:49:03.000000 python_telegram_broadcast-0.8.0/python_telegram_broadcast.egg-info/PKG-INFO
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)      554 2024-05-07 02:49:03.000000 python_telegram_broadcast-0.8.0/python_telegram_broadcast.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)        1 2024-05-07 02:49:03.000000 python_telegram_broadcast-0.8.0/python_telegram_broadcast.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)       33 2024-05-07 02:49:03.000000 python_telegram_broadcast-0.8.0/python_telegram_broadcast.egg-info/requires.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)       26 2024-05-07 02:49:03.000000 python_telegram_broadcast-0.8.0/python_telegram_broadcast.egg-info/top_level.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)       38 2024-05-07 02:49:03.307685 python_telegram_broadcast-0.8.0/setup.cfg
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)      952 2024-05-07 02:48:36.000000 python_telegram_broadcast-0.8.0/setup.py
```

### Comparing `python-telegram-broadcast-0.7.0/LICENSE` & `python_telegram_broadcast-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-telegram-broadcast-0.7.0/PKG-INFO` & `python_telegram_broadcast-0.8.0/python_telegram_broadcast.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-telegram-broadcast
-Version: 0.7.0
+Version: 0.8.0
 Summary: Package that wraps the python-telegram-bot library to make broadcasting easier.
 Author: jonah_whaler_2348
 Author-email: jk_saga@proton.me
 License: MIT
 Keywords: python,telegram,broadcast,bot
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -36,15 +36,15 @@
 
 ## Dependencies
 - [python-telegram-bot](https://pypi.org/project/python-telegram-bot/)=21.1.1
 - [mypy](https://pypi.org/project/mypy/)
 
 ## Installation
   ```bash
-  pip3 install python-telegram-broadcast
+  pip3 install python_telegram_broadcast
   ```
 
 ## Example
 
 ### Get File ID from Telegram
 ```python
 import asyncio
```

### Comparing `python-telegram-broadcast-0.7.0/README.md` & `python_telegram_broadcast-0.8.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 ## Dependencies
 - [python-telegram-bot](https://pypi.org/project/python-telegram-bot/)=21.1.1
 - [mypy](https://pypi.org/project/mypy/)
 
 ## Installation
   ```bash
-  pip3 install python-telegram-broadcast
+  pip3 install python_telegram_broadcast
   ```
 
 ## Example
 
 ### Get File ID from Telegram
 ```python
 import asyncio
```

### Comparing `python-telegram-broadcast-0.7.0/python-telegram-broadcast/__init__.py` & `python_telegram_broadcast-0.8.0/python_telegram_broadcast/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         handle_broadcast(
             slist, token, method, stg, payload, "...",
             use_multiproc=False, use_nproc=1, seconds=0.0, max_retry=5
         )
     )
 
 
-# CLI: python3 -m python-telegram-broadcast.__init__
+# CLI: python3 -m python_telegram_broadcast.__init__
 if __name__ == "__main__":
     bot_token: str = "TELEGRAM_BOT_TOKEN"   # << Change to your bot token
     user_telegram_id: int = 123456789       # << Change to your telegram id
     file_path: str = ""                     # << Change to your file path or the URL of your file
 
     broadcast_method = select_broadcast_method(BroadcastMethodType.PHOTO)
```

### Comparing `python-telegram-broadcast-0.7.0/python-telegram-broadcast/custom_dataclass.py` & `python_telegram_broadcast-0.8.0/python_telegram_broadcast/custom_dataclass.py`

 * *Files identical despite different names*

### Comparing `python-telegram-broadcast-0.7.0/python-telegram-broadcast/custom_exception.py` & `python_telegram_broadcast-0.8.0/python_telegram_broadcast/custom_exception.py`

 * *Files identical despite different names*

### Comparing `python-telegram-broadcast-0.7.0/python-telegram-broadcast/custom_util.py` & `python_telegram_broadcast-0.8.0/python_telegram_broadcast/custom_util.py`

 * *Files identical despite different names*

### Comparing `python-telegram-broadcast-0.7.0/python-telegram-broadcast/main.py` & `python_telegram_broadcast-0.8.0/python_telegram_broadcast/main.py`

 * *Files identical despite different names*

### Comparing `python-telegram-broadcast-0.7.0/python-telegram-broadcast/send_method.py` & `python_telegram_broadcast-0.8.0/python_telegram_broadcast/send_method.py`

 * *Files identical despite different names*

### Comparing `python-telegram-broadcast-0.7.0/python-telegram-broadcast/strategy.py` & `python_telegram_broadcast-0.8.0/python_telegram_broadcast/strategy.py`

 * *Files identical despite different names*

### Comparing `python-telegram-broadcast-0.7.0/python_telegram_broadcast.egg-info/PKG-INFO` & `python_telegram_broadcast-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: python-telegram-broadcast
-Version: 0.7.0
+Name: python_telegram_broadcast
+Version: 0.8.0
 Summary: Package that wraps the python-telegram-bot library to make broadcasting easier.
 Author: jonah_whaler_2348
 Author-email: jk_saga@proton.me
 License: MIT
 Keywords: python,telegram,broadcast,bot
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -36,15 +36,15 @@
 
 ## Dependencies
 - [python-telegram-bot](https://pypi.org/project/python-telegram-bot/)=21.1.1
 - [mypy](https://pypi.org/project/mypy/)
 
 ## Installation
   ```bash
-  pip3 install python-telegram-broadcast
+  pip3 install python_telegram_broadcast
   ```
 
 ## Example
 
 ### Get File ID from Telegram
 ```python
 import asyncio
```

### Comparing `python-telegram-broadcast-0.7.0/python_telegram_broadcast.egg-info/SOURCES.txt` & `python_telegram_broadcast-0.8.0/python_telegram_broadcast.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 LICENSE
 README.md
 setup.py
-python-telegram-broadcast/__init__.py
-python-telegram-broadcast/custom_dataclass.py
-python-telegram-broadcast/custom_exception.py
-python-telegram-broadcast/custom_util.py
-python-telegram-broadcast/main.py
-python-telegram-broadcast/send_method.py
-python-telegram-broadcast/strategy.py
+python_telegram_broadcast/__init__.py
+python_telegram_broadcast/custom_dataclass.py
+python_telegram_broadcast/custom_exception.py
+python_telegram_broadcast/custom_util.py
+python_telegram_broadcast/main.py
+python_telegram_broadcast/send_method.py
+python_telegram_broadcast/strategy.py
 python_telegram_broadcast.egg-info/PKG-INFO
 python_telegram_broadcast.egg-info/SOURCES.txt
 python_telegram_broadcast.egg-info/dependency_links.txt
 python_telegram_broadcast.egg-info/requires.txt
 python_telegram_broadcast.egg-info/top_level.txt
```

### Comparing `python-telegram-broadcast-0.7.0/setup.py` & `python_telegram_broadcast-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 DESCRIPTION = 'Package that wraps the python-telegram-bot library to make broadcasting easier.'
 
 # python3 setup.py sdist bdist_wheel
 # twine upload --skip-existing dist/*
 
-VERSION = '0.7.0'
+VERSION = '0.8.0'
 
 setup(
-    name='python-telegram-broadcast',
+    name='python_telegram_broadcast',
     version=VERSION,
     packages=find_packages(),
     description=DESCRIPTION,
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='jonah_whaler_2348',
     author_email='jk_saga@proton.me',
```

