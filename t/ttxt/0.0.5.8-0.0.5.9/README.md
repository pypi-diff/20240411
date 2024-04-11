# Comparing `tmp/ttxt-0.0.5.8.tar.gz` & `tmp/ttxt-0.0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttxt-0.0.5.8.tar", last modified: Thu Apr  4 18:31:54 2024, max compression
+gzip compressed data, was "ttxt-0.0.5.9.tar", last modified: Thu Apr 11 11:55:59 2024, max compression
```

## Comparing `ttxt-0.0.5.8.tar` & `ttxt-0.0.5.9.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-04 18:31:54.309857 ttxt-0.0.5.8/
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11357 2023-11-29 00:08:24.000000 ttxt-0.0.5.8/LICENSE
--rw-r--r--   0 sushantkumar   (501) staff       (20)      125 2024-04-04 18:31:54.309693 ttxt-0.0.5.8/PKG-INFO
--rw-r--r--   0 sushantkumar   (501) staff       (20)       58 2023-11-29 00:08:24.000000 ttxt-0.0.5.8/README.md
--rw-r--r--   0 sushantkumar   (501) staff       (20)       38 2024-04-04 18:31:54.309912 ttxt-0.0.5.8/setup.cfg
--rw-r--r--   0 sushantkumar   (501) staff       (20)      306 2024-04-04 18:31:48.000000 ttxt-0.0.5.8/setup.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-04 18:31:54.301385 ttxt-0.0.5.8/ttxt/
--rw-r--r--   0 sushantkumar   (501) staff       (20)     1040 2024-03-14 11:17:46.000000 ttxt-0.0.5.8/ttxt/__init__.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-04 18:31:54.302446 ttxt-0.0.5.8/ttxt/base/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-13 13:39:15.000000 ttxt-0.0.5.8/ttxt/base/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)     1394 2024-01-23 17:20:28.000000 ttxt-0.0.5.8/ttxt/base/baseFuturesExchange.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)     1224 2024-03-14 09:27:50.000000 ttxt-0.0.5.8/ttxt/base/baseSpotExchange.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-04 18:31:54.307707 ttxt-0.0.5.8/ttxt/exchanges/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-06 13:36:21.000000 ttxt-0.0.5.8/ttxt/exchanges/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    13324 2023-12-21 12:03:19.000000 ttxt-0.0.5.8/ttxt/exchanges/biconomy.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)     9966 2024-03-22 17:14:03.000000 ttxt-0.0.5.8/ttxt/exchanges/binance.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    13165 2024-03-22 17:15:32.000000 ttxt-0.0.5.8/ttxt/exchanges/bingx.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    12850 2024-03-22 17:15:07.000000 ttxt-0.0.5.8/ttxt/exchanges/bitget.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    10504 2024-01-26 15:22:11.000000 ttxt-0.0.5.8/ttxt/exchanges/bitgetFutures.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    12255 2024-03-22 17:15:48.000000 ttxt-0.0.5.8/ttxt/exchanges/bitmart.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    20701 2024-03-30 03:47:36.000000 ttxt-0.0.5.8/ttxt/exchanges/bybit.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    17967 2024-01-23 17:20:48.000000 ttxt-0.0.5.8/ttxt/exchanges/bybitFutures.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11712 2024-03-22 17:16:03.000000 ttxt-0.0.5.8/ttxt/exchanges/cryptocom.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    14163 2024-03-11 15:19:34.000000 ttxt-0.0.5.8/ttxt/exchanges/gateFutures.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    15302 2024-03-22 17:13:33.000000 ttxt-0.0.5.8/ttxt/exchanges/gateio.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    14560 2024-03-29 07:17:38.000000 ttxt-0.0.5.8/ttxt/exchanges/huobi.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11284 2024-03-22 17:12:44.000000 ttxt-0.0.5.8/ttxt/exchanges/kucoin.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11671 2024-03-22 17:16:57.000000 ttxt-0.0.5.8/ttxt/exchanges/mexc.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11747 2024-04-04 18:31:35.000000 ttxt-0.0.5.8/ttxt/exchanges/okx.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-19 13:51:46.000000 ttxt-0.0.5.8/ttxt/exchanges/xt.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-04 18:31:54.307910 ttxt-0.0.5.8/ttxt/tests/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-06 13:02:46.000000 ttxt-0.0.5.8/ttxt/tests/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)     9606 2024-04-04 18:26:15.000000 ttxt-0.0.5.8/ttxt/tests/testExchange.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-04 18:31:54.308172 ttxt-0.0.5.8/ttxt/types/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-13 13:42:34.000000 ttxt-0.0.5.8/ttxt/types/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)     1428 2023-12-28 02:37:11.000000 ttxt-0.0.5.8/ttxt/types/baseTypes.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-04 18:31:54.308879 ttxt-0.0.5.8/ttxt/utils/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-20 23:39:43.000000 ttxt-0.0.5.8/ttxt/utils/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)      778 2024-03-11 15:19:34.000000 ttxt-0.0.5.8/ttxt/utils/general.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    42572 2023-12-20 23:39:43.000000 ttxt-0.0.5.8/ttxt/utils/xtUtils.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-04 18:31:54.301919 ttxt-0.0.5.8/ttxt.egg-info/
--rw-r--r--   0 sushantkumar   (501) staff       (20)      125 2024-04-04 18:31:54.000000 ttxt-0.0.5.8/ttxt.egg-info/PKG-INFO
--rw-r--r--   0 sushantkumar   (501) staff       (20)      844 2024-04-04 18:31:54.000000 ttxt-0.0.5.8/ttxt.egg-info/SOURCES.txt
--rw-r--r--   0 sushantkumar   (501) staff       (20)        1 2024-04-04 18:31:54.000000 ttxt-0.0.5.8/ttxt.egg-info/dependency_links.txt
--rw-r--r--   0 sushantkumar   (501) staff       (20)        5 2024-04-04 18:31:54.000000 ttxt-0.0.5.8/ttxt.egg-info/top_level.txt
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-11 11:55:59.840091 ttxt-0.0.5.9/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11357 2023-11-29 00:08:24.000000 ttxt-0.0.5.9/LICENSE
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      125 2024-04-11 11:55:59.839921 ttxt-0.0.5.9/PKG-INFO
+-rw-r--r--   0 sushantkumar   (501) staff       (20)       58 2023-11-29 00:08:24.000000 ttxt-0.0.5.9/README.md
+-rw-r--r--   0 sushantkumar   (501) staff       (20)       38 2024-04-11 11:55:59.840144 ttxt-0.0.5.9/setup.cfg
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      306 2024-04-11 11:55:36.000000 ttxt-0.0.5.9/setup.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-11 11:55:59.828086 ttxt-0.0.5.9/ttxt/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     1101 2024-04-05 05:36:17.000000 ttxt-0.0.5.9/ttxt/__init__.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-11 11:55:59.829137 ttxt-0.0.5.9/ttxt/base/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-13 13:39:15.000000 ttxt-0.0.5.9/ttxt/base/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     1394 2024-01-23 17:20:28.000000 ttxt-0.0.5.9/ttxt/base/baseFuturesExchange.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     1224 2024-03-14 09:27:50.000000 ttxt-0.0.5.9/ttxt/base/baseSpotExchange.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-11 11:55:59.837544 ttxt-0.0.5.9/ttxt/exchanges/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-06 13:36:21.000000 ttxt-0.0.5.9/ttxt/exchanges/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11279 2024-04-06 07:37:14.000000 ttxt-0.0.5.9/ttxt/exchanges/ascendex.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    13324 2023-12-21 12:03:19.000000 ttxt-0.0.5.9/ttxt/exchanges/biconomy.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     9966 2024-03-22 17:14:03.000000 ttxt-0.0.5.9/ttxt/exchanges/binance.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    13165 2024-03-22 17:15:32.000000 ttxt-0.0.5.9/ttxt/exchanges/bingx.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    12850 2024-03-22 17:15:07.000000 ttxt-0.0.5.9/ttxt/exchanges/bitget.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    10504 2024-01-26 15:22:11.000000 ttxt-0.0.5.9/ttxt/exchanges/bitgetFutures.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    12255 2024-03-22 17:15:48.000000 ttxt-0.0.5.9/ttxt/exchanges/bitmart.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    20707 2024-04-11 11:55:19.000000 ttxt-0.0.5.9/ttxt/exchanges/bybit.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    17967 2024-01-23 17:20:48.000000 ttxt-0.0.5.9/ttxt/exchanges/bybitFutures.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11712 2024-03-22 17:16:03.000000 ttxt-0.0.5.9/ttxt/exchanges/cryptocom.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    14163 2024-03-11 15:19:34.000000 ttxt-0.0.5.9/ttxt/exchanges/gateFutures.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    15302 2024-03-22 17:13:33.000000 ttxt-0.0.5.9/ttxt/exchanges/gateio.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    14560 2024-03-29 07:17:38.000000 ttxt-0.0.5.9/ttxt/exchanges/huobi.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11284 2024-03-22 17:12:44.000000 ttxt-0.0.5.9/ttxt/exchanges/kucoin.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11671 2024-03-22 17:16:57.000000 ttxt-0.0.5.9/ttxt/exchanges/mexc.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11747 2024-04-05 05:36:24.000000 ttxt-0.0.5.9/ttxt/exchanges/okx.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-19 13:51:46.000000 ttxt-0.0.5.9/ttxt/exchanges/xt.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-11 11:55:59.837789 ttxt-0.0.5.9/ttxt/tests/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-06 13:02:46.000000 ttxt-0.0.5.9/ttxt/tests/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     9863 2024-04-06 07:37:14.000000 ttxt-0.0.5.9/ttxt/tests/testExchange.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-11 11:55:59.838286 ttxt-0.0.5.9/ttxt/types/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-13 13:42:34.000000 ttxt-0.0.5.9/ttxt/types/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     1428 2023-12-28 02:37:11.000000 ttxt-0.0.5.9/ttxt/types/baseTypes.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-11 11:55:59.838968 ttxt-0.0.5.9/ttxt/utils/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-20 23:39:43.000000 ttxt-0.0.5.9/ttxt/utils/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      778 2024-03-11 15:19:34.000000 ttxt-0.0.5.9/ttxt/utils/general.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    42572 2023-12-20 23:39:43.000000 ttxt-0.0.5.9/ttxt/utils/xtUtils.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-11 11:55:59.828686 ttxt-0.0.5.9/ttxt.egg-info/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      125 2024-04-11 11:55:59.000000 ttxt-0.0.5.9/ttxt.egg-info/PKG-INFO
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      871 2024-04-11 11:55:59.000000 ttxt-0.0.5.9/ttxt.egg-info/SOURCES.txt
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        1 2024-04-11 11:55:59.000000 ttxt-0.0.5.9/ttxt.egg-info/dependency_links.txt
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        5 2024-04-11 11:55:59.000000 ttxt-0.0.5.9/ttxt.egg-info/top_level.txt
```

### Comparing `ttxt-0.0.5.8/LICENSE` & `ttxt-0.0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.8/ttxt/__init__.py` & `ttxt-0.0.5.9/ttxt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from ttxt.base import baseFuturesExchange, baseSpotExchange
+from ttxt.exchanges.ascendex import ascendex
 from ttxt.exchanges.gateFutures import gateFutures
 from ttxt.exchanges.bybitFutures import bybitFutures
 from ttxt.exchanges.bitgetFutures import bitgetFutures
 from ttxt.exchanges.bingx import bingx
 from ttxt.exchanges.biconomy import biconomy
 from ttxt.exchanges.mexc import mexc
 from ttxt.exchanges.gateio import gateio
@@ -12,14 +13,15 @@
 from ttxt.exchanges.bitmart import bitmart
 from ttxt.exchanges.cryptocom import cryptocom
 from ttxt.exchanges.bitget import bitget
 from ttxt.exchanges.binance import binance
 from ttxt.exchanges.kucoin import kucoin
 
 exchanges = [
+    "ascendex",
     "biconomy",
     "binance",
     "bingx",
     "bitgetFutures",
     "bitget",
     "bybitFutures",
     "gateFutures",
```

### Comparing `ttxt-0.0.5.8/ttxt/base/baseFuturesExchange.py` & `ttxt-0.0.5.9/ttxt/base/baseFuturesExchange.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.8/ttxt/base/baseSpotExchange.py` & `ttxt-0.0.5.9/ttxt/base/baseSpotExchange.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.8/ttxt/exchanges/biconomy.py` & `ttxt-0.0.5.9/ttxt/exchanges/biconomy.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.8/ttxt/exchanges/binance.py` & `ttxt-0.0.5.9/ttxt/exchanges/binance.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.8/ttxt/exchanges/bingx.py` & `ttxt-0.0.5.9/ttxt/exchanges/bingx.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.8/ttxt/exchanges/bitget.py` & `ttxt-0.0.5.9/ttxt/exchanges/bitget.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.8/ttxt/exchanges/bitgetFutures.py` & `ttxt-0.0.5.9/ttxt/exchanges/bitgetFutures.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.8/ttxt/exchanges/bitmart.py` & `ttxt-0.0.5.9/ttxt/exchanges/bitmart.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.8/ttxt/exchanges/bybit.py` & `ttxt-0.0.5.9/ttxt/exchanges/bybit.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,15 +396,15 @@
     def create_limit_order(self, symbol, amount, side, price, params={}):
         ticker = self._getSymbol(symbol)
         body = {
             "category": self.category,
             "symbol": ticker,
             "isLeverage": params["isLeverage"] if "isLeverage" in params else 0,  # 1 is for margin, 0 for spot
             "side": side.capitalize(),
-            "orderType": "Limit",
+            "orderType": "Limit-Maker",
             "qty": float(amount),
             "price": float(price),
             "timeInForce": params["timeInForce"] if "timeInForce" in params else "GTC",
             "positionIdx": params["positionIdx"] if "positionIdx" in params else 0,
         }
         apiUrl = "/v5/order/create"
         try:
```

### Comparing `ttxt-0.0.5.8/ttxt/exchanges/bybitFutures.py` & `ttxt-0.0.5.9/ttxt/exchanges/bybitFutures.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.8/ttxt/exchanges/cryptocom.py` & `ttxt-0.0.5.9/ttxt/exchanges/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.8/ttxt/exchanges/gateFutures.py` & `ttxt-0.0.5.9/ttxt/exchanges/gateFutures.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.8/ttxt/exchanges/gateio.py` & `ttxt-0.0.5.9/ttxt/exchanges/gateio.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.8/ttxt/exchanges/huobi.py` & `ttxt-0.0.5.9/ttxt/exchanges/huobi.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.8/ttxt/exchanges/kucoin.py` & `ttxt-0.0.5.9/ttxt/exchanges/kucoin.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.8/ttxt/exchanges/mexc.py` & `ttxt-0.0.5.9/ttxt/exchanges/mexc.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.8/ttxt/exchanges/okx.py` & `ttxt-0.0.5.9/ttxt/exchanges/okx.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.8/ttxt/tests/testExchange.py` & `ttxt-0.0.5.9/ttxt/tests/testExchange.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 DIR_NAME = os.path.dirname(os.path.abspath(__file__))
 root = os.path.dirname(os.path.dirname(DIR_NAME))
 sys.path.append(root)
 
 import ttxt
 
 def getTtxtExchange(exchangeName):
+    if exchangeName == "ascendex":
+        print('returned ascendex')
+        return ttxt.ascendex(key=os.getenv("KEY"), secret=os.getenv("SECRET"), password=os.getenv("PASSWORD"))
     if exchangeName == "gateFutures":
         print("returned gateFuture")
         return ttxt.gateFutures(key=os.getenv("KEY"), secret=os.getenv("SECRET"))
     if exchangeName == "bybitFutures":
         print("returned bybitFutures")
         return ttxt.bybitFutures(key=os.getenv("KEY"), secret=os.getenv("SECRET"))
     if exchangeName == "bitgetFutures":
@@ -78,23 +81,23 @@
             print(resp)
         except Exception as e:
             print("balance could not be fetched")
             print(e)
     if "createOrder" in params and params["createOrder"]:
         print("testing create order...")
         try:
-            resp = ttxtExchange.create_order(symbol=tickerToTest, order_type="limit", amount="5", side="sell", price=5)
+            resp = ttxtExchange.create_order(symbol=tickerToTest, order_type="market", amount="50", side="sell", price=0.3)
             print(f"createOrder response: {resp}")
         except Exception as e:
             print("order could not be created")
             print(e)
     if "createLimitOrder" in params and params["createLimitOrder"]:
         print("testing limit create order...")
         try:
-            resp = ttxtExchange.create_limit_order(symbol=tickerToTest, amount=50, side="buy", price=0.20)
+            resp = ttxtExchange.create_limit_order(symbol=tickerToTest, amount=50, side="buy", price=0.2)
             print(f"createLimitOrder response: {resp}")
         except Exception as e:
             print("limit order could not be created")
             print(e)
     if "createMarketSellOrder" in params and params["createMarketSellOrder"]:
         print("testing market sell create order...")
         try:
@@ -110,31 +113,31 @@
             print(f"createMarketBuyOrder response: {resp}")
         except Exception as e:
             print("market buy order could not be created")
             print(e)
     if "create_market_order" in params and params["create_market_order"]:
         print("testing create market order...")
         try:
-            resp = ttxtExchange.create_market_order(symbol=tickerToTest, side="sell", amount=1)
+            resp = ttxtExchange.create_market_order(symbol=tickerToTest, side="sell", amount=50)
             print(f"create_market_order response: {resp}")
         except Exception as e:
             print("market order could not be created")
             print(e)
     if "fetchOrder" in params and params["fetchOrder"]:
         print("testing fetch order...")
         try:
-            resp = ttxtExchange.fetch_order(id=45577069671, symbol=tickerToTest)
+            resp = ttxtExchange.fetch_order(id="a18eae908f85U3317077942fPhjnp6nH", symbol=tickerToTest)
             print(f"fetchOrder response: {resp}")
         except Exception as e:
             print("order could not be fetched")
             print(e)
     if "cancelOrder" in params and params["cancelOrder"]:
         print("testing cancel order...")
         try:
-            resp = ttxtExchange.cancel_order(id=698922787, symbol=tickerToTest)
+            resp = ttxtExchange.cancel_order(id="a18eaf2a165cU3317077942BKbakNWlN", symbol=tickerToTest)
             print(f"cancelOrder response: {resp}")
         except Exception as e:
             print("order could not be canceled")
             print(e)
     if "fetchOpenOrders" in params and params["fetchOpenOrders"]:
         print("testing open orders...")
         try:
@@ -195,25 +198,26 @@
             print(resp)
         except Exception as e:
             print("myTrades could not be fetched")
             print(e)
 
 
 if __name__ == "__main__":
-    tickerToTest = "GALA/USDT"
+    tickerToTest = "OPUL/USDT"
     testingParams = {"ticker": False, 
-                     "balance": True, 
+                     "balance": False, 
                      "ohlcv": False, 
                      "createOrder": False, 
                      "fetchOrder": False, 
                      "cancelOrder": False, 
                      "fetchOpenOrders": False, 
                      "setLeverage": False, 
                      "createLimitOrder": False,
                      "createMarketSellOrder": False, 
                      "createMarketBuyOrder": False, 
                      "orderbook": False, 
                      "candlestick": False,
                      "create_market_order": False, 
                      "cancelAllOrders": False, 
-                     "myTrades": False}
-    test(params=testingParams, exchangeName="bybit")
+                     "myTrades": True
+                    }
+    test(params=testingParams, exchangeName="ascendex")
```

### Comparing `ttxt-0.0.5.8/ttxt/types/baseTypes.py` & `ttxt-0.0.5.9/ttxt/types/baseTypes.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.8/ttxt/utils/general.py` & `ttxt-0.0.5.9/ttxt/utils/general.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.8/ttxt/utils/xtUtils.py` & `ttxt-0.0.5.9/ttxt/utils/xtUtils.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.8/ttxt.egg-info/SOURCES.txt` & `ttxt-0.0.5.9/ttxt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 ttxt.egg-info/SOURCES.txt
 ttxt.egg-info/dependency_links.txt
 ttxt.egg-info/top_level.txt
 ttxt/base/__init__.py
 ttxt/base/baseFuturesExchange.py
 ttxt/base/baseSpotExchange.py
 ttxt/exchanges/__init__.py
+ttxt/exchanges/ascendex.py
 ttxt/exchanges/biconomy.py
 ttxt/exchanges/binance.py
 ttxt/exchanges/bingx.py
 ttxt/exchanges/bitget.py
 ttxt/exchanges/bitgetFutures.py
 ttxt/exchanges/bitmart.py
 ttxt/exchanges/bybit.py
```

