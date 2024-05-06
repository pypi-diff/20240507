# Comparing `tmp/lasertools_pulsedispersiondata-0.0.1.1.tar.gz` & `tmp/lasertools_pulsedispersiondata-0.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lasertools_pulsedispersiondata-0.0.1.1.tar", last modified: Mon May  6 21:59:16 2024, max compression
+gzip compressed data, was "lasertools_pulsedispersiondata-0.0.1.3.tar", last modified: Mon May  6 22:16:32 2024, max compression
```

## Comparing `lasertools_pulsedispersiondata-0.0.1.1.tar` & `lasertools_pulsedispersiondata-0.0.1.3.tar`

### file list

```diff
@@ -1,12 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 21:59:16.481491 lasertools_pulsedispersiondata-0.0.1.1/
--rw-rw-rw-   0        0        0    35823 2024-05-06 21:38:47.000000 lasertools_pulsedispersiondata-0.0.1.1/LICENSE
--rw-rw-rw-   0        0        0      586 2024-05-06 21:59:16.481491 lasertools_pulsedispersiondata-0.0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       72 2024-05-06 21:42:46.000000 lasertools_pulsedispersiondata-0.0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 21:59:16.480494 lasertools_pulsedispersiondata-0.0.1.1/lasertools_pulsedispersiondata.egg-info/
--rw-rw-rw-   0        0        0      586 2024-05-06 21:59:16.000000 lasertools_pulsedispersiondata-0.0.1.1/lasertools_pulsedispersiondata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-06 21:59:16.000000 lasertools_pulsedispersiondata-0.0.1.1/lasertools_pulsedispersiondata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 21:59:16.000000 lasertools_pulsedispersiondata-0.0.1.1/lasertools_pulsedispersiondata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-06 21:59:16.000000 lasertools_pulsedispersiondata-0.0.1.1/lasertools_pulsedispersiondata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 21:59:16.000000 lasertools_pulsedispersiondata-0.0.1.1/lasertools_pulsedispersiondata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-06 21:59:16.482490 lasertools_pulsedispersiondata-0.0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      842 2024-05-06 21:58:05.000000 lasertools_pulsedispersiondata-0.0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 22:16:32.803401 lasertools_pulsedispersiondata-0.0.1.3/
+-rw-rw-rw-   0        0        0    35823 2024-05-06 21:38:47.000000 lasertools_pulsedispersiondata-0.0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      586 2024-05-06 22:16:32.803401 lasertools_pulsedispersiondata-0.0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       72 2024-05-06 21:42:46.000000 lasertools_pulsedispersiondata-0.0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 22:16:32.760415 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/
+-rw-rw-rw-   0        0        0      131 2024-05-06 21:50:01.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 22:16:32.783455 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/arbitrary_index/
+-rw-rw-rw-   0        0        0      291 2024-01-25 04:59:54.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/arbitrary_index/KBr.json
+-rw-rw-rw-   0        0        0      218 2024-01-05 23:53:53.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/arbitrary_index/air.json
+drwxrwxrwx   0        0        0        0 2024-05-06 22:16:32.785450 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/arbitrary_phase/
+-rw-rw-rw-   0        0        0      400 2024-02-09 05:41:10.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/arbitrary_phase/gratings.json
+-rw-rw-rw-   0        0        0      341 2024-01-12 00:55:26.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/arbitrary_phase/polynomial.json
+-rw-rw-rw-   0        0        0      838 2024-01-11 04:24:56.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/helpers.py
+-rw-rw-rw-   0        0        0     1128 2024-01-12 00:52:56.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/loader.py
+drwxrwxrwx   0        0        0        0 2024-05-06 22:16:32.794426 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/numerical_gdd/
+-rw-rw-rw-   0        0        0     3303 2024-01-05 23:34:53.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/numerical_gdd/Layertec_182697_p.json
+-rw-rw-rw-   0        0        0    34471 2024-01-05 23:34:10.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/numerical_gdd/Layertec_182697_s.json
+-rw-rw-rw-   0        0        0    82562 2024-01-05 23:31:12.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/numerical_gdd/UFI_HD120_u.json
+-rw-rw-rw-   0        0        0   297423 2024-04-29 23:03:06.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/numerical_gdd/UFI_HD2203_u.json
+-rw-rw-rw-   0        0        0     4016 2024-01-05 19:25:54.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/numerical_gdd/UFI_HD59_p.json
+-rw-rw-rw-   0        0        0   106387 2024-01-17 19:13:45.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/numerical_gdd/bain_custom_1_rs.json
+-rw-rw-rw-   0        0        0   106394 2024-01-17 19:13:56.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/numerical_gdd/bain_custom_1_tp.json
+-rw-rw-rw-   0        0        0   106457 2024-01-17 19:13:18.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/numerical_gdd/bain_custom_1_ts.json
+drwxrwxrwx   0        0        0        0 2024-05-06 22:16:32.796420 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/numerical_phase/
+-rw-rw-rw-   0        0        0    88555 2024-01-05 23:39:23.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/numerical_phase/UFI_HD120_u_alt.json
+-rw-rw-rw-   0        0        0   305764 2024-04-29 23:03:06.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/numerical_phase/UFI_HD2203_u_alt.json
+drwxrwxrwx   0        0        0        0 2024-05-06 22:16:32.802404 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/sellmeier_index/
+-rw-rw-rw-   0        0        0      338 2024-01-05 19:26:48.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/sellmeier_index/BK7.json
+-rw-rw-rw-   0        0        0      355 2024-01-05 19:26:52.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/sellmeier_index/CaF2.json
+-rw-rw-rw-   0        0        0      355 2024-01-05 19:26:55.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/sellmeier_index/FS.json
+-rw-rw-rw-   0        0        0      359 2024-01-05 19:26:59.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/sellmeier_index/MgF2.json
+-rw-rw-rw-   0        0        0      346 2024-01-05 19:27:02.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/sellmeier_index/Si.json
+-rw-rw-rw-   0        0        0      329 2024-01-05 19:28:19.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata/sellmeier_index/ZnSe.json
+drwxrwxrwx   0        0        0        0 2024-05-06 22:16:32.781460 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata.egg-info/
+-rw-rw-rw-   0        0        0      586 2024-05-06 22:16:32.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1664 2024-05-06 22:16:32.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 22:16:32.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-06 22:16:32.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2024-05-06 22:16:32.000000 lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-06 22:16:32.805398 lasertools_pulsedispersiondata-0.0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      892 2024-05-06 22:14:20.000000 lasertools_pulsedispersiondata-0.0.1.3/setup.py
```

### Comparing `lasertools_pulsedispersiondata-0.0.1.1/LICENSE` & `lasertools_pulsedispersiondata-0.0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lasertools_pulsedispersiondata-0.0.1.1/PKG-INFO` & `lasertools_pulsedispersiondata-0.0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lasertools_pulsedispersiondata
-Version: 0.0.1.1
+Version: 0.0.1.3
 Summary: A module to store data for laser pulse dispersion
 Home-page: https://github.com/lasertools/lasertools_pulsedispersiondata
 Author: brittonm
 Author-email: 68578865+brittonm@users.noreply.github.com
 License: GPLv3
-Download-URL: https://github.com/lasertools/lasertools_pulsedispersiondata/archive/refs/tags/v_0_0_1_1.tar.gz
+Download-URL: https://github.com/lasertools/lasertools_pulsedispersiondata/archive/refs/tags/v_0_0_1_3.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
 
 # pulsedispersiondata
 A module to store data for laser pulse dispersion
```

### Comparing `lasertools_pulsedispersiondata-0.0.1.1/lasertools_pulsedispersiondata.egg-info/PKG-INFO` & `lasertools_pulsedispersiondata-0.0.1.3/lasertools_pulsedispersiondata.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lasertools-pulsedispersiondata
-Version: 0.0.1.1
+Version: 0.0.1.3
 Summary: A module to store data for laser pulse dispersion
 Home-page: https://github.com/lasertools/lasertools_pulsedispersiondata
 Author: brittonm
 Author-email: 68578865+brittonm@users.noreply.github.com
 License: GPLv3
-Download-URL: https://github.com/lasertools/lasertools_pulsedispersiondata/archive/refs/tags/v_0_0_1_1.tar.gz
+Download-URL: https://github.com/lasertools/lasertools_pulsedispersiondata/archive/refs/tags/v_0_0_1_3.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
 
 # pulsedispersiondata
 A module to store data for laser pulse dispersion
```

### Comparing `lasertools_pulsedispersiondata-0.0.1.1/setup.py` & `lasertools_pulsedispersiondata-0.0.1.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="lasertools_pulsedispersiondata",
-    version="0.0.1.1",
+    version="0.0.1.3",
     description="A module to store data for laser pulse dispersion",
     license="GPLv3",
     long_description=long_description,
     author="brittonm",
     author_email="68578865+brittonm@users.noreply.github.com",
     url="https://github.com/lasertools/lasertools_pulsedispersiondata",
-    download_url = 'https://github.com/lasertools/lasertools_pulsedispersiondata/archive/refs/tags/v_0_0_1_1.tar.gz',
+    download_url = 'https://github.com/lasertools/lasertools_pulsedispersiondata/archive/refs/tags/v_0_0_1_3.tar.gz',
+    packages=["lasertools_pulsedispersiondata"],
     install_requires=[
         "numpy",
     ],
     classifiers=[
       'Programming Language :: Python :: 3.9',
     ],
     package_data={
```

