# Comparing `tmp/dsplus-0.4.6.tar.gz` & `tmp/dsplus-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsplus-0.4.6.tar", last modified: Mon May  6 04:53:12 2024, max compression
+gzip compressed data, was "dsplus-0.4.8.tar", last modified: Tue May  7 13:02:57 2024, max compression
```

## Comparing `dsplus-0.4.6.tar` & `dsplus-0.4.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 04:53:12.730253 dsplus-0.4.6/
--rw-rw-rw-   0        0        0     1083 2024-03-15 02:57:42.000000 dsplus-0.4.6/LICENSE
--rw-rw-rw-   0        0        0      690 2024-05-06 04:53:12.727916 dsplus-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0       99 2024-02-24 21:14:11.000000 dsplus-0.4.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 04:53:12.708559 dsplus-0.4.6/dsplus/
--rw-rw-rw-   0        0        0      171 2024-05-06 04:52:49.000000 dsplus-0.4.6/dsplus/__init__.py
--rw-rw-rw-   0        0        0    25408 2024-05-06 04:32:05.000000 dsplus-0.4.6/dsplus/pb_functions_general.py
--rw-rw-rw-   0        0        0    42785 2024-05-02 23:18:42.000000 dsplus-0.4.6/dsplus/pb_functions_pandas.py
--rw-rw-rw-   0        0        0    56910 2024-05-06 04:05:06.000000 dsplus-0.4.6/dsplus/pb_functions_plotly.py
--rw-rw-rw-   0        0        0    59122 2024-05-06 04:39:55.000000 dsplus-0.4.6/dsplus/pb_functions_spatial.py
-drwxrwxrwx   0        0        0        0 2024-05-06 04:53:12.720429 dsplus-0.4.6/dsplus.egg-info/
--rw-rw-rw-   0        0        0      690 2024-05-06 04:53:12.000000 dsplus-0.4.6/dsplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-05-06 04:53:12.000000 dsplus-0.4.6/dsplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 04:53:12.000000 dsplus-0.4.6/dsplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-06 04:53:12.000000 dsplus-0.4.6/dsplus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 04:53:12.730253 dsplus-0.4.6/setup.cfg
--rw-rw-rw-   0        0        0     1650 2024-03-29 02:13:48.000000 dsplus-0.4.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 04:53:12.722405 dsplus-0.4.6/tests/
--rw-rw-rw-   0        0        0    12530 2024-04-17 03:55:44.000000 dsplus-0.4.6/tests/Test_pandas.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:02:57.815959 dsplus-0.4.8/
+-rw-rw-rw-   0        0        0     1083 2024-03-15 02:57:42.000000 dsplus-0.4.8/LICENSE
+-rw-rw-rw-   0        0        0      690 2024-05-07 13:02:57.812332 dsplus-0.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0       99 2024-02-24 21:14:11.000000 dsplus-0.4.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 13:02:57.792309 dsplus-0.4.8/dsplus/
+-rw-rw-rw-   0        0        0      171 2024-05-07 13:02:39.000000 dsplus-0.4.8/dsplus/__init__.py
+-rw-rw-rw-   0        0        0    25485 2024-05-07 12:38:31.000000 dsplus-0.4.8/dsplus/pb_functions_general.py
+-rw-rw-rw-   0        0        0    43707 2024-05-07 13:01:59.000000 dsplus-0.4.8/dsplus/pb_functions_pandas.py
+-rw-rw-rw-   0        0        0    57143 2024-05-06 23:46:36.000000 dsplus-0.4.8/dsplus/pb_functions_plotly.py
+-rw-rw-rw-   0        0        0    59122 2024-05-06 04:39:55.000000 dsplus-0.4.8/dsplus/pb_functions_spatial.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:02:57.805184 dsplus-0.4.8/dsplus.egg-info/
+-rw-rw-rw-   0        0        0      690 2024-05-07 13:02:57.000000 dsplus-0.4.8/dsplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-05-07 13:02:57.000000 dsplus-0.4.8/dsplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 13:02:57.000000 dsplus-0.4.8/dsplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-07 13:02:57.000000 dsplus-0.4.8/dsplus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 13:02:57.815959 dsplus-0.4.8/setup.cfg
+-rw-rw-rw-   0        0        0     1650 2024-03-29 02:13:48.000000 dsplus-0.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:02:57.806722 dsplus-0.4.8/tests/
+-rw-rw-rw-   0        0        0    13083 2024-05-07 12:46:09.000000 dsplus-0.4.8/tests/Test_pandas.py
```

### Comparing `dsplus-0.4.6/LICENSE` & `dsplus-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.6/PKG-INFO` & `dsplus-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsplus
-Version: 0.4.6
+Version: 0.4.8
 Summary: Helper functions for data science applications.
 Author: Prashana Bajracharya
 Author-email: pajracharya713@gmail.com
 Keywords: data science,pandas
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dsplus-0.4.6/dsplus/pb_functions_general.py` & `dsplus-0.4.8/dsplus/pb_functions_general.py`

 * *Files 1% similar despite different names*

```diff
@@ -402,14 +402,15 @@
 
     Notes:
         - Each vector can be either of length 1 or of a constant length.
 
     Examples:
         >>> str_concat('x', '_', ['y', 'z'])
     '''
+    v_str = [pd.Series(val_str).to_numpy() for val_str in v_str]
     v_str_len = [len(x) if not isinstance(x, str) else 1 for x in v_str]
 
     if len(v_str_len) == 0:
         str_c = ''
         for str_current in v_str:
             str_c += str_current
         return (str_c)
@@ -422,15 +423,15 @@
             temp_str_current = pd_to_series(str_current)
             if str_len < max_str_len:
                 temp_str_current = temp_str_current.repeat(max_str_len)
             temp_str_current = temp_str_current.reset_index(drop = True)
 
             str_c = str_c.str.cat(temp_str_current.astype(str))
 
-        return (str_c)
+        return (str_c.to_numpy())
 
 #%%
 def str_join(v_str: list|np.ndarray|pd.Series, join_sep: str = ',') -> str:
     '''Join multiple strings into a single string with a join separator. Wrapper around 'join()'.
 
     Args:
         v_str (list | np.ndarray | pd.Series): Vector of strings.
```

### Comparing `dsplus-0.4.6/dsplus/pb_functions_pandas.py` & `dsplus-0.4.8/dsplus/pb_functions_pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,28 +104,57 @@
     elif isinstance(vector, pd.core.indexes.base.Index):
         vector = vector.to_series()
     else:
         vector = pd.Series() #np.nan
 
     return vector
 
+#%%
+def pd_to_numpy(vector: str|list|np.ndarray|pd.Series) -> np.ndarray:
+    '''Convert different types of vectors to array.
+
+    Args:
+        vector (str | list | np.ndarray | pd.Series): Vector.
+
+    Returns:
+        np.ndarray: Converted array. If unrecognized type is passed, np.nan is returned.
+
+    Examples:
+        >>> pd_to_numpy('a')
+        >>> pd_to_numpy([1, 2, 3])
+    '''
+    if isinstance(vector, str):
+        vector = np.array([vector])
+    elif isinstance(vector, list):
+        vector = np.array(vector)
+    elif isinstance(vector, np.ndarray):
+        pass
+    elif isinstance(vector, pd.Series):
+        vector = vector.to_numpy()
+    elif isinstance(vector, pd.core.indexes.base.Index):
+        vector = vector.to_series().to_numpy()
+    else:
+        vector = np.array() #np.nan
+
+    return vector
+
 #endregion -----------------------------------------------------------------------------------------
 #region Functions: Pandas: Slice
 
 #%%
-def pd_cols(df: pd.DataFrame, cols: str, to_list = True) -> list|pd.Series:
-    '''Get a vector of desired column names in desired order. Works well together with 'pd_select_simple()'.
+def pd_cols(df: pd.DataFrame, cols: str, to_numpy = True) -> np.ndarray|pd.Series:
+    '''Get a vector of desired column names in desired order.
 
     Args:
         df (pd.DataFrame): Dataframe whose column names are to be extracted.
         cols (str): String representing column name extraction rules. See notes.
-        to_list (bool, optional): Whether to return a list or series of column names. Defaults to True (return list).
+        to_numpy (bool, optional): Whether to return an array or series of column names. Defaults to True (return array).
 
     Returns:
-        list | pd.Series: List or series of column names.
+        np.ndarray | pd.Series: Array or series of column names.
 
     Notes:
         - 'cols' is comprised of individual pieces separated by comma.
             - Whitespaces before and after comma are ignored.
         - Each piece can be a column name, a slice, a pandas string function, or an asterisk (*).
         - Slice means a two column names separated by a colon. eg. 'v1:v5' means all columns from 'v1' to 'v5' (inclusive).
             - If the first columnn name is omitted, it means everything before. For eg. ':v5' means all column upto and including 'v5'.
@@ -206,16 +235,16 @@
                             v_cols.iloc[index_everything+1:]])
 
     if v_cols.size == 0:
         v_cols = v_cols_all.copy()
 
     v_cols = set_diff(v_cols, v_cols_drop)
 
-    if to_list:
-        v_cols = v_cols.tolist()
+    if to_numpy:
+        v_cols = v_cols.to_numpy()
     else:
         v_cols = v_cols.reset_index(drop=True)
 
     return v_cols
 
 #%%
 def pd_select(df: pd.DataFrame, cols: str) -> pd.DataFrame:
@@ -263,109 +292,14 @@
         >>> df.pipe(pd_select, 'str.contains("v2"), *, -str.startswith("v1"), -v8')
         >>> df.pipe(pd_select, '-select_dtypes("category")')
         >>> df.pipe(pd_select, 'select_dtypes("number"), *')
         >>> df.pipe(pd_select, '-v2:')
     '''
     return df[lambda _: pd_cols(_, cols)]
 
-#%%
-def pd_select_simple(df: pd.DataFrame,
-                     cols_before: str|list|np.ndarray|pd.Series = None,
-                     cols_after: str|list|np.ndarray|pd.Series = None,
-                     cols_drop: str|list|np.ndarray|pd.Series = None,
-                     remaining = True) -> pd.DataFrame:
-    '''Select columns to keep or drop from dataframe. Can be used to change order of columns.
-
-    Args:
-        df (pd.DataFrame): Dataframe.
-        cols_before (str | list | np.ndarray | pd.Series, optional): Columns to keep at the start. Defaults to None.
-        cols_after (str | list | np.ndarray | pd.Series, optional): Columns to keep at the end. Defaults to None.
-        cols_drop (str | list | np.ndarray | pd.Series, optional): Columns to drop. Defaults to None.
-        remaining (bool, optional): If true, the remaining columns (except the ones to drop) are placed between 'cols_before' and 'cols_after'. Defaults to True.
-
-    Returns:
-        pd.DataFrame: Dataframe with specified columns.
-
-    Examples:
-        >>> df.pipe(pd_select_simple, cols_before='type2', cols_after='value1', cols_drop='value5')
-        >>> df.pipe(pd_select_simple, cols_before=['value2', 'value4'], remaining=False)
-        >>> df.pipe(pd_select_simple, cols_before=pd_cols_archive(df, 'value2', 'value4'))
-        >>> df.pipe(pd_select_simple, cols_before=['type1', *pd_cols_archive(df, 'value2', 'value4')])
-        >>> df.assign(var=0).pipe(lambda _: pd_select_simple(_, cols_before=['var']))
-        >>> df.assign(var1=0, var2=5, var3=10).pipe(lambda _: pd_select_simple(_, cols_before=pd_cols_archive(_, 'var1', 'var3')))
-    '''
-    if cols_before is None:
-        cols_before = []
-    else:
-        cols_before = pd_to_series(cols_before).tolist()
-
-    if cols_after is None:
-        cols_after = []
-    else:
-        cols_after = pd_to_series(cols_after).tolist()
-
-    if cols_drop is None:
-        cols_drop = []
-    else:
-        cols_drop = pd_to_series(cols_drop).tolist()
-
-    if remaining:
-        cols_others = df.columns.difference(cols_before + cols_after, sort=False).tolist()
-        cols_keep = cols_before + cols_others + cols_after
-    else:
-        cols_keep = cols_before + cols_after
-
-    cols_keep = [x for x in cols_keep if x not in cols_drop]
-
-    return df[cols_keep]
-
-#%%
-def pd_drop(df: pd.DataFrame,
-            cols: str|list|np.ndarray|pd.Series = None,
-            col_from: str = None,
-            col_to: str = None) -> pd.DataFrame:
-    '''Drop selected columns from dataframe.
-
-    Args:
-        df (pd.DataFrame): Dataframe.
-        cols (str | list | np.ndarray | pd.Series, optional): Vector of columns to drop. Defaults to None (first column).
-        col_from (str, optional): First column in series of columns to drop. Defaults to None (last column).
-        col_to (str, optional): Last column in series of column to drop. Defaults to None.
-
-    Returns:
-        pd.DataFrame: Dataframe after dropping specified columns.
-
-    Notes:
-        - Any value in 'cols' not in 'df' is ignored. 'col_from' and 'col_to' have to in in 'df'.
-
-    Examples:
-        >>> df.pipe(pd_drop, 'value2')
-        >>> df.pipe(pd_drop, cols=['value2', 'type2'], col_from='value3', col_to='value5')
-        >>> df.pipe(pd_drop, col_from='value3')
-    '''
-    if cols is not None:
-        cols = pd_to_series(cols)
-        cols_all = pd.Series(df.columns)
-        cols = cols[cols.isin(cols_all)]
-        df = df.drop(cols, axis=1)
-    if (col_from is not None) | (col_to is not None):
-        cols_all = pd.Series(df.columns)
-        if col_from is not None:
-            index_from = cols_all.tolist().index(col_from)
-        else:
-            index_from = 0
-        if col_to is not None:
-            index_to = cols_all.tolist().index(col_to) + 1
-        else:
-            index_to = len(cols_all)
-        cols_to_drop = cols_all.iloc[index_from:index_to]
-
-        df = df.drop(cols_to_drop, axis=1)
-    return df
-
 #endregion -----------------------------------------------------------------------------------------
 #region Functions: Pandas: Concat
 
 #%%
 def pd_concat_series(v_values: pd.Series, values: float|list|np.ndarray|pd.Series) -> pd.Series:
     '''Append values to series.
 
@@ -481,15 +415,15 @@
 #%%
 def pd_merge_asof(df1: pd.DataFrame,
                   df2: pd.DataFrame,
                   on: str = None,
                   left_on: str = None,
                   right_on: str = None,
                   direction: Literal['backward', 'forward', 'nearest'] = 'forward',
-                  one_to_many = False):
+                  one_to_many = False) -> pd.DataFrame:
     '''Perform a merge by key direction. Wrapper around 'pandas.merge_asof()'. Unlike 'pandas.merge_asof()', default direction is 'forward'. Additionally, 'one_to_many' is an additional option. Finally, if one of the two dataframes are blank, 'df1' is still returned along with columns from 'df2' added and set to np.nan, and no error is raised
 
     Args:
         df1 (pd.DataFrame): Dataframe.
         df2 (pd.DataFrame): Dataframe.
         on (str, optional): Common column name from 'df1' and 'df2' to join on. Defaults to None.
         left_on (str, optional): Column name from 'df1' to be joined on. Defaults to None.
@@ -890,15 +824,15 @@
         else:
             df.columns = df.columns.rename(None)
 
     return df
 
 #%%
 def pd_set_colnames(df: pd.DataFrame,
-                    col_names: str|list|np.ndarray|pd.Series):
+                    col_names: str|list|np.ndarray|pd.Series) -> pd.DataFrame:
     '''Set column names. Wrapper around 'pd.concat()'. Works with length mismatches.
 
     Args:
         df (pd.DataFrame): Dataframe.
         col_names (str | list | np.ndnp.ndarray | pd.Series): Vector of column names.
 
     Returns:
@@ -1027,14 +961,109 @@
 
     return df
 
 #endregion -----------------------------------------------------------------------------------------
 #region Archive
 
 #%%
+def pd_select_simple(df: pd.DataFrame,
+                     cols_before: str|list|np.ndarray|pd.Series = None,
+                     cols_after: str|list|np.ndarray|pd.Series = None,
+                     cols_drop: str|list|np.ndarray|pd.Series = None,
+                     remaining = True) -> pd.DataFrame:
+    '''DEPRECATED: Use `pd_select()`. Select columns to keep or drop from dataframe. Can be used to change order of columns.
+
+    Args:
+        df (pd.DataFrame): Dataframe.
+        cols_before (str | list | np.ndarray | pd.Series, optional): Columns to keep at the start. Defaults to None.
+        cols_after (str | list | np.ndarray | pd.Series, optional): Columns to keep at the end. Defaults to None.
+        cols_drop (str | list | np.ndarray | pd.Series, optional): Columns to drop. Defaults to None.
+        remaining (bool, optional): If true, the remaining columns (except the ones to drop) are placed between 'cols_before' and 'cols_after'. Defaults to True.
+
+    Returns:
+        pd.DataFrame: Dataframe with specified columns.
+
+    Examples:
+        >>> df.pipe(pd_select_simple, cols_before='type2', cols_after='value1', cols_drop='value5')
+        >>> df.pipe(pd_select_simple, cols_before=['value2', 'value4'], remaining=False)
+        >>> df.pipe(pd_select_simple, cols_before=pd_cols_archive(df, 'value2', 'value4'))
+        >>> df.pipe(pd_select_simple, cols_before=['type1', *pd_cols_archive(df, 'value2', 'value4')])
+        >>> df.assign(var=0).pipe(lambda _: pd_select_simple(_, cols_before=['var']))
+        >>> df.assign(var1=0, var2=5, var3=10).pipe(lambda _: pd_select_simple(_, cols_before=pd_cols_archive(_, 'var1', 'var3')))
+    '''
+    if cols_before is None:
+        cols_before = []
+    else:
+        cols_before = pd_to_series(cols_before).tolist()
+
+    if cols_after is None:
+        cols_after = []
+    else:
+        cols_after = pd_to_series(cols_after).tolist()
+
+    if cols_drop is None:
+        cols_drop = []
+    else:
+        cols_drop = pd_to_series(cols_drop).tolist()
+
+    if remaining:
+        cols_others = df.columns.difference(cols_before + cols_after, sort=False).tolist()
+        cols_keep = cols_before + cols_others + cols_after
+    else:
+        cols_keep = cols_before + cols_after
+
+    cols_keep = [x for x in cols_keep if x not in cols_drop]
+
+    return df[cols_keep]
+
+#%%
+def pd_drop(df: pd.DataFrame,
+            cols: str|list|np.ndarray|pd.Series = None,
+            col_from: str = None,
+            col_to: str = None) -> pd.DataFrame:
+    '''DEPRECATED: Use `pd_select()`. Drop selected columns from dataframe.
+
+    Args:
+        df (pd.DataFrame): Dataframe.
+        cols (str | list | np.ndarray | pd.Series, optional): Vector of columns to drop. Defaults to None (first column).
+        col_from (str, optional): First column in series of columns to drop. Defaults to None (last column).
+        col_to (str, optional): Last column in series of column to drop. Defaults to None.
+
+    Returns:
+        pd.DataFrame: Dataframe after dropping specified columns.
+
+    Notes:
+        - Any value in 'cols' not in 'df' is ignored. 'col_from' and 'col_to' have to in in 'df'.
+
+    Examples:
+        >>> df.pipe(pd_drop, 'value2')
+        >>> df.pipe(pd_drop, cols=['value2', 'type2'], col_from='value3', col_to='value5')
+        >>> df.pipe(pd_drop, col_from='value3')
+    '''
+    if cols is not None:
+        cols = pd_to_series(cols)
+        cols_all = pd.Series(df.columns)
+        cols = cols[cols.isin(cols_all)]
+        df = df.drop(cols, axis=1)
+    if (col_from is not None) | (col_to is not None):
+        cols_all = pd.Series(df.columns)
+        if col_from is not None:
+            index_from = cols_all.tolist().index(col_from)
+        else:
+            index_from = 0
+        if col_to is not None:
+            index_to = cols_all.tolist().index(col_to) + 1
+        else:
+            index_to = len(cols_all)
+        cols_to_drop = cols_all.iloc[index_from:index_to]
+
+        df = df.drop(cols_to_drop, axis=1)
+    return df
+
+#%%
 def pd_cols_archive(df: pd.DataFrame,
             col_from: str=None,
             col_to: str=None) -> list:
     '''Get column names between two column names for given dataframe.
 
     Args:
         df (pd.DataFrame): Dataframe.
```

### Comparing `dsplus-0.4.6/dsplus/pb_functions_plotly.py` & `dsplus-0.4.8/dsplus/pb_functions_plotly.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-#region Libraries
+#region Libraries   
 
 #%%
 from typing import Literal, Self, Callable, Any
 
 import pandas as pd
 import numpy as np
 
 import plotly.express as px
 import plotly.graph_objects as go
 import plotly.figure_factory as ff
 import plotly.io as pio
 
+from .pb_functions_general import *
+
 #endregion -----------------------------------------------------------------------------------------
 #region Functions
 
 #%%
 def px_add_trace_data(fig_original, *figs):
     '''Add trace(s) to plotly figure.
 
@@ -251,14 +253,17 @@
             - Category order arguments
             - Facet arguments
             - Marginal arguemnts
             - Hover arguemnts
         '''
         def inner(func):
             def wrapper(self, *args, **kwargs):
+                # kwargs = combine_arguments(func, [0, *args], kwargs)
+                # kwargs.pop('self')
+
                 if kwargs.get('category_orders') is not None or self.category_orders is not None:
                     kwargs['category_orders']=({} if kwargs.get('category_orders') is None else kwargs.get('category_orders')) | ({} if self.category_orders is None else self.category_orders)
                 else:
                     kwargs['category_orders']=self.category_orders
 
                 kwargs['facet_row']=self.facet_row
                 kwargs['facet_col']=self.facet_col
@@ -297,17 +302,19 @@
                 elif marginal == '':
                     pass
                 else:
                     kwargs['marginal']=self.marginal_xy
 
                 kwargs = {k:v for k,v in kwargs.items() if v is not None}
 
+                # kwargs |= _
                 # return func(self, *args, **kwargs)
 
                 trace = func(self, *args, **kwargs)
+                # trace = func(self, **kwargs)
 
                 self._update_legend_show(trace, kwargs.get('legend_show'), kwargs.get('legend_name'))
 
                 self.add(trace)
 
                 self._update_facet_axes()
```

### Comparing `dsplus-0.4.6/dsplus/pb_functions_spatial.py` & `dsplus-0.4.8/dsplus/pb_functions_spatial.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.6/dsplus.egg-info/PKG-INFO` & `dsplus-0.4.8/dsplus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsplus
-Version: 0.4.6
+Version: 0.4.8
 Summary: Helper functions for data science applications.
 Author: Prashana Bajracharya
 Author-email: pajracharya713@gmail.com
 Keywords: data science,pandas
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dsplus-0.4.6/setup.py` & `dsplus-0.4.8/setup.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.6/tests/Test_pandas.py` & `dsplus-0.4.8/tests/Test_pandas.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,14 +80,34 @@
 def test_pd_to_series_4():
     assert ds.pd_to_series(pd.Series([1,2,3])).equals(pd.Series([1,2,3]))
 
 #%%
 def test_pd_to_series_5():
     assert ds.pd_to_series(pd.Series([1,2,3]).index).equals(pd.Series([0,1,2]))
 
+#%%
+def test_pd_to_numpy_1():
+    assert np.array_equal(ds.pd_to_numpy([1,2,3]), np.array([1,2,3]))
+
+#%%
+def test_pd_to_numpy_2():
+    assert np.array_equal(ds.pd_to_numpy([]), np.array([]))
+
+#%%
+def test_pd_to_numpy_3():
+    assert np.array_equal(ds.pd_to_numpy(np.array([1,2,3])), np.array([1,2,3]))
+
+#%%
+def test_pd_to_numpy_4():
+    assert np.array_equal(ds.pd_to_numpy(pd.Series([1,2,3])), np.array([1,2,3]))
+
+#%%
+def test_pd_to_numpy_5():
+    assert np.array_equal(ds.pd_to_numpy(pd.Series([1,2,3]).index), np.array([0,1,2]))
+
 #endregion -----------------------------------------------------------------------------------------
 #region Slice
 
 #%%
 def test_pd_select_1():
     df = pd.DataFrame(columns = ['v'+str(_) for _ in range(21)])
```

