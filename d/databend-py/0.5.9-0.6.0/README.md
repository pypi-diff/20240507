# Comparing `tmp/databend-py-0.5.9.tar.gz` & `tmp/databend-py-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databend-py-0.5.9.tar", last modified: Fri Apr 26 08:22:16 2024, max compression
+gzip compressed data, was "databend-py-0.6.0.tar", last modified: Tue May  7 00:37:08 2024, max compression
```

## Comparing `databend-py-0.5.9.tar` & `databend-py-0.6.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:22:16.938605 databend-py-0.5.9/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 08:22:04.000000 databend-py-0.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-26 08:22:04.000000 databend-py-0.5.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-26 08:22:16.938605 databend-py-0.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-26 08:22:04.000000 databend-py-0.5.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:22:16.938605 databend-py-0.5.9/databend_py/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11151 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10215 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/datetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/defines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/sdk_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:22:16.938605 databend-py-0.5.9/databend_py/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/util/escape.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/util/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:22:16.938605 databend-py-0.5.9/databend_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-26 08:22:16.000000 databend-py-0.5.9/databend_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-26 08:22:16.000000 databend-py-0.5.9/databend_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 08:22:16.000000 databend-py-0.5.9/databend_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-26 08:22:16.000000 databend-py-0.5.9/databend_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 08:22:16.000000 databend-py-0.5.9/databend_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-26 08:22:16.938605 databend-py-0.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-26 08:22:04.000000 databend-py-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:37:08.604370 databend-py-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 00:36:51.000000 databend-py-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 00:36:51.000000 databend-py-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-07 00:37:08.604370 databend-py-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-07 00:36:51.000000 databend-py-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:37:08.600370 databend-py-0.6.0/databend_py/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 00:36:51.000000 databend-py-0.6.0/databend_py/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-07 00:36:51.000000 databend-py-0.6.0/databend_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11151 2024-05-07 00:36:51.000000 databend-py-0.6.0/databend_py/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10215 2024-05-07 00:36:51.000000 databend-py-0.6.0/databend_py/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-07 00:36:51.000000 databend-py-0.6.0/databend_py/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-07 00:36:51.000000 databend-py-0.6.0/databend_py/datetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-07 00:36:51.000000 databend-py-0.6.0/databend_py/defines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-07 00:36:51.000000 databend-py-0.6.0/databend_py/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-07 00:36:51.000000 databend-py-0.6.0/databend_py/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-07 00:36:51.000000 databend-py-0.6.0/databend_py/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-07 00:36:51.000000 databend-py-0.6.0/databend_py/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-07 00:36:51.000000 databend-py-0.6.0/databend_py/sdk_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-05-07 00:36:51.000000 databend-py-0.6.0/databend_py/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:37:08.600370 databend-py-0.6.0/databend_py/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 00:36:51.000000 databend-py-0.6.0/databend_py/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-07 00:36:51.000000 databend-py-0.6.0/databend_py/util/escape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-07 00:36:51.000000 databend-py-0.6.0/databend_py/util/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:37:08.600370 databend-py-0.6.0/databend_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-07 00:37:07.000000 databend-py-0.6.0/databend_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-07 00:37:07.000000 databend-py-0.6.0/databend_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 00:37:07.000000 databend-py-0.6.0/databend_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-07 00:37:07.000000 databend-py-0.6.0/databend_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 00:37:07.000000 databend-py-0.6.0/databend_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-07 00:37:08.604370 databend-py-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-07 00:36:51.000000 databend-py-0.6.0/setup.py
```

### Comparing `databend-py-0.5.9/LICENSE` & `databend-py-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `databend-py-0.5.9/PKG-INFO` & `databend-py-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databend-py
-Version: 0.5.9
+Version: 0.6.0
 Summary: Python driver with native interface for Databend
 Home-page: https://github.com/databendcloud/databend-py
 Author: Databend Cloud Team
 Author-email: hantmac@outlook.com
 License: Apache License
 Keywords: databend db database cloud analytics
 Platform: UNKNOWN
```

### Comparing `databend-py-0.5.9/README.md` & `databend-py-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `databend-py-0.5.9/databend_py/__init__.py` & `databend-py-0.6.0/databend_py/__init__.py`

 * *Files identical despite different names*

### Comparing `databend-py-0.5.9/databend_py/client.py` & `databend-py-0.6.0/databend_py/client.py`

 * *Files identical despite different names*

### Comparing `databend-py-0.5.9/databend_py/connection.py` & `databend-py-0.6.0/databend_py/connection.py`

 * *Files identical despite different names*

### Comparing `databend-py-0.5.9/databend_py/context.py` & `databend-py-0.6.0/databend_py/context.py`

 * *Files identical despite different names*

### Comparing `databend-py-0.5.9/databend_py/datetypes.py` & `databend-py-0.6.0/databend_py/datetypes.py`

 * *Files identical despite different names*

### Comparing `databend-py-0.5.9/databend_py/errors.py` & `databend-py-0.6.0/databend_py/errors.py`

 * *Files identical despite different names*

### Comparing `databend-py-0.5.9/databend_py/result.py` & `databend-py-0.6.0/databend_py/result.py`

 * *Files identical despite different names*

### Comparing `databend-py-0.5.9/databend_py/retry.py` & `databend-py-0.6.0/databend_py/retry.py`

 * *Files identical despite different names*

### Comparing `databend-py-0.5.9/databend_py/uploader.py` & `databend-py-0.6.0/databend_py/uploader.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,19 +68,19 @@
 
     def _serialize_data(self, data, compress):
         # In Python3 csv.writer expects a file-like object opened in text mode. In Python2, csv.writer expects a file-like object opened in binary mode.
         start_time = time.time()
         buf = io.StringIO()
         csvwriter = csv.writer(buf, delimiter=',', quoting=csv.QUOTE_MINIMAL)
         csvwriter.writerows(data)
-        output = buf.getvalue()
+        output = buf.getvalue().encode('utf-8')
         if compress:
             buf = io.BytesIO()
             with gzip.GzipFile(fileobj=buf, mode="wb") as gzwriter:
-                gzwriter.write(output.encode('utf-8'))
+                gzwriter.write(output)
             output = buf.getvalue()
         if self._debug:
             print('upload:_serialize_data %s' % (time.time() - start_time))
         return output
 
     def _upload_to_presigned_url(self, presigned_url, headers, data):
         # Check if data is bytes or File
```

### Comparing `databend-py-0.5.9/databend_py/util/escape.py` & `databend-py-0.6.0/databend_py/util/escape.py`

 * *Files identical despite different names*

### Comparing `databend-py-0.5.9/databend_py/util/helper.py` & `databend-py-0.6.0/databend_py/util/helper.py`

 * *Files identical despite different names*

### Comparing `databend-py-0.5.9/databend_py.egg-info/PKG-INFO` & `databend-py-0.6.0/databend_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databend-py
-Version: 0.5.9
+Version: 0.6.0
 Summary: Python driver with native interface for Databend
 Home-page: https://github.com/databendcloud/databend-py
 Author: Databend Cloud Team
 Author-email: hantmac@outlook.com
 License: Apache License
 Keywords: databend db database cloud analytics
 Platform: UNKNOWN
```

### Comparing `databend-py-0.5.9/databend_py.egg-info/SOURCES.txt` & `databend-py-0.6.0/databend_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `databend-py-0.5.9/setup.py` & `databend-py-0.6.0/setup.py`

 * *Files identical despite different names*

