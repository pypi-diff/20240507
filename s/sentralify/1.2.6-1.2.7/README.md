# Comparing `tmp/sentralify-1.2.6.tar.gz` & `tmp/sentralify-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentralify-1.2.6.tar", last modified: Thu Apr 11 20:49:17 2024, max compression
+gzip compressed data, was "sentralify-1.2.7.tar", last modified: Tue May  7 21:17:49 2024, max compression
```

## Comparing `sentralify-1.2.6.tar` & `sentralify-1.2.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-04-11 20:49:17.538726 sentralify-1.2.6/
--rw-r--r--   0 James     (1000) James     (1000)    35129 2024-02-09 23:22:38.000000 sentralify-1.2.6/LICENSE
--rw-r--r--   0 James     (1000) James     (1000)    57814 2024-04-11 20:49:17.538726 sentralify-1.2.6/PKG-INFO
--rw-r--r--   0 James     (1000) James     (1000)    16607 2024-04-11 20:49:16.000000 sentralify-1.2.6/README.md
--rw-r--r--   0 James     (1000) James     (1000)      884 2024-04-11 20:49:13.000000 sentralify-1.2.6/pyproject.toml
--rw-r--r--   0 James     (1000) James     (1000)       38 2024-04-11 20:49:17.538726 sentralify-1.2.6/setup.cfg
--rw-r--r--   0 James     (1000) James     (1000)       38 2024-02-12 20:14:52.000000 sentralify-1.2.6/setup.py
-drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-04-11 20:49:17.535393 sentralify-1.2.6/src/
-drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-04-11 20:49:17.535393 sentralify-1.2.6/src/sentralify/
--rw-r--r--   0 James     (1000) James     (1000)     4095 2024-04-11 20:49:16.000000 sentralify-1.2.6/src/sentralify/__init__.py
--rw-r--r--   0 James     (1000) James     (1000)    18560 2024-04-11 20:49:16.000000 sentralify-1.2.6/src/sentralify/generators.py
--rw-r--r--   0 James     (1000) James     (1000)    13062 2024-04-11 20:49:16.000000 sentralify-1.2.6/src/sentralify/scrapers.py
-drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-04-11 20:49:17.535393 sentralify-1.2.6/src/sentralify.egg-info/
--rw-r--r--   0 James     (1000) James     (1000)    57814 2024-04-11 20:49:17.000000 sentralify-1.2.6/src/sentralify.egg-info/PKG-INFO
--rw-r--r--   0 James     (1000) James     (1000)      313 2024-04-11 20:49:17.000000 sentralify-1.2.6/src/sentralify.egg-info/SOURCES.txt
--rw-r--r--   0 James     (1000) James     (1000)        1 2024-04-11 20:49:17.000000 sentralify-1.2.6/src/sentralify.egg-info/dependency_links.txt
--rw-r--r--   0 James     (1000) James     (1000)       97 2024-04-11 20:49:17.000000 sentralify-1.2.6/src/sentralify.egg-info/requires.txt
--rw-r--r--   0 James     (1000) James     (1000)       11 2024-04-11 20:49:17.000000 sentralify-1.2.6/src/sentralify.egg-info/top_level.txt
+drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-05-07 21:17:49.012364 sentralify-1.2.7/
+-rw-r--r--   0 James     (1000) James     (1000)    35129 2024-02-09 23:22:38.000000 sentralify-1.2.7/LICENSE
+-rw-r--r--   0 James     (1000) James     (1000)    57913 2024-05-07 21:17:49.012364 sentralify-1.2.7/PKG-INFO
+-rw-r--r--   0 James     (1000) James     (1000)    16706 2024-05-07 21:17:47.000000 sentralify-1.2.7/README.md
+-rw-r--r--   0 James     (1000) James     (1000)      884 2024-05-07 21:17:44.000000 sentralify-1.2.7/pyproject.toml
+-rw-r--r--   0 James     (1000) James     (1000)       38 2024-05-07 21:17:49.012364 sentralify-1.2.7/setup.cfg
+-rw-r--r--   0 James     (1000) James     (1000)       38 2024-02-12 20:14:52.000000 sentralify-1.2.7/setup.py
+drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-05-07 21:17:49.012364 sentralify-1.2.7/src/
+drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-05-07 21:17:49.012364 sentralify-1.2.7/src/sentralify/
+-rw-r--r--   0 James     (1000) James     (1000)     4026 2024-05-07 21:17:47.000000 sentralify-1.2.7/src/sentralify/__init__.py
+-rw-r--r--   0 James     (1000) James     (1000)    18754 2024-05-07 21:17:47.000000 sentralify-1.2.7/src/sentralify/generators.py
+-rw-r--r--   0 James     (1000) James     (1000)    13062 2024-05-07 21:17:47.000000 sentralify-1.2.7/src/sentralify/scrapers.py
+drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-05-07 21:17:49.012364 sentralify-1.2.7/src/sentralify.egg-info/
+-rw-r--r--   0 James     (1000) James     (1000)    57913 2024-05-07 21:17:49.000000 sentralify-1.2.7/src/sentralify.egg-info/PKG-INFO
+-rw-r--r--   0 James     (1000) James     (1000)      313 2024-05-07 21:17:49.000000 sentralify-1.2.7/src/sentralify.egg-info/SOURCES.txt
+-rw-r--r--   0 James     (1000) James     (1000)        1 2024-05-07 21:17:49.000000 sentralify-1.2.7/src/sentralify.egg-info/dependency_links.txt
+-rw-r--r--   0 James     (1000) James     (1000)       97 2024-05-07 21:17:49.000000 sentralify-1.2.7/src/sentralify.egg-info/requires.txt
+-rw-r--r--   0 James     (1000) James     (1000)       11 2024-05-07 21:17:49.000000 sentralify-1.2.7/src/sentralify.egg-info/top_level.txt
```

### Comparing `sentralify-1.2.6/LICENSE` & `sentralify-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sentralify-1.2.6/PKG-INFO` & `sentralify-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentralify
-Version: 1.2.6
+Version: 1.2.7
 Summary: Scrape Sentral data and use it!
 Author-email: mario872 <jamesaglynn10@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -691,14 +691,16 @@
 Requires-Dist: lxml>=5.1.0
 Requires-Dist: markdownify>=0.11.6
 Requires-Dist: python-dateutil>=2.8.2
 
 # sentralify
 Scrape Sentral data and use it!
 
+A Web Interface to the data scraped by Sentralify can be found [here](https://jimmyscompany.top).
+
 Sentralify was designed to be an **unofficial** replacement for [get-sentral](https://github.com/J-J-B-J/get-sentral) a ***fantastic*** package developed by J-J-B-J and SuperHarmony910.
 Sentralify can scrape data from the new Sentral frontend. So far it can scrape:
  - Timetable
  - ICS Timetable
  - Awards
  - Attendance
  - Activites
```

### Comparing `sentralify-1.2.6/README.md` & `sentralify-1.2.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # sentralify
 Scrape Sentral data and use it!
 
+A Web Interface to the data scraped by Sentralify can be found [here](https://jimmyscompany.top).
+
 Sentralify was designed to be an **unofficial** replacement for [get-sentral](https://github.com/J-J-B-J/get-sentral) a ***fantastic*** package developed by J-J-B-J and SuperHarmony910.
 Sentralify can scrape data from the new Sentral frontend. So far it can scrape:
  - Timetable
  - ICS Timetable
  - Awards
  - Attendance
  - Activites
```

### Comparing `sentralify-1.2.6/pyproject.toml` & `sentralify-1.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sentralify"
-version = "1.2.6"
+version = "1.2.7"
 description = "Scrape Sentral data and use it!"
 readme = "README.md"
 authors = [{ name = "mario872", email = "jamesaglynn10@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `sentralify-1.2.6/src/sentralify/__init__.py` & `sentralify-1.2.7/src/sentralify/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,18 +40,15 @@
 
     Returns:
         dict: A dictionary with the timetable, notices, calendar, student details, and the amount of time it took to gather the data
     """
     
     start = time.time() # So that we can know how long it took to scrape the Sentral data
     
-    try:
-        p = sync_playwright().start() # Start a playwright instance
-    except playwright._impl._errors.Error:
-        pass
+    p = sync_playwright().start() # Start a playwright instance
     
     # Initialise the generators and scrapers
     Sentral = generators
     scraper = scrapers(config)
     
     if check_login: persistent = False
```

### Comparing `sentralify-1.2.6/src/sentralify/generators.py` & `sentralify-1.2.7/src/sentralify/generators.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,18 @@
                         timetable[timetable_day]['periods'][period]['end'] = None
                         timetable[timetable_day]['periods'][period]['start_time_date'] = None
                         timetable[timetable_day]['periods'][period]['end_time_date'] = None
                     
                     if current_day_data['period'][period]['lessons'] != []: # If it's a period without a lesson, then there's nothing in the lesson parameter
                         timetable[timetable_day]['periods'][period]['full_name'] = current_day_data['period'][period]['lessons'][0]['subject_name']
                         timetable[timetable_day]['periods'][period]['name'] = current_day_data['period'][period]['lessons'][0]['lesson_class_name']
-                        timetable[timetable_day]['periods'][period]['room'] = current_day_data['period'][period]['lessons'][0]['room_name']
+                        try:
+                            timetable[timetable_day]['periods'][period]['room'] = current_day_data['period'][period]['lessons'][0]['room_name']
+                        except KeyError: # If there's not set it to None:
+                            timetable[timetable_day]['periods'][period]['room'] = None
                         timetable[timetable_day]['periods'][period]['border_colour'] = current_day_data['period'][period]['lessons'][0]['class_border_colour']
                         timetable[timetable_day]['periods'][period]['background_colour'] = current_day_data['period'][period]['lessons'][0]['class_background_colour']
                         try: # This checks that there is a teacher during the lesson
                             timetable[timetable_day]['periods'][period]['teacher'] = current_day_data['period'][period]['lessons'][0]['teachers'][0] # The 0 at the end could be a mistake, if anyone knows, please open an issue
                         except KeyError: # If there's not set it to None
                             timetable[timetable_day]['periods'][period]['teacher'] = None
                     else: # If there isn't a lesson on, then it's not a proper period
```

### Comparing `sentralify-1.2.6/src/sentralify/scrapers.py` & `sentralify-1.2.7/src/sentralify/scrapers.py`

 * *Files identical despite different names*

### Comparing `sentralify-1.2.6/src/sentralify.egg-info/PKG-INFO` & `sentralify-1.2.7/src/sentralify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentralify
-Version: 1.2.6
+Version: 1.2.7
 Summary: Scrape Sentral data and use it!
 Author-email: mario872 <jamesaglynn10@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -691,14 +691,16 @@
 Requires-Dist: lxml>=5.1.0
 Requires-Dist: markdownify>=0.11.6
 Requires-Dist: python-dateutil>=2.8.2
 
 # sentralify
 Scrape Sentral data and use it!
 
+A Web Interface to the data scraped by Sentralify can be found [here](https://jimmyscompany.top).
+
 Sentralify was designed to be an **unofficial** replacement for [get-sentral](https://github.com/J-J-B-J/get-sentral) a ***fantastic*** package developed by J-J-B-J and SuperHarmony910.
 Sentralify can scrape data from the new Sentral frontend. So far it can scrape:
  - Timetable
  - ICS Timetable
  - Awards
  - Attendance
  - Activites
```

