# Comparing `tmp/yolink-api-0.4.3.tar.gz` & `tmp/yolink-api-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yolink-api-0.4.3.tar", last modified: Tue Apr  9 03:45:27 2024, max compression
+gzip compressed data, was "yolink-api-0.4.4.tar", last modified: Tue May  7 03:04:26 2024, max compression
```

## Comparing `yolink-api-0.4.3.tar` & `yolink-api-0.4.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:45:27.437464 yolink-api-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-09 03:45:22.000000 yolink-api-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-09 03:45:27.437464 yolink-api-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-09 03:45:22.000000 yolink-api-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-09 03:45:22.000000 yolink-api-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 03:45:27.437464 yolink-api-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-09 03:45:22.000000 yolink-api-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:45:27.437464 yolink-api-0.4.3/yolink/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/auth_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/client_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/device.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/home_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/message_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/message_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/outlet_request_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/thermostat_request_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/unit_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:45:27.437464 yolink-api-0.4.3/yolink_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-09 03:45:27.000000 yolink-api-0.4.3/yolink_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-09 03:45:27.000000 yolink-api-0.4.3/yolink_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 03:45:27.000000 yolink-api-0.4.3/yolink_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 03:45:27.000000 yolink-api-0.4.3/yolink_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 03:45:27.000000 yolink-api-0.4.3/yolink_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 03:45:27.000000 yolink-api-0.4.3/yolink_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:04:26.574784 yolink-api-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-07 03:04:24.000000 yolink-api-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-07 03:04:26.574784 yolink-api-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-07 03:04:24.000000 yolink-api-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-07 03:04:24.000000 yolink-api-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 03:04:26.574784 yolink-api-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-07 03:04:24.000000 yolink-api-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:04:26.570784 yolink-api-0.4.4/yolink/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:04:24.000000 yolink-api-0.4.4/yolink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-07 03:04:24.000000 yolink-api-0.4.4/yolink/auth_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-07 03:04:24.000000 yolink-api-0.4.4/yolink/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-07 03:04:24.000000 yolink-api-0.4.4/yolink/client_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-07 03:04:24.000000 yolink-api-0.4.4/yolink/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-07 03:04:24.000000 yolink-api-0.4.4/yolink/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-07 03:04:24.000000 yolink-api-0.4.4/yolink/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-07 03:04:24.000000 yolink-api-0.4.4/yolink/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-05-07 03:04:24.000000 yolink-api-0.4.4/yolink/home_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-07 03:04:24.000000 yolink-api-0.4.4/yolink/message_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-07 03:04:24.000000 yolink-api-0.4.4/yolink/message_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-07 03:04:24.000000 yolink-api-0.4.4/yolink/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-05-07 03:04:24.000000 yolink-api-0.4.4/yolink/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-07 03:04:24.000000 yolink-api-0.4.4/yolink/outlet_request_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-07 03:04:24.000000 yolink-api-0.4.4/yolink/thermostat_request_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-07 03:04:24.000000 yolink-api-0.4.4/yolink/unit_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:04:26.570784 yolink-api-0.4.4/yolink_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-07 03:04:26.000000 yolink-api-0.4.4/yolink_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-07 03:04:26.000000 yolink-api-0.4.4/yolink_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 03:04:26.000000 yolink-api-0.4.4/yolink_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 03:04:26.000000 yolink-api-0.4.4/yolink_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 03:04:26.000000 yolink-api-0.4.4/yolink_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 03:04:26.000000 yolink-api-0.4.4/yolink_api.egg-info/top_level.txt
```

### Comparing `yolink-api-0.4.3/LICENSE` & `yolink-api-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.3/PKG-INFO` & `yolink-api-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolink-api
-Version: 0.4.3
+Version: 0.4.4
 Summary: A library to authenticate with yolink device
 Home-page: https://github.com/YoSmart-Inc/yolink-api
 Author: YoSmart
 License: MIT
 Project-URL: Bug Tracker, https://github.com/YoSmart-Inc/yolink-api/issues
 Keywords: yolink api
 Platform: UNKNOWN
```

### Comparing `yolink-api-0.4.3/README.md` & `yolink-api-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.3/setup.py` & `yolink-api-0.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="yolink-api",
-    version="0.4.3",
+    version="0.4.4",
     author="YoSmart",
     description="A library to authenticate with yolink device",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/YoSmart-Inc/yolink-api",
     project_urls={
         "Bug Tracker": "https://github.com/YoSmart-Inc/yolink-api/issues",
```

### Comparing `yolink-api-0.4.3/yolink/auth_mgr.py` & `yolink-api-0.4.4/yolink/auth_mgr.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.3/yolink/client.py` & `yolink-api-0.4.4/yolink/client.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.3/yolink/const.py` & `yolink-api-0.4.4/yolink/const.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.3/yolink/device.py` & `yolink-api-0.4.4/yolink/device.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.3/yolink/endpoint.py` & `yolink-api-0.4.4/yolink/endpoint.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.3/yolink/exception.py` & `yolink-api-0.4.4/yolink/exception.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.3/yolink/home_manager.py` & `yolink-api-0.4.4/yolink/home_manager.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.3/yolink/message_resolver.py` & `yolink-api-0.4.4/yolink/message_resolver.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.3/yolink/model.py` & `yolink-api-0.4.4/yolink/model.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.3/yolink/mqtt_client.py` & `yolink-api-0.4.4/yolink/mqtt_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -114,15 +114,21 @@
             try:
                 device_id = keys[2]
                 msg_data = BRDP.parse_raw(msg.payload.decode("UTF-8"))
                 if msg_data.event is None:
                     return
                 msg_event = msg_data.event.split(".")
                 msg_type = msg_event[len(msg_event) - 1]
-                if msg_type not in ["Report", "Alert", "StatusChange", "getState"]:
+                if msg_type not in [
+                    "Report",
+                    "Alert",
+                    "StatusChange",
+                    "getState",
+                    "setState",
+                ]:
                     return
                 device = self._home_devices.get(device_id)
                 if device is None:
                     return
                 paired_device_id = device.get_paired_device_id()
                 if paired_device_id is not None:
                     paired_device = self._home_devices.get(paired_device_id)
```

### Comparing `yolink-api-0.4.3/yolink/outlet_request_builder.py` & `yolink-api-0.4.4/yolink/outlet_request_builder.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.3/yolink/thermostat_request_builder.py` & `yolink-api-0.4.4/yolink/thermostat_request_builder.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.3/yolink/unit_helper.py` & `yolink-api-0.4.4/yolink/unit_helper.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.3/yolink_api.egg-info/PKG-INFO` & `yolink-api-0.4.4/yolink_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolink-api
-Version: 0.4.3
+Version: 0.4.4
 Summary: A library to authenticate with yolink device
 Home-page: https://github.com/YoSmart-Inc/yolink-api
 Author: YoSmart
 License: MIT
 Project-URL: Bug Tracker, https://github.com/YoSmart-Inc/yolink-api/issues
 Keywords: yolink api
 Platform: UNKNOWN
```

### Comparing `yolink-api-0.4.3/yolink_api.egg-info/SOURCES.txt` & `yolink-api-0.4.4/yolink_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

