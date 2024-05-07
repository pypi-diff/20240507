# Comparing `tmp/assetsstore-1.1.0.tar.gz` & `tmp/assetsstore-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assetsstore-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "assetsstore-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `assetsstore-1.1.0.tar` & `assetsstore-1.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       91 2024-04-10 15:51:30.190093 assetsstore-1.1.0/.flake8
--rw-r--r--   0        0        0     1776 2024-04-10 15:51:30.190093 assetsstore-1.1.0/.gitignore
--rw-r--r--   0        0        0      366 2024-04-10 15:51:30.190093 assetsstore-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11358 2024-04-08 11:14:38.232095 assetsstore-1.1.0/LICENSE
--rw-r--r--   0        0        0     2179 2024-04-10 15:51:30.190093 assetsstore-1.1.0/README.md
--rw-r--r--   0        0        0      104 2024-04-23 09:37:13.843635 assetsstore-1.1.0/assetsstore/__init__.py
--rw-r--r--   0        0        0       64 2024-04-23 09:37:13.843635 assetsstore-1.1.0/assetsstore/assets/__init__.py
--rw-r--r--   0        0        0     6667 2024-04-23 09:37:13.843635 assetsstore-1.1.0/assetsstore/assets/assets.py
--rw-r--r--   0        0        0       62 2024-04-10 15:51:30.194093 assetsstore-1.1.0/assetsstore/assets/azr/__init__.py
--rw-r--r--   0        0        0     5690 2024-04-10 15:51:30.194093 assetsstore-1.1.0/assetsstore/assets/azr/azure_files.py
--rw-r--r--   0        0        0       62 2024-04-10 15:51:30.194093 assetsstore-1.1.0/assetsstore/assets/local/__init__.py
--rw-r--r--   0        0        0     4241 2024-04-10 15:51:30.194093 assetsstore-1.1.0/assetsstore/assets/local/local_files.py
--rw-r--r--   0        0        0       56 2024-04-10 15:51:30.194093 assetsstore-1.1.0/assetsstore/assets/minio/__init__.py
--rw-r--r--   0        0        0     8983 2024-04-10 15:51:30.194093 assetsstore-1.1.0/assetsstore/assets/minio/minio.py
--rw-r--r--   0        0        0     6234 2024-04-10 15:51:30.194093 assetsstore-1.1.0/assetsstore/assets/minio/progress.py
--rw-r--r--   0        0        0       53 2024-04-10 15:51:30.194093 assetsstore-1.1.0/assetsstore/assets/s3/__init__.py
--rw-r--r--   0        0        0    11381 2024-04-10 15:51:30.194093 assetsstore-1.1.0/assetsstore/assets/s3/s3_files.py
--rw-r--r--   0        0        0       65 2024-04-10 15:51:30.194093 assetsstore-1.1.0/assetsstore/assets/server/__init__.py
--rw-r--r--   0        0        0     7486 2024-04-10 15:51:30.194093 assetsstore-1.1.0/assetsstore/assets/server/server_files.py
--rw-r--r--   0        0        0        0 2024-04-10 15:51:30.194093 assetsstore-1.1.0/assetsstore/tests/__init__.py
--rw-r--r--   0        0        0     1751 2024-04-23 09:37:13.843635 assetsstore-1.1.0/assetsstore/tests/assets_test.py
--rw-r--r--   0        0        0        0 2024-04-08 11:14:38.232095 assetsstore-1.1.0/assetsstore/tests/fixtures/test.txt
--rw-r--r--   0        0        0       19 2024-04-08 11:14:38.232095 assetsstore-1.1.0/assetsstore/tests/fixtures/test_folder/test2.txt
--rw-r--r--   0        0        0     4085 2024-04-10 15:51:30.194093 assetsstore-1.1.0/assetsstore/tests/test_minio.py
--rw-r--r--   0        0        0      262 2024-04-08 11:14:38.232095 assetsstore-1.1.0/docker-compose.yml
--rw-r--r--   0        0        0      960 2024-04-23 09:37:13.843635 assetsstore-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3171 1970-01-01 00:00:00.000000 assetsstore-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       91 2024-04-10 08:28:00.409764 assetsstore-1.3.0/.flake8
+-rw-r--r--   0        0        0     1776 2024-04-10 13:09:37.356566 assetsstore-1.3.0/.gitignore
+-rw-r--r--   0        0        0      392 2024-05-07 10:29:26.538153 assetsstore-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11358 2024-04-08 10:58:38.589211 assetsstore-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2179 2024-04-10 13:33:14.652681 assetsstore-1.3.0/README.md
+-rw-r--r--   0        0        0      104 2024-05-07 10:31:05.359119 assetsstore-1.3.0/assetsstore/__init__.py
+-rw-r--r--   0        0        0       64 2024-04-23 09:28:30.458153 assetsstore-1.3.0/assetsstore/assets/__init__.py
+-rw-r--r--   0        0        0     6901 2024-05-07 10:19:30.038656 assetsstore-1.3.0/assetsstore/assets/assets.py
+-rw-r--r--   0        0        0       62 2024-04-10 08:39:38.191992 assetsstore-1.3.0/assetsstore/assets/azr/__init__.py
+-rw-r--r--   0        0        0     5746 2024-05-07 10:26:29.199925 assetsstore-1.3.0/assetsstore/assets/azr/azure_files.py
+-rw-r--r--   0        0        0       62 2024-04-10 08:39:38.191992 assetsstore-1.3.0/assetsstore/assets/local/__init__.py
+-rw-r--r--   0        0        0     4297 2024-05-07 10:26:22.191836 assetsstore-1.3.0/assetsstore/assets/local/local_files.py
+-rw-r--r--   0        0        0       56 2024-04-10 08:39:38.195992 assetsstore-1.3.0/assetsstore/assets/minio/__init__.py
+-rw-r--r--   0        0        0     9619 2024-05-07 10:21:12.139940 assetsstore-1.3.0/assetsstore/assets/minio/minio.py
+-rw-r--r--   0        0        0     6234 2024-04-10 08:39:38.299993 assetsstore-1.3.0/assetsstore/assets/minio/progress.py
+-rw-r--r--   0        0        0       53 2024-04-10 08:39:38.195992 assetsstore-1.3.0/assetsstore/assets/s3/__init__.py
+-rw-r--r--   0        0        0    11879 2024-05-07 10:25:54.795492 assetsstore-1.3.0/assetsstore/assets/s3/s3_files.py
+-rw-r--r--   0        0        0       65 2024-04-10 08:39:38.191992 assetsstore-1.3.0/assetsstore/assets/server/__init__.py
+-rw-r--r--   0        0        0     7542 2024-05-07 10:26:39.376052 assetsstore-1.3.0/assetsstore/assets/server/server_files.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:52:27.137433 assetsstore-1.3.0/assetsstore/tests/__init__.py
+-rw-r--r--   0        0        0     1751 2024-04-23 09:32:47.832953 assetsstore-1.3.0/assetsstore/tests/assets_test.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:58:38.589211 assetsstore-1.3.0/assetsstore/tests/fixtures/test.txt
+-rw-r--r--   0        0        0       19 2024-04-08 10:58:38.589211 assetsstore-1.3.0/assetsstore/tests/fixtures/test_folder/test2.txt
+-rw-r--r--   0        0        0     4465 2024-05-07 10:28:49.365686 assetsstore-1.3.0/assetsstore/tests/test_minio.py
+-rw-r--r--   0        0        0      262 2024-04-08 10:58:38.589211 assetsstore-1.3.0/docker-compose.yml
+-rw-r--r--   0        0        0      960 2024-04-10 18:35:56.114971 assetsstore-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3171 1970-01-01 00:00:00.000000 assetsstore-1.3.0/PKG-INFO
```

### Comparing `assetsstore-1.1.0/.gitignore` & `assetsstore-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `assetsstore-1.1.0/LICENSE` & `assetsstore-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `assetsstore-1.1.0/README.md` & `assetsstore-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `assetsstore-1.1.0/assetsstore/assets/assets.py` & `assetsstore-1.3.0/assetsstore/assets/assets.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,22 @@
     def get_access(self, filename: str, seconds: int):
         """
         Abstract method that needs to be implemented by subclasses.
         Retrieves access to a file for a specified duration.
         """
         raise NotImplementedError
 
+    @abc.abstractmethod
+    def check_if_exists(self, path: str):
+        """
+        Abstract method that needs to be implemented by subclasses.
+        Checks if desired object exists.
+        """
+        raise NotImplementedError
+
     def put_folder(self, path: str):
         """
         Uploads a folder to the asset store by
         recursively uploading all files and subfolders.
         """
         local_folder = os.path.join(self.local_store, path)
         self._put_folder(local_folder)
```

### Comparing `assetsstore-1.1.0/assetsstore/assets/azr/azure_files.py` & `assetsstore-1.3.0/assetsstore/assets/azr/azure_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 
         self.connection = BlockBlobService(
             account_name=self.azure_storage_name,
             account_key=self.azure_storage_key,
         )
         super().__init__()
 
+    def check_if_exists(self, path: str):
+        pass
+
     def get_access(self, filename: str, seconds: int = 0, *args, **kwargs):
         """
         Get the access URL for a file in Azure.
 
         Args:
             filename (str): The name of the file.
             seconds (int, optional): The number of seconds
```

### Comparing `assetsstore-1.1.0/assetsstore/assets/local/local_files.py` & `assetsstore-1.3.0/assetsstore/assets/local/local_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,17 @@
     """
 
     def __init__(self):
         self.location = os.getenv("ASSET_LOCATION")
         self.server_url = os.getenv("ASSET_PUBLIC_URL")
         super().__init__()
 
+    def check_if_exists(self, path: str):
+        pass
+
     def get_access(self, filename: str, *args, **kwargs):
         """
         Get the access URL for a file.
 
         Args:
             filename (str): The name of the file.
```

### Comparing `assetsstore-1.1.0/assetsstore/assets/minio/minio.py` & `assetsstore-1.3.0/assetsstore/assets/minio/minio.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,35 @@
         self.host = os.getenv("ASSET_PUBLIC_URL", "localhost:9000")
         self.tls_enabled = os.getenv("ASSET_TLS_ENABLED", False)
         self.client = Minio(
             self.host, self.access_key, self.secret_key, secure=self.tls_enabled
         )
         super().__init__()
 
+    def check_if_exists(self, path: str):
+        """
+        Checks if desired object exists.
+        Args:
+            path (str): The path in the Minio bucket.
+
+        Returns:
+            bool: True if file exists, False otherwise.
+        """
+        response = None
+        try:
+            response = self.client.get_object(self.bucket_name, path)
+            success = True
+        except Exception as e:
+            success = False
+            logger.warn("Cannot access bucket object. Exception {}".format(str(e)))
+        if response:
+            response.close()
+            response.release_conn()
+        return success
+
     def get_size(self, folder: str):
         """
         Get the total size of a folder in the Minio bucket.
 
         Args:
             folder (str): The folder path in the Minio bucket.
```

### Comparing `assetsstore-1.1.0/assetsstore/assets/minio/progress.py` & `assetsstore-1.3.0/assetsstore/assets/minio/progress.py`

 * *Files identical despite different names*

### Comparing `assetsstore-1.1.0/assetsstore/assets/s3/s3_files.py` & `assetsstore-1.3.0/assetsstore/assets/s3/s3_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,14 +71,30 @@
             session = boto3.Session()
         self.connection = session.client(
             "s3", config=Config(region_name=self.region_name, signature_version="s3v4")
         )
         self.resource = session.resource("s3")
         super().__init__()
 
+    def check_if_exists(self, path: str):
+        """
+        Checks if desired object exists.
+        Args:
+            path (str): The path in the S3 bucket.
+
+        Returns:
+            bool: True if file exists, False otherwise.
+        """
+        try:
+            self.connection.head_object(Bucket=self.s3_bucket_name, Key=path)
+            return True
+        except Exception as e:
+            logger.warn("Cannot access bucket object. Exception {}".format(str(e)))
+        return False
+
     def get_size(self, folder: str):
         """
         Get the total size of files in a folder in the S3 bucket.
 
         Args:
             folder (str): The folder path in the S3 bucket.
```

### Comparing `assetsstore-1.1.0/assetsstore/assets/server/server_files.py` & `assetsstore-1.3.0/assetsstore/assets/server/server_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,17 @@
         else:
             self.password = os.getenv("ASSET_SECRET_ACCESS_KEY")
             self.ssh.connect(
                 self.server, username=self.username, password=self.password
             )
         super().__init__()
 
+    def check_if_exists(self, path: str):
+        pass
+
     def get_access(self, filename, *args, **kwargs):
         """
         Get the access URL for a file.
 
         Args:
             filename (str): The name of the file.
```

### Comparing `assetsstore-1.1.0/assetsstore/tests/assets_test.py` & `assetsstore-1.3.0/assetsstore/tests/assets_test.py`

 * *Files identical despite different names*

### Comparing `assetsstore-1.1.0/assetsstore/tests/test_minio.py` & `assetsstore-1.3.0/assetsstore/tests/test_minio.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import os
 import logging
 import json
 import requests
 
 
 class AsssetsLocalTest(TestCase):
-
     def setUp(self):
         os.environ["ASSET_STORE"] = "MinioFiles"
         os.environ["ASSET_ACCESS_KEY"] = "minio"
         os.environ["ASSET_SECRET_ACCESS_KEY"] = "minio123"
         os.environ["ASSET_LOCATION"] = "test"
         os.environ["LOCAL_STORE"] = "assetsstore/tests/fixtures/"
         self.maxDiff = None
@@ -93,14 +92,21 @@
 
     def test_get_folder_size(self):
         handler = FileAssets.get_asset()
         self.assertEqual(True, handler.put_file("test_folder/test2.txt"))
         self.assertEqual(19, handler.get_size("test_folder"))
         self.assertEqual(True, handler.del_file("test_folder/test2.txt"))
 
+    def test_check_if_file_exists(self):
+        handler = FileAssets.get_asset()
+        self.assertEqual(True, handler.put_file("test_folder/test2.txt"))
+        self.assertTrue(handler.check_if_exists("test_folder/test2.txt"))
+        self.assertFalse(handler.check_if_exists("test_folder/test33.txt"))
+        self.assertEqual(True, handler.del_file("test_folder/test2.txt"))
+
     def tearDown(self):
         handler = FileAssets.get_asset()
         handler.client.remove_bucket("test")
         for file in glob.glob("results/*"):
             if ".gitkeep" not in file:
                 os.remove(file)
         for file in glob.glob("results/remote/*"):
```

### Comparing `assetsstore-1.1.0/pyproject.toml` & `assetsstore-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `assetsstore-1.1.0/PKG-INFO` & `assetsstore-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AssetsStore
-Version: 1.1.0
+Version: 1.3.0
 Summary: Python package for managing file upload/download via selected file system.
 Author-email: Nebojsa Mrkic <mrkic.nebojsa@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: requests>=2.28.2
 Requires-Dist: urllib3>=2.0.0
 Requires-Dist: azure-storage-blob==2.1.0 ; extra == "azure"
```

