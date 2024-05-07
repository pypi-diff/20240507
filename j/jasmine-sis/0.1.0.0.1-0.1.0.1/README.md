# Comparing `tmp/jasmine_sis-0.1.0.0.1.tar.gz` & `tmp/jasmine_sis-0.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jasmine_sis-0.1.0.0.1.tar", last modified: Tue May  7 20:56:25 2024, max compression
+gzip compressed data, was "jasmine_sis-0.1.0.1.tar", last modified: Tue May  7 20:53:46 2024, max compression
```

## Comparing `jasmine_sis-0.1.0.0.1.tar` & `jasmine_sis-0.1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 sishitan (344948379) staff       (20)        0 2024-05-07 20:56:25.455903 jasmine_sis-0.1.0.0.1/
--rw-r--r--   0 sishitan (344948379) staff       (20)     1065 2024-04-17 18:49:24.000000 jasmine_sis-0.1.0.0.1/LICENSE
--rw-r--r--   0 sishitan (344948379) staff       (20)      437 2024-05-07 20:56:25.455228 jasmine_sis-0.1.0.0.1/PKG-INFO
--rw-r--r--   0 sishitan (344948379) staff       (20)     2077 2024-05-01 23:08:17.000000 jasmine_sis-0.1.0.0.1/README.md
-drwxr-xr-x   0 sishitan (344948379) staff       (20)        0 2024-05-07 20:56:25.454498 jasmine_sis-0.1.0.0.1/jasmine_sis.egg-info/
--rw-r--r--   0 sishitan (344948379) staff       (20)      437 2024-05-07 20:56:25.000000 jasmine_sis-0.1.0.0.1/jasmine_sis.egg-info/PKG-INFO
--rw-r--r--   0 sishitan (344948379) staff       (20)      234 2024-05-07 20:56:25.000000 jasmine_sis-0.1.0.0.1/jasmine_sis.egg-info/SOURCES.txt
--rw-r--r--   0 sishitan (344948379) staff       (20)        1 2024-05-07 20:56:25.000000 jasmine_sis-0.1.0.0.1/jasmine_sis.egg-info/dependency_links.txt
--rw-r--r--   0 sishitan (344948379) staff       (20)        1 2024-05-07 20:48:18.000000 jasmine_sis-0.1.0.0.1/jasmine_sis.egg-info/not-zip-safe
--rw-r--r--   0 sishitan (344948379) staff       (20)       81 2024-05-07 20:56:25.000000 jasmine_sis-0.1.0.0.1/jasmine_sis.egg-info/requires.txt
--rw-r--r--   0 sishitan (344948379) staff       (20)        8 2024-05-07 20:56:25.000000 jasmine_sis-0.1.0.0.1/jasmine_sis.egg-info/top_level.txt
--rw-r--r--   0 sishitan (344948379) staff       (20)       38 2024-05-07 20:56:25.456006 jasmine_sis-0.1.0.0.1/setup.cfg
--rw-r--r--   0 sishitan (344948379) staff       (20)      613 2024-05-07 20:56:14.000000 jasmine_sis-0.1.0.0.1/setup.py
+drwxr-xr-x   0 sishitan (344948379) staff       (20)        0 2024-05-07 20:53:46.324549 jasmine_sis-0.1.0.1/
+-rw-r--r--   0 sishitan (344948379) staff       (20)     1065 2024-04-17 18:49:24.000000 jasmine_sis-0.1.0.1/LICENSE
+-rw-r--r--   0 sishitan (344948379) staff       (20)      435 2024-05-07 20:53:46.324005 jasmine_sis-0.1.0.1/PKG-INFO
+-rw-r--r--   0 sishitan (344948379) staff       (20)     2077 2024-05-01 23:08:17.000000 jasmine_sis-0.1.0.1/README.md
+drwxr-xr-x   0 sishitan (344948379) staff       (20)        0 2024-05-07 20:53:46.323357 jasmine_sis-0.1.0.1/jasmine_sis.egg-info/
+-rw-r--r--   0 sishitan (344948379) staff       (20)      435 2024-05-07 20:53:46.000000 jasmine_sis-0.1.0.1/jasmine_sis.egg-info/PKG-INFO
+-rw-r--r--   0 sishitan (344948379) staff       (20)      234 2024-05-07 20:53:46.000000 jasmine_sis-0.1.0.1/jasmine_sis.egg-info/SOURCES.txt
+-rw-r--r--   0 sishitan (344948379) staff       (20)        1 2024-05-07 20:53:46.000000 jasmine_sis-0.1.0.1/jasmine_sis.egg-info/dependency_links.txt
+-rw-r--r--   0 sishitan (344948379) staff       (20)        1 2024-05-07 20:48:18.000000 jasmine_sis-0.1.0.1/jasmine_sis.egg-info/not-zip-safe
+-rw-r--r--   0 sishitan (344948379) staff       (20)       81 2024-05-07 20:53:46.000000 jasmine_sis-0.1.0.1/jasmine_sis.egg-info/requires.txt
+-rw-r--r--   0 sishitan (344948379) staff       (20)        8 2024-05-07 20:53:46.000000 jasmine_sis-0.1.0.1/jasmine_sis.egg-info/top_level.txt
+-rw-r--r--   0 sishitan (344948379) staff       (20)       38 2024-05-07 20:53:46.324662 jasmine_sis-0.1.0.1/setup.cfg
+-rw-r--r--   0 sishitan (344948379) staff       (20)      611 2024-05-07 20:53:41.000000 jasmine_sis-0.1.0.1/setup.py
```

### Comparing `jasmine_sis-0.1.0.0.1/LICENSE` & `jasmine_sis-0.1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jasmine_sis-0.1.0.0.1/README.md` & `jasmine_sis-0.1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `jasmine_sis-0.1.0.0.1/setup.py` & `jasmine_sis-0.1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='jasmine-sis',
-      version='0.1.0.0.1',
+      version='0.1.0.1',
       description='JASMINE: Joint Analysis of Simulations for Microlensing INterest Events',
       url='https://github.com/stelais/jasmine',
       author='Stela IS',
       author_email='stela.ishitanisilva@nasa.gov',
       license='MIT',
       packages=['jasmine'],
       zip_safe=False,
```

