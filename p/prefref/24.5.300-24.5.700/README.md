# Comparing `tmp/prefref-24.5.300.tar.gz` & `tmp/prefref-24.5.700.tar.gz`

## Comparing `prefref-24.5.300.tar` & `prefref-24.5.700.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 prefref-24.5.300/.python-version
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 prefref-24.5.300/Makefile
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 prefref-24.5.300/requirements.txt
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 prefref-24.5.300/todo.md
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 prefref-24.5.300/src/prefref/__init__.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 prefref-24.5.300/src/prefref/examples.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 prefref-24.5.300/src/prefref/exceptions.py
--rw-r--r--   0        0        0    18744 2020-02-02 00:00:00.000000 prefref-24.5.300/src/prefref/prefref.py
--rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 prefref-24.5.300/.gitignore
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 prefref-24.5.300/LICENSE
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 prefref-24.5.300/README.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 prefref-24.5.300/pyproject.toml
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 prefref-24.5.300/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 prefref-24.5.700/.python-version
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 prefref-24.5.700/Makefile
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 prefref-24.5.700/requirements.txt
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 prefref-24.5.700/todo.md
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 prefref-24.5.700/src/prefref/__init__.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 prefref-24.5.700/src/prefref/examples.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 prefref-24.5.700/src/prefref/exceptions.py
+-rw-r--r--   0        0        0    18817 2020-02-02 00:00:00.000000 prefref-24.5.700/src/prefref/prefref.py
+-rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 prefref-24.5.700/.gitignore
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 prefref-24.5.700/LICENSE
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 prefref-24.5.700/README.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 prefref-24.5.700/pyproject.toml
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 prefref-24.5.700/PKG-INFO
```

### Comparing `prefref-24.5.300/Makefile` & `prefref-24.5.700/Makefile`

 * *Files identical despite different names*

### Comparing `prefref-24.5.300/todo.md` & `prefref-24.5.700/todo.md`

 * *Files identical despite different names*

### Comparing `prefref-24.5.300/src/prefref/examples.py` & `prefref-24.5.700/src/prefref/examples.py`

 * *Files identical despite different names*

### Comparing `prefref-24.5.300/src/prefref/exceptions.py` & `prefref-24.5.700/src/prefref/exceptions.py`

 * *Files identical despite different names*

### Comparing `prefref-24.5.300/src/prefref/prefref.py` & `prefref-24.5.700/src/prefref/prefref.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,14 +350,15 @@
   # create a new json file
   def create_json_config(self, options: Config_Options) -> dict:
     content: dict = {}
     for key in options.__dict__:
       option = options.__dict__[key]
       if not option.no_file:
         content[key] = option.value
+    os.makedirs(os.path.dirname(options.config_filepath), exist_ok=True)
     self.write_json_config(content=content)
     return self.read_json_config()
 
 
   # write values to json file, converting some values for proper storage
   def write_json_config(self, content: dict = {}) -> dict:
     self.logger.debug(f'Writing JSON file: {self.config_filepath}')
```

### Comparing `prefref-24.5.300/.gitignore` & `prefref-24.5.700/.gitignore`

 * *Files identical despite different names*

### Comparing `prefref-24.5.300/LICENSE` & `prefref-24.5.700/LICENSE`

 * *Files identical despite different names*

### Comparing `prefref-24.5.300/README.md` & `prefref-24.5.700/README.md`

 * *Files identical despite different names*

### Comparing `prefref-24.5.300/PKG-INFO` & `prefref-24.5.700/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: prefref
-Version: 24.5.300
+Version: 24.5.700
 Summary: A basic config package that reads a JSON config file, environment variables, and console arguments (prioritized in that order)
 Project-URL: Homepage, https://github.com/ghostdisco/prefref
 Project-URL: Issues, https://github.com/ghostdisco/prefref/issues
 Author-email: ghostdisco <pypi@ghostdisco.me>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

