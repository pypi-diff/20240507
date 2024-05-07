# Comparing `tmp/crosslab_soa_service_file-0.2.7.tar.gz` & `tmp/crosslab_soa_service_file-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslab_soa_service_file-0.2.7.tar", last modified: Fri Apr  5 09:17:29 2024, max compression
+gzip compressed data, was "crosslab_soa_service_file-0.2.8.tar", last modified: Tue May  7 16:57:34 2024, max compression
```

## Comparing `crosslab_soa_service_file-0.2.7.tar` & `crosslab_soa_service_file-0.2.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:29.974671 crosslab_soa_service_file-0.2.7/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      399 2024-04-05 09:17:29.974671 crosslab_soa_service_file-0.2.7/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-11-08 12:05:40.000000 crosslab_soa_service_file-0.2.7/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)      574 2024-04-05 09:17:29.974671 crosslab_soa_service_file-0.2.7/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)       37 2023-11-08 12:05:40.000000 crosslab_soa_service_file-0.2.7/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:29.974671 crosslab_soa_service_file-0.2.7/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:29.974671 crosslab_soa_service_file-0.2.7/src/crosslab/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:29.974671 crosslab_soa_service_file-0.2.7/src/crosslab/soa_services/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:29.974671 crosslab_soa_service_file-0.2.7/src/crosslab/soa_services/file/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      192 2023-11-08 12:05:40.000000 crosslab_soa_service_file-0.2.7/src/crosslab/soa_services/file/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2551 2023-11-08 12:05:40.000000 crosslab_soa_service_file-0.2.7/src/crosslab/soa_services/file/file_service.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      222 2023-11-08 12:05:40.000000 crosslab_soa_service_file-0.2.7/src/crosslab/soa_services/file/messages.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_service_file-0.2.7/src/crosslab/soa_services/file/py.typed
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:29.974671 crosslab_soa_service_file-0.2.7/src/crosslab_soa_service_file.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      399 2024-04-05 09:17:29.000000 crosslab_soa_service_file-0.2.7/src/crosslab_soa_service_file.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      493 2024-04-05 09:17:29.000000 crosslab_soa_service_file-0.2.7/src/crosslab_soa_service_file.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-04-05 09:17:29.000000 crosslab_soa_service_file-0.2.7/src/crosslab_soa_service_file.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       25 2024-04-05 09:17:29.000000 crosslab_soa_service_file-0.2.7/src/crosslab_soa_service_file.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2024-04-05 09:17:29.000000 crosslab_soa_service_file-0.2.7/src/crosslab_soa_service_file.egg-info/top_level.txt
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:29.974671 crosslab_soa_service_file-0.2.7/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      898 2023-11-08 12:05:40.000000 crosslab_soa_service_file-0.2.7/tests/test_standard.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 16:57:34.459480 crosslab_soa_service_file-0.2.8/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      399 2024-05-07 16:57:34.459480 crosslab_soa_service_file-0.2.8/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-11-08 12:05:40.000000 crosslab_soa_service_file-0.2.8/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      574 2024-05-07 16:57:34.459480 crosslab_soa_service_file-0.2.8/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       37 2023-11-08 12:05:40.000000 crosslab_soa_service_file-0.2.8/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 16:57:34.455480 crosslab_soa_service_file-0.2.8/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 16:57:34.455480 crosslab_soa_service_file-0.2.8/src/crosslab/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 16:57:34.455480 crosslab_soa_service_file-0.2.8/src/crosslab/soa_services/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 16:57:34.459480 crosslab_soa_service_file-0.2.8/src/crosslab/soa_services/file/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      192 2024-04-22 18:51:13.000000 crosslab_soa_service_file-0.2.8/src/crosslab/soa_services/file/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3134 2024-05-07 16:28:32.000000 crosslab_soa_service_file-0.2.8/src/crosslab/soa_services/file/file_service.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      222 2023-11-08 12:05:40.000000 crosslab_soa_service_file-0.2.8/src/crosslab/soa_services/file/messages.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_service_file-0.2.8/src/crosslab/soa_services/file/py.typed
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 16:57:34.459480 crosslab_soa_service_file-0.2.8/src/crosslab_soa_service_file.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      399 2024-05-07 16:57:34.000000 crosslab_soa_service_file-0.2.8/src/crosslab_soa_service_file.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      493 2024-05-07 16:57:34.000000 crosslab_soa_service_file-0.2.8/src/crosslab_soa_service_file.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-05-07 16:57:34.000000 crosslab_soa_service_file-0.2.8/src/crosslab_soa_service_file.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       25 2024-05-07 16:57:34.000000 crosslab_soa_service_file-0.2.8/src/crosslab_soa_service_file.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2024-05-07 16:57:34.000000 crosslab_soa_service_file-0.2.8/src/crosslab_soa_service_file.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 16:57:34.459480 crosslab_soa_service_file-0.2.8/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      898 2023-11-08 12:05:40.000000 crosslab_soa_service_file-0.2.8/tests/test_standard.py
```

### Comparing `crosslab_soa_service_file-0.2.7/setup.cfg` & `crosslab_soa_service_file-0.2.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosslab_soa_service_file
-version = 0.2.7
+version = 0.2.8
 author = Johannes Nau
 author_email = johannes.nau@tu-ilmenau.de
 description = The CrossLab SOA file Service.
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Other/Proprietary License
 	Operating System :: OS Independent
```

### Comparing `crosslab_soa_service_file-0.2.7/src/crosslab/soa_services/file/file_service.py` & `crosslab_soa_service_file-0.2.8/src/crosslab/soa_services/file/file_service.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 from typing import Union
 
 from crosslab.soa_client.connection import Connection, DataChannel
 from crosslab.soa_client.service import Service
-from pyee.asyncio import AsyncIOEventEmitter
-
 from crosslab.soa_services.file.messages import FileServiceConfig, FileServiceEvent
+from pyee.asyncio import AsyncIOEventEmitter
 
 
 class FileService__Producer(Service):
     service_type = "https://api.goldi-labs.de/serviceTypes/file"
     service_direction = "producer"
     service_id: str
 
@@ -30,16 +29,22 @@
         else:
             connection.receive(serviceConfig, "data", self.channel)
 
     def teardownConnection(self, connection: Connection):
         pass
 
     async def sendFile(self, file_type: str, content: bytes):
+        await self.channel.ready()
         self.channel.send(json.dumps({"fileType": file_type, "length": len(content)}))
-        self.channel.send(content)
+        # fragment to 8kb chunks
+        chunkSize = 8192
+        for i in range(0, len(content), chunkSize):
+            chunk = bytes(content[i : i + chunkSize])
+            print(len(chunk))
+            self.channel.send(chunk)
 
 
 class FileService__Consumer(Service, AsyncIOEventEmitter):
     service_type = "https://api.goldi-labs.de/serviceTypes/file"
     service_direction = "consumer"
     service_id: str
 
@@ -65,10 +70,20 @@
     def teardownConnection(self, connection: Connection):
         pass
 
     def handleData(self, data: Union[str, bytes]):
         if isinstance(data, str):
             header = json.loads(data)
             self.file_type = header["fileType"]
+            self.file_length = header["length"]
+            self.dataRead = 0
+            self.dataBuffer = b""
         elif self.file_type is not None:
-            event: FileServiceEvent = {"file_type": self.file_type, "content": data}
-            self.emit("file", event)
+            self.dataBuffer += data
+            self.dataRead += len(data)
+            if self.dataRead == self.file_length:
+                event: FileServiceEvent = {
+                    "file_type": self.file_type,
+                    "content": self.dataBuffer,
+                }
+                self.emit("file", event)
+                self.file_type = None
```

### Comparing `crosslab_soa_service_file-0.2.7/tests/test_standard.py` & `crosslab_soa_service_file-0.2.8/tests/test_standard.py`

 * *Files identical despite different names*

