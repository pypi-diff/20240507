# Comparing `tmp/orange3_sqlite3-0.0.2.tar.gz` & `tmp/orange3_sqlite3-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orange3_sqlite3-0.0.2.tar", last modified: Tue May  7 19:31:05 2024, max compression
+gzip compressed data, was "orange3_sqlite3-0.0.3.tar", last modified: Tue May  7 19:34:06 2024, max compression
```

## Comparing `orange3_sqlite3-0.0.2.tar` & `orange3_sqlite3-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-07 19:31:05.072034 orange3_sqlite3-0.0.2/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-07 19:31:05.072034 orange3_sqlite3-0.0.2/Orange3_Sqlite3.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)     1058 2024-05-07 19:31:05.000000 orange3_sqlite3-0.0.2/Orange3_Sqlite3.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      495 2024-05-07 19:31:05.000000 orange3_sqlite3-0.0.2/Orange3_Sqlite3.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2024-05-07 19:31:05.000000 orange3_sqlite3-0.0.2/Orange3_Sqlite3.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      196 2024-05-07 19:31:05.000000 orange3_sqlite3-0.0.2/Orange3_Sqlite3.egg-info/entry_points.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       14 2024-05-07 19:31:05.000000 orange3_sqlite3-0.0.2/Orange3_Sqlite3.egg-info/namespace_packages.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      149 2024-05-07 19:31:05.000000 orange3_sqlite3-0.0.2/Orange3_Sqlite3.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       14 2024-05-07 19:31:05.000000 orange3_sqlite3-0.0.2/Orange3_Sqlite3.egg-info/top_level.txt
--rw-r--r--   0 chris     (1000) chris     (1000)     1058 2024-05-07 19:31:05.072034 orange3_sqlite3-0.0.2/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      136 2024-05-07 02:14:41.000000 orange3_sqlite3-0.0.2/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-07 19:31:05.068034 orange3_sqlite3-0.0.2/orangecontrib/
--rw-rw-r--   0 chris     (1000) chris     (1000)       79 2024-05-07 02:15:14.000000 orange3_sqlite3-0.0.2/orangecontrib/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-07 19:31:05.068034 orange3_sqlite3-0.0.2/orangecontrib/sqlite3/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2024-05-07 02:15:34.000000 orange3_sqlite3-0.0.2/orangecontrib/sqlite3/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-07 19:31:05.068034 orange3_sqlite3-0.0.2/orangecontrib/sqlite3/widgets/
--rw-rw-r--   0 chris     (1000) chris     (1000)      938 2024-05-07 02:16:44.000000 orange3_sqlite3-0.0.2/orangecontrib/sqlite3/widgets/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-07 19:31:05.068034 orange3_sqlite3-0.0.2/orangecontrib/sqlite3/widgets/icons/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1822 2024-05-07 02:19:04.000000 orange3_sqlite3-0.0.2/orangecontrib/sqlite3/widgets/icons/sqlite3.svg
--rw-rw-r--   0 chris     (1000) chris     (1000)     6338 2024-05-07 19:16:25.000000 orange3_sqlite3-0.0.2/orangecontrib/sqlite3/widgets/owsqlite3.py
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2024-05-07 19:31:05.072034 orange3_sqlite3-0.0.2/setup.cfg
--rw-rw-r--   0 chris     (1000) chris     (1000)     2791 2024-05-07 19:31:00.000000 orange3_sqlite3-0.0.2/setup.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-07 19:34:06.656040 orange3_sqlite3-0.0.3/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-07 19:34:06.656040 orange3_sqlite3-0.0.3/Orange3_Sqlite3.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)     1058 2024-05-07 19:34:06.000000 orange3_sqlite3-0.0.3/Orange3_Sqlite3.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      495 2024-05-07 19:34:06.000000 orange3_sqlite3-0.0.3/Orange3_Sqlite3.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2024-05-07 19:34:06.000000 orange3_sqlite3-0.0.3/Orange3_Sqlite3.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      196 2024-05-07 19:34:06.000000 orange3_sqlite3-0.0.3/Orange3_Sqlite3.egg-info/entry_points.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       14 2024-05-07 19:34:06.000000 orange3_sqlite3-0.0.3/Orange3_Sqlite3.egg-info/namespace_packages.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      149 2024-05-07 19:34:06.000000 orange3_sqlite3-0.0.3/Orange3_Sqlite3.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       14 2024-05-07 19:34:06.000000 orange3_sqlite3-0.0.3/Orange3_Sqlite3.egg-info/top_level.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)     1058 2024-05-07 19:34:06.656040 orange3_sqlite3-0.0.3/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      136 2024-05-07 02:14:41.000000 orange3_sqlite3-0.0.3/README.md
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-07 19:34:06.652040 orange3_sqlite3-0.0.3/orangecontrib/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       79 2024-05-07 02:15:14.000000 orange3_sqlite3-0.0.3/orangecontrib/__init__.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-07 19:34:06.652040 orange3_sqlite3-0.0.3/orangecontrib/sqlite3/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2024-05-07 02:15:34.000000 orange3_sqlite3-0.0.3/orangecontrib/sqlite3/__init__.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-07 19:34:06.652040 orange3_sqlite3-0.0.3/orangecontrib/sqlite3/widgets/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      938 2024-05-07 02:16:44.000000 orange3_sqlite3-0.0.3/orangecontrib/sqlite3/widgets/__init__.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-07 19:34:06.652040 orange3_sqlite3-0.0.3/orangecontrib/sqlite3/widgets/icons/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1822 2024-05-07 02:19:04.000000 orange3_sqlite3-0.0.3/orangecontrib/sqlite3/widgets/icons/sqlite3.svg
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6369 2024-05-07 19:33:42.000000 orange3_sqlite3-0.0.3/orangecontrib/sqlite3/widgets/owsqlite3.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2024-05-07 19:34:06.656040 orange3_sqlite3-0.0.3/setup.cfg
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2791 2024-05-07 19:33:59.000000 orange3_sqlite3-0.0.3/setup.py
```

### Comparing `orange3_sqlite3-0.0.2/Orange3_Sqlite3.egg-info/PKG-INFO` & `orange3_sqlite3-0.0.3/Orange3_Sqlite3.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Orange3-Sqlite3
-Version: 0.0.2
+Version: 0.0.3
 Summary:  
 Home-page: https://github.com/chrislee35/orange3-sqlite3
 Author: Chris Lee
 Author-email: github@chrislee.dhs.org
 License: GPL3+
 Keywords: orange3 add-on
 Classifier: Development Status :: 1 - Planning
```

### Comparing `orange3_sqlite3-0.0.2/PKG-INFO` & `orange3_sqlite3-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Orange3-Sqlite3
-Version: 0.0.2
+Version: 0.0.3
 Summary:  
 Home-page: https://github.com/chrislee35/orange3-sqlite3
 Author: Chris Lee
 Author-email: github@chrislee.dhs.org
 License: GPL3+
 Keywords: orange3 add-on
 Classifier: Development Status :: 1 - Planning
```

### Comparing `orange3_sqlite3-0.0.2/orangecontrib/sqlite3/widgets/__init__.py` & `orange3_sqlite3-0.0.3/orangecontrib/sqlite3/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `orange3_sqlite3-0.0.2/orangecontrib/sqlite3/widgets/icons/sqlite3.svg` & `orange3_sqlite3-0.0.3/orangecontrib/sqlite3/widgets/icons/sqlite3.svg`

 * *Files identical despite different names*

### Comparing `orange3_sqlite3-0.0.2/orangecontrib/sqlite3/widgets/owsqlite3.py` & `orange3_sqlite3-0.0.3/orangecontrib/sqlite3/widgets/owsqlite3.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     sqlhist = settings.ContextSetting([])
     
     want_control_area = False
     
     def __init__(self):
         super().__init__()
         self.file_index = 0
+        self.result_set = None
         
         self.populate_controlArea()
         self.populate_mainArea()
         
         self.populate_comboboxes()
         self.reload()
```

### Comparing `orange3_sqlite3-0.0.2/setup.py` & `orange3_sqlite3-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open('README.md', 'r', encoding='utf-8') as f:
     ABOUT = f.read()
 
 NAME = 'Orange3-Sqlite3'
 
 MAJOR = 0
 MINOR = 0
-MICRO = 2
+MICRO = 3
 VERSION = '%d.%d.%d' % (MAJOR, MINOR, MICRO)
 
 AUTHOR = 'Chris Lee'
 AUTHOR_EMAIL = 'github@chrislee.dhs.org'
 
 URL = 'https://github.com/chrislee35/orange3-sqlite3'
 DESCRIPTION = ' '
```

