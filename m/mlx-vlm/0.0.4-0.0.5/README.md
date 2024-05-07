# Comparing `tmp/mlx_vlm-0.0.4.tar.gz` & `tmp/mlx_vlm-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlx_vlm-0.0.4.tar", last modified: Fri May  3 20:54:34 2024, max compression
+gzip compressed data, was "mlx_vlm-0.0.5.tar", last modified: Tue May  7 08:42:06 2024, max compression
```

## Comparing `mlx_vlm-0.0.4.tar` & `mlx_vlm-0.0.5.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:54:34.427915 mlx_vlm-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-03 20:54:34.427915 mlx_vlm-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:54:34.423915 mlx_vlm-0.0.4/mlx_vlm/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:54:34.423915 mlx_vlm-0.0.4/mlx_vlm/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:54:34.423915 mlx_vlm-0.0.4/mlx_vlm/models/idefics2/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/idefics2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10797 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/idefics2/idefics2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/idefics2/language.py
--rw-r--r--   0 runner    (1001) docker     (127)     9220 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/idefics2/vision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:54:34.423915 mlx_vlm-0.0.4/mlx_vlm/models/llava/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/llava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/llava/language.py
--rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/llava/llava.py
--rw-r--r--   0 runner    (1001) docker     (127)     7839 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/llava/vision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:54:34.423915 mlx_vlm-0.0.4/mlx_vlm/models/nanoLlava/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/nanoLlava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/nanoLlava/language.py
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/nanoLlava/nanoLlava.py
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/nanoLlava/vision.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/prompt_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/sample_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:54:34.427915 mlx_vlm-0.0.4/mlx_vlm/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    10110 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/tokenizer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25427 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:54:34.427915 mlx_vlm-0.0.4/mlx_vlm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-03 20:54:34.000000 mlx_vlm-0.0.4/mlx_vlm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-03 20:54:34.000000 mlx_vlm-0.0.4/mlx_vlm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:54:34.000000 mlx_vlm-0.0.4/mlx_vlm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-03 20:54:34.000000 mlx_vlm-0.0.4/mlx_vlm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 20:54:34.000000 mlx_vlm-0.0.4/mlx_vlm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 20:54:34.427915 mlx_vlm-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:42:06.839632 mlx_vlm-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-07 08:42:06.839632 mlx_vlm-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:42:06.835632 mlx_vlm-0.0.5/mlx_vlm/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/chat_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:42:06.835632 mlx_vlm-0.0.5/mlx_vlm/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:42:06.835632 mlx_vlm-0.0.5/mlx_vlm/models/idefics2/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/idefics2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10797 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/idefics2/idefics2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/idefics2/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9220 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/idefics2/vision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:42:06.839632 mlx_vlm-0.0.5/mlx_vlm/models/llava/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/llava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/llava/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/llava/llava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7839 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/llava/vision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:42:06.839632 mlx_vlm-0.0.5/mlx_vlm/models/nanoLlava/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/nanoLlava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/nanoLlava/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/nanoLlava/nanoLlava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/nanoLlava/vision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/prompt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/sample_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:42:06.839632 mlx_vlm-0.0.5/mlx_vlm/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10110 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/tokenizer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26042 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:42:06.839632 mlx_vlm-0.0.5/mlx_vlm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-07 08:42:06.000000 mlx_vlm-0.0.5/mlx_vlm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-07 08:42:06.000000 mlx_vlm-0.0.5/mlx_vlm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 08:42:06.000000 mlx_vlm-0.0.5/mlx_vlm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-07 08:42:06.000000 mlx_vlm-0.0.5/mlx_vlm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 08:42:06.000000 mlx_vlm-0.0.5/mlx_vlm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 08:42:06.839632 mlx_vlm-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/setup.py
```

### Comparing `mlx_vlm-0.0.4/LICENSE` & `mlx_vlm-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.4/mlx_vlm/convert.py` & `mlx_vlm-0.0.5/mlx_vlm/convert.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.4/mlx_vlm/generate.py` & `mlx_vlm-0.0.5/mlx_vlm/generate.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.4/mlx_vlm/models/base.py` & `mlx_vlm-0.0.5/mlx_vlm/models/base.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.4/mlx_vlm/models/idefics2/idefics2.py` & `mlx_vlm-0.0.5/mlx_vlm/models/idefics2/idefics2.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.4/mlx_vlm/models/idefics2/language.py` & `mlx_vlm-0.0.5/mlx_vlm/models/idefics2/language.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.4/mlx_vlm/models/idefics2/vision.py` & `mlx_vlm-0.0.5/mlx_vlm/models/idefics2/vision.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.4/mlx_vlm/models/llava/language.py` & `mlx_vlm-0.0.5/mlx_vlm/models/llava/language.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.4/mlx_vlm/models/llava/llava.py` & `mlx_vlm-0.0.5/mlx_vlm/models/llava/llava.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.4/mlx_vlm/models/llava/vision.py` & `mlx_vlm-0.0.5/mlx_vlm/models/llava/vision.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.4/mlx_vlm/models/nanoLlava/language.py` & `mlx_vlm-0.0.5/mlx_vlm/models/nanoLlava/language.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.4/mlx_vlm/models/nanoLlava/nanoLlava.py` & `mlx_vlm-0.0.5/mlx_vlm/models/nanoLlava/nanoLlava.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.4/mlx_vlm/models/nanoLlava/vision.py` & `mlx_vlm-0.0.5/mlx_vlm/models/nanoLlava/vision.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.4/mlx_vlm/prompt_utils.py` & `mlx_vlm-0.0.5/mlx_vlm/prompt_utils.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.4/mlx_vlm/sample_utils.py` & `mlx_vlm-0.0.5/mlx_vlm/sample_utils.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.4/mlx_vlm/tests/test_models.py` & `mlx_vlm-0.0.5/mlx_vlm/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.4/mlx_vlm/tokenizer_utils.py` & `mlx_vlm-0.0.5/mlx_vlm/tokenizer_utils.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.4/mlx_vlm/utils.py` & `mlx_vlm-0.0.5/mlx_vlm/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,33 @@
 
     config = load_config(model_path)
     quantization = config.get("quantization", None)
 
     weight_files = glob.glob(str(model_path / "*.safetensors"))
     if not weight_files:
         logging.error(f"No safetensors found in {model_path}")
-        raise FileNotFoundError(f"No safetensors found in {model_path}")
+        message = f"""
+No safetensors found in {model_path}
+Create safetensors using the following code:
+```
+from transformers import AutoModelForCausalLM, AutoProcessor
+
+model_id= "<huggingface_model_id>"
+model = AutoModelForCausalLM.from_pretrained(model_id)
+processor = AutoProcessor.from_pretrained(model_id)
+
+model.save_pretrained("<local_dir>")
+processor.save_pretrained("<local_dir>")
+```
+Then use the <local_dir> as the --hf-path in the convert script.
+```
+python -m mlx_vlm.convert --hf-path <local_dir> --mlx-path <mlx_dir>
+```
+        """
+        raise FileNotFoundError(message)
 
     weights = {}
     for wf in weight_files:
         weights.update(mx.load(wf))
 
     model_class, model_type = get_model_and_args(config=config)
 
@@ -211,15 +229,19 @@
 
     model = load_model(model_path, lazy)
     processor = load_processor(model_path, processor_config=processor_config)
 
     return model, processor
 
 
-def load_config(model_path: Path) -> dict:
+def load_config(model_path: Union[str, Path]) -> dict:
+
+    if isinstance(model_path, str):
+        model_path = get_model_path(model_path)
+
     try:
         with open(model_path / "config.json", "r") as f:
             config = json.load(f)
     except FileNotFoundError:
         logging.error(f"Config file not found in {model_path}")
         raise
     return config
@@ -301,15 +323,15 @@
     from . import __version__
 
     card = ModelCard.load(hf_path)
     card.data.tags = ["mlx"] if card.data.tags is None else card.data.tags + ["mlx"]
     card.text = dedent(
         f"""
         # {upload_repo}
-        This model was converted to MLX format from [`{hf_path}`]() using mlx-vllm version **{__version__}**.
+        This model was converted to MLX format from [`{hf_path}`]() using mlx-vlm version **{__version__}**.
         Refer to the [original model card](https://huggingface.co/{hf_path}) for more details on the model.
         ## Use with mlx
 
         ```bash
         pip install -U mlx-vlm
         ```
```

### Comparing `mlx_vlm-0.0.4/mlx_vlm.egg-info/SOURCES.txt` & `mlx_vlm-0.0.5/mlx_vlm.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 ./requirements.txt
 mlx_vlm/__init__.py
+mlx_vlm/chat_ui.py
 mlx_vlm/convert.py
 mlx_vlm/generate.py
 mlx_vlm/prompt_utils.py
 mlx_vlm/sample_utils.py
 mlx_vlm/tokenizer_utils.py
 mlx_vlm/utils.py
 mlx_vlm/version.py
```

### Comparing `mlx_vlm-0.0.4/setup.py` & `mlx_vlm-0.0.5/setup.py`

 * *Files identical despite different names*

