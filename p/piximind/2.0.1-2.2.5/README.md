# Comparing `tmp/piximind-2.0.1.tar.gz` & `tmp/piximind-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piximind-2.0.1.tar", last modified: Tue May  7 11:24:10 2024, max compression
+gzip compressed data, was "piximind-2.2.5.tar", last modified: Tue May  7 15:52:44 2024, max compression
```

## Comparing `piximind-2.0.1.tar` & `piximind-2.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 11:24:10.947424 piximind-2.0.1/
--rw-rw-rw-   0        0        0     1088 2024-05-07 11:15:35.000000 piximind-2.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      227 2024-05-07 11:24:10.945338 piximind-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       54 2024-05-07 11:14:28.000000 piximind-2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 11:24:10.902743 piximind-2.0.1/piximind/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:20:47.000000 piximind-2.0.1/piximind/__init__.py
--rw-rw-rw-   0        0        0       68 2024-05-07 11:23:12.000000 piximind-2.0.1/piximind/princo.py
-drwxrwxrwx   0        0        0        0 2024-05-07 11:24:10.943342 piximind-2.0.1/piximind.egg-info/
--rw-rw-rw-   0        0        0      227 2024-05-07 11:24:10.000000 piximind-2.0.1/piximind.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2024-05-07 11:24:10.000000 piximind-2.0.1/piximind.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 11:24:10.000000 piximind-2.0.1/piximind.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-07 11:24:10.000000 piximind-2.0.1/piximind.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 11:24:10.947424 piximind-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      509 2024-05-07 11:20:50.000000 piximind-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:52:44.813480 piximind-2.2.5/
+-rw-rw-rw-   0        0        0     1088 2024-05-07 11:15:35.000000 piximind-2.2.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      227 2024-05-07 15:52:44.811993 piximind-2.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       54 2024-05-07 11:14:28.000000 piximind-2.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 15:52:44.784660 piximind-2.2.5/piximind/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:20:47.000000 piximind-2.2.5/piximind/__init__.py
+-rw-rw-rw-   0        0        0      780 2024-05-07 15:50:23.000000 piximind-2.2.5/piximind/princo.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:52:44.809080 piximind-2.2.5/piximind.egg-info/
+-rw-rw-rw-   0        0        0      227 2024-05-07 15:52:44.000000 piximind-2.2.5/piximind.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2024-05-07 15:52:44.000000 piximind-2.2.5/piximind.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 15:52:44.000000 piximind-2.2.5/piximind.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-07 15:52:44.000000 piximind-2.2.5/piximind.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 15:52:44.814487 piximind-2.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      509 2024-05-07 15:50:47.000000 piximind-2.2.5/setup.py
```

### Comparing `piximind-2.0.1/LICENSE.txt` & `piximind-2.2.5/LICENSE.txt`

 * *Files identical despite different names*

