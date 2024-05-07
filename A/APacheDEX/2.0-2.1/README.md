# Comparing `tmp/APacheDEX-2.0.tar.gz` & `tmp/APacheDEX-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "APacheDEX-2.0.tar", last modified: Tue Jan  9 02:31:33 2024, max compression
+gzip compressed data, was "APacheDEX-2.1.tar", last modified: Tue May  7 06:19:34 2024, max compression
```

## Comparing `APacheDEX-2.0.tar` & `APacheDEX-2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2024-01-09 02:31:33.970023 APacheDEX-2.0/
-drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2024-01-09 02:31:33.970023 APacheDEX-2.0/APacheDEX.egg-info/
--rw-r--r--   0 vincent   (1000) vincent   (1000)    10609 2024-01-09 02:31:33.000000 APacheDEX-2.0/APacheDEX.egg-info/PKG-INFO
--rw-r--r--   0 vincent   (1000) vincent   (1000)      558 2024-01-09 02:31:33.000000 APacheDEX-2.0/APacheDEX.egg-info/SOURCES.txt
--rw-r--r--   0 vincent   (1000) vincent   (1000)        1 2024-01-09 02:31:33.000000 APacheDEX-2.0/APacheDEX.egg-info/dependency_links.txt
--rw-r--r--   0 vincent   (1000) vincent   (1000)       45 2024-01-09 02:31:33.000000 APacheDEX-2.0/APacheDEX.egg-info/entry_points.txt
--rw-r--r--   0 vincent   (1000) vincent   (1000)       10 2024-01-09 02:31:33.000000 APacheDEX-2.0/APacheDEX.egg-info/top_level.txt
--rw-r--r--   0 vincent   (1000) vincent   (1000)        1 2013-04-15 20:21:34.000000 APacheDEX-2.0/APacheDEX.egg-info/zip-safe
--rw-r--r--   0 vincent   (1000) vincent   (1000)    17987 2013-04-05 07:34:04.000000 APacheDEX-2.0/COPYING
--rw-r--r--   0 vincent   (1000) vincent   (1000)      236 2021-01-21 05:45:14.000000 APacheDEX-2.0/MANIFEST.in
--rw-r--r--   0 vincent   (1000) vincent   (1000)    10609 2024-01-09 02:31:33.970023 APacheDEX-2.0/PKG-INFO
--rw-r--r--   0 vincent   (1000) vincent   (1000)     9783 2019-05-28 07:53:52.000000 APacheDEX-2.0/README.rst
--rw-r--r--   0 vincent   (1000) vincent   (1000)      176 2013-04-23 20:16:21.000000 APacheDEX-2.0/TODO
-drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2024-01-09 02:31:33.970023 APacheDEX-2.0/apachedex/
--rwxr-xr-x   0 vincent   (1000) vincent   (1000)    65051 2024-01-09 02:23:46.000000 APacheDEX-2.0/apachedex/__init__.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)     1403 2023-12-27 06:34:51.000000 APacheDEX-2.0/apachedex/__main__.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)      495 2024-01-09 02:31:33.970023 APacheDEX-2.0/apachedex/_version.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)     1536 2013-04-07 20:23:47.000000 APacheDEX-2.0/apachedex/apachedex.css
--rw-r--r--   0 vincent   (1000) vincent   (1000)     2540 2019-05-28 07:53:52.000000 APacheDEX-2.0/apachedex/apachedex.js
--rw-r--r--   0 vincent   (1000) vincent   (1000)   228002 2019-05-28 07:46:39.000000 APacheDEX-2.0/apachedex/jquery-ui.js
--rw-r--r--   0 vincent   (1000) vincent   (1000)    17580 2019-05-28 07:46:27.000000 APacheDEX-2.0/apachedex/jquery.flot.axislabels.js
--rw-r--r--   0 vincent   (1000) vincent   (1000)   116087 2019-05-28 07:46:28.000000 APacheDEX-2.0/apachedex/jquery.flot.js
--rw-r--r--   0 vincent   (1000) vincent   (1000)    11679 2019-05-28 07:46:26.000000 APacheDEX-2.0/apachedex/jquery.flot.time.js
--rw-r--r--   0 vincent   (1000) vincent   (1000)    92629 2019-05-28 07:46:49.000000 APacheDEX-2.0/apachedex/jquery.js
--rw-r--r--   0 vincent   (1000) vincent   (1000)     7516 2023-12-27 05:01:42.000000 APacheDEX-2.0/apachedex/tests.py
--rwxr-xr-x   0 vincent   (1000) vincent   (1000)     1176 2023-12-27 04:57:20.000000 APacheDEX-2.0/parallel_parse.sh
--rw-r--r--   0 vincent   (1000) vincent   (1000)      206 2024-01-09 02:31:33.970023 APacheDEX-2.0/setup.cfg
--rw-r--r--   0 vincent   (1000) vincent   (1000)     2925 2024-01-09 02:29:21.000000 APacheDEX-2.0/setup.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)       36 2019-05-28 07:53:52.000000 APacheDEX-2.0/stdeb.cfg
--rw-r--r--   0 vincent   (1000) vincent   (1000)    68611 2021-01-21 05:45:14.000000 APacheDEX-2.0/versioneer.py
+drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-07 06:19:34.824711 APacheDEX-2.1/
+drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-07 06:19:34.824711 APacheDEX-2.1/APacheDEX.egg-info/
+-rw-r--r--   0 vincent   (1000) vincent   (1000)    10425 2024-05-07 06:19:34.000000 APacheDEX-2.1/APacheDEX.egg-info/PKG-INFO
+-rw-r--r--   0 vincent   (1000) vincent   (1000)      558 2024-05-07 06:19:34.000000 APacheDEX-2.1/APacheDEX.egg-info/SOURCES.txt
+-rw-r--r--   0 vincent   (1000) vincent   (1000)        1 2024-05-07 06:19:34.000000 APacheDEX-2.1/APacheDEX.egg-info/dependency_links.txt
+-rw-r--r--   0 vincent   (1000) vincent   (1000)       45 2024-05-07 06:19:34.000000 APacheDEX-2.1/APacheDEX.egg-info/entry_points.txt
+-rw-r--r--   0 vincent   (1000) vincent   (1000)       10 2024-05-07 06:19:34.000000 APacheDEX-2.1/APacheDEX.egg-info/top_level.txt
+-rw-r--r--   0 vincent   (1000) vincent   (1000)        1 2013-04-15 20:21:34.000000 APacheDEX-2.1/APacheDEX.egg-info/zip-safe
+-rw-r--r--   0 vincent   (1000) vincent   (1000)    17987 2013-04-05 07:34:04.000000 APacheDEX-2.1/COPYING
+-rw-r--r--   0 vincent   (1000) vincent   (1000)      236 2021-01-21 05:45:14.000000 APacheDEX-2.1/MANIFEST.in
+-rw-r--r--   0 vincent   (1000) vincent   (1000)    10425 2024-05-07 06:19:34.824711 APacheDEX-2.1/PKG-INFO
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     9599 2024-01-10 01:34:43.000000 APacheDEX-2.1/README.rst
+-rw-r--r--   0 vincent   (1000) vincent   (1000)      176 2013-04-23 20:16:21.000000 APacheDEX-2.1/TODO
+drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-07 06:19:34.824711 APacheDEX-2.1/apachedex/
+-rwxr-xr-x   0 vincent   (1000) vincent   (1000)    65020 2024-05-07 03:45:26.000000 APacheDEX-2.1/apachedex/__init__.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     1403 2023-12-27 06:34:51.000000 APacheDEX-2.1/apachedex/__main__.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)      495 2024-05-07 06:19:34.824711 APacheDEX-2.1/apachedex/_version.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     1536 2013-04-07 20:23:47.000000 APacheDEX-2.1/apachedex/apachedex.css
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     2540 2019-05-28 07:53:52.000000 APacheDEX-2.1/apachedex/apachedex.js
+-rw-r--r--   0 vincent   (1000) vincent   (1000)   228002 2019-05-28 07:46:39.000000 APacheDEX-2.1/apachedex/jquery-ui.js
+-rw-r--r--   0 vincent   (1000) vincent   (1000)    17580 2019-05-28 07:46:27.000000 APacheDEX-2.1/apachedex/jquery.flot.axislabels.js
+-rw-r--r--   0 vincent   (1000) vincent   (1000)   116087 2019-05-28 07:46:28.000000 APacheDEX-2.1/apachedex/jquery.flot.js
+-rw-r--r--   0 vincent   (1000) vincent   (1000)    11679 2019-05-28 07:46:26.000000 APacheDEX-2.1/apachedex/jquery.flot.time.js
+-rw-r--r--   0 vincent   (1000) vincent   (1000)    92629 2019-05-28 07:46:49.000000 APacheDEX-2.1/apachedex/jquery.js
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     7516 2023-12-27 05:01:42.000000 APacheDEX-2.1/apachedex/tests.py
+-rwxr-xr-x   0 vincent   (1000) vincent   (1000)     1176 2023-12-27 04:57:20.000000 APacheDEX-2.1/parallel_parse.sh
+-rw-r--r--   0 vincent   (1000) vincent   (1000)      206 2024-05-07 06:19:34.824711 APacheDEX-2.1/setup.cfg
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     2925 2024-01-09 02:29:21.000000 APacheDEX-2.1/setup.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)       36 2019-05-28 07:53:52.000000 APacheDEX-2.1/stdeb.cfg
+-rw-r--r--   0 vincent   (1000) vincent   (1000)    68611 2021-01-21 05:45:14.000000 APacheDEX-2.1/versioneer.py
```

### Comparing `APacheDEX-2.0/APacheDEX.egg-info/PKG-INFO` & `APacheDEX-2.1/APacheDEX.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: APacheDEX
-Version: 2.0
+Version: 2.1
 Summary: Compute APDEX from Apache-style logs.
 Home-page: https://lab.nexedi.com/nexedi/apachedex.git
 Author: Vincent Pelletier
 Author-email: vincent@nexedi.com
 License: GPL 2+
 Platform: any
 Classifier: Intended Audience :: Developers
@@ -91,18 +91,14 @@
 
 If you installed apachedex (using an egg or with a distribution's package) you
 should have them already.
 If you are running from repository, you need to fetch them first::
 
   python setup.py deps
 
-Also, apachedex can make use of backports.lzma
-(http://pypi.python.org/pypi/backports.lzma/) if it's installed to support xz
-file compression.
-
 Input
 -----
 
 All default "combined" log format fields are supported (more can easily be
 added), plus %D.
 
 Mandatory fields are (in any order) `%t`, `%r` (for request's URL), `%>s`,
@@ -111,15 +107,15 @@
 
 Input files may be provided uncompressed or compressed in:
 
 - bzip
 
 - gzip2
 
-- xz (if module backports.lzma is installed)
+- xz
 
 Input filename "-" is understood as stdin.
 
 Output
 ------
 
 The output is HTML + CSS + JS, so you need a web browser to read it.
```

### Comparing `APacheDEX-2.0/APacheDEX.egg-info/SOURCES.txt` & `APacheDEX-2.1/APacheDEX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `APacheDEX-2.0/COPYING` & `APacheDEX-2.1/COPYING`

 * *Files identical despite different names*

### Comparing `APacheDEX-2.0/PKG-INFO` & `APacheDEX-2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: APacheDEX
-Version: 2.0
+Version: 2.1
 Summary: Compute APDEX from Apache-style logs.
 Home-page: https://lab.nexedi.com/nexedi/apachedex.git
 Author: Vincent Pelletier
 Author-email: vincent@nexedi.com
 License: GPL 2+
 Platform: any
 Classifier: Intended Audience :: Developers
@@ -91,18 +91,14 @@
 
 If you installed apachedex (using an egg or with a distribution's package) you
 should have them already.
 If you are running from repository, you need to fetch them first::
 
   python setup.py deps
 
-Also, apachedex can make use of backports.lzma
-(http://pypi.python.org/pypi/backports.lzma/) if it's installed to support xz
-file compression.
-
 Input
 -----
 
 All default "combined" log format fields are supported (more can easily be
 added), plus %D.
 
 Mandatory fields are (in any order) `%t`, `%r` (for request's URL), `%>s`,
@@ -111,15 +107,15 @@
 
 Input files may be provided uncompressed or compressed in:
 
 - bzip
 
 - gzip2
 
-- xz (if module backports.lzma is installed)
+- xz
 
 Input filename "-" is understood as stdin.
 
 Output
 ------
 
 The output is HTML + CSS + JS, so you need a web browser to read it.
```

### Comparing `APacheDEX-2.0/README.rst` & `APacheDEX-2.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -68,18 +68,14 @@
 
 If you installed apachedex (using an egg or with a distribution's package) you
 should have them already.
 If you are running from repository, you need to fetch them first::
 
   python setup.py deps
 
-Also, apachedex can make use of backports.lzma
-(http://pypi.python.org/pypi/backports.lzma/) if it's installed to support xz
-file compression.
-
 Input
 -----
 
 All default "combined" log format fields are supported (more can easily be
 added), plus %D.
 
 Mandatory fields are (in any order) `%t`, `%r` (for request's URL), `%>s`,
@@ -88,15 +84,15 @@
 
 Input files may be provided uncompressed or compressed in:
 
 - bzip
 
 - gzip2
 
-- xz (if module backports.lzma is installed)
+- xz
 
 Input filename "-" is understood as stdin.
 
 Output
 ------
 
 The output is HTML + CSS + JS, so you need a web browser to read it.
```

### Comparing `APacheDEX-2.0/apachedex/__init__.py` & `APacheDEX-2.1/apachedex/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,15 +301,15 @@
 
   def accumulateFrom(self, other):
     for attribute in ('apdex_1', 'apdex_4', 'hit', 'duration_total'):
       setattr(self, attribute,
         getattr(self, attribute) + getattr(other, attribute))
     self.duration_max = max(self.duration_max, other.duration_max)
     if self.enable_median:
-      self.duration_list = itertools.chain(self.duration_list, other.duration_list)
+      self.duration_list.extend(other.duration_list)
 
   def getApdex(self):
     if self.hit:
       return (self.apdex_1 + self.apdex_4 * .5) / self.hit
     return 1
 
   def getAverage(self):
```

### Comparing `APacheDEX-2.0/apachedex/__main__.py` & `APacheDEX-2.1/apachedex/__main__.py`

 * *Files identical despite different names*

### Comparing `APacheDEX-2.0/apachedex/apachedex.css` & `APacheDEX-2.1/apachedex/apachedex.css`

 * *Files identical despite different names*

### Comparing `APacheDEX-2.0/apachedex/apachedex.js` & `APacheDEX-2.1/apachedex/apachedex.js`

 * *Files identical despite different names*

### Comparing `APacheDEX-2.0/apachedex/jquery-ui.js` & `APacheDEX-2.1/apachedex/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `APacheDEX-2.0/apachedex/jquery.flot.axislabels.js` & `APacheDEX-2.1/apachedex/jquery.flot.axislabels.js`

 * *Files identical despite different names*

### Comparing `APacheDEX-2.0/apachedex/jquery.flot.js` & `APacheDEX-2.1/apachedex/jquery.flot.js`

 * *Files identical despite different names*

### Comparing `APacheDEX-2.0/apachedex/jquery.flot.time.js` & `APacheDEX-2.1/apachedex/jquery.flot.time.js`

 * *Files identical despite different names*

### Comparing `APacheDEX-2.0/apachedex/jquery.js` & `APacheDEX-2.1/apachedex/jquery.js`

 * *Files identical despite different names*

### Comparing `APacheDEX-2.0/apachedex/tests.py` & `APacheDEX-2.1/apachedex/tests.py`

 * *Files identical despite different names*

### Comparing `APacheDEX-2.0/parallel_parse.sh` & `APacheDEX-2.1/parallel_parse.sh`

 * *Files identical despite different names*

### Comparing `APacheDEX-2.0/setup.py` & `APacheDEX-2.1/setup.py`

 * *Files identical despite different names*

### Comparing `APacheDEX-2.0/versioneer.py` & `APacheDEX-2.1/versioneer.py`

 * *Files identical despite different names*

