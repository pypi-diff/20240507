# Comparing `tmp/clean_loop_timer-0.0.4.tar.gz` & `tmp/clean_loop_timer-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clean_loop_timer-0.0.4.tar", last modified: Sun Oct  8 04:30:23 2023, max compression
+gzip compressed data, was "dist/clean_loop_timer-0.1.0.tar", last modified: Tue May  7 20:24:37 2024, max compression
```

## Comparing `clean_loop_timer-0.0.4.tar` & `clean_loop_timer-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 tylerlum  (1000) tylerlum  (1000)        0 2023-10-08 04:30:23.000000 clean_loop_timer-0.0.4/
--rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)     1066 2023-10-02 09:22:52.000000 clean_loop_timer-0.0.4/LICENSE
--rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)    13437 2023-10-08 04:30:23.000000 clean_loop_timer-0.0.4/PKG-INFO
--rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)    12827 2023-10-08 04:28:33.000000 clean_loop_timer-0.0.4/README.md
-drwxrwxr-x   0 tylerlum  (1000) tylerlum  (1000)        0 2023-10-08 04:30:23.000000 clean_loop_timer-0.0.4/clean_loop_timer/
--rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)       44 2023-10-02 10:29:17.000000 clean_loop_timer-0.0.4/clean_loop_timer/__init__.py
--rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)     5348 2023-10-08 04:24:58.000000 clean_loop_timer-0.0.4/clean_loop_timer/timers.py
-drwxrwxr-x   0 tylerlum  (1000) tylerlum  (1000)        0 2023-10-08 04:30:23.000000 clean_loop_timer-0.0.4/clean_loop_timer.egg-info/
--rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)    13437 2023-10-08 04:30:23.000000 clean_loop_timer-0.0.4/clean_loop_timer.egg-info/PKG-INFO
--rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)      281 2023-10-08 04:30:23.000000 clean_loop_timer-0.0.4/clean_loop_timer.egg-info/SOURCES.txt
--rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)        1 2023-10-08 04:30:23.000000 clean_loop_timer-0.0.4/clean_loop_timer.egg-info/dependency_links.txt
--rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)       21 2023-10-08 04:30:23.000000 clean_loop_timer-0.0.4/clean_loop_timer.egg-info/requires.txt
--rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)       17 2023-10-08 04:30:23.000000 clean_loop_timer-0.0.4/clean_loop_timer.egg-info/top_level.txt
--rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)       38 2023-10-08 04:30:23.000000 clean_loop_timer-0.0.4/setup.cfg
--rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)      958 2023-10-08 04:29:19.000000 clean_loop_timer-0.0.4/setup.py
+drwxrwxr-x   0 tylerlum  (1000) tylerlum  (1000)        0 2024-05-07 20:24:37.000000 clean_loop_timer-0.1.0/
+-rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)     1066 2023-10-02 09:22:52.000000 clean_loop_timer-0.1.0/LICENSE
+-rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)    12730 2024-05-07 20:24:37.000000 clean_loop_timer-0.1.0/PKG-INFO
+-rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)    12120 2024-05-07 20:23:20.000000 clean_loop_timer-0.1.0/README.md
+drwxrwxr-x   0 tylerlum  (1000) tylerlum  (1000)        0 2024-05-07 20:24:37.000000 clean_loop_timer-0.1.0/clean_loop_timer/
+-rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)       69 2024-05-07 20:22:11.000000 clean_loop_timer-0.1.0/clean_loop_timer/__init__.py
+-rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)     5348 2023-10-08 04:24:58.000000 clean_loop_timer-0.1.0/clean_loop_timer/timers.py
+drwxrwxr-x   0 tylerlum  (1000) tylerlum  (1000)        0 2024-05-07 20:24:37.000000 clean_loop_timer-0.1.0/clean_loop_timer.egg-info/
+-rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)    12730 2024-05-07 20:24:37.000000 clean_loop_timer-0.1.0/clean_loop_timer.egg-info/PKG-INFO
+-rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)      281 2024-05-07 20:24:37.000000 clean_loop_timer-0.1.0/clean_loop_timer.egg-info/SOURCES.txt
+-rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)        1 2024-05-07 20:24:37.000000 clean_loop_timer-0.1.0/clean_loop_timer.egg-info/dependency_links.txt
+-rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)       21 2024-05-07 20:24:37.000000 clean_loop_timer-0.1.0/clean_loop_timer.egg-info/requires.txt
+-rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)       17 2024-05-07 20:24:37.000000 clean_loop_timer-0.1.0/clean_loop_timer.egg-info/top_level.txt
+-rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)       38 2024-05-07 20:24:37.000000 clean_loop_timer-0.1.0/setup.cfg
+-rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)      958 2024-05-07 20:23:49.000000 clean_loop_timer-0.1.0/setup.py
```

### Comparing `clean_loop_timer-0.0.4/LICENSE` & `clean_loop_timer-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clean_loop_timer-0.0.4/PKG-INFO` & `clean_loop_timer-0.1.0/clean_loop_timer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: clean_loop_timer
-Version: 0.0.4
+Name: clean-loop-timer
+Version: 0.1.0
 Summary: Easy-to-use timer for profiling complex loops in dataset generation and neural network training
 Home-page: https://github.com/tylerlum/clean_loop_timer
 Author: Tyler Lum
 Author-email: tylergwlum@gmail.com
 License: UNKNOWN
 Keywords: python,profiling,timer,loop
 Platform: UNKNOWN
@@ -42,66 +42,46 @@
 ```
 from tqdm import tqdm
 import time
 
 from clean_loop_timer import LoopTimer
 
 loop_timer = LoopTimer()
-pbar = tqdm(range(100))
-for i in pbar:
+for i in tqdm(range(100)):
     with loop_timer.add_section_timer("test"):
         if i < 3:
             time.sleep(1.0)
         else:
             time.sleep(0.1)
 
     with loop_timer.add_section_timer("test2"):
         time.sleep(0.3)
 
-    section_times_df = loop_timer.get_section_times_df()
-    loop_timer.pretty_print_section_times(df=section_times_df)
-    pbar.set_description(
-        " | ".join(
-            [
-                f"{section_times_df['Section'].iloc[j]}: {section_times_df['Most Recent Time (ms)'].iloc[j]:.0f}"
-                for j in range(len(section_times_df))
-            ]
-        )
-    )
+    loop_timer.pretty_print_section_times()
 ```
 
 Full example with global loop timer:
 
 ```
 from tqdm import tqdm
 import time
 
 from clean_loop_timer import get_loop_timer_instance
 
-pbar = tqdm(range(100))
-for i in pbar:
+for i in tqdm(range(100)):
     with get_loop_timer_instance().add_section_timer("test"):
         if i < 3:
             time.sleep(1.0)
         else:
             time.sleep(0.1)
 
     with get_loop_timer_instance().add_section_timer("test2"):
         time.sleep(0.3)
 
-    section_times_df = get_loop_timer_instance().get_section_times_df()
-    get_loop_timer_instance().pretty_print_section_times(df=section_times_df)
-    pbar.set_description(
-        " | ".join(
-            [
-                f"{section_times_df['Section'].iloc[j]}: {section_times_df['Most Recent Time (ms)'].iloc[j]:.0f}"
-                for j in range(len(section_times_df))
-            ]
-        )
-    )
+    get_loop_timer_instance().pretty_print_section_times()
 ```
 
 
 Example output:
 
 ```
 (loop_timer_env) ➜  clean_loop_timer git:(main) ✗ python timers.py
```

### Comparing `clean_loop_timer-0.0.4/README.md` & `clean_loop_timer-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: clean_loop_timer
+Version: 0.1.0
+Summary: Easy-to-use timer for profiling complex loops in dataset generation and neural network training
+Home-page: https://github.com/tylerlum/clean_loop_timer
+Author: Tyler Lum
+Author-email: tylergwlum@gmail.com
+License: UNKNOWN
+Keywords: python,profiling,timer,loop
+Platform: UNKNOWN
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Debuggers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # clean_loop_timer
 
 Easy-to-use timer for profiling complex loops in dataset generation and neural network training
 
 # Installing
 
 Install:
@@ -25,66 +42,46 @@
 ```
 from tqdm import tqdm
 import time
 
 from clean_loop_timer import LoopTimer
 
 loop_timer = LoopTimer()
-pbar = tqdm(range(100))
-for i in pbar:
+for i in tqdm(range(100)):
     with loop_timer.add_section_timer("test"):
         if i < 3:
             time.sleep(1.0)
         else:
             time.sleep(0.1)
 
     with loop_timer.add_section_timer("test2"):
         time.sleep(0.3)
 
-    section_times_df = loop_timer.get_section_times_df()
-    loop_timer.pretty_print_section_times(df=section_times_df)
-    pbar.set_description(
-        " | ".join(
-            [
-                f"{section_times_df['Section'].iloc[j]}: {section_times_df['Most Recent Time (ms)'].iloc[j]:.0f}"
-                for j in range(len(section_times_df))
-            ]
-        )
-    )
+    loop_timer.pretty_print_section_times()
 ```
 
 Full example with global loop timer:
 
 ```
 from tqdm import tqdm
 import time
 
 from clean_loop_timer import get_loop_timer_instance
 
-pbar = tqdm(range(100))
-for i in pbar:
+for i in tqdm(range(100)):
     with get_loop_timer_instance().add_section_timer("test"):
         if i < 3:
             time.sleep(1.0)
         else:
             time.sleep(0.1)
 
     with get_loop_timer_instance().add_section_timer("test2"):
         time.sleep(0.3)
 
-    section_times_df = get_loop_timer_instance().get_section_times_df()
-    get_loop_timer_instance().pretty_print_section_times(df=section_times_df)
-    pbar.set_description(
-        " | ".join(
-            [
-                f"{section_times_df['Section'].iloc[j]}: {section_times_df['Most Recent Time (ms)'].iloc[j]:.0f}"
-                for j in range(len(section_times_df))
-            ]
-        )
-    )
+    get_loop_timer_instance().pretty_print_section_times()
 ```
 
 
 Example output:
 
 ```
 (loop_timer_env) ➜  clean_loop_timer git:(main) ✗ python timers.py
@@ -258,7 +255,9 @@
     loop_timer.pretty_print_section_times()
 
     if batch_idx < len(dataloader) - 1:  # Avoid starting timer at end of last batch
         dataload_section_timer = loop_timer.add_section_timer("Data").start()
 ```
 
 Note how the manual timing results in many error-prone variables and messy print statements, but the loop timer results in clean uses of `with` statements that act as section comments.
+
+
```

### Comparing `clean_loop_timer-0.0.4/clean_loop_timer/timers.py` & `clean_loop_timer-0.1.0/clean_loop_timer/timers.py`

 * *Files identical despite different names*

### Comparing `clean_loop_timer-0.0.4/clean_loop_timer.egg-info/PKG-INFO` & `clean_loop_timer-0.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: clean-loop-timer
-Version: 0.0.4
-Summary: Easy-to-use timer for profiling complex loops in dataset generation and neural network training
-Home-page: https://github.com/tylerlum/clean_loop_timer
-Author: Tyler Lum
-Author-email: tylergwlum@gmail.com
-License: UNKNOWN
-Keywords: python,profiling,timer,loop
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Debuggers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # clean_loop_timer
 
 Easy-to-use timer for profiling complex loops in dataset generation and neural network training
 
 # Installing
 
 Install:
@@ -42,66 +25,46 @@
 ```
 from tqdm import tqdm
 import time
 
 from clean_loop_timer import LoopTimer
 
 loop_timer = LoopTimer()
-pbar = tqdm(range(100))
-for i in pbar:
+for i in tqdm(range(100)):
     with loop_timer.add_section_timer("test"):
         if i < 3:
             time.sleep(1.0)
         else:
             time.sleep(0.1)
 
     with loop_timer.add_section_timer("test2"):
         time.sleep(0.3)
 
-    section_times_df = loop_timer.get_section_times_df()
-    loop_timer.pretty_print_section_times(df=section_times_df)
-    pbar.set_description(
-        " | ".join(
-            [
-                f"{section_times_df['Section'].iloc[j]}: {section_times_df['Most Recent Time (ms)'].iloc[j]:.0f}"
-                for j in range(len(section_times_df))
-            ]
-        )
-    )
+    loop_timer.pretty_print_section_times()
 ```
 
 Full example with global loop timer:
 
 ```
 from tqdm import tqdm
 import time
 
 from clean_loop_timer import get_loop_timer_instance
 
-pbar = tqdm(range(100))
-for i in pbar:
+for i in tqdm(range(100)):
     with get_loop_timer_instance().add_section_timer("test"):
         if i < 3:
             time.sleep(1.0)
         else:
             time.sleep(0.1)
 
     with get_loop_timer_instance().add_section_timer("test2"):
         time.sleep(0.3)
 
-    section_times_df = get_loop_timer_instance().get_section_times_df()
-    get_loop_timer_instance().pretty_print_section_times(df=section_times_df)
-    pbar.set_description(
-        " | ".join(
-            [
-                f"{section_times_df['Section'].iloc[j]}: {section_times_df['Most Recent Time (ms)'].iloc[j]:.0f}"
-                for j in range(len(section_times_df))
-            ]
-        )
-    )
+    get_loop_timer_instance().pretty_print_section_times()
 ```
 
 
 Example output:
 
 ```
 (loop_timer_env) ➜  clean_loop_timer git:(main) ✗ python timers.py
@@ -275,9 +238,7 @@
     loop_timer.pretty_print_section_times()
 
     if batch_idx < len(dataloader) - 1:  # Avoid starting timer at end of last batch
         dataload_section_timer = loop_timer.add_section_timer("Data").start()
 ```
 
 Note how the manual timing results in many error-prone variables and messy print statements, but the loop timer results in clean uses of `with` statements that act as section comments.
-
-
```

### Comparing `clean_loop_timer-0.0.4/setup.py` & `clean_loop_timer-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
-VERSION = "0.0.4"
+VERSION = "0.1.0"
 DESCRIPTION = "Easy-to-use timer for profiling complex loops in dataset generation and neural network training"
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="clean_loop_timer",
     version=VERSION,
```

