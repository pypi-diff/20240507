# Comparing `tmp/ba_tsconcat-0.1.2.tar.gz` & `tmp/ba_tsconcat-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ba_tsconcat-0.1.2.tar", max compression
+gzip compressed data, was "ba_tsconcat-0.1.3.tar", max compression
```

## Comparing `ba_tsconcat-0.1.2.tar` & `ba_tsconcat-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    26190 2024-05-01 16:03:10.204197 ba_tsconcat-0.1.2/LICENSE
--rw-r--r--   0        0        0     2779 2024-05-01 16:03:10.204197 ba_tsconcat-0.1.2/README.md
--rw-r--r--   0        0        0     1778 2024-05-01 16:03:10.204197 ba_tsconcat-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      262 2024-05-01 16:03:10.204197 ba_tsconcat-0.1.2/src/tsconcat/__init__.py
--rw-r--r--   0        0        0     6511 2024-05-01 16:03:10.204197 ba_tsconcat-0.1.2/src/tsconcat/cli.py
--rw-r--r--   0        0        0     1565 2024-05-01 16:03:10.204197 ba_tsconcat-0.1.2/src/tsconcat/concat.py
--rw-r--r--   0        0        0     2623 2024-05-01 16:03:10.204197 ba_tsconcat-0.1.2/src/tsconcat/pretreeprint.py
--rw-r--r--   0        0        0     2829 2024-05-01 16:03:10.204197 ba_tsconcat-0.1.2/src/tsconcat/utils.py
--rw-r--r--   0        0        0     3494 1970-01-01 00:00:00.000000 ba_tsconcat-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    26190 2024-05-07 14:26:17.088379 ba_tsconcat-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2779 2024-05-07 14:26:17.088379 ba_tsconcat-0.1.3/README.md
+-rw-r--r--   0        0        0     1776 2024-05-07 14:26:17.088379 ba_tsconcat-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      262 2024-05-07 14:26:17.088379 ba_tsconcat-0.1.3/src/tsconcat/__init__.py
+-rw-r--r--   0        0        0      608 2024-05-07 14:26:17.088379 ba_tsconcat-0.1.3/src/tsconcat/b2t_columns.py
+-rw-r--r--   0        0        0     7470 2024-05-07 14:26:17.088379 ba_tsconcat-0.1.3/src/tsconcat/cli.py
+-rw-r--r--   0        0        0     1565 2024-05-07 14:26:17.088379 ba_tsconcat-0.1.3/src/tsconcat/concat.py
+-rw-r--r--   0        0        0     2623 2024-05-07 14:26:17.088379 ba_tsconcat-0.1.3/src/tsconcat/pretreeprint.py
+-rw-r--r--   0        0        0     2962 2024-05-07 14:26:17.088379 ba_tsconcat-0.1.3/src/tsconcat/utils.py
+-rw-r--r--   0        0        0     3492 1970-01-01 00:00:00.000000 ba_tsconcat-0.1.3/PKG-INFO
```

### Comparing `ba_tsconcat-0.1.2/LICENSE` & `ba_tsconcat-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ba_tsconcat-0.1.2/README.md` & `ba_tsconcat-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ba_tsconcat-0.1.2/pyproject.toml` & `ba_tsconcat-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "ba-tsconcat"
-version = "0.1.2"
+version = "0.1.3"
 description = "BIDS App and Python library for concatenating MRI time series."
 authors = ["CMI DAIR Center <florian.rupprecht@childmind.org>"]
 license = "LGPL-2.1"
 readme = "README.md"
 packages = [{include = "tsconcat", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-bids2table = "^0.1.0b0"
 nibabel = "^5.2.0"
 numpy = "^1.26.3"
 pandas = ">1.0"
 rich = "^13.4.2"
+bids2table = "^0.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 mypy = "^1.8.0"
 pre-commit = "^3.6.0"
 pytest-cov = "^4.1.0"
 ruff = "^0.1.8"
```

### Comparing `ba_tsconcat-0.1.2/src/tsconcat/concat.py` & `ba_tsconcat-0.1.3/src/tsconcat/concat.py`

 * *Files identical despite different names*

### Comparing `ba_tsconcat-0.1.2/src/tsconcat/pretreeprint.py` & `ba_tsconcat-0.1.3/src/tsconcat/pretreeprint.py`

 * *Files identical despite different names*

### Comparing `ba_tsconcat-0.1.2/src/tsconcat/utils.py` & `ba_tsconcat-0.1.3/src/tsconcat/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import time
 from contextlib import contextmanager
 from typing import Generator, List
 
 import bids2table.table
 import pandas as pd
 
+from tsconcat.b2t_columns import B2tColumn
+
 
 @contextmanager
 def timeprint(title: str) -> Generator[None, None, None]:
     """Context manager to print the time elapsed between entering and exiting the context.
 
     Args:
         title: Title to be printed before and after the context.
@@ -41,53 +43,53 @@
     )
     parser.add_argument(
         "output_dir",
         action="store",
         type=pl.Path,
         help="Output BIDS folder path.",
     )
-    parser.add_argument("analysis_level", choices=["group"], help='Processing stage, must be "group".')
+    parser.add_argument("analysis_level", default="group", choices=["group"], help='Processing stage, must be "group".')
     return parser
 
 
 def file_paths_from_b2table(df: pd.DataFrame, include_sidecars: bool = False, inplace: bool = False) -> List[pl.Path]:
     """Generate list of filepaths from bids2table dataframe."""
     # b2t crashes if sidecar is not None
     if not inplace:
         df = df.copy()
-    df["meta__json"] = None
+    df[B2tColumn.MetaJson] = None
 
     paths = list(df.apply(func=lambda row: bids2table.table.join_bids_path(row), axis=1).values)
 
     if include_sidecars:
         sidecar_paths = list(
             df.apply(
-                func=lambda row: bids2table.table.join_bids_path({**row, "ext": ".json"}),
+                func=lambda row: bids2table.table.join_bids_path({**row, B2tColumn.FileExtension: ".json"}),
                 axis=1,
             ).values
         )
         return paths + sidecar_paths
 
     return paths
 
 
 def file_path_from_b2table_row(row: pd.Series, inplace: bool = False, sidecar: bool = False) -> pl.Path:
     """Generate list of filepaths from bids2table dataframe."""
     # b2t crashes if sidecar is not None
     if not inplace:
         row = row.copy()
-    row["meta__json"] = None
+    row[B2tColumn.MetaJson] = None
 
     if sidecar:
-        row = {**row, "ext": ".json"}
+        row = {**row, B2tColumn.FileExtension: ".json"}
 
     return bids2table.table.join_bids_path(row)
 
 
 def sidecar_path_from_b2table_row(row: pd.Series, inplace: bool = False) -> pl.Path:
     """Generate list of filepaths from bids2table dataframe."""
     # b2t crashes if sidecar is not None
     if not inplace:
         row = row.copy()
-    row["meta__json"] = None
+    row[B2tColumn.MetaJson] = None
 
-    return bids2table.table.join_bids_path({**row, "ext": ".json"})
+    return bids2table.table.join_bids_path({**row, B2tColumn.FileExtension: ".json"})
```

### Comparing `ba_tsconcat-0.1.2/PKG-INFO` & `ba_tsconcat-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: ba-tsconcat
-Version: 0.1.2
+Version: 0.1.3
 Summary: BIDS App and Python library for concatenating MRI time series.
 License: LGPL-2.1
 Author: CMI DAIR Center
 Author-email: florian.rupprecht@childmind.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: bids2table (>=0.1.0b0,<0.2.0)
+Requires-Dist: bids2table (>=0.1.0,<0.2.0)
 Requires-Dist: nibabel (>=5.2.0,<6.0.0)
 Requires-Dist: numpy (>=1.26.3,<2.0.0)
 Requires-Dist: pandas (>1.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Description-Content-Type: text/markdown
 
 # `tsconcat`
```

