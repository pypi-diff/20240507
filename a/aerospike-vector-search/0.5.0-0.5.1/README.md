# Comparing `tmp/aerospike-vector-search-0.5.0.tar.gz` & `tmp/aerospike-vector-search-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aerospike-vector-search-0.5.0.tar", last modified: Tue Apr 30 17:03:43 2024, max compression
+gzip compressed data, was "aerospike-vector-search-0.5.1.tar", last modified: Mon May  6 23:33:23 2024, max compression
```

## Comparing `aerospike-vector-search-0.5.0.tar` & `aerospike-vector-search-0.5.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-04-30 17:03:43.644420 aerospike-vector-search-0.5.0/
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)    11357 2024-04-24 15:28:08.000000 aerospike-vector-search-0.5.0/LICENSE
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     2271 2024-04-30 17:03:43.644420 aerospike-vector-search-0.5.0/PKG-INFO
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     1431 2024-04-30 14:24:15.000000 aerospike-vector-search-0.5.0/README.md
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     1291 2024-04-30 16:58:37.000000 aerospike-vector-search-0.5.0/pyproject.toml
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)       38 2024-04-30 17:03:43.644420 aerospike-vector-search-0.5.0/setup.cfg
-drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-04-30 17:03:43.644420 aerospike-vector-search-0.5.0/src/
-drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-04-30 17:03:43.644420 aerospike-vector-search-0.5.0/src/aerospike_vector_search/
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)       29 2024-04-26 16:27:18.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search/__init__.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)    11008 2024-04-29 16:49:04.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search/admin.py
-drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-04-30 17:03:43.644420 aerospike-vector-search-0.5.0/src/aerospike_vector_search/aio/
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)       29 2024-04-26 16:27:18.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search/aio/__init__.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)    11179 2024-04-29 16:47:38.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search/aio/admin.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)    11639 2024-04-30 15:50:12.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search/aio/client.py
-drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-04-30 17:03:43.644420 aerospike-vector-search-0.5.0/src/aerospike_vector_search/aio/internal/
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     3555 2024-04-30 15:28:42.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search/aio/internal/channel_provider.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)    11496 2024-04-30 15:49:48.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search/client.py
-drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-04-30 17:03:43.644420 aerospike-vector-search-0.5.0/src/aerospike_vector_search/internal/
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)        0 2024-04-24 15:28:08.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search/internal/__init__.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     3442 2024-04-30 14:04:56.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search/internal/channel_provider.py
-drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-04-30 17:03:43.644420 aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)        0 2024-04-24 15:28:08.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/__init__.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     5097 2024-04-29 17:23:34.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/admin_helpers.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     4311 2024-04-30 13:59:41.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/base_channel_provider.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     6039 2024-04-29 17:38:21.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/client_helpers.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     3861 2024-04-26 22:58:39.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/conversions.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)      779 2024-04-30 16:04:08.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/helpers.py
-drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-04-30 17:03:43.644420 aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/proto_generated/
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     1735 2024-04-26 23:36:39.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/proto_generated/auth_pb2.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     2308 2024-04-26 23:36:39.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/proto_generated/auth_pb2_grpc.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     2063 2024-04-26 23:36:39.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/proto_generated/index_pb2.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     8361 2024-04-26 23:36:39.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/proto_generated/index_pb2_grpc.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     3588 2024-04-26 23:36:39.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/proto_generated/transact_pb2.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     8310 2024-04-26 23:36:39.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/proto_generated/transact_pb2_grpc.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     7941 2024-04-26 23:36:39.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/proto_generated/types_pb2.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)      159 2024-04-26 23:36:39.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/proto_generated/types_pb2_grpc.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     4790 2024-04-26 23:36:39.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/proto_generated/vector_db_pb2.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     9503 2024-04-26 23:36:39.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/proto_generated/vector_db_pb2_grpc.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     8730 2024-04-29 15:28:32.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search/types.py
-drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-04-30 17:03:43.644420 aerospike-vector-search-0.5.0/src/aerospike_vector_search.egg-info/
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     2271 2024-04-30 17:03:43.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search.egg-info/PKG-INFO
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     1767 2024-04-30 17:03:43.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search.egg-info/SOURCES.txt
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)        1 2024-04-30 17:03:43.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search.egg-info/dependency_links.txt
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)        1 2024-04-30 14:44:08.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search.egg-info/not-zip-safe
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)       16 2024-04-30 17:03:43.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search.egg-info/requires.txt
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)       24 2024-04-30 17:03:43.000000 aerospike-vector-search-0.5.0/src/aerospike_vector_search.egg-info/top_level.txt
+drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-05-06 23:33:23.267812 aerospike-vector-search-0.5.1/
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)    11357 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/LICENSE
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     2271 2024-05-06 23:33:23.267812 aerospike-vector-search-0.5.1/PKG-INFO
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     1431 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/README.md
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     1291 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/pyproject.toml
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)       38 2024-05-06 23:33:23.267812 aerospike-vector-search-0.5.1/setup.cfg
+drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-05-06 23:33:23.263811 aerospike-vector-search-0.5.1/src/
+drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-05-06 23:33:23.263811 aerospike-vector-search-0.5.1/src/aerospike_vector_search/
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)      197 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/__init__.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)    11145 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/admin.py
+drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-05-06 23:33:23.267812 aerospike-vector-search-0.5.1/src/aerospike_vector_search/aio/
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)      198 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/aio/__init__.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)    11671 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/aio/admin.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)    12289 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/aio/client.py
+drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-05-06 23:33:23.267812 aerospike-vector-search-0.5.1/src/aerospike_vector_search/aio/internal/
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     4463 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/aio/internal/channel_provider.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)    11830 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/client.py
+drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-05-06 23:33:23.267812 aerospike-vector-search-0.5.1/src/aerospike_vector_search/internal/
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)        0 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/internal/__init__.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     3757 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/internal/channel_provider.py
+drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-05-06 23:33:23.267812 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)        0 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/__init__.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     5147 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/admin_helpers.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     4337 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/base_channel_provider.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     6090 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/client_helpers.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     3861 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/conversions.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)      775 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/helpers.py
+drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-05-06 23:33:23.267812 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     1735 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/auth_pb2.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     2308 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/auth_pb2_grpc.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     2063 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/index_pb2.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     8361 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/index_pb2_grpc.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     3588 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/transact_pb2.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     8310 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/transact_pb2_grpc.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     7941 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/types_pb2.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)      159 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/types_pb2_grpc.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     4790 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/vector_db_pb2.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     9503 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/vector_db_pb2_grpc.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     8729 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/types.py
+drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-05-06 23:33:23.267812 aerospike-vector-search-0.5.1/src/aerospike_vector_search.egg-info/
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     2271 2024-05-06 23:33:23.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search.egg-info/PKG-INFO
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     1767 2024-05-06 23:33:23.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search.egg-info/SOURCES.txt
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)        1 2024-05-06 23:33:23.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search.egg-info/dependency_links.txt
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)        1 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search.egg-info/not-zip-safe
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)       16 2024-05-06 23:33:23.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search.egg-info/requires.txt
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)       24 2024-05-06 23:33:23.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search.egg-info/top_level.txt
```

### Comparing `aerospike-vector-search-0.5.0/LICENSE` & `aerospike-vector-search-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aerospike-vector-search-0.5.0/PKG-INFO` & `aerospike-vector-search-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aerospike-vector-search
-Version: 0.5.0
+Version: 0.5.1
 Summary: Aerospike Proximus Client Library for Python
 Author-email: "Aerospike, Inc." <info@aerospike.com>
 License: Apache Software License
 Project-URL: Homepage, https://aerospike.com
 Keywords: aerospike,vector,database,ANN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `aerospike-vector-search-0.5.0/README.md` & `aerospike-vector-search-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `aerospike-vector-search-0.5.0/pyproject.toml` & `aerospike-vector-search-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Database"
 ]
-version = "0.5.0"
+version = "0.5.1"
 requires-python = ">3.8"
 dependencies = [
     "grpcio",
     "protobuf"
 ]
 
 [project.urls]
```

### Comparing `aerospike-vector-search-0.5.0/src/aerospike_vector_search/admin.py` & `aerospike-vector-search-0.5.1/src/aerospike_vector_search/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,32 +20,32 @@
     def __init__(
         self,
         *,
         seeds: Union[types.HostPort, tuple[types.HostPort, ...]],
         listener_name: Optional[str] = None,
         is_loadbalancer: Optional[bool] = False,
     ) -> None:
-
-        seeds = self.prepare_seeds(seeds)
-
-        self._channelProvider = channel_provider.ChannelProvider(
-            seeds, listener_name, is_loadbalancer
-        )
         """
         Initialize the Aerospike Vector Search Admin Client.
 
         Args:
             seeds (Union[types.HostPort, tuple[types.HostPort, ...]]): Used to create appropriate gRPC channels for interacting with Aerospike Vector Search.
             listener_name (Optional[str], optional): Advertised listener for the client. Defaults to None.
             is_loadbalancer (bool, optional): If true, the first seed address will be treated as a load balancer node.
 
         Raises:
             Exception: Raised when no seed host is provided.
 
         """
+        seeds = self._prepare_seeds(seeds)
+
+        self._channel_provider = channel_provider.ChannelProvider(
+            seeds, listener_name, is_loadbalancer
+        )
+
 
     def index_create(
         self,
         *,
         namespace: str,
         name: str,
         vector_field: str,
@@ -78,15 +78,15 @@
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
 
         Note:
             This method creates an index with the specified parameters and waits for the index creation to complete.
             It waits for up to 100,000 seconds for the index creation to complete.
         """
-        (index_stub, index_create_request) = self.prepare_index_create(namespace, name, vector_field, dimensions, vector_distance_metric, sets, index_params, index_meta_data, logger)
+        (index_stub, index_create_request) = self._prepare_index_create(namespace, name, vector_field, dimensions, vector_distance_metric, sets, index_params, index_meta_data, logger)
         try:
             index_stub.Create(index_create_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
             raise e
         try:
             self._wait_for_index_creation(
@@ -108,15 +108,15 @@
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
 
         Note:
             This method drops an index with the specified parameters and waits for the index deletion to complete.
             It waits for up to 100,000 seconds for the index deletion to complete.
         """
-        (index_stub, index_drop_request) = self.prepare_index_drop(namespace, name, logger)
+        (index_stub, index_drop_request) = self._prepare_index_drop(namespace, name, logger)
         try:
             index_stub.Drop(index_drop_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
             raise e
         try:
             self._wait_for_index_deletion(
@@ -133,21 +133,21 @@
         Returns:
             list[dict]: A list of indices.
 
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
         """
-        (index_stub, index_list_request) = self.prepare_index_list(logger)
+        (index_stub, index_list_request) = self._prepare_index_list(logger)
         try:
             response = index_stub.List(index_list_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
             raise e
-        return self.respond_index_list(response)
+        return self._respond_index_list(response)
 
     def index_get(
         self, *, namespace: str, name: str
     ) -> dict[str, Union[int, str]]:
         """
         Retrieve the information related with an index.
 
@@ -159,21 +159,21 @@
             dict[str, Union[int, str]: Information about an index.
 
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
 
         """
-        (index_stub, index_get_request) = self.prepare_index_get(namespace, name, logger)
+        (index_stub, index_get_request) = self._prepare_index_get(namespace, name, logger)
         try:
             response = index_stub.Get(index_get_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
             raise e
-        return self.respond_index_get(response)
+        return self._respond_index_get(response)
 
 
     def index_get_status(self, *, namespace: str, name: str) -> int:
         """
         Retrieve the number of records queued to be merged into an index.
 
         Args:
@@ -189,32 +189,32 @@
 
         Note:
             This method retrieves the status of the specified index. If index_get_status is called the vector client puts some records into Aerospike Vector Search,
             the records may not immediately begin to merge into the index. To wait for all records to be merged into an index, use vector_client.wait_for_index_completion.
 
             Warning: This API is subject to change.
         """
-        (index_stub, index_get_status_request) = self.prepare_index_get_status(namespace, name, logger)
+        (index_stub, index_get_status_request) = self._prepare_index_get_status(namespace, name, logger)
         try:
             response = index_stub.GetStatus(index_get_status_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
             raise e
 
-        return self.respond_index_get_status(response)
+        return self._respond_index_get_status(response)
 
     def _wait_for_index_creation(
-        self, *, namespace: str, name: str, timeout: int = sys.maxsize
+        self, *, namespace: str, name: str, timeout: Optional[int] = sys.maxsize, wait_interval: Optional[int] = 0.1
     ) -> None:
         """
         Wait for the index to be created.
         """
-        (index_stub, wait_interval, start_time, _, _, index_creation_request) = self.prepare_wait_for_index_waiting(namespace, name)
+        (index_stub, wait_interval, start_time, _, _, index_creation_request) = self._prepare_wait_for_index_waiting(namespace, name, wait_interval)
         while True:
-            self.check_timeout(start_time, timeout)
+            self._check_timeout(start_time, timeout)
             try:
                 index_stub.GetStatus(index_creation_request)
                 logger.debug("Index created succesfully")
                 # Index has been created
                 return
             except grpc.RpcError as e:
                 if e.code() in (grpc.StatusCode.UNAVAILABLE, grpc.StatusCode.NOT_FOUND):
@@ -222,25 +222,25 @@
                     # Wait for some more time.
                     time.sleep(wait_interval)
                 else:
                     logger.error("Failed with error: %s", e)
                     raise e
 
     def _wait_for_index_deletion(
-        self, *, namespace: str, name: str, timeout: int = sys.maxsize
+        self, *, namespace: str, name: str, timeout: Optional[int] = sys.maxsize, wait_interval: Optional[int] = 0.1
     ) -> None:
         """
         Wait for the index to be deleted.
         """
 
         # Wait interval between polling
-        (index_stub, wait_interval, start_time, _, _, index_deletion_request) = self.prepare_wait_for_index_waiting(namespace, name)
+        (index_stub, wait_interval, start_time, _, _, index_deletion_request) = self._prepare_wait_for_index_waiting(namespace, name, wait_interval)
 
         while True:
-            self.check_timeout(start_time, timeout)
+            self._check_timeout(start_time, timeout)
 
             try:
                 index_stub.GetStatus(index_deletion_request)
                 # Wait for some more time.
                 time.sleep(wait_interval)
             except grpc.RpcError as e:
                 if e.code() in (grpc.StatusCode.UNAVAILABLE, grpc.StatusCode.NOT_FOUND):
@@ -255,15 +255,15 @@
         Close the Aerospike Vector Search Admin Client.
 
         This method closes gRPC channels connected to Aerospike Vector Search.
 
         Note:
             This method should be called when the VectorDbAdminClient is no longer needed to release resources.
         """
-        self._channelProvider.close()
+        self._channel_provider.close()
 
     def __enter__(self):
         """
         Enter an asynchronous context manager for the admin client.
 
         Returns:
             VectorDbAdminlient: Aerospike Vector Search Admin Client instance.
```

### Comparing `aerospike-vector-search-0.5.0/src/aerospike_vector_search/aio/admin.py` & `aerospike-vector-search-0.5.1/src/aerospike_vector_search/aio/admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import asyncio
 import logging
 import sys
-import time
 from typing import Any, Optional, Union
 import grpc
 
 from .. import types
 from .internal import channel_provider
 from ..shared.admin_helpers import BaseClient
 
@@ -21,32 +20,32 @@
     def __init__(
         self,
         *,
         seeds: Union[types.HostPort, tuple[types.HostPort, ...]],
         listener_name: Optional[str] = None,
         is_loadbalancer: Optional[bool] = False,
     ) -> None:
-
-        seeds = self.prepare_seeds(seeds)
-
-        self._channelProvider = channel_provider.ChannelProvider(
-            seeds, listener_name, is_loadbalancer
-        )
         """
         Initialize the Aerospike Vector Search Admin Client.
 
         Args:
             seeds (Union[types.HostPort, tuple[types.HostPort, ...]]): Used to create appropriate gRPC channels for interacting with Aerospike Vector Search.
             listener_name (Optional[str], optional): Advertised listener for the client. Defaults to None.
             is_loadbalancer (bool, optional): If true, the first seed address will be treated as a load balancer node.
 
         Raises:
             Exception: Raised when no seed host is provided.
 
         """
+        seeds = self._prepare_seeds(seeds)
+
+        self._channel_provider = channel_provider.ChannelProvider(
+            seeds, listener_name, is_loadbalancer
+        )
+
 
     async def index_create(
         self,
         *,
         namespace: str,
         name: str,
         vector_field: str,
@@ -79,15 +78,19 @@
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
 
         Note:
             This method creates an index with the specified parameters and waits for the index creation to complete.
             It waits for up to 100,000 seconds for the index creation to complete.
         """
-        (index_stub, index_create_request) = self.prepare_index_create(namespace, name, vector_field, dimensions, vector_distance_metric, sets, index_params, index_meta_data, logger)
+
+        await self._channel_provider._is_ready()
+
+        (index_stub, index_create_request) = self._prepare_index_create(namespace, name, vector_field, dimensions, vector_distance_metric, sets, index_params, index_meta_data, logger)
+        
         try:
             await index_stub.Create(index_create_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
             raise e
         try:
             await self._wait_for_index_creation(
@@ -109,15 +112,17 @@
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
 
         Note:
             This method drops an index with the specified parameters and waits for the index deletion to complete.
             It waits for up to 100,000 seconds for the index deletion to complete.
         """
-        (index_stub, index_drop_request) = self.prepare_index_drop(namespace, name, logger)
+        await self._channel_provider._is_ready()
+
+        (index_stub, index_drop_request) = self._prepare_index_drop(namespace, name, logger)
         try:
             await index_stub.Drop(index_drop_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
             raise e
         try:
             await self._wait_for_index_deletion(
@@ -134,21 +139,23 @@
         Returns:
             list[dict]: A list of indices.
 
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
         """
-        (index_stub, index_list_request) = self.prepare_index_list(logger)
+        await self._channel_provider._is_ready()
+        
+        (index_stub, index_list_request) = self._prepare_index_list(logger)
         try:
             response = await index_stub.List(index_list_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
             raise e
-        return self.respond_index_list(response)
+        return self._respond_index_list(response)
 
     async def index_get(
         self, *, namespace: str, name: str
     ) -> dict[str, Union[int, str]]:
         """
         Retrieve the information related with an index.
 
@@ -160,21 +167,23 @@
             dict[str, Union[int, str]: Information about an index.
 
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
 
         """
-        (index_stub, index_get_request) = self.prepare_index_get(namespace, name, logger)
+        await self._channel_provider._is_ready()
+
+        (index_stub, index_get_request) = self._prepare_index_get(namespace, name, logger)
         try:
             response = await index_stub.Get(index_get_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
             raise e
-        return self.respond_index_get(response)
+        return self._respond_index_get(response)
 
 
     async def index_get_status(self, *, namespace: str, name: str) -> int:
         """
         Retrieve the number of records queued to be merged into an index.
 
         Args:
@@ -190,32 +199,36 @@
 
         Note:
             This method retrieves the status of the specified index. If index_get_status is called the vector client puts some records into Aerospike Vector Search,
             the records may not immediately begin to merge into the index. To wait for all records to be merged into an index, use vector_client.wait_for_index_completion.
 
             Warning: This API is subject to change.
         """
-        (index_stub, index_get_status_request) = self.prepare_index_get_status(namespace, name, logger)
+        await self._channel_provider._is_ready()
+
+        (index_stub, index_get_status_request) = self._prepare_index_get_status(namespace, name, logger)
         try:
             response = await index_stub.GetStatus(index_get_status_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
             raise e
 
-        return self.respond_index_get_status(response)
+        return self._respond_index_get_status(response)
 
     async def _wait_for_index_creation(
-        self, *, namespace: str, name: str, timeout: int = sys.maxsize
+        self, *, namespace: str, name: str, timeout: Optional[int] = sys.maxsize, wait_interval: Optional[int] = 0.1
     ) -> None:
         """
         Wait for the index to be created.
         """
-        (index_stub, wait_interval, start_time, _, _, index_creation_request) = self.prepare_wait_for_index_waiting(namespace, name)
+        await self._channel_provider._is_ready()
+
+        (index_stub, wait_interval, start_time, _, _, index_creation_request) = self._prepare_wait_for_index_waiting(namespace, name, wait_interval)
         while True:
-            self.check_timeout(start_time, timeout)
+            self._check_timeout(start_time, timeout)
             try:
                 await index_stub.GetStatus(index_creation_request)
                 logger.debug("Index created succesfully")
                 # Index has been created
                 return
             except grpc.RpcError as e:
                 if e.code() in (grpc.StatusCode.UNAVAILABLE, grpc.StatusCode.NOT_FOUND):
@@ -223,25 +236,26 @@
                     # Wait for some more time.
                     await asyncio.sleep(wait_interval)
                 else:
                     logger.error("Failed with error: %s", e)
                     raise e
 
     async def _wait_for_index_deletion(
-        self, *, namespace: str, name: str, timeout: int = sys.maxsize
+        self, *, namespace: str, name: str, timeout: Optional[int] = sys.maxsize, wait_interval: Optional[int] = 0.1
     ) -> None:
         """
         Wait for the index to be deleted.
         """
+        await self._channel_provider._is_ready()
 
         # Wait interval between polling
-        (index_stub, wait_interval, start_time, _, _, index_deletion_request) = self.prepare_wait_for_index_waiting(namespace, name)
+        (index_stub, wait_interval, start_time, _, _, index_deletion_request) = self._prepare_wait_for_index_waiting(namespace, name, wait_interval)
 
         while True:
-            self.check_timeout(start_time, timeout)
+            self._check_timeout(start_time, timeout)
 
             try:
                 await index_stub.GetStatus(index_deletion_request)
                 # Wait for some more time.
                 await asyncio.sleep(wait_interval)
             except grpc.RpcError as e:
                 if e.code() in (grpc.StatusCode.UNAVAILABLE, grpc.StatusCode.NOT_FOUND):
@@ -256,15 +270,15 @@
         Close the Aerospike Vector Search Admin Client.
 
         This method closes gRPC channels connected to Aerospike Vector Search.
 
         Note:
             This method should be called when the VectorDbAdminClient is no longer needed to release resources.
         """
-        await self._channelProvider.close()
+        await self._channel_provider.close()
 
     async def __aenter__(self):
         """
         Enter an asynchronous context manager for the admin client.
 
         Returns:
             VectorDbAdminlient: Aerospike Vector Search Admin Client instance.
```

### Comparing `aerospike-vector-search-0.5.0/src/aerospike_vector_search/aio/client.py` & `aerospike-vector-search-0.5.1/src/aerospike_vector_search/aio/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,16 +37,16 @@
                 Advertised listener for the client. Defaults to None.
             is_loadbalancer (bool, optional):
                 If true, the first seed address will be treated as a load balancer node.
 
         Raises:
             Exception: Raised when no seed host is provided.
         """
-        seeds = self.prepare_seeds(seeds)
-        self._channelProvider = channel_provider.ChannelProvider(
+        seeds = self._prepare_seeds(seeds)
+        self._channel_provider = channel_provider.ChannelProvider(
             seeds, listener_name, is_loadbalancer
         )
 
     async def put(
         self,
         *,
         namespace: str,
@@ -64,15 +64,18 @@
             set_name (Optional[str], optional): The name of the set to which the record belongs. Defaults to None.
 
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
 
         """
-        (transact_stub, put_request) = self.prepare_put(namespace, key, record_data, set_name, logger)
+
+        await self._channel_provider._is_ready()
+
+        (transact_stub, put_request) = self._prepare_put(namespace, key, record_data, set_name, logger)
 
         try:
             await transact_stub.Put(put_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
             raise e
 
@@ -97,22 +100,25 @@
         Returns:
             types.RecordWithKey: A record with its associated key.
 
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
         """
-        (transact_stub, key, get_request) = self.prepare_get(namespace, key, bin_names, set_name, logger)
+
+        await self._channel_provider._is_ready()
+
+        (transact_stub, key, get_request) = self._prepare_get(namespace, key, bin_names, set_name, logger)
         try:
             response = await transact_stub.Get(get_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
             raise e
 
-        return self.respond_get(response, key)
+        return self._respond_get(response, key)
 
     async def exists(
         self, *, namespace: str, key: Any, set_name: Optional[str] = None
     ) -> bool:
         """
         Check if a record exists in Aerospike Vector Search.
 
@@ -124,22 +130,25 @@
         Returns:
             bool: True if the record exists, False otherwise.
 
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
         """
-        (transact_stub, key) = self.prepare_exists(namespace, key, set_name, logger)
+
+        await self._channel_provider._is_ready()
+
+        (transact_stub, key) = self._prepare_exists(namespace, key, set_name, logger)
         try:
             response = await transact_stub.Exists(key)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
             raise e
 
-        return self.respond_exists(response)
+        return self._respond_exists(response)
 
     async def is_indexed(
         self,
         *,
         namespace: str,
         key: Union[int, str, bytes, bytearray],
         index_name: str,
@@ -160,21 +169,24 @@
         Returns:
             bool: True if the record is indexed, False otherwise.
 
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
         """
-        (transact_stub, is_indexed_request) = self.prepare_is_indexed(namespace, key, index_name, index_namespace, set_name, logger)
+
+        await self._channel_provider._is_ready()
+
+        (transact_stub, is_indexed_request) = self._prepare_is_indexed(namespace, key, index_name, index_namespace, set_name, logger)
         try:
             response = await transact_stub.IsIndexed(is_indexed_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
             raise e
-        return self.respond_is_indexed(response)
+        return self._respond_is_indexed(response)
 
     async def vector_search(
         self,
         *,
         namespace: str,
         index_name: str,
         query: list[Union[bool, float]],
@@ -198,61 +210,67 @@
         Returns:
             list[types.Neighbor]: A list of neighbors records found by the search.
 
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
         """
-        (transact_stub, vector_search_request) = self.prepare_vector_search(namespace, index_name, query, limit, search_params, bin_names, logger)
+        await self._channel_provider._is_ready()
+
+        (transact_stub, vector_search_request) = self._prepare_vector_search(namespace, index_name, query, limit, search_params, bin_names, logger)
 
         try:
             results_stream = transact_stub.VectorSearch(vector_search_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
             raise e
         async_results = []
         async for result in results_stream:
-            async_results.append(self.respond_neighbor(result))
+            async_results.append(self._respond_neighbor(result))
 
         return async_results
 
     async def wait_for_index_completion(
-        self, *, namespace: str, name: str, timeout: Optional[int] = sys.maxsize
+        self, *, namespace: str, name: str, timeout: Optional[int] = sys.maxsize, wait_interval: Optional[int] = 12
     ) -> None:
         """
         Wait for the index to have no pending index update operations.
 
         Args:
             namespace (str): The namespace of the index.
             name (str): The name of the index.
             timeout (int, optional): The maximum time (in seconds) to wait for the index to complete.
             Defaults to sys.maxsize.
-
+            wait_interval (int, optional): The time (in seconds) to wait between index completion status request to the server.
+            Lowering this value increases the chance that the index completion status is incorrect, which can result in poor search accuracy.
+            
         Raises:
             Exception: Raised when the timeout occurs while waiting for index completion.
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
 
         Note:
             The function polls the index status with a wait interval of 10 seconds until either
             the timeout is reached or the index has no pending index update operations.
         """
+        await self._channel_provider._is_ready()
+
         # Wait interval between polling
-        (index_stub, wait_interval, start_time, unmerged_record_initialized, double_check, index_completion_request) = self.prepare_wait_for_index_waiting(namespace, name)
+        (index_stub, wait_interval, start_time, unmerged_record_initialized, double_check, index_completion_request) = self._prepare_wait_for_index_waiting(namespace, name, wait_interval)
         while True:
             try:
                 index_status = await index_stub.GetStatus(index_completion_request)
 
             except grpc.RpcError as e:
                 if e.code() == grpc.StatusCode.UNAVAILABLE:
                     continue
                 else:
                     logger.error("Failed with error: %s", e)
                     raise e
-            if self.check_completion_condition(start_time, timeout, index_status, unmerged_record_initialized):
+            if self._check_completion_condition(start_time, timeout, index_status, unmerged_record_initialized):
                 if double_check:
                     return
                 else:
                     double_check = True
             else:
                 double_check = False
             await asyncio.sleep(wait_interval)
@@ -262,15 +280,15 @@
         Close the Aerospike Vector Search Vector Client.
 
         This method closes gRPC channels connected to Aerospike Vector Search.
 
         Note:
             This method should be called when the VectorDbAdminClient is no longer needed to release resources.
         """
-        await self._channelProvider.close()
+        await self._channel_provider.close()
 
     async def __aenter__(self):
         """
         Enter an asynchronous context manager for the vector client.
 
         Returns:
             VectorDbClient: Aerospike Vector Search Vector Client instance.
```

### Comparing `aerospike-vector-search-0.5.0/src/aerospike_vector_search/aio/internal/channel_provider.py` & `aerospike-vector-search-0.5.1/src/aerospike_vector_search/internal/channel_provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,97 +1,106 @@
 import re
-import asyncio
+import time
 import logging
+import threading
 from typing import Optional, Union
 
 import google.protobuf.empty_pb2
 import grpc
-import random
 
-from ... import types
-from ...shared.proto_generated import vector_db_pb2
-from ...shared.proto_generated import vector_db_pb2_grpc
-from ...shared import base_channel_provider
+from .. import types
+from ..shared.proto_generated import vector_db_pb2
+from ..shared.proto_generated import vector_db_pb2_grpc
+from ..shared import base_channel_provider
 
 empty = google.protobuf.empty_pb2.Empty()
 
 logger = logging.getLogger(__name__)
 
 
 class ChannelProvider(base_channel_provider.BaseChannelProvider):
     """Proximus Channel Provider"""
     def __init__(
         self, seeds: tuple[types.HostPort, ...], listener_name: Optional[str] = None, is_loadbalancer: Optional[bool] = False
     ) -> None:
         super().__init__(seeds, listener_name, is_loadbalancer)
-        asyncio.create_task(self._tend())
+        self._tend_ended = threading.Event()
+        self._timer = None
+        self._tend()
 
-    async def close(self):
+    def close(self):
         self._closed = True
+        self._tend_ended.wait()
+
         for channel in self._seedChannels:
-            await channel.close()
+            channel.close()
 
         for k, channelEndpoints in self._node_channels.items():
             if channelEndpoints.channel:
-                await channelEndpoints.channel.close()
+                channelEndpoints.channel.close()
+
+        if self._timer != None:
+            self._timer.join()
+ 
+    def _tend(self):
+        (temp_endpoints, update_endpoints_stub, channels, end_tend) = self.init_tend()
 
-    async def _tend(self):
-        (temp_endpoints, update_endpoints, channels, end_tend) = self.init_tend()
         if end_tend:
-            return
+            self._tend_ended.set()
 
-        for seedChannel in channels:
+            return
+        for channel in channels:
 
-            stub = vector_db_pb2_grpc.ClusterInfoStub(seedChannel)
+            stub = vector_db_pb2_grpc.ClusterInfoStub(channel)
             
             try:
-                new_cluster_id = await stub.GetClusterId(empty).id
+                new_cluster_id = stub.GetClusterId(empty).id
                 if self.check_cluster_id(new_cluster_id):
-                    update_endpoints = True
+                    update_endpoints_stub = stub
+                    break
                 else:
                     continue
 
             except Exception as e:
                 logger.debug("While tending, failed to get cluster id with error:" + str(e))
 
 
+        if update_endpoints_stub:
             try:
-                response = await stub.GetClusterEndpoints(
+                response = stub.GetClusterEndpoints(
                     vector_db_pb2.ClusterNodeEndpointsRequest(
                         listenerName=self.listener_name
                     )
                 )
+                temp_endpoints = self.update_temp_endpoints(response, temp_endpoints)
             except Exception as e:
                 logger.debug("While tending, failed to get cluster endpoints with error:" + str(e))
 
-            temp_endpoints = self.update_temp_endpoints(response, temp_endpoints)
-
-        if update_endpoints:
             for node, newEndpoints in temp_endpoints.items():
                 (channel_endpoints, add_new_channel) = self.check_for_new_endpoints(node, newEndpoints)
+
                 if add_new_channel:
                     try:
                         # TODO: Wait for all calls to drain
-                        await channel_endpoints.channel.close()
+                        channel_endpoints.channel.close()
                     except Exception as e:
                         logger.debug("While tending, failed to close GRPC channel:" + str(e))
 
                     self.add_new_channel_to_node_channels(node, newEndpoints)
 
-            for node, channel_endpoints in self._node_channels.items():
+            temp_node_channels = self._node_channels.items()
+            for node, channel_endpoints in temp_node_channels:
                 if not temp_endpoints.get(node):
                     # TODO: Wait for all calls to drain
                     try:
-                        await channel_endpoints.channel.close()
+                        channel_endpoints.channel.close()
                         del self._node_channels[node]
                         
                     except Exception as e:
                         logger.debug("While tending, failed to close GRPC channel:" + str(e))
-
         # TODO: check tend interval.
-        await asyncio.sleep(1)
-        asyncio.create_task(self._tend())
+        self._timer = threading.Timer(1, self._tend).start()
 
-    def _create_channel(self, host: str, port: int, is_tls: bool) -> grpc.aio.Channel:
+    def _create_channel(self, host: str, port: int, is_tls: bool) -> grpc.Channel:
         # TODO: Take care of TLS
         host = re.sub(r"%.*", "", host)
-        return grpc.aio.insecure_channel(f"{host}:{port}")
+        return grpc.insecure_channel(f"{host}:{port}")
```

### Comparing `aerospike-vector-search-0.5.0/src/aerospike_vector_search/client.py` & `aerospike-vector-search-0.5.1/src/aerospike_vector_search/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,16 @@
                 Advertised listener for the client. Defaults to None.
             is_loadbalancer (bool, optional):
                 If true, the first seed address will be treated as a load balancer node.
 
         Raises:
             Exception: Raised when no seed host is provided.
         """
-        seeds = self.prepare_seeds(seeds)
-        self._channelProvider = channel_provider.ChannelProvider(
+        seeds = self._prepare_seeds(seeds)
+        self._channel_provider = channel_provider.ChannelProvider(
             seeds, listener_name, is_loadbalancer
         )
 
     def put(
         self,
         *,
         namespace: str,
@@ -64,15 +64,15 @@
             set_name (Optional[str], optional): The name of the set to which the record belongs. Defaults to None.
 
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
 
         """
-        (transact_stub, put_request) = self.prepare_put(namespace, key, record_data, set_name, logger)
+        (transact_stub, put_request) = self._prepare_put(namespace, key, record_data, set_name, logger)
 
         try:
             transact_stub.Put(put_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
             raise e
 
@@ -97,22 +97,22 @@
         Returns:
             types.RecordWithKey: A record with its associated key.
 
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
         """
-        (transact_stub, key, get_request) = self.prepare_get(namespace, key, bin_names, set_name, logger)
+        (transact_stub, key, get_request) = self._prepare_get(namespace, key, bin_names, set_name, logger)
         try:
             response = transact_stub.Get(get_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
             raise e
 
-        return self.respond_get(response, key)
+        return self._respond_get(response, key)
 
     def exists(
         self, *, namespace: str, key: Any, set_name: Optional[str] = None
     ) -> bool:
         """
         Check if a record exists in Aerospike Vector Search.
 
@@ -124,22 +124,22 @@
         Returns:
             bool: True if the record exists, False otherwise.
 
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
         """
-        (transact_stub, key) = self.prepare_exists(namespace, key, set_name, logger)
+        (transact_stub, key) = self._prepare_exists(namespace, key, set_name, logger)
         try:
             response = transact_stub.Exists(key)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
             raise e
 
-        return self.respond_exists(response)
+        return self._respond_exists(response)
 
     def is_indexed(
         self,
         *,
         namespace: str,
         key: Union[int, str, bytes, bytearray],
         index_name: str,
@@ -160,21 +160,21 @@
         Returns:
             bool: True if the record is indexed, False otherwise.
 
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
         """
-        (transact_stub, is_indexed_request) = self.prepare_is_indexed(namespace, key, index_name, index_namespace, set_name, logger)
+        (transact_stub, is_indexed_request) = self._prepare_is_indexed(namespace, key, index_name, index_namespace, set_name, logger)
         try:
             response = transact_stub.IsIndexed(is_indexed_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
             raise e
-        return self.respond_is_indexed(response)
+        return self._respond_is_indexed(response)
 
     def vector_search(
         self,
         *,
         namespace: str,
         index_name: str,
         query: list[Union[bool, float]],
@@ -198,61 +198,63 @@
         Returns:
             list[types.Neighbor]: A list of neighbors records found by the search.
 
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
         """
-        (transact_stub, vector_search_request) = self.prepare_vector_search(namespace, index_name, query, limit, search_params, bin_names, logger)
+        (transact_stub, vector_search_request) = self._prepare_vector_search(namespace, index_name, query, limit, search_params, bin_names, logger)
 
         try:
             results_stream = transact_stub.VectorSearch(vector_search_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
             raise e
         results = []
         for result in results_stream:
-            results.append(self.respond_neighbor(result))
+            results.append(self._respond_neighbor(result))
 
         return results
 
     def wait_for_index_completion(
-        self, *, namespace: str, name: str, timeout: Optional[int] = sys.maxsize
+        self, *, namespace: str, name: str, timeout: Optional[int] = sys.maxsize, wait_interval: Optional[int] = 12
     ) -> None:
         """
         Wait for the index to have no pending index update operations.
 
         Args:
             namespace (str): The namespace of the index.
             name (str): The name of the index.
             timeout (int, optional): The maximum time (in seconds) to wait for the index to complete.
             Defaults to sys.maxsize.
+            wait_interval (int, optional): The time (in seconds) to wait between index completion status request to the server.
+            Lowering this value increases the chance that the index completion status is incorrect, which can result in poor search accuracy.
 
         Raises:
             Exception: Raised when the timeout occurs while waiting for index completion.
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
 
         Note:
             The function polls the index status with a wait interval of 10 seconds until either
             the timeout is reached or the index has no pending index update operations.
         """
         # Wait interval between polling
-        (index_stub, wait_interval, start_time, unmerged_record_initialized, double_check, index_completion_request) = self.prepare_wait_for_index_waiting(namespace, name)
+        (index_stub, wait_interval, start_time, unmerged_record_initialized, double_check, index_completion_request) = self._prepare_wait_for_index_waiting(namespace, name, wait_interval)
         while True:
             try:
                 index_status = index_stub.GetStatus(index_completion_request)
 
             except grpc.RpcError as e:
                 if e.code() == grpc.StatusCode.UNAVAILABLE:
                     continue
                 else:
                     logger.error("Failed with error: %s", e)
                     raise e
-            if self.check_completion_condition(start_time, timeout, index_status, unmerged_record_initialized):
+            if self._check_completion_condition(start_time, timeout, index_status, unmerged_record_initialized):
                 if double_check:
                     return
                 else:
                     double_check = True
             else:
                 double_check = False
             time.sleep(wait_interval)
@@ -262,15 +264,15 @@
         Close the Aerospike Vector Search Vector Client.
 
         This method closes gRPC channels connected to Aerospike Vector Search.
 
         Note:
             This method should be called when the VectorDbAdminClient is no longer needed to release resources.
         """
-        self._channelProvider.close()
+        self._channel_provider.close()
 
     def __enter__(self):
         """
         Enter an asynchronous context manager for the vector client.
 
         Returns:
             VectorDbClient: Aerospike Vector Search Vector Client instance.
```

### Comparing `aerospike-vector-search-0.5.0/src/aerospike_vector_search/internal/channel_provider.py` & `aerospike-vector-search-0.5.1/src/aerospike_vector_search/aio/internal/channel_provider.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,97 +1,131 @@
 import re
+import asyncio
 import logging
-import threading
 from typing import Optional, Union
 
 import google.protobuf.empty_pb2
 import grpc
+import random
 
-from .. import types
-from ..shared.proto_generated import vector_db_pb2
-from ..shared.proto_generated import vector_db_pb2_grpc
-from ..shared import base_channel_provider
+from ... import types
+from ...shared.proto_generated import vector_db_pb2
+from ...shared.proto_generated import vector_db_pb2_grpc
+from ...shared import base_channel_provider
 
 empty = google.protobuf.empty_pb2.Empty()
 
 logger = logging.getLogger(__name__)
 
 
+
 class ChannelProvider(base_channel_provider.BaseChannelProvider):
     """Proximus Channel Provider"""
     def __init__(
         self, seeds: tuple[types.HostPort, ...], listener_name: Optional[str] = None, is_loadbalancer: Optional[bool] = False
     ) -> None:
         super().__init__(seeds, listener_name, is_loadbalancer)
-        self._tend()
+        asyncio.create_task(self._tend())
+        self._tend_initalized: asyncio.Event =  asyncio.Event()
+
+        self._tend_ended: asyncio.Event =  asyncio.Event()
+        self._task: Optional[asyncio.Task] = None
+
+
 
-    def close(self):
+    async def close(self):
         self._closed = True
+        await self._tend_ended.wait()
+
         for channel in self._seedChannels:
-            channel.close()
+            await channel.close()
 
         for k, channelEndpoints in self._node_channels.items():
             if channelEndpoints.channel:
-                channelEndpoints.channel.close()
+                await channelEndpoints.channel.close()
+
+        if self._task != None:
+            await self._task
 
-    def _tend(self):
-        (temp_endpoints, update_endpoints, channels, end_tend) = self.init_tend()
+    async def _is_ready(self):
+        await self._tend_initalized.wait()
+
+    async def _tend(self):
+        (temp_endpoints, update_endpoints_stub, channels, end_tend) = self.init_tend()
 
         if end_tend:
+            self._tend_ended.set()
             return
 
-        for seedChannel in channels:
+        stubs = []
+        tasks = []
+
+        for channel in channels:
 
-            stub = vector_db_pb2_grpc.ClusterInfoStub(seedChannel)
-            
+            stub = vector_db_pb2_grpc.ClusterInfoStub(channel)
+            stubs.append(stub)
             try:
-                new_cluster_id = stub.GetClusterId(empty).id
-                if self.check_cluster_id(new_cluster_id):
-                    update_endpoints = True
-                else:
-                    continue
+                tasks.append(stub.GetClusterId(empty))
 
             except Exception as e:
                 logger.debug("While tending, failed to get cluster id with error:" + str(e))
 
+        new_cluster_ids = await asyncio.gather(*tasks)
 
+        for index, value in enumerate(new_cluster_ids):
+            if self.check_cluster_id(value.id):
+                update_endpoints_stub = stubs[index]
+                break
+
+        if update_endpoints_stub:
             try:
-                response = stub.GetClusterEndpoints(
+                response = await update_endpoints_stub.GetClusterEndpoints(
                     vector_db_pb2.ClusterNodeEndpointsRequest(
                         listenerName=self.listener_name
                     )
                 )
                 temp_endpoints = self.update_temp_endpoints(response, temp_endpoints)
             except Exception as e:
                 logger.debug("While tending, failed to get cluster endpoints with error:" + str(e))
 
+            tasks = []
+            add_new_channel_info = []
 
-        if update_endpoints:
             for node, newEndpoints in temp_endpoints.items():
                 (channel_endpoints, add_new_channel) = self.check_for_new_endpoints(node, newEndpoints)
-
+                
                 if add_new_channel:
                     try:
                         # TODO: Wait for all calls to drain
-                        channel_endpoints.channel.close()
+                        tasks.append(channel_endpoints.channel.close())
                     except Exception as e:
                         logger.debug("While tending, failed to close GRPC channel:" + str(e))
+                    add_new_channel_info.append((node, newEndpoints))
+
+
+            for node, newEndpoints in add_new_channel_info:
+                self.add_new_channel_to_node_channels(node, newEndpoints)
 
-                    self.add_new_channel_to_node_channels(node, newEndpoints)
 
-            for node, channel_endpoints in self._node_channels.items():
+            temp_node_channels = self._node_channels.items()
+            for node, channel_endpoints in temp_node_channels:
                 if not temp_endpoints.get(node):
-                    # TODO: Wait for all calls to drain
                     try:
-                        channel_endpoints.channel.close()
+                        # TODO: Wait for all calls to drain
+                        tasks.append(channel_endpoints.channel.close())
                         del self._node_channels[node]
                         
                     except Exception as e:
                         logger.debug("While tending, failed to close GRPC channel:" + str(e))
 
+            await asyncio.gather(*tasks)
+
+        self._tend_initalized.set()
+
         # TODO: check tend interval.
-        threading.Timer(1, self._tend).start()
+        await asyncio.sleep(1)
+        self._task = asyncio.create_task(self._tend())
 
-    def _create_channel(self, host: str, port: int, is_tls: bool) -> grpc.Channel:
+    def _create_channel(self, host: str, port: int, is_tls: bool) -> grpc.aio.Channel:
         # TODO: Take care of TLS
         host = re.sub(r"%.*", "", host)
-        return grpc.insecure_channel(f"{host}:{port}")
+        return grpc.aio.insecure_channel(f"{host}:{port}")
```

### Comparing `aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/admin_helpers.py` & `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/admin_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 logger = logging.getLogger(__name__)
 
 empty = google.protobuf.empty_pb2.Empty()
 
 
 class BaseClient(object):
 
-    def prepare_seeds(self, seeds) -> None:
-        return helpers.prepare_seeds(seeds)
+    def _prepare_seeds(self, seeds) -> None:
+        return helpers._prepare_seeds(seeds)
 
-    def prepare_index_create(self, namespace, name, vector_field, dimensions, vector_distance_metric, sets, index_params, index_meta_data, logger) -> None:
+    def _prepare_index_create(self, namespace, name, vector_field, dimensions, vector_distance_metric, sets, index_params, index_meta_data, logger) -> None:
 
         logger.debug(
             "Creating index: namespace=%s, name=%s, vector_field=%s, dimensions=%d, vector_distance_metric=%s, "
             "sets=%s, index_params=%s, index_meta_data=%s",
             namespace,
             name,
             vector_field,
@@ -37,70 +37,70 @@
             index_meta_data,
         )
 
         if sets and not sets.strip():
             sets = None
         if index_params != None:
             index_params = index_params._to_pb2()
-        id = self.get_index_id(namespace, name)
+        id = self._get_index_id(namespace, name)
         vector_distance_metric = vector_distance_metric.value
 
-        index_stub = self.get_index_stub()
+        index_stub = self._get_index_stub()
 
         index_create_request = types_pb2.IndexDefinition(
             id=id,
             vectorDistanceMetric=vector_distance_metric,
             setFilter=sets,
             hnswParams=index_params,
             bin=vector_field,
             dimensions=dimensions,
             labels=index_meta_data,
         )
         return (index_stub, index_create_request)
 
-    def prepare_index_drop(self, namespace, name, logger) -> None:
+    def _prepare_index_drop(self, namespace, name, logger) -> None:
         
         logger.debug("Dropping index: namespace=%s, name=%s", namespace, name)
 
-        index_stub = self.get_index_stub()
-        index_drop_request = self.get_index_id(namespace, name)
+        index_stub = self._get_index_stub()
+        index_drop_request = self._get_index_id(namespace, name)
 
         return (index_stub, index_drop_request)
 
-    def prepare_index_list(self, logger) -> None:
+    def _prepare_index_list(self, logger) -> None:
 
         logger.debug("Getting index list")
 
-        index_stub = self.get_index_stub()
+        index_stub = self._get_index_stub()
         index_list_request = empty
 
         return (index_stub, index_list_request)
 
-    def prepare_index_get(self, namespace, name, logger) -> None:
+    def _prepare_index_get(self, namespace, name, logger) -> None:
 
         logger.debug(
             "Getting index information: namespace=%s, name=%s", namespace, name
         )
 
-        index_stub = self.get_index_stub()
-        index_get_request = self.get_index_id(namespace, name)
+        index_stub = self._get_index_stub()
+        index_get_request = self._get_index_id(namespace, name)
 
         return (index_stub, index_get_request)
 
-    def prepare_index_get_status(self, namespace, name, logger) -> None:
+    def _prepare_index_get_status(self, namespace, name, logger) -> None:
 
         logger.debug("Getting index status: namespace=%s, name=%s", namespace, name)
 
-        index_stub = self.get_index_stub()
-        index_get_status_request = self.get_index_id(namespace, name)
+        index_stub = self._get_index_stub()
+        index_get_status_request = self._get_index_id(namespace, name)
 
 
         return (index_stub, index_get_status_request)
 
-    def respond_index_list(self, response) -> None:
+    def _respond_index_list(self, response) -> None:
         response_list = []
         for index in response.indices:
             response_dict = MessageToDict(index)
 
             # Modifying dict to adhere to PEP-8 naming
             hnsw_params_dict = response_dict.pop("hnswParams", None)
 
@@ -114,15 +114,15 @@
             )
             hnsw_params_dict["batching_params"] = batching_params_dict
 
             response_dict["hnsw_params"] = hnsw_params_dict
             response_list.append(response_dict)
         return response_list
 
-    def respond_index_get(self, response) -> None:
+    def _respond_index_get(self, response) -> None:
         response_dict = MessageToDict(response)
 
         # Modifying dict to adhere to PEP-8 naming
         hnsw_params_dict = response_dict.pop("hnswParams", None)
 
         hnsw_params_dict["ef_construction"] = hnsw_params_dict.pop(
             "efConstruction", None
@@ -133,29 +133,25 @@
             "maxRecords", None
         )
         hnsw_params_dict["batching_params"] = batching_params_dict
 
         response_dict["hnsw_params"] = hnsw_params_dict
         return response_dict
 
-    def respond_index_get_status(self, response) -> None:
+    def _respond_index_get_status(self, response) -> None:
         return response.unmergedRecordCount
 
-    def get_index_stub(self):
+    def _get_index_stub(self):
         return index_pb2_grpc.IndexServiceStub(
-            self._channelProvider.get_channel()
+            self._channel_provider.get_channel()
         )
 
-    def get_index_id(self, namespace, name):
+    def _get_index_id(self, namespace, name):
         return types_pb2.IndexId(namespace=namespace, name=name)
 
-    def prepare_wait_for_index_waiting(self, namespace, name):
-        return helpers.prepare_wait_for_index_waiting(self, namespace, name)
+    def _prepare_wait_for_index_waiting(self, namespace, name, wait_interval):
+        return helpers._prepare_wait_for_index_waiting(self, namespace, name, wait_interval)
 
 
-    def check_timeout(self, start_time, timeout):
+    def _check_timeout(self, start_time, timeout):
         if start_time + timeout < time.monotonic():
-            raise "timed-out waiting for index creation"
-
-
-
-
+            raise "timed-out waiting for index creation"
```

### Comparing `aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/base_channel_provider.py` & `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/base_channel_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,26 +19,25 @@
 
 
 class BaseChannelProvider(object):
     """Proximus Channel Provider"""
     def __init__(
         self, seeds: tuple[types.HostPort, ...], listener_name: Optional[str] = None, is_loadbalancer: Optional[bool] = False
     ) -> None:
-        if not seeds:
-            raise Exception("at least one seed host needed")
+        self.seeds: tuple[types.HostPort, ...] = seeds
+        self.listener_name: Optional[str] = listener_name
+        self._is_loadbalancer: Optional[bool] = is_loadbalancer
+        # dict of Node Number and ChannelAndEndponts object
         self._node_channels: dict[int, ChannelAndEndpoints] = {}
-        self._seedChannels: Union[dict[grpc.Channel], dict[grpc.Channel.aio]] = {}
-        self._closed = False
-        self._cluster_id = 0
-        self.seeds = seeds
-        self.listener_name = listener_name
-        self._is_loadbalancer = is_loadbalancer
-        self._seedChannels = [
+        self._seedChannels: Union[list[grpc.Channel], list[grpc.Channel.aio]] = [
             self._create_channel_from_host_port(seed) for seed in self.seeds
         ]
+        self._closed: bool = False
+        self._cluster_id: int = 0
+
 
     def get_channel(self) -> Union[grpc.aio.Channel, grpc.Channel]:
         if not self._is_loadbalancer:
             discovered_channels: list[ChannelAndEndpoints] = list(
                 self._node_channels.values())
             if len(discovered_channels) <= 0:
                 return self._seedChannels[0]
@@ -46,14 +45,15 @@
 
             # Return a random channel.
             channel = random.choice(discovered_channels).channel
             if channel:
                 return channel
 
         return self._seedChannels[0]
+
     def _create_channel_from_host_port(self, host: types.HostPort) -> Union[grpc.aio.Channel, grpc.Channel]:
         return self._create_channel(host.host, host.port, host.is_tls)
 
     def _create_channel_from_server_endpoint_list(
         self, endpoints: vector_db_pb2.ServerEndpointList
     ) -> Union[grpc.aio.Channel, grpc.Channel]:
         # TODO: Create channel with all endpoints
@@ -86,19 +86,19 @@
 
         if self._closed:
             end_tend = True
 
         # TODO: Worry about thread safety
         temp_endpoints: dict[int, vector_db_pb2.ServerEndpointList] = {}
 
-        update_endpoints = False
+        update_endpoints_stub = None
         channels = self._seedChannels + [
             x.channel for x in self._node_channels.values()
         ]
-        return (temp_endpoints, update_endpoints, channels, end_tend)
+        return (temp_endpoints, update_endpoints_stub, channels, end_tend)
 
 
     def check_cluster_id(self, new_cluster_id) -> None:
         if new_cluster_id == self._cluster_id:
             return False
 
         self._cluster_id = new_cluster_id
```

### Comparing `aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/client_helpers.py` & `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/client_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from .proto_generated import transact_pb2_grpc
 from .. import types
 from .proto_generated import types_pb2
 from . import helpers
 
 class BaseClient(object):
 
-    def prepare_seeds(self, seeds) -> None:
-        return helpers.prepare_seeds(seeds)
+    def _prepare_seeds(self, seeds) -> None:
+        return helpers._prepare_seeds(seeds)
         
-    def prepare_put(self, namespace, key, record_data, set_name, logger) -> None:
+    def _prepare_put(self, namespace, key, record_data, set_name, logger) -> None:
 
         logger.debug(
             "Putting record: namespace=%s, key=%s, record_data:%s, set_name:%s",
             namespace,
             key,
             record_data,
             set_name,
@@ -25,54 +25,54 @@
 
         key = self._get_key(namespace, set_name, key)
         bin_list = [
             types_pb2.Bin(name=k, value=conversions.toVectorDbValue(v))
             for (k, v) in record_data.items()
         ]
 
-        transact_stub = self.get_transact_stub()
+        transact_stub = self._get_transact_stub()
         put_request = transact_pb2.PutRequest(key=key, bins=bin_list)
 
         return (transact_stub, put_request)
 
-    def prepare_get(self, namespace, key, bin_names, set_name, logger) -> None:
+    def _prepare_get(self, namespace, key, bin_names, set_name, logger) -> None:
 
         logger.debug(
             "Getting record: namespace=%s, key=%s, bin_names:%s, set_name:%s",
             namespace,
             key,
             bin_names,
             set_name,
         )
 
 
         key = self._get_key(namespace, set_name, key)
         bin_selector = self._get_bin_selector(bin_names=bin_names)
 
-        transact_stub = self.get_transact_stub()
+        transact_stub = self._get_transact_stub()
         get_request = transact_pb2.GetRequest(key=key, binSelector=bin_selector)
 
         return (transact_stub, key, get_request)
 
-    def prepare_exists(self, namespace, key, set_name, logger) -> None:
+    def _prepare_exists(self, namespace, key, set_name, logger) -> None:
 
         logger.debug(
             "Getting record existence: namespace=%s, key=%s, set_name:%s",
             namespace,
             key,
             set_name,
         )
 
         key = self._get_key(namespace, set_name, key)
 
-        transact_stub = self.get_transact_stub()
+        transact_stub = self._get_transact_stub()
 
         return (transact_stub, key)
 
-    def prepare_is_indexed(self, namespace, key, index_name, index_namespace, set_name, logger) -> None:
+    def _prepare_is_indexed(self, namespace, key, index_name, index_namespace, set_name, logger) -> None:
 
         logger.debug(
             "Checking if index exists: namespace=%s, key=%s, index_name=%s, index_namespace=%s, set_name=%s",
             namespace,
             key,
             index_name,
             index_namespace,
@@ -80,20 +80,20 @@
         )
 
         if not index_namespace:
             index_namespace = namespace
         index_id = types_pb2.IndexId(namespace=index_namespace, name=index_name)
         key = self._get_key(namespace, set_name, key)
 
-        transact_stub = self.get_transact_stub()
+        transact_stub = self._get_transact_stub()
         is_indexed_request = transact_pb2.IsIndexedRequest(key=key, indexId=index_id)
 
         return (transact_stub, is_indexed_request)
 
-    def prepare_vector_search(self, namespace, index_name, query, limit, search_params, bin_names, logger) -> None:
+    def _prepare_vector_search(self, namespace, index_name, query, limit, search_params, bin_names, logger) -> None:
 
         logger.debug(
             "Performing vector search: namespace=%s, index_name=%s, query=%s, limit=%s, search_params=%s, bin_names=%s",
             namespace,
             index_name,
             query,
             limit,
@@ -104,44 +104,44 @@
         if search_params != None:
             search_params = search_params._to_pb2()
         bin_selector = self._get_bin_selector(bin_names=bin_names)
         index = types_pb2.IndexId(namespace=namespace, name=index_name)
         query_vector = conversions.toVectorDbValue(query).vectorValue
 
 
-        transact_stub = self.get_transact_stub()
+        transact_stub = self._get_transact_stub()
 
         vector_search_request = transact_pb2.VectorSearchRequest(
             index=index,
             queryVector=query_vector,
             limit=limit,
             hnswSearchParams=search_params,
             binSelector=bin_selector,
         )
         
         return (transact_stub, vector_search_request)
 
-    def get_transact_stub(self):
+    def _get_transact_stub(self):
         return transact_pb2_grpc.TransactStub(
-            self._channelProvider.get_channel()
+            self._channel_provider.get_channel()
         )
 
-    def respond_get(self, response, key) -> None:
+    def _respond_get(self, response, key) -> None:
         return types.RecordWithKey(
             key=conversions.fromVectorDbKey(key),
             bins=conversions.fromVectorDbRecord(response),
         )
 
-    def respond_exists(self, response) -> None:
+    def _respond_exists(self, response) -> None:
         return response.value
 
-    def respond_is_indexed(self, response) -> None:
+    def _respond_is_indexed(self, response) -> None:
         return response.value
 
-    def respond_neighbor(self, response) -> None:
+    def _respond_neighbor(self, response) -> None:
         return conversions.fromVectorDbNeighbor(response)
 
     def _get_bin_selector(self, *, bin_names: Optional[list] = None):
 
         if not bin_names:
             bin_selector = transact_pb2.BinSelector(
                 type=transact_pb2.BinSelectorType.ALL, binNames=bin_names
@@ -159,18 +159,18 @@
             key = types_pb2.Key(namespace=namespace, set=set, longValue=key)
         elif isinstance(key, (bytes, bytearray)):
             key = types_pb2.Key(namespace=namespace, set=set, bytesValue=key)
         else:
             raise Exception("Invalid key type" + type(key))
         return key
 
-    def prepare_wait_for_index_waiting(self, namespace, name):
-        return helpers.prepare_wait_for_index_waiting(self, namespace, name)
+    def _prepare_wait_for_index_waiting(self, namespace, name, wait_interval):
+        return helpers._prepare_wait_for_index_waiting(self, namespace, name, wait_interval)
 
-    def check_completion_condition(self, start_time, timeout, index_status, unmerged_record_initialized):
+    def _check_completion_condition(self, start_time, timeout, index_status, unmerged_record_initialized):
 
         if start_time + 10 < time.monotonic():
             unmerged_record_initialized = True
             
         if index_status.unmergedRecordCount > 0:
             unmerged_record_initialized = True
```

### Comparing `aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/conversions.py` & `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/conversions.py`

 * *Files identical despite different names*

### Comparing `aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/helpers.py` & `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import time
 from .. import types
 from .proto_generated import types_pb2
 from .proto_generated import index_pb2_grpc
 
-def prepare_seeds(seeds) -> None:
+def _prepare_seeds(seeds) -> None:
 
     if not seeds:
         raise Exception("at least one seed host needed")
 
     if isinstance(seeds, types.HostPort):
         seeds = (seeds,)
 
     return seeds
 
 
-def prepare_wait_for_index_waiting(self, namespace, name):
+def _prepare_wait_for_index_waiting(self, namespace, name, wait_interval):
 
-    wait_interval = 5
     unmerged_record_initialized = False
     start_time = time.monotonic()
     double_check = False
 
     index_stub = index_pb2_grpc.IndexServiceStub(
-        self._channelProvider.get_channel()
+        self._channel_provider.get_channel()
     )
     index_wait_request = types_pb2.IndexId(namespace=namespace, name=name)
     return (index_stub, wait_interval, start_time, unmerged_record_initialized, False, index_wait_request)
```

### Comparing `aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/proto_generated/auth_pb2.py` & `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/proto_generated/auth_pb2_grpc.py` & `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/auth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/proto_generated/index_pb2.py` & `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/index_pb2.py`

 * *Files identical despite different names*

### Comparing `aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/proto_generated/index_pb2_grpc.py` & `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/index_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/proto_generated/transact_pb2.py` & `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/transact_pb2.py`

 * *Files identical despite different names*

### Comparing `aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/proto_generated/transact_pb2_grpc.py` & `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/transact_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/proto_generated/types_pb2.py` & `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/types_pb2.py`

 * *Files identical despite different names*

### Comparing `aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/proto_generated/vector_db_pb2.py` & `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/vector_db_pb2.py`

 * *Files identical despite different names*

### Comparing `aerospike-vector-search-0.5.0/src/aerospike_vector_search/shared/proto_generated/vector_db_pb2_grpc.py` & `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/vector_db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aerospike-vector-search-0.5.0/src/aerospike_vector_search/types.py` & `aerospike-vector-search-0.5.1/src/aerospike_vector_search/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     """
 
     def __init__(self, *, host: str, port: int, is_tls: Optional[bool] = False) -> None:
         self.host = host
         self.port = port
         self.is_tls = is_tls
 
-
 class Key(object):
     """
     Represents a record key.
     Used in RecordWithKey.
 
     Args:
         namespace (str): The namespace for the key.
```

### Comparing `aerospike-vector-search-0.5.0/src/aerospike_vector_search.egg-info/PKG-INFO` & `aerospike-vector-search-0.5.1/src/aerospike_vector_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aerospike-vector-search
-Version: 0.5.0
+Version: 0.5.1
 Summary: Aerospike Proximus Client Library for Python
 Author-email: "Aerospike, Inc." <info@aerospike.com>
 License: Apache Software License
 Project-URL: Homepage, https://aerospike.com
 Keywords: aerospike,vector,database,ANN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `aerospike-vector-search-0.5.0/src/aerospike_vector_search.egg-info/SOURCES.txt` & `aerospike-vector-search-0.5.1/src/aerospike_vector_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

