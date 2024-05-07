# Comparing `tmp/data-quality-validation-pydeequ-0.5.tar.gz` & `tmp/data-quality-validation-pydeequ-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-quality-validation-pydeequ-0.5.tar", last modified: Tue May  7 04:01:07 2024, max compression
+gzip compressed data, was "data-quality-validation-pydeequ-0.6.tar", last modified: Tue May  7 05:53:17 2024, max compression
```

## Comparing `data-quality-validation-pydeequ-0.5.tar` & `data-quality-validation-pydeequ-0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 04:01:07.053671 data-quality-validation-pydeequ-0.5/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     5889 2024-05-07 04:01:07.053284 data-quality-validation-pydeequ-0.5/PKG-INFO
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     5408 2024-05-07 04:00:37.000000 data-quality-validation-pydeequ-0.5/README.md
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 04:01:07.052724 data-quality-validation-pydeequ-0.5/data_quality_validation_pydeequ.egg-info/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     5889 2024-05-07 04:01:06.000000 data-quality-validation-pydeequ-0.5/data_quality_validation_pydeequ.egg-info/PKG-INFO
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)      366 2024-05-07 04:01:07.000000 data-quality-validation-pydeequ-0.5/data_quality_validation_pydeequ.egg-info/SOURCES.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        1 2024-05-07 04:01:06.000000 data-quality-validation-pydeequ-0.5/data_quality_validation_pydeequ.egg-info/dependency_links.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)       28 2024-05-07 04:01:06.000000 data-quality-validation-pydeequ-0.5/data_quality_validation_pydeequ.egg-info/requires.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        4 2024-05-07 04:01:06.000000 data-quality-validation-pydeequ-0.5/data_quality_validation_pydeequ.egg-info/top_level.txt
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 04:01:07.051800 data-quality-validation-pydeequ-0.5/dqv/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 06:16:20.000000 data-quality-validation-pydeequ-0.5/dqv/__init__.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)    11706 2024-05-06 09:17:04.000000 data-quality-validation-pydeequ-0.5/dqv/data_quality_validation_pydeequ.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     1650 2024-05-06 09:01:46.000000 data-quality-validation-pydeequ-0.5/dqv/dqv_pydeequ.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)       38 2024-05-07 04:01:07.053747 data-quality-validation-pydeequ-0.5/setup.cfg
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)      826 2024-05-07 04:01:05.000000 data-quality-validation-pydeequ-0.5/setup.py
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 05:53:17.905751 data-quality-validation-pydeequ-0.6/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     6067 2024-05-07 05:53:17.905298 data-quality-validation-pydeequ-0.6/PKG-INFO
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     5586 2024-05-07 05:53:03.000000 data-quality-validation-pydeequ-0.6/README.md
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 05:53:17.904823 data-quality-validation-pydeequ-0.6/data_quality_validation_pydeequ.egg-info/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     6067 2024-05-07 05:53:17.000000 data-quality-validation-pydeequ-0.6/data_quality_validation_pydeequ.egg-info/PKG-INFO
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)      366 2024-05-07 05:53:17.000000 data-quality-validation-pydeequ-0.6/data_quality_validation_pydeequ.egg-info/SOURCES.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        1 2024-05-07 05:53:17.000000 data-quality-validation-pydeequ-0.6/data_quality_validation_pydeequ.egg-info/dependency_links.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)       28 2024-05-07 05:53:17.000000 data-quality-validation-pydeequ-0.6/data_quality_validation_pydeequ.egg-info/requires.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        4 2024-05-07 05:53:17.000000 data-quality-validation-pydeequ-0.6/data_quality_validation_pydeequ.egg-info/top_level.txt
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 05:53:17.903937 data-quality-validation-pydeequ-0.6/dqv/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 06:16:20.000000 data-quality-validation-pydeequ-0.6/dqv/__init__.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)    11706 2024-05-06 09:17:04.000000 data-quality-validation-pydeequ-0.6/dqv/data_quality_validation_pydeequ.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     1650 2024-05-06 09:01:46.000000 data-quality-validation-pydeequ-0.6/dqv/dqv_pydeequ.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)       38 2024-05-07 05:53:17.906048 data-quality-validation-pydeequ-0.6/setup.cfg
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)      826 2024-05-07 05:53:12.000000 data-quality-validation-pydeequ-0.6/setup.py
```

### Comparing `data-quality-validation-pydeequ-0.5/PKG-INFO` & `data-quality-validation-pydeequ-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-quality-validation-pydeequ
-Version: 0.5
+Version: 0.6
 Summary: A library for data quality validation using PyDeequ.
 Author: Ketan Kirange
 Author-email: k.kirange@reply.com
 Keywords: data quality validation pydeequ
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -12,15 +12,17 @@
 Requires-Dist: pandas
 Requires-Dist: pydeequ
 Requires-Dist: boto3
 Requires-Dist: pyyaml
 
 <span style='color: Pink; font-size:25px'>  **Data Quality Validation** </span>
 
-This is a repository for the data quality validation.
+This package is designed for performing data quality validation using PyDeequ.  
+It enables users to validate the quality of their data,  
+identifying any potential issues that may affect its suitability for processing or analysis.
 
 **Author**: Ketan Kirange
 
 **Contributors**: Ketan Kirange, Rahul Ajay, Ruth Mifsud
 
 This repository contains tools and utilities for performing data quality checks on data files in 
  - Pandas,
```

### Comparing `data-quality-validation-pydeequ-0.5/README.md` & `data-quality-validation-pydeequ-0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 <span style='color: Pink; font-size:25px'>  **Data Quality Validation** </span>
 
-This is a repository for the data quality validation.
+This package is designed for performing data quality validation using PyDeequ.  
+It enables users to validate the quality of their data,  
+identifying any potential issues that may affect its suitability for processing or analysis.
 
 **Author**: Ketan Kirange
 
 **Contributors**: Ketan Kirange, Rahul Ajay, Ruth Mifsud
 
 This repository contains tools and utilities for performing data quality checks on data files in 
  - Pandas,
```

### Comparing `data-quality-validation-pydeequ-0.5/data_quality_validation_pydeequ.egg-info/PKG-INFO` & `data-quality-validation-pydeequ-0.6/data_quality_validation_pydeequ.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-quality-validation-pydeequ
-Version: 0.5
+Version: 0.6
 Summary: A library for data quality validation using PyDeequ.
 Author: Ketan Kirange
 Author-email: k.kirange@reply.com
 Keywords: data quality validation pydeequ
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -12,15 +12,17 @@
 Requires-Dist: pandas
 Requires-Dist: pydeequ
 Requires-Dist: boto3
 Requires-Dist: pyyaml
 
 <span style='color: Pink; font-size:25px'>  **Data Quality Validation** </span>
 
-This is a repository for the data quality validation.
+This package is designed for performing data quality validation using PyDeequ.  
+It enables users to validate the quality of their data,  
+identifying any potential issues that may affect its suitability for processing or analysis.
 
 **Author**: Ketan Kirange
 
 **Contributors**: Ketan Kirange, Rahul Ajay, Ruth Mifsud
 
 This repository contains tools and utilities for performing data quality checks on data files in 
  - Pandas,
```

### Comparing `data-quality-validation-pydeequ-0.5/dqv/data_quality_validation_pydeequ.py` & `data-quality-validation-pydeequ-0.6/dqv/data_quality_validation_pydeequ.py`

 * *Files identical despite different names*

### Comparing `data-quality-validation-pydeequ-0.5/dqv/dqv_pydeequ.py` & `data-quality-validation-pydeequ-0.6/dqv/dqv_pydeequ.py`

 * *Files identical despite different names*

### Comparing `data-quality-validation-pydeequ-0.5/setup.py` & `data-quality-validation-pydeequ-0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Reading the README.md file for long description in PyPI site
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='data-quality-validation-pydeequ',
-    version='0.5',
+    version='0.6',
     author='Ketan Kirange',
     author_email='k.kirange@reply.com',
     description='A library for data quality validation using PyDeequ.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

