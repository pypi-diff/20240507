# Comparing `tmp/exponent_server_sdk_async-2.1.4.tar.gz` & `tmp/exponent_server_sdk_async-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exponent_server_sdk_async-2.1.4.tar", last modified: Mon Apr 29 13:24:45 2024, max compression
+gzip compressed data, was "exponent_server_sdk_async-2.1.5.tar", last modified: Tue May  7 12:33:48 2024, max compression
```

## Comparing `exponent_server_sdk_async-2.1.4.tar` & `exponent_server_sdk_async-2.1.5.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1075 2024-04-29 10:49:11.229618 exponent_server_sdk_async-2.1.4/LICENSE
--rw-r--r--   0        0        0     2195 2024-04-29 13:20:17.696800 exponent_server_sdk_async-2.1.4/README.md
--rw-r--r--   0        0        0    15289 2024-04-29 13:17:59.314579 exponent_server_sdk_async-2.1.4/exponent_server_sdk_async/__init__.py
--rw-r--r--   0        0        0     1637 2024-04-29 13:18:42.022933 exponent_server_sdk_async-2.1.4/exponent_server_sdk_async/main.py
--rw-r--r--   0        0        0      724 2024-04-29 13:24:45.989581 exponent_server_sdk_async-2.1.4/pyproject.toml
--rw-r--r--   0        0        0     2806 1970-01-01 00:00:00.000000 exponent_server_sdk_async-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-04-29 10:49:11.229618 exponent_server_sdk_async-2.1.5/LICENSE
+-rw-r--r--   0        0        0     2195 2024-04-29 13:20:17.696800 exponent_server_sdk_async-2.1.5/README.md
+-rw-r--r--   0        0        0    15289 2024-04-29 13:17:59.314579 exponent_server_sdk_async-2.1.5/exponent_server_sdk_async/__init__.py
+-rw-r--r--   0        0        0    68833 2024-05-05 10:11:35.421426 exponent_server_sdk_async-2.1.5/exponent_server_sdk_async/debug.log
+-rw-r--r--   0        0        0     2044 2024-05-07 12:28:20.228450 exponent_server_sdk_async-2.1.5/exponent_server_sdk_async/main.py
+-rw-r--r--   0        0        0      666 2024-05-07 12:33:48.872338 exponent_server_sdk_async-2.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2724 1970-01-01 00:00:00.000000 exponent_server_sdk_async-2.1.5/PKG-INFO
```

### Comparing `exponent_server_sdk_async-2.1.4/LICENSE` & `exponent_server_sdk_async-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `exponent_server_sdk_async-2.1.4/README.md` & `exponent_server_sdk_async-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `exponent_server_sdk_async-2.1.4/exponent_server_sdk_async/__init__.py` & `exponent_server_sdk_async-2.1.5/exponent_server_sdk_async/__init__.py`

 * *Files identical despite different names*

### Comparing `exponent_server_sdk_async-2.1.4/exponent_server_sdk_async/main.py` & `exponent_server_sdk_async-2.1.5/exponent_server_sdk_async/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,64 @@
+import asyncio
 import os
 import httpx
-from httpx import HTTPError, NetworkError
 from loguru import logger
 from dotenv import load_dotenv
 from exponent_server_sdk_async import (
-    DeviceNotRegisteredError,
     AsyncPushClient,
     PushMessage,
-    PushServerError,
+    DeviceNotRegisteredError,
     PushTicketError,
+    PushServerError
 )
 
+# Logger setup
 logger.add("debug.log", rotation="1 week", compression="zip")
 load_dotenv()
 logger.debug("Using Expo Token: {}", os.getenv('EXPO_TOKEN'))
 
 
-async def send_push_message(token, message, extra=None):
+async def send_push_message(token, message, extra, title, navigate_to=None):
     async with httpx.AsyncClient(headers={
         "Authorization": f"Bearer {os.getenv('EXPO_TOKEN')}",
         "Accept": "application/json",
         "Content-Type": "application/json",
     }) as session:
+        push_client = AsyncPushClient(session=session)
+        push_message = PushMessage(
+            to=token,
+            body=message,
+            data={'extra': extra, 'navigateTo': navigate_to},
+            badge=1,
+            title=title,
+            sound="default"
+        )
         try:
-            response = await AsyncPushClient(session=session).publish(
-                PushMessage(to=token, body=message, data=extra, sound="default"))
-            response.validate_response()
+            push_ticket = await push_client.publish(push_message)
+            if push_ticket.is_success():
+                logger.info("Notification sent successfully to: {}", token)
+            else:
+                logger.warning("Failed to send notification to: {}, Error: {}", token, push_ticket.message)
         except PushServerError as exc:
             logger.error("Push server error: {}", exc)
             raise
-        except (NetworkError, HTTPError) as exc:
-            logger.error("Network or HTTP error: {}", exc)
+        except DeviceNotRegisteredError as exc:
+            logger.error("Device not registered error: {}", exc)
             raise
-        except DeviceNotRegisteredError:
-            logger.warning("Device not registered, deactivating token: {}", token)
-
         except PushTicketError as exc:
             logger.error("Push ticket error: {}", exc)
             raise
 
+
 async def main():
     token = "ExponentPushToken[TOKEN]"
-    message = "HI! This is a test message."
     extra_parameters = {"key": "value"}
-    await send_push_message(token, message, extra_parameters)
 
+    # Send a simple push message
+    await send_push_message(token, "Hello World", extra_parameters, "Hello World")
+
+    # Navigate to home data
+    await send_push_message(token, "Navigate to home", extra_parameters, "Home", "/(tabs)/(home)")
 
-if __name__ == "__main__":
-    import asyncio
 
+if __name__ == "__main__":
     asyncio.run(main())
```

### Comparing `exponent_server_sdk_async-2.1.4/PKG-INFO` & `exponent_server_sdk_async-2.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: exponent_server_sdk_async
-Version: 2.1.4
+Version: 2.1.5
 Summary: Expo Server SDK for Python async
 Author-Email: =?utf-8?q?Bahad=C4=B1r_Araz?= <bahadiraraz@protonmail.com>, Expo Team <exponent.team@gmail.com>
 License: MIT
-Project-URL: Homepage, https://github.com/expo/exponent-server-sdk-python
+Project-URL: Homepage, https://github.com/Learnity-AI/expo-server-sdk-python-async
 Requires-Python: >=3.12
 Requires-Dist: setuptools>=69.5.1
-Requires-Dist: requests
 Requires-Dist: six
 Requires-Dist: httpx>=0.27.0
-Requires-Dist: pytest>=8.2.0
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: python-dotenv>=1.0.1
-Requires-Dist: pytest-asyncio>=0.23.6
 Description-Content-Type: text/markdown
 
 # exponent-server-sdk-python-async
 
 This repo is made for the async version of the [exponent-server-sdk-python](https://github.com/expo-community/expo-server-sdk-python) made by [Bahadır Araz](https://github.com/bahadiraraz).
 
 ## Installation
```

