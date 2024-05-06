# Comparing `tmp/nsj_sql_utils_lib-1.3.4.tar.gz` & `tmp/nsj_sql_utils_lib-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_sql_utils_lib-1.3.4.tar", last modified: Tue Apr 30 23:43:01 2024, max compression
+gzip compressed data, was "nsj_sql_utils_lib-2.0.0.tar", last modified: Mon May  6 22:56:02 2024, max compression
```

## Comparing `nsj_sql_utils_lib-1.3.4.tar` & `nsj_sql_utils_lib-2.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-30 23:43:01.752900 nsj_sql_utils_lib-1.3.4/
--rw-r--r--   0 sergio    (1000) sergio    (1000)     5136 2024-04-30 23:43:01.752900 nsj_sql_utils_lib-1.3.4/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4366 2024-04-18 17:44:27.000000 nsj_sql_utils_lib-1.3.4/README.md
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-30 23:43:01.748900 nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-22 21:56:47.000000 nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      925 2024-01-12 20:44:34.000000 nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib/dao_util.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     6275 2024-04-30 23:33:41.000000 nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib/dbadapter3.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2166 2024-04-30 22:57:24.000000 nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib/dbconection.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      916 2024-04-30 22:23:54.000000 nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib/dbconection_mysql_connector.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1005 2024-04-30 22:30:45.000000 nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib/dbconection_psycopg2.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-30 23:43:01.752900 nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib/updater/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2024-01-12 20:44:34.000000 nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib/updater/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1040 2024-04-18 17:44:27.000000 nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib/updater/create_script.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1809 2024-01-12 20:44:34.000000 nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib/updater/db_updater.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     9738 2024-04-18 17:44:27.000000 nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib/updater/erp_database_updater.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      341 2024-01-02 22:09:17.000000 nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib/updater/vars.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-30 23:43:01.752900 nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib.egg-info/
--rw-r--r--   0 sergio    (1000) sergio    (1000)     5136 2024-04-30 23:43:01.000000 nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib.egg-info/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      691 2024-04-30 23:43:01.000000 nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2024-04-30 23:43:01.000000 nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       89 2024-04-30 23:43:01.000000 nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib.egg-info/requires.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       18 2024-04-30 23:43:01.000000 nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib.egg-info/top_level.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-22 22:03:17.000000 nsj_sql_utils_lib-1.3.4/pyproject.toml
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      868 2024-04-30 23:43:01.752900 nsj_sql_utils_lib-1.3.4/setup.cfg
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-05-06 22:56:02.200920 nsj_sql_utils_lib-2.0.0/
+-rw-r--r--   0 sergio    (1000) sergio    (1000)     5136 2024-05-06 22:56:02.200920 nsj_sql_utils_lib-2.0.0/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4366 2024-04-18 17:44:27.000000 nsj_sql_utils_lib-2.0.0/README.md
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-05-06 22:56:02.200920 nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-22 21:56:47.000000 nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      925 2024-01-12 20:44:34.000000 nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib/dao_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     6256 2024-05-06 22:23:45.000000 nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib/dbadapter3.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2168 2024-05-06 22:25:04.000000 nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib/dbconnection.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      916 2024-04-30 22:23:54.000000 nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib/dbconnection_mysql_connector.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1005 2024-04-30 22:30:45.000000 nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib/dbconnection_psycopg2.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-05-06 22:56:02.200920 nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib/updater/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2024-01-12 20:44:34.000000 nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib/updater/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1040 2024-04-18 17:44:27.000000 nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib/updater/create_script.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1799 2024-05-06 22:25:00.000000 nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib/updater/db_updater.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     9738 2024-04-18 17:44:27.000000 nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib/updater/erp_database_updater.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      341 2024-01-02 22:09:17.000000 nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib/updater/vars.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-05-06 22:56:02.200920 nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib.egg-info/
+-rw-r--r--   0 sergio    (1000) sergio    (1000)     5136 2024-05-06 22:56:02.000000 nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      694 2024-05-06 22:56:02.000000 nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2024-05-06 22:56:02.000000 nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       89 2024-05-06 22:56:02.000000 nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib.egg-info/requires.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       18 2024-05-06 22:56:02.000000 nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib.egg-info/top_level.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-22 22:03:17.000000 nsj_sql_utils_lib-2.0.0/pyproject.toml
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      868 2024-05-06 22:56:02.200920 nsj_sql_utils_lib-2.0.0/setup.cfg
```

### Comparing `nsj_sql_utils_lib-1.3.4/PKG-INFO` & `nsj_sql_utils_lib-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj_sql_utils_lib
-Version: 1.3.4
+Version: 2.0.0
 Summary: Biblioteca de utilitários Python para facilitar a implementação de sistemas com acesso a banco de dados.
 Home-page: https://github.com/Nasajon/nsj-sql-utils-lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj-sql-utils-lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_sql_utils_lib-1.3.4/README.md` & `nsj_sql_utils_lib-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib/dao_util.py` & `nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib/dao_util.py`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib/dbadapter3.py` & `nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib/dbadapter3.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,14 @@
 
     def _ajustar_query_sqlalchemy(self, sql: str, pars: dict[str, any]):
         sql = re.sub(r"%\(([^\(\)]+)\)s", r":\1", sql)
         return SQLParams("named", "format").format(sql, pars)
 
     def _ajustar_query_adapter2_to3(self, sql: str):
         sql = re.sub(r":([^ \n,\)\"/]+)", r"%(\1)s", sql)
-        re.match()
         return sql
 
     def execute_query_to_model(self, sql: str, model_class: object, **kwargs) -> list:
         """
         Executando uma instrução sql com retorno.
 
         O retorno é feito em forma de uma lista (list), com elementos do tipo passado pelo parâmetro
```

### Comparing `nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib/dbconection.py` & `nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib/dbconnection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import enum
 
-from nsj_sql_utils_lib.dbconection_mysql_connector import DBConnectionMySQLConnector
-from nsj_sql_utils_lib.dbconection_psycopg2 import DBConnectionPsycopg2
+from nsj_sql_utils_lib.dbconnection_mysql_connector import DBConnectionMySQLConnector
+from nsj_sql_utils_lib.dbconnection_psycopg2 import DBConnectionPsycopg2
 
 
 class DBConnectionDriver(enum.Enum):
     POSTGRES = "POSTGRES"
     SINGLE_STORE = "SINGLE_STORE"
     MYSQL = "MYSQL"
```

### Comparing `nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib/dbconection_mysql_connector.py` & `nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib/dbconnection_mysql_connector.py`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib/dbconection_psycopg2.py` & `nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib/dbconnection_psycopg2.py`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib/updater/create_script.py` & `nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib/updater/create_script.py`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib/updater/erp_database_updater.py` & `nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib/updater/erp_database_updater.py`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib.egg-info/PKG-INFO` & `nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj_sql_utils_lib
-Version: 1.3.4
+Version: 2.0.0
 Summary: Biblioteca de utilitários Python para facilitar a implementação de sistemas com acesso a banco de dados.
 Home-page: https://github.com/Nasajon/nsj-sql-utils-lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj-sql-utils-lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_sql_utils_lib-1.3.4/nsj_sql_utils_lib.egg-info/SOURCES.txt` & `nsj_sql_utils_lib-2.0.0/nsj_sql_utils_lib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 README.md
 pyproject.toml
 setup.cfg
 ./nsj_sql_utils_lib/__init__.py
 ./nsj_sql_utils_lib/dao_util.py
 ./nsj_sql_utils_lib/dbadapter3.py
-./nsj_sql_utils_lib/dbconection.py
-./nsj_sql_utils_lib/dbconection_mysql_connector.py
-./nsj_sql_utils_lib/dbconection_psycopg2.py
+./nsj_sql_utils_lib/dbconnection.py
+./nsj_sql_utils_lib/dbconnection_mysql_connector.py
+./nsj_sql_utils_lib/dbconnection_psycopg2.py
 ./nsj_sql_utils_lib.egg-info/PKG-INFO
 ./nsj_sql_utils_lib.egg-info/SOURCES.txt
 ./nsj_sql_utils_lib.egg-info/dependency_links.txt
 ./nsj_sql_utils_lib.egg-info/requires.txt
 ./nsj_sql_utils_lib.egg-info/top_level.txt
 ./nsj_sql_utils_lib/updater/__init__.py
 ./nsj_sql_utils_lib/updater/create_script.py
```

### Comparing `nsj_sql_utils_lib-1.3.4/setup.cfg` & `nsj_sql_utils_lib-2.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nsj_sql_utils_lib
-version = 1.3.4
+version = 2.0.0
 author = Nasajon Sistemas
 author_email = contact.dev@nasajon.com.br
 description = Biblioteca de utilitários Python para facilitar a implementação de sistemas com acesso a banco de dados.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nasajon/nsj-sql-utils-lib
 project_urls =
```

