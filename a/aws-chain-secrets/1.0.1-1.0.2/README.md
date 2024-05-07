# Comparing `tmp/aws_chain_secrets-1.0.1.tar.gz` & `tmp/aws_chain_secrets-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_chain_secrets-1.0.1.tar", last modified: Sun Apr 23 06:25:57 2023, max compression
+gzip compressed data, was "aws_chain_secrets-1.0.2.tar", last modified: Tue May  7 08:21:33 2024, max compression
```

## Comparing `aws_chain_secrets-1.0.1.tar` & `aws_chain_secrets-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hyouk      (501) staff       (20)        0 2023-04-23 06:25:57.091938 aws_chain_secrets-1.0.1/
--rw-r--r--   0 hyouk      (501) staff       (20)     1065 2023-04-23 06:20:51.000000 aws_chain_secrets-1.0.1/LICENSE
--rw-r--r--   0 hyouk      (501) staff       (20)     3519 2023-04-23 06:25:57.091797 aws_chain_secrets-1.0.1/PKG-INFO
--rw-r--r--   0 hyouk      (501) staff       (20)     2835 2023-04-23 06:20:51.000000 aws_chain_secrets-1.0.1/README.rst
-drwxr-xr-x   0 hyouk      (501) staff       (20)        0 2023-04-23 06:25:57.090423 aws_chain_secrets-1.0.1/aws_chain_secrets/
--rw-r--r--   0 hyouk      (501) staff       (20)       44 2023-04-23 06:20:51.000000 aws_chain_secrets-1.0.1/aws_chain_secrets/__init__.py
--rw-r--r--   0 hyouk      (501) staff       (20)     2142 2023-04-23 06:20:51.000000 aws_chain_secrets-1.0.1/aws_chain_secrets/caster.py
--rw-r--r--   0 hyouk      (501) staff       (20)     1173 2023-04-23 06:20:51.000000 aws_chain_secrets-1.0.1/aws_chain_secrets/client.py
--rw-r--r--   0 hyouk      (501) staff       (20)     1597 2023-04-23 06:20:51.000000 aws_chain_secrets-1.0.1/aws_chain_secrets/exceptions.py
--rw-r--r--   0 hyouk      (501) staff       (20)        0 2023-04-23 06:20:51.000000 aws_chain_secrets-1.0.1/aws_chain_secrets/py.typed
--rw-r--r--   0 hyouk      (501) staff       (20)     3621 2023-04-23 06:20:51.000000 aws_chain_secrets-1.0.1/aws_chain_secrets/secrets_manager.py
-drwxr-xr-x   0 hyouk      (501) staff       (20)        0 2023-04-23 06:25:57.091355 aws_chain_secrets-1.0.1/aws_chain_secrets.egg-info/
--rw-r--r--   0 hyouk      (501) staff       (20)     3519 2023-04-23 06:25:57.000000 aws_chain_secrets-1.0.1/aws_chain_secrets.egg-info/PKG-INFO
--rw-r--r--   0 hyouk      (501) staff       (20)      452 2023-04-23 06:25:57.000000 aws_chain_secrets-1.0.1/aws_chain_secrets.egg-info/SOURCES.txt
--rw-r--r--   0 hyouk      (501) staff       (20)        1 2023-04-23 06:25:57.000000 aws_chain_secrets-1.0.1/aws_chain_secrets.egg-info/dependency_links.txt
--rw-r--r--   0 hyouk      (501) staff       (20)        6 2023-04-23 06:25:57.000000 aws_chain_secrets-1.0.1/aws_chain_secrets.egg-info/requires.txt
--rw-r--r--   0 hyouk      (501) staff       (20)       24 2023-04-23 06:25:57.000000 aws_chain_secrets-1.0.1/aws_chain_secrets.egg-info/top_level.txt
--rw-r--r--   0 hyouk      (501) staff       (20)       38 2023-04-23 06:25:57.091972 aws_chain_secrets-1.0.1/setup.cfg
--rw-r--r--   0 hyouk      (501) staff       (20)     1022 2023-04-23 06:25:43.000000 aws_chain_secrets-1.0.1/setup.py
-drwxr-xr-x   0 hyouk      (501) staff       (20)        0 2023-04-23 06:25:57.091602 aws_chain_secrets-1.0.1/tests/
--rw-r--r--   0 hyouk      (501) staff       (20)        0 2023-04-23 06:20:51.000000 aws_chain_secrets-1.0.1/tests/__init__.py
--rw-r--r--   0 hyouk      (501) staff       (20)      631 2023-04-23 06:20:51.000000 aws_chain_secrets-1.0.1/tests/test_caster.py
+drwxr-xr-x   0 hyouk      (501) staff       (20)        0 2024-05-07 08:21:33.853196 aws_chain_secrets-1.0.2/
+-rw-r--r--   0 hyouk      (501) staff       (20)     1065 2023-04-23 06:20:51.000000 aws_chain_secrets-1.0.2/LICENSE
+-rw-r--r--   0 hyouk      (501) staff       (20)     3767 2024-05-07 08:21:33.853009 aws_chain_secrets-1.0.2/PKG-INFO
+-rw-r--r--   0 hyouk      (501) staff       (20)     3062 2024-05-07 08:14:32.000000 aws_chain_secrets-1.0.2/README.rst
+drwxr-xr-x   0 hyouk      (501) staff       (20)        0 2024-05-07 08:21:33.851215 aws_chain_secrets-1.0.2/aws_chain_secrets/
+-rw-r--r--   0 hyouk      (501) staff       (20)       44 2023-04-23 06:20:51.000000 aws_chain_secrets-1.0.2/aws_chain_secrets/__init__.py
+-rw-r--r--   0 hyouk      (501) staff       (20)     2142 2023-04-23 06:20:51.000000 aws_chain_secrets-1.0.2/aws_chain_secrets/caster.py
+-rw-r--r--   0 hyouk      (501) staff       (20)     1173 2023-04-23 06:20:51.000000 aws_chain_secrets-1.0.2/aws_chain_secrets/client.py
+-rw-r--r--   0 hyouk      (501) staff       (20)     1597 2023-04-23 06:20:51.000000 aws_chain_secrets-1.0.2/aws_chain_secrets/exceptions.py
+-rw-r--r--   0 hyouk      (501) staff       (20)        0 2023-04-23 06:20:51.000000 aws_chain_secrets-1.0.2/aws_chain_secrets/py.typed
+-rw-r--r--   0 hyouk      (501) staff       (20)     4101 2024-05-07 08:14:20.000000 aws_chain_secrets-1.0.2/aws_chain_secrets/secrets_manager.py
+drwxr-xr-x   0 hyouk      (501) staff       (20)        0 2024-05-07 08:21:33.852687 aws_chain_secrets-1.0.2/aws_chain_secrets.egg-info/
+-rw-r--r--   0 hyouk      (501) staff       (20)     3767 2024-05-07 08:21:33.000000 aws_chain_secrets-1.0.2/aws_chain_secrets.egg-info/PKG-INFO
+-rw-r--r--   0 hyouk      (501) staff       (20)      452 2024-05-07 08:21:33.000000 aws_chain_secrets-1.0.2/aws_chain_secrets.egg-info/SOURCES.txt
+-rw-r--r--   0 hyouk      (501) staff       (20)        1 2024-05-07 08:21:33.000000 aws_chain_secrets-1.0.2/aws_chain_secrets.egg-info/dependency_links.txt
+-rw-r--r--   0 hyouk      (501) staff       (20)        6 2024-05-07 08:21:33.000000 aws_chain_secrets-1.0.2/aws_chain_secrets.egg-info/requires.txt
+-rw-r--r--   0 hyouk      (501) staff       (20)       24 2024-05-07 08:21:33.000000 aws_chain_secrets-1.0.2/aws_chain_secrets.egg-info/top_level.txt
+-rw-r--r--   0 hyouk      (501) staff       (20)       38 2024-05-07 08:21:33.853353 aws_chain_secrets-1.0.2/setup.cfg
+-rw-r--r--   0 hyouk      (501) staff       (20)     1022 2024-05-07 08:11:23.000000 aws_chain_secrets-1.0.2/setup.py
+drwxr-xr-x   0 hyouk      (501) staff       (20)        0 2024-05-07 08:21:33.852333 aws_chain_secrets-1.0.2/tests/
+-rw-r--r--   0 hyouk      (501) staff       (20)        0 2023-04-23 06:20:51.000000 aws_chain_secrets-1.0.2/tests/__init__.py
+-rw-r--r--   0 hyouk      (501) staff       (20)      631 2023-04-23 06:20:51.000000 aws_chain_secrets-1.0.2/tests/test_caster.py
```

### Comparing `aws_chain_secrets-1.0.1/LICENSE` & `aws_chain_secrets-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_chain_secrets-1.0.1/PKG-INFO` & `aws_chain_secrets-1.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: aws_chain_secrets
-Version: 1.0.1
+Version: 1.0.2
 Summary: This aims to enable the use of one or more secrets from AWS SecretsManager.
 Home-page: https://github.com/h5kure/aws_chain_secrets
 Author: Hyouk Oh
 Author-email: h.5.kure@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: boto3
 
 AWS chain secrets
 ===================
 
 This package aims to make using AWS SecretsManager more comfortable.
 
 Introduce
@@ -114,14 +115,16 @@
     >>> secrets(key="A", default=0)
     0
 
 change value
 """"""""""""
 
 You can change (or add) the value of a specified secret by name.
+If `None` is given, the value is set to the highest priority secret (last given as a parameter) with key value.
+If there is no secret with the given key, it is registered as a new value in the secret with the highest priority.
 
 .. code-block:: python
 
     >>> secrets.set('secret_name_1', 'key', 'value')
 
 update remote (AWS secrets manager) data from local
 """""""""""""""""""""""""""""""""""""""""""""""""""
```

### Comparing `aws_chain_secrets-1.0.1/README.rst` & `aws_chain_secrets-1.0.2/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -96,14 +96,16 @@
     >>> secrets(key="A", default=0)
     0
 
 change value
 """"""""""""
 
 You can change (or add) the value of a specified secret by name.
+If `None` is given, the value is set to the highest priority secret (last given as a parameter) with key value.
+If there is no secret with the given key, it is registered as a new value in the secret with the highest priority.
 
 .. code-block:: python
 
     >>> secrets.set('secret_name_1', 'key', 'value')
 
 update remote (AWS secrets manager) data from local
 """""""""""""""""""""""""""""""""""""""""""""""""""
```

### Comparing `aws_chain_secrets-1.0.1/aws_chain_secrets/caster.py` & `aws_chain_secrets-1.0.2/aws_chain_secrets/caster.py`

 * *Files identical despite different names*

### Comparing `aws_chain_secrets-1.0.1/aws_chain_secrets/client.py` & `aws_chain_secrets-1.0.2/aws_chain_secrets/client.py`

 * *Files identical despite different names*

### Comparing `aws_chain_secrets-1.0.1/aws_chain_secrets/exceptions.py` & `aws_chain_secrets-1.0.2/aws_chain_secrets/exceptions.py`

 * *Files identical despite different names*

### Comparing `aws_chain_secrets-1.0.1/aws_chain_secrets/secrets_manager.py` & `aws_chain_secrets-1.0.2/aws_chain_secrets/secrets_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             *secret_names: str,
             aws_access_key_id: str = None,
             aws_secret_access_key: str = None
     ):
         """
         initial setup
         :param region_name: AWS region name
-        :param secret_names: These are the secret names from which to read settings. The last name has priority.
+        :param secret_names: The secret names that come later has higher precedence..
         """
         self.secret_names = secret_names
         super().__init__(
             "secretsmanager",
             region_name,
             aws_access_key_id,
             aws_secret_access_key
@@ -66,18 +66,27 @@
                 raise KeyError(f"{repr(key)} not found. Please check secret value in AWS Secrets Manager.")
             return default
         return cast(value, casting_type)
 
     def set(self, secret_name: str, key, value):
         """
         set a `key: value` to the specified secret
-        :param secret_name: secret_name of AWS Secrets Manager
+        :param secret_name: secret_name of AWS Secrets Manager.
+         If None is given, the value is set to the highest priority secret (last given as a parameter) with key value.
+         If there is no secret with the given key,
+          it is registered as a new value in the secret with the highest priority.
         :param key: key of map
         :param value: value of map
         """
+        if secret_name is None:
+            for name in reversed(self._secrets.keys()):
+                if secret_name is None:
+                    secret_name = name
+                if key in self._secrets[name]:
+                    secret_name = name
         self._secrets[secret_name][key] = value
 
     def keys(self):
         return self._combined.keys()
 
     def values(self):
         return self._combined.values()
```

### Comparing `aws_chain_secrets-1.0.1/aws_chain_secrets.egg-info/PKG-INFO` & `aws_chain_secrets-1.0.2/aws_chain_secrets.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
-Name: aws-chain-secrets
-Version: 1.0.1
+Name: aws_chain_secrets
+Version: 1.0.2
 Summary: This aims to enable the use of one or more secrets from AWS SecretsManager.
 Home-page: https://github.com/h5kure/aws_chain_secrets
 Author: Hyouk Oh
 Author-email: h.5.kure@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: boto3
 
 AWS chain secrets
 ===================
 
 This package aims to make using AWS SecretsManager more comfortable.
 
 Introduce
@@ -114,14 +115,16 @@
     >>> secrets(key="A", default=0)
     0
 
 change value
 """"""""""""
 
 You can change (or add) the value of a specified secret by name.
+If `None` is given, the value is set to the highest priority secret (last given as a parameter) with key value.
+If there is no secret with the given key, it is registered as a new value in the secret with the highest priority.
 
 .. code-block:: python
 
     >>> secrets.set('secret_name_1', 'key', 'value')
 
 update remote (AWS secrets manager) data from local
 """""""""""""""""""""""""""""""""""""""""""""""""""
```

### Comparing `aws_chain_secrets-1.0.1/setup.py` & `aws_chain_secrets-1.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.rst", "r", encoding='utf-8') as readme:
     long_description = readme.read()
 
 setuptools.setup(
     name="aws_chain_secrets",
-    version='1.0.1',
+    version='1.0.2',
     author="Hyouk Oh",
     author_email="h.5.kure@gmail.com",
     description="This aims to enable the use of one or more secrets from AWS SecretsManager.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/h5kure/aws_chain_secrets",
     packages=setuptools.find_packages(),
```

### Comparing `aws_chain_secrets-1.0.1/tests/test_caster.py` & `aws_chain_secrets-1.0.2/tests/test_caster.py`

 * *Files identical despite different names*

