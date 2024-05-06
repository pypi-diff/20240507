# Comparing `tmp/galileo_protect-0.6.0.tar.gz` & `tmp/galileo_protect-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galileo_protect-0.6.0.tar", max compression
+gzip compressed data, was "galileo_protect-0.6.1.tar", max compression
```

## Comparing `galileo_protect-0.6.0.tar` & `galileo_protect-0.6.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    10946 2024-04-30 02:12:57.377982 galileo_protect-0.6.0/LICENSE
--rw-r--r--   0        0        0      118 2024-04-30 02:12:57.377982 galileo_protect-0.6.0/README.md
--rw-r--r--   0        0        0     2583 2024-04-30 02:12:58.273980 galileo_protect-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      431 2024-04-30 02:12:58.273980 galileo_protect-0.6.0/src/galileo_protect/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 02:12:57.377982 galileo_protect-0.6.0/src/galileo_protect/constants/__init__.py
--rw-r--r--   0        0        0       80 2024-04-30 02:12:57.377982 galileo_protect-0.6.0/src/galileo_protect/constants/invoke.py
--rw-r--r--   0        0        0      324 2024-04-30 02:12:57.377982 galileo_protect-0.6.0/src/galileo_protect/constants/routes.py
--rw-r--r--   0        0        0        0 2024-04-30 02:12:57.377982 galileo_protect-0.6.0/src/galileo_protect/helpers/__init__.py
--rw-r--r--   0        0        0      530 2024-04-30 02:12:57.377982 galileo_protect-0.6.0/src/galileo_protect/helpers/config.py
--rw-r--r--   0        0        0     2088 2024-04-30 02:12:57.377982 galileo_protect-0.6.0/src/galileo_protect/invoke.py
--rw-r--r--   0        0        0      638 2024-04-30 02:12:57.377982 galileo_protect-0.6.0/src/galileo_protect/project.py
--rw-r--r--   0        0        0      665 2024-04-30 02:12:57.381982 galileo_protect-0.6.0/src/galileo_protect/schemas/__init__.py
--rw-r--r--   0        0        0      212 2024-04-30 02:12:57.381982 galileo_protect-0.6.0/src/galileo_protect/schemas/invoke.py
--rw-r--r--   0        0        0      308 2024-04-30 02:12:57.381982 galileo_protect-0.6.0/src/galileo_protect/schemas/rule.py
--rw-r--r--   0        0        0      124 2024-04-30 02:12:57.381982 galileo_protect-0.6.0/src/galileo_protect/schemas/stage.py
--rw-r--r--   0        0        0     3529 2024-04-30 02:12:57.381982 galileo_protect-0.6.0/src/galileo_protect/stage.py
--rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 galileo_protect-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    10946 2024-05-06 22:55:32.556611 galileo_protect-0.6.1/LICENSE
+-rw-r--r--   0        0        0      118 2024-05-06 22:55:32.556611 galileo_protect-0.6.1/README.md
+-rw-r--r--   0        0        0     2583 2024-05-06 22:55:33.532610 galileo_protect-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      508 2024-05-06 22:55:33.532610 galileo_protect-0.6.1/src/galileo_protect/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 22:55:32.560611 galileo_protect-0.6.1/src/galileo_protect/constants/__init__.py
+-rw-r--r--   0        0        0       80 2024-05-06 22:55:32.560611 galileo_protect-0.6.1/src/galileo_protect/constants/invoke.py
+-rw-r--r--   0        0        0      324 2024-05-06 22:55:32.560611 galileo_protect-0.6.1/src/galileo_protect/constants/routes.py
+-rw-r--r--   0        0        0        0 2024-05-06 22:55:32.560611 galileo_protect-0.6.1/src/galileo_protect/helpers/__init__.py
+-rw-r--r--   0        0        0      530 2024-05-06 22:55:32.560611 galileo_protect-0.6.1/src/galileo_protect/helpers/config.py
+-rw-r--r--   0        0        0     2088 2024-05-06 22:55:32.560611 galileo_protect-0.6.1/src/galileo_protect/invoke.py
+-rw-r--r--   0        0        0      638 2024-05-06 22:55:32.560611 galileo_protect-0.6.1/src/galileo_protect/project.py
+-rw-r--r--   0        0        0      665 2024-05-06 22:55:32.560611 galileo_protect-0.6.1/src/galileo_protect/schemas/__init__.py
+-rw-r--r--   0        0        0      212 2024-05-06 22:55:32.560611 galileo_protect-0.6.1/src/galileo_protect/schemas/invoke.py
+-rw-r--r--   0        0        0      308 2024-05-06 22:55:32.560611 galileo_protect-0.6.1/src/galileo_protect/schemas/rule.py
+-rw-r--r--   0        0        0      124 2024-05-06 22:55:32.560611 galileo_protect-0.6.1/src/galileo_protect/schemas/stage.py
+-rw-r--r--   0        0        0     3529 2024-05-06 22:55:32.560611 galileo_protect-0.6.1/src/galileo_protect/stage.py
+-rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 galileo_protect-0.6.1/PKG-INFO
```

### Comparing `galileo_protect-0.6.0/LICENSE` & `galileo_protect-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.6.0/pyproject.toml` & `galileo_protect-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "galileo-protect"
-version = "0.6.0"
+version = "0.6.1"
 description = "🛡️ Secure your Generative AI applications with Galileo Protect!"
 authors = ["Galileo Technologies Inc. <team@rungalileo.io>"]
 readme = "README.md"
 packages = [{include = "galileo_protect", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1,<3.13"
-galileo-core = "^0.12.0"
+galileo-core = "^0.13.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.1"
 coverage = "^7.3.4"
 pytest-cov = "^5.0.0"
 pytest-xdist = "^3.5.0"
```

### Comparing `galileo_protect-0.6.0/src/galileo_protect/helpers/config.py` & `galileo_protect-0.6.1/src/galileo_protect/helpers/config.py`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.6.0/src/galileo_protect/invoke.py` & `galileo_protect-0.6.1/src/galileo_protect/invoke.py`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.6.0/src/galileo_protect/project.py` & `galileo_protect-0.6.1/src/galileo_protect/project.py`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.6.0/src/galileo_protect/schemas/__init__.py` & `galileo_protect-0.6.1/src/galileo_protect/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.6.0/src/galileo_protect/stage.py` & `galileo_protect-0.6.1/src/galileo_protect/stage.py`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.6.0/PKG-INFO` & `galileo_protect-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: galileo-protect
-Version: 0.6.0
+Version: 0.6.1
 Summary: 🛡️ Secure your Generative AI applications with Galileo Protect!
 Author: Galileo Technologies Inc.
 Author-email: team@rungalileo.io
 Requires-Python: >=3.8.1,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: galileo-core (>=0.12.0,<0.13.0)
+Requires-Dist: galileo-core (>=0.13.0,<0.14.0)
 Description-Content-Type: text/markdown
 
 # galileo-protect
 
 🛡️ Secure your Generative AI applications with [Galileo Protect](https://www.rungalileo.io/).
```

