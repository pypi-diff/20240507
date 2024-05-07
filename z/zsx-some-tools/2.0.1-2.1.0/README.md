# Comparing `tmp/zsx_some_tools-2.0.1.tar.gz` & `tmp/zsx_some_tools-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zsx_some_tools-2.0.1.tar", last modified: Fri Mar 31 05:32:42 2023, max compression
+gzip compressed data, was "zsx_some_tools-2.1.0.tar", last modified: Tue May  7 13:11:37 2024, max compression
```

## Comparing `zsx_some_tools-2.0.1.tar` & `zsx_some_tools-2.1.0.tar`

### file list

```diff
@@ -1,18 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 05:32:42.102836 zsx_some_tools-2.0.1/
--rw-rw-rw-   0        0        0      611 2023-03-31 05:32:42.102836 zsx_some_tools-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       17 2023-03-31 02:25:22.000000 zsx_some_tools-2.0.1/README.md
--rw-rw-rw-   0        0        0      526 2023-03-31 02:36:32.000000 zsx_some_tools-2.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-31 05:32:42.102836 zsx_some_tools-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      322 2023-03-31 05:31:15.000000 zsx_some_tools-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-31 05:32:42.092884 zsx_some_tools-2.0.1/zsx_some_tools/
--rw-rw-rw-   0        0        0      218 2022-08-10 11:39:56.000000 zsx_some_tools-2.0.1/zsx_some_tools/__init__.py
--rw-rw-rw-   0        0        0    17950 2023-02-15 07:30:22.000000 zsx_some_tools-2.0.1/zsx_some_tools/basic_tools.py
--rw-rw-rw-   0        0        0    19798 2023-03-29 01:34:30.000000 zsx_some_tools-2.0.1/zsx_some_tools/bio_tools.py
--rw-rw-rw-   0        0        0     7903 2022-12-29 11:59:11.000000 zsx_some_tools-2.0.1/zsx_some_tools/plot_tools.py
--rw-rw-rw-   0        0        0    16938 2023-03-24 02:33:24.000000 zsx_some_tools-2.0.1/zsx_some_tools/read_write_tools.py
--rw-rw-rw-   0        0        0      616 2022-08-30 03:00:52.000000 zsx_some_tools-2.0.1/zsx_some_tools/za.py
-drwxrwxrwx   0        0        0        0 2023-03-31 05:32:42.099859 zsx_some_tools-2.0.1/zsx_some_tools.egg-info/
--rw-rw-rw-   0        0        0      611 2023-03-31 05:32:42.000000 zsx_some_tools-2.0.1/zsx_some_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-03-31 05:32:42.000000 zsx_some_tools-2.0.1/zsx_some_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 05:32:42.000000 zsx_some_tools-2.0.1/zsx_some_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-03-31 05:32:42.000000 zsx_some_tools-2.0.1/zsx_some_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 13:11:37.138693 zsx_some_tools-2.1.0/
+-rw-rw-rw-   0        0        0      531 2024-05-07 13:11:37.136696 zsx_some_tools-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2023-03-31 02:25:24.000000 zsx_some_tools-2.1.0/README.md
+-rw-rw-rw-   0        0        0      526 2024-04-30 08:59:28.000000 zsx_some_tools-2.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-07 13:11:37.138693 zsx_some_tools-2.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-07 13:11:37.076211 zsx_some_tools-2.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-07 13:11:37.106486 zsx_some_tools-2.1.0/src/zsx_some_tools/
+-rw-rw-rw-   0        0        0      218 2022-08-10 11:39:58.000000 zsx_some_tools-2.1.0/src/zsx_some_tools/__init__.py
+-rw-rw-rw-   0        0        0    24835 2024-04-30 09:12:31.000000 zsx_some_tools-2.1.0/src/zsx_some_tools/basic_tools.py
+-rw-rw-rw-   0        0        0    38126 2024-04-30 09:12:31.000000 zsx_some_tools-2.1.0/src/zsx_some_tools/bio_tools.py
+-rw-rw-rw-   0        0        0    12301 2024-04-30 08:28:55.000000 zsx_some_tools-2.1.0/src/zsx_some_tools/plot_tools.py
+-rw-rw-rw-   0        0        0    21568 2024-04-26 05:23:52.000000 zsx_some_tools-2.1.0/src/zsx_some_tools/read_write_tools.py
+-rw-rw-rw-   0        0        0      322 2023-03-31 05:31:16.000000 zsx_some_tools-2.1.0/src/zsx_some_tools/setup.py
+-rw-rw-rw-   0        0        0     2785 2024-01-13 07:29:54.000000 zsx_some_tools-2.1.0/src/zsx_some_tools/za.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:11:37.131693 zsx_some_tools-2.1.0/src/zsx_some_tools/zsx_some_tools/
+-rw-rw-rw-   0        0        0      218 2022-08-10 11:39:58.000000 zsx_some_tools-2.1.0/src/zsx_some_tools/zsx_some_tools/__init__.py
+-rw-rw-rw-   0        0        0    17950 2023-02-15 07:30:24.000000 zsx_some_tools-2.1.0/src/zsx_some_tools/zsx_some_tools/basic_tools.py
+-rw-rw-rw-   0        0        0    19798 2023-03-29 01:34:32.000000 zsx_some_tools-2.1.0/src/zsx_some_tools/zsx_some_tools/bio_tools.py
+-rw-rw-rw-   0        0        0     7903 2022-12-29 11:59:12.000000 zsx_some_tools-2.1.0/src/zsx_some_tools/zsx_some_tools/plot_tools.py
+-rw-rw-rw-   0        0        0    16938 2023-03-24 02:33:26.000000 zsx_some_tools-2.1.0/src/zsx_some_tools/zsx_some_tools/read_write_tools.py
+-rw-rw-rw-   0        0        0      616 2022-08-30 03:00:54.000000 zsx_some_tools-2.1.0/src/zsx_some_tools/zsx_some_tools/za.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:11:37.133692 zsx_some_tools-2.1.0/src/zsx_some_tools.egg-info/
+-rw-rw-rw-   0        0        0      531 2024-05-07 13:11:37.000000 zsx_some_tools-2.1.0/src/zsx_some_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      698 2024-05-07 13:11:37.000000 zsx_some_tools-2.1.0/src/zsx_some_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 13:11:37.000000 zsx_some_tools-2.1.0/src/zsx_some_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-07 13:11:37.000000 zsx_some_tools-2.1.0/src/zsx_some_tools.egg-info/top_level.txt
```

### Comparing `zsx_some_tools-2.0.1/pyproject.toml` & `zsx_some_tools-2.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "zsx_some_tools"
-version = "2.0.1"
+version = "2.1.0"
 authors = [
   { name="Zhang Senxin", email="sxzhang997@qq.com" },
 ]
 description = "Package tools for daily use"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `zsx_some_tools-2.0.1/zsx_some_tools/basic_tools.py` & `zsx_some_tools-2.1.0/src/zsx_some_tools/zsx_some_tools/basic_tools.py`

 * *Files identical despite different names*

### Comparing `zsx_some_tools-2.0.1/zsx_some_tools/bio_tools.py` & `zsx_some_tools-2.1.0/src/zsx_some_tools/zsx_some_tools/bio_tools.py`

 * *Files identical despite different names*

### Comparing `zsx_some_tools-2.0.1/zsx_some_tools/plot_tools.py` & `zsx_some_tools-2.1.0/src/zsx_some_tools/zsx_some_tools/plot_tools.py`

 * *Files identical despite different names*

### Comparing `zsx_some_tools-2.0.1/zsx_some_tools/read_write_tools.py` & `zsx_some_tools-2.1.0/src/zsx_some_tools/zsx_some_tools/read_write_tools.py`

 * *Files identical despite different names*

### Comparing `zsx_some_tools-2.0.1/zsx_some_tools/za.py` & `zsx_some_tools-2.1.0/src/zsx_some_tools/zsx_some_tools/za.py`

 * *Files identical despite different names*

