# Comparing `tmp/EmpireStateRunUp-0.0.6.tar.gz` & `tmp/EmpireStateRunUp-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EmpireStateRunUp-0.0.6.tar", last modified: Fri Mar 29 19:47:27 2024, max compression
+gzip compressed data, was "EmpireStateRunUp-0.0.7.tar", last modified: Tue May  7 01:44:15 2024, max compression
```

## Comparing `EmpireStateRunUp-0.0.6.tar` & `EmpireStateRunUp-0.0.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 josevnz   (1000) josevnz   (1000)        0 2024-03-29 19:47:27.796290 EmpireStateRunUp-0.0.6/
-drwxr-xr-x   0 josevnz   (1000) josevnz   (1000)        0 2024-03-29 19:47:27.795290 EmpireStateRunUp-0.0.6/EmpireStateRunUp.egg-info/
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)     3471 2024-03-29 19:47:27.000000 EmpireStateRunUp-0.0.6/EmpireStateRunUp.egg-info/PKG-INFO
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)     1189 2024-03-29 19:47:27.000000 EmpireStateRunUp-0.0.6/EmpireStateRunUp.egg-info/SOURCES.txt
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)        1 2024-03-29 19:47:27.000000 EmpireStateRunUp-0.0.6/EmpireStateRunUp.egg-info/dependency_links.txt
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)      398 2024-03-29 19:47:27.000000 EmpireStateRunUp-0.0.6/EmpireStateRunUp.egg-info/entry_points.txt
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)      111 2024-03-29 19:47:27.000000 EmpireStateRunUp-0.0.6/EmpireStateRunUp.egg-info/requires.txt
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)       29 2024-03-29 19:47:27.000000 EmpireStateRunUp-0.0.6/EmpireStateRunUp.egg-info/top_level.txt
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    20137 2024-01-19 14:51:11.000000 EmpireStateRunUp-0.0.6/LICENSE
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)     3471 2024-03-29 19:47:27.796290 EmpireStateRunUp-0.0.6/PKG-INFO
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)     2724 2024-01-01 17:18:32.000000 EmpireStateRunUp-0.0.6/README.md
-drwxr-xr-x   0 josevnz   (1000) josevnz   (1000)        0 2024-03-29 19:47:27.791290 EmpireStateRunUp-0.0.6/empirestaterunup/
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)        0 2023-10-07 23:44:51.000000 EmpireStateRunUp-0.0.6/empirestaterunup/__init__.py
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)     6194 2024-03-29 19:46:08.000000 EmpireStateRunUp-0.0.6/empirestaterunup/analyze.py
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    19172 2024-03-29 19:46:08.000000 EmpireStateRunUp-0.0.6/empirestaterunup/apps.py
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)      262 2023-10-22 10:20:27.000000 EmpireStateRunUp-0.0.6/empirestaterunup/browser.tcss
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    20759 2023-10-28 14:39:38.000000 EmpireStateRunUp-0.0.6/empirestaterunup/country_codes.csv
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    21511 2024-03-29 19:46:08.000000 EmpireStateRunUp-0.0.6/empirestaterunup/data.py
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)      215 2023-11-26 23:53:15.000000 EmpireStateRunUp-0.0.6/empirestaterunup/five_numbers.tcss
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)      257 2023-11-26 23:53:15.000000 EmpireStateRunUp-0.0.6/empirestaterunup/outliers.tcss
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    32840 2023-11-26 23:53:15.000000 EmpireStateRunUp-0.0.6/empirestaterunup/results-first-level-2023.csv
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    97015 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.6/empirestaterunup/results-full-level-2023.csv
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)       65 2023-10-27 10:47:05.000000 EmpireStateRunUp-0.0.6/empirestaterunup/runner_details.tcss
--rwxr-xr-x   0 josevnz   (1000) josevnz   (1000)     7429 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.6/empirestaterunup/runners.py
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    12294 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.6/empirestaterunup/scrapper.py
-drwxr-xr-x   0 josevnz   (1000) josevnz   (1000)        0 2024-03-29 19:47:27.794290 EmpireStateRunUp-0.0.6/images/
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    26334 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.6/images/age_histogram.png
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    13114 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.6/images/age_plot.png
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)   479274 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.6/images/empire_state_runup.png
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    33396 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.6/images/esrm_outlier_first_screen.png
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    45546 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.6/images/esrm_outlier_runner_detail.png
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    26093 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.6/images/esru_age_box_plot.png
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)   188519 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.6/images/esru_browser.png
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)   119343 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.6/images/esru_numbers.svg
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    47801 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.6/images/esru_outlier-1.svg
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    82044 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.6/images/esru_outlier-2.svg
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    43577 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.6/images/gender_distribution.png
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)   122624 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.6/images/participants_per_country.png
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)   196079 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.6/images/race_runners_2023-12-31T18_35_53_558956.svg
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)     1408 2024-03-29 19:46:08.000000 EmpireStateRunUp-0.0.6/pyproject.toml
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)      110 2024-03-29 19:46:08.000000 EmpireStateRunUp-0.0.6/requirements.txt
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)       38 2024-03-29 19:47:27.796290 EmpireStateRunUp-0.0.6/setup.cfg
-drwxr-xr-x   0 josevnz   (1000) josevnz   (1000)        0 2024-03-29 19:47:27.795290 EmpireStateRunUp-0.0.6/test/
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)     3000 2024-03-29 19:46:08.000000 EmpireStateRunUp-0.0.6/test/test_analyze.py
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)     1239 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.6/test/test_app.py
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)     6081 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.6/test/test_data.py
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)     2147 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.6/test/test_scrapper.py
+drwxr-xr-x   0 josevnz   (1000) josevnz   (1000)        0 2024-05-07 01:44:15.206233 EmpireStateRunUp-0.0.7/
+drwxr-xr-x   0 josevnz   (1000) josevnz   (1000)        0 2024-05-07 01:44:15.199233 EmpireStateRunUp-0.0.7/EmpireStateRunUp.egg-info/
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)     3255 2024-05-07 01:44:15.000000 EmpireStateRunUp-0.0.7/EmpireStateRunUp.egg-info/PKG-INFO
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)     1188 2024-05-07 01:44:15.000000 EmpireStateRunUp-0.0.7/EmpireStateRunUp.egg-info/SOURCES.txt
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)        1 2024-05-07 01:44:15.000000 EmpireStateRunUp-0.0.7/EmpireStateRunUp.egg-info/dependency_links.txt
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)      396 2024-05-07 01:44:15.000000 EmpireStateRunUp-0.0.7/EmpireStateRunUp.egg-info/entry_points.txt
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)      111 2024-05-07 01:44:15.000000 EmpireStateRunUp-0.0.7/EmpireStateRunUp.egg-info/requires.txt
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)       29 2024-05-07 01:44:15.000000 EmpireStateRunUp-0.0.7/EmpireStateRunUp.egg-info/top_level.txt
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    20137 2024-01-19 14:51:11.000000 EmpireStateRunUp-0.0.7/LICENSE
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)     3255 2024-05-07 01:44:15.206233 EmpireStateRunUp-0.0.7/PKG-INFO
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)     2724 2024-01-01 17:18:32.000000 EmpireStateRunUp-0.0.7/README.md
+drwxr-xr-x   0 josevnz   (1000) josevnz   (1000)        0 2024-05-07 01:44:15.201233 EmpireStateRunUp-0.0.7/empirestaterunup/
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)        0 2023-10-07 23:44:51.000000 EmpireStateRunUp-0.0.7/empirestaterunup/__init__.py
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)     6194 2024-03-29 19:46:08.000000 EmpireStateRunUp-0.0.7/empirestaterunup/analyze.py
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    19172 2024-03-29 19:46:08.000000 EmpireStateRunUp-0.0.7/empirestaterunup/apps.py
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)      262 2023-10-22 10:20:27.000000 EmpireStateRunUp-0.0.7/empirestaterunup/browser.tcss
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    20759 2023-10-28 14:39:38.000000 EmpireStateRunUp-0.0.7/empirestaterunup/country_codes.csv
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    21505 2024-05-07 01:18:00.000000 EmpireStateRunUp-0.0.7/empirestaterunup/data.py
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)      215 2023-11-26 23:53:15.000000 EmpireStateRunUp-0.0.7/empirestaterunup/five_numbers.tcss
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)      257 2023-11-26 23:53:15.000000 EmpireStateRunUp-0.0.7/empirestaterunup/outliers.tcss
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    32840 2023-11-26 23:53:15.000000 EmpireStateRunUp-0.0.7/empirestaterunup/results-first-level-2023.csv
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    97015 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/empirestaterunup/results-full-level-2023.csv
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)       65 2023-10-27 10:47:05.000000 EmpireStateRunUp-0.0.7/empirestaterunup/runner_details.tcss
+-rwxr-xr-x   0 josevnz   (1000) josevnz   (1000)     7410 2024-05-07 01:16:59.000000 EmpireStateRunUp-0.0.7/empirestaterunup/runners.py
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    12292 2024-05-07 01:15:19.000000 EmpireStateRunUp-0.0.7/empirestaterunup/scraper.py
+drwxr-xr-x   0 josevnz   (1000) josevnz   (1000)        0 2024-05-07 01:44:15.205233 EmpireStateRunUp-0.0.7/images/
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    26334 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/images/age_histogram.png
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    13114 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/images/age_plot.png
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)   479274 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/images/empire_state_runup.png
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    33396 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/images/esrm_outlier_first_screen.png
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    45546 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/images/esrm_outlier_runner_detail.png
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    26093 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/images/esru_age_box_plot.png
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)   188519 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/images/esru_browser.png
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)   119343 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/images/esru_numbers.svg
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    47801 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/images/esru_outlier-1.svg
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    82044 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/images/esru_outlier-2.svg
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    43577 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/images/gender_distribution.png
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)   122624 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/images/participants_per_country.png
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)   196079 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/images/race_runners_2023-12-31T18_35_53_558956.svg
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)     1406 2024-05-07 01:27:29.000000 EmpireStateRunUp-0.0.7/pyproject.toml
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)      110 2024-03-29 19:46:08.000000 EmpireStateRunUp-0.0.7/requirements.txt
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)       38 2024-05-07 01:44:15.206233 EmpireStateRunUp-0.0.7/setup.cfg
+drwxr-xr-x   0 josevnz   (1000) josevnz   (1000)        0 2024-05-07 01:44:15.206233 EmpireStateRunUp-0.0.7/test/
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)     3000 2024-03-29 19:46:08.000000 EmpireStateRunUp-0.0.7/test/test_analyze.py
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)     1239 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/test/test_app.py
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)     6081 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/test/test_data.py
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)     2140 2024-05-07 01:15:55.000000 EmpireStateRunUp-0.0.7/test/test_scrapper.py
```

### Comparing `EmpireStateRunUp-0.0.6/EmpireStateRunUp.egg-info/PKG-INFO` & `EmpireStateRunUp-0.0.7/EmpireStateRunUp.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 Metadata-Version: 2.1
 Name: EmpireStateRunUp
-Version: 0.0.6
+Version: 0.0.7
 Summary: Collection of scripts to analyze the results of the 2023 Empire State Run Up race
 Author-email: Jose Vicente Nunez <kodegeek.com@protonmail.com>
 Keywords: running,race
 Classifier: Environment :: Console
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pandas==2.2.1
-Requires-Dist: textual-dev==1.5.1
-Requires-Dist: textual==0.54.0
-Requires-Dist: rich==13.7.1
-Requires-Dist: numpy==1.26.0
-Requires-Dist: matplotlib==3.8.3
-Requires-Dist: selenium==4.15.2
 
 # Empire State Run Up
 
 [![Downloads](https://static.pepy.tech/badge/EmpireStateRunUp)](https://pepy.tech/project/EmpireStateRunUp)
 
 ![empire_state_runup.png](images/empire_state_runup.png)
```

### Comparing `EmpireStateRunUp-0.0.6/EmpireStateRunUp.egg-info/SOURCES.txt` & `EmpireStateRunUp-0.0.7/EmpireStateRunUp.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 empirestaterunup/data.py
 empirestaterunup/five_numbers.tcss
 empirestaterunup/outliers.tcss
 empirestaterunup/results-first-level-2023.csv
 empirestaterunup/results-full-level-2023.csv
 empirestaterunup/runner_details.tcss
 empirestaterunup/runners.py
-empirestaterunup/scrapper.py
+empirestaterunup/scraper.py
 images/age_histogram.png
 images/age_plot.png
 images/empire_state_runup.png
 images/esrm_outlier_first_screen.png
 images/esrm_outlier_runner_detail.png
 images/esru_age_box_plot.png
 images/esru_browser.png
```

### Comparing `EmpireStateRunUp-0.0.6/LICENSE` & `EmpireStateRunUp-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.6/PKG-INFO` & `EmpireStateRunUp-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 Metadata-Version: 2.1
 Name: EmpireStateRunUp
-Version: 0.0.6
+Version: 0.0.7
 Summary: Collection of scripts to analyze the results of the 2023 Empire State Run Up race
 Author-email: Jose Vicente Nunez <kodegeek.com@protonmail.com>
 Keywords: running,race
 Classifier: Environment :: Console
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pandas==2.2.1
-Requires-Dist: textual-dev==1.5.1
-Requires-Dist: textual==0.54.0
-Requires-Dist: rich==13.7.1
-Requires-Dist: numpy==1.26.0
-Requires-Dist: matplotlib==3.8.3
-Requires-Dist: selenium==4.15.2
 
 # Empire State Run Up
 
 [![Downloads](https://static.pepy.tech/badge/EmpireStateRunUp)](https://pepy.tech/project/EmpireStateRunUp)
 
 ![empire_state_runup.png](images/empire_state_runup.png)
```

### Comparing `EmpireStateRunUp-0.0.6/README.md` & `EmpireStateRunUp-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.6/empirestaterunup/analyze.py` & `EmpireStateRunUp-0.0.7/empirestaterunup/analyze.py`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.6/empirestaterunup/apps.py` & `EmpireStateRunUp-0.0.7/empirestaterunup/apps.py`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.6/empirestaterunup/country_codes.csv` & `EmpireStateRunUp-0.0.7/empirestaterunup/country_codes.csv`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.6/empirestaterunup/data.py` & `EmpireStateRunUp-0.0.7/empirestaterunup/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Data loading logic, after web scrapping process is completed.
+Data loading logic, after web scraping process is completed.
 author: Jose Vicente Nunez <kodegeek.com@protonmail.com>
 """
 import csv
 import datetime
 import math
 import re
 from enum import Enum
@@ -88,15 +88,15 @@
     SIXTY_FIVE_FLOOR_TIME = '65th floor time'
     WAVE = "wave"
     LEVEL = "level"
     URL = "url"
 
 
 FIELD_NAMES = [x.value for x in RaceFields if x != RaceFields.URL]
-FIELD_NAMES_FOR_SCRAPPING = [x.value for x in RaceFields]
+FIELD_NAMES_FOR_SCRAPING = [x.value for x in RaceFields]
 FIELD_NAMES_AND_POS: Dict[RaceFields, int] = {}
 pos = 0
 for field in RaceFields:
     FIELD_NAMES_AND_POS[field] = pos
     pos += 1
 
 
@@ -120,15 +120,15 @@
     record = {}
     with open(raw_file, 'r') as raw_csv_file:
         reader = csv.DictReader(raw_csv_file)
         row: Dict[str, Any]
         for row in reader:
             try:
                 csv_field: str
-                for csv_field in FIELD_NAMES_FOR_SCRAPPING:
+                for csv_field in FIELD_NAMES_FOR_SCRAPING:
                     column_val = row[csv_field].strip()
                     if csv_field == RaceFields.BIB.value:
                         bib = int(column_val)
                         record[csv_field] = bib
                     elif csv_field in [
                         RaceFields.GENDER_POSITION.value,
                         RaceFields.DIVISION_POSITION.value,
@@ -181,15 +181,15 @@
             except IndexError:
                 raise
 
 
 def raw_copy_paste_read(raw_file: Path) -> Iterable[Dict[str, Any]]:
     """
     Read the whole RAW file, product of a manual copy and paste, return a clean version.
-    Deprecation warning: You should use the raw_csv_read() method on the file produced by the scrapper.
+    Deprecation warning: You should use the raw_csv_read() method on the file produced by the scraper.
     Each record looks like this (copy and paste from the website):
 
     NAME
     GENDER BIB CITY,STATE,COUNTRY
     OVERALL_POSITION
     GENDER_POSITION
     DIVISION_POSITION
@@ -203,15 +203,15 @@
     1
     1
     1
     53:00
     MIN/MI
     10:36
     ```
-    :param raw_file: Yes, copied and pasted all the 8 pages when started the project, before writing a scrapper :D
+    :param raw_file: Yes, copied and pasted all the 8 pages when started the project, before writing a scraper :D
     :return:
     """
     with open(raw_file, 'r') as file_data:
         tk_cnt = 0
         ln_cnt = 0
         record = {}
         info_pattern = re.compile("([A-Z]) (\\d+)Bib (\\d*)(.*)")
@@ -401,15 +401,15 @@
     df[RaceFields.SIXTY_FIVE_FLOOR_PACE.value] = df[RaceFields.SIXTY_FIVE_FLOOR_PACE.value].fillna(sixty_five_floor_pace_median)
     df[RaceFields.SIXTY_FIVE_FLOOR_TIME.value] = df[RaceFields.SIXTY_FIVE_FLOOR_TIME.value].fillna(sixty_five_floor_time_median)
 
     # Normalize BIB and make it the index
     df[RaceFields.BIB.value] = df[RaceFields.BIB.value].astype(int)
     df.set_index(RaceFields.BIB.value, inplace=True)
 
-    # URL was useful during scrapping, not needed for analysis
+    # URL was useful during scraping, not needed for analysis
     df.drop([RaceFields.URL.value], axis=1, inplace=True)
 
     return df
 
 
 def df_to_list_of_tuples(
         df: DataFrame,
```

### Comparing `EmpireStateRunUp-0.0.6/empirestaterunup/results-first-level-2023.csv` & `EmpireStateRunUp-0.0.7/empirestaterunup/results-first-level-2023.csv`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.6/empirestaterunup/results-full-level-2023.csv` & `EmpireStateRunUp-0.0.7/empirestaterunup/results-full-level-2023.csv`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.6/empirestaterunup/runners.py` & `EmpireStateRunUp-0.0.7/empirestaterunup/runners.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #!/usr/bin/env python
 """
 I wrote this script to normalize the data results from the 'Empire State Building Run-Up', October 4, 2023.
-The race results website doesn't offer an export option and quite honestly writing a web scrapper seemed to be overkill.
+The race results website doesn't offer an export option and quite honestly writing a web scraper seemed to be overkill.
 So just coping and pasting the 8 pages of results took less time, the data normalizer is quite simple and was used
 to generate a nicer CSV file.
 
 Author Jose Vicente Nunez (kodegeek.com@protonmail.com)
 """
 import csv
 from pathlib import Path
 from argparse import ArgumentParser
 import logging
 
 from matplotlib import pyplot as plt
 
 from empirestaterunup.apps import FiveNumberApp, OutlierApp, Plotter, BrowserApp
 from empirestaterunup.data import raw_copy_paste_read, FIELD_NAMES, load_data, load_country_details, RaceFields, \
-    raw_csv_read, FIELD_NAMES_FOR_SCRAPPING
-from empirestaterunup.scrapper import RacerLinksScrapper, RacerDetailsScrapper
+    raw_csv_read, FIELD_NAMES_FOR_SCRAPING
+from empirestaterunup.scraper import RacerLinksScraper, RacerDetailsScraper
 
 logging.basicConfig(format='%(asctime)s %(message)s', encoding='utf-8', level=logging.INFO)
 
 
 def run_raw_cleaner():
     parser = ArgumentParser(description=__doc__)
     parser.add_argument(
@@ -163,38 +163,38 @@
         country_data=country_df
     )
     app.title = f"Race runners".title()
     app.sub_title = f"Browse details: {app.df.shape[0]}"
     app.run()
 
 
-def run_scrapper():
-    parser = ArgumentParser(description="Website scrapper for race results")
+def run_scraper():
+    parser = ArgumentParser(description="Website scraper for race results")
     parser.add_argument(
         "report_file",
         action="store",
         type=Path,
-        help="Location of the final scrapping results"
+        help="Location of the final SCRAPING results"
     )
     options = parser.parse_args()
     report_file = Path(options.report_file)
     logging.info("Saving results to %s", report_file)
-    with RacerLinksScrapper(headless=True, debug=False) as link_scrapper:
-        total = len(link_scrapper.racers)
+    with RacerLinksScraper(headless=True, debug=False) as link_scraper:
+        total = len(link_scraper.racers)
         logging.info(f"Got {total} racer results")
         with open(report_file, 'w') as csv_file:
-            writer = csv.DictWriter(csv_file, fieldnames=FIELD_NAMES_FOR_SCRAPPING, quoting=csv.QUOTE_NONNUMERIC)
+            writer = csv.DictWriter(csv_file, fieldnames=FIELD_NAMES_FOR_SCRAPING, quoting=csv.QUOTE_NONNUMERIC)
             writer.writeheader()
-            for bib in link_scrapper.racers:
-                url = link_scrapper.racers[bib][RaceFields.URL.value]
+            for bib in link_scraper.racers:
+                url = link_scraper.racers[bib][RaceFields.URL.value]
                 logging.info(f"Processing BIB: {bib}, will fetch: {url}")
-                with RacerDetailsScrapper(racer=link_scrapper.racers[bib], debug_level=0) as rds:
+                with RacerDetailsScraper(racer=link_scraper.racers[bib], debug_level=0) as rds:
                     try:
-                        position = link_scrapper.racers[bib][RaceFields.OVERALL_POSITION.value]
-                        name = link_scrapper.racers[bib][RaceFields.NAME.value]
+                        position = link_scraper.racers[bib][RaceFields.OVERALL_POSITION.value]
+                        name = link_scraper.racers[bib][RaceFields.NAME.value]
                         writer.writerow(rds.racer)
                         logging.info(f"Wrote: name={name}, position={position}, {rds.racer}")
                     except ValueError as ve:
                         raise ValueError(f"row={rds.racer}", ve)
 
 
 def run_csv_cleaner():
@@ -215,15 +215,15 @@
         'report_file',
         type=Path,
         help='New report file'
     )
     OPTIONS = parser.parse_args()
     try:
         with open(OPTIONS.report_file, 'w', newline='') as csvfile:
-            writer = csv.DictWriter(csvfile, fieldnames=FIELD_NAMES_FOR_SCRAPPING, quoting=csv.QUOTE_NONNUMERIC)
+            writer = csv.DictWriter(csvfile, fieldnames=FIELD_NAMES_FOR_SCRAPING, quoting=csv.QUOTE_NONNUMERIC)
             writer.writeheader()
             for row in raw_csv_read(OPTIONS.raw_file):
                 try:
                     writer.writerow(row)
                     if OPTIONS.verbose:
                         logging.warning(row)
                 except ValueError as ve:
```

### Comparing `EmpireStateRunUp-0.0.6/empirestaterunup/scrapper.py` & `EmpireStateRunUp-0.0.7/empirestaterunup/scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from selenium.webdriver.support import expected_conditions
 
 from empirestaterunup.data import RaceFields, Level
 
 EMPIRE_STATE_2013_RACE_RESULTS = "https://www.athlinks.com/event/382111/results/Event/1062909/Course/2407855/Results"
 
 
-class RacerLinksScrapper:
+class RacerLinksScraper:
 
     def __init__(self, headless: bool = True, load_wait: int = 5, debug: bool = False):
         self.rank_to_bib: list[int] = []
         options = Options()
         if headless:
             options.add_argument("--headless")
         self.driver = webdriver.Firefox(options=options)
@@ -150,15 +150,15 @@
             expected_conditions.element_to_be_clickable((By.CSS_SELECTOR, f"div:nth-child({level}) > button")))
         # Bug on Selenium, trigger click with Javascript
         self.driver.execute_script("arguments[0].click();", button)
         sleep(2.5)
         return button
 
 
-class RacerDetailsScrapper:
+class RacerDetailsScraper:
 
     def __init__(self, racer: Dict[str, Any], headless: bool = True, load_wait: int = 5, debug_level: int = 0):
         options = Options()
         fp = webdriver.FirefoxProfile()
         service = webdriver.FirefoxService()
         if headless:
             options.add_argument("--headless")
```

### Comparing `EmpireStateRunUp-0.0.6/images/age_histogram.png` & `EmpireStateRunUp-0.0.7/images/age_histogram.png`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.6/images/age_plot.png` & `EmpireStateRunUp-0.0.7/images/age_plot.png`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.6/images/empire_state_runup.png` & `EmpireStateRunUp-0.0.7/images/empire_state_runup.png`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.6/images/esrm_outlier_first_screen.png` & `EmpireStateRunUp-0.0.7/images/esrm_outlier_first_screen.png`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.6/images/esrm_outlier_runner_detail.png` & `EmpireStateRunUp-0.0.7/images/esrm_outlier_runner_detail.png`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.6/images/esru_age_box_plot.png` & `EmpireStateRunUp-0.0.7/images/esru_age_box_plot.png`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.6/images/esru_browser.png` & `EmpireStateRunUp-0.0.7/images/esru_browser.png`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.6/images/esru_numbers.svg` & `EmpireStateRunUp-0.0.7/images/esru_numbers.svg`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.6/images/esru_outlier-1.svg` & `EmpireStateRunUp-0.0.7/images/esru_outlier-1.svg`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.6/images/esru_outlier-2.svg` & `EmpireStateRunUp-0.0.7/images/esru_outlier-2.svg`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.6/images/gender_distribution.png` & `EmpireStateRunUp-0.0.7/images/gender_distribution.png`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.6/images/participants_per_country.png` & `EmpireStateRunUp-0.0.7/images/participants_per_country.png`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.6/images/race_runners_2023-12-31T18_35_53_558956.svg` & `EmpireStateRunUp-0.0.7/images/race_runners_2023-12-31T18_35_53_558956.svg`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.6/pyproject.toml` & `EmpireStateRunUp-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "twine",
     "textual-dev"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "EmpireStateRunUp"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     {name = "Jose Vicente Nunez", email = "kodegeek.com@protonmail.com"},
 ]
 description = "Collection of scripts to analyze the results of the 2023 Empire State Run Up race"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["running", "race"]
@@ -23,15 +23,15 @@
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "Intended Audience :: End Users/Desktop",
     "Topic :: Utilities"
 ]
 dynamic = ["dependencies"]
 [project.scripts]
-esru_scrapper = "empirestaterunup.runners:run_scrapper"
+esru_scraper = "empirestaterunup.runners:run_scraper"
 esru_csv_cleaner = "empirestaterunup.runners:run_csv_cleaner"
 esru_raw_cleaner = "empirestaterunup.runners:run_raw_cleaner"
 esru_numbers = "empirestaterunup.runners:run_5_number"
 esru_outlier = "empirestaterunup.runners:run_outlier"
 esru_browser = "empirestaterunup.runners:run_browser"
 esru_plot = "empirestaterunup.runners:simple_plot"
```

### Comparing `EmpireStateRunUp-0.0.6/test/test_analyze.py` & `EmpireStateRunUp-0.0.7/test/test_analyze.py`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.6/test/test_app.py` & `EmpireStateRunUp-0.0.7/test/test_app.py`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.6/test/test_data.py` & `EmpireStateRunUp-0.0.7/test/test_data.py`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.6/test/test_scrapper.py` & `EmpireStateRunUp-0.0.7/test/test_scrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import logging
 import pprint
 import unittest
 
 from empirestaterunup.data import RaceFields
-from empirestaterunup.scrapper import RacerLinksScrapper, RacerDetailsScrapper
+from empirestaterunup.scraper import RacerLinksScraper, RacerDetailsScraper
 
 logger = logging.getLogger('selenium')
 logger.setLevel(logging.DEBUG)
 
 
-class RacerLinksScrapperTestCase(unittest.TestCase):
-    def test_link_scrapper(self):
-        with RacerLinksScrapper(headless=True, debug=False) as esc:
+class RacerLinksScraperTestCase(unittest.TestCase):
+    def test_link_scraper(self):
+        with RacerLinksScraper(headless=True, debug=False) as esc:
             self.assertIsNotNone(esc)
             self.assertEqual(377, len(esc.racers))
             self.assertEqual(377, len(esc.rank_to_bib))
 
     def test_runner_detail(self):
         racer_details = [
             {
@@ -34,15 +34,15 @@
                 RaceFields.NAME.value: 'HARPREET Sethi',
                 RaceFields.URL.value: 'https://www.athlinks.com/event/382111/results/Event/1062909/Course/2407855/Bib/434'
             }
         ]
         for racer in racer_details:
             name = racer[RaceFields.NAME.value]
             print(f"name={name}, url={racer[RaceFields.URL.value]}")
-            with RacerDetailsScrapper(
+            with RacerDetailsScraper(
                 racer=racer,
                 debug_level=0,
             ) as rds:
                 self.assertIsNotNone(rds)
                 self.assertIsNotNone(rds.racer)
                 for field in [
                     RaceFields.TIME.value,
```

