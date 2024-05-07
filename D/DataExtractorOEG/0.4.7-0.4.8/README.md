# Comparing `tmp/dataextractoroeg-0.4.7.tar.gz` & `tmp/dataextractoroeg-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dataextractoroeg-0.4.7.tar", last modified: Mon May  6 11:12:15 2024, max compression
+gzip compressed data, was "dist\dataextractoroeg-0.4.8.tar", last modified: Mon May  6 11:19:46 2024, max compression
```

## Comparing `dataextractoroeg-0.4.7.tar` & `dataextractoroeg-0.4.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 11:12:15.063369 dataextractoroeg-0.4.7/
--rw-rw-rw-   0        0        0       70 2024-04-29 12:43:01.000000 dataextractoroeg-0.4.7/.gitignore
-drwxrwxrwx   0        0        0        0 2024-05-06 11:12:15.052513 dataextractoroeg-0.4.7/DataExtractorOEG.egg-info/
--rw-rw-rw-   0        0        0     3078 2024-05-06 11:12:14.000000 dataextractoroeg-0.4.7/DataExtractorOEG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      470 2024-05-06 11:12:14.000000 dataextractoroeg-0.4.7/DataExtractorOEG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 11:12:14.000000 dataextractoroeg-0.4.7/DataExtractorOEG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-06 11:12:14.000000 dataextractoroeg-0.4.7/DataExtractorOEG.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-05-06 11:12:14.000000 dataextractoroeg-0.4.7/DataExtractorOEG.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-06 11:12:14.000000 dataextractoroeg-0.4.7/DataExtractorOEG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.4.7/LICENSE.txt
--rw-rw-rw-   0        0        0     3078 2024-05-06 11:12:15.059366 dataextractoroeg-0.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     2807 2024-04-29 12:08:53.000000 dataextractoroeg-0.4.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 11:12:15.046245 dataextractoroeg-0.4.7/doiExtractor/
-drwxrwxrwx   0        0        0        0 2024-05-06 11:12:15.052513 dataextractoroeg-0.4.7/doiExtractor/ExistingPapers/
--rw-rw-rw-   0        0        0   542602 2024-04-10 16:37:25.000000 dataextractoroeg-0.4.7/doiExtractor/ExistingPapers/Papers.csv
--rw-rw-rw-   0        0        0     4080 2024-04-12 14:53:18.000000 dataextractoroeg-0.4.7/doiExtractor/ExistingPapers/name_doi_papers.csv
--rw-rw-rw-   0        0        0       21 2024-04-25 13:35:45.000000 dataextractoroeg-0.4.7/doiExtractor/__init__.py
--rw-rw-rw-   0        0        0     8448 2024-05-06 10:55:59.000000 dataextractoroeg-0.4.7/doiExtractor/doiExtractor.py
--rw-rw-rw-   0        0        0     2635 2024-05-06 11:11:59.000000 dataextractoroeg-0.4.7/doiExtractor/main.py
--rw-rw-rw-   0        0        0     4119 2024-05-06 10:43:20.000000 dataextractoroeg-0.4.7/doiExtractor/openAlex.py
--rw-rw-rw-   0        0        0       42 2024-05-06 11:12:15.063597 dataextractoroeg-0.4.7/setup.cfg
--rw-rw-rw-   0        0        0      633 2024-05-06 11:12:04.000000 dataextractoroeg-0.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:19:46.682600 dataextractoroeg-0.4.8/
+-rw-rw-rw-   0        0        0       70 2024-04-29 12:43:01.000000 dataextractoroeg-0.4.8/.gitignore
+drwxrwxrwx   0        0        0        0 2024-05-06 11:19:46.678265 dataextractoroeg-0.4.8/DataExtractorOEG.egg-info/
+-rw-rw-rw-   0        0        0     3078 2024-05-06 11:19:46.000000 dataextractoroeg-0.4.8/DataExtractorOEG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2024-05-06 11:19:46.000000 dataextractoroeg-0.4.8/DataExtractorOEG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 11:19:46.000000 dataextractoroeg-0.4.8/DataExtractorOEG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-06 11:19:46.000000 dataextractoroeg-0.4.8/DataExtractorOEG.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-05-06 11:19:46.000000 dataextractoroeg-0.4.8/DataExtractorOEG.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-06 11:19:46.000000 dataextractoroeg-0.4.8/DataExtractorOEG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.4.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     3078 2024-05-06 11:19:46.679323 dataextractoroeg-0.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2807 2024-04-29 12:08:53.000000 dataextractoroeg-0.4.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 11:19:46.667521 dataextractoroeg-0.4.8/doiExtractor/
+drwxrwxrwx   0        0        0        0 2024-05-06 11:19:46.674264 dataextractoroeg-0.4.8/doiExtractor/ExistingPapers/
+-rw-rw-rw-   0        0        0   542602 2024-04-10 16:37:25.000000 dataextractoroeg-0.4.8/doiExtractor/ExistingPapers/Papers.csv
+-rw-rw-rw-   0        0        0     4080 2024-04-12 14:53:18.000000 dataextractoroeg-0.4.8/doiExtractor/ExistingPapers/name_doi_papers.csv
+-rw-rw-rw-   0        0        0       21 2024-04-25 13:35:45.000000 dataextractoroeg-0.4.8/doiExtractor/__init__.py
+-rw-rw-rw-   0        0        0     8348 2024-05-06 11:19:28.000000 dataextractoroeg-0.4.8/doiExtractor/doiExtractor.py
+-rw-rw-rw-   0        0        0     2454 2024-05-06 11:19:03.000000 dataextractoroeg-0.4.8/doiExtractor/main.py
+-rw-rw-rw-   0        0        0     4119 2024-05-06 10:43:20.000000 dataextractoroeg-0.4.8/doiExtractor/openAlex.py
+-rw-rw-rw-   0        0        0       42 2024-05-06 11:19:46.683599 dataextractoroeg-0.4.8/setup.cfg
+-rw-rw-rw-   0        0        0      633 2024-05-06 11:19:11.000000 dataextractoroeg-0.4.8/setup.py
```

### Comparing `dataextractoroeg-0.4.7/DataExtractorOEG.egg-info/PKG-INFO` & `dataextractoroeg-0.4.8/DataExtractorOEG.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataExtractorOEG
-Version: 0.4.7
+Version: 0.4.8
 Author: Pablo Torija Martínez
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: selenium
 Requires-Dist: requests
 Requires-Dist: pandas
```

### Comparing `dataextractoroeg-0.4.7/LICENSE.txt` & `dataextractoroeg-0.4.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.7/PKG-INFO` & `dataextractoroeg-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataExtractorOEG
-Version: 0.4.7
+Version: 0.4.8
 Author: Pablo Torija Martínez
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: selenium
 Requires-Dist: requests
 Requires-Dist: pandas
```

### Comparing `dataextractoroeg-0.4.7/README.md` & `dataextractoroeg-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.7/doiExtractor/ExistingPapers/Papers.csv` & `dataextractoroeg-0.4.8/doiExtractor/ExistingPapers/Papers.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.7/doiExtractor/ExistingPapers/name_doi_papers.csv` & `dataextractoroeg-0.4.8/doiExtractor/ExistingPapers/name_doi_papers.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.7/doiExtractor/doiExtractor.py` & `dataextractoroeg-0.4.8/doiExtractor/doiExtractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from bs4 import BeautifulSoup
 import pandas as pd
 import urllib.parse
 import requests
 import csv
 import os
 
-
-
 # Function to extract the DOI
 def extract_doi(url_pagina, csv_file):
     response = requests.get(url_pagina)
 
     if response.status_code == 200:
         # Extract HTML content of the page
         html_doc = response.text
@@ -196,10 +194,8 @@
     df.to_json(json_file, orient='records', indent=4)
 
 
 def find_file_by_name(path, name):
     for root, dirs, files in os.walk(path):
         if name in files:
             print(f"Found existing papers")
-            return os.path.join(root, name)
-        
-csv_to_json("doiExtractor/Outputs/results.csv", "doiExtractor/Outputs/results.json")
+            return os.path.join(root, name)
```

### Comparing `dataextractoroeg-0.4.7/doiExtractor/main.py` & `dataextractoroeg-0.4.8/doiExtractor/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,40 +13,34 @@
     parser.add_argument("--output", default="doiExtractor/Outputs", help="File path for the outputs")
     args = parser.parse_args()
 
     if args.start:
         url = args.url + "#14"
         url_docs = args.url
 
-        os.makedirs(args.output, exist_ok=True)
-
         # Files to write the output
         txt_filename = args.output + "/dois.txt"
         csv_filename = args.output + "/results.csv"
         json_filename = args.output + "/results.json"
 
+        os.makedirs(args.output, exist_ok=True)
+
         # ExistingPapers
         papers = find_file_by_name(os.getcwd(),"name_doi_papers.csv")
 
         logging.info("DOI Extractor Tool started")
         logging.info(f"Search in: {url}, Output csv: {csv_filename}, Output txt: {txt_filename}")
 
         # Delete contents of the files if already created
         if os.path.exists(csv_filename):
             open(csv_filename, 'w').close()
-        else:
-            open(csv_filename, 'x').close()
         if os.path.exists(txt_filename):
             open(txt_filename, 'w').close()
-        else:
-            open(txt_filename, 'x').close()
         if os.path.exists(json_filename):
             open(json_filename, 'w').close()
-        else:
-            open(json_filename, 'x').close()
 
         # Extract dois from url
         search_papers(url, url_docs, csv_filename)
 
         # Merge them with the existing from the papers
         merge_csv(csv_filename, papers)
```

### Comparing `dataextractoroeg-0.4.7/doiExtractor/openAlex.py` & `dataextractoroeg-0.4.8/doiExtractor/openAlex.py`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.7/setup.py` & `dataextractoroeg-0.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="DataExtractorOEG",
-    version="0.4.7",
+    version="0.4.8",
     author =  "Pablo Torija Martínez",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "beautifulsoup4",
         "selenium",
         "requests",
```

