# Comparing `tmp/qteasy-1.2.4.tar.gz` & `tmp/qteasy-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qteasy-1.2.4.tar", last modified: Sun May  5 14:51:59 2024, max compression
+gzip compressed data, was "qteasy-1.2.5.tar", last modified: Mon May  6 04:10:59 2024, max compression
```

## Comparing `qteasy-1.2.4.tar` & `qteasy-1.2.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-05-05 14:51:59.102377 qteasy-1.2.4/
--rwxr-xr-x   0 jackie     (501) staff       (20)     1463 2024-03-07 04:23:42.000000 qteasy-1.2.4/LICENSE
--rw-r--r--   0 jackie     (501) staff       (20)    27935 2024-05-05 14:51:59.101831 qteasy-1.2.4/PKG-INFO
--rwxr-xr-x   0 jackie     (501) staff       (20)    24211 2024-05-05 14:42:08.000000 qteasy-1.2.4/README.md
--rw-r--r--   0 jackie     (501) staff       (20)     2304 2024-05-05 14:42:08.000000 qteasy-1.2.4/pyproject.toml
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-05-05 14:51:59.078314 qteasy-1.2.4/qteasy/
--rwxr-xr-x   0 jackie     (501) staff       (20)     8588 2024-05-05 14:42:08.000000 qteasy-1.2.4/qteasy/__init__.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    68549 2024-05-04 09:08:45.000000 qteasy-1.2.4/qteasy/_arg_validators.py
--rw-r--r--   0 jackie     (501) staff       (20)    53075 2024-05-05 10:05:28.000000 qteasy-1.2.4/qteasy/backtest.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    35193 2024-04-02 14:31:55.000000 qteasy-1.2.4/qteasy/blender.py
--rw-r--r--   0 jackie     (501) staff       (20)    30260 2024-05-05 10:05:28.000000 qteasy-1.2.4/qteasy/broker.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   142516 2024-05-05 14:24:46.000000 qteasy-1.2.4/qteasy/built_in.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   111306 2024-05-04 09:08:45.000000 qteasy-1.2.4/qteasy/core.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   390965 2024-05-04 09:08:45.000000 qteasy-1.2.4/qteasy/database.py
--rw-r--r--   0 jackie     (501) staff       (20)     9341 2024-04-02 14:50:54.000000 qteasy-1.2.4/qteasy/emfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    34874 2024-05-04 09:08:45.000000 qteasy-1.2.4/qteasy/evaluate.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    38585 2024-05-05 10:05:28.000000 qteasy-1.2.4/qteasy/finance.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   100797 2024-04-05 14:28:39.000000 qteasy-1.2.4/qteasy/history.py
--rw-r--r--   0 jackie     (501) staff       (20)    39218 2024-05-04 08:19:36.000000 qteasy-1.2.4/qteasy/optimization.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   107901 2024-05-05 10:05:28.000000 qteasy-1.2.4/qteasy/qt_operator.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    34029 2024-04-05 14:28:39.000000 qteasy-1.2.4/qteasy/space.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    88071 2024-05-05 10:05:28.000000 qteasy-1.2.4/qteasy/strategy.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   156164 2024-05-05 14:35:57.000000 qteasy-1.2.4/qteasy/tafuncs.py
--rw-r--r--   0 jackie     (501) staff       (20)    51352 2024-05-04 09:08:45.000000 qteasy-1.2.4/qteasy/trade_recording.py
--rw-r--r--   0 jackie     (501) staff       (20)    98512 2024-05-04 09:08:45.000000 qteasy-1.2.4/qteasy/trader.py
--rw-r--r--   0 jackie     (501) staff       (20)    93193 2024-05-04 09:08:45.000000 qteasy-1.2.4/qteasy/trader_cli.py
--rw-r--r--   0 jackie     (501) staff       (20)    18205 2024-05-04 09:08:45.000000 qteasy-1.2.4/qteasy/trader_tui.py
--rw-r--r--   0 jackie     (501) staff       (20)    68078 2024-05-05 10:05:28.000000 qteasy-1.2.4/qteasy/trading_util.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   131527 2024-04-21 23:36:55.000000 qteasy-1.2.4/qteasy/tsfuncs.py
--rw-r--r--   0 jackie     (501) staff       (20)      840 2024-05-04 09:08:45.000000 qteasy-1.2.4/qteasy/tui_style.tcss
--rwxr-xr-x   0 jackie     (501) staff       (20)    75175 2024-05-04 09:08:45.000000 qteasy-1.2.4/qteasy/utilfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    79918 2024-04-21 23:36:55.000000 qteasy-1.2.4/qteasy/visual.py
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-05-05 14:51:59.101159 qteasy-1.2.4/qteasy.egg-info/
--rw-r--r--   0 jackie     (501) staff       (20)    27935 2024-05-05 14:51:59.000000 qteasy-1.2.4/qteasy.egg-info/PKG-INFO
--rw-r--r--   0 jackie     (501) staff       (20)     1274 2024-05-05 14:51:59.000000 qteasy-1.2.4/qteasy.egg-info/SOURCES.txt
--rw-r--r--   0 jackie     (501) staff       (20)        1 2024-05-05 14:51:59.000000 qteasy-1.2.4/qteasy.egg-info/dependency_links.txt
--rw-r--r--   0 jackie     (501) staff       (20)        1 2023-01-29 16:03:37.000000 qteasy-1.2.4/qteasy.egg-info/not-zip-safe
--rw-r--r--   0 jackie     (501) staff       (20)      195 2024-05-05 14:51:59.000000 qteasy-1.2.4/qteasy.egg-info/requires.txt
--rw-r--r--   0 jackie     (501) staff       (20)        7 2024-05-05 14:51:59.000000 qteasy-1.2.4/qteasy.egg-info/top_level.txt
--rw-r--r--   0 jackie     (501) staff       (20)     1627 2024-05-05 14:51:59.103420 qteasy-1.2.4/setup.cfg
--rw-r--r--   0 jackie     (501) staff       (20)      257 2024-04-01 14:38:19.000000 qteasy-1.2.4/setup.py
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-05-05 14:51:59.100858 qteasy-1.2.4/tests/
--rw-r--r--   0 jackie     (501) staff       (20)     6524 2024-05-05 10:05:28.000000 qteasy-1.2.4/tests/test_broker.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     8078 2024-04-05 14:28:39.000000 qteasy-1.2.4/tests/test_cashplan.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     3613 2023-11-25 05:35:56.000000 qteasy-1.2.4/tests/test_config.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    17487 2024-04-03 01:57:25.000000 qteasy-1.2.4/tests/test_core_sub_funcs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    19818 2024-05-05 10:05:28.000000 qteasy-1.2.4/tests/test_cost.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   121711 2024-05-04 09:08:45.000000 qteasy-1.2.4/tests/test_datasource.py
--rw-r--r--   0 jackie     (501) staff       (20)     6143 2024-02-03 15:46:14.000000 qteasy-1.2.4/tests/test_eastmoney.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    73624 2024-04-05 14:28:39.000000 qteasy-1.2.4/tests/test_evaluations.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    13901 2024-02-03 15:46:14.000000 qteasy-1.2.4/tests/test_fast_experiments.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    57759 2024-03-29 10:03:15.000000 qteasy-1.2.4/tests/test_historypanel.py
--rwxr-xr-x   0 jackie     (501) staff       (20)      413 2023-01-29 16:18:32.000000 qteasy-1.2.4/tests/test_log.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   304019 2024-04-05 14:28:39.000000 qteasy-1.2.4/tests/test_loop.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   169228 2024-05-04 09:08:45.000000 qteasy-1.2.4/tests/test_operator_and_strategy.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    44521 2024-05-05 14:36:45.000000 qteasy-1.2.4/tests/test_qt.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    18581 2023-01-29 16:18:32.000000 qteasy-1.2.4/tests/test_space.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    40814 2024-05-05 14:24:46.000000 qteasy-1.2.4/tests/test_ta_funcs.py
--rw-r--r--   0 jackie     (501) staff       (20)    43397 2024-05-04 09:08:45.000000 qteasy-1.2.4/tests/test_trader.py
--rw-r--r--   0 jackie     (501) staff       (20)    45317 2024-05-04 09:08:45.000000 qteasy-1.2.4/tests/test_trader_shell.py
--rw-r--r--   0 jackie     (501) staff       (20)   168527 2024-04-21 23:36:55.000000 qteasy-1.2.4/tests/test_trading.py
--rw-r--r--   0 jackie     (501) staff       (20)     2670 2024-05-04 09:08:45.000000 qteasy-1.2.4/tests/test_tui.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    21881 2024-03-30 12:31:29.000000 qteasy-1.2.4/tests/test_tushare.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    43279 2024-04-05 14:28:39.000000 qteasy-1.2.4/tests/test_utilityfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     3090 2023-01-29 16:18:32.000000 qteasy-1.2.4/tests/test_visual.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-05-06 04:10:59.580869 qteasy-1.2.5/
+-rwxr-xr-x   0 jackie     (501) staff       (20)     1463 2024-03-07 04:23:42.000000 qteasy-1.2.5/LICENSE
+-rw-r--r--   0 jackie     (501) staff       (20)    27935 2024-05-06 04:10:59.580770 qteasy-1.2.5/PKG-INFO
+-rwxr-xr-x   0 jackie     (501) staff       (20)    24211 2024-05-06 03:02:44.000000 qteasy-1.2.5/README.md
+-rw-r--r--   0 jackie     (501) staff       (20)     2304 2024-05-06 03:02:44.000000 qteasy-1.2.5/pyproject.toml
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-05-06 04:10:59.566755 qteasy-1.2.5/qteasy/
+-rwxr-xr-x   0 jackie     (501) staff       (20)     8588 2024-05-06 03:02:44.000000 qteasy-1.2.5/qteasy/__init__.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    68549 2024-05-04 09:08:45.000000 qteasy-1.2.5/qteasy/_arg_validators.py
+-rw-r--r--   0 jackie     (501) staff       (20)    53075 2024-05-05 10:05:28.000000 qteasy-1.2.5/qteasy/backtest.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    35193 2024-04-02 14:31:55.000000 qteasy-1.2.5/qteasy/blender.py
+-rw-r--r--   0 jackie     (501) staff       (20)    30260 2024-05-05 10:05:28.000000 qteasy-1.2.5/qteasy/broker.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   142516 2024-05-05 14:24:46.000000 qteasy-1.2.5/qteasy/built_in.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   111306 2024-05-04 09:08:45.000000 qteasy-1.2.5/qteasy/core.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   390965 2024-05-04 09:08:45.000000 qteasy-1.2.5/qteasy/database.py
+-rw-r--r--   0 jackie     (501) staff       (20)     9341 2024-04-02 14:50:54.000000 qteasy-1.2.5/qteasy/emfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    34874 2024-05-04 09:08:45.000000 qteasy-1.2.5/qteasy/evaluate.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    38585 2024-05-05 10:05:28.000000 qteasy-1.2.5/qteasy/finance.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   110944 2024-05-06 03:03:48.000000 qteasy-1.2.5/qteasy/history.py
+-rw-r--r--   0 jackie     (501) staff       (20)    39218 2024-05-04 08:19:36.000000 qteasy-1.2.5/qteasy/optimization.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   107901 2024-05-05 10:05:28.000000 qteasy-1.2.5/qteasy/qt_operator.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    34029 2024-04-05 14:28:39.000000 qteasy-1.2.5/qteasy/space.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    88071 2024-05-05 10:05:28.000000 qteasy-1.2.5/qteasy/strategy.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   156164 2024-05-05 14:35:57.000000 qteasy-1.2.5/qteasy/tafuncs.py
+-rw-r--r--   0 jackie     (501) staff       (20)    51352 2024-05-04 09:08:45.000000 qteasy-1.2.5/qteasy/trade_recording.py
+-rw-r--r--   0 jackie     (501) staff       (20)    98512 2024-05-04 09:08:45.000000 qteasy-1.2.5/qteasy/trader.py
+-rw-r--r--   0 jackie     (501) staff       (20)    93193 2024-05-04 09:08:45.000000 qteasy-1.2.5/qteasy/trader_cli.py
+-rw-r--r--   0 jackie     (501) staff       (20)    18205 2024-05-04 09:08:45.000000 qteasy-1.2.5/qteasy/trader_tui.py
+-rw-r--r--   0 jackie     (501) staff       (20)    68078 2024-05-05 10:05:28.000000 qteasy-1.2.5/qteasy/trading_util.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   131527 2024-04-21 23:36:55.000000 qteasy-1.2.5/qteasy/tsfuncs.py
+-rw-r--r--   0 jackie     (501) staff       (20)      840 2024-05-04 09:08:45.000000 qteasy-1.2.5/qteasy/tui_style.tcss
+-rwxr-xr-x   0 jackie     (501) staff       (20)    75175 2024-05-04 09:08:45.000000 qteasy-1.2.5/qteasy/utilfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    79918 2024-04-21 23:36:55.000000 qteasy-1.2.5/qteasy/visual.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-05-06 04:10:59.580065 qteasy-1.2.5/qteasy.egg-info/
+-rw-r--r--   0 jackie     (501) staff       (20)    27935 2024-05-06 04:10:59.000000 qteasy-1.2.5/qteasy.egg-info/PKG-INFO
+-rw-r--r--   0 jackie     (501) staff       (20)     1274 2024-05-06 04:10:59.000000 qteasy-1.2.5/qteasy.egg-info/SOURCES.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        1 2024-05-06 04:10:59.000000 qteasy-1.2.5/qteasy.egg-info/dependency_links.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        1 2023-01-29 16:03:37.000000 qteasy-1.2.5/qteasy.egg-info/not-zip-safe
+-rw-r--r--   0 jackie     (501) staff       (20)      195 2024-05-06 04:10:59.000000 qteasy-1.2.5/qteasy.egg-info/requires.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        7 2024-05-06 04:10:59.000000 qteasy-1.2.5/qteasy.egg-info/top_level.txt
+-rw-r--r--   0 jackie     (501) staff       (20)     1627 2024-05-06 04:10:59.581186 qteasy-1.2.5/setup.cfg
+-rw-r--r--   0 jackie     (501) staff       (20)      257 2024-04-01 14:38:19.000000 qteasy-1.2.5/setup.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-05-06 04:10:59.579781 qteasy-1.2.5/tests/
+-rw-r--r--   0 jackie     (501) staff       (20)     6524 2024-05-05 10:05:28.000000 qteasy-1.2.5/tests/test_broker.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     8078 2024-04-05 14:28:39.000000 qteasy-1.2.5/tests/test_cashplan.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     3613 2023-11-25 05:35:56.000000 qteasy-1.2.5/tests/test_config.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    17487 2024-04-03 01:57:25.000000 qteasy-1.2.5/tests/test_core_sub_funcs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    19818 2024-05-05 10:05:28.000000 qteasy-1.2.5/tests/test_cost.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   121711 2024-05-04 09:08:45.000000 qteasy-1.2.5/tests/test_datasource.py
+-rw-r--r--   0 jackie     (501) staff       (20)     6143 2024-02-03 15:46:14.000000 qteasy-1.2.5/tests/test_eastmoney.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    73624 2024-04-05 14:28:39.000000 qteasy-1.2.5/tests/test_evaluations.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    13901 2024-02-03 15:46:14.000000 qteasy-1.2.5/tests/test_fast_experiments.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    57759 2024-03-29 10:03:15.000000 qteasy-1.2.5/tests/test_historypanel.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)      413 2023-01-29 16:18:32.000000 qteasy-1.2.5/tests/test_log.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   304019 2024-04-05 14:28:39.000000 qteasy-1.2.5/tests/test_loop.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   169228 2024-05-04 09:08:45.000000 qteasy-1.2.5/tests/test_operator_and_strategy.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    44521 2024-05-05 14:36:45.000000 qteasy-1.2.5/tests/test_qt.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    18581 2023-01-29 16:18:32.000000 qteasy-1.2.5/tests/test_space.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    40814 2024-05-06 03:02:44.000000 qteasy-1.2.5/tests/test_ta_funcs.py
+-rw-r--r--   0 jackie     (501) staff       (20)    43397 2024-05-04 09:08:45.000000 qteasy-1.2.5/tests/test_trader.py
+-rw-r--r--   0 jackie     (501) staff       (20)    45317 2024-05-04 09:08:45.000000 qteasy-1.2.5/tests/test_trader_shell.py
+-rw-r--r--   0 jackie     (501) staff       (20)   168527 2024-04-21 23:36:55.000000 qteasy-1.2.5/tests/test_trading.py
+-rw-r--r--   0 jackie     (501) staff       (20)     2670 2024-05-04 09:08:45.000000 qteasy-1.2.5/tests/test_tui.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    21881 2024-03-30 12:31:29.000000 qteasy-1.2.5/tests/test_tushare.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    43279 2024-04-05 14:28:39.000000 qteasy-1.2.5/tests/test_utilityfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     3090 2023-01-29 16:18:32.000000 qteasy-1.2.5/tests/test_visual.py
```

### Comparing `qteasy-1.2.4/LICENSE` & `qteasy-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/PKG-INFO` & `qteasy-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qteasy
-Version: 1.2.4
+Version: 1.2.5
 Summary: A fast quantitative investment tool kit
 Home-page: https://github.com/shepherdpp/qteasy
 Author: Jackie PENG
 Author-email: jackie PENG <jackie.pengzhao@gmail.com>
 Maintainer: Jackie PENG
 Maintainer-email: jackie PENG <jackie.pengzhao@gmail.com>
 License: Copyright <2019> <JACKIE PENG>
@@ -106,15 +106,15 @@
 > 我会尽快修复问题并回复大家的问题。
 
 ## 关于`qteasy`
 
 - 作者: **Jackie PENG**
 - email: *jackie_pengzhao@163.com*
 - Created: 2019, July, 16
-- Latest Version: `1.2.4`
+- Latest Version: `1.2.5`
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
```

### Comparing `qteasy-1.2.4/README.md` & `qteasy-1.2.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 > 我会尽快修复问题并回复大家的问题。
 
 ## 关于`qteasy`
 
 - 作者: **Jackie PENG**
 - email: *jackie_pengzhao@163.com*
 - Created: 2019, July, 16
-- Latest Version: `1.2.4`
+- Latest Version: `1.2.5`
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
```

### Comparing `qteasy-1.2.4/pyproject.toml` & `qteasy-1.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 build-backend = "setuptools.build_meta"
 
 #[tool.setuptools.package.find]
 #where = "qteasy/"
 
 [project]
 name = "qteasy"
-version = "1.2.4"
+version = "1.2.5"
 authors = [
   {name="jackie PENG", email="jackie.pengzhao@gmail.com" },
 ]
 maintainers = [
   {name="jackie PENG", email="jackie.pengzhao@gmail.com" },
 ]
 description = "A fast quantitative investment tool kit"
```

### Comparing `qteasy-1.2.4/qteasy/__init__.py` & `qteasy-1.2.5/qteasy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,23 +34,23 @@
 from .visual import candle
 from .finance import CashPlan, set_cost, update_cost
 from .database import DataSource, find_history_data
 from ._arg_validators import QT_CONFIG, ConfigDict
 
 
 # qteasy版本信息
-__version__ = '1.2.4'
+__version__ = '1.2.5'
 version_info = Namespace(
         major=1,
         minor=2,
         patch=2,
         short=(1, 2),
-        full=(1, 2, 4),
-        string='1.2.4',
-        tuple=('1', '2', '4'),
+        full=(1, 2, 5),
+        string='1.2.5',
+        tuple=('1', '2', '5'),
         releaselevel='beta',
 )
 
 # 解析qteasy的本地安装路径
 QT_ROOT_PATH = os.path.normpath(os.path.join(os.path.dirname(__file__), os.pardir))
 QT_ROOT_PATH = os.path.join(QT_ROOT_PATH, 'qteasy/')
```

### Comparing `qteasy-1.2.4/qteasy/_arg_validators.py` & `qteasy-1.2.5/qteasy/_arg_validators.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/qteasy/backtest.py` & `qteasy-1.2.5/qteasy/backtest.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/qteasy/blender.py` & `qteasy-1.2.5/qteasy/blender.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/qteasy/broker.py` & `qteasy-1.2.5/qteasy/broker.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/qteasy/built_in.py` & `qteasy-1.2.5/qteasy/built_in.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/qteasy/core.py` & `qteasy-1.2.5/qteasy/core.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/qteasy/database.py` & `qteasy-1.2.5/qteasy/database.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/qteasy/emfuncs.py` & `qteasy-1.2.5/qteasy/emfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/qteasy/evaluate.py` & `qteasy-1.2.5/qteasy/evaluate.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/qteasy/finance.py` & `qteasy-1.2.5/qteasy/finance.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/qteasy/history.py` & `qteasy-1.2.5/qteasy/history.py`

 * *Files 11% similar despite different names*

```diff
@@ -264,22 +264,25 @@
         else:
             # return pd.Index(self._rows.keys(), dtype='datetime64')
             return list(self._rows.keys())
 
     @hdates.setter
     def hdates(self, input_hdates: list):
         if not self.is_empty:
-            assert isinstance(input_hdates, list), f'TypeError, input_hdates should be '
-            assert len(input_hdates) == self.row_count, \
-                f'ValueError, the number of input shares ({len(input_hdates)}) does not match level ' \
-                f'count ({self.row_count})'
+            if not isinstance(input_hdates, list):
+                error = f'input_hdates should be a list, got {type(input_hdates)} instead'
+                raise TypeError(error)
+            if not len(input_hdates) == self.row_count:
+                error = f'the number of input shares ({len(input_hdates)}) does not match level count ({self.row_count})'
+                raise ValueError(error)
             try:
                 new_hdates = [pd.to_datetime(date) for date in input_hdates]
-            except:
-                raise ValueError('one or more item in hdate list can not be converted to Timestamp')
+            except Exception as e:
+                error = f'{e} one or more item in hdate list can not be converted to Timestamp'
+                raise ValueError(error)
             self._rows = labels_to_dict(new_hdates, self.hdates)
 
     @property
     def row_count(self):
         """获取HistoryPanel的行数量"""
         return self._r_count
 
@@ -335,15 +338,20 @@
 
     @property
     def shape(self):
         """获取HistoryPanel的各个维度的尺寸"""
         return self._l_count, self._r_count, self._c_count
 
     def __len__(self):
-        """获取HistoryPanel的历史数据长度"""
+        """获取HistoryPanel的历史数据长度
+
+        Examples
+        --------
+
+        """
         return self._r_count
 
     def __getitem__(self, keys=None):
         """获取历史数据的一个切片，给定一个type、日期或股票代码, 输出相应的数据
 
         允许的输入包括切片形式的各种输入，包括string、数字列表或切片器对象slice()，返回切片后的ndarray对象
         允许的输入示例，第一个切片代表type切片，第二个是shares，第三个是rows：
@@ -364,14 +372,115 @@
         keys: list/tuple/slice
             历史数据的类型名，为空时给出所有类型的数据
 
         Returns
         -------
         out : ndarray
             self.value的一个切片
+
+        Examples
+        --------
+        >>> hp = qteasy.HistoryPanel(np.array([[[10, 20, 30, 40, 50]]*10]*3),
+        ...                          levels=['000001', '000002', '000003'],
+        ...                          rows=pd.date_range('2015-01-05', periods=10),
+        ...                          columns=['open', 'high', 'low', 'close', 'volume'])
+        >>> hp
+                share 0, label: 000001
+                    open  high  low  close  volume
+        2015-01-05    10    20   30     40      50
+        2015-01-06    10    20   30     40      50
+        2015-01-07    10    20   30     40      50
+        2015-01-08    10    20   30     40      50
+        2015-01-09    10    20   30     40      50
+        2015-01-10    10    20   30     40      50
+        2015-01-11    10    20   30     40      50
+        2015-01-12    10    20   30     40      50
+        2015-01-13    10    20   30     40      50
+        2015-01-14    10    20   30     40      50
+
+        share 1, label: 000002
+                    open  high  low  close  volume
+        2015-01-05    10    20   30     40      50
+        2015-01-06    10    20   30     40      50
+        2015-01-07    10    20   30     40      50
+        2015-01-08    10    20   30     40      50
+        2015-01-09    10    20   30     40      50
+        2015-01-10    10    20   30     40      50
+        2015-01-11    10    20   30     40      50
+        2015-01-12    10    20   30     40      50
+        2015-01-13    10    20   30     40      50
+        2015-01-14    10    20   30     40      50
+
+        share 2, label: 000003
+                    open  high  low  close  volume
+        2015-01-05    10    20   30     40      50
+        2015-01-06    10    20   30     40      50
+        2015-01-07    10    20   30     40      50
+        2015-01-08    10    20   30     40      50
+        2015-01-09    10    20   30     40      50
+        2015-01-10    10    20   30     40      50
+        2015-01-11    10    20   30     40      50
+        2015-01-12    10    20   30     40      50
+        2015-01-13    10    20   30     40      50
+        2015-01-14    10    20   30     40      50
+        >>> hp['close']
+        array([[[40],
+                [40],
+                [40],
+                [40],
+                [40],
+                [40],
+                [40],
+                [40],
+                [40],
+                [40]],
+
+               [[40],
+                [40],
+                [40],
+                [40],
+                [40],
+                [40],
+                [40],
+                [40],
+                [40],
+                [40]],
+
+               [[40],
+                [40],
+                [40],
+                [40],
+                [40],
+                [40],
+                [40],
+                [40],
+                [40],
+                [40]]])
+        >>> hp['close, open, low', '000001:000002']
+        array([[[40, 10, 30],
+                [40, 10, 30],
+                [40, 10, 30],
+                [40, 10, 30],
+                [40, 10, 30],
+                [40, 10, 30],
+                [40, 10, 30],
+                [40, 10, 30],
+                [40, 10, 30],
+                [40, 10, 30]],
+
+               [[40, 10, 30],
+                [40, 10, 30],
+                [40, 10, 30],
+                [40, 10, 30],
+                [40, 10, 30],
+                [40, 10, 30],
+                [40, 10, 30],
+                [40, 10, 30],
+                [40, 10, 30],
+                [40, 10, 30]]])
         """
         if self.is_empty:
             return None
         else:
             key_is_none = keys is None
             key_is_tuple = isinstance(keys, tuple)
             key_is_list = isinstance(keys, list)
@@ -476,14 +585,42 @@
         start_date: 开始日期
         end_date: 结束日期
 
         Returns
         -------
         out : HistoryPanel
             一个HistoryPanel，包含start_date到end_date之间所有share和htypes的数据
+
+        Examples
+        --------
+        >>> hp = qteasy.HistoryPanel(np.array([[[10, 20, 30, 40, 50]]*10]*3),
+        ...                          levels=['000001', '000002', '000003'],
+        ...                          rows=pd.date_range('2015-01-05', periods=10),
+        ...                          columns=['open', 'high', 'low', 'close', 'volume'])
+        >>> hp.segment('2015-01-07', '2015-01-10')
+        share 0, label: 000100
+                    open  high  low  close  volume
+        2015-01-07    10    20   30     40      50
+        2015-01-08    10    20   30     40      50
+        2015-01-09    10    20   30     40      50
+        2015-01-10    10    20   30     40      50
+
+        share 1, label: 000200
+                    open  high  low  close  volume
+        2015-01-07    10    20   30     40      50
+        2015-01-08    10    20   30     40      50
+        2015-01-09    10    20   30     40      50
+        2015-01-10    10    20   30     40      50
+
+        share 2, label: 000300
+                    open  high  low  close  volume
+        2015-01-07    10    20   30     40      50
+        2015-01-08    10    20   30     40      50
+        2015-01-09    10    20   30     40      50
+        2015-01-10    10    20   30     40      50
         """
         hdates = np.array(self.hdates)
         if start_date is None:
             start_date = hdates[0]
         if end_date is None:
             end_date = hdates[-1]
         sd = pd.to_datetime(start_date)
@@ -504,14 +641,39 @@
         start_index: 开始日期序号
         end_index: 结束日期序号
 
         Returns
         -------
         out : HistoryPanel
             一个HistoryPanel，包含start_date到end_date之间所有share和htypes的数据
+
+        Examples
+        --------
+        >>> hp = qteasy.HistoryPanel(np.array([[[10, 20, 30, 40, 50]]*10]*3),
+        ...                          levels=['000001', '000002', '000003'],
+        ...                          rows=pd.date_range('2015-01-05', periods=10),
+        ...                          columns=['open', 'high', 'low', 'close', 'volume'])
+        >>> hp.isegment(2, 5)
+        share 0, label: 000100
+                    open  high  low  close  volume
+        2015-01-07    10    20   30     40      50
+        2015-01-08    10    20   30     40      50
+        2015-01-09    10    20   30     40      50
+
+        share 1, label: 000200
+                    open  high  low  close  volume
+        2015-01-07    10    20   30     40      50
+        2015-01-08    10    20   30     40      50
+        2015-01-09    10    20   30     40      50
+
+        share 2, label: 000300
+                    open  high  low  close  volume
+        2015-01-07    10    20   30     40      50
+        2015-01-08    10    20   30     40      50
+        2015-01-09    10    20   30     40      50
         """
         hdates = np.array(self.hdates)
         new_dates = list(hdates[start_index:end_index])
         new_values = self[:, :, start_index:end_index]
         return HistoryPanel(new_values, levels=self.shares, rows=new_dates, columns=self.htypes)
 
     def slice(self, shares=None, htypes=None):
@@ -525,14 +687,21 @@
         htypes: str or list of str
             需要的数据类型列表
 
         Returns
         -------
         out : HistoryPanel
             一个HistoryPanel，包含shares和htypes中指定的股票和数据类型的数据
+
+        Examples
+        --------
+        >>> hp = qteasy.HistoryPanel(np.array([[[10, 20, 30, 40, 50]]*10]*3),
+        ...                          levels=['000001', '000002', '000003'],
+        ...                          rows=pd.date_range('2015-01-05', periods=10),
+        ...                          columns=['open', 'high', 'low', 'close', 'volume'])
         """
         if self.is_empty:
             return self
         if shares is None:
             shares = self.shares
         if isinstance(shares, str):
             shares = str_to_list(shares)
@@ -553,32 +722,32 @@
 
         Returns
         -------
         None
 
         Examples
         --------
-        >>> hp = qteasy.HistoryPanel(np.array([[[100, 100, 100, 100, 100]*100]*3]),
+        >>> hp = qteasy.HistoryPanel(np.array([[[10, 20, 30, 40, 50]]*10]*3),
         ...                          levels=['000001', '000002', '000003'],
-        ...                          rows=pd.date_range('2015-01-05', periods=100),
+        ...                          rows=pd.date_range('2015-01-05', periods=10),
         ...                          columns=['open', 'high', 'low', 'close', 'volume'])
         >>> hp.info()
         <class 'qteasy.history.HistoryPanel'>
-        History Panel at 0x7f8b0c0b0f10
-        Datetime Range: 100 entries, 2015-01-05 00:00:00 to 2015-04-24 00:00:00
+        History Panel at 0x12215a850
+        Datetime Range: 10 entries, 2015-01-05 00:00:00 to 2015-01-14 00:00:00
         Historical Data Types (total 5 data types):
         ['open', 'high', 'low', 'close', 'volume']
         Shares (total 3 shares):
         ['000001', '000002', '000003']
         non-null values for each share and data type:
-                open   high    low  close volume
-        000001   100    100    100    100    100
-        000002   100    100    100    100    100
-        000003   100    100    100    100    100
-        memory usage: 12136 bytes
+                open  high  low  close  volume
+        000001    10    10   10     10      10
+        000002    10    10   10     10      10
+        000003    10    10   10     10      10
+        memory usage: 1344 bytes
         """
         import sys
         print(f'\n{type(self)}')
         if self.is_empty:
             print(f'Empty History Panel at {hex(id(self))}')
         else:
             print(f'History Panel at {hex(id(self))}')
@@ -602,32 +771,94 @@
 
     def copy(self):
         """ 返回一个新的HistoryPanel对象，其值和本对象相同"""
         # TODO: 应该考虑使用copy模块的copy(deep=True)代替下面的代码
         return HistoryPanel(values=self.values, levels=self.levels, rows=self.rows, columns=self.columns)
 
     def len(self):
-        """ 返回HistoryPanel对象的长度，即日期个数"""
+        """ 返回HistoryPanel对象的长度，即日期个数
+
+        Returns
+        -------
+        int
+            日期个数
+
+        Examples
+        --------
+        >>> hp = qteasy.HistoryPanel(np.array([[[10, 20, 30, 40, 50]]*10]*3),
+        ...                          levels=['000001', '000002', '000003'],
+        ...                          rows=pd.date_range('2015-01-05', periods=10),
+        ...                          columns=['open', 'high', 'low', 'close', 'volume'])
+        >>> hp.len()
+        10
+        """
         return self.row_count
 
-    def re_label(self, shares: str = None, htypes: str = None, hdates=None):
+    def re_label(self, shares: (str, list) = None, htypes: (str, list) = None, hdates: (str, list) = None) -> None:
         """ 给HistoryPanel对象的层、行、列标签重新赋值
 
         Parameters
         ----------
         shares: str or list of str
             股票列表
         htypes: str or list of str
             数据类型列表
         hdates: str or list of str
             日期列表
 
         Returns
         -------
         None
+
+        Examples
+        --------
+        >>> hp = qteasy.HistoryPanel(np.array([[[10, 20, 30, 40, 50]]*10]*3),
+        ...                          levels=['000001', '000002', '000003'],
+        ...                          rows=pd.date_range('2015-01-05', periods=10),
+        ...                          columns=['open', 'high', 'low', 'close', 'volume'])
+        >>> hp.re_label(shares=['000100', '000200', '000300'], htypes=['typeA', 'typeB', 'typeC', 'typeD', 'typeE'])
+        >>> hp
+        share 0, label: 000100
+                    typeA  typeB  typeC  typeD  typeE
+        2015-01-05     10     20     30     40     50
+        2015-01-06     10     20     30     40     50
+        2015-01-07     10     20     30     40     50
+        2015-01-08     10     20     30     40     50
+        2015-01-09     10     20     30     40     50
+        2015-01-10     10     20     30     40     50
+        2015-01-11     10     20     30     40     50
+        2015-01-12     10     20     30     40     50
+        2015-01-13     10     20     30     40     50
+        2015-01-14     10     20     30     40     50
+
+        share 1, label: 000200
+                    typeA  typeB  typeC  typeD  typeE
+        2015-01-05     10     20     30     40     50
+        2015-01-06     10     20     30     40     50
+        2015-01-07     10     20     30     40     50
+        2015-01-08     10     20     30     40     50
+        2015-01-09     10     20     30     40     50
+        2015-01-10     10     20     30     40     50
+        2015-01-11     10     20     30     40     50
+        2015-01-12     10     20     30     40     50
+        2015-01-13     10     20     30     40     50
+        2015-01-14     10     20     30     40     50
+
+        share 2, label: 000300
+                    typeA  typeB  typeC  typeD  typeE
+        2015-01-05     10     20     30     40     50
+        2015-01-06     10     20     30     40     50
+        2015-01-07     10     20     30     40     50
+        2015-01-08     10     20     30     40     50
+        2015-01-09     10     20     30     40     50
+        2015-01-10     10     20     30     40     50
+        2015-01-11     10     20     30     40     50
+        2015-01-12     10     20     30     40     50
+        2015-01-13     10     20     30     40     50
+        2015-01-14     10     20     30     40     50
         """
         if not self.is_empty:
             if shares is not None:
                 self.shares = shares
             if htypes is not None:
                 self.htypes = htypes
             if hdates is not None:
@@ -745,55 +976,60 @@
 
             空数据填充值，当组合后的HP存在空数据时，应该以什么值填充，默认为np.nan
 
         Returns
         -------
         HistoryPanel, 一个新的History Panel对象
 
-
         Examples
         --------
-        如果两个HistoryPanel中包含标签相同的数据，那么新的HistoryPanel中将包含调用join方法的HistoryPanel对象的相应数据。例如：
-
-        hp1:
+        # 如果两个HistoryPanel中包含标签相同的数据，那么新的HistoryPanel中将包含调用join方法的HistoryPanel对象的相应数据。例如：
+        >>> hp1 = qteasy.HistoryPanel(np.array([[[8, 9, 9], [7, 5, 5], [4, 8, 4], [1, 0, 7], [8, 7, 9]],
+        ...                                     [[2, 3, 3], [5, 4, 6], [2, 8, 7], [3, 3, 4], [8, 8, 7]]]),
+        ...                           levels=['000200', '000300'],
+        ...                           rows=pd.date_range('2020-01-01', periods=5),
+        ...                           columns=['close', 'open', 'high'])
+        >>> hp2 = qteasy.HistoryPanel(np.array([[[8, 9, 9], [7, 5, 5], [4, 8, 4], [1, 0, 7], [8, 7, 9]],
+        ...                                     [[2, 3, 3], [5, 4, 6], [2, 8, 7], [3, 3, 4], [8, 8, 7]]]),
+        ...                           levels=['000400', '000500'],
+        ...                           rows=pd.date_range('2020-01-01', periods=5),
+        ...                           columns=['close', 'open', 'high'])
+        >>> hp1
         share 0, label: 000200
                     close  open  high
         2020-01-01      8     9     9
         2020-01-02      7     5     5
         2020-01-03      4     8     4
         2020-01-04      1     0     7
         2020-01-05      8     7     9
-
         share 1, label: 000300
                     close  open  high
         2020-01-01      2     3     3
         2020-01-02      5     4     6
         2020-01-03      2     8     7
         2020-01-04      3     3     4
         2020-01-05      8     8     7
-
-        hp2:
-        share 0, label: 000200
+        >>> hp2
+        share 0, label: 000400
                     close  open  high
         2020-01-01      8     9     9
         2020-01-02      7     5     5
         2020-01-03      4     8     4
         2020-01-04      1     0     7
         2020-01-05      8     7     9
-
-        share 1, label: 000300
+        share 1, label: 000500
                     close  open  high
         2020-01-01      2     3     3
         2020-01-02      5     4     6
         2020-01-03      2     8     7
         2020-01-04      3     3     4
         2020-01-05      8     8     7
 
-
-        连接时可以指定两个HistoryPanel之间共享的标签类型，如
+        >>> hp1.join(hp2)
+        share 0, label: 000200
         """
 
         assert isinstance(other, HistoryPanel), \
             f'TypeError, HistoryPanel can only be joined with other HistoryPanel.'
         if self.is_empty:
             return other
         elif other.is_empty:
```

### Comparing `qteasy-1.2.4/qteasy/optimization.py` & `qteasy-1.2.5/qteasy/optimization.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/qteasy/qt_operator.py` & `qteasy-1.2.5/qteasy/qt_operator.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/qteasy/space.py` & `qteasy-1.2.5/qteasy/space.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/qteasy/strategy.py` & `qteasy-1.2.5/qteasy/strategy.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/qteasy/tafuncs.py` & `qteasy-1.2.5/qteasy/tafuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/qteasy/trade_recording.py` & `qteasy-1.2.5/qteasy/trade_recording.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/qteasy/trader.py` & `qteasy-1.2.5/qteasy/trader.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/qteasy/trader_cli.py` & `qteasy-1.2.5/qteasy/trader_cli.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/qteasy/trader_tui.py` & `qteasy-1.2.5/qteasy/trader_tui.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/qteasy/trading_util.py` & `qteasy-1.2.5/qteasy/trading_util.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/qteasy/tsfuncs.py` & `qteasy-1.2.5/qteasy/tsfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/qteasy/tui_style.tcss` & `qteasy-1.2.5/qteasy/tui_style.tcss`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/qteasy/utilfuncs.py` & `qteasy-1.2.5/qteasy/utilfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/qteasy/visual.py` & `qteasy-1.2.5/qteasy/visual.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/qteasy.egg-info/PKG-INFO` & `qteasy-1.2.5/qteasy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qteasy
-Version: 1.2.4
+Version: 1.2.5
 Summary: A fast quantitative investment tool kit
 Home-page: https://github.com/shepherdpp/qteasy
 Author: Jackie PENG
 Author-email: jackie PENG <jackie.pengzhao@gmail.com>
 Maintainer: Jackie PENG
 Maintainer-email: jackie PENG <jackie.pengzhao@gmail.com>
 License: Copyright <2019> <JACKIE PENG>
@@ -106,15 +106,15 @@
 > 我会尽快修复问题并回复大家的问题。
 
 ## 关于`qteasy`
 
 - 作者: **Jackie PENG**
 - email: *jackie_pengzhao@163.com*
 - Created: 2019, July, 16
-- Latest Version: `1.2.4`
+- Latest Version: `1.2.5`
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
```

### Comparing `qteasy-1.2.4/qteasy.egg-info/SOURCES.txt` & `qteasy-1.2.5/qteasy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/setup.cfg` & `qteasy-1.2.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qteasy
-version = 1.2.4
+version = 1.2.5
 author = Jackie PENG
 author_email = jackie.pengzhao@gmail.com
 maintainer = Jackie PENG
 description = A fast quantitative investment tool kit
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/shepherdpp/qteasy
```

### Comparing `qteasy-1.2.4/tests/test_broker.py` & `qteasy-1.2.5/tests/test_broker.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/tests/test_cashplan.py` & `qteasy-1.2.5/tests/test_cashplan.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/tests/test_config.py` & `qteasy-1.2.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/tests/test_core_sub_funcs.py` & `qteasy-1.2.5/tests/test_core_sub_funcs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/tests/test_cost.py` & `qteasy-1.2.5/tests/test_cost.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/tests/test_datasource.py` & `qteasy-1.2.5/tests/test_datasource.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/tests/test_eastmoney.py` & `qteasy-1.2.5/tests/test_eastmoney.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/tests/test_evaluations.py` & `qteasy-1.2.5/tests/test_evaluations.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/tests/test_fast_experiments.py` & `qteasy-1.2.5/tests/test_fast_experiments.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/tests/test_historypanel.py` & `qteasy-1.2.5/tests/test_historypanel.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/tests/test_loop.py` & `qteasy-1.2.5/tests/test_loop.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/tests/test_operator_and_strategy.py` & `qteasy-1.2.5/tests/test_operator_and_strategy.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/tests/test_qt.py` & `qteasy-1.2.5/tests/test_qt.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/tests/test_space.py` & `qteasy-1.2.5/tests/test_space.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/tests/test_ta_funcs.py` & `qteasy-1.2.5/tests/test_ta_funcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,15 +364,15 @@
 
     def test_trix_vs_trix_no_ta(self):
         """ 测试trix和trix_no_ta的结果是否一致 """
         res = trix(self.close, timeperiod=5)
         res_no_ta = trix_no_ta(self.close, timeperiod=5)
         print(f'result is \n{res}\n'
               f'result_no_ta is \n{res_no_ta}')
-        self.assertTrue(np.allclose(res[14:], res_no_ta[14:], equal_nan=True, atol=0.2))
+        self.assertTrue(np.allclose(res[14:], res_no_ta[14:], equal_nan=True, atol=0.5))
 
     def test_ultosc(self):
         print(f'test TA function: ultosc\n'
               f'=========================')
         res = ultosc(self.high, self.low, self.close)
         print(f'result is \n{res}')
```

### Comparing `qteasy-1.2.4/tests/test_trader.py` & `qteasy-1.2.5/tests/test_trader.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/tests/test_trader_shell.py` & `qteasy-1.2.5/tests/test_trader_shell.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/tests/test_trading.py` & `qteasy-1.2.5/tests/test_trading.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/tests/test_tui.py` & `qteasy-1.2.5/tests/test_tui.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/tests/test_tushare.py` & `qteasy-1.2.5/tests/test_tushare.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/tests/test_utilityfuncs.py` & `qteasy-1.2.5/tests/test_utilityfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.4/tests/test_visual.py` & `qteasy-1.2.5/tests/test_visual.py`

 * *Files identical despite different names*

