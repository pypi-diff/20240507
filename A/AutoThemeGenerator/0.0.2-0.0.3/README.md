# Comparing `tmp/autothemegenerator-0.0.2.tar.gz` & `tmp/autothemegenerator-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autothemegenerator-0.0.2.tar", last modified: Tue May  7 12:08:53 2024, max compression
+gzip compressed data, was "autothemegenerator-0.0.3.tar", last modified: Tue May  7 12:20:33 2024, max compression
```

## Comparing `autothemegenerator-0.0.2.tar` & `autothemegenerator-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 12:08:53.751789 autothemegenerator-0.0.2/
-drwxrwxrwx   0        0        0        0 2024-05-07 12:08:53.733336 autothemegenerator-0.0.2/AutoThemeGenerator/
--rw-rw-rw-   0        0        0    29092 2024-05-07 11:10:33.000000 autothemegenerator-0.0.2/AutoThemeGenerator/AutoThemeGenerator.py
--rw-rw-rw-   0        0        0      116 2024-05-07 11:14:13.000000 autothemegenerator-0.0.2/AutoThemeGenerator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 12:08:53.741567 autothemegenerator-0.0.2/AutoThemeGenerator.egg-info/
--rw-rw-rw-   0        0        0     3960 2024-05-07 12:08:53.000000 autothemegenerator-0.0.2/AutoThemeGenerator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-05-07 12:08:53.000000 autothemegenerator-0.0.2/AutoThemeGenerator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 12:08:53.000000 autothemegenerator-0.0.2/AutoThemeGenerator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-05-07 12:08:53.000000 autothemegenerator-0.0.2/AutoThemeGenerator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-07 12:08:53.000000 autothemegenerator-0.0.2/AutoThemeGenerator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      177 2024-05-07 12:08:21.000000 autothemegenerator-0.0.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1067 2024-05-07 12:08:17.000000 autothemegenerator-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2024-05-07 12:08:18.000000 autothemegenerator-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3960 2024-05-07 12:08:53.751789 autothemegenerator-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3079 2024-05-07 12:08:19.000000 autothemegenerator-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-07 12:08:53.751789 autothemegenerator-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1320 2024-05-07 12:08:20.000000 autothemegenerator-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:20:33.928073 autothemegenerator-0.0.3/
+drwxrwxrwx   0        0        0        0 2024-05-07 12:20:33.917209 autothemegenerator-0.0.3/AutoThemeGenerator/
+-rw-rw-rw-   0        0        0    29092 2024-05-07 12:17:48.000000 autothemegenerator-0.0.3/AutoThemeGenerator/AutoThemeGenerator.py
+-rw-rw-rw-   0        0        0       86 2024-05-07 12:19:43.000000 autothemegenerator-0.0.3/AutoThemeGenerator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:20:33.926026 autothemegenerator-0.0.3/AutoThemeGenerator.egg-info/
+-rw-rw-rw-   0        0        0     3960 2024-05-07 12:20:33.000000 autothemegenerator-0.0.3/AutoThemeGenerator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-05-07 12:20:33.000000 autothemegenerator-0.0.3/AutoThemeGenerator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 12:20:33.000000 autothemegenerator-0.0.3/AutoThemeGenerator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-05-07 12:20:33.000000 autothemegenerator-0.0.3/AutoThemeGenerator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-07 12:20:33.000000 autothemegenerator-0.0.3/AutoThemeGenerator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      275 2024-05-07 12:17:34.000000 autothemegenerator-0.0.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1067 2024-05-07 12:08:17.000000 autothemegenerator-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2024-05-07 12:08:18.000000 autothemegenerator-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3960 2024-05-07 12:20:33.927074 autothemegenerator-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3079 2024-05-07 12:08:19.000000 autothemegenerator-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-07 12:20:33.928073 autothemegenerator-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1320 2024-05-07 12:17:40.000000 autothemegenerator-0.0.3/setup.py
```

### Comparing `autothemegenerator-0.0.2/AutoThemeGenerator/AutoThemeGenerator.py` & `autothemegenerator-0.0.3/AutoThemeGenerator/AutoThemeGenerator.py`

 * *Files identical despite different names*

### Comparing `autothemegenerator-0.0.2/AutoThemeGenerator.egg-info/PKG-INFO` & `autothemegenerator-0.0.3/AutoThemeGenerator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoThemeGenerator
-Version: 0.0.2
+Version: 0.0.3
 Summary: Performing thematic analysis with OpenAI's GPT-4 models
 Author: Charles Alba
 Author-email: alba@wustl.edu
 Keywords: GPT models,Thematic analysis,OpenAI,Qualitiative studies,transcripts,interviews
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `autothemegenerator-0.0.2/LICENSE.txt` & `autothemegenerator-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autothemegenerator-0.0.2/PKG-INFO` & `autothemegenerator-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoThemeGenerator
-Version: 0.0.2
+Version: 0.0.3
 Summary: Performing thematic analysis with OpenAI's GPT-4 models
 Author: Charles Alba
 Author-email: alba@wustl.edu
 Keywords: GPT models,Thematic analysis,OpenAI,Qualitiative studies,transcripts,interviews
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `autothemegenerator-0.0.2/README.md` & `autothemegenerator-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `autothemegenerator-0.0.2/setup.py` & `autothemegenerator-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 readme_path = os.path.join(here, "README.md")
 with codecs.open(readme_path, encoding="utf-8") as fh:
     long_description = fh.read()
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Performing thematic analysis with OpenAI\'s GPT-4 models'
 LONG_DESCRIPTION = 'A package uses openAI\'s GPT-4 model to perform thematic analysis using interview transcripts from qualititative studies'
 
 # Setting up
 setup(
     name="AutoThemeGenerator",
     version=VERSION,
```

