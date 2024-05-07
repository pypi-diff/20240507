# Comparing `tmp/myswiki-1.0.1.tar.gz` & `tmp/myswiki-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myswiki-1.0.1.tar", last modified: Tue May  7 09:04:58 2024, max compression
+gzip compressed data, was "myswiki-1.0.2.tar", last modified: Tue May  7 14:10:10 2024, max compression
```

## Comparing `myswiki-1.0.1.tar` & `myswiki-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 09:04:58.060536 myswiki-1.0.1/
--rw-rw-rw-   0        0        0     1088 2024-05-07 08:54:42.000000 myswiki-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      191 2024-05-07 09:04:58.059536 myswiki-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-07 09:04:58.058535 myswiki-1.0.1/myswiki.egg-info/
--rw-rw-rw-   0        0        0      191 2024-05-07 09:04:57.000000 myswiki-1.0.1/myswiki.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      151 2024-05-07 09:04:58.000000 myswiki-1.0.1/myswiki.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 09:04:57.000000 myswiki-1.0.1/myswiki.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-07 09:04:57.000000 myswiki-1.0.1/myswiki.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4281 2024-05-07 09:04:53.000000 myswiki-1.0.1/myswiki.py
--rw-rw-rw-   0        0        0       42 2024-05-07 09:04:58.060536 myswiki-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      257 2024-05-07 09:04:53.000000 myswiki-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 14:10:10.795763 myswiki-1.0.2/
+-rw-rw-rw-   0        0        0     1088 2024-05-07 08:54:42.000000 myswiki-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2161 2024-05-07 14:10:10.794762 myswiki-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1890 2024-05-07 14:03:42.000000 myswiki-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 14:10:10.794762 myswiki-1.0.2/myswiki.egg-info/
+-rw-rw-rw-   0        0        0     2161 2024-05-07 14:10:10.000000 myswiki-1.0.2/myswiki.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2024-05-07 14:10:10.000000 myswiki-1.0.2/myswiki.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 14:10:10.000000 myswiki-1.0.2/myswiki.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-07 14:10:10.000000 myswiki-1.0.2/myswiki.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4281 2024-05-07 09:04:53.000000 myswiki-1.0.2/myswiki.py
+-rw-rw-rw-   0        0        0       42 2024-05-07 14:10:10.795763 myswiki-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      412 2024-05-07 14:09:25.000000 myswiki-1.0.2/setup.py
```

### Comparing `myswiki-1.0.1/LICENSE` & `myswiki-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `myswiki-1.0.1/myswiki.py` & `myswiki-1.0.2/myswiki.py`

 * *Files identical despite different names*

