# Comparing `tmp/name_matching-0.8.8.tar.gz` & `tmp/name_matching-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "name_matching-0.8.8.tar", last modified: Sun Oct 15 14:56:15 2023, max compression
+gzip compressed data, was "name_matching-0.8.9.tar", last modified: Fri Nov  3 12:38:51 2023, max compression
```

## Comparing `name_matching-0.8.8.tar` & `name_matching-0.8.9.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-10-15 14:56:15.232308 name_matching-0.8.8/
--rw-rw-rw-   0        0        0     4035 2023-10-15 14:56:15.233312 name_matching-0.8.8/PKG-INFO
--rw-rw-rw-   0        0        0     3611 2023-10-13 10:30:32.000000 name_matching-0.8.8/README.md
-drwxrwxrwx   0        0        0        0 2023-10-15 14:56:15.180803 name_matching-0.8.8/distances/
--rw-rw-rw-   0        0        0     2271 2022-06-22 17:40:35.000000 name_matching-0.8.8/distances/__init__.py
--rw-rw-rw-   0        0        0     4980 2022-06-22 17:41:11.000000 name_matching-0.8.8/distances/_bag.py
--rw-rw-rw-   0        0        0     4530 2022-06-22 17:41:21.000000 name_matching-0.8.8/distances/_baulieu_xiii.py
--rw-rw-rw-   0        0        0     2428 2022-06-22 17:41:26.000000 name_matching-0.8.8/distances/_character.py
--rw-rw-rw-   0        0        0     4649 2022-06-22 17:41:31.000000 name_matching-0.8.8/distances/_clement.py
--rw-rw-rw-   0        0        0     3215 2022-06-22 11:33:51.000000 name_matching-0.8.8/distances/_cormode_lz.py
--rw-rw-rw-   0        0        0     7982 2022-06-22 11:33:51.000000 name_matching-0.8.8/distances/_damerau_levenshtein.py
--rw-rw-rw-   0        0        0     3982 2022-06-22 17:41:40.000000 name_matching-0.8.8/distances/_dice_asymmetric_i.py
--rw-rw-rw-   0        0        0    12069 2022-06-22 11:33:52.000000 name_matching-0.8.8/distances/_discounted_levenshtein.py
--rw-rw-rw-   0        0        0     2823 2022-06-22 17:24:35.000000 name_matching-0.8.8/distances/_distance.py
--rw-rw-rw-   0        0        0    36197 2022-06-22 11:34:04.000000 name_matching-0.8.8/distances/_double_metaphone.py
--rw-rw-rw-   0        0        0     8921 2022-06-22 11:33:52.000000 name_matching-0.8.8/distances/_editex.py
--rw-rw-rw-   0        0        0     2552 2022-06-22 11:33:53.000000 name_matching-0.8.8/distances/_fuzzywuzzy_partial_string.py
--rw-rw-rw-   0        0        0     3740 2022-06-22 17:42:02.000000 name_matching-0.8.8/distances/_fuzzywuzzy_token_set.py
--rw-rw-rw-   0        0        0     3398 2022-06-22 17:42:14.000000 name_matching-0.8.8/distances/_fuzzywuzzy_token_sort.py
--rw-rw-rw-   0        0        0     4766 2022-06-22 11:33:54.000000 name_matching-0.8.8/distances/_hamming.py
--rw-rw-rw-   0        0        0     2398 2022-06-22 11:33:54.000000 name_matching-0.8.8/distances/_indel.py
--rw-rw-rw-   0        0        0     5962 2022-06-22 11:33:54.000000 name_matching-0.8.8/distances/_iterative_substring.py
--rw-rw-rw-   0        0        0     6008 2022-06-22 17:42:24.000000 name_matching-0.8.8/distances/_kuhns_iii.py
--rw-rw-rw-   0        0        0     4129 2022-06-22 11:33:56.000000 name_matching-0.8.8/distances/_lcprefix.py
--rw-rw-rw-   0        0        0     5137 2022-06-22 11:33:56.000000 name_matching-0.8.8/distances/_lcsseq.py
--rw-rw-rw-   0        0        0    12646 2022-06-22 11:33:56.000000 name_matching-0.8.8/distances/_levenshtein.py
--rw-rw-rw-   0        0        0     2424 2022-06-22 11:33:56.000000 name_matching-0.8.8/distances/_lig3.py
--rw-rw-rw-   0        0        0     2862 2022-06-22 11:33:57.000000 name_matching-0.8.8/distances/_ncd_bz2.py
--rw-rw-rw-   0        0        0     3910 2022-06-22 17:42:41.000000 name_matching-0.8.8/distances/_overlap.py
--rw-rw-rw-   0        0        0     6920 2022-06-22 17:42:46.000000 name_matching-0.8.8/distances/_pearson_chi_squared.py
--rw-rw-rw-   0        0        0     5449 2022-06-22 17:42:51.000000 name_matching-0.8.8/distances/_pearson_ii.py
--rw-rw-rw-   0        0        0     2623 2022-06-22 11:34:05.000000 name_matching-0.8.8/distances/_phonetic.py
--rw-rw-rw-   0        0        0     7528 2022-12-01 06:55:53.000000 name_matching-0.8.8/distances/_phonetic_distance.py
--rw-rw-rw-   0        0        0     7175 2022-06-22 17:39:16.000000 name_matching-0.8.8/distances/_q_grams.py
--rw-rw-rw-   0        0        0     8571 2022-06-22 17:39:17.000000 name_matching-0.8.8/distances/_q_skipgrams.py
--rw-rw-rw-   0        0        0     5341 2022-06-22 11:33:59.000000 name_matching-0.8.8/distances/_ratcliff_obershelp.py
--rw-rw-rw-   0        0        0     4042 2022-06-22 11:34:06.000000 name_matching-0.8.8/distances/_refined_soundex.py
--rw-rw-rw-   0        0        0     3256 2022-06-22 17:43:20.000000 name_matching-0.8.8/distances/_regexp.py
--rw-rw-rw-   0        0        0     2540 2022-06-22 13:25:07.000000 name_matching-0.8.8/distances/_rouge_l.py
--rw-rw-rw-   0        0        0     4905 2022-06-22 17:43:52.000000 name_matching-0.8.8/distances/_ssk.py
--rw-rw-rw-   0        0        0     5336 2022-06-22 11:34:01.000000 name_matching-0.8.8/distances/_tichy.py
--rw-rw-rw-   0        0        0    39254 2022-12-01 06:55:53.000000 name_matching-0.8.8/distances/_token_distance.py
--rw-rw-rw-   0        0        0     7897 2022-06-22 17:39:30.000000 name_matching-0.8.8/distances/_tokenizer.py
--rw-rw-rw-   0        0        0    13854 2022-06-22 11:34:01.000000 name_matching-0.8.8/distances/_typo.py
--rw-rw-rw-   0        0        0     4523 2022-06-22 17:44:55.000000 name_matching-0.8.8/distances/_warrens_iv.py
--rw-rw-rw-   0        0        0     4346 2022-06-22 17:45:01.000000 name_matching-0.8.8/distances/_weighted_jaccard.py
--rw-rw-rw-   0        0        0     2572 2022-06-22 17:45:19.000000 name_matching-0.8.8/distances/_whitespace.py
-drwxrwxrwx   0        0        0        0 2023-10-15 14:56:15.202123 name_matching-0.8.8/name_matching/
--rw-rw-rw-   0        0        0        0 2022-06-22 14:59:21.000000 name_matching-0.8.8/name_matching/__init__.py
--rw-rw-rw-   0        0        0    12133 2023-03-21 08:32:24.000000 name_matching-0.8.8/name_matching/distance_metrics.py
--rw-rw-rw-   0        0        0    32223 2023-10-15 14:46:34.000000 name_matching-0.8.8/name_matching/name_matcher.py
--rw-rw-rw-   0        0        0    14942 2023-03-22 16:29:57.000000 name_matching-0.8.8/name_matching/run_nm.py
--rw-rw-rw-   0        0        0     6087 2022-06-22 14:06:42.000000 name_matching-0.8.8/name_matching/sparse_cosine.py
-drwxrwxrwx   0        0        0        0 2023-10-15 14:56:15.225125 name_matching-0.8.8/name_matching.egg-info/
--rw-rw-rw-   0        0        0     4035 2023-10-15 14:56:13.000000 name_matching-0.8.8/name_matching.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1476 2023-10-15 14:56:14.000000 name_matching-0.8.8/name_matching.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-15 14:56:13.000000 name_matching-0.8.8/name_matching.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-10-15 14:56:14.000000 name_matching-0.8.8/name_matching.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-10-15 14:56:14.000000 name_matching-0.8.8/name_matching.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-10-15 14:56:15.235618 name_matching-0.8.8/setup.cfg
--rw-rw-rw-   0        0        0      819 2023-10-15 11:53:55.000000 name_matching-0.8.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-11-03 12:38:51.478078 name_matching-0.8.9/
+-rw-rw-rw-   0        0        0     4035 2023-11-03 12:38:51.479081 name_matching-0.8.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3522 2023-10-26 06:40:10.000000 name_matching-0.8.9/README.md
+drwxrwxrwx   0        0        0        0 2023-11-03 12:38:51.286083 name_matching-0.8.9/distances/
+-rw-rw-rw-   0        0        0     2271 2023-10-26 06:40:10.000000 name_matching-0.8.9/distances/__init__.py
+-rw-rw-rw-   0        0        0     4980 2023-10-26 06:40:10.000000 name_matching-0.8.9/distances/_bag.py
+-rw-rw-rw-   0        0        0     4530 2023-10-26 06:40:10.000000 name_matching-0.8.9/distances/_baulieu_xiii.py
+-rw-rw-rw-   0        0        0     2428 2023-10-26 06:40:10.000000 name_matching-0.8.9/distances/_character.py
+-rw-rw-rw-   0        0        0     4649 2023-10-26 06:40:10.000000 name_matching-0.8.9/distances/_clement.py
+-rw-rw-rw-   0        0        0     3215 2023-10-26 06:40:10.000000 name_matching-0.8.9/distances/_cormode_lz.py
+-rw-rw-rw-   0        0        0     7982 2023-10-26 06:40:10.000000 name_matching-0.8.9/distances/_damerau_levenshtein.py
+-rw-rw-rw-   0        0        0     3982 2023-10-26 06:40:10.000000 name_matching-0.8.9/distances/_dice_asymmetric_i.py
+-rw-rw-rw-   0        0        0    12069 2023-10-26 06:40:10.000000 name_matching-0.8.9/distances/_discounted_levenshtein.py
+-rw-rw-rw-   0        0        0     2823 2023-10-26 06:40:10.000000 name_matching-0.8.9/distances/_distance.py
+-rw-rw-rw-   0        0        0    36197 2023-10-26 06:40:10.000000 name_matching-0.8.9/distances/_double_metaphone.py
+-rw-rw-rw-   0        0        0     8921 2023-10-26 06:40:10.000000 name_matching-0.8.9/distances/_editex.py
+-rw-rw-rw-   0        0        0     2552 2023-10-26 06:40:10.000000 name_matching-0.8.9/distances/_fuzzywuzzy_partial_string.py
+-rw-rw-rw-   0        0        0     3740 2023-10-26 06:40:10.000000 name_matching-0.8.9/distances/_fuzzywuzzy_token_set.py
+-rw-rw-rw-   0        0        0     3398 2023-10-26 06:40:10.000000 name_matching-0.8.9/distances/_fuzzywuzzy_token_sort.py
+-rw-rw-rw-   0        0        0     4766 2023-10-26 06:40:10.000000 name_matching-0.8.9/distances/_hamming.py
+-rw-rw-rw-   0        0        0     2398 2023-10-26 06:40:10.000000 name_matching-0.8.9/distances/_indel.py
+-rw-rw-rw-   0        0        0     5962 2023-10-26 06:40:10.000000 name_matching-0.8.9/distances/_iterative_substring.py
+-rw-rw-rw-   0        0        0     6008 2023-10-26 06:40:12.000000 name_matching-0.8.9/distances/_kuhns_iii.py
+-rw-rw-rw-   0        0        0     4129 2023-10-26 06:40:12.000000 name_matching-0.8.9/distances/_lcprefix.py
+-rw-rw-rw-   0        0        0     5137 2023-10-26 06:40:12.000000 name_matching-0.8.9/distances/_lcsseq.py
+-rw-rw-rw-   0        0        0    12646 2023-10-26 06:40:12.000000 name_matching-0.8.9/distances/_levenshtein.py
+-rw-rw-rw-   0        0        0     2424 2023-10-26 06:40:12.000000 name_matching-0.8.9/distances/_lig3.py
+-rw-rw-rw-   0        0        0     2862 2023-10-26 06:40:12.000000 name_matching-0.8.9/distances/_ncd_bz2.py
+-rw-rw-rw-   0        0        0     3910 2023-10-26 06:40:12.000000 name_matching-0.8.9/distances/_overlap.py
+-rw-rw-rw-   0        0        0     6920 2023-10-26 06:40:12.000000 name_matching-0.8.9/distances/_pearson_chi_squared.py
+-rw-rw-rw-   0        0        0     5449 2023-10-26 06:40:12.000000 name_matching-0.8.9/distances/_pearson_ii.py
+-rw-rw-rw-   0        0        0     2623 2023-10-26 06:40:12.000000 name_matching-0.8.9/distances/_phonetic.py
+-rw-rw-rw-   0        0        0     7287 2023-10-26 06:40:12.000000 name_matching-0.8.9/distances/_phonetic_distance.py
+-rw-rw-rw-   0        0        0     7175 2023-10-26 06:40:12.000000 name_matching-0.8.9/distances/_q_grams.py
+-rw-rw-rw-   0        0        0     8571 2023-10-26 06:40:12.000000 name_matching-0.8.9/distances/_q_skipgrams.py
+-rw-rw-rw-   0        0        0     5341 2023-10-26 06:40:12.000000 name_matching-0.8.9/distances/_ratcliff_obershelp.py
+-rw-rw-rw-   0        0        0     4042 2023-10-26 06:40:12.000000 name_matching-0.8.9/distances/_refined_soundex.py
+-rw-rw-rw-   0        0        0     3256 2023-10-26 06:40:12.000000 name_matching-0.8.9/distances/_regexp.py
+-rw-rw-rw-   0        0        0     2540 2023-10-26 06:40:12.000000 name_matching-0.8.9/distances/_rouge_l.py
+-rw-rw-rw-   0        0        0     4905 2023-10-26 06:40:12.000000 name_matching-0.8.9/distances/_ssk.py
+-rw-rw-rw-   0        0        0     5336 2023-10-26 06:40:12.000000 name_matching-0.8.9/distances/_tichy.py
+-rw-rw-rw-   0        0        0    38265 2023-10-26 06:40:12.000000 name_matching-0.8.9/distances/_token_distance.py
+-rw-rw-rw-   0        0        0     7897 2023-10-26 06:40:12.000000 name_matching-0.8.9/distances/_tokenizer.py
+-rw-rw-rw-   0        0        0    13854 2023-10-26 06:40:12.000000 name_matching-0.8.9/distances/_typo.py
+-rw-rw-rw-   0        0        0     4523 2023-10-26 06:40:12.000000 name_matching-0.8.9/distances/_warrens_iv.py
+-rw-rw-rw-   0        0        0     4346 2023-10-26 06:40:12.000000 name_matching-0.8.9/distances/_weighted_jaccard.py
+-rw-rw-rw-   0        0        0     2572 2023-10-26 06:40:12.000000 name_matching-0.8.9/distances/_whitespace.py
+drwxrwxrwx   0        0        0        0 2023-11-03 12:38:51.362082 name_matching-0.8.9/name_matching/
+-rw-rw-rw-   0        0        0        0 2023-10-26 06:40:16.000000 name_matching-0.8.9/name_matching/__init__.py
+-rw-rw-rw-   0        0        0    11867 2023-10-26 06:40:16.000000 name_matching-0.8.9/name_matching/distance_metrics.py
+-rw-rw-rw-   0        0        0    31343 2023-10-26 08:06:56.000000 name_matching-0.8.9/name_matching/name_matcher.py
+-rw-rw-rw-   0        0        0    14632 2023-10-26 06:40:16.000000 name_matching-0.8.9/name_matching/run_nm.py
+-rw-rw-rw-   0        0        0     5934 2023-10-26 06:40:16.000000 name_matching-0.8.9/name_matching/sparse_cosine.py
+drwxrwxrwx   0        0        0        0 2023-11-03 12:38:51.450083 name_matching-0.8.9/name_matching.egg-info/
+-rw-rw-rw-   0        0        0     4035 2023-11-03 12:38:49.000000 name_matching-0.8.9/name_matching.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1476 2023-11-03 12:38:50.000000 name_matching-0.8.9/name_matching.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-03 12:38:49.000000 name_matching-0.8.9/name_matching.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-11-03 12:38:49.000000 name_matching-0.8.9/name_matching.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-11-03 12:38:49.000000 name_matching-0.8.9/name_matching.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-11-03 12:38:51.487078 name_matching-0.8.9/setup.cfg
+-rw-rw-rw-   0        0        0      794 2023-10-26 08:10:44.000000 name_matching-0.8.9/setup.py
```

### Comparing `name_matching-0.8.8/PKG-INFO` & `name_matching-0.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: name_matching
-Version: 0.8.8
+Version: 0.8.9
 Summary: A package for the matching of company names
 Author: Michiel Nijhuis
 Author-email: m.nijhuis@dnb.nl
 License: UNKNOWN
 Project-URL: Documentation, https://name-matching.readthedocs.io/en/latest/index.html
 Project-URL: Source Code, https://github.com/DeNederlandscheBank/name_matching
 Platform: UNKNOWN
```

### Comparing `name_matching-0.8.8/README.md` & `name_matching-0.8.9/name_matching.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: name-matching
+Version: 0.8.9
+Summary: A package for the matching of company names
+Author: Michiel Nijhuis
+Author-email: m.nijhuis@dnb.nl
+License: UNKNOWN
+Project-URL: Documentation, https://name-matching.readthedocs.io/en/latest/index.html
+Project-URL: Source Code, https://github.com/DeNederlandscheBank/name_matching
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
 [![name_matching](https://github.com/DeNederlandscheBank/name_matching/actions/workflows/python-app.yml/badge.svg?branch=main)](https://github.com/DeNederlandscheBank/name_matching/actions/workflows/python-app.yml)
 
 # Name matching
 
 Name matching is a Python package for the matching of company names. This package has been developed to match the names of companies from different databases together to allow them to be merged. The package has a number of options to determine how exact the matches should be and also for the selection of different name matching algorithms.
 
 For a more in-depth discussion of the name matching package please see the [company name matching](https://medium.com/dnb-data-science-hub/company-name-matching-6a6330710334) medium post
@@ -35,15 +47,15 @@
         'Agricultural Bank of China',
         'Bank of China',
         'JPMorgan Chase',
         'Mitsubishi UFJ Financial Group',
         'Bank of America',
         'HSBC',
         'BNP Paribas',
-        'Crédit Agricole']})
+        'CrÃ©dit Agricole']})
 
 # alter each of the bank names a bit to test the matching
 df_companies_b = pd.DataFrame({'name': [
         'Bank of China Limited',
         'Mitsubishi Financial Group',
         'Construction Bank China',
         'Agricultural Bank',
@@ -83,7 +95,9 @@
 All contributions are welcome. For more substantial changes, please open an issue first to discuss what you would like to change.
 
 ## License
 The code is licensed under the MIT/X license an extended version of the licence: [MIT](https://choosealicense.com/licenses/mit/)
 
 ## Thanks
 Thanks to the work of implementing name matching algorithms done in the [Abydos package](https://github.com/chrislit/abydos). These form the basis of the name matching algorithms used in this package.
+
+
```

### Comparing `name_matching-0.8.8/distances/__init__.py` & `name_matching-0.8.9/distances/__init__.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_bag.py` & `name_matching-0.8.9/distances/_bag.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_baulieu_xiii.py` & `name_matching-0.8.9/distances/_baulieu_xiii.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_character.py` & `name_matching-0.8.9/distances/_character.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_clement.py` & `name_matching-0.8.9/distances/_clement.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_cormode_lz.py` & `name_matching-0.8.9/distances/_cormode_lz.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_damerau_levenshtein.py` & `name_matching-0.8.9/distances/_damerau_levenshtein.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_dice_asymmetric_i.py` & `name_matching-0.8.9/distances/_dice_asymmetric_i.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_discounted_levenshtein.py` & `name_matching-0.8.9/distances/_discounted_levenshtein.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_distance.py` & `name_matching-0.8.9/distances/_distance.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_double_metaphone.py` & `name_matching-0.8.9/distances/_double_metaphone.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_editex.py` & `name_matching-0.8.9/distances/_editex.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_fuzzywuzzy_partial_string.py` & `name_matching-0.8.9/distances/_fuzzywuzzy_partial_string.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_fuzzywuzzy_token_set.py` & `name_matching-0.8.9/distances/_fuzzywuzzy_token_set.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_fuzzywuzzy_token_sort.py` & `name_matching-0.8.9/distances/_fuzzywuzzy_token_sort.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_hamming.py` & `name_matching-0.8.9/distances/_hamming.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_indel.py` & `name_matching-0.8.9/distances/_indel.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_iterative_substring.py` & `name_matching-0.8.9/distances/_iterative_substring.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_kuhns_iii.py` & `name_matching-0.8.9/distances/_kuhns_iii.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_lcprefix.py` & `name_matching-0.8.9/distances/_lcprefix.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_lcsseq.py` & `name_matching-0.8.9/distances/_lcsseq.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_levenshtein.py` & `name_matching-0.8.9/distances/_levenshtein.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_lig3.py` & `name_matching-0.8.9/distances/_lig3.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_ncd_bz2.py` & `name_matching-0.8.9/distances/_ncd_bz2.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_overlap.py` & `name_matching-0.8.9/distances/_overlap.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_pearson_chi_squared.py` & `name_matching-0.8.9/distances/_pearson_chi_squared.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_pearson_ii.py` & `name_matching-0.8.9/distances/_pearson_ii.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_phonetic.py` & `name_matching-0.8.9/distances/_phonetic.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_phonetic_distance.py` & `name_matching-0.8.9/distances/_phonetic_distance.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,241 +1,241 @@
-# Copyright 2019-2020 by Christopher C. Little.
-# This file is part of Abydos.
-#
-# Abydos is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# Abydos is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with Abydos. If not, see <http://www.gnu.org/licenses/>.
-
-"""abydos.distance._phonetic_distance.
-
-Phonetic distance.
-"""
-
-from typing import Any, Callable, List, Optional, Sequence, Type, Union
-
-from ._distance import _Distance
-from ._phonetic import _Phonetic
-
-__all__ = ['PhoneticDistance']
-
-
-class PhoneticDistance(_Distance):
-    """Phonetic distance.
-
-    Phonetic distance applies one or more supplied string transformations to
-    words and compares the resulting transformed strings using a supplied
-    distance measure.
-
-    A simple example would be to create a 'Soundex distance':
-
-    >>> from abydos.phonetic import Soundex
-    >>> soundex = PhoneticDistance(transforms=Soundex())
-    >>> soundex.dist('Ashcraft', 'Ashcroft')
-    0.0
-    >>> soundex.dist('Robert', 'Ashcraft')
-    1.0
-
-    .. versionadded:: 0.4.1
-    """
-
-    def __init__(
-        self,
-        transforms: Optional[
-            Union[
-                Type[_Phonetic],
-                _Phonetic,
-                Callable[[str], str],
-                Sequence[
-                    Union[
-                        Type[_Phonetic],
-                        _Phonetic,
-                        Callable[[str], str],
-                    ]
-                ],
-            ]
-        ] = None,
-        metric: Optional[Union[Type[_Distance], _Distance]] = None,
-        encode_alpha: bool = False,
-        **kwargs: Any
-    ) -> None:
-        """Initialize PhoneticDistance instance.
-
-        Parameters
-        ----------
-        transforms : list or _Phonetic or _Stemmer or _Fingerprint or type
-            An instance of a subclass of _Phonetic, _Stemmer, or _Fingerprint,
-            or a list (or other iterable) of such instances to apply to each
-            input word before computing their distance or similarity. If
-            omitted, no transformations will be performed.
-        metric : _Distance or type
-            An instance of a subclass of _Distance, used for computing the
-            inputs' distance or similarity after being transformed. If omitted,
-            the strings will be compared for identify (returning 0.0 if
-            identical, otherwise 1.0, when distance is computed).
-        encode_alpha : bool
-            Set to true to use the encode_alpha method of phonetic algorithms
-            whenever possible.
-        **kwargs
-            Arbitrary keyword arguments
-
-
-        .. versionadded:: 0.4.1
-
-        """
-        super(PhoneticDistance, self).__init__(**kwargs)
-        self.transforms = []  # type: List[Callable[[str], str]]
-        if transforms:
-            if isinstance(transforms, Sequence):
-                transforms = list(transforms)
-            else:
-                transforms = [transforms]
-
-            for i, trans in enumerate(transforms):
-                if isinstance(trans, (_Phonetic)):
-                    continue
-                elif isinstance(trans, type) and issubclass(
-                    trans, (_Phonetic)
-                ):
-                    transforms[i] = trans()
-                elif callable(trans):
-                    continue
-                else:
-                    raise TypeError(
-                        '{} has unknown type {}'.format(trans, type(trans))
-                    )
-
-            for trans in transforms:
-                if isinstance(trans, _Phonetic):
-                    if encode_alpha:
-                        self.transforms.append(trans.encode_alpha)
-                    else:
-                        self.transforms.append(trans.encode)
-                else:  # callable(trans)
-                    self.transforms.append(trans)  # type: ignore
-
-        if isinstance(metric, type) and issubclass(metric, _Distance):
-            self.metric = metric()  # type: Optional[_Distance]
-        elif isinstance(metric, _Distance):
-            self.metric = metric
-        elif metric is None:
-            self.metric = None
-        else:
-            raise TypeError(
-                '{} has unknown type {}'.format(metric, type(metric))
-            )
-
-    def dist_abs(self, src: str, tar: str) -> float:
-        """Return the Phonetic distance.
-
-        Parameters
-        ----------
-        src : str
-            Source string for comparison
-        tar : str
-            Target string for comparison
-
-        Returns
-        -------
-        float or int
-            The Phonetic distance
-
-        Examples
-        --------
-        >>> from abydos.phonetic import Soundex
-        >>> cmp = PhoneticDistance(Soundex())
-        >>> cmp.dist_abs('cat', 'hat')
-        1
-        >>> cmp.dist_abs('Niall', 'Neil')
-        0
-        >>> cmp.dist_abs('Colin', 'Cuilen')
-        0
-        >>> cmp.dist_abs('ATCG', 'TAGC')
-        1
-
-        >>> from abydos.distance import Levenshtein
-        >>> cmp = PhoneticDistance(transforms=[Soundex], metric=Levenshtein)
-        >>> cmp.dist_abs('cat', 'hat')
-        1
-        >>> cmp.dist_abs('Niall', 'Neil')
-        0
-        >>> cmp.dist_abs('Colin', 'Cuilen')
-        0
-        >>> cmp.dist_abs('ATCG', 'TAGC')
-        3
-
-
-        .. versionadded:: 0.4.1
-
-        """
-        for trans in self.transforms:
-            src = trans(src)
-            tar = trans(tar)
-        if self.metric:
-            return self.metric.dist_abs(src, tar)
-        else:
-            return int(src != tar)
-
-    def dist(self, src: str, tar: str) -> float:
-        """Return the normalized Phonetic distance.
-
-        Parameters
-        ----------
-        src : str
-            Source string for comparison
-        tar : str
-            Target string for comparison
-
-        Returns
-        -------
-        float
-            The normalized Phonetic distance
-
-        Examples
-        --------
-        >>> from abydos.phonetic import Soundex
-        >>> cmp = PhoneticDistance(Soundex())
-        >>> cmp.dist('cat', 'hat')
-        1.0
-        >>> cmp.dist('Niall', 'Neil')
-        0.0
-        >>> cmp.dist('Colin', 'Cuilen')
-        0.0
-        >>> cmp.dist('ATCG', 'TAGC')
-        1.0
-
-        >>> from abydos.distance import Levenshtein
-        >>> cmp = PhoneticDistance(transforms=[Soundex], metric=Levenshtein)
-        >>> cmp.dist('cat', 'hat')
-        0.25
-        >>> cmp.dist('Niall', 'Neil')
-        0.0
-        >>> cmp.dist('Colin', 'Cuilen')
-        0.0
-        >>> cmp.dist('ATCG', 'TAGC')
-        0.75
-
-
-        .. versionadded:: 0.4.1
-
-        """
-        for trans in self.transforms:
-            src = trans(src)
-            tar = trans(tar)
-        if self.metric:
-            return self.metric.dist(src, tar)
-        else:
-            return float(src != tar)
-
-
-if __name__ == '__main__':
-    import doctest
-
-    doctest.testmod()
+# Copyright 2019-2020 by Christopher C. Little.
+# This file is part of Abydos.
+#
+# Abydos is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# Abydos is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with Abydos. If not, see <http://www.gnu.org/licenses/>.
+
+"""abydos.distance._phonetic_distance.
+
+Phonetic distance.
+"""
+
+from typing import Any, Callable, List, Optional, Sequence, Type, Union
+
+from ._distance import _Distance
+from ._phonetic import _Phonetic
+
+__all__ = ['PhoneticDistance']
+
+
+class PhoneticDistance(_Distance):
+    """Phonetic distance.
+
+    Phonetic distance applies one or more supplied string transformations to
+    words and compares the resulting transformed strings using a supplied
+    distance measure.
+
+    A simple example would be to create a 'Soundex distance':
+
+    >>> from abydos.phonetic import Soundex
+    >>> soundex = PhoneticDistance(transforms=Soundex())
+    >>> soundex.dist('Ashcraft', 'Ashcroft')
+    0.0
+    >>> soundex.dist('Robert', 'Ashcraft')
+    1.0
+
+    .. versionadded:: 0.4.1
+    """
+
+    def __init__(
+        self,
+        transforms: Optional[
+            Union[
+                Type[_Phonetic],
+                _Phonetic,
+                Callable[[str], str],
+                Sequence[
+                    Union[
+                        Type[_Phonetic],
+                        _Phonetic,
+                        Callable[[str], str],
+                    ]
+                ],
+            ]
+        ] = None,
+        metric: Optional[Union[Type[_Distance], _Distance]] = None,
+        encode_alpha: bool = False,
+        **kwargs: Any
+    ) -> None:
+        """Initialize PhoneticDistance instance.
+
+        Parameters
+        ----------
+        transforms : list or _Phonetic or _Stemmer or _Fingerprint or type
+            An instance of a subclass of _Phonetic, _Stemmer, or _Fingerprint,
+            or a list (or other iterable) of such instances to apply to each
+            input word before computing their distance or similarity. If
+            omitted, no transformations will be performed.
+        metric : _Distance or type
+            An instance of a subclass of _Distance, used for computing the
+            inputs' distance or similarity after being transformed. If omitted,
+            the strings will be compared for identify (returning 0.0 if
+            identical, otherwise 1.0, when distance is computed).
+        encode_alpha : bool
+            Set to true to use the encode_alpha method of phonetic algorithms
+            whenever possible.
+        **kwargs
+            Arbitrary keyword arguments
+
+
+        .. versionadded:: 0.4.1
+
+        """
+        super(PhoneticDistance, self).__init__(**kwargs)
+        self.transforms = []  # type: List[Callable[[str], str]]
+        if transforms:
+            if isinstance(transforms, Sequence):
+                transforms = list(transforms)
+            else:
+                transforms = [transforms]
+
+            for i, trans in enumerate(transforms):
+                if isinstance(trans, (_Phonetic)):
+                    continue
+                elif isinstance(trans, type) and issubclass(
+                    trans, (_Phonetic)
+                ):
+                    transforms[i] = trans()
+                elif callable(trans):
+                    continue
+                else:
+                    raise TypeError(
+                        '{} has unknown type {}'.format(trans, type(trans))
+                    )
+
+            for trans in transforms:
+                if isinstance(trans, _Phonetic):
+                    if encode_alpha:
+                        self.transforms.append(trans.encode_alpha)
+                    else:
+                        self.transforms.append(trans.encode)
+                else:  # callable(trans)
+                    self.transforms.append(trans)  # type: ignore
+
+        if isinstance(metric, type) and issubclass(metric, _Distance):
+            self.metric = metric()  # type: Optional[_Distance]
+        elif isinstance(metric, _Distance):
+            self.metric = metric
+        elif metric is None:
+            self.metric = None
+        else:
+            raise TypeError(
+                '{} has unknown type {}'.format(metric, type(metric))
+            )
+
+    def dist_abs(self, src: str, tar: str) -> float:
+        """Return the Phonetic distance.
+
+        Parameters
+        ----------
+        src : str
+            Source string for comparison
+        tar : str
+            Target string for comparison
+
+        Returns
+        -------
+        float or int
+            The Phonetic distance
+
+        Examples
+        --------
+        >>> from abydos.phonetic import Soundex
+        >>> cmp = PhoneticDistance(Soundex())
+        >>> cmp.dist_abs('cat', 'hat')
+        1
+        >>> cmp.dist_abs('Niall', 'Neil')
+        0
+        >>> cmp.dist_abs('Colin', 'Cuilen')
+        0
+        >>> cmp.dist_abs('ATCG', 'TAGC')
+        1
+
+        >>> from abydos.distance import Levenshtein
+        >>> cmp = PhoneticDistance(transforms=[Soundex], metric=Levenshtein)
+        >>> cmp.dist_abs('cat', 'hat')
+        1
+        >>> cmp.dist_abs('Niall', 'Neil')
+        0
+        >>> cmp.dist_abs('Colin', 'Cuilen')
+        0
+        >>> cmp.dist_abs('ATCG', 'TAGC')
+        3
+
+
+        .. versionadded:: 0.4.1
+
+        """
+        for trans in self.transforms:
+            src = trans(src)
+            tar = trans(tar)
+        if self.metric:
+            return self.metric.dist_abs(src, tar)
+        else:
+            return int(src != tar)
+
+    def dist(self, src: str, tar: str) -> float:
+        """Return the normalized Phonetic distance.
+
+        Parameters
+        ----------
+        src : str
+            Source string for comparison
+        tar : str
+            Target string for comparison
+
+        Returns
+        -------
+        float
+            The normalized Phonetic distance
+
+        Examples
+        --------
+        >>> from abydos.phonetic import Soundex
+        >>> cmp = PhoneticDistance(Soundex())
+        >>> cmp.dist('cat', 'hat')
+        1.0
+        >>> cmp.dist('Niall', 'Neil')
+        0.0
+        >>> cmp.dist('Colin', 'Cuilen')
+        0.0
+        >>> cmp.dist('ATCG', 'TAGC')
+        1.0
+
+        >>> from abydos.distance import Levenshtein
+        >>> cmp = PhoneticDistance(transforms=[Soundex], metric=Levenshtein)
+        >>> cmp.dist('cat', 'hat')
+        0.25
+        >>> cmp.dist('Niall', 'Neil')
+        0.0
+        >>> cmp.dist('Colin', 'Cuilen')
+        0.0
+        >>> cmp.dist('ATCG', 'TAGC')
+        0.75
+
+
+        .. versionadded:: 0.4.1
+
+        """
+        for trans in self.transforms:
+            src = trans(src)
+            tar = trans(tar)
+        if self.metric:
+            return self.metric.dist(src, tar)
+        else:
+            return float(src != tar)
+
+
+if __name__ == '__main__':
+    import doctest
+
+    doctest.testmod()
```

### Comparing `name_matching-0.8.8/distances/_q_grams.py` & `name_matching-0.8.9/distances/_q_grams.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_q_skipgrams.py` & `name_matching-0.8.9/distances/_q_skipgrams.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_ratcliff_obershelp.py` & `name_matching-0.8.9/distances/_ratcliff_obershelp.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_refined_soundex.py` & `name_matching-0.8.9/distances/_refined_soundex.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_regexp.py` & `name_matching-0.8.9/distances/_regexp.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_rouge_l.py` & `name_matching-0.8.9/distances/_rouge_l.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_ssk.py` & `name_matching-0.8.9/distances/_ssk.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_tichy.py` & `name_matching-0.8.9/distances/_tichy.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_token_distance.py` & `name_matching-0.8.9/distances/_token_distance.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,989 +1,989 @@
-# Copyright 2018-2020 by Christopher C. Little.
-# This file is part of Abydos.
-#
-# Abydos is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# Abydos is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with Abydos. If not, see <http://www.gnu.org/licenses/>.
-
-"""abydos.distance._token_distance.
-
-The distance._token_distance._TokenDistance module implements abstract class
-_TokenDistance.
-"""
-
-from collections import Counter, OrderedDict
-from itertools import product
-from math import exp, log1p
-from typing import (
-    Any,
-    Callable,
-    Counter as TCounter,
-    Optional,
-    Tuple,
-    Union,
-    cast,
-)
-
-import numpy as np
-
-from ._damerau_levenshtein import DamerauLevenshtein
-from ._distance import _Distance
-from ._lcprefix import LCPrefix
-from ._levenshtein import Levenshtein
-from ._tokenizer import _Tokenizer
-from ._whitespace import WhitespaceTokenizer
-from ._q_grams import QGrams
-from ._q_skipgrams import QSkipgrams
-
-__all__ = ['_TokenDistance']
-
-
-class _TokenDistance(_Distance):
-    r"""Abstract Token Distance class.
-
-    .. _confusion_table:
-
-    +----------------+--------------+-----------------+-------+
-    |                | |in| ``tar`` | |notin| ``tar`` |       |
-    +----------------+--------------+-----------------+-------+
-    | |in| ``src``   | |a|          | |b|             | |a+b| |
-    +----------------+--------------+-----------------+-------+
-    | |notin| ``src``| |c|          | |d|             | |c+d| |
-    +----------------+--------------+-----------------+-------+
-    |                | |a+c|        | |b+d|           | |n|   |
-    +----------------+--------------+-----------------+-------+
-
-    .. |in| replace:: :math:`x \in`
-    .. |notin| replace:: :math:`x \notin`
-
-    .. |a| replace:: :math:`a = |X \cap Y|`
-    .. |b| replace:: :math:`b = |X\setminus Y|`
-    .. |c| replace:: :math:`c = |Y \setminus X|`
-    .. |d| replace:: :math:`d = |(N\setminus X)\setminus Y|`
-    .. |n| replace:: :math:`n = |N|`
-    .. |a+b| replace:: :math:`p_1 = a+b = |X|`
-    .. |a+c| replace:: :math:`p_2 = a+c = |Y|`
-    .. |c+d| replace:: :math:`q_1 = c+d = |N\setminus X|`
-    .. |b+d| replace:: :math:`q_2 = b+d = |N\setminus Y|`
-
-    .. versionadded:: 0.3.6
-    """
-
-    def __init__(
-        self,
-        tokenizer: Optional[_Tokenizer] = None,
-        intersection_type: str = 'crisp',
-        **kwargs: Any
-    ) -> None:
-        r"""Initialize _TokenDistance instance.
-
-        .. _intersection_type:
-
-        Parameters
-        ----------
-        tokenizer : _Tokenizer
-            A tokenizer instance from the :py:mod:`abydos.tokenizer` package
-        intersection_type : str
-            Specifies the intersection type, and set type as a result:
-
-                - 'crisp': Ordinary intersection, wherein items are entirely
-                  members or non-members of the intersection. (Default)
-                - ``fuzzy``: Fuzzy intersection, defined by :cite:`Wang:2014`,
-                  wherein items can be partially members of the intersection
-                  if their similarity meets or exceeds a threshold value. This
-                  also takes `metric` (by default :class:`Levenshtein()`) and
-                  `threshold` (by default 0.8) parameters.
-                - ``soft``: Soft intersection, defined by :cite:`Russ:2014`,
-                  wherein items can be partially members of the intersection
-                  depending on their similarity. This also takes a `metric`
-                  (by default :class:`DamerauLevenshtein()`) parameter.
-                - ``linkage``: Group linkage, defined by :cite:`On:2007`. Like
-                  the soft intersection, items can be partially members of the
-                  intersection, but the method of pairing similar members is
-                  somewhat more complex. See the cited paper for details. This
-                  also takes `metric`
-                  (by default :class:`DamerauLevenshtein()`) and `threshold`
-                  (by default 0.1) parameters.
-        **kwargs
-            Arbitrary keyword arguments
-
-
-        .. _alphabet:
-
-        Other Parameters
-        ----------------
-        qval : int
-            The length of each q-gram. Using this parameter and tokenizer=None
-            will cause the instance to use the QGram tokenizer with this
-            q value.
-        metric : _Distance
-            A string distance measure class for use in the ``soft`` and
-            ``fuzzy`` variants.
-        threshold : float
-            A threshold value, similarities above which are counted as
-            members of the intersection for the ``fuzzy`` variant.
-        alphabet : Counter, collection, int, or None
-            This represents the alphabet of possible tokens.
-
-                - If a Counter is supplied, it is used directly in computing
-                  the complement of the tokens in both sets.
-                - If a collection is supplied, it is converted to a Counter
-                  and used directly. In the case of a single string being
-                  supplied and the QGram tokenizer being used, the full
-                  alphabet is inferred (i.e.
-                  :math:`len(set(alphabet+QGrams.start\_stop))^{QGrams.qval}`
-                  is used as the cardinality of the full alphabet.
-                - If an int is supplied, it is used as the cardinality of the
-                  full alphabet.
-                - If None is supplied, the cardinality of the full alphabet
-                  is inferred if QGram of QSkipgrams tokenization is used (i.e.
-                  :math:`28^{QGrams.qval}` is used as the cardinality of the
-                  full alphabet or :math:`26` if QGrams.qval is 1, which
-                  assumes the strings are English language strings and only
-                  contain letters of a single case). Otherwise, the cardinality
-                  of the complement of the total will be 0.
-        normalizer : str
-            This represents the normalization applied to the values in the
-            2x2 contingency table prior to any of the cardinality (\*_card)
-            methods returning a value. By default, no normalization is applied,
-            but the following values are supported:
-
-                - ``proportional`` : :math:`\frac{x}{n}`, where n is the total
-                  population
-                - ``log`` : :math:`log(1+x)`
-                - ``exp`` : :math:`e^x`
-                - ``laplace`` : :math:`x+1`
-                - ``inverse`` : :math:`\frac{1}{x}`
-                - ``complement`` : :math:`n-x`, where n is the total population
-
-        .. versionadded:: 0.4.0
-
-        """
-        super(_TokenDistance, self).__init__(
-            intersection_type=intersection_type, **kwargs
-        )
-
-        qval = 2 if 'qval' not in self.params else self.params['qval']
-        self.params['tokenizer'] = (
-            tokenizer
-            if tokenizer is not None
-            else WhitespaceTokenizer()
-            if qval == 0
-            else QGrams(qval=qval, start_stop='$#', skip=0, scaler=None)
-        )
-
-        if hasattr(self.params['tokenizer'], 'qval'):
-            if isinstance(self.params['tokenizer'].qval, int):
-                qvals = [self.params['tokenizer'].qval]
-            else:
-                qvals = list(self.params['tokenizer'].qval)
-        else:
-            qvals = []
-
-        if 'alphabet' in self.params:
-            if isinstance(self.params['alphabet'], str):
-                alpha_set = set(self.params['alphabet'])
-                if isinstance(self.params['tokenizer'], (QGrams, QSkipgrams)):
-                    alpha_set |= set(self.params['tokenizer'].start_stop)
-                    self.params['alphabet'] = sum(
-                        len(alpha_set) ** qval for qval in qvals
-                    )
-            if hasattr(self.params['alphabet'], '__len__') and not isinstance(
-                self.params['alphabet'], Counter
-            ):
-                self.params['alphabet'] = len(self.params['alphabet'])
-            elif self.params['alphabet'] is None and isinstance(
-                self.params['tokenizer'], (QGrams, QSkipgrams)
-            ):
-                self.params['alphabet'] = sum(
-                    28 ** qval if qval > 1 else 26 for qval in qvals
-                )
-        else:
-            if isinstance(self.params['tokenizer'], (QGrams, QSkipgrams)):
-                self.params['alphabet'] = sum(
-                    28 ** qval if qval > 1 else 26 for qval in qvals
-                )
-            else:
-                self.params['alphabet'] = None
-
-        if intersection_type == 'soft':
-            if 'metric' not in self.params or self.params['metric'] is None:
-                self.params['metric'] = Levenshtein()
-            self._lcprefix = LCPrefix()
-            self._intersection = self._soft_intersection  # type: ignore
-        elif intersection_type == 'fuzzy':
-            if 'metric' not in self.params or self.params['metric'] is None:
-                self.params['metric'] = Levenshtein()
-            if 'threshold' not in self.params:
-                self.params['threshold'] = 0.8
-            self._intersection = self._fuzzy_intersection  # type: ignore
-        elif intersection_type == 'linkage':
-            if 'metric' not in self.params or self.params['metric'] is None:
-                self.params['metric'] = DamerauLevenshtein()
-            if 'threshold' not in self.params:
-                self.params['threshold'] = 0.1
-            self._intersection = (  # type: ignore
-                self._group_linkage_intersection
-            )
-        else:
-            self._intersection = self._crisp_intersection  # type: ignore
-
-        self._src_tokens = Counter()  # type: TCounter[str]
-        self._tar_tokens = Counter()  # type: TCounter[str]
-        self._population_card_value = 0  # type: float
-
-        # initialize normalizer
-        self.normalizer = (
-            self._norm_none
-        )  # type: Callable[[float, int, float], float]  # noqa: E501
-
-        self._norm_dict = {
-            'proportional': self._norm_proportional,
-            'log': self._norm_log,
-            'exp': self._norm_exp,
-            'laplace': self._norm_laplace,
-            'inverse': self._norm_inverse,
-            'complement': self._norm_complement,
-        }
-
-        # initialize values for soft intersection
-        self._soft_intersection_precalc = Counter()  # type: TCounter[str]
-        self._soft_src_only = Counter()  # type: TCounter[str]
-        self._soft_tar_only = Counter()  # type: TCounter[str]
-
-    @staticmethod
-    def _norm_none(x: float, _squares: int, _pop: float) -> float:
-        return x
-
-    @staticmethod
-    def _norm_proportional(x: float, _squares: int, pop: float) -> float:
-        return x / max(1, pop)
-
-    @staticmethod
-    def _norm_log(x: float, _squares: int, _pop: float) -> float:
-        return log1p(x)
-
-    @staticmethod
-    def _norm_exp(x: float, _squares: int, _pop: float) -> float:
-        return exp(x)
-
-    @staticmethod
-    def _norm_laplace(x: float, squares: int, _pop: float) -> float:
-        return x + squares
-
-    @staticmethod
-    def _norm_inverse(x: float, _squares: int, pop: float) -> float:
-        return 1 / x if x else pop
-
-    @staticmethod
-    def _norm_complement(x: float, _squares: int, pop: float) -> float:
-        return pop - x
-
-    def _tokenize(
-        self, src: Union[str, TCounter[str]], tar: Union[str, TCounter[str]]
-    ) -> '_TokenDistance':
-        """Return the Q-Grams in src & tar.
-
-        Parameters
-        ----------
-        src : str
-            Source string (or QGrams/Counter objects) for comparison
-        tar : str
-            Target string (or QGrams/Counter objects) for comparison
-
-        Returns
-        -------
-        tuple of Counters
-            Q-Grams
-
-        Examples
-        --------
-        >>> pe = _TokenDistance()
-        >>> pe._tokenize('AT', 'TT')._get_tokens()
-        (Counter({'$A': 1, 'AT': 1, 'T#': 1}),
-         Counter({'$T': 1, 'TT': 1, 'T#': 1}))
-
-
-        .. versionadded:: 0.1.0
-        .. versionchanged:: 0.3.6
-            Encapsulated in class
-
-        """
-        self._src_orig = src
-        self._tar_orig = tar
-
-        if isinstance(src, Counter):
-            self._src_tokens = src
-        else:
-            self._src_tokens = (
-                self.params['tokenizer'].tokenize(src).get_counter()
-            )
-        if isinstance(tar, Counter):
-            self._tar_tokens = tar
-        else:
-            self._tar_tokens = (
-                self.params['tokenizer'].tokenize(tar).get_counter()
-            )
-
-        self._population_card_value = self._calc_population_card()
-
-        # Set up the normalizer, a function of two variables:
-        # x is the value in the contingency table square(s)
-        # n is the number of squares that x represents
-        if (
-            'normalizer' in self.params
-            and self.params['normalizer'] in self._norm_dict
-        ):
-            self.normalizer = self._norm_dict[self.params['normalizer']]
-
-        # clear values for soft intersection
-        self._soft_intersection_precalc = Counter()
-        self._soft_src_only = Counter()
-        self._soft_tar_only = Counter()
-
-        return self
-
-    def _get_tokens(self) -> Tuple[TCounter[str], TCounter[str]]:
-        """Return the src and tar tokens as a tuple."""
-        return self._src_tokens, self._tar_tokens
-
-    def _src_card(self) -> float:
-        r"""Return the cardinality of the tokens in the source set."""
-        if self.params['intersection_type'] == 'soft':
-            if not len(self._soft_intersection_precalc):
-                self._intersection()
-            return self.normalizer(
-                sum(
-                    abs(val)
-                    for val in (
-                        self._soft_intersection_precalc + self._soft_src_only
-                    ).values()
-                ),
-                2,
-                self._population_card_value,
-            )
-        return self.normalizer(
-            sum(abs(val) for val in self._src_tokens.values()),
-            2,
-            self._population_card_value,
-        )
-
-    def _src_only(self) -> TCounter[str]:
-        r"""Return the src tokens minus the tar tokens.
-
-        For (multi-)sets S and T, this is :math:`S \setminus T`.
-        """
-        if self.params['intersection_type'] == 'soft':
-            if not len(self._soft_intersection_precalc):
-                self._intersection()
-            return self._soft_src_only
-        src_only = self._src_tokens - self._intersection()
-        if self.params['intersection_type'] != 'crisp':
-            src_only -= self._intersection() - self._crisp_intersection()
-        return src_only
-
-    def _src_only_card(self) -> float:
-        """Return the cardinality of the tokens only in the source set."""
-        return self.normalizer(
-            sum(abs(val) for val in self._src_only().values()),
-            1,
-            self._population_card_value,
-        )
-
-    def _tar_card(self) -> float:
-        r"""Return the cardinality of the tokens in the target set."""
-        if self.params['intersection_type'] == 'soft':
-            if not len(self._soft_intersection_precalc):
-                self._intersection()
-            return self.normalizer(
-                sum(
-                    abs(val)
-                    for val in (
-                        self._soft_intersection_precalc + self._soft_tar_only
-                    ).values()
-                ),
-                2,
-                self._population_card_value,
-            )
-        return self.normalizer(
-            sum(abs(val) for val in self._tar_tokens.values()),
-            2,
-            self._population_card_value,
-        )
-
-    def _tar_only(self) -> TCounter[str]:
-        r"""Return the tar tokens minus the src tokens.
-
-        For (multi-)sets S and T, this is :math:`T \setminus S`.
-        """
-        if self.params['intersection_type'] == 'soft':
-            if not len(self._soft_intersection_precalc):
-                self._intersection()
-            return self._soft_tar_only
-        tar_only = self._tar_tokens - self._intersection()
-        if self.params['intersection_type'] != 'crisp':
-            tar_only -= self._intersection() - self._crisp_intersection()
-        return tar_only
-
-    def _tar_only_card(self) -> float:
-        """Return the cardinality of the tokens only in the target set."""
-        return self.normalizer(
-            sum(abs(val) for val in self._tar_only().values()),
-            1,
-            self._population_card_value,
-        )
-
-    def _symmetric_difference(self) -> TCounter[str]:
-        r"""Return the symmetric difference of tokens from src and tar.
-
-        For (multi-)sets S and T, this is :math:`S \triangle T`.
-        """
-        return self._src_only() + self._tar_only()
-
-    def _symmetric_difference_card(self) -> float:
-        """Return the cardinality of the symmetric difference."""
-        return self.normalizer(
-            sum(abs(val) for val in self._symmetric_difference().values()),
-            2,
-            self._population_card_value,
-        )
-
-    def _total(self) -> TCounter[str]:
-        """Return the sum of the sets.
-
-        For (multi-)sets S and T, this is :math:`S + T`.
-
-        In the case of multisets, this counts values in the intersection
-        twice. In the case of sets, this is identical to the union.
-        """
-        if self.params['intersection_type'] == 'soft':
-            if not len(self._soft_intersection_precalc):
-                self._intersection()
-            return (
-                self._soft_tar_only
-                + self._soft_src_only
-                + self._soft_intersection_precalc
-                + self._soft_intersection_precalc
-            )
-        return self._src_tokens + self._tar_tokens
-
-    def _total_card(self) -> float:
-        """Return the cardinality of the complement of the total."""
-        return self.normalizer(
-            sum(abs(val) for val in self._total().values()),
-            3,
-            self._population_card_value,
-        )
-
-    def _total_complement_card(self) -> float:
-        """Return the cardinality of the complement of the total."""
-        if self.params['alphabet'] is None:
-            return self.normalizer(0, 1, self._population_card_value)
-        elif isinstance(self.params['alphabet'], Counter):
-            return self.normalizer(
-                max(
-                    0,
-                    sum(
-                        abs(val)
-                        for val in (
-                            self.params['alphabet'] - self._total()
-                        ).values()
-                    ),
-                ),
-                1,
-                self._population_card_value,
-            )
-        return self.normalizer(
-            max(0, self.params['alphabet'] - len(self._total().values())),
-            1,
-            self._population_card_value,
-        )
-
-    def _calc_population_card(self) -> float:
-        """Return the cardinality of the population."""
-        save_normalizer = self.normalizer
-        self.normalizer = self._norm_none
-        save_intersection = self.params['intersection_type']
-        self.params['intersection_type'] = 'crisp'
-        pop = self._total_card() + self._total_complement_card()
-        self.normalizer = save_normalizer
-        self.params['intersection_type'] = save_intersection
-        return pop
-
-    def _population_card(self) -> float:
-        """Return the cardinality of the population."""
-        return self.normalizer(
-            self._population_card_value, 4, self._population_card_value
-        )
-
-    def _population_unique_card(self) -> float:
-        """Return the cardinality of the population minus the intersection."""
-        return self.normalizer(
-            self._population_card_value - self._intersection_card(),
-            4,
-            self._population_card_value,
-        )
-
-    def _union(self) -> TCounter[str]:
-        r"""Return the union of tokens from src and tar.
-
-        For (multi-)sets S and T, this is :math:`S \cup T`.
-        """
-        if self.params['intersection_type'] == 'soft':
-            if not len(self._soft_intersection_precalc):
-                self._intersection()
-            return (
-                self._soft_tar_only
-                + self._soft_src_only
-                + self._soft_intersection_precalc
-            )
-        union = self._total() - self._intersection()
-        if self.params['intersection_type'] != 'crisp':
-            union -= self._intersection() - self._crisp_intersection()
-        return union
-
-    def _union_card(self) -> float:
-        """Return the cardinality of the union."""
-        return self.normalizer(
-            sum(abs(val) for val in self._union().values()),
-            3,
-            self._population_card_value,
-        )
-
-    def _difference(self) -> TCounter[str]:
-        """Return the difference of the tokens, supporting negative values."""
-        if self.params['intersection_type'] == 'soft':
-            if not len(self._soft_intersection_precalc):
-                self._intersection()
-            _src_copy = Counter(self._soft_src_only)
-            _src_copy.subtract(self._soft_tar_only)
-            return _src_copy
-        _src_copy = Counter(self._src_tokens)
-        _src_copy.subtract(self._tar_tokens)
-        return _src_copy
-
-    def _crisp_intersection(self) -> TCounter[str]:
-        r"""Return the intersection of tokens from src and tar.
-
-        For (multi-)sets S and T, this is :math:`S \cap T`.
-        """
-        return self._src_tokens & self._tar_tokens
-
-    def _soft_intersection(self) -> TCounter[str]:
-        """Return the soft source, target, & intersection tokens & weights.
-
-        This implements the soft intersection defined by :cite:`Russ:2014` in
-        a way that can reproduce the results in the paper.
-        """
-        if not hasattr(self.params['metric'], 'alignment'):
-            raise TypeError(
-                "Soft similarity requires a 'metric' with an alignment \
-member function, such as Levenshtein."
-            )
-
-        intersection = self._crisp_intersection()
-        src_only = self._src_tokens - self._tar_tokens
-        tar_only = self._tar_tokens - self._src_tokens
-
-        src_new = Counter()  # type: TCounter[str]
-        tar_new = Counter()  # type: TCounter[str]
-
-        def _membership(src: str, tar: str) -> float:
-            greater_length = max(len(src), len(tar))
-            return cast(
-                float,
-                max(
-                    greater_length - self.params['metric'].dist_abs(src, tar),
-                    self._lcprefix.dist_abs(src, tar),
-                )
-                / greater_length,
-            )
-
-        def _token_src_tar_int(
-            src: str, tar: str
-        ) -> Tuple[str, float, str, float, str, float]:
-            src_tok = []
-            tar_tok = []
-            int_tok = []
-
-            src_val = 0.0
-            tar_val = 0.0
-            int_val = 0.0
-
-            _cost, _src, _tar = self.params['metric'].alignment(src, tar)
-
-            for i in range(len(_src)):
-                if _src[i] == _tar[i]:
-                    src_tok.append('-')
-                    tar_tok.append('-')
-                    int_tok.append(_src[i])
-                    int_val += 1
-                else:
-                    src_tok.append(_src[i])
-                    if _src[i] != '-':
-                        src_val += 1
-                    tar_tok.append(_tar[i])
-                    if _tar[i] != '-':
-                        tar_val += 1
-                    int_tok.append('-')
-
-            src_val /= len(_src)
-            tar_val /= len(_src)
-            int_val /= len(_src)
-
-            src_tok_str = ''.join(src_tok).strip('-')
-            tar_tok_str = ''.join(tar_tok).strip('-')
-            int_tok_str = ''.join(int_tok).strip('-')
-
-            return (
-                src_tok_str,
-                src_val,
-                tar_tok_str,
-                tar_val,
-                int_tok_str,
-                int_val,
-            )
-
-        # Dictionary ordering is important for reproducibility, so insertion
-        # order needs to be controlled and retained.
-        memberships = OrderedDict(
-            ((src, tar), _membership(src, tar))
-            for src, tar in sorted(product(src_only, tar_only))
-        )
-
-        while memberships:
-            src_tok, tar_tok = max(memberships, key=memberships.get)
-            if memberships[src_tok, tar_tok] > 0.0:
-                pairings = min(src_only[src_tok], tar_only[tar_tok])
-                if pairings:
-                    (
-                        src_ntok,
-                        src_val,
-                        tar_ntok,
-                        tar_val,
-                        int_ntok,
-                        int_val,
-                    ) = _token_src_tar_int(src_tok, tar_tok)
-
-                    src_new[src_ntok] += src_val * pairings  # type: ignore
-                    tar_new[tar_ntok] += tar_val * pairings  # type: ignore
-                    intersection[int_ntok] += int_val * pairings  # type: ignore
-
-                    # Remove pairings from src_only/tar_only
-                    src_only[src_tok] -= pairings
-                    tar_only[tar_tok] -= pairings
-
-            del memberships[src_tok, tar_tok]
-
-        # Add src_new/tar_new back into src_only/tar_only
-        src_only += src_new
-        tar_only += tar_new
-
-        # Save src_only/tar_only to the instance for retrieval later.
-        self._soft_src_only = src_only
-        self._soft_tar_only = tar_only
-        self._soft_intersection_precalc = intersection
-
-        return intersection
-
-    def _fuzzy_intersection(self) -> TCounter[str]:
-        r"""Return the fuzzy intersection of the tokens in src and tar.
-
-        This implements the fuzzy intersection defined by :cite:`Wang:2014`.
-
-        For two sets X and Y, the intersection :cite:`Wang:2014` is the sum of
-        similarities of all tokens in the two sets that are greater than or
-        equal to some threshold value (:math:`\delta`).
-
-        The lower bound of on this intersection and the value when
-        :math:`\delta = 1.0`, is the crisp intersection. Tokens shorter than
-        :math:`\frac{\delta}{1-\delta}`, 4 in the case of the default threshold
-        :math:`\delta = 0.8`, must match exactly to be included in the
-        intersection.
-
-
-        .. versionadded:: 0.4.0
-
-        """
-        intersection = self._crisp_intersection()
-        src_only = self._src_tokens - self._tar_tokens
-        tar_only = self._tar_tokens - self._src_tokens
-
-        pair = {}
-        for src_tok in sorted(src_only):
-            for tar_tok in sorted(tar_only):
-                sim = self.params['metric'].sim(src_tok, tar_tok)
-                if sim >= self.params['threshold']:
-                    pair[(src_tok, tar_tok)] = sim
-
-        ordered_keys = [(pair[_], _[0], _[1]) for _ in pair]
-        ordered_keys.sort(key=lambda x: x[2])
-        ordered_keys.sort(key=lambda x: x[1])
-        ordered_keys.sort(key=lambda x: x[0], reverse=True)
-
-        for _, src_tok, tar_tok in ordered_keys:
-            pairings = min(src_only[src_tok], tar_only[tar_tok])
-            if pairings:
-                sim = pair[(src_tok, tar_tok)]
-
-                intersection[src_tok] += sim / 2 * pairings
-                intersection[tar_tok] += sim / 2 * pairings
-
-                src_only[src_tok] -= pairings
-                tar_only[tar_tok] -= pairings
-
-        """
-        # Here is a slightly different optimization method, which is even
-        # greedier than the above.
-        # ordered by sim*pairings rather than just sim
-
-        pair = {}
-        for src_tok in sorted(src_only):
-            for tar_tok in sorted(tar_only):
-                sim = self.params['metric'].sim(src_tok, tar_tok)
-                if sim >= self.params['threshold']:
-                    pairings = min(src_only[src_tok], tar_only[tar_tok])
-                    pair[(src_tok, tar_tok)] = sim*pairings
-
-        for src_tok, tar_tok in sorted(pair, key=pair.get, reverse=True):
-            pairings = min(src_only[src_tok], tar_only[tar_tok])
-            if pairings:
-                sim = pair[(src_tok, tar_tok)]
-
-                intersection[src_tok] += sim / 2
-                intersection[tar_tok] += sim / 2
-
-                src_only[src_tok] -= pairings
-                tar_only[tar_tok] -= pairings
-        """
-
-        return intersection
-
-    def _group_linkage_intersection(self) -> TCounter[str]:
-        r"""Return the group linkage intersection of the tokens in src and tar.
-
-        This is based on group linkage, as defined by :cite:`On:2007`.
-
-        Most of this method is concerned with solving the assignment problem,
-        in order to find the weight of the maximum weight bipartite matching.
-        The Hungarian algorithm of Munkres :cite:`Munkres:1957`, implemented
-        below in Python & Numpy is used to solve the assignment problem since
-        it is roughly twice as fast as SciPy's implementation.
-
-        .. versionadded:: 0.4.0
-        .. versionchanged:: 0.4.1
-            Corrected the Hungarian algorithm & optimized it so that SciPy's
-            version is no longer needed.
-
-        """
-        intersection = self._crisp_intersection()
-        src_only_tok = sorted(self._src_tokens - self._tar_tokens)
-        tar_only_tok = sorted(self._tar_tokens - self._src_tokens)
-        src_only = self._src_tokens - self._tar_tokens
-        tar_only = self._tar_tokens - self._src_tokens
-
-        # Quoted text below is from Munkres (1957), cited above.
-
-        # Pre-preliminaries: create square the matrix of scores
-        n = max(len(src_only_tok), len(tar_only_tok))
-        arr = np.zeros((n, n), dtype=float)
-
-        for col in range(len(src_only_tok)):
-            for row in range(len(tar_only_tok)):
-                arr[row, col] = self.params['metric'].dist(
-                    src_only_tok[col], tar_only_tok[row]
-                )
-
-        src_only_tok += [''] * (n - len(src_only_tok))
-        tar_only_tok += [''] * (n - len(tar_only_tok))
-
-        starred = np.zeros((n, n), dtype=np.bool_)
-        primed = np.zeros((n, n), dtype=np.bool_)
-        row_covered = np.zeros(n, dtype=np.bool_)
-        col_covered = np.zeros(n, dtype=np.bool_)
-
-        orig_sim = 1 - np.copy(arr)
-        # Preliminaries:
-        # P: "No lines are covered; no zeros are starred or primed."
-        # P: "Consider a row of matrix A; subtract from each element in
-        # this row the smallest element of this row. Do the same for each
-        # row of A."
-        arr -= arr.min(axis=1, keepdims=True)
-        # P: "Then consider each column of the resulting matrix and
-        # subtract from each column its smallest entry."
-        arr -= arr.min(axis=0, keepdims=True)
-
-        # P: "Consider a zero Z of the matrix. If there is no starred zero
-        # in its row and none in its column, star Z. Repeat, considering
-        # each zero in the matrix in turn. Then cover every column
-        # containing a starred zero.
-        for col in range(n):
-            for row in range(n):
-                if arr[row, col] == 0:
-                    if (
-                        np.count_nonzero(starred[row, :]) == 0
-                        and np.count_nonzero(starred[:, col]) == 0
-                    ):
-                        starred[row, col] = True
-                        col_covered[col] = True
-
-        step = 1
-        # This is the simple case where independent assignments are obvious
-        # and found without the rest of the algorithm.
-        if np.count_nonzero(col_covered) == n:
-            step = 4
-
-        while step < 4:
-            if step == 1:
-                # Step 1:
-                # 1: "Choose a non-covered zero and prime it. Consider the
-                # row containing it. If there is no starred zero in this
-                # row, go at once to Step 2. If there is a starred zero Z
-                # in this row, cover this row and uncover the column of Z."
-                # 1: Repeat until all zeros are covered. Go to Step 3."
-                zeros = tuple(zip(*((arr == 0).nonzero())))
-                while step == 1:
-                    for row, col in zeros:
-                        if not (col_covered[col] | row_covered[row]):
-                            primed[row, col] = True
-                            z_cols = (starred[row, :]).nonzero()[0]
-                            if not z_cols.size:
-                                step = 2
-                                break
-                            else:
-                                row_covered[row] = True
-                                col_covered[z_cols[0]] = False
-
-                    if step != 1:
-                        break
-
-                    for row, col in zeros:
-                        if not (col_covered[col] | row_covered[row]):
-                            break
-                    else:
-                        step = 3
-
-            if step == 2:
-                # Step 2:
-                # 2: "There is a sequence of alternating starred and primed
-                # zeros, constructed as follows: Let Z_0 denote the
-                # uncovered 0'. [There is only one.] Let Z_1 denote the 0*
-                # in Z_0's column (if any). Let Z_2 denote the 0' in Z_1's
-                # row (we must prove that it exists). Let Z_3 denote the 0*
-                # in Z_2's column (if any). Similarly continue until the
-                # sequence stops at a 0', Z_{2k}, which has no 0* in its
-                # column."
-                z_series = []
-                for row, col in zeros:  # pragma: no branch
-                    if primed[row, col] and not (
-                        row_covered[row] | col_covered[col]
-                    ):
-                        z_series.append((row, col))
-                        break
-                col = z_series[-1][1]
-                while True:
-                    row_content = tuple(
-                        set((arr[:, col] == 0).nonzero()[0])
-                        & set((starred[:, col]).nonzero()[0])
-                    )
-                    if row_content:
-                        row = row_content[0]
-                        z_series.append((row, col))
-                        col = tuple(
-                            set((arr[row, :] == 0).nonzero()[0])
-                            & set((primed[row, :]).nonzero()[0])
-                        )[0]
-                        z_series.append((row, col))
-                    else:
-                        break
-
-                # 2: "Unstar each starred zero of the sequence and star
-                # each primed zero of the sequence. Erase all primes,
-                # uncover every row, and cover every column containing a
-                # 0*."
-                primed[:, :] = False
-                row_covered[:] = False
-                col_covered[:] = False
-                for row, col in z_series:
-                    starred[row, col] = not starred[row, col]
-                for col in range(n):
-                    if np.count_nonzero(starred[:, col]):
-                        col_covered[col] = True
-                # 2: "If all columns are covered, the starred zeros form
-                # the desired independent set. Otherwise, return to Step
-                # 1."
-                if np.count_nonzero(col_covered) == n:
-                    step = 4
-                else:
-                    step = 1
-
-            if step == 3:
-                # Step 3:
-                # 3: "Let h denote the smallest non-covered element of the
-                # matrix; it will be positive. Add h to each covered row;
-                # then subtract h from each uncovered column."
-                h_val = float('inf')
-                for col in range(n):
-                    if not (col_covered[col]):
-                        for row in range(n):
-                            if (
-                                not (row_covered[row])
-                                and arr[row, col] < h_val
-                            ):
-                                h_val = arr[row, col]
-                for row in range(n):
-                    if row_covered[row]:
-                        arr[row, :] += h_val
-                for col in range(n):
-                    if not (col_covered[col]):
-                        arr[:, col] -= h_val
-
-                # 3: "Return to Step 1, without altering any asterisks,
-                # primes, or covered lines."
-                step = 1
-
-        for row, col in tuple(zip(*(starred.nonzero()))):
-            sim = orig_sim[row, col]
-            if sim >= self.params['threshold']:
-                score = float(
-                    (sim / 2)
-                    * min(
-                        src_only[src_only_tok[col]],
-                        tar_only[tar_only_tok[row]],
-                    )
-                )
-                intersection[src_only_tok[col]] += score  # type: ignore
-                intersection[tar_only_tok[row]] += score  # type: ignore
-
-        return intersection
-
-    def _intersection_card(self) -> float:
-        """Return the cardinality of the intersection."""
-        return self.normalizer(
-            sum(abs(val) for val in self._intersection().values()),
-            1,
-            self._population_card_value,
-        )
-
-    def _intersection(self) -> TCounter[str]:
-        """Return the intersection.
-
-        This function may be overridden by setting the intersection_type during
-        initialization.
-        """
-        return self._crisp_intersection()  # pragma: no cover
-
-
-if __name__ == '__main__':
-    import doctest
-
-    doctest.testmod()
+# Copyright 2018-2020 by Christopher C. Little.
+# This file is part of Abydos.
+#
+# Abydos is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# Abydos is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with Abydos. If not, see <http://www.gnu.org/licenses/>.
+
+"""abydos.distance._token_distance.
+
+The distance._token_distance._TokenDistance module implements abstract class
+_TokenDistance.
+"""
+
+from collections import Counter, OrderedDict
+from itertools import product
+from math import exp, log1p
+from typing import (
+    Any,
+    Callable,
+    Counter as TCounter,
+    Optional,
+    Tuple,
+    Union,
+    cast,
+)
+
+import numpy as np
+
+from ._damerau_levenshtein import DamerauLevenshtein
+from ._distance import _Distance
+from ._lcprefix import LCPrefix
+from ._levenshtein import Levenshtein
+from ._tokenizer import _Tokenizer
+from ._whitespace import WhitespaceTokenizer
+from ._q_grams import QGrams
+from ._q_skipgrams import QSkipgrams
+
+__all__ = ['_TokenDistance']
+
+
+class _TokenDistance(_Distance):
+    r"""Abstract Token Distance class.
+
+    .. _confusion_table:
+
+    +----------------+--------------+-----------------+-------+
+    |                | |in| ``tar`` | |notin| ``tar`` |       |
+    +----------------+--------------+-----------------+-------+
+    | |in| ``src``   | |a|          | |b|             | |a+b| |
+    +----------------+--------------+-----------------+-------+
+    | |notin| ``src``| |c|          | |d|             | |c+d| |
+    +----------------+--------------+-----------------+-------+
+    |                | |a+c|        | |b+d|           | |n|   |
+    +----------------+--------------+-----------------+-------+
+
+    .. |in| replace:: :math:`x \in`
+    .. |notin| replace:: :math:`x \notin`
+
+    .. |a| replace:: :math:`a = |X \cap Y|`
+    .. |b| replace:: :math:`b = |X\setminus Y|`
+    .. |c| replace:: :math:`c = |Y \setminus X|`
+    .. |d| replace:: :math:`d = |(N\setminus X)\setminus Y|`
+    .. |n| replace:: :math:`n = |N|`
+    .. |a+b| replace:: :math:`p_1 = a+b = |X|`
+    .. |a+c| replace:: :math:`p_2 = a+c = |Y|`
+    .. |c+d| replace:: :math:`q_1 = c+d = |N\setminus X|`
+    .. |b+d| replace:: :math:`q_2 = b+d = |N\setminus Y|`
+
+    .. versionadded:: 0.3.6
+    """
+
+    def __init__(
+        self,
+        tokenizer: Optional[_Tokenizer] = None,
+        intersection_type: str = 'crisp',
+        **kwargs: Any
+    ) -> None:
+        r"""Initialize _TokenDistance instance.
+
+        .. _intersection_type:
+
+        Parameters
+        ----------
+        tokenizer : _Tokenizer
+            A tokenizer instance from the :py:mod:`abydos.tokenizer` package
+        intersection_type : str
+            Specifies the intersection type, and set type as a result:
+
+                - 'crisp': Ordinary intersection, wherein items are entirely
+                  members or non-members of the intersection. (Default)
+                - ``fuzzy``: Fuzzy intersection, defined by :cite:`Wang:2014`,
+                  wherein items can be partially members of the intersection
+                  if their similarity meets or exceeds a threshold value. This
+                  also takes `metric` (by default :class:`Levenshtein()`) and
+                  `threshold` (by default 0.8) parameters.
+                - ``soft``: Soft intersection, defined by :cite:`Russ:2014`,
+                  wherein items can be partially members of the intersection
+                  depending on their similarity. This also takes a `metric`
+                  (by default :class:`DamerauLevenshtein()`) parameter.
+                - ``linkage``: Group linkage, defined by :cite:`On:2007`. Like
+                  the soft intersection, items can be partially members of the
+                  intersection, but the method of pairing similar members is
+                  somewhat more complex. See the cited paper for details. This
+                  also takes `metric`
+                  (by default :class:`DamerauLevenshtein()`) and `threshold`
+                  (by default 0.1) parameters.
+        **kwargs
+            Arbitrary keyword arguments
+
+
+        .. _alphabet:
+
+        Other Parameters
+        ----------------
+        qval : int
+            The length of each q-gram. Using this parameter and tokenizer=None
+            will cause the instance to use the QGram tokenizer with this
+            q value.
+        metric : _Distance
+            A string distance measure class for use in the ``soft`` and
+            ``fuzzy`` variants.
+        threshold : float
+            A threshold value, similarities above which are counted as
+            members of the intersection for the ``fuzzy`` variant.
+        alphabet : Counter, collection, int, or None
+            This represents the alphabet of possible tokens.
+
+                - If a Counter is supplied, it is used directly in computing
+                  the complement of the tokens in both sets.
+                - If a collection is supplied, it is converted to a Counter
+                  and used directly. In the case of a single string being
+                  supplied and the QGram tokenizer being used, the full
+                  alphabet is inferred (i.e.
+                  :math:`len(set(alphabet+QGrams.start\_stop))^{QGrams.qval}`
+                  is used as the cardinality of the full alphabet.
+                - If an int is supplied, it is used as the cardinality of the
+                  full alphabet.
+                - If None is supplied, the cardinality of the full alphabet
+                  is inferred if QGram of QSkipgrams tokenization is used (i.e.
+                  :math:`28^{QGrams.qval}` is used as the cardinality of the
+                  full alphabet or :math:`26` if QGrams.qval is 1, which
+                  assumes the strings are English language strings and only
+                  contain letters of a single case). Otherwise, the cardinality
+                  of the complement of the total will be 0.
+        normalizer : str
+            This represents the normalization applied to the values in the
+            2x2 contingency table prior to any of the cardinality (\*_card)
+            methods returning a value. By default, no normalization is applied,
+            but the following values are supported:
+
+                - ``proportional`` : :math:`\frac{x}{n}`, where n is the total
+                  population
+                - ``log`` : :math:`log(1+x)`
+                - ``exp`` : :math:`e^x`
+                - ``laplace`` : :math:`x+1`
+                - ``inverse`` : :math:`\frac{1}{x}`
+                - ``complement`` : :math:`n-x`, where n is the total population
+
+        .. versionadded:: 0.4.0
+
+        """
+        super(_TokenDistance, self).__init__(
+            intersection_type=intersection_type, **kwargs
+        )
+
+        qval = 2 if 'qval' not in self.params else self.params['qval']
+        self.params['tokenizer'] = (
+            tokenizer
+            if tokenizer is not None
+            else WhitespaceTokenizer()
+            if qval == 0
+            else QGrams(qval=qval, start_stop='$#', skip=0, scaler=None)
+        )
+
+        if hasattr(self.params['tokenizer'], 'qval'):
+            if isinstance(self.params['tokenizer'].qval, int):
+                qvals = [self.params['tokenizer'].qval]
+            else:
+                qvals = list(self.params['tokenizer'].qval)
+        else:
+            qvals = []
+
+        if 'alphabet' in self.params:
+            if isinstance(self.params['alphabet'], str):
+                alpha_set = set(self.params['alphabet'])
+                if isinstance(self.params['tokenizer'], (QGrams, QSkipgrams)):
+                    alpha_set |= set(self.params['tokenizer'].start_stop)
+                    self.params['alphabet'] = sum(
+                        len(alpha_set) ** qval for qval in qvals
+                    )
+            if hasattr(self.params['alphabet'], '__len__') and not isinstance(
+                self.params['alphabet'], Counter
+            ):
+                self.params['alphabet'] = len(self.params['alphabet'])
+            elif self.params['alphabet'] is None and isinstance(
+                self.params['tokenizer'], (QGrams, QSkipgrams)
+            ):
+                self.params['alphabet'] = sum(
+                    28 ** qval if qval > 1 else 26 for qval in qvals
+                )
+        else:
+            if isinstance(self.params['tokenizer'], (QGrams, QSkipgrams)):
+                self.params['alphabet'] = sum(
+                    28 ** qval if qval > 1 else 26 for qval in qvals
+                )
+            else:
+                self.params['alphabet'] = None
+
+        if intersection_type == 'soft':
+            if 'metric' not in self.params or self.params['metric'] is None:
+                self.params['metric'] = Levenshtein()
+            self._lcprefix = LCPrefix()
+            self._intersection = self._soft_intersection  # type: ignore
+        elif intersection_type == 'fuzzy':
+            if 'metric' not in self.params or self.params['metric'] is None:
+                self.params['metric'] = Levenshtein()
+            if 'threshold' not in self.params:
+                self.params['threshold'] = 0.8
+            self._intersection = self._fuzzy_intersection  # type: ignore
+        elif intersection_type == 'linkage':
+            if 'metric' not in self.params or self.params['metric'] is None:
+                self.params['metric'] = DamerauLevenshtein()
+            if 'threshold' not in self.params:
+                self.params['threshold'] = 0.1
+            self._intersection = (  # type: ignore
+                self._group_linkage_intersection
+            )
+        else:
+            self._intersection = self._crisp_intersection  # type: ignore
+
+        self._src_tokens = Counter()  # type: TCounter[str]
+        self._tar_tokens = Counter()  # type: TCounter[str]
+        self._population_card_value = 0  # type: float
+
+        # initialize normalizer
+        self.normalizer = (
+            self._norm_none
+        )  # type: Callable[[float, int, float], float]  # noqa: E501
+
+        self._norm_dict = {
+            'proportional': self._norm_proportional,
+            'log': self._norm_log,
+            'exp': self._norm_exp,
+            'laplace': self._norm_laplace,
+            'inverse': self._norm_inverse,
+            'complement': self._norm_complement,
+        }
+
+        # initialize values for soft intersection
+        self._soft_intersection_precalc = Counter()  # type: TCounter[str]
+        self._soft_src_only = Counter()  # type: TCounter[str]
+        self._soft_tar_only = Counter()  # type: TCounter[str]
+
+    @staticmethod
+    def _norm_none(x: float, _squares: int, _pop: float) -> float:
+        return x
+
+    @staticmethod
+    def _norm_proportional(x: float, _squares: int, pop: float) -> float:
+        return x / max(1, pop)
+
+    @staticmethod
+    def _norm_log(x: float, _squares: int, _pop: float) -> float:
+        return log1p(x)
+
+    @staticmethod
+    def _norm_exp(x: float, _squares: int, _pop: float) -> float:
+        return exp(x)
+
+    @staticmethod
+    def _norm_laplace(x: float, squares: int, _pop: float) -> float:
+        return x + squares
+
+    @staticmethod
+    def _norm_inverse(x: float, _squares: int, pop: float) -> float:
+        return 1 / x if x else pop
+
+    @staticmethod
+    def _norm_complement(x: float, _squares: int, pop: float) -> float:
+        return pop - x
+
+    def _tokenize(
+        self, src: Union[str, TCounter[str]], tar: Union[str, TCounter[str]]
+    ) -> '_TokenDistance':
+        """Return the Q-Grams in src & tar.
+
+        Parameters
+        ----------
+        src : str
+            Source string (or QGrams/Counter objects) for comparison
+        tar : str
+            Target string (or QGrams/Counter objects) for comparison
+
+        Returns
+        -------
+        tuple of Counters
+            Q-Grams
+
+        Examples
+        --------
+        >>> pe = _TokenDistance()
+        >>> pe._tokenize('AT', 'TT')._get_tokens()
+        (Counter({'$A': 1, 'AT': 1, 'T#': 1}),
+         Counter({'$T': 1, 'TT': 1, 'T#': 1}))
+
+
+        .. versionadded:: 0.1.0
+        .. versionchanged:: 0.3.6
+            Encapsulated in class
+
+        """
+        self._src_orig = src
+        self._tar_orig = tar
+
+        if isinstance(src, Counter):
+            self._src_tokens = src
+        else:
+            self._src_tokens = (
+                self.params['tokenizer'].tokenize(src).get_counter()
+            )
+        if isinstance(tar, Counter):
+            self._tar_tokens = tar
+        else:
+            self._tar_tokens = (
+                self.params['tokenizer'].tokenize(tar).get_counter()
+            )
+
+        self._population_card_value = self._calc_population_card()
+
+        # Set up the normalizer, a function of two variables:
+        # x is the value in the contingency table square(s)
+        # n is the number of squares that x represents
+        if (
+            'normalizer' in self.params
+            and self.params['normalizer'] in self._norm_dict
+        ):
+            self.normalizer = self._norm_dict[self.params['normalizer']]
+
+        # clear values for soft intersection
+        self._soft_intersection_precalc = Counter()
+        self._soft_src_only = Counter()
+        self._soft_tar_only = Counter()
+
+        return self
+
+    def _get_tokens(self) -> Tuple[TCounter[str], TCounter[str]]:
+        """Return the src and tar tokens as a tuple."""
+        return self._src_tokens, self._tar_tokens
+
+    def _src_card(self) -> float:
+        r"""Return the cardinality of the tokens in the source set."""
+        if self.params['intersection_type'] == 'soft':
+            if not len(self._soft_intersection_precalc):
+                self._intersection()
+            return self.normalizer(
+                sum(
+                    abs(val)
+                    for val in (
+                        self._soft_intersection_precalc + self._soft_src_only
+                    ).values()
+                ),
+                2,
+                self._population_card_value,
+            )
+        return self.normalizer(
+            sum(abs(val) for val in self._src_tokens.values()),
+            2,
+            self._population_card_value,
+        )
+
+    def _src_only(self) -> TCounter[str]:
+        r"""Return the src tokens minus the tar tokens.
+
+        For (multi-)sets S and T, this is :math:`S \setminus T`.
+        """
+        if self.params['intersection_type'] == 'soft':
+            if not len(self._soft_intersection_precalc):
+                self._intersection()
+            return self._soft_src_only
+        src_only = self._src_tokens - self._intersection()
+        if self.params['intersection_type'] != 'crisp':
+            src_only -= self._intersection() - self._crisp_intersection()
+        return src_only
+
+    def _src_only_card(self) -> float:
+        """Return the cardinality of the tokens only in the source set."""
+        return self.normalizer(
+            sum(abs(val) for val in self._src_only().values()),
+            1,
+            self._population_card_value,
+        )
+
+    def _tar_card(self) -> float:
+        r"""Return the cardinality of the tokens in the target set."""
+        if self.params['intersection_type'] == 'soft':
+            if not len(self._soft_intersection_precalc):
+                self._intersection()
+            return self.normalizer(
+                sum(
+                    abs(val)
+                    for val in (
+                        self._soft_intersection_precalc + self._soft_tar_only
+                    ).values()
+                ),
+                2,
+                self._population_card_value,
+            )
+        return self.normalizer(
+            sum(abs(val) for val in self._tar_tokens.values()),
+            2,
+            self._population_card_value,
+        )
+
+    def _tar_only(self) -> TCounter[str]:
+        r"""Return the tar tokens minus the src tokens.
+
+        For (multi-)sets S and T, this is :math:`T \setminus S`.
+        """
+        if self.params['intersection_type'] == 'soft':
+            if not len(self._soft_intersection_precalc):
+                self._intersection()
+            return self._soft_tar_only
+        tar_only = self._tar_tokens - self._intersection()
+        if self.params['intersection_type'] != 'crisp':
+            tar_only -= self._intersection() - self._crisp_intersection()
+        return tar_only
+
+    def _tar_only_card(self) -> float:
+        """Return the cardinality of the tokens only in the target set."""
+        return self.normalizer(
+            sum(abs(val) for val in self._tar_only().values()),
+            1,
+            self._population_card_value,
+        )
+
+    def _symmetric_difference(self) -> TCounter[str]:
+        r"""Return the symmetric difference of tokens from src and tar.
+
+        For (multi-)sets S and T, this is :math:`S \triangle T`.
+        """
+        return self._src_only() + self._tar_only()
+
+    def _symmetric_difference_card(self) -> float:
+        """Return the cardinality of the symmetric difference."""
+        return self.normalizer(
+            sum(abs(val) for val in self._symmetric_difference().values()),
+            2,
+            self._population_card_value,
+        )
+
+    def _total(self) -> TCounter[str]:
+        """Return the sum of the sets.
+
+        For (multi-)sets S and T, this is :math:`S + T`.
+
+        In the case of multisets, this counts values in the intersection
+        twice. In the case of sets, this is identical to the union.
+        """
+        if self.params['intersection_type'] == 'soft':
+            if not len(self._soft_intersection_precalc):
+                self._intersection()
+            return (
+                self._soft_tar_only
+                + self._soft_src_only
+                + self._soft_intersection_precalc
+                + self._soft_intersection_precalc
+            )
+        return self._src_tokens + self._tar_tokens
+
+    def _total_card(self) -> float:
+        """Return the cardinality of the complement of the total."""
+        return self.normalizer(
+            sum(abs(val) for val in self._total().values()),
+            3,
+            self._population_card_value,
+        )
+
+    def _total_complement_card(self) -> float:
+        """Return the cardinality of the complement of the total."""
+        if self.params['alphabet'] is None:
+            return self.normalizer(0, 1, self._population_card_value)
+        elif isinstance(self.params['alphabet'], Counter):
+            return self.normalizer(
+                max(
+                    0,
+                    sum(
+                        abs(val)
+                        for val in (
+                            self.params['alphabet'] - self._total()
+                        ).values()
+                    ),
+                ),
+                1,
+                self._population_card_value,
+            )
+        return self.normalizer(
+            max(0, self.params['alphabet'] - len(self._total().values())),
+            1,
+            self._population_card_value,
+        )
+
+    def _calc_population_card(self) -> float:
+        """Return the cardinality of the population."""
+        save_normalizer = self.normalizer
+        self.normalizer = self._norm_none
+        save_intersection = self.params['intersection_type']
+        self.params['intersection_type'] = 'crisp'
+        pop = self._total_card() + self._total_complement_card()
+        self.normalizer = save_normalizer
+        self.params['intersection_type'] = save_intersection
+        return pop
+
+    def _population_card(self) -> float:
+        """Return the cardinality of the population."""
+        return self.normalizer(
+            self._population_card_value, 4, self._population_card_value
+        )
+
+    def _population_unique_card(self) -> float:
+        """Return the cardinality of the population minus the intersection."""
+        return self.normalizer(
+            self._population_card_value - self._intersection_card(),
+            4,
+            self._population_card_value,
+        )
+
+    def _union(self) -> TCounter[str]:
+        r"""Return the union of tokens from src and tar.
+
+        For (multi-)sets S and T, this is :math:`S \cup T`.
+        """
+        if self.params['intersection_type'] == 'soft':
+            if not len(self._soft_intersection_precalc):
+                self._intersection()
+            return (
+                self._soft_tar_only
+                + self._soft_src_only
+                + self._soft_intersection_precalc
+            )
+        union = self._total() - self._intersection()
+        if self.params['intersection_type'] != 'crisp':
+            union -= self._intersection() - self._crisp_intersection()
+        return union
+
+    def _union_card(self) -> float:
+        """Return the cardinality of the union."""
+        return self.normalizer(
+            sum(abs(val) for val in self._union().values()),
+            3,
+            self._population_card_value,
+        )
+
+    def _difference(self) -> TCounter[str]:
+        """Return the difference of the tokens, supporting negative values."""
+        if self.params['intersection_type'] == 'soft':
+            if not len(self._soft_intersection_precalc):
+                self._intersection()
+            _src_copy = Counter(self._soft_src_only)
+            _src_copy.subtract(self._soft_tar_only)
+            return _src_copy
+        _src_copy = Counter(self._src_tokens)
+        _src_copy.subtract(self._tar_tokens)
+        return _src_copy
+
+    def _crisp_intersection(self) -> TCounter[str]:
+        r"""Return the intersection of tokens from src and tar.
+
+        For (multi-)sets S and T, this is :math:`S \cap T`.
+        """
+        return self._src_tokens & self._tar_tokens
+
+    def _soft_intersection(self) -> TCounter[str]:
+        """Return the soft source, target, & intersection tokens & weights.
+
+        This implements the soft intersection defined by :cite:`Russ:2014` in
+        a way that can reproduce the results in the paper.
+        """
+        if not hasattr(self.params['metric'], 'alignment'):
+            raise TypeError(
+                "Soft similarity requires a 'metric' with an alignment \
+member function, such as Levenshtein."
+            )
+
+        intersection = self._crisp_intersection()
+        src_only = self._src_tokens - self._tar_tokens
+        tar_only = self._tar_tokens - self._src_tokens
+
+        src_new = Counter()  # type: TCounter[str]
+        tar_new = Counter()  # type: TCounter[str]
+
+        def _membership(src: str, tar: str) -> float:
+            greater_length = max(len(src), len(tar))
+            return cast(
+                float,
+                max(
+                    greater_length - self.params['metric'].dist_abs(src, tar),
+                    self._lcprefix.dist_abs(src, tar),
+                )
+                / greater_length,
+            )
+
+        def _token_src_tar_int(
+            src: str, tar: str
+        ) -> Tuple[str, float, str, float, str, float]:
+            src_tok = []
+            tar_tok = []
+            int_tok = []
+
+            src_val = 0.0
+            tar_val = 0.0
+            int_val = 0.0
+
+            _cost, _src, _tar = self.params['metric'].alignment(src, tar)
+
+            for i in range(len(_src)):
+                if _src[i] == _tar[i]:
+                    src_tok.append('-')
+                    tar_tok.append('-')
+                    int_tok.append(_src[i])
+                    int_val += 1
+                else:
+                    src_tok.append(_src[i])
+                    if _src[i] != '-':
+                        src_val += 1
+                    tar_tok.append(_tar[i])
+                    if _tar[i] != '-':
+                        tar_val += 1
+                    int_tok.append('-')
+
+            src_val /= len(_src)
+            tar_val /= len(_src)
+            int_val /= len(_src)
+
+            src_tok_str = ''.join(src_tok).strip('-')
+            tar_tok_str = ''.join(tar_tok).strip('-')
+            int_tok_str = ''.join(int_tok).strip('-')
+
+            return (
+                src_tok_str,
+                src_val,
+                tar_tok_str,
+                tar_val,
+                int_tok_str,
+                int_val,
+            )
+
+        # Dictionary ordering is important for reproducibility, so insertion
+        # order needs to be controlled and retained.
+        memberships = OrderedDict(
+            ((src, tar), _membership(src, tar))
+            for src, tar in sorted(product(src_only, tar_only))
+        )
+
+        while memberships:
+            src_tok, tar_tok = max(memberships, key=memberships.get)
+            if memberships[src_tok, tar_tok] > 0.0:
+                pairings = min(src_only[src_tok], tar_only[tar_tok])
+                if pairings:
+                    (
+                        src_ntok,
+                        src_val,
+                        tar_ntok,
+                        tar_val,
+                        int_ntok,
+                        int_val,
+                    ) = _token_src_tar_int(src_tok, tar_tok)
+
+                    src_new[src_ntok] += src_val * pairings  # type: ignore
+                    tar_new[tar_ntok] += tar_val * pairings  # type: ignore
+                    intersection[int_ntok] += int_val * pairings  # type: ignore
+
+                    # Remove pairings from src_only/tar_only
+                    src_only[src_tok] -= pairings
+                    tar_only[tar_tok] -= pairings
+
+            del memberships[src_tok, tar_tok]
+
+        # Add src_new/tar_new back into src_only/tar_only
+        src_only += src_new
+        tar_only += tar_new
+
+        # Save src_only/tar_only to the instance for retrieval later.
+        self._soft_src_only = src_only
+        self._soft_tar_only = tar_only
+        self._soft_intersection_precalc = intersection
+
+        return intersection
+
+    def _fuzzy_intersection(self) -> TCounter[str]:
+        r"""Return the fuzzy intersection of the tokens in src and tar.
+
+        This implements the fuzzy intersection defined by :cite:`Wang:2014`.
+
+        For two sets X and Y, the intersection :cite:`Wang:2014` is the sum of
+        similarities of all tokens in the two sets that are greater than or
+        equal to some threshold value (:math:`\delta`).
+
+        The lower bound of on this intersection and the value when
+        :math:`\delta = 1.0`, is the crisp intersection. Tokens shorter than
+        :math:`\frac{\delta}{1-\delta}`, 4 in the case of the default threshold
+        :math:`\delta = 0.8`, must match exactly to be included in the
+        intersection.
+
+
+        .. versionadded:: 0.4.0
+
+        """
+        intersection = self._crisp_intersection()
+        src_only = self._src_tokens - self._tar_tokens
+        tar_only = self._tar_tokens - self._src_tokens
+
+        pair = {}
+        for src_tok in sorted(src_only):
+            for tar_tok in sorted(tar_only):
+                sim = self.params['metric'].sim(src_tok, tar_tok)
+                if sim >= self.params['threshold']:
+                    pair[(src_tok, tar_tok)] = sim
+
+        ordered_keys = [(pair[_], _[0], _[1]) for _ in pair]
+        ordered_keys.sort(key=lambda x: x[2])
+        ordered_keys.sort(key=lambda x: x[1])
+        ordered_keys.sort(key=lambda x: x[0], reverse=True)
+
+        for _, src_tok, tar_tok in ordered_keys:
+            pairings = min(src_only[src_tok], tar_only[tar_tok])
+            if pairings:
+                sim = pair[(src_tok, tar_tok)]
+
+                intersection[src_tok] += sim / 2 * pairings
+                intersection[tar_tok] += sim / 2 * pairings
+
+                src_only[src_tok] -= pairings
+                tar_only[tar_tok] -= pairings
+
+        """
+        # Here is a slightly different optimization method, which is even
+        # greedier than the above.
+        # ordered by sim*pairings rather than just sim
+
+        pair = {}
+        for src_tok in sorted(src_only):
+            for tar_tok in sorted(tar_only):
+                sim = self.params['metric'].sim(src_tok, tar_tok)
+                if sim >= self.params['threshold']:
+                    pairings = min(src_only[src_tok], tar_only[tar_tok])
+                    pair[(src_tok, tar_tok)] = sim*pairings
+
+        for src_tok, tar_tok in sorted(pair, key=pair.get, reverse=True):
+            pairings = min(src_only[src_tok], tar_only[tar_tok])
+            if pairings:
+                sim = pair[(src_tok, tar_tok)]
+
+                intersection[src_tok] += sim / 2
+                intersection[tar_tok] += sim / 2
+
+                src_only[src_tok] -= pairings
+                tar_only[tar_tok] -= pairings
+        """
+
+        return intersection
+
+    def _group_linkage_intersection(self) -> TCounter[str]:
+        r"""Return the group linkage intersection of the tokens in src and tar.
+
+        This is based on group linkage, as defined by :cite:`On:2007`.
+
+        Most of this method is concerned with solving the assignment problem,
+        in order to find the weight of the maximum weight bipartite matching.
+        The Hungarian algorithm of Munkres :cite:`Munkres:1957`, implemented
+        below in Python & Numpy is used to solve the assignment problem since
+        it is roughly twice as fast as SciPy's implementation.
+
+        .. versionadded:: 0.4.0
+        .. versionchanged:: 0.4.1
+            Corrected the Hungarian algorithm & optimized it so that SciPy's
+            version is no longer needed.
+
+        """
+        intersection = self._crisp_intersection()
+        src_only_tok = sorted(self._src_tokens - self._tar_tokens)
+        tar_only_tok = sorted(self._tar_tokens - self._src_tokens)
+        src_only = self._src_tokens - self._tar_tokens
+        tar_only = self._tar_tokens - self._src_tokens
+
+        # Quoted text below is from Munkres (1957), cited above.
+
+        # Pre-preliminaries: create square the matrix of scores
+        n = max(len(src_only_tok), len(tar_only_tok))
+        arr = np.zeros((n, n), dtype=float)
+
+        for col in range(len(src_only_tok)):
+            for row in range(len(tar_only_tok)):
+                arr[row, col] = self.params['metric'].dist(
+                    src_only_tok[col], tar_only_tok[row]
+                )
+
+        src_only_tok += [''] * (n - len(src_only_tok))
+        tar_only_tok += [''] * (n - len(tar_only_tok))
+
+        starred = np.zeros((n, n), dtype=np.bool_)
+        primed = np.zeros((n, n), dtype=np.bool_)
+        row_covered = np.zeros(n, dtype=np.bool_)
+        col_covered = np.zeros(n, dtype=np.bool_)
+
+        orig_sim = 1 - np.copy(arr)
+        # Preliminaries:
+        # P: "No lines are covered; no zeros are starred or primed."
+        # P: "Consider a row of matrix A; subtract from each element in
+        # this row the smallest element of this row. Do the same for each
+        # row of A."
+        arr -= arr.min(axis=1, keepdims=True)
+        # P: "Then consider each column of the resulting matrix and
+        # subtract from each column its smallest entry."
+        arr -= arr.min(axis=0, keepdims=True)
+
+        # P: "Consider a zero Z of the matrix. If there is no starred zero
+        # in its row and none in its column, star Z. Repeat, considering
+        # each zero in the matrix in turn. Then cover every column
+        # containing a starred zero.
+        for col in range(n):
+            for row in range(n):
+                if arr[row, col] == 0:
+                    if (
+                        np.count_nonzero(starred[row, :]) == 0
+                        and np.count_nonzero(starred[:, col]) == 0
+                    ):
+                        starred[row, col] = True
+                        col_covered[col] = True
+
+        step = 1
+        # This is the simple case where independent assignments are obvious
+        # and found without the rest of the algorithm.
+        if np.count_nonzero(col_covered) == n:
+            step = 4
+
+        while step < 4:
+            if step == 1:
+                # Step 1:
+                # 1: "Choose a non-covered zero and prime it. Consider the
+                # row containing it. If there is no starred zero in this
+                # row, go at once to Step 2. If there is a starred zero Z
+                # in this row, cover this row and uncover the column of Z."
+                # 1: Repeat until all zeros are covered. Go to Step 3."
+                zeros = tuple(zip(*((arr == 0).nonzero())))
+                while step == 1:
+                    for row, col in zeros:
+                        if not (col_covered[col] | row_covered[row]):
+                            primed[row, col] = True
+                            z_cols = (starred[row, :]).nonzero()[0]
+                            if not z_cols.size:
+                                step = 2
+                                break
+                            else:
+                                row_covered[row] = True
+                                col_covered[z_cols[0]] = False
+
+                    if step != 1:
+                        break
+
+                    for row, col in zeros:
+                        if not (col_covered[col] | row_covered[row]):
+                            break
+                    else:
+                        step = 3
+
+            if step == 2:
+                # Step 2:
+                # 2: "There is a sequence of alternating starred and primed
+                # zeros, constructed as follows: Let Z_0 denote the
+                # uncovered 0'. [There is only one.] Let Z_1 denote the 0*
+                # in Z_0's column (if any). Let Z_2 denote the 0' in Z_1's
+                # row (we must prove that it exists). Let Z_3 denote the 0*
+                # in Z_2's column (if any). Similarly continue until the
+                # sequence stops at a 0', Z_{2k}, which has no 0* in its
+                # column."
+                z_series = []
+                for row, col in zeros:  # pragma: no branch
+                    if primed[row, col] and not (
+                        row_covered[row] | col_covered[col]
+                    ):
+                        z_series.append((row, col))
+                        break
+                col = z_series[-1][1]
+                while True:
+                    row_content = tuple(
+                        set((arr[:, col] == 0).nonzero()[0])
+                        & set((starred[:, col]).nonzero()[0])
+                    )
+                    if row_content:
+                        row = row_content[0]
+                        z_series.append((row, col))
+                        col = tuple(
+                            set((arr[row, :] == 0).nonzero()[0])
+                            & set((primed[row, :]).nonzero()[0])
+                        )[0]
+                        z_series.append((row, col))
+                    else:
+                        break
+
+                # 2: "Unstar each starred zero of the sequence and star
+                # each primed zero of the sequence. Erase all primes,
+                # uncover every row, and cover every column containing a
+                # 0*."
+                primed[:, :] = False
+                row_covered[:] = False
+                col_covered[:] = False
+                for row, col in z_series:
+                    starred[row, col] = not starred[row, col]
+                for col in range(n):
+                    if np.count_nonzero(starred[:, col]):
+                        col_covered[col] = True
+                # 2: "If all columns are covered, the starred zeros form
+                # the desired independent set. Otherwise, return to Step
+                # 1."
+                if np.count_nonzero(col_covered) == n:
+                    step = 4
+                else:
+                    step = 1
+
+            if step == 3:
+                # Step 3:
+                # 3: "Let h denote the smallest non-covered element of the
+                # matrix; it will be positive. Add h to each covered row;
+                # then subtract h from each uncovered column."
+                h_val = float('inf')
+                for col in range(n):
+                    if not (col_covered[col]):
+                        for row in range(n):
+                            if (
+                                not (row_covered[row])
+                                and arr[row, col] < h_val
+                            ):
+                                h_val = arr[row, col]
+                for row in range(n):
+                    if row_covered[row]:
+                        arr[row, :] += h_val
+                for col in range(n):
+                    if not (col_covered[col]):
+                        arr[:, col] -= h_val
+
+                # 3: "Return to Step 1, without altering any asterisks,
+                # primes, or covered lines."
+                step = 1
+
+        for row, col in tuple(zip(*(starred.nonzero()))):
+            sim = orig_sim[row, col]
+            if sim >= self.params['threshold']:
+                score = float(
+                    (sim / 2)
+                    * min(
+                        src_only[src_only_tok[col]],
+                        tar_only[tar_only_tok[row]],
+                    )
+                )
+                intersection[src_only_tok[col]] += score  # type: ignore
+                intersection[tar_only_tok[row]] += score  # type: ignore
+
+        return intersection
+
+    def _intersection_card(self) -> float:
+        """Return the cardinality of the intersection."""
+        return self.normalizer(
+            sum(abs(val) for val in self._intersection().values()),
+            1,
+            self._population_card_value,
+        )
+
+    def _intersection(self) -> TCounter[str]:
+        """Return the intersection.
+
+        This function may be overridden by setting the intersection_type during
+        initialization.
+        """
+        return self._crisp_intersection()  # pragma: no cover
+
+
+if __name__ == '__main__':
+    import doctest
+
+    doctest.testmod()
```

### Comparing `name_matching-0.8.8/distances/_tokenizer.py` & `name_matching-0.8.9/distances/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_typo.py` & `name_matching-0.8.9/distances/_typo.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_warrens_iv.py` & `name_matching-0.8.9/distances/_warrens_iv.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_weighted_jaccard.py` & `name_matching-0.8.9/distances/_weighted_jaccard.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/distances/_whitespace.py` & `name_matching-0.8.9/distances/_whitespace.py`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/name_matching/distance_metrics.py` & `name_matching-0.8.9/name_matching/distance_metrics.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,266 +1,266 @@
-from distances import Indel, DiscountedLevenshtein, CormodeLZ, Tichy, IterativeSubString, BaulieuXIII, Clement, DiceAsymmetricI, KuhnsIII, Overlap, PearsonII, WeightedJaccard, WarrensIV, Bag, RougeL, RatcliffObershelp, NCDbz2, FuzzyWuzzyPartialString, FuzzyWuzzyTokenSort, FuzzyWuzzyTokenSet, Editex, Typo,LIG3, SSK, Levenshtein, DoubleMetaphone, RefinedSoundex, PhoneticDistance
-from collections import defaultdict
-
-def make_distance_metrics(indel=False,
-                          discounted_levenshtein=False,
-                          tichy=False,
-                          cormodel_z=False,
-                          iterative_sub_string=False,
-                          baulieu_xiii=False,
-                          clement=False,
-                          dice_asymmetrici=False,
-                          kuhns_iii=False,
-                          overlap=False,
-                          pearson_ii=False,
-                          weighted_jaccard=False,
-                          warrens_iv=False,
-                          bag=False,
-                          rouge_l=False,
-                          ratcliff_obershelp=False,
-                          ncd_bz2=False,
-                          fuzzy_wuzzy_partial_string=False,
-                          fuzzy_wuzzy_token_sort=False,
-                          fuzzy_wuzzy_token_set=False,
-                          editex=False,
-                          typo=False,
-                          lig_3=False,
-                          ssk=False,
-                          refined_soundex=False,
-                          double_metaphone=False) -> dict:
-    r"""
-    A function which returns a dict containing the distance metrics that should be 
-    used during the fuzzy string matching
-
-    Levenshtein edit distance
-        - Indel
-        - Discounted Levenshtein
-        - LIG3
-    Block edit distances
-        - Tichy
-        - CormodeLZ
-    Multi-set token-based distance
-        - BaulieuXIII
-        - Clement
-        - DiceAsymmetricI
-        - KuhnsIII
-        - Overlap
-        - PearsonII
-        - WeightedJaccard
-        - WarrensIV
-        - Bag
-        - RougeL
-    Subsequence distances
-        - IterativeSubString
-        - RatcliffObershelp
-        - SSK
-    Normalized compression distance
-        - NCDbz2
-    FuzzyWuzzy distances
-        - FuzzyWuzzyPartialString
-        - FuzzyWuzzyTokenSort
-        - FuzzyWuzzyTokenSet
-    Ponetic distances
-        - RefinedSoundex
-        - DoubleMetaphone
-    Edit distances
-        - Editex
-        - Typo
-
-
-    Parameters
-    ----------
-    indel: bool
-        Boolean indicating whether the Indel method should be used during the 
-        fuzzy name matching. The indel method is equal to a regular levenshtein 
-        distance with a twice as high substitution weight 
-        default=False
-    discounted_levenshtein: bool
-        Boolean indicating whether the DiscountedLevenshtein method should be used 
-        during the fuzzy name matching. Equal to the regular levenshtein distance,
-        only errors later in the string are counted at a discounted rate. To for
-        instance limit the importance of suffix differences
-        default=False
-    tichy: bool
-        Boolean indicating whether the Tichy method should be used during the 
-        fuzzy name matching. This algorithm provides a shortest edit distance based
-        on substring and add operations.
-        default=False
-    cormodel_z: bool
-        Boolean indicating whether the CormodeLZ method should be used during the 
-        fuzzy name matching. The CormodeLZ distance between strings x and y, is the 
-        minimum number of single characters or substrings of y or of the partially 
-        built string which are required to produce x from left to right.
-        default=False
-    iterative_sub_string: bool
-        Boolean indicating whether the IterativeSubString method should be used 
-        during the fuzzy name matching. A method that counts the similarities 
-        between two strings substrings and subtracts the differences taking into
-        account the winkler similarity between the string and the substring.
-        default=False
-    baulieu_xiii: bool
-        Boolean indicating whether the BaulieuXIII method should be used during 
-        the fuzzy name matching. The Baulieu XIII distance between two strings is
-        given by the following formula: (|X \ Y| + |Y \ X|) / (
-        |X ∩ Y| + |X \ Y| + |Y \ X| + |X ∩ Y| ∙ (|X ∩ Y| - 4)^2)
-        default=False
-    clement: bool
-        Boolean indicating whether the Clement method should be used during the
-        fuzzy name matching. The Clement distance between two strings is given 
-        by the following formula: (|X ∩ Y|/|X|)*(1-|X|/|N|) + (|(N \ X) \ Y|/|N \ X|) *
-        (1-|N \ X|/|N|)
-        default=False
-    dice_asymmetrici: bool
-        Boolean indicating whether the DiceAsymmetricI method should be used during 
-        the fuzzy name matching. The Dice asymmetric similarity is given be |X ∩ Y|/|X|
-        default=False
-    kuhns_iii: bool
-        Boolean indicating whether the KuhnsIII method should be used during the 
-        fuzzy name matching
-        default=False
-    overlap: bool
-        Boolean indicating whether the Overlap method should be used during the 
-        fuzzy name matching. The overlap distance is given by: |X ∩ Y|/min(|X|,|Y|)
-        default=True
-    pearson_ii: bool
-        Boolean indicating whether the PearsonII method should be used during the 
-        fuzzy name matching. This algorithm is based on the Phi coefficient or the 
-        mean square contingency
-        default=False
-    weighted_jaccard: bool
-        Boolean indicating whether the WeightedJaccard method should be used during 
-        the fuzzy name matching. This is the Jaccard distance only using a wheighing 
-        for the differences of 3.
-        default=True
-    warrens_iv: bool
-        Boolean indicating whether the WarrensIV method should be used during the 
-        fuzzy name matching
-        default=False
-    bag: bool
-        Boolean indicating whether the Bag method should be used during the fuzzy
-            name matching. Is a simplification of the regular edit distance by using
-            a similarity tree structure.
-        default=False
-    rouge_l: bool
-        Boolean indicating whether the ROUGE-L method should be used during the 
-        fuzzy name matching. The ROGUE-L method is a measure that counts the longest
-        substring between to strings
-        default=False
-    ratcliff_obershelp: bool
-        Boolean indicating whether the RatcliffObershelp method should be used 
-        during the fuzzy name matching. This method finds the longest common substring
-        and evaluates the longest common substrings to the right and the left of the 
-        original longest common substring
-        default=True
-    ncd_bz2: bool
-        Boolean indicating whether the NCDbz2 method should be used during the 
-        fuzzy name matching. Applies the Burrows-Wheeler transform to the strings and 
-        subsequently returns the normalised compression distance.
-        default=False
-    fuzzy_wuzzy_partial_string: bool
-        Boolean indicating whether the FuzzyWuzzyPartialString method should be used
-        during the fuzzy name matching. This methods takes the length of the longest 
-        common substring and divides it over the minimum of the length of each of 
-        the two strings.
-        default=False
-    fuzzy_wuzzy_token_sort: bool
-        Boolean indicating whether the FuzzyWuzzyTokenSort method should be used 
-        during the fuzzy name matching. This tokenizes the words in the string
-        and sorts them, subsequently a hamming distance is calculated
-        default=True
-    fuzzy_wuzzy_token_set: bool
-        Boolean indicating whether the FuzzyWuzzyTokenSet method should be used 
-        during the fuzzy name matching. This method tokenizes the strings and 
-        find the largest intersection of the two substrings and divides it over 
-        the length of the shortest string
-        default=False
-    editex: bool
-        Boolean indicating whether the Editex method should be used during the 
-        fuzzy name matching
-        default=True
-    typo: bool
-        Boolean indicating whether the Typo method should be used during the 
-        fuzzy name matching. The typo distance is calculated based on the distance
-        on a keyboard between edits.
-        default=False
-    lig_3: bool
-        Boolean indicating whether the LIG3 method should be used during the fuzzy 
-        name matching
-        default=False
-    ssk: bool
-        Boolean indicating whether the SSK method should be used during the fuzzy 
-        name matching. The ssk algorithm looks at the string kernel generated by all 
-        the possible different subsequences present between the two strings.
-        default=False
-    refined_soundex: bool
-        Boolean indicating whether the string should be represented by the RefinedSoundex
-        phonetix translation and the Levensthein distance of the translated strings should
-        be included in the fuzzy matching process
-        default=False
-    double_metaphone: bool
-        Boolean indicating whether the string should be represented by the DoubleMetaphone
-        phonetix translation and the Levensthein distance of the translated strings should
-        be included in the fuzzy matching process
-        default=False
-
-    """
-    distance_metrics = defaultdict(list)
-    if indel:
-        distance_metrics['Levenshtein'].append(Indel())
-    if discounted_levenshtein:
-        distance_metrics['Levenshtein'].append(
-            DiscountedLevenshtein())
-    if cormodel_z:
-        distance_metrics['block'].append(CormodeLZ())
-    if tichy:
-        distance_metrics['block'].append(Tichy())
-    if iterative_sub_string:
-        distance_metrics['Subsequence'].append(
-            IterativeSubString())
-    if baulieu_xiii:
-        distance_metrics['multiset'].append(BaulieuXIII())
-    if clement:
-        distance_metrics['multiset'].append(Clement())
-    if dice_asymmetrici:
-        distance_metrics['multiset'].append(DiceAsymmetricI())
-    if kuhns_iii:
-        distance_metrics['multiset'].append(KuhnsIII())
-    if overlap:
-        distance_metrics['multiset'].append(Overlap())
-    if pearson_ii:
-        distance_metrics['multiset'].append(PearsonII())
-    if weighted_jaccard:
-        distance_metrics['multiset'].append(WeightedJaccard())
-    if warrens_iv:
-        distance_metrics['multiset'].append(WarrensIV())
-    if bag:
-        distance_metrics['multiset'].append(Bag())
-    if rouge_l:
-        distance_metrics['multiset'].append(RougeL())
-    if ratcliff_obershelp:
-        distance_metrics['Subsequence'].append(
-            RatcliffObershelp())
-    if ncd_bz2:
-        distance_metrics['compression'].append(NCDbz2())
-    if fuzzy_wuzzy_partial_string:
-        distance_metrics['fuzzy'].append(
-            FuzzyWuzzyPartialString())
-    if fuzzy_wuzzy_token_sort:
-        distance_metrics['fuzzy'].append(FuzzyWuzzyTokenSort())
-    if fuzzy_wuzzy_token_set:
-        distance_metrics['fuzzy'].append(FuzzyWuzzyTokenSet())
-    if editex:
-        distance_metrics['edit'].append(Editex())
-    if typo:
-        distance_metrics['edit'].append(Typo())
-    if lig_3:
-        distance_metrics['Levenshtein'].append(LIG3())
-    if ssk:
-        distance_metrics['Subsequence'].append(SSK())
-    if refined_soundex:
-        distance_metrics['phonetic'].append(PhoneticDistance(
-            transforms=RefinedSoundex(max_length=30), metric=Levenshtein(), encode_alpha=True))
-    if double_metaphone:
-        distance_metrics['phonetic'].append(PhoneticDistance(
-            transforms=DoubleMetaphone(max_length=30), metric=Levenshtein(), encode_alpha=True))
-
-    return distance_metrics
+from distances import Indel, DiscountedLevenshtein, CormodeLZ, Tichy, IterativeSubString, BaulieuXIII, Clement, DiceAsymmetricI, KuhnsIII, Overlap, PearsonII, WeightedJaccard, WarrensIV, Bag, RougeL, RatcliffObershelp, NCDbz2, FuzzyWuzzyPartialString, FuzzyWuzzyTokenSort, FuzzyWuzzyTokenSet, Editex, Typo,LIG3, SSK, Levenshtein, DoubleMetaphone, RefinedSoundex, PhoneticDistance
+from collections import defaultdict
+
+def make_distance_metrics(indel=False,
+                          discounted_levenshtein=False,
+                          tichy=False,
+                          cormodel_z=False,
+                          iterative_sub_string=False,
+                          baulieu_xiii=False,
+                          clement=False,
+                          dice_asymmetrici=False,
+                          kuhns_iii=False,
+                          overlap=False,
+                          pearson_ii=False,
+                          weighted_jaccard=False,
+                          warrens_iv=False,
+                          bag=False,
+                          rouge_l=False,
+                          ratcliff_obershelp=False,
+                          ncd_bz2=False,
+                          fuzzy_wuzzy_partial_string=False,
+                          fuzzy_wuzzy_token_sort=False,
+                          fuzzy_wuzzy_token_set=False,
+                          editex=False,
+                          typo=False,
+                          lig_3=False,
+                          ssk=False,
+                          refined_soundex=False,
+                          double_metaphone=False) -> dict:
+    r"""
+    A function which returns a dict containing the distance metrics that should be 
+    used during the fuzzy string matching
+
+    Levenshtein edit distance
+        - Indel
+        - Discounted Levenshtein
+        - LIG3
+    Block edit distances
+        - Tichy
+        - CormodeLZ
+    Multi-set token-based distance
+        - BaulieuXIII
+        - Clement
+        - DiceAsymmetricI
+        - KuhnsIII
+        - Overlap
+        - PearsonII
+        - WeightedJaccard
+        - WarrensIV
+        - Bag
+        - RougeL
+    Subsequence distances
+        - IterativeSubString
+        - RatcliffObershelp
+        - SSK
+    Normalized compression distance
+        - NCDbz2
+    FuzzyWuzzy distances
+        - FuzzyWuzzyPartialString
+        - FuzzyWuzzyTokenSort
+        - FuzzyWuzzyTokenSet
+    Ponetic distances
+        - RefinedSoundex
+        - DoubleMetaphone
+    Edit distances
+        - Editex
+        - Typo
+
+
+    Parameters
+    ----------
+    indel: bool
+        Boolean indicating whether the Indel method should be used during the 
+        fuzzy name matching. The indel method is equal to a regular levenshtein 
+        distance with a twice as high substitution weight 
+        default=False
+    discounted_levenshtein: bool
+        Boolean indicating whether the DiscountedLevenshtein method should be used 
+        during the fuzzy name matching. Equal to the regular levenshtein distance,
+        only errors later in the string are counted at a discounted rate. To for
+        instance limit the importance of suffix differences
+        default=False
+    tichy: bool
+        Boolean indicating whether the Tichy method should be used during the 
+        fuzzy name matching. This algorithm provides a shortest edit distance based
+        on substring and add operations.
+        default=False
+    cormodel_z: bool
+        Boolean indicating whether the CormodeLZ method should be used during the 
+        fuzzy name matching. The CormodeLZ distance between strings x and y, is the 
+        minimum number of single characters or substrings of y or of the partially 
+        built string which are required to produce x from left to right.
+        default=False
+    iterative_sub_string: bool
+        Boolean indicating whether the IterativeSubString method should be used 
+        during the fuzzy name matching. A method that counts the similarities 
+        between two strings substrings and subtracts the differences taking into
+        account the winkler similarity between the string and the substring.
+        default=False
+    baulieu_xiii: bool
+        Boolean indicating whether the BaulieuXIII method should be used during 
+        the fuzzy name matching. The Baulieu XIII distance between two strings is
+        given by the following formula: (|X \ Y| + |Y \ X|) / (
+        |X ∩ Y| + |X \ Y| + |Y \ X| + |X ∩ Y| ∙ (|X ∩ Y| - 4)^2)
+        default=False
+    clement: bool
+        Boolean indicating whether the Clement method should be used during the
+        fuzzy name matching. The Clement distance between two strings is given 
+        by the following formula: (|X ∩ Y|/|X|)*(1-|X|/|N|) + (|(N \ X) \ Y|/|N \ X|) *
+        (1-|N \ X|/|N|)
+        default=False
+    dice_asymmetrici: bool
+        Boolean indicating whether the DiceAsymmetricI method should be used during 
+        the fuzzy name matching. The Dice asymmetric similarity is given be |X ∩ Y|/|X|
+        default=False
+    kuhns_iii: bool
+        Boolean indicating whether the KuhnsIII method should be used during the 
+        fuzzy name matching
+        default=False
+    overlap: bool
+        Boolean indicating whether the Overlap method should be used during the 
+        fuzzy name matching. The overlap distance is given by: |X ∩ Y|/min(|X|,|Y|)
+        default=True
+    pearson_ii: bool
+        Boolean indicating whether the PearsonII method should be used during the 
+        fuzzy name matching. This algorithm is based on the Phi coefficient or the 
+        mean square contingency
+        default=False
+    weighted_jaccard: bool
+        Boolean indicating whether the WeightedJaccard method should be used during 
+        the fuzzy name matching. This is the Jaccard distance only using a wheighing 
+        for the differences of 3.
+        default=True
+    warrens_iv: bool
+        Boolean indicating whether the WarrensIV method should be used during the 
+        fuzzy name matching
+        default=False
+    bag: bool
+        Boolean indicating whether the Bag method should be used during the fuzzy
+            name matching. Is a simplification of the regular edit distance by using
+            a similarity tree structure.
+        default=False
+    rouge_l: bool
+        Boolean indicating whether the ROUGE-L method should be used during the 
+        fuzzy name matching. The ROGUE-L method is a measure that counts the longest
+        substring between to strings
+        default=False
+    ratcliff_obershelp: bool
+        Boolean indicating whether the RatcliffObershelp method should be used 
+        during the fuzzy name matching. This method finds the longest common substring
+        and evaluates the longest common substrings to the right and the left of the 
+        original longest common substring
+        default=True
+    ncd_bz2: bool
+        Boolean indicating whether the NCDbz2 method should be used during the 
+        fuzzy name matching. Applies the Burrows-Wheeler transform to the strings and 
+        subsequently returns the normalised compression distance.
+        default=False
+    fuzzy_wuzzy_partial_string: bool
+        Boolean indicating whether the FuzzyWuzzyPartialString method should be used
+        during the fuzzy name matching. This methods takes the length of the longest 
+        common substring and divides it over the minimum of the length of each of 
+        the two strings.
+        default=False
+    fuzzy_wuzzy_token_sort: bool
+        Boolean indicating whether the FuzzyWuzzyTokenSort method should be used 
+        during the fuzzy name matching. This tokenizes the words in the string
+        and sorts them, subsequently a hamming distance is calculated
+        default=True
+    fuzzy_wuzzy_token_set: bool
+        Boolean indicating whether the FuzzyWuzzyTokenSet method should be used 
+        during the fuzzy name matching. This method tokenizes the strings and 
+        find the largest intersection of the two substrings and divides it over 
+        the length of the shortest string
+        default=False
+    editex: bool
+        Boolean indicating whether the Editex method should be used during the 
+        fuzzy name matching
+        default=True
+    typo: bool
+        Boolean indicating whether the Typo method should be used during the 
+        fuzzy name matching. The typo distance is calculated based on the distance
+        on a keyboard between edits.
+        default=False
+    lig_3: bool
+        Boolean indicating whether the LIG3 method should be used during the fuzzy 
+        name matching
+        default=False
+    ssk: bool
+        Boolean indicating whether the SSK method should be used during the fuzzy 
+        name matching. The ssk algorithm looks at the string kernel generated by all 
+        the possible different subsequences present between the two strings.
+        default=False
+    refined_soundex: bool
+        Boolean indicating whether the string should be represented by the RefinedSoundex
+        phonetix translation and the Levensthein distance of the translated strings should
+        be included in the fuzzy matching process
+        default=False
+    double_metaphone: bool
+        Boolean indicating whether the string should be represented by the DoubleMetaphone
+        phonetix translation and the Levensthein distance of the translated strings should
+        be included in the fuzzy matching process
+        default=False
+
+    """
+    distance_metrics = defaultdict(list)
+    if indel:
+        distance_metrics['Levenshtein'].append(Indel())
+    if discounted_levenshtein:
+        distance_metrics['Levenshtein'].append(
+            DiscountedLevenshtein())
+    if cormodel_z:
+        distance_metrics['block'].append(CormodeLZ())
+    if tichy:
+        distance_metrics['block'].append(Tichy())
+    if iterative_sub_string:
+        distance_metrics['Subsequence'].append(
+            IterativeSubString())
+    if baulieu_xiii:
+        distance_metrics['multiset'].append(BaulieuXIII())
+    if clement:
+        distance_metrics['multiset'].append(Clement())
+    if dice_asymmetrici:
+        distance_metrics['multiset'].append(DiceAsymmetricI())
+    if kuhns_iii:
+        distance_metrics['multiset'].append(KuhnsIII())
+    if overlap:
+        distance_metrics['multiset'].append(Overlap())
+    if pearson_ii:
+        distance_metrics['multiset'].append(PearsonII())
+    if weighted_jaccard:
+        distance_metrics['multiset'].append(WeightedJaccard())
+    if warrens_iv:
+        distance_metrics['multiset'].append(WarrensIV())
+    if bag:
+        distance_metrics['multiset'].append(Bag())
+    if rouge_l:
+        distance_metrics['multiset'].append(RougeL())
+    if ratcliff_obershelp:
+        distance_metrics['Subsequence'].append(
+            RatcliffObershelp())
+    if ncd_bz2:
+        distance_metrics['compression'].append(NCDbz2())
+    if fuzzy_wuzzy_partial_string:
+        distance_metrics['fuzzy'].append(
+            FuzzyWuzzyPartialString())
+    if fuzzy_wuzzy_token_sort:
+        distance_metrics['fuzzy'].append(FuzzyWuzzyTokenSort())
+    if fuzzy_wuzzy_token_set:
+        distance_metrics['fuzzy'].append(FuzzyWuzzyTokenSet())
+    if editex:
+        distance_metrics['edit'].append(Editex())
+    if typo:
+        distance_metrics['edit'].append(Typo())
+    if lig_3:
+        distance_metrics['Levenshtein'].append(LIG3())
+    if ssk:
+        distance_metrics['Subsequence'].append(SSK())
+    if refined_soundex:
+        distance_metrics['phonetic'].append(PhoneticDistance(
+            transforms=RefinedSoundex(max_length=30), metric=Levenshtein(), encode_alpha=True))
+    if double_metaphone:
+        distance_metrics['phonetic'].append(PhoneticDistance(
+            transforms=DoubleMetaphone(max_length=30), metric=Levenshtein(), encode_alpha=True))
+
+    return distance_metrics
```

### Comparing `name_matching-0.8.8/name_matching/name_matcher.py` & `name_matching-0.8.9/name_matching/name_matcher.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,750 +1,747 @@
-import unicodedata
-import functools
-import operator
-import re
-import numpy as np
-import pandas as pd
-from tqdm import tqdm
-from typing import Union, Tuple
-from itertools import compress
-from sklearn.feature_extraction.text import TfidfVectorizer
-from name_matching.distance_metrics import make_distance_metrics
-from cleanco.termdata import terms_by_type, terms_by_country
-from name_matching.sparse_cosine import sparse_cosine_top_n
-
-
-class NameMatcher:
-
-    """
-    A class for the name matching of data based on the strings in a single column. The NameMatcher
-    first applies a cosine similarity on the ngrams of the strings to get an approximate match followed 
-    by a fuzzy matching based on a number of different algorithms.
-
-    Parameters
-    ----------
-    ngrams : tuple of integers
-        The length of the ngrams which should be used for the generation of ngrams for the cosine
-        similarity comparison of the possible matches
-        default=(2, 3)
-    top_n : integer
-        The number of possible matches that should be included in the group which will be analysed
-        with the fuzzy matching algorithms
-        default=50
-    low_memory : bool
-        Bool indicating if the a low memory approach should be taken in the sparse cosine similarity
-        step.
-        default=False
-    number_of_rows : integer
-        Determines how many rows should be calculated at once with the sparse cosine similarity step.
-        If the low_memory bool is True this number is unused.
-        default=5000
-    number_of_matches : int
-        The number of matches which should be returned by the matching algorithm. If a number higher
-        than 1 is given, a number of alternative matches are also returned. If the number is equal
-        to the number of algorithms used, the best match for each algorithm is returned. If the
-        number is equal to the number of algorithm groups which are included the best match for each
-        group is returned.
-        default=1
-    legal_suffixes : bool
-        Boolean indicating whether the most common company legal terms should be excluded when calculating 
-        the final score. The terms are still included in determining the best match.
-        default=False
-    common_words : bool
-        Boolean indicating whether the most common words from the matching data should be excluded 
-        when calculating the final score. The terms are still included in determining the best match.
-        default=False
-    cut_off_no_scoring_words: float
-        the cut off percentage of the occurrence of the most occurring word for which words are still included 
-        in the no_soring_words set
-        default=0.01
-    lowercase : bool
-        A boolean indicating whether during the preprocessing all characters should be converted to
-        lowercase, to generate case insensitive matching
-        default=True
-    punctuations : bool
-        A boolean indicating whether during the preprocessing all punctuations should be ignored
-        default=True
-    remove_ascii : bool
-        A boolean indicating whether during the preprocessing all characters should be converted to
-        ascii characters
-        default=True : bool
-    preprocess_split
-        Indicating whether during the preprocessing an additional step should be taken in which only 
-        the most common words out of a name are isolated and used in the matching process. The removing 
-        of the common words is only done for the n-grams cosine matching part.
-        default=False
-    verbose : bool
-        A boolean indicating whether progress printing should be done
-        default=True
-    distance_metrics: list
-        A list of The distance metrics to be used during the fuzzy matching. For a list of possible distance
-        metrics see the distance_metrics.py file. By default the following metrics are used: overlap, weighted_jaccard, 
-                ratcliff_obershelp, fuzzy_wuzzy_token_sort and editex.
-    row_numbers : bool
-        Bool indicating whether the row number should be used as match_index rather than the original index as
-        was the default case before version 0.8.8  
-        default=False
-    """
-
-    def __init__(self,
-                 ngrams: tuple = (2, 3),
-                 top_n: int = 50,
-                 low_memory: bool = False,
-                 number_of_rows: int = 5000,
-                 number_of_matches: int = 1,
-                 lowercase: bool = True,
-                 punctuations: bool = True,
-                 remove_ascii: bool = True,
-                 legal_suffixes: bool = False,
-                 common_words: bool = False,
-                 cut_off_no_scoring_words: float = 0.01,
-                 preprocess_split: bool = False,
-                 verbose: bool = True,
-                 distance_metrics: Union[list, tuple] = ['overlap', 'weighted_jaccard', 'ratcliff_obershelp',
-                                                         'fuzzy_wuzzy_token_sort', 'editex'],
-                 row_numbers: bool = False):
-
-        self._possible_matches = None
-        self._preprocessed = False
-        self._word_set = set()
-        self._df_matching_data = pd.DataFrame()
-
-        self._number_of_rows = number_of_rows
-        self._low_memory = low_memory
-
-        self._column = ''
-        self._column_matching = ''
-
-        self._verbose = verbose
-        self._number_of_matches = number_of_matches
-        self._top_n = top_n
-
-        self._preprocess_lowercase = lowercase
-        self._preprocess_punctuations = punctuations
-        self._preprocess_ascii = remove_ascii
-        self._postprocess_company_legal_id = legal_suffixes
-        self._postprocess_common_words = common_words
-
-        self._preprocess_common_words = pd.Series(dtype=float)
-        self._preprocess_split = preprocess_split
-        self._cut_off = cut_off_no_scoring_words
-
-        if self._postprocess_company_legal_id:
-            self._word_set = self._make_no_scoring_words(
-                'legal', self._word_set, self._cut_off)
-            
-        self._original_indexes = not row_numbers
-
-        self.set_distance_metrics(distance_metrics)
-
-        self._vec = TfidfVectorizer(
-            lowercase=False, analyzer="char", ngram_range=(ngrams))
-        self._n_grams_matching = None
-
-    def set_distance_metrics(self, metrics: list) -> None:
-        """
-        A method to set which of the distance metrics should be employed during the
-        fuzzy matching. For very short explanations of most of the name matching 
-        algorithms please see the make_distance_metrics function in distance_matrics.py
-
-        Parameters
-        ----------
-        metrics: list 
-            The list with the distance metrics to be used during the name matching. The
-            distance metrics can be chosen from the list below:
-                indel
-                discounted_levenshtein
-                tichy
-                cormodeL_z
-                iterative_sub_string
-                baulieu_xiii
-                clement
-                dice_asymmetricI
-                kuhns_iii
-                overlap
-                pearson_ii
-                weighted_jaccard
-                warrens_iv
-                bag
-                rouge_l
-                ratcliff_obershelp
-                ncd_bz2
-                fuzzy_wuzzy_partial_string
-                fuzzy_wuzzy_token_sort
-                fuzzy_wuzzy_token_set
-                editex
-                typo
-                lig_3
-                ssk
-                refined_soundex
-                double_metaphone
-        """
-
-        input_metrics = {str(metric).lower(): True for metric in metrics}
-        try:
-            self._distance_metrics = make_distance_metrics(**input_metrics)
-        except TypeError:
-            raise TypeError('Not all of the supplied distance metrics are available. Please check the' +
-                            'list of options in the make_distance_metrics function and adjust your list accordingly')
-        self._num_distance_metrics = sum(
-            [len(x) for x in self._distance_metrics.values()])
-
-    def _select_top_words(self, word: str, word_counts: pd.Series, occurrence_count: int) -> str:
-        """Remove the top words from the string word based on an occurrence_count threshold
-
-        Parameters
-        ----------
-        word: str 
-            the string from which the words should be removed
-        word_counts: pd.Series
-            the words which should be removed with their counts as result from a value_counts
-        occurrence_count: int 
-            the multiplication factor of the minimum occurrences below which to select 
-
-        Returns
-        -------
-        str
-           The string word with the words with a too high word_counts removed
-        """
-        compressed_list = list(compress(
-            word, (word_counts[word] < occurrence_count*word_counts[word].min()).values))
-
-        return ' '.join(compressed_list)
-
-    def _preprocess_reduce(self,
-                           to_be_matched: pd.DataFrame,
-                           occurrence_count: int = 3) -> pd.DataFrame:
-        """Preprocesses and copies the data to obtain the data with reduced strings. The strings have all words
-        removed which appear more than 3x as often as the least common word in the string and returns an adjusted 
-        copy of the input 
-
-        Parameters
-        ----------
-        to_be_matched: pd.DataFrame 
-            A dataframe from which the most common words should be removed
-        occurrence_count: int
-            The number of occurrence a word can occur more then the least common word in the string for which it will
-            still be included in the process 
-            default=3
-
-        Returns
-        -------
-        pd.DataFrame
-            A dataframe that will contain the reduced strings
-        """
-        individual_words = to_be_matched[self._column_matching].str.split(
-            expand=True).stack()
-        word_counts = individual_words.value_counts()
-        preprocess_common_words_inst = pd.concat([self._preprocess_common_words,
-            word_counts]).fillna(0)
-        to_be_matched_new = to_be_matched.copy()
-        name = to_be_matched[self._column_matching].str.split()
-        to_be_matched_new[self._column_matching] = name.apply(
-            lambda word: self._select_top_words(word, preprocess_common_words_inst, occurrence_count))
-
-        return to_be_matched_new
-
-    def load_and_process_master_data(self,
-                                     column: str,
-                                     df_matching_data: pd.DataFrame,
-                                     start_processing: bool = True,
-                                     transform: bool = True) -> None:
-        """Load the matching data into the NameMatcher and start the preprocessing.
-
-        Parameters
-        ----------
-        column : string
-            The column name of the dataframe which should be used for the matching
-        df_matching_data: pd.DataFrame
-            The dataframe which is used to match the data to.
-        start_processing : bool 
-            A boolean indicating whether to start the preprocessing step after loading the matching data 
-            default: True
-        transform : bool 
-            A boolean indicating whether or not the data should be transformed after the vectoriser is initialised 
-            default: True
-        """
-        self._column = column
-        self._df_matching_data = df_matching_data
-        if start_processing:
-            self._process_matching_data(transform)
-
-    def _process_matching_data(self,
-                               transform: bool = True) -> None:
-        """Function to process the matching data. First the matching data is preprocessed and assigned to 
-        a variable within the NameMatcher. Next the data is used to initialise the TfidfVectorizer. 
-
-        Parameters
-        ----------
-        transform : bool 
-            A boolean indicating whether or not the data should be transformed after the vectoriser is initialised 
-            default: True
-        """
-        self._df_matching_data = self.preprocess(
-            self._df_matching_data, self._column)
-        if self._postprocess_common_words:
-            self._word_set = self._make_no_scoring_words(
-                'common', self._word_set, self._cut_off)
-        self._vectorise_data(transform)
-        self._preprocessed = True
-
-    def match_names(self,
-                    to_be_matched: Union[pd.Series, pd.DataFrame],
-                    column_matching: str) -> Union[pd.Series, pd.DataFrame]:
-        """Performs the name matching operation on the to_be_matched data. First it does the preprocessing of the 
-        data to be matched as well as the matching data if this has not been performed. Subsequently based on 
-        ngrams a cosine similarity is computed between the matching data and the data to be matched, to the top n
-        matches fuzzy matching algorithms are performed to determine the best match and the quality of the match
-
-        Parameters
-        ----------
-        to_be_matched: Union[pd.Series, pd.DataFrame]
-            The data which should be matched
-        column_matching: str
-            string indicating the column which will be matched
-
-        Returns
-        -------
-        Union[pd.Series, pd.DataFrame]
-            A series or dataframe depending on the input containing the match index from the matching_data dataframe. 
-            the name in the to_be_matched data, the name to which the datapoint was matched and a score between 0 
-            (no match) and 100(perfect match) to indicate the quality of the matches
-        """
-        if self._column == '':
-            raise ValueError(
-                'Please first load the master data via the method: load_and_process_master_data')
-        if self._verbose:
-            tqdm.pandas()
-            tqdm.write('preprocessing...\n')
-        self._column_matching = column_matching
-
-        is_dataframe = True
-        if isinstance(to_be_matched, pd.Series):
-            is_dataframe = False
-            to_be_matched = pd.DataFrame(
-                [to_be_matched.values], columns=to_be_matched.index.to_list())
-        if not self._preprocessed:
-            self._process_matching_data()
-        to_be_matched = self.preprocess(to_be_matched, self._column_matching)
-
-        original_index = to_be_matched.index
-
-        if self._verbose:
-            tqdm.write('preprocessing complete \n searching for matches...\n')
-
-        self._possible_matches = self._search_for_possible_matches(
-            to_be_matched)
-
-        if self._preprocess_split:
-            self._possible_matches = np.hstack((self._search_for_possible_matches(
-                self._preprocess_reduce(to_be_matched)), self._possible_matches))
-
-        if self._verbose:
-            tqdm.write('possible matches found   \n fuzzy matching...\n')
-            data_matches = to_be_matched.progress_apply(lambda x: self.fuzzy_matches(
-                self._possible_matches[to_be_matched.index.get_loc(x.name), :], x), axis=1)
-        else:
-            data_matches = to_be_matched.apply(lambda x: self.fuzzy_matches(
-                self._possible_matches[to_be_matched.index.get_loc(x.name), :], x), axis=1)
-
-        if self._number_of_matches == 1:
-            data_matches = data_matches.rename(columns={'match_name_0': 'match_name',
-                                                        'score_0': 'score', 'match_index_0': 'match_index'})
-        if is_dataframe and self._original_indexes:
-            for col in data_matches.columns[data_matches.columns.str.contains('match_index')]:
-                data_matches[col] = original_index[data_matches[col].astype(int).fillna(0)]
-
-        if self._verbose:
-            tqdm.write('done')
-
-        return data_matches
-
-    def fuzzy_matches(self,
-                      possible_matches: np.array,
-                      to_be_matched: pd.Series) -> pd.Series:
-        """ A method which performs the fuzzy matching between the data in the to_be_matched series as well
-        as the indicated indexes of the matching_data points which are possible matching candidates.
-
-        Parameters
-        ----------
-        possible_matches : np.array
-            An array containing the indexes of the matching data with potential matches
-        to_be_matched : pd.Series
-            The data which should be matched
-
-        Returns
-        -------
-        pd.Series
-            A series containing the match index from the matching_data dataframe. the name in the to_be_matched data,
-            the name to which the datapoint was matched and a score between 0 (no match) and 100(perfect match) to 
-            indicate the quality of the matches
-        """
-        if len(possible_matches.shape) > 1:
-            possible_matches = possible_matches[0]
-
-        indexes = np.array([[f'match_name_{num}', f'score_{num}', f'match_index_{num}']
-                            for num in range(self._number_of_matches)]).flatten()
-        match = pd.Series(index=np.append('original_name', indexes), dtype=float)
-        match['original_name'] = to_be_matched[self._column_matching]
-        list_possible_matches = self._df_matching_data.iloc[
-            possible_matches.flatten(), :][self._column].values
-
-        match_score = self._score_matches(
-            to_be_matched[self._column_matching], list_possible_matches)
-        ind = self._rate_matches(match_score)
-
-        for num, col_num in enumerate(ind):
-            match[f'match_name_{num}'] = list_possible_matches[col_num]
-            match[f'match_index_{num}'] = possible_matches[col_num]
-
-        match = self._adjust_scores(match_score[ind, :], match)
-
-        if self._postprocess_common_words or self._postprocess_company_legal_id:
-            match = self.postprocess(match)
-
-        return match
-
-    def _score_matches(self,
-                       to_be_matched_instance: str,
-                       possible_matches: list) -> np.array:
-        """A method to score a name to_be_matched_instance to a list of possible matches. The scoring is done
-        based on all the metrics which are enabled.
-
-        Parameters
-        ----------
-        to_be_matched_instance : str
-            The name which should match one of the possible matches
-        possible_matches : list
-            list of the names of the possible matches
-
-        Returns
-        -------
-        np.array
-            The score of each of the matches with respect to the different metrics which are assessed.
-        """
-        match_score = np.zeros(
-            (len(possible_matches), self._num_distance_metrics))
-        idx = 0
-        for method_list in self._distance_metrics.values():
-            for method in method_list:
-                match_score[:, idx] = np.array(
-                    [method.sim(to_be_matched_instance, s) for s in possible_matches])
-                idx = idx + 1
-
-        return match_score
-
-    def _rate_matches(self,
-                      match_score: np.array) -> np.array:
-        """Converts the match scores from the score_matches method to a list of indexes of the best scoring 
-        matches limited to the _number_of_matches.
-
-        Parameters
-        ----------
-        match_score : np.array
-            An array containing the scores of each of the possible alternatives for each
-            of the different methods used
-
-        Returns
-        -------
-        np.array
-            The indexes of the best rated matches
-        """
-        if self._number_of_matches == 1:
-            ind = [np.argmax(np.mean(match_score, axis=1))]
-        elif self._number_of_matches == len(self._distance_metrics):
-            ind = np.zeros(len(self._distance_metrics))
-            idx = 0
-            for num, method_list in enumerate(self._distance_metrics.values()):
-                method_grouped_results = np.reshape(
-                    match_score[:, idx: idx + len(method_list)], (-1, len(method_list)))
-                ind[num] = np.argmax(np.mean(method_grouped_results, axis=1))
-                idx = idx + len(method_list)
-        elif self._number_of_matches == self._num_distance_metrics:
-            ind = np.argmax(match_score, axis=1)
-        else:
-            ind = np.argsort(np.mean(match_score, axis=1)
-                             )[-self._number_of_matches:][::-1]
-
-        return np.array(ind, dtype=int)
-
-    def _get_alternative_names(self, match: pd.Series) -> list:
-        """Gets all the possible match names from the match.
-
-        Parameters
-        ----------
-        match : pd.Series
-            The series with the possible matches and original scores
-
-        Returns
-        -------
-        list
-            A list with the alternative names for this match
-        """
-        alt_names = []
-
-        for num in range(self._number_of_matches):
-            alt_names.append(str(match[f'match_name_{num}']))
-
-        return alt_names
-
-    def _process_words(self, org_name: str, alt_names: list) -> Tuple[str, list]:
-        """Removes the words from the word list from the org_name and all the names in alt_names .
-
-        Parameters
-        ----------
-        org_name : str
-            The original name for the matching data
-        alt_names : list
-            A list of names from which the words should be removed
-
-        Returns
-        -------
-        Tuple[str, list]
-            The processed version of the org_name and the alt_names, with the words removed
-        """
-        len_atl_names = len(alt_names)
-        for word in self._word_set:
-            org_name = ' '.join(
-                re.sub(fr'\b{re.escape(word)}\b', '', org_name).split())
-            for num in range(len_atl_names):
-                alt_names[num] = ' '.join(
-                    re.sub(fr'\b{re.escape(word)}\b', '', alt_names[num]).split())
-
-        return org_name, alt_names
-
-    def _adjust_scores(self, match_score: np.array, match: pd.Series) -> pd.Series:
-        """Adjust the scores to be between 0 and 100
-
-        Parameters
-        ----------
-        match_score : np.array
-            An array with the scores for each of the options
-        match : pd.Series
-            The series with the possible matches and original scores
-
-        Returns
-        -------
-        pd.Series
-            The series with the possible matches and adjusted scores
-        """
-        for num in range(self._number_of_matches):
-            match[f'score_{num}'] = 100*np.mean(match_score[num, :])
-
-        return match
-
-    def postprocess(self,
-                    match: pd.Series) -> pd.Series:
-        """Postprocesses the scores to exclude certain specific company words or the most 
-        common words. In this method only the scores are adjusted, the matches still stand.
-
-        Parameters
-        ----------
-        match : pd.Series
-            The series with the possible matches and original scores
-
-        Returns
-        -------
-        pd.Series
-            A new version of the input series with updated scores
-        """
-        alt_names = self._get_alternative_names(match)
-        org_name = str(match['original_name'])
-
-        org_name, alt_names = self._process_words(org_name, alt_names)
-
-        match_score = self._score_matches(org_name, alt_names)
-
-        match = self._adjust_scores(match_score, match)
-
-        return match
-
-    def _vectorise_data(self,
-                        transform: bool = True):
-        """Initialises the TfidfVectorizer, which generates ngrams and weights them based on the occurrance.
-        Subsequently the matching data will be used to fit the vectoriser and the matching data might also be send
-        to the transform_data function depending on the transform boolean.
-
-        Parameters
-        ----------
-        transform : bool 
-            A boolean indicating whether or not the data should be transformed after the vectoriser is initialised 
-            default: True
-        """
-        self._vec.fit(self._df_matching_data[self._column].values.flatten())
-        if transform:
-            self.transform_data()
-
-    def transform_data(self):
-        """A method which transforms the matching data based on the ngrams transformer. After the 
-        transformation (the generation of the ngrams), the data is normalised by dividing each row
-        by the sum of the row. Subsequently the data is changed to a coo sparse matrix format with
-        the column indices in ascending order.
-        """
-        ngrams = self._vec.transform(
-            self._df_matching_data[self._column].astype(str))
-        for i, j in zip(ngrams.indptr[:-1], ngrams.indptr[1:]):
-            ngrams.data[i:j] = ngrams.data[i:j]/np.sum(ngrams.data[i:j])
-        self._n_grams_matching = ngrams.tocsc()
-        if self._low_memory:
-            self._n_grams_matching = self._n_grams_matching.tocoo()
-
-    def _search_for_possible_matches(self,
-                                     to_be_matched: pd.DataFrame) -> np.array:
-        """Generates ngrams from the data which should be matched, calculate the cosine simularity
-        between these data and the matching data. Hereafter a top n of the matches is selected and
-        returned.
-
-        Parameters
-        ----------
-        to_be_matched : pd.Series
-            A series containing a single instance of the data to be matched
-
-        Returns
-        -------
-        np.array
-            An array of top n values which are most closely matched to the to be matched data based
-            on the ngrams
-        """
-        if self._n_grams_matching is None:
-            raise RuntimeError(
-                """First the data needs to be transformed to be able to use the sparse cosine simularity. To""" +
-                """transform the data, run transform_data or run load_and_process_master_data with transform=True""")
-
-        if self._low_memory:
-            results = np.zeros((len(to_be_matched), self._top_n))
-            input_data = to_be_matched[self._column_matching]
-            for idx, row_name in enumerate(tqdm(input_data, disable=not self._verbose)):
-                match_ngrams = self._vec.transform([row_name])
-                results[idx, :] = sparse_cosine_top_n(
-                    matrix_a=self._n_grams_matching, matrix_b=match_ngrams, top_n=self._top_n, low_memory=self._low_memory, number_of_rows=self._number_of_rows, verbose=self._verbose)
-        else:
-            match_ngrams = self._vec.transform(
-                to_be_matched[self._column_matching].tolist()).tocsc()
-            results = sparse_cosine_top_n(
-                matrix_a=self._n_grams_matching, matrix_b=match_ngrams, top_n=self._top_n, low_memory=self._low_memory, number_of_rows=self._number_of_rows, verbose=self._verbose)
-
-        return results
-
-    def preprocess(self,
-                   df: pd.DataFrame,
-                   column_name: str) -> pd.DataFrame:
-        """Preprocess a dataframe before applying a name matching algorithm. The preprocessing consists of 
-        removing special characters, spaces, converting all characters to lower case and removing the
-        words given in the word lists
-
-        Parameters
-        ----------
-        df : DataFrame
-            The dataframe or series on which the preprocessing needs to be performed        
-        column_name : str
-            The name of the column that is used for the preprocessing
-
-        Returns
-        -------
-        pd.DataFrame
-            The preprocessed dataframe or series depending on the input
-        """
-        df.loc[:, column_name] = df[column_name].astype(str)
-        if self._preprocess_lowercase:
-            df.loc[:, column_name] = df[column_name].str.lower()
-        if self._preprocess_punctuations:
-            df.loc[:, column_name] = df[column_name].str.replace(
-                '[^\w\s]', '', regex=True)
-            df.loc[:, column_name] = df[column_name].str.replace(
-                '  ', ' ').str.strip()
-        if self._preprocess_ascii:
-            df.loc[:, column_name] = df[column_name].apply(lambda string: unicodedata.normalize(
-                'NFKD', str(string)).encode('ASCII', 'ignore').decode())
-
-        return df
-
-    def _preprocess_word_list(self, terms: dict) -> list:
-        """Preprocess legal words to remove punctuations and trailing leading space
-
-        Parameters
-        -------
-        terms: dict
-            a dictionary of legal words
-
-        Returns
-        -------
-        list
-            A list of preprocessed legal words  
-        """
-        if self._preprocess_punctuations:
-            return [re.sub(r'[^\w\s]', '', s).strip() for s in functools.reduce(
-                operator.iconcat, terms.values(), [])]
-        else:
-            return [s.strip() for s in functools.reduce(
-                    operator.iconcat, terms.values(), [])]
-
-    def _process_legal_words(self, word_set: set) -> set:
-        """Preprocess legal words and add them to the word_set
-
-        Parameters
-        -------
-        word_set: str
-            the current word list which should be extended with additional words
-
-        Returns
-        -------
-        Set
-            The original word_set with the legal words added
-        """
-        terms_type = self._preprocess_word_list(terms_by_type)
-        terms_country = self._preprocess_word_list(terms_by_country)
-        word_set = word_set.union(set(terms_country + terms_type))
-
-        return word_set
-
-    def _process_common_words(self, word_set: set, cut_off: float) -> set:
-        """A method to select the most common words from the matching_data.
-
-        Parameters
-        -------
-        word_set: str
-            the current word list which should be extended with additional words  
-        cut_off: float
-            the cut_off percentage of the occurrence of the most occurring word for which words are still included 
-            in the no_soring_words set
-
-        Returns
-        -------
-        Set
-            The current word set with the most common words from the matching_data added
-        """
-        word_counts = self._df_matching_data[self._column].str.split(
-            expand=True).stack().value_counts()
-        word_set = word_set.union(
-            set(word_counts[word_counts > np.max(word_counts)*cut_off].index))
-
-        return word_set
-
-    def _make_no_scoring_words(self,
-                               indicator: str,
-                               word_set: set,
-                               cut_off: float) -> set:
-        """A method to make a set of words which are not taken into account when scoring matches.
-
-        Parameters
-        -------
-        indicator: str
-            indicator for which types of words should be excluded can be legal for
-            legal suffixes or common for the most common words
-        word_set: str
-            the current word list which should be extended with additional words  
-        cut_off: float
-            the cut_off percentage of the occurrence of the most occurring word for which words are still included 
-            in the no_soring_words set
-
-        Returns
-        -------
-        Set
-            The set of no scoring words
-        """
-        if indicator == 'legal':
-            word_set = self._process_legal_words(word_set)
-        if indicator == 'common':
-            word_set = self._process_common_words(word_set, cut_off)
-
-        return word_set
+import unicodedata
+import functools
+import operator
+import re
+import numpy as np
+import pandas as pd
+from tqdm import tqdm
+from typing import Union, Tuple
+from itertools import compress
+from sklearn.feature_extraction.text import TfidfVectorizer
+from name_matching.distance_metrics import make_distance_metrics
+from cleanco.termdata import terms_by_type, terms_by_country
+from name_matching.sparse_cosine import sparse_cosine_top_n
+
+
+class NameMatcher:
+
+    """
+    A class for the name matching of data based on the strings in a single column. The NameMatcher
+    first applies a cosine similarity on the ngrams of the strings to get an approximate match followed 
+    by a fuzzy matching based on a number of different algorithms.
+
+    Parameters
+    ----------
+    ngrams : tuple of integers
+        The length of the ngrams which should be used for the generation of ngrams for the cosine
+        similarity comparison of the possible matches
+        default=(2, 3)
+    top_n : integer
+        The number of possible matches that should be included in the group which will be analysed
+        with the fuzzy matching algorithms
+        default=50
+    low_memory : bool
+        Bool indicating if the a low memory approach should be taken in the sparse cosine similarity
+        step.
+        default=False
+    number_of_rows : integer
+        Determines how many rows should be calculated at once with the sparse cosine similarity step.
+        If the low_memory bool is True this number is unused.
+        default=5000
+    number_of_matches : int
+        The number of matches which should be returned by the matching algorithm. If a number higher
+        than 1 is given, a number of alternative matches are also returned. If the number is equal
+        to the number of algorithms used, the best match for each algorithm is returned. If the
+        number is equal to the number of algorithm groups which are included the best match for each
+        group is returned.
+        default=1
+    legal_suffixes : bool
+        Boolean indicating whether the most common company legal terms should be excluded when calculating 
+        the final score. The terms are still included in determining the best match.
+        default=False
+    common_words : bool
+        Boolean indicating whether the most common words from the matching data should be excluded 
+        when calculating the final score. The terms are still included in determining the best match.
+        default=False
+    cut_off_no_scoring_words: float
+        the cut off percentage of the occurrence of the most occurring word for which words are still included 
+        in the no_soring_words set
+        default=0.01
+    lowercase : bool
+        A boolean indicating whether during the preprocessing all characters should be converted to
+        lowercase, to generate case insensitive matching
+        default=True
+    punctuations : bool
+        A boolean indicating whether during the preprocessing all punctuations should be ignored
+        default=True
+    remove_ascii : bool
+        A boolean indicating whether during the preprocessing all characters should be converted to
+        ascii characters
+        default=True : bool
+    preprocess_split
+        Indicating whether during the preprocessing an additional step should be taken in which only 
+        the most common words out of a name are isolated and used in the matching process. The removing 
+        of the common words is only done for the n-grams cosine matching part.
+        default=False
+    verbose : bool
+        A boolean indicating whether progress printing should be done
+        default=True
+    distance_metrics: list
+        A list of The distance metrics to be used during the fuzzy matching. For a list of possible distance
+        metrics see the distance_metrics.py file. By default the following metrics are used: overlap, weighted_jaccard, 
+                ratcliff_obershelp, fuzzy_wuzzy_token_sort and editex.
+    row_numbers : bool
+        Bool indicating whether the row number should be used as match_index rather than the original index as
+        was the default case before version 0.8.8  
+        default=False
+    """
+
+    def __init__(self,
+                 ngrams: tuple = (2, 3),
+                 top_n: int = 50,
+                 low_memory: bool = False,
+                 number_of_rows: int = 5000,
+                 number_of_matches: int = 1,
+                 lowercase: bool = True,
+                 punctuations: bool = True,
+                 remove_ascii: bool = True,
+                 legal_suffixes: bool = False,
+                 common_words: bool = False,
+                 cut_off_no_scoring_words: float = 0.01,
+                 preprocess_split: bool = False,
+                 verbose: bool = True,
+                 distance_metrics: Union[list, tuple] = ['overlap', 'weighted_jaccard', 'ratcliff_obershelp',
+                                                         'fuzzy_wuzzy_token_sort', 'editex'],
+                 row_numbers: bool = False):
+
+        self._possible_matches = None
+        self._preprocessed = False
+        self._word_set = set()
+        self._df_matching_data = pd.DataFrame()
+
+        self._number_of_rows = number_of_rows
+        self._low_memory = low_memory
+
+        self._column = ''
+        self._column_matching = ''
+
+        self._verbose = verbose
+        self._number_of_matches = number_of_matches
+        self._top_n = top_n
+
+        self._preprocess_lowercase = lowercase
+        self._preprocess_punctuations = punctuations
+        self._preprocess_ascii = remove_ascii
+        self._postprocess_company_legal_id = legal_suffixes
+        self._postprocess_common_words = common_words
+
+        self._preprocess_split = preprocess_split
+        self._cut_off = cut_off_no_scoring_words
+
+        if self._postprocess_company_legal_id:
+            self._word_set = self._make_no_scoring_words(
+                'legal', self._word_set, self._cut_off)
+            
+        self._original_indexes = not row_numbers
+        self._original_index = None
+
+        self.set_distance_metrics(distance_metrics)
+
+        self._vec = TfidfVectorizer(
+            lowercase=False, analyzer="char", ngram_range=(ngrams))
+        self._n_grams_matching = None
+
+    def set_distance_metrics(self, metrics: list) -> None:
+        """
+        A method to set which of the distance metrics should be employed during the
+        fuzzy matching. For very short explanations of most of the name matching 
+        algorithms please see the make_distance_metrics function in distance_matrics.py
+
+        Parameters
+        ----------
+        metrics: list 
+            The list with the distance metrics to be used during the name matching. The
+            distance metrics can be chosen from the list below:
+                indel
+                discounted_levenshtein
+                tichy
+                cormodeL_z
+                iterative_sub_string
+                baulieu_xiii
+                clement
+                dice_asymmetricI
+                kuhns_iii
+                overlap
+                pearson_ii
+                weighted_jaccard
+                warrens_iv
+                bag
+                rouge_l
+                ratcliff_obershelp
+                ncd_bz2
+                fuzzy_wuzzy_partial_string
+                fuzzy_wuzzy_token_sort
+                fuzzy_wuzzy_token_set
+                editex
+                typo
+                lig_3
+                ssk
+                refined_soundex
+                double_metaphone
+        """
+
+        input_metrics = {str(metric).lower(): True for metric in metrics}
+        try:
+            self._distance_metrics = make_distance_metrics(**input_metrics)
+        except TypeError:
+            raise TypeError('Not all of the supplied distance metrics are available. Please check the' +
+                            'list of options in the make_distance_metrics function and adjust your list accordingly')
+        self._num_distance_metrics = sum(
+            [len(x) for x in self._distance_metrics.values()])
+
+    def _select_top_words(self, word: str, word_counts: pd.Series, occurrence_count: int) -> str:
+        """Remove the top words from the string word based on an occurrence_count threshold
+
+        Parameters
+        ----------
+        word: str 
+            the string from which the words should be removed
+        word_counts: pd.Series
+            the words which should be removed with their counts as result from a value_counts
+        occurrence_count: int 
+            the multiplication factor of the minimum occurrences below which to select 
+
+        Returns
+        -------
+        str
+           The string word with the words with a too high word_counts removed
+        """
+        compressed_list = list(compress(
+            word, (word_counts[word] < occurrence_count*word_counts[word].min()).values))
+
+        return ' '.join(compressed_list)
+
+    def _preprocess_reduce(self,
+                           to_be_matched: pd.DataFrame,
+                           occurrence_count: int = 3) -> pd.DataFrame:
+        """Preprocesses and copies the data to obtain the data with reduced strings. The strings have all words
+        removed which appear more than 3x as often as the least common word in the string and returns an adjusted 
+        copy of the input 
+
+        Parameters
+        ----------
+        to_be_matched: pd.DataFrame 
+            A dataframe from which the most common words should be removed
+        occurrence_count: int
+            The number of occurrence a word can occur more then the least common word in the string for which it will
+            still be included in the process 
+            default=3
+
+        Returns
+        -------
+        pd.DataFrame
+            A dataframe that will contain the reduced strings
+        """
+        individual_words = to_be_matched[self._column_matching].str.split(
+            expand=True).stack()
+        word_counts = individual_words.value_counts()
+        to_be_matched_new = to_be_matched.copy()
+        name = to_be_matched[self._column_matching].str.split()
+        to_be_matched_new[self._column_matching] = name.apply(
+            lambda word: self._select_top_words(word, word_counts, occurrence_count))
+
+        return to_be_matched_new
+
+    def load_and_process_master_data(self,
+                                     column: str,
+                                     df_matching_data: pd.DataFrame,
+                                     start_processing: bool = True,
+                                     transform: bool = True) -> None:
+        """Load the matching data into the NameMatcher and start the preprocessing.
+
+        Parameters
+        ----------
+        column : string
+            The column name of the dataframe which should be used for the matching
+        df_matching_data: pd.DataFrame
+            The dataframe which is used to match the data to.
+        start_processing : bool 
+            A boolean indicating whether to start the preprocessing step after loading the matching data 
+            default: True
+        transform : bool 
+            A boolean indicating whether or not the data should be transformed after the vectoriser is initialised 
+            default: True
+        """
+        self._column = column
+        self._df_matching_data = df_matching_data        
+        self._original_index = df_matching_data.index
+        if start_processing:
+            self._process_matching_data(transform)
+
+    def _process_matching_data(self,
+                               transform: bool = True) -> None:
+        """Function to process the matching data. First the matching data is preprocessed and assigned to 
+        a variable within the NameMatcher. Next the data is used to initialise the TfidfVectorizer. 
+
+        Parameters
+        ----------
+        transform : bool 
+            A boolean indicating whether or not the data should be transformed after the vectoriser is initialised 
+            default: True
+        """
+        self._df_matching_data = self.preprocess(
+            self._df_matching_data, self._column)
+        if self._postprocess_common_words:
+            self._word_set = self._make_no_scoring_words(
+                'common', self._word_set, self._cut_off)
+        self._vectorise_data(transform)
+        self._preprocessed = True
+
+    def match_names(self,
+                    to_be_matched: Union[pd.Series, pd.DataFrame],
+                    column_matching: str) -> Union[pd.Series, pd.DataFrame]:
+        """Performs the name matching operation on the to_be_matched data. First it does the preprocessing of the 
+        data to be matched as well as the matching data if this has not been performed. Subsequently based on 
+        ngrams a cosine similarity is computed between the matching data and the data to be matched, to the top n
+        matches fuzzy matching algorithms are performed to determine the best match and the quality of the match
+
+        Parameters
+        ----------
+        to_be_matched: Union[pd.Series, pd.DataFrame]
+            The data which should be matched
+        column_matching: str
+            string indicating the column which will be matched
+
+        Returns
+        -------
+        Union[pd.Series, pd.DataFrame]
+            A series or dataframe depending on the input containing the match index from the matching_data dataframe. 
+            the name in the to_be_matched data, the name to which the datapoint was matched and a score between 0 
+            (no match) and 100(perfect match) to indicate the quality of the matches
+        """
+        if self._column == '':
+            raise ValueError(
+                'Please first load the master data via the method: load_and_process_master_data')
+        if self._verbose:
+            tqdm.pandas()
+            tqdm.write('preprocessing...\n')
+        self._column_matching = column_matching
+
+        is_dataframe = True
+        if isinstance(to_be_matched, pd.Series):
+            is_dataframe = False
+            to_be_matched = pd.DataFrame(
+                [to_be_matched.values], columns=to_be_matched.index.to_list())
+        if not self._preprocessed:
+            self._process_matching_data()
+        to_be_matched = self.preprocess(to_be_matched, self._column_matching)
+
+        if self._verbose:
+            tqdm.write('preprocessing complete \n searching for matches...\n')
+
+        self._possible_matches = self._search_for_possible_matches(
+            to_be_matched)
+
+        if self._preprocess_split:
+            self._possible_matches = np.hstack((self._search_for_possible_matches(
+                self._preprocess_reduce(to_be_matched)), self._possible_matches))
+        
+        if self._verbose:
+            tqdm.write('possible matches found   \n fuzzy matching...\n')
+            data_matches = to_be_matched.progress_apply(lambda x: self.fuzzy_matches(
+                self._possible_matches[to_be_matched.index.get_loc(x.name), :], x), axis=1)
+        else:
+            data_matches = to_be_matched.apply(lambda x: self.fuzzy_matches(
+                self._possible_matches[to_be_matched.index.get_loc(x.name), :], x), axis=1)
+
+        if self._number_of_matches == 1:
+            data_matches = data_matches.rename(columns={'match_name_0': 'match_name',
+                                                        'score_0': 'score', 'match_index_0': 'match_index'})
+        if is_dataframe and self._original_indexes:
+            for col in data_matches.columns[data_matches.columns.str.contains('match_index')]:
+                data_matches[col] = self._original_index[data_matches[col].astype(int).fillna(0)]
+
+        if self._verbose:
+            tqdm.write('done')
+
+        return data_matches
+
+    def fuzzy_matches(self,
+                      possible_matches: np.array,
+                      to_be_matched: pd.Series) -> pd.Series:
+        """ A method which performs the fuzzy matching between the data in the to_be_matched series as well
+        as the indicated indexes of the matching_data points which are possible matching candidates.
+
+        Parameters
+        ----------
+        possible_matches : np.array
+            An array containing the indexes of the matching data with potential matches
+        to_be_matched : pd.Series
+            The data which should be matched
+
+        Returns
+        -------
+        pd.Series
+            A series containing the match index from the matching_data dataframe. the name in the to_be_matched data,
+            the name to which the datapoint was matched and a score between 0 (no match) and 100(perfect match) to 
+            indicate the quality of the matches
+        """
+        if len(possible_matches.shape) > 1:
+            possible_matches = possible_matches[0]
+
+        indexes = np.array([[f'match_name_{num}', f'score_{num}', f'match_index_{num}']
+                            for num in range(self._number_of_matches)]).flatten()
+        match = pd.Series(index=np.append('original_name', indexes), dtype=object)
+        match['original_name'] = to_be_matched[self._column_matching]
+        list_possible_matches = self._df_matching_data.iloc[
+            possible_matches.flatten(), :][self._column].values
+
+        match_score = self._score_matches(
+            to_be_matched[self._column_matching], list_possible_matches)
+        ind = self._rate_matches(match_score)
+
+        for num, col_num in enumerate(ind):
+            match[f'match_name_{num}'] = list_possible_matches[col_num]
+            match[f'match_index_{num}'] = possible_matches[col_num]
+
+        match = self._adjust_scores(match_score[ind, :], match)
+
+        if self._postprocess_common_words or self._postprocess_company_legal_id:
+            match = self.postprocess(match)
+
+        return match
+
+    def _score_matches(self,
+                       to_be_matched_instance: str,
+                       possible_matches: list) -> np.array:
+        """A method to score a name to_be_matched_instance to a list of possible matches. The scoring is done
+        based on all the metrics which are enabled.
+
+        Parameters
+        ----------
+        to_be_matched_instance : str
+            The name which should match one of the possible matches
+        possible_matches : list
+            list of the names of the possible matches
+
+        Returns
+        -------
+        np.array
+            The score of each of the matches with respect to the different metrics which are assessed.
+        """
+        match_score = np.zeros(
+            (len(possible_matches), self._num_distance_metrics))
+        idx = 0
+        for method_list in self._distance_metrics.values():
+            for method in method_list:
+                match_score[:, idx] = np.array(
+                    [method.sim(to_be_matched_instance, s) for s in possible_matches])
+                idx = idx + 1
+
+        return match_score
+
+    def _rate_matches(self,
+                      match_score: np.array) -> np.array:
+        """Converts the match scores from the score_matches method to a list of indexes of the best scoring 
+        matches limited to the _number_of_matches.
+
+        Parameters
+        ----------
+        match_score : np.array
+            An array containing the scores of each of the possible alternatives for each
+            of the different methods used
+
+        Returns
+        -------
+        np.array
+            The indexes of the best rated matches
+        """
+        if self._number_of_matches == 1:
+            ind = [np.argmax(np.mean(match_score, axis=1))]
+        elif self._number_of_matches == len(self._distance_metrics):
+            ind = np.zeros(len(self._distance_metrics))
+            idx = 0
+            for num, method_list in enumerate(self._distance_metrics.values()):
+                method_grouped_results = np.reshape(
+                    match_score[:, idx: idx + len(method_list)], (-1, len(method_list)))
+                ind[num] = np.argmax(np.mean(method_grouped_results, axis=1))
+                idx = idx + len(method_list)
+        elif self._number_of_matches == self._num_distance_metrics:
+            ind = np.argmax(match_score, axis=1)
+        else:
+            ind = np.argsort(np.mean(match_score, axis=1)
+                             )[-self._number_of_matches:][::-1]
+
+        return np.array(ind, dtype=int)
+
+    def _get_alternative_names(self, match: pd.Series) -> list:
+        """Gets all the possible match names from the match.
+
+        Parameters
+        ----------
+        match : pd.Series
+            The series with the possible matches and original scores
+
+        Returns
+        -------
+        list
+            A list with the alternative names for this match
+        """
+        alt_names = []
+
+        for num in range(self._number_of_matches):
+            alt_names.append(str(match[f'match_name_{num}']))
+
+        return alt_names
+
+    def _process_words(self, org_name: str, alt_names: list) -> Tuple[str, list]:
+        """Removes the words from the word list from the org_name and all the names in alt_names .
+
+        Parameters
+        ----------
+        org_name : str
+            The original name for the matching data
+        alt_names : list
+            A list of names from which the words should be removed
+
+        Returns
+        -------
+        Tuple[str, list]
+            The processed version of the org_name and the alt_names, with the words removed
+        """
+        len_atl_names = len(alt_names)
+        for word in self._word_set:
+            org_name = ' '.join(
+                re.sub(fr'\b{re.escape(word)}\b', '', org_name).split())
+            for num in range(len_atl_names):
+                alt_names[num] = ' '.join(
+                    re.sub(fr'\b{re.escape(word)}\b', '', alt_names[num]).split())
+
+        return org_name, alt_names
+
+    def _adjust_scores(self, match_score: np.array, match: pd.Series) -> pd.Series:
+        """Adjust the scores to be between 0 and 100
+
+        Parameters
+        ----------
+        match_score : np.array
+            An array with the scores for each of the options
+        match : pd.Series
+            The series with the possible matches and original scores
+
+        Returns
+        -------
+        pd.Series
+            The series with the possible matches and adjusted scores
+        """
+        for num in range(self._number_of_matches):
+            match[f'score_{num}'] = 100*np.mean(match_score[num, :])
+
+        return match
+
+    def postprocess(self,
+                    match: pd.Series) -> pd.Series:
+        """Postprocesses the scores to exclude certain specific company words or the most 
+        common words. In this method only the scores are adjusted, the matches still stand.
+
+        Parameters
+        ----------
+        match : pd.Series
+            The series with the possible matches and original scores
+
+        Returns
+        -------
+        pd.Series
+            A new version of the input series with updated scores
+        """
+        alt_names = self._get_alternative_names(match)
+        org_name = str(match['original_name'])
+
+        org_name, alt_names = self._process_words(org_name, alt_names)
+
+        match_score = self._score_matches(org_name, alt_names)
+
+        match = self._adjust_scores(match_score, match)
+
+        return match
+
+    def _vectorise_data(self,
+                        transform: bool = True):
+        """Initialises the TfidfVectorizer, which generates ngrams and weights them based on the occurrance.
+        Subsequently the matching data will be used to fit the vectoriser and the matching data might also be send
+        to the transform_data function depending on the transform boolean.
+
+        Parameters
+        ----------
+        transform : bool 
+            A boolean indicating whether or not the data should be transformed after the vectoriser is initialised 
+            default: True
+        """
+        self._vec.fit(self._df_matching_data[self._column].values.flatten())
+        if transform:
+            self.transform_data()
+
+    def transform_data(self):
+        """A method which transforms the matching data based on the ngrams transformer. After the 
+        transformation (the generation of the ngrams), the data is normalised by dividing each row
+        by the sum of the row. Subsequently the data is changed to a coo sparse matrix format with
+        the column indices in ascending order.
+        """
+        ngrams = self._vec.transform(
+            self._df_matching_data[self._column].astype(str))
+        for i, j in zip(ngrams.indptr[:-1], ngrams.indptr[1:]):
+            ngrams.data[i:j] = ngrams.data[i:j]/np.sum(ngrams.data[i:j])
+        self._n_grams_matching = ngrams.tocsc()
+        if self._low_memory:
+            self._n_grams_matching = self._n_grams_matching.tocoo()
+
+    def _search_for_possible_matches(self,
+                                     to_be_matched: pd.DataFrame) -> np.array:
+        """Generates ngrams from the data which should be matched, calculate the cosine simularity
+        between these data and the matching data. Hereafter a top n of the matches is selected and
+        returned.
+
+        Parameters
+        ----------
+        to_be_matched : pd.Series
+            A series containing a single instance of the data to be matched
+
+        Returns
+        -------
+        np.array
+            An array of top n values which are most closely matched to the to be matched data based
+            on the ngrams
+        """
+        if self._n_grams_matching is None:
+            raise RuntimeError(
+                """First the data needs to be transformed to be able to use the sparse cosine simularity. To""" +
+                """transform the data, run transform_data or run load_and_process_master_data with transform=True""")
+
+        if self._low_memory:
+            results = np.zeros((len(to_be_matched), self._top_n))
+            input_data = to_be_matched[self._column_matching]
+            for idx, row_name in enumerate(tqdm(input_data, disable=not self._verbose)):
+                match_ngrams = self._vec.transform([row_name])
+                results[idx, :] = sparse_cosine_top_n(
+                    matrix_a=self._n_grams_matching, matrix_b=match_ngrams, top_n=self._top_n, low_memory=self._low_memory, number_of_rows=self._number_of_rows, verbose=self._verbose)
+        else:
+            match_ngrams = self._vec.transform(
+                to_be_matched[self._column_matching].tolist()).tocsc()
+            results = sparse_cosine_top_n(
+                matrix_a=self._n_grams_matching, matrix_b=match_ngrams, top_n=self._top_n, low_memory=self._low_memory, number_of_rows=self._number_of_rows, verbose=self._verbose)
+
+        return results
+
+    def preprocess(self,
+                   df: pd.DataFrame,
+                   column_name: str) -> pd.DataFrame:
+        """Preprocess a dataframe before applying a name matching algorithm. The preprocessing consists of 
+        removing special characters, spaces, converting all characters to lower case and removing the
+        words given in the word lists
+
+        Parameters
+        ----------
+        df : DataFrame
+            The dataframe or series on which the preprocessing needs to be performed        
+        column_name : str
+            The name of the column that is used for the preprocessing
+
+        Returns
+        -------
+        pd.DataFrame
+            The preprocessed dataframe or series depending on the input
+        """
+        df.loc[:, column_name] = df[column_name].astype(str)
+        if self._preprocess_lowercase:
+            df.loc[:, column_name] = df[column_name].str.lower()
+        if self._preprocess_punctuations:
+            df.loc[:, column_name] = df[column_name].str.replace(
+                '[^\w\s]', '', regex=True)
+            df.loc[:, column_name] = df[column_name].str.replace(
+                '  ', ' ').str.strip()
+        if self._preprocess_ascii:
+            df.loc[:, column_name] = df[column_name].apply(lambda string: unicodedata.normalize(
+                'NFKD', str(string)).encode('ASCII', 'ignore').decode())
+
+        return df
+
+    def _preprocess_word_list(self, terms: dict) -> list:
+        """Preprocess legal words to remove punctuations and trailing leading space
+
+        Parameters
+        -------
+        terms: dict
+            a dictionary of legal words
+
+        Returns
+        -------
+        list
+            A list of preprocessed legal words  
+        """
+        if self._preprocess_punctuations:
+            return [re.sub(r'[^\w\s]', '', s).strip() for s in functools.reduce(
+                operator.iconcat, terms.values(), [])]
+        else:
+            return [s.strip() for s in functools.reduce(
+                    operator.iconcat, terms.values(), [])]
+
+    def _process_legal_words(self, word_set: set) -> set:
+        """Preprocess legal words and add them to the word_set
+
+        Parameters
+        -------
+        word_set: str
+            the current word list which should be extended with additional words
+
+        Returns
+        -------
+        Set
+            The original word_set with the legal words added
+        """
+        terms_type = self._preprocess_word_list(terms_by_type)
+        terms_country = self._preprocess_word_list(terms_by_country)
+        word_set = word_set.union(set(terms_country + terms_type))
+
+        return word_set
+
+    def _process_common_words(self, word_set: set, cut_off: float) -> set:
+        """A method to select the most common words from the matching_data.
+
+        Parameters
+        -------
+        word_set: str
+            the current word list which should be extended with additional words  
+        cut_off: float
+            the cut_off percentage of the occurrence of the most occurring word for which words are still included 
+            in the no_soring_words set
+
+        Returns
+        -------
+        Set
+            The current word set with the most common words from the matching_data added
+        """
+        word_counts = self._df_matching_data[self._column].str.split(
+            expand=True).stack().value_counts()
+        word_set = word_set.union(
+            set(word_counts[word_counts > np.max(word_counts)*cut_off].index))
+
+        return word_set
+
+    def _make_no_scoring_words(self,
+                               indicator: str,
+                               word_set: set,
+                               cut_off: float) -> set:
+        """A method to make a set of words which are not taken into account when scoring matches.
+
+        Parameters
+        -------
+        indicator: str
+            indicator for which types of words should be excluded can be legal for
+            legal suffixes or common for the most common words
+        word_set: str
+            the current word list which should be extended with additional words  
+        cut_off: float
+            the cut_off percentage of the occurrence of the most occurring word for which words are still included 
+            in the no_soring_words set
+
+        Returns
+        -------
+        Set
+            The set of no scoring words
+        """
+        if indicator == 'legal':
+            word_set = self._process_legal_words(word_set)
+        if indicator == 'common':
+            word_set = self._process_common_words(word_set, cut_off)
+
+        return word_set
```

### Comparing `name_matching-0.8.8/name_matching/run_nm.py` & `name_matching-0.8.9/name_matching/run_nm.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,310 +1,310 @@
-from name_matching.name_matcher import NameMatcher
-from typing import Union, Tuple
-import pandas as pd
-import unicodedata
-
-
-def _match_names_check_data(data: Union[pd.Series, pd.DataFrame],
-                            column: str,
-                            group_column: str) -> pd.DataFrame:
-    """
-    Checks the input data of the name matching function to see whether the defined columns can 
-    be found and makes a new column which will be used for the name matching
-    ----------
-    data: Union[pd.DataFrame, pd.Series]
-        The first dataframe or series used for the name matching        
-    column: str
-        The column in which the name that should be matched can be found for data
-    group_column_first: str
-        The name of the column that should be used to generate groups within the data.
-
-    Returns
-    -------
-    pd.DataFrame
-        A dataframe containing data and an additional column 'name_matching_data' containing the
-        names which should be matched
-    """
-
-    if isinstance(data, pd.DataFrame):
-        if column == '':
-            raise ValueError(
-                'For one of the dataframes no column is given to perform the name matching on')
-        if column not in data.columns:
-            raise ValueError(
-                'Could not find one of the columns in the dataframe')
-        if (group_column != '') & (group_column not in data.columns):
-            raise ValueError(
-                'Could not find one of the group_columns in the dataframe')
-        data['name_matching_data'] = data[column]
-    else:
-        if group_column != '':
-            raise ValueError(
-                'Grouping is only possible when a dataframe is used for both inputs')
-        data = pd.DataFrame(data, columns=['name_matching_data'])
-
-    return data
-
-def _match_names_preprocess_data(column: str,
-                                data_first: pd.DataFrame,
-                                data_second: pd.DataFrame,
-                                case_sensitive: bool,
-                                punctuation_sensitive: bool,
-                                special_character_sensitive: bool) -> Tuple[pd.DataFrame, pd.DataFrame]:
-    """
-    Preprocess the data by making the names lower case, removing punctuations and special characters. 
-    And convert the indexes of the second dataframe to a column.
-    ----------
-    data: Union[pd.DataFrame, pd.Series]
-        The first dataframe or series used for the name matching        
-    column: str
-        The column in which the name that should be matched can be found for data
-    group_column_first: str
-        The name of the column that should be used to generate groups within the data.
-    case_sensitive: bool
-        Boolean value indicating whether the names should be converted to lower case names
-        before the name matching starts. If False all the characters are converted to lowercase
-    punctuation_sensitive: bool
-        Boolean value indicating whether punctuations should be removed from the original names
-        before the name matching starts. If False the punctuations are removed
-    special_character_sensitive: bool
-        Boolean value indicating whether special characters should be converted to unicode
-        before the name matching starts. If False the special characters are replaced
-
-    Returns
-    -------
-    Tuple[pd.DataFrame, pd.DataFrame]
-        A dataframe containing data and an additional column 'name_matching_data' containing the
-        names which should be matched
-    """
-
-    if not case_sensitive:
-        data_first[column] = data_first[column].str.lower().str.strip()
-        data_second[column] = data_second[column].str.lower().str.strip()
-    if not punctuation_sensitive:
-        data_first[column] = data_first[column].str.replace('[^\w\s]', '', regex=True)
-        data_second[column] = data_second[column].str.replace(
-            '[^\w\s]', '', regex=True)
-    if not special_character_sensitive:
-        data_first[column] = data_first[column].apply(lambda string: unicodedata.normalize(
-            'NFKD', string).encode('ASCII', 'ignore').decode())
-        data_second[column] = data_second[column].apply(lambda string: unicodedata.normalize(
-            'NFKD', string).encode('ASCII', 'ignore').decode())
-
-    data_second = data_second.rename_axis('index').reset_index(drop=False)
-    
-    return data_first, data_second
-
-def _match_names_combine_data(data_first: pd.DataFrame, 
-                              data_second: pd.DataFrame, 
-                              left_cols: list, 
-                              right_cols: list) -> pd.DataFrame:
-    """
-    Perform a merge to match data based on whether the names are equal
-    ----------
-    data_first: pd.DataFrame
-        The first dataframe or series used for the name matching        
-    data_second: pd.DataFrame
-        The second dataframe or series used for the name matching        
-    left_cols: list
-        A list of columns on which the first dataframe should be merged  
-    right_cols: list
-        A list of columns on which the first dataframe should be merged
-
-    Returns
-    -------
-    pd.DataFrame
-        A dataframe containing the original name, matched name, match score and match index. The index of the
-        dataframe is equal to the original index of data_first, the match index is the index in data_second
-        for the matched name.
-    """
-    matches = pd.merge(data_first, data_second, how='left',
-                        left_on=left_cols, right_on=right_cols, suffixes=['', '_matched'])
-    matches['score'] = 100
-    matches = matches.dropna(subset=['index'])
-    matches = matches.rename(columns={'index':'match_index'})
-    matches = matches[['match_index', 'score']] 
-
-    return matches
-
-def _match_names_match_single(matcher: NameMatcher,
-                              data_first: pd.DataFrame,
-                              data_second: pd.DataFrame,
-                              name_column: str) -> pd.DataFrame:
-    """
-    Perform the name matching. First by doing a perfect string match with a merge statement, followed
-    by the fuzzy matching approach as done in NameMatcher. 
-    ----------
-    matcher: NameMatcher
-        The NameMatcher to be used for the name matching part        
-    data_first: pd.DataFrame
-        The first dataframe or series used for the name matching        
-    data_second: pd.DataFrame
-        The second dataframe or series used for the name matching        
-    name_column: str
-        The column in which the name that should be matched can be found for both dataframes
-
-    Returns
-    -------
-    pd.DataFrame
-        A dataframe containing the original name, matched name, match score and match index. The index of the
-        dataframe is equal to the original index of data_first, the match index is the index in data_second
-        for the matched name.
-    """
-
-    matches = _match_names_combine_data(data_first, data_second,
-                            [name_column], [name_column])
-    unmatched = data_first[~data_first.index.isin(matches.index)].copy()
-    if len(unmatched) > 0:
-        matcher.load_and_process_master_data(name_column, data_second, transform=True)
-        matches = pd.concat([matches,(matcher.match_names(
-            to_be_matched=unmatched, column_matching=name_column))])
-        return matches
-    else:
-        print('All data matched with basic string matching')
-        return matches
-
-def _match_names_match_group(matcher: NameMatcher,
-                            data_first: pd.DataFrame,
-                            data_second: pd.DataFrame,
-                            name_column: str,
-                            group_column_first: str,
-                            group_column_second: str) -> pd.DataFrame:
-    """
-    Perform the name matching based on the subgroups as indicated by the group_column strings. First by doing
-    a perfect string match with a merge statement, followed by the fuzzy matching approach as done in NameMatcher. 
-    ----------
-    matcher: NameMatcher
-        The NameMatcher to be used for the name matching part        
-    data_first: pd.DataFrame
-        The first dataframe or series used for the name matching        
-    data_second: pd.DataFrame
-        The second dataframe or series used for the name matching        
-    name_column: str
-        The column in which the name that should be matched can be found for both dataframes
-    group_column_first: str
-        The name of the column that should be used to generate groups within the data.
-    group_column_second: str
-        The name of the column that should be used to generate groups within the data.
-
-    Returns
-    -------
-    pd.DataFrame
-        A dataframe containing the original name, matched name, match score and match index. The index of the
-        dataframe is equal to the original index of data_first, the match index is the index in data_second
-        for the matched name.
-    """
-
-    matches = _match_names_combine_data(data_first, data_second, [
-                            name_column, group_column_first], [name_column, group_column_second])
-    unmatched = data_first[~data_first.index.isin(matches.index)]
-    if len(unmatched) > 0:
-        matcher.load_and_process_master_data(name_column, data_second, transform=False)
-        for group in data_first[group_column_first].unique():
-            data_second_group = data_second[data_second[group_column_second] == group].copy()
-            matcher.load_and_process_master_data(name_column, 
-                data_second_group, start_processing=False)
-            matcher.transform_data()
-            matches = pd.concat([matches, matcher.match_names(
-                to_be_matched=unmatched[unmatched[group_column_first] == group].copy(), column_matching=name_column)])
-    else:
-        print('All data matched with basic string matching')
-        return matches
-
-    return matches
-
-
-def match_names(data_first: Union[pd.DataFrame, pd.Series],
-                data_second: Union[pd.DataFrame, pd.Series],
-                column_first='',
-                column_second='',
-                group_column_first='',
-                group_column_second='',
-                case_sensitive=False,
-                punctuation_sensitive=False,
-                special_character_sensitive=False,
-                threshold=95,
-                **kwargs) -> pd.DataFrame:
-    """Function which performs name matching. First a simple merge on the data is performed
-    to get the instances in which the name matches perfectly. Subsequently the matches are
-    matched using the name matching algorithm as defined in name_matcher.
-
-    Parameters
-    ----------
-    data_first: Union[pd.DataFrame, pd.Series]
-        The first dataframe or series used for the name matching
-    data_second: Union[pd.DataFrame, pd.Series]
-        The second dataframe or series used for the name matching, for matching the data to 
-        itself data_second should be equal to data first
-    column_first: str
-        If data_first is a dataframe column_first should be the column in which the name 
-        that should be matched can be found for data_first
-        default=''
-    column_second: str
-        If data_second is a dataframe column_second should be the column in which the name 
-        that should be matched can be found for data_second
-        default=''
-    group_column_first: str
-        The name of the column that should be used to generate groups within the data_first 
-        dataframe. The matchig is then only performed for instances in which the groups are
-        identical
-        default=''
-    group_column_second: str
-        The name of the column that should be used to generate groups within the data_second 
-        dataframe. The matchig is then only performed for instances in which the groups are
-        identical
-        default=''
-    case_sensitive: bool
-        Boolean value indicating whether the names should be converted to lower case names
-        before the name matching starts. If False all the characters are converted to lowercase
-        default=False
-    punctuation_sensitive: bool
-        Boolean value indicating whether punctuations should be removed from the original names
-        before the name matching starts. If False the punctuations are removed
-        default=False
-    special_character_sensitive: bool
-        Boolean value indicating whether special characters should be converted to unicode
-        before the name matching starts. If False the special characters are replaced
-        default=False
-    threshold: int
-        the minimal score a match should have to be part of the output
-        default=95
-    **kwargs
-        Additional inputs for the name_matcher
-
-    Returns
-    -------
-    pd.DataFrame
-        A dataframe containing the matched rows were the match score is above the threshold. The
-        dataframe consists of 4 columns; original_name: the original name from data_first after 
-        preprocessing, match_name_0: the name it is matched to from data_second after preprocessing,
-        score_0: the score of the match, match_index_0: the index of the match in data_second. The 
-        match_index_0 can be used to join the data from both dataframes. 
-    """
-    if 'number_of_matches' in kwargs:
-        raise ValueError(
-            'The number of matches can only be changed by using a custom matching approach')
-
-    data_first = _match_names_check_data(data_first, column_first, group_column_first)
-    data_second = _match_names_check_data(data_second, column_second, group_column_second)
-
-    name_column = 'name_matching_data'
-
-    if ((group_column_first == '') & (group_column_second != '')) | ((group_column_second == '') & (group_column_first != '')):
-        raise ValueError(
-            'For the grouping to work both the grouping column in the first as well as the second dataframe have to be indicated')
-
-    if (threshold > 100) | (threshold < 0):
-        raise ValueError('Please pick a threshold between 0 and 100')
-
-    data_first, data_second = _match_names_preprocess_data(name_column, data_first, 
-            data_second, case_sensitive, punctuation_sensitive, special_character_sensitive)
-
-    matcher = NameMatcher(**kwargs)
-
-    if group_column_first == '':
-        matches = _match_names_match_single(matcher, data_first, data_second, name_column)
-    else:
-        matches = _match_names_match_group(matcher, data_first, data_second,
-                              name_column, group_column_first, group_column_second)
-
-    return matches[matches['score'] > threshold]
+from name_matching.name_matcher import NameMatcher
+from typing import Union, Tuple
+import pandas as pd
+import unicodedata
+
+
+def _match_names_check_data(data: Union[pd.Series, pd.DataFrame],
+                            column: str,
+                            group_column: str) -> pd.DataFrame:
+    """
+    Checks the input data of the name matching function to see whether the defined columns can 
+    be found and makes a new column which will be used for the name matching
+    ----------
+    data: Union[pd.DataFrame, pd.Series]
+        The first dataframe or series used for the name matching        
+    column: str
+        The column in which the name that should be matched can be found for data
+    group_column_first: str
+        The name of the column that should be used to generate groups within the data.
+
+    Returns
+    -------
+    pd.DataFrame
+        A dataframe containing data and an additional column 'name_matching_data' containing the
+        names which should be matched
+    """
+
+    if isinstance(data, pd.DataFrame):
+        if column == '':
+            raise ValueError(
+                'For one of the dataframes no column is given to perform the name matching on')
+        if column not in data.columns:
+            raise ValueError(
+                'Could not find one of the columns in the dataframe')
+        if (group_column != '') & (group_column not in data.columns):
+            raise ValueError(
+                'Could not find one of the group_columns in the dataframe')
+        data['name_matching_data'] = data[column]
+    else:
+        if group_column != '':
+            raise ValueError(
+                'Grouping is only possible when a dataframe is used for both inputs')
+        data = pd.DataFrame(data, columns=['name_matching_data'])
+
+    return data
+
+def _match_names_preprocess_data(column: str,
+                                data_first: pd.DataFrame,
+                                data_second: pd.DataFrame,
+                                case_sensitive: bool,
+                                punctuation_sensitive: bool,
+                                special_character_sensitive: bool) -> Tuple[pd.DataFrame, pd.DataFrame]:
+    """
+    Preprocess the data by making the names lower case, removing punctuations and special characters. 
+    And convert the indexes of the second dataframe to a column.
+    ----------
+    data: Union[pd.DataFrame, pd.Series]
+        The first dataframe or series used for the name matching        
+    column: str
+        The column in which the name that should be matched can be found for data
+    group_column_first: str
+        The name of the column that should be used to generate groups within the data.
+    case_sensitive: bool
+        Boolean value indicating whether the names should be converted to lower case names
+        before the name matching starts. If False all the characters are converted to lowercase
+    punctuation_sensitive: bool
+        Boolean value indicating whether punctuations should be removed from the original names
+        before the name matching starts. If False the punctuations are removed
+    special_character_sensitive: bool
+        Boolean value indicating whether special characters should be converted to unicode
+        before the name matching starts. If False the special characters are replaced
+
+    Returns
+    -------
+    Tuple[pd.DataFrame, pd.DataFrame]
+        A dataframe containing data and an additional column 'name_matching_data' containing the
+        names which should be matched
+    """
+
+    if not case_sensitive:
+        data_first[column] = data_first[column].str.lower().str.strip()
+        data_second[column] = data_second[column].str.lower().str.strip()
+    if not punctuation_sensitive:
+        data_first[column] = data_first[column].str.replace('[^\w\s]', '', regex=True)
+        data_second[column] = data_second[column].str.replace(
+            '[^\w\s]', '', regex=True)
+    if not special_character_sensitive:
+        data_first[column] = data_first[column].apply(lambda string: unicodedata.normalize(
+            'NFKD', string).encode('ASCII', 'ignore').decode())
+        data_second[column] = data_second[column].apply(lambda string: unicodedata.normalize(
+            'NFKD', string).encode('ASCII', 'ignore').decode())
+
+    data_second = data_second.rename_axis('index').reset_index(drop=False)
+    
+    return data_first, data_second
+
+def _match_names_combine_data(data_first: pd.DataFrame, 
+                              data_second: pd.DataFrame, 
+                              left_cols: list, 
+                              right_cols: list) -> pd.DataFrame:
+    """
+    Perform a merge to match data based on whether the names are equal
+    ----------
+    data_first: pd.DataFrame
+        The first dataframe or series used for the name matching        
+    data_second: pd.DataFrame
+        The second dataframe or series used for the name matching        
+    left_cols: list
+        A list of columns on which the first dataframe should be merged  
+    right_cols: list
+        A list of columns on which the first dataframe should be merged
+
+    Returns
+    -------
+    pd.DataFrame
+        A dataframe containing the original name, matched name, match score and match index. The index of the
+        dataframe is equal to the original index of data_first, the match index is the index in data_second
+        for the matched name.
+    """
+    matches = pd.merge(data_first, data_second, how='left',
+                        left_on=left_cols, right_on=right_cols, suffixes=['', '_matched'])
+    matches['score'] = 100
+    matches = matches.dropna(subset=['index'])
+    matches = matches.rename(columns={'index':'match_index'})
+    matches = matches[['match_index', 'score']] 
+
+    return matches
+
+def _match_names_match_single(matcher: NameMatcher,
+                              data_first: pd.DataFrame,
+                              data_second: pd.DataFrame,
+                              name_column: str) -> pd.DataFrame:
+    """
+    Perform the name matching. First by doing a perfect string match with a merge statement, followed
+    by the fuzzy matching approach as done in NameMatcher. 
+    ----------
+    matcher: NameMatcher
+        The NameMatcher to be used for the name matching part        
+    data_first: pd.DataFrame
+        The first dataframe or series used for the name matching        
+    data_second: pd.DataFrame
+        The second dataframe or series used for the name matching        
+    name_column: str
+        The column in which the name that should be matched can be found for both dataframes
+
+    Returns
+    -------
+    pd.DataFrame
+        A dataframe containing the original name, matched name, match score and match index. The index of the
+        dataframe is equal to the original index of data_first, the match index is the index in data_second
+        for the matched name.
+    """
+
+    matches = _match_names_combine_data(data_first, data_second,
+                            [name_column], [name_column])
+    unmatched = data_first[~data_first.index.isin(matches.index)].copy()
+    if len(unmatched) > 0:
+        matcher.load_and_process_master_data(name_column, data_second, transform=True)
+        matches = pd.concat([matches,(matcher.match_names(
+            to_be_matched=unmatched, column_matching=name_column))])
+        return matches
+    else:
+        print('All data matched with basic string matching')
+        return matches
+
+def _match_names_match_group(matcher: NameMatcher,
+                            data_first: pd.DataFrame,
+                            data_second: pd.DataFrame,
+                            name_column: str,
+                            group_column_first: str,
+                            group_column_second: str) -> pd.DataFrame:
+    """
+    Perform the name matching based on the subgroups as indicated by the group_column strings. First by doing
+    a perfect string match with a merge statement, followed by the fuzzy matching approach as done in NameMatcher. 
+    ----------
+    matcher: NameMatcher
+        The NameMatcher to be used for the name matching part        
+    data_first: pd.DataFrame
+        The first dataframe or series used for the name matching        
+    data_second: pd.DataFrame
+        The second dataframe or series used for the name matching        
+    name_column: str
+        The column in which the name that should be matched can be found for both dataframes
+    group_column_first: str
+        The name of the column that should be used to generate groups within the data.
+    group_column_second: str
+        The name of the column that should be used to generate groups within the data.
+
+    Returns
+    -------
+    pd.DataFrame
+        A dataframe containing the original name, matched name, match score and match index. The index of the
+        dataframe is equal to the original index of data_first, the match index is the index in data_second
+        for the matched name.
+    """
+
+    matches = _match_names_combine_data(data_first, data_second, [
+                            name_column, group_column_first], [name_column, group_column_second])
+    unmatched = data_first[~data_first.index.isin(matches.index)]
+    if len(unmatched) > 0:
+        matcher.load_and_process_master_data(name_column, data_second, transform=False)
+        for group in data_first[group_column_first].unique():
+            data_second_group = data_second[data_second[group_column_second] == group].copy()
+            matcher.load_and_process_master_data(name_column, 
+                data_second_group, start_processing=False)
+            matcher.transform_data()
+            matches = pd.concat([matches, matcher.match_names(
+                to_be_matched=unmatched[unmatched[group_column_first] == group].copy(), column_matching=name_column)])
+    else:
+        print('All data matched with basic string matching')
+        return matches
+
+    return matches
+
+
+def match_names(data_first: Union[pd.DataFrame, pd.Series],
+                data_second: Union[pd.DataFrame, pd.Series],
+                column_first='',
+                column_second='',
+                group_column_first='',
+                group_column_second='',
+                case_sensitive=False,
+                punctuation_sensitive=False,
+                special_character_sensitive=False,
+                threshold=95,
+                **kwargs) -> pd.DataFrame:
+    """Function which performs name matching. First a simple merge on the data is performed
+    to get the instances in which the name matches perfectly. Subsequently the matches are
+    matched using the name matching algorithm as defined in name_matcher.
+
+    Parameters
+    ----------
+    data_first: Union[pd.DataFrame, pd.Series]
+        The first dataframe or series used for the name matching
+    data_second: Union[pd.DataFrame, pd.Series]
+        The second dataframe or series used for the name matching, for matching the data to 
+        itself data_second should be equal to data first
+    column_first: str
+        If data_first is a dataframe column_first should be the column in which the name 
+        that should be matched can be found for data_first
+        default=''
+    column_second: str
+        If data_second is a dataframe column_second should be the column in which the name 
+        that should be matched can be found for data_second
+        default=''
+    group_column_first: str
+        The name of the column that should be used to generate groups within the data_first 
+        dataframe. The matchig is then only performed for instances in which the groups are
+        identical
+        default=''
+    group_column_second: str
+        The name of the column that should be used to generate groups within the data_second 
+        dataframe. The matchig is then only performed for instances in which the groups are
+        identical
+        default=''
+    case_sensitive: bool
+        Boolean value indicating whether the names should be converted to lower case names
+        before the name matching starts. If False all the characters are converted to lowercase
+        default=False
+    punctuation_sensitive: bool
+        Boolean value indicating whether punctuations should be removed from the original names
+        before the name matching starts. If False the punctuations are removed
+        default=False
+    special_character_sensitive: bool
+        Boolean value indicating whether special characters should be converted to unicode
+        before the name matching starts. If False the special characters are replaced
+        default=False
+    threshold: int
+        the minimal score a match should have to be part of the output
+        default=95
+    **kwargs
+        Additional inputs for the name_matcher
+
+    Returns
+    -------
+    pd.DataFrame
+        A dataframe containing the matched rows were the match score is above the threshold. The
+        dataframe consists of 4 columns; original_name: the original name from data_first after 
+        preprocessing, match_name_0: the name it is matched to from data_second after preprocessing,
+        score_0: the score of the match, match_index_0: the index of the match in data_second. The 
+        match_index_0 can be used to join the data from both dataframes. 
+    """
+    if 'number_of_matches' in kwargs:
+        raise ValueError(
+            'The number of matches can only be changed by using a custom matching approach')
+
+    data_first = _match_names_check_data(data_first, column_first, group_column_first)
+    data_second = _match_names_check_data(data_second, column_second, group_column_second)
+
+    name_column = 'name_matching_data'
+
+    if ((group_column_first == '') & (group_column_second != '')) | ((group_column_second == '') & (group_column_first != '')):
+        raise ValueError(
+            'For the grouping to work both the grouping column in the first as well as the second dataframe have to be indicated')
+
+    if (threshold > 100) | (threshold < 0):
+        raise ValueError('Please pick a threshold between 0 and 100')
+
+    data_first, data_second = _match_names_preprocess_data(name_column, data_first, 
+            data_second, case_sensitive, punctuation_sensitive, special_character_sensitive)
+
+    matcher = NameMatcher(**kwargs)
+
+    if group_column_first == '':
+        matches = _match_names_match_single(matcher, data_first, data_second, name_column)
+    else:
+        matches = _match_names_match_group(matcher, data_first, data_second,
+                              name_column, group_column_first, group_column_second)
+
+    return matches[matches['score'] > threshold]
```

### Comparing `name_matching-0.8.8/name_matching/sparse_cosine.py` & `name_matching-0.8.9/name_matching/sparse_cosine.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,154 +1,154 @@
-import numpy as np
-from tqdm import tqdm
-# from numba import jit
-from scipy.sparse import csc_matrix, coo_matrix
-from typing import Union
-
-# @jit(nopython=True, fastmath=True)
-def _sparse_cosine_low_memory(matrix_row: np.array,
-                              matrix_col: np.array,
-                              matrix_data: np.array,
-                              matrix_len: int,
-                              vector_ind: np.array,
-                              vector_data: np.array) -> np.array:
-    """
-    A sparse cosine simularity calculation between a matrix and a vector. The sparse matrix should be sorted
-    in ascending order based on the matrix_col values. The vector should be sorted based on the indexes in 
-    ascending order.
-
-    Parameters
-    ----------
-    matrix_row : np.array
-        The row indices of the ngrams matrix of the matching data
-    matrix_col : np.array
-        The column indices of the ngrams matrix of the matching data in ascending order
-    matrix_data : np.array
-        The data of the ngrams matrix of the matching data
-    matrix_len : int
-        The length (number of rows) of the ngrams matrix of the matching data
-    vector_ind : np.array
-        The indices of the ngrams vector of the to be matched data
-    vector_data : np.array
-        The data of the ngrams vector of the to be matched data
-
-    Returns
-    -------
-    np.array
-        The cosine simularity between each of the rows of the matrix and the vector
-
-    """
-    ind = 0
-    res = np.zeros(matrix_len, np.float32)
-    for mat_ind in range(len(matrix_col)):
-        col = matrix_col[mat_ind]
-        if col > vector_ind[ind]:
-            ind = ind + 1
-            if ind == len(vector_ind):
-                break
-        if col == vector_ind[ind]:
-            res[matrix_row[mat_ind]] = res[matrix_row[mat_ind]] + \
-                matrix_data[mat_ind] * vector_data[ind]
-
-    return res
-
-
-def _sparse_cosine_top_n_standard(matrix_a: csc_matrix,
-                                  matrix_b: csc_matrix,
-                                  number_of_rows_at_once: int,
-                                  top_n: int,
-                                  verbose: bool) -> np.array:
-    """
-    A function for sparse matrix multiplication followed by an argpartition to
-    only take the top_n indexes.
-
-    Parameters
-    -------
-    matrix_a: csc_matric
-        The largest sparse csc matrix which should be multiplied
-    matrix_b: csc_matric
-        The smallest sparse csc matrix which should be multiplied
-    number_of_rows_at_once: int
-        The number of rows which should be processed at once, a lower
-        number of rows reduces the memory usage
-    top_n: int
-        The best n matches that should be returned
-    verbose: bool
-        A boolean indicating whether the progress should be printed
-
-    Returns
-    -------
-    np.array
-        The indexes for the n best sparse cosine matches between matrix a and b
-
-    """
-
-    results_arg = np.zeros(
-        (matrix_b.shape[0], top_n), dtype=np.float32)
-
-    # Split up the matrice in a certain number of rows
-    for j in tqdm(range(0, matrix_b.shape[0], number_of_rows_at_once), disable=not verbose):
-        number_of_rows_at_once_min = min(
-            [number_of_rows_at_once, matrix_b.shape[0]-j])
-        matrix_b_temp = matrix_b[j:j+number_of_rows_at_once_min, :]
-
-        # Calculate the matrix dot product
-        results_full = (matrix_a * (matrix_b_temp.T)).tocsc()
-
-        # For each of the rows of the original matrix select the argpartition
-        for i in range(number_of_rows_at_once_min):
-            results_full_temp = results_full.data[results_full.indptr[i]:results_full.indptr[i+1]]
-
-            # If there are more results then top_n only select the top_n results
-            if len(results_full_temp) > top_n:
-                ind = results_full.indices[results_full.indptr[i]:results_full.indptr[i+1]]
-                results_arg[j + i, :] = ind[np.argpartition(
-                    results_full_temp, -top_n)[-top_n:]]
-            
-            # else just select all the results
-            else:
-                results_arg[j + i, :len(results_full_temp)
-                            ] = results_full.indices[results_full.indptr[i]:results_full.indptr[i+1]]
-    return results_arg
-
-def sparse_cosine_top_n(matrix_a: Union[csc_matrix, coo_matrix], 
-                        matrix_b: csc_matrix, 
-                        top_n: int, 
-                        low_memory: bool,
-                        number_of_rows: int,
-                        verbose: bool):
-    """
-    Calculates the top_n cosine matches between matrix_a and matrix_b. Takes into account
-    the amount of  memory that should be used based on the low_memory int
-
-    Parameters
-    -------
-    matrix_a: csc_matric
-        The largest sparse csc matrix which should be multiplied
-    matrix_b: csc_matric
-        The smallest sparse csc matrix which should be multiplied
-    top_n: int
-        The best n matches that should be returned
-    low_memory: bool
-        A bool indicating whether the low memory sparse cosine approach should be used
-    number_of_rows: int
-        An int inidcating the number of rows which should be 
-        processed at once when calculating the cosine simalarity
-    verbose: bool
-        A boolean indicating whether the progress should be printed
-
-    Returns
-    -------
-    np.array
-        The indexes for the n best sparse cosine matches between matrix a and b
-
-    """
-    if low_memory:
-        matrix_b.sort_indices()
-        res = _sparse_cosine_low_memory(matrix_a.row, matrix_a.col, matrix_a.data,
-                        matrix_a.shape[0], matrix_b.indices, matrix_b.data)
-
-        top_n_adjusted = -np.min([top_n, len(res)])
-
-        return np.argpartition(res, top_n_adjusted, axis=0)[top_n_adjusted:]
-    else:
+import numpy as np
+from tqdm import tqdm
+# from numba import jit
+from scipy.sparse import csc_matrix, coo_matrix
+from typing import Union
+
+# @jit(nopython=True, fastmath=True)
+def _sparse_cosine_low_memory(matrix_row: np.array,
+                              matrix_col: np.array,
+                              matrix_data: np.array,
+                              matrix_len: int,
+                              vector_ind: np.array,
+                              vector_data: np.array) -> np.array:
+    """
+    A sparse cosine simularity calculation between a matrix and a vector. The sparse matrix should be sorted
+    in ascending order based on the matrix_col values. The vector should be sorted based on the indexes in 
+    ascending order.
+
+    Parameters
+    ----------
+    matrix_row : np.array
+        The row indices of the ngrams matrix of the matching data
+    matrix_col : np.array
+        The column indices of the ngrams matrix of the matching data in ascending order
+    matrix_data : np.array
+        The data of the ngrams matrix of the matching data
+    matrix_len : int
+        The length (number of rows) of the ngrams matrix of the matching data
+    vector_ind : np.array
+        The indices of the ngrams vector of the to be matched data
+    vector_data : np.array
+        The data of the ngrams vector of the to be matched data
+
+    Returns
+    -------
+    np.array
+        The cosine simularity between each of the rows of the matrix and the vector
+
+    """
+    ind = 0
+    res = np.zeros(matrix_len, np.float32)
+    for mat_ind in range(len(matrix_col)):
+        col = matrix_col[mat_ind]
+        if col > vector_ind[ind]:
+            ind = ind + 1
+            if ind == len(vector_ind):
+                break
+        if col == vector_ind[ind]:
+            res[matrix_row[mat_ind]] = res[matrix_row[mat_ind]] + \
+                matrix_data[mat_ind] * vector_data[ind]
+
+    return res
+
+
+def _sparse_cosine_top_n_standard(matrix_a: csc_matrix,
+                                  matrix_b: csc_matrix,
+                                  number_of_rows_at_once: int,
+                                  top_n: int,
+                                  verbose: bool) -> np.array:
+    """
+    A function for sparse matrix multiplication followed by an argpartition to
+    only take the top_n indexes.
+
+    Parameters
+    -------
+    matrix_a: csc_matric
+        The largest sparse csc matrix which should be multiplied
+    matrix_b: csc_matric
+        The smallest sparse csc matrix which should be multiplied
+    number_of_rows_at_once: int
+        The number of rows which should be processed at once, a lower
+        number of rows reduces the memory usage
+    top_n: int
+        The best n matches that should be returned
+    verbose: bool
+        A boolean indicating whether the progress should be printed
+
+    Returns
+    -------
+    np.array
+        The indexes for the n best sparse cosine matches between matrix a and b
+
+    """
+
+    results_arg = np.zeros(
+        (matrix_b.shape[0], top_n), dtype=np.float32)
+
+    # Split up the matrice in a certain number of rows
+    for j in tqdm(range(0, matrix_b.shape[0], number_of_rows_at_once), disable=not verbose):
+        number_of_rows_at_once_min = min(
+            [number_of_rows_at_once, matrix_b.shape[0]-j])
+        matrix_b_temp = matrix_b[j:j+number_of_rows_at_once_min, :]
+
+        # Calculate the matrix dot product
+        results_full = (matrix_a * (matrix_b_temp.T)).tocsc()
+
+        # For each of the rows of the original matrix select the argpartition
+        for i in range(number_of_rows_at_once_min):
+            results_full_temp = results_full.data[results_full.indptr[i]:results_full.indptr[i+1]]
+
+            # If there are more results then top_n only select the top_n results
+            if len(results_full_temp) > top_n:
+                ind = results_full.indices[results_full.indptr[i]:results_full.indptr[i+1]]
+                results_arg[j + i, :] = ind[np.argpartition(
+                    results_full_temp, -top_n)[-top_n:]]
+            
+            # else just select all the results
+            else:
+                results_arg[j + i, :len(results_full_temp)
+                            ] = results_full.indices[results_full.indptr[i]:results_full.indptr[i+1]]
+    return results_arg
+
+def sparse_cosine_top_n(matrix_a: Union[csc_matrix, coo_matrix], 
+                        matrix_b: csc_matrix, 
+                        top_n: int, 
+                        low_memory: bool,
+                        number_of_rows: int,
+                        verbose: bool):
+    """
+    Calculates the top_n cosine matches between matrix_a and matrix_b. Takes into account
+    the amount of  memory that should be used based on the low_memory int
+
+    Parameters
+    -------
+    matrix_a: csc_matric
+        The largest sparse csc matrix which should be multiplied
+    matrix_b: csc_matric
+        The smallest sparse csc matrix which should be multiplied
+    top_n: int
+        The best n matches that should be returned
+    low_memory: bool
+        A bool indicating whether the low memory sparse cosine approach should be used
+    number_of_rows: int
+        An int inidcating the number of rows which should be 
+        processed at once when calculating the cosine simalarity
+    verbose: bool
+        A boolean indicating whether the progress should be printed
+
+    Returns
+    -------
+    np.array
+        The indexes for the n best sparse cosine matches between matrix a and b
+
+    """
+    if low_memory:
+        matrix_b.sort_indices()
+        res = _sparse_cosine_low_memory(matrix_a.row, matrix_a.col, matrix_a.data,
+                        matrix_a.shape[0], matrix_b.indices, matrix_b.data)
+
+        top_n_adjusted = -np.min([top_n, len(res)])
+
+        return np.argpartition(res, top_n_adjusted, axis=0)[top_n_adjusted:]
+    else:
         return _sparse_cosine_top_n_standard(matrix_a, matrix_b, number_of_rows, top_n, verbose)
```

### Comparing `name_matching-0.8.8/name_matching.egg-info/PKG-INFO` & `name_matching-0.8.9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,103 +1,89 @@
-Metadata-Version: 2.1
-Name: name-matching
-Version: 0.8.8
-Summary: A package for the matching of company names
-Author: Michiel Nijhuis
-Author-email: m.nijhuis@dnb.nl
-License: UNKNOWN
-Project-URL: Documentation, https://name-matching.readthedocs.io/en/latest/index.html
-Project-URL: Source Code, https://github.com/DeNederlandscheBank/name_matching
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
-[![name_matching](https://github.com/DeNederlandscheBank/name_matching/actions/workflows/python-app.yml/badge.svg?branch=main)](https://github.com/DeNederlandscheBank/name_matching/actions/workflows/python-app.yml)
-
-# Name matching
-
-Name matching is a Python package for the matching of company names. This package has been developed to match the names of companies from different databases together to allow them to be merged. The package has a number of options to determine how exact the matches should be and also for the selection of different name matching algorithms.
-
-For a more in-depth discussion of the name matching package please see the [company name matching](https://medium.com/dnb-data-science-hub/company-name-matching-6a6330710334) medium post
-
-
-## Installation
-
-The package can be installed via PiPy:
-
-```bash
-pip install name_matching
-```
-
-Alternatively you could install the package by downloading the repo, navigating to the folder and run the setup in pip locally
-
-```bash
-pip install .
-```
-
-## Usage
-
-To see example usage of the package you can use the notebook folder. An example of the usage is also given below
-```python
-import pandas as pd
-from name_matching.name_matcher import NameMatcher
-
-# define a dataset with bank names
-df_companies_a = pd.DataFrame({'Company name': [
-        'Industrial and Commercial Bank of China Limited',
-        'China Construction Bank',
-        'Agricultural Bank of China',
-        'Bank of China',
-        'JPMorgan Chase',
-        'Mitsubishi UFJ Financial Group',
-        'Bank of America',
-        'HSBC',
-        'BNP Paribas',
-        'CrÃ©dit Agricole']})
-
-# alter each of the bank names a bit to test the matching
-df_companies_b = pd.DataFrame({'name': [
-        'Bank of China Limited',
-        'Mitsubishi Financial Group',
-        'Construction Bank China',
-        'Agricultural Bank',
-        'Bank of Amerika',
-        'BNP Parisbas',
-        'JP Morgan Chase',
-        'HSCB',
-        'Industrial and Commercial Bank of China',
-        'Credite Agricole']})
-
-# initialise the name matcher
-matcher = NameMatcher(number_of_matches=1, 
-                      legal_suffixes=True, 
-                      common_words=False, 
-                      top_n=50, 
-                      verbose=True)
-
-# adjust the distance metrics to use
-matcher.set_distance_metrics(['bag', 'typo', 'refined_soundex'])
-
-# load the data to which the names should be matched
-matcher.load_and_process_master_data(column='Company name',
-                                     df_matching_data=df_companies_a, 
-                                     transform=True)
-
-# perform the name matching on the data you want matched
-matches = matcher.match_names(to_be_matched=df_companies_b, 
-                              column_matching='name')
-
-# combine the datasets based on the matches
-combined = pd.merge(df_companies_a, matches, how='left', left_index=True, right_on='match_index')
-combined = pd.merge(combined, df_companies_b, how='left', left_index=True, right_index=True)
-
-```
-
-## Contributing
-All contributions are welcome. For more substantial changes, please open an issue first to discuss what you would like to change.
-
-## License
-The code is licensed under the MIT/X license an extended version of the licence: [MIT](https://choosealicense.com/licenses/mit/)
-
-## Thanks
-Thanks to the work of implementing name matching algorithms done in the [Abydos package](https://github.com/chrislit/abydos). These form the basis of the name matching algorithms used in this package.
-
-
+[![name_matching](https://github.com/DeNederlandscheBank/name_matching/actions/workflows/python-app.yml/badge.svg?branch=main)](https://github.com/DeNederlandscheBank/name_matching/actions/workflows/python-app.yml)
+
+# Name matching
+
+Name matching is a Python package for the matching of company names. This package has been developed to match the names of companies from different databases together to allow them to be merged. The package has a number of options to determine how exact the matches should be and also for the selection of different name matching algorithms.
+
+For a more in-depth discussion of the name matching package please see the [company name matching](https://medium.com/dnb-data-science-hub/company-name-matching-6a6330710334) medium post
+
+
+## Installation
+
+The package can be installed via PiPy:
+
+```bash
+pip install name_matching
+```
+
+Alternatively you could install the package by downloading the repo, navigating to the folder and run the setup in pip locally
+
+```bash
+pip install .
+```
+
+## Usage
+
+To see example usage of the package you can use the notebook folder. An example of the usage is also given below
+```python
+import pandas as pd
+from name_matching.name_matcher import NameMatcher
+
+# define a dataset with bank names
+df_companies_a = pd.DataFrame({'Company name': [
+        'Industrial and Commercial Bank of China Limited',
+        'China Construction Bank',
+        'Agricultural Bank of China',
+        'Bank of China',
+        'JPMorgan Chase',
+        'Mitsubishi UFJ Financial Group',
+        'Bank of America',
+        'HSBC',
+        'BNP Paribas',
+        'Crédit Agricole']})
+
+# alter each of the bank names a bit to test the matching
+df_companies_b = pd.DataFrame({'name': [
+        'Bank of China Limited',
+        'Mitsubishi Financial Group',
+        'Construction Bank China',
+        'Agricultural Bank',
+        'Bank of Amerika',
+        'BNP Parisbas',
+        'JP Morgan Chase',
+        'HSCB',
+        'Industrial and Commercial Bank of China',
+        'Credite Agricole']})
+
+# initialise the name matcher
+matcher = NameMatcher(number_of_matches=1, 
+                      legal_suffixes=True, 
+                      common_words=False, 
+                      top_n=50, 
+                      verbose=True)
+
+# adjust the distance metrics to use
+matcher.set_distance_metrics(['bag', 'typo', 'refined_soundex'])
+
+# load the data to which the names should be matched
+matcher.load_and_process_master_data(column='Company name',
+                                     df_matching_data=df_companies_a, 
+                                     transform=True)
+
+# perform the name matching on the data you want matched
+matches = matcher.match_names(to_be_matched=df_companies_b, 
+                              column_matching='name')
+
+# combine the datasets based on the matches
+combined = pd.merge(df_companies_a, matches, how='left', left_index=True, right_on='match_index')
+combined = pd.merge(combined, df_companies_b, how='left', left_index=True, right_index=True)
+
+```
+
+## Contributing
+All contributions are welcome. For more substantial changes, please open an issue first to discuss what you would like to change.
+
+## License
+The code is licensed under the MIT/X license an extended version of the licence: [MIT](https://choosealicense.com/licenses/mit/)
+
+## Thanks
+Thanks to the work of implementing name matching algorithms done in the [Abydos package](https://github.com/chrislit/abydos). These form the basis of the name matching algorithms used in this package.
```

### Comparing `name_matching-0.8.8/name_matching.egg-info/SOURCES.txt` & `name_matching-0.8.9/name_matching.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `name_matching-0.8.8/setup.py` & `name_matching-0.8.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from setuptools import setup
-from pathlib import Path
-
-this_directory = Path(__file__).parent
-long_description = (this_directory / "README.md").read_text()
-
-setup(
-   name='name_matching',
-   version='0.8.8',
-   description='A package for the matching of company names',
-   author='Michiel Nijhuis',
-   author_email='m.nijhuis@dnb.nl',
-   project_urls = {
-        'Documentation': 'https://name-matching.readthedocs.io/en/latest/index.html',
-        'Source Code': 'https://github.com/DeNederlandscheBank/name_matching'},
-   packages=['name_matching','distances'],
-   install_requires = [
-			'cleanco',
-			'scikit-learn', 
-                        'pandas',
-                        'numpy',
-			'tqdm'],
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-)
+from setuptools import setup
+from pathlib import Path
+
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
+setup(
+   name='name_matching',
+   version='0.8.9',
+   description='A package for the matching of company names',
+   author='Michiel Nijhuis',
+   author_email='m.nijhuis@dnb.nl',
+   project_urls = {
+        'Documentation': 'https://name-matching.readthedocs.io/en/latest/index.html',
+        'Source Code': 'https://github.com/DeNederlandscheBank/name_matching'},
+   packages=['name_matching','distances'],
+   install_requires = [
+			'cleanco',
+			'scikit-learn', 
+                        'pandas',
+                        'numpy',
+			'tqdm'],
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+)
```

