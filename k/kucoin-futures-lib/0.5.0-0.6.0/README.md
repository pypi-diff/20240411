# Comparing `tmp/kucoin_futures_lib-0.5.0.tar.gz` & `tmp/kucoin_futures_lib-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kucoin_futures_lib-0.5.0.tar", max compression
+gzip compressed data, was "kucoin_futures_lib-0.6.0.tar", max compression
```

## Comparing `kucoin_futures_lib-0.5.0.tar` & `kucoin_futures_lib-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2024-04-10 23:04:04.213113 kucoin_futures_lib-0.5.0/LICENSE
--rw-r--r--   0        0        0     1760 2024-04-10 23:04:04.213113 kucoin_futures_lib-0.5.0/README.md
--rw-r--r--   0        0        0      719 2024-04-10 23:04:04.213113 kucoin_futures_lib-0.5.0/kucoin_futures_lib/__init__.py
--rw-r--r--   0        0        0     2329 2024-04-10 23:04:04.213113 kucoin_futures_lib-0.5.0/kucoin_futures_lib/factory.py
--rw-r--r--   0        0        0      339 2024-04-10 23:04:04.213113 kucoin_futures_lib-0.5.0/kucoin_futures_lib/handlers/__init__.py
--rw-r--r--   0        0        0      961 2024-04-10 23:04:04.213113 kucoin_futures_lib-0.5.0/kucoin_futures_lib/handlers/base.py
--rw-r--r--   0        0        0     2097 2024-04-10 23:04:04.213113 kucoin_futures_lib-0.5.0/kucoin_futures_lib/handlers/entry.py
--rw-r--r--   0        0        0     2769 2024-04-10 23:04:04.213113 kucoin_futures_lib-0.5.0/kucoin_futures_lib/handlers/oco.py
--rw-r--r--   0        0        0     3660 2024-04-10 23:04:04.213113 kucoin_futures_lib-0.5.0/kucoin_futures_lib/handlers/trailing.py
--rw-r--r--   0        0        0     1813 2024-04-10 23:04:04.213113 kucoin_futures_lib-0.5.0/kucoin_futures_lib/helper.py
--rw-r--r--   0        0        0     2464 2024-04-10 23:04:04.213113 kucoin_futures_lib-0.5.0/kucoin_futures_lib/kucoinf.py
--rw-r--r--   0        0        0     3117 2024-04-10 23:04:04.213113 kucoin_futures_lib-0.5.0/kucoin_futures_lib/market.py
--rw-r--r--   0        0        0    17231 2024-04-10 23:04:04.217113 kucoin_futures_lib-0.5.0/kucoin_futures_lib/trade.py
--rw-r--r--   0        0        0     1068 2024-04-10 23:04:04.217113 kucoin_futures_lib-0.5.0/kucoin_futures_lib/user.py
--rw-r--r--   0        0        0     3133 2024-04-10 23:04:04.217113 kucoin_futures_lib-0.5.0/kucoin_futures_lib/websocket.py
--rw-r--r--   0        0        0      455 2024-04-10 23:04:04.217113 kucoin_futures_lib-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2389 1970-01-01 00:00:00.000000 kucoin_futures_lib-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-11 01:54:19.267816 kucoin_futures_lib-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1760 2024-04-11 01:54:19.267816 kucoin_futures_lib-0.6.0/README.md
+-rw-r--r--   0        0        0      719 2024-04-11 01:54:19.267816 kucoin_futures_lib-0.6.0/kucoin_futures_lib/__init__.py
+-rw-r--r--   0        0        0     2329 2024-04-11 01:54:19.267816 kucoin_futures_lib-0.6.0/kucoin_futures_lib/factory.py
+-rw-r--r--   0        0        0      339 2024-04-11 01:54:19.267816 kucoin_futures_lib-0.6.0/kucoin_futures_lib/handlers/__init__.py
+-rw-r--r--   0        0        0      961 2024-04-11 01:54:19.267816 kucoin_futures_lib-0.6.0/kucoin_futures_lib/handlers/base.py
+-rw-r--r--   0        0        0     2695 2024-04-11 01:54:19.267816 kucoin_futures_lib-0.6.0/kucoin_futures_lib/handlers/entry.py
+-rw-r--r--   0        0        0     2769 2024-04-11 01:54:19.267816 kucoin_futures_lib-0.6.0/kucoin_futures_lib/handlers/oco.py
+-rw-r--r--   0        0        0     3660 2024-04-11 01:54:19.267816 kucoin_futures_lib-0.6.0/kucoin_futures_lib/handlers/trailing.py
+-rw-r--r--   0        0        0     1813 2024-04-11 01:54:19.267816 kucoin_futures_lib-0.6.0/kucoin_futures_lib/helper.py
+-rw-r--r--   0        0        0     2464 2024-04-11 01:54:19.267816 kucoin_futures_lib-0.6.0/kucoin_futures_lib/kucoinf.py
+-rw-r--r--   0        0        0     3117 2024-04-11 01:54:19.267816 kucoin_futures_lib-0.6.0/kucoin_futures_lib/market.py
+-rw-r--r--   0        0        0    17231 2024-04-11 01:54:19.267816 kucoin_futures_lib-0.6.0/kucoin_futures_lib/trade.py
+-rw-r--r--   0        0        0     1068 2024-04-11 01:54:19.267816 kucoin_futures_lib-0.6.0/kucoin_futures_lib/user.py
+-rw-r--r--   0        0        0     3133 2024-04-11 01:54:19.267816 kucoin_futures_lib-0.6.0/kucoin_futures_lib/websocket.py
+-rw-r--r--   0        0        0      598 2024-04-11 01:54:19.267816 kucoin_futures_lib-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2389 1970-01-01 00:00:00.000000 kucoin_futures_lib-0.6.0/PKG-INFO
```

### Comparing `kucoin_futures_lib-0.5.0/LICENSE` & `kucoin_futures_lib-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.5.0/README.md` & `kucoin_futures_lib-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.5.0/kucoin_futures_lib/__init__.py` & `kucoin_futures_lib-0.6.0/kucoin_futures_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.5.0/kucoin_futures_lib/factory.py` & `kucoin_futures_lib-0.6.0/kucoin_futures_lib/factory.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.5.0/kucoin_futures_lib/handlers/base.py` & `kucoin_futures_lib-0.6.0/kucoin_futures_lib/handlers/base.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.5.0/kucoin_futures_lib/handlers/entry.py` & `kucoin_futures_lib-0.6.0/kucoin_futures_lib/handlers/entry.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 """ This is an entry range handler that waits for the instrument to reach a certain price range."""
 import asyncio
 import logging
+from typing import Union, Callable, Awaitable, Optional, Any
+from unittest.mock import AsyncMock
 
 from kucoin_futures_lib.handlers.base import HandlerABC
 
 logger = logging.getLogger(__name__)
 
 
 class EntryRangeHandler(HandlerABC):
     """Handler that waits for the instrument to reach a certain price range"""
 
     def __init__(
         self,
         instrument: str,
         entry_high: float,
         entry_low: float,
+        callback: Optional[
+            Union[Callable[..., Any], Callable[..., Awaitable[Any]]]
+        ] = None,
     ):
         assert entry_high > entry_low, "Entry high must be greater than entry low"
         self.instrument = instrument
         self.entry_low = entry_low
         self.entry_high = entry_high
+        self._callback = callback
         self._entered = asyncio.Event()
         self._topic = "/contractMarket/tickerV2"
 
     def __repr__(self):
         return f"EntryRangeHandler('{self.instrument}', entry_high={self.entry_high}, entry_low={self.entry_low})"
 
     @property
@@ -37,27 +43,37 @@
         return f"{self._topic}:{self.instrument}"
 
     @property
     def private(self) -> bool:
         """Return the privacy status for the topic."""
         return False
 
+    async def call(self):
+        """Call the callback function."""
+        if self._callback:
+            if asyncio.iscoroutinefunction(self._callback) or isinstance(self._callback, AsyncMock):
+                await self._callback()
+            else:
+                self._callback()
+
     async def handle(self, msg):
         """Handle the trade order message from
         :param msg: The trade order message.
         https://www.kucoin.com/docs/websocket/futures-trading/public-channels/get-ticker-v2
         """
 
         if self._entered.is_set():
             return
 
         ticker = msg.get("data", {})
         best_bid_price = float(ticker.get("bestBidPrice", 0))
         best_ask_price = float(ticker.get("bestAskPrice", 0))
         if best_bid_price >= self.entry_low and best_ask_price <= self.entry_high:
+            if self._callback:
+                await self.call()
             self._entered.set()
             logger.info(
                 "Instrument %s has reached the entry range: %s <= %s <= %s",
                 self.instrument,
                 self.entry_low,
                 best_bid_price,
                 self.entry_high,
```

### Comparing `kucoin_futures_lib-0.5.0/kucoin_futures_lib/handlers/oco.py` & `kucoin_futures_lib-0.6.0/kucoin_futures_lib/handlers/oco.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.5.0/kucoin_futures_lib/handlers/trailing.py` & `kucoin_futures_lib-0.6.0/kucoin_futures_lib/handlers/trailing.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.5.0/kucoin_futures_lib/helper.py` & `kucoin_futures_lib-0.6.0/kucoin_futures_lib/helper.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.5.0/kucoin_futures_lib/kucoinf.py` & `kucoin_futures_lib-0.6.0/kucoin_futures_lib/kucoinf.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.5.0/kucoin_futures_lib/market.py` & `kucoin_futures_lib-0.6.0/kucoin_futures_lib/market.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.5.0/kucoin_futures_lib/trade.py` & `kucoin_futures_lib-0.6.0/kucoin_futures_lib/trade.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.5.0/kucoin_futures_lib/user.py` & `kucoin_futures_lib-0.6.0/kucoin_futures_lib/user.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.5.0/kucoin_futures_lib/websocket.py` & `kucoin_futures_lib-0.6.0/kucoin_futures_lib/websocket.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.5.0/PKG-INFO` & `kucoin_futures_lib-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kucoin-futures-lib
-Version: 0.5.0
+Version: 0.6.0
 Summary: Kucoin Futures wrapper library
 License: Apache-2.0
 Author: Evgeny Aleshin
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

