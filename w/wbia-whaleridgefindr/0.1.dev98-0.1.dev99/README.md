# Comparing `tmp/wbia_whaleridgefindr-0.1.dev98-py3-none-any.whl.zip` & `tmp/wbia_whaleridgefindr-0.1.dev99-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 17507 bytes, number of entries: 8
--rw-r--r--  2.0 unx      183 b- defN 23-Aug-28 08:51 wbia-whaleridgefindr/__init__.py
--rw-r--r--  2.0 unx    43646 b- defN 23-Aug-28 08:51 wbia-whaleridgefindr/_plugin.py
--rw-r--r--  2.0 unx       25 b- defN 23-Aug-28 08:52 wbia-whaleridgefindr/_version.py
--rwxr-xr-x  2.0 unx    11324 b- defN 23-Aug-28 08:52 wbia_whaleridgefindr-0.1.dev98.dist-info/LICENSE
--rw-r--r--  2.0 unx     5684 b- defN 23-Aug-28 08:52 wbia_whaleridgefindr-0.1.dev98.dist-info/METADATA
--rw-r--r--  2.0 unx       86 b- defN 23-Aug-28 08:52 wbia_whaleridgefindr-0.1.dev98.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-Aug-28 08:52 wbia_whaleridgefindr-0.1.dev98.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      736 b- defN 23-Aug-28 08:52 wbia_whaleridgefindr-0.1.dev98.dist-info/RECORD
-8 files, 61705 bytes uncompressed, 16199 bytes compressed:  73.7%
+Zip file size: 17510 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      183 b- defN 23-Aug-28 08:52 wbia-whaleridgefindr/__init__.py
+-rw-r--r--  2.0 unx    43646 b- defN 23-Aug-28 08:52 wbia-whaleridgefindr/_plugin.py
+-rw-r--r--  2.0 unx       25 b- defN 23-Aug-28 08:53 wbia-whaleridgefindr/_version.py
+-rwxr-xr-x  2.0 unx    11324 b- defN 23-Aug-28 08:53 wbia_whaleridgefindr-0.1.dev99.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5684 b- defN 23-Aug-28 08:53 wbia_whaleridgefindr-0.1.dev99.dist-info/METADATA
+-rw-r--r--  2.0 unx       86 b- defN 23-Aug-28 08:53 wbia_whaleridgefindr-0.1.dev99.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-Aug-28 08:53 wbia_whaleridgefindr-0.1.dev99.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      736 b- defN 23-Aug-28 08:53 wbia_whaleridgefindr-0.1.dev99.dist-info/RECORD
+8 files, 61705 bytes uncompressed, 16202 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: wbia-whaleridgefindr/_plugin.py
 Comment: 
 
 Filename: wbia-whaleridgefindr/_version.py
 Comment: 
 
-Filename: wbia_whaleridgefindr-0.1.dev98.dist-info/LICENSE
+Filename: wbia_whaleridgefindr-0.1.dev99.dist-info/LICENSE
 Comment: 
 
-Filename: wbia_whaleridgefindr-0.1.dev98.dist-info/METADATA
+Filename: wbia_whaleridgefindr-0.1.dev99.dist-info/METADATA
 Comment: 
 
-Filename: wbia_whaleridgefindr-0.1.dev98.dist-info/WHEEL
+Filename: wbia_whaleridgefindr-0.1.dev99.dist-info/WHEEL
 Comment: 
 
-Filename: wbia_whaleridgefindr-0.1.dev98.dist-info/top_level.txt
+Filename: wbia_whaleridgefindr-0.1.dev99.dist-info/top_level.txt
 Comment: 
 
-Filename: wbia_whaleridgefindr-0.1.dev98.dist-info/RECORD
+Filename: wbia_whaleridgefindr-0.1.dev99.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wbia-whaleridgefindr/__init__.py

```diff
@@ -1,7 +1,7 @@
 # -*- coding: utf-8 -*-
 try:
     from wbia-whaleridgefindr._version import __version__
 except ImportError:
-    __version__ = '0.0.0'
+    __version__ = '0.1.1'
 
 from wbia-whaleridgefindr import _plugin  # NOQA
```

## wbia-whaleridgefindr/_version.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.dev98"
+__version__ = "0.1.dev99"
```

## Comparing `wbia_whaleridgefindr-0.1.dev98.dist-info/LICENSE` & `wbia_whaleridgefindr-0.1.dev99.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `wbia_whaleridgefindr-0.1.dev98.dist-info/METADATA` & `wbia_whaleridgefindr-0.1.dev99.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbia-whaleridgefindr
-Version: 0.1.dev98
+Version: 0.1.dev99
 Summary: wbia-whaleridgefindr - A plug-in for the finFindR gray whale ID algorithm
 Home-page: https://github.com/WildbookOrg/wbia-plugin-whaleridgefindr
 Author: Jason Parham
 Author-email: info@wildme.org
 License: Apache Version 2.0
 Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: BSD License
```

