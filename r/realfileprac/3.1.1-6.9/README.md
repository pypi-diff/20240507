# Comparing `tmp/realfileprac-3.1.1.tar.gz` & `tmp/realfileprac-6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "realfileprac-3.1.1.tar", last modified: Tue May  7 19:02:57 2024, max compression
+gzip compressed data, was "realfileprac-6.9.tar", last modified: Tue May  7 19:39:03 2024, max compression
```

## Comparing `realfileprac-3.1.1.tar` & `realfileprac-6.9.tar`

### file list

```diff
@@ -1,13 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 19:02:57.892071 realfileprac-3.1.1/
--rw-rw-rw-   0        0        0      207 2024-05-07 19:02:57.892071 realfileprac-3.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-07 19:02:57.880054 realfileprac-3.1.1/realfileprac/
--rw-rw-rw-   0        0        0        0 2024-05-07 18:37:10.000000 realfileprac-3.1.1/realfileprac/__init__.py
--rw-rw-rw-   0        0        0     1758 2024-05-07 18:23:04.000000 realfileprac-3.1.1/realfileprac/dsassi1.py
--rw-rw-rw-   0        0        0     1691 2024-05-07 18:57:40.000000 realfileprac-3.1.1/realfileprac/dsassi5.py
-drwxrwxrwx   0        0        0        0 2024-05-07 19:02:57.892071 realfileprac-3.1.1/realfileprac.egg-info/
--rw-rw-rw-   0        0        0      207 2024-05-07 19:02:57.000000 realfileprac-3.1.1/realfileprac.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2024-05-07 19:02:57.000000 realfileprac-3.1.1/realfileprac.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 19:02:57.000000 realfileprac-3.1.1/realfileprac.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-07 19:02:57.000000 realfileprac-3.1.1/realfileprac.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 19:02:57.892071 realfileprac-3.1.1/setup.cfg
--rw-rw-rw-   0        0        0      307 2024-05-07 19:02:48.000000 realfileprac-3.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 19:39:03.057130 realfileprac-6.9/
+-rw-rw-rw-   0        0        0      205 2024-05-07 19:39:03.057130 realfileprac-6.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-07 19:39:03.009815 realfileprac-6.9/realfileprac/
+-rw-rw-rw-   0        0        0        0 2024-05-07 18:37:10.000000 realfileprac-6.9/realfileprac/__init__.py
+-rw-rw-rw-   0        0        0     1946 2024-05-07 19:18:35.000000 realfileprac-6.9/realfileprac/ds_assi_6.py
+-rw-rw-rw-   0        0        0     1758 2024-05-07 18:23:04.000000 realfileprac-6.9/realfileprac/dsassi1.py
+-rw-rw-rw-   0        0        0     1739 2024-05-07 19:29:48.000000 realfileprac-6.9/realfileprac/dsassi10.py
+-rw-rw-rw-   0        0        0     1237 2024-05-07 19:33:32.000000 realfileprac-6.9/realfileprac/dsassi2.py
+-rw-rw-rw-   0        0        0      965 2024-05-07 19:38:17.000000 realfileprac-6.9/realfileprac/dsassi3.py
+-rw-rw-rw-   0        0        0     1020 2024-05-07 19:08:05.000000 realfileprac-6.9/realfileprac/dsassi4.py
+-rw-rw-rw-   0        0        0     1691 2024-05-07 18:57:40.000000 realfileprac-6.9/realfileprac/dsassi5.py
+-rw-rw-rw-   0        0        0     1946 2024-05-07 19:18:57.000000 realfileprac-6.9/realfileprac/dsassi6.py
+-rw-rw-rw-   0        0        0     1672 2024-05-07 19:23:24.000000 realfileprac-6.9/realfileprac/dsassi7.py
+-rw-rw-rw-   0        0        0     1589 2024-05-07 19:31:20.000000 realfileprac-6.9/realfileprac/dsassi8.py
+-rw-rw-rw-   0        0        0     1452 2024-05-07 19:28:28.000000 realfileprac-6.9/realfileprac/dsassi9.py
+-rw-rw-rw-   0        0        0     2659 2024-05-07 19:35:14.000000 realfileprac-6.9/realfileprac/spark.py
+drwxrwxrwx   0        0        0        0 2024-05-07 19:39:03.057130 realfileprac-6.9/realfileprac.egg-info/
+-rw-rw-rw-   0        0        0      205 2024-05-07 19:39:02.000000 realfileprac-6.9/realfileprac.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2024-05-07 19:39:02.000000 realfileprac-6.9/realfileprac.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 19:39:02.000000 realfileprac-6.9/realfileprac.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-07 19:39:02.000000 realfileprac-6.9/realfileprac.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 19:39:03.057130 realfileprac-6.9/setup.cfg
+-rw-rw-rw-   0        0        0      305 2024-05-07 19:35:36.000000 realfileprac-6.9/setup.py
```

### Comparing `realfileprac-3.1.1/realfileprac/dsassi1.py` & `realfileprac-6.9/realfileprac/dsassi1.py`

 * *Files identical despite different names*

### Comparing `realfileprac-3.1.1/realfileprac/dsassi5.py` & `realfileprac-6.9/realfileprac/dsassi5.py`

 * *Files identical despite different names*

