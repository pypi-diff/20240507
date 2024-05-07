# Comparing `tmp/wauo-0.1.tar.gz` & `tmp/wauo-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wauo-0.1.tar", last modified: Tue May  7 12:15:51 2024, max compression
+gzip compressed data, was "wauo-0.2.tar", last modified: Tue May  7 12:46:24 2024, max compression
```

## Comparing `wauo-0.1.tar` & `wauo-0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-07 12:15:51.654202 wauo-0.1/
--rw-r--r--   0 wangtuo    (501) staff       (20)      176 2024-05-07 12:15:51.654062 wauo-0.1/PKG-INFO
--rw-r--r--   0 wangtuo    (501) staff       (20)       38 2024-05-07 12:15:51.654246 wauo-0.1/setup.cfg
--rw-r--r--   0 wangtuo    (501) staff       (20)      294 2024-05-07 12:13:15.000000 wauo-0.1/setup.py
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-07 12:15:51.653076 wauo-0.1/wauo/
--rw-r--r--   0 wangtuo    (501) staff       (20)       95 2024-05-03 02:43:04.000000 wauo-0.1/wauo/__init__.py
--rw-r--r--   0 wangtuo    (501) staff       (20)      345 2023-11-08 06:17:07.000000 wauo-0.1/wauo/exceptions.py
--rw-r--r--   0 wangtuo    (501) staff       (20)      789 2024-05-03 11:40:02.000000 wauo-0.1/wauo/response.py
--rw-r--r--   0 wangtuo    (501) staff       (20)     4733 2024-05-03 14:42:18.000000 wauo-0.1/wauo/spiders.py
--rw-r--r--   0 wangtuo    (501) staff       (20)      351 2024-05-03 14:44:50.000000 wauo-0.1/wauo/test.py
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-07 12:15:51.653917 wauo-0.1/wauo.egg-info/
--rw-r--r--   0 wangtuo    (501) staff       (20)      176 2024-05-07 12:15:51.000000 wauo-0.1/wauo.egg-info/PKG-INFO
--rw-r--r--   0 wangtuo    (501) staff       (20)      229 2024-05-07 12:15:51.000000 wauo-0.1/wauo.egg-info/SOURCES.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-07 12:15:51.000000 wauo-0.1/wauo.egg-info/dependency_links.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-07 12:13:42.000000 wauo-0.1/wauo.egg-info/not-zip-safe
--rw-r--r--   0 wangtuo    (501) staff       (20)        5 2024-05-07 12:15:51.000000 wauo-0.1/wauo.egg-info/top_level.txt
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-07 12:46:24.016098 wauo-0.2/
+-rw-r--r--   0 wangtuo    (501) staff       (20)      230 2024-05-07 12:46:24.015866 wauo-0.2/PKG-INFO
+-rw-r--r--   0 wangtuo    (501) staff       (20)       38 2024-05-07 12:46:24.016133 wauo-0.2/setup.cfg
+-rw-r--r--   0 wangtuo    (501) staff       (20)      434 2024-05-07 12:43:34.000000 wauo-0.2/setup.py
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-07 12:46:24.014749 wauo-0.2/wauo/
+-rw-r--r--   0 wangtuo    (501) staff       (20)       95 2024-05-03 02:43:04.000000 wauo-0.2/wauo/__init__.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)      345 2023-11-08 06:17:07.000000 wauo-0.2/wauo/exceptions.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)      789 2024-05-03 11:40:02.000000 wauo-0.2/wauo/response.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)     4733 2024-05-03 14:42:18.000000 wauo-0.2/wauo/spiders.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)      351 2024-05-03 14:44:50.000000 wauo-0.2/wauo/test.py
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-07 12:46:24.015706 wauo-0.2/wauo.egg-info/
+-rw-r--r--   0 wangtuo    (501) staff       (20)      230 2024-05-07 12:46:23.000000 wauo-0.2/wauo.egg-info/PKG-INFO
+-rw-r--r--   0 wangtuo    (501) staff       (20)      256 2024-05-07 12:46:23.000000 wauo-0.2/wauo.egg-info/SOURCES.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-07 12:46:23.000000 wauo-0.2/wauo.egg-info/dependency_links.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-07 12:46:23.000000 wauo-0.2/wauo.egg-info/not-zip-safe
+-rw-r--r--   0 wangtuo    (501) staff       (20)       31 2024-05-07 12:46:23.000000 wauo-0.2/wauo.egg-info/requires.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        5 2024-05-07 12:46:23.000000 wauo-0.2/wauo.egg-info/top_level.txt
```

### Comparing `wauo-0.1/wauo/response.py` & `wauo-0.2/wauo/response.py`

 * *Files identical despite different names*

### Comparing `wauo-0.1/wauo/spiders.py` & `wauo-0.2/wauo/spiders.py`

 * *Files identical despite different names*

