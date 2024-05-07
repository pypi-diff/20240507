# Comparing `tmp/realfileprac-3.1.tar.gz` & `tmp/realfileprac-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "realfileprac-3.1.tar", last modified: Tue May  7 18:38:23 2024, max compression
+gzip compressed data, was "realfileprac-3.1.1.tar", last modified: Tue May  7 19:02:57 2024, max compression
```

## Comparing `realfileprac-3.1.tar` & `realfileprac-3.1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 18:38:23.889961 realfileprac-3.1/
--rw-rw-rw-   0        0        0      205 2024-05-07 18:38:23.889961 realfileprac-3.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-07 18:38:23.858679 realfileprac-3.1/realfileprac/
--rw-rw-rw-   0        0        0        0 2024-05-07 18:37:10.000000 realfileprac-3.1/realfileprac/__init__.py
--rw-rw-rw-   0        0        0     1758 2024-05-07 18:23:04.000000 realfileprac-3.1/realfileprac/dsassi1.py
-drwxrwxrwx   0        0        0        0 2024-05-07 18:38:23.889961 realfileprac-3.1/realfileprac.egg-info/
--rw-rw-rw-   0        0        0      205 2024-05-07 18:38:23.000000 realfileprac-3.1/realfileprac.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-05-07 18:38:23.000000 realfileprac-3.1/realfileprac.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 18:38:23.000000 realfileprac-3.1/realfileprac.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-07 18:38:23.000000 realfileprac-3.1/realfileprac.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 18:38:23.889961 realfileprac-3.1/setup.cfg
--rw-rw-rw-   0        0        0      305 2024-05-07 18:28:11.000000 realfileprac-3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 19:02:57.892071 realfileprac-3.1.1/
+-rw-rw-rw-   0        0        0      207 2024-05-07 19:02:57.892071 realfileprac-3.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-07 19:02:57.880054 realfileprac-3.1.1/realfileprac/
+-rw-rw-rw-   0        0        0        0 2024-05-07 18:37:10.000000 realfileprac-3.1.1/realfileprac/__init__.py
+-rw-rw-rw-   0        0        0     1758 2024-05-07 18:23:04.000000 realfileprac-3.1.1/realfileprac/dsassi1.py
+-rw-rw-rw-   0        0        0     1691 2024-05-07 18:57:40.000000 realfileprac-3.1.1/realfileprac/dsassi5.py
+drwxrwxrwx   0        0        0        0 2024-05-07 19:02:57.892071 realfileprac-3.1.1/realfileprac.egg-info/
+-rw-rw-rw-   0        0        0      207 2024-05-07 19:02:57.000000 realfileprac-3.1.1/realfileprac.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-05-07 19:02:57.000000 realfileprac-3.1.1/realfileprac.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 19:02:57.000000 realfileprac-3.1.1/realfileprac.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-07 19:02:57.000000 realfileprac-3.1.1/realfileprac.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 19:02:57.892071 realfileprac-3.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      307 2024-05-07 19:02:48.000000 realfileprac-3.1.1/setup.py
```

### Comparing `realfileprac-3.1/realfileprac/dsassi1.py` & `realfileprac-3.1.1/realfileprac/dsassi1.py`

 * *Files identical despite different names*

