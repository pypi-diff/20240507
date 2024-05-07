# Comparing `tmp/pygenuz-0.2.1.tar.gz` & `tmp/pygenuz-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygenuz-0.2.1.tar", last modified: Tue May  7 17:45:24 2024, max compression
+gzip compressed data, was "pygenuz-0.2.2.tar", last modified: Tue May  7 17:47:42 2024, max compression
```

## Comparing `pygenuz-0.2.1.tar` & `pygenuz-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:45:24.496129 pygenuz-0.2.1/
--rw-r--r--   0 khezozbek   (501) staff       (20)    13651 2024-05-07 17:45:24.495940 pygenuz-0.2.1/PKG-INFO
--rw-r--r--   0 khezozbek   (501) staff       (20)    13020 2024-05-07 17:45:07.000000 pygenuz-0.2.1/README.md
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:45:24.494894 pygenuz-0.2.1/pygenuz/
--rw-r--r--   0 khezozbek   (501) staff       (20)        0 2024-05-07 07:34:41.000000 pygenuz-0.2.1/pygenuz/__init__.py
--rw-r--r--   0 khezozbek   (501) staff       (20)     3787 2024-05-07 15:58:04.000000 pygenuz-0.2.1/pygenuz/app.py
--rw-r--r--   0 khezozbek   (501) staff       (20)       86 2024-05-07 16:18:44.000000 pygenuz-0.2.1/pygenuz/configs.py
--rw-r--r--   0 khezozbek   (501) staff       (20)      201 2024-05-07 16:08:54.000000 pygenuz-0.2.1/pygenuz/db.py
--rw-r--r--   0 khezozbek   (501) staff       (20)      680 2024-05-06 07:56:45.000000 pygenuz-0.2.1/pygenuz/middelware.py
--rw-r--r--   0 khezozbek   (501) staff       (20)      953 2024-05-06 09:07:08.000000 pygenuz-0.2.1/pygenuz/response.py
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:45:24.495701 pygenuz-0.2.1/pygenuz.egg-info/
--rw-r--r--   0 khezozbek   (501) staff       (20)    13651 2024-05-07 17:45:24.000000 pygenuz-0.2.1/pygenuz.egg-info/PKG-INFO
--rw-r--r--   0 khezozbek   (501) staff       (20)      282 2024-05-07 17:45:24.000000 pygenuz-0.2.1/pygenuz.egg-info/SOURCES.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)        1 2024-05-07 17:45:24.000000 pygenuz-0.2.1/pygenuz.egg-info/dependency_links.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)      116 2024-05-07 17:45:24.000000 pygenuz-0.2.1/pygenuz.egg-info/requires.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)        8 2024-05-07 17:45:24.000000 pygenuz-0.2.1/pygenuz.egg-info/top_level.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)       38 2024-05-07 17:45:24.496193 pygenuz-0.2.1/setup.cfg
--rw-r--r--   0 khezozbek   (501) staff       (20)     3912 2024-05-07 17:45:20.000000 pygenuz-0.2.1/setup.py
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:47:42.861922 pygenuz-0.2.2/
+-rw-r--r--   0 khezozbek   (501) staff       (20)    13654 2024-05-07 17:47:42.861704 pygenuz-0.2.2/PKG-INFO
+-rw-r--r--   0 khezozbek   (501) staff       (20)    13023 2024-05-07 17:47:25.000000 pygenuz-0.2.2/README.md
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:47:42.859602 pygenuz-0.2.2/pygenuz/
+-rw-r--r--   0 khezozbek   (501) staff       (20)        0 2024-05-07 07:34:41.000000 pygenuz-0.2.2/pygenuz/__init__.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)     3787 2024-05-07 15:58:04.000000 pygenuz-0.2.2/pygenuz/app.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)       86 2024-05-07 16:18:44.000000 pygenuz-0.2.2/pygenuz/configs.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)      201 2024-05-07 16:08:54.000000 pygenuz-0.2.2/pygenuz/db.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)      680 2024-05-06 07:56:45.000000 pygenuz-0.2.2/pygenuz/middelware.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)      953 2024-05-06 09:07:08.000000 pygenuz-0.2.2/pygenuz/response.py
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:47:42.861440 pygenuz-0.2.2/pygenuz.egg-info/
+-rw-r--r--   0 khezozbek   (501) staff       (20)    13654 2024-05-07 17:47:42.000000 pygenuz-0.2.2/pygenuz.egg-info/PKG-INFO
+-rw-r--r--   0 khezozbek   (501) staff       (20)      282 2024-05-07 17:47:42.000000 pygenuz-0.2.2/pygenuz.egg-info/SOURCES.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)        1 2024-05-07 17:47:42.000000 pygenuz-0.2.2/pygenuz.egg-info/dependency_links.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)      116 2024-05-07 17:47:42.000000 pygenuz-0.2.2/pygenuz.egg-info/requires.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)        8 2024-05-07 17:47:42.000000 pygenuz-0.2.2/pygenuz.egg-info/top_level.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)       38 2024-05-07 17:47:42.861978 pygenuz-0.2.2/setup.cfg
+-rw-r--r--   0 khezozbek   (501) staff       (20)     3912 2024-05-07 17:47:36.000000 pygenuz-0.2.2/setup.py
```

### Comparing `pygenuz-0.2.1/PKG-INFO` & `pygenuz-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygenuz
-Version: 0.2.1
+Version: 0.2.2
 Summary: My first Python web framework.
 Home-page: https://github.com/me/myproject
 Author: E'zozbek Kholbutayev
 Author-email: cssezozbel@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -345,15 +345,15 @@
         return session 
     else:
         return None
 
 if __name__ == "__main__":
     configure_database()
 ```
-#### After writing configure.py, you need to copy your models to the database. To do this, you need to write a command in the terminal or cmd
+#### After writing configure.py, you need to migrate your models to the database. To do this, you need to write a command in the terminal or cmd
 ```
 python configure.py 
 ```
 ##### will return you a Migrated response if successful else error
 
 ## Using models.py in your views.py or main.py, you must import these codes.
 ```
```

### Comparing `pygenuz-0.2.1/README.md` & `pygenuz-0.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -326,15 +326,15 @@
         return session 
     else:
         return None
 
 if __name__ == "__main__":
     configure_database()
 ```
-#### After writing configure.py, you need to copy your models to the database. To do this, you need to write a command in the terminal or cmd
+#### After writing configure.py, you need to migrate your models to the database. To do this, you need to write a command in the terminal or cmd
 ```
 python configure.py 
 ```
 ##### will return you a Migrated response if successful else error
 
 ## Using models.py in your views.py or main.py, you must import these codes.
 ```
```

### Comparing `pygenuz-0.2.1/pygenuz/app.py` & `pygenuz-0.2.2/pygenuz/app.py`

 * *Files identical despite different names*

### Comparing `pygenuz-0.2.1/pygenuz/middelware.py` & `pygenuz-0.2.2/pygenuz/middelware.py`

 * *Files identical despite different names*

### Comparing `pygenuz-0.2.1/pygenuz/response.py` & `pygenuz-0.2.2/pygenuz/response.py`

 * *Files identical despite different names*

### Comparing `pygenuz-0.2.1/pygenuz.egg-info/PKG-INFO` & `pygenuz-0.2.2/pygenuz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygenuz
-Version: 0.2.1
+Version: 0.2.2
 Summary: My first Python web framework.
 Home-page: https://github.com/me/myproject
 Author: E'zozbek Kholbutayev
 Author-email: cssezozbel@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -345,15 +345,15 @@
         return session 
     else:
         return None
 
 if __name__ == "__main__":
     configure_database()
 ```
-#### After writing configure.py, you need to copy your models to the database. To do this, you need to write a command in the terminal or cmd
+#### After writing configure.py, you need to migrate your models to the database. To do this, you need to write a command in the terminal or cmd
 ```
 python configure.py 
 ```
 ##### will return you a Migrated response if successful else error
 
 ## Using models.py in your views.py or main.py, you must import these codes.
 ```
```

### Comparing `pygenuz-0.2.1/setup.py` & `pygenuz-0.2.2/setup.py`

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
-VERSION = '0.2.1'
+VERSION = '0.2.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.4",
     "parse==1.20.1",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
```

