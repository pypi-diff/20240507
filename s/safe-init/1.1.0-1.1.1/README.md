# Comparing `tmp/safe_init-1.1.0.tar.gz` & `tmp/safe_init-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe_init-1.1.0.tar", max compression
+gzip compressed data, was "safe_init-1.1.1.tar", max compression
```

## Comparing `safe_init-1.1.0.tar` & `safe_init-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1063 2024-05-07 06:00:23.823182 safe_init-1.1.0/LICENSE
--rw-r--r--   0        0        0    14385 2024-05-07 06:00:23.823182 safe_init-1.1.0/README.md
--rw-r--r--   0        0        0     3226 2024-05-07 06:00:23.835182 safe_init-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      736 2024-05-07 06:00:23.835182 safe_init-1.1.0/safe_init/__init__.py
--rw-r--r--   0        0        0     7429 2024-05-07 06:00:23.835182 safe_init-1.1.0/safe_init/decorator.py
--rw-r--r--   0        0        0     4240 2024-05-07 06:00:23.835182 safe_init-1.1.0/safe_init/dlq.py
--rw-r--r--   0        0        0      751 2024-05-07 06:00:23.835182 safe_init-1.1.0/safe_init/errors.py
--rw-r--r--   0        0        0     5810 2024-05-07 06:00:23.835182 safe_init-1.1.0/safe_init/handler.py
--rw-r--r--   0        0        0        0 2024-05-07 06:00:23.835182 safe_init-1.1.0/safe_init/py.typed
--rw-r--r--   0        0        0     3909 2024-05-07 06:00:23.835182 safe_init-1.1.0/safe_init/safe_logging.py
--rw-r--r--   0        0        0     5832 2024-05-07 06:00:23.839182 safe_init-1.1.0/safe_init/secrets.py
--rw-r--r--   0        0        0     2551 2024-05-07 06:00:23.839182 safe_init-1.1.0/safe_init/sentry.py
--rw-r--r--   0        0        0     5621 2024-05-07 06:00:23.839182 safe_init-1.1.0/safe_init/slack.py
--rw-r--r--   0        0        0     6334 2024-05-07 06:00:23.839182 safe_init-1.1.0/safe_init/timeout.py
--rw-r--r--   0        0        0     3918 2024-05-07 06:00:23.839182 safe_init-1.1.0/safe_init/tracer.py
--rw-r--r--   0        0        0     3949 2024-05-07 06:00:23.839182 safe_init-1.1.0/safe_init/utils.py
--rw-r--r--   0        0        0    15904 1970-01-01 00:00:00.000000 safe_init-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-07 10:37:58.387028 safe_init-1.1.1/LICENSE
+-rw-r--r--   0        0        0    14385 2024-05-07 10:37:58.387028 safe_init-1.1.1/README.md
+-rw-r--r--   0        0        0     3226 2024-05-07 10:37:58.399028 safe_init-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      736 2024-05-07 10:37:58.399028 safe_init-1.1.1/safe_init/__init__.py
+-rw-r--r--   0        0        0     7429 2024-05-07 10:37:58.399028 safe_init-1.1.1/safe_init/decorator.py
+-rw-r--r--   0        0        0     4240 2024-05-07 10:37:58.399028 safe_init-1.1.1/safe_init/dlq.py
+-rw-r--r--   0        0        0      751 2024-05-07 10:37:58.399028 safe_init-1.1.1/safe_init/errors.py
+-rw-r--r--   0        0        0     5810 2024-05-07 10:37:58.399028 safe_init-1.1.1/safe_init/handler.py
+-rw-r--r--   0        0        0        0 2024-05-07 10:37:58.399028 safe_init-1.1.1/safe_init/py.typed
+-rw-r--r--   0        0        0     3909 2024-05-07 10:37:58.399028 safe_init-1.1.1/safe_init/safe_logging.py
+-rw-r--r--   0        0        0     5832 2024-05-07 10:37:58.399028 safe_init-1.1.1/safe_init/secrets.py
+-rw-r--r--   0        0        0     2551 2024-05-07 10:37:58.399028 safe_init-1.1.1/safe_init/sentry.py
+-rw-r--r--   0        0        0     5621 2024-05-07 10:37:58.399028 safe_init-1.1.1/safe_init/slack.py
+-rw-r--r--   0        0        0     6334 2024-05-07 10:37:58.399028 safe_init-1.1.1/safe_init/timeout.py
+-rw-r--r--   0        0        0     3918 2024-05-07 10:37:58.399028 safe_init-1.1.1/safe_init/tracer.py
+-rw-r--r--   0        0        0     3949 2024-05-07 10:37:58.399028 safe_init-1.1.1/safe_init/utils.py
+-rw-r--r--   0        0        0    15904 1970-01-01 00:00:00.000000 safe_init-1.1.1/PKG-INFO
```

### Comparing `safe_init-1.1.0/LICENSE` & `safe_init-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `safe_init-1.1.0/README.md` & `safe_init-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `safe_init-1.1.0/pyproject.toml` & `safe_init-1.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "safe-init"
-version = "1.1.0"
+version = "1.1.1"
 description = "Safe Init is a Python library that enhances AWS Lambda functions with advanced error handling, logging, monitoring, and resilience features, providing comprehensive observability and reliability for serverless applications."
 license = "MIT"
 authors = ["Maciej Wilczyński <maciej@lupine.software>"]
 repository = "https://github.com/kalepa/safe-init"
 readme = "README.md"
 packages = [{ include = "safe_init" }]
 include = ["safe_init/py.typed"]
```

### Comparing `safe_init-1.1.0/safe_init/__init__.py` & `safe_init-1.1.1/safe_init/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any
 
-__VERSION__ = "1.1.0"
+__VERSION__ = "1.1.1"
 
 _wrapped_handler = None
 
 
 class LazyHandler:
     @staticmethod
     def _init_handler() -> None:
```

### Comparing `safe_init-1.1.0/safe_init/decorator.py` & `safe_init-1.1.1/safe_init/decorator.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.1.0/safe_init/dlq.py` & `safe_init-1.1.1/safe_init/dlq.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.1.0/safe_init/errors.py` & `safe_init-1.1.1/safe_init/errors.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.1.0/safe_init/handler.py` & `safe_init-1.1.1/safe_init/handler.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.1.0/safe_init/safe_logging.py` & `safe_init-1.1.1/safe_init/safe_logging.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.1.0/safe_init/secrets.py` & `safe_init-1.1.1/safe_init/secrets.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.1.0/safe_init/sentry.py` & `safe_init-1.1.1/safe_init/sentry.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.1.0/safe_init/slack.py` & `safe_init-1.1.1/safe_init/slack.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.1.0/safe_init/timeout.py` & `safe_init-1.1.1/safe_init/timeout.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.1.0/safe_init/tracer.py` & `safe_init-1.1.1/safe_init/tracer.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.1.0/safe_init/utils.py` & `safe_init-1.1.1/safe_init/utils.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.1.0/PKG-INFO` & `safe_init-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-init
-Version: 1.1.0
+Version: 1.1.1
 Summary: Safe Init is a Python library that enhances AWS Lambda functions with advanced error handling, logging, monitoring, and resilience features, providing comprehensive observability and reliability for serverless applications.
 Home-page: https://github.com/kalepa/safe-init
 License: MIT
 Author: Maciej Wilczyński
 Author-email: maciej@lupine.software
 Requires-Python: >=3.11,<3.12
 Classifier: Development Status :: 5 - Production/Stable
```

