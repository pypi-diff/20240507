# Comparing `tmp/tabqa-0.1.2.tar.gz` & `tmp/tabqa-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabqa-0.1.2.tar", last modified: Sun Apr 28 13:01:12 2024, max compression
+gzip compressed data, was "tabqa-0.1.3.tar", last modified: Tue May  7 13:03:38 2024, max compression
```

## Comparing `tabqa-0.1.2.tar` & `tabqa-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ketanmore   (501) staff       (20)        0 2024-04-28 13:01:12.503252 tabqa-0.1.2/
--rw-r--r--   0 ketanmore   (501) staff       (20)       18 2024-04-28 06:22:23.000000 tabqa-0.1.2/MANIFEST.in
--rw-r--r--   0 ketanmore   (501) staff       (20)     2449 2024-04-28 13:01:12.503051 tabqa-0.1.2/PKG-INFO
--rw-r--r--   0 ketanmore   (501) staff       (20)     2086 2024-04-28 12:46:59.000000 tabqa-0.1.2/README.md
--rw-r--r--   0 ketanmore   (501) staff       (20)       38 2024-04-28 13:01:12.503288 tabqa-0.1.2/setup.cfg
--rw-r--r--   0 ketanmore   (501) staff       (20)      759 2024-04-28 13:00:25.000000 tabqa-0.1.2/setup.py
-drwxr-xr-x   0 ketanmore   (501) staff       (20)        0 2024-04-28 13:01:12.501972 tabqa-0.1.2/tabqa/
--rw-r--r--   0 ketanmore   (501) staff       (20)       26 2024-03-17 13:17:51.000000 tabqa-0.1.2/tabqa/__init__.py
--rw-r--r--   0 ketanmore   (501) staff       (20)     3814 2024-03-24 08:14:44.000000 tabqa-0.1.2/tabqa/myfunctions.py
-drwxr-xr-x   0 ketanmore   (501) staff       (20)        0 2024-04-28 13:01:12.502871 tabqa-0.1.2/tabqa.egg-info/
--rw-r--r--   0 ketanmore   (501) staff       (20)     2449 2024-04-28 13:01:12.000000 tabqa-0.1.2/tabqa.egg-info/PKG-INFO
--rw-r--r--   0 ketanmore   (501) staff       (20)      213 2024-04-28 13:01:12.000000 tabqa-0.1.2/tabqa.egg-info/SOURCES.txt
--rw-r--r--   0 ketanmore   (501) staff       (20)        1 2024-04-28 13:01:12.000000 tabqa-0.1.2/tabqa.egg-info/dependency_links.txt
--rw-r--r--   0 ketanmore   (501) staff       (20)       52 2024-04-28 13:01:12.000000 tabqa-0.1.2/tabqa.egg-info/requires.txt
--rw-r--r--   0 ketanmore   (501) staff       (20)        6 2024-04-28 13:01:12.000000 tabqa-0.1.2/tabqa.egg-info/top_level.txt
+drwxr-xr-x   0 ketanmore   (501) staff       (20)        0 2024-05-07 13:03:38.960466 tabqa-0.1.3/
+-rw-r--r--   0 ketanmore   (501) staff       (20)       18 2024-04-28 06:22:23.000000 tabqa-0.1.3/MANIFEST.in
+-rw-r--r--   0 ketanmore   (501) staff       (20)     2455 2024-05-07 13:03:38.960189 tabqa-0.1.3/PKG-INFO
+-rw-r--r--   0 ketanmore   (501) staff       (20)     2092 2024-05-07 13:02:45.000000 tabqa-0.1.3/README.md
+-rw-r--r--   0 ketanmore   (501) staff       (20)       38 2024-05-07 13:03:38.960507 tabqa-0.1.3/setup.cfg
+-rw-r--r--   0 ketanmore   (501) staff       (20)      759 2024-05-07 13:02:48.000000 tabqa-0.1.3/setup.py
+drwxr-xr-x   0 ketanmore   (501) staff       (20)        0 2024-05-07 13:03:38.958929 tabqa-0.1.3/tabqa/
+-rw-r--r--   0 ketanmore   (501) staff       (20)       26 2024-03-17 13:17:51.000000 tabqa-0.1.3/tabqa/__init__.py
+-rw-r--r--   0 ketanmore   (501) staff       (20)     3814 2024-03-24 08:14:44.000000 tabqa-0.1.3/tabqa/myfunctions.py
+drwxr-xr-x   0 ketanmore   (501) staff       (20)        0 2024-05-07 13:03:38.959965 tabqa-0.1.3/tabqa.egg-info/
+-rw-r--r--   0 ketanmore   (501) staff       (20)     2455 2024-05-07 13:03:38.000000 tabqa-0.1.3/tabqa.egg-info/PKG-INFO
+-rw-r--r--   0 ketanmore   (501) staff       (20)      213 2024-05-07 13:03:38.000000 tabqa-0.1.3/tabqa.egg-info/SOURCES.txt
+-rw-r--r--   0 ketanmore   (501) staff       (20)        1 2024-05-07 13:03:38.000000 tabqa-0.1.3/tabqa.egg-info/dependency_links.txt
+-rw-r--r--   0 ketanmore   (501) staff       (20)       52 2024-05-07 13:03:38.000000 tabqa-0.1.3/tabqa.egg-info/requires.txt
+-rw-r--r--   0 ketanmore   (501) staff       (20)        6 2024-05-07 13:03:38.000000 tabqa-0.1.3/tabqa.egg-info/top_level.txt
```

### Comparing `tabqa-0.1.2/PKG-INFO` & `tabqa-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabqa
-Version: 0.1.2
+Version: 0.1.3
 Summary: This Python package provides functions to convert natural language to SQL queries using a pre-trained language model.
 Author: Ketan More
 Description-Content-Type: text/markdown
 Requires-Dist: torch
 Requires-Dist: transformers
 Requires-Dist: bitsandbytes
 Requires-Dist: accelerate
@@ -23,18 +23,18 @@
 ```
 
 ## Quick Start
 ```python
 from tabqa import sql_model, generate_schema
 
 # Define the natural language question
-question = "Count Number products"
+question = "Count Number of products"
 
 # Path to the SQL file containing the database schema
-file_path = "schema.sql"
+file_path = "schema.sql"  #
 
 # Initialize the SQL model
 model = sql_model()
 
 # Generate the SQL schema from the natural language question
 result = generate_schema(question, file_path, model)
```

### Comparing `tabqa-0.1.2/README.md` & `tabqa-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 ```
 
 ## Quick Start
 ```python
 from tabqa import sql_model, generate_schema
 
 # Define the natural language question
-question = "Count Number products"
+question = "Count Number of products"
 
 # Path to the SQL file containing the database schema
-file_path = "schema.sql"
+file_path = "schema.sql"  #
 
 # Initialize the SQL model
 model = sql_model()
 
 # Generate the SQL schema from the natural language question
 result = generate_schema(question, file_path, model)
```

### Comparing `tabqa-0.1.2/setup.py` & `tabqa-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='tabqa',
     packages=find_packages(),
-    version='0.1.2',
+    version='0.1.3',
     description='This Python package provides functions to convert natural language to SQL queries using a pre-trained language model.',
     long_description = long_description,
     long_description_content_type='text/markdown',
     author='Ketan More',
     install_requires = ["torch", "transformers", "bitsandbytes", "accelerate", "sqlparse"],
     setup_requires = ["torch", "transformers", "bitsandbytes", "accelerate", "sqlparse"],
     tests_require= ["torch", "transformers", "bitsandbytes", "accelerate", "sqlparse"],
```

### Comparing `tabqa-0.1.2/tabqa/myfunctions.py` & `tabqa-0.1.3/tabqa/myfunctions.py`

 * *Files identical despite different names*

### Comparing `tabqa-0.1.2/tabqa.egg-info/PKG-INFO` & `tabqa-0.1.3/tabqa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabqa
-Version: 0.1.2
+Version: 0.1.3
 Summary: This Python package provides functions to convert natural language to SQL queries using a pre-trained language model.
 Author: Ketan More
 Description-Content-Type: text/markdown
 Requires-Dist: torch
 Requires-Dist: transformers
 Requires-Dist: bitsandbytes
 Requires-Dist: accelerate
@@ -23,18 +23,18 @@
 ```
 
 ## Quick Start
 ```python
 from tabqa import sql_model, generate_schema
 
 # Define the natural language question
-question = "Count Number products"
+question = "Count Number of products"
 
 # Path to the SQL file containing the database schema
-file_path = "schema.sql"
+file_path = "schema.sql"  #
 
 # Initialize the SQL model
 model = sql_model()
 
 # Generate the SQL schema from the natural language question
 result = generate_schema(question, file_path, model)
```

