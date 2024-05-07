# Comparing `tmp/qubx-0.1.0.tar.gz` & `tmp/qubx-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qubx-0.1.0.tar", max compression
+gzip compressed data, was "qubx-0.1.3.tar", max compression
```

## Comparing `qubx-0.1.0.tar` & `qubx-0.1.3.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0      940 2024-04-25 07:51:17.473695 qubx-0.1.0/README.md
--rw-r--r--   0        0        0     9305 2024-04-21 10:35:06.164526 qubx-0.1.0/build.py
--rw-r--r--   0        0        0     1338 2024-04-25 07:51:17.477695 qubx-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5428 2024-04-21 10:35:06.176526 qubx-0.1.0/src/qubx/__init__.py
--rw-r--r--   0        0        0     1730 2024-04-25 07:51:17.477695 qubx-0.1.0/src/qubx/_nb_magic.py
--rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.1.0/src/qubx/core/__init__.py
--rw-r--r--   0        0        0     6707 2024-04-25 07:51:17.477695 qubx-0.1.0/src/qubx/core/account.py
--rw-r--r--   0        0        0    14763 2024-04-25 07:51:17.477695 qubx-0.1.0/src/qubx/core/basics.py
--rw-r--r--   0        0        0    11899 2024-04-25 07:51:17.477695 qubx-0.1.0/src/qubx/core/loggers.py
--rw-r--r--   0        0        0    13688 2024-04-21 10:35:06.176526 qubx-0.1.0/src/qubx/core/lookups.py
--rw-r--r--   0        0        0     2847 2024-04-21 10:35:06.176526 qubx-0.1.0/src/qubx/core/series.pxd
--rw-r--r--   0        0        0    28108 2024-04-21 10:35:06.176526 qubx-0.1.0/src/qubx/core/series.pyx
--rw-r--r--   0        0        0    25029 2024-04-25 07:51:17.477695 qubx-0.1.0/src/qubx/core/strategy.py
--rw-r--r--   0        0        0     1368 2024-02-29 14:43:31.739720 qubx-0.1.0/src/qubx/core/utils.pyx
--rw-r--r--   0        0        0    15531 2024-04-21 10:35:06.176526 qubx-0.1.0/src/qubx/data/readers.py
--rw-r--r--   0        0        0     9013 2024-04-25 07:51:17.481695 qubx-0.1.0/src/qubx/impl/ccxt_connector.py
--rw-r--r--   0        0        0     9092 2024-04-25 07:51:17.481695 qubx-0.1.0/src/qubx/impl/ccxt_trading.py
--rw-r--r--   0        0        0     3488 2024-04-21 10:35:06.176526 qubx-0.1.0/src/qubx/impl/exchange_customizations.py
--rw-r--r--   0        0        0     3565 2024-04-25 07:51:17.481695 qubx-0.1.0/src/qubx/impl/utils.py
--rw-r--r--   0        0        0       33 2024-02-29 14:43:31.739720 qubx-0.1.0/src/qubx/math/__init__.py
--rw-r--r--   0        0        0     1176 2024-02-29 14:43:31.739720 qubx-0.1.0/src/qubx/math/stats.py
--rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.1.0/src/qubx/ta/__init__.py
--rw-r--r--   0        0        0     7708 2024-02-29 14:43:31.739720 qubx-0.1.0/src/qubx/ta/indicators.pyx
--rw-r--r--   0        0        0       60 2024-04-21 10:35:06.176526 qubx-0.1.0/src/qubx/trackers/__init__.py
--rw-r--r--   0        0        0     5522 2024-04-21 10:35:06.176526 qubx-0.1.0/src/qubx/trackers/rebalancers.py
--rw-r--r--   0        0        0      262 2024-04-21 10:35:06.176526 qubx-0.1.0/src/qubx/utils/__init__.py
--rw-r--r--   0        0        0    12076 2024-04-21 10:35:06.176526 qubx-0.1.0/src/qubx/utils/_pyxreloader.py
--rw-r--r--   0        0        0     5937 2024-02-29 14:43:31.739720 qubx-0.1.0/src/qubx/utils/charting/mpl_helpers.py
--rw-r--r--   0        0        0    10999 2024-04-21 10:35:06.176526 qubx-0.1.0/src/qubx/utils/marketdata/binance.py
--rw-r--r--   0        0        0     9821 2024-04-25 07:51:17.481695 qubx-0.1.0/src/qubx/utils/misc.py
--rw-r--r--   0        0        0    18583 2024-04-21 10:35:06.176526 qubx-0.1.0/src/qubx/utils/pandas.py
--rw-r--r--   0        0        0     8656 2024-04-25 07:51:17.481695 qubx-0.1.0/src/qubx/utils/runner.py
--rw-r--r--   0        0        0     4604 2024-02-29 14:43:31.739720 qubx-0.1.0/src/qubx/utils/time.py
--rw-r--r--   0        0        0     2062 1970-01-01 00:00:00.000000 qubx-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      940 2024-04-25 07:51:17.473695 qubx-0.1.3/README.md
+-rw-r--r--   0        0        0     9305 2024-04-21 10:35:06.164526 qubx-0.1.3/build.py
+-rw-r--r--   0        0        0     1378 2024-05-07 13:17:10.565607 qubx-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5428 2024-04-21 10:35:06.176526 qubx-0.1.3/src/qubx/__init__.py
+-rw-r--r--   0        0        0     1730 2024-04-25 07:51:17.477695 qubx-0.1.3/src/qubx/_nb_magic.py
+-rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.1.3/src/qubx/core/__init__.py
+-rw-r--r--   0        0        0     6707 2024-04-25 07:51:17.477695 qubx-0.1.3/src/qubx/core/account.py
+-rw-r--r--   0        0        0    14777 2024-05-07 13:17:10.565607 qubx-0.1.3/src/qubx/core/basics.py
+-rw-r--r--   0        0        0    11559 2024-05-07 13:17:10.565607 qubx-0.1.3/src/qubx/core/helpers.py
+-rw-r--r--   0        0        0    11910 2024-05-07 13:17:10.565607 qubx-0.1.3/src/qubx/core/loggers.py
+-rw-r--r--   0        0        0    13688 2024-04-21 10:35:06.176526 qubx-0.1.3/src/qubx/core/lookups.py
+-rw-r--r--   0        0        0     2847 2024-04-21 10:35:06.176526 qubx-0.1.3/src/qubx/core/series.pxd
+-rw-r--r--   0        0        0    28108 2024-04-21 10:35:06.176526 qubx-0.1.3/src/qubx/core/series.pyx
+-rw-r--r--   0        0        0    30330 2024-05-07 13:17:10.565607 qubx-0.1.3/src/qubx/core/strategy.py
+-rw-r--r--   0        0        0     1368 2024-02-29 14:43:31.739720 qubx-0.1.3/src/qubx/core/utils.pyx
+-rw-r--r--   0        0        0    20161 2024-05-07 13:17:10.565607 qubx-0.1.3/src/qubx/data/readers.py
+-rw-r--r--   0        0        0     9150 2024-05-07 13:17:10.565607 qubx-0.1.3/src/qubx/impl/ccxt_connector.py
+-rw-r--r--   0        0        0     3488 2024-05-07 13:17:10.565607 qubx-0.1.3/src/qubx/impl/ccxt_customizations.py
+-rw-r--r--   0        0        0     9097 2024-05-07 13:17:10.565607 qubx-0.1.3/src/qubx/impl/ccxt_trading.py
+-rw-r--r--   0        0        0     3565 2024-05-07 13:17:10.565607 qubx-0.1.3/src/qubx/impl/ccxt_utils.py
+-rw-r--r--   0        0        0       33 2024-02-29 14:43:31.739720 qubx-0.1.3/src/qubx/math/__init__.py
+-rw-r--r--   0        0        0     1176 2024-02-29 14:43:31.739720 qubx-0.1.3/src/qubx/math/stats.py
+-rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.1.3/src/qubx/ta/__init__.py
+-rw-r--r--   0        0        0     7708 2024-02-29 14:43:31.739720 qubx-0.1.3/src/qubx/ta/indicators.pyx
+-rw-r--r--   0        0        0       60 2024-04-21 10:35:06.176526 qubx-0.1.3/src/qubx/trackers/__init__.py
+-rw-r--r--   0        0        0     5522 2024-04-21 10:35:06.176526 qubx-0.1.3/src/qubx/trackers/rebalancers.py
+-rw-r--r--   0        0        0      273 2024-05-07 13:17:10.569607 qubx-0.1.3/src/qubx/utils/__init__.py
+-rw-r--r--   0        0        0    12076 2024-04-21 10:35:06.176526 qubx-0.1.3/src/qubx/utils/_pyxreloader.py
+-rw-r--r--   0        0        0    35158 2024-05-07 13:17:10.569607 qubx-0.1.3/src/qubx/utils/charting/mpl_helpers.py
+-rw-r--r--   0        0        0    10999 2024-04-21 10:35:06.176526 qubx-0.1.3/src/qubx/utils/marketdata/binance.py
+-rw-r--r--   0        0        0     9837 2024-05-07 13:17:10.569607 qubx-0.1.3/src/qubx/utils/misc.py
+-rw-r--r--   0        0        0    18605 2024-05-07 13:17:10.569607 qubx-0.1.3/src/qubx/utils/pandas.py
+-rw-r--r--   0        0        0     9277 2024-05-07 13:17:10.569607 qubx-0.1.3/src/qubx/utils/runner.py
+-rw-r--r--   0        0        0     4884 2024-05-07 13:17:10.569607 qubx-0.1.3/src/qubx/utils/time.py
+-rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 qubx-0.1.3/PKG-INFO
```

### Comparing `qubx-0.1.0/README.md` & `qubx-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `qubx-0.1.0/build.py` & `qubx-0.1.3/build.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.0/pyproject.toml` & `qubx-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Qubx"
-version = "0.1.0"
+version = "0.1.3"
 description = "Qubx - quantitative trading framework"
 authors = ["Dmitry Marienko <dmitry@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "qubx", from = "src" },
 ]
 repository = "https://github.com/dmarienko/Qubx"
@@ -27,14 +27,16 @@
 pydantic = "^1.10.2"
 python-dotenv = "^1.0.0"
 python-binance = "^1.0.19"
 pyarrow = "^15.0.0"
 scipy = "^1.12.0"
 cython = "3.0.8"
 ccxt = "^4.2.68"
+croniter = "^2.0.5"
+psycopg = "^3.1.18"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.20.0"
 pytest = "^7.1.3"
 
 #[project.optional-dependencies]
 #numba = "^0.57.1"
```

### Comparing `qubx-0.1.0/src/qubx/__init__.py` & `qubx-0.1.3/src/qubx/__init__.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.0/src/qubx/_nb_magic.py` & `qubx-0.1.3/src/qubx/_nb_magic.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.0/src/qubx/core/account.py` & `qubx-0.1.3/src/qubx/core/account.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.0/src/qubx/core/basics.py` & `qubx-0.1.3/src/qubx/core/basics.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,20 +334,20 @@
     Controlled data communication channel
     """
     control: Event
     queue: Queue     # we need something like disruptor here (Queue is temporary)
     name: str
     lock: Lock
 
-    def __init__(self, name: str, sent=(None, None)):
+    def __init__(self, name: str, sentinel=(None, None, None)):
         self.name = name
         self.control = Event()
         self.queue = Queue()
         self.lock = Lock()
-        self.sent = sent
+        self.sent = sentinel
         self.start()
 
     def stop(self):
         if self.control.is_set():
             self.control.clear()
             self.queue.put(self.sent) # send sentinel
```

### Comparing `qubx-0.1.0/src/qubx/core/loggers.py` & `qubx-0.1.3/src/qubx/core/loggers.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
                 with open(self._balance_file_path, "w", newline='') as f:
                     w = csv.writer(f)
                     w.writerow(self._header(data[0]))
                     w.writerows(self._values(data))
 
     def write_data(self, log_type: str, data: List[Dict[str, Any]]):
         if len(data) > 0:
-            self.pool.apply(self._do_write, (log_type, data))
+            self.pool.apply_async(self._do_write, (log_type, data))
 
     def flush_data(self):
         try:
             self._pfl_file_.flush()
             self._execs_file_.flush()
         except Exception as e:
             logger.warning(f"Error flushing log writer: {str(e)}")
@@ -257,15 +257,15 @@
             for s, d in balance.items():
                 data.append({
                     'timestamp': timestamp,
                     'instrument_id': s,
                     'total': d[0],
                     'locked': d[1],
                 })
-        self._writer.write_data('balance', data)
+            self._writer.write_data('balance', data)
 
     def store(self, timestamp: np.datetime64):
         pass
 
     def close(self):
         self._writer.flush_data()
 
@@ -336,8 +336,8 @@
 
         # - notify portfolio records logger
         if self.portfolio_logger:
             self.portfolio_logger.store(timestamp)
 
     def save_deals(self, symbol: str, deals: List[Deal]):
         if self.executions_logger:
-            self.executions_logger.record_deals(symbol, deals)
+            self.executions_logger.record_deals(symbol, deals)
```

### Comparing `qubx-0.1.0/src/qubx/core/lookups.py` & `qubx-0.1.3/src/qubx/core/lookups.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.0/src/qubx/core/series.pxd` & `qubx-0.1.3/src/qubx/core/series.pxd`

 * *Files identical despite different names*

### Comparing `qubx-0.1.0/src/qubx/core/series.pyx` & `qubx-0.1.3/src/qubx/core/series.pyx`

 * *Files identical despite different names*

### Comparing `qubx-0.1.0/src/qubx/core/strategy.py` & `qubx-0.1.3/src/qubx/core/strategy.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,29 @@
 """
  # All interfaces related to strategy etc
 """
-from collections import defaultdict
-from threading import Thread
-import traceback
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 from types import FunctionType
-import numpy as np
+from collections import defaultdict
 from dataclasses import dataclass
-from enum import Enum
+from threading import Thread
+from multiprocessing.pool import ThreadPool
+import traceback
 
 import pandas as pd
 
 from qubx import lookup, logger
 from qubx.core.account import AccountProcessor
-from qubx.core.loggers import BalanceLogger, ExecutionsLogger, LogsWriter, PortfolioLogger, PositionsDumper, StrategyLogging
+from qubx.core.helpers import BasicScheduler, CachedMarketDataHolder, process_schedule_spec
+from qubx.core.loggers import LogsWriter, StrategyLogging
 from qubx.core.lookups import InstrumentsLookup
 from qubx.core.basics import Deal, Instrument, Order, Position, Signal, dt_64, td_64, CtrlChannel
 from qubx.core.series import TimeSeries, Trade, Quote, Bar, OHLCV
-from qubx.utils.time import convert_tf_str_td64
 from qubx.utils.misc import Stopwatch
-
-
-@dataclass
-class EventFromExchange:
-    time: dt_64
-    type: str
-    data: Optional[Any] 
+from qubx.utils.time import convert_seconds_to_str
 
 
 @dataclass
 class TriggerEvent:
     time: dt_64
     type: str
     instrument: Optional[Instrument]
@@ -41,15 +34,15 @@
 
     def subscribe(self, subscription_type: str, symbols: List[str], **kwargs) -> bool:
         raise NotImplementedError("subscribe")
 
     def get_communication_channel(self) -> CtrlChannel:
         raise NotImplementedError("get_communication_channel")
 
-    def get_historical_ohlcs(self, symbol: str, timeframe: str, nbarsback: int) -> List[Bar] | None:
+    def get_historical_ohlcs(self, symbol: str, timeframe: str, nbarsback: int) -> List[Bar]:
         raise NotImplementedError("get_historical_ohlcs")
 
     def get_quote(self, symbol: str) -> Quote | None:
         raise NotImplementedError("get_quote")
 
 
 class IExchangeServiceProvider:
@@ -63,17 +56,14 @@
 
     def get_account(self) -> AccountProcessor:
         return self.acc
 
     def get_name(self) -> str:
         raise NotImplementedError("get_name is not implemented")
 
-    def schedule_trigger(self, trigger_id: str, when: str):
-        raise NotImplementedError("schedule_trigger is not implemented")
-
     def get_capital(self) -> float:
         return self.acc.get_capital()
 
     def send_order(self, instrument: Instrument, order_side: str, order_type: str, amount: float, price: float | None = None, 
         client_id: str | None = None, time_in_force: str='gtc') -> Order | None:
         raise NotImplementedError("send_order is not implemented")
 
@@ -97,124 +87,65 @@
         self.ctx = ctx
     
 
 class IStrategy:
     ctx: 'StrategyContext'
 
     def on_start(self, ctx: 'StrategyContext'):
+        """
+        This method is called strategy is started
+        """
         pass
 
+    def on_fit(self, ctx: 'StrategyContext', fit_time: str | pd.Timestamp, previous_fit_time: str | pd.Timestamp | None = None):
+        """
+        This method is called when it's time to fit model
+        :param fit_time: last time of fit data to use 
+        :param previous_fit_time: last time of fit data used in previous fit call 
+        """
+        return None
+
     def on_event(self, ctx: 'StrategyContext', event: TriggerEvent) -> Optional[List[Signal]]:
         return None
 
     def on_stop(self, ctx: 'StrategyContext'):
         pass
 
     def tracker(self, ctx: 'StrategyContext') -> PositionsTracker | None:
         pass
 
 
-def _dict_with_exc(dct, f):
+def _dict_with_exception(dct, f):
     if f not in dct:
         raise ValueError(f"Configuration {dct} must contain field '{f}'")
     return dct[f]
 
 
 def _round_down_at_min_qty(x: float, min_size: float) -> float:
     return (int(x / min_size)) * min_size
 
 
 _SW = Stopwatch()
 
-
-class CachedMarketDataHolder: 
-    _min_timeframe: dt_64
-    _last_bar: Dict[str, Optional[Bar]]
-    _ohlcvs: Dict[str, Dict[td_64, OHLCV]]
-
-    def __init__(self, minimal_timeframe: str) -> None:
-        self._min_timeframe = convert_tf_str_td64(minimal_timeframe)
-        self._ohlcvs = dict()
-        self._last_bar = defaultdict(lambda: None)
-
-    def init_ohlcv(self, symbol: str, max_size=np.inf):
-        self._ohlcvs[symbol] = {self._min_timeframe: OHLCV(symbol, self._min_timeframe, max_size)}
-    
-    @_SW.watch('CachedMarketDataHolder')
-    def get_ohlcv(self, symbol: str, timeframe: str, max_size=np.inf) -> OHLCV:
-        tf = convert_tf_str_td64(timeframe) 
-
-        if symbol not in self._ohlcvs:
-           self._ohlcvs[symbol] = {}
-
-        if tf not in self._ohlcvs[symbol]: 
-            # - check requested timeframe
-            new_ohlc = OHLCV(symbol, tf, max_size)
-            if tf < self._min_timeframe:
-                logger.warning(f"[{symbol}] Request for timeframe {timeframe} that is smaller then minimal {self._min_timeframe}")
-            else:
-                # - first try to resample from smaller frame
-                if (basis := self._ohlcvs[symbol].get(self._min_timeframe)):
-                    for b in basis[::-1]:
-                        new_ohlc.update_by_bar(b.time, b.open, b.high, b.low, b.close, b.volume, b.bought_volume)
-                
-            self._ohlcvs[symbol][tf] = new_ohlc
-
-        return self._ohlcvs[symbol][tf]
-
-    @_SW.watch('CachedMarketDataHolder')
-    def update_by_bar(self, symbol: str, bar: Bar):
-        _last_bar = self._last_bar[symbol]
-        v_tot_inc = bar.volume
-        v_buy_inc = bar.bought_volume
-
-        if _last_bar is not None:
-            if _last_bar.time == bar.time: # just current bar updated
-                v_tot_inc -= _last_bar.volume
-                v_buy_inc -= _last_bar.bought_volume
-
-            if _last_bar.time > bar.time: # update is too late - skip it
-                return
-
-        if symbol in self._ohlcvs:
-            self._last_bar[symbol] = bar
-            for ser in self._ohlcvs[symbol].values():
-                ser.update_by_bar(bar.time, bar.open, bar.high, bar.low, bar.close, v_tot_inc, v_buy_inc)
-
-    @_SW.watch('CachedMarketDataHolder')
-    def update_by_quote(self, symbol: str, quote: Quote):
-        series = self._ohlcvs.get(symbol)
-        if series:
-            for ser in series.values():
-                ser.update(quote.time, quote.mid_price(), 0)
-
-    @_SW.watch('CachedMarketDataHolder')
-    def update_by_trade(self, symbol: str, trade: Trade):
-        series = self._ohlcvs.get(symbol)
-        if series:
-            total_vol = trade.size 
-            bought_vol = total_vol if trade.taker >= 1 else 0.0 
-            for ser in series.values():
-                ser.update(trade.time, trade.price, total_vol, bought_vol)
-
  
 class StrategyContext:
     MAX_NUMBER_OF_STRATEGY_FAILURES = 10
 
     strategy: IStrategy                         # strategy instance
     exchange_service: IExchangeServiceProvider  # service for exchange API: orders managemewnt
     data_provider: IDataProvider                # market data provider 
     instruments: List[Instrument]               # list of instruments this strategy trades
     positions: Dict[str, Position]              # positions of the strategy (instrument -> position)
 
     # - loggers
     _logging: StrategyLogging                    # recording all activities for the strat: execs, positions, portfolio
 
-    # - cached marked data
+    # - cached marked data anb scheduler
     _cache: CachedMarketDataHolder # market data cache
+    _scheduler: BasicScheduler
 
     # - configuration
     _market_data_subcription_type:str = 'unknown'
     _market_data_subcription_params: dict = dict()
     _thread_data_loop: Thread | None = None            # market data loop
 
     _trig_interval_in_bar_nsec: int
@@ -226,29 +157,37 @@
     _trig_on_book: bool = False
     _current_bar_trigger_processed: bool = False
     _is_initilized: bool = False
     _symb_to_instr: Dict[str, Instrument]
     __strategy_id: str
     __order_id: int 
     __handlers: Dict[str, Callable[['StrategyContext', str, Any], TriggerEvent | None]]
+    __fit_is_running: bool = False                       # during fitting working it stops calling on_event method
+    __init_fit_was_called: bool = False                  # true if initial fit was already run
+    __init_fit_args: Tuple = (None, None)                # arguments for initial on_fit() method call
+    __pool: ThreadPool | None = None                     # thread pool used for running aux tasks (fit etc)
 
     def __init__(self, 
             # - strategy with parameters
             strategy: IStrategy, config: Dict[str, Any] | None,
             # - - - - - - - - - - - - - - - - - - - - -
 
             # - data provider and exchange service
             data_provider: IDataProvider,
             exchange_service: IExchangeServiceProvider, 
             instruments: List[Instrument],
             # - - - - - - - - - - - - - - - - - - - - -
 
-            # - context's parameters - - - - - - - - - -
-            trigger: Dict[str, Any] = dict(type='ohlc', timeframe='1Min', nback=60),
-            md_subscription: Dict[str,Any] = dict(type='ohlc', timeframe='1Min'),
+            # - data subscription - - - - - - - - - - -
+            md_subscription: Dict[str,Any] = dict(type='ohlc', timeframe='1Min', nback=60),
+            # - - - - - - - - - - - - - - - - - - - - -
+
+            # - when need to trigger and fit strategy - - - - - - -
+            trigger_spec: str = 'bar: -1Sec',       # 1 sec before subscription bar is closed
+            fit_spec: str | None = None,
             # - - - - - - - - - - - - - - - - - - - - -
 
             # - how to write logs - - - - - - - - - -
             logs_writer: LogsWriter | None = None,
             positions_log_freq: str = '1Min',
             portfolio_log_freq: str = '5Min',
             num_exec_records_to_write = 1      # in live let's write every execution 
@@ -256,39 +195,46 @@
 
         # - initialization
         self.exchange_service = exchange_service
         self.data_provider = data_provider
         self.config = config
         self.instruments = instruments
         self.positions = {}
-
-        # - create strategy instance and populate custom paramameters
-        self.__instantiate_strategy(strategy, config)
+        self.__fit_is_running = False         
+        self.__init_fit_was_called = False     
+        self.__pool = None 
 
         # - for fast access to instrument by it's symbol
         self._symb_to_instr = {i.symbol: i for i in instruments}
- 
-        # - process trigger configuration
-        self.__check_how_to_trigger_strategy(trigger)
 
-        # - process market data configuration
-        self.__check_how_to_listen_to_market_data(md_subscription)
+        # - create scheduler
+        self._scheduler = BasicScheduler(self.data_provider.get_communication_channel(), lambda: self.time().item())
 
         # - instantiate logging functional
-        self._logging = StrategyLogging(
-            logs_writer, positions_log_freq, portfolio_log_freq, num_exec_records_to_write
-        )
+        self._logging = StrategyLogging(logs_writer, positions_log_freq, portfolio_log_freq, num_exec_records_to_write)
 
         # - extract data and event handlers
         self.__handlers = {
             n.split('_processing_')[1]: f for n, f in self.__class__.__dict__.items() 
             if type(f) == FunctionType and n.startswith('_processing_') 
         }
 
-    def __instantiate_strategy(self, strategy: IStrategy, config: Dict[str, Any] | None):
+        # - create strategy instance and populate custom paramameters
+        self._instantiate_strategy(strategy, config)
+
+        # - process market data configuration
+        self.__check_how_to_listen_to_market_data(md_subscription)
+ 
+        # - process trigger and fit configurations
+        self.__check_how_to_trigger_and_fit_strategy(trigger_spec, fit_spec)
+
+        # - run cron scheduler
+        self._scheduler.run()
+
+    def _instantiate_strategy(self, strategy: IStrategy, config: Dict[str, Any] | None):
         # - set parameters to strategy (not sure we will do it here)
         self.strategy = strategy
         if isinstance(strategy, type):
             self.strategy = strategy()
         self.strategy.ctx = self
 
         # TODO: - trackers - - - - - - - - - - - - -
@@ -299,18 +245,18 @@
         # - set strategy custom parameters 
         self.populate_parameters_to_strategy(self.strategy, **config if config else {})
         self._is_initilized = False
         self.__strategy_id = self.strategy.__class__.__name__ + "_"
         self.__order_id = self.time().item() // 100_000_000
 
     def __check_how_to_listen_to_market_data(self, md_config: dict):
-        self._market_data_subcription_type = _dict_with_exc(md_config, 'type').lower()
+        self._market_data_subcription_type = _dict_with_exception(md_config, 'type').lower()
         match self._market_data_subcription_type:
             case 'ohlc':
-                timeframe = _dict_with_exc(md_config, 'timeframe')
+                timeframe = _dict_with_exception(md_config, 'timeframe')
                 self._market_data_subcription_params = {
                     'timeframe': timeframe,
                     'nback': md_config.get('nback', 1), 
                 }
                 self._cache = CachedMarketDataHolder(timeframe) 
 
             case 'trade' | 'trades' | 'tas':
@@ -321,79 +267,145 @@
 
             case 'ob' | 'orderbook':
                 self._cache = CachedMarketDataHolder('1Sec') 
 
             case _:
                 raise ValueError(f"{self._market_data_subcription_type} is not a valid value for market data subcription type !!!")
 
-    def __check_how_to_trigger_strategy(self, trigger_config: dict):
-        # - check how it's configured to be triggered
-        self._trig_interval_in_bar_nsec = 0
+    def __check_how_to_trigger_and_fit_strategy(self, trigger_schedule: str | None, fit_schedue: str | None):
+        _td2ns = lambda x: x.as_unit('ns').asm8.item()
 
-        match (_trigger := _dict_with_exc(trigger_config, 'type').lower()):
-            case 'bar': 
-                self._trig_on_bar = True
-
-                _bar_timeframe = pd.Timedelta(_dict_with_exc(trigger_config, 'timeframe'))
-                _inside_bar_delay = pd.Timedelta(_dict_with_exc(trigger_config, 'delay'))
+        self._trig_interval_in_bar_nsec = 0
+        
+        if not trigger_schedule:
+            raise ValueError("trigger parameter can't be empty !")
+        t_rules = process_schedule_spec(trigger_schedule)
+        f_rules = process_schedule_spec(fit_schedue)
+
+        if t_rules is None:
+            raise ValueError(f"Couldn't recognize 'trigger' parameter specification: {trigger_schedule} !")
+
+        # - we can use it as reference if bar timeframe is not secified
+        _default_data_timeframe = pd.Timedelta(self._cache.default_timeframe)
+
+        # - check trigger spec - - - - -
+        match t_rules['type']:
+            # it triggers on_event method when new bar is formed.
+            # in this case it won't arm scheduler but just ruled by actual market data updates 
+            # - TODO: so probably need to drop this in favor to cron tasks
+            # it's also possible to specify delay
+            # "bar: -1s"      - it uses default timeframe and wake up 1 sec before every bar's close
+            # "bar.5m: -5sec" - 5 sec before 5min bar's close
+            # "bar.5m: 1sec"  - 1 sec after 5min bar closed (in next bar)
+            case 'bar':
+                _r_tf = t_rules.get('timeframe')
+                _bar_timeframe = _default_data_timeframe if not _r_tf else pd.Timedelta(_r_tf)
+                _inside_bar_delay: pd.Timedelta = t_rules.get('delay', pd.Timedelta(0))
 
                 if abs(pd.Timedelta(_inside_bar_delay)) > pd.Timedelta(_bar_timeframe):
-                    raise ValueError(f"Delay must be less or equal to bar's timeframe for {_trigger} trigger: you set delay {_inside_bar_delay} for {_bar_timeframe}")
+                    raise ValueError(f"Delay must be less or equal to bar's timeframe for bar trigger: you used {_inside_bar_delay} delay for {_bar_timeframe}")
 
                 # for positive delay - trigger strategy when this interval passed after new bar's open
                 if _inside_bar_delay >= pd.Timedelta(0): 
-                    self._trig_interval_in_bar_nsec = _inside_bar_delay.asm8.item()
+                    self._trig_interval_in_bar_nsec = _td2ns(_inside_bar_delay)
+
                 # for negative delay - trigger strategy when time is closer to bar's closing time more than this interval
                 else:
-                    self._trig_interval_in_bar_nsec = (_bar_timeframe + _inside_bar_delay).asm8.item()
-                self._trig_bar_freq_nsec = _bar_timeframe.asm8.item()
+                    self._trig_interval_in_bar_nsec = _td2ns(_bar_timeframe + _inside_bar_delay)
+
+                self._trig_bar_freq_nsec = _td2ns(_bar_timeframe)
+                self._trig_on_bar = True
 
-            case 'time': 
-                self._trig_on_time = True
-                _time_to_trigger = _dict_with_exc(trigger_config, 'when')
+                logger.debug(f"Triggering strategy on every {convert_seconds_to_str(self._trig_bar_freq_nsec/1e9)} bar after {convert_seconds_to_str(self._trig_interval_in_bar_nsec/1e9)}")
 
-                # - schedule periodic timer
-                self.exchange_service.schedule_trigger('time', _time_to_trigger)
+            case 'cron':
+                if 'schedule' not in t_rules:
+                    raise ValueError(f"cron trigger type is specified but cron schedule not found !")
+
+                self._scheduler.schedule_event(t_rules['schedule'], 'time_event')
 
             case 'quote': 
                 self._trig_on_quote = True
-                raise ValueError(f"{_trigger} NOT IMPLEMENTED")
+                raise ValueError(f"quote trigger NOT IMPLEMENTED YET")
 
             case 'trade': 
                 self._trig_on_trade = True
-                raise ValueError(f"{_trigger} NOT IMPLEMENTED")
+                raise ValueError(f"trade trigger NOT IMPLEMENTED YET")
 
             case 'orderbook' | 'ob': 
                 self._trig_on_book = True
-                raise ValueError(f"{_trigger} NOT IMPLEMENTED")
+                raise ValueError(f"orderbook trigger NOT IMPLEMENTED YET")
+
+            case _: 
+                raise ValueError(f"Wrong trigger type {t_rules['type']}")
+
+        # - check fit spec - - - - -
+        _last_fit_data_can_be_used = pd.Timestamp(self.time())
+        match f_rules.get('type'):
+            case 'cron':
+                if 'schedule' not in f_rules:
+                    raise ValueError(f"cron fit trigger type is specified but cron schedule not found !")
+
+                self._scheduler.schedule_event(f_rules['schedule'], 'fit_event')
+                _last_fit_data_can_be_used = self._scheduler.get_event_last_time('fit_event')
+
+            case 'bar':
+                raise ValueError("Raw 'bar' type is not supported for fitting spec yet, please use cron type !")
 
             case _: 
-                raise ValueError(f"Wrong trigger type {_trigger}")
+                # if schedule is not specified just do not arm the task 
+                # only initial fit will be called
+                pass
+
+        # - we can't just call on_fit right now because not all market data may be ready
+        # - so we just mark it as not called yet
+        self.__init_fit_was_called = False
+        self.__init_fit_args = (None, _last_fit_data_can_be_used) 
    
     def _process_incoming_data(self, channel: CtrlChannel):
         _fails_counter = 0 
         logger.info("(StrategyContext) Start processing market data")
 
         while channel.control.is_set():
             # - start loop latency measurement 
             _SW.start('StrategyContext._process_incoming_data')
 
             # - waiting for incoming market data
             symbol, d_type, data = channel.queue.get()
 
             # - process data if handler is registered
             handler = self.__handlers.get(d_type)
-            _strategy_trigger_event = handler(self, symbol, data) if handler else None
-            if _strategy_trigger_event:
+            _SW.start('StrategyContext.handler')
+            _strategy_trigger_on_event = handler(self, symbol, data) if handler else None
+            _SW.stop('StrategyContext.handler')
+
+            # - check if it still didn't call on_fit() for first time
+            if not self.__init_fit_was_called:
+                self._processing_fit_event(None, self.__init_fit_args)
+
+            if _strategy_trigger_on_event:
+
+                # - if fit was not called - skip on_event call
+                if not self.__init_fit_was_called:
+                    _SW.stop('StrategyContext._process_incoming_data')
+                    logger.warning(f"[{self.time()}] {self.strategy.__class__.__name__}::on_event() is SKIPPED for now because on_fit() was not called yet !")
+                    continue
+
+                # - if strategy still fitting - skip on_event call
+                if self.__fit_is_running:
+                    _SW.stop('StrategyContext._process_incoming_data')
+                    logger.warning(f"[{self.time()}] {self.strategy.__class__.__name__}::on_event() is SKIPPED for now because is being still fitting !")
+                    continue
+
                 try:
                     _SW.start('strategy.on_event')
-                    self.strategy.on_event(self, _strategy_trigger_event)
+                    self.strategy.on_event(self, _strategy_trigger_on_event)
                     _fails_counter = 0
                 except Exception as strat_error:
-                    # - TODO: probably we need some cooldown interval after exception to prevent flooding
+                    # - probably we need some cooldown interval after exception to prevent flooding
                     logger.error(f"[{self.time()}]: Strategy {self.strategy.__class__.__name__} raised an exception: {strat_error}")
                     logger.opt(colors=False).error(traceback.format_exc())
 
                     #  - we stop execution after let's say maximal number of errors in a row
                     if (_fails_counter := _fails_counter + 1) >= StrategyContext.MAX_NUMBER_OF_STRATEGY_FAILURES:
                         logger.error("STRATEGY FAILURES IN THE ROW EXCEEDED MAX ALLOWED NUMBER - STOPPING ...")
                         channel.stop()
@@ -406,37 +418,81 @@
 
             # - notify poition and portfolio loggers
             self._logging.notify(self.time())
 
         _SW.stop('StrategyContext._process_incoming_data')
         logger.info("(StrategyContext) Market data processing stopped")
 
+    def _invoke_on_fit(self, current_fit_time: str | pd.Timestamp, prev_fit_time: str | pd.Timestamp | None):
+        try:
+            self.__fit_is_running = True
+            logger.debug(f"[{self.time()}]: Invoking {self.strategy.__class__.__name__} on_fit('{current_fit_time}', '{prev_fit_time}')")
+            _SW.start('strategy.on_fit')
+            self.strategy.on_fit(self, current_fit_time, prev_fit_time)
+            logger.debug(f"[{self.time()}]: {self.strategy.__class__.__name__} is fitted")
+        except Exception as strat_error:
+            logger.error(f"[{self.time()}]: Strategy {self.strategy.__class__.__name__} on_fit('{current_fit_time}', '{prev_fit_time}') raised an exception: {strat_error}")
+            logger.opt(colors=False).error(traceback.format_exc())
+        finally:
+            self.__fit_is_running = False
+            self.__init_fit_was_called = True
+            _SW.stop('strategy.on_fit')
+        return None
+
+    def _processing_time_event(self, symbol: str, data: Any) -> TriggerEvent | None:
+        """
+        When scheduled time event is happened - we need to invoke strategy on_event method
+        """
+        return TriggerEvent(self.time(), 'time', None, data)
+
+    def _processing_fit_event(self, symbol: str | None, data: Any) -> TriggerEvent | None:
+        """
+        When scheduled fit event is happened - we need to invoke strategy on_fit method
+        """
+        if not self._cache.is_data_ready():
+            return None
+
+        # times are in seconds here
+        prev_fit_time, now_fit_time = data
+
+        # - we need to run this in separate thread
+        self.__fit_is_running = True
+        self._run_in_thread_pool(self._invoke_on_fit, (
+            pd.Timestamp(now_fit_time, unit='s'), 
+            pd.Timestamp(prev_fit_time, unit='s') if prev_fit_time else None
+        ))
+
+        return None
+
     def _processing_hist_bar(self, symbol: str, bar: Bar) -> TriggerEvent | None:
         # - processing single historical bar
         #   here it just updates cache - historical bar can't trigger strategy logic
         self._cache.update_by_bar(symbol, bar)
         return None
 
     def _processing_hist_bars(self, symbol: str, bars: List[Bar]) -> TriggerEvent | None:
         # - processing historical bars as list
         for b in bars:
             self._processing_hist_bar(symbol, b)
         return None
 
+    @_SW.watch('StrategyContext')
     def _processing_bar(self, symbol: str, bar: Bar) -> TriggerEvent | None:
         # - processing current bar's update
         self._cache.update_by_bar(symbol, bar)
+
+        # - check if it's time to trigger the on_event if it's configured
         if self._trig_on_bar:
             t = self.exchange_service.time().item()
             _time_to_trigger = t % self._trig_bar_freq_nsec >= self._trig_interval_in_bar_nsec
             if _time_to_trigger: 
                 # we want to trigger only first one - not every
                 if not self._current_bar_trigger_processed:
                     self._current_bar_trigger_processed = True
-                    return TriggerEvent(self.time(), 'bar', symbol, bar)
+                    return TriggerEvent(self.time(), 'bar', self._symb_to_instr.get(symbol), bar)
             else:
                 self._current_bar_trigger_processed = False
         return None
 
     def _processing_trade(self, symbol: str, trade: Trade) -> TriggerEvent | None:
         if self._trig_on_trade:
             return TriggerEvent(self.time(), 'trade', symbol, trade)
@@ -446,19 +502,14 @@
         # - TODO: here we can apply throttlings or filters
         #  - let's say we can skip quotes if bid & ask is not changed
         #  - or we can collect let's say N quotes before sending to strategy
         if self._trig_on_quote:
             return TriggerEvent(self.time(), 'quote', symbol, quote)
         return None
 
-    def _processing_event(self, symbol: str, event: EventFromExchange) -> TriggerEvent | None:
-        if self._trig_on_time and event.type == 'time':
-            return TriggerEvent(self.time(), 'time', symbol, event)
-        return None
-
     @_SW.watch('StrategyContext')
     def _processing_order(self, symbol: str, order: Order) -> TriggerEvent | None:
         logger.debug(f"[{order.id} / {order.client_id}] : {order.type} {order.side} {order.quantity} of {symbol} { (' @ ' + str(order.price)) if order.price else '' } -> [{order.status}]")
         # - check if we want to trigger any strat's logic on order
         return None
 
     @_SW.watch('StrategyContext')
@@ -537,14 +588,17 @@
             except Exception as strat_error:
                 logger.error(f"(StrategyContext) Strategy {self.strategy.__class__.__name__} raised an exception in on_stop: {strat_error}")
                 logger.error(traceback.format_exc())
             self._thread_data_loop = None
 
         # - close logging
         self._logging.close()
+        self.get_latencies_report()
+
+    def get_latencies_report(self):
         for l in _SW.latencies.keys():
             logger.info(f"\t<w>{l}</w> took <r>{_SW.latency_sec(l):.7f}</r> secs")
 
     def populate_parameters_to_strategy(self, strategy: IStrategy, **kwargs):
         _log_info = ""
         for k,v in kwargs.items():
             if k.startswith('_'):
@@ -593,8 +647,61 @@
     def quote(self, symbol: str) -> Quote | None:
         return self.data_provider.get_quote(symbol)
 
     def get_capital(self) -> float:
         return self.exchange_service.get_capital()
 
     def get_reserved(self, instrument: Instrument) -> float:
-        return self.exchange_service.get_account().get_reserved(instrument)
+        return self.exchange_service.get_account().get_reserved(instrument)
+
+    @_SW.watch('StrategyContext')
+    def get_historical_ohlcs(self, instrument: Instrument | str, timeframe: str, length: int) -> OHLCV | None:
+        """
+        Helper for historical ohlc data
+        """
+        instr = self._symb_to_instr.get(instrument) if isinstance(instrument, str) else instrument
+
+        if instr is None:
+            logger.warning(f"Can't find instrument for {instrument} symbol !")
+            return None
+
+        # - first check if we can use cached series
+        rc = self.ohlc(instr, timeframe)
+        if len(rc) >= length:
+            return rc
+
+        # - send request for historical data
+        bars = self.data_provider.get_historical_ohlcs(instr.symbol, timeframe, length) 
+        r = self._cache.update_by_bars(instr.symbol, timeframe, bars)
+        return r 
+
+    def _run_in_thread_pool(self, func: Callable, args=()):
+        """
+        For backtester we need to override this method and just call function
+        """
+        if self.__pool is None:
+            self.__pool = ThreadPool(2)
+        self.__pool.apply_async(func, args)
+
+
+if __name__ == '__main__':
+    from qubx.utils.runner import create_strategy_context
+    import time, sys
+    filename, accounts, paths = '../experiments/configs/zero_test_scheduler.yaml', "../experiments/configs/.env", ['../']
+
+    # - create context
+    ctx = create_strategy_context(filename, accounts, paths)
+    if ctx is None:
+        sys.exit(0)
+
+    # - run main loop
+    try:
+        ctx.start()
+
+        # - just wake up every 60 sec and check if it's OK 
+        while True: 
+            time.sleep(60)
+
+    except KeyboardInterrupt:
+        ctx.stop()
+        time.sleep(1)
+        sys.exit(0)
```

### Comparing `qubx-0.1.0/src/qubx/core/utils.pyx` & `qubx-0.1.3/src/qubx/core/utils.pyx`

 * *Files identical despite different names*

### Comparing `qubx-0.1.0/src/qubx/data/readers.py` & `qubx-0.1.3/src/qubx/data/readers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+import re
 from typing import List, Union, Optional, Iterable, Any
 from os.path import exists
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 from pyarrow import csv
+import psycopg as pg
+from functools import wraps
 
 from qubx import logger
 from qubx.core.series import TimeSeries, OHLCV, time_as_nsec, Quote, Trade
 from qubx.utils.time import infer_series_frequency, handle_start_stop
 
 _DT = lambda x: pd.Timedelta(x).to_numpy().item()
 D1, H1 = _DT('1D'), _DT('1h')
@@ -39,23 +42,30 @@
     """
     Common interface for data processor with default aggregating into list implementation
     """
     def __init__(self) -> None:
         self.buffer = {}
         self._column_names = []
 
-    def start_processing(self, column_names: List[str]):
+    def start_processing(self, column_names: List[str], name: str | None = None):
         self._column_names = column_names
         self.buffer = {c: [] for c in column_names}
 
-    def process_data(self, columns_data: list) -> Optional[Iterable]:
+    def process_data_columns(self, columns_data: list) -> Optional[Iterable]:
         for i, c in enumerate(columns_data):
             self.buffer[self._column_names[i]].append(c)
         return None
 
+    def process_data_rows(self, rows_data: list) -> Optional[Iterable]:
+        for r in rows_data:
+            c = []
+            for j, d in enumerate(r):
+                self.buffer[self._column_names[j]].append(d)
+        return None
+
     def get_result(self) -> Any:
         return self.buffer
 
 
 class DataReader:
     """
     Common interface for data reader
@@ -69,23 +79,23 @@
         pass
 
     
 class QuotesDataProcessor(DataProcessor):
     """
     Process quotes data and collect them as list
     """
-    def start_processing(self, fieldnames: List[str]):
+    def start_processing(self, fieldnames: List[str], name: str | None = None):
         self.buffer = list()
         self._time_idx = _find_column_index_in_list(fieldnames, 'time', 'timestamp', 'datetime')
         self._bid_idx = _find_column_index_in_list(fieldnames, 'bid')
         self._ask_idx = _find_column_index_in_list(fieldnames, 'ask')
         self._bidvol_idx = _find_column_index_in_list(fieldnames, 'bidvol', 'bid_vol', 'bidsize', 'bid_size')
         self._askvol_idx = _find_column_index_in_list(fieldnames, 'askvol', 'ask_vol', 'asksize', 'ask_size')
 
-    def process_data(self, columns_data: list) -> Optional[Iterable]:
+    def process_data_columns(self, columns_data: list) -> Optional[Iterable]:
         tms = columns_data[self._time_idx] 
         bids = columns_data[self._bid_idx]
         asks = columns_data[self._ask_idx]
         bidvol = columns_data[self._bidvol_idx]
         askvol = columns_data[self._askvol_idx]
         for i in range(len(tms)):
             self.buffer.append(Quote(tms[i], bids[i], asks[i], bidvol[i], askvol[i]))
@@ -106,15 +116,15 @@
         self._trades = trades
         self._bid_size = default_bid_size
         self._ask_size = default_ask_size
         self._s2 = spread / 2.0
         self._d_session_start = daily_session_start_end[0]
         self._d_session_end = daily_session_start_end[1]
 
-    def start_processing(self, fieldnames: List[str]):
+    def start_processing(self, fieldnames: List[str], name: str | None = None):
         self._time_idx = _find_column_index_in_list(fieldnames, 'time', 'timestamp', 'datetime', 'date')
         self._open_idx = _find_column_index_in_list(fieldnames, 'open')
         self._high_idx = _find_column_index_in_list(fieldnames, 'high')
         self._low_idx = _find_column_index_in_list(fieldnames, 'low')
         self._close_idx = _find_column_index_in_list(fieldnames, 'close')
         self._volume_idx = None
         self._timeframe = None
@@ -122,15 +132,15 @@
         try:
             self._volume_idx = _find_column_index_in_list(fieldnames, 'volume', 'vol')
         except:
             pass
 
         self.buffer = []
 
-    def process_data(self, data: list) -> Optional[Iterable]:
+    def process_data_columns(self, data: list) -> Optional[Iterable]:
         s2 = self._s2
         if self._timeframe is None:
             _freq = infer_series_frequency(data[self._time_idx])
             self._timeframe = _freq.astype('timedelta64[s]')
 
             # - timestamps when we emit simulated quotes
             dt = _freq.astype('timedelta64[ns]').item()
@@ -197,65 +207,84 @@
         return self.buffer
 
 
 class OhlcvDataProcessor(DataProcessor):
     """
     Process data and convert it to Qube OHLCV timeseries 
     """
-    def __init__(self, name: str) -> None:
+    def __init__(self, name: str | None = None) -> None:
         super().__init__()
         self._name = name
 
-    def start_processing(self, fieldnames: List[str]):
+    def start_processing(self, fieldnames: List[str], name: str | None = None):
         self._time_idx = _find_column_index_in_list(fieldnames, 'time', 'timestamp', 'datetime', 'date')
         self._open_idx = _find_column_index_in_list(fieldnames, 'open')
         self._high_idx = _find_column_index_in_list(fieldnames, 'high')
         self._low_idx = _find_column_index_in_list(fieldnames, 'low')
         self._close_idx = _find_column_index_in_list(fieldnames, 'close')
         self._volume_idx = None
         self._b_volume_idx = None
         self._timeframe = None
+        self._name = name if name else self._name
 
         try:
             self._volume_idx = _find_column_index_in_list(fieldnames, 'quote_volume', 'volume', 'vol')
         except: pass
 
         try:
             self._b_volume_idx = _find_column_index_in_list(fieldnames, 'taker_buy_volume', 'taker_buy_quote_volume', 'buy_volume')
         except: pass
 
         self.ohlc = None
 
-    def process_data(self, data: list) -> Optional[Iterable]:
+    def process_data_columns(self, data: list) -> Optional[Iterable]:
         if self._timeframe is None:
             self._timeframe = infer_series_frequency(data[self._time_idx]).astype('timedelta64[s]')
 
             # - create instance after first data received
             self.ohlc = OHLCV(self._name, self._timeframe)
 
         self.ohlc.append_data(
             data[self._time_idx],
             data[self._open_idx], data[self._high_idx], data[self._low_idx], data[self._close_idx], 
             data[self._volume_idx] if self._volume_idx else np.empty(0),
             data[self._b_volume_idx] if self._b_volume_idx else np.empty(0)
         )
         return None
 
+    def process_data_rows(self, data: List[list]) -> Iterable | None:
+        if self._timeframe is None:
+            ts = [t[self._time_idx] for t in data[:100]]
+            self._timeframe = pd.Timedelta(infer_series_frequency(ts)).asm8.item()
+
+            # - create instance after first data received
+            self.ohlc = OHLCV(self._name, self._timeframe)
+
+        for d in data:
+            self.ohlc.update_by_bar(
+                np.datetime64(d[self._time_idx], 'ns').item(),
+                d[self._open_idx], d[self._high_idx], d[self._low_idx], d[self._close_idx], 
+                d[self._volume_idx] if self._volume_idx else 0,
+                d[self._b_volume_idx] if self._b_volume_idx else 0
+            )
+        return None
+
     def get_result(self) -> Any:
         return self.ohlc
 
 
 class OhlcvPandasDataProcessor(DataProcessor):
     """
     Process data and convert it to pandas OHLCV dataframes 
     """
     def __init__(self) -> None:
         super().__init__()
+        self._fieldnames: List = []
 
-    def start_processing(self, fieldnames: List[str]):
+    def start_processing(self, fieldnames: List[str], name: str | None = None):
         self._time_idx = _find_column_index_in_list(fieldnames, 'time', 'timestamp', 'datetime', 'date')
         self._open_idx = _find_column_index_in_list(fieldnames, 'open')
         self._high_idx = _find_column_index_in_list(fieldnames, 'high')
         self._low_idx = _find_column_index_in_list(fieldnames, 'low')
         self._close_idx = _find_column_index_in_list(fieldnames, 'close')
         self._volume_idx = None
         self._b_volume_idx = None
@@ -265,25 +294,31 @@
             self._volume_idx = _find_column_index_in_list(fieldnames, 'quote_volume', 'volume', 'vol')
         except: pass
 
         try:
             self._b_volume_idx = _find_column_index_in_list(fieldnames, 'taker_buy_volume', 'taker_buy_quote_volume', 'buy_volume')
         except: pass
 
-        # self.ohlc = pd.DataFrame()
-
         self._time = np.array([], dtype=np.datetime64)
         self._open = np.array([])
         self._high = np.array([])
         self._low = np.array([])
         self._close = np.array([])
         self._volume = np.array([])
         self._bvolume = np.array([])
+        self._fieldnames = fieldnames
+        self._ohlc = pd.DataFrame()
+
+    def process_data_rows(self, data: List[list]) -> Optional[Iterable]:
+        p = pd.DataFrame.from_records(data, columns=self._fieldnames)
+        p.set_index(self._fieldnames[self._time_idx], drop=True, inplace=True)
+        self._ohlc = pd.concat((self._ohlc, p), axis=0, sort=True, copy=True)
+        return None
 
-    def process_data(self, data: list) -> Optional[Iterable]:
+    def process_data_columns(self, data: list) -> Optional[Iterable]:
         # p = pd.DataFrame({
         #     'open': data[self._open_idx], 
         #     'high': data[self._high_idx], 
         #     'low': data[self._low_idx], 
         #     'close': data[self._close_idx], 
         #     'volume': data[self._volume_idx] if self._volume_idx else []},
         #     index = data[self._time_idx]
@@ -298,14 +333,17 @@
             self._volume = np.concatenate((self._volume, data[self._volume_idx]))
         if self._b_volume_idx:
             self._bvolume = np.concatenate((self._bvolume, data[self._b_volume_idx]))
 
         return None
 
     def get_result(self) -> Any:
+        if not self._ohlc.empty:
+            return self._ohlc
+
         rd = {
             'open': self._open, 'high': self._high, 'low': self._low, 'close': self._close, 
         }
 
         if self._volume_idx:
             rd['volume'] = self._volume
 
@@ -388,10 +426,90 @@
         selected_table = table.slice(start_idx, length)
         n_chunks = selected_table[table.column_names[0]].num_chunks
         for n in range(n_chunks):
             data = [
                 # - in some cases we need to convert time index to primitive type
                 _time_cast_function(selected_table[k].chunk(n)).to_numpy() if k == _time_field_idx else selected_table[k].chunk(n).to_numpy()
                 for k in range(selected_table.num_columns)]
-            self._processor.process_data(data)
+            self._processor.process_data_columns(data)
         return self._processor.get_result()
-            
+
+
+def _retry(fn):
+    @wraps(fn)
+    def wrapper(*args, **kw):
+        cls = args[0]
+        for x in range(cls._reconnect_tries):
+            # print(x, cls._reconnect_tries)
+            try:
+                return fn(*args, **kw)
+            except (pg.InterfaceError, pg.OperationalError) as e:
+                logger.warning("Database Connection [InterfaceError or OperationalError]")
+                # print ("Idle for %s seconds" % (cls._reconnect_idle))
+                # time.sleep(cls._reconnect_idle)
+                cls._connect()
+    return wrapper
+
+
+class QuestDBConnector(DataReader):
+    """
+    Very first version of QuestDB connector
+
+    # Connect to an existing QuestDB instance
+    >>> db = QuestDBConnector('user=admin password=quest host=localhost port=8812', OhlcvPandasDataProcessor())
+    >>> db.read('BINANCEF.ETHUSDT', '5m', '2024-01-01')
+    """
+    _reconnect_tries = 5
+    _reconnect_idle = 0.1  # wait seconds before retying
+
+    def __init__(self, connection_url: str, processor: DataProcessor | None=None) -> None:
+        super().__init__(processor)
+        self._connection = None
+        self._cursor = None
+        self.connection_url = connection_url
+        self._connect()
+
+    def _connect(self):
+        logger.info("Connecting to QuestDB ...")
+        self._connection = pg.connect(self.connection_url, autocommit=True)
+        self._cursor = self._connection.cursor()
+
+    @_retry
+    def read(self, symbol: str, timeframe: str, start: str|None=None, stop: str|None=None) -> Any:
+        start, end = handle_start_stop(start, stop)
+        w0 = f"timestamp >= '{start}'" if start else ''
+        w1 = f"timestamp <= '{end}'" if end else ''
+        where = f'where {w0} and {w1}' if (w0 and w1) else f"where {(w0 or w1)}"
+
+        self._cursor.execute(
+            f"""
+                select timestamp, 
+                first(open) as open, 
+                max(high) as high,
+                min(low) as low,
+                last(close) as close,
+                sum(volume) as volume,
+                sum(quote_volume) as quote_volume,
+                sum(count) as count,
+                sum(taker_buy_volume) as taker_buy_volume,
+                sum(taker_buy_quote_volume) as taker_buy_quote_volume
+                from "{symbol.upper()}" {where}
+                SAMPLE by {timeframe};
+            """ # type: ignore
+        )
+        records = self._cursor.fetchall()
+        names = [d.name for d in self._cursor.description]
+
+        self._processor.start_processing(names, re.split(r'[.:]', symbol)[-1])
+        
+        # d = np.array(records)
+        self._processor.process_data_rows(records)
+        return self._processor.get_result()
+
+    def __del__(self):
+        for c in (self._cursor, self._connection):
+            try:
+                logger.info("Closing connection")
+                c.close()
+            except:
+                pass
+
```

### Comparing `qubx-0.1.0/src/qubx/impl/ccxt_connector.py` & `qubx-0.1.3/src/qubx/impl/ccxt_connector.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 import re
 import pandas as pd
 
 from qubx import logger
 from qubx.core.basics import Instrument, Position, dt_64, Deal
 from qubx.core.strategy import IDataProvider, CtrlChannel, IExchangeServiceProvider
 from qubx.core.series import TimeSeries, Bar, Trade, Quote
-from qubx.impl.utils import DATA_PROVIDERS_ALIASES
+from qubx.impl.ccxt_utils import DATA_PROVIDERS_ALIASES
 
 from .ccxt_trading import CCXTSyncTradingConnector
 
 # - register custom wrappers
-from .exchange_customizations import BinanceQV
+from .ccxt_customizations import BinanceQV
 cxp.binanceqv = BinanceQV            # type: ignore
 cxp.exchanges.append('binanceqv')
 
 
 class CCXTConnector(IDataProvider, CCXTSyncTradingConnector):
     _exchange: Exchange
     _subsriptions: Dict[str, List[str]]
@@ -47,15 +47,15 @@
 
         # - create new even loop
         self._loop = asyncio.new_event_loop()
         asyncio.set_event_loop(self._loop)
 
         # - create exchange's instance
         self._exchange = getattr(cxp, exch)(exchange_auth | {'asyncio_loop': self._loop})
-        self._ch_market_data = CtrlChannel(exch + '.marketdata', sent=(None, None, None))
+        self._ch_market_data = CtrlChannel(exch + '.marketdata', sentinel=(None, None, None))
         self._last_quotes = defaultdict(lambda: None)
         self._subsriptions: Dict[str, List[str]] = defaultdict(list)
 
         logger.info(f"{self.get_name().upper()} initialized - current time {self.time()}")
 
     def subscribe(self, subscription_type: str, symbols: List[str], timeframe:Optional[str]=None, nback:int=0) -> bool:
         to_process = self._check_existing_subscription(subscription_type.lower(), symbols)
@@ -105,20 +105,22 @@
             if s not in subscribed:
                 to_subscribe.append(s)
         return to_subscribe
 
     def _time_msec_nbars_back(self, timeframe: str, nbarsback: int) -> int:
         return (self.time() - nbarsback * pd.Timedelta(timeframe)).asm8.item() // 1000000
 
-    def get_historical_ohlcs(self, symbol: str, timeframe: str, nbarsback: int) -> Optional[List[Bar]]:
+    def get_historical_ohlcs(self, symbol: str, timeframe: str, nbarsback: int) -> List[Bar]:
         assert nbarsback >= 1
         since = self._time_msec_nbars_back(timeframe, nbarsback)
 
         # - get this from sync 
-        res = self.sync.fetch_ohlcv(symbol, self._get_exch_timeframe(timeframe), since=since)
+        # - TODO: check if nbarsback > max_limit (1000) we need to do more requests
+        # - TODO: how to get quoted volumes ?
+        res = self.sync.fetch_ohlcv(symbol, self._get_exch_timeframe(timeframe), since=since, limit=1000)
         _arr = []  
         for oh in res: # type: ignore
             _arr.append(
                 Bar(oh[0] * 1_000_000, oh[1], oh[2], oh[3], oh[4], oh[6], oh[7]) 
                 if len(oh) > 6 else 
                 Bar(oh[0] * 1_000_000, oh[1], oh[2], oh[3], oh[4], oh[5]) 
             )
```

### Comparing `qubx-0.1.0/src/qubx/impl/ccxt_trading.py` & `qubx-0.1.3/src/qubx/impl/ccxt_trading.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import pandas as pd
 
 from qubx import logger, lookup
 from qubx.core.account import AccountProcessor
 from qubx.core.basics import Instrument, Position, Order, TransactionCostsCalculator, dt_64, Deal
 from qubx.core.strategy import IDataProvider, CtrlChannel, IExchangeServiceProvider
 from qubx.core.series import TimeSeries, Bar, Trade, Quote
-from qubx.impl.utils import EXCHANGE_ALIASES, ccxt_convert_order_info, ccxt_convert_deal_info, ccxt_extract_deals_from_exec, ccxt_restore_position_from_deals
+from qubx.impl.ccxt_utils import EXCHANGE_ALIASES, ccxt_convert_order_info, ccxt_convert_deal_info, ccxt_extract_deals_from_exec, ccxt_restore_position_from_deals
 
 
 ORDERS_HISTORY_LOOKBACK_DAYS = 30
 
 
 class CCXTSyncTradingConnector(IExchangeServiceProvider):
     """
```

### Comparing `qubx-0.1.0/src/qubx/impl/exchange_customizations.py` & `qubx-0.1.3/src/qubx/impl/ccxt_customizations.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.0/src/qubx/impl/utils.py` & `qubx-0.1.3/src/qubx/impl/ccxt_utils.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.0/src/qubx/math/stats.py` & `qubx-0.1.3/src/qubx/math/stats.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.0/src/qubx/ta/indicators.pyx` & `qubx-0.1.3/src/qubx/ta/indicators.pyx`

 * *Files identical despite different names*

### Comparing `qubx-0.1.0/src/qubx/trackers/rebalancers.py` & `qubx-0.1.3/src/qubx/trackers/rebalancers.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.0/src/qubx/utils/_pyxreloader.py` & `qubx-0.1.3/src/qubx/utils/_pyxreloader.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.0/src/qubx/utils/marketdata/binance.py` & `qubx-0.1.3/src/qubx/utils/marketdata/binance.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.0/src/qubx/utils/misc.py` & `qubx-0.1.3/src/qubx/utils/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     :return: environment name, possible values:
              - 'notebook' jupyter notebook
              - 'shell' any interactive shell (ipython, PyCharm's console etc)
              - 'python' standard python interpreter
              - 'unknown' can't recognize environment
     """
     try:
-        from IPython import get_ipython
+        from IPython.core.getipython import get_ipython
         shell = get_ipython().__class__.__name__
 
         if shell == 'ZMQInteractiveShell':  # Jupyter notebook or qtconsole
             return 'notebook'
         elif shell.endswith('TerminalInteractiveShell'):  # Terminal running IPython
             return 'shell'
         else:
```

### Comparing `qubx-0.1.0/src/qubx/utils/pandas.py` & `qubx-0.1.3/src/qubx/utils/pandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
     """
     if not isinstance(data, dict):
         raise ValueError('Data must be passed as dictionary')
 
     return pd.concat([data[k][columns] for k in data.keys()], axis=1, keys=data.keys())
 
 
-def continuous_periods(xs, cond) -> Struct:
+def continuous_periods(xs: pd.Series, cond: pd.Series) -> Struct:
     """
     Detect continues periods on series xs based on condition cond
     """
     df = scols(xs, cond, keys=['_XS_', 'sig'])
     df['block'] = (df.sig.shift(1) != df.sig).astype(int).cumsum()
     idx_col_name = xs.index.name
```

### Comparing `qubx-0.1.0/src/qubx/utils/runner.py` & `qubx-0.1.3/src/qubx/utils/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,38 +16,55 @@
     components = name.split('.')
     clz = components[-1]
     mod = __import__('.'.join(components[:-1]), fromlist=[clz])
     mod = getattr(mod, clz)
     return mod
 
 
+def _instruments_for_exchange(exch: str, symbols: list) -> list:
+    instrs = []
+    for s in symbols:
+        instr = lookup.find_symbol(exch.upper(), s.upper()) 
+        if instr is not None:
+            instrs.append(instr)
+        else:
+            logger.warning(f"Can't find instrument for symbol {s} - try to refresh lookup first !")
+    return instrs
+
+
 def load_strategy_config(filename: str) -> Struct:
     with open(filename, 'r') as f:
         content = yaml.safe_load(f)
 
     config = content['config']
-    execution = config['execution']
     strat = config['strategy']
     name = strat.split('.')[-1]
     r = Struct(
         strategy = strat,
         name = name,
         parameters = config.get('parameters', dict()),
-        connector = execution['connector'],
-        exchange = execution['exchange'],
-        account = execution.get('account'),
-        md_subscr = execution['subscription'],
-        strategy_trigger = execution['trigger'],
+        connector = config['connector'],
+        exchange = config['exchange'],
+        account = config.get('account'),
+        md_subscr = config['subscription'],
+        strategy_trigger = config['trigger'],
+        strategy_fit_trigger = config.get('fit', ''),
         portfolio_logger = config.get('logger', None),
         log_positions_interval = config.get('log_positions_interval', None),
         log_portfolio_interval = config.get('log_portfolio_interval', None)
     )
 
-    universe = execution['universe']
-    r.instruments = [lookup.find_symbol(r.exchange.upper(), s.upper()) for s in universe ]
+    universe = config['universe']
+    if isinstance(universe, dict):
+        r.instruments = []
+        for e, symbs in universe.items():
+            r.instruments.extend(_instruments_for_exchange(e, symbs))
+    else:
+       r.instruments = _instruments_for_exchange(r.exchange, universe)
+
     return r
 
 
 def get_account_config(account_id: str, accounts_cfg_file: str) -> dict | None:
     parser = configparser.ConfigParser()
     try:
         parser.optionxform=str  # type: ignore
@@ -117,20 +134,21 @@
         except Exception as err:
             logger.warning(f"Can't instantiate specified writer {_w_class}: {str(err)}")
             writer = LogsWriter(acc_config['account_id'], strategy.__name__, run_id)
         
     logger.info(f""" - - - <blue>Qubx</blue> (ver. <red>{version()}</red>) - - -\n - Strategy: {strategy}\n - Config: {cfg.parameters} """)
     ctx = StrategyContext(
         strategy, cfg.parameters, connector, connector, 
-        instruments=cfg.instruments, 
-        md_subscription=cfg.md_subscr, 
-        trigger=cfg.strategy_trigger,
-        logs_writer=writer, 
-        positions_log_freq=cfg.log_positions_interval,
-        portfolio_log_freq=cfg.log_portfolio_interval
+        instruments        = cfg.instruments, 
+        md_subscription    = cfg.md_subscr, 
+        trigger_spec       = cfg.strategy_trigger,
+        fit_spec           = cfg.strategy_fit_trigger,
+        logs_writer        = writer, 
+        positions_log_freq = cfg.log_positions_interval,
+        portfolio_log_freq = cfg.log_portfolio_interval
     )
  
     return ctx
 
 
 def _run_in_jupyter(filename: str, accounts: str, paths: list):
     """
```

### Comparing `qubx-0.1.0/src/qubx/utils/time.py` & `qubx-0.1.3/src/qubx/utils/time.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re
 
 import pandas as pd
 
 UNIX_T0 = np.datetime64('1970-01-01T00:00:00')
 
 
-time_to_str = lambda t, u='us': np.datetime_as_string(t if isinstance(t, np.datetime64) else np.datetime64(t, u), unit=u)
+time_to_str = lambda t, u='us': np.datetime_as_string(t if isinstance(t, np.datetime64) else np.datetime64(t, u), unit=u) # type: ignore
 
 
 def convert_tf_str_td64(c_tf: str) -> np.timedelta64:
     """
     Convert string timeframe to timedelta64
 
     '15Min' -> timedelta64(15, 'm') etc
@@ -37,28 +37,41 @@
             unit = u2
 
         _dt += np.timedelta64(n, unit)
     
     return _dt
 
 
-def convert_seconds_to_str(seconds: int) -> str:
+def convert_seconds_to_str(seconds: int, convert_months=False) -> str:
     """
     Convert seconds to string representation: 310 -> '5Min10S' etc
     """
-    days, seconds = divmod(seconds, 86400)
-    hours, seconds = divmod(seconds, 3600)
-    minutes, seconds = divmod(seconds, 60)
     r = ''
+
+    if convert_months:
+        months, seconds = divmod(seconds, 4*7*86400)
+        if months > 0:
+            r += '%dmonth' % months
+
+    weeks, seconds = divmod(seconds, 7*86400)
+    if weeks > 0:
+        r += '%dw' % weeks
+
+    days, seconds = divmod(seconds, 86400)
     if days > 0:
-        r += '%dD' % days
+        r += '%dd' % days
+
+    hours, seconds = divmod(seconds, 3600)
     if hours > 0:
-        r += '%dH' % hours
+        r += '%dh' % hours
+
+    minutes, seconds = divmod(seconds, 60)
     if minutes > 0:
         r += '%dMin' % minutes
+
     if seconds > 0:
         r += '%dS' % seconds
     return r
 
 
 def floor_t64(time: Union[np.datetime64, datetime], dt: Union[np.timedelta64, int, str]):
     """
@@ -91,15 +104,15 @@
         times_index = series
     else:
         raise ValueError("Can't recognize input data")
 
     if times_index.shape[0] < 2:
         raise ValueError("Series must have at least 2 points to determ frequency")
 
-    values = np.array(sorted([(x if isinstance(x, np.timedelta64) else x.total_seconds()) for x in np.abs(np.diff(times_index))]))
+    values = np.array(sorted([(x if isinstance(x, np.timedelta64) else int(1e9 * x.total_seconds())) for x in np.abs(np.diff(times_index))]))
     diff = np.concatenate(([1], np.diff(values)))
     idx = np.concatenate((np.where(diff)[0], [len(values)]))
     freqs = dict(zip(values[idx[:-1]], np.diff(idx)))
     return np.timedelta64(max(freqs, key=freqs.get))
 
 
 def handle_start_stop(s: Optional[str], e: Optional[str], convert=str) -> tuple:
```

### Comparing `qubx-0.1.0/PKG-INFO` & `qubx-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: Qubx
-Version: 0.1.0
+Version: 0.1.3
 Summary: Qubx - quantitative trading framework
 Home-page: https://github.com/dmarienko/Qubx
 Author: Dmitry Marienko
 Author-email: dmitry@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ccxt (>=4.2.68,<5.0.0)
+Requires-Dist: croniter (>=2.0.5,<3.0.0)
 Requires-Dist: cython (==3.0.8)
 Requires-Dist: importlib-metadata
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: ntplib (>=0.4.0,<0.5.0)
 Requires-Dist: numpy (>=1.26.3,<2.0.0)
+Requires-Dist: psycopg (>=3.1.18,<4.0.0)
 Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pymongo (>=4.6.1,<5.0.0)
 Requires-Dist: pytest[lazyfixture] (>=7.2.0,<8.0.0)
 Requires-Dist: python-binance (>=1.0.19,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: scipy (>=1.12.0,<2.0.0)
```

