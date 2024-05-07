# Comparing `tmp/suql-1.1.7a1.tar.gz` & `tmp/suql-1.1.7a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suql-1.1.7a1.tar", last modified: Thu May  2 17:44:39 2024, max compression
+gzip compressed data, was "suql-1.1.7a2.tar", last modified: Tue May  7 05:12:34 2024, max compression
```

## Comparing `suql-1.1.7a1.tar` & `suql-1.1.7a2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwx------   0 oval      (1000) users      (100)        0 2024-05-02 17:44:39.552665 suql-1.1.7a1/
--rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.1.7a1/LICENSE
--rw-------   0 oval      (1000) users      (100)     5021 2024-05-02 17:44:39.552665 suql-1.1.7a1/PKG-INFO
--rw-------   0 oval      (1000) users      (100)     4415 2024-04-30 04:28:53.000000 suql-1.1.7a1/README.md
--rw-------   0 oval      (1000) users      (100)       38 2024-05-02 17:44:39.552665 suql-1.1.7a1/setup.cfg
--rw-------   0 oval      (1000) users      (100)     1541 2024-05-02 17:42:54.000000 suql-1.1.7a1/setup.py
-drwx------   0 oval      (1000) users      (100)        0 2024-05-02 17:44:39.552665 suql-1.1.7a1/src/
-drwx------   0 oval      (1000) users      (100)        0 2024-05-02 17:44:39.552665 suql-1.1.7a1/src/suql/
--rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.1.7a1/src/suql/__init__.py
--rw-------   0 oval      (1000) users      (100)    17393 2024-04-25 17:52:02.000000 suql-1.1.7a1/src/suql/agent.py
--rw-------   0 oval      (1000) users      (100)    20797 2024-05-02 02:56:05.000000 suql-1.1.7a1/src/suql/faiss_embedding.py
--rw-------   0 oval      (1000) users      (100)     8792 2024-04-17 07:27:02.000000 suql-1.1.7a1/src/suql/free_text_fcns_server.py
--rw-------   0 oval      (1000) users      (100)     3563 2024-04-25 17:52:02.000000 suql-1.1.7a1/src/suql/postgresql_connection.py
--rw-------   0 oval      (1000) users      (100)     9612 2024-04-17 08:33:05.000000 suql-1.1.7a1/src/suql/prompt_continuation.py
-drwx------   0 oval      (1000) users      (100)        0 2024-05-02 17:44:39.552665 suql-1.1.7a1/src/suql/prompts/
--rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:18.000000 suql-1.1.7a1/src/suql/prompts/__init__.py
--rw-------   0 oval      (1000) users      (100)      169 2024-04-03 06:02:28.000000 suql-1.1.7a1/src/suql/prompts/answer_qa.prompt
--rw-------   0 oval      (1000) users      (100)      451 2024-04-03 06:02:28.000000 suql-1.1.7a1/src/suql/prompts/field_classification.prompt
--rw-------   0 oval      (1000) users      (100)     2945 2024-04-03 06:02:28.000000 suql-1.1.7a1/src/suql/prompts/if_db_classification.prompt
--rw-------   0 oval      (1000) users      (100)     1305 2024-04-03 06:02:28.000000 suql-1.1.7a1/src/suql/prompts/opening_hours.prompt
--rw-------   0 oval      (1000) users      (100)     5574 2024-04-03 06:02:28.000000 suql-1.1.7a1/src/suql/prompts/parser_suql.prompt
--rw-------   0 oval      (1000) users      (100)      227 2024-04-03 06:02:28.000000 suql-1.1.7a1/src/suql/prompts/verification.prompt
--rw-------   0 oval      (1000) users      (100)     2983 2024-04-03 06:02:28.000000 suql-1.1.7a1/src/suql/prompts/yelp_response_SQL.prompt
--rw-------   0 oval      (1000) users      (100)     1454 2024-04-03 06:02:28.000000 suql-1.1.7a1/src/suql/prompts/yelp_response_no_results.prompt
-drwx------   0 oval      (1000) users      (100)        0 2024-05-02 17:44:39.552665 suql-1.1.7a1/src/suql/sql_free_text_support/
--rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:11.000000 suql-1.1.7a1/src/suql/sql_free_text_support/__init__.py
--rw-------   0 oval      (1000) users      (100)    70881 2024-05-02 17:42:48.000000 suql-1.1.7a1/src/suql/sql_free_text_support/execute_free_text_sql.py
--rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.1.7a1/src/suql/utils.py
-drwx------   0 oval      (1000) users      (100)        0 2024-05-02 17:44:39.552665 suql-1.1.7a1/src/suql.egg-info/
--rw-r--r--   0 oval      (1000) users      (100)     5021 2024-05-02 17:44:39.000000 suql-1.1.7a1/src/suql.egg-info/PKG-INFO
--rw-------   0 oval      (1000) users      (100)      824 2024-05-02 17:44:39.000000 suql-1.1.7a1/src/suql.egg-info/SOURCES.txt
--rw-------   0 oval      (1000) users      (100)        1 2024-05-02 17:44:39.000000 suql-1.1.7a1/src/suql.egg-info/dependency_links.txt
--rw-------   0 oval      (1000) users      (100)      206 2024-05-02 17:44:39.000000 suql-1.1.7a1/src/suql.egg-info/requires.txt
--rw-------   0 oval      (1000) users      (100)        5 2024-05-02 17:44:39.000000 suql-1.1.7a1/src/suql.egg-info/top_level.txt
+drwx------   0 oval      (1000) users      (100)        0 2024-05-07 05:12:34.676460 suql-1.1.7a2/
+-rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.1.7a2/LICENSE
+-rw-------   0 oval      (1000) users      (100)     5021 2024-05-07 05:12:34.676460 suql-1.1.7a2/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)     4415 2024-04-30 04:28:53.000000 suql-1.1.7a2/README.md
+-rw-------   0 oval      (1000) users      (100)       38 2024-05-07 05:12:34.676460 suql-1.1.7a2/setup.cfg
+-rw-------   0 oval      (1000) users      (100)     1541 2024-05-07 05:12:07.000000 suql-1.1.7a2/setup.py
+drwx------   0 oval      (1000) users      (100)        0 2024-05-07 05:12:34.672460 suql-1.1.7a2/src/
+drwx------   0 oval      (1000) users      (100)        0 2024-05-07 05:12:34.676460 suql-1.1.7a2/src/suql/
+-rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.1.7a2/src/suql/__init__.py
+-rw-------   0 oval      (1000) users      (100)    17393 2024-05-02 21:44:59.000000 suql-1.1.7a2/src/suql/agent.py
+-rw-------   0 oval      (1000) users      (100)    20797 2024-05-06 23:18:06.000000 suql-1.1.7a2/src/suql/faiss_embedding.py
+-rw-------   0 oval      (1000) users      (100)     8792 2024-04-17 07:27:02.000000 suql-1.1.7a2/src/suql/free_text_fcns_server.py
+-rw-------   0 oval      (1000) users      (100)     3563 2024-05-06 21:19:43.000000 suql-1.1.7a2/src/suql/postgresql_connection.py
+-rw-------   0 oval      (1000) users      (100)     9612 2024-04-17 08:33:05.000000 suql-1.1.7a2/src/suql/prompt_continuation.py
+drwx------   0 oval      (1000) users      (100)        0 2024-05-07 05:12:34.676460 suql-1.1.7a2/src/suql/prompts/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:18.000000 suql-1.1.7a2/src/suql/prompts/__init__.py
+-rw-------   0 oval      (1000) users      (100)      169 2024-04-03 06:02:28.000000 suql-1.1.7a2/src/suql/prompts/answer_qa.prompt
+-rw-------   0 oval      (1000) users      (100)      451 2024-04-03 06:02:28.000000 suql-1.1.7a2/src/suql/prompts/field_classification.prompt
+-rw-------   0 oval      (1000) users      (100)     2945 2024-04-03 06:02:28.000000 suql-1.1.7a2/src/suql/prompts/if_db_classification.prompt
+-rw-------   0 oval      (1000) users      (100)     1305 2024-04-03 06:02:28.000000 suql-1.1.7a2/src/suql/prompts/opening_hours.prompt
+-rw-------   0 oval      (1000) users      (100)     5574 2024-04-03 06:02:28.000000 suql-1.1.7a2/src/suql/prompts/parser_suql.prompt
+-rw-------   0 oval      (1000) users      (100)      227 2024-04-03 06:02:28.000000 suql-1.1.7a2/src/suql/prompts/verification.prompt
+-rw-------   0 oval      (1000) users      (100)     2983 2024-04-03 06:02:28.000000 suql-1.1.7a2/src/suql/prompts/yelp_response_SQL.prompt
+-rw-------   0 oval      (1000) users      (100)     1454 2024-04-03 06:02:28.000000 suql-1.1.7a2/src/suql/prompts/yelp_response_no_results.prompt
+drwx------   0 oval      (1000) users      (100)        0 2024-05-07 05:12:34.676460 suql-1.1.7a2/src/suql/sql_free_text_support/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:11.000000 suql-1.1.7a2/src/suql/sql_free_text_support/__init__.py
+-rw-------   0 oval      (1000) users      (100)    71135 2024-05-07 05:12:07.000000 suql-1.1.7a2/src/suql/sql_free_text_support/execute_free_text_sql.py
+-rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.1.7a2/src/suql/utils.py
+drwx------   0 oval      (1000) users      (100)        0 2024-05-07 05:12:34.676460 suql-1.1.7a2/src/suql.egg-info/
+-rw-r--r--   0 oval      (1000) users      (100)     5021 2024-05-07 05:12:34.000000 suql-1.1.7a2/src/suql.egg-info/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)      824 2024-05-07 05:12:34.000000 suql-1.1.7a2/src/suql.egg-info/SOURCES.txt
+-rw-------   0 oval      (1000) users      (100)        1 2024-05-07 05:12:34.000000 suql-1.1.7a2/src/suql.egg-info/dependency_links.txt
+-rw-------   0 oval      (1000) users      (100)      206 2024-05-07 05:12:34.000000 suql-1.1.7a2/src/suql.egg-info/requires.txt
+-rw-------   0 oval      (1000) users      (100)        5 2024-05-07 05:12:34.000000 suql-1.1.7a2/src/suql.egg-info/top_level.txt
```

### Comparing `suql-1.1.7a1/LICENSE` & `suql-1.1.7a2/LICENSE`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a1/PKG-INFO` & `suql-1.1.7a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.1.7a1
+Version: 1.1.7a2
 Summary: Structured and Unstructured Query Language (SUQL) Python API
 Home-page: https://github.com/stanford-oval/suql
 Author: Shicheng Liu
 Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: suql Version: 1.1.7a1 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.1.7a2 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `suql-1.1.7a1/README.md` & `suql-1.1.7a2/README.md`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a1/setup.py` & `suql-1.1.7a2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 # Package metadata
 name = "suql"
-version = "1.1.7a1"
+version = "1.1.7a2"
 description = "Structured and Unstructured Query Language (SUQL) Python API"
 author = "Shicheng Liu"
 author_email = "shicheng@cs.stanford.edu"
 url = "https://github.com/stanford-oval/suql"
 
 # Specify the packages to include. You can use `find_packages` to automatically discover them.
 packages = find_packages(where="src")
```

### Comparing `suql-1.1.7a1/src/suql/agent.py` & `suql-1.1.7a2/src/suql/agent.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a1/src/suql/faiss_embedding.py` & `suql-1.1.7a2/src/suql/faiss_embedding.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a1/src/suql/free_text_fcns_server.py` & `suql-1.1.7a2/src/suql/free_text_fcns_server.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a1/src/suql/postgresql_connection.py` & `suql-1.1.7a2/src/suql/postgresql_connection.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a1/src/suql/prompt_continuation.py` & `suql-1.1.7a2/src/suql/prompt_continuation.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a1/src/suql/prompts/if_db_classification.prompt` & `suql-1.1.7a2/src/suql/prompts/if_db_classification.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a1/src/suql/prompts/opening_hours.prompt` & `suql-1.1.7a2/src/suql/prompts/opening_hours.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a1/src/suql/prompts/parser_suql.prompt` & `suql-1.1.7a2/src/suql/prompts/parser_suql.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a1/src/suql/prompts/yelp_response_SQL.prompt` & `suql-1.1.7a2/src/suql/prompts/yelp_response_SQL.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a1/src/suql/prompts/yelp_response_no_results.prompt` & `suql-1.1.7a2/src/suql/prompts/yelp_response_no_results.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a1/src/suql/sql_free_text_support/execute_free_text_sql.py` & `suql-1.1.7a2/src/suql/sql_free_text_support/execute_free_text_sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -935,15 +935,16 @@
                     return
 
         to_execute_node = deepcopy(self.node)
 
         # change projection to include everything
         to_execute_node.targetList = (ResTarget(val=ColumnRef(fields=(A_Star(),))),)
         # set limit to 1, to see if there are results
-        to_execute_node.limitCount = Integer(ival=1)
+        to_execute_node.limitCount = A_Const(val=Integer(ival=1))
+        to_execute_node.limitOption = pglast.enums.nodes.LimitOption.LIMIT_OPTION_COUNT
         # change predicates
         to_execute_node.whereClause = node
         # reset any groupby clause
         to_execute_node.groupClause = None
         # reset sorting
         to_execute_node.sortClause = None
 
@@ -1117,14 +1118,17 @@
     def __call__(self, node):
         super().__call__(node)
 
     def visit_ColumnRef(self, ancestors: Ancestor, node: ColumnRef):
         if len(list(map(lambda x: x.sval, node.fields))) > 1:
             assert len(list(map(lambda x: x.sval, node.fields))) == 2
             node.fields = (String(sval="^".join(map(lambda x: x.sval, node.fields))),)
+        elif "^" in node.fields[0].sval:
+            # this means that it has already been replaced
+            pass
         else:
             res = None
             for table_name, columns in self.table_column_mapping.items():
                 if node.fields[0].sval in map(lambda x: x[0], columns):
                     if res is not None:
                         # the same field appears twice, this means that the original syntax is problematic
                         break
@@ -1138,35 +1142,32 @@
     predicate: BoolExpr,
     cache: dict,
     fts_fields: List,
     select_username: str,
     select_userpswd: str,
     llm_model_name: str
 ):
+    _ = RawStream()(original_node) # RawStream takes care of some issue, to investigate
     node = deepcopy(original_node)
     # change projection to include everything
     # there are a couple of cases here
     # the simplest case is if it is one table
     if len(node.fromClause) == 1 and isinstance(node.fromClause[0], RangeVar):
         node.targetList = (ResTarget(val=ColumnRef(fields=(A_Star(),))),)
     # these are full joins
     elif len(node.fromClause) == 1 and isinstance(node.fromClause[0], JoinExpr):
         all_projection_fields = []
         table_column_mapping = {}
         for table in [node.fromClause[0].larg, node.fromClause[0].rarg]:
             # find out what columns this table has
-            _, columns = _execute_structural_sql(
-                SelectStmt(fromClause=(table,)),
+            _, columns = execute_sql_with_column_info(
+                RawStream()(SelectStmt(fromClause=(table,), targetList=(ResTarget(val=ColumnRef(fields=(A_Star(),))),))),
                 database,
-                None,
-                cache,
-                fts_fields,
                 select_username,
                 select_userpswd,
-                llm_model_name
             )
             # give the projection fields new names
             projection_table_name = (
                 table.alias.aliasname if table.alias is not None else table.relname
             )
             table_column_mapping[projection_table_name] = columns
 
@@ -1191,23 +1192,19 @@
         if original_node.sortClause is not None:
             replace_original_target_visitor(original_node.sortClause)
     # next, there are tuple joins (self joins)
     elif len(node.fromClause) > 1 and isinstance(node.fromClause, tuple):
         all_projection_fields = []
         for table in node.fromClause:
             # find out what columns this table has
-            _, columns = _execute_structural_sql(
-                SelectStmt(fromClause=(table,)),
+            _, columns = execute_sql_with_column_info(
+                RawStream()(SelectStmt(fromClause=(table,), targetList=(ResTarget(val=ColumnRef(fields=(A_Star(),))),))),
                 database,
-                None,
-                cache,
-                fts_fields,
                 select_username,
                 select_userpswd,
-                llm_model_name
             )
             # give the projection fields new names
             projection_table_name = (
                 table.alias.aliasname if table.alias is not None else table.relname
             )
             for column in columns:
                 new_projection_clause = ResTarget(
```

### Comparing `suql-1.1.7a1/src/suql/utils.py` & `suql-1.1.7a2/src/suql/utils.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a1/src/suql.egg-info/PKG-INFO` & `suql-1.1.7a2/src/suql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.1.7a1
+Version: 1.1.7a2
 Summary: Structured and Unstructured Query Language (SUQL) Python API
 Home-page: https://github.com/stanford-oval/suql
 Author: Shicheng Liu
 Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: suql Version: 1.1.7a1 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.1.7a2 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `suql-1.1.7a1/src/suql.egg-info/SOURCES.txt` & `suql-1.1.7a2/src/suql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

