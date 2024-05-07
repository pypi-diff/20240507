# Comparing `tmp/dapla_toolbelt-2.0.8.tar.gz` & `tmp/dapla_toolbelt-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapla_toolbelt-2.0.8.tar", max compression
+gzip compressed data, was "dapla_toolbelt-2.0.9.tar", max compression
```

## Comparing `dapla_toolbelt-2.0.8.tar` & `dapla_toolbelt-2.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1073 2024-03-03 18:26:46.726100 dapla_toolbelt-2.0.8/LICENSE
--rw-r--r--   0        0        0     5656 2024-03-03 18:26:46.726100 dapla_toolbelt-2.0.8/README.md
--rw-r--r--   0        0        0     4528 2024-03-03 18:27:01.894015 dapla_toolbelt-2.0.8/pyproject.toml
--rw-r--r--   0        0        0     1948 2024-03-03 18:26:46.730100 dapla_toolbelt-2.0.8/src/dapla/__init__.py
--rw-r--r--   0        0        0     7266 2024-03-03 18:26:46.730100 dapla_toolbelt-2.0.8/src/dapla/auth.py
--rw-r--r--   0        0        0     1875 2024-03-03 18:26:46.730100 dapla_toolbelt-2.0.8/src/dapla/backports.py
--rw-r--r--   0        0        0     2380 2024-03-03 18:26:46.730100 dapla_toolbelt-2.0.8/src/dapla/collector.py
--rw-r--r--   0        0        0     4982 2024-03-03 18:26:46.730100 dapla_toolbelt-2.0.8/src/dapla/converter.py
--rw-r--r--   0        0        0     4339 2024-03-03 18:26:46.730100 dapla_toolbelt-2.0.8/src/dapla/doctor.py
--rw-r--r--   0        0        0     6706 2024-03-03 18:26:46.730100 dapla_toolbelt-2.0.8/src/dapla/files.py
--rw-r--r--   0        0        0     2562 2024-03-03 18:26:46.730100 dapla_toolbelt-2.0.8/src/dapla/gcs.py
--rw-r--r--   0        0        0     1143 2024-03-03 18:26:46.730100 dapla_toolbelt-2.0.8/src/dapla/git.py
--rw-r--r--   0        0        0     3042 2024-03-03 18:26:46.730100 dapla_toolbelt-2.0.8/src/dapla/guardian.py
--rw-r--r--   0        0        0     1194 2024-03-03 18:26:46.730100 dapla_toolbelt-2.0.8/src/dapla/jupyterhub.py
--rw-r--r--   0        0        0     8450 2024-03-03 18:26:46.730100 dapla_toolbelt-2.0.8/src/dapla/pandas.py
--rw-r--r--   0        0        0     6405 2024-03-03 18:26:46.730100 dapla_toolbelt-2.0.8/src/dapla/pubsub.py
--rw-r--r--   0        0        0        0 2024-03-03 18:26:46.730100 dapla_toolbelt-2.0.8/src/dapla/py.typed
--rw-r--r--   0        0        0       23 2024-03-03 18:26:46.730100 dapla_toolbelt-2.0.8/src/dapla/spark/__init__.py
--rw-r--r--   0        0        0      402 2024-03-03 18:26:46.730100 dapla_toolbelt-2.0.8/src/dapla/spark/sparkui.py
--rw-r--r--   0        0        0     6912 1970-01-01 00:00:00.000000 dapla_toolbelt-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-03-12 12:32:04.538453 dapla_toolbelt-2.0.9/LICENSE
+-rw-r--r--   0        0        0     5656 2024-03-12 12:32:04.538453 dapla_toolbelt-2.0.9/README.md
+-rw-r--r--   0        0        0     4528 2024-03-12 12:32:18.518437 dapla_toolbelt-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1948 2024-03-12 12:32:04.542453 dapla_toolbelt-2.0.9/src/dapla/__init__.py
+-rw-r--r--   0        0        0     7266 2024-03-12 12:32:04.542453 dapla_toolbelt-2.0.9/src/dapla/auth.py
+-rw-r--r--   0        0        0     1875 2024-03-12 12:32:04.542453 dapla_toolbelt-2.0.9/src/dapla/backports.py
+-rw-r--r--   0        0        0     2380 2024-03-12 12:32:04.542453 dapla_toolbelt-2.0.9/src/dapla/collector.py
+-rw-r--r--   0        0        0     4982 2024-03-12 12:32:04.542453 dapla_toolbelt-2.0.9/src/dapla/converter.py
+-rw-r--r--   0        0        0     4339 2024-03-12 12:32:04.542453 dapla_toolbelt-2.0.9/src/dapla/doctor.py
+-rw-r--r--   0        0        0     6706 2024-03-12 12:32:04.542453 dapla_toolbelt-2.0.9/src/dapla/files.py
+-rw-r--r--   0        0        0     2562 2024-03-12 12:32:04.542453 dapla_toolbelt-2.0.9/src/dapla/gcs.py
+-rw-r--r--   0        0        0     1143 2024-03-12 12:32:04.542453 dapla_toolbelt-2.0.9/src/dapla/git.py
+-rw-r--r--   0        0        0     3042 2024-03-12 12:32:04.542453 dapla_toolbelt-2.0.9/src/dapla/guardian.py
+-rw-r--r--   0        0        0     1194 2024-03-12 12:32:04.542453 dapla_toolbelt-2.0.9/src/dapla/jupyterhub.py
+-rw-r--r--   0        0        0     8450 2024-03-12 12:32:04.542453 dapla_toolbelt-2.0.9/src/dapla/pandas.py
+-rw-r--r--   0        0        0     6595 2024-03-12 12:32:18.518437 dapla_toolbelt-2.0.9/src/dapla/pubsub.py
+-rw-r--r--   0        0        0        0 2024-03-12 12:32:04.542453 dapla_toolbelt-2.0.9/src/dapla/py.typed
+-rw-r--r--   0        0        0       23 2024-03-12 12:32:04.542453 dapla_toolbelt-2.0.9/src/dapla/spark/__init__.py
+-rw-r--r--   0        0        0      402 2024-03-12 12:32:04.542453 dapla_toolbelt-2.0.9/src/dapla/spark/sparkui.py
+-rw-r--r--   0        0        0     6912 1970-01-01 00:00:00.000000 dapla_toolbelt-2.0.9/PKG-INFO
```

### Comparing `dapla_toolbelt-2.0.8/LICENSE` & `dapla_toolbelt-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-2.0.8/README.md` & `dapla_toolbelt-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-2.0.8/pyproject.toml` & `dapla_toolbelt-2.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapla-toolbelt"
-version = "2.0.8"
+version = "2.0.9"
 description = "Dapla Toolbelt"
 authors = ["Dapla Developers <dapla-platform-developers@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/dapla-toolbelt"
 repository = "https://github.com/statisticsnorway/dapla-toolbelt"
 documentation = "https://statisticsnorway.github.io/dapla-toolbelt"
```

### Comparing `dapla_toolbelt-2.0.8/src/dapla/__init__.py` & `dapla_toolbelt-2.0.9/src/dapla/__init__.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-2.0.8/src/dapla/auth.py` & `dapla_toolbelt-2.0.9/src/dapla/auth.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-2.0.8/src/dapla/backports.py` & `dapla_toolbelt-2.0.9/src/dapla/backports.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-2.0.8/src/dapla/collector.py` & `dapla_toolbelt-2.0.9/src/dapla/collector.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-2.0.8/src/dapla/converter.py` & `dapla_toolbelt-2.0.9/src/dapla/converter.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-2.0.8/src/dapla/doctor.py` & `dapla_toolbelt-2.0.9/src/dapla/doctor.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-2.0.8/src/dapla/files.py` & `dapla_toolbelt-2.0.9/src/dapla/files.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-2.0.8/src/dapla/gcs.py` & `dapla_toolbelt-2.0.9/src/dapla/gcs.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-2.0.8/src/dapla/git.py` & `dapla_toolbelt-2.0.9/src/dapla/git.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-2.0.8/src/dapla/guardian.py` & `dapla_toolbelt-2.0.9/src/dapla/guardian.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-2.0.8/src/dapla/jupyterhub.py` & `dapla_toolbelt-2.0.9/src/dapla/jupyterhub.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-2.0.8/src/dapla/pandas.py` & `dapla_toolbelt-2.0.9/src/dapla/pandas.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-2.0.8/src/dapla/pubsub.py` & `dapla_toolbelt-2.0.9/src/dapla/pubsub.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,28 +14,29 @@
 class EmptyListError(Exception):
     """Empty list error."""
 
     pass
 
 
 def _get_list_of_blobs_with_prefix(
-    bucket_name: str, folder_prefix: str
+    bucket_name: str, folder_prefix: str, project_id: str
 ) -> list[storage.Blob]:
     """Helper function that gets a list of Blob objects in a Google Cloud Storage bucket that has a certain prefix.
 
     Args:
         bucket_name (str): The name of the Google Cloud Storage bucket to get blobs from.
         folder_prefix (str): The prefix to filter blobs by.
+        project_id (str): The ID of the Google Cloud project that the Pub/Sub topic belongs to.
 
     Returns:
         An list over the `storage.Blob` objects representing the blobs in the specified bucket and with names starting
         with the given prefix.
     """
     google_credentials = AuthClient.fetch_google_credentials()
-    storage_client = storage.Client(credentials=google_credentials)
+    storage_client = storage.Client(project=project_id, credentials=google_credentials)
     return list(storage_client.list_blobs(bucket_name, prefix=folder_prefix))
 
 
 def _generate_pubsub_data(bucket_id: str, object_id: str) -> bytes:
     """Helper function that generates the message data to be published to a Google Cloud Pub/Sub topic.
 
     Args:
@@ -90,15 +91,15 @@
         folder_prefix (str): The prefix of the folder containing the objects to be published.
         topic_id (str): The ID of the Pub/Sub topic to publish to.
 
     Raises:
         EmptyListError: If there are no objects in the bucket with the given prefix.
 
     """
-    blob_list = _get_list_of_blobs_with_prefix(bucket_id, folder_prefix)
+    blob_list = _get_list_of_blobs_with_prefix(bucket_id, folder_prefix, project_id)
 
     if len(blob_list) == 0:
         raise EmptyListError(
             f"There are no files in {bucket_id:} with the given {folder_prefix:}."
         )
 
     publisher = PublisherClient(credentials=AuthClient.fetch_google_credentials())
@@ -159,15 +160,15 @@
 
 def trigger_source_data_processing(
     project_id: str, source_name: str, folder_prefix: str, kuben: bool = False
 ) -> None:
     """Triggers a source data processing service with every file that has a given prefix.
 
     Args:
-        project_id (str): The ID of Google Cloud project containing the source.
+        project_id (str): The ID of Google Cloud project containing the pubsub topic, this is normally the standard project.
         folder_prefix (str): The folder prefix of the files to be processed.
         source_name (str): The name of source that should process the files.
         kuben (bool): Whether the team is on kuben or legacy.
     """
     project_name = _extract_project_name(project_id)
 
     if kuben:
```

### Comparing `dapla_toolbelt-2.0.8/PKG-INFO` & `dapla_toolbelt-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapla-toolbelt
-Version: 2.0.8
+Version: 2.0.9
 Summary: Dapla Toolbelt
 Home-page: https://github.com/statisticsnorway/dapla-toolbelt
 License: MIT
 Author: Dapla Developers
 Author-email: dapla-platform-developers@ssb.no
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

