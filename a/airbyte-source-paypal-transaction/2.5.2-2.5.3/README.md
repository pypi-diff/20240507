# Comparing `tmp/airbyte_source_paypal_transaction-2.5.2.tar.gz` & `tmp/airbyte_source_paypal_transaction-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_paypal_transaction-2.5.2.tar", max compression
+gzip compressed data, was "airbyte_source_paypal_transaction-2.5.3.tar", max compression
```

## Comparing `airbyte_source_paypal_transaction-2.5.2.tar` & `airbyte_source_paypal_transaction-2.5.3.tar`

### file list

```diff
@@ -1,16 +1,9 @@
--rw-r--r--   0        0        0    11632 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/README.md
--rw-r--r--   0        0        0      832 2024-04-19 13:30:50.120081 airbyte_source_paypal_transaction-2.5.2/pyproject.toml
--rw-r--r--   0        0        0      146 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/__init__.py
--rw-r--r--   0        0        0     3072 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/components.py
--rw-r--r--   0        0        0    13334 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/manifest.yaml
--rw-r--r--   0        0        0      264 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/run.py
--rw-r--r--   0        0        0     1535 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/schemas/balances.json
--rw-r--r--   0        0        0     1772 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/schemas/list_disputes.json
--rw-r--r--   0        0        0     7895 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/schemas/list_payments.json
--rw-r--r--   0        0        0      689 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/schemas/list_products.json
--rw-r--r--   0        0        0    13751 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/schemas/search_invoices.json
--rw-r--r--   0        0        0      946 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/schemas/show_product_details.json
--rw-r--r--   0        0        0    11212 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/schemas/transactions.json
--rw-r--r--   0        0        0      523 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/source.py
--rw-r--r--   0        0        0     3021 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/spec.yaml
--rw-r--r--   0        0        0    12370 1970-01-01 00:00:00.000000 airbyte_source_paypal_transaction-2.5.2/PKG-INFO
+-rw-r--r--   0        0        0    11632 2024-05-07 10:51:28.000000 airbyte_source_paypal_transaction-2.5.3/README.md
+-rw-r--r--   0        0        0      836 2024-05-07 13:36:53.356879 airbyte_source_paypal_transaction-2.5.3/pyproject.toml
+-rw-r--r--   0        0        0      146 2024-05-07 10:51:28.000000 airbyte_source_paypal_transaction-2.5.3/source_paypal_transaction/__init__.py
+-rw-r--r--   0        0        0     3072 2024-05-07 10:51:28.000000 airbyte_source_paypal_transaction-2.5.3/source_paypal_transaction/components.py
+-rw-r--r--   0        0        0   101426 2024-05-07 10:51:28.000000 airbyte_source_paypal_transaction-2.5.3/source_paypal_transaction/manifest.yaml
+-rw-r--r--   0        0        0      264 2024-05-07 10:51:28.000000 airbyte_source_paypal_transaction-2.5.3/source_paypal_transaction/run.py
+-rw-r--r--   0        0        0      523 2024-05-07 10:51:28.000000 airbyte_source_paypal_transaction-2.5.3/source_paypal_transaction/source.py
+-rw-r--r--   0        0        0     3021 2024-05-07 10:51:28.000000 airbyte_source_paypal_transaction-2.5.3/source_paypal_transaction/spec.yaml
+-rw-r--r--   0        0        0    12372 1970-01-01 00:00:00.000000 airbyte_source_paypal_transaction-2.5.3/PKG-INFO
```

### Comparing `airbyte_source_paypal_transaction-2.5.2/README.md` & `airbyte_source_paypal_transaction-2.5.3/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_paypal_transaction-2.5.2/pyproject.toml` & `airbyte_source_paypal_transaction-2.5.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.5.2"
+version = "2.5.3"
 name = "airbyte-source-paypal-transaction"
 description = "Source implementation for Paypal Transaction."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_paypal_transaction" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "^0"
+airbyte-cdk = "0.82.0"
 
 [tool.poetry.scripts]
 source-paypal-transaction = "source_paypal_transaction.run:run"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0"
 pytest-mock = "^3.12"
```

### Comparing `airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/components.py` & `airbyte_source_paypal_transaction-2.5.3/source_paypal_transaction/components.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/source.py` & `airbyte_source_paypal_transaction-2.5.3/source_paypal_transaction/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/spec.yaml` & `airbyte_source_paypal_transaction-2.5.3/source_paypal_transaction/spec.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_paypal_transaction-2.5.2/PKG-INFO` & `airbyte_source_paypal_transaction-2.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-paypal-transaction
-Version: 2.5.2
+Version: 2.5.3
 Summary: Source implementation for Paypal Transaction.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (>=0,<1)
+Requires-Dist: airbyte-cdk (==0.82.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/paypal-transaction
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Paypal-Transaction source connector
 
 This is the repository for the Paypal-Transaction source connector, written in Python.
```

