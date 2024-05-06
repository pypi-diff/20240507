# Comparing `tmp/grader_helper-0.1.1.tar.gz` & `tmp/grader_helper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grader_helper-0.1.1.tar", max compression
+gzip compressed data, was "grader_helper-0.1.3.tar", max compression
```

## Comparing `grader_helper-0.1.1.tar` & `grader_helper-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2024-05-06 20:01:12.196652 grader_helper-0.1.1/grader_helper/__init__.py
--rw-r--r--   0        0        0     1607 2024-05-06 19:47:00.017889 grader_helper-0.1.1/grader_helper/distribute_feedback_sheets.py
--rw-r--r--   0        0        0     2592 2024-05-06 19:47:00.030900 grader_helper-0.1.1/grader_helper/distribute_graders_groups.py
--rw-r--r--   0        0        0     1967 2024-05-06 19:46:59.931883 grader_helper-0.1.1/grader_helper/distribute_graders_individual.py
--rw-r--r--   0        0        0     1483 2024-05-06 19:47:00.070903 grader_helper-0.1.1/grader_helper/import_brightspace_classlist.py
--rw-r--r--   0        0        0      644 2024-05-06 20:26:06.293171 grader_helper-0.1.1/grader_helper/load_graders.py
--rw-r--r--   0        0        0     3639 2024-05-06 19:47:00.235415 grader_helper-0.1.1/grader_helper/rename_folders.py
--rw-r--r--   0        0        0     1603 2024-05-06 19:47:00.297419 grader_helper-0.1.1/grader_helper/save_distributed_graders.py
--rw-r--r--   0        0        0     2189 2024-05-06 19:47:00.142422 grader_helper-0.1.1/grader_helper/save_grader_sheets.py
--rw-r--r--   0        0        0      441 2024-05-06 20:27:45.346834 grader_helper-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-06 20:05:58.335712 grader_helper-0.1.1/README.md
--rw-r--r--   0        0        0      479 1970-01-01 00:00:00.000000 grader_helper-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      794 2024-05-06 22:37:50.633298 grader_helper-0.1.3/grader_helper/__init__.py
+-rw-r--r--   0        0        0     1607 2024-05-06 19:47:00.017889 grader_helper-0.1.3/grader_helper/distribute_feedback_sheets.py
+-rw-r--r--   0        0        0     2592 2024-05-06 19:47:00.030900 grader_helper-0.1.3/grader_helper/distribute_graders_groups.py
+-rw-r--r--   0        0        0     1967 2024-05-06 19:46:59.931883 grader_helper-0.1.3/grader_helper/distribute_graders_individual.py
+-rw-r--r--   0        0        0     1483 2024-05-06 19:47:00.070903 grader_helper-0.1.3/grader_helper/import_brightspace_classlist.py
+-rw-r--r--   0        0        0      644 2024-05-06 20:26:06.293171 grader_helper-0.1.3/grader_helper/load_graders.py
+-rw-r--r--   0        0        0     3639 2024-05-06 19:47:00.235415 grader_helper-0.1.3/grader_helper/rename_folders.py
+-rw-r--r--   0        0        0     1604 2024-05-06 22:39:35.413885 grader_helper-0.1.3/grader_helper/save_distributed_graders.py
+-rw-r--r--   0        0        0     2189 2024-05-06 19:47:00.142422 grader_helper-0.1.3/grader_helper/save_grader_sheets.py
+-rw-r--r--   0        0        0      441 2024-05-06 22:41:32.983632 grader_helper-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-06 20:05:58.335712 grader_helper-0.1.3/README.md
+-rw-r--r--   0        0        0      479 1970-01-01 00:00:00.000000 grader_helper-0.1.3/PKG-INFO
```

### Comparing `grader_helper-0.1.1/grader_helper/distribute_feedback_sheets.py` & `grader_helper-0.1.3/grader_helper/distribute_feedback_sheets.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.1/grader_helper/distribute_graders_groups.py` & `grader_helper-0.1.3/grader_helper/distribute_graders_groups.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.1/grader_helper/distribute_graders_individual.py` & `grader_helper-0.1.3/grader_helper/distribute_graders_individual.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.1/grader_helper/import_brightspace_classlist.py` & `grader_helper-0.1.3/grader_helper/import_brightspace_classlist.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.1/grader_helper/load_graders.py` & `grader_helper-0.1.3/grader_helper/load_graders.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.1/grader_helper/rename_folders.py` & `grader_helper-0.1.3/grader_helper/rename_folders.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.1/grader_helper/save_distributed_graders.py` & `grader_helper-0.1.3/grader_helper/save_distributed_graders.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas as pd
 import pathlib as pl
-from distribute_graders_individual import distribute_graders_individual
+from .distribute_graders_individual import distribute_graders_individual
 
 
 def main():
     # Example usage
     # Create a DataFrame with student information
     data = {
         "student_id": [1, 2, 3, 4, 5],
```

### Comparing `grader_helper-0.1.1/grader_helper/save_grader_sheets.py` & `grader_helper-0.1.3/grader_helper/save_grader_sheets.py`

 * *Files identical despite different names*

