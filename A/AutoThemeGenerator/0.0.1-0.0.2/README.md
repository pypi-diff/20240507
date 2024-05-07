# Comparing `tmp/AutoThemeGenerator-0.0.1.tar.gz` & `tmp/autothemegenerator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoThemeGenerator-0.0.1.tar", last modified: Tue May  7 11:50:50 2024, max compression
+gzip compressed data, was "autothemegenerator-0.0.2.tar", last modified: Tue May  7 12:08:53 2024, max compression
```

## Comparing `AutoThemeGenerator-0.0.1.tar` & `autothemegenerator-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 11:50:50.865391 AutoThemeGenerator-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-05-07 11:50:50.858879 AutoThemeGenerator-0.0.1/AutoThemeGenerator/
--rw-rw-rw-   0        0        0    29092 2024-05-07 11:10:33.000000 AutoThemeGenerator-0.0.1/AutoThemeGenerator/AutoThemeGenerator.py
--rw-rw-rw-   0        0        0      116 2024-05-07 11:14:13.000000 AutoThemeGenerator-0.0.1/AutoThemeGenerator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 11:50:50.865391 AutoThemeGenerator-0.0.1/AutoThemeGenerator.egg-info/
--rw-rw-rw-   0        0        0     3962 2024-05-07 11:50:50.000000 AutoThemeGenerator-0.0.1/AutoThemeGenerator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2024-05-07 11:50:50.000000 AutoThemeGenerator-0.0.1/AutoThemeGenerator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 11:50:50.000000 AutoThemeGenerator-0.0.1/AutoThemeGenerator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-05-07 11:50:50.000000 AutoThemeGenerator-0.0.1/AutoThemeGenerator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-07 11:50:50.000000 AutoThemeGenerator-0.0.1/AutoThemeGenerator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2024-05-07 11:29:40.000000 AutoThemeGenerator-0.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1067 2024-05-07 11:27:08.000000 AutoThemeGenerator-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2024-05-07 11:30:45.000000 AutoThemeGenerator-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3962 2024-05-07 11:50:50.865391 AutoThemeGenerator-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-07 11:50:50.865391 AutoThemeGenerator-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1304 2024-05-07 11:49:31.000000 AutoThemeGenerator-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:08:53.751789 autothemegenerator-0.0.2/
+drwxrwxrwx   0        0        0        0 2024-05-07 12:08:53.733336 autothemegenerator-0.0.2/AutoThemeGenerator/
+-rw-rw-rw-   0        0        0    29092 2024-05-07 11:10:33.000000 autothemegenerator-0.0.2/AutoThemeGenerator/AutoThemeGenerator.py
+-rw-rw-rw-   0        0        0      116 2024-05-07 11:14:13.000000 autothemegenerator-0.0.2/AutoThemeGenerator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:08:53.741567 autothemegenerator-0.0.2/AutoThemeGenerator.egg-info/
+-rw-rw-rw-   0        0        0     3960 2024-05-07 12:08:53.000000 autothemegenerator-0.0.2/AutoThemeGenerator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-05-07 12:08:53.000000 autothemegenerator-0.0.2/AutoThemeGenerator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 12:08:53.000000 autothemegenerator-0.0.2/AutoThemeGenerator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-05-07 12:08:53.000000 autothemegenerator-0.0.2/AutoThemeGenerator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-07 12:08:53.000000 autothemegenerator-0.0.2/AutoThemeGenerator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      177 2024-05-07 12:08:21.000000 autothemegenerator-0.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1067 2024-05-07 12:08:17.000000 autothemegenerator-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2024-05-07 12:08:18.000000 autothemegenerator-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3960 2024-05-07 12:08:53.751789 autothemegenerator-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3079 2024-05-07 12:08:19.000000 autothemegenerator-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-07 12:08:53.751789 autothemegenerator-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1320 2024-05-07 12:08:20.000000 autothemegenerator-0.0.2/setup.py
```

### Comparing `AutoThemeGenerator-0.0.1/AutoThemeGenerator/AutoThemeGenerator.py` & `autothemegenerator-0.0.2/AutoThemeGenerator/AutoThemeGenerator.py`

 * *Files identical despite different names*

### Comparing `AutoThemeGenerator-0.0.1/AutoThemeGenerator.egg-info/PKG-INFO` & `autothemegenerator-0.0.2/AutoThemeGenerator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoThemeGenerator
-Version: 0.0.1
+Version: 0.0.2
 Summary: Performing thematic analysis with OpenAI's GPT-4 models
 Author: Charles Alba
 Author-email: alba@wustl.edu
 Keywords: GPT models,Thematic analysis,OpenAI,Qualitiative studies,transcripts,interviews
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,14 @@
 Requires-Dist: textract
 Requires-Dist: openai==1.12.0
 Requires-Dist: nltk==3.8.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: python-docx
 Requires-Dist: tqdm
 
-
 `AutoThemeGenerator` is a package that allows you to perform qualitative analysis using OpenAI's GPT models.
 
 ## Requirements
 ### Required packages
 To use `AutoThemeGenerator`, you are required to have the following packages installed:  
 - `openai`  
 - `docx`
```

### Comparing `AutoThemeGenerator-0.0.1/LICENSE.txt` & `autothemegenerator-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `AutoThemeGenerator-0.0.1/PKG-INFO` & `autothemegenerator-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoThemeGenerator
-Version: 0.0.1
+Version: 0.0.2
 Summary: Performing thematic analysis with OpenAI's GPT-4 models
 Author: Charles Alba
 Author-email: alba@wustl.edu
 Keywords: GPT models,Thematic analysis,OpenAI,Qualitiative studies,transcripts,interviews
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,14 @@
 Requires-Dist: textract
 Requires-Dist: openai==1.12.0
 Requires-Dist: nltk==3.8.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: python-docx
 Requires-Dist: tqdm
 
-
 `AutoThemeGenerator` is a package that allows you to perform qualitative analysis using OpenAI's GPT models.
 
 ## Requirements
 ### Required packages
 To use `AutoThemeGenerator`, you are required to have the following packages installed:  
 - `openai`  
 - `docx`
```

### Comparing `AutoThemeGenerator-0.0.1/setup.py` & `autothemegenerator-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
-
-with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
-    long_description = "\n" + fh.read()
-
-VERSION = '0.0.1'
+readme_path = os.path.join(here, "README.md")
+with codecs.open(readme_path, encoding="utf-8") as fh:
+    long_description = fh.read()
+VERSION = '0.0.2'
 DESCRIPTION = 'Performing thematic analysis with OpenAI\'s GPT-4 models'
 LONG_DESCRIPTION = 'A package uses openAI\'s GPT-4 model to perform thematic analysis using interview transcripts from qualititative studies'
 
 # Setting up
 setup(
     name="AutoThemeGenerator",
     version=VERSION,
```

