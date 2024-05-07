# Comparing `tmp/pyrcv-1.0.2.tar.gz` & `tmp/pyrcv-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrcv-1.0.2.tar", last modified: Fri Jan 12 20:41:59 2024, max compression
+gzip compressed data, was "pyrcv-1.0.3.tar", last modified: Tue May  7 17:57:24 2024, max compression
```

## Comparing `pyrcv-1.0.2.tar` & `pyrcv-1.0.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 20:41:59.042105 pyrcv-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-01-12 20:41:43.000000 pyrcv-1.0.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-12 20:41:43.000000 pyrcv-1.0.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-01-12 20:41:43.000000 pyrcv-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-01-12 20:41:43.000000 pyrcv-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-01-12 20:41:59.042105 pyrcv-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-01-12 20:41:43.000000 pyrcv-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 20:41:59.038105 pyrcv-1.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-01-12 20:41:43.000000 pyrcv-1.0.2/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)     5323 2024-01-12 20:41:43.000000 pyrcv-1.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-12 20:41:43.000000 pyrcv-1.0.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-12 20:41:43.000000 pyrcv-1.0.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-01-12 20:41:43.000000 pyrcv-1.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-01-12 20:41:43.000000 pyrcv-1.0.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-01-12 20:41:43.000000 pyrcv-1.0.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-01-12 20:41:43.000000 pyrcv-1.0.2/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-01-12 20:41:43.000000 pyrcv-1.0.2/docs/pyrcv.rst
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-12 20:41:43.000000 pyrcv-1.0.2/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-01-12 20:41:43.000000 pyrcv-1.0.2/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-12 20:41:43.000000 pyrcv-1.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 20:41:59.042105 pyrcv-1.0.2/pyrcv/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-01-12 20:41:43.000000 pyrcv-1.0.2/pyrcv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-01-12 20:41:43.000000 pyrcv-1.0.2/pyrcv/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    11621 2024-01-12 20:41:43.000000 pyrcv-1.0.2/pyrcv/pyrcv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-01-12 20:41:43.000000 pyrcv-1.0.2/pyrcv/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-01-12 20:41:43.000000 pyrcv-1.0.2/pyrcv/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-01-12 20:41:43.000000 pyrcv-1.0.2/pyrcv/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 20:41:59.042105 pyrcv-1.0.2/pyrcv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-01-12 20:41:58.000000 pyrcv-1.0.2/pyrcv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-01-12 20:41:59.000000 pyrcv-1.0.2/pyrcv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 20:41:58.000000 pyrcv-1.0.2/pyrcv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-12 20:41:58.000000 pyrcv-1.0.2/pyrcv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 20:41:58.000000 pyrcv-1.0.2/pyrcv.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-12 20:41:58.000000 pyrcv-1.0.2/pyrcv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-12 20:41:58.000000 pyrcv-1.0.2/pyrcv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-01-12 20:41:59.046105 pyrcv-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-01-12 20:41:43.000000 pyrcv-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 20:41:59.042105 pyrcv-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-12 20:41:43.000000 pyrcv-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-01-12 20:41:43.000000 pyrcv-1.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-01-12 20:41:43.000000 pyrcv-1.0.2/tests/test_pyrcv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-01-12 20:41:43.000000 pyrcv-1.0.2/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-01-12 20:41:43.000000 pyrcv-1.0.2/tests/test_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 20:41:59.042105 pyrcv-1.0.2/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-01-12 20:41:43.000000 pyrcv-1.0.2/tests/testdata/transform_float_testdata.csv
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-01-12 20:41:43.000000 pyrcv-1.0.2/tests/testdata/transform_indeterminate_testdata.csv
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-01-12 20:41:43.000000 pyrcv-1.0.2/tests/testdata/transform_int_testdata.csv
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-01-12 20:41:43.000000 pyrcv-1.0.2/tests/testdata/transform_testdata.csv
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-01-12 20:41:43.000000 pyrcv-1.0.2/tests/testdata/transform_weighted_testdata.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-01-12 20:41:43.000000 pyrcv-1.0.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:57:24.376400 pyrcv-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-07 17:57:04.000000 pyrcv-1.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-07 17:57:04.000000 pyrcv-1.0.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-07 17:57:04.000000 pyrcv-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-07 17:57:04.000000 pyrcv-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-07 17:57:24.376400 pyrcv-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-07 17:57:04.000000 pyrcv-1.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:57:24.372400 pyrcv-1.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-07 17:57:04.000000 pyrcv-1.0.3/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5323 2024-05-07 17:57:04.000000 pyrcv-1.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 17:57:04.000000 pyrcv-1.0.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 17:57:04.000000 pyrcv-1.0.3/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-07 17:57:04.000000 pyrcv-1.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-07 17:57:04.000000 pyrcv-1.0.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-07 17:57:04.000000 pyrcv-1.0.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-07 17:57:04.000000 pyrcv-1.0.3/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-07 17:57:04.000000 pyrcv-1.0.3/docs/pyrcv.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-07 17:57:04.000000 pyrcv-1.0.3/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-07 17:57:04.000000 pyrcv-1.0.3/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-07 17:57:04.000000 pyrcv-1.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:57:24.372400 pyrcv-1.0.3/pyrcv/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-07 17:57:04.000000 pyrcv-1.0.3/pyrcv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-07 17:57:04.000000 pyrcv-1.0.3/pyrcv/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11622 2024-05-07 17:57:04.000000 pyrcv-1.0.3/pyrcv/pyrcv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-07 17:57:04.000000 pyrcv-1.0.3/pyrcv/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-07 17:57:04.000000 pyrcv-1.0.3/pyrcv/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-05-07 17:57:04.000000 pyrcv-1.0.3/pyrcv/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:57:24.372400 pyrcv-1.0.3/pyrcv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-07 17:57:24.000000 pyrcv-1.0.3/pyrcv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-07 17:57:24.000000 pyrcv-1.0.3/pyrcv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 17:57:24.000000 pyrcv-1.0.3/pyrcv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 17:57:24.000000 pyrcv-1.0.3/pyrcv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 17:57:24.000000 pyrcv-1.0.3/pyrcv.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-07 17:57:24.000000 pyrcv-1.0.3/pyrcv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 17:57:24.000000 pyrcv-1.0.3/pyrcv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-07 17:57:24.376400 pyrcv-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-07 17:57:04.000000 pyrcv-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:57:24.376400 pyrcv-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-07 17:57:04.000000 pyrcv-1.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-07 17:57:04.000000 pyrcv-1.0.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8613 2024-05-07 17:57:04.000000 pyrcv-1.0.3/tests/test_pyrcv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-07 17:57:04.000000 pyrcv-1.0.3/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-07 17:57:04.000000 pyrcv-1.0.3/tests/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:57:24.376400 pyrcv-1.0.3/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-07 17:57:04.000000 pyrcv-1.0.3/tests/testdata/transform_float_testdata.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-07 17:57:04.000000 pyrcv-1.0.3/tests/testdata/transform_indeterminate_testdata.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-07 17:57:04.000000 pyrcv-1.0.3/tests/testdata/transform_int_testdata.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-07 17:57:04.000000 pyrcv-1.0.3/tests/testdata/transform_testdata.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-07 17:57:04.000000 pyrcv-1.0.3/tests/testdata/transform_weighted_testdata.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-07 17:57:04.000000 pyrcv-1.0.3/tests/utils.py
```

### Comparing `pyrcv-1.0.2/CONTRIBUTING.rst` & `pyrcv-1.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyrcv-1.0.2/LICENSE` & `pyrcv-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrcv-1.0.2/PKG-INFO` & `pyrcv-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrcv
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python API for adjudicating single transferable vote elections.  Also contains basic web server to adjudicate results in CSV format.
 Home-page: https://github.com/chrisroat/pyrcv
 Author: Chris Roat
 Author-email: chris.roat@gmail.com
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/chrisroat/pyrcv/issues
 Project-URL: Production Server, https://www.pyrcv.org
```

### Comparing `pyrcv-1.0.2/README.rst` & `pyrcv-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `pyrcv-1.0.2/docs/Makefile` & `pyrcv-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyrcv-1.0.2/docs/conf.py` & `pyrcv-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyrcv-1.0.2/docs/index.rst` & `pyrcv-1.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyrcv-1.0.2/docs/installation.rst` & `pyrcv-1.0.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pyrcv-1.0.2/docs/make.bat` & `pyrcv-1.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyrcv-1.0.2/docs/pyrcv.rst` & `pyrcv-1.0.3/docs/pyrcv.rst`

 * *Files identical despite different names*

### Comparing `pyrcv-1.0.2/docs/usage.rst` & `pyrcv-1.0.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `pyrcv-1.0.2/pyrcv/cli.py` & `pyrcv-1.0.3/pyrcv/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Script to tabulate single-transferable vote results from a csv file.
 
 The format required is parsed in the function
 :func:`pyrcv.transform.parse_google_form_csv`.
 """
+
 from typing import TextIO
 
 import click
 
 import pyrcv
 from pyrcv import RoundMode
```

### Comparing `pyrcv-1.0.2/pyrcv/pyrcv.py` & `pyrcv-1.0.3/pyrcv/pyrcv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Implementation of Single Transferable Vote."""
+
 from __future__ import annotations
 
 import collections
 import enum
 import itertools
 
 import numpy as np
```

### Comparing `pyrcv-1.0.2/pyrcv/transform.py` & `pyrcv-1.0.3/pyrcv/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities to convert a csv format from Google Forms into pyrcv standard format."""
+
 import re
 from typing import Tuple
 
 import numpy as np
 import pandas as pd
 from pandas._typing import FilePath, ReadCsvBuffer
```

### Comparing `pyrcv-1.0.2/pyrcv/types.py` & `pyrcv-1.0.3/pyrcv/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Common types used in :mod:`pyrcv`."""
+
 from dataclasses import dataclass
 
 from icontract import invariant
 
 
 class PyRcvError(Exception):
     """Error in pyrcv."""
```

### Comparing `pyrcv-1.0.2/pyrcv/viz.py` & `pyrcv-1.0.3/pyrcv/viz.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities for creating Sankey plots of RCV results."""
+
 from typing import Tuple
 
 import pandas as pd
 import plotly.graph_objects as go
 from plotly.colors import qualitative
 
 from pyrcv import RaceResult
```

### Comparing `pyrcv-1.0.2/pyrcv.egg-info/PKG-INFO` & `pyrcv-1.0.3/pyrcv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrcv
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python API for adjudicating single transferable vote elections.  Also contains basic web server to adjudicate results in CSV format.
 Home-page: https://github.com/chrisroat/pyrcv
 Author: Chris Roat
 Author-email: chris.roat@gmail.com
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/chrisroat/pyrcv/issues
 Project-URL: Production Server, https://www.pyrcv.org
```

### Comparing `pyrcv-1.0.2/pyrcv.egg-info/SOURCES.txt` & `pyrcv-1.0.3/pyrcv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrcv-1.0.2/setup.cfg` & `pyrcv-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyrcv
-version = 1.0.2
+version = 1.0.3
 author = Chris Roat
 author_email = chris.roat@gmail.com
 description = Python API for adjudicating single transferable vote elections.  Also contains basic web server to adjudicate results in CSV format.
 license = GNU General Public License v3
 license_files = LICENSE
 long_description = file: README.rst
 long_description_content_type = text/x-rst
```

### Comparing `pyrcv-1.0.2/tests/test_pyrcv.py` & `pyrcv-1.0.3/tests/test_pyrcv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for `pyrcv` package."""
+
 import pathlib
 
 import pytest
 from click.testing import CliRunner
 from numpy.testing import assert_equal
 
 import pyrcv
```

### Comparing `pyrcv-1.0.2/tests/test_transform.py` & `pyrcv-1.0.3/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `pyrcv-1.0.2/tests/test_viz.py` & `pyrcv-1.0.3/tests/test_viz.py`

 * *Files identical despite different names*

### Comparing `pyrcv-1.0.2/tests/utils.py` & `pyrcv-1.0.3/tests/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities for testing."""
+
 from numpy.testing import assert_allclose, assert_equal
 
 
 def assert_race_equal(actual, desired):
     assert len(actual.rounds) == len(desired.rounds)
     for r, (ar, dr) in enumerate(zip(actual.rounds, desired.rounds)):
         assert_round_equal(ar, dr, err_msg=f"round {r}")
```

