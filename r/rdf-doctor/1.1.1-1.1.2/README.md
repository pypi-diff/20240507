# Comparing `tmp/rdf_doctor-1.1.1-py3-none-any.whl.zip` & `tmp/rdf_doctor-1.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 59877 bytes, number of entries: 12
--rw-r--r--  2.0 unx       22 b- defN 24-Apr-25 04:53 doctor/__init__.py
--rw-r--r--  2.0 unx     1754 b- defN 24-Apr-24 04:07 doctor/consts.py
--rw-r--r--  2.0 unx    81134 b- defN 24-Apr-25 04:53 doctor/doctor.py
--rw-r--r--  2.0 unx   134314 b- defN 24-Apr-24 04:07 doctor/reference/prefixes.tsv
--rw-r--r--  2.0 unx       90 b- defN 24-Mar-06 07:08 doctor/reference/refine-class-uris.tsv
--rw-r--r--  2.0 unx      577 b- defN 24-Mar-06 07:13 doctor/reference/refine-prefix-uris.tsv
--rw-r--r--  2.0 unx     1061 b- defN 24-Apr-25 04:56 rdf_doctor-1.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    10665 b- defN 24-Apr-25 04:56 rdf_doctor-1.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-25 04:56 rdf_doctor-1.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 24-Apr-25 04:56 rdf_doctor-1.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-25 04:56 rdf_doctor-1.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      995 b- defN 24-Apr-25 04:56 rdf_doctor-1.1.1.dist-info/RECORD
-12 files, 230763 bytes uncompressed, 58197 bytes compressed:  74.8%
+Zip file size: 59873 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       22 b- defN 24-May-07 07:07 doctor/__init__.py
+-rw-r--r--  2.0 unx     1754 b- defN 24-May-07 05:38 doctor/consts.py
+-rw-r--r--  2.0 unx    81134 b- defN 24-May-07 05:38 doctor/doctor.py
+-rw-r--r--  2.0 unx   134314 b- defN 24-May-07 05:38 doctor/reference/prefixes.tsv
+-rw-r--r--  2.0 unx       90 b- defN 24-May-07 05:38 doctor/reference/refine-class-uris.tsv
+-rw-r--r--  2.0 unx      577 b- defN 24-May-07 05:38 doctor/reference/refine-prefix-uris.tsv
+-rw-r--r--  2.0 unx     1061 b- defN 24-May-07 07:16 rdf_doctor-1.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10651 b- defN 24-May-07 07:16 rdf_doctor-1.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-07 07:16 rdf_doctor-1.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 24-May-07 07:16 rdf_doctor-1.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 24-May-07 07:16 rdf_doctor-1.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      995 b- defN 24-May-07 07:16 rdf_doctor-1.1.2.dist-info/RECORD
+12 files, 230749 bytes uncompressed, 58193 bytes compressed:  74.8%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: doctor/reference/refine-class-uris.tsv
 Comment: 
 
 Filename: doctor/reference/refine-prefix-uris.tsv
 Comment: 
 
-Filename: rdf_doctor-1.1.1.dist-info/LICENSE
+Filename: rdf_doctor-1.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: rdf_doctor-1.1.1.dist-info/METADATA
+Filename: rdf_doctor-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: rdf_doctor-1.1.1.dist-info/WHEEL
+Filename: rdf_doctor-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: rdf_doctor-1.1.1.dist-info/entry_points.txt
+Filename: rdf_doctor-1.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: rdf_doctor-1.1.1.dist-info/top_level.txt
+Filename: rdf_doctor-1.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: rdf_doctor-1.1.1.dist-info/RECORD
+Filename: rdf_doctor-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## doctor/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.1.1"
+__version__ = "1.1.2"
```

## Comparing `rdf_doctor-1.1.1.dist-info/LICENSE` & `rdf_doctor-1.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rdf_doctor-1.1.1.dist-info/METADATA` & `rdf_doctor-1.1.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: rdf-doctor
-Version: 1.1.1
+Version: 1.1.2
 Summary: Validate RDF data, report problems, and support creation of more accurate data
 Home-page: https://github.com/dbcls/rdf-doctor
 Author: DBCLS
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Flask (>=2.2.5)
-Requires-Dist: Flask-Cors (>=3.0.9)
-Requires-Dist: rdflib (>=6.3.1)
-Requires-Dist: SPARQLWrapper (>=2.0.0)
-Requires-Dist: wlighter (>=1.0.1)
-Requires-Dist: shexer (==2.3.0)
-Requires-Dist: unidecode (>=1.3.6)
+Requires-Dist: Flask >=2.2.5
+Requires-Dist: Flask-Cors >=3.0.9
+Requires-Dist: rdflib >=6.3.1
+Requires-Dist: SPARQLWrapper >=2.0.0
+Requires-Dist: wlighter >=1.0.1
+Requires-Dist: shexer >=2.4.1
+Requires-Dist: unidecode >=1.3.6
 
 # rdf-doctor
 [![Pyversions](https://img.shields.io/pypi/pyversions/rdf-doctor.svg)](https://pypi.python.org/pypi/rdf-doctor)
 
 ## Motivation
 DBCLS has conducted to convert various life science databases to RDF and support it. This development will enable us to provide a high-quality dataset that better links existing RDF datasets stored in the RDF portal site and newly developed RDF.
```

## Comparing `rdf_doctor-1.1.1.dist-info/RECORD` & `rdf_doctor-1.1.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-doctor/__init__.py,sha256=q8_5C0f-8mHWNb6mMw02zlYPnEGXBqvOmP3z0CEwZKM,22
+doctor/__init__.py,sha256=5SgGjThsHu_ITn8V83BvCziqCwxdXxTQqcC3KQMHPfM,22
 doctor/consts.py,sha256=U8KOzdPFgMuf_nMul1Vw9qtAvKtZbu8WLwkiYD49IAs,1754
 doctor/doctor.py,sha256=Z8YHopV7U7kpliAh54FxESObTfSHBpczC-iXFHRwfsQ,81134
 doctor/reference/prefixes.tsv,sha256=_1hW0wBl6K1YvcM8stdiEdD4elzST_ecJqQEvhD9Auk,134314
 doctor/reference/refine-class-uris.tsv,sha256=pd_nOSjR7bia96u9hhcjhBg9J6LUAuDFlyy-JE9tsys,90
 doctor/reference/refine-prefix-uris.tsv,sha256=KY5PZ4WCaLeB0APNBjAWq7_Q5Whc6FLg9ncX7BSPeuw,577
-rdf_doctor-1.1.1.dist-info/LICENSE,sha256=e5qMQtuffizvdi23h6MoQ37f3xmNY0VBq8V0tgWuZNg,1061
-rdf_doctor-1.1.1.dist-info/METADATA,sha256=UTZcKIEJwUKRI44c-x56CoImZyzkJgHL9az2AJOSHsU,10665
-rdf_doctor-1.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rdf_doctor-1.1.1.dist-info/entry_points.txt,sha256=1vHyYdY5pMK7zOINHh2ymwU_Uid1YzZx7Vte5tjHCls,52
-rdf_doctor-1.1.1.dist-info/top_level.txt,sha256=8awHkjBkPxJ8N_ygAwmuUTUz5ZKfy9aqNcWTSI_Ma_8,7
-rdf_doctor-1.1.1.dist-info/RECORD,,
+rdf_doctor-1.1.2.dist-info/LICENSE,sha256=e5qMQtuffizvdi23h6MoQ37f3xmNY0VBq8V0tgWuZNg,1061
+rdf_doctor-1.1.2.dist-info/METADATA,sha256=QGhHrL6ZWSA4EXyrjGEOY5OmAMyfVTSqF79bUK10Y8w,10651
+rdf_doctor-1.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+rdf_doctor-1.1.2.dist-info/entry_points.txt,sha256=1vHyYdY5pMK7zOINHh2ymwU_Uid1YzZx7Vte5tjHCls,52
+rdf_doctor-1.1.2.dist-info/top_level.txt,sha256=8awHkjBkPxJ8N_ygAwmuUTUz5ZKfy9aqNcWTSI_Ma_8,7
+rdf_doctor-1.1.2.dist-info/RECORD,,
```

