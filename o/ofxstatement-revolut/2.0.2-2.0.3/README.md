# Comparing `tmp/ofxstatement-revolut-2.0.2.tar.gz` & `tmp/ofxstatement_revolut-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofxstatement-revolut-2.0.2.tar", last modified: Sat Jan 22 10:51:56 2022, max compression
+gzip compressed data, was "ofxstatement_revolut-2.0.3.tar", last modified: Tue May  7 15:40:01 2024, max compression
```

## Comparing `ofxstatement-revolut-2.0.2.tar` & `ofxstatement_revolut-2.0.3.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-22 10:51:56.540946 ofxstatement-revolut-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-01-22 10:51:39.000000 ofxstatement-revolut-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3303 2022-01-22 10:51:56.540946 ofxstatement-revolut-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1371 2022-01-22 10:51:39.000000 ofxstatement-revolut-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-22 10:51:56.540946 ofxstatement-revolut-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1635 2022-01-22 10:51:39.000000 ofxstatement-revolut-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-22 10:51:56.536946 ofxstatement-revolut-2.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-22 10:51:56.536946 ofxstatement-revolut-2.0.2/src/ofxstatement/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-01-22 10:51:39.000000 ofxstatement-revolut-2.0.2/src/ofxstatement/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-22 10:51:56.536946 ofxstatement-revolut-2.0.2/src/ofxstatement/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-01-22 10:51:39.000000 ofxstatement-revolut-2.0.2/src/ofxstatement/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4078 2022-01-22 10:51:39.000000 ofxstatement-revolut-2.0.2/src/ofxstatement/plugins/revolut.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-22 10:51:56.540946 ofxstatement-revolut-2.0.2/src/ofxstatement_revolut.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3303 2022-01-22 10:51:56.000000 ofxstatement-revolut-2.0.2/src/ofxstatement_revolut.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-01-22 10:51:56.000000 ofxstatement-revolut-2.0.2/src/ofxstatement_revolut.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-22 10:51:56.000000 ofxstatement-revolut-2.0.2/src/ofxstatement_revolut.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-01-22 10:51:56.000000 ofxstatement-revolut-2.0.2/src/ofxstatement_revolut.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-01-22 10:51:56.000000 ofxstatement-revolut-2.0.2/src/ofxstatement_revolut.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-01-22 10:51:56.000000 ofxstatement-revolut-2.0.2/src/ofxstatement_revolut.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-01-22 10:51:56.000000 ofxstatement-revolut-2.0.2/src/ofxstatement_revolut.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-22 10:51:41.000000 ofxstatement-revolut-2.0.2/src/ofxstatement_revolut.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:40:01.118986 ofxstatement_revolut-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-07 15:39:50.000000 ofxstatement_revolut-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-07 15:40:01.118986 ofxstatement_revolut-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-07 15:39:50.000000 ofxstatement_revolut-2.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 15:40:01.118986 ofxstatement_revolut-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-07 15:39:50.000000 ofxstatement_revolut-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:40:01.118986 ofxstatement_revolut-2.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:40:01.118986 ofxstatement_revolut-2.0.3/src/ofxstatement/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-07 15:39:50.000000 ofxstatement_revolut-2.0.3/src/ofxstatement/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:40:01.118986 ofxstatement_revolut-2.0.3/src/ofxstatement/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-07 15:39:50.000000 ofxstatement_revolut-2.0.3/src/ofxstatement/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-07 15:39:50.000000 ofxstatement_revolut-2.0.3/src/ofxstatement/plugins/revolut.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:40:01.118986 ofxstatement_revolut-2.0.3/src/ofxstatement_revolut.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-07 15:40:01.000000 ofxstatement_revolut-2.0.3/src/ofxstatement_revolut.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-07 15:40:01.000000 ofxstatement_revolut-2.0.3/src/ofxstatement_revolut.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 15:40:01.000000 ofxstatement_revolut-2.0.3/src/ofxstatement_revolut.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-07 15:40:01.000000 ofxstatement_revolut-2.0.3/src/ofxstatement_revolut.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 15:40:01.000000 ofxstatement_revolut-2.0.3/src/ofxstatement_revolut.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-07 15:40:01.000000 ofxstatement_revolut-2.0.3/src/ofxstatement_revolut.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 15:40:01.000000 ofxstatement_revolut-2.0.3/src/ofxstatement_revolut.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 15:39:54.000000 ofxstatement_revolut-2.0.3/src/ofxstatement_revolut.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:40:01.118986 ofxstatement_revolut-2.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-07 15:39:50.000000 ofxstatement_revolut-2.0.3/tests/test_revolut.py
```

### Comparing `ofxstatement-revolut-2.0.2/LICENSE` & `ofxstatement_revolut-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ofxstatement-revolut-2.0.2/PKG-INFO` & `ofxstatement_revolut-2.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: ofxstatement-revolut
-Version: 2.0.2
+Version: 2.0.3
 Summary: Bank statement parser for Revolut
 Home-page: https://github.com/mlaitinen/ofxstatement-revolut
 Author: Miku Laitinen
 Author-email: miku@avoin.systems
 License: GPLv3
 Keywords: ofx,ofxstatement,banking,statement,revolut
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Utilities
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: ofxstatement>=0.7.2
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 # ofxstatement-revolut
 
 ![badge](https://github.com/mlaitinen/ofxstatement-revolut/actions/workflows/build-and-publish.yml/badge.svg)
 
 
 This is a plugin for [ofxstatement](https://github.com/kedder/ofxstatement). It implements
@@ -41,20 +42,25 @@
 ```
 git clone https://github.com/mlaitinen/ofxstatement-revolut.git
 python3 setup.py install
 ```
 
 ## Configuration options
 
-| Option        | Description                                                                                                                                    |
-|---------------|------------------------------------------------------------------------------------------------------------------------------------------------|
-| `account`     | Define the account of this bank statement                                                                                                      |
-| `currency`    | The base currency of the account                                                                                                               |
-| `date_format` | The date format in the bank statement. Note that you have to use double `%`-marks in the settings file like this: `date_format = %%b %%d, %%Y` |
+| Option        | Description                                                                                                                                               |
+|---------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `account`     | Define the account of this bank statement                                                                                                                 |
+| `currency`    | The base currency of the account                                                                                                                          |
+| `date_format` | The date format in the bank statement. Note that you have to use double `%`-marks in the settings file like this: `date_format = %%Y-%%m-%%d %%H:%%M:%%S` |
+
 
+2.0.3
+-----
+- Use ATM types for ATM events, XFER type for EXCHANGE operations, and add FEE type (thanks @3v1n0)
+- Handle empty balance fields (thanks @3v1n0)
 
 2.0.2
 -----
 - Ignore other than COMPLETED transactions. Pending transactions have their own structure in OFX
   called STMTTRNP, but ofxstatement doesn't support it.
 - Include the "Started Date" as the date the user initiated the transaction.
 
@@ -101,9 +107,7 @@
 
 - Support April 2018 CSV format
 
 1.0.0
 -----
 
 - First release
-
-
```

### Comparing `ofxstatement-revolut-2.0.2/README.md` & `ofxstatement_revolut-2.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,12 +19,12 @@
 ```
 git clone https://github.com/mlaitinen/ofxstatement-revolut.git
 python3 setup.py install
 ```
 
 ## Configuration options
 
-| Option        | Description                                                                                                                                    |
-|---------------|------------------------------------------------------------------------------------------------------------------------------------------------|
-| `account`     | Define the account of this bank statement                                                                                                      |
-| `currency`    | The base currency of the account                                                                                                               |
-| `date_format` | The date format in the bank statement. Note that you have to use double `%`-marks in the settings file like this: `date_format = %%b %%d, %%Y` |
+| Option        | Description                                                                                                                                               |
+|---------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `account`     | Define the account of this bank statement                                                                                                                 |
+| `currency`    | The base currency of the account                                                                                                                          |
+| `date_format` | The date format in the bank statement. Note that you have to use double `%`-marks in the settings file like this: `date_format = %%Y-%%m-%%d %%H:%%M:%%S` |
```

### Comparing `ofxstatement-revolut-2.0.2/setup.py` & `ofxstatement_revolut-2.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 from setuptools import find_packages
 from setuptools.command.test import test as TestCommand
 from distutils.core import setup
 
 import unittest
 
-version = "2.0.2"
+version = "2.0.3"
 
 setup(name="ofxstatement-revolut",
       version=version,
       author="Miku Laitinen",
       author_email="miku@avoin.systems",
       url="https://github.com/mlaitinen/ofxstatement-revolut",
       description=("Bank statement parser for Revolut"),
```

### Comparing `ofxstatement-revolut-2.0.2/src/ofxstatement/plugins/revolut.py` & `ofxstatement_revolut-2.0.3/src/ofxstatement/plugins/revolut.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 from ofxstatement.statement import StatementLine, Currency, Statement
 
 TRANSACTION_TYPES = {
     "TRANSFER": "XFER",
     "CARD_PAYMENT": "POS",
     "CARD_REFUND": "POS",
     "TOPUP": "DEP",
-    "EXCHANGE": "OTHER",
-    # "???": "ATM",  # TODO: What's Revolut's type for ATM transactions?
+    "EXCHANGE": "XFER",
+    "ATM": "ATM",
+    "FEE": "FEE",
 }
 
 
 class RevolutCSVStatementParser(CsvStatementParser):
 
     __slots__ = 'columns'
 
@@ -54,15 +55,16 @@
         # Ignore pending charges
         if line[c["State"]] != "COMPLETED":
             return None
 
         stmt_line = super().parse_record(line)
 
         # Generate a unique ID
-        balance = self.parse_float(line[c["Balance"]])
+        balance_content = line[c["Balance"]]
+        balance = self.parse_float(balance_content) if balance_content else 0
         stmt_line.id = md5(f"{stmt_line.date}-{stmt_line.payee}-{stmt_line.amount}-{balance}".encode())\
             .hexdigest()
 
         return stmt_line
 
     # noinspection PyUnresolvedReferences
     def parse(self) -> Statement:
```

### Comparing `ofxstatement-revolut-2.0.2/src/ofxstatement_revolut.egg-info/PKG-INFO` & `ofxstatement_revolut-2.0.3/src/ofxstatement_revolut.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: ofxstatement-revolut
-Version: 2.0.2
+Version: 2.0.3
 Summary: Bank statement parser for Revolut
 Home-page: https://github.com/mlaitinen/ofxstatement-revolut
 Author: Miku Laitinen
 Author-email: miku@avoin.systems
 License: GPLv3
 Keywords: ofx,ofxstatement,banking,statement,revolut
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Utilities
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: ofxstatement>=0.7.2
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 # ofxstatement-revolut
 
 ![badge](https://github.com/mlaitinen/ofxstatement-revolut/actions/workflows/build-and-publish.yml/badge.svg)
 
 
 This is a plugin for [ofxstatement](https://github.com/kedder/ofxstatement). It implements
@@ -41,20 +42,25 @@
 ```
 git clone https://github.com/mlaitinen/ofxstatement-revolut.git
 python3 setup.py install
 ```
 
 ## Configuration options
 
-| Option        | Description                                                                                                                                    |
-|---------------|------------------------------------------------------------------------------------------------------------------------------------------------|
-| `account`     | Define the account of this bank statement                                                                                                      |
-| `currency`    | The base currency of the account                                                                                                               |
-| `date_format` | The date format in the bank statement. Note that you have to use double `%`-marks in the settings file like this: `date_format = %%b %%d, %%Y` |
+| Option        | Description                                                                                                                                               |
+|---------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `account`     | Define the account of this bank statement                                                                                                                 |
+| `currency`    | The base currency of the account                                                                                                                          |
+| `date_format` | The date format in the bank statement. Note that you have to use double `%`-marks in the settings file like this: `date_format = %%Y-%%m-%%d %%H:%%M:%%S` |
+
 
+2.0.3
+-----
+- Use ATM types for ATM events, XFER type for EXCHANGE operations, and add FEE type (thanks @3v1n0)
+- Handle empty balance fields (thanks @3v1n0)
 
 2.0.2
 -----
 - Ignore other than COMPLETED transactions. Pending transactions have their own structure in OFX
   called STMTTRNP, but ofxstatement doesn't support it.
 - Include the "Started Date" as the date the user initiated the transaction.
 
@@ -101,9 +107,7 @@
 
 - Support April 2018 CSV format
 
 1.0.0
 -----
 
 - First release
-
-
```

