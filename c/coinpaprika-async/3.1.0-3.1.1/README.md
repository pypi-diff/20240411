# Comparing `tmp/coinpaprika_async-3.1.0.tar.gz` & `tmp/coinpaprika_async-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coinpaprika_async-3.1.0.tar", max compression
+gzip compressed data, was "coinpaprika_async-3.1.1.tar", max compression
```

## Comparing `coinpaprika_async-3.1.0.tar` & `coinpaprika_async-3.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      537 2024-04-10 19:15:12.474999 coinpaprika_async-3.1.0/coinpaprika_async_client/__init__.py
--rw-r--r--   0        0        0      125 2024-04-10 07:39:36.455175 coinpaprika_async-3.1.0/coinpaprika_async_client/__version__.py
--rw-r--r--   0        0        0       62 2024-04-10 19:16:23.702687 coinpaprika_async-3.1.0/coinpaprika_async_client/client/__init__.py
--rw-r--r--   0        0        0     1415 2024-04-10 19:16:10.754193 coinpaprika_async-3.1.0/coinpaprika_async_client/client/coinpaprika_async_client.py
--rw-r--r--   0        0        0       43 2023-06-17 19:19:52.763805 coinpaprika_async-3.1.0/coinpaprika_async_client/coins/__init__.py
--rw-r--r--   0        0        0     6492 2024-04-10 19:17:36.999935 coinpaprika_async-3.1.0/coinpaprika_async_client/coins/api.py
--rw-r--r--   0        0        0     3032 2024-04-10 08:05:34.426767 coinpaprika_async-3.1.0/coinpaprika_async_client/coins/models.py
--rw-r--r--   0        0        0       43 2023-06-18 16:33:51.447490 coinpaprika_async-3.1.0/coinpaprika_async_client/exchanges/__init__.py
--rw-r--r--   0        0        0     1166 2024-04-10 19:17:11.487434 coinpaprika_async-3.1.0/coinpaprika_async_client/exchanges/api.py
--rw-r--r--   0        0        0     1322 2024-04-08 22:41:52.869451 coinpaprika_async-3.1.0/coinpaprika_async_client/exchanges/models.py
--rw-r--r--   0        0        0       43 2023-06-17 19:19:50.315267 coinpaprika_async-3.1.0/coinpaprika_async_client/key/__init__.py
--rw-r--r--   0        0        0      993 2024-04-10 19:18:22.652039 coinpaprika_async-3.1.0/coinpaprika_async_client/key/api.py
--rw-r--r--   0        0        0      351 2023-06-20 16:48:12.366887 coinpaprika_async-3.1.0/coinpaprika_async_client/key/models.py
--rw-r--r--   0        0        0       43 2023-06-17 19:19:39.258082 coinpaprika_async-3.1.0/coinpaprika_async_client/market/__init__.py
--rw-r--r--   0        0        0      453 2024-04-10 19:18:38.537515 coinpaprika_async-3.1.0/coinpaprika_async_client/market/api.py
--rw-r--r--   0        0        0      408 2023-06-20 16:48:12.366887 coinpaprika_async-3.1.0/coinpaprika_async_client/market/models.py
--rw-r--r--   0        0        0       43 2023-06-18 16:28:26.393731 coinpaprika_async-3.1.0/coinpaprika_async_client/misc/__init__.py
--rw-r--r--   0        0        0     3417 2024-04-10 19:18:49.157594 coinpaprika_async-3.1.0/coinpaprika_async_client/misc/api.py
--rw-r--r--   0        0        0     1457 2023-06-20 17:52:21.337155 coinpaprika_async-3.1.0/coinpaprika_async_client/misc/models.py
--rw-r--r--   0        0        0       62 2024-04-10 19:00:09.499127 coinpaprika_async-3.1.0/coinpaprika_async_client/networking_layer/__init__.py
--rw-r--r--   0        0        0     2803 2024-04-10 12:02:51.311704 coinpaprika_async-3.1.0/coinpaprika_async_client/networking_layer/http_async_client.py
--rw-r--r--   0        0        0      217 2023-06-20 17:03:37.194237 coinpaprika_async-3.1.0/coinpaprika_async_client/networking_layer/http_models.py
--rw-r--r--   0        0        0       43 2023-06-18 16:28:26.393731 coinpaprika_async-3.1.0/coinpaprika_async_client/people/__init__.py
--rw-r--r--   0        0        0     1271 2024-04-10 19:19:06.254703 coinpaprika_async-3.1.0/coinpaprika_async_client/people/api.py
--rw-r--r--   0        0        0      569 2023-06-20 18:13:19.881849 coinpaprika_async-3.1.0/coinpaprika_async_client/people/models.py
--rw-r--r--   0        0        0       43 2023-06-18 16:37:29.668193 coinpaprika_async-3.1.0/coinpaprika_async_client/tags/__init__.py
--rw-r--r--   0        0        0     1014 2024-04-10 19:19:13.806061 coinpaprika_async-3.1.0/coinpaprika_async_client/tags/api.py
--rw-r--r--   0        0        0      241 2023-06-20 20:03:04.015456 coinpaprika_async-3.1.0/coinpaprika_async_client/tags/models.py
--rw-r--r--   0        0        0       43 2023-06-17 19:19:52.763805 coinpaprika_async-3.1.0/coinpaprika_async_client/tickers/__init__.py
--rw-r--r--   0        0        0     2747 2024-04-10 19:19:22.052321 coinpaprika_async-3.1.0/coinpaprika_async_client/tickers/api.py
--rw-r--r--   0        0        0     1056 2023-06-20 17:15:14.018308 coinpaprika_async-3.1.0/coinpaprika_async_client/tickers/models.py
--rw-r--r--   0        0        0     1084 2023-05-21 17:45:15.267559 coinpaprika_async-3.1.0/LICENSE
--rw-r--r--   0        0        0     1220 2024-04-10 20:32:44.638165 coinpaprika_async-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     1346 2024-04-10 11:51:13.154098 coinpaprika_async-3.1.0/README.md
--rw-r--r--   0        0        0     1805 1970-01-01 00:00:00.000000 coinpaprika_async-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0      537 2024-04-10 19:15:12.474999 coinpaprika_async-3.1.1/coinpaprika_async_client/__init__.py
+-rw-r--r--   0        0        0      125 2024-04-10 07:39:36.455175 coinpaprika_async-3.1.1/coinpaprika_async_client/__version__.py
+-rw-r--r--   0        0        0       62 2024-04-10 19:16:23.702687 coinpaprika_async-3.1.1/coinpaprika_async_client/client/__init__.py
+-rw-r--r--   0        0        0     1415 2024-04-10 19:16:10.754193 coinpaprika_async-3.1.1/coinpaprika_async_client/client/coinpaprika_async_client.py
+-rw-r--r--   0        0        0       43 2023-06-17 19:19:52.763805 coinpaprika_async-3.1.1/coinpaprika_async_client/coins/__init__.py
+-rw-r--r--   0        0        0     6490 2024-04-10 21:18:47.990316 coinpaprika_async-3.1.1/coinpaprika_async_client/coins/api.py
+-rw-r--r--   0        0        0     3032 2024-04-10 08:05:34.426767 coinpaprika_async-3.1.1/coinpaprika_async_client/coins/models.py
+-rw-r--r--   0        0        0       43 2023-06-18 16:33:51.447490 coinpaprika_async-3.1.1/coinpaprika_async_client/exchanges/__init__.py
+-rw-r--r--   0        0        0     1164 2024-04-10 21:18:47.854681 coinpaprika_async-3.1.1/coinpaprika_async_client/exchanges/api.py
+-rw-r--r--   0        0        0     1322 2024-04-08 22:41:52.869451 coinpaprika_async-3.1.1/coinpaprika_async_client/exchanges/models.py
+-rw-r--r--   0        0        0       43 2023-06-17 19:19:50.315267 coinpaprika_async-3.1.1/coinpaprika_async_client/key/__init__.py
+-rw-r--r--   0        0        0      991 2024-04-10 21:18:47.875681 coinpaprika_async-3.1.1/coinpaprika_async_client/key/api.py
+-rw-r--r--   0        0        0      351 2023-06-20 16:48:12.366887 coinpaprika_async-3.1.1/coinpaprika_async_client/key/models.py
+-rw-r--r--   0        0        0       43 2023-06-17 19:19:39.258082 coinpaprika_async-3.1.1/coinpaprika_async_client/market/__init__.py
+-rw-r--r--   0        0        0      451 2024-04-10 21:18:47.873680 coinpaprika_async-3.1.1/coinpaprika_async_client/market/api.py
+-rw-r--r--   0        0        0      408 2023-06-20 16:48:12.366887 coinpaprika_async-3.1.1/coinpaprika_async_client/market/models.py
+-rw-r--r--   0        0        0       43 2023-06-18 16:28:26.393731 coinpaprika_async-3.1.1/coinpaprika_async_client/misc/__init__.py
+-rw-r--r--   0        0        0     3415 2024-04-10 21:18:47.995317 coinpaprika_async-3.1.1/coinpaprika_async_client/misc/api.py
+-rw-r--r--   0        0        0     1457 2023-06-20 17:52:21.337155 coinpaprika_async-3.1.1/coinpaprika_async_client/misc/models.py
+-rw-r--r--   0        0        0       62 2024-04-10 19:00:09.499127 coinpaprika_async-3.1.1/coinpaprika_async_client/networking_layer/__init__.py
+-rw-r--r--   0        0        0     2803 2024-04-10 12:02:51.311704 coinpaprika_async-3.1.1/coinpaprika_async_client/networking_layer/http_async_client.py
+-rw-r--r--   0        0        0      217 2023-06-20 17:03:37.194237 coinpaprika_async-3.1.1/coinpaprika_async_client/networking_layer/http_models.py
+-rw-r--r--   0        0        0       43 2023-06-18 16:28:26.393731 coinpaprika_async-3.1.1/coinpaprika_async_client/people/__init__.py
+-rw-r--r--   0        0        0     1269 2024-04-10 21:18:47.961315 coinpaprika_async-3.1.1/coinpaprika_async_client/people/api.py
+-rw-r--r--   0        0        0      569 2023-06-20 18:13:19.881849 coinpaprika_async-3.1.1/coinpaprika_async_client/people/models.py
+-rw-r--r--   0        0        0       43 2023-06-18 16:37:29.668193 coinpaprika_async-3.1.1/coinpaprika_async_client/tags/__init__.py
+-rw-r--r--   0        0        0     1012 2024-04-10 21:18:47.946316 coinpaprika_async-3.1.1/coinpaprika_async_client/tags/api.py
+-rw-r--r--   0        0        0      241 2023-06-20 20:03:04.015456 coinpaprika_async-3.1.1/coinpaprika_async_client/tags/models.py
+-rw-r--r--   0        0        0       43 2023-06-17 19:19:52.763805 coinpaprika_async-3.1.1/coinpaprika_async_client/tickers/__init__.py
+-rw-r--r--   0        0        0     2745 2024-04-10 21:18:48.059316 coinpaprika_async-3.1.1/coinpaprika_async_client/tickers/api.py
+-rw-r--r--   0        0        0     1056 2023-06-20 17:15:14.018308 coinpaprika_async-3.1.1/coinpaprika_async_client/tickers/models.py
+-rw-r--r--   0        0        0     1084 2023-05-21 17:45:15.267559 coinpaprika_async-3.1.1/LICENSE
+-rw-r--r--   0        0        0     1220 2024-04-10 21:42:17.809304 coinpaprika_async-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1346 2024-04-10 11:51:13.154098 coinpaprika_async-3.1.1/README.md
+-rw-r--r--   0        0        0     1805 1970-01-01 00:00:00.000000 coinpaprika_async-3.1.1/PKG-INFO
```

### Comparing `coinpaprika_async-3.1.0/coinpaprika_async_client/__init__.py` & `coinpaprika_async-3.1.1/coinpaprika_async_client/__init__.py`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.1.0/coinpaprika_async_client/client/coinpaprika_async_client.py` & `coinpaprika_async-3.1.1/coinpaprika_async_client/client/coinpaprika_async_client.py`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.1.0/coinpaprika_async_client/coins/api.py` & `coinpaprika_async-3.1.1/coinpaprika_async_client/coins/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from ..networking_layer import Result, ApiError
 
 from .models import *
 
 
 class CoinsEndpoint:
-
     def __init__(self) -> None:
         self.__internal = CoinPaprikaAsyncClient()
 
     async def get_all(self) -> ApiError | list[CoinItem]:
         res = await self.__internal.call_api("coins")
 
         if res.Error:
```

### Comparing `coinpaprika_async-3.1.0/coinpaprika_async_client/coins/models.py` & `coinpaprika_async-3.1.1/coinpaprika_async_client/coins/models.py`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.1.0/coinpaprika_async_client/exchanges/api.py` & `coinpaprika_async-3.1.1/coinpaprika_async_client/exchanges/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from ..networking_layer import ApiError
 
 from .models import *
 
 
 class ExchangesEndpoint:
-
     def __init__(self) -> None:
         self.__internal = CoinPaprikaAsyncClient()
 
     async def exchange_list(self, **params: Any) -> ApiError | list[Exchange]:
         res = await self.__internal.call_api("exchanges", **params)
 
         if res.Error:
```

### Comparing `coinpaprika_async-3.1.0/coinpaprika_async_client/exchanges/models.py` & `coinpaprika_async-3.1.1/coinpaprika_async_client/exchanges/models.py`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.1.0/coinpaprika_async_client/key/api.py` & `coinpaprika_async-3.1.1/coinpaprika_async_client/key/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from ..networking_layer import ApiError
 
 from .models import KeyInfo, APIUsage, CurrentMonthUsage
 
 
 class KeyEndpoint:
-
     def __init__(self) -> None:
         self.__internal = CoinPaprikaAsyncClient()
 
     async def get_key_info(self) -> ApiError | KeyInfo:
         res = await self.__internal.call_api("key/info")
 
         if res.Error:
```

### Comparing `coinpaprika_async-3.1.0/coinpaprika_async_client/misc/api.py` & `coinpaprika_async-3.1.1/coinpaprika_async_client/misc/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from ..networking_layer import ApiError
 
 from .models import *
 
 
 class MiscellaneousEndpoints:
-
     def __init__(self) -> None:
         self.__internal = CoinPaprikaAsyncClient()
 
     async def people(self, person_id: str) -> ApiError | list[PeopleItem]:
         res = await self.__internal.call_api(f"people/{person_id}")
 
         if res.Error:
```

### Comparing `coinpaprika_async-3.1.0/coinpaprika_async_client/misc/models.py` & `coinpaprika_async-3.1.1/coinpaprika_async_client/misc/models.py`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.1.0/coinpaprika_async_client/networking_layer/http_async_client.py` & `coinpaprika_async-3.1.1/coinpaprika_async_client/networking_layer/http_async_client.py`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.1.0/coinpaprika_async_client/people/api.py` & `coinpaprika_async-3.1.1/coinpaprika_async_client/people/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from ..networking_layer import ApiError
 
 from .models import *
 
 
 class PeopleEndpoint:
-
     def __init__(self) -> None:
         self.__internal = CoinPaprikaAsyncClient()
 
     async def people(self, person_id: str) -> ApiError | list[PeopleItem]:
         res = await self.__internal.call_api(f"people/{person_id}")
 
         if res.Error:
```

### Comparing `coinpaprika_async-3.1.0/coinpaprika_async_client/people/models.py` & `coinpaprika_async-3.1.1/coinpaprika_async_client/people/models.py`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.1.0/coinpaprika_async_client/tags/api.py` & `coinpaprika_async-3.1.1/coinpaprika_async_client/tags/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from ..networking_layer import ApiError
 
 from .models import *
 
 
 class TagsEndpoint:
-
     def __init__(self) -> None:
         self.__internal = CoinPaprikaAsyncClient()
 
     async def tags(
         self, additional_fields: Optional[str] = None
     ) -> ApiError | list[Tag]:
         res = await self.__internal.call_api(
```

### Comparing `coinpaprika_async-3.1.0/coinpaprika_async_client/tickers/api.py` & `coinpaprika_async-3.1.1/coinpaprika_async_client/tickers/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from ..networking_layer import ApiError
 
 from .models import *
 
 
 class TickersEndpoint:
-
     def __init__(self) -> None:
         self.__internal = CoinPaprikaAsyncClient()
 
     async def tickers(self, quotes: str = "USD") -> ApiError | list[TickerItem]:
         res = await self.__internal.call_api("tickers", quotes=quotes)
         if res.Error:
             return res.Error
```

### Comparing `coinpaprika_async-3.1.0/coinpaprika_async_client/tickers/models.py` & `coinpaprika_async-3.1.1/coinpaprika_async_client/tickers/models.py`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.1.0/LICENSE` & `coinpaprika_async-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.1.0/pyproject.toml` & `coinpaprika_async-3.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coinpaprika-async"
-version = "3.1.0"
+version = "3.1.1"
 description = "An asynchronous library for interacting with the Coinpaprika.com API, written with httpx in Python."
 authors = ["DroidZed <41507665+DroidZed@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "coinpaprika_async_client" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `coinpaprika_async-3.1.0/README.md` & `coinpaprika_async-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.1.0/PKG-INFO` & `coinpaprika_async-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinpaprika-async
-Version: 3.1.0
+Version: 3.1.1
 Summary: An asynchronous library for interacting with the Coinpaprika.com API, written with httpx in Python.
 Author: DroidZed
 Author-email: 41507665+DroidZed@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

