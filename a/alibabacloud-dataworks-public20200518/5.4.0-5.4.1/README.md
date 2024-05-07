# Comparing `tmp/alibabacloud_dataworks-public20200518-5.4.0.tar.gz` & `tmp/alibabacloud_dataworks-public20200518-5.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dataworks-public20200518-5.4.0.tar", last modified: Wed Apr 24 17:19:53 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dataworks-public20200518-5.4.1.tar", last modified: Tue May  7 17:13:18 2024, max compression
```

## Comparing `alibabacloud_dataworks-public20200518-5.4.0.tar` & `alibabacloud_dataworks-public20200518-5.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 17:19:53.000000 alibabacloud_dataworks-public20200518-5.4.0/
--rw-r--r--   0 root         (0) root         (0)     7926 2024-04-24 17:19:53.000000 alibabacloud_dataworks-public20200518-5.4.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-24 17:19:53.000000 alibabacloud_dataworks-public20200518-5.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-24 17:19:53.000000 alibabacloud_dataworks-public20200518-5.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2492 2024-04-24 17:19:53.000000 alibabacloud_dataworks-public20200518-5.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1147 2024-04-24 17:19:53.000000 alibabacloud_dataworks-public20200518-5.4.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1232 2024-04-24 17:19:53.000000 alibabacloud_dataworks-public20200518-5.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 17:19:53.000000 alibabacloud_dataworks-public20200518-5.4.0/alibabacloud_dataworks_public20200518/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-24 17:19:53.000000 alibabacloud_dataworks-public20200518-5.4.0/alibabacloud_dataworks_public20200518/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1110433 2024-04-24 17:19:53.000000 alibabacloud_dataworks-public20200518-5.4.0/alibabacloud_dataworks_public20200518/client.py
--rw-r--r--   0 root         (0) root         (0)  2723063 2024-04-24 17:19:53.000000 alibabacloud_dataworks-public20200518-5.4.0/alibabacloud_dataworks_public20200518/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 17:19:53.000000 alibabacloud_dataworks-public20200518-5.4.0/alibabacloud_dataworks_public20200518.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2492 2024-04-24 17:19:53.000000 alibabacloud_dataworks-public20200518-5.4.0/alibabacloud_dataworks_public20200518.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      524 2024-04-24 17:19:53.000000 alibabacloud_dataworks-public20200518-5.4.0/alibabacloud_dataworks_public20200518.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 17:19:53.000000 alibabacloud_dataworks-public20200518-5.4.0/alibabacloud_dataworks_public20200518.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      316 2024-04-24 17:19:53.000000 alibabacloud_dataworks-public20200518-5.4.0/alibabacloud_dataworks_public20200518.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 17:19:53.000000 alibabacloud_dataworks-public20200518-5.4.0/alibabacloud_dataworks_public20200518.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-24 17:19:53.000000 alibabacloud_dataworks-public20200518-5.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2869 2024-04-24 17:19:53.000000 alibabacloud_dataworks-public20200518-5.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 17:13:18.000000 alibabacloud_dataworks-public20200518-5.4.1/
+-rw-r--r--   0 root         (0) root         (0)     8442 2024-05-07 17:13:18.000000 alibabacloud_dataworks-public20200518-5.4.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-07 17:13:18.000000 alibabacloud_dataworks-public20200518-5.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-07 17:13:18.000000 alibabacloud_dataworks-public20200518-5.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2492 2024-05-07 17:13:18.000000 alibabacloud_dataworks-public20200518-5.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-05-07 17:13:18.000000 alibabacloud_dataworks-public20200518-5.4.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1232 2024-05-07 17:13:18.000000 alibabacloud_dataworks-public20200518-5.4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 17:13:18.000000 alibabacloud_dataworks-public20200518-5.4.1/alibabacloud_dataworks_public20200518/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-07 17:13:18.000000 alibabacloud_dataworks-public20200518-5.4.1/alibabacloud_dataworks_public20200518/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1110433 2024-05-07 17:13:18.000000 alibabacloud_dataworks-public20200518-5.4.1/alibabacloud_dataworks_public20200518/client.py
+-rw-r--r--   0 root         (0) root         (0)  2723063 2024-05-07 17:13:18.000000 alibabacloud_dataworks-public20200518-5.4.1/alibabacloud_dataworks_public20200518/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 17:13:18.000000 alibabacloud_dataworks-public20200518-5.4.1/alibabacloud_dataworks_public20200518.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2492 2024-05-07 17:13:18.000000 alibabacloud_dataworks-public20200518-5.4.1/alibabacloud_dataworks_public20200518.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      524 2024-05-07 17:13:18.000000 alibabacloud_dataworks-public20200518-5.4.1/alibabacloud_dataworks_public20200518.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 17:13:18.000000 alibabacloud_dataworks-public20200518-5.4.1/alibabacloud_dataworks_public20200518.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      316 2024-05-07 17:13:18.000000 alibabacloud_dataworks-public20200518-5.4.1/alibabacloud_dataworks_public20200518.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 17:13:18.000000 alibabacloud_dataworks-public20200518-5.4.1/alibabacloud_dataworks_public20200518.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-07 17:13:18.000000 alibabacloud_dataworks-public20200518-5.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2869 2024-05-07 17:13:18.000000 alibabacloud_dataworks-public20200518-5.4.1/setup.py
```

### Comparing `alibabacloud_dataworks-public20200518-5.4.0/ChangeLog.md` & `alibabacloud_dataworks-public20200518-5.4.1/ChangeLog.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+2024-04-24 Version: 5.4.0
+- Support API AddRecognizeRule.
+- Support API DeleteRecognizeRule.
+- Support API DsgRunSensIdentify.
+- Support API DsgStopSensIdentify.
+- Support API EditRecognizeRule.
+- Support API QueryDefaultTemplate.
+- Support API QueryRecognizeDataByRuleType.
+- Support API QueryRecognizeRuleDetail.
+- Support API QueryRecognizeRulesType.
+- Support API QuerySensClassification.
+- Support API QuerySensLevel.
+- Support API QuerySensNodeInfo.
+- Update API SubmitDataServiceApi: update response param.
+
+
 2024-04-17 Version: 5.3.0
 - Support API DsgQuerySensResult.
 - Update API CreateFile: update param DependentType.
 - Update API ListInstances: update param NodeId.
 - Update API UpdateFile: update param DependentType.
```

### Comparing `alibabacloud_dataworks-public20200518-5.4.0/LICENSE` & `alibabacloud_dataworks-public20200518-5.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dataworks-public20200518-5.4.0/PKG-INFO` & `alibabacloud_dataworks-public20200518-5.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dataworks-public20200518
-Version: 5.4.0
+Version: 5.4.1
 Summary: Alibaba Cloud dataworks-public (20200518) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dataworks-public20200518-5.4.0/README-CN.md` & `alibabacloud_dataworks-public20200518-5.4.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dataworks-public20200518-5.4.0/README.md` & `alibabacloud_dataworks-public20200518-5.4.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dataworks-public20200518-5.4.0/alibabacloud_dataworks_public20200518/client.py` & `alibabacloud_dataworks-public20200518-5.4.1/alibabacloud_dataworks_public20200518/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dataworks-public20200518-5.4.0/alibabacloud_dataworks_public20200518/models.py` & `alibabacloud_dataworks-public20200518-5.4.1/alibabacloud_dataworks_public20200518/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dataworks-public20200518-5.4.0/alibabacloud_dataworks_public20200518.egg-info/PKG-INFO` & `alibabacloud_dataworks-public20200518-5.4.1/alibabacloud_dataworks_public20200518.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dataworks-public20200518
-Version: 5.4.0
+Version: 5.4.1
 Summary: Alibaba Cloud dataworks-public (20200518) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dataworks-public20200518-5.4.0/alibabacloud_dataworks_public20200518.egg-info/SOURCES.txt` & `alibabacloud_dataworks-public20200518-5.4.1/alibabacloud_dataworks_public20200518.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_dataworks-public20200518-5.4.0/setup.py` & `alibabacloud_dataworks-public20200518-5.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dataworks-public20200518.
 
-Created on 24/04/2024
+Created on 07/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dataworks_public20200518"
 NAME = "alibabacloud_dataworks-public20200518" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud dataworks-public (20200518) SDK Library for Python"
```

