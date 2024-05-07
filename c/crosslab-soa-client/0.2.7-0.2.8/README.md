# Comparing `tmp/crosslab_soa_client-0.2.7.tar.gz` & `tmp/crosslab_soa_client-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslab_soa_client-0.2.7.tar", last modified: Fri Apr  5 09:16:59 2024, max compression
+gzip compressed data, was "crosslab_soa_client-0.2.8.tar", last modified: Tue May  7 17:13:24 2024, max compression
```

## Comparing `crosslab_soa_client-0.2.7.tar` & `crosslab_soa_client-0.2.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:16:59.030526 crosslab_soa_client-0.2.7/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      397 2024-04-05 09:16:59.030526 crosslab_soa_client-0.2.7/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2494 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)      617 2024-04-05 09:16:59.030526 crosslab_soa_client-0.2.7/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)       37 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:16:59.026526 crosslab_soa_client-0.2.7/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:16:59.026526 crosslab_soa_client-0.2.7/src/crosslab/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:16:59.030526 crosslab_soa_client-0.2.7/src/crosslab/soa_client/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1774 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/connection.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10234 2023-12-11 21:52:54.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/connection_webrtc.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7790 2024-03-01 08:08:11.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/device_handler.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:16:59.030526 crosslab_soa_client-0.2.7/src/crosslab/soa_client/media/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/media/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      395 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/media/gst_track.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      557 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/media/udp_track.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/message_handling.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1623 2024-03-01 08:08:11.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/messages.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/py.typed
--rw-r--r--   0 vscode    (1000) vscode    (1000)      778 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/service.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:16:59.030526 crosslab_soa_client-0.2.7/src/crosslab/soa_client/test_helper/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       81 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/test_helper/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1051 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/test_helper/connection_stub.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      787 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/test_helper/dummy_track.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4331 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/test_helper/service_stub.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:16:59.030526 crosslab_soa_client-0.2.7/src/crosslab_soa_client.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      397 2024-04-05 09:16:59.000000 crosslab_soa_client-0.2.7/src/crosslab_soa_client.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      981 2024-04-05 09:16:59.000000 crosslab_soa_client-0.2.7/src/crosslab_soa_client.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-04-05 09:16:59.000000 crosslab_soa_client-0.2.7/src/crosslab_soa_client.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       36 2024-04-05 09:16:59.000000 crosslab_soa_client-0.2.7/src/crosslab_soa_client.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2024-04-05 09:16:59.000000 crosslab_soa_client-0.2.7/src/crosslab_soa_client.egg-info/top_level.txt
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:16:59.030526 crosslab_soa_client-0.2.7/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2046 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/tests/test_device_handler.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5239 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/tests/test_webrtc_connection.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 17:13:24.816310 crosslab_soa_client-0.2.8/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      397 2024-05-07 17:13:24.816310 crosslab_soa_client-0.2.8/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2494 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.8/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.8/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      617 2024-05-07 17:13:24.816310 crosslab_soa_client-0.2.8/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       37 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.8/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 17:13:24.812310 crosslab_soa_client-0.2.8/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 17:13:24.812310 crosslab_soa_client-0.2.8/src/crosslab/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 17:13:24.812310 crosslab_soa_client-0.2.8/src/crosslab/soa_client/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.8/src/crosslab/soa_client/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2049 2024-05-07 16:28:32.000000 crosslab_soa_client-0.2.8/src/crosslab/soa_client/connection.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10234 2024-05-07 16:21:09.000000 crosslab_soa_client-0.2.8/src/crosslab/soa_client/connection_webrtc.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7790 2024-05-07 16:28:32.000000 crosslab_soa_client-0.2.8/src/crosslab/soa_client/device_handler.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 17:13:24.816310 crosslab_soa_client-0.2.8/src/crosslab/soa_client/media/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.8/src/crosslab/soa_client/media/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      395 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.8/src/crosslab/soa_client/media/gst_track.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      557 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.8/src/crosslab/soa_client/media/udp_track.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.8/src/crosslab/soa_client/message_handling.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1623 2024-05-07 16:28:32.000000 crosslab_soa_client-0.2.8/src/crosslab/soa_client/messages.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.8/src/crosslab/soa_client/py.typed
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      778 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.8/src/crosslab/soa_client/service.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 17:13:24.816310 crosslab_soa_client-0.2.8/src/crosslab/soa_client/test_helper/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       81 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.8/src/crosslab/soa_client/test_helper/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1119 2024-05-07 16:28:32.000000 crosslab_soa_client-0.2.8/src/crosslab/soa_client/test_helper/connection_stub.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      787 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.8/src/crosslab/soa_client/test_helper/dummy_track.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4331 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.8/src/crosslab/soa_client/test_helper/service_stub.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 17:13:24.816310 crosslab_soa_client-0.2.8/src/crosslab_soa_client.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      397 2024-05-07 17:13:24.000000 crosslab_soa_client-0.2.8/src/crosslab_soa_client.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      981 2024-05-07 17:13:24.000000 crosslab_soa_client-0.2.8/src/crosslab_soa_client.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-05-07 17:13:24.000000 crosslab_soa_client-0.2.8/src/crosslab_soa_client.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       36 2024-05-07 17:13:24.000000 crosslab_soa_client-0.2.8/src/crosslab_soa_client.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2024-05-07 17:13:24.000000 crosslab_soa_client-0.2.8/src/crosslab_soa_client.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 17:13:24.816310 crosslab_soa_client-0.2.8/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2046 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.8/tests/test_device_handler.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5239 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.8/tests/test_webrtc_connection.py
```

### Comparing `crosslab_soa_client-0.2.7/README.md` & `crosslab_soa_client-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.7/setup.cfg` & `crosslab_soa_client-0.2.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosslab_soa_client
-version = 0.2.7
+version = 0.2.8
 author = Johannes Nau
 author_email = johannes.nau@tu-ilmenau.de
 description = The CrossLab SOA Client
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Other/Proprietary License
 	Operating System :: OS Independent
```

### Comparing `crosslab_soa_client-0.2.7/src/crosslab/soa_client/connection.py` & `crosslab_soa_client-0.2.8/src/crosslab/soa_client/connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 from abc import ABC, abstractmethod
 from typing import Any, Literal, Optional, Union
 
 from crosslab.soa_client.messages import SignalingMessage
 from pyee.asyncio import AsyncIOEventEmitter  # type: ignore
 
 MediaStreamTrack = Any
@@ -26,22 +27,31 @@
     def close(self):
         self.emit("close")
         self.remove_all_listeners()
 
 
 class DataChannel(Channel, AsyncIOEventEmitter):
     channel_type = "DataChannel"
+    _ready = False
 
     def send(self, data: Union[bytes, str]):
         self.emit("upstreamData", data)
 
     def downstreamData(self, data: Union[bytes, str]):
         self.emit("data", data)
 
+    async def ready(self):
+        if self._ready:
+            return
+        _future = asyncio.get_running_loop().create_future()
+        self.once("open", lambda: _future.set_result(None))
+        await _future
+
     async def opened(self):
+        self._ready = True
         self.emit("open")
 
     def close(self):
         self.emit("close")
         self.remove_all_listeners()
```

### Comparing `crosslab_soa_client-0.2.7/src/crosslab/soa_client/connection_webrtc.py` & `crosslab_soa_client-0.2.8/src/crosslab/soa_client/connection_webrtc.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.7/src/crosslab/soa_client/device_handler.py` & `crosslab_soa_client-0.2.8/src/crosslab/soa_client/device_handler.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.7/src/crosslab/soa_client/media/udp_track.py` & `crosslab_soa_client-0.2.8/src/crosslab/soa_client/media/udp_track.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.7/src/crosslab/soa_client/messages.py` & `crosslab_soa_client-0.2.8/src/crosslab/soa_client/messages.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.7/src/crosslab/soa_client/service.py` & `crosslab_soa_client-0.2.8/src/crosslab/soa_client/service.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.7/src/crosslab/soa_client/test_helper/connection_stub.py` & `crosslab_soa_client-0.2.8/src/crosslab/soa_client/test_helper/connection_stub.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,21 +13,23 @@
         self.channels.clear()
 
     def transmit(self, serviceConfig, id: str, channel):
         self.messages[id] = []
         self.channels[id] = channel
         if isinstance(channel, DataChannel):
             channel.on("upstreamData", lambda data: self.messages[id].append(data))
+            channel._ready = True
             channel.emit("open")
 
     def receive(self, serviceConfig, id: str, channel):
         pass
         self.messages[id] = []
         self.channels[id] = channel
         if isinstance(channel, DataChannel):
             channel.on("upstreamData", lambda data: self.messages[id].append(data))
+            channel._ready = True
             channel.emit("open")
 
     def handleSignalingMessage(self, message):
         raise NotImplementedError()
 
     pass
```

### Comparing `crosslab_soa_client-0.2.7/src/crosslab/soa_client/test_helper/dummy_track.py` & `crosslab_soa_client-0.2.8/src/crosslab/soa_client/test_helper/dummy_track.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.7/src/crosslab/soa_client/test_helper/service_stub.py` & `crosslab_soa_client-0.2.8/src/crosslab/soa_client/test_helper/service_stub.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.7/src/crosslab_soa_client.egg-info/SOURCES.txt` & `crosslab_soa_client-0.2.8/src/crosslab_soa_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.7/tests/test_device_handler.py` & `crosslab_soa_client-0.2.8/tests/test_device_handler.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.7/tests/test_webrtc_connection.py` & `crosslab_soa_client-0.2.8/tests/test_webrtc_connection.py`

 * *Files identical despite different names*

