# Comparing `tmp/octoflow_plugins-0.0.4.tar.gz` & `tmp/octoflow_plugins-0.0.5.tar.gz`

## Comparing `octoflow_plugins-0.0.4.tar` & `octoflow_plugins-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,14 @@
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.4/octoflow_plugins/__init__.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.4/octoflow_plugins/data/__init__.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.4/octoflow_plugins/data/loaders.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.4/octoflow_plugins/tracking/__init__.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.4/octoflow_plugins/tracking/artifacts/__init__.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.4/octoflow_plugins/tracking/artifacts/json_handler.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.4/octoflow_plugins/tracking/artifacts/pandas_handler.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.4/octoflow_plugins/tracking/artifacts/pickle_handler.py
--rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.4/octoflow_plugins/tracking/artifacts/safetensors_handler.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.4/octoflow_plugins/tracking/artifacts/torch_handler.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.4/octoflow_plugins/tracking/artifacts/transformers_handler.py
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.4/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.4/LICENSE
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.4/README.md
--rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.5/octoflow_plugins/__init__.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.5/octoflow_plugins/tracking/__init__.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.5/octoflow_plugins/tracking/artifacts/__init__.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.5/octoflow_plugins/tracking/artifacts/json_handler.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.5/octoflow_plugins/tracking/artifacts/pandas_handler.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.5/octoflow_plugins/tracking/artifacts/pickle_handler.py
+-rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.5/octoflow_plugins/tracking/artifacts/safetensors_handler.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.5/octoflow_plugins/tracking/artifacts/torch_handler.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.5/octoflow_plugins/tracking/artifacts/transformers_handler.py
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.5/LICENSE
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.5/README.md
+-rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 octoflow_plugins-0.0.5/PKG-INFO
```

### Comparing `octoflow_plugins-0.0.4/octoflow_plugins/tracking/artifacts/__init__.py` & `octoflow_plugins-0.0.5/octoflow_plugins/tracking/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `octoflow_plugins-0.0.4/octoflow_plugins/tracking/artifacts/json_handler.py` & `octoflow_plugins-0.0.5/octoflow_plugins/tracking/artifacts/json_handler.py`

 * *Files identical despite different names*

### Comparing `octoflow_plugins-0.0.4/octoflow_plugins/tracking/artifacts/pandas_handler.py` & `octoflow_plugins-0.0.5/octoflow_plugins/tracking/artifacts/pandas_handler.py`

 * *Files identical despite different names*

### Comparing `octoflow_plugins-0.0.4/octoflow_plugins/tracking/artifacts/pickle_handler.py` & `octoflow_plugins-0.0.5/octoflow_plugins/tracking/artifacts/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `octoflow_plugins-0.0.4/octoflow_plugins/tracking/artifacts/safetensors_handler.py` & `octoflow_plugins-0.0.5/octoflow_plugins/tracking/artifacts/safetensors_handler.py`

 * *Files identical despite different names*

### Comparing `octoflow_plugins-0.0.4/octoflow_plugins/tracking/artifacts/torch_handler.py` & `octoflow_plugins-0.0.5/octoflow_plugins/tracking/artifacts/torch_handler.py`

 * *Files identical despite different names*

### Comparing `octoflow_plugins-0.0.4/octoflow_plugins/tracking/artifacts/transformers_handler.py` & `octoflow_plugins-0.0.5/octoflow_plugins/tracking/artifacts/transformers_handler.py`

 * *Files identical despite different names*

### Comparing `octoflow_plugins-0.0.4/.gitignore` & `octoflow_plugins-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `octoflow_plugins-0.0.4/LICENSE` & `octoflow_plugins-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `octoflow_plugins-0.0.4/pyproject.toml` & `octoflow_plugins-0.0.5/pyproject.toml`

 * *Files identical despite different names*

