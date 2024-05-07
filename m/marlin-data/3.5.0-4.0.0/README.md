# Comparing `tmp/marlin_data-3.5.0.tar.gz` & `tmp/marlin_data-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marlin_data-3.5.0.tar", last modified: Fri Mar 15 08:16:07 2024, max compression
+gzip compressed data, was "marlin_data-4.0.0.tar", last modified: Tue May  7 13:59:02 2024, max compression
```

## Comparing `marlin_data-3.5.0.tar` & `marlin_data-4.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:16:07.099417 marlin_data-3.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:16:07.087417 marlin_data-3.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:16:07.099417 marlin_data-3.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-15 08:15:51.000000 marlin_data-3.5.0/.github/workflows/python-app.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-15 08:15:51.000000 marlin_data-3.5.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-15 08:15:51.000000 marlin_data-3.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-03-15 08:16:07.099417 marlin_data-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-03-15 08:15:51.000000 marlin_data-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-15 08:15:51.000000 marlin_data-3.5.0/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:16:07.099417 marlin_data-3.5.0/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)    13490 2024-03-15 08:15:51.000000 marlin_data-3.5.0/__pycache__/marlin_data.cpython-311.pyc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:16:07.099417 marlin_data-3.5.0/marlin_data/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-15 08:15:51.000000 marlin_data-3.5.0/marlin_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-15 08:15:51.000000 marlin_data-3.5.0/marlin_data/data.env
--rw-r--r--   0 runner    (1001) docker     (127)    51702 2024-03-15 08:15:51.000000 marlin_data-3.5.0/marlin_data/marlin_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:16:07.099417 marlin_data-3.5.0/marlin_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-03-15 08:16:07.000000 marlin_data-3.5.0/marlin_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-15 08:16:07.000000 marlin_data-3.5.0/marlin_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 08:16:07.000000 marlin_data-3.5.0/marlin_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-15 08:16:07.000000 marlin_data-3.5.0/marlin_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17996 2024-03-15 08:15:51.000000 marlin_data-3.5.0/marlin_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-15 08:15:51.000000 marlin_data-3.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 08:16:07.099417 marlin_data-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-15 08:15:51.000000 marlin_data-3.5.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)  5292000 2024-03-15 08:15:51.000000 marlin_data-3.5.0/testfile.vixen
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-15 08:15:51.000000 marlin_data-3.5.0/token
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:59:02.704330 marlin_data-4.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:59:02.692330 marlin_data-4.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:59:02.704330 marlin_data-4.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-07 13:58:49.000000 marlin_data-4.0.0/.github/workflows/python-app.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-07 13:58:49.000000 marlin_data-4.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-07 13:58:49.000000 marlin_data-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-07 13:59:02.704330 marlin_data-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-05-07 13:58:49.000000 marlin_data-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 13:58:49.000000 marlin_data-4.0.0/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:59:02.704330 marlin_data-4.0.0/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)    13490 2024-05-07 13:58:49.000000 marlin_data-4.0.0/__pycache__/marlin_data.cpython-311.pyc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:59:02.704330 marlin_data-4.0.0/marlin_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 13:58:49.000000 marlin_data-4.0.0/marlin_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-07 13:58:49.000000 marlin_data-4.0.0/marlin_data/data.env
+-rw-r--r--   0 runner    (1001) docker     (127)    51702 2024-05-07 13:58:49.000000 marlin_data-4.0.0/marlin_data/marlin_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:59:02.704330 marlin_data-4.0.0/marlin_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-07 13:59:02.000000 marlin_data-4.0.0/marlin_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 13:59:02.000000 marlin_data-4.0.0/marlin_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 13:59:02.000000 marlin_data-4.0.0/marlin_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 13:59:02.000000 marlin_data-4.0.0/marlin_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17996 2024-05-07 13:58:49.000000 marlin_data-4.0.0/marlin_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-07 13:58:49.000000 marlin_data-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 13:59:02.704330 marlin_data-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-07 13:58:49.000000 marlin_data-4.0.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)  5292000 2024-05-07 13:58:49.000000 marlin_data-4.0.0/testfile.vixen
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 13:58:49.000000 marlin_data-4.0.0/token
```

### Comparing `marlin_data-3.5.0/.github/workflows/python-app.yml` & `marlin_data-4.0.0/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `marlin_data-3.5.0/.github/workflows/python-publish.yml` & `marlin_data-4.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `marlin_data-3.5.0/LICENSE` & `marlin_data-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `marlin_data-3.5.0/PKG-INFO` & `marlin_data-4.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marlin_data
-Version: 3.5.0
+Version: 4.0.0
 Summary: Marlin | Data Framework
 Author: Rahul Tandon
 Author-email: r.tandon@rsaqua.co.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `marlin_data-3.5.0/README.md` & `marlin_data-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `marlin_data-3.5.0/__pycache__/marlin_data.cpython-311.pyc` & `marlin_data-4.0.0/__pycache__/marlin_data.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `marlin_data-3.5.0/marlin_data/marlin_data.py` & `marlin_data-4.0.0/marlin_data/marlin_data.py`

 * *Files identical despite different names*

### Comparing `marlin_data-3.5.0/marlin_data.egg-info/PKG-INFO` & `marlin_data-4.0.0/marlin_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marlin_data
-Version: 3.5.0
+Version: 4.0.0
 Summary: Marlin | Data Framework
 Author: Rahul Tandon
 Author-email: r.tandon@rsaqua.co.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `marlin_data-3.5.0/marlin_data.py` & `marlin_data-4.0.0/marlin_data.py`

 * *Files identical despite different names*

### Comparing `marlin_data-3.5.0/setup.py` & `marlin_data-4.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
 
     name="marlin_data", # Replace with your own username
-    version="3.5.0",
+    version="4.0.0",
     author="Rahul Tandon",
     author_email="r.tandon@rsaqua.co.uk",
     description="Marlin | Data Framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # url="https://github.com/vixencapital/brahma/archive/0.0.5.tar.gz",
     packages=setuptools.find_packages(),
```

### Comparing `marlin_data-3.5.0/testfile.vixen` & `marlin_data-4.0.0/testfile.vixen`

 * *Files identical despite different names*

