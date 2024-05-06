# Comparing `tmp/okn_py_updater-1.0.6.tar.gz` & `tmp/okn_py_updater-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okn_py_updater-1.0.6.tar", last modified: Mon Aug 14 23:43:39 2023, max compression
+gzip compressed data, was "okn_py_updater-1.0.7.tar", last modified: Mon May  6 22:36:41 2024, max compression
```

## Comparing `okn_py_updater-1.0.6.tar` & `okn_py_updater-1.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-14 23:43:39.409579 okn_py_updater-1.0.6/
--rw-rw-rw-   0        0        0    11558 2023-08-07 21:09:13.000000 okn_py_updater-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     3706 2023-08-14 23:43:39.409579 okn_py_updater-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3129 2023-08-14 21:59:14.000000 okn_py_updater-1.0.6/README.md
--rw-rw-rw-   0        0        0      657 2023-08-14 23:40:34.000000 okn_py_updater-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-14 23:43:39.409579 okn_py_updater-1.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-14 23:43:39.393889 okn_py_updater-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-08-14 23:43:39.393889 okn_py_updater-1.0.6/src/okn_py_updater/
--rw-rw-rw-   0        0        0        0 2023-08-07 21:09:13.000000 okn_py_updater-1.0.6/src/okn_py_updater/__init__.py
--rw-rw-rw-   0        0        0    18522 2023-08-14 21:59:14.000000 okn_py_updater-1.0.6/src/okn_py_updater/okn_py_updater.py
-drwxrwxrwx   0        0        0        0 2023-08-14 23:43:39.409579 okn_py_updater-1.0.6/src/okn_py_updater.egg-info/
--rw-rw-rw-   0        0        0     3706 2023-08-14 23:43:39.000000 okn_py_updater-1.0.6/src/okn_py_updater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-08-14 23:43:39.000000 okn_py_updater-1.0.6/src/okn_py_updater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-14 23:43:39.000000 okn_py_updater-1.0.6/src/okn_py_updater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-08-14 23:43:39.000000 okn_py_updater-1.0.6/src/okn_py_updater.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 22:36:41.233960 okn_py_updater-1.0.7/
+-rw-rw-rw-   0        0        0    11558 2024-05-06 22:12:10.000000 okn_py_updater-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     3706 2024-05-06 22:36:41.232953 okn_py_updater-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3129 2024-05-06 22:12:10.000000 okn_py_updater-1.0.7/README.md
+-rw-rw-rw-   0        0        0      657 2024-05-06 22:36:30.000000 okn_py_updater-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 22:36:41.233960 okn_py_updater-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 22:36:41.209179 okn_py_updater-1.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 22:36:41.213701 okn_py_updater-1.0.7/src/okn_py_updater/
+-rw-rw-rw-   0        0        0        0 2024-05-06 22:12:10.000000 okn_py_updater-1.0.7/src/okn_py_updater/__init__.py
+-rw-rw-rw-   0        0        0    18323 2024-05-06 22:35:43.000000 okn_py_updater-1.0.7/src/okn_py_updater/okn_py_updater.py
+drwxrwxrwx   0        0        0        0 2024-05-06 22:36:41.231443 okn_py_updater-1.0.7/src/okn_py_updater.egg-info/
+-rw-rw-rw-   0        0        0     3706 2024-05-06 22:36:41.000000 okn_py_updater-1.0.7/src/okn_py_updater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2024-05-06 22:36:41.000000 okn_py_updater-1.0.7/src/okn_py_updater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 22:36:41.000000 okn_py_updater-1.0.7/src/okn_py_updater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-06 22:36:41.000000 okn_py_updater-1.0.7/src/okn_py_updater.egg-info/top_level.txt
```

### Comparing `okn_py_updater-1.0.6/LICENSE` & `okn_py_updater-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `okn_py_updater-1.0.6/PKG-INFO` & `okn_py_updater-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okn_py_updater
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python Library for OKN Data Updater
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/ZawLinTun16925410/okn_data_updater
 Project-URL: Bug Tracker, https://github.com/ZawLinTun16925410/okn_data_updater/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `okn_py_updater-1.0.6/README.md` & `okn_py_updater-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `okn_py_updater-1.0.6/pyproject.toml` & `okn_py_updater-1.0.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "okn_py_updater"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="Zaw Lin Tun", email="zawlintun1511@gmail.com" },
 ]
 description = "Python Library for OKN Data Updater"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `okn_py_updater-1.0.6/src/okn_py_updater/okn_py_updater.py` & `okn_py_updater-1.0.7/src/okn_py_updater/okn_py_updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import collections
 import numpy as np
 import math
 from scipy.signal import medfilt
 
 
-def dispatch_function(filter_config_info, data_dict_input, config_info=None):
+def live_dispatch_function(filter_config_info, data_dict_input):
     match_item = filter_config_info["function"]
     # print(f"Dispatched function name: {match_item}")
     if match_item == 'cdp_direction':
         # t = data_dict_input[filter_config_info["input"]]
         # # need to be fixed ********
         # keyname = "need to be fixed"
         # f = cdp_direction(config_info.log, keyname, t)
@@ -93,29 +93,24 @@
     elif match_item == 'deblinker':
         print(f"{match_item} will be coming soon.")
 
     elif match_item == 'shiftSignal':
         print(f"{match_item} will be coming soon.")
 
     elif match_item == 'medianFilter':
-        # input_column = filter_config_info["input"][0]
-        # f = data_dict_input[input_column]
-        # n = filter_config_info["npoint"]
-        # if len(f) >= n:
-        #     data_dict_input[filter_config_info["output"]] = medfilt(f, n)
-        #     print("*")
-        #     print(len(f))
-        #     print(f)
-        #     print(input_column)
-        #     print(medfilt(f, n))
-        #     print("*")
-        # else:
-        #     data_dict_input[filter_config_info["output"]] = f
-        pass
-        # print(f"{input_column} column has been median filtered with n point {n}.")
+        input_column = filter_config_info["input"][0]
+        f = data_dict_input[input_column]
+        n = filter_config_info["npoint"]
+        if len(f) >= n:
+            last_n_number_array = f[-n:]
+            mean_value = np.nanmean(last_n_number_array)
+            f[-1] = mean_value
+            data_dict_input[filter_config_info["output"]] = f
+        else:
+            data_dict_input[filter_config_info["output"]] = f
 
     elif match_item == 'replaceNanBy':
         input_column = filter_config_info["input"][0]
         input_array = data_dict_input[input_column]
         pointer = filter_config_info["pointer"]
         data_dict_input[filter_config_info["output"]] = replace_nan_by(data_dict_input, input_array, pointer)
 
@@ -383,15 +378,15 @@
             for data in self.circular_buffer:
                 for header_index, header_string in enumerate(self.header_array):
                     data_dict[header_string].append(float(data[header_index]))
 
             # if len(self.circular_buffer) >= 3:
             for filter_info in self.filter_config:
                 if filter_info["Enabled"]:
-                    data_dict = dispatch_function(filter_info, data_dict, self.config)
+                    data_dict = live_dispatch_function(filter_info, data_dict)
                 else:
                     pass
 
             for index in range(len(data_dict[output_header_array[0]])):
                 temp_array = []
                 for header in output_header_array:
                     try:
@@ -421,15 +416,15 @@
                 for data in self.circular_buffer:
                     for header_index, header_string in enumerate(self.header_array):
                         data_dict[header_string].append(float(data[header_index]))
 
                 # if len(self.circular_buffer) >= 3:
                 for filter_info in self.filter_config:
                     if filter_info["Enabled"]:
-                        data_dict = dispatch_function(filter_info, data_dict, self.config)
+                        data_dict = live_dispatch_function(filter_info, data_dict)
                     else:
                         pass
 
                 for index in range(len(data_dict[output_header_array[0]])):
                     temp_array = []
                     for header in output_header_array:
                         try:
```

### Comparing `okn_py_updater-1.0.6/src/okn_py_updater.egg-info/PKG-INFO` & `okn_py_updater-1.0.7/src/okn_py_updater.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: okn-py-updater
-Version: 1.0.6
+Name: okn_py_updater
+Version: 1.0.7
 Summary: Python Library for OKN Data Updater
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/ZawLinTun16925410/okn_data_updater
 Project-URL: Bug Tracker, https://github.com/ZawLinTun16925410/okn_data_updater/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

