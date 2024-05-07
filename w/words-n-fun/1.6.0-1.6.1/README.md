# Comparing `tmp/words_n_fun-1.6.0.tar.gz` & `tmp/words_n_fun-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "words_n_fun-1.6.0.tar", last modified: Fri Oct 13 09:14:12 2023, max compression
+gzip compressed data, was "words_n_fun-1.6.1.tar", last modified: Tue May  7 07:31:34 2024, max compression
```

## Comparing `words_n_fun-1.6.0.tar` & `words_n_fun-1.6.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 09:14:12.094347 words_n_fun-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    31709 2023-10-13 09:14:05.000000 words_n_fun-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2023-10-13 09:14:12.094347 words_n_fun-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2023-10-13 09:14:05.000000 words_n_fun-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-13 09:14:12.094347 words_n_fun-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2023-10-13 09:14:05.000000 words_n_fun-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 09:14:12.090347 words_n_fun-1.6.0/words_n_fun/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-10-13 09:14:05.000000 words_n_fun-1.6.0/words_n_fun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 09:14:12.090347 words_n_fun-1.6.0/words_n_fun/configs/
--rw-r--r--   0 runner    (1001) docker     (127)     7230 2023-10-13 09:14:05.000000 words_n_fun-1.6.0/words_n_fun/configs/pipeline_usage_order.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 09:14:12.090347 words_n_fun-1.6.0/words_n_fun/nltk_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 09:14:12.090347 words_n_fun-1.6.0/words_n_fun/nltk_data/corpora/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 09:14:12.090347 words_n_fun-1.6.0/words_n_fun/nltk_data/corpora/stopwords/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-10-13 09:14:05.000000 words_n_fun-1.6.0/words_n_fun/nltk_data/corpora/stopwords/french
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 09:14:12.094347 words_n_fun-1.6.0/words_n_fun/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-13 09:14:05.000000 words_n_fun-1.6.0/words_n_fun/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26556 2023-10-13 09:14:05.000000 words_n_fun-1.6.0/words_n_fun/preprocessing/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22086 2023-10-13 09:14:05.000000 words_n_fun-1.6.0/words_n_fun/preprocessing/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2023-10-13 09:14:05.000000 words_n_fun-1.6.0/words_n_fun/preprocessing/lemmatizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2023-10-13 09:14:05.000000 words_n_fun-1.6.0/words_n_fun/preprocessing/split_sentences.py
--rw-r--r--   0 runner    (1001) docker     (127)    13197 2023-10-13 09:14:05.000000 words_n_fun-1.6.0/words_n_fun/preprocessing/stopwords.py
--rw-r--r--   0 runner    (1001) docker     (127)     8255 2023-10-13 09:14:05.000000 words_n_fun-1.6.0/words_n_fun/preprocessing/synonym_malefemale_replacement.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2023-10-13 09:14:05.000000 words_n_fun-1.6.0/words_n_fun/preprocessing/vectorization_tokenization.py
--rw-r--r--   0 runner    (1001) docker     (127)    38354 2023-10-13 09:14:05.000000 words_n_fun-1.6.0/words_n_fun/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 09:14:12.090347 words_n_fun-1.6.0/words_n_fun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2023-10-13 09:14:12.000000 words_n_fun-1.6.0/words_n_fun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      684 2023-10-13 09:14:12.000000 words_n_fun-1.6.0/words_n_fun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-13 09:14:12.000000 words_n_fun-1.6.0/words_n_fun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-10-13 09:14:12.000000 words_n_fun-1.6.0/words_n_fun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-13 09:14:12.000000 words_n_fun-1.6.0/words_n_fun.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:31:34.134466 words_n_fun-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    31709 2024-05-07 07:31:30.000000 words_n_fun-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-07 07:31:34.130466 words_n_fun-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-07 07:31:30.000000 words_n_fun-1.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:31:34.134466 words_n_fun-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-07 07:31:30.000000 words_n_fun-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:31:34.130466 words_n_fun-1.6.1/words_n_fun/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-07 07:31:30.000000 words_n_fun-1.6.1/words_n_fun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:31:34.130466 words_n_fun-1.6.1/words_n_fun/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-05-07 07:31:30.000000 words_n_fun-1.6.1/words_n_fun/configs/pipeline_usage_order.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:31:34.130466 words_n_fun-1.6.1/words_n_fun/nltk_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:31:34.130466 words_n_fun-1.6.1/words_n_fun/nltk_data/corpora/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:31:34.130466 words_n_fun-1.6.1/words_n_fun/nltk_data/corpora/stopwords/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-07 07:31:30.000000 words_n_fun-1.6.1/words_n_fun/nltk_data/corpora/stopwords/french
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:31:34.130466 words_n_fun-1.6.1/words_n_fun/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:31:30.000000 words_n_fun-1.6.1/words_n_fun/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26556 2024-05-07 07:31:30.000000 words_n_fun-1.6.1/words_n_fun/preprocessing/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22086 2024-05-07 07:31:30.000000 words_n_fun-1.6.1/words_n_fun/preprocessing/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-07 07:31:30.000000 words_n_fun-1.6.1/words_n_fun/preprocessing/lemmatizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-05-07 07:31:30.000000 words_n_fun-1.6.1/words_n_fun/preprocessing/split_sentences.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13197 2024-05-07 07:31:30.000000 words_n_fun-1.6.1/words_n_fun/preprocessing/stopwords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-05-07 07:31:30.000000 words_n_fun-1.6.1/words_n_fun/preprocessing/synonym_malefemale_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-07 07:31:30.000000 words_n_fun-1.6.1/words_n_fun/preprocessing/vectorization_tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38354 2024-05-07 07:31:30.000000 words_n_fun-1.6.1/words_n_fun/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:31:34.130466 words_n_fun-1.6.1/words_n_fun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-07 07:31:34.000000 words_n_fun-1.6.1/words_n_fun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-07 07:31:34.000000 words_n_fun-1.6.1/words_n_fun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:31:34.000000 words_n_fun-1.6.1/words_n_fun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-07 07:31:34.000000 words_n_fun-1.6.1/words_n_fun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 07:31:34.000000 words_n_fun-1.6.1/words_n_fun.egg-info/top_level.txt
```

### Comparing `words_n_fun-1.6.0/LICENSE` & `words_n_fun-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `words_n_fun-1.6.0/PKG-INFO` & `words_n_fun-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: words_n_fun
-Version: 1.6.0
+Version: 1.6.1
 Summary: Semantic library of the Data Services agency
 Home-page: https://github.com/OSS-Pole-Emploi/words_n_fun
 Author: Agence Data Services PE Nantes
 Author-email: contactadsaiframeworks.00619@pole-emploi.fr
 License: AGPL-3.0
 Platform: windows
 Platform: linux
```

### Comparing `words_n_fun-1.6.0/README.md` & `words_n_fun-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `words_n_fun-1.6.0/setup.py` & `words_n_fun-1.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `words_n_fun-1.6.0/words_n_fun/__init__.py` & `words_n_fun-1.6.1/words_n_fun/__init__.py`

 * *Files identical despite different names*

### Comparing `words_n_fun-1.6.0/words_n_fun/configs/pipeline_usage_order.json` & `words_n_fun-1.6.1/words_n_fun/configs/pipeline_usage_order.json`

 * *Files identical despite different names*

### Comparing `words_n_fun-1.6.0/words_n_fun/nltk_data/corpora/stopwords/french` & `words_n_fun-1.6.1/words_n_fun/nltk_data/corpora/stopwords/french`

 * *Files identical despite different names*

### Comparing `words_n_fun-1.6.0/words_n_fun/preprocessing/api.py` & `words_n_fun-1.6.1/words_n_fun/preprocessing/api.py`

 * *Files identical despite different names*

### Comparing `words_n_fun-1.6.0/words_n_fun/preprocessing/basic.py` & `words_n_fun-1.6.1/words_n_fun/preprocessing/basic.py`

 * *Files identical despite different names*

### Comparing `words_n_fun-1.6.0/words_n_fun/preprocessing/lemmatizer.py` & `words_n_fun-1.6.1/words_n_fun/preprocessing/lemmatizer.py`

 * *Files identical despite different names*

### Comparing `words_n_fun-1.6.0/words_n_fun/preprocessing/stopwords.py` & `words_n_fun-1.6.1/words_n_fun/preprocessing/stopwords.py`

 * *Files identical despite different names*

### Comparing `words_n_fun-1.6.0/words_n_fun/preprocessing/synonym_malefemale_replacement.py` & `words_n_fun-1.6.1/words_n_fun/preprocessing/synonym_malefemale_replacement.py`

 * *Files identical despite different names*

### Comparing `words_n_fun-1.6.0/words_n_fun/preprocessing/vectorization_tokenization.py` & `words_n_fun-1.6.1/words_n_fun/preprocessing/vectorization_tokenization.py`

 * *Files identical despite different names*

### Comparing `words_n_fun-1.6.0/words_n_fun/utils.py` & `words_n_fun-1.6.1/words_n_fun/utils.py`

 * *Files identical despite different names*

### Comparing `words_n_fun-1.6.0/words_n_fun.egg-info/PKG-INFO` & `words_n_fun-1.6.1/words_n_fun.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: words-n-fun
-Version: 1.6.0
+Version: 1.6.1
 Summary: Semantic library of the Data Services agency
 Home-page: https://github.com/OSS-Pole-Emploi/words_n_fun
 Author: Agence Data Services PE Nantes
 Author-email: contactadsaiframeworks.00619@pole-emploi.fr
 License: AGPL-3.0
 Platform: windows
 Platform: linux
```

### Comparing `words_n_fun-1.6.0/words_n_fun.egg-info/SOURCES.txt` & `words_n_fun-1.6.1/words_n_fun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

