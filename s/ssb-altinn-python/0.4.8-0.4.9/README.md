# Comparing `tmp/ssb_altinn_python-0.4.8.tar.gz` & `tmp/ssb_altinn_python-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_altinn_python-0.4.8.tar", max compression
+gzip compressed data, was "ssb_altinn_python-0.4.9.tar", max compression
```

## Comparing `ssb_altinn_python-0.4.8.tar` & `ssb_altinn_python-0.4.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2024-04-11 08:17:12.838420 ssb_altinn_python-0.4.8/LICENSE
--rw-r--r--   0        0        0     9093 2024-04-11 08:17:12.838420 ssb_altinn_python-0.4.8/README.md
--rw-r--r--   0        0        0     4352 2024-04-11 08:17:22.990492 ssb_altinn_python-0.4.8/pyproject.toml
--rw-r--r--   0        0        0      325 2024-04-11 08:17:12.842420 ssb_altinn_python-0.4.8/src/altinn/__init__.py
--rw-r--r--   0        0        0      198 2024-04-11 08:17:12.842420 ssb_altinn_python-0.4.8/src/altinn/__main__.py
--rw-r--r--   0        0        0     2207 2024-04-11 08:17:12.842420 ssb_altinn_python-0.4.8/src/altinn/file.py
--rw-r--r--   0        0        0    12654 2024-04-11 08:17:12.842420 ssb_altinn_python-0.4.8/src/altinn/flatten.py
--rw-r--r--   0        0        0     4245 2024-04-11 08:17:12.842420 ssb_altinn_python-0.4.8/src/altinn/parser.py
--rw-r--r--   0        0        0        0 2024-04-11 08:17:12.842420 ssb_altinn_python-0.4.8/src/altinn/py.typed
--rw-r--r--   0        0        0     1378 2024-04-11 08:17:12.842420 ssb_altinn_python-0.4.8/src/altinn/utils.py
--rw-r--r--   0        0        0    10170 1970-01-01 00:00:00.000000 ssb_altinn_python-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-22 10:14:12.452719 ssb_altinn_python-0.4.9/LICENSE
+-rw-r--r--   0        0        0    10533 2024-04-22 10:14:12.452719 ssb_altinn_python-0.4.9/README.md
+-rw-r--r--   0        0        0     4352 2024-04-22 10:14:24.048654 ssb_altinn_python-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0      325 2024-04-22 10:14:12.456719 ssb_altinn_python-0.4.9/src/altinn/__init__.py
+-rw-r--r--   0        0        0      198 2024-04-22 10:14:12.456719 ssb_altinn_python-0.4.9/src/altinn/__main__.py
+-rw-r--r--   0        0        0     2207 2024-04-22 10:14:12.456719 ssb_altinn_python-0.4.9/src/altinn/file.py
+-rw-r--r--   0        0        0    14593 2024-04-22 10:14:12.456719 ssb_altinn_python-0.4.9/src/altinn/flatten.py
+-rw-r--r--   0        0        0     4245 2024-04-22 10:14:12.456719 ssb_altinn_python-0.4.9/src/altinn/parser.py
+-rw-r--r--   0        0        0        0 2024-04-22 10:14:12.456719 ssb_altinn_python-0.4.9/src/altinn/py.typed
+-rw-r--r--   0        0        0     1663 2024-04-22 10:14:12.456719 ssb_altinn_python-0.4.9/src/altinn/utils.py
+-rw-r--r--   0        0        0    11610 1970-01-01 00:00:00.000000 ssb_altinn_python-0.4.9/PKG-INFO
```

### Comparing `ssb_altinn_python-0.4.8/LICENSE` & `ssb_altinn_python-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.4.8/README.md` & `ssb_altinn_python-0.4.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -37,28 +37,30 @@
 from altinn import isee_transform
 
 file = "gs://ssb-prod-dapla-felles-data-delt/altinn3/RA-0595/2023/2/6/810409282_460784f978a2_ebc7af7e-4ebe-4883-b844-66ee6292a93a/form_460784f978a2.xml"
 
 isee_transform(file)
 ```
 
+#### Mapping the FELTNAVN-column
 If you want to recode/map names in the FELTNAVN-column, you can use a dictionary with the original names from the xml as keys, and the new names as values. And then pass the dictionary as an argument when running the function isee_transform(file, mapping).
 
 ```python
 from altinn import isee_transform
 
 file = "gs://ssb-prod-dapla-felles-data-delt/altinn3/RA-0595/2023/2/6/810409282_460784f978a2_ebc7af7e-4ebe-4883-b844-66ee6292a93a/form_460784f978a2.xml"
 
 mapping = {'kontAmbulForeDispJaNei':'ISEE_VAR1',
            'kontAmbulForeDispAnt':'ISEE_VAR2',
            'kontAmbulForeDriftAnt':'ISEE_VAR3',}
 
 isee_transform(file, mapping)
 ```
 
+#### Flatten more tags than SkjemaData
 If you need to flatten more than 'SkjemaData' from the XML, you can make a list of the tags in the XML you need to flatten, and add this list as an argument (tag_list) when running the function isee_transform(file, taglist=taglist). The default value is 'SkjemaData', so if you only need to flatten this, its not needed to pass the argument tag_list.
 
 ```python
 from altinn import isee_transform
 
 file = "gs://ssb-prod-dapla-felles-data-delt/altinn3/RA-0595/2023/2/6/810409282_460784f978a2_ebc7af7e-4ebe-4883-b844-66ee6292a93a/form_460784f978a2.xml"
 
@@ -68,15 +70,41 @@
            'kontaktPersonNavn'; 'ISEE_KONTAKTPERSON',}
 
 tags = ['SkjemaData', 'Kontakt']
 
 isee_transform(file, mapping, tag_list=tags)
 ```
 
+#### Flatten checkboxes
+Altinn 3 checkboxes comes as a string value seperated by ",". To get this into oracle, the value must be extracted and pivoted to unique rows. Listing variables from altinn 3 xml file that are checkboxes in checkbox_vars will make each value to a unique row.
+Checkboxes can use unique codes from KLASS or be 1:N. If your checkbox codes are unique, you should also set unique_code to True.
+When we then transform the xml file to isee format, we will end up with more variables than we begun with. This extra potential variables must then be included in the mapping so they have the right name when loaded into oracle.
+
+```python
+
+from altinn import isee_transform
+
+file = 'gs://ra0187-01-altinn-data-staging-c629-ssb-altinn/2024/4/11/7d5b52259b89_de4a24aa-4948-48d8-b2e4-a0f2160a0bd0/form_7d5b52259b89.xml'
+
+mapping = {
+    "storOkningOmsAarsak31":"ISEE_storOkningOmsAarsak31",
+    "storOkningOmsAarsak33":"ISEE_storOkningOmsAarsak33",
+    "omsForrigePerPrefill":"ISEE_omsForrigePerPrefill",
+}
+
+checkboxList = ["storOkningOmsAarsak"]
+
+isee_transform(file=file,mapping=mapping,checkbox_vars=checkboxList,unique_code=False)
+
+```
+
+
 The function handles flat structures and 'tables' in the XML. If the XML contains repeating values, it puts a suffix containig a number at the end of the FELTNAVN-column. If the XML-contains more complex structures as 'table in table' if will give a warning with a list of which values in FELTNAVN that needs to be further processed before it can be used in ISEE.
+These warnings will not be visible in 'Kildomaten' unless you check the logs, so it's recommended to test outside of 'Kildomaten' before ypu put it in production.
+
 
 The XML needs to contain certain fields in the 'InternInfo'-block, The required filds are:
 - 'enhetsIdent'
 - 'enhetsType'
 - 'delregNr'
 
 If one or more of these fields are missing in the XML, the processing will stop, giving a message with witch fields that are missing.
@@ -151,15 +179,15 @@
 # Check if xml-file is valid. Useful to inspect xml-files with formal errors in the xml-schema.
 form.validate()
 # Returns True og False
 ```
 
 ### Parse xml-file
 
-If you want to transform an Altinn3 xml-file to a Pandas Dataframe, you can use the ParseSingleXml-class.
+If you want to transform an Altinn3 xml-file to a Pandas Dataframe, you can use the ParseSingleXml-class. This will not handle complex structures of the XML.
 
 ```python
 from altinn import ParseSingleXml
 
 file = "gs://ssb-prod-dapla-felles-data-delt/altinn3/RA-0595/2023/2/6/810409282_460784f978a2_ebc7af7e-4ebe-4883-b844-66ee6292a93a/form_460784f978a2.xml"
 
 form_content=ParseSingleXml(file)
```

### Comparing `ssb_altinn_python-0.4.8/pyproject.toml` & `ssb_altinn_python-0.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-altinn-python"
-version = "0.4.8"
+version = "0.4.9"
 description = "SSB Altinn Python"
 authors = ["Vidar Strandseter <vidar.strandseter@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/ssb-altinn-python"
 repository = "https://github.com/statisticsnorway/ssb-altinn-python"
 documentation = "https://statisticsnorway.github.io/ssb-altinn-python"
```

### Comparing `ssb_altinn_python-0.4.8/src/altinn/file.py` & `ssb_altinn_python-0.4.9/src/altinn/file.py`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.4.8/src/altinn/flatten.py` & `ssb_altinn_python-0.4.9/src/altinn/flatten.py`

 * *Files 14% similar despite different names*

```diff
@@ -225,18 +225,69 @@
             df.at[index, "FELTNAVN"] += "_" + last_counter_value.zfill(3)
 
     df = df.drop(["COUNTER", "LEVELS"], axis=1)
 
     return df
 
 
+def _transform_checkbox_var(
+    df: pd.DataFrame,
+    checkbox_var: str,
+    unique_code: bool = False,
+    new_value: str = "1",
+) -> pd.DataFrame:
+    """transform_dict_code_vars.
+
+    Transform a dictionary by removing a key and using its value as a new key with a new value.
+
+    Args:
+        df: The DataFrame to be transformed.
+        checkbox_var: The value to remove from the DataFrame and flatten into seperate rows.
+        unique_code: Bool for if you are using unique codes from Klass or not.
+        new_value: Optional new value to add, default is 1 as str.
+
+    Returns:
+        df: The transformed DataFrame.
+    """
+    if checkbox_var in df["FELTNAVN"].values:
+
+        checkbox_df = df[df["FELTNAVN"] == checkbox_var].copy()
+
+        df = df[df["FELTNAVN"] != checkbox_var]
+
+        for _, row in checkbox_df.iterrows():
+
+            value = row["FELTVERDI"]
+            values = utils._split_string(value)
+
+            for value in values:
+
+                new_row = row.copy()
+
+                if unique_code is False:
+                    new_row["FELTNAVN"] = checkbox_var + value
+                    new_row["FELTVERDI"] = new_value
+                else:
+                    new_row["FELTNAVN"] = value
+                    new_row["FELTVERDI"] = new_value
+
+                df = pd.concat(
+                    [df, pd.DataFrame([new_row]).reset_index(drop=True)],
+                    ignore_index=True,
+                )
+
+    return df
+
+
 def isee_transform(
     file_path: str,
     mapping: dict[str, str] | None = None,
     tag_list: list[str] | None = None,
+    checkbox_vars: list[str] | None = None,
+    unique_code: bool = False,
 ) -> pd.DataFrame:
     """Transforms a XML to ISEE-format using xmltodict.
 
     Transforms the XML to ISEE-format by using xmltodict to transform the XML
     to a dictionary. Traverses/scans the key/values in dictionary for lists,
     dicts and simple values.
     Stores the results in a list of dictionaries, that converts to a DataFrame
@@ -244,14 +295,16 @@
     Args:
         file_path: The path to the XML file.
         mapping: The mapping dictionary to map variable names in the
             'feltnavn' column. The default value is an empty dictionary
             (if mapping is not needed).
         tag_list: A list containing the tags in the XML that will be flatten
             The default value is ['SkjemaData']
+        checkbox_vars: Optional list of str for elements from xml containing KLASS codes.
+        unique_code: Bool for if you are using unique codes from Klass or not.
 
     Returns:
         pandas.DataFrame: A transformed DataFrame which aligns with the
         ISEE dynarev format.
 
     Raises:
         ValueError: If invalid gcs-file or xml-file.
@@ -298,14 +351,20 @@
                 r"£.*?\$", "", regex=True
             )
 
             final_df["FELTVERDI"] = final_df["FELTVERDI"].str.replace("\n", " ")
 
             final_df["LEVELS"] = final_df.apply(_create_levels_col, axis=1)
 
+            if checkbox_vars is not None:
+                for checkbox_var in checkbox_vars:
+                    final_df = _transform_checkbox_var(
+                        final_df, checkbox_var, unique_code
+                    )
+
             if mapping is not None:
                 final_df["FELTNAVN"] = final_df["FELTNAVN"].replace(mapping)
 
             final_df = _add_lopenr(final_df)
 
             columns_order = [
                 "SKJEMA_ID",
```

### Comparing `ssb_altinn_python-0.4.8/src/altinn/parser.py` & `ssb_altinn_python-0.4.9/src/altinn/parser.py`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.4.8/src/altinn/utils.py` & `ssb_altinn_python-0.4.9/src/altinn/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -42,7 +42,19 @@
             expanded_path = os.path.expanduser(file_path)
             with open(expanded_path) as file:
                 # Read and parse the local file
                 parseString(file.read())
                 return True
         except (ParseError, OSError):
             return False
+
+
+def _split_string(input_string: str) -> list[str]:
+    """Split a string into a list of strings using ',' as the separator.
+
+    Args:
+        input_string: The input string to be split.
+
+    Returns:
+        list: A list of split strings.
+    """
+    return input_string.split(",")
```

### Comparing `ssb_altinn_python-0.4.8/PKG-INFO` & `ssb_altinn_python-0.4.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-altinn-python
-Version: 0.4.8
+Version: 0.4.9
 Summary: SSB Altinn Python
 Home-page: https://github.com/statisticsnorway/ssb-altinn-python
 License: MIT
 Author: Vidar Strandseter
 Author-email: vidar.strandseter@ssb.no
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -63,28 +63,30 @@
 from altinn import isee_transform
 
 file = "gs://ssb-prod-dapla-felles-data-delt/altinn3/RA-0595/2023/2/6/810409282_460784f978a2_ebc7af7e-4ebe-4883-b844-66ee6292a93a/form_460784f978a2.xml"
 
 isee_transform(file)
 ```
 
+#### Mapping the FELTNAVN-column
 If you want to recode/map names in the FELTNAVN-column, you can use a dictionary with the original names from the xml as keys, and the new names as values. And then pass the dictionary as an argument when running the function isee_transform(file, mapping).
 
 ```python
 from altinn import isee_transform
 
 file = "gs://ssb-prod-dapla-felles-data-delt/altinn3/RA-0595/2023/2/6/810409282_460784f978a2_ebc7af7e-4ebe-4883-b844-66ee6292a93a/form_460784f978a2.xml"
 
 mapping = {'kontAmbulForeDispJaNei':'ISEE_VAR1',
            'kontAmbulForeDispAnt':'ISEE_VAR2',
            'kontAmbulForeDriftAnt':'ISEE_VAR3',}
 
 isee_transform(file, mapping)
 ```
 
+#### Flatten more tags than SkjemaData
 If you need to flatten more than 'SkjemaData' from the XML, you can make a list of the tags in the XML you need to flatten, and add this list as an argument (tag_list) when running the function isee_transform(file, taglist=taglist). The default value is 'SkjemaData', so if you only need to flatten this, its not needed to pass the argument tag_list.
 
 ```python
 from altinn import isee_transform
 
 file = "gs://ssb-prod-dapla-felles-data-delt/altinn3/RA-0595/2023/2/6/810409282_460784f978a2_ebc7af7e-4ebe-4883-b844-66ee6292a93a/form_460784f978a2.xml"
 
@@ -94,15 +96,41 @@
            'kontaktPersonNavn'; 'ISEE_KONTAKTPERSON',}
 
 tags = ['SkjemaData', 'Kontakt']
 
 isee_transform(file, mapping, tag_list=tags)
 ```
 
+#### Flatten checkboxes
+Altinn 3 checkboxes comes as a string value seperated by ",". To get this into oracle, the value must be extracted and pivoted to unique rows. Listing variables from altinn 3 xml file that are checkboxes in checkbox_vars will make each value to a unique row.
+Checkboxes can use unique codes from KLASS or be 1:N. If your checkbox codes are unique, you should also set unique_code to True.
+When we then transform the xml file to isee format, we will end up with more variables than we begun with. This extra potential variables must then be included in the mapping so they have the right name when loaded into oracle.
+
+```python
+
+from altinn import isee_transform
+
+file = 'gs://ra0187-01-altinn-data-staging-c629-ssb-altinn/2024/4/11/7d5b52259b89_de4a24aa-4948-48d8-b2e4-a0f2160a0bd0/form_7d5b52259b89.xml'
+
+mapping = {
+    "storOkningOmsAarsak31":"ISEE_storOkningOmsAarsak31",
+    "storOkningOmsAarsak33":"ISEE_storOkningOmsAarsak33",
+    "omsForrigePerPrefill":"ISEE_omsForrigePerPrefill",
+}
+
+checkboxList = ["storOkningOmsAarsak"]
+
+isee_transform(file=file,mapping=mapping,checkbox_vars=checkboxList,unique_code=False)
+
+```
+
+
 The function handles flat structures and 'tables' in the XML. If the XML contains repeating values, it puts a suffix containig a number at the end of the FELTNAVN-column. If the XML-contains more complex structures as 'table in table' if will give a warning with a list of which values in FELTNAVN that needs to be further processed before it can be used in ISEE.
+These warnings will not be visible in 'Kildomaten' unless you check the logs, so it's recommended to test outside of 'Kildomaten' before ypu put it in production.
+
 
 The XML needs to contain certain fields in the 'InternInfo'-block, The required filds are:
 - 'enhetsIdent'
 - 'enhetsType'
 - 'delregNr'
 
 If one or more of these fields are missing in the XML, the processing will stop, giving a message with witch fields that are missing.
@@ -177,15 +205,15 @@
 # Check if xml-file is valid. Useful to inspect xml-files with formal errors in the xml-schema.
 form.validate()
 # Returns True og False
 ```
 
 ### Parse xml-file
 
-If you want to transform an Altinn3 xml-file to a Pandas Dataframe, you can use the ParseSingleXml-class.
+If you want to transform an Altinn3 xml-file to a Pandas Dataframe, you can use the ParseSingleXml-class. This will not handle complex structures of the XML.
 
 ```python
 from altinn import ParseSingleXml
 
 file = "gs://ssb-prod-dapla-felles-data-delt/altinn3/RA-0595/2023/2/6/810409282_460784f978a2_ebc7af7e-4ebe-4883-b844-66ee6292a93a/form_460784f978a2.xml"
 
 form_content=ParseSingleXml(file)
```

