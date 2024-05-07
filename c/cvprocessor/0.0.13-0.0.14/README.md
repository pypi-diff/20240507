# Comparing `tmp/cvprocessor-0.0.13.tar.gz` & `tmp/cvprocessor-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvprocessor-0.0.13.tar", last modified: Mon May  6 10:05:12 2024, max compression
+gzip compressed data, was "cvprocessor-0.0.14.tar", last modified: Tue May  7 00:04:06 2024, max compression
```

## Comparing `cvprocessor-0.0.13.tar` & `cvprocessor-0.0.14.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-06 10:05:12.846043 cvprocessor-0.0.13/
--rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.0.13/LICENSE
--rw-r--r--   0 fernando   (501) staff       (20)     1690 2024-05-06 10:05:12.845450 cvprocessor-0.0.13/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)     1042 2024-05-05 07:13:28.000000 cvprocessor-0.0.13/README.md
--rw-r--r--   0 fernando   (501) staff       (20)      770 2024-05-06 10:04:41.000000 cvprocessor-0.0.13/pyproject.toml
--rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-06 10:05:12.846314 cvprocessor-0.0.13/setup.cfg
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-06 10:05:12.830892 cvprocessor-0.0.13/src/
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-06 10:05:12.841378 cvprocessor-0.0.13/src/cvprocessor/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.0.13/src/cvprocessor/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)     5851 2024-05-04 22:18:45.000000 cvprocessor-0.0.13/src/cvprocessor/authors.py
--rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.0.13/src/cvprocessor/common.py
--rw-r--r--   0 fernando   (501) staff       (20)     2106 2024-05-06 08:04:06.000000 cvprocessor-0.0.13/src/cvprocessor/cv.py
--rw-r--r--   0 fernando   (501) staff       (20)     3514 2024-05-04 09:03:16.000000 cvprocessor-0.0.13/src/cvprocessor/education.py
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-04 07:19:43.000000 cvprocessor-0.0.13/src/cvprocessor/experience.py
--rw-r--r--   0 fernando   (501) staff       (20)     3340 2024-05-06 10:02:34.000000 cvprocessor-0.0.13/src/cvprocessor/institutes.py
--rw-r--r--   0 fernando   (501) staff       (20)     1396 2024-05-04 09:02:35.000000 cvprocessor-0.0.13/src/cvprocessor/intro.py
--rw-r--r--   0 fernando   (501) staff       (20)     2088 2024-05-05 08:39:17.000000 cvprocessor-0.0.13/src/cvprocessor/news.py
--rw-r--r--   0 fernando   (501) staff       (20)     9424 2024-05-06 08:04:12.000000 cvprocessor-0.0.13/src/cvprocessor/publications.py
--rw-r--r--   0 fernando   (501) staff       (20)     1050 2024-05-05 10:18:42.000000 cvprocessor-0.0.13/src/cvprocessor/research_interests.py
--rw-r--r--   0 fernando   (501) staff       (20)     2967 2024-05-06 05:39:04.000000 cvprocessor-0.0.13/src/cvprocessor/software.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-06 10:05:12.844869 cvprocessor-0.0.13/src/cvprocessor.egg-info/
--rw-r--r--   0 fernando   (501) staff       (20)     1690 2024-05-06 10:05:12.000000 cvprocessor-0.0.13/src/cvprocessor.egg-info/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      565 2024-05-06 10:05:12.000000 cvprocessor-0.0.13/src/cvprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-06 10:05:12.000000 cvprocessor-0.0.13/src/cvprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-06 10:05:12.000000 cvprocessor-0.0.13/src/cvprocessor.egg-info/requires.txt
--rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-06 10:05:12.000000 cvprocessor-0.0.13/src/cvprocessor.egg-info/top_level.txt
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 00:04:06.617749 cvprocessor-0.0.14/
+-rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.0.14/LICENSE
+-rw-r--r--   0 fernando   (501) staff       (20)     1690 2024-05-07 00:04:06.617170 cvprocessor-0.0.14/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)     1042 2024-05-05 07:13:28.000000 cvprocessor-0.0.14/README.md
+-rw-r--r--   0 fernando   (501) staff       (20)      770 2024-05-07 00:03:18.000000 cvprocessor-0.0.14/pyproject.toml
+-rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-07 00:04:06.617859 cvprocessor-0.0.14/setup.cfg
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 00:04:06.603472 cvprocessor-0.0.14/src/
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 00:04:06.613686 cvprocessor-0.0.14/src/cvprocessor/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.0.14/src/cvprocessor/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5851 2024-05-04 22:18:45.000000 cvprocessor-0.0.14/src/cvprocessor/authors.py
+-rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.0.14/src/cvprocessor/common.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2106 2024-05-07 00:03:13.000000 cvprocessor-0.0.14/src/cvprocessor/cv.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3514 2024-05-04 09:03:16.000000 cvprocessor-0.0.14/src/cvprocessor/education.py
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-04 07:19:43.000000 cvprocessor-0.0.14/src/cvprocessor/experience.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3340 2024-05-06 10:02:34.000000 cvprocessor-0.0.14/src/cvprocessor/institutes.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1396 2024-05-04 09:02:35.000000 cvprocessor-0.0.14/src/cvprocessor/intro.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2088 2024-05-05 08:39:17.000000 cvprocessor-0.0.14/src/cvprocessor/news.py
+-rw-r--r--   0 fernando   (501) staff       (20)     9450 2024-05-07 00:03:04.000000 cvprocessor-0.0.14/src/cvprocessor/publications.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1050 2024-05-05 10:18:42.000000 cvprocessor-0.0.14/src/cvprocessor/research_interests.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2967 2024-05-06 05:39:04.000000 cvprocessor-0.0.14/src/cvprocessor/software.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 00:04:06.616578 cvprocessor-0.0.14/src/cvprocessor.egg-info/
+-rw-r--r--   0 fernando   (501) staff       (20)     1690 2024-05-07 00:04:06.000000 cvprocessor-0.0.14/src/cvprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      565 2024-05-07 00:04:06.000000 cvprocessor-0.0.14/src/cvprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-07 00:04:06.000000 cvprocessor-0.0.14/src/cvprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-07 00:04:06.000000 cvprocessor-0.0.14/src/cvprocessor.egg-info/requires.txt
+-rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-07 00:04:06.000000 cvprocessor-0.0.14/src/cvprocessor.egg-info/top_level.txt
```

### Comparing `cvprocessor-0.0.13/LICENSE` & `cvprocessor-0.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.13/PKG-INFO` & `cvprocessor-0.0.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.0.13
+Version: 0.0.14
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.0.13/README.md` & `cvprocessor-0.0.14/README.md`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.13/pyproject.toml` & `cvprocessor-0.0.14/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cvprocessor"
-version = "0.0.13"
+version = "0.0.14"
 authors = [
     { name = "F. Fernando Jurado-Lasso", email = "fdo.jurado@gmail.com" },
 ]
 description = "CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cvprocessor-0.0.13/src/cvprocessor/authors.py` & `cvprocessor-0.0.14/src/cvprocessor/authors.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.13/src/cvprocessor/cv.py` & `cvprocessor-0.0.14/src/cvprocessor/cv.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.13/src/cvprocessor/education.py` & `cvprocessor-0.0.14/src/cvprocessor/education.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.13/src/cvprocessor/institutes.py` & `cvprocessor-0.0.14/src/cvprocessor/institutes.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.13/src/cvprocessor/intro.py` & `cvprocessor-0.0.14/src/cvprocessor/intro.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.13/src/cvprocessor/news.py` & `cvprocessor-0.0.14/src/cvprocessor/news.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.13/src/cvprocessor/publications.py` & `cvprocessor-0.0.14/src/cvprocessor/publications.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,14 +276,15 @@
 
     def get_num_publications_by_author(self, author_id):
         count = 0
         for publication in self.publications:
             for author in publication.authors:
                 if author.id == author_id:
                     count += 1
+                    break
         return count
 
     def get_publications_year_range(self):
         years = []
         for publication in self.publications:
             years.append(publication.year.year)
         return min(years), max(years)
```

### Comparing `cvprocessor-0.0.13/src/cvprocessor/research_interests.py` & `cvprocessor-0.0.14/src/cvprocessor/research_interests.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.13/src/cvprocessor/software.py` & `cvprocessor-0.0.14/src/cvprocessor/software.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.13/src/cvprocessor.egg-info/PKG-INFO` & `cvprocessor-0.0.14/src/cvprocessor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.0.13
+Version: 0.0.14
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.0.13/src/cvprocessor.egg-info/SOURCES.txt` & `cvprocessor-0.0.14/src/cvprocessor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

