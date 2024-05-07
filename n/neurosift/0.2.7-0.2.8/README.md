# Comparing `tmp/neurosift-0.2.7.tar.gz` & `tmp/neurosift-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurosift-0.2.7.tar", last modified: Fri Apr 12 15:28:54 2024, max compression
+gzip compressed data, was "neurosift-0.2.8.tar", last modified: Tue May  7 15:47:11 2024, max compression
```

## Comparing `neurosift-0.2.7.tar` & `neurosift-0.2.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-04-12 15:28:54.011087 neurosift-0.2.7/
--rw-rw-r--   0 magland   (1000) magland   (1000)      103 2024-02-25 01:27:01.000000 neurosift-0.2.7/MANIFEST.in
--rw-r--r--   0 magland   (1000) magland   (1000)     1014 2024-04-12 15:28:54.011087 neurosift-0.2.7/PKG-INFO
--rw-rw-r--   0 magland   (1000) magland   (1000)      471 2024-02-25 01:27:01.000000 neurosift-0.2.7/README.md
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-04-12 15:28:54.007087 neurosift-0.2.7/neurosift/
--rw-rw-r--   0 magland   (1000) magland   (1000)     1446 2023-12-22 21:08:36.000000 neurosift-0.2.7/neurosift/TemporaryDirectory.py
--rw-rw-r--   0 magland   (1000) magland   (1000)        0 2024-02-01 21:59:30.000000 neurosift-0.2.7/neurosift/__init__.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     3050 2024-03-05 14:15:17.000000 neurosift-0.2.7/neurosift/cli.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-04-12 15:28:54.007087 neurosift-0.2.7/neurosift/codecs/
--rw-rw-r--   0 magland   (1000) magland   (1000)     3104 2024-04-12 15:28:02.000000 neurosift-0.2.7/neurosift/codecs/MP4AVCCodec.py
--rw-rw-r--   0 magland   (1000) magland   (1000)       51 2024-04-04 10:50:34.000000 neurosift-0.2.7/neurosift/codecs/__init__.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-04-12 15:28:54.007087 neurosift-0.2.7/neurosift/local-file-access-js/
--rw-rw-r--   0 magland   (1000) magland   (1000)      318 2024-02-25 01:27:01.000000 neurosift-0.2.7/neurosift/local-file-access-js/package.json
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-04-12 15:28:54.007087 neurosift-0.2.7/neurosift/local-file-access-js/src/
--rw-rw-r--   0 magland   (1000) magland   (1000)     2189 2024-03-05 14:13:19.000000 neurosift-0.2.7/neurosift/local-file-access-js/src/index.js
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-04-12 15:28:54.011087 neurosift-0.2.7/neurosift.egg-info/
--rw-r--r--   0 magland   (1000) magland   (1000)     1014 2024-04-12 15:28:53.000000 neurosift-0.2.7/neurosift.egg-info/PKG-INFO
--rw-rw-r--   0 magland   (1000) magland   (1000)      460 2024-04-12 15:28:53.000000 neurosift-0.2.7/neurosift.egg-info/SOURCES.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)        1 2024-04-12 15:28:53.000000 neurosift-0.2.7/neurosift.egg-info/dependency_links.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)       54 2024-04-12 15:28:53.000000 neurosift-0.2.7/neurosift.egg-info/entry_points.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)        6 2024-04-12 15:28:53.000000 neurosift-0.2.7/neurosift.egg-info/requires.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)       10 2024-04-12 15:28:53.000000 neurosift-0.2.7/neurosift.egg-info/top_level.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)      528 2024-04-12 15:28:54.011087 neurosift-0.2.7/setup.cfg
--rw-rw-r--   0 magland   (1000) magland   (1000)      509 2024-02-25 01:27:01.000000 neurosift-0.2.7/setup.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-05-07 15:47:11.239995 neurosift-0.2.8/
+-rw-rw-r--   0 magland   (1000) magland   (1000)      103 2024-02-25 01:27:01.000000 neurosift-0.2.8/MANIFEST.in
+-rw-r--r--   0 magland   (1000) magland   (1000)     1014 2024-05-07 15:47:11.239995 neurosift-0.2.8/PKG-INFO
+-rw-rw-r--   0 magland   (1000) magland   (1000)      471 2024-02-25 01:27:01.000000 neurosift-0.2.8/README.md
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-05-07 15:47:11.239995 neurosift-0.2.8/neurosift/
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1446 2023-12-22 21:08:36.000000 neurosift-0.2.8/neurosift/TemporaryDirectory.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)        0 2024-02-01 21:59:30.000000 neurosift-0.2.8/neurosift/__init__.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     3050 2024-03-05 14:15:17.000000 neurosift-0.2.8/neurosift/cli.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-05-07 15:47:11.239995 neurosift-0.2.8/neurosift/codecs/
+-rw-rw-r--   0 magland   (1000) magland   (1000)     3104 2024-04-12 15:28:02.000000 neurosift-0.2.8/neurosift/codecs/MP4AVCCodec.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)       51 2024-04-04 10:50:34.000000 neurosift-0.2.8/neurosift/codecs/__init__.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-05-07 15:47:11.239995 neurosift-0.2.8/neurosift/local-file-access-js/
+-rw-rw-r--   0 magland   (1000) magland   (1000)      318 2024-02-25 01:27:01.000000 neurosift-0.2.8/neurosift/local-file-access-js/package.json
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-05-07 15:47:11.239995 neurosift-0.2.8/neurosift/local-file-access-js/src/
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2228 2024-05-07 15:42:10.000000 neurosift-0.2.8/neurosift/local-file-access-js/src/index.js
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-05-07 15:47:11.239995 neurosift-0.2.8/neurosift.egg-info/
+-rw-r--r--   0 magland   (1000) magland   (1000)     1014 2024-05-07 15:47:11.000000 neurosift-0.2.8/neurosift.egg-info/PKG-INFO
+-rw-rw-r--   0 magland   (1000) magland   (1000)      460 2024-05-07 15:47:11.000000 neurosift-0.2.8/neurosift.egg-info/SOURCES.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)        1 2024-05-07 15:47:11.000000 neurosift-0.2.8/neurosift.egg-info/dependency_links.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)       54 2024-05-07 15:47:11.000000 neurosift-0.2.8/neurosift.egg-info/entry_points.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)        6 2024-05-07 15:47:11.000000 neurosift-0.2.8/neurosift.egg-info/requires.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)       10 2024-05-07 15:47:11.000000 neurosift-0.2.8/neurosift.egg-info/top_level.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)      528 2024-05-07 15:47:11.243995 neurosift-0.2.8/setup.cfg
+-rw-rw-r--   0 magland   (1000) magland   (1000)      509 2024-02-25 01:27:01.000000 neurosift-0.2.8/setup.py
```

### Comparing `neurosift-0.2.7/PKG-INFO` & `neurosift-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurosift
-Version: 0.2.7
+Version: 0.2.8
 Summary: Simple utility to view local NWB files using Neurosift
 Home-page: https://github.com/flatironinstitute/neurosift
 Author: Jeremy Magland
 Author-email: jmagland@flatironinstitute.org
 Project-URL: Bug Tracker, https://github.com/flatironinstitute/neurosift/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `neurosift-0.2.7/neurosift/TemporaryDirectory.py` & `neurosift-0.2.8/neurosift/TemporaryDirectory.py`

 * *Files identical despite different names*

### Comparing `neurosift-0.2.7/neurosift/cli.py` & `neurosift-0.2.8/neurosift/cli.py`

 * *Files identical despite different names*

### Comparing `neurosift-0.2.7/neurosift/codecs/MP4AVCCodec.py` & `neurosift-0.2.8/neurosift/codecs/MP4AVCCodec.py`

 * *Files identical despite different names*

### Comparing `neurosift-0.2.7/neurosift/local-file-access-js/src/index.js` & `neurosift-0.2.8/neurosift/local-file-access-js/src/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -4,16 +4,16 @@
 const dir = process.argv[2]
 if (!dir) {
     console.error('Please specify a directory.')
     process.exit(-1)
 }
 console.info('Serving files in', dir)
 
-// Allow CORS from flatironinstitute.github.io and localhost:3000
-const allowedOrigins = ['https://flatironinstitute.github.io', 'http://localhost:3000', 'http://localhost:4200']
+// Allow CORS from neurosift.app flatironinstitute.github.io and localhost:3000
+const allowedOrigins = ['https://neurosift.app', 'https://flatironinstitute.github.io', 'http://localhost:3000', 'http://localhost:4200']
 app.use((req, resp, next) => {
     const origin = req.get('origin')
     const allowedOrigin = allowedOrigins.includes(origin) ? origin : undefined
     if (allowedOrigin) {
         resp.header('Access-Control-Allow-Origin', allowedOrigin)
         resp.header('Access-Control-Allow-Headers', "Origin, X-Requested-With, Content-Type, Accept, Range")
     }
```

### Comparing `neurosift-0.2.7/neurosift.egg-info/PKG-INFO` & `neurosift-0.2.8/neurosift.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurosift
-Version: 0.2.7
+Version: 0.2.8
 Summary: Simple utility to view local NWB files using Neurosift
 Home-page: https://github.com/flatironinstitute/neurosift
 Author: Jeremy Magland
 Author-email: jmagland@flatironinstitute.org
 Project-URL: Bug Tracker, https://github.com/flatironinstitute/neurosift/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `neurosift-0.2.7/setup.cfg` & `neurosift-0.2.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = neurosift
-version = 0.2.7
+version = 0.2.8
 author = Jeremy Magland
 author_email = jmagland@flatironinstitute.org
 description = Simple utility to view local NWB files using Neurosift
 url = https://github.com/flatironinstitute/neurosift
 include_package_data = True
 project_urls = 
 	Bug Tracker = https://github.com/flatironinstitute/neurosift/issues
```

