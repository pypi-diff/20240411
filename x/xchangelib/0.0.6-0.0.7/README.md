# Comparing `tmp/xchangelib-0.0.6.tar.gz` & `tmp/xchangelib-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xchangelib-0.0.6.tar", last modified: Wed Apr 10 08:03:44 2024, max compression
+gzip compressed data, was "xchangelib-0.0.7.tar", last modified: Thu Apr 11 08:41:50 2024, max compression
```

## Comparing `xchangelib-0.0.6.tar` & `xchangelib-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-10 08:03:44.265513 xchangelib-0.0.6/
--rw-r--r--   0 rohanv     (501) staff       (20)     1070 2024-04-10 08:02:54.000000 xchangelib-0.0.6/LICENSE
--rw-r--r--   0 rohanv     (501) staff       (20)      716 2024-04-10 08:03:44.264645 xchangelib-0.0.6/PKG-INFO
--rw-r--r--   0 rohanv     (501) staff       (20)      140 2024-04-10 08:02:54.000000 xchangelib-0.0.6/README.md
--rw-r--r--   0 rohanv     (501) staff       (20)      650 2024-04-10 08:02:54.000000 xchangelib-0.0.6/pyproject.toml
--rw-r--r--   0 rohanv     (501) staff       (20)       38 2024-04-10 08:03:44.265750 xchangelib-0.0.6/setup.cfg
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-10 08:03:44.248309 xchangelib-0.0.6/src/
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-10 08:03:44.256552 xchangelib-0.0.6/src/xchangelib/
--rw-r--r--   0 rohanv     (501) staff       (20)        0 2024-04-10 08:02:54.000000 xchangelib-0.0.6/src/xchangelib/__init__.py
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-10 08:03:44.248969 xchangelib-0.0.6/src/xchangelib/docs/
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-10 08:03:44.261261 xchangelib-0.0.6/src/xchangelib/docs/source/
--rw-r--r--   0 rohanv     (501) staff       (20)     2246 2024-04-10 08:02:54.000000 xchangelib-0.0.6/src/xchangelib/docs/source/conf.py
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-10 08:03:44.262379 xchangelib-0.0.6/src/xchangelib/examples/
--rw-r--r--   0 rohanv     (501) staff       (20)     3414 2024-04-10 08:02:54.000000 xchangelib-0.0.6/src/xchangelib/examples/example_bot.py
--rw-r--r--   0 rohanv     (501) staff       (20)    12187 2024-04-10 08:02:54.000000 xchangelib-0.0.6/src/xchangelib/service_pb2.py
--rw-r--r--   0 rohanv     (501) staff       (20)     8437 2024-04-10 08:02:54.000000 xchangelib-0.0.6/src/xchangelib/service_pb2_grpc.py
--rw-r--r--   0 rohanv     (501) staff       (20)      398 2024-04-10 08:02:54.000000 xchangelib-0.0.6/src/xchangelib/setup.py
--rw-r--r--   0 rohanv     (501) staff       (20)    14296 2024-04-10 08:02:54.000000 xchangelib-0.0.6/src/xchangelib/xchange_client.py
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-10 08:03:44.263584 xchangelib-0.0.6/src/xchangelib.egg-info/
--rw-r--r--   0 rohanv     (501) staff       (20)      716 2024-04-10 08:03:44.000000 xchangelib-0.0.6/src/xchangelib.egg-info/PKG-INFO
--rw-r--r--   0 rohanv     (501) staff       (20)      444 2024-04-10 08:03:44.000000 xchangelib-0.0.6/src/xchangelib.egg-info/SOURCES.txt
--rw-r--r--   0 rohanv     (501) staff       (20)        1 2024-04-10 08:03:44.000000 xchangelib-0.0.6/src/xchangelib.egg-info/dependency_links.txt
--rw-r--r--   0 rohanv     (501) staff       (20)       49 2024-04-10 08:03:44.000000 xchangelib-0.0.6/src/xchangelib.egg-info/requires.txt
--rw-r--r--   0 rohanv     (501) staff       (20)       11 2024-04-10 08:03:44.000000 xchangelib-0.0.6/src/xchangelib.egg-info/top_level.txt
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-11 08:41:50.234673 xchangelib-0.0.7/
+-rw-r--r--   0 rohanv     (501) staff       (20)     1070 2024-04-11 08:41:35.000000 xchangelib-0.0.7/LICENSE
+-rw-r--r--   0 rohanv     (501) staff       (20)      716 2024-04-11 08:41:50.233536 xchangelib-0.0.7/PKG-INFO
+-rw-r--r--   0 rohanv     (501) staff       (20)      140 2024-04-11 08:41:35.000000 xchangelib-0.0.7/README.md
+-rw-r--r--   0 rohanv     (501) staff       (20)      650 2024-04-11 08:41:35.000000 xchangelib-0.0.7/pyproject.toml
+-rw-r--r--   0 rohanv     (501) staff       (20)       38 2024-04-11 08:41:50.234868 xchangelib-0.0.7/setup.cfg
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-11 08:41:50.224705 xchangelib-0.0.7/src/
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-11 08:41:50.229849 xchangelib-0.0.7/src/xchangelib/
+-rw-r--r--   0 rohanv     (501) staff       (20)        0 2024-04-11 08:41:35.000000 xchangelib-0.0.7/src/xchangelib/__init__.py
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-11 08:41:50.225042 xchangelib-0.0.7/src/xchangelib/docs/
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-11 08:41:50.231921 xchangelib-0.0.7/src/xchangelib/docs/source/
+-rw-r--r--   0 rohanv     (501) staff       (20)     2246 2024-04-11 08:41:35.000000 xchangelib-0.0.7/src/xchangelib/docs/source/conf.py
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-11 08:41:50.232424 xchangelib-0.0.7/src/xchangelib/examples/
+-rw-r--r--   0 rohanv     (501) staff       (20)     3683 2024-04-11 08:41:35.000000 xchangelib-0.0.7/src/xchangelib/examples/example_bot.py
+-rw-r--r--   0 rohanv     (501) staff       (20)    12187 2024-04-11 08:41:35.000000 xchangelib-0.0.7/src/xchangelib/service_pb2.py
+-rw-r--r--   0 rohanv     (501) staff       (20)     8437 2024-04-11 08:41:35.000000 xchangelib-0.0.7/src/xchangelib/service_pb2_grpc.py
+-rw-r--r--   0 rohanv     (501) staff       (20)      398 2024-04-11 08:41:35.000000 xchangelib-0.0.7/src/xchangelib/setup.py
+-rw-r--r--   0 rohanv     (501) staff       (20)    15346 2024-04-11 08:41:35.000000 xchangelib-0.0.7/src/xchangelib/xchange_client.py
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-11 08:41:50.232982 xchangelib-0.0.7/src/xchangelib.egg-info/
+-rw-r--r--   0 rohanv     (501) staff       (20)      716 2024-04-11 08:41:50.000000 xchangelib-0.0.7/src/xchangelib.egg-info/PKG-INFO
+-rw-r--r--   0 rohanv     (501) staff       (20)      444 2024-04-11 08:41:50.000000 xchangelib-0.0.7/src/xchangelib.egg-info/SOURCES.txt
+-rw-r--r--   0 rohanv     (501) staff       (20)        1 2024-04-11 08:41:50.000000 xchangelib-0.0.7/src/xchangelib.egg-info/dependency_links.txt
+-rw-r--r--   0 rohanv     (501) staff       (20)       49 2024-04-11 08:41:50.000000 xchangelib-0.0.7/src/xchangelib.egg-info/requires.txt
+-rw-r--r--   0 rohanv     (501) staff       (20)       11 2024-04-11 08:41:50.000000 xchangelib-0.0.7/src/xchangelib.egg-info/top_level.txt
```

### Comparing `xchangelib-0.0.6/LICENSE` & `xchangelib-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xchangelib-0.0.6/PKG-INFO` & `xchangelib-0.0.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchangelib
-Version: 0.0.6
+Version: 0.0.7
 Summary: A client library for interacting with xchange-v3
 Author-email: Rohan Voddhi <rohan.voddhi@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/UChicagoFM/xchangelib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xchangelib-0.0.6/pyproject.toml` & `xchangelib-0.0.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xchangelib"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     { name="Rohan Voddhi", email="rohan.voddhi@gmail.com" },
 ]
 description = "A client library for interacting with xchange-v3"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = ['setuptools>=69.0','protobuf==5.26.0', 'grpcio==1.62.1']
```

### Comparing `xchangelib-0.0.6/src/xchangelib/docs/source/conf.py` & `xchangelib-0.0.7/src/xchangelib/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `xchangelib-0.0.6/src/xchangelib/examples/example_bot.py` & `xchangelib-0.0.7/src/xchangelib/examples/example_bot.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 class MyXchangeClient(xchange_client.XChangeClient):
     '''A shell client with the methods that can be implemented to interact with the xchange.'''
 
     def __init__(self, host: str, username: str, password: str):
         super().__init__(host, username, password)
 
     async def bot_handle_cancel_response(self, order_id: str, success: bool, error: Optional[str]) -> None:
-        order = self.open_orders[order_id]
-        print(f"{'Market' if order[2] else 'Limit'} Order ID {order_id} cancelled, {order[1]} unfilled")
+        if success:
+            order = self.open_orders[order_id]
+            print(f"{'Market' if order[2] else 'Limit'} Order ID {order_id} cancelled, {order[1]} unfilled")
 
     async def bot_handle_order_fill(self, order_id: str, qty: int, price: int):
         print("order fill", self.positions)
 
     async def bot_handle_order_rejected(self, order_id: str, reason: str) -> None:
         print("order rejected because of ", reason)
 
@@ -32,15 +33,14 @@
     async def bot_handle_swap_response(self, swap: str, qty: int, success: bool):
         # print("Swap response")
         pass
 
 
     async def trade(self):
         """This is a task that is started right before the bot connects and runs in the background."""
-        await asyncio.sleep(5)
         print("attempting to trade")
         await self.place_order("BRV",3, xchange_client.Side.SELL, 7)
 
         # Cancelling an order
         order_to_cancel = await self.place_order("BRV",3, xchange_client.Side.BUY, 5)
         await asyncio.sleep(5)
         await self.cancel_order(order_to_cancel)
@@ -69,20 +69,28 @@
             await asyncio.sleep(3)
             for security, book in self.order_books.items():
                 sorted_bids = sorted((k,v) for k,v in book.bids.items() if v != 0)
                 sorted_asks = sorted((k,v) for k,v in book.asks.items() if v != 0)
                 print(f"Bids for {security}:\n{sorted_bids}")
                 print(f"Asks for {security}:\n{sorted_asks}")
 
+    async def view_pnl_estimates(self):
+        """Prints an estimate of the PnL every 3 seconds."""
+        while True:
+            await asyncio.sleep(5)
+            print("My PnL Estimate:", self.estimate_pnl())
+
+
     async def start(self):
         """
         Creates tasks that can be run in the background. Then connects to the exchange
         and listens for messages.
         """
         asyncio.create_task(self.trade())
+        asyncio.create_task(self.view_pnl_estimates())
         # asyncio.create_task(self.view_books())
         await self.connect()
 
 
 async def main():
     SERVER = '18.188.190.235:3333' # run on sandbox
     my_client = MyXchangeClient(SERVER,"USERNAME","PASSWORD")
```

### Comparing `xchangelib-0.0.6/src/xchangelib/service_pb2.py` & `xchangelib-0.0.7/src/xchangelib/service_pb2.py`

 * *Files identical despite different names*

### Comparing `xchangelib-0.0.6/src/xchangelib/service_pb2_grpc.py` & `xchangelib-0.0.7/src/xchangelib/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xchangelib-0.0.6/src/xchangelib/xchange_client.py` & `xchangelib-0.0.7/src/xchangelib/xchange_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import grpc
+import asyncio
 from grpc import aio
 from . import service_pb2 as utc_bot_pb2
 from . import service_pb2_grpc as utc_bot_pb2_grpc
 from enum import Enum
 import logging
 from dataclasses import dataclass, field
 from collections import defaultdict
 from typing import Optional
 import time
 
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 
 logging.basicConfig(level=logging.INFO)
 _LOGGER = logging.getLogger("xchange-client")
 _LOGGER.setLevel(logging.INFO)
 
 
 @dataclass
@@ -64,14 +65,15 @@
         self.positions = defaultdict(int)
         self.open_orders = dict()
         self.order_books = {sym: OrderBook() for sym in SYMBOLS}
         self.order_id = int(time.time() * 1e9)  # start order id number from time
         self.history = []
         self.connected = False
         self.call = None
+        self.request_lock = asyncio.Lock()
         if silent:
             _LOGGER.setLevel(logging.WARNING)
 
 
     async def connect(self) -> None:
         """
         Connects to the server using the username and password from initialization. Main loop of the bot that
@@ -81,15 +83,16 @@
         _LOGGER.info("Connecting to host %s as %s", self.host, self.username)
         channel = aio.insecure_channel(self.host)
         stub = utc_bot_pb2_grpc.ClientStub(channel)
         self.call = stub.Start()
 
         auth_request = utc_bot_pb2.AuthenticateRequest(username=self.username, password=self.password)
         request = utc_bot_pb2.ClientMessageToExchange(authenticate=auth_request)
-        await self.call.write(request)
+        async with self.request_lock:
+            await self.call.write(request)
 
         while True:
             response = await self.call.read()
             await self.process_message(response)
 
         await channel.close()
 
@@ -112,38 +115,40 @@
         else:
             limit_order_msg = utc_bot_pb2.LimitOrder(qty=qty, px=px)
             order_request = utc_bot_pb2.NewOrderRequest(symbol=symbol, id=str(self.order_id), limit=limit_order_msg,
                                                         side=side)
         request = utc_bot_pb2.ClientMessageToExchange(new_order=order_request)
         key = str(self.order_id)
         self.order_id += 1
-        await self.call.write(request)
+        async with self.request_lock:
+            await self.call.write(request)
         self.open_orders[key] = [order_request, qty, is_market]
         return key
     async def place_swap_order(self, swap: str, qty: int) -> None:
         """
         Places a swap request with the exchange.
         :param swap: Name of the swap
         :param qty: Quantity of swaps to execute
         :return:
         """
         swap_request = utc_bot_pb2.SwapRequest(name=swap, qty=qty)
         request = utc_bot_pb2.ClientMessageToExchange(swap=swap_request)
-        await self.call.write(request)
+        async with self.request_lock:
+            await self.call.write(request)
 
     async def cancel_order(self, order_id: str) -> None:
         """ Places a cancel order request for the given order id
         :param order_id: order_id of the order to cancel
         :return:
         """
         _LOGGER.info("Requesting to cancel order: %s", order_id)
         cancel_request = utc_bot_pb2.CancelOrderRequest(id=order_id)
         request = utc_bot_pb2.ClientMessageToExchange(cancel_order=cancel_request)
-        await self.call.write(request)
-
+        async with self.request_lock:
+            await self.call.write(request)
     async def handle_trade_msg(self, msg):
         """Calls the bot trade message handler."""
         await self.bot_handle_trade_msg(msg.symbol, msg.px, msg.qty)
 
     async def handle_order_fill(self, msg) -> None:
         """
         Updates the positions based on the order fill. Then calls the bot specific code.
@@ -240,14 +245,36 @@
         """Copy over positions from the exchange records"""
         positions = {position.symbol: position.position for position in msg.positions}
         positions['cash'] = msg.cash
         self.positions = defaultdict(int, positions)
         _LOGGER.info("Received Positions from server")
         _LOGGER.info(self.positions)
 
+    def estimate_pnl(self):
+        """Calculates a pnl estimate using mid market prices"""
+        pnl = 0
+        if len(self.positions) == 0:
+            return pnl
+        for symbol, qty in self.positions.items():
+            if qty == 0:
+                continue
+            if symbol == 'cash':
+                pnl += qty
+            elif symbol in self.order_books:
+                book = self.order_books[symbol]
+                bids = [px  for px,qty in book.bids.items() if qty != 0]
+                asks = [px  for px,qty in book.asks.items() if qty != 0]
+                if len(bids) == 0 or len(asks) == 0:
+                    continue
+                best_bid = max(bids)
+                best_ask = min(asks)
+                mid = (best_bid + best_ask) / 2
+                pnl += mid * qty
+        return pnl
+
     async def bot_handle_book_update(self, symbol: str) -> None:
         """
         Function for the user to fill in if they want to have any action upon receiving
         book updates.
         # TODO: Fill in subclassed bot.
         :return:
         """
```

### Comparing `xchangelib-0.0.6/src/xchangelib.egg-info/PKG-INFO` & `xchangelib-0.0.7/src/xchangelib.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchangelib
-Version: 0.0.6
+Version: 0.0.7
 Summary: A client library for interacting with xchange-v3
 Author-email: Rohan Voddhi <rohan.voddhi@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/UChicagoFM/xchangelib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

