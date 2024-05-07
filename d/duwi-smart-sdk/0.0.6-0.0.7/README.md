# Comparing `tmp/duwi_smart_sdk-0.0.6.tar.gz` & `tmp/duwi_smart_sdk-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duwi_smart_sdk-0.0.6.tar", last modified: Tue May  7 02:05:27 2024, max compression
+gzip compressed data, was "duwi_smart_sdk-0.0.7.tar", last modified: Tue May  7 02:10:05 2024, max compression
```

## Comparing `duwi_smart_sdk-0.0.6.tar` & `duwi_smart_sdk-0.0.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 02:05:27.113631 duwi_smart_sdk-0.0.6/
--rw-rw-rw-   0        0        0      628 2024-05-07 02:05:27.113631 duwi_smart_sdk-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      145 2024-05-07 01:14:28.000000 duwi_smart_sdk-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 02:05:27.074487 duwi_smart_sdk-0.0.6/duwi_smart_sdk/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 02:05:27.091162 duwi_smart_sdk-0.0.6/duwi_smart_sdk/api/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk/api/__init__.py
--rw-rw-rw-   0        0        0     1361 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk/api/control.py
--rw-rw-rw-   0        0        0     2597 2024-05-07 01:23:47.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk/api/discover.py
--rw-rw-rw-   0        0        0     2188 2024-05-07 01:23:47.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk/api/house.py
--rw-rw-rw-   0        0        0     1723 2024-05-07 01:23:47.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk/api/login.py
--rw-rw-rw-   0        0        0     1534 2024-05-07 01:23:50.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk/api/refresh_token.py
--rw-rw-rw-   0        0        0     4259 2024-05-07 02:05:21.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk/api/ws.py
-drwxrwxrwx   0        0        0        0 2024-05-07 02:05:27.096045 duwi_smart_sdk-0.0.6/duwi_smart_sdk/const/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk/const/__init__.py
--rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk/const/const.py
--rw-rw-rw-   0        0        0      279 2024-05-07 01:12:57.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk/const/status.py
--rw-rw-rw-   0        0        0     1194 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk/const/type_map.py
-drwxrwxrwx   0        0        0        0 2024-05-07 02:05:27.097022 duwi_smart_sdk-0.0.6/duwi_smart_sdk/model/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 02:05:27.098969 duwi_smart_sdk-0.0.6/duwi_smart_sdk/model/req/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk/model/req/__init__.py
--rw-rw-rw-   0        0        0     1584 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk/model/req/device_control.py
-drwxrwxrwx   0        0        0        0 2024-05-07 02:05:27.104844 duwi_smart_sdk-0.0.6/duwi_smart_sdk/model/resp/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk/model/resp/__init__.py
--rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk/model/resp/auth.py
--rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk/model/resp/control.py
--rw-rw-rw-   0        0        0     2767 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk/model/resp/device.py
--rw-rw-rw-   0        0        0     1113 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk/model/resp/house.py
-drwxrwxrwx   0        0        0        0 2024-05-07 02:05:27.108744 duwi_smart_sdk-0.0.6/duwi_smart_sdk/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk/util/__init__.py
--rw-rw-rw-   0        0        0     1926 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk/util/http.py
--rw-rw-rw-   0        0        0      906 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk/util/sign.py
--rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk/util/timestamp.py
-drwxrwxrwx   0        0        0        0 2024-05-07 02:05:27.082364 duwi_smart_sdk-0.0.6/duwi_smart_sdk.egg-info/
--rw-rw-rw-   0        0        0      628 2024-05-07 02:05:26.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1087 2024-05-07 02:05:27.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 02:05:26.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-07 02:05:26.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-07 02:05:26.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-07 02:05:26.000000 duwi_smart_sdk-0.0.6/duwi_smart_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 02:05:27.113631 duwi_smart_sdk-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      908 2024-05-07 02:05:21.000000 duwi_smart_sdk-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 02:05:27.109721 duwi_smart_sdk-0.0.6/test/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.6/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 02:05:27.111675 duwi_smart_sdk-0.0.6/test/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.6/test/util/__init__.py
--rw-rw-rw-   0        0        0     1192 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.6/test/util/test_http.py
+drwxrwxrwx   0        0        0        0 2024-05-07 02:10:05.252071 duwi_smart_sdk-0.0.7/
+-rw-rw-rw-   0        0        0      628 2024-05-07 02:10:05.252071 duwi_smart_sdk-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      145 2024-05-07 01:14:28.000000 duwi_smart_sdk-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 02:10:05.206307 duwi_smart_sdk-0.0.7/duwi_smart_sdk/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 02:10:05.222772 duwi_smart_sdk-0.0.7/duwi_smart_sdk/api/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk/api/__init__.py
+-rw-rw-rw-   0        0        0     1361 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk/api/control.py
+-rw-rw-rw-   0        0        0     2597 2024-05-07 01:23:47.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk/api/discover.py
+-rw-rw-rw-   0        0        0     2188 2024-05-07 01:23:47.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk/api/house.py
+-rw-rw-rw-   0        0        0     1723 2024-05-07 01:23:47.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk/api/login.py
+-rw-rw-rw-   0        0        0     1534 2024-05-07 01:23:50.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk/api/refresh_token.py
+-rw-rw-rw-   0        0        0     4306 2024-05-07 02:09:52.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk/api/ws.py
+drwxrwxrwx   0        0        0        0 2024-05-07 02:10:05.227664 duwi_smart_sdk-0.0.7/duwi_smart_sdk/const/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk/const/__init__.py
+-rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk/const/const.py
+-rw-rw-rw-   0        0        0      279 2024-05-07 01:12:57.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk/const/status.py
+-rw-rw-rw-   0        0        0     1194 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk/const/type_map.py
+drwxrwxrwx   0        0        0        0 2024-05-07 02:10:05.228636 duwi_smart_sdk-0.0.7/duwi_smart_sdk/model/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 02:10:05.231565 duwi_smart_sdk-0.0.7/duwi_smart_sdk/model/req/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk/model/req/__init__.py
+-rw-rw-rw-   0        0        0     1584 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk/model/req/device_control.py
+drwxrwxrwx   0        0        0        0 2024-05-07 02:10:05.238402 duwi_smart_sdk-0.0.7/duwi_smart_sdk/model/resp/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk/model/resp/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk/model/resp/auth.py
+-rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk/model/resp/control.py
+-rw-rw-rw-   0        0        0     2767 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk/model/resp/device.py
+-rw-rw-rw-   0        0        0     1113 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk/model/resp/house.py
+drwxrwxrwx   0        0        0        0 2024-05-07 02:10:05.244261 duwi_smart_sdk-0.0.7/duwi_smart_sdk/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk/util/__init__.py
+-rw-rw-rw-   0        0        0     1926 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk/util/http.py
+-rw-rw-rw-   0        0        0      906 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk/util/sign.py
+-rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk/util/timestamp.py
+drwxrwxrwx   0        0        0        0 2024-05-07 02:10:05.213768 duwi_smart_sdk-0.0.7/duwi_smart_sdk.egg-info/
+-rw-rw-rw-   0        0        0      628 2024-05-07 02:10:05.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1087 2024-05-07 02:10:05.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 02:10:05.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-07 02:10:05.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-07 02:10:05.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-07 02:10:05.000000 duwi_smart_sdk-0.0.7/duwi_smart_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 02:10:05.253049 duwi_smart_sdk-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      908 2024-05-07 02:10:01.000000 duwi_smart_sdk-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 02:10:05.246213 duwi_smart_sdk-0.0.7/test/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.7/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 02:10:05.250117 duwi_smart_sdk-0.0.7/test/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.7/test/util/__init__.py
+-rw-rw-rw-   0        0        0     1192 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.7/test/util/test_http.py
```

### Comparing `duwi_smart_sdk-0.0.6/PKG-INFO` & `duwi_smart_sdk-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smart_sdk
-Version: 0.0.6
+Version: 0.0.7
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smart_sdk-0.0.6/duwi_smart_sdk/api/control.py` & `duwi_smart_sdk-0.0.7/duwi_smart_sdk/api/control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.6/duwi_smart_sdk/api/discover.py` & `duwi_smart_sdk-0.0.7/duwi_smart_sdk/api/discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.6/duwi_smart_sdk/api/house.py` & `duwi_smart_sdk-0.0.7/duwi_smart_sdk/api/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.6/duwi_smart_sdk/api/login.py` & `duwi_smart_sdk-0.0.7/duwi_smart_sdk/api/login.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.6/duwi_smart_sdk/api/refresh_token.py` & `duwi_smart_sdk-0.0.7/duwi_smart_sdk/api/refresh_token.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.6/duwi_smart_sdk/api/ws.py` & `duwi_smart_sdk-0.0.7/duwi_smart_sdk/api/ws.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,16 @@
             await self._connection.send(message)
 
     async def disconnect(self):
         if self._connection:
             await self._connection.close()
 
     async def reconnect(self):
+        if self._is_over:
+            return
         _LOGGER.info("ws reconnect --------------")
         await self.connect()
         await self.link()
         await self.bind()
 
     async def listen(self):
         while True:
```

### Comparing `duwi_smart_sdk-0.0.6/duwi_smart_sdk/const/type_map.py` & `duwi_smart_sdk-0.0.7/duwi_smart_sdk/const/type_map.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.6/duwi_smart_sdk/model/req/device_control.py` & `duwi_smart_sdk-0.0.7/duwi_smart_sdk/model/req/device_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.6/duwi_smart_sdk/model/resp/auth.py` & `duwi_smart_sdk-0.0.7/duwi_smart_sdk/model/resp/auth.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.6/duwi_smart_sdk/model/resp/device.py` & `duwi_smart_sdk-0.0.7/duwi_smart_sdk/model/resp/device.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.6/duwi_smart_sdk/model/resp/house.py` & `duwi_smart_sdk-0.0.7/duwi_smart_sdk/model/resp/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.6/duwi_smart_sdk/util/http.py` & `duwi_smart_sdk-0.0.7/duwi_smart_sdk/util/http.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.6/duwi_smart_sdk/util/sign.py` & `duwi_smart_sdk-0.0.7/duwi_smart_sdk/util/sign.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.6/duwi_smart_sdk.egg-info/PKG-INFO` & `duwi_smart_sdk-0.0.7/duwi_smart_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi-smart-sdk
-Version: 0.0.6
+Version: 0.0.7
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smart_sdk-0.0.6/duwi_smart_sdk.egg-info/SOURCES.txt` & `duwi_smart_sdk-0.0.7/duwi_smart_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.6/setup.py` & `duwi_smart_sdk-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'sdk for duwi third platform'
 
 setup(
     name="duwi_smart_sdk",
     version=VERSION,
     author="ledger",
     author_email="ledgerbiggg@gmail.com",
```

### Comparing `duwi_smart_sdk-0.0.6/test/util/test_http.py` & `duwi_smart_sdk-0.0.7/test/util/test_http.py`

 * *Files identical despite different names*

