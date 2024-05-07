# Comparing `tmp/naas_python-1.3.2.tar.gz` & `tmp/naas_python-1.4.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naas_python-1.3.2.tar", max compression
+gzip compressed data, was "naas_python-1.4.0.dev1.tar", max compression
```

## Comparing `naas_python-1.3.2.tar` & `naas_python-1.4.0.dev1.tar`

### file list

```diff
@@ -1,40 +1,59 @@
--rw-r--r--   0        0        0    34523 2024-05-07 10:20:58.951112 naas_python-1.3.2/LICENSE
--rw-r--r--   0        0        0       13 2024-05-07 10:20:58.951112 naas_python-1.3.2/README.md
--rw-r--r--   0        0        0      303 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/__init__.py
--rw-r--r--   0        0        0     1030 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/cli.py
--rw-r--r--   0        0        0     1398 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/domains/registry/RegistryDomain.py
--rw-r--r--   0        0        0     2174 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/domains/registry/RegistrySchema.py
--rw-r--r--   0        0        0     2006 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/domains/registry/adaptors/primary/SDKRegistryAdaptor.py
--rw-r--r--   0        0        0     7354 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/domains/registry/adaptors/primary/TyperRegistryAdaptor.py
--rw-r--r--   0        0        0     6393 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/domains/registry/adaptors/secondary/NaasRegistryAPIAdaptor.py
--rw-r--r--   0        0        0      329 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/domains/registry/handlers/CLIRegistryHandler.py
--rw-r--r--   0        0        0      323 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/domains/registry/handlers/PythonHandler.py
--rw-r--r--   0        0        0     1220 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/domains/secret/SecretDomain.py
--rw-r--r--   0        0        0     2119 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/domains/secret/SecretSchema.py
--rw-r--r--   0        0        0     1392 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/domains/secret/adaptors/primary/SDKSecretAdaptor.py
--rw-r--r--   0        0        0     5705 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/domains/secret/adaptors/primary/TyperSecretAdaptor.py
--rw-r--r--   0        0        0     1331 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/domains/secret/adaptors/primary/utils.py
--rw-r--r--   0        0        0     4660 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/domains/secret/adaptors/secondary/NaasSecretAPIAdaptor.py
--rw-r--r--   0        0        0      523 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/domains/secret/handlers/CLISecretHandler.py
--rw-r--r--   0        0        0      305 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/domains/secret/handlers/PythonHandler.py
--rw-r--r--   0        0        0       45 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/domains/secret/models/Secret.py
--rw-r--r--   0        0        0       26 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/domains/secret/models/__init__.py
--rw-r--r--   0        0        0     1251 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/domains/space/SpaceDomain.py
--rw-r--r--   0        0        0     2192 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/domains/space/SpaceSchema.py
--rw-r--r--   0        0        0     7702 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/domains/space/adaptors/primary/SDKSpaceAdaptor.py
--rw-r--r--   0        0        0    17679 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/domains/space/adaptors/primary/TyperSpaceAdaptor.py
--rw-r--r--   0        0        0     1329 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/domains/space/adaptors/primary/utils.py
--rw-r--r--   0        0        0     7609 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/domains/space/adaptors/secondary/NaasSpaceAPIAdaptor.py
--rw-r--r--   0        0        0      512 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/domains/space/handlers/CLISpaceHandler.py
--rw-r--r--   0        0        0      296 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/domains/space/handlers/PythonHandler.py
--rw-r--r--   0        0        0       96 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/main.py
--rw-r--r--   0        0        0        0 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/utils/__init__.py
--rw-r--r--   0        0        0     2039 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/utils/cicd.py
--rw-r--r--   0        0        0        0 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/utils/domains_base/__init__.py
--rw-r--r--   0        0        0    15947 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/utils/domains_base/authorization.py
--rw-r--r--   0        0        0     4022 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/utils/domains_base/secondary/BaseAPIAdaptor.py
--rw-r--r--   0        0        0     3203 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/utils/exceptions.py
--rw-r--r--   0        0        0     1873 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/utils/log.py
--rw-r--r--   0        0        0      357 2024-05-07 10:20:58.951112 naas_python-1.3.2/naas_python/utils/workflow_template.j2
--rw-r--r--   0        0        0      762 2024-05-07 10:21:13.467202 naas_python-1.3.2/pyproject.toml
--rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 naas_python-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-03 12:19:12.825601 naas_python-1.4.0.dev1/LICENSE
+-rw-r--r--   0        0        0       13 2024-05-03 12:19:12.825601 naas_python-1.4.0.dev1/README.md
+-rw-r--r--   0        0        0      455 2024-05-03 12:19:12.825601 naas_python-1.4.0.dev1/naas_python/__init__.py
+-rw-r--r--   0        0        0     1429 2024-05-03 12:19:12.825601 naas_python-1.4.0.dev1/naas_python/cli.py
+-rw-r--r--   0        0        0      996 2024-05-03 12:19:12.825601 naas_python-1.4.0.dev1/naas_python/domains/asset/AssetDomain.py
+-rw-r--r--   0        0        0     1651 2024-05-03 12:19:12.825601 naas_python-1.4.0.dev1/naas_python/domains/asset/AssetSchema.py
+-rw-r--r--   0        0        0     1167 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/asset/adaptors/primary/SDKAssetAdaptor.py
+-rw-r--r--   0        0        0     6097 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/asset/adaptors/primary/TyperAssetAdaptor.py
+-rw-r--r--   0        0        0     2884 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/asset/adaptors/secondary/NaasAssetAPIAdaptor.py
+-rw-r--r--   0        0        0      392 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/asset/handlers/CLIAssetHandler.py
+-rw-r--r--   0        0        0      367 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/asset/handlers/PythonHandler.py
+-rw-r--r--   0        0        0       44 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/asset/models/Asset.py
+-rw-r--r--   0        0        0       24 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/asset/models/__init__.py
+-rw-r--r--   0        0        0     1398 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/registry/RegistryDomain.py
+-rw-r--r--   0        0        0     2174 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/registry/RegistrySchema.py
+-rw-r--r--   0        0        0     2006 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/registry/adaptors/primary/SDKRegistryAdaptor.py
+-rw-r--r--   0        0        0     7354 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/registry/adaptors/primary/TyperRegistryAdaptor.py
+-rw-r--r--   0        0        0     6393 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/registry/adaptors/secondary/NaasRegistryAPIAdaptor.py
+-rw-r--r--   0        0        0      329 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/registry/handlers/CLIRegistryHandler.py
+-rw-r--r--   0        0        0      323 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/registry/handlers/PythonHandler.py
+-rw-r--r--   0        0        0     1220 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/secret/SecretDomain.py
+-rw-r--r--   0        0        0     2119 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/secret/SecretSchema.py
+-rw-r--r--   0        0        0     1392 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/secret/adaptors/primary/SDKSecretAdaptor.py
+-rw-r--r--   0        0        0     5705 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/secret/adaptors/primary/TyperSecretAdaptor.py
+-rw-r--r--   0        0        0     1331 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/secret/adaptors/primary/utils.py
+-rw-r--r--   0        0        0     4660 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/secret/adaptors/secondary/NaasSecretAPIAdaptor.py
+-rw-r--r--   0        0        0      523 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/secret/handlers/CLISecretHandler.py
+-rw-r--r--   0        0        0      305 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/secret/handlers/PythonHandler.py
+-rw-r--r--   0        0        0       45 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/secret/models/Secret.py
+-rw-r--r--   0        0        0       26 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/secret/models/__init__.py
+-rw-r--r--   0        0        0     1251 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/space/SpaceDomain.py
+-rw-r--r--   0        0        0     2192 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/space/SpaceSchema.py
+-rw-r--r--   0        0        0     7702 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/space/adaptors/primary/SDKSpaceAdaptor.py
+-rw-r--r--   0        0        0    17679 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/space/adaptors/primary/TyperSpaceAdaptor.py
+-rw-r--r--   0        0        0     1329 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/space/adaptors/primary/utils.py
+-rw-r--r--   0        0        0     7609 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/space/adaptors/secondary/NaasSpaceAPIAdaptor.py
+-rw-r--r--   0        0        0      512 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/space/handlers/CLISpaceHandler.py
+-rw-r--r--   0        0        0      296 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/space/handlers/PythonHandler.py
+-rw-r--r--   0        0        0     4955 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/storage/StorageDomain.py
+-rw-r--r--   0        0        0     5656 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/storage/StorageSchema.py
+-rw-r--r--   0        0        0     3252 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/storage/adaptors/primary/SDKStorageAdaptor.py
+-rw-r--r--   0        0        0     9514 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/storage/adaptors/primary/TyperStorageAdaptor.py
+-rw-r--r--   0        0        0     3994 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/storage/adaptors/secondary/NaasStorageAPIAdaptor.py
+-rw-r--r--   0        0        0    12234 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/storage/adaptors/secondary/providers/S3StorageProviderAdaptor.py
+-rw-r--r--   0        0        0      867 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/storage/handlers/CLIStorageHandler.py
+-rw-r--r--   0        0        0      644 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/storage/handlers/PythonHandler.py
+-rw-r--r--   0        0        0       46 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/storage/models/Storage.py
+-rw-r--r--   0        0        0       28 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/domains/storage/models/__init__.py
+-rw-r--r--   0        0        0       96 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/main.py
+-rw-r--r--   0        0        0        0 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/utils/__init__.py
+-rw-r--r--   0        0        0     2039 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/utils/cicd.py
+-rw-r--r--   0        0        0        0 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/utils/domains_base/__init__.py
+-rw-r--r--   0        0        0    15947 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/utils/domains_base/authorization.py
+-rw-r--r--   0        0        0     4024 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/utils/domains_base/secondary/BaseAPIAdaptor.py
+-rw-r--r--   0        0        0     3203 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/utils/exceptions.py
+-rw-r--r--   0        0        0     1873 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/utils/log.py
+-rw-r--r--   0        0        0      357 2024-05-03 12:19:12.829601 naas_python-1.4.0.dev1/naas_python/utils/workflow_template.j2
+-rw-r--r--   0        0        0      745 2024-05-03 12:19:27.337765 naas_python-1.4.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 naas_python-1.4.0.dev1/PKG-INFO
```

### Comparing `naas_python-1.3.2/LICENSE` & `naas_python-1.4.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.2/naas_python/cli.py` & `naas_python-1.4.0.dev1/naas_python/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import typer
+import logging
+logging.basicConfig(level=logging.ERROR)
 
 from naas_python.domains.registry.handlers.CLIRegistryHandler import (
     primaryAdaptor as typerRegistryAdaptor,
 )
 
 # from naas_python.domains import spaceCliAdaptor  # , registryCliAdaptor
 from naas_python.domains.space.handlers.CLISpaceHandler import (
@@ -10,25 +12,36 @@
 )
 
 # from naas_python.domains import secretCliAdaptor  # , secretCliAdaptor
 from naas_python.domains.secret.handlers.CLISecretHandler import (
     primaryAdaptor as typerSecretAdaptor,
 )
 
+from naas_python.domains.asset.handlers.CLIAssetHandler import (
+    primaryAdaptor as typerAssetAdaptor,
+)
+
+from naas_python.domains.storage.handlers.CLIStorageHandler import (
+    primaryAdaptor as typerStorageAdaptor,
+)
+
 
 def _create_cli_app():
     app = typer.Typer(
         epilog="Found a bug? Report it at https://github.com/jupyter-naas/naas-python/issues",
         pretty_exceptions_show_locals=False,
         pretty_exceptions_short=True,
         # pretty_exceptions_enable=False,
     )
 
     # Registry domain's related commands
     app.add_typer(typerSpaceAdaptor.app, name="space")
     app.add_typer(typerRegistryAdaptor.app, name="registry")
     app.add_typer(typerSecretAdaptor.app, name="secret")
+    app.add_typer(typerAssetAdaptor.app, name="asset")
+    app.add_typer(typerStorageAdaptor.app, name="storage")    
+
 
     return app
 
 
 app = _create_cli_app()
```

### Comparing `naas_python-1.3.2/naas_python/domains/registry/RegistryDomain.py` & `naas_python-1.4.0.dev1/naas_python/domains/registry/RegistryDomain.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.2/naas_python/domains/registry/RegistrySchema.py` & `naas_python-1.4.0.dev1/naas_python/domains/registry/RegistrySchema.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.2/naas_python/domains/registry/adaptors/primary/SDKRegistryAdaptor.py` & `naas_python-1.4.0.dev1/naas_python/domains/registry/adaptors/primary/SDKRegistryAdaptor.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.2/naas_python/domains/registry/adaptors/primary/TyperRegistryAdaptor.py` & `naas_python-1.4.0.dev1/naas_python/domains/registry/adaptors/primary/TyperRegistryAdaptor.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.2/naas_python/domains/registry/adaptors/secondary/NaasRegistryAPIAdaptor.py` & `naas_python-1.4.0.dev1/naas_python/domains/registry/adaptors/secondary/NaasRegistryAPIAdaptor.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.2/naas_python/domains/secret/SecretDomain.py` & `naas_python-1.4.0.dev1/naas_python/domains/secret/SecretDomain.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.2/naas_python/domains/secret/SecretSchema.py` & `naas_python-1.4.0.dev1/naas_python/domains/secret/SecretSchema.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.2/naas_python/domains/secret/adaptors/primary/SDKSecretAdaptor.py` & `naas_python-1.4.0.dev1/naas_python/domains/secret/adaptors/primary/SDKSecretAdaptor.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.2/naas_python/domains/secret/adaptors/primary/TyperSecretAdaptor.py` & `naas_python-1.4.0.dev1/naas_python/domains/secret/adaptors/primary/TyperSecretAdaptor.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.2/naas_python/domains/secret/adaptors/primary/utils.py` & `naas_python-1.4.0.dev1/naas_python/domains/secret/adaptors/primary/utils.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.2/naas_python/domains/secret/adaptors/secondary/NaasSecretAPIAdaptor.py` & `naas_python-1.4.0.dev1/naas_python/domains/secret/adaptors/secondary/NaasSecretAPIAdaptor.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.2/naas_python/domains/secret/handlers/CLISecretHandler.py` & `naas_python-1.4.0.dev1/naas_python/domains/secret/handlers/CLISecretHandler.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.2/naas_python/domains/space/SpaceDomain.py` & `naas_python-1.4.0.dev1/naas_python/domains/space/SpaceDomain.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.2/naas_python/domains/space/SpaceSchema.py` & `naas_python-1.4.0.dev1/naas_python/domains/space/SpaceSchema.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.2/naas_python/domains/space/adaptors/primary/SDKSpaceAdaptor.py` & `naas_python-1.4.0.dev1/naas_python/domains/space/adaptors/primary/SDKSpaceAdaptor.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.2/naas_python/domains/space/adaptors/primary/TyperSpaceAdaptor.py` & `naas_python-1.4.0.dev1/naas_python/domains/space/adaptors/primary/TyperSpaceAdaptor.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.2/naas_python/domains/space/adaptors/primary/utils.py` & `naas_python-1.4.0.dev1/naas_python/domains/space/adaptors/primary/utils.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.2/naas_python/domains/space/adaptors/secondary/NaasSpaceAPIAdaptor.py` & `naas_python-1.4.0.dev1/naas_python/domains/space/adaptors/secondary/NaasSpaceAPIAdaptor.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.2/naas_python/domains/space/handlers/CLISpaceHandler.py` & `naas_python-1.4.0.dev1/naas_python/domains/space/handlers/CLISpaceHandler.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.2/naas_python/utils/cicd.py` & `naas_python-1.4.0.dev1/naas_python/utils/cicd.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.2/naas_python/utils/domains_base/authorization.py` & `naas_python-1.4.0.dev1/naas_python/utils/domains_base/authorization.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.2/naas_python/utils/domains_base/secondary/BaseAPIAdaptor.py` & `naas_python-1.4.0.dev1/naas_python/utils/domains_base/secondary/BaseAPIAdaptor.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 class ServiceStatusError(NaasException):
     pass
 
 
 class BaseAPIAdaptor(NaasSpaceAuthenticatorAdapter):
     host = os.environ.get("NAAS_PYTHON_API_BASE_URL", "https://api.naas.ai")
-    #host = os.environ.get("NAAS_PYTHON_API_BASE_URL", "http://localhost:8000")
+    # host = os.environ.get("NAAS_PYTHON_API_BASE_URL", "http://localhost:8000")
     # Cache name is the name of the calling module
     cache_name = __name__
     cache_expire_after = 60  # Cache expires after 60 seconds
 
     def __init__(self) -> None:
         # Base authenticator class
         super().__init__()
@@ -53,15 +53,15 @@
         except (ConnectionError, NewConnectionError, MaxRetryError) as e:
             raise ServiceStatusError(
                 f"Unable to connect to [cyan]{self.host}[/cyan]. The service is currently unavailable. Please try again within a few minutes.",
                 e,
             )
 
     @staticmethod
-    def service_status_decorator(func):
+    def  service_status_decorator(func):
         def wrapper(self, *args, **kwargs):
             self._check_service_status()
             return func(self, *args, **kwargs)
 
         return wrapper
 
     def make_api_request(
```

### Comparing `naas_python-1.3.2/naas_python/utils/exceptions.py` & `naas_python-1.4.0.dev1/naas_python/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.2/naas_python/utils/log.py` & `naas_python-1.4.0.dev1/naas_python/utils/log.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.2/pyproject.toml` & `naas_python-1.4.0.dev1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 [tool.poetry]
 name = "naas-python"
-version = "1.3.2"
+version = "1.4.0.dev1"
 description = "Naas Python SDK"
 authors = ["Maxime Jublou <maxime@naas.ai>"]
 license = "AGPL"
 readme = "README.md"
 packages = [{ include = "naas_python" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 typer = { extras = ["all"], version = "^0.9.0" }
 requests = "^2.31.0"
+protobuf_to_pydantic = { version = "0.2.6.2" }
 cachetools = "^5.3.1"
-#naas-models = { git = "https://github.com/jupyter-naas/naas-models.git", tag = "v1.4.1", subdirectory = "python" }
 jinja2 = "^3.0.1"
-naas-models = "1.11.1"
+naas-models = "1.11.0"
 grpcio = "^1.60.0"
 pydash = "^7.0.7"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 requests = "^2.31.0"
+protobuf_to_pydantic = { version = "0.2.6.2" }
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 naas-python = "naas_python.main:main"
```

### Comparing `naas_python-1.3.2/PKG-INFO` & `naas_python-1.4.0.dev1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: naas-python
-Version: 1.3.2
+Version: 1.4.0.dev1
 Summary: Naas Python SDK
 License: AGPL
 Author: Maxime Jublou
 Author-email: maxime@naas.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cachetools (>=5.3.1,<6.0.0)
 Requires-Dist: grpcio (>=1.60.0,<2.0.0)
 Requires-Dist: jinja2 (>=3.0.1,<4.0.0)
-Requires-Dist: naas-models (==1.11.1)
+Requires-Dist: naas-models (==1.11.0)
+Requires-Dist: protobuf_to_pydantic (==0.2.6.2)
 Requires-Dist: pydash (>=7.0.7,<8.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # python-naas
```

