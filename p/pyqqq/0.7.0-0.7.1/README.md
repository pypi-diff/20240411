# Comparing `tmp/pyqqq-0.7.0.tar.gz` & `tmp/pyqqq-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq-0.7.0.tar", max compression
+gzip compressed data, was "pyqqq-0.7.1.tar", max compression
```

## Comparing `pyqqq-0.7.0.tar` & `pyqqq-0.7.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.7.0/README.md
--rw-r--r--   0        0        0      770 2024-04-11 03:47:28.860737 pyqqq-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      591 2024-03-22 09:17:58.927909 pyqqq-0.7.0/pyqqq/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.7.0/pyqqq/brokerage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.7.0/pyqqq/brokerage/ebest/__init__.py
--rw-r--r--   0        0        0    39030 2024-04-04 06:07:52.832635 pyqqq-0.7.0/pyqqq/brokerage/ebest/domestic_stock.py
--rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.7.0/pyqqq/brokerage/ebest/oauth.py
--rw-r--r--   0        0        0    24011 2024-04-11 03:47:21.485388 pyqqq-0.7.0/pyqqq/brokerage/ebest/simple.py
--rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.7.0/pyqqq/brokerage/ebest/tr_client.py
--rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.7.0/pyqqq/brokerage/kis/__init__.py
--rw-r--r--   0        0        0   187461 2024-04-04 05:49:48.946800 pyqqq-0.7.0/pyqqq/brokerage/kis/domestic_stock.py
--rw-r--r--   0        0        0     5319 2024-03-22 09:17:58.928711 pyqqq-0.7.0/pyqqq/brokerage/kis/oauth.py
--rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.7.0/pyqqq/brokerage/kis/overseas_stock.py
--rw-r--r--   0        0        0    24359 2024-04-11 03:46:13.044337 pyqqq-0.7.0/pyqqq/brokerage/kis/simple.py
--rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.7.0/pyqqq/brokerage/kis/tr_client.py
--rw-r--r--   0        0        0      437 2024-03-25 05:15:17.008929 pyqqq-0.7.0/pyqqq/config.py
--rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.7.0/pyqqq/data/__init__.py
--rw-r--r--   0        0        0     4156 2024-04-01 05:25:31.374959 pyqqq-0.7.0/pyqqq/data/daily.py
--rw-r--r--   0        0        0     6546 2024-04-09 03:46:33.909510 pyqqq-0.7.0/pyqqq/data/domestic.py
--rw-r--r--   0        0        0     7289 2024-04-04 05:56:05.786196 pyqqq-0.7.0/pyqqq/data/realtime.py
--rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.7.0/pyqqq/datatypes.py
--rw-r--r--   0        0        0        0 2024-03-07 01:02:36.878098 pyqqq-0.7.0/pyqqq/utils/__init__.py
--rw-r--r--   0        0        0      951 2024-04-09 08:23:47.157710 pyqqq-0.7.0/pyqqq/utils/array.py
--rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.7.0/pyqqq/utils/display.py
--rw-r--r--   0        0        0     3963 2024-03-12 02:15:43.150036 pyqqq-0.7.0/pyqqq/utils/kvstore.py
--rw-r--r--   0        0        0     1511 2024-02-26 08:31:21.240645 pyqqq-0.7.0/pyqqq/utils/limiter.py
--rw-r--r--   0        0        0     1070 2024-03-22 09:17:58.929708 pyqqq-0.7.0/pyqqq/utils/logger.py
--rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.7.0/pyqqq/utils/market_schedule.py
--rw-r--r--   0        0        0     1425 2024-02-26 08:29:26.774617 pyqqq-0.7.0/pyqqq/utils/retry.py
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.7.1/README.md
+-rw-r--r--   0        0        0      770 2024-04-11 04:26:19.637148 pyqqq-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      591 2024-03-22 09:17:58.927909 pyqqq-0.7.1/pyqqq/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.7.1/pyqqq/brokerage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.7.1/pyqqq/brokerage/ebest/__init__.py
+-rw-r--r--   0        0        0    39030 2024-04-04 06:07:52.832635 pyqqq-0.7.1/pyqqq/brokerage/ebest/domestic_stock.py
+-rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.7.1/pyqqq/brokerage/ebest/oauth.py
+-rw-r--r--   0        0        0    24219 2024-04-11 04:25:37.648517 pyqqq-0.7.1/pyqqq/brokerage/ebest/simple.py
+-rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.7.1/pyqqq/brokerage/ebest/tr_client.py
+-rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.7.1/pyqqq/brokerage/kis/__init__.py
+-rw-r--r--   0        0        0   187461 2024-04-04 05:49:48.946800 pyqqq-0.7.1/pyqqq/brokerage/kis/domestic_stock.py
+-rw-r--r--   0        0        0     5319 2024-03-22 09:17:58.928711 pyqqq-0.7.1/pyqqq/brokerage/kis/oauth.py
+-rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.7.1/pyqqq/brokerage/kis/overseas_stock.py
+-rw-r--r--   0        0        0    24359 2024-04-11 03:46:13.044337 pyqqq-0.7.1/pyqqq/brokerage/kis/simple.py
+-rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.7.1/pyqqq/brokerage/kis/tr_client.py
+-rw-r--r--   0        0        0      437 2024-03-25 05:15:17.008929 pyqqq-0.7.1/pyqqq/config.py
+-rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.7.1/pyqqq/data/__init__.py
+-rw-r--r--   0        0        0     4156 2024-04-01 05:25:31.374959 pyqqq-0.7.1/pyqqq/data/daily.py
+-rw-r--r--   0        0        0     6546 2024-04-09 03:46:33.909510 pyqqq-0.7.1/pyqqq/data/domestic.py
+-rw-r--r--   0        0        0     7289 2024-04-04 05:56:05.786196 pyqqq-0.7.1/pyqqq/data/realtime.py
+-rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.7.1/pyqqq/datatypes.py
+-rw-r--r--   0        0        0        0 2024-03-07 01:02:36.878098 pyqqq-0.7.1/pyqqq/utils/__init__.py
+-rw-r--r--   0        0        0      951 2024-04-09 08:23:47.157710 pyqqq-0.7.1/pyqqq/utils/array.py
+-rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.7.1/pyqqq/utils/display.py
+-rw-r--r--   0        0        0     3963 2024-03-12 02:15:43.150036 pyqqq-0.7.1/pyqqq/utils/kvstore.py
+-rw-r--r--   0        0        0     1511 2024-02-26 08:31:21.240645 pyqqq-0.7.1/pyqqq/utils/limiter.py
+-rw-r--r--   0        0        0     1070 2024-03-22 09:17:58.929708 pyqqq-0.7.1/pyqqq/utils/logger.py
+-rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.7.1/pyqqq/utils/market_schedule.py
+-rw-r--r--   0        0        0     1425 2024-02-26 08:29:26.774617 pyqqq-0.7.1/pyqqq/utils/retry.py
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.7.1/PKG-INFO
```

### Comparing `pyqqq-0.7.0/README.md` & `pyqqq-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.0/pyproject.toml` & `pyqqq-0.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyqqq"
-version = "0.7.0"
+version = "0.7.1"
 description = "Package for quantitative strategy development on the PyQQQ platform"
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pyqqq"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
```

### Comparing `pyqqq-0.7.0/pyqqq/__init__.py` & `pyqqq-0.7.1/pyqqq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.0/pyqqq/brokerage/ebest/domestic_stock.py` & `pyqqq-0.7.1/pyqqq/brokerage/ebest/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.0/pyqqq/brokerage/ebest/oauth.py` & `pyqqq-0.7.1/pyqqq/brokerage/ebest/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.0/pyqqq/brokerage/ebest/simple.py` & `pyqqq-0.7.1/pyqqq/brokerage/ebest/simple.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,24 +98,33 @@
             - total_balance (int): 총 평가 금액
             - purchase_amount (int): 매입 금액
             - evaluated_amount (int): 평가 금액
             - pnl_amount (int): 손익 금액
             - pnl_rate (Decimal): 손익률
         """
 
-        r = self.stock_api.get_account_deposit_orderable_total_evaluation()
+        r = self.stock_api.get_stock_balance()
 
-        data = r["output2"]
+        data = r["output1"]
+
+        purchase_amount = data["mamt"]
+        evaluated_amount = data["tappamt"]
+        pnl_amount = data["tdtsunik"]
+        pnl_rate = (
+            Decimal(pnl_amount / purchase_amount * 100)
+            if purchase_amount != 0
+            else Decimal(0)
+        )
 
         result = {
-            "total_balance": data["DpsastTotamt"],
-            "purchase_amount": data["InvstOrgAmt"],
-            "evaluated_amount": data["BalEvalAmt"],
-            "pnl_amount": data["InvstPlAmt"],
-            "pnl_rate": Decimal(data["PnlRat"]),
+            "total_balance": data["sunamt"],
+            "purchase_amount": purchase_amount,
+            "evaluated_amount": evaluated_amount,
+            "pnl_amount": pnl_amount,
+            "pnl_rate": pnl_rate,
         }
         return result
 
     def get_possible_quantity(
         self, asset_code: str, order_type: OrderType = OrderType.MARKET, price: int = 0
     ) -> dict:
         """
```

### Comparing `pyqqq-0.7.0/pyqqq/brokerage/ebest/tr_client.py` & `pyqqq-0.7.1/pyqqq/brokerage/ebest/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.0/pyqqq/brokerage/kis/domestic_stock.py` & `pyqqq-0.7.1/pyqqq/brokerage/kis/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.0/pyqqq/brokerage/kis/oauth.py` & `pyqqq-0.7.1/pyqqq/brokerage/kis/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.0/pyqqq/brokerage/kis/overseas_stock.py` & `pyqqq-0.7.1/pyqqq/brokerage/kis/overseas_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.0/pyqqq/brokerage/kis/simple.py` & `pyqqq-0.7.1/pyqqq/brokerage/kis/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.0/pyqqq/brokerage/kis/tr_client.py` & `pyqqq-0.7.1/pyqqq/brokerage/kis/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.0/pyqqq/data/daily.py` & `pyqqq-0.7.1/pyqqq/data/daily.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.0/pyqqq/data/domestic.py` & `pyqqq-0.7.1/pyqqq/data/domestic.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.0/pyqqq/data/realtime.py` & `pyqqq-0.7.1/pyqqq/data/realtime.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.0/pyqqq/datatypes.py` & `pyqqq-0.7.1/pyqqq/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.0/pyqqq/utils/array.py` & `pyqqq-0.7.1/pyqqq/utils/array.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.0/pyqqq/utils/display.py` & `pyqqq-0.7.1/pyqqq/utils/display.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.0/pyqqq/utils/kvstore.py` & `pyqqq-0.7.1/pyqqq/utils/kvstore.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.0/pyqqq/utils/limiter.py` & `pyqqq-0.7.1/pyqqq/utils/limiter.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.0/pyqqq/utils/logger.py` & `pyqqq-0.7.1/pyqqq/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.0/pyqqq/utils/market_schedule.py` & `pyqqq-0.7.1/pyqqq/utils/market_schedule.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.0/pyqqq/utils/retry.py` & `pyqqq-0.7.1/pyqqq/utils/retry.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.0/PKG-INFO` & `pyqqq-0.7.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqqq
-Version: 0.7.0
+Version: 0.7.1
 Summary: Package for quantitative strategy development on the PyQQQ platform
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

