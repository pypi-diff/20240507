# Comparing `tmp/pkscreener-0.44.20240506.350.tar.gz` & `tmp/pkscreener-0.44.20240507.351.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240506.350.tar", last modified: Mon May  6 21:11:11 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240507.351.tar", last modified: Tue May  7 05:27:13 2024, max compression
```

## Comparing `pkscreener-0.44.20240506.350.tar` & `pkscreener-0.44.20240507.351.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 21:11:11.356858 pkscreener-0.44.20240506.350/
--rw-rw-rw-   0        0        0     1086 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-06 21:11:11.356858 pkscreener-0.44.20240506.350/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 21:11:11.341240 pkscreener-0.44.20240506.350/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 21:11:11.356858 pkscreener-0.44.20240506.350/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    26895 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    10662 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    30557 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    11375 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    23429 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    21218 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18443 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   119820 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    52163 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    82528 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-06 21:11:01.000000 pkscreener-0.44.20240506.350/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   127567 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/globals.py
--rw-rw-rw-   0        0        0      872 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    48083 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    28426 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-06 21:11:11.341240 pkscreener-0.44.20240506.350/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-06 21:11:11.000000 pkscreener-0.44.20240506.350/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-06 21:11:11.000000 pkscreener-0.44.20240506.350/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 21:11:11.000000 pkscreener-0.44.20240506.350/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-06 21:11:11.000000 pkscreener-0.44.20240506.350/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-06 21:11:11.000000 pkscreener-0.44.20240506.350/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-06 21:11:11.000000 pkscreener-0.44.20240506.350/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-06 21:11:11.356858 pkscreener-0.44.20240506.350/setup.cfg
--rw-rw-rw-   0        0        0     4765 2024-05-06 21:06:05.000000 pkscreener-0.44.20240506.350/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 05:27:13.879524 pkscreener-0.44.20240507.351/
+-rw-rw-rw-   0        0        0     1086 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-07 05:27:13.879524 pkscreener-0.44.20240507.351/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 05:27:13.863897 pkscreener-0.44.20240507.351/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 05:27:13.879524 pkscreener-0.44.20240507.351/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    26895 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    10662 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    30557 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    11375 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    23429 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    21218 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18443 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   119820 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    52163 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    82528 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-07 05:27:05.000000 pkscreener-0.44.20240507.351/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   127567 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      872 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    47956 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    28426 2024-05-07 05:21:32.000000 pkscreener-0.44.20240507.351/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-07 05:27:13.863897 pkscreener-0.44.20240507.351/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-07 05:27:13.000000 pkscreener-0.44.20240507.351/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-07 05:27:13.000000 pkscreener-0.44.20240507.351/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 05:27:13.000000 pkscreener-0.44.20240507.351/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-07 05:27:13.000000 pkscreener-0.44.20240507.351/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-07 05:27:13.000000 pkscreener-0.44.20240507.351/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-07 05:27:13.000000 pkscreener-0.44.20240507.351/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-07 05:27:13.879524 pkscreener-0.44.20240507.351/setup.cfg
+-rw-rw-rw-   0        0        0     4765 2024-05-07 05:21:33.000000 pkscreener-0.44.20240507.351/setup.py
```

### Comparing `pkscreener-0.44.20240506.350/LICENSE` & `pkscreener-0.44.20240507.351/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/LICENSE-Others` & `pkscreener-0.44.20240507.351/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/PKG-INFO` & `pkscreener-0.44.20240507.351/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240506.350
+Version: 0.44.20240507.351
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240506.350.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240507.351.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.349/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.350/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.349/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.350/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.349/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.350/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240506.350/README.md` & `pkscreener-0.44.20240507.351/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.349/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.350/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.349/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.350/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.349/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.350/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240506.350/pkscreener/__init__.py` & `pkscreener-0.44.20240507.351/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/classes/ArtTexts.py` & `pkscreener-0.44.20240507.351/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240507.351/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240507.351/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240507.351/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240507.351/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240507.351/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240507.351/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240507.351/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240507.351/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240507.351/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240507.351/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240507.351/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240507.351/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240507.351/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240507.351/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240507.351/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240507.351/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240507.351/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240507.351/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240507.351/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240507.351/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240507.351/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240507.351/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240507.351/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240507.351/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/classes/keys.py` & `pkscreener-0.44.20240507.351/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/courbd.ttf` & `pkscreener-0.44.20240507.351/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/globals.py` & `pkscreener-0.44.20240507.351/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240507.351/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240507.351/pkscreener/pkscreenerbot.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,15 +193,15 @@
     if data == "MI":
         from PKDevTools.classes import Archiver
         filePath = os.path.join(Archiver.get_user_outputs_dir(), "monitor_outputs.txt")
         appLogsEnabled = ("PKDevTools_Default_Log_Level" in os.environ.keys())
         # User wants an Int. Monitor
         launcher = "/home/runner/work/PKScreener/PKScreener/pkscreenercli.bin" if "MONITORING_BOT_RUNNER" in os.environ.keys() else "pkscreener"
         launcher = f"python3.11 {launcher}" if launcher.endswith(".py") else launcher
-        # print(f"launcher is {sys.argv[0]} -a Y -m 'X' -p --telegram")
+        result_outputs = "Starting up the monitor for this hour. Please try again after 30-40 seconds."
         try:
             from subprocess import Popen
             global monitor_proc
             if monitor_proc is None or monitor_proc.poll() is not None: # Process finished from an earlier launch
                 if os.path.exists(filePath):
                     # Let's remove the old file so that the new app can begin to run
                     # If we don't remove, it might just exit assuming that there's another instance
@@ -211,36 +211,31 @@
                 if appLogsEnabled:
                     appArgs.append("-l")
                 else:
                     appArgs.append("-p")
                 monitor_proc = Popen(appArgs)
                 logger.info(f"{launcher} -a Y -m 'X' -p --telegram launched")
             else:
+                result_outputs = "Monitor is running, but the results are being prepared. Try again in next few seconds."
                 logger.info(f"{launcher} -a Y -m 'X' -p --telegram already running")
         except Exception as e:
+            result_outputs = "Something went wrong with the monitor. Try again later."
             logger.info(f"{launcher} -a Y -m 'X' -p --telegram could not be launched")
             logger.info(e)
             pass
         try:
-            # if not os.path.exists(filePath):
-            #     sleep(5)
-            #     if not os.path.exists(filePath):
-            #         f = open(filePath, "w")
-            #         f.write("Please wait...")
-            #         f.close()
             if os.path.exists(filePath):
                 f = open(filePath, "r")
                 result_outputs = f.read()
                 f.close()
-            else:
-                result_outputs = "No New update. Please try again in the next few seconds."
             await start(update, context, updatedResults=result_outputs)
             return START_ROUTES
         except:
-            await start(update, context, updatedResults="No New update. Please try again in the next few seconds.")
+            result_outputs = "Something went wrong with the monitor. Try again later."
+            await start(update, context, updatedResults=result_outputs)
             return START_ROUTES
 
     midSkip = "1" if data == "X" else "N"
     skipMenus = [midSkip]
     skipMenus.extend(INDEX_SKIP_MENUS)
     menuText = (
         m1.renderForMenu(
@@ -460,15 +455,15 @@
     reply_markup = InlineKeyboardMarkup(keyboard)
     return reply_markup
 
 
 async def sendUpdatedMenu(menuText, update: Update, context, reply_markup, replaceWhiteSpaces=True):
     try:
         if update.callback_query.message.text == menuText:
-            menuText = f"Something went wrong! Maybe try again later.\n{PKDateUtilities.currentDateTime()}: {menuText}"
+            menuText = f"{PKDateUtilities.currentDateTime()}:\n{menuText}"
         await update.callback_query.edit_message_text(
             text=menuText.replace("     ", "").replace("    ", "").replace("\t", "").replace(colorText.FAIL,"").replace(colorText.END,"") if replaceWhiteSpaces else menuText,
             parse_mode="HTML",
             reply_markup=reply_markup,
         )
     except Exception as e:# pragma: no cover
         logger.log(e)
```

### Comparing `pkscreener-0.44.20240506.350/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240507.351/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240507.351/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240506.350
+Version: 0.44.20240507.351
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240506.350.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240507.351.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.349/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.350/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.349/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.350/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.349/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.350/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240506.350/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240507.351/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.350/setup.py` & `pkscreener-0.44.20240507.351/setup.py`

 * *Files identical despite different names*

