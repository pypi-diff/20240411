# Comparing `tmp/galapy_core-0.1.1.tar.gz` & `tmp/galapy_core-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galapy_core-0.1.1.tar", max compression
+gzip compressed data, was "galapy_core-0.1.2.tar", max compression
```

## Comparing `galapy_core-0.1.1.tar` & `galapy_core-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2024-04-10 02:38:11.989631 galapy_core-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-10 02:40:16.917509 galapy_core-0.1.1/galapy_core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 02:40:16.924086 galapy_core-0.1.1/galapy_core/accounts.py
--rw-r--r--   0        0        0    19258 2024-04-11 18:47:25.035325 galapy_core-0.1.1/galapy_core/assets.py
--rw-r--r--   0        0        0      971 2024-04-11 19:08:29.053181 galapy_core-0.1.1/galapy_core/core.py
--rw-r--r--   0        0        0      160 2024-04-11 18:34:19.554350 galapy_core-0.1.1/galapy_core/generators/README.md
--rw-r--r--   0        0        0       34 2024-04-11 18:08:11.489360 galapy_core-0.1.1/galapy_core/generators/__init__.py
--rw-r--r--   0        0        0     1601 2024-04-11 18:34:30.553299 galapy_core-0.1.1/galapy_core/generators/price.py
--rw-r--r--   0        0        0     1219 2024-04-10 04:08:01.496749 galapy_core-0.1.1/galapy_core/generators.py
--rw-r--r--   0        0        0    12575 2024-04-10 04:09:23.792177 galapy_core-0.1.1/galapy_core/handlers.py
--rw-r--r--   0        0        0     7141 2024-04-11 19:05:22.667607 galapy_core-0.1.1/galapy_core/market_data.py
--rw-r--r--   0        0        0     9499 2024-04-11 19:07:14.900484 galapy_core-0.1.1/galapy_core/metrics.py
--rw-r--r--   0        0        0     8142 2024-04-11 19:07:36.802779 galapy_core-0.1.1/galapy_core/orders.py
--rw-r--r--   0        0        0    11285 2024-04-11 18:17:58.304006 galapy_core-0.1.1/galapy_core/portfolio.py
--rw-r--r--   0        0        0      484 2024-04-11 19:05:13.410144 galapy_core-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      587 1970-01-01 00:00:00.000000 galapy_core-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-10 02:38:11.989631 galapy_core-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-10 02:40:16.917509 galapy_core-0.1.2/galapy_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 02:40:16.924086 galapy_core-0.1.2/galapy_core/accounts.py
+-rw-r--r--   0        0        0    19258 2024-04-11 18:47:25.035325 galapy_core-0.1.2/galapy_core/assets.py
+-rw-r--r--   0        0        0      971 2024-04-11 19:53:15.372470 galapy_core-0.1.2/galapy_core/core.py
+-rw-r--r--   0        0        0      160 2024-04-11 18:34:19.554350 galapy_core-0.1.2/galapy_core/generators/README.md
+-rw-r--r--   0        0        0       34 2024-04-11 18:08:11.489360 galapy_core-0.1.2/galapy_core/generators/__init__.py
+-rw-r--r--   0        0        0     1601 2024-04-11 18:34:30.553299 galapy_core-0.1.2/galapy_core/generators/price.py
+-rw-r--r--   0        0        0     1219 2024-04-10 04:08:01.496749 galapy_core-0.1.2/galapy_core/generators.py
+-rw-r--r--   0        0        0    12575 2024-04-10 04:09:23.792177 galapy_core-0.1.2/galapy_core/handlers.py
+-rw-r--r--   0        0        0     7141 2024-04-11 19:05:22.667607 galapy_core-0.1.2/galapy_core/market_data.py
+-rw-r--r--   0        0        0     9499 2024-04-11 19:07:14.900484 galapy_core-0.1.2/galapy_core/metrics.py
+-rw-r--r--   0        0        0     8142 2024-04-11 19:07:36.802779 galapy_core-0.1.2/galapy_core/orders.py
+-rw-r--r--   0        0        0    11285 2024-04-11 18:17:58.304006 galapy_core-0.1.2/galapy_core/portfolio.py
+-rw-r--r--   0        0        0      485 2024-04-11 19:56:22.022760 galapy_core-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 galapy_core-0.1.2/PKG-INFO
```

### Comparing `galapy_core-0.1.1/galapy_core/assets.py` & `galapy_core-0.1.2/galapy_core/assets.py`

 * *Files identical despite different names*

### Comparing `galapy_core-0.1.1/galapy_core/core.py` & `galapy_core-0.1.2/galapy_core/core.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,18 @@
         return MarketDataClient()
 
     @property
     def metrics(self) -> "MetricClient":
         return MetricClient()
 
     @property
+    def portfolio(self) -> PortfolioClient:
+        return PortfolioClient()
+
+    @property
     def account(self):
         pass
 
     @property
     def order(self):
         pass
 
@@ -32,18 +36,14 @@
         pass
 
     @property
     def wallet(self):
         pass
 
     @property
-    def portfolio(self) -> PortfolioClient:
-        return PortfolioClient()
-
-    @property
     def defi(self):
         pass
 
 
 def main():
     backroom = GalaxyBackroom()
     # backroom.assets.add_asset()
```

### Comparing `galapy_core-0.1.1/galapy_core/generators/price.py` & `galapy_core-0.1.2/galapy_core/generators/price.py`

 * *Files identical despite different names*

### Comparing `galapy_core-0.1.1/galapy_core/generators.py` & `galapy_core-0.1.2/galapy_core/generators.py`

 * *Files identical despite different names*

### Comparing `galapy_core-0.1.1/galapy_core/handlers.py` & `galapy_core-0.1.2/galapy_core/handlers.py`

 * *Files identical despite different names*

### Comparing `galapy_core-0.1.1/galapy_core/market_data.py` & `galapy_core-0.1.2/galapy_core/market_data.py`

 * *Files identical despite different names*

### Comparing `galapy_core-0.1.1/galapy_core/metrics.py` & `galapy_core-0.1.2/galapy_core/metrics.py`

 * *Files identical despite different names*

### Comparing `galapy_core-0.1.1/galapy_core/orders.py` & `galapy_core-0.1.2/galapy_core/orders.py`

 * *Files identical despite different names*

### Comparing `galapy_core-0.1.1/galapy_core/portfolio.py` & `galapy_core-0.1.2/galapy_core/portfolio.py`

 * *Files identical despite different names*

### Comparing `galapy_core-0.1.1/PKG-INFO` & `galapy_core-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: galapy-core
-Version: 0.1.1
+Version: 0.1.2
 Summary: The backend and DB interactive layer for the GalaPy project
 Author: Kevin Hill
 Author-email: kivo360@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: ccxt (>=4.2.93,<5.0.0)
 Requires-Dist: decorator (>=5.1.1,<6.0.0)
 Requires-Dist: devtools (>=0.12.2,<0.13.0)
 Requires-Dist: faker (>=24.8.0,<25.0.0)
 Requires-Dist: stochastic (>=0.7.0,<0.8.0)
-Requires-Dist: supamodel (==0.4.9)
+Requires-Dist: supamodel (>=0.5.0,<0.6.0)
 Description-Content-Type: text/markdown
```

