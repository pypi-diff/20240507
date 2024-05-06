# Comparing `tmp/grader_helper-0.1.3.tar.gz` & `tmp/grader_helper-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grader_helper-0.1.3.tar", max compression
+gzip compressed data, was "grader_helper-0.1.4.tar", max compression
```

## Comparing `grader_helper-0.1.3.tar` & `grader_helper-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      794 2024-05-06 22:37:50.633298 grader_helper-0.1.3/grader_helper/__init__.py
--rw-r--r--   0        0        0     1607 2024-05-06 19:47:00.017889 grader_helper-0.1.3/grader_helper/distribute_feedback_sheets.py
--rw-r--r--   0        0        0     2592 2024-05-06 19:47:00.030900 grader_helper-0.1.3/grader_helper/distribute_graders_groups.py
--rw-r--r--   0        0        0     1967 2024-05-06 19:46:59.931883 grader_helper-0.1.3/grader_helper/distribute_graders_individual.py
--rw-r--r--   0        0        0     1483 2024-05-06 19:47:00.070903 grader_helper-0.1.3/grader_helper/import_brightspace_classlist.py
--rw-r--r--   0        0        0      644 2024-05-06 20:26:06.293171 grader_helper-0.1.3/grader_helper/load_graders.py
--rw-r--r--   0        0        0     3639 2024-05-06 19:47:00.235415 grader_helper-0.1.3/grader_helper/rename_folders.py
--rw-r--r--   0        0        0     1604 2024-05-06 22:39:35.413885 grader_helper-0.1.3/grader_helper/save_distributed_graders.py
--rw-r--r--   0        0        0     2189 2024-05-06 19:47:00.142422 grader_helper-0.1.3/grader_helper/save_grader_sheets.py
--rw-r--r--   0        0        0      441 2024-05-06 22:41:32.983632 grader_helper-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-06 20:05:58.335712 grader_helper-0.1.3/README.md
--rw-r--r--   0        0        0      479 1970-01-01 00:00:00.000000 grader_helper-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      794 2024-05-06 22:37:50.633298 grader_helper-0.1.4/grader_helper/__init__.py
+-rw-r--r--   0        0        0     1607 2024-05-06 19:47:00.017889 grader_helper-0.1.4/grader_helper/distribute_feedback_sheets.py
+-rw-r--r--   0        0        0     2592 2024-05-06 19:47:00.030900 grader_helper-0.1.4/grader_helper/distribute_graders_groups.py
+-rw-r--r--   0        0        0     1967 2024-05-06 19:46:59.931883 grader_helper-0.1.4/grader_helper/distribute_graders_individual.py
+-rw-r--r--   0        0        0     1483 2024-05-06 19:47:00.070903 grader_helper-0.1.4/grader_helper/import_brightspace_classlist.py
+-rw-r--r--   0        0        0      644 2024-05-06 20:26:06.293171 grader_helper-0.1.4/grader_helper/load_graders.py
+-rw-r--r--   0        0        0     4414 2024-05-06 23:11:08.696784 grader_helper-0.1.4/grader_helper/rename_folders.py
+-rw-r--r--   0        0        0     1604 2024-05-06 22:39:35.413885 grader_helper-0.1.4/grader_helper/save_distributed_graders.py
+-rw-r--r--   0        0        0     2189 2024-05-06 19:47:00.142422 grader_helper-0.1.4/grader_helper/save_grader_sheets.py
+-rw-r--r--   0        0        0      441 2024-05-06 23:12:04.972346 grader_helper-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-06 20:05:58.335712 grader_helper-0.1.4/README.md
+-rw-r--r--   0        0        0      479 1970-01-01 00:00:00.000000 grader_helper-0.1.4/PKG-INFO
```

### Comparing `grader_helper-0.1.3/grader_helper/__init__.py` & `grader_helper-0.1.4/grader_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.3/grader_helper/distribute_feedback_sheets.py` & `grader_helper-0.1.4/grader_helper/distribute_feedback_sheets.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.3/grader_helper/distribute_graders_groups.py` & `grader_helper-0.1.4/grader_helper/distribute_graders_groups.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.3/grader_helper/distribute_graders_individual.py` & `grader_helper-0.1.4/grader_helper/distribute_graders_individual.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.3/grader_helper/import_brightspace_classlist.py` & `grader_helper-0.1.4/grader_helper/import_brightspace_classlist.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.3/grader_helper/load_graders.py` & `grader_helper-0.1.4/grader_helper/load_graders.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.3/grader_helper/rename_folders.py` & `grader_helper-0.1.4/grader_helper/rename_folders.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,92 +1,74 @@
 import pandas as pd
 import pathlib as pl
 
 
-def rename_folders(df: pd.DataFrame, subs_folder: pl.Path) -> None:
+def rename_folders(df, subs_folder):
     """
     Renames folders in subs_folder based on a DataFrame mapping of names to student IDs.
-
+    
     Args:
         df (pd.DataFrame): DataFrame containing columns 'Last Name', 'First Name', and 'Student ID'.
         subs_folder (Path): pathlib.Path object pointing to the directory containing the folders to be renamed.
     """
     # Convert DataFrame to a dictionary for easier lookup
-    name_id_map = {
-        (row["Last Name"].upper(), row["First Name"].upper()): row["Student ID"]
-        for _, row in df.iterrows()
-    }
-
+    name_id_map = {(row['Last Name'].upper(), row['First Name'].upper()): row['Student ID'] for _, row in df.iterrows()}
+    
     def ask_to_rename(folder_name, suggested_name):
         """Prompts user for rename confirmation."""
-        response = (
-            input(f"Rename '{folder_name}' to '{suggested_name}'? (y/n): ")
-            .strip()
-            .lower()
-        )
-        return response == "y"
+        response = input(f"Rename '{folder_name}' to '{suggested_name}'? (y/n): ").strip().lower()
+        return response == 'y'
 
     rename_attempts = []  # Initialize a list to keep track of rename attempts
 
     for folder in subs_folder.iterdir():
-        if not folder.is_dir():
-            continue
-
-        folder_name_upper = folder.name.upper()
-        matched = False
-
-        for (last_name, first_name), student_id in name_id_map.items():
-            if last_name in folder_name_upper and first_name in folder_name_upper:
-                new_folder_name = f"{last_name}, {first_name} ({student_id})"
-                try:
-                    folder.rename(subs_folder / new_folder_name)
-                    print(f"Folder renamed for {new_folder_name}")
-                    outcome = "Renamed"
-                except Exception as e:
-                    print(f"Failed to rename folder for {new_folder_name}: {e}")
-                    outcome = "Failed"
-                rename_attempts.append(
-                    {
-                        "Original Name": folder.name,
-                        "Suggested Name": new_folder_name,
-                        "Outcome": outcome,
-                    }
-                )
-                matched = True
-                break
-
-        if not matched:
+        if folder.is_dir():
+            folder_name_upper = folder.name.upper()
+            matched = False
+            
             for (last_name, first_name), student_id in name_id_map.items():
-                if f" {first_name} " in folder_name_upper:
-                    new_folder_name = f"{last_name}, {first_name} ({student_id})"
-                elif f" {last_name} " in folder_name_upper:
+                if last_name in folder_name_upper and first_name in folder_name_upper:
                     new_folder_name = f"{last_name}, {first_name} ({student_id})"
-                else:
-                    continue
-
-                if ask_to_rename(folder.name, new_folder_name):
                     try:
                         folder.rename(subs_folder / new_folder_name)
-                        outcome = "User Confirmed"
+                        print(f"Folder renamed for {new_folder_name}")
+                        rename_attempts.append({'Original Name': folder.name, 'Suggested Name': new_folder_name, 'Outcome': 'Renamed'})
+                        matched = True
+                        break
                     except Exception as e:
                         print(f"Failed to rename folder for {new_folder_name}: {e}")
-                        outcome = "Failed After User Confirmation"
-                else:
-                    outcome = "User Rejected"
-                rename_attempts.append(
-                    {
-                        "Original Name": folder.name,
-                        "Suggested Name": new_folder_name,
-                        "Outcome": outcome,
-                    }
-                )
-                matched = True
-                break
-
-        if not matched:
-            rename_attempts.append(
-                {
-                    "Original Name": folder.name,
-                    "Suggested Name": "N/A",
-                    "Outcome": "No Match Found",
-                }
-            )
+                        rename_attempts.append({'Original Name': folder.name, 'Suggested Name': new_folder_name, 'Outcome': 'Failed'})
+                        matched = True
+                        break
+
+            if not matched:
+                for (last_name, first_name), student_id in name_id_map.items():
+                    if f" {first_name} " in folder_name_upper and not matched:
+                        new_folder_name = f"{last_name}, {first_name} ({student_id})"
+                        if ask_to_rename(folder.name, new_folder_name):
+                            try:
+                                folder.rename(subs_folder / new_folder_name)
+                                rename_attempts.append({'Original Name': folder.name, 'Suggested Name': new_folder_name, 'Outcome': 'User Confirmed'})
+                                matched = True
+                                break
+                            except Exception as e:
+                                print(f"Failed to rename folder for {new_folder_name}: {e}")
+                                rename_attempts.append({'Original Name': folder.name, 'Suggested Name': new_folder_name, 'Outcome': 'Failed After User Confirmation'})
+                                matched = True
+                                break
+
+                    elif f" {last_name} " in folder_name_upper and not matched:
+                        new_folder_name = f"{last_name}, {first_name} ({student_id})"
+                        if ask_to_rename(folder.name, new_folder_name):
+                            try:
+                                folder.rename(subs_folder / new_folder_name)
+                                rename_attempts.append({'Original Name': folder.name, 'Suggested Name': new_folder_name, 'Outcome': 'User Confirmed'})
+                                matched = True
+                            except Exception as e:
+                                print(f"Failed to rename folder for {new_folder_name}: {e}")
+                                rename_attempts.append({'Original Name': folder.name, 'Suggested Name': new_folder_name, 'Outcome': 'Failed After User Confirmation'})
+                        else:
+                            rename_attempts.append({'Original Name': folder.name, 'Suggested Name': new_folder_name, 'Outcome': 'User Rejected'})
+                            matched = True
+
+            if not matched:
+                rename_attempts.append({'Original Name': folder.name, 'Suggested Name': 'N/A', 'Outcome': 'No Match Found'})
```

### Comparing `grader_helper-0.1.3/grader_helper/save_distributed_graders.py` & `grader_helper-0.1.4/grader_helper/save_distributed_graders.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.3/grader_helper/save_grader_sheets.py` & `grader_helper-0.1.4/grader_helper/save_grader_sheets.py`

 * *Files identical despite different names*

