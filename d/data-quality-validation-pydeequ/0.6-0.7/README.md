# Comparing `tmp/data-quality-validation-pydeequ-0.6.tar.gz` & `tmp/data-quality-validation-pydeequ-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-quality-validation-pydeequ-0.6.tar", last modified: Tue May  7 05:53:17 2024, max compression
+gzip compressed data, was "data-quality-validation-pydeequ-0.7.tar", last modified: Tue May  7 08:32:36 2024, max compression
```

## Comparing `data-quality-validation-pydeequ-0.6.tar` & `data-quality-validation-pydeequ-0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 05:53:17.905751 data-quality-validation-pydeequ-0.6/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     6067 2024-05-07 05:53:17.905298 data-quality-validation-pydeequ-0.6/PKG-INFO
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     5586 2024-05-07 05:53:03.000000 data-quality-validation-pydeequ-0.6/README.md
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 05:53:17.904823 data-quality-validation-pydeequ-0.6/data_quality_validation_pydeequ.egg-info/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     6067 2024-05-07 05:53:17.000000 data-quality-validation-pydeequ-0.6/data_quality_validation_pydeequ.egg-info/PKG-INFO
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)      366 2024-05-07 05:53:17.000000 data-quality-validation-pydeequ-0.6/data_quality_validation_pydeequ.egg-info/SOURCES.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        1 2024-05-07 05:53:17.000000 data-quality-validation-pydeequ-0.6/data_quality_validation_pydeequ.egg-info/dependency_links.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)       28 2024-05-07 05:53:17.000000 data-quality-validation-pydeequ-0.6/data_quality_validation_pydeequ.egg-info/requires.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        4 2024-05-07 05:53:17.000000 data-quality-validation-pydeequ-0.6/data_quality_validation_pydeequ.egg-info/top_level.txt
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 05:53:17.903937 data-quality-validation-pydeequ-0.6/dqv/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 06:16:20.000000 data-quality-validation-pydeequ-0.6/dqv/__init__.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)    11706 2024-05-06 09:17:04.000000 data-quality-validation-pydeequ-0.6/dqv/data_quality_validation_pydeequ.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     1650 2024-05-06 09:01:46.000000 data-quality-validation-pydeequ-0.6/dqv/dqv_pydeequ.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)       38 2024-05-07 05:53:17.906048 data-quality-validation-pydeequ-0.6/setup.cfg
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)      826 2024-05-07 05:53:12.000000 data-quality-validation-pydeequ-0.6/setup.py
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 08:32:36.066926 data-quality-validation-pydeequ-0.7/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     6083 2024-05-07 08:32:36.066469 data-quality-validation-pydeequ-0.7/PKG-INFO
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     5602 2024-05-07 08:32:19.000000 data-quality-validation-pydeequ-0.7/README.md
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 08:32:36.065878 data-quality-validation-pydeequ-0.7/data_quality_validation_pydeequ.egg-info/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     6083 2024-05-07 08:32:35.000000 data-quality-validation-pydeequ-0.7/data_quality_validation_pydeequ.egg-info/PKG-INFO
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)      366 2024-05-07 08:32:36.000000 data-quality-validation-pydeequ-0.7/data_quality_validation_pydeequ.egg-info/SOURCES.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        1 2024-05-07 08:32:35.000000 data-quality-validation-pydeequ-0.7/data_quality_validation_pydeequ.egg-info/dependency_links.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)       28 2024-05-07 08:32:35.000000 data-quality-validation-pydeequ-0.7/data_quality_validation_pydeequ.egg-info/requires.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        4 2024-05-07 08:32:35.000000 data-quality-validation-pydeequ-0.7/data_quality_validation_pydeequ.egg-info/top_level.txt
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 08:32:36.065153 data-quality-validation-pydeequ-0.7/dqv/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 06:16:20.000000 data-quality-validation-pydeequ-0.7/dqv/__init__.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)    11706 2024-05-06 09:17:04.000000 data-quality-validation-pydeequ-0.7/dqv/data_quality_validation_pydeequ.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     1650 2024-05-06 09:01:46.000000 data-quality-validation-pydeequ-0.7/dqv/dqv_pydeequ.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)       38 2024-05-07 08:32:36.067242 data-quality-validation-pydeequ-0.7/setup.cfg
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)      826 2024-05-07 08:32:31.000000 data-quality-validation-pydeequ-0.7/setup.py
```

### Comparing `data-quality-validation-pydeequ-0.6/PKG-INFO` & `data-quality-validation-pydeequ-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-quality-validation-pydeequ
-Version: 0.6
+Version: 0.7
 Summary: A library for data quality validation using PyDeequ.
 Author: Ketan Kirange
 Author-email: k.kirange@reply.com
 Keywords: data quality validation pydeequ
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -13,31 +13,31 @@
 Requires-Dist: pydeequ
 Requires-Dist: boto3
 Requires-Dist: pyyaml
 
 <span style='color: Pink; font-size:25px'>  **Data Quality Validation** </span>
 
 This package is designed for performing data quality validation using PyDeequ.  
-It enables users to validate the quality of their data,  
-identifying any potential issues that may affect its suitability for processing or analysis.
+It enables users to validate the quality of their data, identifying any potential issues that may affect its suitability for processing or analysis.
 
 **Author**: Ketan Kirange
 
-**Contributors**: Ketan Kirange, Rahul Ajay, Ruth Mifsud
+**Contributors**: Ketan Kirange, Ajay Rahul Raja, Ruth Mifsud
 
 This repository contains tools and utilities for performing data quality checks on data files in 
  - Pandas, 
  - Dask, and 
  - PySpark formats, leveraging libraries such as PyDeequ and SODA utilities.
 
 These checks help ensure the integrity, accuracy, and completeness of the data, essential for robust data-driven decision-making processes.
 
 <span style='color: Pink; font-size:25px'> **Importance of Data Quality** </span>
 
 Data quality plays a pivotal role in any engineering project, especially in data science, reporting, and analysis.  
+
 Here's why ensuring high data quality is crucial:
 
 <span style='color: Pink; font-size:25px'> 1. Reliable Insights </span>
 
 High-quality data leads to reliable and trustworthy insights.  
 When the data is accurate, complete, and consistent, data scientists and analysts can make informed decisions confidently.
 
@@ -77,14 +77,17 @@
 
 <span style='color: Pink; font-size:25px'> **Contributing** </span>
 
 We welcome contributions from the community to enhance and expand the capabilities of this data quality validation repository.  
 Please refer to the [contribution guidelines](link-to-contribution-guidelines) for more information on how to contribute.
 
 
+
+
+<br></br>
 <span style="font-size:13pt; color:orange">**Prerequisites:**</span>
 
 - Step 1: Download Java, Python, and Apache Spark.    
 Having the appropriate versions is essential to run the code on a local system.  
 
 <span style="font-size:11pt; color:green"> **Java:** </span>     [Java 1.8 Archive Downloads](https://www.oracle.com/uk/java/technologies/javase/javase8-archive-downloads.html)
```

### Comparing `data-quality-validation-pydeequ-0.6/README.md` & `data-quality-validation-pydeequ-0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <span style='color: Pink; font-size:25px'>  **Data Quality Validation** </span>
 
 This package is designed for performing data quality validation using PyDeequ.  
-It enables users to validate the quality of their data,  
-identifying any potential issues that may affect its suitability for processing or analysis.
+It enables users to validate the quality of their data, identifying any potential issues that may affect its suitability for processing or analysis.
 
 **Author**: Ketan Kirange
 
-**Contributors**: Ketan Kirange, Rahul Ajay, Ruth Mifsud
+**Contributors**: Ketan Kirange, Ajay Rahul Raja, Ruth Mifsud
 
 This repository contains tools and utilities for performing data quality checks on data files in 
  - Pandas, 
  - Dask, and 
  - PySpark formats, leveraging libraries such as PyDeequ and SODA utilities.
 
 These checks help ensure the integrity, accuracy, and completeness of the data, essential for robust data-driven decision-making processes.
 
 <span style='color: Pink; font-size:25px'> **Importance of Data Quality** </span>
 
 Data quality plays a pivotal role in any engineering project, especially in data science, reporting, and analysis.  
+
 Here's why ensuring high data quality is crucial:
 
 <span style='color: Pink; font-size:25px'> 1. Reliable Insights </span>
 
 High-quality data leads to reliable and trustworthy insights.  
 When the data is accurate, complete, and consistent, data scientists and analysts can make informed decisions confidently.
 
@@ -61,14 +61,17 @@
 
 <span style='color: Pink; font-size:25px'> **Contributing** </span>
 
 We welcome contributions from the community to enhance and expand the capabilities of this data quality validation repository.  
 Please refer to the [contribution guidelines](link-to-contribution-guidelines) for more information on how to contribute.
 
 
+
+
+<br></br>
 <span style="font-size:13pt; color:orange">**Prerequisites:**</span>
 
 - Step 1: Download Java, Python, and Apache Spark.    
 Having the appropriate versions is essential to run the code on a local system.  
 
 <span style="font-size:11pt; color:green"> **Java:** </span>     [Java 1.8 Archive Downloads](https://www.oracle.com/uk/java/technologies/javase/javase8-archive-downloads.html)
```

### Comparing `data-quality-validation-pydeequ-0.6/data_quality_validation_pydeequ.egg-info/PKG-INFO` & `data-quality-validation-pydeequ-0.7/data_quality_validation_pydeequ.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-quality-validation-pydeequ
-Version: 0.6
+Version: 0.7
 Summary: A library for data quality validation using PyDeequ.
 Author: Ketan Kirange
 Author-email: k.kirange@reply.com
 Keywords: data quality validation pydeequ
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -13,31 +13,31 @@
 Requires-Dist: pydeequ
 Requires-Dist: boto3
 Requires-Dist: pyyaml
 
 <span style='color: Pink; font-size:25px'>  **Data Quality Validation** </span>
 
 This package is designed for performing data quality validation using PyDeequ.  
-It enables users to validate the quality of their data,  
-identifying any potential issues that may affect its suitability for processing or analysis.
+It enables users to validate the quality of their data, identifying any potential issues that may affect its suitability for processing or analysis.
 
 **Author**: Ketan Kirange
 
-**Contributors**: Ketan Kirange, Rahul Ajay, Ruth Mifsud
+**Contributors**: Ketan Kirange, Ajay Rahul Raja, Ruth Mifsud
 
 This repository contains tools and utilities for performing data quality checks on data files in 
  - Pandas, 
  - Dask, and 
  - PySpark formats, leveraging libraries such as PyDeequ and SODA utilities.
 
 These checks help ensure the integrity, accuracy, and completeness of the data, essential for robust data-driven decision-making processes.
 
 <span style='color: Pink; font-size:25px'> **Importance of Data Quality** </span>
 
 Data quality plays a pivotal role in any engineering project, especially in data science, reporting, and analysis.  
+
 Here's why ensuring high data quality is crucial:
 
 <span style='color: Pink; font-size:25px'> 1. Reliable Insights </span>
 
 High-quality data leads to reliable and trustworthy insights.  
 When the data is accurate, complete, and consistent, data scientists and analysts can make informed decisions confidently.
 
@@ -77,14 +77,17 @@
 
 <span style='color: Pink; font-size:25px'> **Contributing** </span>
 
 We welcome contributions from the community to enhance and expand the capabilities of this data quality validation repository.  
 Please refer to the [contribution guidelines](link-to-contribution-guidelines) for more information on how to contribute.
 
 
+
+
+<br></br>
 <span style="font-size:13pt; color:orange">**Prerequisites:**</span>
 
 - Step 1: Download Java, Python, and Apache Spark.    
 Having the appropriate versions is essential to run the code on a local system.  
 
 <span style="font-size:11pt; color:green"> **Java:** </span>     [Java 1.8 Archive Downloads](https://www.oracle.com/uk/java/technologies/javase/javase8-archive-downloads.html)
```

### Comparing `data-quality-validation-pydeequ-0.6/dqv/data_quality_validation_pydeequ.py` & `data-quality-validation-pydeequ-0.7/dqv/data_quality_validation_pydeequ.py`

 * *Files identical despite different names*

### Comparing `data-quality-validation-pydeequ-0.6/dqv/dqv_pydeequ.py` & `data-quality-validation-pydeequ-0.7/dqv/dqv_pydeequ.py`

 * *Files identical despite different names*

### Comparing `data-quality-validation-pydeequ-0.6/setup.py` & `data-quality-validation-pydeequ-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Reading the README.md file for long description in PyPI site
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='data-quality-validation-pydeequ',
-    version='0.6',
+    version='0.7',
     author='Ketan Kirange',
     author_email='k.kirange@reply.com',
     description='A library for data quality validation using PyDeequ.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

