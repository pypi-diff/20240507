# Comparing `tmp/pyesorm-0.4.0.tar.gz` & `tmp/pyesorm-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyesorm-0.4.0.tar", last modified: Tue May  7 08:45:02 2024, max compression
+gzip compressed data, was "pyesorm-0.4.1.tar", last modified: Tue May  7 11:44:39 2024, max compression
```

## Comparing `pyesorm-0.4.0.tar` & `pyesorm-0.4.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 08:45:02.773973 pyesorm-0.4.0/
--rw-r--r--   0 wallner    (501) staff       (20)    16725 2023-10-30 16:10:12.000000 pyesorm-0.4.0/LICENSE
--rw-r--r--   0 wallner    (501) staff       (20)    23956 2024-05-07 08:45:02.773765 pyesorm-0.4.0/PKG-INFO
--rw-r--r--   0 wallner    (501) staff       (20)    22319 2024-05-07 06:59:22.000000 pyesorm-0.4.0/README.md
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 08:45:02.759979 pyesorm-0.4.0/docs/
--rw-r--r--   0 wallner    (501) staff       (20)        0 2024-01-17 15:06:14.000000 pyesorm-0.4.0/docs/__init__.py
--rw-r--r--   0 wallner    (501) staff       (20)     1484 2024-01-17 15:18:18.000000 pyesorm-0.4.0/docs/changelog.py
--rw-r--r--   0 wallner    (501) staff       (20)     1462 2024-01-17 15:10:11.000000 pyesorm-0.4.0/docs/conf.py
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 08:45:02.767406 pyesorm-0.4.0/esorm/
--rw-r--r--   0 wallner    (501) staff       (20)      666 2024-04-29 11:40:09.000000 pyesorm-0.4.0/esorm/__init__.py
--rw-r--r--   0 wallner    (501) staff       (20)     3132 2024-01-22 17:32:29.000000 pyesorm-0.4.0/esorm/aggs.py
--rw-r--r--   0 wallner    (501) staff       (20)     4447 2024-05-07 05:08:54.000000 pyesorm-0.4.0/esorm/bulk.py
--rw-r--r--   0 wallner    (501) staff       (20)     1267 2024-05-07 05:07:07.000000 pyesorm-0.4.0/esorm/error.py
--rw-r--r--   0 wallner    (501) staff       (20)     1943 2023-10-31 19:12:30.000000 pyesorm-0.4.0/esorm/esorm.py
--rw-r--r--   0 wallner    (501) staff       (20)     3500 2024-01-24 09:39:22.000000 pyesorm-0.4.0/esorm/fastapi.py
--rw-r--r--   0 wallner    (501) staff       (20)    11640 2023-10-31 19:12:30.000000 pyesorm-0.4.0/esorm/fields.py
--rw-r--r--   0 wallner    (501) staff       (20)       52 2023-10-30 16:10:12.000000 pyesorm-0.4.0/esorm/logger.py
--rw-r--r--   0 wallner    (501) staff       (20)    41802 2024-05-07 05:46:54.000000 pyesorm-0.4.0/esorm/model.py
--rw-r--r--   0 wallner    (501) staff       (20)     9605 2024-01-18 19:16:18.000000 pyesorm-0.4.0/esorm/query.py
--rw-r--r--   0 wallner    (501) staff       (20)     1315 2024-01-18 19:06:35.000000 pyesorm-0.4.0/esorm/response.py
--rw-r--r--   0 wallner    (501) staff       (20)      996 2024-01-23 07:15:23.000000 pyesorm-0.4.0/esorm/utils.py
--rw-r--r--   0 wallner    (501) staff       (20)     5538 2023-10-30 16:10:12.000000 pyesorm-0.4.0/esorm/watcher.py
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 08:45:02.771621 pyesorm-0.4.0/pyesorm.egg-info/
--rw-r--r--   0 wallner    (501) staff       (20)    23956 2024-05-07 08:45:02.000000 pyesorm-0.4.0/pyesorm.egg-info/PKG-INFO
--rw-r--r--   0 wallner    (501) staff       (20)      514 2024-05-07 08:45:02.000000 pyesorm-0.4.0/pyesorm.egg-info/SOURCES.txt
--rw-r--r--   0 wallner    (501) staff       (20)        1 2024-05-07 08:45:02.000000 pyesorm-0.4.0/pyesorm.egg-info/dependency_links.txt
--rw-r--r--   0 wallner    (501) staff       (20)      272 2024-05-07 08:45:02.000000 pyesorm-0.4.0/pyesorm.egg-info/requires.txt
--rw-r--r--   0 wallner    (501) staff       (20)       17 2024-05-07 08:45:02.000000 pyesorm-0.4.0/pyesorm.egg-info/top_level.txt
--rw-r--r--   0 wallner    (501) staff       (20)       87 2023-10-31 20:33:56.000000 pyesorm-0.4.0/pyproject.toml
--rw-r--r--   0 wallner    (501) staff       (20)     1306 2024-05-07 08:45:02.774615 pyesorm-0.4.0/setup.cfg
--rw-r--r--   0 wallner    (501) staff       (20)       37 2023-10-30 16:10:12.000000 pyesorm-0.4.0/setup.py
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 08:45:02.770544 pyesorm-0.4.0/tests/
--rw-r--r--   0 wallner    (501) staff       (20)        0 2023-10-30 16:10:12.000000 pyesorm-0.4.0/tests/__init__.py
--rw-r--r--   0 wallner    (501) staff       (20)     7056 2024-05-03 18:47:40.000000 pyesorm-0.4.0/tests/conftest.py
--rw-r--r--   0 wallner    (501) staff       (20)    27877 2024-05-07 06:56:41.000000 pyesorm-0.4.0/tests/test_esorm.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 11:44:39.747530 pyesorm-0.4.1/
+-rw-r--r--   0 wallner    (501) staff       (20)    16725 2023-10-30 16:10:12.000000 pyesorm-0.4.1/LICENSE
+-rw-r--r--   0 wallner    (501) staff       (20)    23956 2024-05-07 11:44:39.747168 pyesorm-0.4.1/PKG-INFO
+-rw-r--r--   0 wallner    (501) staff       (20)    22319 2024-05-07 06:59:22.000000 pyesorm-0.4.1/README.md
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 11:44:39.725538 pyesorm-0.4.1/docs/
+-rw-r--r--   0 wallner    (501) staff       (20)        0 2024-01-17 15:06:14.000000 pyesorm-0.4.1/docs/__init__.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1484 2024-01-17 15:18:18.000000 pyesorm-0.4.1/docs/changelog.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1462 2024-01-17 15:10:11.000000 pyesorm-0.4.1/docs/conf.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 11:44:39.735208 pyesorm-0.4.1/esorm/
+-rw-r--r--   0 wallner    (501) staff       (20)      728 2024-05-07 10:10:02.000000 pyesorm-0.4.1/esorm/__init__.py
+-rw-r--r--   0 wallner    (501) staff       (20)     3132 2024-01-22 17:32:29.000000 pyesorm-0.4.1/esorm/aggs.py
+-rw-r--r--   0 wallner    (501) staff       (20)     4447 2024-05-07 05:08:54.000000 pyesorm-0.4.1/esorm/bulk.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1267 2024-05-07 05:07:07.000000 pyesorm-0.4.1/esorm/error.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1943 2023-10-31 19:12:30.000000 pyesorm-0.4.1/esorm/esorm.py
+-rw-r--r--   0 wallner    (501) staff       (20)     3500 2024-01-24 09:39:22.000000 pyesorm-0.4.1/esorm/fastapi.py
+-rw-r--r--   0 wallner    (501) staff       (20)    11640 2023-10-31 19:12:30.000000 pyesorm-0.4.1/esorm/fields.py
+-rw-r--r--   0 wallner    (501) staff       (20)       52 2023-10-30 16:10:12.000000 pyesorm-0.4.1/esorm/logger.py
+-rw-r--r--   0 wallner    (501) staff       (20)    41741 2024-05-07 11:35:34.000000 pyesorm-0.4.1/esorm/model.py
+-rw-r--r--   0 wallner    (501) staff       (20)     9605 2024-01-18 19:16:18.000000 pyesorm-0.4.1/esorm/query.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1315 2024-01-18 19:06:35.000000 pyesorm-0.4.1/esorm/response.py
+-rw-r--r--   0 wallner    (501) staff       (20)      996 2024-01-23 07:15:23.000000 pyesorm-0.4.1/esorm/utils.py
+-rw-r--r--   0 wallner    (501) staff       (20)     5538 2023-10-30 16:10:12.000000 pyesorm-0.4.1/esorm/watcher.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 11:44:39.743040 pyesorm-0.4.1/pyesorm.egg-info/
+-rw-r--r--   0 wallner    (501) staff       (20)    23956 2024-05-07 11:44:39.000000 pyesorm-0.4.1/pyesorm.egg-info/PKG-INFO
+-rw-r--r--   0 wallner    (501) staff       (20)      514 2024-05-07 11:44:39.000000 pyesorm-0.4.1/pyesorm.egg-info/SOURCES.txt
+-rw-r--r--   0 wallner    (501) staff       (20)        1 2024-05-07 11:44:39.000000 pyesorm-0.4.1/pyesorm.egg-info/dependency_links.txt
+-rw-r--r--   0 wallner    (501) staff       (20)      272 2024-05-07 11:44:39.000000 pyesorm-0.4.1/pyesorm.egg-info/requires.txt
+-rw-r--r--   0 wallner    (501) staff       (20)       17 2024-05-07 11:44:39.000000 pyesorm-0.4.1/pyesorm.egg-info/top_level.txt
+-rw-r--r--   0 wallner    (501) staff       (20)       87 2023-10-31 20:33:56.000000 pyesorm-0.4.1/pyproject.toml
+-rw-r--r--   0 wallner    (501) staff       (20)     1306 2024-05-07 11:44:39.748289 pyesorm-0.4.1/setup.cfg
+-rw-r--r--   0 wallner    (501) staff       (20)       37 2023-10-30 16:10:12.000000 pyesorm-0.4.1/setup.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 11:44:39.740726 pyesorm-0.4.1/tests/
+-rw-r--r--   0 wallner    (501) staff       (20)        0 2023-10-30 16:10:12.000000 pyesorm-0.4.1/tests/__init__.py
+-rw-r--r--   0 wallner    (501) staff       (20)     7056 2024-05-03 18:47:40.000000 pyesorm-0.4.1/tests/conftest.py
+-rw-r--r--   0 wallner    (501) staff       (20)    29087 2024-05-07 11:05:38.000000 pyesorm-0.4.1/tests/test_esorm.py
```

### Comparing `pyesorm-0.4.0/LICENSE` & `pyesorm-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.0/PKG-INFO` & `pyesorm-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyesorm
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python ElasticSearch ORM based on Pydantic
 Home-page: https://github.com/wallneradam/esorm
 Author: Adam Wallner
 Author-email: Adam.wallner@gmail.com
 License: MPL-2.0
 Project-URL: Bug Tracker, https://github.com/wallneradam/esorm/issues
 Project-URL: Documentation, https://esorm.readthedocs.io/en/latest/
```

### Comparing `pyesorm-0.4.0/README.md` & `pyesorm-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.0/docs/changelog.py` & `pyesorm-0.4.1/docs/changelog.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.0/docs/conf.py` & `pyesorm-0.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.0/esorm/__init__.py` & `pyesorm-0.4.1/esorm/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 """
 
 from .error import (
     InvalidResponseError,
     InvalidModelError,
     NotFoundError,
 )
-from .model import TModel, ESBaseModel, ESModel, ESModelTimestamp, Pagination, Sort, setup_mappings, lazy_property
+from .model import (TModel, ESBaseModel, ESModel, ESModelTimestamp, Pagination, Sort, setup_mappings,
+                    lazy_property, retry_on_conflict)
 from .esorm import es, connect
 from .fields import Field
 from .bulk import ESBulk
 from . import fields
 
 __all__ = [
     "TModel", "ESBaseModel", "ESModel", "ESModelTimestamp", "ESBulk",
-    'lazy_property',
+    'lazy_property', 'retry_on_conflict',
     "es",
     "NotFoundError",
     "InvalidModelError",
     "InvalidResponseError",
     "connect",
     "setup_mappings",
     "Field",
```

### Comparing `pyesorm-0.4.0/esorm/aggs.py` & `pyesorm-0.4.1/esorm/aggs.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.0/esorm/bulk.py` & `pyesorm-0.4.1/esorm/bulk.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.0/esorm/error.py` & `pyesorm-0.4.1/esorm/error.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.0/esorm/esorm.py` & `pyesorm-0.4.1/esorm/esorm.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.0/esorm/fastapi.py` & `pyesorm-0.4.1/esorm/fastapi.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.0/esorm/fields.py` & `pyesorm-0.4.1/esorm/fields.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.0/esorm/model.py` & `pyesorm-0.4.1/esorm/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import textwrap
 import traceback
 from contextvars import ContextVar
 from datetime import datetime, date, time
 from functools import wraps
 
 import elasticsearch
-from elasticsearch import NotFoundError as ElasticNotFoundError
+from elasticsearch import NotFoundError as ElasticNotFoundError, ConflictError as ElasticConflictError
 from pydantic import main as pydantic_main
 from pydantic import BaseModel, ConfigDict
 from pydantic.fields import Field, PrivateAttr
 # noinspection PyProtectedMember
 from pydantic.fields import FieldInfo  # It is just not in __all__ of pydantic.fields, but we strongly need it
 
 from .utils import snake_case, utcnow
@@ -38,15 +38,16 @@
     'ESModel',
     'ESModelTimestamp',
     'Pagination', 'Sort',
     'setup_mappings',
     'create_index_template',
     'set_default_index_prefix',
     'set_max_lazy_property_concurrency',
-    'lazy_property'
+    'lazy_property',
+    'retry_on_conflict'
 ]
 
 #
 # Global variables and types
 #
 
 # noinspection PyProtectedMember
@@ -754,72 +755,39 @@
 class ESModelTimestamp(ESModel):
     """
     Model which stores `created_at` and `modified_at` fields automatcally.
     """
     created_at: Optional[datetime] = Field(None, description="Creation date and time")
     modified_at: Optional[datetime] = Field(default_factory=utcnow, description="Modification date and time")
 
-    async def save(self, *, force_new=False, wait_for=False, pipeline: Optional[str] = None,
+    async def save(self, *, wait_for=False, force_new=False, pipeline: Optional[str] = None,
                    routing: Optional[str] = None) -> str:
         """
         Save document into elasticsearch.
 
         If document already exists, existing document will be updated as per native elasticsearch index operation.
         If model has id (Meta.id_field or __id__), this will be used as the elasticsearch _id. The id field will be
         removed from the document before indexing.
         If no id is provided, then document will be indexed and elasticsearch will generate a suitable id that will be
         populated on the returned model.
 
-        :param force_new: Force creation of new document, it is assumed that document does not exist in elasticsearch
         :param wait_for: Waits for all shards to sync before returning response - useful when writing
             tests. Defaults to False.
+        :param force_new: It is assumed to be a new document, so created_at will be set to current time
+                          (it is no more necessary, because created_at is set to current time if it is None.
+                          It is here for backward compatibility)
         :param pipeline: Pipeline to use for indexing
         :param routing: Shard routing value
         :return: The new document's ID
         """
-        # If we know that the document is new, we can call the original save method
-        if force_new:
+        self.modified_at = utcnow()
+        # Set created_at if not already set
+        if force_new or not self.created_at:
             self.created_at = self.modified_at
-            return await super().save(wait_for=wait_for, pipeline=pipeline, routing=routing)
-
-        # We use update method with upsert here to make created_at set only on creation
-        doc_upsert = self.to_es()
-        doc = dict(doc_upsert)
-        del doc['created_at']
-
-        # Default created_at will be the same as modified_at
-        if not doc_upsert['created_at']:
-            doc_upsert['created_at'] = doc_upsert['modified_at']
-
-        kwargs = dict(
-            doc=doc,  # It is really doc, not document as in index :-/
-            wait_for=wait_for,
-            upsert=doc_upsert
-        )
-
-        if pipeline is not None:
-            kwargs['pipeline'] = pipeline
-
-        if routing is not None:
-            kwargs['routing'] = routing
-
-        if self._primary_term is not None:
-            kwargs['if_primary_term'] = self._primary_term
-        if self._seq_no is not None:
-            kwargs['if_seq_no'] = self._seq_no
-
-        # Set id field
-        kwargs['id'] = self.__id__
-        # Remove the id field from the document
-        if self.ESConfig.id_field:
-            del doc[self.ESConfig.id_field]
-            del doc_upsert[self.ESConfig.id_field]
-
-        es_res = await self.call('update', **kwargs)
-        return es_res.get('_id')
+        return await super().save(wait_for=wait_for, pipeline=pipeline, routing=routing)
 
 
 #
 # Lazy properties
 #
 
 def set_max_lazy_property_concurrency(concurrency: int):
@@ -909,14 +877,46 @@
     # Set the original function as __lazy_property_func__
     setattr(wrapper, '__lazy_property__', async_wrapper)
 
     return prop
 
 
 #
+# Optimistic concurrency control
+#
+
+def retry_on_conflict(max_retries=-1):
+    """
+    Decorator for optimistic concurrency control
+
+    :param max_retries: The maximum number of retries, -1 for infinite
+    :return: The decorated function
+    """
+
+    def decorator(func: Callable):
+        @wraps(func)
+        async def wrapper(*args, **kwargs):
+            retries = 0
+            while True:
+                try:
+                    return await func(*args, **kwargs)
+                except ElasticConflictError:
+                    if max_retries == -1 or retries < max_retries:
+                        retries += 1
+                        logger.warning(f"Optimistic concurrency control conflict, retrying {retries}/{max_retries}")
+                        continue
+                    else:
+                        raise
+
+        return wrapper
+
+    return decorator
+
+
+#
 # Pagination and sort
 #
 
 class Pagination(BaseModel):
     """
     Pagination parameters
     """
```

### Comparing `pyesorm-0.4.0/esorm/query.py` & `pyesorm-0.4.1/esorm/query.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.0/esorm/response.py` & `pyesorm-0.4.1/esorm/response.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.0/esorm/utils.py` & `pyesorm-0.4.1/esorm/utils.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.0/esorm/watcher.py` & `pyesorm-0.4.1/esorm/watcher.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.0/pyesorm.egg-info/PKG-INFO` & `pyesorm-0.4.1/pyesorm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyesorm
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python ElasticSearch ORM based on Pydantic
 Home-page: https://github.com/wallneradam/esorm
 Author: Adam Wallner
 Author-email: Adam.wallner@gmail.com
 License: MPL-2.0
 Project-URL: Bug Tracker, https://github.com/wallneradam/esorm/issues
 Project-URL: Documentation, https://esorm.readthedocs.io/en/latest/
```

### Comparing `pyesorm-0.4.0/pyesorm.egg-info/SOURCES.txt` & `pyesorm-0.4.1/pyesorm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.0/setup.cfg` & `pyesorm-0.4.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyesorm
-version = 0.4.0
+version = 0.4.1
 author = Adam Wallner
 author_email = Adam.wallner@gmail.com
 description = Python ElasticSearch ORM based on Pydantic
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = ElasticSearch, ORM, Pydantic
 license = MPL-2.0
```

### Comparing `pyesorm-0.4.0/tests/conftest.py` & `pyesorm-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.0/tests/test_esorm.py` & `pyesorm-0.4.1/tests/test_esorm.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,14 +262,56 @@
             await doc1.save(wait_for=True)
             await doc2.delete()
 
         doc = await model_nested.get(doc_id)
         assert doc is not None
         assert doc.f_float == 3.0
 
+    async def test_retry_on_conflict(self, es, esorm, model_timestamp):
+        """
+        Test optimistic concurrency control with retry
+        """
+        import asyncio
+        from elasticsearch import ConflictError
+
+        doc = model_timestamp(f_str="occ_retry", f_int=10)
+        await doc.save()
+
+        @esorm.retry_on_conflict(3)
+        async def update_doc(doc_id):
+            _doc = await model_timestamp.get(doc_id)
+            _doc.f_int += 1
+            await _doc.save()
+
+        await asyncio.gather(
+            update_doc(doc._id),
+            update_doc(doc._id),
+            update_doc(doc._id),
+        )
+
+        await doc.reload()
+        assert doc.f_int == 13
+
+        doc = model_timestamp(f_str="occ_retry", f_int=10)
+        await doc.save()
+
+        # Test it without retry logic
+
+        async def update_without_retry(doc_id):
+            _doc = await model_timestamp.get(doc_id)
+            _doc.f_int += 1
+            await _doc.save()
+
+        with pytest.raises(ConflictError):
+            await asyncio.gather(
+                update_without_retry(doc._id),
+                update_without_retry(doc._id),
+                update_without_retry(doc._id),
+            )
+
     # noinspection PyBroadException
     async def test_crud_delete(self, es, esorm, model_nested):
         """
         Test delete
         """
         doc_id = self.__class__.doc_id
         # Delete
```

