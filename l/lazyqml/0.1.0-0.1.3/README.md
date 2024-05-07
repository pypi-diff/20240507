# Comparing `tmp/lazyqml-0.1.0.tar.gz` & `tmp/lazyqml-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyqml-0.1.0.tar", last modified: Mon May  6 10:52:00 2024, max compression
+gzip compressed data, was "lazyqml-0.1.3.tar", last modified: Mon May  6 11:09:10 2024, max compression
```

## Comparing `lazyqml-0.1.0.tar` & `lazyqml-0.1.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:52:00.628927 lazyqml-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-06 10:51:28.000000 lazyqml-0.1.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:52:00.620927 lazyqml-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:52:00.620927 lazyqml-0.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-06 10:51:28.000000 lazyqml-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-06 10:51:28.000000 lazyqml-0.1.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-06 10:51:28.000000 lazyqml-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:52:00.624927 lazyqml-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-06 10:51:28.000000 lazyqml-0.1.0/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-06 10:51:28.000000 lazyqml-0.1.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-06 10:51:28.000000 lazyqml-0.1.0/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-06 10:51:28.000000 lazyqml-0.1.0/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-06 10:51:28.000000 lazyqml-0.1.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-06 10:51:28.000000 lazyqml-0.1.0/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-06 10:51:28.000000 lazyqml-0.1.0/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-06 10:51:28.000000 lazyqml-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-06 10:51:28.000000 lazyqml-0.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-06 10:51:28.000000 lazyqml-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-06 10:51:28.000000 lazyqml-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-06 10:52:00.628927 lazyqml-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-06 10:51:28.000000 lazyqml-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:52:00.624927 lazyqml-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-06 10:51:28.000000 lazyqml-0.1.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-06 10:51:28.000000 lazyqml-0.1.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 10:51:28.000000 lazyqml-0.1.0/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-06 10:51:28.000000 lazyqml-0.1.0/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:52:00.624927 lazyqml-0.1.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-06 10:51:28.000000 lazyqml-0.1.0/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 10:51:28.000000 lazyqml-0.1.0/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-06 10:51:28.000000 lazyqml-0.1.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-06 10:51:28.000000 lazyqml-0.1.0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-06 10:51:28.000000 lazyqml-0.1.0/docs/lazyqml.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:52:00.624927 lazyqml-0.1.0/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-06 10:51:28.000000 lazyqml-0.1.0/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-06 10:51:28.000000 lazyqml-0.1.0/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:52:00.624927 lazyqml-0.1.0/lazyqml/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-06 10:51:28.000000 lazyqml-0.1.0/lazyqml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22448 2024-05-06 10:51:28.000000 lazyqml-0.1.0/lazyqml/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    17507 2024-05-06 10:51:28.000000 lazyqml-0.1.0/lazyqml/supervised.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:52:00.624927 lazyqml-0.1.0/lazyqml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-06 10:52:00.000000 lazyqml-0.1.0/lazyqml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-06 10:52:00.000000 lazyqml-0.1.0/lazyqml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 10:52:00.000000 lazyqml-0.1.0/lazyqml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-06 10:52:00.000000 lazyqml-0.1.0/lazyqml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-06 10:52:00.000000 lazyqml-0.1.0/lazyqml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-06 10:52:00.000000 lazyqml-0.1.0/lazyqml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-06 10:51:28.000000 lazyqml-0.1.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-06 10:51:28.000000 lazyqml-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-06 10:51:28.000000 lazyqml-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-06 10:51:28.000000 lazyqml-0.1.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 10:52:00.628927 lazyqml-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:52:00.624927 lazyqml-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-06 10:51:28.000000 lazyqml-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-06 10:51:28.000000 lazyqml-0.1.0/tests/test_lazyqml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:10.743124 lazyqml-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-06 11:09:00.000000 lazyqml-0.1.3/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:10.731124 lazyqml-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:10.735124 lazyqml-0.1.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-06 11:09:00.000000 lazyqml-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-06 11:09:00.000000 lazyqml-0.1.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-06 11:09:00.000000 lazyqml-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:10.735124 lazyqml-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-06 11:09:00.000000 lazyqml-0.1.3/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-06 11:09:00.000000 lazyqml-0.1.3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-06 11:09:00.000000 lazyqml-0.1.3/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-06 11:09:00.000000 lazyqml-0.1.3/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-06 11:09:00.000000 lazyqml-0.1.3/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-06 11:09:00.000000 lazyqml-0.1.3/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-06 11:09:00.000000 lazyqml-0.1.3/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-06 11:09:00.000000 lazyqml-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-06 11:09:00.000000 lazyqml-0.1.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-06 11:09:00.000000 lazyqml-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-06 11:09:00.000000 lazyqml-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-06 11:09:10.743124 lazyqml-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-06 11:09:00.000000 lazyqml-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:10.739124 lazyqml-0.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-06 11:09:00.000000 lazyqml-0.1.3/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-06 11:09:00.000000 lazyqml-0.1.3/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 11:09:00.000000 lazyqml-0.1.3/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-06 11:09:00.000000 lazyqml-0.1.3/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:10.739124 lazyqml-0.1.3/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-06 11:09:00.000000 lazyqml-0.1.3/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 11:09:00.000000 lazyqml-0.1.3/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-06 11:09:00.000000 lazyqml-0.1.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-06 11:09:00.000000 lazyqml-0.1.3/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-06 11:09:00.000000 lazyqml-0.1.3/docs/lazyqml.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:10.739124 lazyqml-0.1.3/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-06 11:09:00.000000 lazyqml-0.1.3/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-06 11:09:00.000000 lazyqml-0.1.3/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:10.739124 lazyqml-0.1.3/lazyqml/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-06 11:09:00.000000 lazyqml-0.1.3/lazyqml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22448 2024-05-06 11:09:00.000000 lazyqml-0.1.3/lazyqml/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17114 2024-05-06 11:09:00.000000 lazyqml-0.1.3/lazyqml/supervised.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:10.739124 lazyqml-0.1.3/lazyqml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-06 11:09:10.000000 lazyqml-0.1.3/lazyqml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-06 11:09:10.000000 lazyqml-0.1.3/lazyqml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 11:09:10.000000 lazyqml-0.1.3/lazyqml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-06 11:09:10.000000 lazyqml-0.1.3/lazyqml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-06 11:09:10.000000 lazyqml-0.1.3/lazyqml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-06 11:09:10.000000 lazyqml-0.1.3/lazyqml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-06 11:09:00.000000 lazyqml-0.1.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-06 11:09:00.000000 lazyqml-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-06 11:09:00.000000 lazyqml-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-06 11:09:00.000000 lazyqml-0.1.3/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 11:09:10.743124 lazyqml-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:10.739124 lazyqml-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-06 11:09:00.000000 lazyqml-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-06 11:09:00.000000 lazyqml-0.1.3/tests/test_lazyqml.py
```

### Comparing `lazyqml-0.1.0/.github/workflows/docs-build.yml` & `lazyqml-0.1.3/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.1.0/.github/workflows/docs.yml` & `lazyqml-0.1.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.1.0/.github/workflows/installation.yml` & `lazyqml-0.1.3/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.1.0/.github/workflows/macos.yml` & `lazyqml-0.1.3/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.1.0/.github/workflows/pypi.yml` & `lazyqml-0.1.3/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.1.0/.github/workflows/ubuntu.yml` & `lazyqml-0.1.3/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.1.0/.github/workflows/windows.yml` & `lazyqml-0.1.3/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.1.0/.gitignore` & `lazyqml-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lazyqml-0.1.0/LICENSE` & `lazyqml-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lazyqml-0.1.0/PKG-INFO` & `lazyqml-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: lazyqml
-Version: 0.1.0
+Version: 0.1.3
 Summary: LazyQML benchmarking utility to test quantum machine learning models.
-Author-email: Diego García Vega <garciavdiego@uniovi.es>
+Author-email: Diego García Vega <garciavdiego@uniovi.es>, Fernando Álvaro Plou Llorente <ploufernando@uniovi.es>, Alejandro Leal Castaño <lealcalejandro@uniovi.es>
 License: MIT License
 Project-URL: Homepage, https://github.com/DiegoGV-Uniovi/lazyqml
 Keywords: lazyqml
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `lazyqml-0.1.0/docs/contributing.md` & `lazyqml-0.1.3/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `lazyqml-0.1.0/docs/installation.md` & `lazyqml-0.1.3/docs/installation.md`

 * *Files identical despite different names*

### Comparing `lazyqml-0.1.0/lazyqml/common.py` & `lazyqml-0.1.3/lazyqml/common.py`

 * *Files identical despite different names*

### Comparing `lazyqml-0.1.0/lazyqml/supervised.py` & `lazyqml-0.1.3/lazyqml/supervised.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Main Module
 #======================================================================================
 
 """
  Import modules
 """
 
-from common import *
+from .common import *
 
 """
  Classifiers
 """
 
 ansatzs = ['hardware_efficient','tree_tensor','two_local','HPzRx']
 
@@ -346,24 +346,11 @@
             "Model"
         )
         if self.predictions:
             predictions_df = pd.DataFrame.from_dict(predictions)
         return scores, predictions_df if self.predictions is True else scores
 
 
-from sklearn.datasets import load_breast_cancer, load_iris
-from sklearn.model_selection import train_test_split
-data = load_iris()
-X = data.data
-y = data.target
-print(y)
 
-X_train, X_test, y_train, y_test = train_test_split(X, y,test_size=.3,random_state =123)  
-
-q = QuantumClassifier(nqubits=4,classifiers=["qnn_bag"],verbose=0)
-
-scores = q.fit(X_train, X_test, y_train, y_test)
-
-print(scores)
```

### Comparing `lazyqml-0.1.0/lazyqml.egg-info/PKG-INFO` & `lazyqml-0.1.3/lazyqml.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: lazyqml
-Version: 0.1.0
+Version: 0.1.3
 Summary: LazyQML benchmarking utility to test quantum machine learning models.
-Author-email: Diego García Vega <garciavdiego@uniovi.es>
+Author-email: Diego García Vega <garciavdiego@uniovi.es>, Fernando Álvaro Plou Llorente <ploufernando@uniovi.es>, Alejandro Leal Castaño <lealcalejandro@uniovi.es>
 License: MIT License
 Project-URL: Homepage, https://github.com/DiegoGV-Uniovi/lazyqml
 Keywords: lazyqml
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `lazyqml-0.1.0/lazyqml.egg-info/SOURCES.txt` & `lazyqml-0.1.3/lazyqml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lazyqml-0.1.0/lazyqml.egg-info/requires.txt` & `lazyqml-0.1.3/lazyqml.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `lazyqml-0.1.0/mkdocs.yml` & `lazyqml-0.1.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.1.0/pyproject.toml` & `lazyqml-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [project]
 name = "lazyqml"
-version = "0.1.0"
+version = "0.1.3"
 dynamic = [
     "dependencies",
 ]
 description = "LazyQML benchmarking utility to test quantum machine learning models."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
     "lazyqml",
 ]
 license = {text = "MIT License"}
 authors = [
   {name = "Diego García Vega", email = "garciavdiego@uniovi.es"},
+  {name = "Fernando Álvaro Plou Llorente", email = "ploufernando@uniovi.es"},
+  {name = "Alejandro Leal Castaño", email = "lealcalejandro@uniovi.es"}
 ]
 classifiers = [
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3.9"
 ]
@@ -44,15 +46,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.1.0"
+current_version = "0.1.3"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `lazyqml-0.1.0/requirements.txt` & `lazyqml-0.1.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `lazyqml-0.1.0/requirements_dev.txt` & `lazyqml-0.1.3/requirements_dev.txt`

 * *Files identical despite different names*

