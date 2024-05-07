# Comparing `tmp/oaipmh_scythe-0.12.1.tar.gz` & `tmp/oaipmh_scythe-0.13.0.tar.gz`

## Comparing `oaipmh_scythe-0.12.1.tar` & `oaipmh_scythe-0.13.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    12092 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/CHANGELOG.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/docs/src/changelog.md
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/docs/src/contributing.md
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/docs/src/customizing.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/docs/src/index.md
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/docs/src/license.md
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/docs/src/oaipmh.md
--rw-r--r--   0        0        0    11441 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/docs/src/tutorial.md
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/docs/src/api/client.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/docs/src/api/exceptions.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/docs/src/api/iterator.md
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/docs/src/api/models.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/docs/src/api/response.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/docs/src/api/utils.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/src/oaipmh_scythe/__about__.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/src/oaipmh_scythe/__init__.py
--rw-r--r--   0        0        0    18229 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/src/oaipmh_scythe/client.py
--rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/src/oaipmh_scythe/exceptions.py
--rw-r--r--   0        0        0     8881 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/src/oaipmh_scythe/iterator.py
--rw-r--r--   0        0        0    11670 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/src/oaipmh_scythe/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/src/oaipmh_scythe/py.typed
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/src/oaipmh_scythe/response.py
--rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/src/oaipmh_scythe/utils.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/.gitignore
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/AUTHORS.md
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/LICENSE
--rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/README.md
--rw-r--r--   0        0        0     7408 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/pyproject.toml
--rw-r--r--   0        0        0     9275 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/PKG-INFO
+-rw-r--r--   0        0        0    12846 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/CHANGELOG.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/docs/src/changelog.md
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/docs/src/contributing.md
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/docs/src/customizing.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/docs/src/index.md
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/docs/src/license.md
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/docs/src/oaipmh.md
+-rw-r--r--   0        0        0    11442 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/docs/src/tutorial.md
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/docs/src/api/client.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/docs/src/api/exceptions.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/docs/src/api/iterator.md
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/docs/src/api/models.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/docs/src/api/response.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/docs/src/api/utils.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/src/oaipmh_scythe/__about__.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/src/oaipmh_scythe/__init__.py
+-rw-r--r--   0        0        0    18661 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/src/oaipmh_scythe/client.py
+-rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/src/oaipmh_scythe/exceptions.py
+-rw-r--r--   0        0        0     8881 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/src/oaipmh_scythe/iterator.py
+-rw-r--r--   0        0        0    11670 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/src/oaipmh_scythe/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/src/oaipmh_scythe/py.typed
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/src/oaipmh_scythe/response.py
+-rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/src/oaipmh_scythe/utils.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/.gitignore
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/AUTHORS.md
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/LICENSE
+-rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/README.md
+-rw-r--r--   0        0        0     7241 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/pyproject.toml
+-rw-r--r--   0        0        0     9378 2020-02-02 00:00:00.000000 oaipmh_scythe-0.13.0/PKG-INFO
```

### Comparing `oaipmh_scythe-0.12.1/CHANGELOG.md` & `oaipmh_scythe-0.13.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,31 @@
 
 All notable changes to this project will be documented in this file.
 
 This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html). See
 [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/) for commit guidelines.
 
 
-## [Unreleased](https://github.com/afuetterer/oaipmh-scythe/compare/0.12.1...main)
+## [Unreleased](https://github.com/afuetterer/oaipmh-scythe/compare/0.13.0...main)
 
 
 
+## [0.13.0](https://github.com/afuetterer/oaipmh-scythe/compare/0.12.1...0.13.0) (2024-05-07)
+
+### Features
+
+- **client:** make numeric arguments accept &#39;int | float&#39; (#366) ([`b53bbed`](https://github.com/afuetterer/oaipmh-scythe/commit/b53bbed65440f974b6c09b161a66a303fb57c3bd))
+
+### Documentation
+
+- **readme:** add codeql badge (#365) ([`eca3e3b`](https://github.com/afuetterer/oaipmh-scythe/commit/eca3e3b221bebdb47d72112c0e5f529298eadf77))
+- **tutorial:** fix typo (#353) ([`65f75b8`](https://github.com/afuetterer/oaipmh-scythe/commit/65f75b82515cc772d82cf745b8763cb291d3ff2a))
+- add references to exceptions in docstrings (#351) ([`4df8491`](https://github.com/afuetterer/oaipmh-scythe/commit/4df8491502bc65ae0589c6686b71756d205f4411))
+
+
 ## [0.12.1](https://github.com/afuetterer/oaipmh-scythe/compare/0.12.0...0.12.1) (2024-04-25)
 
 ### Bug Fixes
 
 - **exceptions:** rename nometadataformat to nometadataformats (#349) ([`255acb2`](https://github.com/afuetterer/oaipmh-scythe/commit/255acb257a35533e78b0eb1aed85704c386e4e0a))
 
 ### Code Refactoring
```

### Comparing `oaipmh_scythe-0.12.1/docs/src/customizing.md` & `oaipmh_scythe-0.13.0/docs/src/customizing.md`

 * *Files identical despite different names*

### Comparing `oaipmh_scythe-0.12.1/docs/src/oaipmh.md` & `oaipmh_scythe-0.13.0/docs/src/oaipmh.md`

 * *Files identical despite different names*

### Comparing `oaipmh_scythe-0.12.1/docs/src/tutorial.md` & `oaipmh_scythe-0.13.0/docs/src/tutorial.md`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 Start with a ListRecords request:
 
 ```python
 records = scythe.list_records()
 ```
 
 Note that all keyword arguments you provide to this function are passed to the OAI interface as HTTP parameters.
-Therefore, the example request would send the parameter `verb=ListRecord`.
+Therefore, the example request would send the parameter `verb=ListRecords`.
 
 ## Performing Selective Harvesting
 
 ### Harvesting Records Based on Publication Date
 
 To selectively harvest records within a specific publication date range, the
 [list_records()][oaipmh_scythe.client.Scythe.list_records] and
```

### Comparing `oaipmh_scythe-0.12.1/src/oaipmh_scythe/__init__.py` & `oaipmh_scythe-0.13.0/src/oaipmh_scythe/__init__.py`

 * *Files identical despite different names*

### Comparing `oaipmh_scythe-0.12.1/src/oaipmh_scythe/client.py` & `oaipmh_scythe-0.13.0/src/oaipmh_scythe/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,35 +77,42 @@
     def __init__(
         self,
         endpoint: str,
         http_method: str = "GET",
         iterator: type[BaseOAIIterator] = OAIItemIterator,
         max_retries: int = 0,
         retry_status_codes: Iterable[int] | None = None,
-        default_retry_after: int = 60,
+        default_retry_after: int | float = 60,
         class_mapping: dict[str, type[OAIItem]] | None = None,
         encoding: str = "utf-8",
         auth: AuthTypes | None = None,
-        timeout: int = 60,
+        timeout: int | float = 60,
     ):
         self.endpoint = endpoint
         if http_method not in ("GET", "POST"):
             raise ValueError("Invalid HTTP method: %s! Must be GET or POST.")
         self.http_method = http_method
         if inspect.isclass(iterator) and issubclass(iterator, BaseOAIIterator):
             self.iterator = iterator
         else:
             raise TypeError("Argument 'iterator' must be subclass of %s" % BaseOAIIterator.__name__)
         self.max_retries = max_retries
         self.retry_status_codes = retry_status_codes or (503,)
+        if default_retry_after <= 0:
+            raise ValueError(
+                "Invalid value for 'default_retry_after': %s. default_retry_after must be positive int or float."
+                % default_retry_after
+            )
         self.default_retry_after = default_retry_after
         self.oai_namespace = OAI_NAMESPACE
         self.class_mapping = class_mapping or DEFAULT_CLASS_MAP
         self.encoding = encoding
         self.auth = auth
+        if timeout <= 0:
+            raise ValueError("Invalid value for 'timeout': %s. Timeout must be positive int or float." % timeout)
         self.timeout = timeout
         self._client: httpx.Client | None = None
 
     @property
     def client(self) -> httpx.Client:
         """Provide a reusable HTTP client instance for making requests.
 
@@ -158,15 +165,15 @@
         Args:
             query: A dictionary containing the request parameters.
 
         Returns:
             An OAIResponse object encapsulating the server's response.
 
         Raises:
-            HTTPError: If the HTTP request fails after the maximum number of retries.
+            httpx.HTTPError: If the HTTP request fails after the maximum number of retries.
         """
         http_response = self._request(query)
         for _ in range(self.max_retries):
             if httpx.codes.is_error(http_response.status_code) and http_response.status_code in self.retry_status_codes:
                 retry_after = self.get_retry_after(http_response)
                 logger.warning("HTTP %d! Retrying after %d seconds...", http_response.status_code, retry_after)
                 time.sleep(retry_after)
@@ -209,22 +216,23 @@
             until: An optional date string specifying the end of a date range for harvesting records.
             metadata_prefix: The metadata format for the records to be harvested. Defaults to "oai_dc".
             set_: An optional set identifier to restrict the harvest to records within a specific set.
             resumption_token: An optional token for pagination, used to continue a request for the next page of records.
             ignore_deleted: If True, skip records flagged as deleted in the response.
 
         Yields:
-            An iterator over OAIResponse or Record objects, each representing an individual record or response from the server.
+            An iterator over OAIResponse or Record objects, each representing an individual record or response
+                from the server.
 
         Raises:
-            badArgument: If the arguments provided do not conform to the expectations of the OAI server.
-            badResumptionToken: If the provided resumption token is invalid or expired.
-            cannotDisseminateFormat: If the specified metadata_prefix is not supported by the OAI server.
-            noRecordsMatch: If no records match the provided criteria.
-            noSetHierarchy: If set-based harvesting is requested but the OAI server does not support sets.
+            BadArgument: If the arguments provided do not conform to the expectations of the OAI server.
+            BadResumptionToken: If the provided resumption token is invalid or expired.
+            CannotDisseminateFormat: If the specified metadata_prefix is not supported by the OAI server.
+            NoRecordsMatch: If no records match the provided criteria.
+            NoSetHierarchy: If set-based harvesting is requested but the OAI server does not support sets.
 
         """
         _query = {
             "verb": "ListRecords",
             "from": from_,
             "until": until,
             "metadataPrefix": metadata_prefix,
@@ -252,26 +260,27 @@
         Ref: <https://openarchives.org/OAI/openarchivesprotocol.html#ListIdentifiers>
 
         Args:
             from_: An optional date string specifying the start of a date range for harvesting records.
             until: An optional date string specifying the end of a date range for harvesting records.
             metadata_prefix: The metadata format for the records to be harvested. Defaults to "oai_dc".
             set_: An optional set identifier to restrict the harvest to records within a specific set.
-            resumption_token: An optional token for pagination, used to continue a request for the next page of identifiers.
+            resumption_token: An optional token for pagination, used to continue a request for the next page of
+                identifiers.
             ignore_deleted: If True, skip records flagged as deleted in the response.
 
         Yields:
             An iterator over OAIResponse or Header objects, each representing an individual record identifier
                 or response from the server.
 
         Raises:
-            badResumptionToken: If the provided resumption token is invalid or expired.
-            cannotDisseminateFormat: If the specified metadata_prefix is not supported by the OAI server.
-            noRecordsMatch: If no records match the provided criteria.
-            noSetHierarchy: If set-based harvesting is requested but the OAI server does not support sets.
+            BadResumptionToken: If the provided resumption token is invalid or expired.
+            CannotDisseminateFormat: If the specified metadata_prefix is not supported by the OAI server.
+            NoRecordsMatch: If no records match the provided criteria.
+            NoSetHierarchy: If set-based harvesting is requested but the OAI server does not support sets.
 
         """
         _query = {
             "verb": "ListIdentifiers",
             "from": from_,
             "until": until,
             "metadataPrefix": metadata_prefix,
@@ -294,16 +303,16 @@
         Args:
             resumption_token: An optional token for pagination, used to continue a request for the next batch of sets.
 
         Yields:
             An iterator over OAIResponse or Set objects, representing an individual set or response from the server.
 
         Raises:
-            badResumptionToken: If the provided resumption token is invalid or expired.
-            noSetHierarchy: If the OAI server does not support sets or has no set hierarchy available.
+            BadResumptionToken: If the provided resumption token is invalid or expired.
+            NoSetHierarchy: If the OAI server does not support sets or has no set hierarchy available.
 
         """
         _query = {
             "verb": "ListSets",
             "resumptionToken": resumption_token,
         }
         query = remove_none_values(filter_dict_except_resumption_token(_query))
@@ -315,16 +324,16 @@
         Send a request to identify the OAI server and retrieve its information. This includes details such as the repository name,
         the base URL, the protocol version, and other relevant data about the OAI server. It's useful for understanding the
         capabilities and configuration of the server.
 
         Ref: <https://openarchives.org/OAI/openarchivesprotocol.html#Identify>
 
         Returns:
-            Identify: An object encapsulating the server's identify response, which contains various pieces of information
-            about the OAI server.
+            An object encapsulating the server's identify response, which contains various pieces of information about
+                the OAI server.
 
         """
         query = {"verb": "Identify"}
         return Identify(self.harvest(query))
 
     def get_record(self, identifier: str, metadata_prefix: str = "oai_dc") -> OAIResponse | Record:
         """Issue a GetRecord request to the OAI server.
@@ -340,17 +349,17 @@
             identifier: A unique identifier for the record to be retrieved from the OAI server.
             metadata_prefix: The metadata format to be returned for the record. Defaults to "oai_dc".
 
         Returns:
             An OAIResponse or Record object representing the requested record.
 
         Raises:
-            cannotDisseminateFormat: If the specified metadata_prefix is not supported by the OAI server
-                for the requested record.
-            idDoesNotExist: If the specified identifier does not correspond to any record in the OAI server.
+            CannotDisseminateFormat: If the specified metadata_prefix is not supported by the OAI server for
+                the requested record.
+            IdDoesNotExist: If the specified identifier does not correspond to any record in the OAI server.
 
         """
         query = {
             "verb": "GetRecord",
             "identifier": identifier,
             "metadataPrefix": metadata_prefix,
         }
@@ -368,29 +377,29 @@
 
         Args:
             identifier: An optional unique identifier for a specific record to query available metadata formats.
                         If None, all metadata formats available in the repository are listed.
 
         Yields:
             An iterator over OAIResponse or MetadataFormat objects, each representing an individual metadata format
-            or response from the server.
+                or response from the server.
 
         Raises:
-            idDoesNotExist: If the specified identifier does not correspond to any record in the OAI server.
-            noMetadataFormats: If there are no metadata formats available for the requested record or repository.
+            IdDoesNotExist: If the specified identifier does not correspond to any record in the OAI server.
+            NoMetadataFormats: If there are no metadata formats available for the requested record or repository.
 
         """
         _query = {
             "verb": "ListMetadataFormats",
             "identifier": identifier,
         }
         query = remove_none_values(_query)
         yield from self.iterator(self, query)
 
-    def get_retry_after(self, http_response: httpx.Response) -> int:
+    def get_retry_after(self, http_response: httpx.Response) -> int | float:
         """Determine the appropriate time to wait before retrying a request, based on the server's response.
 
         Check the status code of the provided HTTP response. If it's 503 (Service Unavailable),
         attempt to parse the 'retry-after' header to find the suggested wait time. If parsing fails
         or a different status code is received, use the default retry time.
 
         Args:
```

### Comparing `oaipmh_scythe-0.12.1/src/oaipmh_scythe/exceptions.py` & `oaipmh_scythe-0.13.0/src/oaipmh_scythe/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     GeneralOAIPMHError: A general exception class for OAI-PMH errors not specifically covered by other classes.
     BadArgument: Raised when a request contains illegal, missing, or improperly formatted arguments.
     BadVerb: Raised when the verb argument in a request is invalid or improperly used.
     BadResumptionToken: Raised when a resumption token is invalid or expired.
     CannotDisseminateFormat: Raised when a requested metadata format is not supported.
     IdDoesNotExist: Raised when an identifier does not exist or is illegal in a repository.
     NoSetHierarchy: Raised when a repository does not support set hierarchies.
-    NoMetadataFormat: Raised when no metadata formats are available for an item.
+    NoMetadataFormats: Raised when no metadata formats are available for an item.
     NoRecordsMatch: Raised when a query yields no results due to specific argument combinations.
 
 These custom exceptions enhance the robustness and clarity of error handling in OAI-PMH client implementations,
 aligning closely with the protocol's standard error conditions.
 
 Ref: https://openarchives.org/OAI/openarchivesprotocol.html#ErrorConditions
 """
```

### Comparing `oaipmh_scythe-0.12.1/src/oaipmh_scythe/iterator.py` & `oaipmh_scythe-0.13.0/src/oaipmh_scythe/iterator.py`

 * *Files identical despite different names*

### Comparing `oaipmh_scythe-0.12.1/src/oaipmh_scythe/models.py` & `oaipmh_scythe-0.13.0/src/oaipmh_scythe/models.py`

 * *Files identical despite different names*

### Comparing `oaipmh_scythe-0.12.1/src/oaipmh_scythe/response.py` & `oaipmh_scythe-0.13.0/src/oaipmh_scythe/response.py`

 * *Files identical despite different names*

### Comparing `oaipmh_scythe-0.12.1/src/oaipmh_scythe/utils.py` & `oaipmh_scythe-0.13.0/src/oaipmh_scythe/utils.py`

 * *Files identical despite different names*

### Comparing `oaipmh_scythe-0.12.1/.gitignore` & `oaipmh_scythe-0.13.0/.gitignore`

 * *Files identical despite different names*

### Comparing `oaipmh_scythe-0.12.1/LICENSE` & `oaipmh_scythe-0.13.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oaipmh_scythe-0.12.1/README.md` & `oaipmh_scythe-0.13.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # oaipmh-scythe: A Scythe for harvesting OAI-PMH repositories.
 
 Welcome to `oaipmh-scythe`, an updated and modernized version of the original
 [sickle](https://github.com/mloesch/sickle), now with additional features and ongoing maintenance.
 
-| __CI__      | [![pre-commit.ci status][pre-commit-ci-badge]][pre-commit-ci-status] [![ci][ci-badge]][ci-workflow] [![coverage][coverage-badge]][ci-workflow]                                                                                        |
+| __CI__      | [![pre-commit.ci status][pre-commit-ci-badge]][pre-commit-ci-status] [![ci][ci-badge]][ci-workflow] [![coverage][coverage-badge]][ci-workflow] [![codeql][codeql-badge]][codeql-workflow]                                             |
 | :---------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
 | __Docs__    | [![docs][docs-badge]][docs-workflow]                                                                                                                                                                                                  |
 | __Package__ | [![pypi-version][pypi-version-badge]][pypi-url] [![pypi-python-versions][pypi-python-versions-badge]][pypi-url] [![all-downloads][all-downloads-badge]][pepy-tech-url] [![monthly-downloads][monthly-downloads-badge]][pepy-tech-url] |
 | __Meta__    | [![OpenSSF Scorecard][scorecard-badge]][scorecard-url] [![hatch][hatch-badge]][hatch] [![ruff][ruff-badge]][ruff] [![mypy][mypy-badge]][mypy] [![License][license-badge]][license]                                                    |
 
 `oaipmh-scythe` is a lightweight [OAI-PMH](http://www.openarchives.org/OAI/openarchivesprotocol.html) client library
 written in Python. It has been designed for conveniently retrieving data from OAI interfaces the Pythonic way:
@@ -78,14 +78,16 @@
 `oaipmh-scythe` is distributed under the terms of the [BSD license](https://spdx.org/licenses/BSD-3-Clause.html).
 
 <!-- Refs -->
 
 [all-downloads-badge]: https://static.pepy.tech/badge/oaipmh-scythe
 [ci-badge]: https://github.com/afuetterer/oaipmh-scythe/actions/workflows/main.yml/badge.svg
 [ci-workflow]: https://github.com/afuetterer/oaipmh-scythe/actions/workflows/main.yml
+[codeql-badge]: https://github.com/afuetterer/oaipmh-scythe/actions/workflows/codeql.yml/badge.svg
+[codeql-workflow]: https://github.com/afuetterer/oaipmh-scythe/actions/workflows/codeql.yml
 [coverage-badge]: https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/afuetterer/fcb87d45f4d7defdfeffa65eb1d65f63/raw/coverage-badge.json
 [docs-badge]: https://github.com/afuetterer/oaipmh-scythe/actions/workflows/docs.yml/badge.svg
 [docs-url]: https://afuetterer.github.io/oaipmh-scythe
 [docs-workflow]: https://github.com/afuetterer/oaipmh-scythe/actions/workflows/docs.yml
 [hatch]: https://github.com/pypa/hatch
 [hatch-badge]: https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg
 [license]: https://spdx.org/licenses/BSD-3-Clause.html
```

### Comparing `oaipmh_scythe-0.12.1/pyproject.toml` & `oaipmh_scythe-0.13.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -42,17 +42,14 @@
 ]
 docs = [
   "mkdocs~=1.5",
   "mkdocs-include-markdown-plugin~=6.0",
   "mkdocs-material~=9.5",
   "mkdocstrings[python]~=0.24",
 ]
-release = [
-  "python-semantic-release~=9.1",
-]
 test = [
   "pytest~=8.0",
   "pytest-cov~=5.0",
   "pytest-mock~=3.12",
   "pytest-randomly~=3.15",
   "pytest-recording~=0.13",
   "pytest-xdist~=3.5",
@@ -79,14 +76,15 @@
 [tool.hatch.build.targets.wheel]
 packages = ["src/oaipmh_scythe"]
 
 [tool.hatch.version]
 path = "src/oaipmh_scythe/__about__.py"
 
 [tool.hatch.envs.default]
+installer = "uv"
 features = ["dev", "test"]
 post-install-commands = ["pre-commit install"]
 [tool.hatch.envs.default.scripts]
 check = ["lint", "typecheck"]
 lint = "SKIP=mypy pre-commit run --all-files --color=always --show-diff-on-failure"
 typecheck = "pre-commit run --all-files --color=always --show-diff-on-failure mypy"
 test = "pytest {args:tests}"
@@ -101,25 +99,14 @@
 features = ["docs"]
 template = "docs"
 [tool.hatch.envs.docs.scripts]
 build = "mkdocs build --config-file=docs/mkdocs.yml"
 serve = "mkdocs serve --verbose --config-file=docs/mkdocs.yml"
 deploy = "mkdocs gh-deploy --force --config-file=docs/mkdocs.yml"
 
-[tool.hatch.envs.release]
-features = ["release"]
-template = "release"
-[tool.hatch.envs.release.scripts]
-next-version = "semantic-release version --print"
-update-citation = """
-  sed -i "s/^version: .*/version: $(semantic-release version --print)/" CITATION.cff
-  sed -i "s/^date-released: .*/date-released: $(date "+%Y-%m-%d")/" CITATION.cff
-  cat CITATION.cff
-"""
-
 # ruff
 # Ref: https://docs.astral.sh/ruff/configuration/
 # ------------------------------------------------------------------------------
 
 [tool.ruff]
 line-length = 120
 src = ["src", "tests"]
@@ -245,23 +232,26 @@
 format = "ansi"
 
 # python-semantic-release
 # Ref: https://python-semantic-release.readthedocs.io/en/latest/configuration.html#settings
 # ------------------------------------------------------------------------------
 
 [tool.semantic_release]
+commit_author = "github-actions[bot] <41898282+github-actions[bot]@users.noreply.github.com>"
 commit_message = "chore: release {version}\n\nAutomatically generated by python-semantic-release [skip ci]"
-logging_use_named_masks = true
 major_on_zero = false
 tag_format = "{version}"
 version_variables = [
   "src/oaipmh_scythe/__about__.py:__version__",
 ]
+assets = ["CITATION.cff"]
 build_command = """
-python -m pip install build[uv]
+sed -i "s/^version: .*/version: $NEW_VERSION/" CITATION.cff
+sed -i "s/^date-released: .*/date-released: $(date "+%Y-%m-%d")/" CITATION.cff
+python -m pip install "build[uv]"
 python -m build --installer=uv
 """
 changelog.template_dir = ".github/templates"
 changelog.environment.keep_trailing_newline = true
 
 # typos
 # Ref: https://github.com/crate-ci/typos/blob/master/docs/reference.md
```

### Comparing `oaipmh_scythe-0.12.1/PKG-INFO` & `oaipmh_scythe-0.13.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: oaipmh-scythe
-Version: 0.12.1
+Version: 0.13.0
 Summary: A Scythe for harvesting OAI-PMH repositories.
 Project-URL: Changelog, https://github.com/afuetterer/oaipmh-scythe/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://afuetterer.github.io/oaipmh-scythe
 Project-URL: Issues, https://github.com/afuetterer/oaipmh-scythe/issues
 Project-URL: Repository, https://github.com/afuetterer/oaipmh-scythe.git
 Author: Heinz-Alexander Fütterer
 License: BSD-3-Clause
@@ -28,16 +28,14 @@
 Provides-Extra: dev
 Requires-Dist: pre-commit~=3.6; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: mkdocs-include-markdown-plugin~=6.0; extra == 'docs'
 Requires-Dist: mkdocs-material~=9.5; extra == 'docs'
 Requires-Dist: mkdocstrings[python]~=0.24; extra == 'docs'
 Requires-Dist: mkdocs~=1.5; extra == 'docs'
-Provides-Extra: release
-Requires-Dist: python-semantic-release~=9.1; extra == 'release'
 Provides-Extra: test
 Requires-Dist: pytest-cov~=5.0; extra == 'test'
 Requires-Dist: pytest-mock~=3.12; extra == 'test'
 Requires-Dist: pytest-randomly~=3.15; extra == 'test'
 Requires-Dist: pytest-recording~=0.13; extra == 'test'
 Requires-Dist: pytest-xdist~=3.5; extra == 'test'
 Requires-Dist: pytest~=8.0; extra == 'test'
@@ -45,15 +43,15 @@
 Description-Content-Type: text/markdown
 
 # oaipmh-scythe: A Scythe for harvesting OAI-PMH repositories.
 
 Welcome to `oaipmh-scythe`, an updated and modernized version of the original
 [sickle](https://github.com/mloesch/sickle), now with additional features and ongoing maintenance.
 
-| __CI__      | [![pre-commit.ci status][pre-commit-ci-badge]][pre-commit-ci-status] [![ci][ci-badge]][ci-workflow] [![coverage][coverage-badge]][ci-workflow]                                                                                        |
+| __CI__      | [![pre-commit.ci status][pre-commit-ci-badge]][pre-commit-ci-status] [![ci][ci-badge]][ci-workflow] [![coverage][coverage-badge]][ci-workflow] [![codeql][codeql-badge]][codeql-workflow]                                             |
 | :---------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
 | __Docs__    | [![docs][docs-badge]][docs-workflow]                                                                                                                                                                                                  |
 | __Package__ | [![pypi-version][pypi-version-badge]][pypi-url] [![pypi-python-versions][pypi-python-versions-badge]][pypi-url] [![all-downloads][all-downloads-badge]][pepy-tech-url] [![monthly-downloads][monthly-downloads-badge]][pepy-tech-url] |
 | __Meta__    | [![OpenSSF Scorecard][scorecard-badge]][scorecard-url] [![hatch][hatch-badge]][hatch] [![ruff][ruff-badge]][ruff] [![mypy][mypy-badge]][mypy] [![License][license-badge]][license]                                                    |
 
 `oaipmh-scythe` is a lightweight [OAI-PMH](http://www.openarchives.org/OAI/openarchivesprotocol.html) client library
 written in Python. It has been designed for conveniently retrieving data from OAI interfaces the Pythonic way:
@@ -124,14 +122,16 @@
 `oaipmh-scythe` is distributed under the terms of the [BSD license](https://spdx.org/licenses/BSD-3-Clause.html).
 
 <!-- Refs -->
 
 [all-downloads-badge]: https://static.pepy.tech/badge/oaipmh-scythe
 [ci-badge]: https://github.com/afuetterer/oaipmh-scythe/actions/workflows/main.yml/badge.svg
 [ci-workflow]: https://github.com/afuetterer/oaipmh-scythe/actions/workflows/main.yml
+[codeql-badge]: https://github.com/afuetterer/oaipmh-scythe/actions/workflows/codeql.yml/badge.svg
+[codeql-workflow]: https://github.com/afuetterer/oaipmh-scythe/actions/workflows/codeql.yml
 [coverage-badge]: https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/afuetterer/fcb87d45f4d7defdfeffa65eb1d65f63/raw/coverage-badge.json
 [docs-badge]: https://github.com/afuetterer/oaipmh-scythe/actions/workflows/docs.yml/badge.svg
 [docs-url]: https://afuetterer.github.io/oaipmh-scythe
 [docs-workflow]: https://github.com/afuetterer/oaipmh-scythe/actions/workflows/docs.yml
 [hatch]: https://github.com/pypa/hatch
 [hatch-badge]: https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg
 [license]: https://spdx.org/licenses/BSD-3-Clause.html
```

