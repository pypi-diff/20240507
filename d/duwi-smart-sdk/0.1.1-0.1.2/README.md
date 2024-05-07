# Comparing `tmp/duwi_smart_sdk-0.1.1.tar.gz` & `tmp/duwi_smart_sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duwi_smart_sdk-0.1.1.tar", last modified: Tue May  7 07:06:30 2024, max compression
+gzip compressed data, was "duwi_smart_sdk-0.1.2.tar", last modified: Tue May  7 07:20:14 2024, max compression
```

## Comparing `duwi_smart_sdk-0.1.1.tar` & `duwi_smart_sdk-0.1.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 07:06:30.169222 duwi_smart_sdk-0.1.1/
--rw-rw-rw-   0        0        0      649 2024-05-07 07:06:30.169222 duwi_smart_sdk-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      147 2024-05-07 06:42:21.000000 duwi_smart_sdk-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 07:06:30.112766 duwi_smart_sdk-0.1.1/duwi_smart_sdk/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 07:06:30.128345 duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/__init__.py
--rw-rw-rw-   0        0        0     2095 2024-05-07 06:43:46.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/account.py
--rw-rw-rw-   0        0        0     2784 2024-05-07 06:21:35.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/control.py
--rw-rw-rw-   0        0        0     4309 2024-05-07 06:25:47.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/discover.py
--rw-rw-rw-   0        0        0     2695 2024-05-07 06:09:49.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/house.py
--rw-rw-rw-   0        0        0     2153 2024-05-07 06:09:49.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/refresh_token.py
--rw-rw-rw-   0        0        0     4717 2024-05-07 07:06:01.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/ws.py
-drwxrwxrwx   0        0        0        0 2024-05-07 07:06:30.134406 duwi_smart_sdk-0.1.1/duwi_smart_sdk/const/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/const/__init__.py
--rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/const/const.py
--rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/const/status.py
--rw-rw-rw-   0        0        0     1154 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/const/type_map.py
-drwxrwxrwx   0        0        0        0 2024-05-07 07:06:30.135813 duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 07:06:30.138403 duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/req/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/req/__init__.py
--rw-rw-rw-   0        0        0     1584 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/req/device_control.py
-drwxrwxrwx   0        0        0        0 2024-05-07 07:06:30.146280 duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/resp/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/resp/__init__.py
--rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/resp/auth.py
--rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/resp/control.py
--rw-rw-rw-   0        0        0     2767 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/resp/device.py
--rw-rw-rw-   0        0        0     1113 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/resp/house.py
-drwxrwxrwx   0        0        0        0 2024-05-07 07:06:30.152763 duwi_smart_sdk-0.1.1/duwi_smart_sdk/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/util/__init__.py
--rw-rw-rw-   0        0        0     1926 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/util/http.py
--rw-rw-rw-   0        0        0      906 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/util/sign.py
--rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/util/timestamp.py
-drwxrwxrwx   0        0        0        0 2024-05-07 07:06:30.118630 duwi_smart_sdk-0.1.1/duwi_smart_sdk.egg-info/
--rw-rw-rw-   0        0        0      649 2024-05-07 07:06:30.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1227 2024-05-07 07:06:30.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 07:06:30.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-07 07:06:30.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-07 07:06:30.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-07 07:06:30.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 07:06:30.170199 duwi_smart_sdk-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      938 2024-05-07 07:06:23.000000 duwi_smart_sdk-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 07:06:30.153739 duwi_smart_sdk-0.1.1/test/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 07:06:30.164257 duwi_smart_sdk-0.1.1/test/api/
--rw-rw-rw-   0        0        0        0 2024-05-07 06:10:48.000000 duwi_smart_sdk-0.1.1/test/api/__init__.py
--rw-rw-rw-   0        0        0      949 2024-05-07 06:21:35.000000 duwi_smart_sdk-0.1.1/test/api/test_control.py
--rw-rw-rw-   0        0        0      812 2024-05-07 06:26:29.000000 duwi_smart_sdk-0.1.1/test/api/test_discover.py
--rw-rw-rw-   0        0        0      687 2024-05-07 06:29:35.000000 duwi_smart_sdk-0.1.1/test/api/test_house.py
--rw-rw-rw-   0        0        0      640 2024-05-07 06:43:46.000000 duwi_smart_sdk-0.1.1/test/api/test_login.py
--rw-rw-rw-   0        0        0      894 2024-05-07 06:41:28.000000 duwi_smart_sdk-0.1.1/test/api/test_ws.py
-drwxrwxrwx   0        0        0        0 2024-05-07 07:06:30.167220 duwi_smart_sdk-0.1.1/test/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/test/util/__init__.py
--rw-rw-rw-   0        0        0     1222 2024-05-07 06:12:53.000000 duwi_smart_sdk-0.1.1/test/util/test_http.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:20:14.123560 duwi_smart_sdk-0.1.2/
+-rw-rw-rw-   0        0        0      649 2024-05-07 07:20:14.123560 duwi_smart_sdk-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2024-05-07 06:42:21.000000 duwi_smart_sdk-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 07:20:14.082497 duwi_smart_sdk-0.1.2/duwi_smart_sdk/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:20:14.096200 duwi_smart_sdk-0.1.2/duwi_smart_sdk/api/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk/api/__init__.py
+-rw-rw-rw-   0        0        0     2095 2024-05-07 06:43:46.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk/api/account.py
+-rw-rw-rw-   0        0        0     2784 2024-05-07 06:21:35.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk/api/control.py
+-rw-rw-rw-   0        0        0     4309 2024-05-07 06:25:47.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk/api/discover.py
+-rw-rw-rw-   0        0        0     2695 2024-05-07 06:09:49.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk/api/house.py
+-rw-rw-rw-   0        0        0     2153 2024-05-07 06:09:49.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk/api/refresh_token.py
+-rw-rw-rw-   0        0        0     4791 2024-05-07 07:19:48.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk/api/ws.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:20:14.101082 duwi_smart_sdk-0.1.2/duwi_smart_sdk/const/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk/const/__init__.py
+-rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk/const/const.py
+-rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk/const/status.py
+-rw-rw-rw-   0        0        0     1154 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk/const/type_map.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:20:14.102059 duwi_smart_sdk-0.1.2/duwi_smart_sdk/model/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:20:14.104011 duwi_smart_sdk-0.1.2/duwi_smart_sdk/model/req/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk/model/req/__init__.py
+-rw-rw-rw-   0        0        0     1584 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk/model/req/device_control.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:20:14.108895 duwi_smart_sdk-0.1.2/duwi_smart_sdk/model/resp/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk/model/resp/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk/model/resp/auth.py
+-rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk/model/resp/control.py
+-rw-rw-rw-   0        0        0     2767 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk/model/resp/device.py
+-rw-rw-rw-   0        0        0     1113 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk/model/resp/house.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:20:14.112800 duwi_smart_sdk-0.1.2/duwi_smart_sdk/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk/util/__init__.py
+-rw-rw-rw-   0        0        0     1926 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk/util/http.py
+-rw-rw-rw-   0        0        0      906 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk/util/sign.py
+-rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk/util/timestamp.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:20:14.089364 duwi_smart_sdk-0.1.2/duwi_smart_sdk.egg-info/
+-rw-rw-rw-   0        0        0      649 2024-05-07 07:20:13.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1227 2024-05-07 07:20:14.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 07:20:14.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-07 07:20:14.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-07 07:20:14.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-07 07:20:14.000000 duwi_smart_sdk-0.1.2/duwi_smart_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 07:20:14.123560 duwi_smart_sdk-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      936 2024-05-07 07:19:55.000000 duwi_smart_sdk-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:20:14.113776 duwi_smart_sdk-0.1.2/test/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.2/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:20:14.120612 duwi_smart_sdk-0.1.2/test/api/
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:10:48.000000 duwi_smart_sdk-0.1.2/test/api/__init__.py
+-rw-rw-rw-   0        0        0      949 2024-05-07 06:21:35.000000 duwi_smart_sdk-0.1.2/test/api/test_control.py
+-rw-rw-rw-   0        0        0      812 2024-05-07 06:26:29.000000 duwi_smart_sdk-0.1.2/test/api/test_discover.py
+-rw-rw-rw-   0        0        0      687 2024-05-07 06:29:35.000000 duwi_smart_sdk-0.1.2/test/api/test_house.py
+-rw-rw-rw-   0        0        0      640 2024-05-07 06:43:46.000000 duwi_smart_sdk-0.1.2/test/api/test_login.py
+-rw-rw-rw-   0        0        0     1020 2024-05-07 07:13:14.000000 duwi_smart_sdk-0.1.2/test/api/test_ws.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:20:14.122565 duwi_smart_sdk-0.1.2/test/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.2/test/util/__init__.py
+-rw-rw-rw-   0        0        0     1222 2024-05-07 06:12:53.000000 duwi_smart_sdk-0.1.2/test/util/test_http.py
```

### Comparing `duwi_smart_sdk-0.1.1/PKG-INFO` & `duwi_smart_sdk-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smart_sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/account.py` & `duwi_smart_sdk-0.1.2/duwi_smart_sdk/api/account.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/control.py` & `duwi_smart_sdk-0.1.2/duwi_smart_sdk/api/control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/discover.py` & `duwi_smart_sdk-0.1.2/duwi_smart_sdk/api/discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/house.py` & `duwi_smart_sdk-0.1.2/duwi_smart_sdk/api/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/refresh_token.py` & `duwi_smart_sdk-0.1.2/duwi_smart_sdk/api/refresh_token.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/ws.py` & `duwi_smart_sdk-0.1.2/duwi_smart_sdk/api/ws.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,31 +35,31 @@
         self._house_no = house_no
         self._app_version = app_version
         self._client_version = client_version
         self._client_model = client_model
         self._is_over = False
         self._connection = None
 
-    async def close(self):
-        self._is_over = True
-        if self._connection:
-            await self._connection.close()
 
     async def connect(self):
+        _LOGGER.info('connect ws server...')
         self._connection = await websockets.connect(self._server_uri)
 
     async def send(self, message):
         if self._connection:
+            _LOGGER.info('send message: %s', message)
             await self._connection.send(message)
 
     async def disconnect(self):
         if self._connection:
+            _LOGGER.info('disconnect ws server...')
             await self._connection.close()
 
     async def reconnect(self):
+        _LOGGER.info('reconnect ws server...')
         if self._is_over:
             return
         await self.connect()
         await self.link()
         await self.bind()
 
     async def listen(self):
@@ -129,12 +129,12 @@
                 await self.reconnect()
 
     async def process_messages(self):
         async for message in self._connection:
             try:
                 if message == "KEEPALIVE":
                     continue
-                _LOGGER.info(f"ws接受消息:{message}")
+                _LOGGER.info(f"ws receive message:{message}")
                 message = str.replace(message, "&excision&", "")
                 await self._on_callback(message)
             except Exception as e:
                 _LOGGER.error(f"error message detail: \n{traceback.format_exc()}")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `duwi_smart_sdk-0.1.1/duwi_smart_sdk/const/status.py` & `duwi_smart_sdk-0.1.2/duwi_smart_sdk/const/status.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.1/duwi_smart_sdk/const/type_map.py` & `duwi_smart_sdk-0.1.2/duwi_smart_sdk/const/type_map.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/req/device_control.py` & `duwi_smart_sdk-0.1.2/duwi_smart_sdk/model/req/device_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/resp/auth.py` & `duwi_smart_sdk-0.1.2/duwi_smart_sdk/model/resp/auth.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/resp/device.py` & `duwi_smart_sdk-0.1.2/duwi_smart_sdk/model/resp/device.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/resp/house.py` & `duwi_smart_sdk-0.1.2/duwi_smart_sdk/model/resp/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.1/duwi_smart_sdk/util/http.py` & `duwi_smart_sdk-0.1.2/duwi_smart_sdk/util/http.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.1/duwi_smart_sdk/util/sign.py` & `duwi_smart_sdk-0.1.2/duwi_smart_sdk/util/sign.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.1/duwi_smart_sdk.egg-info/PKG-INFO` & `duwi_smart_sdk-0.1.2/duwi_smart_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi-smart-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smart_sdk-0.1.1/duwi_smart_sdk.egg-info/SOURCES.txt` & `duwi_smart_sdk-0.1.2/duwi_smart_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.1/setup.py` & `duwi_smart_sdk-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.001'
+VERSION = '0.1.2'
 DESCRIPTION = 'sdk for duwi third platform'
 
 setup(
     name="duwi_smart_sdk",
     version=VERSION,
     author="ledger",
     author_email="ledgerbiggg@gmail.com",
```

### Comparing `duwi_smart_sdk-0.1.1/test/api/test_control.py` & `duwi_smart_sdk-0.1.2/test/api/test_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.1/test/api/test_discover.py` & `duwi_smart_sdk-0.1.2/test/api/test_discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.1/test/api/test_house.py` & `duwi_smart_sdk-0.1.2/test/api/test_house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.1/test/api/test_login.py` & `duwi_smart_sdk-0.1.2/test/api/test_login.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.1/test/api/test_ws.py` & `duwi_smart_sdk-0.1.2/test/api/test_ws.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,17 @@
             ws = DeviceSynchronizationWS(
                 on_callback=on_callback,
                 app_key="2e479831-1fb7-751e-7017-7534f7f99fc1",
                 app_secret="26af4883a943083a4c34083897fcea10",
                 access_token="715d1c63-85c0-4d74-9a89-5a0aa4806f74",
                 refresh_token="c539ec1b-99d9-44f2-8bb0-b942545c0aca",
                 house_no="c7bf567d-225a-4533-ab72-5dc080b794f5",
+                app_version="0.0.1",
+                client_version="0.0.1",
+                client_model="homeassistant",
             )
 
             await ws.reconnect()
             await ws.listen()
             await ws.keep_alive()
 
         asyncio.run(run_test())
```

### Comparing `duwi_smart_sdk-0.1.1/test/util/test_http.py` & `duwi_smart_sdk-0.1.2/test/util/test_http.py`

 * *Files identical despite different names*

