# Comparing `tmp/bpgtask-0.1.2.tar.gz` & `tmp/bpgtask-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpgtask-0.1.2.tar", max compression
+gzip compressed data, was "bpgtask-0.1.3.tar", max compression
```

## Comparing `bpgtask-0.1.2.tar` & `bpgtask-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      648 2024-05-03 09:28:31.173078 bpgtask-0.1.2/README.md
--rw-r--r--   0        0        0      482 2024-05-07 05:51:35.957537 bpgtask-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-19 13:03:34.857002 bpgtask-0.1.2/src/my_package/__init__.py
--rw-r--r--   0        0        0      118 2024-04-20 06:48:04.619105 bpgtask-0.1.2/src/my_package/main.py
--rw-r--r--   0        0        0       49 2024-04-20 06:59:51.512349 bpgtask-0.1.2/src/my_package/my_module.py
--rw-r--r--   0        0        0      326 2024-04-20 07:51:13.017525 bpgtask-0.1.2/src/my_package/testable_code/example.py
--rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 bpgtask-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      707 2024-05-07 05:53:05.436223 bpgtask-0.1.3/README.md
+-rw-r--r--   0        0        0      482 2024-05-07 05:59:20.576586 bpgtask-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-19 13:03:34.857002 bpgtask-0.1.3/src/my_package/__init__.py
+-rw-r--r--   0        0        0     3328 2024-05-07 05:55:35.971708 bpgtask-0.1.3/src/my_package/bpgtask.py
+-rw-r--r--   0        0        0      118 2024-04-20 06:48:04.619105 bpgtask-0.1.3/src/my_package/main.py
+-rw-r--r--   0        0        0       49 2024-04-20 06:59:51.512349 bpgtask-0.1.3/src/my_package/my_module.py
+-rw-r--r--   0        0        0      326 2024-04-20 07:51:13.017525 bpgtask-0.1.3/src/my_package/testable_code/example.py
+-rw-r--r--   0        0        0     1072 1970-01-01 00:00:00.000000 bpgtask-0.1.3/PKG-INFO
```

### Comparing `bpgtask-0.1.2/README.md` & `bpgtask-0.1.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -29,14 +29,17 @@
 
 # run the project
 poetry run python src/my_package/main.py
 
 # build the project
 poetry build
 
+# publish the project (with build)
+poetry publish --build
+
 
 # FAQ
 - What is Poetry - dependency management and packaging tool for Python
 
 - poetry.lock should be committed to the repository
```

### Comparing `bpgtask-0.1.2/PKG-INFO` & `bpgtask-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpgtask
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Yu Chang
 Author-email: yu.chang@rokt.com
 Requires-Python: >=3.12,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: flytekit (>=1.11.0,<2.0.0)
@@ -42,14 +42,17 @@
 
 # run the project
 poetry run python src/my_package/main.py
 
 # build the project
 poetry build
 
+# publish the project (with build)
+poetry publish --build
+
 
 # FAQ
 - What is Poetry - dependency management and packaging tool for Python
 
 - poetry.lock should be committed to the repository
```

