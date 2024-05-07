# Comparing `tmp/skrutable-1.3.0.dev1.tar.gz` & `tmp/skrutable-1.3.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skrutable-1.3.0.dev1.tar", last modified: Tue May  7 00:14:12 2024, max compression
+gzip compressed data, was "skrutable-1.3.0.dev2.tar", last modified: Tue May  7 00:33:32 2024, max compression
```

## Comparing `skrutable-1.3.0.dev1.tar` & `skrutable-1.3.0.dev2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-07 00:14:12.038125 skrutable-1.3.0.dev1/
--rw-r--r--   0 tyler      (501) staff       (20)      165 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev1/LICENSE.md
--rw-r--r--   0 tyler      (501) staff       (20)      414 2024-05-07 00:14:12.038060 skrutable-1.3.0.dev1/PKG-INFO
--rw-r--r--   0 tyler      (501) staff       (20)      824 2024-05-06 02:59:42.000000 skrutable-1.3.0.dev1/README.md
--rw-r--r--   0 tyler      (501) staff       (20)      106 2024-05-07 00:14:12.038318 skrutable-1.3.0.dev1/setup.cfg
--rw-r--r--   0 tyler      (501) staff       (20)      784 2024-05-07 00:13:28.000000 skrutable-1.3.0.dev1/setup.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-07 00:14:12.031524 skrutable-1.3.0.dev1/src/
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-07 00:14:12.036771 skrutable-1.3.0.dev1/src/skrutable/
--rw-r--r--   0 tyler      (501) staff       (20)     1115 2024-05-06 03:32:29.000000 skrutable-1.3.0.dev1/src/skrutable/config.json
--rw-r--r--   0 tyler      (501) staff       (20)      281 2024-05-06 12:26:54.000000 skrutable-1.3.0.dev1/src/skrutable/config.py
--rw-r--r--   0 tyler      (501) staff       (20)    16697 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev1/src/skrutable/manual.md
--rw-r--r--   0 tyler      (501) staff       (20)    27225 2024-05-07 00:13:55.000000 skrutable-1.3.0.dev1/src/skrutable/meter_identification.py
--rw-r--r--   0 tyler      (501) staff       (20)    12348 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev1/src/skrutable/meter_patterns.py
--rw-r--r--   0 tyler      (501) staff       (20)     4957 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev1/src/skrutable/phonemes.py
--rw-r--r--   0 tyler      (501) staff       (20)    10736 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev1/src/skrutable/scansion.py
--rw-r--r--   0 tyler      (501) staff       (20)     1339 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev1/src/skrutable/scheme_detection.py
--rw-r--r--   0 tyler      (501) staff       (20)    17766 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev1/src/skrutable/scheme_maps.py
--rw-r--r--   0 tyler      (501) staff       (20)   212298 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev1/src/skrutable/scheme_vectors_mbh.py
--rw-r--r--   0 tyler      (501) staff       (20)     2933 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev1/src/skrutable/skrutable_one.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-07 00:14:12.037549 skrutable-1.3.0.dev1/src/skrutable/splitter/
--rw-r--r--   0 tyler      (501) staff       (20)     7878 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev1/src/skrutable/splitter/wrapper.py
--rw-r--r--   0 tyler      (501) staff       (20)     5532 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev1/src/skrutable/transliteration.py
--rw-r--r--   0 tyler      (501) staff       (20)     1435 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev1/src/skrutable/virAma_avoidance.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-07 00:14:12.037840 skrutable-1.3.0.dev1/src/skrutable.egg-info/
--rw-r--r--   0 tyler      (501) staff       (20)      414 2024-05-07 00:14:12.000000 skrutable-1.3.0.dev1/src/skrutable.egg-info/PKG-INFO
--rw-r--r--   0 tyler      (501) staff       (20)      650 2024-05-07 00:14:12.000000 skrutable-1.3.0.dev1/src/skrutable.egg-info/SOURCES.txt
--rw-r--r--   0 tyler      (501) staff       (20)        1 2024-05-07 00:14:12.000000 skrutable-1.3.0.dev1/src/skrutable.egg-info/dependency_links.txt
--rw-r--r--   0 tyler      (501) staff       (20)       15 2024-05-07 00:14:12.000000 skrutable-1.3.0.dev1/src/skrutable.egg-info/requires.txt
--rw-r--r--   0 tyler      (501) staff       (20)       10 2024-05-07 00:14:12.000000 skrutable-1.3.0.dev1/src/skrutable.egg-info/top_level.txt
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-07 00:33:32.705302 skrutable-1.3.0.dev2/
+-rw-r--r--   0 tyler      (501) staff       (20)      165 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev2/LICENSE.md
+-rw-r--r--   0 tyler      (501) staff       (20)      414 2024-05-07 00:33:32.705247 skrutable-1.3.0.dev2/PKG-INFO
+-rw-r--r--   0 tyler      (501) staff       (20)      824 2024-05-06 02:59:42.000000 skrutable-1.3.0.dev2/README.md
+-rw-r--r--   0 tyler      (501) staff       (20)      106 2024-05-07 00:33:32.705491 skrutable-1.3.0.dev2/setup.cfg
+-rw-r--r--   0 tyler      (501) staff       (20)     1198 2024-05-07 00:33:21.000000 skrutable-1.3.0.dev2/setup.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-07 00:33:32.698439 skrutable-1.3.0.dev2/src/
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-07 00:33:32.703889 skrutable-1.3.0.dev2/src/skrutable/
+-rw-r--r--   0 tyler      (501) staff       (20)       26 2024-05-07 00:33:21.000000 skrutable-1.3.0.dev2/src/skrutable/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1115 2024-05-06 03:32:29.000000 skrutable-1.3.0.dev2/src/skrutable/config.json
+-rw-r--r--   0 tyler      (501) staff       (20)      281 2024-05-06 12:26:54.000000 skrutable-1.3.0.dev2/src/skrutable/config.py
+-rw-r--r--   0 tyler      (501) staff       (20)    16697 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev2/src/skrutable/manual.md
+-rw-r--r--   0 tyler      (501) staff       (20)    27225 2024-05-07 00:13:55.000000 skrutable-1.3.0.dev2/src/skrutable/meter_identification.py
+-rw-r--r--   0 tyler      (501) staff       (20)    12348 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev2/src/skrutable/meter_patterns.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4957 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev2/src/skrutable/phonemes.py
+-rw-r--r--   0 tyler      (501) staff       (20)    10736 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev2/src/skrutable/scansion.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1339 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev2/src/skrutable/scheme_detection.py
+-rw-r--r--   0 tyler      (501) staff       (20)    17766 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev2/src/skrutable/scheme_maps.py
+-rw-r--r--   0 tyler      (501) staff       (20)   212298 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev2/src/skrutable/scheme_vectors_mbh.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2933 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev2/src/skrutable/skrutable_one.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-07 00:33:32.704592 skrutable-1.3.0.dev2/src/skrutable/splitter/
+-rw-r--r--   0 tyler      (501) staff       (20)     7878 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev2/src/skrutable/splitter/wrapper.py
+-rw-r--r--   0 tyler      (501) staff       (20)     5532 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev2/src/skrutable/transliteration.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1435 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev2/src/skrutable/virAma_avoidance.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-07 00:33:32.705010 skrutable-1.3.0.dev2/src/skrutable.egg-info/
+-rw-r--r--   0 tyler      (501) staff       (20)      414 2024-05-07 00:33:32.000000 skrutable-1.3.0.dev2/src/skrutable.egg-info/PKG-INFO
+-rw-r--r--   0 tyler      (501) staff       (20)      676 2024-05-07 00:33:32.000000 skrutable-1.3.0.dev2/src/skrutable.egg-info/SOURCES.txt
+-rw-r--r--   0 tyler      (501) staff       (20)        1 2024-05-07 00:33:32.000000 skrutable-1.3.0.dev2/src/skrutable.egg-info/dependency_links.txt
+-rw-r--r--   0 tyler      (501) staff       (20)       15 2024-05-07 00:33:32.000000 skrutable-1.3.0.dev2/src/skrutable.egg-info/requires.txt
+-rw-r--r--   0 tyler      (501) staff       (20)       10 2024-05-07 00:33:32.000000 skrutable-1.3.0.dev2/src/skrutable.egg-info/top_level.txt
```

### Comparing `skrutable-1.3.0.dev1/README.md` & `skrutable-1.3.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `skrutable-1.3.0.dev1/src/skrutable/config.json` & `skrutable-1.3.0.dev2/src/skrutable/config.json`

 * *Files identical despite different names*

### Comparing `skrutable-1.3.0.dev1/src/skrutable/manual.md` & `skrutable-1.3.0.dev2/src/skrutable/manual.md`

 * *Files identical despite different names*

### Comparing `skrutable-1.3.0.dev1/src/skrutable/meter_identification.py` & `skrutable-1.3.0.dev2/src/skrutable/meter_identification.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.3.0.dev1/src/skrutable/meter_patterns.py` & `skrutable-1.3.0.dev2/src/skrutable/meter_patterns.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.3.0.dev1/src/skrutable/phonemes.py` & `skrutable-1.3.0.dev2/src/skrutable/phonemes.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.3.0.dev1/src/skrutable/scansion.py` & `skrutable-1.3.0.dev2/src/skrutable/scansion.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.3.0.dev1/src/skrutable/scheme_detection.py` & `skrutable-1.3.0.dev2/src/skrutable/scheme_detection.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.3.0.dev1/src/skrutable/scheme_maps.py` & `skrutable-1.3.0.dev2/src/skrutable/scheme_maps.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.3.0.dev1/src/skrutable/scheme_vectors_mbh.py` & `skrutable-1.3.0.dev2/src/skrutable/scheme_vectors_mbh.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.3.0.dev1/src/skrutable/skrutable_one.py` & `skrutable-1.3.0.dev2/src/skrutable/skrutable_one.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.3.0.dev1/src/skrutable/splitter/wrapper.py` & `skrutable-1.3.0.dev2/src/skrutable/splitter/wrapper.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.3.0.dev1/src/skrutable/transliteration.py` & `skrutable-1.3.0.dev2/src/skrutable/transliteration.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.3.0.dev1/src/skrutable/virAma_avoidance.py` & `skrutable-1.3.0.dev2/src/skrutable/virAma_avoidance.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.3.0.dev1/src/skrutable.egg-info/SOURCES.txt` & `skrutable-1.3.0.dev2/src/skrutable.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.md
 README.md
 setup.cfg
 setup.py
+src/skrutable/__init__.py
 src/skrutable/config.json
 src/skrutable/config.py
 src/skrutable/manual.md
 src/skrutable/meter_identification.py
 src/skrutable/meter_patterns.py
 src/skrutable/phonemes.py
 src/skrutable/scansion.py
```

