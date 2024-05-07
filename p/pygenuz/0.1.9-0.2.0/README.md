# Comparing `tmp/pygenuz-0.1.9.tar.gz` & `tmp/pygenuz-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygenuz-0.1.9.tar", last modified: Tue May  7 17:40:26 2024, max compression
+gzip compressed data, was "pygenuz-0.2.0.tar", last modified: Tue May  7 17:43:01 2024, max compression
```

## Comparing `pygenuz-0.1.9.tar` & `pygenuz-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:40:26.872564 pygenuz-0.1.9/
--rw-r--r--   0 khezozbek   (501) staff       (20)    13702 2024-05-07 17:40:26.871370 pygenuz-0.1.9/PKG-INFO
--rw-r--r--   0 khezozbek   (501) staff       (20)    13071 2024-05-07 17:39:54.000000 pygenuz-0.1.9/README.md
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:40:26.870001 pygenuz-0.1.9/pygenuz/
--rw-r--r--   0 khezozbek   (501) staff       (20)        0 2024-05-07 07:34:41.000000 pygenuz-0.1.9/pygenuz/__init__.py
--rw-r--r--   0 khezozbek   (501) staff       (20)     3787 2024-05-07 15:58:04.000000 pygenuz-0.1.9/pygenuz/app.py
--rw-r--r--   0 khezozbek   (501) staff       (20)       86 2024-05-07 16:18:44.000000 pygenuz-0.1.9/pygenuz/configs.py
--rw-r--r--   0 khezozbek   (501) staff       (20)      201 2024-05-07 16:08:54.000000 pygenuz-0.1.9/pygenuz/db.py
--rw-r--r--   0 khezozbek   (501) staff       (20)      680 2024-05-06 07:56:45.000000 pygenuz-0.1.9/pygenuz/middelware.py
--rw-r--r--   0 khezozbek   (501) staff       (20)      953 2024-05-06 09:07:08.000000 pygenuz-0.1.9/pygenuz/response.py
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:40:26.871021 pygenuz-0.1.9/pygenuz.egg-info/
--rw-r--r--   0 khezozbek   (501) staff       (20)    13702 2024-05-07 17:40:26.000000 pygenuz-0.1.9/pygenuz.egg-info/PKG-INFO
--rw-r--r--   0 khezozbek   (501) staff       (20)      282 2024-05-07 17:40:26.000000 pygenuz-0.1.9/pygenuz.egg-info/SOURCES.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)        1 2024-05-07 17:40:26.000000 pygenuz-0.1.9/pygenuz.egg-info/dependency_links.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)      116 2024-05-07 17:40:26.000000 pygenuz-0.1.9/pygenuz.egg-info/requires.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)        8 2024-05-07 17:40:26.000000 pygenuz-0.1.9/pygenuz.egg-info/top_level.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)       38 2024-05-07 17:40:26.872706 pygenuz-0.1.9/setup.cfg
--rw-r--r--   0 khezozbek   (501) staff       (20)     3912 2024-05-07 17:40:20.000000 pygenuz-0.1.9/setup.py
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:43:01.899109 pygenuz-0.2.0/
+-rw-r--r--   0 khezozbek   (501) staff       (20)    13637 2024-05-07 17:43:01.898804 pygenuz-0.2.0/PKG-INFO
+-rw-r--r--   0 khezozbek   (501) staff       (20)    13006 2024-05-07 17:42:47.000000 pygenuz-0.2.0/README.md
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:43:01.897479 pygenuz-0.2.0/pygenuz/
+-rw-r--r--   0 khezozbek   (501) staff       (20)        0 2024-05-07 07:34:41.000000 pygenuz-0.2.0/pygenuz/__init__.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)     3787 2024-05-07 15:58:04.000000 pygenuz-0.2.0/pygenuz/app.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)       86 2024-05-07 16:18:44.000000 pygenuz-0.2.0/pygenuz/configs.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)      201 2024-05-07 16:08:54.000000 pygenuz-0.2.0/pygenuz/db.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)      680 2024-05-06 07:56:45.000000 pygenuz-0.2.0/pygenuz/middelware.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)      953 2024-05-06 09:07:08.000000 pygenuz-0.2.0/pygenuz/response.py
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:43:01.898548 pygenuz-0.2.0/pygenuz.egg-info/
+-rw-r--r--   0 khezozbek   (501) staff       (20)    13637 2024-05-07 17:43:01.000000 pygenuz-0.2.0/pygenuz.egg-info/PKG-INFO
+-rw-r--r--   0 khezozbek   (501) staff       (20)      282 2024-05-07 17:43:01.000000 pygenuz-0.2.0/pygenuz.egg-info/SOURCES.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)        1 2024-05-07 17:43:01.000000 pygenuz-0.2.0/pygenuz.egg-info/dependency_links.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)      116 2024-05-07 17:43:01.000000 pygenuz-0.2.0/pygenuz.egg-info/requires.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)        8 2024-05-07 17:43:01.000000 pygenuz-0.2.0/pygenuz.egg-info/top_level.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)       38 2024-05-07 17:43:01.899179 pygenuz-0.2.0/setup.cfg
+-rw-r--r--   0 khezozbek   (501) staff       (20)     3912 2024-05-07 17:42:56.000000 pygenuz-0.2.0/setup.py
```

### Comparing `pygenuz-0.1.9/PKG-INFO` & `pygenuz-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygenuz
-Version: 0.1.9
+Version: 0.2.0
 Summary: My first Python web framework.
 Home-page: https://github.com/me/myproject
 Author: E'zozbek Kholbutayev
 Author-email: cssezozbel@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -76,15 +76,14 @@
             "home.html",
             context = {"new_title": "New title", "new_body": "New body"}
         )
 
 ```
 
 ## How we can use json? 
-![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json)
 
 ```
     @app.route("/json")
     def json_handler(req, resp):
         response_data = {"name": "some name"}
         resp.json = response_data
```

### Comparing `pygenuz-0.1.9/README.md` & `pygenuz-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,14 @@
             "home.html",
             context = {"new_title": "New title", "new_body": "New body"}
         )
 
 ```
 
 ## How we can use json? 
-![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json)
 
 ```
     @app.route("/json")
     def json_handler(req, resp):
         response_data = {"name": "some name"}
         resp.json = response_data
```

### Comparing `pygenuz-0.1.9/pygenuz/app.py` & `pygenuz-0.2.0/pygenuz/app.py`

 * *Files identical despite different names*

### Comparing `pygenuz-0.1.9/pygenuz/middelware.py` & `pygenuz-0.2.0/pygenuz/middelware.py`

 * *Files identical despite different names*

### Comparing `pygenuz-0.1.9/pygenuz/response.py` & `pygenuz-0.2.0/pygenuz/response.py`

 * *Files identical despite different names*

### Comparing `pygenuz-0.1.9/pygenuz.egg-info/PKG-INFO` & `pygenuz-0.2.0/pygenuz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygenuz
-Version: 0.1.9
+Version: 0.2.0
 Summary: My first Python web framework.
 Home-page: https://github.com/me/myproject
 Author: E'zozbek Kholbutayev
 Author-email: cssezozbel@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -76,15 +76,14 @@
             "home.html",
             context = {"new_title": "New title", "new_body": "New body"}
         )
 
 ```
 
 ## How we can use json? 
-![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json)
 
 ```
     @app.route("/json")
     def json_handler(req, resp):
         response_data = {"name": "some name"}
         resp.json = response_data
```

### Comparing `pygenuz-0.1.9/setup.py` & `pygenuz-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'pygenuz'
 DESCRIPTION = 'My first Python web framework.'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'cssezozbel@gmail.com'
 AUTHOR = "E'zozbek Kholbutayev"
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.1.9'
+VERSION = '0.2.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.4",
     "parse==1.20.1",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
```

