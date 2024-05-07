# Comparing `tmp/pygenuz-0.1.8.tar.gz` & `tmp/pygenuz-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygenuz-0.1.8.tar", last modified: Tue May  7 17:39:25 2024, max compression
+gzip compressed data, was "pygenuz-0.1.9.tar", last modified: Tue May  7 17:40:26 2024, max compression
```

## Comparing `pygenuz-0.1.8.tar` & `pygenuz-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:39:25.696710 pygenuz-0.1.8/
--rw-r--r--   0 khezozbek   (501) staff       (20)    13745 2024-05-07 17:39:25.696531 pygenuz-0.1.8/PKG-INFO
--rw-r--r--   0 khezozbek   (501) staff       (20)    13114 2024-05-07 17:39:11.000000 pygenuz-0.1.8/README.md
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:39:25.694650 pygenuz-0.1.8/pygenuz/
--rw-r--r--   0 khezozbek   (501) staff       (20)        0 2024-05-07 07:34:41.000000 pygenuz-0.1.8/pygenuz/__init__.py
--rw-r--r--   0 khezozbek   (501) staff       (20)     3787 2024-05-07 15:58:04.000000 pygenuz-0.1.8/pygenuz/app.py
--rw-r--r--   0 khezozbek   (501) staff       (20)       86 2024-05-07 16:18:44.000000 pygenuz-0.1.8/pygenuz/configs.py
--rw-r--r--   0 khezozbek   (501) staff       (20)      201 2024-05-07 16:08:54.000000 pygenuz-0.1.8/pygenuz/db.py
--rw-r--r--   0 khezozbek   (501) staff       (20)      680 2024-05-06 07:56:45.000000 pygenuz-0.1.8/pygenuz/middelware.py
--rw-r--r--   0 khezozbek   (501) staff       (20)      953 2024-05-06 09:07:08.000000 pygenuz-0.1.8/pygenuz/response.py
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:39:25.695992 pygenuz-0.1.8/pygenuz.egg-info/
--rw-r--r--   0 khezozbek   (501) staff       (20)    13745 2024-05-07 17:39:25.000000 pygenuz-0.1.8/pygenuz.egg-info/PKG-INFO
--rw-r--r--   0 khezozbek   (501) staff       (20)      282 2024-05-07 17:39:25.000000 pygenuz-0.1.8/pygenuz.egg-info/SOURCES.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)        1 2024-05-07 17:39:25.000000 pygenuz-0.1.8/pygenuz.egg-info/dependency_links.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)      116 2024-05-07 17:39:25.000000 pygenuz-0.1.8/pygenuz.egg-info/requires.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)        8 2024-05-07 17:39:25.000000 pygenuz-0.1.8/pygenuz.egg-info/top_level.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)       38 2024-05-07 17:39:25.696814 pygenuz-0.1.8/setup.cfg
--rw-r--r--   0 khezozbek   (501) staff       (20)     3912 2024-05-07 17:39:22.000000 pygenuz-0.1.8/setup.py
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:40:26.872564 pygenuz-0.1.9/
+-rw-r--r--   0 khezozbek   (501) staff       (20)    13702 2024-05-07 17:40:26.871370 pygenuz-0.1.9/PKG-INFO
+-rw-r--r--   0 khezozbek   (501) staff       (20)    13071 2024-05-07 17:39:54.000000 pygenuz-0.1.9/README.md
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:40:26.870001 pygenuz-0.1.9/pygenuz/
+-rw-r--r--   0 khezozbek   (501) staff       (20)        0 2024-05-07 07:34:41.000000 pygenuz-0.1.9/pygenuz/__init__.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)     3787 2024-05-07 15:58:04.000000 pygenuz-0.1.9/pygenuz/app.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)       86 2024-05-07 16:18:44.000000 pygenuz-0.1.9/pygenuz/configs.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)      201 2024-05-07 16:08:54.000000 pygenuz-0.1.9/pygenuz/db.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)      680 2024-05-06 07:56:45.000000 pygenuz-0.1.9/pygenuz/middelware.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)      953 2024-05-06 09:07:08.000000 pygenuz-0.1.9/pygenuz/response.py
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:40:26.871021 pygenuz-0.1.9/pygenuz.egg-info/
+-rw-r--r--   0 khezozbek   (501) staff       (20)    13702 2024-05-07 17:40:26.000000 pygenuz-0.1.9/pygenuz.egg-info/PKG-INFO
+-rw-r--r--   0 khezozbek   (501) staff       (20)      282 2024-05-07 17:40:26.000000 pygenuz-0.1.9/pygenuz.egg-info/SOURCES.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)        1 2024-05-07 17:40:26.000000 pygenuz-0.1.9/pygenuz.egg-info/dependency_links.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)      116 2024-05-07 17:40:26.000000 pygenuz-0.1.9/pygenuz.egg-info/requires.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)        8 2024-05-07 17:40:26.000000 pygenuz-0.1.9/pygenuz.egg-info/top_level.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)       38 2024-05-07 17:40:26.872706 pygenuz-0.1.9/setup.cfg
+-rw-r--r--   0 khezozbek   (501) staff       (20)     3912 2024-05-07 17:40:20.000000 pygenuz-0.1.9/setup.py
```

### Comparing `pygenuz-0.1.8/PKG-INFO` & `pygenuz-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygenuz
-Version: 0.1.8
+Version: 0.1.9
 Summary: My first Python web framework.
 Home-page: https://github.com/me/myproject
 Author: E'zozbek Kholbutayev
 Author-email: cssezozbel@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -409,15 +409,14 @@
             "author": book.author,
             "published_date": str(book.published_date)
         }
         for book in books
     ]
     response.json = books_data
 ```
-![json](https://img.shields.io/badge/json)
 ##### POST json data 
 ```
 @app.route("/api/book", allowed_methods=["post"])
 def create_book(request, response):
     session = configure_database()
     book_data = request.json
     new_book = Book(
```

### Comparing `pygenuz-0.1.8/README.md` & `pygenuz-0.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -390,15 +390,14 @@
             "author": book.author,
             "published_date": str(book.published_date)
         }
         for book in books
     ]
     response.json = books_data
 ```
-![json](https://img.shields.io/badge/json)
 ##### POST json data 
 ```
 @app.route("/api/book", allowed_methods=["post"])
 def create_book(request, response):
     session = configure_database()
     book_data = request.json
     new_book = Book(
```

### Comparing `pygenuz-0.1.8/pygenuz/app.py` & `pygenuz-0.1.9/pygenuz/app.py`

 * *Files identical despite different names*

### Comparing `pygenuz-0.1.8/pygenuz/middelware.py` & `pygenuz-0.1.9/pygenuz/middelware.py`

 * *Files identical despite different names*

### Comparing `pygenuz-0.1.8/pygenuz/response.py` & `pygenuz-0.1.9/pygenuz/response.py`

 * *Files identical despite different names*

### Comparing `pygenuz-0.1.8/pygenuz.egg-info/PKG-INFO` & `pygenuz-0.1.9/pygenuz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygenuz
-Version: 0.1.8
+Version: 0.1.9
 Summary: My first Python web framework.
 Home-page: https://github.com/me/myproject
 Author: E'zozbek Kholbutayev
 Author-email: cssezozbel@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -409,15 +409,14 @@
             "author": book.author,
             "published_date": str(book.published_date)
         }
         for book in books
     ]
     response.json = books_data
 ```
-![json](https://img.shields.io/badge/json)
 ##### POST json data 
 ```
 @app.route("/api/book", allowed_methods=["post"])
 def create_book(request, response):
     session = configure_database()
     book_data = request.json
     new_book = Book(
```

### Comparing `pygenuz-0.1.8/setup.py` & `pygenuz-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'pygenuz'
 DESCRIPTION = 'My first Python web framework.'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'cssezozbel@gmail.com'
 AUTHOR = "E'zozbek Kholbutayev"
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.4",
     "parse==1.20.1",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
```

