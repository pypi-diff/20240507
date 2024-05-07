# Comparing `tmp/glyco-0.0.1rc1.tar.gz` & `tmp/glyco-0.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glyco-0.0.1rc1.tar", last modified: Mon Sep 18 09:58:27 2023, max compression
+gzip compressed data, was "glyco-0.0.1rc2.tar", last modified: Tue May  7 17:46:15 2024, max compression
```

## Comparing `glyco-0.0.1rc1.tar` & `glyco-0.0.1rc2.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 ismail     (501) admin       (80)        0 2023-09-18 09:58:27.780706 glyco-0.0.1rc1/
--rw-r--r--   0 ismail     (501) admin       (80)     1075 2023-09-17 17:53:58.000000 glyco-0.0.1rc1/LICENSE
--rw-r--r--   0 ismail     (501) admin       (80)     8507 2023-09-18 09:58:27.779915 glyco-0.0.1rc1/PKG-INFO
--rw-r--r--   0 ismail     (501) admin       (80)     6084 2023-09-18 09:58:07.000000 glyco-0.0.1rc1/README.md
--rw-r--r--   0 ismail     (501) admin       (80)     1187 2023-09-18 09:51:53.000000 glyco-0.0.1rc1/pyproject.toml
--rw-r--r--   0 ismail     (501) admin       (80)       38 2023-09-18 09:58:27.780854 glyco-0.0.1rc1/setup.cfg
-drwxr-xr-x   0 ismail     (501) admin       (80)        0 2023-09-18 09:58:27.687464 glyco-0.0.1rc1/src/
-drwxr-xr-x   0 ismail     (501) admin       (80)        0 2023-09-18 09:58:27.758383 glyco-0.0.1rc1/src/glyco/
--rw-r--r--   0 ismail     (501) admin       (80)      102 2023-09-17 17:53:58.000000 glyco-0.0.1rc1/src/glyco/__init__.py
--rw-r--r--   0 ismail     (501) admin       (80)      227 2023-09-17 17:53:58.000000 glyco-0.0.1rc1/src/glyco/constants.py
--rw-r--r--   0 ismail     (501) admin       (80)        6 2023-09-16 14:36:33.000000 glyco-0.0.1rc1/src/glyco/features.py
--rw-r--r--   0 ismail     (501) admin       (80)    45039 2023-09-18 09:49:30.000000 glyco-0.0.1rc1/src/glyco/glucose.py
--rw-r--r--   0 ismail     (501) admin       (80)    20270 2023-09-18 09:49:48.000000 glyco-0.0.1rc1/src/glyco/meals.py
--rw-r--r--   0 ismail     (501) admin       (80)     4476 2023-09-17 17:53:58.000000 glyco-0.0.1rc1/src/glyco/utils.py
-drwxr-xr-x   0 ismail     (501) admin       (80)        0 2023-09-18 09:58:27.771873 glyco-0.0.1rc1/src/glyco.egg-info/
--rw-r--r--   0 ismail     (501) admin       (80)     8507 2023-09-18 09:58:27.000000 glyco-0.0.1rc1/src/glyco.egg-info/PKG-INFO
--rw-r--r--   0 ismail     (501) admin       (80)      372 2023-09-18 09:58:27.000000 glyco-0.0.1rc1/src/glyco.egg-info/SOURCES.txt
--rw-r--r--   0 ismail     (501) admin       (80)        1 2023-09-18 09:58:27.000000 glyco-0.0.1rc1/src/glyco.egg-info/dependency_links.txt
--rw-r--r--   0 ismail     (501) admin       (80)       46 2023-09-18 09:58:27.000000 glyco-0.0.1rc1/src/glyco.egg-info/entry_points.txt
--rw-r--r--   0 ismail     (501) admin       (80)      116 2023-09-18 09:58:27.000000 glyco-0.0.1rc1/src/glyco.egg-info/requires.txt
--rw-r--r--   0 ismail     (501) admin       (80)        6 2023-09-18 09:58:27.000000 glyco-0.0.1rc1/src/glyco.egg-info/top_level.txt
-drwxr-xr-x   0 ismail     (501) admin       (80)        0 2023-09-18 09:58:27.773151 glyco-0.0.1rc1/tests/
--rw-r--r--   0 ismail     (501) admin       (80)      501 2023-09-17 17:53:58.000000 glyco-0.0.1rc1/tests/test.py
+drwxr-xr-x   0 ismail     (501) admin       (80)        0 2024-05-07 17:46:15.578995 glyco-0.0.1rc2/
+-rw-r--r--   0 ismail     (501) admin       (80)     1075 2023-09-17 17:53:58.000000 glyco-0.0.1rc2/LICENSE
+-rw-r--r--   0 ismail     (501) admin       (80)     9212 2024-05-07 17:46:15.560271 glyco-0.0.1rc2/PKG-INFO
+-rw-r--r--   0 ismail     (501) admin       (80)     6815 2024-05-07 15:02:19.000000 glyco-0.0.1rc2/README.md
+-rw-r--r--   0 ismail     (501) admin       (80)     1169 2024-05-07 16:03:35.000000 glyco-0.0.1rc2/pyproject.toml
+-rw-r--r--   0 ismail     (501) admin       (80)       38 2024-05-07 17:46:15.582935 glyco-0.0.1rc2/setup.cfg
+drwxr-xr-x   0 ismail     (501) admin       (80)        0 2024-05-07 17:46:15.503898 glyco-0.0.1rc2/src/
+drwxr-xr-x   0 ismail     (501) admin       (80)        0 2024-05-07 17:46:15.527963 glyco-0.0.1rc2/src/glyco/
+-rw-r--r--   0 ismail     (501) admin       (80)      167 2024-05-07 13:56:43.000000 glyco-0.0.1rc2/src/glyco/__init__.py
+-rw-r--r--   0 ismail     (501) admin       (80)    50849 2024-05-07 16:23:03.000000 glyco-0.0.1rc2/src/glyco/glucose.py
+-rw-r--r--   0 ismail     (501) admin       (80)    21236 2024-05-07 16:25:09.000000 glyco-0.0.1rc2/src/glyco/meals.py
+-rw-r--r--   0 ismail     (501) admin       (80)     3890 2024-05-07 15:38:59.000000 glyco-0.0.1rc2/src/glyco/privacy.py
+-rw-r--r--   0 ismail     (501) admin       (80)     4401 2024-01-07 10:45:40.000000 glyco-0.0.1rc2/src/glyco/utils.py
+drwxr-xr-x   0 ismail     (501) admin       (80)        0 2024-05-07 17:46:15.556767 glyco-0.0.1rc2/src/glyco.egg-info/
+-rw-r--r--   0 ismail     (501) admin       (80)     9212 2024-05-07 17:46:15.000000 glyco-0.0.1rc2/src/glyco.egg-info/PKG-INFO
+-rw-r--r--   0 ismail     (501) admin       (80)      455 2024-05-07 17:46:15.000000 glyco-0.0.1rc2/src/glyco.egg-info/SOURCES.txt
+-rw-r--r--   0 ismail     (501) admin       (80)        1 2024-05-07 17:46:15.000000 glyco-0.0.1rc2/src/glyco.egg-info/dependency_links.txt
+-rw-r--r--   0 ismail     (501) admin       (80)       46 2024-05-07 17:46:15.000000 glyco-0.0.1rc2/src/glyco.egg-info/entry_points.txt
+-rw-r--r--   0 ismail     (501) admin       (80)      105 2024-05-07 17:46:15.000000 glyco-0.0.1rc2/src/glyco.egg-info/requires.txt
+-rw-r--r--   0 ismail     (501) admin       (80)        6 2024-05-07 17:46:15.000000 glyco-0.0.1rc2/src/glyco.egg-info/top_level.txt
+drwxr-xr-x   0 ismail     (501) admin       (80)        0 2024-05-07 17:46:15.556113 glyco-0.0.1rc2/tests/
+-rw-r--r--   0 ismail     (501) admin       (80)      605 2023-12-02 13:46:55.000000 glyco-0.0.1rc2/tests/test.py
+-rw-r--r--   0 ismail     (501) admin       (80)        0 2023-12-02 13:51:27.000000 glyco-0.0.1rc2/tests/test_features.py
+-rw-r--r--   0 ismail     (501) admin       (80)     2721 2023-12-02 15:00:03.000000 glyco-0.0.1rc2/tests/test_glucose.py
+-rw-r--r--   0 ismail     (501) admin       (80)        0 2023-12-02 13:51:27.000000 glyco-0.0.1rc2/tests/test_meals.py
+-rw-r--r--   0 ismail     (501) admin       (80)        0 2023-12-02 13:51:27.000000 glyco-0.0.1rc2/tests/test_privacy.py
+-rw-r--r--   0 ismail     (501) admin       (80)        0 2023-12-02 13:51:27.000000 glyco-0.0.1rc2/tests/test_utils.py
```

### Comparing `glyco-0.0.1rc1/LICENSE` & `glyco-0.0.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `glyco-0.0.1rc1/PKG-INFO` & `glyco-0.0.1rc2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glyco
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: Read and analyse continuous glucose monitoring data
 Author-email: Ismail Elouafiq <contact@ismail.bio>
 License: MIT License
         
         Copyright (c) [2022] [Ismail Elouafiq]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,15 +33,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: matplotlib-inline
 Requires-Dist: rich
 Requires-Dist: seaborn
@@ -130,14 +129,26 @@
     ```Python
     # you can provide a list or dataframe that contains the event times
     events = gl.get_events(event_times)
     ```
     You can even get the events from a folder of pictures. More on this in the [meals and events documentation](https://github.com/nidhog/glyco/blob/main/docs/concepts/events_and_meals.md)).
 3. **Advanced analysis of events**, including metrics for meals or events and how they impact glucose. As well as ranking meals and more, to further aid in understanding the glucose data.
 
+4. **On Privacy and Personally Identifieable Information** *Glyco also enables making the glucose data more private by hiding sensitive information*
+    ```Python
+    # you can set the 'mask_private_info' to true
+    anonymised_df = gl.read_csv(
+        file_path='my_glucose_data.csv',
+        mask_private_info=True
+        )
+    ```
+    The mask_private_info masks private information by: resetting the minimum datetime, removing specific columns (such as the device serial number), replacing categorical columns using a hash function and adding noise to the glucose data.
+
+    More details on how to use the privacy feature in [the privacy documentation here](https://github.com/nidhog/glyco/blob/main/docs/extra/privacy.md).
+
 ## Limitations
 * The metric calculations for days assumes the device timezone is the user's timezone.
 
 > ***Disclaimer*** Glyco is not a medical product and shall not be used to diagnose, treat or evaluate any medical conditions.
 For more on the intended use and indications of use please read the [healthcare considerations document](https://github.com/nidhog/glyco/blob/main/docs/extra/healthcare.md).
 
 ## Built on the shoulders of giants
```

### Comparing `glyco-0.0.1rc1/README.md` & `glyco-0.0.1rc2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -76,14 +76,26 @@
     ```Python
     # you can provide a list or dataframe that contains the event times
     events = gl.get_events(event_times)
     ```
     You can even get the events from a folder of pictures. More on this in the [meals and events documentation](https://github.com/nidhog/glyco/blob/main/docs/concepts/events_and_meals.md)).
 3. **Advanced analysis of events**, including metrics for meals or events and how they impact glucose. As well as ranking meals and more, to further aid in understanding the glucose data.
 
+4. **On Privacy and Personally Identifieable Information** *Glyco also enables making the glucose data more private by hiding sensitive information*
+    ```Python
+    # you can set the 'mask_private_info' to true
+    anonymised_df = gl.read_csv(
+        file_path='my_glucose_data.csv',
+        mask_private_info=True
+        )
+    ```
+    The mask_private_info masks private information by: resetting the minimum datetime, removing specific columns (such as the device serial number), replacing categorical columns using a hash function and adding noise to the glucose data.
+
+    More details on how to use the privacy feature in [the privacy documentation here](https://github.com/nidhog/glyco/blob/main/docs/extra/privacy.md).
+
 ## Limitations
 * The metric calculations for days assumes the device timezone is the user's timezone.
 
 > ***Disclaimer*** Glyco is not a medical product and shall not be used to diagnose, treat or evaluate any medical conditions.
 For more on the intended use and indications of use please read the [healthcare considerations document](https://github.com/nidhog/glyco/blob/main/docs/extra/healthcare.md).
 
 ## Built on the shoulders of giants
```

### Comparing `glyco-0.0.1rc1/pyproject.toml` & `glyco-0.0.1rc2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "glyco"
-version = "0.0.1rc1"
+version = "0.0.1rc2"
 description = "Read and analyse continuous glucose monitoring data"
 readme = "README.md"
 authors = [{ name = "Ismail Elouafiq", email = "contact@ismail.bio" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -22,15 +22,14 @@
     "glucose",
     "glyco",
     "cgm",
     "continuous glucose monitoring",
     "health",
     "healthcare"]
 dependencies = [
-    "matplotlib",
     "pandas",
     "scipy",
     "numpy",
     "matplotlib",
     "matplotlib-inline",
     "rich",
     "seaborn"]
```

### Comparing `glyco-0.0.1rc1/src/glyco/glucose.py` & `glyco-0.0.1rc2/src/glyco/glucose.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,96 +1,87 @@
-"""Defines glucose functions used in glyco"""
-from cProfile import label
-from enum import Enum, auto
+import hashlib
 import logging
-from typing import Callable, Dict, Optional, Union, List
+from datetime import date as date_type, datetime as dt, timedelta as tdel
+from typing import Callable, Dict, List, Optional, Union
+
 import pandas as pd
-# TODO: add logging
-# TODO use pydantic or dataclasses typedframe
-from datetime import datetime as dt, timedelta as tdel, date as date_type
 from matplotlib import pyplot as plt
+from rich.console import Console
+from rich.table import Table
 
-from .utils import Units, Devices, find_nearest, weekday_map, is_weekend, autoplot, units_to_mmolL_factor
-from .constants import GLUCOSE_COL, TIMESTAMP_COL
-from rich import print as rprint
-
+from glyco.privacy import mask_private_information
+from glyco.utils import Devices, Units, end_plot, find_nearest, is_weekend, units_to_mmolL_factor, weekday_map
 
 logger = logging.getLogger(__name__)
 """Warning and Error Messages
 """
 error_not_implemented_method = (
     "NOT IMPLEMENTED: Method not yet supported in this version."
 )
 
 """Default Values
 """
+TIMESTAMP_COL = 'tsp'
+GLUCOSE_COL = 'glucose'
 # Default values for column names as found in Freestyle Libre data
 DEFAULT_INPUT_TSP_COL = "Device Timestamp"
 DEFAULT_INPUT_GLUC_COL = "Historic Glucose mmol/L"
 
 # Default formats
 DEFAULT_INPUT_TSP_FMT = "%d-%m-%Y %H:%M"
 DEFAULT_OUT_DATE_FMT = "%d-%m-%Y (%A)"
 
-# Dafault value for glucose limit used as a threshold in the #TODO: properties, features, what name?
-DEFAULT_GLUC_LIMIT = 6
+DEFAULT_GLUC_LIMIT = 6 # glucose threshold used for calculating Area Under the Curve
 DEFAULT_CSV_DELIMITER = ","
 
 # Values for column names glyco generates in a dataframe
-# Note: All generated column variables start with an underscor '_'
+# Note: All generated column variables start with an underscore '_'
 _DT_COL = "dt"
 _DG_COL = "dg"
 _DGDT_COL = "dg_dt"
 _AUC_COL = "auc_mean"
 _AUCLIM_COL = "auc_lim"
 _AUCMIN_MIN = "auc_min"
 # time derivatives
 _DATE_COL = "date"
 _HOUR_COL = "hour"
 _DAYOFWEEK_COL = "weekday_number"
 _WEEKDAY_COL = "weekday_name"
 _ISWEEKEND_COL = "is_weekend"
 # Used for smoothening the glucose curve
-# FIXME: _default_glucose_prep_kwargs to GlucoseTransform dataclass
 _default_glucose_prep_kwargs = {
     'interpolate': True,
     'interp_met':'polynomial',
     'interp_ord':1,
     'rolling_avg':3,
 }
 
 # Meals
 _meal_note_col = "Notes"
 _meal_ref_col = "Reference"
 _freestyle_rec_type_col = "Record Type" # TODO separate freestyle specific to separate class in utils or devices
+_freestyle_serial_number_col = "Serial Number" 
 _freestyle_notes_rec_type = 6
 _freestyle_glucose_rec_type = 0
 _optional_cols = [_meal_note_col, _meal_ref_col]
 meal_default_cols = [TIMESTAMP_COL, _meal_ref_col, _meal_ref_col]
+_default_shift_hours = 7
+
+_default_private_info_kwargs = {
+    'set_start_date': '01-01-2023 00:00',
+    'remove_columns': [_freestyle_serial_number_col],
+    'replace_columns': [_meal_note_col],
+    'replace_func': lambda x: hashlib.sha256(str(x).encode()).hexdigest(),
+    'noise_std': 0.2
+}
 
 general_date_type = Union[str, pd.Timestamp, date_type]
 
-# TODO: complete and use schema
-# class FreeStyleInput(TypedDataFrame):
-#     schema = {
-#     }
 """File reading
 """
-
-# TODO LIST idiomatic: 
-# * use chaining to make code readable
-# * never mutate
-# * use agg([min, mean etc.]) instead of groupby repeats
-# * use unstack when plotting
-# * use the right type in gdf
-# * remove useless heavy columns only use necessary
-# * types int64 not need that much memory
-# * use chaining with assign with specific placement
-# * no need for date_str
-# * handle different timezones
 def read_csv(
     file_path: str,
     timestamp_col: str = DEFAULT_INPUT_TSP_COL,
     timestamp_fmt: str = DEFAULT_INPUT_TSP_FMT,
     glucose_col: str = DEFAULT_INPUT_GLUC_COL,
     glucose_unit: str = Units.mmolL.value,
     unit_autodetect: bool = False,
@@ -98,15 +89,17 @@
     glucose_lim: int=DEFAULT_GLUC_LIMIT,  # predefined glucose limit used for AUC calculation
     filter_glucose_rows=False,
     delimiter: str = DEFAULT_CSV_DELIMITER,
     skiprows: int = 0,
     generated_glucose_col: str = GLUCOSE_COL,
     generated_date_col: str = _DATE_COL,
     generated_timestamp_col: str =TIMESTAMP_COL,
-    glucose_prep_kwargs: Optional[Dict] = _default_glucose_prep_kwargs
+    glucose_prep_kwargs: Dict = _default_glucose_prep_kwargs,
+    mask_private_info: Optional[bool] = False,
+    private_info_kwargs: Optional[Dict] = _default_private_info_kwargs
 ) -> pd.DataFrame:
     # TODO: reorder by importance to improve UX
     # TODO: assert generated G column different from G column? Or warn if similar
     """Reads a CSV file with glucose data and generates a Glucose DataFrame.
     - The file needs to have at least: one column for glucose, one timestamp column.
 
     Args:
@@ -143,18 +136,26 @@
             Defaults to GLUCOSE_COL.
         generated_date_col (str, optional): the name of the generated date column
             in the resulting Glucose Dataframe. 
             Defaults to _DATE_COL.
         generated_timestamp_col (str, optional): the name of the generated timestamp 
             column in the resulting Glucose Dataframe. 
             Defaults to TIMESTAMP_COL.
-        glucose_prep_kwargs (Optional[Dict], optional): arugments that can be used 
+        glucose_prep_kwargs (Dict, optional): arugments that can be used 
             to smoothening the glucose curve.
             See the Glucose Prep Arguments section of the Glucose documentation.
             Defaults to _default_glucose_prep_kwargs.
+        mask_private_info (bool, optional): choose to mask or not to mask private information.
+            This uses the 'mask_private_information' function.
+            See the Privacy documentation for more on how this works.
+            Defaults to false.
+        private_info_kwargs (Optional[Dict], optional): arugments that can be used 
+            to mask private information. These are give to the 'mask_private_information' function.
+            See the Privacy documentation for more on how this works.
+            Defaults to _default_private_info_kwargs.
 
     Returns:
         pd.DataFrame: The resulting Glucose Dataframe that contains the file data, 
             along with the Generated Glucose Properties
     """
     df = pd.read_csv(
         filepath_or_buffer=file_path,
@@ -172,21 +173,17 @@
         calculate_glucose_properties=calculate_glucose_properties,
         glucose_lim=glucose_lim,
         filter_glucose_rows=filter_glucose_rows,
         generated_glucose_col=generated_glucose_col,
         generated_date_col=generated_date_col,
         generated_timestamp_col=generated_timestamp_col,
         glucose_prep_kwargs=glucose_prep_kwargs,
+        mask_private_info=mask_private_info,
+        private_info_kwargs=private_info_kwargs,
     )
-    # TODO: only one tsp
-    # TODO: only return important columns
-    # TODO: use insert to choose a position for columns
-    # TODO use assign instead
-    # TODO filter glucose record type only
-
     return df
 
 def validate_glucose_columns(df: pd.DataFrame, glucose_col: str, timestamp_col: str):
     """Validates the glucose and timestamp columns in the dataframe.
     Currently, only checks their existence.
 
     Args:
@@ -202,27 +199,29 @@
         raise ValueError(f"The Glucose column '{glucose_col}' is not in the input columns."\
             "Please provide 'glucose_col' as input.")
     if timestamp_col not in df.columns:
         raise ValueError(f"The Timestamp column '{timestamp_col}' is not in the input columns."\
             "Please provide 'timestamp_col' as input.")
     
 
-def read_df(df: pd.DataFrame, # TODO: rename to 'get_glucose_from_df'
+def read_df(df: pd.DataFrame,
     timestamp_col: str = DEFAULT_INPUT_TSP_COL,
     timestamp_fmt: str = DEFAULT_INPUT_TSP_FMT,
     glucose_col: str = DEFAULT_INPUT_GLUC_COL,
     glucose_unit: str = Units.mmolL.value,
     unit_autodetect : bool = False,
     calculate_glucose_properties: bool = True,
     glucose_lim: int=DEFAULT_GLUC_LIMIT, 
     filter_glucose_rows=False,
     generated_glucose_col: str = GLUCOSE_COL,
     generated_date_col: str = _DATE_COL,
     generated_timestamp_col: str =TIMESTAMP_COL,
-    glucose_prep_kwargs: Optional[Dict] = _default_glucose_prep_kwargs
+    glucose_prep_kwargs: Dict = _default_glucose_prep_kwargs,
+    mask_private_info: Optional[bool] = False,
+    private_info_kwargs: Optional[Dict] = _default_private_info_kwargs
 ):
     """Reads a pandas Dataframe with glucose data and generates a Glucose Dataframe.
     - The Dataframe needs to have at least: one column for glucose, one timestamp column.
 
     Args:
         df (pd.DataFrame): the pandas Dataframe with glucose data.
         timestamp_col (str, optional): the name of the timestamp column in the CSV file. 
@@ -254,70 +253,60 @@
             Defaults to GLUCOSE_COL.
         generated_date_col (str, optional): the name of the generated date column
             in the resulting Glucose Dataframe. 
             Defaults to _DATE_COL.
         generated_timestamp_col (str, optional): the name of the generated timestamp 
             column in the resulting Glucose Dataframe. 
             Defaults to TIMESTAMP_COL.
-        glucose_prep_kwargs (Optional[Dict], optional): arugments that can be used 
+        glucose_prep_kwargs (Dict, optional): arugments that can be used 
             to smoothening the glucose curve.
             See the Glucose Prep Arguments section of the Glucose documentation.
             Defaults to _default_glucose_prep_kwargs.
+        mask_private_info (bool, optional): choose to mask or not to mask private information.
+            This uses the 'mask_private_information' function.
+            See the Privacy documentation for more on how this works.
+            Defaults to false.
+        private_info_kwargs (Optional[Dict], optional): arugments that can be used 
+            to mask private information. These are give to the 'mask_private_information' function.
+            See the Privacy documentation for more on how this works.
+            Defaults to _default_private_info_kwargs.
 
     Returns:
         pd.DataFrame: The resulting Glucose Dataframe that contains the file data, 
             along with the Generated Glucose Properties.
-
-
-
-        TODO: only select the following from glucose, but add option to keep original columns:
-    keep_columns = ['Device', 'Device Timestamp', 'Record Type', 'Historic Glucose mmol/L', 'Scan Glucose mmol/L',
-    'Carbohydrates (grams)', 'Carbohydrates (servings)', 'Notes', 'Strip Glucose mmol/L', 'Ketone mmol/L'
-    
-    if not keep_original_columns else df.columns
-
-    we will then add 'date', 'date_str', 'hour',
-       'weekday_number', 'weekday_name', 'is_weekend', 'shifted_t',
-       'shifted_date', 'shifted_date_str', 'shifted_hour',
-       'shifted_weekday_number', 'shifted_weekday_name', 'shifted_is_weekend',
-       'G', 't', 'dg', 'dt', 'dg_dt', 'auc_mean', 'auc_lim', 'auc_min'
-     ]
-     TODO: we will ignore insulin measurements and following 
-    ['', 'Serial Number', '', '',
-       '', ',
-       'Non-numeric Rapid-Acting Insulin', 'Rapid-Acting Insulin (units)',
-       'Non-numeric Food', 'Carbohydrates (grams)', 'Carbohydrates (servings)',
-       'Non-numeric Long-Acting Insulin', 'Long-Acting Insulin Value (units)',
-       ''.
-       'Meal Insulin (units)', 'Correction Insulin (units)',
-       'User Change Insulin (units)', 
     """
     validate_glucose_columns(df=df, glucose_col=glucose_col, timestamp_col=timestamp_col)
+    # df = convert_tsp(ndf=df, tlbl=generated_timestamp_col, tsp_lbl=timestamp_col, timestamp_fmt=timestamp_fmt)
     if unit_autodetect:
         glucose_unit = autodetect_unit(df[glucose_col])
-        logger.info("Autodetected unit is (%s)", glucose_unit)
-    df = (
-        df
-        if not (filter_glucose_rows)
-        else filter_glucose_by_column_val(
+    logger.info("Using the glucose unit (%s)", glucose_unit)
+    # filter rows based on the values of a column (filter_val)
+    if filter_glucose_rows:
+        df = filter_glucose_by_column_val(
             df,
             filter_col=_freestyle_rec_type_col,
-            filter_val=_freestyle_glucose_rec_type,
+            filter_val=_freestyle_glucose_rec_type
         )
-    )
+    # mask private information
+    if mask_private_info:
+        df, _, _ = mask_private_information(gdf=df,
+        glucose_col=glucose_col,
+        tsp_col=timestamp_col,
+        tsp_fmt=timestamp_fmt,
+        **private_info_kwargs)
+    # add calculated glucose properties
     if calculate_glucose_properties:
-        if glucose_prep_kwargs is None:
-            glucose_prep_kwargs = _default_glucose_prep_kwargs
-        
-        df =( 
+        df =(
+            # 
             prepare_glucose(
                 glucose_df=df,
                 glucose_col=glucose_col,
                 tsp_lbl=timestamp_col,
                 timestamp_fmt=timestamp_fmt,
+                timestamp_is_formatted=False,
                 unit=glucose_unit,
                 glbl=generated_glucose_col,
                 tlbl=generated_timestamp_col,
                 dlbl=generated_date_col,
                 **glucose_prep_kwargs
             ).pipe(
                 get_properties, 
@@ -326,16 +315,16 @@
                 glim=glucose_lim
             )    
         )
     return df
 
 # Verify the file
 # List of implemented devices and units
-implemented_devices = list(map(lambda x: x.name, Devices))
-implemented_units = list(map(lambda x: x.name, Units))
+implemented_devices = list(map(lambda x: x.value, Devices))
+implemented_units = list(map(lambda x: x.value, Units))
 
 def is_valid_entry(unit: str, device: str, fail_on_invalid: bool = True) -> bool:
     """Verifies the device and unit are implemented.
 
     Args:
         device (str): name of the device used, e.g.: abbott
         unit (str): unit used, e.g.: mg/dL, mmol/L
@@ -390,17 +379,14 @@
     Returns:
         pd.DataFrame: dataframe where only specific columns are selected.
     """
     logger.info(f"Selecting only columns with a {filter_col} with the value {filter_val}")
     return df[df[filter_col] == filter_val]
 
 
-# TODO turn into function
-# TODO hide function as private or don't import in init
-# get datetime, date, hour etc. from timestamp
 def add_time_values(df, tlbl: str = TIMESTAMP_COL, tsp_lbl: str = DEFAULT_INPUT_TSP_COL, timestamp_fmt: str = DEFAULT_INPUT_TSP_FMT, dlbl: str = _DATE_COL, weekday_map=weekday_map, timestamp_is_formatted: bool = False):
     """Adds generated time-values to the dataframe based on the timestamp. These include:
     Date, Date string, Hour, Weekday number, Weekday name, Is or is not a weekend day.
 
     Args:
         df (_type_): the glucose dataframe.
         tlbl (str, optional): the name of the new timestamp column generated with datetime values.
@@ -423,56 +409,84 @@
     """
     ndf = df.copy()
     # if timestamp is not a string but already a pd.Timestamp type
     if timestamp_is_formatted:
         ndf[tlbl] = ndf[tsp_lbl]
     # else convert timestamp using timestamp_fmt
     else:
-        try:
-            ndf[tlbl] = pd.to_datetime(ndf[tsp_lbl], format=timestamp_fmt)
-        except ValueError as e:
-            raise ValueError(f"Failed to convert timestamp '{tsp_lbl}' using the format '{timestamp_fmt}'."\
-                f"Error: '{e}'."\
-                f"Verify that you are using the correct 'timestamp_fmt' as input")
+        ndf = convert_tsp(ndf=ndf, tlbl=tlbl, tsp_lbl=tsp_lbl, timestamp_fmt=timestamp_fmt)
     ndf[dlbl] = ndf[tlbl].dt.date
     ndf[f"{dlbl}_str"] = ndf[dlbl].map(lambda x: x.strftime(DEFAULT_OUT_DATE_FMT) if type(x)==pd.DatetimeIndex else x)
     ndf[_HOUR_COL] = ndf[tlbl].dt.hour
     ndf[_DAYOFWEEK_COL] = ndf[tlbl].dt.weekday
     ndf = ndf.assign()
     ndf[_WEEKDAY_COL] = ndf[_DAYOFWEEK_COL].map(weekday_map)
     ndf[_ISWEEKEND_COL] = ndf[_DAYOFWEEK_COL].map(is_weekend)
     return ndf
 
+def convert_tsp(ndf: pd.DataFrame, tlbl: str, tsp_lbl: str, timestamp_fmt: str) -> None:
+    """
+    Convert a timestamp column in a DataFrame to datetime using a specified format.
+
+    Args:
+        ndf (pd.DataFrame): The DataFrame containing the timestamp column to convert.
+        tlbl (str): The label for the new column where the converted timestamps will be stored.
+        tsp_lbl (str): The label of the timestamp column to convert.
+        timestamp_fmt (str): The format to use for parsing the timestamps.
+
+    Raises:
+        ValueError: If the timestamp conversion fails, this exception is raised with a detailed error message.
+
+    Example:
+    ```python
+    import pandas as pd
+
+    # Assuming you have a DataFrame `ndf`, column labels `tlbl`, `tsp_lbl`, and a valid `timestamp_fmt`.
+    convert_tsp(ndf, tlbl, tsp_lbl, timestamp_fmt)
+    ```
+    """
+    df = ndf.copy()
+    try:
+        df[tlbl] = pd.to_datetime(df[tsp_lbl], format=timestamp_fmt)
+        return df
+    except ValueError as e:
+        raise ValueError(f"Failed to convert timestamp '{tsp_lbl}' using the format '{timestamp_fmt}'. "
+                         f"Error: '{e}'. "
+                         f"Verify that you are using the correct 'timestamp_fmt' as input")
+
+
 def prepare_glucose(
     glucose_df: pd.DataFrame,
     glucose_col: str,
     tsp_lbl: str,
     timestamp_fmt: str,
     unit: str = Units.mmolL.value,
     glbl: str = GLUCOSE_COL,
     tlbl: str = TIMESTAMP_COL,
     dlbl: str = _DATE_COL,
+    timestamp_is_formatted: bool = True,
     interpolate: bool = True,
     interp_met: str = "polynomial",
     interp_ord: int = 1,
     rolling_avg: int = 3,
-    extra_shift_in_time: int = 7,
+    extra_shift_in_time: int = _default_shift_hours,
 ):
     """Parses the glucose data.
     - Creates extra columns for hours, days, etc.
     - Sorts the dataframe by time.
     - Creates columns for shifted time if needed (used for certain computations).
     - Converts units if needed.
     - Adds interpolated glucose measures to fill in the gaps.
 
     Args:
         df (pd.DataFrame): the glucose dataframe
         glucose_col (str): the name of the original glucose column
         tsp_lbl (str): the name of the original timestamp column
         tsp_fmt (str): the format of timestamps in the original timestamp column
+        timestamp_is_formatted (bool): wether the timestamp is already a datetime (no need for formatting)
         unit (str, optional): the unit of glucose values in the glucose column.
             Defaults to Units.mmol.value.
         glbl (str, optional): the name of the glucose column to be created.
             Defaults to GLUCOSE_COL.
         tlbl (str, optional): the name of the timestamp column to be created. 
             Defaults to TIMESTAMP_COL.
         dlbl (str, optional): the name of the date column to be created.
@@ -486,69 +500,70 @@
         rolling_avg (int, optional): the number used as a rolling average
             for glucose. Defaults to 3.
         extra_shift_in_time (int, optional): adds shifted time values. Defaults to 7.
 
     Returns:
         _type_: _description_
     """
-    df = add_time_values(glucose_df, tlbl=tlbl, dlbl=dlbl, tsp_lbl=tsp_lbl, timestamp_fmt=timestamp_fmt, weekday_map=weekday_map)
+    df = add_time_values(
+        glucose_df,
+        tlbl=tlbl,
+        dlbl=dlbl,
+        tsp_lbl=tsp_lbl,
+        timestamp_fmt=timestamp_fmt,
+        weekday_map=weekday_map,
+        timestamp_is_formatted=timestamp_is_formatted)
 
     if extra_shift_in_time:
         df = add_shifted_time(df, tlbl, dlbl, extra_shift_in_time)
 
     # convert to mmol/L
     df[glbl] = (
-        df[glucose_col]
+        pd.to_numeric(df[glucose_col])
         if unit == Units.mmolL.value
-        else convert_to_mmolL(df[glucose_col], from_unit=unit)
+        else convert_to_mmolL(pd.to_numeric(df[glucose_col]), from_unit=unit)
     )
 
     # index by time and keep time column
     df['idx'] = df[tlbl]
     df = df.set_index('idx').sort_index()
-
     # interpolate and smoothen glucose
     if interpolate:
-        # TODO handle Nan
-        # TODO FIX missing values should still be nan otherwise averaged
         df[glbl] = df[glbl].rolling(window=rolling_avg).mean()
-        # TODO smoothen methods
         df[glbl] = df[glbl].interpolate(method=interp_met, order=interp_ord)
         df = df[df[glbl].map(lambda g: g > 0 and g < 30)]
     return df
 
 
-def add_shifted_time(df: pd.DataFrame, tlbl: str, dlbl: str, extra_shift_in_time: int):
+def add_shifted_time(df: pd.DataFrame, tlbl: str, dlbl: str, shift_hours_back: int):
     """Adds shifted time values. 
     These are used by certain utility functions to make calculations faster,
     and to include nighttime glucose in certain calculations.
     See the shifted time values chapter in the glucose documentation for more.
 
     Args:
         df (pd.DataFrame): the glucose dataframe.
         tlbl (str): the timestamp column name.
         dlbl (str): the date column name.
-        extra_shift_in_time (int): how many hours for the shifted time values.
+        shift_hours_back (int): how many hours for the shifted time values.
             This value will be substracted (if negative, shift will happen forward).
     """
     shift_tlbl = f"shifted_{tlbl}"
     shift_dlbl = f"shifted_{dlbl}"
 
-    df[shift_tlbl] = df[tlbl].map(lambda x: x - tdel(hours=extra_shift_in_time))
+    df[shift_tlbl] = df[tlbl].map(lambda x: x - tdel(hours=shift_hours_back))
     df[shift_dlbl] = df[shift_tlbl].dt.date
     df[f"{shift_dlbl}_str"] = df[shift_dlbl].map(lambda x: x.strftime(DEFAULT_OUT_DATE_FMT))
     df[f"shifted_{_HOUR_COL}"] = df[shift_tlbl].dt.hour
     df[f"shifted_{_DAYOFWEEK_COL}"] = df[shift_tlbl].dt.weekday
     df[f"shifted_{_WEEKDAY_COL}"] = df[f"shifted_{_DAYOFWEEK_COL}"].map(weekday_map)
     df[f"shifted_{_ISWEEKEND_COL}"] = df[f"shifted_{_DAYOFWEEK_COL}"].map(is_weekend)
     return df
 
 
-
-
 """Properties and Stats
 """
 def set_derivative(
     df: pd.DataFrame, glucose_col: str, timestamp_col: str
 ) -> pd.DataFrame:
     """Sets the glucose time derivative (dG/dt)
 
@@ -654,15 +669,15 @@
         NotImplementedError: if the unit is not implemented.
             Implemented units are found in the Units Enum under utils.py
 
     Returns:
         float: converted glucose value
     """
     if from_unit in implemented_units:
-        return g * units_to_mmolL_factor[from_unit] # TODO fix inconsistency between implemented units and dict keys
+        return g * units_to_mmolL_factor[from_unit]
     raise NotImplementedError(error_not_implemented_method)
 
 
 def autodetect_unit(glucose_values: pd.Series) -> str:
     """Autodetects the Glucose unit as one of:
     - mmol/L
     - mg/dL
@@ -681,15 +696,15 @@
     logger.warning("Using unit autodetection." \
         "This may result in unexpected behavior.")
     cast_glucose_sample = pd.to_numeric(
             (
                 glucose_values
                 .sample(
                     n=min(100, len(glucose_values)),
-                    replacement=False
+                    replace=False
                 )
             ), errors='coerce')
     m = cast_glucose_sample.mean()
     if m > 33:
         return Units.mgdL.value
     if m > 6:
         return Units.mmolL.value
@@ -697,16 +712,14 @@
         return Units.gL.value
     return Units.mmolL.value
 
 
 """Plotting
 """
 
-
-@autoplot
 def plot_glucose(
     df: pd.DataFrame,
     glbl: str = GLUCOSE_COL,
     tlbl: str = TIMESTAMP_COL,
     from_time: Optional[general_date_type] = None,
     to_time: Optional[general_date_type] = None,
 ):
@@ -723,15 +736,14 @@
             Could be a string or timestamp or date.
             Defaults to None.
 
     Raises:
         KeyError: if the glucose column is not in the glucose dataframe
     """
     plot_df = df[from_time:to_time]
-    # TODO make as similar to pyplot as possible
 
     if glbl not in plot_df.keys():
         raise KeyError(f"Glucose Column {glbl} does not seem to be in the DataFrame.")
     for d in plot_df.date.unique():
         plt.axvline(d, color="brown", linestyle="--", alpha=0.5)
     plt.axhline(DEFAULT_GLUC_LIMIT)
     plt.axhline(DEFAULT_GLUC_LIMIT - 1)
@@ -749,25 +761,37 @@
 
     Args:
         df (pd.DataFrame): the glucose dataframe.
         glbl (str, optional): the glucose column name. Defaults to GLUCOSE_COL.
     """
     plot_percentiles(df, stat_col=glbl, group_by_col=_HOUR_COL, percentiles=[0.01, 0.05])
 
+
 def plot_trend_by_weekday(df: pd.DataFrame, glbl=GLUCOSE_COL):
     """Plots the glucose trend for each weekday (Monday to Sunday) as
     a box plot for each weekday.
 
     Args:
         df (pd.DataFrame): the glucose dataframe.
         glbl (str, optional): the glucose column name. Defaults to GLUCOSE_COL.
     """
     plot_comparison(df=df, glbl=glbl, compare_by=_WEEKDAY_COL, outliers=False, label_map=None, method='box', sort_vals = False)
 
 
+def plot_trend_by_day(df: pd.DataFrame, glbl=GLUCOSE_COL):
+    """Plots the glucose trend for each weekday (Monday to Sunday) as
+    a box plot for each weekday.
+
+    Args:
+        df (pd.DataFrame): the glucose dataframe.
+        glbl (str, optional): the glucose column name. Defaults to GLUCOSE_COL.
+    """
+    plot_comparison(df=df, glbl=glbl, compare_by=_DATE_COL, outliers=False, label_map=None, method='box', sort_vals = False)
+
+
 def plot_percentiles(df: pd.DataFrame, stat_col: str, percentiles: List[float], group_by_col: str=_HOUR_COL, color: str='green', label: str=None):
     """Groups glucose by a column column and plots percentiles of glucose.
     Percentiles are plotted using an area color between the main curve and each percentile.
     Does not show plot.
 
     Args:
         df (pd.DataFrame): the glucose dataframe.
@@ -776,39 +800,77 @@
         group_by_col (str, optional): the name of the column to group values by (X-axis).
             Defaults to _HOUR_COL.
         color (str, optional): the name of the color to use for the percentiles area. 
             Defaults to 'green'.
         label (str, optional): the title of the plot. 
             Defaults to None.
     """
-    # TODO use only get_stats and remove get_percentiles_and_stats
+    # TODO use only get_stats and remove get_percentiles_and_stats?
     _, _, med, perc_l, perc_h = get_percentiles_and_stats(
         df, percentiles, stat_col, group_by_col)
 
     stats_df = df.pipe(
         get_stats,
         stats_cols=stat_col, 
         group_by_col=group_by_col, 
         percentiles=percentiles
     )
     
 
-    stats_df['50%'].plot(label=label)
+    stats_df['50%'].plot(label='50%')
     
     for i in range(len(percentiles)):
         plt.fill_between(
             # TODO enable changing alpha and label
             med.index, perc_l[i], perc_h[i], color=color, alpha=0.2, label=f"{100*(1-percentiles[i])}th")
-    plt.title('Trend of {} for the percentiles: {} as well as {}'.format(stat_col,
+    if not label:
+        label = 'Trend of {} for the percentiles: {} as well as {}'.format(stat_col,
                                                                          ', '.join(
                                                                              [str(int(i*100)) for i in percentiles]),
-                                                                         ', '.join([str(int((1-i)*100)) for i in percentiles])))
+                                                                         ', '.join([str(int((1-i)*100)) for i in percentiles]))
+    plt.title(label)
     plt.xlabel(group_by_col)
     plt.ylabel(stat_col)
 
+def plot_sleep_trends(df: pd.DataFrame, glbl: str = GLUCOSE_COL, sleep_time_filter_col: str = f'shifted_{_HOUR_COL}', sleep_time_hour: int = 24 - (_default_shift_hours + 2)):
+    # filter sleep glucose data
+    gdf = df[df[sleep_time_filter_col] >= sleep_time_hour]
+    # make new plotting time
+    gdf.loc[:, 'sleep_hours'] = gdf[sleep_time_filter_col]- gdf[sleep_time_filter_col].min()
+    plot_percentiles(df=gdf,
+        stat_col=glbl, group_by_col='sleep_hours', percentiles=[0.01, 0.05], label='Hourly trend of Glucose during Sleep')
+    plt.ylabel('Glucose during sleep')
+    plt.xlabel('Hours of sleep (from 0-8)')
+    end_plot()
+    plot_comparison(df=gdf, glbl=glbl, compare_by=f'shifted_{_DATE_COL}_str', outliers=False,
+        method='box', sort_vals = False, label='Daily trend of Glucose during Sleep')
+    plt.ylabel('Glucose during sleep')
+    plt.xlabel('Day (sleep from evening of this day)')
+    end_plot()
+
+def plot_day_curve(df: pd.DataFrame, d: str, glbl: str = GLUCOSE_COL, tlbl: str = TIMESTAMP_COL, extended=False):
+    """Plots day glucose curve
+
+    :param df: Dataframe containing glucose
+    :param glbl: Name of the glucose column
+    :return:
+    """
+    plot_df = df.loc[d]
+    #plt.axvline(d, color='brown', linestyle='--', alpha=0.5)
+    plt.axhline(plot_df[glbl].mean(), color='red', linestyle='--', alpha=0.5, label='Day Average')
+    plt.axhline(df[glbl].mean(), color='brown', linestyle='--', alpha=0.2, label='Your general Average')
+    plt.axhline(df[glbl].mean() + 2, color='green', linestyle='--', alpha=0.5, label='Recommended range')
+    plt.axhline(df[glbl].mean() - 1, color='green', linestyle='--', alpha=0.5)
+    plt.plot(plot_df[tlbl], plot_df[glbl])
+
+    
+    if extended:
+        # TODO find a cleaner way to do this
+        xt = df.loc[d: (dt.strptime(d, '%Y-%m-%d')+tdel(days=1, hours=7)).strftime('%Y-%m-%d %H')]
+        plt.plot(xt[tlbl], xt[glbl], color='brown', alpha=0.5, label='sleep')
 
 def get_stats(df: pd.DataFrame, stats_cols: Union[List, str], group_by_col: str = None, percentiles: Optional[List[float]] = None):
     """Get descriptive statistics about specific columns of a dataframe.
 
     Args:
         df (pd.DataFrame): the glucose dataframe.
         stats_cols (Union[List[str], str]): the glucose column name, or a column name,
@@ -823,14 +885,20 @@
     """
     if group_by_col:
         return (df
             .groupby(group_by_col)
             [stats_cols]
             .describe(percentiles=percentiles)
         )
+
+
+    #     grouped_df = df.groupby(group_by_col)[stats_cols]
+    #     r= pd.concat([grouped_df.describe(percentiles=percentiles), grouped_df.sum()], axis=1)
+    #     return r.reorder_levels([1, 0], axis=1).sort_index(axis=1, level=[0, 1])
+    # return df[stats_cols].describe(percentiles=percentiles),  df[stats_cols].sum()
     return df[stats_cols].describe(percentiles=percentiles)
     
 def get_percentiles_and_stats(df: pd.DataFrame, percentiles: List[float], stat_col: str, group_by_col: str):
     """Get descriptive statistics about a specific column of a dataframe.
 
     Args:
         percentiles (Optional[List[float]], optional): a list of percentiles to plot 
@@ -839,24 +907,24 @@
         percentiles (List[float]): a list of percentiles to plot (each value between 0 and 1).
         stat_col (str): the glucose column name or a column name to get stats.
         group_by_col (str): the name of the column to group values by. 
 
     Returns:
         Tuple[float]: mean, standard deviation, percentiles, 1-percentiles
     """
-    # TODO replace completely with get_stats
+    # TODO replace completely with get_stats?
     grouped = df.groupby([group_by_col])[stat_col]
     mean = grouped.mean()
     med = grouped.median()
     dev = grouped.std()
     perc_l = [grouped.quantile(q) for q in percentiles]
     perc_h = [grouped.quantile(1-q) for q in percentiles]
-    return mean, dev, med, perc_l, perc_h # FIXME: use dataclass, do we need mean, med?
+    return mean, dev, med, perc_l, perc_h
 
-def plot_comparison(df: pd.DataFrame, glbl: str=GLUCOSE_COL, compare_by: str=_WEEKDAY_COL, outliers: bool=False, label_map: Union[Callable, Dict]=None, method: str='box', sort_vals: bool = False):
+def plot_comparison(df: pd.DataFrame, glbl: str=GLUCOSE_COL, compare_by: str=_WEEKDAY_COL, outliers: bool=False, label_map: Union[Callable, Dict]=None, method: str='box', sort_vals: bool = False, label: Optional[str] = None):
     """
 
     :param df: dataframe containing the values to be compared and the comparison field
     :param glbl: 
     :param compare_by: 
     :param outliers: boolean to show or not show outliers, defaults to False
     :param label_map: 
@@ -873,14 +941,16 @@
             Defaults to False.
         label_map (Union[Callable, Dict], optional): lambda function to map
             the unique values of the compare_by field to some labels. Defaults to None.
         method (str, optional): the method used for comparison. Currently only supports
             box plots as 'box'. Defaults to 'box'.
         sort_vals (bool, optional): wether or not to sort values plotted.
             Defaults to False.
+        label (Optional[str], optional): title of the plot, if None a default will be generated.
+            Defaults to None.
 
     Raises:
         NotImplementedError: if the method used for comparison is not implemented.
     """
     all_vals = df[compare_by].unique()
     if sort_vals: all_vals.sort()
     if method == 'box':
@@ -888,16 +958,17 @@
                     labels=all_vals if label_map is None else [
                         label_map(i) for i in all_vals],
                     showfliers=outliers)
     else:
         raise NotImplementedError(f"Method {method} not implemented for comparison please use one of: 'box'")
     plt.ylabel(f"Trend for {glbl}")
     plt.xlabel(f"{compare_by}")
-    plt.title('Comparing {} by {}. Outliers are {}.'.
-                format(glbl, compare_by, 'shown' if outliers else 'not shown'))
+    if not label:
+        label='Comparing {} by {}. Outliers are {}.'.format(glbl, compare_by, 'shown' if outliers else 'not shown')
+    plt.title(label)
 
 
 def get_response_bounds(df: pd.DataFrame, event_time: pd.Timestamp, pre_pad_min: int = 20, post_pad_min: int = 0, resp_time_min: int = 120, glbl: str = GLUCOSE_COL, t_lbl: str = TIMESTAMP_COL):
     """Finds the boundaries of a glucose response (used for plotting) by:
     - Finding the nearest time with a glucose value, 'g_event_time', to the event time 'event_time'.
     - Setting the start of the glucose bounds to: 'g_event_time - pre_pad_min'
     - Setting the end to: 'g_event_time + resp_time_min + post_pad_min'
@@ -971,23 +1042,23 @@
 def write_glucose(gdf : pd.DataFrame, output_file : str):
     """Writes glucose to a csv file
 
     Args:
         gdf (pd.DataFrame): the glucose dataframe.
         output_file (str): the output file path.
     """
-    # TODO Do we need this? to csv already handled
     logger.info("Writing glucose data to %s", output_file)
     gdf.to_csv(output_file)
 
 """
 Day/Week Metrics
 """
 _summary_cols = [GLUCOSE_COL, _AUC_COL, _DG_COL, _DT_COL, _DGDT_COL]
 
+
 def get_metrics_by_day(gdf : pd.DataFrame, day_col : str =_DATE_COL, percentiles: list = None, summary_cols : list = _summary_cols):
     """
     Get metrics and statistics by day related to specific columns of a dataframe.
 
     Args:
         gdf (pd.DataFrame): the glucose dataframe.
         day_col (str, optional): the day column name. Defaults to _HOUR_COL.
@@ -997,14 +1068,15 @@
             or a list of column names for which to get stats. Defaults to _summary_cols.
 
     Returns:
         pd.Series or pd.DataFrame: descriptive statistics grouped hour
     """
     return get_stats(gdf, stats_cols=summary_cols, percentiles=percentiles, group_by_col=day_col)
 
+
 def get_metrics_by_hour(gdf : pd.DataFrame, hour_col : str =_HOUR_COL, percentiles : Optional[List[float]] = None, summary_cols : Union[List[str], str] = _summary_cols):
     """Get metrics and statistics by hour related to specific columns of a dataframe.
 
     Args:
         gdf (pd.DataFrame): the glucose dataframe.
         hour_col (str, optional): the hour column name. Defaults to _HOUR_COL.
         percentiles (Optional[List[float]], optional): a list of percentiles to plot 
@@ -1013,14 +1085,15 @@
             or a list of column names for which to get stats. Defaults to _summary_cols.
 
     Returns:
         pd.Series or pd.DataFrame: descriptive statistics grouped hour
     """
     return get_stats(gdf, stats_cols=summary_cols, percentiles=percentiles, group_by_col=hour_col)
 
+
 def get_metrics(gdf : pd.DataFrame, percentiles : Optional[List[float]] = None, summary_cols : Union[List[str], str] = _summary_cols, group_by_col: Optional[str] = None):
     """Get metrics and statistics related to specific columns of a dataframe.
 
     Args:
         gdf (pd.DataFrame): the glucose dataframe.
         percentiles (Optional[List[float]], optional): a list of percentiles to plot 
             (each value between 0 and 1). Defaults to None.
@@ -1030,7 +1103,48 @@
             Defaults to None.
 
     Returns:
        pd.Series or pd.DataFrame: descriptive statistics grouped by the given column
     """
     return get_stats(gdf, stats_cols=summary_cols, percentiles=percentiles, group_by_col=group_by_col)
 
+def describe_glucose(df: pd.DataFrame, glucose_col: str = GLUCOSE_COL, timestamp_col: str = TIMESTAMP_COL, default_unit: str = Units.mmolL.value):
+    """Describes the glucose DataFrame by providing a summary with the total number of days, start and end dates,
+    and overall summary statistics of glucose including the unit of measurement.
+
+    Args:
+        df (pd.DataFrame): The glucose dataframe.
+        glucose_col (str): Column name for glucose data.
+        timestamp_col (str): Column name for timestamp data.
+        default_unit (str): Default unit for glucose measurements.
+    """
+    console = Console()
+    # Ensure timestamps are converted to datetime if not already done
+    if not pd.api.types.is_datetime64_any_dtype(df[timestamp_col]):
+        df[timestamp_col] = pd.to_datetime(df[timestamp_col])
+
+    start_date = df[timestamp_col].min()
+    end_date = df[timestamp_col].max()
+    total_days = (end_date - start_date).days + 1
+
+    # Printing the overall summary
+    console.print("[bold magenta]Glucose Data Summary[/bold magenta]")
+    console.print(
+        f"• Total number of days in the data: [bold green]{total_days}[/bold green]\n"
+        f"• Starting at: [bold green]{start_date.strftime('%Y-%m-%d %H:%M')}[/bold green]\n"
+        f"• Ending at: [bold green]{end_date.strftime('%Y-%m-%d %H:%M')}[/bold green]"
+    )
+
+    glucose_stats = get_stats(df, glucose_col)
+    table = Table(title="Glucose Statistics", show_header=True, header_style="bold magenta")
+    table.add_column("Measure", style="dim")
+    table.add_column(f"Value in {default_unit}")
+
+    for stat in ['mean', 'std', 'min', '25%', '50%', '75%', 'max']:
+        value = glucose_stats.get(stat, 'N/A')
+        table.add_row(stat.capitalize(), f"{value:.2f}")
+
+    console.print(table)
+    console.print(f"Columns in the data: [bold yellow]{', '.join(df.columns)}[/bold yellow]")
+    console.print(
+        f"[bold magenta]First rows in the data:[/bold magenta]\n",
+        df[[timestamp_col, glucose_col]].head())
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `glyco-0.0.1rc1/src/glyco/meals.py` & `glyco-0.0.1rc2/src/glyco/meals.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,19 +5,29 @@
 from datetime import timedelta as tdel
 from datetime import datetime as dt
 import pandas as pd
 from matplotlib import pyplot as plt
 
 from typing import Callable, Iterable, Optional
 
-from glyco.glucose import _AUC_COL, _AUCLIM_COL, _AUCMIN_MIN, DEFAULT_INPUT_TSP_FMT, general_date_type, add_time_values
-from .utils import find_nearest
-
-from .constants import GLUCOSE_COL, TIMESTAMP_COL
+from glyco.glucose import (
+    GLUCOSE_COL,
+    TIMESTAMP_COL,
+    _AUC_COL,
+    _AUCLIM_COL,
+    _AUCMIN_MIN,
+    DEFAULT_INPUT_TSP_FMT,
+    general_date_type,
+    add_time_values,
+    error_not_implemented_method
+)
+from glyco.utils import find_nearest
 
+import logging
+logger = logging.getLogger(__name__)
 
 _event_note_col = 'event_notes'
 _event_ref_col = 'event_reference'
 _freestyle_rec_type_col = "Record Type"
 _freestyle_notes_rec_type = 6
 _freestyle_glucose_rec_type = 0
 _optional_cols = [_event_note_col, _event_ref_col]
@@ -105,15 +115,14 @@
                     ref_col: str = _event_ref_col, 
                     note_col: str = None, 
                     timestamp_fmt : str = DEFAULT_INPUT_TSP_FMT, 
                     timestamp_is_formatted: bool = False, 
                     delimiter: str = ",",
                     skiprows: int = 0
                     ):
-    # TODO NEXT finish
     df = pd.read_csv(
         filepath_or_buffer=file_path,
         delimiter=delimiter,
         skiprows=skiprows
     )
     df = read_events_df(
         edf=df, 
@@ -134,15 +143,16 @@
     
 
 
 
 """Freestyle Libre Specific
 """
 def infer_events_from_notes(df, filter_notes_map: Callable = None):
-    """
+    """Assume the notes column is referring to events and use those instead
+
     filter_notes_map example: `lambda x: False if not x else str(x).startswith('food')`
     """
     events_df = df[df[_freestyle_rec_type_col]==_freestyle_notes_rec_type]
     if filter_notes_map:
         events_df = events_df[events_df[_event_note_col].map(filter_notes_map)]
     return events_df
 
@@ -249,140 +259,142 @@
         ).assign(
             estimated_len = lambda x: (x[estimated_end]-x[estimated_start]).dt.total_seconds()
         )
         .set_index(event_tsp, drop=False)
     )
     return edf
 
-def sessionize_events(events_df: pd.DataFrame, gdf: pd.DataFrame, event_timestamp: str = _original_timestamp, session_seconds: int = _default_event_session_seconds):    
-    """DEPRECATED
-    TODO REMOVE 
-    TODO takes very long to run
-    FIXME OPTIMISE takes too long
-    """
-    edf = events_df.sort_values(event_timestamp)
-    edf[_next_event]= edf[event_timestamp].diff().dt.total_seconds()
-    edf[_prev_event]= edf[event_timestamp].diff(-1).dt.total_seconds().map(abs)
-    # TODO change name to is_session_first
-    edf[is_session_first] = (edf[_next_event].isnull()) | (edf[_next_event] > session_seconds)
-    edf[is_session_last] = (edf[_prev_event].isnull()) | (edf[_prev_event] > session_seconds)
-    # TODO ? find end? edf['event_session_end'] = (edf.dt_next_event.notnull()) & (edf.dt_next_event > session_seconds)
-    edf[session_first] = edf[edf[is_session_first]][event_timestamp]
-    edf[session_last] = edf[edf[is_session_last]][event_timestamp]
-    edf[session_id] = edf[edf[is_session_first]][event_timestamp].rank(method='first').astype(int)
-    edf[session_id] = edf[session_id].fillna(method='ffill').astype(int)
-
-    # define 10 minutes delta
-    delta = 10 * 60
-    jump = session_seconds + delta
-    edf[estimated_start] = edf[session_first].map(lambda x: x if not type(x)==pd.Timestamp else find_nearest(gdf, x - tdel(seconds=delta), TIMESTAMP_COL)) # TODO replace with search start method
-    # FIXME error here NaT needs to be filled
-    edf[estimated_end] = edf[session_last].map(lambda x: x if not type(x)==pd.Timestamp else find_nearest(gdf, x + tdel(seconds=jump), TIMESTAMP_COL)) # TODO replace with search end method
+# Commented in case some of the logic is needed
+# def sessionize_events(events_df: pd.DataFrame, gdf: pd.DataFrame, event_timestamp: str = _original_timestamp, session_seconds: int = _default_event_session_seconds):    
+#     """DEPRECATED
+#     TODO REMOVE 
+#     TODO takes very long to run
+#     FIXME OPTIMISE takes too long
+#     """
+#     edf = events_df.sort_values(event_timestamp)
+#     edf[_next_event]= edf[event_timestamp].diff().dt.total_seconds()
+#     edf[_prev_event]= edf[event_timestamp].diff(-1).dt.total_seconds().map(abs)
+#     # TODO change name to is_session_first
+#     edf[is_session_first] = (edf[_next_event].isnull()) | (edf[_next_event] > session_seconds)
+#     edf[is_session_last] = (edf[_prev_event].isnull()) | (edf[_prev_event] > session_seconds)
+#     # TODO ? find end? edf['event_session_end'] = (edf.dt_next_event.notnull()) & (edf.dt_next_event > session_seconds)
+#     edf[session_first] = edf[edf[is_session_first]][event_timestamp]
+#     edf[session_last] = edf[edf[is_session_last]][event_timestamp]
+#     edf[session_id] = edf[edf[is_session_first]][event_timestamp].rank(method='first').astype(int)
+#     edf[session_id] = edf[session_id].fillna(method='ffill').astype(int)
+
+#     # define 10 minutes delta
+#     delta = 10 * 60
+#     jump = session_seconds + delta
+#     edf[estimated_start] = edf[session_first].map(lambda x: x if not type(x)==pd.Timestamp else find_nearest(gdf, x - tdel(seconds=delta), TIMESTAMP_COL)) # TODO replace with search start method
+#     # FIXME error here NaT needs to be filled
+#     edf[estimated_end] = edf[session_last].map(lambda x: x if not type(x)==pd.Timestamp else find_nearest(gdf, x + tdel(seconds=jump), TIMESTAMP_COL)) # TODO replace with search end method
     
 
 
-    # Fill empty fields
-    edf[session_first] = edf[session_first].fillna(method='ffill')
-    edf[estimated_start] = edf[estimated_start].fillna(method='ffill')
-    edf[session_last] = edf[session_last].fillna(method='bfill')
-    edf[estimated_end] = edf[estimated_end].fillna(method='bfill')
-    edf[session_len] = session_seconds
+#     # Fill empty fields
+#     edf[session_first] = edf[session_first].fillna(method='ffill')
+#     edf[estimated_start] = edf[estimated_start].fillna(method='ffill')
+#     edf[session_last] = edf[session_last].fillna(method='bfill')
+#     edf[estimated_end] = edf[estimated_end].fillna(method='bfill')
+#     edf[session_len] = session_seconds
     
-    # TODO is it better to resort by index
-    edf.sort_index()
-    return edf
+#     # TODO is it better to resort by index
+#     edf.sort_index()
+#     return edf
 
 # TODO get events automatically
 def get_events_infer(gdf: pd.DataFrame, limit: float = None):
-    events = None
-    return events
+    """Not implemented"""
+    raise NotImplementedError(error_not_implemented_method)
 
 # TODO this is freestyle libre specific
 def get_events_from_fs_notes(gdf: pd.DataFrame, edf: pd.DataFrame):
-    events = None
-    return events
+    """Not implemented"""
+    raise NotImplementedError(error_not_implemented_method)
 
 def get_events_from_df(gdf: pd.DataFrame, edf: pd.DataFrame):
-    events = None
-    return events
+    """Not implemented"""
+    raise NotImplementedError(error_not_implemented_method)
 
 def get_events_from_times(gdf: pd.DataFrame, event_times: Iterable):
-    events = None
-    return events
+    """Not implemented"""
+    raise NotImplementedError(error_not_implemented_method)
 
 def get_event_metrics(gdf, edf, eid):
-    metrics = None
-    return metrics
+    """Not implemented"""
+    raise NotImplementedError(error_not_implemented_method)
 
 def describe_event(gdf, edf, eid):
-    metrics = None
-    return metrics
+    """Not implemented"""
+    raise NotImplementedError(error_not_implemented_method)
 
 
 
 """Plotting
 
 TODO: 
 * add plotting multiple sessions
 * add comparing meals
 """
 def plot_compare_sessions():
-    # TODO
-    pass
+    """Not implemented"""
+    raise NotImplementedError(error_not_implemented_method)
 
 def plot_day_sessions():
-    # TODO
-    pass
+    """Not implemented"""
+    raise NotImplementedError(error_not_implemented_method)
 
 def plot_all_sessions():
-    # TODO plot day with sessions
-    pass
+    """Not implemented"""
+    raise NotImplementedError(error_not_implemented_method)
 
-def plot_session_response(glucose_df: pd.DataFrame, sessions_df: pd.DataFrame, session_id: int, session_title: Optional[str]=None, use_notes_as_title: str=False, notes_col: str='Notes', show_events: bool=False, glbl: str=GLUCOSE_COL, show_auc=True):
+def plot_session_response(glucose_df: pd.DataFrame, sessions_df: pd.DataFrame, session_id: int, use_notes_as_title: str=False, session_title: Optional[str]=None, notes_col: str='Notes', show_events: bool=False, events_tsp: str = TIMESTAMP_COL, glbl: str=GLUCOSE_COL, show_auc=True):
     """Plots the glucose response during one specific event session given by its session id.
 
     Args:
         glucose_df (_type_): 
         sessions_df (_type_): 
         session_id (_type_): the id of the session to plot
 
     Args:
         glucose_df (pd.DataFrame): the glucose dataframe.
         sessions_df (pd.DataFrame): the event sessions dataframe.
         session_id (int): the id of the session to plot.
-        session_title (Optional[str], optional): the title of the session used in the plot.
-            Overriden by 'use_notes_as_title'. Defaults to None.
         use_notes_as_title (str, optional): whether or not to use the Notes column for the event title.
             Overrides 'session_title'. Defaults to False.
+        session_title (Optional[str], optional): the title of the session used in the plot.
+            Overriden by 'use_notes_as_title'. Defaults to None.
         notes_col (str, optional): the name of the notes column, only used in combination with 'use_notes_as_title'.
             Defaults to 'Notes'.
         show_events (bool, optional): whether or not to show each specific event in the event session.
             Defaults to False.
+        events_tsp (str, optional): timestamp column for event sessions, only used for showing events.
         glbl (str, optional): the glucose column name in the glucose dataframe. Defaults to GLUCOSE_COL.
         show_auc (bool, optional): whether or not to show the area under the curve in the plot. Defaults to True.
     """
     session = sessions_df[sessions_df['session_id']==session_id]
     start = session.iloc[-1]['estimated_start']
     end = session.iloc[-1]['estimated_end'] # TODO move to get_session_bounds
     # TODO add Notes capability
     truncated_glucose = glucose_df[start:end][glbl]
     plt.plot(truncated_glucose)
     if show_auc:
-        plot_auc_above_threshold(truncated_glucose, truncated_glucose.mean())
+        _plot_auc_above_threshold(truncated_glucose, truncated_glucose.mean())
 
     plt.axvline(session.iloc[-1]['session_first'], color='red', label='First event', linestyle='--', alpha=0.1)
     if use_notes_as_title:
-        session_title = f"Session with the events: ({'; '.join([x for x in session[notes_col]])})"
+        session_title = f"Session with the events: ({'; '.join([x for x in session[notes_col] if x and isinstance(x, str)])})"
     if session_title:
         plt.title(session_title)
     if show_events:
-        [plt.axvline(session.iloc[i]['t'], color='black', linestyle='--', alpha=0.1) for i in range(len(session))]
+        [plt.axvline(session.iloc[i][events_tsp], color='black', linestyle='--', alpha=0.1) for i in range(len(session))]
     plt.xticks(rotation=45)
 
-def plot_auc_above_threshold(values: Iterable, threshold: float):
+def _plot_auc_above_threshold(values: Iterable, threshold: float):
     """Plot area under the curve between some values and a specific threshold.
 
     Args:
         values (_type_): values under which to plot the area under the curve (in Y-axis).
         threshold (_type_): threshold above which to plot the area under the curve (in Y-axis).
     """
     lim_df = values.map(lambda x: x if x>threshold else threshold)
@@ -411,24 +423,24 @@
     g_events = gdf[gdf[g_col]>lim][[g_col, tsp_col]]
     e_sessions = get_event_sessions(
         events_df = g_events, 
         glucose_df = gdf, 
         event_tsp=tsp_col, 
         session_seconds=60*60
         )
-    # TODO select only some of the events instead of keeping all?
+    # TODO select only some of the events instead of keeping all of them?
     meal_events = e_sessions
     return meal_events
 
 
 """Event metrics
 """
 def get_event_metrics(gdf, start, end):
-    stats = None
-    return stats
+    """Not implemented"""
+    raise NotImplementedError(error_not_implemented_method)
 
 
 def get_event_auc(gdf: pd.DataFrame, start: general_date_type, end: general_date_type):
     """Get Area under the curve values for a time range.
 
     Args:
         gdf (pd.DataFrame): the glucose dataframe.
```

### Comparing `glyco-0.0.1rc1/src/glyco/utils.py` & `glyco-0.0.1rc2/src/glyco/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 class Units(enum.Enum):
     """Enum for supported glucose units
     Glyco mainly uses mmol/L but performs conversion if the unit is different.
     """
     mmolL = "mmol/L"
     mgdL = "mg/dL"
-    gL = "g/L" # TODO handle more units
+    gL = "g/L"
 
 
 # Will be used to convert glucose to mmol/L (Glucose in mmol/L = units_to_mmolL_factor[input unit] * Glucose in input unit)
 units_to_mmolL_factor = {
     Units.mmolL.value: 1,
     Units.mgdL.value: 1/18.0182,
     Units.gL.value: 100/18.0182
@@ -55,15 +55,14 @@
 
     Args:
         df (pd.DataFrame): dataframe to search in
         pivot (pd.Timestamp): timestamp to search for
         col (str): column of the dataframe to search in
         n_iter (int, optional): number of iterations before saying there is nothing. Defaults to 100.
     """
-    # TODO add prioritise smaller or larger value
     items = list(df.index)
     n = items.copy()
     for i in range(n_iter):
         m = min(n, key=lambda x: abs(x - pivot))
         q = df.loc[m][col]
         if type(q) == pd.Series:
             q = q[0]
```

### Comparing `glyco-0.0.1rc1/src/glyco.egg-info/PKG-INFO` & `glyco-0.0.1rc2/src/glyco.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glyco
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: Read and analyse continuous glucose monitoring data
 Author-email: Ismail Elouafiq <contact@ismail.bio>
 License: MIT License
         
         Copyright (c) [2022] [Ismail Elouafiq]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,15 +33,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: matplotlib-inline
 Requires-Dist: rich
 Requires-Dist: seaborn
@@ -130,14 +129,26 @@
     ```Python
     # you can provide a list or dataframe that contains the event times
     events = gl.get_events(event_times)
     ```
     You can even get the events from a folder of pictures. More on this in the [meals and events documentation](https://github.com/nidhog/glyco/blob/main/docs/concepts/events_and_meals.md)).
 3. **Advanced analysis of events**, including metrics for meals or events and how they impact glucose. As well as ranking meals and more, to further aid in understanding the glucose data.
 
+4. **On Privacy and Personally Identifieable Information** *Glyco also enables making the glucose data more private by hiding sensitive information*
+    ```Python
+    # you can set the 'mask_private_info' to true
+    anonymised_df = gl.read_csv(
+        file_path='my_glucose_data.csv',
+        mask_private_info=True
+        )
+    ```
+    The mask_private_info masks private information by: resetting the minimum datetime, removing specific columns (such as the device serial number), replacing categorical columns using a hash function and adding noise to the glucose data.
+
+    More details on how to use the privacy feature in [the privacy documentation here](https://github.com/nidhog/glyco/blob/main/docs/extra/privacy.md).
+
 ## Limitations
 * The metric calculations for days assumes the device timezone is the user's timezone.
 
 > ***Disclaimer*** Glyco is not a medical product and shall not be used to diagnose, treat or evaluate any medical conditions.
 For more on the intended use and indications of use please read the [healthcare considerations document](https://github.com/nidhog/glyco/blob/main/docs/extra/healthcare.md).
 
 ## Built on the shoulders of giants
```

