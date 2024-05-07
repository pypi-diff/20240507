# Comparing `tmp/duwi_smart_sdk-0.0.9.tar.gz` & `tmp/duwi_smart_sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duwi_smart_sdk-0.0.9.tar", last modified: Tue May  7 06:48:12 2024, max compression
+gzip compressed data, was "duwi_smart_sdk-0.1.1.tar", last modified: Tue May  7 07:06:30 2024, max compression
```

## Comparing `duwi_smart_sdk-0.0.9.tar` & `duwi_smart_sdk-0.1.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 06:48:12.992642 duwi_smart_sdk-0.0.9/
--rw-rw-rw-   0        0        0      649 2024-05-07 06:48:12.992642 duwi_smart_sdk-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      147 2024-05-07 06:42:21.000000 duwi_smart_sdk-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 06:48:12.950208 duwi_smart_sdk-0.0.9/duwi_smart_sdk/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:48:12.963883 duwi_smart_sdk-0.0.9/duwi_smart_sdk/api/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/api/__init__.py
--rw-rw-rw-   0        0        0     2095 2024-05-07 06:43:46.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/api/account.py
--rw-rw-rw-   0        0        0     2784 2024-05-07 06:21:35.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/api/control.py
--rw-rw-rw-   0        0        0     4309 2024-05-07 06:25:47.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/api/discover.py
--rw-rw-rw-   0        0        0     2695 2024-05-07 06:09:49.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/api/house.py
--rw-rw-rw-   0        0        0     2153 2024-05-07 06:09:49.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/api/refresh_token.py
--rw-rw-rw-   0        0        0     4123 2024-05-07 05:45:38.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/api/ws.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:48:12.968761 duwi_smart_sdk-0.0.9/duwi_smart_sdk/const/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/const/__init__.py
--rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/const/const.py
--rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/const/status.py
--rw-rw-rw-   0        0        0     1154 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/const/type_map.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:48:12.969738 duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:48:12.970716 duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/req/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/req/__init__.py
--rw-rw-rw-   0        0        0     1584 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/req/device_control.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:48:12.976479 duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/resp/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/resp/__init__.py
--rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/resp/auth.py
--rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/resp/control.py
--rw-rw-rw-   0        0        0     2767 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/resp/device.py
--rw-rw-rw-   0        0        0     1113 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/resp/house.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:48:12.980920 duwi_smart_sdk-0.0.9/duwi_smart_sdk/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/util/__init__.py
--rw-rw-rw-   0        0        0     1926 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/util/http.py
--rw-rw-rw-   0        0        0      906 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/util/sign.py
--rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/util/timestamp.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:48:12.956073 duwi_smart_sdk-0.0.9/duwi_smart_sdk.egg-info/
--rw-rw-rw-   0        0        0      649 2024-05-07 06:48:12.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1227 2024-05-07 06:48:12.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 06:48:12.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-07 06:48:12.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-07 06:48:12.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-07 06:48:12.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 06:48:12.992642 duwi_smart_sdk-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      936 2024-05-07 06:47:57.000000 duwi_smart_sdk-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:48:12.981896 duwi_smart_sdk-0.0.9/test/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:48:12.988734 duwi_smart_sdk-0.0.9/test/api/
--rw-rw-rw-   0        0        0        0 2024-05-07 06:10:48.000000 duwi_smart_sdk-0.0.9/test/api/__init__.py
--rw-rw-rw-   0        0        0      949 2024-05-07 06:21:35.000000 duwi_smart_sdk-0.0.9/test/api/test_control.py
--rw-rw-rw-   0        0        0      812 2024-05-07 06:26:29.000000 duwi_smart_sdk-0.0.9/test/api/test_discover.py
--rw-rw-rw-   0        0        0      687 2024-05-07 06:29:35.000000 duwi_smart_sdk-0.0.9/test/api/test_house.py
--rw-rw-rw-   0        0        0      640 2024-05-07 06:43:46.000000 duwi_smart_sdk-0.0.9/test/api/test_login.py
--rw-rw-rw-   0        0        0      894 2024-05-07 06:41:28.000000 duwi_smart_sdk-0.0.9/test/api/test_ws.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:48:12.990687 duwi_smart_sdk-0.0.9/test/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/test/util/__init__.py
--rw-rw-rw-   0        0        0     1222 2024-05-07 06:12:53.000000 duwi_smart_sdk-0.0.9/test/util/test_http.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:06:30.169222 duwi_smart_sdk-0.1.1/
+-rw-rw-rw-   0        0        0      649 2024-05-07 07:06:30.169222 duwi_smart_sdk-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2024-05-07 06:42:21.000000 duwi_smart_sdk-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 07:06:30.112766 duwi_smart_sdk-0.1.1/duwi_smart_sdk/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:06:30.128345 duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/__init__.py
+-rw-rw-rw-   0        0        0     2095 2024-05-07 06:43:46.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/account.py
+-rw-rw-rw-   0        0        0     2784 2024-05-07 06:21:35.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/control.py
+-rw-rw-rw-   0        0        0     4309 2024-05-07 06:25:47.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/discover.py
+-rw-rw-rw-   0        0        0     2695 2024-05-07 06:09:49.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/house.py
+-rw-rw-rw-   0        0        0     2153 2024-05-07 06:09:49.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/refresh_token.py
+-rw-rw-rw-   0        0        0     4717 2024-05-07 07:06:01.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/ws.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:06:30.134406 duwi_smart_sdk-0.1.1/duwi_smart_sdk/const/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/const/__init__.py
+-rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/const/const.py
+-rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/const/status.py
+-rw-rw-rw-   0        0        0     1154 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/const/type_map.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:06:30.135813 duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:06:30.138403 duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/req/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/req/__init__.py
+-rw-rw-rw-   0        0        0     1584 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/req/device_control.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:06:30.146280 duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/resp/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/resp/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/resp/auth.py
+-rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/resp/control.py
+-rw-rw-rw-   0        0        0     2767 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/resp/device.py
+-rw-rw-rw-   0        0        0     1113 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/resp/house.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:06:30.152763 duwi_smart_sdk-0.1.1/duwi_smart_sdk/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/util/__init__.py
+-rw-rw-rw-   0        0        0     1926 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/util/http.py
+-rw-rw-rw-   0        0        0      906 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/util/sign.py
+-rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk/util/timestamp.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:06:30.118630 duwi_smart_sdk-0.1.1/duwi_smart_sdk.egg-info/
+-rw-rw-rw-   0        0        0      649 2024-05-07 07:06:30.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1227 2024-05-07 07:06:30.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 07:06:30.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-07 07:06:30.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-07 07:06:30.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-07 07:06:30.000000 duwi_smart_sdk-0.1.1/duwi_smart_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 07:06:30.170199 duwi_smart_sdk-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      938 2024-05-07 07:06:23.000000 duwi_smart_sdk-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:06:30.153739 duwi_smart_sdk-0.1.1/test/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:06:30.164257 duwi_smart_sdk-0.1.1/test/api/
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:10:48.000000 duwi_smart_sdk-0.1.1/test/api/__init__.py
+-rw-rw-rw-   0        0        0      949 2024-05-07 06:21:35.000000 duwi_smart_sdk-0.1.1/test/api/test_control.py
+-rw-rw-rw-   0        0        0      812 2024-05-07 06:26:29.000000 duwi_smart_sdk-0.1.1/test/api/test_discover.py
+-rw-rw-rw-   0        0        0      687 2024-05-07 06:29:35.000000 duwi_smart_sdk-0.1.1/test/api/test_house.py
+-rw-rw-rw-   0        0        0      640 2024-05-07 06:43:46.000000 duwi_smart_sdk-0.1.1/test/api/test_login.py
+-rw-rw-rw-   0        0        0      894 2024-05-07 06:41:28.000000 duwi_smart_sdk-0.1.1/test/api/test_ws.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:06:30.167220 duwi_smart_sdk-0.1.1/test/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.1/test/util/__init__.py
+-rw-rw-rw-   0        0        0     1222 2024-05-07 06:12:53.000000 duwi_smart_sdk-0.1.1/test/util/test_http.py
```

### Comparing `duwi_smart_sdk-0.0.9/PKG-INFO` & `duwi_smart_sdk-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smart_sdk
-Version: 0.0.9
+Version: 0.1.1
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smart_sdk-0.0.9/duwi_smart_sdk/api/account.py` & `duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/account.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.9/duwi_smart_sdk/api/control.py` & `duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.9/duwi_smart_sdk/api/discover.py` & `duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.9/duwi_smart_sdk/api/house.py` & `duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.9/duwi_smart_sdk/api/refresh_token.py` & `duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/refresh_token.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.9/duwi_smart_sdk/api/ws.py` & `duwi_smart_sdk-0.1.1/duwi_smart_sdk/api/ws.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,23 +11,35 @@
 from duwi_smart_sdk.util.sign import md5_encrypt, sha256_base64
 from duwi_smart_sdk.util.timestamp import current_timestamp
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceSynchronizationWS:
-    def __init__(self, on_callback: callable, app_key: str, app_secret: str, access_token: str,
-                 refresh_token: str, house_no: str):
+    def __init__(self,
+                 on_callback: callable,
+                 app_key: str,
+                 app_secret: str,
+                 access_token: str,
+                 refresh_token: str,
+                 house_no: str,
+                 app_version: str,
+                 client_version: str,  # client_version
+                 client_model=None
+                 ):
         self._on_callback = on_callback
         self._server_uri = WS_URL
         self._app_key = app_key
         self._app_secret = app_secret
         self._access_token = access_token
         self._refresh_token = refresh_token
         self._house_no = house_no
+        self._app_version = app_version
+        self._client_version = client_version
+        self._client_model = client_model
         self._is_over = False
         self._connection = None
 
     async def close(self):
         self._is_over = True
         if self._connection:
             await self._connection.close()
@@ -83,15 +95,22 @@
         }
         json_string = json.dumps(data)
         await self.send(
             'BIND|' + json_string
         )
 
     async def refresh_token(self):
-        auth = AuthTokenRefresherClient(app_key=self._app_key, app_secret=self._app_secret)
+        auth = AuthTokenRefresherClient(
+            app_key=self._app_key,
+            app_secret=self._app_secret,
+            access_token=self._access_token,
+            app_version=self._app_version,
+            client_version=self._client_version,
+            client_model=self._client_model,
+        )
         while True:
             if self._is_over:
                 return
             status, token = await auth.refresh(
                 refresh_token=self._refresh_token)
             if status == Code.SUCCESS.value:
                 self._access_token = token.access_token
```

### Comparing `duwi_smart_sdk-0.0.9/duwi_smart_sdk/const/status.py` & `duwi_smart_sdk-0.1.1/duwi_smart_sdk/const/status.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.9/duwi_smart_sdk/const/type_map.py` & `duwi_smart_sdk-0.1.1/duwi_smart_sdk/const/type_map.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/req/device_control.py` & `duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/req/device_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/resp/auth.py` & `duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/resp/auth.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/resp/device.py` & `duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/resp/device.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/resp/house.py` & `duwi_smart_sdk-0.1.1/duwi_smart_sdk/model/resp/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.9/duwi_smart_sdk/util/http.py` & `duwi_smart_sdk-0.1.1/duwi_smart_sdk/util/http.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.9/duwi_smart_sdk/util/sign.py` & `duwi_smart_sdk-0.1.1/duwi_smart_sdk/util/sign.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.9/duwi_smart_sdk.egg-info/PKG-INFO` & `duwi_smart_sdk-0.1.1/duwi_smart_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi-smart-sdk
-Version: 0.0.9
+Version: 0.1.1
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smart_sdk-0.0.9/duwi_smart_sdk.egg-info/SOURCES.txt` & `duwi_smart_sdk-0.1.1/duwi_smart_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.9/setup.py` & `duwi_smart_sdk-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.9'
+VERSION = '0.1.001'
 DESCRIPTION = 'sdk for duwi third platform'
 
 setup(
     name="duwi_smart_sdk",
     version=VERSION,
     author="ledger",
     author_email="ledgerbiggg@gmail.com",
```

### Comparing `duwi_smart_sdk-0.0.9/test/api/test_control.py` & `duwi_smart_sdk-0.1.1/test/api/test_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.9/test/api/test_discover.py` & `duwi_smart_sdk-0.1.1/test/api/test_discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.9/test/api/test_house.py` & `duwi_smart_sdk-0.1.1/test/api/test_house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.9/test/api/test_login.py` & `duwi_smart_sdk-0.1.1/test/api/test_login.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.9/test/api/test_ws.py` & `duwi_smart_sdk-0.1.1/test/api/test_ws.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.9/test/util/test_http.py` & `duwi_smart_sdk-0.1.1/test/util/test_http.py`

 * *Files identical despite different names*

