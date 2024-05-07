# Comparing `tmp/datalibro_backend-1.1.2.tar.gz` & `tmp/datalibro_backend-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalibro_backend-1.1.2.tar", last modified: Thu Apr 18 06:06:27 2024, max compression
+gzip compressed data, was "datalibro_backend-1.1.3.tar", last modified: Tue May  7 02:48:11 2024, max compression
```

## Comparing `datalibro_backend-1.1.2.tar` & `datalibro_backend-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-04-18 06:06:27.546993 datalibro_backend-1.1.2/
--rw-r--r--   0 zhoulucy   (501) staff       (20)     1070 2023-12-08 09:34:06.000000 datalibro_backend-1.1.2/LICENSE.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-04-18 06:06:27.546700 datalibro_backend-1.1.2/PKG-INFO
--rw-r--r--   0 zhoulucy   (501) staff       (20)     1683 2023-12-08 09:30:25.000000 datalibro_backend-1.1.2/README.md
-drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-04-18 06:06:27.545446 datalibro_backend-1.1.2/datalibro_backend/
--rw-r--r--   0 zhoulucy   (501) staff       (20)      207 2024-02-01 06:19:04.000000 datalibro_backend-1.1.2/datalibro_backend/__init__.py
--rw-r--r--   0 zhoulucy   (501) staff       (20)    15308 2024-04-18 06:06:10.000000 datalibro_backend-1.1.2/datalibro_backend/quality_check.py
--rw-r--r--   0 zhoulucy   (501) staff       (20)     6994 2024-02-01 06:18:54.000000 datalibro_backend-1.1.2/datalibro_backend/read_file.py
-drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-04-18 06:06:27.546470 datalibro_backend-1.1.2/datalibro_backend.egg-info/
--rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-04-18 06:06:27.000000 datalibro_backend-1.1.2/datalibro_backend.egg-info/PKG-INFO
--rw-r--r--   0 zhoulucy   (501) staff       (20)      290 2024-04-18 06:06:27.000000 datalibro_backend-1.1.2/datalibro_backend.egg-info/SOURCES.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)        1 2024-04-18 06:06:27.000000 datalibro_backend-1.1.2/datalibro_backend.egg-info/dependency_links.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)       18 2024-04-18 06:06:27.000000 datalibro_backend-1.1.2/datalibro_backend.egg-info/top_level.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)       38 2024-04-18 06:06:27.547055 datalibro_backend-1.1.2/setup.cfg
--rw-r--r--   0 zhoulucy   (501) staff       (20)      594 2024-04-18 06:06:18.000000 datalibro_backend-1.1.2/setup.py
+drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-05-07 02:48:11.359733 datalibro_backend-1.1.3/
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     1070 2023-12-08 09:34:06.000000 datalibro_backend-1.1.3/LICENSE.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-05-07 02:48:11.357417 datalibro_backend-1.1.3/PKG-INFO
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     1683 2023-12-08 09:30:25.000000 datalibro_backend-1.1.3/README.md
+drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-05-07 02:48:11.352096 datalibro_backend-1.1.3/datalibro_backend/
+-rw-r--r--   0 zhoulucy   (501) staff       (20)      207 2024-02-01 06:19:04.000000 datalibro_backend-1.1.3/datalibro_backend/__init__.py
+-rw-r--r--   0 zhoulucy   (501) staff       (20)    15308 2024-04-18 06:06:10.000000 datalibro_backend-1.1.3/datalibro_backend/quality_check.py
+-rw-r--r--   0 zhoulucy   (501) staff       (20)    10977 2024-05-07 01:58:43.000000 datalibro_backend-1.1.3/datalibro_backend/read_file.py
+drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-05-07 02:48:11.355596 datalibro_backend-1.1.3/datalibro_backend.egg-info/
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-05-07 02:48:06.000000 datalibro_backend-1.1.3/datalibro_backend.egg-info/PKG-INFO
+-rw-r--r--   0 zhoulucy   (501) staff       (20)      290 2024-05-07 02:48:07.000000 datalibro_backend-1.1.3/datalibro_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)        1 2024-05-07 02:48:06.000000 datalibro_backend-1.1.3/datalibro_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)       18 2024-05-07 02:48:06.000000 datalibro_backend-1.1.3/datalibro_backend.egg-info/top_level.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)       38 2024-05-07 02:48:11.359964 datalibro_backend-1.1.3/setup.cfg
+-rw-r--r--   0 zhoulucy   (501) staff       (20)      594 2024-05-07 02:02:56.000000 datalibro_backend-1.1.3/setup.py
```

### Comparing `datalibro_backend-1.1.2/LICENSE.txt` & `datalibro_backend-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datalibro_backend-1.1.2/PKG-INFO` & `datalibro_backend-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalibro_backend
-Version: 1.1.2
+Version: 1.1.3
 Summary: A small package for your backend service
 Home-page: https://github.com/DesignLibro/datalibro_backend
 Author: lucy
 Author-email: lucy@petlibro.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datalibro_backend-1.1.2/README.md` & `datalibro_backend-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `datalibro_backend-1.1.2/datalibro_backend/quality_check.py` & `datalibro_backend-1.1.3/datalibro_backend/quality_check.py`

 * *Files identical despite different names*

### Comparing `datalibro_backend-1.1.2/datalibro_backend.egg-info/PKG-INFO` & `datalibro_backend-1.1.3/datalibro_backend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalibro-backend
-Version: 1.1.2
+Version: 1.1.3
 Summary: A small package for your backend service
 Home-page: https://github.com/DesignLibro/datalibro_backend
 Author: lucy
 Author-email: lucy@petlibro.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datalibro_backend-1.1.2/setup.py` & `datalibro_backend-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="datalibro_backend",
-  version="1.1.2",
+  version="1.1.3",
   author="lucy",
   author_email="lucy@petlibro.com",
   description="A small package for your backend service",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/DesignLibro/datalibro_backend",
   packages=setuptools.find_packages(),
```

