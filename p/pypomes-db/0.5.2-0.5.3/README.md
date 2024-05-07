# Comparing `tmp/pypomes_db-0.5.2.tar.gz` & `tmp/pypomes_db-0.5.3.tar.gz`

## Comparing `pypomes_db-0.5.2.tar` & `pypomes_db-0.5.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 pypomes_db-0.5.2/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 pypomes_db-0.5.2/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    26033 2020-02-02 00:00:00.000000 pypomes_db-0.5.2/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.2/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    12464 2020-02-02 00:00:00.000000 pypomes_db-0.5.2/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    10253 2020-02-02 00:00:00.000000 pypomes_db-0.5.2/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    10367 2020-02-02 00:00:00.000000 pypomes_db-0.5.2/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.5.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.5.2/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.2/README.md
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pypomes_db-0.5.3/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 pypomes_db-0.5.3/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    29559 2020-02-02 00:00:00.000000 pypomes_db-0.5.3/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.3/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    15841 2020-02-02 00:00:00.000000 pypomes_db-0.5.3/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    13749 2020-02-02 00:00:00.000000 pypomes_db-0.5.3/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    13882 2020-02-02 00:00:00.000000 pypomes_db-0.5.3/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.5.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.5.3/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.3/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.5.3/PKG-INFO
```

### Comparing `pypomes_db-0.5.2/src/pypomes_db/__init__.py` & `pypomes_db-0.5.3/src/pypomes_db/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from .db_pomes import (
     db_setup, db_get_engines, db_get_params,
     db_assert_connection, db_connect, db_exists,
     db_select_one, db_select_all, db_update,
-    db_delete, db_insert, db_bulk_insert,
+    db_delete, db_insert, db_bulk_insert, db_bulk_copy,
     db_execute, db_call_function, db_call_procedure,
 )
 
 __all__ = [
     # db_pomes
     "db_setup", "db_get_engines", "db_get_params",
     "db_assert_connection", "db_connect", "db_exists",
     "db_select_one", "db_select_all", "db_update",
-    "db_delete", "db_insert", "db_bulk_insert",
+    "db_delete", "db_insert", "db_bulk_insert", "db_bulk_copy",
     "db_execute", "db_call_function", "db_call_procedure",
 ]
 
 from importlib.metadata import version
 __version__ = version("pypomes_db")
 __version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
```

### Comparing `pypomes_db-0.5.2/src/pypomes_db/db_common.py` & `pypomes_db-0.5.3/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.5.2/src/pypomes_db/db_pomes.py` & `pypomes_db-0.5.3/src/pypomes_db/db_pomes.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,16 +102,16 @@
 
     curr_engine: str = _assert_engine(errors=errors,
                                       engine=engine)
     proceed: bool = True
     if curr_engine == "oracle":
         from . import oracle_pomes
         # noinspection PyProtectedMember
-        proceed = oracle_pomes._initialize(errors=errors,
-                                           logger=logger)
+        proceed = oracle_pomes.initialize(errors=errors,
+                                          logger=logger)
     if proceed:
         conn: Any = db_connect(errors=errors,
                                engine=curr_engine,
                                logger=logger)
         if conn:
             conn.close()
             result = True
@@ -435,14 +435,84 @@
                                                 insert_vals=insert_vals,
                                                 conn=conn,
                                                 logger=logger)
 
     return result
 
 
+def db_bulk_copy(errors: list[str] | None,
+                 sel_stmt: str,
+                 insert_stmt: str,
+                 target_engine: str,
+                 batch_size: int = None,
+                 where_vals: tuple = None,
+                 target_conn: Any = None,
+                 engine: str = None,
+                 conn: Any = None,
+                 logger: Logger = None) -> int:
+    """
+    Bulk copy data from a Oracle database to another database.
+
+    The destination database brand must be in the list of databases configured and supported by this package.
+
+    :param errors: incidental error messages
+    :param sel_stmt: SELECT command for the search
+    :param insert_stmt: the insert statement to use for bulk-inserting
+    :param target_engine: the destination database engine type
+    :param batch_size: number of tuples in the batch, or 0 or None for no limit
+    :param where_vals: the values to be associated with the search criteria
+    :param target_conn: the connection to the destination database
+    :param engine: the database engine to use (uses the default engine, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param logger: optional logger
+    :return: number of tuples effectively copied
+    """
+    # initialize the return variable
+    result: int | None = None
+
+    curr_engine: str = _assert_engine(errors, engine)
+    if curr_engine == "mysql":
+        pass
+    elif curr_engine == "oracle":
+        from . import oracle_pomes
+        result = oracle_pomes.db_bulk_copy(errors=errors,
+                                           sel_stmt=sel_stmt,
+                                           insert_stmt=insert_stmt,
+                                           batch_size=batch_size,
+                                           target_engine=target_engine,
+                                           where_vals=where_vals,
+                                           target_conn=target_conn,
+                                           conn=conn,
+                                           logger=logger)
+    elif curr_engine == "postgres":
+        from . import postgres_pomes
+        result = postgres_pomes.db_bulk_copy(errors=errors,
+                                             sel_stmt=sel_stmt,
+                                             insert_stmt=insert_stmt,
+                                             batch_size=batch_size,
+                                             target_engine=target_engine,
+                                             where_vals=where_vals,
+                                             target_conn=target_conn,
+                                             conn=conn,
+                                             logger=logger)
+    elif curr_engine == "sqlserver":
+        from . import sqlserver_pomes
+        result = sqlserver_pomes.db_bulk_copy(errors=errors,
+                                              sel_stmt=sel_stmt,
+                                              insert_stmt=insert_stmt,
+                                              batch_size=batch_size,
+                                              target_engine=target_engine,
+                                              where_vals=where_vals,
+                                              target_conn=target_conn,
+                                              conn=conn,
+                                              logger=logger)
+
+    return result
+
+
 def db_execute(errors: list[str] | None,
                exc_stmt: str,
                bind_vals: tuple = None,
                engine: str = None,
                conn: Any = None,
                logger: Logger = None) -> int:
     """
```

### Comparing `pypomes_db-0.5.2/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.5.3/src/pypomes_db/sqlserver_pomes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 from logging import Logger
-from oracledb import Connection, connect, init_oracle_client
+from pyodbc import connect, Connection, Row
+from typing import Any
 
 from .db_common import (
-    _DB_CONN_DATA,
     _assert_query_quota, _db_get_params, _db_log, _db_except_msg
 )
-
-# TODO: db_call_function, db_call_procedure
+from .db_pomes import db_bulk_insert as db_bulk_insert_to
 
 
 def db_connect(errors: list[str],
-               logger: Logger) -> Connection:
+               logger: Logger = None) -> Connection:
     """
     Obtain and return a connection to the database, or *None* if the connection could not be obtained.
 
     :param errors: incidental error messages
     :param logger: optional logger
     :return: the connection to the database
     """
-    # initialize the return variable
+    # initialize the return valiable
     result: Connection | None = None
 
-    # retrieve the connection parameters
-    name, user, pwd, host, port = _db_get_params("oracle")
+    # retrieve the connection parameters and build the connection string
+    name, user, pwd, host, port, driver = _db_get_params("sqlserver")
+    connection_kwargs: str = (
+        f"DRIVER={{{driver}}};SERVER={host},{port};"
+        f"DATABASE={name};UID={user};PWD={pwd};TrustServerCertificate=yes;"
+    )
 
     # obtain a connection to the database
     err_msg: str | None = None
     try:
-        result = connect(service_name=name,
-                         host=host,
-                         port=port,
-                         user=user,
-                         password=pwd)
+        result = connect(connection_kwargs)
         # make sure the connection is not in autocommit mode
         result.autocommit = False
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+                                 engine="sqlserver")
 
     # log the results
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
             query_stmt=f"Connecting to '{name}' at '{host}'")
 
@@ -74,42 +73,41 @@
     # initialize the return variable
     result: list[tuple] = []
 
     # make sure to have a connection
     curr_conn: Connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
+    err_msg: str | None = None
     if isinstance(require_max, int) and require_max > 0:
-        sel_stmt: str = f"{sel_stmt} FETCH NEXT {require_max} ROWS ONLY"
+        sel_stmt: str = sel_stmt.replace("SELECT", f"SELECT TOP {require_max}", 1)
 
-    err_msg: str | None = None
     try:
-        # obtain a cursor and perform the operation
+        # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
-            # execute the query
-            cursor.execute(statement=sel_stmt,
-                           parameters=where_vals)
+            cursor.execute(sel_stmt, where_vals)
             # obtain the number of tuples returned
             count: int = cursor.rowcount
 
             # has the query quota been satisfied ?
             if _assert_query_quota(errors=errors,
                                    query=sel_stmt,
                                    where_vals=where_vals,
                                    count=count,
                                    require_min=require_min,
                                    require_max=require_max):
                 # yes, retrieve the returned tuples
-                rows: list = cursor.fetchall()
+                rows: list[Row] = cursor.fetchall()
                 result = [tuple(row) for row in rows]
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
+        curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+                                 engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
@@ -125,17 +123,16 @@
                    insert_stmt: str,
                    insert_vals: list[tuple],
                    conn: Connection,
                    logger: Logger) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
-    The binding must be done by position. Thus, the *VALUES* clause in *insert_stmt*
-    must contain as many ':n' placeholders as there are elements in the tuples found in the
-    list provided in *insert_vals*, where 'n' is the 1-based position of the data in the tuple.
+    The *VALUES* clause in *insert_stmt* must contain as many '%s' placeholders
+    as there are elements in the tuples found in the list provided in *insert_vals*.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the number of inserted tuples, or None if an error occurred
@@ -147,25 +144,26 @@
     curr_conn: Connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
     err_msg: str | None = None
     try:
         # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
+            cursor.fast_executemany = True
             try:
-                cursor.executemany(statement=insert_stmt,
-                                   parameters=insert_vals)
+                cursor.executemany(insert_stmt, insert_vals)
                 result = len(insert_vals)
             except Exception:
                 conn.rollback()
                 raise
         curr_conn.commit()
     except Exception as e:
+        curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+                                 engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
@@ -173,14 +171,102 @@
             logger=logger,
             query_stmt=insert_stmt,
             bind_vals=insert_vals[0])
 
     return result
 
 
+def db_bulk_copy(errors: list[str],
+                 sel_stmt: str,
+                 insert_stmt: str,
+                 target_engine: str,
+                 batch_size: int,
+                 where_vals: tuple,
+                 target_conn: Any,
+                 conn: Connection,
+                 logger: Logger) -> int:
+    """
+    Bulk copy data from a Oracle database to another database.
+
+    The destination database brand must be in the list of databases configured and supported by this package.
+
+    :param errors: incidental error messages
+    :param sel_stmt: SELECT command for the search
+    :param insert_stmt: the insert statement to use for bulk-inserting
+    :param target_engine: the destination database engine type
+    :param batch_size: number of tuples in the batch, or 0 or None for no limit
+    :param where_vals: the values to be associated with the search criteria
+    :param target_conn: the connection to the destination database
+    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param logger: optional logger
+    :return: number of tuples effectively copied
+    """
+    # initialize the return variable
+    result: int | None = None
+
+    # make sure to have a connection
+    curr_conn: Connection = conn or db_connect(errors=errors,
+                                               logger=logger)
+
+    err_msg: str | None = None
+    try:
+        with curr_conn.cursor() as cursor:
+
+            # noinspection DuplicatedCode
+            # execute the query
+            cursor.execute(sel_stmt, where_vals)
+
+            # fetch rows in batches/all rows
+            result = 0
+            op_errors: list[str] = []
+            rows: list[Row]
+            if batch_size:
+                rows = cursor.fetchmany(batch_size)
+            else:
+                rows = cursor.fetchall()
+            while rows:
+                tuples: list[tuple] = [tuple(row) for row in rows]
+                result += db_bulk_insert_to(errors=op_errors,
+                                            insert_stmt=insert_stmt,
+                                            insert_vals=tuples,
+                                            engine=target_engine,
+                                            conn=target_conn,
+                                            logger=logger)
+                # errors ?
+                if op_errors:
+                    # yes, register them and abort the operation
+                    errors.extend(op_errors)
+                    break
+                if not batch_size:
+                    break
+                rows = cursor.fetchmany(batch_size)
+
+        # commit the source and target transactions
+        curr_conn.commit()
+        target_conn.commit()
+    except Exception as e:
+        err_msg = _db_except_msg(exception=e,
+                                 engine="postgres")
+        curr_conn.rollback()
+        target_conn.rollback()
+    finally:
+        # close the connection, if locally acquired
+        if not conn:
+            curr_conn.close()
+
+    # log the results
+    _db_log(errors=errors,
+            err_msg=err_msg,
+            logger=logger,
+            query_stmt=sel_stmt,
+            bind_vals=where_vals)
+
+    return result
+
+
 def db_execute(errors: list[str],
                exc_stmt: str,
                bind_vals: tuple,
                conn: Connection,
                logger: Logger) -> int:
     """
     Execute the command *exc_stmt* on the database.
@@ -207,22 +293,22 @@
     curr_conn: Connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
     err_msg: str | None = None
     try:
         # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
-            cursor.execute(statement=exc_stmt,
-                           parameters=bind_vals)
+            cursor.execute(exc_stmt, bind_vals)
             result = cursor.rowcount
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
+        curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+                                 engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
@@ -230,115 +316,61 @@
             logger=logger,
             query_stmt=exc_stmt,
             bind_vals=bind_vals)
 
     return result
 
 
-# TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
-# noinspection PyUnusedLocal
-def db_call_function(errors: list[str],
-                     func_name: str,
-                     func_vals: tuple,
-                     conn: Connection,
-                     logger: Logger) -> list[tuple]:
-    """
-    Execute the stored function *func_name* in the database, with the parameters given in *func_vals*.
-
-    :param errors: incidental error messages
-    :param func_name: name of the stored function
-    :param func_vals: parameters for the stored function
-    :param conn: optional connection to use (obtains a new one, if not specified)
-    :param logger: optional logger
-    :return: the data returned by the function
-    """
-    # initialize the return variable
-    result: list[tuple] = []
-
-    return result
-
-
-# TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
 def db_call_procedure(errors: list[str],
                       proc_name: str,
                       proc_vals: tuple,
                       conn: Connection,
-                      logger: Logger) -> list[tuple]:
+                      logger: Logger = None) -> list[tuple]:
     """
     Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
     :param errors: incidental error messages
     :param proc_name: name of the stored procedure
     :param proc_vals: parameters for the stored procedure
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
-    # noinspection DuplicatedCode
-    result: list[tuple] = []
+    result: list[tuple] | None = None
 
     # make sure to have a connection
     curr_conn: Connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
+    # build the command
+    proc_stmt: str | None = None
+
     # execute the stored procedure
     err_msg: str | None = None
     try:
-        # obtain a cursor and perform the operation
+        # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
-            cursor.callproc(name=proc_name,
-                            parameters=proc_vals)
-
+            proc_stmt = f"SET NOCOUNT ON; EXEC {proc_name} {','.join(('?',) * len(proc_vals))}"
+            cursor.execute(proc_stmt, proc_vals)
             # retrieve the returned tuples
-            result = list(cursor)
+            rows: list[Row] = cursor.fetchall()
+            result = [tuple(row) for row in rows]
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
+        curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+                                 engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
-            query_stmt=proc_name,
+            query_stmt=proc_stmt,
             bind_vals=proc_vals)
 
     return result
-
-__is_initialized: str | None = None
-
-def _initialize(errors: list[str],
-                logger: Logger) -> bool:
-    """
-    Setup the oracle engine to access the database throught the installed client software.
-
-    :param errors: incidental error messages
-    :param logger: optional logger
-    :return: False if an error happened, True otherwise
-    """
-    # initialize the return variable
-    result: bool = True
-
-    global __is_initialized
-    if not __is_initialized:
-        err_msg: str | None = None
-        client: str = _DB_CONN_DATA["oracle"]["client"]
-        try:
-            init_oracle_client(client)
-            __is_initialized = True
-        except Exception as e:
-            result = False
-            err_msg = _db_except_msg(exception=e,
-                                     engine="oracle")
-        # log the results
-        _db_log(errors=errors,
-                err_msg=err_msg,
-                logger=logger,
-                query_stmt="Initializing the client")
-
-    return result
```

### Comparing `pypomes_db-0.5.2/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.5.3/src/pypomes_db/postgres_pomes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from logging import Logger
 from psycopg2 import connect
 from psycopg2.extras import execute_values
 # noinspection PyProtectedMember
 from psycopg2._psycopg import connection
+from typing import Any
 
 from .db_common import (
     _assert_query_quota, _db_get_params, _db_log, _db_except_msg
 )
+from .db_pomes import db_bulk_insert as db_bulk_insert_to
 
 
 def db_connect(errors: list[str],
                logger: Logger = None) -> connection:
     """
     Obtain and return a connection to the database, or *None* if the connection could not be obtained.
 
@@ -98,14 +100,15 @@
                                    require_max=require_max):
                 # yes, retrieve the returned tuples
                 result = list(cursor)
 
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
+        curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
                                  engine="postgres")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
@@ -153,14 +156,15 @@
             execute_values(cur=cursor,
                            sql=insert_stmt,
                            argslist=insert_vals)
             result = len(insert_vals)
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
+        curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
                                  engine="postgres")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
@@ -169,14 +173,102 @@
             err_msg=err_msg,
             logger=logger,
             query_stmt=insert_stmt)
 
     return result
 
 
+def db_bulk_copy(errors: list[str],
+                 sel_stmt: str,
+                 insert_stmt: str,
+                 target_engine: str,
+                 batch_size: int,
+                 where_vals: tuple,
+                 target_conn: Any,
+                 conn: connection,
+                 logger: Logger) -> int:
+    """
+    Bulk copy data from a Oracle database to another database.
+
+    The destination database brand must be in the list of databases configured and supported by this package.
+
+    :param errors: incidental error messages
+    :param sel_stmt: SELECT command for the search
+    :param insert_stmt: the insert statement to use for bulk-inserting
+    :param target_engine: the destination database engine type
+    :param batch_size: number of tuples in the batch, or 0 or None for no limit
+    :param where_vals: the values to be associated with the search criteria
+    :param target_conn: the connection to the destination database
+    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param logger: optional logger
+    :return: number of tuples effectively copied
+    """
+    # initialize the return variable
+    result: int | None = None
+
+    # make sure to have a connection
+    curr_conn: connection = conn or db_connect(errors=errors,
+                                               logger=logger)
+
+    err_msg: str | None = None
+    try:
+        with curr_conn.cursor() as cursor:
+
+            # noinspection DuplicatedCode
+            # execute the query
+            cursor.execute(statement=sel_stmt,
+                           parameters=where_vals)
+
+            # fetch rows in batches/all rows
+            result = 0
+            op_errors: list[str] = []
+            rows: list[tuple]
+            if batch_size:
+                rows = cursor.fetchmany(batch_size)
+            else:
+                rows = cursor.fetchall()
+            while rows:
+                result += db_bulk_insert_to(errors=op_errors,
+                                            insert_stmt=insert_stmt,
+                                            insert_vals=rows,
+                                            engine=target_engine,
+                                            conn=target_conn,
+                                            logger=logger)
+                # errors ?
+                if op_errors:
+                    # yes, register them and abort the operation
+                    errors.extend(op_errors)
+                    break
+                if not batch_size:
+                    break
+                rows = cursor.fetchmany(batch_size)
+
+        # commit the source and target transactions
+        curr_conn.commit()
+        target_conn.commit()
+    except Exception as e:
+        err_msg = _db_except_msg(exception=e,
+                                 engine="postgres")
+        curr_conn.rollback()
+        target_conn.rollback()
+    finally:
+        # close the connection, if locally acquired
+        if not conn:
+            curr_conn.close()
+
+    # log the results
+    _db_log(errors=errors,
+            err_msg=err_msg,
+            logger=logger,
+            query_stmt=sel_stmt,
+            bind_vals=where_vals)
+
+    return result
+
+
 def db_execute(errors: list[str],
                exc_stmt: str,
                bind_vals: tuple,
                conn: connection,
                logger: Logger) -> int:
     """
     Execute the command *exc_stmt* on the database.
@@ -209,14 +301,15 @@
         with curr_conn.cursor() as cursor:
             cursor.execute(query=f"{exc_stmt};",
                            vars=bind_vals)
             result = cursor.rowcount
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
+        curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
                                  engine="postgres")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
@@ -263,14 +356,15 @@
             cursor.execute(query=proc_stmt,
                            argslist=proc_vals)
             # retrieve the returned tuples
             result = list(cursor)
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
+        curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
                                  engine="postgres")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
```

### Comparing `pypomes_db-0.5.2/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.5.3/src/pypomes_db/oracle_pomes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 from logging import Logger
-from pyodbc import connect, Connection, Row
+from oracledb import Connection, connect, init_oracle_client
+from typing import Any
 
 from .db_common import (
+    _DB_CONN_DATA,
     _assert_query_quota, _db_get_params, _db_log, _db_except_msg
 )
+from .db_pomes import db_bulk_insert as db_bulk_insert_to
+
+# TODO: db_call_function, db_call_procedure
 
 
 def db_connect(errors: list[str],
-               logger: Logger = None) -> Connection:
+               logger: Logger) -> Connection:
     """
     Obtain and return a connection to the database, or *None* if the connection could not be obtained.
 
     :param errors: incidental error messages
     :param logger: optional logger
     :return: the connection to the database
     """
-    # initialize the return valiable
+    # initialize the return variable
     result: Connection | None = None
 
-    # retrieve the connection parameters and build the connection string
-    name, user, pwd, host, port, driver = _db_get_params("sqlserver")
-    connection_kwargs: str = (
-        f"DRIVER={{{driver}}};SERVER={host},{port};"
-        f"DATABASE={name};UID={user};PWD={pwd};TrustServerCertificate=yes;"
-    )
+    # retrieve the connection parameters
+    name, user, pwd, host, port = _db_get_params("oracle")
 
     # obtain a connection to the database
     err_msg: str | None = None
     try:
-        result = connect(connection_kwargs)
+        result = connect(service_name=name,
+                         host=host,
+                         port=port,
+                         user=user,
+                         password=pwd)
         # make sure the connection is not in autocommit mode
         result.autocommit = False
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
-                                 engine="sqlserver")
+                                 engine="oracle")
 
     # log the results
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
             query_stmt=f"Connecting to '{name}' at '{host}'")
 
@@ -71,40 +76,43 @@
     # initialize the return variable
     result: list[tuple] = []
 
     # make sure to have a connection
     curr_conn: Connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
-    err_msg: str | None = None
     if isinstance(require_max, int) and require_max > 0:
-        sel_stmt: str = sel_stmt.replace("SELECT", f"SELECT TOP {require_max}", 1)
+        sel_stmt: str = f"{sel_stmt} FETCH NEXT {require_max} ROWS ONLY"
 
+    err_msg: str | None = None
     try:
-        # obtain a cursor and execute the operation
+        # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
-            cursor.execute(sel_stmt, where_vals)
+            # execute the query
+            cursor.execute(statement=sel_stmt,
+                           parameters=where_vals)
             # obtain the number of tuples returned
             count: int = cursor.rowcount
 
             # has the query quota been satisfied ?
             if _assert_query_quota(errors=errors,
                                    query=sel_stmt,
                                    where_vals=where_vals,
                                    count=count,
                                    require_min=require_min,
                                    require_max=require_max):
                 # yes, retrieve the returned tuples
-                rows: list[Row] = cursor.fetchall()
+                rows: list = cursor.fetchall()
                 result = [tuple(row) for row in rows]
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
+        curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="sqlserver")
+                                 engine="oracle")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
@@ -120,16 +128,17 @@
                    insert_stmt: str,
                    insert_vals: list[tuple],
                    conn: Connection,
                    logger: Logger) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
-    The *VALUES* clause in *insert_stmt* must contain as many '%s' placeholders
-    as there are elements in the tuples found in the list provided in *insert_vals*.
+    The binding must be done by position. Thus, the *VALUES* clause in *insert_stmt*
+    must contain as many ':n' placeholders as there are elements in the tuples found in the
+    list provided in *insert_vals*, where 'n' is the 1-based position of the data in the tuple.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the number of inserted tuples, or None if an error occurred
@@ -141,25 +150,22 @@
     curr_conn: Connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
     err_msg: str | None = None
     try:
         # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
-            cursor.fast_executemany = True
-            try:
-                cursor.executemany(insert_stmt, insert_vals)
-                result = len(insert_vals)
-            except Exception:
-                conn.rollback()
-                raise
+            cursor.executemany(statement=insert_stmt,
+                               parameters=insert_vals)
+            result = len(insert_vals)
         curr_conn.commit()
     except Exception as e:
+        curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="sqlserver")
+                                 engine="oracle")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
@@ -167,14 +173,102 @@
             logger=logger,
             query_stmt=insert_stmt,
             bind_vals=insert_vals[0])
 
     return result
 
 
+def db_bulk_copy(errors: list[str],
+                 sel_stmt: str,
+                 insert_stmt: str,
+                 target_engine: str,
+                 batch_size: int,
+                 where_vals: tuple,
+                 target_conn: Any,
+                 conn: Connection,
+                 logger: Logger) -> int:
+    """
+    Bulk copy data from a Oracle database to another database.
+
+    The destination database brand must be in the list of databases configured and supported by this package.
+
+    :param errors: incidental error messages
+    :param sel_stmt: SELECT command for the search
+    :param insert_stmt: the insert statement to use for bulk-inserting
+    :param target_engine: the destination database engine type
+    :param batch_size: number of tuples in the batch, or 0 or None for no limit
+    :param where_vals: the values to be associated with the search criteria
+    :param target_conn: the connection to the destination database
+    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param logger: optional logger
+    :return: number of tuples effectively copied
+    """
+    # initialize the return variable
+    result: int | None = None
+
+    # make sure to have a connection
+    curr_conn: Connection = conn or db_connect(errors=errors,
+                                               logger=logger)
+
+    err_msg: str | None = None
+    try:
+        with (curr_conn.cursor() as cursor):
+
+            # noinspection DuplicatedCode
+            # execute the query
+            cursor.execute(statement=sel_stmt,
+                           parameters=where_vals)
+
+            # fetch rows in batches/all rows
+            result = 0
+            op_errors: list[str] = []
+            rows: list[tuple]
+            if batch_size:
+                rows = cursor.fetchmany(batch_size)
+            else:
+                rows = cursor.fetchall()
+            while rows:
+                result += db_bulk_insert_to(errors=op_errors,
+                                            insert_stmt=insert_stmt,
+                                            insert_vals=rows,
+                                            engine=target_engine,
+                                            conn=target_conn,
+                                            logger=logger)
+                # errors ?
+                if op_errors:
+                    # yes, register them and abort the operation
+                    errors.extend(op_errors)
+                    break
+                if not batch_size:
+                    break
+                rows = cursor.fetchmany(batch_size)
+
+        # commit the source and target transactions
+        curr_conn.commit()
+        target_conn.commit()
+    except Exception as e:
+        err_msg = _db_except_msg(exception=e,
+                                 engine="oracle")
+        curr_conn.rollback()
+        target_conn.rollback()
+    finally:
+        # close the connection, if locally acquired
+        if not conn:
+            curr_conn.close()
+
+    # log the results
+    _db_log(errors=errors,
+            err_msg=err_msg,
+            logger=logger,
+            query_stmt=sel_stmt,
+            bind_vals=where_vals)
+
+    return result
+
+
 def db_execute(errors: list[str],
                exc_stmt: str,
                bind_vals: tuple,
                conn: Connection,
                logger: Logger) -> int:
     """
     Execute the command *exc_stmt* on the database.
@@ -201,21 +295,23 @@
     curr_conn: Connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
     err_msg: str | None = None
     try:
         # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
-            cursor.execute(exc_stmt, bind_vals)
+            cursor.execute(statement=exc_stmt,
+                           parameters=bind_vals)
             result = cursor.rowcount
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
+        curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="sqlserver")
+                                 engine="oracle")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
@@ -223,60 +319,116 @@
             logger=logger,
             query_stmt=exc_stmt,
             bind_vals=bind_vals)
 
     return result
 
 
+# TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
+# noinspection PyUnusedLocal
+def db_call_function(errors: list[str],
+                     func_name: str,
+                     func_vals: tuple,
+                     conn: Connection,
+                     logger: Logger) -> list[tuple]:
+    """
+    Execute the stored function *func_name* in the database, with the parameters given in *func_vals*.
+
+    :param errors: incidental error messages
+    :param func_name: name of the stored function
+    :param func_vals: parameters for the stored function
+    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param logger: optional logger
+    :return: the data returned by the function
+    """
+    # initialize the return variable
+    result: list[tuple] = []
+
+    return result
+
+
+# TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
 def db_call_procedure(errors: list[str],
                       proc_name: str,
                       proc_vals: tuple,
                       conn: Connection,
-                      logger: Logger = None) -> list[tuple]:
+                      logger: Logger) -> list[tuple]:
     """
     Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
     :param errors: incidental error messages
     :param proc_name: name of the stored procedure
     :param proc_vals: parameters for the stored procedure
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
-    result: list[tuple] | None = None
+    # noinspection DuplicatedCode
+    result: list[tuple] = []
 
     # make sure to have a connection
     curr_conn: Connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
-    # build the command
-    proc_stmt: str | None = None
-
     # execute the stored procedure
     err_msg: str | None = None
     try:
-        # obtain a cursor and execute the operation
+        # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
-            proc_stmt = f"SET NOCOUNT ON; EXEC {proc_name} {','.join(('?',) * len(proc_vals))}"
-            cursor.execute(proc_stmt, proc_vals)
+            cursor.callproc(name=proc_name,
+                            parameters=proc_vals)
+
             # retrieve the returned tuples
-            rows: list[Row] = cursor.fetchall()
-            result = [tuple(row) for row in rows]
+            result = list(cursor)
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
+        curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="sqlserver")
+                                 engine="oracle")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
-            query_stmt=proc_stmt,
+            query_stmt=proc_name,
             bind_vals=proc_vals)
 
     return result
+
+__is_initialized: str | None = None
+
+def initialize(errors: list[str],
+               logger: Logger) -> bool:
+    """
+    Setup the oracle engine to access the database throught the installed client software.
+
+    :param errors: incidental error messages
+    :param logger: optional logger
+    :return: False if an error happened, True otherwise
+    """
+    # initialize the return variable
+    result: bool = True
+
+    global __is_initialized
+    if not __is_initialized:
+        err_msg: str | None = None
+        client: str = _DB_CONN_DATA["oracle"]["client"]
+        try:
+            init_oracle_client(client)
+            __is_initialized = True
+        except Exception as e:
+            result = False
+            err_msg = _db_except_msg(exception=e,
+                                     engine="oracle")
+        # log the results
+        _db_log(errors=errors,
+                err_msg=err_msg,
+                logger=logger,
+                query_stmt="Initializing the client")
+
+    return result
```

### Comparing `pypomes_db-0.5.2/LICENSE` & `pypomes_db-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.5.2/pyproject.toml` & `pypomes_db-0.5.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.5.2"
+version = "0.5.3"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "pip>=24.0",
-#   "oracledb>=2.1.2",
+#   "mysql-connector-python>=8.4.0",
+#   "oracledb>=2.2.0",
 #   "psycopg2-binary>=2.9.9",
 #   "pyodbc>=5.1.0",
     "pypomes_core>=0.9.7",
     "setuptools>=68.0.0",
     "wheel>=0.42.0"
 ]
```

### Comparing `pypomes_db-0.5.2/PKG-INFO` & `pypomes_db-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.5.2
+Version: 0.5.3
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

