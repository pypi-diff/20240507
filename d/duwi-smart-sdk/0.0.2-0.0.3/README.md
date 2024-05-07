# Comparing `tmp/duwi_smart_sdk-0.0.2.tar.gz` & `tmp/duwi_smart_sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duwi_smart_sdk-0.0.2.tar", last modified: Mon May  6 08:42:00 2024, max compression
+gzip compressed data, was "duwi_smart_sdk-0.0.3.tar", last modified: Tue May  7 01:14:33 2024, max compression
```

## Comparing `duwi_smart_sdk-0.0.2.tar` & `duwi_smart_sdk-0.0.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 08:42:00.645693 duwi_smart_sdk-0.0.2/
--rw-rw-rw-   0        0        0      543 2024-05-06 08:42:00.644716 duwi_smart_sdk-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       60 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 08:42:00.579125 duwi_smart_sdk-0.0.2/duwi_smart_sdk/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 08:42:00.608585 duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/__init__.py
--rw-rw-rw-   0        0        0     1361 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/control.py
--rw-rw-rw-   0        0        0     2597 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/discover.py
--rw-rw-rw-   0        0        0     2188 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/house.py
--rw-rw-rw-   0        0        0     1723 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/login.py
--rw-rw-rw-   0        0        0     1534 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/refresh_token.py
--rw-rw-rw-   0        0        0     4752 2024-05-06 08:41:25.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/ws.py
-drwxrwxrwx   0        0        0        0 2024-05-06 08:42:00.617373 duwi_smart_sdk-0.0.2/duwi_smart_sdk/const/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/const/__init__.py
--rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/const/const.py
--rw-rw-rw-   0        0        0      274 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/const/status.py
--rw-rw-rw-   0        0        0     1194 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/const/type_map.py
-drwxrwxrwx   0        0        0        0 2024-05-06 08:42:00.619326 duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 08:42:00.622256 duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/req/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/req/__init__.py
--rw-rw-rw-   0        0        0     1584 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/req/device_control.py
-drwxrwxrwx   0        0        0        0 2024-05-06 08:42:00.630068 duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/resp/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/resp/__init__.py
--rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/resp/auth.py
--rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/resp/control.py
--rw-rw-rw-   0        0        0     2767 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/resp/device.py
--rw-rw-rw-   0        0        0     1113 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/resp/house.py
-drwxrwxrwx   0        0        0        0 2024-05-06 08:42:00.637887 duwi_smart_sdk-0.0.2/duwi_smart_sdk/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/util/__init__.py
--rw-rw-rw-   0        0        0     1926 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/util/http.py
--rw-rw-rw-   0        0        0      906 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/util/sign.py
--rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/util/timestamp.py
-drwxrwxrwx   0        0        0        0 2024-05-06 08:42:00.592973 duwi_smart_sdk-0.0.2/duwi_smart_sdk.egg-info/
--rw-rw-rw-   0        0        0      543 2024-05-06 08:42:00.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1087 2024-05-06 08:42:00.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 08:42:00.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-06 08:42:00.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-06 08:42:00.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-06 08:42:00.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 08:42:00.645693 duwi_smart_sdk-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      908 2024-05-06 08:41:33.000000 duwi_smart_sdk-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 08:42:00.639833 duwi_smart_sdk-0.0.2/test/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 08:42:00.642763 duwi_smart_sdk-0.0.2/test/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/test/util/__init__.py
--rw-rw-rw-   0        0        0     1192 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/test/util/test_http.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:14:33.068988 duwi_smart_sdk-0.0.3/
+-rw-rw-rw-   0        0        0      628 2024-05-07 01:14:33.068988 duwi_smart_sdk-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      145 2024-05-07 01:14:28.000000 duwi_smart_sdk-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 01:14:33.026952 duwi_smart_sdk-0.0.3/duwi_smart_sdk/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:14:33.043570 duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/__init__.py
+-rw-rw-rw-   0        0        0     1361 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/control.py
+-rw-rw-rw-   0        0        0     2597 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/discover.py
+-rw-rw-rw-   0        0        0     2188 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/house.py
+-rw-rw-rw-   0        0        0     1723 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/login.py
+-rw-rw-rw-   0        0        0     1534 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/refresh_token.py
+-rw-rw-rw-   0        0        0     3917 2024-05-07 01:11:44.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/ws.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:14:33.048441 duwi_smart_sdk-0.0.3/duwi_smart_sdk/const/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/const/__init__.py
+-rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/const/const.py
+-rw-rw-rw-   0        0        0      279 2024-05-07 01:12:57.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/const/status.py
+-rw-rw-rw-   0        0        0     1194 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/const/type_map.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:14:33.049416 duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:14:33.052350 duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/req/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/req/__init__.py
+-rw-rw-rw-   0        0        0     1584 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/req/device_control.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:14:33.059217 duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/resp/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/resp/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/resp/auth.py
+-rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/resp/control.py
+-rw-rw-rw-   0        0        0     2767 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/resp/device.py
+-rw-rw-rw-   0        0        0     1113 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/resp/house.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:14:33.064099 duwi_smart_sdk-0.0.3/duwi_smart_sdk/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/util/__init__.py
+-rw-rw-rw-   0        0        0     1926 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/util/http.py
+-rw-rw-rw-   0        0        0      906 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/util/sign.py
+-rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/util/timestamp.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:14:33.033788 duwi_smart_sdk-0.0.3/duwi_smart_sdk.egg-info/
+-rw-rw-rw-   0        0        0      628 2024-05-07 01:14:32.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1087 2024-05-07 01:14:32.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 01:14:32.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-07 01:14:32.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-07 01:14:32.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-07 01:14:32.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 01:14:33.069958 duwi_smart_sdk-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      908 2024-05-07 01:13:21.000000 duwi_smart_sdk-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:14:33.065076 duwi_smart_sdk-0.0.3/test/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:14:33.067034 duwi_smart_sdk-0.0.3/test/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/test/util/__init__.py
+-rw-rw-rw-   0        0        0     1192 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/test/util/test_http.py
```

### Comparing `duwi_smart_sdk-0.0.2/PKG-INFO` & `duwi_smart_sdk-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smart_sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi
 Classifier: Development Status :: 3 - Alpha
@@ -14,8 +14,13 @@
 Description-Content-Type: text/markdown
 
 install sdk
 ```shell
 pip install duwi-smart-sdk
 ```
 
+Update existing dependencies
+```shell
+pip install --upgrade duwi-smart-sdk
+```
+
```

### Comparing `duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/control.py` & `duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/discover.py` & `duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/house.py` & `duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/login.py` & `duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/login.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/refresh_token.py` & `duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/refresh_token.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/ws.py` & `duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/ws.py`

 * *Files 18% similar despite different names*

```diff
@@ -106,23 +106,7 @@
                 _LOGGER.info(f"ws接受消息:{message}")
                 message = str.replace(message, "&excision&", "")
                 await self._on_callback(message)
             except Exception as e:
                 _LOGGER.error(f"ws接受消息出现异常:{e}")
                 _LOGGER.error(f"error message detail: \n{traceback.format_exc()}")
 
-            # try:
-            #     if message == "KEEPALIVE":
-            #         continue
-
-            #     _LOGGER.info(f"replace message is :{message}")
-            #     flag, device_no, domain, action, attrs = trans(self.hass, self._instance_id, message)
-            #     if not flag:
-            #         _LOGGER.warning(f"flag is not true {flag} reason is {domain}")
-            #         continue
-            #     await self.hass.services.async_call(domain, action, attrs)
-            # except Exception as e:
-            #     _LOGGER.error(f"ws accept error: {e}")
-            #     _LOGGER.error(f"error message detail: \n{traceback.format_exc()}")
-            # finally:
-            #     if device_no:
-            #         self.hass.data[DUWI_DOMAIN][self._instance_id]["LOCK"][device_no] = False
```

### Comparing `duwi_smart_sdk-0.0.2/duwi_smart_sdk/const/type_map.py` & `duwi_smart_sdk-0.0.3/duwi_smart_sdk/const/type_map.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/req/device_control.py` & `duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/req/device_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/resp/auth.py` & `duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/resp/auth.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/resp/device.py` & `duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/resp/device.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/resp/house.py` & `duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/resp/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.2/duwi_smart_sdk/util/http.py` & `duwi_smart_sdk-0.0.3/duwi_smart_sdk/util/http.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.2/duwi_smart_sdk/util/sign.py` & `duwi_smart_sdk-0.0.3/duwi_smart_sdk/util/sign.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.2/duwi_smart_sdk.egg-info/PKG-INFO` & `duwi_smart_sdk-0.0.3/duwi_smart_sdk.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi-smart-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi
 Classifier: Development Status :: 3 - Alpha
@@ -14,8 +14,13 @@
 Description-Content-Type: text/markdown
 
 install sdk
 ```shell
 pip install duwi-smart-sdk
 ```
 
+Update existing dependencies
+```shell
+pip install --upgrade duwi-smart-sdk
+```
+
```

### Comparing `duwi_smart_sdk-0.0.2/duwi_smart_sdk.egg-info/SOURCES.txt` & `duwi_smart_sdk-0.0.3/duwi_smart_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.2/setup.py` & `duwi_smart_sdk-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'sdk for duwi third platform'
 
 setup(
     name="duwi_smart_sdk",
     version=VERSION,
     author="ledger",
     author_email="ledgerbiggg@gmail.com",
```

### Comparing `duwi_smart_sdk-0.0.2/test/util/test_http.py` & `duwi_smart_sdk-0.0.3/test/util/test_http.py`

 * *Files identical despite different names*
