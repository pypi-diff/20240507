# Comparing `tmp/myswiki-2.0.0.tar.gz` & `tmp/myswiki-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myswiki-2.0.0.tar", last modified: Tue May  7 18:02:53 2024, max compression
+gzip compressed data, was "myswiki-2.0.1.tar", last modified: Tue May  7 18:06:18 2024, max compression
```

## Comparing `myswiki-2.0.0.tar` & `myswiki-2.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 18:02:53.392605 myswiki-2.0.0/
--rw-rw-rw-   0        0        0     1088 2024-05-07 08:54:42.000000 myswiki-2.0.0/LICENSE
--rw-rw-rw-   0        0        0     2162 2024-05-07 18:02:53.391605 myswiki-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1891 2024-05-07 14:17:59.000000 myswiki-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 18:02:53.390605 myswiki-2.0.0/myswiki.egg-info/
--rw-rw-rw-   0        0        0     2162 2024-05-07 18:02:53.000000 myswiki-2.0.0/myswiki.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      161 2024-05-07 18:02:53.000000 myswiki-2.0.0/myswiki.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 18:02:53.000000 myswiki-2.0.0/myswiki.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-07 18:02:53.000000 myswiki-2.0.0/myswiki.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4807 2024-05-07 18:00:48.000000 myswiki-2.0.0/myswiki.py
--rw-rw-rw-   0        0        0       42 2024-05-07 18:02:53.392605 myswiki-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      412 2024-05-07 18:02:48.000000 myswiki-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 18:06:18.942260 myswiki-2.0.1/
+-rw-rw-rw-   0        0        0     1088 2024-05-07 08:54:42.000000 myswiki-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2162 2024-05-07 18:06:18.941261 myswiki-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1891 2024-05-07 14:17:59.000000 myswiki-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 18:06:18.941261 myswiki-2.0.1/myswiki.egg-info/
+-rw-rw-rw-   0        0        0     2162 2024-05-07 18:06:18.000000 myswiki-2.0.1/myswiki.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2024-05-07 18:06:18.000000 myswiki-2.0.1/myswiki.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 18:06:18.000000 myswiki-2.0.1/myswiki.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-07 18:06:18.000000 myswiki-2.0.1/myswiki.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4807 2024-05-07 18:00:48.000000 myswiki-2.0.1/myswiki.py
+-rw-rw-rw-   0        0        0       42 2024-05-07 18:06:18.942260 myswiki-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      412 2024-05-07 18:06:12.000000 myswiki-2.0.1/setup.py
```

### Comparing `myswiki-2.0.0/LICENSE` & `myswiki-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `myswiki-2.0.0/PKG-INFO` & `myswiki-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myswiki
-Version: 2.0.0
+Version: 2.0.1
 Summary: A program for searching and reading Wikipedia articles in multiple languages
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `myswiki-2.0.0/README.md` & `myswiki-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `myswiki-2.0.0/myswiki.egg-info/PKG-INFO` & `myswiki-2.0.1/myswiki.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myswiki
-Version: 2.0.0
+Version: 2.0.1
 Summary: A program for searching and reading Wikipedia articles in multiple languages
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `myswiki-2.0.0/myswiki.py` & `myswiki-2.0.1/myswiki.py`

 * *Files identical despite different names*

