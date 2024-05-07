# Comparing `tmp/biodata-0.0.6.tar.gz` & `tmp/biodata-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biodata-0.0.6.tar", last modified: Mon Jan 23 07:00:15 2023, max compression
+gzip compressed data, was "biodata-0.0.7.tar", last modified: Tue May  7 11:15:28 2024, max compression
```

## Comparing `biodata-0.0.6.tar` & `biodata-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2023-01-23 07:00:15.024163 biodata-0.0.6/
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)     5621 2023-01-23 07:00:15.024163 biodata-0.0.6/PKG-INFO
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)     5037 2023-01-23 06:58:01.000000 biodata-0.0.6/README.md
-drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2023-01-23 07:00:15.009162 biodata-0.0.6/biodata/
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)        0 2021-11-03 03:50:28.000000 biodata-0.0.6/biodata/__init__.py
--rwxr-x---   0 kl945     (5298) hy299_0001 (80905)     9483 2023-01-03 16:21:03.000000 biodata-0.0.6/biodata/baseio.py
--rwxr-x---   0 kl945     (5298) hy299_0001 (80905)    11057 2023-01-03 17:37:44.000000 biodata-0.0.6/biodata/bed.py
--rwxr-x---   0 kl945     (5298) hy299_0001 (80905)     8834 2023-01-03 16:21:18.000000 biodata-0.0.6/biodata/delimited.py
--rwxr-x---   0 kl945     (5298) hy299_0001 (80905)     5522 2023-01-14 08:29:58.000000 biodata-0.0.6/biodata/fasta.py
--rwxr-x---   0 kl945     (5298) hy299_0001 (80905)     5659 2023-01-23 06:58:54.000000 biodata-0.0.6/biodata/gff.py
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)     6360 2023-01-21 06:14:11.000000 biodata-0.0.6/biodata/meme.py
-drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2023-01-23 07:00:15.023163 biodata-0.0.6/biodata.egg-info/
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)     5621 2023-01-23 07:00:12.000000 biodata-0.0.6/biodata.egg-info/PKG-INFO
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)      294 2023-01-23 07:00:12.000000 biodata-0.0.6/biodata.egg-info/SOURCES.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)        1 2023-01-23 07:00:12.000000 biodata-0.0.6/biodata.egg-info/dependency_links.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)       20 2023-01-23 07:00:12.000000 biodata-0.0.6/biodata.egg-info/requires.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)        8 2023-01-23 07:00:12.000000 biodata-0.0.6/biodata.egg-info/top_level.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)       38 2023-01-23 07:00:15.024163 biodata-0.0.6/setup.cfg
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)      842 2023-01-23 06:58:10.000000 biodata-0.0.6/setup.py
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-05-07 11:15:28.787828 biodata-0.0.7/
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)     5621 2024-05-07 11:15:28.786827 biodata-0.0.7/PKG-INFO
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)     5037 2023-01-23 06:58:01.000000 biodata-0.0.7/README.md
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-05-07 11:15:28.763826 biodata-0.0.7/biodata/
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)        0 2021-11-03 03:50:28.000000 biodata-0.0.7/biodata/__init__.py
+-rwxr-x---   0 kl945     (5298) hy299_0001 (80905)     9933 2024-05-07 11:00:55.000000 biodata-0.0.7/biodata/baseio.py
+-rwxr-x---   0 kl945     (5298) hy299_0001 (80905)    11057 2023-01-03 17:37:44.000000 biodata-0.0.7/biodata/bed.py
+-rwxr-x---   0 kl945     (5298) hy299_0001 (80905)     8834 2023-01-03 16:21:18.000000 biodata-0.0.7/biodata/delimited.py
+-rwxr-x---   0 kl945     (5298) hy299_0001 (80905)     5522 2023-01-14 08:29:58.000000 biodata-0.0.7/biodata/fasta.py
+-rwxr-x---   0 kl945     (5298) hy299_0001 (80905)     5659 2023-01-23 06:58:54.000000 biodata-0.0.7/biodata/gff.py
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)     6360 2023-01-21 06:14:11.000000 biodata-0.0.7/biodata/meme.py
+-rwxr-x---   0 kl945     (5298) hy299_0001 (80905)     9483 2023-01-03 16:21:03.000000 biodata-0.0.7/biodata/old.py
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-05-07 11:15:28.786827 biodata-0.0.7/biodata.egg-info/
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)     5621 2024-05-07 11:15:23.000000 biodata-0.0.7/biodata.egg-info/PKG-INFO
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)      309 2024-05-07 11:15:23.000000 biodata-0.0.7/biodata.egg-info/SOURCES.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)        1 2024-05-07 11:15:23.000000 biodata-0.0.7/biodata.egg-info/dependency_links.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)       20 2024-05-07 11:15:23.000000 biodata-0.0.7/biodata.egg-info/requires.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)        8 2024-05-07 11:15:23.000000 biodata-0.0.7/biodata.egg-info/top_level.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)       38 2024-05-07 11:15:28.787828 biodata-0.0.7/setup.cfg
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)      842 2024-05-07 11:07:30.000000 biodata-0.0.7/setup.py
```

### Comparing `biodata-0.0.6/PKG-INFO` & `biodata-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biodata
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python package for common biological data I/O
 Home-page: https://github.com/aldenleung/biodata/
 Author: Alden Leung
 Author-email: alden.leung@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `biodata-0.0.6/README.md` & `biodata-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `biodata-0.0.6/biodata/baseio.py` & `biodata-0.0.7/biodata/old.py`

 * *Files identical despite different names*

### Comparing `biodata-0.0.6/biodata/bed.py` & `biodata-0.0.7/biodata/bed.py`

 * *Files identical despite different names*

### Comparing `biodata-0.0.6/biodata/delimited.py` & `biodata-0.0.7/biodata/delimited.py`

 * *Files identical despite different names*

### Comparing `biodata-0.0.6/biodata/fasta.py` & `biodata-0.0.7/biodata/fasta.py`

 * *Files identical despite different names*

### Comparing `biodata-0.0.6/biodata/gff.py` & `biodata-0.0.7/biodata/gff.py`

 * *Files identical despite different names*

### Comparing `biodata-0.0.6/biodata/meme.py` & `biodata-0.0.7/biodata/meme.py`

 * *Files identical despite different names*

### Comparing `biodata-0.0.6/biodata.egg-info/PKG-INFO` & `biodata-0.0.7/biodata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biodata
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python package for common biological data I/O
 Home-page: https://github.com/aldenleung/biodata/
 Author: Alden Leung
 Author-email: alden.leung@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `biodata-0.0.6/setup.py` & `biodata-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as readme_file:
 	readme = readme_file.read()
 
 requirements = ["genomictools>=0.0.5"]
 
 setup(
 	name="biodata",
-	version="0.0.6",
+	version="0.0.7",
 	author="Alden Leung",
 	author_email="alden.leung@gmail.com",
 	description="A python package for common biological data I/O",
 	long_description=readme,
 	long_description_content_type="text/markdown",
 	url="https://github.com/aldenleung/biodata/",
 	packages=find_packages(),
```

