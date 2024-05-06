# Comparing `tmp/model_checker-0.2.6.tar.gz` & `tmp/model_checker-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_checker-0.2.6.tar", last modified: Mon May  6 20:48:40 2024, max compression
+gzip compressed data, was "model_checker-0.2.7.tar", last modified: Mon May  6 21:02:04 2024, max compression
```

## Comparing `model_checker-0.2.6.tar` & `model_checker-0.2.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 20:48:40.571088 model_checker-0.2.6/
--rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-04-26 19:58:45.000000 model_checker-0.2.6/LICENCE
--rw-r--r--   0 benjamin  (1000) users      (100)     1372 2024-05-06 20:48:40.570088 model_checker-0.2.6/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)      683 2024-05-06 19:44:36.000000 model_checker-0.2.6/README.md
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 20:48:40.570088 model_checker-0.2.6/model_checker.egg-info/
--rw-r--r--   0 benjamin  (1000) users      (100)     1372 2024-05-06 20:48:40.000000 model_checker-0.2.6/model_checker.egg-info/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)      456 2024-05-06 20:48:40.000000 model_checker-0.2.6/model_checker.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-06 20:48:40.000000 model_checker-0.2.6/model_checker.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       61 2024-05-06 20:48:40.000000 model_checker-0.2.6/model_checker.egg-info/entry_points.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-06 20:48:40.000000 model_checker-0.2.6/model_checker.egg-info/requires.txt
--rw-r--r--   0 benjamin  (1000) users      (100)        8 2024-05-06 20:48:40.000000 model_checker-0.2.6/model_checker.egg-info/top_level.txt
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 20:48:40.570088 model_checker-0.2.6/package/
--rw-r--r--   0 benjamin  (1000) users      (100)        0 2024-05-06 20:40:08.000000 model_checker-0.2.6/package/__init__.py
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 20:48:40.570088 model_checker-0.2.6/package/modules/
--rw-r--r--   0 benjamin  (1000) users      (100)        0 2024-05-06 20:40:02.000000 model_checker-0.2.6/package/modules/__init__.py
--rw-r--r--   0 benjamin  (1000) users      (100)    16023 2024-05-06 20:40:50.000000 model_checker-0.2.6/package/modules/model_definitions.py
--rw-r--r--   0 benjamin  (1000) users      (100)    34591 2024-05-06 20:40:50.000000 model_checker-0.2.6/package/modules/model_structure.py
--rw-r--r--   0 benjamin  (1000) users      (100)    19660 2024-05-06 20:40:50.000000 model_checker-0.2.6/package/modules/semantics.py
--rw-r--r--   0 benjamin  (1000) users      (100)     7265 2024-05-06 20:40:50.000000 model_checker-0.2.6/package/modules/syntax.py
--rw-r--r--   0 benjamin  (1000) users      (100)     5846 2024-05-06 20:44:05.000000 model_checker-0.2.6/package/test_complete.py
--rw-r--r--   0 benjamin  (1000) users      (100)      901 2024-05-06 20:38:48.000000 model_checker-0.2.6/pyproject.toml
--rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-06 20:48:40.571088 model_checker-0.2.6/setup.cfg
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 21:02:04.972786 model_checker-0.2.7/
+-rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-04-26 19:58:45.000000 model_checker-0.2.7/LICENCE
+-rw-r--r--   0 benjamin  (1000) users      (100)     1372 2024-05-06 21:02:04.971786 model_checker-0.2.7/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)      683 2024-05-06 19:44:36.000000 model_checker-0.2.7/README.md
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 21:02:04.971786 model_checker-0.2.7/model_checker.egg-info/
+-rw-r--r--   0 benjamin  (1000) users      (100)     1372 2024-05-06 21:02:04.000000 model_checker-0.2.7/model_checker.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)      456 2024-05-06 21:02:04.000000 model_checker-0.2.7/model_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-06 21:02:04.000000 model_checker-0.2.7/model_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       61 2024-05-06 21:02:04.000000 model_checker-0.2.7/model_checker.egg-info/entry_points.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-06 21:02:04.000000 model_checker-0.2.7/model_checker.egg-info/requires.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)        8 2024-05-06 21:02:04.000000 model_checker-0.2.7/model_checker.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 21:02:04.971786 model_checker-0.2.7/package/
+-rw-r--r--   0 benjamin  (1000) users      (100)        0 2024-05-06 20:40:08.000000 model_checker-0.2.7/package/__init__.py
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 21:02:04.971786 model_checker-0.2.7/package/modules/
+-rw-r--r--   0 benjamin  (1000) users      (100)        0 2024-05-06 20:40:02.000000 model_checker-0.2.7/package/modules/__init__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    16027 2024-05-06 21:00:04.000000 model_checker-0.2.7/package/modules/model_definitions.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    34591 2024-05-06 20:40:50.000000 model_checker-0.2.7/package/modules/model_structure.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    19660 2024-05-06 20:40:50.000000 model_checker-0.2.7/package/modules/semantics.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     7265 2024-05-06 20:40:50.000000 model_checker-0.2.7/package/modules/syntax.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     5847 2024-05-06 20:58:18.000000 model_checker-0.2.7/package/test_complete.py
+-rw-r--r--   0 benjamin  (1000) users      (100)      901 2024-05-06 21:00:57.000000 model_checker-0.2.7/pyproject.toml
+-rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-06 21:02:04.972786 model_checker-0.2.7/setup.cfg
```

### Comparing `model_checker-0.2.6/LICENCE` & `model_checker-0.2.7/LICENCE`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.6/PKG-INFO` & `model_checker-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-checker
-Version: 0.2.6
+Version: 0.2.7
 Summary: A hyperintensional model checker for counterfactual conditionals
 Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
 Keywords: semantics,Z3,counterfactuals,model checker,theorem prover
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `model_checker-0.2.6/README.md` & `model_checker-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.6/model_checker.egg-info/PKG-INFO` & `model_checker-0.2.7/model_checker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-checker
-Version: 0.2.6
+Version: 0.2.7
 Summary: A hyperintensional model checker for counterfactual conditionals
 Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
 Keywords: semantics,Z3,counterfactuals,model checker,theorem prover
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `model_checker-0.2.6/package/modules/model_definitions.py` & `model_checker-0.2.7/package/modules/model_definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 '''
 file contains all definitions for defining the model structure
 '''
 
 import sys
 from z3 import (
-    BitVecVal, simplify,
+    BitVecVal,
+    simplify,
 )
 
 from .syntax import Infix
 
 def summation(n, func, start = 0):
     '''summation of i ranging from start to n of func(i)
     used in find_all_bits'''
```

### Comparing `model_checker-0.2.6/package/modules/model_structure.py` & `model_checker-0.2.7/package/modules/model_structure.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.6/package/modules/semantics.py` & `model_checker-0.2.7/package/modules/semantics.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.6/package/modules/syntax.py` & `model_checker-0.2.7/package/modules/syntax.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.6/package/test_complete.py` & `model_checker-0.2.7/package/test_complete.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 '''
 
 import argparse
 import os
 import importlib.util
 import sys
 from string import Template
-from modules.model_structure import make_model_for
+from modules import model_structure
 
 script_template = Template("""
 '''
 Model Checker: ${name}
 '''
 import os
 parent_directory = os.path.dirname(__file__)
@@ -50,15 +50,15 @@
 # premises = ['((A vee B) boxright C)']
 # conclusions = ['(A boxright C)']
 
 """)
 
 def print_or_save(module):
     """print the model and prompt user to store the output"""
-    mod = make_model_for(module.N)(module.premises, module.conclusions)
+    mod = model_structure.make_model_for(module.N)(module.premises, module.conclusions)
     if module.use_constraints_bool:
         mod.constraints = module.all_constraints
     mod.print_to(module.print_cons_bool, module.print_unsat_core_bool)
     if not module.save_bool:
         return
     result = input("Would you like to save the output? (y/n):\n")
     if not result in ['Yes', 'yes', 'y']:
```

### Comparing `model_checker-0.2.6/pyproject.toml` & `model_checker-0.2.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model-checker"
-version = "0.2.6"
+version = "0.2.7"
 description = "A hyperintensional model checker for counterfactual conditionals"
 authors = [
     { name = "Benjamin Brast-McKie", email = "benbrastmckie@gmail.com" },
     { name = "Miguel Buitrago", email = "mbuit82@gmail.com" },
 ]
 license = { text = "MIT" }
 readme = "README.md"
```

