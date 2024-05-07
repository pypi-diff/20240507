# Comparing `tmp/clvm-0.9.8-py3-none-any.whl.zip` & `tmp/clvm-0.9.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 19889 bytes, number of entries: 19
--rw-r--r--  2.0 unx      855 b- defN 23-Aug-17 13:21 clvm/CLVMObject.py
--rw-r--r--  2.0 unx      132 b- defN 23-Aug-17 13:21 clvm/EvalError.py
--rw-r--r--  2.0 unx     6968 b- defN 23-Aug-17 13:21 clvm/SExp.py
--rw-r--r--  2.0 unx      233 b- defN 23-Aug-17 13:21 clvm/__init__.py
--rw-r--r--  2.0 unx     1089 b- defN 23-Aug-17 13:21 clvm/as_python.py
--rw-r--r--  2.0 unx      627 b- defN 23-Aug-17 13:21 clvm/casts.py
--rw-r--r--  2.0 unx     1738 b- defN 23-Aug-17 13:21 clvm/core_ops.py
--rw-r--r--  2.0 unx     1200 b- defN 23-Aug-17 13:21 clvm/costs.py
--rw-r--r--  2.0 unx    10730 b- defN 23-Aug-17 13:21 clvm/more_ops.py
--rw-r--r--  2.0 unx      427 b- defN 23-Aug-17 13:21 clvm/op_utils.py
--rw-r--r--  2.0 unx     6186 b- defN 23-Aug-17 13:21 clvm/operators.py
--rw-r--r--  2.0 unx     5725 b- defN 23-Aug-17 13:21 clvm/run_program.py
--rw-r--r--  2.0 unx     5193 b- defN 23-Aug-17 13:21 clvm/serialize.py
--rw-r--r--  2.0 unx      212 b- defN 23-Aug-17 13:21 clvm/version.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Aug-17 13:21 clvm-0.9.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     1296 b- defN 23-Aug-17 13:21 clvm-0.9.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-17 13:21 clvm-0.9.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Aug-17 13:21 clvm-0.9.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1386 b- defN 23-Aug-17 13:21 clvm-0.9.8.dist-info/RECORD
-19 files, 55451 bytes uncompressed, 17691 bytes compressed:  68.1%
+Zip file size: 19941 bytes, number of entries: 19
+-rw-r--r--  2.0 unx      855 b- defN 24-Mar-05 20:33 clvm/CLVMObject.py
+-rw-r--r--  2.0 unx      132 b- defN 24-Mar-05 20:33 clvm/EvalError.py
+-rw-r--r--  2.0 unx     6968 b- defN 24-Mar-05 20:33 clvm/SExp.py
+-rw-r--r--  2.0 unx      233 b- defN 24-Mar-05 20:33 clvm/__init__.py
+-rw-r--r--  2.0 unx     1089 b- defN 24-Mar-05 20:33 clvm/as_python.py
+-rw-r--r--  2.0 unx      627 b- defN 24-Mar-05 20:33 clvm/casts.py
+-rw-r--r--  2.0 unx     1738 b- defN 24-Mar-05 20:33 clvm/core_ops.py
+-rw-r--r--  2.0 unx     1200 b- defN 24-Mar-05 20:33 clvm/costs.py
+-rw-r--r--  2.0 unx    10732 b- defN 24-Mar-05 20:33 clvm/more_ops.py
+-rw-r--r--  2.0 unx      550 b- defN 24-Mar-05 20:33 clvm/op_utils.py
+-rw-r--r--  2.0 unx     6186 b- defN 24-Mar-05 20:33 clvm/operators.py
+-rw-r--r--  2.0 unx     5725 b- defN 24-Mar-05 20:33 clvm/run_program.py
+-rw-r--r--  2.0 unx     5183 b- defN 24-Mar-05 20:33 clvm/serialize.py
+-rw-r--r--  2.0 unx      194 b- defN 24-Mar-05 20:33 clvm/version.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-Mar-05 20:33 clvm-0.9.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1518 b- defN 24-Mar-05 20:33 clvm-0.9.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-05 20:33 clvm-0.9.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Mar-05 20:33 clvm-0.9.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1386 b- defN 24-Mar-05 20:33 clvm-0.9.9.dist-info/RECORD
+19 files, 55770 bytes uncompressed, 17743 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: clvm/serialize.py
 Comment: 
 
 Filename: clvm/version.py
 Comment: 
 
-Filename: clvm-0.9.8.dist-info/LICENSE
+Filename: clvm-0.9.9.dist-info/LICENSE
 Comment: 
 
-Filename: clvm-0.9.8.dist-info/METADATA
+Filename: clvm-0.9.9.dist-info/METADATA
 Comment: 
 
-Filename: clvm-0.9.8.dist-info/WHEEL
+Filename: clvm-0.9.9.dist-info/WHEEL
 Comment: 
 
-Filename: clvm-0.9.8.dist-info/top_level.txt
+Filename: clvm-0.9.9.dist-info/top_level.txt
 Comment: 
 
-Filename: clvm-0.9.8.dist-info/RECORD
+Filename: clvm-0.9.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## clvm/more_ops.py

```diff
@@ -1,11 +1,11 @@
 import hashlib
 import io
 
-from blspy import G1Element, PrivateKey
+from chia_rs import G1Element, PrivateKey
 
 from .EvalError import EvalError
 from .casts import limbs_for_int
 from .SExp import SExp
 
 from .costs import (
     ARITH_BASE_COST,
```

## clvm/op_utils.py

```diff
@@ -1,12 +1,17 @@
-def operators_for_dict(keyword_to_atom, op_dict, op_name_lookup={}):
+def operators_for_dict(keyword_to_atom, op_dict, op_name_lookup=None):
+    if op_name_lookup is None:
+        op_name_lookup = {}
+
     d = {}
     for op in keyword_to_atom.keys():
         op_name = "op_%s" % op_name_lookup.get(op, op)
         op_f = op_dict.get(op_name)
         if op_f:
             d[keyword_to_atom[op]] = op_f
     return d
 
 
-def operators_for_module(keyword_to_atom, mod, op_name_lookup={}):
+def operators_for_module(keyword_to_atom, mod, op_name_lookup=None):
+    if op_name_lookup is None:
+        op_name_lookup = {}
     return operators_for_dict(keyword_to_atom, mod.__dict__, op_name_lookup)
```

## clvm/serialize.py

```diff
@@ -20,21 +20,21 @@
 CONS_BOX_MARKER = 0xFF
 
 
 def sexp_to_byte_iterator(sexp):
     todo_stack = [sexp]
     while todo_stack:
         sexp = todo_stack.pop()
-        pair = sexp.as_pair()
+        pair = sexp.pair
         if pair:
             yield bytes([CONS_BOX_MARKER])
             todo_stack.append(pair[1])
             todo_stack.append(pair[0])
         else:
-            yield from atom_to_byte_iterator(sexp.as_atom())
+            yield from atom_to_byte_iterator(sexp.atom)
 
 
 def atom_to_byte_iterator(as_atom):
     size = len(as_atom)
     if size == 0:
         yield b"\x80"
         return
```

## clvm/version.py

```diff
@@ -1,7 +1,7 @@
-from pkg_resources import get_distribution, DistributionNotFound
+import importlib_metadata
 
 try:
-    __version__ = get_distribution(__name__).version
-except DistributionNotFound:
+    __version__ = importlib_metadata.version(__name__)
+except importlib_metadata.PackageNotFoundError:
     # package is not installed
     __version__ = "unknown"
```

## Comparing `clvm-0.9.8.dist-info/LICENSE` & `clvm-0.9.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `clvm-0.9.8.dist-info/METADATA` & `clvm-0.9.9.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: clvm
-Version: 0.9.8
+Version: 0.9.9
 Summary: [Contract Language | Chialisp] Virtual Machine
 Home-page: https://github.com/Chia-Network/clvm
 Author: Chia Network, Inc.
 Author-email: hello@chia.net
 License: https://opensource.org/licenses/Apache-2.0
 Project-URL: Bug Reports, https://github.com/Chia-Network/clvm
 Project-URL: Source, https://github.com/Chia-Network/clvm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Security :: Cryptography
+Requires-Python: >=3.8.1, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: blspy >=0.9
+Requires-Dist: chia-rs >=0.2.13
+Requires-Dist: importlib-metadata ~=6.11.0
 Provides-Extra: dev
 Requires-Dist: clvm-tools >=0.4.4 ; extra == 'dev'
 Requires-Dist: pytest ; extra == 'dev'
+Requires-Dist: setuptools ; extra == 'dev'
 
 [![Coverage Status](https://coveralls.io/repos/github/Chia-Network/clvm/badge.svg?branch=main)](https://coveralls.io/github/Chia-Network/clvm?branch=main)
 
 This is the in-development version of a LISP-like language for encumbering and releasing funds with smart-contract capabilities.
 
 See docs/clvm.org or https://chialisp.com/ for more info.
```

## Comparing `clvm-0.9.8.dist-info/RECORD` & `clvm-0.9.9.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 clvm/EvalError.py,sha256=3wtxrEO1A-H7djONqvcSV6LNz20P0SboZp6laPIsJjk,132
 clvm/SExp.py,sha256=drF0yvhMBZpTOQhGsqs53UXGVLMeWhvmpO6UkYj1uxk,6968
 clvm/__init__.py,sha256=F_MQiGGnobQfAzmlVHKlj5iE9tATixBthNE9eZ0unow,233
 clvm/as_python.py,sha256=IbXuXXDhsSf3FwLQg60fX4lHahZSMqGMRaN_pSu8kyg,1089
 clvm/casts.py,sha256=nv3Bh24oT8cy6Ew18lHu7ey1tMCHGJNZojRlH9Qeais,627
 clvm/core_ops.py,sha256=WUCBl0Oq_kjo7f2AYOL4hACyMDTjNBtE9bFW8oI-2iA,1738
 clvm/costs.py,sha256=osdTrSCxNg2c7lTtJYm6YUAUp3vltNStyBpzbR8wmPY,1200
-clvm/more_ops.py,sha256=I1rjh_YgTsqOq5iHPmrUf2pRx1y4k_yXJS1HaKnhzUs,10730
-clvm/op_utils.py,sha256=CRXf8epX6bqp2Qaoq6woo1I8Iv_Qk76Br8VZJxS67wg,427
+clvm/more_ops.py,sha256=Yj32HkmZLANvVw0syvgzD2bsmJl25EpplnhpjWG8VD8,10732
+clvm/op_utils.py,sha256=jbeexlEo1h1cTIuRyU1sCQ_X9akPPx_ZYrv0uS1dFlw,550
 clvm/operators.py,sha256=QQJG7LyB0N4obm3kbKA46BUF-7s3xxSG6vY8dkjmddY,6186
 clvm/run_program.py,sha256=Gc2MH7kdlUGt3_QT1JMDjUbe2RhOx23Y3oYIdPOoZz8,5725
-clvm/serialize.py,sha256=UOZiexIpWD6Wqm6GHDKHMijB5ljnGT52eeSHiWint-s,5193
-clvm/version.py,sha256=phF8Rm7BiuLJWF4-L_sBP5KFtFtgG-s1OAuQJ4O4DGU,212
-clvm-0.9.8.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-clvm-0.9.8.dist-info/METADATA,sha256=l585bhkN9dJP4V4SPL326ddXYG6I36oNQrK5ENm0luE,1296
-clvm-0.9.8.dist-info/WHEEL,sha256=5sUXSg9e4bi7lTLOHcm6QEYwO5TIF1TNbTSVFVjcJcc,92
-clvm-0.9.8.dist-info/top_level.txt,sha256=Cel1c5Yf8on0xQ02qSS-UsSxHiyqQmlxGM4on6Tw7tg,5
-clvm-0.9.8.dist-info/RECORD,,
+clvm/serialize.py,sha256=ukif6NZubwe2BwhwOROCEJltpXc-sGqyPFCW1RwEXkE,5183
+clvm/version.py,sha256=LiRFdralfvZz5N27iK7L-LgcVu2T9fc1u1GC_HZHbQs,194
+clvm-0.9.9.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+clvm-0.9.9.dist-info/METADATA,sha256=Jvrc3inVpcAga_rTAZAfSXWaASb6YbjXr8WaJaJtTuM,1518
+clvm-0.9.9.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+clvm-0.9.9.dist-info/top_level.txt,sha256=Cel1c5Yf8on0xQ02qSS-UsSxHiyqQmlxGM4on6Tw7tg,5
+clvm-0.9.9.dist-info/RECORD,,
```

