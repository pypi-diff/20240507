# Comparing `tmp/sag_py_auth_brand-0.3.0.tar.gz` & `tmp/sag_py_auth_brand-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sag_py_auth_brand-0.3.0.tar", last modified: Wed Apr 24 10:11:04 2024, max compression
+gzip compressed data, was "sag_py_auth_brand-0.3.1.tar", last modified: Tue May  7 12:45:17 2024, max compression
```

## Comparing `sag_py_auth_brand-0.3.0.tar` & `sag_py_auth_brand-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:11:04.915811 sag_py_auth_brand-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-04-24 10:11:04.915811 sag_py_auth_brand-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:11:04.911811 sag_py_auth_brand-0.3.0/sag_py_auth_brand/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/sag_py_auth_brand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/sag_py_auth_brand/brand_jwt_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/sag_py_auth_brand/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/sag_py_auth_brand/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/sag_py_auth_brand/request_brand_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/sag_py_auth_brand/request_brand_logging_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:11:04.911811 sag_py_auth_brand-0.3.0/sag_py_auth_brand.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-04-24 10:11:04.000000 sag_py_auth_brand-0.3.0/sag_py_auth_brand.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-24 10:11:04.000000 sag_py_auth_brand-0.3.0/sag_py_auth_brand.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:11:04.000000 sag_py_auth_brand-0.3.0/sag_py_auth_brand.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-24 10:11:04.000000 sag_py_auth_brand-0.3.0/sag_py_auth_brand.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 10:11:04.000000 sag_py_auth_brand-0.3.0/sag_py_auth_brand.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-24 10:11:04.915811 sag_py_auth_brand-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:11:04.911811 sag_py_auth_brand-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/tests/test_brand_jwt_auth__call.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/tests/test_brand_jwt_auth__init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/tests/test_brand_jwt_auth__verify_brand.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/tests/test_request_brand_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/tests/test_request_brand_logging_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:45:17.840397 sag_py_auth_brand-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-07 12:45:14.000000 sag_py_auth_brand-0.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-07 12:45:17.840397 sag_py_auth_brand-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-07 12:45:14.000000 sag_py_auth_brand-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-07 12:45:14.000000 sag_py_auth_brand-0.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:45:17.840397 sag_py_auth_brand-0.3.1/sag_py_auth_brand/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-07 12:45:14.000000 sag_py_auth_brand-0.3.1/sag_py_auth_brand/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-07 12:45:14.000000 sag_py_auth_brand-0.3.1/sag_py_auth_brand/brand_jwt_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-07 12:45:14.000000 sag_py_auth_brand-0.3.1/sag_py_auth_brand/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 12:45:14.000000 sag_py_auth_brand-0.3.1/sag_py_auth_brand/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-07 12:45:14.000000 sag_py_auth_brand-0.3.1/sag_py_auth_brand/request_brand_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-07 12:45:14.000000 sag_py_auth_brand-0.3.1/sag_py_auth_brand/request_brand_logging_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:45:17.840397 sag_py_auth_brand-0.3.1/sag_py_auth_brand.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-07 12:45:17.000000 sag_py_auth_brand-0.3.1/sag_py_auth_brand.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-07 12:45:17.000000 sag_py_auth_brand-0.3.1/sag_py_auth_brand.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 12:45:17.000000 sag_py_auth_brand-0.3.1/sag_py_auth_brand.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-07 12:45:17.000000 sag_py_auth_brand-0.3.1/sag_py_auth_brand.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 12:45:17.000000 sag_py_auth_brand-0.3.1/sag_py_auth_brand.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-07 12:45:17.840397 sag_py_auth_brand-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-07 12:45:14.000000 sag_py_auth_brand-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:45:17.840397 sag_py_auth_brand-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-07 12:45:14.000000 sag_py_auth_brand-0.3.1/tests/test_brand_jwt_auth__call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-07 12:45:14.000000 sag_py_auth_brand-0.3.1/tests/test_brand_jwt_auth__init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-07 12:45:14.000000 sag_py_auth_brand-0.3.1/tests/test_brand_jwt_auth__verify_brand.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-07 12:45:14.000000 sag_py_auth_brand-0.3.1/tests/test_request_brand_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-07 12:45:14.000000 sag_py_auth_brand-0.3.1/tests/test_request_brand_logging_filter.py
```

### Comparing `sag_py_auth_brand-0.3.0/LICENSE.txt` & `sag_py_auth_brand-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sag_py_auth_brand-0.3.0/PKG-INFO` & `sag_py_auth_brand-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-auth-brand
-Version: 0.3.0
+Version: 0.3.1
 Summary: Keycloak brand/instance authentication for python projects
 Home-page: https://github.com/SamhammerAG/sag_py_auth_brand
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_auth_brand
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_auth_brand/issues
@@ -16,16 +16,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: contextvars>=2.4
-Requires-Dist: fastapi[all]>=0.104.1
-Requires-Dist: sag-py-auth>=0.1.4
+Requires-Dist: fastapi[all]>=0.110.3
+Requires-Dist: sag-py-auth>=0.1.7
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 
 # sag_py_auth_brand
 
 [![Maintainability][codeclimate-image]][codeclimate-url]
 [![Coverage Status][coveralls-image]][coveralls-url]
```

### Comparing `sag_py_auth_brand-0.3.0/README.md` & `sag_py_auth_brand-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `sag_py_auth_brand-0.3.0/sag_py_auth_brand/brand_jwt_auth.py` & `sag_py_auth_brand-0.3.1/sag_py_auth_brand/brand_jwt_auth.py`

 * *Files identical despite different names*

### Comparing `sag_py_auth_brand-0.3.0/sag_py_auth_brand/request_brand_context.py` & `sag_py_auth_brand-0.3.1/sag_py_auth_brand/request_brand_context.py`

 * *Files identical despite different names*

### Comparing `sag_py_auth_brand-0.3.0/sag_py_auth_brand.egg-info/PKG-INFO` & `sag_py_auth_brand-0.3.1/sag_py_auth_brand.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-auth-brand
-Version: 0.3.0
+Version: 0.3.1
 Summary: Keycloak brand/instance authentication for python projects
 Home-page: https://github.com/SamhammerAG/sag_py_auth_brand
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_auth_brand
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_auth_brand/issues
@@ -16,16 +16,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: contextvars>=2.4
-Requires-Dist: fastapi[all]>=0.104.1
-Requires-Dist: sag-py-auth>=0.1.4
+Requires-Dist: fastapi[all]>=0.110.3
+Requires-Dist: sag-py-auth>=0.1.7
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 
 # sag_py_auth_brand
 
 [![Maintainability][codeclimate-image]][codeclimate-url]
 [![Coverage Status][coveralls-image]][coveralls-url]
```

### Comparing `sag_py_auth_brand-0.3.0/sag_py_auth_brand.egg-info/SOURCES.txt` & `sag_py_auth_brand-0.3.1/sag_py_auth_brand.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sag_py_auth_brand-0.3.0/setup.py` & `sag_py_auth_brand-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     REQS = fin.read().splitlines()
 
 with open("requirements-dev.txt", "r") as fin:
     REQS_DEV = [item for item in fin.read().splitlines() if not item.endswith(".txt")]
 
 setuptools.setup(
     name="sag-py-auth-brand",
-    version="0.3.0",
+    version="0.3.1",
     description="Keycloak brand/instance authentication for python projects",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/SamhammerAG/sag_py_auth_brand",
     author="Samhammer AG",
     author_email="support@samhammer.de",
     license="MIT",
```

### Comparing `sag_py_auth_brand-0.3.0/tests/test_brand_jwt_auth__call.py` & `sag_py_auth_brand-0.3.1/tests/test_brand_jwt_auth__call.py`

 * *Files identical despite different names*

### Comparing `sag_py_auth_brand-0.3.0/tests/test_brand_jwt_auth__init.py` & `sag_py_auth_brand-0.3.1/tests/test_brand_jwt_auth__init.py`

 * *Files identical despite different names*

### Comparing `sag_py_auth_brand-0.3.0/tests/test_brand_jwt_auth__verify_brand.py` & `sag_py_auth_brand-0.3.1/tests/test_brand_jwt_auth__verify_brand.py`

 * *Files identical despite different names*

### Comparing `sag_py_auth_brand-0.3.0/tests/test_request_brand_context.py` & `sag_py_auth_brand-0.3.1/tests/test_request_brand_context.py`

 * *Files identical despite different names*

### Comparing `sag_py_auth_brand-0.3.0/tests/test_request_brand_logging_filter.py` & `sag_py_auth_brand-0.3.1/tests/test_request_brand_logging_filter.py`

 * *Files identical despite different names*

