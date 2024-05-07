# Comparing `tmp/zemia-0.0.4.tar.gz` & `tmp/zemia-0.0.5.tar.gz`

## Comparing `zemia-0.0.4.tar` & `zemia-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 zemia-0.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 zemia-0.0.4/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zemia-0.0.4/src/zemia/__init__.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 zemia-0.0.4/src/zemia/common.py
--rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 zemia-0.0.4/src/zemia/file.py
--rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 zemia-0.0.4/src/zemia/spreadsheet.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 zemia-0.0.4/src/zemia/sql.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zemia-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 zemia-0.0.4/tests/test_common.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 zemia-0.0.4/LICENSE
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 zemia-0.0.4/README.md
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 zemia-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 zemia-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 zemia-0.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 zemia-0.0.5/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zemia-0.0.5/src/zemia/__init__.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 zemia-0.0.5/src/zemia/common.py
+-rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 zemia-0.0.5/src/zemia/file.py
+-rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 zemia-0.0.5/src/zemia/spreadsheet.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 zemia-0.0.5/src/zemia/sql.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zemia-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 zemia-0.0.5/tests/test_common.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 zemia-0.0.5/LICENSE
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 zemia-0.0.5/README.md
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 zemia-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 zemia-0.0.5/PKG-INFO
```

### Comparing `zemia-0.0.4/.github/workflows/python-publish.yml` & `zemia-0.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `zemia-0.0.4/src/zemia/file.py` & `zemia-0.0.5/src/zemia/file.py`

 * *Files identical despite different names*

### Comparing `zemia-0.0.4/src/zemia/spreadsheet.py` & `zemia-0.0.5/src/zemia/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `zemia-0.0.4/src/zemia/sql.py` & `zemia-0.0.5/src/zemia/sql.py`

 * *Files identical despite different names*

### Comparing `zemia-0.0.4/LICENSE` & `zemia-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zemia-0.0.4/pyproject.toml` & `zemia-0.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zemia"
-version = "0.0.4"
+version = "0.0.5"
 dependencies = [
   "google-api-python-client", 
   "google-auth-httplib2", 
-  "google-auth-oauthlib"
+  "google-auth-oauthlib",
+  "dataclasses"
 ]
 authors = [
   { name="OK_Diamond", email="ok.thekirks@gmail.com" },
 ]
 description = "Common utilities for Python projects."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `zemia-0.0.4/PKG-INFO` & `zemia-0.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.3
 Name: zemia
-Version: 0.0.4
+Version: 0.0.5
 Summary: Common utilities for Python projects.
 Project-URL: Homepage, https://github.com/Land-of-Zemia/ZemiaLib
 Project-URL: Issues, https://github.com/Land-of-Zemia/ZemiaLib/issues
 Author-email: OK_Diamond <ok.thekirks@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: dataclasses
 Requires-Dist: google-api-python-client
 Requires-Dist: google-auth-httplib2
 Requires-Dist: google-auth-oauthlib
 Description-Content-Type: text/markdown
 
 # ZemiaLib by OK_Diamond
```

