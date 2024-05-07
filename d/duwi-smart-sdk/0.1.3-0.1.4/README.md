# Comparing `tmp/duwi_smart_sdk-0.1.3.tar.gz` & `tmp/duwi_smart_sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duwi_smart_sdk-0.1.3.tar", last modified: Tue May  7 07:26:41 2024, max compression
+gzip compressed data, was "duwi_smart_sdk-0.1.4.tar", last modified: Tue May  7 07:32:50 2024, max compression
```

## Comparing `duwi_smart_sdk-0.1.3.tar` & `duwi_smart_sdk-0.1.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 07:26:41.336931 duwi_smart_sdk-0.1.3/
--rw-rw-rw-   0        0        0      649 2024-05-07 07:26:41.335954 duwi_smart_sdk-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      147 2024-05-07 06:42:21.000000 duwi_smart_sdk-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 07:26:41.274553 duwi_smart_sdk-0.1.3/duwi_smart_sdk/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 07:26:41.292130 duwi_smart_sdk-0.1.3/duwi_smart_sdk/api/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk/api/__init__.py
--rw-rw-rw-   0        0        0     2095 2024-05-07 06:43:46.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk/api/account.py
--rw-rw-rw-   0        0        0     2784 2024-05-07 06:21:35.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk/api/control.py
--rw-rw-rw-   0        0        0     4309 2024-05-07 06:25:47.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk/api/discover.py
--rw-rw-rw-   0        0        0     2695 2024-05-07 06:09:49.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk/api/house.py
--rw-rw-rw-   0        0        0     2153 2024-05-07 06:09:49.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk/api/refresh_token.py
--rw-rw-rw-   0        0        0     4809 2024-05-07 07:25:43.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk/api/ws.py
-drwxrwxrwx   0        0        0        0 2024-05-07 07:26:41.297012 duwi_smart_sdk-0.1.3/duwi_smart_sdk/const/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk/const/__init__.py
--rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk/const/const.py
--rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk/const/status.py
--rw-rw-rw-   0        0        0     1154 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk/const/type_map.py
-drwxrwxrwx   0        0        0        0 2024-05-07 07:26:41.297989 duwi_smart_sdk-0.1.3/duwi_smart_sdk/model/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 07:26:41.300922 duwi_smart_sdk-0.1.3/duwi_smart_sdk/model/req/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk/model/req/__init__.py
--rw-rw-rw-   0        0        0     1584 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk/model/req/device_control.py
-drwxrwxrwx   0        0        0        0 2024-05-07 07:26:41.308920 duwi_smart_sdk-0.1.3/duwi_smart_sdk/model/resp/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk/model/resp/__init__.py
--rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk/model/resp/auth.py
--rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk/model/resp/control.py
--rw-rw-rw-   0        0        0     2767 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk/model/resp/device.py
--rw-rw-rw-   0        0        0     1113 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk/model/resp/house.py
-drwxrwxrwx   0        0        0        0 2024-05-07 07:26:41.317021 duwi_smart_sdk-0.1.3/duwi_smart_sdk/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk/util/__init__.py
--rw-rw-rw-   0        0        0     1926 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk/util/http.py
--rw-rw-rw-   0        0        0      906 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk/util/sign.py
--rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk/util/timestamp.py
-drwxrwxrwx   0        0        0        0 2024-05-07 07:26:41.282365 duwi_smart_sdk-0.1.3/duwi_smart_sdk.egg-info/
--rw-rw-rw-   0        0        0      649 2024-05-07 07:26:41.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1227 2024-05-07 07:26:41.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 07:26:41.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-07 07:26:41.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-07 07:26:41.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-07 07:26:41.000000 duwi_smart_sdk-0.1.3/duwi_smart_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 07:26:41.336931 duwi_smart_sdk-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      936 2024-05-07 07:26:05.000000 duwi_smart_sdk-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 07:26:41.318973 duwi_smart_sdk-0.1.3/test/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.3/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 07:26:41.330603 duwi_smart_sdk-0.1.3/test/api/
--rw-rw-rw-   0        0        0        0 2024-05-07 06:10:48.000000 duwi_smart_sdk-0.1.3/test/api/__init__.py
--rw-rw-rw-   0        0        0      949 2024-05-07 06:21:35.000000 duwi_smart_sdk-0.1.3/test/api/test_control.py
--rw-rw-rw-   0        0        0      812 2024-05-07 06:26:29.000000 duwi_smart_sdk-0.1.3/test/api/test_discover.py
--rw-rw-rw-   0        0        0      687 2024-05-07 06:29:35.000000 duwi_smart_sdk-0.1.3/test/api/test_house.py
--rw-rw-rw-   0        0        0      640 2024-05-07 06:43:46.000000 duwi_smart_sdk-0.1.3/test/api/test_login.py
--rw-rw-rw-   0        0        0     1020 2024-05-07 07:13:14.000000 duwi_smart_sdk-0.1.3/test/api/test_ws.py
-drwxrwxrwx   0        0        0        0 2024-05-07 07:26:41.334470 duwi_smart_sdk-0.1.3/test/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.3/test/util/__init__.py
--rw-rw-rw-   0        0        0     1222 2024-05-07 06:12:53.000000 duwi_smart_sdk-0.1.3/test/util/test_http.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:32:50.122394 duwi_smart_sdk-0.1.4/
+-rw-rw-rw-   0        0        0      649 2024-05-07 07:32:50.122394 duwi_smart_sdk-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2024-05-07 06:42:21.000000 duwi_smart_sdk-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 07:32:50.080750 duwi_smart_sdk-0.1.4/duwi_smart_sdk/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:32:50.095013 duwi_smart_sdk-0.1.4/duwi_smart_sdk/api/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk/api/__init__.py
+-rw-rw-rw-   0        0        0     2095 2024-05-07 06:43:46.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk/api/account.py
+-rw-rw-rw-   0        0        0     2784 2024-05-07 06:21:35.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk/api/control.py
+-rw-rw-rw-   0        0        0     4309 2024-05-07 06:25:47.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk/api/discover.py
+-rw-rw-rw-   0        0        0     2695 2024-05-07 06:09:49.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk/api/house.py
+-rw-rw-rw-   0        0        0     2153 2024-05-07 06:09:49.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk/api/refresh_token.py
+-rw-rw-rw-   0        0        0     4788 2024-05-07 07:31:40.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk/api/ws.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:32:50.098921 duwi_smart_sdk-0.1.4/duwi_smart_sdk/const/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk/const/__init__.py
+-rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk/const/const.py
+-rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk/const/status.py
+-rw-rw-rw-   0        0        0     1154 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk/const/type_map.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:32:50.100875 duwi_smart_sdk-0.1.4/duwi_smart_sdk/model/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:32:50.102822 duwi_smart_sdk-0.1.4/duwi_smart_sdk/model/req/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk/model/req/__init__.py
+-rw-rw-rw-   0        0        0     1584 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk/model/req/device_control.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:32:50.107755 duwi_smart_sdk-0.1.4/duwi_smart_sdk/model/resp/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk/model/resp/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk/model/resp/auth.py
+-rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk/model/resp/control.py
+-rw-rw-rw-   0        0        0     2767 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk/model/resp/device.py
+-rw-rw-rw-   0        0        0     1113 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk/model/resp/house.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:32:50.111614 duwi_smart_sdk-0.1.4/duwi_smart_sdk/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk/util/__init__.py
+-rw-rw-rw-   0        0        0     1926 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk/util/http.py
+-rw-rw-rw-   0        0        0      906 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk/util/sign.py
+-rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk/util/timestamp.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:32:50.087587 duwi_smart_sdk-0.1.4/duwi_smart_sdk.egg-info/
+-rw-rw-rw-   0        0        0      649 2024-05-07 07:32:49.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1227 2024-05-07 07:32:50.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 07:32:49.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-07 07:32:49.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-07 07:32:49.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-07 07:32:49.000000 duwi_smart_sdk-0.1.4/duwi_smart_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 07:32:50.123380 duwi_smart_sdk-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      936 2024-05-07 07:32:26.000000 duwi_smart_sdk-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:32:50.112590 duwi_smart_sdk-0.1.4/test/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.4/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:32:50.118453 duwi_smart_sdk-0.1.4/test/api/
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:10:48.000000 duwi_smart_sdk-0.1.4/test/api/__init__.py
+-rw-rw-rw-   0        0        0      949 2024-05-07 06:21:35.000000 duwi_smart_sdk-0.1.4/test/api/test_control.py
+-rw-rw-rw-   0        0        0      812 2024-05-07 06:26:29.000000 duwi_smart_sdk-0.1.4/test/api/test_discover.py
+-rw-rw-rw-   0        0        0      687 2024-05-07 06:29:35.000000 duwi_smart_sdk-0.1.4/test/api/test_house.py
+-rw-rw-rw-   0        0        0      640 2024-05-07 06:43:46.000000 duwi_smart_sdk-0.1.4/test/api/test_login.py
+-rw-rw-rw-   0        0        0     1020 2024-05-07 07:13:14.000000 duwi_smart_sdk-0.1.4/test/api/test_ws.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:32:50.121385 duwi_smart_sdk-0.1.4/test/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.4/test/util/__init__.py
+-rw-rw-rw-   0        0        0     1222 2024-05-07 06:12:53.000000 duwi_smart_sdk-0.1.4/test/util/test_http.py
```

### Comparing `duwi_smart_sdk-0.1.3/PKG-INFO` & `duwi_smart_sdk-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smart_sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smart_sdk-0.1.3/duwi_smart_sdk/api/account.py` & `duwi_smart_sdk-0.1.4/duwi_smart_sdk/api/account.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.3/duwi_smart_sdk/api/control.py` & `duwi_smart_sdk-0.1.4/duwi_smart_sdk/api/control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.3/duwi_smart_sdk/api/discover.py` & `duwi_smart_sdk-0.1.4/duwi_smart_sdk/api/discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.3/duwi_smart_sdk/api/house.py` & `duwi_smart_sdk-0.1.4/duwi_smart_sdk/api/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.3/duwi_smart_sdk/api/refresh_token.py` & `duwi_smart_sdk-0.1.4/duwi_smart_sdk/api/refresh_token.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.3/duwi_smart_sdk/api/ws.py` & `duwi_smart_sdk-0.1.4/duwi_smart_sdk/api/ws.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,43 +37,43 @@
         self._client_version = client_version
         self._client_model = client_model
         self._is_over = False
         self._connection = None
 
 
     async def connect(self):
-        _LOGGER.warning('connect ws server...')
+        _LOGGER.info('connect ws server...')
         self._connection = await websockets.connect(self._server_uri)
 
     async def send(self, message):
         if self._connection:
-            _LOGGER.warning('send message: %s', message)
+            _LOGGER.info('send message: %s', message)
             await self._connection.send(message)
 
     async def disconnect(self):
         if self._connection:
-            _LOGGER.warning('disconnect ws server...')
+            _LOGGER.info('disconnect ws server...')
             await self._connection.close()
 
     async def reconnect(self):
-        _LOGGER.warning('reconnect ws server...')
+        _LOGGER.info('reconnect ws server...')
         if self._is_over:
             return
         await self.connect()
         await self.link()
         await self.bind()
 
     async def listen(self):
         while True:
             try:
                 if self._is_over:
                     return
                 await self.process_messages()
             except websockets.exceptions.ConnectionClosedError:
-                _LOGGER.warning('listen ws connection closed, trying to reconnect...')
+                _LOGGER.info('listen ws connection closed, trying to reconnect...')
                 await self.reconnect()
                 await asyncio.sleep(5)
 
     async def link(self):
         timestamp = current_timestamp()
         client_id = md5_encrypt(timestamp)
 
@@ -121,20 +121,20 @@
         while True:
             try:
                 if self._is_over:
                     return
                 await self.send('KEEPALIVE')
                 await asyncio.sleep(20)
             except websockets.exceptions.ConnectionClosedError:
-                _LOGGER.warning('keep_alive ws,connection closed, trying to reconnect...')
+                _LOGGER.info('keep_alive ws,connection closed, trying to reconnect...')
                 await self.reconnect()
 
     async def process_messages(self):
         async for message in self._connection:
             try:
                 if message == "KEEPALIVE":
                     continue
-                _LOGGER.warning(f"ws receive message:{message}")
+                _LOGGER.info(f"ws receive message:{message}")
                 message = str.replace(message, "&excision&", "")
                 await self._on_callback(message)
             except Exception as e:
                 _LOGGER.error(f"error message detail: \n{traceback.format_exc()}")
```

### Comparing `duwi_smart_sdk-0.1.3/duwi_smart_sdk/const/status.py` & `duwi_smart_sdk-0.1.4/duwi_smart_sdk/const/status.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.3/duwi_smart_sdk/const/type_map.py` & `duwi_smart_sdk-0.1.4/duwi_smart_sdk/const/type_map.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.3/duwi_smart_sdk/model/req/device_control.py` & `duwi_smart_sdk-0.1.4/duwi_smart_sdk/model/req/device_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.3/duwi_smart_sdk/model/resp/auth.py` & `duwi_smart_sdk-0.1.4/duwi_smart_sdk/model/resp/auth.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.3/duwi_smart_sdk/model/resp/device.py` & `duwi_smart_sdk-0.1.4/duwi_smart_sdk/model/resp/device.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.3/duwi_smart_sdk/model/resp/house.py` & `duwi_smart_sdk-0.1.4/duwi_smart_sdk/model/resp/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.3/duwi_smart_sdk/util/http.py` & `duwi_smart_sdk-0.1.4/duwi_smart_sdk/util/http.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.3/duwi_smart_sdk/util/sign.py` & `duwi_smart_sdk-0.1.4/duwi_smart_sdk/util/sign.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.3/duwi_smart_sdk.egg-info/PKG-INFO` & `duwi_smart_sdk-0.1.4/duwi_smart_sdk.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi-smart-sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smart_sdk-0.1.3/duwi_smart_sdk.egg-info/SOURCES.txt` & `duwi_smart_sdk-0.1.4/duwi_smart_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.3/setup.py` & `duwi_smart_sdk-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 DESCRIPTION = 'sdk for duwi third platform'
 
 setup(
     name="duwi_smart_sdk",
     version=VERSION,
     author="ledger",
     author_email="ledgerbiggg@gmail.com",
```

### Comparing `duwi_smart_sdk-0.1.3/test/api/test_control.py` & `duwi_smart_sdk-0.1.4/test/api/test_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.3/test/api/test_discover.py` & `duwi_smart_sdk-0.1.4/test/api/test_discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.3/test/api/test_house.py` & `duwi_smart_sdk-0.1.4/test/api/test_house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.3/test/api/test_login.py` & `duwi_smart_sdk-0.1.4/test/api/test_login.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.3/test/api/test_ws.py` & `duwi_smart_sdk-0.1.4/test/api/test_ws.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.3/test/util/test_http.py` & `duwi_smart_sdk-0.1.4/test/util/test_http.py`

 * *Files identical despite different names*

