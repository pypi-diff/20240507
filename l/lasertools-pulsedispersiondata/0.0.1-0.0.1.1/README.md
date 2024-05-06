# Comparing `tmp/lasertools_pulsedispersiondata-0.0.1.tar.gz` & `tmp/lasertools_pulsedispersiondata-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lasertools_pulsedispersiondata-0.0.1.tar", last modified: Mon May  6 21:45:57 2024, max compression
+gzip compressed data, was "lasertools_pulsedispersiondata-0.0.1.1.tar", last modified: Mon May  6 21:59:16 2024, max compression
```

## Comparing `lasertools_pulsedispersiondata-0.0.1.tar` & `lasertools_pulsedispersiondata-0.0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 21:45:57.849862 lasertools_pulsedispersiondata-0.0.1/
--rw-rw-rw-   0        0        0    35823 2024-05-06 21:38:47.000000 lasertools_pulsedispersiondata-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      582 2024-05-06 21:45:57.849862 lasertools_pulsedispersiondata-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       72 2024-05-06 21:42:46.000000 lasertools_pulsedispersiondata-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 21:45:57.848865 lasertools_pulsedispersiondata-0.0.1/lasertools_pulsedispersiondata.egg-info/
--rw-rw-rw-   0        0        0      582 2024-05-06 21:45:57.000000 lasertools_pulsedispersiondata-0.0.1/lasertools_pulsedispersiondata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-06 21:45:57.000000 lasertools_pulsedispersiondata-0.0.1/lasertools_pulsedispersiondata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 21:45:57.000000 lasertools_pulsedispersiondata-0.0.1/lasertools_pulsedispersiondata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-06 21:45:57.000000 lasertools_pulsedispersiondata-0.0.1/lasertools_pulsedispersiondata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 21:45:57.000000 lasertools_pulsedispersiondata-0.0.1/lasertools_pulsedispersiondata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-06 21:45:57.851856 lasertools_pulsedispersiondata-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      830 2024-05-06 21:44:14.000000 lasertools_pulsedispersiondata-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 21:59:16.481491 lasertools_pulsedispersiondata-0.0.1.1/
+-rw-rw-rw-   0        0        0    35823 2024-05-06 21:38:47.000000 lasertools_pulsedispersiondata-0.0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      586 2024-05-06 21:59:16.481491 lasertools_pulsedispersiondata-0.0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       72 2024-05-06 21:42:46.000000 lasertools_pulsedispersiondata-0.0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 21:59:16.480494 lasertools_pulsedispersiondata-0.0.1.1/lasertools_pulsedispersiondata.egg-info/
+-rw-rw-rw-   0        0        0      586 2024-05-06 21:59:16.000000 lasertools_pulsedispersiondata-0.0.1.1/lasertools_pulsedispersiondata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-06 21:59:16.000000 lasertools_pulsedispersiondata-0.0.1.1/lasertools_pulsedispersiondata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 21:59:16.000000 lasertools_pulsedispersiondata-0.0.1.1/lasertools_pulsedispersiondata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-06 21:59:16.000000 lasertools_pulsedispersiondata-0.0.1.1/lasertools_pulsedispersiondata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 21:59:16.000000 lasertools_pulsedispersiondata-0.0.1.1/lasertools_pulsedispersiondata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-06 21:59:16.482490 lasertools_pulsedispersiondata-0.0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      842 2024-05-06 21:58:05.000000 lasertools_pulsedispersiondata-0.0.1.1/setup.py
```

### Comparing `lasertools_pulsedispersiondata-0.0.1/LICENSE` & `lasertools_pulsedispersiondata-0.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lasertools_pulsedispersiondata-0.0.1/PKG-INFO` & `lasertools_pulsedispersiondata-0.0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lasertools_pulsedispersiondata
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: A module to store data for laser pulse dispersion
 Home-page: https://github.com/lasertools/lasertools_pulsedispersiondata
 Author: brittonm
 Author-email: 68578865+brittonm@users.noreply.github.com
 License: GPLv3
-Download-URL: https://github.com/lasertools/lasertools_pulsedispersiondata/archive/refs/tags/v_0_0_1.tar.gz
+Download-URL: https://github.com/lasertools/lasertools_pulsedispersiondata/archive/refs/tags/v_0_0_1_1.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
 
 # pulsedispersiondata
 A module to store data for laser pulse dispersion
```

### Comparing `lasertools_pulsedispersiondata-0.0.1/lasertools_pulsedispersiondata.egg-info/PKG-INFO` & `lasertools_pulsedispersiondata-0.0.1.1/lasertools_pulsedispersiondata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lasertools-pulsedispersiondata
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: A module to store data for laser pulse dispersion
 Home-page: https://github.com/lasertools/lasertools_pulsedispersiondata
 Author: brittonm
 Author-email: 68578865+brittonm@users.noreply.github.com
 License: GPLv3
-Download-URL: https://github.com/lasertools/lasertools_pulsedispersiondata/archive/refs/tags/v_0_0_1.tar.gz
+Download-URL: https://github.com/lasertools/lasertools_pulsedispersiondata/archive/refs/tags/v_0_0_1_1.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
 
 # pulsedispersiondata
 A module to store data for laser pulse dispersion
```

### Comparing `lasertools_pulsedispersiondata-0.0.1/setup.py` & `lasertools_pulsedispersiondata-0.0.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="lasertools_pulsedispersiondata",
-    version="0.0.1",
+    version="0.0.1.1",
     description="A module to store data for laser pulse dispersion",
     license="GPLv3",
     long_description=long_description,
     author="brittonm",
     author_email="68578865+brittonm@users.noreply.github.com",
     url="https://github.com/lasertools/lasertools_pulsedispersiondata",
-    download_url = 'https://github.com/lasertools/lasertools_pulsedispersiondata/archive/refs/tags/v_0_0_1.tar.gz',
+    download_url = 'https://github.com/lasertools/lasertools_pulsedispersiondata/archive/refs/tags/v_0_0_1_1.tar.gz',
     install_requires=[
         "numpy",
     ],
     classifiers=[
       'Programming Language :: Python :: 3.9',
     ],
     package_data={
-        "pulsedispersiondatadev": [
+        "lasertools_pulsedispersiondata": [
             "*/*.json"
         ],
     },
 )
```

