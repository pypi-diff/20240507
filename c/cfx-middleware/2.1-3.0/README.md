# Comparing `tmp/cfx_middleware-2.1.tar.gz` & `tmp/cfx_middleware-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfx_middleware-2.1.tar", last modified: Sat Mar  2 16:04:53 2024, max compression
+gzip compressed data, was "cfx_middleware-3.0.tar", last modified: Tue May  7 16:01:59 2024, max compression
```

## Comparing `cfx_middleware-2.1.tar` & `cfx_middleware-3.0.tar`

### file list

```diff
@@ -1,46 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-03-02 16:04:53.242907 cfx_middleware-2.1/
--rw-rw-rw-   0        0        0     1677 2024-03-02 16:04:53.241909 cfx_middleware-2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1147 2024-02-21 02:16:28.000000 cfx_middleware-2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-02 16:04:53.030863 cfx_middleware-2.1/cfx_middleware/
--rw-rw-rw-   0        0        0       66 2024-02-26 18:00:20.000000 cfx_middleware-2.1/cfx_middleware/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-02 16:04:53.100736 cfx_middleware-2.1/cfx_middleware/__pycache__/
--rw-rw-rw-   0        0        0     5290 2024-02-20 03:12:12.000000 cfx_middleware-2.1/cfx_middleware/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     5854 2024-02-26 17:18:10.000000 cfx_middleware-2.1/cfx_middleware/__pycache__/cfx_middleware.cpython-311.pyc
--rw-rw-rw-   0        0        0     5225 2024-02-20 03:15:18.000000 cfx_middleware-2.1/cfx_middleware/__pycache__/parser_result.cpython-311.pyc
--rw-rw-rw-   0        0        0     5065 2024-02-26 17:56:47.000000 cfx_middleware-2.1/cfx_middleware/cfx_middleware.py
-drwxrwxrwx   0        0        0        0 2024-03-02 16:04:53.119811 cfx_middleware-2.1/cfx_middleware/classes/
--rw-rw-rw-   0        0        0      566 2024-02-26 17:18:57.000000 cfx_middleware-2.1/cfx_middleware/classes/ChildSerialNumber.py
--rw-rw-rw-   0        0        0      211 2024-02-16 16:17:17.000000 cfx_middleware-2.1/cfx_middleware/classes/Parameters.py
--rw-rw-rw-   0        0        0     1701 2024-02-26 17:18:57.000000 cfx_middleware-2.1/cfx_middleware/classes/ParserResult.py
--rw-rw-rw-   0        0        0      999 2024-02-16 16:54:16.000000 cfx_middleware-2.1/cfx_middleware/classes/TestResult.py
-drwxrwxrwx   0        0        0        0 2024-03-02 16:04:53.179023 cfx_middleware-2.1/cfx_middleware/classes/__pycache__/
--rw-rw-rw-   0        0        0     1401 2024-02-26 17:18:28.000000 cfx_middleware-2.1/cfx_middleware/classes/__pycache__/ChildSerialNumber.cpython-311.pyc
--rw-rw-rw-   0        0        0      792 2024-02-16 16:17:19.000000 cfx_middleware-2.1/cfx_middleware/classes/__pycache__/Parameters.cpython-311.pyc
--rw-rw-rw-   0        0        0     2263 2024-02-26 17:18:28.000000 cfx_middleware-2.1/cfx_middleware/classes/__pycache__/ParserResult.cpython-311.pyc
--rw-rw-rw-   0        0        0     1521 2024-02-16 16:55:16.000000 cfx_middleware-2.1/cfx_middleware/classes/__pycache__/TestResult.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-03-02 16:04:53.181018 cfx_middleware-2.1/cfx_middleware/enums/
--rw-rw-rw-   0        0        0      203 2024-02-16 15:49:58.000000 cfx_middleware-2.1/cfx_middleware/enums/MethodsEnum.py
-drwxrwxrwx   0        0        0        0 2024-03-02 16:04:53.184010 cfx_middleware-2.1/cfx_middleware/enums/__pycache__/
--rw-rw-rw-   0        0        0      548 2024-02-16 15:50:00.000000 cfx_middleware-2.1/cfx_middleware/enums/__pycache__/MethodsEnum.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-03-02 16:04:53.189994 cfx_middleware-2.1/cfx_middleware/exceptions/
--rw-rw-rw-   0        0        0      397 2024-02-26 17:18:57.000000 cfx_middleware-2.1/cfx_middleware/exceptions/MethodNotValid.py
--rw-rw-rw-   0        0        0      229 2024-02-16 15:33:22.000000 cfx_middleware-2.1/cfx_middleware/exceptions/NotDictException.py
-drwxrwxrwx   0        0        0        0 2024-03-02 16:04:53.210011 cfx_middleware-2.1/cfx_middleware/exceptions/__pycache__/
--rw-rw-rw-   0        0        0     1155 2024-02-26 17:18:28.000000 cfx_middleware-2.1/cfx_middleware/exceptions/__pycache__/MethodNotValid.cpython-311.pyc
--rw-rw-rw-   0        0        0      723 2024-02-16 15:33:26.000000 cfx_middleware-2.1/cfx_middleware/exceptions/__pycache__/NotDictException.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-03-02 16:04:53.214073 cfx_middleware-2.1/cfx_middleware/helpers/
-drwxrwxrwx   0        0        0        0 2024-03-02 16:04:53.216972 cfx_middleware-2.1/cfx_middleware/helpers/__pycache__/
--rw-rw-rw-   0        0        0     3539 2024-02-26 17:18:28.000000 cfx_middleware-2.1/cfx_middleware/helpers/__pycache__/utils.cpython-311.pyc
--rw-rw-rw-   0        0        0     1430 2024-02-26 17:18:57.000000 cfx_middleware-2.1/cfx_middleware/helpers/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-02 16:04:53.220960 cfx_middleware-2.1/cfx_middleware/rabbit/
-drwxrwxrwx   0        0        0        0 2024-03-02 16:04:53.240911 cfx_middleware-2.1/cfx_middleware/rabbit/__pycache__/
--rw-rw-rw-   0        0        0     2195 2024-02-16 16:30:41.000000 cfx_middleware-2.1/cfx_middleware/rabbit/__pycache__/send_rabbit.cpython-311.pyc
--rw-rw-rw-   0        0        0     1493 2024-02-26 18:20:05.000000 cfx_middleware-2.1/cfx_middleware/rabbit/send_rabbit.py
-drwxrwxrwx   0        0        0        0 2024-03-02 16:04:53.037844 cfx_middleware-2.1/cfx_middleware.egg-info/
--rw-rw-rw-   0        0        0     1677 2024-03-02 16:04:52.000000 cfx_middleware-2.1/cfx_middleware.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1363 2024-03-02 16:04:52.000000 cfx_middleware-2.1/cfx_middleware.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-02 16:04:52.000000 cfx_middleware-2.1/cfx_middleware.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-03-02 16:04:52.000000 cfx_middleware-2.1/cfx_middleware.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-03-02 16:04:52.000000 cfx_middleware-2.1/cfx_middleware.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-02 16:04:53.242907 cfx_middleware-2.1/setup.cfg
--rw-rw-rw-   0        0        0      980 2024-02-26 18:00:16.000000 cfx_middleware-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 16:01:59.085985 cfx_middleware-3.0/
+-rw-rw-rw-   0        0        0     1677 2024-05-07 16:01:59.081995 cfx_middleware-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1147 2024-05-07 15:16:41.000000 cfx_middleware-3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 16:01:59.054071 cfx_middleware-3.0/cfx_middleware/
+-rw-rw-rw-   0        0        0       66 2024-05-07 15:52:20.000000 cfx_middleware-3.0/cfx_middleware/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 16:01:59.059057 cfx_middleware-3.0/cfx_middleware/__pycache__/
+-rw-rw-rw-   0        0        0     6006 2024-05-07 15:47:46.000000 cfx_middleware-3.0/cfx_middleware/__pycache__/cfx_middleware.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4755 2024-05-07 15:56:04.000000 cfx_middleware-3.0/cfx_middleware/cfx_middleware.py
+drwxrwxrwx   0        0        0        0 2024-05-07 16:01:59.062048 cfx_middleware-3.0/cfx_middleware/classes/
+-rw-rw-rw-   0        0        0      566 2024-05-07 15:50:16.000000 cfx_middleware-3.0/cfx_middleware/classes/ChildSerialNumber.py
+-rw-rw-rw-   0        0        0      211 2024-05-07 15:16:41.000000 cfx_middleware-3.0/cfx_middleware/classes/Parameters.py
+-rw-rw-rw-   0        0        0     1701 2024-05-07 15:50:16.000000 cfx_middleware-3.0/cfx_middleware/classes/ParserResult.py
+-rw-rw-rw-   0        0        0      999 2024-05-07 15:16:41.000000 cfx_middleware-3.0/cfx_middleware/classes/TestResult.py
+drwxrwxrwx   0        0        0        0 2024-05-07 16:01:59.067036 cfx_middleware-3.0/cfx_middleware/classes/__pycache__/
+-rw-rw-rw-   0        0        0     1414 2024-05-07 15:48:06.000000 cfx_middleware-3.0/cfx_middleware/classes/__pycache__/ChildSerialNumber.cpython-311.pyc
+-rw-rw-rw-   0        0        0      820 2024-05-07 15:48:06.000000 cfx_middleware-3.0/cfx_middleware/classes/__pycache__/Parameters.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2276 2024-05-07 15:48:06.000000 cfx_middleware-3.0/cfx_middleware/classes/__pycache__/ParserResult.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1549 2024-05-07 15:48:06.000000 cfx_middleware-3.0/cfx_middleware/classes/__pycache__/TestResult.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-05-07 16:01:59.068033 cfx_middleware-3.0/cfx_middleware/enums/
+-rw-rw-rw-   0        0        0      357 2024-05-07 15:35:31.000000 cfx_middleware-3.0/cfx_middleware/enums/MethodsEnum.py
+drwxrwxrwx   0        0        0        0 2024-05-07 16:01:59.069030 cfx_middleware-3.0/cfx_middleware/enums/__pycache__/
+-rw-rw-rw-   0        0        0      696 2024-05-07 15:48:06.000000 cfx_middleware-3.0/cfx_middleware/enums/__pycache__/MethodsEnum.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-05-07 16:01:59.072022 cfx_middleware-3.0/cfx_middleware/exceptions/
+-rw-rw-rw-   0        0        0      397 2024-05-07 15:50:16.000000 cfx_middleware-3.0/cfx_middleware/exceptions/MethodNotValid.py
+-rw-rw-rw-   0        0        0      229 2024-05-07 15:16:41.000000 cfx_middleware-3.0/cfx_middleware/exceptions/NotDictException.py
+drwxrwxrwx   0        0        0        0 2024-05-07 16:01:59.075015 cfx_middleware-3.0/cfx_middleware/exceptions/__pycache__/
+-rw-rw-rw-   0        0        0     1168 2024-05-07 15:48:06.000000 cfx_middleware-3.0/cfx_middleware/exceptions/__pycache__/MethodNotValid.cpython-311.pyc
+-rw-rw-rw-   0        0        0      751 2024-05-07 15:48:06.000000 cfx_middleware-3.0/cfx_middleware/exceptions/__pycache__/NotDictException.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-05-07 16:01:59.076012 cfx_middleware-3.0/cfx_middleware/helpers/
+drwxrwxrwx   0        0        0        0 2024-05-07 16:01:59.077009 cfx_middleware-3.0/cfx_middleware/helpers/__pycache__/
+-rw-rw-rw-   0        0        0     3899 2024-05-07 15:48:06.000000 cfx_middleware-3.0/cfx_middleware/helpers/__pycache__/utils.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1741 2024-05-07 15:50:16.000000 cfx_middleware-3.0/cfx_middleware/helpers/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-07 16:01:59.078005 cfx_middleware-3.0/cfx_middleware/rabbit/
+drwxrwxrwx   0        0        0        0 2024-05-07 16:01:59.080001 cfx_middleware-3.0/cfx_middleware/rabbit/__pycache__/
+-rw-rw-rw-   0        0        0     2397 2024-05-07 15:48:06.000000 cfx_middleware-3.0/cfx_middleware/rabbit/__pycache__/send_rabbit.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1493 2024-05-07 15:16:41.000000 cfx_middleware-3.0/cfx_middleware/rabbit/send_rabbit.py
+drwxrwxrwx   0        0        0        0 2024-05-07 16:01:59.058059 cfx_middleware-3.0/cfx_middleware.egg-info/
+-rw-rw-rw-   0        0        0     1677 2024-05-07 16:01:58.000000 cfx_middleware-3.0/cfx_middleware.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1254 2024-05-07 16:01:58.000000 cfx_middleware-3.0/cfx_middleware.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 16:01:58.000000 cfx_middleware-3.0/cfx_middleware.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-07 16:01:58.000000 cfx_middleware-3.0/cfx_middleware.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-07 16:01:58.000000 cfx_middleware-3.0/cfx_middleware.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 16:01:59.085985 cfx_middleware-3.0/setup.cfg
+-rw-rw-rw-   0        0        0      980 2024-05-07 15:52:08.000000 cfx_middleware-3.0/setup.py
```

### Comparing `cfx_middleware-2.1/PKG-INFO` & `cfx_middleware-3.0/cfx_middleware.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cfx_middleware
-Version: 2.1
+Name: cfx-middleware
+Version: 3.0
 Summary: Provide a Middleware between the system and CFX
 Home-page: https://dev.azure.com/USI-Applications/USI%20Global%20Development/_git/PCD.Middleware.CFX.Python
 Author: Victor Dominguez
 Author-email: e-victor_dominguez@usiglobal.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cfx_middleware-2.1/README.md` & `cfx_middleware-3.0/README.md`

 * *Files identical despite different names*

### Comparing `cfx_middleware-2.1/cfx_middleware/__pycache__/__init__.cpython-311.pyc` & `cfx_middleware-3.0/cfx_middleware/__pycache__/cfx_middleware.cpython-311.pyc`

 * *Files 20% similar despite different names*

#### Python bytecode

```diff
@@ -1,794 +1,873 @@
 magic:    0xa70d0d0a
-moddate:  0x5317d465 (Tue Feb 20 03:06:59 2024 UTC)
-files sz: 5070
+moddate:  0xf64c3a66 (Tue May  7 15:47:02 2024 UTC)
+files sz: 4720
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 22
    flags     : 0
    code
-      0x9700640064016c005a00640064016c015a01640064026c026d035a0301
-      00640064016c045a04640064036c056d065a060100640064046c076d085a
-      086d095a090100640064056c0a6d0b5a0b6d0c5a0c0100640064066c0d6d
-      0e5a0e6d0f5a0f0100640064076c106d115a11010002006503a6000000ab
-      000000000000000000a01200000000000000000000000000000000000000
-      006408a6010000ab0100000000000000005a13640984005a14640a651566
-      02640b84045a16640a65066602640c84045a17640a65066602640d84045a
-      18640a65066602640e84045a19640a65066602640f84045a1a651b64106b
-      0200000000726c0200651469006411641293016413641493016415641693
-      01641764189301641964149301641a641b9301641c641d9301641e641f93
-      016420642193016422642393016424642593016426642793016428642993
-      01642a642b9301642c64149301642d64149301642e641f9301642b641464
-      2f9c026414643064316421643264336434643564366437641f6414641464
-      146414641464389c0c643264336434643564366437641f64146414641464
-      14641464389c0c6702642164399c046701643a9c04a501a6010000ab0100
-      0000000000000001006401530064015300
+      0x9700640064016c005a00640064026c016d025a020100640064036c036d
+      045a046d055a050100640064046c066d075a076d085a080100640064056c
+      096d0a5a0a6d0b5a0b6d0c5a0c0100640064066c0d6d0e5a0e0100640784
+      005a0f640865106602640984045a11640865026602640a84045a12640865
+      026602640b84045a13640865026602640c84045a14640865026602640d84
+      045a15640865026602640e84045a166517640f6b0200000000726d020065
+      0f6900641064119301641264139301641464159301641664179301641864
+      1393016419641a9301641b641c9301641d641e9301641f64209301642164
+      2293016423642493016425642693016427642893016429642a9301642b64
+      2c9301642d64139301642e64139301641e642c6413642f9c026413643064
+      316420643264336434643564366437641e6413641364136413641364389c
+      0c6701642064399c046701643a9c05a501a6010000ab0100000000000000
+      005a1802006519643b65189b009d02a6010000ab01000000000000000001
+      006401530064015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (sys)
                  8 STORE_NAME               0 (sys)
    
-     2          10 LOAD_CONST               0 (0)
-                12 LOAD_CONST               1 (None)
-                14 IMPORT_NAME              1 (json)
-                16 STORE_NAME               1 (json)
+     3          10 LOAD_CONST               0 (0)
+                12 LOAD_CONST               2 (('ParserResult',))
+                14 IMPORT_NAME              1 (cfx_middleware.classes.ParserResult)
+                16 IMPORT_FROM              2 (ParserResult)
+                18 STORE_NAME               2 (ParserResult)
+                20 POP_TOP
    
-     3          18 LOAD_CONST               0 (0)
-                20 LOAD_CONST               2 (('dotenv_values',))
-                22 IMPORT_NAME              2 (dotenv)
-                24 IMPORT_FROM              3 (dotenv_values)
-                26 STORE_NAME               3 (dotenv_values)
-                28 POP_TOP
+     4          22 LOAD_CONST               0 (0)
+                24 LOAD_CONST               3 (('NotDictException', 'is_dict'))
+                26 IMPORT_NAME              3 (cfx_middleware.exceptions.NotDictException)
+                28 IMPORT_FROM              4 (NotDictException)
+                30 STORE_NAME               4 (NotDictException)
+                32 IMPORT_FROM              5 (is_dict)
+                34 STORE_NAME               5 (is_dict)
+                36 POP_TOP
    
-     4          30 LOAD_CONST               0 (0)
-                32 LOAD_CONST               1 (None)
-                34 IMPORT_NAME              4 (pprint)
-                36 STORE_NAME               4 (pprint)
+     5          38 LOAD_CONST               0 (0)
+                40 LOAD_CONST               4 (('MethodNotValid', 'validate_method'))
+                42 IMPORT_NAME              6 (cfx_middleware.exceptions.MethodNotValid)
+                44 IMPORT_FROM              7 (MethodNotValid)
+                46 STORE_NAME               7 (MethodNotValid)
+                48 IMPORT_FROM              8 (validate_method)
+                50 STORE_NAME               8 (validate_method)
+                52 POP_TOP
    
-     6          38 LOAD_CONST               0 (0)
-                40 LOAD_CONST               3 (('ParserResult',))
-                42 IMPORT_NAME              5 (parser_result.classes.ParserResult)
-                44 IMPORT_FROM              6 (ParserResult)
-                46 STORE_NAME               6 (ParserResult)
-                48 POP_TOP
+     6          54 LOAD_CONST               0 (0)
+                56 LOAD_CONST               5 (('class_to_json', 'json_to_dict', 'all_methods'))
+                58 IMPORT_NAME              9 (cfx_middleware.helpers.utils)
+                60 IMPORT_FROM             10 (class_to_json)
+                62 STORE_NAME              10 (class_to_json)
+                64 IMPORT_FROM             11 (json_to_dict)
+                66 STORE_NAME              11 (json_to_dict)
+                68 IMPORT_FROM             12 (all_methods)
+                70 STORE_NAME              12 (all_methods)
+                72 POP_TOP
    
-     7          50 LOAD_CONST               0 (0)
-                52 LOAD_CONST               4 (('NotDictException', 'is_dict'))
-                54 IMPORT_NAME              7 (parser_result.exceptions.NotDictException)
-                56 IMPORT_FROM              8 (NotDictException)
-                58 STORE_NAME               8 (NotDictException)
-                60 IMPORT_FROM              9 (is_dict)
-                62 STORE_NAME               9 (is_dict)
-                64 POP_TOP
+     7          74 LOAD_CONST               0 (0)
+                76 LOAD_CONST               6 (('send_message',))
+                78 IMPORT_NAME             13 (cfx_middleware.rabbit.send_rabbit)
+                80 IMPORT_FROM             14 (send_message)
+                82 STORE_NAME              14 (send_message)
+                84 POP_TOP
    
-     8          66 LOAD_CONST               0 (0)
-                68 LOAD_CONST               5 (('MethodNotValid', 'validate_method'))
-                70 IMPORT_NAME             10 (parser_result.exceptions.MethodNotValid)
-                72 IMPORT_FROM             11 (MethodNotValid)
-                74 STORE_NAME              11 (MethodNotValid)
-                76 IMPORT_FROM             12 (validate_method)
-                78 STORE_NAME              12 (validate_method)
-                80 POP_TOP
+    10          86 LOAD_CONST               7 (<code object parser_result, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\cfx_middleware.py", line 10>)
+                88 MAKE_FUNCTION            0
+                90 STORE_NAME              15 (parser_result)
    
-     9          82 LOAD_CONST               0 (0)
-                84 LOAD_CONST               6 (('class_to_json', 'json_to_dict'))
-                86 IMPORT_NAME             13 (parser_result.helpers.utils)
-                88 IMPORT_FROM             14 (class_to_json)
-                90 STORE_NAME              14 (class_to_json)
-                92 IMPORT_FROM             15 (json_to_dict)
-                94 STORE_NAME              15 (json_to_dict)
-                96 POP_TOP
+    33          92 LOAD_CONST               8 ('parser_result')
+                94 LOAD_NAME               16 (dict)
+                96 BUILD_TUPLE              2
+                98 LOAD_CONST               9 (<code object validate_parser_result, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\cfx_middleware.py", line 33>)
+               100 MAKE_FUNCTION            4 (annotations)
+               102 STORE_NAME              17 (validate_parser_result)
    
-    10          98 LOAD_CONST               0 (0)
-               100 LOAD_CONST               7 (('send_message',))
-               102 IMPORT_NAME             16 (parser_result.rabbit.send_rabbit)
-               104 IMPORT_FROM             17 (send_message)
-               106 STORE_NAME              17 (send_message)
-               108 POP_TOP
+    56         104 LOAD_CONST               8 ('parser_result')
+               106 LOAD_NAME                2 (ParserResult)
+               108 BUILD_TUPLE              2
+               110 LOAD_CONST              10 (<code object send_parser, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\cfx_middleware.py", line 56>)
+               112 MAKE_FUNCTION            4 (annotations)
+               114 STORE_NAME              18 (send_parser)
    
-    12         110 PUSH_NULL
-               112 LOAD_NAME                3 (dotenv_values)
-               114 PRECALL                  0
-               118 CALL                     0
-               128 LOAD_METHOD             18 (get)
-               150 LOAD_CONST               8 ('RABBITMQ_EXCHANGE_PARSER_QUEUE')
-               152 PRECALL                  1
-               156 CALL                     1
-               166 STORE_NAME              19 (RABBITMQ_EXCHANGE_PARSER_QUEUE)
+    63         116 LOAD_CONST               8 ('parser_result')
+               118 LOAD_NAME                2 (ParserResult)
+               120 BUILD_TUPLE              2
+               122 LOAD_CONST              11 (<code object validate_units, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\cfx_middleware.py", line 63>)
+               124 MAKE_FUNCTION            4 (annotations)
+               126 STORE_NAME              19 (validate_units)
    
-    15         168 LOAD_CONST               9 (<code object parser_result, file "D:\Proyectos\ParserResult\parser_result\__init__.py", line 15>)
-               170 MAKE_FUNCTION            0
-               172 STORE_NAME              20 (parser_result)
+    70         128 LOAD_CONST               8 ('parser_result')
+               130 LOAD_NAME                2 (ParserResult)
+               132 BUILD_TUPLE              2
+               134 LOAD_CONST              12 (<code object units_inspected, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\cfx_middleware.py", line 70>)
+               136 MAKE_FUNCTION            4 (annotations)
+               138 STORE_NAME              20 (units_inspected)
    
-    25         174 LOAD_CONST              10 ('parser_result')
-               176 LOAD_NAME               21 (dict)
-               178 BUILD_TUPLE              2
-               180 LOAD_CONST              11 (<code object validate_parser_result, file "D:\Proyectos\ParserResult\parser_result\__init__.py", line 25>)
-               182 MAKE_FUNCTION            4 (annotations)
-               184 STORE_NAME              22 (validate_parser_result)
+    77         140 LOAD_CONST               8 ('parser_result')
+               142 LOAD_NAME                2 (ParserResult)
+               144 BUILD_TUPLE              2
+               146 LOAD_CONST              13 (<code object units_departed, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\cfx_middleware.py", line 77>)
+               148 MAKE_FUNCTION            4 (annotations)
+               150 STORE_NAME              21 (units_departed)
    
-    47         186 LOAD_CONST              10 ('parser_result')
-               188 LOAD_NAME                6 (ParserResult)
-               190 BUILD_TUPLE              2
-               192 LOAD_CONST              12 (<code object validate_units, file "D:\Proyectos\ParserResult\parser_result\__init__.py", line 47>)
-               194 MAKE_FUNCTION            4 (annotations)
-               196 STORE_NAME              23 (validate_units)
+    84         152 LOAD_CONST               8 ('parser_result')
+               154 LOAD_NAME                2 (ParserResult)
+               156 BUILD_TUPLE              2
+               158 LOAD_CONST              14 (<code object state_change, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\cfx_middleware.py", line 84>)
+               160 MAKE_FUNCTION            4 (annotations)
+               162 STORE_NAME              22 (state_change)
    
-    54         198 LOAD_CONST              10 ('parser_result')
-               200 LOAD_NAME                6 (ParserResult)
-               202 BUILD_TUPLE              2
-               204 LOAD_CONST              13 (<code object units_inspected, file "D:\Proyectos\ParserResult\parser_result\__init__.py", line 54>)
-               206 MAKE_FUNCTION            4 (annotations)
-               208 STORE_NAME              24 (units_inspected)
+    91         164 LOAD_NAME               23 (__name__)
+               166 LOAD_CONST              15 ('__main__')
+               168 COMPARE_OP               2 (==)
+               174 POP_JUMP_FORWARD_IF_FALSE   109 (to 394)
    
-    61         210 LOAD_CONST              10 ('parser_result')
-               212 LOAD_NAME                6 (ParserResult)
-               214 BUILD_TUPLE              2
-               216 LOAD_CONST              14 (<code object units_departed, file "D:\Proyectos\ParserResult\parser_result\__init__.py", line 61>)
-               218 MAKE_FUNCTION            4 (annotations)
-               220 STORE_NAME              25 (units_departed)
+    92         176 PUSH_NULL
+               178 LOAD_NAME               15 (parser_result)
    
-    68         222 LOAD_CONST              10 ('parser_result')
-               224 LOAD_NAME                6 (ParserResult)
-               226 BUILD_TUPLE              2
-               228 LOAD_CONST              15 (<code object state_change, file "D:\Proyectos\ParserResult\parser_result\__init__.py", line 68>)
-               230 MAKE_FUNCTION            4 (annotations)
-               232 STORE_NAME              26 (state_change)
+    93         180 BUILD_MAP                0
    
-    75         234 LOAD_NAME               27 (__name__)
-               236 LOAD_CONST              16 ('__main__')
-               238 COMPARE_OP               2 (==)
-               244 POP_JUMP_FORWARD_IF_FALSE   108 (to 462)
+    94         182 LOAD_CONST              16 ('SerialNumber')
+               184 LOAD_CONST              17 ('P69660003012311280100684')
    
-    76         246 PUSH_NULL
-               248 LOAD_NAME               20 (parser_result)
+    93         186 MAP_ADD                  1
    
-    77         250 BUILD_MAP                0
+    95         188 LOAD_CONST              18 ('Sequence')
+               190 LOAD_CONST              19 ('None')
    
-    78         252 LOAD_CONST              17 ('SerialNumber')
-               254 LOAD_CONST              18 ('P69660003012311280100684')
+    93         192 MAP_ADD                  1
    
-    77         256 MAP_ADD                  1
+    96         194 LOAD_CONST              20 ('Assembly')
+               196 LOAD_CONST              21 ('6966-0003-01')
    
-    79         258 LOAD_CONST              19 ('Sequence')
-               260 LOAD_CONST              20 ('None')
+    93         198 MAP_ADD                  1
    
-    77         262 MAP_ADD                  1
+    97         200 LOAD_CONST              22 ('RouteStep')
+               202 LOAD_CONST              23 ('AOI_T')
    
-    80         264 LOAD_CONST              21 ('Assembly')
-               266 LOAD_CONST              22 ('6966-0003-01')
+    93         204 MAP_ADD                  1
    
-    77         268 MAP_ADD                  1
+    98         206 LOAD_CONST              24 ('WorkOrder')
+               208 LOAD_CONST              19 ('None')
    
-    81         270 LOAD_CONST              23 ('RouteStep')
-               272 LOAD_CONST              24 ('AOI_T')
+    93         210 MAP_ADD                  1
    
-    77         274 MAP_ADD                  1
+    99         212 LOAD_CONST              25 ('Step')
+               214 LOAD_CONST              26 ('2')
    
-    82         276 LOAD_CONST              25 ('WorkOrder')
-               278 LOAD_CONST              20 ('None')
+    93         216 MAP_ADD                  1
    
-    77         280 MAP_ADD                  1
+   100         218 LOAD_CONST              27 ('Line')
+               220 LOAD_CONST              28 ('L16')
    
-    83         282 LOAD_CONST              26 ('Step')
-               284 LOAD_CONST              27 ('2')
+    93         222 MAP_ADD                  1
    
-    77         286 MAP_ADD                  1
+   101         224 LOAD_CONST              29 ('IsPanel')
+               226 LOAD_CONST              30 (True)
    
-    84         288 LOAD_CONST              28 ('Line')
-               290 LOAD_CONST              29 ('L16')
+    93         228 MAP_ADD                  1
    
-    77         292 MAP_ADD                  1
+   102         230 LOAD_CONST              31 ('PassFail')
+               232 LOAD_CONST              32 (1)
    
-    85         294 LOAD_CONST              30 ('IsPanel')
-               296 LOAD_CONST              31 (True)
+    93         234 MAP_ADD                  1
    
-    77         298 MAP_ADD                  1
+   103         236 LOAD_CONST              33 ('User')
+               238 LOAD_CONST              34 ('SAUL RUIZ')
    
-    86         300 LOAD_CONST              32 ('PassFail')
-               302 LOAD_CONST              33 (1)
+    93         240 MAP_ADD                  1
    
-    77         304 MAP_ADD                  1
+   104         242 LOAD_CONST              35 ('StartTime')
+               244 LOAD_CONST              36 ('2023-11-29T10:24:31')
    
-    87         306 LOAD_CONST              34 ('User')
-               308 LOAD_CONST              35 ('SAUL RUIZ')
+    93         246 MAP_ADD                  1
    
-    77         310 MAP_ADD                  1
+   105         248 LOAD_CONST              37 ('EndTime')
+               250 LOAD_CONST              38 ('2023-11-29T10:24:46')
    
-    88         312 LOAD_CONST              36 ('StartTime')
-               314 LOAD_CONST              37 ('2023-11-29T10:24:31')
+    93         252 MAP_ADD                  1
    
-    77         316 MAP_ADD                  1
+   106         254 LOAD_CONST              39 ('MachineId')
+               256 LOAD_CONST              40 ('AOI-L16')
    
-    89         318 LOAD_CONST              38 ('EndTime')
-               320 LOAD_CONST              39 ('2023-11-29T10:24:46')
+    93         258 MAP_ADD                  1
    
-    77         322 MAP_ADD                  1
+   107         260 LOAD_CONST              41 ('IoTId')
+               262 LOAD_CONST              42 ('84968468')
    
-    90         324 LOAD_CONST              40 ('MachineId')
-               326 LOAD_CONST              41 ('AOI-L16')
+    93         264 MAP_ADD                  1
    
-    77         328 MAP_ADD                  1
+   108         266 LOAD_CONST              43 ('ProgramName')
+               268 LOAD_CONST              44 ('6966-0003-01_BOT')
    
-    91         330 LOAD_CONST              42 ('ProgramName')
-               332 LOAD_CONST              43 ('6966-0003-01_BOT')
+    93         270 MAP_ADD                  1
    
-    77         334 MAP_ADD                  1
+   109         272 LOAD_CONST              45 ('LogFileName')
+               274 LOAD_CONST              19 ('None')
    
-    92         336 LOAD_CONST              44 ('LogFileName')
-               338 LOAD_CONST              20 ('None')
+    93         276 MAP_ADD                  1
    
-    77         340 MAP_ADD                  1
+   110         278 LOAD_CONST              46 ('Remarks')
+               280 LOAD_CONST              19 ('None')
    
-    93         342 LOAD_CONST              45 ('Remarks')
-               344 LOAD_CONST              20 ('None')
+    93         282 MAP_ADD                  1
    
-    77         346 MAP_ADD                  1
+   111         284 LOAD_CONST              30 (True)
    
-    94         348 LOAD_CONST              46 ('IsBirth')
-               350 LOAD_CONST              31 (True)
+   112         286 LOAD_CONST              44 ('6966-0003-01_BOT')
+               288 LOAD_CONST              19 ('None')
+               290 LOAD_CONST              47 (('RecipeName', 'RecipeRevision'))
+               292 BUILD_CONST_KEY_MAP      2
    
-    77         352 MAP_ADD                  1
+   113         294 LOAD_CONST              19 ('None')
    
-    95         354 LOAD_CONST              43 ('6966-0003-01_BOT')
-               356 LOAD_CONST              20 ('None')
-               358 LOAD_CONST              47 (('RecipeName', 'RecipeRevision'))
-               360 BUILD_CONST_KEY_MAP      2
+   114         296 LOAD_CONST              48 ('units_inspected')
    
-    96         362 LOAD_CONST              20 ('None')
+   117         298 LOAD_CONST              49 ('')
    
-    97         364 LOAD_CONST              48 ('units_inspecteds')
+   118         300 LOAD_CONST              32 (1)
    
-   100         366 LOAD_CONST              49 ('')
+   121         302 LOAD_CONST              50 ('ST5901_Polarity3_Polarity_AI2-3D-1_AI2_3D_ConfidenceLevel')
    
-   101         368 LOAD_CONST              33 (1)
+   122         304 LOAD_CONST              51 (5)
    
-   104         370 LOAD_CONST              50 ('ST5901_Polarity3_Polarity_AI2-3D-1_AI2_3D_ConfidenceLevel')
+   123         306 LOAD_CONST              52 ('OK')
    
-   105         372 LOAD_CONST              51 (5)
+   124         308 LOAD_CONST              53 ('1')
    
-   106         374 LOAD_CONST              52 ('OK')
+   125         310 LOAD_CONST              54 ('100')
    
-   107         376 LOAD_CONST              53 ('1')
+   126         312 LOAD_CONST              55 ('82.3721508947464')
    
-   108         378 LOAD_CONST              54 ('100')
+   127         314 LOAD_CONST              30 (True)
    
-   109         380 LOAD_CONST              55 ('82.3721508947464')
+   128         316 LOAD_CONST              19 ('None')
    
-   110         382 LOAD_CONST              31 (True)
+   129         318 LOAD_CONST              19 ('None')
    
-   111         384 LOAD_CONST              20 ('None')
+   130         320 LOAD_CONST              19 ('None')
    
-   112         386 LOAD_CONST              20 ('None')
+   131         322 LOAD_CONST              19 ('None')
    
-   113         388 LOAD_CONST              20 ('None')
+   132         324 LOAD_CONST              19 ('None')
    
-   114         390 LOAD_CONST              20 ('None')
+   120         326 LOAD_CONST              56 (('TestName', 'Sequence', 'PassFail', 'LowLimit', 'HighLimit', 'Value', 'IsCritical', 'Defect', 'ErrorCode', 'ErrorLocation', 'ErrorMessage', 'Parameters'))
+               328 BUILD_CONST_KEY_MAP     12
    
-   115         392 LOAD_CONST              20 ('None')
+   119         330 BUILD_LIST               1
    
-   103         394 LOAD_CONST              56 (('TestName', 'Sequence', 'PassFail', 'LowLimit', 'HighLimit', 'Value', 'IsCritical', 'Defect', 'ErrorCode', 'ErrorLocation', 'ErrorMessage', 'Parameters'))
-               396 BUILD_CONST_KEY_MAP     12
+   135         332 LOAD_CONST              32 (1)
    
-   118         398 LOAD_CONST              50 ('ST5901_Polarity3_Polarity_AI2-3D-1_AI2_3D_ConfidenceLevel')
+   116         334 LOAD_CONST              57 (('SerialNumber', 'Sequence', 'TestResult', 'PassFail'))
+               336 BUILD_CONST_KEY_MAP      4
    
-   119         400 LOAD_CONST              51 (5)
+   115         338 BUILD_LIST               1
    
-   120         402 LOAD_CONST              52 ('OK')
+    93         340 LOAD_CONST              58 (('IsBirth', 'Parameters', 'TestResults', 'Method', 'ChildSerialNumbers'))
+               342 BUILD_CONST_KEY_MAP      5
+               344 DICT_UPDATE              1
    
-   121         404 LOAD_CONST              53 ('1')
+    92         346 PRECALL                  1
+               350 CALL                     1
+               360 STORE_NAME              24 (success)
    
-   122         406 LOAD_CONST              54 ('100')
+   141         362 PUSH_NULL
+               364 LOAD_NAME               25 (print)
+               366 LOAD_CONST              59 ('Success ')
+               368 LOAD_NAME               24 (success)
+               370 FORMAT_VALUE             0
+               372 BUILD_STRING             2
+               374 PRECALL                  1
+               378 CALL                     1
+               388 POP_TOP
+               390 LOAD_CONST               1 (None)
+               392 RETURN_VALUE
    
-   123         408 LOAD_CONST              55 ('82.3721508947464')
-   
-   124         410 LOAD_CONST              31 (True)
-   
-   125         412 LOAD_CONST              20 ('None')
-   
-   126         414 LOAD_CONST              20 ('None')
-   
-   127         416 LOAD_CONST              20 ('None')
-   
-   128         418 LOAD_CONST              20 ('None')
-   
-   129         420 LOAD_CONST              20 ('None')
-   
-   117         422 LOAD_CONST              56 (('TestName', 'Sequence', 'PassFail', 'LowLimit', 'HighLimit', 'Value', 'IsCritical', 'Defect', 'ErrorCode', 'ErrorLocation', 'ErrorMessage', 'Parameters'))
-               424 BUILD_CONST_KEY_MAP     12
-   
-   102         426 BUILD_LIST               2
-   
-   132         428 LOAD_CONST              33 (1)
-   
-    99         430 LOAD_CONST              57 (('SerialNumber', 'Sequence', 'TestResult', 'PassFail'))
-               432 BUILD_CONST_KEY_MAP      4
-   
-    98         434 BUILD_LIST               1
-   
-    77         436 LOAD_CONST              58 (('Parameters', 'TestResults', 'Method', 'ChildSerialNumbers'))
-               438 BUILD_CONST_KEY_MAP      4
-               440 DICT_UPDATE              1
-   
-    76         442 PRECALL                  1
-               446 CALL                     1
-               456 POP_TOP
-               458 LOAD_CONST               1 (None)
-               460 RETURN_VALUE
-   
-    75     >>  462 LOAD_CONST               1 (None)
-               464 RETURN_VALUE
+    91     >>  394 LOAD_CONST               1 (None)
+               396 RETURN_VALUE
    consts
       0
       None
-      ('dotenv_values',)
       ('ParserResult',)
       ('NotDictException', 'is_dict')
       ('MethodNotValid', 'validate_method')
-      ('class_to_json', 'json_to_dict')
+      ('class_to_json', 'json_to_dict', 'all_methods')
       ('send_message',)
-      'RABBITMQ_EXCHANGE_PARSER_QUEUE'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 4
          flags     : 3
          code
             0x97007401000000000000000000007c00740200000000000000000000a6
-            020000ab020000000000000000720f7405000000000000000000007c00a6
-            010000ab0100000000000000007d007407000000000000000000007c00a6
-            010000ab0100000000000000007d01740900000000000000000000a60000
-            00ab0000000000000000007c016a05000000000000000019000000000000
-            0000007d0202007c027c01a6010000ab0100000000000000000100640053
-            00
-          15           0 RESUME                   0
+            020000ab02000000000000000072347c0073237405000000000000000000
+            006401a6010000ab01000000000000000001007407000000000000000000
+            006a0400000000000000006402a6010000ab010000000000000000010074
+            0b000000000000000000007c00a6010000ab0100000000000000007d007c
+            0073237405000000000000000000006403a6010000ab0100000000000000
+            0001007407000000000000000000006a0400000000000000006402a60100
+            00ab0100000000000000000100740d000000000000000000007c00a60100
+            00ab0100000000000000007d017c016a07000000000000000064046b0300
+            0000007224741100000000000000000000a6000000ab0000000000000000
+            007c016a070000000000000000190000000000000000007d0202007c027c
+            01a6010000ab0100000000000000005300741300000000000000000000a6
+            000000ab0000000000000000007c015f0700000000000000007415000000
+            000000000000007c01a6010000ab0100000000000000005300
+          10           0 RESUME                   0
          
-          16           2 LOAD_GLOBAL              1 (NULL + isinstance)
+          12           2 LOAD_GLOBAL              1 (NULL + isinstance)
                       14 LOAD_FAST                0 (parser_result_data)
                       16 LOAD_GLOBAL              2 (str)
                       28 PRECALL                  2
                       32 CALL                     2
-                      42 POP_JUMP_FORWARD_IF_FALSE    15 (to 74)
+                      42 POP_JUMP_FORWARD_IF_FALSE    52 (to 148)
+         
+          13          44 LOAD_FAST                0 (parser_result_data)
+                      46 POP_JUMP_FORWARD_IF_TRUE    35 (to 118)
          
-          17          44 LOAD_GLOBAL              5 (NULL + json_to_dict)
-                      56 LOAD_FAST                0 (parser_result_data)
-                      58 PRECALL                  1
-                      62 CALL                     1
-                      72 STORE_FAST               0 (parser_result_data)
-         
-          19     >>   74 LOAD_GLOBAL              7 (NULL + validate_parser_result)
-                      86 LOAD_FAST                0 (parser_result_data)
-                      88 PRECALL                  1
-                      92 CALL                     1
-                     102 STORE_FAST               1 (data_object)
-         
-          21         104 LOAD_GLOBAL              9 (NULL + globals)
-                     116 PRECALL                  0
-                     120 CALL                     0
-                     130 LOAD_FAST                1 (data_object)
-                     132 LOAD_ATTR                5 (method)
-                     142 BINARY_SUBSCR
-                     152 STORE_FAST               2 (method_to_execute)
-         
-          22         154 PUSH_NULL
-                     156 LOAD_FAST                2 (method_to_execute)
-                     158 LOAD_FAST                1 (data_object)
-                     160 PRECALL                  1
-                     164 CALL                     1
-                     174 POP_TOP
-                     176 LOAD_CONST               0 (None)
-                     178 RETURN_VALUE
+          14          48 LOAD_GLOBAL              5 (NULL + print)
+                      60 LOAD_CONST               1 ('You provided an empty JSON, please review your code')
+                      62 PRECALL                  1
+                      66 CALL                     1
+                      76 POP_TOP
+         
+          15          78 LOAD_GLOBAL              7 (NULL + sys)
+                      90 LOAD_ATTR                4 (exit)
+                     100 LOAD_CONST               2 (1)
+                     102 PRECALL                  1
+                     106 CALL                     1
+                     116 POP_TOP
+         
+          17     >>  118 LOAD_GLOBAL             11 (NULL + json_to_dict)
+                     130 LOAD_FAST                0 (parser_result_data)
+                     132 PRECALL                  1
+                     136 CALL                     1
+                     146 STORE_FAST               0 (parser_result_data)
+         
+          19     >>  148 LOAD_FAST                0 (parser_result_data)
+                     150 POP_JUMP_FORWARD_IF_TRUE    35 (to 222)
+         
+          20         152 LOAD_GLOBAL              5 (NULL + print)
+                     164 LOAD_CONST               3 ('You provided an empty dict, please review your code')
+                     166 PRECALL                  1
+                     170 CALL                     1
+                     180 POP_TOP
+         
+          21         182 LOAD_GLOBAL              7 (NULL + sys)
+                     194 LOAD_ATTR                4 (exit)
+                     204 LOAD_CONST               2 (1)
+                     206 PRECALL                  1
+                     210 CALL                     1
+                     220 POP_TOP
+         
+          23     >>  222 LOAD_GLOBAL             13 (NULL + validate_parser_result)
+                     234 LOAD_FAST                0 (parser_result_data)
+                     236 PRECALL                  1
+                     240 CALL                     1
+                     250 STORE_FAST               1 (data_object)
+         
+          25         252 LOAD_FAST                1 (data_object)
+                     254 LOAD_ATTR                7 (method)
+                     264 LOAD_CONST               4 ('*')
+                     266 COMPARE_OP               3 (!=)
+                     272 POP_JUMP_FORWARD_IF_FALSE    36 (to 346)
+         
+          26         274 LOAD_GLOBAL             17 (NULL + globals)
+                     286 PRECALL                  0
+                     290 CALL                     0
+                     300 LOAD_FAST                1 (data_object)
+                     302 LOAD_ATTR                7 (method)
+                     312 BINARY_SUBSCR
+                     322 STORE_FAST               2 (method_to_execute)
+         
+          27         324 PUSH_NULL
+                     326 LOAD_FAST                2 (method_to_execute)
+                     328 LOAD_FAST                1 (data_object)
+                     330 PRECALL                  1
+                     334 CALL                     1
+                     344 RETURN_VALUE
+         
+          29     >>  346 LOAD_GLOBAL             19 (NULL + all_methods)
+                     358 PRECALL                  0
+                     362 CALL                     0
+                     372 LOAD_FAST                1 (data_object)
+                     374 STORE_ATTR               7 (method)
+         
+          30         384 LOAD_GLOBAL             21 (NULL + send_parser)
+                     396 LOAD_FAST                1 (data_object)
+                     398 PRECALL                  1
+                     402 CALL                     1
+                     412 RETURN_VALUE
          consts
             None
-         names      ('isinstance', 'str', 'json_to_dict', 'validate_parser_result', 'globals', 'method')
+            'You provided an empty JSON, please review your code'
+            1
+            'You provided an empty dict, please review your code'
+            '*'
+         names      ('isinstance', 'str', 'print', 'sys', 'exit', 'json_to_dict', 'validate_parser_result', 'method', 'globals', 'all_methods', 'send_parser')
          varnames   ('parser_result_data', 'data_object', 'method_to_execute')
          freevars   ()
          cellvars   ()
-         filename   'D:\\Proyectos\\ParserResult\\parser_result\\__init__.py'
+         filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\cfx_middleware.py'
          name       'parser_result'
-         firstlineno 15
-         lnotab 0x02012a011e021e023201
+         firstlineno 10
+         lnotab 0x02022a0104011e0128021e0204011e0128021e021601320116022601
       'parser_result'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
          code
             0x970009007401000000000000000000007c00a6010000ab010000000000
-            00000001007403000000000000000000007c006401190000000000000000
-            00a6010000ab010000000000000000010074050000000000000000000064
-            0769007c00a4018e01530023007406000000000000000000002400723e7d
-            017409000000000000000000006402740b000000000000000000007c01a6
-            010000ab0100000000000000007a000000a6010000ab0100000000000000
-            000100740d000000000000000000006a0700000000000000006403a60100
-            00ab0100000000000000000100590064007d017e016400530064007d017e
-            0177017410000000000000000000002400723e7d02740900000000000000
-            0000006404740b000000000000000000007c02a6010000ab010000000000
-            0000007a000000a6010000ab0100000000000000000100740d0000000000
-            00000000006a0700000000000000006403a6010000ab0100000000000000
-            000100590064007d027e026400530064007d027e02770174120000000000
-            00000000002400723e7d037409000000000000000000006405740b000000
-            000000000000007c03a6010000ab0100000000000000007a000000a60100
-            00ab0100000000000000000100740d000000000000000000006a07000000
-            00000000006403a6010000ab0100000000000000000100590064007d037e
-            036400530064007d037e0377017414000000000000000000002400723e7d
-            047409000000000000000000006406740b000000000000000000007c04a6
-            010000ab0100000000000000007a000000a6010000ab0100000000000000
-            000100740d000000000000000000006a0700000000000000006403a60100
-            00ab0100000000000000000100590064007d047e046400530064007d047e
-            0477017700780359007701
-          25           0 RESUME                   0
+            00000001007c0064011900000000000000000064026b0300000000721574
+            03000000000000000000007c00640119000000000000000000a6010000ab
+            0100000000000000000100740500000000000000000000640869007c00a4
+            018e01530023007406000000000000000000002400723e7d017409000000
+            000000000000006403740b000000000000000000007c01a6010000ab0100
+            000000000000007a000000a6010000ab0100000000000000000100740d00
+            0000000000000000006a0700000000000000006404a6010000ab01000000
+            00000000000100590064007d017e016400530064007d017e017701741000
+            0000000000000000002400723e7d02740900000000000000000000640574
+            0b000000000000000000007c02a6010000ab0100000000000000007a0000
+            00a6010000ab0100000000000000000100740d000000000000000000006a
+            0700000000000000006404a6010000ab0100000000000000000100590064
+            007d027e026400530064007d027e02770174120000000000000000000024
+            00723e7d037409000000000000000000006406740b000000000000000000
+            007c03a6010000ab0100000000000000007a000000a6010000ab01000000
+            00000000000100740d000000000000000000006a07000000000000000064
+            04a6010000ab0100000000000000000100590064007d037e036400530064
+            007d037e0377017414000000000000000000002400723e7d047409000000
+            000000000000006407740b000000000000000000007c04a6010000ab0100
+            000000000000007a000000a6010000ab0100000000000000000100740d00
+            0000000000000000006a0700000000000000006404a6010000ab01000000
+            00000000000100590064007d047e046400530064007d047e047701770078
+            0359007701
+          33           0 RESUME                   0
          
-          26           2 NOP
+          34           2 NOP
          
-          28           4 LOAD_GLOBAL              1 (NULL + is_dict)
+          36           4 LOAD_GLOBAL              1 (NULL + is_dict)
                       16 LOAD_FAST                0 (parser_result)
                       18 PRECALL                  1
                       22 CALL                     1
                       32 POP_TOP
          
-          30          34 LOAD_GLOBAL              3 (NULL + validate_method)
-                      46 LOAD_FAST                0 (parser_result)
-                      48 LOAD_CONST               1 ('Method')
-                      50 BINARY_SUBSCR
-                      60 PRECALL                  1
-                      64 CALL                     1
-                      74 POP_TOP
-         
-          32          76 LOAD_GLOBAL              5 (NULL + ParserResult)
-                      88 LOAD_CONST               7 (())
-                      90 BUILD_MAP                0
-                      92 LOAD_FAST                0 (parser_result)
-                      94 DICT_MERGE               1
-                      96 CALL_FUNCTION_EX         1
-                      98 RETURN_VALUE
-                 >>  100 PUSH_EXC_INFO
-         
-          33         102 LOAD_GLOBAL              6 (ValueError)
-                     114 CHECK_EXC_MATCH
-                     116 POP_JUMP_FORWARD_IF_FALSE    62 (to 242)
-                     118 STORE_FAST               1 (ve)
-         
-          34         120 LOAD_GLOBAL              9 (NULL + print)
-                     132 LOAD_CONST               2 ('Value Error: ')
-                     134 LOAD_GLOBAL             11 (NULL + str)
-                     146 LOAD_FAST                1 (ve)
-                     148 PRECALL                  1
-                     152 CALL                     1
-                     162 BINARY_OP                0 (+)
-                     166 PRECALL                  1
-                     170 CALL                     1
-                     180 POP_TOP
-         
-          35         182 LOAD_GLOBAL             13 (NULL + sys)
-                     194 LOAD_ATTR                7 (exit)
-                     204 LOAD_CONST               3 (1)
-                     206 PRECALL                  1
-                     210 CALL                     1
-                     220 POP_TOP
-                     222 POP_EXCEPT
-                     224 LOAD_CONST               0 (None)
-                     226 STORE_FAST               1 (ve)
-                     228 DELETE_FAST              1 (ve)
-                     230 LOAD_CONST               0 (None)
-                     232 RETURN_VALUE
-                 >>  234 LOAD_CONST               0 (None)
-                     236 STORE_FAST               1 (ve)
-                     238 DELETE_FAST              1 (ve)
-                     240 RERAISE                  1
-         
-          36     >>  242 LOAD_GLOBAL             16 (TypeError)
-                     254 CHECK_EXC_MATCH
-                     256 POP_JUMP_FORWARD_IF_FALSE    62 (to 382)
-                     258 STORE_FAST               2 (te)
-         
-          37         260 LOAD_GLOBAL              9 (NULL + print)
-                     272 LOAD_CONST               4 ('Type Error: ')
-                     274 LOAD_GLOBAL             11 (NULL + str)
-                     286 LOAD_FAST                2 (te)
-                     288 PRECALL                  1
-                     292 CALL                     1
-                     302 BINARY_OP                0 (+)
-                     306 PRECALL                  1
-                     310 CALL                     1
-                     320 POP_TOP
-         
-          38         322 LOAD_GLOBAL             13 (NULL + sys)
-                     334 LOAD_ATTR                7 (exit)
-                     344 LOAD_CONST               3 (1)
-                     346 PRECALL                  1
-                     350 CALL                     1
-                     360 POP_TOP
-                     362 POP_EXCEPT
-                     364 LOAD_CONST               0 (None)
-                     366 STORE_FAST               2 (te)
-                     368 DELETE_FAST              2 (te)
-                     370 LOAD_CONST               0 (None)
-                     372 RETURN_VALUE
-                 >>  374 LOAD_CONST               0 (None)
-                     376 STORE_FAST               2 (te)
-                     378 DELETE_FAST              2 (te)
-                     380 RERAISE                  1
-         
-          39     >>  382 LOAD_GLOBAL             18 (NotDictException)
-                     394 CHECK_EXC_MATCH
-                     396 POP_JUMP_FORWARD_IF_FALSE    62 (to 522)
-                     398 STORE_FAST               3 (nde)
-         
-          40         400 LOAD_GLOBAL              9 (NULL + print)
-                     412 LOAD_CONST               5 ('Dict Error: ')
-                     414 LOAD_GLOBAL             11 (NULL + str)
-                     426 LOAD_FAST                3 (nde)
-                     428 PRECALL                  1
-                     432 CALL                     1
-                     442 BINARY_OP                0 (+)
-                     446 PRECALL                  1
-                     450 CALL                     1
-                     460 POP_TOP
-         
-          41         462 LOAD_GLOBAL             13 (NULL + sys)
-                     474 LOAD_ATTR                7 (exit)
-                     484 LOAD_CONST               3 (1)
-                     486 PRECALL                  1
-                     490 CALL                     1
-                     500 POP_TOP
-                     502 POP_EXCEPT
-                     504 LOAD_CONST               0 (None)
-                     506 STORE_FAST               3 (nde)
-                     508 DELETE_FAST              3 (nde)
-                     510 LOAD_CONST               0 (None)
-                     512 RETURN_VALUE
-                 >>  514 LOAD_CONST               0 (None)
-                     516 STORE_FAST               3 (nde)
-                     518 DELETE_FAST              3 (nde)
-                     520 RERAISE                  1
-         
-          42     >>  522 LOAD_GLOBAL             20 (MethodNotValid)
-                     534 CHECK_EXC_MATCH
-                     536 POP_JUMP_FORWARD_IF_FALSE    62 (to 662)
-                     538 STORE_FAST               4 (mnv)
-         
-          43         540 LOAD_GLOBAL              9 (NULL + print)
-                     552 LOAD_CONST               6 ('Method Error: ')
-                     554 LOAD_GLOBAL             11 (NULL + str)
-                     566 LOAD_FAST                4 (mnv)
-                     568 PRECALL                  1
-                     572 CALL                     1
-                     582 BINARY_OP                0 (+)
-                     586 PRECALL                  1
-                     590 CALL                     1
-                     600 POP_TOP
-         
-          44         602 LOAD_GLOBAL             13 (NULL + sys)
-                     614 LOAD_ATTR                7 (exit)
-                     624 LOAD_CONST               3 (1)
-                     626 PRECALL                  1
-                     630 CALL                     1
-                     640 POP_TOP
-                     642 POP_EXCEPT
-                     644 LOAD_CONST               0 (None)
-                     646 STORE_FAST               4 (mnv)
-                     648 DELETE_FAST              4 (mnv)
-                     650 LOAD_CONST               0 (None)
-                     652 RETURN_VALUE
-                 >>  654 LOAD_CONST               0 (None)
-                     656 STORE_FAST               4 (mnv)
-                     658 DELETE_FAST              4 (mnv)
-                     660 RERAISE                  1
-         
-          42     >>  662 RERAISE                  0
-                 >>  664 COPY                     3
+          38          34 LOAD_FAST                0 (parser_result)
+                      36 LOAD_CONST               1 ('Method')
+                      38 BINARY_SUBSCR
+                      48 LOAD_CONST               2 ('*')
+                      50 COMPARE_OP               3 (!=)
+                      56 POP_JUMP_FORWARD_IF_FALSE    21 (to 100)
+         
+          39          58 LOAD_GLOBAL              3 (NULL + validate_method)
+                      70 LOAD_FAST                0 (parser_result)
+                      72 LOAD_CONST               1 ('Method')
+                      74 BINARY_SUBSCR
+                      84 PRECALL                  1
+                      88 CALL                     1
+                      98 POP_TOP
+         
+          41     >>  100 LOAD_GLOBAL              5 (NULL + ParserResult)
+                     112 LOAD_CONST               8 (())
+                     114 BUILD_MAP                0
+                     116 LOAD_FAST                0 (parser_result)
+                     118 DICT_MERGE               1
+                     120 CALL_FUNCTION_EX         1
+                     122 RETURN_VALUE
+                 >>  124 PUSH_EXC_INFO
+         
+          42         126 LOAD_GLOBAL              6 (ValueError)
+                     138 CHECK_EXC_MATCH
+                     140 POP_JUMP_FORWARD_IF_FALSE    62 (to 266)
+                     142 STORE_FAST               1 (ve)
+         
+          43         144 LOAD_GLOBAL              9 (NULL + print)
+                     156 LOAD_CONST               3 ('Value Error: ')
+                     158 LOAD_GLOBAL             11 (NULL + str)
+                     170 LOAD_FAST                1 (ve)
+                     172 PRECALL                  1
+                     176 CALL                     1
+                     186 BINARY_OP                0 (+)
+                     190 PRECALL                  1
+                     194 CALL                     1
+                     204 POP_TOP
+         
+          44         206 LOAD_GLOBAL             13 (NULL + sys)
+                     218 LOAD_ATTR                7 (exit)
+                     228 LOAD_CONST               4 (1)
+                     230 PRECALL                  1
+                     234 CALL                     1
+                     244 POP_TOP
+                     246 POP_EXCEPT
+                     248 LOAD_CONST               0 (None)
+                     250 STORE_FAST               1 (ve)
+                     252 DELETE_FAST              1 (ve)
+                     254 LOAD_CONST               0 (None)
+                     256 RETURN_VALUE
+                 >>  258 LOAD_CONST               0 (None)
+                     260 STORE_FAST               1 (ve)
+                     262 DELETE_FAST              1 (ve)
+                     264 RERAISE                  1
+         
+          45     >>  266 LOAD_GLOBAL             16 (TypeError)
+                     278 CHECK_EXC_MATCH
+                     280 POP_JUMP_FORWARD_IF_FALSE    62 (to 406)
+                     282 STORE_FAST               2 (te)
+         
+          46         284 LOAD_GLOBAL              9 (NULL + print)
+                     296 LOAD_CONST               5 ('Type Error: ')
+                     298 LOAD_GLOBAL             11 (NULL + str)
+                     310 LOAD_FAST                2 (te)
+                     312 PRECALL                  1
+                     316 CALL                     1
+                     326 BINARY_OP                0 (+)
+                     330 PRECALL                  1
+                     334 CALL                     1
+                     344 POP_TOP
+         
+          47         346 LOAD_GLOBAL             13 (NULL + sys)
+                     358 LOAD_ATTR                7 (exit)
+                     368 LOAD_CONST               4 (1)
+                     370 PRECALL                  1
+                     374 CALL                     1
+                     384 POP_TOP
+                     386 POP_EXCEPT
+                     388 LOAD_CONST               0 (None)
+                     390 STORE_FAST               2 (te)
+                     392 DELETE_FAST              2 (te)
+                     394 LOAD_CONST               0 (None)
+                     396 RETURN_VALUE
+                 >>  398 LOAD_CONST               0 (None)
+                     400 STORE_FAST               2 (te)
+                     402 DELETE_FAST              2 (te)
+                     404 RERAISE                  1
+         
+          48     >>  406 LOAD_GLOBAL             18 (NotDictException)
+                     418 CHECK_EXC_MATCH
+                     420 POP_JUMP_FORWARD_IF_FALSE    62 (to 546)
+                     422 STORE_FAST               3 (nde)
+         
+          49         424 LOAD_GLOBAL              9 (NULL + print)
+                     436 LOAD_CONST               6 ('Dict Error: ')
+                     438 LOAD_GLOBAL             11 (NULL + str)
+                     450 LOAD_FAST                3 (nde)
+                     452 PRECALL                  1
+                     456 CALL                     1
+                     466 BINARY_OP                0 (+)
+                     470 PRECALL                  1
+                     474 CALL                     1
+                     484 POP_TOP
+         
+          50         486 LOAD_GLOBAL             13 (NULL + sys)
+                     498 LOAD_ATTR                7 (exit)
+                     508 LOAD_CONST               4 (1)
+                     510 PRECALL                  1
+                     514 CALL                     1
+                     524 POP_TOP
+                     526 POP_EXCEPT
+                     528 LOAD_CONST               0 (None)
+                     530 STORE_FAST               3 (nde)
+                     532 DELETE_FAST              3 (nde)
+                     534 LOAD_CONST               0 (None)
+                     536 RETURN_VALUE
+                 >>  538 LOAD_CONST               0 (None)
+                     540 STORE_FAST               3 (nde)
+                     542 DELETE_FAST              3 (nde)
+                     544 RERAISE                  1
+         
+          51     >>  546 LOAD_GLOBAL             20 (MethodNotValid)
+                     558 CHECK_EXC_MATCH
+                     560 POP_JUMP_FORWARD_IF_FALSE    62 (to 686)
+                     562 STORE_FAST               4 (mnv)
+         
+          52         564 LOAD_GLOBAL              9 (NULL + print)
+                     576 LOAD_CONST               7 ('Method Error: ')
+                     578 LOAD_GLOBAL             11 (NULL + str)
+                     590 LOAD_FAST                4 (mnv)
+                     592 PRECALL                  1
+                     596 CALL                     1
+                     606 BINARY_OP                0 (+)
+                     610 PRECALL                  1
+                     614 CALL                     1
+                     624 POP_TOP
+         
+          53         626 LOAD_GLOBAL             13 (NULL + sys)
+                     638 LOAD_ATTR                7 (exit)
+                     648 LOAD_CONST               4 (1)
+                     650 PRECALL                  1
+                     654 CALL                     1
+                     664 POP_TOP
                      666 POP_EXCEPT
-                     668 RERAISE                  1
+                     668 LOAD_CONST               0 (None)
+                     670 STORE_FAST               4 (mnv)
+                     672 DELETE_FAST              4 (mnv)
+                     674 LOAD_CONST               0 (None)
+                     676 RETURN_VALUE
+                 >>  678 LOAD_CONST               0 (None)
+                     680 STORE_FAST               4 (mnv)
+                     682 DELETE_FAST              4 (mnv)
+                     684 RERAISE                  1
+         
+          51     >>  686 RERAISE                  0
+                 >>  688 COPY                     3
+                     690 POP_EXCEPT
+                     692 RERAISE                  1
          ExceptionTable:
-           4 to 96 -> 100 [0]
-           100 to 118 -> 664 [1] lasti
-           120 to 220 -> 234 [1] lasti
-           234 to 258 -> 664 [1] lasti
-           260 to 360 -> 374 [1] lasti
-           374 to 398 -> 664 [1] lasti
-           400 to 500 -> 514 [1] lasti
-           514 to 538 -> 664 [1] lasti
-           540 to 640 -> 654 [1] lasti
-           654 to 662 -> 664 [1] lasti
+           4 to 120 -> 124 [0]
+           124 to 142 -> 688 [1] lasti
+           144 to 244 -> 258 [1] lasti
+           258 to 282 -> 688 [1] lasti
+           284 to 384 -> 398 [1] lasti
+           398 to 422 -> 688 [1] lasti
+           424 to 524 -> 538 [1] lasti
+           538 to 562 -> 688 [1] lasti
+           564 to 664 -> 678 [1] lasti
+           678 to 686 -> 688 [1] lasti
          consts
             None
             'Method'
+            '*'
             'Value Error: '
             1
             'Type Error: '
             'Dict Error: '
             'Method Error: '
             ()
          names      ('is_dict', 'validate_method', 'ParserResult', 'ValueError', 'print', 'str', 'sys', 'exit', 'TypeError', 'NotDictException', 'MethodNotValid')
          varnames   ('parser_result', 've', 'te', 'nde', 'mnv')
          freevars   ()
          cellvars   ()
-         filename   'D:\\Proyectos\\ParserResult\\parser_result\\__init__.py'
+         filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\cfx_middleware.py'
          name       'validate_parser_result'
-         firstlineno 25
+         firstlineno 33
          lnotab
-            0x020102021e022a021a0112013e013c0112013e013c0112013e013c0112
-            013e013cfe
+            0x020102021e0218012a021a0112013e013c0112013e013c0112013e013c
+            0112013e013cfe
+      code
+         argcount  : 1
+         nlocals   : 2
+         stacksize : 3
+         flags     : 3
+         code
+            0x97007401000000000000000000007c00a6010000ab0100000000000000
+            007d017403000000000000000000007c01a6010000ab0100000000000000
+            0001007403000000000000000000006401a6010000ab0100000000000000
+            00010064025300
+          56           0 RESUME                   0
+         
+          57           2 LOAD_GLOBAL              1 (NULL + class_to_json)
+                      14 LOAD_FAST                0 (parser_result)
+                      16 PRECALL                  1
+                      20 CALL                     1
+                      30 STORE_FAST               1 (data_converted)
+         
+          58          32 LOAD_GLOBAL              3 (NULL + print)
+                      44 LOAD_FAST                1 (data_converted)
+                      46 PRECALL                  1
+                      50 CALL                     1
+                      60 POP_TOP
+         
+          59          62 LOAD_GLOBAL              3 (NULL + print)
+                      74 LOAD_CONST               1 ('Parser Result send to Queue')
+                      76 PRECALL                  1
+                      80 CALL                     1
+                      90 POP_TOP
+         
+          60          92 LOAD_CONST               2 (True)
+                      94 RETURN_VALUE
+         consts
+            None
+            'Parser Result send to Queue'
+            True
+         names      ('class_to_json', 'print')
+         varnames   ('parser_result', 'data_converted')
+         freevars   ()
+         cellvars   ()
+         filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\cfx_middleware.py'
+         name       'send_parser'
+         firstlineno 56
+         lnotab 0x02011e011e011e01
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
-            007d017403000000000000000000006a0100000000000000007c01a60100
-            00ab01000000000000000001007405000000000000000000006401a60100
-            00ab010000000000000000010064005300
-          47           0 RESUME                   0
+            007d017403000000000000000000007c01a6010000ab0100000000000000
+            0001007403000000000000000000006401a6010000ab0100000000000000
+            00010064025300
+          63           0 RESUME                   0
          
-          48           2 LOAD_GLOBAL              1 (NULL + class_to_json)
+          64           2 LOAD_GLOBAL              1 (NULL + class_to_json)
                       14 LOAD_FAST                0 (parser_result)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 STORE_FAST               1 (data_converted)
          
-          50          32 LOAD_GLOBAL              3 (NULL + pprint)
-                      44 LOAD_ATTR                1 (pprint)
-                      54 LOAD_FAST                1 (data_converted)
-                      56 PRECALL                  1
-                      60 CALL                     1
-                      70 POP_TOP
-         
-          51          72 LOAD_GLOBAL              5 (NULL + print)
-                      84 LOAD_CONST               1 ('validate_units')
-                      86 PRECALL                  1
-                      90 CALL                     1
-                     100 POP_TOP
-                     102 LOAD_CONST               0 (None)
-                     104 RETURN_VALUE
+          65          32 LOAD_GLOBAL              3 (NULL + print)
+                      44 LOAD_FAST                1 (data_converted)
+                      46 PRECALL                  1
+                      50 CALL                     1
+                      60 POP_TOP
+         
+          66          62 LOAD_GLOBAL              3 (NULL + print)
+                      74 LOAD_CONST               1 ('Method to execute validate_units')
+                      76 PRECALL                  1
+                      80 CALL                     1
+                      90 POP_TOP
+         
+          67          92 LOAD_CONST               2 (True)
+                      94 RETURN_VALUE
          consts
             None
-            'validate_units'
-         names      ('class_to_json', 'pprint', 'print')
+            'Method to execute validate_units'
+            True
+         names      ('class_to_json', 'print')
          varnames   ('parser_result', 'data_converted')
          freevars   ()
          cellvars   ()
-         filename   'D:\\Proyectos\\ParserResult\\parser_result\\__init__.py'
+         filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\cfx_middleware.py'
          name       'validate_units'
-         firstlineno 47
-         lnotab 0x02011e022801
+         firstlineno 63
+         lnotab 0x02011e011e011e01
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
-            007d017403000000000000000000006a0100000000000000007c01a60100
-            00ab01000000000000000001007405000000000000000000006401a60100
-            00ab010000000000000000010064005300
-          54           0 RESUME                   0
+            007d017403000000000000000000007c01a6010000ab0100000000000000
+            0001007403000000000000000000006401a6010000ab0100000000000000
+            00010064025300
+          70           0 RESUME                   0
          
-          55           2 LOAD_GLOBAL              1 (NULL + class_to_json)
+          71           2 LOAD_GLOBAL              1 (NULL + class_to_json)
                       14 LOAD_FAST                0 (parser_result)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 STORE_FAST               1 (data_converted)
          
-          57          32 LOAD_GLOBAL              3 (NULL + pprint)
-                      44 LOAD_ATTR                1 (pprint)
-                      54 LOAD_FAST                1 (data_converted)
-                      56 PRECALL                  1
-                      60 CALL                     1
-                      70 POP_TOP
-         
-          58          72 LOAD_GLOBAL              5 (NULL + print)
-                      84 LOAD_CONST               1 ('units_inspected')
-                      86 PRECALL                  1
-                      90 CALL                     1
-                     100 POP_TOP
-                     102 LOAD_CONST               0 (None)
-                     104 RETURN_VALUE
+          72          32 LOAD_GLOBAL              3 (NULL + print)
+                      44 LOAD_FAST                1 (data_converted)
+                      46 PRECALL                  1
+                      50 CALL                     1
+                      60 POP_TOP
+         
+          73          62 LOAD_GLOBAL              3 (NULL + print)
+                      74 LOAD_CONST               1 ('Method to execute units_inspected')
+                      76 PRECALL                  1
+                      80 CALL                     1
+                      90 POP_TOP
+         
+          74          92 LOAD_CONST               2 (True)
+                      94 RETURN_VALUE
          consts
             None
-            'units_inspected'
-         names      ('class_to_json', 'pprint', 'print')
+            'Method to execute units_inspected'
+            True
+         names      ('class_to_json', 'print')
          varnames   ('parser_result', 'data_converted')
          freevars   ()
          cellvars   ()
-         filename   'D:\\Proyectos\\ParserResult\\parser_result\\__init__.py'
+         filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\cfx_middleware.py'
          name       'units_inspected'
-         firstlineno 54
-         lnotab 0x02011e022801
+         firstlineno 70
+         lnotab 0x02011e011e011e01
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
-            007d017403000000000000000000006a0100000000000000007c01a60100
-            00ab01000000000000000001007405000000000000000000006401a60100
-            00ab010000000000000000010064005300
-          61           0 RESUME                   0
+            007d017403000000000000000000007c01a6010000ab0100000000000000
+            0001007403000000000000000000006401a6010000ab0100000000000000
+            00010064025300
+          77           0 RESUME                   0
          
-          62           2 LOAD_GLOBAL              1 (NULL + class_to_json)
+          78           2 LOAD_GLOBAL              1 (NULL + class_to_json)
                       14 LOAD_FAST                0 (parser_result)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 STORE_FAST               1 (data_converted)
          
-          64          32 LOAD_GLOBAL              3 (NULL + pprint)
-                      44 LOAD_ATTR                1 (pprint)
-                      54 LOAD_FAST                1 (data_converted)
-                      56 PRECALL                  1
-                      60 CALL                     1
-                      70 POP_TOP
-         
-          65          72 LOAD_GLOBAL              5 (NULL + print)
-                      84 LOAD_CONST               1 ('units_departed')
-                      86 PRECALL                  1
-                      90 CALL                     1
-                     100 POP_TOP
-                     102 LOAD_CONST               0 (None)
-                     104 RETURN_VALUE
+          79          32 LOAD_GLOBAL              3 (NULL + print)
+                      44 LOAD_FAST                1 (data_converted)
+                      46 PRECALL                  1
+                      50 CALL                     1
+                      60 POP_TOP
+         
+          80          62 LOAD_GLOBAL              3 (NULL + print)
+                      74 LOAD_CONST               1 ('Method to execute units_departed')
+                      76 PRECALL                  1
+                      80 CALL                     1
+                      90 POP_TOP
+         
+          81          92 LOAD_CONST               2 (True)
+                      94 RETURN_VALUE
          consts
             None
-            'units_departed'
-         names      ('class_to_json', 'pprint', 'print')
+            'Method to execute units_departed'
+            True
+         names      ('class_to_json', 'print')
          varnames   ('parser_result', 'data_converted')
          freevars   ()
          cellvars   ()
-         filename   'D:\\Proyectos\\ParserResult\\parser_result\\__init__.py'
+         filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\cfx_middleware.py'
          name       'units_departed'
-         firstlineno 61
-         lnotab 0x02011e022801
+         firstlineno 77
+         lnotab 0x02011e011e011e01
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
-            007d017403000000000000000000006a0100000000000000007c01a60100
-            00ab01000000000000000001007405000000000000000000006401a60100
-            00ab010000000000000000010064005300
-          68           0 RESUME                   0
+            007d017403000000000000000000007c01a6010000ab0100000000000000
+            0001007403000000000000000000006401a6010000ab0100000000000000
+            00010064025300
+          84           0 RESUME                   0
          
-          69           2 LOAD_GLOBAL              1 (NULL + class_to_json)
+          85           2 LOAD_GLOBAL              1 (NULL + class_to_json)
                       14 LOAD_FAST                0 (parser_result)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 STORE_FAST               1 (data_converted)
          
-          71          32 LOAD_GLOBAL              3 (NULL + pprint)
-                      44 LOAD_ATTR                1 (pprint)
-                      54 LOAD_FAST                1 (data_converted)
-                      56 PRECALL                  1
-                      60 CALL                     1
-                      70 POP_TOP
-         
-          72          72 LOAD_GLOBAL              5 (NULL + print)
-                      84 LOAD_CONST               1 ('state_change')
-                      86 PRECALL                  1
-                      90 CALL                     1
-                     100 POP_TOP
-                     102 LOAD_CONST               0 (None)
-                     104 RETURN_VALUE
+          86          32 LOAD_GLOBAL              3 (NULL + print)
+                      44 LOAD_FAST                1 (data_converted)
+                      46 PRECALL                  1
+                      50 CALL                     1
+                      60 POP_TOP
+         
+          87          62 LOAD_GLOBAL              3 (NULL + print)
+                      74 LOAD_CONST               1 ('Method to execute state_change')
+                      76 PRECALL                  1
+                      80 CALL                     1
+                      90 POP_TOP
+         
+          88          92 LOAD_CONST               2 (True)
+                      94 RETURN_VALUE
          consts
             None
-            'state_change'
-         names      ('class_to_json', 'pprint', 'print')
+            'Method to execute state_change'
+            True
+         names      ('class_to_json', 'print')
          varnames   ('parser_result', 'data_converted')
          freevars   ()
          cellvars   ()
-         filename   'D:\\Proyectos\\ParserResult\\parser_result\\__init__.py'
+         filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\cfx_middleware.py'
          name       'state_change'
-         firstlineno 68
-         lnotab 0x02011e022801
+         firstlineno 84
+         lnotab 0x02011e011e011e01
       '__main__'
       'SerialNumber'
       'P69660003012311280100684'
       'Sequence'
       'None'
       'Assembly'
       '6966-0003-01'
@@ -807,39 +886,40 @@
       'SAUL RUIZ'
       'StartTime'
       '2023-11-29T10:24:31'
       'EndTime'
       '2023-11-29T10:24:46'
       'MachineId'
       'AOI-L16'
+      'IoTId'
+      '84968468'
       'ProgramName'
       '6966-0003-01_BOT'
       'LogFileName'
       'Remarks'
-      'IsBirth'
       ('RecipeName', 'RecipeRevision')
-      'units_inspecteds'
+      'units_inspected'
       ''
       'ST5901_Polarity3_Polarity_AI2-3D-1_AI2_3D_ConfidenceLevel'
       5
       'OK'
       '1'
       '100'
       '82.3721508947464'
       ('TestName', 'Sequence', 'PassFail', 'LowLimit', 'HighLimit', 'Value', 'IsCritical', 'Defect', 'ErrorCode', 'ErrorLocation', 'ErrorMessage', 'Parameters')
       ('SerialNumber', 'Sequence', 'TestResult', 'PassFail')
-      ('Parameters', 'TestResults', 'Method', 'ChildSerialNumbers')
-   names      ('sys', 'json', 'dotenv', 'dotenv_values', 'pprint', 'parser_result.classes.ParserResult', 'ParserResult', 'parser_result.exceptions.NotDictException', 'NotDictException', 'is_dict', 'parser_result.exceptions.MethodNotValid', 'MethodNotValid', 'validate_method', 'parser_result.helpers.utils', 'class_to_json', 'json_to_dict', 'parser_result.rabbit.send_rabbit', 'send_message', 'get', 'RABBITMQ_EXCHANGE_PARSER_QUEUE', 'parser_result', 'dict', 'validate_parser_result', 'validate_units', 'units_inspected', 'units_departed', 'state_change', '__name__')
+      ('IsBirth', 'Parameters', 'TestResults', 'Method', 'ChildSerialNumbers')
+      'Success '
+   names      ('sys', 'cfx_middleware.classes.ParserResult', 'ParserResult', 'cfx_middleware.exceptions.NotDictException', 'NotDictException', 'is_dict', 'cfx_middleware.exceptions.MethodNotValid', 'MethodNotValid', 'validate_method', 'cfx_middleware.helpers.utils', 'class_to_json', 'json_to_dict', 'all_methods', 'cfx_middleware.rabbit.send_rabbit', 'send_message', 'parser_result', 'dict', 'validate_parser_result', 'send_parser', 'validate_units', 'units_inspected', 'units_departed', 'state_change', '__name__', 'success', 'print')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'D:\\Proyectos\\ParserResult\\parser_result\\__init__.py'
+   filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\cfx_middleware.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff0201080108010c0108020c011001100110010c023a03060a0c160c
-      070c070c070c070c010401020104ff020204fe020304fd020404fc020504
-      fb020604fa020704f9020804f8020904f7020a04f6020b04f5020c04f402
-      0d04f3020e04f2020f04f1021004f0021104ef0212080102010203020102
-      030201020102010201020102010201020102010201020102f4040f020102
-      0102010201020102010201020102010201020102f404f1021e02df04ff02
-      eb06ff14ff
+      0x00ff020108020c011001100114010c0306170c170c070c070c070c070c
+      070c010401020104ff020204fe020304fd020404fc020504fb020604fa02
+      0704f9020804f8020904f7020a04f6020b04f5020c04f4020d04f3020e04
+      f2020f04f1021004f0021104ef0212020108010201020302010203020102
+      0102010201020102010201020102010201020102f404ff021002ed04ff02
+      ea06ff103120ce
```

### Comparing `cfx_middleware-2.1/cfx_middleware/cfx_middleware.py` & `cfx_middleware-3.0/cfx_middleware/cfx_middleware.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 
 from cfx_middleware.classes.ParserResult import ParserResult
 from cfx_middleware.exceptions.NotDictException import NotDictException, is_dict
 from cfx_middleware.exceptions.MethodNotValid import MethodNotValid, validate_method
-from cfx_middleware.helpers.utils import class_to_json, json_to_dict
+from cfx_middleware.helpers.utils import class_to_json, json_to_dict, all_methods
 from cfx_middleware.rabbit.send_rabbit import send_message
 
 
 def parser_result(parser_result_data):
 
     if isinstance(parser_result_data, str):
         if not parser_result_data:
@@ -18,24 +18,29 @@
 
     if not parser_result_data:
         print("You provided an empty dict, please review your code")
         sys.exit(1)
 
     data_object = validate_parser_result(parser_result_data)
 
-    method_to_execute = globals()[data_object.method]
-    return method_to_execute(data_object)
+    if data_object.method != "*":
+        method_to_execute = globals()[data_object.method]
+        return method_to_execute(data_object)
+    else:
+        data_object.method = all_methods()
+        return send_parser(data_object)
 
 
 def validate_parser_result(parser_result: dict):
     try:
         # Validate that data provided is Dict
         is_dict(parser_result)
         # Validate that method provided exists
-        validate_method(parser_result["Method"])
+        if parser_result["Method"] != "*":
+            validate_method(parser_result["Method"])
 
         return ParserResult(**parser_result)
     except ValueError as ve:
         print("Value Error: " + str(ve))
         sys.exit(1)
     except TypeError as te:
         print("Type Error: " + str(te))
@@ -44,14 +49,21 @@
         print("Dict Error: " + str(nde))
         sys.exit(1)
     except MethodNotValid as mnv:
         print("Method Error: " + str(mnv))
         sys.exit(1)
 
 
+def send_parser(parser_result: ParserResult):
+    data_converted = class_to_json(parser_result)
+    send_message(data_converted)
+    print("Parser Result send to Queue")
+    return True
+
+
 def validate_units(parser_result: ParserResult):
     data_converted = class_to_json(parser_result)
     send_message(data_converted)
     print("Method to execute validate_units")
     return True
 
 
@@ -108,28 +120,14 @@
                         {
                             "TestName": "ST5901_Polarity3_Polarity_AI2-3D-1_AI2_3D_ConfidenceLevel",
                             "Sequence": 5,
                             "PassFail": "OK",
                             "LowLimit": "1",
                             "HighLimit": "100",
                             "Value": "82.3721508947464",
-                            "IsCritical": True,
-                            "Defect": "None",
-                            "ErrorCode": "None",
-                            "ErrorLocation": "None",
-                            "ErrorMessage": "None",
-                            "Parameters": "None",
-                        },
-                        {
-                            "TestName": "ST5901_Polarity3_Polarity_AI2-3D-1_AI2_3D_ConfidenceLevel",
-                            "Sequence": 5,
-                            "PassFail": "OK",
-                            "LowLimit": "1",
-                            "HighLimit": "100",
-                            "Value": "82.3721508947464",
                             "IsCritical": True,
                             "Defect": "None",
                             "ErrorCode": "None",
                             "ErrorLocation": "None",
                             "ErrorMessage": "None",
                             "Parameters": "None",
                         },
```

### Comparing `cfx_middleware-2.1/cfx_middleware/classes/ChildSerialNumber.py` & `cfx_middleware-3.0/cfx_middleware/classes/ChildSerialNumber.py`

 * *Files identical despite different names*

### Comparing `cfx_middleware-2.1/cfx_middleware/classes/ParserResult.py` & `cfx_middleware-3.0/cfx_middleware/classes/ParserResult.py`

 * *Files identical despite different names*

### Comparing `cfx_middleware-2.1/cfx_middleware/classes/TestResult.py` & `cfx_middleware-3.0/cfx_middleware/classes/TestResult.py`

 * *Files identical despite different names*

### Comparing `cfx_middleware-2.1/cfx_middleware/classes/__pycache__/ChildSerialNumber.cpython-311.pyc` & `cfx_middleware-3.0/cfx_middleware/classes/__pycache__/ChildSerialNumber.cpython-311.pyc`

 * *Files 7% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xe1c7dc65 (Mon Feb 26 17:18:25 2024 UTC)
+moddate:  0x334d3a66 (Tue May  7 15:48:03 2024 UTC)
 files sz: 551
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
@@ -16,15 +16,15 @@
                  6 IMPORT_NAME              0 (classes.TestResult)
                  8 IMPORT_FROM              1 (TestResult)
                 10 STORE_NAME               2 (C_TestResult)
                 12 POP_TOP
    
      4          14 PUSH_NULL
                 16 LOAD_BUILD_CLASS
-                18 LOAD_CONST               2 (<code object ChildSerialNumber, file "D:\Proyectos\ParserResult\cfx_middleware\classes\ChildSerialNumber.py", line 4>)
+                18 LOAD_CONST               2 (<code object ChildSerialNumber, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\classes\ChildSerialNumber.py", line 4>)
                 20 MAKE_FUNCTION            0
                 22 LOAD_CONST               3 ('ChildSerialNumber')
                 24 PRECALL                  2
                 28 CALL                     2
                 38 STORE_NAME               3 (ChildSerialNumber)
                 40 LOAD_CONST               4 (None)
                 42 RETURN_VALUE
@@ -39,19 +39,19 @@
          code 0x970065005a0164005a02640184005a03640284005a0464035300
            4           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ChildSerialNumber')
                        8 STORE_NAME               2 (__qualname__)
          
-           5          10 LOAD_CONST               1 (<code object __init__, file "D:\Proyectos\ParserResult\cfx_middleware\classes\ChildSerialNumber.py", line 5>)
+           5          10 LOAD_CONST               1 (<code object __init__, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\classes\ChildSerialNumber.py", line 5>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (__init__)
          
-          20          16 LOAD_CONST               2 (<code object to_dict, file "D:\Proyectos\ParserResult\cfx_middleware\classes\ChildSerialNumber.py", line 20>)
+          20          16 LOAD_CONST               2 (<code object to_dict, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\classes\ChildSerialNumber.py", line 20>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (to_dict)
                       22 LOAD_CONST               3 (None)
                       24 RETURN_VALUE
          consts
             'ChildSerialNumber'
             code
@@ -85,15 +85,15 @@
                             76 LOAD_FAST                0 (self)
                             78 STORE_ATTR               3 (serial_number)
                
                 16          88 LOAD_FAST                2 (Sequence)
                             90 LOAD_FAST                0 (self)
                             92 STORE_ATTR               4 (sequence)
                
-                17         102 LOAD_CONST               2 (<code object <listcomp>, file "D:\Proyectos\ParserResult\cfx_middleware\classes\ChildSerialNumber.py", line 17>)
+                17         102 LOAD_CONST               2 (<code object <listcomp>, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\classes\ChildSerialNumber.py", line 17>)
                            104 MAKE_FUNCTION            0
                            106 LOAD_FAST                3 (TestResult)
                            108 GET_ITER
                            110 PRECALL                  0
                            114 CALL                     0
                            124 LOAD_FAST                0 (self)
                            126 STORE_ATTR               5 (test_result)
@@ -130,23 +130,23 @@
                              >>   36 RETURN_VALUE
                      consts
                         ()
                      names      ('C_TestResult',)
                      varnames   ('.0', 'tr')
                      freevars   ()
                      cellvars   ()
-                     filename   'D:\\Proyectos\\ParserResult\\cfx_middleware\\classes\\ChildSerialNumber.py'
+                     filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\classes\\ChildSerialNumber.py'
                      name       '<listcomp>'
                      firstlineno 17
                      lnotab 0x
                names      ('isinstance', 'int', 'ValueError', 'serial_number', 'sequence', 'test_result', 'pass_fail')
                varnames   ('self', 'SerialNumber', 'Sequence', 'TestResult', 'PassFail')
                freevars   ()
                cellvars   ()
-               filename   'D:\\Proyectos\\ParserResult\\cfx_middleware\\classes\\ChildSerialNumber.py'
+               filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\classes\\ChildSerialNumber.py'
                name       '__init__'
                firstlineno 5
                lnotab 0x02072a011e020e010e012201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
@@ -163,30 +163,30 @@
                             30 RETURN_VALUE
                consts
                   None
                names      ('vars',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'D:\\Proyectos\\ParserResult\\cfx_middleware\\classes\\ChildSerialNumber.py'
+               filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\classes\\ChildSerialNumber.py'
                name       'to_dict'
                firstlineno 20
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', '__init__', 'to_dict')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'D:\\Proyectos\\ParserResult\\cfx_middleware\\classes\\ChildSerialNumber.py'
+         filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\classes\\ChildSerialNumber.py'
          name       'ChildSerialNumber'
          firstlineno 4
          lnotab 0x0a01060f
       'ChildSerialNumber'
       None
    names      ('classes.TestResult', 'TestResult', 'C_TestResult', 'ChildSerialNumber')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'D:\\Proyectos\\ParserResult\\cfx_middleware\\classes\\ChildSerialNumber.py'
+   filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\classes\\ChildSerialNumber.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c03
```

### Comparing `cfx_middleware-2.1/cfx_middleware/classes/__pycache__/Parameters.cpython-311.pyc` & `cfx_middleware-3.0/cfx_middleware/classes/__pycache__/Parameters.cpython-311.pyc`

 * *Files 15% similar despite different names*

#### Python bytecode

```diff
@@ -1,23 +1,23 @@
 magic:    0xa70d0d0a
-moddate:  0x8d8acf65 (Fri Feb 16 16:17:17 2024 UTC)
+moddate:  0xd9453a66 (Tue May  7 15:16:41 2024 UTC)
 files sz: 211
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x970002004700640084006401a6020000ab0200000000000000005a0064
       025300
      0           0 RESUME                   0
    
      1           2 PUSH_NULL
                  4 LOAD_BUILD_CLASS
-                 6 LOAD_CONST               0 (<code object Parameters, file "D:\Proyectos\ParserResult\classes\Parameters.py", line 1>)
+                 6 LOAD_CONST               0 (<code object Parameters, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\classes\Parameters.py", line 1>)
                  8 MAKE_FUNCTION            0
                 10 LOAD_CONST               1 ('Parameters')
                 12 PRECALL                  2
                 16 CALL                     2
                 26 STORE_NAME               0 (Parameters)
                 28 LOAD_CONST               2 (None)
                 30 RETURN_VALUE
@@ -30,19 +30,19 @@
          code 0x970065005a0164005a02640184005a03640284005a0464035300
            1           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Parameters')
                        8 STORE_NAME               2 (__qualname__)
          
-           2          10 LOAD_CONST               1 (<code object __init__, file "D:\Proyectos\ParserResult\classes\Parameters.py", line 2>)
+           2          10 LOAD_CONST               1 (<code object __init__, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\classes\Parameters.py", line 2>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (__init__)
          
-           6          16 LOAD_CONST               2 (<code object to_dict, file "D:\Proyectos\ParserResult\classes\Parameters.py", line 6>)
+           6          16 LOAD_CONST               2 (<code object to_dict, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\classes\Parameters.py", line 6>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (to_dict)
                       22 LOAD_CONST               3 (None)
                       24 RETURN_VALUE
          consts
             'Parameters'
             code
@@ -66,15 +66,15 @@
                             32 RETURN_VALUE
                consts
                   None
                names      ('recipe_name', 'recipe_revision')
                varnames   ('self', 'RecipeName', 'RecipeRevision')
                freevars   ()
                cellvars   ()
-               filename   'D:\\Proyectos\\ParserResult\\classes\\Parameters.py'
+               filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\classes\\Parameters.py'
                name       '__init__'
                firstlineno 2
                lnotab 0x02010e01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
@@ -91,30 +91,30 @@
                             30 RETURN_VALUE
                consts
                   None
                names      ('vars',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'D:\\Proyectos\\ParserResult\\classes\\Parameters.py'
+               filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\classes\\Parameters.py'
                name       'to_dict'
                firstlineno 6
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', '__init__', 'to_dict')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'D:\\Proyectos\\ParserResult\\classes\\Parameters.py'
+         filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\classes\\Parameters.py'
          name       'Parameters'
          firstlineno 1
          lnotab 0x0a010604
       'Parameters'
       None
    names      ('Parameters',)
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'D:\\Proyectos\\ParserResult\\classes\\Parameters.py'
+   filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\classes\\Parameters.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff0201
```

### Comparing `cfx_middleware-2.1/cfx_middleware/classes/__pycache__/ParserResult.cpython-311.pyc` & `cfx_middleware-3.0/cfx_middleware/classes/__pycache__/ParserResult.cpython-311.pyc`

 * *Files 7% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xe1c7dc65 (Mon Feb 26 17:18:25 2024 UTC)
+moddate:  0x334d3a66 (Tue May  7 15:48:03 2024 UTC)
 files sz: 1671
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
@@ -23,15 +23,15 @@
                 18 IMPORT_NAME              3 (classes.ChildSerialNumber)
                 20 IMPORT_FROM              4 (ChildSerialNumber)
                 22 STORE_NAME               4 (ChildSerialNumber)
                 24 POP_TOP
    
      5          26 PUSH_NULL
                 28 LOAD_BUILD_CLASS
-                30 LOAD_CONST               3 (<code object ParserResult, file "D:\Proyectos\ParserResult\cfx_middleware\classes\ParserResult.py", line 5>)
+                30 LOAD_CONST               3 (<code object ParserResult, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\classes\ParserResult.py", line 5>)
                 32 MAKE_FUNCTION            0
                 34 LOAD_CONST               4 ('ParserResult')
                 36 PRECALL                  2
                 40 CALL                     2
                 50 STORE_NAME               5 (ParserResult)
                 52 LOAD_CONST               5 (None)
                 54 RETURN_VALUE
@@ -47,15 +47,15 @@
          code 0x970065005a0164005a02640184005a0364025300
            5           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ParserResult')
                        8 STORE_NAME               2 (__qualname__)
          
-           6          10 LOAD_CONST               1 (<code object __init__, file "D:\Proyectos\ParserResult\cfx_middleware\classes\ParserResult.py", line 6>)
+           6          10 LOAD_CONST               1 (<code object __init__, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\classes\ParserResult.py", line 6>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (__init__)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'ParserResult'
             code
@@ -194,15 +194,15 @@
                            434 LOAD_FAST                0 (self)
                            436 STORE_ATTR              23 (parameters)
                
                 57         446 LOAD_FAST               21 (TestResults)
                            448 LOAD_FAST                0 (self)
                            450 STORE_ATTR              24 (test_results)
                
-                58         460 LOAD_CONST               3 (<code object <listcomp>, file "D:\Proyectos\ParserResult\cfx_middleware\classes\ParserResult.py", line 58>)
+                58         460 LOAD_CONST               3 (<code object <listcomp>, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\classes\ParserResult.py", line 58>)
                            462 MAKE_FUNCTION            0
                
                 59         464 LOAD_FAST               22 (ChildSerialNumbers)
                
                 58         466 GET_ITER
                            468 PRECALL                  0
                            472 CALL                     0
@@ -240,41 +240,41 @@
                              >>   36 RETURN_VALUE
                      consts
                         ()
                      names      ('ChildSerialNumber',)
                      varnames   ('.0', 'csn')
                      freevars   ()
                      cellvars   ()
-                     filename   'D:\\Proyectos\\ParserResult\\cfx_middleware\\classes\\ParserResult.py'
+                     filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\classes\\ParserResult.py'
                      name       '<listcomp>'
                      firstlineno 58
                      lnotab 0x080118ff
                   ()
                names      ('isinstance', 'bool', 'ValueError', 'method', 'serial_number', 'sequence', 'assembly', 'route_step', 'work_order', 'step', 'line', 'is_panel', 'pass_fail', 'user', 'start_time', 'end_time', 'machine_id', 'ioT_id', 'program_name', 'log_file_name', 'remarks', 'is_birth', 'C_Parameters', 'parameters', 'test_results', 'child_serial_numbers')
                varnames   ('self', 'Method', 'SerialNumber', 'Sequence', 'Assembly', 'RouteStep', 'WorkOrder', 'Step', 'Line', 'IsPanel', 'PassFail', 'User', 'StartTime', 'EndTime', 'MachineId', 'IoTId', 'ProgramName', 'LogFileName', 'Remarks', 'IsBirth', 'Parameters', 'TestResults', 'ChildSerialNumbers')
                freevars   ()
                cellvars   ()
-               filename   'D:\\Proyectos\\ParserResult\\cfx_middleware\\classes\\ParserResult.py'
+               filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\classes\\ParserResult.py'
                name       '__init__'
                firstlineno 6
                lnotab
                   0x02192a011e022a011e020e010e010e010e010e010e010e010e010e010e
                   010e010e010e010e010e010e010e010e010e0122010e01040102ff
             None
          names      ('__name__', '__module__', '__qualname__', '__init__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'D:\\Proyectos\\ParserResult\\cfx_middleware\\classes\\ParserResult.py'
+         filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\classes\\ParserResult.py'
          name       'ParserResult'
          firstlineno 5
          lnotab 0x0a01
       'ParserResult'
       None
    names      ('classes.Parameters', 'Parameters', 'C_Parameters', 'classes.ChildSerialNumber', 'ChildSerialNumber', 'ParserResult')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'D:\\Proyectos\\ParserResult\\cfx_middleware\\classes\\ParserResult.py'
+   filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\classes\\ParserResult.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c010c03
```

### Comparing `cfx_middleware-2.1/cfx_middleware/classes/__pycache__/TestResult.cpython-311.pyc` & `cfx_middleware-3.0/cfx_middleware/classes/__pycache__/TestResult.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,23 +1,23 @@
 magic:    0xa70d0d0a
-moddate:  0x3893cf65 (Fri Feb 16 16:54:16 2024 UTC)
+moddate:  0xd9453a66 (Tue May  7 15:16:41 2024 UTC)
 files sz: 999
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x970002004700640084006401a6020000ab0200000000000000005a0064
       025300
      0           0 RESUME                   0
    
      1           2 PUSH_NULL
                  4 LOAD_BUILD_CLASS
-                 6 LOAD_CONST               0 (<code object TestResult, file "D:\Proyectos\ParserResult\classes\TestResult.py", line 1>)
+                 6 LOAD_CONST               0 (<code object TestResult, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\classes\TestResult.py", line 1>)
                  8 MAKE_FUNCTION            0
                 10 LOAD_CONST               1 ('TestResult')
                 12 PRECALL                  2
                 16 CALL                     2
                 26 STORE_NAME               0 (TestResult)
                 28 LOAD_CONST               2 (None)
                 30 RETURN_VALUE
@@ -30,19 +30,19 @@
          code 0x970065005a0164005a02640184005a03640284005a0464035300
            1           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('TestResult')
                        8 STORE_NAME               2 (__qualname__)
          
-           2          10 LOAD_CONST               1 (<code object __init__, file "D:\Proyectos\ParserResult\classes\TestResult.py", line 2>)
+           2          10 LOAD_CONST               1 (<code object __init__, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\classes\TestResult.py", line 2>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (__init__)
          
-          36          16 LOAD_CONST               2 (<code object to_dict, file "D:\Proyectos\ParserResult\classes\TestResult.py", line 36>)
+          36          16 LOAD_CONST               2 (<code object to_dict, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\classes\TestResult.py", line 36>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (to_dict)
                       22 LOAD_CONST               3 (None)
                       24 RETURN_VALUE
          consts
             'TestResult'
             code
@@ -143,15 +143,15 @@
                   None
                   'IsCritical must be Boolean'
                   'Sequence must be integer'
                names      ('isinstance', 'bool', 'ValueError', 'int', 'test_name', 'sequence', 'pass_fail', 'low_limit', 'high_limit', 'value', 'is_critical', 'defect', 'error_code', 'error_location', 'error_message', 'parameters')
                varnames   ('self', 'TestName', 'Sequence', 'PassFail', 'LowLimit', 'HighLimit', 'Value', 'IsCritical', 'Defect', 'ErrorCode', 'ErrorLocation', 'ErrorMessage', 'Parameters')
                freevars   ()
                cellvars   ()
-               filename   'D:\\Proyectos\\ParserResult\\classes\\TestResult.py'
+               filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\classes\\TestResult.py'
                name       '__init__'
                firstlineno 2
                lnotab
                   0x020f2a011e022a011e020e010e010e010e010e010e010e010e010e010e
                   010e01
             code
                argcount  : 1
@@ -170,30 +170,30 @@
                             30 RETURN_VALUE
                consts
                   None
                names      ('vars',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'D:\\Proyectos\\ParserResult\\classes\\TestResult.py'
+               filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\classes\\TestResult.py'
                name       'to_dict'
                firstlineno 36
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', '__init__', 'to_dict')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'D:\\Proyectos\\ParserResult\\classes\\TestResult.py'
+         filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\classes\\TestResult.py'
          name       'TestResult'
          firstlineno 1
          lnotab 0x0a010622
       'TestResult'
       None
    names      ('TestResult',)
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'D:\\Proyectos\\ParserResult\\classes\\TestResult.py'
+   filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\classes\\TestResult.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff0201
```

### Comparing `cfx_middleware-2.1/cfx_middleware/exceptions/__pycache__/MethodNotValid.cpython-311.pyc` & `cfx_middleware-3.0/cfx_middleware/exceptions/__pycache__/MethodNotValid.cpython-311.pyc`

 * *Files 16% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xe1c7dc65 (Mon Feb 26 17:18:25 2024 UTC)
+moddate:  0x334d3a66 (Tue May  7 15:48:03 2024 UTC)
 files sz: 382
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
@@ -16,23 +16,23 @@
                  6 IMPORT_NAME              0 (enums.MethodsEnum)
                  8 IMPORT_FROM              1 (Methods)
                 10 STORE_NAME               1 (Methods)
                 12 POP_TOP
    
      4          14 PUSH_NULL
                 16 LOAD_BUILD_CLASS
-                18 LOAD_CONST               2 (<code object MethodNotValid, file "D:\Proyectos\ParserResult\cfx_middleware\exceptions\MethodNotValid.py", line 4>)
+                18 LOAD_CONST               2 (<code object MethodNotValid, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\exceptions\MethodNotValid.py", line 4>)
                 20 MAKE_FUNCTION            0
                 22 LOAD_CONST               3 ('MethodNotValid')
                 24 LOAD_NAME                2 (Exception)
                 26 PRECALL                  3
                 30 CALL                     3
                 40 STORE_NAME               3 (MethodNotValid)
    
-     8          42 LOAD_CONST               4 (<code object validate_method, file "D:\Proyectos\ParserResult\cfx_middleware\exceptions\MethodNotValid.py", line 8>)
+     8          42 LOAD_CONST               4 (<code object validate_method, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\exceptions\MethodNotValid.py", line 8>)
                 44 MAKE_FUNCTION            0
                 46 STORE_NAME               4 (validate_method)
                 48 LOAD_CONST               5 (None)
                 50 RETURN_VALUE
    consts
       0
       ('Methods',)
@@ -53,15 +53,15 @@
          consts
             'MethodNotValid'
             None
          names      ('__name__', '__module__', '__qualname__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'D:\\Proyectos\\ParserResult\\cfx_middleware\\exceptions\\MethodNotValid.py'
+         filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\exceptions\\MethodNotValid.py'
          name       'MethodNotValid'
          firstlineno 4
          lnotab 0x0a01
       'MethodNotValid'
       code
          argcount  : 1
          nlocals   : 2
@@ -79,15 +79,15 @@
                        4 LOAD_GLOBAL              0 (Methods)
                       16 LOAD_ATTR                1 (__members__)
                       26 CONTAINS_OP              1
                       28 POP_JUMP_FORWARD_IF_FALSE    57 (to 144)
          
           10          30 LOAD_CONST               1 (', ')
                       32 LOAD_METHOD              2 (join)
-                      54 LOAD_CONST               2 (<code object <genexpr>, file "D:\Proyectos\ParserResult\cfx_middleware\exceptions\MethodNotValid.py", line 10>)
+                      54 LOAD_CONST               2 (<code object <genexpr>, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\exceptions\MethodNotValid.py", line 10>)
                       56 MAKE_FUNCTION            0
                       58 LOAD_GLOBAL              0 (Methods)
                       70 GET_ITER
                       72 PRECALL                  0
                       76 CALL                     0
                       86 PRECALL                  1
                       90 CALL                     1
@@ -136,30 +136,30 @@
                             34 RETURN_VALUE
                consts
                   None
                names      ('value',)
                varnames   ('.0', 'member')
                freevars   ()
                cellvars   ()
-               filename   'D:\\Proyectos\\ParserResult\\cfx_middleware\\exceptions\\MethodNotValid.py'
+               filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\exceptions\\MethodNotValid.py'
                name       '<genexpr>'
                firstlineno 10
                lnotab 0x
             "The method provided '"
             "' doesn't exist, methods available are: "
          names      ('Methods', '__members__', 'join', 'MethodNotValid')
          varnames   ('method', 'methods_valids')
          freevars   ()
          cellvars   ()
-         filename   'D:\\Proyectos\\ParserResult\\cfx_middleware\\exceptions\\MethodNotValid.py'
+         filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\exceptions\\MethodNotValid.py'
          name       'validate_method'
          firstlineno 8
          lnotab 0x02011c0148020c010eff10fd
       None
    names      ('enums.MethodsEnum', 'Methods', 'Exception', 'MethodNotValid', 'validate_method')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'D:\\Proyectos\\ParserResult\\cfx_middleware\\exceptions\\MethodNotValid.py'
+   filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\exceptions\\MethodNotValid.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c031c04
```

### Comparing `cfx_middleware-2.1/cfx_middleware/exceptions/__pycache__/NotDictException.cpython-311.pyc` & `cfx_middleware-3.0/cfx_middleware/exceptions/__pycache__/NotDictException.cpython-311.pyc`

 * *Files 14% similar despite different names*

#### Python bytecode

```diff
@@ -1,31 +1,31 @@
 magic:    0xa70d0d0a
-moddate:  0x4280cf65 (Fri Feb 16 15:33:22 2024 UTC)
+moddate:  0xd9453a66 (Tue May  7 15:16:41 2024 UTC)
 files sz: 229
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700020047006400840064016500a6030000ab0300000000000000005a
       01640284005a0264035300
      0           0 RESUME                   0
    
      1           2 PUSH_NULL
                  4 LOAD_BUILD_CLASS
-                 6 LOAD_CONST               0 (<code object NotDictException, file "D:\Proyectos\ParserResult\exceptions\NotDictException.py", line 1>)
+                 6 LOAD_CONST               0 (<code object NotDictException, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\exceptions\NotDictException.py", line 1>)
                  8 MAKE_FUNCTION            0
                 10 LOAD_CONST               1 ('NotDictException')
                 12 LOAD_NAME                0 (Exception)
                 14 PRECALL                  3
                 18 CALL                     3
                 28 STORE_NAME               1 (NotDictException)
    
-     5          30 LOAD_CONST               2 (<code object is_dict, file "D:\Proyectos\ParserResult\exceptions\NotDictException.py", line 5>)
+     5          30 LOAD_CONST               2 (<code object is_dict, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\exceptions\NotDictException.py", line 5>)
                 32 MAKE_FUNCTION            0
                 34 STORE_NAME               2 (is_dict)
                 36 LOAD_CONST               3 (None)
                 38 RETURN_VALUE
    consts
       code
          argcount  : 0
@@ -44,15 +44,15 @@
          consts
             'NotDictException'
             None
          names      ('__name__', '__module__', '__qualname__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'D:\\Proyectos\\ParserResult\\exceptions\\NotDictException.py'
+         filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\exceptions\\NotDictException.py'
          name       'NotDictException'
          firstlineno 1
          lnotab 0x0a01
       'NotDictException'
       code
          argcount  : 1
          nlocals   : 1
@@ -84,20 +84,20 @@
          consts
             None
             'The data provided is not a dict, please review the data'
          names      ('isinstance', 'dict', 'NotDictException')
          varnames   ('variable',)
          freevars   ()
          cellvars   ()
-         filename   'D:\\Proyectos\\ParserResult\\exceptions\\NotDictException.py'
+         filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\exceptions\\NotDictException.py'
          name       'is_dict'
          firstlineno 5
          lnotab 0x02012a010c0102ff10ff
       None
    names      ('Exception', 'NotDictException', 'is_dict')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'D:\\Proyectos\\ParserResult\\exceptions\\NotDictException.py'
+   filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\exceptions\\NotDictException.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02011c04
```

### Comparing `cfx_middleware-2.1/cfx_middleware/helpers/__pycache__/utils.cpython-311.pyc` & `cfx_middleware-3.0/cfx_middleware/helpers/__pycache__/utils.cpython-311.pyc`

 * *Files 27% similar despite different names*

#### Python bytecode

```diff
@@ -1,19 +1,19 @@
 magic:    0xa70d0d0a
-moddate:  0xe1c7dc65 (Mon Feb 26 17:18:25 2024 UTC)
-files sz: 1415
+moddate:  0x334d3a66 (Tue May  7 15:48:03 2024 UTC)
+files sz: 1726
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064026c026d035a0301
       00640384005a04640484005a05640584005a06640665036602640784045a
-      07640884005a0864015300
+      07640884005a08640984005a0964015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (json)
                  8 STORE_NAME               0 (json)
    
@@ -25,38 +25,42 @@
      4          18 LOAD_CONST               0 (0)
                 20 LOAD_CONST               2 (('ParserResult',))
                 22 IMPORT_NAME              2 (classes.ParserResult)
                 24 IMPORT_FROM              3 (ParserResult)
                 26 STORE_NAME               3 (ParserResult)
                 28 POP_TOP
    
-     7          30 LOAD_CONST               3 (<code object to_camel_case, file "D:\Proyectos\ParserResult\cfx_middleware\helpers\utils.py", line 7>)
+     7          30 LOAD_CONST               3 (<code object to_camel_case, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\helpers\utils.py", line 7>)
                 32 MAKE_FUNCTION            0
                 34 STORE_NAME               4 (to_camel_case)
    
-    12          36 LOAD_CONST               4 (<code object convert_to_camel_case_dict, file "D:\Proyectos\ParserResult\cfx_middleware\helpers\utils.py", line 12>)
+    12          36 LOAD_CONST               4 (<code object convert_to_camel_case_dict, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\helpers\utils.py", line 12>)
                 38 MAKE_FUNCTION            0
                 40 STORE_NAME               5 (convert_to_camel_case_dict)
    
-    26          42 LOAD_CONST               5 (<code object convert_to_dict, file "D:\Proyectos\ParserResult\cfx_middleware\helpers\utils.py", line 26>)
+    26          42 LOAD_CONST               5 (<code object convert_to_dict, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\helpers\utils.py", line 26>)
                 44 MAKE_FUNCTION            0
                 46 STORE_NAME               6 (convert_to_dict)
    
     37          48 LOAD_CONST               6 ('parser_result')
                 50 LOAD_NAME                3 (ParserResult)
                 52 BUILD_TUPLE              2
-                54 LOAD_CONST               7 (<code object class_to_json, file "D:\Proyectos\ParserResult\cfx_middleware\helpers\utils.py", line 37>)
+                54 LOAD_CONST               7 (<code object class_to_json, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\helpers\utils.py", line 37>)
                 56 MAKE_FUNCTION            4 (annotations)
                 58 STORE_NAME               7 (class_to_json)
    
-    44          60 LOAD_CONST               8 (<code object json_to_dict, file "D:\Proyectos\ParserResult\cfx_middleware\helpers\utils.py", line 44>)
+    44          60 LOAD_CONST               8 (<code object json_to_dict, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\helpers\utils.py", line 44>)
                 62 MAKE_FUNCTION            0
                 64 STORE_NAME               8 (json_to_dict)
-                66 LOAD_CONST               1 (None)
-                68 RETURN_VALUE
+   
+    53          66 LOAD_CONST               9 (<code object all_methods, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\helpers\utils.py", line 53>)
+                68 MAKE_FUNCTION            0
+                70 STORE_NAME               9 (all_methods)
+                72 LOAD_CONST               1 (None)
+                74 RETURN_VALUE
    consts
       0
       None
       ('ParserResult',)
       code
          argcount  : 1
          nlocals   : 2
@@ -74,15 +78,15 @@
                       26 LOAD_CONST               1 ('_')
                       28 PRECALL                  1
                       32 CALL                     1
                       42 STORE_FAST               1 (parts)
          
            9          44 LOAD_CONST               2 ('')
                       46 LOAD_METHOD              1 (join)
-                      68 LOAD_CONST               3 (<code object <genexpr>, file "D:\Proyectos\ParserResult\cfx_middleware\helpers\utils.py", line 9>)
+                      68 LOAD_CONST               3 (<code object <genexpr>, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\helpers\utils.py", line 9>)
                       70 MAKE_FUNCTION            0
                       72 LOAD_FAST                1 (parts)
                       74 GET_ITER
                       76 PRECALL                  0
                       80 CALL                     0
                       90 PRECALL                  1
                       94 CALL                     1
@@ -118,23 +122,23 @@
                             60 RETURN_VALUE
                consts
                   None
                names      ('capitalize',)
                varnames   ('.0', 'x')
                freevars   ()
                cellvars   ()
-               filename   'D:\\Proyectos\\ParserResult\\cfx_middleware\\helpers\\utils.py'
+               filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\helpers\\utils.py'
                name       '<genexpr>'
                firstlineno 9
                lnotab 0x
          names      ('split', 'join')
          varnames   ('s', 'parts')
          freevars   ()
          cellvars   ()
-         filename   'D:\\Proyectos\\ParserResult\\cfx_middleware\\helpers\\utils.py'
+         filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\helpers\\utils.py'
          name       'to_camel_case'
          firstlineno 7
          lnotab 0x02012a01
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 6
@@ -188,15 +192,15 @@
           17     >>  162 LOAD_GLOBAL              3 (NULL + isinstance)
                      174 LOAD_FAST                3 (value)
                      176 LOAD_GLOBAL             10 (list)
                      188 PRECALL                  2
                      192 CALL                     2
                      202 POP_JUMP_FORWARD_IF_FALSE    29 (to 262)
          
-          18         204 LOAD_CONST               1 (<code object <listcomp>, file "D:\Proyectos\ParserResult\cfx_middleware\helpers\utils.py", line 18>)
+          18         204 LOAD_CONST               1 (<code object <listcomp>, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\helpers\utils.py", line 18>)
                      206 MAKE_FUNCTION            0
          
           19         208 LOAD_FAST                3 (value)
          
           18         210 GET_ITER
                      212 PRECALL                  0
                      216 CALL                     0
@@ -244,23 +248,23 @@
                             40 JUMP_BACKWARD           18 (to 6)
                        >>   42 RETURN_VALUE
                consts
                names      ('convert_to_camel_case_dict',)
                varnames   ('.0', 'item')
                freevars   ()
                cellvars   ()
-               filename   'D:\\Proyectos\\ParserResult\\cfx_middleware\\helpers\\utils.py'
+               filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\helpers\\utils.py'
                name       '<listcomp>'
                firstlineno 18
                lnotab 0x08011eff
          names      ('items', 'isinstance', 'dict', 'convert_to_camel_case_dict', 'to_camel_case', 'list')
          varnames   ('input_dict', 'output_dict', 'key', 'value')
          freevars   ()
          cellvars   ()
-         filename   'D:\\Proyectos\\ParserResult\\cfx_middleware\\helpers\\utils.py'
+         filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\helpers\\utils.py'
          name       'convert_to_camel_case_dict'
          firstlineno 12
          lnotab 0x0201040132012a0140012a01040102ff34042601
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 4
@@ -281,15 +285,15 @@
           27           2 LOAD_GLOBAL              1 (NULL + isinstance)
                       14 LOAD_FAST                0 (obj)
                       16 LOAD_GLOBAL              2 (dict)
                       28 PRECALL                  2
                       32 CALL                     2
                       42 POP_JUMP_FORWARD_IF_FALSE    30 (to 104)
          
-          28          44 LOAD_CONST               1 (<code object <dictcomp>, file "D:\Proyectos\ParserResult\cfx_middleware\helpers\utils.py", line 28>)
+          28          44 LOAD_CONST               1 (<code object <dictcomp>, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\helpers\utils.py", line 28>)
                       46 MAKE_FUNCTION            0
                       48 LOAD_FAST                0 (obj)
                       50 LOAD_METHOD              2 (items)
                       72 PRECALL                  0
                       76 CALL                     0
                       86 GET_ITER
                       88 PRECALL                  0
@@ -299,15 +303,15 @@
           29     >>  104 LOAD_GLOBAL              1 (NULL + isinstance)
                      116 LOAD_FAST                0 (obj)
                      118 LOAD_GLOBAL              6 (list)
                      130 PRECALL                  2
                      134 CALL                     2
                      144 POP_JUMP_FORWARD_IF_FALSE    12 (to 170)
          
-          30         146 LOAD_CONST               2 (<code object <listcomp>, file "D:\Proyectos\ParserResult\cfx_middleware\helpers\utils.py", line 30>)
+          30         146 LOAD_CONST               2 (<code object <listcomp>, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\helpers\utils.py", line 30>)
                      148 MAKE_FUNCTION            0
                      150 LOAD_FAST                0 (obj)
                      152 GET_ITER
                      154 PRECALL                  0
                      158 CALL                     0
                      168 RETURN_VALUE
          
@@ -355,15 +359,15 @@
                             48 JUMP_BACKWARD           22 (to 6)
                        >>   50 RETURN_VALUE
                consts
                names      ('convert_to_dict',)
                varnames   ('.0', 'k', 'v')
                freevars   ()
                cellvars   ()
-               filename   'D:\\Proyectos\\ParserResult\\cfx_middleware\\helpers\\utils.py'
+               filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\helpers\\utils.py'
                name       '<dictcomp>'
                firstlineno 28
                lnotab 0x
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
@@ -384,24 +388,24 @@
                             40 JUMP_BACKWARD           18 (to 6)
                        >>   42 RETURN_VALUE
                consts
                names      ('convert_to_dict',)
                varnames   ('.0', 'item')
                freevars   ()
                cellvars   ()
-               filename   'D:\\Proyectos\\ParserResult\\cfx_middleware\\helpers\\utils.py'
+               filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\helpers\\utils.py'
                name       '<listcomp>'
                firstlineno 30
                lnotab 0x
             'to_dict'
          names      ('isinstance', 'dict', 'items', 'list', 'hasattr', 'convert_to_dict', 'to_dict')
          varnames   ('obj',)
          freevars   ()
          cellvars   ()
-         filename   'D:\\Proyectos\\ParserResult\\cfx_middleware\\helpers\\utils.py'
+         filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\helpers\\utils.py'
          name       'convert_to_dict'
          firstlineno 26
          lnotab 0x02012a013c012a01180120014202
       'parser_result'
       code
          argcount  : 1
          nlocals   : 3
@@ -433,15 +437,15 @@
                       90 RETURN_VALUE
          consts
             None
          names      ('vars', 'convert_to_camel_case_dict', 'convert_to_dict')
          varnames   ('parser_result', 'attributes', 'data_converted')
          freevars   ()
          cellvars   ()
-         filename   'D:\\Proyectos\\ParserResult\\cfx_middleware\\helpers\\utils.py'
+         filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\helpers\\utils.py'
          name       'class_to_json'
          firstlineno 37
          lnotab 0x02011e013802
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 7
@@ -516,19 +520,77 @@
             None
             'JSON Error:'
             1
          names      ('json', 'loads', 'JSONDecodeError', 'print', 'str', 'sys', 'exit')
          varnames   ('variable', 'json_data', 'jsde')
          freevars   ()
          cellvars   ()
-         filename   'D:\\Proyectos\\ParserResult\\cfx_middleware\\helpers\\utils.py'
+         filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\helpers\\utils.py'
          name       'json_to_dict'
          firstlineno 44
          lnotab 0x02010201280106011c013e013cfe
-   names      ('json', 'sys', 'classes.ParserResult', 'ParserResult', 'to_camel_case', 'convert_to_camel_case_dict', 'convert_to_dict', 'class_to_json', 'json_to_dict')
+      code
+         argcount  : 0
+         nlocals   : 0
+         stacksize : 8
+         flags     : 3
+         code
+            0x9700640164026901640164036901640164046901640164056901640164
+            06690164016407690164016408690167075300
+          53           0 RESUME                   0
+         
+          55           2 LOAD_CONST               1 ('Value')
+                       4 LOAD_CONST               2 ('units_arrived')
+                       6 BUILD_MAP                1
+         
+          56           8 LOAD_CONST               1 ('Value')
+                      10 LOAD_CONST               3 ('recipe_activated')
+                      12 BUILD_MAP                1
+         
+          57          14 LOAD_CONST               1 ('Value')
+                      16 LOAD_CONST               4 ('validate_units')
+                      18 BUILD_MAP                1
+         
+          58          20 LOAD_CONST               1 ('Value')
+                      22 LOAD_CONST               5 ('work_started')
+                      24 BUILD_MAP                1
+         
+          59          26 LOAD_CONST               1 ('Value')
+                      28 LOAD_CONST               6 ('units_inspected')
+                      30 BUILD_MAP                1
+         
+          60          32 LOAD_CONST               1 ('Value')
+                      34 LOAD_CONST               7 ('work_completed')
+                      36 BUILD_MAP                1
+         
+          61          38 LOAD_CONST               1 ('Value')
+                      40 LOAD_CONST               8 ('units_departed')
+                      42 BUILD_MAP                1
+         
+          54          44 BUILD_LIST               7
+                      46 RETURN_VALUE
+         consts
+            None
+            'Value'
+            'units_arrived'
+            'recipe_activated'
+            'validate_units'
+            'work_started'
+            'units_inspected'
+            'work_completed'
+            'units_departed'
+         names      ()
+         varnames   ()
+         freevars   ()
+         cellvars   ()
+         filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\helpers\\utils.py'
+         name       'all_methods'
+         firstlineno 53
+         lnotab 0x020206010601060106010601060106f9
+   names      ('json', 'sys', 'classes.ParserResult', 'ParserResult', 'to_camel_case', 'convert_to_camel_case_dict', 'convert_to_dict', 'class_to_json', 'json_to_dict', 'all_methods')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'D:\\Proyectos\\ParserResult\\cfx_middleware\\helpers\\utils.py'
+   filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\helpers\\utils.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff0201080108020c030605060e060b0c07
+   lnotab 0x00ff0201080108020c030605060e060b0c070609
```

### Comparing `cfx_middleware-2.1/cfx_middleware/helpers/utils.py` & `cfx_middleware-3.0/cfx_middleware/helpers/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,7 +44,19 @@
 def json_to_dict(variable):
     try:
         json_data = json.loads(variable)
         return json_data
     except json.JSONDecodeError as jsde:
         print("JSON Error:" + str(jsde))
         sys.exit(1)
+
+
+def all_methods():
+    return [
+        {"Value": "units_arrived"},
+        {"Value": "recipe_activated"},
+        {"Value": "validate_units"},
+        {"Value": "work_started"},
+        {"Value": "units_inspected"},
+        {"Value": "work_completed"},
+        {"Value": "units_departed"},
+    ]
```

### Comparing `cfx_middleware-2.1/cfx_middleware/rabbit/__pycache__/send_rabbit.cpython-311.pyc` & `cfx_middleware-3.0/cfx_middleware/rabbit/__pycache__/send_rabbit.cpython-311.pyc`

 * *Files 17% similar despite different names*

#### Python bytecode

```diff
@@ -1,281 +1,312 @@
 magic:    0xa70d0d0a
-moddate:  0xde8ccf65 (Fri Feb 16 16:27:10 2024 UTC)
-files sz: 1319
+moddate:  0xd9453a66 (Tue May  7 15:16:41 2024 UTC)
+files sz: 1493
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 3
+   stacksize : 4
    flags     : 0
    code
-      0x970064005a00640164026c015a01640164026c025a02640164036c036d
-      045a04010002006504a6000000ab000000000000000000a0050000000000
-      0000000000000000000000000000006404a6010000ab0100000000000000
-      005a0602006504a6000000ab000000000000000000a00500000000000000
-      000000000000000000000000006405a6010000ab0100000000000000005a
-      0702006504a6000000ab000000000000000000a005000000000000000000
-      00000000000000000000006406a6010000ab0100000000000000005a0802
-      006504a6000000ab000000000000000000a0050000000000000000000000
-      0000000000000000006407a6010000ab0100000000000000005a09020065
-      04a6000000ab000000000000000000a00500000000000000000000000000
-      000000000000006408a6010000ab0100000000000000005a0a640c640a65
-      0b6602640b84055a0c64025300
+      0x970064005a00640164026c015a01640164026c025a02640164026c035a
+      03640164036c046d055a050100020065026a060000000000000000a60000
+      00ab0000000000000000005a0765026a080000000000000000a009000000
+      000000000000000000000000000000000065076404a6020000ab02000000
+      00000000005a0a02006505650aa6010000ab010000000000000000010002
+      0065026a0b00000000000000006405a6010000ab0100000000000000005a
+      0c020065026a0b00000000000000006406a6010000ab0100000000000000
+      005a0d020065026a0b00000000000000006407a6010000ab010000000000
+      0000005a0e020065026a0b00000000000000006408a6010000ab01000000
+      00000000005a0f020065026a0b00000000000000006409a6010000ab0100
+      000000000000005a10020065026a0b0000000000000000640aa6010000ab
+      0100000000000000005a11640e640c65126602640d84055a1364025300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('Generic way to send a RabbitMQ message.')
                  4 STORE_NAME               0 (__doc__)
    
      4           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (None)
                 10 IMPORT_NAME              1 (json)
                 12 STORE_NAME               1 (json)
    
-     7          14 LOAD_CONST               1 (0)
+     5          14 LOAD_CONST               1 (0)
                 16 LOAD_CONST               2 (None)
-                18 IMPORT_NAME              2 (pika)
-                20 STORE_NAME               2 (pika)
+                18 IMPORT_NAME              2 (os)
+                20 STORE_NAME               2 (os)
    
      8          22 LOAD_CONST               1 (0)
-                24 LOAD_CONST               3 (('dotenv_values',))
-                26 IMPORT_NAME              3 (dotenv)
-                28 IMPORT_FROM              4 (dotenv_values)
-                30 STORE_NAME               4 (dotenv_values)
-                32 POP_TOP
-   
-    10          34 PUSH_NULL
-                36 LOAD_NAME                4 (dotenv_values)
-                38 PRECALL                  0
-                42 CALL                     0
-                52 LOAD_METHOD              5 (get)
-                74 LOAD_CONST               4 ('RABBITMQ_HOST')
-                76 PRECALL                  1
-                80 CALL                     1
-                90 STORE_NAME               6 (RABBITMQ_HOST)
-   
-    11          92 PUSH_NULL
-                94 LOAD_NAME                4 (dotenv_values)
-                96 PRECALL                  0
-               100 CALL                     0
-               110 LOAD_METHOD              5 (get)
-               132 LOAD_CONST               5 ('RABBITMQ_PORT')
-               134 PRECALL                  1
-               138 CALL                     1
-               148 STORE_NAME               7 (RABBITMQ_PORT)
-   
-    12         150 PUSH_NULL
-               152 LOAD_NAME                4 (dotenv_values)
-               154 PRECALL                  0
-               158 CALL                     0
-               168 LOAD_METHOD              5 (get)
-               190 LOAD_CONST               6 ('RABBITMQ_VIRTUAL_HOST')
-               192 PRECALL                  1
-               196 CALL                     1
-               206 STORE_NAME               8 (RABBITMQ_VIRTUAL_HOST)
-   
-    13         208 PUSH_NULL
-               210 LOAD_NAME                4 (dotenv_values)
-               212 PRECALL                  0
-               216 CALL                     0
-               226 LOAD_METHOD              5 (get)
-               248 LOAD_CONST               7 ('RABBITMQ_USERNAME')
-               250 PRECALL                  1
-               254 CALL                     1
-               264 STORE_NAME               9 (RABBITMQ_USERNAME)
-   
-    14         266 PUSH_NULL
-               268 LOAD_NAME                4 (dotenv_values)
-               270 PRECALL                  0
-               274 CALL                     0
-               284 LOAD_METHOD              5 (get)
-               306 LOAD_CONST               8 ('RABBITMQ_PASSWORD')
-               308 PRECALL                  1
-               312 CALL                     1
-               322 STORE_NAME              10 (RABBITMQ_PASSWORD)
-   
-    17         324 LOAD_CONST              12 (('',))
-               326 LOAD_CONST              10 ('return')
-               328 LOAD_NAME               11 (bool)
-               330 BUILD_TUPLE              2
-               332 LOAD_CONST              11 (<code object send_message, file "D:\Proyectos\ParserResult\rabbit\send_rabbit.py", line 17>)
-               334 MAKE_FUNCTION            5 (defaults, annotations)
-               336 STORE_NAME              12 (send_message)
-               338 LOAD_CONST               2 (None)
-               340 RETURN_VALUE
+                24 LOAD_CONST               2 (None)
+                26 IMPORT_NAME              3 (pika)
+                28 STORE_NAME               3 (pika)
+   
+     9          30 LOAD_CONST               1 (0)
+                32 LOAD_CONST               3 (('load_dotenv',))
+                34 IMPORT_NAME              4 (dotenv)
+                36 IMPORT_FROM              5 (load_dotenv)
+                38 STORE_NAME               5 (load_dotenv)
+                40 POP_TOP
+   
+    11          42 PUSH_NULL
+                44 LOAD_NAME                2 (os)
+                46 LOAD_ATTR                6 (getcwd)
+                56 PRECALL                  0
+                60 CALL                     0
+                70 STORE_NAME               7 (current_directory)
+   
+    12          72 LOAD_NAME                2 (os)
+                74 LOAD_ATTR                8 (path)
+                84 LOAD_METHOD              9 (join)
+               106 LOAD_NAME                7 (current_directory)
+               108 LOAD_CONST               4 ('.env')
+               110 PRECALL                  2
+               114 CALL                     2
+               124 STORE_NAME              10 (dotenv_path)
+   
+    14         126 PUSH_NULL
+               128 LOAD_NAME                5 (load_dotenv)
+               130 LOAD_NAME               10 (dotenv_path)
+               132 PRECALL                  1
+               136 CALL                     1
+               146 POP_TOP
+   
+    16         148 PUSH_NULL
+               150 LOAD_NAME                2 (os)
+               152 LOAD_ATTR               11 (getenv)
+               162 LOAD_CONST               5 ('RABBITMQ_HOST')
+               164 PRECALL                  1
+               168 CALL                     1
+               178 STORE_NAME              12 (RABBITMQ_HOST)
+   
+    17         180 PUSH_NULL
+               182 LOAD_NAME                2 (os)
+               184 LOAD_ATTR               11 (getenv)
+               194 LOAD_CONST               6 ('RABBITMQ_PORT')
+               196 PRECALL                  1
+               200 CALL                     1
+               210 STORE_NAME              13 (RABBITMQ_PORT)
+   
+    18         212 PUSH_NULL
+               214 LOAD_NAME                2 (os)
+               216 LOAD_ATTR               11 (getenv)
+               226 LOAD_CONST               7 ('RABBITMQ_VIRTUAL_HOST')
+               228 PRECALL                  1
+               232 CALL                     1
+               242 STORE_NAME              14 (RABBITMQ_VIRTUAL_HOST)
+   
+    19         244 PUSH_NULL
+               246 LOAD_NAME                2 (os)
+               248 LOAD_ATTR               11 (getenv)
+               258 LOAD_CONST               8 ('RABBITMQ_USERNAME')
+               260 PRECALL                  1
+               264 CALL                     1
+               274 STORE_NAME              15 (RABBITMQ_USERNAME)
+   
+    20         276 PUSH_NULL
+               278 LOAD_NAME                2 (os)
+               280 LOAD_ATTR               11 (getenv)
+               290 LOAD_CONST               9 ('RABBITMQ_PASSWORD')
+               292 PRECALL                  1
+               296 CALL                     1
+               306 STORE_NAME              16 (RABBITMQ_PASSWORD)
+   
+    22         308 PUSH_NULL
+               310 LOAD_NAME                2 (os)
+               312 LOAD_ATTR               11 (getenv)
+               322 LOAD_CONST              10 ('RABBITMQ_EXCHANGE_PARSER_QUEUE')
+               324 PRECALL                  1
+               328 CALL                     1
+               338 STORE_NAME              17 (RABBITMQ_EXCHANGE_PARSER_QUEUE)
+   
+    24         340 LOAD_CONST              14 (('',))
+               342 LOAD_CONST              12 ('return')
+               344 LOAD_NAME               18 (bool)
+               346 BUILD_TUPLE              2
+               348 LOAD_CONST              13 (<code object send_message, file "D:\Proyectos\PCD.Middleware.CFX.Python\cfx_middleware\rabbit\send_rabbit.py", line 24>)
+               350 MAKE_FUNCTION            5 (defaults, annotations)
+               352 STORE_NAME              19 (send_message)
+               354 LOAD_CONST               2 (None)
+               356 RETURN_VALUE
    consts
       'Generic way to send a RabbitMQ message.'
       0
       None
-      ('dotenv_values',)
+      ('load_dotenv',)
+      '.env'
       'RABBITMQ_HOST'
       'RABBITMQ_PORT'
       'RABBITMQ_VIRTUAL_HOST'
       'RABBITMQ_USERNAME'
       'RABBITMQ_PASSWORD'
+      'RABBITMQ_EXCHANGE_PARSER_QUEUE'
       ''
       'return'
       code
-         argcount  : 3
-         nlocals   : 8
+         argcount  : 2
+         nlocals   : 7
          stacksize : 8
          flags     : 3
          code
             0x97007401000000000000000000006a0100000000000000007404000000
             00000000000000740600000000000000000000a6020000ab020000000000
-            0000007d037401000000000000000000006a040000000000000000740a00
+            0000007d027401000000000000000000006a040000000000000000740a00
             000000000000000000740c00000000000000000000740e00000000000000
-            0000007c0364016402ac03a6060000ab0600000000000000007d04090074
-            01000000000000000000006a0800000000000000007c04a6010000ab0100
-            000000000000007d057c05a0090000000000000000000000000000000000
-            000000a6000000ab0000000000000000007d067c06a00a00000000000000
-            000000000000000000000000007c007c027417000000000000000000006a
-            0c00000000000000007c01a6010000ab010000000000000000ac04a60300
-            00ab03000000000000000001007c05a00d00000000000000000000000000
-            00000000000000a6000000ab000000000000000000010064055300230074
-            1c000000000000000000002400722e7d07741f0000000000000000000064
-            067c079b009d02a6010000ab0100000000000000000100741f0000000000
-            000000000064077c009b009d02a6010000ab010000000000000000010059
-            0064087d077e076e0864087d077e077701770078035900770164095300
-          17           0 RESUME                   0
+            0000007c0264016402ac03a6060000ab0600000000000000007d03090074
+            01000000000000000000006a0800000000000000007c03a6010000ab0100
+            000000000000007d047c04a0090000000000000000000000000000000000
+            000000a6000000ab0000000000000000007d057c05a00a00000000000000
+            000000000000000000000000007416000000000000000000007c01741900
+            0000000000000000006a0d00000000000000007c00a6010000ab01000000
+            0000000000ac04a6030000ab03000000000000000001007c04a00e000000
+            0000000000000000000000000000000000a6000000ab0000000000000000
+            000100640553002300741e00000000000000000000240072337d06742100
+            00000000000000000064067c069b009d02a6010000ab0100000000000000
+            00010074210000000000000000000064077416000000000000000000009b
+            009d02a6010000ab0100000000000000000100590064087d067e066e0864
+            087d067e067701770078035900770164095300
+          24           0 RESUME                   0
          
-          19           2 LOAD_GLOBAL              1 (NULL + pika)
+          26           2 LOAD_GLOBAL              1 (NULL + pika)
                       14 LOAD_ATTR                1 (PlainCredentials)
                       24 LOAD_GLOBAL              4 (RABBITMQ_USERNAME)
                       36 LOAD_GLOBAL              6 (RABBITMQ_PASSWORD)
                       48 PRECALL                  2
                       52 CALL                     2
-                      62 STORE_FAST               3 (credentials)
+                      62 STORE_FAST               2 (credentials)
          
-          21          64 LOAD_GLOBAL              1 (NULL + pika)
+          28          64 LOAD_GLOBAL              1 (NULL + pika)
                       76 LOAD_ATTR                4 (ConnectionParameters)
          
-          22          86 LOAD_GLOBAL             10 (RABBITMQ_HOST)
+          29          86 LOAD_GLOBAL             10 (RABBITMQ_HOST)
          
-          23          98 LOAD_GLOBAL             12 (RABBITMQ_PORT)
+          30          98 LOAD_GLOBAL             12 (RABBITMQ_PORT)
          
-          24         110 LOAD_GLOBAL             14 (RABBITMQ_VIRTUAL_HOST)
+          31         110 LOAD_GLOBAL             14 (RABBITMQ_VIRTUAL_HOST)
          
-          25         122 LOAD_FAST                3 (credentials)
+          32         122 LOAD_FAST                2 (credentials)
          
-          26         124 LOAD_CONST               1 (5)
+          33         124 LOAD_CONST               1 (5)
          
-          27         126 LOAD_CONST               2 (1)
+          34         126 LOAD_CONST               2 (1)
          
-          21         128 KW_NAMES                 3
+          28         128 KW_NAMES                 3
                      130 PRECALL                  6
                      134 CALL                     6
-                     144 STORE_FAST               4 (parameters)
+                     144 STORE_FAST               3 (parameters)
          
-          30         146 NOP
+          37         146 NOP
          
-          31         148 LOAD_GLOBAL              1 (NULL + pika)
+          38         148 LOAD_GLOBAL              1 (NULL + pika)
                      160 LOAD_ATTR                8 (BlockingConnection)
-                     170 LOAD_FAST                4 (parameters)
+                     170 LOAD_FAST                3 (parameters)
                      172 PRECALL                  1
                      176 CALL                     1
-                     186 STORE_FAST               5 (connection)
+                     186 STORE_FAST               4 (connection)
          
-          32         188 LOAD_FAST                5 (connection)
+          39         188 LOAD_FAST                4 (connection)
                      190 LOAD_METHOD              9 (channel)
                      212 PRECALL                  0
                      216 CALL                     0
-                     226 STORE_FAST               6 (channel)
+                     226 STORE_FAST               5 (channel)
          
-          34         228 LOAD_FAST                6 (channel)
+          41         228 LOAD_FAST                5 (channel)
                      230 LOAD_METHOD             10 (basic_publish)
          
-          35         252 LOAD_FAST                0 (exchange_name)
-                     254 LOAD_FAST                2 (routing_key)
-                     256 LOAD_GLOBAL             23 (NULL + json)
-                     268 LOAD_ATTR               12 (dumps)
-                     278 LOAD_FAST                1 (body)
-                     280 PRECALL                  1
-                     284 CALL                     1
-         
-          34         294 KW_NAMES                 4
-                     296 PRECALL                  3
-                     300 CALL                     3
-                     310 POP_TOP
-         
-          38         312 LOAD_FAST                5 (connection)
-                     314 LOAD_METHOD             13 (close)
-                     336 PRECALL                  0
-                     340 CALL                     0
-                     350 POP_TOP
-         
-          40         352 LOAD_CONST               5 (True)
-                     354 RETURN_VALUE
-                 >>  356 PUSH_EXC_INFO
-         
-          41         358 LOAD_GLOBAL             28 (Exception)
-                     370 CHECK_EXC_MATCH
-                     372 POP_JUMP_FORWARD_IF_FALSE    46 (to 466)
-                     374 STORE_FAST               7 (e)
-         
-          42         376 LOAD_GLOBAL             31 (NULL + print)
-                     388 LOAD_CONST               6 ('Error: ')
-                     390 LOAD_FAST                7 (e)
-                     392 FORMAT_VALUE             0
-                     394 BUILD_STRING             2
-                     396 PRECALL                  1
-                     400 CALL                     1
-                     410 POP_TOP
-         
-          43         412 LOAD_GLOBAL             31 (NULL + print)
-                     424 LOAD_CONST               7 ('Error sending message to ')
-                     426 LOAD_FAST                0 (exchange_name)
-                     428 FORMAT_VALUE             0
-                     430 BUILD_STRING             2
-                     432 PRECALL                  1
-                     436 CALL                     1
-                     446 POP_TOP
-                     448 POP_EXCEPT
-                     450 LOAD_CONST               8 (None)
-                     452 STORE_FAST               7 (e)
-                     454 DELETE_FAST              7 (e)
-                     456 JUMP_FORWARD             8 (to 474)
-                 >>  458 LOAD_CONST               8 (None)
-                     460 STORE_FAST               7 (e)
-                     462 DELETE_FAST              7 (e)
-                     464 RERAISE                  1
-         
-          41     >>  466 RERAISE                  0
-                 >>  468 COPY                     3
-                     470 POP_EXCEPT
-                     472 RERAISE                  1
+          42         252 LOAD_GLOBAL             22 (RABBITMQ_EXCHANGE_PARSER_QUEUE)
+                     264 LOAD_FAST                1 (routing_key)
+                     266 LOAD_GLOBAL             25 (NULL + json)
+                     278 LOAD_ATTR               13 (dumps)
+                     288 LOAD_FAST                0 (body)
+                     290 PRECALL                  1
+                     294 CALL                     1
+         
+          41         304 KW_NAMES                 4
+                     306 PRECALL                  3
+                     310 CALL                     3
+                     320 POP_TOP
+         
+          45         322 LOAD_FAST                4 (connection)
+                     324 LOAD_METHOD             14 (close)
+                     346 PRECALL                  0
+                     350 CALL                     0
+                     360 POP_TOP
+         
+          47         362 LOAD_CONST               5 (True)
+                     364 RETURN_VALUE
+                 >>  366 PUSH_EXC_INFO
+         
+          48         368 LOAD_GLOBAL             30 (Exception)
+                     380 CHECK_EXC_MATCH
+                     382 POP_JUMP_FORWARD_IF_FALSE    51 (to 486)
+                     384 STORE_FAST               6 (e)
+         
+          49         386 LOAD_GLOBAL             33 (NULL + print)
+                     398 LOAD_CONST               6 ('Error: ')
+                     400 LOAD_FAST                6 (e)
+                     402 FORMAT_VALUE             0
+                     404 BUILD_STRING             2
+                     406 PRECALL                  1
+                     410 CALL                     1
+                     420 POP_TOP
+         
+          50         422 LOAD_GLOBAL             33 (NULL + print)
+                     434 LOAD_CONST               7 ('Error sending message to ')
+                     436 LOAD_GLOBAL             22 (RABBITMQ_EXCHANGE_PARSER_QUEUE)
+                     448 FORMAT_VALUE             0
+                     450 BUILD_STRING             2
+                     452 PRECALL                  1
+                     456 CALL                     1
+                     466 POP_TOP
+                     468 POP_EXCEPT
+                     470 LOAD_CONST               8 (None)
+                     472 STORE_FAST               6 (e)
+                     474 DELETE_FAST              6 (e)
+                     476 JUMP_FORWARD             8 (to 494)
+                 >>  478 LOAD_CONST               8 (None)
+                     480 STORE_FAST               6 (e)
+                     482 DELETE_FAST              6 (e)
+                     484 RERAISE                  1
+         
+          48     >>  486 RERAISE                  0
+                 >>  488 COPY                     3
+                     490 POP_EXCEPT
+                     492 RERAISE                  1
          
-          45     >>  474 LOAD_CONST               9 (False)
-                     476 RETURN_VALUE
+          52     >>  494 LOAD_CONST               9 (False)
+                     496 RETURN_VALUE
          ExceptionTable:
-           148 to 350 -> 356 [0]
-           356 to 374 -> 468 [1] lasti
-           376 to 446 -> 458 [1] lasti
-           458 to 466 -> 468 [1] lasti
+           148 to 360 -> 366 [0]
+           366 to 384 -> 488 [1] lasti
+           386 to 466 -> 478 [1] lasti
+           478 to 486 -> 488 [1] lasti
          consts
             'Send a message to RabbitMQ.'
             5
             1
             ('host', 'port', 'virtual_host', 'credentials', 'connection_attempts', 'retry_delay')
             ('exchange', 'routing_key', 'body')
             True
             'Error: '
             'Error sending message to '
             None
             False
-         names      ('pika', 'PlainCredentials', 'RABBITMQ_USERNAME', 'RABBITMQ_PASSWORD', 'ConnectionParameters', 'RABBITMQ_HOST', 'RABBITMQ_PORT', 'RABBITMQ_VIRTUAL_HOST', 'BlockingConnection', 'channel', 'basic_publish', 'json', 'dumps', 'close', 'Exception', 'print')
-         varnames   ('exchange_name', 'body', 'routing_key', 'credentials', 'parameters', 'connection', 'channel', 'e')
+         names      ('pika', 'PlainCredentials', 'RABBITMQ_USERNAME', 'RABBITMQ_PASSWORD', 'ConnectionParameters', 'RABBITMQ_HOST', 'RABBITMQ_PORT', 'RABBITMQ_VIRTUAL_HOST', 'BlockingConnection', 'channel', 'basic_publish', 'RABBITMQ_EXCHANGE_PARSER_QUEUE', 'json', 'dumps', 'close', 'Exception', 'print')
+         varnames   ('body', 'routing_key', 'credentials', 'parameters', 'connection', 'channel', 'e')
          freevars   ()
          cellvars   ()
-         filename   'D:\\Proyectos\\ParserResult\\rabbit\\send_rabbit.py'
+         filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\rabbit\\send_rabbit.py'
          name       'send_message'
-         firstlineno 17
+         firstlineno 24
          lnotab
-            0x02023e0216010c010c010c010201020102fa120902012801280218012a
-            ff1204280206011201240136fe0804
+            0x02023e0216010c010c010c010201020102fa1209020128012802180134
+            ff1204280206011201240140fe0804
       ('',)
-   names      ('__doc__', 'json', 'pika', 'dotenv', 'dotenv_values', 'get', 'RABBITMQ_HOST', 'RABBITMQ_PORT', 'RABBITMQ_VIRTUAL_HOST', 'RABBITMQ_USERNAME', 'RABBITMQ_PASSWORD', 'bool', 'send_message')
+   names      ('__doc__', 'json', 'os', 'pika', 'dotenv', 'load_dotenv', 'getcwd', 'current_directory', 'path', 'join', 'dotenv_path', 'getenv', 'RABBITMQ_HOST', 'RABBITMQ_PORT', 'RABBITMQ_VIRTUAL_HOST', 'RABBITMQ_USERNAME', 'RABBITMQ_PASSWORD', 'RABBITMQ_EXCHANGE_PARSER_QUEUE', 'bool', 'send_message')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'D:\\Proyectos\\ParserResult\\rabbit\\send_rabbit.py'
+   filename   'D:\\Proyectos\\PCD.Middleware.CFX.Python\\cfx_middleware\\rabbit\\send_rabbit.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010403080308010c023a013a013a013a013a03
+   lnotab
+      0x00ff020104030801080308010c021e0136021602200120012001200120
+      022002
```

### Comparing `cfx_middleware-2.1/cfx_middleware/rabbit/send_rabbit.py` & `cfx_middleware-3.0/cfx_middleware/rabbit/send_rabbit.py`

 * *Files identical despite different names*

### Comparing `cfx_middleware-2.1/cfx_middleware.egg-info/PKG-INFO` & `cfx_middleware-3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cfx-middleware
-Version: 2.1
+Name: cfx_middleware
+Version: 3.0
 Summary: Provide a Middleware between the system and CFX
 Home-page: https://dev.azure.com/USI-Applications/USI%20Global%20Development/_git/PCD.Middleware.CFX.Python
 Author: Victor Dominguez
 Author-email: e-victor_dominguez@usiglobal.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cfx_middleware-2.1/cfx_middleware.egg-info/SOURCES.txt` & `cfx_middleware-3.0/cfx_middleware.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 cfx_middleware/__init__.py
 cfx_middleware/cfx_middleware.py
 cfx_middleware.egg-info/PKG-INFO
 cfx_middleware.egg-info/SOURCES.txt
 cfx_middleware.egg-info/dependency_links.txt
 cfx_middleware.egg-info/requires.txt
 cfx_middleware.egg-info/top_level.txt
-cfx_middleware/__pycache__/__init__.cpython-311.pyc
 cfx_middleware/__pycache__/cfx_middleware.cpython-311.pyc
-cfx_middleware/__pycache__/parser_result.cpython-311.pyc
 cfx_middleware/classes/ChildSerialNumber.py
 cfx_middleware/classes/Parameters.py
 cfx_middleware/classes/ParserResult.py
 cfx_middleware/classes/TestResult.py
 cfx_middleware/classes/__pycache__/ChildSerialNumber.cpython-311.pyc
 cfx_middleware/classes/__pycache__/Parameters.cpython-311.pyc
 cfx_middleware/classes/__pycache__/ParserResult.cpython-311.pyc
```

### Comparing `cfx_middleware-2.1/setup.py` & `cfx_middleware-3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 cfx_middleware_files = [
     str(path.relative_to("cfx_middleware"))
     for path in Path("cfx_middleware").rglob("*")
 ]
 
 setup(
     name="cfx_middleware",
-    version="2.1",
+    version="3.0",
     packages=find_packages(),
     package_data={"": cfx_middleware_files},
     install_requires=["python-dotenv"],
     python_requires=">=3",
     author="Victor Dominguez",
     author_email="e-victor_dominguez@usiglobal.com",
     description="Provide a Middleware between the system and CFX",
```

