# Comparing `tmp/substrate-120240502.0.1.tar.gz` & `tmp/substrate-120240502.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrate-120240502.0.1.tar", max compression
+gzip compressed data, was "substrate-120240502.0.2.tar", max compression
```

## Comparing `substrate-120240502.0.1.tar` & `substrate-120240502.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1066 2024-03-19 21:46:08.735767 substrate-120240502.0.1/LICENSE
--rw-r--r--   0        0        0     2715 2024-05-01 20:59:44.017862 substrate-120240502.0.1/README.md
--rw-r--r--   0        0        0     2079 2024-05-06 20:37:10.262783 substrate-120240502.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-11 19:17:25.000000 substrate-120240502.0.1/substrate/.keep
--rw-r--r--   0        0        0       17 2024-05-02 15:36:22.000000 substrate-120240502.0.1/substrate/GEN_VERSION
--rw-r--r--   0        0        0     2188 2024-05-02 15:36:23.000000 substrate-120240502.0.1/substrate/__init__.py
--rw-r--r--   0        0        0     5773 2024-05-06 20:31:04.737347 substrate-120240502.0.1/substrate/_client.py
--rw-r--r--   0        0        0       30 2024-03-13 14:46:31.829473 substrate-120240502.0.1/substrate/_version.py
--rw-r--r--   0        0        0        1 2024-05-06 18:17:22.557192 substrate-120240502.0.1/substrate/core/__init__.py
--rw-r--r--   0        0        0       27 2024-05-06 18:17:22.556974 substrate-120240502.0.1/substrate/core/_version.py
--rw-r--r--   0        0        0     1535 2024-05-06 18:17:22.557750 substrate-120240502.0.1/substrate/core/base_future.py
--rw-r--r--   0        0        0        0 2024-05-06 18:17:22.558969 substrate-120240502.0.1/substrate/core/client/__init__.py
--rw-r--r--   0        0        0     1750 2024-05-06 18:17:22.559173 substrate-120240502.0.1/substrate/core/client/find_futures_client.py
--rw-r--r--   0        0        0     2697 2024-05-06 18:17:22.559372 substrate-120240502.0.1/substrate/core/client/future.py
--rw-r--r--   0        0        0     1212 2024-05-06 18:17:22.558706 substrate-120240502.0.1/substrate/core/client/graph.py
--rw-r--r--   0        0        0     1149 2024-05-06 18:17:22.557488 substrate-120240502.0.1/substrate/core/coregraph.py
--rw-r--r--   0        0        0     2212 2024-05-06 18:17:22.552509 substrate-120240502.0.1/substrate/core/corenode.py
--rw-r--r--   0        0        0     1587 2024-05-06 18:17:22.557988 substrate-120240502.0.1/substrate/core/future_directive.py
--rw-r--r--   0        0        0      894 2024-05-06 18:17:22.552230 substrate-120240502.0.1/substrate/core/id_generator.py
--rw-r--r--   0        0        0    37176 2024-05-06 18:17:22.556197 substrate-120240502.0.1/substrate/core/models.py
--rw-r--r--   0        0        0     3798 2024-05-06 18:17:22.551865 substrate-120240502.0.1/substrate/core/sb.py
--rw-r--r--   0        0        0    32553 2024-04-19 00:53:25.000000 substrate-120240502.0.1/substrate/dataclass_models.py
--rw-r--r--   0        0        0    47757 2024-05-02 15:36:20.000000 substrate-120240502.0.1/substrate/future_dataclass_models.py
--rw-r--r--   0        0        0    42949 2024-05-02 15:36:23.000000 substrate-120240502.0.1/substrate/nodes.py
--rw-r--r--   0        0        0        0 2024-02-07 23:39:17.000078 substrate-120240502.0.1/substrate/py.typed
--rw-r--r--   0        0        0     2196 2024-05-06 18:16:14.492293 substrate-120240502.0.1/substrate/substrate.py
--rw-r--r--   0        0        0     1015 2024-04-30 17:24:23.842724 substrate-120240502.0.1/substrate/substrate_response.py
--rw-r--r--   0        0        0    37584 2024-05-02 15:36:18.000000 substrate-120240502.0.1/substrate/typeddict_models.py
--rw-r--r--   0        0        0     3352 1970-01-01 00:00:00.000000 substrate-120240502.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-19 21:46:08.735767 substrate-120240502.0.2/LICENSE
+-rw-r--r--   0        0        0     2715 2024-05-01 20:59:44.017862 substrate-120240502.0.2/README.md
+-rw-r--r--   0        0        0     2079 2024-05-07 18:33:22.925402 substrate-120240502.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 19:17:25.000000 substrate-120240502.0.2/substrate/.keep
+-rw-r--r--   0        0        0       17 2024-05-02 15:36:22.000000 substrate-120240502.0.2/substrate/GEN_VERSION
+-rw-r--r--   0        0        0     2188 2024-05-02 15:36:23.000000 substrate-120240502.0.2/substrate/__init__.py
+-rw-r--r--   0        0        0     5773 2024-05-06 20:31:04.737347 substrate-120240502.0.2/substrate/_client.py
+-rw-r--r--   0        0        0       29 2024-05-07 18:33:22.926841 substrate-120240502.0.2/substrate/_version.py
+-rw-r--r--   0        0        0        1 2024-05-06 18:17:22.557192 substrate-120240502.0.2/substrate/core/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-06 18:17:22.556974 substrate-120240502.0.2/substrate/core/_version.py
+-rw-r--r--   0        0        0     1535 2024-05-06 18:17:22.557750 substrate-120240502.0.2/substrate/core/base_future.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:17:22.558969 substrate-120240502.0.2/substrate/core/client/__init__.py
+-rw-r--r--   0        0        0     1750 2024-05-06 18:17:22.559173 substrate-120240502.0.2/substrate/core/client/find_futures_client.py
+-rw-r--r--   0        0        0     2697 2024-05-06 18:17:22.559372 substrate-120240502.0.2/substrate/core/client/future.py
+-rw-r--r--   0        0        0     1212 2024-05-06 18:17:22.558706 substrate-120240502.0.2/substrate/core/client/graph.py
+-rw-r--r--   0        0        0     1149 2024-05-06 18:17:22.557488 substrate-120240502.0.2/substrate/core/coregraph.py
+-rw-r--r--   0        0        0     2212 2024-05-06 18:17:22.552509 substrate-120240502.0.2/substrate/core/corenode.py
+-rw-r--r--   0        0        0     1587 2024-05-06 18:17:22.557988 substrate-120240502.0.2/substrate/core/future_directive.py
+-rw-r--r--   0        0        0      894 2024-05-06 18:17:22.552230 substrate-120240502.0.2/substrate/core/id_generator.py
+-rw-r--r--   0        0        0    37176 2024-05-06 18:17:22.556197 substrate-120240502.0.2/substrate/core/models.py
+-rw-r--r--   0        0        0     3798 2024-05-06 18:17:22.551865 substrate-120240502.0.2/substrate/core/sb.py
+-rw-r--r--   0        0        0    32553 2024-04-19 00:53:25.000000 substrate-120240502.0.2/substrate/dataclass_models.py
+-rw-r--r--   0        0        0    47757 2024-05-02 15:36:20.000000 substrate-120240502.0.2/substrate/future_dataclass_models.py
+-rw-r--r--   0        0        0    42949 2024-05-02 15:36:23.000000 substrate-120240502.0.2/substrate/nodes.py
+-rw-r--r--   0        0        0        0 2024-02-07 23:39:17.000078 substrate-120240502.0.2/substrate/py.typed
+-rw-r--r--   0        0        0     2196 2024-05-06 18:16:14.492293 substrate-120240502.0.2/substrate/substrate.py
+-rw-r--r--   0        0        0     1015 2024-04-30 17:24:23.842724 substrate-120240502.0.2/substrate/substrate_response.py
+-rw-r--r--   0        0        0    37584 2024-05-02 15:36:18.000000 substrate-120240502.0.2/substrate/typeddict_models.py
+-rw-r--r--   0        0        0     3352 1970-01-01 00:00:00.000000 substrate-120240502.0.2/PKG-INFO
```

### Comparing `substrate-120240502.0.1/LICENSE` & `substrate-120240502.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.1/README.md` & `substrate-120240502.0.2/README.md`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.1/pyproject.toml` & `substrate-120240502.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "substrate"
-version = "120240502.0.1"
+version = "120240502.0.2"
 description = "Substrate Python SDK"
 readme = "README.md"
 authors = [ "vprtwn <ben@substrate.run>", "liamgriffiths <liam@substrate.run>",]
 [[tool.poetry.packages]]
 include = "substrate"
 
 [tool.pyright]
```

### Comparing `substrate-120240502.0.1/substrate/__init__.py` & `substrate-120240502.0.2/substrate/__init__.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.1/substrate/_client.py` & `substrate-120240502.0.2/substrate/_client.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.1/substrate/core/base_future.py` & `substrate-120240502.0.2/substrate/core/base_future.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.1/substrate/core/client/find_futures_client.py` & `substrate-120240502.0.2/substrate/core/client/find_futures_client.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.1/substrate/core/client/future.py` & `substrate-120240502.0.2/substrate/core/client/future.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.1/substrate/core/client/graph.py` & `substrate-120240502.0.2/substrate/core/client/graph.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.1/substrate/core/coregraph.py` & `substrate-120240502.0.2/substrate/core/coregraph.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.1/substrate/core/corenode.py` & `substrate-120240502.0.2/substrate/core/corenode.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.1/substrate/core/future_directive.py` & `substrate-120240502.0.2/substrate/core/future_directive.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.1/substrate/core/id_generator.py` & `substrate-120240502.0.2/substrate/core/id_generator.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.1/substrate/core/models.py` & `substrate-120240502.0.2/substrate/core/models.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.1/substrate/core/sb.py` & `substrate-120240502.0.2/substrate/core/sb.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.1/substrate/dataclass_models.py` & `substrate-120240502.0.2/substrate/dataclass_models.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.1/substrate/future_dataclass_models.py` & `substrate-120240502.0.2/substrate/future_dataclass_models.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.1/substrate/nodes.py` & `substrate-120240502.0.2/substrate/nodes.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.1/substrate/substrate.py` & `substrate-120240502.0.2/substrate/substrate.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.1/substrate/substrate_response.py` & `substrate-120240502.0.2/substrate/substrate_response.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.1/substrate/typeddict_models.py` & `substrate-120240502.0.2/substrate/typeddict_models.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.1/PKG-INFO` & `substrate-120240502.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrate
-Version: 120240502.0.1
+Version: 120240502.0.2
 Summary: Substrate Python SDK
 Author: vprtwn
 Author-email: ben@substrate.run
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

