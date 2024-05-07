# Comparing `tmp/beanhub_import-0.0.7.tar.gz` & `tmp/beanhub_import-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanhub_import-0.0.7.tar", max compression
+gzip compressed data, was "beanhub_import-0.0.8.tar", max compression
```

## Comparing `beanhub_import-0.0.7.tar` & `beanhub_import-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2024-05-06 06:38:21.463721 beanhub_import-0.0.7/LICENSE
--rw-r--r--   0        0        0      174 2024-05-06 06:38:21.463721 beanhub_import-0.0.7/README.md
--rw-r--r--   0        0        0        0 2024-05-06 06:38:21.463721 beanhub_import-0.0.7/beanhub_import/__init__.py
--rw-r--r--   0        0        0       28 2024-05-06 06:38:21.463721 beanhub_import-0.0.7/beanhub_import/constants.py
--rw-r--r--   0        0        0     3583 2024-05-06 06:38:21.463721 beanhub_import-0.0.7/beanhub_import/data_types.py
--rw-r--r--   0        0        0     6767 2024-05-06 06:38:21.463721 beanhub_import-0.0.7/beanhub_import/post_processor.py
--rw-r--r--   0        0        0     8229 2024-05-06 06:38:21.463721 beanhub_import-0.0.7/beanhub_import/processor.py
--rw-r--r--   0        0        0      725 2024-05-06 06:38:21.463721 beanhub_import-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 beanhub_import-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-06 06:43:51.394695 beanhub_import-0.0.8/LICENSE
+-rw-r--r--   0        0        0      174 2024-05-06 06:43:51.394695 beanhub_import-0.0.8/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 06:43:51.394695 beanhub_import-0.0.8/beanhub_import/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-06 06:43:51.394695 beanhub_import-0.0.8/beanhub_import/constants.py
+-rw-r--r--   0        0        0     3633 2024-05-06 06:43:51.394695 beanhub_import-0.0.8/beanhub_import/data_types.py
+-rw-r--r--   0        0        0     6767 2024-05-06 06:43:51.394695 beanhub_import-0.0.8/beanhub_import/post_processor.py
+-rw-r--r--   0        0        0     8666 2024-05-06 06:43:51.394695 beanhub_import-0.0.8/beanhub_import/processor.py
+-rw-r--r--   0        0        0      725 2024-05-06 06:43:51.394695 beanhub_import-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 beanhub_import-0.0.8/PKG-INFO
```

### Comparing `beanhub_import-0.0.7/LICENSE` & `beanhub_import-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.0.7/beanhub_import/data_types.py` & `beanhub_import-0.0.8/beanhub_import/data_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,26 +105,27 @@
     narration: str
     payee: str | None = None
     postings: list[GeneratedPosting]
 
 
 class ActionAddTxn(ImportBaseModel):
     type: typing.Literal[ActionType.add_txn] = pydantic.Field(ActionType.add_txn)
-    file: str
+    file: str | None = None
     txn: TransactionTemplate
 
 
 Action = ActionAddTxn
 
 
 SimpleFileMatch = str | StrExactMatch | StrRegexMatch
 
 
 class InputConfigDetails(ImportBaseModel):
     extractor: str | None = None
+    default_file: str | None = None
     prepend_postings: list[PostingTemplate] | None = None
     appending_postings: list[PostingTemplate] | None = None
     default_txn: TransactionTemplate | None = None
 
 
 class InputConfig(ImportBaseModel):
     match: SimpleFileMatch
```

### Comparing `beanhub_import-0.0.7/beanhub_import/post_processor.py` & `beanhub_import-0.0.8/beanhub_import/post_processor.py`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.0.7/beanhub_import/processor.py` & `beanhub_import-0.0.8/beanhub_import/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,16 +157,25 @@
                         account=render_str(posting_template.account),
                         amount=amount,
                         price=price,
                         cost=cost,
                     )
                 )
 
+            output_file = first_non_none(action.file, input_config.default_file)
+            if output_file is None:
+                logger.error(
+                    "Output file not defined when generating transaction with rule %s",
+                    import_rule,
+                )
+                raise ValueError(
+                    f"Output file not defined when generating transaction with rule {import_rule}"
+                )
             yield GeneratedTransaction(
-                file=render_str(action.file),
+                file=render_str(output_file),
                 postings=generated_postings,
                 **{key: render_str(value) for key, value in template_values.items()},
             )
         break
     logger.debug(
         "No match found for transaction %s at %s:%s", txn, txn.file, txn.lineno
     )
```

### Comparing `beanhub_import-0.0.7/pyproject.toml` & `beanhub_import-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beanhub-import"
-version = "0.0.7"
+version = "0.0.8"
 description = "The simple library for import extracted transactions provided by beanhub-extract and generate corresponding Beancount transactions based on predefined rules"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `beanhub_import-0.0.7/PKG-INFO` & `beanhub_import-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beanhub-import
-Version: 0.0.7
+Version: 0.0.8
 Summary: The simple library for import extracted transactions provided by beanhub-extract and generate corresponding Beancount transactions based on predefined rules
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

