# Comparing `tmp/antelope_interface-0.2.4.tar.gz` & `tmp/antelope_interface-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antelope_interface-0.2.4.tar", last modified: Thu Apr 18 05:36:15 2024, max compression
+gzip compressed data, was "antelope_interface-0.2.5.tar", last modified: Mon May  6 23:05:55 2024, max compression
```

## Comparing `antelope_interface-0.2.4.tar` & `antelope_interface-0.2.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 05:36:15.509111 antelope_interface-0.2.4/
--rw-r--r--   0 b          (500) b          (506)     1520 2020-05-28 23:57:28.000000 antelope_interface-0.2.4/LICENSE
--rw-r--r--   0 b          (500) b          (506)       48 2024-03-26 23:28:57.000000 antelope_interface-0.2.4/MANIFEST.in
--rw-r--r--   0 b          (500) b          (506)     2553 2024-04-18 05:36:15.509111 antelope_interface-0.2.4/PKG-INFO
--rw-r--r--   0 b          (500) b          (506)     1871 2024-04-11 07:45:58.000000 antelope_interface-0.2.4/README.md
--rw-r--r--   0 b          (500) b          (506)      864 2024-04-17 23:03:37.000000 antelope_interface-0.2.4/pyproject.toml
--rw-r--r--   0 b          (500) b          (506)       38 2024-04-18 05:36:15.509111 antelope_interface-0.2.4/setup.cfg
--rw-r--r--   0 b          (500) b          (506)     2327 2024-04-17 23:12:49.000000 antelope_interface-0.2.4/setup.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 05:36:15.505776 antelope_interface-0.2.4/src/
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 05:36:15.505776 antelope_interface-0.2.4/src/antelope/
--rw-r--r--   0 b          (500) b          (506)     7294 2024-04-18 05:03:09.000000 antelope_interface-0.2.4/src/antelope/__init__.py
--rw-r--r--   0 b          (500) b          (506)     7128 2023-07-21 21:50:52.000000 antelope_interface-0.2.4/src/antelope/exchanges_from_spreadsheet.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 05:36:15.505776 antelope_interface-0.2.4/src/antelope/flows/
--rw-r--r--   0 b          (500) b          (506)       89 2023-07-21 21:50:52.000000 antelope_interface-0.2.4/src/antelope/flows/__init__.py
--rw-r--r--   0 b          (500) b          (506)    12139 2024-04-18 05:19:57.000000 antelope_interface-0.2.4/src/antelope/flows/flow.py
--rw-r--r--   0 b          (500) b          (506)     3824 2024-04-18 05:10:28.000000 antelope_interface-0.2.4/src/antelope/flows/flow_interface.py
--rw-r--r--   0 b          (500) b          (506)    13903 2023-07-21 21:50:52.000000 antelope_interface-0.2.4/src/antelope/flows/openlca_locales.json
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 05:36:15.509111 antelope_interface-0.2.4/src/antelope/interfaces/
--rw-r--r--   0 b          (500) b          (506)      169 2024-04-17 23:12:49.000000 antelope_interface-0.2.4/src/antelope/interfaces/__init__.py
--rw-r--r--   0 b          (500) b          (506)     1769 2024-04-18 05:27:57.000000 antelope_interface-0.2.4/src/antelope/interfaces/abstract_query.py
--rw-r--r--   0 b          (500) b          (506)    10480 2023-07-21 21:50:52.000000 antelope_interface-0.2.4/src/antelope/interfaces/ibackground.py
--rw-r--r--   0 b          (500) b          (506)     4879 2024-04-18 05:31:46.000000 antelope_interface-0.2.4/src/antelope/interfaces/ibasic.py
--rw-r--r--   0 b          (500) b          (506)     4333 2024-04-18 05:28:30.000000 antelope_interface-0.2.4/src/antelope/interfaces/iconfigure.py
--rw-r--r--   0 b          (500) b          (506)     5164 2024-04-18 05:29:58.000000 antelope_interface-0.2.4/src/antelope/interfaces/iexchange.py
--rw-r--r--   0 b          (500) b          (506)     8785 2024-04-18 05:15:43.000000 antelope_interface-0.2.4/src/antelope/interfaces/iforeground.py
--rw-r--r--   0 b          (500) b          (506)     7432 2024-03-13 01:45:20.000000 antelope_interface-0.2.4/src/antelope/interfaces/iindex.py
--rw-r--r--   0 b          (500) b          (506)    13917 2024-04-18 05:17:15.000000 antelope_interface-0.2.4/src/antelope/interfaces/iquantity.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 05:36:15.509111 antelope_interface-0.2.4/src/antelope/models/
--rw-r--r--   0 b          (500) b          (506)    21308 2024-04-18 05:18:56.000000 antelope_interface-0.2.4/src/antelope/models/__init__.py
--rw-r--r--   0 b          (500) b          (506)     4683 2023-11-18 09:46:10.000000 antelope_interface-0.2.4/src/antelope/models/auth.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 05:36:15.509111 antelope_interface-0.2.4/src/antelope/refs/
--rw-r--r--   0 b          (500) b          (506)      185 2024-03-20 21:43:30.000000 antelope_interface-0.2.4/src/antelope/refs/__init__.py
--rw-r--r--   0 b          (500) b          (506)    14361 2024-04-18 05:17:38.000000 antelope_interface-0.2.4/src/antelope/refs/base.py
--rw-r--r--   0 b          (500) b          (506)     4702 2024-03-13 01:45:20.000000 antelope_interface-0.2.4/src/antelope/refs/catalog_ref.py
--rw-r--r--   0 b          (500) b          (506)     8424 2024-03-13 02:00:24.000000 antelope_interface-0.2.4/src/antelope/refs/exchange_ref.py
--rw-r--r--   0 b          (500) b          (506)     5179 2024-03-13 01:44:47.000000 antelope_interface-0.2.4/src/antelope/refs/flow_ref.py
--rw-r--r--   0 b          (500) b          (506)    12182 2024-04-11 07:44:14.000000 antelope_interface-0.2.4/src/antelope/refs/process_ref.py
--rw-r--r--   0 b          (500) b          (506)     9422 2024-04-18 05:26:09.000000 antelope_interface-0.2.4/src/antelope/refs/quantity_ref.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 05:36:15.509111 antelope_interface-0.2.4/src/antelope/refs/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2023-07-21 21:50:52.000000 antelope_interface-0.2.4/src/antelope/refs/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     1150 2023-07-21 21:50:52.000000 antelope_interface-0.2.4/src/antelope/refs/tests/test_flows.py
--rw-r--r--   0 b          (500) b          (506)     4717 2023-11-28 23:43:13.000000 antelope_interface-0.2.4/src/antelope/xdb_tokens.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 05:36:15.509111 antelope_interface-0.2.4/src/antelope_interface.egg-info/
--rw-r--r--   0 b          (500) b          (506)     2553 2024-04-18 05:36:15.000000 antelope_interface-0.2.4/src/antelope_interface.egg-info/PKG-INFO
--rw-r--r--   0 b          (500) b          (506)     1202 2024-04-18 05:36:15.000000 antelope_interface-0.2.4/src/antelope_interface.egg-info/SOURCES.txt
--rw-r--r--   0 b          (500) b          (506)        1 2024-04-18 05:36:15.000000 antelope_interface-0.2.4/src/antelope_interface.egg-info/dependency_links.txt
--rw-r--r--   0 b          (500) b          (506)       36 2024-04-18 05:36:15.000000 antelope_interface-0.2.4/src/antelope_interface.egg-info/requires.txt
--rw-r--r--   0 b          (500) b          (506)        9 2024-04-18 05:36:15.000000 antelope_interface-0.2.4/src/antelope_interface.egg-info/top_level.txt
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-05-06 23:05:55.728871 antelope_interface-0.2.5/
+-rw-r--r--   0 b          (500) b          (506)     1520 2020-05-28 23:57:28.000000 antelope_interface-0.2.5/LICENSE
+-rw-r--r--   0 b          (500) b          (506)       48 2024-03-26 23:28:57.000000 antelope_interface-0.2.5/MANIFEST.in
+-rw-r--r--   0 b          (500) b          (506)     2553 2024-05-06 23:05:55.728871 antelope_interface-0.2.5/PKG-INFO
+-rw-r--r--   0 b          (500) b          (506)     1871 2024-04-18 06:11:03.000000 antelope_interface-0.2.5/README.md
+-rw-r--r--   0 b          (500) b          (506)      864 2024-05-06 23:03:57.000000 antelope_interface-0.2.5/pyproject.toml
+-rw-r--r--   0 b          (500) b          (506)       38 2024-05-06 23:05:55.728871 antelope_interface-0.2.5/setup.cfg
+-rw-r--r--   0 b          (500) b          (506)     2440 2024-05-06 23:03:57.000000 antelope_interface-0.2.5/setup.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-05-06 23:05:55.725538 antelope_interface-0.2.5/src/
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-05-06 23:05:55.725538 antelope_interface-0.2.5/src/antelope/
+-rw-r--r--   0 b          (500) b          (506)     7294 2024-04-18 06:11:03.000000 antelope_interface-0.2.5/src/antelope/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     7226 2024-04-18 06:11:08.000000 antelope_interface-0.2.5/src/antelope/exchanges_from_spreadsheet.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-05-06 23:05:55.725538 antelope_interface-0.2.5/src/antelope/flows/
+-rw-r--r--   0 b          (500) b          (506)       89 2023-07-21 21:50:52.000000 antelope_interface-0.2.5/src/antelope/flows/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    12139 2024-04-18 06:11:03.000000 antelope_interface-0.2.5/src/antelope/flows/flow.py
+-rw-r--r--   0 b          (500) b          (506)     3824 2024-04-18 06:11:03.000000 antelope_interface-0.2.5/src/antelope/flows/flow_interface.py
+-rw-r--r--   0 b          (500) b          (506)    13903 2023-07-21 21:50:52.000000 antelope_interface-0.2.5/src/antelope/flows/openlca_locales.json
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-05-06 23:05:55.728871 antelope_interface-0.2.5/src/antelope/interfaces/
+-rw-r--r--   0 b          (500) b          (506)      169 2024-04-18 06:11:03.000000 antelope_interface-0.2.5/src/antelope/interfaces/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     1773 2024-04-18 06:11:03.000000 antelope_interface-0.2.5/src/antelope/interfaces/abstract_query.py
+-rw-r--r--   0 b          (500) b          (506)    10459 2024-05-06 19:13:21.000000 antelope_interface-0.2.5/src/antelope/interfaces/ibackground.py
+-rw-r--r--   0 b          (500) b          (506)     5302 2024-05-06 19:13:21.000000 antelope_interface-0.2.5/src/antelope/interfaces/ibasic.py
+-rw-r--r--   0 b          (500) b          (506)     4333 2024-04-18 06:11:03.000000 antelope_interface-0.2.5/src/antelope/interfaces/iconfigure.py
+-rw-r--r--   0 b          (500) b          (506)     5164 2024-04-18 06:11:03.000000 antelope_interface-0.2.5/src/antelope/interfaces/iexchange.py
+-rw-r--r--   0 b          (500) b          (506)     8785 2024-04-18 06:11:03.000000 antelope_interface-0.2.5/src/antelope/interfaces/iforeground.py
+-rw-r--r--   0 b          (500) b          (506)     7432 2024-03-13 01:45:20.000000 antelope_interface-0.2.5/src/antelope/interfaces/iindex.py
+-rw-r--r--   0 b          (500) b          (506)    13917 2024-04-18 06:11:03.000000 antelope_interface-0.2.5/src/antelope/interfaces/iquantity.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-05-06 23:05:55.728871 antelope_interface-0.2.5/src/antelope/models/
+-rw-r--r--   0 b          (500) b          (506)    21397 2024-04-23 18:25:18.000000 antelope_interface-0.2.5/src/antelope/models/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     4683 2023-11-18 09:46:10.000000 antelope_interface-0.2.5/src/antelope/models/auth.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-05-06 23:05:55.728871 antelope_interface-0.2.5/src/antelope/refs/
+-rw-r--r--   0 b          (500) b          (506)      185 2024-03-20 21:43:30.000000 antelope_interface-0.2.5/src/antelope/refs/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    14361 2024-04-18 06:11:03.000000 antelope_interface-0.2.5/src/antelope/refs/base.py
+-rw-r--r--   0 b          (500) b          (506)     4702 2024-03-13 01:45:20.000000 antelope_interface-0.2.5/src/antelope/refs/catalog_ref.py
+-rw-r--r--   0 b          (500) b          (506)     8424 2024-03-13 02:00:24.000000 antelope_interface-0.2.5/src/antelope/refs/exchange_ref.py
+-rw-r--r--   0 b          (500) b          (506)     5179 2024-03-13 01:44:47.000000 antelope_interface-0.2.5/src/antelope/refs/flow_ref.py
+-rw-r--r--   0 b          (500) b          (506)    12319 2024-05-06 19:13:21.000000 antelope_interface-0.2.5/src/antelope/refs/process_ref.py
+-rw-r--r--   0 b          (500) b          (506)     9422 2024-04-18 06:11:03.000000 antelope_interface-0.2.5/src/antelope/refs/quantity_ref.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-05-06 23:05:55.728871 antelope_interface-0.2.5/src/antelope/refs/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2023-07-21 21:50:52.000000 antelope_interface-0.2.5/src/antelope/refs/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     1150 2023-07-21 21:50:52.000000 antelope_interface-0.2.5/src/antelope/refs/tests/test_flows.py
+-rw-r--r--   0 b          (500) b          (506)     4717 2023-11-28 23:43:13.000000 antelope_interface-0.2.5/src/antelope/xdb_tokens.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-05-06 23:05:55.728871 antelope_interface-0.2.5/src/antelope_interface.egg-info/
+-rw-r--r--   0 b          (500) b          (506)     2553 2024-05-06 23:05:55.000000 antelope_interface-0.2.5/src/antelope_interface.egg-info/PKG-INFO
+-rw-r--r--   0 b          (500) b          (506)     1202 2024-05-06 23:05:55.000000 antelope_interface-0.2.5/src/antelope_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 b          (500) b          (506)        1 2024-05-06 23:05:55.000000 antelope_interface-0.2.5/src/antelope_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 b          (500) b          (506)       36 2024-05-06 23:05:55.000000 antelope_interface-0.2.5/src/antelope_interface.egg-info/requires.txt
+-rw-r--r--   0 b          (500) b          (506)        9 2024-05-06 23:05:55.000000 antelope_interface-0.2.5/src/antelope_interface.egg-info/top_level.txt
```

### Comparing `antelope_interface-0.2.4/LICENSE` & `antelope_interface-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.4/PKG-INFO` & `antelope_interface-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antelope_interface
-Version: 0.2.4
+Version: 0.2.5
 Summary: A common interface for accessing LCA data
 Author-email: Brandon Kuczenski <bkuczenski@ucsb.edu>
 License: BSD-3-Clause
 Keywords: one,two
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `antelope_interface-0.2.4/README.md` & `antelope_interface-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.4/pyproject.toml` & `antelope_interface-0.2.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -18,11 +18,11 @@
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering"
 ]
 dependencies = ["synonym_dict >= 0.2.4", "pydantic >= 2.5.0"]
-version = "0.2.4"
+version = "0.2.5"
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `antelope_interface-0.2.4/setup.py` & `antelope_interface-0.2.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from setuptools import setup
 
 setup()
 
 
 """
 Version History:
+0.2.5 2024/05/06 - bg_lcia() becomes a basic interface route; sys_lcia() is the fully-featured background route
+
 0.2.4 2024/04/17 - split out BasicInterface from AbstractQuery. 
                    abandon setup.py except for this changelog.
                    Redesign ExteriorFlow to have maybe a little bit more logic
                    First pass at API documentation
 
 0.2.3.2 2024/03/26 move to src layout
```

### Comparing `antelope_interface-0.2.4/src/antelope/__init__.py` & `antelope_interface-0.2.5/src/antelope/__init__.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.4/src/antelope/exchanges_from_spreadsheet.py` & `antelope_interface-0.2.5/src/antelope/exchanges_from_spreadsheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """
 This module provides a routine that generates a list of exchange refs from a properly formatted spreadsheet
 """
+
 from .refs import CatalogRef, ExchangeRef
 from .interfaces import check_direction
 
 
 class ValueIsBalance(Exception):
+    """
+    Used to signal when an exchange is reached that is designated as a balance.
+    """
     pass
 
 
 class TermDictDeprecated(Exception):
     """
     Exchanges are allowed to specify terminations, including context, compartment, defaultprovider, activitylinkid,
     or target. However, the exchanges-from-spreadsheet code is not allowed to apply any interpretation or mapping
@@ -89,14 +93,15 @@
     Requirements for the sheet-like object: XlrdLike / xls_tools
      - name property that returns a string
      - nrows property that reports the number of rows
      - row(index) function that returns an ordered list of entries for the specified index (0-indexed).
      - row(0) returns a header list
      - row(1) is the process's reference flow
      - subsequent rows are dependent flows
+
      !TODO: support multiple references with is_ref or is_reference field
 
     "entries" in the row() return must be "cell-like":
      - value property that returns the cell's value
      - ctype property [*not currently used*] that corresponds with xlrd.sheet.Cell:
         0=empty, 1=text, 2=number, 3=date, 4=boolean, 5=error, 6=blank
         (not clear what the difference is between empty and blank)
```

### Comparing `antelope_interface-0.2.4/src/antelope/flows/flow.py` & `antelope_interface-0.2.5/src/antelope/flows/flow.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.4/src/antelope/flows/flow_interface.py` & `antelope_interface-0.2.5/src/antelope/flows/flow_interface.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.4/src/antelope/flows/openlca_locales.json` & `antelope_interface-0.2.5/src/antelope/flows/openlca_locales.json`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.4/src/antelope/interfaces/abstract_query.py` & `antelope_interface-0.2.5/src/antelope/interfaces/abstract_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,16 @@
     """
     :meta exclude:
     """
     pass
 
 
 class AbstractQuery(object):
-    """ Not-quite-abstract base class for executing queries
+    """
+    Not-quite-abstract base class for executing queries
 
     Query implementation must provide:
      - origin (property)
      - _iface (generator: itype)
      - _tm (property) a TermManager
     """
     _validated = None
```

### Comparing `antelope_interface-0.2.4/src/antelope/interfaces/ibackground.py` & `antelope_interface-0.2.5/src/antelope/interfaces/ibackground.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 database.
 
 More plugins are yet imagined.
 """
 
 from .abstract_query import AbstractQuery
 from ..refs import ExchangeRef
-from itertools import chain
 
 
 class BackgroundRequired(Exception):
     pass
 
 
 _interface = 'background'
@@ -132,15 +131,15 @@
         :param ref_flow:
         :return:
         """
         return self._perform_query(_interface, 'lci', BackgroundRequired,
                                    process, ref_flow=ref_flow, **kwargs)
 
     def _make_sys_lci_exchange(self, x):
-        return ExchangeRef(self.get(x.process), self.make_ref(x.flow), x.direction, value=x.value,
+        return ExchangeRef(self.make_ref(x.process), self.make_ref(x.flow), x.direction, value=x.value,
                            termination=x.termination, comment='SYS LCI', is_reference=False)
 
     def sys_lci(self, demand, **kwargs):
         """
         Perform LCI on an arbitrary demand vector, which should be supplied as an iterable of UnallocatedExchange
         models whose terminations can be found in the background database.
 
@@ -156,25 +155,25 @@
         :param demand: an iterable of exchanges with terminations that can be found in the background database.
         :param kwargs:
         :return:
         """
         for i in self._perform_query(_interface, 'sys_lci', BackgroundRequired, demand, **kwargs):
             yield self._make_sys_lci_exchange(i)
 
-    def bg_lcia(self, process, query_qty, observed=None, ref_flow=None, **kwargs):
+    def sys_lcia(self, process, query_qty, observed=None, ref_flow=None, **kwargs):
         """
 
         :param process:
         :param query_qty:
         :param observed:
         :param ref_flow:
         :param kwargs:
         :return:
         """
-        return self._perform_query(_interface, 'bg_lcia', BackgroundRequired,
+        return self._perform_query(_interface, 'sys_lcia', BackgroundRequired,
                                    process, query_qty, observed=observed, ref_flow=ref_flow, **kwargs)
 
     '''
     Methods requiring a partial ordering (implemented by antelope_background)
     '''
     def foreground_flows(self, search=None, **kwargs):
         """
```

### Comparing `antelope_interface-0.2.4/src/antelope/interfaces/ibasic.py` & `antelope_interface-0.2.5/src/antelope/interfaces/ibasic.py`

 * *Files 7% similar despite different names*

```diff
@@ -138,8 +138,20 @@
         """
 
         try:
             return self._perform_query('basic', 'is_lcia_engine', TypeError, **kwargs)
         except TypeError:
             return False
 
+    def bg_lcia(self, process, query_qty=None, ref_flow=None, **kwargs):
+        """
+
+        :param process:
+        :param query_qty: if omitted, a catalog may select a default LCIA method
+        :param ref_flow:
+        :param kwargs:
+        :return:
+        """
+        return self._perform_query('basic', 'bg_lcia', BasicRequired,
+                                   process, query_qty, ref_flow=ref_flow, **kwargs)
+
```

### Comparing `antelope_interface-0.2.4/src/antelope/interfaces/iconfigure.py` & `antelope_interface-0.2.5/src/antelope/interfaces/iconfigure.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.4/src/antelope/interfaces/iexchange.py` & `antelope_interface-0.2.5/src/antelope/interfaces/iexchange.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.4/src/antelope/interfaces/iforeground.py` & `antelope_interface-0.2.5/src/antelope/interfaces/iforeground.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.4/src/antelope/interfaces/iindex.py` & `antelope_interface-0.2.5/src/antelope/interfaces/iindex.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.4/src/antelope/interfaces/iquantity.py` & `antelope_interface-0.2.5/src/antelope/interfaces/iquantity.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.4/src/antelope/models/__init__.py` & `antelope_interface-0.2.5/src/antelope/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,14 +283,18 @@
     """
     An ExteriorFlow is essentially a row in the LCI Environment `B` matrix. It consists of a directed flow,
     enhanced with a context. Now I know a flow already has a context, but (a) context is not required for a flow and
     (b) flows can be terminated to contexts other than their 'default'
     """
     context: List[str]
 
+    @property
+    def termination(self):
+        return self.context
+
     @classmethod
     def from_background(cls, flow, direction, context):
         if hasattr(context, 'entity_type'):
             if context.entity_type == 'context':
                 cx = context.as_list()
             else:
                 raise TypeError('supplied Context %s (type %s)' % (context, context.entity_type))
@@ -337,15 +341,15 @@
 
 
 class ReferenceExchange(Exchange):
     is_reference: bool = True
     termination: None
 
     @classmethod
-    def from_exchange(cls, x):
+    def from_exchange(cls, x, **kwargs):
         if x.termination is not None:
             cx = list(x.termination)
         else:
             cx = None
         return cls(origin=x.process.origin, process=x.process.external_ref, flow=FlowEntity.from_flow(x.flow),
                    direction=x.direction, termination=None, context=cx, type=x.type, comment=x.comment, str=str(x))
 
@@ -425,18 +429,19 @@
 
 def generate_pydantic_inventory(xs, mode=None, values=False, ref_flow=None):
     """
     Not currently used
 
     :param xs: iterable of exchanges
     :param mode: [None] whether to filter the exchanges by type. could be one of:
-     None: generate all exchanges
-     'interior'
-     'exterior'
-     'cutoff'
+     - None: generate all exchanges
+     - 'interior'
+     - 'exterior'
+     - 'cutoff'
+
     :param values: (bool) [False] whether to include exchange values.
     :param ref_flow: (ignored if values=False) the reference flow with which the exchange value was computed. If None,
      this implies the exchange reports un-allocated exchange values
     :return:
     """
     if hasattr(ref_flow, 'entity_type'):
         if ref_flow.entity_type == 'flow':
```

### Comparing `antelope_interface-0.2.4/src/antelope/models/auth.py` & `antelope_interface-0.2.5/src/antelope/models/auth.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.4/src/antelope/refs/base.py` & `antelope_interface-0.2.5/src/antelope/refs/base.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.4/src/antelope/refs/catalog_ref.py` & `antelope_interface-0.2.5/src/antelope/refs/catalog_ref.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.4/src/antelope/refs/exchange_ref.py` & `antelope_interface-0.2.5/src/antelope/refs/exchange_ref.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.4/src/antelope/refs/flow_ref.py` & `antelope_interface-0.2.5/src/antelope/refs/flow_ref.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.4/src/antelope/refs/process_ref.py` & `antelope_interface-0.2.5/src/antelope/refs/process_ref.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,8 +311,11 @@
         :param lcia_qty: should be a quantity ref (or qty), not an external ID
         :param observed: see unobserved_lci
         :param ref_flow:
         :param kwargs:
         :return:
         """
         ref_flow = self._use_ref_exch(ref_flow)
-        return self._query.bg_lcia(self.external_ref, lcia_qty, observed=observed, ref_flow=ref_flow, **kwargs)
+        if observed:
+            return self._query.sys_lcia(self.external_ref, lcia_qty, observed=observed, ref_flow=ref_flow, **kwargs)
+        else:
+            return self._query.bg_lcia(self.external_ref, lcia_qty, ref_flow=ref_flow, **kwargs)
```

### Comparing `antelope_interface-0.2.4/src/antelope/refs/quantity_ref.py` & `antelope_interface-0.2.5/src/antelope/refs/quantity_ref.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.4/src/antelope/refs/tests/test_flows.py` & `antelope_interface-0.2.5/src/antelope/refs/tests/test_flows.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.4/src/antelope/xdb_tokens.py` & `antelope_interface-0.2.5/src/antelope/xdb_tokens.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.4/src/antelope_interface.egg-info/PKG-INFO` & `antelope_interface-0.2.5/src/antelope_interface.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antelope_interface
-Version: 0.2.4
+Version: 0.2.5
 Summary: A common interface for accessing LCA data
 Author-email: Brandon Kuczenski <bkuczenski@ucsb.edu>
 License: BSD-3-Clause
 Keywords: one,two
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `antelope_interface-0.2.4/src/antelope_interface.egg-info/SOURCES.txt` & `antelope_interface-0.2.5/src/antelope_interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

