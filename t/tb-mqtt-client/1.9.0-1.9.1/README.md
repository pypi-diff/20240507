# Comparing `tmp/tb-mqtt-client-1.9.0.tar.gz` & `tmp/tb-mqtt-client-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tb-mqtt-client-1.9.0.tar", last modified: Thu Mar 21 09:41:50 2024, max compression
+gzip compressed data, was "tb-mqtt-client-1.9.1.tar", last modified: Tue May  7 07:54:12 2024, max compression
```

## Comparing `tb-mqtt-client-1.9.0.tar` & `tb-mqtt-client-1.9.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-21 09:41:50.917929 tb-mqtt-client-1.9.0/
--rw-r--r--   0 imbeacon   (501) staff       (20)      549 2024-02-06 08:47:51.000000 tb-mqtt-client-1.9.0/LICENSE
--rw-r--r--   0 imbeacon   (501) staff       (20)    11764 2024-03-21 09:41:50.917719 tb-mqtt-client-1.9.0/PKG-INFO
--rw-r--r--   0 imbeacon   (501) staff       (20)    11196 2024-02-06 08:44:17.000000 tb-mqtt-client-1.9.0/README.md
--rw-r--r--   0 imbeacon   (501) staff       (20)      608 2024-02-06 08:47:51.000000 tb-mqtt-client-1.9.0/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     3458 2024-02-06 08:47:51.000000 tb-mqtt-client-1.9.0/sdk_utils.py
--rw-r--r--   0 imbeacon   (501) staff       (20)       38 2024-03-21 09:41:50.917975 tb-mqtt-client-1.9.0/setup.cfg
--rw-r--r--   0 imbeacon   (501) staff       (20)     1438 2024-03-21 09:39:52.000000 tb-mqtt-client-1.9.0/setup.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    18630 2024-02-06 08:47:51.000000 tb-mqtt-client-1.9.0/tb_device_http.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    42396 2024-03-21 09:39:25.000000 tb-mqtt-client-1.9.0/tb_device_mqtt.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    11614 2024-03-21 07:53:27.000000 tb-mqtt-client-1.9.0/tb_gateway_mqtt.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-21 09:41:50.917516 tb-mqtt-client-1.9.0/tb_mqtt_client.egg-info/
--rw-r--r--   0 imbeacon   (501) staff       (20)    11764 2024-03-21 09:41:50.000000 tb-mqtt-client-1.9.0/tb_mqtt_client.egg-info/PKG-INFO
--rw-r--r--   0 imbeacon   (501) staff       (20)      304 2024-03-21 09:41:50.000000 tb-mqtt-client-1.9.0/tb_mqtt_client.egg-info/SOURCES.txt
--rw-r--r--   0 imbeacon   (501) staff       (20)        1 2024-03-21 09:41:50.000000 tb-mqtt-client-1.9.0/tb_mqtt_client.egg-info/dependency_links.txt
--rw-r--r--   0 imbeacon   (501) staff       (20)       55 2024-03-21 09:41:50.000000 tb-mqtt-client-1.9.0/tb_mqtt_client.egg-info/requires.txt
--rw-r--r--   0 imbeacon   (501) staff       (20)        1 2024-03-21 09:41:50.000000 tb-mqtt-client-1.9.0/tb_mqtt_client.egg-info/top_level.txt
--rw-r--r--   0 imbeacon   (501) staff       (20)     1704 2024-02-06 08:47:51.000000 tb-mqtt-client-1.9.0/utils.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-07 07:54:12.585042 tb-mqtt-client-1.9.1/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      549 2024-02-06 08:47:51.000000 tb-mqtt-client-1.9.1/LICENSE
+-rw-r--r--   0 imbeacon   (501) staff       (20)    11764 2024-05-07 07:54:12.584793 tb-mqtt-client-1.9.1/PKG-INFO
+-rw-r--r--   0 imbeacon   (501) staff       (20)    11196 2024-02-06 08:44:17.000000 tb-mqtt-client-1.9.1/README.md
+-rw-r--r--   0 imbeacon   (501) staff       (20)      608 2024-02-06 08:47:51.000000 tb-mqtt-client-1.9.1/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     3458 2024-02-06 08:47:51.000000 tb-mqtt-client-1.9.1/sdk_utils.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)       38 2024-05-07 07:54:12.585088 tb-mqtt-client-1.9.1/setup.cfg
+-rw-r--r--   0 imbeacon   (501) staff       (20)     1438 2024-05-07 07:52:58.000000 tb-mqtt-client-1.9.1/setup.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    18630 2024-02-06 08:47:51.000000 tb-mqtt-client-1.9.1/tb_device_http.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    42006 2024-05-07 07:52:40.000000 tb-mqtt-client-1.9.1/tb_device_mqtt.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    11614 2024-03-21 07:53:27.000000 tb-mqtt-client-1.9.1/tb_gateway_mqtt.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-07 07:54:12.584570 tb-mqtt-client-1.9.1/tb_mqtt_client.egg-info/
+-rw-r--r--   0 imbeacon   (501) staff       (20)    11764 2024-05-07 07:54:12.000000 tb-mqtt-client-1.9.1/tb_mqtt_client.egg-info/PKG-INFO
+-rw-r--r--   0 imbeacon   (501) staff       (20)      304 2024-05-07 07:54:12.000000 tb-mqtt-client-1.9.1/tb_mqtt_client.egg-info/SOURCES.txt
+-rw-r--r--   0 imbeacon   (501) staff       (20)        1 2024-05-07 07:54:12.000000 tb-mqtt-client-1.9.1/tb_mqtt_client.egg-info/dependency_links.txt
+-rw-r--r--   0 imbeacon   (501) staff       (20)       55 2024-05-07 07:54:12.000000 tb-mqtt-client-1.9.1/tb_mqtt_client.egg-info/requires.txt
+-rw-r--r--   0 imbeacon   (501) staff       (20)        1 2024-05-07 07:54:12.000000 tb-mqtt-client-1.9.1/tb_mqtt_client.egg-info/top_level.txt
+-rw-r--r--   0 imbeacon   (501) staff       (20)     1704 2024-02-06 08:47:51.000000 tb-mqtt-client-1.9.1/utils.py
```

### Comparing `tb-mqtt-client-1.9.0/LICENSE` & `tb-mqtt-client-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tb-mqtt-client-1.9.0/PKG-INFO` & `tb-mqtt-client-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tb-mqtt-client
-Version: 1.9.0
+Version: 1.9.1
 Summary: ThingsBoard python client SDK
 Home-page: https://github.com/thingsboard/thingsboard-python-client-sdk
-Download-URL: https://github.com/thingsboard/thingsboard-python-client-sdk/archive/1.9.0.tar.gz
+Download-URL: https://github.com/thingsboard/thingsboard-python-client-sdk/archive/1.9.1.tar.gz
 Author: ThingsBoard
 Author-email: info@thingsboard.io
 License: Apache Software License (Apache Software License 2.0)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tb-paho-mqtt-client>=1.6.3
```

### Comparing `tb-mqtt-client-1.9.0/README.md` & `tb-mqtt-client-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `tb-mqtt-client-1.9.0/__init__.py` & `tb-mqtt-client-1.9.1/__init__.py`

 * *Files identical despite different names*

### Comparing `tb-mqtt-client-1.9.0/sdk_utils.py` & `tb-mqtt-client-1.9.1/sdk_utils.py`

 * *Files identical despite different names*

### Comparing `tb-mqtt-client-1.9.0/setup.py` & `tb-mqtt-client-1.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from setuptools import setup
 
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md')) as f:
     long_description = f.read()
 
-VERSION = "1.9.0"
+VERSION = "1.9.1"
 
 setup(
     version=VERSION,
     name="tb-mqtt-client",
     author="ThingsBoard",
     author_email="info@thingsboard.io",
     license="Apache Software License (Apache Software License 2.0)",
```

### Comparing `tb-mqtt-client-1.9.0/tb_device_http.py` & `tb-mqtt-client-1.9.1/tb_device_http.py`

 * *Files identical despite different names*

### Comparing `tb-mqtt-client-1.9.0/tb_device_mqtt.py` & `tb-mqtt-client-1.9.1/tb_device_mqtt.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,15 +347,15 @@
         self.__responses = {}
         self.__sending_thread = Thread(target=self.__sending_thread_main, name="Sending thread", daemon=True)
         self.__sending_thread.start()
         self.__housekeeping_thread = Thread(target=self.__housekeeping_thread_main,
                                             name="Housekeeping thread",
                                             daemon=True)
         self.__housekeeping_thread.start()
-        self.__timeout_queue = queue.Queue()
+        self.__attrs_request_timeout = {}
         self.__timeout_thread = Thread(target=self.__timeout_check)
         self.__timeout_thread.daemon = True
         self.__timeout_thread.start()
         self._client.on_connect = self._on_connect
         # self._client.on_log = self._on_log
         self._client.on_publish = self._on_publish
         self._client.on_message = self._on_message
@@ -659,14 +659,15 @@
         """Set the callback that will be called when a server-side RPC is received."""
         self.__device_on_server_side_rpc_response = handler
 
     def __sending_thread_main(self):
         while not self.stopped:
             try:
                 if not self.is_connected():
+                    sleep(.1)
                     continue
                 if (not self.__rate_limit.check_limit_reached()
                         and (self.__rate_limit.get_minimal_limit() == 0
                              or self.__rate_limit.get_minimal_limit() > len(self._client._out_packet))):
                     if not self.__sending_queue.empty():
                         item = self.__sending_queue.get(False)
                         if item is not None:
@@ -677,14 +678,16 @@
                                     continue
                                 self.__responses[item['id']] = {"info": info, "timeout_ts": int(time()) + DEFAULT_TIMEOUT}
                                 self.__rate_limit.add_counter()
                             elif item["method"] == TBSendMethod.SUBSCRIBE:
                                 result = self._client.subscribe(item["topic"], qos=item["qos"])
                                 self.__responses[item['id']] = {"info": result, "timeout_ts": int(time()) + DEFAULT_TIMEOUT}
                                 self.__rate_limit.add_counter()
+                    else:
+                        sleep(.1)
                 else:
                     sleep(0.1)
             except Exception as e:
                 log.exception("Error during data sending:", exc_info=e)
                 sleep(1)
 
     def __housekeeping_thread_main(self):
@@ -839,54 +842,50 @@
         ts_in_millis = int(time() * 1000)
 
         attr_request_number = self._add_attr_request_callback(callback)
 
         info = self._publish_data(msg, ATTRIBUTES_TOPIC_REQUEST + str(attr_request_number), self.quality_of_service,
                                   high_priority=True)
 
-        self._add_timeout(attr_request_number, ts_in_millis + DEFAULT_TIMEOUT * 1000)
+        self._add_timeout(attr_request_number, ts_in_millis, timeout=20)
         return info
 
-    def _add_timeout(self, attr_request_number, timestamp):
-        self.__timeout_queue.put({"ts": timestamp, "attribute_request_id": attr_request_number})
+    def _add_timeout(self, attr_request_number, timestamp, timeout=DEFAULT_TIMEOUT):
+        timestamp += timeout
+        self.__attrs_request_timeout[attr_request_number] = int(timestamp)
 
     def _add_attr_request_callback(self, callback):
         with self._lock:
             self.__attr_request_number += 1
             self._attr_request_dict.update({self.__attr_request_number: callback})
             attr_request_number = self.__attr_request_number
         return attr_request_number
 
     def __timeout_check(self):
         while not self.stopped:
-            if not self.__timeout_queue.empty():
-                item = self.__timeout_queue.get_nowait()
-                if item is not None:
-                    while not self.stopped:
-                        current_ts_in_millis = int(time() * 1000)
-                        if current_ts_in_millis > item["ts"]:
-                            break
-                        sleep(0.2)
-
-                    with self._lock:
-                        callback = None
-                        if item.get("attribute_request_id"):
-                            if self._attr_request_dict.get(item["attribute_request_id"]):
-                                callback = self._attr_request_dict.pop(item["attribute_request_id"])
-                        elif item.get("rpc_request_id"):
-                            if self.__device_client_rpc_dict.get(item["rpc_request_id"]):
-                                callback = self.__device_client_rpc_dict.pop(item["rpc_request_id"])
-                    if callback is not None:
-                        if isinstance(callback, tuple):
-                            callback[0](None, TBTimeoutException("Timeout while waiting for a reply from ThingsBoard!"),
-                                        callback[1])
-                        else:
-                            callback(None, TBTimeoutException("Timeout while waiting for a reply from ThingsBoard!"))
-            else:
-                sleep(0.2)
+            current_ts_in_millis = int(time())
+            for (attr_request_number, ts) in tuple(self.__attrs_request_timeout.items()):
+                if current_ts_in_millis < ts:
+                    continue
+
+                with self._lock:
+                    callback = None
+                    if self._attr_request_dict.get(attr_request_number):
+                        callback = self._attr_request_dict.pop(attr_request_number)
+
+                if callback is not None:
+                    if isinstance(callback, tuple):
+                        callback[0](None, TBTimeoutException("Timeout while waiting for a reply from ThingsBoard!"),
+                                    callback[1])
+                    else:
+                        callback(None, TBTimeoutException("Timeout while waiting for a reply from ThingsBoard!"))
+
+                self.__attrs_request_timeout.pop(attr_request_number)
+
+            sleep(0.2)
 
     def claim(self, secret_key, duration=30000):
         """Claim the device in Thingsboard. The duration is in milliseconds."""
         claiming_request = {
             "secretKey": secret_key,
             "durationMs": duration
         }
```

### Comparing `tb-mqtt-client-1.9.0/tb_gateway_mqtt.py` & `tb-mqtt-client-1.9.1/tb_gateway_mqtt.py`

 * *Files identical despite different names*

### Comparing `tb-mqtt-client-1.9.0/tb_mqtt_client.egg-info/PKG-INFO` & `tb-mqtt-client-1.9.1/tb_mqtt_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tb-mqtt-client
-Version: 1.9.0
+Version: 1.9.1
 Summary: ThingsBoard python client SDK
 Home-page: https://github.com/thingsboard/thingsboard-python-client-sdk
-Download-URL: https://github.com/thingsboard/thingsboard-python-client-sdk/archive/1.9.0.tar.gz
+Download-URL: https://github.com/thingsboard/thingsboard-python-client-sdk/archive/1.9.1.tar.gz
 Author: ThingsBoard
 Author-email: info@thingsboard.io
 License: Apache Software License (Apache Software License 2.0)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tb-paho-mqtt-client>=1.6.3
```

### Comparing `tb-mqtt-client-1.9.0/utils.py` & `tb-mqtt-client-1.9.1/utils.py`

 * *Files identical despite different names*

