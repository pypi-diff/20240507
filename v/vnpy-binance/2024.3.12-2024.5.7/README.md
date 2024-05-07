# Comparing `tmp/vnpy_binance-2024.3.12.tar.gz` & `tmp/vnpy_binance-2024.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_binance-2024.3.12.tar", last modified: Tue Mar 12 05:20:25 2024, max compression
+gzip compressed data, was "vnpy_binance-2024.5.7.tar", last modified: Tue May  7 00:15:06 2024, max compression
```

## Comparing `vnpy_binance-2024.3.12.tar` & `vnpy_binance-2024.5.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-03-12 05:20:25.097965 vnpy_binance-2024.3.12/
--rw-rw-rw-   0        0        0     1101 2024-03-12 01:01:43.000000 vnpy_binance-2024.3.12/LICENSE
--rw-rw-rw-   0        0        0     3002 2024-03-12 05:20:25.097965 vnpy_binance-2024.3.12/PKG-INFO
--rw-rw-rw-   0        0        0     1985 2024-03-12 01:27:33.000000 vnpy_binance-2024.3.12/README.md
--rw-rw-rw-   0        0        0     1105 2024-03-12 05:20:25.099961 vnpy_binance-2024.3.12/setup.cfg
--rw-rw-rw-   0        0        0       43 2024-03-05 02:02:16.000000 vnpy_binance-2024.3.12/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-12 05:20:25.069853 vnpy_binance-2024.3.12/vnpy_binance/
--rw-rw-rw-   0        0        0     1374 2024-03-12 01:02:56.000000 vnpy_binance-2024.3.12/vnpy_binance/__init__.py
--rw-rw-rw-   0        0        0    34585 2024-03-12 00:45:24.000000 vnpy_binance-2024.3.12/vnpy_binance/binance_inverse_gateway.py
--rw-rw-rw-   0        0        0    34565 2024-03-12 00:57:56.000000 vnpy_binance-2024.3.12/vnpy_binance/binance_linear_gateway.py
--rw-rw-rw-   0        0        0    31572 2024-03-12 00:52:30.000000 vnpy_binance-2024.3.12/vnpy_binance/binance_spot_gateway.py
-drwxrwxrwx   0        0        0        0 2024-03-12 05:20:25.096955 vnpy_binance-2024.3.12/vnpy_binance.egg-info/
--rw-rw-rw-   0        0        0     3002 2024-03-12 05:20:24.000000 vnpy_binance-2024.3.12/vnpy_binance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2024-03-12 05:20:25.000000 vnpy_binance-2024.3.12/vnpy_binance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-12 05:20:24.000000 vnpy_binance-2024.3.12/vnpy_binance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-05 02:30:31.000000 vnpy_binance-2024.3.12/vnpy_binance.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2024-03-12 05:20:24.000000 vnpy_binance-2024.3.12/vnpy_binance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-03-12 05:20:24.000000 vnpy_binance-2024.3.12/vnpy_binance.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 00:15:06.652527 vnpy_binance-2024.5.7/
+-rw-rw-rw-   0        0        0     1101 2024-03-12 01:01:43.000000 vnpy_binance-2024.5.7/LICENSE
+-rw-rw-rw-   0        0        0     3000 2024-05-07 00:15:06.652527 vnpy_binance-2024.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1984 2024-05-07 00:12:49.000000 vnpy_binance-2024.5.7/README.md
+-rw-rw-rw-   0        0        0     1105 2024-05-07 00:15:06.653532 vnpy_binance-2024.5.7/setup.cfg
+-rw-rw-rw-   0        0        0       43 2024-03-05 02:02:16.000000 vnpy_binance-2024.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 00:15:06.627507 vnpy_binance-2024.5.7/vnpy_binance/
+-rw-rw-rw-   0        0        0     1373 2024-05-07 00:12:56.000000 vnpy_binance-2024.5.7/vnpy_binance/__init__.py
+-rw-rw-rw-   0        0        0    35060 2024-05-07 00:09:45.000000 vnpy_binance-2024.5.7/vnpy_binance/binance_inverse_gateway.py
+-rw-rw-rw-   0        0        0    35040 2024-05-07 00:09:27.000000 vnpy_binance-2024.5.7/vnpy_binance/binance_linear_gateway.py
+-rw-rw-rw-   0        0        0    32044 2024-05-07 00:11:16.000000 vnpy_binance-2024.5.7/vnpy_binance/binance_spot_gateway.py
+drwxrwxrwx   0        0        0        0 2024-05-07 00:15:06.651553 vnpy_binance-2024.5.7/vnpy_binance.egg-info/
+-rw-rw-rw-   0        0        0     3000 2024-05-07 00:15:06.000000 vnpy_binance-2024.5.7/vnpy_binance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2024-05-07 00:15:06.000000 vnpy_binance-2024.5.7/vnpy_binance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 00:15:06.000000 vnpy_binance-2024.5.7/vnpy_binance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-03-05 02:30:31.000000 vnpy_binance-2024.5.7/vnpy_binance.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2024-05-07 00:15:06.000000 vnpy_binance-2024.5.7/vnpy_binance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-07 00:15:06.000000 vnpy_binance-2024.5.7/vnpy_binance.egg-info/top_level.txt
```

### Comparing `vnpy_binance-2024.3.12/LICENSE` & `vnpy_binance-2024.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_binance-2024.3.12/PKG-INFO` & `vnpy_binance-2024.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy_binance
-Version: 2024.3.12
+Version: 2024.5.7
 Summary: BINANCE trading gateway for VeighNa Evo.
 Home-page: https://www.github.com/veighna-global
 Author: VeighNa Global
 Author-email: veighna@hotmail.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading,binance,btc,crypto
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,15 +25,15 @@
 # Binance trading gateway for VeighNa Evo
 
 <p align="center">
   <img src ="https://github.com/veighna-global/vnpy_evo/blob/dev/logo.png" width="300" height="300"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-2024.3.12-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-2024.5.7-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg"/>
     <img src ="https://img.shields.io/github/license/veighna-global/vnpy_evo.svg?color=orange"/>
 </p>
 
 
 ## Introduction
```

### Comparing `vnpy_binance-2024.3.12/README.md` & `vnpy_binance-2024.5.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Binance trading gateway for VeighNa Evo
 
 <p align="center">
   <img src ="https://github.com/veighna-global/vnpy_evo/blob/dev/logo.png" width="300" height="300"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-2024.3.12-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-2024.5.7-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg"/>
     <img src ="https://img.shields.io/github/license/veighna-global/vnpy_evo.svg?color=orange"/>
 </p>
 
 
 ## Introduction
```

### Comparing `vnpy_binance-2024.3.12/setup.cfg` & `vnpy_binance-2024.5.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `vnpy_binance-2024.3.12/vnpy_binance/__init__.py` & `vnpy_binance-2024.5.7/vnpy_binance/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 # SOFTWARE.
 
 from .binance_spot_gateway import BinanceSpotGateway
 from .binance_linear_gateway import BinanceLinearGateway, BinanceUsdtGateway
 from .binance_inverse_gateway import BinanceInverseGateway
 
 
-__version__ = "2024.3.12"
+__version__ = "2024.5.7"
```

### Comparing `vnpy_binance-2024.3.12/vnpy_binance/binance_inverse_gateway.py` & `vnpy_binance-2024.5.7/vnpy_binance/binance_inverse_gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from copy import copy
 from datetime import datetime, timedelta
 from enum import Enum
 from time import sleep
 from asyncio import run_coroutine_threadsafe
 
 from aiohttp import ClientSSLError
+from numpy import format_float_positional
 
 from vnpy_evo.event import Event, EventEngine
 from vnpy_evo.trader.constant import (
     Direction,
     Exchange,
     Product,
     Status,
@@ -303,20 +304,14 @@
         self.start()
 
         self.gateway.write_log("REST API started")
 
         self.query_time()
         self.query_contract()
 
-        if key and secret:
-            self.query_account()
-            self.query_position()
-            self.query_order()
-            self.start_user_stream()
-
     def query_time(self) -> None:
         """Query server time"""
         data: dict = {"security": Security.NONE}
 
         path: str = "/dapi/v1/time"
 
         return self.add_request(
@@ -393,28 +388,28 @@
 
         # Create order parameters
         data: dict = {"security": Security.SIGNED}
 
         params: dict = {
             "symbol": req.symbol,
             "side": DIRECTION_VT2BINANCES[req.direction],
-            "quantity": float(req.volume),
+            "quantity": format_float(req.volume),
             "newClientOrderId": orderid,
         }
 
         if req.type == OrderType.MARKET:
             params["type"] = "MARKET"
         elif req.type == OrderType.STOP:
             params["type"] = "STOP_MARKET"
-            params["stopPrice"] = float(req.price)
+            params["stopPrice"] = format_float(req.price)
         else:
             order_type, time_condition = ORDERTYPE_VT2BINANCES[req.type]
             params["type"] = order_type
             params["timeInForce"] = time_condition
-            params["price"] = float(req.price)
+            params["price"] = format_float(req.price)
 
         path: str = "/dapi/v1/order"
 
         self.add_request(
             method="POST",
             path=path,
             callback=self.on_send_order,
@@ -489,14 +484,23 @@
 
     def on_query_time(self, data: dict, request: Request) -> None:
         """Callback of server time query"""
         local_time: int = int(time.time() * 1000)
         server_time: int = int(data["serverTime"])
         self.time_offset: int = local_time - server_time
 
+        self.gateway.write_log(f"Server time updated, local offset: {self.time_offset}ms")
+
+        # Query private data after time offset is calculated
+        if self.key and self.secret:
+            self.query_account()
+            self.query_position()
+            self.query_order()
+            self.start_user_stream()
+
     def on_query_account(self, data: dict, request: Request) -> None:
         """Callback of account balance query"""
         for asset in data["assets"]:
             account: AccountData = AccountData(
                 accountid=asset["asset"],
                 balance=float(asset["walletBalance"]),
                 frozen=float(asset["maintMargin"]),
@@ -1027,7 +1031,16 @@
 
 
 def generate_datetime(timestamp: float) -> datetime:
     """Generate datetime object from Binance timestamp"""
     dt: datetime = datetime.fromtimestamp(timestamp / 1000)
     dt: datetime = dt.replace(tzinfo=UTC_TZ)
     return dt
+
+
+def format_float(f: float) -> str:
+    """
+    Convert float number to string with correct precision.
+
+    Fix potential error -1111: Parameter 'quantity' has too much precision
+    """
+    return format_float_positional(f, trim='-')
```

### Comparing `vnpy_binance-2024.3.12/vnpy_binance/binance_linear_gateway.py` & `vnpy_binance-2024.5.7/vnpy_binance/binance_linear_gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from copy import copy
 from enum import Enum
 from time import sleep
 from datetime import datetime, timedelta
 from asyncio import run_coroutine_threadsafe
 
 from aiohttp import ClientSSLError
+from numpy import format_float_positional
 
 from vnpy_evo.event import Event, EventEngine
 from vnpy_evo.trader.constant import (
     Direction,
     Exchange,
     Product,
     Status,
@@ -303,20 +304,14 @@
         self.start()
 
         self.gateway.write_log("REST API started")
 
         self.query_time()
         self.query_contract()
 
-        if key and secret:
-            self.query_account()
-            self.query_position()
-            self.query_order()
-            self.start_user_stream()
-
     def query_time(self) -> None:
         """Query server time"""
         data: dict = {"security": Security.NONE}
 
         path: str = "/fapi/v1/time"
 
         self.add_request(
@@ -393,28 +388,28 @@
 
         # Create order parameters
         data: dict = {"security": Security.SIGNED}
 
         params: dict = {
             "symbol": req.symbol,
             "side": DIRECTION_VT2BINANCES[req.direction],
-            "quantity": float(req.volume),
+            "quantity": format_float(req.volume),
             "newClientOrderId": orderid,
         }
 
         if req.type == OrderType.MARKET:
             params["type"] = "MARKET"
         elif req.type == OrderType.STOP:
             params["type"] = "STOP_MARKET"
-            params["stopPrice"] = float(req.price)
+            params["stopPrice"] = format_float(req.price)
         else:
             order_type, time_condition = ORDERTYPE_VT2BINANCES[req.type]
             params["type"] = order_type
             params["timeInForce"] = time_condition
-            params["price"] = float(req.price)
+            params["price"] = format_float(req.price)
 
         path: str = "/fapi/v1/order"
 
         self.add_request(
             method="POST",
             path=path,
             callback=self.on_send_order,
@@ -487,14 +482,23 @@
 
     def on_query_time(self, data: dict, request: Request) -> None:
         """Callback of server time query"""
         local_time: int = int(time.time() * 1000)
         server_time: int = int(data["serverTime"])
         self.time_offset: int = local_time - server_time
 
+        self.gateway.write_log(f"Server time updated, local offset: {self.time_offset}ms")
+
+        # Query private data after time offset is calculated
+        if self.key and self.secret:
+            self.query_account()
+            self.query_position()
+            self.query_order()
+            self.start_user_stream()
+
     def on_query_account(self, data: dict, request: Request) -> None:
         """Callback of account balance query"""
         for asset in data["assets"]:
             account: AccountData = AccountData(
                 accountid=asset["asset"],
                 balance=float(asset["walletBalance"]),
                 frozen=float(asset["maintMargin"]),
@@ -1023,11 +1027,20 @@
 def generate_datetime(timestamp: float) -> datetime:
     """Generate datetime object from Binance timestamp"""
     dt: datetime = datetime.fromtimestamp(timestamp / 1000)
     dt: datetime = dt.replace(tzinfo=UTC_TZ)
     return dt
 
 
+def format_float(f: float) -> str:
+    """
+    Convert float number to string with correct precision.
+
+    Fix potential error -1111: Parameter 'quantity' has too much precision
+    """
+    return format_float_positional(f, trim='-')
+
+
 class BinanceUsdtGateway(BinanceLinearGateway):
     """Compatibility interface for the old BinanceUsdtGateway"""
 
     default_name: str = "BINANCE_USDT"
```

### Comparing `vnpy_binance-2024.3.12/vnpy_binance/binance_spot_gateway.py` & `vnpy_binance-2024.5.7/vnpy_binance/binance_spot_gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from datetime import datetime, timedelta
 from enum import Enum
 from asyncio import run_coroutine_threadsafe
 from zoneinfo import ZoneInfo
 from time import sleep
 
 from aiohttp import ClientSSLError
+from numpy import format_float_positional
 
 from vnpy_evo.event import Event, EventEngine
 from vnpy_evo.trader.constant import (
     Direction,
     Exchange,
     Product,
     Status,
@@ -299,19 +300,14 @@
         self.start()
 
         self.gateway.write_log("REST API started")
 
         self.query_time()
         self.query_contract()
 
-        if key and secret:
-            self.query_account()
-            self.query_order()
-            self.start_user_stream()
-
     def query_time(self) -> None:
         """Query server time"""
         data: dict = {"security": Security.NONE}
 
         path: str = "/api/v3/time"
 
         return self.add_request(
@@ -370,25 +366,25 @@
         # Create order parameters
         data: dict = {"security": Security.SIGNED}
 
         params: dict = {
             "symbol": req.symbol.upper(),
             "side": DIRECTION_VT2BINANCE[req.direction],
             "type": ORDERTYPE_VT2BINANCE[req.type],
-            "quantity": format(req.volume, "f"),
+            "quantity": format_float(req.volume),
             "newClientOrderId": orderid,
             "newOrderRespType": "ACK"
         }
 
         if req.type == OrderType.LIMIT:
             params["timeInForce"] = "GTC"
-            params["price"] = str(req.price)
+            params["price"] = format_float(req.price)
         elif req.type == OrderType.STOP:
             params["type"] = "STOP_LOSS"
-            params["stopPrice"] = float(req.price)
+            params["stopPrice"] = format_float(req.price)
 
         self.add_request(
             method="POST",
             path="/api/v3/order",
             callback=self.on_send_order,
             data=data,
             params=params,
@@ -453,14 +449,22 @@
 
     def on_query_time(self, data: dict, request: Request) -> None:
         """Callback of server time query"""
         local_time = int(time.time() * 1000)
         server_time = int(data["serverTime"])
         self.time_offset = local_time - server_time
 
+        self.gateway.write_log(f"Server time updated, local offset: {self.time_offset}ms")
+
+        # Query private data after time offset is calculated
+        if self.key and self.secret:
+            self.query_account()
+            self.query_order()
+            self.start_user_stream()
+
     def on_query_account(self, data: dict, request: Request) -> None:
         """Callback of account balance query"""
         for account_data in data["balances"]:
             account: AccountData = AccountData(
                 accountid=account_data["asset"],
                 balance=float(account_data["free"]) + float(account_data["locked"]),
                 frozen=float(account_data["locked"]),
@@ -558,15 +562,15 @@
     def on_cancel_failed(self, status_code: str, request: Request) -> None:
         """Failed callback of cancel_order"""
         if request.extra:
             order = request.extra
             order.status = Status.REJECTED
             self.gateway.on_order(order)
 
-        msg = f"Cancel orde failed, status code: {status_code}, message: {request.response.text}, order: {request.extra} "
+        msg = f"Cancel order failed, status code: {status_code}, message: {request.response.text}, order: {request.extra} "
         self.gateway.write_log(msg)
 
     def on_start_user_stream(self, data: dict, request: Request) -> None:
         """Successful callback of start_user_stream"""
         self.user_stream_key = data["listenKey"]
         self.keep_alive_count = 0
 
@@ -941,7 +945,16 @@
 
 
 def generate_datetime(timestamp: float) -> datetime:
     """Generate datetime object from Binance timestamp"""
     dt: datetime = datetime.fromtimestamp(timestamp / 1000)
     dt: datetime = dt.replace(tzinfo=UTC_TZ)
     return dt
+
+
+def format_float(f: float) -> str:
+    """
+    Convert float number to string with correct precision.
+
+    Fix potential error -1111: Parameter 'quantity' has too much precision
+    """
+    return format_float_positional(f, trim='-')
```

### Comparing `vnpy_binance-2024.3.12/vnpy_binance.egg-info/PKG-INFO` & `vnpy_binance-2024.5.7/vnpy_binance.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy-binance
-Version: 2024.3.12
+Version: 2024.5.7
 Summary: BINANCE trading gateway for VeighNa Evo.
 Home-page: https://www.github.com/veighna-global
 Author: VeighNa Global
 Author-email: veighna@hotmail.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading,binance,btc,crypto
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,15 +25,15 @@
 # Binance trading gateway for VeighNa Evo
 
 <p align="center">
   <img src ="https://github.com/veighna-global/vnpy_evo/blob/dev/logo.png" width="300" height="300"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-2024.3.12-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-2024.5.7-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg"/>
     <img src ="https://img.shields.io/github/license/veighna-global/vnpy_evo.svg?color=orange"/>
 </p>
 
 
 ## Introduction
```

