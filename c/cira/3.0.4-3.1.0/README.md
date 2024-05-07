# Comparing `tmp/cira-3.0.4.tar.gz` & `tmp/cira-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cira-3.0.4.tar", last modified: Sun Mar 24 16:48:07 2024, max compression
+gzip compressed data, was "cira-3.1.0.tar", last modified: Tue May  7 08:43:45 2024, max compression
```

## Comparing `cira-3.0.4.tar` & `cira-3.1.0.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:48:07.863239 cira-3.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-24 16:47:52.000000 cira-3.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-24 16:47:52.000000 cira-3.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-03-24 16:48:07.863239 cira-3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-03-24 16:47:52.000000 cira-3.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:48:07.859239 cira-3.0.4/cira/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-24 16:47:52.000000 cira-3.0.4/cira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-24 16:47:52.000000 cira-3.0.4/cira/alpaca_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11771 2024-03-24 16:47:52.000000 cira-3.0.4/cira/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-03-24 16:47:52.000000 cira-3.0.4/cira/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-24 16:47:52.000000 cira-3.0.4/cira/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-03-24 16:47:52.000000 cira-3.0.4/cira/exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-24 16:47:52.000000 cira-3.0.4/cira/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-03-24 16:47:52.000000 cira-3.0.4/cira/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-03-24 16:47:52.000000 cira-3.0.4/cira/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-24 16:47:52.000000 cira-3.0.4/cira/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:48:07.863239 cira-3.0.4/cira.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-03-24 16:48:07.000000 cira-3.0.4/cira.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-24 16:48:07.000000 cira-3.0.4/cira.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 16:48:07.000000 cira-3.0.4/cira.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-24 16:48:07.000000 cira-3.0.4/cira.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-24 16:48:07.000000 cira-3.0.4/cira.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 16:48:07.863239 cira-3.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-24 16:47:52.000000 cira-3.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:43:45.469777 cira-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-07 08:43:27.000000 cira-3.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 08:43:27.000000 cira-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-05-07 08:43:45.469777 cira-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-07 08:43:27.000000 cira-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:43:45.465777 cira-3.1.0/cira/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-07 08:43:27.000000 cira-3.1.0/cira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-07 08:43:27.000000 cira-3.1.0/cira/alpaca_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10627 2024-05-07 08:43:27.000000 cira-3.1.0/cira/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-07 08:43:27.000000 cira-3.1.0/cira/asset_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-07 08:43:27.000000 cira-3.1.0/cira/asset_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-05-07 08:43:27.000000 cira-3.1.0/cira/assset_cryptocurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-07 08:43:27.000000 cira-3.1.0/cira/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-07 08:43:27.000000 cira-3.1.0/cira/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-07 08:43:27.000000 cira-3.1.0/cira/exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-07 08:43:27.000000 cira-3.1.0/cira/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-05-07 08:43:27.000000 cira-3.1.0/cira/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-07 08:43:27.000000 cira-3.1.0/cira/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-07 08:43:27.000000 cira-3.1.0/cira/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:43:45.469777 cira-3.1.0/cira.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-05-07 08:43:45.000000 cira-3.1.0/cira.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-07 08:43:45.000000 cira-3.1.0/cira.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 08:43:45.000000 cira-3.1.0/cira.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-07 08:43:45.000000 cira-3.1.0/cira.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 08:43:45.000000 cira-3.1.0/cira.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 08:43:45.469777 cira-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-07 08:43:27.000000 cira-3.1.0/setup.py
```

### Comparing `cira-3.0.4/LICENSE.txt` & `cira-3.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cira-3.0.4/PKG-INFO` & `cira-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cira
-Version: 3.0.4
+Version: 3.1.0
 Summary: A simpler library for the alapaca trade api
 Home-page: https://github.com/AxelGard/cira
 Author: Axel Gard
 Author-email: axel.gard@tutanota.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Office/Business :: Financial
```

### Comparing `cira-3.0.4/README.md` & `cira-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cira-3.0.4/cira/asset.py` & `cira-3.1.0/cira/asset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,82 +1,68 @@
 from typing import List
 from datetime import datetime
 import logging
 import warnings
+
+# Alpaca
 import alpaca
-from alpaca.data import CryptoHistoricalDataClient, StockHistoricalDataClient
-from alpaca.data.requests import StockLatestQuoteRequest
-from alpaca.data.requests import CryptoLatestQuoteRequest
-from alpaca.data.requests import CryptoBarsRequest, StockBarsRequest
+from alpaca.trading.requests import GetAssetsRequest
+from alpaca.trading.enums import AssetClass, OrderType, AssetStatus
+from alpaca.data.models import Bar
+from alpaca.trading.enums import OrderSide, TimeInForce
 from alpaca.data.timeframe import TimeFrame
+from alpaca.trading.requests import LimitOrderRequest, StopLimitOrderRequest
+from alpaca.trading.client import TradingClient
+
+# stock
+from alpaca.data import StockHistoricalDataClient
+from alpaca.data.requests import StockLatestQuoteRequest
+from alpaca.data.requests import StockBarsRequest
 from alpaca.trading.requests import MarketOrderRequest
-from alpaca.trading.enums import OrderSide, TimeInForce
 from alpaca.data.live import StockDataStream
-from alpaca.trading.client import TradingClient
-from alpaca.trading.requests import LimitOrderRequest
-from alpaca.data.models import Bar
+
+# crypto
+from alpaca.data import CryptoHistoricalDataClient
+from alpaca.data.live.crypto import CryptoDataStream
+from alpaca.data.requests import CryptoLatestQuoteRequest
+from alpaca.data.requests import CryptoBarsRequest
 
 import pandas as pd
 
 from . import auth
 from . import config
 from . import util
 from . import log
 
 
 class Asset:
     def __init__(self, symbol: str) -> None:
         """Interface class"""
         self.symbol = symbol
-
-    def historical_data_df(
-        self, start_date: datetime, end_date: datetime
-    ) -> pd.DataFrame:
-        raise NotImplementedError
+        self.live_client: StockDataStream = None
+        self.history: StockHistoricalDataClient = None
+        self.trade: TradingClient = None
+        self.latest_quote_request: StockLatestQuoteRequest = None
+        self.bars_request: StockBarsRequest = None
 
     def price(self) -> float:
         raise NotImplementedError
 
-    def __str__(self) -> str:
-        return self.symbol
-
-    def __repr__(self) -> str:
-        return self.symbol
-
-    def __eq__(self, other):
-        if not isinstance(other, Asset):
-            raise ValueError
-        return self.symbol == other.symbol
-
-    def __ne__(self, other):
-        return not self.__eq__(other)
-
-
-class Stock(Asset):
-    def __init__(self, symbol: str) -> None:
-        """Exchange for trading stocks"""
-        APCA_ID, APCA_SECRET = auth.get_api_keys()
-        self.live_client = StockDataStream(APCA_ID, APCA_SECRET)
-        self.history = StockHistoricalDataClient(APCA_ID, APCA_SECRET)
-        self.trade = TradingClient(APCA_ID, APCA_SECRET, paper=config.PAPER_TRADING)
-        self.symbol = symbol
-
-    def price(self) -> float:
-        """gets the asking price of the symbol"""
-        perms = StockLatestQuoteRequest(symbol_or_symbols=self.symbol)
-        return float(self.history.get_stock_latest_quote(perms)[self.symbol].ask_price)
+    @classmethod
+    def get_all_assets(self):
+        raise NotImplementedError
 
     def live_data(self, async_function_to_resolve_to, run: bool = True) -> None:
         self.live_client.subscribe_quotes(async_function_to_resolve_to, self.symbol)
         if run:
             self.live_client.run()
 
     def _get_bars(self, start_date: datetime, end_date: datetime):
         """returns aplc bars from the given dates"""
-        params = StockBarsRequest(
+        params = self.bars_request(
             symbol_or_symbols=self.symbol,
             timeframe=TimeFrame.Day,
             start=start_date,
             end=end_date,
             adjustment="all",
         )
         return self.history.get_stock_bars(params)
@@ -124,36 +110,39 @@
 
     def buy_at(self, qty: int, price: float) -> None:
         """Buy the asset at a given price,
         qty is the number of the asset that you buy"""
         limit_order_data = LimitOrderRequest(
             symbol=self.symbol,
             limit_price=price,
-            notional=qty,
+            qty=qty,
             side=OrderSide.BUY,
             time_in_force=TimeInForce.FOK,
         )
         if config.IS_LOGGING:
             log.log("BUY", self.symbol, qty)
         self.trade.submit_order(order_data=limit_order_data)
 
     def sell_at(self, qty: int, price: float) -> None:
         """Sell the asset at a given price,
         qty is the number of the asset that you sell"""
         limit_order_data = LimitOrderRequest(
             symbol=self.symbol,
             limit_price=price,
-            notional=qty,
+            qty=qty,
             side=OrderSide.SELL,
             time_in_force=TimeInForce.FOK,
         )
         if config.IS_LOGGING:
             log.log("SELL", self.symbol, qty)
         self.trade.submit_order(order_data=limit_order_data)
 
+    def cancel_orders(self):
+        return self.trade.cancel_orders()
+
     def save_historical_data(
         self, file_path, start_date: datetime, end_date: datetime
     ) -> None:
         data = self.historical_data_df(start_date=start_date, end_date=end_date)
         data.to_csv(file_path)
 
     @classmethod
@@ -166,15 +155,15 @@
         """
         data = pd.read_csv(file_path)
         data["timestamp"] = pd.to_datetime(data["timestamp"])
         data.set_index("timestamp", inplace=True)
         return data
 
     def value(self) -> float:  # prev: value_of_stock
-        """takes a string sym. Gets and returns the stock value at close"""
+        """takes a string sym. Gets and returns the asset value at close"""
 
         warnings.warn(f"Warning: function is deprecated ({self.value})")
 
         nr_days = 1
         bars = self.barset(nr_days)
         if bars is None:
             self._value = 0.0
@@ -193,119 +182,119 @@
             )
         order = auth.api().submit_order(
             symbol=self.symbol, qty=qty, side=beh, type="market", time_in_force="gtc"
         )
         return order
 
     def is_sortable(self) -> bool:
-        """checks if stock can be shorted"""
+        """checks if asset can be shorted"""
         return bool(auth.api().get_asset(self.symbol).shortable)
 
     def can_borrow(self) -> bool:
         """check whether the name is currently
         available to short at Alpaca"""
         return auth.api().get_asset(self.symbol).easy_to_borrow
 
     def barset(self, limit: int):
-        """returns barset for stock for time period lim"""
+        """returns barset for asset for time period lim"""
         return alpaca.api().get_bars(self.symbol, TimeFrame.Minute, limit=int(limit))
 
     def is_tradable(self) -> bool:
-        """return if the stock can be traded"""
+        """return if the asset can be traded"""
         return bool(auth.api().get_asset(self.symbol).tradable)
 
     def position(self):
-        """returns position of stock"""
+        """returns position of asset"""
 
         warnings.warn(f"Warning: function is deprecated ({self.position})")
 
         pos = auth.api().get_position(self.symbol)
         self._position = util.reformat_position(pos)
         return self._position
 
     def today_plpc(self) -> float:
-        """stock today's profit/loss percent"""
+        """asset today's profit/loss percent"""
         self._today_plpc = self.position()["unrealized_intraday_plpc"]
         return self._today_plpc
 
     def plpc(self) -> float:
-        """stock sym (str) Unrealized profit/loss percentage"""
+        """asset sym (str) Unrealized profit/loss percentage"""
         self._plpc = self.position()["unrealized_plpc"]
         return self._plpc
 
     # Operators
 
     def __eq__(self, other):
         if isinstance(other, (int, float)):
             return self.price() == other
-        return self.price() == other.price
+        return self.price() == other.price()
 
     def __ne__(self, other):
         if isinstance(other, (int, float)):
             return self.price() != other
-        return self.price() != other.price
+        return self.price() != other.price()
 
     def __lt__(self, other):
         if isinstance(other, (int, float)):
             return self.price() < other
-        return self.price() < other.price
+        return self.price() < other.price()
 
     def __le__(self, other):
         if isinstance(other, (int, float)):
             return self.price() <= other
-        return self.price() <= other.price
+        return self.price() <= other.price()
 
     def __gt__(self, other):
         if isinstance(other, (int, float)):
             return self.price() > other
-        return self.price() > other.price
+        return self.price() > other.price()
 
     def __ge__(self, other):
         if isinstance(other, (int, float)):
             return self.price() >= other
-        return self.price() >= other.price
+        return self.price() >= other.price()
 
     # Arithmetic Operators
 
     def __add__(self, other):
         if isinstance(other, (int, float)):
             return self.price() + other
-        return self.price() + other.price
+        return self.price() + other.price()
 
     def __radd__(self, other):
         return self.price() + other
 
     def __sub__(self, other):
         if isinstance(other, (int, float)):
             return self.price() - other
-        return self.price() - other.price
+        return self.price() - other.price()
 
     def __rsub__(self, other):
         return self.price() - other
 
     def __mul__(self, other):
         if isinstance(other, (int, float)):
             return self.price() * other
-        return self.price() * other.price
+        return self.price() * other.price()
 
     def __rmul__(self, other):
         return self.price() * other
 
     def __truediv__(self, other):
         if isinstance(other, (int, float)):
             return self.price() / other
-        return self.price() / other.price
+        return self.price() / other.price()
 
     def __rdiv__(self, other):
         return self.price() / other
 
     def __floordiv__(self, other):
         if isinstance(other, (int, float)):
             return self.price() // other
-        return self.price() // other.price
+        return self.price() // other.price()
 
     def __rfloordiv__(self, other):
         return self.price() // other
 
     # Type Conversion
 
     def __abs__(self):
@@ -318,34 +307,20 @@
 
     def __float__(self):
         return float(self.price)
 
     def __round__(self, nDigits):
         return round(self.price, nDigits)
 
+    def __str__(self) -> str:
+        return self.symbol
 
-class Cryptocurrency(Asset):
-    def __init__(self, symbol: str) -> None:
-        """Exchange for trading cryptocurrencies"""
-        APCA_ID, APCA_SECRET = auth.get_api_keys()
-        self.client = CryptoHistoricalDataClient(APCA_ID, APCA_SECRET)
-        self.symbol = symbol
-        warnings.warn("WARNING: this is very broken and will be fixed later")
-
-    def _get_bars(self, start_date: datetime, end_date: datetime):
-        params = CryptoBarsRequest(
-            symbol_or_symbols=[self.symbol],
-            timeframe=TimeFrame.Day,
-            start=start_date,
-            end=end_date,
-        )
-        return self.client.get_crypto_bars(params)
+    def __repr__(self) -> str:
+        return self.symbol
 
-    def historical_data_df(
-        self, start_date: datetime, end_date: datetime
-    ) -> pd.DataFrame:
-        return self._get_bars(start_date, end_date).df
+    def __eq__(self, other):
+        if not isinstance(other, Asset):
+            raise ValueError
+        return self.symbol == other.symbol
 
-    def price(self) -> float:
-        """gets the asking price of the symbol"""
-        perms = CryptoLatestQuoteRequest(symbol_or_symbols=self.symbol)
-        return float(self.client.get_crypto_latest_quote(perms)[self.symbol].ask_price)
+    def __ne__(self, other):
+        return not self.__eq__(other)
```

### Comparing `cira-3.0.4/cira/auth.py` & `cira-3.1.0/cira/auth.py`

 * *Files identical despite different names*

### Comparing `cira-3.0.4/cira/exchange.py` & `cira-3.1.0/cira/exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def to_asset(self, symbol: str) -> asset.Asset:
         """Takes a symbols and returns
         it as a cira Assets objects"""
         return asset.Stock(symbol)
 
     def get_all_stocks(
         self, is_tradeable: bool = True, force_reload: bool = False
-    ) -> List[asset.Stock]:
+    ) -> List[asset.Asset]:
         """Returns a list of all stocks as cira asset,
         objects will be cached, can be turn off in config."""
         if config.USE_CASHING and self.stock_cache != [] and not force_reload:
             return self.stock_cache
         search_params = GetAssetsRequest(asset_class=AssetClass.US_EQUITY)
         alpc_assets = self.alpc_client.get_all_assets(search_params)
         self.stock_cache = [
```

### Comparing `cira-3.0.4/cira/portfolio.py` & `cira-3.1.0/cira/portfolio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Dict
 import warnings
 from alpaca.trading.client import TradingClient
 from . import auth
 from . import config
-from .asset import Stock
+from .asset_stock import Stock
 
 
 class Position:
     def __init__(self, symbol) -> None:
         APCA_ID, APCA_SECRET = auth.get_api_keys()
         self.client = TradingClient(APCA_ID, APCA_SECRET, paper=config.PAPER_TRADING)
         self.symbol = symbol
```

### Comparing `cira-3.0.4/cira/strategy.py` & `cira-3.1.0/cira/strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         )
         self.allocation.append(al)
         return al
 
 
 class ByAndHold(Strategy):
     def __init__(self) -> None:
-        super().__init__(name="ByAndHold")
+        super().__init__(name="BuyAndHold")
         self.is_first = True
         self.allocation = []
 
     def iterate(
         self,
         feature_data: pd.DataFrame,
         prices: pd.DataFrame,
@@ -88,15 +88,15 @@
             self.allocation.append(al)
             return al
         al = np.array([0] * len(prices.keys()))
         self.allocation.append(al)
         return al
 
 
-FEE_RATE = 0.004 # this is what alpaca takes 
+FEE_RATE = 0.004  # this is what alpaca takes
 
 fees = lambda prices, allocation: FEE_RATE * np.matmul(prices.T, allocation)
 
 
 def back_test(
     strat: Strategy,
     feature_data: pd.DataFrame,
```

### Comparing `cira-3.0.4/cira/util.py` & `cira-3.1.0/cira/util.py`

 * *Files identical despite different names*

### Comparing `cira-3.0.4/cira.egg-info/PKG-INFO` & `cira-3.1.0/cira.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cira
-Version: 3.0.4
+Version: 3.1.0
 Summary: A simpler library for the alapaca trade api
 Home-page: https://github.com/AxelGard/cira
 Author: Axel Gard
 Author-email: axel.gard@tutanota.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Office/Business :: Financial
```

### Comparing `cira-3.0.4/setup.py` & `cira-3.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="cira",
-    version="3.0.4",
+    version="3.1.0",
     description="A simpler library for the alapaca trade api",
     url="https://github.com/AxelGard/cira",
     author="Axel Gard",
     author_email="axel.gard@tutanota.com",
     license="MIT",
     packages=["cira"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
-        "alpaca-py==0.5.4",
+        "alpaca-py==0.21.0",
         "alpaca-trade-api==2.3.0",
         "schedule==1.2.0",
     ],
     extras_requires={"dev": ["pytest"]},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Topic :: Office/Business :: Financial",
```

