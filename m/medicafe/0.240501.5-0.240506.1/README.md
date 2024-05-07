# Comparing `tmp/medicafe-0.240501.5.tar.gz` & `tmp/medicafe-0.240506.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240501.5.tar", last modified: Thu May  2 03:08:46 2024, max compression
+gzip compressed data, was "medicafe-0.240506.1.tar", last modified: Tue May  7 00:54:31 2024, max compression
```

## Comparing `medicafe-0.240501.5.tar` & `medicafe-0.240506.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 03:08:46.617000 medicafe-0.240501.5/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240501.5/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240501.5/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-02 03:08:45.376000 medicafe-0.240501.5/MediBot/
--rwxrwxrwx   0        0        0     2712 2024-05-02 00:07:18.000000 medicafe-0.240501.5/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    16168 2024-05-01 03:57:12.000000 medicafe-0.240501.5/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240501.5/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    29101 2024-05-02 03:05:50.000000 medicafe-0.240501.5/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240501.5/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0     9619 2024-05-01 03:56:22.000000 medicafe-0.240501.5/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     6314 2024-04-20 04:29:42.000000 medicafe-0.240501.5/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240501.5/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240501.5/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240501.5/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240501.5/MediBot/update_json.py
--rw-rw-rw-   0        0        0      829 2024-05-02 02:20:59.000000 medicafe-0.240501.5/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-02 03:08:46.186000 medicafe-0.240501.5/MediLink/
--rw-rw-rw-   0        0        0    17570 2024-05-02 00:11:11.000000 medicafe-0.240501.5/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240501.5/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    19881 2024-04-30 22:21:02.000000 medicafe-0.240501.5/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    33088 2024-05-01 04:35:27.000000 medicafe-0.240501.5/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3791 2024-05-01 23:56:13.000000 medicafe-0.240501.5/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    10677 2024-05-01 03:49:34.000000 medicafe-0.240501.5/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7123 2024-05-01 03:44:49.000000 medicafe-0.240501.5/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240501.5/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6313 2024-05-01 03:44:48.000000 medicafe-0.240501.5/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240501.5/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240501.5/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     4950 2024-04-30 21:38:34.000000 medicafe-0.240501.5/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0     6051 2024-05-01 03:44:47.000000 medicafe-0.240501.5/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240501.5/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240501.5/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240501.5/MediLink/__init__.py
--rw-rw-rw-   0        0        0      730 2024-05-02 03:08:46.525000 medicafe-0.240501.5/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240501.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 03:08:46.500000 medicafe-0.240501.5/medicafe.egg-info/
--rw-rw-rw-   0        0        0      730 2024-05-02 03:08:44.000000 medicafe-0.240501.5/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-05-02 03:08:44.000000 medicafe-0.240501.5/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 03:08:44.000000 medicafe-0.240501.5/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240501.5/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-02 03:08:44.000000 medicafe-0.240501.5/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-02 03:08:44.000000 medicafe-0.240501.5/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 03:08:46.544000 medicafe-0.240501.5/setup.cfg
--rw-rw-rw-   0        0        0     1164 2024-05-02 03:08:43.000000 medicafe-0.240501.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 00:54:31.560000 medicafe-0.240506.1/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240506.1/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240506.1/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-07 00:54:30.841000 medicafe-0.240506.1/MediBot/
+-rwxrwxrwx   0        0        0     2712 2024-05-02 00:07:18.000000 medicafe-0.240506.1/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    16281 2024-05-02 09:57:36.000000 medicafe-0.240506.1/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240506.1/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    31244 2024-05-06 23:17:52.000000 medicafe-0.240506.1/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240506.1/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0     9619 2024-05-01 03:56:22.000000 medicafe-0.240506.1/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     6314 2024-04-20 04:29:42.000000 medicafe-0.240506.1/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240506.1/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240506.1/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240506.1/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240506.1/MediBot/update_json.py
+-rw-rw-rw-   0        0        0      967 2024-05-03 17:14:28.000000 medicafe-0.240506.1/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-07 00:54:31.350000 medicafe-0.240506.1/MediLink/
+-rw-rw-rw-   0        0        0    17958 2024-05-07 00:47:53.000000 medicafe-0.240506.1/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240506.1/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    19881 2024-04-30 22:21:02.000000 medicafe-0.240506.1/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    33095 2024-05-02 15:19:01.000000 medicafe-0.240506.1/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3791 2024-05-01 23:56:13.000000 medicafe-0.240506.1/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    10989 2024-05-06 23:09:35.000000 medicafe-0.240506.1/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7131 2024-05-02 10:20:35.000000 medicafe-0.240506.1/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240506.1/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     6297 2024-05-06 22:21:25.000000 medicafe-0.240506.1/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240506.1/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240506.1/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     4950 2024-04-30 21:38:34.000000 medicafe-0.240506.1/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0     5909 2024-05-02 10:20:36.000000 medicafe-0.240506.1/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240506.1/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240506.1/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240506.1/MediLink/__init__.py
+-rw-rw-rw-   0        0        0      730 2024-05-07 00:54:31.544000 medicafe-0.240506.1/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240506.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 00:54:31.526000 medicafe-0.240506.1/medicafe.egg-info/
+-rw-rw-rw-   0        0        0      730 2024-05-07 00:54:30.000000 medicafe-0.240506.1/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2024-05-07 00:54:30.000000 medicafe-0.240506.1/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 00:54:30.000000 medicafe-0.240506.1/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240506.1/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-07 00:54:30.000000 medicafe-0.240506.1/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-07 00:54:30.000000 medicafe-0.240506.1/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 00:54:31.556000 medicafe-0.240506.1/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2024-05-07 00:54:26.000000 medicafe-0.240506.1/setup.py
```

### Comparing `medicafe-0.240501.5/LICENSE` & `medicafe-0.240506.1/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.5/MediBot/MediBot.bat` & `medicafe-0.240506.1/MediBot/MediBot.bat`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.5/MediBot/MediBot.py` & `medicafe-0.240506.1/MediBot/MediBot.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,14 +198,16 @@
     pass 
 
 class ExecutionState:
     def __init__(self, config_path, crosswalk_path) -> None:
         try:
             config, crosswalk = MediLink_ConfigLoader.load_configuration(config_path, crosswalk_path)
             self.verify_config_type(config)
+            self.crosswalk = crosswalk
+            self.config = config
             MediLink_ConfigLoader.log("Config loaded successfully...")
             
             MediBot_Preprocessor.crosswalk_update(config, crosswalk)
             MediLink_ConfigLoader.log("Crosswalk update complete...")
             
             initialize(config)
             MediLink_ConfigLoader.log("Constants initialized...")
@@ -239,15 +241,15 @@
         
         e_state = ExecutionState(config_path, crosswalk_path)
         
         #print("Loading CSV Data...")
         csv_data = MediBot_Preprocessor.load_csv_data(CSV_FILE_PATH)
         
         #print("Pre-processing CSV Data...")
-        MediBot_Preprocessor.preprocess_csv_data(csv_data)  # Pre-process CSV data to add combined fields
+        MediBot_Preprocessor.preprocess_csv_data(csv_data, e_state.crosswalk)  # Pre-process CSV data to add combined fields & crosswalk values.
         headers = csv_data[0].keys() # Including Patient Name and Patient Address
         
         #print("Performing Intake Scan...")
         # identified_fields is an OrderedDict
         identified_fields = MediBot_Preprocessor.intake_scan(headers, field_mapping)
         
         # Reverse the identified_fields mapping for lookup
```

### Comparing `medicafe-0.240501.5/MediBot/MediBot_Charges.py` & `medicafe-0.240506.1/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.5/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240506.1/MediBot/MediBot_Preprocessor.py`

 * *Files 4% similar despite different names*

```diff
@@ -210,29 +210,27 @@
             file_path = os.path.join(directory_path, filename)
             if filename.endswith('.csv'):
                 try:
                     with open(file_path, 'r', encoding='utf-8') as csvfile:
                                 reader = csv.DictReader(csvfile)
                                 found_data = False  # Flag to track if any valid data is found in the CSV
                                 for row in reader:
-                                    if 'Patient ID' not in row:
-                                        raise ValueError("CSV file '{}' is misformatted or empty.".format(filename))
-                                    elif not row.get('Patient ID').strip():
-                                        raise ValueError("CSV file '{}' is misformatted: Missing or empty 'Patient ID' in row {}".format(filename, row))
+                                    if 'Patient ID' not in row or 'Ins1 Payer ID' not in row:
+                                        continue  # Skip this row if either key is missing
+                                    if not row.get('Patient ID').strip() or not row.get('Ins1 Payer ID').strip():
+                                        continue  # Skip this row if either value is missing or empty
                                     
-                                    # Check if 'Ins1 Payer ID' exists and is not empty
-                                    payer_id = row.get('Ins1 Payer ID', '').strip()
-                                    if payer_id:
-                                        found_data = True
-                                        patient_id = row['Patient ID'].strip()
-                                        payer_to_patient_ids[payer_id].add(patient_id)
-                                        MediLink_ConfigLoader.log("Found Patient ID {} with Payer ID {}".format(patient_id, payer_id))
+                                    found_data = True
+                                    payer_id = row['Ins1 Payer ID'].strip()
+                                    patient_id = row['Patient ID'].strip()
+                                    payer_to_patient_ids[payer_id].add(patient_id)
+                                    MediLink_ConfigLoader.log("Found Patient ID {} with Payer ID {}".format(patient_id, payer_id))
                                 
                                 if not found_data:
-                                    raise ValueError("CSV file '{}' is empty.".format(filename))
+                                    raise ValueError("CSV file '{}' is empty or does not have either Patient ID or Payer ID.".format(filename))
                 except Exception as e:
                     print("Error processing file {}: {}".format(filename, e))
     except FileNotFoundError as e:
         print("Error: {}".format(e))
 
     if not payer_to_patient_ids:
         print("No historical mappings were generated.")
@@ -250,22 +248,23 @@
 
     Output: A fully populated crosswalk.json file that serves as a baseline for future updates.
     """
     payer_id_to_details = {}
     
     # Load historical Patient ID to Insurance ID mappings from MAPAT
     patient_id_to_insurance_id = load_insurance_data_from_mapat(config, crosswalk)
-
+    print(patient_id_to_insurance_id)
     # Check if patient_id_to_insurance_id is empty
     if not patient_id_to_insurance_id:
         print("Error: Failed to load historical Patient ID to Insurance ID mappings from MAPAT.")
         sys.exit(1)
 
     # Process historical Carol's CSVs
     payer_id_to_patient_ids = load_historical_payer_to_patient_mappings(config)
+    print(payer_id_to_patient_ids)
     
     # Check if payer_id_to_patient_ids is empty
     if not payer_id_to_patient_ids:
         print("Error: Failed to load historical Carol's CSVs.")
         sys.exit(1)
 
     # Map Payer IDs to Insurance IDs
@@ -391,15 +390,15 @@
     crosswalk_path = config['MediLink_Config'].get('crosswalkPath')
     if not save_crosswalk(crosswalk_path, crosswalk):
         return False
 
     return True
 
 # CSV Preprocessor built for Carol
-def preprocess_csv_data(csv_data):
+def preprocess_csv_data(csv_data, crosswalk):
     try:
         # Filter out rows without a Patient ID
         csv_data[:] = [row for row in csv_data if row.get('Patient ID', '').strip()]
         
         # Remove Patients (rows) that are Primary Insurance: 'AETNA', 'AETNA MEDICARE', or 'HUMANA MED HMO'.
         csv_data[:] = [row for row in csv_data if row.get('Primary Insurance', '').strip() not in ['AETNA', 'AETNA MEDICARE', 'HUMANA MED HMO']]
                 
@@ -424,14 +423,16 @@
         # Update csv_data to only include unique patient records
         csv_data[:] = list(unique_patients.values())
 
         # Re-sort the csv_data after deduplication to ensure correct order
         csv_data.sort(key=lambda x: (x['Surgery Date'], x.get('Patient Last', '').strip()))
         
         # Maybe make a dataformat_library function for this? csv_data = format_preprocessor(csv_data)?
+        # Maybe not though because we're now adding a column using this same loop. Maybe they should be 
+        # separate though...
         for row in csv_data:
             # Convert 'Surgery Date' back to string format if needed for further processing (cleanup)
             row['Surgery Date'] = row['Surgery Date'].strftime('%m/%d/%Y')
             
             # Combine name fields
             first_name = row.get('Patient First', '').strip()
             middle_name = row.get('Patient Middle', '').strip()
@@ -439,30 +440,51 @@
             row['Patient Name'] = "{}, {} {}".format(last_name, first_name, middle_name).strip()
 
             # Combine address fields
             address1 = row.get('Patient Address1', '').strip()
             address2 = row.get('Patient Address2', '').strip()
             row['Patient Street'] = "{} {}".format(address1, address2).strip()
             
-            # Probably make a data_format function for this:
-            # Define the replacements as a dictionary
+            # Probably make a data_format function for this?
+            # Define the replacements as a dictionary.
+            # TODO this probably needs to sit in the config eventually and not hardcode
             replacements = {
                 '777777777': '',  # Replace '777777777' with an empty string
                 'RAILROAD MEDICARE': 'RAILROAD',  # Replace 'RAILROAD MEDICARE' with 'RAILROAD'
                 'AARP MEDICARE COMPLETE': 'AARP COMPLETE'  # Replace 'AARP MEDICARE COMPLETE' with 'AARP COMPLETE'
             }
 
             # Iterate over each key-value pair in the replacements dictionary
             for old_value, new_value in replacements.items():
                 # Replace the old value with the new value if it exists in the row
                 if row.get('Patient SSN', '') == old_value:
                     row['Patient SSN'] = new_value
                 elif row.get('Primary Insurance', '') == old_value:
                     row['Primary Insurance'] = new_value
 
+            # TODO This is probably the wrong place to implement this? 
+            # TODO Also check to see if it's not overwriting the Medicare '1' assginment within triage.
+            # Add a column with header "Ins1 Insurance ID" based on crosswalk and "Ins1 Payer ID" column for each row
+            ins1_payer_id = row.get('Ins1 Payer ID', '').strip()  # Get the Ins1 Payer ID from the row
+            if ins1_payer_id:  # Check if Ins1 Payer ID is not empty
+                if ins1_payer_id in crosswalk.get('payer_id', {}):  # Check if Ins1 Payer ID exists in the crosswalk
+                    # Get the corresponding medisoft_id(s) for the Ins1 Payer ID from the crosswalk
+                    medisoft_ids = crosswalk['payer_id'][ins1_payer_id].get('medisoft_id', [])
+                    if medisoft_ids:  # Check if medisoft_ids exist
+                        # TODO Default now is always Assign the first medisoft_id to the "Ins1 Insurance ID" column.
+                        # This needs to be updated so try to match against Carol's naming convention to get a better match
+                        row['Ins1 Insurance ID'] = medisoft_ids[0]
+                else:
+                    # TODO If Ins1 Payer ID is not found in the crosswalk then we should make a crosswalk_update entry for the new payer_id
+                    # and then it should be passively looking for when the user updates one of these patients in Medisoft. This behavior
+                    # should already be covered by the way crosswalk_update works or by the initializer or something, but the initialization
+                    # is still pretty janky and I think it will miss older assignments if it doesn't basically do a full re-initialize each time. 
+                    # Obviously diminishing returns on age of CSV.
+                    MediLink_ConfigLoader.log("Ins1 Payer ID '{}' not found in the crosswalk.".format(ins1_payer_id))
+
     except Exception as e:
         print("An error occurred while pre-processing CSV data. Please repair the CSV directly and try again:", e)
 
 def check_existing_patients(selected_patient_ids, MAPAT_MED_PATH):
     existing_patients = []
     patients_to_process = list(selected_patient_ids)  # Clone the selected patient IDs list
 
@@ -556,15 +578,15 @@
         print("Loading CSV data...")
         csv_data = load_csv_data(config['CSV_FILE_PATH'])
         print("Loaded {} records from the CSV.".format(len(csv_data)))
 
     if args.preprocess_csv:
         if 'csv_data' in locals():
             print("Preprocessing CSV data...")
-            preprocess_csv_data(csv_data)
+            preprocess_csv_data(csv_data, crosswalk)
         else:
             print("Error: CSV data needs to be loaded before preprocessing. Use --load-csv.")
     
     if args.open_csv:
         print("Opening CSV for editing...")
         open_csv_for_editing(config['CSV_FILE_PATH'])
```

### Comparing `medicafe-0.240501.5/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240506.1/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.5/MediBot/MediBot_UI.py` & `medicafe-0.240506.1/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.5/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240506.1/MediBot/MediBot_dataformat_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.5/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240506.1/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.5/MediBot/update_json.py` & `medicafe-0.240506.1/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.5/MediLink/MediLink.py` & `medicafe-0.240506.1/MediLink/MediLink.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import logging
 import MediLink_Down
 import MediLink_Up
 import MediLink_ConfigLoader
 import MediLink_837p_encoder
 
 # For UI Functions
 import os
@@ -124,15 +123,14 @@
         # TODO This suggested endpoint should be a payerid_to_endpoint_mapping.
         # BUG No, we've completely changed this structure so the whole thing is wrong.
         # We're going to have something like payer_id {endpoint:'AVAILITY', insurance_id: {105, 12}}
         # we'll need MAINS to map primary_insurance to insurance_id first and then look for the number in the values.
         try:
             suggested_endpoint = crosswalk['insurance_to_endpoint_mapping'][primary_insurance]
         except KeyError:
-            print("The new crosswalk logic needs to be implemented!")
             suggested_endpoint = 'AVAILITY'
 
         # Directly enrich detailed patient data with additional information and suggested endpoint
         detailed_data = parsed_data.copy()  # Copy parsed_data to avoid modifying the original dictionary
         detailed_data.update({
             'file_path': file_path,
             'patient_id': parsed_data.get('CHART'),
@@ -203,14 +201,17 @@
         else:
             print("No endpoints were processed.")
 
 def user_decision_on_suggestions(detailed_patient_data, config):
     """
     Presents the user with all patient summaries and suggested endpoints,
     then asks for confirmation to proceed with all or specify adjustments manually.
+    
+    BUG The display summary suggested_endpoint key isn't updating per the user's decision 
+    although the user decision is persisting.
     """
     # Display summaries of patient details and endpoints.
     MediLink_UI.display_patient_summaries(detailed_patient_data)
 
     # Ask the user if they want to proceed with all suggested endpoints.
     proceed = MediLink_UI.ask_for_proceeding_with_endpoints()
 
@@ -229,14 +230,18 @@
         if 'confirmed_endpoint' not in data:
             data['confirmed_endpoint'] = data['suggested_endpoint']
     return detailed_patient_data
 
 def select_and_adjust_files(detailed_patient_data, config):
     """
     Allows users to select patients and adjust their endpoints by interfacing with UI functions.
+    
+    BUG After the user is done making their selection, suggested_endpoint should update to persist the 
+    user selection as priority over its original suggestion. Also, the crosswalk should persist the change 
+    in the endpoint as well.
     """
     # Display options for patients
     MediLink_UI.display_patient_options(detailed_patient_data)
 
     # Get user-selected indices for adjustment
     selected_indices = MediLink_UI.get_selected_indices(len(detailed_patient_data))
     
@@ -253,14 +258,15 @@
             MediLink_UI.display_endpoint_options(config['MediLink_Config']['endpoints'])
             endpoint_index = int(MediLink_UI.get_new_endpoint_choice()) - 1  # Adjusting for zero-based index
             
             if 0 <= endpoint_index < len(endpoint_keys):
                 selected_endpoint_key = endpoint_keys[endpoint_index]
                 data['confirmed_endpoint'] = selected_endpoint_key
                 print("Endpoint changed to {0} for patient {1}.".format(config['MediLink_Config']['endpoints'][selected_endpoint_key]['name'], data['patient_name']))
+                # BUG Probably update crosswalk and suggested endpoint here???
             else:
                 print("Invalid selection. Keeping the suggested endpoint.")
         else:
             data['confirmed_endpoint'] = data.get('suggested_endpoint', 'N/A')
 
     return detailed_patient_data
```

### Comparing `medicafe-0.240501.5/MediLink/MediLink_277_decoder.py` & `medicafe-0.240506.1/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.5/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240506.1/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.5/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240506.1/MediLink/MediLink_837p_encoder_library.py`

 * *Files 1% similar despite different names*

```diff
@@ -424,20 +424,31 @@
     # Determine the payer responsibility sequence number code based on the payer type
     # If the payer is Medicare, use 'P' (Primary)
     # If the payer is not Medicare and is primary insurance, use 'P' (Primary)
     # If the payer is secondary insurance after Medicare, use 'S' (Secondary)
     # Assume everything is Primary for now.
     responsibility_code = 'P'
 
-    # Determine the insurance type code based on the payer
-    # Map different payers to their respective insurance type codes
-    # For simplicity, 'CI' (Commercial Insurance) as a default
-    # BUG I have no idea how to solve this. 
-    # TODO This needs to be a user menu option for now.
+    # Insurance Type Code
+    insurance_type_code = insurance_type_selection()
+
+
+    # Construct the SBR segment using the determined codes
+    sbr_segment = "SBR*{responsibility_code}*18*******{insurance_type_code}~".format(
+        responsibility_code=responsibility_code,
+        insurance_type_code=insurance_type_code
+    )
+
+    return sbr_segment
+
+def insurance_type_selection():
     """
+    TODO Finish making this function. This should integrate into a menu for now and then figure 
+    out the automated/API method to getting this.
+    
     11 - Other Non-Federal Programs
     12 - Preferred Provider Organization (PPO)
     13 - Point of Service (POS)
     14 - Exclusive Provider Organization (EPO)
     15 - Indemnity Insurance
     16 - Health Maintenance Organization (HMO) Medicare Risk
     17 - Dental Maintenance Organization
@@ -455,23 +466,15 @@
     OF - Other Federal Program
     TV - Title V
     VA - Veterans Affairs Plan
     WC - Workers’ Compensation Health Claim
     ZZ - Mutually Defined (This is generic default setting)
     """
     insurance_type_code = 'CI'
-
-
-    # Construct the SBR segment using the determined codes
-    sbr_segment = "SBR*{responsibility_code}*18*******{insurance_type_code}~".format(
-        responsibility_code=responsibility_code,
-        insurance_type_code=insurance_type_code
-    )
-
-    return sbr_segment
+    return insurance_type_code
 
 # Constructs the NM1 segment for subscriber based on parsed data and configuration.
 def create_nm1_subscriber_segment(config, parsed_data, endpoint):
     if endpoint.lower() == 'optumedi':
         entity_identifier_code = config['endpoints']['OPTUMEDI'].get('subscriber_entity_code', 'IL')
     else:
         entity_identifier_code = 'IL'  # Default value if endpoint is not 'optumedi'
```

### Comparing `medicafe-0.240501.5/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240506.1/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.5/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240506.1/MediLink/MediLink_DataMgmt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import csv
 import os
 from datetime import datetime, timedelta
-import logging
 import subprocess # BUG Currently disabled for testing.
-import logging
 
 # Need this for running Medibot and MediLink
 try:
     import MediLink_ConfigLoader
 except ImportError:
     from . import MediLink_ConfigLoader
 
@@ -104,15 +102,15 @@
         writer = csv.writer(csvfile)
         writer.writerows(consolidated_data)
 
     MediLink_ConfigLoader.log("Consolidated CSVs into {}".format(consolidated_filepath))
     
     return consolidated_filepath
 
-def operate_winscp(operation_type, files, endpoint_config, local_storage_path):
+def operate_winscp(operation_type, files, endpoint_config, local_storage_path, config):
     """
     General function to operate WinSCP for uploading or downloading files.
 
     :param operation_type: 'upload' or 'download'
     :param files: List of files to upload or pattern for files to download.
     :param endpoint_config: Dictionary containing endpoint configuration.
     :param local_storage_path: Base local storage path for logs and files.
@@ -120,23 +118,23 @@
     # Example of how to call this function for uploads
     upload_files = ['path/to/local/file1.txt', 'path/to/local/file2.txt']
     upload_config = {
         'session_name': 'MySession',
         'remote_directory_up': '/remote/upload/path'
     }
 
-    operate_winscp('upload', upload_files, upload_config, 'path/to/local/storage')
+    operate_winscp('upload', upload_files, upload_config, 'path/to/local/storage', config)
 
     # Example of how to call this function for downloads
     download_config = {
         'session_name': 'MySession',
         'remote_directory_down': '/remote/download/path'
     }
 
-    operate_winscp('download', None, download_config, 'path/to/local/storage')
+    operate_winscp('download', None, download_config, 'path/to/local/storage', config)
     """
     # Setup paths
     try:
         winscp_path = endpoint_config['winscp_path']
     except KeyError:
         winscp_path = os.path.join(os.getcwd(), "Installers", "WinSCP-Portable", "WinSCP.com")
     except Exception as e:
@@ -178,17 +176,24 @@
             normalized_path = os.path.normpath(file_path)
             command.append("put \"{}\"".format(normalized_path))
     else:
         command.append('get *')  # Adjust pattern as needed
 
     command += ['close', 'exit']
 
-    # Execute command
-    # process = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=False)
-    # stdout, stderr = process.communicate()
+    # Check if TestMode is enabled in the configuration
+    if config.get("MediLink_Config", {}).get("TestMode", True):
+        # TestMode is enabled, do not execute the command
+        print("Test Mode is enabled. Command not executed.")
+        return None, None
+    else:
+        # TestMode is not enabled, execute the command
+        process = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=False)
+        stdout, stderr = process.communicate()
+
     
     if True: #process.returncode == 0:
         # Replace this with your condition to check if WinSCP operation was successful
         # BUG This return code is a little trigger happy.
         # BUG If the WinSCP command specifies the correct download path, this might not be necessary
         # move_downloaded_files(local_storage_path)
         # print("WINSCP IS CURRENTLY DISABLED FOR TESTING.") # BUG
```

### Comparing `medicafe-0.240501.5/MediLink/MediLink_Down.py` & `medicafe-0.240506.1/MediLink/MediLink_Down.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         endpoint_key = 'AVAILITY'
     
     # Retrieve endpoint configuration and local storage path
     endpoint_config = config['MediLink_Config']['endpoints'][endpoint_key]
     local_storage_path = config['MediLink_Config']['local_storage_path']
         
     # Download ERA files from the configured endpoint
-    downloaded_files = operate_winscp("download", None, endpoint_config, local_storage_path)
+    downloaded_files = operate_winscp("download", None, endpoint_config, local_storage_path, config)
 
     # Translate downloaded ERA files to CSV format
     translated_csv_paths = []
     for file in downloaded_files:
         # TODO This needs to add functionality for differentiating between ERA, 277, IBT or 
         # whatever else might be included in the download folders.
         MediLink_ERA_decoder.translate_era_to_csv([file], output_directory)
```

### Comparing `medicafe-0.240501.5/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240506.1/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.5/MediLink/MediLink_Gmail.py` & `medicafe-0.240506.1/MediLink/MediLink_Gmail.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     - Authenticate and access Gmail to extract the 'Read the message' link.
     - Provide support for initial email filtering and link extraction.
     - Not involved in the decryption or direct handling of PHI data to ensure compliance with HIPAA.
 
 This architecture ensures the system handles sensitive PHI data in compliance with HIPAA regulations while maintaining robust and reliable email processing and file handling mechanisms. All sensitive data transfers occur directly from Microsoft's secure environment, minimizing the risk of unauthorized access during transit.
 """
 import requests
-import logging
 import webbrowser
 import time
 from MediLink_ConfigLoader import log
 
 def initiate_process():
     """
     Initiates the process to retrieve the link and OTP from the Google Apps Script,
@@ -77,15 +76,15 @@
         log("Failed to retrieve the link.")
 
 def retrieve_link():
     """
     Retrieves the 'Read the message' link from the Google Apps Script.
     """
     try:
-        url = "https://script.google.com/macros/s/AKfycby0E1fYhXO4DNQh9_D_TOArRfsko8LAnk1HN1SiZRb_RnErARvJHuWX5TaFW8xGB7aaKA/exec"
+        url = "https://script.google.com/macros/s/AKfycbzlq8d32mDlLdtFxgL_zvLJernlGPB64ftyxyH8F1nNlr3P-VBH6Yd0NGa1pbBc5AozvQ/exec"
         params = {'action': 'get_link'}
         response = requests.get(url, params=params)
         if response.status_code == 200 and response.text.startswith("http"):
             return response.text
         else:
             log("Failed to retrieve link: HTTP status {}, Response text: {}".format(response.status_code, response.text))
             return None
@@ -93,15 +92,15 @@
         log("Error retrieving link: {}".format(str(e)))
         return None
 
 def poll_for_otp():
     """
     Polls the Google Apps Script for the OTP, waiting until it is available.
     """
-    url = "https://script.google.com/macros/s/AKfycby0E1fYhXO4DNQh9_D_TOArRfsko8LAnk1HN1SiZRb_RnErARvJHuWX5TaFW8xGB7aaKA/exec"
+    url = "https://script.google.com/macros/s/AKfycbzlq8d32mDlLdtFxgL_zvLJernlGPB64ftyxyH8F1nNlr3P-VBH6Yd0NGa1pbBc5AozvQ/exec"
     params = {'action': 'get_otp'}
     timeout = time.time() + 60*3  # Poll for 3 minutes max
     while time.time() < timeout:
         response = requests.get(url, params=params)
         if response.status_code == 200 and response.text.isdigit():
             return response.text
         elif response.status_code != 200:
```

### Comparing `medicafe-0.240501.5/MediLink/MediLink_Scheduler.py` & `medicafe-0.240506.1/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.5/MediLink/MediLink_UI.py` & `medicafe-0.240506.1/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.5/MediLink/MediLink_Up.py` & `medicafe-0.240506.1/MediLink/MediLink_Up.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,19 +66,16 @@
 
         # Confirm transmission to each endpoint with detailed overview
         if True: #confirm_transmission({endpoint: patients_data}):
             if check_internet_connection():
                 # Process and transmit files per endpoint
                 converted_files = MediLink_837p_encoder.convert_files_for_submission(patients_data, config)
                 if converted_files:  # Check if files were successfully converted
-                    # BUG DISABLE TRANSMISSION FOR TESTING
-                    # transmission_result = operate_winscp("upload", converted_files, config['MediLink_Config']['endpoints'][endpoint], config['MediLink_Config']['local_claims_path'])
-                    print("Would have uploaded here!") # DEBUG
-                    
-                    # handle_transmission_result(transmission_result)
+                    transmission_result = operate_winscp("upload", converted_files, config['MediLink_Config']['endpoints'][endpoint], config['MediLink_Config']['local_claims_path'], config)
+                    handle_transmission_result(transmission_result)
                     # This doesn't really do much
                     # BUG This has to fail better. If one endpoint is unreachable, it should still try the next endpoint.
                     # BUG handle_transmission_result is wrong.
                 else:
                     print("No files were converted for transmission to {0}.".format(endpoint))
             else:
                 print("No internet connection detected.")
```

### Comparing `medicafe-0.240501.5/PKG-INFO` & `medicafe-0.240506.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240501.5
+Version: 0.240506.1
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240501.5/README.md` & `medicafe-0.240506.1/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.5/medicafe.egg-info/PKG-INFO` & `medicafe-0.240506.1/medicafe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240501.5
+Version: 0.240506.1
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240501.5/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240506.1/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.5/setup.py` & `medicafe-0.240506.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240501.5",
+    version="0.240506.1",
     description='MediCafe',
     long_description='This module ensures that MediCafe remains up-to-date by performing version checks for its dependencies on startup. It utilizes PyPI, the official repository for Python packages, to retrieve information about the latest available versions of the required packages. When an internet connection is available, MediUpdate automatically installs any available updates using pip, the package installer for Python.',
     long_description_content_type='text/markdown',
     keywords = 'medicafe python34 medibot medilink',
     url='https://github.com/katanada2',
     author='Daniel Vidaud',
     author_email='daniel@personalizedtransformation.com',
```

