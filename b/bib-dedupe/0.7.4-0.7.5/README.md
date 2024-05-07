# Comparing `tmp/bib_dedupe-0.7.4.tar.gz` & `tmp/bib_dedupe-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bib_dedupe-0.7.4.tar", max compression
+gzip compressed data, was "bib_dedupe-0.7.5.tar", max compression
```

## Comparing `bib_dedupe-0.7.4.tar` & `bib_dedupe-0.7.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1070 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/LICENSE
--rw-r--r--   0        0        0     3867 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/README.md
--rw-r--r--   0        0        0      411 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/__init__.py
--rw-r--r--   0        0        0     6496 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/bib_dedupe.py
--rw-r--r--   0        0        0     8465 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/block.py
--rw-r--r--   0        0        0      269 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/cli.py
--rw-r--r--   0        0        0     2795 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/cluster.py
--rw-r--r--   0        0        0      253 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/constants/__init__.py
--rw-r--r--   0        0        0      191 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/constants/colors.py
--rw-r--r--   0        0        0      490 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/constants/entrytypes.py
--rw-r--r--   0        0        0     1033 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/constants/fields.py
--rw-r--r--   0        0        0     2212 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/debug.py
--rw-r--r--   0        0        0    19504 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/dedupe_benchmark.py
--rw-r--r--   0        0        0   109747 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/journal_variants.csv
--rw-r--r--   0        0        0     5770 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/match.py
--rw-r--r--   0        0        0     5683 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/match_conditions.py
--rw-r--r--   0        0        0     5789 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/maybe_cases.py
--rw-r--r--   0        0        0     7871 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/merge.py
--rw-r--r--   0        0        0     7191 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/prep.py
--rw-r--r--   0        0        0     2071 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/prep_abstract.py
--rw-r--r--   0        0        0     9428 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/prep_author.py
--rw-r--r--   0        0        0     5719 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/prep_container_title.py
--rw-r--r--   0        0        0     1220 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/prep_doi.py
--rw-r--r--   0        0        0      817 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/prep_number.py
--rw-r--r--   0        0        0     2516 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/prep_pages.py
--rw-r--r--   0        0        0     5010 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/prep_title.py
--rw-r--r--   0        0        0     1374 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/prep_volume.py
--rw-r--r--   0        0        0      573 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/prep_year.py
--rw-r--r--   0        0        0    15071 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/sim.py
--rw-r--r--   0        0        0      836 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/util.py
--rw-r--r--   0        0        0     1541 2024-04-29 05:22:59.086204 bib_dedupe-0.7.4/pyproject.toml
--rw-r--r--   0        0        0     5137 1970-01-01 00:00:00.000000 bib_dedupe-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-07 10:50:56.598713 bib_dedupe-0.7.5/LICENSE
+-rw-r--r--   0        0        0     3867 2024-05-07 10:50:56.598713 bib_dedupe-0.7.5/README.md
+-rw-r--r--   0        0        0      411 2024-05-07 10:50:56.598713 bib_dedupe-0.7.5/bib_dedupe/__init__.py
+-rw-r--r--   0        0        0     6496 2024-05-07 10:50:56.598713 bib_dedupe-0.7.5/bib_dedupe/bib_dedupe.py
+-rw-r--r--   0        0        0     8465 2024-05-07 10:50:56.598713 bib_dedupe-0.7.5/bib_dedupe/block.py
+-rw-r--r--   0        0        0      269 2024-05-07 10:50:56.598713 bib_dedupe-0.7.5/bib_dedupe/cli.py
+-rw-r--r--   0        0        0     2795 2024-05-07 10:50:56.598713 bib_dedupe-0.7.5/bib_dedupe/cluster.py
+-rw-r--r--   0        0        0      253 2024-05-07 10:50:56.598713 bib_dedupe-0.7.5/bib_dedupe/constants/__init__.py
+-rw-r--r--   0        0        0      191 2024-05-07 10:50:56.598713 bib_dedupe-0.7.5/bib_dedupe/constants/colors.py
+-rw-r--r--   0        0        0      490 2024-05-07 10:50:56.598713 bib_dedupe-0.7.5/bib_dedupe/constants/entrytypes.py
+-rw-r--r--   0        0        0     1033 2024-05-07 10:50:56.598713 bib_dedupe-0.7.5/bib_dedupe/constants/fields.py
+-rw-r--r--   0        0        0     2212 2024-05-07 10:50:56.598713 bib_dedupe-0.7.5/bib_dedupe/debug.py
+-rw-r--r--   0        0        0    19504 2024-05-07 10:50:56.598713 bib_dedupe-0.7.5/bib_dedupe/dedupe_benchmark.py
+-rw-r--r--   0        0        0   109747 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/journal_variants.csv
+-rw-r--r--   0        0        0     5852 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/match.py
+-rw-r--r--   0        0        0     5683 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/match_conditions.py
+-rw-r--r--   0        0        0     5789 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/maybe_cases.py
+-rw-r--r--   0        0        0     7871 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/merge.py
+-rw-r--r--   0        0        0     7191 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/prep.py
+-rw-r--r--   0        0        0     2071 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/prep_abstract.py
+-rw-r--r--   0        0        0     9428 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/prep_author.py
+-rw-r--r--   0        0        0     5719 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/prep_container_title.py
+-rw-r--r--   0        0        0     1220 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/prep_doi.py
+-rw-r--r--   0        0        0      817 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/prep_number.py
+-rw-r--r--   0        0        0     2516 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/prep_pages.py
+-rw-r--r--   0        0        0     5010 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/prep_title.py
+-rw-r--r--   0        0        0     1374 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/prep_volume.py
+-rw-r--r--   0        0        0      573 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/prep_year.py
+-rw-r--r--   0        0        0    15071 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/sim.py
+-rw-r--r--   0        0        0      836 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/util.py
+-rw-r--r--   0        0        0     2230 2024-05-07 10:50:57.746723 bib_dedupe-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0     5604 1970-01-01 00:00:00.000000 bib_dedupe-0.7.5/PKG-INFO
```

### Comparing `bib_dedupe-0.7.4/LICENSE` & `bib_dedupe-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.4/README.md` & `bib_dedupe-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.4/bib_dedupe/bib_dedupe.py` & `bib_dedupe-0.7.5/bib_dedupe/bib_dedupe.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.4/bib_dedupe/block.py` & `bib_dedupe-0.7.5/bib_dedupe/block.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.4/bib_dedupe/cluster.py` & `bib_dedupe-0.7.5/bib_dedupe/cluster.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.4/bib_dedupe/constants/fields.py` & `bib_dedupe-0.7.5/bib_dedupe/constants/fields.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.4/bib_dedupe/debug.py` & `bib_dedupe-0.7.5/bib_dedupe/debug.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.4/bib_dedupe/dedupe_benchmark.py` & `bib_dedupe-0.7.5/bib_dedupe/dedupe_benchmark.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.4/bib_dedupe/journal_variants.csv` & `bib_dedupe-0.7.5/bib_dedupe/journal_variants.csv`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.4/bib_dedupe/match.py` & `bib_dedupe-0.7.5/bib_dedupe/match.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,32 +64,34 @@
         elif similarity > 0.6:
             verbose_print.print(f"{ORANGE}Similarity {item:<20}: {similarity:.2f}{END}")
         else:
             verbose_print.print(f"{RED}Similarity {item:<20}: {similarity:.2f}{END}")
 
     verbose_print.print("Merge conditions that matched:")
     for duplicate_condition in DUPLICATE_CONDITIONS:
-        if pairs.query(duplicate_condition).shape[0] > 0:
+        if pairs.query(duplicate_condition, engine="python").shape[0] > 0:
             verbose_print.print(f"{GREEN}{duplicate_condition}{END}")
         else:
             verbose_print.print(f"{duplicate_condition}")
 
     verbose_print.print()
     verbose_print.print(pairs)
     verbose_print.print("Non-merge conditions that matched:")
     for non_duplicate_condition in NON_DUPLICATE_CONDITIONS:
-        if pairs.query(non_duplicate_condition).shape[0] != 0:
+        if pairs.query(non_duplicate_condition, engine="python").shape[0] != 0:
             verbose_print.print(f"{RED}{non_duplicate_condition}{END}")
         else:
             verbose_print.print(non_duplicate_condition)
 
 
 def __get_true_pairs(pairs: pd.DataFrame) -> pd.DataFrame:
-    true_pairs = pairs.query("|".join(DUPLICATE_CONDITIONS))
-    true_pairs = true_pairs.query("~(" + " | ".join(NON_DUPLICATE_CONDITIONS) + ")")
+    true_pairs = pairs.query("|".join(DUPLICATE_CONDITIONS), engine="python")
+    true_pairs = true_pairs.query(
+        "~(" + " | ".join(NON_DUPLICATE_CONDITIONS) + ")", engine="python"
+    )
     true_pairs = true_pairs.drop_duplicates()
 
     # Add a label column to each dataframe
     true_pairs[DUPLICATE_LABEL] = DUPLICATE
     # Select the ID_1 and ID_2 fields and the new label column
     true_pairs = true_pairs[[f"{ID}_1", f"{ID}_2", DUPLICATE_LABEL]]
```

### Comparing `bib_dedupe-0.7.4/bib_dedupe/match_conditions.py` & `bib_dedupe-0.7.5/bib_dedupe/match_conditions.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.4/bib_dedupe/maybe_cases.py` & `bib_dedupe-0.7.5/bib_dedupe/maybe_cases.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.4/bib_dedupe/merge.py` & `bib_dedupe-0.7.5/bib_dedupe/merge.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.4/bib_dedupe/prep.py` & `bib_dedupe-0.7.5/bib_dedupe/prep.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.4/bib_dedupe/prep_abstract.py` & `bib_dedupe-0.7.5/bib_dedupe/prep_abstract.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.4/bib_dedupe/prep_author.py` & `bib_dedupe-0.7.5/bib_dedupe/prep_author.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.4/bib_dedupe/prep_container_title.py` & `bib_dedupe-0.7.5/bib_dedupe/prep_container_title.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.4/bib_dedupe/prep_doi.py` & `bib_dedupe-0.7.5/bib_dedupe/prep_doi.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.4/bib_dedupe/prep_number.py` & `bib_dedupe-0.7.5/bib_dedupe/prep_number.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.4/bib_dedupe/prep_pages.py` & `bib_dedupe-0.7.5/bib_dedupe/prep_pages.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.4/bib_dedupe/prep_title.py` & `bib_dedupe-0.7.5/bib_dedupe/prep_title.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.4/bib_dedupe/prep_volume.py` & `bib_dedupe-0.7.5/bib_dedupe/prep_volume.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.4/bib_dedupe/prep_year.py` & `bib_dedupe-0.7.5/bib_dedupe/prep_year.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.4/bib_dedupe/sim.py` & `bib_dedupe-0.7.5/bib_dedupe/sim.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.4/bib_dedupe/util.py` & `bib_dedupe-0.7.5/bib_dedupe/util.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.4/PKG-INFO` & `bib_dedupe-0.7.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 Metadata-Version: 2.1
 Name: bib-dedupe
-Version: 0.7.4
+Version: 0.7.5
 Summary: Identify and merge duplicates in bibliographic records
+Home-page: https://github.com/CoLRev-Environment/bib-dedupe
 License: MIT
+Keywords: de-duplication,duplicate,meta-analysis,research,reproducible research,open science,literature,literature review,systematic review,systematic literature review
 Author: Gerit Wagner
 Author-email: gerit.wagner@uni-bamberg.de
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering
+Classifier: Typing :: Typed
 Provides-Extra: dev
 Provides-Extra: with-data
 Requires-Dist: asreview (>=1.5,<2.0) ; extra == "with-data"
 Requires-Dist: coverage[toml] (>=7.3.2,<8.0.0) ; extra == "dev"
-Requires-Dist: notebook (>=6.4.11,<7.0.0) ; extra == "with-data"
 Requires-Dist: number-parser (>=0.3.2,<0.4.0)
 Requires-Dist: numpy (>=1.19.5,<2.0.0)
 Requires-Dist: pandas (>=1.3.4,<2.0.0) ; extra == "with-data"
 Requires-Dist: pylint (==3.0.1) ; extra == "dev"
 Requires-Dist: pytest (>=7.2.1,<8.0.0) ; extra == "dev"
 Requires-Dist: rapidfuzz (>=3.5.2,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: setuptools (>=69.1.1,<70.0.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
+Project-URL: Documentation, https://colrev-environment.github.io/bib-dedupe/
+Project-URL: Repository, https://github.com/CoLRev-Environment/bib-dedupe
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # BibDedupe
```

