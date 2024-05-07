# Comparing `tmp/climatePy-0.5.0.tar.gz` & `tmp/climatePy-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climatePy-0.5.0.tar", last modified: Mon Feb 12 23:33:03 2024, max compression
+gzip compressed data, was "climatePy-0.5.1.tar", last modified: Tue May  7 20:23:40 2024, max compression
```

## Comparing `climatePy-0.5.0.tar` & `climatePy-0.5.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 23:33:03.257684 climatePy-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34867 2024-02-12 23:33:01.000000 climatePy-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-02-12 23:33:03.257684 climatePy-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-02-12 23:33:01.000000 climatePy-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 23:33:03.257684 climatePy-0.5.0/climatePy/
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-02-12 23:33:01.000000 climatePy-0.5.0/climatePy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30688 2024-02-12 23:33:01.000000 climatePy-0.5.0/climatePy/_climatepy_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)   106156 2024-02-12 23:33:01.000000 climatePy-0.5.0/climatePy/_dap.py
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-02-12 23:33:01.000000 climatePy-0.5.0/climatePy/_extract_sites.py
--rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-02-12 23:33:01.000000 climatePy-0.5.0/climatePy/_netrc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    39496 2024-02-12 23:33:01.000000 climatePy-0.5.0/climatePy/_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (127)    52954 2024-02-12 23:33:01.000000 climatePy-0.5.0/climatePy/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-02-12 23:33:01.000000 climatePy-0.5.0/climatePy/_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 23:33:03.257684 climatePy-0.5.0/climatePy/data/
--rw-r--r--   0 runner    (1001) docker     (127)   954304 2024-02-12 23:33:01.000000 climatePy-0.5.0/climatePy/data/catalog.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 23:33:03.257684 climatePy-0.5.0/climatePy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-02-12 23:33:03.000000 climatePy-0.5.0/climatePy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-12 23:33:03.000000 climatePy-0.5.0/climatePy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 23:33:03.000000 climatePy-0.5.0/climatePy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-12 23:33:03.000000 climatePy-0.5.0/climatePy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-12 23:33:03.000000 climatePy-0.5.0/climatePy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 23:33:03.257684 climatePy-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-02-12 23:33:02.000000 climatePy-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 23:33:03.257684 climatePy-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 23:33:01.000000 climatePy-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-02-12 23:33:01.000000 climatePy-0.5.0/tests/test_climatepy_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10440 2024-02-12 23:33:01.000000 climatePy-0.5.0/tests/test_dap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-02-12 23:33:01.000000 climatePy-0.5.0/tests/test_extract_sites.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-02-12 23:33:01.000000 climatePy-0.5.0/tests/test_netrc.py
--rw-r--r--   0 runner    (1001) docker     (127)    52401 2024-02-12 23:33:01.000000 climatePy-0.5.0/tests/test_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-02-12 23:33:01.000000 climatePy-0.5.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-02-12 23:33:01.000000 climatePy-0.5.0/tests/test_vrt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:23:40.768428 climatePy-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    34867 2024-05-07 20:23:37.000000 climatePy-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-07 20:23:40.768428 climatePy-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-05-07 20:23:37.000000 climatePy-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:23:40.764428 climatePy-0.5.1/climatePy/
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-07 20:23:37.000000 climatePy-0.5.1/climatePy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31227 2024-05-07 20:23:37.000000 climatePy-0.5.1/climatePy/_climatepy_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)   106156 2024-05-07 20:23:37.000000 climatePy-0.5.1/climatePy/_dap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-05-07 20:23:37.000000 climatePy-0.5.1/climatePy/_extract_sites.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-05-07 20:23:37.000000 climatePy-0.5.1/climatePy/_netrc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39496 2024-05-07 20:23:37.000000 climatePy-0.5.1/climatePy/_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52954 2024-05-07 20:23:37.000000 climatePy-0.5.1/climatePy/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-07 20:23:37.000000 climatePy-0.5.1/climatePy/_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:23:40.768428 climatePy-0.5.1/climatePy/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   954304 2024-05-07 20:23:37.000000 climatePy-0.5.1/climatePy/data/catalog.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:23:40.764428 climatePy-0.5.1/climatePy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-07 20:23:40.000000 climatePy-0.5.1/climatePy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-07 20:23:40.000000 climatePy-0.5.1/climatePy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:23:40.000000 climatePy-0.5.1/climatePy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-07 20:23:40.000000 climatePy-0.5.1/climatePy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 20:23:40.000000 climatePy-0.5.1/climatePy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 20:23:40.768428 climatePy-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-07 20:23:39.000000 climatePy-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:23:40.768428 climatePy-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:23:37.000000 climatePy-0.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-05-07 20:23:37.000000 climatePy-0.5.1/tests/test_climatepy_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10440 2024-05-07 20:23:37.000000 climatePy-0.5.1/tests/test_dap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-07 20:23:37.000000 climatePy-0.5.1/tests/test_extract_sites.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-07 20:23:37.000000 climatePy-0.5.1/tests/test_netrc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52354 2024-05-07 20:23:37.000000 climatePy-0.5.1/tests/test_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-07 20:23:37.000000 climatePy-0.5.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-05-07 20:23:37.000000 climatePy-0.5.1/tests/test_vrt.py
```

### Comparing `climatePy-0.5.0/LICENSE` & `climatePy-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `climatePy-0.5.0/PKG-INFO` & `climatePy-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Python package for getting point and gridded climate data by AOI.
 Author: Angus Watters, Mike Johnson
 Author-email: anguswatters@gmail.com, mikecp11@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `climatePy-0.5.0/README.md` & `climatePy-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `climatePy-0.5.0/climatePy/__init__.py` & `climatePy-0.5.1/climatePy/__init__.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.5.0/climatePy/_climatepy_filter.py` & `climatePy-0.5.1/climatePy/_climatepy_filter.py`

 * *Files 3% similar despite different names*

```diff
@@ -206,16 +206,22 @@
         
         # if all elements in varname are in u, filter down to varname
         if all(elem in u for elem in varname):
             catalog = catalog.loc[catalog['varname'].isin(varname) | catalog['variable'].isin(varname)]
         else:
             bad = list(set(varname) - set(u))
             m = catalog[['variable', 'description', 'units']].drop_duplicates()
-            message = f"'{bad}' not avaliable parameter for '{catalog.iloc[0]['id']}'. Try: \n\t{'> ' + m['variable'] + ' [' + m['units'] + '] (' + m['description'] + ')' }"
-            raise Exception(message)
+            suggested_vals = list(zip(m['variable'].tolist(), m['description'].tolist(), m['units'].tolist()))
+            suggested_strs = "\n\t> " +  "\n\t> ".join([f"{i[0]} [{i[2]}] ({i[1]})" for i in suggested_vals])
+            message = f"'{bad}' not avaliable parameter for '{catalog.iloc[0]['id']}'. Try: {suggested_strs}"
+
+            # message = f"'{bad}' not avaliable parameter for '{catalog.iloc[0]['id']}'. Try: \n\t{'> ' + m['variable'] + ' [' + m['units'] + '] (' + m['description'] + ')' }"
+            # message = f"'{bad}' not avaliable parameter for '{catalog.iloc[0]['id']}'. Try: \n\t{'> ' + str(m['variable']) + ' [' + str(m['units']) + '] (' + str(m['description']) + ')' }"
+            
+            raise ValueError(message)
     
     # 2. scenario filter
     if scenario is not None:
 
         # Check if "historical" is in the catalog, if so, add "historical" to the scenario list
         if "historical" in catalog["scenario"].unique():
             if isinstance(scenario, str):
```

### Comparing `climatePy-0.5.0/climatePy/_dap.py` & `climatePy-0.5.1/climatePy/_dap.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.5.0/climatePy/_extract_sites.py` & `climatePy-0.5.1/climatePy/_extract_sites.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.5.0/climatePy/_netrc_utils.py` & `climatePy-0.5.1/climatePy/_netrc_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.5.0/climatePy/_shortcuts.py` & `climatePy-0.5.1/climatePy/_shortcuts.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.5.0/climatePy/_utils.py` & `climatePy-0.5.1/climatePy/_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.5.0/climatePy/_viz.py` & `climatePy-0.5.1/climatePy/_viz.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.5.0/climatePy/data/catalog.parquet` & `climatePy-0.5.1/climatePy/data/catalog.parquet`

 * *Files identical despite different names*

### Comparing `climatePy-0.5.0/climatePy.egg-info/PKG-INFO` & `climatePy-0.5.1/climatePy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Python package for getting point and gridded climate data by AOI.
 Author: Angus Watters, Mike Johnson
 Author-email: anguswatters@gmail.com, mikecp11@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `climatePy-0.5.0/climatePy.egg-info/SOURCES.txt` & `climatePy-0.5.1/climatePy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `climatePy-0.5.0/setup.py` & `climatePy-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="climatePy",                         # pkg name
-    version='0.5.0',
+    version='0.5.1',
     author="Angus Watters, Mike Johnson",     # authors
     author_email = "anguswatters@gmail.com, mikecp11@gmail.com",
     description="A Python package for getting point and gridded climate data by AOI.",
     long_description=long_description,      # long description is read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # python modules to install
     classifiers=[
```

### Comparing `climatePy-0.5.0/tests/test_climatepy_filter.py` & `climatePy-0.5.1/tests/test_climatepy_filter.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.5.0/tests/test_dap.py` & `climatePy-0.5.1/tests/test_dap.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.5.0/tests/test_extract_sites.py` & `climatePy-0.5.1/tests/test_extract_sites.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.5.0/tests/test_netrc.py` & `climatePy-0.5.1/tests/test_netrc.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.5.0/tests/test_shortcuts.py` & `climatePy-0.5.1/tests/test_shortcuts.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 # old imports
 # import climatePy._utils as climatePy
 # import climatePy._extract_sites as climatePy
 # import climatePy._dap as climatePy
 import climatePy._shortcuts as climatePy
 # import climatePy._climatepy_filter as climatePy
+# import climatePy
 
 # data manipulation libs
 import pandas as pd
 import geopandas as gpd
 import xarray as xr
 
 # standard python libs
@@ -233,15 +234,19 @@
     end_date1   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["rmin"].time.values])
 
     assert end_date1 - start_date1 == pd.Timedelta("1826D")
 
     assert "rmin" in output["rmin"].time[0].values.item()
     assert len(output["rmin"].time.values) == 1827
 
-    
+def test_getGridMET_value_error_with_incorrect_varname(AOI):
+
+    with pytest.raises(ValueError):
+        climatePy.getGridMET(AOI, "prcp", "2010-01-01", "2010-02-01", verbose=True)
+
 def test_getTerraClimNormals_case1(AOI):
     
     # ---- Case 1 ----
     verbose   = True
     varname = ["ppt", "tmax"]
     scenario  = '19611990'
     month     = [1, 2]
@@ -1121,173 +1126,173 @@
 
     # assert len(output["Vertisols"]) == 432
     # assert len(output["Gypsisols"]) == 432
 
     # assert output['Vertisols'].shape == (432, 945)
     # assert output['Gypsisols'].shape == (432, 945)
 
-# # def test_getCHIRPS_case1(AOI):
+# def test_getCHIRPS_case1(AOI):
     
-# #     #  ---- Case 1: Single month CHIRPS ----
-# #     verbose   = True
-# #     startDate = "2019-01-01"
-# #     endDate   = "2019-01-01"
-# #     varname   = 'precip'
-# #     timeRes   = "daily"
+#     #  ---- Case 1: Single month CHIRPS ----
+#     verbose   = True
+#     startDate = "2019-01-01"
+#     endDate   = "2019-01-01"
+#     varname   = 'precip'
+#     timeRes   = "daily"
 
-# #     # NOTE: CHIRPS data is currently inaccesible due to server issues with the data provider
-# #     # NOTE: This test will fail until the data provider resolves the server issues
-# #     with pytest.raises(Exception):
-# #         # Call function to get output
-# #         output = climatePy.getCHIRPS(AOI, varname, startDate, endDate, timeRes, verbose)
+#     # NOTE: CHIRPS data is currently inaccesible due to server issues with the data provider
+#     # NOTE: This test will fail until the data provider resolves the server issues
+#     with pytest.raises(Exception):
+#         # Call function to get output
+#         output = climatePy.getCHIRPS(AOI, varname, startDate, endDate, timeRes, verbose)
 
-# #     # # Assert that the output is a dictionary
-# #     # assert type(output) == dict
+#     # # Assert that the output is a dictionary
+#     # assert type(output) == dict
 
-# #     # # Assert that the output dictionary has the correct keys
-# #     # assert set(output.keys()) == {"precip"}
+#     # # Assert that the output dictionary has the correct keys
+#     # assert set(output.keys()) == {"precip"}
 
-# #     # # Assert that the values of the output dictionary are xarray DataArrays
-# #     # assert isinstance(output["precip"], xr.DataArray)
+#     # # Assert that the values of the output dictionary are xarray DataArrays
+#     # assert isinstance(output["precip"], xr.DataArray)
 
-# #     # # Assert that the dimensions of the output DataArrays are correct
-# #     # assert output["precip"].dims == ("y", "x", "time")
+#     # # Assert that the dimensions of the output DataArrays are correct
+#     # assert output["precip"].dims == ("y", "x", "time")
 
-# #     # # Assert that the temporal resolution of the output DataArrays is correct
-# #     # start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["precip"].time[0].values.item()).group(0), "%Y-%m-%d")
-# #     # end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["precip"].time[-1].values.item()).group(0), "%Y-%m-%d")
+#     # # Assert that the temporal resolution of the output DataArrays is correct
+#     # start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["precip"].time[0].values.item()).group(0), "%Y-%m-%d")
+#     # end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["precip"].time[-1].values.item()).group(0), "%Y-%m-%d")
 
-# #     # # check temporal range
-# #     # assert end_date1 - start_date1 == pd.Timedelta("0D")
+#     # # check temporal range
+#     # assert end_date1 - start_date1 == pd.Timedelta("0D")
 
-# #     # assert "precip" in output["precip"].time[0].values.item()
+#     # assert "precip" in output["precip"].time[0].values.item()
 
-# #     # assert len(output["precip"].time.values) == 1
-# #     # assert output['precip'].shape == (19, 40, 1)
+#     # assert len(output["precip"].time.values) == 1
+#     # assert output['precip'].shape == (19, 40, 1)
 
-# # def test_getCHIRPS_case2(AOI):
-# #     #  ---- Case 2: Multi Month CHIRPS ----
-# #     verbose   = True
-# #     startDate = "2019-01-01"
-# #     endDate   = "2019-03-01"
-# #     varname   = 'precip'
-# #     timeRes   = "daily"
+# def test_getCHIRPS_case2(AOI):
+#     #  ---- Case 2: Multi Month CHIRPS ----
+#     verbose   = True
+#     startDate = "2019-01-01"
+#     endDate   = "2019-03-01"
+#     varname   = 'precip'
+#     timeRes   = "daily"
 
-# #     # NOTE: CHIRPS data is currently inaccesible due to server issues with the data provider
-# #     # NOTE: This test will fail until the data provider resolves the server issues
-# #     with pytest.raises(Exception):
-# #         # Call function to get output
-# #         output = climatePy.getCHIRPS(AOI, varname, startDate, endDate, timeRes, verbose)
-# #         print(f"----- CHIRPS test case 2 keys: \n > {output.keys()} ----")
+#     # NOTE: CHIRPS data is currently inaccesible due to server issues with the data provider
+#     # NOTE: This test will fail until the data provider resolves the server issues
+#     with pytest.raises(Exception):
+#         # Call function to get output
+#         output = climatePy.getCHIRPS(AOI, varname, startDate, endDate, timeRes, verbose)
+#         print(f"----- CHIRPS test case 2 keys: \n > {output.keys()} ----")
 
-# #     # assert type(output) == dict
+#     # assert type(output) == dict
 
-# #     # # Assert that the output dictionary has the correct keys
-# #     # assert set(output.keys()) == {"precip"}
+#     # # Assert that the output dictionary has the correct keys
+#     # assert set(output.keys()) == {"precip"}
 
-# #     # # Assert that the values of the output dictionary are xarray DataArrays
-# #     # assert isinstance(output["precip"], xr.DataArray)
+#     # # Assert that the values of the output dictionary are xarray DataArrays
+#     # assert isinstance(output["precip"], xr.DataArray)
 
-# #     # # Assert that the dimensions of the output DataArrays are correct
-# #     # assert output["precip"].dims == ("y", "x", "time")
+#     # # Assert that the dimensions of the output DataArrays are correct
+#     # assert output["precip"].dims == ("y", "x", "time")
 
-# #     # # Assert that the temporal resolution of the output DataArrays is correct
-# #     # start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["precip"].time[0].values.item()).group(0), "%Y-%m-%d")
-# #     # end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["precip"].time[-1].values.item()).group(0), "%Y-%m-%d")
+#     # # Assert that the temporal resolution of the output DataArrays is correct
+#     # start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["precip"].time[0].values.item()).group(0), "%Y-%m-%d")
+#     # end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["precip"].time[-1].values.item()).group(0), "%Y-%m-%d")
 
-# #     # # check temporal range
-# #     # assert end_date1 - start_date1 == pd.Timedelta("59D")
+#     # # check temporal range
+#     # assert end_date1 - start_date1 == pd.Timedelta("59D")
 
-# #     # assert "precip" in output["precip"].time[0].values.item()
+#     # assert "precip" in output["precip"].time[0].values.item()
 
-# # 	# assert len(output["precip"].time.values) == 3
-# # 	# assert output['precip'].shape == (19, 40, 3)
+# 	# assert len(output["precip"].time.values) == 3
+# 	# assert output['precip'].shape == (19, 40, 3)
 
 
-# # def test_getCHIRPS_case3(AOI):
-# #     #  ---- Case 3: Multi Year Month CHIRPS ----
-# #     verbose   = True
-# #     startDate = "2019-01-01"
-# #     endDate   = "2019-01-15"
-# #     varname       = 'precip'
-# #     timeRes = "daily"
+# def test_getCHIRPS_case3(AOI):
+#     #  ---- Case 3: Multi Year Month CHIRPS ----
+#     verbose   = True
+#     startDate = "2019-01-01"
+#     endDate   = "2019-01-15"
+#     varname       = 'precip'
+#     timeRes = "daily"
 
-# #     # NOTE: CHIRPS data is currently inaccesible due to server issues with the data provider
-# #     # NOTE: This test will fail until the data provider resolves the server issues
-# #     with pytest.raises(Exception):
-# #         # Call function to get output
-# #         output = climatePy.getCHIRPS(AOI, varname, startDate, endDate, timeRes, verbose)
+#     # NOTE: CHIRPS data is currently inaccesible due to server issues with the data provider
+#     # NOTE: This test will fail until the data provider resolves the server issues
+#     with pytest.raises(Exception):
+#         # Call function to get output
+#         output = climatePy.getCHIRPS(AOI, varname, startDate, endDate, timeRes, verbose)
 
-# #         print(f"----- CHIRPS test case 3 keys: \n > {output.keys()} ----")    
+#         print(f"----- CHIRPS test case 3 keys: \n > {output.keys()} ----")    
 
-# #     # # Assert that the output is a dictionary
-# #     # assert type(output) == dict
+#     # # Assert that the output is a dictionary
+#     # assert type(output) == dict
 
-# #     # # Assert that the output dictionary has the correct keys
-# #     # assert set(output.keys()) == {"precip"}
+#     # # Assert that the output dictionary has the correct keys
+#     # assert set(output.keys()) == {"precip"}
 
-# #     # # Assert that the values of the output dictionary are xarray DataArrays
-# #     # assert isinstance(output["precip"], xr.DataArray)
+#     # # Assert that the values of the output dictionary are xarray DataArrays
+#     # assert isinstance(output["precip"], xr.DataArray)
 
-# #     # # Assert that the dimensions of the output DataArrays are correct
-# #     # assert output["precip"].dims == ("y", "x", "time")
+#     # # Assert that the dimensions of the output DataArrays are correct
+#     # assert output["precip"].dims == ("y", "x", "time")
 
-# #     # # Assert that the temporal resolution of the output DataArrays is correct
-# #     # start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}',
-# #     #                                           output["precip"].time[0].values.item()).group(0), "%Y-%m-%d")
+#     # # Assert that the temporal resolution of the output DataArrays is correct
+#     # start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}',
+#     #                                           output["precip"].time[0].values.item()).group(0), "%Y-%m-%d")
 
-# #     # end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', 
-# #     #                                           output["precip"].time[-1].values.item()).group(0), "%Y-%m-%d")
+#     # end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', 
+#     #                                           output["precip"].time[-1].values.item()).group(0), "%Y-%m-%d")
 
-# #     # # check temporal range
-# #     # assert end_date1 - start_date1 == pd.Timedelta("15D")
+#     # # check temporal range
+#     # assert end_date1 - start_date1 == pd.Timedelta("15D")
 
-# #     # assert "precip" in output["precip"].time[0].values.item()
+#     # assert "precip" in output["precip"].time[0].values.item()
 
-# #     # assert len(output["precip"].time.values) == 14
-# #     # assert output['precip'].shape == (19, 40, 14)
+#     # assert len(output["precip"].time.values) == 14
+#     # assert output['precip'].shape == (19, 40, 14)
 
-# # def test_getCHIRPS_case4(AOI):
-# #     #  ---- Case 4: Monthly Multi Year CHIRPS ----
-# #     verbose   = True
-# #     startDate = "2019-01-01"
-# #     endDate   = "2020-02-01"
-# #     varname       = 'precip'
-# #     timeRes = "monthly"
+# def test_getCHIRPS_case4(AOI):
+#     #  ---- Case 4: Monthly Multi Year CHIRPS ----
+#     verbose   = True
+#     startDate = "2019-01-01"
+#     endDate   = "2020-02-01"
+#     varname       = 'precip'
+#     timeRes = "monthly"
 
-# #     # NOTE: CHIRPS data is currently inaccesible due to server issues with the data provider
-# #     # NOTE: This test will fail until the data provider resolves the server issues
-# #     with pytest.raises(Exception):
-# #         # Call function to get output
-# #         output = climatePy.getCHIRPS(AOI, varname, startDate, endDate, timeRes, verbose)
+#     # NOTE: CHIRPS data is currently inaccesible due to server issues with the data provider
+#     # NOTE: This test will fail until the data provider resolves the server issues
+#     with pytest.raises(Exception):
+#         # Call function to get output
+#         output = climatePy.getCHIRPS(AOI, varname, startDate, endDate, timeRes, verbose)
 
-# #     # # Assert that the output is a dictionary
-# #     # assert type(output) == dict
+#     # # Assert that the output is a dictionary
+#     # assert type(output) == dict
 
-# #     # # Assert that the output dictionary has the correct keys
-# #     # assert set(output.keys()) == {"precip"}
+#     # # Assert that the output dictionary has the correct keys
+#     # assert set(output.keys()) == {"precip"}
 
-# #     # # Assert that the values of the output dictionary are xarray DataArrays
-# #     # assert isinstance(output["precip"], xr.DataArray)
+#     # # Assert that the values of the output dictionary are xarray DataArrays
+#     # assert isinstance(output["precip"], xr.DataArray)
 
-# #     # # Assert that the dimensions of the output DataArrays are correct
-# #     # assert output["precip"].dims == ("y", "x", "time")
+#     # # Assert that the dimensions of the output DataArrays are correct
+#     # assert output["precip"].dims == ("y", "x", "time")
 
-# #     # # Assert that the temporal resolution of the output DataArrays is correct
-# #     # start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}',
-# #     # 				output["precip"].time[0].values.item()).group(0), "%Y-%m-%d")
+#     # # Assert that the temporal resolution of the output DataArrays is correct
+#     # start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}',
+#     # 				output["precip"].time[0].values.item()).group(0), "%Y-%m-%d")
 
-# #     # end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', 
-# #     # 				output["precip"].time[-1].values.item()).group(0), "%Y-%m-%d")
+#     # end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', 
+#     # 				output["precip"].time[-1].values.item()).group(0), "%Y-%m-%d")
 
-# #     # # check temporal range
-# #     # assert end_date1 - start_date1 == pd.Timedelta("396D")
-# #     # assert "precip" in output["precip"].time[0].values.item()
+#     # # check temporal range
+#     # assert end_date1 - start_date1 == pd.Timedelta("396D")
+#     # assert "precip" in output["precip"].time[0].values.item()
 
-# #     # # calculate number of months
-# #     # months = (end_date1.year - start_date1.year) * 12 + end_date1.month - start_date1.month
-# #     # months = months + 1 if end_date1.day >= end_date1.day else months
+#     # # calculate number of months
+#     # months = (end_date1.year - start_date1.year) * 12 + end_date1.month - start_date1.month
+#     # months = months + 1 if end_date1.day >= end_date1.day else months
 
-# #     # # check that number of months in output is correct (within 1 month)
-# #     # assert (len(output["precip"]['time']) == months or
-# #     # 		len(output["precip"]['time']) + 1 == months or
-# #     # 		len(output["precip"]['time']) - 1 == months)
+#     # # check that number of months in output is correct (within 1 month)
+#     # assert (len(output["precip"]['time']) == months or
+#     # 		len(output["precip"]['time']) + 1 == months or
+#     # 		len(output["precip"]['time']) - 1 == months)
```

### Comparing `climatePy-0.5.0/tests/test_utils.py` & `climatePy-0.5.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.5.0/tests/test_vrt.py` & `climatePy-0.5.1/tests/test_vrt.py`

 * *Files identical despite different names*

