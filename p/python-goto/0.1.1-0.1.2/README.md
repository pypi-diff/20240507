# Comparing `tmp/python_goto-0.1.1.tar.gz` & `tmp/python_goto-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_goto-0.1.1.tar", last modified: Tue May  7 13:53:35 2024, max compression
+gzip compressed data, was "python_goto-0.1.2.tar", last modified: Tue May  7 13:58:58 2024, max compression
```

## Comparing `python_goto-0.1.1.tar` & `python_goto-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 13:53:35.348867 python_goto-0.1.1/
--rw-rw-rw-   0        0        0      940 2024-05-07 13:53:35.347867 python_goto-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      707 2024-05-07 13:53:26.000000 python_goto-0.1.1/README.md
--rw-rw-rw-   0        0        0     1087 2024-05-07 12:35:55.000000 python_goto-0.1.1/licence.txt
-drwxrwxrwx   0        0        0        0 2024-05-07 13:53:35.332868 python_goto-0.1.1/python_goto/
--rw-rw-rw-   0        0        0       28 2024-05-07 13:48:11.000000 python_goto-0.1.1/python_goto/__init__.py
--rw-rw-rw-   0        0        0      528 2024-05-07 12:35:55.000000 python_goto-0.1.1/python_goto/goto.py
-drwxrwxrwx   0        0        0        0 2024-05-07 13:53:35.346867 python_goto-0.1.1/python_goto.egg-info/
--rw-rw-rw-   0        0        0      940 2024-05-07 13:53:35.000000 python_goto-0.1.1/python_goto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2024-05-07 13:53:35.000000 python_goto-0.1.1/python_goto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 13:53:35.000000 python_goto-0.1.1/python_goto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-07 13:53:35.000000 python_goto-0.1.1/python_goto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 13:53:35.349866 python_goto-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      488 2024-05-07 13:52:58.000000 python_goto-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:58:58.147496 python_goto-0.1.2/
+-rw-rw-rw-   0        0        0      940 2024-05-07 13:58:58.144496 python_goto-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      707 2024-05-07 13:53:26.000000 python_goto-0.1.2/README.md
+-rw-rw-rw-   0        0        0     1087 2024-05-07 12:35:55.000000 python_goto-0.1.2/licence.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 13:58:58.129505 python_goto-0.1.2/python_goto/
+-rw-rw-rw-   0        0        0       33 2024-05-07 13:56:28.000000 python_goto-0.1.2/python_goto/__init__.py
+-rw-rw-rw-   0        0        0      528 2024-05-07 12:35:55.000000 python_goto-0.1.2/python_goto/goto.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:58:58.143522 python_goto-0.1.2/python_goto.egg-info/
+-rw-rw-rw-   0        0        0      940 2024-05-07 13:58:58.000000 python_goto-0.1.2/python_goto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2024-05-07 13:58:58.000000 python_goto-0.1.2/python_goto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 13:58:58.000000 python_goto-0.1.2/python_goto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-07 13:58:58.000000 python_goto-0.1.2/python_goto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 13:58:58.147496 python_goto-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      488 2024-05-07 13:58:51.000000 python_goto-0.1.2/setup.py
```

### Comparing `python_goto-0.1.1/PKG-INFO` & `python_goto-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-goto
-Version: 0.1.1
+Version: 0.1.2
 Summary: Add goto to Python
 Author: The Lumberjack
 Author-email: just4now@example.com
 Keywords: goto
 Description-Content-Type: text/markdown
 License-File: licence.txt
```

### Comparing `python_goto-0.1.1/README.md` & `python_goto-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `python_goto-0.1.1/licence.txt` & `python_goto-0.1.2/licence.txt`

 * *Files identical despite different names*

### Comparing `python_goto-0.1.1/python_goto/goto.py` & `python_goto-0.1.2/python_goto/goto.py`

 * *Files identical despite different names*

### Comparing `python_goto-0.1.1/python_goto.egg-info/PKG-INFO` & `python_goto-0.1.2/python_goto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-goto
-Version: 0.1.1
+Version: 0.1.2
 Summary: Add goto to Python
 Author: The Lumberjack
 Author-email: just4now@example.com
 Keywords: goto
 Description-Content-Type: text/markdown
 License-File: licence.txt
```

