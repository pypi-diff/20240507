# Comparing `tmp/python-negar-1.2.8.tar.gz` & `tmp/python-negar-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-negar-1.2.8.tar", last modified: Thu Sep 21 11:53:14 2023, max compression
+gzip compressed data, was "python-negar-1.2.9.tar", last modified: Mon May  6 22:28:04 2024, max compression
```

## Comparing `python-negar-1.2.8.tar` & `python-negar-1.2.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-09-21 11:53:14.515279 python-negar-1.2.8/
--rw-r--r--   0 javad     (1000) javad     (1000)       41 2022-03-28 12:11:27.000000 python-negar-1.2.8/AUTHORS
--rw-r--r--   0 javad     (1000) javad     (1000)     7141 2023-09-21 11:52:27.000000 python-negar-1.2.8/Changelog.txt
--rw-r--r--   0 javad     (1000) javad     (1000)    35147 2022-03-28 12:06:56.000000 python-negar-1.2.8/LICENSE
--rw-r--r--   0 javad     (1000) javad     (1000)      125 2023-06-15 16:17:35.000000 python-negar-1.2.8/MANIFEST.in
--rw-r--r--   0 javad     (1000) javad     (1000)     8548 2023-09-21 11:53:14.515279 python-negar-1.2.8/PKG-INFO
--rw-r--r--   0 javad     (1000) javad     (1000)     7590 2022-09-09 08:02:13.000000 python-negar-1.2.8/README.md
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-09-21 11:53:14.511946 python-negar-1.2.8/negar/
--rw-r--r--   0 javad     (1000) javad     (1000)       96 2022-03-28 12:34:31.000000 python-negar-1.2.8/negar/__init__.py
--rw-r--r--   0 javad     (1000) javad     (1000)     5164 2023-09-21 11:51:22.000000 python-negar-1.2.8/negar/constants.py
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-09-21 11:53:14.511946 python-negar-1.2.8/negar/data/
--rw-r--r--   0 javad     (1000) javad     (1000)        0 2022-03-28 12:06:56.000000 python-negar-1.2.8/negar/data/__init__.py
--rw-r--r--   0 javad     (1000) javad     (1000)    29312 2022-12-21 09:31:33.000000 python-negar-1.2.8/negar/data/untouchable.dat
--rw-r--r--   0 javad     (1000) javad     (1000)      346 2023-03-28 18:56:35.000000 python-negar-1.2.8/negar/gui.py
--rw-r--r--   0 javad     (1000) javad     (1000)    15377 2023-09-21 11:45:37.000000 python-negar-1.2.8/negar/virastar.py
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-09-21 11:53:14.515279 python-negar-1.2.8/python_negar.egg-info/
--rw-r--r--   0 javad     (1000) javad     (1000)     8548 2023-09-21 11:53:14.000000 python-negar-1.2.8/python_negar.egg-info/PKG-INFO
--rw-r--r--   0 javad     (1000) javad     (1000)      396 2023-09-21 11:53:14.000000 python-negar-1.2.8/python_negar.egg-info/SOURCES.txt
--rw-r--r--   0 javad     (1000) javad     (1000)        1 2023-09-21 11:53:14.000000 python-negar-1.2.8/python_negar.egg-info/dependency_links.txt
--rw-r--r--   0 javad     (1000) javad     (1000)       42 2023-09-21 11:53:14.000000 python-negar-1.2.8/python_negar.egg-info/entry_points.txt
--rw-r--r--   0 javad     (1000) javad     (1000)        6 2023-09-21 11:53:14.000000 python-negar-1.2.8/python_negar.egg-info/requires.txt
--rw-r--r--   0 javad     (1000) javad     (1000)        6 2023-09-21 11:53:14.000000 python-negar-1.2.8/python_negar.egg-info/top_level.txt
--rw-r--r--   0 javad     (1000) javad     (1000)       38 2023-09-21 11:53:14.515279 python-negar-1.2.8/setup.cfg
--rw-r--r--   0 javad     (1000) javad     (1000)     1543 2023-08-06 20:39:57.000000 python-negar-1.2.8/setup.py
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2024-05-06 22:28:04.816594 python-negar-1.2.9/
+-rw-r--r--   0 javad     (1000) javad     (1000)       41 2022-03-28 12:11:27.000000 python-negar-1.2.9/AUTHORS
+-rw-r--r--   0 javad     (1000) javad     (1000)     7287 2024-05-06 22:24:03.000000 python-negar-1.2.9/Changelog.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)    35147 2022-03-28 12:06:56.000000 python-negar-1.2.9/LICENSE
+-rw-r--r--   0 javad     (1000) javad     (1000)      125 2023-06-15 16:17:35.000000 python-negar-1.2.9/MANIFEST.in
+-rw-r--r--   0 javad     (1000) javad     (1000)     8548 2024-05-06 22:28:04.816594 python-negar-1.2.9/PKG-INFO
+-rw-r--r--   0 javad     (1000) javad     (1000)     7590 2022-09-09 08:02:13.000000 python-negar-1.2.9/README.md
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2024-05-06 22:28:04.816594 python-negar-1.2.9/negar/
+-rw-r--r--   0 javad     (1000) javad     (1000)       96 2022-03-28 12:34:31.000000 python-negar-1.2.9/negar/__init__.py
+-rw-r--r--   0 javad     (1000) javad     (1000)     5164 2024-05-06 22:08:03.000000 python-negar-1.2.9/negar/constants.py
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2024-05-06 22:28:04.816594 python-negar-1.2.9/negar/data/
+-rw-r--r--   0 javad     (1000) javad     (1000)        0 2022-03-28 12:06:56.000000 python-negar-1.2.9/negar/data/__init__.py
+-rw-r--r--   0 javad     (1000) javad     (1000)    29312 2022-12-21 09:31:33.000000 python-negar-1.2.9/negar/data/untouchable.dat
+-rw-r--r--   0 javad     (1000) javad     (1000)      346 2023-03-28 18:56:35.000000 python-negar-1.2.9/negar/gui.py
+-rw-r--r--   0 javad     (1000) javad     (1000)    15379 2024-05-06 22:12:21.000000 python-negar-1.2.9/negar/virastar.py
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2024-05-06 22:28:04.816594 python-negar-1.2.9/python_negar.egg-info/
+-rw-r--r--   0 javad     (1000) javad     (1000)     8548 2024-05-06 22:28:04.000000 python-negar-1.2.9/python_negar.egg-info/PKG-INFO
+-rw-r--r--   0 javad     (1000) javad     (1000)      396 2024-05-06 22:28:04.000000 python-negar-1.2.9/python_negar.egg-info/SOURCES.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)        1 2024-05-06 22:28:04.000000 python-negar-1.2.9/python_negar.egg-info/dependency_links.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)       42 2024-05-06 22:28:04.000000 python-negar-1.2.9/python_negar.egg-info/entry_points.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)        6 2024-05-06 22:28:04.000000 python-negar-1.2.9/python_negar.egg-info/requires.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)        6 2024-05-06 22:28:04.000000 python-negar-1.2.9/python_negar.egg-info/top_level.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)       38 2024-05-06 22:28:04.816594 python-negar-1.2.9/setup.cfg
+-rw-r--r--   0 javad     (1000) javad     (1000)     1543 2023-08-06 20:39:57.000000 python-negar-1.2.9/setup.py
```

### Comparing `python-negar-1.2.8/Changelog.txt` & `python-negar-1.2.9/Changelog.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+1.2.9 - 2024-05-07
+-- Fix subtle issue with untoucahle words which stick to nonliteral symbols like Parantheses
+-- new test for untoucahle words
+
 1.2.8 - 2023-09-21
 -- Fix subtle issue with triple dots at the end of sentence followed by another [?!.]
 
 1.2.7 - 2023-08-07
 -- Remove dot from saving directory under Windows OS.
 
 1.2.6 - 2023-08-07
```

### Comparing `python-negar-1.2.8/LICENSE` & `python-negar-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python-negar-1.2.8/PKG-INFO` & `python-negar-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-negar
-Version: 1.2.8
+Version: 1.2.9
 Summary: Negar is a spell corrector and Persian text editor
 Home-page: http://github.com/shahinism/python-negar
 Author: Shahin Azad
 Author-email: ishahinism@gmail.com
 Maintainer: Javad Razavian, Alireza Savand
 Maintainer-email: javadr@gmail.com, alireza.savand@gmail.com
 License: GPL
```

### Comparing `python-negar-1.2.8/README.md` & `python-negar-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `python-negar-1.2.8/negar/constants.py` & `python-negar-1.2.9/negar/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import platform
 from pathlib import Path
 
-__version__ = "1.2.8"
+__version__ = "1.2.9"
 
 DATAFILE = Path(__file__).parent.absolute() / "data/untouchable.dat"
 APPDATA = "AppData/Roaming/" if platform.system() == "Windows" else "."
 USERFILE = Path.home() / f"{APPDATA}python-negar"
 
 INFO = f"""قابلیت های ویراستار ' نگار  ' -- نسخه {__version__} :
 * جایگزینی
```

### Comparing `python-negar-1.2.8/negar/data/untouchable.dat` & `python-negar-1.2.9/negar/data/untouchable.dat`

 * *Files identical despite different names*

### Comparing `python-negar-1.2.8/negar/virastar.py` & `python-negar-1.2.9/negar/virastar.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,15 @@
     def fix_suffix_separate(self):
         """Put ZWNJ between a word with its suffix (haye, ...)."""
         exag = r"""
             تر(ی(ن)?)?|
             [تمش]ان|
             ها(ی(ی|ت|م|ش|تان|شان)?)?|""" if self._exaggerating_zwnj else ""
         regx = re.compile(
-            rf"""(\S+?) # not-greedy fetch to handle some case like هایشان instead شان
+            rf"""\b(\S+?) # not-greedy fetch to handle some case like هایشان instead شان
             ({exag}
             # تر(ی(ن)?)?
             # [تمش]ان|
             # ها(ی(ی|ت|م|ش|تان|شان)?)?|
             شناس(ی)?|
             گذار(ی)?|گزار(ی)?
             )\b""", re.VERBOSE,
```

### Comparing `python-negar-1.2.8/python_negar.egg-info/PKG-INFO` & `python-negar-1.2.9/python_negar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-negar
-Version: 1.2.8
+Version: 1.2.9
 Summary: Negar is a spell corrector and Persian text editor
 Home-page: http://github.com/shahinism/python-negar
 Author: Shahin Azad
 Author-email: ishahinism@gmail.com
 Maintainer: Javad Razavian, Alireza Savand
 Maintainer-email: javadr@gmail.com, alireza.savand@gmail.com
 License: GPL
```

### Comparing `python-negar-1.2.8/setup.py` & `python-negar-1.2.9/setup.py`

 * *Files identical despite different names*

