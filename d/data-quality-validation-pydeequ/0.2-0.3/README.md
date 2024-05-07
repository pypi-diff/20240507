# Comparing `tmp/data-quality-validation-pydeequ-0.2.tar.gz` & `tmp/data-quality-validation-pydeequ-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-quality-validation-pydeequ-0.2.tar", last modified: Mon May  6 09:55:28 2024, max compression
+gzip compressed data, was "data-quality-validation-pydeequ-0.3.tar", last modified: Tue May  7 03:08:38 2024, max compression
```

## Comparing `data-quality-validation-pydeequ-0.2.tar` & `data-quality-validation-pydeequ-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 09:55:28.847597 data-quality-validation-pydeequ-0.2/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)      439 2024-05-06 09:55:28.847151 data-quality-validation-pydeequ-0.2/PKG-INFO
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     3218 2024-05-06 06:17:24.000000 data-quality-validation-pydeequ-0.2/README.md
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 09:55:28.846562 data-quality-validation-pydeequ-0.2/data_quality_validation_pydeequ.egg-info/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)      439 2024-05-06 09:55:28.000000 data-quality-validation-pydeequ-0.2/data_quality_validation_pydeequ.egg-info/PKG-INFO
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)      366 2024-05-06 09:55:28.000000 data-quality-validation-pydeequ-0.2/data_quality_validation_pydeequ.egg-info/SOURCES.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        1 2024-05-06 09:55:28.000000 data-quality-validation-pydeequ-0.2/data_quality_validation_pydeequ.egg-info/dependency_links.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)       28 2024-05-06 09:55:28.000000 data-quality-validation-pydeequ-0.2/data_quality_validation_pydeequ.egg-info/requires.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        4 2024-05-06 09:55:28.000000 data-quality-validation-pydeequ-0.2/data_quality_validation_pydeequ.egg-info/top_level.txt
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 09:55:28.844797 data-quality-validation-pydeequ-0.2/dqv/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 06:16:20.000000 data-quality-validation-pydeequ-0.2/dqv/__init__.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)    11706 2024-05-06 09:17:04.000000 data-quality-validation-pydeequ-0.2/dqv/data_quality_validation_pydeequ.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     1650 2024-05-06 09:01:46.000000 data-quality-validation-pydeequ-0.2/dqv/dqv_pydeequ.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)       38 2024-05-06 09:55:28.847667 data-quality-validation-pydeequ-0.2/setup.cfg
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)      586 2024-05-06 09:24:21.000000 data-quality-validation-pydeequ-0.2/setup.py
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 03:08:38.064651 data-quality-validation-pydeequ-0.3/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)      573 2024-05-07 03:08:38.064224 data-quality-validation-pydeequ-0.3/PKG-INFO
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     3218 2024-05-06 06:17:24.000000 data-quality-validation-pydeequ-0.3/README.md
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 03:08:38.063597 data-quality-validation-pydeequ-0.3/data_quality_validation_pydeequ.egg-info/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)      573 2024-05-07 03:08:37.000000 data-quality-validation-pydeequ-0.3/data_quality_validation_pydeequ.egg-info/PKG-INFO
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)      366 2024-05-07 03:08:38.000000 data-quality-validation-pydeequ-0.3/data_quality_validation_pydeequ.egg-info/SOURCES.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        1 2024-05-07 03:08:37.000000 data-quality-validation-pydeequ-0.3/data_quality_validation_pydeequ.egg-info/dependency_links.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)       28 2024-05-07 03:08:37.000000 data-quality-validation-pydeequ-0.3/data_quality_validation_pydeequ.egg-info/requires.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        4 2024-05-07 03:08:37.000000 data-quality-validation-pydeequ-0.3/data_quality_validation_pydeequ.egg-info/top_level.txt
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 03:08:38.062210 data-quality-validation-pydeequ-0.3/dqv/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 06:16:20.000000 data-quality-validation-pydeequ-0.3/dqv/__init__.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)    11706 2024-05-06 09:17:04.000000 data-quality-validation-pydeequ-0.3/dqv/data_quality_validation_pydeequ.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     1650 2024-05-06 09:01:46.000000 data-quality-validation-pydeequ-0.3/dqv/dqv_pydeequ.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)       38 2024-05-07 03:08:38.064721 data-quality-validation-pydeequ-0.3/setup.cfg
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)      754 2024-05-07 03:08:31.000000 data-quality-validation-pydeequ-0.3/setup.py
```

### Comparing `data-quality-validation-pydeequ-0.2/README.md` & `data-quality-validation-pydeequ-0.3/README.md`

 * *Files identical despite different names*

### Comparing `data-quality-validation-pydeequ-0.2/dqv/data_quality_validation_pydeequ.py` & `data-quality-validation-pydeequ-0.3/dqv/data_quality_validation_pydeequ.py`

 * *Files identical despite different names*

### Comparing `data-quality-validation-pydeequ-0.2/dqv/dqv_pydeequ.py` & `data-quality-validation-pydeequ-0.3/dqv/dqv_pydeequ.py`

 * *Files identical despite different names*

### Comparing `data-quality-validation-pydeequ-0.2/setup.py` & `data-quality-validation-pydeequ-0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='data-quality-validation-pydeequ',
-    version='0.2',
+    version='0.3',
     author='Ketan Kirange',
     author_email='k.kirange@reply.com',
     description='A library for data quality validation using PyDeequ.',
+    long_description='A Python library that provides classes for performing data quality validation using Pydeequ.',
+    long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'pandas',
         'pydeequ',
         'boto3',
         'pyyaml',  
     ],
```

