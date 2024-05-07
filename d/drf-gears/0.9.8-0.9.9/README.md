# Comparing `tmp/drf-gears-0.9.8.tar.gz` & `tmp/drf-gears-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-gears-0.9.8.tar", last modified: Sat Mar 16 22:01:38 2024, max compression
+gzip compressed data, was "drf-gears-0.9.9.tar", last modified: Sat Mar 16 22:13:42 2024, max compression
```

## Comparing `drf-gears-0.9.8.tar` & `drf-gears-0.9.9.tar`

### file list

```diff
@@ -1,50 +1,54 @@
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-03-16 22:01:38.023827 drf-gears-0.9.8/
--rw-r--r--   0 alexander   (501) staff       (20)     1069 2022-08-31 14:23:16.000000 drf-gears-0.9.8/LICENSE
--rw-r--r--   0 alexander   (501) staff       (20)     8675 2024-03-16 22:01:38.023717 drf-gears-0.9.8/PKG-INFO
--rw-r--r--   0 alexander   (501) staff       (20)     8080 2022-08-31 06:54:14.000000 drf-gears-0.9.8/README.md
--rw-r--r--   0 alexander   (501) staff       (20)       79 2024-03-16 22:01:38.024058 drf-gears-0.9.8/setup.cfg
--rw-r--r--   0 alexander   (501) staff       (20)      928 2024-03-16 22:01:35.000000 drf-gears-0.9.8/setup.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-03-16 22:01:38.016789 drf-gears-0.9.8/src/
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-03-16 22:01:38.018657 drf-gears-0.9.8/src/drf_gears.egg-info/
--rw-r--r--   0 alexander   (501) staff       (20)     8675 2024-03-16 22:01:37.000000 drf-gears-0.9.8/src/drf_gears.egg-info/PKG-INFO
--rw-r--r--   0 alexander   (501) staff       (20)     1037 2024-03-16 22:01:37.000000 drf-gears-0.9.8/src/drf_gears.egg-info/SOURCES.txt
--rw-r--r--   0 alexander   (501) staff       (20)        1 2024-03-16 22:01:37.000000 drf-gears-0.9.8/src/drf_gears.egg-info/dependency_links.txt
--rw-r--r--   0 alexander   (501) staff       (20)        6 2024-03-16 22:01:37.000000 drf-gears-0.9.8/src/drf_gears.egg-info/top_level.txt
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-03-16 22:01:38.019362 drf-gears-0.9.8/src/gears/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 17:27:25.000000 drf-gears-0.9.8/src/gears/__init__.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-03-16 22:01:38.019690 drf-gears-0.9.8/src/gears/admin/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2023-11-30 07:10:55.000000 drf-gears-0.9.8/src/gears/admin/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)      820 2023-11-30 07:13:52.000000 drf-gears-0.9.8/src/gears/admin/singleton.py
--rw-r--r--   0 alexander   (501) staff       (20)       43 2022-08-31 14:30:39.000000 drf-gears-0.9.8/src/gears/example.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-03-16 22:01:38.019974 drf-gears-0.9.8/src/gears/management/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2023-09-29 18:48:34.000000 drf-gears-0.9.8/src/gears/management/__init__.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-03-16 22:01:38.020172 drf-gears-0.9.8/src/gears/management/commands/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2023-09-29 18:48:57.000000 drf-gears-0.9.8/src/gears/management/commands/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)     3269 2023-09-30 09:46:47.000000 drf-gears-0.9.8/src/gears/management/commands/run_gears_server.py
--rw-r--r--   0 alexander   (501) staff       (20)      523 2022-08-22 18:21:05.000000 drf-gears-0.9.8/src/gears/mixins.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-03-16 22:01:38.021047 drf-gears-0.9.8/src/gears/models/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 16:41:07.000000 drf-gears-0.9.8/src/gears/models/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)     7321 2024-01-11 23:08:40.000000 drf-gears-0.9.8/src/gears/models/change.py
--rw-r--r--   0 alexander   (501) staff       (20)     3669 2022-08-31 20:29:26.000000 drf-gears-0.9.8/src/gears/models/jwt.py
--rw-r--r--   0 alexander   (501) staff       (20)      993 2022-09-15 17:18:53.000000 drf-gears-0.9.8/src/gears/models/singleton.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-03-16 22:01:38.021432 drf-gears-0.9.8/src/gears/pagination/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2024-03-15 16:37:46.000000 drf-gears-0.9.8/src/gears/pagination/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)     1017 2024-03-15 17:00:12.000000 drf-gears-0.9.8/src/gears/pagination/summary.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-03-16 22:01:38.022153 drf-gears-0.9.8/src/gears/renderers/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 16:39:27.000000 drf-gears-0.9.8/src/gears/renderers/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)     3346 2023-02-28 09:58:58.000000 drf-gears-0.9.8/src/gears/renderers/exception_handlers.py
--rw-r--r--   0 alexander   (501) staff       (20)      314 2022-08-31 16:39:41.000000 drf-gears-0.9.8/src/gears/renderers/mapping.py
--rw-r--r--   0 alexander   (501) staff       (20)     2021 2024-03-16 22:01:10.000000 drf-gears-0.9.8/src/gears/renderers/renderer.py
--rw-r--r--   0 alexander   (501) staff       (20)      427 2024-03-15 20:18:52.000000 drf-gears-0.9.8/src/gears/renderers/types.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-03-16 22:01:38.022477 drf-gears-0.9.8/src/gears/serializers/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 16:41:07.000000 drf-gears-0.9.8/src/gears/serializers/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)      481 2022-08-31 16:40:18.000000 drf-gears-0.9.8/src/gears/serializers/jwt.py
--rw-r--r--   0 alexander   (501) staff       (20)      332 2023-09-29 19:39:48.000000 drf-gears-0.9.8/src/gears/settings.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-03-16 22:01:38.022728 drf-gears-0.9.8/src/gears/views/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 16:41:07.000000 drf-gears-0.9.8/src/gears/views/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)      353 2022-08-31 20:02:15.000000 drf-gears-0.9.8/src/gears/views/jwt.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-03-16 22:01:38.023380 drf-gears-0.9.8/src/gears/viewsets/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 16:41:07.000000 drf-gears-0.9.8/src/gears/viewsets/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)      724 2022-08-31 16:40:43.000000 drf-gears-0.9.8/src/gears/viewsets/permissions.py
--rw-r--r--   0 alexander   (501) staff       (20)     1096 2022-08-31 16:40:48.000000 drf-gears-0.9.8/src/gears/viewsets/querysets.py
--rw-r--r--   0 alexander   (501) staff       (20)     1153 2022-08-31 16:40:56.000000 drf-gears-0.9.8/src/gears/viewsets/serializers.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-03-16 22:13:42.575122 drf-gears-0.9.9/
+-rw-r--r--   0 alexander   (501) staff       (20)     1069 2022-08-31 14:23:16.000000 drf-gears-0.9.9/LICENSE
+-rw-r--r--   0 alexander   (501) staff       (20)     8675 2024-03-16 22:13:42.574960 drf-gears-0.9.9/PKG-INFO
+-rw-r--r--   0 alexander   (501) staff       (20)     8080 2022-08-31 06:54:14.000000 drf-gears-0.9.9/README.md
+-rw-r--r--   0 alexander   (501) staff       (20)       79 2024-03-16 22:13:42.575363 drf-gears-0.9.9/setup.cfg
+-rw-r--r--   0 alexander   (501) staff       (20)      928 2024-03-16 22:13:19.000000 drf-gears-0.9.9/setup.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-03-16 22:13:42.565254 drf-gears-0.9.9/src/
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-03-16 22:13:42.567366 drf-gears-0.9.9/src/drf_gears.egg-info/
+-rw-r--r--   0 alexander   (501) staff       (20)     8675 2024-03-16 22:13:42.000000 drf-gears-0.9.9/src/drf_gears.egg-info/PKG-INFO
+-rw-r--r--   0 alexander   (501) staff       (20)     1135 2024-03-16 22:13:42.000000 drf-gears-0.9.9/src/drf_gears.egg-info/SOURCES.txt
+-rw-r--r--   0 alexander   (501) staff       (20)        1 2024-03-16 22:13:42.000000 drf-gears-0.9.9/src/drf_gears.egg-info/dependency_links.txt
+-rw-r--r--   0 alexander   (501) staff       (20)        6 2024-03-16 22:13:42.000000 drf-gears-0.9.9/src/drf_gears.egg-info/top_level.txt
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-03-16 22:13:42.567812 drf-gears-0.9.9/src/gears/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 17:27:25.000000 drf-gears-0.9.9/src/gears/__init__.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-03-16 22:13:42.568160 drf-gears-0.9.9/src/gears/admin/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2023-11-30 07:10:55.000000 drf-gears-0.9.9/src/gears/admin/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)      820 2023-11-30 07:13:52.000000 drf-gears-0.9.9/src/gears/admin/singleton.py
+-rw-r--r--   0 alexander   (501) staff       (20)       43 2022-08-31 14:30:39.000000 drf-gears-0.9.9/src/gears/example.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-03-16 22:13:42.568375 drf-gears-0.9.9/src/gears/exceptions/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2024-03-16 22:11:31.000000 drf-gears-0.9.9/src/gears/exceptions/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)       46 2024-03-16 22:13:19.000000 drf-gears-0.9.9/src/gears/exceptions/views.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-03-16 22:13:42.568487 drf-gears-0.9.9/src/gears/management/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2023-09-29 18:48:34.000000 drf-gears-0.9.9/src/gears/management/__init__.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-03-16 22:13:42.568696 drf-gears-0.9.9/src/gears/management/commands/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2023-09-29 18:48:57.000000 drf-gears-0.9.9/src/gears/management/commands/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)     3269 2023-09-30 09:46:47.000000 drf-gears-0.9.9/src/gears/management/commands/run_gears_server.py
+-rw-r--r--   0 alexander   (501) staff       (20)      523 2022-08-22 18:21:05.000000 drf-gears-0.9.9/src/gears/mixins.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-03-16 22:13:42.569581 drf-gears-0.9.9/src/gears/models/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 16:41:07.000000 drf-gears-0.9.9/src/gears/models/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)     7321 2024-01-11 23:08:40.000000 drf-gears-0.9.9/src/gears/models/change.py
+-rw-r--r--   0 alexander   (501) staff       (20)     3669 2022-08-31 20:29:26.000000 drf-gears-0.9.9/src/gears/models/jwt.py
+-rw-r--r--   0 alexander   (501) staff       (20)      993 2022-09-15 17:18:53.000000 drf-gears-0.9.9/src/gears/models/singleton.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-03-16 22:13:42.569798 drf-gears-0.9.9/src/gears/pagination/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2024-03-15 16:37:46.000000 drf-gears-0.9.9/src/gears/pagination/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1017 2024-03-15 17:00:12.000000 drf-gears-0.9.9/src/gears/pagination/summary.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-03-16 22:13:42.570470 drf-gears-0.9.9/src/gears/renderers/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 16:39:27.000000 drf-gears-0.9.9/src/gears/renderers/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)     3346 2023-02-28 09:58:58.000000 drf-gears-0.9.9/src/gears/renderers/exception_handlers.py
+-rw-r--r--   0 alexander   (501) staff       (20)      314 2022-08-31 16:39:41.000000 drf-gears-0.9.9/src/gears/renderers/mapping.py
+-rw-r--r--   0 alexander   (501) staff       (20)     2021 2024-03-16 22:01:10.000000 drf-gears-0.9.9/src/gears/renderers/renderer.py
+-rw-r--r--   0 alexander   (501) staff       (20)      427 2024-03-15 20:18:52.000000 drf-gears-0.9.9/src/gears/renderers/types.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-03-16 22:13:42.570824 drf-gears-0.9.9/src/gears/serializers/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 16:41:07.000000 drf-gears-0.9.9/src/gears/serializers/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)      481 2022-08-31 16:40:18.000000 drf-gears-0.9.9/src/gears/serializers/jwt.py
+-rw-r--r--   0 alexander   (501) staff       (20)      332 2023-09-29 19:39:48.000000 drf-gears-0.9.9/src/gears/settings.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-03-16 22:13:42.573635 drf-gears-0.9.9/src/gears/views/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 16:41:07.000000 drf-gears-0.9.9/src/gears/views/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)      353 2022-08-31 20:02:15.000000 drf-gears-0.9.9/src/gears/views/jwt.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-03-16 22:13:42.574602 drf-gears-0.9.9/src/gears/viewsets/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 16:41:07.000000 drf-gears-0.9.9/src/gears/viewsets/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)      724 2022-08-31 16:40:43.000000 drf-gears-0.9.9/src/gears/viewsets/permissions.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1096 2022-08-31 16:40:48.000000 drf-gears-0.9.9/src/gears/viewsets/querysets.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1153 2022-08-31 16:40:56.000000 drf-gears-0.9.9/src/gears/viewsets/serializers.py
+-rw-r--r--   0 alexander   (501) staff       (20)      423 2024-03-16 22:13:19.000000 drf-gears-0.9.9/src/gears/viewsets/service_data.py
```

### Comparing `drf-gears-0.9.8/LICENSE` & `drf-gears-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-gears-0.9.8/PKG-INFO` & `drf-gears-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-gears
-Version: 0.9.8
+Version: 0.9.9
 Summary: Some gears collection for getting life a little bit better.
 Home-page: https://github.com/san4ezy/drf-gears
 Author: Alexander Yudkin
 Author-email: san4ezy@gmail.com
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `drf-gears-0.9.8/README.md` & `drf-gears-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `drf-gears-0.9.8/setup.py` & `drf-gears-0.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="drf-gears",
-    version="0.9.8",
+    version="0.9.9",
     author="Alexander Yudkin",
     author_email="san4ezy@gmail.com",
     description="Some gears collection for getting life a little bit better.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/san4ezy/drf-gears",
     packages=setuptools.find_packages(where='src'),
```

### Comparing `drf-gears-0.9.8/src/drf_gears.egg-info/PKG-INFO` & `drf-gears-0.9.9/src/drf_gears.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-gears
-Version: 0.9.8
+Version: 0.9.9
 Summary: Some gears collection for getting life a little bit better.
 Home-page: https://github.com/san4ezy/drf-gears
 Author: Alexander Yudkin
 Author-email: san4ezy@gmail.com
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `drf-gears-0.9.8/src/drf_gears.egg-info/SOURCES.txt` & `drf-gears-0.9.9/src/drf_gears.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 src/drf_gears.egg-info/top_level.txt
 src/gears/__init__.py
 src/gears/example.py
 src/gears/mixins.py
 src/gears/settings.py
 src/gears/admin/__init__.py
 src/gears/admin/singleton.py
+src/gears/exceptions/__init__.py
+src/gears/exceptions/views.py
 src/gears/management/__init__.py
 src/gears/management/commands/__init__.py
 src/gears/management/commands/run_gears_server.py
 src/gears/models/__init__.py
 src/gears/models/change.py
 src/gears/models/jwt.py
 src/gears/models/singleton.py
@@ -29,8 +31,9 @@
 src/gears/serializers/__init__.py
 src/gears/serializers/jwt.py
 src/gears/views/__init__.py
 src/gears/views/jwt.py
 src/gears/viewsets/__init__.py
 src/gears/viewsets/permissions.py
 src/gears/viewsets/querysets.py
-src/gears/viewsets/serializers.py
+src/gears/viewsets/serializers.py
+src/gears/viewsets/service_data.py
```

### Comparing `drf-gears-0.9.8/src/gears/admin/singleton.py` & `drf-gears-0.9.9/src/gears/admin/singleton.py`

 * *Files identical despite different names*

### Comparing `drf-gears-0.9.8/src/gears/management/commands/run_gears_server.py` & `drf-gears-0.9.9/src/gears/management/commands/run_gears_server.py`

 * *Files identical despite different names*

### Comparing `drf-gears-0.9.8/src/gears/mixins.py` & `drf-gears-0.9.9/src/gears/mixins.py`

 * *Files identical despite different names*

### Comparing `drf-gears-0.9.8/src/gears/models/change.py` & `drf-gears-0.9.9/src/gears/models/change.py`

 * *Files identical despite different names*

### Comparing `drf-gears-0.9.8/src/gears/models/jwt.py` & `drf-gears-0.9.9/src/gears/models/jwt.py`

 * *Files identical despite different names*

### Comparing `drf-gears-0.9.8/src/gears/models/singleton.py` & `drf-gears-0.9.9/src/gears/models/singleton.py`

 * *Files identical despite different names*

### Comparing `drf-gears-0.9.8/src/gears/pagination/summary.py` & `drf-gears-0.9.9/src/gears/pagination/summary.py`

 * *Files identical despite different names*

### Comparing `drf-gears-0.9.8/src/gears/renderers/exception_handlers.py` & `drf-gears-0.9.9/src/gears/renderers/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `drf-gears-0.9.8/src/gears/renderers/renderer.py` & `drf-gears-0.9.9/src/gears/renderers/renderer.py`

 * *Files identical despite different names*

### Comparing `drf-gears-0.9.8/src/gears/viewsets/permissions.py` & `drf-gears-0.9.9/src/gears/viewsets/permissions.py`

 * *Files identical despite different names*

### Comparing `drf-gears-0.9.8/src/gears/viewsets/querysets.py` & `drf-gears-0.9.9/src/gears/viewsets/querysets.py`

 * *Files identical despite different names*

### Comparing `drf-gears-0.9.8/src/gears/viewsets/serializers.py` & `drf-gears-0.9.9/src/gears/viewsets/serializers.py`

 * *Files identical despite different names*

