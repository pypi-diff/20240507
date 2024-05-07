# Comparing `tmp/enthalpy_estimator-0.2.5.tar.gz` & `tmp/enthalpy_estimator-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enthalpy_estimator-0.2.5.tar", max compression
+gzip compressed data, was "enthalpy_estimator-0.3.tar", max compression
```

## Comparing `enthalpy_estimator-0.2.5.tar` & `enthalpy_estimator-0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35768 2024-05-03 19:09:07.867044 enthalpy_estimator-0.2.5/LICENSE
--rw-r--r--   0        0        0      441 2024-05-07 13:33:42.416693 enthalpy_estimator-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      763 2024-05-04 21:56:43.249913 enthalpy_estimator-0.2.5/README.md
--rw-r--r--   0        0        0      386 2024-05-03 19:37:10.055544 enthalpy_estimator-0.2.5/src/enthalpy_estimator/__init__.py
--rw-r--r--   0        0        0       18 2024-05-03 17:47:18.389710 enthalpy_estimator-0.2.5/src/enthalpy_estimator/cfg.py
--rw-r--r--   0        0        0     5141 2024-05-07 13:33:34.515970 enthalpy_estimator-0.2.5/src/enthalpy_estimator/generator.py
--rw-r--r--   0        0        0    45568 2023-11-16 15:28:28.012939 enthalpy_estimator-0.2.5/src/enthalpy_estimator/rgen.dll
--rw-r--r--   0        0        0    22120 2023-11-20 18:00:58.231043 enthalpy_estimator-0.2.5/src/enthalpy_estimator/rgen.so
--rw-r--r--   0        0        0     2911 2024-05-04 19:02:59.973822 enthalpy_estimator-0.2.5/src/enthalpy_estimator/simple_vectorizer.py
--rw-r--r--   0        0        0     4477 2024-05-04 19:34:39.570018 enthalpy_estimator-0.2.5/src/enthalpy_estimator/single_reaction.py
--rw-r--r--   0        0        0     1793 2024-05-04 20:59:22.245878 enthalpy_estimator-0.2.5/src/enthalpy_estimator/smiles_vectorizer.py
--rw-r--r--   0        0        0     1336 1970-01-01 00:00:00.000000 enthalpy_estimator-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    35768 2024-05-03 19:09:07.867044 enthalpy_estimator-0.3/LICENSE
+-rw-r--r--   0        0        0      439 2024-05-07 13:45:16.194911 enthalpy_estimator-0.3/pyproject.toml
+-rw-r--r--   0        0        0      763 2024-05-04 21:56:43.249913 enthalpy_estimator-0.3/README.md
+-rw-r--r--   0        0        0      386 2024-05-03 19:37:10.055544 enthalpy_estimator-0.3/src/enthalpy_estimator/__init__.py
+-rw-r--r--   0        0        0       18 2024-05-03 17:47:18.389710 enthalpy_estimator-0.3/src/enthalpy_estimator/cfg.py
+-rw-r--r--   0        0        0     5141 2024-05-07 13:33:34.515970 enthalpy_estimator-0.3/src/enthalpy_estimator/generator.py
+-rw-r--r--   0        0        0    45568 2023-11-16 15:28:28.012939 enthalpy_estimator-0.3/src/enthalpy_estimator/rgen.dll
+-rw-r--r--   0        0        0    22120 2023-11-20 18:00:58.231043 enthalpy_estimator-0.3/src/enthalpy_estimator/rgen.so
+-rw-r--r--   0        0        0     2953 2024-05-07 13:45:04.075217 enthalpy_estimator-0.3/src/enthalpy_estimator/simple_vectorizer.py
+-rw-r--r--   0        0        0     4477 2024-05-04 19:34:39.570018 enthalpy_estimator-0.3/src/enthalpy_estimator/single_reaction.py
+-rw-r--r--   0        0        0     1793 2024-05-04 20:59:22.245878 enthalpy_estimator-0.3/src/enthalpy_estimator/smiles_vectorizer.py
+-rw-r--r--   0        0        0     1334 1970-01-01 00:00:00.000000 enthalpy_estimator-0.3/PKG-INFO
```

### Comparing `enthalpy_estimator-0.2.5/LICENSE` & `enthalpy_estimator-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `enthalpy_estimator-0.2.5/README.md` & `enthalpy_estimator-0.3/README.md`

 * *Files identical despite different names*

### Comparing `enthalpy_estimator-0.2.5/src/enthalpy_estimator/generator.py` & `enthalpy_estimator-0.3/src/enthalpy_estimator/generator.py`

 * *Files identical despite different names*

### Comparing `enthalpy_estimator-0.2.5/src/enthalpy_estimator/rgen.dll` & `enthalpy_estimator-0.3/src/enthalpy_estimator/rgen.dll`

 * *Files identical despite different names*

### Comparing `enthalpy_estimator-0.2.5/src/enthalpy_estimator/rgen.so` & `enthalpy_estimator-0.3/src/enthalpy_estimator/rgen.so`

 * *Files identical despite different names*

### Comparing `enthalpy_estimator-0.2.5/src/enthalpy_estimator/simple_vectorizer.py` & `enthalpy_estimator-0.3/src/enthalpy_estimator/simple_vectorizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,21 +64,21 @@
 
         s = ''
         s += '+'.join(
                 ''.join([str(r[i].item()) + '*'
                          if abs(r[i].item()) != 1
                          else '', 
                          self.all_species[i]['name']
-                         if 'name' in self.all_species[i]
+                         if 'name' in self.all_species[i] and 'name' is not ''
                          else self.vector_to_str(self.basis[i])]) 
                 for i in reagents)
         s += '->'
         s += '+'.join(
                 ''.join([str(-r[i].item()) + '*'
                          if abs(r[i].item()) != 1
                          else '', 
                          self.all_species[i]['name']
-                         if 'name' in self.all_species[i]
+                         if 'name' in self.all_species[i] and 'name' is not ''
                          else self.vector_to_str(self.basis[i])]) 
                 for i in products)
 
         return s
```

### Comparing `enthalpy_estimator-0.2.5/src/enthalpy_estimator/single_reaction.py` & `enthalpy_estimator-0.3/src/enthalpy_estimator/single_reaction.py`

 * *Files identical despite different names*

### Comparing `enthalpy_estimator-0.2.5/src/enthalpy_estimator/smiles_vectorizer.py` & `enthalpy_estimator-0.3/src/enthalpy_estimator/smiles_vectorizer.py`

 * *Files identical despite different names*

### Comparing `enthalpy_estimator-0.2.5/PKG-INFO` & `enthalpy_estimator-0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enthalpy_estimator
-Version: 0.2.5
+Version: 0.3
 Summary: A package to automatically generate reactions and estimate enthalpy.
 License: GNU General Public License v3.0
 Author: Egor Nosach
 Requires-Python: >=3.9
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

