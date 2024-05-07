# Comparing `tmp/medicafe-0.240506.1.tar.gz` & `tmp/medicafe-0.240506.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240506.1.tar", last modified: Tue May  7 00:54:31 2024, max compression
+gzip compressed data, was "medicafe-0.240506.2.tar", last modified: Tue May  7 02:12:14 2024, max compression
```

## Comparing `medicafe-0.240506.1.tar` & `medicafe-0.240506.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 00:54:31.560000 medicafe-0.240506.1/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240506.1/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240506.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-07 00:54:30.841000 medicafe-0.240506.1/MediBot/
--rwxrwxrwx   0        0        0     2712 2024-05-02 00:07:18.000000 medicafe-0.240506.1/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    16281 2024-05-02 09:57:36.000000 medicafe-0.240506.1/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240506.1/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    31244 2024-05-06 23:17:52.000000 medicafe-0.240506.1/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240506.1/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0     9619 2024-05-01 03:56:22.000000 medicafe-0.240506.1/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     6314 2024-04-20 04:29:42.000000 medicafe-0.240506.1/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240506.1/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240506.1/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240506.1/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240506.1/MediBot/update_json.py
--rw-rw-rw-   0        0        0      967 2024-05-03 17:14:28.000000 medicafe-0.240506.1/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:54:31.350000 medicafe-0.240506.1/MediLink/
--rw-rw-rw-   0        0        0    17958 2024-05-07 00:47:53.000000 medicafe-0.240506.1/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240506.1/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    19881 2024-04-30 22:21:02.000000 medicafe-0.240506.1/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    33095 2024-05-02 15:19:01.000000 medicafe-0.240506.1/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3791 2024-05-01 23:56:13.000000 medicafe-0.240506.1/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    10989 2024-05-06 23:09:35.000000 medicafe-0.240506.1/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7131 2024-05-02 10:20:35.000000 medicafe-0.240506.1/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240506.1/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6297 2024-05-06 22:21:25.000000 medicafe-0.240506.1/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240506.1/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240506.1/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     4950 2024-04-30 21:38:34.000000 medicafe-0.240506.1/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0     5909 2024-05-02 10:20:36.000000 medicafe-0.240506.1/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240506.1/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240506.1/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240506.1/MediLink/__init__.py
--rw-rw-rw-   0        0        0      730 2024-05-07 00:54:31.544000 medicafe-0.240506.1/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240506.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 00:54:31.526000 medicafe-0.240506.1/medicafe.egg-info/
--rw-rw-rw-   0        0        0      730 2024-05-07 00:54:30.000000 medicafe-0.240506.1/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-05-07 00:54:30.000000 medicafe-0.240506.1/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 00:54:30.000000 medicafe-0.240506.1/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240506.1/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-07 00:54:30.000000 medicafe-0.240506.1/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-07 00:54:30.000000 medicafe-0.240506.1/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 00:54:31.556000 medicafe-0.240506.1/setup.cfg
--rw-rw-rw-   0        0        0     1164 2024-05-07 00:54:26.000000 medicafe-0.240506.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 02:12:14.492000 medicafe-0.240506.2/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240506.2/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240506.2/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-07 02:12:13.926000 medicafe-0.240506.2/MediBot/
+-rwxrwxrwx   0        0        0     2712 2024-05-02 00:07:18.000000 medicafe-0.240506.2/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    16281 2024-05-02 09:57:36.000000 medicafe-0.240506.2/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240506.2/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    31630 2024-05-07 02:05:06.000000 medicafe-0.240506.2/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240506.2/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0     9619 2024-05-01 03:56:22.000000 medicafe-0.240506.2/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     6314 2024-04-20 04:29:42.000000 medicafe-0.240506.2/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240506.2/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240506.2/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240506.2/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240506.2/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     1055 2024-05-07 01:05:17.000000 medicafe-0.240506.2/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-07 02:12:14.324000 medicafe-0.240506.2/MediLink/
+-rw-rw-rw-   0        0        0    17958 2024-05-07 00:47:53.000000 medicafe-0.240506.2/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240506.2/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    19881 2024-04-30 22:21:02.000000 medicafe-0.240506.2/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    35032 2024-05-07 02:09:20.000000 medicafe-0.240506.2/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3791 2024-05-01 23:56:13.000000 medicafe-0.240506.2/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    10989 2024-05-06 23:09:35.000000 medicafe-0.240506.2/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7131 2024-05-02 10:20:35.000000 medicafe-0.240506.2/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240506.2/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     6297 2024-05-06 22:21:25.000000 medicafe-0.240506.2/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240506.2/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240506.2/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     4950 2024-04-30 21:38:34.000000 medicafe-0.240506.2/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0     5909 2024-05-02 10:20:36.000000 medicafe-0.240506.2/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240506.2/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240506.2/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240506.2/MediLink/__init__.py
+-rw-rw-rw-   0        0        0      730 2024-05-07 02:12:14.478000 medicafe-0.240506.2/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240506.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 02:12:14.464000 medicafe-0.240506.2/medicafe.egg-info/
+-rw-rw-rw-   0        0        0      730 2024-05-07 02:12:13.000000 medicafe-0.240506.2/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2024-05-07 02:12:13.000000 medicafe-0.240506.2/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 02:12:13.000000 medicafe-0.240506.2/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240506.2/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-07 02:12:13.000000 medicafe-0.240506.2/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-07 02:12:13.000000 medicafe-0.240506.2/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 02:12:14.490000 medicafe-0.240506.2/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2024-05-07 02:12:12.000000 medicafe-0.240506.2/setup.py
```

### Comparing `medicafe-0.240506.1/LICENSE` & `medicafe-0.240506.2/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240506.1/MediBot/MediBot.bat` & `medicafe-0.240506.2/MediBot/MediBot.bat`

 * *Files identical despite different names*

### Comparing `medicafe-0.240506.1/MediBot/MediBot.py` & `medicafe-0.240506.2/MediBot/MediBot.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240506.1/MediBot/MediBot_Charges.py` & `medicafe-0.240506.2/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240506.1/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240506.2/MediBot/MediBot_Preprocessor.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,30 @@
 import re
 from datetime import datetime
 from collections import OrderedDict # so that the field_mapping stays in order.
 from collections import defaultdict
 import re
 import sys
 import argparse
-from MediBot_Preprocessor_lib import save_crosswalk, open_csv_for_editing, load_csv_data
 
 # Add parent directory of the project to the Python path
 project_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
 sys.path.append(project_dir)
 
-from MediLink import MediLink_ConfigLoader
-from MediLink import MediLink_DataMgmt
+try: 
+    from MediLink import MediLink_ConfigLoader
+    from MediLink import MediLink_DataMgmt
+except ImportError:
+    import MediLink_ConfigLoader
+    import MediLink_DataMgmt
+
+try:
+    import MediBot_Preprocessor_lib
+except ImportError:
+    from MediBot import MediBot_Preprocessor_lib
 
 """
 Preprocessing Enhancements
 - [X] Preprocess Insurance Policy Numbers and Group Numbers to replace '-' with ''.
 - [X] De-duplicate entries in the CSV and only entering the px once even if they show up twice in the file.
 - [ ] Implement dynamic field combination in CSV pre-processing for flexibility with various CSV formats.
 - [ ] Enhance SSN cleaning logic to handle more variations of sensitive data masking.
@@ -104,15 +112,18 @@
 
     Args:
         config (dict): Configuration object containing necessary paths and parameters.
 
     Returns:
         dict: A dictionary mapping insurance names to insurance IDs.
     """
-    # Retrieve MAINS path and slicing information from the configuration
+    # Reset config pull to make sure its not using the MediLink config key subset
+    config, crosswalk = MediLink_ConfigLoader.load_configuration()
+    
+    # Retrieve MAINS path and slicing information from the configuration   
     mains_path = config['MAINS_MED_PATH']
     mains_slices = crosswalk['mains_mapping']['slices']
     
     # Initialize the dictionary to hold the insurance to insurance ID mappings
     insurance_to_id = {}
     
     # Read data from MAINS using a provided function to handle fixed-width data
@@ -283,15 +294,15 @@
                 "medisoft_id": list(medisoft_ids)
             }
     
     # Update the crosswalk for payer IDs only, retaining other mappings
     crosswalk['payer_id'] = payer_id_to_details
     
     # Save the initial crosswalk
-    save_crosswalk(config['MediLink_Config']['crosswalkPath'], crosswalk)
+    MediBot_Preprocessor_lib.save_crosswalk(config['MediLink_Config']['crosswalkPath'], crosswalk)
 
     MediLink_ConfigLoader.log("Crosswalk initialized with mappings for {} payers.".format(len(crosswalk.get('payer_id', {}))))
     
     # Return isn't really necessary since its just a one-off run from args.
     return payer_id_to_details
 
 def crosswalk_update(config, crosswalk):
@@ -384,15 +395,15 @@
     # Convert sets to lists just before saving
     for payer_id in crosswalk['payer_id']:
         if isinstance(crosswalk['payer_id'][payer_id]['medisoft_id'], set):
             crosswalk['payer_id'][payer_id]['medisoft_id'] = list(crosswalk['payer_id'][payer_id]['medisoft_id'])
 
     # Save the updated crosswalk to the specified file
     crosswalk_path = config['MediLink_Config'].get('crosswalkPath')
-    if not save_crosswalk(crosswalk_path, crosswalk):
+    if not MediBot_Preprocessor_lib.save_crosswalk(crosswalk_path, crosswalk):
         return False
 
     return True
 
 # CSV Preprocessor built for Carol
 def preprocess_csv_data(csv_data, crosswalk):
     try:
@@ -572,23 +583,23 @@
         crosswalk_update(config, crosswalk)
 
     if args.init_crosswalk:
         initialize_crosswalk_from_mapat(config, crosswalk)
 
     if args.load_csv:
         print("Loading CSV data...")
-        csv_data = load_csv_data(config['CSV_FILE_PATH'])
+        csv_data = MediBot_Preprocessor_lib.load_csv_data(config['CSV_FILE_PATH'])
         print("Loaded {} records from the CSV.".format(len(csv_data)))
 
     if args.preprocess_csv:
         if 'csv_data' in locals():
             print("Preprocessing CSV data...")
             preprocess_csv_data(csv_data, crosswalk)
         else:
             print("Error: CSV data needs to be loaded before preprocessing. Use --load-csv.")
     
     if args.open_csv:
         print("Opening CSV for editing...")
-        open_csv_for_editing(config['CSV_FILE_PATH'])
+        MediBot_Preprocessor_lib.open_csv_for_editing(config['CSV_FILE_PATH'])
 
 if __name__ == '__main__':
     main()
```

### Comparing `medicafe-0.240506.1/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240506.2/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240506.1/MediBot/MediBot_UI.py` & `medicafe-0.240506.2/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240506.1/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240506.2/MediBot/MediBot_dataformat_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240506.1/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240506.2/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240506.1/MediBot/update_json.py` & `medicafe-0.240506.2/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240506.1/MediBot/update_medicafe.py` & `medicafe-0.240506.2/MediBot/update_medicafe.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 import subprocess
 import sys
 from tqdm import tqdm
 
 def upgrade_medicafe(package):
     try:
-        # Use tqdm to create a progress bar
         with tqdm(total=100, desc="Upgrading %s" % package, unit="%") as progress_bar:
-            # Upgrade the package using pip with --no-cache-dir option
-            subprocess.check_call([sys.executable, '-m', 'pip', 'install', '--upgrade', package, '--no-cache-dir', '--no-deps', '--disable-pip-version-check'], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
-            # Update progress bar to 100% upon completion
+            # Capture both stdout and stderr
+            result = subprocess.run([sys.executable, '-m', 'pip', 'install', '--upgrade', package, '--no-cache-dir', '--disable-pip-version-check', '--no-deps'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+            
+            if result.returncode != 0:
+                # If the return code is non-zero, print error details
+                print("Error: Upgrade failed. Details:")
+                print("stdout:", result.stdout)
+                print("stderr:", result.stderr)
+                sys.exit(1)
+                
             progress_bar.update(100 - progress_bar.n)
-    except subprocess.CalledProcessError as e:
-        # Log the error details
-        print("Error: Upgrade failed. Details:", e)
-        print("Please check your internet connection and try again later.")
+    except Exception as e:
+        # Log any other exceptions
+        print("Error:", e)
         sys.exit(1)
 
 if __name__ == "__main__":
     medicafe_package = "medicafe"
-    upgrade_medicafe(medicafe_package)
+    upgrade_medicafe(medicafe_package)
```

### Comparing `medicafe-0.240506.1/MediLink/MediLink.py` & `medicafe-0.240506.2/MediLink/MediLink.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240506.1/MediLink/MediLink_277_decoder.py` & `medicafe-0.240506.2/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240506.1/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240506.2/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240506.1/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240506.2/MediLink/MediLink_837p_encoder_library.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 from datetime import datetime
 import json
 import requests
 import time
 import sys
 from MediLink import MediLink_ConfigLoader
 
+# Add parent directory of the project to the Python path
+import sys
+import os
+project_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
+sys.path.append(project_dir)
+
+from MediBot import MediBot_Preprocessor
+
 """
 1. Code Refactoring: Increase modularity and clarity, particularly in segment creation functions (e.g., `create_st_segment`, `create_nm1_billing_provider_segment`), for better maintenance and readability.
 2. Endpoint Support: Extend support within segment creation for additional endpoints with attention to their unique claim submission requirements.
 3. Payer Identification Mechanism: Refine the mechanism for dynamically identifying payers, leveraging payer mappings and integrating with external APIs like Availity for precise payer information retrieval.
 4. Adherence to Endpoint-Specific Standards: Implement and verify the compliance of claim data formatting and inclusion based on the specific demands of each target endpoint within the segment creation logic.
 5. De-persisting Intermediate Files.
 6. Get an API for Optum "Entered As". 
@@ -167,37 +175,63 @@
     """
     Maps the insurance name provided by Medisoft to the corresponding payer ID by referencing
     a crosswalk mapping stored in the "crosswalk" JSON file. This file must be located at a path
     specified in the config under the key 'crosswalk_path'.
 
     Inputs:
     - insurance_name: The name of the insurance as provided by Medisoft.
+    - config: A dictionary containing configuration parameters, including the path to the crosswalk JSON file.
 
     Outputs:
     - payer_id: The unique identifier (ID) corresponding to the insurance name, if the mapping
       is successful. It will be a 5-character alphanumeric code.
 
     Functionality:
-    - This function retrieves the mapping from a "crosswalk" JSON file.
+    - This function retrieves the mapping from a "crosswalk" JSON file using the provided configuration.
+    - It first uses the MAINS data to map the insurance name to its corresponding Medisoft ID.
+    - Then, it looks up the payer ID associated with the Medisoft ID in the crosswalk.
     - If the mapping is successful, it returns the payer ID.
     - If the mapping fails or the payer ID cannot be retrieved, it raises an error indicating
       the inability to extract the payer ID.
     """
+
     _, crosswalk = MediLink_ConfigLoader.load_configuration(None, config.get('crosswalkPath', 'crosswalk.json'))
     
     try:
-        payer_id = crosswalk['medisoft_insurance_to_payer_id'].get(insurance_name)
-        if not payer_id:
-            raise ValueError("No payer ID found for insurance name: {}".format(insurance_name))
-        return payer_id
-    except json.JSONDecodeError:
-        raise ValueError("Error decoding the crosswalk JSON file")
+        # Load insurance data from MAINS to get insurance ID
+        insurance_to_id = MediBot_Preprocessor.load_insurance_data_from_mains(config)
+        
+        # Get medisoft ID corresponding to the insurance name
+        medisoft_id = insurance_to_id.get(insurance_name)
+        if medisoft_id is None:
+            raise ValueError("No Medisoft ID found for insurance name: {}".format(insurance_name))
+        
+        # Get payer ID corresponding to the medisoft ID
+        for payer, payer_info in crosswalk['payer_id'].items():
+            if medisoft_id in payer_info['medisoft_id']:
+                return payer
+        
+        raise ValueError("No payer ID found for Medisoft ID: {}".format(medisoft_id))
+        # TODO OK so then what? This is when the crosswalk has insufficient information.
+        # This means there is a new insurance from the Z data that we haven't seen before?
+        # update_crosswalk would have had to catch this earlier in the flow.
+        
+    except ValueError as e:
+        if "JSON" in str(e) and "decode" in str(e):
+            raise ValueError("Error decoding the crosswalk JSON file")
+        else:
+            raise e
 
 def fetch_payer_name_from_crosswalk(payer_id, config, endpoint):
     """
+    BUG TODO This is the backup function for when Availity cant resolve the payer name.
+    The best thing to do here would probably be to pull from Carol's CSV but maybe we 
+    can start with trying to pull from MAINS and just use that as the default for now.
+    For now, this is not make-work because Availity can resolve what we want right now.
+    
     Retrieves the payer name corresponding to a given payer ID from a crosswalk mapping.
     
     Parameters:
     - payer_id: The unique identifier for the payer whose name is to be resolved.
     - config: Configuration dictionary including the path to the crosswalk JSON.
     
     Returns:
@@ -209,17 +243,18 @@
     # Ensure the 'crosswalkPath' key exists in config and contains the path to the crosswalk JSON file
     if 'crosswalkPath' not in config:
         raise ValueError("Crosswalk path not defined in configuration.")
 
     crosswalk_path = config.get('crosswalkPath')
     try:
         with open(crosswalk_path, 'r') as file:
-            crosswalk_mappings = json.load(file)
+            crosswalk_mappings = json.load(file) # BUG This should be using ConfigLoader.
         # Select the endpoint-specific section from the mappings
-        endpoint_mappings = crosswalk_mappings['payer_id_to_name'].get(endpoint, {})
+        # BUG This whole thing needs to be re-worked.
+        endpoint_mappings = crosswalk_mappings['payer_id'].get(endpoint, {})
         payer_name = endpoint_mappings.get(payer_id)
 
         if not payer_name:
             raise ValueError("Payer name not found for payer ID: {} in {} mappings.".format(payer_id, endpoint))
 
         return payer_name
     except FileNotFoundError:
@@ -259,15 +294,15 @@
 
     payer_name = ''
     # Step 2: Attempt to Retrieve Payer Name from Availity API (current API integration)
     endpoint = 'availity' # Force availity API because none of the other ones are connected BUG
     if True: #endpoint.lower() == 'availity':
         try:
             payer_name = fetch_payer_name_from_api(payer_id, config, endpoint)
-            log("Resolved payer name {} via {} API for Payer ID: {}".format(payer_name, endpoint, payer_id), config, level="INFO")
+            MediLink_ConfigLoader.log("Resolved payer name {} via {} API for Payer ID: {}".format(payer_name, endpoint, payer_id), config, level="INFO")
         except Exception as api_error:
             print("{} API call failed for Payer ID '{}': {}".format(endpoint, payer_id, api_error))
 
     # Placeholder for future API integrations with other endpoints
     # elif endpoint.lower() == 'optum':
     #     payer_name = fetch_payer_name_from_optum_api(payer_id, config)
     # elif endpoint.lower() == 'pnt_data':
@@ -643,15 +678,15 @@
     # GS06 Group Control Number, Field Length 1/9, must match GE02
     gs06 = '1' # Placeholder for now?
     
     gs_segment = "GS*HC*{}*{}*{}*{}*{}*X*005010X222A1~".format(
         gs_sender_code, gs_receiver_code, format_datetime(), format_datetime(format_type='time'), gs06
     )
 
-    log("Created interchange header for endpoint: {}".format(endpoint), config, level="INFO")
+    MediLink_ConfigLoader.log("Created interchange header for endpoint: {}".format(endpoint), config, level="INFO")
     
     return isa_segment, gs_segment
 
 # Generates the GE and IEA segments for the interchange trailer based on the number of transactions and functional groups.
 def create_interchange_trailer(config, endpoint, num_transactions, num_functional_groups=1):
     """
     Generate GE and IEA segments for the interchange trailer.
@@ -673,15 +708,15 @@
     # IEA Segment: Interchange Control Trailer
     isa13 = '000000001' # Default Interchange Control Number. Not sure what to do with this. date? See also trailer
     isa13_value = endpoint_config.get('isa_13_value', isa13) # Needs to match IEA02, can this be a date/time?
     # Indicates the end of an interchange and provides the count of the number of functional groups within it.
     # The Interchange Control Number needs to match isa13 and iea02
     iea_segment = "IEA*{}*{}~".format(num_functional_groups, isa13_value)
     
-    log("Created interchange trailer", config, level="INFO")
+    MediLink_ConfigLoader.log("Created interchange trailer", config, level="INFO")
     
     return ge_segment, iea_segment
 
 # Generates segment counts for the formatted 837P transaction and updates SE segment.
 def generate_segment_counts(compiled_segments, transaction_set_control_number):
     # Count the number of segments, not including the placeholder SE segment
     segment_count = compiled_segments.count('~')   # + 1 Including SE segment itself, but seems to be giving errors.
```

### Comparing `medicafe-0.240506.1/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240506.2/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240506.1/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240506.2/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240506.1/MediLink/MediLink_Down.py` & `medicafe-0.240506.2/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240506.1/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240506.2/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240506.1/MediLink/MediLink_Gmail.py` & `medicafe-0.240506.2/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240506.1/MediLink/MediLink_Scheduler.py` & `medicafe-0.240506.2/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240506.1/MediLink/MediLink_UI.py` & `medicafe-0.240506.2/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240506.1/MediLink/MediLink_Up.py` & `medicafe-0.240506.2/MediLink/MediLink_Up.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240506.1/PKG-INFO` & `medicafe-0.240506.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240506.1
+Version: 0.240506.2
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240506.1/README.md` & `medicafe-0.240506.2/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240506.1/medicafe.egg-info/PKG-INFO` & `medicafe-0.240506.2/medicafe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240506.1
+Version: 0.240506.2
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240506.1/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240506.2/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240506.1/setup.py` & `medicafe-0.240506.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240506.1",
+    version="0.240506.2",
     description='MediCafe',
     long_description='This module ensures that MediCafe remains up-to-date by performing version checks for its dependencies on startup. It utilizes PyPI, the official repository for Python packages, to retrieve information about the latest available versions of the required packages. When an internet connection is available, MediUpdate automatically installs any available updates using pip, the package installer for Python.',
     long_description_content_type='text/markdown',
     keywords = 'medicafe python34 medibot medilink',
     url='https://github.com/katanada2',
     author='Daniel Vidaud',
     author_email='daniel@personalizedtransformation.com',
```

