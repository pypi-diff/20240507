# Comparing `tmp/iaklogger-1.0.4.tar.gz` & `tmp/iaklogger-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iaklogger-1.0.4.tar", last modified: Fri Mar  8 08:47:34 2024, max compression
+gzip compressed data, was "iaklogger-1.0.5.tar", last modified: Tue May  7 18:44:04 2024, max compression
```

## Comparing `iaklogger-1.0.4.tar` & `iaklogger-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:47:34.191269 iaklogger-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-08 08:47:34.191269 iaklogger-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-03-08 08:47:30.000000 iaklogger-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:47:34.191269 iaklogger-1.0.4/iaklogger/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-08 08:47:30.000000 iaklogger-1.0.4/iaklogger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-03-08 08:47:30.000000 iaklogger-1.0.4/iaklogger/iaklogger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:47:34.191269 iaklogger-1.0.4/iaklogger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-08 08:47:34.000000 iaklogger-1.0.4/iaklogger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-08 08:47:34.000000 iaklogger-1.0.4/iaklogger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 08:47:34.000000 iaklogger-1.0.4/iaklogger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-08 08:47:34.000000 iaklogger-1.0.4/iaklogger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-08 08:47:34.191269 iaklogger-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-03-08 08:47:30.000000 iaklogger-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:44:04.543305 iaklogger-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-07 18:44:04.543305 iaklogger-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-05-07 18:44:00.000000 iaklogger-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:44:04.543305 iaklogger-1.0.5/iaklogger/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 18:44:00.000000 iaklogger-1.0.5/iaklogger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-07 18:44:00.000000 iaklogger-1.0.5/iaklogger/iaklogger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-07 18:44:00.000000 iaklogger-1.0.5/iaklogger/test_iaklogger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:44:04.543305 iaklogger-1.0.5/iaklogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-07 18:44:04.000000 iaklogger-1.0.5/iaklogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-07 18:44:04.000000 iaklogger-1.0.5/iaklogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 18:44:04.000000 iaklogger-1.0.5/iaklogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-07 18:44:04.000000 iaklogger-1.0.5/iaklogger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-07 18:44:04.543305 iaklogger-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-07 18:44:00.000000 iaklogger-1.0.5/setup.py
```

### Comparing `iaklogger-1.0.4/PKG-INFO` & `iaklogger-1.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iaklogger
-Version: 1.0.4
+Version: 1.0.5
 Summary: Very basic and easy logger
 Home-page: https://github.com/Iakl/iaklogger
 Download-URL: https://github.com/Iakl/iaklogger/archive/refs/tags/v1.0.0.tar.gz
 Author: Iakl
 Author-email: estebaniakl@gmail.com
 License: MIT
 Keywords: logger,easy,print,log,basic,logging
@@ -12,9 +12,10 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 
 Very basic and easy logger for python. It allows to print logs to the console and/or to a file. It also allows to mute logs by tags, mute all logs, show tags before the message, show time before the message, and set a maximum size for the log file.
```

### Comparing `iaklogger-1.0.4/README.md` & `iaklogger-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `iaklogger-1.0.4/iaklogger/iaklogger.py` & `iaklogger-1.0.5/iaklogger/iaklogger.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,41 +10,50 @@
     """str (Default: None): File path to save the log. If set, the log will be saved to this file."""
     log_file_max_size_mb = 1024 * 1024 * 10
     """int (Default: 10MB): Maximum size of the log file. If the file exceeds this size, it will be truncated."""
     mute_default = False
     """bool (Default: False): True to mute DEFAULT tag."""
     mute_all = False
     """bool (Default: False): True to mute all logs."""
+    newline_after_tag = False
+    """bool (Default: False): True to add a newline after tags."""
     show_tags = False
     """bool (Default: False): True to print tags before the message."""
     show_time = False
     """bool (Default: False): True to print time before the message."""
 
 
 def check_tags(list1, list2):
     return all(tag in list2 for tag in list1)
 
 
-def log(printable_obj, tags=[DEFAULT]):
+def log(printable_obj, tags=[DEFAULT], new_line=False):
     """
     Logs the message to the console and/or to a file.
     Args:
         printable_obj (str): Message to log.
         tags (list, optional): List of tags for this message. Default to [DEFAULT].
     Returns:
         bool: True if the message was logged, False otherwise.
     """
+    new_line_str = ""
+    tags_str = ""
+    time_str = ""
     if not check_tags(tags, OPTIONS.allowed_tags) and (not check_tags(tags, [DEFAULT]) or OPTIONS.mute_default):
         return False
     elif not OPTIONS.mute_all:
+        if OPTIONS.newline_after_tag or new_line:
+            new_line_str = "\n"
         if OPTIONS.show_tags:
-            printable_obj = f"[{'-'.join(tags)}] {printable_obj}"
+            tags_str = f"[{'-'.join(tags)}] "
+            # printable_obj = f"[{'-'.join(tags)}]{new_line}{printable_obj}"
         if OPTIONS.show_time:
-            printable_obj = f"{time.strftime('%Y-%m-%d %H:%M:%S')} {printable_obj}"
-        print(printable_obj)
+            time_str = f'{time.strftime("%Y-%m-%d %H:%M:%S")} '
+            # printable_obj = f"{time.strftime('%Y-%m-%d %H:%M:%S')} {printable_obj}"
+        print(f"{time_str}{tags_str}{new_line_str}{printable_obj}")
         if OPTIONS.log_file:
             log_to_file(printable_obj)
         return True
 
 
 def log_to_file(printable_obj):
     printable_obj_size = len(printable_obj.encode('utf-8'))
```

### Comparing `iaklogger-1.0.4/iaklogger.egg-info/PKG-INFO` & `iaklogger-1.0.5/iaklogger.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iaklogger
-Version: 1.0.4
+Version: 1.0.5
 Summary: Very basic and easy logger
 Home-page: https://github.com/Iakl/iaklogger
 Download-URL: https://github.com/Iakl/iaklogger/archive/refs/tags/v1.0.0.tar.gz
 Author: Iakl
 Author-email: estebaniakl@gmail.com
 License: MIT
 Keywords: logger,easy,print,log,basic,logging
@@ -12,9 +12,10 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 
 Very basic and easy logger for python. It allows to print logs to the console and/or to a file. It also allows to mute logs by tags, mute all logs, show tags before the message, show time before the message, and set a maximum size for the log file.
```

### Comparing `iaklogger-1.0.4/setup.py` & `iaklogger-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from distutils.core import setup
 setup(
     name='iaklogger',         # How you named your package folder (MyLib)
     packages=['iaklogger'],   # Chose the same as "name"
-    version='1.0.4',      # Start with a small number and increase it with every change you make
+    version='1.0.5',      # Start with a small number and increase it with every change you make
     # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     license='MIT',
     # Give a short description about your library
     description='Very basic and easy logger',
     long_description='Very basic and easy logger for python. It allows to print logs to the console and/or to a file. It also allows to mute logs by tags, mute all logs, show tags before the message, show time before the message, and set a maximum size for the log file.',
     author='Iakl',                   # Type in your name
     author_email='estebaniakl@gmail.com',      # Type in your E-Mail
@@ -26,9 +26,10 @@
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',   # Again, pick a license
         # Specify which pyhton versions that you want to support
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
     ],
 )
```

