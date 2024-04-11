# Comparing `tmp/PyAibote-1.3.7.tar.gz` & `tmp/PyAibote-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyAibote-1.3.7.tar", last modified: Thu Apr 11 06:45:22 2024, max compression
+gzip compressed data, was "PyAibote-1.3.8.tar", last modified: Thu Apr 11 10:11:42 2024, max compression
```

## Comparing `PyAibote-1.3.7.tar` & `PyAibote-1.3.8.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 06:45:22.264578 PyAibote-1.3.7/
--rw-rw-rw-   0        0        0     1089 2024-04-11 06:45:22.256578 PyAibote-1.3.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-11 06:45:21.441293 PyAibote-1.3.7/PyAibote/
--rw-rw-rw-   0        0        0     2788 2024-03-19 01:40:59.000000 PyAibote-1.3.7/PyAibote/AndroidBot.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:45:21.665954 PyAibote-1.3.7/PyAibote/AndroidBotModel/
--rw-rw-rw-   0        0        0     7670 2024-02-27 11:01:39.000000 PyAibote-1.3.7/PyAibote/AndroidBotModel/AndroidHidCorrelation.py
--rw-rw-rw-   0        0        0     2401 2024-04-11 06:32:49.000000 PyAibote-1.3.7/PyAibote/AndroidBotModel/AndroidLoadWait.py
--rw-rw-rw-   0        0        0     3104 2024-03-19 01:39:35.000000 PyAibote-1.3.7/PyAibote/AndroidBotModel/ColorFindingOperation.py
--rw-rw-rw-   0        0        0     6238 2024-01-18 22:33:52.000000 PyAibote-1.3.7/PyAibote/AndroidBotModel/Control.py
--rw-rw-rw-   0        0        0     5580 2024-03-19 01:39:35.000000 PyAibote-1.3.7/PyAibote/AndroidBotModel/CoordinateOperation.py
--rw-rw-rw-   0        0        0    13015 2024-01-17 22:58:26.000000 PyAibote-1.3.7/PyAibote/AndroidBotModel/ElementOperation.py
--rw-rw-rw-   0        0        0    16690 2024-03-22 10:35:59.000000 PyAibote-1.3.7/PyAibote/AndroidBotModel/EquipmentOperation.py
--rw-rw-rw-   0        0        0     3094 2024-01-17 08:25:14.000000 PyAibote-1.3.7/PyAibote/AndroidBotModel/FileTransfer.py
--rw-rw-rw-   0        0        0     8280 2024-03-28 05:05:11.000000 PyAibote-1.3.7/PyAibote/AndroidBotModel/MapFindingOperation.py
--rw-rw-rw-   0        0        0     9184 2024-04-11 00:08:51.000000 PyAibote-1.3.7/PyAibote/AndroidBotModel/OcrCorrelation.py
--rw-rw-rw-   0        0        0     1207 2024-01-17 06:31:31.000000 PyAibote-1.3.7/PyAibote/AndroidBotModel/ScreenProjectionOperation.py
--rw-rw-rw-   0        0        0     9303 2024-01-18 00:26:45.000000 PyAibote-1.3.7/PyAibote/AndroidBotModel/ScreenshotOperation.py
--rw-rw-rw-   0        0        0     2012 2024-04-02 11:03:01.000000 PyAibote-1.3.7/PyAibote/AndroidBotModel/UrlRequest.py
--rw-rw-rw-   0        0        0     4476 2024-01-18 22:34:37.000000 PyAibote-1.3.7/PyAibote/AndroidBotModel/VerificationCodeOperation.py
--rw-rw-rw-   0        0        0     1867 2024-01-20 10:06:51.000000 PyAibote-1.3.7/PyAibote/AndroidBotModel/YoloService.py
--rw-rw-rw-   0        0        0     1088 2024-02-27 23:24:38.000000 PyAibote-1.3.7/PyAibote/AndroidBotModel/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:45:21.670957 PyAibote-1.3.7/PyAibote/CommonUse/
--rw-rw-rw-   0        0        0     2101 2024-02-15 23:31:42.000000 PyAibote-1.3.7/PyAibote/CommonUse/ChatGenerative.py
--rw-rw-rw-   0        0        0        0 2024-02-27 23:33:36.000000 PyAibote-1.3.7/PyAibote/CommonUse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:45:21.984573 PyAibote-1.3.7/PyAibote/Tool/
--rw-rw-rw-   0        0        0     5457 2024-03-19 01:40:59.000000 PyAibote-1.3.7/PyAibote/Tool/DatabaseFunc.py
--rw-rw-rw-   0        0        0     2188 2024-03-19 01:39:35.000000 PyAibote-1.3.7/PyAibote/Tool/DebugStartDriver.py
--rw-rw-rw-   0        0        0     2223 2024-03-19 01:40:59.000000 PyAibote-1.3.7/PyAibote/Tool/Logger.py
--rw-rw-rw-   0        0        0     1749 2024-03-19 01:40:59.000000 PyAibote-1.3.7/PyAibote/Tool/LoggerFunc.py
--rw-rw-rw-   0        0        0      912 2024-03-19 01:40:59.000000 PyAibote-1.3.7/PyAibote/Tool/SendTcpData.py
--rw-rw-rw-   0        0        0      532 2024-01-13 09:10:40.000000 PyAibote-1.3.7/PyAibote/Tool/SocketServer.py
--rw-rw-rw-   0        0        0     3342 2024-03-19 01:40:59.000000 PyAibote-1.3.7/PyAibote/Tool/Sqlite3DataBase.py
--rw-rw-rw-   0        0        0      660 2024-01-18 08:34:16.000000 PyAibote-1.3.7/PyAibote/Tool/UniversalFunction.py
--rw-rw-rw-   0        0        0     4364 2024-03-19 01:40:59.000000 PyAibote-1.3.7/PyAibote/Tool/WriteReadFileFunc.py
--rw-rw-rw-   0        0        0      550 2024-03-19 01:40:59.000000 PyAibote-1.3.7/PyAibote/Tool/__init__.py
--rw-rw-rw-   0        0        0     1998 2024-03-19 01:40:59.000000 PyAibote-1.3.7/PyAibote/WebBot.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:45:22.105578 PyAibote-1.3.7/PyAibote/WebBotModel/
--rw-rw-rw-   0        0        0     3645 2024-01-26 01:18:21.000000 PyAibote-1.3.7/PyAibote/WebBotModel/CookiesOperation.py
--rw-rw-rw-   0        0        0      392 2024-01-18 22:24:47.000000 PyAibote-1.3.7/PyAibote/WebBotModel/DrivingOperation.py
--rw-rw-rw-   0        0        0    11550 2024-04-04 13:28:08.000000 PyAibote-1.3.7/PyAibote/WebBotModel/ElementOperation.py
--rw-rw-rw-   0        0        0      697 2024-01-12 10:05:13.000000 PyAibote-1.3.7/PyAibote/WebBotModel/IframeOperation.py
--rw-rw-rw-   0        0        0      890 2024-01-18 22:24:31.000000 PyAibote-1.3.7/PyAibote/WebBotModel/JSinjection.py
--rw-rw-rw-   0        0        0     3592 2024-01-26 00:38:04.000000 PyAibote-1.3.7/PyAibote/WebBotModel/KeymouseOperation.py
--rw-rw-rw-   0        0        0     3993 2024-01-13 12:29:13.000000 PyAibote-1.3.7/PyAibote/WebBotModel/PagesAndNavigation.py
--rw-rw-rw-   0        0        0     1091 2024-01-18 22:23:35.000000 PyAibote-1.3.7/PyAibote/WebBotModel/PopUpWindow.py
--rw-rw-rw-   0        0        0     3433 2024-04-11 06:33:06.000000 PyAibote-1.3.7/PyAibote/WebBotModel/WebLoadWait.py
--rw-rw-rw-   0        0        0     5606 2024-01-25 23:04:37.000000 PyAibote-1.3.7/PyAibote/WebBotModel/WindowOperation.py
--rw-rw-rw-   0        0        0      654 2024-02-15 23:42:13.000000 PyAibote-1.3.7/PyAibote/WebBotModel/__init__.py
--rw-rw-rw-   0        0        0     4186 2024-03-19 01:40:59.000000 PyAibote-1.3.7/PyAibote/WindowsBot.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:45:22.255577 PyAibote-1.3.7/PyAibote/WindowsBotModel/
--rw-rw-rw-   0        0        0    20130 2024-03-28 05:07:36.000000 PyAibote-1.3.7/PyAibote/WindowsBotModel/ColorOperation.py
--rw-rw-rw-   0        0        0    21461 2024-03-28 05:02:42.000000 PyAibote-1.3.7/PyAibote/WindowsBotModel/DigitalHumanOperation.py
--rw-rw-rw-   0        0        0     1824 2024-04-03 02:16:48.000000 PyAibote-1.3.7/PyAibote/WindowsBotModel/DrivingOperation.py
--rw-rw-rw-   0        0        0    14186 2024-01-18 22:29:18.000000 PyAibote-1.3.7/PyAibote/WindowsBotModel/ElementOperation.py
--rw-rw-rw-   0        0        0     5207 2024-01-22 22:39:26.000000 PyAibote-1.3.7/PyAibote/WindowsBotModel/ExcelOperation.py
--rw-rw-rw-   0        0        0     6629 2024-01-13 17:47:39.000000 PyAibote-1.3.7/PyAibote/WindowsBotModel/KeymouseOperation.py
--rw-rw-rw-   0        0        0     8395 2024-03-19 01:39:35.000000 PyAibote-1.3.7/PyAibote/WindowsBotModel/OcrOperation.py
--rw-rw-rw-   0        0        0      703 2024-01-15 07:27:07.000000 PyAibote-1.3.7/PyAibote/WindowsBotModel/OtherOperations.py
--rw-rw-rw-   0        0        0     2379 2024-03-22 11:06:00.000000 PyAibote-1.3.7/PyAibote/WindowsBotModel/SystemOperation.py
--rw-rw-rw-   0        0        0     5962 2024-01-22 23:03:02.000000 PyAibote-1.3.7/PyAibote/WindowsBotModel/VerificationCodeOperation.py
--rw-rw-rw-   0        0        0     6402 2024-01-22 23:49:04.000000 PyAibote-1.3.7/PyAibote/WindowsBotModel/VoiceService.py
--rw-rw-rw-   0        0        0     7513 2024-01-18 22:31:38.000000 PyAibote-1.3.7/PyAibote/WindowsBotModel/WinHidCorrelation.py
--rw-rw-rw-   0        0        0     2424 2024-04-11 06:32:59.000000 PyAibote-1.3.7/PyAibote/WindowsBotModel/WinLoadWait.py
--rw-rw-rw-   0        0        0     7160 2024-01-14 20:16:53.000000 PyAibote-1.3.7/PyAibote/WindowsBotModel/WindowOperation.py
--rw-rw-rw-   0        0        0     2936 2024-01-14 20:29:30.000000 PyAibote-1.3.7/PyAibote/WindowsBotModel/YoloOperation.py
--rw-rw-rw-   0        0        0     1115 2024-02-15 23:42:02.000000 PyAibote-1.3.7/PyAibote/WindowsBotModel/__init__.py
--rw-rw-rw-   0        0        0      277 2024-02-27 10:41:36.000000 PyAibote-1.3.7/PyAibote/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:45:21.470295 PyAibote-1.3.7/PyAibote.egg-info/
--rw-rw-rw-   0        0        0     1089 2024-04-11 06:45:21.000000 PyAibote-1.3.7/PyAibote.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2493 2024-04-11 06:45:21.000000 PyAibote-1.3.7/PyAibote.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 06:45:21.000000 PyAibote-1.3.7/PyAibote.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-04-11 06:45:21.000000 PyAibote-1.3.7/PyAibote.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-11 06:45:21.000000 PyAibote-1.3.7/PyAibote.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8925 2024-03-19 02:24:43.000000 PyAibote-1.3.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-11 06:45:22.264578 PyAibote-1.3.7/setup.cfg
--rw-rw-rw-   0        0        0     1425 2024-04-11 06:44:56.000000 PyAibote-1.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 10:11:42.826027 PyAibote-1.3.8/
+-rw-rw-rw-   0        0        0     1089 2024-04-11 10:11:42.797030 PyAibote-1.3.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-11 10:11:41.927030 PyAibote-1.3.8/PyAibote/
+-rw-rw-rw-   0        0        0     2788 2024-03-19 01:40:59.000000 PyAibote-1.3.8/PyAibote/AndroidBot.py
+drwxrwxrwx   0        0        0        0 2024-04-11 10:11:42.149029 PyAibote-1.3.8/PyAibote/AndroidBotModel/
+-rw-rw-rw-   0        0        0     7670 2024-02-27 11:01:39.000000 PyAibote-1.3.8/PyAibote/AndroidBotModel/AndroidHidCorrelation.py
+-rw-rw-rw-   0        0        0     2401 2024-04-11 06:32:49.000000 PyAibote-1.3.8/PyAibote/AndroidBotModel/AndroidLoadWait.py
+-rw-rw-rw-   0        0        0     3104 2024-03-19 01:39:35.000000 PyAibote-1.3.8/PyAibote/AndroidBotModel/ColorFindingOperation.py
+-rw-rw-rw-   0        0        0     6238 2024-01-18 22:33:52.000000 PyAibote-1.3.8/PyAibote/AndroidBotModel/Control.py
+-rw-rw-rw-   0        0        0     5580 2024-03-19 01:39:35.000000 PyAibote-1.3.8/PyAibote/AndroidBotModel/CoordinateOperation.py
+-rw-rw-rw-   0        0        0    13015 2024-01-17 22:58:26.000000 PyAibote-1.3.8/PyAibote/AndroidBotModel/ElementOperation.py
+-rw-rw-rw-   0        0        0    18473 2024-04-11 09:45:01.000000 PyAibote-1.3.8/PyAibote/AndroidBotModel/EquipmentOperation.py
+-rw-rw-rw-   0        0        0     3094 2024-01-17 08:25:14.000000 PyAibote-1.3.8/PyAibote/AndroidBotModel/FileTransfer.py
+-rw-rw-rw-   0        0        0     8280 2024-03-28 05:05:11.000000 PyAibote-1.3.8/PyAibote/AndroidBotModel/MapFindingOperation.py
+-rw-rw-rw-   0        0        0     9184 2024-04-11 00:08:51.000000 PyAibote-1.3.8/PyAibote/AndroidBotModel/OcrCorrelation.py
+-rw-rw-rw-   0        0        0     1207 2024-01-17 06:31:31.000000 PyAibote-1.3.8/PyAibote/AndroidBotModel/ScreenProjectionOperation.py
+-rw-rw-rw-   0        0        0     9303 2024-01-18 00:26:45.000000 PyAibote-1.3.8/PyAibote/AndroidBotModel/ScreenshotOperation.py
+-rw-rw-rw-   0        0        0     2012 2024-04-02 11:03:01.000000 PyAibote-1.3.8/PyAibote/AndroidBotModel/UrlRequest.py
+-rw-rw-rw-   0        0        0     4476 2024-01-18 22:34:37.000000 PyAibote-1.3.8/PyAibote/AndroidBotModel/VerificationCodeOperation.py
+-rw-rw-rw-   0        0        0     1867 2024-01-20 10:06:51.000000 PyAibote-1.3.8/PyAibote/AndroidBotModel/YoloService.py
+-rw-rw-rw-   0        0        0     1088 2024-02-27 23:24:38.000000 PyAibote-1.3.8/PyAibote/AndroidBotModel/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 10:11:42.153030 PyAibote-1.3.8/PyAibote/CommonUse/
+-rw-rw-rw-   0        0        0     2101 2024-02-15 23:31:42.000000 PyAibote-1.3.8/PyAibote/CommonUse/ChatGenerative.py
+-rw-rw-rw-   0        0        0        0 2024-02-27 23:33:36.000000 PyAibote-1.3.8/PyAibote/CommonUse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 10:11:42.353027 PyAibote-1.3.8/PyAibote/Tool/
+-rw-rw-rw-   0        0        0     5457 2024-03-19 01:40:59.000000 PyAibote-1.3.8/PyAibote/Tool/DatabaseFunc.py
+-rw-rw-rw-   0        0        0     2188 2024-03-19 01:39:35.000000 PyAibote-1.3.8/PyAibote/Tool/DebugStartDriver.py
+-rw-rw-rw-   0        0        0     2223 2024-03-19 01:40:59.000000 PyAibote-1.3.8/PyAibote/Tool/Logger.py
+-rw-rw-rw-   0        0        0     1749 2024-03-19 01:40:59.000000 PyAibote-1.3.8/PyAibote/Tool/LoggerFunc.py
+-rw-rw-rw-   0        0        0      912 2024-03-19 01:40:59.000000 PyAibote-1.3.8/PyAibote/Tool/SendTcpData.py
+-rw-rw-rw-   0        0        0      532 2024-01-13 09:10:40.000000 PyAibote-1.3.8/PyAibote/Tool/SocketServer.py
+-rw-rw-rw-   0        0        0     3342 2024-03-19 01:40:59.000000 PyAibote-1.3.8/PyAibote/Tool/Sqlite3DataBase.py
+-rw-rw-rw-   0        0        0      660 2024-01-18 08:34:16.000000 PyAibote-1.3.8/PyAibote/Tool/UniversalFunction.py
+-rw-rw-rw-   0        0        0     4364 2024-03-19 01:40:59.000000 PyAibote-1.3.8/PyAibote/Tool/WriteReadFileFunc.py
+-rw-rw-rw-   0        0        0      550 2024-03-19 01:40:59.000000 PyAibote-1.3.8/PyAibote/Tool/__init__.py
+-rw-rw-rw-   0        0        0     1998 2024-03-19 01:40:59.000000 PyAibote-1.3.8/PyAibote/WebBot.py
+drwxrwxrwx   0        0        0        0 2024-04-11 10:11:42.548027 PyAibote-1.3.8/PyAibote/WebBotModel/
+-rw-rw-rw-   0        0        0     3645 2024-01-26 01:18:21.000000 PyAibote-1.3.8/PyAibote/WebBotModel/CookiesOperation.py
+-rw-rw-rw-   0        0        0      978 2024-04-11 09:33:52.000000 PyAibote-1.3.8/PyAibote/WebBotModel/DrivingOperation.py
+-rw-rw-rw-   0        0        0    11550 2024-04-04 13:28:08.000000 PyAibote-1.3.8/PyAibote/WebBotModel/ElementOperation.py
+-rw-rw-rw-   0        0        0      697 2024-01-12 10:05:13.000000 PyAibote-1.3.8/PyAibote/WebBotModel/IframeOperation.py
+-rw-rw-rw-   0        0        0      890 2024-01-18 22:24:31.000000 PyAibote-1.3.8/PyAibote/WebBotModel/JSinjection.py
+-rw-rw-rw-   0        0        0     3592 2024-01-26 00:38:04.000000 PyAibote-1.3.8/PyAibote/WebBotModel/KeymouseOperation.py
+-rw-rw-rw-   0        0        0     3993 2024-01-13 12:29:13.000000 PyAibote-1.3.8/PyAibote/WebBotModel/PagesAndNavigation.py
+-rw-rw-rw-   0        0        0     1091 2024-01-18 22:23:35.000000 PyAibote-1.3.8/PyAibote/WebBotModel/PopUpWindow.py
+-rw-rw-rw-   0        0        0     3433 2024-04-11 06:33:06.000000 PyAibote-1.3.8/PyAibote/WebBotModel/WebLoadWait.py
+-rw-rw-rw-   0        0        0     5606 2024-01-25 23:04:37.000000 PyAibote-1.3.8/PyAibote/WebBotModel/WindowOperation.py
+-rw-rw-rw-   0        0        0      654 2024-02-15 23:42:13.000000 PyAibote-1.3.8/PyAibote/WebBotModel/__init__.py
+-rw-rw-rw-   0        0        0     4186 2024-03-19 01:40:59.000000 PyAibote-1.3.8/PyAibote/WindowsBot.py
+drwxrwxrwx   0        0        0        0 2024-04-11 10:11:42.795028 PyAibote-1.3.8/PyAibote/WindowsBotModel/
+-rw-rw-rw-   0        0        0    20130 2024-03-28 05:07:36.000000 PyAibote-1.3.8/PyAibote/WindowsBotModel/ColorOperation.py
+-rw-rw-rw-   0        0        0    21461 2024-03-28 05:02:42.000000 PyAibote-1.3.8/PyAibote/WindowsBotModel/DigitalHumanOperation.py
+-rw-rw-rw-   0        0        0     1824 2024-04-03 02:16:48.000000 PyAibote-1.3.8/PyAibote/WindowsBotModel/DrivingOperation.py
+-rw-rw-rw-   0        0        0    14186 2024-01-18 22:29:18.000000 PyAibote-1.3.8/PyAibote/WindowsBotModel/ElementOperation.py
+-rw-rw-rw-   0        0        0     5207 2024-01-22 22:39:26.000000 PyAibote-1.3.8/PyAibote/WindowsBotModel/ExcelOperation.py
+-rw-rw-rw-   0        0        0     6629 2024-01-13 17:47:39.000000 PyAibote-1.3.8/PyAibote/WindowsBotModel/KeymouseOperation.py
+-rw-rw-rw-   0        0        0     8395 2024-03-19 01:39:35.000000 PyAibote-1.3.8/PyAibote/WindowsBotModel/OcrOperation.py
+-rw-rw-rw-   0        0        0      703 2024-01-15 07:27:07.000000 PyAibote-1.3.8/PyAibote/WindowsBotModel/OtherOperations.py
+-rw-rw-rw-   0        0        0     2379 2024-03-22 11:06:00.000000 PyAibote-1.3.8/PyAibote/WindowsBotModel/SystemOperation.py
+-rw-rw-rw-   0        0        0     5962 2024-01-22 23:03:02.000000 PyAibote-1.3.8/PyAibote/WindowsBotModel/VerificationCodeOperation.py
+-rw-rw-rw-   0        0        0     6402 2024-01-22 23:49:04.000000 PyAibote-1.3.8/PyAibote/WindowsBotModel/VoiceService.py
+-rw-rw-rw-   0        0        0     7513 2024-01-18 22:31:38.000000 PyAibote-1.3.8/PyAibote/WindowsBotModel/WinHidCorrelation.py
+-rw-rw-rw-   0        0        0     2424 2024-04-11 06:32:59.000000 PyAibote-1.3.8/PyAibote/WindowsBotModel/WinLoadWait.py
+-rw-rw-rw-   0        0        0     8941 2024-04-11 09:46:20.000000 PyAibote-1.3.8/PyAibote/WindowsBotModel/WindowOperation.py
+-rw-rw-rw-   0        0        0     2936 2024-01-14 20:29:30.000000 PyAibote-1.3.8/PyAibote/WindowsBotModel/YoloOperation.py
+-rw-rw-rw-   0        0        0     1115 2024-02-15 23:42:02.000000 PyAibote-1.3.8/PyAibote/WindowsBotModel/__init__.py
+-rw-rw-rw-   0        0        0      277 2024-02-27 10:41:36.000000 PyAibote-1.3.8/PyAibote/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 10:11:42.040027 PyAibote-1.3.8/PyAibote.egg-info/
+-rw-rw-rw-   0        0        0     1089 2024-04-11 10:11:41.000000 PyAibote-1.3.8/PyAibote.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2493 2024-04-11 10:11:41.000000 PyAibote-1.3.8/PyAibote.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 10:11:41.000000 PyAibote-1.3.8/PyAibote.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-11 10:11:41.000000 PyAibote-1.3.8/PyAibote.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-11 10:11:41.000000 PyAibote-1.3.8/PyAibote.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9118 2024-04-11 10:04:43.000000 PyAibote-1.3.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-11 10:11:42.826027 PyAibote-1.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     1425 2024-04-11 10:08:00.000000 PyAibote-1.3.8/setup.py
```

### Comparing `PyAibote-1.3.7/PKG-INFO` & `PyAibote-1.3.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAibote
-Version: 1.3.7
+Version: 1.3.8
 Summary: A pure code RPA office automation framework, which supports Android, Browser and Windows
 Home-page: https://www.pyaibote.com
 Author: Riven
 Author-email: pyaibote@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7,<4.0
```

### Comparing `PyAibote-1.3.7/PyAibote/AndroidBot.py` & `PyAibote-1.3.8/PyAibote/AndroidBot.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/AndroidBotModel/AndroidHidCorrelation.py` & `PyAibote-1.3.8/PyAibote/AndroidBotModel/AndroidHidCorrelation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/AndroidBotModel/AndroidLoadWait.py` & `PyAibote-1.3.8/PyAibote/AndroidBotModel/AndroidLoadWait.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/AndroidBotModel/ColorFindingOperation.py` & `PyAibote-1.3.8/PyAibote/AndroidBotModel/ColorFindingOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/AndroidBotModel/Control.py` & `PyAibote-1.3.8/PyAibote/AndroidBotModel/Control.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/AndroidBotModel/CoordinateOperation.py` & `PyAibote-1.3.8/PyAibote/AndroidBotModel/CoordinateOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/AndroidBotModel/ElementOperation.py` & `PyAibote-1.3.8/PyAibote/AndroidBotModel/ElementOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/AndroidBotModel/EquipmentOperation.py` & `PyAibote-1.3.8/PyAibote/AndroidBotModel/EquipmentOperation.py`

 * *Files 6% similar despite different names*

```diff
@@ -450,14 +450,54 @@
             remote_path: Android file path.
             return: Returns True successfully, and returns False if it fails
         """
         if not remote_path.startswith("/storage/emulated/0/"):
             remote_path = "/storage/emulated/0/" + remote_path
         return "true" in self.SendData("deleteAndroidFile", remote_path) 
 
+    def coordinate_transform(self, coordinate: tuple, resolution_a: tuple, resolution_b: tuple) -> tuple:
+        """
+            根据屏幕分辨率缩放比例，进行不同分辨率坐标转换
+            According to the screen resolution scaling, coordinate conversion with different resolutions is carried out.
+
+            coordinate: 需要装换的坐标可以是x,y坐标，也可以是矩形坐标 x1, y1, x2, y2
+            resolution_a: 你抓取过坐标的设备标准分辨率
+            resolution_b：你需要转换的设备分辨率
+            retrun: 元祖
+
+            coordinate: the coordinates to be replaced can be x,y coordinates or rectangular coordinates x1, y1, x2, y2
+            resolution_a: The standard resolution of the device for which you have grabbed the coordinates
+            resolution_b: The device resolution you need to convert
+            retrun: Yuanzu
+        """
+        
+        def convert_coordinates(x, y, resolution_a, resolution_b):
+            W_A, H_A = resolution_a  
+            W_B, H_B = resolution_b 
+            
+
+            scale_x = W_B / W_A
+            scale_y = H_B / H_A
+            
+
+            x_b = x * scale_x
+            y_b = y * scale_y
+            
+            return (x_b, y_b)
+
+        if len(coordinate) == 2:
+            result = convert_coordinates(coordinate[0], coordinate[1], resolution_a, resolution_b)
+            return result
+
+        if len(coordinate) == 4:
+            result = convert_coordinates(coordinate[0], coordinate[1], resolution_a, resolution_b)
+            result2 = convert_coordinates(coordinate[2], coordinate[3], resolution_a, resolution_b)
+            return (result[0], result[1], result2[0], result2[1])
+        return ()
+
     def close_driver(self):
         """
             关闭连接
             Close the connection
         """
         self.SendData("closeDriver")
```

### Comparing `PyAibote-1.3.7/PyAibote/AndroidBotModel/FileTransfer.py` & `PyAibote-1.3.8/PyAibote/AndroidBotModel/FileTransfer.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/AndroidBotModel/MapFindingOperation.py` & `PyAibote-1.3.8/PyAibote/AndroidBotModel/MapFindingOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/AndroidBotModel/OcrCorrelation.py` & `PyAibote-1.3.8/PyAibote/AndroidBotModel/OcrCorrelation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/AndroidBotModel/ScreenProjectionOperation.py` & `PyAibote-1.3.8/PyAibote/AndroidBotModel/ScreenProjectionOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/AndroidBotModel/ScreenshotOperation.py` & `PyAibote-1.3.8/PyAibote/AndroidBotModel/ScreenshotOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/AndroidBotModel/UrlRequest.py` & `PyAibote-1.3.8/PyAibote/AndroidBotModel/UrlRequest.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/AndroidBotModel/VerificationCodeOperation.py` & `PyAibote-1.3.8/PyAibote/AndroidBotModel/VerificationCodeOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/AndroidBotModel/YoloService.py` & `PyAibote-1.3.8/PyAibote/AndroidBotModel/YoloService.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/AndroidBotModel/__init__.py` & `PyAibote-1.3.8/PyAibote/AndroidBotModel/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/CommonUse/ChatGenerative.py` & `PyAibote-1.3.8/PyAibote/CommonUse/ChatGenerative.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/Tool/DatabaseFunc.py` & `PyAibote-1.3.8/PyAibote/Tool/DatabaseFunc.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/Tool/DebugStartDriver.py` & `PyAibote-1.3.8/PyAibote/Tool/DebugStartDriver.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/Tool/Logger.py` & `PyAibote-1.3.8/PyAibote/Tool/Logger.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/Tool/LoggerFunc.py` & `PyAibote-1.3.8/PyAibote/Tool/LoggerFunc.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/Tool/SendTcpData.py` & `PyAibote-1.3.8/PyAibote/Tool/SendTcpData.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/Tool/SocketServer.py` & `PyAibote-1.3.8/PyAibote/Tool/SocketServer.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/Tool/Sqlite3DataBase.py` & `PyAibote-1.3.8/PyAibote/Tool/Sqlite3DataBase.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/Tool/UniversalFunction.py` & `PyAibote-1.3.8/PyAibote/Tool/UniversalFunction.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/Tool/WriteReadFileFunc.py` & `PyAibote-1.3.8/PyAibote/Tool/WriteReadFileFunc.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/Tool/__init__.py` & `PyAibote-1.3.8/PyAibote/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/WebBot.py` & `PyAibote-1.3.8/PyAibote/WebBot.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/WebBotModel/CookiesOperation.py` & `PyAibote-1.3.8/PyAibote/WebBotModel/CookiesOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/WebBotModel/ElementOperation.py` & `PyAibote-1.3.8/PyAibote/WebBotModel/ElementOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/WebBotModel/IframeOperation.py` & `PyAibote-1.3.8/PyAibote/WebBotModel/IframeOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/WebBotModel/JSinjection.py` & `PyAibote-1.3.8/PyAibote/WebBotModel/JSinjection.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/WebBotModel/KeymouseOperation.py` & `PyAibote-1.3.8/PyAibote/WebBotModel/KeymouseOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/WebBotModel/PagesAndNavigation.py` & `PyAibote-1.3.8/PyAibote/WebBotModel/PagesAndNavigation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/WebBotModel/PopUpWindow.py` & `PyAibote-1.3.8/PyAibote/WebBotModel/PopUpWindow.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/WebBotModel/WebLoadWait.py` & `PyAibote-1.3.8/PyAibote/WebBotModel/WebLoadWait.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/WebBotModel/WindowOperation.py` & `PyAibote-1.3.8/PyAibote/WebBotModel/WindowOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/WebBotModel/__init__.py` & `PyAibote-1.3.8/PyAibote/WebBotModel/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/WindowsBot.py` & `PyAibote-1.3.8/PyAibote/WindowsBot.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/WindowsBotModel/ColorOperation.py` & `PyAibote-1.3.8/PyAibote/WindowsBotModel/ColorOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/WindowsBotModel/DigitalHumanOperation.py` & `PyAibote-1.3.8/PyAibote/WindowsBotModel/DigitalHumanOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/WindowsBotModel/DrivingOperation.py` & `PyAibote-1.3.8/PyAibote/WindowsBotModel/DrivingOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/WindowsBotModel/ElementOperation.py` & `PyAibote-1.3.8/PyAibote/WindowsBotModel/ElementOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/WindowsBotModel/ExcelOperation.py` & `PyAibote-1.3.8/PyAibote/WindowsBotModel/ExcelOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/WindowsBotModel/KeymouseOperation.py` & `PyAibote-1.3.8/PyAibote/WindowsBotModel/KeymouseOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/WindowsBotModel/OcrOperation.py` & `PyAibote-1.3.8/PyAibote/WindowsBotModel/OcrOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/WindowsBotModel/OtherOperations.py` & `PyAibote-1.3.8/PyAibote/WindowsBotModel/OtherOperations.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/WindowsBotModel/SystemOperation.py` & `PyAibote-1.3.8/PyAibote/WindowsBotModel/SystemOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/WindowsBotModel/VerificationCodeOperation.py` & `PyAibote-1.3.8/PyAibote/WindowsBotModel/VerificationCodeOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/WindowsBotModel/VoiceService.py` & `PyAibote-1.3.8/PyAibote/WindowsBotModel/VoiceService.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/WindowsBotModel/WinHidCorrelation.py` & `PyAibote-1.3.8/PyAibote/WindowsBotModel/WinHidCorrelation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/WindowsBotModel/WinLoadWait.py` & `PyAibote-1.3.8/PyAibote/WindowsBotModel/WinLoadWait.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/WindowsBotModel/WindowOperation.py` & `PyAibote-1.3.8/PyAibote/WindowsBotModel/WindowOperation.py`

 * *Files 17% similar despite different names*

```diff
@@ -196,7 +196,47 @@
             return: 布尔值
 
             hwnd: Current window handle
             top: Set top or not, True set top, False cancel set top
             return: bool
         """
         return "true" in self.SendData("setWindowTop", hwnd, top)
+
+    def coordinate_transform(self, coordinate: tuple, resolution_a: tuple, resolution_b: tuple) -> tuple:
+        """
+            根据屏幕分辨率缩放比例，进行不同分辨率坐标转换
+            According to the screen resolution scaling, coordinate conversion with different resolutions is carried out.
+
+            coordinate: 需要装换的坐标可以是x,y坐标，也可以是矩形坐标 x1, y1, x2, y2
+            resolution_a: 你抓取过坐标的设备标准分辨率
+            resolution_b：你需要转换的设备分辨率
+            retrun: 元祖
+
+            coordinate: the coordinates to be replaced can be x,y coordinates or rectangular coordinates x1, y1, x2, y2
+            resolution_a: The standard resolution of the device for which you have grabbed the coordinates
+            resolution_b: The device resolution you need to convert
+            retrun: Yuanzu
+        """
+        
+        def convert_coordinates(x, y, resolution_a, resolution_b):
+            W_A, H_A = resolution_a  
+            W_B, H_B = resolution_b 
+            
+
+            scale_x = W_B / W_A
+            scale_y = H_B / H_A
+            
+
+            x_b = x * scale_x
+            y_b = y * scale_y
+            
+            return (x_b, y_b)
+
+        if len(coordinate) == 2:
+            result = convert_coordinates(coordinate[0], coordinate[1], resolution_a, resolution_b)
+            return result
+
+        if len(coordinate) == 4:
+            result = convert_coordinates(coordinate[0], coordinate[1], resolution_a, resolution_b)
+            result2 = convert_coordinates(coordinate[2], coordinate[3], resolution_a, resolution_b)
+            return (result[0], result[1], result2[0], result2[1])
+        return ()
```

### Comparing `PyAibote-1.3.7/PyAibote/WindowsBotModel/YoloOperation.py` & `PyAibote-1.3.8/PyAibote/WindowsBotModel/YoloOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote/WindowsBotModel/__init__.py` & `PyAibote-1.3.8/PyAibote/WindowsBotModel/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/PyAibote.egg-info/PKG-INFO` & `PyAibote-1.3.8/PyAibote.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAibote
-Version: 1.3.7
+Version: 1.3.8
 Summary: A pure code RPA office automation framework, which supports Android, Browser and Windows
 Home-page: https://www.pyaibote.com
 Author: Riven
 Author-email: pyaibote@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7,<4.0
```

### Comparing `PyAibote-1.3.7/PyAibote.egg-info/SOURCES.txt` & `PyAibote-1.3.8/PyAibote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.7/README.md` & `PyAibote-1.3.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -189,12 +189,12 @@
     # 7.3. 如本地部署脚本，需要传递 WebDriver 启动参数时，参考下面方式，如不需传递启动参数，则忽略：
     # 7.3. For local deployment scripts, when the WebDriver startup parameters need to be passed, please refer to the following methods. If the startup parameters don't need to be passed, ignore them:
     driver_params = {
         "browserName": "chrome",
         "debugPort": 0,
         "userDataDir": "./UserData",
         "browserPath": None,
-        "argument": None,
+        "argument": None   # 无头模式(后台运行浏览器)启动参数: --headless   浏览器版本大于112 的无头模式:--headless=new，多个启动参数空格隔开，示例: "argument": "--headless=new"
     }
 
     CustomWebScript.execute("0.0.0.0", 9999, Debug=True, Driver_Params=driver_params)
 ```
```

### Comparing `PyAibote-1.3.7/setup.py` & `PyAibote-1.3.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "Pillow",
     "requests",
     "pymysql"
 ]
 
 setup(
     name="PyAibote", 
-    version="1.3.7", 
+    version="1.3.8", 
     author="Riven", 
     author_email="pyaibote@163.com", 
     description="A pure code RPA office automation framework, which supports Android, Browser and Windows", 
     long_description="Support Android native APP and H5 interface elements and color positioning. The speed of element location is 10 times that of Appium framework, and the color location of 2340*1080 image only takes 50 milliseconds, It supports the positioning of window interface elements and colors developed by Windows applications,. NET, WinForm, WPF, QT, Java (GUI libraries such JAVA(Swing and AWT) and Electron. The exclusive xpath algorithm is concise and rapid, and the positioning speed of elements/colors is 3 times and 20 times that of visual RPA, respectively, All browsers and applications that support the chromium kernel. A web automation framework developed by C/C++ language based on browser kernel protocol. Ten times faster than Selenium", # 加载read_me的内容
     long_description_content_type="text/markdown", 
     url="https://www.pyaibote.com",  
     packages=packages,
```

