# Comparing `tmp/pyesorm-0.4.1.tar.gz` & `tmp/pyesorm-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyesorm-0.4.1.tar", last modified: Tue May  7 11:44:39 2024, max compression
+gzip compressed data, was "pyesorm-0.4.2.tar", last modified: Tue May  7 15:07:03 2024, max compression
```

## Comparing `pyesorm-0.4.1.tar` & `pyesorm-0.4.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 11:44:39.747530 pyesorm-0.4.1/
--rw-r--r--   0 wallner    (501) staff       (20)    16725 2023-10-30 16:10:12.000000 pyesorm-0.4.1/LICENSE
--rw-r--r--   0 wallner    (501) staff       (20)    23956 2024-05-07 11:44:39.747168 pyesorm-0.4.1/PKG-INFO
--rw-r--r--   0 wallner    (501) staff       (20)    22319 2024-05-07 06:59:22.000000 pyesorm-0.4.1/README.md
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 11:44:39.725538 pyesorm-0.4.1/docs/
--rw-r--r--   0 wallner    (501) staff       (20)        0 2024-01-17 15:06:14.000000 pyesorm-0.4.1/docs/__init__.py
--rw-r--r--   0 wallner    (501) staff       (20)     1484 2024-01-17 15:18:18.000000 pyesorm-0.4.1/docs/changelog.py
--rw-r--r--   0 wallner    (501) staff       (20)     1462 2024-01-17 15:10:11.000000 pyesorm-0.4.1/docs/conf.py
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 11:44:39.735208 pyesorm-0.4.1/esorm/
--rw-r--r--   0 wallner    (501) staff       (20)      728 2024-05-07 10:10:02.000000 pyesorm-0.4.1/esorm/__init__.py
--rw-r--r--   0 wallner    (501) staff       (20)     3132 2024-01-22 17:32:29.000000 pyesorm-0.4.1/esorm/aggs.py
--rw-r--r--   0 wallner    (501) staff       (20)     4447 2024-05-07 05:08:54.000000 pyesorm-0.4.1/esorm/bulk.py
--rw-r--r--   0 wallner    (501) staff       (20)     1267 2024-05-07 05:07:07.000000 pyesorm-0.4.1/esorm/error.py
--rw-r--r--   0 wallner    (501) staff       (20)     1943 2023-10-31 19:12:30.000000 pyesorm-0.4.1/esorm/esorm.py
--rw-r--r--   0 wallner    (501) staff       (20)     3500 2024-01-24 09:39:22.000000 pyesorm-0.4.1/esorm/fastapi.py
--rw-r--r--   0 wallner    (501) staff       (20)    11640 2023-10-31 19:12:30.000000 pyesorm-0.4.1/esorm/fields.py
--rw-r--r--   0 wallner    (501) staff       (20)       52 2023-10-30 16:10:12.000000 pyesorm-0.4.1/esorm/logger.py
--rw-r--r--   0 wallner    (501) staff       (20)    41741 2024-05-07 11:35:34.000000 pyesorm-0.4.1/esorm/model.py
--rw-r--r--   0 wallner    (501) staff       (20)     9605 2024-01-18 19:16:18.000000 pyesorm-0.4.1/esorm/query.py
--rw-r--r--   0 wallner    (501) staff       (20)     1315 2024-01-18 19:06:35.000000 pyesorm-0.4.1/esorm/response.py
--rw-r--r--   0 wallner    (501) staff       (20)      996 2024-01-23 07:15:23.000000 pyesorm-0.4.1/esorm/utils.py
--rw-r--r--   0 wallner    (501) staff       (20)     5538 2023-10-30 16:10:12.000000 pyesorm-0.4.1/esorm/watcher.py
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 11:44:39.743040 pyesorm-0.4.1/pyesorm.egg-info/
--rw-r--r--   0 wallner    (501) staff       (20)    23956 2024-05-07 11:44:39.000000 pyesorm-0.4.1/pyesorm.egg-info/PKG-INFO
--rw-r--r--   0 wallner    (501) staff       (20)      514 2024-05-07 11:44:39.000000 pyesorm-0.4.1/pyesorm.egg-info/SOURCES.txt
--rw-r--r--   0 wallner    (501) staff       (20)        1 2024-05-07 11:44:39.000000 pyesorm-0.4.1/pyesorm.egg-info/dependency_links.txt
--rw-r--r--   0 wallner    (501) staff       (20)      272 2024-05-07 11:44:39.000000 pyesorm-0.4.1/pyesorm.egg-info/requires.txt
--rw-r--r--   0 wallner    (501) staff       (20)       17 2024-05-07 11:44:39.000000 pyesorm-0.4.1/pyesorm.egg-info/top_level.txt
--rw-r--r--   0 wallner    (501) staff       (20)       87 2023-10-31 20:33:56.000000 pyesorm-0.4.1/pyproject.toml
--rw-r--r--   0 wallner    (501) staff       (20)     1306 2024-05-07 11:44:39.748289 pyesorm-0.4.1/setup.cfg
--rw-r--r--   0 wallner    (501) staff       (20)       37 2023-10-30 16:10:12.000000 pyesorm-0.4.1/setup.py
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 11:44:39.740726 pyesorm-0.4.1/tests/
--rw-r--r--   0 wallner    (501) staff       (20)        0 2023-10-30 16:10:12.000000 pyesorm-0.4.1/tests/__init__.py
--rw-r--r--   0 wallner    (501) staff       (20)     7056 2024-05-03 18:47:40.000000 pyesorm-0.4.1/tests/conftest.py
--rw-r--r--   0 wallner    (501) staff       (20)    29087 2024-05-07 11:05:38.000000 pyesorm-0.4.1/tests/test_esorm.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 15:07:03.422381 pyesorm-0.4.2/
+-rw-r--r--   0 wallner    (501) staff       (20)    16725 2023-10-30 16:10:12.000000 pyesorm-0.4.2/LICENSE
+-rw-r--r--   0 wallner    (501) staff       (20)    23956 2024-05-07 15:07:03.422093 pyesorm-0.4.2/PKG-INFO
+-rw-r--r--   0 wallner    (501) staff       (20)    22319 2024-05-07 06:59:22.000000 pyesorm-0.4.2/README.md
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 15:07:03.405659 pyesorm-0.4.2/docs/
+-rw-r--r--   0 wallner    (501) staff       (20)        0 2024-01-17 15:06:14.000000 pyesorm-0.4.2/docs/__init__.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1484 2024-01-17 15:18:18.000000 pyesorm-0.4.2/docs/changelog.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1462 2024-01-17 15:10:11.000000 pyesorm-0.4.2/docs/conf.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 15:07:03.415391 pyesorm-0.4.2/esorm/
+-rw-r--r--   0 wallner    (501) staff       (20)      728 2024-05-07 10:10:02.000000 pyesorm-0.4.2/esorm/__init__.py
+-rw-r--r--   0 wallner    (501) staff       (20)     3132 2024-01-22 17:32:29.000000 pyesorm-0.4.2/esorm/aggs.py
+-rw-r--r--   0 wallner    (501) staff       (20)     4447 2024-05-07 05:08:54.000000 pyesorm-0.4.2/esorm/bulk.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1267 2024-05-07 05:07:07.000000 pyesorm-0.4.2/esorm/error.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1943 2023-10-31 19:12:30.000000 pyesorm-0.4.2/esorm/esorm.py
+-rw-r--r--   0 wallner    (501) staff       (20)     3500 2024-01-24 09:39:22.000000 pyesorm-0.4.2/esorm/fastapi.py
+-rw-r--r--   0 wallner    (501) staff       (20)    11640 2023-10-31 19:12:30.000000 pyesorm-0.4.2/esorm/fields.py
+-rw-r--r--   0 wallner    (501) staff       (20)       52 2023-10-30 16:10:12.000000 pyesorm-0.4.2/esorm/logger.py
+-rw-r--r--   0 wallner    (501) staff       (20)    41748 2024-05-07 14:34:50.000000 pyesorm-0.4.2/esorm/model.py
+-rw-r--r--   0 wallner    (501) staff       (20)     9605 2024-01-18 19:16:18.000000 pyesorm-0.4.2/esorm/query.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1315 2024-01-18 19:06:35.000000 pyesorm-0.4.2/esorm/response.py
+-rw-r--r--   0 wallner    (501) staff       (20)      996 2024-01-23 07:15:23.000000 pyesorm-0.4.2/esorm/utils.py
+-rw-r--r--   0 wallner    (501) staff       (20)     5538 2023-10-30 16:10:12.000000 pyesorm-0.4.2/esorm/watcher.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 15:07:03.419878 pyesorm-0.4.2/pyesorm.egg-info/
+-rw-r--r--   0 wallner    (501) staff       (20)    23956 2024-05-07 15:07:03.000000 pyesorm-0.4.2/pyesorm.egg-info/PKG-INFO
+-rw-r--r--   0 wallner    (501) staff       (20)      514 2024-05-07 15:07:03.000000 pyesorm-0.4.2/pyesorm.egg-info/SOURCES.txt
+-rw-r--r--   0 wallner    (501) staff       (20)        1 2024-05-07 15:07:03.000000 pyesorm-0.4.2/pyesorm.egg-info/dependency_links.txt
+-rw-r--r--   0 wallner    (501) staff       (20)      272 2024-05-07 15:07:03.000000 pyesorm-0.4.2/pyesorm.egg-info/requires.txt
+-rw-r--r--   0 wallner    (501) staff       (20)       17 2024-05-07 15:07:03.000000 pyesorm-0.4.2/pyesorm.egg-info/top_level.txt
+-rw-r--r--   0 wallner    (501) staff       (20)       87 2023-10-31 20:33:56.000000 pyesorm-0.4.2/pyproject.toml
+-rw-r--r--   0 wallner    (501) staff       (20)     1306 2024-05-07 15:07:03.423168 pyesorm-0.4.2/setup.cfg
+-rw-r--r--   0 wallner    (501) staff       (20)       37 2023-10-30 16:10:12.000000 pyesorm-0.4.2/setup.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 15:07:03.418722 pyesorm-0.4.2/tests/
+-rw-r--r--   0 wallner    (501) staff       (20)        0 2023-10-30 16:10:12.000000 pyesorm-0.4.2/tests/__init__.py
+-rw-r--r--   0 wallner    (501) staff       (20)     7758 2024-05-07 14:38:00.000000 pyesorm-0.4.2/tests/conftest.py
+-rw-r--r--   0 wallner    (501) staff       (20)    31583 2024-05-07 14:58:58.000000 pyesorm-0.4.2/tests/test_esorm.py
```

### Comparing `pyesorm-0.4.1/LICENSE` & `pyesorm-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.1/PKG-INFO` & `pyesorm-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyesorm
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python ElasticSearch ORM based on Pydantic
 Home-page: https://github.com/wallneradam/esorm
 Author: Adam Wallner
 Author-email: Adam.wallner@gmail.com
 License: MPL-2.0
 Project-URL: Bug Tracker, https://github.com/wallneradam/esorm/issues
 Project-URL: Documentation, https://esorm.readthedocs.io/en/latest/
```

### Comparing `pyesorm-0.4.1/README.md` & `pyesorm-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.1/docs/changelog.py` & `pyesorm-0.4.2/docs/changelog.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.1/docs/conf.py` & `pyesorm-0.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.1/esorm/__init__.py` & `pyesorm-0.4.2/esorm/__init__.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.1/esorm/aggs.py` & `pyesorm-0.4.2/esorm/aggs.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.1/esorm/bulk.py` & `pyesorm-0.4.2/esorm/bulk.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.1/esorm/error.py` & `pyesorm-0.4.2/esorm/error.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.1/esorm/esorm.py` & `pyesorm-0.4.2/esorm/esorm.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.1/esorm/fastapi.py` & `pyesorm-0.4.2/esorm/fastapi.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.1/esorm/fields.py` & `pyesorm-0.4.2/esorm/fields.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.1/esorm/model.py` & `pyesorm-0.4.2/esorm/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,15 +254,15 @@
 
 class ESModel(ESBaseModel):
     """
     ElasticSearch Base Model
     """
 
     _id: Optional[str] = PrivateAttr(None)
-    """ The ES id of the document """
+    """ The ES id of the document (it is always a string) """
 
     _routing: Optional[str] = PrivateAttr(None)
     """ The routing of the document """
 
     _version: Optional[int] = PrivateAttr(None)
     """ The version of the document """
 
@@ -470,15 +470,15 @@
         If no id is provided, then document will be indexed and elasticsearch will generate a suitable id that will be
         populated on the returned model.
 
         :param wait_for: Waits for all shards to sync before returning response - useful when writing
                          tests. Defaults to False.
         :param pipeline: Pipeline to use for indexing
         :param routing: Shard routing value
-        :return: The new document's ID
+        :return: The new document's ID, it is always a string, even if the id field is an integer
         """
         kwargs = dict(
             document=self.to_es(),
             wait_for=wait_for,
         )
 
         kwargs['id'] = self.__id__
@@ -515,19 +515,15 @@
         Fetches document and returns ESModel instance populated with properties.
 
         :param id: Document id
         :param routing: Shard routing value
         :raises esorm.error.NotFoundError: Returned if document not found
         :return: ESModel object
         """
-        kwargs = dict(id=str(id))
-        if routing:
-            kwargs['routing'] = routing
-        else:
-            kwargs['routing'] = cls.__routing__
+        kwargs = {'id': id, 'routing': routing if routing else cls.__routing__}
         try:
             es_res = await cls.call('get', **kwargs)
             return await _lazy_process_results(cls.from_es(es_res))
         except ElasticNotFoundError:
             raise NotFoundError(f"Document with id {id} not found")
 
     async def delete(self, *, wait_for=False, routing: Optional[str] = None):
```

### Comparing `pyesorm-0.4.1/esorm/query.py` & `pyesorm-0.4.2/esorm/query.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.1/esorm/response.py` & `pyesorm-0.4.2/esorm/response.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.1/esorm/utils.py` & `pyesorm-0.4.2/esorm/utils.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.1/esorm/watcher.py` & `pyesorm-0.4.2/esorm/watcher.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.1/pyesorm.egg-info/PKG-INFO` & `pyesorm-0.4.2/pyesorm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyesorm
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python ElasticSearch ORM based on Pydantic
 Home-page: https://github.com/wallneradam/esorm
 Author: Adam Wallner
 Author-email: Adam.wallner@gmail.com
 License: MPL-2.0
 Project-URL: Bug Tracker, https://github.com/wallneradam/esorm/issues
 Project-URL: Documentation, https://esorm.readthedocs.io/en/latest/
```

### Comparing `pyesorm-0.4.1/pyesorm.egg-info/SOURCES.txt` & `pyesorm-0.4.2/pyesorm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.1/setup.cfg` & `pyesorm-0.4.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyesorm
-version = 0.4.1
+version = 0.4.2
 author = Adam Wallner
 author_email = Adam.wallner@gmail.com
 description = Python ElasticSearch ORM based on Pydantic
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = ElasticSearch, ORM, Pydantic
 license = MPL-2.0
```

### Comparing `pyesorm-0.4.1/tests/conftest.py` & `pyesorm-0.4.2/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -211,14 +211,53 @@
     yield IdModel
 
     del IdModel
 
 
 # noinspection PyUnresolvedReferences
 @pytest.fixture(scope="class")
+def model_with_int_id(esorm):
+    """
+    Model to test int id field
+    """
+
+    class IntIdModel(esorm.ESModel):
+        class ESConfig:
+            id_field = 'custom_id'
+
+        custom_id: int
+        f_str: str
+
+    yield IntIdModel
+
+    del IntIdModel
+
+
+# noinspection PyUnresolvedReferences
+@pytest.fixture(scope="class")
+def model_with_prop_id(esorm):
+    """
+    Model to test property id field
+    """
+
+    class PropIdModel(esorm.ESModel):
+        @property
+        def __id__(self) -> int:
+            return self.custom_id + 1000
+
+        custom_id: int
+        f_str: str
+
+    yield PropIdModel
+
+    del PropIdModel
+
+
+# noinspection PyUnresolvedReferences
+@pytest.fixture(scope="class")
 def model_nested(esorm, model_timestamp):
     """
     Model to test nested fields
     """
 
     class NestedFieldModel(esorm.ESModel):
         f_nested: model_timestamp
```

### Comparing `pyesorm-0.4.1/tests/test_esorm.py` & `pyesorm-0.4.2/tests/test_esorm.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,24 +75,40 @@
         """
         Test model with config
         """
         assert model_with_id is not None
         assert model_with_id.ESConfig.index == 'esorm-id_model'
         assert model_with_id.ESConfig.id_field == 'id'
 
+    async def test_create_model_with_int_id(self, es, esorm, model_with_int_id):
+        """
+        Test model with int id
+        """
+        assert model_with_int_id is not None
+        assert model_with_int_id.ESConfig.index == 'esorm-int_id_model'
+        assert model_with_int_id.ESConfig.id_field == 'custom_id'
+
+    async def test_create_model_with_prop_id(self, es, esorm, model_with_prop_id):
+        """
+        Test model with property id
+        """
+        assert model_with_prop_id is not None
+        assert model_with_prop_id.ESConfig.index == 'esorm-prop_id_model'
+        assert model_with_prop_id.ESConfig.id_field is None
+
     async def test_create_nested_model(self, es, esorm, model_nested):
         """
         Test nested model
         """
         assert model_nested is not None
         assert model_nested.ESConfig.index == 'esorm-nested_field_model'
 
     async def test_create_mappings(self, es, esorm, model_python, model_es, model_es_optional,
-                                   model_timestamp, model_config, model_with_id, model_nested,
-                                   model_lazy_prop):
+                                   model_timestamp, model_config, model_with_id, model_with_int_id,
+                                   model_with_prop_id, model_nested, model_lazy_prop):
         """
         Test create mappings
         """
         await esorm.setup_mappings()
         # Check if index exists
         assert await es.indices.exists(index=model_python.ESConfig.index)
 
@@ -151,14 +167,26 @@
 
         # Check if mappings are correct for model with id
         mappings = await es.indices.get_mapping(index=model_with_id.ESConfig.index)
         assert mappings[model_with_id.ESConfig.index]['mappings']['properties']['f_str']['type'] == 'keyword'
         assert 'id' not in mappings[model_with_id.ESConfig.index]['mappings']['properties'], \
             "Id fields should not be in mappings"
 
+        # Check if mappings are correct for model with int id
+        mappings = await es.indices.get_mapping(index=model_with_int_id.ESConfig.index)
+        assert mappings[model_with_int_id.ESConfig.index]['mappings']['properties']['f_str']['type'] == 'keyword'
+        assert 'custom_id' not in mappings[model_with_int_id.ESConfig.index]['mappings']['properties'], \
+            "Id fields should not be in mappings"
+
+        # Check if mappings are correct for model with prop id
+        mappings = await es.indices.get_mapping(index=model_with_prop_id.ESConfig.index)
+        assert mappings[model_with_prop_id.ESConfig.index]['mappings']['properties']['f_str']['type'] == 'keyword'
+        # It is used in the id, but remains in the db
+        assert mappings[model_with_prop_id.ESConfig.index]['mappings']['properties']['custom_id']['type'] == 'long'
+
         # Check if mappings are correct for nested model
         mappings = await es.indices.get_mapping(index=model_nested.ESConfig.index)
         assert 'properties' in mappings[model_nested.ESConfig.index]['mappings']['properties']['f_nested'], \
             "Nested field should have properties"
         assert 'created_at' in mappings[model_nested.ESConfig.index]['mappings']['properties']['f_nested'][
             'properties']
         assert 'modified_at' in mappings[model_nested.ESConfig.index]['mappings']['properties']['f_nested'][
@@ -198,14 +226,44 @@
         assert doc.f_nested.f_str == "nested_test"
 
         # Check private fields
         assert doc._version == 1
         assert doc._primary_term == 1
         assert doc._seq_no == 0
 
+    async def test_crud_get_by_int_id(self, es, esorm, model_with_int_id):
+        """
+        Test get by int id
+        """
+        # Create a document
+        doc_id = await model_with_int_id(custom_id=1, f_str="int_id_test").save()
+        assert doc_id == "1"
+
+        # Get by id
+        doc = await model_with_int_id.get(1)
+        assert doc is not None
+        assert doc.custom_id == 1
+        assert doc.f_str == "int_id_test"
+        assert doc._id == "1"
+
+    async def test_crud_get_by_prop_id(self, es, esorm, model_with_prop_id):
+        """
+        Test get by prop id
+        """
+        # Create a document
+        doc_id = await model_with_prop_id(custom_id=1, f_str="prop_id_test").save()
+        assert doc_id == "1001"
+
+        # Get by id
+        doc = await model_with_prop_id.get(1001)
+        assert doc is not None
+        assert doc.custom_id == 1
+        assert doc.f_str == "prop_id_test"
+        assert doc._id == "1001"
+
     async def test_crud_update(self, es, esorm, model_nested):
         """
         Test update
         """
         doc_id = self.__class__.doc_id
         # Update
         doc = await model_nested.get(doc_id)
```

