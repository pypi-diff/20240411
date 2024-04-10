# Comparing `tmp/prosperity2bt-0.3.1.tar.gz` & `tmp/prosperity2bt-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosperity2bt-0.3.1.tar", last modified: Tue Apr  9 15:25:25 2024, max compression
+gzip compressed data, was "prosperity2bt-0.4.0.tar", last modified: Wed Apr 10 22:59:20 2024, max compression
```

## Comparing `prosperity2bt-0.3.1.tar` & `prosperity2bt-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:25:25.120809 prosperity2bt-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-09 15:25:17.000000 prosperity2bt-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-09 15:25:25.120809 prosperity2bt-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-09 15:25:17.000000 prosperity2bt-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:25:25.112809 prosperity2bt-0.3.1/prosperity2bt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:25:17.000000 prosperity2bt-0.3.1/prosperity2bt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-04-09 15:25:17.000000 prosperity2bt-0.3.1/prosperity2bt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10041 2024-04-09 15:25:17.000000 prosperity2bt-0.3.1/prosperity2bt/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-09 15:25:17.000000 prosperity2bt-0.3.1/prosperity2bt/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-09 15:25:17.000000 prosperity2bt-0.3.1/prosperity2bt/datamodel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:25:25.116809 prosperity2bt-0.3.1/prosperity2bt/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:25:17.000000 prosperity2bt-0.3.1/prosperity2bt/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:25:25.116809 prosperity2bt-0.3.1/prosperity2bt/resources/round0/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:25:17.000000 prosperity2bt-0.3.1/prosperity2bt/resources/round0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-09 15:25:17.000000 prosperity2bt-0.3.1/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-09 15:25:17.000000 prosperity2bt-0.3.1/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:25:25.120809 prosperity2bt-0.3.1/prosperity2bt/resources/round1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:25:17.000000 prosperity2bt-0.3.1/prosperity2bt/resources/round1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1257340 2024-04-09 15:25:17.000000 prosperity2bt-0.3.1/prosperity2bt/resources/round1/prices_round_1_day_-1.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1258643 2024-04-09 15:25:17.000000 prosperity2bt-0.3.1/prosperity2bt/resources/round1/prices_round_1_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1237383 2024-04-09 15:25:17.000000 prosperity2bt-0.3.1/prosperity2bt/resources/round1/prices_round_1_day_0.csv
--rw-r--r--   0 runner    (1001) docker     (127)   204939 2024-04-09 15:25:17.000000 prosperity2bt-0.3.1/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   208522 2024-04-09 15:25:17.000000 prosperity2bt-0.3.1/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   202884 2024-04-09 15:25:17.000000 prosperity2bt-0.3.1/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:25:25.120809 prosperity2bt-0.3.1/prosperity2bt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-09 15:25:25.000000 prosperity2bt-0.3.1/prosperity2bt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-09 15:25:25.000000 prosperity2bt-0.3.1/prosperity2bt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:25:25.000000 prosperity2bt-0.3.1/prosperity2bt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 15:25:25.000000 prosperity2bt-0.3.1/prosperity2bt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-09 15:25:25.000000 prosperity2bt-0.3.1/prosperity2bt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-09 15:25:25.000000 prosperity2bt-0.3.1/prosperity2bt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-09 15:25:22.000000 prosperity2bt-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:25:25.120809 prosperity2bt-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:59:20.634518 prosperity2bt-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-10 22:59:20.634518 prosperity2bt-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:59:20.626519 prosperity2bt-0.4.0/prosperity2bt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11967 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/datamodel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:59:20.626519 prosperity2bt-0.4.0/prosperity2bt/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:59:20.626519 prosperity2bt-0.4.0/prosperity2bt/resources/round0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/resources/round0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:59:20.634518 prosperity2bt-0.4.0/prosperity2bt/resources/round1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/resources/round1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1257340 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/resources/round1/prices_round_1_day_-1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1258643 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/resources/round1/prices_round_1_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1237383 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/resources/round1/prices_round_1_day_0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   204939 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   208522 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   202884 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:59:20.634518 prosperity2bt-0.4.0/prosperity2bt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-10 22:59:20.000000 prosperity2bt-0.4.0/prosperity2bt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-10 22:59:20.000000 prosperity2bt-0.4.0/prosperity2bt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 22:59:20.000000 prosperity2bt-0.4.0/prosperity2bt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-10 22:59:20.000000 prosperity2bt-0.4.0/prosperity2bt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-10 22:59:20.000000 prosperity2bt-0.4.0/prosperity2bt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 22:59:20.000000 prosperity2bt-0.4.0/prosperity2bt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-10 22:59:18.000000 prosperity2bt-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 22:59:20.634518 prosperity2bt-0.4.0/setup.cfg
```

### Comparing `prosperity2bt-0.3.1/LICENSE` & `prosperity2bt-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.3.1/PKG-INFO` & `prosperity2bt-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.3.1
+Version: 0.4.0
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -93,14 +93,14 @@
 # Print trader's output to stdout while running
 # This may be helpful when debugging a broken trader
 $ prosperity2bt example/starter.py 1 --print
 ```
 
 ## Order Matching
 
-Orders placed by `Trader.run` at a given timestamp are matched against the order depths of that timestamp's state. Market trades are ignored in the matching process. Orders are executed at your best possible price, e.g. if you place a buy order for €10 but there is non-zero ask volume at €9, your order is (possibly partially) filled at €9. Similarly, if you place a sell order for €10 but there is non-zero bid volume at €11, your order is (possibly partially) filled at €11.
+Orders placed by `Trader.run` at a given timestamp are matched against the order depths and market trades of that timestamp's state. Order depths take priority, if an order can be filled completely using volume in the relevant order depth, market trades are not considered. If not, the backtester matches your order against the timestamp's market trades. In this case the backtester assumes that for each trade, the buyer and the seller of the trade are willing to trade with you instead at the trade's price and volume. Your orders are matched at the price of your orders, e.g. if you place a sell order for €9 and there is a market trade for €10, the sell order is matched at €9 (even though there is a buyer willing to pay €10, this appears to be consistent with what the official Prosperity environment does).
 
 Limits are enforced before orders are matched to order depths. If for a product your position would exceed the limit, assuming all your orders would get filled, all your orders for that product get canceled.
 
 ## Development
 
 If you want to make changes to the backtester, clone (or fork and clone) this repository and run `pip install -e .` in the project's root. This installs the project in editable mode, so any changes you make are automatically taken into account the next time you run `prosperity2bt`.
```

### Comparing `prosperity2bt-0.3.1/README.md` & `prosperity2bt-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -51,14 +51,14 @@
 # Print trader's output to stdout while running
 # This may be helpful when debugging a broken trader
 $ prosperity2bt example/starter.py 1 --print
 ```
 
 ## Order Matching
 
-Orders placed by `Trader.run` at a given timestamp are matched against the order depths of that timestamp's state. Market trades are ignored in the matching process. Orders are executed at your best possible price, e.g. if you place a buy order for €10 but there is non-zero ask volume at €9, your order is (possibly partially) filled at €9. Similarly, if you place a sell order for €10 but there is non-zero bid volume at €11, your order is (possibly partially) filled at €11.
+Orders placed by `Trader.run` at a given timestamp are matched against the order depths and market trades of that timestamp's state. Order depths take priority, if an order can be filled completely using volume in the relevant order depth, market trades are not considered. If not, the backtester matches your order against the timestamp's market trades. In this case the backtester assumes that for each trade, the buyer and the seller of the trade are willing to trade with you instead at the trade's price and volume. Your orders are matched at the price of your orders, e.g. if you place a sell order for €9 and there is a market trade for €10, the sell order is matched at €9 (even though there is a buyer willing to pay €10, this appears to be consistent with what the official Prosperity environment does).
 
 Limits are enforced before orders are matched to order depths. If for a product your position would exceed the limit, assuming all your orders would get filled, all your orders for that product get canceled.
 
 ## Development
 
 If you want to make changes to the backtester, clone (or fork and clone) this repository and run `pip install -e .` in the project's root. This installs the project in editable mode, so any changes you make are automatically taken into account the next time you run `prosperity2bt`.
```

### Comparing `prosperity2bt-0.3.1/prosperity2bt/__main__.py` & `prosperity2bt-0.4.0/prosperity2bt/__main__.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.3.1/prosperity2bt/core.py` & `prosperity2bt-0.4.0/prosperity2bt/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,14 +30,20 @@
     round: int
     day: int
 
     sandbox_logs: list[dict[str, Any]]
     activity_logs: list[ActivityLogRow]
     trades: list[Trade]
 
+@dataclass
+class MarketTrade:
+    trade: Trade
+    buy_quantity: int
+    sell_quantity: int
+
 def check_limits(
     tradable_products: list[str],
     orders_by_symbol: dict[Symbol, list[Order]],
     own_positions: dict[str, int],
 ) -> None:
     sandbox_log_lines = []
     for product in tradable_products:
@@ -59,76 +65,113 @@
 
 def process_buy_order(
     timestamp: int,
     order: Order,
     order_depth: OrderDepth,
     own_positions: dict[Symbol, int],
     profit_loss_by_product: dict[Symbol, float],
+    market_trades: list[MarketTrade],
 ) -> list[Trade]:
     new_trades = []
 
-    price_matches = sorted(price for price in order_depth.sell_orders.keys() if price <= order.price)
+    price_matches = sorted((price for price in order_depth.sell_orders.keys() if price <= order.price), reverse=True)
     for price in price_matches:
         volume = min(order.quantity, abs(order_depth.sell_orders[price]))
 
-        new_trades.append(Trade(order.symbol, price, volume, "SUBMISSION", "", timestamp))
+        new_trades.append(Trade(order.symbol, order.price, volume, "SUBMISSION", "", timestamp))
 
         own_positions[order.symbol] += volume
-        profit_loss_by_product[order.symbol] -= price * volume
+        profit_loss_by_product[order.symbol] -= order.price * volume
 
         order_depth.sell_orders[price] += volume
         if order_depth.sell_orders[price] == 0:
             order_depth.sell_orders.pop(price)
 
         order.quantity -= volume
         if order.quantity == 0:
-            break
+            return new_trades
+
+    for trade in market_trades:
+        if trade.sell_quantity == 0 or trade.trade.price > order.price:
+            continue
+
+        volume = min(order.quantity, trade.sell_quantity)
+
+        new_trades.append(Trade(order.symbol, order.price, volume, "SUBMISSION", trade.trade.seller, timestamp))
+
+        own_positions[order.symbol] += volume
+        profit_loss_by_product[order.symbol] -= order.price * volume
+
+        trade.sell_quantity -= volume
+
+        order.quantity -= volume
+        if order.quantity == 0:
+            return new_trades
 
     return new_trades
 
 def process_sell_order(
     timestamp: int,
     order: Order,
     order_depth: OrderDepth,
     own_positions: dict[Symbol, int],
     profit_loss_by_product: dict[Symbol, float],
+    market_trades: list[MarketTrade],
 ) -> list[Trade]:
     new_trades = []
 
-    price_matches = sorted((price for price in order_depth.buy_orders.keys() if price >= order.price), reverse=True)
+    price_matches = sorted(price for price in order_depth.buy_orders.keys() if price >= order.price)
     for price in price_matches:
         volume = min(abs(order.quantity), order_depth.buy_orders[price])
 
-        new_trades.append(Trade(order.symbol, price, volume, "", "SUBMISSION", timestamp))
+        new_trades.append(Trade(order.symbol, order.price, volume, "", "SUBMISSION", timestamp))
 
         own_positions[order.symbol] -= volume
-        profit_loss_by_product[order.symbol] += price * volume
+        profit_loss_by_product[order.symbol] += order.price * volume
 
         order_depth.buy_orders[price] -= volume
         if order_depth.buy_orders[price] == 0:
             order_depth.buy_orders.pop(price)
 
         order.quantity += volume
         if order.quantity == 0:
-            break
+            return new_trades
+
+    for trade in market_trades:
+        if trade.buy_quantity == 0 or trade.trade.price < order.price:
+            continue
+
+        volume = min(abs(order.quantity), trade.buy_quantity)
+
+        new_trades.append(Trade(order.symbol, order.price, volume, trade.trade.buyer, "SUBMISSION", timestamp))
+
+        own_positions[order.symbol] -= volume
+        profit_loss_by_product[order.symbol] += order.price * volume
+
+        trade.buy_quantity -= volume
+
+        order.quantity += volume
+        if order.quantity == 0:
+            return new_trades
 
     return new_trades
 
 def process_order(
     timestamp: int,
     order: Order,
     order_depths: dict[Symbol, OrderDepth],
     own_positions: dict[Symbol, int],
     profit_loss_by_product: dict[Symbol, float],
+    market_trades: list[MarketTrade],
 ) -> list[Trade]:
     order_depth = order_depths[order.symbol]
     if order.quantity > 0:
-        return process_buy_order(timestamp, order, order_depth, own_positions, profit_loss_by_product)
+        return process_buy_order(timestamp, order, order_depth, own_positions, profit_loss_by_product, market_trades)
     elif order.quantity < 0:
-        return process_sell_order(timestamp, order, order_depth, own_positions, profit_loss_by_product)
+        return process_sell_order(timestamp, order, order_depth, own_positions, profit_loss_by_product, market_trades)
     else:
         return []
 
 def trade_to_dict(trade: Trade) -> dict[str, Any]:
     return {
         "timestamp": trade.timestamp,
         "buyer": trade.buyer,
@@ -270,25 +313,39 @@
 
         result.sandbox_logs.append({
             "sandboxLog": sandbox_log,
             "lambdaLog": stdout.getvalue().rstrip(),
             "timestamp": timestamp,
         })
 
+        current_market_trades = {}
+        for product, trades in trades_by_timestamp[timestamp].items():
+            current_market_trades[product] = [MarketTrade(t, t.quantity, t.quantity) for t in trades]
+
         for product in tradable_products:
             new_trades = []
 
             for order in orders_by_symbol.get(product, []):
-                new_trades.extend(process_order(timestamp, order, order_depths, own_positions, profit_loss_by_product))
+                new_trades.extend(process_order(
+                    timestamp,
+                    order,
+                    order_depths,
+                    own_positions,
+                    profit_loss_by_product,
+                    current_market_trades.get(product, []),
+                ))
 
             if len(new_trades) > 0:
                 own_trades[product] = new_trades
 
-        for product, trades in trades_by_timestamp[timestamp].items():
-            market_trades[product] = trades
+        for product, trades in current_market_trades.items():
+            for trade in trades:
+                trade.trade.quantity = min(trade.buy_quantity, trade.sell_quantity)
+
+            market_trades[product] = [t.trade for t in trades if t.trade.quantity > 0]
 
         current_trades = []
         for product in tradable_products:
             current_trades.extend([trade_to_dict(trade) for trade in own_trades[product]])
         for product in tradable_products:
             current_trades.extend([trade_to_dict(trade) for trade in trades_by_timestamp[timestamp][product]])
```

### Comparing `prosperity2bt-0.3.1/prosperity2bt/data.py` & `prosperity2bt-0.4.0/prosperity2bt/data.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.3.1/prosperity2bt/datamodel.py` & `prosperity2bt-0.4.0/prosperity2bt/datamodel.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.3.1/prosperity2bt/resources/round0/prices_round_0_day_-2.csv` & `prosperity2bt-0.4.0/prosperity2bt/resources/round0/prices_round_0_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.3.1/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv` & `prosperity2bt-0.4.0/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.3.1/prosperity2bt/resources/round1/prices_round_1_day_-1.csv` & `prosperity2bt-0.4.0/prosperity2bt/resources/round1/prices_round_1_day_-1.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.3.1/prosperity2bt/resources/round1/prices_round_1_day_-2.csv` & `prosperity2bt-0.4.0/prosperity2bt/resources/round1/prices_round_1_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.3.1/prosperity2bt/resources/round1/prices_round_1_day_0.csv` & `prosperity2bt-0.4.0/prosperity2bt/resources/round1/prices_round_1_day_0.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.3.1/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv` & `prosperity2bt-0.4.0/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.3.1/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv` & `prosperity2bt-0.4.0/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.3.1/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv` & `prosperity2bt-0.4.0/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.3.1/prosperity2bt.egg-info/PKG-INFO` & `prosperity2bt-0.4.0/prosperity2bt.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.3.1
+Version: 0.4.0
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -93,14 +93,14 @@
 # Print trader's output to stdout while running
 # This may be helpful when debugging a broken trader
 $ prosperity2bt example/starter.py 1 --print
 ```
 
 ## Order Matching
 
-Orders placed by `Trader.run` at a given timestamp are matched against the order depths of that timestamp's state. Market trades are ignored in the matching process. Orders are executed at your best possible price, e.g. if you place a buy order for €10 but there is non-zero ask volume at €9, your order is (possibly partially) filled at €9. Similarly, if you place a sell order for €10 but there is non-zero bid volume at €11, your order is (possibly partially) filled at €11.
+Orders placed by `Trader.run` at a given timestamp are matched against the order depths and market trades of that timestamp's state. Order depths take priority, if an order can be filled completely using volume in the relevant order depth, market trades are not considered. If not, the backtester matches your order against the timestamp's market trades. In this case the backtester assumes that for each trade, the buyer and the seller of the trade are willing to trade with you instead at the trade's price and volume. Your orders are matched at the price of your orders, e.g. if you place a sell order for €9 and there is a market trade for €10, the sell order is matched at €9 (even though there is a buyer willing to pay €10, this appears to be consistent with what the official Prosperity environment does).
 
 Limits are enforced before orders are matched to order depths. If for a product your position would exceed the limit, assuming all your orders would get filled, all your orders for that product get canceled.
 
 ## Development
 
 If you want to make changes to the backtester, clone (or fork and clone) this repository and run `pip install -e .` in the project's root. This installs the project in editable mode, so any changes you make are automatically taken into account the next time you run `prosperity2bt`.
```

### Comparing `prosperity2bt-0.3.1/prosperity2bt.egg-info/SOURCES.txt` & `prosperity2bt-0.4.0/prosperity2bt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.3.1/pyproject.toml` & `prosperity2bt-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prosperity2bt"
 description = "Backtester for IMC Prosperity 2 algorithms"
-version = "0.3.1"
+version = "0.4.0"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [{name = "Jasper van Merle", email = "jaspervmerle@gmail.com"}]
 keywords = ["imc", "prosperity", "backtest", "backtester"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

