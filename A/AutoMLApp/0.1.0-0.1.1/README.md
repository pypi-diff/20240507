# Comparing `tmp/automlapp-0.1.0.tar.gz` & `tmp/automlapp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automlapp-0.1.0.tar", last modified: Fri May  3 11:42:02 2024, max compression
+gzip compressed data, was "automlapp-0.1.1.tar", last modified: Tue May  7 09:15:37 2024, max compression
```

## Comparing `automlapp-0.1.0.tar` & `automlapp-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 11:42:02.689894 automlapp-0.1.0/
-drwxrwxrwx   0        0        0        0 2024-05-03 11:42:02.684317 automlapp-0.1.0/AutoMLApp.egg-info/
--rw-rw-rw-   0        0        0     5051 2024-05-03 11:42:02.000000 automlapp-0.1.0/AutoMLApp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2024-05-03 11:42:02.000000 automlapp-0.1.0/AutoMLApp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 11:42:02.000000 automlapp-0.1.0/AutoMLApp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-05-03 11:42:02.000000 automlapp-0.1.0/AutoMLApp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      268 2024-05-03 11:42:02.000000 automlapp-0.1.0/AutoMLApp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 11:42:02.000000 automlapp-0.1.0/AutoMLApp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-05-03 11:39:36.000000 automlapp-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     5051 2024-05-03 11:42:02.684317 automlapp-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3993 2024-04-12 09:40:36.000000 automlapp-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-03 11:42:02.689894 automlapp-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1473 2024-05-03 11:38:22.000000 automlapp-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 09:15:37.559116 automlapp-0.1.1/
+drwxrwxrwx   0        0        0        0 2024-05-07 09:15:37.559116 automlapp-0.1.1/AutoMLApp.egg-info/
+-rw-rw-rw-   0        0        0     5051 2024-05-07 09:15:37.000000 automlapp-0.1.1/AutoMLApp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2024-05-07 09:15:37.000000 automlapp-0.1.1/AutoMLApp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 09:15:37.000000 automlapp-0.1.1/AutoMLApp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-07 09:15:37.000000 automlapp-0.1.1/AutoMLApp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      268 2024-05-07 09:15:37.000000 automlapp-0.1.1/AutoMLApp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 09:15:37.000000 automlapp-0.1.1/AutoMLApp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-05-03 11:39:36.000000 automlapp-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     5051 2024-05-07 09:15:37.559116 automlapp-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3993 2024-04-12 09:40:36.000000 automlapp-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-07 09:15:37.559116 automlapp-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1473 2024-05-07 09:15:14.000000 automlapp-0.1.1/setup.py
```

### Comparing `automlapp-0.1.0/AutoMLApp.egg-info/PKG-INFO` & `automlapp-0.1.1/AutoMLApp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoMLApp
-Version: 0.1.0
+Version: 0.1.1
 Summary: An automated machine learning application designed for efficient model training, evaluation, and hyperparameter tuning.
 Author: Shivam Nikam
 Author-email: shivam.nikam@think360.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `automlapp-0.1.0/LICENSE` & `automlapp-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.0/PKG-INFO` & `automlapp-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoMLApp
-Version: 0.1.0
+Version: 0.1.1
 Summary: An automated machine learning application designed for efficient model training, evaluation, and hyperparameter tuning.
 Author: Shivam Nikam
 Author-email: shivam.nikam@think360.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `automlapp-0.1.0/README.md` & `automlapp-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.0/setup.py` & `automlapp-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="AutoMLApp",
-    version="0.1.0",
+    version="0.1.1",
     author="Shivam Nikam",
     author_email="shivam.nikam@think360.ai",
     description="An automated machine learning application designed for efficient model training, evaluation, and hyperparameter tuning.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     #url="https://github.com/YourGithub/AutoMLApp",
     packages=find_packages(),
@@ -38,11 +38,11 @@
         ],
     },
     package_data={
         "sample": ["package_data.dat"],
     },
     entry_points={
         "console_scripts": [
-            "automlapp=automlapp.cli:main",
+            "automlapp=automlapp.app:main",
         ],
     },
 )
```

