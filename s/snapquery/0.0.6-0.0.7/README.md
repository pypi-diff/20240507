# Comparing `tmp/snapquery-0.0.6.tar.gz` & `tmp/snapquery-0.0.7.tar.gz`

## Comparing `snapquery-0.0.6.tar` & `snapquery-0.0.7.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 snapquery-0.0.6/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 snapquery-0.0.6/.pydevproject
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 snapquery-0.0.6/snapquery.puml
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 snapquery-0.0.6/.github/workflows/build.yml
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 snapquery-0.0.6/.github/workflows/upload-to-pypi.yml
--rw-r--r--   0        0        0     7717 2020-02-02 00:00:00.000000 snapquery-0.0.6/samples/ceur-ws.json
--rw-r--r--   0        0        0   476121 2020-02-02 00:00:00.000000 snapquery-0.0.6/samples/scholia.json
--rw-r--r--   0        0        0   249023 2020-02-02 00:00:00.000000 snapquery-0.0.6/samples/wikidata-examples.json
--rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 snapquery-0.0.6/scripts/blackisort
--rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 snapquery-0.0.6/scripts/install
--rwxr-xr-x   0        0        0      231 2020-02-02 00:00:00.000000 snapquery-0.0.6/scripts/restore_db
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 snapquery-0.0.6/scripts/test
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snapquery-0.0.6/snapquery/__init__.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 snapquery-0.0.6/snapquery/error_filter.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 snapquery-0.0.6/snapquery/mwlogin.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 snapquery-0.0.6/snapquery/params.py
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 snapquery-0.0.6/snapquery/qimport.py
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 snapquery-0.0.6/snapquery/qimport_view.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 snapquery-0.0.6/snapquery/scholia.py
--rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 snapquery-0.0.6/snapquery/snapquery_cmd.py
--rw-r--r--   0        0        0    21351 2020-02-02 00:00:00.000000 snapquery-0.0.6/snapquery/snapquery_core.py
--rw-r--r--   0        0        0     7781 2020-02-02 00:00:00.000000 snapquery-0.0.6/snapquery/snapquery_view.py
--rw-r--r--   0        0        0     9162 2020-02-02 00:00:00.000000 snapquery-0.0.6/snapquery/snapquery_webserver.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 snapquery-0.0.6/snapquery/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snapquery-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 snapquery-0.0.6/tests/test_cmdline.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 snapquery-0.0.6/tests/test_endpoints.py
--rw-r--r--   0        0        0     9431 2020-02-02 00:00:00.000000 snapquery-0.0.6/tests/test_error_filter.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 snapquery-0.0.6/tests/test_import.py
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 snapquery-0.0.6/tests/test_namedqueries.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 snapquery-0.0.6/tests/test_oauth.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 snapquery-0.0.6/tests/test_params.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 snapquery-0.0.6/tests/test_restful_api.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 snapquery-0.0.6/tests/test_scholia.py
--rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 snapquery-0.0.6/tests/test_wd_query_parsing.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 snapquery-0.0.6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 snapquery-0.0.6/LICENSE
--rw-r--r--   0        0        0     9293 2020-02-02 00:00:00.000000 snapquery-0.0.6/README.md
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 snapquery-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    10798 2020-02-02 00:00:00.000000 snapquery-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 snapquery-0.0.7/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 snapquery-0.0.7/.pydevproject
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 snapquery-0.0.7/snapquery.puml
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 snapquery-0.0.7/.github/workflows/build.yml
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 snapquery-0.0.7/.github/workflows/upload-to-pypi.yml
+-rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 snapquery-0.0.7/scripts/blackisort
+-rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 snapquery-0.0.7/scripts/install
+-rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 snapquery-0.0.7/scripts/restore_db
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 snapquery-0.0.7/scripts/test
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snapquery-0.0.7/snapquery/__init__.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 snapquery-0.0.7/snapquery/error_filter.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 snapquery-0.0.7/snapquery/mwlogin.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 snapquery-0.0.7/snapquery/params_view.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 snapquery-0.0.7/snapquery/qimport.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 snapquery-0.0.7/snapquery/qimport_view.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 snapquery-0.0.7/snapquery/scholia.py
+-rw-r--r--   0        0        0     4678 2020-02-02 00:00:00.000000 snapquery-0.0.7/snapquery/snapquery_cmd.py
+-rw-r--r--   0        0        0    22470 2020-02-02 00:00:00.000000 snapquery-0.0.7/snapquery/snapquery_core.py
+-rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 snapquery-0.0.7/snapquery/snapquery_view.py
+-rw-r--r--   0        0        0    10538 2020-02-02 00:00:00.000000 snapquery-0.0.7/snapquery/snapquery_webserver.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 snapquery-0.0.7/snapquery/version.py
+-rw-r--r--   0        0        0     7717 2020-02-02 00:00:00.000000 snapquery-0.0.7/snapquery/samples/ceur-ws.json
+-rw-r--r--   0        0        0     7915 2020-02-02 00:00:00.000000 snapquery-0.0.7/snapquery/samples/endpoints.yaml
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 snapquery-0.0.7/snapquery/samples/meta_query.yaml
+-rw-r--r--   0        0        0   476121 2020-02-02 00:00:00.000000 snapquery-0.0.7/snapquery/samples/scholia.json
+-rw-r--r--   0        0        0   249023 2020-02-02 00:00:00.000000 snapquery-0.0.7/snapquery/samples/wikidata-examples.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snapquery-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 snapquery-0.0.7/tests/test_cmdline.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 snapquery-0.0.7/tests/test_endpoints.py
+-rw-r--r--   0        0        0     9431 2020-02-02 00:00:00.000000 snapquery-0.0.7/tests/test_error_filter.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 snapquery-0.0.7/tests/test_import.py
+-rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 snapquery-0.0.7/tests/test_namedqueries.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 snapquery-0.0.7/tests/test_oauth.py
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 snapquery-0.0.7/tests/test_restful_api.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 snapquery-0.0.7/tests/test_scholia.py
+-rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 snapquery-0.0.7/tests/test_wd_query_parsing.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 snapquery-0.0.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 snapquery-0.0.7/LICENSE
+-rw-r--r--   0        0        0     9293 2020-02-02 00:00:00.000000 snapquery-0.0.7/README.md
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 snapquery-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    10798 2020-02-02 00:00:00.000000 snapquery-0.0.7/PKG-INFO
```

### Comparing `snapquery-0.0.6/snapquery.puml` & `snapquery-0.0.7/snapquery.puml`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.6/.github/workflows/build.yml` & `snapquery-0.0.7/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.6/.github/workflows/upload-to-pypi.yml` & `snapquery-0.0.7/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.6/samples/ceur-ws.json` & `snapquery-0.0.7/snapquery/samples/ceur-ws.json`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.6/samples/scholia.json` & `snapquery-0.0.7/snapquery/samples/scholia.json`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.6/samples/wikidata-examples.json` & `snapquery-0.0.7/snapquery/samples/wikidata-examples.json`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.6/snapquery/error_filter.py` & `snapquery-0.0.7/snapquery/error_filter.py`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.6/snapquery/mwlogin.py` & `snapquery-0.0.7/snapquery/mwlogin.py`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.6/snapquery/qimport.py` & `snapquery-0.0.7/snapquery/qimport.py`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.6/snapquery/qimport_view.py` & `snapquery-0.0.7/snapquery/qimport_view.py`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.6/snapquery/scholia.py` & `snapquery-0.0.7/snapquery/scholia.py`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.6/snapquery/snapquery_cmd.py` & `snapquery-0.0.7/snapquery/snapquery_cmd.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 @author: wf
 """
 
 import sys
 from argparse import ArgumentParser
 
-from lodstorage.query import EndpointManager, Format
+from lodstorage.params import Params, StoreDictKeyPair
+from lodstorage.query import Format
 from ngwidgets.cmd import WebserverCmd
 
 from snapquery.qimport import QueryImport
 from snapquery.snapquery_core import NamedQueryManager
 from snapquery.snapquery_webserver import SnapQueryWebServer
 
 
@@ -44,14 +45,19 @@
             action="store_true",
             help="show the list of available endpoints",
         )
         parser.add_argument(
             "--limit", type=int, default=None, help="set limit parameter of query"
         )
         parser.add_argument(
+            "--params",
+            action=StoreDictKeyPair,
+            help="query parameters as Key-value pairs in the format key1=value1,key2=value2",
+        )
+        parser.add_argument(
             "--namespace",
             type=str,
             default="wikidata-examples",
             help="namespace to filter queries",
         )
         parser.add_argument("-f", "--format", type=Format, choices=list(Format))
         parser.add_argument("-qn", "--queryName", help="run a named query")
@@ -65,31 +71,38 @@
 
     def handle_args(self) -> bool:
         """
         handle the command line args
         """
         # Call the superclass handle_args to maintain base class behavior
         handled = super().handle_args()
-        endpoints = EndpointManager.getEndpoints(self.args.endpointPath, lang="sparql")
+        nqm = NamedQueryManager.from_samples()
         # Check if listing of endpoints is requested
         if self.args.listEndpoints:
             # List endpoints
-            for endpoint in endpoints.values():
+            for endpoint in nqm.endpoints.values():
                 print(endpoint)
             handled = True  # Operation handled
         elif self.args.queryName is not None:
-            nqm = NamedQueryManager.from_samples()
             namespace = self.args.namespace
             name = self.args.queryName
             endpoint_name = self.args.endpointName
             r_format = self.args.format
             limit = self.args.limit
             qb = nqm.get_query(
                 name=name, namespace=namespace, endpoint_name=endpoint_name, limit=limit
             )
+            query = qb.query
+            params = Params(query.query)
+            if params.has_params:
+                if not self.args.params:
+                    raise Exception(f"{query.name} needs parameters")
+                else:
+                    params.set(self.args.params)
+                    query.query = params.apply_parameters()
             if r_format == Format.raw:
                 formatted_result = qb.raw_query()
             else:
                 qlod = qb.get_lod()
                 formatted_result = qb.format_result(qlod=qlod, r_format=r_format)
             print(formatted_result)
         elif self.args.import_file:
```

### Comparing `snapquery-0.0.6/snapquery/snapquery_core.py` & `snapquery-0.0.7/snapquery/snapquery_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 import re
 import uuid
 from dataclasses import field, fields
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Type
 
 import requests
-from lodstorage.csv import CSV
-from lodstorage.query import Endpoint, EndpointManager, Format, Query
+from lodstorage.lod_csv import CSV
+from lodstorage.query import Endpoint, EndpointManager, Format, Query, QueryManager
 from lodstorage.sparql import SPARQL
 from lodstorage.sql import SQLDB, EntityInfo
 from lodstorage.yamlable import lod_storable
 from ngwidgets.widgets import Link
 
 
 @lod_storable
@@ -27,14 +27,15 @@
     """
     statistics about a query
     """
 
     stats_id: str = field(init=False)
     query_id: str  # foreign key
     endpoint_name: str  # foreign key
+    records: Optional[int] = None
     time_stamp: datetime.datetime = field(init=False)
     duration: float = field(init=False, default=None)  # duration in seconds
     error_msg: Optional[str] = None
 
     def __post_init__(self):
         """
         Post-initialization processing to construct a unique identifier for the query
@@ -53,31 +54,36 @@
         """
         Handle exception of query
         """
         self.duration = None
         self.error_msg = str(ex)
 
     def as_record(self) -> Dict:
+        """
+        convert my declared attributes to a dict
+        @TODO may be use asdict from dataclasses instead?
+        """
         record = {}
         for field in fields(self):
             # Include field in the record dictionary if it has already been initialized (i.e., not None or has default)
             if hasattr(self, field.name):
                 record[field.name] = getattr(self, field.name)
         return record
 
     @classmethod
     def get_samples(cls) -> dict[str, "QueryStats"]:
         """
         get samples
         """
         samples = {
-            "wikidata-examples": [
+            "snapquery-examples": [
                 QueryStats(
-                    query_id="wikidata-examples.cats",
+                    query_id="snapquery-examples.cats",
                     endpoint_name="wikidata",
+                    records=223,
                     error_msg="",
                 )
             ]
         }
         # Set the duration for each sample instance
         for sample_list in samples.values():
             for sample in sample_list:
@@ -123,48 +129,50 @@
 
     @classmethod
     def get_samples(cls) -> dict[str, "NamedQuery"]:
         """
         get samples
         """
         samples = {
-            "wikidata-examples": [
+            "snapquery-examples": [
                 NamedQuery(
-                    namespace="wikidata-examples",
+                    namespace="snapquery-examples",
                     name="cats",
                     url="https://www.wikidata.org/wiki/Wikidata:SPARQL_query_service/queries/examples#Cats",
                     title="Cats on Wikidata",
                     description="This query retrieves all items classified under 'house cat' (Q146) on Wikidata.",
-                    sparql="""
+                    sparql="""# snapquery cats example
 SELECT ?item ?itemLabel
 WHERE {
   ?item wdt:P31 wd:Q146. # Must be a cat
-  SERVICE wikibase:label { bd:serviceParam wikibase:language "[AUTO_LANGUAGE],en". }
+  OPTIONAL { ?item rdfs:label ?itemLabel. }
+  FILTER (LANG(?itemLabel) = "en")
 }
 """,
                 ),
                 NamedQuery(
-                    namespace="wikidata-examples",
+                    namespace="snapquery-examples",
                     name="horses",
                     url="https://www.wikidata.org/wiki/Wikidata:SPARQL_query_service/queries/examples#Horses_(showing_some_info_about_them)",
                     title="Horses on Wikidata",
                     description="This query retrieves information about horses, including parents, gender, and approximate birth and death years.",
-                    sparql="""
+                    sparql="""# snapquery example horses
 SELECT DISTINCT ?horse ?horseLabel ?mother ?motherLabel ?father ?fatherLabel 
 (year(?birthdate) as ?birthyear) (year(?deathdate) as ?deathyear) ?genderLabel
 WHERE {
   ?horse wdt:P31/wdt:P279* wd:Q726 .     # Instance and subclasses of horse (Q726)
   OPTIONAL{?horse wdt:P25 ?mother .}     # Mother
   OPTIONAL{?horse wdt:P22 ?father .}     # Father
   OPTIONAL{?horse wdt:P569 ?birthdate .} # Birth date
   OPTIONAL{?horse wdt:P570 ?deathdate .} # Death date
   OPTIONAL{?horse wdt:P21 ?gender .}     # Gender
-  SERVICE wikibase:label {
-    bd:serviceParam wikibase:language "[AUTO_LANGUAGE],fr,ar,be,bg,bn,ca,cs,da,de,el,en,es,et,fa,fi,he,hi,hu,hy,id,it,ja,jv,ko,nb,nl,eo,pa,pl,pt,ro,ru,sh,sk,sr,sv,sw,te,th,tr,uk,yue,vec,vi,zh"
-  }
+  OPTIONAL { ?horse rdfs:label ?horseLabel . FILTER (lang(?horseLabel) = "en") }
+  OPTIONAL { ?mother rdfs:label ?motherLabel . FILTER (lang(?motherLabel) = "en") }
+  OPTIONAL { ?father rdfs:label ?fatherLabel . FILTER (lang(?fatherLabel) = "en") }
+  OPTIONAL { ?gender rdfs:label ?genderLabel . FILTER (lang(?genderLabel) = "en") }
 }
 ORDER BY ?horse
 """,
                 ),
             ]
         }
         return samples
@@ -226,27 +234,30 @@
     Attributes:
         named_query (NamedQuery): The named query object, which includes metadata about the query.
         query (Query): The actual query object that contains the SPARQL query string.
         endpoint (Endpoint): The endpoint object where the SPARQL query should be executed.
         sparql (SPARQL): A SPARQL service object initialized with the endpoint URL.
     """
 
-    def __init__(self, named_query: NamedQuery, query: Query, endpoint: Endpoint):
+    def __init__(
+        self, named_query: NamedQuery, query: Query, endpoint: Endpoint = None
+    ):
         """
         Initializes a new instance of the QueryBundle class.
 
         Args:
             named_query (NamedQuery): An instance of NamedQuery that provides a named reference to the query.
             query (Query): An instance of Query containing the SPARQL query string.
             endpoint (Endpoint): An instance of Endpoint representing the SPARQL endpoint URL.
         """
         self.named_query = named_query
         self.query = query
         self.endpoint = endpoint
-        self.sparql = SPARQL(endpoint.endpoint)
+        if endpoint:
+            self.sparql = SPARQL(endpoint.endpoint)
 
     def raw_query(self, resultFormat, mime_type: str = None, timeout: float = 10.0):
         """
         returns raw result of the endpoint
 
         Args:
             resultFormat(str): format of the result
@@ -292,14 +303,15 @@
             List[dict]: A list where each dictionary represents a row of results from the SPARQL query.
         """
         query_stat = QueryStats(
             query_id=self.query.name, endpoint_name=self.endpoint.name
         )
         try:
             lod = self.sparql.queryAsListOfDicts(self.query.query)
+            query_stat.records = len(lod) if lod else -1
             query_stat.done()
         except Exception as ex:
             lod = None
             query_stat.error(ex)
         return (lod, query_stat)
 
     def format_result(
@@ -321,17 +333,20 @@
         if qlod is None:
             qlod = self.get_lod()
         if r_format is None:
             r_format = Format.json
         if r_format == Format.csv:
             csv_output = CSV.toCSV(qlod)
             return csv_output
-        elif r_format in [Format.latex, Format.github, Format.mediawiki, Format.html]:
+        elif r_format in [Format.latex, 
+            Format.github, 
+            Format.mediawiki, 
+            Format.html]:
             doc = self.query.documentQueryResult(
-                qlod, tablefmt=str(r_format), floatfmt=".0f"
+                qlod, tablefmt=str(r_format), floatfmt=".1f"
             )
             return doc.asText()
         elif r_format == Format.json:
             return json.dumps(qlod, indent=2, sort_keys=True, default=str)
         return None  # In case no format is matched or needed
 
     def set_limit(self, limit: int = None):
@@ -373,15 +388,27 @@
             sql_db (SQLDB): An instance of SQLDB to manage the SQLite database interactions.
             endpoints (dict): A dictionary of SPARQL endpoints configured for use.
         """
         if db_path is None:
             db_path = NamedQueryManager.get_cache_path()
         self.debug = debug
         self.sql_db = SQLDB(dbname=db_path, check_same_thread=False, debug=debug)
-        self.endpoints = EndpointManager.getEndpoints(lang="sparql")
+        # Get the path of the yaml_file relative to the current Python module
+        samples_path = os.path.join(
+            os.path.dirname(os.path.abspath(__file__)), "samples"
+        )
+        endpoints_path = os.path.join(samples_path, "endpoints.yaml")
+        self.endpoints = EndpointManager.getEndpoints(
+            endpointPath=endpoints_path, lang="sparql", with_default=False
+        )
+        yaml_path = os.path.join(samples_path, "meta_query.yaml")
+        self.meta_qm = QueryManager(
+            queriesPath=yaml_path, with_default=False, lang="sql"
+        )
+        pass
 
     @classmethod
     def get_cache_path(cls) -> str:
         home = str(Path.home())
         cache_dir = f"{home}/.solutions/snapquery/storage"
         os.makedirs(cache_dir, exist_ok=True)
         cache_path = f"{cache_dir}/named_queries.db"
@@ -560,15 +587,16 @@
         query = Query(
             name=name,
             query=sparql_query,
             lang="sparql",
             endpoint=endpoint.endpoint,
             limit=limit,
         )
-        endpointConf = self.endpoints.get(endpoint_name, Endpoint.getDefault())
+        self.endpointConf = self.endpoints.get(endpoint_name, Endpoint.getDefault())
         query.tryItUrl = query.getTryItUrl(endpoint.website, endpoint.database)
-        query.database = endpointConf.database
+        query.database = self.endpointConf.database
+        query.query = f"{self.endpointConf.prefixes}\n{query.query}"
         query_bundle = QueryBundle(
             named_query=named_query, query=query, endpoint=endpoint
         )
         query_bundle.set_limit(limit)
         return query_bundle
```

### Comparing `snapquery-0.0.6/snapquery/snapquery_view.py` & `snapquery-0.0.7/snapquery/snapquery_view.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 @author: wf
 """
 
 import asyncio
 from typing import List
 
+from lodstorage.params import Params
 from lodstorage.query import QuerySyntaxHighlight, ValueFormatter
-from ngwidgets.dict_edit import DictEdit
 from ngwidgets.input_webserver import InputWebSolution
 from ngwidgets.lod_grid import ListOfDictsGrid
 from ngwidgets.widgets import Link
 from nicegui import background_tasks, run, ui
 
 from snapquery.error_filter import ErrorFilter
-from snapquery.params import Params
+from snapquery.params_view import ParamsView
 from snapquery.snapquery_core import NamedQuery, QueryBundle, QueryStats
 
 
 class NamedQueryView:
     """
     display a named Query
     """
@@ -55,15 +55,16 @@
                 ui.number(label="limit").bind_value(self, "limit")
                 ui.number(label="time out").bind_value(self, "timeout")
             with ui.row() as self.query_row:
                 self.try_it_link = ui.html(link)
                 ui.label(nq.description)
                 self.params = Params(nq.sparql)
                 if self.params.has_params:
-                    self.params_edit = self.params.get_dict_edit()
+                    self.params_view = ParamsView(self, self.params)
+                    self.params_edit = self.params_view.get_dict_edit()
                     pass
                 ui.button(icon="play_arrow", on_click=self.run_query)
                 self.stats_html = ui.html()
             with ui.row():
                 with ui.expansion("Show Query", icon="manage_search").classes("w-full"):
                     query_syntax_highlight = QuerySyntaxHighlight(
                         self.query_bundle.query
@@ -78,15 +79,15 @@
 
     async def load_query_results(self):
         """
         (re) load the query results
         """
         if self.params.has_params:
             self.query_bundle.query.query = self.params.apply_parameters()
-            self.params.close()
+            self.params_view.close()
         self.query_bundle.set_limit(int(self.limit))
         (lod, stats) = await run.io_bound(self.query_bundle.get_lod_with_stats)
         self.nqm.store(
             [stats.as_record()], source_class=QueryStats, primary_key="stats_id"
         )
         self.grid_row.clear()
         if stats.error_msg:
```

### Comparing `snapquery-0.0.6/snapquery/snapquery_webserver.py` & `snapquery-0.0.7/snapquery/snapquery_webserver.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 Created on 2024-05-03
 @author: wf
 """
 
 from fastapi import HTTPException
-from fastapi.responses import FileResponse, HTMLResponse, PlainTextResponse
+from fastapi.responses import HTMLResponse, PlainTextResponse
 from lodstorage.query import Format
 from ngwidgets.input_webserver import InputWebserver, InputWebSolution, WebserverConfig
 from ngwidgets.login import Login
 from ngwidgets.users import Users
 from nicegui import app, ui
 from nicegui.client import Client
 from starlette.responses import RedirectResponse
 
 from snapquery.qimport_view import QueryImportView
-from snapquery.snapquery_core import NamedQueryManager, QueryStats
+from snapquery.snapquery_core import NamedQueryManager, QueryBundle, QueryStats
 from snapquery.snapquery_view import NamedQuerySearch, NamedQueryView
 from snapquery.version import Version
 
 
 class SnapQueryWebServer(InputWebserver):
     """
     server to supply named Queries
@@ -31,14 +31,15 @@
         """
         copy_right = ""
         config = WebserverConfig(
             short_name="snapquery",
             copy_right=copy_right,
             version=Version(),
             default_port=9862,
+            timeout=6.0,
         )
         server_config = WebserverConfig.get(config)
         server_config.solution_class = SnapQuerySolution
         return server_config
 
     def __init__(self):
         """Constructs all the necessary attributes for the WebServer object."""
@@ -82,17 +83,38 @@
                 endpoint_name=endpoint_name,
                 limit=limit,
                 r_format_str=format,
             )
 
         @app.get("/api/endpoints")
         def get_endpoints():
+            """
+            list all endpoints
+            """
             endpoints = self.nqm.endpoints
             return endpoints
 
+        @app.get("/api/meta_query/{name}")
+        def meta_query(name: str, limit: int = None):
+            """
+            run the meta query with the given name
+            """
+            name, r_format = self.get_r_format(name, "json")
+            if not name in self.nqm.meta_qm.queriesByName:
+                raise HTTPException(
+                    status_code=404, detail=f"meta query {name} not known"
+                )
+            query = self.nqm.meta_qm.queriesByName[name]
+            qb = QueryBundle(named_query=None, query=query)
+            qlod = self.nqm.sql_db.query(query.query)
+            if limit:
+                qlod = qlod[:limit]
+            content = qb.format_result(qlod, r_format)
+            return HTMLResponse(content)
+
         @app.get("/api/sparql/{namespace}/{name}")
         def sparql(
             namespace: str,
             name: str,
             endpoint_name: str = "wikidata",
             limit: int = None,
         ) -> PlainTextResponse:
@@ -141,14 +163,35 @@
             )
             if not content:
                 raise HTTPException(status_code=500, detail="Could not create result")
 
             # Return the content as an HTML response
             return HTMLResponse(content)
 
+    def get_r_format(self, name: str, default_format_str: str = "html") -> Format:
+        """
+        get the result format from the given query name following the
+        dot convention that <name>.<r_format_str> specifies the result format
+        e.g. cats.json will ask for the json result format
+
+        Args:
+            name(str): the name of the query/meta query
+            default_format_str(str): the name of the default format to use
+
+        Returns:
+            Format: the result format
+        """
+        if "." in name:
+            r_format_str = name.split(".")[-1]
+            name = name[: name.rfind(".")]
+        else:
+            r_format_str = default_format_str
+        r_format = Format[r_format_str]
+        return name, r_format
+
     def query(
         self,
         namespace: str,
         name: str,
         endpoint_name: str = "wikidata",
         limit: int = None,
     ) -> str:
@@ -160,24 +203,17 @@
             name (str): The name identifier of the data to be queried.
             endpoint_name (str): The name of the endpoint to be used for the query. Defaults to 'wikidata'.
             limit(int): the limit for the query default: None
 
             Returns:
                 str: the content retrieved
         """
-        # content negotiation
-        # Determine response format by extension in the name or Accept header
-        if "." in name:
-            r_format_str = name.split(".")[-1]
-            name = name[: name.rfind(".")]
-        else:
-            r_format_str = "html"
-
         try:
-            r_format = Format[r_format_str]
+            # content negotiation
+            name, r_format = self.get_r_format(name)
             qb = self.nqm.get_query(name, namespace, endpoint_name, limit)
             (qlod, stats) = qb.get_lod_with_stats()
             self.nqm.store(
                 [stats.as_record()], source_class=QueryStats, primary_key="stats_id"
             )
             content = qb.format_result(qlod, r_format)
             return content
```

### Comparing `snapquery-0.0.6/snapquery/version.py` & `snapquery-0.0.7/snapquery/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     """
     Version handling for nicepdf
     """
 
     name = "snapquery"
     version = snapquery.__version__
     date = "2024-05-03"
-    updated = "2024-05-06"
+    updated = "2024-05-07"
     description = "Introduce Named Queries and Named Query Middleware to wikidata"
 
     authors = "Wolfgang Fahl"
 
     doc_url = "https://wiki.bitplan.com/index.php/snapquery"
     chat_url = "https://github.com/WolfgangFahl/snapquery/discussions"
     cm_url = "https://github.com/WolfgangFahl/snapquery"
```

### Comparing `snapquery-0.0.6/tests/test_cmdline.py` & `snapquery-0.0.7/tests/test_cmdline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Created on 2024-05-04
 
 @author: wf
 """
 import contextlib
 import json
-import sys
 import unittest
 from io import StringIO
 
 from ngwidgets.basetest import Basetest
 
 from snapquery import snapquery_cmd
```

### Comparing `snapquery-0.0.6/tests/test_endpoints.py` & `snapquery-0.0.7/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.6/tests/test_error_filter.py` & `snapquery-0.0.7/tests/test_error_filter.py`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.6/tests/test_import.py` & `snapquery-0.0.7/tests/test_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 class TestImport(Basetest):
     """
     test importing  named queries
     """
 
-    def setUp(self, debug=True, profile=True):
+    def setUp(self, debug=False, profile=True):
         Basetest.setUp(self, debug=debug, profile=profile)
 
     def testImport(self):
         """
         Test importing named queries.
         """
         qimport = QueryImport()
```

### Comparing `snapquery-0.0.6/tests/test_namedqueries.py` & `snapquery-0.0.7/tests/test_namedqueries.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 
     def testNamedQueries(self):
         """
         test getting a named query manager
         """
         db_path = "/tmp/named_queries.db"
         nqm = NamedQueryManager.from_samples(db_path=db_path)
-        for name, ex_count in [("x-invalid", -1), ("cats", 223)]:
+        for name, ex_count in [("x-invalid", -1), ("cats", 205)]:
             try:
-                query_bundle = nqm.get_query(name)
+                query_bundle = nqm.get_query(namespace="snapquery-examples", name=name)
                 lod = query_bundle.get_lod()
                 if self.debug:
                     print(f"{name}:")
                     print(json.dumps(lod, default=str, indent=2))
                 self.assertEqual(ex_count, len(lod))
             except Exception as ex:
                 if self.debug:
@@ -42,29 +42,50 @@
 
     def test_query_with_stats(self):
         """
         tests executing a query with stats
         """
         with tempfile.NamedTemporaryFile() as tmpfile:
             nqm = NamedQueryManager.from_samples(db_path=tmpfile.name)
-            query_bundle = nqm.get_query("cats")
+            query_bundle = nqm.get_query(namespace="snapquery-examples", name="cats")
             lod, query_stats = query_bundle.get_lod_with_stats()
             self.assertEqual(query_bundle.query.name, query_stats.query_id)
             self.assertEqual(query_stats.endpoint_name, query_bundle.endpoint.name)
             self.assertIsNone(query_stats.error_msg)
             self.assertIsNotNone(query_stats.duration)
 
-    @unittest.skip
+    def test_meta_queries(self):
+        """
+        test meta queries
+        """
+        nqm = NamedQueryManager.from_samples()
+        self.assertTrue("query_count" in nqm.meta_qm.queriesByName)
+        pass
+
     def test_query_with_stats_evaluation(self):
         """
         test query stats evaluation and storage on a bunch of queries
         """
-        nqm = NamedQueryManager.from_samples()
-        query_records = nqm.sql_db.query("SELECT * FROM NamedQuery LIMIT 20")
+        nqm = NamedQueryManager.from_samples(db_path="/tmp/stats_eval.db")
+        limit = 1
+        if self.inPublicCI():
+            limit = 2
+        query_records = nqm.sql_db.query(
+            f"SELECT * FROM NamedQuery WHERE namespace='snapquery-examples' LIMIT {limit}"
+        )
         query_stats = []
-        for query_record in query_records:
+        for i, query_record in enumerate(query_records):
             named_query = NamedQuery.from_record(query_record)
-            query_bundle = nqm.get_query(named_query.name, named_query.namespace)
+            query_bundle = nqm.get_query(
+                named_query.name,
+                named_query.namespace,
+                endpoint_name="wikidata-openlinksw",
+            )
+            if self.debug:
+                print(f"{i+1:3}/{len(query_records)}:{named_query.query_id}")
             lod, query_stat = query_bundle.get_lod_with_stats()
+            lod_len = len(lod) if lod else 0
+            if self.debug:
+                print(f"    {lod_len} records:{query_stat.duration:.1f} s")
             query_stats.append(query_stat)
         stat_lod = [qs.as_record() for qs in query_stats]
         nqm.store(stat_lod, source_class=QueryStats, primary_key="stats_id")
```

### Comparing `snapquery-0.0.6/tests/test_oauth.py` & `snapquery-0.0.7/tests/test_oauth.py`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.6/tests/test_restful_api.py` & `snapquery-0.0.7/tests/test_restful_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,36 +24,48 @@
         """
         test API docs access
         """
         # self.debug=True
         html = self.getHtml("/docs")
         self.assertTrue("Swagger" in html)
 
+    def testMetaApi(self):
+        """
+        test the meta api
+        """
+        for qname, ex_status in [("query_count", 200), ("unknown_query_name", 404)]:
+            try:
+                meta_data = self.get_json(f"/api/meta_query/{qname}", ex_status)
+                if self.debug:
+                    print(meta_data)
+            except Exception as _ex:
+                self.assertEqual(404, ex_status)
+
     def testEndpointApi(self):
         """
         test the endpoints api
         """
         endpoints_data = self.get_json("/api/endpoints")
         if self.debug:
             print(endpoints_data)
         self.assertTrue("wikidata" in endpoints_data)
 
     def testSparqlApi(self):
         """
         test the plaintext SPARQL API
         """
         for example in ["cats", "horses"]:
-            path = f"/api/sparql/wikidata-examples/{example}?limit=10"
+            path = f"/api/sparql/snapquery-examples/{example}?limit=10"
             sparql_query = self.getHtml(path)
             if self.debug:
                 print(sparql_query)
             self.assertTrue("SELECT" in sparql_query)
 
     def testQueryApi(self):
         """
         test the RESTFul Query API
         """
         for r_format in ["mediawiki", "github", "latex", "html", "json"]:
-            path = f"/api/query/wikidata-examples/cats.{r_format}?limit=10"
+            path = f"/api/query/snapquery-examples/cats.{r_format}?limit=10"
             result = self.getHtml(path)
             if self.debug:
                 print(result)
```

### Comparing `snapquery-0.0.6/tests/test_scholia.py` & `snapquery-0.0.7/tests/test_scholia.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 class TestScholia(Basetest):
     """
     test scholia queries
     """
 
-    def setUp(self, debug=True, profile=True):
+    def setUp(self, debug=False, profile=True):
         Basetest.setUp(self, debug=debug, profile=profile)
 
     def test_scholia_queries(self):
         """
         test retrieving scholia queries
         """
         db_path = "/tmp/scholia_queries.db"
```

### Comparing `snapquery-0.0.6/tests/test_wd_query_parsing.py` & `snapquery-0.0.7/tests/test_wd_query_parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 class TestWdQueryParsing(Basetest):
     """
     test wikidata query parsing
     """
 
-    def setUp(self, debug=True, profile=True):
+    def setUp(self, debug=False, profile=True):
         Basetest.setUp(self, debug=debug, profile=profile)
         self.base_url = "https://www.wikidata.org/wiki/Wikidata:SPARQL_query_service/queries/examples"
 
     def _get_examples_wikitext(self) -> str:
         """Get wiki text with SPARQL query examples"""
         res = requests.get(f"{self.base_url}?action=raw")
         return res.text
```

### Comparing `snapquery-0.0.6/.gitignore` & `snapquery-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.6/LICENSE` & `snapquery-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.6/README.md` & `snapquery-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.6/pyproject.toml` & `snapquery-0.0.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 license = {text = "Apache-2.0"}
 
 
 dependencies = [
 	# https://github.com/WolfgangFahl/nicegui_widgets
 	"ngwidgets>=0.15.0",
     # https://pypi.org/project/pyLodStorage/
-    "pyLodStorage>=0.10.5",
+    "pyLodStorage>=0.11.2",
     "wikitextparser",
     "requests",
     # https://pypi.org/project/mwoauth/
     "mwoauth>=0.4.0",
     #"mwoauth@git+https://github.com/mediawiki-utilities/python-mwoauth"
     #https://pypi.org/project/tqdm/
     "tqdm>=4.66.4"
```

### Comparing `snapquery-0.0.6/PKG-INFO` & `snapquery-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: snapquery
-Version: 0.0.6
+Version: 0.0.7
 Summary: snapquery: Introduce Named Queries and Named Query Middleware to wikidata
 Project-URL: Home, https://github.com/WolfgangFahl/snapquery
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/snapquery
 Project-URL: Source, https://github.com/WolfgangFahl/snapquery
 Author-email: Wolfgang Fahl <wf@WolfgangFahl.com>
 Maintainer-email: Wolfgang Fahl <wf@WolfgangFahl.com>
 License: Apache-2.0
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.9
 Requires-Dist: mwoauth>=0.4.0
 Requires-Dist: ngwidgets>=0.15.0
-Requires-Dist: pylodstorage>=0.10.5
+Requires-Dist: pylodstorage>=0.11.2
 Requires-Dist: requests
 Requires-Dist: tqdm>=4.66.4
 Requires-Dist: wikitextparser
 Provides-Extra: test
 Requires-Dist: green; extra == 'test'
 Description-Content-Type: text/markdown
```

