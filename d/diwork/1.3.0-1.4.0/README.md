# Comparing `tmp/diwork-1.3.0.tar.gz` & `tmp/diwork-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diwork-1.3.0.tar", last modified: Mon May  6 09:30:18 2024, max compression
+gzip compressed data, was "diwork-1.4.0.tar", last modified: Tue May  7 09:36:22 2024, max compression
```

## Comparing `diwork-1.3.0.tar` & `diwork-1.4.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-06 09:30:18.760968 diwork-1.3.0/
--rw-r--r--   0 the220th  (1000) the220th  (1000)     1066 2023-02-10 11:11:21.000000 diwork-1.3.0/LICENSE
--rw-r--r--   0 the220th  (1000) the220th  (1000)      116 2024-05-06 09:30:18.760968 diwork-1.3.0/PKG-INFO
--rw-r--r--   0 the220th  (1000) the220th  (1000)      211 2024-05-04 08:36:38.000000 diwork-1.3.0/README.md
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-06 09:30:18.753968 diwork-1.3.0/diwork/
--rw-r--r--   0 the220th  (1000) the220th  (1000)      343 2024-05-04 08:22:40.000000 diwork-1.3.0/diwork/__init__.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)      115 2024-05-04 08:01:22.000000 diwork-1.3.0/diwork/__main__.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)       47 2024-05-06 09:21:12.000000 diwork-1.3.0/diwork/__version__.py
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-06 09:30:18.759968 diwork-1.3.0/diwork/diwork_mains/
--rw-r--r--   0 the220th  (1000) the220th  (1000)      734 2024-05-04 08:48:21.000000 diwork-1.3.0/diwork/diwork_mains/__init__.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     5695 2024-05-06 09:17:43.000000 diwork-1.3.0/diwork/diwork_mains/diwork_archive.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     5118 2024-05-06 09:17:43.000000 diwork-1.3.0/diwork/diwork_mains/diwork_clone.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     7525 2024-05-06 09:17:44.000000 diwork-1.3.0/diwork/diwork_mains/diwork_diff.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     6710 2024-05-06 09:29:15.000000 diwork-1.3.0/diwork/diwork_mains/diwork_diffclone.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     3245 2024-05-06 09:17:43.000000 diwork-1.3.0/diwork/diwork_mains/diwork_difx.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     9183 2024-05-06 09:17:44.000000 diwork-1.3.0/diwork/diwork_mains/diwork_exec.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     5176 2024-05-06 09:17:43.000000 diwork-1.3.0/diwork/diwork_mains/diwork_hash.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)      582 2023-02-18 08:13:38.000000 diwork-1.3.0/diwork/diwork_mains/diwork_help.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     2902 2024-05-06 09:17:44.000000 diwork-1.3.0/diwork/diwork_mains/diwork_repeats.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     9066 2024-05-06 09:17:43.000000 diwork-1.3.0/diwork/diwork_mains/diwork_sshclone.py
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-06 09:30:18.760968 diwork-1.3.0/diwork/diwork_ways/
--rw-r--r--   0 the220th  (1000) the220th  (1000)      613 2024-05-06 09:17:43.000000 diwork-1.3.0/diwork/diwork_ways/__init__.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     1033 2024-05-04 10:29:33.000000 diwork-1.3.0/diwork/diwork_ways/diwork_parse.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)    11534 2024-05-06 09:18:41.000000 diwork-1.3.0/diwork/diwork_ways/diwork_sup.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     1390 2024-05-04 10:12:20.000000 diwork-1.3.0/diwork/main.py
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-06 09:30:18.760968 diwork-1.3.0/diwork.egg-info/
--rw-r--r--   0 the220th  (1000) the220th  (1000)      116 2024-05-06 09:30:18.000000 diwork-1.3.0/diwork.egg-info/PKG-INFO
--rw-r--r--   0 the220th  (1000) the220th  (1000)      795 2024-05-06 09:30:18.000000 diwork-1.3.0/diwork.egg-info/SOURCES.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)        1 2024-05-06 09:30:18.000000 diwork-1.3.0/diwork.egg-info/dependency_links.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)       44 2024-05-06 09:30:18.000000 diwork-1.3.0/diwork.egg-info/entry_points.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)       14 2024-05-06 09:30:18.000000 diwork-1.3.0/diwork.egg-info/requires.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)        7 2024-05-06 09:30:18.000000 diwork-1.3.0/diwork.egg-info/top_level.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)       81 2024-05-04 07:49:04.000000 diwork-1.3.0/pyproject.toml
--rw-r--r--   0 the220th  (1000) the220th  (1000)       38 2024-05-06 09:30:18.761968 diwork-1.3.0/setup.cfg
--rw-r--r--   0 the220th  (1000) the220th  (1000)      997 2024-05-04 08:57:56.000000 diwork-1.3.0/setup.py
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-07 09:36:22.185793 diwork-1.4.0/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     1066 2023-02-10 11:11:21.000000 diwork-1.4.0/LICENSE
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      116 2024-05-07 09:36:22.184794 diwork-1.4.0/PKG-INFO
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      211 2024-05-04 08:36:38.000000 diwork-1.4.0/README.md
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-07 09:36:22.146794 diwork-1.4.0/diwork/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      343 2024-05-04 08:22:40.000000 diwork-1.4.0/diwork/__init__.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      115 2024-05-04 08:01:22.000000 diwork-1.4.0/diwork/__main__.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       47 2024-05-07 08:09:50.000000 diwork-1.4.0/diwork/__version__.py
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-07 09:36:22.183794 diwork-1.4.0/diwork/diwork_mains/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      798 2024-05-07 09:23:33.000000 diwork-1.4.0/diwork/diwork_mains/__init__.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     5695 2024-05-06 09:17:43.000000 diwork-1.4.0/diwork/diwork_mains/diwork_archive.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     5118 2024-05-06 09:17:43.000000 diwork-1.4.0/diwork/diwork_mains/diwork_clone.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     5432 2024-05-07 09:26:18.000000 diwork-1.4.0/diwork/diwork_mains/diwork_contains.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     7525 2024-05-06 09:17:44.000000 diwork-1.4.0/diwork/diwork_mains/diwork_diff.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     6708 2024-05-07 08:10:15.000000 diwork-1.4.0/diwork/diwork_mains/diwork_diffclone.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     3245 2024-05-06 09:17:43.000000 diwork-1.4.0/diwork/diwork_mains/diwork_difx.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     9183 2024-05-06 09:17:44.000000 diwork-1.4.0/diwork/diwork_mains/diwork_exec.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     5176 2024-05-06 09:17:43.000000 diwork-1.4.0/diwork/diwork_mains/diwork_hash.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      582 2023-02-18 08:13:38.000000 diwork-1.4.0/diwork/diwork_mains/diwork_help.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     2902 2024-05-06 09:17:44.000000 diwork-1.4.0/diwork/diwork_mains/diwork_repeats.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     9066 2024-05-06 09:17:43.000000 diwork-1.4.0/diwork/diwork_mains/diwork_sshclone.py
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-07 09:36:22.184794 diwork-1.4.0/diwork/diwork_ways/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      613 2024-05-06 09:17:43.000000 diwork-1.4.0/diwork/diwork_ways/__init__.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     1033 2024-05-04 10:29:33.000000 diwork-1.4.0/diwork/diwork_ways/diwork_parse.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)    11534 2024-05-06 09:18:41.000000 diwork-1.4.0/diwork/diwork_ways/diwork_sup.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     1484 2024-05-07 09:24:20.000000 diwork-1.4.0/diwork/main.py
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-07 09:36:22.184794 diwork-1.4.0/diwork.egg-info/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      116 2024-05-07 09:36:22.000000 diwork-1.4.0/diwork.egg-info/PKG-INFO
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      834 2024-05-07 09:36:22.000000 diwork-1.4.0/diwork.egg-info/SOURCES.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)        1 2024-05-07 09:36:22.000000 diwork-1.4.0/diwork.egg-info/dependency_links.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       44 2024-05-07 09:36:22.000000 diwork-1.4.0/diwork.egg-info/entry_points.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       14 2024-05-07 09:36:22.000000 diwork-1.4.0/diwork.egg-info/requires.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)        7 2024-05-07 09:36:22.000000 diwork-1.4.0/diwork.egg-info/top_level.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       81 2024-05-04 07:49:04.000000 diwork-1.4.0/pyproject.toml
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       38 2024-05-07 09:36:22.185793 diwork-1.4.0/setup.cfg
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      997 2024-05-04 08:57:56.000000 diwork-1.4.0/setup.py
```

### Comparing `diwork-1.3.0/LICENSE` & `diwork-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `diwork-1.3.0/diwork/diwork_mains/__init__.py` & `diwork-1.4.0/diwork/diwork_mains/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,20 +9,22 @@
 from .diwork_difx import main_difx
 from .diwork_repeats import main_repeats
 from .diwork_exec import main_exec
 from .diwork_help import main_help
 from .diwork_sshclone import main_sshclone
 from .diwork_archive import main_archive
 from .diwork_diffclone import main_diffclone
+from .diwork_contains import main_contains
 
 __all__ = [
     "main_help",
     "main_hash",
     "main_clone",
     "main_diff",
     "main_difx",
     "main_repeats",
     "main_exec",
     "main_sshclone",
     "main_archive",
-    "main_diffclone"
+    "main_diffclone",
+    "main_contains"
 ]
```

### Comparing `diwork-1.3.0/diwork/diwork_mains/diwork_archive.py` & `diwork-1.4.0/diwork/diwork_mains/diwork_archive.py`

 * *Files identical despite different names*

### Comparing `diwork-1.3.0/diwork/diwork_mains/diwork_clone.py` & `diwork-1.4.0/diwork/diwork_mains/diwork_clone.py`

 * *Files identical despite different names*

### Comparing `diwork-1.3.0/diwork/diwork_mains/diwork_diff.py` & `diwork-1.4.0/diwork/diwork_mains/diwork_diff.py`

 * *Files identical despite different names*

### Comparing `diwork-1.3.0/diwork/diwork_mains/diwork_diffclone.py` & `diwork-1.4.0/diwork/diwork_mains/diwork_diffclone.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         file_i_rel = os.path.relpath(file_i, dir_path)
         d[file_i_rel] = get_hash_file(file_i)
     return d
 
 
 def main_diffclone(args: list):
     platform = sys.platform
-    parser = argparse.ArgumentParser(prog = "diwork diffclone",
+    parser = argparse.ArgumentParser(prog="diwork diffclone",
         description="This module will clone all the contents of {folder_src} to {folder_dest}, but only files, which does not already contains in {folder_dest}. "
                     "Old files will be renamed if needed.")
     parser.add_argument("folder_src", type=str, nargs=1,
                        help="Path to source directory")
     parser.add_argument("folder_dest", type=str, nargs=1,
                        help="Path to destination directory")
     parser.add_argument("--no_check_hash", default=False, action='store_true',
```

### Comparing `diwork-1.3.0/diwork/diwork_mains/diwork_difx.py` & `diwork-1.4.0/diwork/diwork_mains/diwork_difx.py`

 * *Files identical despite different names*

### Comparing `diwork-1.3.0/diwork/diwork_mains/diwork_exec.py` & `diwork-1.4.0/diwork/diwork_mains/diwork_exec.py`

 * *Files identical despite different names*

### Comparing `diwork-1.3.0/diwork/diwork_mains/diwork_hash.py` & `diwork-1.4.0/diwork/diwork_mains/diwork_hash.py`

 * *Files identical despite different names*

### Comparing `diwork-1.3.0/diwork/diwork_mains/diwork_help.py` & `diwork-1.4.0/diwork/diwork_mains/diwork_help.py`

 * *Files identical despite different names*

### Comparing `diwork-1.3.0/diwork/diwork_mains/diwork_repeats.py` & `diwork-1.4.0/diwork/diwork_mains/diwork_repeats.py`

 * *Files identical despite different names*

### Comparing `diwork-1.3.0/diwork/diwork_mains/diwork_sshclone.py` & `diwork-1.4.0/diwork/diwork_mains/diwork_sshclone.py`

 * *Files identical despite different names*

### Comparing `diwork-1.3.0/diwork/diwork_ways/__init__.py` & `diwork-1.4.0/diwork/diwork_ways/__init__.py`

 * *Files identical despite different names*

### Comparing `diwork-1.3.0/diwork/diwork_ways/diwork_parse.py` & `diwork-1.4.0/diwork/diwork_ways/diwork_parse.py`

 * *Files identical despite different names*

### Comparing `diwork-1.3.0/diwork/diwork_ways/diwork_sup.py` & `diwork-1.4.0/diwork/diwork_ways/diwork_sup.py`

 * *Files identical despite different names*

### Comparing `diwork-1.3.0/diwork/main.py` & `diwork-1.4.0/diwork/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from diwork_mains import *
 
 from . import __version__
 
 VERSION = __version__
 
 def main():
-    MODULES = "{help, hash, clone, diffclone, sshclone, diff, difx, repeats, exec, archive}"
+    MODULES = "{help, hash, clone, diffclone, sshclone, contains, diff, difx, repeats, exec, archive}"
     SyntaxError_str = f"Syntax error. Expected: \"> python folder_work.py {MODULES} ...\""
     argc = len(sys.argv)
     Global.version = VERSION
     if(argc < 2):
         pout(SyntaxError_str)
         exit()
     else:
@@ -29,14 +29,16 @@
             main_diffclone(sys.argv[2:])
         elif(sub_modul_name == "sshclone"):
             main_sshclone(sys.argv[2:])
         elif(sub_modul_name == "diff"):
             main_diff(sys.argv[2:])
         elif(sub_modul_name == "repeats"):
             main_repeats(sys.argv[2:])
+        elif(sub_modul_name == "contains"):
+            main_contains(sys.argv[2:])
         elif(sub_modul_name == "difx"):
             main_difx(sys.argv[2:])
         elif(sub_modul_name == "exec"):
             main_exec(sys.argv[2:])
         elif(sub_modul_name == "archive"):
             main_archive(sys.argv[2:])
         elif(sub_modul_name == "help"):
```

### Comparing `diwork-1.3.0/diwork.egg-info/SOURCES.txt` & `diwork-1.4.0/diwork.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 diwork.egg-info/dependency_links.txt
 diwork.egg-info/entry_points.txt
 diwork.egg-info/requires.txt
 diwork.egg-info/top_level.txt
 diwork/diwork_mains/__init__.py
 diwork/diwork_mains/diwork_archive.py
 diwork/diwork_mains/diwork_clone.py
+diwork/diwork_mains/diwork_contains.py
 diwork/diwork_mains/diwork_diff.py
 diwork/diwork_mains/diwork_diffclone.py
 diwork/diwork_mains/diwork_difx.py
 diwork/diwork_mains/diwork_exec.py
 diwork/diwork_mains/diwork_hash.py
 diwork/diwork_mains/diwork_help.py
 diwork/diwork_mains/diwork_repeats.py
```

### Comparing `diwork-1.3.0/setup.py` & `diwork-1.4.0/setup.py`

 * *Files identical despite different names*

