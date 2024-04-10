# Comparing `tmp/kucoin_futures_lib-0.3.0.tar.gz` & `tmp/kucoin_futures_lib-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kucoin_futures_lib-0.3.0.tar", max compression
+gzip compressed data, was "kucoin_futures_lib-0.4.0.tar", max compression
```

## Comparing `kucoin_futures_lib-0.3.0.tar` & `kucoin_futures_lib-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/LICENSE
--rw-r--r--   0        0        0       52 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/README.md
--rw-r--r--   0        0        0      719 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/kucoin_futures_lib/__init__.py
--rw-r--r--   0        0        0     2329 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/kucoin_futures_lib/factory.py
--rw-r--r--   0        0        0      251 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/kucoin_futures_lib/handlers/__init__.py
--rw-r--r--   0        0        0      961 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/kucoin_futures_lib/handlers/base.py
--rw-r--r--   0        0        0     1977 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/kucoin_futures_lib/handlers/entry.py
--rw-r--r--   0        0        0     2554 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/kucoin_futures_lib/handlers/oco.py
--rw-r--r--   0        0        0     1775 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/kucoin_futures_lib/helper.py
--rw-r--r--   0        0        0     2464 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/kucoin_futures_lib/kucoinf.py
--rw-r--r--   0        0        0     3117 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/kucoin_futures_lib/market.py
--rw-r--r--   0        0        0    12789 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/kucoin_futures_lib/trade.py
--rw-r--r--   0        0        0     1068 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/kucoin_futures_lib/user.py
--rw-r--r--   0        0        0     3079 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/kucoin_futures_lib/websocket.py
--rw-r--r--   0        0        0      455 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 kucoin_futures_lib-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-10 03:30:34.816202 kucoin_futures_lib-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1760 2024-04-10 03:30:34.816202 kucoin_futures_lib-0.4.0/README.md
+-rw-r--r--   0        0        0      719 2024-04-10 03:30:34.816202 kucoin_futures_lib-0.4.0/kucoin_futures_lib/__init__.py
+-rw-r--r--   0        0        0     2329 2024-04-10 03:30:34.816202 kucoin_futures_lib-0.4.0/kucoin_futures_lib/factory.py
+-rw-r--r--   0        0        0      251 2024-04-10 03:30:34.816202 kucoin_futures_lib-0.4.0/kucoin_futures_lib/handlers/__init__.py
+-rw-r--r--   0        0        0      961 2024-04-10 03:30:34.816202 kucoin_futures_lib-0.4.0/kucoin_futures_lib/handlers/base.py
+-rw-r--r--   0        0        0     1997 2024-04-10 03:30:34.816202 kucoin_futures_lib-0.4.0/kucoin_futures_lib/handlers/entry.py
+-rw-r--r--   0        0        0     2585 2024-04-10 03:30:34.816202 kucoin_futures_lib-0.4.0/kucoin_futures_lib/handlers/oco.py
+-rw-r--r--   0        0        0     1813 2024-04-10 03:30:34.816202 kucoin_futures_lib-0.4.0/kucoin_futures_lib/helper.py
+-rw-r--r--   0        0        0     2464 2024-04-10 03:30:34.816202 kucoin_futures_lib-0.4.0/kucoin_futures_lib/kucoinf.py
+-rw-r--r--   0        0        0     3117 2024-04-10 03:30:34.816202 kucoin_futures_lib-0.4.0/kucoin_futures_lib/market.py
+-rw-r--r--   0        0        0    17231 2024-04-10 03:30:34.816202 kucoin_futures_lib-0.4.0/kucoin_futures_lib/trade.py
+-rw-r--r--   0        0        0     1068 2024-04-10 03:30:34.816202 kucoin_futures_lib-0.4.0/kucoin_futures_lib/user.py
+-rw-r--r--   0        0        0     3133 2024-04-10 03:30:34.816202 kucoin_futures_lib-0.4.0/kucoin_futures_lib/websocket.py
+-rw-r--r--   0        0        0      455 2024-04-10 03:30:34.816202 kucoin_futures_lib-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2389 1970-01-01 00:00:00.000000 kucoin_futures_lib-0.4.0/PKG-INFO
```

### Comparing `kucoin_futures_lib-0.3.0/LICENSE` & `kucoin_futures_lib-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.3.0/kucoin_futures_lib/__init__.py` & `kucoin_futures_lib-0.4.0/kucoin_futures_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.3.0/kucoin_futures_lib/factory.py` & `kucoin_futures_lib-0.4.0/kucoin_futures_lib/factory.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.3.0/kucoin_futures_lib/handlers/base.py` & `kucoin_futures_lib-0.4.0/kucoin_futures_lib/handlers/base.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.3.0/kucoin_futures_lib/handlers/entry.py` & `kucoin_futures_lib-0.4.0/kucoin_futures_lib/handlers/entry.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self.instrument = instrument
         self.entry_low = entry_low
         self.entry_high = entry_high
         self._entered = asyncio.Event()
         self._topic = "/contractMarket/tickerV2"
 
     def __repr__(self):
-        return f"EntryRangeHandler('{self.instrument}', {self.entry_high}, {self.entry_low})"
+        return f"EntryRangeHandler('{self.instrument}', entry_high={self.entry_high}, entry_low={self.entry_low})"
 
     @property
     def done(self) -> asyncio.Event:
         """Return the done status for the handler."""
         return self._entered
 
     @property
@@ -57,8 +57,7 @@
             logger.info(
                 "Instrument %s has reached the entry range: %s <= %s <= %s",
                 self.instrument,
                 self.entry_low,
                 best_bid_price,
                 self.entry_high,
             )
-
```

### Comparing `kucoin_futures_lib-0.3.0/kucoin_futures_lib/handlers/oco.py` & `kucoin_futures_lib-0.4.0/kucoin_futures_lib/handlers/oco.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         self.market_order_id = market_order_id
         self.instrument = instrument
         self._canceled = asyncio.Event()
         self._cancel_order = cancel_order
         self._topic = "/contractMarket/tradeOrders"
 
     def __repr__(self):
-        return f"OcoHandler({self.instrument}, {self.limit_order_id}, {self.market_order_id})"
+        return f"OcoHandler({self.instrument}, limit_order_id={self.limit_order_id}, market_order_id={self.market_order_id})"
 
     @property
     def topic(self) -> str:
         """Return the topic supported by the handler."""
         return f"{self._topic}:{self.instrument}"
 
     @property
```

### Comparing `kucoin_futures_lib-0.3.0/kucoin_futures_lib/helper.py` & `kucoin_futures_lib-0.4.0/kucoin_futures_lib/helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 
 
 class KucoinFuturesHelper:
     """Kucoin Helpers mixin class."""
 
     @staticmethod
     def calculate_lots(
-        lot_size: float, current_price: float, investment_amount: float,
+        lot_size: float,
+        current_price: float,
+        investment_amount: float,
     ) -> int:
         """Calculate the maximum number of lots to buy based on the investment amount, current price, and lot size.
         :param lot_size: The lot size for the instrument. E.g. 0.001 for BTC/USDT.
         :param current_price: The current price of the instrument.
         :param investment_amount: The maximum amount to invest.
         :return: The maximum number of lots to buy.
         """
@@ -31,15 +33,17 @@
             return 0
 
         current_price = Decimal(str(current_price))
         investment_amount = Decimal(str(investment_amount))
         lot_size = Decimal(str(lot_size))
 
         lot_price = current_price * lot_size
-        lots = (investment_amount / lot_price).to_integral_value(rounding='ROUND_FLOOR')  # Use Decimal's floor rounding
+        lots = (investment_amount / lot_price).to_integral_value(
+            rounding="ROUND_FLOOR"
+        )  # Use Decimal's floor rounding
         return int(lots)
 
     @staticmethod
     def calculate_precision(tick_size: float) -> int:
         """Calculate the precision of a tick size.
         :param tick_size: The tick size to calculate the precision of.
         :return: The precision of the tick size.
```

### Comparing `kucoin_futures_lib-0.3.0/kucoin_futures_lib/kucoinf.py` & `kucoin_futures_lib-0.4.0/kucoin_futures_lib/kucoinf.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.3.0/kucoin_futures_lib/market.py` & `kucoin_futures_lib-0.4.0/kucoin_futures_lib/market.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.3.0/kucoin_futures_lib/trade.py` & `kucoin_futures_lib-0.4.0/kucoin_futures_lib/trade.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from collections import namedtuple
 from typing import List, Dict, Any, Optional, Literal
 
 from kucoin_futures.client import Trade
 
 logger = logging.getLogger(__name__)
 
-
 TpSlOrderIds = namedtuple("OrderIds", "tp_order_id sl_order_id")
 
 
 class KucoinFuturesTrade:
     """Kucoin Futures trade wrapper class."""
 
     def __init__(
@@ -22,27 +21,82 @@
         client: Trade = None,
         leverage: int = 2,
     ):
         """Initialize the Kucoin Futures client."""
         self.client = client
         self.leverage = leverage
 
-    def get_open_orders(self, instrument: str = None) -> List[Dict[str, Any]]:  # Unused
-        """https://www.kucoin.com/docs/rest/futures-trading/orders/get-order-list
+    def get_open_limit_orders(
+        self,
+        instrument: str = None,
+        side: Literal["buy", "sell"] = None,
+    ) -> List[Dict[str, Any]]:
+        """Method for getting active limit orders.
+        https://www.kucoin.com/docs/rest/futures-trading/orders/get-order-list
         :param instrument: The instrument symbol
+        :param side: The side of the orders to get (buy or sell)
         :return: A dictionary containing the open orders for the instrument"""
-        logger.debug("Getting open orders")
-        response = self.client.get_order_list()
-        if instrument:
-            open_orders = [
-                order for order in response["items"] if order["symbol"] == instrument
-            ]
-        else:
-            open_orders = response["items"]
-        return open_orders
+
+        params = {
+            "instrument": instrument,
+            "status": "active",
+            "side": side,
+        }
+        params = {k: v for k, v in params.items() if v is not None}
+        logger.debug("Getting orders with params: %s", json.dumps(params))
+        response = self.client.get_order_list(**params)
+        orders = response.get("items", [])
+        return orders
+
+    def get_open_stop_orders(
+        self,
+        instrument: str = None,
+        side: Literal["buy", "sell"] = None,
+        order_type: Literal["limit", "market"] = None,
+    ):
+        """Method for getting untriggered stop orders.
+        https://www.kucoin.com/docs/rest/futures-trading/orders/get-untriggered-stop-order-list
+        :param instrument: The instrument symbol
+        :param side: The side of the orders to get (buy or sell)
+        :param order_type: The type of the orders to get (limit or market)
+        """
+        params = {
+            "instrument": instrument,
+            "side": side,
+            "type": order_type,
+        }
+        params = {k: v for k, v in params.items() if v is not None}
+        logger.debug("Getting orders with params: %s", json.dumps(params))
+        response = self.client.get_open_stop_order(**params)
+        orders = response.get("items", [])
+        return orders
+
+    def get_order_history(
+        self,
+        instrument: str = None,
+        side: Literal["buy", "sell"] = None,
+        order_type: Literal["limit", "market"] = None,
+    ):
+        """Method for getting order history.
+        https://www.kucoin.com/docs/rest/futures-trading/orders/get-order-list
+        :param instrument: The instrument symbol
+        :param side: The side of the orders to get (buy or sell)
+        :param order_type: The type of the orders to get (limit or market)
+        :return: A dictionary containing the open orders for the instrument"""
+        params = {
+            "instrument": instrument,
+            "status": "done",
+            "side": side,
+            "type": order_type,
+        }
+        params = {k: v for k, v in params.items() if v is not None}
+        logger.debug("Getting order history with params: %s", json.dumps(params))
+        response = self.client.get_order_list(**params)
+        orders = response.get("items", [])
+        return orders
 
     def cancel_order(self, order_id: str) -> None:
         """Cancel an order by order id.
         https://www.kucoin.com/docs/rest/futures-trading/orders/cancel-order-by-orderid
         """
         logger.debug("Cancelling order by order id: %s", order_id)
         self.client.cancel_order(orderId=order_id)
@@ -55,51 +109,63 @@
         logger.info("Order %s has been cancelled", order_id)
 
     def create_take_profit_limit(
         self,
         instrument: str,
         entry_side: str,
         tp_price: float,
+        reduce_amount: Optional[int] = None,
     ) -> str:
         """Create a take profit order using limit order.
         https://www.kucoin.com/docs/rest/futures-trading/orders/place-order
         """
+        close_order = False if reduce_amount else True
+        reduce_only = True if reduce_amount else False
+        size = str(reduce_amount) if reduce_amount else None
+
         response = self.client.create_limit_order(
             symbol=instrument,
             side="buy" if entry_side == "sell" else "sell",
             price=str(tp_price),
             timeInForce="GTC",
-            closeOrder=True,
+            closeOrder=close_order,
+            reduceOnly=reduce_only,
             lever=None,
-            size=None,
+            size=size,
         )
         logger.info(
             "Take profit (limit) order created for %s at %s", instrument, tp_price
         )
         return response["orderId"]
 
     def create_take_profit_stop(
         self,
         instrument: str,
         entry_side: str,
         tp_price: float,
+        reduce_amount: Optional[int] = None,
     ) -> str:
         """Create take profit order using stop market order.
         https://www.kucoin.com/docs/rest/futures-trading/orders/place-order
         """
         side, stop = ("sell", "up") if entry_side == "buy" else ("buy", "down")
+        close_order = False if reduce_amount else True
+        reduce_only = True if reduce_amount else False
+        size = str(reduce_amount) if reduce_amount else None
+
         response = self.client.create_market_order(
             symbol=instrument,
             side=side,
             stop=stop,
             stopPriceType="TP",
             stopPrice=str(tp_price),
             timeInForce="GTC",
-            closeOrder=True,
-            size=None,
+            closeOrder=close_order,
+            reduceOnly=reduce_only,
+            size=size,
             lever=None,
         )
         logger.info(
             "Take profit (stop) order created for %s at %s", instrument, tp_price
         )
         return response["orderId"]
 
@@ -157,14 +223,48 @@
             lever=None,
         )
         logger.info(
             "Stop loss order (limit) created for %s at %s", instrument, sl_price
         )
         return response["orderId"]
 
+    async def update_stop_loss_stop_price(self, order_id: str, sl_price: float) -> None:
+        """Update the stop loss order price.
+        https://www.kucoin.com/docs/rest/futures-trading/orders/update-order
+        :param order_id: The order id of the stop loss order
+        :param sl_price: The new stop loss price
+        """
+        orders = self.get_open_stop_orders()
+        order = next((o for o in orders if o["id"] == order_id), None)
+        if not order:
+            raise ValueError(f"Order {order_id} not found.")
+        self.cancel_order(order_id)
+
+        instrument = order["symbol"]
+        side = order["side"]
+        stop = order["stop"]
+        stop_price_type = order["stopPriceType"]
+        time_in_force = order["timeInForce"]
+        close_order = order["closeOrder"]
+        leverage = str(order["leverage"])
+        price = str(sl_price)
+        response = self.client.create_market_order(
+            symbol=instrument,
+            side=side,
+            stop=stop,
+            lever=leverage,
+            stopPriceType=stop_price_type,
+            stopPrice=price,
+            timeInForce=time_in_force,
+            closeOrder=close_order,
+        )
+
+        logger.info("Stop loss (stop) order %s updated to %s", order_id, sl_price)
+        return response["orderId"]
+
     def create_market_order(
         self,
         instrument: str,
         side: str,
         size: int,
         leverage: Optional[int] = None,
     ) -> str:
@@ -228,15 +328,23 @@
         instrument: str,
         side: str,
         take_profit: float,
         stop_loss: float,
         take_profit_type: Literal["limit", "stop"] = "limit",
         stop_loss_type: Literal["limit", "stop"] = "stop",
     ) -> TpSlOrderIds:
-        """Convenience method to create stop loss and take profit orders for an open position."""
+        """Convenience method to create stop loss and take profit orders for an open position.
+        This method will close the position if the stop loss or take profit is hit.
+        :param instrument: The instrument symbol
+        :param side: The side of the order (buy or sell)
+        :param take_profit: The take profit price
+        :param stop_loss: The stop loss price
+        :param take_profit_type: The type of take profit order (limit or stop)
+        :param stop_loss_type: The type of stop loss order (limit or stop)
+        """
 
         if take_profit_type == "stop":
             tp_order_id = self.create_take_profit_stop(
                 instrument=instrument, entry_side=side, tp_price=take_profit
             )
         else:  # take_profit_type == "limit" if take_profit_type is incorrect default to limit
             tp_order_id = self.create_take_profit_limit(
```

### Comparing `kucoin_futures_lib-0.3.0/kucoin_futures_lib/user.py` & `kucoin_futures_lib-0.4.0/kucoin_futures_lib/user.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.3.0/kucoin_futures_lib/websocket.py` & `kucoin_futures_lib-0.4.0/kucoin_futures_lib/websocket.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,16 @@
             else:
                 await handler.done.wait()
         except asyncio.TimeoutError:
             handler.done.set()
             raise asyncio.TimeoutError(f"Timeout reached for {handler}")
         finally:
             logger.info("Unsubscribing from %s", handler.topic)
-            await ws_client.unsubscribe(handler.topic)
+            # noinspection PyAsyncCall
+            asyncio.create_task(ws_client.unsubscribe(handler.topic))
 
     async def listen_for_entry(
         self,
         instrument: str,
         entry_high: float,
         entry_low: float,
         timeout: float = 60 * 60 * 12,
```

