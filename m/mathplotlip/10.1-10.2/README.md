# Comparing `tmp/mathplotlip-10.1.tar.gz` & `tmp/mathplotlip-10.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathplotlip-10.1.tar", last modified: Tue May  7 19:45:20 2024, max compression
+gzip compressed data, was "mathplotlip-10.2.tar", last modified: Tue May  7 19:45:40 2024, max compression
```

## Comparing `mathplotlip-10.1.tar` & `mathplotlip-10.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 19:45:20.363005 mathplotlip-10.1/
--rw-rw-rw-   0        0        0      205 2024-05-07 19:45:20.363005 mathplotlip-10.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-07 19:45:20.363005 mathplotlip-10.1/mathplotlip.egg-info/
--rw-rw-rw-   0        0        0      205 2024-05-07 19:45:20.000000 mathplotlip-10.1/mathplotlip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      462 2024-05-07 19:45:20.000000 mathplotlip-10.1/mathplotlip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 19:45:20.000000 mathplotlip-10.1/mathplotlip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-07 19:45:20.000000 mathplotlip-10.1/mathplotlip.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-07 19:45:20.363005 mathplotlip-10.1/realfileprac/
--rw-rw-rw-   0        0        0        0 2024-05-07 18:37:10.000000 mathplotlip-10.1/realfileprac/__init__.py
--rw-rw-rw-   0        0        0     1946 2024-05-07 19:18:35.000000 mathplotlip-10.1/realfileprac/ds_assi_6.py
--rw-rw-rw-   0        0        0     1758 2024-05-07 18:23:04.000000 mathplotlip-10.1/realfileprac/dsassi1.py
--rw-rw-rw-   0        0        0     1739 2024-05-07 19:29:48.000000 mathplotlip-10.1/realfileprac/dsassi10.py
--rw-rw-rw-   0        0        0     1237 2024-05-07 19:33:32.000000 mathplotlip-10.1/realfileprac/dsassi2.py
--rw-rw-rw-   0        0        0      965 2024-05-07 19:38:17.000000 mathplotlip-10.1/realfileprac/dsassi3.py
--rw-rw-rw-   0        0        0     1020 2024-05-07 19:08:05.000000 mathplotlip-10.1/realfileprac/dsassi4.py
--rw-rw-rw-   0        0        0     1691 2024-05-07 18:57:40.000000 mathplotlip-10.1/realfileprac/dsassi5.py
--rw-rw-rw-   0        0        0     1946 2024-05-07 19:18:57.000000 mathplotlip-10.1/realfileprac/dsassi6.py
--rw-rw-rw-   0        0        0     1672 2024-05-07 19:23:24.000000 mathplotlip-10.1/realfileprac/dsassi7.py
--rw-rw-rw-   0        0        0     1589 2024-05-07 19:31:20.000000 mathplotlip-10.1/realfileprac/dsassi8.py
--rw-rw-rw-   0        0        0     1452 2024-05-07 19:28:28.000000 mathplotlip-10.1/realfileprac/dsassi9.py
--rw-rw-rw-   0        0        0     2659 2024-05-07 19:35:14.000000 mathplotlip-10.1/realfileprac/spark.py
--rw-rw-rw-   0        0        0       42 2024-05-07 19:45:20.378676 mathplotlip-10.1/setup.cfg
--rw-rw-rw-   0        0        0      305 2024-05-07 19:45:15.000000 mathplotlip-10.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 19:45:40.872146 mathplotlip-10.2/
+-rw-rw-rw-   0        0        0      205 2024-05-07 19:45:40.872146 mathplotlip-10.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-07 19:45:40.872146 mathplotlip-10.2/mathplotlip.egg-info/
+-rw-rw-rw-   0        0        0      205 2024-05-07 19:45:40.000000 mathplotlip-10.2/mathplotlip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      462 2024-05-07 19:45:40.000000 mathplotlip-10.2/mathplotlip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 19:45:40.000000 mathplotlip-10.2/mathplotlip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-07 19:45:40.000000 mathplotlip-10.2/mathplotlip.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 19:45:40.872146 mathplotlip-10.2/realfileprac/
+-rw-rw-rw-   0        0        0        0 2024-05-07 18:37:10.000000 mathplotlip-10.2/realfileprac/__init__.py
+-rw-rw-rw-   0        0        0     1946 2024-05-07 19:18:35.000000 mathplotlip-10.2/realfileprac/ds_assi_6.py
+-rw-rw-rw-   0        0        0     1758 2024-05-07 18:23:04.000000 mathplotlip-10.2/realfileprac/dsassi1.py
+-rw-rw-rw-   0        0        0     1739 2024-05-07 19:29:48.000000 mathplotlip-10.2/realfileprac/dsassi10.py
+-rw-rw-rw-   0        0        0     1237 2024-05-07 19:33:32.000000 mathplotlip-10.2/realfileprac/dsassi2.py
+-rw-rw-rw-   0        0        0      965 2024-05-07 19:38:17.000000 mathplotlip-10.2/realfileprac/dsassi3.py
+-rw-rw-rw-   0        0        0     1020 2024-05-07 19:08:05.000000 mathplotlip-10.2/realfileprac/dsassi4.py
+-rw-rw-rw-   0        0        0     1691 2024-05-07 18:57:40.000000 mathplotlip-10.2/realfileprac/dsassi5.py
+-rw-rw-rw-   0        0        0     1946 2024-05-07 19:18:57.000000 mathplotlip-10.2/realfileprac/dsassi6.py
+-rw-rw-rw-   0        0        0     1672 2024-05-07 19:23:24.000000 mathplotlip-10.2/realfileprac/dsassi7.py
+-rw-rw-rw-   0        0        0     1589 2024-05-07 19:31:20.000000 mathplotlip-10.2/realfileprac/dsassi8.py
+-rw-rw-rw-   0        0        0     1452 2024-05-07 19:28:28.000000 mathplotlip-10.2/realfileprac/dsassi9.py
+-rw-rw-rw-   0        0        0     2659 2024-05-07 19:35:14.000000 mathplotlip-10.2/realfileprac/spark.py
+-rw-rw-rw-   0        0        0       42 2024-05-07 19:45:40.887800 mathplotlip-10.2/setup.cfg
+-rw-rw-rw-   0        0        0      305 2024-05-07 19:45:38.000000 mathplotlip-10.2/setup.py
```

### Comparing `mathplotlip-10.1/realfileprac/ds_assi_6.py` & `mathplotlip-10.2/realfileprac/ds_assi_6.py`

 * *Files identical despite different names*

### Comparing `mathplotlip-10.1/realfileprac/dsassi1.py` & `mathplotlip-10.2/realfileprac/dsassi1.py`

 * *Files identical despite different names*

### Comparing `mathplotlip-10.1/realfileprac/dsassi10.py` & `mathplotlip-10.2/realfileprac/dsassi10.py`

 * *Files identical despite different names*

### Comparing `mathplotlip-10.1/realfileprac/dsassi2.py` & `mathplotlip-10.2/realfileprac/dsassi2.py`

 * *Files identical despite different names*

### Comparing `mathplotlip-10.1/realfileprac/dsassi3.py` & `mathplotlip-10.2/realfileprac/dsassi3.py`

 * *Files identical despite different names*

### Comparing `mathplotlip-10.1/realfileprac/dsassi4.py` & `mathplotlip-10.2/realfileprac/dsassi4.py`

 * *Files identical despite different names*

### Comparing `mathplotlip-10.1/realfileprac/dsassi5.py` & `mathplotlip-10.2/realfileprac/dsassi5.py`

 * *Files identical despite different names*

### Comparing `mathplotlip-10.1/realfileprac/dsassi6.py` & `mathplotlip-10.2/realfileprac/dsassi6.py`

 * *Files identical despite different names*

### Comparing `mathplotlip-10.1/realfileprac/dsassi7.py` & `mathplotlip-10.2/realfileprac/dsassi7.py`

 * *Files identical despite different names*

### Comparing `mathplotlip-10.1/realfileprac/dsassi8.py` & `mathplotlip-10.2/realfileprac/dsassi8.py`

 * *Files identical despite different names*

### Comparing `mathplotlip-10.1/realfileprac/dsassi9.py` & `mathplotlip-10.2/realfileprac/dsassi9.py`

 * *Files identical despite different names*

### Comparing `mathplotlip-10.1/realfileprac/spark.py` & `mathplotlip-10.2/realfileprac/spark.py`

 * *Files identical despite different names*

