# Comparing `tmp/backtesting_server-0.4.1.tar.gz` & `tmp/backtesting_server-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backtesting_server-0.4.1.tar", max compression
+gzip compressed data, was "backtesting_server-0.4.2.tar", max compression
```

## Comparing `backtesting_server-0.4.1.tar` & `backtesting_server-0.4.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1089 2024-04-03 23:27:00.840175 backtesting_server-0.4.1/LICENSE
--rw-r--r--   0        0        0      628 2024-05-06 16:53:04.522719 backtesting_server-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1858 2024-04-15 23:43:05.933161 backtesting_server-0.4.1/README.md
--rw-r--r--   0        0        0      202 2024-05-06 11:19:03.439830 backtesting_server-0.4.1/src/backtesting_server/__init__.py
--rw-r--r--   0        0        0    24794 2024-05-06 16:52:41.967220 backtesting_server-0.4.1/src/backtesting_server/main.py
--rw-r--r--   0        0        0     2465 1970-01-01 00:00:00.000000 backtesting_server-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-03 23:27:00.840175 backtesting_server-0.4.2/LICENSE
+-rw-r--r--   0        0        0      628 2024-05-06 21:00:22.813298 backtesting_server-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1858 2024-04-15 23:43:05.933161 backtesting_server-0.4.2/README.md
+-rw-r--r--   0        0        0      202 2024-05-06 11:19:03.439830 backtesting_server-0.4.2/src/backtesting_server/__init__.py
+-rw-r--r--   0        0        0    24795 2024-05-06 20:58:06.527831 backtesting_server-0.4.2/src/backtesting_server/main.py
+-rw-r--r--   0        0        0     2465 1970-01-01 00:00:00.000000 backtesting_server-0.4.2/PKG-INFO
```

### Comparing `backtesting_server-0.4.1/LICENSE` & `backtesting_server-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `backtesting_server-0.4.1/pyproject.toml` & `backtesting_server-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "backtesting-server"
-version = "0.4.1"
+version = "0.4.2"
 description = "Package to interact with MySQL server, recording results of the backtesting."
 authors = ["hnewey7 <hnewey7@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `backtesting_server-0.4.1/README.md` & `backtesting_server-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `backtesting_server-0.4.1/src/backtesting_server/main.py` & `backtesting_server-0.4.2/src/backtesting_server/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
       return True
 
   def _create_historical_data_summary(self) -> None:
     """ Creating the historical data summary on the MySQL server."""
     try:
       self.cursor.execute('CREATE TABLE HistoricalDataSummary (\
       ID INT NOT NULL AUTO_INCREMENT,\
-      InstrumentName VARCHAR(20),\
+      InstrumentName VARCHAR(100),\
       Epic VARCHAR(100),\
       LiveTracking BOOL DEFAULT False,\
       InstrumentGroup SET("") DEFAULT NULL,\
       PRIMARY KEY (ID)\
       );')
       logger.info("Created Historical Data Summary.")
     except:
```

### Comparing `backtesting_server-0.4.1/PKG-INFO` & `backtesting_server-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backtesting-server
-Version: 0.4.1
+Version: 0.4.2
 Summary: Package to interact with MySQL server, recording results of the backtesting.
 License: MIT
 Author: hnewey7
 Author-email: hnewey7@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

