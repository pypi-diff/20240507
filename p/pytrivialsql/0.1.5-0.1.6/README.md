# Comparing `tmp/pytrivialsql-0.1.5.tar.gz` & `tmp/pytrivialsql-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrivialsql-0.1.5.tar", last modified: Sun May  5 21:22:13 2024, max compression
+gzip compressed data, was "pytrivialsql-0.1.6.tar", last modified: Tue May  7 14:57:02 2024, max compression
```

## Comparing `pytrivialsql-0.1.5.tar` & `pytrivialsql-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:22:13.844227 pytrivialsql-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-05 21:21:57.000000 pytrivialsql-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-05 21:22:13.844227 pytrivialsql-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-05 21:21:57.000000 pytrivialsql-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-05 21:21:57.000000 pytrivialsql-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 21:22:13.844227 pytrivialsql-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:22:13.844227 pytrivialsql-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:22:13.844227 pytrivialsql-0.1.5/src/pytrivialsql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 21:21:57.000000 pytrivialsql-0.1.5/src/pytrivialsql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-05-05 21:21:57.000000 pytrivialsql-0.1.5/src/pytrivialsql/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-05 21:21:57.000000 pytrivialsql-0.1.5/src/pytrivialsql/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-05 21:21:57.000000 pytrivialsql-0.1.5/src/pytrivialsql/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:22:13.844227 pytrivialsql-0.1.5/src/pytrivialsql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-05 21:22:13.000000 pytrivialsql-0.1.5/src/pytrivialsql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-05 21:22:13.000000 pytrivialsql-0.1.5/src/pytrivialsql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 21:22:13.000000 pytrivialsql-0.1.5/src/pytrivialsql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-05 21:22:13.000000 pytrivialsql-0.1.5/src/pytrivialsql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-05 21:22:13.000000 pytrivialsql-0.1.5/src/pytrivialsql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:22:13.844227 pytrivialsql-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-05 21:21:57.000000 pytrivialsql-0.1.5/tests/test_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-05-05 21:21:57.000000 pytrivialsql-0.1.5/tests/test_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-05 21:21:57.000000 pytrivialsql-0.1.5/tests/test_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:02.012923 pytrivialsql-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-07 14:56:43.000000 pytrivialsql-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-07 14:57:02.012923 pytrivialsql-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-07 14:56:43.000000 pytrivialsql-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-07 14:56:43.000000 pytrivialsql-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 14:57:02.012923 pytrivialsql-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:02.008923 pytrivialsql-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:02.008923 pytrivialsql-0.1.6/src/pytrivialsql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:56:43.000000 pytrivialsql-0.1.6/src/pytrivialsql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-07 14:56:43.000000 pytrivialsql-0.1.6/src/pytrivialsql/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-07 14:56:43.000000 pytrivialsql-0.1.6/src/pytrivialsql/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-07 14:56:43.000000 pytrivialsql-0.1.6/src/pytrivialsql/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:02.012923 pytrivialsql-0.1.6/src/pytrivialsql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-07 14:57:02.000000 pytrivialsql-0.1.6/src/pytrivialsql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-07 14:57:02.000000 pytrivialsql-0.1.6/src/pytrivialsql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:57:02.000000 pytrivialsql-0.1.6/src/pytrivialsql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 14:57:02.000000 pytrivialsql-0.1.6/src/pytrivialsql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 14:57:02.000000 pytrivialsql-0.1.6/src/pytrivialsql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:02.012923 pytrivialsql-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-07 14:56:43.000000 pytrivialsql-0.1.6/tests/test_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-05-07 14:56:43.000000 pytrivialsql-0.1.6/tests/test_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-07 14:56:43.000000 pytrivialsql-0.1.6/tests/test_sqlite.py
```

### Comparing `pytrivialsql-0.1.5/LICENSE` & `pytrivialsql-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrivialsql-0.1.5/pyproject.toml` & `pytrivialsql-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytrivialsql"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="inaimathi", email="leo.zovic@gmail.com" },
 ]
 description = "A trivial set of QOL bindings for SQL in Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pytrivialsql-0.1.5/src/pytrivialsql/postgres.py` & `pytrivialsql-0.1.6/src/pytrivialsql/postgres.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         returning = args.get("returning", args.get("RETURNING", None))
         try:
             with self._conn.cursor() as cur:
                 for k, v in args.items():
                     if k in {"returning", "RETURNING"}:
                         if type(v) is str:
                             args[k] = [v]
-                    if type(v) in _JSON_TYPES:
+                    elif type(v) in _JSON_TYPES:
                         args[k] = json.dumps(v)
                 args["placeholder"] = "%s"
                 q, qargs = sql.insert_q(table_name, **args)
                 cur.execute(q, qargs)
                 if returning is None:
                     res = None
                 else:
```

### Comparing `pytrivialsql-0.1.5/src/pytrivialsql/sql.py` & `pytrivialsql-0.1.6/src/pytrivialsql/sql.py`

 * *Files identical despite different names*

### Comparing `pytrivialsql-0.1.5/src/pytrivialsql/sqlite.py` & `pytrivialsql-0.1.6/src/pytrivialsql/sqlite.py`

 * *Files identical despite different names*

### Comparing `pytrivialsql-0.1.5/tests/test_postgres.py` & `pytrivialsql-0.1.6/tests/test_postgres.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,11 +53,18 @@
         )
         self.assertEqual(select_res[0]["a_column"], "a row")
         self.assertFalse(select_res[0]["another_column"])
 
         rid = DB.insert("a_table", a_column="another row", RETURNING="id")
         self.assertIsInstance(rid, int)
 
+        rlist = DB.insert(
+            "a_table",
+            a_column="another row",
+            RETURNING=["id", "a_column", "a_json_column"],
+        )
+        self.assertIsInstance(rlist, dict)
+
         DB.drop("a_table")
         with self.assertRaises(psycopg.errors.UndefinedTable):
             DB.select("a_table", "*")
         DB.close()
```

### Comparing `pytrivialsql-0.1.5/tests/test_sql.py` & `pytrivialsql-0.1.6/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `pytrivialsql-0.1.5/tests/test_sqlite.py` & `pytrivialsql-0.1.6/tests/test_sqlite.py`

 * *Files identical despite different names*

