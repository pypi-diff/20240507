# Comparing `tmp/amortization-2.3.0.tar.gz` & `tmp/amortization-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amortization-2.3.0.tar", max compression
+gzip compressed data, was "amortization-2.4.0.tar", max compression
```

## Comparing `amortization-2.3.0.tar` & `amortization-2.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-07-06 22:22:56.640949 amortization-2.3.0/LICENSE
--rw-r--r--   0        0        0     6382 2023-07-06 22:22:56.644949 amortization-2.3.0/README.md
--rw-r--r--   0        0        0        0 2023-07-06 22:22:56.644949 amortization-2.3.0/amortization/__init__.py
--rw-r--r--   0        0        0     3523 2023-07-06 22:22:56.644949 amortization-2.3.0/amortization/amortize.py
--rw-r--r--   0        0        0      850 2023-07-06 22:22:56.644949 amortization-2.3.0/amortization/amount.py
--rw-r--r--   0        0        0      195 2023-07-06 22:22:56.644949 amortization-2.3.0/amortization/enums.py
--rw-r--r--   0        0        0      893 2023-07-06 22:22:56.644949 amortization-2.3.0/amortization/period.py
--rw-r--r--   0        0        0     1251 2023-07-06 22:22:56.644949 amortization-2.3.0/amortization/schedule.py
--rw-r--r--   0        0        0     2160 2023-07-06 22:22:56.644949 amortization-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     7553 1970-01-01 00:00:00.000000 amortization-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-07 20:29:36.534939 amortization-2.4.0/LICENSE
+-rw-r--r--   0        0        0     6382 2024-05-07 20:29:36.534939 amortization-2.4.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-07 20:29:36.534939 amortization-2.4.0/amortization/__init__.py
+-rw-r--r--   0        0        0     3523 2024-05-07 20:29:36.534939 amortization-2.4.0/amortization/amortize.py
+-rw-r--r--   0        0        0      850 2024-05-07 20:29:36.534939 amortization-2.4.0/amortization/amount.py
+-rw-r--r--   0        0        0      216 2024-05-07 20:29:36.534939 amortization-2.4.0/amortization/enums.py
+-rw-r--r--   0        0        0      893 2024-05-07 20:29:36.534939 amortization-2.4.0/amortization/period.py
+-rw-r--r--   0        0        0     1251 2024-05-07 20:29:36.534939 amortization-2.4.0/amortization/schedule.py
+-rw-r--r--   0        0        0     2161 2024-05-07 20:29:36.534939 amortization-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7604 1970-01-01 00:00:00.000000 amortization-2.4.0/PKG-INFO
```

### Comparing `amortization-2.3.0/LICENSE` & `amortization-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `amortization-2.3.0/README.md` & `amortization-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `amortization-2.3.0/amortization/amortize.py` & `amortization-2.4.0/amortization/amortize.py`

 * *Files identical despite different names*

### Comparing `amortization-2.3.0/amortization/amount.py` & `amortization-2.4.0/amortization/amount.py`

 * *Files identical despite different names*

### Comparing `amortization-2.3.0/amortization/period.py` & `amortization-2.4.0/amortization/period.py`

 * *Files identical despite different names*

### Comparing `amortization-2.3.0/amortization/schedule.py` & `amortization-2.4.0/amortization/schedule.py`

 * *Files identical despite different names*

### Comparing `amortization-2.3.0/pyproject.toml` & `amortization-2.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "amortization"
-version = "2.3.0"
+version = "2.4.0"
 repository = "https://github.com/roniemartinez/amortization"
 description = "Python library for calculating amortizations and generating amortization schedules"
 authors = ["Ronie Martinez <ronmarti18@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = [
     "amortization"
@@ -31,20 +31,20 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 tabulate = "^0.9.0"
 
 [tool.poetry.dev-dependencies]
 autoflake = "^1.7.8"
-black = "^23.3"
-isort = "^5.11.5"
-mypy = "^1.4"
+black = "^24.4"
+isort = "^5.13.2"
+mypy = "^1.10"
 pyproject-flake8 = "^5.0.4"
-pytest = "^7.4.0"
-pytest-cov = "^4.1.0"
+pytest = "^8.2.0"
+pytest-cov = "^5.0.0"
 types-tabulate = "^0.9.0"
 
 [tool.isort]
 line_length = 120
 multi_line_output = 3
 force_grid_wrap = 0
 use_parentheses = true
```

### Comparing `amortization-2.3.0/PKG-INFO` & `amortization-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: amortization
-Version: 2.3.0
+Version: 2.4.0
 Summary: Python library for calculating amortizations and generating amortization schedules
 Home-page: https://github.com/roniemartinez/amortization
 License: MIT
 Keywords: amortization
 Author: Ronie Martinez
 Author-email: ronmarti18@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Donate, https://www.buymeacoffee.com/roniemartinez
 Project-URL: Repository, https://github.com/roniemartinez/amortization
```

