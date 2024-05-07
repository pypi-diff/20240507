# Comparing `tmp/duwi_smart_sdk-0.0.8.tar.gz` & `tmp/duwi_smart_sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duwi_smart_sdk-0.0.8.tar", last modified: Tue May  7 02:13:48 2024, max compression
+gzip compressed data, was "duwi_smart_sdk-0.0.9.tar", last modified: Tue May  7 06:48:12 2024, max compression
```

## Comparing `duwi_smart_sdk-0.0.8.tar` & `duwi_smart_sdk-0.0.9.tar`

### file list

```diff
@@ -1,48 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 02:13:48.951478 duwi_smart_sdk-0.0.8/
--rw-rw-rw-   0        0        0      628 2024-05-07 02:13:48.950500 duwi_smart_sdk-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      145 2024-05-07 01:14:28.000000 duwi_smart_sdk-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 02:13:48.906577 duwi_smart_sdk-0.0.8/duwi_smart_sdk/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 02:13:48.920322 duwi_smart_sdk-0.0.8/duwi_smart_sdk/api/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk/api/__init__.py
--rw-rw-rw-   0        0        0     1361 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk/api/control.py
--rw-rw-rw-   0        0        0     2597 2024-05-07 01:23:47.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk/api/discover.py
--rw-rw-rw-   0        0        0     2188 2024-05-07 01:23:47.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk/api/house.py
--rw-rw-rw-   0        0        0     1723 2024-05-07 01:23:47.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk/api/login.py
--rw-rw-rw-   0        0        0     1534 2024-05-07 01:23:50.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk/api/refresh_token.py
--rw-rw-rw-   0        0        0     4330 2024-05-07 02:13:30.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk/api/ws.py
-drwxrwxrwx   0        0        0        0 2024-05-07 02:13:48.924881 duwi_smart_sdk-0.0.8/duwi_smart_sdk/const/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk/const/__init__.py
--rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk/const/const.py
--rw-rw-rw-   0        0        0      279 2024-05-07 01:12:57.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk/const/status.py
--rw-rw-rw-   0        0        0     1194 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk/const/type_map.py
-drwxrwxrwx   0        0        0        0 2024-05-07 02:13:48.925866 duwi_smart_sdk-0.0.8/duwi_smart_sdk/model/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 02:13:48.927815 duwi_smart_sdk-0.0.8/duwi_smart_sdk/model/req/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk/model/req/__init__.py
--rw-rw-rw-   0        0        0     1584 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk/model/req/device_control.py
-drwxrwxrwx   0        0        0        0 2024-05-07 02:13:48.936925 duwi_smart_sdk-0.0.8/duwi_smart_sdk/model/resp/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk/model/resp/__init__.py
--rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk/model/resp/auth.py
--rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk/model/resp/control.py
--rw-rw-rw-   0        0        0     2767 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk/model/resp/device.py
--rw-rw-rw-   0        0        0     1113 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk/model/resp/house.py
-drwxrwxrwx   0        0        0        0 2024-05-07 02:13:48.944252 duwi_smart_sdk-0.0.8/duwi_smart_sdk/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk/util/__init__.py
--rw-rw-rw-   0        0        0     1926 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk/util/http.py
--rw-rw-rw-   0        0        0      906 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk/util/sign.py
--rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk/util/timestamp.py
-drwxrwxrwx   0        0        0        0 2024-05-07 02:13:48.912434 duwi_smart_sdk-0.0.8/duwi_smart_sdk.egg-info/
--rw-rw-rw-   0        0        0      628 2024-05-07 02:13:48.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1087 2024-05-07 02:13:48.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 02:13:48.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-07 02:13:48.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-07 02:13:48.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-07 02:13:48.000000 duwi_smart_sdk-0.0.8/duwi_smart_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 02:13:48.951478 duwi_smart_sdk-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      908 2024-05-07 02:13:44.000000 duwi_smart_sdk-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 02:13:48.945612 duwi_smart_sdk-0.0.8/test/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.8/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 02:13:48.949523 duwi_smart_sdk-0.0.8/test/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.8/test/util/__init__.py
--rw-rw-rw-   0        0        0     1192 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.8/test/util/test_http.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:48:12.992642 duwi_smart_sdk-0.0.9/
+-rw-rw-rw-   0        0        0      649 2024-05-07 06:48:12.992642 duwi_smart_sdk-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2024-05-07 06:42:21.000000 duwi_smart_sdk-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 06:48:12.950208 duwi_smart_sdk-0.0.9/duwi_smart_sdk/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:48:12.963883 duwi_smart_sdk-0.0.9/duwi_smart_sdk/api/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/api/__init__.py
+-rw-rw-rw-   0        0        0     2095 2024-05-07 06:43:46.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/api/account.py
+-rw-rw-rw-   0        0        0     2784 2024-05-07 06:21:35.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/api/control.py
+-rw-rw-rw-   0        0        0     4309 2024-05-07 06:25:47.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/api/discover.py
+-rw-rw-rw-   0        0        0     2695 2024-05-07 06:09:49.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/api/house.py
+-rw-rw-rw-   0        0        0     2153 2024-05-07 06:09:49.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/api/refresh_token.py
+-rw-rw-rw-   0        0        0     4123 2024-05-07 05:45:38.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/api/ws.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:48:12.968761 duwi_smart_sdk-0.0.9/duwi_smart_sdk/const/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/const/__init__.py
+-rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/const/const.py
+-rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/const/status.py
+-rw-rw-rw-   0        0        0     1154 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/const/type_map.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:48:12.969738 duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:48:12.970716 duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/req/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/req/__init__.py
+-rw-rw-rw-   0        0        0     1584 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/req/device_control.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:48:12.976479 duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/resp/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/resp/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/resp/auth.py
+-rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/resp/control.py
+-rw-rw-rw-   0        0        0     2767 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/resp/device.py
+-rw-rw-rw-   0        0        0     1113 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/resp/house.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:48:12.980920 duwi_smart_sdk-0.0.9/duwi_smart_sdk/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/util/__init__.py
+-rw-rw-rw-   0        0        0     1926 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/util/http.py
+-rw-rw-rw-   0        0        0      906 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/util/sign.py
+-rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk/util/timestamp.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:48:12.956073 duwi_smart_sdk-0.0.9/duwi_smart_sdk.egg-info/
+-rw-rw-rw-   0        0        0      649 2024-05-07 06:48:12.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1227 2024-05-07 06:48:12.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 06:48:12.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-07 06:48:12.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-07 06:48:12.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-07 06:48:12.000000 duwi_smart_sdk-0.0.9/duwi_smart_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 06:48:12.992642 duwi_smart_sdk-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      936 2024-05-07 06:47:57.000000 duwi_smart_sdk-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:48:12.981896 duwi_smart_sdk-0.0.9/test/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:48:12.988734 duwi_smart_sdk-0.0.9/test/api/
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:10:48.000000 duwi_smart_sdk-0.0.9/test/api/__init__.py
+-rw-rw-rw-   0        0        0      949 2024-05-07 06:21:35.000000 duwi_smart_sdk-0.0.9/test/api/test_control.py
+-rw-rw-rw-   0        0        0      812 2024-05-07 06:26:29.000000 duwi_smart_sdk-0.0.9/test/api/test_discover.py
+-rw-rw-rw-   0        0        0      687 2024-05-07 06:29:35.000000 duwi_smart_sdk-0.0.9/test/api/test_house.py
+-rw-rw-rw-   0        0        0      640 2024-05-07 06:43:46.000000 duwi_smart_sdk-0.0.9/test/api/test_login.py
+-rw-rw-rw-   0        0        0      894 2024-05-07 06:41:28.000000 duwi_smart_sdk-0.0.9/test/api/test_ws.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:48:12.990687 duwi_smart_sdk-0.0.9/test/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.9/test/util/__init__.py
+-rw-rw-rw-   0        0        0     1222 2024-05-07 06:12:53.000000 duwi_smart_sdk-0.0.9/test/util/test_http.py
```

### Comparing `duwi_smart_sdk-0.0.8/PKG-INFO` & `duwi_smart_sdk-0.0.9/duwi_smart_sdk.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: duwi_smart_sdk
-Version: 0.0.8
+Name: duwi-smart-sdk
+Version: 0.0.9
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
-Keywords: python,duwi
+Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 install sdk
@@ -20,7 +20,8 @@
 
 Update existing dependencies
 ```shell
 pip install --upgrade duwi-smart-sdk
 ```
 
 
+
```

### Comparing `duwi_smart_sdk-0.0.8/duwi_smart_sdk/api/login.py` & `duwi_smart_sdk-0.0.9/duwi_smart_sdk/api/account.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,39 +4,49 @@
 from duwi_smart_sdk.const.status import Code
 from duwi_smart_sdk.const.const import URL
 from duwi_smart_sdk.util.sign import md5_encrypt
 from duwi_smart_sdk.util.timestamp import current_timestamp
 from duwi_smart_sdk.model.resp.auth import AuthToken
 
 
-class LoginClient:
-    def __init__(self, app_key: str, app_secret: str):
+class AccountClient:
+    def __init__(self,
+                 app_key: str,
+                 app_secret: str,
+                 app_version: str,
+                 client_version: str,
+                 client_model: str = None
+                 ):
         self._url = URL
         self._app_key = app_key
         self._app_secret = app_secret
-        # 设置默认值，如果未传入headers或body
+        self._app_version = app_version
+        self._client_version = client_version
+        self._client_model = client_model
 
     async def login(self, phone: str, password: str) -> tuple[str, AuthToken | None]:
         # 更新body的内容，传入phone和password
         body = {
             "phone": phone,
             "password": password,
         }
         body_string = json.dumps(body, separators=(',', ':'))
         sign = md5_encrypt(body_string + self._app_key + str(current_timestamp()))
 
-        # 更新headers的内容，传入必要的认证信息
-        header = {
+        headers = {
             'Content-Type': 'application/json',
             'appkey': self._app_key,
             'secret': self._app_secret,
-            'time': current_timestamp(),
-            'sign': sign
+            'time': str(current_timestamp()),  # Ensure it's converted to string
+            'sign': sign,
+            'appVersion': self._app_version,
+            'clientVersion': self._client_version,
+            'clientModel': self._client_model
         }
-        status, message, res = await post(self._url + "/account/login", header, body)
+        status, message, res = await post(self._url + "/account/login", headers, body)
 
         if status == Code.SUCCESS.value:
             return status, AuthToken(
                 access_token=res.get("accessToken"),
                 access_token_expire_time=res.get("accessTokenExpireTime"),
                 refresh_token=res.get("refreshToken"),
                 refresh_token_expire_time=res.get("refreshTokenExpireTime")
```

### Comparing `duwi_smart_sdk-0.0.8/duwi_smart_sdk/api/refresh_token.py` & `duwi_smart_sdk-0.0.9/duwi_smart_sdk/api/refresh_token.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,33 +5,48 @@
 from duwi_smart_sdk.const.status import Code
 from duwi_smart_sdk.util.sign import md5_encrypt
 from duwi_smart_sdk.util.timestamp import current_timestamp
 from duwi_smart_sdk.model.resp.auth import AuthToken
 
 
 class AuthTokenRefresherClient:
-    def __init__(self, app_key: str, app_secret: str):
+    def __init__(self,
+                 app_key: str,
+                 app_secret: str,
+                 access_token: str,
+                 app_version: str,
+                 client_version: str,
+                 client_model: str = None
+                 ):
         self._url = URL
         self._app_key = app_key
         self._app_secret = app_secret
+        self._access_token = access_token
+        self._app_version = app_version
+        self._client_version = client_version
+        self._client_model = client_model
 
     async def refresh(self, refresh_token: str) -> tuple[str, AuthToken | None]:
         body = {
             "refreshToken": refresh_token,
         }
 
         body_string = json.dumps(body, separators=(',', ':'))
         sign = md5_encrypt(body_string + self._app_key + str(current_timestamp()))
 
         headers = {
             'Content-Type': 'application/json',
+            'accessToken': self._access_token,
             'appkey': self._app_key,
             'secret': self._app_secret,
-            'time': current_timestamp(),
-            'sign': sign
+            'time': str(current_timestamp()),  # Ensure it's converted to string
+            'sign': sign,
+            'appVersion': self._app_version,
+            'clientVersion': self._client_version,
+            'clientModel': self._client_model
         }
 
         status, message, res = await put(self._url + "/account/token", headers, body)
         if status == Code.SUCCESS.value:
             return status, AuthToken(
                 access_token=res.get("accessToken"),
                 access_token_expire_time=res.get("accessTokenExpireTime"),
```

### Comparing `duwi_smart_sdk-0.0.8/duwi_smart_sdk/api/ws.py` & `duwi_smart_sdk-0.0.9/duwi_smart_sdk/api/ws.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,31 +27,29 @@
         self._is_over = False
         self._connection = None
 
     async def close(self):
         self._is_over = True
         if self._connection:
             await self._connection.close()
+
     async def connect(self):
-        _LOGGER.info(f"ws connect {self._server_uri}")
         self._connection = await websockets.connect(self._server_uri)
 
     async def send(self, message):
-        _LOGGER.info(f"ws send {message}")
         if self._connection:
             await self._connection.send(message)
 
     async def disconnect(self):
         if self._connection:
             await self._connection.close()
 
     async def reconnect(self):
         if self._is_over:
             return
-        _LOGGER.info("ws reconnect --------------")
         await self.connect()
         await self.link()
         await self.bind()
 
     async def listen(self):
         while True:
             try:
@@ -94,15 +92,15 @@
             if self._is_over:
                 return
             status, token = await auth.refresh(
                 refresh_token=self._refresh_token)
             if status == Code.SUCCESS.value:
                 self._access_token = token.access_token
                 self._refresh_token = token.refresh_token
-            await asyncio.sleep(432000)
+            await asyncio.sleep(5 * 24 * 60 * 60)
 
     async def keep_alive(self):
         while True:
             try:
                 if self._is_over:
                     return
                 await self.send('KEEPALIVE')
@@ -116,9 +114,8 @@
             try:
                 if message == "KEEPALIVE":
                     continue
                 _LOGGER.info(f"ws接受消息:{message}")
                 message = str.replace(message, "&excision&", "")
                 await self._on_callback(message)
             except Exception as e:
-                _LOGGER.error(f"ws接受消息出现异常:{e}")
                 _LOGGER.error(f"error message detail: \n{traceback.format_exc()}")
```

### Comparing `duwi_smart_sdk-0.0.8/duwi_smart_sdk/const/type_map.py` & `duwi_smart_sdk-0.0.9/duwi_smart_sdk/const/type_map.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,11 +40,7 @@
     #     "7-003-001": "light",
     #     "7-011-001": "volatileOrganicCompounds",
     #     "7-005-001": "pm25",
     #     "7-006-001": "carbonDioxide",
     #     "7-010-001": "carbonMonoxide",
     # }
 }
-# 指令映射
-instruction_map = {
-
-}
```

### Comparing `duwi_smart_sdk-0.0.8/duwi_smart_sdk/model/req/device_control.py` & `duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/req/device_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.8/duwi_smart_sdk/model/resp/auth.py` & `duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/resp/auth.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.8/duwi_smart_sdk/model/resp/device.py` & `duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/resp/device.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.8/duwi_smart_sdk/model/resp/house.py` & `duwi_smart_sdk-0.0.9/duwi_smart_sdk/model/resp/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.8/duwi_smart_sdk/util/http.py` & `duwi_smart_sdk-0.0.9/duwi_smart_sdk/util/http.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.8/duwi_smart_sdk/util/sign.py` & `duwi_smart_sdk-0.0.9/duwi_smart_sdk/util/sign.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.8/duwi_smart_sdk.egg-info/PKG-INFO` & `duwi_smart_sdk-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: duwi-smart-sdk
-Version: 0.0.8
+Name: duwi_smart_sdk
+Version: 0.0.9
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
-Keywords: python,duwi
+Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 install sdk
@@ -20,7 +20,8 @@
 
 Update existing dependencies
 ```shell
 pip install --upgrade duwi-smart-sdk
 ```
 
 
+
```

### Comparing `duwi_smart_sdk-0.0.8/duwi_smart_sdk.egg-info/SOURCES.txt` & `duwi_smart_sdk-0.0.9/duwi_smart_sdk.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 duwi_smart_sdk.egg-info/PKG-INFO
 duwi_smart_sdk.egg-info/SOURCES.txt
 duwi_smart_sdk.egg-info/dependency_links.txt
 duwi_smart_sdk.egg-info/entry_points.txt
 duwi_smart_sdk.egg-info/requires.txt
 duwi_smart_sdk.egg-info/top_level.txt
 duwi_smart_sdk/api/__init__.py
+duwi_smart_sdk/api/account.py
 duwi_smart_sdk/api/control.py
 duwi_smart_sdk/api/discover.py
 duwi_smart_sdk/api/house.py
-duwi_smart_sdk/api/login.py
 duwi_smart_sdk/api/refresh_token.py
 duwi_smart_sdk/api/ws.py
 duwi_smart_sdk/const/__init__.py
 duwi_smart_sdk/const/const.py
 duwi_smart_sdk/const/status.py
 duwi_smart_sdk/const/type_map.py
 duwi_smart_sdk/model/__init__.py
@@ -27,9 +27,15 @@
 duwi_smart_sdk/model/resp/device.py
 duwi_smart_sdk/model/resp/house.py
 duwi_smart_sdk/util/__init__.py
 duwi_smart_sdk/util/http.py
 duwi_smart_sdk/util/sign.py
 duwi_smart_sdk/util/timestamp.py
 test/__init__.py
+test/api/__init__.py
+test/api/test_control.py
+test/api/test_discover.py
+test/api/test_house.py
+test/api/test_login.py
+test/api/test_ws.py
 test/util/__init__.py
 test/util/test_http.py
```

### Comparing `duwi_smart_sdk-0.0.8/test/util/test_http.py` & `duwi_smart_sdk-0.0.9/test/util/test_http.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 from unittest import TestCase
 
-from util.http import get
-from util.timestamp import current_timestamp
+from duwi_smart_sdk.util.http import get
+from duwi_smart_sdk.util.timestamp import current_timestamp
 
 
 class TestGet(TestCase):
     def test_get(self):
         # 定义一个运行异步测试的辅助函数
         async def run_test():
             url = "http://8.140.128.174:8019/homeApi/v1/house/infos"  # 用你想要测试的URL替换这个
```

