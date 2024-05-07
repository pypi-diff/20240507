# Comparing `tmp/experiment_helpers-0.0.6.tar.gz` & `tmp/experiment_helpers-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experiment_helpers-0.0.6.tar", last modified: Mon May  6 23:42:07 2024, max compression
+gzip compressed data, was "experiment_helpers-0.0.8.tar", last modified: Tue May  7 01:06:12 2024, max compression
```

## Comparing `experiment_helpers-0.0.6.tar` & `experiment_helpers-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 23:42:07.548274 experiment_helpers-0.0.6/
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)     1071 2024-05-06 22:03:19.000000 experiment_helpers-0.0.6/LICENSE
--rw-r--r--   0 jlb638   (157170) jlb638   (157170)      375 2024-05-06 23:42:07.513496 experiment_helpers-0.0.6/PKG-INFO
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 22:01:10.000000 experiment_helpers-0.0.6/README.md
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)      361 2024-05-06 23:41:58.000000 experiment_helpers-0.0.6/pyproject.toml
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)       38 2024-05-06 23:42:07.548480 experiment_helpers-0.0.6/setup.cfg
-drwxrwxr-x   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 23:42:07.505190 experiment_helpers-0.0.6/src/
-drwxrwxr-x   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 23:42:07.509921 experiment_helpers-0.0.6/src/experiment_helpers/
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 22:05:13.000000 experiment_helpers-0.0.6/src/experiment_helpers/__init__.py
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)    18911 2024-05-06 22:05:55.000000 experiment_helpers-0.0.6/src/experiment_helpers/better_vit_model.py
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)     5922 2024-05-06 23:41:40.000000 experiment_helpers-0.0.6/src/experiment_helpers/measuring.py
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)     1084 2024-05-06 22:40:35.000000 experiment_helpers-0.0.6/src/experiment_helpers/static_globals.py
-drwxrwxr-x   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 23:42:07.512476 experiment_helpers-0.0.6/src/experiment_helpers.egg-info/
--rw-r--r--   0 jlb638   (157170) jlb638   (157170)      375 2024-05-06 23:42:07.510678 experiment_helpers-0.0.6/src/experiment_helpers.egg-info/PKG-INFO
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)      371 2024-05-06 23:42:07.511349 experiment_helpers-0.0.6/src/experiment_helpers.egg-info/SOURCES.txt
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)        1 2024-05-06 23:42:07.511957 experiment_helpers-0.0.6/src/experiment_helpers.egg-info/dependency_links.txt
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)       19 2024-05-06 23:42:07.512618 experiment_helpers-0.0.6/src/experiment_helpers.egg-info/top_level.txt
+drwxrwxr-x   0 jlb638   (157170) jlb638   (157170)        0 2024-05-07 01:06:12.232883 experiment_helpers-0.0.8/
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)     1071 2024-05-06 22:03:19.000000 experiment_helpers-0.0.8/LICENSE
+-rw-r--r--   0 jlb638   (157170) jlb638   (157170)      375 2024-05-07 01:06:12.232029 experiment_helpers-0.0.8/PKG-INFO
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 22:01:10.000000 experiment_helpers-0.0.8/README.md
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)      361 2024-05-07 01:06:04.000000 experiment_helpers-0.0.8/pyproject.toml
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)       38 2024-05-07 01:06:12.233017 experiment_helpers-0.0.8/setup.cfg
+drwxrwxr-x   0 jlb638   (157170) jlb638   (157170)        0 2024-05-07 01:06:12.223895 experiment_helpers-0.0.8/src/
+drwxrwxr-x   0 jlb638   (157170) jlb638   (157170)        0 2024-05-07 01:06:12.228985 experiment_helpers-0.0.8/src/experiment_helpers/
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 22:05:13.000000 experiment_helpers-0.0.8/src/experiment_helpers/__init__.py
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)    18911 2024-05-06 22:05:55.000000 experiment_helpers-0.0.8/src/experiment_helpers/better_vit_model.py
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)     5924 2024-05-07 01:04:42.000000 experiment_helpers-0.0.8/src/experiment_helpers/measuring.py
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)     1084 2024-05-06 22:40:35.000000 experiment_helpers-0.0.8/src/experiment_helpers/static_globals.py
+drwxrwxr-x   0 jlb638   (157170) jlb638   (157170)        0 2024-05-07 01:06:12.231369 experiment_helpers-0.0.8/src/experiment_helpers.egg-info/
+-rw-r--r--   0 jlb638   (157170) jlb638   (157170)      375 2024-05-07 01:06:12.229744 experiment_helpers-0.0.8/src/experiment_helpers.egg-info/PKG-INFO
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)      371 2024-05-07 01:06:12.230370 experiment_helpers-0.0.8/src/experiment_helpers.egg-info/SOURCES.txt
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)        1 2024-05-07 01:06:12.230940 experiment_helpers-0.0.8/src/experiment_helpers.egg-info/dependency_links.txt
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)       19 2024-05-07 01:06:12.231477 experiment_helpers-0.0.8/src/experiment_helpers.egg-info/top_level.txt
```

### Comparing `experiment_helpers-0.0.6/LICENSE` & `experiment_helpers-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `experiment_helpers-0.0.6/src/experiment_helpers/better_vit_model.py` & `experiment_helpers-0.0.8/src/experiment_helpers/better_vit_model.py`

 * *Files identical despite different names*

### Comparing `experiment_helpers-0.0.6/src/experiment_helpers/measuring.py` & `experiment_helpers-0.0.8/src/experiment_helpers/measuring.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     embedding_model = SentenceTransformer('Alibaba-NLP/gte-large-en-v1.5', trust_remote_code=True)
     src_blip_embedding_list=embedding_model.encode(src_blip_caption_list)
     image_blip_embedding_list=embedding_model.encode(image_blip_caption_list)
     evaluation_blip_embedding_list=embedding_model.encode(evaluation_prompt_list)
 
     metric_dict[BLIP_TARGET_CAPTION_SIMILARITY]=np.mean(cos_sim_st(src_blip_embedding_list, image_blip_embedding_list).cpu().detach().numpy())
     metric_dict[BLIP_PROMPT_CAPTION_SIMILARITY]=np.mean(
-        cos_sim_st(evaluation_blip_embedding, image_blip_caption).cpu().detach().numpy() for evaluation_blip_embedding, image_blip_caption in zip(evaluation_blip_embedding_list, image_blip_caption_list)
+        [cos_sim_st(evaluation_blip_embedding, image_blip_caption).cpu().detach().numpy() for evaluation_blip_embedding, image_blip_caption in zip(evaluation_blip_embedding_list, image_blip_caption_list)]
     )
 
     '''blip_model=Blip2Model.from_pretrained("Salesforce/blip2-opt-2.7b")
     blip_inputs=blip_processor(text=evaluation_prompt_list, images=evaluation_image_list+image_list)
     blip_outputs=blip_model(**blip_inputs)'''
```

### Comparing `experiment_helpers-0.0.6/src/experiment_helpers/static_globals.py` & `experiment_helpers-0.0.8/src/experiment_helpers/static_globals.py`

 * *Files identical despite different names*
