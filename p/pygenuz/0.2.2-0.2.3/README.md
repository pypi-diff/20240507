# Comparing `tmp/pygenuz-0.2.2.tar.gz` & `tmp/pygenuz-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygenuz-0.2.2.tar", last modified: Tue May  7 17:47:42 2024, max compression
+gzip compressed data, was "pygenuz-0.2.3.tar", last modified: Tue May  7 17:50:40 2024, max compression
```

## Comparing `pygenuz-0.2.2.tar` & `pygenuz-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:47:42.861922 pygenuz-0.2.2/
--rw-r--r--   0 khezozbek   (501) staff       (20)    13654 2024-05-07 17:47:42.861704 pygenuz-0.2.2/PKG-INFO
--rw-r--r--   0 khezozbek   (501) staff       (20)    13023 2024-05-07 17:47:25.000000 pygenuz-0.2.2/README.md
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:47:42.859602 pygenuz-0.2.2/pygenuz/
--rw-r--r--   0 khezozbek   (501) staff       (20)        0 2024-05-07 07:34:41.000000 pygenuz-0.2.2/pygenuz/__init__.py
--rw-r--r--   0 khezozbek   (501) staff       (20)     3787 2024-05-07 15:58:04.000000 pygenuz-0.2.2/pygenuz/app.py
--rw-r--r--   0 khezozbek   (501) staff       (20)       86 2024-05-07 16:18:44.000000 pygenuz-0.2.2/pygenuz/configs.py
--rw-r--r--   0 khezozbek   (501) staff       (20)      201 2024-05-07 16:08:54.000000 pygenuz-0.2.2/pygenuz/db.py
--rw-r--r--   0 khezozbek   (501) staff       (20)      680 2024-05-06 07:56:45.000000 pygenuz-0.2.2/pygenuz/middelware.py
--rw-r--r--   0 khezozbek   (501) staff       (20)      953 2024-05-06 09:07:08.000000 pygenuz-0.2.2/pygenuz/response.py
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:47:42.861440 pygenuz-0.2.2/pygenuz.egg-info/
--rw-r--r--   0 khezozbek   (501) staff       (20)    13654 2024-05-07 17:47:42.000000 pygenuz-0.2.2/pygenuz.egg-info/PKG-INFO
--rw-r--r--   0 khezozbek   (501) staff       (20)      282 2024-05-07 17:47:42.000000 pygenuz-0.2.2/pygenuz.egg-info/SOURCES.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)        1 2024-05-07 17:47:42.000000 pygenuz-0.2.2/pygenuz.egg-info/dependency_links.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)      116 2024-05-07 17:47:42.000000 pygenuz-0.2.2/pygenuz.egg-info/requires.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)        8 2024-05-07 17:47:42.000000 pygenuz-0.2.2/pygenuz.egg-info/top_level.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)       38 2024-05-07 17:47:42.861978 pygenuz-0.2.2/setup.cfg
--rw-r--r--   0 khezozbek   (501) staff       (20)     3912 2024-05-07 17:47:36.000000 pygenuz-0.2.2/setup.py
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:50:40.906551 pygenuz-0.2.3/
+-rw-r--r--   0 khezozbek   (501) staff       (20)    13632 2024-05-07 17:50:40.906366 pygenuz-0.2.3/PKG-INFO
+-rw-r--r--   0 khezozbek   (501) staff       (20)    13001 2024-05-07 17:50:20.000000 pygenuz-0.2.3/README.md
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:50:40.905259 pygenuz-0.2.3/pygenuz/
+-rw-r--r--   0 khezozbek   (501) staff       (20)        0 2024-05-07 07:34:41.000000 pygenuz-0.2.3/pygenuz/__init__.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)     3787 2024-05-07 15:58:04.000000 pygenuz-0.2.3/pygenuz/app.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)       86 2024-05-07 16:18:44.000000 pygenuz-0.2.3/pygenuz/configs.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)      201 2024-05-07 16:08:54.000000 pygenuz-0.2.3/pygenuz/db.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)      680 2024-05-06 07:56:45.000000 pygenuz-0.2.3/pygenuz/middelware.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)      953 2024-05-06 09:07:08.000000 pygenuz-0.2.3/pygenuz/response.py
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:50:40.906164 pygenuz-0.2.3/pygenuz.egg-info/
+-rw-r--r--   0 khezozbek   (501) staff       (20)    13632 2024-05-07 17:50:40.000000 pygenuz-0.2.3/pygenuz.egg-info/PKG-INFO
+-rw-r--r--   0 khezozbek   (501) staff       (20)      282 2024-05-07 17:50:40.000000 pygenuz-0.2.3/pygenuz.egg-info/SOURCES.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)        1 2024-05-07 17:50:40.000000 pygenuz-0.2.3/pygenuz.egg-info/dependency_links.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)      116 2024-05-07 17:50:40.000000 pygenuz-0.2.3/pygenuz.egg-info/requires.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)        8 2024-05-07 17:50:40.000000 pygenuz-0.2.3/pygenuz.egg-info/top_level.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)       38 2024-05-07 17:50:40.906601 pygenuz-0.2.3/setup.cfg
+-rw-r--r--   0 khezozbek   (501) staff       (20)     3912 2024-05-07 17:50:39.000000 pygenuz-0.2.3/setup.py
```

### Comparing `pygenuz-0.2.2/PKG-INFO` & `pygenuz-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygenuz
-Version: 0.2.2
+Version: 0.2.3
 Summary: My first Python web framework.
 Home-page: https://github.com/me/myproject
 Author: E'zozbek Kholbutayev
 Author-email: cssezozbel@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -453,15 +453,14 @@
 
 def delete_book(request, response, book_id):
     book = session.query(Book).filter_by(id=book_id).first()
     if not book:
         response.text = f"Book with ID {book_id} not found"
         response.status_code = 404
         return
-    # Delete the book
     session.delete(book)
     session.commit()
     response.text = "Book deleted successfully"
 ```
 
 # EVERY MONDAY YOU WILL SEE A NEW BIG UPDATE UNTIL V1.0.0
```

### Comparing `pygenuz-0.2.2/README.md` & `pygenuz-0.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -434,14 +434,13 @@
 
 def delete_book(request, response, book_id):
     book = session.query(Book).filter_by(id=book_id).first()
     if not book:
         response.text = f"Book with ID {book_id} not found"
         response.status_code = 404
         return
-    # Delete the book
     session.delete(book)
     session.commit()
     response.text = "Book deleted successfully"
 ```
 
 # EVERY MONDAY YOU WILL SEE A NEW BIG UPDATE UNTIL V1.0.0
```

### Comparing `pygenuz-0.2.2/pygenuz/app.py` & `pygenuz-0.2.3/pygenuz/app.py`

 * *Files identical despite different names*

### Comparing `pygenuz-0.2.2/pygenuz/middelware.py` & `pygenuz-0.2.3/pygenuz/middelware.py`

 * *Files identical despite different names*

### Comparing `pygenuz-0.2.2/pygenuz/response.py` & `pygenuz-0.2.3/pygenuz/response.py`

 * *Files identical despite different names*

### Comparing `pygenuz-0.2.2/pygenuz.egg-info/PKG-INFO` & `pygenuz-0.2.3/pygenuz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygenuz
-Version: 0.2.2
+Version: 0.2.3
 Summary: My first Python web framework.
 Home-page: https://github.com/me/myproject
 Author: E'zozbek Kholbutayev
 Author-email: cssezozbel@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -453,15 +453,14 @@
 
 def delete_book(request, response, book_id):
     book = session.query(Book).filter_by(id=book_id).first()
     if not book:
         response.text = f"Book with ID {book_id} not found"
         response.status_code = 404
         return
-    # Delete the book
     session.delete(book)
     session.commit()
     response.text = "Book deleted successfully"
 ```
 
 # EVERY MONDAY YOU WILL SEE A NEW BIG UPDATE UNTIL V1.0.0
```

### Comparing `pygenuz-0.2.2/setup.py` & `pygenuz-0.2.3/setup.py`

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
-VERSION = '0.2.2'
+VERSION = '0.2.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.4",
     "parse==1.20.1",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
```

