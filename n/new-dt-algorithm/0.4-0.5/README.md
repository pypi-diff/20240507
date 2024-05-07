# Comparing `tmp/new_dt_algorithm-0.4.tar.gz` & `tmp/new_dt_algorithm-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "new_dt_algorithm-0.4.tar", last modified: Tue May  7 11:31:54 2024, max compression
+gzip compressed data, was "new_dt_algorithm-0.5.tar", last modified: Tue May  7 12:00:30 2024, max compression
```

## Comparing `new_dt_algorithm-0.4.tar` & `new_dt_algorithm-0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 11:31:54.644910 new_dt_algorithm-0.4/
--rw-rw-rw-   0        0        0      214 2024-05-07 11:31:54.644910 new_dt_algorithm-0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-07 11:26:56.000000 new_dt_algorithm-0.4/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 11:31:54.644910 new_dt_algorithm-0.4/new_dt_algorithm.egg-info/
--rw-rw-rw-   0        0        0      214 2024-05-07 11:31:54.000000 new_dt_algorithm-0.4/new_dt_algorithm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2024-05-07 11:31:54.000000 new_dt_algorithm-0.4/new_dt_algorithm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 11:31:54.000000 new_dt_algorithm-0.4/new_dt_algorithm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-07 11:31:54.000000 new_dt_algorithm-0.4/new_dt_algorithm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    21625 2024-05-07 09:22:37.000000 new_dt_algorithm-0.4/new_dt_algorithm.py
--rw-rw-rw-   0        0        0       42 2024-05-07 11:31:54.644910 new_dt_algorithm-0.4/setup.cfg
--rw-rw-rw-   0        0        0      443 2024-05-07 11:31:37.000000 new_dt_algorithm-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:00:30.550313 new_dt_algorithm-0.5/
+-rw-rw-rw-   0        0        0      214 2024-05-07 12:00:30.550313 new_dt_algorithm-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:26:56.000000 new_dt_algorithm-0.5/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:00:30.550313 new_dt_algorithm-0.5/new_dt_algorithm.egg-info/
+-rw-rw-rw-   0        0        0      214 2024-05-07 12:00:30.000000 new_dt_algorithm-0.5/new_dt_algorithm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-07 12:00:30.000000 new_dt_algorithm-0.5/new_dt_algorithm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 12:00:30.000000 new_dt_algorithm-0.5/new_dt_algorithm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-07 12:00:30.000000 new_dt_algorithm-0.5/new_dt_algorithm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    21648 2024-05-07 11:56:18.000000 new_dt_algorithm-0.5/new_dt_algorithm.py
+-rw-rw-rw-   0        0        0       42 2024-05-07 12:00:30.550313 new_dt_algorithm-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      443 2024-05-07 11:59:49.000000 new_dt_algorithm-0.5/setup.py
```

### Comparing `new_dt_algorithm-0.4/new_dt_algorithm.py` & `new_dt_algorithm-0.5/new_dt_algorithm.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
         Parameters:
             data (DataFrame): Input DataFrame.
             Target (str): Name of the target variable.
             na_impute (int, optional): Value to use for imputing missing values. Default is -99999.
         """
         import pandas as pd
-
+        self.__init__()
         self.data = data
         self.Target = Target.lower()
         self.data.columns = self.data.columns.str.lower()
         self.data[self.Target] = pd.to_numeric(self.data[self.Target], errors='coerce')
         self.data = self.data.dropna(axis=1, how="all")
         self.data = self.data.dropna(axis=0, how="all")
         self.data = self.data.fillna(na_impute)
```

