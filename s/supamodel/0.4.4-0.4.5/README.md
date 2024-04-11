# Comparing `tmp/supamodel-0.4.4.tar.gz` & `tmp/supamodel-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supamodel-0.4.4.tar", max compression
+gzip compressed data, was "supamodel-0.4.5.tar", max compression
```

## Comparing `supamodel-0.4.4.tar` & `supamodel-0.4.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     3741 2024-04-10 02:14:13.207577 supamodel-0.4.4/README.md
--rw-r--r--   0        0        0      806 2024-04-10 02:42:03.257767 supamodel-0.4.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-09 16:17:58.633418 supamodel-0.4.4/supamodel/__init__.py
--rw-r--r--   0        0        0     8349 2024-04-10 01:39:15.607798 supamodel-0.4.4/supamodel/_abc.py
--rw-r--r--   0        0        0      291 2024-04-10 00:46:46.921212 supamodel-0.4.4/supamodel/_client.py
--rw-r--r--   0        0        0        0 2024-04-10 01:03:32.730144 supamodel-0.4.4/supamodel/_core.py
--rw-r--r--   0        0        0      646 2024-04-10 00:56:58.984128 supamodel-0.4.4/supamodel/_logging.py
--rw-r--r--   0        0        0      335 2024-04-10 02:17:30.714990 supamodel-0.4.4/supamodel/_types.py
--rw-r--r--   0        0        0     1484 2024-04-09 21:08:01.785026 supamodel-0.4.4/supamodel/config.py
--rw-r--r--   0        0        0     2284 2024-04-09 21:21:46.805022 supamodel-0.4.4/supamodel/enums.py
--rw-r--r--   0        0        0      321 2024-04-09 17:20:12.482160 supamodel-0.4.4/supamodel/errors.py
--rw-r--r--   0        0        0     1432 2024-04-10 01:57:59.819676 supamodel-0.4.4/supamodel/exceptions.py
--rw-r--r--   0        0        0     8307 2024-04-09 23:43:15.347009 supamodel-0.4.4/supamodel/supa.py
--rw-r--r--   0        0        0     4187 2024-04-10 02:22:32.745766 supamodel-0.4.4/supamodel/supa_builder.py
--rw-r--r--   0        0        0        0 2024-04-09 16:50:35.833946 supamodel-0.4.4/supamodel/trading/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 21:29:20.829143 supamodel-0.4.4/supamodel/trading/assets.py
--rw-r--r--   0        0        0     3690 2024-04-09 21:24:42.417053 supamodel-0.4.4/supamodel/trading/clock.py
--rw-r--r--   0        0        0     3436 2024-04-09 21:20:23.128058 supamodel-0.4.4/supamodel/trading/exchange.py
--rw-r--r--   0        0        0     1347 2024-04-09 21:21:25.286277 supamodel-0.4.4/supamodel/trading/market_data.py
--rw-r--r--   0        0        0     1865 2024-04-10 01:01:58.246531 supamodel-0.4.4/supamodel/trading/order_management.py
--rw-r--r--   0        0        0     1832 2024-04-10 01:02:12.075303 supamodel-0.4.4/supamodel/trading/portfolio.py
--rw-r--r--   0        0        0    11225 2024-04-10 02:41:43.253244 supamodel-0.4.4/supamodel/trading/tokens.py
--rw-r--r--   0        0        0    14903 2024-04-10 02:26:32.677556 supamodel-0.4.4/supamodel/utils.py
--rw-r--r--   0        0        0     4709 1970-01-01 00:00:00.000000 supamodel-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     3741 2024-04-10 02:14:13.207577 supamodel-0.4.5/README.md
+-rw-r--r--   0        0        0      826 2024-04-11 18:17:38.390312 supamodel-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0      190 2024-04-10 06:14:30.018688 supamodel-0.4.5/supamodel/__init__.py
+-rw-r--r--   0        0        0     8349 2024-04-10 01:39:15.607798 supamodel-0.4.5/supamodel/_abc.py
+-rw-r--r--   0        0        0      291 2024-04-10 00:46:46.921212 supamodel-0.4.5/supamodel/_client.py
+-rw-r--r--   0        0        0        0 2024-04-10 01:03:32.730144 supamodel-0.4.5/supamodel/_core.py
+-rw-r--r--   0        0        0      646 2024-04-10 00:56:58.984128 supamodel-0.4.5/supamodel/_logging.py
+-rw-r--r--   0        0        0      335 2024-04-10 02:17:30.714990 supamodel-0.4.5/supamodel/_types.py
+-rw-r--r--   0        0        0     1484 2024-04-09 21:08:01.785026 supamodel-0.4.5/supamodel/config.py
+-rw-r--r--   0        0        0     2284 2024-04-09 21:21:46.805022 supamodel-0.4.5/supamodel/enums.py
+-rw-r--r--   0        0        0      321 2024-04-09 17:20:12.482160 supamodel-0.4.5/supamodel/errors.py
+-rw-r--r--   0        0        0     1432 2024-04-10 01:57:59.819676 supamodel-0.4.5/supamodel/exceptions.py
+-rw-r--r--   0        0        0     8307 2024-04-09 23:43:15.347009 supamodel-0.4.5/supamodel/supa.py
+-rw-r--r--   0        0        0     4187 2024-04-10 02:22:32.745766 supamodel-0.4.5/supamodel/supa_builder.py
+-rw-r--r--   0        0        0        0 2024-04-09 16:50:35.833946 supamodel-0.4.5/supamodel/trading/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 21:29:20.829143 supamodel-0.4.5/supamodel/trading/assets.py
+-rw-r--r--   0        0        0     3690 2024-04-09 21:24:42.417053 supamodel-0.4.5/supamodel/trading/clock.py
+-rw-r--r--   0        0        0     3436 2024-04-09 21:20:23.128058 supamodel-0.4.5/supamodel/trading/exchange.py
+-rw-r--r--   0        0        0     1347 2024-04-09 21:21:25.286277 supamodel-0.4.5/supamodel/trading/market_data.py
+-rw-r--r--   0        0        0     1865 2024-04-10 01:01:58.246531 supamodel-0.4.5/supamodel/trading/order_management.py
+-rw-r--r--   0        0        0     1832 2024-04-10 01:02:12.075303 supamodel-0.4.5/supamodel/trading/portfolio.py
+-rw-r--r--   0        0        0    11288 2024-04-10 06:12:08.523415 supamodel-0.4.5/supamodel/trading/tokens.py
+-rw-r--r--   0        0        0    14903 2024-04-10 02:26:32.677556 supamodel-0.4.5/supamodel/utils.py
+-rw-r--r--   0        0        0     4751 1970-01-01 00:00:00.000000 supamodel-0.4.5/PKG-INFO
```

### Comparing `supamodel-0.4.4/README.md` & `supamodel-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.4/pyproject.toml` & `supamodel-0.4.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "supamodel"
-version = "0.4.4"
+version = "0.4.5"
 description = "Pydantic Models for Trading Algos and Supabase"
 authors = ["Kevin Hill <kivo360@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<=3.11"
 pendulum = ">=2.0.0,<4.0.0"
@@ -16,14 +16,15 @@
 inflector = "^3.1.1"
 supabase = "^2.4.1"
 pandas = "^2.2.1"
 solana = "^0.33.0"
 orjson = "^3.10.0"
 diskcache = "^5.6.3"
 typer = "^0.12.3"
+solders = "^0.21.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest-testmon = "^2.1.1"
 devtools = "^0.12.2"
 
 [build-system]
```

### Comparing `supamodel-0.4.4/supamodel/_abc.py` & `supamodel-0.4.5/supamodel/_abc.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.4/supamodel/_logging.py` & `supamodel-0.4.5/supamodel/_logging.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.4/supamodel/config.py` & `supamodel-0.4.5/supamodel/config.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.4/supamodel/enums.py` & `supamodel-0.4.5/supamodel/enums.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.4/supamodel/exceptions.py` & `supamodel-0.4.5/supamodel/exceptions.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.4/supamodel/supa.py` & `supamodel-0.4.5/supamodel/supa.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.4/supamodel/supa_builder.py` & `supamodel-0.4.5/supamodel/supa_builder.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.4/supamodel/trading/clock.py` & `supamodel-0.4.5/supamodel/trading/clock.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.4/supamodel/trading/exchange.py` & `supamodel-0.4.5/supamodel/trading/exchange.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.4/supamodel/trading/market_data.py` & `supamodel-0.4.5/supamodel/trading/market_data.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.4/supamodel/trading/order_management.py` & `supamodel-0.4.5/supamodel/trading/order_management.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.4/supamodel/trading/portfolio.py` & `supamodel-0.4.5/supamodel/trading/portfolio.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.4/supamodel/trading/tokens.py` & `supamodel-0.4.5/supamodel/trading/tokens.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,7 +323,15 @@
             _df.set_index("timestamp", inplace=True)
 
         return _df
 
     @computed_field
     def count(self) -> int:
         return len(self.data)
+
+
+def main():
+    pass
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `supamodel-0.4.4/supamodel/utils.py` & `supamodel-0.4.5/supamodel/utils.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.4/PKG-INFO` & `supamodel-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supamodel
-Version: 0.4.4
+Version: 0.4.5
 Summary: Pydantic Models for Trading Algos and Supabase
 Author: Kevin Hill
 Author-email: kivo360@gmail.com
 Requires-Python: >=3.9,<=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -16,14 +16,15 @@
 Requires-Dist: orjson (>=3.10.0,<4.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: pendulum (>=2.0.0,<4.0.0)
 Requires-Dist: pydantic (>=2.0.0,<=3.0.0)
 Requires-Dist: pydantic-settings (>=2.0.0,<=3.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: solana (>=0.33.0,<0.34.0)
+Requires-Dist: solders (>=0.21.0,<0.22.0)
 Requires-Dist: supabase (>=2.4.1,<3.0.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0)
 Description-Content-Type: text/markdown
 
 # SupaModel - Pydantic BaseModels and ORM for Supabase
 
 `SupaModel` is a Python package that provides `pydantic` BaseModels and ORM for `Supabase`. It is built on top of [supabase-py](https://supabase.com/docs/reference/python/start) and [pydantic](https://pydantic-docs.helpmanual.io/).
```

