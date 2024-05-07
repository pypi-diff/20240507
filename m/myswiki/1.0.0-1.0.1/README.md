# Comparing `tmp/myswiki-1.0.0.tar.gz` & `tmp/myswiki-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myswiki-1.0.0.tar", last modified: Tue May  7 09:00:09 2024, max compression
+gzip compressed data, was "myswiki-1.0.1.tar", last modified: Tue May  7 09:04:58 2024, max compression
```

## Comparing `myswiki-1.0.0.tar` & `myswiki-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 09:00:09.636326 myswiki-1.0.0/
--rw-rw-rw-   0        0        0     1088 2024-05-07 08:54:42.000000 myswiki-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      191 2024-05-07 09:00:09.635326 myswiki-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-07 09:00:09.634326 myswiki-1.0.0/myswiki.egg-info/
--rw-rw-rw-   0        0        0      191 2024-05-07 09:00:09.000000 myswiki-1.0.0/myswiki.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      151 2024-05-07 09:00:09.000000 myswiki-1.0.0/myswiki.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 09:00:09.000000 myswiki-1.0.0/myswiki.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-07 09:00:09.000000 myswiki-1.0.0/myswiki.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       61 2024-05-07 08:56:19.000000 myswiki-1.0.0/myswiki.py
--rw-rw-rw-   0        0        0       42 2024-05-07 09:00:09.636326 myswiki-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      257 2024-05-07 08:56:19.000000 myswiki-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 09:04:58.060536 myswiki-1.0.1/
+-rw-rw-rw-   0        0        0     1088 2024-05-07 08:54:42.000000 myswiki-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      191 2024-05-07 09:04:58.059536 myswiki-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-07 09:04:58.058535 myswiki-1.0.1/myswiki.egg-info/
+-rw-rw-rw-   0        0        0      191 2024-05-07 09:04:57.000000 myswiki-1.0.1/myswiki.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      151 2024-05-07 09:04:58.000000 myswiki-1.0.1/myswiki.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 09:04:57.000000 myswiki-1.0.1/myswiki.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-07 09:04:57.000000 myswiki-1.0.1/myswiki.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4281 2024-05-07 09:04:53.000000 myswiki-1.0.1/myswiki.py
+-rw-rw-rw-   0        0        0       42 2024-05-07 09:04:58.060536 myswiki-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      257 2024-05-07 09:04:53.000000 myswiki-1.0.1/setup.py
```

### Comparing `myswiki-1.0.0/LICENSE` & `myswiki-1.0.1/LICENSE`

 * *Files identical despite different names*

