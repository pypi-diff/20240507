# Comparing `tmp/dsi_cocoa-0.1.6.tar.gz` & `tmp/dsi_cocoa-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsi_cocoa-0.1.6.tar", last modified: Mon May  6 18:15:58 2024, max compression
+gzip compressed data, was "dsi_cocoa-0.1.7.tar", last modified: Mon May  6 18:22:24 2024, max compression
```

## Comparing `dsi_cocoa-0.1.6.tar` & `dsi_cocoa-0.1.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:15:58.282008 dsi_cocoa-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-06 18:15:53.000000 dsi_cocoa-0.1.6/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:15:58.274008 dsi_cocoa-0.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:15:58.278008 dsi_cocoa-0.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-06 18:15:53.000000 dsi_cocoa-0.1.6/.github/workflows/main.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-06 18:15:53.000000 dsi_cocoa-0.1.6/.github/workflows/publish.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-06 18:15:53.000000 dsi_cocoa-0.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-06 18:15:53.000000 dsi_cocoa-0.1.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-06 18:15:58.282008 dsi_cocoa-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-06 18:15:53.000000 dsi_cocoa-0.1.6/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-06 18:15:53.000000 dsi_cocoa-0.1.6/eval-repo.sh
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-06 18:15:53.000000 dsi_cocoa-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-06 18:15:53.000000 dsi_cocoa-0.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-06 18:15:58.282008 dsi_cocoa-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:15:58.274008 dsi_cocoa-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:15:58.278008 dsi_cocoa-0.1.6/src/cocoa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 18:15:53.000000 dsi_cocoa-0.1.6/src/cocoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-06 18:15:53.000000 dsi_cocoa-0.1.6/src/cocoa/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-06 18:15:53.000000 dsi_cocoa-0.1.6/src/cocoa/evaluate_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-06 18:15:53.000000 dsi_cocoa-0.1.6/src/cocoa/linting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-06 18:15:53.000000 dsi_cocoa-0.1.6/src/cocoa/notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-06 18:15:53.000000 dsi_cocoa-0.1.6/src/cocoa/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-06 18:15:53.000000 dsi_cocoa-0.1.6/src/cocoa/spring2024.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:15:58.282008 dsi_cocoa-0.1.6/src/dsi_cocoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-06 18:15:58.000000 dsi_cocoa-0.1.6/src/dsi_cocoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-06 18:15:58.000000 dsi_cocoa-0.1.6/src/dsi_cocoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 18:15:58.000000 dsi_cocoa-0.1.6/src/dsi_cocoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 18:15:58.000000 dsi_cocoa-0.1.6/src/dsi_cocoa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-06 18:15:58.000000 dsi_cocoa-0.1.6/src/dsi_cocoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 18:15:58.000000 dsi_cocoa-0.1.6/src/dsi_cocoa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:22:24.066199 dsi_cocoa-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-06 18:22:14.000000 dsi_cocoa-0.1.7/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:22:24.058199 dsi_cocoa-0.1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:22:24.062199 dsi_cocoa-0.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-06 18:22:14.000000 dsi_cocoa-0.1.7/.github/workflows/main.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-06 18:22:14.000000 dsi_cocoa-0.1.7/.github/workflows/publish.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-06 18:22:14.000000 dsi_cocoa-0.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-06 18:22:14.000000 dsi_cocoa-0.1.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-06 18:22:24.066199 dsi_cocoa-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-06 18:22:14.000000 dsi_cocoa-0.1.7/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-06 18:22:14.000000 dsi_cocoa-0.1.7/eval-repo.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-06 18:22:14.000000 dsi_cocoa-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-06 18:22:14.000000 dsi_cocoa-0.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-06 18:22:24.066199 dsi_cocoa-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:22:24.058199 dsi_cocoa-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:22:24.062199 dsi_cocoa-0.1.7/src/cocoa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 18:22:14.000000 dsi_cocoa-0.1.7/src/cocoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-06 18:22:14.000000 dsi_cocoa-0.1.7/src/cocoa/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-06 18:22:14.000000 dsi_cocoa-0.1.7/src/cocoa/evaluate_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-06 18:22:14.000000 dsi_cocoa-0.1.7/src/cocoa/linting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-06 18:22:14.000000 dsi_cocoa-0.1.7/src/cocoa/notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-06 18:22:14.000000 dsi_cocoa-0.1.7/src/cocoa/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-06 18:22:14.000000 dsi_cocoa-0.1.7/src/cocoa/spring2024.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:22:24.066199 dsi_cocoa-0.1.7/src/dsi_cocoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-06 18:22:24.000000 dsi_cocoa-0.1.7/src/dsi_cocoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-06 18:22:24.000000 dsi_cocoa-0.1.7/src/dsi_cocoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 18:22:24.000000 dsi_cocoa-0.1.7/src/dsi_cocoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 18:22:24.000000 dsi_cocoa-0.1.7/src/dsi_cocoa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-06 18:22:24.000000 dsi_cocoa-0.1.7/src/dsi_cocoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 18:22:24.000000 dsi_cocoa-0.1.7/src/dsi_cocoa.egg-info/top_level.txt
```

### Comparing `dsi_cocoa-0.1.6/.github/workflows/main.workflow.yml` & `dsi_cocoa-0.1.7/.github/workflows/main.workflow.yml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.6/.github/workflows/publish.workflow.yml` & `dsi_cocoa-0.1.7/.github/workflows/publish.workflow.yml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.6/.gitignore` & `dsi_cocoa-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.6/.pre-commit-config.yaml` & `dsi_cocoa-0.1.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.6/PKG-INFO` & `dsi_cocoa-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: dsi-cocoa
-Version: 0.1.6
+Version: 0.1.7
 Summary: Clinic Opinionated Codebase Oversight and Analysis
 Author-email: Nick Ross <tspread@uchicago.edu>, Trevor Spreadbury <tspread@uchicago.edu>
 Maintainer: Nick Ross, Trevor Spreadbury
 Keywords: codebase analysis,uchicago dsi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: GitPython
 Requires-Dist: pyflakes
 Requires-Dist: pylint
 Requires-Dist: nbconvert
 Requires-Dist: ipython
 Requires-Dist: termcolor
 Requires-Dist: black
+Requires-Dist: requests
 
 # Clinic Opinionated Codebase Oversight and Analysis
 
 This repository was developed in order to generate automated reports on how well codebases adhere to the [coding standards](https://github.com/dsi-clinic/coding-standards) of the University of Chicago's DSI [Clinic course](https://datascience.uchicago.edu/education/data-science-clinic/).
 
 The goals of this codebase is to provide a quick and easy way to review code and to alert contributors where their code may be failing.
```

### Comparing `dsi_cocoa-0.1.6/README.md` & `dsi_cocoa-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.6/pyproject.toml` & `dsi_cocoa-0.1.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 dependencies = [
     "GitPython",
     "pyflakes",
     "pylint",
     "nbconvert",
     "ipython",
     "termcolor",
-    "black", 
+    "black",
+    "requests" 
 ]
 
 [project.scripts]
 cocoa = "cocoa.evaluate_repo:main"
 
 [tool.setuptools_scm]
```

### Comparing `dsi_cocoa-0.1.6/src/cocoa/evaluate_repo.py` & `dsi_cocoa-0.1.7/src/cocoa/evaluate_repo.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.6/src/cocoa/linting.py` & `dsi_cocoa-0.1.7/src/cocoa/linting.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.6/src/cocoa/notebooks.py` & `dsi_cocoa-0.1.7/src/cocoa/notebooks.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.6/src/cocoa/repo.py` & `dsi_cocoa-0.1.7/src/cocoa/repo.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.6/src/cocoa/spring2024.py` & `dsi_cocoa-0.1.7/src/cocoa/spring2024.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.6/src/dsi_cocoa.egg-info/PKG-INFO` & `dsi_cocoa-0.1.7/src/dsi_cocoa.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: dsi-cocoa
-Version: 0.1.6
+Version: 0.1.7
 Summary: Clinic Opinionated Codebase Oversight and Analysis
 Author-email: Nick Ross <tspread@uchicago.edu>, Trevor Spreadbury <tspread@uchicago.edu>
 Maintainer: Nick Ross, Trevor Spreadbury
 Keywords: codebase analysis,uchicago dsi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: GitPython
 Requires-Dist: pyflakes
 Requires-Dist: pylint
 Requires-Dist: nbconvert
 Requires-Dist: ipython
 Requires-Dist: termcolor
 Requires-Dist: black
+Requires-Dist: requests
 
 # Clinic Opinionated Codebase Oversight and Analysis
 
 This repository was developed in order to generate automated reports on how well codebases adhere to the [coding standards](https://github.com/dsi-clinic/coding-standards) of the University of Chicago's DSI [Clinic course](https://datascience.uchicago.edu/education/data-science-clinic/).
 
 The goals of this codebase is to provide a quick and easy way to review code and to alert contributors where their code may be failing.
```

### Comparing `dsi_cocoa-0.1.6/src/dsi_cocoa.egg-info/SOURCES.txt` & `dsi_cocoa-0.1.7/src/dsi_cocoa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

