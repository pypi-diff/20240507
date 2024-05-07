# Comparing `tmp/finml_utils-2.1.9.tar.gz` & `tmp/finml_utils-2.2.0.tar.gz`

## Comparing `finml_utils-2.1.9.tar` & `finml_utils-2.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 finml_utils-2.1.9/codecov.yml
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 finml_utils-2.1.9/src/finml_utils/__init__.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 finml_utils-2.1.9/src/finml_utils/dataframes.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 finml_utils-2.1.9/src/finml_utils/enums.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 finml_utils-2.1.9/src/finml_utils/files.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 finml_utils-2.1.9/src/finml_utils/introspection.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 finml_utils-2.1.9/src/finml_utils/list.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 finml_utils-2.1.9/src/finml_utils/parallel.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 finml_utils-2.1.9/src/finml_utils/returns.py
--rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 finml_utils-2.1.9/src/finml_utils/s3_store.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 finml_utils-2.1.9/src/finml_utils/shuffle.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 finml_utils-2.1.9/src/finml_utils/stats.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 finml_utils-2.1.9/.gitignore
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 finml_utils-2.1.9/README.md
--rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 finml_utils-2.1.9/pyproject.toml
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 finml_utils-2.1.9/PKG-INFO
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 finml_utils-2.2.0/codecov.yml
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 finml_utils-2.2.0/src/finml_utils/__init__.py
+-rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 finml_utils-2.2.0/src/finml_utils/dataframes.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 finml_utils-2.2.0/src/finml_utils/enums.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 finml_utils-2.2.0/src/finml_utils/files.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 finml_utils-2.2.0/src/finml_utils/introspection.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 finml_utils-2.2.0/src/finml_utils/list.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 finml_utils-2.2.0/src/finml_utils/parallel.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 finml_utils-2.2.0/src/finml_utils/returns.py
+-rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 finml_utils-2.2.0/src/finml_utils/s3_store.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 finml_utils-2.2.0/src/finml_utils/shuffle.py
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 finml_utils-2.2.0/src/finml_utils/stats.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 finml_utils-2.2.0/src/finml_utils/transformations.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 finml_utils-2.2.0/.gitignore
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 finml_utils-2.2.0/README.md
+-rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 finml_utils-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 finml_utils-2.2.0/PKG-INFO
```

### Comparing `finml_utils-2.1.9/src/finml_utils/dataframes.py` & `finml_utils-2.2.0/src/finml_utils/dataframes.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,7 +145,15 @@
     Rebase all series to a given intial base.
     This makes comparing/plotting different series together easier.
     Args:
         * prices: Expects a price series/dataframe
         * base (number): starting value for all series.
     """
     return prices.dropna() / prices.dropna().iloc[0] * base
+
+
+
+
+def get_delisted_columns(data: pd.DataFrame, timeframe: int) -> list[str]:
+    isnan_period = data.iloc[-timeframe:].isna().sum().sort_values(ascending=False)
+    is_discountinued = isnan_period == len(data.iloc[-timeframe:])
+    return is_discountinued[is_discountinued].index.to_list()
```

### Comparing `finml_utils-2.1.9/src/finml_utils/list.py` & `finml_utils-2.2.0/src/finml_utils/list.py`

 * *Files identical despite different names*

### Comparing `finml_utils-2.1.9/src/finml_utils/parallel.py` & `finml_utils-2.2.0/src/finml_utils/parallel.py`

 * *Files identical despite different names*

### Comparing `finml_utils-2.1.9/src/finml_utils/returns.py` & `finml_utils-2.2.0/src/finml_utils/returns.py`

 * *Files identical despite different names*

### Comparing `finml_utils-2.1.9/src/finml_utils/s3_store.py` & `finml_utils-2.2.0/src/finml_utils/s3_store.py`

 * *Files identical despite different names*

### Comparing `finml_utils-2.1.9/src/finml_utils/shuffle.py` & `finml_utils-2.2.0/src/finml_utils/shuffle.py`

 * *Files identical despite different names*

### Comparing `finml_utils-2.1.9/src/finml_utils/stats.py` & `finml_utils-2.2.0/src/finml_utils/stats.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,19 +9,35 @@
     res = returns.mean() / divisor
 
     if isnan(res):
         return -10.0
 
     return res * sqrt(annualization_period)
 
+
 def beta(returns: pd.Series, underlying: pd.Series) -> float:
     matrix = np.cov(returns, underlying.loc[returns.index])
     return matrix[0, 1] / matrix[1, 1]
 
 
+def alpha(
+    returns: pd.Series, underlying: pd.Series, annualization_period: int | None = None
+) -> float:
+    return (returns.mean() - beta(returns, underlying) * underlying.mean()) * (
+        annualization_period or 1
+    )
+
+
+def geometric_alpha(
+    returns: pd.Series, underlying: pd.Series, annualization_period: int | None = None
+) -> float:
+    return (
+        np.log1p(returns) - beta(returns, underlying) * np.log1p(underlying).mean()
+    ) * (annualization_period or 1)
+
 
 def sortino(returns, annualization_period: int) -> float:
     downside = np.sqrt((returns[returns < 0] ** 2).sum() / len(returns))
     res = returns.mean() / downside
     return res * sqrt(annualization_period)
```

### Comparing `finml_utils-2.1.9/.gitignore` & `finml_utils-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `finml_utils-2.1.9/pyproject.toml` & `finml_utils-2.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "finml-utils"
-version = "2.1.9"
+version = "2.2.0"
 authors = [
   { name="Mark Aron Szulyovszky", email="mark@dreamfaster.ai" },
   { name="Daniel Szemerey", email="daniel@dreamfaster.ai" },
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python",
@@ -50,15 +50,15 @@
   "pytest~=7.1.2",
   "pytest-cov>=4.0",
 ]
 
 
 # bumpver command: ``bumpver update --patch``
 [tool.bumpver]
-current_version = "2.1.9"
+current_version = "2.2.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore(Release): Bump version from {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `finml_utils-2.1.9/PKG-INFO` & `finml_utils-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: finml-utils
-Version: 2.1.9
+Version: 2.2.0
 Project-URL: Issues, https://github.com/dream-faster/finml-utils/issues
 Project-URL: Source, https://github.com/dream-faster/finml-utils
 Author-email: Mark Aron Szulyovszky <mark@dreamfaster.ai>, Daniel Szemerey <daniel@dreamfaster.ai>
 License-Expression: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

