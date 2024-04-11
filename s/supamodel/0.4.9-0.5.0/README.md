# Comparing `tmp/supamodel-0.4.9.tar.gz` & `tmp/supamodel-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supamodel-0.4.9.tar", max compression
+gzip compressed data, was "supamodel-0.5.0.tar", max compression
```

## Comparing `supamodel-0.4.9.tar` & `supamodel-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     3741 2024-04-10 02:14:13.207577 supamodel-0.4.9/README.md
--rw-r--r--   0        0        0      851 2024-04-11 19:04:03.379112 supamodel-0.4.9/pyproject.toml
--rw-r--r--   0        0        0      190 2024-04-10 06:14:30.018688 supamodel-0.4.9/supamodel/__init__.py
--rw-r--r--   0        0        0     8349 2024-04-10 01:39:15.607798 supamodel-0.4.9/supamodel/_abc.py
--rw-r--r--   0        0        0      291 2024-04-11 18:39:05.846694 supamodel-0.4.9/supamodel/_client.py
--rw-r--r--   0        0        0     8016 2024-04-11 18:59:20.927159 supamodel-0.4.9/supamodel/_core.py
--rw-r--r--   0        0        0      674 2024-04-11 18:39:19.350451 supamodel-0.4.9/supamodel/_logging.py
--rw-r--r--   0        0        0      335 2024-04-10 02:17:30.714990 supamodel-0.4.9/supamodel/_types.py
--rw-r--r--   0        0        0     1488 2024-04-11 18:28:24.659195 supamodel-0.4.9/supamodel/config.py
--rw-r--r--   0        0        0     2284 2024-04-09 21:21:46.805022 supamodel-0.4.9/supamodel/enums.py
--rw-r--r--   0        0        0      321 2024-04-09 17:20:12.482160 supamodel-0.4.9/supamodel/errors.py
--rw-r--r--   0        0        0     1432 2024-04-10 01:57:59.819676 supamodel-0.4.9/supamodel/exceptions.py
--rw-r--r--   0        0        0     8307 2024-04-09 23:43:15.347009 supamodel-0.4.9/supamodel/supa.py
--rw-r--r--   0        0        0     4187 2024-04-10 02:22:32.745766 supamodel-0.4.9/supamodel/supa_builder.py
--rw-r--r--   0        0        0        0 2024-04-09 16:50:35.833946 supamodel-0.4.9/supamodel/trading/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 21:29:20.829143 supamodel-0.4.9/supamodel/trading/assets.py
--rw-r--r--   0        0        0     3690 2024-04-09 21:24:42.417053 supamodel-0.4.9/supamodel/trading/clock.py
--rw-r--r--   0        0        0     3436 2024-04-09 21:20:23.128058 supamodel-0.4.9/supamodel/trading/exchange.py
--rw-r--r--   0        0        0     1347 2024-04-09 21:21:25.286277 supamodel-0.4.9/supamodel/trading/market_data.py
--rw-r--r--   0        0        0     1865 2024-04-10 01:01:58.246531 supamodel-0.4.9/supamodel/trading/order_management.py
--rw-r--r--   0        0        0     1832 2024-04-10 01:02:12.075303 supamodel-0.4.9/supamodel/trading/portfolio.py
--rw-r--r--   0        0        0    11288 2024-04-11 18:47:56.777606 supamodel-0.4.9/supamodel/trading/tokens.py
--rw-r--r--   0        0        0    14903 2024-04-10 02:26:32.677556 supamodel-0.4.9/supamodel/utils.py
--rw-r--r--   0        0        0     4757 1970-01-01 00:00:00.000000 supamodel-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0     3741 2024-04-10 02:14:13.207577 supamodel-0.5.0/README.md
+-rw-r--r--   0        0        0      851 2024-04-11 19:20:46.296213 supamodel-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      190 2024-04-10 06:14:30.018688 supamodel-0.5.0/supamodel/__init__.py
+-rw-r--r--   0        0        0     8349 2024-04-10 01:39:15.607798 supamodel-0.5.0/supamodel/_abc.py
+-rw-r--r--   0        0        0      291 2024-04-11 18:39:05.846694 supamodel-0.5.0/supamodel/_client.py
+-rw-r--r--   0        0        0     8016 2024-04-11 18:59:20.927159 supamodel-0.5.0/supamodel/_core.py
+-rw-r--r--   0        0        0      674 2024-04-11 18:39:19.350451 supamodel-0.5.0/supamodel/_logging.py
+-rw-r--r--   0        0        0      335 2024-04-10 02:17:30.714990 supamodel-0.5.0/supamodel/_types.py
+-rw-r--r--   0        0        0     1488 2024-04-11 18:28:24.659195 supamodel-0.5.0/supamodel/config.py
+-rw-r--r--   0        0        0     2284 2024-04-09 21:21:46.805022 supamodel-0.5.0/supamodel/enums.py
+-rw-r--r--   0        0        0      321 2024-04-09 17:20:12.482160 supamodel-0.5.0/supamodel/errors.py
+-rw-r--r--   0        0        0     1432 2024-04-10 01:57:59.819676 supamodel-0.5.0/supamodel/exceptions.py
+-rw-r--r--   0        0        0     8307 2024-04-09 23:43:15.347009 supamodel-0.5.0/supamodel/supa.py
+-rw-r--r--   0        0        0     4187 2024-04-10 02:22:32.745766 supamodel-0.5.0/supamodel/supa_builder.py
+-rw-r--r--   0        0        0        0 2024-04-09 16:50:35.833946 supamodel-0.5.0/supamodel/trading/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 21:29:20.829143 supamodel-0.5.0/supamodel/trading/assets.py
+-rw-r--r--   0        0        0     3690 2024-04-09 21:24:42.417053 supamodel-0.5.0/supamodel/trading/clock.py
+-rw-r--r--   0        0        0     3436 2024-04-11 19:20:04.370291 supamodel-0.5.0/supamodel/trading/exchange.py
+-rw-r--r--   0        0        0     1337 2024-04-11 19:19:55.875484 supamodel-0.5.0/supamodel/trading/market_data.py
+-rw-r--r--   0        0        0     1865 2024-04-10 01:01:58.246531 supamodel-0.5.0/supamodel/trading/order_management.py
+-rw-r--r--   0        0        0     1832 2024-04-10 01:02:12.075303 supamodel-0.5.0/supamodel/trading/portfolio.py
+-rw-r--r--   0        0        0    11288 2024-04-11 18:47:56.777606 supamodel-0.5.0/supamodel/trading/tokens.py
+-rw-r--r--   0        0        0    14903 2024-04-10 02:26:32.677556 supamodel-0.5.0/supamodel/utils.py
+-rw-r--r--   0        0        0     4757 1970-01-01 00:00:00.000000 supamodel-0.5.0/PKG-INFO
```

### Comparing `supamodel-0.4.9/README.md` & `supamodel-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.9/pyproject.toml` & `supamodel-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "supamodel"
-version = "0.4.9"
+version = "0.5.0"
 description = "Pydantic Models for Trading Algos and Supabase"
 authors = ["Kevin Hill <kivo360@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<=3.11"
 pendulum = ">=2.0.0,<4.0.0"
```

### Comparing `supamodel-0.4.9/supamodel/_abc.py` & `supamodel-0.5.0/supamodel/_abc.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.9/supamodel/_core.py` & `supamodel-0.5.0/supamodel/_core.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.9/supamodel/_logging.py` & `supamodel-0.5.0/supamodel/_logging.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.9/supamodel/config.py` & `supamodel-0.5.0/supamodel/config.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.9/supamodel/enums.py` & `supamodel-0.5.0/supamodel/enums.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.9/supamodel/exceptions.py` & `supamodel-0.5.0/supamodel/exceptions.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.9/supamodel/supa.py` & `supamodel-0.5.0/supamodel/supa.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.9/supamodel/supa_builder.py` & `supamodel-0.5.0/supamodel/supa_builder.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.9/supamodel/trading/clock.py` & `supamodel-0.5.0/supamodel/trading/clock.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.9/supamodel/trading/exchange.py` & `supamodel-0.5.0/supamodel/trading/exchange.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.9/supamodel/trading/market_data.py` & `supamodel-0.5.0/supamodel/trading/market_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from datetime import datetime
 from typing import Any, Optional
 from uuid import UUID
 
 import pendulum as pdm
-from galapy.models.core import BaseModel, CamelModel, Data
-from microbots.birdeye.enums import TimeIntSQL
 from pydantic import Field, model_validator
 
+from supamodel._core import BaseModel, CamelModel, Data
+from supamodel.enums import TimeIntSQL
+
 
 def now_utc():
     return pdm.now("UTC")
 
 
 class PriceBar(CamelModel):
     address: str | None = Field(None, repr=False)
```

### Comparing `supamodel-0.4.9/supamodel/trading/order_management.py` & `supamodel-0.5.0/supamodel/trading/order_management.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.9/supamodel/trading/portfolio.py` & `supamodel-0.5.0/supamodel/trading/portfolio.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.9/supamodel/trading/tokens.py` & `supamodel-0.5.0/supamodel/trading/tokens.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.9/supamodel/utils.py` & `supamodel-0.5.0/supamodel/utils.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.9/PKG-INFO` & `supamodel-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supamodel
-Version: 0.4.9
+Version: 0.5.0
 Summary: Pydantic Models for Trading Algos and Supabase
 Author: Kevin Hill
 Author-email: kivo360@gmail.com
 Requires-Python: >=3.9,<=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

