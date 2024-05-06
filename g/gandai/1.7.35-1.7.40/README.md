# Comparing `tmp/gandai-1.7.35.tar.gz` & `tmp/gandai-1.7.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.7.35.tar", last modified: Mon May  6 17:49:30 2024, max compression
+gzip compressed data, was "gandai-1.7.40.tar", last modified: Mon May  6 20:33:47 2024, max compression
```

## Comparing `gandai-1.7.35.tar` & `gandai-1.7.40.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 17:49:30.584470 gandai-1.7.35/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.35/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-06 17:49:30.584265 gandai-1.7.35/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 17:49:30.578303 gandai-1.7.35/gandai/
--rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.35/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 17:49:30.582476 gandai-1.7.35/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.35/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.35/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.35/gandai/__pycache__/analytics.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.35/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2600 2024-03-29 15:40:37.000000 gandai-1.7.35/gandai/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.35/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.35/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.35/gandai/__pycache__/google.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5002 2024-05-06 16:10:12.000000 gandai-1.7.35/gandai/__pycache__/gpt.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5730 2023-11-29 03:59:25.000000 gandai-1.7.35/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1394 2024-03-29 15:42:35.000000 gandai-1.7.35/gandai/__pycache__/helpers.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    19189 2024-03-29 16:29:36.000000 gandai-1.7.35/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    10668 2024-05-06 17:41:54.000000 gandai-1.7.35/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    40632 2024-03-29 16:27:30.000000 gandai-1.7.35/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.35/gandai/__pycache__/secrets.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.35/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.35/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1695 2024-03-29 16:07:35.000000 gandai-1.7.35/gandai/__pycache__/tasks.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.35/gandai/analytics.py
--rw-r--r--   0 parker     (501) staff       (20)     1674 2024-03-29 15:34:07.000000 gandai-1.7.35/gandai/constants.py
--rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.35/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.35/gandai/google.py
--rw-r--r--   0 parker     (501) staff       (20)     4216 2024-05-06 16:10:07.000000 gandai-1.7.35/gandai/gpt.py
--rw-r--r--   0 parker     (501) staff       (20)     3969 2023-11-29 03:58:56.000000 gandai-1.7.35/gandai/grata.py
--rw-r--r--   0 parker     (501) staff       (20)      452 2024-03-29 15:34:07.000000 gandai-1.7.35/gandai/helpers.py
--rw-r--r--   0 parker     (501) staff       (20)    14496 2024-03-29 16:29:34.000000 gandai-1.7.35/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 17:49:30.582980 gandai-1.7.35/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.35/gandai/migrations/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 17:49:30.583346 gandai-1.7.35/gandai/migrations/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.35/gandai/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.35/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.35/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.35/gandai/migrations/db_seed.py
--rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.35/gandai/migrations/dealcloud.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 17:49:30.583910 gandai-1.7.35/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.35/gandai/migrations/sql/2305023-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.35/gandai/migrations/sql/230818-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     3342 2024-03-29 15:34:07.000000 gandai-1.7.35/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     4516 2024-05-06 17:41:51.000000 gandai-1.7.35/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)    27713 2024-03-29 16:27:28.000000 gandai-1.7.35/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.35/gandai/secrets.py
--rw-r--r--   0 parker     (501) staff       (20)     1079 2024-03-29 16:07:32.000000 gandai-1.7.35/gandai/tasks.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 17:49:30.584071 gandai-1.7.35/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-06 17:49:30.000000 gandai-1.7.35/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1478 2024-05-06 17:49:30.000000 gandai-1.7.35/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-06 17:49:30.000000 gandai-1.7.35/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-06 17:49:30.000000 gandai-1.7.35/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-06 17:49:11.000000 gandai-1.7.35/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-06 17:49:30.584518 gandai-1.7.35/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.35/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 20:33:47.993949 gandai-1.7.40/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.40/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-06 20:33:47.993707 gandai-1.7.40/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 20:33:47.982163 gandai-1.7.40/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.40/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 20:33:47.990724 gandai-1.7.40/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.40/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.40/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.40/gandai/__pycache__/analytics.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.40/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2600 2024-03-29 15:40:37.000000 gandai-1.7.40/gandai/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.40/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.40/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.40/gandai/__pycache__/google.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5002 2024-05-06 16:10:12.000000 gandai-1.7.40/gandai/__pycache__/gpt.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5730 2023-11-29 03:59:25.000000 gandai-1.7.40/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1394 2024-03-29 15:42:35.000000 gandai-1.7.40/gandai/__pycache__/helpers.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    19189 2024-05-06 20:32:38.000000 gandai-1.7.40/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    10448 2024-05-06 20:32:25.000000 gandai-1.7.40/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    41777 2024-05-06 19:12:07.000000 gandai-1.7.40/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.40/gandai/__pycache__/secrets.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.40/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.40/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1695 2024-03-29 16:07:35.000000 gandai-1.7.40/gandai/__pycache__/tasks.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.40/gandai/analytics.py
+-rw-r--r--   0 parker     (501) staff       (20)     1674 2024-03-29 15:34:07.000000 gandai-1.7.40/gandai/constants.py
+-rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.40/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.40/gandai/google.py
+-rw-r--r--   0 parker     (501) staff       (20)     4216 2024-05-06 16:10:07.000000 gandai-1.7.40/gandai/gpt.py
+-rw-r--r--   0 parker     (501) staff       (20)     3969 2023-11-29 03:58:56.000000 gandai-1.7.40/gandai/grata.py
+-rw-r--r--   0 parker     (501) staff       (20)      452 2024-03-29 15:34:07.000000 gandai-1.7.40/gandai/helpers.py
+-rw-r--r--   0 parker     (501) staff       (20)    14496 2024-05-06 20:32:35.000000 gandai-1.7.40/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 20:33:47.991497 gandai-1.7.40/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.40/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 20:33:47.991858 gandai-1.7.40/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.40/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.40/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.40/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.40/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.40/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 20:33:47.993090 gandai-1.7.40/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.40/gandai/migrations/sql/2305023-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.40/gandai/migrations/sql/230818-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     3342 2024-03-29 15:34:07.000000 gandai-1.7.40/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     4381 2024-05-06 20:32:23.000000 gandai-1.7.40/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)    28456 2024-05-06 19:12:05.000000 gandai-1.7.40/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.40/gandai/secrets.py
+-rw-r--r--   0 parker     (501) staff       (20)     1079 2024-03-29 16:07:32.000000 gandai-1.7.40/gandai/tasks.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 20:33:47.993442 gandai-1.7.40/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-06 20:33:47.000000 gandai-1.7.40/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1478 2024-05-06 20:33:47.000000 gandai-1.7.40/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-06 20:33:47.000000 gandai-1.7.40/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-06 20:33:47.000000 gandai-1.7.40/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-06 20:33:33.000000 gandai-1.7.40/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-06 20:33:47.994020 gandai-1.7.40/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.40/setup.py
```

### Comparing `gandai-1.7.35/gandai/__pycache__/__init__.cpython-311.pyc` & `gandai-1.7.40/gandai/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.7.40/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/__pycache__/analytics.cpython-311.pyc` & `gandai-1.7.40/gandai/__pycache__/analytics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.7.40/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/__pycache__/constants.cpython-311.pyc` & `gandai-1.7.40/gandai/__pycache__/constants.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.7.40/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/__pycache__/db.cpython-311.pyc` & `gandai-1.7.40/gandai/__pycache__/db.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/__pycache__/google.cpython-311.pyc` & `gandai-1.7.40/gandai/__pycache__/google.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/__pycache__/gpt.cpython-311.pyc` & `gandai-1.7.40/gandai/__pycache__/gpt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.7.40/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/__pycache__/helpers.cpython-311.pyc` & `gandai-1.7.40/gandai/__pycache__/helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.7.40/gandai/__pycache__/main.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x6eec0666 (Fri Mar 29 16:29:34 2024 UTC)
+moddate:  0x633e3966 (Mon May  6 20:32:35 2024 UTC)
 files sz: 14496
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `gandai-1.7.35/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.7.40/gandai/__pycache__/models.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x5f163966 (Mon May  6 17:41:51 2024 UTC)
-files sz: 4516
+moddate:  0x573e3966 (Mon May  6 20:32:23 2024 UTC)
+files sz: 4381
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a026d035a036d045a0401
@@ -1418,16 +1418,16 @@
             0464043c000000020065066509ac03a6010000ab0100000000000000005a
             0a6509650464053c000000650b64066505660264078404a6000000ab0000
             000000000000005a0c650b64066505660264088404a6000000ab00000000
             00000000005a0d650b64066505660264098404a6000000ab000000000000
             0000005a0e650b640665056602640a8404a6000000ab0000000000000000
             005a0f650b640665056602640b8404a6000000ab0000000000000000005a
             10650b640665056602640c8404a6000000ab0000000000000000005a1165
-            0b640665056602640d8404a6000000ab0000000000000000005a12650b64
-            0665056602640e8404a6000000ab0000000000000000005a13640f5300
+            0b640665056602640d8404a6000000ab0000000000000000005a12640e53
+            00
          133           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Search')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
@@ -1544,36 +1544,23 @@
          165         266 STORE_NAME              17 (customers)
          
          169         268 LOAD_NAME               11 (property)
          
          170         270 LOAD_CONST               6 ('return')
                      272 LOAD_NAME                5 (str)
                      274 BUILD_TUPLE              2
-                     276 LOAD_CONST              13 (<code object was_acquired, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 169>)
+                     276 LOAD_CONST              13 (<code object token, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 169>)
                      278 MAKE_FUNCTION            4 (annotations)
          
          169         280 PRECALL                  0
                      284 CALL                     0
          
-         170         294 STORE_NAME              18 (was_acquired)
-         
-         174         296 LOAD_NAME               11 (property)
-         
-         175         298 LOAD_CONST               6 ('return')
-                     300 LOAD_NAME                5 (str)
-                     302 BUILD_TUPLE              2
-                     304 LOAD_CONST              14 (<code object token, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 174>)
-                     306 MAKE_FUNCTION            4 (annotations)
-         
-         174         308 PRECALL                  0
-                     312 CALL                     0
-         
-         175         322 STORE_NAME              19 (token)
-                     324 LOAD_CONST              15 (None)
-                     326 RETURN_VALUE
+         170         294 STORE_NAME              18 (token)
+                     296 LOAD_CONST              14 (None)
+                     298 RETURN_VALUE
          consts
             'Search'
             'uid'
             'label'
             ('default_factory',)
             'meta'
             'criteria'
@@ -1751,55 +1738,26 @@
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       'customers'
                firstlineno 164
                lnotab 0x0203
             code
                argcount  : 1
                nlocals   : 1
-               stacksize : 4
-               flags     : 3
-               code
-                  0x97007c006a000000000000000000a00100000000000000000000000000
-                  0000000000000064016400a6020000ab0200000000000000005300
-               169           0 RESUME                   0
-               
-               172           2 LOAD_FAST                0 (self)
-                             4 LOAD_ATTR                0 (meta)
-                            14 LOAD_METHOD              1 (get)
-                            36 LOAD_CONST               1 ('was_acquired')
-                            38 LOAD_CONST               0 (None)
-                            40 PRECALL                  2
-                            44 CALL                     2
-                            54 RETURN_VALUE
-               consts
-                  None
-                  'was_acquired'
-               names      ('meta', 'get')
-               varnames   ('self',)
-               freevars   ()
-               cellvars   ()
-               filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
-               name       'was_acquired'
-               firstlineno 169
-               lnotab 0x0203
-            code
-               argcount  : 1
-               nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007405000000
                   000000000000007c006a030000000000000000a6010000ab010000000000
                   000000a00400000000000000000000000000000000000000006401a60100
                   00ab010000000000000000a6010000ab010000000000000000a005000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   005300
-               174           0 RESUME                   0
+               169           0 RESUME                   0
                
-               177           2 LOAD_GLOBAL              1 (NULL + hashlib)
+               172           2 LOAD_GLOBAL              1 (NULL + hashlib)
                             14 LOAD_ATTR                1 (md5)
                             24 LOAD_GLOBAL              5 (NULL + str)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                3 (uid)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 LOAD_METHOD              4 (encode)
@@ -1817,28 +1775,28 @@
                   'utf-8'
                names      ('hashlib', 'md5', 'str', 'uid', 'encode', 'hexdigest')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       'token'
-               firstlineno 174
+               firstlineno 169
                lnotab 0x0203
             None
-         names      ('__name__', '__module__', '__qualname__', 'int', '__annotations__', 'str', 'field', 'dict', 'meta', 'Criteria', 'criteria', 'property', 'notes', 'type', 'prompt', 'products', 'services', 'customers', 'was_acquired', 'token')
+         names      ('__name__', '__module__', '__qualname__', 'int', '__annotations__', 'str', 'field', 'dict', 'meta', 'Criteria', 'criteria', 'property', 'notes', 'type', 'prompt', 'products', 'services', 'customers', 'token')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Search'
          firstlineno 133
          lnotab
             0x0c020a010a012201220402010aff0e01020302010aff0e01020302010a
             ff0e01020302010aff0e01020402010aff0e01020402010aff0e01020402
-            010aff0e01020402010aff0e01
+            010aff0e01
       'Search'
    names      ('hashlib', 'dataclasses', 'asdict', 'dataclass', 'field', 'enum', 'Enum', 'auto', 'typing', 'Any', 'List', 'Optional', 'Actor', 'Company', 'str', 'EventType', 'Event', 'Comment', 'Rating', 'Inclusion', 'Exclusion', 'Criteria', 'Maps', 'Search')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
    name       '<module>'
```

### Comparing `gandai-1.7.35/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.7.40/gandai/__pycache__/query.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xf0eb0666 (Fri Mar 29 16:27:28 2024 UTC)
-files sz: 27713
+moddate:  0x852b3966 (Mon May  6 19:12:05 2024 UTC)
+files sz: 28456
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 13
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064026c026d035a0301
@@ -13,30 +13,31 @@
       066c0d6d0e5a0e01000200650ea6000000ab000000000000000000010064
       0064016c0f5a10640064076c0f6d115a110100640064086c126d135a1301
       00640064096c146d155a156d165a166d175a176d185a186d195a19010002
       006513a6000000ab0000000000000000005a1a640a6517640b6517660464
       0c84045a1b640d6516640b65106a1c00000000000000006a160000000000
       0000006604640e84045a1d640f6515640b65156604641084045a1e641165
       19640b65196604641284045a1f640a65106a1c00000000000000006a1700
-      00000000000000640b64016604641384045a200900090064376415650765
+      00000000000000640b64016604641384045a200900090064386415650765
       061900000000000000000064166521641765226418652364196522640b64
       01660c641a84055a24640b65096a2500000000000000006602641b84045a
-      266438641d6521640b65096a2500000000000000006604641e84055a2764
+      266439641d6521640b65096a2500000000000000006604641e84055a2764
       1f84005a28640b65096a2500000000000000006602642084045a29642184
       005a2a640b65096a2500000000000000006602642284045a2b640b65096a
       2500000000000000006602642384045a2c641665216602642484045a2d64
       166521640b65096a2500000000000000006604642584045a2e6416652164
-      0b65096a2500000000000000006604642684045a2f64276521640b65106a
-      1c00000000000000006a1900000000000000006604642884045a30642965
-      22640b65106a1c00000000000000006a1900000000000000006604642a84
-      045a31642b6522640b65166604642c84045a32642d6522640b6516660464
-      2e84045a33642f6521640b65176604643084045a34640d6516640b640166
-      04643184045a3564116519640b64016604643284045a36642f6521640b64
-      016604643384045a3764346521640b64016604643584045a386416652164
-      0b64016604643684045a3964015300
+      0b65096a2500000000000000006604642684045a2f64166521640b65096a
+      2500000000000000006604642784045a3064286521640b65106a1c000000
+      00000000006a1900000000000000006604642984045a31642a6522640b65
+      106a1c00000000000000006a1900000000000000006604642b84045a3264
+      2c6522640b65166604642d84045a33642e6522640b65166604642f84045a
+      3464306521640b65176604643184045a35640d6516640b64016604643284
+      045a3664116519640b64016604643384045a3764306521640b6401660464
+      3484045a3864356521640b64016604643684045a3964166521640b640166
+      04643784045a3a64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (hashlib)
                  8 STORE_NAME               0 (hashlib)
    
@@ -187,15 +188,15 @@
                314 MAKE_FUNCTION            4 (annotations)
                316 STORE_NAME              32 (important_targets_from_event)
    
    177         318 NOP
    
    178         320 NOP
    
-   173         322 LOAD_CONST              55 ((False, None))
+   173         322 LOAD_CONST              56 ((False, None))
                324 LOAD_CONST              21 ('companies')
    
    174         326 LOAD_NAME                7 (List)
                328 LOAD_NAME                6 (Any)
                330 BINARY_SUBSCR
    
    173         340 LOAD_CONST              22 ('search_uid')
@@ -227,15 +228,15 @@
                370 LOAD_NAME                9 (pd)
                372 LOAD_ATTR               37 (DataFrame)
                382 BUILD_TUPLE              2
                384 LOAD_CONST              27 (<code object searches_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 269>)
                386 MAKE_FUNCTION            4 (annotations)
                388 STORE_NAME              38 (searches_query)
    
-   302         390 LOAD_CONST              56 ((90,))
+   302         390 LOAD_CONST              57 ((90,))
                392 LOAD_CONST              29 ('trailing_days')
                394 LOAD_NAME               33 (int)
                396 LOAD_CONST              11 ('return')
                398 LOAD_NAME                9 (pd)
                400 LOAD_ATTR               37 (DataFrame)
                410 BUILD_TUPLE              4
                412 LOAD_CONST              30 (<code object recent_validations, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 302>)
@@ -297,109 +298,119 @@
                540 LOAD_NAME                9 (pd)
                542 LOAD_ATTR               37 (DataFrame)
                552 BUILD_TUPLE              4
                554 LOAD_CONST              38 (<code object event_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 642>)
                556 MAKE_FUNCTION            4 (annotations)
                558 STORE_NAME              47 (event_history)
    
-   675         560 LOAD_CONST              39 ('uid')
+   672         560 LOAD_CONST              22 ('search_uid')
                562 LOAD_NAME               33 (int)
                564 LOAD_CONST              11 ('return')
-               566 LOAD_NAME               16 (ts)
-               568 LOAD_ATTR               28 (models)
-               578 LOAD_ATTR               25 (Search)
-               588 BUILD_TUPLE              4
-               590 LOAD_CONST              40 (<code object find_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 675>)
-               592 MAKE_FUNCTION            4 (annotations)
-               594 STORE_NAME              48 (find_search)
-   
-   704         596 LOAD_CONST              41 ('searchToken')
-               598 LOAD_NAME               34 (str)
-               600 LOAD_CONST              11 ('return')
-               602 LOAD_NAME               16 (ts)
-               604 LOAD_ATTR               28 (models)
-               614 LOAD_ATTR               25 (Search)
-               624 BUILD_TUPLE              4
-               626 LOAD_CONST              42 (<code object find_search_by_token, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 704>)
-               628 MAKE_FUNCTION            4 (annotations)
-               630 STORE_NAME              49 (find_search_by_token)
-   
-   713         632 LOAD_CONST              43 ('domain')
-               634 LOAD_NAME               34 (str)
-               636 LOAD_CONST              11 ('return')
-               638 LOAD_NAME               22 (Company)
-               640 BUILD_TUPLE              4
-               642 LOAD_CONST              44 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 713>)
-               644 MAKE_FUNCTION            4 (annotations)
-               646 STORE_NAME              50 (find_company_by_domain)
-   
-   729         648 LOAD_CONST              45 ('email')
-               650 LOAD_NAME               34 (str)
-               652 LOAD_CONST              11 ('return')
-               654 LOAD_NAME               22 (Company)
-               656 BUILD_TUPLE              4
-               658 LOAD_CONST              46 (<code object find_actor_by_email, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 729>)
-               660 MAKE_FUNCTION            4 (annotations)
-               662 STORE_NAME              51 (find_actor_by_email)
-   
-   745         664 LOAD_CONST              47 ('event_id')
-               666 LOAD_NAME               33 (int)
-               668 LOAD_CONST              11 ('return')
-               670 LOAD_NAME               23 (Event)
-               672 BUILD_TUPLE              4
-               674 LOAD_CONST              48 (<code object find_event_by_id, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 745>)
-               676 MAKE_FUNCTION            4 (annotations)
-               678 STORE_NAME              52 (find_event_by_id)
-   
-   764         680 LOAD_CONST              13 ('company')
-               682 LOAD_NAME               22 (Company)
-               684 LOAD_CONST              11 ('return')
-               686 LOAD_CONST               1 (None)
-               688 BUILD_TUPLE              4
-               690 LOAD_CONST              49 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 764>)
-               692 MAKE_FUNCTION            4 (annotations)
-               694 STORE_NAME              53 (update_company)
-   
-   793         696 LOAD_CONST              17 ('search')
-               698 LOAD_NAME               25 (Search)
-               700 LOAD_CONST              11 ('return')
-               702 LOAD_CONST               1 (None)
-               704 BUILD_TUPLE              4
-               706 LOAD_CONST              50 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 793>)
-               708 MAKE_FUNCTION            4 (annotations)
-               710 STORE_NAME              54 (update_search)
-   
-   816         712 LOAD_CONST              47 ('event_id')
-               714 LOAD_NAME               33 (int)
-               716 LOAD_CONST              11 ('return')
-               718 LOAD_CONST               1 (None)
-               720 BUILD_TUPLE              4
-               722 LOAD_CONST              51 (<code object mute_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 816>)
-               724 MAKE_FUNCTION            4 (annotations)
-               726 STORE_NAME              55 (mute_event)
-   
-   839         728 LOAD_CONST              52 ('comment_id')
-               730 LOAD_NAME               33 (int)
-               732 LOAD_CONST              11 ('return')
-               734 LOAD_CONST               1 (None)
-               736 BUILD_TUPLE              4
-               738 LOAD_CONST              53 (<code object delete_comment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 839>)
-               740 MAKE_FUNCTION            4 (annotations)
-               742 STORE_NAME              56 (delete_comment)
-   
-   850         744 LOAD_CONST              22 ('search_uid')
-               746 LOAD_NAME               33 (int)
-               748 LOAD_CONST              11 ('return')
-               750 LOAD_CONST               1 (None)
-               752 BUILD_TUPLE              4
-               754 LOAD_CONST              54 (<code object reset_inbox, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 850>)
-               756 MAKE_FUNCTION            4 (annotations)
-               758 STORE_NAME              57 (reset_inbox)
+               566 LOAD_NAME                9 (pd)
+               568 LOAD_ATTR               37 (DataFrame)
+               578 BUILD_TUPLE              4
+               580 LOAD_CONST              39 (<code object search_criteria_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 672>)
+               582 MAKE_FUNCTION            4 (annotations)
+               584 STORE_NAME              48 (search_criteria_history)
+   
+   701         586 LOAD_CONST              40 ('uid')
+               588 LOAD_NAME               33 (int)
+               590 LOAD_CONST              11 ('return')
+               592 LOAD_NAME               16 (ts)
+               594 LOAD_ATTR               28 (models)
+               604 LOAD_ATTR               25 (Search)
+               614 BUILD_TUPLE              4
+               616 LOAD_CONST              41 (<code object find_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 701>)
+               618 MAKE_FUNCTION            4 (annotations)
+               620 STORE_NAME              49 (find_search)
+   
+   730         622 LOAD_CONST              42 ('searchToken')
+               624 LOAD_NAME               34 (str)
+               626 LOAD_CONST              11 ('return')
+               628 LOAD_NAME               16 (ts)
+               630 LOAD_ATTR               28 (models)
+               640 LOAD_ATTR               25 (Search)
+               650 BUILD_TUPLE              4
+               652 LOAD_CONST              43 (<code object find_search_by_token, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 730>)
+               654 MAKE_FUNCTION            4 (annotations)
+               656 STORE_NAME              50 (find_search_by_token)
+   
+   739         658 LOAD_CONST              44 ('domain')
+               660 LOAD_NAME               34 (str)
+               662 LOAD_CONST              11 ('return')
+               664 LOAD_NAME               22 (Company)
+               666 BUILD_TUPLE              4
+               668 LOAD_CONST              45 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 739>)
+               670 MAKE_FUNCTION            4 (annotations)
+               672 STORE_NAME              51 (find_company_by_domain)
+   
+   755         674 LOAD_CONST              46 ('email')
+               676 LOAD_NAME               34 (str)
+               678 LOAD_CONST              11 ('return')
+               680 LOAD_NAME               22 (Company)
+               682 BUILD_TUPLE              4
+               684 LOAD_CONST              47 (<code object find_actor_by_email, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 755>)
+               686 MAKE_FUNCTION            4 (annotations)
+               688 STORE_NAME              52 (find_actor_by_email)
+   
+   771         690 LOAD_CONST              48 ('event_id')
+               692 LOAD_NAME               33 (int)
+               694 LOAD_CONST              11 ('return')
+               696 LOAD_NAME               23 (Event)
+               698 BUILD_TUPLE              4
+               700 LOAD_CONST              49 (<code object find_event_by_id, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 771>)
+               702 MAKE_FUNCTION            4 (annotations)
+               704 STORE_NAME              53 (find_event_by_id)
+   
+   790         706 LOAD_CONST              13 ('company')
+               708 LOAD_NAME               22 (Company)
+               710 LOAD_CONST              11 ('return')
+               712 LOAD_CONST               1 (None)
+               714 BUILD_TUPLE              4
+               716 LOAD_CONST              50 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 790>)
+               718 MAKE_FUNCTION            4 (annotations)
+               720 STORE_NAME              54 (update_company)
+   
+   819         722 LOAD_CONST              17 ('search')
+               724 LOAD_NAME               25 (Search)
+               726 LOAD_CONST              11 ('return')
+               728 LOAD_CONST               1 (None)
+               730 BUILD_TUPLE              4
+               732 LOAD_CONST              51 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 819>)
+               734 MAKE_FUNCTION            4 (annotations)
+               736 STORE_NAME              55 (update_search)
+   
+   842         738 LOAD_CONST              48 ('event_id')
+               740 LOAD_NAME               33 (int)
+               742 LOAD_CONST              11 ('return')
+               744 LOAD_CONST               1 (None)
+               746 BUILD_TUPLE              4
+               748 LOAD_CONST              52 (<code object mute_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 842>)
+               750 MAKE_FUNCTION            4 (annotations)
+               752 STORE_NAME              56 (mute_event)
+   
+   865         754 LOAD_CONST              53 ('comment_id')
+               756 LOAD_NAME               33 (int)
+               758 LOAD_CONST              11 ('return')
                760 LOAD_CONST               1 (None)
-               762 RETURN_VALUE
+               762 BUILD_TUPLE              4
+               764 LOAD_CONST              54 (<code object delete_comment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 865>)
+               766 MAKE_FUNCTION            4 (annotations)
+               768 STORE_NAME              57 (delete_comment)
+   
+   876         770 LOAD_CONST              22 ('search_uid')
+               772 LOAD_NAME               33 (int)
+               774 LOAD_CONST              11 ('return')
+               776 LOAD_CONST               1 (None)
+               778 BUILD_TUPLE              4
+               780 LOAD_CONST              55 (<code object reset_inbox, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 876>)
+               782 MAKE_FUNCTION            4 (annotations)
+               784 STORE_NAME              58 (reset_inbox)
+               786 LOAD_CONST               1 (None)
+               788 RETURN_VALUE
    consts
       0
       None
       ('asdict',)
       ('time',)
       ('Any', 'List')
       ('from_dict',)
@@ -3283,14 +3294,110 @@
          varnames   ('search_uid', 'statement', 'conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'event_history'
          firstlineno 642
          lnotab 0x02012e0104163401540174fe2e03
+      code
+         argcount  : 1
+         nlocals   : 5
+         stacksize : 6
+         flags     : 3
+         code
+            0x970064017d01740000000000000000000000a001000000000000000000
+            0000000000000000000000a6000000ab00000000000000000035007d027c
+            02a002000000000000000000000000000000000000000074070000000000
+            00000000006a0400000000000000007c01a6010000ab0100000000000000
+            0064027c006901a6020000ab0200000000000000007d03740b0000000000
+            00000000006a0600000000000000007c03a0070000000000000000000000
+            000000000000000000a6000000ab0000000000000000007c03a008000000
+            0000000000000000000000000000000000a6000000ab0000000000000000
+            00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
+            02000000000000000001006e0b2300310073047702780359007701010059
+            00010001007c045300
+         672           0 RESUME                   0
+         
+         674           2 LOAD_CONST               1 ("\n    SELECT \n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.data,\n        -- a.type as actor_type,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type in ('import', 'criteria','google','google_maps')\n    ORDER BY created DESC\n    ;\n    ")
+                       4 STORE_FAST               1 (statement)
+         
+         692           6 LOAD_GLOBAL              0 (db)
+                      18 LOAD_METHOD              1 (connect)
+                      40 PRECALL                  0
+                      44 CALL                     0
+                      54 BEFORE_WITH
+                      56 STORE_FAST               2 (conn)
+         
+         693          58 LOAD_FAST                2 (conn)
+                      60 LOAD_METHOD              2 (execute)
+                      82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+                      94 LOAD_ATTR                4 (text)
+                     104 LOAD_FAST                1 (statement)
+                     106 PRECALL                  1
+                     110 CALL                     1
+                     120 LOAD_CONST               2 ('search_uid')
+                     122 LOAD_FAST                0 (search_uid)
+                     124 BUILD_MAP                1
+                     126 PRECALL                  2
+                     130 CALL                     2
+                     140 STORE_FAST               3 (result)
+         
+         694         142 LOAD_GLOBAL             11 (NULL + pd)
+                     154 LOAD_ATTR                6 (DataFrame)
+                     164 LOAD_FAST                3 (result)
+                     166 LOAD_METHOD              7 (fetchall)
+                     188 PRECALL                  0
+                     192 CALL                     0
+                     202 LOAD_FAST                3 (result)
+                     204 LOAD_METHOD              8 (keys)
+                     226 PRECALL                  0
+                     230 CALL                     0
+                     240 KW_NAMES                 3
+                     242 PRECALL                  2
+                     246 CALL                     2
+                     256 STORE_FAST               4 (df)
+         
+         692         258 LOAD_CONST               0 (None)
+                     260 LOAD_CONST               0 (None)
+                     262 LOAD_CONST               0 (None)
+                     264 PRECALL                  2
+                     268 CALL                     2
+                     278 POP_TOP
+                     280 JUMP_FORWARD            11 (to 304)
+                 >>  282 PUSH_EXC_INFO
+                     284 WITH_EXCEPT_START
+                     286 POP_JUMP_FORWARD_IF_TRUE     4 (to 296)
+                     288 RERAISE                  2
+                 >>  290 COPY                     3
+                     292 POP_EXCEPT
+                     294 RERAISE                  1
+                 >>  296 POP_TOP
+                     298 POP_EXCEPT
+                     300 POP_TOP
+                     302 POP_TOP
+         
+         695     >>  304 LOAD_FAST                4 (df)
+                     306 RETURN_VALUE
+         ExceptionTable:
+           56 to 256 -> 282 [1] lasti
+           282 to 288 -> 290 [3] lasti
+           296 to 296 -> 290 [3] lasti
+         consts
+            None
+            "\n    SELECT \n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.data,\n        -- a.type as actor_type,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type in ('import', 'criteria','google','google_maps')\n    ORDER BY created DESC\n    ;\n    "
+            'search_uid'
+            ('columns',)
+         names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
+         varnames   ('search_uid', 'statement', 'conn', 'result', 'df')
+         freevars   ()
+         cellvars   ()
+         filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
+         name       'search_criteria_history'
+         firstlineno 672
+         lnotab 0x020204123401540174fe2e03
       'uid'
       code
          argcount  : 1
          nlocals   : 7
          stacksize : 7
          flags     : 3
          code
@@ -3307,96 +3414,96 @@
             000000000000007d05741300000000000000000000741400000000000000
             0000006a0b00000000000000006a0c00000000000000007c05a6020000ab
             0200000000000000007d067c066a0d0000000000000000a00e0000000000
             0000000000000000000000000000006403a6010000ab0100000000000000
             006404190000000000000000007c066a0f000000000000000064053c0000
             00640064006400a6020000ab02000000000000000001006e0b2300310073
             04770278035900770101005900010001007c065300
-         675           0 RESUME                   0
+         701           0 RESUME                   0
          
-         676           2 LOAD_GLOBAL              0 (db)
+         702           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         677          54 LOAD_CONST               1 ("\n            SELECT \n                uid, \n                label, \n                meta, \n                fields, \n                meta->>'next_due_date' as next_due_date,\n                meta->>'notes' as notes,\n                COALESCE(criteria.data, '{}'::jsonb) as criteria\n            FROM search\n            LEFT JOIN criteria ON search.uid = criteria.search_uid\n            \n            WHERE uid = :uid\n            ")
+         703          54 LOAD_CONST               1 ("\n            SELECT \n                uid, \n                label, \n                meta, \n                fields, \n                meta->>'next_due_date' as next_due_date,\n                meta->>'notes' as notes,\n                COALESCE(criteria.data, '{}'::jsonb) as criteria\n            FROM search\n            LEFT JOIN criteria ON search.uid = criteria.search_uid\n            \n            WHERE uid = :uid\n            ")
                       56 STORE_FAST               2 (statement)
          
-         691          58 LOAD_FAST                1 (conn)
+         717          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('uid')
                      122 LOAD_FAST                0 (uid)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         693         142 LOAD_FAST                3 (result)
+         719         142 LOAD_FAST                3 (result)
                      144 LOAD_METHOD              5 (fetchone)
                      166 PRECALL                  0
                      170 CALL                     0
                      180 STORE_FAST               4 (row)
          
-         694         182 LOAD_FAST                4 (row)
+         720         182 LOAD_FAST                4 (row)
                      184 POP_JUMP_FORWARD_IF_NOT_NONE    14 (to 214)
          
-         695         186 NOP
+         721         186 NOP
          
-         676         188 LOAD_CONST               0 (None)
+         702         188 LOAD_CONST               0 (None)
                      190 LOAD_CONST               0 (None)
                      192 LOAD_CONST               0 (None)
                      194 PRECALL                  2
                      198 CALL                     2
                      208 POP_TOP
                      210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         697     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         723     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                4 (row)
                      278 PRECALL                  2
                      282 CALL                     2
                      292 PRECALL                  1
                      296 CALL                     1
                      306 STORE_FAST               5 (obj)
          
-         698         308 LOAD_GLOBAL             19 (NULL + from_dict)
+         724         308 LOAD_GLOBAL             19 (NULL + from_dict)
                      320 LOAD_GLOBAL             20 (ts)
                      332 LOAD_ATTR               11 (models)
                      342 LOAD_ATTR               12 (Search)
                      352 LOAD_FAST                5 (obj)
                      354 PRECALL                  2
                      358 CALL                     2
                      368 STORE_FAST               6 (search)
          
-         699         370 LOAD_FAST                6 (search)
+         725         370 LOAD_FAST                6 (search)
                      372 LOAD_ATTR               13 (label)
                      382 LOAD_METHOD             14 (split)
                      404 LOAD_CONST               3 (' - ')
                      406 PRECALL                  1
                      410 CALL                     1
                      420 LOAD_CONST               4 (0)
                      422 BINARY_SUBSCR
                      432 LOAD_FAST                6 (search)
                      434 LOAD_ATTR               15 (meta)
                      444 LOAD_CONST               5 ('client')
                      446 STORE_SUBSCR
          
-         676         450 LOAD_CONST               0 (None)
+         702         450 LOAD_CONST               0 (None)
                      452 LOAD_CONST               0 (None)
                      454 LOAD_CONST               0 (None)
                      456 PRECALL                  2
                      460 CALL                     2
                      470 POP_TOP
                      472 JUMP_FORWARD            11 (to 496)
                  >>  474 PUSH_EXC_INFO
@@ -3407,15 +3514,15 @@
                      484 POP_EXCEPT
                      486 RERAISE                  1
                  >>  488 POP_TOP
                      490 POP_EXCEPT
                      492 POP_TOP
                      494 POP_TOP
          
-         701     >>  496 LOAD_FAST                6 (search)
+         727     >>  496 LOAD_FAST                6 (search)
                      498 RETURN_VALUE
          ExceptionTable:
            52 to 186 -> 474 [1] lasti
            214 to 448 -> 474 [1] lasti
            474 to 480 -> 482 [3] lasti
            488 to 488 -> 482 [3] lasti
          consts
@@ -3427,52 +3534,52 @@
             'client'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'fetchone', 'dict', 'zip', 'keys', 'from_dict', 'ts', 'models', 'Search', 'label', 'split', 'meta')
          varnames   ('uid', 'conn', 'statement', 'result', 'row', 'obj', 'search')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_search'
-         firstlineno 675
+         firstlineno 701
          lnotab 0x02013401040e54022801040102ed1a155e013e0150e92e19
       'searchToken'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 4
          flags     : 3
          code
             0x9700740100000000000000000000a6000000ab0000000000000000007d
             017c017c016401190000000000000000007c006b02000000001900000000
             00000000007d027c026a0100000000000000007202640053007405000000
             000000000000007c026a0300000000000000006402190000000000000000
             00640319000000000000000000a6010000ab0100000000000000005300
-         704           0 RESUME                   0
+         730           0 RESUME                   0
          
-         705           2 LOAD_GLOBAL              1 (NULL + searches_query)
+         731           2 LOAD_GLOBAL              1 (NULL + searches_query)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 STORE_FAST               1 (searches)
          
-         706          30 LOAD_FAST                1 (searches)
+         732          30 LOAD_FAST                1 (searches)
                       32 LOAD_FAST                1 (searches)
                       34 LOAD_CONST               1 ('searchToken')
                       36 BINARY_SUBSCR
                       46 LOAD_FAST                0 (searchToken)
                       48 COMPARE_OP               2 (==)
                       54 BINARY_SUBSCR
                       64 STORE_FAST               2 (search)
          
-         707          66 LOAD_FAST                2 (search)
+         733          66 LOAD_FAST                2 (search)
                       68 LOAD_ATTR                1 (empty)
                       78 POP_JUMP_FORWARD_IF_FALSE     2 (to 84)
          
-         708          80 LOAD_CONST               0 (None)
+         734          80 LOAD_CONST               0 (None)
                       82 RETURN_VALUE
          
-         710     >>   84 LOAD_GLOBAL              5 (NULL + find_search)
+         736     >>   84 LOAD_GLOBAL              5 (NULL + find_search)
                       96 LOAD_FAST                2 (search)
                       98 LOAD_ATTR                3 (iloc)
                      108 LOAD_CONST               2 (0)
                      110 BINARY_SUBSCR
                      120 LOAD_CONST               3 ('uid')
                      122 BINARY_SUBSCR
                      132 PRECALL                  1
@@ -3485,15 +3592,15 @@
             'uid'
          names      ('searches_query', 'empty', 'find_search', 'iloc')
          varnames   ('searchToken', 'searches', 'search')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_search_by_token'
-         firstlineno 704
+         firstlineno 730
          lnotab 0x02011c0124010e010402
       'domain'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -3507,41 +3614,41 @@
             0101005900010001007c036a05000000000000000064036b020000000072
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000005300
-         713           0 RESUME                   0
+         739           0 RESUME                   0
          
-         714           2 LOAD_GLOBAL              0 (db)
+         740           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         715          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
+         741          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         720          58 LOAD_FAST                1 (conn)
+         746          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('domain')
                      122 LOAD_FAST                0 (domain)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         714         142 LOAD_CONST               0 (None)
+         740         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -3552,24 +3659,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         722     >>  188 LOAD_FAST                3 (result)
+         748     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         723         210 LOAD_CONST               0 (None)
+         749         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         725     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         751     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -3577,15 +3684,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         726         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         752         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Company)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
@@ -3598,15 +3705,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Company')
          varnames   ('domain', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_company_by_domain'
-         firstlineno 713
+         firstlineno 739
          lnotab 0x02013401040554fa2e08160104028201
       'email'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -3621,41 +3728,41 @@
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000006a0c00000000000000006a0d00000000000000007c
             04a6020000ab0200000000000000005300
-         729           0 RESUME                   0
+         755           0 RESUME                   0
          
-         730           2 LOAD_GLOBAL              0 (db)
+         756           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         731          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM actor\n                WHERE email = :email\n            ')
+         757          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM actor\n                WHERE email = :email\n            ')
                       56 STORE_FAST               2 (statement)
          
-         736          58 LOAD_FAST                1 (conn)
+         762          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('email')
                      122 LOAD_FAST                0 (email)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         730         142 LOAD_CONST               0 (None)
+         756         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -3666,24 +3773,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         738     >>  188 LOAD_FAST                3 (result)
+         764     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         739         210 LOAD_CONST               0 (None)
+         765         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         741     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         767     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -3691,15 +3798,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         742         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         768         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (ts)
                      368 LOAD_ATTR               12 (models)
                      378 LOAD_ATTR               13 (Actor)
                      388 LOAD_FAST                4 (obj)
                      390 PRECALL                  2
                      394 CALL                     2
                      404 RETURN_VALUE
@@ -3714,15 +3821,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'ts', 'models', 'Actor')
          varnames   ('email', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_actor_by_email'
-         firstlineno 729
+         firstlineno 755
          lnotab 0x02013401040554fa2e08160104028201
       'event_id'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -3736,41 +3843,41 @@
             0101005900010001007c036a05000000000000000064036b020000000072
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000005300
-         745           0 RESUME                   0
+         771           0 RESUME                   0
          
-         746           2 LOAD_GLOBAL              0 (db)
+         772           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         747          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE id = :event_id\n            ')
+         773          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE id = :event_id\n            ')
                       56 STORE_FAST               2 (statement)
          
-         752          58 LOAD_FAST                1 (conn)
+         778          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('event_id')
                      122 LOAD_FAST                0 (event_id)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         746         142 LOAD_CONST               0 (None)
+         772         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -3781,24 +3888,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         754     >>  188 LOAD_FAST                3 (result)
+         780     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         755         210 LOAD_CONST               0 (None)
+         781         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         757     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         783     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -3806,15 +3913,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         758         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         784         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Event)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
@@ -3827,15 +3934,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Event')
          varnames   ('event_id', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_event_by_id'
-         firstlineno 745
+         firstlineno 771
          lnotab 0x02013401040554fa2e08160104028201
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 12
          flags     : 3
          code
@@ -3847,71 +3954,71 @@
             000000000000007c006a0800000000000000007c006a0900000000000000
             007415000000000000000000006a0b00000000000000007c006a0c000000
             0000000000a6010000ab01000000000000000064029c06a6020000ab0200
             0000000000000001007c01a00d0000000000000000000000000000000000
             000000a6000000ab0000000000000000000100640064006400a6020000ab
             020000000000000000010064005300230031007304770278035900770101
             0059000100010064005300
-         764           0 RESUME                   0
+         790           0 RESUME                   0
          
-         765           2 LOAD_GLOBAL              0 (db)
+         791           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         766          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                uid = :uid,\n                name = :name,\n                description = :description,\n                source = :source,\n                meta = :meta,\n                updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n            WHERE domain = :domain\n            ')
+         792          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                uid = :uid,\n                name = :name,\n                description = :description,\n                source = :source,\n                meta = :meta,\n                updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n            WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         778          58 LOAD_FAST                1 (conn)
+         804          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         779          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         805          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         781         120 LOAD_FAST                0 (company)
+         807         120 LOAD_FAST                0 (company)
                      122 LOAD_ATTR                5 (uid)
          
-         782         132 LOAD_FAST                0 (company)
+         808         132 LOAD_FAST                0 (company)
                      134 LOAD_ATTR                6 (name)
          
-         783         144 LOAD_FAST                0 (company)
+         809         144 LOAD_FAST                0 (company)
                      146 LOAD_ATTR                7 (description)
          
-         784         156 LOAD_FAST                0 (company)
+         810         156 LOAD_FAST                0 (company)
                      158 LOAD_ATTR                8 (domain)
          
-         785         168 LOAD_FAST                0 (company)
+         811         168 LOAD_FAST                0 (company)
                      170 LOAD_ATTR                9 (source)
          
-         786         180 LOAD_GLOBAL             21 (NULL + json)
+         812         180 LOAD_GLOBAL             21 (NULL + json)
                      192 LOAD_ATTR               11 (dumps)
                      202 LOAD_FAST                0 (company)
                      204 LOAD_ATTR               12 (meta)
                      214 PRECALL                  1
                      218 CALL                     1
          
-         780         228 LOAD_CONST               2 (('uid', 'name', 'description', 'domain', 'source', 'meta'))
+         806         228 LOAD_CONST               2 (('uid', 'name', 'description', 'domain', 'source', 'meta'))
                      230 BUILD_CONST_KEY_MAP      6
          
-         778         232 PRECALL                  2
+         804         232 PRECALL                  2
                      236 CALL                     2
                      246 POP_TOP
          
-         790         248 LOAD_FAST                1 (conn)
+         816         248 LOAD_FAST                1 (conn)
                      250 LOAD_METHOD             13 (commit)
                      272 PRECALL                  0
                      276 CALL                     0
                      286 POP_TOP
          
-         765         288 LOAD_CONST               0 (None)
+         791         288 LOAD_CONST               0 (None)
                      290 LOAD_CONST               0 (None)
                      292 LOAD_CONST               0 (None)
                      294 PRECALL                  2
                      298 CALL                     2
                      308 POP_TOP
                      310 LOAD_CONST               0 (None)
                      312 RETURN_VALUE
@@ -3938,15 +4045,15 @@
             ('uid', 'name', 'description', 'domain', 'source', 'meta')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'uid', 'name', 'description', 'domain', 'source', 'json', 'dumps', 'meta', 'commit')
          varnames   ('company', 'conn', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_company'
-         firstlineno 764
+         firstlineno 790
          lnotab 0x02013401040c180126020c010c010c010c010c0130fa04fe100c28e7
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 7
          flags     : 3
          code
@@ -3956,58 +4063,58 @@
             006a0400000000000000006401a6010000ab010000000000000000740b00
             0000000000000000006a0600000000000000007c006a0700000000000000
             00a6010000ab0100000000000000007c006a08000000000000000064029c
             02a6020000ab02000000000000000001007c01a009000000000000000000
             0000000000000000000000a6000000ab0000000000000000000100640064
             006400a6020000ab02000000000000000001006400530023003100730477
             02780359007701010059000100010064005300
-         793           0 RESUME                   0
+         819           0 RESUME                   0
          
-         794           2 LOAD_GLOBAL              0 (db)
+         820           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         795          54 LOAD_FAST                1 (conn)
+         821          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         796          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         822          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         797         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    meta = :meta,\n                    updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n                WHERE uid = :uid\n                ')
+         823         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    meta = :meta,\n                    updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n                WHERE uid = :uid\n                ')
          
-         796         102 PRECALL                  1
+         822         102 PRECALL                  1
                      106 CALL                     1
          
-         806         116 LOAD_GLOBAL             11 (NULL + json)
+         832         116 LOAD_GLOBAL             11 (NULL + json)
                      128 LOAD_ATTR                6 (dumps)
                      138 LOAD_FAST                0 (search)
                      140 LOAD_ATTR                7 (meta)
                      150 PRECALL                  1
                      154 CALL                     1
          
-         807         164 LOAD_FAST                0 (search)
+         833         164 LOAD_FAST                0 (search)
                      166 LOAD_ATTR                8 (uid)
          
-         805         176 LOAD_CONST               2 (('meta', 'uid'))
+         831         176 LOAD_CONST               2 (('meta', 'uid'))
                      178 BUILD_CONST_KEY_MAP      2
          
-         795         180 PRECALL                  2
+         821         180 PRECALL                  2
                      184 CALL                     2
                      194 POP_TOP
          
-         810         196 LOAD_FAST                1 (conn)
+         836         196 LOAD_FAST                1 (conn)
                      198 LOAD_METHOD              9 (commit)
                      220 PRECALL                  0
                      224 CALL                     0
                      234 POP_TOP
          
-         794         236 LOAD_CONST               0 (None)
+         820         236 LOAD_CONST               0 (None)
                      238 LOAD_CONST               0 (None)
                      240 LOAD_CONST               0 (None)
                      242 PRECALL                  2
                      246 CALL                     2
                      256 POP_TOP
                      258 LOAD_CONST               0 (None)
                      260 RETURN_VALUE
@@ -4034,15 +4141,15 @@
             ('meta', 'uid')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'json', 'dumps', 'meta', 'uid', 'commit')
          varnames   ('search', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_search'
-         firstlineno 793
+         firstlineno 819
          lnotab 0x020134011801160102ff0e0a30010cfe04f6100f28f0
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
@@ -4053,61 +4160,61 @@
             006901a6020000ab02000000000000000001007c01a00200000000000000
             000000000000000000000000007407000000000000000000006a04000000
             00000000006403a6010000ab010000000000000000a6010000ab01000000
             000000000001007c01a00500000000000000000000000000000000000000
             00a6000000ab0000000000000000000100640064006400a6020000ab0200
             000000000000000100640053002300310073047702780359007701010059
             000100010064005300
-         816           0 RESUME                   0
+         842           0 RESUME                   0
          
-         818           2 LOAD_GLOBAL              0 (db)
+         844           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         819          54 LOAD_FAST                1 (conn)
+         845          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         820          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         846          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         821         100 LOAD_CONST               1 ("\n                UPDATE event\n                SET\n                    type = 'mute'\n                WHERE id = :event_id\n                ")
+         847         100 LOAD_CONST               1 ("\n                UPDATE event\n                SET\n                    type = 'mute'\n                WHERE id = :event_id\n                ")
          
-         820         102 PRECALL                  1
+         846         102 PRECALL                  1
                      106 CALL                     1
          
-         829         116 LOAD_CONST               2 ('event_id')
+         855         116 LOAD_CONST               2 ('event_id')
                      118 LOAD_FAST                0 (event_id)
          
-         828         120 BUILD_MAP                1
+         854         120 BUILD_MAP                1
          
-         819         122 PRECALL                  2
+         845         122 PRECALL                  2
                      126 CALL                     2
                      136 POP_TOP
          
-         832         138 LOAD_FAST                1 (conn)
+         858         138 LOAD_FAST                1 (conn)
                      140 LOAD_METHOD              2 (execute)
                      162 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      174 LOAD_ATTR                4 (text)
                      184 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW comment')
                      186 PRECALL                  1
                      190 CALL                     1
                      200 PRECALL                  1
                      204 CALL                     1
                      214 POP_TOP
          
-         833         216 LOAD_FAST                1 (conn)
+         859         216 LOAD_FAST                1 (conn)
                      218 LOAD_METHOD              5 (commit)
                      240 PRECALL                  0
                      244 CALL                     0
                      254 POP_TOP
          
-         818         256 LOAD_CONST               0 (None)
+         844         256 LOAD_CONST               0 (None)
                      258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 PRECALL                  2
                      266 CALL                     2
                      276 POP_TOP
                      278 LOAD_CONST               0 (None)
                      280 RETURN_VALUE
@@ -4135,15 +4242,15 @@
             'REFRESH MATERIALIZED VIEW comment'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit')
          varnames   ('event_id', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'mute_event'
-         firstlineno 816
+         firstlineno 842
          lnotab 0x020234011801160102ff0e0904ff02f7100d4e0128f1
       'comment_id'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
@@ -4155,58 +4262,58 @@
             0064027c006901a6020000ab02000000000000000001007c01a002000000
             00000000000000000000000000000000007407000000000000000000006a
             0400000000000000006403a6010000ab010000000000000000a6010000ab
             01000000000000000001007c01a005000000000000000000000000000000
             0000000000a6000000ab0000000000000000000100640064006400a60200
             00ab02000000000000000001006400530023003100730477027803590077
             01010059000100010064005300
-         839           0 RESUME                   0
+         865           0 RESUME                   0
          
-         840           2 LOAD_GLOBAL              0 (db)
+         866           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         841          54 LOAD_CONST               1 ('\n                DELETE FROM event\n                WHERE id = :comment_id\n            ')
+         867          54 LOAD_CONST               1 ('\n                DELETE FROM event\n                WHERE id = :comment_id\n            ')
                       56 STORE_FAST               2 (statement)
          
-         845          58 LOAD_FAST                1 (conn)
+         871          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('comment_id')
                      122 LOAD_FAST                0 (comment_id)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 POP_TOP
          
-         846         142 LOAD_FAST                1 (conn)
+         872         142 LOAD_FAST                1 (conn)
                      144 LOAD_METHOD              2 (execute)
                      166 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      178 LOAD_ATTR                4 (text)
                      188 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW comment')
                      190 PRECALL                  1
                      194 CALL                     1
                      204 PRECALL                  1
                      208 CALL                     1
                      218 POP_TOP
          
-         847         220 LOAD_FAST                1 (conn)
+         873         220 LOAD_FAST                1 (conn)
                      222 LOAD_METHOD              5 (commit)
                      244 PRECALL                  0
                      248 CALL                     0
                      258 POP_TOP
          
-         840         260 LOAD_CONST               0 (None)
+         866         260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 LOAD_CONST               0 (None)
                      266 PRECALL                  2
                      270 CALL                     2
                      280 POP_TOP
                      282 LOAD_CONST               0 (None)
                      284 RETURN_VALUE
@@ -4234,15 +4341,15 @@
             'REFRESH MATERIALIZED VIEW comment'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit')
          varnames   ('comment_id', 'conn', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'delete_comment'
-         firstlineno 839
+         firstlineno 865
          lnotab 0x02013401040454014e0128f9
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
@@ -4255,71 +4362,71 @@
             00000000006403a6010000ab010000000000000000a6010000ab01000000
             000000000001007c01a00200000000000000000000000000000000000000
             007407000000000000000000006a0400000000000000006404a6010000ab
             010000000000000000a6010000ab01000000000000000001007c01a00500
             00000000000000000000000000000000000000a6000000ab000000000000
             0000000100640064006400a6020000ab0200000000000000000100640053
             002300310073047702780359007701010059000100010064005300
-         850           0 RESUME                   0
+         876           0 RESUME                   0
          
-         854           2 LOAD_GLOBAL              0 (db)
+         880           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         855          54 LOAD_FAST                1 (conn)
+         881          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         856          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         882          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         857         100 LOAD_CONST               1 ("\n                DELETE FROM event\n                WHERE search_uid = :search_uid\n                and type = 'create'\n                ")
+         883         100 LOAD_CONST               1 ("\n                DELETE FROM event\n                WHERE search_uid = :search_uid\n                and type = 'create'\n                ")
          
-         856         102 PRECALL                  1
+         882         102 PRECALL                  1
                      106 CALL                     1
          
-         863         116 LOAD_CONST               2 ('search_uid')
+         889         116 LOAD_CONST               2 ('search_uid')
                      118 LOAD_FAST                0 (search_uid)
                      120 BUILD_MAP                1
          
-         855         122 PRECALL                  2
+         881         122 PRECALL                  2
                      126 CALL                     2
                      136 POP_TOP
          
-         865         138 LOAD_FAST                1 (conn)
+         891         138 LOAD_FAST                1 (conn)
                      140 LOAD_METHOD              2 (execute)
                      162 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      174 LOAD_ATTR                4 (text)
                      184 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW comment')
                      186 PRECALL                  1
                      190 CALL                     1
                      200 PRECALL                  1
                      204 CALL                     1
                      214 POP_TOP
          
-         866         216 LOAD_FAST                1 (conn)
+         892         216 LOAD_FAST                1 (conn)
                      218 LOAD_METHOD              2 (execute)
                      240 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      252 LOAD_ATTR                4 (text)
                      262 LOAD_CONST               4 ('REFRESH MATERIALIZED VIEW rating')
                      264 PRECALL                  1
                      268 CALL                     1
                      278 PRECALL                  1
                      282 CALL                     1
                      292 POP_TOP
          
-         869         294 LOAD_FAST                1 (conn)
+         895         294 LOAD_FAST                1 (conn)
                      296 LOAD_METHOD              5 (commit)
                      318 PRECALL                  0
                      322 CALL                     0
                      332 POP_TOP
          
-         854         334 LOAD_CONST               0 (None)
+         880         334 LOAD_CONST               0 (None)
                      336 LOAD_CONST               0 (None)
                      338 LOAD_CONST               0 (None)
                      340 PRECALL                  2
                      344 CALL                     2
                      354 POP_TOP
                      356 LOAD_CONST               0 (None)
                      358 RETURN_VALUE
@@ -4348,23 +4455,23 @@
             'REFRESH MATERIALIZED VIEW rating'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit')
          varnames   ('search_uid', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'reset_inbox'
-         firstlineno 850
+         firstlineno 876
          lnotab 0x020434011801160102ff0e0706f8100a4e014e0328f1
       (False, None)
       (90,)
-   names      ('hashlib', 'json', 'dataclasses', 'asdict', 'time', 'typing', 'Any', 'List', 'pandas', 'pd', 'sqlalchemy', 'dacite', 'from_dict', 'dotenv', 'load_dotenv', 'gandai', 'ts', 'helpers', 'gandai.db', 'connect_with_connector', 'gandai.models', 'Actor', 'Company', 'Event', 'EventType', 'Search', 'db', 'insert_event', 'models', 'insert_company', 'insert_actor', 'insert_search', 'important_targets_from_event', 'int', 'str', 'bool', 'insert_companies_as_targets', 'DataFrame', 'searches_query', 'recent_validations', 'average_rating_per_search_query', 'validation_history', 'enriched_searches_query', 'actor', 'buyer', 'search_targets', 'event', 'event_history', 'find_search', 'find_search_by_token', 'find_company_by_domain', 'find_actor_by_email', 'find_event_by_id', 'update_company', 'update_search', 'mute_event', 'delete_comment', 'reset_inbox')
+   names      ('hashlib', 'json', 'dataclasses', 'asdict', 'time', 'typing', 'Any', 'List', 'pandas', 'pd', 'sqlalchemy', 'dacite', 'from_dict', 'dotenv', 'load_dotenv', 'gandai', 'ts', 'helpers', 'gandai.db', 'connect_with_connector', 'gandai.models', 'Actor', 'Company', 'Event', 'EventType', 'Search', 'db', 'insert_event', 'models', 'insert_company', 'insert_actor', 'insert_search', 'important_targets_from_event', 'int', 'str', 'bool', 'insert_companies_as_targets', 'DataFrame', 'searches_query', 'recent_validations', 'average_rating_per_search_query', 'validation_history', 'enriched_searches_query', 'actor', 'buyer', 'search_targets', 'event', 'event_history', 'search_criteria_history', 'find_search', 'find_search_by_token', 'find_company_by_domain', 'find_actor_by_email', 'find_event_by_id', 'update_company', 'update_search', 'mute_event', 'delete_comment', 'reset_inbox')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201080108010c010c011002080108010c010c02140208010c010c
       011c021406101e240e100f1010244d020102fb04010eff020202fe020302
       fd020402fc020502fb020602fa086016211c2d060c16290617160e163e0c
-      7f00041a0c1a21241d2409101010101013101d10171017100b
+      7f00041a0c1a1e1a1d241d2409101010101013101d10171017100b
```

### Comparing `gandai-1.7.35/gandai/__pycache__/secrets.cpython-311.pyc` & `gandai-1.7.40/gandai/__pycache__/secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.7.40/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.7.40/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/__pycache__/tasks.cpython-311.pyc` & `gandai-1.7.40/gandai/__pycache__/tasks.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/analytics.py` & `gandai-1.7.40/gandai/analytics.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/constants.py` & `gandai-1.7.40/gandai/constants.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/db.py` & `gandai-1.7.40/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/google.py` & `gandai-1.7.40/gandai/google.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/gpt.py` & `gandai-1.7.40/gandai/gpt.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/grata.py` & `gandai-1.7.40/gandai/grata.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/main.py` & `gandai-1.7.40/gandai/main.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.7.40/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/migrations/db_seed.py` & `gandai-1.7.40/gandai/migrations/db_seed.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/migrations/dealcloud.py` & `gandai-1.7.40/gandai/migrations/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/migrations/sql/230818-alter.sql` & `gandai-1.7.40/gandai/migrations/sql/230818-alter.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/migrations/sql/schema.sql` & `gandai-1.7.40/gandai/migrations/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/models.py` & `gandai-1.7.40/gandai/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,15 +163,10 @@
 
     @property
     def customers(self) -> str:
         # as csv
         return self.meta.get("customers", None)
 
     @property
-    def was_acquired(self) -> str:
-        # starts with Yes, or No,
-        return self.meta.get("was_acquired", None)
-
-    @property
     def token(self) -> str:
         # Create an MD5 hash of the uid converted to string
         return hashlib.md5(str(self.uid).encode("utf-8")).hexdigest()
```

### Comparing `gandai-1.7.35/gandai/query.py` & `gandai-1.7.40/gandai/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -665,14 +665,40 @@
     """
     with db.connect() as conn:
         result = conn.execute(sqlalchemy.text(statement), {"search_uid": search_uid})
         df = pd.DataFrame(result.fetchall(), columns=result.keys())
     return df
 
 
+def search_criteria_history(search_uid: int) -> pd.DataFrame:
+
+    statement = """
+    SELECT 
+        e.type as event_type,
+        s.label as search_label,
+        e.search_uid,
+        e.data,
+        -- a.type as actor_type,
+        a.name,
+        to_timestamp(e.created) as created 
+    FROM event e
+    JOIN actor a on e.actor_key = a.key
+    JOIN search s on e.search_uid = s.uid
+    WHERE 
+        e.search_uid = :search_uid
+        AND e.type in ('import', 'criteria','google','google_maps')
+    ORDER BY created DESC
+    ;
+    """
+    with db.connect() as conn:
+        result = conn.execute(sqlalchemy.text(statement), {"search_uid": search_uid})
+        df = pd.DataFrame(result.fetchall(), columns=result.keys())
+    return df
+
+
 ### FINDERS -> dataclass ###
 
 
 def find_search(uid: int) -> ts.models.Search:
     with db.connect() as conn:
         statement = """
             SELECT
```

### Comparing `gandai-1.7.35/gandai/secrets.py` & `gandai-1.7.40/gandai/secrets.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai/tasks.py` & `gandai-1.7.40/gandai/tasks.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.35/gandai.egg-info/SOURCES.txt` & `gandai-1.7.40/gandai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

