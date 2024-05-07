# Comparing `tmp/fabrictestbed-1.7.0b1.tar.gz` & `tmp/fabrictestbed-1.7.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-1.7.0b1.tar", last modified: Mon Apr 15 21:37:46 2024, max compression
+gzip compressed data, was "fabrictestbed-1.7.0b2.tar", last modified: Tue May  7 21:32:59 2024, max compression
```

## Comparing `fabrictestbed-1.7.0b1.tar` & `fabrictestbed-1.7.0b2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1806 2024-01-09 19:41:33.369979 fabrictestbed-1.7.0b1/.gitignore
--rw-r--r--   0        0        0     1071 2024-01-09 19:41:33.370192 fabrictestbed-1.7.0b1/LICENSE
--rw-r--r--   0        0        0       24 2024-01-09 19:41:33.370298 fabrictestbed-1.7.0b1/MANIFEST.in
--rw-r--r--   0        0        0     5603 2024-01-09 19:41:33.370450 fabrictestbed-1.7.0b1/README.md
--rw-r--r--   0        0        0       50 2024-04-15 21:37:10.772143 fabrictestbed-1.7.0b1/fabrictestbed/__init__.py
--rw-r--r--   0        0        0        0 2024-01-09 19:41:33.370692 fabrictestbed-1.7.0b1/fabrictestbed/cli/__init__.py
--rw-r--r--   0        0        0    24704 2024-01-09 19:41:33.370900 fabrictestbed-1.7.0b1/fabrictestbed/cli/cli.py
--rw-r--r--   0        0        0     1452 2024-01-09 19:41:33.371041 fabrictestbed-1.7.0b1/fabrictestbed/cli/exceptions.py
--rw-r--r--   0        0        0        0 2024-01-09 19:45:22.070471 fabrictestbed-1.7.0b1/fabrictestbed/external_api/__init__.py
--rw-r--r--   0        0        0    10820 2024-01-23 16:03:35.627515 fabrictestbed-1.7.0b1/fabrictestbed/external_api/core_api.py
--rw-r--r--   0        0        0     1914 2024-01-09 19:41:33.371186 fabrictestbed-1.7.0b1/fabrictestbed/slice_editor/__init__.py
--rw-r--r--   0        0        0      201 2024-01-09 19:41:33.371321 fabrictestbed-1.7.0b1/fabrictestbed/slice_manager/__init__.py
--rw-r--r--   0        0        0    30239 2024-04-15 21:37:10.779668 fabrictestbed-1.7.0b1/fabrictestbed/slice_manager/slice_manager.py
--rw-r--r--   0        0        0        0 2024-01-09 19:41:33.371679 fabrictestbed-1.7.0b1/fabrictestbed/util/__init__.py
--rw-r--r--   0        0        0     1713 2024-01-09 20:14:27.091289 fabrictestbed-1.7.0b1/fabrictestbed/util/constants.py
--rw-r--r--   0        0        0     3275 2024-01-21 19:21:10.034009 fabrictestbed-1.7.0b1/fabrictestbed/util/utils.py
--rw-r--r--   0        0        0     1102 2024-04-15 21:37:10.786478 fabrictestbed-1.7.0b1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-09 19:41:33.372122 fabrictestbed-1.7.0b1/test/__init__.py
--rw-r--r--   0        0        0     2210 2024-01-09 19:41:33.372285 fabrictestbed-1.7.0b1/test/test_cli.py
--rw-r--r--   0        0        0     6573 1970-01-01 00:00:00.000000 fabrictestbed-1.7.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1806 2024-01-09 19:41:33.369979 fabrictestbed-1.7.0b2/.gitignore
+-rw-r--r--   0        0        0     1071 2024-01-09 19:41:33.370192 fabrictestbed-1.7.0b2/LICENSE
+-rw-r--r--   0        0        0       24 2024-01-09 19:41:33.370298 fabrictestbed-1.7.0b2/MANIFEST.in
+-rw-r--r--   0        0        0     5603 2024-01-09 19:41:33.370450 fabrictestbed-1.7.0b2/README.md
+-rw-r--r--   0        0        0       50 2024-04-17 15:18:33.125607 fabrictestbed-1.7.0b2/fabrictestbed/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-09 19:41:33.370692 fabrictestbed-1.7.0b2/fabrictestbed/cli/__init__.py
+-rw-r--r--   0        0        0    24704 2024-01-09 19:41:33.370900 fabrictestbed-1.7.0b2/fabrictestbed/cli/cli.py
+-rw-r--r--   0        0        0     1452 2024-01-09 19:41:33.371041 fabrictestbed-1.7.0b2/fabrictestbed/cli/exceptions.py
+-rw-r--r--   0        0        0        0 2024-01-09 19:45:22.070471 fabrictestbed-1.7.0b2/fabrictestbed/external_api/__init__.py
+-rw-r--r--   0        0        0    10820 2024-01-23 16:03:35.627515 fabrictestbed-1.7.0b2/fabrictestbed/external_api/core_api.py
+-rw-r--r--   0        0        0     1914 2024-01-09 19:41:33.371186 fabrictestbed-1.7.0b2/fabrictestbed/slice_editor/__init__.py
+-rw-r--r--   0        0        0      201 2024-01-09 19:41:33.371321 fabrictestbed-1.7.0b2/fabrictestbed/slice_manager/__init__.py
+-rw-r--r--   0        0        0    30257 2024-04-17 15:18:33.111519 fabrictestbed-1.7.0b2/fabrictestbed/slice_manager/slice_manager.py
+-rw-r--r--   0        0        0        0 2024-01-09 19:41:33.371679 fabrictestbed-1.7.0b2/fabrictestbed/util/__init__.py
+-rw-r--r--   0        0        0     1713 2024-01-09 20:14:27.091289 fabrictestbed-1.7.0b2/fabrictestbed/util/constants.py
+-rw-r--r--   0        0        0     3275 2024-01-21 19:21:10.034009 fabrictestbed-1.7.0b2/fabrictestbed/util/utils.py
+-rw-r--r--   0        0        0     1102 2024-04-17 15:18:33.116642 fabrictestbed-1.7.0b2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-09 19:41:33.372122 fabrictestbed-1.7.0b2/test/__init__.py
+-rw-r--r--   0        0        0     2210 2024-01-09 19:41:33.372285 fabrictestbed-1.7.0b2/test/test_cli.py
+-rw-r--r--   0        0        0     6573 1970-01-01 00:00:00.000000 fabrictestbed-1.7.0b2/PKG-INFO
```

### Comparing `fabrictestbed-1.7.0b1/.gitignore` & `fabrictestbed-1.7.0b2/.gitignore`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.7.0b1/LICENSE` & `fabrictestbed-1.7.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.7.0b1/README.md` & `fabrictestbed-1.7.0b2/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.7.0b1/fabrictestbed/cli/cli.py` & `fabrictestbed-1.7.0b2/fabrictestbed/cli/cli.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.7.0b1/fabrictestbed/cli/exceptions.py` & `fabrictestbed-1.7.0b2/fabrictestbed/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.7.0b1/fabrictestbed/external_api/core_api.py` & `fabrictestbed-1.7.0b2/fabrictestbed/external_api/core_api.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.7.0b1/fabrictestbed/slice_editor/__init__.py` & `fabrictestbed-1.7.0b2/fabrictestbed/slice_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.7.0b1/fabrictestbed/slice_manager/slice_manager.py` & `fabrictestbed-1.7.0b2/fabrictestbed/slice_manager/slice_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,16 +153,14 @@
                 self.tokens = json.loads(stream.read())
             refresh_token = self.get_refresh_token()
         else:
             # First time login, use environment variable to load the tokens
             refresh_token = os.environ.get(Constants.CILOGON_REFRESH_TOKEN)
         # Renew the tokens to ensure any project_id changes are taken into account
         if refresh and self.auto_refresh:
-            if refresh_token is None:
-                raise SliceManagerException(f"Unable to refresh tokens: no refresh token found!")
             self.refresh_tokens(refresh_token=refresh_token)
 
     def get_refresh_token(self) -> str:
         """
         Get Refresh Token
         @return refresh token
         """
@@ -275,22 +273,23 @@
             cache_file_name = self.token_location
         status, exception = self.cm_proxy.clear_token_cache(file_name=cache_file_name)
         if status == CmStatus.OK:
             return Status.OK, None
         return Status.FAILURE, f"Failed to clear token cache: {Utils.extract_error_message(exception=exception)}"
 
     def create(self, *, slice_name: str, ssh_key: Union[str, List[str]], topology: ExperimentTopology = None,
-               slice_graph: str = None,
+               slice_graph: str = None, lease_start_time: str = None,
                lease_end_time: str = None) -> Tuple[Status, Union[SliceManagerException, List[Sliver]]]:
         """
         Create a slice
         @param slice_name slice name
         @param ssh_key SSH Key(s)
         @param topology Experiment topology
         @param slice_graph Slice Graph string
+        @param lease_start_time Lease Start Time
         @param lease_end_time Lease End Time
         @return Tuple containing Status and Exception/Json containing slivers created
         """
         if slice_name is None or not isinstance(slice_name, str) or ssh_key is None:
             return Status.INVALID_ARGUMENTS, SliceManagerException("Invalid arguments - slice_name or ssh key")
 
         if topology is not None and not isinstance(topology, ExperimentTopology):
@@ -302,15 +301,16 @@
         if lease_end_time is not None and not isinstance(lease_end_time, str):
             return Status.INVALID_ARGUMENTS, SliceManagerException("Invalid arguments - lease_end_time")
 
         try:
             if self.__should_renew():
                 self.__load_tokens()
             return self.oc_proxy.create(token=self.get_id_token(), slice_name=slice_name, ssh_key=ssh_key,
-                                        topology=topology, slice_graph=slice_graph, lease_end_time=lease_end_time)
+                                        topology=topology, slice_graph=slice_graph, lease_end_time=lease_end_time,
+                                        lease_start_time=lease_start_time)
         except Exception as e:
             error_message = Utils.extract_error_message(exception=e)
             return Status.FAILURE, SliceManagerException(error_message)
 
     def modify(self, *, slice_id: str, topology: ExperimentTopology = None,
                slice_graph: str = None) -> Tuple[Status, Union[SliceManagerException, List[Sliver]]]:
         """
```

### Comparing `fabrictestbed-1.7.0b1/fabrictestbed/util/constants.py` & `fabrictestbed-1.7.0b2/fabrictestbed/util/constants.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.7.0b1/fabrictestbed/util/utils.py` & `fabrictestbed-1.7.0b2/fabrictestbed/util/utils.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.7.0b1/pyproject.toml` & `fabrictestbed-1.7.0b2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 keywords = ["Swagger", "FABRIC Python Client Library with CLI"]
 
 requires-python = '>=3.9'
 dependencies = [
     "fabric_fss_utils>=1.5.1",
     "click",
     "fabric-credmgr-client==1.6.1",
-    "fabric-orchestrator-client==1.7.0b1",
+    "fabric-orchestrator-client==1.7.0b2",
     "paramiko"
     ]
 
 scripts = {"fabric-cli" = "fabrictestbed.cli.cli:cli"}
 
 [project.optional-dependencies]
 test = ["coverage>=4.0.3",
```

### Comparing `fabrictestbed-1.7.0b1/test/test_cli.py` & `fabrictestbed-1.7.0b2/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.7.0b1/PKG-INFO` & `fabrictestbed-1.7.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: fabrictestbed
-Version: 1.7.0b1
+Version: 1.7.0b2
 Summary: FABRIC Python Client Library with CLI
 Keywords: Swagger,FABRIC Python Client Library with CLI
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: fabric_fss_utils>=1.5.1
 Requires-Dist: click
 Requires-Dist: fabric-credmgr-client==1.6.1
-Requires-Dist: fabric-orchestrator-client==1.7.0b1
+Requires-Dist: fabric-orchestrator-client==1.7.0b2
 Requires-Dist: paramiko
 Requires-Dist: coverage>=4.0.3 ; extra == "test"
 Requires-Dist: nose>=1.3.7 ; extra == "test"
 Requires-Dist: pluggy>=0.3.1 ; extra == "test"
 Requires-Dist: py>=1.4.31 ; extra == "test"
 Requires-Dist: randomize>=0.13 ; extra == "test"
 Project-URL: Home, https://fabric-testbed.net/
```

