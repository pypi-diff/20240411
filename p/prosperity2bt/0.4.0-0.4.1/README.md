# Comparing `tmp/prosperity2bt-0.4.0.tar.gz` & `tmp/prosperity2bt-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosperity2bt-0.4.0.tar", last modified: Wed Apr 10 22:59:20 2024, max compression
+gzip compressed data, was "prosperity2bt-0.4.1.tar", last modified: Wed Apr 10 23:12:02 2024, max compression
```

## Comparing `prosperity2bt-0.4.0.tar` & `prosperity2bt-0.4.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:59:20.634518 prosperity2bt-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-10 22:59:20.634518 prosperity2bt-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:59:20.626519 prosperity2bt-0.4.0/prosperity2bt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11967 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/datamodel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:59:20.626519 prosperity2bt-0.4.0/prosperity2bt/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:59:20.626519 prosperity2bt-0.4.0/prosperity2bt/resources/round0/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/resources/round0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:59:20.634518 prosperity2bt-0.4.0/prosperity2bt/resources/round1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/resources/round1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1257340 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/resources/round1/prices_round_1_day_-1.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1258643 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/resources/round1/prices_round_1_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1237383 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/resources/round1/prices_round_1_day_0.csv
--rw-r--r--   0 runner    (1001) docker     (127)   204939 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   208522 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   202884 2024-04-10 22:59:13.000000 prosperity2bt-0.4.0/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:59:20.634518 prosperity2bt-0.4.0/prosperity2bt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-10 22:59:20.000000 prosperity2bt-0.4.0/prosperity2bt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-10 22:59:20.000000 prosperity2bt-0.4.0/prosperity2bt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 22:59:20.000000 prosperity2bt-0.4.0/prosperity2bt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-10 22:59:20.000000 prosperity2bt-0.4.0/prosperity2bt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-10 22:59:20.000000 prosperity2bt-0.4.0/prosperity2bt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 22:59:20.000000 prosperity2bt-0.4.0/prosperity2bt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-10 22:59:18.000000 prosperity2bt-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 22:59:20.634518 prosperity2bt-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:12:02.305780 prosperity2bt-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-04-10 23:12:02.305780 prosperity2bt-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:12:02.297780 prosperity2bt-0.4.1/prosperity2bt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11943 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/datamodel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:12:02.297780 prosperity2bt-0.4.1/prosperity2bt/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:12:02.301780 prosperity2bt-0.4.1/prosperity2bt/resources/round0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/resources/round0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:12:02.305780 prosperity2bt-0.4.1/prosperity2bt/resources/round1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/resources/round1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1257340 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/resources/round1/prices_round_1_day_-1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1258643 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/resources/round1/prices_round_1_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1237383 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/resources/round1/prices_round_1_day_0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   204939 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   208522 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   202884 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:12:02.305780 prosperity2bt-0.4.1/prosperity2bt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-04-10 23:12:02.000000 prosperity2bt-0.4.1/prosperity2bt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-10 23:12:02.000000 prosperity2bt-0.4.1/prosperity2bt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:12:02.000000 prosperity2bt-0.4.1/prosperity2bt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-10 23:12:02.000000 prosperity2bt-0.4.1/prosperity2bt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-10 23:12:02.000000 prosperity2bt-0.4.1/prosperity2bt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 23:12:02.000000 prosperity2bt-0.4.1/prosperity2bt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-10 23:12:00.000000 prosperity2bt-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 23:12:02.305780 prosperity2bt-0.4.1/setup.cfg
```

### Comparing `prosperity2bt-0.4.0/LICENSE` & `prosperity2bt-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.0/PKG-INFO` & `prosperity2bt-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.4.0
+Version: 0.4.1
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
 
-Orders placed by `Trader.run` at a given timestamp are matched against the order depths and market trades of that timestamp's state. Order depths take priority, if an order can be filled completely using volume in the relevant order depth, market trades are not considered. If not, the backtester matches your order against the timestamp's market trades. In this case the backtester assumes that for each trade, the buyer and the seller of the trade are willing to trade with you instead at the trade's price and volume. Your orders are matched at the price of your orders, e.g. if you place a sell order for €9 and there is a market trade for €10, the sell order is matched at €9 (even though there is a buyer willing to pay €10, this appears to be consistent with what the official Prosperity environment does).
+Orders placed by `Trader.run` at a given timestamp are matched against the order depths and market trades of that timestamp's state. Order depths take priority, if an order can be filled completely using volume in the relevant order depth, market trades are not considered. If not, the backtester matches your order against the timestamp's market trades. In this case the backtester assumes that for each trade, the buyer and the seller of the trade are willing to trade with you instead at the trade's price and volume. Market trades are matched at the price of your orders, e.g. if you place a sell order for €9 and there is a market trade for €10, the sell order is matched at €9 (even though there is a buyer willing to pay €10, this appears to be consistent with what the official Prosperity environment does).
 
 Limits are enforced before orders are matched to order depths. If for a product your position would exceed the limit, assuming all your orders would get filled, all your orders for that product get canceled.
 
 ## Development
 
 If you want to make changes to the backtester, clone (or fork and clone) this repository and run `pip install -e .` in the project's root. This installs the project in editable mode, so any changes you make are automatically taken into account the next time you run `prosperity2bt`.
```

### Comparing `prosperity2bt-0.4.0/README.md` & `prosperity2bt-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,14 @@
 # Print trader's output to stdout while running
 # This may be helpful when debugging a broken trader
 $ prosperity2bt example/starter.py 1 --print
 ```
 
 ## Order Matching
 
-Orders placed by `Trader.run` at a given timestamp are matched against the order depths and market trades of that timestamp's state. Order depths take priority, if an order can be filled completely using volume in the relevant order depth, market trades are not considered. If not, the backtester matches your order against the timestamp's market trades. In this case the backtester assumes that for each trade, the buyer and the seller of the trade are willing to trade with you instead at the trade's price and volume. Your orders are matched at the price of your orders, e.g. if you place a sell order for €9 and there is a market trade for €10, the sell order is matched at €9 (even though there is a buyer willing to pay €10, this appears to be consistent with what the official Prosperity environment does).
+Orders placed by `Trader.run` at a given timestamp are matched against the order depths and market trades of that timestamp's state. Order depths take priority, if an order can be filled completely using volume in the relevant order depth, market trades are not considered. If not, the backtester matches your order against the timestamp's market trades. In this case the backtester assumes that for each trade, the buyer and the seller of the trade are willing to trade with you instead at the trade's price and volume. Market trades are matched at the price of your orders, e.g. if you place a sell order for €9 and there is a market trade for €10, the sell order is matched at €9 (even though there is a buyer willing to pay €10, this appears to be consistent with what the official Prosperity environment does).
 
 Limits are enforced before orders are matched to order depths. If for a product your position would exceed the limit, assuming all your orders would get filled, all your orders for that product get canceled.
 
 ## Development
 
 If you want to make changes to the backtester, clone (or fork and clone) this repository and run `pip install -e .` in the project's root. This installs the project in editable mode, so any changes you make are automatically taken into account the next time you run `prosperity2bt`.
```

### Comparing `prosperity2bt-0.4.0/prosperity2bt/__main__.py` & `prosperity2bt-0.4.1/prosperity2bt/__main__.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.0/prosperity2bt/core.py` & `prosperity2bt-0.4.1/prosperity2bt/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,22 +69,22 @@
     order_depth: OrderDepth,
     own_positions: dict[Symbol, int],
     profit_loss_by_product: dict[Symbol, float],
     market_trades: list[MarketTrade],
 ) -> list[Trade]:
     new_trades = []
 
-    price_matches = sorted((price for price in order_depth.sell_orders.keys() if price <= order.price), reverse=True)
+    price_matches = sorted(price for price in order_depth.sell_orders.keys() if price <= order.price)
     for price in price_matches:
         volume = min(order.quantity, abs(order_depth.sell_orders[price]))
 
-        new_trades.append(Trade(order.symbol, order.price, volume, "SUBMISSION", "", timestamp))
+        new_trades.append(Trade(order.symbol, price, volume, "SUBMISSION", "", timestamp))
 
         own_positions[order.symbol] += volume
-        profit_loss_by_product[order.symbol] -= order.price * volume
+        profit_loss_by_product[order.symbol] -= price * volume
 
         order_depth.sell_orders[price] += volume
         if order_depth.sell_orders[price] == 0:
             order_depth.sell_orders.pop(price)
 
         order.quantity -= volume
         if order.quantity == 0:
@@ -115,22 +115,22 @@
     order_depth: OrderDepth,
     own_positions: dict[Symbol, int],
     profit_loss_by_product: dict[Symbol, float],
     market_trades: list[MarketTrade],
 ) -> list[Trade]:
     new_trades = []
 
-    price_matches = sorted(price for price in order_depth.buy_orders.keys() if price >= order.price)
+    price_matches = sorted((price for price in order_depth.buy_orders.keys() if price >= order.price), reverse=True)
     for price in price_matches:
         volume = min(abs(order.quantity), order_depth.buy_orders[price])
 
-        new_trades.append(Trade(order.symbol, order.price, volume, "", "SUBMISSION", timestamp))
+        new_trades.append(Trade(order.symbol, price, volume, "", "SUBMISSION", timestamp))
 
         own_positions[order.symbol] -= volume
-        profit_loss_by_product[order.symbol] += order.price * volume
+        profit_loss_by_product[order.symbol] += price * volume
 
         order_depth.buy_orders[price] -= volume
         if order_depth.buy_orders[price] == 0:
             order_depth.buy_orders.pop(price)
 
         order.quantity += volume
         if order.quantity == 0:
```

### Comparing `prosperity2bt-0.4.0/prosperity2bt/data.py` & `prosperity2bt-0.4.1/prosperity2bt/data.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.0/prosperity2bt/datamodel.py` & `prosperity2bt-0.4.1/prosperity2bt/datamodel.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.0/prosperity2bt/resources/round0/prices_round_0_day_-2.csv` & `prosperity2bt-0.4.1/prosperity2bt/resources/round0/prices_round_0_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.0/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv` & `prosperity2bt-0.4.1/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.0/prosperity2bt/resources/round1/prices_round_1_day_-1.csv` & `prosperity2bt-0.4.1/prosperity2bt/resources/round1/prices_round_1_day_-1.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.0/prosperity2bt/resources/round1/prices_round_1_day_-2.csv` & `prosperity2bt-0.4.1/prosperity2bt/resources/round1/prices_round_1_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.0/prosperity2bt/resources/round1/prices_round_1_day_0.csv` & `prosperity2bt-0.4.1/prosperity2bt/resources/round1/prices_round_1_day_0.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.0/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv` & `prosperity2bt-0.4.1/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.0/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv` & `prosperity2bt-0.4.1/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.0/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv` & `prosperity2bt-0.4.1/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.0/prosperity2bt.egg-info/PKG-INFO` & `prosperity2bt-0.4.1/prosperity2bt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.4.0
+Version: 0.4.1
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
 
-Orders placed by `Trader.run` at a given timestamp are matched against the order depths and market trades of that timestamp's state. Order depths take priority, if an order can be filled completely using volume in the relevant order depth, market trades are not considered. If not, the backtester matches your order against the timestamp's market trades. In this case the backtester assumes that for each trade, the buyer and the seller of the trade are willing to trade with you instead at the trade's price and volume. Your orders are matched at the price of your orders, e.g. if you place a sell order for €9 and there is a market trade for €10, the sell order is matched at €9 (even though there is a buyer willing to pay €10, this appears to be consistent with what the official Prosperity environment does).
+Orders placed by `Trader.run` at a given timestamp are matched against the order depths and market trades of that timestamp's state. Order depths take priority, if an order can be filled completely using volume in the relevant order depth, market trades are not considered. If not, the backtester matches your order against the timestamp's market trades. In this case the backtester assumes that for each trade, the buyer and the seller of the trade are willing to trade with you instead at the trade's price and volume. Market trades are matched at the price of your orders, e.g. if you place a sell order for €9 and there is a market trade for €10, the sell order is matched at €9 (even though there is a buyer willing to pay €10, this appears to be consistent with what the official Prosperity environment does).
 
 Limits are enforced before orders are matched to order depths. If for a product your position would exceed the limit, assuming all your orders would get filled, all your orders for that product get canceled.
 
 ## Development
 
 If you want to make changes to the backtester, clone (or fork and clone) this repository and run `pip install -e .` in the project's root. This installs the project in editable mode, so any changes you make are automatically taken into account the next time you run `prosperity2bt`.
```

### Comparing `prosperity2bt-0.4.0/prosperity2bt.egg-info/SOURCES.txt` & `prosperity2bt-0.4.1/prosperity2bt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.0/pyproject.toml` & `prosperity2bt-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prosperity2bt"
 description = "Backtester for IMC Prosperity 2 algorithms"
-version = "0.4.0"
+version = "0.4.1"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [{name = "Jasper van Merle", email = "jaspervmerle@gmail.com"}]
 keywords = ["imc", "prosperity", "backtest", "backtester"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

