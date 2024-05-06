# Comparing `tmp/pyprql-0.8.0.tar.gz` & `tmp/pyprql-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprql-0.8.0.tar", max compression
+gzip compressed data, was "pyprql-0.9.0.tar", max compression
```

## Comparing `pyprql-0.8.0.tar` & `pyprql-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    10284 2023-04-15 04:20:51.643572 pyprql-0.8.0/LICENSE
--rw-r--r--   0        0        0     2278 2023-04-15 04:20:51.643572 pyprql-0.8.0/README.md
--rw-r--r--   0        0        0     2213 2023-04-15 04:21:27.104441 pyprql-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      140 2023-04-15 04:21:27.068440 pyprql-0.8.0/pyprql/__init__.py
--rw-r--r--   0        0        0     6502 2023-04-15 04:20:51.643572 pyprql-0.8.0/pyprql/magic/README.md
--rw-r--r--   0        0        0      689 2023-04-15 04:20:51.643572 pyprql-0.8.0/pyprql/magic/__init__.py
--rw-r--r--   0        0        0     4440 2023-04-15 04:20:51.643572 pyprql-0.8.0/pyprql/magic/prql.py
--rw-r--r--   0        0        0      246 2023-04-15 04:20:51.643572 pyprql-0.8.0/pyprql/pandas_accessor/__init__.py
--rw-r--r--   0        0        0      878 2023-04-15 04:20:51.643572 pyprql-0.8.0/pyprql/pandas_accessor/prql.py
--rw-r--r--   0        0        0        0 2023-04-15 04:20:51.643572 pyprql-0.8.0/pyprql/py.typed
--rw-r--r--   0        0        0      645 2023-04-15 04:20:51.643572 pyprql-0.8.0/pyprql/tests/__init__.py
--rw-r--r--   0        0        0       30 2023-04-15 04:20:51.643572 pyprql-0.8.0/pyprql/tests/_regtest_outputs/test_magic.test_memory_db.out
--rw-r--r--   0        0        0       33 2023-04-15 04:20:51.643572 pyprql-0.8.0/pyprql/tests/_regtest_outputs/test_magic.test_pass_existing_engine.out
--rw-r--r--   0        0        0     1947 2023-04-15 04:20:51.643572 pyprql-0.8.0/pyprql/tests/conftest.py
--rw-r--r--   0        0        0    14569 2023-04-15 04:20:51.643572 pyprql-0.8.0/pyprql/tests/test_magic.py
--rw-r--r--   0        0        0     3037 2023-04-15 04:20:51.643572 pyprql-0.8.0/pyprql/tests/test_prql_python.py
--rw-r--r--   0        0        0     3399 1970-01-01 00:00:00.000000 pyprql-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    10284 2023-07-25 23:12:05.247011 pyprql-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2280 2023-07-25 23:12:05.247011 pyprql-0.9.0/README.md
+-rw-r--r--   0        0        0     2245 2023-07-25 23:12:42.961155 pyprql-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      140 2023-07-25 23:12:05.251011 pyprql-0.9.0/pyprql/__init__.py
+-rw-r--r--   0        0        0     6502 2023-07-25 23:12:05.251011 pyprql-0.9.0/pyprql/magic/README.md
+-rw-r--r--   0        0        0      689 2023-07-25 23:12:05.251011 pyprql-0.9.0/pyprql/magic/__init__.py
+-rw-r--r--   0        0        0     4440 2023-07-25 23:12:05.251011 pyprql-0.9.0/pyprql/magic/prql.py
+-rw-r--r--   0        0        0      246 2023-07-25 23:12:05.251011 pyprql-0.9.0/pyprql/pandas_accessor/__init__.py
+-rw-r--r--   0        0        0      878 2023-07-25 23:12:05.251011 pyprql-0.9.0/pyprql/pandas_accessor/prql.py
+-rw-r--r--   0        0        0        0 2023-07-25 23:12:05.251011 pyprql-0.9.0/pyprql/py.typed
+-rw-r--r--   0        0        0      645 2023-07-25 23:12:05.251011 pyprql-0.9.0/pyprql/tests/__init__.py
+-rw-r--r--   0        0        0       30 2023-07-25 23:12:05.251011 pyprql-0.9.0/pyprql/tests/_regtest_outputs/test_magic.test_memory_db.out
+-rw-r--r--   0        0        0       33 2023-07-25 23:12:05.251011 pyprql-0.9.0/pyprql/tests/_regtest_outputs/test_magic.test_pass_existing_engine.out
+-rw-r--r--   0        0        0     1947 2023-07-25 23:12:05.251011 pyprql-0.9.0/pyprql/tests/conftest.py
+-rw-r--r--   0        0        0    14569 2023-07-25 23:12:05.251011 pyprql-0.9.0/pyprql/tests/test_magic.py
+-rw-r--r--   0        0        0     3045 2023-07-25 23:12:05.251011 pyprql-0.9.0/pyprql/tests/test_prql_python.py
+-rw-r--r--   0        0        0     3201 1970-01-01 00:00:00.000000 pyprql-0.9.0/PKG-INFO
```

### Comparing `pyprql-0.8.0/LICENSE` & `pyprql-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprql-0.8.0/README.md` & `pyprql-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,30 +29,30 @@
 ### Pandas integration
 
 ```python
 import pandas as pd
 import pyprql.pandas_accessor
 
 df = (...)
-results_df = df.prql.query("select [age,name,occupation] | filter age > 21")
+results_df = df.prql.query("select {age, name, occupation} | filter age > 21")
 ```
 
 ### Jupyter Magic
 
 ```python
 In [1]: %load_ext pyprql.magic
 In [2]: %prql postgresql://user:password@localhost:5432/database
 In [3]: %%prql
    ...: from p
    ...: group categoryID (
-   ...:   aggregate [average unitPrice]
+   ...:   aggregate {average unitPrice}
    ...: )
 In [4]: %%prql results <<
    ...: from p
-   ...: aggregate [min unitsInStock, max unitsInStock]
+   ...: aggregate {min unitsInStock, max unitsInStock}
 
 ```
 
 ### Compilation
 
 This library exposes `prql-python.compile`, so we can simply generate SQL:
```

### Comparing `pyprql-0.8.0/pyproject.toml` & `pyprql-0.9.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -15,67 +15,66 @@
 ]
 description = "Python extensions for PRQL"
 homepage = "https://prql-lang.org"
 license = "Apache-2.0"
 name = "pyprql"
 readme = "README.md"
 repository = "https://github.com/prql/pyprql"
-version = "0.8.0"
+version = "0.9.0"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
-duckdb-engine = "^0.7"
+duckdb-engine = ">=0.7,<0.10"
 ipython = "^8"
 jupysql = ">=0.7"
 pandas = ">=1.5"
-prql-python = "^0.8"
+prql-python = "^0.9"
 traitlets = "^5"
 
 [tool.poetry.dev-dependencies]
-Sphinx = "~4.3"
-black = "^22.1.0"
-commitizen = "^2.21.2"
-coverage = "^6.3.2"
+Sphinx = "~6.2"
+black = "^23.7.0"
+commitizen = "^3.5.2"
+coverage = "^7.2.7"
 darglint = "^1.8.1"
-mypy = "^0.982"
-myst-parser = "^0.17.0"
-nox = "^2022.1.7"
-pre-commit = "^2.17.0"
-# pytest-regtest compat
-pytest = "<7.2"
+mypy = "^1.4"
+myst-parser = "^2.0.0"
+nox = "^2023.4.22"
+polars = ">=0.16"
+pre-commit = "^3.3.2"
+pytest = ">7"
+# pytest-regtest compat https://gitlab.com/uweschmitt/pytest-regtest/-/merge_requests/9
+py = "1.11"
 pytest-clarity = "^1.0.1"
-pytest-cov = "^3.0.0"
+pytest-cov = "^4.1.0"
 pytest-regtest = "*"
 pytest-sugar = "^0.9.4"
 pytest-testmon = "*"
-pytest-xdist = "^2.5.0"
-python-semantic-release = "^7.32.2"
-ruff = "^0.0.225"
+pytest-xdist = "^3.3.1"
+python-semantic-release = "^8.0.1"
+ruff = "^0.0.270"
 safety = "^2"
-sphinx-rtd-theme = "^1.0.0"
-xdoctest = "^0.15.10"
-polars = ">=0.16"
-
-[tool.poetry.scripts]
-pyprql = "pyprql.cli.__init__:main"
+sphinx-rtd-theme = "^1.2.1"
+xdoctest = "^1.1.1"
+twine = "^4.0.2"
 
 [tool.semantic_release]
 branch = "main"
 build_command = "poetry build"
 changelog_file = "CHANGELOG.md"
+major_on_zero = false
 upload_to_pypi = true
 upload_to_release = true
 version_toml = [
   "pyproject.toml:tool.poetry.version",
 ]
 version_variable = [
   "pyprql/__init__.py:__version__",
 ]
-major_on_zero = false
 
 [tool.pytest.ini_options]
 addopts = """
 --xdoctest
 """
 
 [tool.coverage.run]
```

### Comparing `pyprql-0.8.0/pyprql/magic/README.md` & `pyprql-0.9.0/pyprql/magic/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 2          3  Aniseed Syrup           1           2  12 - 550 ml bottles       10.0            13            70            25             0
 ```
 
 ```
 In [5]: %%prql
    ...: from p = `products.csv`
    ...: group categoryID (
-   ...:   aggregate [average unitPrice]
+   ...:   aggregate {average unitPrice}
    ...: )
 
 Done.
 Returning data to local variable _
    categoryID  avg("unitPrice")
 0           1         37.979167
 1           2         23.062500
@@ -119,28 +119,28 @@
 ```
 
 We can capture the results into a different variable like so:
 
 ```
 In [6]: %%prql results <<
    ...: from p = `products.csv`
-   ...: aggregate [min unitsInStock, max unitsInStock]
+   ...: aggregate {min unitsInStock, max unitsInStock}
 
 Done.
 Returning data to local variable results
    min("unitsInStock")  max("unitsInStock")
 0                    0                  125
 ```
 
 Now, the output of the query is saved to `results`.
 
 We can also use a line magic to capture the results like this:
 
 ```
-In [7]: results = %prql from p = `products.csv` | aggregate [min unitsInStock, max unitsInStock]
+In [7]: results = %prql from p = `products.csv` | aggregate {min unitsInStock, max unitsInStock}
 ```
 
 ## Configuration
 
 We strive to provide sane defaults;
 however,
 should you need to change settings,
```

### Comparing `pyprql-0.8.0/pyprql/magic/__init__.py` & `pyprql-0.9.0/pyprql/magic/__init__.py`

 * *Files identical despite different names*

### Comparing `pyprql-0.8.0/pyprql/magic/prql.py` & `pyprql-0.9.0/pyprql/magic/prql.py`

 * *Files identical despite different names*

### Comparing `pyprql-0.8.0/pyprql/pandas_accessor/prql.py` & `pyprql-0.9.0/pyprql/pandas_accessor/prql.py`

 * *Files identical despite different names*

### Comparing `pyprql-0.8.0/pyprql/tests/__init__.py` & `pyprql-0.9.0/pyprql/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyprql-0.8.0/pyprql/tests/conftest.py` & `pyprql-0.9.0/pyprql/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyprql-0.8.0/pyprql/tests/test_magic.py` & `pyprql-0.9.0/pyprql/tests/test_magic.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 def test_html(ip):
     result = run_prql(ip, "from test")
     assert "<td>foo</td>" in result._repr_html_().lower()
 
 
 def test_line_magic(ip):
-    result = ip.run_line_magic("prql", "from      test   |     select [name]")
+    result = ip.run_line_magic("prql", "from      test   |     select {name}")
     assert "foo" in str(result)
 
 
 @pytest.mark.skip(reason="We only support pandas")
 def test_print(ip):
     result = run_prql(ip, "from test")
     assert re.search(r"1\s+\|\s+foo", str(result))
@@ -105,15 +105,15 @@
 
 def test_duplicate_column_names_accepted(ip):
     ip.run_line_magic("config", "SqlMagic.autopandas = False")
     result = ip.run_cell_magic(
         "prql",
         "sqlite://",
         """
-        from author | select [last_name, last_name]
+        from author | select {last_name, last_name}
         """,
     )
     assert ("Brecht", "Brecht") in result
 
 
 def test_persist(ip):
     ip.run_line_magic("config", "SqlMagic.autopandas = False")
```

### Comparing `pyprql-0.8.0/pyprql/tests/test_prql_python.py` & `pyprql-0.9.0/pyprql/tests/test_prql_python.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,46 +6,46 @@
 @pytest.fixture(autouse=True)
 def import_accessor():
     import pyprql.pandas_accessor  # noqa
 
 
 def test_pyql_python():
     """It compiles sql from prql."""
-    sql: str = prql.compile("from employees | select [ name, age ]").replace("\n", " ")
+    sql: str = prql.compile("from employees | select {name, age}").replace("\n", " ")
     assert sql.startswith("SELECT   name,   age FROM   employees")
 
 
 def test_df_accessor():
     df = pd.DataFrame({"latitude": [1, 2, 3], "longitude": [1, 2, 3]})
-    res = df.prql.query("select [latitude, longitude] | filter latitude > 1")
+    res = df.prql.query("select {latitude, longitude} | filter latitude > 1")
     assert len(res.index) == 2
     assert res.iloc[0]["latitude"] == 2
     assert res.iloc[1]["latitude"] == 3
 
 
 def test_target_dialect():
     df = pd.DataFrame({"foo": ["a"], "bar": ["b"]})
-    res = df.prql.query("select ![bar]")  # duckdb supports EXCLUDE
+    res = df.prql.query("select !{bar}")  # duckdb supports EXCLUDE
     assert len(res.columns) == 1
 
 
 def test_df_supports_grouped_aggs():
     rows = {
         "title": ["ceo", "developer", "wizard"],
         "country": ["USA", "USA", "Slovenia"],
         "salary": [120, 100, 130],
     }
     df = pd.DataFrame(rows)
     res = df.prql.query(
         """
-        group [country] (
-          aggregate [
+        group {country} (
+          aggregate {
             avg_sal = average salary,
-            ct = count
-          ]
+            ct = count this
+          }
         )
         """
     )
 
     row1 = res.iloc[0]
     row2 = res.iloc[1]
 
@@ -55,29 +55,29 @@
     assert row1["avg_sal"] == 110
     assert row2["avg_sal"] == 130
 
 
 def test_df_big_prql_query():
     q = """
         filter start_date > @2021-01-01
-        derive [
+        derive {
           gross_salary = salary + tax ?? 0,
           gross_cost = gross_salary + benefits_cost,
-        ]
+        }
         filter gross_cost > 0
-        group [title, country] (
-          aggregate [
+        group {title, country} (
+          aggregate {
             avg_gross_salary = average gross_salary,
             sum_gross_cost = sum gross_cost,
-            cnt = count
-          ]
+            cnt = count this
+          }
         )
         filter sum_gross_cost > 100
         derive id = f"{title}_{country}"
-        sort [sum_gross_cost, -country]
+        sort {sum_gross_cost, -country}
         take 1..20
         """
     rows = {
         "title": ["developer", "developer", "wizard", "horologist"],
         "country": ["USA", "USA", "Slovenia", "Slovenia"],
         "benefits_cost": [10, 20, 50, 0],
         "salary": [120, 100, 130, 0],
```

### Comparing `pyprql-0.8.0/PKG-INFO` & `pyprql-0.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 Metadata-Version: 2.1
 Name: pyprql
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python extensions for PRQL
 Home-page: https://prql-lang.org
 License: Apache-2.0
 Author: Charlie Sanders
 Author-email: charlie.fats@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Typing :: Typed
-Requires-Dist: duckdb-engine (>=0.7,<0.8)
+Requires-Dist: duckdb-engine (>=0.7,<0.10)
 Requires-Dist: ipython (>=8,<9)
 Requires-Dist: jupysql (>=0.7)
 Requires-Dist: pandas (>=1.5)
-Requires-Dist: prql-python (>=0.8,<0.9)
+Requires-Dist: prql-python (>=0.9,<0.10)
 Requires-Dist: traitlets (>=5,<6)
 Project-URL: Repository, https://github.com/prql/pyprql
 Description-Content-Type: text/markdown
 
 # pyprql
 
 [![CI/CD](https://github.com/prql/pyprql/actions/workflows/pull-request.yaml/badge.svg?branch=main)](https://github.com/prql/pyprql/actions/workflows/pull-request.yaml)
@@ -59,30 +55,30 @@
 ### Pandas integration
 
 ```python
 import pandas as pd
 import pyprql.pandas_accessor
 
 df = (...)
-results_df = df.prql.query("select [age,name,occupation] | filter age > 21")
+results_df = df.prql.query("select {age, name, occupation} | filter age > 21")
 ```
 
 ### Jupyter Magic
 
 ```python
 In [1]: %load_ext pyprql.magic
 In [2]: %prql postgresql://user:password@localhost:5432/database
 In [3]: %%prql
    ...: from p
    ...: group categoryID (
-   ...:   aggregate [average unitPrice]
+   ...:   aggregate {average unitPrice}
    ...: )
 In [4]: %%prql results <<
    ...: from p
-   ...: aggregate [min unitsInStock, max unitsInStock]
+   ...: aggregate {min unitsInStock, max unitsInStock}
 
 ```
 
 ### Compilation
 
 This library exposes `prql-python.compile`, so we can simply generate SQL:
```

