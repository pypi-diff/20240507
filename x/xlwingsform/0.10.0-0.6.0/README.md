# Comparing `tmp/xlwingsform-0.10.0.tar.gz` & `tmp/xlwingsform-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlwingsform-0.10.0.tar", last modified: Wed Apr 24 05:14:46 2024, max compression
+gzip compressed data, was "xlwingsform-0.6.0.tar", last modified: Tue May  7 06:41:07 2024, max compression
```

## Comparing `xlwingsform-0.10.0.tar` & `xlwingsform-0.6.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 a.kano     (501) staff       (20)        0 2024-04-24 05:14:46.818981 xlwingsform-0.10.0/
--rw-r--r--   0 a.kano     (501) staff       (20)       56 2024-04-24 05:14:46.818721 xlwingsform-0.10.0/PKG-INFO
--rw-r--r--   0 a.kano     (501) staff       (20)       38 2024-04-24 05:14:46.819020 xlwingsform-0.10.0/setup.cfg
--rw-r--r--   0 a.kano     (501) staff       (20)      129 2024-04-24 05:14:37.000000 xlwingsform-0.10.0/setup.py
-drwxr-xr-x   0 a.kano     (501) staff       (20)        0 2024-04-24 05:14:46.817820 xlwingsform-0.10.0/xlwingsform/
--rw-r--r--   0 a.kano     (501) staff       (20)       37 2024-04-24 02:55:55.000000 xlwingsform-0.10.0/xlwingsform/__init__.py
--rw-r--r--   0 a.kano     (501) staff       (20)      996 2024-04-24 02:58:53.000000 xlwingsform-0.10.0/xlwingsform/xlwingsform.py
-drwxr-xr-x   0 a.kano     (501) staff       (20)        0 2024-04-24 05:14:46.818540 xlwingsform-0.10.0/xlwingsform.egg-info/
--rw-r--r--   0 a.kano     (501) staff       (20)       56 2024-04-24 05:14:46.000000 xlwingsform-0.10.0/xlwingsform.egg-info/PKG-INFO
--rw-r--r--   0 a.kano     (501) staff       (20)      199 2024-04-24 05:14:46.000000 xlwingsform-0.10.0/xlwingsform.egg-info/SOURCES.txt
--rw-r--r--   0 a.kano     (501) staff       (20)        1 2024-04-24 05:14:46.000000 xlwingsform-0.10.0/xlwingsform.egg-info/dependency_links.txt
--rw-r--r--   0 a.kano     (501) staff       (20)       12 2024-04-24 05:14:46.000000 xlwingsform-0.10.0/xlwingsform.egg-info/top_level.txt
+drwxr-xr-x   0 a.kano     (501) staff       (20)        0 2024-05-07 06:41:07.681928 xlwingsform-0.6.0/
+-rw-r--r--   0 a.kano     (501) staff       (20)       55 2024-05-07 06:41:07.681665 xlwingsform-0.6.0/PKG-INFO
+-rw-r--r--   0 a.kano     (501) staff       (20)        0 2024-05-07 06:37:47.000000 xlwingsform-0.6.0/README.md
+-rw-r--r--   0 a.kano     (501) staff       (20)       38 2024-05-07 06:41:07.681966 xlwingsform-0.6.0/setup.cfg
+-rw-r--r--   0 a.kano     (501) staff       (20)      128 2024-05-07 06:37:47.000000 xlwingsform-0.6.0/setup.py
+drwxr-xr-x   0 a.kano     (501) staff       (20)        0 2024-05-07 06:41:07.680787 xlwingsform-0.6.0/xlwingsform/
+-rw-r--r--   0 a.kano     (501) staff       (20)       37 2024-05-07 06:37:47.000000 xlwingsform-0.6.0/xlwingsform/__init__.py
+-rw-r--r--   0 a.kano     (501) staff       (20)      962 2024-05-07 06:38:04.000000 xlwingsform-0.6.0/xlwingsform/xlwingsform.py
+drwxr-xr-x   0 a.kano     (501) staff       (20)        0 2024-05-07 06:41:07.681489 xlwingsform-0.6.0/xlwingsform.egg-info/
+-rw-r--r--   0 a.kano     (501) staff       (20)       55 2024-05-07 06:41:07.000000 xlwingsform-0.6.0/xlwingsform.egg-info/PKG-INFO
+-rw-r--r--   0 a.kano     (501) staff       (20)      209 2024-05-07 06:41:07.000000 xlwingsform-0.6.0/xlwingsform.egg-info/SOURCES.txt
+-rw-r--r--   0 a.kano     (501) staff       (20)        1 2024-05-07 06:41:07.000000 xlwingsform-0.6.0/xlwingsform.egg-info/dependency_links.txt
+-rw-r--r--   0 a.kano     (501) staff       (20)       12 2024-05-07 06:41:07.000000 xlwingsform-0.6.0/xlwingsform.egg-info/top_level.txt
```

### Comparing `xlwingsform-0.10.0/xlwingsform/xlwingsform.py` & `xlwingsform-0.6.0/xlwingsform/xlwingsform.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     def __init__(self, ws) -> None:
         self.ws = ws
 
     def get_values(self, range_name):
         return self.ws.range(range_name).value
 
     def set_values(self, range_name, values):
-        print(range_name, values)
         self.ws.range(range_name).value = values
 
 
 class Workbook:
     def __init__(self, path, dst_sheets, template_sheet_name) -> None:
         self.template_sheet_name = template_sheet_name
         self.dst_sheets = dst_sheets
```

