# Comparing `tmp/linkml_store-0.1.6.tar.gz` & `tmp/linkml_store-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkml_store-0.1.6.tar", max compression
+gzip compressed data, was "linkml_store-0.1.7.tar", max compression
```

## Comparing `linkml_store-0.1.6.tar` & `linkml_store-0.1.7.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0     1086 2024-05-02 02:57:57.011154 linkml_store-0.1.6/LICENSE
--rw-r--r--   0        0        0      451 2024-05-02 02:57:57.011154 linkml_store-0.1.6/README.md
--rw-r--r--   0        0        0     3447 2024-05-02 02:58:24.819061 linkml_store-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      118 2024-05-02 02:57:57.019154 linkml_store-0.1.6/src/linkml_store/__init__.py
--rw-r--r--   0        0        0      226 2024-05-02 02:57:57.019154 linkml_store-0.1.6/src/linkml_store/api/__init__.py
--rw-r--r--   0        0        0     7551 2024-05-02 02:57:57.019154 linkml_store-0.1.6/src/linkml_store/api/client.py
--rw-r--r--   0        0        0    17203 2024-05-02 02:57:57.019154 linkml_store-0.1.6/src/linkml_store/api/collection.py
--rw-r--r--   0        0        0     3269 2024-05-02 02:57:57.019154 linkml_store-0.1.6/src/linkml_store/api/config.py
--rw-r--r--   0        0        0    13701 2024-05-02 02:57:57.019154 linkml_store-0.1.6/src/linkml_store/api/database.py
--rw-r--r--   0        0        0     2028 2024-05-02 02:57:57.019154 linkml_store-0.1.6/src/linkml_store/api/queries.py
--rw-r--r--   0        0        0        0 2024-05-02 02:57:57.019154 linkml_store-0.1.6/src/linkml_store/api/stores/__init__.py
--rw-r--r--   0        0        0        0 2024-05-02 02:57:57.019154 linkml_store-0.1.6/src/linkml_store/api/stores/chromadb/__init__.py
--rw-r--r--   0        0        0     4186 2024-05-02 02:57:57.019154 linkml_store-0.1.6/src/linkml_store/api/stores/chromadb/chromadb_collection.py
--rw-r--r--   0        0        0     3205 2024-05-02 02:57:57.019154 linkml_store-0.1.6/src/linkml_store/api/stores/chromadb/chromadb_database.py
--rw-r--r--   0        0        0        0 2024-05-02 02:57:57.019154 linkml_store-0.1.6/src/linkml_store/api/stores/duckdb/__init__.py
--rw-r--r--   0        0        0     5859 2024-05-02 02:57:57.019154 linkml_store-0.1.6/src/linkml_store/api/stores/duckdb/duckdb_collection.py
--rw-r--r--   0        0        0     6591 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/api/stores/duckdb/duckdb_database.py
--rw-r--r--   0        0        0      123 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/api/stores/duckdb/mappings.py
--rw-r--r--   0        0        0        0 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/api/stores/hdf5/__init__.py
--rw-r--r--   0        0        0     3806 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/api/stores/hdf5/hdf5_collection.py
--rw-r--r--   0        0        0     2714 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/api/stores/hdf5/hdf5_database.py
--rw-r--r--   0        0        0        0 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/api/stores/mongodb/__init__.py
--rw-r--r--   0        0        0     3959 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/api/stores/mongodb/mongodb_collection.py
--rw-r--r--   0        0        0     3670 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/api/stores/mongodb/mongodb_database.py
--rw-r--r--   0        0        0     4723 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/api/stores/solr/solr_collection.py
--rw-r--r--   0        0        0     2876 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/api/stores/solr/solr_database.py
--rw-r--r--   0        0        0        0 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/api/stores/solr/solr_utils.py
--rw-r--r--   0        0        0    13667 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/cli.py
--rw-r--r--   0        0        0      112 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/constants.py
--rw-r--r--   0        0        0      881 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/index/__init__.py
--rw-r--r--   0        0        0        0 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/index/implementations/__init__.py
--rw-r--r--   0        0        0     1069 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/index/implementations/llm_indexer.py
--rw-r--r--   0        0        0     1251 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/index/implementations/simple_indexer.py
--rw-r--r--   0        0        0     3462 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/index/indexer.py
--rw-r--r--   0        0        0        0 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/utils/__init__.py
--rw-r--r--   0        0        0     3081 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/utils/format_utils.py
--rw-r--r--   0        0        0      884 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/utils/io.py
--rw-r--r--   0        0        0     2214 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/utils/object_utils.py
--rw-r--r--   0        0        0     5651 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/utils/sql_utils.py
--rw-r--r--   0        0        0     2064 1970-01-01 00:00:00.000000 linkml_store-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-05-06 22:05:38.652254 linkml_store-0.1.7/LICENSE
+-rw-r--r--   0        0        0      451 2024-05-06 22:05:38.652254 linkml_store-0.1.7/README.md
+-rw-r--r--   0        0        0     3471 2024-05-06 22:06:09.360716 linkml_store-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      118 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/__init__.py
+-rw-r--r--   0        0        0      226 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/api/__init__.py
+-rw-r--r--   0        0        0     7709 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/api/client.py
+-rw-r--r--   0        0        0    18460 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/api/collection.py
+-rw-r--r--   0        0        0     3409 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/api/config.py
+-rw-r--r--   0        0        0    17098 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/api/database.py
+-rw-r--r--   0        0        0     2028 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/api/queries.py
+-rw-r--r--   0        0        0        0 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/api/stores/__init__.py
+-rw-r--r--   0        0        0       46 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/api/stores/chromadb/__init__.py
+-rw-r--r--   0        0        0     4270 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/api/stores/chromadb/chromadb_collection.py
+-rw-r--r--   0        0        0     3205 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/api/stores/chromadb/chromadb_database.py
+-rw-r--r--   0        0        0      213 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/api/stores/duckdb/__init__.py
+-rw-r--r--   0        0        0     5854 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/api/stores/duckdb/duckdb_collection.py
+-rw-r--r--   0        0        0     6663 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/api/stores/duckdb/duckdb_database.py
+-rw-r--r--   0        0        0      123 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/api/stores/duckdb/mappings.py
+-rw-r--r--   0        0        0        0 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/api/stores/hdf5/__init__.py
+-rw-r--r--   0        0        0     3805 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/api/stores/hdf5/hdf5_collection.py
+-rw-r--r--   0        0        0     2714 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/api/stores/hdf5/hdf5_database.py
+-rw-r--r--   0        0        0        0 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/api/stores/mongodb/__init__.py
+-rw-r--r--   0        0        0     4111 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/api/stores/mongodb/mongodb_collection.py
+-rw-r--r--   0        0        0     3670 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/api/stores/mongodb/mongodb_database.py
+-rw-r--r--   0        0        0       36 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/api/stores/solr/__init__.py
+-rw-r--r--   0        0        0     4723 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/api/stores/solr/solr_collection.py
+-rw-r--r--   0        0        0     2877 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/api/stores/solr/solr_database.py
+-rw-r--r--   0        0        0        0 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/api/stores/solr/solr_utils.py
+-rw-r--r--   0        0        0    13667 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/cli.py
+-rw-r--r--   0        0        0      112 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/constants.py
+-rw-r--r--   0        0        0      881 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/index/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/index/implementations/__init__.py
+-rw-r--r--   0        0        0     1069 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/index/implementations/llm_indexer.py
+-rw-r--r--   0        0        0     1251 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/index/implementations/simple_indexer.py
+-rw-r--r--   0        0        0     3462 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/index/indexer.py
+-rw-r--r--   0        0        0        0 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/utils/__init__.py
+-rw-r--r--   0        0        0     3081 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/utils/format_utils.py
+-rw-r--r--   0        0        0      884 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/utils/io.py
+-rw-r--r--   0        0        0     2539 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/utils/object_utils.py
+-rw-r--r--   0        0        0     5651 2024-05-06 22:05:38.660255 linkml_store-0.1.7/src/linkml_store/utils/sql_utils.py
+-rw-r--r--   0        0        0     2064 1970-01-01 00:00:00.000000 linkml_store-0.1.7/PKG-INFO
```

### Comparing `linkml_store-0.1.6/LICENSE` & `linkml_store-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `linkml_store-0.1.6/pyproject.toml` & `linkml_store-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linkml-store"
-version = "0.1.6"
+version = "0.1.7"
 description = "linkml-store"
 authors = ["Author 1 <author@org.org>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9, !=3.9.7"
@@ -32,14 +32,15 @@
 pytest = {version = ">=7.1.2"}
 tox = {version = ">=3.25.1"}
 pre-commit = {version = ">=3.3.3"}
 sphinx = {version = ">=6.1.3"}
 sphinx-rtd-theme = {version = ">=1.0.0"}
 sphinx-autodoc-typehints = {version = "<2.0.0"}
 sphinx-click = {version = ">=4.3.0"}
+sphinx-automodapi = "*"
 myst-parser = {version = ">=0.18.1"}
 furo = {version = "*"}
 nbsphinx = "*"
 jupyter = "*"
 
 [tool.poetry.group.tests.dependencies]
 pytest = "^7.4.0"
```

### Comparing `linkml_store-0.1.6/src/linkml_store/api/client.py` & `linkml_store-0.1.7/src/linkml_store/api/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,19 @@
     "mongodb": MongoDBDatabase,
     "chromadb": ChromaDBDatabase,
 }
 
 
 class Client:
     """
-    A client provides access to named collections.
+    A client is the top-level object for interacting with databases.
+
+    A client has access to one or more :class:`Database` objects.
+
+    Each database consists of a number of :class:`.Collection` objects.
 
     Examples
     --------
     >>> client = Client()
     >>> db = client.attach_database("duckdb", alias="test")
     >>> collection = db.create_collection("Person")
     >>> objs = [{"id": "P1", "name": "John", "age_in_years": 30}, {"id": "P2", "name": "Alice", "age_in_years": 25}]
```

### Comparing `linkml_store-0.1.6/src/linkml_store/api/collection.py` & `linkml_store-0.1.7/src/linkml_store/api/collection.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import numpy as np
 from linkml_runtime.linkml_model import ClassDefinition, SlotDefinition
 from linkml_runtime.linkml_model.meta import ArrayExpression
 from pydantic import BaseModel
 
 from linkml_store.index import get_indexer
+from linkml_store.utils.object_utils import clean_empties
 
 try:
     from linkml.validator.report import ValidationResult
 except ImportError:
     ValidationResult = None
 
 from linkml_store.api.config import CollectionConfig
@@ -57,36 +58,49 @@
         else:
             self.metadata = CollectionConfig(name=name, **kwargs)
         if name is not None and self.metadata.name is not None and name != self.metadata.name:
             raise ValueError(f"Name mismatch: {name} != {self.metadata.name}")
 
     @property
     def name(self) -> str:
+        """
+        Return the name of the collection
+
+        :return:
+        """
         return self.metadata.name
 
     @property
     def hidden(self) -> bool:
+        """
+        True if the collection is hidden.
+
+        An example of a hidden collection is a collection that indexes another
+        collection
+
+        :return: True if the collection is hidden
+        """
         return self.metadata.hidden
 
     @property
-    def _target_class_name(self):
+    def target_class_name(self):
         """
         Return the name of the class that this collection represents
 
         This MUST be a LinkML class name
 
         :return:
         """
         # TODO: this is a shim layer until we can normalize on this
         if self.metadata.type:
             return self.metadata.type
         return self.name
 
     @property
-    def _alias(self):
+    def alias(self):
         """
         Return the primary name/alias used for the collection.
 
         This MAY be the name of the LinkML class, but it may be desirable
         to have an alias, for example "persons" which collects all instances
         of class Person.
 
@@ -152,15 +166,15 @@
         :param objs:
         :param kwargs:
         :return:
         """
         raise NotImplementedError
 
     def _create_query(self, **kwargs) -> Query:
-        return Query(from_table=self._alias, **kwargs)
+        return Query(from_table=self.alias, **kwargs)
 
     def query(self, query: Query, **kwargs) -> QueryResult:
         """
         Run a query against the collection
 
         :param query:
         :param kwargs:
@@ -197,29 +211,60 @@
         """
         Get one or more objects by ID.
 
         :param ids:
         :param kwargs:
         :return:
         """
-        id_field = self.identifier_field
-        q = self._create_query(where_clause={id_field: ids})
-        return self.query(q, **kwargs)
+        # TODO
+        id_field = self.identifier_attribute_name
+        return self.find({id_field: ids})
+
+    def get_one(self, id: IDENTIFIER, **kwargs) -> Optional[OBJECT]:
+        """
+        Get one object by ID.
+
+        :param id:
+        :param kwargs:
+        :return:
+        """
+        if not id:
+            raise ValueError("Must pass an ID")
+        id_field = self.identifier_attribute_name
+        if not id_field:
+            raise ValueError(f"No identifier for {self.name}")
+        w = {id_field: id}
+        qr = self.find(w)
+        if qr.num_rows == 1:
+            return qr.rows[0]
+        return None
 
     def find(self, where: Optional[Any] = None, **kwargs) -> QueryResult:
         """
         Find objects in the collection using a where query.
 
         :param where:
         :param kwargs:
         :return:
         """
         query = self._create_query(where_clause=where)
         return self.query(query, **kwargs)
 
+    def find_iter(self, where: Optional[Any] = None, **kwargs) -> Iterator[OBJECT]:
+        """
+        Find objects in the collection using a where query.
+
+        :param where:
+        :param kwargs:
+        :return:
+        """
+        qr = self.find(where=where, limit=-1, **kwargs)
+        for row in qr.rows:
+            yield row
+
     def search(
         self,
         query: str,
         where: Optional[Any] = None,
         index_name: Optional[str] = None,
         limit: Optional[int] = None,
         **kwargs,
@@ -358,29 +403,30 @@
         """
         Return the class definition for the collection.
 
         :return:
         """
         sv = self.parent.schema_view
         if sv:
-            cls = sv.get_class(self._target_class_name)
+            cls = sv.get_class(self.target_class_name)
             return cls
         return None
 
+    @property
     def identifier_attribute_name(self) -> Optional[str]:
         """
         Return the name of the identifier attribute for the collection.
 
         AKA the primary key.
 
         :return: The name of the identifier attribute, if one exists.
         """
         cd = self.class_definition()
         if cd:
-            for att in cd.attributes.values():
+            for att in self.parent.schema_view.class_induced_slots(cd.name):
                 if att.identifier:
                     return att.name
         return None
 
     def object_identifier(self, obj: OBJECT, auto=True) -> Optional[IDENTIFIER]:
         """
         Return the identifier for an object.
@@ -407,15 +453,15 @@
         This uses a heuristic procedure to infer the class definition from a list of objects.
         In general it is recommended you explicitly provide a schema.
 
         :param objs:
         :param max_sample_size:
         :return:
         """
-        cd = ClassDefinition(self._target_class_name)
+        cd = ClassDefinition(self.target_class_name)
         keys = defaultdict(list)
         for obj in objs[0:max_sample_size]:
             if isinstance(obj, BaseModel):
                 obj = obj.model_dump()
             if not isinstance(obj, dict):
                 logger.warning(f"Skipping non-dict object: {obj}")
                 continue
@@ -470,15 +516,15 @@
                 if rng != other_rng:
                     raise ValueError(f"Conflict: {rng} != {other_rng} for {vs}")
             cd.attributes[k] = SlotDefinition(k, range=rng, multivalued=multivalued, inlined=inlined)
             if exact_dimensions_list:
                 array_expr = ArrayExpression(exact_number_dimensions=len(exact_dimensions_list[0]))
                 cd.attributes[k].array = array_expr
         sv = self.parent.schema_view
-        sv.schema.classes[self._target_class_name] = cd
+        sv.schema.classes[self.target_class_name] = cd
         sv.set_modified()
         return cd
 
     def import_data(self, location: Union[Path, str, TextIO], **kwargs):
         """
         Import data from a file or stream
 
@@ -507,12 +553,13 @@
         """
         from linkml.validator import JsonschemaValidationPlugin, Validator
 
         validation_plugins = [JsonschemaValidationPlugin(closed=True)]
         validator = Validator(self.parent.schema_view.schema, validation_plugins=validation_plugins)
         cd = self.class_definition()
         if not cd:
-            raise ValueError(f"Cannot find class definition for {self._target_class_name}")
+            raise ValueError(f"Cannot find class definition for {self.target_class_name}")
         class_name = cd.name
         result = self.find(**kwargs)
         for obj in result.rows:
+            obj = clean_empties(obj)
             yield from validator.iter_results(obj, class_name)
```

### Comparing `linkml_store-0.1.6/src/linkml_store/api/config.py` & `linkml_store-0.1.7/src/linkml_store/api/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,14 +72,18 @@
             "document space; if this has a field 'document_type', then this field should be set"
         ),
     )
     searchable_slots: Optional[List[str]] = Field(
         default=None,
         description="Optional configuration for search fields",
     )
+    ensure_referential_integrity: bool = Field(
+        default=False,
+        description="Whether to ensure referential integrity",
+    )
 
 
 class ClientConfig(BaseModel):
     handle: Optional[str] = Field(
         default=None,
         description="The client handle",
     )
```

### Comparing `linkml_store-0.1.6/src/linkml_store/api/database.py` & `linkml_store-0.1.7/src/linkml_store/api/database.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
 from abc import ABC
+from collections import defaultdict
 from copy import copy
 from pathlib import Path
 from typing import TYPE_CHECKING, ClassVar, Dict, Iterator, Optional, Sequence, Type, Union
 
 try:
-    from linkml.validator.report import ValidationResult
+    from linkml.validator.report import Severity, ValidationResult
 except ImportError:
     ValidationResult = None
 
 from linkml_runtime import SchemaView
 from linkml_runtime.linkml_model import ClassDefinition, SchemaDefinition
 
 from linkml_store.api.collection import Collection
@@ -200,15 +201,14 @@
         :param alias: alias for the collection
         :param metadata: metadata for the collection
         :param recreate_if_exists: recreate the collection if it already exists
         :param kwargs: additional arguments
         """
         if not name:
             raise ValueError(f"Collection name must be provided: alias: {alias} metadata: {metadata}")
-        # collection_cls = self._collection_class
         collection_cls = self.collection_class
         collection = collection_cls(name=name, alias=alias, parent=self, metadata=metadata)
         if metadata and metadata.attributes:
             sv = self.schema_view
             schema = sv.schema
             cd = ClassDefinition(name=metadata.type, attributes=metadata.attributes)
             schema.classes[cd.name] = cd
@@ -337,22 +337,50 @@
         """
         if not self._schema_view:
             self._initialize_schema()
         if not self._schema_view:
             self._schema_view = self.induce_schema_view()
         return self._schema_view
 
-    def set_schema_view(self, schema_view: SchemaView):
+    def set_schema_view(self, schema_view: Union[str, Path, SchemaView]):
         """
         Set the schema view for the database.
 
         :param schema_view:
         :return:
         """
+        if isinstance(schema_view, Path):
+            schema_view = str(schema_view)
+        if isinstance(schema_view, str):
+            schema_view = SchemaView(schema_view)
         self._schema_view = schema_view
+        if not self._collections:
+            return
+        # align with induced schema
+        roots = [c for c in schema_view.all_classes().values() if c.tree_root]
+        if len(roots) == 0:
+            all_ranges = set()
+            for cn in schema_view.all_classes():
+                for slot in schema_view.class_induced_slots(cn):
+                    if slot.range:
+                        all_ranges.add(slot.range)
+            roots = [
+                c
+                for c in schema_view.all_classes().values()
+                if not all_ranges.intersection(schema_view.class_ancestors(c.name, reflexive=True))
+            ]
+        if len(roots) == 1:
+            root = roots[0]
+            for slot in schema_view.class_induced_slots(root.name):
+                inlined = slot.inlined or slot.inlined_as_list
+                if inlined and slot.range:
+                    if slot.name in self._collections:
+                        coll = self._collections[slot.name]
+                        if not coll.metadata.type:
+                            coll.metadata.type = slot.range
 
     def load_schema_view(self, path: Union[str, Path]):
         """
         Load a schema view from a file.
 
         >>> from linkml_store.api.client import Client
         >>> client = Client()
@@ -393,13 +421,59 @@
         Validate the contents of the database.
 
         :param kwargs:
         :return: iterator over validation results
         """
         for collection in self.list_collections():
             yield from collection.iter_validate_collection(**kwargs)
+        if self.metadata.ensure_referential_integrity:
+            yield from self._validate_referential_integrity(**kwargs)
+
+    def _validate_referential_integrity(self, **kwargs) -> Iterator["ValidationResult"]:
+        """
+        Validate referential integrity of the database.
+
+        :param kwargs:
+        :return: iterator over validation results
+        """
+        sv = self.schema_view
+        cmap = defaultdict(list)
+        for collection in self.list_collections():
+            if not collection.target_class_name:
+                raise ValueError(f"Collection {collection.name} has no target class")
+            cmap[collection.target_class_name].append(collection)
+        for collection in self.list_collections():
+            cd = collection.class_definition()
+            induced_slots = sv.class_induced_slots(cd.name)
+            slot_map = {s.name: s for s in induced_slots}
+            # rmap = {s.name: s.range for s in induced_slots}
+            sr_to_coll = {s.name: cmap.get(s.range, []) for s in induced_slots if s.range}
+            for obj in collection.find_iter():
+                for k, v in obj.items():
+                    if k not in sr_to_coll:
+                        continue
+                    ref_colls = sr_to_coll[k]
+                    if not ref_colls:
+                        continue
+                    if not isinstance(v, (str, int)):
+                        continue
+                    slot = slot_map[k]
+                    found = False
+                    for ref_coll in ref_colls:
+                        ref_obj = ref_coll.get_one(v)
+                        if ref_obj:
+                            found = True
+                            break
+                    if not found:
+                        yield ValidationResult(
+                            type="ReferentialIntegrity",
+                            severity=Severity.ERROR,
+                            message=f"Referential integrity error: {slot.range} not found",
+                            instantiates=slot.range,
+                            instance=v,
+                        )
 
     def drop(self, **kwargs):
         """
         Drop the database and all collections
         """
         raise NotImplementedError()
```

### Comparing `linkml_store-0.1.6/src/linkml_store/api/queries.py` & `linkml_store-0.1.7/src/linkml_store/api/queries.py`

 * *Files identical despite different names*

### Comparing `linkml_store-0.1.6/src/linkml_store/api/stores/chromadb/chromadb_collection.py` & `linkml_store-0.1.7/src/linkml_store/api/stores/chromadb/chromadb_collection.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+ChromaDB Collection
+"""
+
 import logging
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from chromadb.api.models.Collection import Collection as ChromaCollection
 from linkml_runtime.linkml_model import SlotDefinition
 
 from linkml_store.api import Collection
@@ -9,14 +13,17 @@
 from linkml_store.api.queries import Query, QueryResult
 from linkml_store.index import Indexer
 
 logger = logging.getLogger(__name__)
 
 
 class ChromaDBCollection(Collection):
+    """
+    A wrapper for ChromaDB collections.
+    """
 
     @property
     def native_collection(self) -> ChromaCollection:
         return self.parent.client.get_collection(self.name)
 
     def insert(self, objs: Union[OBJECT, List[OBJECT]], **kwargs):
         if not isinstance(objs, list):
@@ -46,15 +53,15 @@
         if not isinstance(objs, list):
             objs = [objs]
         ids = [obj["id"] for obj in objs]
         self.native_collection.delete(ids=ids)
         return len(ids)
 
     def delete_where(self, where: Optional[Dict[str, Any]] = None, missing_ok=True, **kwargs) -> int:
-        logger.info(f"Deleting from {self._target_class_name} where: {where}")
+        logger.info(f"Deleting from {self.target_class_name} where: {where}")
         if where is None:
             where = {}
         results = self.native_collection.get(where=where)
         ids = [result["id"] for result in results]
         self.native_collection.delete(ids=ids)
         return len(ids)
```

### Comparing `linkml_store-0.1.6/src/linkml_store/api/stores/chromadb/chromadb_database.py` & `linkml_store-0.1.7/src/linkml_store/api/stores/chromadb/chromadb_database.py`

 * *Files identical despite different names*

### Comparing `linkml_store-0.1.6/src/linkml_store/api/stores/duckdb/duckdb_collection.py` & `linkml_store-0.1.7/src/linkml_store/api/stores/duckdb/duckdb_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         if not objs:
             return
         cd = self.class_definition()
         if not cd:
             cd = self.induce_class_definition_from_objects(objs)
         self._create_table(cd)
         table = self._sqla_table(cd)
-        logger.info(f"Inserting into: {self._alias} // T={table.name}")
+        logger.info(f"Inserting into: {self.alias} // T={table.name}")
         engine = self.parent.engine
         col_names = [c.name for c in table.columns]
         objs = [{k: obj.get(k, None) for k in col_names} for obj in objs]
         with engine.connect() as conn:
             with conn.begin():
                 conn.execute(insert(table), objs)
             conn.commit()
@@ -51,20 +51,20 @@
                 stmt = delete(table).where(*conditions)
                 stmt = stmt.compile(engine)
                 conn.execute(stmt)
                 conn.commit()
         return len(objs)
 
     def delete_where(self, where: Optional[Dict[str, Any]] = None, missing_ok=True, **kwargs) -> int:
-        logger.info(f"Deleting from {self._target_class_name} where: {where}")
+        logger.info(f"Deleting from {self.target_class_name} where: {where}")
         if where is None:
             where = {}
         cd = self.class_definition()
         if not cd:
-            logger.info(f"No class definition found for {self._target_class_name}, assuming not prepopulated")
+            logger.info(f"No class definition found for {self.target_class_name}, assuming not prepopulated")
             return 0
         table = self._sqla_table(cd)
         engine = self.parent.engine
         inspector = inspect(engine)
         table_exists = table.name in inspector.get_table_names()
         if not table_exists:
             logger.info(f"Table {table.name} does not exist, assuming no data")
@@ -111,23 +111,23 @@
                 typ = sqla.JSON
             if att.multivalued:
                 typ = sqla.ARRAY(typ, dimensions=1)
             if att.array:
                 typ = sqla.ARRAY(typ, dimensions=1)
             col = Column(att.name, typ)
             cols.append(col)
-        t = Table(self._alias, metadata_obj, *cols)
+        t = Table(self.alias, metadata_obj, *cols)
         return t
 
     def _create_table(self, cd: ClassDefinition):
         if self._table_created or self.metadata.is_prepopulated:
             logger.info(f"Already have table for: {cd.name}")
             return
         query = Query(
-            from_table="information_schema.tables", where_clause={"table_type": "BASE TABLE", "table_name": self._alias}
+            from_table="information_schema.tables", where_clause={"table_type": "BASE TABLE", "table_name": self.alias}
         )
         qr = self.parent.query(query)
         if qr.num_rows > 0:
             logger.info(f"Table already exists for {cd.name}")
             self._table_created = True
             self.metadata.is_prepopulated = True
             return
```

### Comparing `linkml_store-0.1.6/src/linkml_store/api/stores/duckdb/duckdb_database.py` & `linkml_store-0.1.7/src/linkml_store/api/stores/duckdb/duckdb_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,20 +69,20 @@
                 if qr.num_rows == 0:
                     logger.debug(f"Table {query.from_table} not created yet")
                     return QueryResult(query=query, num_rows=0, rows=[])
             sv = self._schema_view
             if sv:
                 cd = None
                 for c in self._collections.values():
-                    if c.name == query.from_table:
+                    if c.name == query.from_table or c.metadata.alias == query.from_table:
                         cd = c.class_definition()
                         break
                 if cd:
-                    for att in cd.attributes.values():
-                        if att.inlined:
+                    for att in sv.class_induced_slots(cd.name):
+                        if att.inlined or att.inlined_as_list:
                             json_encoded_cols.append(att.name)
         with self.engine.connect() as conn:
             count_query_str = text(query_to_sql(query, count=True))
             num_rows = list(conn.execute(count_query_str))[0][0]
             logger.debug(f"num_rows: {num_rows}")
             query_str = query_to_sql(query, **kwargs)  # include offset, limit
             logger.debug(f"query_str: {query_str}")
```

### Comparing `linkml_store-0.1.6/src/linkml_store/api/stores/hdf5/hdf5_collection.py` & `linkml_store-0.1.7/src/linkml_store/api/stores/hdf5/hdf5_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             obj_id = str(obj["id"])
             if obj_id in self.hdf5_group:
                 del self.hdf5_group[obj_id]
                 count += 1
         return count
 
     def delete_where(self, where: Optional[Dict[str, Any]] = None, missing_ok=True, **kwargs) -> int:
-        logger.info(f"Deleting from {self._target_class_name} where: {where}")
+        logger.info(f"Deleting from {self.target_class_name} where: {where}")
         if where is None:
             where = {}
         results = self.query(Query(where_clause=where)).rows
         count = self.delete(results)
         return count
 
     def query(self, query: Query, **kwargs) -> QueryResult:
```

### Comparing `linkml_store-0.1.6/src/linkml_store/api/stores/hdf5/hdf5_database.py` & `linkml_store-0.1.7/src/linkml_store/api/stores/hdf5/hdf5_database.py`

 * *Files identical despite different names*

### Comparing `linkml_store-0.1.6/src/linkml_store/api/stores/mongodb/mongodb_collection.py` & `linkml_store-0.1.7/src/linkml_store/api/stores/mongodb/mongodb_collection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from copy import copy
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from linkml_runtime.linkml_model import SlotDefinition
 from pymongo.collection import Collection as MongoCollection
 
 from linkml_store.api import Collection
 from linkml_store.api.collection import DEFAULT_FACET_LIMIT, OBJECT
@@ -27,15 +28,20 @@
     def query(self, query: Query, **kwargs) -> QueryResult:
         mongo_filter = self._build_mongo_filter(query.where_clause)
         if query.limit:
             cursor = self.mongo_collection.find(mongo_filter).limit(query.limit)
         else:
             cursor = self.mongo_collection.find(mongo_filter)
 
-        rows = list(cursor)
+        def _as_row(row: dict):
+            row = copy(row)
+            del row["_id"]
+            return row
+
+        rows = [_as_row(row) for row in cursor]
         count = self.mongo_collection.count_documents(mongo_filter)
 
         return QueryResult(query=query, num_rows=count, rows=rows)
 
     def _build_mongo_filter(self, where_clause: Dict[str, Any]) -> Dict[str, Any]:
         mongo_filter = {}
         if where_clause:
@@ -88,15 +94,15 @@
             for key, value in obj.items():
                 filter_condition[key] = value
             filter_conditions.append(filter_condition)
         result = self.mongo_collection.delete_many({"$or": filter_conditions})
         return result.deleted_count
 
     def delete_where(self, where: Optional[Dict[str, Any]] = None, missing_ok=True, **kwargs) -> int:
-        logger.info(f"Deleting from {self._target_class_name} where: {where}")
+        logger.info(f"Deleting from {self.target_class_name} where: {where}")
         if where is None:
             where = {}
         result = self.mongo_collection.delete_many(where)
         deleted_rows_count = result.deleted_count
         if deleted_rows_count == 0 and not missing_ok:
             raise ValueError(f"No rows found for {where}")
         return deleted_rows_count
```

### Comparing `linkml_store-0.1.6/src/linkml_store/api/stores/mongodb/mongodb_database.py` & `linkml_store-0.1.7/src/linkml_store/api/stores/mongodb/mongodb_database.py`

 * *Files identical despite different names*

### Comparing `linkml_store-0.1.6/src/linkml_store/api/stores/solr/solr_collection.py` & `linkml_store-0.1.7/src/linkml_store/api/stores/solr/solr_collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # solr_collection.py
 
 import logging
 from copy import copy
 from typing import Any, Dict, List, Optional, Union
 
 import requests
+
 from linkml_store.api import Collection
 from linkml_store.api.collection import DEFAULT_FACET_LIMIT
 from linkml_store.api.queries import Query, QueryResult
 
 logger = logging.getLogger(__name__)
 
 
@@ -115,15 +116,15 @@
 
     def _build_solr_where_clause(self, where_clause: Dict) -> str:
         if where_clause is None:
             where_clause = {}
         conditions = []
         if self.parent.metadata.collection_type_slot:
             where_clause = copy(where_clause)
-            where_clause[self.parent.metadata.collection_type_slot] = self._alias
+            where_clause[self.parent.metadata.collection_type_slot] = self.alias
         for field, value in where_clause.items():
             if not isinstance(value, (list, tuple)):
                 value = [value]
             value = [f'"{v}"' if isinstance(v, str) else str(v) for v in value]
             if len(value) > 1:
                 conditions.append(f"{field}:({' '.join(value)})")
             else:
```

### Comparing `linkml_store-0.1.6/src/linkml_store/api/stores/solr/solr_database.py` & `linkml_store-0.1.7/src/linkml_store/api/stores/solr/solr_database.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 from typing import Optional
 
 import requests
+
 from linkml_store.api import Collection, Database
 from linkml_store.api.config import CollectionConfig
 from linkml_store.api.queries import Query, QueryResult
 from linkml_store.api.stores.solr.solr_collection import SolrCollection
 
 logger = logging.getLogger(__name__)
```

### Comparing `linkml_store-0.1.6/src/linkml_store/cli.py` & `linkml_store-0.1.7/src/linkml_store/cli.py`

 * *Files identical despite different names*

### Comparing `linkml_store-0.1.6/src/linkml_store/index/__init__.py` & `linkml_store-0.1.7/src/linkml_store/index/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml_store-0.1.6/src/linkml_store/index/implementations/llm_indexer.py` & `linkml_store-0.1.7/src/linkml_store/index/implementations/llm_indexer.py`

 * *Files identical despite different names*

### Comparing `linkml_store-0.1.6/src/linkml_store/index/implementations/simple_indexer.py` & `linkml_store-0.1.7/src/linkml_store/index/implementations/simple_indexer.py`

 * *Files identical despite different names*

### Comparing `linkml_store-0.1.6/src/linkml_store/index/indexer.py` & `linkml_store-0.1.7/src/linkml_store/index/indexer.py`

 * *Files identical despite different names*

### Comparing `linkml_store-0.1.6/src/linkml_store/utils/format_utils.py` & `linkml_store-0.1.7/src/linkml_store/utils/format_utils.py`

 * *Files identical despite different names*

### Comparing `linkml_store-0.1.6/src/linkml_store/utils/io.py` & `linkml_store-0.1.7/src/linkml_store/utils/io.py`

 * *Files identical despite different names*

### Comparing `linkml_store-0.1.6/src/linkml_store/utils/object_utils.py` & `linkml_store-0.1.7/src/linkml_store/utils/object_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from copy import deepcopy
-from typing import Any, Dict, Union
+from typing import Any, Dict, List, Union
 
 from pydantic import BaseModel
 
 
 def object_path_update(
     obj: Union[BaseModel, Dict[str, Any]], path: str, value: Any
 ) -> Union[BaseModel, Dict[str, Any]]:
@@ -67,7 +67,15 @@
     """
     try:
         path, val = expr.split("=", 1)
         val = json.loads(val)
     except ValueError:
         return None
     return path, val
+
+
+def clean_empties(value: Union[Dict, List]) -> Any:
+    if isinstance(value, dict):
+        value = {k: v for k, v in ((k, clean_empties(v)) for k, v in value.items()) if v is not None}
+    elif isinstance(value, list):
+        value = [v for v in (clean_empties(v) for v in value) if v is not None]
+    return value
```

### Comparing `linkml_store-0.1.6/src/linkml_store/utils/sql_utils.py` & `linkml_store-0.1.7/src/linkml_store/utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `linkml_store-0.1.6/PKG-INFO` & `linkml_store-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkml-store
-Version: 0.1.6
+Version: 0.1.7
 Summary: linkml-store
 License: MIT
 Author: Author 1
 Author-email: author@org.org
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

