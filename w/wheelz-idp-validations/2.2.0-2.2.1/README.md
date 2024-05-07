# Comparing `tmp/wheelz_idp_validations-2.2.0.tar.gz` & `tmp/wheelz_idp_validations-2.2.1.tar.gz`

## Comparing `wheelz_idp_validations-2.2.0.tar` & `wheelz_idp_validations-2.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/LICESNSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/requirements.txt
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/__init__.py
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/id_sanitizer.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/pcv1_sanitizer.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/pcv2_sanitizer.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitize_exception.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/exceptions/__init__.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/exceptions/cif_exceptions.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/exceptions/date_exceptions.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/exceptions/full_name_exceptions.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/exceptions/gender_exceptions.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/exceptions/id_exceptions.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/exceptions/plate_exceptions.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/exceptions/vin_exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/__init__.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/cif.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/date.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/full_name.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/gender.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/id_number.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/plate.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/vin.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/.gitignore
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/pyproject.toml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/readme.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/LICESNSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/requirements.txt
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/__init__.py
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/id_sanitizer.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/pcv1_sanitizer.py
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/pcv2_sanitizer.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/sanitize_exception.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/exceptions/__init__.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/exceptions/cif_exceptions.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/exceptions/date_exceptions.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/exceptions/full_name_exceptions.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/exceptions/gender_exceptions.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/exceptions/id_exceptions.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/exceptions/plate_exceptions.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/exceptions/vin_exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/sanitizers/__init__.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/sanitizers/cif.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/sanitizers/date.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/sanitizers/full_name.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/sanitizers/gender.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/sanitizers/id_number.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/sanitizers/plate.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/sanitizers/vin.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/.gitignore
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/readme.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.1/PKG-INFO
```

### Comparing `wheelz_idp_validations-2.2.0/LICESNSE` & `wheelz_idp_validations-2.2.1/LICESNSE`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.2.0/.github/workflows/python-publish.yml` & `wheelz_idp_validations-2.2.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/id_sanitizer.py` & `wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/id_sanitizer.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/pcv1_sanitizer.py` & `wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/pcv1_sanitizer.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/exceptions/cif_exceptions.py` & `wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/exceptions/cif_exceptions.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/exceptions/id_exceptions.py` & `wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/exceptions/id_exceptions.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/cif.py` & `wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/sanitizers/cif.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/date.py` & `wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/sanitizers/date.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/full_name.py` & `wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/sanitizers/full_name.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/gender.py` & `wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/sanitizers/gender.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/id_number.py` & `wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/sanitizers/id_number.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/plate.py` & `wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/sanitizers/plate.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/vin.py` & `wheelz_idp_validations-2.2.1/src/wheelz_idp_validations/sanitizers/vin.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.2.0/pyproject.toml` & `wheelz_idp_validations-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/wheelz_idp_validations"]
 
 
 [project]
 name = "wheelz_idp_validations"
-version = "2.2.0"
+version = "2.2.1"
 authors = [
   { name="Lluis" },
 ]
 description = "Validation for spasnish documents"
 readme = "readme.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `wheelz_idp_validations-2.2.0/PKG-INFO` & `wheelz_idp_validations-2.2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: wheelz_idp_validations
-Version: 2.2.0
+Version: 2.2.1
 Summary: Validation for spasnish documents
 Project-URL: Homepage, https://github.com/albertvazquezm/wheelz-idp-validations
 Project-URL: Issues, https://github.com/albertvazquezm/wheelz-idp-validationsissues
 Author: Lluis
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

