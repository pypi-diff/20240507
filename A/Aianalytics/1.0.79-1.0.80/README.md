# Comparing `tmp/Aianalytics-1.0.79.tar.gz` & `tmp/Aianalytics-1.0.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Aianalytics-1.0.79.tar", last modified: Mon Mar  4 14:30:55 2024, max compression
+gzip compressed data, was "Aianalytics-1.0.80.tar", last modified: Tue May  7 14:53:04 2024, max compression
```

## Comparing `Aianalytics-1.0.79.tar` & `Aianalytics-1.0.80.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-04 14:30:55.509391 Aianalytics-1.0.79/
-drwxrwxrwx   0        0        0        0 2024-03-04 14:30:55.486518 Aianalytics-1.0.79/Aianalytics/
--rw-rw-rw-   0        0        0    41057 2024-03-04 14:30:23.000000 Aianalytics-1.0.79/Aianalytics/__init__.py
--rw-rw-rw-   0        0        0    41045 2024-03-04 00:12:24.000000 Aianalytics-1.0.79/Aianalytics/a.py
-drwxrwxrwx   0        0        0        0 2024-03-04 14:30:55.506399 Aianalytics-1.0.79/Aianalytics.egg-info/
--rw-rw-rw-   0        0        0      579 2024-03-04 14:30:55.000000 Aianalytics-1.0.79/Aianalytics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-03-04 14:30:55.000000 Aianalytics-1.0.79/Aianalytics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-04 14:30:55.000000 Aianalytics-1.0.79/Aianalytics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      143 2024-03-04 14:30:55.000000 Aianalytics-1.0.79/Aianalytics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-04 14:30:55.000000 Aianalytics-1.0.79/Aianalytics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1477 2023-07-11 09:07:10.000000 Aianalytics-1.0.79/LICENSE.txt
--rw-rw-rw-   0        0        0      579 2024-03-04 14:30:55.508394 Aianalytics-1.0.79/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-03-04 14:30:55.509391 Aianalytics-1.0.79/setup.cfg
--rw-rw-rw-   0        0        0     1078 2024-03-04 14:30:44.000000 Aianalytics-1.0.79/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 14:53:04.350286 Aianalytics-1.0.80/
+drwxrwxrwx   0        0        0        0 2024-05-07 14:53:04.317400 Aianalytics-1.0.80/Aianalytics/
+-rw-rw-rw-   0        0        0    86147 2024-05-07 14:52:06.000000 Aianalytics-1.0.80/Aianalytics/__init__.py
+-rw-rw-rw-   0        0        0    86147 2024-05-07 14:52:21.000000 Aianalytics-1.0.80/Aianalytics/a.py
+drwxrwxrwx   0        0        0        0 2024-05-07 14:53:04.345299 Aianalytics-1.0.80/Aianalytics.egg-info/
+-rw-rw-rw-   0        0        0      579 2024-05-07 14:53:03.000000 Aianalytics-1.0.80/Aianalytics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-05-07 14:53:03.000000 Aianalytics-1.0.80/Aianalytics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 14:53:03.000000 Aianalytics-1.0.80/Aianalytics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      143 2024-05-07 14:53:03.000000 Aianalytics-1.0.80/Aianalytics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-07 14:53:03.000000 Aianalytics-1.0.80/Aianalytics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1477 2023-07-11 09:07:10.000000 Aianalytics-1.0.80/LICENSE.txt
+-rw-rw-rw-   0        0        0      579 2024-05-07 14:53:04.347293 Aianalytics-1.0.80/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-07 14:53:04.350286 Aianalytics-1.0.80/setup.cfg
+-rw-rw-rw-   0        0        0     1078 2024-05-07 14:52:52.000000 Aianalytics-1.0.80/setup.py
```

### Comparing `Aianalytics-1.0.79/Aianalytics.egg-info/PKG-INFO` & `Aianalytics-1.0.80/Aianalytics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Aianalytics
-Version: 1.0.79
+Version: 1.0.80
 Summary: A module for image processing
 Author: Armankhanvsit
 Author-email: armanpconly@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `Aianalytics-1.0.79/LICENSE.txt` & `Aianalytics-1.0.80/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Aianalytics-1.0.79/PKG-INFO` & `Aianalytics-1.0.80/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Aianalytics
-Version: 1.0.79
+Version: 1.0.80
 Summary: A module for image processing
 Author: Armankhanvsit
 Author-email: armanpconly@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `Aianalytics-1.0.79/setup.py` & `Aianalytics-1.0.80/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='Aianalytics',
-    version='1.0.79',
+    version='1.0.80',
     author='Armankhanvsit',
     author_email='armanpconly@gmail.com',
     description='A module for image processing',
     long_description='A module for image processing using numpy, PIL, scipy, and matplotlib.',
     packages=['Aianalytics'],
   install_requires=[
     'numpy',
```

