# Comparing `tmp/filewatchdog-0.1.0.tar.gz` & `tmp/filewatchdog-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filewatchdog-0.1.0.tar", max compression
+gzip compressed data, was "filewatchdog-0.1.1.tar", max compression
```

## Comparing `filewatchdog-0.1.0.tar` & `filewatchdog-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1106 2024-01-26 03:37:30.564384 filewatchdog-0.1.0/LICENSE
--rw-r--r--   0        0        0     1043 2024-01-26 03:37:30.564384 filewatchdog-0.1.0/README.md
--rw-r--r--   0        0        0     4687 2024-01-26 03:59:06.314170 filewatchdog-0.1.0/filewatchdog/__init__.py
--rw-r--r--   0        0        0      483 2024-01-26 03:47:42.855338 filewatchdog-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1619 1970-01-01 00:00:00.000000 filewatchdog-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1106 2024-05-07 01:40:15.000000 filewatchdog-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1371 2024-05-07 01:40:15.000000 filewatchdog-0.1.1/README.md
+-rw-r--r--   0        0        0     5426 2024-05-07 01:40:15.000000 filewatchdog-0.1.1/filewatchdog/__init__.py
+-rw-r--r--   0        0        0      466 2024-05-07 02:38:28.208325 filewatchdog-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1947 1970-01-01 00:00:00.000000 filewatchdog-0.1.1/PKG-INFO
```

### Comparing `filewatchdog-0.1.0/LICENSE` & `filewatchdog-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `filewatchdog-0.1.0/README.md` & `filewatchdog-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -20,16 +20,32 @@
 ```py
 import filewatchdog as watcher
 import time
 
 def job():
     print("I'm working...")
 
+
+# detecting changes to one single file
+
+watcher.once().file('C:/Temp/1.txt').modified.do(job)
+watcher.once().file('C:/Temp/1.txt').exist.do(job)
+
+
+# detecting file changes in a directory recursively
+
+watcher.once().folder('C:/Temp').modified.do(job)
+watcher.once().folder('C:/Temp').exist.do(job)
+
+
+# watching multiple files
+
 files = ['C:/Temp/1.txt', 'C:/Temp/2.txt', 'C:/Temp/3.txt']
 
 watcher.once().one_of(files).modified.do(job)
 watcher.once().all_of(files).exist.do(job)
 
+
 while True:
     watcher.run_pending()
     time.sleep(1)
 ```
```

### Comparing `filewatchdog-0.1.0/filewatchdog/__init__.py` & `filewatchdog-0.1.1/filewatchdog/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import schedule
 import functools, datetime, logging, pathlib
 from time import sleep
 from typing import List, Optional, Callable
+import os
 
 logger = logging.getLogger("watcher")
 
 
 class WatcherError(Exception):
     """Base watcher exception"""
     
@@ -51,14 +52,34 @@
         self.event = 'modified'
         return self
     
     @property
     def exist(self):
         self.event = 'exist'
         return self
+    
+    def file(self,file_path:str):
+        if os.path.isfile(file_path):
+            self.num_of = 'one_of'
+            self.files = [file_path]
+            self.mtime_last_check.update({file_path:self._get_mtime(file_path)})
+        else:
+            raise ValueError(f"Path {file_path} is not a file")
+        return self
+    
+    def folder(self,folder_path:str):
+        files = []
+        if os.path.isdir(folder_path):
+            for root,dir,filenames in os.walk(folder_path):
+                for file in filenames:
+                    files.append(os.path.join(root,file))
+            self.one_of(files)
+        else:
+            raise ValueError(f"Folder path {folder_path} is not a directory")
+        return self
             
     def one_of(self, files: List[str]): 
         self.num_of = 'one_of'
         self.files = files
         for file in self.files:
             if pathlib.Path(file).exists():
                 self.mtime_last_check.update({file: self._get_mtime(file)})
```

### Comparing `filewatchdog-0.1.0/PKG-INFO` & `filewatchdog-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filewatchdog
-Version: 0.1.0
+Version: 0.1.1
 Summary: Runs Python functions once a certain file is created or modified.
 License: MIT
 Author: BeginnerSC
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -36,17 +36,33 @@
 ```py
 import filewatchdog as watcher
 import time
 
 def job():
     print("I'm working...")
 
+
+# detecting changes to one single file
+
+watcher.once().file('C:/Temp/1.txt').modified.do(job)
+watcher.once().file('C:/Temp/1.txt').exist.do(job)
+
+
+# detecting file changes in a directory recursively
+
+watcher.once().folder('C:/Temp').modified.do(job)
+watcher.once().folder('C:/Temp').exist.do(job)
+
+
+# watching multiple files
+
 files = ['C:/Temp/1.txt', 'C:/Temp/2.txt', 'C:/Temp/3.txt']
 
 watcher.once().one_of(files).modified.do(job)
 watcher.once().all_of(files).exist.do(job)
 
+
 while True:
     watcher.run_pending()
     time.sleep(1)
 ```
```

