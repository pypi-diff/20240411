# Comparing `tmp/pkscreener-0.44.20240407.251.tar.gz` & `tmp/pkscreener-0.44.20240410.252.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240407.251.tar", last modified: Sun Apr  7 00:38:06 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240410.252.tar", last modified: Wed Apr 10 21:12:51 2024, max compression
```

## Comparing `pkscreener-0.44.20240407.251.tar` & `pkscreener-0.44.20240410.252.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 00:38:06.887719 pkscreener-0.44.20240407.251/
--rw-rw-rw-   0        0        0     1086 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-07 00:38:06.887719 pkscreener-0.44.20240407.251/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 00:38:06.872114 pkscreener-0.44.20240407.251/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 00:38:06.887719 pkscreener-0.44.20240407.251/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0    17333 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    24554 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9291 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     2571 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    27486 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    15888 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    17381 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     7653 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    16886 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    48873 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   108935 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    44525 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    77593 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-07 00:37:57.000000 pkscreener-0.44.20240407.251/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   109963 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/globals.py
--rw-rw-rw-   0        0        0      565 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    47815 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    16959 2024-04-07 00:34:09.000000 pkscreener-0.44.20240407.251/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-07 00:38:06.872114 pkscreener-0.44.20240407.251/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-07 00:38:06.000000 pkscreener-0.44.20240407.251/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1250 2024-04-07 00:38:06.000000 pkscreener-0.44.20240407.251/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 00:38:06.000000 pkscreener-0.44.20240407.251/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-04-07 00:38:06.000000 pkscreener-0.44.20240407.251/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-07 00:38:06.000000 pkscreener-0.44.20240407.251/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-07 00:38:06.000000 pkscreener-0.44.20240407.251/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-07 00:38:06.887719 pkscreener-0.44.20240407.251/setup.cfg
--rw-rw-rw-   0        0        0     4715 2024-04-07 00:34:10.000000 pkscreener-0.44.20240407.251/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 21:12:51.162744 pkscreener-0.44.20240410.252/
+-rw-rw-rw-   0        0        0     1086 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-10 21:12:51.162744 pkscreener-0.44.20240410.252/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 21:12:51.147121 pkscreener-0.44.20240410.252/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 21:12:51.162744 pkscreener-0.44.20240410.252/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0    17333 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    24554 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9291 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     2571 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    27488 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    15888 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    17381 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     7653 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    16886 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    48873 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   108935 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    44525 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    77593 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-10 21:12:34.000000 pkscreener-0.44.20240410.252/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   110051 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      565 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    47815 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    16959 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-10 21:12:51.147121 pkscreener-0.44.20240410.252/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-10 21:12:51.000000 pkscreener-0.44.20240410.252/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1250 2024-04-10 21:12:51.000000 pkscreener-0.44.20240410.252/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 21:12:51.000000 pkscreener-0.44.20240410.252/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-04-10 21:12:51.000000 pkscreener-0.44.20240410.252/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-10 21:12:51.000000 pkscreener-0.44.20240410.252/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-10 21:12:51.000000 pkscreener-0.44.20240410.252/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-10 21:12:51.162744 pkscreener-0.44.20240410.252/setup.cfg
+-rw-rw-rw-   0        0        0     4715 2024-04-10 21:09:05.000000 pkscreener-0.44.20240410.252/setup.py
```

### Comparing `pkscreener-0.44.20240407.251/LICENSE` & `pkscreener-0.44.20240410.252/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/LICENSE-Others` & `pkscreener-0.44.20240410.252/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/PKG-INFO` & `pkscreener-0.44.20240410.252/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240407.251
+Version: 0.44.20240410.252
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240407.251.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240410.252.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240406.250/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240407.251/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240406.250/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240407.251/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240406.250/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240407.251/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240407.251/README.md` & `pkscreener-0.44.20240410.252/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240406.250/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240407.251/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240406.250/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240407.251/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240406.250/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240407.251/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240407.251/pkscreener/__init__.py` & `pkscreener-0.44.20240410.252/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240410.252/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240410.252/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240410.252/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240410.252/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240410.252/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240410.252/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240410.252/pkscreener/classes/MenuOptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     "10": "Closing at least 2% up since last 3 days",
     "11": "Short term bullish (Ichimoku)  ",
     "12": "15 Minute Price & Volume breakout(Intraday)",
     "13": "Bullish RSI & MACD             ",
     "14": "NR4 Daily Today",
     "15": "52 week low breakout(today)(Sell)",
     "16": "10 days low breakout(Sell)",
-    "17": "52 week high breakout(today)"   ,
+    "17": "52 week high breakout(today)     ",
     "18": "Bullish Aroon(14) Crossover",
     "19": "MACD Histogram x below 0 (Sell) ",
     "20": "Bullish for next day",
     "21": "MF/FIIs Popular Stocks         ",
     "22": "View Stock Performance         ",
     "23": "Breaking out now               ",
     "24": "Higher Highs,Lows & Close (SuperTrend)",
```

### Comparing `pkscreener-0.44.20240407.251/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240410.252/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240410.252/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240410.252/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240410.252/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240410.252/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240410.252/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240410.252/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240410.252/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240410.252/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240410.252/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240410.252/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240410.252/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240410.252/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240410.252/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240410.252/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/pkscreener/classes/keys.py` & `pkscreener-0.44.20240410.252/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/pkscreener/courbd.ttf` & `pkscreener-0.44.20240410.252/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/pkscreener/globals.py` & `pkscreener-0.44.20240410.252/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1198,17 +1198,19 @@
                     dividend_df = pd.merge(screen_copy, dividend_df, on='Stock')
                     bonus_df = pd.merge(screen_copy, bonus_df, on='Stock')
                     stockSplit_df = pd.merge(screen_copy, stockSplit_df, on='Stock')
                     corp_dfs = [dividend_df, bonus_df, stockSplit_df]
                     shareable_strings = []
                     shouldSend = False
                     for corp_df in corp_dfs:
-                        corp_df.set_index("Stock", inplace=True)
+                        if corp_df is None:
+                            continue
                         tab_results = ""
-                        if corp_df is not None and len(corp_df) > 0:
+                        if corp_df is not None and not corp_df.empty:
+                            corp_df.set_index("Stock", inplace=True)
                             tab_results = colorText.miniTabulator().tabulate(
                                 corp_df,
                                 headers="keys",
                                 tablefmt=colorText.No_Pad_GridFormat,
                                 # showindex = False,
                                 maxcolwidths=Utility.tools.getMaxColumnWidths(dividend_df)
                             ).encode("utf-8").decode(STD_ENCODING)
```

### Comparing `pkscreener-0.44.20240407.251/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240410.252/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240410.252/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240410.252/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240410.252/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240407.251
+Version: 0.44.20240410.252
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240407.251.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240410.252.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240406.250/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240407.251/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240406.250/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240407.251/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240406.250/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240407.251/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240407.251/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240410.252/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240407.251/setup.py` & `pkscreener-0.44.20240410.252/setup.py`

 * *Files identical despite different names*

