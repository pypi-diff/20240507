# Comparing `tmp/unnecessary_abstraction-1.0.1.tar.gz` & `tmp/unnecessary_abstraction-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unnecessary_abstraction-1.0.1.tar", max compression
+gzip compressed data, was "unnecessary_abstraction-1.0.2.tar", max compression
```

## Comparing `unnecessary_abstraction-1.0.1.tar` & `unnecessary_abstraction-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      424 2024-05-05 12:25:40.569669 unnecessary_abstraction-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-05 12:17:36.486574 unnecessary_abstraction-1.0.1/README.md
--rw-r--r--   0        0        0      306 2024-04-17 21:48:39.000000 unnecessary_abstraction-1.0.1/unnecessary-abstraction/__init__.py
--rw-r--r--   0        0        0     3789 2024-04-17 10:39:30.000000 unnecessary_abstraction-1.0.1/unnecessary-abstraction/database.py
--rw-r--r--   0        0        0    15397 2024-02-24 03:42:20.000000 unnecessary_abstraction-1.0.1/unnecessary-abstraction/database_interface.py
--rw-r--r--   0        0        0     1499 2024-04-09 10:09:47.000000 unnecessary_abstraction-1.0.1/unnecessary-abstraction/postgis_interface.py
--rw-r--r--   0        0        0    16687 2024-05-05 02:12:30.904945 unnecessary_abstraction-1.0.1/unnecessary-abstraction/postgres_interface.py
--rw-r--r--   0        0        0     3801 2024-05-05 02:09:59.336969 unnecessary_abstraction-1.0.1/unnecessary-abstraction/schema_objects.py
--rw-r--r--   0        0        0    12833 2024-05-05 02:09:29.709757 unnecessary_abstraction-1.0.1/unnecessary-abstraction/sqlite_interface.py
--rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 unnecessary_abstraction-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      306 2024-04-17 21:48:39.000000 unnecessary_abstraction-1.0.2/database_interface/__init__.py
+-rw-r--r--   0        0        0     3789 2024-04-17 10:39:30.000000 unnecessary_abstraction-1.0.2/database_interface/database.py
+-rw-r--r--   0        0        0    15397 2024-02-24 03:42:20.000000 unnecessary_abstraction-1.0.2/database_interface/database_interface.py
+-rw-r--r--   0        0        0     1499 2024-04-09 10:09:47.000000 unnecessary_abstraction-1.0.2/database_interface/postgis_interface.py
+-rw-r--r--   0        0        0    16687 2024-05-06 13:30:00.401742 unnecessary_abstraction-1.0.2/database_interface/postgres_interface.py
+-rw-r--r--   0        0        0     3801 2024-05-05 02:09:59.336969 unnecessary_abstraction-1.0.2/database_interface/schema_objects.py
+-rw-r--r--   0        0        0    12833 2024-05-05 02:09:29.709757 unnecessary_abstraction-1.0.2/database_interface/sqlite_interface.py
+-rw-r--r--   0        0        0      419 2024-05-07 00:14:00.579999 unnecessary_abstraction-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-05 12:17:36.486574 unnecessary_abstraction-1.0.2/README.md
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 unnecessary_abstraction-1.0.2/PKG-INFO
```

### Comparing `unnecessary_abstraction-1.0.1/unnecessary-abstraction/database.py` & `unnecessary_abstraction-1.0.2/database_interface/database.py`

 * *Files identical despite different names*

### Comparing `unnecessary_abstraction-1.0.1/unnecessary-abstraction/database_interface.py` & `unnecessary_abstraction-1.0.2/database_interface/database_interface.py`

 * *Files identical despite different names*

### Comparing `unnecessary_abstraction-1.0.1/unnecessary-abstraction/postgis_interface.py` & `unnecessary_abstraction-1.0.2/database_interface/postgis_interface.py`

 * *Files identical despite different names*

### Comparing `unnecessary_abstraction-1.0.1/unnecessary-abstraction/postgres_interface.py` & `unnecessary_abstraction-1.0.2/database_interface/postgres_interface.py`

 * *Files identical despite different names*

### Comparing `unnecessary_abstraction-1.0.1/unnecessary-abstraction/schema_objects.py` & `unnecessary_abstraction-1.0.2/database_interface/schema_objects.py`

 * *Files identical despite different names*

### Comparing `unnecessary_abstraction-1.0.1/unnecessary-abstraction/sqlite_interface.py` & `unnecessary_abstraction-1.0.2/database_interface/sqlite_interface.py`

 * *Files identical despite different names*

