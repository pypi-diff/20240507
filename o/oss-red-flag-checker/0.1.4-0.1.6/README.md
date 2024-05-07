# Comparing `tmp/oss_red_flag_checker-0.1.4.tar.gz` & `tmp/oss_red_flag_checker-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oss_red_flag_checker-0.1.4.tar", max compression
+gzip compressed data, was "oss_red_flag_checker-0.1.6.tar", max compression
```

## Comparing `oss_red_flag_checker-0.1.4.tar` & `oss_red_flag_checker-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    11358 2024-02-06 13:11:41.082730 oss_red_flag_checker-0.1.4/LICENSE.txt
-drwxr-xr-x   0        0        0        0 2024-02-06 13:11:41.082730 oss_red_flag_checker-0.1.4/LICENSES/
--rw-r--r--   0        0        0     8418 2024-02-06 13:11:41.086730 oss_red_flag_checker-0.1.4/README.md
--rw-r--r--   0        0        0      394 2024-02-06 13:11:41.086730 oss_red_flag_checker-0.1.4/ossrfc/__init__.py
--rw-r--r--   0        0        0     9540 2024-02-06 13:11:41.086730 oss_red_flag_checker-0.1.4/ossrfc/_analysis.py
--rw-r--r--   0        0        0     5022 2024-02-06 13:11:41.086730 oss_red_flag_checker-0.1.4/ossrfc/_contributions.py
--rw-r--r--   0        0        0     7619 2024-02-06 13:11:41.086730 oss_red_flag_checker-0.1.4/ossrfc/_git.py
--rw-r--r--   0        0        0     7564 2024-02-06 13:11:41.086730 oss_red_flag_checker-0.1.4/ossrfc/_licensing.py
--rw-r--r--   0        0        0      870 2024-02-06 13:11:41.086730 oss_red_flag_checker-0.1.4/ossrfc/_matching.py
--rw-r--r--   0        0        0     5798 2024-02-06 13:11:41.086730 oss_red_flag_checker-0.1.4/ossrfc/_report.py
--rw-r--r--   0        0        0     7691 2024-02-06 13:11:41.086730 oss_red_flag_checker-0.1.4/ossrfc/checker.py
--rw-r--r--   0        0        0     1410 2024-02-06 13:11:41.086730 oss_red_flag_checker-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     9699 1970-01-01 00:00:00.000000 oss_red_flag_checker-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-07 11:51:38.804883 oss_red_flag_checker-0.1.6/LICENSE.txt
+drwxr-xr-x   0        0        0        0 2024-05-07 11:51:38.804883 oss_red_flag_checker-0.1.6/LICENSES/
+-rw-r--r--   0        0        0    11358 2024-05-07 11:51:38.804883 oss_red_flag_checker-0.1.6/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0     8418 2024-05-07 11:51:38.804883 oss_red_flag_checker-0.1.6/README.md
+-rw-r--r--   0        0        0      394 2024-05-07 11:51:38.804883 oss_red_flag_checker-0.1.6/ossrfc/__init__.py
+-rw-r--r--   0        0        0     9540 2024-05-07 11:51:38.804883 oss_red_flag_checker-0.1.6/ossrfc/_analysis.py
+-rw-r--r--   0        0        0     5022 2024-05-07 11:51:38.804883 oss_red_flag_checker-0.1.6/ossrfc/_contributions.py
+-rw-r--r--   0        0        0     7619 2024-05-07 11:51:38.804883 oss_red_flag_checker-0.1.6/ossrfc/_git.py
+-rw-r--r--   0        0        0     7564 2024-05-07 11:51:38.804883 oss_red_flag_checker-0.1.6/ossrfc/_licensing.py
+-rw-r--r--   0        0        0      870 2024-05-07 11:51:38.804883 oss_red_flag_checker-0.1.6/ossrfc/_matching.py
+-rw-r--r--   0        0        0     5798 2024-05-07 11:51:38.804883 oss_red_flag_checker-0.1.6/ossrfc/_report.py
+-rw-r--r--   0        0        0     7691 2024-05-07 11:51:38.804883 oss_red_flag_checker-0.1.6/ossrfc/checker.py
+-rw-r--r--   0        0        0     1415 2024-05-07 11:51:38.804883 oss_red_flag_checker-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     9699 1970-01-01 00:00:00.000000 oss_red_flag_checker-0.1.6/PKG-INFO
```

### Comparing `oss_red_flag_checker-0.1.4/LICENSE.txt` & `oss_red_flag_checker-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oss_red_flag_checker-0.1.4/README.md` & `oss_red_flag_checker-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `oss_red_flag_checker-0.1.4/ossrfc/_analysis.py` & `oss_red_flag_checker-0.1.6/ossrfc/_analysis.py`

 * *Files identical despite different names*

### Comparing `oss_red_flag_checker-0.1.4/ossrfc/_contributions.py` & `oss_red_flag_checker-0.1.6/ossrfc/_contributions.py`

 * *Files identical despite different names*

### Comparing `oss_red_flag_checker-0.1.4/ossrfc/_git.py` & `oss_red_flag_checker-0.1.6/ossrfc/_git.py`

 * *Files identical despite different names*

### Comparing `oss_red_flag_checker-0.1.4/ossrfc/_licensing.py` & `oss_red_flag_checker-0.1.6/ossrfc/_licensing.py`

 * *Files identical despite different names*

### Comparing `oss_red_flag_checker-0.1.4/ossrfc/_matching.py` & `oss_red_flag_checker-0.1.6/ossrfc/_matching.py`

 * *Files identical despite different names*

### Comparing `oss_red_flag_checker-0.1.4/ossrfc/_report.py` & `oss_red_flag_checker-0.1.6/ossrfc/_report.py`

 * *Files identical despite different names*

### Comparing `oss_red_flag_checker-0.1.4/ossrfc/checker.py` & `oss_red_flag_checker-0.1.6/ossrfc/checker.py`

 * *Files identical despite different names*

### Comparing `oss_red_flag_checker-0.1.4/pyproject.toml` & `oss_red_flag_checker-0.1.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2023 DB Systel GmbH
 #
 # SPDX-License-Identifier: Apache-2.0
 
 [tool.poetry]
 name = "oss-red-flag-checker"
-version = "0.1.4"
+version = "0.1.6"
 description = "Check remote repositories for typical red flags like CLAs and risks due to low development activity"
 authors = ["Open Source at Deutsche Bahn <opensource@deutschebahn.com>"]
 maintainers = ["Max Mehl <max.mehl@deutschebahn.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/dbsystel/oss-red-flag-checker/"
 keywords = ["ospo", "open-source-management", "supply-chain", "risk-analysis"]
@@ -26,15 +26,15 @@
 tqdm = "^4.66.1"
 termcolor = "^2.3.0"
 
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
 pylint = "^2.17.5"
-black = "^23.7.0"
+black = ">=23.7,<25.0"
 pylama = "^8.4.1"
 mypy = "^1.5.1"
 types-tqdm = "^4.66.0.2"
 pytest = "^7.4.2"
 pytest-cov = "^4.1.0"
 
 [tool.poetry.scripts]
```

### Comparing `oss_red_flag_checker-0.1.4/PKG-INFO` & `oss_red_flag_checker-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oss-red-flag-checker
-Version: 0.1.4
+Version: 0.1.6
 Summary: Check remote repositories for typical red flags like CLAs and risks due to low development activity
 Home-page: https://github.com/dbsystel/oss-red-flag-checker/
 License: Apache-2.0
 Keywords: ospo,open-source-management,supply-chain,risk-analysis
 Author: Open Source at Deutsche Bahn
 Author-email: opensource@deutschebahn.com
 Maintainer: Max Mehl
```

