# Comparing `tmp/database_mysql_local-0.0.288.tar.gz` & `tmp/database_mysql_local-0.0.289.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.288.tar", last modified: Mon May  6 20:44:29 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.289.tar", last modified: Tue May  7 16:41:05 2024, max compression
```

## Comparing `database_mysql_local-0.0.288.tar` & `database_mysql_local-0.0.289.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:44:29.777999 database_mysql_local-0.0.288/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-06 20:44:29.777999 database_mysql_local-0.0.288/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:44:29.773998 database_mysql_local-0.0.288/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:44:29.777999 database_mysql_local-0.0.288/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    39424 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    31705 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-06 20:43:48.000000 database_mysql_local-0.0.288/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:44:29.777999 database_mysql_local-0.0.288/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-06 20:44:29.000000 database_mysql_local-0.0.288/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-06 20:44:29.000000 database_mysql_local-0.0.288/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 20:44:29.000000 database_mysql_local-0.0.288/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-06 20:44:29.000000 database_mysql_local-0.0.288/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 20:44:29.000000 database_mysql_local-0.0.288/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 20:44:29.777999 database_mysql_local-0.0.288/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:41:05.815959 database_mysql_local-0.0.289/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:57.000000 database_mysql_local-0.0.289/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-07 16:41:05.815959 database_mysql_local-0.0.289/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-07 16:39:57.000000 database_mysql_local-0.0.289/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:41:05.807959 database_mysql_local-0.0.289/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:41:05.815959 database_mysql_local-0.0.289/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:57.000000 database_mysql_local-0.0.289/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-05-07 16:39:57.000000 database_mysql_local-0.0.289/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-07 16:39:57.000000 database_mysql_local-0.0.289/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-07 16:39:57.000000 database_mysql_local-0.0.289/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39344 2024-05-07 16:40:26.000000 database_mysql_local-0.0.289/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31705 2024-05-07 16:39:57.000000 database_mysql_local-0.0.289/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-05-07 16:39:57.000000 database_mysql_local-0.0.289/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-07 16:39:57.000000 database_mysql_local-0.0.289/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-07 16:39:57.000000 database_mysql_local-0.0.289/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-07 16:39:57.000000 database_mysql_local-0.0.289/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-07 16:40:23.000000 database_mysql_local-0.0.289/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-07 16:39:57.000000 database_mysql_local-0.0.289/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-07 16:39:57.000000 database_mysql_local-0.0.289/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:41:05.815959 database_mysql_local-0.0.289/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-07 16:41:05.000000 database_mysql_local-0.0.289/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-07 16:41:05.000000 database_mysql_local-0.0.289/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 16:41:05.000000 database_mysql_local-0.0.289/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-07 16:41:05.000000 database_mysql_local-0.0.289/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-07 16:41:05.000000 database_mysql_local-0.0.289/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-07 16:39:57.000000 database_mysql_local-0.0.289/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 16:41:05.815959 database_mysql_local-0.0.289/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-07 16:39:57.000000 database_mysql_local-0.0.289/setup.py
```

### Comparing `database_mysql_local-0.0.288/PKG-INFO` & `database_mysql_local-0.0.289/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.288
+Version: 0.0.289
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.288/README.md` & `database_mysql_local-0.0.289/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.288/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.289/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.288/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.289/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.288/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.289/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.288/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.289/database_mysql_local/src/generic_crud.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,16 +110,16 @@
         view_table_name = view_table_name or self.default_view_table_name
         id_column_name = self.generate_id_column_name(table_name)
         self._validate_args(args=locals())
         if not data_json:
             self.logger.warning(log_message="GenericCRUD.upsert: data_json is empty")
             return None
         if not data_json_compare:
-            return GenericCRUD.insert(self, schema_name=schema_name, table_name=table_name, data_json=data_json,
-                                      ignore_duplicate=True)
+            return self.insert(schema_name=schema_name, table_name=table_name, data_json=data_json,
+                               ignore_duplicate=True)
 
         columns, values, processed_data_json_compare = process_insert_data_json(data_json=data_json_compare)
         where_clauses = []
         params = []
         for key, value in processed_data_json_compare.items():
             if isinstance(value, list):
                 where_clauses.append(f"({ ' OR '.join([f'{key}=%s' for _ in value]) })")
@@ -127,27 +127,27 @@
             else:
                 where_clauses.append(f"{key}=%s")
                 params.append(value)
 
         where_clause = " OR " if compare_with_or else " AND "
         where_clause = where_clause.join(where_clauses)
 
-        table_id = GenericCRUD.select_one_value_by_where(
-            self, schema_name=schema_name, view_table_name=view_table_name, select_clause_value=id_column_name,
+        table_id = self.select_one_value_by_where(
+            schema_name=schema_name, view_table_name=view_table_name, select_clause_value=id_column_name,
             where=where_clause,
             params=tuple(params),
             order_by=order_by)
         if table_id:
-            GenericCRUD.update_by_id(self, schema_name=schema_name, table_name=table_name,
-                                     id_column_name=id_column_name,
-                                     id_column_value=table_id, data_json=data_json)
+            self.update_by_id(schema_name=schema_name, table_name=table_name,
+                              id_column_name=id_column_name,
+                              id_column_value=table_id, data_json=data_json)
             return table_id
         else:
-            return GenericCRUD.insert(self, schema_name=schema_name, table_name=table_name, data_json=data_json,
-                                      ignore_duplicate=True)
+            return self.insert(schema_name=schema_name, table_name=table_name, data_json=data_json,
+                               ignore_duplicate=True)
 
     def _get_existing_duplicate_id(self, table_name: str, error: Exception) -> int:
         pattern = r'Duplicate entry \'(.+?)\' for key \'(.+?)\''
         match = re.search(pattern, str(error))
         if not match:  # a different error
             raise error
         duplicate_value = match.group(1)
```

### Comparing `database_mysql_local-0.0.288/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.289/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.288/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.289/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.288/database_mysql_local/src/point.py` & `database_mysql_local-0.0.289/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.288/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.289/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.288/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.289/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.288/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.289/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.288/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.289/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.288/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.289/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.288/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.289/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.288
+Version: 0.0.289
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.288/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.289/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.288/pyproject.toml` & `database_mysql_local-0.0.289/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "database-mysql-local"
-version = "0.0.288" # https://pypi.org/project/database-mysql-local
+version = "0.0.289" # https://pypi.org/project/database-mysql-local
 description = "database-mysql-local Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
 
 # dephell deps convert --from pyproject.toml --from-format poetry --to setup.py --to-format setuppy
```

### Comparing `database_mysql_local-0.0.288/setup.py` & `database_mysql_local-0.0.289/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 package_dir = PACKAGE_NAME.replace("-", "_")
 # TODO: we are migrating from circles_local_database_python to database_mysql_local
 #  but in the meantime we want to keep both names
 old_name = "circles_local_database_python"
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.288',
+    version='0.0.289',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir, old_name],
     package_dir={package_dir: f'{package_dir}/src', old_name: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

