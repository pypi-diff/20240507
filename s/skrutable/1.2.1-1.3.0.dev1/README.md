# Comparing `tmp/skrutable-1.2.1.tar.gz` & `tmp/skrutable-1.3.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skrutable-1.2.1.tar", last modified: Sun May  5 02:37:52 2024, max compression
+gzip compressed data, was "skrutable-1.3.0.dev1.tar", last modified: Tue May  7 00:14:12 2024, max compression
```

## Comparing `skrutable-1.2.1.tar` & `skrutable-1.3.0.dev1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-05 02:37:52.351500 skrutable-1.2.1/
--rw-r--r--   0 tyler      (501) staff       (20)      165 2024-05-05 02:36:03.000000 skrutable-1.2.1/LICENSE.md
--rw-r--r--   0 tyler      (501) staff       (20)      409 2024-05-05 02:37:52.351446 skrutable-1.2.1/PKG-INFO
--rw-r--r--   0 tyler      (501) staff       (20)      716 2024-05-05 02:06:10.000000 skrutable-1.2.1/README.md
--rw-r--r--   0 tyler      (501) staff       (20)      106 2024-05-05 02:37:52.351694 skrutable-1.2.1/setup.cfg
--rw-r--r--   0 tyler      (501) staff       (20)      779 2024-05-05 02:36:42.000000 skrutable-1.2.1/setup.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-05 02:37:52.345083 skrutable-1.2.1/src/
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-05 02:37:52.350210 skrutable-1.2.1/src/skrutable/
--rw-r--r--   0 tyler      (501) staff       (20)     1077 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/config.json
--rw-r--r--   0 tyler      (501) staff       (20)      281 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/config.py
--rw-r--r--   0 tyler      (501) staff       (20)    16697 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/manual.md
--rw-r--r--   0 tyler      (501) staff       (20)    26789 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/meter_identification.py
--rw-r--r--   0 tyler      (501) staff       (20)    12348 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/meter_patterns.py
--rw-r--r--   0 tyler      (501) staff       (20)     4957 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/phonemes.py
--rw-r--r--   0 tyler      (501) staff       (20)    10736 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/scansion.py
--rw-r--r--   0 tyler      (501) staff       (20)     1339 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/scheme_detection.py
--rw-r--r--   0 tyler      (501) staff       (20)    17766 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/scheme_maps.py
--rw-r--r--   0 tyler      (501) staff       (20)   212298 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/scheme_vectors_mbh.py
--rw-r--r--   0 tyler      (501) staff       (20)     2933 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/skrutable_one.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-05 02:37:52.350929 skrutable-1.2.1/src/skrutable/splitter/
--rw-r--r--   0 tyler      (501) staff       (20)     7878 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/splitter/wrapper.py
--rw-r--r--   0 tyler      (501) staff       (20)     5532 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/transliteration.py
--rw-r--r--   0 tyler      (501) staff       (20)     1435 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/virAma_avoidance.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-05 02:37:52.351241 skrutable-1.2.1/src/skrutable.egg-info/
--rw-r--r--   0 tyler      (501) staff       (20)      409 2024-05-05 02:37:52.000000 skrutable-1.2.1/src/skrutable.egg-info/PKG-INFO
--rw-r--r--   0 tyler      (501) staff       (20)      650 2024-05-05 02:37:52.000000 skrutable-1.2.1/src/skrutable.egg-info/SOURCES.txt
--rw-r--r--   0 tyler      (501) staff       (20)        1 2024-05-05 02:37:52.000000 skrutable-1.2.1/src/skrutable.egg-info/dependency_links.txt
--rw-r--r--   0 tyler      (501) staff       (20)       15 2024-05-05 02:37:52.000000 skrutable-1.2.1/src/skrutable.egg-info/requires.txt
--rw-r--r--   0 tyler      (501) staff       (20)       10 2024-05-05 02:37:52.000000 skrutable-1.2.1/src/skrutable.egg-info/top_level.txt
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-07 00:14:12.038125 skrutable-1.3.0.dev1/
+-rw-r--r--   0 tyler      (501) staff       (20)      165 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev1/LICENSE.md
+-rw-r--r--   0 tyler      (501) staff       (20)      414 2024-05-07 00:14:12.038060 skrutable-1.3.0.dev1/PKG-INFO
+-rw-r--r--   0 tyler      (501) staff       (20)      824 2024-05-06 02:59:42.000000 skrutable-1.3.0.dev1/README.md
+-rw-r--r--   0 tyler      (501) staff       (20)      106 2024-05-07 00:14:12.038318 skrutable-1.3.0.dev1/setup.cfg
+-rw-r--r--   0 tyler      (501) staff       (20)      784 2024-05-07 00:13:28.000000 skrutable-1.3.0.dev1/setup.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-07 00:14:12.031524 skrutable-1.3.0.dev1/src/
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-07 00:14:12.036771 skrutable-1.3.0.dev1/src/skrutable/
+-rw-r--r--   0 tyler      (501) staff       (20)     1115 2024-05-06 03:32:29.000000 skrutable-1.3.0.dev1/src/skrutable/config.json
+-rw-r--r--   0 tyler      (501) staff       (20)      281 2024-05-06 12:26:54.000000 skrutable-1.3.0.dev1/src/skrutable/config.py
+-rw-r--r--   0 tyler      (501) staff       (20)    16697 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev1/src/skrutable/manual.md
+-rw-r--r--   0 tyler      (501) staff       (20)    27225 2024-05-07 00:13:55.000000 skrutable-1.3.0.dev1/src/skrutable/meter_identification.py
+-rw-r--r--   0 tyler      (501) staff       (20)    12348 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev1/src/skrutable/meter_patterns.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4957 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev1/src/skrutable/phonemes.py
+-rw-r--r--   0 tyler      (501) staff       (20)    10736 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev1/src/skrutable/scansion.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1339 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev1/src/skrutable/scheme_detection.py
+-rw-r--r--   0 tyler      (501) staff       (20)    17766 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev1/src/skrutable/scheme_maps.py
+-rw-r--r--   0 tyler      (501) staff       (20)   212298 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev1/src/skrutable/scheme_vectors_mbh.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2933 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev1/src/skrutable/skrutable_one.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-07 00:14:12.037549 skrutable-1.3.0.dev1/src/skrutable/splitter/
+-rw-r--r--   0 tyler      (501) staff       (20)     7878 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev1/src/skrutable/splitter/wrapper.py
+-rw-r--r--   0 tyler      (501) staff       (20)     5532 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev1/src/skrutable/transliteration.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1435 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev1/src/skrutable/virAma_avoidance.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-07 00:14:12.037840 skrutable-1.3.0.dev1/src/skrutable.egg-info/
+-rw-r--r--   0 tyler      (501) staff       (20)      414 2024-05-07 00:14:12.000000 skrutable-1.3.0.dev1/src/skrutable.egg-info/PKG-INFO
+-rw-r--r--   0 tyler      (501) staff       (20)      650 2024-05-07 00:14:12.000000 skrutable-1.3.0.dev1/src/skrutable.egg-info/SOURCES.txt
+-rw-r--r--   0 tyler      (501) staff       (20)        1 2024-05-07 00:14:12.000000 skrutable-1.3.0.dev1/src/skrutable.egg-info/dependency_links.txt
+-rw-r--r--   0 tyler      (501) staff       (20)       15 2024-05-07 00:14:12.000000 skrutable-1.3.0.dev1/src/skrutable.egg-info/requires.txt
+-rw-r--r--   0 tyler      (501) staff       (20)       10 2024-05-07 00:14:12.000000 skrutable-1.3.0.dev1/src/skrutable.egg-info/top_level.txt
```

### Comparing `skrutable-1.2.1/README.md` & `skrutable-1.3.0.dev1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 A toolkit and online workbench providing 
 transliteration, scansion, and meter identification for Sanskrit text,
 as well access to powerful sandhi and compound splitting.
 
 Web-app interface live online at [skrutable.info](https://www.skrutable.info).
 
-See [manual.md](https://github.com/tylergneill/skrutable/blob/master/manual.md) for instructions.
+Install package from [PyPi](https://pypi.org/project/skrutable/) with `pip install skrutable`.
+
+See [manual.md](https://github.com/tylergneill/skrutable/blob/main/src/skrutable/manual.md) for instructions.
 
 Feedback welcome!
 My name is Tyler 
 ([Academia](https://uni-leipzig1.academia.edu/TylerNeill),
 [LinkedIn](https://www.linkedin.com/in/tyler-g-neill/))
 and my Gmail is tyler.g.neill.
```

### Comparing `skrutable-1.2.1/setup.py` & `skrutable-1.3.0.dev1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='skrutable',
-    version='1.2.1',
+    version='1.3.0.dev1',
     description="skrutable library for working with Sanskrit text",
     license='CC BY-SA 4.0',
     author="Tyler Neill",
     author_email='tyler.g.neill@gmail.com',
     package_dir={'':'src'},
     packages=[
     	"skrutable",
```

### Comparing `skrutable-1.2.1/src/skrutable/config.json` & `skrutable-1.3.0.dev1/src/skrutable/config.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976076555023923%*

 * *Differences: {"'meter_scores'": "{'samavṛtta, quarter, perfect': 8}"}*

```diff
@@ -23,14 +23,15 @@
         "j\u0101ti, imperfect": 3,
         "j\u0101ti, perfect": 8,
         "max score": 9,
         "none found": 1,
         "samav\u1e5btta, imperfect (2)": 5,
         "samav\u1e5btta, imperfect (3)": 6,
         "samav\u1e5btta, perfect": 9,
+        "samav\u1e5btta, quarter, perfect": 8,
         "upaj\u0101ti, imperfect": 6,
         "upaj\u0101ti, non-tri\u1e63\u1e6dubh, imperfect": 3,
         "upaj\u0101ti, non-tri\u1e63\u1e6dubh, perfect": 5,
         "upaj\u0101ti, perfect": 7,
         "upaj\u0101ti, tri\u1e63\u1e6dubh-jagat\u012b-sa\u1e43kara, perfect": 4,
         "vi\u1e63amav\u1e5btta, perfect": 9
     },
```

### Comparing `skrutable-1.2.1/src/skrutable/manual.md` & `skrutable-1.3.0.dev1/src/skrutable/manual.md`

 * *Files identical despite different names*

### Comparing `skrutable-1.2.1/src/skrutable/meter_identification.py` & `skrutable-1.3.0.dev1/src/skrutable/meter_identification.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,17 +188,20 @@
 			meter_label += ' [%d: %s]' % ( len(w_to_id), g_to_id )
 
 		score = meter_scores["samavṛtta, perfect"]
 
 		if self.pAdasamatva_count == 3:
 			meter_label += " (? 3 eva pādāḥ yuktāḥ)"
 			score = meter_scores["samavṛtta, imperfect (3)"]
-		if self.pAdasamatva_count == 2:
+		elif self.pAdasamatva_count == 2:
 			meter_label += " (? 2 eva pādāḥ yuktāḥ)"
 			score = meter_scores["samavṛtta, imperfect (2)"]
+		elif self.pAdasamatva_count == 0:
+			meter_label += " (1 eva pādaḥ)"
+			score = meter_scores["samavṛtta, quarter, perfect"]
 
 		# experimental penalty, can later incorporate into config meter_scores
 		if meter_label == "ajñātasamavṛtta":
 			score -= 2
 
 		# may tie with pre-existing result (e.g., upajāti)
 		self.combine_results(Vrs, new_label=meter_label, new_score=score)
@@ -350,14 +353,15 @@
 
 		self.combine_results(Vrs, overall_meter_label, score)
 
 
 	def is_vizamavftta(self, Vrs):
 
 		gs_to_id = Vrs.gaRa_abbreviations.split('\n')
+		if len(gs_to_id) < 4: return False
 
 		for (a, b, c, d) in meter_patterns.vizamavftta_by_4_tuple:
 			if (gs_to_id[0],gs_to_id[1],gs_to_id[2],gs_to_id[3]) == (a, b, c, d):
 				Vrs.identification_score = meter_scores["viṣamavṛtta, perfect"]
 				Vrs.meter_label = meter_patterns.vizamavftta_by_4_tuple[(a, b, c, d)]
 				return True
 
@@ -367,15 +371,19 @@
 	def test_as_samavftta_etc(self, Vrs):
 
 		wbp = Vrs.syllable_weights.split('\n') # weights by pāda
 		wbp_lens = [ len(line) for line in wbp ]
 
 		# make sure full four pādas
 		try: wbp[3]
-		except IndexError: return 0
+		except IndexError:
+			if self.resplit_option == "single_pAda" and len(wbp) == 1:
+				pass
+			else:
+				return 0
 
 		self.count_pAdasamatva(Vrs) # [0,2,3,4]
 
 		# test in following order to prioritize left-right presentation of ties
 		# ties managed in self.combine_results()
 
 		# test perfect samavṛtta
@@ -391,14 +399,19 @@
 
 			 and wbp_lens.count(11) != 4 # bc triṣṭubh upajāti so common
 			 ):
 			# will give id_score == 8
 			self.evaluate_ardhasamavftta(Vrs)
 			# max score not necessarily yet reached, don't return
 
+		# test perfect single pāda of samavṛtta
+		if ( self.pAdasamatva_count == 0 and self.resplit_option == "single_pAda"):
+			self.evaluate_samavftta(Vrs)
+			#....
+
 		# test perfect viṣamavṛtta
 		if self.pAdasamatva_count == 0 and self.is_vizamavftta(Vrs):
 			# will give id_score == 9
 			# label and score already set in is_vizamavftta if test was successful
 			return 1 # max score already reached
 
 		# test perfect upajāti
@@ -726,15 +739,15 @@
 		# gets back mostly populated Verse object
 		V = S.scan(rw_str, from_scheme=from_scheme)
 
 		self.VerseTester = VT = VerseTester()
 		self.VerseTester.resplit_option = resplit_option
 		self.VerseTester.resplit_keep_midpoint = resplit_keep_midpoint
 
-		if resplit_option == 'none' or V.text_cleaned == '':
+		if resplit_option in ['none', 'single_pAda'] or V.text_cleaned == '':
 			success = VT.attempt_identification(V)
 			# label and score set internally
 
 		elif resplit_option in ['resplit_max', 'resplit_lite']:
 
 			# capture any user-provided pāda breaks (= all newlines after scansion cleaning)
 			newline_indices = [
```

### Comparing `skrutable-1.2.1/src/skrutable/meter_patterns.py` & `skrutable-1.3.0.dev1/src/skrutable/meter_patterns.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.2.1/src/skrutable/phonemes.py` & `skrutable-1.3.0.dev1/src/skrutable/phonemes.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.2.1/src/skrutable/scansion.py` & `skrutable-1.3.0.dev1/src/skrutable/scansion.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.2.1/src/skrutable/scheme_detection.py` & `skrutable-1.3.0.dev1/src/skrutable/scheme_detection.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.2.1/src/skrutable/scheme_maps.py` & `skrutable-1.3.0.dev1/src/skrutable/scheme_maps.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.2.1/src/skrutable/scheme_vectors_mbh.py` & `skrutable-1.3.0.dev1/src/skrutable/scheme_vectors_mbh.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.2.1/src/skrutable/skrutable_one.py` & `skrutable-1.3.0.dev1/src/skrutable/skrutable_one.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.2.1/src/skrutable/splitter/wrapper.py` & `skrutable-1.3.0.dev1/src/skrutable/splitter/wrapper.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.2.1/src/skrutable/transliteration.py` & `skrutable-1.3.0.dev1/src/skrutable/transliteration.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.2.1/src/skrutable/virAma_avoidance.py` & `skrutable-1.3.0.dev1/src/skrutable/virAma_avoidance.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.2.1/src/skrutable.egg-info/SOURCES.txt` & `skrutable-1.3.0.dev1/src/skrutable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

