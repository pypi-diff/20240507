# Comparing `tmp/python_spike_beta-0.0.1-py3-none-any.whl.zip` & `tmp/python_spike_beta-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2517 bytes, number of entries: 7
--rw-r--r--  2.0 unx       24 b- defN 24-May-07 13:40 python_spike_beta/__init__.py
+Zip file size: 2535 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       42 b- defN 24-May-07 13:44 python_spike_beta/__init__.py
 -rw-r--r--  2.0 unx      116 b- defN 24-May-07 13:22 python_spike_beta/main.py
--rw-r--r--  2.0 unx     1063 b- defN 24-May-07 13:41 python_spike_beta-0.0.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      330 b- defN 24-May-07 13:41 python_spike_beta-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-07 13:41 python_spike_beta-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 24-May-07 13:41 python_spike_beta-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      604 b- defN 24-May-07 13:41 python_spike_beta-0.0.1.dist-info/RECORD
-7 files, 2247 bytes uncompressed, 1429 bytes compressed:  36.4%
+-rw-r--r--  2.0 unx     1063 b- defN 24-May-07 13:46 python_spike_beta-0.0.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      330 b- defN 24-May-07 13:46 python_spike_beta-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-07 13:46 python_spike_beta-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 24-May-07 13:46 python_spike_beta-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      604 b- defN 24-May-07 13:46 python_spike_beta-0.0.2.dist-info/RECORD
+7 files, 2265 bytes uncompressed, 1447 bytes compressed:  36.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: python_spike_beta/__init__.py
 Comment: 
 
 Filename: python_spike_beta/main.py
 Comment: 
 
-Filename: python_spike_beta-0.0.1.dist-info/LICENSE.txt
+Filename: python_spike_beta-0.0.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: python_spike_beta-0.0.1.dist-info/METADATA
+Filename: python_spike_beta-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: python_spike_beta-0.0.1.dist-info/WHEEL
+Filename: python_spike_beta-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: python_spike_beta-0.0.1.dist-info/top_level.txt
+Filename: python_spike_beta-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: python_spike_beta-0.0.1.dist-info/RECORD
+Filename: python_spike_beta-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## python_spike_beta/__init__.py

```diff
@@ -1 +1 @@
-from main import PySpike
+from python_spike_beta.main import PySpike
```

## Comparing `python_spike_beta-0.0.1.dist-info/LICENSE.txt` & `python_spike_beta-0.0.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `python_spike_beta-0.0.1.dist-info/RECORD` & `python_spike_beta-0.0.2.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-python_spike_beta/__init__.py,sha256=PziJ4HY-zUohQuYefr3n5jEEKr6QDafB9MV1ixHhZTE,24
+python_spike_beta/__init__.py,sha256=kKTtHPCgmC-FFgemTaEglIRuqNtzIQNkU7jKW0HZQtg,42
 python_spike_beta/main.py,sha256=JnaF-cyHAHIiHdnczvj2A0Udno_P7UNXIc5jQl1AHsk,116
-python_spike_beta-0.0.1.dist-info/LICENSE.txt,sha256=K8sUz4-6H5CTMJ-bDAXsmw_vMuPbf4IMYvLCQsvUzlk,1063
-python_spike_beta-0.0.1.dist-info/METADATA,sha256=RMnBirQWv0mnA5eyZAI75rYgQTxIJd_-njVEM4_W8EY,330
-python_spike_beta-0.0.1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-python_spike_beta-0.0.1.dist-info/top_level.txt,sha256=4XnhRpTR-njEIhqCjSbyTpsox60RM7U8KotWBC3Bl54,18
-python_spike_beta-0.0.1.dist-info/RECORD,,
+python_spike_beta-0.0.2.dist-info/LICENSE.txt,sha256=K8sUz4-6H5CTMJ-bDAXsmw_vMuPbf4IMYvLCQsvUzlk,1063
+python_spike_beta-0.0.2.dist-info/METADATA,sha256=RVEKDVc0Frg07qywKKTi_9lhYuMAGs6AAyR7p4alr2s,330
+python_spike_beta-0.0.2.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+python_spike_beta-0.0.2.dist-info/top_level.txt,sha256=4XnhRpTR-njEIhqCjSbyTpsox60RM7U8KotWBC3Bl54,18
+python_spike_beta-0.0.2.dist-info/RECORD,,
```

