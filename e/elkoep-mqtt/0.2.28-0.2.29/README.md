# Comparing `tmp/elkoep-mqtt-0.2.28.tar.gz` & `tmp/elkoep_mqtt-0.2.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elkoep-mqtt-0.2.28.tar", last modified: Fri Apr 12 13:45:26 2024, max compression
+gzip compressed data, was "elkoep_mqtt-0.2.29.tar", last modified: Tue May  7 14:28:07 2024, max compression
```

## Comparing `elkoep-mqtt-0.2.28.tar` & `elkoep_mqtt-0.2.29.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:45:26.798256 elkoep-mqtt-0.2.28/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-12 13:45:26.798256 elkoep-mqtt-0.2.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:45:26.798256 elkoep-mqtt-0.2.28/elkoep_mqtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-12 13:45:26.000000 elkoep-mqtt-0.2.28/elkoep_mqtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-12 13:45:26.000000 elkoep-mqtt-0.2.28/elkoep_mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:45:26.000000 elkoep-mqtt-0.2.28/elkoep_mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:45:26.000000 elkoep-mqtt-0.2.28/elkoep_mqtt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 13:45:26.000000 elkoep-mqtt-0.2.28/elkoep_mqtt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:45:26.794256 elkoep-mqtt-0.2.28/inelsmqtt/
--rw-r--r--   0 runner    (1001) docker     (127)    18091 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/inelsmqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/inelsmqtt/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    22709 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/inelsmqtt/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:45:26.794256 elkoep-mqtt-0.2.28/inelsmqtt/devices/
--rw-r--r--   0 runner    (1001) docker     (127)    10905 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/inelsmqtt/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/inelsmqtt/devices/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/inelsmqtt/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/inelsmqtt/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (127)   105922 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/inelsmqtt/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-12 13:45:26.798256 elkoep-mqtt-0.2.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:45:26.798256 elkoep-mqtt-0.2.28/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/tests/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:45:26.798256 elkoep-mqtt-0.2.28/tests/devices/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/tests/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16688 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/tests/devices/device_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/tests/discovery_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/tests/inels_mqtt_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/tests/online_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:07.728944 elkoep_mqtt-0.2.29/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-07 14:28:07.728944 elkoep_mqtt-0.2.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:07.728944 elkoep_mqtt-0.2.29/elkoep_mqtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-07 14:28:07.000000 elkoep_mqtt-0.2.29/elkoep_mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-07 14:28:07.000000 elkoep_mqtt-0.2.29/elkoep_mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:28:07.000000 elkoep_mqtt-0.2.29/elkoep_mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:28:07.000000 elkoep_mqtt-0.2.29/elkoep_mqtt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 14:28:07.000000 elkoep_mqtt-0.2.29/elkoep_mqtt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:07.728944 elkoep_mqtt-0.2.29/inelsmqtt/
+-rw-r--r--   0 runner    (1001) docker     (127)    18542 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/inelsmqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/inelsmqtt/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22709 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/inelsmqtt/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:07.728944 elkoep_mqtt-0.2.29/inelsmqtt/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)    10905 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/inelsmqtt/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/inelsmqtt/devices/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/inelsmqtt/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/inelsmqtt/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105922 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/inelsmqtt/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-07 14:28:07.728944 elkoep_mqtt-0.2.29/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:07.728944 elkoep_mqtt-0.2.29/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/tests/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:07.728944 elkoep_mqtt-0.2.29/tests/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/tests/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16688 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/tests/devices/device_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/tests/discovery_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/tests/inels_mqtt_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/tests/online_test.py
```

### Comparing `elkoep-mqtt-0.2.28/LICENSE` & `elkoep_mqtt-0.2.29/LICENSE`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.28/PKG-INFO` & `elkoep_mqtt-0.2.29/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elkoep-mqtt
-Version: 0.2.28
+Version: 0.2.29
 Summary: Python library for iNELS mqtt protocol
 Home-page: https://github.com/epdevlab/elkoep-mqtt
 Author: Elko EP s.r.o.
 Author-email: epdevlab@gmail.com
 License: MIT
 Keywords: iNels,Elko EP,Home assistant integration
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `elkoep-mqtt-0.2.28/README.md` & `elkoep_mqtt-0.2.29/README.md`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.28/elkoep_mqtt.egg-info/PKG-INFO` & `elkoep_mqtt-0.2.29/elkoep_mqtt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elkoep-mqtt
-Version: 0.2.28
+Version: 0.2.29
 Summary: Python library for iNELS mqtt protocol
 Home-page: https://github.com/epdevlab/elkoep-mqtt
 Author: Elko EP s.r.o.
 Author-email: epdevlab@gmail.com
 License: MIT
 Keywords: iNels,Elko EP,Home assistant integration
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `elkoep-mqtt-0.2.28/elkoep_mqtt.egg-info/SOURCES.txt` & `elkoep_mqtt-0.2.29/elkoep_mqtt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.28/inelsmqtt/__init__.py` & `elkoep_mqtt-0.2.29/inelsmqtt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,28 +160,28 @@
         """Test connection. It's used only for connection
             testing. After that is disconnected
         Returns:
             bool: Is broker available or not
         """
         try:
             self.__connect()
-            self.disconnect()            
+            self.disconnect()
         except Exception as e:
             if isinstance(e, ConnectionRefusedError):
                 self.__connection_error = 3 # cannot connect
             else:
                 self.__connection_error = 6 # unknown
-        
+
         return self.__connection_error
 
     def subscribe_listener(self, topic: str, unique_id: str, fnc: Callable[[Any], Any]) -> None:
         """Append new item into the datachange listener."""
         #if topic not in self.__listeners:
         #    self.__listeners[topic] = dict[str, Callable[[Any], Any]]()
-        
+
         stripped_topic = "/".join(topic.split("/")[2:])
         self.__listeners[stripped_topic][unique_id] = fnc
 
     def unsubscribe_listeners(self) -> bool:
         """Unsubscribe listeners."""
         self.__listeners.clear()
 
@@ -240,15 +240,15 @@
         self.__try_connect = True
         if reason_code == mqtt.CONNACK_ACCEPTED:
             self.__is_available = True
             self.__connection_error = None
         else:
             self.__is_available = False
             self.__connection_error = reason_code
-        
+
         _LOGGER.info(
             "Mqtt broker %s:%s %s",
             self.__host,
             self.__port,
             "is connected" if self.__is_available else "is not connected",
         )
 
@@ -395,15 +395,15 @@
         client: mqtt.Client,  # pylint: disable=unused-argument
         userdata,  # pylint: disable=unused-argument
         msg,
     ) -> None:
         """Special callback function used only in discover_all function
         placed in on_message. It is the same as on_message callback func,
         but does different things
-        
+
         Args:
             client (MqttClient): Mqtt broker instance
             msg (object): Topic with payload from broker
         """
         _LOGGER.info("Found device from topic %s\n", msg.topic)
 
         # pass only those who belong to known device types
@@ -430,15 +430,15 @@
             if device_type == "gw" and action == "connected":
                 if msg.topic not in self.__is_subscribed_list:
                     client.subscribe(msg.topic, 0, None, None)
                     self.__messages[msg.topic] = msg.payload
                     self.__last_values[msg.topic] = copy.copy(msg.topic)
                     self.__is_subscribed_list[msg.topic] = True
                     _LOGGER.info("Device of type %s found [gw].\n", device_type)
-            
+
     def __on_message(
         self,
         client: mqtt.Client,  # pylint: disable=unused-argument
         userdata,  # pylint: disable=unused-argument
         msg,
     ) -> None:
         """Callback function which is used for subscription
@@ -459,23 +459,34 @@
             self.__last_values[msg.topic] = (
                 copy.copy(self.__messages[msg.topic])
                 if msg.topic in self.__messages
                 else msg.payload
             )
             self.__messages[msg.topic] = msg.payload
 
+        if  device_type == "gw" and message_type == "connected":
+            mac = message_parts[2]
+            for stripped_topic in self.__listeners:
+                if stripped_topic.startswith(mac):
+                    self.__notify_listeners(stripped_topic, True)
+            return
+
         stripped_topic = "/".join(message_parts[2:])
 
         is_connected_message = message_type == "connected"
 
         if len(self.__listeners) > 0 and stripped_topic in self.__listeners:
             # This pass data change directely into the device.
-            if len(self.__listeners[stripped_topic]) > 0:
-                for unique_id in list(self.__listeners[stripped_topic]): #prevents the dictionary increased in size during iteration exception
-                    self.__listeners[stripped_topic][unique_id](is_connected_message)
+            self.__notify_listeners(stripped_topic, is_connected_message)
+
+    def __notify_listeners(self, stripped_topic: str, is_connected_message: bool) -> None:
+        """Notify listeners for a specific topic."""
+        if len(self.__listeners[stripped_topic]) > 0:
+            for unique_id in list(self.__listeners[stripped_topic]): #prevents the dictionary increased in size during iteration exception
+                self.__listeners[stripped_topic][unique_id](is_connected_message)
 
     def __on_subscribe(
         self,
         client: mqtt.Client,  # pylint: disable=unused-argument
         userdata,  # pylint: disable=unused-argument
         mid,  # pylint: disable=unused-argument
         granted_qos,  # pylint: disable=unused-argument
```

### Comparing `elkoep-mqtt-0.2.28/inelsmqtt/config.py` & `elkoep_mqtt-0.2.29/inelsmqtt/config.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.28/inelsmqtt/const.py` & `elkoep_mqtt-0.2.29/inelsmqtt/const.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.28/inelsmqtt/devices/__init__.py` & `elkoep_mqtt-0.2.29/inelsmqtt/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.28/inelsmqtt/devices/switch.py` & `elkoep_mqtt-0.2.29/inelsmqtt/devices/switch.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.28/inelsmqtt/discovery.py` & `elkoep_mqtt-0.2.29/inelsmqtt/discovery.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.28/inelsmqtt/mqtt_client.py` & `elkoep_mqtt-0.2.29/inelsmqtt/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.28/inelsmqtt/util.py` & `elkoep_mqtt-0.2.29/inelsmqtt/util.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.28/setup.py` & `elkoep_mqtt-0.2.29/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Setup script for elkoep-mqtt package."""
 from setuptools import setup, find_packages
 
 setup(
     name="elkoep-mqtt",
-    version="0.2.28",
+    version="0.2.29",
     url="https://github.com/epdevlab/elkoep-mqtt",
     license="MIT",
     author="Elko EP s.r.o.",
     author_email="epdevlab@gmail.com",
     description="Python library for iNELS mqtt protocol",
     keywords=["iNels", "Elko EP", "Home assistant integration"],
     long_description_content_type="text/markdown",
```

### Comparing `elkoep-mqtt-0.2.28/tests/const.py` & `elkoep_mqtt-0.2.29/tests/const.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.28/tests/devices/device_test.py` & `elkoep_mqtt-0.2.29/tests/devices/device_test.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.28/tests/discovery_test.py` & `elkoep_mqtt-0.2.29/tests/discovery_test.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.28/tests/inels_mqtt_test.py` & `elkoep_mqtt-0.2.29/tests/inels_mqtt_test.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.28/tests/online_test.py` & `elkoep_mqtt-0.2.29/tests/online_test.py`

 * *Files identical despite different names*

