# Comparing `tmp/airbyte_source_harvest-1.0.0.tar.gz` & `tmp/airbyte_source_harvest-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_harvest-1.0.0.tar", max compression
+gzip compressed data, was "airbyte_source_harvest-1.0.1.tar", max compression
```

## Comparing `airbyte_source_harvest-1.0.0.tar` & `airbyte_source_harvest-1.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     4519 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/README.md
--rw-r--r--   0        0        0      767 2024-04-15 16:09:38.876249 airbyte_source_harvest-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1136 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/__init__.py
--rw-r--r--   0        0        0     4047 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/config_migrations.py
--rw-r--r--   0        0        0    75102 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/manifest.yaml
--rw-r--r--   0        0        0      331 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/run.py
--rw-r--r--   0        0        0      604 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/billable_rates.json
--rw-r--r--   0        0        0      624 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/clients.json
--rw-r--r--   0        0        0     1174 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/company.json
--rw-r--r--   0        0        0      955 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/contacts.json
--rw-r--r--   0        0        0      604 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/cost_rates.json
--rw-r--r--   0        0        0      386 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/estimate_item_categories.json
--rw-r--r--   0        0        0     1151 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/estimate_messages.json
--rw-r--r--   0        0        0     1930 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/estimates.json
--rw-r--r--   0        0        0      565 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/expense_categories.json
--rw-r--r--   0        0        0     3377 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/expenses.json
--rw-r--r--   0        0        0      533 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/expenses_categories.json
--rw-r--r--   0        0        0      513 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/expenses_clients.json
--rw-r--r--   0        0        0      636 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/expenses_projects.json
--rw-r--r--   0        0        0      573 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/expenses_team.json
--rw-r--r--   0        0        0      516 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/invoice_item_categories.json
--rw-r--r--   0        0        0     1458 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/invoice_messages.json
--rw-r--r--   0        0        0     1080 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/invoice_payments.json
--rw-r--r--   0        0        0     3573 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/invoices.json
--rw-r--r--   0        0        0     2233 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/project_assignments.json
--rw-r--r--   0        0        0      822 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/project_budget.json
--rw-r--r--   0        0        0     1932 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/projects.json
--rw-r--r--   0        0        0      495 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/roles.json
--rw-r--r--   0        0        0     1067 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/task_assignments.json
--rw-r--r--   0        0        0      646 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/tasks.json
--rw-r--r--   0        0        0      576 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/time_clients.json
--rw-r--r--   0        0        0     3977 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/time_entries.json
--rw-r--r--   0        0        0      699 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/time_projects.json
--rw-r--r--   0        0        0      572 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/time_tasks.json
--rw-r--r--   0        0        0      636 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/time_team.json
--rw-r--r--   0        0        0      772 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/uninvoiced.json
--rw-r--r--   0        0        0     1145 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/user_assignments.json
--rw-r--r--   0        0        0     1678 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/users.json
--rw-r--r--   0        0        0      476 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/source.py
--rw-r--r--   0        0        0     5224 1970-01-01 00:00:00.000000 airbyte_source_harvest-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4519 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/README.md
+-rw-r--r--   0        0        0      771 2024-05-07 12:24:49.166843 airbyte_source_harvest-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1136 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/__init__.py
+-rw-r--r--   0        0        0     4047 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/config_migrations.py
+-rw-r--r--   0        0        0    75102 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/manifest.yaml
+-rw-r--r--   0        0        0      331 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/run.py
+-rw-r--r--   0        0        0     1117 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/billable_rates.json
+-rw-r--r--   0        0        0     1147 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/clients.json
+-rw-r--r--   0        0        0     2466 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/company.json
+-rw-r--r--   0        0        0     1701 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/contacts.json
+-rw-r--r--   0        0        0     1219 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/cost_rates.json
+-rw-r--r--   0        0        0      707 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/estimate_item_categories.json
+-rw-r--r--   0        0        0     2168 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/estimate_messages.json
+-rw-r--r--   0        0        0     3938 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/estimates.json
+-rw-r--r--   0        0        0     1095 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/expense_categories.json
+-rw-r--r--   0        0        0     6480 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/expenses.json
+-rw-r--r--   0        0        0      987 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/expenses_categories.json
+-rw-r--r--   0        0        0     1019 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/expenses_clients.json
+-rw-r--r--   0        0        0     1277 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/expenses_projects.json
+-rw-r--r--   0        0        0     1081 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/expenses_team.json
+-rw-r--r--   0        0        0      998 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/invoice_item_categories.json
+-rw-r--r--   0        0        0     2793 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/invoice_messages.json
+-rw-r--r--   0        0        0     2139 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/invoice_payments.json
+-rw-r--r--   0        0        0     6645 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/invoices.json
+-rw-r--r--   0        0        0     4278 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/project_assignments.json
+-rw-r--r--   0        0        0     1604 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/project_budget.json
+-rw-r--r--   0        0        0     3893 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/projects.json
+-rw-r--r--   0        0        0      891 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/roles.json
+-rw-r--r--   0        0        0     2023 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/task_assignments.json
+-rw-r--r--   0        0        0     1174 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/tasks.json
+-rw-r--r--   0        0        0     1440 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/time_clients.json
+-rw-r--r--   0        0        0     7743 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/time_entries.json
+-rw-r--r--   0        0        0     1440 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/time_projects.json
+-rw-r--r--   0        0        0     1165 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/time_tasks.json
+-rw-r--r--   0        0        0     1227 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/time_team.json
+-rw-r--r--   0        0        0     1503 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/uninvoiced.json
+-rw-r--r--   0        0        0     2252 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/user_assignments.json
+-rw-r--r--   0        0        0     3071 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/schemas/users.json
+-rw-r--r--   0        0        0      476 2024-05-07 10:23:34.000000 airbyte_source_harvest-1.0.1/source_harvest/source.py
+-rw-r--r--   0        0        0     5226 1970-01-01 00:00:00.000000 airbyte_source_harvest-1.0.1/PKG-INFO
```

### Comparing `airbyte_source_harvest-1.0.0/README.md` & `airbyte_source_harvest-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-1.0.0/pyproject.toml` & `airbyte_source_harvest-1.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "1.0.0"
+version = "1.0.1"
 name = "airbyte-source-harvest"
 description = "Source implementation for Harvest."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_harvest" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "^0"
+airbyte-cdk = "0.80.0"
 
 [tool.poetry.scripts]
 source-harvest = "source_harvest.run:run"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "^1.11.0"
 pytest-mock = "^3.6.1"
```

### Comparing `airbyte_source_harvest-1.0.0/source_harvest/__init__.py` & `airbyte_source_harvest-1.0.1/source_harvest/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-1.0.0/source_harvest/config_migrations.py` & `airbyte_source_harvest-1.0.1/source_harvest/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-1.0.0/source_harvest/manifest.yaml` & `airbyte_source_harvest-1.0.1/source_harvest/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-1.0.0/source_harvest/schemas/clients.json` & `airbyte_source_harvest-1.0.1/source_harvest/schemas/estimate_item_categories.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8993055555555555%*

 * *Differences: {"'properties'": "{'id': {'description': 'The unique identifier for the estimate item category.'}, "*

 * *                 "'name': {'description': 'The name of the estimate item category.'}, "*

 * *                 "'created_at': {'description': 'The date and time when the estimate item category "*

 * *                 "was created.'}, 'updated_at': {'description': 'The date and time when the "*

 * *                 "estimate item category was last updated.'}, delete: ['is_active', 'address', "*

 * *                 "'statement_ke […]*

```diff
@@ -1,54 +1,34 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
-        "address": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "created_at": {
+            "description": "The date and time when the estimate item category was created.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "currency": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "id": {
+            "description": "The unique identifier for the estimate item category.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "is_active": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
         "name": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "statement_key": {
+            "description": "The name of the estimate item category.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "updated_at": {
+            "description": "The date and time when the estimate item category was last updated.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
```

### Comparing `airbyte_source_harvest-1.0.0/source_harvest/schemas/contacts.json` & `airbyte_source_harvest-1.0.1/source_harvest/schemas/expense_categories.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8601851851851853%*

 * *Differences: {"'properties'": "{'id': {'description': 'The unique identifier for the expense category.'}, "*

 * *                 "'created_at': {'description': 'The date and time when the expense category was "*

 * *                 "created.'}, 'updated_at': {'description': 'The date and time when the expense "*

 * *                 "category was last updated.'}, 'name': OrderedDict([('description', 'The name of "*

 * *                 "the expense category.'), ('type', ['null', 'string'])]), 'unit_name': "*

 * *                 "OrderedDict( […]*

```diff
@@ -1,86 +1,55 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
-        "client": {
-            "properties": {
-                "id": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "name": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
-            "type": [
-                "null",
-                "object"
-            ]
-        },
         "created_at": {
+            "description": "The date and time when the expense category was created.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "email": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "fax": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "first_name": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "id": {
+            "description": "The unique identifier for the expense category.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "last_name": {
+        "is_active": {
+            "description": "Indicates whether the expense category is currently active or not.",
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "phone_mobile": {
+        "name": {
+            "description": "The name of the expense category.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "phone_office": {
+        "unit_name": {
+            "description": "The unit of measurement for the expense category.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "title": {
+        "unit_price": {
+            "description": "The price per unit of the expense category.",
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
         "updated_at": {
+            "description": "The date and time when the expense category was last updated.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
```

### Comparing `airbyte_source_harvest-1.0.0/source_harvest/schemas/estimate_messages.json` & `airbyte_source_harvest-1.0.1/source_harvest/schemas/invoice_item_categories.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8585069444444445%*

 * *Differences: {"'properties'": "{'id': {'description': 'The unique identifier for the invoice item category.'}, "*

 * *                 "'created_at': {'description': 'The date and time when the invoice item category "*

 * *                 "was created.'}, 'updated_at': {'description': 'The date and time when the "*

 * *                 "invoice item category was last updated.'}, 'name': OrderedDict([('description', "*

 * *                 "'The name of the invoice item category.'), ('type', ['null', 'string'])]), "*

 * *                 "'use_ […]*

```diff
@@ -1,100 +1,50 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
-        "body": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "created_at": {
+            "description": "The date and time when the invoice item category was created.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "event_type": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "id": {
+            "description": "The unique identifier for the invoice item category.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "parent_id": {
-            "type": "integer"
-        },
-        "recipients": {
-            "items": {
-                "properties": {
-                    "email": {
-                        "type": [
-                            "string",
-                            "null"
-                        ]
-                    },
-                    "name": {
-                        "type": [
-                            "string",
-                            "null"
-                        ]
-                    }
-                },
-                "type": "object"
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "send_me_a_copy": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "sent_by": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "sent_by_email": {
+        "name": {
+            "description": "The name of the invoice item category.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "sent_from": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "sent_from_email": {
+        "updated_at": {
+            "description": "The date and time when the invoice item category was last updated.",
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "subject": {
+        "use_as_expense": {
+            "description": "Indicates whether the category is used as an expense type.",
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "updated_at": {
-            "format": "date-time",
+        "use_as_service": {
+            "description": "Indicates whether the category is used as a service type.",
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte_source_harvest-1.0.0/source_harvest/schemas/estimates.json` & `airbyte_source_harvest-1.0.1/source_harvest/schemas/company.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('base_uri', OrderedDict([('description', 'The base URI "*

 * *                 "used in constructing URLs for this company.'), ('type', ['null', 'string'])])), "*

 * *                 "('full_domain', OrderedDict([('description', 'The full domain name associated "*

 * *                 "with this company.'), ('type', ['null', 'string'])])), ('name', "*

 * *                 "OrderedDict([('description', 'The name of the company.'), ('type', ['null', "*

 * *                 "'string'])])), (' […]*

```diff
@@ -1,182 +1,125 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
-        "accepted_at": {
+        "approval_required": {
+            "description": "Indicates if approval is required for certain actions.",
             "type": [
                 "null",
-                "string"
-            ]
-        },
-        "amount": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "client": {
-            "properties": {
-                "id": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "name": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
-            "type": [
-                "null",
-                "object"
+                "boolean"
             ]
         },
-        "client_key": {
+        "base_uri": {
+            "description": "The base URI used in constructing URLs for this company.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "created_at": {
-            "format": "date-time",
+        "clock": {
+            "description": "The clock configuration for time tracking.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "creator": {
-            "properties": {
-                "id": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "name": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "currency": {
+        "color_scheme": {
+            "description": "The color scheme used in the user interface.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "declined_at": {
+        "decimal_symbol": {
+            "description": "The symbol used to separate the integer part from the fractional part of a number.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "discount": {
+        "estimate_feature": {
+            "description": "Indicates if the estimate feature is enabled for this company.",
             "type": [
                 "null",
-                "number"
+                "boolean"
             ]
         },
-        "discount_amount": {
+        "expense_feature": {
+            "description": "Indicates if the expense feature is enabled for this company.",
             "type": [
                 "null",
-                "number"
-            ]
-        },
-        "id": {
-            "type": [
-                "null",
-                "integer"
+                "boolean"
             ]
         },
-        "issue_date": {
-            "format": "date",
+        "full_domain": {
+            "description": "The full domain name associated with this company.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "line_items": {
+        "invoice_feature": {
+            "description": "Indicates if the invoice feature is enabled for this company.",
             "type": [
                 "null",
-                "array"
+                "boolean"
             ]
         },
-        "notes": {
+        "is_active": {
+            "description": "Indicates if the company is currently active.",
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "number": {
+        "name": {
+            "description": "The name of the company.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "purchase_order": {
+        "plan_type": {
+            "description": "The type of plan subscribed by the company.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "sent_at": {
-            "format": "date-time",
+        "thousands_separator": {
+            "description": "The symbol used to separate thousands in a number.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "state": {
+        "time_format": {
+            "description": "The format used to display time.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "subject": {
+        "wants_timestamp_timers": {
+            "description": "Indicates if the company wants timestamp timers displayed.",
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "tax": {
+        "week_start_day": {
+            "description": "The day considered the start of the week for this company.",
             "type": [
                 "null",
-                "number"
-            ]
-        },
-        "tax2": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "tax2_amount": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "tax_amount": {
-            "type": [
-                "null",
-                "number"
+                "string"
             ]
         },
-        "updated_at": {
-            "format": "date-time",
+        "weekly_capacity": {
+            "description": "The weekly capacity setting for this company.",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte_source_harvest-1.0.0/source_harvest/schemas/expenses_team.json` & `airbyte_source_harvest-1.0.1/source_harvest/schemas/expenses_team.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'properties'": "{'user_id': {'description': 'The ID of the user associated with the expense'}, "*

 * *                 "'user_name': {'description': 'The name of the user associated with the "*

 * *                 "expense'}, 'is_contractor': {'description': 'Indicates if the user is a "*

 * *                 "contractor'}, 'total_amount': {'description': 'The total amount of the "*

 * *                 "expense'}, 'billable_amount': {'description': 'The amount that can be billed for "*

 * *                 "the expense'}, 'curr […]*

```diff
@@ -1,53 +1,61 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
         "billable_amount": {
+            "description": "The amount that can be billed for the expense",
             "type": [
                 "null",
                 "number"
             ]
         },
         "currency": {
+            "description": "The currency in which the expense is incurred",
             "type": [
                 "null",
                 "string"
             ]
         },
         "from": {
+            "description": "The start date of the expense",
             "type": [
                 "null",
                 "string"
             ]
         },
         "is_contractor": {
+            "description": "Indicates if the user is a contractor",
             "type": [
                 "null",
                 "boolean"
             ]
         },
         "to": {
+            "description": "The end date of the expense",
             "type": [
                 "null",
                 "string"
             ]
         },
         "total_amount": {
+            "description": "The total amount of the expense",
             "type": [
                 "null",
                 "number"
             ]
         },
         "user_id": {
+            "description": "The ID of the user associated with the expense",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "user_name": {
+            "description": "The name of the user associated with the expense",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
     "type": "object"
```

### Comparing `airbyte_source_harvest-1.0.0/source_harvest/schemas/invoice_messages.json` & `airbyte_source_harvest-1.0.1/source_harvest/schemas/estimate_messages.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9258535879629629%*

 * *Differences: {"'properties'": "{'id': {'description': 'The unique identifier for the message.'}, 'parent_id': "*

 * *                 "{'description': 'The identifier of the parent message, if this is a reply.'}, "*

 * *                 "'sent_by': {'description': 'The name of the user who sent the message.'}, "*

 * *                 "'sent_by_email': {'description': 'The email address of the user who sent the "*

 * *                 "message.'}, 'sent_from': {'description': 'The name displayed as the sender.'}, "*

 * *                 "'sent_f […]*

```diff
@@ -1,122 +1,113 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
-        "attach_pdf": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
         "body": {
+            "description": "The main content of the message.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "created_at": {
+            "description": "The date and time when the message was created.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "event_type": {
+            "description": "The type of event associated with the message.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "id": {
+            "description": "The unique identifier for the message.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "include_link_to_client_invoice": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
         "parent_id": {
+            "description": "The identifier of the parent message, if this is a reply.",
             "type": "integer"
         },
         "recipients": {
+            "description": "Details of the recipients of the message.",
             "items": {
                 "properties": {
                     "email": {
-                        "type": "string"
+                        "description": "The email address of a recipient.",
+                        "type": [
+                            "string",
+                            "null"
+                        ]
                     },
                     "name": {
-                        "type": "string"
+                        "description": "The name of a recipient.",
+                        "type": [
+                            "string",
+                            "null"
+                        ]
                     }
                 },
                 "type": "object"
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "reminder": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
         "send_me_a_copy": {
+            "description": "Indicates if the sender requested a copy of the message.",
             "type": [
                 "null",
                 "boolean"
             ]
         },
-        "send_reminder_on": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "sent_by": {
+            "description": "The name of the user who sent the message.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "sent_by_email": {
+            "description": "The email address of the user who sent the message.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "sent_from": {
+            "description": "The name displayed as the sender.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "sent_from_email": {
+            "description": "The email address displayed as the sender.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "subject": {
+            "description": "The subject or title of the message.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "thank_you": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
         "updated_at": {
+            "description": "The date and time when the message was last updated.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
```

### Comparing `airbyte_source_harvest-1.0.0/source_harvest/schemas/projects.json` & `airbyte_source_harvest-1.0.1/source_harvest/schemas/invoice_messages.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8436609686609686%*

 * *Differences: {"'properties'": "{'id': {'description': 'The unique identifier of the invoice message.'}, "*

 * *                 "'created_at': {'description': 'The date and time when the message was "*

 * *                 "created.'}, 'updated_at': {'description': 'The date and time when the message "*

 * *                 'was last updated.\'}, \'parent_id\': OrderedDict([(\'description\', "The ID of '*

 * *                 'the parent message if it\'s a reply or related message."), (\'type\', '*

 * *                 "'integer')]), 'sent_by': […]*

```diff
@@ -1,172 +1,142 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
-        "bill_by": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "budget": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "budget_by": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "budget_is_monthly": {
+        "attach_pdf": {
+            "description": "Indicates if a PDF file is attached to the message.",
             "type": [
                 "null",
                 "boolean"
             ]
         },
-        "client": {
-            "properties": {
-                "currency": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "id": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "name": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "code": {
+        "body": {
+            "description": "The content of the invoice message.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "cost_budget": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "cost_budget_include_expenses": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
         "created_at": {
+            "description": "The date and time when the message was created.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ends_on": {
+        "event_type": {
+            "description": "The type of event associated with the message.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "fee": {
+        "id": {
+            "description": "The unique identifier of the invoice message.",
             "type": [
                 "null",
-                "number"
+                "integer"
             ]
         },
-        "hourly_rate": {
+        "include_link_to_client_invoice": {
+            "description": "Indicates if a link to the client invoice is included.",
             "type": [
                 "null",
-                "number"
+                "boolean"
             ]
         },
-        "id": {
-            "type": [
-                "null",
-                "integer"
-            ]
+        "parent_id": {
+            "description": "The ID of the parent message if it's a reply or related message.",
+            "type": "integer"
         },
-        "is_active": {
+        "recipients": {
+            "description": "List of recipients for the message.",
+            "items": {
+                "properties": {
+                    "email": {
+                        "description": "Email address of the recipient.",
+                        "type": "string"
+                    },
+                    "name": {
+                        "description": "Name of the recipient.",
+                        "type": "string"
+                    }
+                },
+                "type": "object"
+            },
             "type": [
                 "null",
-                "boolean"
+                "array"
             ]
         },
-        "is_billable": {
+        "reminder": {
+            "description": "Indicates if the message is a reminder.",
             "type": [
                 "null",
                 "boolean"
             ]
         },
-        "is_fixed_fee": {
+        "send_me_a_copy": {
+            "description": "Option to send a copy of the message to the sender.",
             "type": [
                 "null",
                 "boolean"
             ]
         },
-        "name": {
+        "send_reminder_on": {
+            "description": "The date to send a reminder for the message.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "notes": {
+        "sent_by": {
+            "description": "The sender of the message.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "notify_when_over_budget": {
+        "sent_by_email": {
+            "description": "Email address of the sender.",
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
-        "over_budget_notification_date": {
-            "format": "date",
+        "sent_from": {
+            "description": "The display name of the sender.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "over_budget_notification_percentage": {
+        "sent_from_email": {
+            "description": "Email address used to send the message.",
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "show_budget_to_all": {
+        "subject": {
+            "description": "The subject of the invoice message.",
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
-        "starts_on": {
-            "format": "date",
+        "thank_you": {
+            "description": "Indicates if the message is a thank you message.",
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
         "updated_at": {
+            "description": "The date and time when the message was last updated.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
```

### Comparing `airbyte_source_harvest-1.0.0/source_harvest/schemas/task_assignments.json` & `airbyte_source_harvest-1.0.1/source_harvest/schemas/roles.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8699494949494949%*

 * *Differences: {"'properties'": "{'id': {'description': 'The unique identifier for the role'}, 'created_at': "*

 * *                 "{'description': 'The date and time when the role was created'}, 'updated_at': "*

 * *                 "{'description': 'The date and time when the role was last updated'}, 'name': "*

 * *                 "OrderedDict([('description', 'The name of the role'), ('type', ['null', "*

 * *                 "'string'])]), 'user_ids': OrderedDict([('description', 'An array of user IDs "*

 * *                 "associated wit […]*

```diff
@@ -1,96 +1,47 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
-        "billable": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "budget": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "created_at": {
+            "description": "The date and time when the role was created",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "hourly_rate": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "id": {
+            "description": "The unique identifier for the role",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "is_active": {
+        "name": {
+            "description": "The name of the role",
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
-        "project": {
-            "properties": {
-                "code": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "id": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "name": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
+        "updated_at": {
+            "description": "The date and time when the role was last updated",
+            "format": "date-time",
             "type": [
                 "null",
-                "object"
+                "string"
             ]
         },
-        "task": {
-            "properties": {
-                "id": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "name": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
+        "user_ids": {
+            "description": "An array of user IDs associated with the role",
+            "items": {
+                "description": "The unique identifier for a user assigned to this role",
+                "type": "integer"
             },
             "type": [
                 "null",
-                "object"
-            ]
-        },
-        "updated_at": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
+                "array"
             ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte_source_harvest-1.0.0/PKG-INFO` & `airbyte_source_harvest-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-harvest
-Version: 1.0.0
+Version: 1.0.1
 Summary: Source implementation for Harvest.
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
+Requires-Dist: airbyte-cdk (==0.80.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/harvest
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Harvest source connector
```

