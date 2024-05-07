# Comparing `tmp/threed_optix-5.0.4.tar.gz` & `tmp/threed_optix-5.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threed_optix-5.0.4.tar", last modified: Mon May  6 11:41:54 2024, max compression
+gzip compressed data, was "threed_optix-5.0.5.tar", last modified: Tue May  7 07:35:27 2024, max compression
```

## Comparing `threed_optix-5.0.4.tar` & `threed_optix-5.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-06 11:41:54.939089 threed_optix-5.0.4/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      148 2024-03-24 13:38:50.000000 threed_optix-5.0.4/.gitignore
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1064 2024-02-20 12:16:48.000000 threed_optix-5.0.4/LICENSE.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2377 2024-05-06 11:41:54.939089 threed_optix-5.0.4/PKG-INFO
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2077 2024-03-24 13:38:50.000000 threed_optix-5.0.4/README.md
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-06 11:41:54.939089 threed_optix-5.0.4/help/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    43940 2024-05-06 11:41:26.000000 threed_optix-5.0.4/help/SDK help text.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    43940 2024-05-06 11:41:26.000000 threed_optix-5.0.4/help/SDK help.md
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      107 2024-05-06 11:41:54.939089 threed_optix-5.0.4/setup.cfg
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1222 2024-05-06 11:41:26.000000 threed_optix-5.0.4/setup.py
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-06 11:41:54.939089 threed_optix-5.0.4/src/
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-06 11:41:54.939089 threed_optix-5.0.4/src/threed_optix/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      844 2024-05-06 11:41:26.000000 threed_optix-5.0.4/src/threed_optix/__init__.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    23704 2024-05-06 11:40:41.000000 threed_optix-5.0.4/src/threed_optix/analyses.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     4172 2024-03-24 13:38:50.000000 threed_optix-5.0.4/src/threed_optix/beams.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    43529 2024-05-06 11:41:26.000000 threed_optix-5.0.4/src/threed_optix/client.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)       29 2024-03-24 13:38:50.000000 threed_optix-5.0.4/src/threed_optix/optimize.py
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-06 11:41:54.939089 threed_optix-5.0.4/src/threed_optix/package_utils/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)       16 2024-03-24 13:38:50.000000 threed_optix-5.0.4/src/threed_optix/package_utils/__init__.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    15563 2024-05-01 11:13:46.000000 threed_optix-5.0.4/src/threed_optix/package_utils/api.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     3247 2024-05-01 11:13:46.000000 threed_optix-5.0.4/src/threed_optix/package_utils/general.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1582 2024-05-01 11:13:46.000000 threed_optix-5.0.4/src/threed_optix/package_utils/math.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)       70 2024-03-24 13:38:50.000000 threed_optix-5.0.4/src/threed_optix/package_utils/matlab.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    19129 2024-05-06 11:41:26.000000 threed_optix-5.0.4/src/threed_optix/package_utils/vars.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    61029 2024-05-06 11:41:26.000000 threed_optix-5.0.4/src/threed_optix/parts.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    15046 2024-05-06 11:41:26.000000 threed_optix-5.0.4/src/threed_optix/simulations.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     4718 2024-05-01 11:13:46.000000 threed_optix-5.0.4/src/threed_optix/utils.py
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-06 11:41:54.939089 threed_optix-5.0.4/src/threed_optix.egg-info/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2377 2024-05-06 11:41:54.000000 threed_optix-5.0.4/src/threed_optix.egg-info/PKG-INFO
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      756 2024-05-06 11:41:54.000000 threed_optix-5.0.4/src/threed_optix.egg-info/SOURCES.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)        1 2024-05-06 11:41:54.000000 threed_optix-5.0.4/src/threed_optix.egg-info/dependency_links.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      107 2024-05-06 11:41:54.000000 threed_optix-5.0.4/src/threed_optix.egg-info/requires.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)       13 2024-05-06 11:41:54.000000 threed_optix-5.0.4/src/threed_optix.egg-info/top_level.txt
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-07 07:35:27.593617 threed_optix-5.0.5/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      148 2024-03-24 13:38:50.000000 threed_optix-5.0.5/.gitignore
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1064 2024-02-20 12:16:48.000000 threed_optix-5.0.5/LICENSE.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2377 2024-05-07 07:35:27.593617 threed_optix-5.0.5/PKG-INFO
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2077 2024-03-24 13:38:50.000000 threed_optix-5.0.5/README.md
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-07 07:35:27.593617 threed_optix-5.0.5/help/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    43940 2024-05-06 11:41:26.000000 threed_optix-5.0.5/help/SDK help text.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    43940 2024-05-06 11:41:26.000000 threed_optix-5.0.5/help/SDK help.md
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      107 2024-05-07 07:35:27.593617 threed_optix-5.0.5/setup.cfg
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1222 2024-05-06 11:41:26.000000 threed_optix-5.0.5/setup.py
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-07 07:35:27.593617 threed_optix-5.0.5/src/
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-07 07:35:27.593617 threed_optix-5.0.5/src/threed_optix/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      844 2024-05-06 11:41:26.000000 threed_optix-5.0.5/src/threed_optix/__init__.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    23949 2024-05-07 07:32:41.000000 threed_optix-5.0.5/src/threed_optix/analyses.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     4172 2024-03-24 13:38:50.000000 threed_optix-5.0.5/src/threed_optix/beams.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    43648 2024-05-07 07:32:41.000000 threed_optix-5.0.5/src/threed_optix/client.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)       29 2024-03-24 13:38:50.000000 threed_optix-5.0.5/src/threed_optix/optimize.py
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-07 07:35:27.593617 threed_optix-5.0.5/src/threed_optix/package_utils/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)       16 2024-03-24 13:38:50.000000 threed_optix-5.0.5/src/threed_optix/package_utils/__init__.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    15563 2024-05-01 11:13:46.000000 threed_optix-5.0.5/src/threed_optix/package_utils/api.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     3248 2024-05-07 07:32:41.000000 threed_optix-5.0.5/src/threed_optix/package_utils/general.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1582 2024-05-01 11:13:46.000000 threed_optix-5.0.5/src/threed_optix/package_utils/math.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)       70 2024-03-24 13:38:50.000000 threed_optix-5.0.5/src/threed_optix/package_utils/matlab.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    19129 2024-05-07 07:32:41.000000 threed_optix-5.0.5/src/threed_optix/package_utils/vars.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    61029 2024-05-07 07:32:32.000000 threed_optix-5.0.5/src/threed_optix/parts.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    15046 2024-05-06 11:41:26.000000 threed_optix-5.0.5/src/threed_optix/simulations.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     4719 2024-05-07 07:32:41.000000 threed_optix-5.0.5/src/threed_optix/utils.py
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-07 07:35:27.593617 threed_optix-5.0.5/src/threed_optix.egg-info/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2377 2024-05-07 07:35:27.000000 threed_optix-5.0.5/src/threed_optix.egg-info/PKG-INFO
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      756 2024-05-07 07:35:27.000000 threed_optix-5.0.5/src/threed_optix.egg-info/SOURCES.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)        1 2024-05-07 07:35:27.000000 threed_optix-5.0.5/src/threed_optix.egg-info/dependency_links.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      107 2024-05-07 07:35:27.000000 threed_optix-5.0.5/src/threed_optix.egg-info/requires.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)       13 2024-05-07 07:35:27.000000 threed_optix-5.0.5/src/threed_optix.egg-info/top_level.txt
```

### Comparing `threed_optix-5.0.4/LICENSE.txt` & `threed_optix-5.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.4/PKG-INFO` & `threed_optix-5.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threed_optix
-Version: 5.0.4
+Version: 5.0.5
 Home-page: https://3doptix.com
 Author: 3DOptix
 Author-email: ereztep@3doptix.com
 License: MIT
 Keywords: Optics,Optical Design,Optical Simulation,Optical Design Software,3DOptix
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `threed_optix-5.0.4/README.md` & `threed_optix-5.0.5/README.md`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.4/help/SDK help text.txt` & `threed_optix-5.0.5/help/SDK help text.txt`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.4/help/SDK help.md` & `threed_optix-5.0.5/help/SDK help.md`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.4/setup.py` & `threed_optix-5.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.4/src/threed_optix/__init__.py` & `threed_optix-5.0.5/src/threed_optix/__init__.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.4/src/threed_optix/analyses.py` & `threed_optix-5.0.5/src/threed_optix/analyses.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,17 @@
 
             return errors
 
         # If rays is an integer, indicating the number of rays for all lasers
         if isinstance(rays, float) or isinstance(rays, int):
             rays = {laser: rays for laser in surface._part._setup.light_sources}
 
+        if isinstance(resolution, (int, float)):
+            resolution = (resolution, resolution)
+
         # Check if the arguments are valid
         errors = verify(fast=fast, name=name, rays=rays, surface = surface)
         if errors:
             raise AssertionError(v.argument_repair_message(errors))
 
 
         self._added = False
@@ -338,15 +341,15 @@
         # Check if the data kind is supported
         if file_results['data_kind'] not in v.SUPPORTED_DATA_KINDS_NAMES:
             if v.DEBUG:
                 print(f"Data kind not in the supported kinds: {file_results['data_kind']}")
             return False
 
         # The data shape should be a matrix of size res_x*res_y for each wavelength. For polarization kind raw, each matrix item has 3 numbers.
-        data_shape =(len(wls), self.resolution[0], self.resolution[1], 3) if headers_nums['polarization kind'][0] == 4 else (len(wls), self.resolution[0], self.resolution[1])
+        data_shape = (len(wls), self.resolution[0], self.resolution[1], 3) if headers_nums['polarization kind'][0] == 4 else (len(wls), self.resolution[0], self.resolution[1])
         num_items = reduce(lambda x, y: x * y, data_shape)
 
         # Check if the data shape is correct
         if data.shape[0] != num_items:
             if v.DEBUG:
                 print(f"Data shape not correct: {data.shape}, Expected: {data_shape}")
             return False
@@ -354,31 +357,32 @@
         # Reshape the long list of numbers to the data matrices
         data_matrices = data.reshape(data_shape)
 
         if v.DEBUG:
             print(f'Data matrices shape: {data_matrices.shape}')
 
         # Create a list of results. It's redundant but important since it will be added to a pandas dataframe
-        file_results_with_wls = [file_results.copy() for _ in wls]
+        file_results_with_wls = []
         for i, wl in enumerate(wls):
-
+            wl_dict = file_results.copy()
             if v.DEBUG:
                 print(f'Processing wavelength {wl} nm')
 
             # Get the matrix for the current wavelength
             matrix = data_matrices[i]
 
             # Add the matrix to the results
-            file_results_with_wls[i]['data'] = matrix
+            wl_dict['data'] = matrix
 
             # Add the wavelength to the results
-            file_results_with_wls[i]['wl'] = wl
-        return file_results_with_wls
+            wl_dict['wl'] = wl
 
+            file_results_with_wls.append(wl_dict)
 
+        return file_results_with_wls
 
     def _process_v2(self, directory):
         '''
         Private.
         Processes the results of the analysis
         '''
         results = []
@@ -417,21 +421,28 @@
 
         else:
             raise Exception(f'Version {version} is not supported')
 
         self._raw_results = results
         if version == 1:
             self.results = gu.reorganize_analysis_results_dict(self._raw_results.values())
+
         elif version == 2:
             self.results = AnalysisResults(self._raw_results, maps=self._maps_json, analysis_object=self)
 
         #delete directory and all subdirectories
         os.system(f'rm -rf {directory}')
+        self.reset()
         return self.results
 
+    def reset(self):
+        self._urls = []
+        self._raw_results = {}
+        return None
+
     def _check_file_version(self, file_path):
         version_bytes  =v.AnalysisFile2.VERSION_BYTES
         with open(file_path, 'rb') as f:
             # versin bytes is the range of the 4 bytes indicating the int32 version number. The first int is the beginning, the second is the end
             f.seek(version_bytes[0])
             version = struct.unpack('i', f.read(version_bytes[1] - version_bytes[0]))[0]
```

### Comparing `threed_optix-5.0.4/src/threed_optix/beams.py` & `threed_optix-5.0.5/src/threed_optix/beams.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.4/src/threed_optix/client.py` & `threed_optix-5.0.5/src/threed_optix/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1005,14 +1005,17 @@
                      force: bool = False
                      ) -> bool:
         if auto_add:
             self._add_analysis(analysis, force = force)
 
         data, _ =  au._run_analysis(setup_id=analysis.surface._part._setup.id, api_key=self.api_key, analysis_id=analysis.id)
 
+        if data['results']['error']['code'] != 0:
+            raise Exception(data['results']['error']['message'])
+
         maps_url = data['maps_url']
         analysis._maps_json = requests.get(maps_url).json()
 
         if v.DEBUG:
             print(f'Maps json is {analysis._maps_json}')
 
 
@@ -1049,19 +1052,22 @@
 
         if auto_add:
             added_successfully = []
             added_failed = []
 
             for analysis in analyses:
                 added = self._add_analysis(analysis, force = force)
+
                 if added:
                     added_successfully.append((analysis, analysis.id))
+
                 else:
                     print(f"Analysis {analysis.id} was failed to be added")
                     added_failed.append((analysis, analysis.id))
+
             response['added'] = added_successfully
             response['failed'] += added_failed
             ids = [analysis[1] for analysis in added_successfully]
 
         ran_successfully = []
         ran_failed = []
```

### Comparing `threed_optix-5.0.4/src/threed_optix/package_utils/api.py` & `threed_optix-5.0.5/src/threed_optix/package_utils/api.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.4/src/threed_optix/package_utils/general.py` & `threed_optix-5.0.5/src/threed_optix/package_utils/general.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 def process_v2_results(data, maps):
     def translate_spot_target(row):
         if row['spot_target_kind'] == 0:
             return maps['sources'][row['spot_target_index']]
         if row['spot_target_kind'] == 1:
             return maps['groups'][row['spot_target_index']] if maps.get('groups') else row['spot_target_index']
         return None
+
     if not data:
         return pd.DataFrame(data)
 
     data = pd.DataFrame(data)
     data['polarization'] = data['polarization_kind'].apply(lambda x: x.split('_')[0].capitalize())
     data['spot_target'] = data.apply(translate_spot_target, axis=1)
     data['spot_target_kind'] = data['spot_target_kind'].apply(lambda x: v.AnalysisFile2.SPOT_TARGET_KINDS.get(x))
```

### Comparing `threed_optix-5.0.4/src/threed_optix/package_utils/math.py` & `threed_optix-5.0.5/src/threed_optix/package_utils/math.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.4/src/threed_optix/package_utils/vars.py` & `threed_optix-5.0.5/src/threed_optix/package_utils/vars.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import re
 
 DEBUG = False
 BASE_BACKUP = 'DEFAULT'
 VALID_RESPONSE_CODES = [200, 201, 202, 204]
 # Take the version of the package
-VERSION = "5.0.4"
+VERSION = "5.0.5"
 
 
 #Base API URL
 API_URL = "https://api.3doptix.com/v1"
 
 class Surfaces:
     DETECTOR_FRONT = 'front'
```

### Comparing `threed_optix-5.0.4/src/threed_optix/parts.py` & `threed_optix-5.0.5/src/threed_optix/parts.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.4/src/threed_optix/simulations.py` & `threed_optix-5.0.5/src/threed_optix/simulations.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.4/src/threed_optix/utils.py` & `threed_optix-5.0.5/src/threed_optix/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,14 +103,15 @@
     plt.figure(figsize=(10, 10))
     plt.imshow(matrix)
     plt.scatter(center_point[1], center_point[0], marker='x', color='red')
     plt.gca().add_patch(plt.Circle((center_point[1], center_point[0]), radius, color='red', fill=False))
     plt.show()
 
 def visualize_matrix(matrix, interactive = False, title = None):
+
     if not interactive:
         plt.figure(figsize=(10, 10))
         plt.imshow(matrix)
         if title:
             plt.title(title)
         plt.show()
```

### Comparing `threed_optix-5.0.4/src/threed_optix.egg-info/PKG-INFO` & `threed_optix-5.0.5/src/threed_optix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threed-optix
-Version: 5.0.4
+Version: 5.0.5
 Home-page: https://3doptix.com
 Author: 3DOptix
 Author-email: ereztep@3doptix.com
 License: MIT
 Keywords: Optics,Optical Design,Optical Simulation,Optical Design Software,3DOptix
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `threed_optix-5.0.4/src/threed_optix.egg-info/SOURCES.txt` & `threed_optix-5.0.5/src/threed_optix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

