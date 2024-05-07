# Comparing `tmp/bondzai.davinsy-py-0.0.8.tar.gz` & `tmp/bondzai.davinsy-py-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.davinsy-py-0.0.8.tar", last modified: Mon Oct 23 14:48:23 2023, max compression
+gzip compressed data, was "bondzai.davinsy-py-0.0.9.tar", last modified: Mon Oct 30 16:29:39 2023, max compression
```

## Comparing `bondzai.davinsy-py-0.0.8.tar` & `bondzai.davinsy-py-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 14:48:23.669901 bondzai.davinsy-py-0.0.8/
--rw-r--r--   0 root         (0) root         (0)      547 2023-10-23 14:47:34.000000 bondzai.davinsy-py-0.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)      491 2023-10-23 14:48:23.669901 bondzai.davinsy-py-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       72 2023-10-23 14:47:34.000000 bondzai.davinsy-py-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 14:48:23.669901 bondzai.davinsy-py-0.0.8/bondzai/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 14:48:23.669901 bondzai.davinsy-py-0.0.8/bondzai/davinsy_py/
--rw-r--r--   0 root         (0) root         (0)       24 2023-10-23 14:47:34.000000 bondzai.davinsy-py-0.0.8/bondzai/davinsy_py/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4317 2023-10-23 14:47:34.000000 bondzai.davinsy-py-0.0.8/bondzai/davinsy_py/davinsy.py
--rw-r--r--   0 root         (0) root         (0)     8966 2023-10-23 14:47:34.000000 bondzai.davinsy-py-0.0.8/bondzai/davinsy_py/enums.py
--rw-r--r--   0 root         (0) root         (0)      332 2023-10-23 14:47:34.000000 bondzai.davinsy-py-0.0.8/bondzai/davinsy_py/logger.py
--rw-r--r--   0 root         (0) root         (0)    21854 2023-10-23 14:47:34.000000 bondzai.davinsy-py-0.0.8/bondzai/davinsy_py/model.py
--rw-r--r--   0 root         (0) root         (0)    38613 2023-10-23 14:47:34.000000 bondzai.davinsy-py-0.0.8/bondzai/davinsy_py/operations.py
--rw-r--r--   0 root         (0) root         (0)     3188 2023-10-23 14:47:34.000000 bondzai.davinsy-py-0.0.8/bondzai/davinsy_py/preproc.py
--rw-r--r--   0 root         (0) root         (0)     1034 2023-10-23 14:47:34.000000 bondzai.davinsy-py-0.0.8/bondzai/davinsy_py/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 14:48:23.669901 bondzai.davinsy-py-0.0.8/bondzai.davinsy_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)      491 2023-10-23 14:48:23.000000 bondzai.davinsy-py-0.0.8/bondzai.davinsy_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      591 2023-10-23 14:48:23.000000 bondzai.davinsy-py-0.0.8/bondzai.davinsy_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-23 14:48:23.000000 bondzai.davinsy-py-0.0.8/bondzai.davinsy_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-10-23 14:48:23.000000 bondzai.davinsy-py-0.0.8/bondzai.davinsy_py.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-10-23 14:48:23.000000 bondzai.davinsy-py-0.0.8/bondzai.davinsy_py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-10-23 14:48:23.000000 bondzai.davinsy-py-0.0.8/bondzai.davinsy_py.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-23 14:48:23.000000 bondzai.davinsy-py-0.0.8/bondzai.davinsy_py.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)       71 2023-10-23 14:47:34.000000 bondzai.davinsy-py-0.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      700 2023-10-23 14:48:23.669901 bondzai.davinsy-py-0.0.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-30 16:29:39.247107 bondzai.davinsy-py-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)      547 2023-10-30 16:28:22.000000 bondzai.davinsy-py-0.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)      491 2023-10-30 16:29:39.247107 bondzai.davinsy-py-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       72 2023-10-30 16:28:22.000000 bondzai.davinsy-py-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-30 16:29:39.247107 bondzai.davinsy-py-0.0.9/bondzai/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-30 16:29:39.247107 bondzai.davinsy-py-0.0.9/bondzai/davinsy_py/
+-rw-r--r--   0 root         (0) root         (0)       24 2023-10-30 16:29:29.000000 bondzai.davinsy-py-0.0.9/bondzai/davinsy_py/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4317 2023-10-30 16:28:22.000000 bondzai.davinsy-py-0.0.9/bondzai/davinsy_py/davinsy.py
+-rw-r--r--   0 root         (0) root         (0)     8996 2023-10-30 16:29:29.000000 bondzai.davinsy-py-0.0.9/bondzai/davinsy_py/enums.py
+-rw-r--r--   0 root         (0) root         (0)      332 2023-10-30 16:28:22.000000 bondzai.davinsy-py-0.0.9/bondzai/davinsy_py/logger.py
+-rw-r--r--   0 root         (0) root         (0)    21854 2023-10-30 16:28:22.000000 bondzai.davinsy-py-0.0.9/bondzai/davinsy_py/model.py
+-rw-r--r--   0 root         (0) root         (0)    39013 2023-10-30 16:29:29.000000 bondzai.davinsy-py-0.0.9/bondzai/davinsy_py/operations.py
+-rw-r--r--   0 root         (0) root         (0)     3188 2023-10-30 16:28:22.000000 bondzai.davinsy-py-0.0.9/bondzai/davinsy_py/preproc.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-10-30 16:28:22.000000 bondzai.davinsy-py-0.0.9/bondzai/davinsy_py/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-30 16:29:39.247107 bondzai.davinsy-py-0.0.9/bondzai.davinsy_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      491 2023-10-30 16:29:39.000000 bondzai.davinsy-py-0.0.9/bondzai.davinsy_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      591 2023-10-30 16:29:39.000000 bondzai.davinsy-py-0.0.9/bondzai.davinsy_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-30 16:29:39.000000 bondzai.davinsy-py-0.0.9/bondzai.davinsy_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-10-30 16:29:39.000000 bondzai.davinsy-py-0.0.9/bondzai.davinsy_py.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-10-30 16:29:39.000000 bondzai.davinsy-py-0.0.9/bondzai.davinsy_py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-10-30 16:29:39.000000 bondzai.davinsy-py-0.0.9/bondzai.davinsy_py.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-30 16:29:39.000000 bondzai.davinsy-py-0.0.9/bondzai.davinsy_py.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)       71 2023-10-30 16:28:22.000000 bondzai.davinsy-py-0.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      700 2023-10-30 16:29:39.247107 bondzai.davinsy-py-0.0.9/setup.cfg
```

### Comparing `bondzai.davinsy-py-0.0.8/NOTICE` & `bondzai.davinsy-py-0.0.9/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.8/bondzai/davinsy_py/davinsy.py` & `bondzai.davinsy-py-0.0.9/bondzai/davinsy_py/davinsy.py`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.8/bondzai/davinsy_py/enums.py` & `bondzai.davinsy-py-0.0.9/bondzai/davinsy_py/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     EVT_EXT_CUSTOM_8 = 0xF07
     EVT_EXT_CUSTOM_9 = 0xF08
     EVT_EXT_CUSTOM_10 = 0xF09
     EVT_INT_EXCEPTION = 0x1000
     EVT_INT_DATA_STORED = 0x1001
     EVT_INT_DISCOVERY = 0x1002
     EVT_INT_TRANSPORT = 0x1003
+    EVT_INT_OVERFLOW = 0x1004
     EVT_INT_DATA_UPDATED = 0x1100
     EVT_INT_READY_TO_PREPROC_BATCH = 0x1101
     EVT_INT_PREPROC_BATCH_DONE = 0x1102
     EVT_INT_TRIGGER_NEXT = 0x1103
     EVT_INT_FINAL = 0x1104
     EVT_INT_READY_TO_PREPROC_SINGLE = 0x1105
     EVT_INT_PREPROC_SINGLE_DONE = 0x1106
```

### Comparing `bondzai.davinsy-py-0.0.8/bondzai/davinsy_py/model.py` & `bondzai.davinsy-py-0.0.9/bondzai/davinsy_py/model.py`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.8/bondzai/davinsy_py/operations.py` & `bondzai.davinsy-py-0.0.9/bondzai/davinsy_py/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,16 +135,16 @@
          data=0,
         _=(c_float * lenvect)(*dataoutArray.flatten())
     )
     return outvect
 
 def VECTOR2DF32_from_pyListOfList(dataoutList):
     dim = [0,0]
-    dim[1] = len(dataoutList)
-    dim[0] = len(dataoutList[0])
+    dim[0] = len(dataoutList)
+    dim[1] = len(dataoutList[0])
 
     dataoutListFlatten = []
     for l in dataoutList:
         dataoutListFlatten += l
 
     lenvect = np.prod(dim)
     outvect = VECTOR2DF32_factory(lenvect)(
@@ -682,16 +682,22 @@
         # cast_paramspan
         # update size
         sizeBytes = parameters["size"]
         span_lenx = int(parameters["span_lenx"] )
         span_leny = int(parameters["span_leny"])
         sizeData = span_lenx*span_leny* 4
 
+        if (span_lenx%2) != 0:
+            logger.warn("Node : Parameters for Power Span might be incorrect, Span X must be a multiple of 2")
+        if len(parameters["span_data"]) != span_lenx*span_leny :
+            l = len(parameters["span_data"])
+            logger.warn(f"Node : Parameters for Power Span might be incorrect,  {span_lenx} by {span_leny}  different from span data: {l}")
+
         if sizeBytes <= 32 : # 64bits pointer
-            logger.warn(f"Overwrite PWSPAN Size with {span_lenx} by {span_leny} = {sizeData} bytes")
+            logger.debug(f"Overwrite PWSPAN Size with {span_lenx} by {span_leny} = {sizeData} bytes")
             sizeBytes += sizeData
 
         res = CALLPARAMS(
             param_pwspan=CPARAMSPAN(
                 typeid=parameters["typeid"],  # 4 Bytes
                 size=sizeBytes,               # 4 Bytes
                 mode=parameters["mode"],      # 4 Bytes
```

### Comparing `bondzai.davinsy-py-0.0.8/bondzai/davinsy_py/preproc.py` & `bondzai.davinsy-py-0.0.9/bondzai/davinsy_py/preproc.py`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.8/bondzai/davinsy_py/utils.py` & `bondzai.davinsy-py-0.0.9/bondzai/davinsy_py/utils.py`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.8/bondzai.davinsy_py.egg-info/SOURCES.txt` & `bondzai.davinsy-py-0.0.9/bondzai.davinsy_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.8/setup.cfg` & `bondzai.davinsy-py-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 	=.
 packages = find_namespace:
 zip_safe = True
 include_package_data = True
 namespace_packages = 
 	bondzai
 install_requires = 
-	numpy==1.24.3
+	numpy>=1.24.3
 	pyyaml==6.0
 
 [options.packages.find]
 where = .
 
 [egg_info]
 tag_build =
```

