# Comparing `tmp/soroban-0.7.2.tar.gz` & `tmp/soroban-0.8.0.tar.gz`

## Comparing `soroban-0.7.2.tar` & `soroban-0.8.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     5452 2020-02-02 00:00:00.000000 soroban-0.7.2/CONTRIBUTING.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 soroban-0.7.2/tea.yaml
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 soroban-0.7.2/src/soroban/__init__.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 soroban-0.7.2/src/soroban/cli.py
--rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 soroban-0.7.2/src/soroban/create.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 soroban-0.7.2/src/soroban/deploy.py
--rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 soroban-0.7.2/src/soroban/invoke.py
--rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 soroban-0.7.2/src/soroban/models.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 soroban-0.7.2/.gitignore
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 soroban-0.7.2/LICENSE.txt
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 soroban-0.7.2/README.md
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 soroban-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 soroban-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     5452 2020-02-02 00:00:00.000000 soroban-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 soroban-0.8.0/tea.yaml
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 soroban-0.8.0/src/soroban/__init__.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 soroban-0.8.0/src/soroban/cli.py
+-rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 soroban-0.8.0/src/soroban/create.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 soroban-0.8.0/src/soroban/deploy.py
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 soroban-0.8.0/src/soroban/invoke.py
+-rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 soroban-0.8.0/src/soroban/models.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 soroban-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 soroban-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 soroban-0.8.0/README.md
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 soroban-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4475 2020-02-02 00:00:00.000000 soroban-0.8.0/PKG-INFO
```

### Comparing `soroban-0.7.2/CONTRIBUTING.md` & `soroban-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `soroban-0.7.2/src/soroban/cli.py` & `soroban-0.8.0/src/soroban/cli.py`

 * *Files identical despite different names*

### Comparing `soroban-0.7.2/src/soroban/create.py` & `soroban-0.8.0/src/soroban/create.py`

 * *Files identical despite different names*

### Comparing `soroban-0.7.2/src/soroban/deploy.py` & `soroban-0.8.0/src/soroban/deploy.py`

 * *Files identical despite different names*

### Comparing `soroban-0.7.2/src/soroban/invoke.py` & `soroban-0.8.0/src/soroban/invoke.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         else soroban_models.Identity.from_source_account(account=source_account)
     )
     network = (
         network
         if isinstance(network, soroban_models.NetworkConfig)
         else soroban_models.NetworkConfig.from_network(network=network)
     )
+    args = args.model_dump() if isinstance(args, soroban_models.Parameters) else args
 
     soroban_server = stellar_sdk.SorobanServer(network.rpc_url)
     source_account_ = soroban_server.load_account(identity.public_key)
 
     tx = (
         stellar_sdk.TransactionBuilder(
             source_account_, network.network_passphrase, base_fee=network.base_fee
```

### Comparing `soroban-0.7.2/src/soroban/models.py` & `soroban-0.8.0/src/soroban/models.py`

 * *Files identical despite different names*

### Comparing `soroban-0.7.2/LICENSE.txt` & `soroban-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `soroban-0.7.2/README.md` & `soroban-0.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 can be easily generated
 
 ```python
 import json
 import soroban
 
 args = json.load(...)
-args = soroban.Parameters(args=args).model_dump()
+args = soroban.Parameters(args=args)
 soroban.invoke(contract_id="AAAA...", function_name="init", args=args)
 ```
 
 The following JSON syntax is supported. Note that vectors are also supported:
 ```json
 [
   {
```

### Comparing `soroban-0.7.2/pyproject.toml` & `soroban-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `soroban-0.7.2/PKG-INFO` & `soroban-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: soroban
-Version: 0.7.2
+Version: 0.8.0
 Summary: API and CLI for Soroban contracts in Python
 Project-URL: homepage, https://github.com/tupui/soroban-cli-python
 Project-URL: documentation, https://github.com/tupui/soroban-cli-python
 Project-URL: source, https://github.com/tupui/soroban-cli-python
 Author: Pamphile Roy
 Maintainer: Soroban API/CLI contributors
 License-Expression: BSD-3-Clause
@@ -79,15 +79,15 @@
 can be easily generated
 
 ```python
 import json
 import soroban
 
 args = json.load(...)
-args = soroban.Parameters(args=args).model_dump()
+args = soroban.Parameters(args=args)
 soroban.invoke(contract_id="AAAA...", function_name="init", args=args)
 ```
 
 The following JSON syntax is supported. Note that vectors are also supported:
 ```json
 [
   {
```

