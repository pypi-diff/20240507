# Comparing `tmp/pkscreener-0.44.20240507.352.tar.gz` & `tmp/pkscreener-0.44.20240507.353.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240507.352.tar", last modified: Tue May  7 06:13:54 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240507.353.tar", last modified: Tue May  7 07:55:52 2024, max compression
```

## Comparing `pkscreener-0.44.20240507.352.tar` & `pkscreener-0.44.20240507.353.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 06:13:54.670587 pkscreener-0.44.20240507.352/
--rw-rw-rw-   0        0        0     1086 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-07 06:13:54.670587 pkscreener-0.44.20240507.352/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 06:13:54.654951 pkscreener-0.44.20240507.352/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:13:54.670587 pkscreener-0.44.20240507.352/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    26895 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    10662 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    30557 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    11375 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    23429 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    21218 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18443 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   119820 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    52163 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    82528 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-07 06:13:45.000000 pkscreener-0.44.20240507.352/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   127567 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/globals.py
--rw-rw-rw-   0        0        0      872 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    48246 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    28426 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:13:54.654951 pkscreener-0.44.20240507.352/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-07 06:13:54.000000 pkscreener-0.44.20240507.352/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-07 06:13:54.000000 pkscreener-0.44.20240507.352/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 06:13:54.000000 pkscreener-0.44.20240507.352/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-07 06:13:54.000000 pkscreener-0.44.20240507.352/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-07 06:13:54.000000 pkscreener-0.44.20240507.352/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-07 06:13:54.000000 pkscreener-0.44.20240507.352/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-07 06:13:54.670587 pkscreener-0.44.20240507.352/setup.cfg
--rw-rw-rw-   0        0        0     4765 2024-05-07 06:09:04.000000 pkscreener-0.44.20240507.352/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:55:52.559788 pkscreener-0.44.20240507.353/
+-rw-rw-rw-   0        0        0     1086 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-07 07:55:52.559788 pkscreener-0.44.20240507.353/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 07:55:52.544189 pkscreener-0.44.20240507.353/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:55:52.559788 pkscreener-0.44.20240507.353/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    26895 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    10662 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    30557 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    11375 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    23429 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    21218 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18443 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   119820 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    52163 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    82528 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-07 07:55:43.000000 pkscreener-0.44.20240507.353/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   127567 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      872 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    48761 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    28426 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:55:52.559788 pkscreener-0.44.20240507.353/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-07 07:55:52.000000 pkscreener-0.44.20240507.353/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-07 07:55:52.000000 pkscreener-0.44.20240507.353/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 07:55:52.000000 pkscreener-0.44.20240507.353/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-07 07:55:52.000000 pkscreener-0.44.20240507.353/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-07 07:55:52.000000 pkscreener-0.44.20240507.353/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-07 07:55:52.000000 pkscreener-0.44.20240507.353/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-07 07:55:52.559788 pkscreener-0.44.20240507.353/setup.cfg
+-rw-rw-rw-   0        0        0     4765 2024-05-07 07:51:13.000000 pkscreener-0.44.20240507.353/setup.py
```

### Comparing `pkscreener-0.44.20240507.352/LICENSE` & `pkscreener-0.44.20240507.353/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/LICENSE-Others` & `pkscreener-0.44.20240507.353/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/PKG-INFO` & `pkscreener-0.44.20240507.353/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240507.352
+Version: 0.44.20240507.353
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240507.352.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240507.353.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.351/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.352/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.351/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.352/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.351/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.352/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240507.352/README.md` & `pkscreener-0.44.20240507.353/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.351/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.352/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.351/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.352/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.351/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.352/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240507.352/pkscreener/__init__.py` & `pkscreener-0.44.20240507.353/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/classes/ArtTexts.py` & `pkscreener-0.44.20240507.353/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240507.353/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240507.353/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240507.353/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240507.353/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240507.353/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240507.353/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240507.353/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240507.353/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240507.353/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240507.353/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240507.353/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240507.353/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240507.353/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240507.353/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240507.353/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240507.353/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240507.353/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240507.353/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240507.353/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240507.353/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240507.353/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240507.353/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240507.353/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240507.353/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/classes/keys.py` & `pkscreener-0.44.20240507.353/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/courbd.ttf` & `pkscreener-0.44.20240507.353/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/globals.py` & `pkscreener-0.44.20240507.353/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240507.353/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240507.353/pkscreener/pkscreenerbot.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,64 +181,78 @@
         chat_id=int(f"-{Channel_Id}"),
         text=f"Name: {user.first_name}, Username:@{user.username} with ID: {str(user.id)} started using the bot!\n{chosenBotMenuOption}",
         parse_mode=ParseMode.HTML,
     )
     # Tell ConversationHandler that we're in state `FIRST` now
     return START_ROUTES
 
+def launchIntradayMonitor():
+    from PKDevTools.classes import Archiver
+    filePath = os.path.join(Archiver.get_user_outputs_dir(), "monitor_outputs.txt")
+    result_outputs = ""
+    if (PKDateUtilities.isTradingTime() and not PKDateUtilities.isTodayHoliday()[0]) or ("PKDevTools_Default_Log_Level" in os.environ.keys()):
+        result_outputs = "Starting up the monitor for this hour. Please try again after 30-40 seconds."
+    else:
+        result_outputs = f"{PKDateUtilities.currentDateTime()}\nIntraday Monitor is available only during the NSE trading hours! Please try during the next trading session."
+        try:
+            os.remove(filePath)
+        except:
+            pass
+        return result_outputs, filePath
+
+    appLogsEnabled = ("PKDevTools_Default_Log_Level" in os.environ.keys())
+    # User wants an Int. Monitor
+    launcher = "/home/runner/work/PKScreener/PKScreener/pkscreenercli.bin" if "MONITORING_BOT_RUNNER" in os.environ.keys() else "pkscreener"
+    launcher = f"python3.11 {launcher}" if launcher.endswith(".py") else launcher
+    
+    try:
+        from subprocess import Popen
+        global monitor_proc
+        if monitor_proc is None or monitor_proc.poll() is not None: # Process finished from an earlier launch
+            if os.path.exists(filePath):
+                # Let's remove the old file so that the new app can begin to run
+                # If we don't remove, it might just exit assuming that there's another instance
+                # already running.
+                os.remove(filePath)
+            appArgs = [f"{launcher}","-a","Y","-m","X","--telegram",]
+            if appLogsEnabled:
+                appArgs.append("-l")
+            else:
+                appArgs.append("-p")
+            monitor_proc = Popen(appArgs)
+            logger.info(f"{launcher} -a Y -m 'X' -p --telegram launched")
+        else:
+            result_outputs = "Monitor is running, but the results are being prepared. Try again in next few seconds."
+            logger.info(f"{launcher} -a Y -m 'X' -p --telegram already running")
+    except Exception as e:
+        result_outputs = "Hmm...It looks like you caught us taking a break! Try again later :-)"
+        logger.info(f"{launcher} -a Y -m 'X' -p --telegram could not be launched")
+        logger.info(e)
+        pass
+    return result_outputs, filePath
 
 async def XScanners(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
     """Show new choice of buttons"""
     query = update.callback_query
     data = query.data.upper().replace("CX", "X").replace("CB", "B").replace("CG", "G").replace("CMI", "MI")
     if data not in TOP_LEVEL_SCANNER_MENUS:
         return start(update, context)
     if data == "MI":
-        from PKDevTools.classes import Archiver
-        filePath = os.path.join(Archiver.get_user_outputs_dir(), "monitor_outputs.txt")
-        appLogsEnabled = ("PKDevTools_Default_Log_Level" in os.environ.keys())
-        # User wants an Int. Monitor
-        launcher = "/home/runner/work/PKScreener/PKScreener/pkscreenercli.bin" if "MONITORING_BOT_RUNNER" in os.environ.keys() else "pkscreener"
-        launcher = f"python3.11 {launcher}" if launcher.endswith(".py") else launcher
-        result_outputs = "Starting up the monitor for this hour. Please try again after 30-40 seconds."
-        try:
-            from subprocess import Popen
-            global monitor_proc
-            if monitor_proc is None or monitor_proc.poll() is not None: # Process finished from an earlier launch
-                if os.path.exists(filePath):
-                    # Let's remove the old file so that the new app can begin to run
-                    # If we don't remove, it might just exit assuming that there's another instance
-                    # already running.
-                    os.remove(filePath)
-                appArgs = [f"{launcher}","-a","Y","-m","X","--telegram",]
-                if appLogsEnabled:
-                    appArgs.append("-l")
-                else:
-                    appArgs.append("-p")
-                monitor_proc = Popen(appArgs)
-                logger.info(f"{launcher} -a Y -m 'X' -p --telegram launched")
-            else:
-                result_outputs = "Monitor is running, but the results are being prepared. Try again in next few seconds."
-                logger.info(f"{launcher} -a Y -m 'X' -p --telegram already running")
-        except Exception as e:
-            result_outputs = "Hmm...It looks like you caught us taking a break! Try again later :-)"
-            logger.info(f"{launcher} -a Y -m 'X' -p --telegram could not be launched")
-            logger.info(e)
-            pass
+        result_outputs, filePath = launchIntradayMonitor()
         try:
             if os.path.exists(filePath):
                 f = open(filePath, "r")
                 result_outputs = f.read()
                 f.close()
             await start(update, context, updatedResults=result_outputs)
             return START_ROUTES
         except Exception as e:
             result_outputs = "Hmm...It looks like you caught us taking a break! Try again later :-)"
             logger.info(e)
-            logger.info(f"{launcher} -a Y -m 'X' -p --telegram could not read {filePath}")
+            logger.info(f"Could not read {filePath}")
             await start(update, context, updatedResults=result_outputs)
             return START_ROUTES
 
     midSkip = "1" if data == "X" else "N"
     skipMenus = [midSkip]
     skipMenus.extend(INDEX_SKIP_MENUS)
     menuText = (
@@ -1056,14 +1070,15 @@
     # application.add_handler(MessageHandler(filters.TEXT & filters.COMMAND, command_handler))
     # application.add_handler(MessageHandler(filters.COMMAND, command_handler))
     # Add ConversationHandler to application that will be used for handling updates
     addCommandsForMenuItems(application)
     application.add_handler(conv_handler)
     # ...and the error handler
     application.add_error_handler(error_handler)
-
+    # Run the intraday monitor
+    launchIntradayMonitor()
     # Run the bot until the user presses Ctrl-C
     application.run_polling(allowed_updates=Update.ALL_TYPES)
 
 
 if __name__ == "__main__":
     runpkscreenerbot()
```

### Comparing `pkscreener-0.44.20240507.352/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240507.353/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240507.353/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240507.352
+Version: 0.44.20240507.353
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240507.352.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240507.353.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.351/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.352/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.351/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.352/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.351/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.352/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240507.352/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240507.353/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.352/setup.py` & `pkscreener-0.44.20240507.353/setup.py`

 * *Files identical despite different names*

