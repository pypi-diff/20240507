# Comparing `tmp/experiment_helpers-0.0.3.tar.gz` & `tmp/experiment_helpers-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experiment_helpers-0.0.3.tar", last modified: Mon May  6 22:49:48 2024, max compression
+gzip compressed data, was "experiment_helpers-0.0.5.tar", last modified: Mon May  6 23:14:52 2024, max compression
```

## Comparing `experiment_helpers-0.0.3.tar` & `experiment_helpers-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 22:49:48.041377 experiment_helpers-0.0.3/
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)     1071 2024-05-06 22:03:19.000000 experiment_helpers-0.0.3/LICENSE
--rw-r--r--   0 jlb638   (157170) jlb638   (157170)      375 2024-05-06 22:49:48.040413 experiment_helpers-0.0.3/PKG-INFO
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 22:01:10.000000 experiment_helpers-0.0.3/README.md
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)      361 2024-05-06 22:49:37.000000 experiment_helpers-0.0.3/pyproject.toml
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)       38 2024-05-06 22:49:48.041573 experiment_helpers-0.0.3/setup.cfg
-drwxrwxr-x   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 22:49:48.028836 experiment_helpers-0.0.3/src/
-drwxrwxr-x   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 22:49:48.035521 experiment_helpers-0.0.3/src/experiment_helpers/
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 22:05:13.000000 experiment_helpers-0.0.3/src/experiment_helpers/__init__.py
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)    18911 2024-05-06 22:05:55.000000 experiment_helpers-0.0.3/src/experiment_helpers/better_vit_model.py
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)     5290 2024-05-06 22:49:01.000000 experiment_helpers-0.0.3/src/experiment_helpers/measuring.py
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)     1084 2024-05-06 22:40:35.000000 experiment_helpers-0.0.3/src/experiment_helpers/static_globals.py
-drwxrwxr-x   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 22:49:48.039197 experiment_helpers-0.0.3/src/experiment_helpers.egg-info/
--rw-r--r--   0 jlb638   (157170) jlb638   (157170)      375 2024-05-06 22:49:48.036627 experiment_helpers-0.0.3/src/experiment_helpers.egg-info/PKG-INFO
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)      371 2024-05-06 22:49:48.037636 experiment_helpers-0.0.3/src/experiment_helpers.egg-info/SOURCES.txt
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)        1 2024-05-06 22:49:48.038479 experiment_helpers-0.0.3/src/experiment_helpers.egg-info/dependency_links.txt
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)       19 2024-05-06 22:49:48.039384 experiment_helpers-0.0.3/src/experiment_helpers.egg-info/top_level.txt
+drwxrwxr-x   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 23:14:52.175660 experiment_helpers-0.0.5/
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)     1071 2024-05-06 22:03:19.000000 experiment_helpers-0.0.5/LICENSE
+-rw-r--r--   0 jlb638   (157170) jlb638   (157170)      375 2024-05-06 23:14:52.174323 experiment_helpers-0.0.5/PKG-INFO
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 22:01:10.000000 experiment_helpers-0.0.5/README.md
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)      361 2024-05-06 23:14:43.000000 experiment_helpers-0.0.5/pyproject.toml
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)       38 2024-05-06 23:14:52.175823 experiment_helpers-0.0.5/setup.cfg
+drwxrwxr-x   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 23:14:52.164977 experiment_helpers-0.0.5/src/
+drwxrwxr-x   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 23:14:52.170218 experiment_helpers-0.0.5/src/experiment_helpers/
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 22:05:13.000000 experiment_helpers-0.0.5/src/experiment_helpers/__init__.py
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)    18911 2024-05-06 22:05:55.000000 experiment_helpers-0.0.5/src/experiment_helpers/better_vit_model.py
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)     5901 2024-05-06 23:12:29.000000 experiment_helpers-0.0.5/src/experiment_helpers/measuring.py
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)     1084 2024-05-06 22:40:35.000000 experiment_helpers-0.0.5/src/experiment_helpers/static_globals.py
+drwxrwxr-x   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 23:14:52.173159 experiment_helpers-0.0.5/src/experiment_helpers.egg-info/
+-rw-r--r--   0 jlb638   (157170) jlb638   (157170)      375 2024-05-06 23:14:52.171184 experiment_helpers-0.0.5/src/experiment_helpers.egg-info/PKG-INFO
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)      371 2024-05-06 23:14:52.172022 experiment_helpers-0.0.5/src/experiment_helpers.egg-info/SOURCES.txt
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)        1 2024-05-06 23:14:52.172666 experiment_helpers-0.0.5/src/experiment_helpers.egg-info/dependency_links.txt
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)       19 2024-05-06 23:14:52.173287 experiment_helpers-0.0.5/src/experiment_helpers.egg-info/top_level.txt
```

### Comparing `experiment_helpers-0.0.3/LICENSE` & `experiment_helpers-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `experiment_helpers-0.0.3/src/experiment_helpers/better_vit_model.py` & `experiment_helpers-0.0.5/src/experiment_helpers/better_vit_model.py`

 * *Files identical despite different names*

### Comparing `experiment_helpers-0.0.3/src/experiment_helpers/measuring.py` & `experiment_helpers-0.0.5/src/experiment_helpers/measuring.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,14 +27,21 @@
 from PIL import Image
 from sentence_transformers import SentenceTransformer
 from sentence_transformers.util import cos_sim as cos_sim_st
 
 def cos_sim(vector_i,vector_j)->float:
     return np.dot(vector_i,vector_j)/(norm(vector_i)*norm(vector_j))
 
+def get_caption(image:Image,blip_processor: Blip2Processor,blip_conditional_gen: Blip2ForConditionalGeneration):
+    caption_inputs = blip_processor(image, "", return_tensors="pt")
+    for name in ["pixel_values","input_ids"]:
+        caption_inputs[name]=caption_inputs[name].to(blip_conditional_gen.device)
+    caption_out=blip_conditional_gen.generate(**caption_inputs)
+    return blip_processor.decode(caption_out[0],skip_special_tokens=True).strip()
+
 def get_metric_dict(evaluation_prompt_list:list, evaluation_image_list:list,image_list:list,accelerator:Accelerator=None):
     metric_dict={}
     
     clip_model = CLIPModel.from_pretrained("openai/clip-vit-base-patch32")
     clip_processor = CLIPProcessor.from_pretrained("openai/clip-vit-base-patch32")
     if accelerator is not None:
         clip_model.to(accelerator.device)
@@ -68,14 +75,17 @@
 
     metric_dict[IDENTITY_CONSISTENCY]=np.mean(identity_consistency_list)
     metric_dict[TARGET_SIMILARITY]=np.mean(target_similarity_list)
     metric_dict[PROMPT_SIMILARITY]=np.mean(prompt_similarity_list)
 
     blip_processor = Blip2Processor.from_pretrained("Salesforce/blip2-opt-2.7b")
     blip_conditional_gen = Blip2ForConditionalGeneration.from_pretrained("Salesforce/blip2-opt-2.7b")
+    if accelerator is not None:
+        blip_conditional_gen.to(accelerator.device)
+        blip_conditional_gen=accelerator.prepare(blip_conditional_gen)
     
 
     src_blip_caption_list=[get_caption(src_image,blip_processor,blip_conditional_gen) for src_image in image_list]
     image_blip_caption_list=[get_caption(image,blip_processor,blip_conditional_gen) for image in evaluation_image_list]
     embedding_model = SentenceTransformer('Alibaba-NLP/gte-large-en-v1.5', trust_remote_code=True)
     src_blip_embedding_list=embedding_model(src_blip_caption_list)
     image_blip_embedding_list=embedding_model(image_blip_caption_list)
```

### Comparing `experiment_helpers-0.0.3/src/experiment_helpers/static_globals.py` & `experiment_helpers-0.0.5/src/experiment_helpers/static_globals.py`

 * *Files identical despite different names*

