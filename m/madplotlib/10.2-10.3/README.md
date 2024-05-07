# Comparing `tmp/madplotlib-10.2.tar.gz` & `tmp/madplotlib-10.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "madplotlib-10.2.tar", last modified: Tue May  7 19:55:32 2024, max compression
+gzip compressed data, was "madplotlib-10.3.tar", last modified: Tue May  7 19:55:55 2024, max compression
```

## Comparing `madplotlib-10.2.tar` & `madplotlib-10.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 19:55:32.193740 madplotlib-10.2/
--rw-rw-rw-   0        0        0      204 2024-05-07 19:55:32.193740 madplotlib-10.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-07 19:55:32.178101 madplotlib-10.2/madplotlib.egg-info/
--rw-rw-rw-   0        0        0      204 2024-05-07 19:55:31.000000 madplotlib-10.2/madplotlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      458 2024-05-07 19:55:31.000000 madplotlib-10.2/madplotlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 19:55:31.000000 madplotlib-10.2/madplotlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-07 19:55:31.000000 madplotlib-10.2/madplotlib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-07 19:55:32.178101 madplotlib-10.2/realfileprac/
--rw-rw-rw-   0        0        0        0 2024-05-07 18:37:10.000000 madplotlib-10.2/realfileprac/__init__.py
--rw-rw-rw-   0        0        0     1946 2024-05-07 19:18:35.000000 madplotlib-10.2/realfileprac/ds_assi_6.py
--rw-rw-rw-   0        0        0     1758 2024-05-07 18:23:04.000000 madplotlib-10.2/realfileprac/dsassi1.py
--rw-rw-rw-   0        0        0     1739 2024-05-07 19:29:48.000000 madplotlib-10.2/realfileprac/dsassi10.py
--rw-rw-rw-   0        0        0     1237 2024-05-07 19:33:32.000000 madplotlib-10.2/realfileprac/dsassi2.py
--rw-rw-rw-   0        0        0      965 2024-05-07 19:38:17.000000 madplotlib-10.2/realfileprac/dsassi3.py
--rw-rw-rw-   0        0        0     1020 2024-05-07 19:08:05.000000 madplotlib-10.2/realfileprac/dsassi4.py
--rw-rw-rw-   0        0        0     1691 2024-05-07 18:57:40.000000 madplotlib-10.2/realfileprac/dsassi5.py
--rw-rw-rw-   0        0        0     1946 2024-05-07 19:18:57.000000 madplotlib-10.2/realfileprac/dsassi6.py
--rw-rw-rw-   0        0        0     1672 2024-05-07 19:23:24.000000 madplotlib-10.2/realfileprac/dsassi7.py
--rw-rw-rw-   0        0        0     1589 2024-05-07 19:31:20.000000 madplotlib-10.2/realfileprac/dsassi8.py
--rw-rw-rw-   0        0        0     1452 2024-05-07 19:28:28.000000 madplotlib-10.2/realfileprac/dsassi9.py
--rw-rw-rw-   0        0        0     2659 2024-05-07 19:35:14.000000 madplotlib-10.2/realfileprac/spark.py
--rw-rw-rw-   0        0        0       42 2024-05-07 19:55:32.193740 madplotlib-10.2/setup.cfg
--rw-rw-rw-   0        0        0      304 2024-05-07 19:55:27.000000 madplotlib-10.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 19:55:55.209833 madplotlib-10.3/
+-rw-rw-rw-   0        0        0      204 2024-05-07 19:55:55.209833 madplotlib-10.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-07 19:55:55.209833 madplotlib-10.3/madplotlib.egg-info/
+-rw-rw-rw-   0        0        0      204 2024-05-07 19:55:54.000000 madplotlib-10.3/madplotlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      458 2024-05-07 19:55:54.000000 madplotlib-10.3/madplotlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 19:55:54.000000 madplotlib-10.3/madplotlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-07 19:55:54.000000 madplotlib-10.3/madplotlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 19:55:55.194205 madplotlib-10.3/realfileprac/
+-rw-rw-rw-   0        0        0        0 2024-05-07 18:37:10.000000 madplotlib-10.3/realfileprac/__init__.py
+-rw-rw-rw-   0        0        0     1946 2024-05-07 19:18:35.000000 madplotlib-10.3/realfileprac/ds_assi_6.py
+-rw-rw-rw-   0        0        0     1758 2024-05-07 18:23:04.000000 madplotlib-10.3/realfileprac/dsassi1.py
+-rw-rw-rw-   0        0        0     1739 2024-05-07 19:29:48.000000 madplotlib-10.3/realfileprac/dsassi10.py
+-rw-rw-rw-   0        0        0     1237 2024-05-07 19:33:32.000000 madplotlib-10.3/realfileprac/dsassi2.py
+-rw-rw-rw-   0        0        0      965 2024-05-07 19:38:17.000000 madplotlib-10.3/realfileprac/dsassi3.py
+-rw-rw-rw-   0        0        0     1020 2024-05-07 19:08:05.000000 madplotlib-10.3/realfileprac/dsassi4.py
+-rw-rw-rw-   0        0        0     1691 2024-05-07 18:57:40.000000 madplotlib-10.3/realfileprac/dsassi5.py
+-rw-rw-rw-   0        0        0     1946 2024-05-07 19:18:57.000000 madplotlib-10.3/realfileprac/dsassi6.py
+-rw-rw-rw-   0        0        0     1672 2024-05-07 19:23:24.000000 madplotlib-10.3/realfileprac/dsassi7.py
+-rw-rw-rw-   0        0        0     1589 2024-05-07 19:31:20.000000 madplotlib-10.3/realfileprac/dsassi8.py
+-rw-rw-rw-   0        0        0     1452 2024-05-07 19:28:28.000000 madplotlib-10.3/realfileprac/dsassi9.py
+-rw-rw-rw-   0        0        0     2659 2024-05-07 19:35:14.000000 madplotlib-10.3/realfileprac/spark.py
+-rw-rw-rw-   0        0        0       42 2024-05-07 19:55:55.209833 madplotlib-10.3/setup.cfg
+-rw-rw-rw-   0        0        0      304 2024-05-07 19:55:51.000000 madplotlib-10.3/setup.py
```

### Comparing `madplotlib-10.2/realfileprac/ds_assi_6.py` & `madplotlib-10.3/realfileprac/ds_assi_6.py`

 * *Files identical despite different names*

### Comparing `madplotlib-10.2/realfileprac/dsassi1.py` & `madplotlib-10.3/realfileprac/dsassi1.py`

 * *Files identical despite different names*

### Comparing `madplotlib-10.2/realfileprac/dsassi10.py` & `madplotlib-10.3/realfileprac/dsassi10.py`

 * *Files identical despite different names*

### Comparing `madplotlib-10.2/realfileprac/dsassi2.py` & `madplotlib-10.3/realfileprac/dsassi2.py`

 * *Files identical despite different names*

### Comparing `madplotlib-10.2/realfileprac/dsassi3.py` & `madplotlib-10.3/realfileprac/dsassi3.py`

 * *Files identical despite different names*

### Comparing `madplotlib-10.2/realfileprac/dsassi4.py` & `madplotlib-10.3/realfileprac/dsassi4.py`

 * *Files identical despite different names*

### Comparing `madplotlib-10.2/realfileprac/dsassi5.py` & `madplotlib-10.3/realfileprac/dsassi5.py`

 * *Files identical despite different names*

### Comparing `madplotlib-10.2/realfileprac/dsassi6.py` & `madplotlib-10.3/realfileprac/dsassi6.py`

 * *Files identical despite different names*

### Comparing `madplotlib-10.2/realfileprac/dsassi7.py` & `madplotlib-10.3/realfileprac/dsassi7.py`

 * *Files identical despite different names*

### Comparing `madplotlib-10.2/realfileprac/dsassi8.py` & `madplotlib-10.3/realfileprac/dsassi8.py`

 * *Files identical despite different names*

### Comparing `madplotlib-10.2/realfileprac/dsassi9.py` & `madplotlib-10.3/realfileprac/dsassi9.py`

 * *Files identical despite different names*

### Comparing `madplotlib-10.2/realfileprac/spark.py` & `madplotlib-10.3/realfileprac/spark.py`

 * *Files identical despite different names*

