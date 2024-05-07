# Comparing `tmp/genie_partner_sdk-1.0.0.tar.gz` & `tmp/genie_partner_sdk-1.0.1.tar.gz`

## Comparing `genie_partner_sdk-1.0.0.tar` & `genie_partner_sdk-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 genie_partner_sdk-1.0.0/src/genie_partner_sdk/__init__.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 genie_partner_sdk-1.0.0/src/genie_partner_sdk/auth.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 genie_partner_sdk-1.0.0/src/genie_partner_sdk/client.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 genie_partner_sdk-1.0.0/src/genie_partner_sdk/model.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 genie_partner_sdk-1.0.0/LICENSE
--rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 genie_partner_sdk-1.0.0/README.md
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 genie_partner_sdk-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 genie_partner_sdk-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 genie_partner_sdk-1.0.1/Pipfile
+-rw-r--r--   0        0        0    32405 2020-02-02 00:00:00.000000 genie_partner_sdk-1.0.1/Pipfile.lock
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 genie_partner_sdk-1.0.1/src/genie_partner_sdk/__init__.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 genie_partner_sdk-1.0.1/src/genie_partner_sdk/auth.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 genie_partner_sdk-1.0.1/src/genie_partner_sdk/client.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 genie_partner_sdk-1.0.1/src/genie_partner_sdk/model.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 genie_partner_sdk-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 genie_partner_sdk-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 genie_partner_sdk-1.0.1/README.md
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 genie_partner_sdk-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 genie_partner_sdk-1.0.1/PKG-INFO
```

### Comparing `genie_partner_sdk-1.0.0/src/genie_partner_sdk/auth.py` & `genie_partner_sdk-1.0.1/src/genie_partner_sdk/auth.py`

 * *Files identical despite different names*

### Comparing `genie_partner_sdk-1.0.0/src/genie_partner_sdk/client.py` & `genie_partner_sdk-1.0.1/src/genie_partner_sdk/client.py`

 * *Files identical despite different names*

### Comparing `genie_partner_sdk-1.0.0/src/genie_partner_sdk/model.py` & `genie_partner_sdk-1.0.1/src/genie_partner_sdk/model.py`

 * *Files identical despite different names*

### Comparing `genie_partner_sdk-1.0.0/LICENSE` & `genie_partner_sdk-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `genie_partner_sdk-1.0.0/README.md` & `genie_partner_sdk-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `genie_partner_sdk-1.0.0/pyproject.toml` & `genie_partner_sdk-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "genie_partner_sdk"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     { name="Adam Johnston", email="adam_johnston@geniecompany.com" },
 ]
 description = "An SDK to interact with the AladdinConnect (or OHD) partner API"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `genie_partner_sdk-1.0.0/PKG-INFO` & `genie_partner_sdk-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: genie_partner_sdk
-Version: 1.0.0
+Version: 1.0.1
 Summary: An SDK to interact with the AladdinConnect (or OHD) partner API
 Project-URL: Homepage, https://github.com/genie-garage/aladdin-python-sdk
 Project-URL: Issues, https://github.com/genie-garage/aladdin-python-sdk/issues
 Author-email: Adam Johnston <adam_johnston@geniecompany.com>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

