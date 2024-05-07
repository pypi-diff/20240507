# Comparing `tmp/facturama-2.0.5.tar.gz` & `tmp/facturama-2.0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facturama-2.0.5.tar", last modified: Tue May  7 01:53:33 2024, max compression
+gzip compressed data, was "facturama-2.0.5.1.tar", last modified: Tue May  7 13:47:40 2024, max compression
```

## Comparing `facturama-2.0.5.tar` & `facturama-2.0.5.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 mchambreuil  (1000) mchambreuil  (1000)        0 2024-05-07 01:53:33.908032 facturama-2.0.5/
--rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)     1068 2024-05-07 01:39:24.000000 facturama-2.0.5/LICENSE
--rw-r--r--   0 mchambreuil  (1000) mchambreuil  (1000)     4162 2024-05-07 01:53:33.908032 facturama-2.0.5/PKG-INFO
--rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)     2048 2024-05-07 01:39:24.000000 facturama-2.0.5/README.md
--rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)       81 2024-05-07 01:39:24.000000 facturama-2.0.5/README.txt
-drwxrwxr-x   0 mchambreuil  (1000) mchambreuil  (1000)        0 2024-05-07 01:53:33.908032 facturama-2.0.5/facturama/
--rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)    24659 2024-05-07 01:39:24.000000 facturama-2.0.5/facturama/__init__.py
-drwxrwxr-x   0 mchambreuil  (1000) mchambreuil  (1000)        0 2024-05-07 01:53:33.908032 facturama-2.0.5/facturama.egg-info/
--rw-r--r--   0 mchambreuil  (1000) mchambreuil  (1000)     4162 2024-05-07 01:53:33.000000 facturama-2.0.5/facturama.egg-info/PKG-INFO
--rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)      421 2024-05-07 01:53:33.000000 facturama-2.0.5/facturama.egg-info/SOURCES.txt
--rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)        1 2024-05-07 01:53:33.000000 facturama-2.0.5/facturama.egg-info/dependency_links.txt
--rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)       25 2024-05-07 01:53:33.000000 facturama-2.0.5/facturama.egg-info/requires.txt
--rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)       16 2024-05-07 01:53:33.000000 facturama-2.0.5/facturama.egg-info/top_level.txt
--rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)        1 2024-05-07 01:40:40.000000 facturama-2.0.5/facturama.egg-info/zip-safe
--rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)      838 2024-05-07 01:51:46.000000 facturama-2.0.5/pyproject.toml
--rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)       38 2024-05-07 01:53:33.908032 facturama-2.0.5/setup.cfg
--rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)     1086 2024-05-07 01:39:24.000000 facturama-2.0.5/setup.py
-drwxrwxr-x   0 mchambreuil  (1000) mchambreuil  (1000)        0 2024-05-07 01:53:33.908032 facturama-2.0.5/tests/
--rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)    18232 2024-05-07 01:39:24.000000 facturama-2.0.5/tests/__init__.py
--rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)      479 2024-05-07 01:39:24.000000 facturama-2.0.5/tests/branch.py
--rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)      301 2024-05-07 01:39:24.000000 facturama-2.0.5/tests/catalogs.py
--rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)     2280 2024-05-07 01:39:24.000000 facturama-2.0.5/tests/cfdi.py
--rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)     2788 2024-05-07 01:39:24.000000 facturama-2.0.5/tests/cfdiMulti.py
--rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)      401 2024-05-07 01:39:24.000000 facturama-2.0.5/tests/csds.py
--rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)     1197 2024-05-07 01:39:24.000000 facturama-2.0.5/tests/csdsMulti.py
--rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)      656 2024-05-07 01:39:24.000000 facturama-2.0.5/tests/customers.py
--rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)      526 2024-05-07 01:39:24.000000 facturama-2.0.5/tests/products.py
+drwxrwxr-x   0 mchambreuil  (1000) mchambreuil  (1000)        0 2024-05-07 13:47:40.234101 facturama-2.0.5.1/
+-rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)     1068 2024-05-07 01:39:24.000000 facturama-2.0.5.1/LICENSE
+-rw-r--r--   0 mchambreuil  (1000) mchambreuil  (1000)     4164 2024-05-07 13:47:40.234101 facturama-2.0.5.1/PKG-INFO
+-rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)     2048 2024-05-07 01:39:24.000000 facturama-2.0.5.1/README.md
+-rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)       81 2024-05-07 01:39:24.000000 facturama-2.0.5.1/README.txt
+drwxrwxr-x   0 mchambreuil  (1000) mchambreuil  (1000)        0 2024-05-07 13:47:40.230101 facturama-2.0.5.1/facturama/
+-rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)    24659 2024-05-07 01:39:24.000000 facturama-2.0.5.1/facturama/__init__.py
+drwxrwxr-x   0 mchambreuil  (1000) mchambreuil  (1000)        0 2024-05-07 13:47:40.234101 facturama-2.0.5.1/facturama.egg-info/
+-rw-r--r--   0 mchambreuil  (1000) mchambreuil  (1000)     4164 2024-05-07 13:47:40.000000 facturama-2.0.5.1/facturama.egg-info/PKG-INFO
+-rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)      421 2024-05-07 13:47:40.000000 facturama-2.0.5.1/facturama.egg-info/SOURCES.txt
+-rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)        1 2024-05-07 13:47:40.000000 facturama-2.0.5.1/facturama.egg-info/dependency_links.txt
+-rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)       25 2024-05-07 13:47:40.000000 facturama-2.0.5.1/facturama.egg-info/requires.txt
+-rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)       16 2024-05-07 13:47:40.000000 facturama-2.0.5.1/facturama.egg-info/top_level.txt
+-rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)        1 2024-05-07 01:40:40.000000 facturama-2.0.5.1/facturama.egg-info/zip-safe
+-rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)      840 2024-05-07 13:47:35.000000 facturama-2.0.5.1/pyproject.toml
+-rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)       38 2024-05-07 13:47:40.234101 facturama-2.0.5.1/setup.cfg
+-rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)     1086 2024-05-07 01:39:24.000000 facturama-2.0.5.1/setup.py
+drwxrwxr-x   0 mchambreuil  (1000) mchambreuil  (1000)        0 2024-05-07 13:47:40.234101 facturama-2.0.5.1/tests/
+-rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)    18232 2024-05-07 01:39:24.000000 facturama-2.0.5.1/tests/__init__.py
+-rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)      479 2024-05-07 01:39:24.000000 facturama-2.0.5.1/tests/branch.py
+-rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)      301 2024-05-07 01:39:24.000000 facturama-2.0.5.1/tests/catalogs.py
+-rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)     2280 2024-05-07 01:39:24.000000 facturama-2.0.5.1/tests/cfdi.py
+-rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)     2788 2024-05-07 01:39:24.000000 facturama-2.0.5.1/tests/cfdiMulti.py
+-rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)      401 2024-05-07 01:39:24.000000 facturama-2.0.5.1/tests/csds.py
+-rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)     1197 2024-05-07 01:39:24.000000 facturama-2.0.5.1/tests/csdsMulti.py
+-rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)      656 2024-05-07 01:39:24.000000 facturama-2.0.5.1/tests/customers.py
+-rw-rw-r--   0 mchambreuil  (1000) mchambreuil  (1000)      526 2024-05-07 01:39:24.000000 facturama-2.0.5.1/tests/products.py
```

### Comparing `facturama-2.0.5/LICENSE` & `facturama-2.0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `facturama-2.0.5/PKG-INFO` & `facturama-2.0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facturama
-Version: 2.0.5
+Version: 2.0.5.1
 Summary: Easy Facturama python wrapper
 Home-page: https://github.com/tingsystems/facturama
 Download-URL: https://github.com/tingsystems/facturama/master
 Author: Tingsystems
 Author-email: Tingsystems <soporte@tingsystems.com>
 License: MIT License
         
@@ -33,15 +33,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: simplejson
 Requires-Dist: nose
 
 # Facturama Python SDK
```

### Comparing `facturama-2.0.5/README.md` & `facturama-2.0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `facturama-2.0.5/facturama/__init__.py` & `facturama-2.0.5.1/facturama/__init__.py`

 * *Files identical despite different names*

### Comparing `facturama-2.0.5/facturama.egg-info/PKG-INFO` & `facturama-2.0.5.1/facturama.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facturama
-Version: 2.0.5
+Version: 2.0.5.1
 Summary: Easy Facturama python wrapper
 Home-page: https://github.com/tingsystems/facturama
 Download-URL: https://github.com/tingsystems/facturama/master
 Author: Tingsystems
 Author-email: Tingsystems <soporte@tingsystems.com>
 License: MIT License
         
@@ -33,15 +33,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: simplejson
 Requires-Dist: nose
 
 # Facturama Python SDK
```

### Comparing `facturama-2.0.5/pyproject.toml` & `facturama-2.0.5.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "facturama"
-version = "2.0.5"
+version = "2.0.5.1"
 description = "Easy Facturama python wrapper"
 readme = "README.md"
 authors = [{ name = "Tingsystems", email = "soporte@tingsystems.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -20,11 +20,11 @@
 ]
 keywords = ["facturama", "wrapper"]
 dependencies = [
     "requests",
     "simplejson",
     "nose",
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 
 [project.urls]
 Homepage = "https://github.com/tingsystems/facturama"
```

### Comparing `facturama-2.0.5/setup.py` & `facturama-2.0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `facturama-2.0.5/tests/__init__.py` & `facturama-2.0.5.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `facturama-2.0.5/tests/cfdi.py` & `facturama-2.0.5.1/tests/cfdi.py`

 * *Files identical despite different names*

### Comparing `facturama-2.0.5/tests/cfdiMulti.py` & `facturama-2.0.5.1/tests/cfdiMulti.py`

 * *Files identical despite different names*

### Comparing `facturama-2.0.5/tests/csdsMulti.py` & `facturama-2.0.5.1/tests/csdsMulti.py`

 * *Files identical despite different names*

### Comparing `facturama-2.0.5/tests/customers.py` & `facturama-2.0.5.1/tests/customers.py`

 * *Files identical despite different names*

### Comparing `facturama-2.0.5/tests/products.py` & `facturama-2.0.5.1/tests/products.py`

 * *Files identical despite different names*

