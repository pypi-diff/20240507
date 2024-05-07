# Comparing `tmp/data-quality-validation-pydeequ-0.4.tar.gz` & `tmp/data-quality-validation-pydeequ-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-quality-validation-pydeequ-0.4.tar", last modified: Tue May  7 03:28:49 2024, max compression
+gzip compressed data, was "data-quality-validation-pydeequ-0.5.tar", last modified: Tue May  7 04:01:07 2024, max compression
```

## Comparing `data-quality-validation-pydeequ-0.4.tar` & `data-quality-validation-pydeequ-0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 03:28:49.912001 data-quality-validation-pydeequ-0.4/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     4175 2024-05-07 03:28:49.911622 data-quality-validation-pydeequ-0.4/PKG-INFO
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     3695 2024-05-07 03:27:51.000000 data-quality-validation-pydeequ-0.4/README.md
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 03:28:49.911187 data-quality-validation-pydeequ-0.4/data_quality_validation_pydeequ.egg-info/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     4175 2024-05-07 03:28:49.000000 data-quality-validation-pydeequ-0.4/data_quality_validation_pydeequ.egg-info/PKG-INFO
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)      366 2024-05-07 03:28:49.000000 data-quality-validation-pydeequ-0.4/data_quality_validation_pydeequ.egg-info/SOURCES.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        1 2024-05-07 03:28:49.000000 data-quality-validation-pydeequ-0.4/data_quality_validation_pydeequ.egg-info/dependency_links.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)       28 2024-05-07 03:28:49.000000 data-quality-validation-pydeequ-0.4/data_quality_validation_pydeequ.egg-info/requires.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        4 2024-05-07 03:28:49.000000 data-quality-validation-pydeequ-0.4/data_quality_validation_pydeequ.egg-info/top_level.txt
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 03:28:49.910476 data-quality-validation-pydeequ-0.4/dqv/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 06:16:20.000000 data-quality-validation-pydeequ-0.4/dqv/__init__.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)    11706 2024-05-06 09:17:04.000000 data-quality-validation-pydeequ-0.4/dqv/data_quality_validation_pydeequ.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     1650 2024-05-06 09:01:46.000000 data-quality-validation-pydeequ-0.4/dqv/dqv_pydeequ.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)       38 2024-05-07 03:28:49.912064 data-quality-validation-pydeequ-0.4/setup.cfg
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)      826 2024-05-07 03:28:47.000000 data-quality-validation-pydeequ-0.4/setup.py
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 04:01:07.053671 data-quality-validation-pydeequ-0.5/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     5889 2024-05-07 04:01:07.053284 data-quality-validation-pydeequ-0.5/PKG-INFO
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     5408 2024-05-07 04:00:37.000000 data-quality-validation-pydeequ-0.5/README.md
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 04:01:07.052724 data-quality-validation-pydeequ-0.5/data_quality_validation_pydeequ.egg-info/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     5889 2024-05-07 04:01:06.000000 data-quality-validation-pydeequ-0.5/data_quality_validation_pydeequ.egg-info/PKG-INFO
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)      366 2024-05-07 04:01:07.000000 data-quality-validation-pydeequ-0.5/data_quality_validation_pydeequ.egg-info/SOURCES.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        1 2024-05-07 04:01:06.000000 data-quality-validation-pydeequ-0.5/data_quality_validation_pydeequ.egg-info/dependency_links.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)       28 2024-05-07 04:01:06.000000 data-quality-validation-pydeequ-0.5/data_quality_validation_pydeequ.egg-info/requires.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        4 2024-05-07 04:01:06.000000 data-quality-validation-pydeequ-0.5/data_quality_validation_pydeequ.egg-info/top_level.txt
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 04:01:07.051800 data-quality-validation-pydeequ-0.5/dqv/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 06:16:20.000000 data-quality-validation-pydeequ-0.5/dqv/__init__.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)    11706 2024-05-06 09:17:04.000000 data-quality-validation-pydeequ-0.5/dqv/data_quality_validation_pydeequ.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     1650 2024-05-06 09:01:46.000000 data-quality-validation-pydeequ-0.5/dqv/dqv_pydeequ.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)       38 2024-05-07 04:01:07.053747 data-quality-validation-pydeequ-0.5/setup.cfg
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)      826 2024-05-07 04:01:05.000000 data-quality-validation-pydeequ-0.5/setup.py
```

### Comparing `data-quality-validation-pydeequ-0.4/dqv/data_quality_validation_pydeequ.py` & `data-quality-validation-pydeequ-0.5/dqv/data_quality_validation_pydeequ.py`

 * *Files identical despite different names*

### Comparing `data-quality-validation-pydeequ-0.4/dqv/dqv_pydeequ.py` & `data-quality-validation-pydeequ-0.5/dqv/dqv_pydeequ.py`

 * *Files identical despite different names*

### Comparing `data-quality-validation-pydeequ-0.4/setup.py` & `data-quality-validation-pydeequ-0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Reading the README.md file for long description in PyPI site
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='data-quality-validation-pydeequ',
-    version='0.4',
+    version='0.5',
     author='Ketan Kirange',
     author_email='k.kirange@reply.com',
     description='A library for data quality validation using PyDeequ.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

