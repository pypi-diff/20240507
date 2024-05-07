# Comparing `tmp/langchain_google_spanner-0.2.1-py3-none-any.whl.zip` & `tmp/langchain_google_spanner-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 28224 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1137 b- defN 24-Mar-06 22:42 langchain_google_spanner/__init__.py
--rw-r--r--  2.0 unx     9711 b- defN 24-Mar-06 22:42 langchain_google_spanner/chat_message_history.py
--rw-r--r--  2.0 unx    17168 b- defN 24-Mar-06 22:42 langchain_google_spanner/loader.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Mar-06 22:42 langchain_google_spanner/py.typed
--rw-r--r--  2.0 unx    45049 b- defN 24-Mar-06 22:42 langchain_google_spanner/vector_store.py
--rw-r--r--  2.0 unx      597 b- defN 24-Mar-06 22:42 langchain_google_spanner/version.py
--rw-rw-r--  2.0 unx    11358 b- defN 24-Mar-06 22:44 langchain_google_spanner-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    18357 b- defN 24-Mar-06 22:44 langchain_google_spanner-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-06 22:44 langchain_google_spanner-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       25 b- defN 24-Mar-06 22:44 langchain_google_spanner-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1039 b- defN 24-Mar-06 22:44 langchain_google_spanner-0.2.1.dist-info/RECORD
-11 files, 104533 bytes uncompressed, 26426 bytes compressed:  74.7%
+Zip file size: 28366 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1137 b- defN 24-May-07 17:25 langchain_google_spanner/__init__.py
+-rw-r--r--  2.0 unx     9697 b- defN 24-May-07 17:25 langchain_google_spanner/chat_message_history.py
+-rw-r--r--  2.0 unx    17168 b- defN 24-May-07 17:25 langchain_google_spanner/loader.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-07 17:25 langchain_google_spanner/py.typed
+-rw-r--r--  2.0 unx    45114 b- defN 24-May-07 17:25 langchain_google_spanner/vector_store.py
+-rw-r--r--  2.0 unx      597 b- defN 24-May-07 17:25 langchain_google_spanner/version.py
+-rw-rw-r--  2.0 unx    11358 b- defN 24-May-07 17:26 langchain_google_spanner-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    19523 b- defN 24-May-07 17:26 langchain_google_spanner-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-07 17:26 langchain_google_spanner-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       25 b- defN 24-May-07 17:26 langchain_google_spanner-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1039 b- defN 24-May-07 17:26 langchain_google_spanner-0.3.0.dist-info/RECORD
+11 files, 105750 bytes uncompressed, 26568 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: langchain_google_spanner/vector_store.py
 Comment: 
 
 Filename: langchain_google_spanner/version.py
 Comment: 
 
-Filename: langchain_google_spanner-0.2.1.dist-info/LICENSE
+Filename: langchain_google_spanner-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: langchain_google_spanner-0.2.1.dist-info/METADATA
+Filename: langchain_google_spanner-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: langchain_google_spanner-0.2.1.dist-info/WHEEL
+Filename: langchain_google_spanner-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: langchain_google_spanner-0.2.1.dist-info/top_level.txt
+Filename: langchain_google_spanner-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: langchain_google_spanner-0.2.1.dist-info/RECORD
+Filename: langchain_google_spanner-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langchain_google_spanner/chat_message_history.py

```diff
@@ -129,24 +129,24 @@
                 )
 
     @staticmethod
     def create_chat_history_table(
         instance_id: str,
         database_id: str,
         table_name: str,
-        client: spanner.Client = spanner.Client(),
+        client: Optional[spanner.Client] = None,
     ) -> None:
         """
         Create a chat history table in a Cloud Spanner database.
 
         Args:
             instance_id (str): The ID of the Cloud Spanner instance.
             database_id (str): The ID of the Cloud Spanner database.
             table_name (str): The name of the table to be created.
-            client (spanner.Client, optional): An instance of the Cloud Spanner client. Defaults to spanner.Client().
+            client (spanner.Client, optional): An instance of the Cloud Spanner client. Defaults to None.
 
         Raises:
             Exception: If the specified instance or database does not exist.
 
         Returns:
             Operation: The operation to create the table.
         """
```

## langchain_google_spanner/vector_store.py

```diff
@@ -272,15 +272,15 @@
     """
 
     @staticmethod
     def init_vector_store_table(
         instance_id: str,
         database_id: str,
         table_name: str,
-        client: spanner.Client = spanner.Client(),
+        client: Optional[spanner.Client] = None,
         id_column: Union[str, TableColumn] = ID_COLUMN_NAME,
         content_column: str = CONTENT_COLUMN_NAME,
         embedding_column: str = EMBEDDING_COLUMN_NAME,
         metadata_columns: Optional[List[TableColumn]] = None,
         primary_key: Optional[str] = None,
         vector_size: Optional[int] = None,
         secondary_indexes: Optional[List[SecondaryIndex]] = None,
@@ -296,14 +296,15 @@
         - id_column (str): The name of the row ID column. Defaults to ID_COLUMN_NAME.
         - content_column (str): The name of the content column. Defaults to CONTENT_COLUMN_NAME.
         - embedding_column (str): The name of the embedding column. Defaults to EMBEDDING_COLUMN_NAME.
         - metadata_columns (Optional[List[Tuple]]): List of tuples containing metadata column information. Defaults to None.
         - vector_size (Optional[int]): The size of the vector. Defaults to None.
         """
 
+        client = client_with_user_agent(client, USER_AGENT_VECTOR_STORE)
         instance = client.instance(instance_id)
 
         if not instance.exists():
             raise Exception("Instance with id:  {} doesn't exist.".format(instance_id))
 
         database = instance.database(database_id)
 
@@ -442,15 +443,15 @@
         instance_id: str,
         database_id: str,
         table_name: str,
         embedding_service: Embeddings,
         id_column: str = ID_COLUMN_NAME,
         content_column: str = CONTENT_COLUMN_NAME,
         embedding_column: str = EMBEDDING_COLUMN_NAME,
-        client: spanner.Client = spanner.Client(),
+        client: Optional[spanner.Client] = None,
         metadata_columns: Optional[List[str]] = None,
         ignore_metadata_columns: Optional[List[str]] = None,
         metadata_json_column: Optional[str] = None,
         query_parameters: QueryParameters = QueryParameters(),
     ):
         """
         Initialize the SpannerVectorStore.
@@ -1105,15 +1106,15 @@
         instance_id: str,
         database_id: str,
         table_name: str,
         id_column: str = ID_COLUMN_NAME,
         content_column: str = CONTENT_COLUMN_NAME,
         embedding_column: str = EMBEDDING_COLUMN_NAME,
         ids: Optional[List[str]] = None,
-        client: spanner.Client = spanner.Client(),
+        client: Optional[spanner.Client] = None,
         metadata_columns: Optional[List[str]] = None,
         ignore_metadata_columns: Optional[List[str]] = None,
         metadata_json_column: Optional[str] = None,
         query_parameter: QueryParameters = QueryParameters(),
         **kwargs: Any,
     ) -> SpannerVectorStore:
         """
@@ -1166,15 +1167,15 @@
         database_id: str,
         table_name: str,
         metadatas: Optional[List[dict]] = None,
         id_column: str = ID_COLUMN_NAME,
         content_column: str = CONTENT_COLUMN_NAME,
         embedding_column: str = EMBEDDING_COLUMN_NAME,
         ids: Optional[List[str]] = None,
-        client: spanner.Client = spanner.Client(),
+        client: Optional[spanner.Client] = None,
         metadata_columns: Optional[List[str]] = None,
         ignore_metadata_columns: Optional[List[str]] = None,
         metadata_json_column: Optional[str] = None,
         query_parameter: QueryParameters = QueryParameters(),
         **kwargs: Any,
     ) -> SpannerVectorStore:
         """
```

## langchain_google_spanner/version.py

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.2.1"
+__version__ = "0.3.0"
```

## Comparing `langchain_google_spanner-0.2.1.dist-info/LICENSE` & `langchain_google_spanner-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langchain_google_spanner-0.2.1.dist-info/METADATA` & `langchain_google_spanner-0.3.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-google-spanner
-Version: 0.2.1
+Version: 0.3.0
 Summary: LangChain integrations for Google Cloud Spanner
 Author-email: Google LLC <googleapis-packages@google.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -206,142 +206,189 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/googleapis/langchain-google-spanner-python
 Project-URL: Repository, https://github.com/googleapis/langchain-google-spanner-python.git
 Project-URL: Bug Tracker, https://github.com/googleapis/langchain-google-spanner-python/issues
 Project-URL: Changelog, https://github.com/googleapis/langchain-google-spanner-python/blob/main/CHANGELOG.md
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: langchain-core <1.0.0,>=0.1.25
 Requires-Dist: langchain-community <1.0.0,>=0.0.18
 Requires-Dist: google-cloud-spanner <4.0.0,>=3.41.0
 Provides-Extra: test
-Requires-Dist: black[jupyter] ==23.12.0 ; extra == 'test'
+Requires-Dist: black[jupyter] ==23.12.1 ; extra == 'test'
 Requires-Dist: bs4 ==0.0.2 ; extra == 'test'
 Requires-Dist: isort ==5.13.2 ; extra == 'test'
-Requires-Dist: mypy ==1.7.1 ; extra == 'test'
+Requires-Dist: mypy ==1.10.0 ; extra == 'test'
 Requires-Dist: pytest ==7.4.4 ; extra == 'test'
-Requires-Dist: pytest-asyncio ==0.23.0 ; extra == 'test'
+Requires-Dist: pytest-asyncio ==0.23.6 ; extra == 'test'
 
-# Spanner for LangChain
+Spanner for LangChain
+=================================
 
-This package contains the [LangChain][langchain] integrations for Spanner.
+|preview| |pypi| |versions|
 
-> **🧪 Preview:** This feature is covered by the Pre-GA Offerings Terms of the Google Cloud Terms of Service. Please note that pre-GA products and features might have limited support, and changes to pre-GA products and features might not be compatible with other pre-GA versions. For more information, see the [launch stage descriptions](https://cloud.google.com/products#product-launch-stages)
+- `Client Library Documentation`_
+- `Product Documentation`_
 
-* [Documentation][docs]
-* [API Reference]()
+.. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
+   :target: https://cloud.google.com/products#product-launch-stages
+.. |pypi| image:: https://img.shields.io/pypi/v/langchain-google-spanner.svg
+   :target: https://pypi.org/project/langchain-google-spanner/
+.. |versions| image:: https://img.shields.io/pypi/pyversions/langchain-google-spanner.svg
+   :target: https://pypi.org/project/langchain-google-spanner/
+.. _Client Library Documentation: https://cloud.google.com/python/docs/reference/langchain-google-spanner/latest
+.. _Product Documentation: https://cloud.google.com/spanner
 
-## Getting Started
+Quick Start
+-----------
 
-In order to use this library, you first need to go through the following steps:
+In order to use this library, you first need to go through the following
+steps:
 
-1. [Select or create a Cloud Platform project.][project]
-2. [Enable billing for your project.][billing]
-3. [Enable the Google Cloud Spanner API.][api]
-4. [Setup Authentication.][auth]
+1. `Select or create a Cloud Platform project.`_
+2. `Enable billing for your project.`_
+3. `Enable the Google Cloud Spanner API.`_
+4. `Setup Authentication.`_
 
-### Installation
+.. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
+.. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
+.. _Enable the Google Cloud Spanner API.: https://console.cloud.google.com/flows/enableapi?apiid=spanner.googleapis.com
+.. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
-Install this library in a [`virtualenv`][venv] using pip. [`virtualenv`][venv] is a tool to
-create isolated Python environments. The basic problem it addresses is one of
-dependencies and versions, and indirectly permissions.
+Installation
+~~~~~~~~~~~~
 
-With [`virtualenv`][venv], it's possible to install this library without needing system
-install permissions, and without clashing with the installed system
-dependencies.
+Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to create isolated Python environments. The basic problem it addresses is
+one of dependencies and versions, and indirectly permissions.
 
-```bash
-pip install virtualenv
-virtualenv <your-env>
-source <your-env>/bin/activate
-<your-env>/bin/pip install langchain-google-spanner
-```
+With `virtualenv`_, it’s possible to install this library without needing system install permissions, and without clashing with the installed system dependencies.
 
-## Vector Store Usage
+.. _`virtualenv`: https://virtualenv.pypa.io/en/latest/
+
+Supported Python Versions
+^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Python >= 3.8
+
+Mac/Linux
+^^^^^^^^^
+
+.. code-block:: console
+
+   pip install virtualenv
+   virtualenv <your-env>
+   source <your-env>/bin/activate
+   <your-env>/bin/pip install langchain-google-spanner
+
+Windows
+^^^^^^^
+
+.. code-block:: console
+
+   pip install virtualenv
+   virtualenv <your-env>
+   <your-env>\Scripts\activate
+   <your-env>\Scripts\pip.exe install langchain-google-spanner
+
+Vector Store Usage
+~~~~~~~~~~~~~~~~~~~
 
 Use a vector store to store embedded data and perform vector search.
 
-```python
-from langchain_google_sapnner import SpannerVectorstore
-from langchain.embeddings import VertexAIEmbeddings
+.. code-block:: python
+
+    from langchain_google_sapnner import SpannerVectorstore
+    from langchain.embeddings import VertexAIEmbeddings
+
+    embeddings_service = VertexAIEmbeddings(model_name="textembedding-gecko@003")
+    vectorstore = SpannerVectorStore(
+        instance_id="my-instance",
+        database_id="my-database",
+        table_name="my-table",
+        embeddings=embedding_service
+    )
+
+See the full `Vector Store`_ tutorial.
 
-embeddings_service = VertexAIEmbeddings()
-vectorstore = SpannerVectorStore(
-    instance_id="my-instance",
-    database_id="my-database",
-    table_name="my-table",
-    embeddings=embedding_service
-)
-```
+.. _`Vector Store`: https://github.com/googleapis/langchain-google-spanner-python/blob/main/docs/vector_store.ipynb
 
-See the full [Vector Store][vectorstore] tutorial.
+Document Loader Usage
+~~~~~~~~~~~~~~~~~~~~~
 
-## Document Loader Usage
+Use a document loader to load data as LangChain ``Document``\ s.
 
-Use a document loader to load data as LangChain `Document`s.
+.. code-block:: python
 
-```python
-from langchain_google_spanner import SpannerLoader
+   from langchain_google_spanner import SpannerLoader
 
 
-loader = SpannerLoader(
-    instance_id="my-instance",
-    database_id="my-database",
-    query="SELECT * from my_table_name"
-)
-docs = loader.lazy_load()
-```
+    loader = SpannerLoader(
+        instance_id="my-instance",
+        database_id="my-database",
+        query="SELECT * from my_table_name"
+    )
+    docs = loader.lazy_load()
 
-See the full [Document Loader][loader] tutorial.
+See the full `Document Loader`_ tutorial.
 
-## Chat Message History Usage
+.. _`Document Loader`: https://github.com/googleapis/langchain-google-spanner-python/blob/main/docs/document_loader.ipynb
 
-Use `ChatMessageHistory` to store messages and provide conversation history to LLMs.
+Chat Message History Usage
+--------------------------
 
-```python
-from langchain_google_spanner import SpannerChatMessageHistory
+Use ``ChatMessageHistory`` to store messages and provide conversation
+history to LLMs.
 
+.. code:: python
 
-history = SpannerChatMessageHistory(
-    instance_id="my-instance",
-    database_id="my-database",
-    table_name="my_table_name",
-    session_id="my-session_id"
-)
-```
+   from langchain_google_spanner import SpannerChatMessageHistory
 
-See the full [Chat Message History][history] tutorial.
 
-## Contributing
+    history = SpannerChatMessageHistory(
+        instance_id="my-instance",
+        database_id="my-database",
+        table_name="my_table_name",
+        session_id="my-session_id"
+    )
+
+See the full `Chat Message History`_ tutorial.
+
+.. _`Chat Message History`: https://github.com/googleapis/langchain-google-spanner-python/blob/main/docs/chat_message_history.ipynb
+
+Contributions
+~~~~~~~~~~~~~
 
 Contributions to this library are always welcome and highly encouraged.
 
-See [CONTRIBUTING][contributing] for more information how to get started.
+See `CONTRIBUTING`_ for more information how to get started.
 
 Please note that this project is released with a Contributor Code of Conduct. By participating in
-this project you agree to abide by its terms. See [Code of Conduct][coc] for more
+this project you agree to abide by its terms. See `Code of Conduct`_ for more
 information.
 
-## License
+.. _`CONTRIBUTING`: https://github.com/googleapis/langchain-google-spanner-python/blob/main/CONTRIBUTING.md
+.. _`Code of Conduct`: https://github.com/googleapis/langchain-google-spanner-python/blob/main/CODE_OF_CONDUCT.md
+
+License
+-------
 
-Apache 2.0 - See [LICENSE][license] for more information.
+Apache 2.0 - See
+`LICENSE <https://github.com/googleapis/langchain-google-spanner-python/blob/main/LICENSE>`_
+for more information.
 
-## Disclaimer
+Disclaimer
+----------
 
 This is not an officially supported Google product.
 
-[project]: https://console.cloud.google.com/project
-[billing]: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-[api]: https://console.cloud.google.com/flows/enableapi?apiid=spanner.googleapis.com
-[auth]: https://googleapis.dev/python/google-api-core/latest/auth.html
-[venv]: https://virtualenv.pypa.io/en/latest/
-[vectorstore]: https://github.com/googleapis/langchain-google-spanner-python/tree/main/docs/vector_store.ipynb
-[loader]: https://github.com/googleapis/langchain-google-spanner-python/tree/main/docs/document_loader.ipynb
-[history]: https://github.com/googleapis/langchain-google-spanner-python/tree/main/docs/chat_message_history.ipynb
-[langchain]: https://github.com/langchain-ai/langchain
-[docs]: https://github.com/googleapis/langchain-google-spanner-python/tree/main/docs
-[license]: https://github.com/googleapis/langchain-google-spanner-python/tree/main/LICENSE
-[contributing]: https://github.com/googleapis/langchain-google-spanner-python/tree/main/CONTRIBUTING.md
-[coc]: https://github.com/googleapis/langchain-google-spanner-python/tree/main/CODE_OF_CONDUCT.md
```

## Comparing `langchain_google_spanner-0.2.1.dist-info/RECORD` & `langchain_google_spanner-0.3.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 langchain_google_spanner/__init__.py,sha256=OkwnZFkNvXB69ny8aj6H6SWIfFMlyMJDLN3lQoLdOfU,1137
-langchain_google_spanner/chat_message_history.py,sha256=R1HYIq5iN5mKxlVxeprQMLag7xbutlry4x6qra9H2WI,9711
+langchain_google_spanner/chat_message_history.py,sha256=DJ-uTsJjBYYlJw4jgmZCcC2hiYYkJLM0n5jTKESoUJY,9697
 langchain_google_spanner/loader.py,sha256=BJSSur_ZdB132K2CzU0_kD7vxOMn-qjwGmokLYx1x6c,17168
 langchain_google_spanner/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-langchain_google_spanner/vector_store.py,sha256=hJtpYUzyi0fdcuwK5KkK-PtkjZYmckHIanGmKTdPSyY,45049
-langchain_google_spanner/version.py,sha256=lal6j0-2qdxqYCLjy1FcTVeiboHQADADWfCBuVKcU3k,597
-langchain_google_spanner-0.2.1.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-langchain_google_spanner-0.2.1.dist-info/METADATA,sha256=KObTUxbPQpUlEHiH7yMIzR0gd44-SFClMHfZUuzQV9U,18357
-langchain_google_spanner-0.2.1.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-langchain_google_spanner-0.2.1.dist-info/top_level.txt,sha256=CrnecUOOApZ7uXTt6m7w1sVSYJ_qZZ3T_TQzPim2r8c,25
-langchain_google_spanner-0.2.1.dist-info/RECORD,,
+langchain_google_spanner/vector_store.py,sha256=rBq5QnqNsdO0BlkgyEBrWMVmS0AVxkXmiksY2OEB9rY,45114
+langchain_google_spanner/version.py,sha256=Bt9xmJb_aic5hHSb19XJI5LMnotdGjBnwcYbbCI4jfo,597
+langchain_google_spanner-0.3.0.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+langchain_google_spanner-0.3.0.dist-info/METADATA,sha256=8wYLvs3QIVpXNblYq9CRlKtPMvejMtAb68YlvkWI0-U,19523
+langchain_google_spanner-0.3.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+langchain_google_spanner-0.3.0.dist-info/top_level.txt,sha256=CrnecUOOApZ7uXTt6m7w1sVSYJ_qZZ3T_TQzPim2r8c,25
+langchain_google_spanner-0.3.0.dist-info/RECORD,,
```

