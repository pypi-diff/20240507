# Comparing `tmp/my_decimal-0.1.1.tar.gz` & `tmp/my_decimal-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_decimal-0.1.1.tar", last modified: Mon May  6 17:19:46 2024, max compression
+gzip compressed data, was "my_decimal-1.1.2.tar", last modified: Tue May  7 14:47:37 2024, max compression
```

## Comparing `my_decimal-0.1.1.tar` & `my_decimal-1.1.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 17:19:46.384568 my_decimal-0.1.1/
--rw-rw-rw-   0        0        0     1088 2024-05-05 23:21:12.000000 my_decimal-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      249 2024-05-06 17:19:46.383569 my_decimal-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-06 17:19:46.383569 my_decimal-0.1.1/my_decimal.egg-info/
--rw-rw-rw-   0        0        0      249 2024-05-06 17:19:46.000000 my_decimal-0.1.1/my_decimal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      166 2024-05-06 17:19:46.000000 my_decimal-0.1.1/my_decimal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 17:19:46.000000 my_decimal-0.1.1/my_decimal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-06 17:19:46.000000 my_decimal-0.1.1/my_decimal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       61 2024-05-06 17:10:58.000000 my_decimal-0.1.1/my_decimal.py
--rw-rw-rw-   0        0        0       42 2024-05-06 17:19:46.384568 my_decimal-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      318 2024-05-06 17:10:58.000000 my_decimal-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 14:47:37.988832 my_decimal-1.1.2/
+-rw-rw-rw-   0        0        0     1088 2024-05-05 23:21:12.000000 my_decimal-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2092 2024-05-07 14:47:37.988832 my_decimal-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1853 2024-05-07 14:45:46.000000 my_decimal-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 14:47:37.987831 my_decimal-1.1.2/my_decimal.egg-info/
+-rw-rw-rw-   0        0        0     2092 2024-05-07 14:47:37.000000 my_decimal-1.1.2/my_decimal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2024-05-07 14:47:37.000000 my_decimal-1.1.2/my_decimal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 14:47:37.000000 my_decimal-1.1.2/my_decimal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-07 14:47:37.000000 my_decimal-1.1.2/my_decimal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       61 2024-05-06 17:10:58.000000 my_decimal-1.1.2/my_decimal.py
+-rw-rw-rw-   0        0        0       42 2024-05-07 14:47:37.989831 my_decimal-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      381 2024-05-07 14:47:34.000000 my_decimal-1.1.2/setup.py
```

### Comparing `my_decimal-0.1.1/LICENSE` & `my_decimal-1.1.2/LICENSE`

 * *Files identical despite different names*

