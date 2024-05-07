# Comparing `tmp/helmet-1.1.0.tar.gz` & `tmp/helmet-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helmet-1.1.0.tar", max compression
+gzip compressed data, was "helmet-1.1.1.tar", max compression
```

## Comparing `helmet-1.1.0.tar` & `helmet-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3116 2024-05-04 08:42:42.774084 helmet-1.1.0/README.md
--rw-r--r--   0        0        0      445 2024-05-04 08:42:42.774084 helmet-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2980 2024-05-04 08:42:42.774084 helmet-1.1.0/src/helmet/__init__.py
--rw-r--r--   0        0        0        0 2024-05-04 08:42:42.774084 helmet-1.1.0/src/helmet/explainers/__init__.py
--rw-r--r--   0        0        0     4948 2024-05-04 08:42:42.774084 helmet-1.1.0/src/helmet/explainers/gradients.py
--rw-r--r--   0        0        0      630 2024-05-04 08:42:42.774084 helmet-1.1.0/src/helmet/explainers/perturbation.py
--rw-r--r--   0        0        0       49 2024-05-04 08:42:42.774084 helmet-1.1.0/src/helmet/model/__init__.py
--rw-r--r--   0        0        0     3769 2024-05-04 08:42:42.774084 helmet-1.1.0/src/helmet/model/base_lm.py
--rw-r--r--   0        0        0     5373 2024-05-04 08:42:42.774084 helmet-1.1.0/src/helmet/model/dec_lm.py
--rw-r--r--   0        0        0     3879 2024-05-04 08:42:42.774084 helmet-1.1.0/src/helmet/updater.py
--rw-r--r--   0        0        0      125 2024-05-04 08:42:42.774084 helmet-1.1.0/src/helmet/utils/constants.py
--rw-r--r--   0        0        0     3623 2024-05-04 08:42:42.774084 helmet-1.1.0/src/helmet/utils/types.py
--rw-r--r--   0        0        0      130 2024-05-04 08:42:42.774084 helmet-1.1.0/src/helmet/utils/utils.py
--rw-r--r--   0        0        0     3759 1970-01-01 00:00:00.000000 helmet-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3492 2024-05-07 07:25:02.358780 helmet-1.1.1/README.md
+-rw-r--r--   0        0        0      445 2024-05-07 07:25:02.362780 helmet-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2976 2024-05-07 07:25:02.362780 helmet-1.1.1/src/helmet/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 07:25:02.362780 helmet-1.1.1/src/helmet/explainers/__init__.py
+-rw-r--r--   0        0        0     5194 2024-05-07 07:25:02.362780 helmet-1.1.1/src/helmet/explainers/gradients.py
+-rw-r--r--   0        0        0      630 2024-05-07 07:25:02.362780 helmet-1.1.1/src/helmet/explainers/perturbation.py
+-rw-r--r--   0        0        0       49 2024-05-07 07:25:02.362780 helmet-1.1.1/src/helmet/model/__init__.py
+-rw-r--r--   0        0        0     2880 2024-05-07 07:25:02.362780 helmet-1.1.1/src/helmet/model/base_lm.py
+-rw-r--r--   0        0        0     5537 2024-05-07 07:25:02.362780 helmet-1.1.1/src/helmet/model/dec_lm.py
+-rw-r--r--   0        0        0     3879 2024-05-07 07:25:02.362780 helmet-1.1.1/src/helmet/updater.py
+-rw-r--r--   0        0        0      125 2024-05-07 07:25:02.362780 helmet-1.1.1/src/helmet/utils/constants.py
+-rw-r--r--   0        0        0     3751 2024-05-07 07:25:02.362780 helmet-1.1.1/src/helmet/utils/types.py
+-rw-r--r--   0        0        0      130 2024-05-07 07:25:02.362780 helmet-1.1.1/src/helmet/utils/utils.py
+-rw-r--r--   0        0        0     4135 1970-01-01 00:00:00.000000 helmet-1.1.1/PKG-INFO
```

### Comparing `helmet-1.1.0/README.md` & `helmet-1.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -29,31 +29,41 @@
 2. A webapp: `helmet-platform`, which deploys an API to save al the runs & projects and interacts with the frontend. A frontend should also be deployed.
 
 ### Configuration files
 
 #### Platform configuration
 
 ```python
-project_setup = {
-    # This should point to the NodeJS API
-    platform_url: "localhost:4000"
-    project_id: "<ID>"
-}
+project_name = "Project Name"
+project_id = "Id" # (get from frontend or code)
+platform_url = "https://" # Please do not change this
+
 ```
 
 #### Model configuration
 
 ```python
-model_checkpoint = "meta-llama/Meta-Llama-3-8B"
-model_setup = {
-    "checkpoint": model_checkpoint,
-    # This can be enc/enc-dec/dec
-    "model_type": "dec",
-    # This should specify where the embeddings are stored
-    "embeddings": "model.embed_tokens",
+# This should be the name as is presented on Huggingface 🤗
+checkpoint = "meta-llama/Meta-Llama-3-8B-Instruct"
+# The embeddings are needed for the XAI part. This varies between models, thus please provide it yourself.
+embeddings = "model.embed_tokens"
+
+# This is for wrapper to know what kind of model it is.
+model_type = "dec"
+```
+
+#### Model Args
+
+```python
+# This is needed to use Llama-3
+access_token = "hf_"
+
+# You can add more here if you like
+model_args = {
+    "token": access_token
 }
 ```
 
 #### Run configuration
 
 ```python
 run_config = {
@@ -63,35 +73,41 @@
 ```
 
 ### Load/create project
 
 Creating a project can be done by current the following python code in your jupyter notebook.
 
 ```python
-project_id = helmet.get_or_create_project("<platform url>", "<project name>", "text_generation")
+project_id = get_or_create_project(platform_url, project_name, "text_generation")
 ```
 
 This will give you back the ID of the project, that you can then use to load the model.
 
 After you have configured the model, platform & device, you can start loading the model like this:
 
 ```python
-model = helmet.from_pretrained(project_setup, model_setup, run_config)
+model = from_pretrained(checkpoint, model_type, embeddings, project_id, device, platform_url, model_args)
 ```
 
 ### Features
 
 - Load any causal model from Huggingface.
 - Create a project for your experiment
 - Run experimental prompts
 
 ### Demo
 
 A demo can be found at [https://helmet.jeroennelen.nl](https://helmet.jeroennelen.nl)
 
+### Component architecture
+
+<p align="center">
+<img  width="75%" src="docs/helmet simplified.png" />
+</p>
+
 ## Install from source
 
 To use helmet in one of the examples perform the following steps:
 
 1. Create venv with `python -m venv .venv`
 2. Activate the venv with `source .venv/bin/activate`
 3. Install HELMET from source (from git, when located in the home folder of helmet `pip install -e .`
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `helmet-1.1.0/src/helmet/__init__.py` & `helmet-1.1.1/src/helmet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,37 +17,37 @@
 model_type_to_model_wrapper = {
     # "enc": ENC_LM,
     # "enc-dec": ENC_DEC_LM,
     "dec": DEC_LM,
 }
 
 
-def from_pretrained(model_checkpoint: str, model_type: str, embeddings_path:str, project_id:str,                     device:str, platform_url:str = url, model_config: dict={}):
+def from_pretrained(model_checkpoint: str, model_type: str, embeddings_path:str, project_id:str, 
+                    device:str, platform_url:str = url, model_config: dict={}):
     """
     Load a model from a checkpoint and return the model object
     Args:
         model_checkpoint (str): The model checkpoint to load
         model_type (str): The type of model to load (enc, dec, enc-dec)
         embeddings_path (str): The embeddings pointer
         project_id (str): The project id to send updates to
         device (str): The device to load the model on (cpu or cuda)
         platform_url (str): The url to send updates to (default is http://localhost:4000)
         model_config (dict): The model configuration
     """
     # First checks
-    assert device in ["cpu", "cuda"], AssertionError("device must be either 'cpu' or 'cuda'")
     assert model_type in ["enc", "dec", "enc-dec"], AssertionError("model_type must be either 'enc', 'dec', or 'enc-dec'")
     if model_type in ["enc", "enc-dec"]:
         raise NotImplementedError("model_type 'enc' and 'enc-dec' not implemented yet")
     
+    assert device in ["cpu", "cuda"], AssertionError("device must be either 'cpu' or 'cuda'")
     if device == "cuda":
         assert torch.cuda.is_available(), AssertionError("cuda is not available")
         torch.device(device)
 
-    
     print("updates will be sent to", platform_url)
     print("setting up model with config, ", model_config)
 
     # Getting the Hugginface class
     model_cls = model_type_to_class[model_type]
 
     # Quantization of the model
```

### Comparing `helmet-1.1.0/src/helmet/explainers/gradients.py` & `helmet-1.1.1/src/helmet/explainers/gradients.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,45 +9,55 @@
     handle = embedding_layer.register_forward_hook(forward_hook)
     return handle
 
 def register_embedding_gradient_hooks(model, embedding_layer, embeddings_gradients):
     def hook_layers(module, grad_in, grad_out):
         embeddings_gradients.append(grad_out[0].detach().cpu().numpy())
     hook = embedding_layer.register_full_backward_hook(hook_layers)
+    # hook = embedding_layer.register_full_backward_hook(hook_layers)
     return hook
 
-def analyze_token(wrapper, input_ids, input_mask, batch=0, correct=None, foil=None):
+def analyze_token(wrapper, input_ids, correct=None, foil=None):
     # Get model gradients and input embeddings
     model = wrapper.model
     embedding_layer = wrapper.embeddings
 
-    model.eval()
     embeddings_list = []
     handle = register_embedding_list_hook(model, embedding_layer, embeddings_list)
     embeddings_gradients = []
     hook = register_embedding_gradient_hooks(model, embedding_layer, embeddings_gradients)
     if correct is None:
+        # All is on CPU at this moment
         correct = input_ids[-1]
         input_ids = input_ids[:-1]
-        input_mask = input_mask[:-1]
-
-    input_ids_new = torch.tensor(input_ids.clone().detach())
-    input_ids_unsqueezed = input_ids_new.unsqueeze(0)
 
+    input_ids = torch.tensor(input_ids).unsqueeze(0).to(wrapper.device)
+    
     with torch.enable_grad():
-        A = model(input_ids=input_ids_unsqueezed, output_attentions=False)
+        if torch.cuda.is_available():
+            torch.cuda.empty_cache()
+        model.eval()
+        for param in model.parameters():
+            param.grad = None
+        
+        A = model(input_ids=input_ids, output_attentions=False)
 
+        # For contrastive explanations
         if foil is not None and correct != foil:
-            (A.logits[0][-1][correct]-A.logits[0][-1][foil]).backward()
+            p = A.logits[0][-1][correct] - A.logits[0][-1][foil]
         else:
-            # Take the last logits and backpropagate the gradient
+            # for feature attributions
             p = A.logits[0][-1][correct]
-            p.backward()
+
+        p.backward()
+        
         handle.remove()
         hook.remove()
+        if torch.cuda.is_available():
+            torch.cuda.empty_cache()
 
     return np.array(embeddings_gradients).squeeze(), np.array(embeddings_list).squeeze()
 
 def input_x_gradient(grads, embds, normalize=False):
     input_grad = np.sum(grads * embds, axis=-1).squeeze()
 
     if normalize:
```

### Comparing `helmet-1.1.0/src/helmet/explainers/perturbation.py` & `helmet-1.1.1/src/helmet/explainers/perturbation.py`

 * *Files identical despite different names*

### Comparing `helmet-1.1.0/src/helmet/model/base_lm.py` & `helmet-1.1.1/src/helmet/model/base_lm.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,107 +3,74 @@
 
 import numpy as np
 import torch
 
 from helmet.updater import get_run, update_app
 from helmet.utils.types import Explanation, Input, Output, Run
 
-
 class Base_LM(ABC):    
     def __init__(self, model_checkpoint: str, model, tokenizer, 
                  model_type: str, url: str, project_id:str, embeddings, device="cpu"):
         self.model = model
         self.model_checkpoint = model_checkpoint
         self.tokenizer = tokenizer
         self.platform_url = url
         self.project_id = project_id
         self.model_type = model_type
         self.embeddings = embeddings
         self.device = device
-        self.__post_init__()
-    
-    def __post_init__(self):
-        self.reset_model()
+        self.model.eval()
+        self.model.zero_grad()
         print("model loaded")
-    
+
     def _encode_text(self, text, **kwargs):
         if isinstance(text, list):
             text = self.tokenizer.apply_chat_template(text, tokenize = False, add_generation_prompt = True)
-
-        enc = self.tokenizer.encode_plus(text, return_tensors="pt", **kwargs)
-        return {k: v.to(self.device) for k, v in enc.items()}
+        # encode = convert_tokens_to_ids(tokenize(text))
+        # encode plus will also give the attention mask
+        return self.tokenizer.encode_plus(text, return_tensors="pt", **kwargs)
 
     def _tokenize(self, text: str, **kwargs):
-        t = self.tokenizer(text, return_tensors="pt", **kwargs)
-        return t.to(self.device)
+        return self.tokenizer(text, return_tensors="pt", **kwargs)
 
     def token_ids_to_string(self, output) -> str:
         # Return back the string
         return self.tokenizer.decode(output, skip_special_tokens=True)
 
     def get_tokens(self, text: str):
         return self.tokenizer.get_tokens(text)
     
-    def to_device(self, tensor):
-        return tensor.to(self.device)
-
-    def get_input_embeddings(self, text: str):
-        """Extract input embeddings
-
-        :param text str: the string to extract embeddings from.
-        """
-        item = self._tokenize(text)
-        item = {k: v.to(self.device) for k, v in item.items()}
-        embeddings = self._get_input_embeds_from_ids(item["input_ids"][0])
-        embeddings = embeddings.unsqueeze(0)
-        return embeddings
-    
     def _get_input_embeds_from_ids(self, ids) -> torch.Tensor:
         return self.model.get_input_embeddings()(ids)
 
     def get_run(self, run_id: str) -> Run:
         resp = get_run(self.platform_url, run_id)
-        if resp is None:
+        if resp is None or not isinstance(resp, Run):
             raise ValueError(f"Run with id {run_id} not found") 
         return resp
 
     def _format_run(self, prompt, output_str, explanations: list[Explanation], execution_time_in_sec=None, **kwargs) -> Run:
         return Run(**{
             "date": datetime.now(),
             "model_checkpoint": self.model_checkpoint,
             "tokenizer": self.tokenizer.name_or_path,
             "model_type": self.model_type,
             "input": Input(prompt, self.tokenizer.tokenize(prompt)),
             "output": Output(output_str, self.tokenizer.tokenize(output_str)),
             "explanations": explanations,
             "project_id": self.project_id,
             "execution_time_in_sec": execution_time_in_sec,
-            **kwargs # e.g. _id or groundtruth
+            **kwargs # e.g. _id, groundtruth, custom args
         })
 
     def normalize(self, attr):
         l2_norm = np.linalg.norm(attr)
         l2_normalized_matrix = attr / l2_norm
         return l2_normalized_matrix
 
     def update_run(self, run: Run):
-        id = update_app(self.platform_url, "/runs", run.dict())
-        return id
-
-    def update_explainer_model(self):
-        b = {
-            "model_checkpoint": self.model_checkpoint,
-            "model": self.model.config.model_type,
-            "tokenizer": self.tokenizer.name_or_path,
-            "model_type": self.model_type
-        }
-        id = update_app(self.platform_url, "/update_model", b)
-
-    def reset_model(self):
-        self.model.eval()
-        self.model.zero_grad()
-
+        return update_app(self.platform_url, "/runs", run.dict())
 
     @abstractmethod
     def predict(self, *args, **kwargs):
         pass
```

### Comparing `helmet-1.1.0/src/helmet/updater.py` & `helmet-1.1.1/src/helmet/updater.py`

 * *Files identical despite different names*

### Comparing `helmet-1.1.0/src/helmet/utils/types.py` & `helmet-1.1.1/src/helmet/utils/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -97,14 +97,15 @@
     model_type: str
     input: Input
     output: Output
     explanations: list[Explanation]
 
     _id: Optional[str] = None
     groundtruth: Optional[str] = None
+    custom_args: Optional[dict] = None
     execution_time_in_sec: Optional[float] = None
     
     def dict(self) -> dict:
         d = {
             "date": self.date,
             "model_checkpoint": self.model_checkpoint,
             "tokenizer": self.tokenizer,
@@ -115,9 +116,11 @@
             "project_id": self.project_id,
             "execution_time_in_sec": self.execution_time_in_sec
         }
         if self._id is not None:
             d["_id"] = self._id
         if self.groundtruth is not None:
             d["groundtruth"] = self.groundtruth
+        if self.custom_args is not None:
+            d["custom_args"] = self.custom_args
         return d
```

### Comparing `helmet-1.1.0/PKG-INFO` & `helmet-1.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helmet
-Version: 1.1.0
+Version: 1.1.1
 Summary: 
 Author: Jeroen
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -48,31 +48,41 @@
 2. A webapp: `helmet-platform`, which deploys an API to save al the runs & projects and interacts with the frontend. A frontend should also be deployed.
 
 ### Configuration files
 
 #### Platform configuration
 
 ```python
-project_setup = {
-    # This should point to the NodeJS API
-    platform_url: "localhost:4000"
-    project_id: "<ID>"
-}
+project_name = "Project Name"
+project_id = "Id" # (get from frontend or code)
+platform_url = "https://" # Please do not change this
+
 ```
 
 #### Model configuration
 
 ```python
-model_checkpoint = "meta-llama/Meta-Llama-3-8B"
-model_setup = {
-    "checkpoint": model_checkpoint,
-    # This can be enc/enc-dec/dec
-    "model_type": "dec",
-    # This should specify where the embeddings are stored
-    "embeddings": "model.embed_tokens",
+# This should be the name as is presented on Huggingface 🤗
+checkpoint = "meta-llama/Meta-Llama-3-8B-Instruct"
+# The embeddings are needed for the XAI part. This varies between models, thus please provide it yourself.
+embeddings = "model.embed_tokens"
+
+# This is for wrapper to know what kind of model it is.
+model_type = "dec"
+```
+
+#### Model Args
+
+```python
+# This is needed to use Llama-3
+access_token = "hf_"
+
+# You can add more here if you like
+model_args = {
+    "token": access_token
 }
 ```
 
 #### Run configuration
 
 ```python
 run_config = {
@@ -82,35 +92,41 @@
 ```
 
 ### Load/create project
 
 Creating a project can be done by current the following python code in your jupyter notebook.
 
 ```python
-project_id = helmet.get_or_create_project("<platform url>", "<project name>", "text_generation")
+project_id = get_or_create_project(platform_url, project_name, "text_generation")
 ```
 
 This will give you back the ID of the project, that you can then use to load the model.
 
 After you have configured the model, platform & device, you can start loading the model like this:
 
 ```python
-model = helmet.from_pretrained(project_setup, model_setup, run_config)
+model = from_pretrained(checkpoint, model_type, embeddings, project_id, device, platform_url, model_args)
 ```
 
 ### Features
 
 - Load any causal model from Huggingface.
 - Create a project for your experiment
 - Run experimental prompts
 
 ### Demo
 
 A demo can be found at [https://helmet.jeroennelen.nl](https://helmet.jeroennelen.nl)
 
+### Component architecture
+
+<p align="center">
+<img  width="75%" src="docs/helmet simplified.png" />
+</p>
+
 ## Install from source
 
 To use helmet in one of the examples perform the following steps:
 
 1. Create venv with `python -m venv .venv`
 2. Activate the venv with `source .venv/bin/activate`
 3. Install HELMET from source (from git, when located in the home folder of helmet `pip install -e .`
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

