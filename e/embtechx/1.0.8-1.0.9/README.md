# Comparing `tmp/embtechx-1.0.8.tar.gz` & `tmp/embtechx-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embtechx-1.0.8.tar", last modified: Thu May  2 07:19:55 2024, max compression
+gzip compressed data, was "embtechx-1.0.9.tar", last modified: Tue May  7 03:26:38 2024, max compression
```

## Comparing `embtechx-1.0.8.tar` & `embtechx-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-05-02 07:19:55.402247 embtechx-1.0.8/
--rw-r--r--   0 ninananakorn   (501) staff       (20)      258 2024-05-02 07:19:55.401666 embtechx-1.0.8/PKG-INFO
-drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-05-02 07:19:55.396612 embtechx-1.0.8/embtechx/
--rw-r--r--   0 ninananakorn   (501) staff       (20)      860 2024-05-02 03:52:37.000000 embtechx-1.0.8/embtechx/__init__.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     3182 2024-05-02 07:18:44.000000 embtechx-1.0.8/embtechx/dataframe.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     2445 2024-05-02 07:18:50.000000 embtechx-1.0.8/embtechx/domain_emb.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     7424 2024-05-02 07:19:35.000000 embtechx-1.0.8/embtechx/embedding.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     8300 2024-05-02 07:19:19.000000 embtechx-1.0.8/embtechx/evaluate.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     2184 2024-05-02 07:19:25.000000 embtechx-1.0.8/embtechx/search.py
-drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-05-02 07:19:55.401225 embtechx-1.0.8/embtechx.egg-info/
--rw-r--r--   0 ninananakorn   (501) staff       (20)      258 2024-05-02 07:19:55.000000 embtechx-1.0.8/embtechx.egg-info/PKG-INFO
--rw-r--r--   0 ninananakorn   (501) staff       (20)      295 2024-05-02 07:19:55.000000 embtechx-1.0.8/embtechx.egg-info/SOURCES.txt
--rw-r--r--   0 ninananakorn   (501) staff       (20)        1 2024-05-02 07:19:55.000000 embtechx-1.0.8/embtechx.egg-info/dependency_links.txt
--rw-r--r--   0 ninananakorn   (501) staff       (20)       86 2024-05-02 07:19:55.000000 embtechx-1.0.8/embtechx.egg-info/requires.txt
--rw-r--r--   0 ninananakorn   (501) staff       (20)        9 2024-05-02 07:19:55.000000 embtechx-1.0.8/embtechx.egg-info/top_level.txt
--rw-r--r--   0 ninananakorn   (501) staff       (20)       38 2024-05-02 07:19:55.402308 embtechx-1.0.8/setup.cfg
--rw-r--r--   0 ninananakorn   (501) staff       (20)      364 2024-05-02 07:18:32.000000 embtechx-1.0.8/setup.py
+drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-05-07 03:26:38.656349 embtechx-1.0.9/
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      258 2024-05-07 03:26:38.655617 embtechx-1.0.9/PKG-INFO
+drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-05-07 03:26:38.651974 embtechx-1.0.9/embtechx/
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      834 2024-05-07 03:25:51.000000 embtechx-1.0.9/embtechx/__init__.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     3182 2024-05-07 03:25:50.000000 embtechx-1.0.9/embtechx/dataframe.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     7424 2024-05-07 03:25:50.000000 embtechx-1.0.9/embtechx/embedding.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     8300 2024-05-07 03:25:48.000000 embtechx-1.0.9/embtechx/evaluate.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     2184 2024-05-07 03:25:49.000000 embtechx-1.0.9/embtechx/search.py
+drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-05-07 03:26:38.655242 embtechx-1.0.9/embtechx.egg-info/
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      258 2024-05-07 03:26:38.000000 embtechx-1.0.9/embtechx.egg-info/PKG-INFO
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      272 2024-05-07 03:26:38.000000 embtechx-1.0.9/embtechx.egg-info/SOURCES.txt
+-rw-r--r--   0 ninananakorn   (501) staff       (20)        1 2024-05-07 03:26:38.000000 embtechx-1.0.9/embtechx.egg-info/dependency_links.txt
+-rw-r--r--   0 ninananakorn   (501) staff       (20)       86 2024-05-07 03:26:38.000000 embtechx-1.0.9/embtechx.egg-info/requires.txt
+-rw-r--r--   0 ninananakorn   (501) staff       (20)        9 2024-05-07 03:26:38.000000 embtechx-1.0.9/embtechx.egg-info/top_level.txt
+-rw-r--r--   0 ninananakorn   (501) staff       (20)       38 2024-05-07 03:26:38.656397 embtechx-1.0.9/setup.cfg
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      364 2024-05-07 03:25:52.000000 embtechx-1.0.9/setup.py
```

### Comparing `embtechx-1.0.8/embtechx/__init__.py` & `embtechx-1.0.9/embtechx/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,12 +15,11 @@
 evaluate = eval_model.evaluate
 evaluate_svm = eval_model.accuracy_svm
 evaluate_knn = eval_model.accuracy_knn
 evaluate_naive_bayes = eval_model.accuracy_naive_bayes
 evaluate_pca = eval_model.evaluate_pca
 evaluate_tsne = eval_model.evaluate_tsne
 
-from .domain_emb import *
 from .search import *
 
 import os
 os.environ["TOKENIZERS_PARALLELISM"] = "false"
```

### Comparing `embtechx-1.0.8/embtechx/dataframe.py` & `embtechx-1.0.9/embtechx/dataframe.py`

 * *Files identical despite different names*

### Comparing `embtechx-1.0.8/embtechx/embedding.py` & `embtechx-1.0.9/embtechx/embedding.py`

 * *Files identical despite different names*

### Comparing `embtechx-1.0.8/embtechx/evaluate.py` & `embtechx-1.0.9/embtechx/evaluate.py`

 * *Files identical despite different names*

### Comparing `embtechx-1.0.8/embtechx/search.py` & `embtechx-1.0.9/embtechx/search.py`

 * *Files identical despite different names*

