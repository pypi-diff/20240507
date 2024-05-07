# Comparing `tmp/bpgtask-0.1.1.tar.gz` & `tmp/bpgtask-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpgtask-0.1.1.tar", max compression
+gzip compressed data, was "bpgtask-0.1.2.tar", max compression
```

## Comparing `bpgtask-0.1.1.tar` & `bpgtask-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      648 2024-05-03 09:28:31.173078 bpgtask-0.1.1/README.md
--rw-r--r--   0        0        0      453 2024-05-07 05:34:16.905039 bpgtask-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-19 13:03:34.857002 bpgtask-0.1.1/src/my_package/__init__.py
--rw-r--r--   0        0        0      118 2024-04-20 06:48:04.619105 bpgtask-0.1.1/src/my_package/main.py
--rw-r--r--   0        0        0       49 2024-04-20 06:59:51.512349 bpgtask-0.1.1/src/my_package/my_module.py
--rw-r--r--   0        0        0      326 2024-04-20 07:51:13.017525 bpgtask-0.1.1/src/my_package/testable_code/example.py
--rw-r--r--   0        0        0     1121 1970-01-01 00:00:00.000000 bpgtask-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      648 2024-05-03 09:28:31.173078 bpgtask-0.1.2/README.md
+-rw-r--r--   0        0        0      482 2024-05-07 05:51:35.957537 bpgtask-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-19 13:03:34.857002 bpgtask-0.1.2/src/my_package/__init__.py
+-rw-r--r--   0        0        0      118 2024-04-20 06:48:04.619105 bpgtask-0.1.2/src/my_package/main.py
+-rw-r--r--   0        0        0       49 2024-04-20 06:59:51.512349 bpgtask-0.1.2/src/my_package/my_module.py
+-rw-r--r--   0        0        0      326 2024-04-20 07:51:13.017525 bpgtask-0.1.2/src/my_package/testable_code/example.py
+-rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 bpgtask-0.1.2/PKG-INFO
```

### Comparing `bpgtask-0.1.1/README.md` & `bpgtask-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `bpgtask-0.1.1/PKG-INFO` & `bpgtask-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: bpgtask
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Yu Chang
 Author-email: yu.chang@rokt.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.12,<3.13
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: flytekit (>=1.11.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Install poetry
 python -m pip install poetry
```

