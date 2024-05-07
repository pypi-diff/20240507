# Comparing `tmp/enthalpy_estimator-0.1.tar.gz` & `tmp/enthalpy_estimator-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enthalpy_estimator-0.1.tar", max compression
+gzip compressed data, was "enthalpy_estimator-0.2.tar", max compression
```

## Comparing `enthalpy_estimator-0.1.tar` & `enthalpy_estimator-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35768 2024-05-03 19:09:07.867044 enthalpy_estimator-0.1/LICENSE
--rw-r--r--   0        0        0      439 2024-05-07 12:43:31.432618 enthalpy_estimator-0.1/pyproject.toml
--rw-r--r--   0        0        0      763 2024-05-04 21:56:43.249913 enthalpy_estimator-0.1/README.md
--rw-r--r--   0        0        0      386 2024-05-03 19:37:10.055544 enthalpy_estimator-0.1/src/enthalpy_estimator/__init__.py
--rw-r--r--   0        0        0       18 2024-05-03 17:47:18.389710 enthalpy_estimator-0.1/src/enthalpy_estimator/cfg.py
--rw-r--r--   0        0        0     5145 2024-05-07 12:35:58.907945 enthalpy_estimator-0.1/src/enthalpy_estimator/generator.py
--rw-r--r--   0        0        0    45568 2023-11-16 15:28:28.012939 enthalpy_estimator-0.1/src/enthalpy_estimator/rgen.dll
--rw-r--r--   0        0        0    22120 2023-11-20 18:00:58.231043 enthalpy_estimator-0.1/src/enthalpy_estimator/rgen.so
--rw-r--r--   0        0        0     2911 2024-05-04 19:02:59.973822 enthalpy_estimator-0.1/src/enthalpy_estimator/simple_vectorizer.py
--rw-r--r--   0        0        0     4477 2024-05-04 19:34:39.570018 enthalpy_estimator-0.1/src/enthalpy_estimator/single_reaction.py
--rw-r--r--   0        0        0     1793 2024-05-04 20:59:22.245878 enthalpy_estimator-0.1/src/enthalpy_estimator/smiles_vectorizer.py
--rw-r--r--   0        0        0     1334 1970-01-01 00:00:00.000000 enthalpy_estimator-0.1/PKG-INFO
+-rw-r--r--   0        0        0    35768 2024-05-03 19:09:07.867044 enthalpy_estimator-0.2/LICENSE
+-rw-r--r--   0        0        0      439 2024-05-07 13:30:25.086307 enthalpy_estimator-0.2/pyproject.toml
+-rw-r--r--   0        0        0      763 2024-05-04 21:56:43.249913 enthalpy_estimator-0.2/README.md
+-rw-r--r--   0        0        0      386 2024-05-03 19:37:10.055544 enthalpy_estimator-0.2/src/enthalpy_estimator/__init__.py
+-rw-r--r--   0        0        0       18 2024-05-03 17:47:18.389710 enthalpy_estimator-0.2/src/enthalpy_estimator/cfg.py
+-rw-r--r--   0        0        0     5141 2024-05-07 13:27:18.606733 enthalpy_estimator-0.2/src/enthalpy_estimator/generator.py
+-rw-r--r--   0        0        0    45568 2023-11-16 15:28:28.012939 enthalpy_estimator-0.2/src/enthalpy_estimator/rgen.dll
+-rw-r--r--   0        0        0    22120 2023-11-20 18:00:58.231043 enthalpy_estimator-0.2/src/enthalpy_estimator/rgen.so
+-rw-r--r--   0        0        0     2911 2024-05-04 19:02:59.973822 enthalpy_estimator-0.2/src/enthalpy_estimator/simple_vectorizer.py
+-rw-r--r--   0        0        0     4477 2024-05-04 19:34:39.570018 enthalpy_estimator-0.2/src/enthalpy_estimator/single_reaction.py
+-rw-r--r--   0        0        0     1793 2024-05-04 20:59:22.245878 enthalpy_estimator-0.2/src/enthalpy_estimator/smiles_vectorizer.py
+-rw-r--r--   0        0        0     1334 1970-01-01 00:00:00.000000 enthalpy_estimator-0.2/PKG-INFO
```

### Comparing `enthalpy_estimator-0.1/LICENSE` & `enthalpy_estimator-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `enthalpy_estimator-0.1/README.md` & `enthalpy_estimator-0.2/README.md`

 * *Files identical despite different names*

### Comparing `enthalpy_estimator-0.1/src/enthalpy_estimator/generator.py` & `enthalpy_estimator-0.2/src/enthalpy_estimator/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     def get_basis(self):
         return self.vectorizer.basis
 
     def init_energies(self):
         def read_energies(entry, r):
             try:
                 with open(r['energies'], 'r') as f:
-                    for l in f.readlines()[2:]:
+                    for l in f.readlines():
                         if '=' in l:
                             l_split = [s.strip() for s in l.split('=')]
                             entry[l_split[0]] = float(l_split[-1])
             except Exception:
                 print(f'Error reading file {r["energies"]}')
 
         def read_Hcorr(entry, r):
```

### Comparing `enthalpy_estimator-0.1/src/enthalpy_estimator/rgen.dll` & `enthalpy_estimator-0.2/src/enthalpy_estimator/rgen.dll`

 * *Files identical despite different names*

### Comparing `enthalpy_estimator-0.1/src/enthalpy_estimator/rgen.so` & `enthalpy_estimator-0.2/src/enthalpy_estimator/rgen.so`

 * *Files identical despite different names*

### Comparing `enthalpy_estimator-0.1/src/enthalpy_estimator/simple_vectorizer.py` & `enthalpy_estimator-0.2/src/enthalpy_estimator/simple_vectorizer.py`

 * *Files identical despite different names*

### Comparing `enthalpy_estimator-0.1/src/enthalpy_estimator/single_reaction.py` & `enthalpy_estimator-0.2/src/enthalpy_estimator/single_reaction.py`

 * *Files identical despite different names*

### Comparing `enthalpy_estimator-0.1/src/enthalpy_estimator/smiles_vectorizer.py` & `enthalpy_estimator-0.2/src/enthalpy_estimator/smiles_vectorizer.py`

 * *Files identical despite different names*

### Comparing `enthalpy_estimator-0.1/PKG-INFO` & `enthalpy_estimator-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enthalpy_estimator
-Version: 0.1
+Version: 0.2
 Summary: A package to automatically generate reactions and estimate enthalpy.
 License: GNU General Public License v3.0
 Author: Egor Nosach
 Requires-Python: >=3.9
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

