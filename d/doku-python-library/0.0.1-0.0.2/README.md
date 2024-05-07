# Comparing `tmp/doku_python_library-0.0.1.tar.gz` & `tmp/doku-python-library-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doku_python_library-0.0.1.tar", last modified: Tue May  7 07:23:31 2024, max compression
+gzip compressed data, was "doku-python-library-0.0.2.tar", last modified: Tue May  7 07:28:39 2024, max compression
```

## Comparing `doku_python_library-0.0.1.tar` & `doku-python-library-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 dokuit     (501) staff       (20)        0 2024-05-07 07:23:31.962394 doku_python_library-0.0.1/
--rw-r--r--   0 dokuit     (501) staff       (20)     1056 2024-05-07 06:11:58.000000 doku_python_library-0.0.1/LICENSE.txt
--rw-r--r--   0 dokuit     (501) staff       (20)      375 2024-05-07 07:23:31.961468 doku_python_library-0.0.1/PKG-INFO
-drwxr-xr-x   0 dokuit     (501) staff       (20)        0 2024-05-07 07:23:31.959903 doku_python_library-0.0.1/doku_python_library.egg-info/
--rw-r--r--   0 dokuit     (501) staff       (20)      375 2024-05-07 07:23:31.000000 doku_python_library-0.0.1/doku_python_library.egg-info/PKG-INFO
--rw-r--r--   0 dokuit     (501) staff       (20)      192 2024-05-07 07:23:31.000000 doku_python_library-0.0.1/doku_python_library.egg-info/SOURCES.txt
--rw-r--r--   0 dokuit     (501) staff       (20)        1 2024-05-07 07:23:31.000000 doku_python_library-0.0.1/doku_python_library.egg-info/dependency_links.txt
--rw-r--r--   0 dokuit     (501) staff       (20)        1 2024-05-07 07:23:31.000000 doku_python_library-0.0.1/doku_python_library.egg-info/top_level.txt
--rw-r--r--   0 dokuit     (501) staff       (20)       38 2024-05-07 07:23:31.962495 doku_python_library-0.0.1/setup.cfg
--rw-r--r--   0 dokuit     (501) staff       (20)      395 2024-05-07 07:21:23.000000 doku_python_library-0.0.1/setup.py
+drwxr-xr-x   0 dokuit     (501) staff       (20)        0 2024-05-07 07:28:39.183453 doku-python-library-0.0.2/
+-rw-r--r--   0 dokuit     (501) staff       (20)     1056 2024-05-07 06:11:58.000000 doku-python-library-0.0.2/LICENSE.txt
+-rw-r--r--   0 dokuit     (501) staff       (20)      375 2024-05-07 07:28:39.182923 doku-python-library-0.0.2/PKG-INFO
+drwxr-xr-x   0 dokuit     (501) staff       (20)        0 2024-05-07 07:28:39.182134 doku-python-library-0.0.2/doku_python_library.egg-info/
+-rw-r--r--   0 dokuit     (501) staff       (20)      375 2024-05-07 07:28:39.000000 doku-python-library-0.0.2/doku_python_library.egg-info/PKG-INFO
+-rw-r--r--   0 dokuit     (501) staff       (20)      192 2024-05-07 07:28:39.000000 doku-python-library-0.0.2/doku_python_library.egg-info/SOURCES.txt
+-rw-r--r--   0 dokuit     (501) staff       (20)        1 2024-05-07 07:28:39.000000 doku-python-library-0.0.2/doku_python_library.egg-info/dependency_links.txt
+-rw-r--r--   0 dokuit     (501) staff       (20)        1 2024-05-07 07:28:39.000000 doku-python-library-0.0.2/doku_python_library.egg-info/top_level.txt
+-rw-r--r--   0 dokuit     (501) staff       (20)       38 2024-05-07 07:28:39.183512 doku-python-library-0.0.2/setup.cfg
+-rw-r--r--   0 dokuit     (501) staff       (20)      395 2024-05-07 07:28:21.000000 doku-python-library-0.0.2/setup.py
```

### Comparing `doku_python_library-0.0.1/LICENSE.txt` & `doku-python-library-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

