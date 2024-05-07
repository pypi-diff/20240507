# Comparing `tmp/sqldatamodel-0.4.2.tar.gz` & `tmp/sqldatamodel-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqldatamodel-0.4.2.tar", last modified: Fri May  3 20:55:28 2024, max compression
+gzip compressed data, was "sqldatamodel-0.4.3.tar", last modified: Tue May  7 19:28:58 2024, max compression
```

## Comparing `sqldatamodel-0.4.2.tar` & `sqldatamodel-0.4.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 20:55:28.271341 sqldatamodel-0.4.2/
--rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 sqldatamodel-0.4.2/LICENSE
--rw-rw-rw-   0        0        0    29556 2024-05-03 20:55:28.264339 sqldatamodel-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0    27664 2024-05-03 20:51:29.000000 sqldatamodel-0.4.2/README.md
--rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 sqldatamodel-0.4.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-03 20:55:28.272562 sqldatamodel-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     2424 2024-05-03 20:53:56.000000 sqldatamodel-0.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 20:55:26.841957 sqldatamodel-0.4.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-03 20:55:28.011722 sqldatamodel-0.4.2/src/SQLDataModel/
--rw-rw-rw-   0        0        0     6644 2024-05-03 15:03:44.000000 sqldatamodel-0.4.2/src/SQLDataModel/ANSIColor.py
--rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 sqldatamodel-0.4.2/src/SQLDataModel/HTMLParser.py
--rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 sqldatamodel-0.4.2/src/SQLDataModel/JSONEncoder.py
--rw-rw-rw-   0        0        0   603587 2024-05-03 17:38:41.000000 sqldatamodel-0.4.2/src/SQLDataModel/SQLDataModel.py
--rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 sqldatamodel-0.4.2/src/SQLDataModel/StandardDeviation.py
--rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 sqldatamodel-0.4.2/src/SQLDataModel/__init__.py
--rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 sqldatamodel-0.4.2/src/SQLDataModel/converters.py
--rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 sqldatamodel-0.4.2/src/SQLDataModel/demo.py
--rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 sqldatamodel-0.4.2/src/SQLDataModel/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-03 20:55:28.189006 sqldatamodel-0.4.2/src/SQLDataModel/extensions/
--rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 sqldatamodel-0.4.2/src/SQLDataModel/extensions/__init__.py
--rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 sqldatamodel-0.4.2/src/SQLDataModel/extensions/str_utils.c
-drwxrwxrwx   0        0        0        0 2024-05-03 20:55:28.258516 sqldatamodel-0.4.2/src/SQLDataModel.egg-info/
--rw-rw-rw-   0        0        0    29556 2024-05-03 20:55:26.000000 sqldatamodel-0.4.2/src/SQLDataModel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2024-05-03 20:55:26.000000 sqldatamodel-0.4.2/src/SQLDataModel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 20:55:26.000000 sqldatamodel-0.4.2/src/SQLDataModel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-03 20:55:26.000000 sqldatamodel-0.4.2/src/SQLDataModel.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-03 20:55:28.203755 sqldatamodel-0.4.2/tests/
--rw-rw-rw-   0        0        0    62183 2024-05-03 20:52:05.000000 sqldatamodel-0.4.2/tests/test_Future.py
--rw-rw-rw-   0        0        0    62186 2024-05-03 20:52:06.000000 sqldatamodel-0.4.2/tests/test_SQLDataModel.py
+drwxrwxrwx   0        0        0        0 2024-05-07 19:28:58.071769 sqldatamodel-0.4.3/
+-rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 sqldatamodel-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0    29557 2024-05-07 19:28:58.062878 sqldatamodel-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0    27665 2024-05-07 00:24:25.000000 sqldatamodel-0.4.3/README.md
+-rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 sqldatamodel-0.4.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-07 19:28:58.073546 sqldatamodel-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     2424 2024-05-07 19:27:52.000000 sqldatamodel-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 19:28:56.209775 sqldatamodel-0.4.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-07 19:28:57.391305 sqldatamodel-0.4.3/src/SQLDataModel/
+-rw-rw-rw-   0        0        0     6644 2024-05-03 15:03:44.000000 sqldatamodel-0.4.3/src/SQLDataModel/ANSIColor.py
+-rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 sqldatamodel-0.4.3/src/SQLDataModel/HTMLParser.py
+-rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 sqldatamodel-0.4.3/src/SQLDataModel/JSONEncoder.py
+-rw-rw-rw-   0        0        0   609546 2024-05-07 18:50:28.000000 sqldatamodel-0.4.3/src/SQLDataModel/SQLDataModel.py
+-rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 sqldatamodel-0.4.3/src/SQLDataModel/StandardDeviation.py
+-rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 sqldatamodel-0.4.3/src/SQLDataModel/__init__.py
+-rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 sqldatamodel-0.4.3/src/SQLDataModel/converters.py
+-rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 sqldatamodel-0.4.3/src/SQLDataModel/demo.py
+-rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 sqldatamodel-0.4.3/src/SQLDataModel/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-07 19:28:57.978627 sqldatamodel-0.4.3/src/SQLDataModel/extensions/
+-rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 sqldatamodel-0.4.3/src/SQLDataModel/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 sqldatamodel-0.4.3/src/SQLDataModel/extensions/str_utils.c
+drwxrwxrwx   0        0        0        0 2024-05-07 19:28:58.056312 sqldatamodel-0.4.3/src/SQLDataModel.egg-info/
+-rw-rw-rw-   0        0        0    29557 2024-05-07 19:28:56.000000 sqldatamodel-0.4.3/src/SQLDataModel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2024-05-07 19:28:56.000000 sqldatamodel-0.4.3/src/SQLDataModel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 19:28:56.000000 sqldatamodel-0.4.3/src/SQLDataModel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-07 19:28:56.000000 sqldatamodel-0.4.3/src/SQLDataModel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 19:28:57.993626 sqldatamodel-0.4.3/tests/
+-rw-rw-rw-   0        0        0    63183 2024-05-07 19:27:28.000000 sqldatamodel-0.4.3/tests/test_Future.py
+-rw-rw-rw-   0        0        0    63186 2024-05-07 19:27:26.000000 sqldatamodel-0.4.3/tests/test_SQLDataModel.py
```

### Comparing `sqldatamodel-0.4.2/LICENSE` & `sqldatamodel-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.2/PKG-INFO` & `sqldatamodel-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.4.2
+Version: 0.4.3
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal-tables,pretty-print-tables,sql2sql,data-analysis,data-science,datamodel,extract,transform,load,web-scraping-tables,data-mining,html,html-table-parsing,apache-arrow,pyarrow,pyarrow-conversion,pyarrow-to-table,pyarrow-to-sql,pyarrow-to-csv,parquet-file-parsing,csv,csv-parsing,markdown,markdown-table-parsing,latex,latex-table-parsing,delimited,delimited-data-parsing,file-conversion,format-conversion,terminal-styling,table-styling,from-sqlite,to-sqlite,from-postgresql,to-postgresql,sql-to-sql,excel,xlsx-file,excel-to-sql,DataFrames,polars2pandas,pandas2polars
@@ -61,15 +61,15 @@
 | Mercury |    0.38 |     0 | True     |
 | Venus   |    0.91 |     0 | True     |
 | Mars    |    0.38 |     2 | True     |
 | Saturn  |    0.92 |   146 | True     |
 | Uranus  |    0.89 |    27 | True     |
 ```
 
-Made for those times when you just want to use raw SQL on your dataframe, or need to move data around but the full Pandas, Numpy, SQLAlchemy installation is just overkill. SQLDataModel includes all the most commonly used features, including additional ones like using plan SQL on your `DataFrame` and pretty printing your table, at _1/1000_ the size, 0.03MB vs 30MB
+Made for those times when you just want to use raw SQL on your dataframe, or need to move data around but the full Pandas, Numpy, SQLAlchemy installation is just overkill. SQLDataModel includes all the most commonly used features, including additional ones like using plain SQL on your `DataFrame` and pretty printing your table, at _1/1000_ the size, 0.03MB vs 30MB
 
 ---
 
 ### Installation
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install SQLDataModel.
 
 ```bash
```

### Comparing `sqldatamodel-0.4.2/README.md` & `sqldatamodel-0.4.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 | Mercury |    0.38 |     0 | True     |
 | Venus   |    0.91 |     0 | True     |
 | Mars    |    0.38 |     2 | True     |
 | Saturn  |    0.92 |   146 | True     |
 | Uranus  |    0.89 |    27 | True     |
 ```
 
-Made for those times when you just want to use raw SQL on your dataframe, or need to move data around but the full Pandas, Numpy, SQLAlchemy installation is just overkill. SQLDataModel includes all the most commonly used features, including additional ones like using plan SQL on your `DataFrame` and pretty printing your table, at _1/1000_ the size, 0.03MB vs 30MB
+Made for those times when you just want to use raw SQL on your dataframe, or need to move data around but the full Pandas, Numpy, SQLAlchemy installation is just overkill. SQLDataModel includes all the most commonly used features, including additional ones like using plain SQL on your `DataFrame` and pretty printing your table, at _1/1000_ the size, 0.03MB vs 30MB
 
 ---
 
 ### Installation
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install SQLDataModel.
 
 ```bash
```

### Comparing `sqldatamodel-0.4.2/setup.py` & `sqldatamodel-0.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='SQLDataModel',  
-     version='0.4.2',
+     version='0.4.3',
      scripts=['src/SQLDataModel/SQLDataModel.py'] ,
      author='Ante Tonkovic-Capin',
      author_email='antetc@icloud.com',
      description='SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.',
      keywords=['SQL','ETL','dataframe','terminal-tables','pretty-print-tables','sql2sql','data-analysis','data-science','datamodel','extract','transform','load','web-scraping-tables','data-mining','html','html-table-parsing','apache-arrow','pyarrow','pyarrow-conversion','pyarrow-to-table','pyarrow-to-sql','pyarrow-to-csv','parquet-file-parsing','csv','csv-parsing','markdown','markdown-table-parsing','latex','latex-table-parsing','delimited','delimited-data-parsing','file-conversion','format-conversion','terminal-styling','table-styling','from-sqlite','to-sqlite','from-postgresql','to-postgresql','sql-to-sql','excel','xlsx-file','excel-to-sql','DataFrames','polars2pandas','pandas2polars'],
      license_file='LICENSE',
      long_description=long_description,
```

### Comparing `sqldatamodel-0.4.2/src/SQLDataModel/ANSIColor.py` & `sqldatamodel-0.4.3/src/SQLDataModel/ANSIColor.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.2/src/SQLDataModel/HTMLParser.py` & `sqldatamodel-0.4.3/src/SQLDataModel/HTMLParser.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.2/src/SQLDataModel/JSONEncoder.py` & `sqldatamodel-0.4.3/src/SQLDataModel/JSONEncoder.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.2/src/SQLDataModel/SQLDataModel.py` & `sqldatamodel-0.4.3/src/SQLDataModel/SQLDataModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -8637,15 +8637,15 @@
 
             # Horizontally stack B onto A
             sdm_ab = sdm_a.hstack(sdm_b)
 
             # View stacked model
             print(sdm_ab)
 
-        This will output the result of stacking B onto A, using the each model's headers and dtypes:    
+        This will output the result of stacking B onto A, using each model's headers and dtypes:    
 
         ```shell
             ┌─────┬─────┬─────┬─────┐
             │ A1  │ A2  │ B1  │ B2  │
             ├─────┼─────┼─────┼─────┤
             │ A   │ B   │ C   │ D   │
             │ 1   │ 2   │ 3   │ 4   │
@@ -8677,15 +8677,15 @@
             └─────┴─────┴─────┴─────┴─────┴─────┘
             [2 rows x 6 columns]
         ```
 
         Note:
             - Model dimensions will be truncated or padded to coerce compatible dimensions when stacking, use :meth:`SQLDataModel.merge()` for strict SQL joins instead of hstack.
             - Headers and data types are inherited from all the models being stacked, this requires aliasing duplicate column names if present, see :meth:`SQLDataModel.alias_duplicates()` for aliasing rules.
-            - Use ``setitem`` syntax such as ``sdm['New Column'] = values`` to create new columns directly into the currently model instead of stacking or see :meth:`SQLDataModel.add_column_with_values()` for convenience method accomplishing the same.
+            - Use ``setitem`` syntax such as ``sdm['New Column'] = values`` to create new columns directly into the current model instead of stacking or see :meth:`SQLDataModel.add_column_with_values()` for convenience method accomplishing the same.
             - See :meth:`SQLDataModel.vstack()` for vertical stacking.
         """
         other = list(other[0]) if len(other) == 1 and isinstance(other[0], (list,tuple)) else list(other)
         if len(other) < 1:
             raise ValueError(
                 SQLDataModel.ErrorFormat(f"ValueError: insufficient model count '{len(other)}', at least 1 additional 'SQLDataModel' is required to horizontally stack against")
             )
@@ -9434,14 +9434,134 @@
             by = [self.sql_idx]
         sort_ord = "asc" if asc else "desc"
         sort_by_str = ",".join([f'"{x}" {sort_ord}' for x in by])
         headers_str = ",".join([f'"{col}"' for col in self.headers])
         sort_stmt = " ".join(("select",headers_str,f'from "{self.sql_model}" order by {sort_by_str}'))
         return self.execute_fetch(sort_stmt)
 
+    def strip(self, characters:str=None, str_dtype_only:bool=True, inplace:bool=False) -> SQLDataModel|None:
+        """
+        Removes the specified characters from the beginning and end of each value in the current ``SQLDataModel`` removing leading and trailing whitespace characters by default.
+
+        Parameters:
+            ``characters`` (str, optional): The characters to remove from both ends of the value. Default is None, removing whitespace (``' '``, ``'\\t'``, ``'\\n'``, ``'\\r'``).
+            ``str_dtype_only`` (bool, optional): If True, only columns with dtype = 'str' are stripped, otherwise all columns are stripped. Default is True.
+            ``inplace`` (bool, optional): If True, modifies the current SQLDataModel instance in-place. Default is False.
+        
+        Raises:
+            ``TypeError``: If ``characters`` argument is provided and is not of type ``'str'`` representing unordered characters to remove.
+
+        Returns:
+            ``SQLDataModel``: If ``inplace=False``, returns a new SQLDataModel with the stripped values. Otherwise modifies the current instance in-place returning None.
+
+        Example::
+            
+            from SQLDataModel import SQLDataModel
+
+            # Create a single item model
+            sdm = SQLDataModel([[' Hello, World! ']])
+
+            # Strip whitespace and print
+            print(sdm.strip())
+
+        This will output the model after stripping the leading and trailing whitespace characters:
+
+        ```shell
+            ┌───┬───────────────┐
+            │   │ 0             │
+            ├───┼───────────────┤
+            │ 0 │ Hello, World! │
+            └───┴───────────────┘
+            [1 rows x 1 columns]
+        ```
+
+        Non-whitespace characters can also be stripped:
+
+        ```python
+            from SQLDataModel import SQLDataModel
+
+            headers = ['Col A', 'Col B', 'Col C']
+            data = [
+                ['A1', 'B1', 'C1'],
+                ['A2', 'B2', 'C2'],
+                ['A3', 'B3', 'C3']
+            ]
+
+            # Create the sample model
+            sdm = SQLDataModel(data, headers)
+
+            # Strip leading and trailing 'A' character
+            sdm_stripped = sdm.strip('A')
+
+            # View result
+            print(sdm_stripped)
+        ```
+
+        This will output a new model where any leading and trailing 'A' characters have been removed:
+
+        ```shell
+            ┌───────┬───────┬───────┐
+            │ Col A │ Col B │ Col C │
+            ├───────┼───────┼───────┤
+            │ 1     │ B1    │ C1    │
+            │ 2     │ B2    │ C2    │
+            │ 3     │ B3    │ C3    │
+            └───────┴───────┴───────┘
+            [3 rows x 3 columns]
+        ```
+
+        Multiple characters can be stripped, and the model modified inplace:
+
+        ```python
+            # Strip multiple characters and this time modify model inplace
+            sdm.strip('123', inplace=True)
+
+            # View result
+            print(sdm)
+        ```
+        
+        This will output the modified model after stripping leading and trailing '123' characters:
+
+        ```shell
+            ┌───────┬───────┬───────┐
+            │ Col A │ Col B │ Col C │
+            ├───────┼───────┼───────┤
+            │ A     │ B     │ C     │
+            │ A     │ B     │ C     │
+            │ A     │ B     │ C     │
+            └───────┴───────┴───────┘
+            [3 rows x 3 columns]
+        ```
+
+        Note:
+            - For string replacement instead of string removal, see :meth:`SQLDataModel.replace()`.
+            - When using ``str_dtype_only = False``, numeric values may be modified due to SQLite's type affinity rules.
+            - This method is equivalent to the SQLite ``trim(string, character)`` function, wrapping and passing the equivalent arguments.
+        """
+        if characters is None:
+            trim_arg = """"""
+        else:
+            if not isinstance(characters, str):
+                raise TypeError(
+                    SQLDataModel.ErrorFormat(f"TypeError: invalid type '{type(characters).__name__}', argument for `characters` must be of type 'str' representing an unordered set of characters to remove")
+                )
+            trim_arg = f""",'{characters}'"""
+        if inplace:
+            trim_cols = ",".join([f""" "{col}"=trim("{col}" {trim_arg}) """ for col in self.headers if self.dtypes[col] == 'str']) if str_dtype_only else ",".join([f""" "{col}"=trim("{col}" {trim_arg}) """ for col in self.headers])
+            trim_stmt = " ".join((f"""update "{self.sql_model}" set""", trim_cols))
+            self.sql_db_conn.execute(trim_stmt)
+            return
+        else:
+            if str_dtype_only:
+                trim_cols = ",".join([f""" trim("{col}" {trim_arg}) as "{col}" """ if self.dtypes[col] == 'str' else f""" "{col}" as "{col}" """ for col in self.headers])
+            else:
+                trim_cols = ",".join([f""" trim("{col}" {trim_arg}) as "{col}" """ for col in self.headers])
+            trim_stmt = " ".join(("select", trim_cols, f'from "{self.sql_model}"'))
+            return self.execute_fetch(trim_stmt)
+
     def tail(self, n_rows:int=5) -> SQLDataModel:
         """
         Returns the last ``n_rows`` of the current ``SQLDataModel``.
 
         Parameters:
             ``n_rows`` (int, optional): Number of rows to return. Defaults to 5.
 
@@ -10060,15 +10180,15 @@
             raise SQLProgrammingError(
                 SQLDataModel.ErrorFormat(f"SQLProgrammingError: unable to rename model table, SQL execution failed with: '{e}'")
             ) from None
         self.sql_model = new_name
      
     def execute_fetch(self, sql_query:str, sql_params:tuple=None, **kwargs) -> SQLDataModel:
         """
-        Returns a new ``SQLDataModel`` object after executing the provided SQL query using the current ``SQLDataModel``. 
+        Returns a new ``SQLDataModel`` object, including display and style properties, after executing the provided SQL query using the current ``SQLDataModel``. 
         This method is called by other methods which expect results to be returned from their execution.
 
         Parameters:
             ``sql_query`` (str): The SQL query to execute with the expectation of rows returned.
             ``**kwargs`` (optional): Additional keyword args to pass to ``SQLDataModel`` constructor
 
         Raises:
@@ -10090,14 +10210,17 @@
 
             # Fetch and save the result to a new instance
             result_model = sdm.execute_fetch(query)
 
         Important:
             - The default table name is ``'sdm'``, or you can use :meth:`SQLDataModel.get_model_name()` to view the current model alias.
             - This function is the primary method used by ``SQLDataModel`` methods that are expected to return a new instance.
+
+        Note:
+            - Display properties such as float precision, index column or table styling are also passed to the new instance when not provided in ``kwargs``.
         """
         try:
             res = self.sql_db_conn.execute(sql_query) if sql_params is None else self.sql_db_conn.execute(sql_query, sql_params) 
         except Exception as e:
             raise SQLProgrammingError(
                 SQLDataModel.ErrorFormat(f'SQLProgrammingError: invalid or malformed SQL, provided query failed with error "{e}"')
             ) from None
```

### Comparing `sqldatamodel-0.4.2/src/SQLDataModel/StandardDeviation.py` & `sqldatamodel-0.4.3/src/SQLDataModel/StandardDeviation.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.2/src/SQLDataModel/converters.py` & `sqldatamodel-0.4.3/src/SQLDataModel/converters.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.2/src/SQLDataModel/demo.py` & `sqldatamodel-0.4.3/src/SQLDataModel/demo.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.2/src/SQLDataModel/exceptions.py` & `sqldatamodel-0.4.3/src/SQLDataModel/exceptions.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.2/src/SQLDataModel/extensions/str_utils.c` & `sqldatamodel-0.4.3/src/SQLDataModel/extensions/str_utils.c`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.2/src/SQLDataModel.egg-info/PKG-INFO` & `sqldatamodel-0.4.3/src/SQLDataModel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.4.2
+Version: 0.4.3
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal-tables,pretty-print-tables,sql2sql,data-analysis,data-science,datamodel,extract,transform,load,web-scraping-tables,data-mining,html,html-table-parsing,apache-arrow,pyarrow,pyarrow-conversion,pyarrow-to-table,pyarrow-to-sql,pyarrow-to-csv,parquet-file-parsing,csv,csv-parsing,markdown,markdown-table-parsing,latex,latex-table-parsing,delimited,delimited-data-parsing,file-conversion,format-conversion,terminal-styling,table-styling,from-sqlite,to-sqlite,from-postgresql,to-postgresql,sql-to-sql,excel,xlsx-file,excel-to-sql,DataFrames,polars2pandas,pandas2polars
@@ -61,15 +61,15 @@
 | Mercury |    0.38 |     0 | True     |
 | Venus   |    0.91 |     0 | True     |
 | Mars    |    0.38 |     2 | True     |
 | Saturn  |    0.92 |   146 | True     |
 | Uranus  |    0.89 |    27 | True     |
 ```
 
-Made for those times when you just want to use raw SQL on your dataframe, or need to move data around but the full Pandas, Numpy, SQLAlchemy installation is just overkill. SQLDataModel includes all the most commonly used features, including additional ones like using plan SQL on your `DataFrame` and pretty printing your table, at _1/1000_ the size, 0.03MB vs 30MB
+Made for those times when you just want to use raw SQL on your dataframe, or need to move data around but the full Pandas, Numpy, SQLAlchemy installation is just overkill. SQLDataModel includes all the most commonly used features, including additional ones like using plain SQL on your `DataFrame` and pretty printing your table, at _1/1000_ the size, 0.03MB vs 30MB
 
 ---
 
 ### Installation
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install SQLDataModel.
 
 ```bash
```

### Comparing `sqldatamodel-0.4.2/src/SQLDataModel.egg-info/SOURCES.txt` & `sqldatamodel-0.4.3/src/SQLDataModel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.2/tests/test_Future.py` & `sqldatamodel-0.4.3/tests/test_Future.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,14 +246,35 @@
     output_data = sdm.data()
     for i, row in enumerate(input_data):
         input_target = row[-1].replace('-X','+Y')
         output_target = output_data[i][-1]
         assert input_target == output_target    
 
 @pytest.mark.core
+def test_strip():
+    input_data = [[f" A_{i}", f" B_{i}", f" C_{i}"] for i in range(1,4)]
+    expected_output = [tuple(x.strip() for x in row) for row in input_data]
+    # Test stripping whitespace and returning new model
+    sdm = SQLDataModel(input_data)
+    output_data = sdm.strip(characters=None,inplace=False).data()
+    # Test stripping whitespace inplace
+    assert output_data == expected_output
+    sdm.strip(characters=None,inplace=True)
+    output_data = sdm.data()
+    assert output_data == expected_output
+    # Test stripping different characters and returning as new (now modified from first test)
+    expected_output = [tuple(x.strip().strip('_2') for x in row) for row in input_data]
+    output_data = sdm.strip('_2', inplace=False).data()
+    assert output_data == expected_output
+    # Test stripping different characters inplace
+    sdm.strip('_2', inplace=True)
+    output_data = sdm.data()
+    assert output_data == expected_output    
+
+@pytest.mark.core
 def test_repr():
     ### test data type appearance ###
     input_headers = ['string', 'integer', 'float', 'bool', 'datetime']
     input_data = [
         ('ej6JF', -934, 935.961423, 0, datetime.datetime(1946, 8, 27, 7, 30, 50)),
         ('hYFu', -145, -621.435864, 0, datetime.datetime(1963, 1, 14, 17, 19, 38)),
         ('TwBgAiOuPJ1G', 798, 796.610811, 0, datetime.datetime(1982, 10, 2, 15, 45, 28)),
```

### Comparing `sqldatamodel-0.4.2/tests/test_SQLDataModel.py` & `sqldatamodel-0.4.3/tests/test_SQLDataModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,14 +246,35 @@
     output_data = sdm.data()
     for i, row in enumerate(input_data):
         input_target = row[-1].replace('-X','+Y')
         output_target = output_data[i][-1]
         assert input_target == output_target    
 
 @pytest.mark.core
+def test_strip():
+    input_data = [[f" A_{i}", f" B_{i}", f" C_{i}"] for i in range(1,4)]
+    expected_output = [tuple(x.strip() for x in row) for row in input_data]
+    # Test stripping whitespace and returning new model
+    sdm = SQLDataModel(input_data)
+    output_data = sdm.strip(characters=None,inplace=False).data()
+    # Test stripping whitespace inplace
+    assert output_data == expected_output
+    sdm.strip(characters=None,inplace=True)
+    output_data = sdm.data()
+    assert output_data == expected_output
+    # Test stripping different characters and returning as new (now modified from first test)
+    expected_output = [tuple(x.strip().strip('_2') for x in row) for row in input_data]
+    output_data = sdm.strip('_2', inplace=False).data()
+    assert output_data == expected_output
+    # Test stripping different characters inplace
+    sdm.strip('_2', inplace=True)
+    output_data = sdm.data()
+    assert output_data == expected_output    
+
+@pytest.mark.core
 def test_repr():
     ### test data type appearance ###
     input_headers = ['string', 'integer', 'float', 'bool', 'datetime']
     input_data = [
         ('ej6JF', -934, 935.961423, 0, datetime.datetime(1946, 8, 27, 7, 30, 50)),
         ('hYFu', -145, -621.435864, 0, datetime.datetime(1963, 1, 14, 17, 19, 38)),
         ('TwBgAiOuPJ1G', 798, 796.610811, 0, datetime.datetime(1982, 10, 2, 15, 45, 28)),
```

