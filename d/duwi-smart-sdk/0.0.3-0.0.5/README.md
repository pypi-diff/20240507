# Comparing `tmp/duwi_smart_sdk-0.0.3.tar.gz` & `tmp/duwi_smart_sdk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duwi_smart_sdk-0.0.3.tar", last modified: Tue May  7 01:14:33 2024, max compression
+gzip compressed data, was "duwi_smart_sdk-0.0.5.tar", last modified: Tue May  7 01:28:11 2024, max compression
```

## Comparing `duwi_smart_sdk-0.0.3.tar` & `duwi_smart_sdk-0.0.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 01:14:33.068988 duwi_smart_sdk-0.0.3/
--rw-rw-rw-   0        0        0      628 2024-05-07 01:14:33.068988 duwi_smart_sdk-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      145 2024-05-07 01:14:28.000000 duwi_smart_sdk-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 01:14:33.026952 duwi_smart_sdk-0.0.3/duwi_smart_sdk/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 01:14:33.043570 duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/__init__.py
--rw-rw-rw-   0        0        0     1361 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/control.py
--rw-rw-rw-   0        0        0     2597 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/discover.py
--rw-rw-rw-   0        0        0     2188 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/house.py
--rw-rw-rw-   0        0        0     1723 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/login.py
--rw-rw-rw-   0        0        0     1534 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/refresh_token.py
--rw-rw-rw-   0        0        0     3917 2024-05-07 01:11:44.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/ws.py
-drwxrwxrwx   0        0        0        0 2024-05-07 01:14:33.048441 duwi_smart_sdk-0.0.3/duwi_smart_sdk/const/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/const/__init__.py
--rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/const/const.py
--rw-rw-rw-   0        0        0      279 2024-05-07 01:12:57.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/const/status.py
--rw-rw-rw-   0        0        0     1194 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/const/type_map.py
-drwxrwxrwx   0        0        0        0 2024-05-07 01:14:33.049416 duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 01:14:33.052350 duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/req/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/req/__init__.py
--rw-rw-rw-   0        0        0     1584 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/req/device_control.py
-drwxrwxrwx   0        0        0        0 2024-05-07 01:14:33.059217 duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/resp/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/resp/__init__.py
--rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/resp/auth.py
--rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/resp/control.py
--rw-rw-rw-   0        0        0     2767 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/resp/device.py
--rw-rw-rw-   0        0        0     1113 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/resp/house.py
-drwxrwxrwx   0        0        0        0 2024-05-07 01:14:33.064099 duwi_smart_sdk-0.0.3/duwi_smart_sdk/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/util/__init__.py
--rw-rw-rw-   0        0        0     1926 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/util/http.py
--rw-rw-rw-   0        0        0      906 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/util/sign.py
--rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk/util/timestamp.py
-drwxrwxrwx   0        0        0        0 2024-05-07 01:14:33.033788 duwi_smart_sdk-0.0.3/duwi_smart_sdk.egg-info/
--rw-rw-rw-   0        0        0      628 2024-05-07 01:14:32.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1087 2024-05-07 01:14:32.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 01:14:32.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-07 01:14:32.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-07 01:14:32.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-07 01:14:32.000000 duwi_smart_sdk-0.0.3/duwi_smart_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 01:14:33.069958 duwi_smart_sdk-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      908 2024-05-07 01:13:21.000000 duwi_smart_sdk-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 01:14:33.065076 duwi_smart_sdk-0.0.3/test/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 01:14:33.067034 duwi_smart_sdk-0.0.3/test/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/test/util/__init__.py
--rw-rw-rw-   0        0        0     1192 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.3/test/util/test_http.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:28:11.813397 duwi_smart_sdk-0.0.5/
+-rw-rw-rw-   0        0        0      628 2024-05-07 01:28:11.813397 duwi_smart_sdk-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      145 2024-05-07 01:14:28.000000 duwi_smart_sdk-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 01:28:11.758141 duwi_smart_sdk-0.0.5/duwi_smart_sdk/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:28:11.788875 duwi_smart_sdk-0.0.5/duwi_smart_sdk/api/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk/api/__init__.py
+-rw-rw-rw-   0        0        0     1361 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk/api/control.py
+-rw-rw-rw-   0        0        0     2597 2024-05-07 01:23:47.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk/api/discover.py
+-rw-rw-rw-   0        0        0     2188 2024-05-07 01:23:47.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk/api/house.py
+-rw-rw-rw-   0        0        0     1723 2024-05-07 01:23:47.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk/api/login.py
+-rw-rw-rw-   0        0        0     1534 2024-05-07 01:23:50.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk/api/refresh_token.py
+-rw-rw-rw-   0        0        0     3917 2024-05-07 01:23:47.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk/api/ws.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:28:11.793759 duwi_smart_sdk-0.0.5/duwi_smart_sdk/const/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk/const/__init__.py
+-rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk/const/const.py
+-rw-rw-rw-   0        0        0      279 2024-05-07 01:12:57.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk/const/status.py
+-rw-rw-rw-   0        0        0     1194 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk/const/type_map.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:28:11.795712 duwi_smart_sdk-0.0.5/duwi_smart_sdk/model/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:28:11.797665 duwi_smart_sdk-0.0.5/duwi_smart_sdk/model/req/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk/model/req/__init__.py
+-rw-rw-rw-   0        0        0     1584 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk/model/req/device_control.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:28:11.804058 duwi_smart_sdk-0.0.5/duwi_smart_sdk/model/resp/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk/model/resp/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk/model/resp/auth.py
+-rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk/model/resp/control.py
+-rw-rw-rw-   0        0        0     2767 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk/model/resp/device.py
+-rw-rw-rw-   0        0        0     1113 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk/model/resp/house.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:28:11.808514 duwi_smart_sdk-0.0.5/duwi_smart_sdk/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk/util/__init__.py
+-rw-rw-rw-   0        0        0     1926 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk/util/http.py
+-rw-rw-rw-   0        0        0      906 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk/util/sign.py
+-rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk/util/timestamp.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:28:11.766373 duwi_smart_sdk-0.0.5/duwi_smart_sdk.egg-info/
+-rw-rw-rw-   0        0        0      628 2024-05-07 01:28:11.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1087 2024-05-07 01:28:11.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 01:28:11.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-07 01:28:11.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-07 01:28:11.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-07 01:28:11.000000 duwi_smart_sdk-0.0.5/duwi_smart_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 01:28:11.813397 duwi_smart_sdk-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      908 2024-05-07 01:27:55.000000 duwi_smart_sdk-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:28:11.809491 duwi_smart_sdk-0.0.5/test/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.5/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:28:11.811443 duwi_smart_sdk-0.0.5/test/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.5/test/util/__init__.py
+-rw-rw-rw-   0        0        0     1192 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.5/test/util/test_http.py
```

### Comparing `duwi_smart_sdk-0.0.3/PKG-INFO` & `duwi_smart_sdk-0.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smart_sdk
-Version: 0.0.3
+Version: 0.0.5
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/control.py` & `duwi_smart_sdk-0.0.5/duwi_smart_sdk/api/control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/discover.py` & `duwi_smart_sdk-0.0.5/duwi_smart_sdk/api/discover.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             'secret': self._app_secret,
             'time': current_timestamp(),
             'sign': sign
         }
 
         status, message, res = await get(self._url + f"/device/infos?houseNo={house_no}", headers, body)
 
-        if status == Code.Success.value:
+        if status == Code.SUCCESS.value:
             devices = res.get("devices", [])
             devices_objects = [self._create_device_obj(device) for device in devices]
             return status, devices_objects
         else:
             return status, None
 
     @staticmethod
```

### Comparing `duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/house.py` & `duwi_smart_sdk-0.0.5/duwi_smart_sdk/api/house.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             'secret': self._app_secret,
             'time': current_timestamp(),
             'sign': sign
         }
 
         status, message, res = await get(URL + "/house/infos", headers, body)
 
-        if status == Code.Success.value:
+        if status == Code.SUCCESS.value:
             house_infos = res.get('houseInfos', [])
             house_info_objects = [self._create_house_info_obj(h_info) for h_info in house_infos]
             return status, house_info_objects
 
         return status, None
 
     @staticmethod
```

### Comparing `duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/login.py` & `duwi_smart_sdk-0.0.5/duwi_smart_sdk/api/login.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             'appkey': self._app_key,
             'secret': self._app_secret,
             'time': current_timestamp(),
             'sign': sign
         }
         status, message, res = await post(self._url + "/account/login", header, body)
 
-        if status == Code.Success.value:
+        if status == Code.SUCCESS.value:
             return status, AuthToken(
                 access_token=res.get("accessToken"),
                 access_token_expire_time=res.get("accessTokenExpireTime"),
                 refresh_token=res.get("refreshToken"),
                 refresh_token_expire_time=res.get("refreshTokenExpireTime")
             )
         else:
```

### Comparing `duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/refresh_token.py` & `duwi_smart_sdk-0.0.5/duwi_smart_sdk/api/refresh_token.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             'appkey': self._app_key,
             'secret': self._app_secret,
             'time': current_timestamp(),
             'sign': sign
         }
 
         status, message, res = await put(self._url + "/account/token", headers, body)
-        if status == Code.Success.value:
+        if status == Code.SUCCESS.value:
             return status, AuthToken(
                 access_token=res.get("accessToken"),
                 access_token_expire_time=res.get("accessTokenExpireTime"),
                 refresh_token=res.get("refreshToken"),
                 refresh_token_expire_time=res.get("refreshTokenExpireTime")
             )
         else:
```

### Comparing `duwi_smart_sdk-0.0.3/duwi_smart_sdk/api/ws.py` & `duwi_smart_sdk-0.0.5/duwi_smart_sdk/api/ws.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         )
 
     async def refresh_token(self):
         auth = AuthTokenRefresherClient(app_key=self._app_key, app_secret=self._app_secret)
         while True:
             status, token = await auth.refresh(
                 refresh_token=self._refresh_token)
-            if status == Code.Success.value:
+            if status == Code.SUCCESS.value:
                 self._access_token = token.access_token
                 self._refresh_token = token.refresh_token
             await asyncio.sleep(432000)
 
     async def keep_alive(self):
         while True:
             try:
```

### Comparing `duwi_smart_sdk-0.0.3/duwi_smart_sdk/const/type_map.py` & `duwi_smart_sdk-0.0.5/duwi_smart_sdk/const/type_map.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/req/device_control.py` & `duwi_smart_sdk-0.0.5/duwi_smart_sdk/model/req/device_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/resp/auth.py` & `duwi_smart_sdk-0.0.5/duwi_smart_sdk/model/resp/auth.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/resp/device.py` & `duwi_smart_sdk-0.0.5/duwi_smart_sdk/model/resp/device.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.3/duwi_smart_sdk/model/resp/house.py` & `duwi_smart_sdk-0.0.5/duwi_smart_sdk/model/resp/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.3/duwi_smart_sdk/util/http.py` & `duwi_smart_sdk-0.0.5/duwi_smart_sdk/util/http.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.3/duwi_smart_sdk/util/sign.py` & `duwi_smart_sdk-0.0.5/duwi_smart_sdk/util/sign.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.3/duwi_smart_sdk.egg-info/PKG-INFO` & `duwi_smart_sdk-0.0.5/duwi_smart_sdk.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi-smart-sdk
-Version: 0.0.3
+Version: 0.0.5
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smart_sdk-0.0.3/duwi_smart_sdk.egg-info/SOURCES.txt` & `duwi_smart_sdk-0.0.5/duwi_smart_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.3/setup.py` & `duwi_smart_sdk-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3'
+VERSION = '0.0.5'
 DESCRIPTION = 'sdk for duwi third platform'
 
 setup(
     name="duwi_smart_sdk",
     version=VERSION,
     author="ledger",
     author_email="ledgerbiggg@gmail.com",
```

### Comparing `duwi_smart_sdk-0.0.3/test/util/test_http.py` & `duwi_smart_sdk-0.0.5/test/util/test_http.py`

 * *Files identical despite different names*

