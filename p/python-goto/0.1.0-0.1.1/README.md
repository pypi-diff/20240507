# Comparing `tmp/python_goto-0.1.0.tar.gz` & `tmp/python_goto-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_goto-0.1.0.tar", last modified: Tue May  7 13:48:56 2024, max compression
+gzip compressed data, was "python_goto-0.1.1.tar", last modified: Tue May  7 13:53:35 2024, max compression
```

## Comparing `python_goto-0.1.0.tar` & `python_goto-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 13:48:56.069599 python_goto-0.1.0/
--rw-rw-rw-   0        0        0      928 2024-05-07 13:48:56.068600 python_goto-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      695 2024-05-07 13:39:40.000000 python_goto-0.1.0/README.md
--rw-rw-rw-   0        0        0     1087 2024-05-07 12:35:55.000000 python_goto-0.1.0/licence.txt
-drwxrwxrwx   0        0        0        0 2024-05-07 13:48:56.046599 python_goto-0.1.0/python_goto/
--rw-rw-rw-   0        0        0       28 2024-05-07 13:48:11.000000 python_goto-0.1.0/python_goto/__init__.py
--rw-rw-rw-   0        0        0      528 2024-05-07 12:35:55.000000 python_goto-0.1.0/python_goto/goto.py
-drwxrwxrwx   0        0        0        0 2024-05-07 13:48:56.067600 python_goto-0.1.0/python_goto.egg-info/
--rw-rw-rw-   0        0        0      928 2024-05-07 13:48:55.000000 python_goto-0.1.0/python_goto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2024-05-07 13:48:55.000000 python_goto-0.1.0/python_goto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 13:48:55.000000 python_goto-0.1.0/python_goto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-07 13:48:55.000000 python_goto-0.1.0/python_goto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 13:48:56.069599 python_goto-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      488 2024-05-07 13:48:52.000000 python_goto-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:53:35.348867 python_goto-0.1.1/
+-rw-rw-rw-   0        0        0      940 2024-05-07 13:53:35.347867 python_goto-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      707 2024-05-07 13:53:26.000000 python_goto-0.1.1/README.md
+-rw-rw-rw-   0        0        0     1087 2024-05-07 12:35:55.000000 python_goto-0.1.1/licence.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 13:53:35.332868 python_goto-0.1.1/python_goto/
+-rw-rw-rw-   0        0        0       28 2024-05-07 13:48:11.000000 python_goto-0.1.1/python_goto/__init__.py
+-rw-rw-rw-   0        0        0      528 2024-05-07 12:35:55.000000 python_goto-0.1.1/python_goto/goto.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:53:35.346867 python_goto-0.1.1/python_goto.egg-info/
+-rw-rw-rw-   0        0        0      940 2024-05-07 13:53:35.000000 python_goto-0.1.1/python_goto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2024-05-07 13:53:35.000000 python_goto-0.1.1/python_goto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 13:53:35.000000 python_goto-0.1.1/python_goto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-07 13:53:35.000000 python_goto-0.1.1/python_goto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 13:53:35.349866 python_goto-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      488 2024-05-07 13:52:58.000000 python_goto-0.1.1/setup.py
```

### Comparing `python_goto-0.1.0/PKG-INFO` & `python_goto-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-goto
-Version: 0.1.0
+Version: 0.1.1
 Summary: Add goto to Python
 Author: The Lumberjack
 Author-email: just4now@example.com
 Keywords: goto
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
@@ -12,21 +12,21 @@
 
 This package adds a revolutionary feature to Python: the Goto statement<br>
 It allows you to feel the essence of early days of C while using a modern language
 
 ## Installation
 
 ```
-pip install addgoto
+pip install python-goto
 ```
 
 ## How to use
 
 ```python
-from addgoto import goto
+from python_goto import goto
 
 x: int = 0
 while x < 10:
     x += 1
     print(x)
     goto(line=4)
 ```
@@ -34,15 +34,15 @@
 ## Limitations
 
 The line you want to jump to must have no indent blocks
 
 For example, the following code won't work
 
 ```python
-from addgoto import goto
+from python_goto import goto
 
 def count_down(n: int) -> None:
     while n > 0:
         n -= 1
         print(n)
         goto(line=4)
 ```
```

### Comparing `python_goto-0.1.0/README.md` & `python_goto-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 This package adds a revolutionary feature to Python: the Goto statement<br>
 It allows you to feel the essence of early days of C while using a modern language
 
 ## Installation
 
 ```
-pip install addgoto
+pip install python-goto
 ```
 
 ## How to use
 
 ```python
-from addgoto import goto
+from python_goto import goto
 
 x: int = 0
 while x < 10:
     x += 1
     print(x)
     goto(line=4)
 ```
@@ -24,15 +24,15 @@
 ## Limitations
 
 The line you want to jump to must have no indent blocks
 
 For example, the following code won't work
 
 ```python
-from addgoto import goto
+from python_goto import goto
 
 def count_down(n: int) -> None:
     while n > 0:
         n -= 1
         print(n)
         goto(line=4)
 ```
```

### Comparing `python_goto-0.1.0/licence.txt` & `python_goto-0.1.1/licence.txt`

 * *Files identical despite different names*

### Comparing `python_goto-0.1.0/python_goto/goto.py` & `python_goto-0.1.1/python_goto/goto.py`

 * *Files identical despite different names*

### Comparing `python_goto-0.1.0/python_goto.egg-info/PKG-INFO` & `python_goto-0.1.1/python_goto.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-goto
-Version: 0.1.0
+Version: 0.1.1
 Summary: Add goto to Python
 Author: The Lumberjack
 Author-email: just4now@example.com
 Keywords: goto
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
@@ -12,21 +12,21 @@
 
 This package adds a revolutionary feature to Python: the Goto statement<br>
 It allows you to feel the essence of early days of C while using a modern language
 
 ## Installation
 
 ```
-pip install addgoto
+pip install python-goto
 ```
 
 ## How to use
 
 ```python
-from addgoto import goto
+from python_goto import goto
 
 x: int = 0
 while x < 10:
     x += 1
     print(x)
     goto(line=4)
 ```
@@ -34,15 +34,15 @@
 ## Limitations
 
 The line you want to jump to must have no indent blocks
 
 For example, the following code won't work
 
 ```python
-from addgoto import goto
+from python_goto import goto
 
 def count_down(n: int) -> None:
     while n > 0:
         n -= 1
         print(n)
         goto(line=4)
 ```
```

