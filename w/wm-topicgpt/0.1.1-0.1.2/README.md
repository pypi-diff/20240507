# Comparing `tmp/wm_topicgpt-0.1.1.tar.gz` & `tmp/wm_topicgpt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wm_topicgpt-0.1.1.tar", last modified: Tue May  7 14:28:45 2024, max compression
+gzip compressed data, was "wm_topicgpt-0.1.2.tar", last modified: Tue May  7 14:44:10 2024, max compression
```

## Comparing `wm_topicgpt-0.1.1.tar` & `wm_topicgpt-0.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:28:45.781172 wm_topicgpt-0.1.1/
--rw-r--r--   0 y0h07pr    (503) staff       (20)     7103 2024-05-07 14:28:45.780643 wm_topicgpt-0.1.1/PKG-INFO
--rw-r--r--   0 y0h07pr    (503) staff       (20)       38 2024-05-07 14:28:45.781237 wm_topicgpt-0.1.1/setup.cfg
--rw-r--r--   0 y0h07pr    (503) staff       (20)      601 2024-05-07 14:26:28.000000 wm_topicgpt-0.1.1/setup.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:28:45.752493 wm_topicgpt-0.1.1/topicgpt/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      209 2024-05-07 14:20:30.000000 wm_topicgpt-0.1.1/topicgpt/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      312 2024-05-05 05:35:46.000000 wm_topicgpt-0.1.1/topicgpt/_config.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      276 2024-05-04 00:03:35.000000 wm_topicgpt-0.1.1/topicgpt/base.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:28:45.755743 wm_topicgpt-0.1.1/topicgpt/clustering/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      191 2024-05-05 22:35:15.000000 wm_topicgpt-0.1.1/topicgpt/clustering/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      428 2024-05-06 03:49:21.000000 wm_topicgpt-0.1.1/topicgpt/clustering/_base_cluster.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     3035 2024-05-06 14:14:30.000000 wm_topicgpt-0.1.1/topicgpt/clustering/_hdbscan.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)    10045 2024-05-06 18:24:02.000000 wm_topicgpt-0.1.1/topicgpt/clustering/_kmeans.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     2285 2024-05-05 03:15:39.000000 wm_topicgpt-0.1.1/topicgpt/clustering/_sampling.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:28:45.757913 wm_topicgpt-0.1.1/topicgpt/generation/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      138 2024-05-06 16:56:29.000000 wm_topicgpt-0.1.1/topicgpt/generation/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     2910 2024-05-07 01:27:18.000000 wm_topicgpt-0.1.1/topicgpt/generation/_keywords.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     5501 2024-05-06 19:42:11.000000 wm_topicgpt-0.1.1/topicgpt/generation/_topic.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:28:45.761834 wm_topicgpt-0.1.1/topicgpt/persistence/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      330 2024-05-07 01:26:00.000000 wm_topicgpt-0.1.1/topicgpt/persistence/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     1012 2024-05-06 03:42:53.000000 wm_topicgpt-0.1.1/topicgpt/persistence/_plot.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     4297 2024-05-07 03:09:02.000000 wm_topicgpt-0.1.1/topicgpt/persistence/_save.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     5360 2024-05-07 14:20:10.000000 wm_topicgpt-0.1.1/topicgpt/pipeline.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:28:45.764564 wm_topicgpt-0.1.1/topicgpt/preprocessing/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      108 2024-05-03 23:14:55.000000 wm_topicgpt-0.1.1/topicgpt/preprocessing/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     2854 2024-05-03 23:14:55.000000 wm_topicgpt-0.1.1/topicgpt/preprocessing/_data.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      412 2024-05-06 00:04:30.000000 wm_topicgpt-0.1.1/topicgpt/utils.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:28:45.771575 wm_topicgpt-0.1.1/topicgpt/walmart_llm/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      153 2024-05-03 23:24:30.000000 wm_topicgpt-0.1.1/topicgpt/walmart_llm/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     9052 2024-05-03 23:35:49.000000 wm_topicgpt-0.1.1/topicgpt/walmart_llm/_chat_model.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     8079 2024-05-03 20:57:39.000000 wm_topicgpt-0.1.1/topicgpt/walmart_llm/_embed_model.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     7922 2024-05-03 23:35:53.000000 wm_topicgpt-0.1.1/topicgpt/walmart_llm/_llm_client.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:28:45.779908 wm_topicgpt-0.1.1/wm_topicgpt.egg-info/
--rw-r--r--   0 y0h07pr    (503) staff       (20)     7103 2024-05-07 14:28:45.000000 wm_topicgpt-0.1.1/wm_topicgpt.egg-info/PKG-INFO
--rw-r--r--   0 y0h07pr    (503) staff       (20)      841 2024-05-07 14:28:45.000000 wm_topicgpt-0.1.1/wm_topicgpt.egg-info/SOURCES.txt
--rw-r--r--   0 y0h07pr    (503) staff       (20)        1 2024-05-07 14:28:45.000000 wm_topicgpt-0.1.1/wm_topicgpt.egg-info/dependency_links.txt
--rw-r--r--   0 y0h07pr    (503) staff       (20)      360 2024-05-07 14:28:45.000000 wm_topicgpt-0.1.1/wm_topicgpt.egg-info/requires.txt
--rw-r--r--   0 y0h07pr    (503) staff       (20)        9 2024-05-07 14:28:45.000000 wm_topicgpt-0.1.1/wm_topicgpt.egg-info/top_level.txt
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:44:10.255239 wm_topicgpt-0.1.2/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     7103 2024-05-07 14:44:10.254460 wm_topicgpt-0.1.2/PKG-INFO
+-rw-r--r--   0 y0h07pr    (503) staff       (20)       38 2024-05-07 14:44:10.255307 wm_topicgpt-0.1.2/setup.cfg
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      601 2024-05-07 14:43:37.000000 wm_topicgpt-0.1.2/setup.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:44:10.224916 wm_topicgpt-0.1.2/topicgpt/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      209 2024-05-07 14:20:30.000000 wm_topicgpt-0.1.2/topicgpt/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      312 2024-05-05 05:35:46.000000 wm_topicgpt-0.1.2/topicgpt/_config.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      276 2024-05-04 00:03:35.000000 wm_topicgpt-0.1.2/topicgpt/base.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:44:10.228474 wm_topicgpt-0.1.2/topicgpt/clustering/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      191 2024-05-05 22:35:15.000000 wm_topicgpt-0.1.2/topicgpt/clustering/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      428 2024-05-06 03:49:21.000000 wm_topicgpt-0.1.2/topicgpt/clustering/_base_cluster.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     3035 2024-05-06 14:14:30.000000 wm_topicgpt-0.1.2/topicgpt/clustering/_hdbscan.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)    10045 2024-05-06 18:24:02.000000 wm_topicgpt-0.1.2/topicgpt/clustering/_kmeans.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     2285 2024-05-05 03:15:39.000000 wm_topicgpt-0.1.2/topicgpt/clustering/_sampling.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:44:10.230316 wm_topicgpt-0.1.2/topicgpt/generation/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      138 2024-05-06 16:56:29.000000 wm_topicgpt-0.1.2/topicgpt/generation/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     2910 2024-05-07 01:27:18.000000 wm_topicgpt-0.1.2/topicgpt/generation/_keywords.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     5501 2024-05-06 19:42:11.000000 wm_topicgpt-0.1.2/topicgpt/generation/_topic.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:44:10.233978 wm_topicgpt-0.1.2/topicgpt/persistence/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      330 2024-05-07 01:26:00.000000 wm_topicgpt-0.1.2/topicgpt/persistence/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     1012 2024-05-06 03:42:53.000000 wm_topicgpt-0.1.2/topicgpt/persistence/_plot.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     4297 2024-05-07 03:09:02.000000 wm_topicgpt-0.1.2/topicgpt/persistence/_save.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     5375 2024-05-07 14:43:13.000000 wm_topicgpt-0.1.2/topicgpt/pipeline.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:44:10.237681 wm_topicgpt-0.1.2/topicgpt/preprocessing/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      108 2024-05-03 23:14:55.000000 wm_topicgpt-0.1.2/topicgpt/preprocessing/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     2854 2024-05-03 23:14:55.000000 wm_topicgpt-0.1.2/topicgpt/preprocessing/_data.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      412 2024-05-06 00:04:30.000000 wm_topicgpt-0.1.2/topicgpt/utils.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:44:10.242231 wm_topicgpt-0.1.2/topicgpt/walmart_llm/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      153 2024-05-03 23:24:30.000000 wm_topicgpt-0.1.2/topicgpt/walmart_llm/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     9052 2024-05-03 23:35:49.000000 wm_topicgpt-0.1.2/topicgpt/walmart_llm/_chat_model.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     8079 2024-05-03 20:57:39.000000 wm_topicgpt-0.1.2/topicgpt/walmart_llm/_embed_model.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     7922 2024-05-03 23:35:53.000000 wm_topicgpt-0.1.2/topicgpt/walmart_llm/_llm_client.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:44:10.253030 wm_topicgpt-0.1.2/wm_topicgpt.egg-info/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     7103 2024-05-07 14:44:10.000000 wm_topicgpt-0.1.2/wm_topicgpt.egg-info/PKG-INFO
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      841 2024-05-07 14:44:10.000000 wm_topicgpt-0.1.2/wm_topicgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 y0h07pr    (503) staff       (20)        1 2024-05-07 14:44:10.000000 wm_topicgpt-0.1.2/wm_topicgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      360 2024-05-07 14:44:10.000000 wm_topicgpt-0.1.2/wm_topicgpt.egg-info/requires.txt
+-rw-r--r--   0 y0h07pr    (503) staff       (20)        9 2024-05-07 14:44:10.000000 wm_topicgpt-0.1.2/wm_topicgpt.egg-info/top_level.txt
```

### Comparing `wm_topicgpt-0.1.1/PKG-INFO` & `wm_topicgpt-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wm_topicgpt
-Version: 0.1.1
+Version: 0.1.2
 Summary: This is a package to generate topics for the text corpus.
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: numpy==1.26.4
 Requires-Dist: pandas==2.2.1
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: azure-ai-textanalytics==5.3.0
```

### Comparing `wm_topicgpt-0.1.1/setup.py` & `wm_topicgpt-0.1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     install_requires = f.read().splitlines()
 
 with open("topicgpt/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='wm_topicgpt',
-    version='0.1.1',
+    version='0.1.2',
     description='This is a package to generate topics for the text corpus.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=install_requires,
     python_requires='>=3.9',
 )
```

### Comparing `wm_topicgpt-0.1.1/topicgpt/clustering/_hdbscan.py` & `wm_topicgpt-0.1.2/topicgpt/clustering/_hdbscan.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.1.1/topicgpt/clustering/_kmeans.py` & `wm_topicgpt-0.1.2/topicgpt/clustering/_kmeans.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.1.1/topicgpt/clustering/_sampling.py` & `wm_topicgpt-0.1.2/topicgpt/clustering/_sampling.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.1.1/topicgpt/generation/_keywords.py` & `wm_topicgpt-0.1.2/topicgpt/generation/_keywords.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.1.1/topicgpt/generation/_topic.py` & `wm_topicgpt-0.1.2/topicgpt/generation/_topic.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.1.1/topicgpt/persistence/_plot.py` & `wm_topicgpt-0.1.2/topicgpt/persistence/_plot.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.1.1/topicgpt/persistence/_save.py` & `wm_topicgpt-0.1.2/topicgpt/persistence/_save.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.1.1/topicgpt/pipeline.py` & `wm_topicgpt-0.1.2/topicgpt/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     },
     'keywords': {'ngram_range': (1, 2), 'topk': 10},
     'save_file': {'data_file': '../save/data.csv', 'topic_file': '../save/topic.csv', 'plot_file': '../save/tree.txt'},
     'bigquery': {'dataset_id': 'analytics', 'table_id': 'topic_modeling_data', 'time_id': 'topic_modeling_time'},
 }
 
 
-def topic_modeling(data_file, col_name):
+def topic_modeling(data_file, col_name, params=params):
     # load data
     dataset_name = os.path.basename(data_file).split(".")[0]
     file_extension = os.path.splitext(data_file)[1].lower()
     if file_extension == '.csv':
         data_df = pd.read_csv(data_file)
     elif file_extension == '.xlsx' or file_extension == '.xls':
         data_df = pd.read_excel(data_file)
```

### Comparing `wm_topicgpt-0.1.1/topicgpt/preprocessing/_data.py` & `wm_topicgpt-0.1.2/topicgpt/preprocessing/_data.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.1.1/topicgpt/walmart_llm/_chat_model.py` & `wm_topicgpt-0.1.2/topicgpt/walmart_llm/_chat_model.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.1.1/topicgpt/walmart_llm/_embed_model.py` & `wm_topicgpt-0.1.2/topicgpt/walmart_llm/_embed_model.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.1.1/topicgpt/walmart_llm/_llm_client.py` & `wm_topicgpt-0.1.2/topicgpt/walmart_llm/_llm_client.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.1.1/wm_topicgpt.egg-info/PKG-INFO` & `wm_topicgpt-0.1.2/wm_topicgpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wm-topicgpt
-Version: 0.1.1
+Version: 0.1.2
 Summary: This is a package to generate topics for the text corpus.
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: numpy==1.26.4
 Requires-Dist: pandas==2.2.1
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: azure-ai-textanalytics==5.3.0
```

### Comparing `wm_topicgpt-0.1.1/wm_topicgpt.egg-info/SOURCES.txt` & `wm_topicgpt-0.1.2/wm_topicgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

