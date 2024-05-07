# Comparing `tmp/views_tensor_utilities-0.8.4.tar.gz` & `tmp/views_tensor_utilities-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "views_tensor_utilities-0.8.4.tar", max compression
+gzip compressed data, was "views_tensor_utilities-0.8.5.tar", max compression
```

## Comparing `views_tensor_utilities-0.8.4.tar` & `views_tensor_utilities-0.8.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     8303 2024-03-04 12:04:18.486295 views_tensor_utilities-0.8.4/README.md
--rw-r--r--   0        0        0      456 2024-04-25 12:56:24.092953 views_tensor_utilities-0.8.4/pyproject.toml
--rw-r--r--   0        0        0        1 2024-02-23 12:07:30.835277 views_tensor_utilities-0.8.4/views_tensor_utilities/__init__.py
--rw-r--r--   0        0        0      406 2024-03-06 13:40:55.851241 views_tensor_utilities-0.8.4/views_tensor_utilities/defaults.py
--rw-r--r--   0        0        0    17552 2024-04-25 11:54:29.257148 views_tensor_utilities-0.8.4/views_tensor_utilities/mappings.py
--rw-r--r--   0        0        0    11099 2024-04-23 11:49:43.048800 views_tensor_utilities-0.8.4/views_tensor_utilities/objects.py
--rw-r--r--   0        0        0     8754 1970-01-01 00:00:00.000000 views_tensor_utilities-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     8303 2024-03-04 12:04:18.486295 views_tensor_utilities-0.8.5/README.md
+-rw-r--r--   0        0        0      456 2024-05-07 11:30:35.989947 views_tensor_utilities-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-02-23 12:07:30.835277 views_tensor_utilities-0.8.5/views_tensor_utilities/__init__.py
+-rw-r--r--   0        0        0      406 2024-03-06 13:40:55.851241 views_tensor_utilities-0.8.5/views_tensor_utilities/defaults.py
+-rw-r--r--   0        0        0    17579 2024-05-07 11:30:35.990360 views_tensor_utilities-0.8.5/views_tensor_utilities/mappings.py
+-rw-r--r--   0        0        0    11099 2024-04-23 11:49:43.048800 views_tensor_utilities-0.8.5/views_tensor_utilities/objects.py
+-rw-r--r--   0        0        0     8805 1970-01-01 00:00:00.000000 views_tensor_utilities-0.8.5/PKG-INFO
```

### Comparing `views_tensor_utilities-0.8.4/README.md` & `views_tensor_utilities-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `views_tensor_utilities-0.8.4/views_tensor_utilities/mappings.py` & `views_tensor_utilities-0.8.5/views_tensor_utilities/mappings.py`

 * *Files 2% similar despite different names*

```diff
@@ -448,15 +448,15 @@
     time_space = TimeSpaceIndices.from_pandas(df)
 
     nfeature = len(df.columns)
 
     if df[df == dne].sum().sum() > 0:
         raise RuntimeError(f'does-not-exist token {dne} found in input data')
 
-    if dtype in defaults.allowed_float_types:
+    if dtype in defaults.allowed_float_types+defaults.allowed_int_types:
         tensor_time_space = np.full((time_space.ntime, time_space.nspace, nfeature), dne, dtype=dtype)
     else:
         tensor_time_space = np.full((time_space.ntime, time_space.nspace, nfeature), dne)
 
     for irow in range(time_space.nrow):
         idx = time_space.index_tuples[irow]
         itime = time_space.time_indices.index(idx[0])
```

### Comparing `views_tensor_utilities-0.8.4/views_tensor_utilities/objects.py` & `views_tensor_utilities-0.8.5/views_tensor_utilities/objects.py`

 * *Files identical despite different names*

### Comparing `views_tensor_utilities-0.8.4/PKG-INFO` & `views_tensor_utilities-0.8.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: views-tensor-utilities
-Version: 0.8.4
+Version: 0.8.5
 Summary: Classes and functions for transforming between VIEWS-compliant dfs and tensors
 Author: jimdale
 Author-email: jimdale@users.noreply.github.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.20.0)
 Requires-Dist: pandas (>=1.5.0)
 Description-Content-Type: text/markdown
 
 # views_tensor_utilities
```

