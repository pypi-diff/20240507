# Comparing `tmp/data-quality-validation-pydeequ-0.3.tar.gz` & `tmp/data-quality-validation-pydeequ-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-quality-validation-pydeequ-0.3.tar", last modified: Tue May  7 03:08:38 2024, max compression
+gzip compressed data, was "data-quality-validation-pydeequ-0.4.tar", last modified: Tue May  7 03:28:49 2024, max compression
```

## Comparing `data-quality-validation-pydeequ-0.3.tar` & `data-quality-validation-pydeequ-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 03:08:38.064651 data-quality-validation-pydeequ-0.3/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)      573 2024-05-07 03:08:38.064224 data-quality-validation-pydeequ-0.3/PKG-INFO
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     3218 2024-05-06 06:17:24.000000 data-quality-validation-pydeequ-0.3/README.md
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 03:08:38.063597 data-quality-validation-pydeequ-0.3/data_quality_validation_pydeequ.egg-info/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)      573 2024-05-07 03:08:37.000000 data-quality-validation-pydeequ-0.3/data_quality_validation_pydeequ.egg-info/PKG-INFO
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)      366 2024-05-07 03:08:38.000000 data-quality-validation-pydeequ-0.3/data_quality_validation_pydeequ.egg-info/SOURCES.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        1 2024-05-07 03:08:37.000000 data-quality-validation-pydeequ-0.3/data_quality_validation_pydeequ.egg-info/dependency_links.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)       28 2024-05-07 03:08:37.000000 data-quality-validation-pydeequ-0.3/data_quality_validation_pydeequ.egg-info/requires.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        4 2024-05-07 03:08:37.000000 data-quality-validation-pydeequ-0.3/data_quality_validation_pydeequ.egg-info/top_level.txt
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 03:08:38.062210 data-quality-validation-pydeequ-0.3/dqv/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 06:16:20.000000 data-quality-validation-pydeequ-0.3/dqv/__init__.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)    11706 2024-05-06 09:17:04.000000 data-quality-validation-pydeequ-0.3/dqv/data_quality_validation_pydeequ.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     1650 2024-05-06 09:01:46.000000 data-quality-validation-pydeequ-0.3/dqv/dqv_pydeequ.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)       38 2024-05-07 03:08:38.064721 data-quality-validation-pydeequ-0.3/setup.cfg
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)      754 2024-05-07 03:08:31.000000 data-quality-validation-pydeequ-0.3/setup.py
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 03:28:49.912001 data-quality-validation-pydeequ-0.4/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     4175 2024-05-07 03:28:49.911622 data-quality-validation-pydeequ-0.4/PKG-INFO
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     3695 2024-05-07 03:27:51.000000 data-quality-validation-pydeequ-0.4/README.md
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 03:28:49.911187 data-quality-validation-pydeequ-0.4/data_quality_validation_pydeequ.egg-info/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     4175 2024-05-07 03:28:49.000000 data-quality-validation-pydeequ-0.4/data_quality_validation_pydeequ.egg-info/PKG-INFO
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)      366 2024-05-07 03:28:49.000000 data-quality-validation-pydeequ-0.4/data_quality_validation_pydeequ.egg-info/SOURCES.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        1 2024-05-07 03:28:49.000000 data-quality-validation-pydeequ-0.4/data_quality_validation_pydeequ.egg-info/dependency_links.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)       28 2024-05-07 03:28:49.000000 data-quality-validation-pydeequ-0.4/data_quality_validation_pydeequ.egg-info/requires.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        4 2024-05-07 03:28:49.000000 data-quality-validation-pydeequ-0.4/data_quality_validation_pydeequ.egg-info/top_level.txt
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 03:28:49.910476 data-quality-validation-pydeequ-0.4/dqv/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 06:16:20.000000 data-quality-validation-pydeequ-0.4/dqv/__init__.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)    11706 2024-05-06 09:17:04.000000 data-quality-validation-pydeequ-0.4/dqv/data_quality_validation_pydeequ.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     1650 2024-05-06 09:01:46.000000 data-quality-validation-pydeequ-0.4/dqv/dqv_pydeequ.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)       38 2024-05-07 03:28:49.912064 data-quality-validation-pydeequ-0.4/setup.cfg
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)      826 2024-05-07 03:28:47.000000 data-quality-validation-pydeequ-0.4/setup.py
```

### Comparing `data-quality-validation-pydeequ-0.3/README.md` & `data-quality-validation-pydeequ-0.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,63 @@
-# Data Quality Validation
+<span style='color: Pink; font-size:25px'>  **Data Quality Validation** </span>
 
 This is a repository for the data quality validation.
 
 **Author**: Ketan Kirange
 
 **Contributors**: Ketan Kirange, Rahul Ajay, Ruth Mifsud
 
-This repository contains tools and utilities for performing data quality checks on data files in Pandas, Dask, and PySpark formats, leveraging libraries such as PyDeequ and SODA utilities. These checks help ensure the integrity, accuracy, and completeness of the data, essential for robust data-driven decision-making processes.
+This repository contains tools and utilities for performing data quality checks on data files in 
+ - Pandas, 
+ - Dask, and 
+ - PySpark formats, leveraging libraries such as PyDeequ and SODA utilities.
 
-## Importance of Data Quality
+These checks help ensure the integrity, accuracy, and completeness of the data, essential for robust data-driven decision-making processes.
 
-Data quality plays a pivotal role in any engineering project, especially in data science, reporting, and analysis. Here's why ensuring high data quality is crucial:
+<span style='color: Pink; font-size:25px'> **Importance of Data Quality** </span>
 
-### 1. Reliable Insights
+Data quality plays a pivotal role in any engineering project, especially in data science, reporting, and analysis.  
+Here's why ensuring high data quality is crucial:
 
-High-quality data leads to reliable and trustworthy insights. When the data is accurate, complete, and consistent, data scientists and analysts can make informed decisions confidently.
+<span style='color: Pink; font-size:25px'> 1. Reliable Insights </span>
 
-### 2. Trustworthy Models
+High-quality data leads to reliable and trustworthy insights.  
+When the data is accurate, complete, and consistent, data scientists and analysts can make informed decisions confidently.
 
-Data quality directly impacts the performance and reliability of machine learning models. Models trained on low-quality data may produce biased or inaccurate predictions, leading to unreliable outcomes.
+<span style='color: Pink; font-size:25px'> 2. Trustworthy Models </span>
 
-### 3. Effective Reporting
+Data quality directly impacts the performance and reliability of machine learning models.  
+Models trained on low-quality data may produce biased or inaccurate predictions, leading to unreliable outcomes.
 
-Quality data is fundamental for generating accurate reports and visualizations. Analysts and stakeholders rely on these reports for understanding trends, identifying patterns, and making strategic decisions. Poor data quality can lead to misleading reports and flawed interpretations.
+<span style='color: Pink; font-size:25px'> 3. Effective Reporting </span>
 
-### 4. Regulatory Compliance
+Quality data is fundamental for generating accurate reports and visualizations.  
+Analysts and stakeholders rely on these reports for understanding trends, identifying patterns, and making strategic decisions.  
+Poor data quality can lead to misleading reports and flawed interpretations.
 
-In many industries, compliance with regulations such as GDPR, HIPAA, or industry-specific standards is mandatory. Ensuring data quality is essential for meeting these regulatory requirements and avoiding potential legal consequences.
+<span style='color: Pink; font-size:25px'> 4. Regulatory Compliance </span>
 
-## Data Quality Validation Tools
+In many industries, compliance with regulations such as GDPR, HIPAA, or industry-specific standards is mandatory.  
+Ensuring data quality is essential for meeting these regulatory requirements and avoiding potential legal consequences.
+
+<span style='color: Pink; font-size:25px'> **Data Quality Validation Tools** </span>
 
 This repository provides a set of tools and utilities to perform comprehensive data quality validation on various data formats:
 
 - **Pandas**: Data quality checks for data stored in Pandas DataFrames, including checks for missing values, data types, and statistical summaries.
 - **Dask**: Scalable data quality checks for large-scale datasets using Dask, ensuring consistency and accuracy across distributed computing environments.
 - **PySpark with PyDeequ**: Integration with PyDeequ, enabling data quality validation on data processed using PySpark, including checks for schema validation, data distribution, and anomaly detection.
 - **SODA Utilities**: Utilities for validating data quality using SODA (Scalable Observations of Data Attributes) framework, allowing for automated quality checks and anomaly detection.
 
-## Getting Started
+<span style='color: Pink; font-size:25px'> **Getting Started** </span>
 
 To get started with data quality validation using this repository, follow the instructions in the respective documentation for each tool:
 
 - [Pandas Data Quality Validation Guide](link-to-pandas-guide)
 - [Dask Data Quality Validation Guide](link-to-dask-guide)
 - [PySpark with PyDeequ Guide](link-to-pyspark-guide)
 - [SODA Utilities Guide](link-to-soda-guide)
 
-## Contributing
+<span style='color: Pink; font-size:25px'> **Contributing** </span>
 
-We welcome contributions from the community to enhance and expand the capabilities of this data quality validation repository. Please refer to the [contribution guidelines](link-to-contribution-guidelines) for more information on how to contribute.
+We welcome contributions from the community to enhance and expand the capabilities of this data quality validation repository.  
+Please refer to the [contribution guidelines](link-to-contribution-guidelines) for more information on how to contribute.
```

### Comparing `data-quality-validation-pydeequ-0.3/dqv/data_quality_validation_pydeequ.py` & `data-quality-validation-pydeequ-0.4/dqv/data_quality_validation_pydeequ.py`

 * *Files identical despite different names*

### Comparing `data-quality-validation-pydeequ-0.3/dqv/dqv_pydeequ.py` & `data-quality-validation-pydeequ-0.4/dqv/dqv_pydeequ.py`

 * *Files identical despite different names*

### Comparing `data-quality-validation-pydeequ-0.3/setup.py` & `data-quality-validation-pydeequ-0.4/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from setuptools import setup, find_packages
 
+# Reading the README.md file for long description in PyPI site
+with open('README.md', 'r', encoding='utf-8') as fh:
+    long_description = fh.read()
+
 setup(
     name='data-quality-validation-pydeequ',
-    version='0.3',
+    version='0.4',
     author='Ketan Kirange',
     author_email='k.kirange@reply.com',
     description='A library for data quality validation using PyDeequ.',
-    long_description='A Python library that provides classes for performing data quality validation using Pydeequ.',
+    long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'pandas',
         'pydeequ',
         'boto3',
         'pyyaml',
```

