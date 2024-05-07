# Comparing `tmp/pygenuz-0.1.6.tar.gz` & `tmp/pygenuz-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygenuz-0.1.6.tar", last modified: Tue May  7 17:36:31 2024, max compression
+gzip compressed data, was "pygenuz-0.1.7.tar", last modified: Tue May  7 17:38:15 2024, max compression
```

## Comparing `pygenuz-0.1.6.tar` & `pygenuz-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:36:31.610078 pygenuz-0.1.6/
--rw-r--r--   0 khezozbek   (501) staff       (20)      660 2024-05-07 17:36:31.609955 pygenuz-0.1.6/PKG-INFO
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:36:31.608415 pygenuz-0.1.6/pygenuz/
--rw-r--r--   0 khezozbek   (501) staff       (20)        0 2024-05-07 07:34:41.000000 pygenuz-0.1.6/pygenuz/__init__.py
--rw-r--r--   0 khezozbek   (501) staff       (20)     3787 2024-05-07 15:58:04.000000 pygenuz-0.1.6/pygenuz/app.py
--rw-r--r--   0 khezozbek   (501) staff       (20)       86 2024-05-07 16:18:44.000000 pygenuz-0.1.6/pygenuz/configs.py
--rw-r--r--   0 khezozbek   (501) staff       (20)      201 2024-05-07 16:08:54.000000 pygenuz-0.1.6/pygenuz/db.py
--rw-r--r--   0 khezozbek   (501) staff       (20)      680 2024-05-06 07:56:45.000000 pygenuz-0.1.6/pygenuz/middelware.py
--rw-r--r--   0 khezozbek   (501) staff       (20)      953 2024-05-06 09:07:08.000000 pygenuz-0.1.6/pygenuz/response.py
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:36:31.609664 pygenuz-0.1.6/pygenuz.egg-info/
--rw-r--r--   0 khezozbek   (501) staff       (20)      660 2024-05-07 17:36:31.000000 pygenuz-0.1.6/pygenuz.egg-info/PKG-INFO
--rw-r--r--   0 khezozbek   (501) staff       (20)      272 2024-05-07 17:36:31.000000 pygenuz-0.1.6/pygenuz.egg-info/SOURCES.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)        1 2024-05-07 17:36:31.000000 pygenuz-0.1.6/pygenuz.egg-info/dependency_links.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)      116 2024-05-07 17:36:31.000000 pygenuz-0.1.6/pygenuz.egg-info/requires.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)        8 2024-05-07 17:36:31.000000 pygenuz-0.1.6/pygenuz.egg-info/top_level.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)       38 2024-05-07 17:36:31.610129 pygenuz-0.1.6/setup.cfg
--rw-r--r--   0 khezozbek   (501) staff       (20)     3912 2024-05-07 17:36:28.000000 pygenuz-0.1.6/setup.py
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:38:15.600419 pygenuz-0.1.7/
+-rw-r--r--   0 khezozbek   (501) staff       (20)    13855 2024-05-07 17:38:15.600222 pygenuz-0.1.7/PKG-INFO
+-rw-r--r--   0 khezozbek   (501) staff       (20)    13224 2024-05-07 17:37:53.000000 pygenuz-0.1.7/README.md
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:38:15.599092 pygenuz-0.1.7/pygenuz/
+-rw-r--r--   0 khezozbek   (501) staff       (20)        0 2024-05-07 07:34:41.000000 pygenuz-0.1.7/pygenuz/__init__.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)     3787 2024-05-07 15:58:04.000000 pygenuz-0.1.7/pygenuz/app.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)       86 2024-05-07 16:18:44.000000 pygenuz-0.1.7/pygenuz/configs.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)      201 2024-05-07 16:08:54.000000 pygenuz-0.1.7/pygenuz/db.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)      680 2024-05-06 07:56:45.000000 pygenuz-0.1.7/pygenuz/middelware.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)      953 2024-05-06 09:07:08.000000 pygenuz-0.1.7/pygenuz/response.py
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:38:15.599979 pygenuz-0.1.7/pygenuz.egg-info/
+-rw-r--r--   0 khezozbek   (501) staff       (20)    13855 2024-05-07 17:38:15.000000 pygenuz-0.1.7/pygenuz.egg-info/PKG-INFO
+-rw-r--r--   0 khezozbek   (501) staff       (20)      282 2024-05-07 17:38:15.000000 pygenuz-0.1.7/pygenuz.egg-info/SOURCES.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)        1 2024-05-07 17:38:15.000000 pygenuz-0.1.7/pygenuz.egg-info/dependency_links.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)      116 2024-05-07 17:38:15.000000 pygenuz-0.1.7/pygenuz.egg-info/requires.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)        8 2024-05-07 17:38:15.000000 pygenuz-0.1.7/pygenuz.egg-info/top_level.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)       38 2024-05-07 17:38:15.600483 pygenuz-0.1.7/setup.cfg
+-rw-r--r--   0 khezozbek   (501) staff       (20)     3912 2024-05-07 17:38:07.000000 pygenuz-0.1.7/setup.py
```

### Comparing `pygenuz-0.1.6/pygenuz/app.py` & `pygenuz-0.1.7/pygenuz/app.py`

 * *Files identical despite different names*

### Comparing `pygenuz-0.1.6/pygenuz/middelware.py` & `pygenuz-0.1.7/pygenuz/middelware.py`

 * *Files identical despite different names*

### Comparing `pygenuz-0.1.6/pygenuz/response.py` & `pygenuz-0.1.7/pygenuz/response.py`

 * *Files identical despite different names*

### Comparing `pygenuz-0.1.6/setup.py` & `pygenuz-0.1.7/setup.py`

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
-VERSION = '0.1.6'
+VERSION = '0.1.7'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.4",
     "parse==1.20.1",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
```

