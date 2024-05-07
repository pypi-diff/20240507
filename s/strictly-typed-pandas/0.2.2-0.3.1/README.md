# Comparing `tmp/strictly_typed_pandas-0.2.2.tar.gz` & `tmp/strictly_typed_pandas-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strictly_typed_pandas-0.2.2.tar", last modified: Mon Feb 26 08:27:39 2024, max compression
+gzip compressed data, was "strictly_typed_pandas-0.3.1.tar", last modified: Tue May  7 18:35:12 2024, max compression
```

## Comparing `strictly_typed_pandas-0.2.2.tar` & `strictly_typed_pandas-0.3.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:27:39.858357 strictly_typed_pandas-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-02-26 08:27:39.858357 strictly_typed_pandas-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 08:27:39.858357 strictly_typed_pandas-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:27:39.854357 strictly_typed_pandas-0.2.2/strictly_typed_pandas/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:27:39.858357 strictly_typed_pandas-0.2.2/strictly_typed_pandas/_vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:27:39.858357 strictly_typed_pandas-0.2.2/strictly_typed_pandas/_vendor/typeguard/
--rw-r--r--   0 runner    (1001) docker     (127)    49186 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/_vendor/typeguard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/_vendor/typeguard/importhook.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/_vendor/typeguard/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/_vendor/typeguard/pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/create_empty_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/immutable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/pandas_types.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/typeguard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/validate_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:27:39.858357 strictly_typed_pandas-0.2.2/strictly_typed_pandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-02-26 08:27:39.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-02-26 08:27:39.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 08:27:39.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-26 08:27:39.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-26 08:27:39.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-26 08:27:39.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:27:39.858357 strictly_typed_pandas-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/tests/test_indexed_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/tests/test_type_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:35:12.120917 strictly_typed_pandas-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-07 18:35:02.000000 strictly_typed_pandas-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-07 18:35:12.120917 strictly_typed_pandas-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-07 18:35:02.000000 strictly_typed_pandas-0.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-07 18:35:02.000000 strictly_typed_pandas-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 18:35:12.120917 strictly_typed_pandas-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-07 18:35:02.000000 strictly_typed_pandas-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:35:12.116917 strictly_typed_pandas-0.3.1/strictly_typed_pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-07 18:35:02.000000 strictly_typed_pandas-0.3.1/strictly_typed_pandas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:35:12.120917 strictly_typed_pandas-0.3.1/strictly_typed_pandas/_vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:35:02.000000 strictly_typed_pandas-0.3.1/strictly_typed_pandas/_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:35:12.120917 strictly_typed_pandas-0.3.1/strictly_typed_pandas/_vendor/typeguard/
+-rw-r--r--   0 runner    (1001) docker     (127)    49186 2024-05-07 18:35:02.000000 strictly_typed_pandas-0.3.1/strictly_typed_pandas/_vendor/typeguard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-05-07 18:35:02.000000 strictly_typed_pandas-0.3.1/strictly_typed_pandas/_vendor/typeguard/importhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:35:02.000000 strictly_typed_pandas-0.3.1/strictly_typed_pandas/_vendor/typeguard/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-07 18:35:02.000000 strictly_typed_pandas-0.3.1/strictly_typed_pandas/_vendor/typeguard/pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-07 18:35:02.000000 strictly_typed_pandas-0.3.1/strictly_typed_pandas/create_empty_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-05-07 18:35:02.000000 strictly_typed_pandas-0.3.1/strictly_typed_pandas/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-07 18:35:02.000000 strictly_typed_pandas-0.3.1/strictly_typed_pandas/immutable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-07 18:35:02.000000 strictly_typed_pandas-0.3.1/strictly_typed_pandas/pandas_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:35:02.000000 strictly_typed_pandas-0.3.1/strictly_typed_pandas/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-07 18:35:02.000000 strictly_typed_pandas-0.3.1/strictly_typed_pandas/pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-07 18:35:02.000000 strictly_typed_pandas-0.3.1/strictly_typed_pandas/typeguard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-07 18:35:02.000000 strictly_typed_pandas-0.3.1/strictly_typed_pandas/validate_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:35:12.120917 strictly_typed_pandas-0.3.1/strictly_typed_pandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-07 18:35:12.000000 strictly_typed_pandas-0.3.1/strictly_typed_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-07 18:35:12.000000 strictly_typed_pandas-0.3.1/strictly_typed_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 18:35:12.000000 strictly_typed_pandas-0.3.1/strictly_typed_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-07 18:35:12.000000 strictly_typed_pandas-0.3.1/strictly_typed_pandas.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-07 18:35:12.000000 strictly_typed_pandas-0.3.1/strictly_typed_pandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 18:35:12.000000 strictly_typed_pandas-0.3.1/strictly_typed_pandas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:35:12.120917 strictly_typed_pandas-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-07 18:35:02.000000 strictly_typed_pandas-0.3.1/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-07 18:35:02.000000 strictly_typed_pandas-0.3.1/tests/test_indexed_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-07 18:35:02.000000 strictly_typed_pandas-0.3.1/tests/test_type_validation.py
```

### Comparing `strictly_typed_pandas-0.2.2/LICENSE` & `strictly_typed_pandas-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.2/PKG-INFO` & `strictly_typed_pandas-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: strictly_typed_pandas
-Version: 0.2.2
+Version: 0.3.1
 Summary: Static type checking of pandas DataFrames
 Home-page: https://github.com/nanne-aben/strictly_typed_pandas
 Author: Nanne Aben
 Author-email: nanne.aben@gmail.com
 License: MIT
 Keywords: typing type checking pandas mypy linting
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: numpy<=1.26.4
-Requires-Dist: pandas<=2.2.1
-Requires-Dist: pandas-stubs<=2.2.0.240218
+Requires-Dist: pandas<=2.2.2
+Requires-Dist: pandas-stubs<=2.2.1.240316
 
 ================================================================
 Strictly Typed Pandas: static type checking of pandas DataFrames
 ================================================================
 
 I love Pandas! But in production code I’m always a bit wary when I see:
```

### Comparing `strictly_typed_pandas-0.2.2/README.rst` & `strictly_typed_pandas-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.2/setup.py` & `strictly_typed_pandas-0.3.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     keywords="typing type checking pandas mypy linting",
     long_description=get_long_description(),
     long_description_content_type="text/x-rst",
     packages=find_packages(include=["strictly_typed_pandas", "strictly_typed_pandas.*"]),
     install_requires=get_requirements(),
     python_requires=">=3.8.0",
     classifiers=["Typing :: Typed"],
-    version_config=True,
+    setuptools_git_versioning={"enabled": True},
     setup_requires=["setuptools-git-versioning"],
     package_data={"strictly_typed_pandas": ["py.typed"]},
     entry_points={
         "pytest11": [
             "strictly_typed_pandas = strictly_typed_pandas.pytest_plugin",
         ],
     },
```

### Comparing `strictly_typed_pandas-0.2.2/strictly_typed_pandas/_vendor/typeguard/__init__.py` & `strictly_typed_pandas-0.3.1/strictly_typed_pandas/_vendor/typeguard/__init__.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.2/strictly_typed_pandas/_vendor/typeguard/importhook.py` & `strictly_typed_pandas-0.3.1/strictly_typed_pandas/_vendor/typeguard/importhook.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.2/strictly_typed_pandas/_vendor/typeguard/pytest_plugin.py` & `strictly_typed_pandas-0.3.1/strictly_typed_pandas/_vendor/typeguard/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.2/strictly_typed_pandas/create_empty_dataframe.py` & `strictly_typed_pandas-0.3.1/strictly_typed_pandas/create_empty_dataframe.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.2/strictly_typed_pandas/dataset.py` & `strictly_typed_pandas-0.3.1/strictly_typed_pandas/dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import inspect
-from abc import ABC, abstractmethod
+from abc import ABC
 from typing import Any, Generic, TypeVar, get_type_hints
 
 import pandas as pd
 
 from strictly_typed_pandas.create_empty_dataframe import (
     create_empty_dataframe,
     create_empty_indexed_dataframe,
@@ -31,29 +31,17 @@
 
         if self.columns.duplicated().any():
             msg = "DataSet has duplicate columns: {cols}".format(
                 cols=self.columns[self.columns.duplicated()]
             )
             raise TypeError(msg)
 
-        # In Python 3.6, self._schema_annotations is set before __init__() is called, hence we continue here
-        if hasattr(self, "_schema_annotations"):
-            self._continue_initialization()
-
     def __setattr__(self, name: str, value: Any) -> None:
         object.__setattr__(self, name, value)
 
-        if name == "__orig_class__" and hasattr(self.__orig_class__, "__args__"):
-            self._schema_annotations = value.__args__
-
-            # In Python 3.7 and above, self._schema_annotations is set after the __init__() is wrapped up, hence we
-            # continue from here
-            if hasattr(self, "shape"):
-                self._continue_initialization()
-
         if name in self.columns and name not in dataframe_member_names:
             raise NotImplementedError(immutable_error_msg)
 
     def __setitem__(self, key: Any, value: Any):
         raise NotImplementedError(immutable_error_msg)
 
     def __getattribute__(self, name: str) -> Any:
@@ -67,18 +55,14 @@
     def iloc(self) -> _ImmutableiLocIndexer:  # type: ignore
         return _ImmutableiLocIndexer("iloc", self)  # type: ignore
 
     @property
     def loc(self) -> _ImmutableLocIndexer:  # type: ignore
         return _ImmutableLocIndexer("loc", self)  # type: ignore
 
-    @abstractmethod
-    def _continue_initialization(self) -> None:
-        pass  # pragma: no cover
-
     def to_dataframe(self) -> pd.DataFrame:
         """Converts the object to a pandas `DataFrame`."""
         return pd.DataFrame(self)
 
     def to_frame(self) -> pd.DataFrame:
         """Synonym of to to_dataframe(): converts the object to a pandas `DataFrame`."""
         return self.to_dataframe()
@@ -104,16 +88,30 @@
         * is immutable, so its schema cannot be changed using inplace modifications.
 
     The `DataSet[Schema]` annotations are compatible with:
         * `mypy` for type checking during linting-time (i.e. while you write your code).
         * `typeguard` (<3.0) for type checking during run-time (i.e. while you run your unit tests).
     """
 
-    def _continue_initialization(self) -> None:
-        schema_expected = get_type_hints(self._schema_annotations[0])
+    _schema_annotations = None
+
+    def __class_getitem__(cls, item):
+        """Allows us to define a schema for the ``DataSet``."""
+        cls = super().__class_getitem__(item)
+        cls._schema_annotations = item
+        return cls
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        if DataSet._schema_annotations is None:
+            return
+
+        schema_expected = get_type_hints(DataSet._schema_annotations)
+        DataSet._schema_annotations = None
 
         if self.shape == (0, 0):
             df = create_empty_dataframe(schema_expected)
             super().__init__(df)
         else:
             schema_observed = dict(zip(self.columns, self.dtypes))
             validate_schema(schema_expected, schema_observed)
@@ -148,17 +146,34 @@
         * is immutable, so its schema cannot be changed using inplace modifications.
 
     The `IndexedDataSet[Schema]` annotations are compatible with:
         * `mypy` for type checking during linting-time (i.e. while you write your code).
         * `typeguard` (<3.0) for type checking during run-time (i.e. while you run your unit tests).
     """
 
-    def _continue_initialization(self) -> None:
-        schema_index_expected = get_type_hints(self._schema_annotations[0])
-        schema_data_expected = get_type_hints(self._schema_annotations[1])
+    _schema_index = None
+    _schema_data = None
+
+    def __class_getitem__(cls, item):
+        """Allows us to define a schema for the ``DataSet``."""
+        cls = super().__class_getitem__(item)
+        cls._schema_index = item[0]
+        cls._schema_data = item[1]
+        return cls
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        if IndexedDataSet._schema_index is None or IndexedDataSet._schema_data is None:
+            return
+
+        schema_index_expected = get_type_hints(IndexedDataSet._schema_index)
+        schema_data_expected = get_type_hints(IndexedDataSet._schema_data)
+        IndexedDataSet._schema_index = None
+        IndexedDataSet._schema_data = None
 
         check_for_duplicate_columns(
             set(schema_index_expected.keys()), set(schema_data_expected.keys())
         )
 
         if self.shape == (0, 0) and self.index.shape == (0,):
             df = create_empty_indexed_dataframe(schema_index_expected, schema_data_expected)
```

### Comparing `strictly_typed_pandas-0.2.2/strictly_typed_pandas/immutable.py` & `strictly_typed_pandas-0.3.1/strictly_typed_pandas/immutable.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.2/strictly_typed_pandas/pandas_types.py` & `strictly_typed_pandas-0.3.1/strictly_typed_pandas/pandas_types.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.2/strictly_typed_pandas/pytest_plugin.py` & `strictly_typed_pandas-0.3.1/strictly_typed_pandas/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.2/strictly_typed_pandas/typeguard.py` & `strictly_typed_pandas-0.3.1/strictly_typed_pandas/typeguard.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.2/strictly_typed_pandas/validate_schema.py` & `strictly_typed_pandas-0.3.1/strictly_typed_pandas/validate_schema.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.2/strictly_typed_pandas.egg-info/PKG-INFO` & `strictly_typed_pandas-0.3.1/strictly_typed_pandas.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: strictly_typed_pandas
-Version: 0.2.2
+Version: 0.3.1
 Summary: Static type checking of pandas DataFrames
 Home-page: https://github.com/nanne-aben/strictly_typed_pandas
 Author: Nanne Aben
 Author-email: nanne.aben@gmail.com
 License: MIT
 Keywords: typing type checking pandas mypy linting
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: numpy<=1.26.4
-Requires-Dist: pandas<=2.2.1
-Requires-Dist: pandas-stubs<=2.2.0.240218
+Requires-Dist: pandas<=2.2.2
+Requires-Dist: pandas-stubs<=2.2.1.240316
 
 ================================================================
 Strictly Typed Pandas: static type checking of pandas DataFrames
 ================================================================
 
 I love Pandas! But in production code I’m always a bit wary when I see:
```

### Comparing `strictly_typed_pandas-0.2.2/strictly_typed_pandas.egg-info/SOURCES.txt` & `strictly_typed_pandas-0.3.1/strictly_typed_pandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.2/tests/test_dataset.py` & `strictly_typed_pandas-0.3.1/tests/test_dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -105,7 +105,38 @@
     df = DataSet[Schema](dictionary)
 
     with tempfile.TemporaryDirectory() as tmpdir:
         pickle.dump(df, open(f"{tmpdir}/test.pkl", "wb"))
         loaded = pickle.load(open(f"{tmpdir}/test.pkl", "rb"))
 
     assert (df == loaded).all().all()
+
+
+class A:
+    a: int
+
+
+class B:
+    a: int
+
+
+def test_resetting_of_schema_annotations():
+    df = DataSet[A]()
+
+    a: pd.DataFrame
+
+    # if no schema is specified, the annotation should be None
+    a = DataSet(df)
+    assert a._schema_annotations is None
+
+    # when we specify a schema, the class variable will be set to A, but afterwards it should be
+    # reset to None again when we initialize a new object without specifying a schema
+    DataSet[A]
+    a = DataSet(df)
+    assert a._schema_annotations is None
+
+    # and then to B
+    a = DataSet[B](df)
+
+    # and then to None again
+    a = DataSet(df)
+    assert a._schema_annotations is None
```

### Comparing `strictly_typed_pandas-0.2.2/tests/test_indexed_dataset.py` & `strictly_typed_pandas-0.3.1/tests/test_indexed_dataset.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.2/tests/test_type_validation.py` & `strictly_typed_pandas-0.3.1/tests/test_type_validation.py`

 * *Files identical despite different names*

