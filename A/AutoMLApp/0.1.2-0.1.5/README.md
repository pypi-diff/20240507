# Comparing `tmp/automlapp-0.1.2.tar.gz` & `tmp/automlapp-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automlapp-0.1.2.tar", last modified: Tue May  7 09:50:20 2024, max compression
+gzip compressed data, was "automlapp-0.1.5.tar", last modified: Tue May  7 10:14:12 2024, max compression
```

## Comparing `automlapp-0.1.2.tar` & `automlapp-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 09:50:20.981434 automlapp-0.1.2/
-drwxrwxrwx   0        0        0        0 2024-05-07 09:50:20.976566 automlapp-0.1.2/AutoMLApp.egg-info/
--rw-rw-rw-   0        0        0     5051 2024-05-07 09:50:20.000000 automlapp-0.1.2/AutoMLApp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2024-05-07 09:50:20.000000 automlapp-0.1.2/AutoMLApp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 09:50:20.000000 automlapp-0.1.2/AutoMLApp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-05-07 09:50:20.000000 automlapp-0.1.2/AutoMLApp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      268 2024-05-07 09:50:20.000000 automlapp-0.1.2/AutoMLApp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 09:50:20.000000 automlapp-0.1.2/AutoMLApp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-05-03 11:39:36.000000 automlapp-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     5051 2024-05-07 09:50:20.976566 automlapp-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3993 2024-04-12 09:40:36.000000 automlapp-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-07 09:50:20.981434 automlapp-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1494 2024-05-07 09:50:03.000000 automlapp-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 10:14:12.305049 automlapp-0.1.5/
+drwxrwxrwx   0        0        0        0 2024-05-07 10:14:12.302002 automlapp-0.1.5/AutoMLApp.egg-info/
+-rw-rw-rw-   0        0        0     5051 2024-05-07 10:14:12.000000 automlapp-0.1.5/AutoMLApp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2024-05-07 10:14:12.000000 automlapp-0.1.5/AutoMLApp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 10:14:12.000000 automlapp-0.1.5/AutoMLApp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-05-07 10:14:12.000000 automlapp-0.1.5/AutoMLApp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      268 2024-05-07 10:14:12.000000 automlapp-0.1.5/AutoMLApp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-07 10:14:12.000000 automlapp-0.1.5/AutoMLApp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-05-03 11:39:36.000000 automlapp-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     5051 2024-05-07 10:14:12.304004 automlapp-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3993 2024-04-12 09:40:36.000000 automlapp-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 10:14:12.297350 automlapp-0.1.5/automlapp/
+-rw-rw-rw-   0        0        0       44 2024-05-07 10:07:08.000000 automlapp-0.1.5/automlapp/__init__.py
+-rw-rw-rw-   0        0        0    60999 2024-05-07 10:10:10.000000 automlapp-0.1.5/automlapp/app.py
+-rw-rw-rw-   0        0        0      405 2024-05-07 09:49:38.000000 automlapp-0.1.5/automlapp/launcher.py
+-rw-rw-rw-   0        0        0       42 2024-05-07 10:14:12.305049 automlapp-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1493 2024-05-07 10:14:07.000000 automlapp-0.1.5/setup.py
```

### Comparing `automlapp-0.1.2/AutoMLApp.egg-info/PKG-INFO` & `automlapp-0.1.5/AutoMLApp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoMLApp
-Version: 0.1.2
+Version: 0.1.5
 Summary: An automated machine learning application designed for efficient model training, evaluation, and hyperparameter tuning.
 Author: Shivam Nikam
 Author-email: shivam.nikam@think360.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `automlapp-0.1.2/LICENSE` & `automlapp-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.2/PKG-INFO` & `automlapp-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoMLApp
-Version: 0.1.2
+Version: 0.1.5
 Summary: An automated machine learning application designed for efficient model training, evaluation, and hyperparameter tuning.
 Author: Shivam Nikam
 Author-email: shivam.nikam@think360.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `automlapp-0.1.2/README.md` & `automlapp-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.2/setup.py` & `automlapp-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="AutoMLApp",
-    version="0.1.2",
+    version="0.1.5",
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
-            "run_automlapp=automlapp.launcher:launch_streamlit",
+            "runautomlapp=automlapp.launcher:launch_streamlit",
         ],
     },
 )
```

