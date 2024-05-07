# Comparing `tmp/gpudb-7.2.0.5-cp39-cp39-win_amd64.whl.zip` & `tmp/gpudb-7.2.0.6-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 503739 bytes, number of entries: 38
--rw-rw-rw-  2.0 fat     2652 b- defN 24-Apr-16 02:47 gpudb/__init__.py
--rw-rw-rw-  2.0 fat  2296594 b- defN 24-Apr-16 03:13 gpudb/gpudb.py
--rw-rw-rw-  2.0 fat    15844 b- defN 24-Apr-16 03:13 gpudb/gpudb_dataframe.py
+Zip file size: 507077 bytes, number of entries: 39
+-rw-rw-rw-  2.0 fat     2838 b- defN 24-Apr-23 04:58 gpudb/__init__.py
+-rw-rw-rw-  2.0 fat  2300706 b- defN 24-Apr-23 04:58 gpudb/gpudb.py
+-rw-rw-rw-  2.0 fat    15822 b- defN 24-Apr-23 04:58 gpudb/gpudb_dataframe.py
 -rw-rw-rw-  2.0 fat    12599 b- defN 24-Apr-16 03:13 gpudb/gpudb_file_handler.py
 -rw-rw-rw-  2.0 fat   181479 b- defN 24-Apr-16 02:47 gpudb/gpudb_multihead_io.py
--rw-rw-rw-  2.0 fat     6280 b- defN 24-Apr-16 03:13 gpudb/gpudb_sql_iterator.py
+-rw-rw-rw-  2.0 fat     8541 b- defN 24-Apr-23 04:58 gpudb/gpudb_sql_context.py
+-rw-rw-rw-  2.0 fat     5136 b- defN 24-Apr-23 04:58 gpudb/gpudb_sql_iterator.py
 -rw-rw-rw-  2.0 fat    76640 b- defN 24-Apr-16 02:47 gpudb/gpudb_table_monitor.py
 -rw-rw-rw-  2.0 fat    82432 b- defN 24-Apr-16 03:14 gpudb/protocol.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-16 02:47 gpudb/packages/__init__.py
 -rw-rw-rw-  2.0 fat    33494 b- defN 24-Apr-16 02:47 gpudb/packages/enum34.py
 -rw-rw-rw-  2.0 fat    40175 b- defN 24-Apr-16 02:47 gpudb/packages/kinetica_tabulate.py
 -rw-rw-rw-  2.0 fat     4413 b- defN 24-Apr-16 02:47 gpudb/packages/ordereddict.py
 -rw-rw-rw-  2.0 fat    14620 b- defN 24-Apr-16 02:47 gpudb/packages/pymmh3.py
@@ -28,13 +29,13 @@
 -rw-rw-rw-  2.0 fat    15680 b- defN 24-Apr-16 02:47 gpudb/packages/avro/avro_py3/datafile.py
 -rw-rw-rw-  2.0 fat    34384 b- defN 24-Apr-16 02:47 gpudb/packages/avro/avro_py3/io.py
 -rw-rw-rw-  2.0 fat    23129 b- defN 24-Apr-16 02:47 gpudb/packages/avro/avro_py3/ipc.py
 -rw-rw-rw-  2.0 fat    12318 b- defN 24-Apr-16 02:47 gpudb/packages/avro/avro_py3/protocol.py
 -rw-rw-rw-  2.0 fat    36588 b- defN 24-Apr-16 03:13 gpudb/packages/avro/avro_py3/schema.py
 -rw-rw-rw-  2.0 fat     5761 b- defN 24-Apr-16 02:47 gpudb/packages/avro/avro_py3/tool.py
 -rw-rw-rw-  2.0 fat     8263 b- defN 24-Apr-16 02:47 gpudb/packages/avro/avro_py3/txipc.py
--rw-rw-rw-  2.0 fat     1104 b- defN 24-Apr-16 03:14 gpudb-7.2.0.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      371 b- defN 24-Apr-16 03:14 gpudb-7.2.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-16 03:14 gpudb-7.2.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-16 03:14 gpudb-7.2.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     3384 b- defN 24-Apr-16 03:14 gpudb-7.2.0.5.dist-info/RECORD
-38 files, 3023738 bytes uncompressed, 498297 bytes compressed:  83.5%
+-rw-rw-rw-  2.0 fat     1104 b- defN 24-Apr-23 05:00 gpudb-7.2.0.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      371 b- defN 24-Apr-23 05:00 gpudb-7.2.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-23 05:00 gpudb-7.2.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-23 05:00 gpudb-7.2.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     3467 b- defN 24-Apr-23 05:00 gpudb-7.2.0.6.dist-info/RECORD
+39 files, 3035494 bytes uncompressed, 501507 bytes compressed:  83.5%
```

## zipnote {}

```diff
@@ -9,14 +9,17 @@
 
 Filename: gpudb/gpudb_file_handler.py
 Comment: 
 
 Filename: gpudb/gpudb_multihead_io.py
 Comment: 
 
+Filename: gpudb/gpudb_sql_context.py
+Comment: 
+
 Filename: gpudb/gpudb_sql_iterator.py
 Comment: 
 
 Filename: gpudb/gpudb_table_monitor.py
 Comment: 
 
 Filename: gpudb/protocol.cp39-win_amd64.pyd
@@ -93,23 +96,23 @@
 
 Filename: gpudb/packages/avro/avro_py3/tool.py
 Comment: 
 
 Filename: gpudb/packages/avro/avro_py3/txipc.py
 Comment: 
 
-Filename: gpudb-7.2.0.5.dist-info/LICENSE
+Filename: gpudb-7.2.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: gpudb-7.2.0.5.dist-info/METADATA
+Filename: gpudb-7.2.0.6.dist-info/METADATA
 Comment: 
 
-Filename: gpudb-7.2.0.5.dist-info/WHEEL
+Filename: gpudb-7.2.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: gpudb-7.2.0.5.dist-info/top_level.txt
+Filename: gpudb-7.2.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: gpudb-7.2.0.5.dist-info/RECORD
+Filename: gpudb-7.2.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gpudb/__init__.py

```diff
@@ -35,14 +35,16 @@
     from gpudb.gpudb_multihead_io import GPUdbWorkerList, GPUdbIngestor, InsertionException, RecordRetriever
 
     from gpudb.gpudb_table_monitor import GPUdbTableMonitor
     from gpudb.gpudb_file_handler import GPUdbFileHandler, OpMode, MultipartOperation
 
     from gpudb.gpudb import collections
     from gpudb.gpudb_sql_iterator import GPUdbSqlIterator
+    from gpudb.gpudb_sql_context import GPUdbSamplesClause, GPUdbTableClause, GPUdbSqlContext
+
 else:
     from gpudb import GPUdb
     from gpudb import GPUdbException
     from gpudb import GPUdbConnectionException
     from gpudb import GPUdbDecodingException
     from gpudb import GPUdbExitException
     from gpudb import GPUdbFailoverDisabledException
@@ -62,7 +64,8 @@
 
     from gpudb_multihead_io import GPUdbWorkerList, GPUdbIngestor, InsertionException, RecordRetriever
 
     from gpudb_table_monitor import GPUdbTableMonitor
 
     from gpudb import collections
     from gpudb_sql_iterator import GPUdbSqlIterator
+    from gpudb_sql_context import GPUdbSamplesClause, GPUdbTableClause, GPUdbSqlContext
```

## gpudb/gpudb.py

```diff
@@ -56,15 +56,15 @@
 IS_PYTHON_3 = (sys.version_info[0] >= 3) # checking the major component
 IS_PYTHON_27_OR_ABOVE = sys.version_info >= (2, 7)
 
 if IS_PYTHON_3:
     long = int
     basestring = str
     class unicode:
-        """Ensure python 3 doesn't complain about use of unicode."""
+        """Ensure Python 3 doesn't complain about use of Unicode."""
         pass
     from collections.abc import Iterator
 else:
     from collections import Iterator
 # end if
 
 
@@ -4971,15 +4971,15 @@
 
     END_OF_SET = -9999
     """(int) Used for indicating that all of the records (till the end of the
     set are desired)--generally used for /get/records/\* functions.
     """
 
     # The version of this API
-    api_version = "7.2.0.5"
+    api_version = "7.2.0.6"
 
     # -------------------------  GPUdb Methods --------------------------------
 
     def __init__( self, host = None, options = None, *args, **kwargs ):
         """
         Construct a new GPUdb client instance.  This object communicates to
         the database server at the given address.  This class implements
@@ -5894,15 +5894,15 @@
     # end __parse_urls_once
 
 
     def __randomize_clusters( self ):
         """Randomly shuffles the list of high availability URL indices so that HA
         failover happens at a random fashion.  One caveat is when a primary host
         is given by the user; in that case, we need to keep the primary host's
-        index as the first one in the list so that upon failover, when we cricle
+        index as the first one in the list so that upon failover, when we circle
         back, we always pick the first/primary host up again.
 
         Also, with the new ha failover order, it's not always random.  We might
         want to keep it in the order found.
         """
         # Re-create the list of HA URL indices (automatically in an
         # monotonically increasing order)
@@ -7528,14 +7528,22 @@
 
 
 
 
     # ------------------------------------------------------------------------
     #                 Endpoint Submission Related Methods
     # ------------------------------------------------------------------------
+    @classmethod
+    def _check_error(cls, response: dict) -> None:
+        status = response['status_info']['status']
+        if (status != 'OK'):
+            message = response['status_info']['message']
+            raise GPUdbException('[%s]: %s' % (status, message))
+
+
     def __submit_request_raw( self, url = None, endpoint = None,
                               request_body = None,
                               # enable_compression = False,
                               timeout = None,
                               get_req_cext = False,
                               get_rsp_cext = False,
                               request_schema  = None,
@@ -9612,15 +9620,15 @@
 
         return _dict
     # end sanitize_dicts
 
 
     def encode_datum(self, SCHEMA, datum, encoding = None):
         """
-        Returns an avro binary or JSON encoded dataum dict using its schema.
+        Returns an Avro binary or JSON encoded datum dict using its schema.
 
         Parameters:
             SCHEMA (str or avro.Schema)
                 A parsed schema object from avro.schema.parse() or a
                 string containing the schema.
 
             datum (dict)
@@ -9642,15 +9650,15 @@
         elif encoding == C._ENCODING_JSON:
             return json.dumps( _Util.convert_dict_bytes_to_str( datum ) )
     # end encode_datum
 
 
     def encode_datum_cext(self, SCHEMA, datum, encoding = None):
         """
-        Returns an avro binary or JSON encoded dataum dict using its schema.
+        Returns an avro binary or JSON encoded datum dict using its schema.
 
         Parameters:
             SCHEMA (str or avro.Schema)
                 A parsed schema object from avro.schema.parse() or a
                 string containing the schema.
 
             datum (dict)
@@ -9886,16 +9894,15 @@
 
 
     def get_records_json(self, table_name, column_names = None, offset = 0, limit = -9999, expression = None, orderby_columns = None, having_clause = None):
         """ This method is used to retrieve records from a Kinetica table in the form of
         a JSON array (stringified). The only mandatory parameter is the 'tableName'.
         The rest are all optional with suitable defaults wherever applicable.
 
-
-        Args:
+        Parameters:
             table_name (str): Name of the table
             column_names (list): the columns names to retrieve
             offset (int): the offset to start from - default 0
             limit (int): the maximum number of records - default GPUdb.END_OF_SET
             expression (str): the filter expression
             orderby_columns (list): the list of columns to order by
             having_clause (str): the having clause
@@ -10286,15 +10293,15 @@
               sql: str,
               sql_params: list = [],
               batch_size: int = 5000,
               sql_opts: dict = {},
               show_progress: bool = False):
         """Runs the given query and converts the result to a Pandas Data Frame.
 
-        Args:
+        Parameters:
             sql (str)
                 The SQL query to run
 
             sql_params (list)
                 The SQL parameters that will be substituted for tokens (e.g. $1 $2)
 
             batch_size (int)
@@ -10384,15 +10391,15 @@
 
             row = sql_iterator.__next__()
             return row
     # end query_one
 
 
     def execute(self, sql, sql_params = [], sql_opts = {}):
-        """Execute a SQL query and return the rowcount.
+        """Execute a SQL query and return the row count.
 
         Parameters:
             sql (str)
                 The SQL to execute
 
             sql_params(list of native types)
                 The SQL parameters that will be substituted for tokens (e.g. $1 $2)
@@ -10402,22 +10409,120 @@
                 :meth:`GPUdb.execute_sql`. Defaults to None.
 
         Returns:
             Number of records affected
         """
         from . import gpudb_sql_iterator
 
-        gpudb_sql_iterator.GPUdbSqlIterator._set_sql_params(sql_opts, sql_params)
+        GPUdb._set_sql_params(sql_opts, sql_params)
         response = self.execute_sql(statement=sql, options=sql_opts)
-        gpudb_sql_iterator.GPUdbSqlIterator._check_error(response)
+        GPUdb._check_error(response)
         count_affected = response['count_affected']
         return count_affected
     # end execute
 
 
+    @classmethod
+    def _set_sql_params(cls, sql_opts: dict, sql_params: list) -> None:
+        """Convert SQL parameters to JSON and set as an option for execute_sql_and_decode()
+
+        Parameters:
+            sql_opts (dict)
+                The parameter list that will be appended to.
+
+            sql_params (list of native types)
+                The SQL parameters that will be substituted for tokens (e.g. $1 $2)
+        """
+        if (len(sql_params) == 0):
+            return
+        
+        for idx, item in enumerate(sql_params):
+            if (isinstance(item, list)):
+                # assume that list type is vector
+                sql_params[idx] = str(item)
+
+        json_params = json.dumps(sql_params)
+        sql_opts['query_parameters'] = json.dumps(sql_params)
+
+
+    @staticmethod
+    def get_connection(
+            enable_ssl_cert_verification = False, 
+            enable_auto_discovery = False,
+            enable_failover = False,
+            logging_level = 'INFO') -> "GPUdb":
+        """ Get a connection to Kinetica getting connection and authentication
+        information from environment variables.
+
+        This method is useful particularly for Jupyter notebooks, which won't
+        need authentication credentials embedded within them.  This, in turn,
+        helps to prevent commit of credentials to the notebook version control.
+        In addition, some features including auto-discovery and SSL certificate
+        verification are disabled by default to simplify connections for simple
+        use cases.
+
+        The following environment variables are required:
+        - `KINETICA_URL`: the url of the Kinetica server
+        - `KINETICA_USER`: the username to connect with
+        - `KINETICA_PASSWD`: the password to connect with
+
+        Parameters:
+            enable_ssl_cert_verification (bool):
+                Enable SSL certificate verification.
+    
+            enable_auto_discovery (bool):
+                Enable auto-discovery of the initial cluster nodes, as well as
+                any attached failover clusters.  This allows for both multi-head
+                ingestion & key lookup, as well as cluster failover.
+    
+            enable_failover (bool):
+                Enable failover to another cluster.
+    
+            logging_level (str):
+                Logging level for the connection. (INFO by default)
+    
+        Returns (GPUdb):
+            An active connection to Kinetica.
+        """
+
+        ENV_URL = 'KINETICA_URL'
+        ENV_USER = 'KINETICA_USER'
+        ENV_PASS = 'KINETICA_PASSWD'
+        ENV_NOT_FOUND_ERROR = 'Environment variable <{}> needs to be set when connecting with get_connection()'
+
+        if ENV_URL in os.environ:
+            url = os.environ[ENV_URL]
+        else:
+            raise GPUdbException(ENV_NOT_FOUND_ERROR.format( ENV_URL ))
+
+        if ENV_USER in os.environ:
+            user = os.environ[ENV_USER]
+        else:
+            raise GPUdbException(ENV_NOT_FOUND_ERROR.format( ENV_USER ))
+
+        if ENV_PASS in os.environ:
+            passwd = os.environ[ENV_PASS]
+        else:
+            raise GPUdbException(ENV_NOT_FOUND_ERROR.format( ENV_PASS ))
+
+        options = GPUdb.Options()
+        options.username = user
+        options.password = passwd
+        options.skip_ssl_cert_verification = not enable_ssl_cert_verification
+        options.disable_auto_discovery = not enable_auto_discovery
+        options.disable_failover = not enable_failover
+        options.logging_level = logging_level
+        kdbc = GPUdb(host = url, options = options)
+
+        kdbc.__log_info("Connected to Kinetica! (host={} api={} server={})".format(kdbc.get_url(), kdbc.api_version, str(kdbc.server_version)))
+
+        return kdbc
+    # end get_connection
+
+
     # ------------- END convenience functions ------------------------------------
 
 
 
 
     # -----------------------------------------------------------------------
     # Begin autogenerated functions
@@ -38200,15 +38305,15 @@
 # ---------------------------------------------------------------------------
 # GPUdbTable - Class to Handle GPUdb Tables
 # ---------------------------------------------------------------------------
 class GPUdbTable( object ):
 
     @staticmethod
     def random_name():
-        """Returns a randomly generated uuid-based name.  Use underscores
+        """Returns a randomly generated UUID-based name.  Use underscores
         instead of hyphens.
         """
         return str( uuid.uuid4() ).replace( '-', '_' )
     # end random_name
 
 
     @staticmethod
@@ -39142,15 +39247,15 @@
 
     @staticmethod
     def convert_special_type_values_in_insert_records(record_type : GPUdbRecordType,
                                                       records: Union[Union[ list, dict], List[Record]]
                                                       ):
         """Convert any special value type (array, json, vector etc.) suitably
 
-        Args:
+        Parameters:
             record_type (GPUdbRecordType): the record type for these 'records'
             records (Union[Union[ list, dict], List[Record]]): A single record value (list or dict)
 
         Returns:
             object: the converted value
         """
         if isinstance(records, list):
@@ -39180,15 +39285,15 @@
 
     @staticmethod
     def convert_special_type_values_in_get_records(record_type : GPUdbRecordType,
                                                    records: Union[Union[ list, dict], List[Record]]
                                                    ):
         """Convert any special value type (array, json, vector etc.) suitably
 
-        Args:
+        Parameters:
             record_type (GPUdbRecordType): the record type for these 'records'
             records (Union[Union[ list, dict], List[Record]]): A single record value (list or dict)
 
         Returns:
             object: the converted value
         """        
         if not (isinstance(records, list) and all(isinstance(e, Record) for e in records)) and \
@@ -39752,15 +39857,15 @@
         end value (offset + limit) parameters (inclusive). If there are
         num_points values in the table then each of the indices between 0 and
         num_points-1 retrieves a unique value.
 
         Note that when using the pagination feature, if the table (or the
         underlying table in case of a view) is updated (records are inserted,
         deleted or modified) the records or values retrieved may differ between
-        calls (discontiguous or overlap) based on the type of the update.
+        calls (noncontiguous or overlap) based on the type of the update.
 
         The response is returned as a dynamic schema. For details see: `dynamic
         schemas documentation <../../../../api/#dynamic-schemas>`_.
 
         Parameters:
 
             column_names (list of str)
@@ -40172,15 +40277,15 @@
                 batch_size: int = 5000,
                 **kwargs):
         """ Load a Data Frame into a table; optionally dropping any existing table,
         creating it if it doesn't exist, and loading data into it; and then returning a
         GPUdbTable reference to the table.
 
 
-        Args:
+        Parameters:
             df (pd.DataFrame)
                 The Pandas Data Frame to load into a table
 
             db (GPUdb)
                 GPUdb instance
 
             table_name (str)
```

## gpudb/gpudb_dataframe.py

```diff
@@ -246,22 +246,22 @@
             GPUdbTable: a GPUdbTable instance created from the Data Frame passed in 
         """
         
         if(df.empty):
             raise GPUdbException(f"Dataframe cannot be empty.")
 
         has_table_resp = db.has_table(table_name)
-        GPUdbSqlIterator._check_error(has_table_resp)
+        GPUdb._check_error(has_table_resp)
         if (not create_table and not has_table_resp["table_exists"]):
             raise GPUdbException(f"{table_name}) Table does not exist and create_table=false")
 
         if (clear_table):
             cls._LOG.debug(f"Clearing table: {table_name}")
             clear_resp = db.clear_table(table_name=table_name, options={'no_error_if_not_exists': 'true'})
-            GPUdbSqlIterator._check_error(clear_resp)
+            GPUdb._check_error(clear_resp)
 
         cls._LOG.debug(f"Creating table: {table_name}")
         col_types = cls._table_types_from_df(df, column_types)
         gpudb_table = GPUdbTable(_type=col_types, name=table_name, db=db, **kwargs)
 
         if (load_data):
             cls.df_insert_into_table(df=df,
```

## gpudb/gpudb_sql_iterator.py

```diff
@@ -54,50 +54,18 @@
         self.records = None
         self.offset = 0
         self.total_count = None
         self.retrieved_count = 0
         self.paging_tables = []
 
         paging_table_name = GPUdbTable.random_name()
-        self._set_sql_params(sql_opts, sql_params)
+        GPUdb._set_sql_params(sql_opts, sql_params)
         self.sql_opts["paging_table"] = paging_table_name
 
 
-    @classmethod
-    def _set_sql_params(cls, sql_opts: dict, sql_params: list) -> None:
-        """Convert SQL parameters to JSON and set as an option for execute_sql_and_decode()
-
-        Parameters:
-            sql_opts (dict)
-                The parameter list that will be appended to.
-
-            sql_params (list of native types)
-                The SQL parameters that will be substituted for tokens (e.g. $1 $2)
-        """
-        if (len(sql_params) == 0):
-            return
-        
-        for idx, item in enumerate(sql_params):
-            if (isinstance(item, list)):
-                # assume that list type is vector
-                sql_params[idx] = str(item)
-
-        json_params = json.dumps(sql_params)
-        LOG.debug(f"json_params: {json_params}")
-        sql_opts['query_parameters'] = json.dumps(sql_params)
-
-
-    @classmethod
-    def _check_error(cls, response: dict) -> None:
-        status = response['status_info']['status']
-        if (status != 'OK'):
-            message = response['status_info']['message']
-            raise GPUdbException('[%s]: %s' % (status, message))
-
-
     def open(self):
         # optional call
         self._check_fetch()
 
     def close(self):
         for table_name in self.paging_tables:
             self.db.clear_table(table_name, options={'no_error_if_not_exists': 'true'})
@@ -157,15 +125,15 @@
             statement=self.sql,
             offset=self.offset,
             limit=limit,
             force_primitive_return_types=False,
             get_column_major=False,
             options=self.sql_opts)
 
-        self._check_error(response)
+        GPUdb._check_error(response)
         self.records = response['records']
 
         if (self.total_count is None):
             self.total_count = response['total_number_of_records']
 
         # self._log.info(f"response: {response}")
         if (self.paging_tables is None):
@@ -187,8 +155,8 @@
         if (self.type_map is None):
             col_defs = self.records[0].type.values()
             col_names = list(col.name for col in col_defs)
             col_types = list(col.data_type for col in col_defs)
             self.type_map = {name: type for (name, type) in zip(col_names, col_types)}
             self._log.debug(f"Type map: {self.type_map}")
 
-# end class KineticaSqlIterator
+# end class GPUdbSqlIterator
```

## Comparing `gpudb-7.2.0.5.dist-info/LICENSE` & `gpudb-7.2.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gpudb-7.2.0.5.dist-info/RECORD` & `gpudb-7.2.0.6.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-gpudb/__init__.py,sha256=Lc3Sj9jzqHMELVoYsJEsFkBDHr4A_F-YhcnmFlc1mGA,2652
-gpudb/gpudb.py,sha256=_OGPpJFox4Shq2JyK-X8AipAxz6d5oIDQ5i5EkjM8aU,2296594
-gpudb/gpudb_dataframe.py,sha256=PzxAEkGjWPTdOtZYaRJBq3TKxc5evaaNnpuLU06tmR8,15844
+gpudb/__init__.py,sha256=tsyXJerWRlMdt0ovZNXh5YGlfRM1wQ4UKVZdmKB5weY,2838
+gpudb/gpudb.py,sha256=qMx4i5U7zVgn-FKw8gWj4Y8TdWKiUD9O27kevrD7rNM,2300706
+gpudb/gpudb_dataframe.py,sha256=AIBwW12ZeSzNWPoGOJmJlKAveFIHv5W7PX_Gadkd0b4,15822
 gpudb/gpudb_file_handler.py,sha256=P2oDXMI4P-sqlwsUxshP7U4yk8edVnR_OerTr9HVPxQ,12599
 gpudb/gpudb_multihead_io.py,sha256=bIpbEaDgmWn6KJFZFWD4x-i97l9ZjwZ_saXib2sTimw,181479
-gpudb/gpudb_sql_iterator.py,sha256=bk_tKbTu7MrZndmcbGWNOW4VTitCPKNgVEchFsKOMnQ,6280
+gpudb/gpudb_sql_context.py,sha256=66OCIzrK3cIzl7LOrJmAUsg7LqTtr_spuH0PDrZZna0,8541
+gpudb/gpudb_sql_iterator.py,sha256=OgKcbMKP913VYmFRy22fDl7uU-rKWWD-W1kTeMjzNsE,5136
 gpudb/gpudb_table_monitor.py,sha256=YKORXw3glZsJCTD2SDBsA-fsHofPrPsKTQobuppY2eM,76640
 gpudb/protocol.cp39-win_amd64.pyd,sha256=INAmDOABPN6gh6Ck2JHj6wNiLGKDVEO8T8THyE6gYDE,82432
 gpudb/packages/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gpudb/packages/enum34.py,sha256=M1JeCFaL3T7ZWVlu_J4OeNuil8SGJ6cNgp9JzEwn8zE,33494
 gpudb/packages/kinetica_tabulate.py,sha256=RTcY5vDKdGwc4WvUyxXLX5dWDoUt2Gt50lVqUxfPf_0,40175
 gpudb/packages/ordereddict.py,sha256=EuzwpZHmxsQnWP2Xa2U5ApZU19YOijgQJCbYx20AvJ4,4413
 gpudb/packages/pymmh3.py,sha256=PkbkLgOTeERrTQZZ9Yrr1JwJHvA9vFbYMS3Tt553Uuc,14620
@@ -27,12 +28,12 @@
 gpudb/packages/avro/avro_py3/datafile.py,sha256=Vmm3imNQDAHFRJ61la0SqVOqAYoGYJRh10CL-68cFdo,15680
 gpudb/packages/avro/avro_py3/io.py,sha256=1TRwjjuhwocrbI6k99hdINJLsmo-RnQBT5pba7uCstw,34384
 gpudb/packages/avro/avro_py3/ipc.py,sha256=UJbNqAw0tGihLLhnSaoRHHy0EjQ55DlrJQEnbHJgwaY,23129
 gpudb/packages/avro/avro_py3/protocol.py,sha256=7oxTKOY7XWqQW59mWHlnamDCvqhoHWnbioMdXvdB3qg,12318
 gpudb/packages/avro/avro_py3/schema.py,sha256=vRbyhng1j09CdZyFWxyHgZfxZlveT245msrfbUYmTe8,36588
 gpudb/packages/avro/avro_py3/tool.py,sha256=7uYBlkBpk4YZIUUldGI_gNWCosBO0cHGbrzUMOszX7I,5761
 gpudb/packages/avro/avro_py3/txipc.py,sha256=MVmWuenBqRcxELmXkh3L15-pwiuUdCNo2bD9wDO5q1A,8263
-gpudb-7.2.0.5.dist-info/LICENSE,sha256=mO8T_HZHSioc8ubjlLCgRqkSEqu6jK7tXsBhPGxk6OI,1104
-gpudb-7.2.0.5.dist-info/METADATA,sha256=G06lEMsVFwH_m2WPddqj5YG3zocfFM6uFnHB2zq9RLw,371
-gpudb-7.2.0.5.dist-info/WHEEL,sha256=jr7ubY0Lkz_yXH9FfFe9PTtLhGOsf62dZkNvTYrJINE,100
-gpudb-7.2.0.5.dist-info/top_level.txt,sha256=WXblkeM06dfvsdiZ156hrZR9H6m3fEQ6L0rUV7YqDAM,6
-gpudb-7.2.0.5.dist-info/RECORD,,
+gpudb-7.2.0.6.dist-info/LICENSE,sha256=mO8T_HZHSioc8ubjlLCgRqkSEqu6jK7tXsBhPGxk6OI,1104
+gpudb-7.2.0.6.dist-info/METADATA,sha256=s1Ml6hhE2-6a91NLukGYpSopSVHW1jicy_LfiXp4fXI,371
+gpudb-7.2.0.6.dist-info/WHEEL,sha256=jr7ubY0Lkz_yXH9FfFe9PTtLhGOsf62dZkNvTYrJINE,100
+gpudb-7.2.0.6.dist-info/top_level.txt,sha256=WXblkeM06dfvsdiZ156hrZR9H6m3fEQ6L0rUV7YqDAM,6
+gpudb-7.2.0.6.dist-info/RECORD,,
```

