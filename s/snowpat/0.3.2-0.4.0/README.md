# Comparing `tmp/snowpat-0.3.2.tar.gz` & `tmp/snowpat-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowpat-0.3.2.tar", max compression
+gzip compressed data, was "snowpat-0.4.0.tar", max compression
```

## Comparing `snowpat-0.3.2.tar` & `snowpat-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,24 @@
--rw-r--r--   0        0        0     4818 2024-03-25 16:50:06.259366 snowpat-0.3.2/README.md
--rw-r--r--   0        0        0      451 2024-04-09 14:03:14.009609 snowpat-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     5580 2024-04-09 12:46:08.457422 snowpat-0.3.2/snowpat/SnowLens/Utils.py
--rw-r--r--   0        0        0      217 2024-03-11 09:34:03.280864 snowpat-0.3.2/snowpat/SnowLens/__init__.py
--rw-r--r--   0        0        0     6575 2024-04-09 13:46:24.733339 snowpat-0.3.2/snowpat/SnowLens/plot_helpers_snowpack.py
--rw-r--r--   0        0        0    15924 2024-04-09 13:44:38.712173 snowpat-0.3.2/snowpat/SnowLens/plot_snowpack.py
--rw-r--r--   0        0        0     5193 2024-04-03 14:37:46.233673 snowpat-0.3.2/snowpat/SnowLens/plotting.py
--rw-r--r--   0        0        0     9053 2024-04-03 14:24:45.399491 snowpat-0.3.2/snowpat/SnowLens/snowlens.py
--rw-r--r--   0        0        0      124 2024-04-09 14:03:14.013609 snowpat-0.3.2/snowpat/__init__.py
--rw-r--r--   0        0        0    26470 2024-04-03 14:58:35.674461 snowpat-0.3.2/snowpat/msgs.py
--rw-r--r--   0        0        0     3497 2024-03-01 12:47:20.304690 snowpat-0.3.2/snowpat/pysmet/ACDD.py
--rw-r--r--   0        0        0     6886 2024-04-03 14:33:30.994355 snowpat-0.3.2/snowpat/pysmet/MetaData.py
--rw-r--r--   0        0        0    16663 2024-04-03 14:34:38.847241 snowpat-0.3.2/snowpat/pysmet/SMET.py
--rw-r--r--   0        0        0       81 2024-03-01 13:25:13.396701 snowpat-0.3.2/snowpat/pysmet/__init__.py
--rw-r--r--   0        0        0     3434 2024-03-11 09:34:03.280864 snowpat-0.3.2/snowpat/pysmet/pySMET.py
--rw-r--r--   0        0        0     7785 2024-04-09 13:50:01.031827 snowpat-0.3.2/snowpat/snowpackreader/Snowpack.py
--rw-r--r--   0        0        0      103 2024-03-11 09:34:03.280864 snowpat-0.3.2/snowpat/snowpackreader/__init__.py
--rw-r--r--   0        0        0    16984 2024-03-11 09:34:03.280864 snowpat-0.3.2/snowpat/snowpackreader/snowpackreader.py
--rw-r--r--   0        0        0     5402 1970-01-01 00:00:00.000000 snowpat-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     5883 2024-05-06 15:06:57.836094 snowpat-0.4.0/README.md
+-rw-r--r--   0        0        0      472 2024-05-07 08:45:06.538553 snowpat-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9053 2024-04-03 14:24:45.399491 snowpat-0.4.0/snowpat/SnowLense/SnowLense.py
+-rw-r--r--   0        0        0     5580 2024-04-09 12:46:08.457422 snowpat-0.4.0/snowpat/SnowLense/Utils.py
+-rw-r--r--   0        0        0      218 2024-05-06 15:10:26.419004 snowpat-0.4.0/snowpat/SnowLense/__init__.py
+-rw-r--r--   0        0        0     6575 2024-04-09 13:46:24.733339 snowpat-0.4.0/snowpat/SnowLense/plot_helpers_snowpack.py
+-rw-r--r--   0        0        0    15924 2024-04-09 13:44:38.712173 snowpat-0.4.0/snowpat/SnowLense/plot_snowpack.py
+-rw-r--r--   0        0        0     5193 2024-04-03 14:37:46.233673 snowpat-0.4.0/snowpat/SnowLense/plotting.py
+-rw-r--r--   0        0        0     4229 2024-05-06 15:06:48.375962 snowpat-0.4.0/snowpat/Utils/ACDD.py
+-rw-r--r--   0        0        0      167 2024-05-07 08:45:06.538553 snowpat-0.4.0/snowpat/__init__.py
+-rw-r--r--   0        0        0       93 2024-05-06 15:06:48.375962 snowpat-0.4.0/snowpat/icsv/__init__.py
+-rw-r--r--   0        0        0      112 2024-05-06 15:06:48.375962 snowpat-0.4.0/snowpat/icsv/application_profile.py
+-rw-r--r--   0        0        0    11645 2024-05-06 15:06:48.375962 snowpat-0.4.0/snowpat/icsv/header.py
+-rw-r--r--   0        0        0    11615 2024-05-06 15:06:48.375962 snowpat-0.4.0/snowpat/icsv/icsv_file.py
+-rw-r--r--   0        0        0      108 2024-05-06 15:06:48.375962 snowpat-0.4.0/snowpat/icsv/utility.py
+-rw-r--r--   0        0        0    26470 2024-04-03 14:58:35.674461 snowpat-0.4.0/snowpat/msgs.py
+-rw-r--r--   0        0        0     6984 2024-05-06 15:06:48.375962 snowpat-0.4.0/snowpat/pysmet/MetaData.py
+-rw-r--r--   0        0        0    17516 2024-05-06 15:06:48.375962 snowpat-0.4.0/snowpat/pysmet/SMET.py
+-rw-r--r--   0        0        0      143 2024-05-06 15:12:47.884976 snowpat-0.4.0/snowpat/pysmet/__init__.py
+-rw-r--r--   0        0        0     3434 2024-03-11 09:34:03.280864 snowpat-0.4.0/snowpat/pysmet/pymset.py
+-rw-r--r--   0        0        0     7785 2024-04-09 13:50:01.031827 snowpat-0.4.0/snowpat/snowpackreader/Snowpack.py
+-rw-r--r--   0        0        0      177 2024-05-06 15:13:07.401249 snowpat-0.4.0/snowpat/snowpackreader/__init__.py
+-rw-r--r--   0        0        0    16984 2024-03-11 09:34:03.280864 snowpat-0.4.0/snowpat/snowpackreader/snowpackreader.py
+-rw-r--r--   0        0        0     6512 1970-01-01 00:00:00.000000 snowpat-0.4.0/PKG-INFO
```

### Comparing `snowpat-0.3.2/README.md` & `snowpat-0.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # SNOWPAT
 
-This is a toolbox for handling file formates most often used at SLF.
+This is a toolbox for handling file formates most often used in Snow Science.
 
 There are two submodules:
 pysmet: Used to read and write SMET files
 snowpackreader: Used to read SNOWPACK output files (.pro) and handle profiles easily (soon also with visualization)
-SnowLense: Plotting Framework for files that can be read with this module (SMET not yet available) ([see Documentation](https://snowpat-patrick-leibersperger-c7ec84b7d2c6ab235482777a3905915fe.gitlab-pages.wsl.ch/indexplot/))
+SnowLense: Plotting Framework for files that can be read with this module (SMET not yet available) ([see Documentation](http://patrick.leibersperger.gitlab-pages.wsl.ch/snowpat))
 
 ## News
 
+2024-05-05: A module to read and write iCSV files.
+
 2024-03-25: Installation via PyPi now possible
 
 2024-03-08: Plotting of Snow Profiles is available with SnowLense module
 
 2024-03-01: A simple merge function is now available to join to SMET Files: merge(SMETFile, override) and mergeFromFile(filename, override)
 
 ## Installation
@@ -34,14 +36,15 @@
 the --user option might be needed if you do not have admin rights.
 
 ### Upgrade
 
 If you already have an installation of Sowpat, that is out of date, run:
 
 ```bash
+pip install [--user] --upgrade snowpat
 pip install [--user] --upgrade git+https://gitlabext.wsl.ch/patrick.leibersperger/snowpat.git
 ```
 
 ### Manually
 
 Download the folder, and from the main directory run:
 
@@ -55,15 +58,15 @@
 pip install [--user] .
 ```
 
 ## Documentation
 
 The main documentation can be found under the respective module names, i.e. pySMET and SMET, as well as snowpackreader
 
-Extensive Documentation is available [online](http://snowpat-patrick-leibersperger-c7ec84b7d2c6ab235482777a3905915fe.gitlab-pages.wsl.ch/), it uses http, so you might get a privacy error in your browser;
+Extensive Documentation is available [online](http://patrick.leibersperger.gitlab-pages.wsl.ch/snowpat), it uses http, so you might get a privacy error in your browser;
 Or prepuilt in artifacts.zip, whic can be found in [job artifacts](https://gitlabext.wsl.ch/patrick.leibersperger/snowpat/-/artifacts): under (Number) files download the folder.
 
 If you download the zip folder just open index.html in your browser.
 
 Or you can build the docs yourself.
 
 ### MkDocs
@@ -93,14 +96,43 @@
 Please see the Documentation for more Examples and information on the full capabilities
 
 ```python
 from snowpat import pysmet as smet
 from snowpat import snowpackreader as spr
 ```
 
+### Examples iCSV
+
+```python
+from snowpat import icsv
+
+file = icsv.read(filename)
+data_pandas = file.data
+data_xarray = file.to_xarray()
+# metadata and fields can be accessed with get_attribute
+field_delimiter = file.metadata.get_attribute("field_delimiter")
+fields = file.fields.get_attribute("fields")
+# required keys will always be present, as a sanity check is done. Any other might return None if it is not available.
+# To see what metadata is available, you can print the information:
+file.info() # prints information about the whole file
+print(file.metadata) # prints information on the metadata only
+print(file.fields) # print information on the fields section
+
+# changing metadata
+file.metadata.set_attribute("field_delimiter", ":")
+
+# and for writing to an output again (if no output filename is provided, the given filename is used with an out flag):
+file.write(out_filename)
+
+# It is possible to convert SMET files to iCSV:
+from snowpat import pysmet as smet
+smet_file = smet.read(smet_filename)
+icsv_file = from_smet(smet_file)
+```
+
 ### Examples pySMET
 
 ```python
 from snowpat import pysmet as smet
 
 file = smet.read(filename)
 data_pandas = file.data
```

### Comparing `snowpat-0.3.2/snowpat/SnowLens/Utils.py` & `snowpat-0.4.0/snowpat/SnowLense/Utils.py`

 * *Files identical despite different names*

### Comparing `snowpat-0.3.2/snowpat/SnowLens/plot_helpers_snowpack.py` & `snowpat-0.4.0/snowpat/SnowLense/plot_helpers_snowpack.py`

 * *Files identical despite different names*

### Comparing `snowpat-0.3.2/snowpat/SnowLens/plot_snowpack.py` & `snowpat-0.4.0/snowpat/SnowLense/plot_snowpack.py`

 * *Files identical despite different names*

### Comparing `snowpat-0.3.2/snowpat/SnowLens/plotting.py` & `snowpat-0.4.0/snowpat/SnowLense/plotting.py`

 * *Files identical despite different names*

### Comparing `snowpat-0.3.2/snowpat/SnowLens/snowlens.py` & `snowpat-0.4.0/snowpat/SnowLense/SnowLense.py`

 * *Files identical despite different names*

### Comparing `snowpat-0.3.2/snowpat/msgs.py` & `snowpat-0.4.0/snowpat/msgs.py`

 * *Files identical despite different names*

### Comparing `snowpat-0.3.2/snowpat/pysmet/MetaData.py` & `snowpat-0.4.0/snowpat/pysmet/MetaData.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,17 @@
                 isEqual = False
                 break
         return isEqual
 
     def __ne__(self, __value: object) -> bool:
         return not self.__eq__(__value)
 
+    def is_latlon(self):
+        return self.latitude is not None and self.longitude is not None
+
     @property
     def adjusted_dict(self):
         return {k: v for k, v in self.__dict__.items() if v is not None}
 
     def __str__(self):
         attributes = [
             ("Latitude", self.latitude),
```

### Comparing `snowpat-0.3.2/snowpat/pysmet/SMET.py` & `snowpat-0.4.0/snowpat/pysmet/SMET.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pandas as pd
 import numpy as np
 import os
 
 from .MetaData import *
-from .ACDD import ACDDMetadata
+from ..Utils.ACDD import ACDDMetadata
 
 from ..msgs import *
 
 class SMETFile:
     """A class used to represent a SMET file.
 
     Attributes:
@@ -19,25 +19,30 @@
         other_meta_data(dict): A dictionary that stores the other metadata of the SMET data.
     """
 
     def __init__(self, filename, read: bool, num_header_lines: int = None, fun:bool = False) -> None:
         if not os.path.isfile(filename) and read:
             raise FileNotFoundError(f"The file {filename} does not exist.")
 
+        self.fun = fun
+
         self.num_header_lines = num_header_lines if read else 1
         self.identifier = None if read else self.getIdentifier()
         self.optional_meta_data = None if read else dict()
         self.filename = filename
         self.data_header = None if read else ""
         self.acdd_meta_data = ACDDMetadata()
         self.other_meta_data = dict()
         self.meta_data = self.read_meta_data() if read else MetaData()
         self.data = self.read_data() if read else pd.DataFrame()
 
-        self.fun = fun
+        
+    @property
+    def all_meta_data(self):
+        return {**self.meta_data.combined_dict, **self.optional_meta_data.adjusted_dict, **self.acdd_meta_data.adjusted_dict, **self.other_meta_data}
 
     def read_data(self) -> pd.DataFrame:
         if not self.meta_data:
             print(
                 "Something went wrong reading MetaData, in the worst case please contact patrick.leibersperger@slf.ch"
             )
         if self.meta_data.fields:
@@ -305,19 +310,36 @@
         Returns:
             None
         """
 
         self.num_header_lines += 1
         self.identifier = f"SMET {version} ASCII"
 
-    def setData(self, data: pd.DataFrame):
+    def setData(self, data: pd.DataFrame, colnames: Optional[List[str]] = None) -> None:
+        """
+        Sets the data for the SMET object.
+
+        Args:
+            data (pd.DataFrame): The data to be set.
+            colnames (Optional[List[str]], optional): A list of column names to be used as fields in the MetaData. Defaults to None.
+
+        Raises:
+            ValueError: If `colnames` is not provided when the first field in the data is "0" or 0.
+
+        Returns:
+            None
+        """
         self.data = data
         fields = data.columns.to_list()
         if fields[0] == "0" or fields[0] == 0:
-            print("Please provide a meaningful list of fields in the MetaData")
+            if not colnames:
+                raise ValueError("Please provide a meaningful list of fields in the MetaData")
+            else:
+                print("Using fields: ", colnames)
+                self.meta_data.fields = colnames                
         else:
             print("Using fields: ", fields)
             self.meta_data.fields = fields
 
     def fromNumpy(
         self, data: np.ndarray, header: List[str], timestamp: Optional[List[str]] = None
     ) -> None:
```

### Comparing `snowpat-0.3.2/snowpat/pysmet/pySMET.py` & `snowpat-0.4.0/snowpat/pysmet/pymset.py`

 * *Files identical despite different names*

### Comparing `snowpat-0.3.2/snowpat/snowpackreader/Snowpack.py` & `snowpat-0.4.0/snowpat/snowpackreader/Snowpack.py`

 * *Files identical despite different names*

### Comparing `snowpat-0.3.2/snowpat/snowpackreader/snowpackreader.py` & `snowpat-0.4.0/snowpat/snowpackreader/snowpackreader.py`

 * *Files identical despite different names*

### Comparing `snowpat-0.3.2/PKG-INFO` & `snowpat-0.4.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 Metadata-Version: 2.1
 Name: snowpat
-Version: 0.3.2
+Version: 0.4.0
 Summary: 
 Author: leibersp
 Author-email: patrick.leibersperger@slf.ch
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: h5py (>=3.5,<4.0)
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
 Requires-Dist: numpy (>=1.26,<2.0)
 Requires-Dist: pandas (>=2,<3)
+Requires-Dist: xarray (>=2024.3.0,<2025.0.0)
 Description-Content-Type: text/markdown
 
 # SNOWPAT
 
-This is a toolbox for handling file formates most often used at SLF.
+This is a toolbox for handling file formates most often used in Snow Science.
 
 There are two submodules:
 pysmet: Used to read and write SMET files
 snowpackreader: Used to read SNOWPACK output files (.pro) and handle profiles easily (soon also with visualization)
-SnowLense: Plotting Framework for files that can be read with this module (SMET not yet available) ([see Documentation](https://snowpat-patrick-leibersperger-c7ec84b7d2c6ab235482777a3905915fe.gitlab-pages.wsl.ch/indexplot/))
+SnowLense: Plotting Framework for files that can be read with this module (SMET not yet available) ([see Documentation](http://patrick.leibersperger.gitlab-pages.wsl.ch/snowpat))
 
 ## News
 
+2024-05-05: A module to read and write iCSV files.
+
 2024-03-25: Installation via PyPi now possible
 
 2024-03-08: Plotting of Snow Profiles is available with SnowLense module
 
 2024-03-01: A simple merge function is now available to join to SMET Files: merge(SMETFile, override) and mergeFromFile(filename, override)
 
 ## Installation
@@ -52,14 +55,15 @@
 the --user option might be needed if you do not have admin rights.
 
 ### Upgrade
 
 If you already have an installation of Sowpat, that is out of date, run:
 
 ```bash
+pip install [--user] --upgrade snowpat
 pip install [--user] --upgrade git+https://gitlabext.wsl.ch/patrick.leibersperger/snowpat.git
 ```
 
 ### Manually
 
 Download the folder, and from the main directory run:
 
@@ -73,15 +77,15 @@
 pip install [--user] .
 ```
 
 ## Documentation
 
 The main documentation can be found under the respective module names, i.e. pySMET and SMET, as well as snowpackreader
 
-Extensive Documentation is available [online](http://snowpat-patrick-leibersperger-c7ec84b7d2c6ab235482777a3905915fe.gitlab-pages.wsl.ch/), it uses http, so you might get a privacy error in your browser;
+Extensive Documentation is available [online](http://patrick.leibersperger.gitlab-pages.wsl.ch/snowpat), it uses http, so you might get a privacy error in your browser;
 Or prepuilt in artifacts.zip, whic can be found in [job artifacts](https://gitlabext.wsl.ch/patrick.leibersperger/snowpat/-/artifacts): under (Number) files download the folder.
 
 If you download the zip folder just open index.html in your browser.
 
 Or you can build the docs yourself.
 
 ### MkDocs
@@ -111,14 +115,43 @@
 Please see the Documentation for more Examples and information on the full capabilities
 
 ```python
 from snowpat import pysmet as smet
 from snowpat import snowpackreader as spr
 ```
 
+### Examples iCSV
+
+```python
+from snowpat import icsv
+
+file = icsv.read(filename)
+data_pandas = file.data
+data_xarray = file.to_xarray()
+# metadata and fields can be accessed with get_attribute
+field_delimiter = file.metadata.get_attribute("field_delimiter")
+fields = file.fields.get_attribute("fields")
+# required keys will always be present, as a sanity check is done. Any other might return None if it is not available.
+# To see what metadata is available, you can print the information:
+file.info() # prints information about the whole file
+print(file.metadata) # prints information on the metadata only
+print(file.fields) # print information on the fields section
+
+# changing metadata
+file.metadata.set_attribute("field_delimiter", ":")
+
+# and for writing to an output again (if no output filename is provided, the given filename is used with an out flag):
+file.write(out_filename)
+
+# It is possible to convert SMET files to iCSV:
+from snowpat import pysmet as smet
+smet_file = smet.read(smet_filename)
+icsv_file = from_smet(smet_file)
+```
+
 ### Examples pySMET
 
 ```python
 from snowpat import pysmet as smet
 
 file = smet.read(filename)
 data_pandas = file.data
```

