# Comparing `tmp/quantylf-0.0.7.tar.gz` & `tmp/quantylf-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantylf-0.0.7.tar", last modified: Tue May  7 16:13:47 2024, max compression
+gzip compressed data, was "quantylf-0.0.8.tar", last modified: Tue May  7 18:02:27 2024, max compression
```

## Comparing `quantylf-0.0.7.tar` & `quantylf-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:13:47.296063 quantylf-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-07 16:13:43.000000 quantylf-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-07 16:13:43.000000 quantylf-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-07 16:13:47.296063 quantylf-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-07 16:13:43.000000 quantylf-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-07 16:13:43.000000 quantylf-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-07 16:13:47.296063 quantylf-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:13:47.292063 quantylf-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:13:47.292063 quantylf-0.0.7/src/QuantyLF/
--rw-r--r--   0 runner    (1001) docker     (127)    18673 2024-05-07 16:13:43.000000 quantylf-0.0.7/src/QuantyLF/QuantyLF.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:13:43.000000 quantylf-0.0.7/src/QuantyLF/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:13:47.296063 quantylf-0.0.7/src/QuantyLF/cases/
--rw-r--r--   0 runner    (1001) docker     (127)    18821 2024-05-07 16:13:43.000000 quantylf-0.0.7/src/QuantyLF/cases/Td_3d.lua
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-07 16:13:43.000000 quantylf-0.0.7/src/QuantyLF/cases/Td_3d.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:13:47.296063 quantylf-0.0.7/src/QuantyLF/cases/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-07 16:13:43.000000 quantylf-0.0.7/src/QuantyLF/cases/utils/slater_integrals.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:13:47.296063 quantylf-0.0.7/src/QuantyLF.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-07 16:13:47.000000 quantylf-0.0.7/src/QuantyLF.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-07 16:13:47.000000 quantylf-0.0.7/src/QuantyLF.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 16:13:47.000000 quantylf-0.0.7/src/QuantyLF.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 16:13:47.000000 quantylf-0.0.7/src/QuantyLF.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 16:13:47.000000 quantylf-0.0.7/src/QuantyLF.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:02:27.754917 quantylf-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-07 18:02:23.000000 quantylf-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-07 18:02:23.000000 quantylf-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-07 18:02:27.754917 quantylf-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-07 18:02:23.000000 quantylf-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-07 18:02:23.000000 quantylf-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-07 18:02:27.754917 quantylf-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:02:27.750917 quantylf-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:02:27.750917 quantylf-0.0.8/src/QuantyLF/
+-rw-r--r--   0 runner    (1001) docker     (127)    18703 2024-05-07 18:02:23.000000 quantylf-0.0.8/src/QuantyLF/QuantyLF.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:02:23.000000 quantylf-0.0.8/src/QuantyLF/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:02:27.754917 quantylf-0.0.8/src/QuantyLF/cases/
+-rw-r--r--   0 runner    (1001) docker     (127)    20402 2024-05-07 18:02:23.000000 quantylf-0.0.8/src/QuantyLF/cases/D3h_3d.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-07 18:02:23.000000 quantylf-0.0.8/src/QuantyLF/cases/D3h_3d.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18754 2024-05-07 18:02:23.000000 quantylf-0.0.8/src/QuantyLF/cases/Oh_3d.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-07 18:02:23.000000 quantylf-0.0.8/src/QuantyLF/cases/Oh_3d.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18821 2024-05-07 18:02:23.000000 quantylf-0.0.8/src/QuantyLF/cases/Td_3d.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-07 18:02:23.000000 quantylf-0.0.8/src/QuantyLF/cases/Td_3d.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:02:27.754917 quantylf-0.0.8/src/QuantyLF/cases/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-07 18:02:23.000000 quantylf-0.0.8/src/QuantyLF/cases/utils/slater_integrals.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:02:27.754917 quantylf-0.0.8/src/QuantyLF.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-07 18:02:27.000000 quantylf-0.0.8/src/QuantyLF.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-07 18:02:27.000000 quantylf-0.0.8/src/QuantyLF.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 18:02:27.000000 quantylf-0.0.8/src/QuantyLF.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 18:02:27.000000 quantylf-0.0.8/src/QuantyLF.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 18:02:27.000000 quantylf-0.0.8/src/QuantyLF.egg-info/top_level.txt
```

### Comparing `quantylf-0.0.7/LICENSE` & `quantylf-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `quantylf-0.0.7/PKG-INFO` & `quantylf-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantyLF
-Version: 0.0.7
+Version: 0.0.8
 Summary: QuantyLF is a libary to help manage Liegand Field simulations in Quanty.
 Home-page: https://github.com/CMM02/XPlotLib
 Author: Carl Magnus Meier
 Author-email: magnus.meier@outook.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quantylf-0.0.7/setup.cfg` & `quantylf-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = QuantyLF
-version = 0.0.7
+version = 0.0.8
 author = Carl Magnus Meier
 author_email = magnus.meier@outook.de
 description = QuantyLF is a libary to help manage Liegand Field simulations in Quanty.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CMM02/XPlotLib
 classifiers =
```

### Comparing `quantylf-0.0.7/src/QuantyLF/QuantyLF.py` & `quantylf-0.0.8/src/QuantyLF/QuantyLF.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,20 +325,20 @@
 
     ----------------
     Returns:
     List of available cases
     """
     def available_cases(self):
         base_path = impresources.files(cases)
-        cases = []
+        available_cases = []
         for file in base_path.iterdir():
             if file.suffix == '.lua':
-                cases.append(file.stem)
+                available_cases.append(file.stem)
 
-        return cases
+        return available_cases
     
 
     """
     Load a Quanty case)
 
     ----------------
     Parameters:
```

### Comparing `quantylf-0.0.7/src/QuantyLF/cases/Td_3d.lua` & `quantylf-0.0.8/src/QuantyLF/cases/Td_3d.lua`

 * *Files identical despite different names*

### Comparing `quantylf-0.0.7/src/QuantyLF/cases/utils/slater_integrals.lua` & `quantylf-0.0.8/src/QuantyLF/cases/utils/slater_integrals.lua`

 * *Files identical despite different names*

### Comparing `quantylf-0.0.7/src/QuantyLF.egg-info/PKG-INFO` & `quantylf-0.0.8/src/QuantyLF.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantyLF
-Version: 0.0.7
+Version: 0.0.8
 Summary: QuantyLF is a libary to help manage Liegand Field simulations in Quanty.
 Home-page: https://github.com/CMM02/XPlotLib
 Author: Carl Magnus Meier
 Author-email: magnus.meier@outook.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

