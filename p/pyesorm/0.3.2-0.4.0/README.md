# Comparing `tmp/pyesorm-0.3.2.tar.gz` & `tmp/pyesorm-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyesorm-0.3.2.tar", last modified: Fri May  3 19:07:13 2024, max compression
+gzip compressed data, was "pyesorm-0.4.0.tar", last modified: Tue May  7 08:45:02 2024, max compression
```

## Comparing `pyesorm-0.3.2.tar` & `pyesorm-0.4.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-03 19:07:13.139805 pyesorm-0.3.2/
--rw-r--r--   0 wallner    (501) staff       (20)    16725 2023-10-30 16:10:12.000000 pyesorm-0.3.2/LICENSE
--rw-r--r--   0 wallner    (501) staff       (20)    22773 2024-05-03 19:07:13.139577 pyesorm-0.3.2/PKG-INFO
--rw-r--r--   0 wallner    (501) staff       (20)    21136 2024-04-29 12:11:29.000000 pyesorm-0.3.2/README.md
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-03 19:07:13.127076 pyesorm-0.3.2/docs/
--rw-r--r--   0 wallner    (501) staff       (20)        0 2024-01-17 15:06:14.000000 pyesorm-0.3.2/docs/__init__.py
--rw-r--r--   0 wallner    (501) staff       (20)     1484 2024-01-17 15:18:18.000000 pyesorm-0.3.2/docs/changelog.py
--rw-r--r--   0 wallner    (501) staff       (20)     1462 2024-01-17 15:10:11.000000 pyesorm-0.3.2/docs/conf.py
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-03 19:07:13.132816 pyesorm-0.3.2/esorm/
--rw-r--r--   0 wallner    (501) staff       (20)      666 2024-04-29 11:40:09.000000 pyesorm-0.3.2/esorm/__init__.py
--rw-r--r--   0 wallner    (501) staff       (20)     3132 2024-01-22 17:32:29.000000 pyesorm-0.3.2/esorm/aggs.py
--rw-r--r--   0 wallner    (501) staff       (20)     2028 2024-05-03 18:04:45.000000 pyesorm-0.3.2/esorm/bulk.py
--rw-r--r--   0 wallner    (501) staff       (20)      470 2023-10-30 16:10:12.000000 pyesorm-0.3.2/esorm/error.py
--rw-r--r--   0 wallner    (501) staff       (20)     1943 2023-10-31 19:12:30.000000 pyesorm-0.3.2/esorm/esorm.py
--rw-r--r--   0 wallner    (501) staff       (20)     3500 2024-01-24 09:39:22.000000 pyesorm-0.3.2/esorm/fastapi.py
--rw-r--r--   0 wallner    (501) staff       (20)    11640 2023-10-31 19:12:30.000000 pyesorm-0.3.2/esorm/fields.py
--rw-r--r--   0 wallner    (501) staff       (20)       52 2023-10-30 16:10:12.000000 pyesorm-0.3.2/esorm/logger.py
--rw-r--r--   0 wallner    (501) staff       (20)    38189 2024-05-03 17:24:16.000000 pyesorm-0.3.2/esorm/model.py
--rw-r--r--   0 wallner    (501) staff       (20)     9605 2024-01-18 19:16:18.000000 pyesorm-0.3.2/esorm/query.py
--rw-r--r--   0 wallner    (501) staff       (20)     1315 2024-01-18 19:06:35.000000 pyesorm-0.3.2/esorm/response.py
--rw-r--r--   0 wallner    (501) staff       (20)      996 2024-01-23 07:15:23.000000 pyesorm-0.3.2/esorm/utils.py
--rw-r--r--   0 wallner    (501) staff       (20)     5538 2023-10-30 16:10:12.000000 pyesorm-0.3.2/esorm/watcher.py
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-03 19:07:13.137446 pyesorm-0.3.2/pyesorm.egg-info/
--rw-r--r--   0 wallner    (501) staff       (20)    22773 2024-05-03 19:07:13.000000 pyesorm-0.3.2/pyesorm.egg-info/PKG-INFO
--rw-r--r--   0 wallner    (501) staff       (20)      514 2024-05-03 19:07:13.000000 pyesorm-0.3.2/pyesorm.egg-info/SOURCES.txt
--rw-r--r--   0 wallner    (501) staff       (20)        1 2024-05-03 19:07:13.000000 pyesorm-0.3.2/pyesorm.egg-info/dependency_links.txt
--rw-r--r--   0 wallner    (501) staff       (20)      272 2024-05-03 19:07:13.000000 pyesorm-0.3.2/pyesorm.egg-info/requires.txt
--rw-r--r--   0 wallner    (501) staff       (20)       17 2024-05-03 19:07:13.000000 pyesorm-0.3.2/pyesorm.egg-info/top_level.txt
--rw-r--r--   0 wallner    (501) staff       (20)       87 2023-10-31 20:33:56.000000 pyesorm-0.3.2/pyproject.toml
--rw-r--r--   0 wallner    (501) staff       (20)     1306 2024-05-03 19:07:13.140502 pyesorm-0.3.2/setup.cfg
--rw-r--r--   0 wallner    (501) staff       (20)       37 2023-10-30 16:10:12.000000 pyesorm-0.3.2/setup.py
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-03 19:07:13.136293 pyesorm-0.3.2/tests/
--rw-r--r--   0 wallner    (501) staff       (20)        0 2023-10-30 16:10:12.000000 pyesorm-0.3.2/tests/__init__.py
--rw-r--r--   0 wallner    (501) staff       (20)     7056 2024-05-03 18:47:40.000000 pyesorm-0.3.2/tests/conftest.py
--rw-r--r--   0 wallner    (501) staff       (20)    25009 2024-05-03 19:04:15.000000 pyesorm-0.3.2/tests/test_esorm.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 08:45:02.773973 pyesorm-0.4.0/
+-rw-r--r--   0 wallner    (501) staff       (20)    16725 2023-10-30 16:10:12.000000 pyesorm-0.4.0/LICENSE
+-rw-r--r--   0 wallner    (501) staff       (20)    23956 2024-05-07 08:45:02.773765 pyesorm-0.4.0/PKG-INFO
+-rw-r--r--   0 wallner    (501) staff       (20)    22319 2024-05-07 06:59:22.000000 pyesorm-0.4.0/README.md
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 08:45:02.759979 pyesorm-0.4.0/docs/
+-rw-r--r--   0 wallner    (501) staff       (20)        0 2024-01-17 15:06:14.000000 pyesorm-0.4.0/docs/__init__.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1484 2024-01-17 15:18:18.000000 pyesorm-0.4.0/docs/changelog.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1462 2024-01-17 15:10:11.000000 pyesorm-0.4.0/docs/conf.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 08:45:02.767406 pyesorm-0.4.0/esorm/
+-rw-r--r--   0 wallner    (501) staff       (20)      666 2024-04-29 11:40:09.000000 pyesorm-0.4.0/esorm/__init__.py
+-rw-r--r--   0 wallner    (501) staff       (20)     3132 2024-01-22 17:32:29.000000 pyesorm-0.4.0/esorm/aggs.py
+-rw-r--r--   0 wallner    (501) staff       (20)     4447 2024-05-07 05:08:54.000000 pyesorm-0.4.0/esorm/bulk.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1267 2024-05-07 05:07:07.000000 pyesorm-0.4.0/esorm/error.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1943 2023-10-31 19:12:30.000000 pyesorm-0.4.0/esorm/esorm.py
+-rw-r--r--   0 wallner    (501) staff       (20)     3500 2024-01-24 09:39:22.000000 pyesorm-0.4.0/esorm/fastapi.py
+-rw-r--r--   0 wallner    (501) staff       (20)    11640 2023-10-31 19:12:30.000000 pyesorm-0.4.0/esorm/fields.py
+-rw-r--r--   0 wallner    (501) staff       (20)       52 2023-10-30 16:10:12.000000 pyesorm-0.4.0/esorm/logger.py
+-rw-r--r--   0 wallner    (501) staff       (20)    41802 2024-05-07 05:46:54.000000 pyesorm-0.4.0/esorm/model.py
+-rw-r--r--   0 wallner    (501) staff       (20)     9605 2024-01-18 19:16:18.000000 pyesorm-0.4.0/esorm/query.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1315 2024-01-18 19:06:35.000000 pyesorm-0.4.0/esorm/response.py
+-rw-r--r--   0 wallner    (501) staff       (20)      996 2024-01-23 07:15:23.000000 pyesorm-0.4.0/esorm/utils.py
+-rw-r--r--   0 wallner    (501) staff       (20)     5538 2023-10-30 16:10:12.000000 pyesorm-0.4.0/esorm/watcher.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 08:45:02.771621 pyesorm-0.4.0/pyesorm.egg-info/
+-rw-r--r--   0 wallner    (501) staff       (20)    23956 2024-05-07 08:45:02.000000 pyesorm-0.4.0/pyesorm.egg-info/PKG-INFO
+-rw-r--r--   0 wallner    (501) staff       (20)      514 2024-05-07 08:45:02.000000 pyesorm-0.4.0/pyesorm.egg-info/SOURCES.txt
+-rw-r--r--   0 wallner    (501) staff       (20)        1 2024-05-07 08:45:02.000000 pyesorm-0.4.0/pyesorm.egg-info/dependency_links.txt
+-rw-r--r--   0 wallner    (501) staff       (20)      272 2024-05-07 08:45:02.000000 pyesorm-0.4.0/pyesorm.egg-info/requires.txt
+-rw-r--r--   0 wallner    (501) staff       (20)       17 2024-05-07 08:45:02.000000 pyesorm-0.4.0/pyesorm.egg-info/top_level.txt
+-rw-r--r--   0 wallner    (501) staff       (20)       87 2023-10-31 20:33:56.000000 pyesorm-0.4.0/pyproject.toml
+-rw-r--r--   0 wallner    (501) staff       (20)     1306 2024-05-07 08:45:02.774615 pyesorm-0.4.0/setup.cfg
+-rw-r--r--   0 wallner    (501) staff       (20)       37 2023-10-30 16:10:12.000000 pyesorm-0.4.0/setup.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-07 08:45:02.770544 pyesorm-0.4.0/tests/
+-rw-r--r--   0 wallner    (501) staff       (20)        0 2023-10-30 16:10:12.000000 pyesorm-0.4.0/tests/__init__.py
+-rw-r--r--   0 wallner    (501) staff       (20)     7056 2024-05-03 18:47:40.000000 pyesorm-0.4.0/tests/conftest.py
+-rw-r--r--   0 wallner    (501) staff       (20)    27877 2024-05-07 06:56:41.000000 pyesorm-0.4.0/tests/test_esorm.py
```

### Comparing `pyesorm-0.3.2/LICENSE` & `pyesorm-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.2/PKG-INFO` & `pyesorm-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyesorm
-Version: 0.3.2
+Version: 0.4.0
 Summary: Python ElasticSearch ORM based on Pydantic
 Home-page: https://github.com/wallneradam/esorm
 Author: Adam Wallner
 Author-email: Adam.wallner@gmail.com
 License: MPL-2.0
 Project-URL: Bug Tracker, https://github.com/wallneradam/esorm/issues
 Project-URL: Documentation, https://esorm.readthedocs.io/en/latest/
@@ -33,15 +33,14 @@
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: sphinx-rtd-theme==1.3.0; extra == "dev"
 Requires-Dist: sphinx-rtd-dark-mode==1.3.0; extra == "dev"
 Requires-Dist: sphinx-autodoc-typehints; extra == "dev"
 Requires-Dist: myst-parser; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
-<!--suppress HtmlDeprecatedAttribute -->
 <img src="https://raw.githubusercontent.com/wallneradam/esorm/main/docs/_static/img/esorm.svg" width="110" height="110" align="left" style="margin-right: 1em;" alt="Logo"/>
 
 # ESORM - Python ElasticSearch ORM based on Pydantic
 
 <small>Some ideas come from [Pydastic](https://github.com/RamiAwar/pydastic) library, which is similar,
 but not as advanced (yet).</small>
 
@@ -61,25 +60,27 @@
         - [Model Settings](#model-settings)
         - [Describe fields](#describe-fields)
         - [ESModelTimestamp](#esmodeltimestamp)
     - [Connecting to ElasticSearch](#connecting-to-elasticsearch)
         - [Client](#client)
     - [Create index templates](#create-index-templates)
     - [Create indices and mappings](#create-indices-and-mappings)
+    - [Model instances](#model-instances)
     - [CRUD: Create](#crud-create)
     - [CRUD: Read](#crud-read)
     - [CRUD: Update](#crud-update)
     - [CRUD: Delete](#crud-delete)
     - [Bulk operations](#bulk-operations)
     - [Search](#search)
         - [General search](#general-search)
         - [Search with field value terms (dictioanry search)](#search-with-field-value-terms-dictionary-search)
     - [Aggregations](#aggregations)
     - [Pagination and sorting](#pagination-and-sorting)
 - [🔬 Advanced usage](docs/advanced.md#advanced-usage) 
+    - [Optimistic concurrency control](docs/advanced.md#optimistic-concurrency-control)
     - [Lazy properties](docs/advanced.md#lazy-properties)
     - [Shard routing](docs/advanced.md#shard-routing)
     - [Watchers](docs/advanced.md#watchers)
     - [FastAPI integration](docs/advanced.md#fastapi-integration)
 - [🧪 Testing](#testing)
 - [🛡 License](#license)
 - [📃 Citation](#citation)
@@ -97,14 +98,15 @@
 
 - Pydantic model representation of ElasticSearch documents
 - Automatic mapping and index creation
 - CRUD operations
 - Full async support (no sync version at all)
 - Mapping to and from ElasticSearch types
 - Support for nested documents
+- Automatic optimistic concurrency control
 - Custom id field
 - Context for bulk operations
 - Supported IDE autocompletion and type checking (PyCharm tested)
 - Everything in the source code is documented and annotated
 - `TypedDict`s for ElasticSearch queries and aggregations
 - Docstring support for fields
 - Shard routing support
@@ -478,14 +480,28 @@
 Then you can call `setup_mappings` function to create indices and mappings for all registered models.
 
 **IMPORTANT:** This method will ignore mapping errors if you already have an index with the same name. It can update the
 indices
 by new fields, but cannot modify or delete fields! For that you need to reindex your ES database. It is an ElasticSearch
 limitation.
 
+<a id="model-instances"></a>
+### Model instances
+
+When you get a model instance from elasticsearch by `search` or `get` methods, you will get the following private
+attributes filled automatically:
+
+| Attribute       | Description                         |
+|-----------------|-------------------------------------|
+| `_id`           | The ES id of the document           |
+| `_routing`      | The routing value of the document   |
+| `_version`      | Version of the document             |
+| `_primary_term` | The primary term of the document    |
+| `_seq_no`       | The sequence number of the document |
+
 <a id="crud-create"></a>
 ### CRUD: Create
 
 ```python
 from esorm import ESModel
 
 
@@ -520,14 +536,17 @@
     user = await User.get(user_id)
     print(user.name)
 ```
 
 <a id="crud-update"></a>
 ### CRUD: Update
 
+On update race conditions are checked automatically (with the help of _primary_term and _seq_no fields).
+This way an optimistic locking mechanism is implemented.
+
 ```python
 from esorm import ESModel
 
 
 # Here the model have automatically generated id
 class User(ESModel):
     name: str
@@ -750,25 +769,33 @@
 ### Pagination and sorting
 
 You can use `Pagination` and `Sort` classes to decorate your models. They simply wrap your models
 and add pagination and sorting functionality to them.
 
 #### Pagination
 
+You can add a callback parameter to the `Pagination` class which will be invoked after the search with
+the total number of documents found.
+
 ```python
 from esorm.model import ESModel, Pagination
 
 
 class User(ESModel):
     id: int  # This will be used as the document _id in the index
     name: str
     age: int
 
 
 def get_users(page = 1, page_size = 10):
+
+    def pagination_callback(total: int):
+        # You may set a header value or something else here
+        print(f'Total users: {total}')
+
     # 1st create the decorator itself
     pagination = Pagination(page=page, page_size=page_size)
     
     # Then decorate your model
     res = pagination(User).search_by_fields(age=18)
     
     # Here the result has maximum 10 items
```

### Comparing `pyesorm-0.3.2/README.md` & `pyesorm-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-<!--suppress HtmlDeprecatedAttribute -->
 <img src="https://raw.githubusercontent.com/wallneradam/esorm/main/docs/_static/img/esorm.svg" width="110" height="110" align="left" style="margin-right: 1em;" alt="Logo"/>
 
 # ESORM - Python ElasticSearch ORM based on Pydantic
 
 <small>Some ideas come from [Pydastic](https://github.com/RamiAwar/pydastic) library, which is similar,
 but not as advanced (yet).</small>
 
@@ -22,25 +21,27 @@
         - [Model Settings](#model-settings)
         - [Describe fields](#describe-fields)
         - [ESModelTimestamp](#esmodeltimestamp)
     - [Connecting to ElasticSearch](#connecting-to-elasticsearch)
         - [Client](#client)
     - [Create index templates](#create-index-templates)
     - [Create indices and mappings](#create-indices-and-mappings)
+    - [Model instances](#model-instances)
     - [CRUD: Create](#crud-create)
     - [CRUD: Read](#crud-read)
     - [CRUD: Update](#crud-update)
     - [CRUD: Delete](#crud-delete)
     - [Bulk operations](#bulk-operations)
     - [Search](#search)
         - [General search](#general-search)
         - [Search with field value terms (dictioanry search)](#search-with-field-value-terms-dictionary-search)
     - [Aggregations](#aggregations)
     - [Pagination and sorting](#pagination-and-sorting)
 - [🔬 Advanced usage](docs/advanced.md#advanced-usage) 
+    - [Optimistic concurrency control](docs/advanced.md#optimistic-concurrency-control)
     - [Lazy properties](docs/advanced.md#lazy-properties)
     - [Shard routing](docs/advanced.md#shard-routing)
     - [Watchers](docs/advanced.md#watchers)
     - [FastAPI integration](docs/advanced.md#fastapi-integration)
 - [🧪 Testing](#testing)
 - [🛡 License](#license)
 - [📃 Citation](#citation)
@@ -58,14 +59,15 @@
 
 - Pydantic model representation of ElasticSearch documents
 - Automatic mapping and index creation
 - CRUD operations
 - Full async support (no sync version at all)
 - Mapping to and from ElasticSearch types
 - Support for nested documents
+- Automatic optimistic concurrency control
 - Custom id field
 - Context for bulk operations
 - Supported IDE autocompletion and type checking (PyCharm tested)
 - Everything in the source code is documented and annotated
 - `TypedDict`s for ElasticSearch queries and aggregations
 - Docstring support for fields
 - Shard routing support
@@ -439,14 +441,28 @@
 Then you can call `setup_mappings` function to create indices and mappings for all registered models.
 
 **IMPORTANT:** This method will ignore mapping errors if you already have an index with the same name. It can update the
 indices
 by new fields, but cannot modify or delete fields! For that you need to reindex your ES database. It is an ElasticSearch
 limitation.
 
+<a id="model-instances"></a>
+### Model instances
+
+When you get a model instance from elasticsearch by `search` or `get` methods, you will get the following private
+attributes filled automatically:
+
+| Attribute       | Description                         |
+|-----------------|-------------------------------------|
+| `_id`           | The ES id of the document           |
+| `_routing`      | The routing value of the document   |
+| `_version`      | Version of the document             |
+| `_primary_term` | The primary term of the document    |
+| `_seq_no`       | The sequence number of the document |
+
 <a id="crud-create"></a>
 ### CRUD: Create
 
 ```python
 from esorm import ESModel
 
 
@@ -481,14 +497,17 @@
     user = await User.get(user_id)
     print(user.name)
 ```
 
 <a id="crud-update"></a>
 ### CRUD: Update
 
+On update race conditions are checked automatically (with the help of _primary_term and _seq_no fields).
+This way an optimistic locking mechanism is implemented.
+
 ```python
 from esorm import ESModel
 
 
 # Here the model have automatically generated id
 class User(ESModel):
     name: str
@@ -711,25 +730,33 @@
 ### Pagination and sorting
 
 You can use `Pagination` and `Sort` classes to decorate your models. They simply wrap your models
 and add pagination and sorting functionality to them.
 
 #### Pagination
 
+You can add a callback parameter to the `Pagination` class which will be invoked after the search with
+the total number of documents found.
+
 ```python
 from esorm.model import ESModel, Pagination
 
 
 class User(ESModel):
     id: int  # This will be used as the document _id in the index
     name: str
     age: int
 
 
 def get_users(page = 1, page_size = 10):
+
+    def pagination_callback(total: int):
+        # You may set a header value or something else here
+        print(f'Total users: {total}')
+
     # 1st create the decorator itself
     pagination = Pagination(page=page, page_size=page_size)
     
     # Then decorate your model
     res = pagination(User).search_by_fields(age=18)
     
     # Here the result has maximum 10 items
```

### Comparing `pyesorm-0.3.2/docs/changelog.py` & `pyesorm-0.4.0/docs/changelog.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.2/docs/conf.py` & `pyesorm-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.2/esorm/__init__.py` & `pyesorm-0.4.0/esorm/__init__.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.2/esorm/aggs.py` & `pyesorm-0.4.0/esorm/aggs.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.2/esorm/esorm.py` & `pyesorm-0.4.0/esorm/esorm.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.2/esorm/fastapi.py` & `pyesorm-0.4.0/esorm/fastapi.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.2/esorm/fields.py` & `pyesorm-0.4.0/esorm/fields.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.2/esorm/model.py` & `pyesorm-0.4.0/esorm/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -258,14 +258,23 @@
 
     _id: Optional[str] = PrivateAttr(None)
     """ The ES id of the document """
 
     _routing: Optional[str] = PrivateAttr(None)
     """ The routing of the document """
 
+    _version: Optional[int] = PrivateAttr(None)
+    """ The version of the document """
+
+    _primary_term: Optional[int] = PrivateAttr(None)
+    """ The primary term of the document """
+
+    _seq_no: Optional[int] = PrivateAttr(None)
+    """ The sequence number of the document """
+
     class ESConfig:
         """ ESModel Config """
         index: Optional[str] = None
         """ The index name """
 
         id_field: Optional[str] = None
         """ The name of the 'id' field """
@@ -317,14 +326,15 @@
         kwargs = dict(kwargs)
         method = getattr(es, method_name)
         index = cls.ESConfig.index
         if wait_for is not None:
             kwargs['refresh'] = "wait_for"
         if 'request_timeout' not in kwargs:
             kwargs['request_timeout'] = 60
+
         return await method(index=index, **kwargs)
 
     def to_es(self, **kwargs) -> dict:
         """
         Generates a dictionary equivalent to what ElasticSearch returns in the '_source' property of a response.
 
         It automatically removes the id field from the document if it is set in ESConfig.id_field to prevent
@@ -368,42 +378,89 @@
                 # Convert subclasses
                 elif isinstance(v, dict):
                     recursive_convert(v)
 
         recursive_convert(d)
         return d
 
+    def update_from_es(self, data: Dict[str, Any]):
+        """
+        Update the model from ElasticSearch data
+
+        :param data: The ElasticSearch data
+        :raises esorm.error.InvalidResponseError: Returned when _id or _source is missing from data
+        """
+        if not data:
+            return None
+
+        source: Optional[dict] = data.get("_source", None)
+        # Get id field
+        _id = data.get("_id", None)
+        if not source or not _id:
+            raise InvalidResponseError
+
+        for k, v in source.items():
+            if k in self.__fields_set__:
+                print(k, '=', v)
+                setattr(self, k, v)
+
+        # Set routing field
+        _routing = data.get("_routing", None)
+        setattr(self, '_routing', _routing)
+
+        # Set version field
+        _version = data.get("_version", None)
+        setattr(self, '_version', _version)
+        # Set primary term field
+        _primary_term = data.get("_primary_term", None)
+        setattr(self, '_primary_term', _primary_term)
+        # Set seq_no field
+        _seq_no = data.get("_seq_no", None)
+        setattr(self, '_seq_no', _seq_no)
+
     @classmethod
     def from_es(cls: Type[TModel], data: Dict[str, Any]) -> Optional[TModel]:
         """
         Returns an ESModel from an elasticsearch document that has _id, _source
 
         :param data: Elasticsearch document that has _id, _source
         :raises esorm.error.InvalidResponseError: Returned when _id or _source is missing from data
         :return: The ESModel instance
         """
         if not data:
             return None
 
         source: Optional[dict] = data.get("_source", None)
+        # Get id field
         _id = data.get("_id", None)
-
         if not source or not _id:
             raise InvalidResponseError
 
         # Add id field to document
         if source is not None and cls.ESConfig.id_field:
             source[cls.ESConfig.id_field] = _id
         obj = cls(**source)
+
+        # Set id field
         setattr(obj, '_id', _id)
 
         # Set routing field
         _routing = data.get("_routing", None)
         setattr(obj, '_routing', _routing)
 
+        # Set version field
+        _version = data.get("_version", None)
+        setattr(obj, '_version', _version)
+        # Set primary term field
+        _primary_term = data.get("_primary_term", None)
+        setattr(obj, '_primary_term', _primary_term)
+        # Set seq_no field
+        _seq_no = data.get("_seq_no", None)
+        setattr(obj, '_seq_no', _seq_no)
+
         return obj
 
     async def save(self, *, wait_for=False, pipeline: Optional[str] = None, routing: Optional[str] = None) -> str:
         """
         Save document into elasticsearch.
 
         If document already exists, existing document will be updated as per native elasticsearch index operation.
@@ -418,25 +475,41 @@
         :param routing: Shard routing value
         :return: The new document's ID
         """
         kwargs = dict(
             document=self.to_es(),
             wait_for=wait_for,
         )
+
         kwargs['id'] = self.__id__
         if self.ESConfig.id_field:
             del kwargs['document'][self.ESConfig.id_field]
+
         if pipeline is not None:
             kwargs['pipeline'] = pipeline
+
         if routing is not None:
             kwargs['routing'] = routing
         else:
             kwargs['routing'] = self.__routing__
+
+        if self._primary_term is not None:
+            kwargs['if_primary_term'] = self._primary_term
+        if self._seq_no is not None:
+            kwargs['if_seq_no'] = self._seq_no
+
         es_res = await self.call('index', **kwargs)
-        return es_res.get('_id')
+
+        # Update private fields
+        self._id = es_res.get('_id', None)
+        self._version = es_res.get('_version', None)
+        self._primary_term = es_res.get('_primary_term', None)
+        self._seq_no = es_res.get('_seq_no', None)
+        # Return the new document's ID
+        return self._id
 
     # noinspection PyShadowingBuiltins
     @classmethod
     async def get(cls: Type[TModel], id: Union[str, int, float], *, routing: Optional[str] = None) -> TModel:
         """
         Fetches document and returns ESModel instance populated with properties.
 
@@ -444,35 +517,59 @@
         :param routing: Shard routing value
         :raises esorm.error.NotFoundError: Returned if document not found
         :return: ESModel object
         """
         kwargs = dict(id=str(id))
         if routing:
             kwargs['routing'] = routing
+        else:
+            kwargs['routing'] = cls.__routing__
         try:
             es_res = await cls.call('get', **kwargs)
             return await _lazy_process_results(cls.from_es(es_res))
         except ElasticNotFoundError:
             raise NotFoundError(f"Document with id {id} not found")
 
     async def delete(self, *, wait_for=False, routing: Optional[str] = None):
         """
-        Deletes document from elasticsearch.
+        Deletes document from ElasticSearch.
 
         :param wait_for: Waits for all shards to sync before returning response - useful when writing
                          tests. Defaults to False.
         :param routing: Shard routing value
         :raises esorm.error.NotFoundError: Returned if document not found
         :raises ValueError: Returned when id attribute missing from instance
         """
+        kwargs = dict(id=self.__id__)
+        if self._primary_term is not None:
+            kwargs['if_primary_term'] = self._primary_term
+        if self._seq_no is not None:
+            kwargs['if_seq_no'] = self._seq_no
         try:
-            await self.call('delete', wait_for=wait_for, id=self.__id__, routing=routing)
+            await self.call('delete', wait_for=wait_for,
+                            routing=routing if routing is not None else self.__routing__,
+                            **kwargs)
         except ElasticNotFoundError:
             raise NotFoundError(f"Document with id {self.__id__} not found!")
 
+    async def reload(self, *, routing: Optional[str] = None) -> TModel:
+        """
+        Reloads the document from ElasticSearch
+
+        :param routing: Shard routing value
+        :raises esorm.error.NotFoundError: Returned if document not found
+        """
+        kwargs = dict(id=self.__id__, routing=routing if routing is not None else self.__routing__)
+        try:
+            es_res = await self.call('get', **kwargs)
+            self.update_from_es(es_res)
+            return await _lazy_process_results(self)
+        except ElasticNotFoundError:
+            raise NotFoundError(f"Document with id {id} not found")
+
     @classmethod
     async def _search(cls: Type[TModel],
                       query: Optional[ESQuery] = None,
                       *,
                       page_size: Optional[int] = None,
                       page: Optional[int] = None,
                       sort: Optional[Union[list, str]] = None,
@@ -499,15 +596,17 @@
 
         if page_size is not None and page is None:
             page = 1
 
         return await cls.call('search', query=query,
                               from_=((page - 1) * page_size) if page_size is not None else 0,
                               size=page_size, sort=sort, routing=routing,
-                              aggs=aggs, **kwargs)
+                              aggs=aggs,
+                              seq_no_primary_term=True, version=True,
+                              **kwargs)
 
     @classmethod
     async def search(cls: Type[TModel], query: ESQuery, *,
                      page_size: Optional[int] = None,
                      page: Optional[int] = None,
                      sort: Optional[Union[list, str]] = None,
                      routing: Optional[str] = None,
@@ -699,14 +798,19 @@
 
         if pipeline is not None:
             kwargs['pipeline'] = pipeline
 
         if routing is not None:
             kwargs['routing'] = routing
 
+        if self._primary_term is not None:
+            kwargs['if_primary_term'] = self._primary_term
+        if self._seq_no is not None:
+            kwargs['if_seq_no'] = self._seq_no
+
         # Set id field
         kwargs['id'] = self.__id__
         # Remove the id field from the document
         if self.ESConfig.id_field:
             del doc[self.ESConfig.id_field]
             del doc_upsert[self.ESConfig.id_field]
```

### Comparing `pyesorm-0.3.2/esorm/query.py` & `pyesorm-0.4.0/esorm/query.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.2/esorm/response.py` & `pyesorm-0.4.0/esorm/response.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.2/esorm/utils.py` & `pyesorm-0.4.0/esorm/utils.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.2/esorm/watcher.py` & `pyesorm-0.4.0/esorm/watcher.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.2/pyesorm.egg-info/PKG-INFO` & `pyesorm-0.4.0/pyesorm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyesorm
-Version: 0.3.2
+Version: 0.4.0
 Summary: Python ElasticSearch ORM based on Pydantic
 Home-page: https://github.com/wallneradam/esorm
 Author: Adam Wallner
 Author-email: Adam.wallner@gmail.com
 License: MPL-2.0
 Project-URL: Bug Tracker, https://github.com/wallneradam/esorm/issues
 Project-URL: Documentation, https://esorm.readthedocs.io/en/latest/
@@ -33,15 +33,14 @@
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: sphinx-rtd-theme==1.3.0; extra == "dev"
 Requires-Dist: sphinx-rtd-dark-mode==1.3.0; extra == "dev"
 Requires-Dist: sphinx-autodoc-typehints; extra == "dev"
 Requires-Dist: myst-parser; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
-<!--suppress HtmlDeprecatedAttribute -->
 <img src="https://raw.githubusercontent.com/wallneradam/esorm/main/docs/_static/img/esorm.svg" width="110" height="110" align="left" style="margin-right: 1em;" alt="Logo"/>
 
 # ESORM - Python ElasticSearch ORM based on Pydantic
 
 <small>Some ideas come from [Pydastic](https://github.com/RamiAwar/pydastic) library, which is similar,
 but not as advanced (yet).</small>
 
@@ -61,25 +60,27 @@
         - [Model Settings](#model-settings)
         - [Describe fields](#describe-fields)
         - [ESModelTimestamp](#esmodeltimestamp)
     - [Connecting to ElasticSearch](#connecting-to-elasticsearch)
         - [Client](#client)
     - [Create index templates](#create-index-templates)
     - [Create indices and mappings](#create-indices-and-mappings)
+    - [Model instances](#model-instances)
     - [CRUD: Create](#crud-create)
     - [CRUD: Read](#crud-read)
     - [CRUD: Update](#crud-update)
     - [CRUD: Delete](#crud-delete)
     - [Bulk operations](#bulk-operations)
     - [Search](#search)
         - [General search](#general-search)
         - [Search with field value terms (dictioanry search)](#search-with-field-value-terms-dictionary-search)
     - [Aggregations](#aggregations)
     - [Pagination and sorting](#pagination-and-sorting)
 - [🔬 Advanced usage](docs/advanced.md#advanced-usage) 
+    - [Optimistic concurrency control](docs/advanced.md#optimistic-concurrency-control)
     - [Lazy properties](docs/advanced.md#lazy-properties)
     - [Shard routing](docs/advanced.md#shard-routing)
     - [Watchers](docs/advanced.md#watchers)
     - [FastAPI integration](docs/advanced.md#fastapi-integration)
 - [🧪 Testing](#testing)
 - [🛡 License](#license)
 - [📃 Citation](#citation)
@@ -97,14 +98,15 @@
 
 - Pydantic model representation of ElasticSearch documents
 - Automatic mapping and index creation
 - CRUD operations
 - Full async support (no sync version at all)
 - Mapping to and from ElasticSearch types
 - Support for nested documents
+- Automatic optimistic concurrency control
 - Custom id field
 - Context for bulk operations
 - Supported IDE autocompletion and type checking (PyCharm tested)
 - Everything in the source code is documented and annotated
 - `TypedDict`s for ElasticSearch queries and aggregations
 - Docstring support for fields
 - Shard routing support
@@ -478,14 +480,28 @@
 Then you can call `setup_mappings` function to create indices and mappings for all registered models.
 
 **IMPORTANT:** This method will ignore mapping errors if you already have an index with the same name. It can update the
 indices
 by new fields, but cannot modify or delete fields! For that you need to reindex your ES database. It is an ElasticSearch
 limitation.
 
+<a id="model-instances"></a>
+### Model instances
+
+When you get a model instance from elasticsearch by `search` or `get` methods, you will get the following private
+attributes filled automatically:
+
+| Attribute       | Description                         |
+|-----------------|-------------------------------------|
+| `_id`           | The ES id of the document           |
+| `_routing`      | The routing value of the document   |
+| `_version`      | Version of the document             |
+| `_primary_term` | The primary term of the document    |
+| `_seq_no`       | The sequence number of the document |
+
 <a id="crud-create"></a>
 ### CRUD: Create
 
 ```python
 from esorm import ESModel
 
 
@@ -520,14 +536,17 @@
     user = await User.get(user_id)
     print(user.name)
 ```
 
 <a id="crud-update"></a>
 ### CRUD: Update
 
+On update race conditions are checked automatically (with the help of _primary_term and _seq_no fields).
+This way an optimistic locking mechanism is implemented.
+
 ```python
 from esorm import ESModel
 
 
 # Here the model have automatically generated id
 class User(ESModel):
     name: str
@@ -750,25 +769,33 @@
 ### Pagination and sorting
 
 You can use `Pagination` and `Sort` classes to decorate your models. They simply wrap your models
 and add pagination and sorting functionality to them.
 
 #### Pagination
 
+You can add a callback parameter to the `Pagination` class which will be invoked after the search with
+the total number of documents found.
+
 ```python
 from esorm.model import ESModel, Pagination
 
 
 class User(ESModel):
     id: int  # This will be used as the document _id in the index
     name: str
     age: int
 
 
 def get_users(page = 1, page_size = 10):
+
+    def pagination_callback(total: int):
+        # You may set a header value or something else here
+        print(f'Total users: {total}')
+
     # 1st create the decorator itself
     pagination = Pagination(page=page, page_size=page_size)
     
     # Then decorate your model
     res = pagination(User).search_by_fields(age=18)
     
     # Here the result has maximum 10 items
```

### Comparing `pyesorm-0.3.2/pyesorm.egg-info/SOURCES.txt` & `pyesorm-0.4.0/pyesorm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.2/setup.cfg` & `pyesorm-0.4.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyesorm
-version = 0.3.2
+version = 0.4.0
 author = Adam Wallner
 author_email = Adam.wallner@gmail.com
 description = Python ElasticSearch ORM based on Pydantic
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = ElasticSearch, ORM, Pydantic
 license = MPL-2.0
```

### Comparing `pyesorm-0.3.2/tests/conftest.py` & `pyesorm-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.2/tests/test_esorm.py` & `pyesorm-0.4.0/tests/test_esorm.py`

 * *Files 4% similar despite different names*

```diff
@@ -193,14 +193,19 @@
         # Get by id
         doc = await model_nested.get(doc_id)
         assert doc is not None
         assert doc.f_float == 0.5  # Default value of the field
         assert doc.f_nested is not None
         assert doc.f_nested.f_str == "nested_test"
 
+        # Check private fields
+        assert doc._version == 1
+        assert doc._primary_term == 1
+        assert doc._seq_no == 0
+
     async def test_crud_update(self, es, esorm, model_nested):
         """
         Test update
         """
         doc_id = self.__class__.doc_id
         # Update
         doc = await model_nested.get(doc_id)
@@ -215,14 +220,56 @@
         assert doc is not None
         assert doc.f_nested.f_str == "nested_test_updated"
         # Test if modified_at is updated even in nested fields
         assert doc.f_nested.modified_at > modified_at
         # Test if created_at is not updated
         assert doc.f_nested.created_at == created_at
 
+        # Check private fields
+        assert doc._version == 2
+        assert doc._primary_term == 1
+        assert doc._seq_no == 5  # It is 5 because other documents have been created
+
+    async def test_race_condition(self, es, esorm, model_nested):
+        """
+        Test race condition
+        Race conditions should raise a ConflictError
+        """
+        from elasticsearch import ConflictError
+
+        ### Test update ###
+
+        doc_id = self.__class__.doc_id
+        # Get 2 instances of the same document
+        doc1 = await model_nested.get(doc_id)
+        doc1.f_float = 1.0
+        doc2 = await model_nested.get(doc_id)
+        doc1.f_float = 2.0
+
+        # The 2nd save should not work
+        with pytest.raises(ConflictError):
+            await doc1.save()
+            await doc2.save()
+
+        ### Test delete ###
+
+        # Get 2 instances of the same document
+        doc1 = await model_nested.get(doc_id)
+        doc1.f_float = 3.0
+        doc2 = await model_nested.get(doc_id)
+
+        # Update and delete at the same time
+        with pytest.raises(ConflictError):
+            await doc1.save(wait_for=True)
+            await doc2.delete()
+
+        doc = await model_nested.get(doc_id)
+        assert doc is not None
+        assert doc.f_float == 3.0
+
     # noinspection PyBroadException
     async def test_crud_delete(self, es, esorm, model_nested):
         """
         Test delete
         """
         doc_id = self.__class__.doc_id
         # Delete
@@ -251,14 +298,42 @@
         # Deleting documents
         async with esorm.ESBulk(wait_for=True) as bulk:  # Here wait_for is important!
             for i in range(10):
                 doc = await model_nested.search_one_by_fields({'f_nested.f_str': f"nested_test1{i}"})
                 assert doc is not None
                 await bulk.delete(doc)
 
+    async def test_bulk_race_condition_and_reload(self, es, esorm, model_nested, model_timestamp):
+        """
+        Test bulk operations with conflict
+        """
+        doc = model_nested(f_nested=model_timestamp(f_str=f"nested_test1"), f_float=10.0)
+        await doc.save()
+
+        with pytest.raises(esorm.error.BulkError):
+            async with esorm.ESBulk(wait_for=True) as bulk:
+                doc1 = await model_nested.search_one_by_fields({'f_nested.f_str': f"nested_test1"})
+                assert doc1._version == 1
+                doc2 = await model_nested.search_one_by_fields({'f_nested.f_str': f"nested_test1"})
+                assert doc2._version == 1
+                assert doc1 is not None
+                assert doc2 is not None
+                doc1.f_float = 11.0
+                doc1.f_nested.f_str = "nested_test1_updated1"
+                await bulk.save(doc1)
+                # This should not work, because this is a race condition
+                doc2.f_float = 11.1
+                doc1.f_nested.f_str = "nested_test1_updated1"
+                await bulk.save(doc2)
+
+        # We test reloading here, it should now update the _primary_term and _seq_no
+        await doc.reload()
+        # So the deletion of document should be ok
+        await doc.delete()
+
     async def test_search(self, es, esorm, model_nested):
         """
         Test search
         """
         if TYPE_CHECKING:
             from esorm.query import ESQuery
 
@@ -272,14 +347,19 @@
                 }
             }
         }
         docs = await model_nested.search(query)
         assert len(docs) == 1
         assert docs[0].f_nested.f_str == 'nested_test2'
 
+        # Should include private fields
+        assert docs[0]._version == 1
+        assert docs[0]._primary_term == 1
+        assert docs[0]._seq_no > 0
+
         # Search all started with nested_test
         query: 'ESQuery' = {
             'bool': {
                 'must': {
                     'prefix': {
                         'f_nested.f_str': 'nested_test'
                     }
```

