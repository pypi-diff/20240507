# Comparing `tmp/eyelogic_sdk-1.1.6-py3-none-any.whl.zip` & `tmp/eyelogic_sdk-1.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,9 @@
-Zip file size: 880476 bytes, number of entries: 15
--rw-rw-rw-  2.0 fat   653224 b- defN 22-Dec-16 14:54 eyelogic/ELApi.dll
--rw-rw-rw-  2.0 fat    29291 b- defN 22-Nov-30 15:43 eyelogic/ELApi.py
--rw-rw-rw-  2.0 fat   247720 b- defN 22-Dec-16 14:54 eyelogic/ELCApi.dll
--rw-rw-rw-  2.0 fat     1168 b- defN 22-Dec-16 14:51 eyelogic/__init__.py
--rw-rw-rw-  2.0 fat   315784 b- defN 21-Aug-03 10:07 eyelogic/concrt140.dll
--rw-rw-rw-  2.0 fat   565640 b- defN 21-Aug-03 10:07 eyelogic/msvcp140.dll
--rw-rw-rw-  2.0 fat    23944 b- defN 21-Aug-03 10:07 eyelogic/msvcp140_1.dll
--rw-rw-rw-  2.0 fat   185736 b- defN 21-Aug-03 10:07 eyelogic/msvcp140_2.dll
--rw-rw-rw-  2.0 fat   334728 b- defN 21-Aug-03 10:07 eyelogic/vccorlib140.dll
--rw-rw-rw-  2.0 fat    97160 b- defN 21-Aug-03 10:07 eyelogic/vcruntime140.dll
--rw-rw-rw-  2.0 fat     7847 b- defN 22-Dec-19 11:28 eyelogic_sdk-1.1.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2440 b- defN 22-Dec-19 11:28 eyelogic_sdk-1.1.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Dec-19 11:28 eyelogic_sdk-1.1.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 22-Dec-19 11:28 eyelogic_sdk-1.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1207 b- defN 22-Dec-19 11:28 eyelogic_sdk-1.1.6.dist-info/RECORD
-15 files, 2465990 bytes uncompressed, 878522 bytes compressed:  64.4%
+Zip file size: 13177 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat    29333 b- defN 23-Jan-05 15:31 eyelogic/ELApi.py
+-rw-rw-rw-  2.0 fat     1168 b- defN 23-Jan-05 20:56 eyelogic/__init__.py
+-rw-rw-rw-  2.0 fat     7852 b- defN 23-Jan-05 21:16 eyelogic_sdk-1.1.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2440 b- defN 23-Jan-05 21:16 eyelogic_sdk-1.1.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jan-05 21:16 eyelogic_sdk-1.1.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jan-05 21:16 eyelogic_sdk-1.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      562 b- defN 23-Jan-05 21:16 eyelogic_sdk-1.1.7.dist-info/RECORD
+7 files, 41456 bytes uncompressed, 12181 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -1,46 +1,22 @@
-Filename: eyelogic/ELApi.dll
-Comment: 
-
 Filename: eyelogic/ELApi.py
 Comment: 
 
-Filename: eyelogic/ELCApi.dll
-Comment: 
-
 Filename: eyelogic/__init__.py
 Comment: 
 
-Filename: eyelogic/concrt140.dll
-Comment: 
-
-Filename: eyelogic/msvcp140.dll
-Comment: 
-
-Filename: eyelogic/msvcp140_1.dll
-Comment: 
-
-Filename: eyelogic/msvcp140_2.dll
-Comment: 
-
-Filename: eyelogic/vccorlib140.dll
-Comment: 
-
-Filename: eyelogic/vcruntime140.dll
-Comment: 
-
-Filename: eyelogic_sdk-1.1.6.dist-info/LICENSE
+Filename: eyelogic_sdk-1.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: eyelogic_sdk-1.1.6.dist-info/METADATA
+Filename: eyelogic_sdk-1.1.7.dist-info/METADATA
 Comment: 
 
-Filename: eyelogic_sdk-1.1.6.dist-info/WHEEL
+Filename: eyelogic_sdk-1.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: eyelogic_sdk-1.1.6.dist-info/top_level.txt
+Filename: eyelogic_sdk-1.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: eyelogic_sdk-1.1.6.dist-info/RECORD
+Filename: eyelogic_sdk-1.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## eyelogic/ELApi.py

```diff
@@ -1,9 +1,9 @@
 # -----------------------------------------------------------------------
-# Copyright (C) 2019-2022, EyeLogic GmbH
+# Copyright (C) 2019-2023, EyeLogic GmbH
 #
 # Permission is hereby granted, free of charge, to any person or
 # organization obtaining a copy of the software and accompanying
 # documentation covered by this license (the "Software") to use,
 # reproduce, display, distribute, execute, and transmit the Software,
 # and to prepare derivative works of the Software, and to permit
 # third-parties to whom the Software is furnished to do so.
@@ -69,17 +69,17 @@
 
 ## callback function type, new gaze samples
 GazeSampleCallback = CFUNCTYPE(None, POINTER(ELGazeSample))
 ## callback function type, event occurred
 EventCallback = CFUNCTYPE(None, c_int32)
 
 if sys.maxsize > 2**32:
-    libname = "ELCApi"
+    libname = os.path.join("x64", "ELCApi")
 else:
-    libname = "ELCApi32"
+    libname = os.path.join("x86", "ELCApi32")
 baseDir = os.path.dirname(os.path.abspath(__file__))
 libnameGlobal = os.path.join(baseDir, libname + ".dll")
 if not os.path.isfile(libnameGlobal):
     raise Exception(
         "WARNING: Could not find EyeLogic dll in its expected location: '{}'".
         format(libnameGlobal))
 try:
```

## eyelogic/__init__.py

```diff
@@ -1,9 +1,9 @@
 # -----------------------------------------------------------------------
-# Copyright (C) 2019-2022, EyeLogic GmbH
+# Copyright (C) 2019-2023, EyeLogic GmbH
 #
 # Permission is hereby granted, free of charge, to any person or
 # organization obtaining a copy of the software and accompanying
 # documentation covered by this license (the "Software") to use,
 # reproduce, display, distribute, execute, and transmit the Software,
 # and to prepare derivative works of the Software, and to permit
 # third-parties to whom the Software is furnished to do so.
@@ -16,8 +16,8 @@
 # LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT
 # OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 # -----------------------------------------------------------------------
 
 __all__ = ["ELApi"]
 __author__ = "EyeLogic GmbH"
-__version__ = "1.1.6"
+__version__ = "1.1.7"
```

## Comparing `eyelogic_sdk-1.1.6.dist-info/LICENSE` & `eyelogic_sdk-1.1.7.dist-info/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2022 EyeLogic GmbH
+Copyright (c) 2019-2023 EyeLogic GmbH
 
 LICENSE AGREEMENT
 
 IMPORTANT – PLEASE READ CAREFULLY:
 The License Agreement is a legal agreement between you and EyeLogic GmbH and its affiliates ("EyeLogic", "we", or "us"). This license agreement governs your use of the EyeLogic software and any third party software that may be distributed therewith (collectively the "software"). EyeLogic agrees to license the software to you (personally and/or on behalf of you employer) (collectively "you" or "your") only if you accept all the terms contained in this license agreement. By installing, using, copying, or distributing all or any portion of the software, you accept and agree to be bound by all of the terms and conditions of this license agreement.
 If you do not agree with any of the terms of this license agreement, do no install or use the software.
```

## Comparing `eyelogic_sdk-1.1.6.dist-info/METADATA` & `eyelogic_sdk-1.1.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyelogic-sdk
-Version: 1.1.6
+Version: 1.1.7
 Summary: Python wrapper for the EyeLogic eye tracking API
 Home-page: https://www.eyelogic.de
 Author: EyeLogic GmbH
 Author-email: info@eyelogic.de
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

