# Comparing `tmp/convert-us-to-uk-0.1.6.tar.gz` & `tmp/convert-us-to-uk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convert-us-to-uk-0.1.6.tar", last modified: Fri May  3 15:50:23 2024, max compression
+gzip compressed data, was "convert-us-to-uk-0.1.7.tar", last modified: Tue May  7 08:18:42 2024, max compression
```

## Comparing `convert-us-to-uk-0.1.6.tar` & `convert-us-to-uk-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 15:50:23.130891 convert-us-to-uk-0.1.6/
--rw-rw-rw-   0        0        0       43 2024-04-17 15:15:06.000000 convert-us-to-uk-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1990 2024-05-03 15:50:23.128745 convert-us-to-uk-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1660 2024-04-18 11:43:12.000000 convert-us-to-uk-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 15:50:23.110747 convert-us-to-uk-0.1.6/convert_us_to_uk/
--rw-rw-rw-   0        0        0        0 2024-04-17 12:42:42.000000 convert-us-to-uk-0.1.6/convert_us_to_uk/__init__.py
--rw-rw-rw-   0        0        0     1533 2024-04-30 10:34:39.000000 convert-us-to-uk-0.1.6/convert_us_to_uk/converter.py
--rw-rw-rw-   0        0        0    39780 2024-05-03 15:49:27.000000 convert-us-to-uk-0.1.6/convert_us_to_uk/us_to_uk_trans.csv
-drwxrwxrwx   0        0        0        0 2024-05-03 15:50:23.123752 convert-us-to-uk-0.1.6/convert_us_to_uk.egg-info/
--rw-rw-rw-   0        0        0     1990 2024-05-03 15:50:22.000000 convert-us-to-uk-0.1.6/convert_us_to_uk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2024-05-03 15:50:23.000000 convert-us-to-uk-0.1.6/convert_us_to_uk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 15:50:22.000000 convert-us-to-uk-0.1.6/convert_us_to_uk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-05-03 15:50:22.000000 convert-us-to-uk-0.1.6/convert_us_to_uk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-05-03 15:50:23.000000 convert-us-to-uk-0.1.6/convert_us_to_uk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 15:50:23.130891 convert-us-to-uk-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      696 2024-05-03 15:49:59.000000 convert-us-to-uk-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 15:50:23.125745 convert-us-to-uk-0.1.6/tests/
--rw-rw-rw-   0        0        0      296 2024-04-17 14:23:12.000000 convert-us-to-uk-0.1.6/tests/test_converter.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:18:42.182963 convert-us-to-uk-0.1.7/
+-rw-rw-rw-   0        0        0       43 2024-04-17 15:15:06.000000 convert-us-to-uk-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1990 2024-05-07 08:18:42.178653 convert-us-to-uk-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1660 2024-04-18 11:43:12.000000 convert-us-to-uk-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 08:18:42.157689 convert-us-to-uk-0.1.7/convert_us_to_uk/
+-rw-rw-rw-   0        0        0        0 2024-04-17 12:42:42.000000 convert-us-to-uk-0.1.7/convert_us_to_uk/__init__.py
+-rw-rw-rw-   0        0        0     1533 2024-04-30 10:34:39.000000 convert-us-to-uk-0.1.7/convert_us_to_uk/converter.py
+-rw-rw-rw-   0        0        0    39744 2024-05-07 08:18:03.000000 convert-us-to-uk-0.1.7/convert_us_to_uk/us_to_uk_trans.csv
+drwxrwxrwx   0        0        0        0 2024-05-07 08:18:42.173776 convert-us-to-uk-0.1.7/convert_us_to_uk.egg-info/
+-rw-rw-rw-   0        0        0     1990 2024-05-07 08:18:41.000000 convert-us-to-uk-0.1.7/convert_us_to_uk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2024-05-07 08:18:41.000000 convert-us-to-uk-0.1.7/convert_us_to_uk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 08:18:41.000000 convert-us-to-uk-0.1.7/convert_us_to_uk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-05-07 08:18:41.000000 convert-us-to-uk-0.1.7/convert_us_to_uk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-05-07 08:18:41.000000 convert-us-to-uk-0.1.7/convert_us_to_uk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 08:18:42.183439 convert-us-to-uk-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      696 2024-05-07 08:18:21.000000 convert-us-to-uk-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:18:42.175311 convert-us-to-uk-0.1.7/tests/
+-rw-rw-rw-   0        0        0      296 2024-04-17 14:23:12.000000 convert-us-to-uk-0.1.7/tests/test_converter.py
```

### Comparing `convert-us-to-uk-0.1.6/PKG-INFO` & `convert-us-to-uk-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convert-us-to-uk
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple utility to convert US spelling to UK spelling.
 Home-page: https://github.com/oliverblane/convert-us-to-uk/tree/main
 Author: Oliver Blane
 Author-email: oliverblane72@gmail.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `convert-us-to-uk-0.1.6/README.md` & `convert-us-to-uk-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `convert-us-to-uk-0.1.6/convert_us_to_uk/converter.py` & `convert-us-to-uk-0.1.7/convert_us_to_uk/converter.py`

 * *Files identical despite different names*

### Comparing `convert-us-to-uk-0.1.6/convert_us_to_uk/us_to_uk_trans.csv` & `convert-us-to-uk-0.1.7/convert_us_to_uk/us_to_uk_trans.csv`

 * *Files 0% similar despite different names*

```diff
@@ -1690,11 +1690,9 @@
 woolies,woollies
 wooly,woolly
 worshiped,worshipped
 worshiping,worshipping
 worshiper,worshipper
 yodeled,yodelled
 yodeling,yodelling
-yogurt,yoghourt
-yogurts,yoghourts
 yogurt,yoghurt
 yogurts,yoghurts
```

### Comparing `convert-us-to-uk-0.1.6/convert_us_to_uk.egg-info/PKG-INFO` & `convert-us-to-uk-0.1.7/convert_us_to_uk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convert-us-to-uk
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple utility to convert US spelling to UK spelling.
 Home-page: https://github.com/oliverblane/convert-us-to-uk/tree/main
 Author: Oliver Blane
 Author-email: oliverblane72@gmail.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `convert-us-to-uk-0.1.6/setup.py` & `convert-us-to-uk-0.1.7/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='convert-us-to-uk',
-    version='0.1.6',
+    version='0.1.7',
     packages=find_packages(),
     include_package_data=True,
     description='A simple utility to convert US spelling to UK spelling.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Oliver Blane',
     author_email='oliverblane72@gmail.com',
```

