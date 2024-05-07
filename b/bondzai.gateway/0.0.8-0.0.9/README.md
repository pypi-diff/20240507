# Comparing `tmp/bondzai.gateway-0.0.8.tar.gz` & `tmp/bondzai.gateway-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.gateway-0.0.8.tar", last modified: Mon Jul 31 12:28:29 2023, max compression
+gzip compressed data, was "bondzai.gateway-0.0.9.tar", last modified: Mon Oct 23 14:49:01 2023, max compression
```

## Comparing `bondzai.gateway-0.0.8.tar` & `bondzai.gateway-0.0.9.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:28:29.511279 bondzai.gateway-0.0.8/
--rw-r--r--   0 theo       (501) staff       (20)      547 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/NOTICE
--rw-r--r--   0 theo       (501) staff       (20)      596 2023-07-31 12:28:29.511500 bondzai.gateway-0.0.8/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      195 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/README.rst
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:28:29.496926 bondzai.gateway-0.0.8/bondzai/
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:28:29.499224 bondzai.gateway-0.0.8/bondzai/gateway/
--rw-r--r--   0 theo       (501) staff       (20)      775 2023-07-31 12:28:18.000000 bondzai.gateway-0.0.8/bondzai/gateway/__init__.py
--rw-r--r--   0 theo       (501) staff       (20)      843 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/config.yml
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:28:29.501467 bondzai.gateway-0.0.8/bondzai/gateway/core/
--rw-r--r--   0 theo       (501) staff       (20)     8525 2023-07-31 12:28:18.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/application.py
--rw-r--r--   0 theo       (501) staff       (20)      328 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/device.py
--rw-r--r--   0 theo       (501) staff       (20)      577 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/events.py
--rw-r--r--   0 theo       (501) staff       (20)      833 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/fsm.py
--rw-r--r--   0 theo       (501) staff       (20)     2127 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/logger.py
--rw-r--r--   0 theo       (501) staff       (20)     2590 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/manager.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:28:29.504448 bondzai.gateway-0.0.8/bondzai/gateway/core/message/
--rw-r--r--   0 theo       (501) staff       (20)     5391 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/message/base.py
--rw-r--r--   0 theo       (501) staff       (20)     4968 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/message/command.py
--rw-r--r--   0 theo       (501) staff       (20)     7572 2023-07-31 12:28:18.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/message/enums.py
--rw-r--r--   0 theo       (501) staff       (20)     7382 2023-07-31 12:28:18.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/message/event.py
--rw-r--r--   0 theo       (501) staff       (20)      337 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/message/payload.py
--rw-r--r--   0 theo       (501) staff       (20)     6821 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/message/process_dbm.py
--rw-r--r--   0 theo       (501) staff       (20)     9408 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/message/response.py
--rw-r--r--   0 theo       (501) staff       (20)      942 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/message/utils.py
--rw-r--r--   0 theo       (501) staff       (20)     2276 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/observer.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:28:29.505865 bondzai.gateway-0.0.8/bondzai/gateway/core/websocket/
--rw-r--r--   0 theo       (501) staff       (20)     1749 2023-07-31 12:28:18.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/websocket/client.py
--rw-r--r--   0 theo       (501) staff       (20)     2652 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/websocket/connector.py
--rw-r--r--   0 theo       (501) staff       (20)     2370 2023-07-31 12:28:18.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/websocket/request.py
--rw-r--r--   0 theo       (501) staff       (20)      171 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/websocket/utils.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:28:29.507171 bondzai.gateway-0.0.8/bondzai/gateway/device_connectors/
--rw-r--r--   0 theo       (501) staff       (20)      201 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/device_connectors/base.py
--rw-r--r--   0 theo       (501) staff       (20)     4426 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/device_connectors/serial.py
--rw-r--r--   0 theo       (501) staff       (20)     7630 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/device_connectors/socket_server.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:28:29.507844 bondzai.gateway-0.0.8/bondzai/gateway/tests/
--rw-r--r--   0 theo       (501) staff       (20)        0 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/tests/__init__.py
--rw-r--r--   0 theo       (501) staff       (20)     2280 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/tests/test_observer.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:28:29.510879 bondzai.gateway-0.0.8/bondzai.gateway.egg-info/
--rw-r--r--   0 theo       (501) staff       (20)      596 2023-07-31 12:28:29.000000 bondzai.gateway-0.0.8/bondzai.gateway.egg-info/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)     1382 2023-07-31 12:28:29.000000 bondzai.gateway-0.0.8/bondzai.gateway.egg-info/SOURCES.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-31 12:28:29.000000 bondzai.gateway-0.0.8/bondzai.gateway.egg-info/dependency_links.txt
--rw-r--r--   0 theo       (501) staff       (20)       57 2023-07-31 12:28:29.000000 bondzai.gateway-0.0.8/bondzai.gateway.egg-info/entry_points.txt
--rw-r--r--   0 theo       (501) staff       (20)        8 2023-07-31 12:28:29.000000 bondzai.gateway-0.0.8/bondzai.gateway.egg-info/namespace_packages.txt
--rw-r--r--   0 theo       (501) staff       (20)      117 2023-07-31 12:28:29.000000 bondzai.gateway-0.0.8/bondzai.gateway.egg-info/requires.txt
--rw-r--r--   0 theo       (501) staff       (20)       13 2023-07-31 12:28:29.000000 bondzai.gateway-0.0.8/bondzai.gateway.egg-info/top_level.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-31 12:28:29.000000 bondzai.gateway-0.0.8/bondzai.gateway.egg-info/zip-safe
--rw-r--r--   0 theo       (501) staff       (20)       71 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/pyproject.toml
--rw-r--r--   0 theo       (501) staff       (20)      913 2023-07-31 12:28:29.512547 bondzai.gateway-0.0.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 14:49:01.681867 bondzai.gateway-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)      547 2023-10-23 14:47:37.000000 bondzai.gateway-0.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)      596 2023-10-23 14:49:01.681867 bondzai.gateway-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      195 2023-10-23 14:47:37.000000 bondzai.gateway-0.0.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 14:49:01.681867 bondzai.gateway-0.0.9/bondzai/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 14:49:01.681867 bondzai.gateway-0.0.9/bondzai/gateway/
+-rw-r--r--   0 root         (0) root         (0)      775 2023-10-23 14:48:51.000000 bondzai.gateway-0.0.9/bondzai/gateway/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      843 2023-10-23 14:47:37.000000 bondzai.gateway-0.0.9/bondzai/gateway/config.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 14:49:01.681867 bondzai.gateway-0.0.9/bondzai/gateway/core/
+-rw-r--r--   0 root         (0) root         (0)     8668 2023-10-23 14:48:51.000000 bondzai.gateway-0.0.9/bondzai/gateway/core/application.py
+-rw-r--r--   0 root         (0) root         (0)     1327 2023-10-23 14:48:51.000000 bondzai.gateway-0.0.9/bondzai/gateway/core/device.py
+-rw-r--r--   0 root         (0) root         (0)      577 2023-10-23 14:47:37.000000 bondzai.gateway-0.0.9/bondzai/gateway/core/events.py
+-rw-r--r--   0 root         (0) root         (0)      833 2023-10-23 14:47:37.000000 bondzai.gateway-0.0.9/bondzai/gateway/core/fsm.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2023-10-23 14:47:37.000000 bondzai.gateway-0.0.9/bondzai/gateway/core/logger.py
+-rw-r--r--   0 root         (0) root         (0)     2590 2023-10-23 14:47:37.000000 bondzai.gateway-0.0.9/bondzai/gateway/core/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 14:49:01.681867 bondzai.gateway-0.0.9/bondzai/gateway/core/message/
+-rw-r--r--   0 root         (0) root         (0)     5695 2023-10-23 14:48:51.000000 bondzai.gateway-0.0.9/bondzai/gateway/core/message/base.py
+-rw-r--r--   0 root         (0) root         (0)     5104 2023-10-23 14:48:51.000000 bondzai.gateway-0.0.9/bondzai/gateway/core/message/command.py
+-rw-r--r--   0 root         (0) root         (0)     8966 2023-10-23 14:48:51.000000 bondzai.gateway-0.0.9/bondzai/gateway/core/message/enums.py
+-rw-r--r--   0 root         (0) root         (0)    11331 2023-10-23 14:48:51.000000 bondzai.gateway-0.0.9/bondzai/gateway/core/message/event.py
+-rw-r--r--   0 root         (0) root         (0)      337 2023-10-23 14:47:37.000000 bondzai.gateway-0.0.9/bondzai/gateway/core/message/payload.py
+-rw-r--r--   0 root         (0) root         (0)     6821 2023-10-23 14:47:37.000000 bondzai.gateway-0.0.9/bondzai/gateway/core/message/process_dbm.py
+-rw-r--r--   0 root         (0) root         (0)     9408 2023-10-23 14:47:37.000000 bondzai.gateway-0.0.9/bondzai/gateway/core/message/response.py
+-rw-r--r--   0 root         (0) root         (0)     3978 2023-10-23 14:48:51.000000 bondzai.gateway-0.0.9/bondzai/gateway/core/message/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2276 2023-10-23 14:47:37.000000 bondzai.gateway-0.0.9/bondzai/gateway/core/observer.py
+-rw-r--r--   0 root         (0) root         (0)     2583 2023-10-23 14:48:51.000000 bondzai.gateway-0.0.9/bondzai/gateway/core/packets_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 14:49:01.681867 bondzai.gateway-0.0.9/bondzai/gateway/core/websocket/
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-10-23 14:48:51.000000 bondzai.gateway-0.0.9/bondzai/gateway/core/websocket/client.py
+-rw-r--r--   0 root         (0) root         (0)     2652 2023-10-23 14:47:37.000000 bondzai.gateway-0.0.9/bondzai/gateway/core/websocket/connector.py
+-rw-r--r--   0 root         (0) root         (0)     2370 2023-10-23 14:47:37.000000 bondzai.gateway-0.0.9/bondzai/gateway/core/websocket/request.py
+-rw-r--r--   0 root         (0) root         (0)      171 2023-10-23 14:47:37.000000 bondzai.gateway-0.0.9/bondzai/gateway/core/websocket/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 14:49:01.681867 bondzai.gateway-0.0.9/bondzai/gateway/device_connectors/
+-rw-r--r--   0 root         (0) root         (0)      201 2023-10-23 14:47:37.000000 bondzai.gateway-0.0.9/bondzai/gateway/device_connectors/base.py
+-rw-r--r--   0 root         (0) root         (0)     3397 2023-10-23 14:48:51.000000 bondzai.gateway-0.0.9/bondzai/gateway/device_connectors/serial.py
+-rw-r--r--   0 root         (0) root         (0)     6795 2023-10-23 14:48:51.000000 bondzai.gateway-0.0.9/bondzai/gateway/device_connectors/socket_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 14:49:01.681867 bondzai.gateway-0.0.9/bondzai/gateway/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-23 14:47:37.000000 bondzai.gateway-0.0.9/bondzai/gateway/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2023-10-23 14:47:37.000000 bondzai.gateway-0.0.9/bondzai/gateway/tests/test_observer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 14:49:01.681867 bondzai.gateway-0.0.9/bondzai.gateway.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      596 2023-10-23 14:49:01.000000 bondzai.gateway-0.0.9/bondzai.gateway.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1424 2023-10-23 14:49:01.000000 bondzai.gateway-0.0.9/bondzai.gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-23 14:49:01.000000 bondzai.gateway-0.0.9/bondzai.gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-10-23 14:49:01.000000 bondzai.gateway-0.0.9/bondzai.gateway.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-10-23 14:49:01.000000 bondzai.gateway-0.0.9/bondzai.gateway.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)      117 2023-10-23 14:49:01.000000 bondzai.gateway-0.0.9/bondzai.gateway.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-10-23 14:49:01.000000 bondzai.gateway-0.0.9/bondzai.gateway.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-23 14:49:01.000000 bondzai.gateway-0.0.9/bondzai.gateway.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)       71 2023-10-23 14:47:37.000000 bondzai.gateway-0.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      913 2023-10-23 14:49:01.681867 bondzai.gateway-0.0.9/setup.cfg
```

### Comparing `bondzai.gateway-0.0.8/NOTICE` & `bondzai.gateway-0.0.9/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.8/PKG-INFO` & `bondzai.gateway-0.0.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.gateway
-Version: 0.0.8
+Version: 0.0.9
 Summary: Bondzai Gateway
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,gateway
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.gateway-0.0.8/bondzai/gateway/__init__.py` & `bondzai.gateway-0.0.9/bondzai/gateway/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import signal
 from pathlib import Path
 
 from .core.application import Application, CONFIG_DEFAULT_PATH
 
 
 CMD_NAME = "bondzai.gateway"
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 
 def run():
     parser = argparse.ArgumentParser(
         prog=CMD_NAME,
         description="Davinsy Gateway"
     )
```

### Comparing `bondzai.gateway-0.0.8/bondzai/gateway/config.yml` & `bondzai.gateway-0.0.9/bondzai/gateway/config.yml`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.8/bondzai/gateway/core/application.py` & `bondzai.gateway-0.0.9/bondzai/gateway/core/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,18 @@
             self.send_device_list_to_clients(client)
         elif request.action == ACT_TRANSFERS_TO_WS_CLIENTS:
             self.transfers_msg_to_clients(request.message, client.id)
         elif request.action == ACT_SEND_TO_DEVICE:
             device = Manager.GetDevice(request.device_name)
             if device:
                 msg = Message.from_json(request.message)
+
+                # Force the session id to be the one generated at handshake
+                msg.header.session = device.session.bytes
+
                 device.send(msg.to_msgpack())
 
     def send_device_list_to_clients(self, client: WebsocketClient = None) -> None:
         # if a client is specified, we send the list only to him, else to all clients
         clients = [client] if client is not None else Manager.GetClients()
         device_list = [d.name for d in Manager.GetDevices()]
         msg = ws_client_serialize({
@@ -179,15 +183,15 @@
     def on_device_disconnected(self, device: Device) -> None:
         log(f"Device disconnected {device.name}")
         Manager.UnregisterDevice(device)
         self.send_device_list_to_clients()
 
     # Callback for Device Event ON_MESSAGE
     def on_device_message(self, device: Device, msg: Message) -> None:
-        # TODO : Handle msg
+        # TODO : Handle msg       
         # TMP : For now send msg to every subscribed websocket clients
         log(f"Application On Device Message {device.name}")
         for client in Manager.GetDeviceEventSubs(device.name):
             log(f"Application Forward")
             client.send(ws_client_serialize({ 
                 "action": EVT_ON_DEVICE_MSG,
                 "device_name": device.name,
```

### Comparing `bondzai.gateway-0.0.8/bondzai/gateway/core/events.py` & `bondzai.gateway-0.0.9/bondzai/gateway/core/events.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.8/bondzai/gateway/core/fsm.py` & `bondzai.gateway-0.0.9/bondzai/gateway/core/fsm.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.8/bondzai/gateway/core/logger.py` & `bondzai.gateway-0.0.9/bondzai/gateway/core/logger.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.8/bondzai/gateway/core/manager.py` & `bondzai.gateway-0.0.9/bondzai/gateway/core/manager.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.8/bondzai/gateway/core/message/base.py` & `bondzai.gateway-0.0.9/bondzai/gateway/core/message/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,14 +33,19 @@
             "id": self.id,
             "op": self.op,
             "typ": self.typ,
             "mod": self.mod
         }
 
     def to_array(self) -> list:
+
+        #make sure session is 32 bytes, else pad
+        if len(self.session) < 32:
+            self.session = self.session + bytearray(32-len(self.session))
+
         return [
             self.session, 
             self.id, 
             self.op, 
             self.typ, 
             self.mod
         ]
@@ -165,7 +170,15 @@
         buffer = BytesIO()
         for i in range(len(raw_data)):
             data = raw_data[i]
             buffer.write(packer.pack(data))
         buffer.seek(0)
 
         return buffer.read()
+
+
+class Handshake(object):
+
+    def __init__(self, hid: int, agent_id: bytes) -> None:
+        self.hid = hid
+        self.agent_id = agent_id
+
```

### Comparing `bondzai.gateway-0.0.8/bondzai/gateway/core/message/command.py` & `bondzai.gateway-0.0.9/bondzai/gateway/core/message/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass
 
 from ..logger import log
 from .payload import MessagePayload
 from .enums import CommandOperationID, MessageModule, LogCommand, DBMCommand
-from .utils import B642B
+from .utils import B642B,B2B64
 
 
 @dataclass
 class CommandGet:
     itemid: int
     
     def to_dict(self) -> str:
@@ -116,15 +116,15 @@
         self.data = bytearray(data)
 
     def to_dict(self) -> str:
         return {
             "itemid": self.itemid,
             "table": self.table,
             "key": self.key,
-            "data": self.data,
+            "data": B2B64(self.data),
         }
 
     def to_array(self) -> list:
         return [
             self.itemid,
             self.table,
             self.key,
@@ -164,15 +164,18 @@
     if not mod in OP_TO_COMMAND_TYPES:
         return None
 
     if not op_id in OP_TO_COMMAND_TYPES[mod]:
         return None
 
     if op_id in (CommandOperationID.CMD_SET.value, CommandOperationID.CMD_START.value):
-        return OP_TO_COMMAND_TYPES[mod][op_id].get(raw_data["data"]["itemid"], None)
+        if isinstance(raw_data,list):
+            return OP_TO_COMMAND_TYPES[mod][op_id][raw_data[0]]
+        else:
+            return OP_TO_COMMAND_TYPES[mod][op_id].get(raw_data["data"]["itemid"], None)
 
     return OP_TO_COMMAND_TYPES[mod][op_id]
 
 
 class CommandMessagePayload(MessagePayload):
     @classmethod
     def from_array(cls, mod: int, operation: int, raw_data: list) -> "MessagePayload":
```

### Comparing `bondzai.gateway-0.0.8/bondzai/gateway/core/message/enums.py` & `bondzai.gateway-0.0.9/bondzai/gateway/core/message/enums.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,18 +14,26 @@
 class EventOperationID(Enum):
     EVT_EXT_EXCEPTION = 0x00
     EVT_EXT_DATA_IN = 0x01
     EVT_EXT_CMD_STATUS = 0x100
     EVT_EXT_LOG = 0x101
     EVT_EXT_VM_RESULT = 0x200
     EVT_EXT_ASL_RESULT = 0x201
+    EVT_EXT_DATA_TRANSFORM_RESULT = 0x202
+    EVT_EXT_DATA_ACQ_RESULT = 0x203
+    EVT_EXT_ENROLL_RESULT = 0x204
+    EVT_EXT_DATASET_PREPARATION_RESULT = 0x205
+    EVT_EXT_TRAINING_RESULT = 0x206
     EVT_EXT_PROCESS_ACK = 0x210
     EVT_EXT_SET_MODE = 0x300
     EVT_EXT_CORRECTION = 0x301
     EVT_EXT_TRIGGER = 0x302
+    EVT_EXT_SET_RECORD_MODE = 0x303
+    EVT_EXT_LAUNCH_TRAIN = 0x304
+    EVT_EXT_KILL = 0x305
     EVT_EXT_CUSTOM_1 = 0xF00
     EVT_EXT_CUSTOM_2 = 0xF01
     EVT_EXT_CUSTOM_3 = 0xF02
     EVT_EXT_CUSTOM_4 = 0xF03
     EVT_EXT_CUSTOM_5 = 0xF04
     EVT_EXT_CUSTOM_6 = 0xF05
     EVT_EXT_CUSTOM_7 = 0xF06
@@ -57,14 +65,15 @@
     EVT_INT_CUSTOM_4 = 0x1F03
     EVT_INT_YIELD_1 = 0x2000
     EVT_INT_YIELD_2 = 0x2001
     EVT_INT_YIELD_3 = 0x2002
     EVT_INT_YIELD_4 = 0x2003
     EVT_INT_FORCE_TRAIN = 0x3001
     EVT_INT_FORCE_DATA_IN = 0x3002
+    EVT_INT_TIMER = 0x4000
     EVT_TRANSIENT_MMS_LOAD = 0xF001
     EVT_TRANSIENT_RAM_LOAD = 0xF002
     EVT_TRANSIENT_FLASH_LOAD = 0xF003
     EVT_MAX = 0xFFFF
 
 
 class AgentAIMode(Enum):
@@ -105,14 +114,15 @@
     OPS_UID_HISTOGRAMF32 = 0x1000014
     OPS_UID_VECTORMATRIX_PRODUCTF32 = 0x1000015
     OPS_UID_FLATTENMATRIXF32 = 0x1000016
     OPS_UID_TRANSPOSEMATRIXF32 = 0x1000017
     OPS_UID_SLICEF32 = 0x1000018
     OPS_UID_SLICEMATRIXROWSF32 = 0x1000019
     OPS_UID_SLICEMATRIXCOLSF32 = 0x100001A
+    OPS_UID_ADD_VECTOR_BUFFERF32 = 0x1000030
     OPS_UID_FFT2048F32 = 0x2000011
     OPS_UID_FFT1024F32 = 0x2000012
     OPS_UID_FFT16F32 = 0x2000018
     OPS_UID_MFCC2048F32 = 0x2000019
     OPS_UID_MFCC1024F32 = 0x200001A
     OPS_UID_MEL2048F32 = 0x2000021
     OPS_UID_MEL1024F32 = 0x2000022
@@ -156,14 +166,27 @@
     DBM_TABLE_ADDRESS_VM = 0x1000
     DBM_TABLE_ADDRESS_LBL = 0x1001
     DBM_TABLE_ADDRESS_DAT = 0x1002
     DBM_TABLE_ADDRESS_KEY = 0x1003
     DBM_TABLE_ADDRESS_CTX = 0x1004
 
 
+class DBMAttributesVM(Enum):
+    DBM_ATT_VM_DESC = 0x00
+    DBM_ATT_VM_PREPROC_GRAPH_TRAIN = 0x01
+    DBM_ATT_VM_PREPROC_GRAPH_INFER = 0x02
+    DBM_ATT_VM_PREPROC_GRAPH_OTHER = 0x03
+    DBM_ATT_VM_DEEPLOMATH = 0x04
+    DBM_ATT_VM_POSTPROC = 0x05
+    DBM_ATT_VM_PREPROC_GRAPH_FEATURE_EXTRACTION = 0x06
+    DBM_ATT_VM_PREPROC_GRAPH_BACKGROUND_AUGMENTATION = 0x07
+    DBM_ATT_VM_PREPROC_GRAPH_DATA_AUGMENTATION = 0x08
+    DBM_ATT_VM_PREPROC_GRAPH_DATA_TRANSFORM = 0x09
+
+
 class LogCommand(Enum):
     LOG_GET_KPI = 0x1100
 
 
 class DBMCommand(Enum):
     DBM_EXPORT = 0x100
     DBM_EXPORT_ROW = 0x200
@@ -185,17 +208,31 @@
     DBM_CTX = 0x04
     DBM_SIG = 0x05
     DBM_GEN = 0x06
     DBM_TABLE_END = 0x07
 
 
 class AgentTriggerType(Enum):
-    TRIGGER_ON = 0
-    TRIGGER_OFF = 1
-    TRIGGER_KILL = 255
+    TRIGGER_ON = 16
+    TRIGGER_OFF = 17
+
+
+class AgentRecordMode(Enum):
+    DAVINSY_RECORD_OFF = 0
+    DAVINSY_RECORD_BACKGROUND = 1
+    DAVINSY_RECORD_SUBJECT = 2
+
+
+class AgentFlowSteps(Enum):
+    DATA_ACQUISITION = 1
+    DATA_TRANSFORM = 2
+    ENROLLEMENT = 3
+    INFERENCE = 4
+    DATASET_PREPARATION = 5
+    TRAINING = 6
 
 
 class MessageModule(Enum):
     BLD = 0x00
     COM = 0x01
     DBM = 0x02
     DLM = 0x03
@@ -236,19 +273,24 @@
     OP_PARAM_DCT = 0x90001104
     OP_PARAM_DCT_2D = 0x90001105
     OP_PARAM_HIST = 0x90001106
     OP_PARAM_NOISEMIX = 0x90001301
     OP_PARAM_PWSPAN = 0x90001302
     OP_PARAM_COMPRESS = 0x90001402
     OP_PARAM_MATRIX = 0x90001403
+    OP_PARAM_PRIVATE_TO_MATRIX = 0x90001410
+    OP_PARAM_PRIVATE_TO_VECTOR = 0x90001411
+    OP_PARAM_PRIVATE_TO_MATRIX_WITHBUFFERS = 0x90001412
+    OP_PARAM_PRIVATE_TO_VECTOR_WITHBUFFERS = 0x90001413
     OP_PARAM_EMPTY = 0x90008000
     OP_PARAM_MODE = 0x90008001
     OP_PARAM_REMOVENFIRST = 0x90008003
     OP_PARAM_SHAPE = 0x90008005
     OP_PARAM_SLICE = 0x90008006
+    OP_PARAM_WITHBUFFERS = 0x90008007
 
 
 class KPITypes(Enum):
     KPI_FREE = 0
     KPI_TRAINING_TIME_START = 1
     KPI_TRAINING_TIME_STOP = 2
     KPI_TRAINING_DATASET_SIZE = 3
@@ -272,14 +314,15 @@
     KPI_TRAINING_NET_LAYERS = 21
 
 
 class RUNCommandParameter(Enum):
     RUN_PARAM_BREAK = 0x0100
     RUN_PARAM_APPS = 0x0200
     RUN_PARAM_OPS = 0x0300
+    RUN_PARAM_EVQ_TIMEOUT = 0x0400
 
 
 class MALCommandParameter(Enum):
     MAL_PARAM_NB_THREADS = 0x0100
     MAL_PARAM_DATA_SOURCES = 0x0200
     MAL_PARAM_LIFE_CYCLE = 0x0300
     MAL_PARAM_NVM_FILE = 0x8100
@@ -287,9 +330,10 @@
     MAL_PARAM_MONITORING = 0x2000
 
 
 class BLDCommandParameter(Enum):
     BLD_PARAM_LINUX_LIB_NAMES = 0x8000
     BLD_PARAM_LINUX_PYTHON_SCRIPT_NAME = 0x8001
     BLD_PARAM_CORTEXM_INIT_DONE = 0x8002
+    BLD_PARAM_AG_ID = 0x8003
```

### Comparing `bondzai.gateway-0.0.8/bondzai/gateway/core/message/event.py` & `bondzai.gateway-0.0.9/bondzai/gateway/core/message/event.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 
 from ..logger import log
 from .payload import MessagePayload
-from .utils import B642B, unpack_buffer_to_list, B2B64
+from .utils import B642B, unpack_buffer_to_list, B2B64, get_step_struct
 from .enums import EventOperationID
 
 @dataclass
 class EventHeader:
     mod: int 
     appid: int 
     timestamp: int
@@ -132,18 +132,24 @@
 class EventInferResult:
     ai_type:int
     label_type: int
     step: int
     result: list
 
     def to_dict(self) -> str:
+        step_fields = get_step_struct(self.step)
+
         return {
             "ai_type": self.ai_type,
             "label_type": self.label_type,
-            "step": self.step,
+            "source_id": step_fields.get("source_id",0),
+            "process_id": step_fields.get("process_id",0),
+            "ai_mode": step_fields.get("ai_mode",0),
+            "record_mode": step_fields.get("record_mode",0),
+            "output": step_fields.get("output",0),
             "result": self.result
         }
 
     def to_array(self) -> list:
         return [
             self.ai_type,
             self.label_type,
@@ -172,31 +178,33 @@
             self.data
         ]
 
 
 @dataclass
 class EventCorrection:
     position: int
+    source_id: int
     ai_type: int
-    data: list
+    data: list  # classification.label_type & classification.label OR regression
 
     def to_dict(self) -> str:
         return {
             "position": self.position,
+            "source_id": self.source_id,
             "ai_type": self.ai_type,
-            "data":self.data
+            "data": self.data
         }
 
     def to_array(self) -> list:
         return [
             self.position,
+            self.source_id,
             self.ai_type,
             self.data
         ]
-    
 
 @dataclass
 class EventTrigger:
     trigger_type: int
     trigger_value: int
 
     def to_dict(self) -> str:
@@ -206,15 +214,49 @@
         }
     
     def to_array(self) -> list:
         return [
             self.trigger_type,
             self.trigger_value
         ]
+ 
+@dataclass
+class EventSetRecordMode:
+    record_mode: int
+    source_id: int
+
+    def to_dict(self) -> str:
+        return {
+            "record_mode": self.record_mode,
+            "source_id": self.source_id,
+        }
+    
+    def to_array(self) -> list:
+        return [
+            self.record_mode,
+            self.source_id
+        ]
+    
+@dataclass
+class EventLaunchTrain:
+
+    def to_dict(self) -> str:
+        return { }
+    
+    def to_array(self) -> list:
+        return [ ]
+
+@dataclass
+class EventKill:
+
+    def to_dict(self) -> str:
+        return { }
     
+    def to_array(self) -> list:
+        return [ ]
 
 @dataclass
 class EventCustom:
     data: bytearray
 
     def __init__(self, data) -> None:
         if(type(data) == str):
@@ -223,64 +265,149 @@
 
     def to_dict(self) -> str:
         return { "data": B2B64(self.data) }
 
     def to_array(self) -> list:
         return [ self.data ]
     
+
 @dataclass
 class EventProcessAck:
     evt_id: int
     process_state: int
     step: int
     app_id: int
     meta: bytes
 
     def to_dict(self) -> str:
+        step_fields = get_step_struct(self.step)
         return {
             "evt_id": self.evt_id,
             "process_state": self.process_state,
-            "step": self.step,
+            "source_id": step_fields.get("source_id",0),
+            "process_id": step_fields.get("process_id",0),
+            "ai_mode": step_fields.get("ai_mode",0),
+            "record_mode": step_fields.get("record_mode",0),
+            "output": step_fields.get("output",0),
             "app_id": self.app_id,
             "meta": self.meta
         }
 
     def to_array(self) -> list:
+
         return [
             self.evt_id,
             self.process_state,
             self.step,
             self.app_id,
             self.meta
         ]
 
+
+@dataclass
+class EventDataResult:
+    evt_id: int
+    process_state: int
+    step: int
+    app_id: int
+    datatype: str
+    result: bytes
+
+    def to_dict(self) -> str:
+        listofresult = [unpack_buffer_to_list(b, self.datatype[0] == "<", 4, self.datatype[1]) for b in self.result]
+        result = [item for onelist in listofresult for item in onelist]
+        step_fields = get_step_struct(self.step)
+
+        return {
+            "evt_id": self.evt_id,
+            "process_state": self.process_state,
+            "source_id": step_fields.get("source_id",0),
+            "process_id": step_fields.get("process_id",0),
+            "ai_mode": step_fields.get("ai_mode",0),
+            "record_mode": step_fields.get("record_mode",0),
+            "output": step_fields.get("output",0),
+            "app_id": self.app_id,
+            "datatype": self.datatype,
+            "result": result
+        }
+
+    def to_array(self) -> list:
+        return [
+            self.evt_id,
+            self.process_state,
+            self.step,
+            self.app_id,
+            self.datatype,
+            self.result
+        ]
+    
+
+@dataclass
+class EventTrainResult:
+    evt_id: int
+    process_state: int
+    step: int
+    app_id: int
+    nb_models: int
+
+    def to_dict(self) -> str:
+        step_fields = get_step_struct(self.step)
+
+        return {
+            "evt_id": self.evt_id,
+            "process_state": self.process_state,
+            "source_id": step_fields.get("source_id",0),
+            "process_id": step_fields.get("process_id",0),
+            "ai_mode": step_fields.get("ai_mode",0),
+            "record_mode": step_fields.get("record_mode",0),
+            "output": step_fields.get("output",0),
+            "app_id": self.app_id,
+            "nb_models": self.nb_models
+        }
+
+    def to_array(self) -> list:
+        return [
+            self.evt_id,
+            self.process_state,
+            self.step,
+            self.app_id,
+            self.nb_models
+        ]    
+
 OP_TO_EVENT_TYPES = {
     EventOperationID.EVT_EXT_EXCEPTION.value:     EventException,
     EventOperationID.EVT_EXT_DATA_IN.value:       EventDataIn,
     EventOperationID.EVT_EXT_CMD_STATUS.value:    EventCMDStatus,
     EventOperationID.EVT_EXT_LOG.value:           EventLog,
     EventOperationID.EVT_EXT_ASL_RESULT.value:    EventAslResult, 
     EventOperationID.EVT_EXT_VM_RESULT.value:     EventInferResult, 
     EventOperationID.EVT_EXT_SET_MODE.value:      EventSetMode,
     EventOperationID.EVT_EXT_CORRECTION.value:    EventCorrection,
     EventOperationID.EVT_EXT_TRIGGER.value:       EventTrigger,
+    EventOperationID.EVT_EXT_SET_RECORD_MODE.value: EventSetRecordMode,
+    EventOperationID.EVT_EXT_LAUNCH_TRAIN.value:  EventLaunchTrain,
+    EventOperationID.EVT_EXT_KILL.value:          EventKill,
     EventOperationID.EVT_EXT_CUSTOM_1.value:      EventCustom,
     EventOperationID.EVT_EXT_CUSTOM_2.value:      EventCustom,
     EventOperationID.EVT_EXT_CUSTOM_3.value:      EventCustom,
     EventOperationID.EVT_EXT_CUSTOM_4.value:      EventCustom,
     EventOperationID.EVT_EXT_CUSTOM_5.value:      EventCustom,
     EventOperationID.EVT_EXT_CUSTOM_6.value:      EventCustom,
     EventOperationID.EVT_EXT_CUSTOM_7.value:      EventCustom,
     EventOperationID.EVT_EXT_CUSTOM_8.value:      EventCustom,
     EventOperationID.EVT_EXT_CUSTOM_9.value:      EventCustom,
     EventOperationID.EVT_EXT_CUSTOM_10.value:     EventCustom,
-    EventOperationID.EVT_EXT_PROCESS_ACK.value:   EventProcessAck
+    EventOperationID.EVT_EXT_PROCESS_ACK.value:   EventProcessAck,
+    EventOperationID.EVT_EXT_DATA_TRANSFORM_RESULT.value:   EventDataResult,
+    EventOperationID.EVT_EXT_DATA_ACQ_RESULT.value:   EventDataResult,
+    EventOperationID.EVT_EXT_ENROLL_RESULT.value: EventDataResult,
+    EventOperationID.EVT_EXT_DATASET_PREPARATION_RESULT.value: EventTrainResult,
+    EventOperationID.EVT_EXT_TRAINING_RESULT.value: EventTrainResult
 }
 
-
 def GetEventClass(event_type_id: int):
     return OP_TO_EVENT_TYPES.get(event_type_id, None)
 
 class EventMessagePayload(MessagePayload):
     @classmethod
     def from_array(cls, operation: int, raw_data: list) -> "MessagePayload":
         EventClass = GetEventClass(operation)
```

### Comparing `bondzai.gateway-0.0.8/bondzai/gateway/core/message/process_dbm.py` & `bondzai.gateway-0.0.9/bondzai/gateway/core/message/process_dbm.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.8/bondzai/gateway/core/message/response.py` & `bondzai.gateway-0.0.9/bondzai/gateway/core/message/response.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.8/bondzai/gateway/core/observer.py` & `bondzai.gateway-0.0.9/bondzai/gateway/core/observer.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.8/bondzai/gateway/core/websocket/client.py` & `bondzai.gateway-0.0.9/bondzai/gateway/core/websocket/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,18 @@
         self.socket = socket
         self.id = uuid4()
 
     async def _do_send(self, msg: str) -> None:
         await self.socket.send(msg)
 
     def send(self, msg: str) -> None:
-        log(f"Sending message to client, msg = {msg}")
+        if len(msg) < 128:
+            log(f"Sending message to client, msg = {msg}")
+        else:
+            log(f"Sending message to client, msg = {msg[:64]} ... {msg[-64:]}")
 
         new_loop = False
         try:
             loop = asyncio.get_event_loop()
             if not loop.is_running():
                 # if the loop is not running we do as if there is none.
                 raise
```

### Comparing `bondzai.gateway-0.0.8/bondzai/gateway/core/websocket/connector.py` & `bondzai.gateway-0.0.9/bondzai/gateway/core/websocket/connector.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.8/bondzai/gateway/core/websocket/request.py` & `bondzai.gateway-0.0.9/bondzai/gateway/core/websocket/request.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.8/bondzai/gateway/device_connectors/serial.py` & `bondzai.gateway-0.0.9/bondzai/gateway/device_connectors/serial.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,25 @@
 import traceback
 from serial import Serial
 import threading
 
+from ..core.packets_handler import PacketsHandler
 from ..core.device import Device
 from ..core.observer import dispatcher
 from ..core.events import ApplicationEvents, DeviceEvents
 from ..core.logger import log
-from ..core.message.base import Message
+from ..core.message.base import Handshake, Message
 from .base import DeviceConnector
 
 
 DEFAULT_PORT = "COM3"
 MAX_PAYLOAD_SIZE = 4 * 1024
 
 
 
-class PacketsHandler(object):
-    """
-    This class is here to handle the packets (before handling the message)
-    It allows to check packet header and to collatione the packet if message is not
-    complete
-    """
-    def __init__(self):
-        self._buffer = bytearray([])
-        self._pid = -1
-         
-    def push(self, packet):
-        if not packet:
-            raise RuntimeError("Connection error, empty packet")
-
-        header = packet[:2]
-        payload = packet[2:]
-
-        #check version
-        version = ((header[0]>>4)&0xF)
-        issecure = (header[0]&8)
-        msgtyp = ((header[0]&6)>>1)
-        islast = (header[0]&1)
-        pid = header[1]
-
-        if (version != 1):
-            raise RuntimeError("Bad protocol version %d, only supporting version 1" % version)
-
-        if (msgtyp != 1):
-            raise RuntimeError("Bad msg type %d, only supporting application message (1)" % msgtyp)
-
-        if (self._pid != -1 and pid != self._pid):
-            raise RuntimeError("This version of proxy doesn't support interleaved messages")
-
-        self._pid = pid
-        self._buffer += payload
-
-        if not islast:
-            return None
-
-        self._pid = -1
-        message = self._buffer
-        self._buffer = bytearray([])
-
-
-        return Message.from_msgpack(message)
 
 
 class RecvStatus:
     def __init__(self, device):
         self.device = device
         self.expected = 0
         self.binary_data = []
@@ -89,15 +45,15 @@
 
 
     def close(self) -> None:
         log(f"Closing serial port")
         self._serial.close()
 
     def new_device(self) -> None:
-        device = Device(self._port)
+        device = Device()
         dispatcher.notify(DeviceEvents.CONNECTED, device)
         x = threading.Thread(target=self._device_sender, args=(device,),daemon=True)
         x.start()
 
         return device
 
     def read_device(self) -> Message:
@@ -140,16 +96,21 @@
 
         try:
             device = self.new_device()
             self._run = True
             while self._run:
                 msg = self.read_device()
                 if msg:
-                    log("Got message from device: %s" % msg.to_json())
-                    dispatcher.notify(DeviceEvents.ON_MESSAGE, device, msg)
+                    if type(msg) == Handshake:
+                        log("Got handshake from device: %s" % msg.to_json())
+                        device.set_name(msg.agent_id)
+
+                    if type(msg) == Message:
+                        log("Got message from device: %s" % msg.to_json())
+                        dispatcher.notify(DeviceEvents.ON_MESSAGE, device, msg)
 
 
         except KeyboardInterrupt:
             self._run = False
         finally:
             log("Closing case 3")
             traceback.print_exc()
```

### Comparing `bondzai.gateway-0.0.8/bondzai/gateway/device_connectors/socket_server.py` & `bondzai.gateway-0.0.9/bondzai/gateway/device_connectors/socket_server.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,26 @@
 import selectors
 import socket
 import traceback
 
+from ..core.packets_handler import PacketsHandler
 from ..core.device import Device
 from ..core.observer import dispatcher
 from ..core.events import ApplicationEvents, DeviceEvents
 from ..core.logger import log
-from ..core.message.base import Message
+from ..core.message.base import Handshake, Message
 from .base import DeviceConnector
 
 
 DEFAULT_HOST = "localhost"
 DEFAULT_PORT = 9588
 DEFAULT_HEADER_LEN = 4
 DEFAULT_MAX_MSG_LEN = 4096
 
 
-class PacketsHandler(object):
-    """
-    This class is here to handle the packets (before handling the message)
-    It allows to check packet header and to collatione the packet if message is not
-    complete
-    """
-    def __init__(self):
-        self._buffer = bytearray([])
-        self._pid = -1
-         
-    def push(self, packet):        
-        if not packet:
-            raise RuntimeError("Connection error, empty packet")
-
-        packet = bytearray(packet)
-        header = packet[:2]
-        payload = packet[2:]
-
-        #check version
-        version = ((header[0]>>4)&0xF)
-        issecure = (header[0]&8)
-        msgtyp = ((header[0]&6)>>1)
-        islast = (header[0]&1)
-        pid = header[1]
-
-        if (version != 1):
-            raise RuntimeError("Bad protocol version %d, only supporting version 1" % version)
-
-        if (msgtyp != 1):
-            raise RuntimeError("Bad msg type %d, only supporting application message (1)" % msgtyp)
-
-        if (self._pid != -1 and pid != self._pid):
-            raise RuntimeError("This version of proxy doesn't support interleaved messages")
-
-        self._pid = pid
-        self._buffer += payload
-
-        if not islast:
-            return None
-
-        self._pid = -1
-        message = self._buffer
-        self._buffer = bytearray([])
-
-        return Message.from_msgpack(message)
-
 
 class RecvStatus:
     def __init__(self, device):
         self.device = device
         self.expected = 0
         self.binary_data = []
 
@@ -104,24 +59,30 @@
         log(f"Socket Server Closing")
         self._socket.close()
         self._selector.close()
 
     def new_device(self, socket: socket.socket) -> None:
         conn, addr = socket.accept()  # Should be ready to read
 
-        device = Device(addr)
+        device = Device()
 
         conn.setblocking(False)
         events = selectors.EVENT_READ | selectors.EVENT_WRITE
         self._selector.register(conn, events, data=RecvStatus(device))
 
-        dispatcher.notify(DeviceEvents.CONNECTED, device)
+        # JDE: the connected event is sent only whe, the device is ready 
 
     def on_device_msg(self, device: Device, socket: socket.socket, msg: Message) -> None:
-        log(f"Socket Server Got message from {device.name}: {msg.to_json()}")
+
+        msg_str = msg.to_json()
+        if len(msg_str) > 128:
+            log(f"Socket Server Got message from {device.name}: {msg_str[:64]} ... {msg_str[-64:]}")
+        else:
+            log(f"Socket Server Got message from {device.name}: {msg_str}")
+
         dispatcher.notify(DeviceEvents.ON_MESSAGE, device, msg)
 
     def read_device(self, socket: socket.socket, status: RecvStatus) -> Message:
         log(f"Socket Server Got Msg")
 
         device = status.device
         if status.expected == 0:
@@ -155,26 +116,31 @@
                 raise err
            
             if len(status.binary_data) == 0:
                 raise RuntimeError("Socket was closed")
         
         status.expected = 0
 
-        return self._handler.push(status.binary_data.copy())
+        return self._handler.push(bytearray(status.binary_data.copy()))
 
     def handle_connection(self, key, mask) -> None:
         sock = key.fileobj
         status: RecvStatus = key.data
 
         try:
             if mask & selectors.EVENT_READ:
                 try:
                     msg = self.read_device(sock, status)
                     if msg:
-                        self.on_device_msg(status.device, sock, msg)
+                        if type(msg) == Handshake:
+                            log("Got handshake from device: %s" % msg.agent_id)
+                            status.device.set_name(msg.hid,msg.agent_id)
+
+                        if type(msg) == Message:
+                            self.on_device_msg(status.device, sock, msg)
                 except RuntimeError as e:
                     self._selector.unregister(sock)
                     log("Closing case 1.1 %s" % e)
                     sock.close()
                     dispatcher.notify(DeviceEvents.DISCONNECTED, status.device)
                 except ConnectionResetError as e:
                     log("Closing case 1.2 %s" % e)
```

### Comparing `bondzai.gateway-0.0.8/bondzai/gateway/tests/test_observer.py` & `bondzai.gateway-0.0.9/bondzai/gateway/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.8/bondzai.gateway.egg-info/PKG-INFO` & `bondzai.gateway-0.0.9/bondzai.gateway.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.gateway
-Version: 0.0.8
+Version: 0.0.9
 Summary: Bondzai Gateway
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,gateway
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.gateway-0.0.8/bondzai.gateway.egg-info/SOURCES.txt` & `bondzai.gateway-0.0.9/bondzai.gateway.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 ./bondzai/gateway/core/application.py
 ./bondzai/gateway/core/device.py
 ./bondzai/gateway/core/events.py
 ./bondzai/gateway/core/fsm.py
 ./bondzai/gateway/core/logger.py
 ./bondzai/gateway/core/manager.py
 ./bondzai/gateway/core/observer.py
+./bondzai/gateway/core/packets_handler.py
 ./bondzai/gateway/core/message/base.py
 ./bondzai/gateway/core/message/command.py
 ./bondzai/gateway/core/message/enums.py
 ./bondzai/gateway/core/message/event.py
 ./bondzai/gateway/core/message/payload.py
 ./bondzai/gateway/core/message/process_dbm.py
 ./bondzai/gateway/core/message/response.py
```

### Comparing `bondzai.gateway-0.0.8/setup.cfg` & `bondzai.gateway-0.0.9/setup.cfg`

 * *Files identical despite different names*

