# Comparing `tmp/sap-business-document-processing-0.4.0.tar.gz` & `tmp/sap_business_document_processing-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sap-business-document-processing-0.4.0.tar", last modified: Thu Nov  2 16:00:46 2023, max compression
+gzip compressed data, was "sap_business_document_processing-0.4.1.tar", last modified: Tue May  7 11:21:51 2024, max compression
```

## Comparing `sap-business-document-processing-0.4.0.tar` & `sap_business_document_processing-0.4.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 16:00:46.572922 sap-business-document-processing-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11380 2023-11-02 16:00:26.000000 sap-business-document-processing-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8669 2023-11-02 16:00:46.572922 sap-business-document-processing-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7814 2023-11-02 16:00:26.000000 sap-business-document-processing-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-02 16:00:36.000000 sap-business-document-processing-0.4.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 16:00:46.564922 sap-business-document-processing-0.4.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 16:00:46.568922 sap-business-document-processing-0.4.0/examples/document_information_extraction_examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2023-11-02 16:00:27.000000 sap-business-document-processing-0.4.0/examples/document_information_extraction_examples/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-11-02 16:00:27.000000 sap-business-document-processing-0.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 16:00:46.568922 sap-business-document-processing-0.4.0/sap_business_document_processing/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2023-11-02 16:00:27.000000 sap-business-document-processing-0.4.0/sap_business_document_processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 16:00:46.568922 sap-business-document-processing-0.4.0/sap_business_document_processing/common/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-11-02 16:00:27.000000 sap-business-document-processing-0.4.0/sap_business_document_processing/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2023-11-02 16:00:27.000000 sap-business-document-processing-0.4.0/sap_business_document_processing/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2023-11-02 16:00:27.000000 sap-business-document-processing-0.4.0/sap_business_document_processing/common/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7878 2023-11-02 16:00:27.000000 sap-business-document-processing-0.4.0/sap_business_document_processing/common/http_client_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 16:00:46.568922 sap-business-document-processing-0.4.0/sap_business_document_processing/document_classification_client/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-11-02 16:00:27.000000 sap-business-document-processing-0.4.0/sap_business_document_processing/document_classification_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2023-11-02 16:00:27.000000 sap-business-document-processing-0.4.0/sap_business_document_processing/document_classification_client/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    27994 2023-11-02 16:00:27.000000 sap-business-document-processing-0.4.0/sap_business_document_processing/document_classification_client/dc_api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 16:00:46.568922 sap-business-document-processing-0.4.0/sap_business_document_processing/document_information_extraction_client/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-11-02 16:00:27.000000 sap-business-document-processing-0.4.0/sap_business_document_processing/document_information_extraction_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2023-11-02 16:00:27.000000 sap-business-document-processing-0.4.0/sap_business_document_processing/document_information_extraction_client/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    41175 2023-11-02 16:00:27.000000 sap-business-document-processing-0.4.0/sap_business_document_processing/document_information_extraction_client/dox_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-11-02 16:00:27.000000 sap-business-document-processing-0.4.0/sap_business_document_processing/document_information_extraction_client/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2023-11-02 16:00:27.000000 sap-business-document-processing-0.4.0/sap_business_document_processing/document_information_extraction_client/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 16:00:46.568922 sap-business-document-processing-0.4.0/sap_business_document_processing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8669 2023-11-02 16:00:46.000000 sap-business-document-processing-0.4.0/sap_business_document_processing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2023-11-02 16:00:46.000000 sap-business-document-processing-0.4.0/sap_business_document_processing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-02 16:00:46.000000 sap-business-document-processing-0.4.0/sap_business_document_processing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-11-02 16:00:46.000000 sap-business-document-processing-0.4.0/sap_business_document_processing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-11-02 16:00:46.000000 sap-business-document-processing-0.4.0/sap_business_document_processing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-11-02 16:00:46.572922 sap-business-document-processing-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-11-02 16:00:27.000000 sap-business-document-processing-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:21:51.029639 sap_business_document_processing-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11380 2024-05-07 11:21:28.000000 sap_business_document_processing-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9346 2024-05-07 11:21:51.029639 sap_business_document_processing-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-05-07 11:21:28.000000 sap_business_document_processing-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 11:21:42.000000 sap_business_document_processing-0.4.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:21:51.025639 sap_business_document_processing-0.4.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:21:51.025639 sap_business_document_processing-0.4.1/examples/document_information_extraction_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-05-07 11:21:28.000000 sap_business_document_processing-0.4.1/examples/document_information_extraction_examples/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-07 11:21:28.000000 sap_business_document_processing-0.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:21:51.025639 sap_business_document_processing-0.4.1/sap_business_document_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-07 11:21:28.000000 sap_business_document_processing-0.4.1/sap_business_document_processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:21:51.029639 sap_business_document_processing-0.4.1/sap_business_document_processing/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-07 11:21:28.000000 sap_business_document_processing-0.4.1/sap_business_document_processing/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-07 11:21:28.000000 sap_business_document_processing-0.4.1/sap_business_document_processing/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-07 11:21:28.000000 sap_business_document_processing-0.4.1/sap_business_document_processing/common/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8007 2024-05-07 11:21:28.000000 sap_business_document_processing-0.4.1/sap_business_document_processing/common/http_client_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:21:51.029639 sap_business_document_processing-0.4.1/sap_business_document_processing/document_classification_client/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-07 11:21:28.000000 sap_business_document_processing-0.4.1/sap_business_document_processing/document_classification_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-07 11:21:28.000000 sap_business_document_processing-0.4.1/sap_business_document_processing/document_classification_client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27994 2024-05-07 11:21:28.000000 sap_business_document_processing-0.4.1/sap_business_document_processing/document_classification_client/dc_api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:21:51.029639 sap_business_document_processing-0.4.1/sap_business_document_processing/document_information_extraction_client/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-07 11:21:28.000000 sap_business_document_processing-0.4.1/sap_business_document_processing/document_information_extraction_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-05-07 11:21:28.000000 sap_business_document_processing-0.4.1/sap_business_document_processing/document_information_extraction_client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57363 2024-05-07 11:21:28.000000 sap_business_document_processing-0.4.1/sap_business_document_processing/document_information_extraction_client/dox_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-07 11:21:28.000000 sap_business_document_processing-0.4.1/sap_business_document_processing/document_information_extraction_client/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-05-07 11:21:28.000000 sap_business_document_processing-0.4.1/sap_business_document_processing/document_information_extraction_client/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:21:51.029639 sap_business_document_processing-0.4.1/sap_business_document_processing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9346 2024-05-07 11:21:51.000000 sap_business_document_processing-0.4.1/sap_business_document_processing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-07 11:21:51.000000 sap_business_document_processing-0.4.1/sap_business_document_processing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 11:21:51.000000 sap_business_document_processing-0.4.1/sap_business_document_processing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-07 11:21:51.000000 sap_business_document_processing-0.4.1/sap_business_document_processing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-07 11:21:51.000000 sap_business_document_processing-0.4.1/sap_business_document_processing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-07 11:21:51.029639 sap_business_document_processing-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-07 11:21:28.000000 sap_business_document_processing-0.4.1/setup.py
```

### Comparing `sap-business-document-processing-0.4.0/LICENSE` & `sap_business_document_processing-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sap-business-document-processing-0.4.0/PKG-INFO` & `sap_business_document_processing-0.4.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sap-business-document-processing
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python client library for convenient usage of SAP Business Document Processing services
 Home-page: https://github.com/sap/business-document-processing
 Download-URL: https://pypi.org/project/sap-business-document-processing
 Author: Alexander Bolshakov
 Author-email: alexander.bolshakov@sap.com
 License: apache-2.0
 Keywords: SAP,business,document,processing,classification,information,extraction,machine learning
@@ -24,19 +24,19 @@
 SPDX-License-Identifier: Apache-2.0
 -->
 
 # Python Client Library for the SAP AI Business Services: Document Classification and Document Information Extraction
 
 [![REUSE status](https://api.reuse.software/badge/github.com/SAP/business-document-processing)](https://api.reuse.software/info/github.com/SAP/business-document-processing)
 
-This repository contains the [source code](sap_business_document_processing) of a Python client library to facilitate the use of the SAP AI Business Services: [Document Classification](https://help.sap.com/dc) and [Document Information Extraction](https://help.sap.com/dox). The client library provides two API Client classes that contain convenient methods to access these services and issue calls to the [Document Classification REST API](https://help.sap.com/viewer/ca60cd2ed44f4261a3ae500234c46f37/SHIP/en-US/c1045a561faf4ba0ae2b0e7713f5e6c4.html) and [Document Information Extraction REST API](https://help.sap.com/viewer/5fa7265b9ff64d73bac7cec61ee55ae6/SHIP/en-US/ded7d34e60f1422ba2e04e892a7f0e25.html) respectively. To use the library you need to [have access to SAP Business Technology Platform](https://www.sap.com/products/cloud-platform/get-started.html).
+This repository contains the [source code](https://github.com/SAP/business-document-processing/tree/main/sap_business_document_processing) of a Python client library to facilitate the use of the SAP AI Business Services: [Document Classification](https://help.sap.com/dc) and [Document Information Extraction](https://help.sap.com/dox). The client library provides two API Client classes that contain convenient methods to access these services and issue calls to the [Document Classification REST API](https://help.sap.com/viewer/ca60cd2ed44f4261a3ae500234c46f37/SHIP/en-US/c1045a561faf4ba0ae2b0e7713f5e6c4.html) and [Document Information Extraction REST API](https://help.sap.com/viewer/5fa7265b9ff64d73bac7cec61ee55ae6/SHIP/en-US/ded7d34e60f1422ba2e04e892a7f0e25.html) respectively. To use the library you need to [have access to SAP Business Technology Platform](https://www.sap.com/products/cloud-platform/get-started.html).
 
-Check out the [**usage examples**](./examples), they are very useful to get started with the services.
+Check out the [**usage examples**](https://github.com/SAP/business-document-processing/tree/main/examples), they are very useful to get started with the services.
 
-Have a look at [**API documentation**](./API.md) in order to use the library.
+Have a look at [**API documentation**](https://github.com/SAP/business-document-processing/blob/main/API.md) in order to use the library.
 
 ### Notes for users of the sap-document-classification-client library
 This library includes all the capabilities of the sap-document-classification-client, which will not be developed further. However, the code is still available [here](https://github.com/SAP/business-document-processing/tree/master).
 If you want to switch to this library, you have to be aware of the following changes:
 
 * The DCApiClient can now be imported directly from the top module via: ```from sap_business_document_processing import DCApiClient```
 * The functions ```classifiy_documents```, ```upload_documents_to_dataset```, ```upload_documents_directory_to_dataset``` now return an iterator instead of a list. You can either analyze individual results using with ```result = next(iterator)``` within a try-catch block (e.g. to handle each failed document) or use ```results = list(iterator)``` to turn it to a list. The latter will raise an error if at least one document failed.
@@ -80,22 +80,22 @@
 * Try out classification using default model [demo](https://mybinder.org/v2/gh/SAP/business-document-processing/main?filepath=examples%2Fdocument_classification_examples%2Fclassification_default_model.ipynb)
 * Try out training and classification using custom model [demo](https://mybinder.org/v2/gh/SAP/business-document-processing/main?filepath=examples%2Fdocument_classification_examples%2Ftrain_and_evaluate_custom_model.ipynb) (requires an enterprise account, trial account is **not** sufficient)
 
 #### Document Information Extraction
 
 Try out the Document Information Extraction service with this [showcase](https://mybinder.org/v2/gh/SAP/business-document-processing/main?filepath=examples%2Fdocument_information_extraction_examples%2Finformation_extraction_showcase.ipynb)
 
-- [Exercises](doc_inf_ext_exercises/)
-    - [Exercise 1 - Set up Document Information Extraction Service and UI](doc_inf_ext_exercises#exercise-1---set-up-document-information-extraction-service-and-ui)
-    - [Exercise 2 - Upload a document for extraction using UI application](doc_inf_ext_exercises#exercise-2---upload-documents-for-extraction-using-ui-application)
-    - [Exercise 3 - Visualize, correct extraction results and confirm document using UI application](doc_inf_ext_exercises#exercise-3---visualize-correct-extraction-results-and-confirm-document-using-ui-application)
-    - [Exercise 4 - Get Auth token to use Document Information Extraction Rest API](doc_inf_ext_exercises#exercise-4---get-auth-token-to-use-document-information-extraction-rest-api)
-    - [Exercise 5 - Get extraction results of document using Rest API](doc_inf_ext_exercises#exercise-5---get-extraction-results-of-document-using-rest-api)
-    - [Exercise 6 - Upload supplier Data for matching](doc_inf_ext_exercises#exercise-6---upload-supplier-data-for-matching)
-    - [Exercise 7 - Upload document through Rest API to enrich the extraction Results with supplier data](doc_inf_ext_exercises#exercise-7---upload-document-through-rest-api-to-enrich-the-extraction-results-with-supplier-data)
+- [Exercises](https://github.com/SAP/business-document-processing/tree/main/doc_inf_ext_exercises)
+    - [Exercise 1 - Set up Document Information Extraction Service and UI](https://github.com/SAP/business-document-processing/tree/main/doc_inf_ext_exercises#exercise-1---set-up-document-information-extraction-service-and-ui)
+    - [Exercise 2 - Upload a document for extraction using UI application](https://github.com/SAP/business-document-processing/tree/main/doc_inf_ext_exercises#exercise-2---upload-documents-for-extraction-using-ui-application)
+    - [Exercise 3 - Visualize, correct extraction results and confirm document using UI application](https://github.com/SAP/business-document-processing/tree/main/doc_inf_ext_exercises#exercise-3---visualize-correct-extraction-results-and-confirm-document-using-ui-application)
+    - [Exercise 4 - Get Auth token to use Document Information Extraction Rest API](https://github.com/SAP/business-document-processing/tree/main/doc_inf_ext_exercises#exercise-4---get-auth-token-to-use-document-information-extraction-rest-api)
+    - [Exercise 5 - Get extraction results of document using Rest API](https://github.com/SAP/business-document-processing/tree/main/doc_inf_ext_exercises#exercise-5---get-extraction-results-of-document-using-rest-api)
+    - [Exercise 6 - Upload supplier Data for matching](https://github.com/SAP/business-document-processing/tree/main/doc_inf_ext_exercises#exercise-6---upload-supplier-data-for-matching)
+    - [Exercise 7 - Upload document through Rest API to enrich the extraction Results with supplier data](https://github.com/SAP/business-document-processing/tree/main/doc_inf_ext_exercises#exercise-7---upload-document-through-rest-api-to-enrich-the-extraction-results-with-supplier-data)
 
 ## Known Issues
 
 Please see the [issues section](https://github.com/SAP/business-document-processing/issues).
 
 ## How to obtain support
```

### Comparing `sap-business-document-processing-0.4.0/README.md` & `sap_business_document_processing-0.4.1/sap_business_document_processing.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,42 @@
+Metadata-Version: 2.1
+Name: sap-business-document-processing
+Version: 0.4.1
+Summary: Python client library for convenient usage of SAP Business Document Processing services
+Home-page: https://github.com/sap/business-document-processing
+Download-URL: https://pypi.org/project/sap-business-document-processing
+Author: Alexander Bolshakov
+Author-email: alexander.bolshakov@sap.com
+License: apache-2.0
+Keywords: SAP,business,document,processing,classification,information,extraction,machine learning
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: urllib3~=1.26
+Requires-Dist: requests~=2.31
+Requires-Dist: requests_oauthlib~=1.3
+
 <!--
 SPDX-FileCopyrightText: 2020 2019-2020 SAP SE
 
 SPDX-License-Identifier: Apache-2.0
 -->
 
 # Python Client Library for the SAP AI Business Services: Document Classification and Document Information Extraction
 
 [![REUSE status](https://api.reuse.software/badge/github.com/SAP/business-document-processing)](https://api.reuse.software/info/github.com/SAP/business-document-processing)
 
-This repository contains the [source code](sap_business_document_processing) of a Python client library to facilitate the use of the SAP AI Business Services: [Document Classification](https://help.sap.com/dc) and [Document Information Extraction](https://help.sap.com/dox). The client library provides two API Client classes that contain convenient methods to access these services and issue calls to the [Document Classification REST API](https://help.sap.com/viewer/ca60cd2ed44f4261a3ae500234c46f37/SHIP/en-US/c1045a561faf4ba0ae2b0e7713f5e6c4.html) and [Document Information Extraction REST API](https://help.sap.com/viewer/5fa7265b9ff64d73bac7cec61ee55ae6/SHIP/en-US/ded7d34e60f1422ba2e04e892a7f0e25.html) respectively. To use the library you need to [have access to SAP Business Technology Platform](https://www.sap.com/products/cloud-platform/get-started.html).
+This repository contains the [source code](https://github.com/SAP/business-document-processing/tree/main/sap_business_document_processing) of a Python client library to facilitate the use of the SAP AI Business Services: [Document Classification](https://help.sap.com/dc) and [Document Information Extraction](https://help.sap.com/dox). The client library provides two API Client classes that contain convenient methods to access these services and issue calls to the [Document Classification REST API](https://help.sap.com/viewer/ca60cd2ed44f4261a3ae500234c46f37/SHIP/en-US/c1045a561faf4ba0ae2b0e7713f5e6c4.html) and [Document Information Extraction REST API](https://help.sap.com/viewer/5fa7265b9ff64d73bac7cec61ee55ae6/SHIP/en-US/ded7d34e60f1422ba2e04e892a7f0e25.html) respectively. To use the library you need to [have access to SAP Business Technology Platform](https://www.sap.com/products/cloud-platform/get-started.html).
 
-Check out the [**usage examples**](./examples), they are very useful to get started with the services.
+Check out the [**usage examples**](https://github.com/SAP/business-document-processing/tree/main/examples), they are very useful to get started with the services.
 
-Have a look at [**API documentation**](./API.md) in order to use the library.
+Have a look at [**API documentation**](https://github.com/SAP/business-document-processing/blob/main/API.md) in order to use the library.
 
 ### Notes for users of the sap-document-classification-client library
 This library includes all the capabilities of the sap-document-classification-client, which will not be developed further. However, the code is still available [here](https://github.com/SAP/business-document-processing/tree/master).
 If you want to switch to this library, you have to be aware of the following changes:
 
 * The DCApiClient can now be imported directly from the top module via: ```from sap_business_document_processing import DCApiClient```
 * The functions ```classifiy_documents```, ```upload_documents_to_dataset```, ```upload_documents_directory_to_dataset``` now return an iterator instead of a list. You can either analyze individual results using with ```result = next(iterator)``` within a try-catch block (e.g. to handle each failed document) or use ```results = list(iterator)``` to turn it to a list. The latter will raise an error if at least one document failed.
@@ -60,22 +80,22 @@
 * Try out classification using default model [demo](https://mybinder.org/v2/gh/SAP/business-document-processing/main?filepath=examples%2Fdocument_classification_examples%2Fclassification_default_model.ipynb)
 * Try out training and classification using custom model [demo](https://mybinder.org/v2/gh/SAP/business-document-processing/main?filepath=examples%2Fdocument_classification_examples%2Ftrain_and_evaluate_custom_model.ipynb) (requires an enterprise account, trial account is **not** sufficient)
 
 #### Document Information Extraction
 
 Try out the Document Information Extraction service with this [showcase](https://mybinder.org/v2/gh/SAP/business-document-processing/main?filepath=examples%2Fdocument_information_extraction_examples%2Finformation_extraction_showcase.ipynb)
 
-- [Exercises](doc_inf_ext_exercises/)
-    - [Exercise 1 - Set up Document Information Extraction Service and UI](doc_inf_ext_exercises#exercise-1---set-up-document-information-extraction-service-and-ui)
-    - [Exercise 2 - Upload a document for extraction using UI application](doc_inf_ext_exercises#exercise-2---upload-documents-for-extraction-using-ui-application)
-    - [Exercise 3 - Visualize, correct extraction results and confirm document using UI application](doc_inf_ext_exercises#exercise-3---visualize-correct-extraction-results-and-confirm-document-using-ui-application)
-    - [Exercise 4 - Get Auth token to use Document Information Extraction Rest API](doc_inf_ext_exercises#exercise-4---get-auth-token-to-use-document-information-extraction-rest-api)
-    - [Exercise 5 - Get extraction results of document using Rest API](doc_inf_ext_exercises#exercise-5---get-extraction-results-of-document-using-rest-api)
-    - [Exercise 6 - Upload supplier Data for matching](doc_inf_ext_exercises#exercise-6---upload-supplier-data-for-matching)
-    - [Exercise 7 - Upload document through Rest API to enrich the extraction Results with supplier data](doc_inf_ext_exercises#exercise-7---upload-document-through-rest-api-to-enrich-the-extraction-results-with-supplier-data)
+- [Exercises](https://github.com/SAP/business-document-processing/tree/main/doc_inf_ext_exercises)
+    - [Exercise 1 - Set up Document Information Extraction Service and UI](https://github.com/SAP/business-document-processing/tree/main/doc_inf_ext_exercises#exercise-1---set-up-document-information-extraction-service-and-ui)
+    - [Exercise 2 - Upload a document for extraction using UI application](https://github.com/SAP/business-document-processing/tree/main/doc_inf_ext_exercises#exercise-2---upload-documents-for-extraction-using-ui-application)
+    - [Exercise 3 - Visualize, correct extraction results and confirm document using UI application](https://github.com/SAP/business-document-processing/tree/main/doc_inf_ext_exercises#exercise-3---visualize-correct-extraction-results-and-confirm-document-using-ui-application)
+    - [Exercise 4 - Get Auth token to use Document Information Extraction Rest API](https://github.com/SAP/business-document-processing/tree/main/doc_inf_ext_exercises#exercise-4---get-auth-token-to-use-document-information-extraction-rest-api)
+    - [Exercise 5 - Get extraction results of document using Rest API](https://github.com/SAP/business-document-processing/tree/main/doc_inf_ext_exercises#exercise-5---get-extraction-results-of-document-using-rest-api)
+    - [Exercise 6 - Upload supplier Data for matching](https://github.com/SAP/business-document-processing/tree/main/doc_inf_ext_exercises#exercise-6---upload-supplier-data-for-matching)
+    - [Exercise 7 - Upload document through Rest API to enrich the extraction Results with supplier data](https://github.com/SAP/business-document-processing/tree/main/doc_inf_ext_exercises#exercise-7---upload-document-through-rest-api-to-enrich-the-extraction-results-with-supplier-data)
 
 ## Known Issues
 
 Please see the [issues section](https://github.com/SAP/business-document-processing/issues).
 
 ## How to obtain support
```

### Comparing `sap-business-document-processing-0.4.0/examples/document_information_extraction_examples/utils.py` & `sap_business_document_processing-0.4.1/examples/document_information_extraction_examples/utils.py`

 * *Files identical despite different names*

### Comparing `sap-business-document-processing-0.4.0/sap_business_document_processing/common/exceptions.py` & `sap_business_document_processing-0.4.1/sap_business_document_processing/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `sap-business-document-processing-0.4.0/sap_business_document_processing/common/helpers.py` & `sap_business_document_processing-0.4.1/sap_business_document_processing/common/helpers.py`

 * *Files identical despite different names*

### Comparing `sap-business-document-processing-0.4.0/sap_business_document_processing/common/http_client_base.py` & `sap_business_document_processing-0.4.1/sap_business_document_processing/common/http_client_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,14 +143,17 @@
 
     def post(self, path: str, validate=True, **kwargs):
         return self._request(self.session.post, path, validate, **kwargs)
 
     def delete(self, path: str, validate=True, **kwargs):
         return self._request(self.session.delete, path, validate, **kwargs)
 
+    def put(self, path: str, validate=True, **kwargs):
+        return self._request(self.session.put, path, validate, **kwargs)
+
     def raise_for_status_with_logging(self, response):
         e = None
         if response.status_code == 401:
             e = BDPUnauthorizedException('Missing authorization for this service', response, status_code=401)
         elif 400 <= response.status_code < 500:
             try:
                 msg = str(response.json())
```

### Comparing `sap-business-document-processing-0.4.0/sap_business_document_processing/document_classification_client/constants.py` & `sap_business_document_processing-0.4.1/sap_business_document_processing/document_classification_client/constants.py`

 * *Files identical despite different names*

### Comparing `sap-business-document-processing-0.4.0/sap_business_document_processing/document_classification_client/dc_api_client.py` & `sap_business_document_processing-0.4.1/sap_business_document_processing/document_classification_client/dc_api_client.py`

 * *Files identical despite different names*

### Comparing `sap-business-document-processing-0.4.0/sap_business_document_processing/document_information_extraction_client/dox_api_client.py` & `sap_business_document_processing-0.4.1/sap_business_document_processing/document_information_extraction_client/dox_api_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 # SPDX-FileCopyrightText: 2020 2019-2020 SAP SE
 #
 # SPDX-License-Identifier: Apache-2.0
-
 from concurrent.futures import ThreadPoolExecutor
 import json
 import logging
 from pathlib import Path
 from typing import Iterator, List, Union
 
 from sap_business_document_processing.common.http_client_base import CommonClient
 from sap_business_document_processing.common.helpers import get_ground_truth_json, function_wrap_errors
 from .constants import API_FIELD_CLIENT_ID, API_FIELD_CLIENT_LIMIT, API_FIELD_CLIENT_NAME, API_FIELD_ID, \
     API_FIELD_EXTRACTED_VALUES, API_FIELD_RESULTS, API_FIELD_RETURN_NULL, API_FIELD_STATUS, API_FIELD_VALUE, \
     API_FIELD_DATA_FOR_RETRAINING, API_HEADER_ACCEPT, API_REQUEST_FIELD_CLIENT_START_WITH, API_REQUEST_FIELD_FILE, \
     API_REQUEST_FIELD_LIMIT, API_REQUEST_FIELD_OFFSET, API_REQUEST_FIELD_OPTIONS, API_REQUEST_FIELD_PAYLOAD, \
     API_REQUEST_FIELD_ENRICHMENT_COMPANYCODE, API_REQUEST_FIELD_ENRICHMENT_ID, API_REQUEST_FIELD_ENRICHMENT_SUBTYPE, \
     API_REQUEST_FIELD_ENRICHMENT_SYSTEM, API_REQUEST_FIELD_ENRICHMENT_TYPE, CONTENT_TYPE_PDF, CONTENT_TYPE_PNG, \
-    CONTENT_TYPE_UNKNOWN, DATA_TYPE_BUSINESS_ENTITY, DOCUMENT_TYPE_ADVICE, FILE_TYPE_EXCEL
+    CONTENT_TYPE_UNKNOWN, DATA_TYPE_BUSINESS_ENTITY, DOCUMENT_TYPE_ADVICE, FILE_TYPE_EXCEL, SCHEMAS_ENDPOINT, \
+    API_FIELD_PREDEFINED, API_REQUEST_FIELD_ORDER, API_FIELD_DOCUMENT_TYPE, \
+    SCHEMAS_UPDATE_ENDPOINT, SCHEMAS_VERSION_FIELDS_ENDPOINT, SCHEMAS_VERSION_ACTIVATE_ENDPOINT, \
+    SCHEMAS_VERSION_DEACTIVATE_ENDPOINT, SCHEMAS_VERSIONS_ENDPOINT, SCHEMAS_VERSION_UUID_ENDPOINT, \
+    SUPPORTED_MODEL_TYPES, SCHEMAS_CAPABILITIES, API_FIELD_NAME, \
+    API_FIELD_DOCUMENT_TYPE_DESCRIPTION, API_FIELD_EXTRACTED_HEADER_FIELDS, API_FIELD_EXTRACTED_LINE_ITEM_FIELDS, \
+    API_FIELD_SCHEMA_DESCRIPTION, MODEL_TYPE_DEFAULT
 from .endpoints import CAPABILITIES_ENDPOINT, CLIENT_ENDPOINT, CLIENT_MAPPING_ENDPOINT, DATA_ACTIVATION_ASYNC_ENDPOINT,\
     DATA_ACTIVATION_ID_ENDPOINT, DATA_ENDPOINT, DATA_ASYNC_ENDPOINT, DATA_ID_ENDPOINT, DOCUMENT_ENDPOINT, \
     DOCUMENT_CONFIRM_ENDPOINT, DOCUMENT_ID_ENDPOINT, DOCUMENT_ID_REQUEST_ENDPOINT, DOCUMENT_PAGE_ENDPOINT, \
     DOCUMENT_PAGE_DIMENSIONS_ENDPOINT, DOCUMENT_PAGES_DIMENSIONS_ENDPOINT, DOCUMENT_PAGE_TEXT_ENDPOINT, \
     DOCUMENT_PAGES_TEXT_ENDPOINT
-from .helpers import create_document_options, create_capability_mapping_options, get_mimetype
+from .helpers import create_document_options, create_capability_mapping_options, get_mimetype, \
+    create_payload_for_schema_fields
 
 
 class DoxApiClient(CommonClient):
     """
     This class provides an interface to access SAP Document Information Extraction REST API from a Python application.
     The structure of the values returned by all the methods is documented in the API reference:
     https://help.sap.com/viewer/5fa7265b9ff64d73bac7cec61ee55ae6/SHIP/en-US/ded7d34e60f1422ba2e04e892a7f0e25.html
@@ -418,15 +424,15 @@
         }
         if data_type == DATA_TYPE_BUSINESS_ENTITY and subtype is not None:
             params[API_REQUEST_FIELD_ENRICHMENT_SUBTYPE] = subtype
         if not isinstance(data, list):
             data = [data]
         resp = self.post(DATA_ASYNC_ENDPOINT, json={API_FIELD_VALUE: data}, params=params,
                          log_msg_before=f'Start uploading {len(data)} enrichment data '
-                         f'records of type {data_type} for client {client_id}')
+                                        f'records of type {data_type} for client {client_id}')
         job_id = resp.json()[API_FIELD_ID]
         response = self._poll_for_url(DATA_ID_ENDPOINT.format(id=job_id), sleep_interval=1,
                                       get_status=lambda r: r[API_FIELD_VALUE][API_FIELD_STATUS],
                                       log_msg_after=f'Successfully uploaded {len(data)} enrichment data records for client {client_id}')
         return response.json()
 
     def get_enrichment_data(self, client_id, data_type: str, subtype: str = None, top: int = None, skip: int = None,
@@ -505,22 +511,22 @@
             API_REQUEST_FIELD_ENRICHMENT_TYPE: data_type
         }
         if subtype is not None:
             params[API_REQUEST_FIELD_ENRICHMENT_SUBTYPE] = subtype
         delete_url = DATA_ASYNC_ENDPOINT if delete_async else DATA_ENDPOINT
         response = self.delete(delete_url, json={API_FIELD_VALUE: enrichment_records}, params=params,
                                log_msg_before=f"Start deleting {len(enrichment_records) if len(enrichment_records) > 0 else 'all'} "
-                               f"enrichment data records for client {client_id}")
+                                              f"enrichment data records for client {client_id}")
 
         if delete_async:
             job_id = response.json()[API_FIELD_ID]
             response = self._poll_for_url(DATA_ID_ENDPOINT.format(id=job_id),
                                           get_status=lambda r: r[API_FIELD_VALUE][API_FIELD_STATUS],
                                           log_msg_after=f"Successfully deleted {len(enrichment_records) if len(enrichment_records) > 0 else 'all'} "
-                                          f"enrichment data records for client {client_id}")
+                                                        f"enrichment data records for client {client_id}")
         return response.json()
 
     def activate_enrichment_data(self, params=None) -> dict:
         """
         Activates all enrichment data records for the current tenant
         :param params: Optional. A dictionary, list of tuples or bytes to send as a query string.
         :return: The API endpoint response as dictionary
@@ -629,7 +635,357 @@
         params = {
             API_FIELD_DATA_FOR_RETRAINING: data_for_retraining
         }
         response = self.post(DOCUMENT_CONFIRM_ENDPOINT.format(document_id=document_id), params=params,
                              log_msg_before=f'Confirming document with ID {document_id}',
                              log_msg_after=f'Successfully confirmed document with ID {document_id}')
         return response.json()
+
+    def create_schema(self, client_id, schema_name, schema_desc, document_type, document_type_desc):
+        """
+        Creates a new schema
+        :param client_id: The client ID for which the schema shall be created
+        :param schema_name: Name for the schema to be created
+        :param schema_desc: Description for the schema to be created
+        :param document_type: Document Type which will be supported by the schema
+        :param document_type_desc: Document Type description for the schema to be created
+        :return: The API endpoint response as dictionary
+        """
+        payload = {
+            API_FIELD_NAME: schema_name,
+            API_FIELD_SCHEMA_DESCRIPTION: schema_desc,
+            API_FIELD_DOCUMENT_TYPE: document_type,
+            API_FIELD_DOCUMENT_TYPE_DESCRIPTION: document_type_desc
+        }
+        if client_id:
+            payload[API_FIELD_CLIENT_ID] = client_id
+        response = self._create_schema(payload)
+        return response.json()
+
+    def _create_schema(self, payload):
+        """
+        POST /schemas
+        """
+        return self.post(SCHEMAS_ENDPOINT, json=payload)
+
+    def get_schema_configurations(self, client_id, predefined: bool = None, document_type: str = None,
+                                  skip: int = None,
+                                  top: int = None,
+                                  order_by: str = None):
+        """
+        Retrieves all schemas for the provided client
+        :param client_id: The client ID for which the schema details need to be fetched
+        :param predefined: (optional) The arguement which specifies if the schema is predefined schema or not
+        :param document_type: (optional) The argument to filter out schemas based on the provided document_type
+        :param skip: (optional) The index of the first record to be returned
+        :param top: (optional) The maximum number records to be returned
+        :param order_by: (optional) The value to order the elements returned based on it
+        :return: The schema values as dictionary with 'schemas' as key of the json response
+        """
+        url = SCHEMAS_ENDPOINT
+        params = {
+            API_FIELD_CLIENT_ID: client_id
+        }
+        if predefined is not None:
+            params[API_FIELD_PREDEFINED] = predefined
+        if document_type is not None:
+            params[API_FIELD_DOCUMENT_TYPE] = document_type
+        if predefined is not None:
+            params[API_REQUEST_FIELD_OFFSET] = skip
+        if predefined is not None:
+            params[API_REQUEST_FIELD_LIMIT] = top
+        if predefined is not None:
+            params[API_REQUEST_FIELD_ORDER] = order_by
+        response = self.get(url, params=params)
+        return response.json()
+
+    def delete_schema(self, client_id, schema_id):
+        """
+        Deletes specified schema for a client
+        :param client_id: The client ID for which the schema shall be deleted
+        :param schema_id: ID of the schema that shall be deleted [string]
+        :return: The API endpoint response as dictionary
+        """
+        payload = {
+            API_FIELD_VALUE: [schema_id]
+        }
+        response = self._delete_schemas(payload, client_id)
+        return response.json()
+
+    def delete_schemas(self, client_id, schema_ids):
+        """
+        Deletes multiple schemas for a client
+        :param client_id: The client ID for which the schemas shall be deleted
+        :param schema_ids: IDs of the schemas that shall be deleted [list of strings]
+        :return: The API endpoint response as dictionary
+        """
+        payload = {
+            API_FIELD_VALUE: schema_ids
+        }
+        response = self._delete_schemas(payload, client_id)
+        return response.json()
+
+    def _delete_schemas(self, payload, client_id):
+        """
+        DELETE /schemas
+        """
+        params = {
+            API_FIELD_CLIENT_ID: client_id
+        }
+        url = SCHEMAS_ENDPOINT
+        return self.delete(url, params=params, json=payload)
+
+    def create_schema_version(self, client_id, schema_id):
+        """
+        Creates a new version for the schema
+        :param client_id: The client ID for which the new version shall be created
+        :param schema_id: ID for the schema from which new version shall be created
+        :return: The API endpoint response as dictionary
+        """
+        response = self._create_schema_version(client_id, schema_id)
+        return response.json()
+
+    def _create_schema_version(self, client_id, schema_id):
+        """
+        POST /schemas/{schemaId}
+        """
+        params = {
+            API_FIELD_CLIENT_ID: client_id
+        }
+        url = SCHEMAS_UPDATE_ENDPOINT.format(schemaId=schema_id)
+        return self.post(url, params=params)
+
+    def get_schema_configuration_details(self, client_id, schema_id):
+        """
+        Retrieves details for a specific schema
+        :param client_id: The client ID for which the schema details shall be fetched
+        :param schema_id: The ID of the schema whose details shall be fetched
+        :return: The schema details as dictionary
+        """
+        response = self._get_schema_configurations_details(client_id, schema_id)
+        return response.json()
+
+    def _get_schema_configurations_details(self, client_id, schema_id):
+        """
+        GET /schemas/{schemaId}
+        """
+        params = {
+            API_FIELD_CLIENT_ID: client_id
+        }
+        url = SCHEMAS_UPDATE_ENDPOINT.format(schemaId=schema_id)
+        return self.get(url, params=params)
+
+    def update_schema_configuration(self, client_id, schema_id, schema_name, schema_desc, document_type_desc):
+        """
+        Updates the schema details for a specific schema
+        :param client_id: The client ID for which the details shall be updated
+        :param schema_id: ID for the schema for which details shall be updated
+        :param schema_name: Name of the schema (updated or old)
+        :param schema_desc: Description for the schema (updated or old)
+        :param document_type_desc: Description of the document-type for the schema (updated or old)
+        :return: The API endpoint response as dictionary
+        """
+        payload = {
+            API_FIELD_NAME: schema_name,
+            API_FIELD_SCHEMA_DESCRIPTION: schema_desc,
+            API_FIELD_DOCUMENT_TYPE_DESCRIPTION: document_type_desc
+        }
+        response = self._update_schema_configuration(client_id, schema_id, payload)
+        return response.json()
+
+    def _update_schema_configuration(self, client_id, schema_id, payload):
+        """
+        PUT /schemas/{schemasId}
+        """
+        params = {
+            API_FIELD_CLIENT_ID: client_id
+        }
+        url = SCHEMAS_UPDATE_ENDPOINT.format(schemaId=schema_id)
+        return self.put(url, params=params, json=payload)
+
+    def add_schema_version_fields(self, client_id, schema_id, version, header_fields=[], line_item_fields=[]):
+        """
+        Adds Header and Line Item fields to a schema version
+        :param client_id: The client ID for which the fields shall be added
+        :param schema_id: ID for the schema for which fields shall be added
+        :param version: Version of the schema for which fields shall be added
+        :param header_fields: (optional) List of header fields that shall be added
+        :param line_item_fields: (optional) List of line item fields that shall be added
+        :return: The API endpoint response as dictionary
+        """
+        payload = {
+            API_FIELD_EXTRACTED_HEADER_FIELDS: header_fields,
+            API_FIELD_EXTRACTED_LINE_ITEM_FIELDS: line_item_fields
+        }
+        response = self._add_schema_version_fields(client_id, schema_id, version, payload)
+        return response.json()
+
+    def _add_schema_version_fields(self, client_id, schema_id, version, payload):
+        """
+        POST /schemas/{schemaId}/versions/{version}/fields
+        """
+        params = {
+            API_FIELD_CLIENT_ID: client_id
+        }
+        url = SCHEMAS_VERSION_FIELDS_ENDPOINT.format(schemaId=schema_id, versionId=version)
+        return self.post(url, params=params, json=payload)
+
+    def activate_schema_version(self, client_id, schema_id, version):
+        """
+        Activates a schema version
+        :param client_id: The client ID for which the schema version shall be activated
+        :param schema_id: ID for the schema for which the schema version shall be activated
+        :param version: Version of the schema that shall be activated
+        :return: The API endpoint response as dictionary
+        """
+        response = self._activate_schema_version(client_id, schema_id, version)
+        return response.json()
+
+    def _activate_schema_version(self, client_id, schema_id, version):
+        """
+        POST /schemas/{schemaId}/versions/{version}/activate
+        """
+        params = {
+            API_FIELD_CLIENT_ID: client_id
+        }
+        url = SCHEMAS_VERSION_ACTIVATE_ENDPOINT.format(schemaId=schema_id, versionId=version)
+        return self.post(url, params=params)
+
+    def deactivate_schema_version(self, client_id, schema_id, version):
+        """
+        Deactivates a schema version
+        :param client_id: The client ID for which the schema version shall be deactivated
+        :param schema_id: ID for the schema for which the schema version shall be deactivated
+        :param version: Version of the schema that shall be deactivated
+        :return: The API endpoint response as dictionary
+        """
+        response = self._deactivate_schema_version(client_id, schema_id, version)
+        return response.json()
+
+    def _deactivate_schema_version(self, client_id, schema_id, version):
+        """
+        POST /schemas/{schemaId}/versions/{version}/deactivate
+        """
+        params = {
+            API_FIELD_CLIENT_ID: client_id
+        }
+        url = SCHEMAS_VERSION_DEACTIVATE_ENDPOINT.format(schemaId=schema_id, versionId=version)
+        return self.post(url, params=params)
+
+    def get_schema_capabilities(self):
+        """
+        Retrieves the capabilities for all schemas
+        :return: The schema capabilities as dictionary
+        """
+        response = self._get_schema_capabilities()
+        return response.json()
+
+    def _get_schema_capabilities(self):
+        """
+        GET /schemas/capabilities
+        """
+        url = SCHEMAS_CAPABILITIES
+        return self.get(url)
+
+    def delete_schema_versions(self, client_id, schema_id, versions):
+        """
+        Deletes specific versions of the schema
+        :param client_id: The client ID for which the schema version shall be deleted
+        :param schema_id: ID for the schema for which the schema version shall be deleted
+        :param versions: List of versions of the schema that shall be deleted
+        :return: The API endpoint response as dictionary
+        """
+        response = self._delete_schema_versions(client_id, schema_id, versions)
+        return response.json()
+
+    def _delete_schema_versions(self, client_id, schema_id, versions):
+        """
+        DELETE /schemas/{schemaId}/versions
+        """
+        params = {
+            API_FIELD_CLIENT_ID: client_id
+        }
+        url = SCHEMAS_VERSIONS_ENDPOINT.format(schemaId=schema_id)
+        payload = {
+            "version": versions
+        }
+        return self.delete(url, params=params, json=payload)
+
+    def get_all_schema_versions(self, client_id, schema_id):
+        """
+        Retrieves all the versions associated with a schema
+        :param client_id: The client ID for which the schema versions shall be fetched
+        :param schema_id: ID for the schema for which the schema versions shall be fetched
+        :return: The schema version details as dictionary with 'schemas' as key of the json response
+        """
+        response = self._get_all_schema_versions(client_id, schema_id)
+        return response.json()
+
+    def _get_all_schema_versions(self, client_id, schema_id):
+        """
+        GET /schemas/{schemaId}/versions
+        """
+        params = {
+            API_FIELD_CLIENT_ID: client_id
+        }
+        url = SCHEMAS_VERSIONS_ENDPOINT.format(schemaId=schema_id)
+        return self.get(url, params=params)
+
+    def get_schema_version_details(self, client_id, schema_id, version):
+        """
+        Retrieves specific version details associated with a schema
+        :param client_id: The client ID for which the schema version shall be fetched
+        :param schema_id: ID for the schema for which the schema version shall be fetched
+        :param version: Version of the schema that shall be fetched
+        :return: Schema version details as dictionary
+        """
+        response = self._get_schema_version_details(client_id, schema_id, version)
+        return response.json()
+
+    def _get_schema_version_details(self, client_id, schema_id, version):
+        """
+        GET /schemas/{schemaId}/versions/{version}
+        """
+        params = {
+            API_FIELD_CLIENT_ID: client_id
+        }
+        url = SCHEMAS_VERSION_UUID_ENDPOINT.format(schemaId=schema_id, versionId=version)
+        return self.get(url, params=params)
+
+    def create_schema_with_fields(self, client_id, schema_name, schema_desc, document_type, document_type_desc,
+                                  model_type, setup_type_version=None, header_fields=None, line_fields=None):
+        """
+        Creates schema along with header fields and line items
+        :param client_id: The client ID for which the schema shall be created
+        :param schema_name: Name for the schema to be created
+        :param schema_desc: Description for the schema to be created
+        :param document_type: Document Type which will be supported by the schema
+        :param document_type_desc: Document Type description for the schema to be created
+        :param model_type: Type of model for document extraction
+        :param setup_type_version: (optional) The version of setup_type for the fields to be added
+        :param header_fields: (optional) List of header fields that shall be added
+        :param line_fields: (optional) List of line item fields that shall be added
+        :return: The response message and schema_id as a dictionary
+
+        Header and Line items should have name, description, label and datatype in dictionary format.
+        """
+        if model_type not in SUPPORTED_MODEL_TYPES or model_type is None:
+            raise ValueError(f'Invalid model. Valid models are {SUPPORTED_MODEL_TYPES}.')
+        if model_type is MODEL_TYPE_DEFAULT:
+            capabilities = self.get_default_extractor_data()
+            header_items, line_items = create_payload_for_schema_fields(model_type, setup_type_version,
+                                                                        header_fields, line_fields, capabilities)
+        else:
+            header_items, line_items = create_payload_for_schema_fields(model_type, setup_type_version,
+                                                                        header_fields, line_fields)
+        response = self.create_schema(client_id, schema_name, schema_desc, document_type, document_type_desc)
+        schema_id = response[API_FIELD_ID]
+        response = self.add_schema_version_fields(client_id, schema_id, '1', header_items, line_items)
+        response[API_FIELD_ID] = schema_id
+        return response
+
+    def get_default_extractor_data(self):
+        try:
+            capabilities = self.get_capabilities()
+            return capabilities
+        except Exception as e:
+            print(e)
```

### Comparing `sap-business-document-processing-0.4.0/sap_business_document_processing/document_information_extraction_client/endpoints.py` & `sap_business_document_processing-0.4.1/sap_business_document_processing/document_information_extraction_client/endpoints.py`

 * *Files identical despite different names*

### Comparing `sap-business-document-processing-0.4.0/sap_business_document_processing.egg-info/SOURCES.txt` & `sap_business_document_processing-0.4.1/sap_business_document_processing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sap-business-document-processing-0.4.0/setup.cfg` & `sap_business_document_processing-0.4.1/setup.cfg`

 * *Files identical despite different names*

