# Comparing `tmp/genai_apis-0.0.3-py3-none-any.whl.zip` & `tmp/genai_apis-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 8524 bytes, number of entries: 11
--rw-r--r--  2.0 unx       95 b- defN 24-May-03 06:58 genai_apis/__init__.py
--rw-r--r--  2.0 unx      265 b- defN 24-May-03 04:28 genai_apis/abstract.py
--rw-r--r--  2.0 unx      819 b- defN 24-May-03 06:58 genai_apis/anthropic_api.py
+Zip file size: 8809 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       91 b- defN 24-May-07 06:15 genai_apis/__init__.py
+-rw-r--r--  2.0 unx      265 b- defN 24-May-07 01:51 genai_apis/abstract.py
+-rw-r--r--  2.0 unx      819 b- defN 24-May-07 01:51 genai_apis/anthropic_api.py
 -rw-r--r--  2.0 unx     2905 b- defN 24-May-03 05:23 genai_apis/factory.py
--rw-r--r--  2.0 unx     1443 b- defN 24-May-03 06:58 genai_apis/gemini_api.py
--rw-r--r--  2.0 unx      790 b- defN 24-May-03 06:58 genai_apis/openai_api.py
--rw-r--r--  2.0 unx    11357 b- defN 24-May-03 06:58 genai_apis-0.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     1025 b- defN 24-May-03 06:58 genai_apis-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-03 06:58 genai_apis-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-May-03 06:58 genai_apis-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      879 b- defN 24-May-03 06:58 genai_apis-0.0.3.dist-info/RECORD
-11 files, 19681 bytes uncompressed, 7038 bytes compressed:  64.2%
+-rw-r--r--  2.0 unx     1443 b- defN 24-May-07 01:51 genai_apis/gemini_api.py
+-rw-r--r--  2.0 unx      790 b- defN 24-May-07 01:51 genai_apis/openai_api.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-07 06:16 genai_apis-0.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1672 b- defN 24-May-07 06:16 genai_apis-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-07 06:16 genai_apis-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-May-07 06:16 genai_apis-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      879 b- defN 24-May-07 06:16 genai_apis-0.0.4.dist-info/RECORD
+11 files, 20324 bytes uncompressed, 7323 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: genai_apis/gemini_api.py
 Comment: 
 
 Filename: genai_apis/openai_api.py
 Comment: 
 
-Filename: genai_apis-0.0.3.dist-info/LICENSE
+Filename: genai_apis-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: genai_apis-0.0.3.dist-info/METADATA
+Filename: genai_apis-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: genai_apis-0.0.3.dist-info/WHEEL
+Filename: genai_apis-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: genai_apis-0.0.3.dist-info/top_level.txt
+Filename: genai_apis-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: genai_apis-0.0.3.dist-info/RECORD
+Filename: genai_apis-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## genai_apis/__init__.py

```diff
@@ -1,5 +1,5 @@
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
-from src.genai_apis.factory import APIFactory
+from genai_apis.factory import APIFactory
 
 __all__ = ["APIFactory"]
```

## Comparing `genai_apis-0.0.3.dist-info/LICENSE` & `genai_apis-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `genai_apis-0.0.3.dist-info/RECORD` & `genai_apis-0.0.4.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-genai_apis/__init__.py,sha256=4qFOKDWg-gIpqtZM4cOBBc1vi3_q1hT-W85JtyEXir0,95
+genai_apis/__init__.py,sha256=WHWHNhabMpLEezO8tiU-kz0fYoI8nXaC6Q9NJ9UM8DE,91
 genai_apis/abstract.py,sha256=a54RxTFFfSWuoO2r8-rIjRpcXcD3LBmEchwPZNCzP7U,265
 genai_apis/anthropic_api.py,sha256=nprzpxgta3ubIY6eQuvaXEz8eA-9WoNxcZUFG17jGlQ,819
 genai_apis/factory.py,sha256=sJgX-cUGVb5c-i7bYjofYAVbEVXqWVnFflURO5C9PIA,2905
 genai_apis/gemini_api.py,sha256=rz26uR1CqKs3DxNucGPIuZ73_ilFKlJ0MtvtQAW1ok4,1443
 genai_apis/openai_api.py,sha256=Uu_i7Mo8KObH7PxkVDxSz5C9tKLhOuW5yMm1ShLTMVM,790
-genai_apis-0.0.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-genai_apis-0.0.3.dist-info/METADATA,sha256=ZJKwrDDIdydV0RTyVgUskHM2xKh8yZ2-YWLU6DKZSBw,1025
-genai_apis-0.0.3.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-genai_apis-0.0.3.dist-info/top_level.txt,sha256=lxy-j5IOQHvkO1zMVLruWLnxQapKtnD_0P9_F_z8cKc,11
-genai_apis-0.0.3.dist-info/RECORD,,
+genai_apis-0.0.4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+genai_apis-0.0.4.dist-info/METADATA,sha256=ByFZkruPZJcxO-tHybfLFqHzc7PdXSNvBH9gZhrVUkM,1672
+genai_apis-0.0.4.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+genai_apis-0.0.4.dist-info/top_level.txt,sha256=lxy-j5IOQHvkO1zMVLruWLnxQapKtnD_0P9_F_z8cKc,11
+genai_apis-0.0.4.dist-info/RECORD,,
```

